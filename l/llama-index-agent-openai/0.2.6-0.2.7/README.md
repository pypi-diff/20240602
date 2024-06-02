# Comparing `tmp/llama_index_agent_openai-0.2.6.tar.gz` & `tmp/llama_index_agent_openai-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai-0.2.6.tar", max compression
+gzip compressed data, was "llama_index_agent_openai-0.2.7.tar", max compression
```

## Comparing `llama_index_agent_openai-0.2.6.tar` & `llama_index_agent_openai-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       39 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/README.md
--rw-r--r--   0        0        0      342 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/__init__.py
--rw-r--r--   0        0        0     4745 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/base.py
--rw-r--r--   0        0        0    19580 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/openai_assistant_agent.py
--rw-r--r--   0        0        0    28901 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/step.py
--rw-r--r--   0        0        0      427 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/utils.py
--rw-r--r--   0        0        0     1522 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-06-02 15:08:39.984190 llama_index_agent_openai-0.2.7/README.md
+-rw-r--r--   0        0        0      342 2024-06-02 15:08:39.984190 llama_index_agent_openai-0.2.7/llama_index/agent/openai/__init__.py
+-rw-r--r--   0        0        0     4745 2024-06-02 15:08:39.984190 llama_index_agent_openai-0.2.7/llama_index/agent/openai/base.py
+-rw-r--r--   0        0        0    19580 2024-06-02 15:08:39.984190 llama_index_agent_openai-0.2.7/llama_index/agent/openai/openai_assistant_agent.py
+-rw-r--r--   0        0        0    28901 2024-06-02 15:08:39.984190 llama_index_agent_openai-0.2.7/llama_index/agent/openai/step.py
+-rw-r--r--   0        0        0      427 2024-06-02 15:08:39.984190 llama_index_agent_openai-0.2.7/llama_index/agent/openai/utils.py
+-rw-r--r--   0        0        0     1522 2024-06-02 15:08:39.984190 llama_index_agent_openai-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.7/PKG-INFO
```

### Comparing `llama_index_agent_openai-0.2.6/llama_index/agent/openai/base.py` & `llama_index_agent_openai-0.2.7/llama_index/agent/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.6/llama_index/agent/openai/openai_assistant_agent.py` & `llama_index_agent_openai-0.2.7/llama_index/agent/openai/openai_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.6/llama_index/agent/openai/step.py` & `llama_index_agent_openai-0.2.7/llama_index/agent/openai/step.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.6/pyproject.toml` & `llama_index_agent_openai-0.2.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai"
 readme = "README.md"
-version = "0.2.6"
+version = "0.2.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.41"
 llama-index-llms-openai = "^0.1.5"
 openai = ">=1.14.0"
```

### Comparing `llama_index_agent_openai-0.2.6/PKG-INFO` & `llama_index_agent_openai-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai
-Version: 0.2.6
+Version: 0.2.7
 Summary: llama-index agent openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

