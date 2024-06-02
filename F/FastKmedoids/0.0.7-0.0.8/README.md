# Comparing `tmp/FastKmedoids-0.0.7.tar.gz` & `tmp/fastkmedoids-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastKmedoids-0.0.7.tar", last modified: Wed Feb 14 16:48:02 2024, max compression
+gzip compressed data, was "fastkmedoids-0.0.8.tar", last modified: Sun Jun  2 06:35:09 2024, max compression
```

## Comparing `FastKmedoids-0.0.7.tar` & `fastkmedoids-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 16:48:02.421787 FastKmedoids-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-02-14 16:48:02.384909 FastKmedoids-0.0.7/FastKmedoids/
--rw-rw-rw-   0        0        0       73 2024-02-14 16:27:52.000000 FastKmedoids-0.0.7/FastKmedoids/FastKmedoids.py
--rw-rw-rw-   0        0        0       42 2024-02-14 16:27:28.000000 FastKmedoids-0.0.7/FastKmedoids/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-14 16:48:02.418787 FastKmedoids-0.0.7/FastKmedoids.egg-info/
--rw-rw-rw-   0        0        0     1005 2024-02-14 16:48:02.000000 FastKmedoids-0.0.7/FastKmedoids.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-02-14 16:48:02.000000 FastKmedoids-0.0.7/FastKmedoids.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 16:48:02.000000 FastKmedoids-0.0.7/FastKmedoids.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-02-14 16:48:02.000000 FastKmedoids-0.0.7/FastKmedoids.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-14 16:48:02.000000 FastKmedoids-0.0.7/FastKmedoids.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 FastKmedoids-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1005 2024-02-14 16:48:02.420786 FastKmedoids-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-02-14 16:24:48.000000 FastKmedoids-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-02-14 16:48:02.422788 FastKmedoids-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      951 2024-02-14 16:46:33.000000 FastKmedoids-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:35:09.606778 fastkmedoids-0.0.8/
+drwxrwxrwx   0        0        0        0 2024-06-02 06:35:09.602823 fastkmedoids-0.0.8/FastKmedoids.egg-info/
+-rw-rw-rw-   0        0        0      894 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 06:35:09.000000 fastkmedoids-0.0.8/FastKmedoids.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 fastkmedoids-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      894 2024-06-02 06:35:09.604465 fastkmedoids-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-02-14 16:49:17.000000 fastkmedoids-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 06:35:09.606778 fastkmedoids-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      951 2024-06-02 06:34:37.000000 fastkmedoids-0.0.8/setup.py
```

### Comparing `FastKmedoids-0.0.7/FastKmedoids.egg-info/PKG-INFO` & `fastkmedoids-0.0.8/FastKmedoids.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: FastKmedoids
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a package to implement a fast and powerful version of the Kmedoids clustering algorithm, which is built on the Generalised Gower distance, already available in the PyDistances package
 Home-page: https://github.com/FabioScielzoOrtiz/FastKmedoids_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: polars
 Requires-Dist: numpy
 
-This is a package to carry out Exploratory Data Analysis, allowing to work on Big Data.
-
-We are currently working to develop the package.
+PACKAGE UNDER CONSTRUCTION. 
 
 Usage:
 
 ```python
 pip install FastKmedoids --upgrade
 ```
```

### Comparing `FastKmedoids-0.0.7/LICENSE` & `fastkmedoids-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FastKmedoids-0.0.7/PKG-INFO` & `fastkmedoids-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: FastKmedoids
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a package to implement a fast and powerful version of the Kmedoids clustering algorithm, which is built on the Generalised Gower distance, already available in the PyDistances package
 Home-page: https://github.com/FabioScielzoOrtiz/FastKmedoids_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: polars
 Requires-Dist: numpy
 
-This is a package to carry out Exploratory Data Analysis, allowing to work on Big Data.
-
-We are currently working to develop the package.
+PACKAGE UNDER CONSTRUCTION. 
 
 Usage:
 
 ```python
 pip install FastKmedoids --upgrade
 ```
```

