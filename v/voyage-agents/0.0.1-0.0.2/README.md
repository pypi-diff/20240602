# Comparing `tmp/voyage_agents-0.0.1.tar.gz` & `tmp/voyage_agents-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyage_agents-0.0.1.tar", last modified: Sun Jun  2 13:37:30 2024, max compression
+gzip compressed data, was "voyage_agents-0.0.2.tar", last modified: Sun Jun  2 15:03:49 2024, max compression
```

## Comparing `voyage_agents-0.0.1.tar` & `voyage_agents-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,13 @@
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/
--rw-rw-r--   0 ville     (1000) ville     (1000)     1072 2024-06-01 13:48:05.000000 voyage_agents-0.0.1/LICENSE
--rw-r--r--   0 ville     (1000) ville     (1000)      818 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/PKG-INFO
--rw-rw-r--   0 ville     (1000) ville     (1000)      275 2024-06-02 09:17:20.000000 voyage_agents-0.0.1/README.md
--rw-r--r--   0 ville     (1000) ville     (1000)      523 2024-06-02 13:34:38.000000 voyage_agents-0.0.1/pyproject.toml
--rw-rw-r--   0 ville     (1000) ville     (1000)       38 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/setup.cfg
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/src/
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/src/voyage_agents/
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/src/voyage_agents/agents/
--rw-r--r--   0 ville     (1000) ville     (1000)      153 2024-06-02 13:31:10.000000 voyage_agents-0.0.1/src/voyage_agents/agents/__init__.py
--rw-r--r--   0 ville     (1000) ville     (1000)     4028 2024-06-02 13:31:18.000000 voyage_agents-0.0.1/src/voyage_agents/agents/agent.py
--rw-rw-r--   0 ville     (1000) ville     (1000)     1348 2024-06-02 13:31:22.000000 voyage_agents-0.0.1/src/voyage_agents/agents/reflector.py
--rw-r--r--   0 ville     (1000) ville     (1000)     2022 2024-06-02 13:31:26.000000 voyage_agents-0.0.1/src/voyage_agents/agents/tool_caller.py
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/src/voyage_agents/core/
--rw-r--r--   0 ville     (1000) ville     (1000)      190 2024-06-02 13:30:34.000000 voyage_agents-0.0.1/src/voyage_agents/core/__init__.py
--rw-r--r--   0 ville     (1000) ville     (1000)     2125 2024-06-02 13:30:46.000000 voyage_agents-0.0.1/src/voyage_agents/core/grammar.py
--rw-r--r--   0 ville     (1000) ville     (1000)      601 2024-06-02 12:03:57.000000 voyage_agents-0.0.1/src/voyage_agents/core/manager.py
--rw-r--r--   0 ville     (1000) ville     (1000)      157 2024-06-02 12:26:11.000000 voyage_agents-0.0.1/src/voyage_agents/core/message.py
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/src/voyage_agents/prompt/
--rw-rw-r--   0 ville     (1000) ville     (1000)      122 2024-06-02 13:30:56.000000 voyage_agents-0.0.1/src/voyage_agents/prompt/__init__.py
--rw-r--r--   0 ville     (1000) ville     (1000)     3162 2024-06-02 13:31:00.000000 voyage_agents-0.0.1/src/voyage_agents/prompt/prompt.py
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/src/voyage_agents/tool/
--rw-r--r--   0 ville     (1000) ville     (1000)      109 2024-06-02 13:31:06.000000 voyage_agents-0.0.1/src/voyage_agents/tool/__init__.py
--rw-r--r--   0 ville     (1000) ville     (1000)     1766 2024-06-02 13:13:53.000000 voyage_agents-0.0.1/src/voyage_agents/tool/tool.py
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 13:37:30.429728 voyage_agents-0.0.1/src/voyage_agents.egg-info/
--rw-r--r--   0 ville     (1000) ville     (1000)      818 2024-06-02 13:37:30.000000 voyage_agents-0.0.1/src/voyage_agents.egg-info/PKG-INFO
--rw-rw-r--   0 ville     (1000) ville     (1000)      620 2024-06-02 13:37:30.000000 voyage_agents-0.0.1/src/voyage_agents.egg-info/SOURCES.txt
--rw-rw-r--   0 ville     (1000) ville     (1000)        1 2024-06-02 13:37:30.000000 voyage_agents-0.0.1/src/voyage_agents.egg-info/dependency_links.txt
--rw-rw-r--   0 ville     (1000) ville     (1000)       14 2024-06-02 13:37:30.000000 voyage_agents-0.0.1/src/voyage_agents.egg-info/top_level.txt
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/
+-rw-rw-r--   0 ville     (1000) ville     (1000)     1072 2024-06-01 13:48:05.000000 voyage_agents-0.0.2/LICENSE
+-rw-r--r--   0 ville     (1000) ville     (1000)     1069 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/PKG-INFO
+-rw-rw-r--   0 ville     (1000) ville     (1000)      494 2024-06-02 14:23:33.000000 voyage_agents-0.0.2/README.md
+-rw-r--r--   0 ville     (1000) ville     (1000)      566 2024-06-02 15:02:47.000000 voyage_agents-0.0.2/pyproject.toml
+-rw-rw-r--   0 ville     (1000) ville     (1000)       38 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/setup.cfg
+-rw-r--r--   0 ville     (1000) ville     (1000)      154 2024-06-02 15:02:54.000000 voyage_agents-0.0.2/setup.py
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/voyage_agents.egg-info/
+-rw-r--r--   0 ville     (1000) ville     (1000)     1069 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 ville     (1000) ville     (1000)      225 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 ville     (1000) ville     (1000)        1 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 ville     (1000) ville     (1000)       17 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/requires.txt
+-rw-rw-r--   0 ville     (1000) ville     (1000)        1 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/top_level.txt
```

### Comparing `voyage_agents-0.0.1/LICENSE` & `voyage_agents-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voyage_agents-0.0.1/PKG-INFO` & `voyage_agents-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: voyage-agents
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI agent and tool calling library for small local models using llama.cpp.
 Author: Ville Kuosmanen
 Project-URL: Homepage, https://github.com/villekuosmanen/voyage-agents
 Project-URL: Issues, https://github.com/villekuosmanen/voyage-agents/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: llama-cpp-python
 
 # voyage-agents
 AI Agents for local GPUs, by Voyage Robotics.
 
+Originally built for a hackathon in 24 hours.
+
 Find a 7B param multi-modal LLaVa x Mistral model in [HuggingFace](https://huggingface.co/villekuosmanen/LLaVa-1.6-Mistral-7B-llama.cpp/tree/main). You can also build models yourself using the llama.cpp library.
+
+This is a standalone package. You need to install llama_cpp as well to use voyage_agents.
+
+## Installation
+
+```
+pip install llama-cpp-python
+pip install voyage_agents
+```
```

### Comparing `voyage_agents-0.0.1/pyproject.toml` & `voyage_agents-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [project]
 name = "voyage-agents"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ville Kuosmanen" },
 ]
 description = "AI agent and tool calling library for small local models using llama.cpp."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "llama-cpp-python",
+]
 
 [project.urls]
 Homepage = "https://github.com/villekuosmanen/voyage-agents"
 Issues = "https://github.com/villekuosmanen/voyage-agents/issues"
```

### Comparing `voyage_agents-0.0.1/src/voyage_agents.egg-info/PKG-INFO` & `voyage_agents-0.0.2/voyage_agents.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: voyage-agents
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI agent and tool calling library for small local models using llama.cpp.
 Author: Ville Kuosmanen
 Project-URL: Homepage, https://github.com/villekuosmanen/voyage-agents
 Project-URL: Issues, https://github.com/villekuosmanen/voyage-agents/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: llama-cpp-python
 
 # voyage-agents
 AI Agents for local GPUs, by Voyage Robotics.
 
+Originally built for a hackathon in 24 hours.
+
 Find a 7B param multi-modal LLaVa x Mistral model in [HuggingFace](https://huggingface.co/villekuosmanen/LLaVa-1.6-Mistral-7B-llama.cpp/tree/main). You can also build models yourself using the llama.cpp library.
+
+This is a standalone package. You need to install llama_cpp as well to use voyage_agents.
+
+## Installation
+
+```
+pip install llama-cpp-python
+pip install voyage_agents
+```
```

