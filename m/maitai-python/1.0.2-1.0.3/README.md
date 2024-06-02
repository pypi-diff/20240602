# Comparing `tmp/maitai_python-1.0.2.tar.gz` & `tmp/maitai_python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai_python-1.0.2.tar", last modified: Sat Jun  1 00:27:05 2024, max compression
+gzip compressed data, was "maitai_python-1.0.3.tar", last modified: Sun Jun  2 19:17:59 2024, max compression
```

## Comparing `maitai_python-1.0.2.tar` & `maitai_python-1.0.3.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.578662 maitai_python-1.0.2/
--rw-r--r--   0 runner    (1001) runner    (1001)     1719 2024-06-01 00:27:05.578662 maitai_python-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     1215 2024-06-01 00:26:26.000000 maitai_python-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.566661 maitai_python-1.0.2/maitai/
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2249 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_config_listener_thread.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14793 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_evaluator.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5720 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_inference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1135 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_maitai_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11510 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_openai.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11754 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_openai_async.py
--rw-r--r--   0 runner    (1001) runner    (1001)      236 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_openai_types.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2324 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_types.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10243 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai/_utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.566661 maitai_python-1.0.2/maitai_common/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_common/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.566661 maitai_python-1.0.2/maitai_common/processes/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_common/processes/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2057 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_common/processes/io_thread.py
--rw-r--r--   0 runner    (1001) runner    (1001)      894 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_common/processes/stream_evaluation_thread.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3392 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_common/processes/websocket_listener_thread.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.566661 maitai_python-1.0.2/maitai_common/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_common/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      407 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_common/utils/proto_utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.570661 maitai_python-1.0.2/maitai_gen/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.570661 maitai_python-1.0.2/maitai_gen/application/
--rw-r--r--   0 runner    (1001) runner    (1001)     1364 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/application/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.570661 maitai_python-1.0.2/maitai_gen/chat/
--rw-r--r--   0 runner    (1001) runner    (1001)    11403 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.570661 maitai_python-1.0.2/maitai_gen/company/
--rw-r--r--   0 runner    (1001) runner    (1001)      641 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/company/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.570661 maitai_python-1.0.2/maitai_gen/inference/
--rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.570661 maitai_python-1.0.2/maitai_gen/notification/
--rw-r--r--   0 runner    (1001) runner    (1001)     1198 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.570661 maitai_python-1.0.2/maitai_gen/sandbox/
--rw-r--r--   0 runner    (1001) runner    (1001)     1460 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.574662 maitai_python-1.0.2/maitai_gen/sentinel/
--rw-r--r--   0 runner    (1001) runner    (1001)     1518 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/sentinel/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.574662 maitai_python-1.0.2/maitai_gen/session/
--rw-r--r--   0 runner    (1001) runner    (1001)      886 2024-06-01 00:26:26.000000 maitai_python-1.0.2/maitai_gen/session/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-01 00:27:05.578662 maitai_python-1.0.2/maitai_python.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1719 2024-06-01 00:27:05.000000 maitai_python-1.0.2/maitai_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      991 2024-06-01 00:27:05.000000 maitai_python-1.0.2/maitai_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-06-01 00:27:05.000000 maitai_python-1.0.2/maitai_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       70 2024-06-01 00:27:05.000000 maitai_python-1.0.2/maitai_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       32 2024-06-01 00:27:05.000000 maitai_python-1.0.2/maitai_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-06-01 00:27:05.578662 maitai_python-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)      762 2024-06-01 00:26:48.000000 maitai_python-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.550672 maitai_python-1.0.3/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1719 2024-06-02 19:17:59.550672 maitai_python-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1215 2024-06-02 19:17:18.000000 maitai_python-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.530672 maitai_python-1.0.3/maitai/
+-rw-r--r--   0 runner    (1001) runner    (1001)      646 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8561 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_azure.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2249 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_config_listener_thread.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14793 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_evaluator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5720 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_inference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1135 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_maitai_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11579 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_openai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11823 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_openai_async.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      236 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_openai_types.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2324 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_types.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10243 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai/_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.530672 maitai_python-1.0.3/maitai_common/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_common/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.534672 maitai_python-1.0.3/maitai_common/processes/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_common/processes/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2057 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_common/processes/io_thread.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      894 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_common/processes/stream_evaluation_thread.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3392 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_common/processes/websocket_listener_thread.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.534672 maitai_python-1.0.3/maitai_common/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      407 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_common/utils/proto_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.534672 maitai_python-1.0.3/maitai_gen/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.538672 maitai_python-1.0.3/maitai_gen/application/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1364 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/application/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.538672 maitai_python-1.0.3/maitai_gen/chat/
+-rw-r--r--   0 runner    (1001) runner    (1001)    11403 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.538672 maitai_python-1.0.3/maitai_gen/company/
+-rw-r--r--   0 runner    (1001) runner    (1001)      641 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/company/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.542672 maitai_python-1.0.3/maitai_gen/inference/
+-rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.542672 maitai_python-1.0.3/maitai_gen/notification/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1198 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.542672 maitai_python-1.0.3/maitai_gen/sandbox/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1460 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.546672 maitai_python-1.0.3/maitai_gen/sentinel/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1518 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/sentinel/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.546672 maitai_python-1.0.3/maitai_gen/session/
+-rw-r--r--   0 runner    (1001) runner    (1001)      886 2024-06-02 19:17:18.000000 maitai_python-1.0.3/maitai_gen/session/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-06-02 19:17:59.546672 maitai_python-1.0.3/maitai_python.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1719 2024-06-02 19:17:59.000000 maitai_python-1.0.3/maitai_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1008 2024-06-02 19:17:59.000000 maitai_python-1.0.3/maitai_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-06-02 19:17:59.000000 maitai_python-1.0.3/maitai_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       70 2024-06-02 19:17:59.000000 maitai_python-1.0.3/maitai_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       32 2024-06-02 19:17:59.000000 maitai_python-1.0.3/maitai_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-06-02 19:17:59.550672 maitai_python-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      762 2024-06-02 19:17:47.000000 maitai_python-1.0.3/setup.py
```

### Comparing `maitai_python-1.0.2/PKG-INFO` & `maitai_python-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maitai-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: MaiTai SDK for Python
 Home-page: https://docs.trymaitai.ai
 Author: Maitai
 Author-email: support@trymaitai.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maitai_python-1.0.2/README.md` & `maitai_python-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai/__init__.py` & `maitai_python-1.0.3/maitai/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
 import maitai._types as types
+from maitai._azure import MaiTaiAsyncAzureOpenAIClient as AsyncAzureOpenAI, MaitaiAzureOpenAIClient as AzureOpenAI
 from maitai._evaluator import Evaluator as Evaluator
 from maitai._inference import Inference as Inference
 from maitai._openai import MaiTaiOpenAIClient as OpenAI
 from maitai._openai_async import MaiTaiAsyncOpenAIClient as AsyncOpenAI
 
 chat = OpenAI().chat
```

### Comparing `maitai_python-1.0.2/maitai/_config.py` & `maitai_python-1.0.3/maitai/_config.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai/_evaluator.py` & `maitai_python-1.0.3/maitai/_evaluator.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai/_inference.py` & `maitai_python-1.0.3/maitai/_inference.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai/_maitai_client.py` & `maitai_python-1.0.3/maitai/_maitai_client.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai/_openai.py` & `maitai_python-1.0.3/maitai/_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             project=project,
             base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
             default_headers=default_headers,
             default_query=default_query,
             http_client=http_client,
+            _strict_response_validation=_strict_response_validation,
         )
         self.chat = Chat(self.client)
 
 
 class Chat:
     def __init__(self, client=None):
         self.completions = Completions(client)
```

### Comparing `maitai_python-1.0.2/maitai/_openai_async.py` & `maitai_python-1.0.3/maitai/_openai_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             project=project,
             base_url=base_url,
             timeout=timeout,
             max_retries=max_retries,
             default_headers=default_headers,
             default_query=default_query,
             http_client=http_client,
+            _strict_response_validation=_strict_response_validation,
         )
 
         self.chat = AsyncChat(self.client)
 
 
 class AsyncChat:
     def __init__(self, client=None):
```

### Comparing `maitai_python-1.0.2/maitai/_types.py` & `maitai_python-1.0.3/maitai/_types.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai/_utils.py` & `maitai_python-1.0.3/maitai/_utils.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_common/processes/io_thread.py` & `maitai_python-1.0.3/maitai_common/processes/io_thread.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_common/processes/stream_evaluation_thread.py` & `maitai_python-1.0.3/maitai_common/processes/stream_evaluation_thread.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_common/processes/websocket_listener_thread.py` & `maitai_python-1.0.3/maitai_common/processes/websocket_listener_thread.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/application/__init__.py` & `maitai_python-1.0.3/maitai_gen/application/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/chat/__init__.py` & `maitai_python-1.0.3/maitai_gen/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/company/__init__.py` & `maitai_python-1.0.3/maitai_gen/company/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/inference/__init__.py` & `maitai_python-1.0.3/maitai_gen/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/notification/__init__.py` & `maitai_python-1.0.3/maitai_gen/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/sandbox/__init__.py` & `maitai_python-1.0.3/maitai_gen/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/sentinel/__init__.py` & `maitai_python-1.0.3/maitai_gen/sentinel/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_gen/session/__init__.py` & `maitai_python-1.0.3/maitai_gen/session/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.2/maitai_python.egg-info/PKG-INFO` & `maitai_python-1.0.3/maitai_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maitai-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: MaiTai SDK for Python
 Home-page: https://docs.trymaitai.ai
 Author: Maitai
 Author-email: support@trymaitai.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maitai_python-1.0.2/maitai_python.egg-info/SOURCES.txt` & `maitai_python-1.0.3/maitai_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 maitai/__init__.py
+maitai/_azure.py
 maitai/_config.py
 maitai/_config_listener_thread.py
 maitai/_evaluator.py
 maitai/_inference.py
 maitai/_maitai_client.py
 maitai/_openai.py
 maitai/_openai_async.py
```

### Comparing `maitai_python-1.0.2/setup.py` & `maitai_python-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 from setuptools import setup, find_packages
 setup(
     name='maitai-python',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(exclude=("maitai_back", "maitai_back.*")),
     install_requires=[
         'requests',
         'openai',
         'betterproto',
         'httpx',
         'aiohttp',
```

