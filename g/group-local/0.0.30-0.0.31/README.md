# Comparing `tmp/group_local-0.0.30.tar.gz` & `tmp/group_local-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.30.tar", last modified: Sun May 26 17:51:12 2024, max compression
+gzip compressed data, was "group_local-0.0.31.tar", last modified: Sun Jun  2 09:39:32 2024, max compression
```

## Comparing `group_local-0.0.30.tar` & `group_local-0.0.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:12.859826 group_local-0.0.30/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-26 17:51:12.859826 group_local-0.0.30/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:12.855826 group_local-0.0.30/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:12.859826 group_local-0.0.30/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 17:50:54.000000 group_local-0.0.30/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-26 17:50:54.000000 group_local-0.0.30/group_local/src/group_local_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    19817 2024-05-26 17:50:54.000000 group_local-0.0.30/group_local/src/groups_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:12.859826 group_local-0.0.30/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-26 17:51:12.000000 group_local-0.0.30/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-26 17:51:12.000000 group_local-0.0.30/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 17:51:12.000000 group_local-0.0.30/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-26 17:51:12.000000 group_local-0.0.30/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 17:51:12.000000 group_local-0.0.30/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-26 17:50:59.000000 group_local-0.0.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 17:51:12.859826 group_local-0.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-26 17:50:54.000000 group_local-0.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:39:32.006318 group_local-0.0.31/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-02 09:39:32.006318 group_local-0.0.31/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:39:32.006318 group_local-0.0.31/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:39:32.006318 group_local-0.0.31/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:39:12.000000 group_local-0.0.31/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-02 09:39:12.000000 group_local-0.0.31/group_local/src/group_local_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19817 2024-06-02 09:39:12.000000 group_local-0.0.31/group_local/src/groups_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:39:32.006318 group_local-0.0.31/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-02 09:39:31.000000 group_local-0.0.31/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-02 09:39:32.000000 group_local-0.0.31/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:39:31.000000 group_local-0.0.31/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-02 09:39:31.000000 group_local-0.0.31/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 09:39:31.000000 group_local-0.0.31/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-02 09:39:18.000000 group_local-0.0.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:39:32.006318 group_local-0.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-06-02 09:39:12.000000 group_local-0.0.31/setup.py
```

### Comparing `group_local-0.0.30/PKG-INFO` & `group_local-0.0.31/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.30
+Version: 0.0.31
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.30/group_local/src/group_local_constants.py` & `group_local-0.0.31/group_local/src/group_local_constants.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.30/group_local/src/groups_local.py` & `group_local-0.0.31/group_local/src/groups_local.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.30/group_local.egg-info/PKG-INFO` & `group_local-0.0.31/group_local.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.30
+Version: 0.0.31
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `group_local-0.0.30/setup.py` & `group_local-0.0.31/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/group-local
-    version='0.0.30',
+    version='0.0.31',
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles group-local Python",
     long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
```

