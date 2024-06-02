# Comparing `tmp/ch9329-1.2.3.tar.gz` & `tmp/ch9329-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.2.3.tar", last modified: Sun Jun  2 17:52:09 2024, max compression
+gzip compressed data, was "ch9329-1.2.4.tar", last modified: Sun Jun  2 17:56:42 2024, max compression
```

## Comparing `ch9329-1.2.3.tar` & `ch9329-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.363115 ch9329-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-02 17:52:04.000000 ch9329-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 17:52:04.000000 ch9329-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-06-02 17:52:09.363115 ch9329-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-02 17:52:04.000000 ch9329-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.359115 ch9329-1.2.3/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.363115 ch9329-1.2.3/ch9329/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/tools/lsch9329.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 17:52:04.000000 ch9329-1.2.3/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:09.363115 ch9329-1.2.3/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 17:52:09.000000 ch9329-1.2.3/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-06-02 17:52:04.000000 ch9329-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:52:09.363115 ch9329-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:56:42.906388 ch9329-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-02 17:56:31.000000 ch9329-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 17:56:31.000000 ch9329-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-06-02 17:56:42.906388 ch9329-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-02 17:56:31.000000 ch9329-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:56:42.902388 ch9329-1.2.4/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:56:42.902388 ch9329-1.2.4/ch9329/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/tools/lsch9329.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 17:56:31.000000 ch9329-1.2.4/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:56:42.906388 ch9329-1.2.4/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-06-02 17:56:42.000000 ch9329-1.2.4/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-02 17:56:42.000000 ch9329-1.2.4/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:56:42.000000 ch9329-1.2.4/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 17:56:42.000000 ch9329-1.2.4/ch9329.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 17:56:42.000000 ch9329-1.2.4/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 17:56:42.000000 ch9329-1.2.4/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-06-02 17:56:31.000000 ch9329-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:56:42.906388 ch9329-1.2.4/setup.cfg
```

### Comparing `ch9329-1.2.3/LICENSE` & `ch9329-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.3/PKG-INFO` & `ch9329-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.2.3/README.md` & `ch9329-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.3/ch9329/config.py` & `ch9329-1.2.4/ch9329/config.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.3/ch9329/hid.py` & `ch9329-1.2.4/ch9329/hid.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.3/ch9329/keyboard.py` & `ch9329-1.2.4/ch9329/keyboard.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.3/ch9329/mouse.py` & `ch9329-1.2.4/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.3/ch9329/tools/lsch9329.py` & `ch9329-1.2.4/ch9329/tools/lsch9329.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     for i in serial.tools.list_ports.comports():
         if i.vid == 6790 and i.pid == 29987:
             try:
                 ser = Serial(i.name, 9600, timeout=0.05)
                 serial_number = get_serial_number(ser)
                 print(
                     f"serial_number={serial_number}, "
-                    f"name={i.name}, "
+                    f"name={i.device}, "
                     f"location={i.location}"
                 )
                 ser.close()
             except serial.serialutil.SerialException:
                 print(
                     f"serial_number=error, "
                     f"name={i.name}, "
```

### Comparing `ch9329-1.2.3/ch9329/utils.py` & `ch9329-1.2.4/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.3/ch9329.egg-info/PKG-INFO` & `ch9329-1.2.4/ch9329.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.2.3/pyproject.toml` & `ch9329-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.2.3"
+version = "1.2.4"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

