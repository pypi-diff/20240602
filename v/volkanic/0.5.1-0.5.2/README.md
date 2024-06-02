# Comparing `tmp/volkanic-0.5.1.tar.gz` & `tmp/volkanic-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volkanic-0.5.1.tar", last modified: Wed Apr 12 09:14:23 2023, max compression
+gzip compressed data, was "volkanic-0.5.2.tar", last modified: Sun Jun  2 10:12:35 2024, max compression
```

## Comparing `volkanic-0.5.1.tar` & `volkanic-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-12 09:14:23.243231 volkanic-0.5.1/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2019-04-25 10:44:00.000000 volkanic-0.5.1/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       25 2019-01-21 17:03:54.000000 volkanic-0.5.1/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     4714 2023-04-12 09:14:23.242869 volkanic-0.5.1/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     3987 2021-09-05 13:58:09.000000 volkanic-0.5.1/README.md
--rw-r--r--   0 Hailong    (502) staff       (20)       12 2022-02-03 05:01:45.000000 volkanic-0.5.1/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2023-04-12 09:14:23.243389 volkanic-0.5.1/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2093 2022-05-12 11:43:32.000000 volkanic-0.5.1/setup.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-12 09:14:23.238583 volkanic-0.5.1/volkanic/
--rw-r--r--   0 Hailong    (502) staff       (20)      203 2023-04-12 09:14:04.000000 volkanic-0.5.1/volkanic/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)      896 2022-01-21 13:22:00.000000 volkanic-0.5.1/volkanic/__main__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     4278 2022-04-18 13:34:09.000000 volkanic-0.5.1/volkanic/cmdline.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1085 2022-04-18 13:34:57.000000 volkanic-0.5.1/volkanic/compat.py
--rw-r--r--   0 Hailong    (502) staff       (20)     8403 2023-04-07 02:22:23.000000 volkanic-0.5.1/volkanic/environ.py
--rw-r--r--   0 Hailong    (502) staff       (20)      614 2023-04-12 09:14:04.000000 volkanic-0.5.1/volkanic/errors.py
--rw-r--r--   0 Hailong    (502) staff       (20)     8787 2023-04-07 02:22:23.000000 volkanic-0.5.1/volkanic/introspect.py
--rw-r--r--   0 Hailong    (502) staff       (20)     6229 2023-04-07 02:22:23.000000 volkanic-0.5.1/volkanic/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-04-12 09:14:23.242338 volkanic-0.5.1/volkanic.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     4714 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      441 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       52 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/entry_points.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2021-08-14 03:53:40.000000 volkanic-0.5.1/volkanic.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       13 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        9 2023-04-12 09:14:23.000000 volkanic-0.5.1/volkanic.egg-info/top_level.txt
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 10:12:35.670417 volkanic-0.5.2/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2019-04-25 10:44:00.000000 volkanic-0.5.2/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       25 2019-01-21 17:03:54.000000 volkanic-0.5.2/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     4714 2024-06-02 10:12:35.670162 volkanic-0.5.2/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     3987 2021-09-05 13:58:09.000000 volkanic-0.5.2/README.md
+-rw-r--r--   0 Hailong    (502) staff       (20)       12 2022-02-03 05:01:45.000000 volkanic-0.5.2/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-06-02 10:12:35.670526 volkanic-0.5.2/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2093 2022-05-12 11:43:32.000000 volkanic-0.5.2/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 10:12:35.666805 volkanic-0.5.2/volkanic/
+-rw-r--r--   0 Hailong    (502) staff       (20)      203 2024-06-02 10:12:05.000000 volkanic-0.5.2/volkanic/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      896 2022-01-21 13:22:00.000000 volkanic-0.5.2/volkanic/__main__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     4370 2023-09-12 01:50:37.000000 volkanic-0.5.2/volkanic/cmdline.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1201 2024-06-02 10:11:07.000000 volkanic-0.5.2/volkanic/compat.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     8435 2023-05-19 02:28:21.000000 volkanic-0.5.2/volkanic/environ.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      614 2023-04-12 09:14:04.000000 volkanic-0.5.2/volkanic/errors.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     8787 2023-04-07 02:22:23.000000 volkanic-0.5.2/volkanic/introspect.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     6936 2024-06-02 10:11:07.000000 volkanic-0.5.2/volkanic/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 10:12:35.669673 volkanic-0.5.2/volkanic.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     4714 2024-06-02 10:12:35.000000 volkanic-0.5.2/volkanic.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      441 2024-06-02 10:12:35.000000 volkanic-0.5.2/volkanic.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-06-02 10:12:35.000000 volkanic-0.5.2/volkanic.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-06-02 10:12:35.000000 volkanic-0.5.2/volkanic.egg-info/entry_points.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2021-08-14 03:53:40.000000 volkanic-0.5.2/volkanic.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       13 2024-06-02 10:12:35.000000 volkanic-0.5.2/volkanic.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        9 2024-06-02 10:12:35.000000 volkanic-0.5.2/volkanic.egg-info/top_level.txt
```

### Comparing `volkanic-0.5.1/LICENSE` & `volkanic-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.1/PKG-INFO` & `volkanic-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkanic
-Version: 0.5.1
+Version: 0.5.2
 Summary: access config and CLI easily and elegantly
 Home-page: https://github.com/frozflame/volkanic
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `volkanic-0.5.1/README.md` & `volkanic-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.1/setup.py` & `volkanic-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.1/volkanic/__main__.py` & `volkanic-0.5.2/volkanic/__main__.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.1/volkanic/cmdline.py` & `volkanic-0.5.2/volkanic/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 from collections import OrderedDict
 from typing import Union
 
 from volkanic.utils import load_symbol
 
 
 @contextlib.contextmanager
-def remember_cwd(path=None):
+def temporary_cwd(path=None):
     """Temporarily change Current Working Directory (CWD/PWD)"""
     prev_cwd = os.getcwd()
     if path:
         os.chdir(path)
     try:
         yield
     finally:
         os.chdir(prev_cwd)
 
 
+# for backward compatiblity.
+# will be removed in ver 0.7.0
+remember_cwd = temporary_cwd
+
+
 def _flatten_recursively(tup: Union[tuple, list]) -> list:
     """
     >>> _flatten_recursively((1, (2, (3, 4))))
     [1, 2, 3, 4]
     """
     stack = list(tup)
     values = []
```

### Comparing `volkanic-0.5.1/volkanic/compat.py` & `volkanic-0.5.2/volkanic/compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,19 @@
         def __init__(self, func):
             self.__doc__ = getattr(func, "__doc__")
             self.func = func
 
         def __get__(self, obj, cls):
             if obj is None:
                 return self
-            value = obj.__dict__[self.func.__name__] = self.func(obj)
-            return value
+            try:
+                return obj.__dict__[self.func.__name__]
+            except KeyError:
+                val = self.func(obj)
+                return obj.__dict__.setdefault(self.func.__name__, val)
 
 
 def abstract_property(func):
     if sys.version_info > (3, 3):
         return property(abc.abstractmethod(func))
     else:
         return abc.abstractproperty(func)
```

### Comparing `volkanic-0.5.1/volkanic/environ.py` & `volkanic-0.5.2/volkanic/environ.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,18 @@
         'confpath_filename': 'config.json5',
     }
 
     # default config and log format
     default_config = {
         '_jinja2_env': {},
     }
-    default_logfmt = \
-        '%(asctime)s %(levelname)s [%(process)s,%(thread)s] %(name)s %(message)s'
+    default_logfmt = (
+        "%(asctime)s %(levelname)s [%(process)s,%(thread)s] "
+        "%(name)s %(funcName)s() %(message)s"
+    )
 
     @classmethod
     def _fmt_envvar_name(cls, name):
         return '{}_{}'.format(cls.identifier, name).upper()
 
     @classmethod
     def _get_option(cls, key: str):
```

### Comparing `volkanic-0.5.1/volkanic/errors.py` & `volkanic-0.5.2/volkanic/errors.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.1/volkanic/introspect.py` & `volkanic-0.5.2/volkanic/introspect.py`

 * *Files identical despite different names*

### Comparing `volkanic-0.5.1/volkanic/utils.py` & `volkanic-0.5.2/volkanic/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,7 +246,32 @@
         return 'application/pdf'
     if content.startswith(b'\x89PNG\r\n\x1a\n'):
         return 'image/png'
     if content.startswith(b'\xFF\xD8\xFF\xE0'):
         return 'image/jpeg'
     if content.startswith(b'\xFF\xD8\xFF\xEE'):
         return 'image/jpeg'
+
+
+# noinspection PyPep8Naming
+class per_process_cached_property:
+    """
+    A property that is only computed once per instance per process.
+    Deleting the attribute resets the property.
+    """
+
+    def __init__(self, func):
+        self.__doc__ = getattr(func, "__doc__")
+        self.func = func
+
+    def __get__(self, obj, cls):
+        if obj is None:
+            return self
+        key = self.func.__name__
+        current_pid = os.getpid()
+        if key in obj.__dict__:
+            val, pid = obj.__dict__[key]
+            if current_pid == pid:
+                return val
+        val = self.func(obj)
+        obj.__dict__.setdefault(key, (val, current_pid))
+        return obj.__dict__[key][0]
```

### Comparing `volkanic-0.5.1/volkanic.egg-info/PKG-INFO` & `volkanic-0.5.2/volkanic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkanic
-Version: 0.5.1
+Version: 0.5.2
 Summary: access config and CLI easily and elegantly
 Home-page: https://github.com/frozflame/volkanic
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

