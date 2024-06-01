# Comparing `tmp/pytest_publish-1.0.0.tar.gz` & `tmp/pytest_publish-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_publish-1.0.0.tar", max compression
+gzip compressed data, was "pytest_publish-1.1.0.tar", max compression
```

## Comparing `pytest_publish-1.0.0.tar` & `pytest_publish-1.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1263 2024-05-25 23:45:33.617705 pytest_publish-1.0.0/README.md
--rw-r--r--   0        0        0      735 2024-05-25 23:45:45.226185 pytest_publish-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1415 2024-05-25 23:45:33.619371 pytest_publish-1.0.0/pytest_publish.py
--rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 pytest_publish-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2045 2024-06-01 23:38:15.343543 pytest_publish-1.1.0/README.md
+-rw-r--r--   0        0        0      784 2024-06-01 23:38:31.448317 pytest_publish-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6806 2024-06-01 23:38:15.345296 pytest_publish-1.1.0/pytest_publish.py
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 pytest_publish-1.1.0/PKG-INFO
```

### Comparing `pytest_publish-1.0.0/pyproject.toml` & `pytest_publish-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "pytest-publish"
-version = "1.0.0"
+version = "1.1.0"
 description = ""
 authors = ["Yuvalino <yuvalino@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest = "^8.0.0"
 requests = "^2.32.2"
+dataclasses-json = "^0.6.6"
+filelock = "^3.14.0"
 
 
 [tool.poetry.group.dev.dependencies]
 flask = "^3.0.3"
 werkzeug = "^3.0.3"
-pytest-xdist = "^3.6.1"
 pre-commit = "^3.5"
 types-requests = "^2.32.0.20240523"
+pytest-xdist = "^3.6.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins]
 pytest11 = { pytest_publish = "pytest_publish"}
```

