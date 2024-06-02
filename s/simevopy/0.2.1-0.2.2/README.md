# Comparing `tmp/simevopy-0.2.1.tar.gz` & `tmp/simevopy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simevopy-0.2.1.tar", last modified: Sun Jun  2 00:53:19 2024, max compression
+gzip compressed data, was "simevopy-0.2.2.tar", last modified: Sun Jun  2 00:58:24 2024, max compression
```

## Comparing `simevopy-0.2.1.tar` & `simevopy-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-02 00:52:42.000000 simevopy-0.2.1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-02 00:52:42.000000 simevopy-0.2.1/.clangd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.622852 simevopy-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-06-02 00:52:42.000000 simevopy-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 00:52:42.000000 simevopy-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-02 00:52:42.000000 simevopy-0.2.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-02 00:52:42.000000 simevopy-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-06-02 00:53:19.630852 simevopy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-06-02 00:52:42.000000 simevopy-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/bindings/core/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/EnvironmentObject_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/Environment_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/Food_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/genes_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/organism_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/python_bindings.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      843 2024-06-02 00:52:42.000000 simevopy-0.2.1/bump_version.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/chasing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/fix_size_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/food_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/oasis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/oasis_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/examples/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/utils/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.622852 simevopy-0.2.1/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/include/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Environment.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/EnvironmentObject.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Food.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Genes.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Organism.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/include/index/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/index/DefaultSpatialIndex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/index/ISpatialIndex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/index/OptimizedSpatialIndex.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/include/test/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/test/SpatialIndexUUIDTest.hpp
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:53:19.630852 simevopy-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-06-02 00:53:18.000000 simevopy-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/simevopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/core/Environment.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/core/Genes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/core/Organism.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/src/index/
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/index/DefaultSpatialIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/index/OptimizedSpatialIndex.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.622852 simevopy-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/tests/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/cpp/SpatialIndexUUIDTest.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/cpp/gtest.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/tests/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/python/test_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-02 00:58:01.000000 simevopy-0.2.2/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-02 00:58:01.000000 simevopy-0.2.2/.clangd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.201573 simevopy-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.205572 simevopy-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-06-02 00:58:01.000000 simevopy-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 00:58:01.000000 simevopy-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-02 00:58:01.000000 simevopy-0.2.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-02 00:58:01.000000 simevopy-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-06-02 00:58:24.209573 simevopy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-06-02 00:58:01.000000 simevopy-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.205572 simevopy-0.2.2/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.205572 simevopy-0.2.2/bindings/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/core/EnvironmentObject_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/core/Environment_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/core/Food_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/core/genes_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/core/organism_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-02 00:58:01.000000 simevopy-0.2.2/bindings/python_bindings.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      843 2024-06-02 00:58:01.000000 simevopy-0.2.2/bump_version.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.205572 simevopy-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/chasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/fix_size_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/food_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/oasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/oasis_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/examples/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-06-02 00:58:01.000000 simevopy-0.2.2/examples/utils/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.205572 simevopy-0.2.2/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/include/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/core/Environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/core/EnvironmentObject.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/core/Food.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/core/Genes.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/core/Organism.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/include/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/index/DefaultSpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/index/ISpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/index/OptimizedSpatialIndex.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/include/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-06-02 00:58:01.000000 simevopy-0.2.2/include/test/SpatialIndexUUIDTest.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:58:24.209573 simevopy-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-06-02 00:58:23.000000 simevopy-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/simevopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-06-02 00:58:24.000000 simevopy-0.2.2/simevopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-02 00:58:24.000000 simevopy-0.2.2/simevopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:58:24.000000 simevopy-0.2.2/simevopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:58:24.000000 simevopy-0.2.2/simevopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-02 00:58:01.000000 simevopy-0.2.2/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-06-02 00:58:01.000000 simevopy-0.2.2/src/core/Environment.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-02 00:58:01.000000 simevopy-0.2.2/src/core/Genes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-06-02 00:58:01.000000 simevopy-0.2.2/src/core/Organism.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/src/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-06-02 00:58:01.000000 simevopy-0.2.2/src/index/DefaultSpatialIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-06-02 00:58:01.000000 simevopy-0.2.2/src/index/OptimizedSpatialIndex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.205572 simevopy-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/tests/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-06-02 00:58:01.000000 simevopy-0.2.2/tests/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-06-02 00:58:01.000000 simevopy-0.2.2/tests/cpp/SpatialIndexUUIDTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-02 00:58:01.000000 simevopy-0.2.2/tests/cpp/gtest.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:24.209573 simevopy-0.2.2/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:58:01.000000 simevopy-0.2.2/tests/python/test_environment.py
```

### Comparing `simevopy-0.2.1/.github/workflows/ci.yml` & `simevopy-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/CMakeLists.txt` & `simevopy-0.2.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/LICENSE` & `simevopy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/PKG-INFO` & `simevopy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simevopy
-Version: 0.2.1
+Version: 0.2.2
 Summary: SimEvo Python bindings
 Home-page: https://github.com/YJack0000/SimEvo
 Author: YJack0000
 Author-email: yjack0000.cs12@nycu.edu.tw
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `simevopy-0.2.1/README.md` & `simevopy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/bindings/CMakeLists.txt` & `simevopy-0.2.2/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/bindings/core/EnvironmentObject_bindings.cpp` & `simevopy-0.2.2/bindings/core/EnvironmentObject_bindings.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/bindings/core/Environment_bindings.cpp` & `simevopy-0.2.2/bindings/core/Environment_bindings.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/bindings/core/organism_bindings.cpp` & `simevopy-0.2.2/bindings/core/organism_bindings.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/bindings/python_bindings.cpp` & `simevopy-0.2.2/bindings/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/bump_version.sh` & `simevopy-0.2.2/bump_version.sh`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/basic.py` & `simevopy-0.2.2/examples/basic.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/chasing.py` & `simevopy-0.2.2/examples/chasing.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/dashboard.py` & `simevopy-0.2.2/examples/dashboard.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/food_path.py` & `simevopy-0.2.2/examples/food_path.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/oasis.py` & `simevopy-0.2.2/examples/oasis.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/oasis_dashboard.py` & `simevopy-0.2.2/examples/oasis_dashboard.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/utils/common.py` & `simevopy-0.2.2/examples/utils/common.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/examples/utils/visualize.py` & `simevopy-0.2.2/examples/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/include/core/Environment.hpp` & `simevopy-0.2.2/include/core/Environment.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/include/core/EnvironmentObject.hpp` & `simevopy-0.2.2/include/core/EnvironmentObject.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/include/core/Organism.hpp` & `simevopy-0.2.2/include/core/Organism.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/include/index/DefaultSpatialIndex.hpp` & `simevopy-0.2.2/include/index/DefaultSpatialIndex.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/include/index/ISpatialIndex.hpp` & `simevopy-0.2.2/include/index/ISpatialIndex.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/include/index/OptimizedSpatialIndex.hpp` & `simevopy-0.2.2/include/index/OptimizedSpatialIndex.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/include/test/SpatialIndexUUIDTest.hpp` & `simevopy-0.2.2/include/test/SpatialIndexUUIDTest.hpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/setup.py` & `simevopy-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="simevopy",
-    version='0.2.1',
+    version='0.2.2',
     description="SimEvo Python bindings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     cmake_source_dir=".",
     url='https://github.com/YJack0000/SimEvo',
     author='YJack0000',
```

### Comparing `simevopy-0.2.1/simevopy.egg-info/PKG-INFO` & `simevopy-0.2.2/simevopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simevopy
-Version: 0.2.1
+Version: 0.2.2
 Summary: SimEvo Python bindings
 Home-page: https://github.com/YJack0000/SimEvo
 Author: YJack0000
 Author-email: yjack0000.cs12@nycu.edu.tw
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `simevopy-0.2.1/simevopy.egg-info/SOURCES.txt` & `simevopy-0.2.2/simevopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/src/CMakeLists.txt` & `simevopy-0.2.2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/src/core/Environment.cpp` & `simevopy-0.2.2/src/core/Environment.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/src/core/Genes.cpp` & `simevopy-0.2.2/src/core/Genes.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/src/core/Organism.cpp` & `simevopy-0.2.2/src/core/Organism.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/src/index/DefaultSpatialIndex.cpp` & `simevopy-0.2.2/src/index/DefaultSpatialIndex.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/src/index/OptimizedSpatialIndex.cpp` & `simevopy-0.2.2/src/index/OptimizedSpatialIndex.cpp`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/tests/cpp/CMakeLists.txt` & `simevopy-0.2.2/tests/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simevopy-0.2.1/tests/cpp/SpatialIndexUUIDTest.cpp` & `simevopy-0.2.2/tests/cpp/SpatialIndexUUIDTest.cpp`

 * *Files identical despite different names*

