# Comparing `tmp/vpx_rtp_py-0.1.1.tar.gz` & `tmp/vpx_rtp_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpx_rtp_py-0.1.1.tar", max compression
+gzip compressed data, was "vpx_rtp_py-0.1.2.tar", max compression
```

## Comparing `vpx_rtp_py-0.1.1.tar` & `vpx_rtp_py-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/LICENSE
--rw-r--r--   0        0        0      363 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/README.md
--rw-r--r--   0        0        0     6753 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/build_cffi_bindings.py
--rw-r--r--   0        0        0     1132 2024-06-02 05:29:35.810882 vpx_rtp_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-06-02 05:29:35.818882 vpx_rtp_py-0.1.1/vpx_rtp/__init__.py
--rw-r--r--   0        0        0      824 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/clock.py
--rw-r--r--   0        0        0       42 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/codecs/_vpx.pyi
--rw-r--r--   0        0        0    13768 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/codecs/vpx.py
--rw-r--r--   0        0        0     4106 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/jitterbuffer.py
--rw-r--r--   0        0        0        0 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/py.typed
--rw-r--r--   0        0        0     2728 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/rtcrtpparameters.py
--rw-r--r--   0        0        0    12103 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/rtp.py
--rw-r--r--   0        0        0       12 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/test.py
--rw-r--r--   0        0        0      978 2024-06-02 05:29:20.874629 vpx_rtp_py-0.1.1/vpx_rtp/utils.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 vpx_rtp_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/LICENSE
+-rw-r--r--   0        0        0      363 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/README.md
+-rw-r--r--   0        0        0     6753 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/build_cffi_bindings.py
+-rw-r--r--   0        0        0     1285 2024-06-02 05:43:14.967742 vpx_rtp_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-02 05:43:14.971742 vpx_rtp_py-0.1.2/vpx_rtp/__init__.py
+-rw-r--r--   0        0        0      824 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/clock.py
+-rw-r--r--   0        0        0       42 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/codecs/_vpx.pyi
+-rw-r--r--   0        0        0    13768 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/codecs/vpx.py
+-rw-r--r--   0        0        0     4106 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/jitterbuffer.py
+-rw-r--r--   0        0        0        0 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/py.typed
+-rw-r--r--   0        0        0     2728 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/rtcrtpparameters.py
+-rw-r--r--   0        0        0    12103 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/rtp.py
+-rw-r--r--   0        0        0       12 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/test.py
+-rw-r--r--   0        0        0      978 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/utils.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 vpx_rtp_py-0.1.2/PKG-INFO
```

### Comparing `vpx_rtp_py-0.1.1/LICENSE` & `vpx_rtp_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/build_cffi_bindings.py` & `vpx_rtp_py-0.1.2/build_cffi_bindings.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/pyproject.toml` & `vpx_rtp_py-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tool.poetry]
 name = "vpx-rtp-py"
-version = "0.1.1"
+version = "0.1.2"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "vpx_rtp"}]
-include = ["vpx_rtp/*", "*.so","*.o"] # include cffi compiled files as otherwise gitignored
+packages = [{ include = "vpx_rtp" }]
+include = [ # include cffi compiled files in wheel as otherwise gitignored
+    { path = "vpx_rtp", format = ["sdist", "wheel"] },
+    { path = "vpx_rtp/codecs/*.so", format = "wheel" },
+    { path = "vpx_rtp/codecs/*.o", format = "wheel" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 av = "^12.1.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
```

### Comparing `vpx_rtp_py-0.1.1/vpx_rtp/clock.py` & `vpx_rtp_py-0.1.2/vpx_rtp/clock.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/vpx_rtp/codecs/vpx.py` & `vpx_rtp_py-0.1.2/vpx_rtp/codecs/vpx.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/vpx_rtp/jitterbuffer.py` & `vpx_rtp_py-0.1.2/vpx_rtp/jitterbuffer.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/vpx_rtp/rtcrtpparameters.py` & `vpx_rtp_py-0.1.2/vpx_rtp/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/vpx_rtp/rtp.py` & `vpx_rtp_py-0.1.2/vpx_rtp/rtp.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/vpx_rtp/utils.py` & `vpx_rtp_py-0.1.2/vpx_rtp/utils.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.1/PKG-INFO` & `vpx_rtp_py-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpx-rtp-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

