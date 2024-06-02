# Comparing `tmp/beforerr-2024.6.1.tar.gz` & `tmp/beforerr-2024.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beforerr-2024.6.1.tar", last modified: Sat Jun  1 07:03:20 2024, max compression
+gzip compressed data, was "beforerr-2024.6.2.tar", last modified: Sun Jun  2 08:04:04 2024, max compression
```

## Comparing `beforerr-2024.6.1.tar` & `beforerr-2024.6.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11337 2024-03-29 05:10:27.069558 beforerr-2024.6.1/LICENSE
--rw-r--r--   0        0        0      185 2024-05-31 23:01:42.632680 beforerr-2024.6.1/README.md
--rw-r--r--   0        0        0       24 2024-06-01 07:03:19.687102 beforerr-2024.6.1/beforerr/__init__.py
--rw-r--r--   0        0        0     2609 2024-06-01 07:03:19.692046 beforerr-2024.6.1/beforerr/_modidx.py
--rw-r--r--   0        0        0      338 2024-06-01 07:03:19.678235 beforerr-2024.6.1/beforerr/basics.py
--rw-r--r--   0        0        0      214 2024-06-01 07:03:19.677426 beforerr-2024.6.1/beforerr/core.py
--rw-r--r--   0        0        0      965 2024-06-01 07:03:19.680479 beforerr-2024.6.1/beforerr/matplotlib.py
--rw-r--r--   0        0        0     3546 2024-06-01 07:03:19.683037 beforerr-2024.6.1/beforerr/polars.py
--rw-r--r--   0        0        0     5504 2024-06-01 07:03:19.686381 beforerr-2024.6.1/beforerr/project.py
--rw-r--r--   0        0        0      811 2024-06-01 07:03:19.679199 beforerr-2024.6.1/beforerr/r.py
--rw-r--r--   0        0        0      955 2024-06-01 07:03:20.955535 beforerr-2024.6.1/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 beforerr-2024.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-03-29 05:10:27.069558 beforerr-2024.6.2/LICENSE
+-rw-r--r--   0        0        0      185 2024-06-01 07:09:11.899951 beforerr-2024.6.2/README.md
+-rw-r--r--   0        0        0       24 2024-06-02 08:04:02.940109 beforerr-2024.6.2/beforerr/__init__.py
+-rw-r--r--   0        0        0     2837 2024-06-02 08:04:02.946069 beforerr-2024.6.2/beforerr/_modidx.py
+-rw-r--r--   0        0        0      338 2024-06-02 08:04:02.930348 beforerr-2024.6.2/beforerr/basics.py
+-rw-r--r--   0        0        0      214 2024-06-02 08:04:02.929336 beforerr-2024.6.2/beforerr/core.py
+-rw-r--r--   0        0        0      965 2024-06-02 08:04:02.932699 beforerr-2024.6.2/beforerr/matplotlib.py
+-rw-r--r--   0        0        0     3925 2024-06-02 08:04:02.935706 beforerr-2024.6.2/beforerr/polars.py
+-rw-r--r--   0        0        0     5504 2024-06-02 08:04:02.939523 beforerr-2024.6.2/beforerr/project.py
+-rw-r--r--   0        0        0      811 2024-06-02 08:04:02.931478 beforerr-2024.6.2/beforerr/r.py
+-rw-r--r--   0        0        0      955 2024-06-02 08:04:04.447049 beforerr-2024.6.2/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 beforerr-2024.6.2/PKG-INFO
```

### Comparing `beforerr-2024.6.1/LICENSE` & `beforerr-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beforerr-2024.6.1/beforerr/_modidx.py` & `beforerr-2024.6.2/beforerr/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
             'beforerr.core': {'beforerr.core.ifnone': ('core.html#ifnone', 'beforerr/core.py')},
             'beforerr.matplotlib': { 'beforerr.matplotlib.unify_axes_fontsize': ( 'matplotlib.html#unify_axes_fontsize',
                                                                                   'beforerr/matplotlib.py'),
                                      'beforerr.matplotlib.unify_axis_fontsize': ( 'matplotlib.html#unify_axis_fontsize',
                                                                                   'beforerr/matplotlib.py')},
             'beforerr.polars': { 'beforerr.polars._expand_selectors': ('polars.html#_expand_selectors', 'beforerr/polars.py'),
                                  'beforerr.polars.convert_to_pd_dataframe': ('polars.html#convert_to_pd_dataframe', 'beforerr/polars.py'),
-                                 'beforerr.polars.create_partitions': ('polars.html#create_partitions', 'beforerr/polars.py'),
                                  'beforerr.polars.decompose_vector': ('polars.html#decompose_vector', 'beforerr/polars.py'),
+                                 'beforerr.polars.filter_df_by_ranges': ('polars.html#filter_df_by_ranges', 'beforerr/polars.py'),
+                                 'beforerr.polars.filter_series_by_ranges_i': ( 'polars.html#filter_series_by_ranges_i',
+                                                                                'beforerr/polars.py'),
                                  'beforerr.polars.pl_norm': ('polars.html#pl_norm', 'beforerr/polars.py'),
                                  'beforerr.polars.sort': ('polars.html#sort', 'beforerr/polars.py')},
             'beforerr.project': { 'beforerr.project.datadir': ('projects.html#datadir', 'beforerr/project.py'),
                                   'beforerr.project.increment_backup_num': ('projects.html#increment_backup_num', 'beforerr/project.py'),
                                   'beforerr.project.projectdir': ('projects.html#projectdir', 'beforerr/project.py'),
                                   'beforerr.project.safesave': ('projects.html#safesave', 'beforerr/project.py'),
                                   'beforerr.project.savename': ('projects.html#savename', 'beforerr/project.py'),
```

### Comparing `beforerr-2024.6.1/beforerr/matplotlib.py` & `beforerr-2024.6.2/beforerr/matplotlib.py`

 * *Files identical despite different names*

### Comparing `beforerr-2024.6.1/beforerr/polars.py` & `beforerr-2024.6.2/beforerr/polars.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/10_polars.ipynb.
 
 # %% auto 0
-__all__ = ['create_partitions', 'convert_to_pd_dataframe', 'sort', 'pl_norm', 'decompose_vector']
+__all__ = ['convert_to_pd_dataframe', 'sort', 'pl_norm', 'decompose_vector', 'filter_series_by_ranges_i', 'filter_df_by_ranges']
 
 # %% ../nbs/10_polars.ipynb 2
 import polars as pl
-
 from typing import Any, Collection
 
-from functools import partial
-
-
-# %% ../nbs/10_polars.ipynb 3
-def create_partitions(files, func):
-    keys = [file.split("/")[-1] for file in files]
-    return {key: partial(func, file) for key, file in zip(keys, files)}
-
-# %% ../nbs/10_polars.ipynb 5
+# %% ../nbs/10_polars.ipynb 4
 def convert_to_pd_dataframe(
     df: pl.DataFrame | pl.LazyFrame, # original DataFrame or LazyFrame
 ):
     """
     Convert a Polars DataFrame or LazyFrame into a pandas-like DataFrame.
     """
     if isinstance(df, pl.LazyFrame):
@@ -29,23 +20,23 @@
         raise TypeError("Input must be a Polars DataFrame or LazyFrame")
 
     data = df.to_pandas(use_pyarrow_extension_array=True)
 
     return data
 
 
-# %% ../nbs/10_polars.ipynb 7
+# %% ../nbs/10_polars.ipynb 6
 def sort(df: pl.DataFrame, col="time"):
     if df.get_column(col).is_sorted():
         return df.set_sorted(col)
     else:
         return df.sort(col)
 
 
-# %% ../nbs/10_polars.ipynb 8
+# %% ../nbs/10_polars.ipynb 7
 def _expand_selectors(items: Any, *more_items: Any) -> list[Any]:
     """
     See `_expand_selectors` in `polars`.
     """
     expanded: list[Any] = []
     for item in (
         *(
@@ -54,15 +45,15 @@
             else [items]
         ),
         *more_items,
     ):
         expanded.append(item)
     return expanded
 
-# %% ../nbs/10_polars.ipynb 9
+# %% ../nbs/10_polars.ipynb 8
 def pl_norm(columns, *more_columns) -> pl.Expr:
     """
     Computes the square root of the sum of squares for the given columns.
 
     Args:
     *columns (str): Names of the columns.
 
@@ -70,15 +61,15 @@
     pl.Expr: Expression representing the square root of the sum of squares.
     """
     all_columns = _expand_selectors(columns, *more_columns)
     squares = [pl.col(column).pow(2) for column in all_columns]
 
     return sum(squares).sqrt()
 
-# %% ../nbs/10_polars.ipynb 10
+# %% ../nbs/10_polars.ipynb 9
 def decompose_vector(
     df: pl.DataFrame, vector_col, name=None, suffixes: list = ["_x", "_y", "_z"]
 ):
     """
     Decompose a vector column in a DataFrame into separate columns for each component with custom suffixes.
 
     Parameters:
@@ -107,7 +98,25 @@
     # Create column expressions for each element in the vector
     column_expressions = [
         pl.col(vector_col).list.get(i).alias(name).name.suffix(suffixes[i])
         for i in range(max_length)
     ]
 
     return df.with_columns(column_expressions)
+
+# %% ../nbs/10_polars.ipynb 11
+def filter_series_by_ranges_i(data: pl.Series, starts: list, stops: list):
+    starts_index = data.search_sorted(starts)
+    ends_index = data.search_sorted(stops, side="right")
+
+    return pl.concat(
+        pl.arange(*range, eager=True) for range in zip(starts_index, ends_index)
+    ).unique()
+
+
+def filter_df_by_ranges(data: pl.DataFrame, starts: list, stops: list, col="time"):
+    """
+    Filter a DataFrame from ranges
+    """
+
+    indices_unique = filter_series_by_ranges_i(data[col], starts, stops)
+    return data[indices_unique]
```

### Comparing `beforerr-2024.6.1/beforerr/project.py` & `beforerr-2024.6.2/beforerr/project.py`

 * *Files identical despite different names*

### Comparing `beforerr-2024.6.1/beforerr/r.py` & `beforerr-2024.6.2/beforerr/r.py`

 * *Files identical despite different names*

### Comparing `beforerr-2024.6.1/pyproject.toml` & `beforerr-2024.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 requires-python = ">= 3.10"
 dependencies = [
     "pipe",
     "loguru",
 ]
 readme = "README.md"
-version = "2024.6.1"
+version = "2024.6.2"
 
 [project.optional-dependencies]
 r = [
     "rpy2",
     "rpy2_arrow",
 ]
```

### Comparing `beforerr-2024.6.1/PKG-INFO` & `beforerr-2024.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beforerr
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: Personal Python utility library
 Author-Email: Beforerr <zzj956959688@gmail.com>
 Project-URL: Homepage, https://beforerr.github.io/beforerr_dev
 Project-URL: Repository, https://github.com/beforerr/beforerr_dev
 Requires-Python: >=3.10
 Requires-Dist: pipe
 Requires-Dist: loguru
```

