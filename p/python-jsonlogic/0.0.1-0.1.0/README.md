# Comparing `tmp/python-jsonlogic-0.0.1.tar.gz` & `tmp/python_jsonlogic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-jsonlogic-0.0.1.tar", last modified: Tue Mar 12 18:23:17 2024, max compression
+gzip compressed data, was "python_jsonlogic-0.1.0.tar", last modified: Sun Jun  2 20:25:51 2024, max compression
```

## Comparing `python-jsonlogic-0.0.1.tar` & `python_jsonlogic-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,43 @@
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-12 18:23:17.267374 python-jsonlogic-0.0.1/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1066 2024-03-12 17:41:18.000000 python-jsonlogic-0.0.1/LICENSE
--rw-r--r--   0 victorien  (1000) victorien  (1000)     2850 2024-03-12 18:23:17.267374 python-jsonlogic-0.0.1/PKG-INFO
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      651 2024-03-12 17:56:23.000000 python-jsonlogic-0.0.1/README.rst
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1871 2024-03-12 18:22:01.000000 python-jsonlogic-0.0.1/pyproject.toml
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       38 2024-03-12 18:23:17.267374 python-jsonlogic-0.0.1/setup.cfg
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-12 18:23:17.259374 python-jsonlogic-0.0.1/src/
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-12 18:23:17.263374 python-jsonlogic-0.0.1/src/jsonlogic/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-03-06 16:53:41.000000 python-jsonlogic-0.0.1/src/jsonlogic/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      219 2024-03-11 19:17:28.000000 python-jsonlogic-0.0.1/src/jsonlogic/_compat.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2268 2024-03-12 17:52:28.000000 python-jsonlogic-0.0.1/src/jsonlogic/core.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-12 18:23:17.263374 python-jsonlogic-0.0.1/src/jsonlogic/json_schema/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1750 2024-03-11 14:07:57.000000 python-jsonlogic-0.0.1/src/jsonlogic/json_schema/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1741 2024-03-12 17:50:55.000000 python-jsonlogic-0.0.1/src/jsonlogic/json_schema/resolvers.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     3755 2024-03-11 19:13:41.000000 python-jsonlogic-0.0.1/src/jsonlogic/json_schema/types.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-12 18:23:17.267374 python-jsonlogic-0.0.1/src/jsonlogic/operators/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      661 2024-03-12 17:45:53.000000 python-jsonlogic-0.0.1/src/jsonlogic/operators/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-03-12 08:19:54.000000 python-jsonlogic-0.0.1/src/jsonlogic/operators/base.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     5240 2024-03-12 17:51:11.000000 python-jsonlogic-0.0.1/src/jsonlogic/operators/operators.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      548 2024-03-12 08:42:58.000000 python-jsonlogic-0.0.1/src/jsonlogic/operators/typechecking.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-03-06 18:59:04.000000 python-jsonlogic-0.0.1/src/jsonlogic/py.typed
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2871 2024-03-12 17:45:26.000000 python-jsonlogic-0.0.1/src/jsonlogic/registry.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      601 2024-03-12 17:45:32.000000 python-jsonlogic-0.0.1/src/jsonlogic/typing.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      260 2024-03-11 19:01:20.000000 python-jsonlogic-0.0.1/src/jsonlogic/utils.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-03-12 18:23:17.267374 python-jsonlogic-0.0.1/src/python_jsonlogic.egg-info/
--rw-r--r--   0 victorien  (1000) victorien  (1000)     2850 2024-03-12 18:23:17.000000 python-jsonlogic-0.0.1/src/python_jsonlogic.egg-info/PKG-INFO
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      678 2024-03-12 18:23:17.000000 python-jsonlogic-0.0.1/src/python_jsonlogic.egg-info/SOURCES.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        1 2024-03-12 18:23:17.000000 python-jsonlogic-0.0.1/src/python_jsonlogic.egg-info/dependency_links.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       53 2024-03-12 18:23:17.000000 python-jsonlogic-0.0.1/src/python_jsonlogic.egg-info/requires.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       10 2024-03-12 18:23:17.000000 python-jsonlogic-0.0.1/src/python_jsonlogic.egg-info/top_level.txt
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.043913 python_jsonlogic-0.1.0/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1066 2024-03-12 17:41:18.000000 python_jsonlogic-0.1.0/LICENSE
+-rw-r--r--   0 victorien  (1000) victorien  (1000)     5258 2024-06-02 20:25:51.043913 python_jsonlogic-0.1.0/PKG-INFO
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3058 2024-05-30 07:49:04.000000 python_jsonlogic-0.1.0/README.rst
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2005 2024-06-02 20:25:02.000000 python_jsonlogic-0.1.0/pyproject.toml
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       38 2024-06-02 20:25:51.043913 python_jsonlogic-0.1.0/setup.cfg
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.039913 python_jsonlogic-0.1.0/src/
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.039913 python_jsonlogic-0.1.0/src/jsonlogic/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      141 2024-03-17 17:23:05.000000 python_jsonlogic-0.1.0/src/jsonlogic/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      339 2024-04-25 19:54:17.000000 python_jsonlogic-0.1.0/src/jsonlogic/_compat.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4655 2024-06-02 20:20:57.000000 python_jsonlogic-0.1.0/src/jsonlogic/core.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.039913 python_jsonlogic-0.1.0/src/jsonlogic/evaluation/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      221 2024-05-29 08:20:15.000000 python_jsonlogic-0.1.0/src/jsonlogic/evaluation/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3153 2024-05-29 08:20:15.000000 python_jsonlogic-0.1.0/src/jsonlogic/evaluation/evaluation_context.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4295 2024-05-15 12:14:24.000000 python_jsonlogic-0.1.0/src/jsonlogic/evaluation/evaluation_settings.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2442 2024-06-02 20:20:57.000000 python_jsonlogic-0.1.0/src/jsonlogic/evaluation/utils.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.039913 python_jsonlogic-0.1.0/src/jsonlogic/json_schema/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     6080 2024-05-27 18:54:26.000000 python_jsonlogic-0.1.0/src/jsonlogic/json_schema/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)    11608 2024-05-29 09:22:06.000000 python_jsonlogic-0.1.0/src/jsonlogic/json_schema/types.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.039913 python_jsonlogic-0.1.0/src/jsonlogic/operators/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1151 2024-04-07 16:37:26.000000 python_jsonlogic-0.1.0/src/jsonlogic/operators/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)    12811 2024-06-02 20:02:10.000000 python_jsonlogic-0.1.0/src/jsonlogic/operators/operators.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-03-06 18:59:04.000000 python_jsonlogic-0.1.0/src/jsonlogic/py.typed
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4397 2024-04-25 19:54:17.000000 python_jsonlogic-0.1.0/src/jsonlogic/registry.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     6208 2024-05-07 17:24:56.000000 python_jsonlogic-0.1.0/src/jsonlogic/resolving.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.043913 python_jsonlogic-0.1.0/src/jsonlogic/typechecking/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      416 2024-04-17 07:53:27.000000 python_jsonlogic-0.1.0/src/jsonlogic/typechecking/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1027 2024-04-17 07:53:27.000000 python_jsonlogic-0.1.0/src/jsonlogic/typechecking/diagnostics.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2773 2024-05-29 08:20:15.000000 python_jsonlogic-0.1.0/src/jsonlogic/typechecking/typecheck_context.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     7465 2024-04-25 19:54:17.000000 python_jsonlogic-0.1.0/src/jsonlogic/typechecking/typecheck_settings.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2042 2024-06-02 20:20:57.000000 python_jsonlogic-0.1.0/src/jsonlogic/typechecking/utils.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1455 2024-06-02 20:20:57.000000 python_jsonlogic-0.1.0/src/jsonlogic/typing.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1055 2024-05-07 17:24:56.000000 python_jsonlogic-0.1.0/src/jsonlogic/utils.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.043913 python_jsonlogic-0.1.0/src/python_jsonlogic.egg-info/
+-rw-r--r--   0 victorien  (1000) victorien  (1000)     5258 2024-06-02 20:25:51.000000 python_jsonlogic-0.1.0/src/python_jsonlogic.egg-info/PKG-INFO
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1057 2024-06-02 20:25:51.000000 python_jsonlogic-0.1.0/src/python_jsonlogic.egg-info/SOURCES.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        1 2024-06-02 20:25:51.000000 python_jsonlogic-0.1.0/src/python_jsonlogic.egg-info/dependency_links.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       54 2024-06-02 20:25:51.000000 python_jsonlogic-0.1.0/src/python_jsonlogic.egg-info/requires.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       10 2024-06-02 20:25:51.000000 python_jsonlogic-0.1.0/src/python_jsonlogic.egg-info/top_level.txt
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-06-02 20:25:51.043913 python_jsonlogic-0.1.0/tests/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      325 2024-06-02 20:20:57.000000 python_jsonlogic-0.1.0/tests/test_json_logic_expression.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2047 2024-03-25 17:05:39.000000 python_jsonlogic-0.1.0/tests/test_registry.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3860 2024-05-30 07:49:04.000000 python_jsonlogic-0.1.0/tests/test_resolving.py
```

### Comparing `python-jsonlogic-0.0.1/LICENSE` & `python_jsonlogic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-jsonlogic-0.0.1/pyproject.toml` & `python_jsonlogic-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-jsonlogic"
 description = "An extensible and sane implementation of JsonLogic"
-version = "0.0.1"
+version = "0.1.0"
 readme = "README.rst"
 authors = [
     {name = "Victorien", email = "contact@vctrn.dev"}
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
@@ -24,15 +24,15 @@
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 dependencies = [
-    "typing-extensions>=4.6.0; python_version < '3.12'",
+    "typing-extensions>=4.10.0; python_version < '3.13'",
 ]
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
@@ -42,14 +42,15 @@
 
 [tool.ruff]
 line-length = 120
 src = ["src"]
 target-version = "py38"
 
 [tool.ruff.lint]
+typing-modules = ["_compat"]
 preview = true
 explicit-preview-rules = true
 select = [
     "E",      # pycodestyle (E)
     "W",      # pycodestyle (W)
     "F",      # Pyflakes
     "UP",     # pyupgrade
@@ -57,18 +58,23 @@
     "PL",     # Pylint
     "RUF",    # Ruff
     "RUF022", # Ruff-preview
     "YTT",    # flake8-2020
     "B",      # flake8-bugbear
     "C4",     # flake8-comprehensions
     "T10",    # flake8-debugger
+    "FA",     # flake8-future-annotations
     "PIE",    # flake8-pie
     "T20",    # flake8-print
     "RSE",    # flake8-raise
     "PTH",    # flake8-use-pathlib
 ]
 ignore = [
-    "PLR2004"
+    "PLR2004",
+    "PLR0911",
 ]
 
 [tool.ruff.lint.isort]
 known-first-party = ["jsonlogic"]
+
+[tool.pytest.ini_options]
+pythonpath = "src"
```

### Comparing `python-jsonlogic-0.0.1/src/python_jsonlogic.egg-info/SOURCES.txt` & `python_jsonlogic-0.1.0/src/python_jsonlogic.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,31 @@
 README.rst
 pyproject.toml
 src/jsonlogic/__init__.py
 src/jsonlogic/_compat.py
 src/jsonlogic/core.py
 src/jsonlogic/py.typed
 src/jsonlogic/registry.py
+src/jsonlogic/resolving.py
 src/jsonlogic/typing.py
 src/jsonlogic/utils.py
+src/jsonlogic/evaluation/__init__.py
+src/jsonlogic/evaluation/evaluation_context.py
+src/jsonlogic/evaluation/evaluation_settings.py
+src/jsonlogic/evaluation/utils.py
 src/jsonlogic/json_schema/__init__.py
-src/jsonlogic/json_schema/resolvers.py
 src/jsonlogic/json_schema/types.py
 src/jsonlogic/operators/__init__.py
-src/jsonlogic/operators/base.py
 src/jsonlogic/operators/operators.py
-src/jsonlogic/operators/typechecking.py
+src/jsonlogic/typechecking/__init__.py
+src/jsonlogic/typechecking/diagnostics.py
+src/jsonlogic/typechecking/typecheck_context.py
+src/jsonlogic/typechecking/typecheck_settings.py
+src/jsonlogic/typechecking/utils.py
 src/python_jsonlogic.egg-info/PKG-INFO
 src/python_jsonlogic.egg-info/SOURCES.txt
 src/python_jsonlogic.egg-info/dependency_links.txt
 src/python_jsonlogic.egg-info/requires.txt
-src/python_jsonlogic.egg-info/top_level.txt
+src/python_jsonlogic.egg-info/top_level.txt
+tests/test_json_logic_expression.py
+tests/test_registry.py
+tests/test_resolving.py
```

