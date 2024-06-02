# Comparing `tmp/gammarers.aws-secure-vpc-bucket-1.4.0.tar.gz` & `tmp/gammarers.aws-secure-vpc-bucket-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-secure-vpc-bucket-1.4.0.tar", last modified: Mon May 27 03:57:49 2024, max compression
+gzip compressed data, was "gammarers.aws-secure-vpc-bucket-1.4.1.tar", last modified: Sun Jun  2 18:24:18 2024, max compression
```

## Comparing `gammarers.aws-secure-vpc-bucket-1.4.0.tar` & `gammarers.aws-secure-vpc-bucket-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:57:49.589686 gammarers.aws-secure-vpc-bucket-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-27 03:57:49.589686 gammarers.aws-secure-vpc-bucket-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 03:57:49.589686 gammarers.aws-secure-vpc-bucket-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:57:49.585687 gammarers.aws-secure-vpc-bucket-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:57:49.585687 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:57:49.589686 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:57:49.589686 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29739 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@1.4.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 03:57:36.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:57:49.585687 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-27 03:57:49.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-27 03:57:49.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 03:57:49.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-27 03:57:49.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 03:57:49.000000 gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:18.317492 gammarers.aws-secure-vpc-bucket-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-06-02 18:24:18.317492 gammarers.aws-secure-vpc-bucket-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:24:18.317492 gammarers.aws-secure-vpc-bucket-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:18.313492 gammarers.aws-secure-vpc-bucket-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:18.317492 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:18.317492 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:18.317492 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29757 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@1.4.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:24:08.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:24:18.317492 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-06-02 18:24:18.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 18:24:18.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:24:18.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-02 18:24:18.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 18:24:18.000000 gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/top_level.txt
```

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/LICENSE` & `gammarers.aws-secure-vpc-bucket-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/PKG-INFO` & `gammarers.aws-secure-vpc-bucket-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-vpc-bucket
-Version: 1.4.0
+Version: 1.4.1
 Summary: Access from specific VPC Endpoint only Bucket
 Home-page: https://github.com/gammarers/aws-secure-vpc-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-vpc-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/README.md` & `gammarers.aws-secure-vpc-bucket-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/setup.py` & `gammarers.aws-secure-vpc-bucket-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-secure-vpc-bucket",
-    "version": "1.4.0",
+    "version": "1.4.1",
     "description": "Access from specific VPC Endpoint only Bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-secure-vpc-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_secure_vpc_bucket",
         "gammarers.aws_secure_vpc_bucket._jsii"
     ],
     "package_data": {
         "gammarers.aws_secure_vpc_bucket._jsii": [
-            "aws-secure-vpc-bucket@1.4.0.jsii.tgz"
+            "aws-secure-vpc-bucket@1.4.1.jsii.tgz"
         ],
         "gammarers.aws_secure_vpc_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/__init__.py` & `gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers/aws_secure_vpc_bucket/_jsii/__init__.py` & `gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers/aws_secure_vpc_bucket/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-secure-vpc-bucket",
-    "1.4.0",
+    "1.4.1",
     __name__[0:-6],
-    "aws-secure-vpc-bucket@1.4.0.jsii.tgz",
+    "aws-secure-vpc-bucket@1.4.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/PKG-INFO` & `gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-vpc-bucket
-Version: 1.4.0
+Version: 1.4.1
 Summary: Access from specific VPC Endpoint only Bucket
 Home-page: https://github.com/gammarers/aws-secure-vpc-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-vpc-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-vpc-bucket-1.4.0/src/gammarers.aws_secure_vpc_bucket.egg-info/SOURCES.txt` & `gammarers.aws-secure-vpc-bucket-1.4.1/src/gammarers.aws_secure_vpc_bucket.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_secure_vpc_bucket.egg-info/SOURCES.txt
 src/gammarers.aws_secure_vpc_bucket.egg-info/dependency_links.txt
 src/gammarers.aws_secure_vpc_bucket.egg-info/requires.txt
 src/gammarers.aws_secure_vpc_bucket.egg-info/top_level.txt
 src/gammarers/aws_secure_vpc_bucket/__init__.py
 src/gammarers/aws_secure_vpc_bucket/py.typed
 src/gammarers/aws_secure_vpc_bucket/_jsii/__init__.py
-src/gammarers/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@1.4.0.jsii.tgz
+src/gammarers/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@1.4.1.jsii.tgz
```
