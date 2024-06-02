# Comparing `tmp/paracelsus-0.5.2.tar.gz` & `tmp/paracelsus-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paracelsus-0.5.2.tar", last modified: Sun Apr 21 21:53:50 2024, max compression
+gzip compressed data, was "paracelsus-0.6.0.tar", last modified: Sun Jun  2 14:23:30 2024, max compression
```

## Comparing `paracelsus-0.5.2.tar` & `paracelsus-0.6.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.806193 paracelsus-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.798193 paracelsus-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.798193 paracelsus-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 21:53:27.000000 paracelsus-0.5.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 21:53:27.000000 paracelsus-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-21 21:53:50.806193 paracelsus-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-21 21:53:27.000000 paracelsus-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.798193 paracelsus-0.5.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.802193 paracelsus-0.5.2/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-21 21:53:27.000000 paracelsus-0.5.2/docs/dev/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-21 21:53:27.000000 paracelsus-0.5.2/docs/dev/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 21:53:27.000000 paracelsus-0.5.2/docs/dev/github.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 21:53:27.000000 paracelsus-0.5.2/docs/dev/pypi.md
--rw-r--r--   0 runner    (1001) docker     (127)    64875 2024-04-21 21:53:27.000000 paracelsus-0.5.2/docs/example.png
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-21 21:53:27.000000 paracelsus-0.5.2/makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.802193 paracelsus-0.5.2/paracelsus/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 21:53:50.000000 paracelsus-0.5.2/paracelsus/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/pyproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.802193 paracelsus-0.5.2/paracelsus/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/transformers/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/transformers/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-21 21:53:27.000000 paracelsus-0.5.2/paracelsus/transformers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.806193 paracelsus-0.5.2/paracelsus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-21 21:53:50.000000 paracelsus-0.5.2/paracelsus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-21 21:53:50.000000 paracelsus-0.5.2/paracelsus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:53:50.000000 paracelsus-0.5.2/paracelsus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 21:53:50.000000 paracelsus-0.5.2/paracelsus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 21:53:50.000000 paracelsus-0.5.2/paracelsus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 21:53:50.000000 paracelsus-0.5.2/paracelsus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-21 21:53:27.000000 paracelsus-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 21:53:50.806193 paracelsus-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.802193 paracelsus-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.802193 paracelsus-0.5.2/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/assets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.802193 paracelsus-0.5.2/tests/assets/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/assets/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/assets/example/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/assets/example/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/assets/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/test_pyproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:50.806193 paracelsus-0.5.2/tests/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/transformers/test_dot.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/transformers/test_mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 21:53:27.000000 paracelsus-0.5.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.809084 paracelsus-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.801084 paracelsus-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.801084 paracelsus-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-02 14:23:08.000000 paracelsus-0.6.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-02 14:23:08.000000 paracelsus-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-06-02 14:23:30.809084 paracelsus-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-06-02 14:23:08.000000 paracelsus-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.801084 paracelsus-0.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.801084 paracelsus-0.6.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-02 14:23:08.000000 paracelsus-0.6.0/docs/dev/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-02 14:23:08.000000 paracelsus-0.6.0/docs/dev/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 14:23:08.000000 paracelsus-0.6.0/docs/dev/github.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 14:23:08.000000 paracelsus-0.6.0/docs/dev/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)    64875 2024-06-02 14:23:08.000000 paracelsus-0.6.0/docs/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-06-02 14:23:08.000000 paracelsus-0.6.0/makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.801084 paracelsus-0.6.0/paracelsus/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-02 14:23:30.000000 paracelsus-0.6.0/paracelsus/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/pyproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.805084 paracelsus-0.6.0/paracelsus/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/transformers/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/transformers/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-02 14:23:08.000000 paracelsus-0.6.0/paracelsus/transformers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.805084 paracelsus-0.6.0/paracelsus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-06-02 14:23:30.000000 paracelsus-0.6.0/paracelsus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-02 14:23:30.000000 paracelsus-0.6.0/paracelsus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:23:30.000000 paracelsus-0.6.0/paracelsus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 14:23:30.000000 paracelsus-0.6.0/paracelsus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-02 14:23:30.000000 paracelsus-0.6.0/paracelsus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-02 14:23:30.000000 paracelsus-0.6.0/paracelsus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-02 14:23:08.000000 paracelsus-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 14:23:30.809084 paracelsus-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.805084 paracelsus-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.805084 paracelsus-0.6.0/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/assets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.805084 paracelsus-0.6.0/tests/assets/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/assets/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/assets/example/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/assets/example/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/assets/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/test_pyproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:30.805084 paracelsus-0.6.0/tests/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/transformers/test_dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/transformers/test_mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-02 14:23:08.000000 paracelsus-0.6.0/tests/utils.py
```

### Comparing `paracelsus-0.5.2/.github/workflows/pypi.yaml` & `paracelsus-0.6.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/.gitignore` & `paracelsus-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/.pre-commit-config.yaml` & `paracelsus-0.6.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 repos:
   - repo: local
     hooks:
       - id: pytest
         name: pytest
-        entry: make pytest_check
+        entry: make pytest
         language: system
         pass_filenames: false
       - id: ruff
         name: ruff
         entry: make ruff_check
         language: system
         pass_filenames: false
```

### Comparing `paracelsus-0.5.2/LICENSE` & `paracelsus-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/PKG-INFO` & `paracelsus-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracelsus
-Version: 0.5.2
+Version: 0.6.0
 Author: Robert Hafner
 License: MIT License
         
         Copyright (c) 2023, Robert Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -113,14 +113,33 @@
 
 This is equivalent to running this style of python import:
 
 ```python
 from example_app.models import *
 ```
 
+### Include or Exclude tables
+
+After importing the models, it is possible to select a subset of those models by using the `--exlude-tables` and `--include-tables` options.
+These are mutually exclusive options, the user can only provide inclusions or exclusions:
+
+```bash
+paracelsus graph example_app.models.base:Base \
+  --import-module "example_app.models.*" \
+  --exclude-tables "comments"
+```
+
+This is equivalent to:
+
+```bash
+paracelsus graph example_app.models.base:Base \
+  --import-module "example_app.models.*" \
+  --include-tables "users"
+  --include-tables "posts"
+```
 
 ### Generate Mermaid Diagrams
 
 
 > paracelsus graph example_app.models.base:Base --import-module "example_app.models:*"
 
 ```text
```

### Comparing `paracelsus-0.5.2/README.md` & `paracelsus-0.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -67,14 +67,33 @@
 
 This is equivalent to running this style of python import:
 
 ```python
 from example_app.models import *
 ```
 
+### Include or Exclude tables
+
+After importing the models, it is possible to select a subset of those models by using the `--exlude-tables` and `--include-tables` options.
+These are mutually exclusive options, the user can only provide inclusions or exclusions:
+
+```bash
+paracelsus graph example_app.models.base:Base \
+  --import-module "example_app.models.*" \
+  --exclude-tables "comments"
+```
+
+This is equivalent to:
+
+```bash
+paracelsus graph example_app.models.base:Base \
+  --import-module "example_app.models.*" \
+  --include-tables "users"
+  --include-tables "posts"
+```
 
 ### Generate Mermaid Diagrams
 
 
 > paracelsus graph example_app.models.base:Base --import-module "example_app.models:*"
 
 ```text
```

### Comparing `paracelsus-0.5.2/docs/example.png` & `paracelsus-0.6.0/docs/example.png`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/makefile` & `paracelsus-0.6.0/makefile`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/paracelsus/cli.py` & `paracelsus-0.6.0/paracelsus/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,22 @@
     ] = None,
     import_module: Annotated[
         List[str],
         typer.Option(
             help="Module, typically an SQL Model, to import. Modules that end in :* will act as `from module import *`"
         ),
     ] = [],
+    exclude_tables: Annotated[
+        List[str],
+        typer.Option(help="List of tables that are excluded from the graph"),
+    ] = [],
+    include_tables: Annotated[
+        List[str],
+        typer.Option(help="List of tables that are included in the graph"),
+    ] = [],
     python_dir: Annotated[
         List[Path],
         typer.Option(
             help="Paths to add to the `PYTHON_PATH` for module lookup.",
             file_okay=False,
             dir_okay=True,
             resolve_path=True,
@@ -62,14 +70,16 @@
     if settings and "imports" in settings:
         import_module.extend(settings["imports"])
 
     typer.echo(
         get_graph_string(
             base_class_path=base_class,
             import_module=import_module,
+            include_tables=set(include_tables),
+            exclude_tables=set(exclude_tables),
             python_dir=python_dir,
             format=format.value,
         )
     )
 
 
 @app.command(help="Create a graph and inject it as a code field into a markdown file.")
@@ -98,14 +108,22 @@
     ] = "<!-- END_SQLALCHEMY_DOCS -->",
     import_module: Annotated[
         List[str],
         typer.Option(
             help="Module, typically an SQL Model, to import. Modules that end in :* will act as `from module import *`"
         ),
     ] = [],
+    exclude_tables: Annotated[
+        List[str],
+        typer.Option(help="List of tables that are excluded from the graph"),
+    ] = [],
+    include_tables: Annotated[
+        List[str],
+        typer.Option(help="List of tables that are included in the graph"),
+    ] = [],
     python_dir: Annotated[
         List[Path],
         typer.Option(
             help="Paths to add to the `PYTHON_PATH` for module lookup.",
             file_okay=False,
             dir_okay=True,
             resolve_path=True,
@@ -123,14 +141,16 @@
         ),
     ] = False,
 ):
     # Generate Graph
     graph = get_graph_string(
         base_class_path=base_class_path,
         import_module=import_module,
+        include_tables=set(include_tables),
+        exclude_tables=set(exclude_tables),
         python_dir=python_dir,
         format=format.value,
     )
 
     comment_format = transformers[format].comment_format  # type: ignore
 
     # Convert Graph to Injection String
```

### Comparing `paracelsus-0.5.2/paracelsus/transformers/mermaid.py` & `paracelsus-0.6.0/paracelsus/transformers/mermaid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import logging
 from sqlalchemy.sql.schema import Column, MetaData, Table
 
 from . import utils
 
 
+logger = logging.getLogger(__name__)
+
+
 class Mermaid:
     comment_format: str = "mermaid"
     metadata: MetaData
 
     def __init__(self, metaclass: MetaData) -> None:
         self.metadata = metaclass
 
@@ -60,14 +64,23 @@
 
         for foreign_key in column.foreign_keys:
             key_parts = foreign_key.target_fullname.split(".")
             left_table = key_parts[0]
             left_column = key_parts[1]
             left_operand = ""
 
+            # We don't add the connection to the fk table if the latter
+            # is not included in our graph.
+            if left_table not in self.metadata.tables:
+                logger.warning(
+                    f"Table '{right_table}.{column_name}' is a foreign key to '{left_table}' "
+                    "which is not included in the graph, skipping the connection."
+                )
+                continue
+
             lcolumn = self.metadata.tables[left_table].columns[left_column]
             if lcolumn.unique or lcolumn.primary_key:
                 left_operand = "||"
             else:
                 left_operand = "}o"
 
             output += f"  {left_table} {left_operand}--{right_operand} {right_table} : {column_name}\n"
```

### Comparing `paracelsus-0.5.2/paracelsus.egg-info/PKG-INFO` & `paracelsus-0.6.0/paracelsus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracelsus
-Version: 0.5.2
+Version: 0.6.0
 Author: Robert Hafner
 License: MIT License
         
         Copyright (c) 2023, Robert Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -113,14 +113,33 @@
 
 This is equivalent to running this style of python import:
 
 ```python
 from example_app.models import *
 ```
 
+### Include or Exclude tables
+
+After importing the models, it is possible to select a subset of those models by using the `--exlude-tables` and `--include-tables` options.
+These are mutually exclusive options, the user can only provide inclusions or exclusions:
+
+```bash
+paracelsus graph example_app.models.base:Base \
+  --import-module "example_app.models.*" \
+  --exclude-tables "comments"
+```
+
+This is equivalent to:
+
+```bash
+paracelsus graph example_app.models.base:Base \
+  --import-module "example_app.models.*" \
+  --include-tables "users"
+  --include-tables "posts"
+```
 
 ### Generate Mermaid Diagrams
 
 
 > paracelsus graph example_app.models.base:Base --import-module "example_app.models:*"
 
 ```text
```

### Comparing `paracelsus-0.5.2/paracelsus.egg-info/SOURCES.txt` & `paracelsus-0.6.0/paracelsus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/pyproject.toml` & `paracelsus-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/tests/assets/example/models.py` & `paracelsus-0.6.0/tests/assets/example/models.py`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/tests/conftest.py` & `paracelsus-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.2/tests/test_cli.py` & `paracelsus-0.6.0/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,52 @@
         ],
     )
 
     assert result.exit_code == 0
     mermaid_assert(result.stdout)
 
 
+def test_graph_with_exclusion(package_path):
+    result = runner.invoke(
+        app,
+        [
+            "graph",
+            "example.base:Base",
+            "--import-module",
+            "example.models",
+            "--python-dir",
+            str(package_path),
+            "--exclude-tables",
+            "comments",
+        ],
+    )
+    assert result.exit_code == 0
+    assert "posts {" in result.stdout
+    assert "comments {" not in result.stdout
+
+
+def test_graph_with_inclusion(package_path):
+    result = runner.invoke(
+        app,
+        [
+            "graph",
+            "example.base:Base",
+            "--import-module",
+            "example.models",
+            "--python-dir",
+            str(package_path),
+            "--include-tables",
+            "comments",
+        ],
+    )
+    assert result.exit_code == 0
+    assert "posts {" not in result.stdout
+    assert "comments {" in result.stdout
+
+
 def test_inject_check(package_path):
     result = runner.invoke(
         app,
         [
             "inject",
             str(package_path / "README.md"),
             "example.base:Base",
```

### Comparing `paracelsus-0.5.2/tests/transformers/test_dot.py` & `paracelsus-0.6.0/tests/transformers/test_dot.py`

 * *Files identical despite different names*

