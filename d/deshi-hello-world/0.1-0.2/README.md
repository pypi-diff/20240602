# Comparing `tmp/deshi_hello_world-0.1.tar.gz` & `tmp/deshi_hello_world-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deshi_hello_world-0.1.tar", last modified: Sun Jun  2 20:59:59 2024, max compression
+gzip compressed data, was "deshi_hello_world-0.2.tar", last modified: Sun Jun  2 21:33:39 2024, max compression
```

## Comparing `deshi_hello_world-0.1.tar` & `deshi_hello_world-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 20:59:59.081590 deshi_hello_world-0.1/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      174 2024-06-02 20:59:59.081590 deshi_hello_world-0.1/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.1/README.md
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 20:59:59.081590 deshi_hello_world-0.1/deshi_hello_world/
--rw-r--r--   0 deshi     (1000) deshi     (1000)       69 2024-06-02 19:13:33.000000 deshi_hello_world-0.1/deshi_hello_world/__init__.py
--rw-r--r--   0 deshi     (1000) deshi     (1000)      213 2024-06-02 20:55:43.000000 deshi_hello_world-0.1/deshi_hello_world/cli.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 20:59:59.081590 deshi_hello_world-0.1/deshi_hello_world.egg-info/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      174 2024-06-02 20:59:58.000000 deshi_hello_world-0.1/deshi_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-02 20:59:58.000000 deshi_hello_world-0.1/deshi_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-02 20:59:58.000000 deshi_hello_world-0.1/deshi_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       66 2024-06-02 20:59:58.000000 deshi_hello_world-0.1/deshi_hello_world.egg-info/entry_points.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-02 20:59:58.000000 deshi_hello_world-0.1/deshi_hello_world.egg-info/requires.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-02 20:59:58.000000 deshi_hello_world-0.1/deshi_hello_world.egg-info/top_level.txt
--rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-02 20:59:59.081590 deshi_hello_world-0.1/setup.cfg
--rw-r--r--   0 deshi     (1000) deshi     (1000)      435 2024-06-02 20:55:11.000000 deshi_hello_world-0.1/setup.py
-drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 20:59:59.081590 deshi_hello_world-0.1/tests/
--rw-r--r--   0 deshi     (1000) deshi     (1000)      120 2024-06-02 19:16:37.000000 deshi_hello_world-0.1/tests/test_hello_world.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 21:33:39.521075 deshi_hello_world-0.2/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      171 2024-06-02 21:33:39.521075 deshi_hello_world-0.2/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       33 2024-06-02 18:42:56.000000 deshi_hello_world-0.2/README.md
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 21:33:39.511075 deshi_hello_world-0.2/deshi_hello_world/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       69 2024-06-02 19:13:33.000000 deshi_hello_world-0.2/deshi_hello_world/__init__.py
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      213 2024-06-02 20:55:43.000000 deshi_hello_world-0.2/deshi_hello_world/cli.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 21:33:39.521075 deshi_hello_world-0.2/deshi_hello_world.egg-info/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      171 2024-06-02 21:33:39.000000 deshi_hello_world-0.2/deshi_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      357 2024-06-02 21:33:39.000000 deshi_hello_world-0.2/deshi_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        1 2024-06-02 21:33:39.000000 deshi_hello_world-0.2/deshi_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       66 2024-06-02 21:33:39.000000 deshi_hello_world-0.2/deshi_hello_world.egg-info/entry_points.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)        6 2024-06-02 21:33:39.000000 deshi_hello_world-0.2/deshi_hello_world.egg-info/requires.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       18 2024-06-02 21:33:39.000000 deshi_hello_world-0.2/deshi_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 deshi     (1000) deshi     (1000)       79 2024-06-02 21:33:39.521075 deshi_hello_world-0.2/setup.cfg
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      432 2024-06-02 21:33:00.000000 deshi_hello_world-0.2/setup.py
+drwxr-xr-x   0 deshi     (1000) deshi     (1000)        0 2024-06-02 21:33:39.511075 deshi_hello_world-0.2/tests/
+-rw-r--r--   0 deshi     (1000) deshi     (1000)      138 2024-06-02 21:32:55.000000 deshi_hello_world-0.2/tests/test_hello_world.py
```

