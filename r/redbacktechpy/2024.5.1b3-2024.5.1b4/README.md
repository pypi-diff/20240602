# Comparing `tmp/redbacktechpy-2024.5.1b3.tar.gz` & `tmp/redbacktechpy-2024.5.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.1b3.tar", last modified: Sat Jun  1 19:52:56 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.1b4.tar", last modified: Sat Jun  1 20:33:04 2024, max compression
```

## Comparing `redbacktechpy-2024.5.1b3.tar` & `redbacktechpy-2024.5.1b4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.335621 redbacktechpy-2024.5.1b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    50856 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.647641 redbacktechpy-2024.5.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 20:33:04.647641 redbacktechpy-2024.5.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:33:04.647641 redbacktechpy-2024.5.1b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.643641 redbacktechpy-2024.5.1b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.643641 redbacktechpy-2024.5.1b4/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50891 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.643641 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.1b3/LICENSE` & `redbacktechpy-2024.5.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b3/PKG-INFO` & `redbacktechpy-2024.5.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b3
+Version: 2024.5.1b4
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.1b3/pyproject.toml` & `redbacktechpy-2024.5.1b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.1b3"
+version = "2024.05.1b4"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.1b3/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.1b4/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b3/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.1b4/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b3/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.1b4/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b3/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.1b4/src/redbacktechpy/redbacktech_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,15 +503,16 @@
         
         #device_type: str = entity['type'].lower()
         data = {
             'id': entity['device_id'] + entity['entity_name']
         }
                
         entity_instance = RedbackEntitys(
-            entity_id=entity['entity_name'],
+            #entity_id=entity['entity_name'],
+            entity_id=data['id'],
             device_id=entity['device_id'],
             type=entity['device_type'],
             data=entity,
             #device_data=entity,
         )
         return entity_instance, data['id']
```

### Comparing `redbacktechpy-2024.5.1b3/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.1b4/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b3
+Version: 2024.5.1b4
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

