# Comparing `tmp/canu-0.1.0.tar.gz` & `tmp/canu-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canu-0.1.0.tar", last modified: Sat Jun  1 10:00:03 2024, max compression
+gzip compressed data, was "canu-0.2.0.tar", last modified: Sun Jun  2 07:39:15 2024, max compression
```

## Comparing `canu-0.1.0.tar` & `canu-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2024-06-01 10:00:03.826585 canu-0.1.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2024-06-01 09:11:47.000000 canu-0.1.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)      362 2024-06-01 10:00:03.826331 canu-0.1.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)       63 2024-06-01 09:57:21.000000 canu-0.1.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2024-06-01 10:00:03.825275 canu-0.1.0/canu/
--rw-r--r--   0 sbslee     (501) staff       (20)     2146 2024-06-01 09:52:21.000000 canu-0.1.0/canu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2024-06-01 09:15:28.000000 canu-0.1.0/canu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2024-06-01 10:00:03.826085 canu-0.1.0/canu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)      362 2024-06-01 10:00:03.000000 canu-0.1.0/canu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      171 2024-06-01 10:00:03.000000 canu-0.1.0/canu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2024-06-01 10:00:03.000000 canu-0.1.0/canu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2024-06-01 10:00:03.000000 canu-0.1.0/canu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2024-06-01 10:00:03.826647 canu-0.1.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      562 2024-06-01 09:17:46.000000 canu-0.1.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2024-06-02 07:39:15.639843 canu-0.2.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2024-06-02 07:38:52.000000 canu-0.2.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)      362 2024-06-02 07:39:15.639587 canu-0.2.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)       63 2024-06-02 07:38:52.000000 canu-0.2.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2024-06-02 07:39:15.638562 canu-0.2.0/canu/
+-rw-r--r--   0 sbslee     (501) staff       (20)     2892 2024-06-02 07:38:52.000000 canu-0.2.0/canu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2024-06-02 07:38:52.000000 canu-0.2.0/canu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2024-06-02 07:39:15.639348 canu-0.2.0/canu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)      362 2024-06-02 07:39:15.000000 canu-0.2.0/canu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      171 2024-06-02 07:39:15.000000 canu-0.2.0/canu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2024-06-02 07:39:15.000000 canu-0.2.0/canu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2024-06-02 07:39:15.000000 canu-0.2.0/canu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2024-06-02 07:39:15.639892 canu-0.2.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      562 2024-06-02 07:38:52.000000 canu-0.2.0/setup.py
```

### Comparing `canu-0.1.0/LICENSE` & `canu-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canu-0.1.0/canu/__init__.py` & `canu-0.2.0/canu/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import yaml
 import streamlit as st
 import streamlit_authenticator as stauth
+import openai
 
 class Container():
     def __init__(self, role, blocks):
         self.container = st.empty()
         self.role = role
         self.blocks = blocks
 
@@ -21,14 +22,36 @@
     def write_blocks(self, stream=False):
         if stream:
             with self.container:
                 self._write_blocks()
         else:
             self._write_blocks()
 
+class EventHandler(openai.AssistantEventHandler):
+    def __init__(self):
+        super().__init__()
+        self.container = None
+
+    def on_text_delta(self, delta, snapshot):
+        if self.container is None:
+            self.container = Container("assistant", [])
+        if not self.container.blocks or self.container.blocks[-1]['type'] != 'text':
+            self.container.blocks.append({'type': 'text', 'content': ""})
+        if delta.annotations is not None:
+            for annotation in delta.annotations:
+                if annotation.type == "file_citation":
+                    cited_file = st.session_state.client.files.retrieve(annotation.file_citation.file_id)
+                    delta.value = delta.value.replace(annotation.text, f"""<a href="#" title="{cited_file.filename}">[❞]</a>""")
+        self.container.blocks[-1]["content"] += delta.value
+        self.container.write_blocks(stream=True)
+
+    def on_end(self):
+        if self.container is not None:
+            st.session_state.containers.append(self.container)
+
 def get_authenticator(yaml_file):
     with open(yaml_file) as f:
         config = yaml.load(f, Loader=yaml.loader.SafeLoader)
     authenticator = stauth.Authenticate(
         config['credentials'],
         config['cookie']['name'],
         config['cookie']['key'],
@@ -41,19 +64,19 @@
         role=role,
         content=content
     )
     st.session_state.containers.append(
         Container(role, [{'type': 'text', 'content': content}])
     )
 
-def on_text_delta(self, delta, snapshot):
-    if self.container is None:
-        self.container = Container("assistant", [])
-    if not self.container.blocks or self.container.blocks[-1]['type'] != 'text':
-        self.container.blocks.append({'type': 'text', 'content': ""})
-    if delta.annotations is not None:
-        for annotation in delta.annotations:
-            if annotation.type == "file_citation":
-                cited_file = st.session_state.client.files.retrieve(annotation.file_citation.file_id)
-                delta.value = delta.value.replace(annotation.text, f"""<a href="#" title="{cited_file.filename}">[❞]</a>""")
-    self.container.blocks[-1]["content"] += delta.value
-    self.container.write_blocks(stream=True)
+def write_stream(event_handler=None):
+    if event_handler is None:
+        event_handler = EventHandler()
+    with st.session_state.client.beta.threads.runs.stream(
+        thread_id=st.session_state.thread.id,
+        assistant_id=st.session_state.assistant.id,
+        event_handler=event_handler,
+    ) as stream:
+        stream.until_done()
+
+def logout():
+    st.session_state.authenticator.logout(location='unrendered')
```

### Comparing `canu-0.1.0/setup.py` & `canu-0.2.0/setup.py`

 * *Files identical despite different names*

