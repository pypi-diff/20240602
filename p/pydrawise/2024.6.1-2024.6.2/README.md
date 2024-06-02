# Comparing `tmp/pydrawise-2024.6.1.tar.gz` & `tmp/pydrawise-2024.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2024.6.1.tar", last modified: Sat Jun  1 14:20:06 2024, max compression
+gzip compressed data, was "pydrawise-2024.6.2.tar", last modified: Sun Jun  2 15:08:22 2024, max compression
```

## Comparing `pydrawise-2024.6.1.tar` & `pydrawise-2024.6.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.440162 pydrawise-2024.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.440162 pydrawise-2024.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/reference/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    55590 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/hydrawise.graphql
--rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/scripts/setup
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25747 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.926378 pydrawise-2024.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.918377 pydrawise-2024.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.918377 pydrawise-2024.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.918377 pydrawise-2024.6.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-02 15:08:22.926378 pydrawise-2024.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.922378 pydrawise-2024.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.922378 pydrawise-2024.6.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/docs/reference/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.922378 pydrawise-2024.6.2/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-02 15:08:22.000000 pydrawise-2024.6.2/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55590 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/hydrawise.graphql
+-rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17750 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pydrawise/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.926378 pydrawise-2024.6.2/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-02 15:08:22.000000 pydrawise-2024.6.2/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-06-02 15:08:22.000000 pydrawise-2024.6.2/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:08:22.000000 pydrawise-2024.6.2/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 15:08:22.000000 pydrawise-2024.6.2/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 15:08:22.000000 pydrawise-2024.6.2/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:08:22.000000 pydrawise-2024.6.2/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.922378 pydrawise-2024.6.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/scripts/setup
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:08:22.926378 pydrawise-2024.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:22.926378 pydrawise-2024.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25738 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-02 15:08:09.000000 pydrawise-2024.6.2/tests/test_schema_utils.py
```

### Comparing `pydrawise-2024.6.1/.devcontainer.json` & `pydrawise-2024.6.2/.devcontainer.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666668%*

 * *Differences: {"'customizations'": "{'vscode': {'extensions': {insert: [(2, 'ms-python.mypy-type-checker')]}}}"}*

```diff
@@ -1,13 +1,14 @@
 {
     "customizations": {
         "vscode": {
             "extensions": [
                 "streetsidesoftware.code-spell-checker",
                 "github.vscode-pull-request-github",
+                "ms-python.mypy-type-checker",
                 "ms-python.python",
                 "ms-python.vscode-pylance",
                 "python.pylint"
             ],
             "settings": {
                 "editor.formatOnPaste": false,
                 "editor.formatOnSave": true,
```

### Comparing `pydrawise-2024.6.1/.github/workflows/build-and-test.yml` & `pydrawise-2024.6.2/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/.github/workflows/publish-python.yml` & `pydrawise-2024.6.2/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/.gitignore` & `pydrawise-2024.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/.pre-commit-config.yaml` & `pydrawise-2024.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/LICENSE` & `pydrawise-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/PKG-INFO` & `pydrawise-2024.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2024.6.1/README.md` & `pydrawise-2024.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/docs/index.md` & `pydrawise-2024.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/mkdocs.yml` & `pydrawise-2024.6.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pydrawise/__init__.py` & `pydrawise-2024.6.2/pydrawise/__init__.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pydrawise/auth.py` & `pydrawise-2024.6.2/pydrawise/auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pydrawise/base.py` & `pydrawise-2024.6.2/pydrawise/base.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pydrawise/client.py` & `pydrawise-2024.6.2/pydrawise/client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pydrawise/exceptions.py` & `pydrawise-2024.6.2/pydrawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pydrawise/hydrawise.graphql` & `pydrawise-2024.6.2/pydrawise/hydrawise.graphql`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pydrawise/legacy.py` & `pydrawise-2024.6.2/pydrawise/legacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """"API for interacting with Hydrawise sprinkler controllers.
 
 This library should remain compatible with https://github.com/ptcryan/hydrawiser.
  """
 
 from datetime import datetime, timedelta
 import time
+from typing import Any
 
 import aiohttp
 import requests
 
 from .base import HydrawiseBase
 from .exceptions import NotInitializedError, UnknownError
 from .schema import (
@@ -233,15 +234,15 @@
     next_run = None
     suspended_until = None
     if zone_json["time"] == 1:
         current_run = ScheduledZoneRun(
             remaining_time=timedelta(seconds=zone_json["run"]),
         )
     elif zone_json["time"] == 1576800000:
-        suspended_until = ZoneSuspension(end_time=datetime.max)
+        suspended_until = datetime.max
     else:
         now = datetime.now().replace(microsecond=0)
         start_time = now + timedelta(seconds=zone_json["time"])
         duration = timedelta(seconds=zone_json["run"])
         next_run = ScheduledZoneRun(
             start_time=start_time,
             end_time=start_time + duration,
@@ -266,16 +267,16 @@
     """Client library for interacting with Hydrawise v1 API.
 
     This should remain (mostly) compatible with https://github.com/ptcryan/hydrawiser
     """
 
     def __init__(self, user_token: str, load_on_init: bool = True) -> None:
         self._api_key = user_token
-        self.controller_info = {}
-        self.controller_status = {}
+        self.controller_info: dict[str, Any] = {}
+        self.controller_status: dict[str, Any] = {}
         if load_on_init:
             self.update_controller_info()
 
     @property
     def current_controller(self) -> dict:
         controllers = self.controller_info.get("controllers", [])
         if not controllers:
@@ -346,15 +347,15 @@
     def _get_controller_info(self) -> dict:
         return self._get("customerdetails.php", type="controllers")
 
     def _get_controller_status(self) -> dict:
         return self._get("statusschedule.php")
 
     def suspend_zone(self, days: int, zone: int | None = None) -> dict:
-        params = {}
+        params: dict[str, Any] = {}
 
         if days > 0:
             params["custom"] = int(time.time() + (days * 24 * 60 * 60))
             params["period_id"] = 999
         else:
             params["period_id"] = 0
 
@@ -366,15 +367,15 @@
             raise NotInitializedError("No zones loaded")
 
         params["action"] = "suspend"
         params["relay_id"] = self.relays_by_zone_number[zone]["relay_id"]
         return self._get("setzone.php", **params)
 
     def run_zone(self, minutes: int, zone: int | None = None) -> dict:
-        params = {}
+        params: dict[str, Any] = {}
 
         if zone is not None:
             if not self.relays:
                 raise NotInitializedError("No zones loaded")
             params["relay_id"] = self.relays_by_zone_number[zone]["relay_id"]
             params["action"] = "run" if minutes > 0 else "stop"
         else:
```

### Comparing `pydrawise-2024.6.1/pydrawise/schema.py` & `pydrawise-2024.6.2/pydrawise/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,21 +5,29 @@
 from dataclasses import dataclass, field
 from datetime import datetime, time, timedelta, timezone
 from enum import Enum, auto
 from typing import Optional, Union
 
 from apischema import type_name
 from apischema.conversions import Conversion
-from apischema.metadata import conversion
+from apischema.metadata import conversion, fall_back_on_default
 
 # The names in this file are from the GraphQL schema and don't always adhere to
 # the naming scheme that pylint expects.
 # pylint: disable=invalid-name
 
 
+def _optional_field(*args, **kwargs):
+    if "metadata" in kwargs:
+        kwargs["metadata"] |= fall_back_on_default
+    else:
+        kwargs["metadata"] = fall_back_on_default
+    return field(*args, **kwargs)
+
+
 def default_datetime() -> datetime:
     """Default datetime factory for fields in this module.
 
     Abstracted so it can be mocked out.
 
     :meta private:
     """
@@ -50,15 +58,15 @@
 
 
 def _time_conversion() -> conversion:
     return conversion(
         Conversion(
             lambda s: datetime.strptime(s, "%H:%M").time(), source=str, target=time
         ),
-        Conversion(lambda t: time.strftime("%H:%M"), source=time, target=str),
+        Conversion(lambda t: t.strftime("%H:%M"), source=time, target=str),
     )
 
 
 def _list_conversion(element_conversion) -> conversion:
     return conversion(
         Conversion(
             lambda l: list(map(element_conversion.deserialization.converter, l)),
@@ -96,24 +104,24 @@
     summary: str = ""
 
 
 @dataclass
 class LocalizedValueType:
     """A localized value."""
 
-    value: Optional[float] = 0.0
-    unit: Optional[str] = ""
+    value: float = _optional_field(default=0.0)
+    unit: str = _optional_field(default="")
 
 
 @dataclass
 class SelectedOption:
     """A generic option."""
 
     value: int = 0
-    label: Optional[str] = ""
+    label: str = _optional_field(default="")
 
 
 @dataclass
 class DateTime:
     """A date & time.
 
     This is only used for serialization and deserialization.
@@ -171,26 +179,26 @@
 
 
 @dataclass
 class RunTimeGroup:
     """The runtime of a watering program group."""
 
     id: int = 0
-    name: Optional[str] = ""
+    name: str = _optional_field(default="")
     duration: timedelta = field(
         metadata=_duration_conversion("minutes"), default=timedelta()
     )
 
 
 @dataclass
 class WateringPeriodicity:
     """Watering frequency description (e.g., "Every Program Start Time")."""
 
-    value: Optional[int] = 0
-    label: Optional[str] = ""
+    value: int = _optional_field(default=0)
+    label: str = _optional_field(default="")
 
 
 @dataclass
 class ProgramWateringFrequency:
     """Watering frequency information."""
 
     label: str = ""
@@ -232,18 +240,18 @@
 
 @dataclass
 class AdvancedProgram(Program):
     """An advanced watering program."""
 
     zone_specific: bool = False
     advanced_program_id: int = 0
-    watering_frequency: Optional[ProgramWateringFrequency] = field(
+    watering_frequency: ProgramWateringFrequency = _optional_field(
         default_factory=ProgramWateringFrequency
     )
-    run_time_group: Optional[RunTimeGroup] = field(default_factory=RunTimeGroup)
+    run_time_group: RunTimeGroup = _optional_field(default_factory=RunTimeGroup)
 
 
 class AdvancedProgramDayPatternEnum(_AutoEnum):
     """A value for an advanced watering program day pattern."""
 
     EVEN = auto()
     ODD = auto()
@@ -265,26 +273,26 @@
     cycle_and_soak_settings: Optional[CycleAndSoakSettings] = None
 
 
 @dataclass
 class AdvancedWateringSettings(WateringSettings):
     """Advanced watering program settings."""
 
-    advanced_program: AdvancedProgram = None
+    advanced_program: Optional[AdvancedProgram] = None
 
 
 @dataclass
 @type_name("Unit")
 class TimeRange:
     """Time range units."""
 
-    valid_from: Optional[datetime] = field(
+    valid_from: datetime = _optional_field(
         metadata=_timestamp_conversion(), default_factory=datetime
     )
-    valid_to: Optional[datetime] = field(
+    valid_to: datetime = _optional_field(
         metadata=_timestamp_conversion(), default_factory=datetime
     )
 
 
 @dataclass
 class StandardProgramPeriodicity:
     """Program frequency for a standard program."""
@@ -295,22 +303,22 @@
     )
 
 
 @dataclass
 class StandardProgram(Program):
     """A standard watering program."""
 
-    start_times: Optional[list[time]] = field(
+    start_times: list[time] = _optional_field(
         metadata=_list_conversion(_time_conversion()), default_factory=list
     )
     time_range: TimeRange = field(default_factory=TimeRange)
     ignore_rain_sensor: bool = False
     days_run: list[DaysOfWeekEnum] = field(default_factory=list)
     standard_program_day_pattern: str = ""
-    periodicity: Optional[StandardProgramPeriodicity] = field(
+    periodicity: StandardProgramPeriodicity = _optional_field(
         default_factory=StandardProgramPeriodicity
     )
 
 
 @dataclass
 class StandardProgramApplication:
     """A standard watering program application."""
@@ -329,23 +337,23 @@
     )
 
 
 @dataclass
 class RunStatus:
     """Run status."""
 
-    value: Optional[int] = 0
-    label: Optional[str] = ""
+    value: int = _optional_field(default=0)
+    label: str = _optional_field(default="")
 
 
 @dataclass
 class ScheduledZoneRun:
     """A scheduled zone run."""
 
-    id: str = 0
+    id: str = ""
     start_time: datetime = field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
     end_time: datetime = field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
     normal_duration: timedelta = field(
@@ -371,15 +379,15 @@
 
 
 @dataclass
 class PastZoneRuns:
     """Previous zone runs."""
 
     last_run: Optional[ScheduledZoneRun] = None
-    runs: Optional[list[ScheduledZoneRun]] = field(default_factory=list)
+    runs: list[ScheduledZoneRun] = _optional_field(default_factory=list)
 
 
 @dataclass
 class ZoneStatus:
     """A zone's status."""
 
     relative_water_balance: int = 0
@@ -389,18 +397,18 @@
 
 
 @dataclass
 class ZoneSuspension:
     """A zone suspension."""
 
     id: int = 0
-    start_time: Optional[datetime] = field(
+    start_time: datetime = _optional_field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
-    end_time: Optional[datetime] = field(
+    end_time: datetime = _optional_field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
 
 
 @dataclass
 class Zone(BaseZone):
     """A watering zone."""
@@ -415,56 +423,56 @@
 
 
 @dataclass
 class ProgramStartTimeApplication:
     """Application of a start time to a program."""
 
     all: bool = False
-    zones: Optional[list[BaseZone]] = field(default_factory=list)
+    zones: list[BaseZone] = _optional_field(default_factory=list)
 
 
 @dataclass
 class ProgramStartTime:
     """Start time for a watering program."""
 
     id: int = 0
     time: time = field(metadata=_time_conversion(), default_factory=time)
-    watering_days: Optional[list[AdvancedProgramDayPatternEnum]] = field(
+    watering_days: list[AdvancedProgramDayPatternEnum] = _optional_field(
         default_factory=list
     )
     application: ProgramStartTimeApplication = field(
         default_factory=ProgramStartTimeApplication
     )
 
 
 @dataclass
 class ControllerFirmware:
     """Information about the controller's firmware."""
 
     type: str = ""
-    version: Optional[str] = ""
+    version: str = _optional_field(default="")
 
 
 @dataclass
 class ControllerModel:
     """Information about a controller model."""
 
     name: str = ""
     description: str = ""
 
 
 @dataclass
 class ControllerHardware:
     """Information about a controller's hardware."""
 
-    serial_number: Optional[str] = ""
-    version: Optional[str] = ""
-    status: Optional[str] = ""
-    model: Optional[ControllerModel] = field(default_factory=ControllerModel)
-    firmware: Optional[list[ControllerFirmware]] = field(default_factory=list)
+    serial_number: str = _optional_field(default="")
+    version: str = _optional_field(default="")
+    status: str = _optional_field(default="")
+    model: ControllerModel = _optional_field(default_factory=ControllerModel)
+    firmware: list[ControllerFirmware] = _optional_field(default_factory=list)
 
 
 class CustomSensorTypeEnum(_AutoEnum):
     """A value for a sensor type."""
 
     LEVEL_OPEN = auto()
     LEVEL_CLOSED = auto()
@@ -473,39 +481,39 @@
 
 
 @dataclass
 class SensorModel:
     """Information about a sensor model."""
 
     id: int = 0
-    name: Optional[str] = ""
-    active: Optional[bool] = False
-    off_level: Optional[int] = 0
-    off_timer: Optional[int] = 0
-    delay: Optional[timedelta] = field(
+    name: str = _optional_field(default="")
+    active: bool = _optional_field(default=False)
+    off_level: int = _optional_field(default=0)
+    off_timer: int = _optional_field(default=0)
+    delay: timedelta = _optional_field(
         metadata=_duration_conversion("minutes"), default=timedelta()
     )
-    divisor: Optional[float] = 0.0
-    flow_rate: Optional[float] = 0.0
+    divisor: float = _optional_field(default=0.0)
+    flow_rate: float = _optional_field(default=0.0)
     sensor_type: Optional[CustomSensorTypeEnum] = None
 
 
 @dataclass
 class SensorStatus:
     """Current status of a sensor."""
 
     water_flow: Optional[LocalizedValueType] = None
-    active: Optional[bool] = False
+    active: bool = _optional_field(default=False)
 
 
 @dataclass
 class SensorFlowSummary:
     """Summary of a sensor's water flow."""
 
-    total_water_volume: Optional[LocalizedValueType] = field(
+    total_water_volume: LocalizedValueType = _optional_field(
         default_factory=LocalizedValueType
     )
 
 
 @dataclass
 class Sensor:
     """A sensor connected to a controller."""
@@ -516,15 +524,15 @@
     status: SensorStatus = field(default_factory=SensorStatus)
 
 
 @dataclass
 class _WaterTime:
     """A water time duration."""
 
-    value: Optional[timedelta] = field(
+    value: timedelta = _optional_field(
         metadata=_duration_conversion("minutes"), default=timedelta()
     )
 
 
 @dataclass
 class ActualWaterTime(_WaterTime):
     """An actual water time duration."""
@@ -537,18 +545,18 @@
 
 @dataclass
 class ControllerStatus:
     """Current status of a controller."""
 
     summary: str = ""
     online: bool = False
-    actual_water_time: Optional[ActualWaterTime] = field(
+    actual_water_time: ActualWaterTime = _optional_field(
         default_factory=ActualWaterTime
     )
-    normal_water_time: Optional[NormalWaterTime] = field(
+    normal_water_time: NormalWaterTime = _optional_field(
         default_factory=NormalWaterTime
     )
     last_contact: Optional[DateTime] = None
 
 
 @dataclass
 class RunStatusType:
@@ -565,80 +573,82 @@
 @dataclass
 @type_name("RunEventType")
 class RunEvent:
     """A Hydrawise run event type."""
 
     id: str = ""
     zone: BaseZone = field(default_factory=BaseZone)
-    standard_program: Optional[StandardProgramRef] = field(
+    standard_program: StandardProgramRef = _optional_field(
         default_factory=StandardProgramRef
     )
-    advanced_program: Optional[AdvancedProgramRef] = field(
+    advanced_program: AdvancedProgramRef = _optional_field(
         default_factory=AdvancedProgramRef
     )
     reported_start_time: Optional[datetime] = field(
         metadata=DateTime.conversion(), default=None
     )
     reported_end_time: Optional[datetime] = field(
         metadata=DateTime.conversion(), default=None
     )
-    reported_duration: Optional[int] = field(
+    reported_duration: timedelta = _optional_field(
         metadata=_duration_conversion("seconds"), default=timedelta()
     )
-    reported_status: Optional[RunStatusType] = field(default_factory=RunStatusType)
-    reported_water_usage: Optional[LocalizedValueType] = field(
+    reported_status: RunStatusType = _optional_field(default_factory=RunStatusType)
+    reported_water_usage: LocalizedValueType = _optional_field(
         default_factory=LocalizedValueType
     )
-    reported_stop_reason: Optional[RunStopReasonType] = field(
+    reported_stop_reason: RunStopReasonType = _optional_field(
         default_factory=RunStopReasonType
     )
-    reported_current: Optional[LocalizedValueType] = field(
+    reported_current: LocalizedValueType = _optional_field(
         default_factory=LocalizedValueType
     )
 
 
 @dataclass
 class WateringReportEntry:
     """A Hydrawise watering report entry."""
 
-    run_event: Optional[RunEvent] = field(default_factory=RunEvent)
+    run_event: RunEvent = _optional_field(
+        default_factory=RunEvent, metadata=fall_back_on_default
+    )
 
 
 @dataclass
 class Controller:
     """A Hydrawise controller."""
 
     id: int = 0
-    name: Optional[str] = ""
-    software_version: Optional[str] = ""
+    name: str = _optional_field(default="")
+    software_version: str = _optional_field(default="")
     hardware: ControllerHardware = field(default_factory=ControllerHardware)
-    last_contact_time: Optional[datetime] = field(
+    last_contact_time: datetime = _optional_field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
-    last_action: Optional[datetime] = field(
+    last_action: datetime = _optional_field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
-    online: Optional[bool] = False
-    sensors: Optional[list[Sensor]] = field(default_factory=list)
-    zones: Optional[list[Zone]] = field(default_factory=list)
-    permitted_program_start_times: Optional[list[ProgramStartTime]] = field(
+    online: bool = _optional_field(default=False)
+    sensors: list[Sensor] = _optional_field(default_factory=list)
+    zones: list[Zone] = _optional_field(default_factory=list)
+    permitted_program_start_times: list[ProgramStartTime] = _optional_field(
         default_factory=list
     )
-    status: ControllerStatus = None
+    status: Optional[ControllerStatus] = None
 
 
 @dataclass
 class User:
     """A Hydrawise user account."""
 
     id: int = 0
     customer_id: int = 0
     name: str = ""
-    email: Optional[str] = ""
-    controllers: Optional[list[Controller]] = field(default_factory=list)
+    email: str = _optional_field(default="")
+    controllers: list[Controller] = _optional_field(default_factory=list)
 
 
 class DaysOfWeekEnum(_AutoEnum):
     """All days of the week."""
 
     SUNDAY = auto()
     MONDAY = auto()
```

### Comparing `pydrawise-2024.6.1/pydrawise/schema_utils.py` & `pydrawise-2024.6.2/pydrawise/schema_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """Constructs GraphQL selectors for the given dataclass.
 
     :meta private:
     """
     ret = []
     skip_now, skip_later = parse_skip(skip_fields or [])
     for f in _fields(cls, skip_now):
-        dsl_field = getattr(getattr(ds, get_type_name(cls).graphql), f.name)
+        dsl_field = getattr(getattr(ds, get_type_name(cls).graphql), f.name)  # type: ignore[arg-type]
         if len(f.types) == 1:
             [f_type] = f.types
             if is_dataclass(f_type):
                 f_skip = skip_later.get(f.name, [])
                 ret.append(
                     getattr(dsl_field, "select")(*get_selectors(ds, f_type, f_skip))
                 )
@@ -96,30 +96,31 @@
             # This is a Union; we must pass an inline fragment for each type.
             sel_args = []
             for f_type in f.types:
                 if not is_dataclass(f_type):
                     raise NotImplementedError
                 sel_args.append(
                     DSLInlineFragment()
-                    .on(getattr(ds, get_type_name(f_type).graphql))
+                    .on(getattr(ds, get_type_name(f_type).graphql))  # type: ignore[arg-type]
                     .select(*get_selectors(ds, f_type))
                 )
             ret.append(getattr(dsl_field, "select")(*sel_args))
     return ret
 
 
 def parse_skip(skip: list[str] | None = None) -> tuple[list[str], dict[str, list[str]]]:
     """Converts a flat list of skip fields into (skip_now, skip_later).
 
     skip_now is a list of fields in the current scope to skip.
     skip_later is a list of descendant fields to skip.
 
     :meta private:
     """
-    now, later = [], {}
-    for item in skip:
+    now: list[str] = []
+    later: dict[str, list[str]] = {}
+    for item in skip or []:
         field, _, descendants = item.partition(".")
         if descendants:
             later.setdefault(field, []).append(descendants)
         else:
             now.append(field)
     return now, later
```

### Comparing `pydrawise-2024.6.1/pydrawise.egg-info/PKG-INFO` & `pydrawise-2024.6.2/pydrawise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2024.6.1/pydrawise.egg-info/SOURCES.txt` & `pydrawise-2024.6.2/pydrawise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/pyproject.toml` & `pydrawise-2024.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/tests/test_auth.py` & `pydrawise-2024.6.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/tests/test_client.py` & `pydrawise-2024.6.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.6.1/tests/test_legacy.py` & `pydrawise-2024.6.2/tests/test_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
                 assert current_run.remaining_time == timedelta(seconds=1788)
                 assert zones[1].scheduled_runs.next_run is None
 
                 assert zones[2].name == "Rotary - Front"
                 assert zones[2].number == 3
                 assert zones[2].scheduled_runs.current_run is None
                 assert zones[2].scheduled_runs.next_run is None
-                assert zones[2].status.suspended_until.end_time == datetime.max
+                assert zones[2].status.suspended_until == datetime.max
 
     async def test_start_zone(self, success_status: dict) -> None:
         """Test the start_zone method."""
         client = legacy.LegacyHydrawiseAsync(API_KEY)
         with aioresponses() as m:
             m.get(
                 re.compile("https://api.hydrawise.com/api/v1/setzone.php"),
```

