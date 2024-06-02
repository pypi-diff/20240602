# Comparing `tmp/demetric-0.1.8.tar.gz` & `tmp/demetric-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demetric-0.1.8.tar", last modified: Sun Jun  2 11:00:01 2024, max compression
+gzip compressed data, was "demetric-0.1.9.tar", last modified: Sun Jun  2 17:25:47 2024, max compression
```

## Comparing `demetric-0.1.8.tar` & `demetric-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.526233 demetric-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1220 2024-06-02 11:00:01.526233 demetric-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      852 2024-06-02 07:53:24.000000 demetric-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      580 2024-06-02 10:59:58.000000 demetric-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-02 11:00:01.526233 demetric-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.516233 demetric-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.526233 demetric-0.1.8/src/demetric/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.8/src/demetric/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      139 2024-06-02 07:51:56.000000 demetric-0.1.8/src/demetric/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-06-01 17:46:12.000000 demetric-0.1.8/src/demetric/agg.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2011 2024-06-02 10:58:56.000000 demetric-0.1.8/src/demetric/metrics.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.526233 demetric-0.1.8/src/demetric.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1220 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      298 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 17:25:47.139248 demetric-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1220 2024-06-02 17:25:47.139248 demetric-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      852 2024-06-02 07:53:24.000000 demetric-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      580 2024-06-02 17:25:44.000000 demetric-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-02 17:25:47.139248 demetric-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 17:25:47.129248 demetric-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 17:25:47.139248 demetric-0.1.9/src/demetric/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.9/src/demetric/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      139 2024-06-02 07:51:56.000000 demetric-0.1.9/src/demetric/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      913 2024-06-02 13:57:39.000000 demetric-0.1.9/src/demetric/agg.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2017 2024-06-02 13:59:47.000000 demetric-0.1.9/src/demetric/metrics.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 17:25:47.139248 demetric-0.1.9/src/demetric.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1220 2024-06-02 17:25:47.000000 demetric-0.1.9/src/demetric.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      298 2024-06-02 17:25:47.000000 demetric-0.1.9/src/demetric.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-02 17:25:47.000000 demetric-0.1.9/src/demetric.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-06-02 17:25:47.000000 demetric-0.1.9/src/demetric.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-06-02 17:25:47.000000 demetric-0.1.9/src/demetric.egg-info/top_level.txt
```

### Comparing `demetric-0.1.8/PKG-INFO` & `demetric-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demetric
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple and composable metric tracking and logging for ML
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: lazy-loader
```

### Comparing `demetric-0.1.8/README.md` & `demetric-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `demetric-0.1.8/pyproject.toml` & `demetric-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "demetric"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple and composable metric tracking and logging for ML"
 dependencies = [
   "pandas", "lazy-loader", "matplotlib"
 ]
```

### Comparing `demetric-0.1.8/src/demetric/agg.py` & `demetric-0.1.9/src/demetric/agg.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-from typing import Sequence
+from typing import Mapping, Iterable
 import pandas as pd
-from . import Run
+from . import Metrics
 
-def readall(runs: Sequence[Run], metric: str) -> list[pd.Series]:
-  """Read all runs' dataframes for a metric"""
-  return [s.rename(run.id) for run in runs if (s := run.read(metric)) is not None]
-
-def adj_concat(series: Sequence[pd.Series], copy: bool = False) -> pd.Series:
+def adj_concat(dfs: Iterable[pd.DataFrame], copy: bool = False) -> pd.Series:
   """Concatenate series with cumulative index"""
   cum_idx = 0
-  adj_series = []
+  adj_dfs = []
 
-  for s in series:
-    last_idx = s.index[-1]
-    adj_s = s.copy() if copy else s
-    adj_s.index = adj_s.index + cum_idx
-    cum_idx += last_idx + 1 # type: ignore
-    adj_series.append(adj_s)
+  for df in dfs:
+    last_idx = df.index[-1]
+    adj_df = df.copy() if copy else df
+    adj_df.index = adj_df.index + cum_idx
+    cum_idx += last_idx + 1
+    adj_dfs.append(adj_df)
 
-  return pd.concat(adj_series) # type: ignore
+  return pd.concat(adj_dfs)
 
-def compare(runs: Sequence[Run], metric: str):
+def compare(runs: Mapping[str, Metrics], metric: str):
   """Concat runs' dataframes by column, prepending the run's id to the column names"""
-  series = readall(runs, metric)
-  return pd.concat(series, axis=1)
+  dfs = { id: df for id, run in runs.items() if (df := run.read(metric)) is not None }
+  return pd.concat(dfs, axis=1)
 
-def concat(runs: Sequence[Run], metric: str):
+def concat(runs: Iterable[Metrics], metric: str):
   """Concat runs' dataframes by row, adjusting the index"""
-  dfs = readall(runs, metric)
+  dfs = [df for run in runs if (df := run.read(metric)) is not None]
   return adj_concat(dfs)
```

### Comparing `demetric-0.1.8/src/demetric/metrics.py` & `demetric-0.1.9/src/demetric/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from dataclasses import dataclass
-from collections import deque
 import os
 from glob import glob
 
 @dataclass
 class Metrics:
 
   path: str
 
-  @property
-  def id(self):
-    return os.path.basename(os.path.abspath(self.path))
-  
   def __repr__(self) -> str:
-    return f'Metrics(id="{self.id}", path="{self.path}")'
+    return f'Metrics(path="{self.path}")'
 
   @classmethod
   def new(cls, path: str, overwrite: bool = False):
     exists = os.path.exists(path)
     if exists and not overwrite:
       raise FileExistsError(f'Metrics already exists at {path}. Use overwrite=True to overwrite it, or Metrics.append to append to it.')
     elif exists:
@@ -41,33 +36,36 @@
     """Log a metric `value` at a `step`"""
 
     path = self.metric_path(metric)
 
     if not os.path.exists(path):
       os.makedirs(self.path, exist_ok=True)
       with open(path, 'w') as f:
-        f.write('step,value\n')
+        f.write(f'step,{metric}\n')
     
     with open(path, 'a') as f:
       f.write(f'{step},{value}\n')
 
   def read(self, metric: str):
     """Read `pd.DataFrame` for `metric`"""
     import pandas as pd
     try:
-      return pd.read_csv(self.metric_path(metric), index_col='step')['value']
+      return pd.read_csv(self.metric_path(metric), index_col='step')
     except FileNotFoundError:
       ...
 
+  def read_all(self):
+    return { metric: self.read(metric) for metric in self.metrics() }
+
   def metrics(self) -> list[str]:
     """List all metrics"""
     return [
       os.path.splitext(os.path.split(f)[-1])[0]
       for f in glob(os.path.join(self.path, '*.csv'))
     ]
 
 def is_run(path: str):
   return os.path.isdir(path) and glob(os.path.join(path, '*.csv')) != []
 
-def runs(glob_: str) -> list[Metrics]:
-  """Read metrics in a directory"""
-  return [Metrics(p) for p in glob(glob_) if is_run(p)]
+def runs(glob_: str, recursive: bool = False) -> list[Metrics]:
+  """Find runs metrics in a directory"""
+  return [Metrics(p) for p in glob(glob_, recursive=recursive) if is_run(p)]
```

### Comparing `demetric-0.1.8/src/demetric.egg-info/PKG-INFO` & `demetric-0.1.9/src/demetric.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demetric
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple and composable metric tracking and logging for ML
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: lazy-loader
```

