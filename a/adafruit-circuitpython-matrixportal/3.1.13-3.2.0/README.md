# Comparing `tmp/adafruit-circuitpython-matrixportal-3.1.13.tar.gz` & `tmp/adafruit_circuitpython_matrixportal-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-matrixportal-3.1.13.tar", last modified: Sat Dec  9 17:45:24 2023, max compression
+gzip compressed data, was "adafruit_circuitpython_matrixportal-3.2.0.tar", last modified: Sun Jun  2 02:54:55 2024, max compression
```

## Comparing `adafruit-circuitpython-matrixportal-3.1.13.tar` & `adafruit_circuitpython_matrixportal-3.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.123070 adafruit-circuitpython-matrixportal-3.1.13/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.115070 adafruit-circuitpython-matrixportal-3.1.13/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.119070 adafruit-circuitpython-matrixportal-3.1.13/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.119070 adafruit-circuitpython-matrixportal-3.1.13/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.119070 adafruit-circuitpython-matrixportal-3.1.13/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-12-09 17:45:24.123070 adafruit-circuitpython-matrixportal-3.1.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.123070 adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-12-09 17:45:24.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-09 17:45:24.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 17:45:24.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-09 17:45:24.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-09 17:45:24.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.119070 adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2576 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7814 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10650 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/matrixportal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3055 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.123070 adafruit-circuitpython-matrixportal-3.1.13/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.123070 adafruit-circuitpython-matrixportal-3.1.13/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 17:45:24.123070 adafruit-circuitpython-matrixportal-3.1.13/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/examples/matrixportal_scrolling_bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/examples/matrixportal_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-09 17:45:17.000000 adafruit-circuitpython-matrixportal-3.1.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-12-09 17:45:11.000000 adafruit-circuitpython-matrixportal-3.1.13/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 17:45:24.123070 adafruit-circuitpython-matrixportal-3.1.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.623730 adafruit_circuitpython_matrixportal-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.615729 adafruit_circuitpython_matrixportal-3.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.615729 adafruit_circuitpython_matrixportal-3.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.619729 adafruit_circuitpython_matrixportal-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.619729 adafruit_circuitpython_matrixportal-3.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-06-02 02:54:55.623730 adafruit_circuitpython_matrixportal-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.623730 adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-06-02 02:54:55.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-06-02 02:54:55.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 02:54:55.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-02 02:54:55.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 02:54:55.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.619729 adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7813 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10762 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/matrixportal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3054 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.623730 adafruit_circuitpython_matrixportal-3.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.623730 adafruit_circuitpython_matrixportal-3.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:54:55.623730 adafruit_circuitpython_matrixportal-3.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/examples/matrixportal_scrolling_bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/examples/matrixportal_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-02 02:54:53.000000 adafruit_circuitpython_matrixportal-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-06-02 02:54:45.000000 adafruit_circuitpython_matrixportal-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 02:54:55.623730 adafruit_circuitpython_matrixportal-3.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_matrixportal-3.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/.gitignore` & `adafruit_circuitpython_matrixportal-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/.pre-commit-config.yaml` & `adafruit_circuitpython_matrixportal-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/.pylintrc` & `adafruit_circuitpython_matrixportal-3.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_matrixportal-3.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/LICENSE` & `adafruit_circuitpython_matrixportal-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_matrixportal-3.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/LICENSES/MIT.txt` & `adafruit_circuitpython_matrixportal-3.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/LICENSES/Unlicense.txt` & `adafruit_circuitpython_matrixportal-3.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/PKG-INFO` & `adafruit_circuitpython_matrixportal-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixportal
-Version: 3.1.13
+Version: 3.2.0
 Summary: CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal
 Keywords: adafruit,matrixportal,matrix,rgb,led,feather,featherwing,shieldbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/README.rst` & `adafruit_circuitpython_matrixportal-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO` & `adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixportal
-Version: 3.1.13
+Version: 3.2.0
 Summary: CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal
 Keywords: adafruit,matrixportal,matrix,rgb,led,feather,featherwing,shieldbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt` & `adafruit_circuitpython_matrixportal-3.2.0/adafruit_circuitpython_matrixportal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/graphics.py` & `adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 from adafruit_portalbase.graphics import GraphicsBase
 from adafruit_matrixportal.matrix import Matrix
 
-__version__ = "3.1.13"
+__version__ = "3.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the MatrixPortal Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/matrix.py` & `adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os
 import board
 import displayio
 import rgbmatrix
 import framebufferio
 
 
-__version__ = "3.1.13"
+__version__ = "3.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Matrix:
     """Class representing the Adafruit RGB Matrix. This is used to automatically
     initialize the display.
```

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/matrixportal.py` & `adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/matrixportal.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import gc
 from time import sleep
 import terminalio
 from adafruit_portalbase import PortalBase
 from adafruit_matrixportal.network import Network
 from adafruit_matrixportal.graphics import Graphics
 
-__version__ = "3.1.13"
+__version__ = "3.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class MatrixPortal(PortalBase):
     """Class representing the Adafruit RGB Matrix Portal.
 
     :param url: The URL of your data source. Defaults to ``None``.
@@ -88,35 +88,39 @@
         color_order="RGB",
         debug=False,
         width=64,
         height=32,
         serpentine=True,
         tile_rows=1,
         rotation=0,
+        use_wifi=True,
     ):
         graphics = Graphics(
             default_bg=default_bg,
             bit_depth=bit_depth,
             width=width,
             height=height,
             alt_addr_pins=alt_addr_pins,
             color_order=color_order,
             serpentine=serpentine,
             tile_rows=tile_rows,
             rotation=rotation,
             debug=debug,
         )
 
-        network = Network(
-            status_neopixel=status_neopixel,
-            esp=esp,
-            external_spi=external_spi,
-            extract_values=False,
-            debug=debug,
-        )
+        if use_wifi:
+            network = Network(
+                status_neopixel=status_neopixel,
+                esp=esp,
+                external_spi=external_spi,
+                extract_values=False,
+                debug=debug,
+            )
+        else:
+            network = None
 
         super().__init__(
             network,
             graphics,
             url=url,
             headers=headers,
             json_path=json_path,
```

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/adafruit_matrixportal/network.py` & `adafruit_circuitpython_matrixportal-3.2.0/adafruit_matrixportal/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from adafruit_portalbase.network import NetworkBase
 
 if os.uname().sysname == "samd51":
     from adafruit_portalbase.wifi_coprocessor import WiFi
 else:
     from adafruit_portalbase.wifi_esp32s2 import WiFi
 
-__version__ = "3.1.13"
+__version__ = "3.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal.git"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit RGB Matrix Portal.
 
     :param status_neopixel: The pin for the status NeoPixel. Use ``board.NEOPIXEL`` for the on-board
```

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/docs/_static/favicon.ico` & `adafruit_circuitpython_matrixportal-3.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/docs/conf.py` & `adafruit_circuitpython_matrixportal-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/docs/index.rst` & `adafruit_circuitpython_matrixportal-3.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/examples/matrixportal_scrolling_bitcoin.py` & `adafruit_circuitpython_matrixportal-3.2.0/examples/matrixportal_scrolling_bitcoin.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/examples/matrixportal_simpletest.py` & `adafruit_circuitpython_matrixportal-3.2.0/examples/matrixportal_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixportal-3.1.13/pyproject.toml` & `adafruit_circuitpython_matrixportal-3.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-matrixportal"
 description = "CircuitPython helper for Adafruit MatrixPortal M4, Adafruit RGB Matrix Shield + Metro M4 Airlift Lite, and Adafruit RGB Matrix FeatherWings"
-version = "3.1.13"
+version = "3.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MatrixPortal"}
 keywords = [
     "adafruit",
```

