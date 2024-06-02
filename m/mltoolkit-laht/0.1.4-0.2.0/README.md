# Comparing `tmp/mltoolkit-laht-0.1.4.tar.gz` & `tmp/mltoolkit-laht-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltoolkit-laht-0.1.4.tar", last modified: Thu May 30 19:41:44 2024, max compression
+gzip compressed data, was "mltoolkit-laht-0.2.0.tar", last modified: Sun Jun  2 16:08:13 2024, max compression
```

## Comparing `mltoolkit-laht-0.1.4.tar` & `mltoolkit-laht-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/mltoolkit_laht/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/mltoolkit_laht/data/
--rw-r--r--   0 runner    (1001) docker     (127)   239469 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/data/BankReviews.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/data_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/mltoolkit_laht/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/mltoolkit_laht/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/visualization/base_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/mltoolkit_laht/visualization/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/mltoolkit_laht.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-30 19:41:43.000000 mltoolkit-laht-0.1.4/mltoolkit_laht.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 19:41:44.000000 mltoolkit-laht-0.1.4/mltoolkit_laht.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:41:43.000000 mltoolkit-laht-0.1.4/mltoolkit_laht.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 19:41:43.000000 mltoolkit-laht-0.1.4/mltoolkit_laht.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 19:41:43.000000 mltoolkit-laht-0.1.4/mltoolkit_laht.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:41:44.045052 mltoolkit-laht-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/tests/test_data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 19:41:36.000000 mltoolkit-laht-0.1.4/tests/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   239469 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data/BankReviews.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/csv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/excel_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/show_info_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/base_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_preprocessing/data_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/base_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/data_visualization/features_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/evaluation/base_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/feature_engineering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/feature_engineering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/feature_engineering/base_feature_engineer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/modeling/base_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/mltoolkit_laht/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/mltoolkit_laht/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.103007 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 16:08:13.000000 mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:08:13.107007 mltoolkit-laht-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-06-02 16:08:05.000000 mltoolkit-laht-0.2.0/tests/test_visualization.py
```

### Comparing `mltoolkit-laht-0.1.4/LICENSE` & `mltoolkit-laht-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.1.4/README.md` & `mltoolkit-laht-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,24 @@
-# mltoolkit-laht 0.1.4
+Metadata-Version: 2.1
+Name: mltoolkit-laht
+Version: 0.2.0
+Summary: A data science and machine learning toolkit
+Home-page: https://github.com/lehidalgo/mltoolkit-laht
+Author: Leandro Alexis Hidalgo Torres
+Author-email: le.hidalgot@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mltoolkit-laht 0.2.0
 
 This is a Python library for data science and machine learning tasks. It provides utilities for data processing, modeling, and visualization.
 
 ## Installation
 
 To install this package, clone the repository and run the setup script:
 
@@ -10,35 +26,15 @@
 git clone https://github.com/lehidalgo/mltoolkit-laht
 cd mltoolkit-laht
 pip install .
 ```
 
 ## Usage
 
-Here is a basic example of how to use this toolkit:
-
-```python
-import pandas as pd
-from mltoolkit_laht import data_processing as dp
-from mltoolkit_laht.datasets import load_banking_reviews_data
-
-# ============================== Load Data ==============================
-data_reader = dp.DataSource(data=load_banking_reviews_data())
-
-# ============================== Data Preprocessing ==============================
-BankReviews = data_reader.load_data()
-BankReviews["Date"] = pd.to_datetime(BankReviews["Date"], format="%d-%m-%Y")
-BankReviews["Year"] = BankReviews["Date"].dt.year
-BankReviews["text_length"] = BankReviews.Reviews.apply(lambda x: len(x))
-
-# ============================== Data Exploration ==============================
-data_reader.show_df_info(num_rows=100)
-```
-
-Full example in Tutorials directory.
+Full examples in Tutorials directory.
 
 ## Testing
 
 To run the tests, use the following command:
 
 ```
 python -m unittest discover tests
@@ -54,7 +50,9 @@
 - matplotlib
 
 Please make sure to install these dependencies before using this toolkit.
 
 ## Contributing
 
 Contributions are welcome! Please submit a pull request or create an issue to propose changes or additions.
+
+
```

### Comparing `mltoolkit-laht-0.1.4/mltoolkit_laht/data/BankReviews.csv` & `mltoolkit-laht-0.2.0/mltoolkit_laht/data/BankReviews.csv`

 * *Files identical despite different names*

### Comparing `mltoolkit-laht-0.1.4/mltoolkit_laht/data_processing.py` & `mltoolkit-laht-0.2.0/mltoolkit_laht/data_loading/csv_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,66 @@
+import os
 import pandas as pd
 import numpy as np
 from IPython.display import display
+from .base_loader import BaseLoader
 
 
-class DataSource:
-
-    SCHEMA_UPDATED = False
-
-    def __init__(self, data: pd.DataFrame = None, file_path: str = None) -> None:
-        self.file_path = file_path
+class CSVLoader(BaseLoader):
+    def __init__(
+        self,
+        file_path: str = None,
+        data: pd.DataFrame = None,
+    ) -> None:
+        super().__init__(file_path)
         self.data = data
 
         if not isinstance(self.data, pd.DataFrame) and self.file_path is None:
-            raise ValueError("Please provide either a DataFrame or a file path.")
+            msg = "Please provide either a DataFrame or a file path."
+            self.logger.error(msg)
+            raise ValueError(msg)
 
     def load_data(self, **kwargs) -> pd.DataFrame:
         """
         Load data from a CSV file.
 
         Parameters:
         **kwargs: specific parameters for the read_csv or read_pickle method.
 
         Returns:
         None
         """
+        if self.file_path:
+            _, file_extension = os.path.splitext(self.file_path)
+            file_extension = file_extension[1:]  # remove the leading dot
+
         if isinstance(self.data, pd.DataFrame):
-            print("Loading data from DataFrame...")
+            self.logger.info("Loading data from DataFrame.")
             return self.data
         else:
-            print("Loading data from a file...")
-            file_extension = self.file_path.split(".")[-1]
             if file_extension == "csv":
+                self.logger.info("Reading data from a CSV file.")
                 self.data = pd.read_csv(self.file_path, **kwargs)
-            elif file_extension == "pkl" or file_extension == "pickle":
+            elif file_extension in ["pkl", "pickle"]:
+                self.logger.info("Reading data from a pickle file.")
                 self.data = pd.read_pickle(self.file_path, **kwargs)
             else:
-                raise ValueError(
-                    f"Unsupported file type: {self.file_path}. Only read pkl, pickle, and csv files."
-                )
+                msg = f"Unsupported file type: {self.file_path}. Only read .pkl, .pickle, and .csv files."
+                self.logger.error(msg)
+                raise ValueError(msg)
             return self.data
 
     def get_schema(self) -> dict:
         return self.data.dtypes.apply(lambda x: x.name).to_dict()
 
     def update_schema(self, new_schema: dict) -> None:
         self.data = self.data.astype(new_schema)
-        SCHEMA_UPDATED = True
         return self.data
 
-    def show_df_info(self, num_rows: int = None, describe_all: str = "all") -> None:
+    def show_info(self, num_rows: int = None, describe_all: str = "all") -> None:
         """
         Print the title and the content to show.
 
         Parameters:
         title (str): The title to print.
         to_show (Any): The content to print.
 
@@ -60,52 +68,34 @@
         None
         """
         if num_rows:
             pd.set_option("display.max_rows", num_rows)
 
         decor_title = "-" * 10
         decor_section = "=" * 100
+        data = self.data  # load data once
 
-        print(f"{decor_section}")
-        print(f"SAMPLE:\n{decor_title}")
-        display(self.data.head())
-        print(f"\n{decor_section}\n")
-        print(f"SCHEMA:\n{decor_title}\n{self.data.dtypes}\n{decor_section}\n")
-        print(f"DATAFRAME SHAPE:\n{decor_title}\n{self.data.shape}\n{decor_section}\n")
-        print(f"NANs:\n{decor_title}\n{self.data.isna().sum()}\n{decor_section}\n")
-        print(
-            f"GENERAL DUPLICATED:\n{decor_title}\n{self.data.duplicated().sum()}\n{decor_section}\n"
+        def print_section(name, content):
+            print(f"{decor_section}\n{name}:\n{decor_section}")
+            print(content)
+
+        print_section("SAMPLE", data.head())
+        print_section("SCHEMA", data.dtypes)
+        print_section("DATAFRAME SHAPE", data.shape)
+        print_section("NANs", data.isna().sum())
+        print_section("GENERAL DUPLICATED", data.duplicated().sum())
+        print_section(
+            "STATISTICS", data.describe(include=describe_all, datetime_is_numeric=True)
         )
-        print(f"STATISTICS:\n{decor_title}")
-        display(self.data.describe(include=describe_all, datetime_is_numeric=True))
-        print(f"\n{decor_section}\nINFO:\n")
-        print(f"{decor_title}\n{self.data.info()}\n{decor_section}")
-        for col in self.data.select_dtypes(exclude=np.number).columns:
-            if pd.api.types.is_categorical_dtype(self.data[col]):
-                display(self.data[col].value_counts())
-
-    @staticmethod
-    def clean_data(df: pd.DataFrame) -> None:
-        """
-        Clean the input DataFrame.
-
-        Parameters:
-        df (DataFrame): Input data.
 
-        Returns:
-        DataFrame: Cleaned data.
-        """
-        raise NotImplementedError("This method needs to be implemented")
+        print(f"{decor_section}\nINFO:\n{decor_section}")
+        data.info(verbose=True)
 
-    @staticmethod
-    def transform_data(df: pd.DataFrame) -> None:
-        """
-        Transform the input DataFrame.
+        categorical_columns = data.select_dtypes(exclude=np.number).columns
+        categorical_value_counts = [
+            data[col].value_counts()
+            for col in categorical_columns
+            if pd.api.types.is_categorical_dtype(data[col])
+        ]
 
-        Parameters:
-        df (DataFrame): Input data.
-
-        Returns:
-        DataFrame: Transformed data.
-        """
-        # Implement your data transformation logic here
-        raise NotImplementedError("This method needs to be implemented")
+        for value_counts in categorical_value_counts:
+            display(value_counts)
```

### Comparing `mltoolkit-laht-0.1.4/mltoolkit_laht.egg-info/SOURCES.txt` & `mltoolkit-laht-0.2.0/mltoolkit_laht.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 mltoolkit_laht/__init__.py
-mltoolkit_laht/data_processing.py
-mltoolkit_laht/models.py
-mltoolkit_laht/utils.py
 mltoolkit_laht.egg-info/PKG-INFO
 mltoolkit_laht.egg-info/SOURCES.txt
 mltoolkit_laht.egg-info/dependency_links.txt
 mltoolkit_laht.egg-info/requires.txt
 mltoolkit_laht.egg-info/top_level.txt
 mltoolkit_laht/data/BankReviews.csv
-mltoolkit_laht/datasets/__init__.py
-mltoolkit_laht/visualization/__init__.py
-mltoolkit_laht/visualization/base_plotter.py
-mltoolkit_laht/visualization/distributions.py
+mltoolkit_laht/data_loading/__init__.py
+mltoolkit_laht/data_loading/base_loader.py
+mltoolkit_laht/data_loading/csv_loader.py
+mltoolkit_laht/data_loading/excel_loader.py
+mltoolkit_laht/data_loading/json_loader.py
+mltoolkit_laht/data_loading/show_info_mixin.py
+mltoolkit_laht/data_preprocessing/__init__.py
+mltoolkit_laht/data_preprocessing/base_preprocessor.py
+mltoolkit_laht/data_preprocessing/data_processing.py
+mltoolkit_laht/data_visualization/__init__.py
+mltoolkit_laht/data_visualization/base_visualizer.py
+mltoolkit_laht/data_visualization/features_visualizer.py
+mltoolkit_laht/evaluation/__init__.py
+mltoolkit_laht/evaluation/base_evaluator.py
+mltoolkit_laht/feature_engineering/__init__.py
+mltoolkit_laht/feature_engineering/base_feature_engineer.py
+mltoolkit_laht/modeling/__init__.py
+mltoolkit_laht/modeling/base_trainer.py
+mltoolkit_laht/utils/__init__.py
+mltoolkit_laht/utils/logger.py
 tests/__init__.py
 tests/test_data_processing.py
 tests/test_models.py
 tests/test_utils.py
 tests/test_visualization.py
```

### Comparing `mltoolkit-laht-0.1.4/setup.py` & `mltoolkit-laht-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mltoolkit-laht",
-    version="0.1.4",
+    version="0.2.0",
     packages=find_packages(),
     include_package_data=True,
     package_data={
         "mltoolkit-laht": ["data/BankReviews.csv"],
     },
     install_requires=[
         "numpy",
```

