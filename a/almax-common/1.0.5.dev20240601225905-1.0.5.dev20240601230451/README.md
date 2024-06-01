# Comparing `tmp/almax_common-1.0.5.dev20240601225905.tar.gz` & `tmp/almax_common-1.0.5.dev20240601230451.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.5.dev20240601225905.tar", last modified: Sat Jun  1 22:59:08 2024, max compression
+gzip compressed data, was "almax_common-1.0.5.dev20240601230451.tar", last modified: Sat Jun  1 23:04:53 2024, max compression
```

## Comparing `almax_common-1.0.5.dev20240601225905.tar` & `almax_common-1.0.5.dev20240601230451.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.427718 almax_common-1.0.5.dev20240601225905/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:59:08.427718 almax_common-1.0.5.dev20240601225905/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:59:08.427718 almax_common-1.0.5.dev20240601225905/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsTime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.739144 almax_common-1.0.5.dev20240601230451/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.739144 almax_common-1.0.5.dev20240601230451/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxUtils/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 23:04:53.000000 almax_common-1.0.5.dev20240601230451/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-01 23:04:53.000000 almax_common-1.0.5.dev20240601230451/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 23:04:53.000000 almax_common-1.0.5.dev20240601230451/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 23:04:53.000000 almax_common-1.0.5.dev20240601230451/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 23:04:53.000000 almax_common-1.0.5.dev20240601230451/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:04:53.743144 almax_common-1.0.5.dev20240601230451/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/tests/test_AlmaxUtilsGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 23:04:42.000000 almax_common-1.0.5.dev20240601230451/tests/test_AlmaxUtilsTime.py
```

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxClasses/__init__.py` & `almax_common-1.0.5.dev20240601230451/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.5.dev20240601230451/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxLogs/LoggerService.py` & `almax_common-1.0.5.dev20240601230451/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.5.dev20240601230451/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.5.dev20240601230451/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxUtils/FileSystem.py` & `almax_common-1.0.5.dev20240601230451/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxUtils/Generic.py` & `almax_common-1.0.5.dev20240601230451/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxUtils/PdfManager.py` & `almax_common-1.0.5.dev20240601230451/AlmaxUtils/PdfManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,16 @@
                 "Prezzo",
                 "Totale (no IVA)"
             ]
         ];
         for order in orders:
             attributes = [];
             for attribute in dir(order):
-                attributes.append(attribute);
+                if not attribute.startswith("__") and not callable(getattr(order, attribute)):
+                    attributes.append(getattr(order, attribute));
             body_table_data.append(
                 ToParagraph_ForTable(
                     attributes
                 )
             );
 
         body_table_style = TableStyle([
```

### Comparing `almax_common-1.0.5.dev20240601225905/AlmaxUtils/Time.py` & `almax_common-1.0.5.dev20240601230451/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/PKG-INFO` & `almax_common-1.0.5.dev20240601230451/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601225905
+Version: 1.0.5.dev20240601230451
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601225905/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.5.dev20240601230451/almax_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601225905
+Version: 1.0.5.dev20240601230451
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601225905/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.5.dev20240601230451/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/setup.py` & `almax_common-1.0.5.dev20240601230451/setup.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsGeneric.py` & `almax_common-1.0.5.dev20240601230451/tests/test_AlmaxUtilsGeneric.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsTime.py` & `almax_common-1.0.5.dev20240601230451/tests/test_AlmaxUtilsTime.py`

 * *Files identical despite different names*

