# Comparing `tmp/datasetsfactory-0.2.tar.gz` & `tmp/datasetsfactory-0.3.tar.gz`

## Comparing `datasetsfactory-0.2.tar` & `datasetsfactory-0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 datasetsfactory-0.2/DatasetsFactory/DatasetsFactory.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 datasetsfactory-0.2/DatasetsFactory/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 datasetsfactory-0.2/DatasetsFactory/usefull.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 datasetsfactory-0.2/HOME/.pypirc
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 datasetsfactory-0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 datasetsfactory-0.2/LICENSE
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 datasetsfactory-0.2/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 datasetsfactory-0.2/pyproject.toml
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 datasetsfactory-0.2/PKG-INFO
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 datasetsfactory-0.3/DatasetsFactory/DatasetsFactory.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 datasetsfactory-0.3/DatasetsFactory/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 datasetsfactory-0.3/DatasetsFactory/usefull.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 datasetsfactory-0.3/HOME/.pypirc
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 datasetsfactory-0.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 datasetsfactory-0.3/LICENSE
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 datasetsfactory-0.3/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 datasetsfactory-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 datasetsfactory-0.3/PKG-INFO
```

### Comparing `datasetsfactory-0.2/DatasetsFactory/DatasetsFactory.py` & `datasetsfactory-0.3/DatasetsFactory/DatasetsFactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from requests import get
-from usefull import CreateDirectory
+from .usefull import CreateDirectory
 
 
 class Datasets:
 
     def __init__(self, token):
         _urlsite_ = "http://localhost/routes"
         # Link-ul catre endpoint-ul de listare a dataseturilor!
```

### Comparing `datasetsfactory-0.2/DatasetsFactory/usefull.py` & `datasetsfactory-0.3/DatasetsFactory/usefull.py`

 * *Files identical despite different names*

### Comparing `datasetsfactory-0.2/LICENSE` & `datasetsfactory-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasetsfactory-0.2/README.md` & `datasetsfactory-0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pip install DatasetsFactory
 ```
 
 ## Usage
 > [!IMPORTANT] 
 > Everytime you want to load a dataset you must follow every step bellow !
 ```python
-from DatasetsFactory.DatasetsFactory import Datasets
+from DatasetsFactory import Datasets
 # Get the token from your profile!
 token = "928e4f5f-50e7-4f06-aaac-459d4c5db8ac"
 # Initialize the library with the token of the user
 init_dataset = Datasets(token)
 
 # Visualize the datasets on which you have privileges
 init_dataset.view_datasets() # -> return None
```

### Comparing `datasetsfactory-0.2/pyproject.toml` & `datasetsfactory-0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DatasetsFactory"
-version = "0.2"
+version = "0.3"
 license = {file = "LICENSE"}
 authors = [
   { name="Denis Ariton", email="denis.ariton@student.upt.ro" },
 ]
 description = "This library is meant to DatasetsFactory app users, and is used for loading the available datasets locally!"
 readme = "README.md"
 requires-python = ">=3.12"
```

### Comparing `datasetsfactory-0.2/PKG-INFO` & `datasetsfactory-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: DatasetsFactory
-Version: 0.2
+Version: 0.3
 Summary: This library is meant to DatasetsFactory app users, and is used for loading the available datasets locally!
 Project-URL: GitHub, https://github.com/DenisAriton/DatasetsFactory_Library
 Author-email: Denis Ariton <denis.ariton@student.upt.ro>
 License: MIT License
         
         Copyright (c) 2024  DatasetsFactory
         
@@ -47,15 +47,15 @@
 pip install DatasetsFactory
 ```
 
 ## Usage
 > [!IMPORTANT] 
 > Everytime you want to load a dataset you must follow every step bellow !
 ```python
-from DatasetsFactory.DatasetsFactory import Datasets
+from DatasetsFactory import Datasets
 # Get the token from your profile!
 token = "928e4f5f-50e7-4f06-aaac-459d4c5db8ac"
 # Initialize the library with the token of the user
 init_dataset = Datasets(token)
 
 # Visualize the datasets on which you have privileges
 init_dataset.view_datasets() # -> return None
```

