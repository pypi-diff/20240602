# Comparing `tmp/dbTelematelAPI-0.0.6.tar.gz` & `tmp/dbTelematelAPI-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbTelematelAPI-0.0.6.tar", last modified: Sun Jun  2 15:19:19 2024, max compression
+gzip compressed data, was "dbTelematelAPI-0.0.7.tar", last modified: Sun Jun  2 18:48:33 2024, max compression
```

## Comparing `dbTelematelAPI-0.0.6.tar` & `dbTelematelAPI-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 15:19:19.584366 dbTelematelAPI-0.0.6/
--rw-rw-rw-   0        0        0      751 2024-06-02 15:19:19.570260 dbTelematelAPI-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      140 2024-06-02 14:45:27.000000 dbTelematelAPI-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 15:19:19.475194 dbTelematelAPI-0.0.6/dbTelematelAPI/
--rw-rw-rw-   0        0        0      139 2024-06-02 15:07:03.000000 dbTelematelAPI-0.0.6/dbTelematelAPI/__init__.py
--rw-rw-rw-   0        0        0      189 2024-06-02 15:00:23.000000 dbTelematelAPI-0.0.6/dbTelematelAPI/__main__.py
--rw-rw-rw-   0        0        0     1176 2024-06-02 15:01:12.000000 dbTelematelAPI-0.0.6/dbTelematelAPI/query_pasarela.py
--rw-rw-rw-   0        0        0     2873 2024-06-02 15:04:14.000000 dbTelematelAPI-0.0.6/dbTelematelAPI/telematel_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-06-02 15:19:19.570260 dbTelematelAPI-0.0.6/dbTelematelAPI.egg-info/
--rw-rw-rw-   0        0        0      751 2024-06-02 15:19:19.000000 dbTelematelAPI-0.0.6/dbTelematelAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-06-02 15:19:19.000000 dbTelematelAPI-0.0.6/dbTelematelAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 15:19:19.000000 dbTelematelAPI-0.0.6/dbTelematelAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-06-02 15:19:19.000000 dbTelematelAPI-0.0.6/dbTelematelAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-06-02 15:19:19.000000 dbTelematelAPI-0.0.6/dbTelematelAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2024-06-02 13:14:24.000000 dbTelematelAPI-0.0.6/license.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 15:19:19.586957 dbTelematelAPI-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-06-02 15:18:42.000000 dbTelematelAPI-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:48:32.985540 dbTelematelAPI-0.0.7/
+-rw-rw-rw-   0        0        0      751 2024-06-02 18:48:32.985540 dbTelematelAPI-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2024-06-02 18:40:23.000000 dbTelematelAPI-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 18:48:32.864771 dbTelematelAPI-0.0.7/dbTelematelAPI/
+-rw-rw-rw-   0        0        0      139 2024-06-02 15:07:03.000000 dbTelematelAPI-0.0.7/dbTelematelAPI/__init__.py
+-rw-rw-rw-   0        0        0      189 2024-06-02 15:00:23.000000 dbTelematelAPI-0.0.7/dbTelematelAPI/__main__.py
+-rw-rw-rw-   0        0        0     1176 2024-06-02 15:01:12.000000 dbTelematelAPI-0.0.7/dbTelematelAPI/query_pasarela.py
+-rw-rw-rw-   0        0        0     2873 2024-06-02 15:04:14.000000 dbTelematelAPI-0.0.7/dbTelematelAPI/telematel_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:48:32.964839 dbTelematelAPI-0.0.7/dbTelematelAPI.egg-info/
+-rw-rw-rw-   0        0        0      751 2024-06-02 18:48:32.000000 dbTelematelAPI-0.0.7/dbTelematelAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-06-02 18:48:32.000000 dbTelematelAPI-0.0.7/dbTelematelAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 18:48:32.000000 dbTelematelAPI-0.0.7/dbTelematelAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 18:48:32.000000 dbTelematelAPI-0.0.7/dbTelematelAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-02 18:48:32.000000 dbTelematelAPI-0.0.7/dbTelematelAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2024-06-02 13:14:24.000000 dbTelematelAPI-0.0.7/license.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 18:48:32.985540 dbTelematelAPI-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-06-02 18:47:50.000000 dbTelematelAPI-0.0.7/setup.py
```

### Comparing `dbTelematelAPI-0.0.6/PKG-INFO` & `dbTelematelAPI-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbTelematelAPI
-Version: 0.0.6
+Version: 0.0.7
 Summary: Permite consumir el API de Telematel
 Home-page: https://github.com/jmsanchez-ibiza/dbTelematelAPI
 Author: José María Sánchez González
 Author-email: miotroyo1970@gmail.com
 License: MIT
 Keywords: jmsanchez-ibiza
 Classifier: Development Status :: 3 - Alpha
@@ -12,11 +12,11 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 <!-- README.md -->
-##dbTelematelAPI
+## dbTelematelAPI
 
-Sirver para conectarse a un API que nos permite hacer consultas
+Sirve para conectarse a un API que nos permite hacer consultas
 sobre la base de datos de Telematel
```

### Comparing `dbTelematelAPI-0.0.6/dbTelematelAPI/query_pasarela.py` & `dbTelematelAPI-0.0.7/dbTelematelAPI/query_pasarela.py`

 * *Files identical despite different names*

### Comparing `dbTelematelAPI-0.0.6/dbTelematelAPI/telematel_wrapper.py` & `dbTelematelAPI-0.0.7/dbTelematelAPI/telematel_wrapper.py`

 * *Files identical despite different names*

### Comparing `dbTelematelAPI-0.0.6/dbTelematelAPI.egg-info/PKG-INFO` & `dbTelematelAPI-0.0.7/dbTelematelAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbTelematelAPI
-Version: 0.0.6
+Version: 0.0.7
 Summary: Permite consumir el API de Telematel
 Home-page: https://github.com/jmsanchez-ibiza/dbTelematelAPI
 Author: José María Sánchez González
 Author-email: miotroyo1970@gmail.com
 License: MIT
 Keywords: jmsanchez-ibiza
 Classifier: Development Status :: 3 - Alpha
@@ -12,11 +12,11 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 <!-- README.md -->
-##dbTelematelAPI
+## dbTelematelAPI
 
-Sirver para conectarse a un API que nos permite hacer consultas
+Sirve para conectarse a un API que nos permite hacer consultas
 sobre la base de datos de Telematel
```

### Comparing `dbTelematelAPI-0.0.6/license.txt` & `dbTelematelAPI-0.0.7/license.txt`

 * *Files identical despite different names*

### Comparing `dbTelematelAPI-0.0.6/setup.py` & `dbTelematelAPI-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path # > 3.6
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Permite consumir el API de Telematel'
 PACKAGE_NAME = 'dbTelematelAPI'
 AUTHOR = 'José María Sánchez González'
 EMAIL = 'miotroyo1970@gmail.com'
 GITHUB_URL = 'https://github.com/jmsanchez-ibiza/dbTelematelAPI'
 
 setup(
```

