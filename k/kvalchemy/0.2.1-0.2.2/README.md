# Comparing `tmp/kvalchemy-0.2.1.tar.gz` & `tmp/kvalchemy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvalchemy-0.2.1.tar", last modified: Sat Jun  1 18:34:21 2024, max compression
+gzip compressed data, was "kvalchemy-0.2.2.tar", last modified: Sat Jun  1 23:34:57 2024, max compression
```

## Comparing `kvalchemy-0.2.1.tar` & `kvalchemy-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.723262 kvalchemy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/kvalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/kvalchemy/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/kvalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 18:34:21.000000 kvalchemy-0.2.1/kvalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:34:21.723262 kvalchemy-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:34:21.719262 kvalchemy-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-06-01 18:34:05.000000 kvalchemy-0.2.1/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:34:57.823126 kvalchemy-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-06-01 23:34:57.823126 kvalchemy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:34:57.819126 kvalchemy-0.2.2/kvalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/kvalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/kvalchemy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/kvalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/kvalchemy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/kvalchemy/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/kvalchemy/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:34:57.819126 kvalchemy-0.2.2/kvalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-06-01 23:34:57.000000 kvalchemy-0.2.2/kvalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-01 23:34:57.000000 kvalchemy-0.2.2/kvalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 23:34:57.000000 kvalchemy-0.2.2/kvalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 23:34:57.000000 kvalchemy-0.2.2/kvalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 23:34:57.000000 kvalchemy-0.2.2/kvalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:34:57.823126 kvalchemy-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:34:57.819126 kvalchemy-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-06-01 23:34:47.000000 kvalchemy-0.2.2/tests/test_time.py
```

### Comparing `kvalchemy-0.2.1/LICENSE.md` & `kvalchemy-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/PKG-INFO` & `kvalchemy-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Requires-Dist: psycopg2-binary; extra == "dev"
 Requires-Dist: PyMySQL[rsa]; extra == "dev"
 Requires-Dist: pymssql; platform_system != "Darwin" and extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # KVAlchemy
 
-[![PyPI version](https://badge.fury.io/py/kvalchemy.svg)](https://badge.fury.io/py/kvalchemy)
+[![PyPI version](https://badge.fury.io/py/kvalchemy.svg?dummy=unused)](https://badge.fury.io/py/kvalchemy?dummy=unused)
 
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
 
 ```
 from kvalchemy import KVAlchemy
```

### Comparing `kvalchemy-0.2.1/README.md` & `kvalchemy-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # KVAlchemy
 
-[![PyPI version](https://badge.fury.io/py/kvalchemy.svg)](https://badge.fury.io/py/kvalchemy)
+[![PyPI version](https://badge.fury.io/py/kvalchemy.svg?dummy=unused)](https://badge.fury.io/py/kvalchemy?dummy=unused)
 
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
 
 ```
 from kvalchemy import KVAlchemy
```

### Comparing `kvalchemy-0.2.1/kvalchemy/client.py` & `kvalchemy-0.2.2/kvalchemy/client.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/kvalchemy/models.py` & `kvalchemy-0.2.2/kvalchemy/models.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/kvalchemy/proxy.py` & `kvalchemy-0.2.2/kvalchemy/proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/kvalchemy/time.py` & `kvalchemy-0.2.2/kvalchemy/time.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/kvalchemy.egg-info/PKG-INFO` & `kvalchemy-0.2.2/kvalchemy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Requires-Dist: psycopg2-binary; extra == "dev"
 Requires-Dist: PyMySQL[rsa]; extra == "dev"
 Requires-Dist: pymssql; platform_system != "Darwin" and extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # KVAlchemy
 
-[![PyPI version](https://badge.fury.io/py/kvalchemy.svg)](https://badge.fury.io/py/kvalchemy)
+[![PyPI version](https://badge.fury.io/py/kvalchemy.svg?dummy=unused)](https://badge.fury.io/py/kvalchemy?dummy=unused)
 
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
 
 ```
 from kvalchemy import KVAlchemy
```

### Comparing `kvalchemy-0.2.1/pyproject.toml` & `kvalchemy-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/tests/test_client.py` & `kvalchemy-0.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/tests/test_proxy.py` & `kvalchemy-0.2.2/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.2.1/tests/test_time.py` & `kvalchemy-0.2.2/tests/test_time.py`

 * *Files identical despite different names*

