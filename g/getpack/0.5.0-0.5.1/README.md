# Comparing `tmp/getpack-0.5.0.tar.gz` & `tmp/getpack-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpack-0.5.0.tar", last modified: Sat Jun  1 23:02:48 2024, max compression
+gzip compressed data, was "getpack-0.5.1.tar", last modified: Sat Jun  1 23:01:40 2024, max compression
```

## Comparing `getpack-0.5.0.tar` & `getpack-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 23:02:48.386943 getpack-0.5.0/
--rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     2514 2024-06-01 23:02:48.386943 getpack-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1819 2024-06-01 23:02:33.000000 getpack-0.5.0/README.md
--rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0     1088 2024-06-01 23:02:48.391932 getpack-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:02:48.264762 getpack-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 23:02:48.310931 getpack-0.5.0/src/getpack/
--rw-rw-rw-   0        0        0      618 2024-06-01 23:02:33.000000 getpack-0.5.0/src/getpack/__init__.py
--rw-rw-rw-   0        0        0     3577 2024-05-31 15:10:51.000000 getpack-0.5.0/src/getpack/executable.py
--rw-rw-rw-   0        0        0     1926 2023-08-09 21:03:35.000000 getpack-0.5.0/src/getpack/extraction.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:02:48.375238 getpack-0.5.0/src/getpack/library/
--rw-rw-rw-   0        0        0     3024 2024-02-10 21:59:25.000000 getpack-0.5.0/src/getpack/library/__init__.py
--rw-rw-rw-   0        0        0    13006 2024-06-01 23:02:33.000000 getpack-0.5.0/src/getpack/resource.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:02:48.371937 getpack-0.5.0/src/getpack.egg-info/
--rw-rw-rw-   0        0        0     2514 2024-06-01 23:02:48.000000 getpack-0.5.0/src/getpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2024-06-01 23:02:48.000000 getpack-0.5.0/src/getpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 23:02:48.000000 getpack-0.5.0/src/getpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2024-06-01 23:02:48.000000 getpack-0.5.0/src/getpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 23:02:48.000000 getpack-0.5.0/src/getpack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 23:02:48.384932 getpack-0.5.0/tests/
--rw-rw-rw-   0        0        0     2467 2024-06-01 23:02:25.000000 getpack-0.5.0/tests/test_common.py
--rw-rw-rw-   0        0        0     1698 2024-06-01 22:54:29.000000 getpack-0.5.0/tests/test_concurrency.py
--rw-rw-rw-   0        0        0      647 2024-06-01 23:02:25.000000 getpack-0.5.0/tests/test_executable.py
--rw-rw-rw-   0        0        0      496 2024-05-31 15:37:58.000000 getpack-0.5.0/tests/test_unicode.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:01:40.929687 getpack-0.5.1/
+-rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     2577 2024-06-01 23:01:40.930544 getpack-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-06-01 22:30:28.000000 getpack-0.5.1/README.md
+-rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1088 2024-06-01 23:01:40.937543 getpack-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:01:40.829546 getpack-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 23:01:40.889090 getpack-0.5.1/src/getpack/
+-rw-rw-rw-   0        0        0      618 2024-06-01 23:00:40.000000 getpack-0.5.1/src/getpack/__init__.py
+-rw-rw-rw-   0        0        0     3577 2024-05-31 15:10:51.000000 getpack-0.5.1/src/getpack/executable.py
+-rw-rw-rw-   0        0        0     1926 2023-08-09 21:03:35.000000 getpack-0.5.1/src/getpack/extraction.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:01:40.916547 getpack-0.5.1/src/getpack/library/
+-rw-rw-rw-   0        0        0     3024 2024-02-10 21:59:25.000000 getpack-0.5.1/src/getpack/library/__init__.py
+-rw-rw-rw-   0        0        0    13145 2024-06-01 22:54:57.000000 getpack-0.5.1/src/getpack/resource.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:01:40.914544 getpack-0.5.1/src/getpack.egg-info/
+-rw-rw-rw-   0        0        0     2577 2024-06-01 23:01:40.000000 getpack-0.5.1/src/getpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2024-06-01 23:01:40.000000 getpack-0.5.1/src/getpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 23:01:40.000000 getpack-0.5.1/src/getpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2024-06-01 23:01:40.000000 getpack-0.5.1/src/getpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 23:01:40.000000 getpack-0.5.1/src/getpack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 23:01:40.926846 getpack-0.5.1/tests/
+-rw-rw-rw-   0        0        0     2467 2024-06-01 22:55:19.000000 getpack-0.5.1/tests/test_common.py
+-rw-rw-rw-   0        0        0     1698 2024-06-01 22:54:29.000000 getpack-0.5.1/tests/test_concurrency.py
+-rw-rw-rw-   0        0        0      647 2024-06-01 22:51:44.000000 getpack-0.5.1/tests/test_executable.py
+-rw-rw-rw-   0        0        0      496 2024-05-31 15:37:58.000000 getpack-0.5.1/tests/test_unicode.py
```

### Comparing `getpack-0.5.0/LICENSE` & `getpack-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getpack-0.5.0/PKG-INFO` & `getpack-0.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.5.0
+Version: 0.5.1
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Platform: UNKNOWN
@@ -57,9 +57,10 @@
 ### Testings
 For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
 
 ### Environs
 * `GETPACK_RETRIES` - int, number of general retries, used for renaming and
     removing temporary folders
 * `GETPACK_BACKOFF` - float, delay between retires
+* `GETPACK_ROOT` - str, default root folder for all resources
```

### Comparing `getpack-0.5.0/README.md` & `getpack-0.5.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -39,7 +39,8 @@
 ### Testings
 For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
 
 ### Environs
 * `GETPACK_RETRIES` - int, number of general retries, used for renaming and
     removing temporary folders
 * `GETPACK_BACKOFF` - float, delay between retires
+* `GETPACK_ROOT` - str, default root folder for all resources
```

### Comparing `getpack-0.5.0/setup.cfg` & `getpack-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `getpack-0.5.0/src/getpack/__init__.py` & `getpack-0.5.1/src/getpack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Copyright (c) 2022 Konstantin Maslyuk. All rights reserved.
 
 This work is licensed under the terms of the MIT license.
 For a copy, see <https://opensource.org/licenses/MIT>.
 """
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 from .executable import Executable, LocalExecutable  # noqa: F401
 from .resource import (  # noqa: F401
     LocalResource,
     PyPiPackage,
     PythonPackage,
     Resource,
```

### Comparing `getpack-0.5.0/src/getpack/executable.py` & `getpack-0.5.1/src/getpack/executable.py`

 * *Files identical despite different names*

### Comparing `getpack-0.5.0/src/getpack/extraction.py` & `getpack-0.5.1/src/getpack/extraction.py`

 * *Files identical despite different names*

### Comparing `getpack-0.5.0/src/getpack/library/__init__.py` & `getpack-0.5.1/src/getpack/library/__init__.py`

 * *Files identical despite different names*

### Comparing `getpack-0.5.0/src/getpack/resource.py` & `getpack-0.5.1/src/getpack/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,18 +170,22 @@
 
     def cleanup(self):
         raise NotImplementedError
 
 
 class LocalResource(Resource):
     """Locally cached resource."""
-    if sys.platform == 'win32':
-        local_base = Path(os.getenv('APPDATA')) / 'getpack'
-    elif sys.platform == 'linux':
-        local_base = Path(os.environ['HOME']) / '.config' / 'getpack'
+    local_base = os.getenv('GETPACK_ROOT')  # type: Path
+    if local_base:
+        local_base = Path(local_base)
+    else:
+        if sys.platform == 'win32':
+            local_base = Path(os.getenv('APPDATA')) / 'getpack'
+        elif sys.platform == 'linux':
+            local_base = Path(os.getenv('HOME')) / '.config' / 'getpack'
     local_prefix = ''
     _path = None
 
     @property
     def path(self):  # type: () -> Path
         if self._path is None:
             assert self.name, 'Resource should be named'
```

### Comparing `getpack-0.5.0/src/getpack.egg-info/PKG-INFO` & `getpack-0.5.1/src/getpack.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpack
-Version: 0.5.0
+Version: 0.5.1
 Summary: Declarative external resources with implicit deployment
 Home-page: https://github.com/kalemas/getpack
 Author: Konstantin Maslyuk
 Author-email: Kostya.Maslyuk@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
 Platform: UNKNOWN
@@ -57,9 +57,10 @@
 ### Testings
 For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
 
 ### Environs
 * `GETPACK_RETRIES` - int, number of general retries, used for renaming and
     removing temporary folders
 * `GETPACK_BACKOFF` - float, delay between retires
+* `GETPACK_ROOT` - str, default root folder for all resources
```

### Comparing `getpack-0.5.0/tests/test_common.py` & `getpack-0.5.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `getpack-0.5.0/tests/test_concurrency.py` & `getpack-0.5.1/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `getpack-0.5.0/tests/test_executable.py` & `getpack-0.5.1/tests/test_executable.py`

 * *Files identical despite different names*

