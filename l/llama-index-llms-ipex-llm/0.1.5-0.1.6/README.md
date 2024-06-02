# Comparing `tmp/llama_index_llms_ipex_llm-0.1.5.tar.gz` & `tmp/llama_index_llms_ipex_llm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ipex_llm-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_llms_ipex_llm-0.1.6.tar", max compression
```

## Comparing `llama_index_llms_ipex_llm-0.1.5.tar` & `llama_index_llms_ipex_llm-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      863 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/README.md
--rw-r--r--   0        0        0       17 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/BUILD
--rw-r--r--   0        0        0       75 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/__init__.py
--rw-r--r--   0        0        0    21176 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/base.py
--rw-r--r--   0        0        0     2520 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      863 2024-06-02 15:08:40.036191 llama_index_llms_ipex_llm-0.1.6/README.md
+-rw-r--r--   0        0        0       17 2024-06-02 15:08:40.036191 llama_index_llms_ipex_llm-0.1.6/llama_index/llms/ipex_llm/BUILD
+-rw-r--r--   0        0        0       75 2024-06-02 15:08:40.036191 llama_index_llms_ipex_llm-0.1.6/llama_index/llms/ipex_llm/__init__.py
+-rw-r--r--   0        0        0    21176 2024-06-02 15:08:40.036191 llama_index_llms_ipex_llm-0.1.6/llama_index/llms/ipex_llm/base.py
+-rw-r--r--   0        0        0     2520 2024-06-02 15:08:40.036191 llama_index_llms_ipex_llm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.6/PKG-INFO
```

### Comparing `llama_index_llms_ipex_llm-0.1.5/README.md` & `llama_index_llms_ipex_llm-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/base.py` & `llama_index_llms_ipex_llm-0.1.6/llama_index/llms/ipex_llm/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_ipex_llm-0.1.5/pyproject.toml` & `llama_index_llms_ipex_llm-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ipex-llm integration"
 license = "MIT"
 name = "llama-index-llms-ipex-llm"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.41"
 ipex-llm = {allow-prereleases = true, extras = ["llama-index"], version = ">=2.1.0b20240529"}
 torch = {optional = true, source = "ipex-xpu-src-us", version = "2.1.0a0"}
 torchvision = {optional = true, source = "ipex-xpu-src-us", version = "0.16.0a0"}
```

### Comparing `llama_index_llms_ipex_llm-0.1.5/PKG-INFO` & `llama_index_llms_ipex_llm-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-ipex-llm
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index llms ipex-llm integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

