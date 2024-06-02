# Comparing `tmp/pyslsqp-0.1.0.dev1.tar.gz` & `tmp/pyslsqp-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslsqp-0.1.0.dev1.tar", last modified: Sun Jun  2 00:24:38 2024, max compression
+gzip compressed data, was "pyslsqp-0.1.0a0.tar", last modified: Sun Jun  2 00:36:50 2024, max compression
```

## Comparing `pyslsqp-0.1.0.dev1.tar` & `pyslsqp-0.1.0a0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.662047 pyslsqp-0.1.0.dev1/
--rw-r--r--   0 anugrah    (501) staff       (20)     1504 2024-05-20 19:29:24.000000 pyslsqp-0.1.0.dev1/LICENSE.txt
--rw-r--r--   0 anugrah    (501) staff       (20)      388 2024-05-27 21:29:25.000000 pyslsqp-0.1.0.dev1/MANIFEST.in
--rw-r--r--   0 anugrah    (501) staff       (20)    10471 2024-06-02 00:24:38.661350 pyslsqp-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 anugrah    (501) staff       (20)     7012 2024-06-01 23:02:13.000000 pyslsqp-0.1.0.dev1/README.md
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.622578 pyslsqp-0.1.0.dev1/docs/
--rw-r--r--   0 anugrah    (501) staff       (20)     6148 2024-05-17 19:36:37.000000 pyslsqp-0.1.0.dev1/docs/.DS_Store
--rw-r--r--   0 anugrah    (501) staff       (20)      634 2024-05-03 22:09:59.000000 pyslsqp-0.1.0.dev1/docs/Makefile
--rw-r--r--   0 anugrah    (501) staff       (20)     4028 2024-05-24 21:31:59.000000 pyslsqp-0.1.0.dev1/docs/conf.py
--rw-r--r--   0 anugrah    (501) staff       (20)       32 2024-05-03 22:09:59.000000 pyslsqp-0.1.0.dev1/docs/index.md
--rw-r--r--   0 anugrah    (501) staff       (20)      800 2024-05-03 22:09:59.000000 pyslsqp-0.1.0.dev1/docs/make.bat
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.636395 pyslsqp-0.1.0.dev1/docs/src/
--rw-r--r--   0 anugrah    (501) staff       (20)      160 2024-05-18 18:03:53.000000 pyslsqp-0.1.0.dev1/docs/src/api.md
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.638022 pyslsqp-0.1.0.dev1/docs/src/api_pages/
--rw-r--r--   0 anugrah    (501) staff       (20)      204 2024-05-18 18:07:48.000000 pyslsqp-0.1.0.dev1/docs/src/api_pages/optimize.md
--rw-r--r--   0 anugrah    (501) staff       (20)      685 2024-05-18 18:07:21.000000 pyslsqp-0.1.0.dev1/docs/src/api_pages/postprocessing.md
--rw-r--r--   0 anugrah    (501) staff       (20)   230110 2024-05-24 22:50:21.000000 pyslsqp-0.1.0.dev1/docs/src/basic.ipynb
--rw-r--r--   0 anugrah    (501) staff       (20)      317 2024-06-01 23:23:43.000000 pyslsqp-0.1.0.dev1/docs/src/changelog.md
--rw-r--r--   0 anugrah    (501) staff       (20)       38 2024-05-15 18:53:58.000000 pyslsqp-0.1.0.dev1/docs/src/contributing.md
--rw-r--r--   0 anugrah    (501) staff       (20)     2528 2024-05-23 01:38:04.000000 pyslsqp-0.1.0.dev1/docs/src/getting_started.md
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.642709 pyslsqp-0.1.0.dev1/docs/src/images/
--rw-r--r--   0 anugrah    (501) staff       (20)   274879 2024-05-03 22:09:59.000000 pyslsqp-0.1.0.dev1/docs/src/images/lsdolab.png
--rw-r--r--   0 anugrah    (501) staff       (20)   944007 2024-05-03 22:09:59.000000 pyslsqp-0.1.0.dev1/docs/src/images/lsdolab_website.png
--rw-r--r--   0 anugrah    (501) staff       (20)      297 2024-05-20 23:06:12.000000 pyslsqp-0.1.0.dev1/docs/src/license.md
--rw-r--r--   0 anugrah    (501) staff       (20)   141033 2024-05-24 22:50:48.000000 pyslsqp-0.1.0.dev1/docs/src/postprocessing.ipynb
--rw-r--r--   0 anugrah    (501) staff       (20)      999 2024-05-16 21:50:43.000000 pyslsqp-0.1.0.dev1/docs/src/references.bib
--rw-r--r--   0 anugrah    (501) staff       (20)     3734 2024-06-01 22:45:30.000000 pyslsqp-0.1.0.dev1/docs/src/welcome.md
--rw-r--r--   0 anugrah    (501) staff       (20)      777 2024-05-29 19:37:29.000000 pyslsqp-0.1.0.dev1/meson.build
--rw-r--r--   0 anugrah    (501) staff       (20)     3173 2024-06-01 22:44:14.000000 pyslsqp-0.1.0.dev1/pyproject.toml
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.647408 pyslsqp-0.1.0.dev1/pyslsqp/
--rw-r--r--   0 anugrah    (501) staff       (20)       82 2024-06-02 00:04:45.000000 pyslsqp-0.1.0.dev1/pyslsqp/__init__.py
--rw-r--r--   0 anugrah    (501) staff       (20)    46786 2024-05-28 19:44:21.000000 pyslsqp-0.1.0.dev1/pyslsqp/main.py
--rw-r--r--   0 anugrah    (501) staff       (20)     1280 2024-05-27 21:10:24.000000 pyslsqp-0.1.0.dev1/pyslsqp/meson.build
--rw-r--r--   0 anugrah    (501) staff       (20)      162 2024-05-18 01:59:22.000000 pyslsqp-0.1.0.dev1/pyslsqp/postprocessing.py
--rw-r--r--   0 anugrah    (501) staff       (20)    17620 2024-05-24 22:44:57.000000 pyslsqp-0.1.0.dev1/pyslsqp/save_and_load.py
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.654628 pyslsqp-0.1.0.dev1/pyslsqp/slsqp/
--rw-r--r--   0 anugrah    (501) staff       (20)     1535 2024-05-20 17:52:13.000000 pyslsqp-0.1.0.dev1/pyslsqp/slsqp/LICENSE.txt
--rw-r--r--   0 anugrah    (501) staff       (20)     2279 2024-05-20 17:36:18.000000 pyslsqp-0.1.0.dev1/pyslsqp/slsqp/slsqp.pyf
--rw-r--r--   0 anugrah    (501) staff       (20)    69941 2024-05-20 17:37:18.000000 pyslsqp-0.1.0.dev1/pyslsqp/slsqp/slsqp_optmz.f
--rw-r--r--   0 anugrah    (501) staff       (20)    10879 2024-05-24 19:56:46.000000 pyslsqp-0.1.0.dev1/pyslsqp/visualize.py
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.660623 pyslsqp-0.1.0.dev1/pyslsqp.egg-info/
--rw-r--r--   0 anugrah    (501) staff       (20)    10471 2024-06-02 00:24:38.000000 pyslsqp-0.1.0.dev1/pyslsqp.egg-info/PKG-INFO
--rw-r--r--   0 anugrah    (501) staff       (20)     1135 2024-06-02 00:24:38.000000 pyslsqp-0.1.0.dev1/pyslsqp.egg-info/SOURCES.txt
--rw-r--r--   0 anugrah    (501) staff       (20)        1 2024-06-02 00:24:38.000000 pyslsqp-0.1.0.dev1/pyslsqp.egg-info/dependency_links.txt
--rw-r--r--   0 anugrah    (501) staff       (20)       39 2024-06-02 00:24:38.000000 pyslsqp-0.1.0.dev1/pyslsqp.egg-info/requires.txt
--rw-r--r--   0 anugrah    (501) staff       (20)       30 2024-06-02 00:24:38.000000 pyslsqp-0.1.0.dev1/pyslsqp.egg-info/top_level.txt
--rw-r--r--   0 anugrah    (501) staff       (20)       38 2024-06-02 00:24:38.662181 pyslsqp-0.1.0.dev1/setup.cfg
--rw-r--r--   0 anugrah    (501) staff       (20)     5595 2024-05-31 20:11:54.000000 pyslsqp-0.1.0.dev1/setup.py
-drwxr-xr-x   0 anugrah    (501) staff       (20)        0 2024-06-02 00:24:38.659824 pyslsqp-0.1.0.dev1/tests/
--rw-r--r--   0 anugrah    (501) staff       (20)    12600 2024-05-24 22:49:54.000000 pyslsqp-0.1.0.dev1/tests/test_docs.py
--rw-r--r--   0 anugrah    (501) staff       (20)      975 2024-05-24 21:13:24.000000 pyslsqp-0.1.0.dev1/tests/test_docstring_examples.py
--rw-r--r--   0 anugrah    (501) staff       (20)    15734 2024-05-24 21:04:13.000000 pyslsqp-0.1.0.dev1/tests/test_optimize.py
--rw-r--r--   0 anugrah    (501) staff       (20)     6170 2024-05-24 22:42:32.000000 pyslsqp-0.1.0.dev1/tests/test_save_and_load.py
--rw-r--r--   0 anugrah    (501) staff       (20)     2332 2024-05-22 20:41:02.000000 pyslsqp-0.1.0.dev1/tests/testing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/api.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/src/api_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/api_pages/optimize.md
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/api_pages/postprocessing.md
+-rw-r--r--   0 runner    (1001) docker     (127)   230110 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.340170 pyslsqp-0.1.0a0/docs/src/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   274879 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/images/lsdolab.png
+-rw-r--r--   0 runner    (1001) docker     (127)   944007 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/images/lsdolab_website.png
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)   141033 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/postprocessing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/docs/src/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/pyslsqp/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46786 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/save_and_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/pyslsqp/slsqp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/slsqp/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp.pyf
+-rw-r--r--   0 runner    (1001) docker     (127)    69941 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp_optmz.f
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/pyslsqp/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/pyslsqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-02 00:36:50.000000 pyslsqp-0.1.0a0/pyslsqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:36:50.344170 pyslsqp-0.1.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_docstring_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/test_save_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-06-02 00:36:44.000000 pyslsqp-0.1.0a0/tests/testing_utils.py
```

### Comparing `pyslsqp-0.1.0.dev1/LICENSE.txt` & `pyslsqp-0.1.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/PKG-INFO` & `pyslsqp-0.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslsqp
-Version: 0.1.0.dev1
+Version: 0.1.0a0
 Summary: A transparent Python interface to the SLSQP optimization algorithm, with advanced features and visualization capabilities.
 Author-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 Maintainer-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 License: Copyright (c) 2024, Anugrah Jo Joshy.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pyslsqp-0.1.0.dev1/README.md` & `pyslsqp-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/Makefile` & `pyslsqp-0.1.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/conf.py` & `pyslsqp-0.1.0a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/make.bat` & `pyslsqp-0.1.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/api_pages/postprocessing.md` & `pyslsqp-0.1.0a0/docs/src/api_pages/postprocessing.md`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/basic.ipynb` & `pyslsqp-0.1.0a0/docs/src/basic.ipynb`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/getting_started.md` & `pyslsqp-0.1.0a0/docs/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/images/lsdolab.png` & `pyslsqp-0.1.0a0/docs/src/images/lsdolab.png`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/images/lsdolab_website.png` & `pyslsqp-0.1.0a0/docs/src/images/lsdolab_website.png`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/postprocessing.ipynb` & `pyslsqp-0.1.0a0/docs/src/postprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/references.bib` & `pyslsqp-0.1.0a0/docs/src/references.bib`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/docs/src/welcome.md` & `pyslsqp-0.1.0a0/docs/src/welcome.md`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/meson.build` & `pyslsqp-0.1.0a0/meson.build`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyproject.toml` & `pyslsqp-0.1.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp/main.py` & `pyslsqp-0.1.0a0/pyslsqp/main.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp/meson.build` & `pyslsqp-0.1.0a0/pyslsqp/meson.build`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp/save_and_load.py` & `pyslsqp-0.1.0a0/pyslsqp/save_and_load.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp/slsqp/LICENSE.txt` & `pyslsqp-0.1.0a0/pyslsqp/slsqp/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp/slsqp/slsqp.pyf` & `pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp.pyf`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp/slsqp/slsqp_optmz.f` & `pyslsqp-0.1.0a0/pyslsqp/slsqp/slsqp_optmz.f`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp/visualize.py` & `pyslsqp-0.1.0a0/pyslsqp/visualize.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp.egg-info/PKG-INFO` & `pyslsqp-0.1.0a0/pyslsqp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslsqp
-Version: 0.1.0.dev1
+Version: 0.1.0a0
 Summary: A transparent Python interface to the SLSQP optimization algorithm, with advanced features and visualization capabilities.
 Author-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 Maintainer-email: Anugrah Jo Joshy <ajoshy.ucsd@gmail.com>
 License: Copyright (c) 2024, Anugrah Jo Joshy.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pyslsqp-0.1.0.dev1/pyslsqp.egg-info/SOURCES.txt` & `pyslsqp-0.1.0a0/pyslsqp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 ./pyslsqp/save_and_load.py
 ./pyslsqp/visualize.py
 ./tests/test_docs.py
 ./tests/test_docstring_examples.py
 ./tests/test_optimize.py
 ./tests/test_save_and_load.py
 ./tests/testing_utils.py
-docs/.DS_Store
 docs/Makefile
 docs/conf.py
 docs/index.md
 docs/make.bat
 docs/src/api.md
 docs/src/basic.ipynb
 docs/src/changelog.md
```

### Comparing `pyslsqp-0.1.0.dev1/setup.py` & `pyslsqp-0.1.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/tests/test_docs.py` & `pyslsqp-0.1.0a0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/tests/test_docstring_examples.py` & `pyslsqp-0.1.0a0/tests/test_docstring_examples.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/tests/test_optimize.py` & `pyslsqp-0.1.0a0/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/tests/test_save_and_load.py` & `pyslsqp-0.1.0a0/tests/test_save_and_load.py`

 * *Files identical despite different names*

### Comparing `pyslsqp-0.1.0.dev1/tests/testing_utils.py` & `pyslsqp-0.1.0a0/tests/testing_utils.py`

 * *Files identical despite different names*

