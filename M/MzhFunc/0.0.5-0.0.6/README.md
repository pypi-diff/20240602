# Comparing `tmp/MzhFunc-0.0.5.tar.gz` & `tmp/mzhfunc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MzhFunc-0.0.5.tar", last modified: Sun Jun  2 15:50:52 2024, max compression
+gzip compressed data, was "mzhfunc-0.0.6.tar", last modified: Sun Jun  2 16:07:57 2024, max compression
```

## Comparing `MzhFunc-0.0.5.tar` & `mzhfunc-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 15:50:52.214371 MzhFunc-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-06-02 15:50:52.212425 MzhFunc-0.0.5/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      397 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      397 2024-06-02 15:50:52.214371 MzhFunc-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 15:50:52.213398 MzhFunc-0.0.5/db/
--rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 MzhFunc-0.0.5/db/MzhFunc.py
--rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 MzhFunc-0.0.5/db/__init__.py
--rw-rw-rw-   0        0        0       48 2024-06-02 13:12:49.000000 MzhFunc-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 15:50:52.214371 MzhFunc-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2026 2024-06-02 15:37:07.000000 MzhFunc-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:07:57.632668 mzhfunc-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:07:57.631694 mzhfunc-0.0.6/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      397 2024-06-02 16:07:57.000000 mzhfunc-0.0.6/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-06-02 16:07:57.000000 mzhfunc-0.0.6/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 16:07:57.000000 mzhfunc-0.0.6/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-02 16:07:57.000000 mzhfunc-0.0.6/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      397 2024-06-02 16:07:57.631694 mzhfunc-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 mzhfunc-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 16:07:57.630721 mzhfunc-0.0.6/db/
+-rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 mzhfunc-0.0.6/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 mzhfunc-0.0.6/db/__init__.py
+-rw-rw-rw-   0        0        0       62 2024-06-02 16:07:53.000000 mzhfunc-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 16:07:57.632668 mzhfunc-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2026 2024-06-02 15:37:07.000000 mzhfunc-0.0.6/setup.py
```

### Comparing `MzhFunc-0.0.5/db/MzhFunc.py` & `mzhfunc-0.0.6/db/MzhFunc.py`

 * *Files identical despite different names*

### Comparing `MzhFunc-0.0.5/setup.py` & `mzhfunc-0.0.6/setup.py`

 * *Files identical despite different names*

