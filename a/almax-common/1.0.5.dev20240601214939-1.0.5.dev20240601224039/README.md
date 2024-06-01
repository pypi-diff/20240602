# Comparing `tmp/almax_common-1.0.5.dev20240601214939.tar.gz` & `tmp/almax_common-1.0.5.dev20240601224039.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.5.dev20240601214939.tar", last modified: Sat Jun  1 21:49:42 2024, max compression
+gzip compressed data, was "almax_common-1.0.5.dev20240601224039.tar", last modified: Sat Jun  1 22:40:42 2024, max compression
```

## Comparing `almax_common-1.0.5.dev20240601214939.tar` & `almax_common-1.0.5.dev20240601224039.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.565773 almax_common-1.0.5.dev20240601214939/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.565773 almax_common-1.0.5.dev20240601214939/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.565773 almax_common-1.0.5.dev20240601214939/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 21:49:42.000000 almax_common-1.0.5.dev20240601214939/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:49:42.569773 almax_common-1.0.5.dev20240601214939/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 21:49:31.000000 almax_common-1.0.5.dev20240601214939/tests/test_AlmaxUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.456641 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 22:40:42.000000 almax_common-1.0.5.dev20240601224039/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:40:42.460641 almax_common-1.0.5.dev20240601224039/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/tests/test_AlmaxUtilsGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 22:40:31.000000 almax_common-1.0.5.dev20240601224039/tests/test_AlmaxUtilsTime.py
```

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxClasses/__init__.py` & `almax_common-1.0.5.dev20240601224039/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.5.dev20240601224039/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxLogs/LoggerService.py` & `almax_common-1.0.5.dev20240601224039/AlmaxLogs/LoggerService.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,25 +30,25 @@
         self.__Istance.info(message);
 
     def StartTiming(self, message):
         self.__Istance.info(message);
         self.__CustomTimer = datetime.now();
 
     def EndTiming(self):
-        self.__Istance.info(f"\tDuration: {Generic.TimeToString(Generic.CalculateTime(self.__CustomTimer))}");
+        self.__Istance.info(f"\tDuration: {Generic.TimeToString(Generic.CalculateTimePassed(self.__CustomTimer))}");
    
     def StartGenericTiming(self):
         self.__Timer = datetime.now();
 
     def ForceEnd(self):
-        self.__Istance.info(f"Total Duration: {Generic.TimeToString(Generic.CalculateTime(self.__Timer))}");
+        self.__Istance.info(f"Total Duration: {Generic.TimeToString(Generic.CalculateTimePassed(self.__Timer))}");
         self.__Istance.info(f"FORCED END\n\n");
 
     def Start(self):
         self.__Istance.info(f"START");
 
     def End(self):
-        self.__Istance.info(f"Total Duration: {Generic.TimeToString(Generic.CalculateTime(self.__Timer))}");
+        self.__Istance.info(f"Total Duration: {Generic.TimeToString(Generic.CalculateTimePassed(self.__Timer))}");
         self.__Istance.info(f"END\n\n");
 
     def LogPath(self) -> str:
         return self.__LogPath;
```

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.5.dev20240601224039/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxUtils/FileSystem.py` & `almax_common-1.0.5.dev20240601224039/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxUtils/Generic.py` & `almax_common-1.0.5.dev20240601224039/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxUtils/PdfManager.py` & `almax_common-1.0.5.dev20240601224039/AlmaxUtils/PdfManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import AlmaxUtils.Time as TimeLib;
 import os;
-import PyPDF2;
+import pypdf;
 
 from reportlab.lib.pagesizes import A4;
 from reportlab.lib import colors;
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle;
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer, Table, TableStyle;
 
 def GeneratePdf(client_info, orders):
     try:
-        now = TimeLib.now();
+        now = TimeLib.now;
         now_month = now.month if now.month > 9 else f"0{now.month}";
         now_day = now.day if now.day > 9 else f"0{now.day}";
         now_hour = now.hour if now.hour > 9 else f"0{now.hour}";
         now_minute = now.minute if now.minute > 9 else f"0{now.minute}";
         now_second = now.second if now.second > 9 else f"0{now.second}";
 
         file_path = f"{now.year}/{now_month}";
         if not os.path.exists(file_path):
             os.makedirs(file_path);
         file_path = f"{file_path}/{now_day}_{now_hour}{now_minute}{now_second}.pdf";
-        file_path = "test.pdf";
+        #file_path = "test.pdf";
 
         size_societyName = 25;
         margin = 10;
         doc = SimpleDocTemplate(
             file_path, 
             pagesize=A4, 
             leftMargin=margin, 
@@ -98,15 +98,15 @@
                 "Descrizione", 
                 "Quantità",
                 "Prezzo",
                 "Totale (no IVA)"
             ]
         ];
         for order in orders:
-            body_table_data.append(ToParagraph_ForTable(order.Description, order.Quantity, order.Price, order.Total));
+            body_table_data.append(ToParagraph_ForTable(order['Description'], order['Quantity'], order['Price'], order['Total']));
 
         body_table_style = TableStyle([
             ('BACKGROUND', (0, 0), (-1, 0), colors.whitesmoke),
             ('ALIGN', (0, 0), (-1, -1), 'CENTER'),
             ('VALIGN', (0, 0), (-1, -1), 'MIDDLE'),
             ('GRID', (0, 0), (-1, -1), 1, colors.black),
 
@@ -160,15 +160,15 @@
 def DivideAndMergePages(pdf_vecchio, indici_pagine, directorySalvataggio, nomeFile):
     """ - DA RISCRIVERE - La funzione usa la libreria PyPDF2 e si occupa di strarre le singole pagine da un dato PDF.
     pdf_vecchio è il reader, generalmente dichiarato come pdfReader = PyPDF2.PdfFileReader(pdfFileObj)
     indici_pagine è la posizione delle pagine specifiche da estrarre; può essere un singolo indice o più di uno; in case fossero tanti, è strettamente necessario sia un array
     directorySalvataggio è il nome della cartella in cui salvare il/i file_estratto
     nomeFile è il nome che verrà assegnato al PDF contenente le pagine divise."""
 
-    file_da_scrivere = PyPDF2.PdfFileWriter()
+    file_da_scrivere = pypdf.PdfFileWriter()
 
     if isinstance(indici_pagine,list):
         for i in indici_pagine:
             file_da_scrivere.addPage(pdf_vecchio.getPage(i))
     else:
         file_da_scrivere.addPage(pdf_vecchio.getPage(indici_pagine))
 
@@ -177,23 +177,23 @@
         file_da_scrivere.write(file_estratto)
 
 
 def MergePDFs(nome_pdf1, nome_pdf2, directorySalvataggio):
     #Lettura PDF
     #nomePDF = simpledialog.askstring(title=nomeProgramma, prompt="Inserire il nome del file PDF senza l'estensione.\nEsempio: se il file si chiama 'test.pdf', basterà inserire 'test'")
     pdfFileObj_1 = open(directorySalvataggio + "/" + nome_pdf1+".pdf", 'rb')
-    pdfReader_1 = PyPDF2.PdfFileReader(pdfFileObj_1)
+    pdfReader_1 = pypdf.PdfFileReader(pdfFileObj_1)
     #print("unisci Ok1" + directorySalvataggio + "/" + nome_pdf2+".pdf")
     pdfFileObj_2 = open(directorySalvataggio + "/" + nome_pdf2+".pdf", 'rb')
-    pdfReader_2 = PyPDF2.PdfFileReader(pdfFileObj_2)
+    pdfReader_2 = pypdf.PdfFileReader(pdfFileObj_2)
     #print("unisci Ok2")
     numPagine1 = pdfReader_1.numPages
     numPagine2 = pdfReader_2.numPages
 
-    pdf_unito = PyPDF2.PdfFileWriter()
+    pdf_unito = pypdf.PdfFileWriter()
     for i in range(numPagine1):
         pdf_unito.addPage(pdfReader_1.getPage(i))
     for i in range(numPagine2):
         pdf_unito.addPage(pdfReader_2.getPage(i))
 
     with open(directorySalvataggio + "/pdfUnito.pdf", "wb") as file_da_scrivere:
         pdf_unito.write(file_da_scrivere)
```

### Comparing `almax_common-1.0.5.dev20240601214939/AlmaxUtils/Time.py` & `almax_common-1.0.5.dev20240601224039/AlmaxUtils/Time.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timedelta;
 
 now = datetime.now();
 
-def CalculateTime(start: datetime):
+def CalculateTimePassed(start: datetime = 0):
     return datetime.now() - start;
 
 def TimeToString(time: datetime) -> str:
     seconds = time.total_seconds();
     minutes = seconds // 60;
     hours = minutes // 60;
     days = hours // 24;
```

### Comparing `almax_common-1.0.5.dev20240601214939/PKG-INFO` & `almax_common-1.0.5.dev20240601224039/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601214939
+Version: 1.0.5.dev20240601224039
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==24.0
 Requires-Dist: pillow==10.3.0
 Requires-Dist: pluggy==1.5.0
-Requires-Dist: PyPDF2==3.0.1
+Requires-Dist: pypdf==4.2.0
 Requires-Dist: pytest==8.2.1
 Requires-Dist: reportlab==4.2.0
 Requires-Dist: setuptools==70.0.0
 
 # AlmaxClasses
 Generic Purpose Classes
```

### Comparing `almax_common-1.0.5.dev20240601214939/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.5.dev20240601224039/almax_common.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601214939
+Version: 1.0.5.dev20240601224039
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==24.0
 Requires-Dist: pillow==10.3.0
 Requires-Dist: pluggy==1.5.0
-Requires-Dist: PyPDF2==3.0.1
+Requires-Dist: pypdf==4.2.0
 Requires-Dist: pytest==8.2.1
 Requires-Dist: reportlab==4.2.0
 Requires-Dist: setuptools==70.0.0
 
 # AlmaxClasses
 Generic Purpose Classes
```

### Comparing `almax_common-1.0.5.dev20240601214939/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.5.dev20240601224039/almax_common.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 ./AlmaxUtils/Xml.py
 ./AlmaxUtils/__init__.py
 almax_common.egg-info/PKG-INFO
 almax_common.egg-info/SOURCES.txt
 almax_common.egg-info/dependency_links.txt
 almax_common.egg-info/requires.txt
 almax_common.egg-info/top_level.txt
-tests/test_AlmaxUtils.py
+tests/test_AlmaxUtilsGeneric.py
+tests/test_AlmaxUtilsTime.py
```

### Comparing `almax_common-1.0.5.dev20240601214939/setup.py` & `almax_common-1.0.5.dev20240601224039/setup.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601214939/tests/test_AlmaxUtils.py` & `almax_common-1.0.5.dev20240601224039/tests/test_AlmaxUtilsGeneric.py`

 * *Files identical despite different names*

