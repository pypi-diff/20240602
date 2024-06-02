# Comparing `tmp/vtacML-0.1.4.tar.gz` & `tmp/vtacML-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtacML-0.1.4.tar", last modified: Sun Jun  2 13:49:20 2024, max compression
+gzip compressed data, was "vtacML-0.1.5.tar", last modified: Sun Jun  2 13:57:30 2024, max compression
```

## Comparing `vtacML-0.1.4.tar` & `vtacML-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:49:20.502373 vtacML-0.1.4/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.4/LICENSE
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:49:20.502153 vtacML-0.1.4/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       84 2024-02-23 14:25:44.000000 vtacML-0.1.4/README.md
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.4/pyproject.toml
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-06-02 13:49:20.502425 vtacML-0.1.4/setup.cfg
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1187 2024-06-02 13:43:38.000000 vtacML-0.1.4/setup.py
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:49:20.501787 vtacML-0.1.4/vtacML.egg-info/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      190 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/SOURCES.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/dependency_links.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       99 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/requires.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-06-02 13:49:20.000000 vtacML-0.1.4/vtacML.egg-info/top_level.txt
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.568168 vtacML-0.1.5/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.5/LICENSE
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:57:30.567947 vtacML-0.1.5/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       84 2024-02-23 14:25:44.000000 vtacML-0.1.5/README.md
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.5/pyproject.toml
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-06-02 13:57:30.568213 vtacML-0.1.5/setup.cfg
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1185 2024-06-02 13:57:21.000000 vtacML-0.1.5/setup.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.565577 vtacML-0.1.5/vtacML/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       33 2024-06-02 13:40:23.000000 vtacML-0.1.5/vtacML/__init__.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      630 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/evaluate_best_model.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)    18180 2024-05-31 19:27:43.000000 vtacML-0.1.5/vtacML/pipeline.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     3764 2024-05-24 17:26:07.000000 vtacML-0.1.5/vtacML/preparation.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      206 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/search_best_model.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.567550 vtacML-0.1.5/vtacML/testing/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 17:36:29.000000 vtacML-0.1.5/vtacML/testing/__init__.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      365 2024-04-10 18:56:40.000000 vtacML-0.1.5/vtacML/testing/config.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      853 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/testing/resampler.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1115 2024-03-28 12:06:52.000000 vtacML-0.1.5/vtacML/testing/training.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      240 2024-03-28 12:06:52.000000 vtacML-0.1.5/vtacML/testing/validation.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      411 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/testing/wrapper.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.566359 vtacML-0.1.5/vtacML.egg-info/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      470 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       99 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/requires.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        7 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/top_level.txt
```

### Comparing `vtacML-0.1.4/LICENSE` & `vtacML-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.4/PKG-INFO` & `vtacML-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.4
+Version: 0.1.5
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vtacML-0.1.4/setup.py` & `vtacML-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vtacML',
-    version='0.1.4',
-    packages=find_packages(include=['testing', 'testing.*']),
+    version='0.1.5',
+    packages=find_packages(include=['vtacML', 'vtacML.*']),
     install_requires=[
         'numpy>=1.26.3',
         'matplotlib>=3.8.0',
         'pandas>=2.1.4',
         'scikit-learn>=1.3.0',
         'seaborn>=0.12.2',
         'yellowbrick>=1.5'
```

### Comparing `vtacML-0.1.4/vtacML.egg-info/PKG-INFO` & `vtacML-0.1.5/vtacML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.4
+Version: 0.1.5
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

