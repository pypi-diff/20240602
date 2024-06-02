# Comparing `tmp/nnops-0.0.1.tar.gz` & `tmp/nnops-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnops-0.0.1.tar", last modified: Fri May 31 23:46:05 2024, max compression
+gzip compressed data, was "nnops-0.0.2.tar", last modified: Sat Jun  1 08:24:52 2024, max compression
```

## Comparing `nnops-0.0.1.tar` & `nnops-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.134832 nnops-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-31 23:45:57.000000 nnops-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-31 23:45:57.000000 nnops-0.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-31 23:45:57.000000 nnops-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-31 23:45:57.000000 nnops-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 23:46:05.134832 nnops-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-31 23:45:57.000000 nnops-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.130832 nnops-0.0.1/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 23:45:57.000000 nnops-0.0.1/csrc/python.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.130832 nnops-0.0.1/nnops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:45:57.000000 nnops-0.0.1/nnops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:46:05.134832 nnops-0.0.1/nnops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 23:46:05.000000 nnops-0.0.1/nnops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-31 23:45:57.000000 nnops-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:46:05.134832 nnops-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-31 23:45:57.000000 nnops-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:24:52.463651 nnops-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-01 08:24:41.000000 nnops-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-01 08:24:41.000000 nnops-0.0.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-06-01 08:24:41.000000 nnops-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-01 08:24:41.000000 nnops-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 08:24:52.463651 nnops-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-06-01 08:24:41.000000 nnops-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:24:52.463651 nnops-0.0.2/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-06-01 08:24:41.000000 nnops-0.0.2/csrc/data_type.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-06-01 08:24:41.000000 nnops-0.0.2/csrc/data_type.h
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-06-01 08:24:41.000000 nnops-0.0.2/csrc/python.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-06-01 08:24:41.000000 nnops-0.0.2/csrc/tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-01 08:24:41.000000 nnops-0.0.2/csrc/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-01 08:24:41.000000 nnops-0.0.2/csrc/tensor_shape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-01 08:24:41.000000 nnops-0.0.2/csrc/tensor_shape.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:24:52.463651 nnops-0.0.2/nnops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:24:41.000000 nnops-0.0.2/nnops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-01 08:24:41.000000 nnops-0.0.2/nnops/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:24:52.463651 nnops-0.0.2/nnops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 08:24:52.000000 nnops-0.0.2/nnops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-06-01 08:24:52.000000 nnops-0.0.2/nnops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:24:52.000000 nnops-0.0.2/nnops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 08:24:52.000000 nnops-0.0.2/nnops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 08:24:52.000000 nnops-0.0.2/nnops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-01 08:24:41.000000 nnops-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 08:24:52.467651 nnops-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-06-01 08:24:41.000000 nnops-0.0.2/setup.py
```

### Comparing `nnops-0.0.1/.gitignore` & `nnops-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nnops-0.0.1/CMakeLists.txt` & `nnops-0.0.2/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -13,10 +13,13 @@
   COMMAND "${Python_EXECUTABLE}" -m nanobind --cmake_dir
   OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NB_DIR)
 list(APPEND CMAKE_PREFIX_PATH "${NB_DIR}")
 find_package(nanobind CONFIG REQUIRED)
 
 nanobind_add_module(
   _C STABLE_ABI
+  csrc/data_type.h csrc/data_type.cpp
+  csrc/tensor_shape.h csrc/tensor_shape.cpp
+  csrc/tensor.h csrc/tensor.cpp
   csrc/python.cpp
 )
 target_link_libraries(_C PRIVATE rt)
```

### Comparing `nnops-0.0.1/LICENSE` & `nnops-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nnops-0.0.1/PKG-INFO` & `nnops-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnops
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neural Network Operators
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/nnops
 Keywords: Deep Learning,Neural Network Operators,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nnops Version: 0.0.1 Summary: Neural Network
+Metadata-Version: 2.1 Name: nnops Version: 0.0.2 Summary: Neural Network
 Operators Author-email: Jiau Zhang
 163.com> Project-URL: Homepage, https://github.com/jiauzhang/nnops Keywords:
 Deep Learning,Neural Network Operators,Artificial Intelligence Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: License :: OSI Approved :: GNU General
 Public License v2 (GPLv2) Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
```

### Comparing `nnops-0.0.1/README.md` & `nnops-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nnops-0.0.1/nnops.egg-info/PKG-INFO` & `nnops-0.0.2/nnops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnops
-Version: 0.0.1
+Version: 0.0.2
 Summary: Neural Network Operators
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/nnops
 Keywords: Deep Learning,Neural Network Operators,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nnops Version: 0.0.1 Summary: Neural Network
+Metadata-Version: 2.1 Name: nnops Version: 0.0.2 Summary: Neural Network
 Operators Author-email: Jiau Zhang
 163.com> Project-URL: Homepage, https://github.com/jiauzhang/nnops Keywords:
 Deep Learning,Neural Network Operators,Artificial Intelligence Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: License :: OSI Approved :: GNU General
 Public License v2 (GPLv2) Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
```

### Comparing `nnops-0.0.1/pyproject.toml` & `nnops-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "cmake >= 3.15",
     "nanobind >= 1.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nnops"
-version = "0.0.1"
+version = "0.0.2"
 description = "Neural Network Operators"
 readme = "README.md"
 authors = [
     {name = "Jiau Zhang", email = "jiauzhang@163.com"},
 ]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `nnops-0.0.1/setup.py` & `nnops-0.0.2/setup.py`

 * *Files identical despite different names*

