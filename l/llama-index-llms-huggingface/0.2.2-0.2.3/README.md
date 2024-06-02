# Comparing `tmp/llama_index_llms_huggingface-0.2.2.tar.gz` & `tmp/llama_index_llms_huggingface-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_huggingface-0.2.2.tar", max compression
+gzip compressed data, was "llama_index_llms_huggingface-0.2.3.tar", max compression
```

## Comparing `llama_index_llms_huggingface-0.2.2.tar` & `llama_index_llms_huggingface-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2024-05-31 04:53:38.095158 llama_index_llms_huggingface-0.2.2/README.md
--rw-r--r--   0        0        0      212 2024-05-31 04:53:38.095158 llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    39794 2024-05-31 04:53:38.099158 llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/base.py
--rw-r--r--   0        0        0     2082 2024-05-31 04:53:38.099158 llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/utils.py
--rw-r--r--   0        0        0     1637 2024-05-31 04:53:38.099158 llama_index_llms_huggingface-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       43 2024-06-02 15:08:40.036191 llama_index_llms_huggingface-0.2.3/README.md
+-rw-r--r--   0        0        0      212 2024-06-02 15:08:40.036191 llama_index_llms_huggingface-0.2.3/llama_index/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    39794 2024-06-02 15:08:40.036191 llama_index_llms_huggingface-0.2.3/llama_index/llms/huggingface/base.py
+-rw-r--r--   0        0        0     2082 2024-06-02 15:08:40.036191 llama_index_llms_huggingface-0.2.3/llama_index/llms/huggingface/utils.py
+-rw-r--r--   0        0        0     1637 2024-06-02 15:08:40.036191 llama_index_llms_huggingface-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.2.3/PKG-INFO
```

### Comparing `llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/base.py` & `llama_index_llms_huggingface-0.2.3/llama_index/llms/huggingface/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/utils.py` & `llama_index_llms_huggingface-0.2.3/llama_index/llms/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_huggingface-0.2.2/pyproject.toml` & `llama_index_llms_huggingface-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms huggingface integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-huggingface"
 readme = "README.md"
-version = "0.2.2"
+version = "0.2.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.41"
 huggingface-hub = "^0.23.0"
 torch = "^2.1.2"
 text-generation = "^0.7.0"
```

### Comparing `llama_index_llms_huggingface-0.2.2/PKG-INFO` & `llama_index_llms_huggingface-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-huggingface
-Version: 0.2.2
+Version: 0.2.3
 Summary: llama-index llms huggingface integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

