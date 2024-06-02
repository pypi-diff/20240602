# Comparing `tmp/hal9-2.1.7.tar.gz` & `tmp/hal9-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.1.7.tar", max compression
+gzip compressed data, was "hal9-2.1.8.tar", max compression
```

## Comparing `hal9-2.1.7.tar` & `hal9-2.1.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     3731 2024-06-01 06:16:21.941512 hal9-2.1.7/README.md
--rw-r--r--   0        0        0       86 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/__init__.py
--rw-r--r--   0        0        0     1220 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/create.py
--rw-r--r--   0        0        0      574 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/run.py
--rw-r--r--   0        0        0      352 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/targets/docker.py
--rw-r--r--   0        0        0     2021 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/targets/hal9.py
--rw-r--r--   0        0        0       42 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/templates/docker/Dockerfile
--rw-r--r--   0        0        0       38 2024-06-01 06:16:21.841512 hal9-2.1.7/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      434 2024-06-01 06:16:21.841512 hal9-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 hal9-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3731 2024-06-01 20:48:05.019742 hal9-2.1.8/README.md
+-rw-r--r--   0        0        0      122 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/__init__.py
+-rw-r--r--   0        0        0     1176 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/cli.py
+-rw-r--r--   0        0        0      584 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/create.py
+-rw-r--r--   0        0        0      542 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/deploy.py
+-rw-r--r--   0        0        0      312 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/iobind.py
+-rw-r--r--   0        0        0      485 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/run.py
+-rw-r--r--   0        0        0      352 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/targets/docker.py
+-rw-r--r--   0        0        0     2021 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       38 2024-06-01 20:48:04.927741 hal9-2.1.8/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-06-01 20:48:04.927741 hal9-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 hal9-2.1.8/PKG-INFO
```

### Comparing `hal9-2.1.7/README.md` & `hal9-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hal9-2.1.7/hal9/create.py` & `hal9-2.1.8/hal9/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import shutil
 from pathlib import Path
 
 def create(path :str, template :str) -> str:
-    """Create an application
+  """Create an application
 
-    Parameters
-    ----------
-    path : str 
-            Path to the application.
-    template : str 
-            The template to use.
-    """
-
-    package_dir = Path(__file__).parent
-    template_path = package_dir / "templates" / template
-
-    os.makedirs(path, exist_ok=True)
-
-    for item in template_path.iterdir():
-        dest = Path(path) / item.name
-        if item.is_dir():
-            shutil.copytree(item, dest)
-        else:
-            shutil.copy2(item, dest)
+  Parameters
+  ----------
+  path : str 
+          Path to the application.
+  template : str 
+          The template to use.
+  """
+
+  package_dir = Path(__file__).parent
+  template_path = package_dir / "templates" / template
+
+  os.makedirs(path, exist_ok=True)
+
+  for item in template_path.iterdir():
+    dest = Path(path) / item.name
+    if item.is_dir():
+      shutil.copytree(item, dest)
+    else:
+      shutil.copy2(item, dest)
 
-    print(f'Project created!')
+  print(f'Project created!')
```

### Comparing `hal9-2.1.7/hal9/deploy.py` & `hal9-2.1.8/hal9/deploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from hal9.targets.docker import deploy as deploy_docker
 from hal9.targets.hal9 import deploy as deploy_hal9
 
 targets = {
-    'docker': deploy_docker,
-    'hal9': deploy_hal9,
+  'docker': deploy_docker,
+  'hal9': deploy_hal9,
 }
 
 def deploy(path :str, target :str, url :str) -> str:
-    """Deploy an application
+  """Deploy an application
 
-    Parameters
-    ----------
-    path : str 
-            Path to the application.
-    target : str 
-            The deployment target, defaults to 'hal9.com'.
-    """
+  Parameters
+  ----------
+  path : str 
+          Path to the application.
+  target : str 
+          The deployment target, defaults to 'hal9.com'.
+  """
 
-    if target in targets:
-        targets[target](path, url)
-    else:
-        raise Exception(f"Deployment target '{target}' is unsupported.")
+  if target in targets:
+    targets[target](path, url)
+  else:
+    raise Exception(f"Deployment target '{target}' is unsupported.")
```

### Comparing `hal9-2.1.7/hal9/targets/hal9.py` & `hal9-2.1.8/hal9/targets/hal9.py`

 * *Files identical despite different names*

### Comparing `hal9-2.1.7/PKG-INFO` & `hal9-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.1.7
+Version: 2.1.8
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

