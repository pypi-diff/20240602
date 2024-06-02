# Comparing `tmp/meghana_hello_world-0.2.tar.gz` & `tmp/meghana_hello_world-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meghana_hello_world-0.2.tar", last modified: Sun Jun  2 21:08:43 2024, max compression
+gzip compressed data, was "meghana_hello_world-0.3.tar", last modified: Sun Jun  2 21:42:39 2024, max compression
```

## Comparing `meghana_hello_world-0.2.tar` & `meghana_hello_world-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:08:43.864502 meghana_hello_world-0.2/
--rw-r--r--   0 meghana   (1000) meghana   (1000)       22 2024-06-02 19:15:26.000000 meghana_hello_world-0.2/LICENSE
--rw-r--r--   0 meghana   (1000) meghana   (1000)       51 2024-06-02 21:02:00.000000 meghana_hello_world-0.2/MANIFEST.in
--rw-r--r--   0 meghana   (1000) meghana   (1000)      196 2024-06-02 21:08:43.864502 meghana_hello_world-0.2/PKG-INFO
--rw-r--r--   0 meghana   (1000) meghana   (1000)       53 2024-06-02 19:15:16.000000 meghana_hello_world-0.2/README.md
-drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:08:43.864502 meghana_hello_world-0.2/meghana_hello_world/
--rw-r--r--   0 meghana   (1000) meghana   (1000)       69 2024-06-02 19:13:51.000000 meghana_hello_world-0.2/meghana_hello_world/__init__.py
--rw-r--r--   0 meghana   (1000) meghana   (1000)      225 2024-06-02 21:02:13.000000 meghana_hello_world-0.2/meghana_hello_world/cli.py
-drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:08:43.864502 meghana_hello_world-0.2/meghana_hello_world.egg-info/
--rw-r--r--   0 meghana   (1000) meghana   (1000)      196 2024-06-02 21:08:43.000000 meghana_hello_world-0.2/meghana_hello_world.egg-info/PKG-INFO
--rw-r--r--   0 meghana   (1000) meghana   (1000)      393 2024-06-02 21:08:43.000000 meghana_hello_world-0.2/meghana_hello_world.egg-info/SOURCES.txt
--rw-r--r--   0 meghana   (1000) meghana   (1000)        1 2024-06-02 21:08:43.000000 meghana_hello_world-0.2/meghana_hello_world.egg-info/dependency_links.txt
--rw-r--r--   0 meghana   (1000) meghana   (1000)       70 2024-06-02 21:08:43.000000 meghana_hello_world-0.2/meghana_hello_world.egg-info/entry_points.txt
--rw-r--r--   0 meghana   (1000) meghana   (1000)        6 2024-06-02 21:08:43.000000 meghana_hello_world-0.2/meghana_hello_world.egg-info/requires.txt
--rw-r--r--   0 meghana   (1000) meghana   (1000)       20 2024-06-02 21:08:43.000000 meghana_hello_world-0.2/meghana_hello_world.egg-info/top_level.txt
--rw-r--r--   0 meghana   (1000) meghana   (1000)       79 2024-06-02 21:08:43.864502 meghana_hello_world-0.2/setup.cfg
--rw-r--r--   0 meghana   (1000) meghana   (1000)      457 2024-06-02 21:08:24.000000 meghana_hello_world-0.2/setup.py
-drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:08:43.864502 meghana_hello_world-0.2/tests/
--rw-r--r--   0 meghana   (1000) meghana   (1000)      128 2024-06-02 21:02:09.000000 meghana_hello_world-0.2/tests/test_hello_world.py
+drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:42:39.394110 meghana_hello_world-0.3/
+-rw-r--r--   0 meghana   (1000) meghana   (1000)       22 2024-06-02 19:15:26.000000 meghana_hello_world-0.3/LICENSE
+-rw-r--r--   0 meghana   (1000) meghana   (1000)       51 2024-06-02 21:02:00.000000 meghana_hello_world-0.3/MANIFEST.in
+-rw-r--r--   0 meghana   (1000) meghana   (1000)      196 2024-06-02 21:42:39.384110 meghana_hello_world-0.3/PKG-INFO
+-rw-r--r--   0 meghana   (1000) meghana   (1000)       53 2024-06-02 19:15:16.000000 meghana_hello_world-0.3/README.md
+drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:42:39.384110 meghana_hello_world-0.3/meghana_hello_world/
+-rw-r--r--   0 meghana   (1000) meghana   (1000)       77 2024-06-02 21:42:14.000000 meghana_hello_world-0.3/meghana_hello_world/__init__.py
+-rw-r--r--   0 meghana   (1000) meghana   (1000)      225 2024-06-02 21:02:13.000000 meghana_hello_world-0.3/meghana_hello_world/cli.py
+drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:42:39.384110 meghana_hello_world-0.3/meghana_hello_world.egg-info/
+-rw-r--r--   0 meghana   (1000) meghana   (1000)      196 2024-06-02 21:42:39.000000 meghana_hello_world-0.3/meghana_hello_world.egg-info/PKG-INFO
+-rw-r--r--   0 meghana   (1000) meghana   (1000)      393 2024-06-02 21:42:39.000000 meghana_hello_world-0.3/meghana_hello_world.egg-info/SOURCES.txt
+-rw-r--r--   0 meghana   (1000) meghana   (1000)        1 2024-06-02 21:42:39.000000 meghana_hello_world-0.3/meghana_hello_world.egg-info/dependency_links.txt
+-rw-r--r--   0 meghana   (1000) meghana   (1000)       70 2024-06-02 21:42:39.000000 meghana_hello_world-0.3/meghana_hello_world.egg-info/entry_points.txt
+-rw-r--r--   0 meghana   (1000) meghana   (1000)        6 2024-06-02 21:42:39.000000 meghana_hello_world-0.3/meghana_hello_world.egg-info/requires.txt
+-rw-r--r--   0 meghana   (1000) meghana   (1000)       20 2024-06-02 21:42:39.000000 meghana_hello_world-0.3/meghana_hello_world.egg-info/top_level.txt
+-rw-r--r--   0 meghana   (1000) meghana   (1000)       79 2024-06-02 21:42:39.394110 meghana_hello_world-0.3/setup.cfg
+-rw-r--r--   0 meghana   (1000) meghana   (1000)      457 2024-06-02 21:42:07.000000 meghana_hello_world-0.3/setup.py
+drwxr-xr-x   0 meghana   (1000) meghana   (1000)        0 2024-06-02 21:42:39.384110 meghana_hello_world-0.3/tests/
+-rw-r--r--   0 meghana   (1000) meghana   (1000)      128 2024-06-02 21:02:09.000000 meghana_hello_world-0.3/tests/test_hello_world.py
```

