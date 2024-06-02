# Comparing `tmp/python-fasthtml-0.0.2.tar.gz` & `tmp/python-fasthtml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-fasthtml-0.0.2.tar", last modified: Fri May 17 08:05:44 2024, max compression
+gzip compressed data, was "python-fasthtml-0.0.3.tar", last modified: Sun Jun  2 05:00:35 2024, max compression
```

## Comparing `python-fasthtml-0.0.2.tar` & `python-fasthtml-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-17 08:05:44.979245 python-fasthtml-0.0.2/
--rw-r--r--   0 jhoward    (501) staff       (20)    11357 2024-05-17 05:17:01.000000 python-fasthtml-0.0.2/LICENSE
--rw-rw-r--   0 jhoward    (501) staff       (20)      111 2023-04-27 10:12:58.000000 python-fasthtml-0.0.2/MANIFEST.in
--rw-r--r--   0 jhoward    (501) staff       (20)     3563 2024-05-17 08:05:44.979055 python-fasthtml-0.0.2/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)     2762 2024-05-17 08:05:22.000000 python-fasthtml-0.0.2/README.md
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-17 08:05:44.977881 python-fasthtml-0.0.2/fasthtml/
--rw-r--r--   0 jhoward    (501) staff       (20)       43 2024-05-17 08:05:12.000000 python-fasthtml-0.0.2/fasthtml/__init__.py
--rw-r--r--   0 jhoward    (501) staff       (20)     1990 2024-05-17 08:05:12.000000 python-fasthtml-0.0.2/fasthtml/_modidx.py
--rw-r--r--   0 jhoward    (501) staff       (20)     4228 2024-05-17 08:05:12.000000 python-fasthtml-0.0.2/fasthtml/core.py
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-17 08:05:44.978735 python-fasthtml-0.0.2/python_fasthtml.egg-info/
--rw-r--r--   0 jhoward    (501) staff       (20)     3563 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)      383 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/SOURCES.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/dependency_links.txt
--rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/entry_points.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-17 05:43:33.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/not-zip-safe
--rw-r--r--   0 jhoward    (501) staff       (20)       56 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/requires.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        9 2024-05-17 08:05:44.000000 python-fasthtml-0.0.2/python_fasthtml.egg-info/top_level.txt
--rw-r--r--   0 jhoward    (501) staff       (20)      893 2024-05-17 08:05:08.000000 python-fasthtml-0.0.2/settings.ini
--rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-17 08:05:44.979294 python-fasthtml-0.0.2/setup.cfg
--rw-rw-r--   0 jhoward    (501) staff       (20)     2598 2024-05-17 05:43:20.000000 python-fasthtml-0.0.2/setup.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-06-02 05:00:35.975847 python-fasthtml-0.0.3/
+-rw-r--r--   0 jhoward    (501) staff       (20)    11357 2024-05-17 05:17:01.000000 python-fasthtml-0.0.3/LICENSE
+-rw-rw-r--   0 jhoward    (501) staff       (20)      111 2023-04-27 10:12:58.000000 python-fasthtml-0.0.3/MANIFEST.in
+-rw-r--r--   0 jhoward    (501) staff       (20)     3658 2024-06-02 05:00:35.975604 python-fasthtml-0.0.3/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)     2762 2024-05-17 08:05:22.000000 python-fasthtml-0.0.3/README.md
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-06-02 05:00:35.974107 python-fasthtml-0.0.3/fasthtml/
+-rw-r--r--   0 jhoward    (501) staff       (20)       90 2024-06-02 03:54:32.000000 python-fasthtml-0.0.3/fasthtml/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     4743 2024-06-02 03:54:32.000000 python-fasthtml-0.0.3/fasthtml/_modidx.py
+-rw-r--r--   0 jhoward    (501) staff       (20)      155 2024-06-01 09:29:12.000000 python-fasthtml-0.0.3/fasthtml/all.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     5119 2024-06-02 03:54:32.000000 python-fasthtml-0.0.3/fasthtml/components.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     9007 2024-06-01 10:24:22.000000 python-fasthtml-0.0.3/fasthtml/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     1108 2024-06-02 01:59:50.000000 python-fasthtml-0.0.3/fasthtml/fastapp.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3555 2024-06-02 03:54:32.000000 python-fasthtml-0.0.3/fasthtml/oauth.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     1007 2024-06-01 10:04:45.000000 python-fasthtml-0.0.3/fasthtml/starlette.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     3485 2024-06-02 03:54:32.000000 python-fasthtml-0.0.3/fasthtml/xtend.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-06-02 05:00:35.975243 python-fasthtml-0.0.3/python_fasthtml.egg-info/
+-rw-r--r--   0 jhoward    (501) staff       (20)     3658 2024-06-02 05:00:35.000000 python-fasthtml-0.0.3/python_fasthtml.egg-info/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)      500 2024-06-02 05:00:35.000000 python-fasthtml-0.0.3/python_fasthtml.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-06-02 05:00:35.000000 python-fasthtml-0.0.3/python_fasthtml.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-06-02 05:00:35.000000 python-fasthtml-0.0.3/python_fasthtml.egg-info/entry_points.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-17 05:43:33.000000 python-fasthtml-0.0.3/python_fasthtml.egg-info/not-zip-safe
+-rw-r--r--   0 jhoward    (501) staff       (20)       91 2024-06-02 05:00:35.000000 python-fasthtml-0.0.3/python_fasthtml.egg-info/requires.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        9 2024-06-02 05:00:35.000000 python-fasthtml-0.0.3/python_fasthtml.egg-info/top_level.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)      930 2024-06-02 04:45:02.000000 python-fasthtml-0.0.3/settings.ini
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-06-02 05:00:35.975899 python-fasthtml-0.0.3/setup.cfg
+-rw-rw-r--   0 jhoward    (501) staff       (20)     2598 2024-05-17 05:43:20.000000 python-fasthtml-0.0.3/setup.py
```

### Comparing `python-fasthtml-0.0.2/LICENSE` & `python-fasthtml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-fasthtml-0.0.2/PKG-INFO` & `python-fasthtml-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fasthtml
-Version: 0.0.2
+Version: 0.0.3
 Summary: The fastest way to create an HTML app
 Home-page: https://github.com/AnswerDotAI/fasthtml
 Author: Jeremy Howard
 Author-email: github@jhoward.fastmail.fm
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -14,17 +14,21 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastcore
 Requires-Dist: python-dateutil
 Requires-Dist: starlette
+Requires-Dist: oauthlib
+Requires-Dist: itsdangerous
+Requires-Dist: uvicorn
+Requires-Dist: httpx
 Provides-Extra: dev
-Requires-Dist: httpx; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: lxml; extra == "dev"
 
 # fasthtml
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 `fasthtml` is a library for writing fast and scalable Starlette-powered
```

### Comparing `python-fasthtml-0.0.2/README.md` & `python-fasthtml-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python-fasthtml-0.0.2/python_fasthtml.egg-info/PKG-INFO` & `python-fasthtml-0.0.3/python_fasthtml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fasthtml
-Version: 0.0.2
+Version: 0.0.3
 Summary: The fastest way to create an HTML app
 Home-page: https://github.com/AnswerDotAI/fasthtml
 Author: Jeremy Howard
 Author-email: github@jhoward.fastmail.fm
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -14,17 +14,21 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastcore
 Requires-Dist: python-dateutil
 Requires-Dist: starlette
+Requires-Dist: oauthlib
+Requires-Dist: itsdangerous
+Requires-Dist: uvicorn
+Requires-Dist: httpx
 Provides-Extra: dev
-Requires-Dist: httpx; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: lxml; extra == "dev"
 
 # fasthtml
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 `fasthtml` is a library for writing fast and scalable Starlette-powered
```

### Comparing `python-fasthtml-0.0.2/settings.ini` & `python-fasthtml-0.0.3/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [DEFAULT]
 repo = fasthtml
 lib_name = fasthtml
-version = 0.0.2
+version = 0.0.3
 min_python = 3.10
 license = apache2
-requirements = fastcore python-dateutil starlette
-dev_requirements = httpx ipython
+requirements = fastcore python-dateutil starlette oauthlib itsdangerous uvicorn httpx
+dev_requirements = ipython lxml
 black_formatting = False
 doc_path = _docs
 lib_path = fasthtml
-nbs_path = .
+nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 branch = main
 custom_sidebar = False
 doc_host = https://AnswerDotAI.github.io
 doc_baseurl = /fasthtml
```

### Comparing `python-fasthtml-0.0.2/setup.py` & `python-fasthtml-0.0.3/setup.py`

 * *Files identical despite different names*

