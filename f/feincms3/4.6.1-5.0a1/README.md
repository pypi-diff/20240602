# Comparing `tmp/feincms3-4.6.1.tar.gz` & `tmp/feincms3-5.0a1.tar.gz`

## Comparing `feincms3-4.6.1.tar` & `feincms3-5.0a1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/__init__.py
--rw-r--r--   0        0        0    18418 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/admin.py
--rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/applications.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/cleanse.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/embedding.py
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/inline_ckeditor.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/mixins.py
--rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/pages.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/regions.py
--rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/renderer.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/shortcuts.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/utils.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7758 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/__init__.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/external.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/html.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/image.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/old_richtext.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/richtext.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/plugins/snippet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/root/__init__.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/root/middleware.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/root/passthru.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/box-drawing.css
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/box-drawing.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor-contents.css
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.css
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.js
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/move-form.css
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/plugin-ckeditor.css
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/static/feincms3/static-path-style.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/templatetags/__init__.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 feincms3-4.6.1/feincms3/templatetags/feincms3.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 feincms3-4.6.1/.gitignore
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 feincms3-4.6.1/LICENSE
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 feincms3-4.6.1/README.rst
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 feincms3-4.6.1/pyproject.toml
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 feincms3-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/__init__.py
+-rw-r--r--   0        0        0    22857 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/admin.py
+-rw-r--r--   0        0        0    23996 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/applications.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/cleanse.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/embedding.py
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/inline_ckeditor.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/mixins.py
+-rw-r--r--   0        0        0     9935 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/pages.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/regions.py
+-rw-r--r--   0        0        0    13486 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/renderer.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/shortcuts.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/utils.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/__init__.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/external.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/html.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/image.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/old_richtext.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/richtext.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/plugins/snippet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/root/__init__.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/root/middleware.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/root/passthru.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/admin.css
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/admin.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor-contents.css
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.css
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.js
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/plugin-ckeditor.css
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/static/feincms3/static-path-style.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/templatetags/__init__.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 feincms3-5.0a1/feincms3/templatetags/feincms3.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 feincms3-5.0a1/.gitignore
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 feincms3-5.0a1/LICENSE
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 feincms3-5.0a1/README.rst
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 feincms3-5.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 feincms3-5.0a1/PKG-INFO
```

### Comparing `feincms3-4.6.1/feincms3/admin.py` & `feincms3-5.0a1/feincms3/admin.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from functools import update_wrapper
 
 from django import forms
 from django.contrib import messages
 from django.contrib.admin import ModelAdmin, SimpleListFilter, display, helpers
 from django.contrib.admin.options import IncorrectLookupParameters, csrf_protect_m
 from django.contrib.admin.utils import unquote
-from django.core.exceptions import PermissionDenied
+from django.core.exceptions import PermissionDenied, ValidationError
 from django.db import router, transaction
+from django.db.models import F
+from django.http import HttpResponse
 from django.shortcuts import redirect
-from django.urls import re_path, reverse
+from django.urls import path, re_path, reverse
 from django.utils.html import format_html, mark_safe
 from django.utils.text import capfirst
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.csrf import csrf_protect
 from js_asset.js import JS
 from tree_queries.forms import TreeNodeChoiceField
 
@@ -73,18 +75,18 @@
     @csrf_protect_m
     def changelist_view(self, request, **kwargs):
         response = super().changelist_view(request, **kwargs)
         if not hasattr(response, "context_data"):
             return response
         context = self.tree_admin_context(request)
         response.context_data["media"] += forms.Media(
-            css={"all": ["feincms3/box-drawing.css"]},
+            css={"all": ["feincms3/admin.css"]},
             js=[
                 JS(
-                    "feincms3/box-drawing.js",
+                    "feincms3/admin.js",
                     {"id": "feincms3-context", "data-context": json.dumps(context)},
                 ),
             ],
         )
         return response
 
     def tree_admin_context(self, request):
@@ -127,45 +129,79 @@
     indented_title.short_description = _("title")
 
     def move_column(self, instance):
         """
         Show a ``move`` link which leads to a separate page where the move
         destination may be selected.
         """
+        return format_html(
+            """\
+<div class="move-controls">
+<button class="move-cut" type="button" data-pk="{}" title="{}">
+  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 -960 960 960" width="24px" fill="currentColor"><path d="M760-120 480-400l-94 94q8 15 11 32t3 34q0 66-47 113T240-80q-66 0-113-47T80-240q0-66 47-113t113-47q17 0 34 3t32 11l94-94-94-94q-15 8-32 11t-34 3q-66 0-113-47T80-720q0-66 47-113t113-47q66 0 113 47t47 113q0 17-3 34t-11 32l494 494v40H760ZM600-520l-80-80 240-240h120v40L600-520ZM240-640q33 0 56.5-23.5T320-720q0-33-23.5-56.5T240-800q-33 0-56.5 23.5T160-720q0 33 23.5 56.5T240-640Zm240 180q8 0 14-6t6-14q0-8-6-14t-14-6q-8 0-14 6t-6 14q0 8 6 14t14 6ZM240-160q33 0 56.5-23.5T320-240q0-33-23.5-56.5T240-320q-33 0-56.5 23.5T160-240q0 33 23.5 56.5T240-160Z"/></svg>
+</button>
+<select class="move-paste" data-pk="{}">
+  <option value="">{}</option>
+  <option value="before">{}</option> -->
+  <option value="first-child">{}</option>
+  <option value="last-child">{}</option>
+  <option value="after">{}</option>
+</select>
+</div>
+""",
+            instance.pk,
+            _("Move '{}' to a new location").format(instance),
+            instance.pk,
+            _("move"),
+            _("before"),
+            _("as first child"),
+            _("as last child"),
+            _("after"),
+        )
+
         opts = self.model._meta
         return format_html(
             '<a href="{}">{}</a>',
             reverse(
                 f"admin:{opts.app_label}_{opts.model_name}_move",
                 args=(instance.pk,),
             ),
             _("move"),
         )
 
-    move_column.short_description = ""
+    move_column.short_description = _("move")
 
     def get_urls(self):
         """
         Add our own ``move`` view.
         """
 
         info = self.model._meta.app_label, self.model._meta.model_name
         return [
+            path(
+                "move-node/",
+                self.admin_site.admin_view(self.move_node_view),
+            ),
             re_path(
                 r"^(.+)/move/$",
                 action_form_view_decorator(self)(self.move_view),
                 name="{}_{}_move".format(*info),
             ),
             re_path(
                 r"^(.+)/clone/$",
                 action_form_view_decorator(self)(self.clone_view),
                 name="{}_{}_clone".format(*info),
             ),
         ] + super().get_urls()
 
+    def move_node_view(self, request):
+        kw = {"request": request, "modeladmin": self}
+        form = MoveNodeForm(request.POST, **kw)
+        return HttpResponse(form.process())
+
     def move_view(self, request, obj):
         return self.action_form_view(
             request, obj, form_class=MoveForm, title=_("Move %s") % obj
         )
 
     def clone_view(self, request, obj):
         return self.action_form_view(
@@ -213,25 +249,102 @@
         )
 
         # Suppress the rendering of the "save and add another" button.
         response.context_data["has_add_permission"] = False
         return response
 
 
+class MoveNodeForm(forms.Form):
+    def __init__(self, *args, **kwargs):
+        self.modeladmin = kwargs.pop("modeladmin")
+        self.request = kwargs.pop("request")
+        super().__init__(*args, **kwargs)
+
+        self.fields["move"] = forms.ModelChoiceField(
+            queryset=self.modeladmin.get_queryset(self.request)
+        )
+        self.fields["relative_to"] = forms.ModelChoiceField(
+            queryset=self.modeladmin.get_queryset(self.request)
+        )
+        positions = ("before", "first-child", "last-child", "after")
+        self.fields["position"] = forms.ChoiceField(choices=zip(positions, positions))
+
+    def process(self):
+        if not self.is_valid():
+            messages.error(self.request, _("Invalid node move request."))
+            messages.error(self.request, str(self.errors))
+            return "error"
+
+        move = self.cleaned_data["move"]
+        relative_to = self.cleaned_data["relative_to"]
+        position = self.cleaned_data["position"]
+
+        print(self.cleaned_data)
+
+        if position in {"first-child", "last-child"}:
+            move.parent = relative_to
+            siblings_qs = relative_to.children
+        else:
+            move.parent = relative_to.parent
+            siblings_qs = relative_to.__class__._default_manager.filter(
+                parent=relative_to.parent
+            )
+
+        try:
+            # All fields of model are not in this form
+            move.full_clean(exclude=[f.name for f in move._meta.get_fields()])
+        except ValidationError as exc:
+            messages.error(
+                self.request,
+                _("Error while validating the new position of '{}'.").format(move),
+            )
+            messages.error(self.request, str(exc))
+            return "error"
+
+        if position == "before":
+            siblings_qs.filter(position__gte=relative_to.position).update(
+                position=F("position") + 10
+            )
+            move.position = relative_to.position
+            move.save()
+
+        elif position == "after":
+            siblings_qs.filter(position__gt=relative_to.position).update(
+                position=F("position") + 10
+            )
+            move.position = relative_to.position + 10
+            move.save()
+
+        elif position == "first-child":
+            siblings_qs.update(position=F("position") + 10)
+            move.position = 10
+            move.save()
+
+        elif position == "last-child":
+            move.position = 0  # Let AbstractPage.save handle the position
+            move.save()
+
+        else:  # pragma: no cover
+            pass
+
+        messages.success(
+            self.request,
+            _("Node '{}' has been moved to its new position.").format(move),
+        )
+        return "ok"
+
+
 class MoveForm(forms.Form):
     """
     Allows making the node the left or right sibling or the first or last
     child of another node.
 
     Requires the node to be moved as ``obj`` keyword argument.
     """
 
-    class Media:
-        css = {"screen": ["feincms3/move-form.css"]}
-
     def __init__(self, *args, **kwargs):
         self.instance = kwargs.pop("obj")
         self.modeladmin = kwargs.pop("modeladmin")
         self.request = kwargs.pop("request")
         self.model = self.instance.__class__
 
         super().__init__(*args, **kwargs)
```

### Comparing `feincms3-4.6.1/feincms3/applications.py` & `feincms3-5.0a1/feincms3/applications.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/cleanse.py` & `feincms3-5.0a1/feincms3/cleanse.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/embedding.py` & `feincms3-5.0a1/feincms3/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/inline_ckeditor.py` & `feincms3-5.0a1/feincms3/inline_ckeditor.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/mixins.py` & `feincms3-5.0a1/feincms3/mixins.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/pages.py` & `feincms3-5.0a1/feincms3/pages.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/regions.py` & `feincms3-5.0a1/feincms3/regions.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/renderer.py` & `feincms3-5.0a1/feincms3/renderer.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/shortcuts.py` & `feincms3-5.0a1/feincms3/shortcuts.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 
         >>> template_name(Article, "_detail")
         "articles/article_detail.html"
         >>> template_name(User, "_form")
         "auth/user_form.html"
     """
 
-    return "{}/{}{}.html".format(
-        model._meta.app_label,
-        model._meta.model_name,
-        template_name_suffix,
+    return (
+        f"{model._meta.app_label}/{model._meta.model_name}{template_name_suffix}.html"
     )
 
 
 def render_list(
     request,
     queryset,
     context=None,
```

### Comparing `feincms3-4.6.1/feincms3/utils.py` & `feincms3-5.0a1/feincms3/utils.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.mo` & `feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -49,27 +49,39 @@
 msgid ""
 "Do not chain redirects. The selected page \"%(title)s\" redirects to "
 "\"%(path)s\"."
 msgstr ""
 "Die gewählte Seite „%(title)s“ leitet schon weiter auf „%(path)s“ weiter, "
 "bitte Verkettungen von Weiterleitungen vermeiden."
 
+msgid "Error while validating the new position of '{}'."
+msgstr "Fehler beim Validieren der neuen Position von '{}'."
+
+msgid "Invalid node move request."
+msgstr "Ungültige Verschiebungsanfrage."
+
 msgid "Move %s"
 msgstr "%s verschieben"
 
+msgid "Move '{}' to a new location"
+msgstr "'{}' zu einer neuen Position verschieben"
+
 msgid ""
 "Moving isn't possible because there are no valid targets. Maybe you selected "
 "the only root node?"
 msgstr ""
 "Verschieben ist nicht möglich weil es keine gültigen Zielorte gibt. "
 "Vielleicht den einzigen Wurzelknoten gewählt?"
 
 msgid "New location"
 msgstr "Neuer Ort"
 
+msgid "Node '{}' has been moved to its new position."
+msgstr "'%(node)s' wurde zur neuen Position verschoben."
+
 msgid ""
 "Objects in the primary language cannot be the translation of another object."
 msgstr ""
 "Objekte in der primären Sprache können nicht eine Übersetzung eines anderen "
 "Objektes sein."
 
 msgid "Only set one redirect value."
@@ -132,17 +144,29 @@
 
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr "Kann das HTML für diese URL nicht laden, tut mir leid!"
 
 msgid "Updated fields of %(node)s: %(fields)s"
 msgstr "Aktualisierte Felder von %(node)s: %(fields)s"
 
+msgid "after"
+msgstr "nachher"
+
 msgid "alternative text"
 msgstr "alternativer Text"
 
+msgid "as first child"
+msgstr "als erstes Unterelement"
+
+msgid "as last child"
+msgstr "als letztes Unterelement"
+
+msgid "before"
+msgstr "vorher"
+
 msgid "caption"
 msgstr "Legende"
 
 msgid "external content"
 msgstr "externer Inhalt"
 
 msgid "image"
```

### Comparing `feincms3-4.6.1/feincms3/locale/de/LC_MESSAGES/django.po` & `feincms3-5.0a1/feincms3/locale/de/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -5,109 +5,150 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-04 16:18+0200\n"
+"POT-Creation-Date: 2024-06-02 19:46+0200\n"
 "PO-Revision-Date: 2020-12-04 09:43+0000\n"
 "Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
-"Language-Team: German <https://hosted.weblate.org/projects/feincms3/feincms3/de/>\n"
+"Language-Team: German <https://hosted.weblate.org/projects/feincms3/feincms3/"
+"de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:128 pages.py:69
+#: admin.py:129 pages.py:84
 msgid "title"
 msgstr "Titel"
 
-#: admin.py:142
+#: admin.py:152
+msgid "Move '{}' to a new location"
+msgstr "'{}' zu einer neuen Position verschieben"
+
+#: admin.py:154 admin.py:168 admin.py:171
 msgid "move"
 msgstr "verschieben"
 
-#: admin.py:168
+#: admin.py:155
+msgid "before"
+msgstr "vorher"
+
+#: admin.py:156
+msgid "as first child"
+msgstr "als erstes Unterelement"
+
+#: admin.py:157
+msgid "as last child"
+msgstr "als letztes Unterelement"
+
+#: admin.py:158
+msgid "after"
+msgstr "nachher"
+
+#: admin.py:203
 #, python-format
 msgid "Move %s"
 msgstr "%s verschieben"
 
-#: admin.py:173
+#: admin.py:208
 #, python-format
 msgid "Clone %s"
 msgstr "%s klonen"
 
-#: admin.py:242
+#: admin.py:273
+msgid "Invalid node move request."
+msgstr "Ungültige Verschiebungsanfrage."
+
+#: admin.py:296
+msgid "Error while validating the new position of '{}'."
+msgstr "Fehler beim Validieren der neuen Position von '{}'."
+
+#: admin.py:327
+msgid "Node '{}' has been moved to its new position."
+msgstr "'%(node)s' wurde zur neuen Position verschoben."
+
+#: admin.py:352
 msgid "New location"
 msgstr "Neuer Ort"
 
-#: admin.py:250
-msgid "Moving isn't possible because there are no valid targets. Maybe you selected the only root node?"
-msgstr "Verschieben ist nicht möglich weil es keine gültigen Zielorte gibt. Vielleicht den einzigen Wurzelknoten gewählt?"
+#: admin.py:360
+msgid ""
+"Moving isn't possible because there are no valid targets. Maybe you selected "
+"the only root node?"
+msgstr ""
+"Verschieben ist nicht möglich weil es keine gültigen Zielorte gibt. "
+"Vielleicht den einzigen Wurzelknoten gewählt?"
 
-#: admin.py:296 admin.py:307 admin.py:317
+#: admin.py:406 admin.py:417 admin.py:427
 msgid "move here"
 msgstr "hierhin verschieben"
 
-#: admin.py:375
+#: admin.py:489
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
 msgstr "%(node)s wurde zur neuen Position verschoben."
 
-#: admin.py:393
+#: admin.py:507
 msgid "target"
 msgstr "Ziel"
 
-#: admin.py:403
+#: admin.py:517
 msgid "Replace target's content"
 msgstr "Inhalt des Ziels ersetzen"
 
-#: admin.py:405
+#: admin.py:519
 #, python-format
 msgid "Affects the following models: %s."
 msgstr "Betrifft die folgenden Inhalte: %s."
 
-#: admin.py:427
+#: admin.py:541
 #, python-format
 msgid "Current: \"%s\""
 msgstr "Aktuell: „%s“"
 
-#: admin.py:437
+#: admin.py:551
 msgid "Cannot clone node to itself."
 msgstr "Kann Knoten nicht zu sich selbst klonen."
 
-#: admin.py:460
+#: admin.py:574
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
 msgstr "Aktualisierte Felder von %(node)s: %(fields)s"
 
-#: admin.py:484
+#: admin.py:598
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
 msgstr "Ersetzte den Inhalt von %(target)s mit dem Inhalt von %(source)s."
 
-#: admin.py:511
+#: admin.py:625
 msgid "subtree"
 msgstr "Unterbaum"
 
-#: applications.py:532
+#: applications.py:525
 msgid "page type"
 msgstr "Seitentyp"
 
-#: applications.py:576
+#: applications.py:569
 #, python-format
 msgid "This field is required for the page type \"%s\"."
 msgstr "Dieses Feld wird für den Seitentyp \"%s\" benötigt."
 
-#: applications.py:602
+#: applications.py:597
 #, python-brace-format
-msgid "The page type \"{page_type}\" with the specified configuration exists already."
-msgstr "Der Seitentyp \"{page_type}\" mit der spezifizierten Konfiguration existiert schon."
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
+msgstr ""
+"Der Seitentyp \"{page_type}\" mit der spezifizierten Konfiguration existiert "
+"schon."
 
 #: mixins.py:20
 msgid "menu"
 msgstr "Menü"
 
 #: mixins.py:72 plugins/snippet.py:33
 msgid "template"
@@ -118,16 +159,19 @@
 msgstr "Sprache"
 
 #: mixins.py:154
 msgid "translation of"
 msgstr "Übersetzung von"
 
 #: mixins.py:215
-msgid "Objects in the primary language cannot be the translation of another object."
-msgstr "Objekte in der primären Sprache können nicht eine Übersetzung eines anderen Objektes sein."
+msgid ""
+"Objects in the primary language cannot be the translation of another object."
+msgstr ""
+"Objekte in der primären Sprache können nicht eine Übersetzung eines anderen "
+"Objektes sein."
 
 #: mixins.py:229
 msgid "Redirect to URL"
 msgstr "Weiterleiten zu URL"
 
 #: mixins.py:237
 msgid "Redirect to page"
@@ -139,63 +183,76 @@
 
 #: mixins.py:268
 msgid "Cannot redirect to self."
 msgstr "Kann nicht zu sich selbst weiterleiten."
 
 #: mixins.py:279
 #, python-format
-msgid "Do not chain redirects. The selected page \"%(title)s\" redirects to \"%(path)s\"."
-msgstr "Die gewählte Seite „%(title)s“ leitet schon weiter auf „%(path)s“ weiter, bitte Verkettungen von Weiterleitungen vermeiden."
+msgid ""
+"Do not chain redirects. The selected page \"%(title)s\" redirects to "
+"\"%(path)s\"."
+msgstr ""
+"Die gewählte Seite „%(title)s“ leitet schon weiter auf „%(path)s“ weiter, "
+"bitte Verkettungen von Weiterleitungen vermeiden."
 
 #: mixins.py:296
 #, python-format
-msgid "Do not chain redirects. The following pages already redirect to this page: %(pages)s"
-msgstr "Verkettung von Weiterleitungen nicht erlaubt. Die folgenden Seiten leiten schon auf diese Seite weiter: %(pages)s"
+msgid ""
+"Do not chain redirects. The following pages already redirect to this page: "
+"%(pages)s"
+msgstr ""
+"Verkettung von Weiterleitungen nicht erlaubt. Die folgenden Seiten leiten "
+"schon auf diese Seite weiter: %(pages)s"
 
-#: pages.py:68
+#: pages.py:83
 msgid "is active"
 msgstr "ist aktiv"
 
-#: pages.py:70
+#: pages.py:85
 msgid "slug"
 msgstr "Slug"
 
-#: pages.py:77
+#: pages.py:92
 msgid "Position is expected to be greater than zero."
 msgstr "Position sollte grösser als Null sein."
 
-#: pages.py:84
+#: pages.py:99
 msgid "path"
 msgstr "Pfad"
 
-#: pages.py:89
-msgid "Automatically generated by concatenating the parent's path and the slug unless the path is defined manually."
-msgstr "Wird automatisch generiert durch das Aneinananderhängen des Pfades der übergeordneten Seite und des Slugs, ausser wenn der Pfad manuell definiert wird."
+#: pages.py:104
+msgid ""
+"Automatically generated by concatenating the parent's path and the slug "
+"unless the path is defined manually."
+msgstr ""
+"Wird automatisch generiert durch das Aneinananderhängen des Pfades der "
+"übergeordneten Seite und des Slugs, ausser wenn der Pfad manuell definiert "
+"wird."
 
-#: pages.py:95
+#: pages.py:110
 msgid "Path must start and end with a slash (/)."
 msgstr "Pfad muss mit einem Slash (/) starten und enden."
 
-#: pages.py:99
+#: pages.py:114
 msgid "manually define the path"
 msgstr "Pfad manuell definieren"
 
-#: pages.py:106
+#: pages.py:121
 msgid "page"
 msgstr "Seite"
 
-#: pages.py:107
+#: pages.py:122
 msgid "pages"
 msgstr "Seiten"
 
-#: pages.py:149
+#: pages.py:167
 msgid "Static paths cannot be empty. Did you mean '/'?"
 msgstr "Statische Pfade können nicht leer sein. Meinten Sie „/“?"
 
-#: pages.py:171
+#: pages.py:189
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr "Der Pfad %(path)s der Seite %(page)s würde nicht eindeutig sein."
 
 #: plugins/external.py:113
 msgid "URL"
 msgstr "URL"
@@ -217,20 +274,29 @@
 msgstr "externer Inhalt"
 
 #: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr "Kann das HTML für diese URL nicht laden, tut mir leid!"
 
 #: plugins/html.py:26
-msgid "The content will be inserted directly into the page. It is VERY important that the HTML snippet is well-formed!"
-msgstr "Der Inhalt wird direkt in die Seite eingefügt. Es ist SEHR wichtig, dass das HTML gültig ist!"
+msgid ""
+"The content will be inserted directly into the page. It is VERY important "
+"that the HTML snippet is well-formed!"
+msgstr ""
+"Der Inhalt wird direkt in die Seite eingefügt. Es ist SEHR wichtig, dass das "
+"HTML gültig ist!"
 
-#: plugins/html.py:59
-msgid "Please note that the HTML must be well formed. It's your responsibility to ensure that nothing breaks now or in the future when using this plugin."
-msgstr "Das HTML muss unbedingt wohlgeformt sein. Es liegt in Ihrer Verantwortung sicherzustellen, dass jetzt und in Zukunft nichts schiefgeht, wenn Sie dieses Plugin verwenden."
+#: plugins/html.py:60
+msgid ""
+"Please note that the HTML must be well formed. It's your responsibility to "
+"ensure that nothing breaks now or in the future when using this plugin."
+msgstr ""
+"Das HTML muss unbedingt wohlgeformt sein. Es liegt in Ihrer Verantwortung "
+"sicherzustellen, dass jetzt und in Zukunft nichts schiefgeht, wenn Sie "
+"dieses Plugin verwenden."
 
 #: plugins/image.py:26 plugins/image.py:51
 msgid "image"
 msgstr "Bild"
 
 #: plugins/image.py:35
 msgid "image width"
@@ -244,38 +310,41 @@
 msgid "primary point of interest"
 msgstr "Fokuspunkt"
 
 #: plugins/image.py:52
 msgid "images"
 msgstr "Bilder"
 
-#: plugins/old_richtext.py:40 plugins/richtext.py:20
+#: plugins/old_richtext.py:41 plugins/richtext.py:20
 msgid "text"
 msgstr "Text"
 
-#: plugins/old_richtext.py:44 plugins/richtext.py:24
+#: plugins/old_richtext.py:45 plugins/richtext.py:24
 msgid "rich text"
 msgstr "Text"
 
-#: plugins/old_richtext.py:45 plugins/richtext.py:25
+#: plugins/old_richtext.py:46 plugins/richtext.py:25
 msgid "rich texts"
 msgstr "Texte"
 
 #: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr "vordefinierter Baustein"
 
 #: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr "vordefinierte Bausteine"
 
 #~ msgid "This exact app already exists."
 #~ msgstr "Diese exakte Anwendung existiert bereits."
 
-#~ msgid "Objects may only be the translation of objects in the primary language."
-#~ msgstr "Objekte können nur Übersetzungen sein von Objekten in der primären Sprache."
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr ""
+#~ "Objekte können nur Übersetzungen sein von Objekten in der primären "
+#~ "Sprache."
 
 #~ msgid "Generated automatically if 'static path' is unset."
 #~ msgstr "Automatisch generiert falls „statischer Pfad“ nicht gesetzt ist."
 
 #~ msgid "static path"
 #~ msgstr "statischer Pfad"
```

### Comparing `feincms3-4.6.1/feincms3/locale/en/LC_MESSAGES/django.po` & `feincms3-5.0a1/feincms3/locale/en/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,107 +4,143 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-04 16:18+0200\n"
+"POT-Creation-Date: 2024-06-02 19:46+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:128 pages.py:69
+#: admin.py:129 pages.py:84
 msgid "title"
 msgstr ""
 
-#: admin.py:142
+#: admin.py:152
+msgid "Move '{}' to a new location"
+msgstr ""
+
+#: admin.py:154 admin.py:168 admin.py:171
 msgid "move"
 msgstr ""
 
-#: admin.py:168
+#: admin.py:155
+msgid "before"
+msgstr ""
+
+#: admin.py:156
+msgid "as first child"
+msgstr ""
+
+#: admin.py:157
+msgid "as last child"
+msgstr ""
+
+#: admin.py:158
+msgid "after"
+msgstr ""
+
+#: admin.py:203
 #, python-format
 msgid "Move %s"
 msgstr ""
 
-#: admin.py:173
+#: admin.py:208
 #, python-format
 msgid "Clone %s"
 msgstr ""
 
-#: admin.py:242
+#: admin.py:273
+msgid "Invalid node move request."
+msgstr ""
+
+#: admin.py:296
+msgid "Error while validating the new position of '{}'."
+msgstr ""
+
+#: admin.py:327
+msgid "Node '{}' has been moved to its new position."
+msgstr ""
+
+#: admin.py:352
 msgid "New location"
 msgstr ""
 
-#: admin.py:250
-msgid "Moving isn't possible because there are no valid targets. Maybe you selected the only root node?"
+#: admin.py:360
+msgid ""
+"Moving isn't possible because there are no valid targets. Maybe you selected "
+"the only root node?"
 msgstr ""
 
-#: admin.py:296 admin.py:307 admin.py:317
+#: admin.py:406 admin.py:417 admin.py:427
 msgid "move here"
 msgstr ""
 
-#: admin.py:375
+#: admin.py:489
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
 msgstr ""
 
-#: admin.py:393
+#: admin.py:507
 msgid "target"
 msgstr ""
 
-#: admin.py:403
+#: admin.py:517
 msgid "Replace target's content"
 msgstr ""
 
-#: admin.py:405
+#: admin.py:519
 #, python-format
 msgid "Affects the following models: %s."
 msgstr ""
 
-#: admin.py:427
+#: admin.py:541
 #, python-format
 msgid "Current: \"%s\""
 msgstr ""
 
-#: admin.py:437
+#: admin.py:551
 msgid "Cannot clone node to itself."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:574
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
 msgstr ""
 
-#: admin.py:484
+#: admin.py:598
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
 msgstr ""
 
-#: admin.py:511
+#: admin.py:625
 msgid "subtree"
 msgstr ""
 
-#: applications.py:532
+#: applications.py:525
 msgid "page type"
 msgstr ""
 
-#: applications.py:576
+#: applications.py:569
 #, python-format
 msgid "This field is required for the page type \"%s\"."
 msgstr ""
 
-#: applications.py:602
+#: applications.py:597
 #, python-brace-format
-msgid "The page type \"{page_type}\" with the specified configuration exists already."
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
 msgstr ""
 
 #: mixins.py:20
 msgid "menu"
 msgstr ""
 
 #: mixins.py:72 plugins/snippet.py:33
@@ -116,15 +152,16 @@
 msgstr ""
 
 #: mixins.py:154
 msgid "translation of"
 msgstr ""
 
 #: mixins.py:215
-msgid "Objects in the primary language cannot be the translation of another object."
+msgid ""
+"Objects in the primary language cannot be the translation of another object."
 msgstr ""
 
 #: mixins.py:229
 msgid "Redirect to URL"
 msgstr ""
 
 #: mixins.py:237
@@ -137,63 +174,69 @@
 
 #: mixins.py:268
 msgid "Cannot redirect to self."
 msgstr ""
 
 #: mixins.py:279
 #, python-format
-msgid "Do not chain redirects. The selected page \"%(title)s\" redirects to \"%(path)s\"."
+msgid ""
+"Do not chain redirects. The selected page \"%(title)s\" redirects to "
+"\"%(path)s\"."
 msgstr ""
 
 #: mixins.py:296
 #, python-format
-msgid "Do not chain redirects. The following pages already redirect to this page: %(pages)s"
+msgid ""
+"Do not chain redirects. The following pages already redirect to this page: "
+"%(pages)s"
 msgstr ""
 
-#: pages.py:68
+#: pages.py:83
 msgid "is active"
 msgstr ""
 
-#: pages.py:70
+#: pages.py:85
 msgid "slug"
 msgstr ""
 
-#: pages.py:77
+#: pages.py:92
 msgid "Position is expected to be greater than zero."
 msgstr ""
 
-#: pages.py:84
+#: pages.py:99
 msgid "path"
 msgstr ""
 
-#: pages.py:89
-msgid "Automatically generated by concatenating the parent's path and the slug unless the path is defined manually."
+#: pages.py:104
+msgid ""
+"Automatically generated by concatenating the parent's path and the slug "
+"unless the path is defined manually."
 msgstr ""
 
-#: pages.py:95
+#: pages.py:110
 msgid "Path must start and end with a slash (/)."
 msgstr ""
 
-#: pages.py:99
+#: pages.py:114
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:106
+#: pages.py:121
 msgid "page"
 msgstr ""
 
-#: pages.py:107
+#: pages.py:122
 msgid "pages"
 msgstr ""
 
-#: pages.py:149
+#: pages.py:167
 msgid "Static paths cannot be empty. Did you mean '/'?"
 msgstr ""
 
-#: pages.py:171
+#: pages.py:189
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr ""
 
 #: plugins/external.py:113
 msgid "URL"
 msgstr ""
@@ -215,19 +258,23 @@
 msgstr ""
 
 #: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr ""
 
 #: plugins/html.py:26
-msgid "The content will be inserted directly into the page. It is VERY important that the HTML snippet is well-formed!"
+msgid ""
+"The content will be inserted directly into the page. It is VERY important "
+"that the HTML snippet is well-formed!"
 msgstr ""
 
-#: plugins/html.py:59
-msgid "Please note that the HTML must be well formed. It's your responsibility to ensure that nothing breaks now or in the future when using this plugin."
+#: plugins/html.py:60
+msgid ""
+"Please note that the HTML must be well formed. It's your responsibility to "
+"ensure that nothing breaks now or in the future when using this plugin."
 msgstr ""
 
 #: plugins/image.py:26 plugins/image.py:51
 msgid "image"
 msgstr ""
 
 #: plugins/image.py:35
@@ -242,23 +289,23 @@
 msgid "primary point of interest"
 msgstr ""
 
 #: plugins/image.py:52
 msgid "images"
 msgstr ""
 
-#: plugins/old_richtext.py:40 plugins/richtext.py:20
+#: plugins/old_richtext.py:41 plugins/richtext.py:20
 msgid "text"
 msgstr ""
 
-#: plugins/old_richtext.py:44 plugins/richtext.py:24
+#: plugins/old_richtext.py:45 plugins/richtext.py:24
 msgid "rich text"
 msgstr ""
 
-#: plugins/old_richtext.py:45 plugins/richtext.py:25
+#: plugins/old_richtext.py:46 plugins/richtext.py:25
 msgid "rich texts"
 msgstr ""
 
 #: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
```

### Comparing `feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.mo` & `feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/locale/fr/LC_MESSAGES/django.po` & `feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -5,315 +5,378 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-04 16:18+0200\n"
-"PO-Revision-Date: 2020-12-04 09:43+0000\n"
-"Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
-"Language-Team: French <https://hosted.weblate.org/projects/feincms3/feincms3/fr/>\n"
-"Language: fr\n"
+"POT-Creation-Date: 2024-06-02 19:46+0200\n"
+"PO-Revision-Date: 2020-12-04 09:46+0000\n"
+"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
+"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
+"feincms3/feincms3/nb_NO/>\n"
+"Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:128 pages.py:69
+#: admin.py:129 pages.py:84
 msgid "title"
-msgstr "titre"
+msgstr "tittel"
 
-#: admin.py:142
+#: admin.py:152
+msgid "Move '{}' to a new location"
+msgstr ""
+
+#: admin.py:154 admin.py:168 admin.py:171
 msgid "move"
-msgstr "déplacer"
+msgstr "flytt"
+
+#: admin.py:155
+msgid "before"
+msgstr ""
+
+#: admin.py:156
+#, fuzzy
+#| msgid "first child"
+msgid "as first child"
+msgstr "erstes Kind"
+
+#: admin.py:157
+#, fuzzy
+#| msgid "last child"
+msgid "as last child"
+msgstr "letztes Kind"
 
-#: admin.py:168
+#: admin.py:158
+msgid "after"
+msgstr ""
+
+#: admin.py:203
 #, python-format
 msgid "Move %s"
-msgstr "Déplacer %s"
+msgstr "Flytt %s"
 
-#: admin.py:173
+#: admin.py:208
 #, python-format
 msgid "Clone %s"
-msgstr "Cloner %s"
+msgstr "Klon %s"
+
+#: admin.py:273
+msgid "Invalid node move request."
+msgstr ""
 
-#: admin.py:242
+#: admin.py:296
+msgid "Error while validating the new position of '{}'."
+msgstr ""
+
+#: admin.py:327
+#, fuzzy
+#| msgid "The node %(node)s has been moved to the new position."
+msgid "Node '{}' has been moved to its new position."
+msgstr "Noden %(node)s har blitt flyttet til ny plassering"
+
+#: admin.py:352
 msgid "New location"
-msgstr "Nouvel emplacement"
+msgstr "Ny plassering"
 
-#: admin.py:250
-msgid "Moving isn't possible because there are no valid targets. Maybe you selected the only root node?"
-msgstr "Le déplacement n’est pas possible car il n’y a pas de cibles valides. Peut-être avez-vous sélectionné le seul nœud racine ?"
+#: admin.py:360
+msgid ""
+"Moving isn't possible because there are no valid targets. Maybe you selected "
+"the only root node?"
+msgstr ""
+"Flytting er ikke mulig fordi det ikke er noen gyldige mål. Kanskje du valgte "
+"den eneste rotnoden?"
 
-#: admin.py:296 admin.py:307 admin.py:317
+#: admin.py:406 admin.py:417 admin.py:427
 msgid "move here"
-msgstr "déplacer ici"
+msgstr "flytt hit"
 
-#: admin.py:375
+#: admin.py:489
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
-msgstr "Le nœud %(node)s a été déplacé vers la nouvelle position."
+msgstr "Noden %(node)s har blitt flyttet til ny plassering"
 
-#: admin.py:393
+#: admin.py:507
 msgid "target"
-msgstr "cible"
+msgstr "mål"
 
-#: admin.py:403
+#: admin.py:517
 msgid "Replace target's content"
-msgstr "Remplacer le contenu de la cible"
+msgstr "Erstatt målets innhold"
 
-#: admin.py:405
+#: admin.py:519
 #, python-format
 msgid "Affects the following models: %s."
-msgstr "Affecte les modèles suivants : %s."
+msgstr "Har innvirkning på følgende moduler: %s."
 
-#: admin.py:427
+#: admin.py:541
 #, python-format
 msgid "Current: \"%s\""
-msgstr "Actuel : « %s »"
+msgstr "Nåværende: «%s»"
 
-#: admin.py:437
+#: admin.py:551
 msgid "Cannot clone node to itself."
-msgstr "Impossible de cloner le nœud sur lui-même."
+msgstr "Kan ikke klone node til seg selv."
 
-#: admin.py:460
+#: admin.py:574
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
-msgstr "Champs mis à jour de %(node)s : %(fields)s"
+msgstr "Oppdaterte felter tilhørende %(node)s: %(fields)s"
 
-#: admin.py:484
+#: admin.py:598
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
-msgstr "Remplacement du contenu de %(target)s par le contenu de %(source)s."
+msgstr "Erstattet innholdet i %(target)s med innholdet i %(source)s."
 
-#: admin.py:511
+#: admin.py:625
 msgid "subtree"
 msgstr ""
 
-#: applications.py:532
+#: applications.py:525
+#, fuzzy
+#| msgid "page"
 msgid "page type"
-msgstr "type de page"
+msgstr "side"
 
-#: applications.py:576
-#, python-format
+#: applications.py:569
+#, fuzzy, python-format
+#| msgid "This field is required for the application %s."
 msgid "This field is required for the page type \"%s\"."
-msgstr "Ce champ est obligatoire pour le type de page \"%s\"."
+msgstr "Dette feltet kreves for programmet %s."
 
-#: applications.py:602
+#: applications.py:597
 #, python-brace-format
-msgid "The page type \"{page_type}\" with the specified configuration exists already."
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
 msgstr ""
 
 #: mixins.py:20
 msgid "menu"
-msgstr "menu"
+msgstr "meny"
 
 #: mixins.py:72 plugins/snippet.py:33
 msgid "template"
-msgstr "modèle"
+msgstr "mal"
 
 #: mixins.py:124
 msgid "language"
-msgstr "langue"
+msgstr "språk"
 
 #: mixins.py:154
 msgid "translation of"
-msgstr "traduction de"
+msgstr "oversettelse av"
 
 #: mixins.py:215
-msgid "Objects in the primary language cannot be the translation of another object."
-msgstr "Les objets dans la langue principale ne peuvent pas être la traduction d’un autre objet."
+msgid ""
+"Objects in the primary language cannot be the translation of another object."
+msgstr ""
+"Objekter i primærspråket kan ikke være oversettelsen av et annet objekt."
 
 #: mixins.py:229
 msgid "Redirect to URL"
-msgstr "Rediriger vers l’URL"
+msgstr "Videresendt til nettadresse"
 
 #: mixins.py:237
 msgid "Redirect to page"
-msgstr "Rediriger vers la page"
+msgstr "Videresendt til side"
 
 #: mixins.py:260
 msgid "Only set one redirect value."
-msgstr "Définissez une seule valeur de redirection."
+msgstr "Kun sett én videresendingsverdi."
 
 #: mixins.py:268
 msgid "Cannot redirect to self."
-msgstr "Impossible de rediriger vers soi."
+msgstr "Kan ikke videresende til seg selv."
 
 #: mixins.py:279
 #, python-format
-msgid "Do not chain redirects. The selected page \"%(title)s\" redirects to \"%(path)s\"."
-msgstr "Ne pas enchaîner les redirections. La page sélectionnée « %(title)s » redirige vers « %(path)s »."
+msgid ""
+"Do not chain redirects. The selected page \"%(title)s\" redirects to "
+"\"%(path)s\"."
+msgstr ""
+"Kan ikke opprette videresendelser i stafett. Valgt side «%(title)s» "
+"videresender til «%(path)s»."
 
 #: mixins.py:296
 #, python-format
-msgid "Do not chain redirects. The following pages already redirect to this page: %(pages)s"
-msgstr "Ne pas enchaîner les redirections. Les pages suivantes redirigent déjà vers cette page : %(pages)s"
+msgid ""
+"Do not chain redirects. The following pages already redirect to this page: "
+"%(pages)s"
+msgstr ""
+"Ikke opprett videresendelser i stafett. Følgende sider videresender til "
+"denne siden: %(pages)s"
 
-#: pages.py:68
+#: pages.py:83
 msgid "is active"
-msgstr "est actif"
+msgstr "er aktiv"
 
-#: pages.py:70
+#: pages.py:85
 msgid "slug"
-msgstr "slug"
+msgstr ""
 
-#: pages.py:77
+#: pages.py:92
 msgid "Position is expected to be greater than zero."
-msgstr "La position devrait être supérieure à zéro."
+msgstr "Posisjonen forventes å være større enn null."
 
-#: pages.py:84
+#: pages.py:99
 msgid "path"
-msgstr "chemin"
+msgstr "sti"
 
-#: pages.py:89
-msgid "Automatically generated by concatenating the parent's path and the slug unless the path is defined manually."
+#: pages.py:104
+msgid ""
+"Automatically generated by concatenating the parent's path and the slug "
+"unless the path is defined manually."
 msgstr ""
 
-#: pages.py:95
+#: pages.py:110
 msgid "Path must start and end with a slash (/)."
-msgstr "Le chemin doit commencer et se terminer par une barre oblique (/)."
+msgstr "Sti må starte og slutt med skråstrek (/)."
 
-#: pages.py:99
+#: pages.py:114
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:106
+#: pages.py:121
 msgid "page"
-msgstr "page"
+msgstr "side"
 
-#: pages.py:107
+#: pages.py:122
 msgid "pages"
-msgstr "pages"
+msgstr "sider"
 
-#: pages.py:149
+#: pages.py:167
 msgid "Static paths cannot be empty. Did you mean '/'?"
-msgstr "Les chemins statiques ne peuvent pas être vides. Vouliez-vous dire « / » ?"
+msgstr "Statiske stier må fylles ut. Mente du «/»?"
 
-#: pages.py:171
+#: pages.py:189
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
-msgstr "Le nouveau chemin %(path)s de la page %(page)s ne serait pas unique."
+msgstr "Siden «%(page)s» sin nye sti %(path)s finnes allerede."
 
 #: plugins/external.py:113
 msgid "URL"
-msgstr "URL"
+msgstr "Nettadresse"
 
 #: plugins/external.py:115 plugins/image.py:42
 msgid "alternative text"
-msgstr "texte alternatif"
+msgstr ""
 
 #: plugins/external.py:116 plugins/image.py:43
 msgid "Describe the contents, e.g. for screenreaders."
-msgstr "Décrit les contenus de l’image, par ex. pour un lecteur d’écran."
+msgstr ""
 
 #: plugins/external.py:120 plugins/image.py:47
+#, fuzzy
+#| msgid "application"
 msgid "caption"
-msgstr "légende"
+msgstr "program"
 
 #: plugins/external.py:124
 msgid "external content"
-msgstr "contenu externe"
+msgstr "eksternt innhold"
 
 #: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
-msgstr "Impossible de récupérer le HTML pour cette URL, désolé !"
+msgstr "Klarte ikke å hente HTML for denne nettadressen."
 
 #: plugins/html.py:26
-msgid "The content will be inserted directly into the page. It is VERY important that the HTML snippet is well-formed!"
-msgstr "Le contenu sera inséré directement dans la page. Il est TRÈS important que l’extrait de code HTML soit bien formé !"
+msgid ""
+"The content will be inserted directly into the page. It is VERY important "
+"that the HTML snippet is well-formed!"
+msgstr ""
 
-#: plugins/html.py:59
-msgid "Please note that the HTML must be well formed. It's your responsibility to ensure that nothing breaks now or in the future when using this plugin."
+#: plugins/html.py:60
+msgid ""
+"Please note that the HTML must be well formed. It's your responsibility to "
+"ensure that nothing breaks now or in the future when using this plugin."
 msgstr ""
 
 #: plugins/image.py:26 plugins/image.py:51
 msgid "image"
-msgstr "image"
+msgstr "bilde"
 
 #: plugins/image.py:35
 msgid "image width"
-msgstr "Largeur de l’image"
+msgstr "bildebredde"
 
 #: plugins/image.py:38
 msgid "image height"
-msgstr "hauteur de l’image"
+msgstr "bildehøyde"
 
 #: plugins/image.py:40
 msgid "primary point of interest"
-msgstr "principal point d’intérêt"
+msgstr "hoved-interessepunkt"
 
 #: plugins/image.py:52
 msgid "images"
-msgstr "images"
+msgstr "bilder"
 
-#: plugins/old_richtext.py:40 plugins/richtext.py:20
+#: plugins/old_richtext.py:41 plugins/richtext.py:20
 msgid "text"
-msgstr "texte"
+msgstr "tekst"
 
-#: plugins/old_richtext.py:44 plugins/richtext.py:24
+#: plugins/old_richtext.py:45 plugins/richtext.py:24
+#, fuzzy
 msgid "rich text"
-msgstr "texte riche"
+msgstr "rikholdig tekst"
 
-#: plugins/old_richtext.py:45 plugins/richtext.py:25
+#: plugins/old_richtext.py:46 plugins/richtext.py:25
+#, fuzzy
 msgid "rich texts"
-msgstr "textes riches"
+msgstr "rikholdige tekster"
 
 #: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
 
 #: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr ""
 
 #~ msgid "This exact app already exists."
-#~ msgstr "Cette application exacte existe déjà."
+#~ msgstr "Akkurat dette programmet finnes allerede."
 
-#~ msgid "Objects may only be the translation of objects in the primary language."
-#~ msgstr "Les objets peuvent seulement être la traduction d’objets dans la langue principale."
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr "Objekter kan kun være oversettelser av objekter i primærspråk."
 
 #~ msgid "Generated automatically if 'static path' is unset."
-#~ msgstr "Généré automatiquement si le « chemin statique » n’est pas défini."
+#~ msgstr "Generert automatisk hvis «statisk sti» ikke er valgt."
 
 #~ msgid "static path"
-#~ msgstr "chemin statique"
+#~ msgstr "statisk sti"
 
 #~ msgid "snippet"
-#~ msgstr "extrait"
+#~ msgstr "tekstsnutt"
 
 #~ msgid "snippets"
-#~ msgstr "extraits"
+#~ msgstr "tekstsnutter"
 
 #~ msgid "template name"
-#~ msgstr "nom du modèle"
+#~ msgstr "malnavn"
 
 #~ msgid "ancestor"
-#~ msgstr "ancêtre"
+#~ msgstr "opphav"
 
 #~ msgid "app instance namespace"
-#~ msgstr "espace de noms d’instance d’application"
+#~ msgstr "programinstans-navnerom"
 
 #~ msgid "move to"
 #~ msgstr "verschieben nach"
 
 #~ msgid "left sibling"
 #~ msgstr "linkes Geschwister"
 
 #~ msgid "right sibling"
 #~ msgstr "rechtes Geschwister"
 
-#~ msgid "first child"
-#~ msgstr "erstes Kind"
-
-#~ msgid "last child"
-#~ msgstr "letztes Kind"
-
 #~ msgid "Make node"
 #~ msgstr "Mach Knoten"
 
 #~ msgctxt "MoveForm"
 #~ msgid "Of"
 #~ msgstr "Von"
```

### Comparing `feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.mo` & `feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/locale/it/LC_MESSAGES/django.po` & `feincms3-5.0a1/feincms3/locale/it/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -5,111 +5,154 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-04 16:18+0200\n"
+"POT-Creation-Date: 2024-06-02 19:46+0200\n"
 "PO-Revision-Date: 2020-12-04 09:43+0000\n"
 "Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
-"Language-Team: Italian <https://hosted.weblate.org/projects/feincms3/feincms3/it/>\n"
+"Language-Team: Italian <https://hosted.weblate.org/projects/feincms3/"
+"feincms3/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:128 pages.py:69
+#: admin.py:129 pages.py:84
 msgid "title"
 msgstr "titolo"
 
-#: admin.py:142
+#: admin.py:152
+msgid "Move '{}' to a new location"
+msgstr ""
+
+#: admin.py:154 admin.py:168 admin.py:171
 msgid "move"
 msgstr "sposta"
 
-#: admin.py:168
+#: admin.py:155
+msgid "before"
+msgstr ""
+
+#: admin.py:156
+#, fuzzy
+#| msgid "first child"
+msgid "as first child"
+msgstr "erstes Kind"
+
+#: admin.py:157
+#, fuzzy
+#| msgid "last child"
+msgid "as last child"
+msgstr "letztes Kind"
+
+#: admin.py:158
+msgid "after"
+msgstr ""
+
+#: admin.py:203
 #, python-format
 msgid "Move %s"
 msgstr "Sposta %s"
 
-#: admin.py:173
+#: admin.py:208
 #, python-format
 msgid "Clone %s"
 msgstr "Clona %s"
 
-#: admin.py:242
+#: admin.py:273
+msgid "Invalid node move request."
+msgstr ""
+
+#: admin.py:296
+msgid "Error while validating the new position of '{}'."
+msgstr ""
+
+#: admin.py:327
+msgid "Node '{}' has been moved to its new position."
+msgstr ""
+
+#: admin.py:352
 msgid "New location"
 msgstr "Nuova posizione"
 
-#: admin.py:250
-msgid "Moving isn't possible because there are no valid targets. Maybe you selected the only root node?"
-msgstr "Lo spostamento non è possibile perché non ci sono bersagli validi. Forse hai selezionato l'unico nodo radice?"
+#: admin.py:360
+msgid ""
+"Moving isn't possible because there are no valid targets. Maybe you selected "
+"the only root node?"
+msgstr ""
+"Lo spostamento non è possibile perché non ci sono bersagli validi. Forse hai "
+"selezionato l'unico nodo radice?"
 
-#: admin.py:296 admin.py:307 admin.py:317
+#: admin.py:406 admin.py:417 admin.py:427
 msgid "move here"
 msgstr "sposta qui"
 
-#: admin.py:375
+#: admin.py:489
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
 msgstr ""
 
-#: admin.py:393
+#: admin.py:507
 msgid "target"
 msgstr ""
 
-#: admin.py:403
+#: admin.py:517
 msgid "Replace target's content"
 msgstr ""
 
-#: admin.py:405
+#: admin.py:519
 #, python-format
 msgid "Affects the following models: %s."
 msgstr ""
 
-#: admin.py:427
+#: admin.py:541
 #, python-format
 msgid "Current: \"%s\""
 msgstr "Attuale: «%s»"
 
-#: admin.py:437
+#: admin.py:551
 msgid "Cannot clone node to itself."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:574
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
 msgstr ""
 
-#: admin.py:484
+#: admin.py:598
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
 msgstr ""
 
-#: admin.py:511
+#: admin.py:625
 msgid "subtree"
 msgstr ""
 
-#: applications.py:532
+#: applications.py:525
 #, fuzzy
 #| msgid "page"
 msgid "page type"
 msgstr "pagina"
 
-#: applications.py:576
+#: applications.py:569
 #, fuzzy, python-format
 #| msgid "This field is required for the application %s."
 msgid "This field is required for the page type \"%s\"."
 msgstr "Questo campo è obbligatorio per l’applicazione %s."
 
-#: applications.py:602
+#: applications.py:597
 #, python-brace-format
-msgid "The page type \"{page_type}\" with the specified configuration exists already."
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
 msgstr ""
 
 #: mixins.py:20
 msgid "menu"
 msgstr "menù"
 
 #: mixins.py:72 plugins/snippet.py:33
@@ -121,16 +164,19 @@
 msgstr "lingua"
 
 #: mixins.py:154
 msgid "translation of"
 msgstr "traduzione di"
 
 #: mixins.py:215
-msgid "Objects in the primary language cannot be the translation of another object."
-msgstr "Gli oggetti nella lingua principale non possono essere la traduzione di un altro oggetto."
+msgid ""
+"Objects in the primary language cannot be the translation of another object."
+msgstr ""
+"Gli oggetti nella lingua principale non possono essere la traduzione di un "
+"altro oggetto."
 
 #: mixins.py:229
 msgid "Redirect to URL"
 msgstr "Reindirizza all’URL"
 
 #: mixins.py:237
 msgid "Redirect to page"
@@ -142,63 +188,69 @@
 
 #: mixins.py:268
 msgid "Cannot redirect to self."
 msgstr ""
 
 #: mixins.py:279
 #, python-format
-msgid "Do not chain redirects. The selected page \"%(title)s\" redirects to \"%(path)s\"."
+msgid ""
+"Do not chain redirects. The selected page \"%(title)s\" redirects to "
+"\"%(path)s\"."
 msgstr ""
 
 #: mixins.py:296
 #, python-format
-msgid "Do not chain redirects. The following pages already redirect to this page: %(pages)s"
+msgid ""
+"Do not chain redirects. The following pages already redirect to this page: "
+"%(pages)s"
 msgstr ""
 
-#: pages.py:68
+#: pages.py:83
 msgid "is active"
 msgstr "è attivo"
 
-#: pages.py:70
+#: pages.py:85
 msgid "slug"
 msgstr ""
 
-#: pages.py:77
+#: pages.py:92
 msgid "Position is expected to be greater than zero."
 msgstr ""
 
-#: pages.py:84
+#: pages.py:99
 msgid "path"
 msgstr ""
 
-#: pages.py:89
-msgid "Automatically generated by concatenating the parent's path and the slug unless the path is defined manually."
+#: pages.py:104
+msgid ""
+"Automatically generated by concatenating the parent's path and the slug "
+"unless the path is defined manually."
 msgstr ""
 
-#: pages.py:95
+#: pages.py:110
 msgid "Path must start and end with a slash (/)."
 msgstr ""
 
-#: pages.py:99
+#: pages.py:114
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:106
+#: pages.py:121
 msgid "page"
 msgstr "pagina"
 
-#: pages.py:107
+#: pages.py:122
 msgid "pages"
 msgstr "pagine"
 
-#: pages.py:149
+#: pages.py:167
 msgid "Static paths cannot be empty. Did you mean '/'?"
 msgstr ""
 
-#: pages.py:171
+#: pages.py:189
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
 msgstr ""
 
 #: plugins/external.py:113
 msgid "URL"
 msgstr "URL"
@@ -222,19 +274,25 @@
 msgstr ""
 
 #: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
 msgstr ""
 
 #: plugins/html.py:26
-msgid "The content will be inserted directly into the page. It is VERY important that the HTML snippet is well-formed!"
-msgstr "Il contenuto verrà inserito direttamente nella pagina. È MOLTO importante che il frammento HTML sia ben formato!"
+msgid ""
+"The content will be inserted directly into the page. It is VERY important "
+"that the HTML snippet is well-formed!"
+msgstr ""
+"Il contenuto verrà inserito direttamente nella pagina. È MOLTO importante "
+"che il frammento HTML sia ben formato!"
 
-#: plugins/html.py:59
-msgid "Please note that the HTML must be well formed. It's your responsibility to ensure that nothing breaks now or in the future when using this plugin."
+#: plugins/html.py:60
+msgid ""
+"Please note that the HTML must be well formed. It's your responsibility to "
+"ensure that nothing breaks now or in the future when using this plugin."
 msgstr ""
 
 #: plugins/image.py:26 plugins/image.py:51
 msgid "image"
 msgstr "imagine"
 
 #: plugins/image.py:35
@@ -249,39 +307,42 @@
 msgid "primary point of interest"
 msgstr ""
 
 #: plugins/image.py:52
 msgid "images"
 msgstr "imagini"
 
-#: plugins/old_richtext.py:40 plugins/richtext.py:20
+#: plugins/old_richtext.py:41 plugins/richtext.py:20
 msgid "text"
 msgstr "testo"
 
-#: plugins/old_richtext.py:44 plugins/richtext.py:24
+#: plugins/old_richtext.py:45 plugins/richtext.py:24
 msgid "rich text"
 msgstr ""
 
-#: plugins/old_richtext.py:45 plugins/richtext.py:25
+#: plugins/old_richtext.py:46 plugins/richtext.py:25
 msgid "rich texts"
 msgstr ""
 
 #: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
 
 #: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr ""
 
 #~ msgid "This exact app already exists."
 #~ msgstr "Questa applicazione esatta esiste già."
 
-#~ msgid "Objects may only be the translation of objects in the primary language."
-#~ msgstr "Gli oggetti possono essere solo la traduzione di oggetti nella lingua principale."
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr ""
+#~ "Gli oggetti possono essere solo la traduzione di oggetti nella lingua "
+#~ "principale."
 
 #~ msgid "snippet"
 #~ msgstr "frammento"
 
 #~ msgid "snippets"
 #~ msgstr "frammenti"
 
@@ -296,20 +357,14 @@
 
 #~ msgid "left sibling"
 #~ msgstr "linkes Geschwister"
 
 #~ msgid "right sibling"
 #~ msgstr "rechtes Geschwister"
 
-#~ msgid "first child"
-#~ msgstr "erstes Kind"
-
-#~ msgid "last child"
-#~ msgstr "letztes Kind"
-
 #~ msgid "Make node"
 #~ msgstr "Mach Knoten"
 
 #~ msgctxt "MoveForm"
 #~ msgid "Of"
 #~ msgstr "Von"
```

### Comparing `feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo` & `feincms3-5.0a1/feincms3/locale/nb_NO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/locale/nb_NO/LC_MESSAGES/django.po` & `feincms3-5.0a1/feincms3/locale/fr/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -5,322 +5,377 @@
 # Translators:
 # Matthias Kestenholz <mk@feinheit.ch>, 2011
 # sbaechler <simon@stellanera.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: feincms\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-04 16:18+0200\n"
-"PO-Revision-Date: 2020-12-04 09:46+0000\n"
-"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
-"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/feincms3/feincms3/nb_NO/>\n"
-"Language: nb_NO\n"
+"POT-Creation-Date: 2024-06-02 19:46+0200\n"
+"PO-Revision-Date: 2020-12-04 09:43+0000\n"
+"Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
+"Language-Team: French <https://hosted.weblate.org/projects/feincms3/feincms3/"
+"fr/>\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.4-dev\n"
 
-#: admin.py:128 pages.py:69
+#: admin.py:129 pages.py:84
 msgid "title"
-msgstr "tittel"
+msgstr "titre"
 
-#: admin.py:142
+#: admin.py:152
+msgid "Move '{}' to a new location"
+msgstr ""
+
+#: admin.py:154 admin.py:168 admin.py:171
 msgid "move"
-msgstr "flytt"
+msgstr "déplacer"
+
+#: admin.py:155
+msgid "before"
+msgstr ""
+
+#: admin.py:156
+#, fuzzy
+#| msgid "first child"
+msgid "as first child"
+msgstr "erstes Kind"
 
-#: admin.py:168
+#: admin.py:157
+#, fuzzy
+#| msgid "last child"
+msgid "as last child"
+msgstr "letztes Kind"
+
+#: admin.py:158
+msgid "after"
+msgstr ""
+
+#: admin.py:203
 #, python-format
 msgid "Move %s"
-msgstr "Flytt %s"
+msgstr "Déplacer %s"
 
-#: admin.py:173
+#: admin.py:208
 #, python-format
 msgid "Clone %s"
-msgstr "Klon %s"
+msgstr "Cloner %s"
 
-#: admin.py:242
+#: admin.py:273
+msgid "Invalid node move request."
+msgstr ""
+
+#: admin.py:296
+msgid "Error while validating the new position of '{}'."
+msgstr ""
+
+#: admin.py:327
+#, fuzzy
+#| msgid "The node %(node)s has been moved to the new position."
+msgid "Node '{}' has been moved to its new position."
+msgstr "Le nœud %(node)s a été déplacé vers la nouvelle position."
+
+#: admin.py:352
 msgid "New location"
-msgstr "Ny plassering"
+msgstr "Nouvel emplacement"
 
-#: admin.py:250
-msgid "Moving isn't possible because there are no valid targets. Maybe you selected the only root node?"
-msgstr "Flytting er ikke mulig fordi det ikke er noen gyldige mål. Kanskje du valgte den eneste rotnoden?"
+#: admin.py:360
+msgid ""
+"Moving isn't possible because there are no valid targets. Maybe you selected "
+"the only root node?"
+msgstr ""
+"Le déplacement n’est pas possible car il n’y a pas de cibles valides. Peut-"
+"être avez-vous sélectionné le seul nœud racine ?"
 
-#: admin.py:296 admin.py:307 admin.py:317
+#: admin.py:406 admin.py:417 admin.py:427
 msgid "move here"
-msgstr "flytt hit"
+msgstr "déplacer ici"
 
-#: admin.py:375
+#: admin.py:489
 #, python-format
 msgid "The node %(node)s has been moved to the new position."
-msgstr "Noden %(node)s har blitt flyttet til ny plassering"
+msgstr "Le nœud %(node)s a été déplacé vers la nouvelle position."
 
-#: admin.py:393
+#: admin.py:507
 msgid "target"
-msgstr "mål"
+msgstr "cible"
 
-#: admin.py:403
+#: admin.py:517
 msgid "Replace target's content"
-msgstr "Erstatt målets innhold"
+msgstr "Remplacer le contenu de la cible"
 
-#: admin.py:405
+#: admin.py:519
 #, python-format
 msgid "Affects the following models: %s."
-msgstr "Har innvirkning på følgende moduler: %s."
+msgstr "Affecte les modèles suivants : %s."
 
-#: admin.py:427
+#: admin.py:541
 #, python-format
 msgid "Current: \"%s\""
-msgstr "Nåværende: «%s»"
+msgstr "Actuel : « %s »"
 
-#: admin.py:437
+#: admin.py:551
 msgid "Cannot clone node to itself."
-msgstr "Kan ikke klone node til seg selv."
+msgstr "Impossible de cloner le nœud sur lui-même."
 
-#: admin.py:460
+#: admin.py:574
 #, python-format
 msgid "Updated fields of %(node)s: %(fields)s"
-msgstr "Oppdaterte felter tilhørende %(node)s: %(fields)s"
+msgstr "Champs mis à jour de %(node)s : %(fields)s"
 
-#: admin.py:484
+#: admin.py:598
 #, python-format
 msgid "Replaced the content of %(target)s with the contents of %(source)s."
-msgstr "Erstattet innholdet i %(target)s med innholdet i %(source)s."
+msgstr "Remplacement du contenu de %(target)s par le contenu de %(source)s."
 
-#: admin.py:511
+#: admin.py:625
 msgid "subtree"
 msgstr ""
 
-#: applications.py:532
-#, fuzzy
-#| msgid "page"
+#: applications.py:525
 msgid "page type"
-msgstr "side"
+msgstr "type de page"
 
-#: applications.py:576
-#, fuzzy, python-format
-#| msgid "This field is required for the application %s."
+#: applications.py:569
+#, python-format
 msgid "This field is required for the page type \"%s\"."
-msgstr "Dette feltet kreves for programmet %s."
+msgstr "Ce champ est obligatoire pour le type de page \"%s\"."
 
-#: applications.py:602
+#: applications.py:597
 #, python-brace-format
-msgid "The page type \"{page_type}\" with the specified configuration exists already."
+msgid ""
+"The page type \"{page_type}\" with the specified configuration exists "
+"already."
 msgstr ""
 
 #: mixins.py:20
 msgid "menu"
-msgstr "meny"
+msgstr "menu"
 
 #: mixins.py:72 plugins/snippet.py:33
 msgid "template"
-msgstr "mal"
+msgstr "modèle"
 
 #: mixins.py:124
 msgid "language"
-msgstr "språk"
+msgstr "langue"
 
 #: mixins.py:154
 msgid "translation of"
-msgstr "oversettelse av"
+msgstr "traduction de"
 
 #: mixins.py:215
-msgid "Objects in the primary language cannot be the translation of another object."
-msgstr "Objekter i primærspråket kan ikke være oversettelsen av et annet objekt."
+msgid ""
+"Objects in the primary language cannot be the translation of another object."
+msgstr ""
+"Les objets dans la langue principale ne peuvent pas être la traduction d’un "
+"autre objet."
 
 #: mixins.py:229
 msgid "Redirect to URL"
-msgstr "Videresendt til nettadresse"
+msgstr "Rediriger vers l’URL"
 
 #: mixins.py:237
 msgid "Redirect to page"
-msgstr "Videresendt til side"
+msgstr "Rediriger vers la page"
 
 #: mixins.py:260
 msgid "Only set one redirect value."
-msgstr "Kun sett én videresendingsverdi."
+msgstr "Définissez une seule valeur de redirection."
 
 #: mixins.py:268
 msgid "Cannot redirect to self."
-msgstr "Kan ikke videresende til seg selv."
+msgstr "Impossible de rediriger vers soi."
 
 #: mixins.py:279
 #, python-format
-msgid "Do not chain redirects. The selected page \"%(title)s\" redirects to \"%(path)s\"."
-msgstr "Kan ikke opprette videresendelser i stafett. Valgt side «%(title)s» videresender til «%(path)s»."
+msgid ""
+"Do not chain redirects. The selected page \"%(title)s\" redirects to "
+"\"%(path)s\"."
+msgstr ""
+"Ne pas enchaîner les redirections. La page sélectionnée « %(title)s » "
+"redirige vers « %(path)s »."
 
 #: mixins.py:296
 #, python-format
-msgid "Do not chain redirects. The following pages already redirect to this page: %(pages)s"
-msgstr "Ikke opprett videresendelser i stafett. Følgende sider videresender til denne siden: %(pages)s"
+msgid ""
+"Do not chain redirects. The following pages already redirect to this page: "
+"%(pages)s"
+msgstr ""
+"Ne pas enchaîner les redirections. Les pages suivantes redirigent déjà vers "
+"cette page : %(pages)s"
 
-#: pages.py:68
+#: pages.py:83
 msgid "is active"
-msgstr "er aktiv"
+msgstr "est actif"
 
-#: pages.py:70
+#: pages.py:85
 msgid "slug"
-msgstr ""
+msgstr "slug"
 
-#: pages.py:77
+#: pages.py:92
 msgid "Position is expected to be greater than zero."
-msgstr "Posisjonen forventes å være større enn null."
+msgstr "La position devrait être supérieure à zéro."
 
-#: pages.py:84
+#: pages.py:99
 msgid "path"
-msgstr "sti"
+msgstr "chemin"
 
-#: pages.py:89
-msgid "Automatically generated by concatenating the parent's path and the slug unless the path is defined manually."
+#: pages.py:104
+msgid ""
+"Automatically generated by concatenating the parent's path and the slug "
+"unless the path is defined manually."
 msgstr ""
 
-#: pages.py:95
+#: pages.py:110
 msgid "Path must start and end with a slash (/)."
-msgstr "Sti må starte og slutt med skråstrek (/)."
+msgstr "Le chemin doit commencer et se terminer par une barre oblique (/)."
 
-#: pages.py:99
+#: pages.py:114
 msgid "manually define the path"
 msgstr ""
 
-#: pages.py:106
+#: pages.py:121
 msgid "page"
-msgstr "side"
+msgstr "page"
 
-#: pages.py:107
+#: pages.py:122
 msgid "pages"
-msgstr "sider"
+msgstr "pages"
 
-#: pages.py:149
+#: pages.py:167
 msgid "Static paths cannot be empty. Did you mean '/'?"
-msgstr "Statiske stier må fylles ut. Mente du «/»?"
+msgstr ""
+"Les chemins statiques ne peuvent pas être vides. Vouliez-vous dire « / » ?"
 
-#: pages.py:171
+#: pages.py:189
 #, python-format
 msgid "The page %(page)s's new path %(path)s would not be unique."
-msgstr "Siden «%(page)s» sin nye sti %(path)s finnes allerede."
+msgstr "Le nouveau chemin %(path)s de la page %(page)s ne serait pas unique."
 
 #: plugins/external.py:113
 msgid "URL"
-msgstr "Nettadresse"
+msgstr "URL"
 
 #: plugins/external.py:115 plugins/image.py:42
 msgid "alternative text"
-msgstr ""
+msgstr "texte alternatif"
 
 #: plugins/external.py:116 plugins/image.py:43
 msgid "Describe the contents, e.g. for screenreaders."
-msgstr ""
+msgstr "Décrit les contenus de l’image, par ex. pour un lecteur d’écran."
 
 #: plugins/external.py:120 plugins/image.py:47
-#, fuzzy
-#| msgid "application"
 msgid "caption"
-msgstr "program"
+msgstr "légende"
 
 #: plugins/external.py:124
 msgid "external content"
-msgstr "eksternt innhold"
+msgstr "contenu externe"
 
 #: plugins/external.py:158
 msgid "Unable to fetch HTML for this URL, sorry!"
-msgstr "Klarte ikke å hente HTML for denne nettadressen."
+msgstr "Impossible de récupérer le HTML pour cette URL, désolé !"
 
 #: plugins/html.py:26
-msgid "The content will be inserted directly into the page. It is VERY important that the HTML snippet is well-formed!"
+msgid ""
+"The content will be inserted directly into the page. It is VERY important "
+"that the HTML snippet is well-formed!"
 msgstr ""
+"Le contenu sera inséré directement dans la page. Il est TRÈS important que "
+"l’extrait de code HTML soit bien formé !"
 
-#: plugins/html.py:59
-msgid "Please note that the HTML must be well formed. It's your responsibility to ensure that nothing breaks now or in the future when using this plugin."
+#: plugins/html.py:60
+msgid ""
+"Please note that the HTML must be well formed. It's your responsibility to "
+"ensure that nothing breaks now or in the future when using this plugin."
 msgstr ""
 
 #: plugins/image.py:26 plugins/image.py:51
 msgid "image"
-msgstr "bilde"
+msgstr "image"
 
 #: plugins/image.py:35
 msgid "image width"
-msgstr "bildebredde"
+msgstr "Largeur de l’image"
 
 #: plugins/image.py:38
 msgid "image height"
-msgstr "bildehøyde"
+msgstr "hauteur de l’image"
 
 #: plugins/image.py:40
 msgid "primary point of interest"
-msgstr "hoved-interessepunkt"
+msgstr "principal point d’intérêt"
 
 #: plugins/image.py:52
 msgid "images"
-msgstr "bilder"
+msgstr "images"
 
-#: plugins/old_richtext.py:40 plugins/richtext.py:20
+#: plugins/old_richtext.py:41 plugins/richtext.py:20
 msgid "text"
-msgstr "tekst"
+msgstr "texte"
 
-#: plugins/old_richtext.py:44 plugins/richtext.py:24
-#, fuzzy
+#: plugins/old_richtext.py:45 plugins/richtext.py:24
 msgid "rich text"
-msgstr "rikholdig tekst"
+msgstr "texte riche"
 
-#: plugins/old_richtext.py:45 plugins/richtext.py:25
-#, fuzzy
+#: plugins/old_richtext.py:46 plugins/richtext.py:25
 msgid "rich texts"
-msgstr "rikholdige tekster"
+msgstr "textes riches"
 
 #: plugins/snippet.py:37
 msgid "predefined snippet"
 msgstr ""
 
 #: plugins/snippet.py:38
 msgid "predefined snippets"
 msgstr ""
 
 #~ msgid "This exact app already exists."
-#~ msgstr "Akkurat dette programmet finnes allerede."
+#~ msgstr "Cette application exacte existe déjà."
 
-#~ msgid "Objects may only be the translation of objects in the primary language."
-#~ msgstr "Objekter kan kun være oversettelser av objekter i primærspråk."
+#~ msgid ""
+#~ "Objects may only be the translation of objects in the primary language."
+#~ msgstr ""
+#~ "Les objets peuvent seulement être la traduction d’objets dans la langue "
+#~ "principale."
 
 #~ msgid "Generated automatically if 'static path' is unset."
-#~ msgstr "Generert automatisk hvis «statisk sti» ikke er valgt."
+#~ msgstr "Généré automatiquement si le « chemin statique » n’est pas défini."
 
 #~ msgid "static path"
-#~ msgstr "statisk sti"
+#~ msgstr "chemin statique"
 
 #~ msgid "snippet"
-#~ msgstr "tekstsnutt"
+#~ msgstr "extrait"
 
 #~ msgid "snippets"
-#~ msgstr "tekstsnutter"
+#~ msgstr "extraits"
 
 #~ msgid "template name"
-#~ msgstr "malnavn"
+#~ msgstr "nom du modèle"
 
 #~ msgid "ancestor"
-#~ msgstr "opphav"
+#~ msgstr "ancêtre"
 
 #~ msgid "app instance namespace"
-#~ msgstr "programinstans-navnerom"
+#~ msgstr "espace de noms d’instance d’application"
 
 #~ msgid "move to"
 #~ msgstr "verschieben nach"
 
 #~ msgid "left sibling"
 #~ msgstr "linkes Geschwister"
 
 #~ msgid "right sibling"
 #~ msgstr "rechtes Geschwister"
 
-#~ msgid "first child"
-#~ msgstr "erstes Kind"
-
-#~ msgid "last child"
-#~ msgstr "letztes Kind"
-
 #~ msgid "Make node"
 #~ msgstr "Mach Knoten"
 
 #~ msgctxt "MoveForm"
 #~ msgid "Of"
 #~ msgstr "Von"
```

### Comparing `feincms3-4.6.1/feincms3/plugins/__init__.py` & `feincms3-5.0a1/feincms3/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/plugins/external.py` & `feincms3-5.0a1/feincms3/plugins/external.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/plugins/html.py` & `feincms3-5.0a1/feincms3/plugins/html.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/plugins/image.py` & `feincms3-5.0a1/feincms3/plugins/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Provides an image plugin with support for setting the primary point of
 interest. This is very useful especially when cropping images. Depends on
-`django-imagefield <https://django-imagefield.readthedocs.io>`__.  """
+`django-imagefield <https://django-imagefield.readthedocs.io>`__."""
 
 import os
 
 from content_editor.admin import ContentEditorInline
 from django.db import models
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
```

### Comparing `feincms3-4.6.1/feincms3/plugins/old_richtext.py` & `feincms3-5.0a1/feincms3/plugins/old_richtext.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Provides a rich text area whose content is automatically cleaned using a
 very restrictive allowlist of tags and attributes.
 
 Depends on
 `django-ckeditor <https://github.com/django-ckeditor/django-ckeditor/>`__ and
 `html-sanitizer <https://pypi.org/project/html-sanitizer>`__.
 """
+
 import warnings
 
 from content_editor.admin import ContentEditorInline
 from django.db import models
 from django.utils.html import mark_safe, strip_tags
 from django.utils.text import Truncator
 from django.utils.translation import gettext_lazy as _
```

### Comparing `feincms3-4.6.1/feincms3/plugins/richtext.py` & `feincms3-5.0a1/feincms3/plugins/richtext.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/plugins/snippet.py` & `feincms3-5.0a1/feincms3/plugins/snippet.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/root/middleware.py` & `feincms3-5.0a1/feincms3/root/middleware.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/root/passthru.py` & `feincms3-5.0a1/feincms3/root/passthru.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.css` & `feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.css`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/feincms3/static/feincms3/inline-ckeditor.js` & `feincms3-5.0a1/feincms3/static/feincms3/inline-ckeditor.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 /* global CKEDITOR, django */ ;
-(function() {
+(() => {
     function onReady(fn) {
         if (
             document.readyState === "complete" ||
             document.readyState === "interactive"
         ) {
             // call on next available tick
             setTimeout(fn, 1)
         } else {
             document.addEventListener("DOMContentLoaded", fn)
         }
     }
 
-    onReady(function() {
+    onReady(() => {
         const configs = {}
         const scripts = document.querySelectorAll("[data-inline-cke-config]")
         scripts.forEach(function parseConfig(script) {
             configs[script.dataset.inlineCkeId] = JSON.parse(
                 script.dataset.inlineCkeConfig,
             )
         })
```

### Comparing `feincms3-4.6.1/feincms3/static/feincms3/static-path-style.js` & `feincms3-5.0a1/feincms3/static/feincms3/static-path-style.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-document.addEventListener("DOMContentLoaded", function() {
+document.addEventListener("DOMContentLoaded", () => {
     const staticPathField = document.querySelector("#id_static_path")
     const pathField = document.querySelector("#id_path")
 
     function update() {
         pathField.classList.toggle("isAuto", !staticPathField.checked)
         pathField.disabled = !staticPathField.checked
     }
@@ -15,12 +15,12 @@
     transition: 0.2s;
   }
   #id_path.isAuto {
     opacity: 0.5;
     background: var(--selected-bg, #e4e4e4);
   }
   `
-    document.head.appendChild(style)
+    document.head.append(style)
 
     update()
     staticPathField.addEventListener("change", update)
 })
```

### Comparing `feincms3-4.6.1/feincms3/templatetags/feincms3.py` & `feincms3-5.0a1/feincms3/templatetags/feincms3.py`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/LICENSE` & `feincms3-5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/README.rst` & `feincms3-5.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3-4.6.1/pyproject.toml` & `feincms3-5.0a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   "hatchling",
 ]
 
 [project]
 name = "feincms3"
 description = "CMS-building toolkit for Django"
 readme = "README.rst"
-license = {text= "BSD-3-Clause"}
+license = { text = "BSD-3-Clause" }
 authors = [
-    { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
+  { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
 ]
 requires-python = ">=3.9"
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
@@ -30,98 +30,99 @@
   "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "asgiref>=3.6",
-  "Django>=3.2",
+  "django>=3.2",
   "django-content-editor>=6",
   "django-js-asset>=2",
   "django-tree-queries>=0.15",
 ]
-[project.optional-dependencies]
-all = [
+optional-dependencies.all = [
   "django-imagefield",
   "html-sanitizer>=1.1.1",
   "requests",
 ]
-tests = [
+optional-dependencies.tests = [
   "coverage",
   "django-ckeditor",
   "requests-mock",
 ]
-[project.urls]
-Homepage = "https://github.com/matthiask/feincms3/"
+urls.Homepage = "https://github.com/matthiask/feincms3/"
 
 [tool.hatch.build]
-include = ["feincms3/"]
+include = [
+  "feincms3/",
+]
 
 [tool.hatch.version]
 path = "feincms3/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "/feincms3",
+  "/feincms3",
 ]
 
 [tool.ruff]
-extend-select = [
-  # pyflakes, pycodestyle
-  "F", "E", "W",
-  # mmcabe
-  "C90",
-  # isort
-  "I",
-  # pep8-naming
-  "N",
-  # pyupgrade
-  "UP",
-  # flake8-2020
-  "YTT",
-  # flake8-boolean-trap
-  "FBT",
+target-version = "py39"
+
+fix = true
+show-fixes = true
+lint.extend-select = [
   # flake8-bugbear
   "B",
   # flake8-comprehensions
   "C4",
+  # mmcabe
+  "C90",
   # flake8-django
   "DJ",
-  # flake8-implicit-string-concatenation
-  "ISC",
-  # flake8-pie
-  "PIE",
-  # flake8-simplify
-  "SIM",
+  "E",
+  # pyflakes, pycodestyle
+  "F",
+  # flake8-boolean-trap
+  "FBT",
+  # isort
+  "I",
   # flake8-gettext
   "INT",
+  # flake8-implicit-string-concatenation
+  "ISC",
+  # pep8-naming
+  "N",
   # pygrep-hooks
   "PGH",
+  # flake8-pie
+  "PIE",
   # pylint
-  "PLC", "PLE", "PLW",
+  "PLC",
+  "PLE",
+  "PLW",
   # unused noqa
   "RUF100",
+  # flake8-simplify
+  "SIM",
+  # pyupgrade
+  "UP",
+  "W",
+  # flake8-2020
+  "YTT",
 ]
-extend-ignore = [
+lint.extend-ignore = [
   # Allow zip() without strict=
   "B905",
   # No line length errors
   "E501",
+  # Do not warn about percent formatting for now
+  "UP031",
 ]
-fix = true
-show-fixes = true
-target-version = "py39"
-
-[tool.ruff.isort]
-combine-as-imports = true
-lines-after-imports = 2
-
-[tool.ruff.mccabe]
-max-complexity = 15
-
-[tool.ruff.per-file-ignores]
-"*/migrat*/*" = [
+lint.per-file-ignores."*/migrat*/*" = [
   # Allow using PascalCase model names in migrations
   "N806",
   # Ignore the fact that migration files are invalid module names
   "N999",
 ]
+lint.isort.combine-as-imports = true
+lint.isort.lines-after-imports = 2
+lint.mccabe.max-complexity = 15
```

### Comparing `feincms3-4.6.1/PKG-INFO` & `feincms3-5.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: feincms3
-Version: 4.6.1
+Version: 5.0a1
 Summary: CMS-building toolkit for Django
 Project-URL: Homepage, https://github.com/matthiask/feincms3/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

