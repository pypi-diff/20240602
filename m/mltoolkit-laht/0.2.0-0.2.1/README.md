# Comparing `tmp/mltoolkit-laht-0.2.0.tar.gz` & `tmp/mltoolkit-laht-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltoolkit-laht-0.2.0.tar", last modified: Sun Jun  2 16:08:13 2024, max compression
+gzip compressed data, was "mltoolkit-laht-0.2.1.tar", last modified: Sun Jun  2 16:25:49 2024, max compression
```

## Comparing `mltoolkit-laht-0.2.0.tar` & `mltoolkit-laht-0.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data/
--rw-r--r--   0 runner    (1001) docker     (127)   239469 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data/BankReviews.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/base_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/csv_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/excel_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/show_info_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/base_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/data_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/base_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/features_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/evaluation/base_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/feature_engineering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/feature_engineering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/feature_engineering/base_feature_engineer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/modeling/base_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/mltoolkit_laht/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.290964 mltoolkit-laht-0.2.1/mltoolkit_laht/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.290964 mltoolkit-laht-0.2.1/mltoolkit_laht/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   239469 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data/BankReviews.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.290964 mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/excel_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/show_info_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.290964 mltoolkit-laht-0.2.1/mltoolkit_laht/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_preprocessing/base_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_preprocessing/data_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.290964 mltoolkit-laht-0.2.1/mltoolkit_laht/data_visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_visualization/base_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/data_visualization/features_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/mltoolkit_laht/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/evaluation/base_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/mltoolkit_laht/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/feature_engineering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/feature_engineering/base_feature_engineer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/mltoolkit_laht/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/modeling/base_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/mltoolkit_laht/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/mltoolkit_laht/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.290964 mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-02 16:25:49.000000 mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-06-02 16:25:49.000000 mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:25:49.000000 mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 16:25:49.000000 mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 16:25:49.000000 mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:25:49.294964 mltoolkit-laht-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/tests/test_data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-06-02 16:25:41.000000 mltoolkit-laht-0.2.1/tests/test_visualization.py
```

### Comparing `mltoolkit-laht-0.2.0/LICENSE` & `mltoolkit-laht-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/PKG-INFO` & `mltoolkit-laht-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mltoolkit-laht
-Version: 0.2.0
+Version: 0.2.1
 Summary: A data science and machine learning toolkit
 Home-page: https://github.com/lehidalgo/mltoolkit-laht
 Author: Leandro Alexis Hidalgo Torres
 Author-email: le.hidalgot@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# mltoolkit-laht 0.2.0
+# mltoolkit-laht 0.2.1
 
 This is a Python library for data science and machine learning tasks. It provides utilities for data processing, modeling, and visualization.
 
 ## Installation
 
 To install this package, clone the repository and run the setup script:
```

### Comparing `mltoolkit-laht-0.2.0/README.md` & `mltoolkit-laht-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mltoolkit-laht 0.2.0
+# mltoolkit-laht 0.2.1
 
 This is a Python library for data science and machine learning tasks. It provides utilities for data processing, modeling, and visualization.
 
 ## Installation
 
 To install this package, clone the repository and run the setup script:
```

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data/BankReviews.csv` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data/BankReviews.csv`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/__init__.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/__init__.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/base_loader.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/base_loader.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/csv_loader.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/csv_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,19 +54,21 @@
 
     def update_schema(self, new_schema: dict) -> None:
         self.data = self.data.astype(new_schema)
         return self.data
 
     def show_info(self, num_rows: int = None, describe_all: str = "all") -> None:
         """
-        Print the title and the content to show.
+        Show data information, including the first few rows, schema, shape, NANs, duplicates, and statistics.
 
         Parameters:
-        title (str): The title to print.
-        to_show (Any): The content to print.
+        - num_rows (int): The number of rows to display. If None, all rows will be displayed.
+        - describe_all (str): The option to include all columns in the describe method.
+          Possible values: "all", "None", "number", "category", "datetime", "timedelta".
+          Default is "all".
 
         Returns:
         None
         """
         if num_rows:
             pd.set_option("display.max_rows", num_rows)
 
@@ -74,22 +76,22 @@
         decor_section = "=" * 100
         data = self.data  # load data once
 
         def print_section(name, content):
             print(f"{decor_section}\n{name}:\n{decor_section}")
             print(content)
 
-        print_section("SAMPLE", data.head())
+        print(f"{decor_section}\nINFO:\n{decor_section}")
+        display(data.head())
         print_section("SCHEMA", data.dtypes)
         print_section("DATAFRAME SHAPE", data.shape)
         print_section("NANs", data.isna().sum())
         print_section("GENERAL DUPLICATED", data.duplicated().sum())
-        print_section(
-            "STATISTICS", data.describe(include=describe_all, datetime_is_numeric=True)
-        )
+        print(f"{decor_section}\nSTATISTICS:\n{decor_section}")
+        display(data.describe(include=describe_all))
 
         print(f"{decor_section}\nINFO:\n{decor_section}")
         data.info(verbose=True)
 
         categorical_columns = data.select_dtypes(exclude=np.number).columns
         categorical_value_counts = [
             data[col].value_counts()
```

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/excel_loader.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/excel_loader.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/json_loader.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/json_loader.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/show_info_mixin.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_loading/show_info_mixin.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/data_processing.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_preprocessing/data_processing.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/base_visualizer.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_visualization/base_visualizer.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/features_visualizer.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/data_visualization/features_visualizer.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht/utils/logger.py` & `mltoolkit-laht-0.2.1/mltoolkit_laht/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/PKG-INFO` & `mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mltoolkit-laht
-Version: 0.2.0
+Version: 0.2.1
 Summary: A data science and machine learning toolkit
 Home-page: https://github.com/lehidalgo/mltoolkit-laht
 Author: Leandro Alexis Hidalgo Torres
 Author-email: le.hidalgot@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# mltoolkit-laht 0.2.0
+# mltoolkit-laht 0.2.1
 
 This is a Python library for data science and machine learning tasks. It provides utilities for data processing, modeling, and visualization.
 
 ## Installation
 
 To install this package, clone the repository and run the setup script:
```

### Comparing `mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/SOURCES.txt` & `mltoolkit-laht-0.2.1/mltoolkit_laht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.2.0/setup.py` & `mltoolkit-laht-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mltoolkit-laht",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     include_package_data=True,
     package_data={
         "mltoolkit-laht": ["data/BankReviews.csv"],
     },
     install_requires=[
         "numpy",
```

### Comparing `mltoolkit-laht-0.2.0/tests/test_data_processing.py` & `mltoolkit-laht-0.2.1/tests/test_data_processing.py`

 * *Files identical despite different names*

