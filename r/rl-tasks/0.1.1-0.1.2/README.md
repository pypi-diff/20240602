# Comparing `tmp/rl_tasks-0.1.1.tar.gz` & `tmp/rl_tasks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_tasks-0.1.1.tar", last modified: Sun Jun  2 14:56:58 2024, max compression
+gzip compressed data, was "rl_tasks-0.1.2.tar", last modified: Sun Jun  2 15:08:30 2024, max compression
```

## Comparing `rl_tasks-0.1.1.tar` & `rl_tasks-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/rl_tasks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-02 14:56:36.000000 rl_tasks-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:30.287084 rl_tasks-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 15:08:30.287084 rl_tasks-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:30.283084 rl_tasks-0.1.2/rl_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:30.283084 rl_tasks-0.1.2/rl_tasks/task_executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:30.283084 rl_tasks-0.1.2/rl_tasks/task_executors/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/base/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/base/task_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/base/task_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/task_1_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/task_2_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/rl_tasks/task_executors/task_3_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:30.283084 rl_tasks-0.1.2/rl_tasks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 15:08:30.000000 rl_tasks-0.1.2/rl_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-06-02 15:08:30.000000 rl_tasks-0.1.2/rl_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:08:30.000000 rl_tasks-0.1.2/rl_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 15:08:30.000000 rl_tasks-0.1.2/rl_tasks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 15:08:30.000000 rl_tasks-0.1.2/rl_tasks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:08:30.287084 rl_tasks-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-02 15:08:06.000000 rl_tasks-0.1.2/setup.py
```

