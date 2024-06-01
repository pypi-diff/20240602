# Comparing `tmp/openai_batch_sdk-0.1.0.tar.gz` & `tmp/openai_batch_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_batch_sdk-0.1.0.tar", last modified: Sat Jun  1 20:36:03 2024, max compression
+gzip compressed data, was "openai_batch_sdk-0.1.1.tar", last modified: Sat Jun  1 23:27:21 2024, max compression
```

## Comparing `openai_batch_sdk-0.1.0.tar` & `openai_batch_sdk-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 adicohen   (501) staff       (20)        0 2024-06-01 20:36:03.271426 openai_batch_sdk-0.1.0/
--rw-r--r--   0 adicohen   (501) staff       (20)       33 2024-06-01 20:25:52.000000 openai_batch_sdk-0.1.0/MANIFEST.in
--rw-r--r--   0 adicohen   (501) staff       (20)     3208 2024-06-01 20:36:03.270972 openai_batch_sdk-0.1.0/PKG-INFO
--rw-r--r--   0 adicohen   (501) staff       (20)     2720 2024-05-31 12:28:30.000000 openai_batch_sdk-0.1.0/README.md
--rw-r--r--   0 adicohen   (501) staff       (20)       38 2024-06-01 20:36:03.271485 openai_batch_sdk-0.1.0/setup.cfg
--rw-r--r--   0 adicohen   (501) staff       (20)      846 2024-06-01 20:35:57.000000 openai_batch_sdk-0.1.0/setup.py
-drwxr-xr-x   0 adicohen   (501) staff       (20)        0 2024-06-01 20:36:03.259734 openai_batch_sdk-0.1.0/src/
-drwxr-xr-x   0 adicohen   (501) staff       (20)        0 2024-06-01 20:36:03.262390 openai_batch_sdk-0.1.0/src/deps/
--rw-r--r--   0 adicohen   (501) staff       (20)        0 2024-06-01 00:30:52.000000 openai_batch_sdk-0.1.0/src/deps/__init__.py
-drwxr-xr-x   0 adicohen   (501) staff       (20)        0 2024-06-01 20:36:03.262834 openai_batch_sdk-0.1.0/src/deps/oai/
--rw-r--r--   0 adicohen   (501) staff       (20)        0 2024-06-01 00:30:54.000000 openai_batch_sdk-0.1.0/src/deps/oai/__init__.py
-drwxr-xr-x   0 adicohen   (501) staff       (20)        0 2024-06-01 20:36:03.263770 openai_batch_sdk-0.1.0/src/deps/oai/batch_api/
--rw-r--r--   0 adicohen   (501) staff       (20)        0 2024-06-01 00:30:46.000000 openai_batch_sdk-0.1.0/src/deps/oai/batch_api/__init__.py
--rw-r--r--   0 adicohen   (501) staff       (20)      889 2024-06-01 17:07:47.000000 openai_batch_sdk-0.1.0/src/deps/oai/batch_api/batch_api.py
-drwxr-xr-x   0 adicohen   (501) staff       (20)        0 2024-06-01 20:36:03.270438 openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/
--rw-r--r--   0 adicohen   (501) staff       (20)     3208 2024-06-01 20:36:03.000000 openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adicohen   (501) staff       (20)      523 2024-06-01 20:36:03.000000 openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adicohen   (501) staff       (20)        1 2024-06-01 20:36:03.000000 openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adicohen   (501) staff       (20)       65 2024-06-01 20:36:03.000000 openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/entry_points.txt
--rw-r--r--   0 adicohen   (501) staff       (20)       21 2024-06-01 20:36:03.000000 openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/requires.txt
--rw-r--r--   0 adicohen   (501) staff       (20)        5 2024-06-01 20:36:03.000000 openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 adicohen   (501) staff       (20)        0 2024-06-01 20:36:03.269898 openai_batch_sdk-0.1.0/tests/
--rw-r--r--   0 adicohen   (501) staff       (20)     1628 2024-06-01 16:19:22.000000 openai_batch_sdk-0.1.0/tests/test_batch_processor.py
--rw-r--r--   0 adicohen   (501) staff       (20)        0 2024-05-31 11:40:19.000000 openai_batch_sdk-0.1.0/tests/test_event_handler.py
--rw-r--r--   0 adicohen   (501) staff       (20)        0 2024-05-31 11:40:24.000000 openai_batch_sdk-0.1.0/tests/test_notifier.py
--rw-r--r--   0 adicohen   (501) staff       (20)        0 2024-05-31 11:40:30.000000 openai_batch_sdk-0.1.0/tests/test_result_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/deps/oai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/oai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/deps/oai/batch_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/oai/batch_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/deps/oai/batch_api/batch_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.756991 openai_batch_sdk-0.1.1/src/openai_batch_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 23:27:21.000000 openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:21.760991 openai_batch_sdk-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_batch_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:27:17.000000 openai_batch_sdk-0.1.1/tests/test_result_handler.py
```

### Comparing `openai_batch_sdk-0.1.0/PKG-INFO` & `openai_batch_sdk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_batch_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: An SDK for OpenAI ChatGPT batch API for a single process.
 Home-page: https://github.com/adico1/openai_batch_sdk
 Author: adico
 Author-email: adico1@gamil.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_batch_sdk-0.1.0/README.md` & `openai_batch_sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_batch_sdk-0.1.0/setup.py` & `openai_batch_sdk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="openai_batch_sdk",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "openai",
         "python-dotenv",
     ],
     entry_points={
```

### Comparing `openai_batch_sdk-0.1.0/src/deps/oai/batch_api/batch_api.py` & `openai_batch_sdk-0.1.1/src/deps/oai/batch_api/batch_api.py`

 * *Files identical despite different names*

### Comparing `openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/PKG-INFO` & `openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_batch_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: An SDK for OpenAI ChatGPT batch API for a single process.
 Home-page: https://github.com/adico1/openai_batch_sdk
 Author: adico
 Author-email: adico1@gamil.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai_batch_sdk-0.1.0/src/openai_batch_sdk.egg-info/SOURCES.txt` & `openai_batch_sdk-0.1.1/src/openai_batch_sdk.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 MANIFEST.in
 README.md
 setup.py
 src/deps/__init__.py
 src/deps/oai/__init__.py
 src/deps/oai/batch_api/__init__.py
 src/deps/oai/batch_api/batch_api.py
+src/openai_batch_sdk/__init__.py
+src/openai_batch_sdk/core.py
+src/openai_batch_sdk/event_handler.py
 src/openai_batch_sdk.egg-info/PKG-INFO
 src/openai_batch_sdk.egg-info/SOURCES.txt
 src/openai_batch_sdk.egg-info/dependency_links.txt
 src/openai_batch_sdk.egg-info/entry_points.txt
 src/openai_batch_sdk.egg-info/requires.txt
 src/openai_batch_sdk.egg-info/top_level.txt
 tests/test_batch_processor.py
```

### Comparing `openai_batch_sdk-0.1.0/tests/test_batch_processor.py` & `openai_batch_sdk-0.1.1/tests/test_batch_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import unittest
 from unittest.mock import MagicMock, patch
 
 # Ensure the src directory is in the Python path
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '../src')))
 
 from src.advanced_batch_processor import init_monitoring
-from src.event_handler import EventHandler
+from src.openai_batch_sdk.event_handler import EventHandler
 
 
 class TestBatchProcessor(unittest.TestCase):
     @patch('src.batch_processor.openai.File.create')
     @patch('src.batch_processor.openai.Batch.create')
     @patch('src.batch_processor.openai.Batch.retrieve')
     @patch('src.batch_processor.openai.File.download')
```

