# Comparing `tmp/rl_tasks-0.1.0.tar.gz` & `tmp/rl_tasks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_tasks-0.1.0.tar", last modified: Sun Jun  2 13:44:16 2024, max compression
+gzip compressed data, was "rl_tasks-0.1.1.tar", last modified: Sun Jun  2 14:56:58 2024, max compression
```

## Comparing `rl_tasks-0.1.0.tar` & `rl_tasks-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:44:16.384577 rl_tasks-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 13:44:16.384577 rl_tasks-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:44:16.384577 rl_tasks-0.1.0/rl_tasks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 13:44:16.000000 rl_tasks-0.1.0/rl_tasks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-02 13:44:16.000000 rl_tasks-0.1.0/rl_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:44:16.000000 rl_tasks-0.1.0/rl_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 13:44:16.000000 rl_tasks-0.1.0/rl_tasks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:44:16.000000 rl_tasks-0.1.0/rl_tasks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 13:44:16.384577 rl_tasks-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-02 13:44:06.000000 rl_tasks-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/rl_tasks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:56:58.000000 rl_tasks-0.1.1/rl_tasks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 14:56:58.949850 rl_tasks-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-02 14:56:36.000000 rl_tasks-0.1.1/setup.py
```

