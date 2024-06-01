# Comparing `tmp/poetry_plugin_dynamic_override_sources-0.0.3.tar.gz` & `tmp/poetry_plugin_dynamic_override_sources-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.3.tar", max compression
+gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.4.tar", max compression
```

## Comparing `poetry_plugin_dynamic_override_sources-0.0.3.tar` & `poetry_plugin_dynamic_override_sources-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      338 2024-06-01 22:34:46.741361 poetry_plugin_dynamic_override_sources-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.3/LICENSE
--rw-r--r--   0        0        0     1923 2024-06-01 22:35:16.987504 poetry_plugin_dynamic_override_sources-0.0.3/README.md
--rw-r--r--   0        0        0     1231 2024-06-01 22:17:19.323392 poetry_plugin_dynamic_override_sources-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/__init__.py
--rw-r--r--   0        0        0     4757 2024-06-01 22:34:40.772440 poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/plugins.py
--rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/py.typed
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      435 2024-06-01 22:38:21.438642 poetry_plugin_dynamic_override_sources-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1870 2024-06-01 22:37:35.520167 poetry_plugin_dynamic_override_sources-0.0.4/README.md
+-rw-r--r--   0        0        0     1231 2024-06-01 22:38:27.105087 poetry_plugin_dynamic_override_sources-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/__init__.py
+-rw-r--r--   0        0        0     4757 2024-06-01 22:34:40.772440 poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/plugins.py
+-rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/py.typed
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.4/PKG-INFO
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.3/LICENSE` & `poetry_plugin_dynamic_override_sources-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dynamic_override_sources-0.0.3/README.md` & `poetry_plugin_dynamic_override_sources-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 - `POETRY_SOURCE_SOME_REPO_URL` will override the source named `some-repo` with the specified url
 - `POETRY_SOURCE_PYPI_URL` will override the `PyPI` repository's URL.  This is a special case.
 
 ## Usage
 
 ### Installation
 
-See [plugin installation instructions](https://python-poetry.org/docs/plugins#using-plugins).
-
 ```bash
-$POETRY_HOME/bin/pip install --user git+https://github.com/burkestar/poetry-plugin-dynamic-override-sources
+poetry self add poetry-plugin-dynamic-override-sources
 ```
 
+See [plugin installation instructions](https://python-poetry.org/docs/plugins#using-plugins).
+
 ## Development
 
 Setup
 
 ```bash
 poetry install
 ```
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.3/pyproject.toml` & `poetry_plugin_dynamic_override_sources-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dynamic-override-sources"
-version = "0.0.3"
+version = "0.0.4"
 description = "Poetry plugin to dynamically override sources for private mirroring"
 authors = [
   "Dustin Burke <dustin@datarobot.com>",
   "Jacob Henner <code@ventricle.us>",
   "Hugh Baxter <hughdbaxter@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/plugins.py` & `poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dynamic_override_sources-0.0.3/PKG-INFO` & `poetry_plugin_dynamic_override_sources-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dynamic-override-sources
-Version: 0.0.3
+Version: 0.0.4
 Summary: Poetry plugin to dynamically override sources for private mirroring
 License: BSD-3-Clause
 Keywords: packaging,poetry,pypi,pip
 Author: Dustin Burke
 Author-email: dustin@datarobot.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -38,20 +38,20 @@
 - `POETRY_SOURCE_SOME_REPO_URL` will override the source named `some-repo` with the specified url
 - `POETRY_SOURCE_PYPI_URL` will override the `PyPI` repository's URL.  This is a special case.
 
 ## Usage
 
 ### Installation
 
-See [plugin installation instructions](https://python-poetry.org/docs/plugins#using-plugins).
-
 ```bash
-$POETRY_HOME/bin/pip install --user git+https://github.com/burkestar/poetry-plugin-dynamic-override-sources
+poetry self add poetry-plugin-dynamic-override-sources
 ```
 
+See [plugin installation instructions](https://python-poetry.org/docs/plugins#using-plugins).
+
 ## Development
 
 Setup
 
 ```bash
 poetry install
 ```
```

