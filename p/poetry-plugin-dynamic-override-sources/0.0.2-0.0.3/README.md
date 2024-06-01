# Comparing `tmp/poetry_plugin_dynamic_override_sources-0.0.2.tar.gz` & `tmp/poetry_plugin_dynamic_override_sources-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.2.tar", max compression
+gzip compressed data, was "poetry_plugin_dynamic_override_sources-0.0.3.tar", max compression
```

## Comparing `poetry_plugin_dynamic_override_sources-0.0.2.tar` & `poetry_plugin_dynamic_override_sources-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.2/LICENSE
--rw-r--r--   0        0        0     1721 2024-05-31 22:20:13.349991 poetry_plugin_dynamic_override_sources-0.0.2/README.md
--rw-r--r--   0        0        0     1204 2024-06-01 14:21:58.990883 poetry_plugin_dynamic_override_sources-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/__init__.py
--rw-r--r--   0        0        0     4657 2024-06-01 13:50:42.708327 poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/plugins.py
--rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/py.typed
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      338 2024-06-01 22:34:46.741361 poetry_plugin_dynamic_override_sources-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1457 2024-05-31 18:18:47.890274 poetry_plugin_dynamic_override_sources-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1923 2024-06-01 22:35:16.987504 poetry_plugin_dynamic_override_sources-0.0.3/README.md
+-rw-r--r--   0        0        0     1231 2024-06-01 22:17:19.323392 poetry_plugin_dynamic_override_sources-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 18:14:15.366535 poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/__init__.py
+-rw-r--r--   0        0        0     4757 2024-06-01 22:34:40.772440 poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/plugins.py
+-rw-r--r--   0        0        0       48 2024-05-31 18:14:15.367108 poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/py.typed
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 poetry_plugin_dynamic_override_sources-0.0.3/PKG-INFO
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.2/LICENSE` & `poetry_plugin_dynamic_override_sources-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dynamic_override_sources-0.0.2/README.md` & `poetry_plugin_dynamic_override_sources-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,44 +12,46 @@
 - `PIP_PROXY`
 
 However, with poetry there is no such option.  The pyproject.toml project configuration specifies one or more
 [sources](https://python-poetry.org/docs/repositories/#package-sources) that are to be used for resolving packages from the artifact storage.
 
 This plugin makes it possible to use environment variable overrides like:
 
-- `PIP_INDEX_URL` will override `PyPI` source
-- `POETRY_SOURCE_FOO_URL` will override the source named `FOO` with the specified url
+- `PIP_INDEX_URL` will override ALL repository urls, intending to function similar to `pip install --index-url`
+- `POETRY_SOURCE_SOME_REPO_URL` will override the source named `some-repo` with the specified url
+- `POETRY_SOURCE_PYPI_URL` will override the `PyPI` repository's URL.  This is a special case.
 
 ## Usage
 
 ### Installation
 
 See [plugin installation instructions](https://python-poetry.org/docs/plugins#using-plugins).
 
 ```bash
 $POETRY_HOME/bin/pip install --user git+https://github.com/burkestar/poetry-plugin-dynamic-override-sources
 ```
 
-### Configuration
-
-
-
 ## Development
 
 Setup
 
 ```bash
 poetry install
 ```
 
 Testing
 
 ```bash
 poetry run pytest
 ```
 
+## Publishing
+
+```bash
+poetry publish --build
+```
 
 ## Links
 
 - [poetry-plugin-use-pip-global-index-url](https://github.com/BaxHugh/poetry-plugin-use-pip-global-index-url) - plugin that this was forked from
 - [poetry-plugin-pypi-mirror](https://github.com/arcesium/poetry-plugin-pypi-mirror) - upstream plugin that inspired `poetry-plugin-use-pip-global-index-url`.
 - [python-poetry/poetry#1632](https://github.com/python-poetry/poetry/issues/1632) - poetry feature request to add support for global repository URL replacement
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.2/pyproject.toml` & `poetry_plugin_dynamic_override_sources-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "poetry-plugin-dynamic-override-sources"
-version = "0.0.2"
+version = "0.0.3"
 description = "Poetry plugin to dynamically override sources for private mirroring"
 authors = [
+  "Dustin Burke <dustin@datarobot.com>",
   "Jacob Henner <code@ventricle.us>",
   "Hugh Baxter <hughdbaxter@gmail.com>",
-  "Dustin Burke <dustin@datarobot.com>",
 ]
 readme = "README.md"
+include = ["CHANGELOG.md"]
 
 license = "BSD-3-Clause"
 keywords = ["packaging", "poetry", "pypi", "pip"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 poetry = ">=1.6.0,<2"
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.2/src/poetry_plugin_dynamic_override_sources/plugins.py` & `poetry_plugin_dynamic_override_sources-0.0.3/src/poetry_plugin_dynamic_override_sources/plugins.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,68 +7,73 @@
 from poetry.config.config import Config
 from poetry.core.constraints.version import Version
 from poetry.core.packages.package import Package
 from poetry.plugins.plugin import Plugin
 from poetry.poetry import Poetry
 from poetry.repositories.legacy_repository import LegacyRepository
 from poetry.repositories.pypi_repository import PyPiRepository
-from poetry.repositories.repository_pool import Priority
+from poetry.repositories.repository_pool import PrioritizedRepository, Priority
 
 PYPI_SOURCE = 'PyPI'
 
 
 def parse_environment_variables() -> dict:
     """ Parse environment variables for configuration of source URLs.
 
-    `PIP_INDEX_URL` will override PyPI source
     `POETRY_SOURCE_FOO_URL` will override the URL for source `FOO`
     """
     source_urls = {}
 
     for key, val in os.environ.items():
-        if key == 'PIP_INDEX_URL':
-            source_urls[PYPI_SOURCE] = val
-
-        match = re.match('^POETRY_SOURCE_(.*)_URL', key)
+        match = re.match('^POETRY_SOURCE_(.*)_URL$', key)
         if match:
             source_name = match.groups()[0].lower().replace('_', '-')
+
+            if source_name == 'pypi':
+                # this is a special case
+                source_name = PYPI_SOURCE
+
             source_urls[source_name] = val
 
     return source_urls
 
 
 class DynamicOverrideSourcesPlugin(Plugin):
-    # If pypi.org and common mirroring/pull-through-cache software used the same
-    # standard API this plugin could simply modify the URL used by
-    # PyPiRepository. Unfortunately, PyPiRepository uses the unstable
-    # non-standard warehouse JSON API. To ensure maximum mirror compatibility
-    # through standards compliance we replace the pypi.org PyPiRepository with a
-    # (modified) LegacyRepository - which uses the PEP 503 API.
+    """
+    Allow dynamic overrides of repository URLs from environment variables.
+
+    For mirror compatibility, LegacyRepository (PEP 503 API) is used instead of PyPiRepository.
+    """
     def activate(self, poetry: Poetry, io: IO):
 
+        pip_index_url = os.environ.get('PIP_INDEX_URL')
+
         source_urls = parse_environment_variables()
 
-        for source_name, url in source_urls.items():
-            # get the existing repository
-            repo = poetry.pool._repositories.get(source_name)
-            if repo is None:
-                continue
-
-            # remove the existing repo and then add a new one to replace it
-            poetry.pool.remove_repository(source_name)
-            poetry.pool.add_repository(
-                repository=SourceStrippedLegacyRepository(
-                    source_name,
-                    url,
-                    config=poetry.config,
-                    disable_cache=repo.repository._disable_cache,
-                ),
-                default=(repo.priority == Priority.DEFAULT),
-                secondary=(repo.priority == Priority.SECONDARY),
-            )
+        for prioritized_repo in poetry.pool._sorted_repositories:
+            repo = prioritized_repo.repository
+
+            # if pip_index_url is set, override all repository urls.
+            # otherwise, only override repository urls for those with an env var set.
+            replace_with_url = pip_index_url if pip_index_url else source_urls.get(repo.name)
+
+            if replace_with_url:
+                # remove the existing repo and then add a new one to replace it
+                poetry.pool.remove_repository(repo.name)
+                poetry.pool.add_repository(
+                    repository=SourceStrippedLegacyRepository(
+                        repo.name,
+                        replace_with_url,
+                        config=poetry.config,
+                        disable_cache=getattr(repo, '_disable_cache', None),
+                    ),
+                    default=(prioritized_repo.priority == Priority.DEFAULT),
+                    secondary=(prioritized_repo.priority == Priority.SECONDARY),
+                )
+
 
 class SourceStrippedLegacyRepository(LegacyRepository):
     def __init__(
         self,
         name: str,
         url: str,
         config: Config | None = None,
```

### Comparing `poetry_plugin_dynamic_override_sources-0.0.2/PKG-INFO` & `poetry_plugin_dynamic_override_sources-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dynamic-override-sources
-Version: 0.0.2
+Version: 0.0.3
 Summary: Poetry plugin to dynamically override sources for private mirroring
 License: BSD-3-Clause
 Keywords: packaging,poetry,pypi,pip
-Author: Jacob Henner
-Author-email: code@ventricle.us
+Author: Dustin Burke
+Author-email: dustin@datarobot.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,45 +30,47 @@
 - `PIP_PROXY`
 
 However, with poetry there is no such option.  The pyproject.toml project configuration specifies one or more
 [sources](https://python-poetry.org/docs/repositories/#package-sources) that are to be used for resolving packages from the artifact storage.
 
 This plugin makes it possible to use environment variable overrides like:
 
-- `PIP_INDEX_URL` will override `PyPI` source
-- `POETRY_SOURCE_FOO_URL` will override the source named `FOO` with the specified url
+- `PIP_INDEX_URL` will override ALL repository urls, intending to function similar to `pip install --index-url`
+- `POETRY_SOURCE_SOME_REPO_URL` will override the source named `some-repo` with the specified url
+- `POETRY_SOURCE_PYPI_URL` will override the `PyPI` repository's URL.  This is a special case.
 
 ## Usage
 
 ### Installation
 
 See [plugin installation instructions](https://python-poetry.org/docs/plugins#using-plugins).
 
 ```bash
 $POETRY_HOME/bin/pip install --user git+https://github.com/burkestar/poetry-plugin-dynamic-override-sources
 ```
 
-### Configuration
-
-
-
 ## Development
 
 Setup
 
 ```bash
 poetry install
 ```
 
 Testing
 
 ```bash
 poetry run pytest
 ```
 
+## Publishing
+
+```bash
+poetry publish --build
+```
 
 ## Links
 
 - [poetry-plugin-use-pip-global-index-url](https://github.com/BaxHugh/poetry-plugin-use-pip-global-index-url) - plugin that this was forked from
 - [poetry-plugin-pypi-mirror](https://github.com/arcesium/poetry-plugin-pypi-mirror) - upstream plugin that inspired `poetry-plugin-use-pip-global-index-url`.
 - [python-poetry/poetry#1632](https://github.com/python-poetry/poetry/issues/1632) - poetry feature request to add support for global repository URL replacement
```

