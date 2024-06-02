# Comparing `tmp/poetry_plugin_dynamic_override_sources-0.0.4.tar.gz` & `tmp/poetry_plugin_dynamic_override_sources-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.4.tar", max compression
+gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.5.tar", max compression
```

## Comparing `poetry_plugin_dynamic_override_sources-0.0.4.tar` & `poetry_plugin_dynamic_override_sources-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      435 2024-06-01 22:38:21.438642 poetry_plugin_dynamic_override_sources-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.4/LICENSE
--rw-r--r--   0        0        0     1870 2024-06-01 22:37:35.520167 poetry_plugin_dynamic_override_sources-0.0.4/README.md
--rw-r--r--   0        0        0     1231 2024-06-01 22:38:27.105087 poetry_plugin_dynamic_override_sources-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/__init__.py
--rw-r--r--   0        0        0     4757 2024-06-01 22:34:40.772440 poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/plugins.py
--rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/py.typed
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      504 2024-06-01 22:43:51.242811 poetry_plugin_dynamic_override_sources-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1870 2024-06-01 22:37:35.520167 poetry_plugin_dynamic_override_sources-0.0.5/README.md
+-rw-r--r--   0        0        0     1441 2024-06-01 22:44:25.932479 poetry_plugin_dynamic_override_sources-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.5/src/poetry_plugin_dynamic_override_sources/__init__.py
+-rw-r--r--   0        0        0     4757 2024-06-01 22:34:40.772440 poetry_plugin_dynamic_override_sources-0.0.5/src/poetry_plugin_dynamic_override_sources/plugins.py
+-rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.5/src/poetry_plugin_dynamic_override_sources/py.typed
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.5/PKG-INFO
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.4/LICENSE` & `poetry_plugin_dynamic_override_sources-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dynamic_override_sources-0.0.4/README.md` & `poetry_plugin_dynamic_override_sources-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dynamic_override_sources-0.0.4/pyproject.toml` & `poetry_plugin_dynamic_override_sources-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [tool.poetry]
 name = "poetry-plugin-dynamic-override-sources"
-version = "0.0.4"
+version = "0.0.5"
 description = "Poetry plugin to dynamically override sources for private mirroring"
 authors = [
   "Dustin Burke <dustin@datarobot.com>",
   "Jacob Henner <code@ventricle.us>",
   "Hugh Baxter <hughdbaxter@gmail.com>",
 ]
+repository = "https://github.com/burkestar/poetry-plugin-dynamic-override-sources"
 readme = "README.md"
 include = ["CHANGELOG.md"]
 
 license = "BSD-3-Clause"
 keywords = ["packaging", "poetry", "pypi", "pip"]
 
+[tool.poetry.urls]
+"Changelog" = "https://github.com/burkestar/poetry-plugin-dynamic-override-sources/blob/main/CHANGELOG.md"
+
 [tool.poetry.dependencies]
 python = "^3.8"
 poetry = ">=1.6.0,<2"
 
 [tool.poetry.plugins."poetry.plugin"]
 demo = "poetry_plugin_dynamic_override_sources.plugins:DynamicOverrideSourcesPlugin"
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.4/src/poetry_plugin_dynamic_override_sources/plugins.py` & `poetry_plugin_dynamic_override_sources-0.0.5/src/poetry_plugin_dynamic_override_sources/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dynamic_override_sources-0.0.4/PKG-INFO` & `poetry_plugin_dynamic_override_sources-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dynamic-override-sources
-Version: 0.0.4
+Version: 0.0.5
 Summary: Poetry plugin to dynamically override sources for private mirroring
+Home-page: https://github.com/burkestar/poetry-plugin-dynamic-override-sources
 License: BSD-3-Clause
 Keywords: packaging,poetry,pypi,pip
 Author: Dustin Burke
 Author-email: dustin@datarobot.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poetry (>=1.6.0,<2)
+Project-URL: Changelog, https://github.com/burkestar/poetry-plugin-dynamic-override-sources/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/burkestar/poetry-plugin-dynamic-override-sources
 Description-Content-Type: text/markdown
 
 # poetry-plugin-dynamic-override-sources
 
 ## Description
 
 *poetry-plugin-dynamic-override-sources* is a [plugin](https://python-poetry.org/docs/master/plugins/)
```

