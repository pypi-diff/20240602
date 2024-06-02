# Comparing `tmp/DCMake-0.0.4.tar.gz` & `tmp/DCMake-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DCMake-0.0.4.tar", last modified: Sat Jun  1 12:47:20 2024, max compression
+gzip compressed data, was "DCMake-0.0.5.tar", last modified: Sun Jun  2 02:03:28 2024, max compression
```

## Comparing `DCMake-0.0.4.tar` & `DCMake-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 12:47:20.870179 DCMake-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-06-01 12:47:20.840016 DCMake-0.0.4/DCMake.egg-info/
--rw-rw-rw-   0        0        0      526 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      526 2024-06-01 12:47:20.850054 DCMake-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 12:47:20.829948 DCMake-0.0.4/dcmake/
--rw-rw-rw-   0        0        0     1124 2024-06-01 12:21:11.000000 DCMake-0.0.4/dcmake/__init__.py
--rw-rw-rw-   0        0        0      589 2024-06-01 12:19:05.000000 DCMake-0.0.4/dcmake/tool.py
--rw-rw-rw-   0        0        0     2224 2024-06-01 12:46:54.000000 DCMake-0.0.4/dcmake/url.py
--rw-rw-rw-   0        0        0       42 2024-06-01 12:47:20.870179 DCMake-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      759 2024-06-01 12:47:06.000000 DCMake-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 02:03:28.849748 DCMake-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-06-02 02:03:28.834163 DCMake-0.0.5/DCMake.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      526 2024-06-02 02:03:28.834163 DCMake-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 02:03:28.818499 DCMake-0.0.5/dcmake/
+-rw-rw-rw-   0        0        0     1583 2024-06-02 01:18:17.000000 DCMake-0.0.5/dcmake/__init__.py
+-rw-rw-rw-   0        0        0      290 2024-06-02 01:14:49.000000 DCMake-0.0.5/dcmake/config.py
+-rw-rw-rw-   0        0        0      685 2024-06-02 01:56:56.000000 DCMake-0.0.5/dcmake/tool.py
+-rw-rw-rw-   0        0        0     5518 2024-06-02 01:59:04.000000 DCMake-0.0.5/dcmake/url.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 02:03:28.849748 DCMake-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      759 2024-06-02 01:59:33.000000 DCMake-0.0.5/setup.py
```

### Comparing `DCMake-0.0.4/DCMake.egg-info/PKG-INFO` & `DCMake-0.0.5/DCMake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.4
+Version: 0.0.5
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.4/LICENSE` & `DCMake-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.4/PKG-INFO` & `DCMake-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.4
+Version: 0.0.5
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.4/setup.py` & `DCMake-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="DCMake",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     install_requires=[
         "requests>=2.31.0",
         "tqdm>=4.66.4"
     ],
     entry_points={
         "console_scripts": [
```

