# Comparing `tmp/ch9329-1.2.2.tar.gz` & `tmp/ch9329-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.2.2.tar", last modified: Thu May 30 18:14:46 2024, max compression
+gzip compressed data, was "ch9329-1.2.3.tar", last modified: Sun Jun  2 17:52:09 2024, max compression
```

## Comparing `ch9329-1.2.2.tar` & `ch9329-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:14:46.738952 ch9329-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 18:14:42.000000 ch9329-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 18:14:42.000000 ch9329-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 18:14:46.738952 ch9329-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 18:14:42.000000 ch9329-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:14:46.738952 ch9329-1.2.2/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 18:14:42.000000 ch9329-1.2.2/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:14:46.738952 ch9329-1.2.2/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 18:14:46.000000 ch9329-1.2.2/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 18:14:46.000000 ch9329-1.2.2/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:14:46.000000 ch9329-1.2.2/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 18:14:46.000000 ch9329-1.2.2/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 18:14:46.000000 ch9329-1.2.2/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 18:14:42.000000 ch9329-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:14:46.738952 ch9329-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.363115 ch9329-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-02 17:52:04.000000 ch9329-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 17:52:04.000000 ch9329-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-06-02 17:52:09.363115 ch9329-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-02 17:52:04.000000 ch9329-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.359115 ch9329-1.2.3/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.363115 ch9329-1.2.3/ch9329/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/tools/lsch9329.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.363115 ch9329-1.2.3/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-06-02 17:52:04.000000 ch9329-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:52:09.363115 ch9329-1.2.3/setup.cfg
```

### Comparing `ch9329-1.2.2/LICENSE` & `ch9329-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.2/PKG-INFO` & `ch9329-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.2.2/README.md` & `ch9329-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.2/ch9329/config.py` & `ch9329-1.2.3/ch9329/config.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.2/ch9329/hid.py` & `ch9329-1.2.3/ch9329/hid.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.2/ch9329/keyboard.py` & `ch9329-1.2.3/ch9329/keyboard.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.2/ch9329/mouse.py` & `ch9329-1.2.3/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.2/ch9329/utils.py` & `ch9329-1.2.3/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.2/ch9329.egg-info/PKG-INFO` & `ch9329-1.2.3/ch9329.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.2.2/pyproject.toml` & `ch9329-1.2.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.2.2"
+version = "1.2.3"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
 classifiers = ["Programming Language :: Python :: 3"]
 
 [project.urls]
 Homepage = "https://github.com/sandbox-pokhara/ch9329"
 Issues = "https://github.com/sandbox-pokhara/ch9329/issues"
 
+[project.scripts]
+lsch9329 = "ch9329.tools.lsch9329:main"
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-dir]
 "ch9329" = "ch9329"
 
 [tool.isort]
```

