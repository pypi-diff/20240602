# Comparing `tmp/voyage_agents-0.0.2.tar.gz` & `tmp/voyage_agents-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyage_agents-0.0.2.tar", last modified: Sun Jun  2 15:03:49 2024, max compression
+gzip compressed data, was "voyage_agents-0.0.3.tar", last modified: Sun Jun  2 15:15:56 2024, max compression
```

## Comparing `voyage_agents-0.0.2.tar` & `voyage_agents-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,32 @@
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/
--rw-rw-r--   0 ville     (1000) ville     (1000)     1072 2024-06-01 13:48:05.000000 voyage_agents-0.0.2/LICENSE
--rw-r--r--   0 ville     (1000) ville     (1000)     1069 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/PKG-INFO
--rw-rw-r--   0 ville     (1000) ville     (1000)      494 2024-06-02 14:23:33.000000 voyage_agents-0.0.2/README.md
--rw-r--r--   0 ville     (1000) ville     (1000)      566 2024-06-02 15:02:47.000000 voyage_agents-0.0.2/pyproject.toml
--rw-rw-r--   0 ville     (1000) ville     (1000)       38 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/setup.cfg
--rw-r--r--   0 ville     (1000) ville     (1000)      154 2024-06-02 15:02:54.000000 voyage_agents-0.0.2/setup.py
-drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:03:49.133875 voyage_agents-0.0.2/voyage_agents.egg-info/
--rw-r--r--   0 ville     (1000) ville     (1000)     1069 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/PKG-INFO
--rw-rw-r--   0 ville     (1000) ville     (1000)      225 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/SOURCES.txt
--rw-rw-r--   0 ville     (1000) ville     (1000)        1 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/dependency_links.txt
--rw-rw-r--   0 ville     (1000) ville     (1000)       17 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/requires.txt
--rw-rw-r--   0 ville     (1000) ville     (1000)        1 2024-06-02 15:03:49.000000 voyage_agents-0.0.2/voyage_agents.egg-info/top_level.txt
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:56.112565 voyage_agents-0.0.3/
+-rw-rw-r--   0 ville     (1000) ville     (1000)     1072 2024-06-01 13:48:05.000000 voyage_agents-0.0.3/LICENSE
+-rw-r--r--   0 ville     (1000) ville     (1000)     1069 2024-06-02 15:15:56.112565 voyage_agents-0.0.3/PKG-INFO
+-rw-rw-r--   0 ville     (1000) ville     (1000)      494 2024-06-02 14:23:33.000000 voyage_agents-0.0.3/README.md
+-rw-r--r--   0 ville     (1000) ville     (1000)      566 2024-06-02 15:13:33.000000 voyage_agents-0.0.3/pyproject.toml
+-rw-rw-r--   0 ville     (1000) ville     (1000)       38 2024-06-02 15:15:56.112565 voyage_agents-0.0.3/setup.cfg
+-rw-r--r--   0 ville     (1000) ville     (1000)      181 2024-06-02 15:14:11.000000 voyage_agents-0.0.3/setup.py
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:56.104565 voyage_agents-0.0.3/voyage_agents/
+-rw-r--r--   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:41.000000 voyage_agents-0.0.3/voyage_agents/__init__.py
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:56.108565 voyage_agents-0.0.3/voyage_agents/agents/
+-rw-r--r--   0 ville     (1000) ville     (1000)      221 2024-06-02 14:41:49.000000 voyage_agents-0.0.3/voyage_agents/agents/__init__.py
+-rw-r--r--   0 ville     (1000) ville     (1000)     4028 2024-06-02 13:31:18.000000 voyage_agents-0.0.3/voyage_agents/agents/agent.py
+-rw-r--r--   0 ville     (1000) ville     (1000)     1866 2024-06-02 14:53:16.000000 voyage_agents-0.0.3/voyage_agents/agents/question_answerer.py
+-rw-rw-r--   0 ville     (1000) ville     (1000)     1348 2024-06-02 13:31:22.000000 voyage_agents-0.0.3/voyage_agents/agents/reflector.py
+-rw-r--r--   0 ville     (1000) ville     (1000)     2022 2024-06-02 13:31:26.000000 voyage_agents-0.0.3/voyage_agents/agents/tool_caller.py
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:56.108565 voyage_agents-0.0.3/voyage_agents/core/
+-rw-r--r--   0 ville     (1000) ville     (1000)      190 2024-06-02 14:55:59.000000 voyage_agents-0.0.3/voyage_agents/core/__init__.py
+-rw-r--r--   0 ville     (1000) ville     (1000)     2125 2024-06-02 13:30:46.000000 voyage_agents-0.0.3/voyage_agents/core/grammar.py
+-rw-r--r--   0 ville     (1000) ville     (1000)      601 2024-06-02 12:03:57.000000 voyage_agents-0.0.3/voyage_agents/core/manager.py
+-rw-r--r--   0 ville     (1000) ville     (1000)      157 2024-06-02 12:26:11.000000 voyage_agents-0.0.3/voyage_agents/core/message.py
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:56.108565 voyage_agents-0.0.3/voyage_agents/prompt/
+-rw-rw-r--   0 ville     (1000) ville     (1000)      122 2024-06-02 13:30:56.000000 voyage_agents-0.0.3/voyage_agents/prompt/__init__.py
+-rw-r--r--   0 ville     (1000) ville     (1000)     3162 2024-06-02 13:31:00.000000 voyage_agents-0.0.3/voyage_agents/prompt/prompt.py
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:56.108565 voyage_agents-0.0.3/voyage_agents/tool/
+-rw-r--r--   0 ville     (1000) ville     (1000)      109 2024-06-02 13:31:06.000000 voyage_agents-0.0.3/voyage_agents/tool/__init__.py
+-rw-r--r--   0 ville     (1000) ville     (1000)     1766 2024-06-02 13:13:53.000000 voyage_agents-0.0.3/voyage_agents/tool/tool.py
+drwxrwxr-x   0 ville     (1000) ville     (1000)        0 2024-06-02 15:15:56.108565 voyage_agents-0.0.3/voyage_agents.egg-info/
+-rw-r--r--   0 ville     (1000) ville     (1000)     1069 2024-06-02 15:15:56.000000 voyage_agents-0.0.3/voyage_agents.egg-info/PKG-INFO
+-rw-rw-r--   0 ville     (1000) ville     (1000)      669 2024-06-02 15:15:56.000000 voyage_agents-0.0.3/voyage_agents.egg-info/SOURCES.txt
+-rw-rw-r--   0 ville     (1000) ville     (1000)        1 2024-06-02 15:15:56.000000 voyage_agents-0.0.3/voyage_agents.egg-info/dependency_links.txt
+-rw-rw-r--   0 ville     (1000) ville     (1000)       17 2024-06-02 15:15:56.000000 voyage_agents-0.0.3/voyage_agents.egg-info/requires.txt
+-rw-rw-r--   0 ville     (1000) ville     (1000)       14 2024-06-02 15:15:56.000000 voyage_agents-0.0.3/voyage_agents.egg-info/top_level.txt
```

### Comparing `voyage_agents-0.0.2/LICENSE` & `voyage_agents-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voyage_agents-0.0.2/PKG-INFO` & `voyage_agents-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voyage-agents
-Version: 0.0.2
+Version: 0.0.3
 Summary: AI agent and tool calling library for small local models using llama.cpp.
 Author: Ville Kuosmanen
 Project-URL: Homepage, https://github.com/villekuosmanen/voyage-agents
 Project-URL: Issues, https://github.com/villekuosmanen/voyage-agents/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `voyage_agents-0.0.2/pyproject.toml` & `voyage_agents-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "voyage-agents"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ville Kuosmanen" },
 ]
 description = "AI agent and tool calling library for small local models using llama.cpp."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `voyage_agents-0.0.2/voyage_agents.egg-info/PKG-INFO` & `voyage_agents-0.0.3/voyage_agents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voyage-agents
-Version: 0.0.2
+Version: 0.0.3
 Summary: AI agent and tool calling library for small local models using llama.cpp.
 Author: Ville Kuosmanen
 Project-URL: Homepage, https://github.com/villekuosmanen/voyage-agents
 Project-URL: Issues, https://github.com/villekuosmanen/voyage-agents/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

