# Comparing `tmp/ruqia-0.0.8.tar.gz` & `tmp/ruqia-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruqia-0.0.8.tar", last modified: Wed Oct 12 22:06:52 2022, max compression
+gzip compressed data, was "ruqia-0.0.9.tar", last modified: Fri Oct 14 07:26:32 2022, max compression
```

## Comparing `ruqia-0.0.8.tar` & `ruqia-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 22:06:52.019327 ruqia-0.0.8/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 20:16:40.000000 ruqia-0.0.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2018 2022-10-12 22:06:52.019327 ruqia-0.0.8/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1028 2022-10-12 22:03:39.000000 ruqia-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 22:06:52.019327 ruqia-0.0.8/data/
--rwxr-xr-x   0 root         (0) root         (0)        9 2022-10-12 07:53:32.000000 ruqia-0.0.8/data/data_file
--rwxr-xr-x   0 root         (0) root         (0)      235 2022-10-12 07:53:32.000000 ruqia-0.0.8/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)       78 2022-10-12 22:06:52.019327 ruqia-0.0.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     8503 2022-10-12 21:58:14.000000 ruqia-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 22:06:52.019327 ruqia-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 22:06:52.019327 ruqia-0.0.8/src/ruqia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2018 2022-10-12 22:06:52.000000 ruqia-0.0.8/src/ruqia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      342 2022-10-12 22:06:52.000000 ruqia-0.0.8/src/ruqia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-12 22:06:52.000000 ruqia-0.0.8/src/ruqia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-10-12 22:06:52.000000 ruqia-0.0.8/src/ruqia.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       50 2022-10-12 22:06:52.000000 ruqia-0.0.8/src/ruqia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-12 22:06:52.000000 ruqia-0.0.8/src/ruqia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 22:06:52.019327 ruqia-0.0.8/src/ruqiya/
--rwxr-xr-x   0 root         (0) root         (0)      114 2022-10-12 07:53:32.000000 ruqia-0.0.8/src/ruqiya/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)        9 2022-10-12 07:53:32.000000 ruqia-0.0.8/src/ruqiya/package_data.dat
--rwxr-xr-x   0 root         (0) root         (0)    17619 2022-10-12 21:46:41.000000 ruqia-0.0.8/src/ruqiya/ruqiya.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 07:26:32.654045 ruqia-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1992 2022-10-14 07:26:32.654045 ruqia-0.0.9/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1028 2022-10-12 22:03:39.000000 ruqia-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 07:26:32.654045 ruqia-0.0.9/data/
+-rwxr-xr-x   0 root         (0) root         (0)        9 2022-10-12 07:53:32.000000 ruqia-0.0.9/data/data_file
+-rwxr-xr-x   0 root         (0) root         (0)      235 2022-10-12 07:53:32.000000 ruqia-0.0.9/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)       78 2022-10-14 07:26:32.654045 ruqia-0.0.9/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     8503 2022-10-14 07:22:51.000000 ruqia-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 07:26:32.644045 ruqia-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 07:26:32.654045 ruqia-0.0.9/src/ruqia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1992 2022-10-14 07:26:32.000000 ruqia-0.0.9/src/ruqia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      330 2022-10-14 07:26:32.000000 ruqia-0.0.9/src/ruqia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-14 07:26:32.000000 ruqia-0.0.9/src/ruqia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2022-10-14 07:26:32.000000 ruqia-0.0.9/src/ruqia.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2022-10-14 07:26:32.000000 ruqia-0.0.9/src/ruqia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-10-14 07:26:32.000000 ruqia-0.0.9/src/ruqia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 07:26:32.654045 ruqia-0.0.9/src/ruqiya/
+-rwxr-xr-x   0 root         (0) root         (0)      114 2022-10-12 07:53:32.000000 ruqia-0.0.9/src/ruqiya/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)        9 2022-10-12 07:53:32.000000 ruqia-0.0.9/src/ruqiya/package_data.dat
+-rwxr-xr-x   0 root         (0) root         (0)    17619 2022-10-12 21:46:41.000000 ruqia-0.0.9/src/ruqiya/ruqiya.py
```

### Comparing `ruqia-0.0.8/PKG-INFO` & `ruqia-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruqia
-Version: 0.0.8
+Version: 0.0.9
 Summary: Arabic NLP
 Home-page: https://github.com/Ruqyai/Ara-NLP-lib
 Author: Ruqiya Bin Safi
 Author-email: myacount05@gmail.com
 Project-URL: Bug Reports, https://github.com/Ruqyai/Ara-NLP-lib/issues
 Project-URL: Become a sponsor, https://github.com/sponsors/Ruqyai
 Project-URL: Source, https://github.com/Ruqyai/Ara-NLP-lib
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE.txt
 
 # Ruqia lib
 This library used for Arabic NLP to process, prepare and clean the Arabic text
 ## Install
 ```
 pip install ruqia
 ```
```

### Comparing `ruqia-0.0.8/README.md` & `ruqia-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ruqia-0.0.8/setup.py` & `ruqia-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name="ruqia",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.8",  # Required
+    version="0.0.9",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Arabic NLP",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ruqia-0.0.8/src/ruqia.egg-info/PKG-INFO` & `ruqia-0.0.9/src/ruqia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruqia
-Version: 0.0.8
+Version: 0.0.9
 Summary: Arabic NLP
 Home-page: https://github.com/Ruqyai/Ara-NLP-lib
 Author: Ruqiya Bin Safi
 Author-email: myacount05@gmail.com
 Project-URL: Bug Reports, https://github.com/Ruqyai/Ara-NLP-lib/issues
 Project-URL: Become a sponsor, https://github.com/sponsors/Ruqyai
 Project-URL: Source, https://github.com/Ruqyai/Ara-NLP-lib
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE.txt
 
 # Ruqia lib
 This library used for Arabic NLP to process, prepare and clean the Arabic text
 ## Install
 ```
 pip install ruqia
 ```
```

### Comparing `ruqia-0.0.8/src/ruqiya/ruqiya.py` & `ruqia-0.0.9/src/ruqiya/ruqiya.py`

 * *Files identical despite different names*

