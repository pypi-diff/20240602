# Comparing `tmp/a9x_webstatistics-0.2.2.tar.gz` & `tmp/a9x_webstatistics-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics-0.2.2.tar", last modified: Sun Jun  2 15:50:18 2024, max compression
+gzip compressed data, was "a9x_webstatistics-0.2.3.tar", last modified: Sun Jun  2 16:01:24 2024, max compression
```

## Comparing `a9x_webstatistics-0.2.2.tar` & `a9x_webstatistics-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:50:18.027759 a9x_webstatistics-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-06-02 15:50:18.027759 a9x_webstatistics-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/dist_del
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-02 15:50:18.027759 a9x_webstatistics-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:50:18.023759 a9x_webstatistics-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:50:18.023759 a9x_webstatistics-0.2.2/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics/gencockpit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics/module1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics/summarizemonth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics/updatestatistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:50:18.027759 a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-06-02 15:50:18.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-06-02 15:50:18.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:50:18.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-02 15:50:18.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 15:50:18.000000 a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:50:18.027759 a9x_webstatistics-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/tests/test_main001.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/tests/test_main010.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/tests/test_module1.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-02 15:50:08.000000 a9x_webstatistics-0.2.2/tests/test_z090_gencockpit010.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:01:24.704489 a9x_webstatistics-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-06-02 16:01:24.704489 a9x_webstatistics-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-02 16:01:24.704489 a9x_webstatistics-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:01:24.700489 a9x_webstatistics-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:01:24.704489 a9x_webstatistics-0.2.3/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics/gencockpit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics/summarizemonth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics/updatestatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:01:24.704489 a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-06-02 16:01:24.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-06-02 16:01:24.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:01:24.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-02 16:01:24.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 16:01:24.000000 a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:01:24.704489 a9x_webstatistics-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/tests/test_module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-02 16:01:14.000000 a9x_webstatistics-0.2.3/tests/test_z090_gencockpit010.py
```

### Comparing `a9x_webstatistics-0.2.2/LICENSE` & `a9x_webstatistics-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/PKG-INFO` & `a9x_webstatistics-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.2.2
+Version: 0.2.3
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.2.2/README.md` & `a9x_webstatistics-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/setup.py` & `a9x_webstatistics-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/src/a9x_webstatistics/gencockpit.py` & `a9x_webstatistics-0.2.3/src/a9x_webstatistics/gencockpit.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         d = json.load(json_file) 
 
         lbl = []
         dta = []
 
         for e in d['days']:
             lbl.append(e)
-            if d['days'][e]['device_hits']['desktop']:
+            if 'desktop' in d['days'][e]['device_hits']:
                 dta.append(d['days'][e]['device_hits']['desktop'])
             else:
                 dta.append(0)
               
         h = genHeader()
         h += 'new Chart(ctx, {'  + "\n"
         h += ' type: \'bar\','   + "\n"
```

### Comparing `a9x_webstatistics-0.2.2/src/a9x_webstatistics/main.py` & `a9x_webstatistics-0.2.3/src/a9x_webstatistics/main.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/src/a9x_webstatistics/summarizemonth.py` & `a9x_webstatistics-0.2.3/src/a9x_webstatistics/summarizemonth.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/src/a9x_webstatistics/updatestatistics.py` & `a9x_webstatistics-0.2.3/src/a9x_webstatistics/updatestatistics.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/PKG-INFO` & `a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.2.2
+Version: 0.2.3
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.2.2/src/a9x_webstatistics.egg-info/SOURCES.txt` & `a9x_webstatistics-0.2.3/src/a9x_webstatistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/tests/test_main001.py` & `a9x_webstatistics-0.2.3/tests/test_main001.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/tests/test_main010.py` & `a9x_webstatistics-0.2.3/tests/test_main010.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.2.2/tests/test_z090_gencockpit010.py` & `a9x_webstatistics-0.2.3/tests/test_z090_gencockpit010.py`

 * *Files identical despite different names*

