# Comparing `tmp/blockchain_data_subnet_shared_libs-0.0.9.tar.gz` & `tmp/blockchain_data_subnet_shared_libs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain_data_subnet_shared_libs-0.0.9.tar", last modified: Sun Jun  2 10:16:22 2024, max compression
+gzip compressed data, was "blockchain_data_subnet_shared_libs-1.0.0.tar", last modified: Thu May 30 19:41:18 2024, max compression
```

## Comparing `blockchain_data_subnet_shared_libs-0.0.9.tar` & `blockchain_data_subnet_shared_libs-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:16:22.058147 blockchain_data_subnet_shared_libs-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 10:16:13.000000 blockchain_data_subnet_shared_libs-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-06-02 10:16:22.054147 blockchain_data_subnet_shared_libs-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-02 10:16:13.000000 blockchain_data_subnet_shared_libs-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:16:22.054147 blockchain_data_subnet_shared_libs-0.0.9/blockchain_data_subnet_shared_libs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-06-02 10:16:22.000000 blockchain_data_subnet_shared_libs-0.0.9/blockchain_data_subnet_shared_libs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-02 10:16:22.000000 blockchain_data_subnet_shared_libs-0.0.9/blockchain_data_subnet_shared_libs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:16:22.000000 blockchain_data_subnet_shared_libs-0.0.9/blockchain_data_subnet_shared_libs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 10:16:22.000000 blockchain_data_subnet_shared_libs-0.0.9/blockchain_data_subnet_shared_libs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 10:16:22.000000 blockchain_data_subnet_shared_libs-0.0.9/blockchain_data_subnet_shared_libs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:16:22.054147 blockchain_data_subnet_shared_libs-0.0.9/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:16:13.000000 blockchain_data_subnet_shared_libs-0.0.9/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 10:16:13.000000 blockchain_data_subnet_shared_libs-0.0.9/protocols/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-02 10:16:13.000000 blockchain_data_subnet_shared_libs-0.0.9/protocols/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-06-02 10:16:13.000000 blockchain_data_subnet_shared_libs-0.0.9/protocols/llm_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:16:22.058147 blockchain_data_subnet_shared_libs-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-06-02 10:16:13.000000 blockchain_data_subnet_shared_libs-0.0.9/setup.py
+drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/
+-rw-r--r--   0 saroot    (1000) saroot    (1000)     1069 2024-05-30 19:18:28.000000 blockchain_data_subnet_shared_libs-1.0.0/LICENSE
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      543 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/PKG-INFO
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      131 2024-05-30 15:27:10.000000 blockchain_data_subnet_shared_libs-1.0.0/README.md
+drwxr-xr-x   0 saroot    (1000) saroot    (1000)        0 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      543 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/PKG-INFO
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      315 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)       19 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/requires.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)        1 2024-05-30 19:41:18.000000 blockchain_data_subnet_shared_libs-1.0.0/blockchain_data_subnet_shared_libs.egg-info/top_level.txt
+-rw-r--r--   0 saroot    (1000) saroot    (1000)       38 2024-05-30 19:41:18.859880 blockchain_data_subnet_shared_libs-1.0.0/setup.cfg
+-rw-r--r--   0 saroot    (1000) saroot    (1000)      735 2024-05-30 19:39:11.000000 blockchain_data_subnet_shared_libs-1.0.0/setup.py
```

### Comparing `blockchain_data_subnet_shared_libs-0.0.9/LICENSE` & `blockchain_data_subnet_shared_libs-1.0.0/LICENSE`

 * *Files identical despite different names*
