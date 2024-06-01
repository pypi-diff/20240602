# Comparing `tmp/almax_common-1.0.5.dev20240601224724.tar.gz` & `tmp/almax_common-1.0.5.dev20240601225905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.5.dev20240601224724.tar", last modified: Sat Jun  1 22:47:26 2024, max compression
+gzip compressed data, was "almax_common-1.0.5.dev20240601225905.tar", last modified: Sat Jun  1 22:59:08 2024, max compression
```

## Comparing `almax_common-1.0.5.dev20240601224724.tar` & `almax_common-1.0.5.dev20240601225905.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.989281 almax_common-1.0.5.dev20240601224724/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 22:47:26.000000 almax_common-1.0.5.dev20240601224724/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.993281 almax_common-1.0.5.dev20240601224724/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 22:47:15.000000 almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsTime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.427718 almax_common-1.0.5.dev20240601225905/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:59:08.427718 almax_common-1.0.5.dev20240601225905/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 22:59:08.000000 almax_common-1.0.5.dev20240601225905/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:59:08.427718 almax_common-1.0.5.dev20240601225905/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:59:08.423718 almax_common-1.0.5.dev20240601225905/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 22:58:57.000000 almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsTime.py
```

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxClasses/__init__.py` & `almax_common-1.0.5.dev20240601225905/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.5.dev20240601225905/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxLogs/LoggerService.py` & `almax_common-1.0.5.dev20240601225905/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.5.dev20240601225905/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxUtils/FileSystem.py` & `almax_common-1.0.5.dev20240601225905/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxUtils/Generic.py` & `almax_common-1.0.5.dev20240601225905/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxUtils/PdfManager.py` & `almax_common-1.0.5.dev20240601225905/AlmaxUtils/PdfManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pypdf;
 
 from reportlab.lib.pagesizes import A4;
 from reportlab.lib import colors;
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle;
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer, Table, TableStyle;
 
-def GeneratePdf(client_info, orders):
+def GeneratePdf(client_info, cls, orders):
     try:
         now = TimeLib.now;
         now_month = now.month if now.month > 9 else f"0{now.month}";
         now_day = now.day if now.day > 9 else f"0{now.day}";
         now_hour = now.hour if now.hour > 9 else f"0{now.hour}";
         now_minute = now.minute if now.minute > 9 else f"0{now.minute}";
         now_second = now.second if now.second > 9 else f"0{now.second}";
@@ -98,15 +98,22 @@
                 "Descrizione", 
                 "Quantità",
                 "Prezzo",
                 "Totale (no IVA)"
             ]
         ];
         for order in orders:
-            body_table_data.append(ToParagraph_ForTable(order['Description'], order['Quantity'], order['Price'], order['Total']));
+            attributes = [];
+            for attribute in dir(order):
+                attributes.append(attribute);
+            body_table_data.append(
+                ToParagraph_ForTable(
+                    attributes
+                )
+            );
 
         body_table_style = TableStyle([
             ('BACKGROUND', (0, 0), (-1, 0), colors.whitesmoke),
             ('ALIGN', (0, 0), (-1, -1), 'CENTER'),
             ('VALIGN', (0, 0), (-1, -1), 'MIDDLE'),
             ('GRID', (0, 0), (-1, -1), 1, colors.black),
 
@@ -127,38 +134,22 @@
         doc.build(content);
 
         print(f'PDF generated successfully at: {file_path}');
     except Exception as e:
         print(f'Error generating PDF: {e}');
 
 
-def ToParagraph_ForTable(Description, Quantity, Price, Total):
+def ToParagraph_ForTable(elements: list):
     style = ParagraphStyle(
         name="Centered",
         parent=getSampleStyleSheet()['Normal'],
         fontName='Times-Roman',
         alignment=1 # 0=left, 1=center, 2=right
     );
-    return [
-        Paragraph(
-            f"{Description}"
-        ),
-        Paragraph(
-            f"{Quantity}", 
-            style
-        ),
-        Paragraph(
-            f"{Price}€", 
-            style
-        ),
-        Paragraph(
-            f"{Total}€", 
-            style
-        )
-    ];
+    return [ Paragraph(f"{element}") for element in elements];
 
 
 def DivideAndMergePages(pdf_vecchio, indici_pagine, directorySalvataggio, nomeFile):
     """ - DA RISCRIVERE - La funzione usa la libreria PyPDF2 e si occupa di strarre le singole pagine da un dato PDF.
     pdf_vecchio è il reader, generalmente dichiarato come pdfReader = PyPDF2.PdfFileReader(pdfFileObj)
     indici_pagine è la posizione delle pagine specifiche da estrarre; può essere un singolo indice o più di uno; in case fossero tanti, è strettamente necessario sia un array
     directorySalvataggio è il nome della cartella in cui salvare il/i file_estratto
```

### Comparing `almax_common-1.0.5.dev20240601224724/AlmaxUtils/Time.py` & `almax_common-1.0.5.dev20240601225905/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/PKG-INFO` & `almax_common-1.0.5.dev20240601225905/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601224724
+Version: 1.0.5.dev20240601225905
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601224724/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.5.dev20240601225905/almax_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601224724
+Version: 1.0.5.dev20240601225905
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601224724/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.5.dev20240601225905/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/setup.py` & `almax_common-1.0.5.dev20240601225905/setup.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsGeneric.py` & `almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsGeneric.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601224724/tests/test_AlmaxUtilsTime.py` & `almax_common-1.0.5.dev20240601225905/tests/test_AlmaxUtilsTime.py`

 * *Files identical despite different names*

