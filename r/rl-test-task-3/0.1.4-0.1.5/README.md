# Comparing `tmp/rl_test_task_3-0.1.4.tar.gz` & `tmp/rl_test_task_3-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_test_task_3-0.1.4.tar", last modified: Sun Jun  2 15:34:12 2024, max compression
+gzip compressed data, was "rl_test_task_3-0.1.5.tar", last modified: Sun Jun  2 15:54:35 2024, max compression
```

## Comparing `rl_test_task_3-0.1.4.tar` & `rl_test_task_3-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.410346 rl_test_task_3-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:34:12.410346 rl_test_task_3-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.410346 rl_test_task_3-0.1.4/rl_test_task_3/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 15:33:53.000000 rl_test_task_3-0.1.4/rl_test_task_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-06-02 15:33:53.000000 rl_test_task_3-0.1.4/rl_test_task_3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.410346 rl_test_task_3-0.1.4/rl_test_task_3/data_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 15:33:53.000000 rl_test_task_3-0.1.4/rl_test_task_3/data_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-02 15:33:53.000000 rl_test_task_3-0.1.4/rl_test_task_3/data_parsers/input_data_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.410346 rl_test_task_3-0.1.4/rl_test_task_3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:34:12.000000 rl_test_task_3-0.1.4/rl_test_task_3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 15:34:12.000000 rl_test_task_3-0.1.4/rl_test_task_3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:34:12.000000 rl_test_task_3-0.1.4/rl_test_task_3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 15:34:12.000000 rl_test_task_3-0.1.4/rl_test_task_3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 15:34:12.000000 rl_test_task_3-0.1.4/rl_test_task_3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:34:12.410346 rl_test_task_3-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-02 15:33:53.000000 rl_test_task_3-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:54:35.097713 rl_test_task_3-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:54:35.097713 rl_test_task_3-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:54:35.097713 rl_test_task_3-0.1.5/rl_test_task_3/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 15:54:16.000000 rl_test_task_3-0.1.5/rl_test_task_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-06-02 15:54:16.000000 rl_test_task_3-0.1.5/rl_test_task_3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:54:35.097713 rl_test_task_3-0.1.5/rl_test_task_3/data_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 15:54:16.000000 rl_test_task_3-0.1.5/rl_test_task_3/data_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-02 15:54:16.000000 rl_test_task_3-0.1.5/rl_test_task_3/data_parsers/input_data_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:54:35.097713 rl_test_task_3-0.1.5/rl_test_task_3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:54:35.000000 rl_test_task_3-0.1.5/rl_test_task_3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 15:54:35.000000 rl_test_task_3-0.1.5/rl_test_task_3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:54:35.000000 rl_test_task_3-0.1.5/rl_test_task_3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 15:54:35.000000 rl_test_task_3-0.1.5/rl_test_task_3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 15:54:35.000000 rl_test_task_3-0.1.5/rl_test_task_3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:54:35.097713 rl_test_task_3-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-02 15:54:16.000000 rl_test_task_3-0.1.5/setup.py
```

### Comparing `rl_test_task_3-0.1.4/rl_test_task_3/client.py` & `rl_test_task_3-0.1.5/rl_test_task_3/client.py`

 * *Files identical despite different names*

