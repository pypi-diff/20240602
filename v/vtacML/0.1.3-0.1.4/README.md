# Comparing `tmp/vtacML-0.1.3.tar.gz` & `tmp/vtacML-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtacML-0.1.3.tar", last modified: Fri May 31 19:54:38 2024, max compression
+gzip compressed data, was "vtacML-0.1.4.tar", last modified: Sun Jun  2 13:49:20 2024, max compression
```

## Comparing `vtacML-0.1.3.tar` & `vtacML-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:54:38.340451 vtacML-0.1.3/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.3/LICENSE
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-05-31 19:54:38.340222 vtacML-0.1.3/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       84 2024-02-23 14:25:44.000000 vtacML-0.1.3/README.md
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.3/pyproject.toml
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-05-31 19:54:38.340505 vtacML-0.1.3/setup.cfg
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1187 2024-05-31 19:54:31.000000 vtacML-0.1.3/setup.py
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 19:54:38.339903 vtacML-0.1.3/vtacML.egg-info/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-05-31 19:54:38.000000 vtacML-0.1.3/vtacML.egg-info/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      190 2024-05-31 19:54:38.000000 vtacML-0.1.3/vtacML.egg-info/SOURCES.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-05-31 19:54:38.000000 vtacML-0.1.3/vtacML.egg-info/dependency_links.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       99 2024-05-31 19:54:38.000000 vtacML-0.1.3/vtacML.egg-info/requires.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-05-31 19:54:38.000000 vtacML-0.1.3/vtacML.egg-info/top_level.txt
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:49:20.502373 vtacML-0.1.4/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.4/LICENSE
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:49:20.502153 vtacML-0.1.4/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       84 2024-02-23 14:25:44.000000 vtacML-0.1.4/README.md
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.4/pyproject.toml
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-06-02 13:49:20.502425 vtacML-0.1.4/setup.cfg
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1187 2024-06-02 13:43:38.000000 vtacML-0.1.4/setup.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:49:20.501787 vtacML-0.1.4/vtacML.egg-info/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      190 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       99 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/requires.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/top_level.txt
```

### Comparing `vtacML-0.1.3/LICENSE` & `vtacML-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.3/PKG-INFO` & `vtacML-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.3
+Version: 0.1.4
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vtacML-0.1.3/setup.py` & `vtacML-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vtacML',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(include=['testing', 'testing.*']),
     install_requires=[
         'numpy>=1.26.3',
         'matplotlib>=3.8.0',
         'pandas>=2.1.4',
         'scikit-learn>=1.3.0',
         'seaborn>=0.12.2',
```

### Comparing `vtacML-0.1.3/vtacML.egg-info/PKG-INFO` & `vtacML-0.1.4/vtacML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.3
+Version: 0.1.4
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

