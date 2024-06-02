# Comparing `tmp/llmdo-0.1.0.tar.gz` & `tmp/llmdo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmdo-0.1.0.tar", last modified: Sun Jun  2 03:16:24 2024, max compression
+gzip compressed data, was "llmdo-0.2.0.tar", last modified: Sun Jun  2 05:27:24 2024, max compression
```

## Comparing `llmdo-0.1.0.tar` & `llmdo-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 03:16:24.298837 llmdo-0.1.0/
--rw-r--r--   0 randombk  (1000) randombk  (1000)        5 2024-06-02 02:31:23.000000 llmdo-0.1.0/.latest-version.generated.txt
--rw-r--r--   0 randombk  (1000) randombk  (1000)    35185 2024-06-02 02:28:08.000000 llmdo-0.1.0/LICENSE
--rw-r--r--   0 randombk  (1000) randombk  (1000)     3277 2024-06-02 03:16:24.298837 llmdo-0.1.0/PKG-INFO
--rw-r--r--   0 randombk  (1000) randombk  (1000)     2901 2024-06-02 03:15:42.000000 llmdo-0.1.0/README.md
--rw-r--r--   0 randombk  (1000) randombk  (1000)      575 2024-06-02 03:12:54.000000 llmdo-0.1.0/pyproject.toml
--rw-r--r--   0 randombk  (1000) randombk  (1000)       38 2024-06-02 03:16:24.298837 llmdo-0.1.0/setup.cfg
-drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 03:16:24.298837 llmdo-0.1.0/src/
-drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 03:16:24.298837 llmdo-0.1.0/src/llmdo/
--rw-r--r--   0 randombk  (1000) randombk  (1000)       23 2024-06-01 22:27:37.000000 llmdo-0.1.0/src/llmdo/__init__.py
--rw-r--r--   0 randombk  (1000) randombk  (1000)      109 2024-06-02 03:15:39.000000 llmdo-0.1.0/src/llmdo/__main__.py
--rw-r--r--   0 randombk  (1000) randombk  (1000)     1345 2024-06-02 02:05:00.000000 llmdo-0.1.0/src/llmdo/config.py
-drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 03:16:24.298837 llmdo-0.1.0/src/llmdo/dispatchers/
--rw-r--r--   0 randombk  (1000) randombk  (1000)     6236 2024-06-02 03:13:24.000000 llmdo-0.1.0/src/llmdo/dispatchers/DefaultDispatcher.py
--rw-r--r--   0 randombk  (1000) randombk  (1000)       23 2024-06-02 00:28:07.000000 llmdo-0.1.0/src/llmdo/dispatchers/__init__.py
--rw-r--r--   0 randombk  (1000) randombk  (1000)     6368 2024-06-02 03:15:39.000000 llmdo-0.1.0/src/llmdo/llmdo.py
--rw-r--r--   0 randombk  (1000) randombk  (1000)      852 2024-06-02 00:22:59.000000 llmdo-0.1.0/src/llmdo/util.py
-drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 03:16:24.298837 llmdo-0.1.0/src/llmdo.egg-info/
--rw-r--r--   0 randombk  (1000) randombk  (1000)     3277 2024-06-02 03:16:24.000000 llmdo-0.1.0/src/llmdo.egg-info/PKG-INFO
--rw-r--r--   0 randombk  (1000) randombk  (1000)      440 2024-06-02 03:16:24.000000 llmdo-0.1.0/src/llmdo.egg-info/SOURCES.txt
--rw-r--r--   0 randombk  (1000) randombk  (1000)        1 2024-06-02 03:16:24.000000 llmdo-0.1.0/src/llmdo.egg-info/dependency_links.txt
--rw-r--r--   0 randombk  (1000) randombk  (1000)       45 2024-06-02 03:16:24.000000 llmdo-0.1.0/src/llmdo.egg-info/entry_points.txt
--rw-r--r--   0 randombk  (1000) randombk  (1000)       34 2024-06-02 03:16:24.000000 llmdo-0.1.0/src/llmdo.egg-info/requires.txt
--rw-r--r--   0 randombk  (1000) randombk  (1000)        6 2024-06-02 03:16:24.000000 llmdo-0.1.0/src/llmdo.egg-info/top_level.txt
+drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 05:27:24.655716 llmdo-0.2.0/
+-rw-r--r--   0 randombk  (1000) randombk  (1000)        5 2024-06-02 04:38:23.000000 llmdo-0.2.0/.latest-version.generated.txt
+-rw-r--r--   0 randombk  (1000) randombk  (1000)    35185 2024-06-02 02:28:08.000000 llmdo-0.2.0/LICENSE
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     3302 2024-06-02 05:27:24.655716 llmdo-0.2.0/PKG-INFO
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     2901 2024-06-02 03:15:42.000000 llmdo-0.2.0/README.md
+-rw-r--r--   0 randombk  (1000) randombk  (1000)      591 2024-06-02 04:07:55.000000 llmdo-0.2.0/pyproject.toml
+-rw-r--r--   0 randombk  (1000) randombk  (1000)       38 2024-06-02 05:27:24.655716 llmdo-0.2.0/setup.cfg
+drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 05:27:24.655716 llmdo-0.2.0/src/
+drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 05:27:24.655716 llmdo-0.2.0/src/llmdo/
+-rw-r--r--   0 randombk  (1000) randombk  (1000)       23 2024-06-01 22:27:37.000000 llmdo-0.2.0/src/llmdo/__init__.py
+-rw-r--r--   0 randombk  (1000) randombk  (1000)      109 2024-06-02 03:15:39.000000 llmdo-0.2.0/src/llmdo/__main__.py
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     1842 2024-06-02 05:16:07.000000 llmdo-0.2.0/src/llmdo/config.py
+drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 05:27:24.655716 llmdo-0.2.0/src/llmdo/dispatchers/
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     1271 2024-06-02 05:24:11.000000 llmdo-0.2.0/src/llmdo/dispatchers/AnthropicDispatcher.py
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     7501 2024-06-02 04:37:22.000000 llmdo-0.2.0/src/llmdo/dispatchers/DefaultDispatcher.py
+-rw-r--r--   0 randombk  (1000) randombk  (1000)       23 2024-06-02 00:28:07.000000 llmdo-0.2.0/src/llmdo/dispatchers/__init__.py
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     6751 2024-06-02 05:23:20.000000 llmdo-0.2.0/src/llmdo/llmdo.py
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     1218 2024-06-02 05:13:32.000000 llmdo-0.2.0/src/llmdo/util.py
+drwxr-xr-x   0 randombk  (1000) randombk  (1000)        0 2024-06-02 05:27:24.655716 llmdo-0.2.0/src/llmdo.egg-info/
+-rw-r--r--   0 randombk  (1000) randombk  (1000)     3302 2024-06-02 05:27:24.000000 llmdo-0.2.0/src/llmdo.egg-info/PKG-INFO
+-rw-r--r--   0 randombk  (1000) randombk  (1000)      485 2024-06-02 05:27:24.000000 llmdo-0.2.0/src/llmdo.egg-info/SOURCES.txt
+-rw-r--r--   0 randombk  (1000) randombk  (1000)        1 2024-06-02 05:27:24.000000 llmdo-0.2.0/src/llmdo.egg-info/dependency_links.txt
+-rw-r--r--   0 randombk  (1000) randombk  (1000)       45 2024-06-02 05:27:24.000000 llmdo-0.2.0/src/llmdo.egg-info/entry_points.txt
+-rw-r--r--   0 randombk  (1000) randombk  (1000)       44 2024-06-02 05:27:24.000000 llmdo-0.2.0/src/llmdo.egg-info/requires.txt
+-rw-r--r--   0 randombk  (1000) randombk  (1000)        6 2024-06-02 05:27:24.000000 llmdo-0.2.0/src/llmdo.egg-info/top_level.txt
```

### Comparing `llmdo-0.1.0/LICENSE` & `llmdo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmdo-0.1.0/PKG-INFO` & `llmdo-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: llmdo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ask GPT to run a command
 Author-email: David Li <david@david-li.com>
 License: GPL-3.0
 Keywords: llm,gpt,cli
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.30.5
+Requires-Dist: anthropic
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # llmdo
 
 `llmdo` is a Python application that leverages Large Language Models (LLMs) to translate English requests into shell commands. It provides a convenient way to interact with your system using natural language.
```

### Comparing `llmdo-0.1.0/README.md` & `llmdo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `llmdo-0.1.0/pyproject.toml` & `llmdo-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 dynamic = ["version"]
 license = {text = "GPL-3.0"}
 requires-python = ">=3.8"
 readme = "README.md"
 authors = [{name = "David Li", email = "david@david-li.com"}]
 keywords = ["llm", "gpt", "cli"]
 dependencies = [
-  "openai>=1.30.5"
+  "openai>=1.30.5",
+  "anthropic",
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [project.scripts]
 llmdo = "llmdo.__main__:cli"
```

### Comparing `llmdo-0.1.0/src/llmdo/config.py` & `llmdo-0.2.0/src/llmdo/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import os
 from io import StringIO
 from dataclasses import dataclass, asdict
 
 @dataclass
 class Config:
-  default_model: str = 'gpt-3.5-turbo'
+  default_model: str = 'gpt-4o'
 
   openai_api_key: str = ''
   claude_api_key: str = ''
 
   local_uri: str = 'http://localhost:8000/v1'
   local_api_key: str = ''
 
-  temperature: float = 0.4
+  temperature: float = 0.2
 
   # Always run in yolo mode
   i_like_to_live_dangerously: bool = False
 
 
   @staticmethod
   def load_config(config_file: str) -> "Config":
@@ -29,19 +29,39 @@
   def from_dict(cls, d: dict) -> "Config":
     return cls(
       default_model = d.get('default_model', 'gpt-3.5-turbo'),
       openai_api_key = d.get('openai_api_key', ''),
       claude_api_key = d.get('claude_api_key', ''),
       local_uri = d.get('local_uri', 'http://localhost:8000/v1'),
       local_api_key = d.get('local_api_key', ''),
-      temperature = d.get('temperature', 0.4),
+      temperature = d.get('temperature', 0.2),
       i_like_to_live_dangerously = d.get('i_like_to_live_dangerously', False),
     )
 
 
+  @property
+  def effective_openai_key(self) -> str:
+    if len(self.openai_api_key) > 0:
+      return self.openai_api_key
+    elif len(os.environ.get('OPENAI_API_KEY', '')) > 0:
+      return os.environ['OPENAI_API_KEY']
+    else:
+      return ''
+
+
+  @property
+  def effective_claude_key(self) -> str:
+    if len(self.claude_api_key) > 0:
+      return self.claude_api_key
+    elif len(os.environ.get('ANTHROPIC_API_KEY', '')) > 0:
+      return os.environ['ANTHROPIC_API_KEY']
+    else:
+      return ''
+
+
   def save_config(self, config_file: str):
     # There are cases where the config location is read-only. Swallow the exception
     try:
       os.makedirs(os.path.dirname(config_file), exist_ok=True)
       with open(config_file, 'w') as f:
         json.dump(asdict(self), f, indent=4)
     except Exception as e:
```

### Comparing `llmdo-0.1.0/src/llmdo/dispatchers/DefaultDispatcher.py` & `llmdo-0.2.0/src/llmdo/dispatchers/DefaultDispatcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List
 import textwrap
 
 from openai import OpenAI
 from openai.types.chat.chat_completion_message import ChatCompletionMessage
 
 from ..config import Config
-
+from ..util import unquote_all
 
 class DefaultDispatcher:
   """
   Default fallback dispatcher for llmdo, used when there isn't a more specific
   dispatcher available. This dispatcher can be extended to customize the
   system prompt or to use a different API.
   """
@@ -35,24 +35,28 @@
     if self.verbose:
       print(f"[DEBUG]: System prompt:\n{system_prompt}")
 
     client = OpenAI(
       base_url=None if self.uri == '' else self.uri,
       api_key='NA' if self.key == '' else self.key,
     )
-    response = client.chat.completions.create(
+    message = client.chat.completions.create(
         model=self.model,
         temperature=self.config.temperature,
         messages=[
           { "role": "system", "content": system_prompt },
           { "role": "user", "content": request_str }
         ],
     )
 
-    return self._clean_output(response.choices[0].message.content.split('\n'))
+    response = message.choices[0].message.content
+    if self.verbose:
+      print(f"[DEBUG]: Response:\n{response}")
+
+    return self._clean_output(response.split('\n'))
 
 
   def _max_context_length(self) -> int:
     """
     Returns the input maximum length of the LLM model.
     """
     return 4096  # Assume the worst case scenario (i.e. gpt-3.5-turbo-instruct supports a 4K window)
@@ -88,14 +92,29 @@
     Returns the contents of the current working directory.
     The `summarize_factor` is used to suppress overly long directory listings.
     """
     items = os.listdir()
     return items[:int(len(items) * summarize_factor)]
 
 
+  def _additional_context(self, summarize_factor: int) -> str:
+    """
+    Returns additional situational context to be included in the system prompt.
+    """
+
+    lines = []
+
+    # If lsb_release is available, include the OS version
+    if os.path.exists('/usr/bin/lsb_release'):
+      lines.append('The OS is:')
+      lines.append(os.popen('/usr/bin/lsb_release -d').read().strip())
+
+    return '\n'.join(lines)
+
+
   def _available_env(self, summarize_factor: int) -> List[str]:
     """
     Returns the list of available environment variables.
     The `summarize_factor` is used to limit the number of results.
     This method also omits some common environment variables that are usually not useful.
     """
     items = set(os.environ.keys())
@@ -144,30 +163,33 @@
     """
     max_length = self._max_system_prompt_length(request_str)
     summarize_factor = 1.0  # Percentage of the env and directory information to include in the prompt
 
     def get_prompt(factor: float) -> str:
       nl = '\n'
       return textwrap.dedent(f"""
-        You are an AI helping the user perform tasks in a POSIX-compliant shell. The user will give you a request,
+        You are an AI helping the user perform tasks in a Bash shell. The user will give you a request,
         and you will generate one or more shell commands to fulfill that request. You can use any shell constructs,
         including pipes, redirection, and loops. You can also use any commands available in the shell environment.
         The shell is configured with `set -e`, so generate appropriate error handling for commands that are allowed
         to fail.
 
         The user is currently logged in as `{self._whoami()}` and the current working directory is `{self._cwd()}`.
 
         The current directory contains the following files: \n{nl.join([f"         - {i}" for i in self._ls(factor)])}
 
         You can refer to the following environment variables: \n{nl.join([f"         - {i}" for i in self._available_env(factor)])}
 
-        YOU MUST RESPOND WITH ONLY VALID SHELL COMMANDS. DO NOT INCLUDE ANYTHING ELSE IN YOUR RESPONSE.
+        \n{self._additional_context(factor)}
+
         Make sure you output valid shell commands, paying special attention to quoting and escaping.
         Do not wrap the response in quotes or backticks. If you want to provide additional information,
         please include it in a shell comment (i.e. `#`) or use `echo`.
+
+        YOU MUST RESPOND WITH ONLY VALID SHELL COMMANDS. DO NOT INCLUDE ANYTHING ELSE IN YOUR RESPONSE.
       """)
 
     prompt = get_prompt(summarize_factor)
     while len(prompt) // 4 > max_length:
       # Reduce the amount of information in the prompt
       summarize_factor = summarize_factor * 0.9 * (max_length / (len(prompt) // 4))
       prompt = get_prompt(summarize_factor)
@@ -175,12 +197,33 @@
     return prompt
 
 
   def _clean_output(self, output: List[str]) -> List[str]:
     """
     Cleans the output by removing any leading or trailing whitespace and other common mistakes.
     """
-    return [
-      i.strip()
-      for i in output
-      if i.strip() != '' and i.strip() != '```'
+
+    # Remove trailing and leading whitespace. This does remove whitespace in front of the command, which does have
+    # meaning within bash (skip writing history), but it's fine to remove it this context.
+    cleaned = [i.strip() for i in output]
+
+    cleaned = [
+      # Remove quotes around the commands
+      unquote_all(i, ['`', '"', "'"])
+
+      for i in cleaned
+
+      if not (
+        # Heuristic: Remove empty lines and code blocks
+        (i == '')
+        or (i == '```')
+        or (i == '```bash')
+        or (i == '```shell')
+        or (i == '```sh')
+
+        # Heuristic: Remove lines where the LLM is trying to be conversational
+        or (i.startswith('Sure'))  # i.e. "Sure! Here is..."
+        or (i.startswith('Here'))  # i.e. "Here is..."
+      )
     ]
+
+    return cleaned
```

### Comparing `llmdo-0.1.0/src/llmdo/llmdo.py` & `llmdo-0.2.0/src/llmdo/llmdo.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import argparse
 import os
 import subprocess
 
 from typing import List, Optional, Dict, Set, Tuple
 
 from .config import Config
-from .util import eprint, ethrow
+from .util import ethrow
 from .dispatchers.DefaultDispatcher import DefaultDispatcher
+from .dispatchers.AnthropicDispatcher import AnthropicDispatcher
 
 class LlmDo(object):
   def __init__(self):
     parser = argparse.ArgumentParser(
       description='Ask GPT to run a command',
       usage='llmdo [options] <request>',
       add_help = True,
@@ -78,61 +79,66 @@
     return config
 
 
   def list_models(self):
     print('Available models:')
     print(f'Models can be configured via {self.args.config}\n')
 
-    max_just_name = max([len(module) for (module, _, _, _) in self.model_list])
+    max_just_name = max([len(module) for (module, _, _, _, _) in self.model_list])
     max_just_avail = len('NOT AVAILABLE')
 
-    for (model, avail, help, _) in self.model_list:
+    for (model, avail, help, _, model_id) in self.model_list:
       print(
         model.ljust(max_just_name + 2) +
         ('OK' if avail else 'NOT AVAILABLE').rjust(max_just_avail) +
         " | "
-        f"{help}"
+        f"({model_id}) {help}"
       )
 
 
   def load_models(self) -> List[Tuple[str, bool, str, str]]:
-    openai_available = len(self.config.openai_api_key) > 0
+    openai_available = len(self.config.effective_openai_key) > 0
     openai_str = "Ready" if openai_available else f"Requires OpenAI API key"
 
-    claude_available = len(self.config.claude_api_key) > 0
+    claude_available = len(self.config.effective_claude_key) > 0
     claude_str = "Ready" if claude_available else f"Requires Claude API key"
 
     local_available = len(self.config.local_uri) > 0
     local_str = f"Ready - {self.config.local_uri}" if local_available else f"Requires local LLM API URI"
 
     return [
-      ('local', local_available, local_str, 'LOCAL'),
-      ('gpt-4o', openai_available, openai_str, 'OPENAI'),
-      ('gpt-3.5-turbo-instruct', openai_available, openai_str, 'OPENAI'),
-      ('gpt-4-turbo', openai_available, openai_str, 'OPENAI'),
-      ('claude-3-opus', claude_available, claude_str, 'CLAUDE'),
-      ('claude-3-sonnet', claude_available, claude_str, 'CLAUDE'),
-      ('claude-3-haiku', claude_available, claude_str, 'CLAUDE'),
+      ('local', local_available, local_str, 'LOCAL', 'local'),
+      ('gpt-4o', openai_available, openai_str, 'OPENAI', 'gpt-4o'),
+      ('gpt-3.5-turbo-instruct', openai_available, openai_str, 'OPENAI', 'gpt-3.5-turbo-instruct'),
+      ('gpt-4-turbo', openai_available, openai_str, 'OPENAI', 'gpt-4-turbo'),
+      ('claude-3-opus', claude_available, claude_str, 'CLAUDE', 'claude-3-opus-20240229'),
+      ('claude-3-sonnet', claude_available, claude_str, 'CLAUDE', 'claude-3-opus-20240229'),
+      ('claude-3-haiku', claude_available, claude_str, 'CLAUDE', 'claude-3-opus-20240307'),
     ]
 
 
   def dispatch_request(self, request: str) -> List[str]:
-    (model_id, _, _, model_type) = self.models[self.selected_model]
+    (_, _, _, model_type, model_id) = self.models[self.selected_model]
 
     # TOTO: Implement dispatcher selection based on the chosen model
     if model_type == 'OPENAI':
       dispatcher = DefaultDispatcher(
         uri = '',  # Defaults to None, which uses the OpenAI API
-        key = self.config.openai_api_key,
+        key = self.config.effective_openai_key,
         model = model_id,
         config = self.config,
         verbose=self.args.verbose,
       )
     elif model_type == 'CLAUDE':
-      ethrow('Claude API not implemented yet')
+      dispatcher = AnthropicDispatcher(
+        key = self.config.effective_claude_key,
+        model = model_id,
+        config = self.config,
+        verbose=self.args.verbose,
+      )
     elif model_type == 'LOCAL':
       dispatcher = DefaultDispatcher(
         uri = self.config.local_uri,
         key = self.config.local_api_key,
         model = model_id,
         config = self.config,
         verbose=self.args.verbose,
@@ -178,11 +184,11 @@
     process.stdin.close()
 
     # Read the output of the command
     while process.stdout.readable():
         output = process.stdout.readline()
         if not output:
             break
-        print(output.strip())
+        print(output.rstrip())
 
     # Close the stdin and wait for the process to finish
     process.wait()
```

### Comparing `llmdo-0.1.0/src/llmdo.egg-info/PKG-INFO` & `llmdo-0.2.0/src/llmdo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: llmdo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ask GPT to run a command
 Author-email: David Li <david@david-li.com>
 License: GPL-3.0
 Keywords: llm,gpt,cli
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.30.5
+Requires-Dist: anthropic
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # llmdo
 
 `llmdo` is a Python application that leverages Large Language Models (LLMs) to translate English requests into shell commands. It provides a convenient way to interact with your system using natural language.
```

