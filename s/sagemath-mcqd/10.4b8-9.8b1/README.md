# Comparing `tmp/sagemath_mcqd-10.4b8.tar.gz` & `tmp/sagemath-mcqd-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath_mcqd-10.4b8.tar", last modified: Sat Jun  1 22:47:26 2024, max compression
+gzip compressed data, was "sagemath-mcqd-9.8b1.tar", last modified: Mon Nov 21 07:31:29 2022, max compression
```

## Comparing `sagemath_mcqd-10.4b8.tar` & `sagemath-mcqd-9.8b1.tar`

### file list

```diff
@@ -1,22 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.071910 sagemath_mcqd-10.4b8/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-06-01 22:47:26.071910 sagemath_mcqd-10.4b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-06-01 22:42:41.000000 sagemath_mcqd-10.4b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/pyproject.toml.m4
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/requirements.txt.m4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.067910 sagemath_mcqd-10.4b8/sage/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/sage/all__sagemath_mcqd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.067910 sagemath_mcqd-10.4b8/sage/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/sage/graphs/all__sagemath_mcqd.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/sage/graphs/mcqd.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/sage/graphs/mcqd.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:47:26.071910 sagemath_mcqd-10.4b8/sagemath_mcqd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-06-01 22:47:24.000000 sagemath_mcqd-10.4b8/sagemath_mcqd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-01 22:47:26.000000 sagemath_mcqd-10.4b8/sagemath_mcqd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:47:24.000000 sagemath_mcqd-10.4b8/sagemath_mcqd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-01 22:47:24.000000 sagemath_mcqd-10.4b8/sagemath_mcqd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 22:47:24.000000 sagemath_mcqd-10.4b8/sagemath_mcqd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:47:26.071910 sagemath_mcqd-10.4b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-06-01 22:41:36.000000 sagemath_mcqd-10.4b8/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.435581 sagemath-mcqd-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-mcqd-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2388 2022-11-21 07:31:29.435722 sagemath-mcqd-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1316 2022-11-20 23:46:42.000000 sagemath-mcqd-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-mcqd-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.432004 sagemath-mcqd-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.433786 sagemath-mcqd-9.8b1/sage/graphs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1677 2022-10-12 20:41:10.000000 sagemath-mcqd-9.8b1/sage/graphs/mcqd.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.435257 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2388 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      261 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1091 2022-11-21 07:31:29.436316 sagemath-mcqd-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2055 2022-11-20 23:45:29.000000 sagemath-mcqd-9.8b1/setup.py
```

### Comparing `sagemath_mcqd-10.4b8/PKG-INFO` & `sagemath-mcqd-9.8b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-mcqd
-Version: 10.4b8
-Summary: Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with mcqd
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: memory_allocator
-Requires-Dist: cysignals>=1.10.2
 
 ===========================================================================
  Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
 ===========================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_mcqd-10.4b8/README.rst` & `sagemath-mcqd-9.8b1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_mcqd-10.4b8/sage/graphs/mcqd.pyx` & `sagemath-mcqd-9.8b1/sage/graphs/mcqd.pyx`

 * *Files identical despite different names*

### Comparing `sagemath_mcqd-10.4b8/sagemath_mcqd.egg-info/PKG-INFO` & `sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: sagemath-mcqd
-Version: 10.4b8
-Summary: Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
-Author-email: The Sage Developers <sage-support@googlegroups.com>
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with mcqd
+Home-page: https://www.sagemath.org
+Author: The Sage Developers
+Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
-Project-URL: Homepage, https://www.sagemath.org
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: memory_allocator
-Requires-Dist: cysignals>=1.10.2
 
 ===========================================================================
  Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
 ===========================================================================
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
-macOS, and Windows (Windows Subsystem for Linux).
+macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
 Sage-the-distribution (https://www.sagemath.org/download-source.html).
 Sage-the-distribution first builds a large number of open source packages from
 source (unless it finds suitable versions installed in the system) and then
 installs the Sage Library (sagelib, implemented in Python and Cython).
```

### Comparing `sagemath_mcqd-10.4b8/setup.py` & `sagemath-mcqd-9.8b1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,28 +38,31 @@
     setenv()
 
     import sage.env
     sage.env.default_required_modules = sage.env.default_optional_modules = ()
 
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
-    from sage_setup.command.sage_build_py import sage_build_py
     sage_build_cython.built_distributions = ['sagemath-mcqd']
 
     cmdclass = dict(build_cython=sage_build_cython,
-                    build_ext=sage_build_ext,
-                    build_py=sage_build_py)
+                    build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-mcqd'])
-
-log.warn('python_packages = {0}'.format(python_packages))
-log.warn('python_modules = {0}'.format(python_modules))
-log.warn('cython_modules = {0}'.format(cython_modules))
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-mcqd'])
+
+    log.warn('python_packages = {0}'.format(python_packages))
+    log.warn('python_modules = {0}'.format(python_modules))
+    log.warn('cython_modules = {0}'.format(cython_modules))
 
 setup(
     cmdclass = cmdclass,
     packages = python_packages,
     py_modules  = python_modules,
     ext_modules = cython_modules,
 )
```

