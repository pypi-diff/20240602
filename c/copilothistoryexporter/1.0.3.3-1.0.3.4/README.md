# Comparing `tmp/copilothistoryexporter-1.0.3.3.tar.gz` & `tmp/copilothistoryexporter-1.0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.3.3.tar", last modified: Sun Jun  2 20:07:34 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.3.4.tar", last modified: Sun Jun  2 20:14:56 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.3.3.tar` & `copilothistoryexporter-1.0.3.4.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:07:34.400203 copilothistoryexporter-1.0.3.3/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.3/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:07:34.400040 copilothistoryexporter-1.0.3.3/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.3/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:07:34.399872 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      255 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:07:34.400238 copilothistoryexporter-1.0.3.3/setup.cfg
--rw-r--r--   0 mustafakilic   (501) staff       (20)      621 2024-06-02 20:07:31.000000 copilothistoryexporter-1.0.3.3/setup.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.764211 copilothistoryexporter-1.0.3.4/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.4/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:14:56.764031 copilothistoryexporter-1.0.3.4/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.4/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.763848 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      449 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:14:56.764263 copilothistoryexporter-1.0.3.4/setup.cfg
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      759 2024-06-02 20:14:28.000000 copilothistoryexporter-1.0.3.4/setup.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.762063 copilothistoryexporter-1.0.3.4/src/
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.763696 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:13:11.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/__init.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1136 2024-06-02 19:54:24.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/main.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/sample.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2359 2024-06-02 19:54:24.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/utils.py
```

### Comparing `copilothistoryexporter-1.0.3.3/LICENCE` & `copilothistoryexporter-1.0.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.3/README.md` & `copilothistoryexporter-1.0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.3/setup.py` & `copilothistoryexporter-1.0.3.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
-
 from setuptools import setup, find_packages
 
-
 setup(
-
     name="copilothistoryexporter",
-    version='1.0.3.3',
+    version='1.0.3.4',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kilic',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
     packages=find_packages(),
     package_data={'': ['*.md']},
     install_requires=[
         "requests",
         "click",
         "mitmproxy",
         "wheel",
         "setuptools",
     ],
+    entry_points={
+        'console_scripts': [
+            'copilothistoryexporter = src.copilothistoryexporter.main:main'
+        ]
+    },
 )
```

