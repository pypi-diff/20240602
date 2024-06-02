# Comparing `tmp/blaze_double_bot-1.2.0.tar.gz` & `tmp/blaze_double_bot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze_double_bot-1.2.0.tar", last modified: Sat Jun  1 19:27:15 2024, max compression
+gzip compressed data, was "blaze_double_bot-1.3.0.tar", last modified: Sat Jun  1 19:52:04 2024, max compression
```

## Comparing `blaze_double_bot-1.2.0.tar` & `blaze_double_bot-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 19:27:15.688366 blaze_double_bot-1.2.0/
--rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3573 2024-06-01 19:27:15.688366 blaze_double_bot-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3076 2024-05-27 01:18:02.000000 blaze_double_bot-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 19:27:15.549345 blaze_double_bot-1.2.0/blaze_double_bot/
--rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-1.2.0/blaze_double_bot/__init__.py
--rw-rw-rw-   0        0        0    12559 2024-06-01 17:19:47.000000 blaze_double_bot-1.2.0/blaze_double_bot/bot.py
-drwxrwxrwx   0        0        0        0 2024-06-01 19:27:15.683118 blaze_double_bot-1.2.0/blaze_double_bot.egg-info/
--rw-rw-rw-   0        0        0     3573 2024-06-01 19:27:12.000000 blaze_double_bot-1.2.0/blaze_double_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-06-01 19:27:13.000000 blaze_double_bot-1.2.0/blaze_double_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 19:27:12.000000 blaze_double_bot-1.2.0/blaze_double_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 19:27:12.000000 blaze_double_bot-1.2.0/blaze_double_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-06-01 19:27:12.000000 blaze_double_bot-1.2.0/blaze_double_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 19:27:15.694097 blaze_double_bot-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-06-01 19:26:00.000000 blaze_double_bot-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:52:04.141352 blaze_double_bot-1.3.0/
+-rw-rw-rw-   0        0        0     1071 2024-05-22 17:31:42.000000 blaze_double_bot-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3573 2024-06-01 19:52:04.139550 blaze_double_bot-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3076 2024-05-27 01:18:02.000000 blaze_double_bot-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 19:52:04.056646 blaze_double_bot-1.3.0/blaze_double_bot/
+-rw-rw-rw-   0        0        0       20 2024-05-23 00:00:30.000000 blaze_double_bot-1.3.0/blaze_double_bot/__init__.py
+-rw-rw-rw-   0        0        0    12559 2024-06-01 17:19:47.000000 blaze_double_bot-1.3.0/blaze_double_bot/bot.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:52:04.136633 blaze_double_bot-1.3.0/blaze_double_bot.egg-info/
+-rw-rw-rw-   0        0        0     3573 2024-06-01 19:52:03.000000 blaze_double_bot-1.3.0/blaze_double_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-06-01 19:52:03.000000 blaze_double_bot-1.3.0/blaze_double_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 19:52:03.000000 blaze_double_bot-1.3.0/blaze_double_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 19:52:03.000000 blaze_double_bot-1.3.0/blaze_double_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-06-01 19:52:03.000000 blaze_double_bot-1.3.0/blaze_double_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 19:52:04.142691 blaze_double_bot-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-06-01 19:50:59.000000 blaze_double_bot-1.3.0/setup.py
```

### Comparing `blaze_double_bot-1.2.0/LICENSE` & `blaze_double_bot-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-1.2.0/PKG-INFO` & `blaze_double_bot-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 1.2.0
+Version: 1.3.0
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-1.2.0/README.md` & `blaze_double_bot-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-1.2.0/blaze_double_bot/bot.py` & `blaze_double_bot-1.3.0/blaze_double_bot/bot.py`

 * *Files identical despite different names*

### Comparing `blaze_double_bot-1.2.0/blaze_double_bot.egg-info/PKG-INFO` & `blaze_double_bot-1.3.0/blaze_double_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaze_double_bot
-Version: 1.2.0
+Version: 1.3.0
 Summary: This Python library automates the betting process on the Blaze Double
 Author: ror74559
 Author-email: ror74559@gmail.com
 License: MIT License
 Keywords: blaze double bot
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `blaze_double_bot-1.2.0/setup.py` & `blaze_double_bot-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
           readme =f.read()
 
 setup(
     name='blaze_double_bot',
     licence='MIT License',
-    version='1.2.0',
+    version='1.3.0',
     author='ror74559',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='ror74559@gmail.com',
     keywords='blaze double bot',
     description='This Python library automates the betting process on the Blaze Double',
     packages=['blaze_double_bot'],
```

