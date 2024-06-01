# Comparing `tmp/almax_common-1.0.5.dev20240601224039.tar.gz` & `tmp/almax_common-1.0.5.dev20240601224724.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.5.dev20240601224039.tar", last modified: Sat Jun  1 22:40:42 2024, max compression
+gzip compressed data, was "almax_common-1.0.5.dev20240601224724.tar", last modified: Sat Jun  1 22:47:26 2024, max compression
```

## Comparing `almax_common-1.0.5.dev20240601224039.tar` & `almax_common-1.0.5.dev20240601224724.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/tests/test_AlmaxUtilsGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/tests/test_AlmaxUtilsTime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsTime.py
```

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxClasses/__init__.py` & `almax_common-1.0.5.dev20240601224724/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.5.dev20240601224724/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxLogs/LoggerService.py` & `almax_common-1.0.5.dev20240601224724/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxUtils/FileSystem.py` & `almax_common-1.0.5.dev20240601224724/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxUtils/Generic.py` & `almax_common-1.0.5.dev20240601224724/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxUtils/PdfManager.py` & `almax_common-1.0.5.dev20240601224724/AlmaxUtils/PdfManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/AlmaxUtils/Time.py` & `almax_common-1.0.5.dev20240601224724/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/PKG-INFO` & `almax_common-1.0.5.dev20240601224724/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601224039
+Version: 1.0.5.dev20240601224724
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601224039/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.5.dev20240601224724/almax_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601224039
+Version: 1.0.5.dev20240601224724
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601224039/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.5.dev20240601224724/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/setup.py` & `almax_common-1.0.5.dev20240601224724/setup.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/tests/test_AlmaxUtilsGeneric.py` & `almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsGeneric.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224039/tests/test_AlmaxUtilsTime.py` & `almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsTime.py`

 * *Files identical despite different names*

