# Comparing `tmp/image_input_handler-0.2.5.tar.gz` & `tmp/image_input_handler-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_input_handler-0.2.5.tar", last modified: Mon May 13 09:09:37 2024, max compression
+gzip compressed data, was "image_input_handler-0.4.0.tar", last modified: Sun Jun  2 09:18:59 2024, max compression
```

## Comparing `image_input_handler-0.2.5.tar` & `image_input_handler-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:09:37.012899 image_input_handler-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-13 09:09:37.012899 image_input_handler-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-13 09:09:30.000000 image_input_handler-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:09:37.008899 image_input_handler-0.2.5/image_input_handler/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 09:09:30.000000 image_input_handler-0.2.5/image_input_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-05-13 09:09:30.000000 image_input_handler-0.2.5/image_input_handler/image_input_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:09:37.012899 image_input_handler-0.2.5/image_input_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-13 09:09:37.000000 image_input_handler-0.2.5/image_input_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 09:09:37.000000 image_input_handler-0.2.5/image_input_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:09:37.000000 image_input_handler-0.2.5/image_input_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 09:09:37.000000 image_input_handler-0.2.5/image_input_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 09:09:37.000000 image_input_handler-0.2.5/image_input_handler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:09:37.012899 image_input_handler-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-13 09:09:30.000000 image_input_handler-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:18:59.787632 image_input_handler-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-06-02 09:18:59.787632 image_input_handler-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-06-02 09:18:56.000000 image_input_handler-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:18:59.787632 image_input_handler-0.4.0/image_input_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 09:18:56.000000 image_input_handler-0.4.0/image_input_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-06-02 09:18:56.000000 image_input_handler-0.4.0/image_input_handler/image_input_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:18:59.787632 image_input_handler-0.4.0/image_input_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-06-02 09:18:59.000000 image_input_handler-0.4.0/image_input_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-02 09:18:59.000000 image_input_handler-0.4.0/image_input_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:18:59.000000 image_input_handler-0.4.0/image_input_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-02 09:18:59.000000 image_input_handler-0.4.0/image_input_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 09:18:59.000000 image_input_handler-0.4.0/image_input_handler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:18:59.787632 image_input_handler-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-06-02 09:18:56.000000 image_input_handler-0.4.0/setup.py
```

### Comparing `image_input_handler-0.2.5/PKG-INFO` & `image_input_handler-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_input_handler
-Version: 0.2.5
+Version: 0.4.0
 Summary: A module to handle different formats of image input
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `image_input_handler-0.2.5/README.md` & `image_input_handler-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `image_input_handler-0.2.5/image_input_handler.egg-info/PKG-INFO` & `image_input_handler-0.4.0/image_input_handler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_input_handler
-Version: 0.2.5
+Version: 0.4.0
 Summary: A module to handle different formats of image input
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `image_input_handler-0.2.5/setup.py` & `image_input_handler-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import setuptools
 import subprocess
 import os
 
 setup(
     name='image_input_handler',  # Package name
-    version='0.2.5',  # Version of your package
+    version='0.4.0',  # Version of your package
     author='Enes Kuzucu',  # Your name
 
     description='A module to handle different formats of image input',  # Short description
     long_description=open('README.md').read(),  # Long description from a README file
     long_description_content_type='text/markdown',  # Type of the long description
 #     url='https://github.com/karaposu/image-input-handler',  # URL to the repository
     packages=find_packages(),  # Automatically find packages in the directory
```

