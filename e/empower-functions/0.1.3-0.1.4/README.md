# Comparing `tmp/empower_functions-0.1.3.tar.gz` & `tmp/empower_functions-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empower_functions-0.1.3.tar", last modified: Tue May 21 03:50:07 2024, max compression
+gzip compressed data, was "empower_functions-0.1.4.tar", last modified: Sat Jun  1 22:33:09 2024, max compression
```

## Comparing `empower_functions-0.1.3.tar` & `empower_functions-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-21 03:50:07.093479 empower_functions-0.1.3/
--rw-r--r--   0 yulong     (501) staff       (20)      849 2024-05-21 03:50:07.093264 empower_functions-0.1.3/PKG-INFO
--rw-r--r--   0 yulong     (501) staff       (20)    13239 2024-05-21 03:49:14.000000 empower_functions-0.1.3/README.md
-drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-21 03:50:07.092294 empower_functions-0.1.3/empower_functions/
--rw-r--r--   0 yulong     (501) staff       (20)      277 2024-05-17 20:27:57.000000 empower_functions-0.1.3/empower_functions/README.md
--rw-r--r--   0 yulong     (501) staff       (20)      173 2024-05-16 16:18:45.000000 empower_functions-0.1.3/empower_functions/__init__.py
--rw-r--r--   0 yulong     (501) staff       (20)    11879 2024-05-17 17:47:18.000000 empower_functions-0.1.3/empower_functions/chat_handler.py
--rw-r--r--   0 yulong     (501) staff       (20)     7070 2024-05-21 03:49:14.000000 empower_functions-0.1.3/empower_functions/prompt.py
--rw-r--r--   0 yulong     (501) staff       (20)     9171 2024-05-16 19:45:02.000000 empower_functions-0.1.3/empower_functions/server.py
-drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-05-21 03:50:07.093013 empower_functions-0.1.3/empower_functions.egg-info/
--rw-r--r--   0 yulong     (501) staff       (20)      849 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/PKG-INFO
--rw-r--r--   0 yulong     (501) staff       (20)      387 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/SOURCES.txt
--rw-r--r--   0 yulong     (501) staff       (20)        1 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/dependency_links.txt
--rw-r--r--   0 yulong     (501) staff       (20)       41 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/requires.txt
--rw-r--r--   0 yulong     (501) staff       (20)       18 2024-05-21 03:50:07.000000 empower_functions-0.1.3/empower_functions.egg-info/top_level.txt
--rw-r--r--   0 yulong     (501) staff       (20)      686 2024-05-21 03:49:42.000000 empower_functions-0.1.3/pyproject.toml
--rw-r--r--   0 yulong     (501) staff       (20)       38 2024-05-21 03:50:07.093533 empower_functions-0.1.3/setup.cfg
--rw-r--r--   0 yulong     (501) staff       (20)      629 2024-05-21 03:49:35.000000 empower_functions-0.1.3/setup.py
+drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-06-01 22:33:09.634506 empower_functions-0.1.4/
+-rw-r--r--   0 yulong     (501) staff       (20)      763 2024-06-01 22:33:09.634389 empower_functions-0.1.4/PKG-INFO
+-rw-r--r--   0 yulong     (501) staff       (20)    14052 2024-05-21 17:26:59.000000 empower_functions-0.1.4/README.md
+drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-06-01 22:33:09.633356 empower_functions-0.1.4/empower_functions/
+-rw-r--r--   0 yulong     (501) staff       (20)      277 2024-05-21 17:26:26.000000 empower_functions-0.1.4/empower_functions/README.md
+-rw-r--r--   0 yulong     (501) staff       (20)      173 2024-05-21 17:26:26.000000 empower_functions-0.1.4/empower_functions/__init__.py
+-rw-r--r--   0 yulong     (501) staff       (20)    12492 2024-06-01 22:31:54.000000 empower_functions-0.1.4/empower_functions/chat_handler.py
+-rw-r--r--   0 yulong     (501) staff       (20)     7441 2024-06-01 22:31:54.000000 empower_functions-0.1.4/empower_functions/prompt.py
+-rw-r--r--   0 yulong     (501) staff       (20)     9493 2024-06-01 22:31:54.000000 empower_functions-0.1.4/empower_functions/server.py
+drwxr-xr-x   0 yulong     (501) staff       (20)        0 2024-06-01 22:33:09.634239 empower_functions-0.1.4/empower_functions.egg-info/
+-rw-r--r--   0 yulong     (501) staff       (20)      763 2024-06-01 22:33:09.000000 empower_functions-0.1.4/empower_functions.egg-info/PKG-INFO
+-rw-r--r--   0 yulong     (501) staff       (20)      387 2024-06-01 22:33:09.000000 empower_functions-0.1.4/empower_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 yulong     (501) staff       (20)        1 2024-06-01 22:33:09.000000 empower_functions-0.1.4/empower_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 yulong     (501) staff       (20)       41 2024-06-01 22:33:09.000000 empower_functions-0.1.4/empower_functions.egg-info/requires.txt
+-rw-r--r--   0 yulong     (501) staff       (20)       18 2024-06-01 22:33:09.000000 empower_functions-0.1.4/empower_functions.egg-info/top_level.txt
+-rw-r--r--   0 yulong     (501) staff       (20)      686 2024-06-01 22:32:15.000000 empower_functions-0.1.4/pyproject.toml
+-rw-r--r--   0 yulong     (501) staff       (20)       38 2024-06-01 22:33:09.634544 empower_functions-0.1.4/setup.cfg
+-rw-r--r--   0 yulong     (501) staff       (20)      629 2024-06-01 22:32:21.000000 empower_functions-0.1.4/setup.py
```

### Comparing `empower_functions-0.1.3/PKG-INFO` & `empower_functions-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: empower_functions
-Version: 0.1.3
+Version: 0.1.4
 Summary: The empower_functions package provides a set of utility functions to run the empower-functions model
 Author-email: "empower.dev" <yulong@empower.dev>
 Project-URL: Homepage, https://empower.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: jinja2
-Requires-Dist: llama-cpp-python[server]
-Requires-Dist: pydantic
 
 ## Project Description
 
 This is the pip package for the empower-functions LLMs which offer GPT-4 level capatiblities for real-world "tool-using" use cases.
 
 For more information, please visit the [Empower Functions](https://github.com/empower-ai/empower-functions) Github repo.
```

### Comparing `empower_functions-0.1.3/README.md` & `empower_functions-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,40 +15,40 @@
 Real-world use cases, particularly those involving conversational agents, often introduce complex requirements for LLMs. Models must be capable of retrieving context from multiple round of conversations([multi-turn](docs/inference/multi-turn.md)), choosing between utilizing tools or engaging in standard dialogue (['auto' mode](docs/inference/introduction.md#tools-parameter)), and asking for clarification if any parameters are missing([clarification](docs/inference/clarification.md)). Furthermore, they should integrate responses with tool outputs in a [streaming](docs/inference/streaming.md) fashion. Additionally, when multiple tools are required to complete a task, models should efficiently execute multiple functions either in parallel ([parallel calling](docs/inference/parallel-calling.md)) or sequentially with dependencies ([sequential calling](docs/inference/sequential-calling.md)).
 
 For example, below is a screenshot demonstrating how the model is used in a medical center coordinator bot. You can explore this further in our [live demo](https://app.empower.dev/chat-demo).
 ![image](assets/demo_screenshot.png)
 
 ## Family of Models
 
-| Model                    | Specs                                                                                             | Links                                                                                                                                                      |                                     |
-| ------------------------ | ------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
-| empower-functions-small  | 8k context, based on [Llama3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B)               | [model](https://huggingface.co/empower-dev/llama3-empower-functions-small), [GGUF](https://huggingface.co/empower-dev/llama3-empower-functions-small-gguf) | most cost effective, local runnable |
-| empower-functions-medium | 32k context, based on [Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) | [model](https://huggingface.co/empower-dev/empower-functions-medium)                                                                                       | balance in accuracy and cost        |
-| empower-functions-large  | 65k context, based on [Mixtral 8x22B](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1)        | model                                                                                                                                                      | best accuracy                       |
+| Model                           | Specs                                                                                             | Links                                                                                                                           | Notes                                |
+| ------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
+| llama3-empower-functions-small  | 8k context, based on [Llama3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B)               | [model](https://huggingface.co/empower-dev/llama3-empower-functions-small), [GGUF](https://huggingface.co/empower-dev/llama3-empower-functions-small-gguf)   | Most cost-effective, locally runnable |
+| empower-functions-medium        | 32k context, based on [Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) | [model](https://huggingface.co/empower-dev/empower-functions-medium)                                                             | Balance in accuracy and cost         |
+| llama3-empower-functions-large  | 8k context, based on [Llama3 70B](https://huggingface.co/meta-llama/Meta-Llama-3-70B)             | [model](https://huggingface.co/empower-dev/llama3-empower-functions-large)                                                      | Best accuracy                        |
 
 #### Hardware Requirement
 
 We have tested and the family of models in following setup:
 
 - empower-functions-small: fp16 on 1xA100 40G, GGUF and 4bit GGUF on Macbook M2 Pro with 32G RAM, in minimal the 4bit GGUF version requires 7.56G RAM.
 - empower-functions-medium: fp16 on 2xA100 80G
 - empower-functions-large: fp16 on 4xA100 80G
 
 ## How to Use?
 
 #### Running Locally
 
-> Running locally is only supported by empower-functions-small model. To use other models, please use our API.
+> Running locally is only supported by the `llama3-empower-functions-small` model. To use other models, please use our API.
 
 Local running is supported through the `empower_functions` pip package, make sure you install it first by running `pip install empower-functions`.
 
-> If you run into errors like RuntimeError: Failed to load shared library, (mach-o file, but is an incompatible architecture (have 'x86_64', need 'arm64')), please re-install the llama-cpp-python package by running `CMAKE_ARGS="-DCMAKE_OSX_ARCHITECTURES=arm64 -DCMAKE_APPLE_SILICON_PROCESSOR=arm64 -DLLAMA_METAL=on" pip install --upgrade --verbose --force-reinstall --no-cache-dir llama-cpp-python`
+> If you encounter errors like RuntimeError: Failed to load shared library, (mach-o file, but is an incompatible architecture (have 'x86_64', need 'arm64')), please re-install the llama-cpp-python package by running `CMAKE_ARGS="-DCMAKE_OSX_ARCHITECTURES=arm64 -DCMAKE_APPLE_SILICON_PROCESSOR=arm64 -DLLAMA_METAL=on" pip install --upgrade --verbose --force-reinstall --no-cache-dir llama-cpp-python`
 
 <details>
-<summary>Using a Local OpenAI Compatible Server</summary>
+<summary>Running a Local OpenAI Compatible Server</summary>
 
 We leverage the `llama-cpp-python` project to run the model locally. To start a local OpenAI compatible server, you'll need to follow the steps below:
 
 1. Download the GGUF model from our [huggingface repo](TODO)
 2. Run the command `python -m empower_functions.server --model <path to GGUF model> --chat_format empower-functions`
 
 You should see the following output when the server is ready:
@@ -111,23 +111,55 @@
 ```python
 import json
 from empower_functions import EmpowerFunctionsCompletionHandler
 from llama_cpp.llama_tokenizer import LlamaHFTokenizer
 from llama_cpp import Llama
 
 llm = Llama.from_pretrained(
-    repo_id="liuylhf/llama-8b-gguf",
+    repo_id="empower-dev/llama3-empower-functions-small-gguf",
     filename="ggml-model-Q4_K_M.gguf",
     chat_format="llama-3",
     chat_handler=EmpowerFunctionsCompletionHandler(),
-    tokenizer=LlamaHFTokenizer.from_pretrained("liuylhf/llama-8b-gguf"),
+    tokenizer=LlamaHFTokenizer.from_pretrained("empower-dev/llama3-empower-functions-small-gguf"),
     n_gpu_layers=0
 )
 
-# You can use the llm object to chat with the model
+# You can then use the llm object to chat with the model
+messages = [
+    {"role": "user", "content": "What's the weather in San Francisco?"}
+]
+
+tools = [
+    {
+        "type": "function",
+        "function": {
+            "name": "get_current_weather",
+            "description": "Get the current weather",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "location": {
+                        "type": "string",
+                        "description": "The city and state, e.g., San Francisco, CA"
+                    }
+                },
+                "required": ["location"]
+            }
+        }
+    }
+]
+
+result = llm.create_chat_completion(
+      messages = messages,
+      tools=tools,
+      tool_choice="auto",
+      max_tokens=128
+)
+print(json.dumps(result["choices"][0], indent=2))
+
 ```
 
 </details>
 
 #### Using Empower API
 
 The empower platform offers an API that is fully compatible with the OpenAI API, allowing you to directly use the OpenAI SDK. An example is shown below. See below for a basic example, more details can be found [here](/docs/inference/introduction.md).
```

#### html2text {}

```diff
@@ -22,74 +22,85 @@
 when multiple tools are required to complete a task, models should efficiently
 execute multiple functions either in parallel ([parallel calling](docs/
 inference/parallel-calling.md)) or sequentially with dependencies ([sequential
 calling](docs/inference/sequential-calling.md)). For example, below is a
 screenshot demonstrating how the model is used in a medical center coordinator
 bot. You can explore this further in our [live demo](https://app.empower.dev/
 chat-demo). ![image](assets/demo_screenshot.png) ## Family of Models | Model |
-Specs | Links | | | ------------------------ | --------------------------------
------------------------------------------------------------------ | -----------
--------------------------------------------------------------------------------
----------------------------------------------------------------- | ------------
------------------------ | | empower-functions-small | 8k context, based on
-[Llama3 8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B) | [model](https:
-//huggingface.co/empower-dev/llama3-empower-functions-small), [GGUF](https://
-huggingface.co/empower-dev/llama3-empower-functions-small-gguf) | most cost
-effective, local runnable | | empower-functions-medium | 32k context, based on
-[Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) |
-[model](https://huggingface.co/empower-dev/empower-functions-medium) | balance
-in accuracy and cost | | empower-functions-large | 65k context, based on
-[Mixtral 8x22B](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1) | model |
-best accuracy | #### Hardware Requirement We have tested and the family of
+Specs | Links | Notes | | ------------------------------- | -------------------
+-----------------------------------------------------------------------------
+- | ---------------------------------------------------------------------------
+---------------------------------------------------- | ------------------------
+------------ | | llama3-empower-functions-small | 8k context, based on [Llama3
+8B](https://huggingface.co/meta-llama/Meta-Llama-3-8B) | [model](https://
+huggingface.co/empower-dev/llama3-empower-functions-small), [GGUF](https://
+huggingface.co/empower-dev/llama3-empower-functions-small-gguf) | Most cost-
+effective, locally runnable | | empower-functions-medium | 32k context, based
+on [Mixtral 8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
+| [model](https://huggingface.co/empower-dev/empower-functions-medium) |
+Balance in accuracy and cost | | llama3-empower-functions-large | 8k context,
+based on [Llama3 70B](https://huggingface.co/meta-llama/Meta-Llama-3-70B) |
+[model](https://huggingface.co/empower-dev/llama3-empower-functions-large) |
+Best accuracy | #### Hardware Requirement We have tested and the family of
 models in following setup: - empower-functions-small: fp16 on 1xA100 40G, GGUF
 and 4bit GGUF on Macbook M2 Pro with 32G RAM, in minimal the 4bit GGUF version
 requires 7.56G RAM. - empower-functions-medium: fp16 on 2xA100 80G - empower-
 functions-large: fp16 on 4xA100 80G ## How to Use? #### Running Locally >
-Running locally is only supported by empower-functions-small model. To use
-other models, please use our API. Local running is supported through the
-`empower_functions` pip package, make sure you install it first by running `pip
-install empower-functions`. > If you run into errors like RuntimeError: Failed
-to load shared library, (mach-o file, but is an incompatible architecture (have
-'x86_64', need 'arm64')), please re-install the llama-cpp-python package by
-running `CMAKE_ARGS="-DCMAKE_OSX_ARCHITECTURES=arm64 -
-DCMAKE_APPLE_SILICON_PROCESSOR=arm64 -DLLAMA_METAL=on" pip install --upgrade --
-verbose --force-reinstall --no-cache-dir llama-cpp-python` Using a Local OpenAI
-Compatible Server We leverage the `llama-cpp-python` project to run the model
-locally. To start a local OpenAI compatible server, you'll need to follow the
-steps below: 1. Download the GGUF model from our [huggingface repo](TODO) 2.
-Run the command `python -m empower_functions.server --model --chat_format
-empower-functions` You should see the following output when the server is
-ready: `INFO: Uvicorn running on http://localhost:8000 (Press CTRL+C to quit)`
-Then you can use the OpenAI SDK to connect to the server. See below for a basic
-example: ```python import openai import json client = openai.OpenAI( base_url =
-"http://localhost:8000/v1", api_key = "YOUR_API_KEY" ) messages = [ {"role":
-"user", "content": "What's the weather in San Francisco?"} ] tools = [
-{ "type": "function", "function": { "name": "get_current_weather",
-"description": "Get the current weather", "parameters": { "type": "object",
-"properties": { "location": { "type": "string", "description": "The city and
-state, e.g., San Francisco, CA" } }, "required": ["location"] } } } ]
-chat_completion = client.chat.completions.create( model="does_not_matter",
-messages=messages, tools=tools, temperature=0, tool_choice="auto" ) print
-(chat_completion) ``` Running in a Python Environment You can directly call the
-model in your python environment through the `llama-cpp-python` package with
-the chat handler provided in the `empower_functions` package. See below for a
-basic example. For more detailed example, please refer to the [python script]
-(https://github.com/empower-ai/empower-functions/blob/main/examples/
-llama_cpp_inference.py). ```python import json from empower_functions import
+Running locally is only supported by the `llama3-empower-functions-small`
+model. To use other models, please use our API. Local running is supported
+through the `empower_functions` pip package, make sure you install it first by
+running `pip install empower-functions`. > If you encounter errors like
+RuntimeError: Failed to load shared library, (mach-o file, but is an
+incompatible architecture (have 'x86_64', need 'arm64')), please re-install the
+llama-cpp-python package by running `CMAKE_ARGS="-
+DCMAKE_OSX_ARCHITECTURES=arm64 -DCMAKE_APPLE_SILICON_PROCESSOR=arm64 -
+DLLAMA_METAL=on" pip install --upgrade --verbose --force-reinstall --no-cache-
+dir llama-cpp-python` Running a Local OpenAI Compatible Server We leverage the
+`llama-cpp-python` project to run the model locally. To start a local OpenAI
+compatible server, you'll need to follow the steps below: 1. Download the GGUF
+model from our [huggingface repo](TODO) 2. Run the command `python -
+m empower_functions.server --model --chat_format empower-functions` You should
+see the following output when the server is ready: `INFO: Uvicorn running on
+http://localhost:8000 (Press CTRL+C to quit)` Then you can use the OpenAI SDK
+to connect to the server. See below for a basic example: ```python import
+openai import json client = openai.OpenAI( base_url = "http://localhost:8000/
+v1", api_key = "YOUR_API_KEY" ) messages = [ {"role": "user", "content":
+"What's the weather in San Francisco?"} ] tools = [ { "type": "function",
+"function": { "name": "get_current_weather", "description": "Get the current
+weather", "parameters": { "type": "object", "properties": { "location":
+{ "type": "string", "description": "The city and state, e.g., San Francisco,
+CA" } }, "required": ["location"] } } } ] chat_completion =
+client.chat.completions.create( model="does_not_matter", messages=messages,
+tools=tools, temperature=0, tool_choice="auto" ) print(chat_completion) ```
+Running in a Python Environment You can directly call the model in your python
+environment through the `llama-cpp-python` package with the chat handler
+provided in the `empower_functions` package. See below for a basic example. For
+more detailed example, please refer to the [python script](https://github.com/
+empower-ai/empower-functions/blob/main/examples/llama_cpp_inference.py).
+```python import json from empower_functions import
 EmpowerFunctionsCompletionHandler from llama_cpp.llama_tokenizer import
 LlamaHFTokenizer from llama_cpp import Llama llm = Llama.from_pretrained
-( repo_id="liuylhf/llama-8b-gguf", filename="ggml-model-Q4_K_M.gguf",
-chat_format="llama-3", chat_handler=EmpowerFunctionsCompletionHandler(),
-tokenizer=LlamaHFTokenizer.from_pretrained("liuylhf/llama-8b-gguf"),
-n_gpu_layers=0 ) # You can use the llm object to chat with the model ``` ####
-Using Empower API The empower platform offers an API that is fully compatible
-with the OpenAI API, allowing you to directly use the OpenAI SDK. An example is
-shown below. See below for a basic example, more details can be found [here](/
-docs/inference/introduction.md). Currently streaming and JSON model is only
-available in Empower API. ```python from openai import OpenAI client = OpenAI
+( repo_id="empower-dev/llama3-empower-functions-small-gguf", filename="ggml-
+model-Q4_K_M.gguf", chat_format="llama-3",
+chat_handler=EmpowerFunctionsCompletionHandler(),
+tokenizer=LlamaHFTokenizer.from_pretrained("empower-dev/llama3-empower-
+functions-small-gguf"), n_gpu_layers=0 ) # You can then use the llm object to
+chat with the model messages = [ {"role": "user", "content": "What's the
+weather in San Francisco?"} ] tools = [ { "type": "function", "function":
+{ "name": "get_current_weather", "description": "Get the current weather",
+"parameters": { "type": "object", "properties": { "location": { "type":
+"string", "description": "The city and state, e.g., San Francisco, CA" } },
+"required": ["location"] } } } ] result = llm.create_chat_completion( messages
+= messages, tools=tools, tool_choice="auto", max_tokens=128 ) print(json.dumps
+(result["choices"][0], indent=2)) ``` #### Using Empower API The empower
+platform offers an API that is fully compatible with the OpenAI API, allowing
+you to directly use the OpenAI SDK. An example is shown below. See below for a
+basic example, more details can be found [here](/docs/inference/
+introduction.md). Currently streaming and JSON model is only available in
+Empower API. ```python from openai import OpenAI client = OpenAI
 ( base_url="https://app.empower.dev/api/v1", api_key="YOU_API_KEY" ) response =
 client.chat.completions.create( model="empower-functions", messages=[{"role":
 "user", "content": "What's the weather in San Francisco and Los Angles in
 Celsius?"}], temperature=0, tools=[{ "type": "function", "function": { "name":
 "get_current_weather", "description": "Get the current weather in a given
 location", "parameters": { "type": "object", "properties": { "location":
 { "type": "string", "description": "The city and state, e.g. San Francisco,
```

### Comparing `empower_functions-0.1.3/empower_functions/chat_handler.py` & `empower_functions-0.1.4/empower_functions/chat_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import json
 
-from typing import Any, Dict, Iterator, List, Literal, Optional, Tuple, Union, Protocol, cast
+from typing import (
+    Any,
+    Dict,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+    Protocol,
+    cast,
+)
 
 import jinja2
 from jinja2.sandbox import ImmutableSandboxedEnvironment
 
 import llama_cpp.llama as llama
 import llama_cpp.llama_types as llama_types
 from llama_cpp.llama_chat_format import LlamaChatCompletionHandler
 from empower_functions.prompt import prompt_messages
+import traceback
 
-class EmpowerFunctionsCompletionHandler(LlamaChatCompletionHandler):
-    SYSTEM_INSTRUCTION = "In this environment you have access to a set of functions defined in the JSON format you can use to address user's requests, use them if needed."
 
+class EmpowerFunctionsCompletionHandler(LlamaChatCompletionHandler):
     def __call__(
         self,
         llama: llama.Llama,
         messages: List[llama_types.ChatCompletionRequestMessage],
         functions: Optional[List[llama_types.ChatCompletionFunction]] = None,
         function_call: Optional[llama_types.ChatCompletionRequestFunctionCall] = None,
         tools: Optional[List[llama_types.ChatCompletionTool]] = None,
@@ -24,15 +35,17 @@
         temperature: float = 0.2,
         top_p: float = 0.95,
         top_k: int = 40,
         min_p: float = 0.05,
         typical_p: float = 1.0,
         stream: bool = False,
         stop: Optional[Union[str, List[str]]] = [],
-        response_format: Optional[llama_types.ChatCompletionRequestResponseFormat] = None,
+        response_format: Optional[
+            llama_types.ChatCompletionRequestResponseFormat
+        ] = None,
         max_tokens: Optional[int] = None,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         repeat_penalty: float = 1.1,
         tfs_z: float = 1.0,
         mirostat_mode: int = 0,
         mirostat_tau: float = 5.0,
@@ -42,15 +55,15 @@
         grammar: Optional[llama.LlamaGrammar] = None,
         logprobs: Optional[bool] = None,
         top_logprobs: Optional[int] = None,
         **kwargs,  # type: ignore
     ) -> Union[
         llama_types.CreateChatCompletionResponse,
         Iterator[llama_types.CreateChatCompletionStreamResponse],
-    ]:        
+    ]:
         template = "{% set loop_messages = messages %}{% for message in loop_messages %}{% set content = '<|start_header_id|>' + message['role'] + '<|end_header_id|>\n\n'+ message['content'] | trim + '<|eot_id|>' %}{% if loop.index0 == 0 %}{% set content = '<|begin_of_text|>' + content %}{% endif %}{{ content }}{% endfor %}{% if add_generation_prompt %}{{ '<|start_header_id|>assistant<|end_header_id|>\n\n' }}{% endif %}"
         template_renderer = ImmutableSandboxedEnvironment(
             autoescape=False,
             undefined=jinja2.StrictUndefined,
         ).from_string(template)
 
         # Convert legacy function_call to tool_choice
@@ -68,126 +81,152 @@
                 }
         if not tool_choice:
             tool_choice = "auto"
 
         assert tool_choice != "any"
 
         if functions is None:
-            functions = [ tool.get('function') for tool in tools ]
-        stop = [stop, "<|eot_id|>"] if isinstance(stop, str) else stop + ["<|eot_id|>"] if stop else ["<|eot_id|>"]
+            functions = [tool.get("function") for tool in tools]
+        stop = (
+            [stop, "<|eot_id|>"]
+            if isinstance(stop, str)
+            else stop + ["<|eot_id|>"] if stop else ["<|eot_id|>"]
+        )
 
         if tool_choice == "none":
             functions = []
-        prompted_messages = prompt_messages(messages, functions)
-        prompt = template_renderer.render(messages=prompted_messages, add_generation_prompt=True)
+
+        include_thinking = False
+        if "include_thinking" in kwargs:
+            include_thinking = kwargs["include_thinking"]
+        prompted_messages = prompt_messages(
+            messages, functions, include_thinking=include_thinking
+        )
+        prompt = template_renderer.render(
+            messages=prompted_messages, add_generation_prompt=True
+        )
 
         # Case 1: No tool choice by user
         generated = llama.create_completion(
-                prompt=prompt,
-                temperature=temperature,
-                top_p=top_p,
-                top_k=top_k,
-                min_p=min_p,
-                typical_p=typical_p,
-                stream=stream,
-                stop=stop,
-                max_tokens=max_tokens,
-                presence_penalty=presence_penalty,
-                frequency_penalty=frequency_penalty,
-                repeat_penalty=repeat_penalty,
-                tfs_z=tfs_z,
-                mirostat_mode=mirostat_mode,
-                mirostat_tau=mirostat_tau,
-                mirostat_eta=mirostat_eta,
-                model=model,
-                logits_processor=logits_processor,
-                grammar=grammar,
-                logprobs=top_logprobs if logprobs else None,
-            )
-        generated_text = generated['choices'][0]['text']
-        if generated_text.startswith('<f>'):
-            json_object = json.loads(generated_text[3:])
+            prompt=prompt,
+            temperature=temperature,
+            top_p=top_p,
+            top_k=top_k,
+            min_p=min_p,
+            typical_p=typical_p,
+            stream=stream,
+            stop=stop,
+            max_tokens=max_tokens,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            repeat_penalty=repeat_penalty,
+            tfs_z=tfs_z,
+            mirostat_mode=mirostat_mode,
+            mirostat_tau=mirostat_tau,
+            mirostat_eta=mirostat_eta,
+            model=model,
+            logits_processor=logits_processor,
+            grammar=grammar,
+            logprobs=top_logprobs if logprobs else None,
+        )
+        thinking = None
+        content = None
+
+        (content, thinking) = _separate_thinking_if_present(
+            generated["choices"][0]["text"]
+        )
+        if content.startswith("<f>"):
+            generated["choices"][0]["text"] = content
             return _convert_completion_to_chat_function(
-                completion_or_chunks=generated
+                completion_or_chunks=generated,
+                thinking=thinking,
             )
-        elif generated_text.startswith('<c>'):
-            generated['choices'][0]['text'] = generated_text[3:]
+        elif content.startswith("<c>"):
+            generated["choices"][0]["text"] = thinking + content[3:]
             return _convert_completion_to_chat(generated, stream=stream)
 
         return _convert_completion_to_chat(generated, stream=stream)
 
+
 def _convert_completion_to_chat(
     completion_or_chunks: Union[
         llama_types.CreateCompletionResponse,
         Iterator[llama_types.CreateCompletionStreamResponse],
     ],
     stream: bool = False,
 ) -> Union[
     llama_types.CreateChatCompletionResponse, Iterator[llama_types.ChatCompletionChunk]
 ]:
     if stream:
-        chunks: Iterator[llama_types.CreateCompletionStreamResponse] = completion_or_chunks  # type: ignore
+        # type: ignore
+        chunks: Iterator[llama_types.CreateCompletionStreamResponse] = completion_or_chunks
         return _convert_text_completion_chunks_to_chat(chunks)
     else:
         completion: llama_types.Completion = completion_or_chunks  # type: ignore
         return _convert_text_completion_to_chat(completion)
 
+
 def _maybe_json_dumps(value: Any) -> str:
     if isinstance(value, str):
         return value
     return json.dumps(value)
 
 
 def _convert_completion_to_chat_function(
     completion_or_chunks: llama_types.CreateCompletionResponse,
+    thinking: Optional[str] = None,
 ):
     completion: llama_types.CreateCompletionResponse = completion_or_chunks  # type: ignore
     assert "usage" in completion
     # tool_id = "call_" + "_0_" + tool_name + "_" + completion["id"]
     # TODO: Fix for legacy function calls
     json_object = json.loads(completion["choices"][0]["text"][3:])
 
-    print(json.dumps(json_object, indent=2))
-
     tool_calls = [
         {
-            "id": "call_" + "_0_" + tool['name'] + "_" + completion["id"] + "_" + str(i),
+            "id": "call_"
+            + "_0_"
+            + tool["name"]
+            + "_"
+            + completion["id"]
+            + "_"
+            + str(i),
             "type": "function",
             "function": {
-                "name": tool['name'],
-                "arguments": _maybe_json_dumps(tool['arguments']),
+                "name": tool["name"],
+                "arguments": _maybe_json_dumps(tool["arguments"]),
             },
         }
-
         for (i, tool) in enumerate(json_object)
     ]
-    
+
     json_object = json.loads(completion["choices"][0]["text"][3:])
-    
+
     chat_completion: llama_types.CreateChatCompletionResponse = {
         "id": "chat" + completion["id"],
         "object": "chat.completion",
         "created": completion["created"],
         "model": completion["model"],
         "choices": [
             {
                 "index": 0,
                 "message": {
                     "role": "assistant",
-                    "content": None,
-                    "tool_calls": tool_calls
+                    "content": thinking,
+                    "tool_calls": tool_calls,
                 },
                 "logprobs": completion["choices"][0]["logprobs"],
                 "finish_reason": "tool_calls",
             }
         ],
         "usage": completion["usage"],
     }
     return chat_completion
 
+
 def _convert_text_completion_chunks_to_chat(
     chunks: Iterator[llama_types.CreateCompletionStreamResponse],
 ) -> Iterator[llama_types.ChatCompletionChunk]:
     for i, chunk in enumerate(chunks):
         if i == 0:
             yield {
                 "id": "chat" + chunk["id"],
@@ -233,20 +272,22 @@
         Iterator[llama_types.CreateCompletionStreamResponse],
     ],
     stream: bool = False,
 ) -> Union[
     llama_types.CreateChatCompletionResponse, Iterator[llama_types.ChatCompletionChunk]
 ]:
     if stream:
-        chunks: Iterator[llama_types.CreateCompletionStreamResponse] = completion_or_chunks  # type: ignore
+        # type: ignore
+        chunks: Iterator[llama_types.CreateCompletionStreamResponse] = completion_or_chunks
         return _convert_text_completion_chunks_to_chat(chunks)
     else:
         completion: llama_types.Completion = completion_or_chunks  # type: ignore
         return _convert_text_completion_to_chat(completion)
 
+
 def _convert_text_completion_to_chat(
     completion: llama_types.Completion,
 ) -> llama_types.ChatCompletion:
     assert "usage" in completion
     return {
         "id": "chat" + completion["id"],
         "object": "chat.completion",
@@ -304,7 +345,20 @@
                         else {}
                     ),
                     "logprobs": chunk["choices"][0]["logprobs"],
                     "finish_reason": chunk["choices"][0]["finish_reason"],
                 }
             ],
         }
+
+
+def _separate_thinking_if_present(text):
+    tag = "</thinking>"
+    tag_position = text.find(tag)
+
+    if tag_position != -1:
+        # Split the string into two parts
+        part1 = text[: tag_position + len(tag)]
+        part2 = text[tag_position + len(tag):]
+        return part2, part1
+    else:
+        return text, None
```

### Comparing `empower_functions-0.1.3/empower_functions/prompt.py` & `empower_functions-0.1.4/empower_functions/prompt.py`

 * *Files 17% similar despite different names*

```diff
@@ -120,22 +120,29 @@
             updated_messages.append(message)
 
         previous_role = message['role']
 
     return updated_messages
 
 
-def prompt_messages(messages, functions_def):
+def prompt_messages(messages, functions_def, include_thinking=False):
     if not functions_def:
         functions_def = []
 
+    if len(functions_def) == 0 and include_thinking:
+        raise Exception(
+            'Currently thinking mode is only supported with tools. Please provide functions_def to enable thinking mode.')
+
     _check_functions_def(functions_def)
     messages = _check_and_merge_messages(messages)
 
     system_instruction = SYSTEM_INSTRUCTION
+    if include_thinking:
+        system_instruction += "\nMake sure to include your thinking inside < thinking > </thinking > before response."
+
     first_user_message = messages[0]
     starting_index = 1
     if messages[0]['role'] == 'system':
         system_instruction = messages[0]['content']
         first_user_message = messages[1]
         starting_index = 2
```

### Comparing `empower_functions-0.1.3/empower_functions/server.py` & `empower_functions-0.1.4/empower_functions/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+from __future__ import annotations
+
 import llama_cpp
 from llama_cpp.server.model import LlamaProxy
 from llama_cpp.server.settings import ModelSettings
 from llama_cpp.server.__main__ import main
+
 from empower_functions.chat_handler import EmpowerFunctionsCompletionHandler
+import json
+from typing import Optional, Union, Dict
+import llama_cpp
+from llama_cpp.server.model import (
+    LlamaProxy,
+)
+from llama_cpp.server.settings import (
+    ModelSettings,
+)
+from empower_functions.monkey_patch.app import patch_app
+
 # Monkey pacthing the LlamaProxy class
 
+
 def load_llama_from_model_settings(settings: ModelSettings) -> llama_cpp.Llama:
     chat_handler = None
     if settings.chat_format == "empower-functions":
         chat_handler = EmpowerFunctionsCompletionHandler()
     elif settings.chat_format == "llava-1-5":
         assert settings.clip_model_path is not None, "clip model not found"
         if settings.hf_model_repo_id is not None:
@@ -202,19 +217,24 @@
         # Misc
         verbose=settings.verbose,
     )
     if settings.cache:
         if settings.cache_type == "disk":
             if settings.verbose:
                 print(f"Using disk cache with size {settings.cache_size}")
-            cache = llama_cpp.LlamaDiskCache(capacity_bytes=settings.cache_size)
+            cache = llama_cpp.LlamaDiskCache(
+                capacity_bytes=settings.cache_size)
         else:
             if settings.verbose:
                 print(f"Using ram cache with size {settings.cache_size}")
             cache = llama_cpp.LlamaRAMCache(capacity_bytes=settings.cache_size)
         _model.set_cache(cache)
     return _model
 
-LlamaProxy.load_llama_from_model_settings = staticmethod(load_llama_from_model_settings)
+
+LlamaProxy.load_llama_from_model_settings = staticmethod(
+    load_llama_from_model_settings)
 
 if __name__ == "__main__":
+    patch_app()
+
     main()
```

### Comparing `empower_functions-0.1.3/pyproject.toml` & `empower_functions-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "empower_functions"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="empower.dev", email="yulong@empower.dev" }
 ]
 description = "The empower_functions package provides a set of utility functions to run the empower-functions model"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `empower_functions-0.1.3/setup.py` & `empower_functions-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "empower_functions/README.md").read_text()
 
 setup(
     name='empower_functions',  # This is the package name
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),  # This will find the `empower_functions` directory
     install_requires=[
         "jinja2",
         "llama-cpp-python[server]",
         "pydantic"
         # Add your dependencies here
     ],
```

