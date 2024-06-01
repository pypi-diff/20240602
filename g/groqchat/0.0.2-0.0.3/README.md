# Comparing `tmp/groqchat-0.0.2.tar.gz` & `tmp/groqchat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqchat-0.0.2.tar", last modified: Fri May 31 11:33:46 2024, max compression
+gzip compressed data, was "groqchat-0.0.3.tar", last modified: Sat Jun  1 22:06:00 2024, max compression
```

## Comparing `groqchat-0.0.2.tar` & `groqchat-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-31 11:33:46.374345 groqchat-0.0.2/
--rw-r--r--   0 admin      (501) staff       (20)     3041 2024-05-31 11:33:46.374240 groqchat-0.0.2/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-31 11:33:46.372872 groqchat-0.0.2/groqchat/
--rw-r--r--   0 admin      (501) staff       (20)     1938 2024-05-31 11:33:46.000000 groqchat-0.0.2/groqchat/README.md
--rw-r--r--   0 admin      (501) staff       (20)     2853 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      931 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/config.py
--rw-r--r--   0 admin      (501) staff       (20)    12501 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/main.py
--rw-r--r--   0 admin      (501) staff       (20)       19 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/requirements.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-31 11:33:46.374065 groqchat-0.0.2/groqchat/utils/
--rw-r--r--   0 admin      (501) staff       (20)     1548 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/utils/promptValidator.py
--rw-r--r--   0 admin      (501) staff       (20)     2757 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/utils/single_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)     7378 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/utils/streaming_word_wrapper.py
--rw-r--r--   0 admin      (501) staff       (20)     4779 2024-05-31 10:05:10.000000 groqchat-0.0.2/groqchat/utils/terminal_mode_dialogs.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-31 11:33:46.373548 groqchat-0.0.2/groqchat.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     3041 2024-05-31 11:33:46.000000 groqchat-0.0.2/groqchat.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      451 2024-05-31 11:33:46.000000 groqchat-0.0.2/groqchat.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-31 11:33:46.000000 groqchat-0.0.2/groqchat.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       45 2024-05-31 11:33:46.000000 groqchat-0.0.2/groqchat.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)       20 2024-05-31 11:33:46.000000 groqchat-0.0.2/groqchat.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        9 2024-05-31 11:33:46.000000 groqchat-0.0.2/groqchat.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-31 11:33:46.374389 groqchat-0.0.2/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     2708 2024-05-31 11:33:41.000000 groqchat-0.0.2/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-06-01 22:06:00.869559 groqchat-0.0.3/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3041 2024-06-01 22:06:00.869559 groqchat-0.0.3/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-06-01 22:06:00.865559 groqchat-0.0.3/groqchat/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1938 2024-06-01 22:06:00.000000 groqchat-0.0.3/groqchat/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2853 2024-06-01 21:59:38.000000 groqchat-0.0.3/groqchat/__init__.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      931 2024-06-01 21:59:38.000000 groqchat-0.0.3/groqchat/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    12535 2024-06-01 22:04:17.000000 groqchat-0.0.3/groqchat/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       19 2024-06-01 21:59:38.000000 groqchat-0.0.3/groqchat/requirements.txt
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-06-01 22:06:00.869559 groqchat-0.0.3/groqchat/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1548 2024-06-01 21:59:38.000000 groqchat-0.0.3/groqchat/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2757 2024-06-01 21:59:38.000000 groqchat-0.0.3/groqchat/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7378 2024-06-01 21:59:38.000000 groqchat-0.0.3/groqchat/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4779 2024-06-01 21:59:38.000000 groqchat-0.0.3/groqchat/utils/terminal_mode_dialogs.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-06-01 22:06:00.865559 groqchat-0.0.3/groqchat.egg-info/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3041 2024-06-01 22:06:00.000000 groqchat-0.0.3/groqchat.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      451 2024-06-01 22:06:00.000000 groqchat-0.0.3/groqchat.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-06-01 22:06:00.000000 groqchat-0.0.3/groqchat.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       45 2024-06-01 22:06:00.000000 groqchat-0.0.3/groqchat.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       20 2024-06-01 22:06:00.000000 groqchat-0.0.3/groqchat.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        9 2024-06-01 22:06:00.000000 groqchat-0.0.3/groqchat.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-06-01 22:06:00.869559 groqchat-0.0.3/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2708 2024-06-01 22:04:46.000000 groqchat-0.0.3/setup.py
```

### Comparing `groqchat-0.0.2/PKG-INFO` & `groqchat-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groqchat
-Version: 0.0.2
+Version: 0.0.3
 Summary: A terminal chatbot, powered by Groq Cloud API (Windows / macOS / Linux / Android / iOS)
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/groqchat
 Project-URL: Tracker, https://github.com/eliranwong/groqchat/issues
```

### Comparing `groqchat-0.0.2/groqchat/README.md` & `groqchat-0.0.3/groqchat/README.md`

 * *Files identical despite different names*

### Comparing `groqchat-0.0.2/groqchat/__init__.py` & `groqchat-0.0.3/groqchat/__init__.py`

 * *Files identical despite different names*

### Comparing `groqchat-0.0.2/groqchat/config.py` & `groqchat-0.0.3/groqchat/config.py`

 * *Files identical despite different names*

### Comparing `groqchat-0.0.2/groqchat/main.py` & `groqchat-0.0.3/groqchat/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
     def resetMessages(self):
         return [{"role": "system", "content": config.systemMessage_groq},]
 
     def changeGroqApi(self):
         print3("# Groq Cloud API Key: allows access to Groq Cloud hosted LLMs")
         print1("To set up Groq Cloud API Key, read:\nhttps://github.com/eliranwong/freegenius/wiki/Set-up-a-Groq-Cloud-API-Key\n")
-        print1("Enter your Groq Cloud API Key:")
+        print1("Enter a single or a list of multiple Groq Cloud API Key(s):")
         print()
-        apikey = SinglePrompt.run(style=self.promptStyle, default=config.groqApi_key, is_password=True)
+        apikey = SinglePrompt.run(style=self.promptStyle, default=str(config.groqApi_key), is_password=True)
         if apikey and not apikey.strip().lower() in (config.cancel_entry, config.exit_entry):
             try:
                 if isinstance(eval(apikey), list):
                     config.groqApi_key = eval(apikey)
             except:
                 config.groqApi_key = apikey
         saveConfig()
```

### Comparing `groqchat-0.0.2/groqchat/utils/promptValidator.py` & `groqchat-0.0.3/groqchat/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `groqchat-0.0.2/groqchat/utils/single_prompt.py` & `groqchat-0.0.3/groqchat/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `groqchat-0.0.2/groqchat/utils/streaming_word_wrapper.py` & `groqchat-0.0.3/groqchat/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `groqchat-0.0.2/groqchat/utils/terminal_mode_dialogs.py` & `groqchat-0.0.3/groqchat/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `groqchat-0.0.2/groqchat.egg-info/PKG-INFO` & `groqchat-0.0.3/groqchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groqchat
-Version: 0.0.2
+Version: 0.0.3
 Summary: A terminal chatbot, powered by Groq Cloud API (Windows / macOS / Linux / Android / iOS)
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/groqchat
 Project-URL: Tracker, https://github.com/eliranwong/groqchat/issues
```

### Comparing `groqchat-0.0.2/setup.py` & `groqchat-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         mod = line.strip()
         if mod:
             install_requires.append(mod)
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.2",
+    version="0.0.3",
     python_requires=">=3.8",
     description="A terminal chatbot, powered by Groq Cloud API (Windows / macOS / Linux / Android / iOS)",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     packages=[
         package,
```

