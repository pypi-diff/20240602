# Comparing `tmp/shgpt-0.3.0.tar.gz` & `tmp/shgpt-0.3.1.tar.gz`

## Comparing `shgpt-0.3.0.tar` & `shgpt-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 shgpt-0.3.0/Makefile
--rw-r--r--   0        0        0    83463 2020-02-02 00:00:00.000000 shgpt-0.3.0/roles.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/__main__.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/app.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/version.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/api/history.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/api/ollama.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/tui/app.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/tui/app.tcss
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/utils/common.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/utils/conf.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 shgpt-0.3.0/shgpt/utils/http.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 shgpt-0.3.0/.gitignore
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 shgpt-0.3.0/README.md
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 shgpt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 shgpt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 shgpt-0.3.1/Makefile
+-rw-r--r--   0        0        0    83463 2020-02-02 00:00:00.000000 shgpt-0.3.1/roles.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/__main__.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/app.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/version.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/api/history.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/api/ollama.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/tui/app.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/tui/app.tcss
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/utils/common.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/utils/conf.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 shgpt-0.3.1/shgpt/utils/http.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 shgpt-0.3.1/.gitignore
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 shgpt-0.3.1/README.md
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 shgpt-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 shgpt-0.3.1/PKG-INFO
```

### Comparing `shgpt-0.3.0/roles.json` & `shgpt-0.3.1/roles.json`

 * *Files identical despite different names*

### Comparing `shgpt-0.3.0/shgpt/app.py` & `shgpt-0.3.1/shgpt/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import argparse, sys, readline
+import argparse
+import sys
 from os import makedirs
 from .api.ollama import Ollama
 from .version import __version__
 from .utils.conf import *
 from .utils.common import *
 from .tui.app import ShellGPTApp
-from functools import partial
+
 
 def init_app():
-    print(f'Create {CONF_PATH}...')
+    print(f"Create {CONF_PATH}...")
     makedirs(CONF_PATH, exist_ok=True)
 
+
 def read_action(cmd):
     if IS_TTY:
-        action = input("(E)xecute, (Y)ank or (C)ontinue(default): ")
+        action = input("(E)xecute, (Y)ank or Continue(default): ")
         action = action.upper()
         if action == "E":
             print(execute_cmd(cmd))
         elif action == "Y":
             copy_text(cmd)
 
 
@@ -27,85 +29,107 @@
         self.llm = Ollama(url, model, role, timeout)
 
     def tui(self, initial_prompt):
         app = ShellGPTApp(self.llm, initial_prompt)
         app.run()
 
     def repl(self, initial_prompt):
-        print(r'''
+        print(r"""
 __      __   _                    _         ___ _        _ _  ___ ___ _____
 \ \    / /__| |__ ___ _ __  ___  | |_ ___  / __| |_  ___| | |/ __| _ \_   _|
  \ \/\/ / -_) / _/ _ \ '  \/ -_) |  _/ _ \ \__ \ ' \/ -_) | | (_ |  _/ | |
   \_/\_/\___|_\__\___/_|_|_\___|  \__\___/ |___/_||_\___|_|_|\___|_|   |_|
-''')
+""")
         self.infer(initial_prompt)
         while True:
             prompt = input("> ")
-            if 'exit' == prompt:
+            if "exit" == prompt:
                 sys.exit(0)
 
             self.infer(prompt)
 
-
     def infer(self, prompt):
         if prompt == "":
             return
 
-        buf = ''
+        buf = ""
         try:
             for r in self.llm.generate(prompt):
                 buf += r
-                print(r, end='')
+                print(r, end="")
 
             print()
-            if self.role == 'shell':
+            if self.role == "shell":
                 read_action(buf)
         except Exception as e:
             print(f"Error when infer: ${e}")
 
 
 def main():
     prog = sys.argv[0]
     parser = argparse.ArgumentParser(
         prog=prog,
-        description='Make Shell easy to use with power of LLM!')
-    parser.add_argument('-V', '--version', action='version', version='%(prog)s ' + __version__)
-    parser.add_argument('-s', '--shell', action='store_true', help='Infer shell command')
-    parser.add_argument('-r', '--role', default='default', help='System role message')
-    parser.add_argument('-l', '--repl', action='store_true', help='Start interactive REPL')
-    parser.add_argument('-t', '--tui', action='store_true', help='Start TUI')
-    parser.add_argument('--init', action='store_true', help='Init config')
-    parser.add_argument('--timeout', type=int, help='Timeout for each inference request', default=INFER_TIMEOUT)
-    parser.add_argument('--ollama-url', default=OLLAMA_URL, help='Ollama URL')
-    parser.add_argument('-m', '--ollama-model', default='llama3', help='Ollama model')
-    parser.add_argument('-v', '--verbose', action='store_true', help='verbose mode')
-    parser.add_argument('prompt', metavar='<prompt>', nargs='*')
+        description="Chat with LLM in your terminal, be it shell generator, story teller, linux-terminal, etc.",
+    )
+    parser.add_argument(
+        "-V", "--version", action="version", version="%(prog)s " + __version__
+    )
+    parser.add_argument(
+        "-s",
+        "--shell",
+        action="store_true",
+        help="System role set to `shell`",
+    )
+    parser.add_argument(
+        "-c",
+        "--code",
+        action="store_true",
+        help="System role set to `code`",
+    )
+    parser.add_argument("-r", "--role", default="default", help="System role to use")
+    parser.add_argument(
+        "-l", "--repl", action="store_true", help="Start interactive REPL"
+    )
+    parser.add_argument("-t", "--tui", action="store_true", help="Start TUI mode")
+    parser.add_argument("--init", action="store_true", help="Init config")
+    parser.add_argument(
+        "--timeout",
+        type=int,
+        help="Timeout for each inference request",
+        default=INFER_TIMEOUT,
+    )
+    parser.add_argument("--ollama-url", default=OLLAMA_URL, help="Ollama URL")
+    parser.add_argument("-m", "--ollama-model", default="llama3", help="Ollama model")
+    parser.add_argument("-v", "--verbose", action="store_true", help="verbose mode")
+    parser.add_argument("prompt", metavar="<prompt>", nargs="*")
     args = parser.parse_args()
     set_verbose(args.verbose)
 
     if args.init:
         init_app()
         sys.exit(0)
 
     sin = read_stdin()
-    prompt = ' '.join(args.prompt)
+    prompt = " ".join(args.prompt)
     if sin is not None:
-        prompt = f'{sin}\n\n{prompt}'
+        prompt = f"{sin}\n\n{prompt}"
 
     if args.repl:
         app_mode = AppMode.REPL
     elif args.tui:
         app_mode = AppMode.TUI
     else:
         app_mode = AppMode.TUI if len(prompt) == 0 else AppMode.Direct
 
     role = args.role
     # tui default to shell role
     if args.shell or app_mode == AppMode.TUI:
-        role = 'shell'
+        role = "shell"
+    elif args.code:
+        role = "code"
 
     if role not in ROLE_CONTENT:
         try:
             load_roles_from_config()
         except Exception as e:
             debug_print(f"Error when load roles: ${e}")
```

### Comparing `shgpt-0.3.0/shgpt/api/ollama.py` & `shgpt-0.3.1/shgpt/api/ollama.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-import json, os
+import json
+import os
 from ..utils.http import TimeoutSession
 from ..utils.common import *
 from ..utils.conf import *
 from .history import DummyHistory, FileHistory
 
-HIST_SEP = '=========='
+HIST_SEP = "=========="
+
 
 # https://github.com/ollama/ollama/blob/main/docs/api.md#generate-a-completion
 class Ollama(object):
     def __init__(self, base_url, model, role, timeout):
         self.base_url = base_url
         self.http_session = TimeoutSession(timeout=timeout)
         if ENABLE_HISTORY:
-            self.history_file = FileHistory(os.path.join(CONF_PATH, 'history'))
+            self.history_file = FileHistory(os.path.join(CONF_PATH, "history"))
         else:
             self.history_file = DummyHistory()
         self.model = model
         self.role = role
 
     def generate(self, prompt, stream=True):
-        url = self.base_url + '/api/chat'
-        debug_print(f"generate: {prompt} to {url} with model {self.model} role {self.role} and stream {stream}")
+        url = self.base_url + "/api/chat"
+        debug_print(
+            f"generate: {prompt} to {url} with model {self.model} role {self.role} and stream {stream}"
+        )
         system_content = ROLE_CONTENT.get(self.role, self.role)
         payload = {
-            'messages': [
-                {'role': 'system', 'content': system_content, 'name': 'ShellGPT'},
-                {'role': 'user', 'content': prompt, 'name': 'user'},
+            "messages": [
+                {"role": "system", "content": system_content, "name": "ShellGPT"},
+                {"role": "user", "content": prompt, "name": "user"},
             ],
-            'model': self.model,
-            'stream': stream
+            "model": self.model,
+            "stream": stream,
         }
-        debug_print(f'Infer message: {payload}')
+        debug_print(f"Infer message: {payload}")
         r = self.http_session.post(url, json=payload, stream=stream)
         if r.status_code != 200:
             raise Exception("Error: " + r.text)
 
-        answer = ''
+        answer = ""
         for item in r.iter_content(chunk_size=None):
             resp = json.loads(item)
-            if resp['done'] is False:
-                content = resp['message']['content']
+            if resp["done"] is False:
+                content = resp["message"]["content"]
                 answer += content
                 yield content
             else:
-                self.history_file.write(fr'''{now_ms()},{resp['eval_duration']},{resp['eval_count']}
+                self.history_file.write(rf"""{now_ms()},{resp['eval_duration']},{resp['eval_count']}
 {prompt}
 {HIST_SEP}
 {answer}
 {HIST_SEP}
-''')
+""")
```

### Comparing `shgpt-0.3.0/shgpt/tui/app.py` & `shgpt-0.3.1/shgpt/tui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from textual.app import App, ComposeResult
 from textual.widgets import Header, Footer, Static, TextArea, Button
 from typing import Optional
 from ..utils.common import *
 
+
 class PromptInput(Static):
     def __init__(self, prompt):
         self.initial_prompt = prompt
         super().__init__()
 
     def compose(self) -> ComposeResult:
         yield TextArea(self.initial_prompt, id="prompt_input")
@@ -77,15 +78,15 @@
             return
 
         self.has_inflight_req = True
         try:
             self.action_infer_inner()
         except Exception as e:
             answer_output = self.query_one("#answer_output")
-            answer_output.load_text(f'Error when infer: {e}')
+            answer_output.load_text(f"Error when infer: {e}")
         finally:
             self.has_inflight_req = False
 
     def get_prompt_input(self) -> Optional[str]:
         prompt_input = self.query_one("#prompt_input")
         prompt = prompt_input.text.strip()
         return None if prompt == "" else prompt
@@ -99,30 +100,29 @@
         prompt = self.get_prompt_input()
         if prompt is None:
             return
 
         debug_print(f"infer {prompt}")
         # llm infer
         resp = self.llm.generate(prompt, True)
-        buf = ''
+        buf = ""
         for item in resp:
             buf += item
 
         debug_print(f"infer ret {buf}")
         answer_output = self.query_one("#answer_output")
         answer_output.load_text(buf)
 
     def action_copy(self) -> None:
         text = self.get_answer_output()
         if text is None:
             return
 
         copy_text(text)
 
-
     def action_run(self) -> None:
         text = self.get_answer_output()
         if text is None:
             return
 
         cmd = text
         output = execute_cmd(cmd)
```

### Comparing `shgpt-0.3.0/shgpt/utils/common.py` & `shgpt-0.3.1/shgpt/utils/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 from enum import Enum
 from typing import Optional
 from datetime import datetime
-import re, platform, os, subprocess, sys
+import re
+import platform
+import os
+import subprocess
+import sys
 import pyperclip
 
 IS_VERBOSE = False
 OS_NAME = platform.system()
 IS_TTY = sys.stdin.isatty()
 
+
 def get_shell_type():
     if OS_NAME in ("Windows", "nt"):
         is_powershell = len(os.getenv("PSModulePath", "").split(os.pathsep)) >= 3
         return "powershell.exe" if is_powershell else "cmd.exe"
     return os.path.basename(os.getenv("SHELL", "/bin/sh"))
 
+
 SHELL = get_shell_type()
 
+
 def set_verbose(v):
     global IS_VERBOSE
     IS_VERBOSE = v
 
 
 def debug_print(msg):
     if IS_VERBOSE:
         print(msg)
 
 
-
 def get_executable_script(text: str) -> Optional[str]:
-    script_blocks = re.findall('```(.*?)\n(.*?)```', text, re.DOTALL)
+    script_blocks = re.findall("```(.*?)\n(.*?)```", text, re.DOTALL)
     if len(script_blocks) == 0:
         return None
     else:
         return script_blocks[0][1].strip()
 
 
 def now_ms():
     return int(datetime.now().timestamp() * 1000)
 
 
 def read_stdin():
     if IS_TTY:
         return None
     else:
-        buf = ''
+        buf = ""
         for line in sys.stdin:
             buf += line
 
         return buf
 
 
 def copy_text(text):
@@ -55,10 +61,10 @@
 
 
 def execute_cmd(cmd):
     return subprocess.getoutput(cmd)
 
 
 class AppMode(Enum):
-    Direct = 1,
-    TUI = 2,
-    REPL = 3,
+    Direct = (1,)
+    TUI = (2,)
+    REPL = (3,)
```

### Comparing `shgpt-0.3.0/shgpt/utils/conf.py` & `shgpt-0.3.1/shgpt/utils/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from os import path, environ
 import json
 from .common import OS_NAME, SHELL
 
 # Configuration
-CONF_PATH = path.expanduser(environ.get('SHELLGPT_CONF_DIR', '~/.shellgpt'))
-OLLAMA_URL = environ.get('SHELLGPT_OLLAMA_URL', "http://127.0.0.1:11434")
-OLLAMA_MODEL = environ.get('SHELLGPT_OLLAMA_MODEL', 'llama3')
-INFER_TIMEOUT = int(environ.get('SHELLGPT_INFER_TIMEOUT', '15'))  # seconds
-ENABLE_HISTORY = int(environ.get('SHELLGPT_ENABLE_HISTORY', '0')) == 1
+CONF_PATH = path.expanduser(environ.get("SHELLGPT_CONF_DIR", "~/.shellgpt"))
+OLLAMA_URL = environ.get("SHELLGPT_OLLAMA_URL", "http://127.0.0.1:11434")
+OLLAMA_MODEL = environ.get("SHELLGPT_OLLAMA_MODEL", "llama3")
+INFER_TIMEOUT = int(environ.get("SHELLGPT_INFER_TIMEOUT", "15"))  # seconds
+ENABLE_HISTORY = int(environ.get("SHELLGPT_ENABLE_HISTORY", "0")) == 1
 
 # There are different roles for different types of prompts
 ROLE_CONTENT = {
-    'default': '',
-    'code': '''
+    "default": "",
+    "code": """
 Provide only code as output without any description.
 Provide only code in plain text format without Markdown formatting.
 Do not include symbols such as ``` or ```python.
 If there is a lack of details, provide most logical solution.
 You are not allowed to ask for more details.
 For example if the prompt is "Hello world Python", you should return "print('Hello world')".
-    ''',
-    'shell': '''
+    """,
+    "shell": """
     You are a shell script assistant on {os_name} running {shell},
     Output the best matching shell commands without any other information, or any quotes.
     Make sure it's valid shell command.
-    '''.format(os_name=OS_NAME, shell=SHELL),
+    """.format(os_name=OS_NAME, shell=SHELL),
     # commit message
-    'cm': f'''
+    "cm": """
     Generate git commit message for this changes.
-    ''',
+    """,
 }
 
 
 def load_roles_from_config():
-    conf_file = path.join(CONF_PATH, 'roles.json')
+    conf_file = path.join(CONF_PATH, "roles.json")
     with open(conf_file) as r:
         roles = json.loads(r.read())
         global ROLE_CONTENT
         ROLE_CONTENT.update(roles)
```

### Comparing `shgpt-0.3.0/README.md` & `shgpt-0.3.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # ShellGPT
 
 [![](https://img.shields.io/pypi/v/shgpt)](https://pypi.org/project/shgpt/)
+[![](https://github.com/jiacai2050/shellgpt/actions/workflows/ci.yml/badge.svg)](https://github.com/jiacai2050/shellgpt/actions/workflows/ci.yml)
+[![](https://github.com/jiacai2050/shellgpt/actions/workflows/release.yml/badge.svg)](https://github.com/jiacai2050/shellgpt/actions/workflows/release.yml)
 
-Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!
+Chat with LLM in your terminal, be it shell generator, story teller, linux-terminal, etc.
 
 # Install
 ```
 pip install -U shgpt
 ```
 
 This will install two commands: `sg` and `shgpt`, which are identical.
@@ -49,13 +51,14 @@
 $ shgpt -r linux-terminal pwd
 /home/user
 
 $ shgpt -r javascript-console 0.1 + 0.2
 0.3
 
 ```
+
 # Requirements
 - [Ollama](https://ollama.com/), you need to download models before try shellgpt.
 
 # License
 
 [GPL-3.0](https://opensource.org/license/GPL-3.0)
```

### Comparing `shgpt-0.3.0/pyproject.toml` & `shgpt-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,39 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "shgpt"
 dynamic = ["version"]
 authors = [{name = "Jiacai Liu", email="dev@liujiacai.net"}]
-description = "Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!"
+description = "Chat with LLM in your terminal, be it shell generator, story teller, linux-terminal, etc."
 readme = "README.md"
 keywords = ["llm", "shell", "gpt"]
 license = "GPL-3.0"
 dependencies = [
   "requests",
   "pyperclip",
   "textual",
 ]
+classifiers = [
+    "Operating System :: OS Independent",
+    "Topic :: Software Development",
+    "License :: OSI Approved :: MIT License",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Developers",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
 
 [project.urls]
 Repository = "https://github.com/jiacai2050/shellgpt"
 Issues = "https://github.com/jiacai2050/shellgpt/issues"
 
 [project.scripts]
 sg = "shgpt:main"
@@ -37,24 +53,10 @@
 ]
 
 [tool.hatch.build.targets.wheel]
 include = [
   "shgpt",
 ]
 
-
-classifiers = [
-    "Operating System :: OS Independent",
-    "Topic :: Software Development",
-    "License :: OSI Approved :: MIT License",
-    "Intended Audience :: Information Technology",
-    "Intended Audience :: System Administrators",
-    "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
+# https://github.com/astral-sh/ruff?tab=readme-ov-file#configuration
+[tool.ruff.lint]
+ignore = ["F405", "F403"]
```

### Comparing `shgpt-0.3.0/PKG-INFO` & `shgpt-0.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 Metadata-Version: 2.3
 Name: shgpt
-Version: 0.3.0
-Summary: Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!
+Version: 0.3.1
+Summary: Chat with LLM in your terminal, be it shell generator, story teller, linux-terminal, etc.
 Project-URL: Repository, https://github.com/jiacai2050/shellgpt
 Project-URL: Issues, https://github.com/jiacai2050/shellgpt/issues
 Author-email: Jiacai Liu <dev@liujiacai.net>
 License-Expression: GPL-3.0
 Keywords: gpt,llm,shell
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: textual
 Description-Content-Type: text/markdown
 
 # ShellGPT
 
 [![](https://img.shields.io/pypi/v/shgpt)](https://pypi.org/project/shgpt/)
+[![](https://github.com/jiacai2050/shellgpt/actions/workflows/ci.yml/badge.svg)](https://github.com/jiacai2050/shellgpt/actions/workflows/ci.yml)
+[![](https://github.com/jiacai2050/shellgpt/actions/workflows/release.yml/badge.svg)](https://github.com/jiacai2050/shellgpt/actions/workflows/release.yml)
 
-Chat with LLM for anything you like, be it shell generator, story teller, linux-terminal, etc. All without leaving your terminal!
+Chat with LLM in your terminal, be it shell generator, story teller, linux-terminal, etc.
 
 # Install
 ```
 pip install -U shgpt
 ```
 
 This will install two commands: `sg` and `shgpt`, which are identical.
@@ -63,13 +79,14 @@
 $ shgpt -r linux-terminal pwd
 /home/user
 
 $ shgpt -r javascript-console 0.1 + 0.2
 0.3
 
 ```
+
 # Requirements
 - [Ollama](https://ollama.com/), you need to download models before try shellgpt.
 
 # License
 
 [GPL-3.0](https://opensource.org/license/GPL-3.0)
```

