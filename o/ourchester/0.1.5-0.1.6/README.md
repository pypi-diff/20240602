# Comparing `tmp/ourchester-0.1.5.tar.gz` & `tmp/ourchester-0.1.6.tar.gz`

## Comparing `ourchester-0.1.5.tar` & `ourchester-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ourchester-0.1.5/.bumpversion.cfg
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ourchester-0.1.5/Makefile
--rwxr-xr-x   0        0        0     1736 2020-02-02 00:00:00.000000 ourchester-0.1.5/make_txtar.sh
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ourchester-0.1.5/ourchester.code-workspace
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 ourchester-0.1.5/requirements-dev.lock
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ourchester-0.1.5/requirements.lock
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 ourchester-0.1.5/src/ourchester/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 ourchester-0.1.5/src/ourchester/cli.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 ourchester-0.1.5/src/ourchester/indexer.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ourchester-0.1.5/src/ourchester/log.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ourchester-0.1.5/src/ourchester/searcher.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file1.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file10.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file2.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file3.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file4.md
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file5.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file6.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file7.md
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file8.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ourchester-0.1.5/testdata/file9.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ourchester-0.1.5/.gitignore
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.5/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ourchester-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ourchester-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ourchester-0.1.6/.bumpversion.cfg
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ourchester-0.1.6/Makefile
+-rwxr-xr-x   0        0        0     1736 2020-02-02 00:00:00.000000 ourchester-0.1.6/make_txtar.sh
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ourchester-0.1.6/ourchester.code-workspace
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 ourchester-0.1.6/requirements-dev.lock
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ourchester-0.1.6/requirements.lock
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 ourchester-0.1.6/src/ourchester/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 ourchester-0.1.6/src/ourchester/cli.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 ourchester-0.1.6/src/ourchester/indexer.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ourchester-0.1.6/src/ourchester/log.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ourchester-0.1.6/src/ourchester/searcher.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file1.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file10.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file2.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file3.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file4.md
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file5.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file6.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file7.md
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file8.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ourchester-0.1.6/testdata/file9.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ourchester-0.1.6/.gitignore
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.6/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ourchester-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ourchester-0.1.6/PKG-INFO
```

### Comparing `ourchester-0.1.5/make_txtar.sh` & `ourchester-0.1.6/make_txtar.sh`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.5/requirements-dev.lock` & `ourchester-0.1.6/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.5/requirements.lock` & `ourchester-0.1.6/requirements.lock`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.5/src/ourchester/__init__.py` & `ourchester-0.1.6/src/ourchester/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import sys
 import typing
 
 import fishhoof.find_files
 import platformdirs
 import whoosh.index
 
 from . import cli, indexer, log, searcher
@@ -52,10 +53,10 @@
     user_cache_dir = platformdirs.user_cache_dir()
     ourchester_cache_dir = pathlib.Path(user_cache_dir) / "ourchester"
     ourchester_cache_dir.mkdir(exist_ok=True, parents=True)
     return ourchester_cache_dir
 
 
 def _print_search_results(results):
-    print(f"Found {len(results):,} documents:")
     for hit in results:
         print(f"{hit['path']}")
+    print(f"Found {len(results):,} documents.", file=sys.stderr)
```

### Comparing `ourchester-0.1.5/src/ourchester/cli.py` & `ourchester-0.1.6/src/ourchester/cli.py`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.5/src/ourchester/indexer.py` & `ourchester-0.1.6/src/ourchester/indexer.py`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.5/pyproject.toml` & `ourchester-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ourchester"
-version = "0.1.5"
+version = "0.1.6"
 description = "Add your description here"
 authors = [
     { name = "Taylor Monacelli", email = "taylormonacelli@gmail.com" }
 ]
 dependencies = [
     "jinja2>=3.1.3",
     "whoosh>=2.7.4",
```

### Comparing `ourchester-0.1.5/PKG-INFO` & `ourchester-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ourchester
-Version: 0.1.5
+Version: 0.1.6
 Summary: Add your description here
 Author-email: Taylor Monacelli <taylormonacelli@gmail.com>
 Requires-Python: >=3.12
 Requires-Dist: fishhoof>=0.0.2
 Requires-Dist: humanize>=4.9.0
 Requires-Dist: ivylantern>=0.1.0
 Requires-Dist: jinja2>=3.1.3
```

