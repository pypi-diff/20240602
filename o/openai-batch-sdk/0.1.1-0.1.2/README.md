# Comparing `tmp/openai_batch_sdk-0.1.1.tar.gz` & `tmp/openai_batch_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_batch_sdk-0.1.1.tar", last modified: Sat Jun  1 23:27:21 2024, max compression
+gzip compressed data, was "openai_batch_sdk-0.1.2.tar", last modified: Sat Jun  1 23:38:08 2024, max compression
```

## Comparing `openai_batch_sdk-0.1.1.tar` & `openai_batch_sdk-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/deps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/deps/oai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/oai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/deps/oai/batch_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/oai/batch_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/oai/batch_api/batch_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/openai_batch_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_batch_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_result_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.743581 openai_batch_sdk-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-06-01 23:38:08.743581 openai_batch_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:38:08.743581 openai_batch_sdk-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.739581 openai_batch_sdk-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.739581 openai_batch_sdk-0.1.2/src/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/deps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.739581 openai_batch_sdk-0.1.2/src/deps/oai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/deps/oai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.739581 openai_batch_sdk-0.1.2/src/deps/oai/batch_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/deps/oai/batch_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/deps/oai/batch_api/batch_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.743581 openai_batch_sdk-0.1.2/src/openai_batch_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.743581 openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-06-01 23:38:08.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-06-01 23:38:08.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 23:38:08.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 23:38:08.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 23:38:08.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 23:38:08.000000 openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.743581 openai_batch_sdk-0.1.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/src/utils/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:08.743581 openai_batch_sdk-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/tests/test_batch_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/tests/test_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/tests/test_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:38:04.000000 openai_batch_sdk-0.1.2/tests/test_result_handler.py
```

### Comparing `openai_batch_sdk-0.1.1/PKG-INFO` & `openai_batch_sdk-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_batch_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: An SDK for OpenAI ChatGPT batch API for a single process.
 Home-page: https://github.com/adico1/openai_batch_sdk
 Author: adico
 Author-email: adico1@gamil.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_batch_sdk-0.1.1/README.md` & `openai_batch_sdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_batch_sdk-0.1.1/setup.py` & `openai_batch_sdk-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="openai_batch_sdk",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "openai",
         "python-dotenv",
     ],
     entry_points={
```

### Comparing `openai_batch_sdk-0.1.1/src/deps/oai/batch_api/batch_api.py` & `openai_batch_sdk-0.1.2/src/deps/oai/batch_api/batch_api.py`

 * *Files identical despite different names*

### Comparing `openai_batch_sdk-0.1.1/src/openai_batch_sdk/core.py` & `openai_batch_sdk-0.1.2/src/openai_batch_sdk/core.py`

 * *Files identical despite different names*

### Comparing `openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/PKG-INFO` & `openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_batch_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: An SDK for OpenAI ChatGPT batch API for a single process.
 Home-page: https://github.com/adico1/openai_batch_sdk
 Author: adico
 Author-email: adico1@gamil.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/SOURCES.txt` & `openai_batch_sdk-0.1.2/src/openai_batch_sdk.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,11 +10,15 @@
 src/openai_batch_sdk/event_handler.py
 src/openai_batch_sdk.egg-info/PKG-INFO
 src/openai_batch_sdk.egg-info/SOURCES.txt
 src/openai_batch_sdk.egg-info/dependency_links.txt
 src/openai_batch_sdk.egg-info/entry_points.txt
 src/openai_batch_sdk.egg-info/requires.txt
 src/openai_batch_sdk.egg-info/top_level.txt
+src/utils/__init__.py
+src/utils/env.py
+src/utils/logging.py
+src/utils/project.py
 tests/test_batch_processor.py
 tests/test_event_handler.py
 tests/test_notifier.py
 tests/test_result_handler.py
```

### Comparing `openai_batch_sdk-0.1.1/tests/test_batch_processor.py` & `openai_batch_sdk-0.1.2/tests/test_batch_processor.py`

 * *Files identical despite different names*

