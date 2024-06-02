# Comparing `tmp/projen-0.82.2.tar.gz` & `tmp/projen-0.82.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.82.2.tar", last modified: Wed May 29 23:22:23 2024, max compression
+gzip compressed data, was "projen-0.82.3.tar", last modified: Sun Jun  2 12:40:31 2024, max compression
```

## Comparing `projen-0.82.2.tar` & `projen-0.82.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.022223 projen-0.82.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 23:22:12.000000 projen-0.82.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 23:22:12.000000 projen-0.82.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-29 23:22:23.022223 projen-0.82.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-29 23:22:12.000000 projen-0.82.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 23:22:12.000000 projen-0.82.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 23:22:23.022223 projen-0.82.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-29 23:22:12.000000 projen-0.82.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.002223 projen-0.82.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.006223 projen-0.82.2/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   653934 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.006223 projen-0.82.2/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.010223 projen-0.82.2/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2650958 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/_jsii/projen@0.82.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.010223 projen-0.82.2/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   425340 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202836 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.014223 projen-0.82.2/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   847962 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.018223 projen-0.82.2/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-29 23:22:12.000000 projen-0.82.2/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:22:23.006223 projen-0.82.2/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 23:22:22.000000 projen-0.82.2/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.815624 projen-0.82.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 12:40:21.000000 projen-0.82.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 12:40:21.000000 projen-0.82.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-06-02 12:40:31.815624 projen-0.82.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-06-02 12:40:21.000000 projen-0.82.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 12:40:21.000000 projen-0.82.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:40:31.815624 projen-0.82.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-06-02 12:40:21.000000 projen-0.82.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.795624 projen-0.82.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.799624 projen-0.82.3/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   653934 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.799624 projen-0.82.3/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.803624 projen-0.82.3/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2651051 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/_jsii/projen@0.82.3.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.803624 projen-0.82.3/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.803624 projen-0.82.3/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.803624 projen-0.82.3/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.803624 projen-0.82.3/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.807624 projen-0.82.3/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.807624 projen-0.82.3/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.807624 projen-0.82.3/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   425340 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.807624 projen-0.82.3/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.807624 projen-0.82.3/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202836 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.807624 projen-0.82.3/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.807624 projen-0.82.3/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   847962 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.811624 projen-0.82.3/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.811624 projen-0.82.3/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.811624 projen-0.82.3/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.811624 projen-0.82.3/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.811624 projen-0.82.3/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-06-02 12:40:21.000000 projen-0.82.3/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:40:31.799624 projen-0.82.3/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-06-02 12:40:31.000000 projen-0.82.3/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-02 12:40:31.000000 projen-0.82.3/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:40:31.000000 projen-0.82.3/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 12:40:31.000000 projen-0.82.3/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 12:40:31.000000 projen-0.82.3/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.82.2/LICENSE` & `projen-0.82.3/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/PKG-INFO` & `projen-0.82.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.82.2
+Version: 0.82.3
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.82.2/README.md` & `projen-0.82.3/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/setup.py` & `projen-0.82.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.82.2",
+    "version": "0.82.3",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.82.2.jsii.tgz"
+            "projen@0.82.3.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `projen-0.82.2/src/projen/__init__.py` & `projen-0.82.3/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/awscdk/__init__.py` & `projen-0.82.3/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/build/__init__.py` & `projen-0.82.3/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/cdk/__init__.py` & `projen-0.82.3/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/cdk8s/__init__.py` & `projen-0.82.3/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/cdktf/__init__.py` & `projen-0.82.3/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/circleci/__init__.py` & `projen-0.82.3/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/github/__init__.py` & `projen-0.82.3/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/github/workflows/__init__.py` & `projen-0.82.3/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/gitlab/__init__.py` & `projen-0.82.3/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/java/__init__.py` & `projen-0.82.3/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/javascript/__init__.py` & `projen-0.82.3/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/python/__init__.py` & `projen-0.82.3/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/release/__init__.py` & `projen-0.82.3/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/typescript/__init__.py` & `projen-0.82.3/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/vscode/__init__.py` & `projen-0.82.3/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen/web/__init__.py` & `projen-0.82.3/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.82.2/src/projen.egg-info/PKG-INFO` & `projen-0.82.3/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.82.2
+Version: 0.82.3
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.82.2/src/projen.egg-info/SOURCES.txt` & `projen-0.82.3/src/projen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.82.2.jsii.tgz
+src/projen/_jsii/projen@0.82.3.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

