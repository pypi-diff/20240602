# Comparing `tmp/bussinwebx_get-1.0.3.tar.gz` & `tmp/bussinwebx_get-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bussinwebx_get-1.0.3.tar", last modified: Sun Jun  2 00:26:57 2024, max compression
+gzip compressed data, was "bussinwebx_get-1.0.4.tar", last modified: Sun Jun  2 00:32:03 2024, max compression
```

## Comparing `bussinwebx_get-1.0.3.tar` & `bussinwebx_get-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:26:57.427387 bussinwebx_get-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 00:26:50.000000 bussinwebx_get-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 00:26:57.427387 bussinwebx_get-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 00:26:50.000000 bussinwebx_get-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-02 00:26:50.000000 bussinwebx_get-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:26:57.427387 bussinwebx_get-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:26:57.427387 bussinwebx_get-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:26:57.427387 bussinwebx_get-1.0.3/src/bussinwebx_get.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 00:26:57.000000 bussinwebx_get-1.0.3/src/bussinwebx_get.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-02 00:26:57.000000 bussinwebx_get-1.0.3/src/bussinwebx_get.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:26:57.000000 bussinwebx_get-1.0.3/src/bussinwebx_get.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 00:26:57.000000 bussinwebx_get-1.0.3/src/bussinwebx_get.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:26:57.427387 bussinwebx_get-1.0.3/src/bussinwebx_get_oddcell/
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-06-02 00:26:50.000000 bussinwebx_get-1.0.3/src/bussinwebx_get_oddcell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:32:03.803637 bussinwebx_get-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 00:31:56.000000 bussinwebx_get-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 00:32:03.803637 bussinwebx_get-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 00:31:56.000000 bussinwebx_get-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-02 00:31:56.000000 bussinwebx_get-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:32:03.803637 bussinwebx_get-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:32:03.799637 bussinwebx_get-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:32:03.803637 bussinwebx_get-1.0.4/src/bussinwebx_get.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 00:32:03.000000 bussinwebx_get-1.0.4/src/bussinwebx_get.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-02 00:32:03.000000 bussinwebx_get-1.0.4/src/bussinwebx_get.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:32:03.000000 bussinwebx_get-1.0.4/src/bussinwebx_get.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 00:32:03.000000 bussinwebx_get-1.0.4/src/bussinwebx_get.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:32:03.803637 bussinwebx_get-1.0.4/src/bussinwebx_get_oddcell/
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-06-02 00:31:56.000000 bussinwebx_get-1.0.4/src/bussinwebx_get_oddcell/__init__.py
```

### Comparing `bussinwebx_get-1.0.3/LICENSE` & `bussinwebx_get-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bussinwebx_get-1.0.3/PKG-INFO` & `bussinwebx_get-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bussinwebx-get
-Version: 1.0.3
+Name: bussinwebx_get
+Version: 1.0.4
 Summary: Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 Maintainer: The Odd Cell
 License: MIT License
 Project-URL: Repository, https://github.com/TheOddCell/bussinwebx-get.git
 Project-URL: Issues, https://github.com/TheOddCell/bussinwebx-get/issues
 Keywords: webx,buss,facedev
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bussinwebx_get-1.0.3/pyproject.toml` & `bussinwebx_get-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-version="1.0.3"
-name = "bussinwebx-get"
+version="1.0.4"
+name = "bussinwebx_get"
 requires-python = ">= 3.8"
 maintainers = [
   {name = "The Odd Cell"}
 ]
 description = "Be able to make GET requests to buss:// websites and get IPs for buss:// websites."
 readme = "README.md"
 license = {text = "MIT License"}
```

### Comparing `bussinwebx_get-1.0.3/src/bussinwebx_get.egg-info/PKG-INFO` & `bussinwebx_get-1.0.4/src/bussinwebx_get.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bussinwebx-get
-Version: 1.0.3
+Name: bussinwebx_get
+Version: 1.0.4
 Summary: Be able to make GET requests to buss:// websites and get IPs for buss:// websites.
 Maintainer: The Odd Cell
 License: MIT License
 Project-URL: Repository, https://github.com/TheOddCell/bussinwebx-get.git
 Project-URL: Issues, https://github.com/TheOddCell/bussinwebx-get/issues
 Keywords: webx,buss,facedev
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bussinwebx_get-1.0.3/src/bussinwebx_get_oddcell/__init__.py` & `bussinwebx_get-1.0.4/src/bussinwebx_get_oddcell/__init__.py`

 * *Files identical despite different names*

