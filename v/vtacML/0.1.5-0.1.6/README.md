# Comparing `tmp/vtacML-0.1.5.tar.gz` & `tmp/vtacML-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtacML-0.1.5.tar", last modified: Sun Jun  2 13:57:30 2024, max compression
+gzip compressed data, was "vtacML-0.1.6.tar", last modified: Sun Jun  2 14:10:19 2024, max compression
```

## Comparing `vtacML-0.1.5.tar` & `vtacML-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.568168 vtacML-0.1.5/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.5/LICENSE
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:57:30.567947 vtacML-0.1.5/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       84 2024-02-23 14:25:44.000000 vtacML-0.1.5/README.md
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.5/pyproject.toml
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-06-02 13:57:30.568213 vtacML-0.1.5/setup.cfg
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1185 2024-06-02 13:57:21.000000 vtacML-0.1.5/setup.py
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.565577 vtacML-0.1.5/vtacML/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       33 2024-06-02 13:40:23.000000 vtacML-0.1.5/vtacML/__init__.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      630 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/evaluate_best_model.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)    18180 2024-05-31 19:27:43.000000 vtacML-0.1.5/vtacML/pipeline.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     3764 2024-05-24 17:26:07.000000 vtacML-0.1.5/vtacML/preparation.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      206 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/search_best_model.py
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.567550 vtacML-0.1.5/vtacML/testing/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 17:36:29.000000 vtacML-0.1.5/vtacML/testing/__init__.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      365 2024-04-10 18:56:40.000000 vtacML-0.1.5/vtacML/testing/config.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      853 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/testing/resampler.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1115 2024-03-28 12:06:52.000000 vtacML-0.1.5/vtacML/testing/training.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      240 2024-03-28 12:06:52.000000 vtacML-0.1.5/vtacML/testing/validation.py
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      411 2024-05-31 19:09:48.000000 vtacML-0.1.5/vtacML/testing/wrapper.py
-drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 13:57:30.566359 vtacML-0.1.5/vtacML.egg-info/
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      769 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/PKG-INFO
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)      470 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/SOURCES.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/dependency_links.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)       99 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/requires.txt
--rw-r--r--   0 jeremypalmerio   (501) staff       (20)        7 2024-06-02 13:57:30.000000 vtacML-0.1.5/vtacML.egg-info/top_level.txt
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 14:10:19.889392 vtacML-0.1.6/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1496 2024-02-23 14:25:44.000000 vtacML-0.1.6/LICENSE
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      827 2024-06-02 14:10:19.889148 vtacML-0.1.6/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       84 2024-02-23 14:25:44.000000 vtacML-0.1.6/README.md
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       94 2024-05-31 18:21:42.000000 vtacML-0.1.6/pyproject.toml
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       38 2024-06-02 14:10:19.889438 vtacML-0.1.6/setup.cfg
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1235 2024-06-02 14:10:05.000000 vtacML-0.1.6/setup.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 14:10:19.886145 vtacML-0.1.6/vtacML/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)       33 2024-06-02 13:40:23.000000 vtacML-0.1.6/vtacML/__init__.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      624 2024-06-02 14:09:54.000000 vtacML-0.1.6/vtacML/evaluate_best_model.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)    18181 2024-06-02 14:08:45.000000 vtacML-0.1.6/vtacML/pipeline.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     3764 2024-05-24 17:26:07.000000 vtacML-0.1.6/vtacML/preparation.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      200 2024-06-02 14:09:54.000000 vtacML-0.1.6/vtacML/search_best_model.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 14:10:19.888600 vtacML-0.1.6/vtacML/testing/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        0 2024-05-31 17:36:29.000000 vtacML-0.1.6/vtacML/testing/__init__.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      365 2024-04-10 18:56:40.000000 vtacML-0.1.6/vtacML/testing/config.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      853 2024-05-31 19:09:48.000000 vtacML-0.1.6/vtacML/testing/resampler.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)     1115 2024-03-28 12:06:52.000000 vtacML-0.1.6/vtacML/testing/training.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      240 2024-03-28 12:06:52.000000 vtacML-0.1.6/vtacML/testing/validation.py
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      411 2024-05-31 19:09:48.000000 vtacML-0.1.6/vtacML/testing/wrapper.py
+drwxr-xr-x   0 jeremypalmerio   (501) staff       (20)        0 2024-06-02 14:10:19.886918 vtacML-0.1.6/vtacML.egg-info/
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      827 2024-06-02 14:10:19.000000 vtacML-0.1.6/vtacML.egg-info/PKG-INFO
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      470 2024-06-02 14:10:19.000000 vtacML-0.1.6/vtacML.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        1 2024-06-02 14:10:19.000000 vtacML-0.1.6/vtacML.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)      127 2024-06-02 14:10:19.000000 vtacML-0.1.6/vtacML.egg-info/requires.txt
+-rw-r--r--   0 jeremypalmerio   (501) staff       (20)        7 2024-06-02 14:10:19.000000 vtacML-0.1.6/vtacML.egg-info/top_level.txt
```

### Comparing `vtacML-0.1.5/LICENSE` & `vtacML-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.5/PKG-INFO` & `vtacML-0.1.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.5
+Version: 0.1.6
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,10 +14,12 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: yellowbrick>=1.5
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: imblearn>=0.0
 
 # VTAC_ML
 Applying machine learning tools to identifying GRBs from simulated data.
```

### Comparing `vtacML-0.1.5/setup.py` & `vtacML-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vtacML',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(include=['vtacML', 'vtacML.*']),
     install_requires=[
         'numpy>=1.26.3',
         'matplotlib>=3.8.0',
         'pandas>=2.1.4',
         'scikit-learn>=1.3.0',
         'seaborn>=0.12.2',
-        'yellowbrick>=1.5'
+        'yellowbrick>=1.5',
+        'pyyaml>=6.0.1',
+        'imblearn>=0.0'
         # List your dependencies here
         # Example: 'numpy', 'pandas', 'scikit-learn',
     ],
     entry_points={
         'console_scripts': [
             # Define any command-line scripts here
             # Example: 'vtac_classifier=pipeline:main',
```

### Comparing `vtacML-0.1.5/vtacML/evaluate_best_model.py` & `vtacML-0.1.6/vtacML/evaluate_best_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from vtacML.pipeline import VTACMLPipe
+from .pipeline import VTACMLPipe
 
 if __name__ == '__main__':
     config_path = "config/config.yaml"
     vtac_ml = VTACMLPipe(config_path=config_path)
 
     best_model_paths = [
         # '../output/models/ada_grid_search.pkl',
```

### Comparing `vtacML-0.1.5/vtacML/pipeline.py` & `vtacML-0.1.6/vtacML/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from sklearn.model_selection import train_test_split, GridSearchCV
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import StandardScaler, Normalizer
 from imblearn.over_sampling import SMOTE
 from yellowbrick import ClassBalance, ROCAUC
 from yellowbrick.model_selection import FeatureImportances, ValidationCurve
 
-from preparation import OneHotEncoderCustom, Cleaner
+from .preparation import OneHotEncoderCustom, Cleaner
 import matplotlib.pyplot as plt
 from yellowbrick.features import ParallelCoordinates
 from yellowbrick.classifier import ClassificationReport, ConfusionMatrix, PrecisionRecallCurve, ClassPredictionError
 from yellowbrick.model_selection import RFECV
 
 log = logging.getLogger(__name__)
```

### Comparing `vtacML-0.1.5/vtacML/preparation.py` & `vtacML-0.1.6/vtacML/preparation.py`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.5/vtacML/testing/resampler.py` & `vtacML-0.1.6/vtacML/testing/resampler.py`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.5/vtacML/testing/training.py` & `vtacML-0.1.6/vtacML/testing/training.py`

 * *Files identical despite different names*

### Comparing `vtacML-0.1.5/vtacML.egg-info/PKG-INFO` & `vtacML-0.1.6/vtacML.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtacML
-Version: 0.1.5
+Version: 0.1.6
 Summary: A machine learning pipeline to classify objects in VTAC dataset as GRB or not.
 Home-page: https://github.com/jerbeario/VTAC_ML
 Author: Jeremy Palmerio
 Author-email: jeremypalmerio05@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,10 +14,12 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: seaborn>=0.12.2
 Requires-Dist: yellowbrick>=1.5
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: imblearn>=0.0
 
 # VTAC_ML
 Applying machine learning tools to identifying GRBs from simulated data.
```

