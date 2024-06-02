# Comparing `tmp/demetric-0.1.7.tar.gz` & `tmp/demetric-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demetric-0.1.7.tar", last modified: Sat Jun  1 17:55:56 2024, max compression
+gzip compressed data, was "demetric-0.1.8.tar", last modified: Sun Jun  2 11:00:01 2024, max compression
```

## Comparing `demetric-0.1.7.tar` & `demetric-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1175 2024-06-01 17:55:56.252522 demetric-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      807 2024-06-01 17:55:48.000000 demetric-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      580 2024-06-01 17:55:53.000000 demetric-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-01 17:55:56.252522 demetric-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/src/demetric/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.7/src/demetric/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      127 2024-06-01 17:26:52.000000 demetric-0.1.7/src/demetric/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-06-01 17:46:12.000000 demetric-0.1.7/src/demetric/agg.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1902 2024-06-01 17:39:07.000000 demetric-0.1.7/src/demetric/run.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/src/demetric.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1175 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      294 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.526233 demetric-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1220 2024-06-02 11:00:01.526233 demetric-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      852 2024-06-02 07:53:24.000000 demetric-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      580 2024-06-02 10:59:58.000000 demetric-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-02 11:00:01.526233 demetric-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.516233 demetric-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.526233 demetric-0.1.8/src/demetric/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.8/src/demetric/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      139 2024-06-02 07:51:56.000000 demetric-0.1.8/src/demetric/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-06-01 17:46:12.000000 demetric-0.1.8/src/demetric/agg.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2011 2024-06-02 10:58:56.000000 demetric-0.1.8/src/demetric/metrics.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 11:00:01.526233 demetric-0.1.8/src/demetric.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1220 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      298 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-06-02 11:00:01.000000 demetric-0.1.8/src/demetric.egg-info/top_level.txt
```

### Comparing `demetric-0.1.7/README.md` & `demetric-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 > Dead simple standard for metric logging
 
 ### Logging
 
 ```python
 import demetric as dm
 
-run = dm.Run.new('runs/gpt2-3')
+metrics = dm.Metrics.new('metrics/gpt2-3')
 
-run.log('loss', value=loss, step=step)
-run.log('accuracy', value=acc, step=step)
+metrics.log('loss', value=loss, step=step)
+metrics.log('accuracy', value=acc, step=step)
 # ...
 ```
 
 
 Creates:
 
 ```
@@ -23,21 +23,21 @@
     loss.csv
     accuracy.csv
 ```
 
 ### Statistics
 
 ```python
-# single run
-run = dm.Run('runs/run1.0')
-run.read('loss') # pd.Series
+# single metrics
+metrics = dm.Metrics('metrics/run1.0')
+metrics.read('loss') # pd.Series
 
 # comparing runs
-runs = dm.runs('runs/run1.*')
+runs = dm.runs('metrics/run1.*')
 df = dm.compare(runs, 'loss') # pd.DataFrame with columns ("run1.0", "run1.1", ...)
 
 # concatenating runs (i.e. they're the same experiment but trained by steps or something)
 df = dm.concat(runs, 'loss') # pd.Series with cumulative step indices
 
 # whatever you want to do with the pd.Series's
-ss = dm.readall(runs, 'loss') # list[pd.Series] with `run.id` as each name
+ss = dm.readall(runs, 'loss') # list[pd.Series] with `metrics.id` as each name
 ```
```

### Comparing `demetric-0.1.7/pyproject.toml` & `demetric-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "demetric"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple and composable metric tracking and logging for ML"
 dependencies = [
   "pandas", "lazy-loader", "matplotlib"
 ]
```

### Comparing `demetric-0.1.7/src/demetric/agg.py` & `demetric-0.1.8/src/demetric/agg.py`

 * *Files identical despite different names*

### Comparing `demetric-0.1.7/src/demetric/run.py` & `demetric-0.1.8/src/demetric/metrics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from dataclasses import dataclass
+from collections import deque
 import os
 from glob import glob
 
 @dataclass
-class Run:
+class Metrics:
 
   path: str
 
   @property
   def id(self):
     return os.path.basename(os.path.abspath(self.path))
   
   def __repr__(self) -> str:
-    return f'Run(id="{self.id}", path="{self.path}")'
+    return f'Metrics(id="{self.id}", path="{self.path}")'
 
   @classmethod
   def new(cls, path: str, overwrite: bool = False):
     exists = os.path.exists(path)
     if exists and not overwrite:
-      raise FileExistsError(f'Run already exists at {path}. Use overwrite=True to overwrite it, or Run.append to append to it.')
+      raise FileExistsError(f'Metrics already exists at {path}. Use overwrite=True to overwrite it, or Metrics.append to append to it.')
     elif exists:
       csvs = glob(os.path.join(path, '*.csv'))
       for csv in csvs:
         os.remove(csv)
         
     os.makedirs(path, exist_ok=True)
-    return Run(path)
+    return Metrics(path)
   
   @classmethod
   def append(cls, path: str):
     if not os.path.exists(path):
-      raise FileNotFoundError(f'Run does not exist at {path}')
-    return Run(path)
+      raise FileNotFoundError(f'Metrics does not exist at {path}')
+    return Metrics(path)
 
   def metric_path(self, metric: str):
     return os.path.join(self.path, f'{metric}.csv')
 
   def log(self, metric: str, *, value, step: int):
     """Log a metric `value` at a `step`"""
 
     path = self.metric_path(metric)
 
     if not os.path.exists(path):
+      os.makedirs(self.path, exist_ok=True)
       with open(path, 'w') as f:
         f.write('step,value\n')
     
     with open(path, 'a') as f:
       f.write(f'{step},{value}\n')
 
   def read(self, metric: str):
@@ -62,10 +64,10 @@
       os.path.splitext(os.path.split(f)[-1])[0]
       for f in glob(os.path.join(self.path, '*.csv'))
     ]
 
 def is_run(path: str):
   return os.path.isdir(path) and glob(os.path.join(path, '*.csv')) != []
 
-def runs(glob_: str) -> list[Run]:
-  """Read all runs in a directory"""
-  return [Run(p) for p in glob(glob_) if is_run(p)]
+def runs(glob_: str) -> list[Metrics]:
+  """Read metrics in a directory"""
+  return [Metrics(p) for p in glob(glob_) if is_run(p)]
```

