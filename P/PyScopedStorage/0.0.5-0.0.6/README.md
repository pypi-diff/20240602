# Comparing `tmp/pyscopedstorage-0.0.5.tar.gz` & `tmp/pyscopedstorage-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscopedstorage-0.0.5.tar", max compression
+gzip compressed data, was "pyscopedstorage-0.0.6.tar", max compression
```

## Comparing `pyscopedstorage-0.0.5.tar` & `pyscopedstorage-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.5/LICENSE
--rw-r--r--   0        0        0     3200 2024-06-03 17:46:56.927260 pyscopedstorage-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       98 2024-06-03 16:44:53.027181 pyscopedstorage-0.0.5/src/PyScopedStorage/__init__.py
--rw-r--r--   0        0        0      567 2024-06-03 17:34:45.702245 pyscopedstorage-0.0.5/src/PyScopedStorage/android_objects.py
--rw-r--r--   0        0        0     2880 2024-06-03 16:44:30.973180 pyscopedstorage-0.0.5/src/PyScopedStorage/filechooser.py
--rw-r--r--   0        0        0      314 2024-06-03 18:01:06.731279 pyscopedstorage-0.0.5/src/PyScopedStorage/io.py
--rw-r--r--   0        0        0     3193 2024-06-03 18:01:45.979280 pyscopedstorage-0.0.5/src/PyScopedStorage/tools.py
--rw-r--r--   0        0        0     4203 2024-06-03 17:45:46.489259 pyscopedstorage-0.0.5/src/PyScopedStorage/utils.py
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3200 2024-06-03 18:03:57.992282 pyscopedstorage-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-06-03 16:44:53.027181 pyscopedstorage-0.0.6/src/PyScopedStorage/__init__.py
+-rw-r--r--   0        0        0      567 2024-06-03 17:34:45.702245 pyscopedstorage-0.0.6/src/PyScopedStorage/android_objects.py
+-rw-r--r--   0        0        0     2880 2024-06-03 16:44:30.973180 pyscopedstorage-0.0.6/src/PyScopedStorage/filechooser.py
+-rw-r--r--   0        0        0      324 2024-06-03 18:25:28.795310 pyscopedstorage-0.0.6/src/PyScopedStorage/io.py
+-rw-r--r--   0        0        0     3233 2024-06-03 18:27:41.953313 pyscopedstorage-0.0.6/src/PyScopedStorage/tools.py
+-rw-r--r--   0        0        0     4203 2024-06-03 17:45:46.489259 pyscopedstorage-0.0.6/src/PyScopedStorage/utils.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.6/PKG-INFO
```

### Comparing `pyscopedstorage-0.0.5/LICENSE` & `pyscopedstorage-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.5/pyproject.toml` & `pyscopedstorage-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyScopedStorage"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python library to simplify storage interaction in Android apps."
 # readme = "README.md"  # TODO..
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `pyscopedstorage-0.0.5/src/PyScopedStorage/android_objects.py` & `pyscopedstorage-0.0.6/src/PyScopedStorage/android_objects.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.5/src/PyScopedStorage/filechooser.py` & `pyscopedstorage-0.0.6/src/PyScopedStorage/filechooser.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.5/src/PyScopedStorage/tools.py` & `pyscopedstorage-0.0.6/src/PyScopedStorage/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,8 +117,9 @@
 	return uri
 
 
 sfopen_sync = scoped_file_open_sync
 sfopen_async = scoped_file_open_async
 
 smkdir_sync = scoped_mkdir_sync
-smkdir_async = wrap2async(scoped_mkdir_sync)
+scoped_mkdir_async = wrap2async(scoped_mkdir_sync)
+smkdir_async = scoped_mkdir_async
```

### Comparing `pyscopedstorage-0.0.5/src/PyScopedStorage/utils.py` & `pyscopedstorage-0.0.6/src/PyScopedStorage/utils.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.5/PKG-INFO` & `pyscopedstorage-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScopedStorage
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library to simplify storage interaction in Android apps.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

