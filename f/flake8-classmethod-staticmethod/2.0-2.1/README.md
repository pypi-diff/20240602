# Comparing `tmp/flake8-classmethod-staticmethod-2.0.tar.gz` & `tmp/flake8_classmethod_staticmethod-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-classmethod-staticmethod-2.0.tar", last modified: Fri Jul 14 23:32:20 2023, max compression
+gzip compressed data, was "flake8_classmethod_staticmethod-2.1.tar", last modified: Sun Jun  2 19:02:20 2024, max compression
```

## Comparing `flake8-classmethod-staticmethod-2.0.tar` & `flake8_classmethod_staticmethod-2.1.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:02:20.368062 flake8_classmethod_staticmethod-2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-06-02 19:02:20.368062 flake8_classmethod_staticmethod-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:02:20.364062 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:02:20.368062 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-06-02 19:02:20.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-06-02 19:02:20.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:02:20.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 19:02:20.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:02:20.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-02 19:02:20.000000 flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-06-02 19:02:20.368062 flake8_classmethod_staticmethod-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:02:20.368062 flake8_classmethod_staticmethod-2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/tests/test_csm100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/tests/test_csm101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/tests/test_csm130.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/tests/test_csm131.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/tests/test_csm132.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-02 19:02:12.000000 flake8_classmethod_staticmethod-2.1/tests/test_general.py
```

### Comparing `flake8-classmethod-staticmethod-2.0/LICENSE` & `flake8_classmethod_staticmethod-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-classmethod-staticmethod-2.0/PKG-INFO` & `flake8_classmethod_staticmethod-2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-classmethod-staticmethod
-Version: 2.0
+Version: 2.1
 Summary: flake8 plugin that checks rules regarding the staticmethod and classmethod decorators.
 Home-page: https://github.com/atollk/flake8-classmethod-staticmethod
 Author: Andreas Tollkötter
 License: MIT
 Keywords: flake8,classmethod,staticmethod
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-classmethod-staticmethod
 [![Build Status](https://github.com/atollk/flake8-classmethod-staticmethod/workflows/tox/badge.svg)](https://github.com/atollk/flake8-classmethod-staticmethod/actions)
 [![Build Status](https://github.com/atollk/flake8-classmethod-staticmethod/workflows/black/badge.svg)](https://github.com/atollk/flake8-classmethod-staticmethod/actions)
@@ -89,14 +90,15 @@
 
 `@classmethod` should not be used.
 
 ### CSM131
 
 A method marked as `@classmethod` should access the parameter `cls`.
 Use `@staticmethod` otherwise.
+A special case that is exempt is a method that has a call to `super()`.
 
 **Bad** 
 ```python
 class MyClass:
     @classmethod
     def my_name(cls):
         return "MyClass"
```

### Comparing `flake8-classmethod-staticmethod-2.0/README.md` & `flake8_classmethod_staticmethod-2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
 `@classmethod` should not be used.
 
 ### CSM131
 
 A method marked as `@classmethod` should access the parameter `cls`.
 Use `@staticmethod` otherwise.
+A special case that is exempt is a method that has a call to `super()`.
 
 **Bad** 
 ```python
 class MyClass:
     @classmethod
     def my_name(cls):
         return "MyClass"
```

### Comparing `flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/checker.py` & `flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod/checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,16 +117,29 @@
 def _csm130(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
     yield _error_tuple(130, node)
 
 
 def _csm131(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
     if node.args.args:
         cls_param = node.args.args[0].arg
-        if not _function_uses_identifier(node, cls_param):
-            yield _error_tuple(131, node)
+        if _function_uses_identifier(node, cls_param):
+            return []
+
+        calls = [
+            child for child in ast.walk(node) if isinstance(child, ast.Call)
+        ]
+        for call in calls:
+            if (
+                isinstance(call.func, ast.Name)
+                and call.func.id == "super"
+                and len(call.args) == 0
+            ):
+                return []
+
+        yield _error_tuple(131, node)
 
 
 def _csm132(
     node: ast.FunctionDef, classname: str
 ) -> Iterable[Tuple[int, int, str, type]]:
     if _function_uses_identifier(node, classname):
         yield _error_tuple(132, node)
```

### Comparing `flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/PKG-INFO` & `flake8_classmethod_staticmethod-2.1/flake8_classmethod_staticmethod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-classmethod-staticmethod
-Version: 2.0
+Version: 2.1
 Summary: flake8 plugin that checks rules regarding the staticmethod and classmethod decorators.
 Home-page: https://github.com/atollk/flake8-classmethod-staticmethod
 Author: Andreas Tollkötter
 License: MIT
 Keywords: flake8,classmethod,staticmethod
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-classmethod-staticmethod
 [![Build Status](https://github.com/atollk/flake8-classmethod-staticmethod/workflows/tox/badge.svg)](https://github.com/atollk/flake8-classmethod-staticmethod/actions)
 [![Build Status](https://github.com/atollk/flake8-classmethod-staticmethod/workflows/black/badge.svg)](https://github.com/atollk/flake8-classmethod-staticmethod/actions)
@@ -89,14 +90,15 @@
 
 `@classmethod` should not be used.
 
 ### CSM131
 
 A method marked as `@classmethod` should access the parameter `cls`.
 Use `@staticmethod` otherwise.
+A special case that is exempt is a method that has a call to `super()`.
 
 **Bad** 
 ```python
 class MyClass:
     @classmethod
     def my_name(cls):
         return "MyClass"
```

### Comparing `flake8-classmethod-staticmethod-2.0/setup.cfg` & `flake8_classmethod_staticmethod-2.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8-classmethod-staticmethod
-version = 2.0
+version = 2.1
 description = flake8 plugin that checks rules regarding the staticmethod and classmethod decorators.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Andreas Tollkötter
 url = https://github.com/atollk/flake8-classmethod-staticmethod
 license = MIT
 license_file = LICENSE
@@ -16,14 +16,15 @@
 	Natural Language :: English
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = 
 	flake8_classmethod_staticmethod
 include_package_data = True
 python_requires = >=3.8
 zip_safe = False
```

