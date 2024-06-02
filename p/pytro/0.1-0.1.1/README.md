# Comparing `tmp/pytro-0.1.tar.gz` & `tmp/pytro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytro-0.1.tar", last modified: Sun Jun  2 10:45:44 2024, max compression
+gzip compressed data, was "pytro-0.1.1.tar", last modified: Sun Jun  2 10:51:12 2024, max compression
```

## Comparing `pytro-0.1.tar` & `pytro-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-06-02 10:45:44.406036 pytro-0.1/
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2024-06-02 10:45:44.406036 pytro-0.1/PKG-INFO
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-06-02 10:45:44.406036 pytro-0.1/pytro.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2024-06-02 10:45:44.000000 pytro-0.1/pytro.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      161 2024-06-02 10:45:44.000000 pytro-0.1/pytro.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       80 2024-06-02 10:45:44.000000 pytro-0.1/pytro.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       24 2024-06-02 10:45:44.000000 pytro-0.1/pytro.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        6 2024-06-02 10:45:44.000000 pytro-0.1/pytro.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)     1046 2024-06-02 09:56:11.000000 pytro-0.1/pytro.py
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2024-06-02 10:45:44.406036 pytro-0.1/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      316 2024-06-02 10:45:31.000000 pytro-0.1/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-06-02 10:51:12.581128 pytro-0.1.1/
+-rw-r--r--   0 alex      (1000) alex      (1000)      182 2024-06-02 10:51:12.581128 pytro-0.1.1/PKG-INFO
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-06-02 10:51:12.581128 pytro-0.1.1/pytro.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      182 2024-06-02 10:51:12.000000 pytro-0.1.1/pytro.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      161 2024-06-02 10:51:12.000000 pytro-0.1.1/pytro.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       79 2024-06-02 10:51:12.000000 pytro-0.1.1/pytro.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       24 2024-06-02 10:51:12.000000 pytro-0.1.1/pytro.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        6 2024-06-02 10:51:12.000000 pytro-0.1.1/pytro.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)     1046 2024-06-02 09:56:11.000000 pytro-0.1.1/pytro.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2024-06-02 10:51:12.584462 pytro-0.1.1/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      317 2024-06-02 10:50:56.000000 pytro-0.1.1/setup.py
```

### Comparing `pytro-0.1/pytro.py` & `pytro-0.1.1/pytro.py`

 * *Files identical despite different names*

