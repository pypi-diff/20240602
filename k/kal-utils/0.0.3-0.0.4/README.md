# Comparing `tmp/kal_utils-0.0.3.tar.gz` & `tmp/kal_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kal_utils-0.0.3.tar", last modified: Mon May 27 09:26:37 2024, max compression
+gzip compressed data, was "kal_utils-0.0.4.tar", last modified: Sun Jun  2 12:37:20 2024, max compression
```

## Comparing `kal_utils-0.0.3.tar` & `kal_utils-0.0.4.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.180592 kal_utils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.168592 kal_utils-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.172592 kal_utils-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.172592 kal_utils-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-27 09:26:23.000000 kal_utils-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 09:26:23.000000 kal_utils-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-27 09:26:23.000000 kal_utils-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-27 09:26:37.180592 kal_utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-27 09:26:23.000000 kal_utils-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.176592 kal_utils-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.176592 kal_utils-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/handle_response.md
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/kal_utils.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/logger.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/mongodb.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.176592 kal_utils-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/requests.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 09:26:23.000000 kal_utils-0.0.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.176592 kal_utils-0.0.3/kal_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-27 09:26:23.000000 kal_utils-0.0.3/kal_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-27 09:26:23.000000 kal_utils-0.0.3/kal_utils/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 09:26:23.000000 kal_utils-0.0.3/kal_utils/kal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 09:26:23.000000 kal_utils-0.0.3/kal_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-27 09:26:23.000000 kal_utils-0.0.3/kal_utils/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-27 09:26:23.000000 kal_utils-0.0.3/kal_utils/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.176592 kal_utils-0.0.3/kal_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-27 09:26:37.000000 kal_utils-0.0.3/kal_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-27 09:26:37.000000 kal_utils-0.0.3/kal_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:26:37.000000 kal_utils-0.0.3/kal_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 09:26:37.000000 kal_utils-0.0.3/kal_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 09:26:37.000000 kal_utils-0.0.3/kal_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 09:26:37.000000 kal_utils-0.0.3/kal_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-27 09:26:23.000000 kal_utils-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-27 09:26:23.000000 kal_utils-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 09:26:23.000000 kal_utils-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 09:26:23.000000 kal_utils-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:26:37.180592 kal_utils-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:26:37.176592 kal_utils-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 09:26:23.000000 kal_utils-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-27 09:26:23.000000 kal_utils-0.0.3/tests/test_kal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.672884 kal_utils-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.664884 kal_utils-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.664884 kal_utils-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.668884 kal_utils-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-06-02 12:37:09.000000 kal_utils-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 12:37:09.000000 kal_utils-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-02 12:37:09.000000 kal_utils-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-06-02 12:37:20.672884 kal_utils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-06-02 12:37:09.000000 kal_utils-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.668884 kal_utils-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/bucket.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.668884 kal_utils-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/handle_response.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/kal_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/logger.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/mongodb.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.668884 kal_utils-0.0.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/requests.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 12:37:09.000000 kal_utils-0.0.4/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.668884 kal_utils-0.0.4/kal_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-02 12:37:09.000000 kal_utils-0.0.4/kal_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-06-02 12:37:09.000000 kal_utils-0.0.4/kal_utils/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-06-02 12:37:09.000000 kal_utils-0.0.4/kal_utils/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-02 12:37:09.000000 kal_utils-0.0.4/kal_utils/kal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 12:37:09.000000 kal_utils-0.0.4/kal_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-06-02 12:37:09.000000 kal_utils-0.0.4/kal_utils/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-06-02 12:37:09.000000 kal_utils-0.0.4/kal_utils/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.672884 kal_utils-0.0.4/kal_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-06-02 12:37:20.000000 kal_utils-0.0.4/kal_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-06-02 12:37:20.000000 kal_utils-0.0.4/kal_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:37:20.000000 kal_utils-0.0.4/kal_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 12:37:20.000000 kal_utils-0.0.4/kal_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-02 12:37:20.000000 kal_utils-0.0.4/kal_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 12:37:20.000000 kal_utils-0.0.4/kal_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-06-02 12:37:09.000000 kal_utils-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-06-02 12:37:09.000000 kal_utils-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 12:37:09.000000 kal_utils-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-02 12:37:09.000000 kal_utils-0.0.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:37:20.672884 kal_utils-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:37:20.672884 kal_utils-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 12:37:09.000000 kal_utils-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-06-02 12:37:09.000000 kal_utils-0.0.4/tests/test_kal_utils.py
```

### Comparing `kal_utils-0.0.3/.github/workflows/docs-build.yml` & `kal_utils-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/.github/workflows/docs.yml` & `kal_utils-0.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/.github/workflows/installation.yml` & `kal_utils-0.0.4/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/.github/workflows/macos.yml` & `kal_utils-0.0.4/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/.github/workflows/pypi.yml` & `kal_utils-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/.github/workflows/ubuntu.yml` & `kal_utils-0.0.4/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/.github/workflows/windows.yml` & `kal_utils-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/.gitignore` & `kal_utils-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/LICENSE` & `kal_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/PKG-INFO` & `kal_utils-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Kaleidoo utils package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-utils
 Keywords: kal-utils
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: fastapi
 Requires-Dist: mongoengine==0.24.2
 Requires-Dist: pymongo==3.11.4
+Requires-Dist: google-cloud-storage
 Provides-Extra: all
 Requires-Dist: kal-utils[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # kal-utils
```

### Comparing `kal_utils-0.0.3/docs/contributing.md` & `kal_utils-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/docs/installation.md` & `kal_utils-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/kal_utils/handle_response.py` & `kal_utils-0.0.4/kal_utils/handle_response.py`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/kal_utils/logger.py` & `kal_utils-0.0.4/kal_utils/logger.py`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/kal_utils/mongodb.py` & `kal_utils-0.0.4/kal_utils/mongodb.py`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/kal_utils/requests.py` & `kal_utils-0.0.4/kal_utils/requests.py`

 * *Files identical despite different names*

### Comparing `kal_utils-0.0.3/kal_utils.egg-info/PKG-INFO` & `kal_utils-0.0.4/kal_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Kaleidoo utils package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-utils
 Keywords: kal-utils
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: fastapi
 Requires-Dist: mongoengine==0.24.2
 Requires-Dist: pymongo==3.11.4
+Requires-Dist: google-cloud-storage
 Provides-Extra: all
 Requires-Dist: kal-utils[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # kal-utils
```

### Comparing `kal_utils-0.0.3/kal_utils.egg-info/SOURCES.txt` & `kal_utils-0.0.4/kal_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,30 @@
 .github/workflows/docs-build.yml
 .github/workflows/docs.yml
 .github/workflows/installation.yml
 .github/workflows/macos.yml
 .github/workflows/pypi.yml
 .github/workflows/ubuntu.yml
 .github/workflows/windows.yml
+docs/bucket.md
 docs/changelog.md
 docs/contributing.md
 docs/faq.md
 docs/handle_response.md
 docs/index.md
 docs/installation.md
 docs/kal_utils.md
 docs/logger.md
 docs/mongodb.md
 docs/requests.md
 docs/usage.md
 docs/examples/intro.ipynb
 docs/overrides/main.html
 kal_utils/__init__.py
+kal_utils/bucket.py
 kal_utils/handle_response.py
 kal_utils/kal_utils.py
 kal_utils/logger.py
 kal_utils/mongodb.py
 kal_utils/requests.py
 kal_utils.egg-info/PKG-INFO
 kal_utils.egg-info/SOURCES.txt
```

### Comparing `kal_utils-0.0.3/mkdocs.yml` & `kal_utils-0.0.4/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -83,7 +83,8 @@
         - examples/intro.ipynb
     - API Reference:
           - kal_utils module: kal_utils.md
           - requests module: requests.md
           - logger module: logger.md
           - handle_response module: handle_response.md
           - mongodb module: mongodb.md
+          - bucket module: bucket.md
```

### Comparing `kal_utils-0.0.3/pyproject.toml` & `kal_utils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kal-utils"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = [
     "dependencies",
 ]
 description = "Kaleidoo utils package"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

