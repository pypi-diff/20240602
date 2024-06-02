# Comparing `tmp/expmiband2-0.1.2.tar.gz` & `tmp/expmiband2-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expmiband2-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "expmiband2-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `expmiband2-0.1.2.tar` & `expmiband2-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        6 2024-05-30 06:27:57.855250 expmiband2-0.1.2/.gitignore
--rw-r--r--   0        0        0     1081 2024-05-30 06:27:57.855250 expmiband2-0.1.2/LICENSE
--rw-r--r--   0        0        0     1759 2024-05-30 06:27:57.855250 expmiband2-0.1.2/README.md
--rw-r--r--   0        0        0      145 2024-05-30 06:42:26.402148 expmiband2-0.1.2/expmiband2/__init__.py
--rw-r--r--   0        0        0     3270 2024-05-30 06:27:57.855250 expmiband2-0.1.2/expmiband2/authsession.py
--rw-r--r--   0        0        0     4278 2024-05-30 06:27:57.855250 expmiband2-0.1.2/expmiband2/band2.py
--rw-r--r--   0        0        0      636 2024-05-30 06:42:17.014366 expmiband2-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 06:35:39.208090 expmiband2-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0       31 2024-05-30 06:36:15.244130 expmiband2-0.1.2/tests/test_it.py
--rw-r--r--   0        0        0     2316 1970-01-01 00:00:00.000000 expmiband2-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2024-05-30 06:27:57.855250 expmiband2-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1081 2024-05-30 06:27:57.855250 expmiband2-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1759 2024-05-30 06:27:57.855250 expmiband2-0.1.3/README.md
+-rw-r--r--   0        0        0      145 2024-06-02 17:25:15.706457 expmiband2-0.1.3/expmiband2/__init__.py
+-rw-r--r--   0        0        0     3270 2024-05-30 06:27:57.855250 expmiband2-0.1.3/expmiband2/authsession.py
+-rw-r--r--   0        0        0     4278 2024-05-30 06:27:57.855250 expmiband2-0.1.3/expmiband2/band2.py
+-rw-r--r--   0        0        0      693 2024-06-02 17:24:59.689693 expmiband2-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 06:35:39.208090 expmiband2-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-30 06:36:15.244130 expmiband2-0.1.3/tests/test_it.py
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 expmiband2-0.1.3/PKG-INFO
```

### Comparing `expmiband2-0.1.2/LICENSE` & `expmiband2-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.2/README.md` & `expmiband2-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.2/expmiband2/authsession.py` & `expmiband2-0.1.3/expmiband2/authsession.py`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.2/expmiband2/band2.py` & `expmiband2-0.1.3/expmiband2/band2.py`

 * *Files identical despite different names*

### Comparing `expmiband2-0.1.2/pyproject.toml` & `expmiband2-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 
 [project.optional-dependencies]
 test = [
     "pytest >= 7.3.0"
 ]
 
 [project.urls]
-Documentation = "https://github.com/anton-ptashnik/test-miband2-api-py"
-Source = "https://github.com/anton-ptashnik/test-miband2-api-py"
+Documentation = "https://github.com/anton-ptashnik/expmiband2-api-py"
+Source = "https://github.com/anton-ptashnik/expmiband2-api-py"
+Home = "https://github.com/anton-ptashnik/expmiband2-api-py"
```

### Comparing `expmiband2-0.1.2/PKG-INFO` & `expmiband2-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: expmiband2
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python API for communicating with MiBand2
 Author-email: Anton Ptashnik <iavtomator@gmail.com>
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: bleak==0.20.1
 Requires-Dist: pyaes==1.6.1
 Requires-Dist: pytest >= 7.3.0 ; extra == "test"
-Project-URL: Documentation, https://github.com/anton-ptashnik/test-miband2-api-py
-Project-URL: Source, https://github.com/anton-ptashnik/test-miband2-api-py
+Project-URL: Documentation, https://github.com/anton-ptashnik/expmiband2-api-py
+Project-URL: Home, https://github.com/anton-ptashnik/expmiband2-api-py
+Project-URL: Source, https://github.com/anton-ptashnik/expmiband2-api-py
 Provides-Extra: test
 
 # MiBand2 Python API based on bleak
 
 The library provides convenient APIs to control and read data of MiBand2.
 
 ## Supported features
```

