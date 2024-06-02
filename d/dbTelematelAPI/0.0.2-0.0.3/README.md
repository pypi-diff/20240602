# Comparing `tmp/dbTelematelAPI-0.0.2.tar.gz` & `tmp/dbTelematelAPI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbTelematelAPI-0.0.2.tar", last modified: Sun Jun  2 13:17:29 2024, max compression
+gzip compressed data, was "dbTelematelAPI-0.0.3.tar", last modified: Sun Jun  2 13:37:33 2024, max compression
```

## Comparing `dbTelematelAPI-0.0.2.tar` & `dbTelematelAPI-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 13:17:29.721609 dbTelematelAPI-0.0.2/
--rw-rw-rw-   0        0        0      634 2024-06-02 13:17:29.721609 dbTelematelAPI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-06-02 13:05:32.000000 dbTelematelAPI-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 13:17:29.569199 dbTelematelAPI-0.0.2/dbTelematelAPI/
--rw-rw-rw-   0        0        0       67 2024-06-02 13:05:32.000000 dbTelematelAPI-0.0.2/dbTelematelAPI/__init__.py
--rw-rw-rw-   0        0        0      231 2024-06-02 13:05:32.000000 dbTelematelAPI-0.0.2/dbTelematelAPI/__main__.py
--rw-rw-rw-   0        0        0      233 2024-06-02 13:05:32.000000 dbTelematelAPI-0.0.2/dbTelematelAPI/funciones.py
-drwxrwxrwx   0        0        0        0 2024-06-02 13:17:29.721609 dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/
--rw-rw-rw-   0        0        0      634 2024-06-02 13:17:29.000000 dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-06-02 13:17:29.000000 dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 13:17:29.000000 dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-06-02 13:17:29.000000 dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 13:17:29.000000 dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-06-02 13:17:29.000000 dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2024-06-02 13:14:24.000000 dbTelematelAPI-0.0.2/license.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 13:17:29.734426 dbTelematelAPI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1222 2024-06-02 13:16:34.000000 dbTelematelAPI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:37:33.384897 dbTelematelAPI-0.0.3/
+-rw-rw-rw-   0        0        0      634 2024-06-02 13:37:33.367780 dbTelematelAPI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-06-02 13:05:32.000000 dbTelematelAPI-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 13:37:33.282191 dbTelematelAPI-0.0.3/dbTelematelAPI/
+-rw-rw-rw-   0        0        0       67 2024-06-02 13:05:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI/__init__.py
+-rw-rw-rw-   0        0        0      231 2024-06-02 13:05:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI/__main__.py
+-rw-rw-rw-   0        0        0      318 2024-06-02 13:32:14.000000 dbTelematelAPI-0.0.3/dbTelematelAPI/funciones.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:37:33.367780 dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-06-02 13:37:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-06-02 13:37:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 13:37:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-06-02 13:37:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 13:37:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-02 13:37:32.000000 dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2024-06-02 13:14:24.000000 dbTelematelAPI-0.0.3/license.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 13:37:33.384897 dbTelematelAPI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1222 2024-06-02 13:34:37.000000 dbTelematelAPI-0.0.3/setup.py
```

### Comparing `dbTelematelAPI-0.0.2/PKG-INFO` & `dbTelematelAPI-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbTelematelAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Permite consumir el API de CódigoFacilito
 Home-page: https://github.com/jmsanchez-ibiza/dbTelematelAPI
 Author: José María Sánchez González
 Author-email: miotroyo1970@gmail.com
 License: MIT
 Keywords: codigofacilito
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dbTelematelAPI-0.0.2/dbTelematelAPI.egg-info/PKG-INFO` & `dbTelematelAPI-0.0.3/dbTelematelAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbTelematelAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Permite consumir el API de CódigoFacilito
 Home-page: https://github.com/jmsanchez-ibiza/dbTelematelAPI
 Author: José María Sánchez González
 Author-email: miotroyo1970@gmail.com
 License: MIT
 Keywords: codigofacilito
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dbTelematelAPI-0.0.2/license.txt` & `dbTelematelAPI-0.0.3/license.txt`

 * *Files identical despite different names*

### Comparing `dbTelematelAPI-0.0.2/setup.py` & `dbTelematelAPI-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path # > 3.6
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Permite consumir el API de CódigoFacilito'
 PACKAGE_NAME = 'dbTelematelAPI'
 AUTHOR = 'José María Sánchez González'
 EMAIL = 'miotroyo1970@gmail.com'
 GITHUB_URL = 'https://github.com/jmsanchez-ibiza/dbTelematelAPI'
 
 setup(
```

