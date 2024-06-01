# Comparing `tmp/bussinwebx_get-1.0.0.tar.gz` & `tmp/bussinwebx_get-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bussinwebx_get-1.0.0.tar", last modified: Sat Jun  1 22:46:23 2024, max compression
+gzip compressed data, was "bussinwebx_get-1.0.1.tar", last modified: Sat Jun  1 23:06:08 2024, max compression
```

## Comparing `bussinwebx_get-1.0.0.tar` & `bussinwebx_get-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:46:23.158884 bussinwebx_get-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-01 22:46:19.000000 bussinwebx_get-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-06-01 22:46:23.158884 bussinwebx_get-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-01 22:46:19.000000 bussinwebx_get-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-06-01 22:46:19.000000 bussinwebx_get-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:46:23.158884 bussinwebx_get-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:46:23.158884 bussinwebx_get-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:46:23.158884 bussinwebx_get-1.0.0/src/bussinwebx-get_oddcell/
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-06-01 22:46:19.000000 bussinwebx_get-1.0.0/src/bussinwebx-get_oddcell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:46:23.158884 bussinwebx_get-1.0.0/src/bussinwebx_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-06-01 22:46:23.000000 bussinwebx_get-1.0.0/src/bussinwebx_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-06-01 22:46:23.000000 bussinwebx_get-1.0.0/src/bussinwebx_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:46:23.000000 bussinwebx_get-1.0.0/src/bussinwebx_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 22:46:23.000000 bussinwebx_get-1.0.0/src/bussinwebx_get.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-01 22:46:23.000000 bussinwebx_get-1.0.0/src/bussinwebx_get.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:06:08.729186 bussinwebx_get-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-01 23:06:04.000000 bussinwebx_get-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-01 23:06:08.729186 bussinwebx_get-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-01 23:06:04.000000 bussinwebx_get-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-01 23:06:04.000000 bussinwebx_get-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:06:08.729186 bussinwebx_get-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:06:08.729186 bussinwebx_get-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:06:08.729186 bussinwebx_get-1.0.1/src/bussinwebx-get_oddcell/
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-06-01 23:06:04.000000 bussinwebx_get-1.0.1/src/bussinwebx-get_oddcell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:06:08.729186 bussinwebx_get-1.0.1/src/bussinwebx_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-01 23:06:08.000000 bussinwebx_get-1.0.1/src/bussinwebx_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 23:06:08.000000 bussinwebx_get-1.0.1/src/bussinwebx_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 23:06:08.000000 bussinwebx_get-1.0.1/src/bussinwebx_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-01 23:06:08.000000 bussinwebx_get-1.0.1/src/bussinwebx_get.egg-info/top_level.txt
```

### Comparing `bussinwebx_get-1.0.0/LICENSE` & `bussinwebx_get-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bussinwebx_get-1.0.0/PKG-INFO` & `bussinwebx_get-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bussinwebx-get
-Version: 1.0.0
+Version: 1.0.1
 Summary: Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 Maintainer: The Odd Cell
 License: MIT License
 Project-URL: Repository, https://github.com/TheOddCell/bussinwebx-get.git
 Project-URL: Issues, https://github.com/TheOddCell/bussinwebx-get/issues
 Keywords: webx,buss,facedev
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: json
 
 # bussinwebx-get
 Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
+
+[What is Bussin Web X (buss://)?](https://github.com/face-hh/webx)
```

### Comparing `bussinwebx_get-1.0.0/pyproject.toml` & `bussinwebx_get-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 [project]
-version = "1.0.0"
+version = "1.0.1"
 name = "bussinwebx-get"
-dependencies = [
-  "requests",
-  "json"
-]
 requires-python = ">= 3.8"
 maintainers = [
   {name = "The Odd Cell"}
 ]
 description = "Be able to make GET requests to buss:// websites and get IPs for buss:// websites."
 readme = "README.md"
 license = {text = "MIT License"}
```

### Comparing `bussinwebx_get-1.0.0/src/bussinwebx-get_oddcell/__init__.py` & `bussinwebx_get-1.0.1/src/bussinwebx-get_oddcell/__init__.py`

 * *Files identical despite different names*

### Comparing `bussinwebx_get-1.0.0/src/bussinwebx_get.egg-info/PKG-INFO` & `bussinwebx_get-1.0.1/src/bussinwebx_get.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bussinwebx-get
-Version: 1.0.0
+Version: 1.0.1
 Summary: Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 Maintainer: The Odd Cell
 License: MIT License
 Project-URL: Repository, https://github.com/TheOddCell/bussinwebx-get.git
 Project-URL: Issues, https://github.com/TheOddCell/bussinwebx-get/issues
 Keywords: webx,buss,facedev
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: json
 
 # bussinwebx-get
 Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
+
+[What is Bussin Web X (buss://)?](https://github.com/face-hh/webx)
```
