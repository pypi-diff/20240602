# Comparing `tmp/checkptr-0.1.0.tar.gz` & `tmp/checkptr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkptr-0.1.0.tar", last modified: Sun Jun  2 05:47:54 2024, max compression
+gzip compressed data, was "checkptr-0.1.1.tar", last modified: Sun Jun  2 19:08:36 2024, max compression
```

## Comparing `checkptr-0.1.0.tar` & `checkptr-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 05:47:54.067367 checkptr-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-06-02 05:47:54.067367 checkptr-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-06-02 05:44:17.000000 checkptr-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      546 2024-06-02 05:35:32.000000 checkptr-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-02 05:47:54.067367 checkptr-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 05:47:54.057367 checkptr-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 05:47:54.067367 checkptr-0.1.0/src/checkptr/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-06-02 05:45:09.000000 checkptr-0.1.0/src/checkptr/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      741 2024-06-02 05:46:39.000000 checkptr-0.1.0/src/checkptr/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 05:47:54.067367 checkptr-0.1.0/src/checkptr.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-06-02 05:47:54.000000 checkptr-0.1.0/src/checkptr.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      214 2024-06-02 05:47:54.000000 checkptr-0.1.0/src/checkptr.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-02 05:47:54.000000 checkptr-0.1.0/src/checkptr.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-06-02 05:47:54.000000 checkptr-0.1.0/src/checkptr.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 19:08:36.179258 checkptr-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-06-02 19:08:36.179258 checkptr-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      543 2024-06-02 05:44:17.000000 checkptr-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      546 2024-06-02 19:08:33.000000 checkptr-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-02 19:08:36.179258 checkptr-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 19:08:36.169258 checkptr-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 19:08:36.169258 checkptr-0.1.1/src/checkptr/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-06-02 05:45:09.000000 checkptr-0.1.1/src/checkptr/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1341 2024-06-02 19:08:31.000000 checkptr-0.1.1/src/checkptr/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-02 19:08:36.179258 checkptr-0.1.1/src/checkptr.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-06-02 19:08:36.000000 checkptr-0.1.1/src/checkptr.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      214 2024-06-02 19:08:36.000000 checkptr-0.1.1/src/checkptr.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-02 19:08:36.000000 checkptr-0.1.1/src/checkptr.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-06-02 19:08:36.000000 checkptr-0.1.1/src/checkptr.egg-info/top_level.txt
```

### Comparing `checkptr-0.1.0/PKG-INFO` & `checkptr-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkptr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple standard for model checkpointing, framework-agnostic
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Checkptr
```

### Comparing `checkptr-0.1.0/README.md` & `checkptr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `checkptr-0.1.0/pyproject.toml` & `checkptr-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "checkptr"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple standard for model checkpointing, framework-agnostic"
 dependencies = [
   
 ]
```

### Comparing `checkptr-0.1.0/src/checkptr.egg-info/PKG-INFO` & `checkptr-0.1.1/src/checkptr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkptr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple standard for model checkpointing, framework-agnostic
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Checkptr
```

