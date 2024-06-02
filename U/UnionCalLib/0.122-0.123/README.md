# Comparing `tmp/unioncallib-0.122.tar.gz` & `tmp/unioncallib-0.123.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unioncallib-0.122.tar", last modified: Sun Jun  2 07:04:36 2024, max compression
+gzip compressed data, was "unioncallib-0.123.tar", last modified: Sun Jun  2 07:14:54 2024, max compression
```

## Comparing `unioncallib-0.122.tar` & `unioncallib-0.123.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 yukyulai   (501) staff       (20)        0 2024-06-02 07:04:36.948842 unioncallib-0.122/
--rw-r--r--   0 yukyulai   (501) staff       (20)      224 2024-06-02 07:04:36.948465 unioncallib-0.122/PKG-INFO
-drwxr-xr-x   0 yukyulai   (501) staff       (20)        0 2024-06-02 07:04:36.948138 unioncallib-0.122/UnionCalLib.egg-info/
--rw-r--r--   0 yukyulai   (501) staff       (20)      224 2024-06-02 07:04:36.000000 unioncallib-0.122/UnionCalLib.egg-info/PKG-INFO
--rw-r--r--   0 yukyulai   (501) staff       (20)      200 2024-06-02 07:04:36.000000 unioncallib-0.122/UnionCalLib.egg-info/SOURCES.txt
--rw-r--r--   0 yukyulai   (501) staff       (20)        1 2024-06-02 07:04:36.000000 unioncallib-0.122/UnionCalLib.egg-info/dependency_links.txt
--rw-r--r--   0 yukyulai   (501) staff       (20)       46 2024-06-02 07:04:36.000000 unioncallib-0.122/UnionCalLib.egg-info/entry_points.txt
--rw-r--r--   0 yukyulai   (501) staff       (20)        1 2024-06-02 07:04:36.000000 unioncallib-0.122/UnionCalLib.egg-info/top_level.txt
--rw-r--r--   0 yukyulai   (501) staff       (20)       38 2024-06-02 07:04:36.948908 unioncallib-0.122/setup.cfg
--rw-r--r--   0 yukyulai   (501) staff       (20)      433 2024-06-02 07:04:32.000000 unioncallib-0.122/setup.py
-drwxr-xr-x   0 yukyulai   (501) staff       (20)        0 2024-06-02 07:04:36.947489 unioncallib-0.122/tests/
--rw-r--r--   0 yukyulai   (501) staff       (20)      457 2024-06-01 18:42:13.000000 unioncallib-0.122/tests/test.py
+drwxr-xr-x   0 yukyulai   (501) staff       (20)        0 2024-06-02 07:14:54.678096 unioncallib-0.123/
+-rw-r--r--   0 yukyulai   (501) staff       (20)      224 2024-06-02 07:14:54.677814 unioncallib-0.123/PKG-INFO
+drwxr-xr-x   0 yukyulai   (501) staff       (20)        0 2024-06-02 07:14:54.677541 unioncallib-0.123/UnionCalLib.egg-info/
+-rw-r--r--   0 yukyulai   (501) staff       (20)      224 2024-06-02 07:14:54.000000 unioncallib-0.123/UnionCalLib.egg-info/PKG-INFO
+-rw-r--r--   0 yukyulai   (501) staff       (20)      200 2024-06-02 07:14:54.000000 unioncallib-0.123/UnionCalLib.egg-info/SOURCES.txt
+-rw-r--r--   0 yukyulai   (501) staff       (20)        1 2024-06-02 07:14:54.000000 unioncallib-0.123/UnionCalLib.egg-info/dependency_links.txt
+-rw-r--r--   0 yukyulai   (501) staff       (20)       46 2024-06-02 07:14:54.000000 unioncallib-0.123/UnionCalLib.egg-info/entry_points.txt
+-rw-r--r--   0 yukyulai   (501) staff       (20)        1 2024-06-02 07:14:54.000000 unioncallib-0.123/UnionCalLib.egg-info/top_level.txt
+-rw-r--r--   0 yukyulai   (501) staff       (20)       38 2024-06-02 07:14:54.678162 unioncallib-0.123/setup.cfg
+-rw-r--r--   0 yukyulai   (501) staff       (20)      433 2024-06-02 07:14:46.000000 unioncallib-0.123/setup.py
+drwxr-xr-x   0 yukyulai   (501) staff       (20)        0 2024-06-02 07:14:54.677148 unioncallib-0.123/tests/
+-rw-r--r--   0 yukyulai   (501) staff       (20)      457 2024-06-01 18:42:13.000000 unioncallib-0.123/tests/test.py
```

