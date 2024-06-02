# Comparing `tmp/mbbank_lib-0.1.3.tar.gz` & `tmp/mbbank_lib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbbank_lib-0.1.3.tar", last modified: Sat Jun  1 06:45:25 2024, max compression
+gzip compressed data, was "mbbank_lib-0.1.4.tar", last modified: Sat Jun  1 07:46:16 2024, max compression
```

## Comparing `mbbank_lib-0.1.3.tar` & `mbbank_lib-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/mbbank/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/mbbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/mbbank/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    13675 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/mbbank/mbasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/mbbank_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 06:45:25.000000 mbbank_lib-0.1.3/mbbank_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:45:25.306233 mbbank_lib-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-01 06:45:16.000000 mbbank_lib-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:46:16.465084 mbbank_lib-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 07:46:07.000000 mbbank_lib-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-06-01 07:46:16.465084 mbbank_lib-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:46:16.461084 mbbank_lib-0.1.4/mbbank/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-01 07:46:07.000000 mbbank_lib-0.1.4/mbbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-06-01 07:46:07.000000 mbbank_lib-0.1.4/mbbank/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13675 2024-06-01 07:46:07.000000 mbbank_lib-0.1.4/mbbank/mbasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:46:16.461084 mbbank_lib-0.1.4/mbbank_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-06-01 07:46:16.000000 mbbank_lib-0.1.4/mbbank_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-01 07:46:16.000000 mbbank_lib-0.1.4/mbbank_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 07:46:16.000000 mbbank_lib-0.1.4/mbbank_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 07:46:16.000000 mbbank_lib-0.1.4/mbbank_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 07:46:16.000000 mbbank_lib-0.1.4/mbbank_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 07:46:16.465084 mbbank_lib-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-01 07:46:07.000000 mbbank_lib-0.1.4/setup.py
```

### Comparing `mbbank_lib-0.1.3/LICENSE.txt` & `mbbank_lib-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbbank_lib-0.1.3/mbbank/main.py` & `mbbank_lib-0.1.4/mbbank/main.py`

 * *Files identical despite different names*

### Comparing `mbbank_lib-0.1.3/mbbank/mbasync.py` & `mbbank_lib-0.1.4/mbbank/mbasync.py`

 * *Files identical despite different names*

### Comparing `mbbank_lib-0.1.3/setup.py` & `mbbank_lib-0.1.4/setup.py`

 * *Files identical despite different names*

