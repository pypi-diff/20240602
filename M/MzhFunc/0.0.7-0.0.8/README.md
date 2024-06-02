# Comparing `tmp/mzhfunc-0.0.7.tar.gz` & `tmp/mzhfunc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzhfunc-0.0.7.tar", last modified: Sun Jun  2 16:11:06 2024, max compression
+gzip compressed data, was "mzhfunc-0.0.8.tar", last modified: Sun Jun  2 16:16:07 2024, max compression
```

## Comparing `mzhfunc-0.0.7.tar` & `mzhfunc-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 16:11:06.913098 mzhfunc-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-06-02 16:11:06.910177 mzhfunc-0.0.7/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      397 2024-06-02 16:11:06.000000 mzhfunc-0.0.7/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-06-02 16:11:06.000000 mzhfunc-0.0.7/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 16:11:06.000000 mzhfunc-0.0.7/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-02 16:11:06.000000 mzhfunc-0.0.7/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      397 2024-06-02 16:11:06.911150 mzhfunc-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 mzhfunc-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 16:11:06.908229 mzhfunc-0.0.7/db/
--rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 mzhfunc-0.0.7/db/MzhFunc.py
--rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 mzhfunc-0.0.7/db/__init__.py
--rw-rw-rw-   0        0        0       67 2024-06-02 16:11:01.000000 mzhfunc-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 16:11:06.913098 mzhfunc-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2026 2024-06-02 15:37:07.000000 mzhfunc-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:16:07.899010 mzhfunc-0.0.8/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:16:07.898036 mzhfunc-0.0.8/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      397 2024-06-02 16:16:07.000000 mzhfunc-0.0.8/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-06-02 16:16:07.000000 mzhfunc-0.0.8/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 16:16:07.000000 mzhfunc-0.0.8/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-02 16:16:07.000000 mzhfunc-0.0.8/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      397 2024-06-02 16:16:07.898036 mzhfunc-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 mzhfunc-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 16:16:07.897062 mzhfunc-0.0.8/db/
+-rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 mzhfunc-0.0.8/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 mzhfunc-0.0.8/db/__init__.py
+-rw-rw-rw-   0        0        0       62 2024-06-02 16:16:04.000000 mzhfunc-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 16:16:07.899010 mzhfunc-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2026 2024-06-02 15:37:07.000000 mzhfunc-0.0.8/setup.py
```

### Comparing `mzhfunc-0.0.7/db/MzhFunc.py` & `mzhfunc-0.0.8/db/MzhFunc.py`

 * *Files identical despite different names*

### Comparing `mzhfunc-0.0.7/setup.py` & `mzhfunc-0.0.8/setup.py`

 * *Files identical despite different names*

