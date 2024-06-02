# Comparing `tmp/lines_dataset-0.2.0.tar.gz` & `tmp/lines_dataset-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lines_dataset-0.2.0.tar", last modified: Sat Jun  1 13:22:38 2024, max compression
+gzip compressed data, was "lines_dataset-0.2.1.tar", last modified: Sun Jun  2 07:32:03 2024, max compression
```

## Comparing `lines_dataset-0.2.0.tar` & `lines_dataset-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1242 2024-06-01 13:08:31.000000 lines_dataset-0.2.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      588 2024-06-01 13:22:29.000000 lines_dataset-0.2.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.960638 lines_dataset-0.2.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.960638 lines_dataset-0.2.0/src/lines_dataset/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      218 2024-06-01 12:32:30.000000 lines_dataset-0.2.0/src/lines_dataset/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.2.0/src/lines_dataset/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-31 11:33:08.000000 lines_dataset-0.2.0/src/lines_dataset/compression.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1926 2024-06-01 13:10:44.000000 lines_dataset-0.2.0/src/lines_dataset/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      277 2024-06-01 12:58:18.000000 lines_dataset-0.2.0/src/lines_dataset/meta.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/src/lines_dataset.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       20 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 07:32:03.427369 lines_dataset-0.2.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1812 2024-06-02 07:32:03.427369 lines_dataset-0.2.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1448 2024-06-02 05:57:24.000000 lines_dataset-0.2.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      588 2024-06-02 07:31:56.000000 lines_dataset-0.2.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-02 07:32:03.427369 lines_dataset-0.2.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 07:32:03.407369 lines_dataset-0.2.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 07:32:03.427369 lines_dataset-0.2.1/src/lines_dataset/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      218 2024-06-01 12:32:30.000000 lines_dataset-0.2.1/src/lines_dataset/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-06-02 05:59:45.000000 lines_dataset-0.2.1/src/lines_dataset/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-31 11:33:08.000000 lines_dataset-0.2.1/src/lines_dataset/compression.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2553 2024-06-02 07:29:59.000000 lines_dataset-0.2.1/src/lines_dataset/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      247 2024-06-02 07:31:53.000000 lines_dataset-0.2.1/src/lines_dataset/meta.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 07:32:03.427369 lines_dataset-0.2.1/src/lines_dataset.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1812 2024-06-02 07:32:03.000000 lines_dataset-0.2.1/src/lines_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-06-02 07:32:03.000000 lines_dataset-0.2.1/src/lines_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-02 07:32:03.000000 lines_dataset-0.2.1/src/lines_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       20 2024-06-02 07:32:03.000000 lines_dataset-0.2.1/src/lines_dataset.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-06-02 07:32:03.000000 lines_dataset-0.2.1/src/lines_dataset.egg-info/top_level.txt
```

### Comparing `lines_dataset-0.2.0/PKG-INFO` & `lines_dataset-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lines-dataset
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple tools for storing inputs + labels datasets as one sample per line
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: haskellian
@@ -49,19 +49,31 @@
       "samples": 2000 // not all files need to have the same number of lines, as long as samples match line by line. The shortest file will determine the length of the dataset.
     },
   },
   // you can add other stuff if you want to
 }
 ```
 
+### Usage
+
 ```python
 import lines_dataset as lds
 
 ds = lds.Dataset.read('path/to/my-dataset')
 num_samples = ds.len('inputs', 'labels') # int | None
 
 for x in ds.samples('inputs', 'labels'):
   x['inputs'] # "the first line of inputs.txt\n"
   x['labels'] # "the decompressed first line of labels.txt.zst\n"
 ```
 
+A common convenience to use is:
+
+```python
+import lines_dataset as lds
+
+datasets = lds.glob('path/to/datasets/*') # list[lds.Dataset]
+for x in lds.chain(datasets, 'inputs', 'labels'):
+  ...
+```
+
 And that's it! Simple.
```

### Comparing `lines_dataset-0.2.0/pyproject.toml` & `lines_dataset-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lines-dataset"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple tools for storing inputs + labels datasets as one sample per line"
 dependencies = [
   "pydantic", "haskellian"
 ]
```

### Comparing `lines_dataset-0.2.0/src/lines_dataset/dataset.py` & `lines_dataset-0.2.1/src/lines_dataset/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing_extensions import Iterable, Mapping, TypeVar, LiteralString
+from typing_extensions import Iterable, Mapping, TypeVar, LiteralString, TextIO
 from dataclasses import dataclass
 import os
 from haskellian import Iter, iter as I, dicts as D
 from .meta import Meta
 
 K = TypeVar('K', bound=LiteralString)
 
@@ -54,8 +54,25 @@
     lens = [self._len(k) for k in keys]
     if None in lens:
       return None
     return min(lens) # type: ignore
 
   def _len(self, key: str) -> int | None:
     file = self.file(key)
-    return file and file.num_lines
+    return file and file.num_lines
+  
+
+def glob(glob: str, *, recursive: bool = False, err_stream: TextIO | None = None) -> list[Dataset]:
+  """Read all datasets that match a glob pattern."""
+  from glob import glob as _glob
+  datasets = []
+  for p in _glob(glob, recursive=recursive):
+    try:
+      datasets.append(Dataset.read(p))
+    except Exception as e:
+      if err_stream:
+        print(f'Error reading dataset at {p}:', e, file=err_stream)
+  return datasets
+
+def chain(datasets: Iterable[Dataset], *keys: K) -> Iter[Mapping[K, str]]:
+  """Chain multiple datasets into a single one."""
+  return I.flatten([ds.samples(*keys) for ds in datasets])
```

### Comparing `lines_dataset-0.2.0/src/lines_dataset.egg-info/PKG-INFO` & `lines_dataset-0.2.1/src/lines_dataset.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lines-dataset
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple tools for storing inputs + labels datasets as one sample per line
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: haskellian
@@ -49,19 +49,31 @@
       "samples": 2000 // not all files need to have the same number of lines, as long as samples match line by line. The shortest file will determine the length of the dataset.
     },
   },
   // you can add other stuff if you want to
 }
 ```
 
+### Usage
+
 ```python
 import lines_dataset as lds
 
 ds = lds.Dataset.read('path/to/my-dataset')
 num_samples = ds.len('inputs', 'labels') # int | None
 
 for x in ds.samples('inputs', 'labels'):
   x['inputs'] # "the first line of inputs.txt\n"
   x['labels'] # "the decompressed first line of labels.txt.zst\n"
 ```
 
+A common convenience to use is:
+
+```python
+import lines_dataset as lds
+
+datasets = lds.glob('path/to/datasets/*') # list[lds.Dataset]
+for x in lds.chain(datasets, 'inputs', 'labels'):
+  ...
+```
+
 And that's it! Simple.
```

