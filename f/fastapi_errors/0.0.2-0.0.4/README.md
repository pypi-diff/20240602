# Comparing `tmp/fastapi_errors-0.0.2.tar.gz` & `tmp/fastapi_errors-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_errors-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_errors-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_errors-0.0.2.tar` & `fastapi_errors-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3098 2024-06-02 11:02:59.594955 fastapi_errors-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2024-06-02 10:02:52.157296 fastapi_errors-0.0.2/LICENSE
--rw-r--r--   0        0        0       11 2024-06-02 11:29:43.608392 fastapi_errors-0.0.2/README.md
--rw-r--r--   0        0        0       51 2024-06-02 11:30:11.661565 fastapi_errors-0.0.2/fastapi_errors/__init__.py
--rw-r--r--   0        0        0     2635 2024-06-02 10:05:25.182230 fastapi_errors-0.0.2/fastapi_errors/exceptions.py
--rw-r--r--   0        0        0     2667 2024-06-02 11:01:45.209799 fastapi_errors-0.0.2/fastapi_errors/generator.py
--rw-r--r--   0        0        0      343 2024-06-02 10:11:42.838293 fastapi_errors-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      189 1970-01-01 00:00:00.000000 fastapi_errors-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3098 2024-06-02 11:02:59.594955 fastapi_errors-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2024-06-02 10:02:52.157296 fastapi_errors-0.0.4/LICENSE
+-rw-r--r--   0        0        0       11 2024-06-02 11:32:42.679564 fastapi_errors-0.0.4/README.md
+-rw-r--r--   0        0        0       51 2024-06-02 11:32:51.895915 fastapi_errors-0.0.4/fastapi_errors/__init__.py
+-rw-r--r--   0        0        0     2635 2024-06-02 10:05:25.182230 fastapi_errors-0.0.4/fastapi_errors/exceptions.py
+-rw-r--r--   0        0        0     2667 2024-06-02 11:01:45.209799 fastapi_errors-0.0.4/fastapi_errors/generator.py
+-rw-r--r--   0        0        0      363 2024-06-02 11:32:42.683564 fastapi_errors-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      242 1970-01-01 00:00:00.000000 fastapi_errors-0.0.4/PKG-INFO
```

### Comparing `fastapi_errors-0.0.2/.gitignore` & `fastapi_errors-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_errors-0.0.2/LICENSE` & `fastapi_errors-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_errors-0.0.2/fastapi_errors/exceptions.py` & `fastapi_errors-0.0.4/fastapi_errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_errors-0.0.2/fastapi_errors/generator.py` & `fastapi_errors-0.0.4/fastapi_errors/generator.py`

 * *Files identical despite different names*

