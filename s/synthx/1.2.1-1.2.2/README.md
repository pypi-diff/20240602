# Comparing `tmp/synthx-1.2.1.tar.gz` & `tmp/synthx-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-1.2.1.tar", max compression
+gzip compressed data, was "synthx-1.2.2.tar", max compression
```

## Comparing `synthx-1.2.1.tar` & `synthx-1.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7544 2024-04-30 07:29:11.374218 synthx-1.2.1/README.md
--rw-r--r--   0        0        0     1270 2024-05-03 10:37:09.855672 synthx-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.2.1/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.2.1/synthx/core/__init__.py
--rw-r--r--   0        0        0    12500 2024-05-02 15:34:22.114713 synthx-1.2.1/synthx/core/dataset.py
--rw-r--r--   0        0        0     9540 2024-05-03 10:37:09.856021 synthx-1.2.1/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.2.1/synthx/core/sample.py
--rw-r--r--   0        0        0      923 2024-04-30 09:13:40.939358 synthx-1.2.1/synthx/errors/__init__.py
--rw-r--r--   0        0        0    11905 2024-05-03 02:10:08.208860 synthx-1.2.1/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.2.1/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.2.1/synthx/stats/norm.py
--rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.2.1/synthx/stats/p.py
--rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7544 2024-04-30 07:29:11.374218 synthx-1.2.2/README.md
+-rw-r--r--   0        0        0     1270 2024-06-02 12:44:18.517600 synthx-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.2.2/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.2.2/synthx/core/__init__.py
+-rw-r--r--   0        0        0    12500 2024-05-02 15:34:22.114713 synthx-1.2.2/synthx/core/dataset.py
+-rw-r--r--   0        0        0     9540 2024-05-03 10:37:48.868061 synthx-1.2.2/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.2.2/synthx/core/sample.py
+-rw-r--r--   0        0        0      923 2024-04-30 09:13:40.939358 synthx-1.2.2/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    11905 2024-05-03 02:10:08.208860 synthx-1.2.2/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.2.2/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.2.2/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.2.2/synthx/stats/p.py
+-rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.2.2/PKG-INFO
```

### Comparing `synthx-1.2.1/README.md` & `synthx-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/pyproject.toml` & `synthx-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "1.2.1"
+version = "1.2.2"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-1.2.1/synthx/core/dataset.py` & `synthx-1.2.2/synthx/core/dataset.py`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/synthx/core/result.py` & `synthx-1.2.2/synthx/core/result.py`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/synthx/core/sample.py` & `synthx-1.2.2/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/synthx/errors/__init__.py` & `synthx-1.2.2/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/synthx/method.py` & `synthx-1.2.2/synthx/method.py`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/synthx/stats/norm.py` & `synthx-1.2.2/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/synthx/stats/p.py` & `synthx-1.2.2/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-1.2.1/PKG-INFO` & `synthx-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

