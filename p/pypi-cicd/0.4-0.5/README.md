# Comparing `tmp/pypi_cicd-0.4.tar.gz` & `tmp/pypi_cicd-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_cicd-0.4.tar", last modified: Sun Jun  2 16:23:22 2024, max compression
+gzip compressed data, was "pypi_cicd-0.5.tar", last modified: Sun Jun  2 17:25:17 2024, max compression
```

## Comparing `pypi_cicd-0.4.tar` & `pypi_cicd-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:23:22.321383 pypi_cicd-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 16:23:22.321383 pypi_cicd-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 16:23:18.000000 pypi_cicd-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:23:22.317382 pypi_cicd-0.4/pypi_cicd/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 16:23:18.000000 pypi_cicd-0.4/pypi_cicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 16:23:18.000000 pypi_cicd-0.4/pypi_cicd/pypi_cicd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:23:22.321383 pypi_cicd-0.4/pypi_cicd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 16:23:22.000000 pypi_cicd-0.4/pypi_cicd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 16:23:22.000000 pypi_cicd-0.4/pypi_cicd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:23:22.000000 pypi_cicd-0.4/pypi_cicd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 16:23:22.000000 pypi_cicd-0.4/pypi_cicd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:23:22.321383 pypi_cicd-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 16:23:18.000000 pypi_cicd-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:23:22.317382 pypi_cicd-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:23:18.000000 pypi_cicd-0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 16:23:18.000000 pypi_cicd-0.4/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:17.465297 pypi_cicd-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 17:25:17.461297 pypi_cicd-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 17:25:14.000000 pypi_cicd-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:17.461297 pypi_cicd-0.5/pypi_cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 17:25:14.000000 pypi_cicd-0.5/pypi_cicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 17:25:14.000000 pypi_cicd-0.5/pypi_cicd/pypi_cicd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:17.461297 pypi_cicd-0.5/pypi_cicd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 17:25:17.000000 pypi_cicd-0.5/pypi_cicd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 17:25:17.000000 pypi_cicd-0.5/pypi_cicd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:25:17.000000 pypi_cicd-0.5/pypi_cicd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 17:25:17.000000 pypi_cicd-0.5/pypi_cicd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:25:17.465297 pypi_cicd-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 17:25:14.000000 pypi_cicd-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:17.461297 pypi_cicd-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:14.000000 pypi_cicd-0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 17:25:14.000000 pypi_cicd-0.5/tests/tests.py
```

### Comparing `pypi_cicd-0.4/tests/tests.py` & `pypi_cicd-0.5/tests/tests.py`

 * *Files identical despite different names*

