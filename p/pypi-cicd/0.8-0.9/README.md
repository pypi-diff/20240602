# Comparing `tmp/pypi_cicd-0.8.tar.gz` & `tmp/pypi_cicd-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_cicd-0.8.tar", last modified: Sun Jun  2 18:00:25 2024, max compression
+gzip compressed data, was "pypi_cicd-0.9.tar", last modified: Sun Jun  2 18:08:52 2024, max compression
```

## Comparing `pypi_cicd-0.8.tar` & `pypi_cicd-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:00:25.922697 pypi_cicd-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 18:00:25.922697 pypi_cicd-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 18:00:18.000000 pypi_cicd-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:00:25.918696 pypi_cicd-0.8/pypi_cicd/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 18:00:18.000000 pypi_cicd-0.8/pypi_cicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 18:00:18.000000 pypi_cicd-0.8/pypi_cicd/pypi_cicd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:00:25.922697 pypi_cicd-0.8/pypi_cicd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 18:00:25.000000 pypi_cicd-0.8/pypi_cicd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 18:00:25.000000 pypi_cicd-0.8/pypi_cicd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:00:25.000000 pypi_cicd-0.8/pypi_cicd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 18:00:25.000000 pypi_cicd-0.8/pypi_cicd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:00:25.922697 pypi_cicd-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 18:00:18.000000 pypi_cicd-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:00:25.922697 pypi_cicd-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:00:18.000000 pypi_cicd-0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 18:00:18.000000 pypi_cicd-0.8/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:52.381606 pypi_cicd-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 18:08:52.381606 pypi_cicd-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-02 18:08:49.000000 pypi_cicd-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:52.377606 pypi_cicd-0.9/pypi_cicd/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 18:08:49.000000 pypi_cicd-0.9/pypi_cicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 18:08:49.000000 pypi_cicd-0.9/pypi_cicd/pypi_cicd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:52.381606 pypi_cicd-0.9/pypi_cicd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 18:08:52.000000 pypi_cicd-0.9/pypi_cicd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 18:08:52.000000 pypi_cicd-0.9/pypi_cicd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:08:52.000000 pypi_cicd-0.9/pypi_cicd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 18:08:52.000000 pypi_cicd-0.9/pypi_cicd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:08:52.381606 pypi_cicd-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 18:08:49.000000 pypi_cicd-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:52.381606 pypi_cicd-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:49.000000 pypi_cicd-0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-06-02 18:08:49.000000 pypi_cicd-0.9/tests/tests.py
```

### Comparing `pypi_cicd-0.8/tests/tests.py` & `pypi_cicd-0.9/tests/tests.py`

 * *Files identical despite different names*
