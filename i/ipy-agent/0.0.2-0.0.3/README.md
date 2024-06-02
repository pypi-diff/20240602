# Comparing `tmp/ipy_agent-0.0.2.tar.gz` & `tmp/ipy_agent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipy_agent-0.0.2.tar", last modified: Sun Jun  2 15:09:22 2024, max compression
+gzip compressed data, was "ipy_agent-0.0.3.tar", last modified: Sun Jun  2 18:54:50 2024, max compression
```

## Comparing `ipy_agent-0.0.2.tar` & `ipy_agent-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-01-22 21:52:29.000000 ipy_agent-0.0.2/LICENSE
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       33 2023-12-26 15:28:37.000000 ipy_agent-0.0.2/MANIFEST.in
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     6093 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5222 2024-06-02 14:55:10.000000 ipy_agent-0.0.2/README.md
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/ipy_agent/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       70 2024-06-02 12:32:54.000000 ipy_agent-0.0.2/ipy_agent/__init__.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      451 2024-03-13 10:59:26.000000 ipy_agent-0.0.2/ipy_agent/attrdict.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     4252 2024-06-02 13:57:26.000000 ipy_agent-0.0.2/ipy_agent/default_preprompt.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5059 2024-06-02 12:58:18.000000 ipy_agent-0.0.2/ipy_agent/dictation.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    12399 2024-05-25 20:09:35.000000 ipy_agent-0.0.2/ipy_agent/get_text.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1562 2024-05-25 20:09:53.000000 ipy_agent-0.0.2/ipy_agent/get_webdriver.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1802 2024-05-25 20:13:46.000000 ipy_agent-0.0.2/ipy_agent/google_search.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1878 2024-06-02 13:50:04.000000 ipy_agent-0.0.2/ipy_agent/init.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     9662 2024-06-02 14:07:07.000000 ipy_agent-0.0.2/ipy_agent/ipy_agent.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1262 2024-05-28 20:11:19.000000 ipy_agent-0.0.2/ipy_agent/llm_client.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       69 2024-06-02 13:32:03.000000 ipy_agent-0.0.2/ipy_agent/main.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     2161 2024-06-02 13:30:07.000000 ipy_agent-0.0.2/ipy_agent/msg_collector.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    16537 2024-05-30 17:55:58.000000 ipy_agent-0.0.2/ipy_agent/retrieval.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    10371 2024-05-29 20:28:02.000000 ipy_agent-0.0.2/ipy_agent/tools.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3070 2024-05-30 18:01:36.000000 ipy_agent-0.0.2/ipy_agent/utils.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5483 2024-06-02 09:46:31.000000 ipy_agent-0.0.2/ipy_agent/voice.py
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/ipy_agent.egg-info/
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     6093 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      603 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       50 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/entry_points.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      163 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/requires.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       10 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/top_level.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/setup.cfg
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1285 2024-06-02 15:09:08.000000 ipy_agent-0.0.2/setup.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 18:54:50.105636 ipy_agent-0.0.3/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-01-22 21:52:29.000000 ipy_agent-0.0.3/LICENSE
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       33 2023-12-26 15:28:37.000000 ipy_agent-0.0.3/MANIFEST.in
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     7120 2024-06-02 18:54:50.105636 ipy_agent-0.0.3/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     6249 2024-06-02 16:19:53.000000 ipy_agent-0.0.3/README.md
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 18:54:50.101636 ipy_agent-0.0.3/ipy_agent/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       31 2024-06-02 18:39:18.000000 ipy_agent-0.0.3/ipy_agent/__init__.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      451 2024-03-13 10:59:26.000000 ipy_agent-0.0.3/ipy_agent/attrdict.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     4252 2024-06-02 13:57:26.000000 ipy_agent-0.0.3/ipy_agent/default_preprompt.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5502 2024-06-02 18:39:13.000000 ipy_agent-0.0.3/ipy_agent/dictation.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    12399 2024-05-25 20:09:35.000000 ipy_agent-0.0.3/ipy_agent/get_text.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1562 2024-05-25 20:09:53.000000 ipy_agent-0.0.3/ipy_agent/get_webdriver.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1802 2024-05-25 20:13:46.000000 ipy_agent-0.0.3/ipy_agent/google_search.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1818 2024-06-02 18:35:46.000000 ipy_agent-0.0.3/ipy_agent/init_shell.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     9771 2024-06-02 18:39:49.000000 ipy_agent-0.0.3/ipy_agent/ipy_agent.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1262 2024-05-28 20:11:19.000000 ipy_agent-0.0.3/ipy_agent/llm_client.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       69 2024-06-02 13:32:03.000000 ipy_agent-0.0.3/ipy_agent/main.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     2161 2024-06-02 13:30:07.000000 ipy_agent-0.0.3/ipy_agent/msg_collector.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    16537 2024-05-30 17:55:58.000000 ipy_agent-0.0.3/ipy_agent/retrieval.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    10371 2024-05-29 20:28:02.000000 ipy_agent-0.0.3/ipy_agent/tools.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3070 2024-05-30 18:01:36.000000 ipy_agent-0.0.3/ipy_agent/utils.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5483 2024-06-02 09:46:31.000000 ipy_agent-0.0.3/ipy_agent/voice.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 18:54:50.101636 ipy_agent-0.0.3/ipy_agent.egg-info/
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     7120 2024-06-02 18:54:49.000000 ipy_agent-0.0.3/ipy_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      609 2024-06-02 18:54:50.000000 ipy_agent-0.0.3/ipy_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-06-02 18:54:49.000000 ipy_agent-0.0.3/ipy_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       50 2024-06-02 18:54:49.000000 ipy_agent-0.0.3/ipy_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      163 2024-06-02 18:54:49.000000 ipy_agent-0.0.3/ipy_agent.egg-info/requires.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       10 2024-06-02 18:54:49.000000 ipy_agent-0.0.3/ipy_agent.egg-info/top_level.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-06-02 18:54:50.105636 ipy_agent-0.0.3/setup.cfg
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1291 2024-06-02 18:35:52.000000 ipy_agent-0.0.3/setup.py
```

### Comparing `ipy_agent-0.0.2/LICENSE` & `ipy_agent-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/PKG-INFO` & `ipy_agent-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,59 @@
-Metadata-Version: 2.1
-Name: ipy_agent
-Version: 0.0.2
-Summary: An AI assistant designed to be integrated in an IPython shell.
-Home-page: https://github.com/B4PT0R/ipy_agent
-Author: Baptiste Ferrand
-Author-email: bferrand.maths@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ipython
-Requires-Dist: PyPDF2
-Requires-Dist: beautifulsoup4
-Requires-Dist: python-docx
-Requires-Dist: get-gecko-driver
-Requires-Dist: google-api-python-client
-Requires-Dist: litellm
-Requires-Dist: numpy
-Requires-Dist: odfpy
-Requires-Dist: openai
-Requires-Dist: pydub
-Requires-Dist: pynput
-Requires-Dist: requests
-Requires-Dist: selenium
-Requires-Dist: sounddevice
-Requires-Dist: tiktoken
-
 
 # ipy_agent
 
 `ipy_agent` is a Python package that implements an AI agent designed to be integrated into any IPython shell (terminal, Jupyter notebook, QtConsole, etc.).
 
 ## Features
 
 - The agent captures all inputs and outputs occurring in the session to populate its context (up to token limit). 
 - Use magic commands `%ai` and `%%ai` to interact with the agent using natural language.
-- Hold `<ctrl>+<space>` to record and transcribe your voice into text inserted at cursor position. Useful to speak out your prompts instead of typing them. 
+- The assistant uses Whisper for multilingual voice synthesis.
+- Hold `<ctrl>+<space>` to record and transcribe your voice into text inserted at cursor position. Useful to speak out your prompts instead of typing them. Once active, it can be used wherever the cursor can go, not just in the notebook. (uses pynput for global keyboard hotkey detection. requires proper permissions to do so.)
 - The agent can autonomously execute Python code within the session.
 - Can be accessed as a declared object in the session, allowing configuration changes or method execution programmatically.
 - Can be used as a smart Python function returning any kind of data/object.
 - Supports various LLM providers and models via [litellm](https://www.litellm.ai/).
 - Integrated tools: The assistant can stream markdown with LaTeX support (in a notebook), talk to you using text to speech, create new code cells in notebooks, observe and extract content (folder, files, URL), introspect python entities (variables, functions, objects, classes, modules...), perform Google searches, perform semantic retrieval using a custom RAG document store (raw text or structured JSON), open files and urls in the browser, open files in a text editor, scrap the web and interact with webpages using a selenium webdriver...
 - Custom tools: you can extend the agent's functionalities by defining your own custom tools.
 
 ## Installation
 
 ```bash
-pip install ipy_agent
+pip install ipy-agent
 ```
 
-## Usage
+## Setup
 
 First, you need to set the API keys for your preferred LLM providers as environment variables.
 Refer to the [litellm](https://www.litellm.ai/) documentation to know the correct names for your environment variables to be recognized.
 
-Integration into the IPython session is as simple as:
+In case you want the agent to be able to use the websearch tool you will also need to setup a Google custom search engine and provide these two API keys:
+
+```bash
+GOOGLE_CUSTOM_SEARCH_API_KEY="..."
+GOOGLE_CUSTOM_SEARCH_CX="..."
+```
+
+These API keys can be placed in your .bashrc, directly in your python code via `os.environ` (not recommended), or provided via a .env file and loaded with python-dotenv for instance.
+
+## Usage
+
+Assuming your API keys are properly set up, integration into the IPython session (such as a Jupyter notebook) is as simple as running:
 
 ```python
 from ipy_agent import IPyAgent
 IPyAgent(name="Jarvis", username="Baptiste");
 ```
 
 Once loaded, the agent can be accessed in the namespace by the name you gave it in lowercase (`jarvis` in this case) and will respond to line and cell magics `%ai` and `%%ai` respectively. If no custom name is provided, the agent will be accessible by default as `agent`.
 
+Alternatively, you may run the command `ipy_agent` directly in the terminal. This will open a new terminal IPython session with the agent already loaded with default configuration. (Just be aware that voice dictation via `<ctrl>+<space>` tend to freeze the terminal IPython shell.)
+
+
 ### Configuration
 
 You can customize the agent by modifying its configuration. Here are some examples:
 
 ```python
 jarvis.config.model = "claude-3-opus-20240229"  # Use Claude-3 LLM model
 jarvis.config.temperature = 0.7  # Adjust the model temperature
@@ -97,15 +82,15 @@
 You can use the agent as a smart python function:
 
 ```python
 even_list = jarvis("Return a list of n even numbers", n=5)
 even_list # Output: [0, 2, 4, 6, 8]
 ```
 
-When doing so, the agent's markdown output will be silenced and only the result of computation will be returned.
+When doing so, the agent's markdown output will be silenced and only the result of computations will be returned.
 
 ### Available Tools
 
 The agent provides several built-in tools to ease various tasks. These tools are primarily intended for the agent's usage but can also be used by the user. Here is a list of available tools:
 
 - `agent.observe(source)` : Extracts information from a folder, file, URL, variable, function, class, or module, and injects it into the agent's context.
 - `agent.get_text(source)` : Extracts and returns text from a folder, file, URL, variable, function, class, or module.
```

### Comparing `ipy_agent-0.0.2/README.md` & `ipy_agent-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,89 @@
+Metadata-Version: 2.1
+Name: ipy_agent
+Version: 0.0.3
+Summary: An AI assistant designed to be integrated in an IPython shell.
+Home-page: https://github.com/B4PT0R/ipy_agent
+Author: Baptiste Ferrand
+Author-email: bferrand.maths@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython
+Requires-Dist: PyPDF2
+Requires-Dist: beautifulsoup4
+Requires-Dist: python-docx
+Requires-Dist: get-gecko-driver
+Requires-Dist: google-api-python-client
+Requires-Dist: litellm
+Requires-Dist: numpy
+Requires-Dist: odfpy
+Requires-Dist: openai
+Requires-Dist: pydub
+Requires-Dist: pynput
+Requires-Dist: requests
+Requires-Dist: selenium
+Requires-Dist: sounddevice
+Requires-Dist: tiktoken
+
 
 # ipy_agent
 
 `ipy_agent` is a Python package that implements an AI agent designed to be integrated into any IPython shell (terminal, Jupyter notebook, QtConsole, etc.).
 
 ## Features
 
 - The agent captures all inputs and outputs occurring in the session to populate its context (up to token limit). 
 - Use magic commands `%ai` and `%%ai` to interact with the agent using natural language.
-- Hold `<ctrl>+<space>` to record and transcribe your voice into text inserted at cursor position. Useful to speak out your prompts instead of typing them. 
+- The assistant uses Whisper for multilingual voice synthesis.
+- Hold `<ctrl>+<space>` to record and transcribe your voice into text inserted at cursor position. Useful to speak out your prompts instead of typing them. Once active, it can be used wherever the cursor can go, not just in the notebook. (uses pynput for global keyboard hotkey detection. requires proper permissions to do so.)
 - The agent can autonomously execute Python code within the session.
 - Can be accessed as a declared object in the session, allowing configuration changes or method execution programmatically.
 - Can be used as a smart Python function returning any kind of data/object.
 - Supports various LLM providers and models via [litellm](https://www.litellm.ai/).
 - Integrated tools: The assistant can stream markdown with LaTeX support (in a notebook), talk to you using text to speech, create new code cells in notebooks, observe and extract content (folder, files, URL), introspect python entities (variables, functions, objects, classes, modules...), perform Google searches, perform semantic retrieval using a custom RAG document store (raw text or structured JSON), open files and urls in the browser, open files in a text editor, scrap the web and interact with webpages using a selenium webdriver...
 - Custom tools: you can extend the agent's functionalities by defining your own custom tools.
 
 ## Installation
 
 ```bash
-pip install ipy_agent
+pip install ipy-agent
 ```
 
-## Usage
+## Setup
 
 First, you need to set the API keys for your preferred LLM providers as environment variables.
 Refer to the [litellm](https://www.litellm.ai/) documentation to know the correct names for your environment variables to be recognized.
 
-Integration into the IPython session is as simple as:
+In case you want the agent to be able to use the websearch tool you will also need to setup a Google custom search engine and provide these two API keys:
+
+```bash
+GOOGLE_CUSTOM_SEARCH_API_KEY="..."
+GOOGLE_CUSTOM_SEARCH_CX="..."
+```
+
+These API keys can be placed in your .bashrc, directly in your python code via `os.environ` (not recommended), or provided via a .env file and loaded with python-dotenv for instance.
+
+## Usage
+
+Assuming your API keys are properly set up, integration into the IPython session (such as a Jupyter notebook) is as simple as running:
 
 ```python
 from ipy_agent import IPyAgent
 IPyAgent(name="Jarvis", username="Baptiste");
 ```
 
 Once loaded, the agent can be accessed in the namespace by the name you gave it in lowercase (`jarvis` in this case) and will respond to line and cell magics `%ai` and `%%ai` respectively. If no custom name is provided, the agent will be accessible by default as `agent`.
 
+Alternatively, you may run the command `ipy_agent` directly in the terminal. This will open a new terminal IPython session with the agent already loaded with default configuration. (Just be aware that voice dictation via `<ctrl>+<space>` tend to freeze the terminal IPython shell.)
+
+
 ### Configuration
 
 You can customize the agent by modifying its configuration. Here are some examples:
 
 ```python
 jarvis.config.model = "claude-3-opus-20240229"  # Use Claude-3 LLM model
 jarvis.config.temperature = 0.7  # Adjust the model temperature
@@ -67,15 +112,15 @@
 You can use the agent as a smart python function:
 
 ```python
 even_list = jarvis("Return a list of n even numbers", n=5)
 even_list # Output: [0, 2, 4, 6, 8]
 ```
 
-When doing so, the agent's markdown output will be silenced and only the result of computation will be returned.
+When doing so, the agent's markdown output will be silenced and only the result of computations will be returned.
 
 ### Available Tools
 
 The agent provides several built-in tools to ease various tasks. These tools are primarily intended for the agent's usage but can also be used by the user. Here is a list of available tools:
 
 - `agent.observe(source)` : Extracts information from a folder, file, URL, variable, function, class, or module, and injects it into the agent's context.
 - `agent.get_text(source)` : Extracts and returns text from a folder, file, URL, variable, function, class, or module.
```

### Comparing `ipy_agent-0.0.2/ipy_agent/default_preprompt.txt` & `ipy_agent-0.0.3/ipy_agent/default_preprompt.txt`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/dictation.py` & `ipy_agent-0.0.3/ipy_agent/dictation.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 from pydub import AudioSegment
 from pynput import keyboard
 from pynput.keyboard import Controller
 import logging
 from threading import Thread
 
 class AudioTranscriber:
-    def __init__(self, language='fr', model="whisper-1"):
+    def __init__(self, language='en', model="whisper-1"):
         self.client = OpenAI()
-        self.language = language
+        self._language=language
         self.model = model
 
+    @property
+    def language(self):
+        return self._language
+
     def transcribe(self, audio_data):
         try:
             audio_data.seek(0)
             transcript = self.client.audio.transcriptions.create(
                 model=self.model,
                 file=audio_data,
                 language=self.language
@@ -119,39 +123,47 @@
                 if not self.listener.is_alive():
                     self.listener = keyboard.Listener(on_press=self._on_press, on_release=self._on_release)
                     self.listener.start()
                 time.sleep(0.5)
         except KeyboardInterrupt:
             logging.info("Interruption par l'utilisateur.")
 
+class Dictation:
 
-def start_dictation():
+    def __init__(self,agent,hotkey="<ctrl>+<space>",model="whisper-1"):
 
-    def on_press():
-        audio_recorder.start_recording()
+        class Transcriber(AudioTranscriber):
+            @property
+            def language(self):
+                return agent.config.language
+        
+        self.audio_transcriber = Transcriber(model=model)
+        self.audio_recorder = AudioRecorder()
+        self.keyboard=Controller()
+        self.keyboard_listener = HotKeyListener()
+        self.keyboard_listener.bind(hotkey,on_press=self.on_press, on_release=self.on_release)
 
-    def on_release():
-        audio_recorder.stop_recording()
-        text = audio_transcriber.transcribe(audio_recorder.audio_data)
-        write_text(text)  # Simuler l'écriture du texte au niveau du curseur actif.
+    def on_press(self):
+        self.audio_recorder.start_recording()
 
-    def write_text(text):
-        keyboard = Controller()
+    def write_text(self,text):
         for char in text:
-            keyboard.press(char)
-            keyboard.release(char)
+            self.keyboard.press(char)
+            self.keyboard.release(char)
             time.sleep(0.005)
 
-    audio_transcriber = AudioTranscriber()
-    audio_recorder = AudioRecorder()
-    keyboard_listener = HotKeyListener()
-    keyboard_listener.bind("<ctrl>+<space>",on_press=on_press, on_release=on_release)
+    def on_release(self):
+        self.audio_recorder.stop_recording()
+        text = self.audio_transcriber.transcribe(self.audio_recorder.audio_data)
+        self.write_text(text)  # Simuler l'écriture du texte au niveau du curseur actif.
 
-    def listen():
+    def listen(self):
         try:
-            keyboard_listener.start()
+            self.keyboard_listener.start()
         except Exception as e:
             logging.error(f"Erreur lors de l'écoute du clavier : {e}")
 
-    listen_thread = Thread(target=listen)
-    listen_thread.daemon = True
-    listen_thread.start()
+    def start(self):
+        self.listen_thread = Thread(target=self.listen)
+        self.listen_thread.daemon = True
+        self.listen_thread.start()
+
```

### Comparing `ipy_agent-0.0.2/ipy_agent/get_text.py` & `ipy_agent-0.0.3/ipy_agent/get_text.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/get_webdriver.py` & `ipy_agent-0.0.3/ipy_agent/get_webdriver.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/google_search.py` & `ipy_agent-0.0.3/ipy_agent/google_search.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/init.py` & `ipy_agent-0.0.3/ipy_agent/init_shell.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from IPython.display import display, Markdown
 from IPython.core.magic import register_line_cell_magic
 from IPython import get_ipython
-from ipy_agent import start_dictation
 import os
                         
 def is_notebook():
     try:
         shell = get_ipython().__class__.__name__
         if shell == 'ZMQInteractiveShell':
             return True   # Jupyter notebook or qtconsole
@@ -46,12 +45,7 @@
 @register_line_cell_magic
 def ai(line, cell=''):
     if line:
         prompt=line+'\n'+cell
     else:
         prompt=cell
     get_ipython().user_ns['<<<self.instance_name>>>'](None,silent=False)
-
-start_dictation()
-
-
-
```

### Comparing `ipy_agent-0.0.2/ipy_agent/ipy_agent.py` & `ipy_agent-0.0.3/ipy_agent/ipy_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from IPython import get_ipython
 from IPython.terminal.interactiveshell import TerminalInteractiveShell
 from .llm_client import LLMClient
 from .attrdict import AttrDict
 import traceback
 from functools import wraps
 from .retrieval import DocumentStore
+from .dictation import Dictation
 from .msg_collector import MsgCollector,CollectIO
 from .tools import get_text, init_tools
 from .utils import root_join,Message,text_content,shell_type,truncate,pack_msgs,total_tokens,sort,extract_python,format
 from .voice import VoiceProcessor
 from textwrap import dedent
 import os
 
@@ -39,14 +40,16 @@
         self.current_name=self.username
         self.tools=AttrDict()
         self.init_workfolder(workfolder=workfolder)
         self.store=DocumentStore(folder=os.path.join(self.workfolder,"documents"))
         self.add_message(Message(content=preprompt or text_content(root_join("default_preprompt.txt")), role="system", name="Instructions", type="header"))
         self.init_shell(shell=shell)
         self.init_tools()
+        self.dictation=Dictation(self)
+        self.dictation.start()
 
     def __getattr__(self,attr):
         if attr in self.tools:
             return self.tools[attr]
         else:
             super().__getattribute__(attr)
 
@@ -60,15 +63,15 @@
 
         self.shell = shell or get_ipython() or TerminalInteractiveShell.instance()
 
         # Injecter l'agent dans l'espace de noms de la console
         self.shell.user_ns[self.instance_name] = self
 
         # Define the magic commands to call the assistant from the console/notebook
-        self.shell.run_cell(format(text_content(root_join("init.py")),context=locals()))
+        self.shell.run_cell(format(text_content(root_join("init_shell.py")),context=locals()))
 
         # Save the original run_cell method
         self.run_cell = self.shell.run_cell
         
         # Decorate it with input/output capture towards the assistant's message history
         @wraps(self.run_cell)
         def run_cell_with_capture(*args, **kwargs):
```

### Comparing `ipy_agent-0.0.2/ipy_agent/llm_client.py` & `ipy_agent-0.0.3/ipy_agent/llm_client.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/msg_collector.py` & `ipy_agent-0.0.3/ipy_agent/msg_collector.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/retrieval.py` & `ipy_agent-0.0.3/ipy_agent/retrieval.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/tools.py` & `ipy_agent-0.0.3/ipy_agent/tools.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/utils.py` & `ipy_agent-0.0.3/ipy_agent/utils.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent/voice.py` & `ipy_agent-0.0.3/ipy_agent/voice.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.2/ipy_agent.egg-info/PKG-INFO` & `ipy_agent-0.0.3/ipy_agent.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipy_agent
-Version: 0.0.2
+Version: 0.0.3
 Summary: An AI assistant designed to be integrated in an IPython shell.
 Home-page: https://github.com/B4PT0R/ipy_agent
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,42 +33,57 @@
 
 `ipy_agent` is a Python package that implements an AI agent designed to be integrated into any IPython shell (terminal, Jupyter notebook, QtConsole, etc.).
 
 ## Features
 
 - The agent captures all inputs and outputs occurring in the session to populate its context (up to token limit). 
 - Use magic commands `%ai` and `%%ai` to interact with the agent using natural language.
-- Hold `<ctrl>+<space>` to record and transcribe your voice into text inserted at cursor position. Useful to speak out your prompts instead of typing them. 
+- The assistant uses Whisper for multilingual voice synthesis.
+- Hold `<ctrl>+<space>` to record and transcribe your voice into text inserted at cursor position. Useful to speak out your prompts instead of typing them. Once active, it can be used wherever the cursor can go, not just in the notebook. (uses pynput for global keyboard hotkey detection. requires proper permissions to do so.)
 - The agent can autonomously execute Python code within the session.
 - Can be accessed as a declared object in the session, allowing configuration changes or method execution programmatically.
 - Can be used as a smart Python function returning any kind of data/object.
 - Supports various LLM providers and models via [litellm](https://www.litellm.ai/).
 - Integrated tools: The assistant can stream markdown with LaTeX support (in a notebook), talk to you using text to speech, create new code cells in notebooks, observe and extract content (folder, files, URL), introspect python entities (variables, functions, objects, classes, modules...), perform Google searches, perform semantic retrieval using a custom RAG document store (raw text or structured JSON), open files and urls in the browser, open files in a text editor, scrap the web and interact with webpages using a selenium webdriver...
 - Custom tools: you can extend the agent's functionalities by defining your own custom tools.
 
 ## Installation
 
 ```bash
-pip install ipy_agent
+pip install ipy-agent
 ```
 
-## Usage
+## Setup
 
 First, you need to set the API keys for your preferred LLM providers as environment variables.
 Refer to the [litellm](https://www.litellm.ai/) documentation to know the correct names for your environment variables to be recognized.
 
-Integration into the IPython session is as simple as:
+In case you want the agent to be able to use the websearch tool you will also need to setup a Google custom search engine and provide these two API keys:
+
+```bash
+GOOGLE_CUSTOM_SEARCH_API_KEY="..."
+GOOGLE_CUSTOM_SEARCH_CX="..."
+```
+
+These API keys can be placed in your .bashrc, directly in your python code via `os.environ` (not recommended), or provided via a .env file and loaded with python-dotenv for instance.
+
+## Usage
+
+Assuming your API keys are properly set up, integration into the IPython session (such as a Jupyter notebook) is as simple as running:
 
 ```python
 from ipy_agent import IPyAgent
 IPyAgent(name="Jarvis", username="Baptiste");
 ```
 
 Once loaded, the agent can be accessed in the namespace by the name you gave it in lowercase (`jarvis` in this case) and will respond to line and cell magics `%ai` and `%%ai` respectively. If no custom name is provided, the agent will be accessible by default as `agent`.
 
+Alternatively, you may run the command `ipy_agent` directly in the terminal. This will open a new terminal IPython session with the agent already loaded with default configuration. (Just be aware that voice dictation via `<ctrl>+<space>` tend to freeze the terminal IPython shell.)
+
+
 ### Configuration
 
 You can customize the agent by modifying its configuration. Here are some examples:
 
 ```python
 jarvis.config.model = "claude-3-opus-20240229"  # Use Claude-3 LLM model
 jarvis.config.temperature = 0.7  # Adjust the model temperature
@@ -97,15 +112,15 @@
 You can use the agent as a smart python function:
 
 ```python
 even_list = jarvis("Return a list of n even numbers", n=5)
 even_list # Output: [0, 2, 4, 6, 8]
 ```
 
-When doing so, the agent's markdown output will be silenced and only the result of computation will be returned.
+When doing so, the agent's markdown output will be silenced and only the result of computations will be returned.
 
 ### Available Tools
 
 The agent provides several built-in tools to ease various tasks. These tools are primarily intended for the agent's usage but can also be used by the user. Here is a list of available tools:
 
 - `agent.observe(source)` : Extracts information from a folder, file, URL, variable, function, class, or module, and injects it into the agent's context.
 - `agent.get_text(source)` : Extracts and returns text from a folder, file, URL, variable, function, class, or module.
```

### Comparing `ipy_agent-0.0.2/ipy_agent.egg-info/SOURCES.txt` & `ipy_agent-0.0.3/ipy_agent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ipy_agent/__init__.py
 ipy_agent/attrdict.py
 ipy_agent/default_preprompt.txt
 ipy_agent/dictation.py
 ipy_agent/get_text.py
 ipy_agent/get_webdriver.py
 ipy_agent/google_search.py
-ipy_agent/init.py
+ipy_agent/init_shell.py
 ipy_agent/ipy_agent.py
 ipy_agent/llm_client.py
 ipy_agent/main.py
 ipy_agent/msg_collector.py
 ipy_agent/retrieval.py
 ipy_agent/tools.py
 ipy_agent/utils.py
```

### Comparing `ipy_agent-0.0.2/setup.py` & `ipy_agent-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipy_agent",
-    version="0.0.2",
+    version="0.0.3",
     author="Baptiste Ferrand",
     author_email="bferrand.maths@gmail.com",
     description="An AI assistant designed to be integrated in an IPython shell.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/B4PT0R/ipy_agent",
     packages=setuptools.find_packages(),
         package_data={
         'ipy_agent': [
             'default_preprompt.txt',
-            'init.py'
+            'init_shell.py'
         ]
     },
     entry_points={
         'console_scripts': [
             'ipy_agent=ipy_agent.main:main',
         ],
     },
```

