# Comparing `tmp/numbsql-7.0.0.tar.gz` & `tmp/numbsql-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbsql-7.0.0.tar", max compression
+gzip compressed data, was "numbsql-7.1.0.tar", max compression
```

## Comparing `numbsql-7.0.0.tar` & `numbsql-7.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11352 2023-12-07 13:31:58.574823 numbsql-7.0.0/LICENSE
--rw-r--r--   0        0        0     2946 2023-12-07 13:31:58.574823 numbsql-7.0.0/README.md
--rw-r--r--   0        0        0     6956 2023-12-07 13:32:44.622743 numbsql-7.0.0/numbsql/__init__.py
--rw-r--r--   0        0        0     4772 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/aggregate.py
--rw-r--r--   0        0        0      991 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/exceptions.py
--rw-r--r--   0        0        0    18928 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/numbaext.py
--rw-r--r--   0        0        0     1971 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/scalar.py
--rw-r--r--   0        0        0     9247 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/sqlite.py
--rw-r--r--   0        0        0     2886 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/tests/conftest.py
--rw-r--r--   0        0        0    10499 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/tests/test_aggregate.py
--rw-r--r--   0        0        0     1091 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/tests/test_numbaext.py
--rw-r--r--   0        0        0     8356 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/tests/test_scalar.py
--rw-r--r--   0        0        0      202 2023-12-07 13:31:58.574823 numbsql-7.0.0/numbsql/tests/test_version.py
--rw-r--r--   0        0        0     1990 2023-12-07 13:32:47.190738 numbsql-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 numbsql-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11352 2024-06-02 12:12:44.337156 numbsql-7.1.0/LICENSE
+-rw-r--r--   0        0        0     2946 2024-06-02 12:12:44.337156 numbsql-7.1.0/README.md
+-rw-r--r--   0        0        0     6956 2024-06-02 12:13:58.697879 numbsql-7.1.0/numbsql/__init__.py
+-rw-r--r--   0        0        0     4772 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/aggregate.py
+-rw-r--r--   0        0        0      991 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/exceptions.py
+-rw-r--r--   0        0        0    18928 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/numbaext.py
+-rw-r--r--   0        0        0     1971 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/scalar.py
+-rw-r--r--   0        0        0     9247 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/sqlite.py
+-rw-r--r--   0        0        0     2886 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/tests/conftest.py
+-rw-r--r--   0        0        0    10499 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/tests/test_aggregate.py
+-rw-r--r--   0        0        0     1091 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/tests/test_numbaext.py
+-rw-r--r--   0        0        0     8356 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/tests/test_scalar.py
+-rw-r--r--   0        0        0      202 2024-06-02 12:12:44.337156 numbsql-7.1.0/numbsql/tests/test_version.py
+-rw-r--r--   0        0        0     1995 2024-06-02 12:14:02.085912 numbsql-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3768 1970-01-01 00:00:00.000000 numbsql-7.1.0/PKG-INFO
```

### Comparing `numbsql-7.0.0/LICENSE` & `numbsql-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/README.md` & `numbsql-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/__init__.py` & `numbsql-7.1.0/numbsql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 __all__ = (
     "create_function",
     "create_aggregate",
     "sqlite_udf",
     "sqlite_udaf",
 )
 
-__version__ = "7.0.0"
+__version__ = "7.1.0"
 
 
 def create_function(
     con: sqlite3.Connection,
     name: str,
     num_params: int,
     func: Callable[..., Any],
```

### Comparing `numbsql-7.0.0/numbsql/aggregate.py` & `numbsql-7.1.0/numbsql/aggregate.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/exceptions.py` & `numbsql-7.1.0/numbsql/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/numbaext.py` & `numbsql-7.1.0/numbsql/numbaext.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/scalar.py` & `numbsql-7.1.0/numbsql/scalar.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/sqlite.py` & `numbsql-7.1.0/numbsql/sqlite.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/tests/conftest.py` & `numbsql-7.1.0/numbsql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/tests/test_aggregate.py` & `numbsql-7.1.0/numbsql/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/tests/test_numbaext.py` & `numbsql-7.1.0/numbsql/tests/test_numbaext.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/numbsql/tests/test_scalar.py` & `numbsql-7.1.0/numbsql/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `numbsql-7.0.0/pyproject.toml` & `numbsql-7.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.poetry]
 name = "numbsql"
 homepage = "https://github.com/cpcloud/numbsql"
 repository = "https://github.com/cpcloud/numbsql"
-version = "7.0.0"
+version = "7.1.0"
 description = "JITted SQLite user-defined scalar and aggregate functions"
 readme = "README.md"
 authors = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 maintainers = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 classifiers = [
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
-llvmlite = ">=0.36,<0.42"
-numba = ">=0.53,<0.59"
+llvmlite = ">=0.36,<0.43"
+numba = ">=0.53,<0.60"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.22.0"
 mypy = "^1.1.1"
 packaging = "^23.0"
-pytest = "^7.2.2"
+pytest = "^8.0.0"
 pytest-benchmark = "^4.0.0"
 pytest-randomly = "^3.12.0"
 pytest-xdist = "^3.2.1"
-ruff = ">=0.1.7,<1"
+ruff = ">=0.4.7,<1"
 testbook = ">=0.4.2,<1"
 
-[tool.ruff]
+[tool.ruff.lint]
 ignore = ["E501"]
 
 [tool.pytest.ini_options]
 xfail_strict = true
 addopts = [
   "--ignore=.direnv",
   "--ignore=examples",
```

### Comparing `numbsql-7.0.0/PKG-INFO` & `numbsql-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: numbsql
-Version: 7.0.0
+Version: 7.1.0
 Summary: JITted SQLite user-defined scalar and aggregate functions
 Home-page: https://github.com/cpcloud/numbsql
 Author: Phillip Cloud
 Author-email: 417981+cpcloud@users.noreply.github.com
 Maintainer: Phillip Cloud
 Maintainer-email: 417981+cpcloud@users.noreply.github.com
 Requires-Python: >=3.9,<4
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: llvmlite (>=0.36,<0.42)
-Requires-Dist: numba (>=0.53,<0.59)
+Requires-Dist: llvmlite (>=0.36,<0.43)
+Requires-Dist: numba (>=0.53,<0.60)
 Project-URL: Repository, https://github.com/cpcloud/numbsql
 Description-Content-Type: text/markdown
 
 # Put some Numba in your SQLite
 
 ## Fair Warning
```

