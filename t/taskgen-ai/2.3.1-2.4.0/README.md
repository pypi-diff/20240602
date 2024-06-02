# Comparing `tmp/taskgen_ai-2.3.1.tar.gz` & `tmp/taskgen_ai-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen_ai-2.3.1.tar", last modified: Fri May 24 15:49:40 2024, max compression
+gzip compressed data, was "taskgen_ai-2.4.0.tar", last modified: Sun Jun  2 06:56:10 2024, max compression
```

## Comparing `taskgen_ai-2.3.1.tar` & `taskgen_ai-2.4.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-24 15:49:40.000617 taskgen_ai-2.3.1/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.3.1/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-24 15:49:39.999879 taskgen_ai-2.3.1/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    21057 2024-05-24 15:27:57.000000 taskgen_ai-2.3.1/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      684 2024-05-24 15:27:59.000000 taskgen_ai-2.3.1/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-05-24 15:49:40.000748 taskgen_ai-2.3.1/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      230 2024-05-24 15:28:00.000000 taskgen_ai-2.3.1/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-24 15:49:39.995235 taskgen_ai-2.3.1/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      237 2024-05-17 02:04:12.000000 taskgen_ai-2.3.1/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    36778 2024-05-24 15:26:23.000000 taskgen_ai-2.3.1/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    33671 2024-05-24 15:28:06.000000 taskgen_ai-2.3.1/taskgen/base.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    19279 2024-05-24 04:30:41.000000 taskgen_ai-2.3.1/taskgen/function.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-05-24 15:49:39.999001 taskgen_ai-2.3.1/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21698 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      283 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       43 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-05-24 15:49:39.000000 taskgen_ai-2.3.1/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-06-02 06:56:10.787741 taskgen_ai-2.4.0/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-2.4.0/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    22499 2024-06-02 06:56:10.787012 taskgen_ai-2.4.0/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    21834 2024-06-02 06:22:10.000000 taskgen_ai-2.4.0/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      696 2024-06-02 05:15:49.000000 taskgen_ai-2.4.0/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-06-02 06:56:10.787968 taskgen_ai-2.4.0/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      230 2024-06-02 05:24:18.000000 taskgen_ai-2.4.0/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-06-02 06:56:10.782680 taskgen_ai-2.4.0/taskgen/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      367 2024-06-02 02:07:04.000000 taskgen_ai-2.4.0/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    64826 2024-06-02 06:41:27.000000 taskgen_ai-2.4.0/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    24881 2024-06-02 02:08:37.000000 taskgen_ai-2.4.0/taskgen/base.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    17035 2024-06-02 06:15:20.000000 taskgen_ai-2.4.0/taskgen/base_async.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    22207 2024-06-02 02:09:02.000000 taskgen_ai-2.4.0/taskgen/function.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)     9082 2024-06-02 05:17:08.000000 taskgen_ai-2.4.0/taskgen/memory.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)     2499 2024-06-02 05:36:59.000000 taskgen_ai-2.4.0/taskgen/ranker.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)     1493 2024-06-02 02:09:42.000000 taskgen_ai-2.4.0/taskgen/utils.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-06-02 06:56:10.786349 taskgen_ai-2.4.0/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    22499 2024-06-02 06:56:10.000000 taskgen_ai-2.4.0/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      358 2024-06-02 06:56:10.000000 taskgen_ai-2.4.0/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-06-02 06:56:10.000000 taskgen_ai-2.4.0/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       52 2024-06-02 06:56:10.000000 taskgen_ai-2.4.0/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-06-02 06:56:10.000000 taskgen_ai-2.4.0/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen_ai-2.3.1/LICENSE` & `taskgen_ai-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen_ai-2.3.1/PKG-INFO` & `taskgen_ai-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.3.1
+Version: 2.4.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 Requires-Dist: termcolor>=2.3.0
+Requires-Dist: requests
 
-# TaskGen v2.3.1
+# TaskGen v2.4.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
@@ -30,14 +31,16 @@
 - Single Agent with LLM Functions
 - Single Agent with External Functions
 - Meta Agent with Inner Agents as Functions
 - Shared Variables for multi-modality support
 - Retrieval Augmented Generation (RAG) over Function space
 - Memory to provide additional task-based prompts for task
 - Global Context for configuring your own prompts + add persistent variables
+- Async mode for Agent, Function and `strict_json` added
+- Community Uploading and Downloading of Agent and Functions
 
 I am quite sure that this is the best open-source agentic framework for task-based execution out there! 
 Existing frameworks like AutoGen rely too much on conversational text which is lengthy and not targeted.
 TaskGen uses StrictJSON (JSON parser with type checking and more!) as the core, and agents are efficient and are able to do Chain of Thought natively using JSON keys and descriptions as a guide.
 
 What can you do to help: 
 - Star the github so more people can use it (It's open source and free to use, even commercially!)
@@ -380,17 +383,24 @@
 - Implementing your own specific instructions to the default planner prompt
     - Implement your own memory-based RAG / global prompt instruction if you need more than what the default prompt can achieve
 <br></br>
 - Avoid Multiple Similar Subtasks in `subtasks_history`
     - If you have multiple similar subtask names, then it is likely the Agent can be confused and think it has already done the subtask
     - In this case, you can disambiguate by resetting the agent and store the persistent information in `shared_variables` and provide it to the agent using `get_global_context`
     - Has the benefit of shifting the Start State closer to End State desired by resetting the Agent's planning cycle
+    
+# Async Agents, Functions, strict_json (See Tutorial 8 and 9)
+- TaskGen now supports Async functionalities
+- We use `AsyncAgent`, `AsyncFunction` and `strict_json_async`
+    - These are the async equivalents of `Agent`, `Function` and `strict_json`
+
 
 # Known Limitations
-- To be added
+- `gpt-3.5-turbo` is not that great with mathematical functions for Agents. Use `gpt-4-turbo` or better for more consistent results
+- `gpt-3.5-turbo` is not that great with Memory (Tutorial 4). Use `gpt-4-turbo` or better for more consistent results
 
 # Contributing to the project
 
 ## Test locally
 1. Clone the repository
 2. If using a virtual environment, activate it
 3. `cd` into taskgen repository
@@ -401,11 +411,11 @@
 1. Fork the repository
 2. Create a new branch
 3. Make your changes
 4. Push your changes to your fork
 5. Submit a pull request
 
 # What are we looking out for?
-1. Integrations with functions - It would be good if we could import function definitions from elsewhere, e.g. LangChain, into the format shown here. It might even be done automatically using LLM-based conversion using StrictJSON!
+1. Contributing example Agents and Functions. Agents can now be contributed easily using `agent.contribute_agent()` and the entire Agent code with all the functions and memory will be converted to text-based code and put on the TaskGen GitHub. Do share your use cases actively so that other people can benefit :) These Agents can be downloaded by others via `agent.load_community_agent(agent_name)`
 2. Jupyter Notebooks showcasing what could be done with the framework for something useful. Let your imagination guide you, we look forward to see what you create
 3. Other Known Limitations - Do test the framework out extensively and note its failure cases. We will see if we can address them, if not we will put them in Known Limitations.
 4. (For the prompt engineer). If you could find a better way to make the prompts work, let us know directly - we do need to test this out across all Tutorial Jupyter Notebooks to make sure that it really works with existing datasets. Also, if you are using other LLMs beside OpenAI, and find the prompts do not work as well - try to rejig your own prompts and let us know as well!
```

### Comparing `taskgen_ai-2.3.1/README.md` & `taskgen_ai-2.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TaskGen v2.3.1
+# TaskGen v2.4.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
@@ -13,14 +13,16 @@
 - Single Agent with LLM Functions
 - Single Agent with External Functions
 - Meta Agent with Inner Agents as Functions
 - Shared Variables for multi-modality support
 - Retrieval Augmented Generation (RAG) over Function space
 - Memory to provide additional task-based prompts for task
 - Global Context for configuring your own prompts + add persistent variables
+- Async mode for Agent, Function and `strict_json` added
+- Community Uploading and Downloading of Agent and Functions
 
 I am quite sure that this is the best open-source agentic framework for task-based execution out there! 
 Existing frameworks like AutoGen rely too much on conversational text which is lengthy and not targeted.
 TaskGen uses StrictJSON (JSON parser with type checking and more!) as the core, and agents are efficient and are able to do Chain of Thought natively using JSON keys and descriptions as a guide.
 
 What can you do to help: 
 - Star the github so more people can use it (It's open source and free to use, even commercially!)
@@ -363,17 +365,24 @@
 - Implementing your own specific instructions to the default planner prompt
     - Implement your own memory-based RAG / global prompt instruction if you need more than what the default prompt can achieve
 <br></br>
 - Avoid Multiple Similar Subtasks in `subtasks_history`
     - If you have multiple similar subtask names, then it is likely the Agent can be confused and think it has already done the subtask
     - In this case, you can disambiguate by resetting the agent and store the persistent information in `shared_variables` and provide it to the agent using `get_global_context`
     - Has the benefit of shifting the Start State closer to End State desired by resetting the Agent's planning cycle
+    
+# Async Agents, Functions, strict_json (See Tutorial 8 and 9)
+- TaskGen now supports Async functionalities
+- We use `AsyncAgent`, `AsyncFunction` and `strict_json_async`
+    - These are the async equivalents of `Agent`, `Function` and `strict_json`
+
 
 # Known Limitations
-- To be added
+- `gpt-3.5-turbo` is not that great with mathematical functions for Agents. Use `gpt-4-turbo` or better for more consistent results
+- `gpt-3.5-turbo` is not that great with Memory (Tutorial 4). Use `gpt-4-turbo` or better for more consistent results
 
 # Contributing to the project
 
 ## Test locally
 1. Clone the repository
 2. If using a virtual environment, activate it
 3. `cd` into taskgen repository
@@ -384,11 +393,11 @@
 1. Fork the repository
 2. Create a new branch
 3. Make your changes
 4. Push your changes to your fork
 5. Submit a pull request
 
 # What are we looking out for?
-1. Integrations with functions - It would be good if we could import function definitions from elsewhere, e.g. LangChain, into the format shown here. It might even be done automatically using LLM-based conversion using StrictJSON!
+1. Contributing example Agents and Functions. Agents can now be contributed easily using `agent.contribute_agent()` and the entire Agent code with all the functions and memory will be converted to text-based code and put on the TaskGen GitHub. Do share your use cases actively so that other people can benefit :) These Agents can be downloaded by others via `agent.load_community_agent(agent_name)`
 2. Jupyter Notebooks showcasing what could be done with the framework for something useful. Let your imagination guide you, we look forward to see what you create
 3. Other Known Limitations - Do test the framework out extensively and note its failure cases. We will see if we can address them, if not we will put them in Known Limitations.
 4. (For the prompt engineer). If you could find a better way to make the prompts work, let us know directly - we do need to test this out across all Tutorial Jupyter Notebooks to make sure that it really works with existing datasets. Also, if you are using other LLMs beside OpenAI, and find the prompts do not work as well - try to rejig your own prompts and let us know as well!
```

### Comparing `taskgen_ai-2.3.1/pyproject.toml` & `taskgen_ai-2.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskgen-ai"
-version = "2.3.1"
+version = "2.4.0"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Task-based agentic framework building on StrictJSON outputs by LLM agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["openai>=1.3.6", "dill>=0.3.7", "termcolor>=2.3.0"]
+dependencies = ["openai>=1.3.6", "dill>=0.3.7", "termcolor>=2.3.0", "requests"]
 
 [project.urls]
 Homepage = "https://github.com/simbianai/taskgen"
 Issues = "https://github.com/simbianai/taskgen/issues"
```

### Comparing `taskgen_ai-2.3.1/taskgen/base.py` & `taskgen_ai-2.4.0/taskgen/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-import os
-import openai
 import json
 import re
 import ast
-import copy
-import inspect
-from typing import get_type_hints
+from typing import Tuple
 from openai import OpenAI
 
+
 ### Helper Functions ###
 
 def convert_to_list(field: str, **kwargs) -> list:
     '''Converts the string field into a list using the LLM (with **kwargs) to list out elements line by line'''
     
     system_msg = '''Output each element of the list in a new line starting with (%item) and ending with \n, e.g. ['hello', 'world'] -> (%item) hello\n(%item) world\nStart your response with (%item) and do not provide explanation'''
     user_msg = str(field)
     res = chat(system_msg, user_msg, **kwargs)
 
     # Extract out list items
     field = re.findall(r'\(%item\)\s*(.*?)\n*(?=\(%item\)|$)', res, flags=re.DOTALL)
     return field
 
+
 def convert_to_dict(field: str, keys: dict, delimiter: str) -> dict:
     '''Converts the string field into a dictionary with keys by splitting on '{delimiter}{key}{delimiter}' '''
     output_d = {}
     for key in keys:
         # if output field missing, raise an error
         if f"'{delimiter}{key}{delimiter}':" not in field and f'"{delimiter}{key}{delimiter}":' not in field: 
             # try to fix it if possible
@@ -49,51 +47,143 @@
 
     # create a dictionary
     for i in range(0, len(curated_matches), 2):
         output_d[curated_matches[i]] = curated_matches[i+1]
         
     return output_d
 
-def llm_check(field, llm_check_msg: str, **kwargs) -> (bool, str):
+def llm_check(field, llm_check_msg: str, **kwargs) -> Tuple[bool, str]:
     ''' Uses the LLM to check if the field adheres to the llm_check_msg.
     Outputs whether requirement is met (True or False) and the action needed'''
     system_msg = f'''Check whether output field meets this requirement: {llm_check_msg}
 Output in the following format:
 ```
 # Thoughts: <Thoughts about whether output field meets requirement>
 # Requirement Met: <Yes or No>
 # Action Needed: <If Requirement Met is No, state in one sentence how to meet requirement. Otherwise, output NA>"
 ```
 Update text enclosed in <>. Be concise.
 '''
     user_msg = str(field)
     res = chat(system_msg, user_msg, **kwargs)
-    
+    requirement_met, action_needed = parse_response_llm_check(res)
+    return requirement_met, action_needed
+
+
+def parse_response_llm_check(res: str) -> Tuple[bool, str]:
     pattern = r"# Thoughts: (.+)\n# Requirement Met: (.+)\n# Action Needed: (.+)"
     matches = re.findall(pattern, res)
 
     if matches:
-        thoughts, requirement_met, action_needed = matches[0]
-        if 'yes' in requirement_met.lower():
-            requirement_met = True
-        else:
-            requirement_met = False
-        # print("Thoughts:", thoughts)
-        print("Requirement Met:", requirement_met)
-        if not requirement_met:
-            print("Action Needed:", action_needed)
-        print('\n')
+        _, requirement_met, action_needed = matches[0]
+        requirement_met = 'yes' in requirement_met.lower()
+        action_needed = action_needed.strip() if not requirement_met else ''
     else:
-        # if regex failed to parse, we just check for yes / no. And append whole string as action needed
-        if 'yes' in res.lower():
-            thoughts, requirement_met, action_needed = '', True, ''
+        requirement_met = 'yes' in res.lower()
+        action_needed = res.strip() if not requirement_met else ''
+
+    return requirement_met, action_needed
+
+
+
+
+def type_check_and_convert(field, key, data_type, **kwargs):
+    if data_type.lower() == 'str':
+        try:
+            # convert to string and remove escape characters from indents and quotations
+            field = str(field)
+        except Exception as e:
+            pass
+        if not isinstance(field, str):
+            raise Exception(f'''Output field of "{key}" not of data type {data_type}. If not possible to match, output '' ''')
+    # special case of str is code, where we remove double backslashes
+    if data_type.lower() == 'code':
+        try:
+            field = str(field)
+        except Exception as e:
+            pass
+        if not isinstance(field, str):
+            raise Exception(f'''Output field of "{key}" not of data type {data_type}. If not possible to match, output '' ''')
+        # do decoding for double backslashes
+        field = bytes(field, "utf-8").decode("unicode_escape")
+        # replace aprostrophes
+        field = field.replace("â\x80\x99", "'")
+        # remove the python and ```, whitespace at the front and back of code if any
+        field = re.sub(r"^(\s|`)*(?i:python)?\s*", "", field)
+        # Removes whitespace & ` from end
+        field = re.sub(r"(\s|`)*$", "", field)
+            
+    # check for int
+    if data_type.lower() == 'int':
+        try:
+            field = int(field)
+        except Exception as e:
+            pass
+        if not isinstance(field, int):
+            raise Exception(f'Output field of "{key}" not of data type {data_type}. If not possible to match, output 0')
+    
+    # check for float
+    if data_type.lower() == 'float':
+        try:
+            field = float(field)
+        except Exception as e:
+            pass
+        if not isinstance(field, float):
+            raise Exception(f'Output field of "{key}" not of data type {data_type}. If not possible to match, output 0.0')
+            
+    # check for bool
+    if data_type.lower() == 'bool':
+        field = str(field)
+        if 'true' == field[:4].lower():
+            field = True
+        elif 'false' == field[:5].lower():
+            field = False
         else:
-            thoughts, requirement_met, action_needed = '', False, res
+            raise Exception(f'Output field of "{key}" not of data type {data_type}. If not possible to match, output True')
+
+    # check for dict
+    if data_type[:4].lower() == 'dict':
+        if not isinstance(field, dict):
+            # first try to see if we can do ast.literal_eval with { and }
+            try:
+                field = str(field)
+                startindex = field.find('{')
+                endindex = field.rfind('}')
+                field = field[startindex: endindex+1]
+                field = ast.literal_eval(field)
+                assert(isinstance(field, dict))
+            except Exception as e:
+                raise Exception(f"Output field of {key} not of data type dict. If not possible to match, rephrase output field into dictionary with attribute names as key and attribute description as value")
             
-    return requirement_met, action_needed
+        # if we define more things in dict, evaluate those
+        if len(data_type) > 4:
+            try:
+                attribute_checks = ast.literal_eval(data_type[4:])
+                assert(isinstance(attribute_checks, list) == True)
+            except Exception as e:
+                raise Exception(f'Dictionary keys {data_type[4:]} of output field of "{key}" are not properly defined. Ensure that it is a proper list')
+                
+            # if data_type is a valid list, check if elements of list are present in dictionary
+            if isinstance(attribute_checks, list):
+                for item in attribute_checks:
+                    if item not in field.keys():
+                        raise Exception(f'Output field of "{key}" of type dict does not contain the key "{item}". The dict should contain keys {attribute_checks}')
+            
+    # check for enum
+    if data_type[:4].lower() == 'enum':
+        try:
+            values = ast.literal_eval(data_type[4:])  
+            assert(isinstance(values, list) == True)
+        except Exception as e:
+            raise Exception(f'Enumeration values {data_type[4:]} of output field of "{key}" are not properly defined. Ensure that it is a proper list')
+        if field not in values:
+            raise Exception(f'Output field of "{key}" ({field}) not one of {values}. If not possible to match, output {values[0]}')
+    return field
+
+
 
 def check_datatype(field, key: dict, data_type: str, **kwargs):
     ''' Ensures that output field of the key of JSON dictionary is of data_type 
     Currently supports int, float, str, code, enum, lists, nested lists, dict, dict with keys
     Takes in **kwargs for the LLM model
     Returns corrected output field that matches the datatype'''
     data_type = data_type.strip()
@@ -142,107 +232,23 @@
         internal_data_type = match.group(1)  # Extract the content inside the brackets
         # do processing for internal elements
         for num in range(len(field)):
             field[num] = check_datatype(field[num], 'array element of '+key, internal_data_type, **kwargs)
             
     # if it is not nested, check individually
     else:
-        # check for string
-        if data_type.lower() == 'str':
-            try:
-                # convert to string and remove escape characters from indents and quotations
-                field = str(field)
-            except Exception as e:
-                pass
-            if not isinstance(field, str):
-                raise Exception(f'''Output field of "{key}" not of data type {data_type}. If not possible to match, output '' ''')
-        # special case of str is code, where we remove double backslashes
-        if data_type.lower() == 'code':
-            try:
-                field = str(field)
-            except Exception as e:
-                pass
-            if not isinstance(field, str):
-                raise Exception(f'''Output field of "{key}" not of data type {data_type}. If not possible to match, output '' ''')
-            # do decoding for double backslashes
-            field = bytes(field, "utf-8").decode("unicode_escape")
-            # replace aprostrophes
-            field = field.replace("â\x80\x99", "'")
-            # remove the python and ```, whitespace at the front and back of code if any
-            field = re.sub(r"^(\s|`)*(?i:python)?\s*", "", field)
-            # Removes whitespace & ` from end
-            field = re.sub(r"(\s|`)*$", "", field)
-                
-        # check for int
-        if data_type.lower() == 'int':
-            try:
-                field = int(field)
-            except Exception as e:
-                pass
-            if not isinstance(field, int):
-                raise Exception(f'Output field of "{key}" not of data type {data_type}. If not possible to match, output 0')
-        
-        # check for float
-        if data_type.lower() == 'float':
-            try:
-                field = float(field)
-            except Exception as e:
-                pass
-            if not isinstance(field, float):
-                raise Exception(f'Output field of "{key}" not of data type {data_type}. If not possible to match, output 0.0')
-                
-        # check for bool
-        if data_type.lower() == 'bool':
-            field = str(field)
-            if 'true' == field[:4].lower():
-                field = True
-            elif 'false' == field[:5].lower():
-                field = False
-            else:
-                raise Exception(f'Output field of "{key}" not of data type {data_type}. If not possible to match, output True')
-
-        # check for dict
-        if data_type[:4].lower() == 'dict':
-            if not isinstance(field, dict):
-                # first try to see if we can do ast.literal_eval with { and }
-                try:
-                    field = str(field)
-                    startindex = field.find('{')
-                    endindex = field.rfind('}')
-                    field = field[startindex: endindex+1]
-                    field = ast.literal_eval(field)
-                    assert(isinstance(field, dict))
-                except Exception as e:
-                    raise Exception(f"Output field of {key} not of data type dict. If not possible to match, rephrase output field into dictionary with attribute names as key and attribute description as value")
-                
-            # if we define more things in dict, evaluate those
-            if len(data_type) > 4:
-                try:
-                    attribute_checks = ast.literal_eval(data_type[4:])
-                    assert(isinstance(attribute_checks, list) == True)
-                except Exception as e:
-                    raise Exception(f'Dictionary keys {data_type[4:]} of output field of "{key}" are not properly defined. Ensure that it is a proper list')
-                    
-                # if data_type is a valid list, check if elements of list are present in dictionary
-                if isinstance(attribute_checks, list):
-                    for item in attribute_checks:
-                        if item not in field.keys():
-                            raise Exception(f'Output field of "{key}" of type dict does not contain the key "{item}". The dict should contain keys {attribute_checks}')
-                
-        # check for enum
-        if data_type[:4].lower() == 'enum':
-            try:
-                values = ast.literal_eval(data_type[4:])  
-                assert(isinstance(values, list) == True)
-            except Exception as e:
-                raise Exception(f'Enumeration values {data_type[4:]} of output field of "{key}" are not properly defined. Ensure that it is a proper list')
-            if field not in values:
-                raise Exception(f'Output field of "{key}" ({field}) not one of {values}. If not possible to match, output {values[0]}')
+        field = type_check_and_convert(field, key, data_type, **kwargs)
     return field
 
+
+
+
+
+
+
 def check_key(field: str, output_format, new_output_format, delimiter: str, delimiter_num: int, **kwargs):
     ''' Check whether each key in dict, or elements in list of new_output_format is present in field, and whether they meet the right data type requirements, then convert field to the right data type
     If needed, calls LLM model with parameters **kwargs to correct the output format for improperly formatted list
     output_format is user-given output format at each level, new_output_format is with delimiters in keys, and angle brackets surrounding values
     If output_format is a string, decode escape characters, so that code can run
     Returns field that is converted to a dictionary if able to. Otherwise, raises Exception errors for missing keys or wrong output format'''
     
@@ -292,14 +298,18 @@
             pass
         return remove_unicode_escape(field)
     
     # otherwise just return the value
     else:
         return field
     
+    
+    
+
+    
 def remove_unicode_escape(my_datatype):
     ''' Removes the unicode escape character from the ending string in my_datatype (can be nested) '''
     if isinstance(my_datatype, dict):
         output_d = {}
         # wrap keys with delimiters
         for key, value in my_datatype.items():
             output_d[key] = remove_unicode_escape(value)
@@ -385,66 +395,14 @@
         print('System prompt:', system_prompt)
         print('\nUser prompt:', user_prompt)
         print('\nGPT response:', res)
             
     return res
 
 
-async def chat_async(system_prompt: str, user_prompt: str, model: str = 'gpt-3.5-turbo', temperature: float = 0, verbose: bool = False, host: str = 'openai', llm_async = None, **kwargs):
-    '''Performs a chat with the host's LLM model with system prompt, user prompt, model, verbose and kwargs
-    Returns the output string res
-    - system_prompt: String. Write in whatever you want the LLM to become. e.g. "You are a \<purpose in life\>"
-    - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
-    - model: String. The LLM model to use for json generation
-    - verbose: Boolean (default: False). Whether or not to print out the system prompt, user prompt, GPT response
-    - host: String. The provider of the LLM
-    - llm: User-made llm function.
-        - Inputs:
-            - system_prompt: String. Write in whatever you want the LLM to become. e.g. "You are a \<purpose in life\>"
-            - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
-        - Output:
-            - res: String. The response of the LLM call
-    - **kwargs: Dict. Additional arguments for LLM chat
-    '''
-    if llm_async is not None:
-        ''' If you specified your own LLM, then we just feed in the system and user prompt 
-        LLM function should take in system prompt (str) and user prompt (str), and output a response (str) '''
-        res = await llm_async(system_prompt = system_prompt, user_prompt = user_prompt)
-    
-    ## This part here is for llms that are OpenAI based
-    elif host == 'openai':
-        # additional checks for openai json mode
-        if 'response_format' in kwargs and kwargs['response_format'] == {"type": "json_object"}:
-            # if model fails, default to gpt-3.5-turbo-1106
-            try:
-                assert(model in ['gpt-4-1106-preview', 'gpt-3.5-turbo-1106'])
-            except Exception as e:
-                model = 'gpt-3.5-turbo-1106'
-                
-        client = OpenAI()
-        response = client.chat.completions.create(
-            model=model,
-            temperature = temperature,
-            messages=[
-                {"role": "system", "content": system_prompt},
-                {"role": "user", "content": user_prompt}
-            ],
-            **kwargs
-        )
-        res = response.choices[0].message.content
-
-    if verbose:
-        print('System prompt:', system_prompt)
-        print('\nUser prompt:', user_prompt)
-        print('\nGPT response:', res)
-            
-    return res
-
-
-
 ### Main Functions ###
 def strict_json(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = None, check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
     ''' Ensures that OpenAI will always adhere to the desired output JSON format defined in output_format. 
     Uses rule-based iterative feedback to ask GPT to self-correct.
     Keeps trying up to num_tries it it does not. Returns empty JSON if unable to after num_tries iterations.
     
     Inputs (compulsory):
@@ -514,122 +472,14 @@
             
             # extract only the chunk including the opening and closing braces
             startindex = res.find('{')
             endindex = res.rfind('}')
             res = res[startindex: endindex+1]
 
             # try-catch block to ensure output format is adhered to
-            try:
-                # check that res is a json string
-                if res[0] != '{' or res[-1] != '}':
-                    raise Exception('Ensure output must be a json string beginning with { and ending with }')
-                
-                # do checks for keys and output format, remove escape characters so code can be run
-                end_dict = check_key(res, output_format, new_output_format, delimiter, delimiter_num = 1, **kwargs)
-                
-                # run user defined custom checks now
-                for key in end_dict:
-                    if key in custom_checks:
-                        for check in custom_checks[key]:
-                            requirement, requirement_met, action_needed = check(end_dict[key], check_data)
-                            print(f'Running check for "{requirement}" on output field of "{key}"')
-                            if not requirement_met:
-                                print(f'Requirement not met. Action needed: "{action_needed}"\n\n')
-                                raise Exception(f'Output field of "{key}" does not meet requirement "{requirement}". Action needed: "{action_needed}"')
-                            else:
-                                print('Requirement met\n\n')
-                if return_as_json:
-                    return json.dumps(end_dict, ensure_ascii=False)
-                else:
-                    return end_dict
-
-            except Exception as e:
-                error_msg = f"\n\nPrevious json: {res}\njson error: {str(e)}\nFix the error."                
-                print("An exception occurred:", str(e))
-                print("Current invalid json format:", res)
-
-        return {}
-    
-    
-async def strict_json_async(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = None, check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
-    ''' Ensures that OpenAI will always adhere to the desired output JSON format defined in output_format. 
-    Uses rule-based iterative feedback to ask GPT to self-correct.
-    Keeps trying up to num_tries it it does not. Returns empty JSON if unable to after num_tries iterations.
-    
-    Inputs (compulsory):
-    - system_prompt: String. Write in whatever you want GPT to become. e.g. "You are a \<purpose in life\>"
-    - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
-    - output_format: Dict. JSON format with the key as the output key, and the value as the output description
-    
-    Inputs (optional):
-    - return_as_json: Bool. Default: False. Whether to return the output as a json. If False, returns as Python dict. If True, returns as json string
-    - custom_checks: Dict. Key is output key, value is function which does checking of content for output field
-    - check_data: Any data type. The additional data for custom_checks to use if required
-    - delimiter: String (Default: '###'). This is the delimiter to surround the keys. With delimiter ###, key becomes ###key###
-    - num_tries: Integer (default: 3). The number of tries to iteratively prompt GPT to generate correct json format
-    - openai_json_mode: Boolean (default: False). Whether or not to use OpenAI JSON Mode
-    - **kwargs: Dict. Additional arguments for LLM chat
-    
-    Output:
-    - res: Dict. The JSON output of the model. Returns {} if JSON parsing failed.
-    '''
-    # default initialise custom_checks to {}
-    if custom_checks is None:
-        custom_checks = {}
-        
-    # If OpenAI JSON mode is selected, then just let OpenAI do the processing
-    if openai_json_mode:
-        # add in code to warn user if type is defined for external function
-        type_check = False
-        for value in output_format.values():
-            if 'type:' in str(value):
-                type_check = True
-        if type_check:
-            print('Note: Type checking (type:) not done for OpenAI JSON Mode')
-        
-        output_format_prompt = "\nOutput in the following json string format: " + str(output_format) + "\nBe concise."
-            
-        my_system_prompt = str(system_prompt) + output_format_prompt
-        my_user_prompt = str(user_prompt) 
-            
-        res = await chat_async(my_system_prompt, my_user_prompt, response_format = {"type": "json_object"}, **kwargs)
-        
-        if return_as_json:
-            return res
-        else:
-            try:
-                loaded_json = json.loads(res)
-            except Exception as e:
-                loaded_json = {}
-            return loaded_json
-        
-    # Otherwise, implement JSON parsing using Strict JSON
-    else:
-        # start off with no error message
-        error_msg = ''
-
-        # wrap the values with angle brackets and wrap keys with delimiter to encourage LLM to modify it
-        new_output_format = wrap_with_angle_brackets(output_format, delimiter, 1)
-        
-        output_format_prompt = f'''\nOutput in the following json string format: {new_output_format}
-Update text enclosed in <>. Output only a valid json string beginning with {{ and ending with }}'''
-
-        for i in range(num_tries):
-            my_system_prompt = str(system_prompt) + output_format_prompt + error_msg
-            my_user_prompt = str(user_prompt) 
-
-            # Use OpenAI to get a response
-            res = await chat_async(my_system_prompt, my_user_prompt, **kwargs)
-            
-            # extract only the chunk including the opening and closing braces
-            startindex = res.find('{')
-            endindex = res.rfind('}')
-            res = res[startindex: endindex+1]
-
-            # try-catch block to ensure output format is adhered to
             try:
                 # check that res is a json string
                 if res[0] != '{' or res[-1] != '}':
                     raise Exception('Ensure output must be a json string beginning with { and ending with }')
                 
                 # do checks for keys and output format, remove escape characters so code can be run
                 end_dict = check_key(res, output_format, new_output_format, delimiter, delimiter_num = 1, **kwargs)
```

### Comparing `taskgen_ai-2.3.1/taskgen/function.py` & `taskgen_ai-2.4.0/taskgen/function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import os
-import openai
-import json
 import re
-import ast
-import copy
 import inspect
 from typing import get_type_hints
-from openai import OpenAI
-from .base import *
+from taskgen import strict_json
+from taskgen.base_async import strict_json_async
+
+from taskgen.utils import ensure_awaitable, get_source_code_for_func
 
 ### Helper Functions ###
 
 def get_clean_typename(typ) -> str:
     """Returns a clean, readable name for a type, including handling generics."""
     if hasattr(typ, '__origin__'):  # Check for generic types
         if typ.__origin__ is not None:  # Generic types, e.g., List, Dict
@@ -24,15 +21,15 @@
         else:  # Non-generic but special types, e.g., typing.List without parameters
             return typ._name if hasattr(typ, '_name') else str(typ)
     elif hasattr(typ, '__name__'):
         return typ.__name__  # Simple types, e.g., int, str
     else:
         return str(typ)  # Fallback, should rarely be used
 
-def get_fn_description(my_function) -> (str, list):
+def get_fn_description(my_function):
     ''' Returns the modified docstring of my_function, that takes into account input variable names and types in angle brackets
     Also returns the list of input parameters to the function in sequence
     e.g.: Adds numbers x and y -> Adds numbers <x: int> and <y: int>
     Input variables that are optional (already assigned a default value) need not be in the docstring
     args and kwargs variables are not parsed '''
      
     if not inspect.isfunction(my_function):
@@ -107,24 +104,23 @@
         else:
             output_format["output_1"] = get_clean_typename(return_type)
 
     return output_format
 
 ### Main Class ###
 
-class Function:
+class BaseFunction:
     def __init__(self,
                  fn_description: str = '', 
                  output_format: dict = None,
                  examples = None,
                  external_fn = None,
                  is_compulsory = False,
                  fn_name = None,
                  llm = None,
-                 llm_async = None,
                  **kwargs):
         ''' 
         Creates an LLM-based function or wraps an external function using fn_description and outputs JSON based on output_format. 
         (Optional) Can define the function based on examples (list of Dict containing input and output variables for each example)
         (Optional) If you would like greater specificity in your function's input, you can describe the variable after the : in the input variable name, e.g. `<var1: an integer from 10 to 30`. Here, `var1` is the input variable and `an integer from 10 to 30` is the description.
         
         Inputs (primary):
@@ -179,15 +175,14 @@
             self.output_format = output_format
             
         self.examples = examples
         self.external_fn = external_fn
         self.is_compulsory = is_compulsory
         self.fn_name = fn_name
         self.llm = llm
-        self.llm_async = llm_async
         self.kwargs = kwargs
         
         self.variable_names = []
         self.shared_variable_names = []
         # use regex to extract variables from function description
         matches = re.findall(r'<(.*?)>', self.fn_description)
             
@@ -202,73 +197,132 @@
                     self.shared_variable_names.append(first_half)
                     # replace the original variable without the <> so as not to confuse the LLM
                     self.fn_description = self.fn_description.replace(f'<{match}>', first_half)
                     
         # make it such that we follow the same order for variable names as per the external function only if there are external function params
         if self.external_param_list != []:
             self.variable_names = [x for x in self.external_param_list if x in self.variable_names]
+             
+
+        # Append examples to description
+        if self.examples is not None:
+            self.fn_description += '\nExamples:\n' + str(examples) 
+            
+    def __str__(self):
+        ''' Prints out the function's parameters '''
+        return f'Description: {self.fn_description}\nInput: {self.variable_names}\nOutput: {self.output_format}\n'
+    
+    def get_python_representation(self):
+        """Returns a Python representation of the Function object, including the external function code if available."""
+        external_fn_code = None
+        external_fn_ref = None
+
+        if self.external_fn:
+            if inspect.isfunction(self.external_fn) and self.external_fn.__name__ == "<lambda>":
+                external_fn_ref = get_source_code_for_func(self.external_fn)
+            else:
+                external_fn_ref = self.external_fn.__name__
+                external_fn_code = get_source_code_for_func(self.external_fn)
+
+        fn_initialization = f"""Function(
+            fn_name="{self.fn_name}",
+            fn_description='''{self.fn_description}''',
+            output_format={self.output_format},
+            examples={self.examples},
+            external_fn={external_fn_ref},
+            is_compulsory={self.is_compulsory})
+        """
+        return (fn_initialization, external_fn_code)
+    
+    
+    def _prepare_function_kwargs(self, *args, **kwargs):
+         # get the shared_variables if there are any
+        shared_variables = kwargs.get('shared_variables', {})
+        # remove the mention of shared_variables in kwargs
+        if 'shared_variables' in kwargs:
+            del kwargs['shared_variables']
+        # extract out only variables listed in variable_list from kwargs
+        function_kwargs = {key: value for key, value in kwargs.items() if key in self.variable_names}
+        # additionally, if function references something in shared_variables, add that in
+        for variable in self.shared_variable_names:
+            if variable in shared_variables:
+                function_kwargs[variable] = shared_variables[variable]
+        # Do the auto-naming of variables as var1, var2, or as variable names defined in variable_names
+        for num, arg in enumerate(args):
+            if len(self.variable_names) > num:
+                function_kwargs[self.variable_names[num]] = arg
+            else:
+                function_kwargs[f'var{num+1}'] = arg
                 
-        # generate function name if not defined
+        return function_kwargs, shared_variables
+
+    def _prepare_strict_json_kwargs(self, **kwargs):
+        return {key: value for key, value in kwargs.items() if key not in self.variable_names}
+
+    def _update_shared_variables(self, results, shared_variables):
+        keys_to_delete = []
+        for key in results:
+            if key.startswith('s_'):
+                shared_variables[key] = results[key]
+                keys_to_delete.append(key)
+
+        for key in keys_to_delete:
+            del results[key]
+
+    def _generate_function_name(self):
+        if self.fn_name is None:
+            if self.external_fn is not None and hasattr(self.external_fn, '__name__') and self.external_fn.__name__ != '<lambda>':
+                self.fn_name = self.external_fn.__name__
+            else:
+                self.fn_name = 'generated_function_name'  # Replace with actual function name generation logic.
+            self.__name__ = self.fn_name
+    
+    
+            
+            
+class Function(BaseFunction):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         if self.fn_name is None:
             # if external function has a name, use it
             if self.external_fn is not None and hasattr(self.external_fn, '__name__') and self.external_fn.__name__ != '<lambda>':
                 self.fn_name = self.external_fn.__name__
             # otherwise, generate name out
             else:
                 res = strict_json(system_prompt = "Output a function name to summarise the usage of this function.",
                                   user_prompt = str(self.fn_description),
                                   output_format = {"Thoughts": "What function does", "Name": "Function name with _ separating words that summarises what function does"},
                                  llm = self.llm,
                                  **self.kwargs)
                 self.fn_name = res['Name']
-                
-        # change instance's name to function's name
+         # change instance's name to function's name
         self.__name__ = self.fn_name
-
-        # Append examples to description
-        if self.examples is not None:
-            self.fn_description += '\nExamples:\n' + str(examples)
-      
-    def __str__(self):
-        ''' Prints out the function's parameters '''
-        return f'Description: {self.fn_description}\nInput: {self.variable_names}\nOutput: {self.output_format}\n'
         
+    
     def __call__(self, *args, **kwargs):
         ''' Describes the function, and inputs the relevant parameters as either unnamed variables (args) or named variables (kwargs)
         
         Inputs:
         - shared_varables: Dict. Default: empty dict. The variables which will be shared between functions. Only passed in if required by function 
         - *args: Tuple. Unnamed input variables of the function. Will be processed to var1, var2 and so on based on order in the tuple
         - **kwargs: Dict. Named input variables of the function. Can also be variables to pass into strict_json
         
         Output:
         - res: Dict. JSON containing the output variables'''
         
         # get the shared_variables if there are any
-        shared_variables = kwargs.get('shared_variables', {})
-        # remove the mention of shared_variables in kwargs
-        if 'shared_variables' in kwargs:
-            del kwargs['shared_variables']
         
-        # extract out only variables listed in variable_list from kwargs
-        function_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key in self.variable_names}
-        # additionally, if function references something in shared_variables, add that in
-        for variable in self.shared_variable_names:
-            if variable in shared_variables:
-                function_kwargs[variable] = shared_variables[variable]
         
+        function_kwargs, shared_variables = self._prepare_function_kwargs(*args, **kwargs)
+
         # extract out only variables not listed in variable list
-        strict_json_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key not in self.variable_names}
-        
-        # Do the auto-naming of variables as var1, var2, or as variable names defined in variable_names
-        for num, arg in enumerate(args):
-            if len(self.variable_names) > num:
-                function_kwargs[self.variable_names[num]] = arg
-            else:
-                function_kwargs['var'+str(num+1)] = arg
+        strict_json_kwargs = {
+            my_key: kwargs[my_key] for my_key in kwargs 
+            if my_key not in self.variable_names and my_key != 'shared_variables'
+        }
                 
         # If strict_json function, do the function. 
         if self.external_fn is None:
             res = strict_json(system_prompt = self.fn_description,
                             user_prompt = function_kwargs,
                             output_format = self.output_format,
                             llm = self.llm,
@@ -294,99 +348,118 @@
                 for i in range(len(fn_output)):
                     if len(output_keys) > i:
                         res[output_keys[i]] = fn_output[i]
                     else:
                         res[f'output_{i+1}'] = fn_output[i]
         
         # check if any of the output variables have a s_, which means we update the shared_variables and not output it
-        keys = list(res.keys())
-        for each in keys:
-            if each[:2] == 's_':
-                shared_variables[each] = res[each]
-                del res[each]
+        self._update_shared_variables(res, shared_variables)
                 
         if res == {}:
             res = {'Status': 'Completed'}
 
         return res
-    
-    async def async_call(self, *args, **kwargs):
+        
+        
+            
+class AsyncFunction(BaseFunction):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        ensure_awaitable(self.llm, 'llm')
+        self.__name__ = self.fn_name
+        
+    async def async_init(self): 
+        if self.fn_name is None:
+            # if external function has a name, use it
+            if self.external_fn is not None and hasattr(self.external_fn, '__name__') and self.external_fn.__name__ != '<lambda>':
+                self.fn_name = self.external_fn.__name__
+            # otherwise, generate name out
+            else:
+                res = await strict_json_async(system_prompt = "Output a function name to summarise the usage of this function.",
+                                  user_prompt = str(self.fn_description),
+                                  output_format = {"Thoughts": "What function does", "Name": "Function name with _ separating words that summarises what function does"},
+                                 llm = self.llm,
+                                 **self.kwargs)
+                self.fn_name = res['Name']
+        
+        # change instance's name to function's name
+        self.__name__ = self.fn_name
+        
+        
+        
+      
+        
+    async def __call__(self, *args, **kwargs):
         ''' Describes the function, and inputs the relevant parameters as either unnamed variables (args) or named variables (kwargs)
         
         Inputs:
         - shared_varables: Dict. Default: empty dict. The variables which will be shared between functions. Only passed in if required by function 
         - *args: Tuple. Unnamed input variables of the function. Will be processed to var1, var2 and so on based on order in the tuple
         - **kwargs: Dict. Named input variables of the function. Can also be variables to pass into strict_json
         
         Output:
         - res: Dict. JSON containing the output variables'''
         
         # get the shared_variables if there are any
-        shared_variables = kwargs.get('shared_variables', {})
-        # remove the mention of shared_variables in kwargs
-        if 'shared_variables' in kwargs:
-            del kwargs['shared_variables']
-        
-        # extract out only variables listed in variable_list from kwargs
-        function_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key in self.variable_names}
-        # additionally, if function references something in shared_variables, add that in
-        for variable in self.shared_variable_names:
-            if variable in shared_variables:
-                function_kwargs[variable] = shared_variables[variable]
+      
+        if self.fn_name is None:
+            await self.async_init()
         
+        function_kwargs, shared_variables = self._prepare_function_kwargs(*args, **kwargs)
+
         # extract out only variables not listed in variable list
-        strict_json_kwargs = {my_key: kwargs[my_key] for my_key in kwargs if my_key not in self.variable_names}
-        
-        # Do the auto-naming of variables as var1, var2, or as variable names defined in variable_names
-        for num, arg in enumerate(args):
-            if len(self.variable_names) > num:
-                function_kwargs[self.variable_names[num]] = arg
-            else:
-                function_kwargs['var'+str(num+1)] = arg
+        strict_json_kwargs = {
+                    my_key: kwargs[my_key] for my_key in kwargs 
+                    if my_key not in self.variable_names and my_key != 'shared_variables'
+                }
+               
                 
         # If strict_json function, do the function. 
         if self.external_fn is None:
             res = await strict_json_async(system_prompt = self.fn_description,
                             user_prompt = function_kwargs,
                             output_format = self.output_format,
-                            llm_async = self.llm_async,
+                            llm = self.llm,
                             **self.kwargs, **strict_json_kwargs)
             
         # Else run the external function
         else:
             res = {}
             # if external function uses shared_variables, pass it in
             argspec = inspect.getfullargspec(self.external_fn)
             if 'shared_variables' in argspec.args:
-                fn_output = self.external_fn(shared_variables = shared_variables, **function_kwargs)
+                if  inspect.iscoroutinefunction(self.external_fn):
+                    fn_output = await self.external_fn(shared_variables = shared_variables, **function_kwargs)
+                else: 
+                    fn_output = self.external_fn(shared_variables = shared_variables, **function_kwargs)
             else:
-                fn_output = self.external_fn(**function_kwargs)
+                if  inspect.iscoroutinefunction(self.external_fn):
+                    fn_output = await self.external_fn(**function_kwargs)
+                else:
+                    fn_output = self.external_fn(**function_kwargs)
                 
             # if there is nothing in fn_output, skip this part
             if fn_output is not None:
                 output_keys = list(self.output_format.keys())
                 # convert the external function into a tuple format to parse it through the JSON dictionary output format
                 if not isinstance(fn_output, tuple):
                     fn_output = [fn_output]
 
                 for i in range(len(fn_output)):
                     if len(output_keys) > i:
                         res[output_keys[i]] = fn_output[i]
                     else:
                         res[f'output_{i+1}'] = fn_output[i]
         
+         
         # check if any of the output variables have a s_, which means we update the shared_variables and not output it
-        keys = list(res.keys())
-        for each in keys:
-            if each[:2] == 's_':
-                shared_variables[each] = res[each]
-                del res[each]
+        self._update_shared_variables(res, shared_variables)
                 
         if res == {}:
             res = {'Status': 'Completed'}
 
         return res
-    
-### Legacy Support
+
+
     
 # alternative name for strict_function (it is now called Function)
 strict_function = Function
```

### Comparing `taskgen_ai-2.3.1/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-2.4.0/taskgen_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 2.3.1
+Version: 2.4.0
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
 Requires-Dist: dill>=0.3.7
 Requires-Dist: termcolor>=2.3.0
+Requires-Dist: requests
 
-# TaskGen v2.3.1
+# TaskGen v2.4.0
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 - TaskGen Ask Me Anything: https://www.youtube.com/watch?v=mheIWKugqF4
 
 ### Creator's Preamble
@@ -30,14 +31,16 @@
 - Single Agent with LLM Functions
 - Single Agent with External Functions
 - Meta Agent with Inner Agents as Functions
 - Shared Variables for multi-modality support
 - Retrieval Augmented Generation (RAG) over Function space
 - Memory to provide additional task-based prompts for task
 - Global Context for configuring your own prompts + add persistent variables
+- Async mode for Agent, Function and `strict_json` added
+- Community Uploading and Downloading of Agent and Functions
 
 I am quite sure that this is the best open-source agentic framework for task-based execution out there! 
 Existing frameworks like AutoGen rely too much on conversational text which is lengthy and not targeted.
 TaskGen uses StrictJSON (JSON parser with type checking and more!) as the core, and agents are efficient and are able to do Chain of Thought natively using JSON keys and descriptions as a guide.
 
 What can you do to help: 
 - Star the github so more people can use it (It's open source and free to use, even commercially!)
@@ -380,17 +383,24 @@
 - Implementing your own specific instructions to the default planner prompt
     - Implement your own memory-based RAG / global prompt instruction if you need more than what the default prompt can achieve
 <br></br>
 - Avoid Multiple Similar Subtasks in `subtasks_history`
     - If you have multiple similar subtask names, then it is likely the Agent can be confused and think it has already done the subtask
     - In this case, you can disambiguate by resetting the agent and store the persistent information in `shared_variables` and provide it to the agent using `get_global_context`
     - Has the benefit of shifting the Start State closer to End State desired by resetting the Agent's planning cycle
+    
+# Async Agents, Functions, strict_json (See Tutorial 8 and 9)
+- TaskGen now supports Async functionalities
+- We use `AsyncAgent`, `AsyncFunction` and `strict_json_async`
+    - These are the async equivalents of `Agent`, `Function` and `strict_json`
+
 
 # Known Limitations
-- To be added
+- `gpt-3.5-turbo` is not that great with mathematical functions for Agents. Use `gpt-4-turbo` or better for more consistent results
+- `gpt-3.5-turbo` is not that great with Memory (Tutorial 4). Use `gpt-4-turbo` or better for more consistent results
 
 # Contributing to the project
 
 ## Test locally
 1. Clone the repository
 2. If using a virtual environment, activate it
 3. `cd` into taskgen repository
@@ -401,11 +411,11 @@
 1. Fork the repository
 2. Create a new branch
 3. Make your changes
 4. Push your changes to your fork
 5. Submit a pull request
 
 # What are we looking out for?
-1. Integrations with functions - It would be good if we could import function definitions from elsewhere, e.g. LangChain, into the format shown here. It might even be done automatically using LLM-based conversion using StrictJSON!
+1. Contributing example Agents and Functions. Agents can now be contributed easily using `agent.contribute_agent()` and the entire Agent code with all the functions and memory will be converted to text-based code and put on the TaskGen GitHub. Do share your use cases actively so that other people can benefit :) These Agents can be downloaded by others via `agent.load_community_agent(agent_name)`
 2. Jupyter Notebooks showcasing what could be done with the framework for something useful. Let your imagination guide you, we look forward to see what you create
 3. Other Known Limitations - Do test the framework out extensively and note its failure cases. We will see if we can address them, if not we will put them in Known Limitations.
 4. (For the prompt engineer). If you could find a better way to make the prompts work, let us know directly - we do need to test this out across all Tutorial Jupyter Notebooks to make sure that it really works with existing datasets. Also, if you are using other LLMs beside OpenAI, and find the prompts do not work as well - try to rejig your own prompts and let us know as well!
```

