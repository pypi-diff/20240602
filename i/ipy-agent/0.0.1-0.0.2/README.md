# Comparing `tmp/ipy_agent-0.0.1.tar.gz` & `tmp/ipy_agent-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipy_agent-0.0.1.tar", last modified: Sun Jun  2 15:05:19 2024, max compression
+gzip compressed data, was "ipy_agent-0.0.2.tar", last modified: Sun Jun  2 15:09:22 2024, max compression
```

## Comparing `ipy_agent-0.0.1.tar` & `ipy_agent-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:05:19.659227 ipy_agent-0.0.1/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-01-22 21:52:29.000000 ipy_agent-0.0.1/LICENSE
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       33 2023-12-26 15:28:37.000000 ipy_agent-0.0.1/MANIFEST.in
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     6091 2024-06-02 15:05:19.659227 ipy_agent-0.0.1/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5222 2024-06-02 14:55:10.000000 ipy_agent-0.0.1/README.md
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:05:19.655227 ipy_agent-0.0.1/ipy_agent/
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       70 2024-06-02 12:32:54.000000 ipy_agent-0.0.1/ipy_agent/__init__.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      451 2024-03-13 10:59:26.000000 ipy_agent-0.0.1/ipy_agent/attrdict.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     4252 2024-06-02 13:57:26.000000 ipy_agent-0.0.1/ipy_agent/default_preprompt.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5059 2024-06-02 12:58:18.000000 ipy_agent-0.0.1/ipy_agent/dictation.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    12399 2024-05-25 20:09:35.000000 ipy_agent-0.0.1/ipy_agent/get_text.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1562 2024-05-25 20:09:53.000000 ipy_agent-0.0.1/ipy_agent/get_webdriver.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1802 2024-05-25 20:13:46.000000 ipy_agent-0.0.1/ipy_agent/google_search.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1878 2024-06-02 13:50:04.000000 ipy_agent-0.0.1/ipy_agent/init.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     9662 2024-06-02 14:07:07.000000 ipy_agent-0.0.1/ipy_agent/ipy_agent.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1262 2024-05-28 20:11:19.000000 ipy_agent-0.0.1/ipy_agent/llm_client.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       69 2024-06-02 13:32:03.000000 ipy_agent-0.0.1/ipy_agent/main.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     2161 2024-06-02 13:30:07.000000 ipy_agent-0.0.1/ipy_agent/msg_collector.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    16537 2024-05-30 17:55:58.000000 ipy_agent-0.0.1/ipy_agent/retrieval.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    10371 2024-05-29 20:28:02.000000 ipy_agent-0.0.1/ipy_agent/tools.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3070 2024-05-30 18:01:36.000000 ipy_agent-0.0.1/ipy_agent/utils.py
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5483 2024-06-02 09:46:31.000000 ipy_agent-0.0.1/ipy_agent/voice.py
-drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:05:19.659227 ipy_agent-0.0.1/ipy_agent.egg-info/
--rw-r--r--   0 baptiste  (1000) baptiste  (1000)     6091 2024-06-02 15:05:19.000000 ipy_agent-0.0.1/ipy_agent.egg-info/PKG-INFO
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      603 2024-06-02 15:05:19.000000 ipy_agent-0.0.1/ipy_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-06-02 15:05:19.000000 ipy_agent-0.0.1/ipy_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       50 2024-06-02 15:05:19.000000 ipy_agent-0.0.1/ipy_agent.egg-info/entry_points.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      161 2024-06-02 15:05:19.000000 ipy_agent-0.0.1/ipy_agent.egg-info/requires.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       10 2024-06-02 15:05:19.000000 ipy_agent-0.0.1/ipy_agent.egg-info/top_level.txt
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-06-02 15:05:19.659227 ipy_agent-0.0.1/setup.cfg
--rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1283 2024-06-02 14:55:39.000000 ipy_agent-0.0.1/setup.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1073 2024-01-22 21:52:29.000000 ipy_agent-0.0.2/LICENSE
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       33 2023-12-26 15:28:37.000000 ipy_agent-0.0.2/MANIFEST.in
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     6093 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5222 2024-06-02 14:55:10.000000 ipy_agent-0.0.2/README.md
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/ipy_agent/
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       70 2024-06-02 12:32:54.000000 ipy_agent-0.0.2/ipy_agent/__init__.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      451 2024-03-13 10:59:26.000000 ipy_agent-0.0.2/ipy_agent/attrdict.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     4252 2024-06-02 13:57:26.000000 ipy_agent-0.0.2/ipy_agent/default_preprompt.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5059 2024-06-02 12:58:18.000000 ipy_agent-0.0.2/ipy_agent/dictation.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    12399 2024-05-25 20:09:35.000000 ipy_agent-0.0.2/ipy_agent/get_text.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1562 2024-05-25 20:09:53.000000 ipy_agent-0.0.2/ipy_agent/get_webdriver.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1802 2024-05-25 20:13:46.000000 ipy_agent-0.0.2/ipy_agent/google_search.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1878 2024-06-02 13:50:04.000000 ipy_agent-0.0.2/ipy_agent/init.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     9662 2024-06-02 14:07:07.000000 ipy_agent-0.0.2/ipy_agent/ipy_agent.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1262 2024-05-28 20:11:19.000000 ipy_agent-0.0.2/ipy_agent/llm_client.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       69 2024-06-02 13:32:03.000000 ipy_agent-0.0.2/ipy_agent/main.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     2161 2024-06-02 13:30:07.000000 ipy_agent-0.0.2/ipy_agent/msg_collector.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    16537 2024-05-30 17:55:58.000000 ipy_agent-0.0.2/ipy_agent/retrieval.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)    10371 2024-05-29 20:28:02.000000 ipy_agent-0.0.2/ipy_agent/tools.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     3070 2024-05-30 18:01:36.000000 ipy_agent-0.0.2/ipy_agent/utils.py
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     5483 2024-06-02 09:46:31.000000 ipy_agent-0.0.2/ipy_agent/voice.py
+drwxrwxr-x   0 baptiste  (1000) baptiste  (1000)        0 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/ipy_agent.egg-info/
+-rw-r--r--   0 baptiste  (1000) baptiste  (1000)     6093 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      603 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)        1 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       50 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)      163 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/requires.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       10 2024-06-02 15:09:21.000000 ipy_agent-0.0.2/ipy_agent.egg-info/top_level.txt
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)       38 2024-06-02 15:09:22.033529 ipy_agent-0.0.2/setup.cfg
+-rw-rw-r--   0 baptiste  (1000) baptiste  (1000)     1285 2024-06-02 15:09:08.000000 ipy_agent-0.0.2/setup.py
```

### Comparing `ipy_agent-0.0.1/LICENSE` & `ipy_agent-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/PKG-INFO` & `ipy_agent-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipy_agent
-Version: 0.0.1
+Version: 0.0.2
 Summary: An AI assistant designed to be integrated in an IPython shell.
 Home-page: https://github.com/B4PT0R/ipy_agent
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: PyPDF2
 Requires-Dist: beautifulsoup4
 Requires-Dist: python-docx
 Requires-Dist: get-gecko-driver
 Requires-Dist: google-api-python-client
 Requires-Dist: litellm
 Requires-Dist: numpy
-Requires-Dist: odf
+Requires-Dist: odfpy
 Requires-Dist: openai
 Requires-Dist: pydub
 Requires-Dist: pynput
 Requires-Dist: requests
 Requires-Dist: selenium
 Requires-Dist: sounddevice
 Requires-Dist: tiktoken
```

### Comparing `ipy_agent-0.0.1/README.md` & `ipy_agent-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/default_preprompt.txt` & `ipy_agent-0.0.2/ipy_agent/default_preprompt.txt`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/dictation.py` & `ipy_agent-0.0.2/ipy_agent/dictation.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/get_text.py` & `ipy_agent-0.0.2/ipy_agent/get_text.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/get_webdriver.py` & `ipy_agent-0.0.2/ipy_agent/get_webdriver.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/google_search.py` & `ipy_agent-0.0.2/ipy_agent/google_search.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/init.py` & `ipy_agent-0.0.2/ipy_agent/init.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/ipy_agent.py` & `ipy_agent-0.0.2/ipy_agent/ipy_agent.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/llm_client.py` & `ipy_agent-0.0.2/ipy_agent/llm_client.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/msg_collector.py` & `ipy_agent-0.0.2/ipy_agent/msg_collector.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/retrieval.py` & `ipy_agent-0.0.2/ipy_agent/retrieval.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/tools.py` & `ipy_agent-0.0.2/ipy_agent/tools.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/utils.py` & `ipy_agent-0.0.2/ipy_agent/utils.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent/voice.py` & `ipy_agent-0.0.2/ipy_agent/voice.py`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/ipy_agent.egg-info/PKG-INFO` & `ipy_agent-0.0.2/ipy_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipy_agent
-Version: 0.0.1
+Version: 0.0.2
 Summary: An AI assistant designed to be integrated in an IPython shell.
 Home-page: https://github.com/B4PT0R/ipy_agent
 Author: Baptiste Ferrand
 Author-email: bferrand.maths@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: PyPDF2
 Requires-Dist: beautifulsoup4
 Requires-Dist: python-docx
 Requires-Dist: get-gecko-driver
 Requires-Dist: google-api-python-client
 Requires-Dist: litellm
 Requires-Dist: numpy
-Requires-Dist: odf
+Requires-Dist: odfpy
 Requires-Dist: openai
 Requires-Dist: pydub
 Requires-Dist: pynput
 Requires-Dist: requests
 Requires-Dist: selenium
 Requires-Dist: sounddevice
 Requires-Dist: tiktoken
```

### Comparing `ipy_agent-0.0.1/ipy_agent.egg-info/SOURCES.txt` & `ipy_agent-0.0.2/ipy_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipy_agent-0.0.1/setup.py` & `ipy_agent-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ipy_agent",
-    version="0.0.1",
+    version="0.0.2",
     author="Baptiste Ferrand",
     author_email="bferrand.maths@gmail.com",
     description="An AI assistant designed to be integrated in an IPython shell.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/B4PT0R/ipy_agent",
     packages=setuptools.find_packages(),
@@ -34,15 +34,15 @@
         "PyPDF2",
         "beautifulsoup4",
         "python-docx",
         "get-gecko-driver",
         "google-api-python-client",
         "litellm",
         "numpy",
-        "odf",
+        "odfpy",
         "openai",
         "pydub",
         "pynput",
         "requests",
         "selenium",
         "sounddevice",
         "tiktoken"
```

