# Comparing `tmp/supervisedclustering-0.0.1.tar.gz` & `tmp/supervisedclustering-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supervisedclustering-0.0.1.tar", last modified: Thu Apr 18 13:55:16 2024, max compression
+gzip compressed data, was "supervisedclustering-0.0.2.tar", last modified: Sun Jun  2 06:49:58 2024, max compression
```

## Comparing `supervisedclustering-0.0.1.tar` & `supervisedclustering-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:55:16.869053 supervisedclustering-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 supervisedclustering-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      673 2024-04-18 13:55:16.869053 supervisedclustering-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       81 2024-04-18 13:54:12.000000 supervisedclustering-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 13:55:16.705020 supervisedclustering-0.0.1/SupervisedClustering/
--rw-rw-rw-   0        0        0       24 2024-04-18 13:48:32.000000 supervisedclustering-0.0.1/SupervisedClustering/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-18 13:48:51.000000 supervisedclustering-0.0.1/SupervisedClustering/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:55:16.869053 supervisedclustering-0.0.1/SupervisedClustering.egg-info/
--rw-rw-rw-   0        0        0      673 2024-04-18 13:55:16.000000 supervisedclustering-0.0.1/SupervisedClustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-18 13:55:16.000000 supervisedclustering-0.0.1/SupervisedClustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:55:16.000000 supervisedclustering-0.0.1/SupervisedClustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 13:55:16.000000 supervisedclustering-0.0.1/SupervisedClustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-18 13:55:16.000000 supervisedclustering-0.0.1/SupervisedClustering.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 13:55:16.869053 supervisedclustering-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      861 2024-04-18 13:53:34.000000 supervisedclustering-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:49:58.234586 supervisedclustering-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 supervisedclustering-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      673 2024-06-02 06:49:58.233074 supervisedclustering-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2024-04-18 13:54:12.000000 supervisedclustering-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 06:49:58.155096 supervisedclustering-0.0.2/SupervisedClustering/
+-rw-rw-rw-   0        0        0      115 2024-04-20 11:23:23.000000 supervisedclustering-0.0.2/SupervisedClustering/__init__.py
+-rw-rw-rw-   0        0        0    29674 2024-05-03 14:33:31.000000 supervisedclustering-0.0.2/SupervisedClustering/models.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:49:58.229033 supervisedclustering-0.0.2/SupervisedClustering.egg-info/
+-rw-rw-rw-   0        0        0      673 2024-06-02 06:49:57.000000 supervisedclustering-0.0.2/SupervisedClustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-06-02 06:49:57.000000 supervisedclustering-0.0.2/SupervisedClustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 06:49:57.000000 supervisedclustering-0.0.2/SupervisedClustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 06:49:57.000000 supervisedclustering-0.0.2/SupervisedClustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-06-02 06:49:57.000000 supervisedclustering-0.0.2/SupervisedClustering.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 06:49:58.234586 supervisedclustering-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      861 2024-06-02 06:47:28.000000 supervisedclustering-0.0.2/setup.py
```

### Comparing `supervisedclustering-0.0.1/LICENSE` & `supervisedclustering-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `supervisedclustering-0.0.1/PKG-INFO` & `supervisedclustering-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SupervisedClustering
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a package to apply clustering algorithms in supervised learning problems.
 Home-page: https://github.com/FabioScielzoOrtiz/SupervisedClustering_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `supervisedclustering-0.0.1/SupervisedClustering.egg-info/PKG-INFO` & `supervisedclustering-0.0.2/SupervisedClustering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SupervisedClustering
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a package to apply clustering algorithms in supervised learning problems.
 Home-page: https://github.com/FabioScielzoOrtiz/SupervisedClustering_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `supervisedclustering-0.0.1/setup.py` & `supervisedclustering-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="SupervisedClustering",
-    version="0.0.1",
+    version="0.0.2",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="This is a package to apply clustering algorithms in supervised learning problems.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/SupervisedClustering_Package",  # add your project URL here
     packages=find_packages(),
```

