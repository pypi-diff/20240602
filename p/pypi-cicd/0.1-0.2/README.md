# Comparing `tmp/pypi_cicd-0.1.tar.gz` & `tmp/pypi_cicd-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_cicd-0.1.tar", last modified: Sun Jun  2 15:43:46 2024, max compression
+gzip compressed data, was "pypi_cicd-0.2.tar", last modified: Sun Jun  2 15:51:02 2024, max compression
```

## Comparing `pypi_cicd-0.1.tar` & `pypi_cicd-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:43:46.893859 pypi_cicd-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 15:43:46.893859 pypi_cicd-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 15:43:43.000000 pypi_cicd-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:43:46.889859 pypi_cicd-0.1/pypi_cicd/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 15:43:43.000000 pypi_cicd-0.1/pypi_cicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 15:43:43.000000 pypi_cicd-0.1/pypi_cicd/pypi_cicd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:43:46.893859 pypi_cicd-0.1/pypi_cicd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 15:43:46.000000 pypi_cicd-0.1/pypi_cicd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 15:43:46.000000 pypi_cicd-0.1/pypi_cicd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:43:46.000000 pypi_cicd-0.1/pypi_cicd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 15:43:46.000000 pypi_cicd-0.1/pypi_cicd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:43:46.893859 pypi_cicd-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 15:43:43.000000 pypi_cicd-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:43:46.893859 pypi_cicd-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:43:43.000000 pypi_cicd-0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 15:43:43.000000 pypi_cicd-0.1/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 15:51:02.729137 pypi_cicd-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 15:50:59.000000 pypi_cicd-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/pypi_cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 15:50:59.000000 pypi_cicd-0.2/pypi_cicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 15:50:59.000000 pypi_cicd-0.2/pypi_cicd/pypi_cicd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/pypi_cicd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 15:51:02.000000 pypi_cicd-0.2/pypi_cicd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:51:02.729137 pypi_cicd-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 15:50:59.000000 pypi_cicd-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:51:02.729137 pypi_cicd-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:50:59.000000 pypi_cicd-0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 15:50:59.000000 pypi_cicd-0.2/tests/tests.py
```

### Comparing `pypi_cicd-0.1/tests/tests.py` & `pypi_cicd-0.2/tests/tests.py`

 * *Files identical despite different names*

