# Comparing `tmp/pypi_cicd-0.2.tar.gz` & `tmp/pypi_cicd-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_cicd-0.2.tar", last modified: Sun Jun  2 15:51:02 2024, max compression
+gzip compressed data, was "pypi_cicd-0.3.tar", last modified: Sun Jun  2 16:12:54 2024, max compression
```

## Comparing `pypi_cicd-0.2.tar` & `pypi_cicd-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 15:51:02.729137 pypi_cicd-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 15:50:59.000000 pypi_cicd-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/pypi_cicd/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 15:50:59.000000 pypi_cicd-0.2/pypi_cicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 15:50:59.000000 pypi_cicd-0.2/pypi_cicd/pypi_cicd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/pypi_cicd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:51:02.729137 pypi_cicd-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 15:50:59.000000 pypi_cicd-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:50:59.000000 pypi_cicd-0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 15:50:59.000000 pypi_cicd-0.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:12:54.060781 pypi_cicd-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 16:12:54.060781 pypi_cicd-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 16:12:47.000000 pypi_cicd-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:12:54.060781 pypi_cicd-0.3/pypi_cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 16:12:47.000000 pypi_cicd-0.3/pypi_cicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 16:12:47.000000 pypi_cicd-0.3/pypi_cicd/pypi_cicd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:12:54.060781 pypi_cicd-0.3/pypi_cicd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 16:12:54.000000 pypi_cicd-0.3/pypi_cicd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 16:12:54.000000 pypi_cicd-0.3/pypi_cicd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:12:54.000000 pypi_cicd-0.3/pypi_cicd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 16:12:54.000000 pypi_cicd-0.3/pypi_cicd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:12:54.060781 pypi_cicd-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 16:12:47.000000 pypi_cicd-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:12:54.060781 pypi_cicd-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:12:47.000000 pypi_cicd-0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 16:12:47.000000 pypi_cicd-0.3/tests/tests.py
```

### Comparing `pypi_cicd-0.2/tests/tests.py` & `pypi_cicd-0.3/tests/tests.py`

 * *Files identical despite different names*

