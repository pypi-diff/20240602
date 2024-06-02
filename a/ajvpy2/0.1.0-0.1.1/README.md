# Comparing `tmp/ajvpy2-0.1.0.tar.gz` & `tmp/ajvpy2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ajvpy2-0.1.0.tar", last modified: Sat Jun  1 21:55:41 2024, max compression
+gzip compressed data, was "ajvpy2-0.1.1.tar", last modified: Sun Jun  2 03:05:36 2024, max compression
```

## Comparing `ajvpy2-0.1.0.tar` & `ajvpy2-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2024-06-01 21:55:41.630909 ajvpy2-0.1.0/
--rw-r--r--   0 anthony    (501) staff       (20)     1073 2024-06-01 19:59:05.000000 ajvpy2-0.1.0/LICENSE
--rw-r--r--   0 anthony    (501) staff       (20)     2092 2024-06-01 21:55:41.630740 ajvpy2-0.1.0/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)     1518 2024-06-01 21:27:16.000000 ajvpy2-0.1.0/README.md
-drwxr-xr-x   0 anthony    (501) staff       (20)        0 2024-06-01 21:55:41.630462 ajvpy2-0.1.0/ajvpy2.egg-info/
--rw-r--r--   0 anthony    (501) staff       (20)     2092 2024-06-01 21:55:41.000000 ajvpy2-0.1.0/ajvpy2.egg-info/PKG-INFO
--rw-r--r--   0 anthony    (501) staff       (20)      208 2024-06-01 21:55:41.000000 ajvpy2-0.1.0/ajvpy2.egg-info/SOURCES.txt
--rw-r--r--   0 anthony    (501) staff       (20)        1 2024-06-01 21:55:41.000000 ajvpy2-0.1.0/ajvpy2.egg-info/dependency_links.txt
--rw-r--r--   0 anthony    (501) staff       (20)       48 2024-06-01 21:55:41.000000 ajvpy2-0.1.0/ajvpy2.egg-info/entry_points.txt
--rw-r--r--   0 anthony    (501) staff       (20)       53 2024-06-01 21:55:41.000000 ajvpy2-0.1.0/ajvpy2.egg-info/requires.txt
--rw-r--r--   0 anthony    (501) staff       (20)        1 2024-06-01 21:55:41.000000 ajvpy2-0.1.0/ajvpy2.egg-info/top_level.txt
--rw-r--r--   0 anthony    (501) staff       (20)       38 2024-06-01 21:55:41.630942 ajvpy2-0.1.0/setup.cfg
--rw-r--r--   0 anthony    (501) staff       (20)      924 2024-06-01 21:53:56.000000 ajvpy2-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:05:36.439609 ajvpy2-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 03:05:26.000000 ajvpy2-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-06-02 03:05:36.439609 ajvpy2-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-06-02 03:05:26.000000 ajvpy2-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:05:36.439609 ajvpy2-0.1.1/ajvpy2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-06-02 03:05:36.000000 ajvpy2-0.1.1/ajvpy2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-06-02 03:05:36.000000 ajvpy2-0.1.1/ajvpy2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 03:05:36.000000 ajvpy2-0.1.1/ajvpy2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-02 03:05:36.000000 ajvpy2-0.1.1/ajvpy2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 03:05:36.000000 ajvpy2-0.1.1/ajvpy2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 03:05:36.000000 ajvpy2-0.1.1/ajvpy2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 03:05:36.439609 ajvpy2-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-06-02 03:05:26.000000 ajvpy2-0.1.1/setup.py
```

### Comparing `ajvpy2-0.1.0/LICENSE` & `ajvpy2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ajvpy2-0.1.0/setup.py` & `ajvpy2-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ajvpy2",
-    version="0.1.0",
+    version="0.1.1",
     author="Anthony Chadwick",
     description="A thin wrapper around the AJV JSON Validator for Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atchad/ajvpy2",
     packages=find_packages(exclude=["tests*", "examples*"]),
     include_package_data=True,
```

