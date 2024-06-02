# Comparing `tmp/movoid_debug-1.0.1.tar.gz` & `tmp/movoid_debug-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_debug-1.0.1.tar", last modified: Sun May 19 19:06:11 2024, max compression
+gzip compressed data, was "movoid_debug-1.2.0.tar", last modified: Sun Jun  2 16:09:38 2024, max compression
```

## Comparing `movoid_debug-1.0.1.tar` & `movoid_debug-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:06:11.511475 movoid_debug-1.0.1/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_debug-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      242 2024-05-19 19:06:11.510475 movoid_debug-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_debug-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 19:06:11.500476 movoid_debug-1.0.1/movoid_debug/
--rw-rw-rw-   0        0        0      227 2024-05-19 18:30:33.000000 movoid_debug-1.0.1/movoid_debug/__init__.py
--rw-rw-rw-   0        0        0     1554 2024-05-19 17:52:46.000000 movoid_debug-1.0.1/movoid_debug/flow.py
--rw-rw-rw-   0        0        0     2169 2024-05-19 19:05:42.000000 movoid_debug-1.0.1/movoid_debug/simple_debug.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:06:11.509476 movoid_debug-1.0.1/movoid_debug.egg-info/
--rw-rw-rw-   0        0        0      242 2024-05-19 19:06:11.000000 movoid_debug-1.0.1/movoid_debug.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-19 19:06:11.000000 movoid_debug-1.0.1/movoid_debug.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:06:11.000000 movoid_debug-1.0.1/movoid_debug.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-19 19:06:11.000000 movoid_debug-1.0.1/movoid_debug.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-19 19:06:11.000000 movoid_debug-1.0.1/movoid_debug.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 19:06:11.511475 movoid_debug-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-05-19 19:05:42.000000 movoid_debug-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:09:38.533728 movoid_debug-1.2.0/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_debug-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      242 2024-06-02 16:09:38.532728 movoid_debug-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_debug-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 16:09:38.517509 movoid_debug-1.2.0/movoid_debug/
+-rw-rw-rw-   0        0        0      285 2024-06-02 16:08:36.000000 movoid_debug-1.2.0/movoid_debug/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:09:38.526664 movoid_debug-1.2.0/movoid_debug/flow/
+-rw-rw-rw-   0        0        0      221 2024-06-02 16:08:37.000000 movoid_debug-1.2.0/movoid_debug/flow/__init__.py
+-rw-rw-rw-   0        0        0     8912 2024-06-02 16:08:37.000000 movoid_debug-1.2.0/movoid_debug/flow/flow.py
+-rw-rw-rw-   0        0        0     2169 2024-05-19 19:05:42.000000 movoid_debug-1.2.0/movoid_debug/simple_debug.py
+-rw-rw-rw-   0        0        0     5742 2024-06-02 16:08:36.000000 movoid_debug-1.2.0/movoid_debug/simple_hot_pause.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:09:38.529034 movoid_debug-1.2.0/movoid_debug/simple_ui/
+-rw-rw-rw-   0        0        0      445 2024-06-02 16:08:37.000000 movoid_debug-1.2.0/movoid_debug/simple_ui/__init__.py
+-rw-rw-rw-   0        0        0     6558 2024-06-02 16:08:37.000000 movoid_debug-1.2.0/movoid_debug/simple_ui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:09:38.531725 movoid_debug-1.2.0/movoid_debug.egg-info/
+-rw-rw-rw-   0        0        0      242 2024-06-02 16:09:38.000000 movoid_debug-1.2.0/movoid_debug.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2024-06-02 16:09:38.000000 movoid_debug-1.2.0/movoid_debug.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 16:09:38.000000 movoid_debug-1.2.0/movoid_debug.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 16:09:38.000000 movoid_debug-1.2.0/movoid_debug.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-02 16:09:38.000000 movoid_debug-1.2.0/movoid_debug.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 16:09:38.533728 movoid_debug-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-06-02 16:09:10.000000 movoid_debug-1.2.0/setup.py
```

### Comparing `movoid_debug-1.0.1/movoid_debug/simple_debug.py` & `movoid_debug-1.2.0/movoid_debug/simple_debug.py`

 * *Files identical despite different names*

