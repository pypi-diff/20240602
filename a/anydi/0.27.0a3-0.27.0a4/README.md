# Comparing `tmp/anydi-0.27.0a3.tar.gz` & `tmp/anydi-0.27.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.27.0a3.tar", max compression
+gzip compressed data, was "anydi-0.27.0a4.tar", max compression
```

## Comparing `anydi-0.27.0a3.tar` & `anydi-0.27.0a4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.27.0a3/LICENSE
--rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.27.0a3/README.md
--rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.27.0a3/anydi/__init__.py
--rw-r--r--   0        0        0    29631 2024-06-02 14:15:07.268714 anydi-0.27.0a3/anydi/_container.py
--rw-r--r--   0        0        0    10815 2024-05-28 05:51:36.811241 anydi-0.27.0a3/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.27.0a3/anydi/_logger.py
--rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.27.0a3/anydi/_module.py
--rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.27.0a3/anydi/_scanner.py
--rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.27.0a3/anydi/_types.py
--rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.27.0a3/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.27.0a3/anydi/ext/__init__.py
--rw-r--r--   0        0        0     2691 2024-06-02 14:18:27.849442 anydi-0.27.0a3/anydi/ext/_utils.py
--rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.27.0a3/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.27.0a3/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.27.0a3/anydi/ext/django/_settings.py
--rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.27.0a3/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.27.0a3/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.27.0a3/anydi/ext/django/middleware.py
--rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.27.0a3/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.27.0a3/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.27.0a3/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     2896 2024-06-02 14:18:27.850113 anydi-0.27.0a3/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     1916 2024-06-02 14:32:36.778643 anydi-0.27.0a3/anydi/ext/faststream.py
--rw-r--r--   0        0        0     4242 2024-06-02 14:18:33.987372 anydi-0.27.0a3/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.27.0a3/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.27.0a3/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.27.0a3/anydi/py.typed
--rw-r--r--   0        0        0     3133 2024-06-02 14:33:04.166439 anydi-0.27.0a3/pyproject.toml
--rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 anydi-0.27.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.27.0a4/LICENSE
+-rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.27.0a4/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.27.0a4/anydi/__init__.py
+-rw-r--r--   0        0        0    29631 2024-06-02 14:15:07.268714 anydi-0.27.0a4/anydi/_container.py
+-rw-r--r--   0        0        0    10815 2024-05-28 05:51:36.811241 anydi-0.27.0a4/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.27.0a4/anydi/_logger.py
+-rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.27.0a4/anydi/_module.py
+-rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.27.0a4/anydi/_scanner.py
+-rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.27.0a4/anydi/_types.py
+-rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.27.0a4/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.27.0a4/anydi/ext/__init__.py
+-rw-r--r--   0        0        0     2691 2024-06-02 14:18:27.849442 anydi-0.27.0a4/anydi/ext/_utils.py
+-rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.27.0a4/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.27.0a4/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.27.0a4/anydi/ext/django/_settings.py
+-rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.27.0a4/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.27.0a4/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.27.0a4/anydi/ext/django/middleware.py
+-rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.27.0a4/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.27.0a4/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.27.0a4/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     2896 2024-06-02 14:18:27.850113 anydi-0.27.0a4/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     1916 2024-06-02 14:32:36.778643 anydi-0.27.0a4/anydi/ext/faststream.py
+-rw-r--r--   0        0        0     4242 2024-06-02 14:18:33.987372 anydi-0.27.0a4/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.27.0a4/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.27.0a4/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.27.0a4/anydi/py.typed
+-rw-r--r--   0        0        0     3150 2024-06-02 15:15:42.902850 anydi-0.27.0a4/pyproject.toml
+-rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 anydi-0.27.0a4/PKG-INFO
```

### Comparing `anydi-0.27.0a3/LICENSE` & `anydi-0.27.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/README.md` & `anydi-0.27.0a4/README.md`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/__init__.py` & `anydi-0.27.0a4/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/_container.py` & `anydi-0.27.0a4/anydi/_container.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/_context.py` & `anydi-0.27.0a4/anydi/_context.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/_module.py` & `anydi-0.27.0a4/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/_scanner.py` & `anydi-0.27.0a4/anydi/_scanner.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/_types.py` & `anydi-0.27.0a4/anydi/_types.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/_utils.py` & `anydi-0.27.0a4/anydi/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/_utils.py` & `anydi-0.27.0a4/anydi/ext/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/django/_settings.py` & `anydi-0.27.0a4/anydi/ext/django/_settings.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/django/_utils.py` & `anydi-0.27.0a4/anydi/ext/django/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/django/apps.py` & `anydi-0.27.0a4/anydi/ext/django/apps.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/django/middleware.py` & `anydi-0.27.0a4/anydi/ext/django/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/django/ninja/__init__.py` & `anydi-0.27.0a4/anydi/ext/django/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/django/ninja/_operation.py` & `anydi-0.27.0a4/anydi/ext/django/ninja/_operation.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/django/ninja/_signature.py` & `anydi-0.27.0a4/anydi/ext/django/ninja/_signature.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/fastapi.py` & `anydi-0.27.0a4/anydi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/faststream.py` & `anydi-0.27.0a4/anydi/ext/faststream.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/pytest_plugin.py` & `anydi-0.27.0a4/anydi/ext/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/anydi/ext/starlette/middleware.py` & `anydi-0.27.0a4/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a3/pyproject.toml` & `anydi-0.27.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.27.0a3"
+version = "0.27.0a4"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
@@ -52,14 +52,15 @@
 pytest-cov = "^5.0.0"
 fastapi = "^0.100.0"
 httpx = "^0.26.0"
 django = "^4.2"
 django-ninja = "^1.1.0"
 pytest-django = "^4.8.0"
 faststream = "^0.5.10"
+redis = "^5.0.4"
 
 [tool.poetry.plugins.pytest11]
 anydi = "anydi.ext.pytest_plugin"
 
 [tool.ruff]
 line-length = 88
```

### Comparing `anydi-0.27.0a3/PKG-INFO` & `anydi-0.27.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.27.0a3
+Version: 0.27.0a4
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
```

