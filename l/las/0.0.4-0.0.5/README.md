# Comparing `tmp/las-0.0.4.tar.gz` & `tmp/las-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "las-0.0.4.tar", last modified: Thu Sep 15 15:35:21 2022, max compression
+gzip compressed data, was "las-0.0.5.tar", last modified: Sun Jun  2 20:30:22 2024, max compression
```

## Comparing `las-0.0.4.tar` & `las-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:35:21.746109 las-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     7404 2022-09-15 15:35:21.746109 las-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6508 2022-09-15 15:35:04.000000 las-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:35:21.746109 las-0.0.4/las.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7404 2022-09-15 15:35:21.000000 las-0.0.4/las.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-15 15:35:21.000000 las-0.0.4/las.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 15:35:21.000000 las-0.0.4/las.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-15 15:35:21.000000 las-0.0.4/las.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-15 15:35:21.000000 las-0.0.4/las.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14695 2022-09-15 15:35:04.000000 las-0.0.4/las.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 15:35:21.746109 las-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-09-15 15:35:04.000000 las-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:30:22.219364 las-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-06-02 20:30:22.219364 las-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-06-02 20:30:18.000000 las-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:30:22.219364 las-0.0.5/las.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-06-02 20:30:22.000000 las-0.0.5/las.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-02 20:30:22.000000 las-0.0.5/las.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 20:30:22.000000 las-0.0.5/las.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 20:30:22.000000 las-0.0.5/las.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-02 20:30:22.000000 las-0.0.5/las.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-06-02 20:30:18.000000 las-0.0.5/las.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 20:30:22.219364 las-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-06-02 20:30:18.000000 las-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:30:22.219364 las-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-06-02 20:30:18.000000 las-0.0.5/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-06-02 20:30:18.000000 las-0.0.5/tests/test_lasitem_from_line.py
```

### Comparing `las-0.0.4/PKG-INFO` & `las-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: las
-Version: 0.0.4
+Version: 0.0.5
 Summary: A reader for Canadian Well Logging Society LAS (Log ASCII Standard) files.
 Home-page: https://github.com/WarrenWeckesser/las
 Author: Warren Weckesser
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
+Requires-Dist: numpy>=1.5.0
 
 las
 ===
 
 The ``las`` module implements a reader for LAS (Log ASCII Standard) well log files (LAS 2.0).
 For more information about this format, see the Canadian Well Logging Society web page
 (https://www.cwls.org/products/).
@@ -167,10 +165,10 @@
     >>> plt.plot(log.data['DEPT'], log.data['GR'])
     >>> plt.xlabel(log.curves.DEPT.descr + " (%s)" % log.curves.DEPT.units)
     >>> plt.ylabel(log.curves.GR.descr + " (%s)" % log.curves.GR.units)
     >>> plt.title(log.well.WELL.data + ', ' + log.well.DATE.data)
     >>> plt.grid()
     >>> plt.show()
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/las/master/examples/example2.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/las/main/examples/example2.png
    :alt: Example 2 plot
    :align: center
```

### Comparing `las-0.0.4/README.rst` & `las-0.0.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -145,10 +145,10 @@
     >>> plt.plot(log.data['DEPT'], log.data['GR'])
     >>> plt.xlabel(log.curves.DEPT.descr + " (%s)" % log.curves.DEPT.units)
     >>> plt.ylabel(log.curves.GR.descr + " (%s)" % log.curves.GR.units)
     >>> plt.title(log.well.WELL.data + ', ' + log.well.DATE.data)
     >>> plt.grid()
     >>> plt.show()
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/las/master/examples/example2.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/las/main/examples/example2.png
    :alt: Example 2 plot
    :align: center
```

### Comparing `las-0.0.4/las.egg-info/PKG-INFO` & `las-0.0.5/las.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: las
-Version: 0.0.4
+Version: 0.0.5
 Summary: A reader for Canadian Well Logging Society LAS (Log ASCII Standard) files.
 Home-page: https://github.com/WarrenWeckesser/las
 Author: Warren Weckesser
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
+Requires-Dist: numpy>=1.5.0
 
 las
 ===
 
 The ``las`` module implements a reader for LAS (Log ASCII Standard) well log files (LAS 2.0).
 For more information about this format, see the Canadian Well Logging Society web page
 (https://www.cwls.org/products/).
@@ -167,10 +165,10 @@
     >>> plt.plot(log.data['DEPT'], log.data['GR'])
     >>> plt.xlabel(log.curves.DEPT.descr + " (%s)" % log.curves.DEPT.units)
     >>> plt.ylabel(log.curves.GR.descr + " (%s)" % log.curves.GR.units)
     >>> plt.title(log.well.WELL.data + ', ' + log.well.DATE.data)
     >>> plt.grid()
     >>> plt.show()
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/las/master/examples/example2.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/las/main/examples/example2.png
    :alt: Example 2 plot
    :align: center
```

### Comparing `las-0.0.4/las.py` & `las-0.0.5/las.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """LAS File Reader
 
 The main class defined here is LASReader, a class that reads a LAS file
 and makes the data available as a Python object.
 """
 
-# Copyright (c) 2011, 2014 Warren Weckesser
+# Copyright (c) 2011, 2014, 2024 Warren Weckesser
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-from __future__ import print_function
 
 import re
 import keyword
 
 import numpy as np
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 def isidentifier(s):
     if s in keyword.kwlist:
         return False
     return re.match(r'^[a-z_][a-z0-9_]*$', s, re.I) is not None
```

### Comparing `las-0.0.4/setup.py` & `las-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,24 +35,21 @@
     long_description_content_type='text/x-rst',
     url="https://github.com/WarrenWeckesser/las",
     license="BSD",
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     py_modules=["las"],
     install_requires=[
         'numpy >= 1.5.0',
     ],
     keyword="numpy las reader",
 )
```

