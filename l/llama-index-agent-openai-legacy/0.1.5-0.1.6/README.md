# Comparing `tmp/llama_index_agent_openai_legacy-0.1.5.tar.gz` & `tmp/llama_index_agent_openai_legacy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai_legacy-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_agent_openai_legacy-0.1.6.tar", max compression
```

## Comparing `llama_index_agent_openai_legacy-0.1.5.tar` & `llama_index_agent_openai_legacy-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       46 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/README.md
--rw-r--r--   0        0        0      412 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/__init__.py
--rw-r--r--   0        0        0     7463 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/context_retriever_agent.py
--rw-r--r--   0        0        0    22767 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/openai_agent.py
--rw-r--r--   0        0        0      857 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/retriever_openai_agent.py
--rw-r--r--   0        0        0      772 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/utils.py
--rw-r--r--   0        0        0     1541 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_agent_openai_legacy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-06-02 15:08:39.984190 llama_index_agent_openai_legacy-0.1.6/README.md
+-rw-r--r--   0        0        0      412 2024-06-02 15:08:39.984190 llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/__init__.py
+-rw-r--r--   0        0        0     7463 2024-06-02 15:08:39.984190 llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/context_retriever_agent.py
+-rw-r--r--   0        0        0    22767 2024-06-02 15:08:39.984190 llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/openai_agent.py
+-rw-r--r--   0        0        0      857 2024-06-02 15:08:39.984190 llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/retriever_openai_agent.py
+-rw-r--r--   0        0        0      772 2024-06-02 15:08:39.984190 llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/utils.py
+-rw-r--r--   0        0        0     1541 2024-06-02 15:08:39.984190 llama_index_agent_openai_legacy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_agent_openai_legacy-0.1.6/PKG-INFO
```

### Comparing `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/context_retriever_agent.py` & `llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/context_retriever_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/openai_agent.py` & `llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/retriever_openai_agent.py` & `llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/retriever_openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/utils.py` & `llama_index_agent_openai_legacy-0.1.6/llama_index/agent/openai_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.5/pyproject.toml` & `llama_index_agent_openai_legacy-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai-legacy integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai-legacy"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.41"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_agent_openai_legacy-0.1.5/PKG-INFO` & `llama_index_agent_openai_legacy-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai-legacy
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index agent openai-legacy integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

