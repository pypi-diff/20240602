# Comparing `tmp/simevopy-0.1.9.tar.gz` & `tmp/simevopy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simevopy-0.1.9.tar", last modified: Tue May 21 09:02:33 2024, max compression
+gzip compressed data, was "simevopy-0.2.1.tar", last modified: Sun Jun  2 00:53:19 2024, max compression
```

## Comparing `simevopy-0.1.9.tar` & `simevopy-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-21 09:02:13.000000 simevopy-0.1.9/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 09:02:13.000000 simevopy-0.1.9/.clangd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.945746 simevopy-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-21 09:02:13.000000 simevopy-0.1.9/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 09:02:13.000000 simevopy-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 09:02:13.000000 simevopy-0.1.9/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 09:02:13.000000 simevopy-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-21 09:02:33.953746 simevopy-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-21 09:02:13.000000 simevopy-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/bindings/core/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/core/genes_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/core/organism_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 09:02:13.000000 simevopy-0.1.9/bindings/python_bindings.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      843 2024-05-21 09:02:13.000000 simevopy-0.1.9/bump_version.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:13.000000 simevopy-0.1.9/examples/size_awareness.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 09:02:13.000000 simevopy-0.1.9/examples/speed_food.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.945746 simevopy-0.1.9/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/include/core/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Environment.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Food.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Genes.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/core/Organism.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/include/index/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/ISpatialIndex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/ISpatialObject.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/SpatialIndex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/index/SpatialObjectWrapper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/include/test/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/test/Dummy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-21 09:02:13.000000 simevopy-0.1.9/include/test/SpatialIndexTest.hpp
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:02:33.953746 simevopy-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 09:02:32.000000 simevopy-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/simevopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:02:33.000000 simevopy-0.1.9/simevopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.949746 simevopy-0.1.9/src/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/core/Environment.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/core/Genes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/core/Organism.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/src/index/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/index/DefaultSpatialIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-21 09:02:13.000000 simevopy-0.1.9/src/index/OptimizedSpatialIndex.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.945746 simevopy-0.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:02:33.953746 simevopy-0.1.9/tests/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-21 09:02:13.000000 simevopy-0.1.9/tests/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-21 09:02:13.000000 simevopy-0.1.9/tests/cpp/SpatialIndexTest.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-21 09:02:13.000000 simevopy-0.1.9/tests/cpp/gtest.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-02 00:52:42.000000 simevopy-0.2.1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-02 00:52:42.000000 simevopy-0.2.1/.clangd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.622852 simevopy-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-06-02 00:52:42.000000 simevopy-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 00:52:42.000000 simevopy-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-02 00:52:42.000000 simevopy-0.2.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-02 00:52:42.000000 simevopy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-06-02 00:53:19.630852 simevopy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-06-02 00:52:42.000000 simevopy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/bindings/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/EnvironmentObject_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/Environment_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/Food_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/genes_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/core/organism_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-02 00:52:42.000000 simevopy-0.2.1/bindings/python_bindings.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      843 2024-06-02 00:52:42.000000 simevopy-0.2.1/bump_version.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/chasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/fix_size_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/food_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/oasis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/oasis_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/examples/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-06-02 00:52:42.000000 simevopy-0.2.1/examples/utils/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.622852 simevopy-0.2.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.626852 simevopy-0.2.1/include/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/EnvironmentObject.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Food.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Genes.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/core/Organism.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/include/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/index/DefaultSpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/index/ISpatialIndex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/index/OptimizedSpatialIndex.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/include/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-06-02 00:52:42.000000 simevopy-0.2.1/include/test/SpatialIndexUUIDTest.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:53:19.630852 simevopy-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-06-02 00:53:18.000000 simevopy-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/simevopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:53:19.000000 simevopy-0.2.1/simevopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/core/Environment.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/core/Genes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/core/Organism.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/src/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/index/DefaultSpatialIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10121 2024-06-02 00:52:42.000000 simevopy-0.2.1/src/index/OptimizedSpatialIndex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.622852 simevopy-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/tests/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/cpp/SpatialIndexUUIDTest.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/cpp/gtest.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:19.630852 simevopy-0.2.1/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:52:42.000000 simevopy-0.2.1/tests/python/test_environment.py
```

### Comparing `simevopy-0.1.9/.github/workflows/ci.yml` & `simevopy-0.2.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     steps:
     - name: Checkout code
       uses: actions/checkout@v4
 
     - name: Install dependencies
       run: |
         sudo apt-get update
-        sudo apt-get install -y cmake make g++ build-essential
+        sudo apt-get install -y cmake make g++ build-essential libboost-all-dev
 
     - name: Configure CMake
       run: cmake -S . -B build -DBUILD_BINDINGS=OFF
 
     - name: Build
       run: cmake --build build
 
@@ -107,12 +107,12 @@
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools twine
 
       - name: Publish package
-        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
           package: dist/*.tar.gz
```

### Comparing `simevopy-0.1.9/CMakeLists.txt` & `simevopy-0.2.1/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 # using BUILD_BINDINGS to enable/disable the python bindings
 option(BUILD_BINDINGS "Build Python bindings" ON)
 if(BUILD_BINDINGS)
   add_subdirectory(bindings)
 endif()
 
 # using BUILD_TESTS to enable/disable the tests
-option(BUILD_TESTS "Build the test programs" ON)
+option(BUILD_TESTS "Build the test programs" OFF)
 if(BUILD_TESTS)
   enable_testing()
   add_subdirectory(tests/cpp)
 endif()
```

### Comparing `simevopy-0.1.9/LICENSE` & `simevopy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.9/PKG-INFO` & `simevopy-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: simevopy
-Version: 0.1.9
+Version: 0.2.1
 Summary: SimEvo Python bindings
 Home-page: https://github.com/YJack0000/SimEvo
 Author: YJack0000
 Author-email: yjack0000.cs12@nycu.edu.tw
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 SimEvo: A Simple Python Library for Simulations of Natural Selection
----
+===
 
+[![PyPI - Implementation](https://img.shields.io/pypi/v/simevopy)](https://pypi.org/project/simevopy/)
 [![CodeFactor](https://www.codefactor.io/repository/github/yjack0000/simevo/badge)](https://www.codefactor.io/repository/github/yjack0000/simevo)
 ![GitHub](https://img.shields.io/github/license/YJack0000/SimEvo)
 ![GitHub repo size](https://img.shields.io/github/repo-size/YJack0000/SimEvo)
 
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
```

### Comparing `simevopy-0.1.9/README.md` & `simevopy-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 SimEvo: A Simple Python Library for Simulations of Natural Selection
----
+===
 
+[![PyPI - Implementation](https://img.shields.io/pypi/v/simevopy)](https://pypi.org/project/simevopy/)
 [![CodeFactor](https://www.codefactor.io/repository/github/yjack0000/simevo/badge)](https://www.codefactor.io/repository/github/yjack0000/simevo)
 ![GitHub](https://img.shields.io/github/license/YJack0000/SimEvo)
 ![GitHub repo size](https://img.shields.io/github/repo-size/YJack0000/SimEvo)
 
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
```

### Comparing `simevopy-0.1.9/bump_version.sh` & `simevopy-0.2.1/bump_version.sh`

 * *Files identical despite different names*

### Comparing `simevopy-0.1.9/include/test/SpatialIndexTest.hpp` & `simevopy-0.2.1/include/test/SpatialIndexUUIDTest.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+
 #ifndef SPATIALINDEXTEST_HPP
 #define SPATIALINDEXTEST_HPP
 
 #include <gtest/gtest.h>
 
+#include <boost/uuid/uuid.hpp>
+#include <boost/uuid/uuid_generators.hpp>
+#include <index/DefaultSpatialIndex.hpp>
 #include <index/ISpatialIndex.hpp>
-#include <index/ISpatialObject.hpp>
-#include <index/SpatialIndex.hpp>
-#include <index/SpatialObjectWrapper.hpp>
+#include <index/OptimizedSpatialIndex.hpp>
 #include <memory>
-#include <test/Dummy.hpp>
+
+using namespace boost;
 
 template <typename T>
-class SpatialIndexTest : public ::testing::Test {
+class SpatialIndexUUIDTest : public ::testing::Test {
 protected:
-    std::unique_ptr<ISpatialIndex> index;
-
+    std::unique_ptr<ISpatialIndex<uuids::uuid>> index;
     void SetUp() override;
-
-    std::shared_ptr<ISpatialObject> makeDummyObject(int x, int y);
 };
 
-// Typedefs for ease of use
-using DefaultSpatialIndexTest = SpatialIndexTest<DefaultSpatialIndex>;
-using OptimizedSpatialIndexTest = SpatialIndexTest<OptimizedSpatialIndex>;
+using IndexTypes =
+    ::testing::Types<DefaultSpatialIndex<uuids::uuid>, OptimizedSpatialIndex<uuids::uuid>>;
+TYPED_TEST_SUITE_P(SpatialIndexUUIDTest);
 
 #endif
```

### Comparing `simevopy-0.1.9/setup.py` & `simevopy-0.2.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="simevopy",
-    version='0.1.9',
+    version='0.2.1',
     description="SimEvo Python bindings",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     cmake_source_dir=".",
     url='https://github.com/YJack0000/SimEvo',
     author='YJack0000',
```

### Comparing `simevopy-0.1.9/simevopy.egg-info/PKG-INFO` & `simevopy-0.2.1/simevopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: simevopy
-Version: 0.1.9
+Version: 0.2.1
 Summary: SimEvo Python bindings
 Home-page: https://github.com/YJack0000/SimEvo
 Author: YJack0000
 Author-email: yjack0000.cs12@nycu.edu.tw
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 SimEvo: A Simple Python Library for Simulations of Natural Selection
----
+===
 
+[![PyPI - Implementation](https://img.shields.io/pypi/v/simevopy)](https://pypi.org/project/simevopy/)
 [![CodeFactor](https://www.codefactor.io/repository/github/yjack0000/simevo/badge)](https://www.codefactor.io/repository/github/yjack0000/simevo)
 ![GitHub](https://img.shields.io/github/license/YJack0000/SimEvo)
 ![GitHub repo size](https://img.shields.io/github/repo-size/YJack0000/SimEvo)
 
 ## Basic Information
 
 > **Project Overview:** Simulating Natural Selection in Ecosystems using C++ and Python
```

### Comparing `simevopy-0.1.9/tests/cpp/CMakeLists.txt` & `simevopy-0.2.1/tests/cpp/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 cmake_minimum_required(VERSION 3.24)
 project(SimEvoTests)
 
 include(gtest.cmake)
 
 # add the test executable
-add_executable(test_spatial_index SpatialIndexTest.cpp)
+add_executable(test_spatial_index_uuid SpatialIndexUUIDTest.cpp)
 
 # include from the parent directory
-target_include_directories(test_spatial_index PRIVATE ${PROJECT_SOURCE_DIR}/../include)
-
-target_link_libraries(test_spatial_index index gtest_main gtest)
+target_include_directories(test_spatial_index_uuid
+                           PRIVATE ${PROJECT_SOURCE_DIR}/../include)
+target_link_libraries(test_spatial_index_uuid index gtest_main gtest)
 
 # add the test to the test suite
-add_test(NAME SpatialIndexTest COMMAND test_spatial_index)
-set_tests_properties(SpatialIndexTest PROPERTIES LABELS "SpatialIndex")
+add_test(NAME SpatialIndexUUIDTest COMMAND test_spatial_index_uuid)
+set_tests_properties(SpatialIndexUUIDTest PROPERTIES LABELS "SpatialIndex")
```

