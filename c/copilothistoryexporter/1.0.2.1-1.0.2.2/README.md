# Comparing `tmp/copilothistoryexporter-1.0.2.1.tar.gz` & `tmp/copilothistoryexporter-1.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.2.1.tar", last modified: Sun Jun  2 17:30:39 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.2.2.tar", last modified: Sun Jun  2 18:06:42 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.2.1.tar` & `copilothistoryexporter-1.0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:30:39.783285 copilothistoryexporter-1.0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 17:30:39.783285 copilothistoryexporter-1.0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:30:39.783285 copilothistoryexporter-1.0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:30:39.775285 copilothistoryexporter-1.0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:30:39.779286 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:30:39.779286 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/addons/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/addons/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:30:39.779286 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/vote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:30:39.779286 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/model/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/model/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/model/request.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/sample.md
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-06-02 17:30:26.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:30:39.783285 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 17:30:39.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 17:30:39.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:30:39.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 17:30:39.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 17:30:39.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 17:30:39.000000 copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:06:42.525700 copilothistoryexporter-1.0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-02 18:06:42.525700 copilothistoryexporter-1.0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:06:42.525700 copilothistoryexporter-1.0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:06:42.521700 copilothistoryexporter-1.0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:06:42.521700 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:06:42.521700 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/addons/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:06:42.525700 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:06:42.525700 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/model/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/model/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/sample.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-06-02 18:06:38.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:06:42.521700 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-02 18:06:42.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 18:06:42.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:06:42.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-02 18:06:42.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 18:06:42.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 18:06:42.000000 copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/top_level.txt
```

### Comparing `copilothistoryexporter-1.0.2.1/LICENCE` & `copilothistoryexporter-1.0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.1/README.md` & `copilothistoryexporter-1.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.1/setup.py` & `copilothistoryexporter-1.0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(
     name="copilothistoryexporter",
-    version='1.0.2.1',
+    version='1.0.2.2',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kılıç',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
     package_dir={'': 'src'},
-    packages=find_packages('src'),
+    packages=find_packages('src', include=["*"]),
     package_data={'': ['*.md']},
     install_requires=REQUIREMENTS,
     entry_points={
         'console_scripts': [
             'copilothistoryexporter=copilothistoryexporter.main:sys_main',
         ],
     },
```

### Comparing `copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/addons/binding.py` & `copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/addons/binding.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 
-from copilothistoryexporter.interceptor import chain
-from copilothistoryexporter.model.conversation import Conversation
-from copilothistoryexporter.model.request import Request
 from mitmproxy import http
 
+from src.copilothistoryexporter.interceptor import chain
+from src.copilothistoryexporter.model.conversation import Conversation
+from src.copilothistoryexporter.model.request import Request
+
 LISTEN_URL = "https://api.githubcopilot.com/chat/completions"
 LISTEN_URL_RATING = "https://copilot-telemetry.githubusercontent.com/telemetry"
 
 
 def get_message_from_response(data) -> list[Conversation]:
     user_contents = [message['content'] for message in data['messages'] if message['role'] == 'user']
     if user_contents.__len__() == 1 and data.get("intent_content", None) is None:
```

### Comparing `copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/interceptor/cache.py` & `copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/interceptor/vote.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from copilothistoryexporter import utils
-from copilothistoryexporter.interceptor.interceptor import Interceptor
-from copilothistoryexporter.model.request import Request
+from src.copilothistoryexporter import utils
+from src.copilothistoryexporter.interceptor.interceptor import Interceptor
+from src.copilothistoryexporter.model.request import Request
 
 
-class CacheInterceptor(Interceptor):
+class VoteInterceptor(Interceptor):
     def process(self, request: Request):
-        conversations = utils.get_json_files()
-        if request.conversation.prompt != "ignore":
-            conversations.append(request.conversation.to_dict())
-            print("Cache updated")
-
-        utils.write_to_json_file(conversations)
-
+        prompt = request.conversation.prompt
+        if prompt == "vote:good" or prompt == "vote:bad":
+            conversations = utils.get_json_files()
+            conversations[-1]["rating"] = "***" if prompt == "vote:good" else "*"
+            utils.write_to_json_file(conversations)
+            request.conversation.prompt = "ignore"
         return request
```

### Comparing `copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/main.py` & `copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import subprocess
 import traceback
 
 import click
-from copilothistoryexporter.utils import SharedValues
+
+from src.copilothistoryexporter.utils import SharedValues
 
 
 @click.command()
 @click.option('--port', default=9696, help='Running port')
 @click.option('--debug', default=False, help='Debug mode')
 @click.argument('project', type=click.Path(exists=True, writable=True), required=False)
 def main(port, debug, project):
@@ -17,14 +18,15 @@
     launch = "mitmdump" if not debug else "mitmweb"
     shell = f"{launch} -s {script} -p {port}"
     print(f"running on --port {port} --debug {debug} {project}")
     print("running mitm with command: ", shell)
     subprocess.run(shell, shell=True)
 
 
+
 def sys_main():
     """
     Runs the main function using the system cli arguments, and
     returns a system error code.
     :return: 0 for success, 1 for failure.
     :rtype: int
     """
```

### Comparing `copilothistoryexporter-1.0.2.1/src/copilothistoryexporter/utils.py` & `copilothistoryexporter-1.0.2.2/src/copilothistoryexporter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from copilothistoryexporter.model.conversation import Conversation
+from src.copilothistoryexporter.model.conversation import Conversation
 
 import subprocess
 
 
 class SharedValues:
     WORKSPACE = ""
```

### Comparing `copilothistoryexporter-1.0.2.1/src/copilothistoryexporter.egg-info/SOURCES.txt` & `copilothistoryexporter-1.0.2.2/src/copilothistoryexporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

