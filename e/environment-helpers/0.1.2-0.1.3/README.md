# Comparing `tmp/environment_helpers-0.1.2.tar.gz` & `tmp/environment_helpers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "environment_helpers-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "environment_helpers-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `environment_helpers-0.1.2.tar` & `environment_helpers-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/LICENSE
--rw-r--r--   0        0        0      195 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/README.md
--rw-r--r--   0        0        0     4056 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/__init__.py
--rw-r--r--   0        0        0      422 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/call.py
--rw-r--r--   0        0        0      348 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/launcher-kind.py
--rw-r--r--   0        0        0      188 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/scheme.py
--rw-r--r--   0        0        0     2033 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/system-scheme.py
--rw-r--r--   0        0        0      197 2024-05-29 12:42:27.075752 environment_helpers-0.1.2/environment_helpers/_scripts/version.py
--rw-r--r--   0        0        0     2148 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/build.py
--rw-r--r--   0        0        0     1049 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/install.py
--rw-r--r--   0        0        0     4835 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/environment_helpers/introspect.py
--rw-r--r--   0        0        0     1888 2024-05-31 18:15:50.263386 environment_helpers-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 environment_helpers-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-29 12:42:27.075752 environment_helpers-0.1.3/LICENSE
+-rw-r--r--   0        0        0      195 2024-05-29 12:42:27.075752 environment_helpers-0.1.3/README.md
+-rw-r--r--   0        0        0     4056 2024-06-02 01:21:58.473979 environment_helpers-0.1.3/environment_helpers/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-29 12:42:27.075752 environment_helpers-0.1.3/environment_helpers/_scripts/call.py
+-rw-r--r--   0        0        0      348 2024-05-29 12:42:27.075752 environment_helpers-0.1.3/environment_helpers/_scripts/launcher-kind.py
+-rw-r--r--   0        0        0      188 2024-05-29 12:42:27.075752 environment_helpers-0.1.3/environment_helpers/_scripts/scheme.py
+-rw-r--r--   0        0        0     2033 2024-05-29 12:42:27.075752 environment_helpers-0.1.3/environment_helpers/_scripts/system-scheme.py
+-rw-r--r--   0        0        0      197 2024-05-29 12:42:27.075752 environment_helpers-0.1.3/environment_helpers/_scripts/version.py
+-rw-r--r--   0        0        0     2148 2024-05-31 18:15:50.263386 environment_helpers-0.1.3/environment_helpers/build.py
+-rw-r--r--   0        0        0     1049 2024-05-31 18:15:50.263386 environment_helpers-0.1.3/environment_helpers/install.py
+-rw-r--r--   0        0        0     4496 2024-06-02 01:21:58.473979 environment_helpers-0.1.3/environment_helpers/introspect.py
+-rw-r--r--   0        0        0     1831 2024-06-02 01:21:58.473979 environment_helpers-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 environment_helpers-0.1.3/PKG-INFO
```

### Comparing `environment_helpers-0.1.2/LICENSE` & `environment_helpers-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.2/environment_helpers/__init__.py` & `environment_helpers-0.1.3/environment_helpers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from typing import Any, Collection, Literal, Optional, Protocol
 
 import environment_helpers.build
 import environment_helpers.install
 import environment_helpers.introspect
 
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 
 class Environment(Protocol):
     """Object representing a Python environment."""
 
     @property
     def base(self) -> pathlib.Path: ...
```

### Comparing `environment_helpers-0.1.2/environment_helpers/_scripts/system-scheme.py` & `environment_helpers-0.1.3/environment_helpers/_scripts/system-scheme.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.2/environment_helpers/build.py` & `environment_helpers-0.1.3/environment_helpers/build.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.2/environment_helpers/install.py` & `environment_helpers-0.1.3/environment_helpers/install.py`

 * *Files identical despite different names*

### Comparing `environment_helpers-0.1.2/environment_helpers/introspect.py` & `environment_helpers-0.1.3/environment_helpers/introspect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from __future__ import annotations
 
 import functools
 import json
 import os
+import pathlib
 import pickle
 import subprocess
-import sys
 import sysconfig
 import warnings
 
 from typing import Any, Callable, Literal, NamedTuple, Optional, TypedDict, TypeVar, Union
 
 
-if sys.version_info >= (3, 9):
-    import importlib.resources as importlib_resources
-else:
-    import importlib_resources
-
-
 LauncherKind = Literal['posix', 'win-ia32', 'win-amd64', 'win-arm', 'win-arm64']
 
 T = TypeVar('T')
 
 
 class SchemeDict(TypedDict):
     stdlib: str
@@ -68,19 +62,16 @@
 
 
 class Introspectable:
     def __init__(self, interpreter: os.PathLike[str]) -> None:
         self._interpreter = interpreter
 
     def _run_script(self, name: str, **kwargs: Any) -> Any:
-        script = importlib_resources.files('environment_helpers._scripts') / f'{name}.py'
-        with importlib_resources.as_file(script) as script_path:
-            data = subprocess.check_output(
-                [os.fspath(self._interpreter), os.fspath(script_path)], **kwargs
-            )
+        script = pathlib.Path(__file__).parent / '_scripts' / f'{name}.py'
+        data = subprocess.check_output([os.fspath(self._interpreter), os.fspath(script)], **kwargs)
         return json.loads(data)
 
     def get_version(self) -> PythonVersion:
         data = self._run_script('version')
         return PythonVersion(**data)
 
     @functools.lru_cache
@@ -129,15 +120,14 @@
         else:
             module = func.__module__
             func_name = func.__qualname__
 
         args_dict = {'args': args, 'kwargs': kwargs}
         pickled_args_dict = pickle.dumps(args_dict)
 
-        script = importlib_resources.files('environment_helpers._scripts') / 'call.py'
-        with importlib_resources.as_file(script) as script_path:
-            data = subprocess.check_output(
-                [os.fspath(self._interpreter), os.fspath(script_path), module, func_name],
-                input=pickled_args_dict,
-            )
+        script = pathlib.Path(__file__).parent / '_scripts' / f'call.py'
+        data = subprocess.check_output(
+            [os.fspath(self._interpreter), os.fspath(script), module, func_name],
+            input=pickled_args_dict,
+        )
 
         return pickle.loads(data)
```

### Comparing `environment_helpers-0.1.2/pyproject.toml` & `environment_helpers-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['flit-core >= 3.4']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'environment-helpers'
-version = '0.1.2'
+version = '0.1.3'
 description = 'Collection of helpers for managing Python environments'
 readme = 'README.md'
 requires-python = '>= 3.8'
 license.file = 'LICENSE'
 authors = [
   { name = 'Filipe Laíns', email = 'lains@riseup.net' },
 ]
@@ -27,15 +27,14 @@
 ]
 urls.homepage = 'https://github.com/FFY00/environment-helpers'
 urls.changelog = 'https://environment-helpers.readthedocs.io/en/stable/changelog.html'
 
 dependencies = [
   'build >= 0.5.0',
   'installer >= 0.5.0',
-  'importlib_resources >= 5.0; python_version < "3.10"',
 ]
 
 [project.optional-dependencies]
 test = [
   'pytest >= 7',
   'podman >= 5',
 ]
```

### Comparing `environment_helpers-0.1.2/PKG-INFO` & `environment_helpers-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environment-helpers
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of helpers for managing Python environments
 Author-email: Filipe Laíns <lains@riseup.net>
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: build >= 0.5.0
 Requires-Dist: installer >= 0.5.0
-Requires-Dist: importlib_resources >= 5.0; python_version < "3.10"
 Requires-Dist: pytest >= 7 ; extra == "test"
 Requires-Dist: podman >= 5 ; extra == "test"
 Project-URL: changelog, https://environment-helpers.readthedocs.io/en/stable/changelog.html
 Project-URL: homepage, https://github.com/FFY00/environment-helpers
 Provides-Extra: test
 
 # environment-helpers
```

