# Comparing `tmp/almax_common-1.0.4.dev20240601201036.tar.gz` & `tmp/almax_common-1.0.5.dev20240601214939.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.4.dev20240601201036.tar", last modified: Sat Jun  1 20:10:41 2024, max compression
+gzip compressed data, was "almax_common-1.0.5.dev20240601214939.tar", last modified: Sat Jun  1 21:49:42 2024, max compression
```

## Comparing `almax_common-1.0.4.dev20240601201036.tar` & `almax_common-1.0.5.dev20240601214939.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.565773 almax_common-1.0.5.dev20240601214939/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.565773 almax_common-1.0.5.dev20240601214939/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.565773 almax_common-1.0.5.dev20240601214939/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/tests/test_AlmaxUtils.py
```

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxClasses/__init__.py` & `almax_common-1.0.5.dev20240601214939/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.5.dev20240601214939/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxLogs/LoggerService.py` & `almax_common-1.0.5.dev20240601214939/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxUtils/FileSystem.py` & `almax_common-1.0.5.dev20240601214939/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxUtils/Generic.py` & `almax_common-1.0.5.dev20240601214939/AlmaxUtils/Generic.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def ReadFile(file_path: str) -> list:
     with open(file_path, 'r') as file:
         lines = file.readlines();
     return lines;
 
 def isCodiceFiscale(parola):
-    """Data in input una stringa, viene analizzata la composizione della stringa per determinare se è un codice fiscale o meno.
+    """ - DA RIVEDERE - Data in input una stringa, viene analizzata la composizione della stringa per determinare se è un codice fiscale o meno.
     Ritorna True in caso sia un codice fiscale, False altrimenti. """
     trovato = False,parola
     if len(parola) > 16:
 
         trovato = isCodiceFiscale(parola[0:16])
         if trovato[0]:
             return True,parola[0:16]
```

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxUtils/PdfManager.py` & `almax_common-1.0.5.dev20240601214939/AlmaxUtils/PdfManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import AlmaxUtils.Generic as Generic;
+import AlmaxUtils.Time as TimeLib;
 import os;
 import PyPDF2;
 
 from reportlab.lib.pagesizes import A4;
 from reportlab.lib import colors;
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle;
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer, Table, TableStyle;
 
 def GeneratePdf(client_info, orders):
     try:
-        now = Generic.now();
+        now = TimeLib.now();
         now_month = now.month if now.month > 9 else f"0{now.month}";
         now_day = now.day if now.day > 9 else f"0{now.day}";
         now_hour = now.hour if now.hour > 9 else f"0{now.hour}";
         now_minute = now.minute if now.minute > 9 else f"0{now.minute}";
         now_second = now.second if now.second > 9 else f"0{now.second}";
 
         file_path = f"{now.year}/{now_month}";
```

### Comparing `almax_common-1.0.4.dev20240601201036/AlmaxUtils/Time.py` & `almax_common-1.0.5.dev20240601214939/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4.dev20240601201036/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.5.dev20240601214939/almax_common.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 ./AlmaxUtils/PdfManager.py
 ./AlmaxUtils/Time.py
 ./AlmaxUtils/Xml.py
 ./AlmaxUtils/__init__.py
 almax_common.egg-info/PKG-INFO
 almax_common.egg-info/SOURCES.txt
 almax_common.egg-info/dependency_links.txt
-almax_common.egg-info/top_level.txt
+almax_common.egg-info/requires.txt
+almax_common.egg-info/top_level.txt
+tests/test_AlmaxUtils.py
```

