# Comparing `tmp/puepy-0.1.2.tar.gz` & `tmp/puepy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puepy-0.1.2.tar", max compression
+gzip compressed data, was "puepy-0.2.0.tar", max compression
```

## Comparing `puepy-0.1.2.tar` & `puepy-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     3040 2024-05-27 21:19:07.414163 puepy-0.1.2/README.md
--rw-r--r--   0        0        0       90 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/__init__.py
--rw-r--r--   0        0        0     2756 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/application.py
--rw-r--r--   0        0        0    21358 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/core.py
--rw-r--r--   0        0        0       84 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/errors.py
--rw-r--r--   0        0        0     2659 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/reactivity.py
--rw-r--r--   0        0        0     2893 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/router.py
--rw-r--r--   0        0        0     1390 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/runtime.py
--rw-r--r--   0        0        0     2211 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/storage.py
--rw-r--r--   0        0        0     4055 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/util.py
--rw-r--r--   0        0        0      466 2024-05-27 21:19:07.414163 puepy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 puepy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      550 2024-06-02 12:57:37.033800 puepy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3040 2024-06-02 12:57:37.033800 puepy-0.2.0/README.md
+-rw-r--r--   0        0        0       90 2024-06-02 12:57:37.033800 puepy-0.2.0/puepy/__init__.py
+-rw-r--r--   0        0        0     3046 2024-06-02 12:57:37.033800 puepy-0.2.0/puepy/application.py
+-rw-r--r--   0        0        0    22164 2024-06-02 12:57:37.037800 puepy-0.2.0/puepy/core.py
+-rw-r--r--   0        0        0       84 2024-06-02 12:57:37.037800 puepy-0.2.0/puepy/errors.py
+-rw-r--r--   0        0        0     2659 2024-06-02 12:57:37.037800 puepy-0.2.0/puepy/reactivity.py
+-rw-r--r--   0        0        0     4676 2024-06-02 12:57:37.037800 puepy-0.2.0/puepy/router.py
+-rw-r--r--   0        0        0     1390 2024-06-02 12:57:37.037800 puepy-0.2.0/puepy/runtime.py
+-rw-r--r--   0        0        0     2211 2024-06-02 12:57:37.037800 puepy-0.2.0/puepy/storage.py
+-rw-r--r--   0        0        0     4048 2024-06-02 12:57:37.037800 puepy-0.2.0/puepy/util.py
+-rw-r--r--   0        0        0      935 2024-06-02 12:57:37.037800 puepy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3989 1970-01-01 00:00:00.000000 puepy-0.2.0/PKG-INFO
```

### Comparing `puepy-0.1.2/README.md` & `puepy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `puepy-0.1.2/puepy/application.py` & `puepy-0.2.0/puepy/application.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from .runtime import is_server_side, add_event_listener, window, history, platform, PLATFORM_PYODIDE
-
-
-from .core import ReactiveDict, jsobj, Page
 from puepy.storage import BrowserStorage
+from .core import Page
+from .runtime import (
+    is_server_side,
+    add_event_listener,
+    window,
+    platform,
+    PLATFORM_PYODIDE,
+)
 
 
 class Application:
     def __init__(self):
-        self.ephemeral = ReactiveDict()
         if is_server_side:
             self.session_storage = None
             self.local_storage = None
         else:
             from js import localStorage, sessionStorage
 
             self.session_storage = BrowserStorage(sessionStorage, "session_storage")
             self.local_storage = BrowserStorage(localStorage, "local_storage")
         self.router = None
-        self.selector_or_element = None
+        self._selector_or_element = None
         self.default_page = None
-        if platform == PLATFORM_PYODIDE:
-            add_event_listener(window, "popstate", self.on_popstate)
-
-        self.enable_history_mode = True
 
     def install_router(self, router_class, **kwargs):
         self.router = router_class(application=self, **kwargs)
+        if platform == PLATFORM_PYODIDE:
+            add_event_listener(window, "popstate", self._on_popstate)
 
     def page(self, route=None, name=None):
         """
         Intended to be called as a secorator.
 
         app = Application()
         @app.page("/my-page")
@@ -49,42 +50,45 @@
 
             def decorator(func):
                 self.default_page = func
                 return func
 
             return decorator
 
-    def navigate_to_path(self, path):
-        if self.enable_history_mode:
-            history.pushState(jsobj(), "", path)
-            return self.mount(self.selector_or_element, path)
-        else:
-            window.location = path
-
-    def on_popstate(self, event):
-        self.mount(self.selector_or_element, window.location.pathname)
+    def _on_popstate(self, event):
+        if self.router.link_mode == self.router.LINK_MODE_HASH:
+            self.mount(self._selector_or_element, window.location.hash.split("#", 1)[-1])
+        elif self.router.link_mode in (self.router.LINK_MODE_DIRECT, self.router.LINK_MODE_HTML5):
+            self.mount(self._selector_or_element, window.location.pathname)
+
+    def mount(self, selector_or_element, path=None, page_kwargs=None):
+        if page_kwargs is None:
+            page_kwargs = {}
 
-    def mount(self, selector_or_element, path=None, **kwargs):
-        path = path or window.location.pathname
-
-        self.selector_or_element = selector_or_element
+        self._selector_or_element = selector_or_element
 
         if self.router:
+            if self.router.link_mode == self.router.LINK_MODE_HASH:
+                path = path or window.location.hash.split("#", 1)[-1]
+            elif self.router.link_mode in (self.router.LINK_MODE_DIRECT, self.router.LINK_MODE_HTML5):
+                path = path or window.location.pathname
+            else:
+                path = ""
             route, arguments = self.router.match(path)
             if arguments:
-                kwargs.update(arguments)
+                page_kwargs.update(arguments)
 
             if route:
                 page_class = route.page
             elif self.default_page:
                 page_class = self.default_page
             else:
                 return None
         elif self.default_page:
             route = None
             page_class = self.default_page
         else:
             return None
 
-        page: Page = page_class(router=self.router, matched_route=route, application=self, **kwargs)
+        page: Page = page_class(matched_route=route, application=self, **page_kwargs)
         page.mount(selector_or_element)
         return page
```

### Comparing `puepy-0.1.2/puepy/core.py` & `puepy-0.2.0/puepy/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,27 +38,38 @@
 class Tag:
     """
     A class that allows you to push and pop a context
     """
 
     stack = []
     population_stack = []
+    origin_stack = [[]]
     component_stack = []
     default_classes = []
     default_attrs = {}
     default_role = None
 
     document = document
 
-    def __init__(self, tag_name, ref, page: "Page" = None, parent=None, parent_component=None, children=None, **kwargs):
+    def __init__(
+        self,
+        tag_name,
+        ref,
+        page: "Page" = None,
+        parent=None,
+        parent_component=None,
+        origin=None,
+        children=None,
+        **kwargs,
+    ):
         self.added_event_listeners = []
         self._rendered_element = None
 
         self.children = []
-        self.children_by_ref = {}
+        self.refs = {}
         if children:
             self.add(*children)
 
         self.tag_name = tag_name
         self.ref = ref
 
         if isinstance(page, Page):
@@ -67,39 +78,49 @@
             self._page = self
         elif page:
             raise Exception(f"Unknown page type {type(page)}")
         else:
             raise Exception("No page passed")
 
         if isinstance(parent, Tag):
+            self.parent = parent
             parent.add(self)
         elif parent:
             raise Exception(f"Unknown parent type {type(parent)}: {repr(parent)}")
         else:
-            self._parent = None
+            self.parent = None
 
         if isinstance(parent_component, Component):
             self.parent_component = parent_component
         elif parent_component:
             raise Exception(f"Unknown parent_component type {type(parent_component)}: {repr(parent_component)}")
         else:
             self.parent_component = None
 
+        self.origin = origin
         self._children_generated = False
         self.destroyed = False
 
-        self._handle_kwargs(kwargs)
+        self._configure(kwargs)
 
-    def _handle_kwargs(self, kwargs):
+    def __del__(self):
+        if not is_server_side:
+            while self.added_event_listeners:
+                remove_event_listener(*self.added_event_listeners.pop())
+
+    @property
+    def application(self):
+        return self._page._application
+
+    def _configure(self, kwargs):
         self.event_handlers = _extract_event_handlers(kwargs)
         self._handle_bind(kwargs)
         self._handle_attrs(kwargs)
 
     def _handle_bind(self, kwargs):
-        self.bind_component = self.population_stack[-1] if self.population_stack else None
         if "bind" in kwargs:
             self.bind = kwargs.pop("bind")
             if "value" in kwargs:
                 raise Exception("Cannot specify both 'bind' and 'value'")
             if "on_input" in self.event_handlers:
                 raise Exception("Cannot specify both 'bind' and 'on_input'")
         else:
@@ -119,33 +140,41 @@
     def generate_children(self):
         """
         Runs populate, but first adds self to self.population_stack, and removes it after populate runs.
 
         That way, as populate is executed, self.population_stack can be used to figure out what the innermost populate()
         method is being run and thus, where to send bind= parameters.
         """
+        self.origin_stack.append([])
+        self._refs_pending_removal = self.refs.copy()
+        self.refs = {}
         self.population_stack.append(self)
         try:
             self.populate()
         finally:
             self.population_stack.pop()
+            self.origin_stack.pop()
 
     def render(self):
         if "xmlns" in self.attrs:
             element = self.document.createElementNS(self.attrs.get("xmlns"), self.tag_name)
         else:
             element = self.document.createElement(self.tag_name)
 
         element.setAttribute("id", self.element_id)
         if is_server_side:
             element.setIdAttribute("id")
 
         self._render_onto(element)
+        self.post_render(element)
         return element
 
+    def post_render(self, element):
+        pass
+
     @property
     def element_id(self):
         return self.attrs.get("id", f"e-{id(self)}")
 
     @property
     def element(self):
         el = self.document.getElementById(self.element_id)
@@ -179,36 +208,35 @@
                     element.setAttribute(attr.replace("_", "-"), value)
 
         if "role" not in self.attrs and self.default_role:
             element.setAttribute("role", self.default_role)
 
         # Add event handlers
         for key, value in self.event_handlers.items():
+            key = key.replace("_", "-")
             if isinstance(value, (list, tuple)):
                 for handler in value:
                     self._add_event_listener(element, key, handler)
             else:
                 self._add_event_listener(element, key, value)
 
         # Add bind
-
-        if self.bind and self.bind_component:
+        if self.bind and self.origin:
             if _element_input_type(element) == "checkbox":
-                if is_server_side and self.bind_component.state[self.bind]:
-                    element.setAttribute("checked", self.bind_component.state[self.bind])
+                if is_server_side and self.origin.state[self.bind]:
+                    element.setAttribute("checked", self.origin.state[self.bind])
                 else:
-                    element.checked = bool(self.bind_component.state[self.bind])
+                    element.checked = bool(self.origin.state[self.bind])
             else:
                 if is_server_side:
-                    element.setAttribute("value", self.bind_component.state[self.bind])
+                    element.setAttribute("value", self.origin.state[self.bind])
                 else:
-                    element.value = self.bind_component.state[self.bind]
+                    element.value = self.origin.state[self.bind]
 
             self._add_event_listener(element, "input", self.on_bind_input)
-
         elif self.bind:
             raise Exception("Cannot specify bind a valid parent component")
 
         self.render_children(element)
 
     def render_children(self, element):
         for child in self.children:
@@ -244,15 +272,15 @@
 
         Should probably not be used outside this class.
         """
         self.added_event_listeners.append((element, event, listener))
         if not is_server_side:
             add_event_listener(element, event, listener)
 
-    def add_event_handler(self, event, handler):
+    def add_event_listener(self, event, handler):
         if event not in self.event_handlers:
             self.event_handlers[event] = handler
         else:
             existing_handler = self.event_handlers[event]
             if isinstance(existing_handler, (list, tuple)):
                 self.event_handlers[event] = [existing_handler] + list(handler)
             else:
@@ -267,14 +295,17 @@
                 self.generate_children()
 
         if isinstance(selector_or_element, str):
             element = self.document.querySelector(selector_or_element)
         else:
             element = selector_or_element
 
+        if not element:
+            raise RuntimeError(f"Element {selector_or_element} not found")
+
         element.innerHTML = ""
         element.appendChild(self.render())
         self.recursive_call("ready")
 
     def recursive_call(self, method, *args, **kwargs):
         for child in self.children:
             if isinstance(child, Tag):
@@ -285,36 +316,55 @@
         pass
 
     def on_redraw(self):
         pass
 
     def on_bind_input(self, event):
         if _element_input_type(event.target) == "checkbox":
-            self.bind_component.state[self.bind] = event.target.checked
+            self.origin.state[self.bind] = event.target.checked
         else:
-            self.bind_component.state[self.bind] = event.target.value
+            self.origin.state[self.bind] = event.target.value
 
     @property
     def page(self):
         if self._page:
             return self._page
         elif isinstance(self, Page):
             return self
 
     @property
+    def router(self):
+        if self.application:
+            return self.application.router
+
+    @property
     def parent(self):
         return self._parent
 
+    @parent.setter
+    def parent(self, new_parent):
+        existing_parent = getattr(self, "_parent", None)
+        if new_parent == existing_parent:
+            if new_parent and self not in new_parent.children:
+                existing_parent.children.append(self)
+            return
+
+        if existing_parent and self in existing_parent.children:
+            existing_parent.children.remove(self)
+        if new_parent and self not in new_parent.children:
+            new_parent.children.append(self)
+
+        self._parent = new_parent
+
     def add(self, *children):
         for child in children:
             if isinstance(child, Tag):
-                self.children_by_ref[child.ref] = child
-                child._parent = self
-
-            self.children.append(child)
+                child.parent = self
+            else:
+                self.children.append(child)
 
     def print_tree(self, n=0):
         if n == 0:
             print("Tree")
         print("." * n, self)
         for child in self.children:
             if isinstance(child, Tag):
@@ -367,45 +417,21 @@
         if old_active_element_id is not None:
             el = self.document.getElementById(old_active_element_id)
             if el:
                 el.focus()
 
         self.recursive_call("on_redraw")
 
-    def destroy_orphans(self):
-        to_remove = []
-        for ref, child in self.children_by_ref.items():
-            if child not in self.children:
-                to_remove.append((ref, child))
-            child.destroy_orphans()
-        for ref, child in to_remove:
-            del self.children_by_ref[ref]
-            if isinstance(child, Tag):
-                child.destroy()
-
-    def destroy(self):
-        self.destroyed = True
-        if self in self.parent.children:
-            self.parent.children.remove(self)
-        if self.ref in self.parent.children_by_ref:
-            del self.parent.children_by_ref[self.ref]
-
-        while self.children:
-            child = self.children.pop()
-            if isinstance(child, Tag):
-                child.destroy()
-
-        if not is_server_side:
-            while self.added_event_listeners:
-                remove_event_listener(*self.added_event_listeners.pop())
-
     def trigger_redraw(self):
         self.page.redraw_tag(self)
 
     def trigger_event(self, event, detail=None, **kwargs):
+        if "_" in event:
+            print("Triggering event with underscores. Did you mean dashes?: ", event)
+
         from pyscript.ffi import to_js
         from js import Object, Map
 
         if detail:
             event_object = to_js({"detail": Map.new(Object.entries(to_js(detail)))})
         else:
             event_object = to_js({})
@@ -413,18 +439,20 @@
         self.element.dispatchEvent(CustomEvent.new(event, event_object))
 
     def update_title(self):
         pass
 
     def __enter__(self):
         self.stack.append(self)
+        self.origin_stack[0].append(self)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stack.pop()
+        self.origin_stack[0].pop()
         return False
 
     def __str__(self):
         return self.tag_name
 
     def __repr__(self):
         return f"<{self} ({id(self)})>"
@@ -493,56 +521,55 @@
                 self.trigger_redraw()
 
     def on_state_change(self, key, value):
         pass
 
     def insert_slot(self, name="default", **kwargs):
         if name in self.slots:
-            assert self.slots[name].page == self.page
-            assert self.slots[name].parent == Tag.stack[-1]
-            if self.slots[name] not in Tag.stack[-1].children:
-                Tag.stack[-1].children.append(self.slots[name])
-            Tag.stack[-1].children_by_ref[self.slots[name].ref] = self.slots[name]
-
-            # Moved this to slot()
-            # self.slots[name].children = []
+            self.slots[name].parent = Tag.stack[-1]  # The children will be cleared during redraw, so re-establish
         else:
             self.slots[name] = Slot(ref=f"slot={name}", slot_name=name, page=self.page, parent=Tag.stack[-1], **kwargs)
-        return self.slots[name]
+        slot = self.slots[name]
+        if self.origin:
+            slot.origin = self.origin
+            if slot.ref:
+                self.origin.refs[slot.ref] = slot
+        return slot
 
     def slot(self, name="default"):
         #
         # We put this here, so it clears the children only when the slot-filler is doing its filling.
         # Otherwise, the previous children are kept. Lucky them.
         self.slots[name].children = []
         return self.slots[name]
 
     def __enter__(self):
         self.stack.append(self)
+        self.origin_stack[0].append(self)
         self.component_stack.append(self)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stack.pop()
+        self.origin_stack[0].pop()
         self.component_stack.pop()
         return False
 
     def __str__(self):
         return f"{self.component_name or self.__class__.__name__} ({self.ref} {id(self)})"
 
     def __repr__(self):
         return f"<{self}>"
 
 
 class Page(Component):
-    def __init__(self, router=None, matched_route=None, application=None, **kwargs):
+    def __init__(self, matched_route=None, application=None, **kwargs):
         ref = mixed_to_underscores(self.__class__.__name__)
-        self.router = router
         self.matched_route = matched_route
-        self.application = application
+        self._application = application
 
         self._redraw_timeout_set = False
         self.redraw_list = set()
 
         super().__init__(ref=ref, **kwargs)
 
     def update_title(self):
@@ -550,14 +577,15 @@
         if title is not None:
             self.document.title = title
 
     def page_title(self):
         pass
 
     def redraw_tag(self, tag):
+        # print("requesting redraw", tag)
         assert isinstance(tag, Tag)
         self.redraw_list.add(tag)
 
         if not self._redraw_timeout_set:
             if is_server_side:
                 self._do_redraw()
             else:
@@ -572,68 +600,78 @@
                 if tag in redrawn_already:
                     raise Exception(
                         "A redraw event is causing a circular redraw event loop. Yo dawg, are you causing "
                         "a redraw from your redraw?"
                     )
                 tag.redraw()
                 redrawn_already.add(tag)
-                tag.destroy_orphans()
         finally:
             self._redraw_timeout_set = False
 
 
 class Builder:
     def __init__(self):
         self.components = {}
 
     def generate_tag(self, tag_name, *children, **kwargs):
         tag_name = tag_name.lower().strip()
+        if kwargs.get("tag"):
+            tag_name = kwargs.pop("tag")
+        elif "_" in tag_name:
+            tag_name = tag_name.replace("_", "-")
+
         parent = Tag.stack[-1] if Tag.stack else None
         parent_component = Tag.component_stack[-1] if Tag.component_stack else None
         root_tag = Tag.stack[0] if Tag.stack else None
+        origin = Tag.population_stack[-1] if Tag.population_stack else None
 
         # The root tag might not always be the page, but if it isn't, it should have a reference to the
         # actual page.
         if isinstance(root_tag, Page):
             page = root_tag
         elif root_tag:
             page = root_tag.page
         else:
             raise Exception("t.generate_tag called without a context")
 
         # Determine ref value
-        ref = kwargs.pop("ref", f"_{tag_name}-{len(parent.children) + 1}")
+        ref_part = f"__{parent.ref}.{tag_name}{len(parent.children) + 1}"
+
+        ref = kwargs.pop("ref", ref_part)
 
-        if ref in parent.children_by_ref:
-            element = parent.children_by_ref[ref]
-            element._handle_kwargs(kwargs)
+        if ref and origin and ref in origin._refs_pending_removal:
+            element = origin._refs_pending_removal.pop(ref)
+            assert element.origin == origin
+            element._configure(kwargs)
             element.children = []
             if children:
                 element.add(*children)
-            if element not in parent.children:
-                parent.children.append(element)
+            element.parent = parent
         elif tag_name in self.components:
             element = self.components[tag_name](
                 ref=ref,
                 page=page,
                 parent=parent,
                 parent_component=parent_component,
+                origin=origin,
                 children=children,
                 **kwargs,
             )
         else:
             element = Tag(
                 tag_name,
                 ref=ref,
                 page=page,
                 parent=parent,
                 parent_component=parent_component,
+                origin=origin,
                 children=children,
                 **kwargs,
             )
+        origin.refs[ref] = element
         with element:
             element.generate_children()
         return element
 
     def add_library(self, library):
         for component in library.components:
             self.add_component(component)
@@ -645,15 +683,15 @@
 
         return inner
 
     def add_component(self, component: Component):
         if component.component_name:
             component_name = component.component_name
         else:
-            component_name = mixed_to_underscores(component.__name__)
+            component_name = mixed_to_underscores(component.__name__, "-")
         self.components[component_name.lower()] = component
 
     def __call__(self, *texts):
         parent = Tag.stack[-1] if Tag.stack else None
         if not parent:
             raise Exception("Cannot call t() to generate text without a parent")
         parent.add(*texts)
```

### Comparing `puepy-0.1.2/puepy/reactivity.py` & `puepy-0.2.0/puepy/reactivity.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.2/puepy/runtime.py` & `puepy-0.2.0/puepy/runtime.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.2/puepy/storage.py` & `puepy-0.2.0/puepy/storage.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.2/puepy/util.py` & `puepy-0.2.0/puepy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
     from pyscript.ffi import to_js
 except ImportError:
 
     def to_js(obj):
         return obj
 
 
-def mixed_to_underscores(input_string):
+def mixed_to_underscores(input_string, separator="_"):
     result = []
     for index, char in enumerate(input_string):
         if char.isupper() and index > 0:
-            result.append("_")
+            result.append(separator)
         result.append(char.lower())
     return "".join(result)
 
 
 def merge_classes(*items):
     classes = set()
     exclude_classes = set()
@@ -80,19 +80,18 @@
     # Remove attributes that don't exist in source element
     for attribute in get_attributes(target_element):
         if not source_element.hasAttribute(attribute):
             target_element.removeAttribute(attribute)
 
     # Set attributes from source to target
     for attribute in get_attributes(source_element):
-        if attribute != "gen-time":
-            target_element.setAttribute(attribute, source_element.getAttribute(attribute))
+        target_element.setAttribute(attribute, source_element.getAttribute(attribute))
 
     if not is_server_side:
-        if source_element.tagName.lower() in ("input", "radio", "option"):
+        if source_element.tagName.lower() in ("input", "radio", "option", "textarea"):
             target_element.value = source_element.value
 
     # Iterate over the children
     target_child_nodes = list(target_element.childNodes)
     source_child_nodes = list(source_element.childNodes)
 
     child_count = max(len(source_child_nodes), len(target_child_nodes))
```

### Comparing `puepy-0.1.2/PKG-INFO` & `puepy-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 Metadata-Version: 2.1
 Name: puepy
-Version: 0.1.2
+Version: 0.2.0
 Summary: Frontend Framework for PyScript
+Home-page: https://puepy.dev/
+License: Apache-2.0
+Keywords: pyscript,webassembly,frontend,framework,reactive
 Author: Ken Kinder
 Author-email: ken+github@kkinder.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Environment :: WebAssembly
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Project-URL: Documentation, https://docs.puepy.dev/
+Project-URL: Repository, https://github.com/kkinder/puepy
 Description-Content-Type: text/markdown
 
 # PuePy -- PyScript Frontend Framework
 
 PuePy is an attempt to create a frontend framework using [PyScript](https://pyscript.net). PuePy is partially inspired by Vue. It runs entirely in your browser, though server-side rendering is likely feasible.  PuePy aims to support two runtime environments: PyScript Pyodide or PyScript Micropython. The Micropython option foregoes some features found in the CPython, but offers a far, far smaller runtime, making it a better option for websites. Line-of-business or scientific webapp developers may prefer the CPython version, which is heavier but more functional.
 
 Without further ado, here's a taste:
```

