# Comparing `tmp/rl_tasks-0.1.3.tar.gz` & `tmp/rl_tasks-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_tasks-0.1.3.tar", last modified: Sun Jun  2 15:13:25 2024, max compression
+gzip compressed data, was "rl_tasks-0.1.4.tar", last modified: Sun Jun  2 15:34:16 2024, max compression
```

## Comparing `rl_tasks-0.1.3.tar` & `rl_tasks-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:25.612667 rl_tasks-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 15:13:25.612667 rl_tasks-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:25.608667 rl_tasks-0.1.3/rl_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:25.608667 rl_tasks-0.1.3/rl_tasks/task_executors/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:25.608667 rl_tasks-0.1.3/rl_tasks/task_executors/base/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/base/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/base/task_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/base/task_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/task_1_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/task_2_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/rl_tasks/task_executors/task_3_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:25.612667 rl_tasks-0.1.3/rl_tasks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 15:13:25.000000 rl_tasks-0.1.3/rl_tasks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-06-02 15:13:25.000000 rl_tasks-0.1.3/rl_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:13:25.000000 rl_tasks-0.1.3/rl_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 15:13:25.000000 rl_tasks-0.1.3/rl_tasks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 15:13:25.000000 rl_tasks-0.1.3/rl_tasks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:13:25.612667 rl_tasks-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-02 15:13:02.000000 rl_tasks-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:16.838332 rl_tasks-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 15:34:16.838332 rl_tasks-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:16.834332 rl_tasks-0.1.4/rl_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:16.834332 rl_tasks-0.1.4/rl_tasks/task_executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:16.834332 rl_tasks-0.1.4/rl_tasks/task_executors/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/base/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/base/task_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/base/task_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/task_1_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/task_2_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/rl_tasks/task_executors/task_3_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:16.838332 rl_tasks-0.1.4/rl_tasks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 15:34:16.000000 rl_tasks-0.1.4/rl_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-06-02 15:34:16.000000 rl_tasks-0.1.4/rl_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:34:16.000000 rl_tasks-0.1.4/rl_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 15:34:16.000000 rl_tasks-0.1.4/rl_tasks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 15:34:16.000000 rl_tasks-0.1.4/rl_tasks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:34:16.838332 rl_tasks-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-02 15:33:53.000000 rl_tasks-0.1.4/setup.py
```

### Comparing `rl_tasks-0.1.3/rl_tasks/task_executors/base/task_chain.py` & `rl_tasks-0.1.4/rl_tasks/task_executors/base/task_chain.py`

 * *Files identical despite different names*

### Comparing `rl_tasks-0.1.3/rl_tasks/task_executors/task_2_executor.py` & `rl_tasks-0.1.4/rl_tasks/task_executors/task_2_executor.py`

 * *Files identical despite different names*

### Comparing `rl_tasks-0.1.3/rl_tasks.egg-info/SOURCES.txt` & `rl_tasks-0.1.4/rl_tasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

