# Comparing `tmp/poetry_plugin_dynamic_override_sources-0.0.1.tar.gz` & `tmp/poetry_plugin_dynamic_override_sources-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.1.tar", max compression
+gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.2.tar", max compression
```

## Comparing `poetry_plugin_dynamic_override_sources-0.0.1.tar` & `poetry_plugin_dynamic_override_sources-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.1/LICENSE
--rw-r--r--   0        0        0     1122 2024-06-01 12:59:14.244338 poetry_plugin_dynamic_override_sources-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.1/src/poetry_plugin_dynamic_override_sources/__init__.py
--rw-r--r--   0        0        0     4657 2024-06-01 13:50:42.708327 poetry_plugin_dynamic_override_sources-0.0.1/src/poetry_plugin_dynamic_override_sources/plugins.py
--rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.1/src/poetry_plugin_dynamic_override_sources/py.typed
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1721 2024-05-31 22:20:13.349991 poetry_plugin_dynamic_override_sources-0.0.2/README.md
+-rw-r--r--   0        0        0     1204 2024-06-01 14:21:58.990883 poetry_plugin_dynamic_override_sources-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/__init__.py
+-rw-r--r--   0        0        0     4657 2024-06-01 13:50:42.708327 poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/plugins.py
+-rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/py.typed
+-rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.2/PKG-INFO
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.1/LICENSE` & `poetry_plugin_dynamic_override_sources-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dynamic_override_sources-0.0.1/pyproject.toml` & `poetry_plugin_dynamic_override_sources-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "poetry-plugin-dynamic-override-sources"
-version = "0.0.1"
+version = "0.0.2"
 description = "Poetry plugin to dynamically override sources for private mirroring"
 authors = [
   "Jacob Henner <code@ventricle.us>",
   "Hugh Baxter <hughdbaxter@gmail.com>",
   "Dustin Burke <dustin@datarobot.com>",
 ]
+readme = "README.md"
+
 license = "BSD-3-Clause"
 keywords = ["packaging", "poetry", "pypi", "pip"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 poetry = ">=1.6.0,<2"
 
@@ -22,14 +24,19 @@
 mypy = "^0.982"
 bandit = "^1.7.4"
 isort = "^5.10.1"
 flake8 = "^3.9.2"
 pre-commit = "^2.20.0"
 pytest = "^8.2.1"
 
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
+
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 src_paths = ["src/poetry_plugin_dynamic_override_sources", "tests"]
 
 [tool.pylint.messages_control]
 disable = "C0330, C0326"
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.1/src/poetry_plugin_dynamic_override_sources/plugins.py` & `poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/plugins.py`

 * *Files identical despite different names*

