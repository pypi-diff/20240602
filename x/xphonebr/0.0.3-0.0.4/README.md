# Comparing `tmp/xphonebr-0.0.3.tar.gz` & `tmp/xphonebr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xphonebr-0.0.3.tar", last modified: Fri May 31 10:44:54 2024, max compression
+gzip compressed data, was "xphonebr-0.0.4.tar", last modified: Sun Jun  2 10:50:31 2024, max compression
```

## Comparing `xphonebr-0.0.3.tar` & `xphonebr-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:44:54.762578 xphonebr-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 10:44:38.000000 xphonebr-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 10:44:54.762578 xphonebr-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-31 10:44:38.000000 xphonebr-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 10:44:54.766578 xphonebr-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-31 10:44:38.000000 xphonebr-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:44:54.762578 xphonebr-0.0.3/xphonebr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:44:54.762578 xphonebr-0.0.3/xphonebr/Util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:44:38.000000 xphonebr-0.0.3/xphonebr/Util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-31 10:44:38.000000 xphonebr-0.0.3/xphonebr/Util/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-31 10:44:38.000000 xphonebr-0.0.3/xphonebr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:44:54.762578 xphonebr-0.0.3/xphonebr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 10:44:54.000000 xphonebr-0.0.3/xphonebr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 10:44:54.000000 xphonebr-0.0.3/xphonebr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:44:54.000000 xphonebr-0.0.3/xphonebr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 10:44:54.000000 xphonebr-0.0.3/xphonebr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 10:44:54.000000 xphonebr-0.0.3/xphonebr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:50:31.435985 xphonebr-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 10:50:19.000000 xphonebr-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-02 10:50:31.435985 xphonebr-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-06-02 10:50:19.000000 xphonebr-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 10:50:31.435985 xphonebr-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-02 10:50:19.000000 xphonebr-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:50:31.435985 xphonebr-0.0.4/xphonebr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:50:31.435985 xphonebr-0.0.4/xphonebr/Util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:50:19.000000 xphonebr-0.0.4/xphonebr/Util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-06-02 10:50:19.000000 xphonebr-0.0.4/xphonebr/Util/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-06-02 10:50:19.000000 xphonebr-0.0.4/xphonebr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:50:31.435985 xphonebr-0.0.4/xphonebr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-02 10:50:31.000000 xphonebr-0.0.4/xphonebr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-06-02 10:50:31.000000 xphonebr-0.0.4/xphonebr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:50:31.000000 xphonebr-0.0.4/xphonebr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-02 10:50:31.000000 xphonebr-0.0.4/xphonebr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 10:50:31.000000 xphonebr-0.0.4/xphonebr.egg-info/top_level.txt
```

### Comparing `xphonebr-0.0.3/LICENSE` & `xphonebr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xphonebr-0.0.3/PKG-INFO` & `xphonebr-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xphonebr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Grapheme to phoneme conversion and tools for tts with deep learning.
 Author: Emerson Pedroso
 Author-email: traderpedroso@icloud.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `xphonebr-0.0.3/README.md` & `xphonebr-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xphonebr-0.0.3/setup.py` & `xphonebr-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 long_description = """XphoneBR is a portuguese transformer base grapheme-to-phoneme normalization  tool modeling library that leverages recent deep learning 
 technology and is optimized for usage in production systems such as TTS. In particular, the library should
 be accurate, fast, easy to use. 
 
 DeepPhonemizerBR is compatible with Python 3.6+ and is distributed under the MIT license.
 
 """
-# Version: 0.0.3
+# Version: 0.0.4
 setup(
     name="xphonebr",
-    version="0.0.3",
+    version="0.0.4",
     author="Emerson Pedroso",
     author_email="traderpedroso@icloud.com",
     description="Grapheme to phoneme conversion and tools for tts with deep learning.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="MIT",
     install_requires=[
```

### Comparing `xphonebr-0.0.3/xphonebr/Util/norm.py` & `xphonebr-0.0.4/xphonebr/Util/norm.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "「": "'",
     "」": "'",
     "& ": " e ",
 }
 
 # Lista de pares (expressão regular, substituição) para abreviações em português do Brasil:
 abbreviations = [
-    (re.compile(r"\b%s\b" % x[0], re.IGNORECASE), x[1])
+    (re.compile(r"\b%s\b" % re.escape(x[0]), re.IGNORECASE), x[1])
     for x in [
         ("sr", "senhor"),
         ("sra", "senhora"),
         ("dr", "doutor"),
         ("dra", "doutora"),
         ("prof", "professor"),
         ("eng", "engenheiro"),
@@ -155,16 +155,16 @@
 
 
 def _normalize_numbers(text):
     return re.sub(r"\b\d+\b", lambda x: num2words(x.group(), lang="pt"), text)
 
 
 def _normalize_abbreviations(text):
-    for regex, substitutions in abbreviations:
-        text = re.sub(regex, substitutions, text)
+    for regex, substitution in abbreviations:
+        text = regex.sub(substitution, text)
     return text
 
 
 def _normalize_am_pm_times(text):
     def am_pm_to_words(match):
         hours = int(match.group(1))
         period = match.group(2).lower()
```

### Comparing `xphonebr-0.0.3/xphonebr/__init__.py` & `xphonebr-0.0.4/xphonebr/__init__.py`

 * *Files identical despite different names*

### Comparing `xphonebr-0.0.3/xphonebr.egg-info/PKG-INFO` & `xphonebr-0.0.4/xphonebr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xphonebr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Grapheme to phoneme conversion and tools for tts with deep learning.
 Author: Emerson Pedroso
 Author-email: traderpedroso@icloud.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

