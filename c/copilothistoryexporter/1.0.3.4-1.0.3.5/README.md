# Comparing `tmp/copilothistoryexporter-1.0.3.4.tar.gz` & `tmp/copilothistoryexporter-1.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.3.4.tar", last modified: Sun Jun  2 20:14:56 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.3.5.tar", last modified: Sun Jun  2 20:22:06 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.3.4.tar` & `copilothistoryexporter-1.0.3.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.764211 copilothistoryexporter-1.0.3.4/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.4/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:14:56.764031 copilothistoryexporter-1.0.3.4/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.4/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.763848 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      449 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:14:56.000000 copilothistoryexporter-1.0.3.4/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:14:56.764263 copilothistoryexporter-1.0.3.4/setup.cfg
--rw-r--r--   0 mustafakilic   (501) staff       (20)      759 2024-06-02 20:14:28.000000 copilothistoryexporter-1.0.3.4/setup.py
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.762063 copilothistoryexporter-1.0.3.4/src/
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:14:56.763696 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/
--rw-r--r--   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:13:11.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/__init.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1136 2024-06-02 19:54:24.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/main.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/sample.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2359 2024-06-02 19:54:24.000000 copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/utils.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.754324 copilothistoryexporter-1.0.3.5/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.5/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:22:06.754129 copilothistoryexporter-1.0.3.5/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.5/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.753932 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      412 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:22:06.000000 copilothistoryexporter-1.0.3.5/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:22:06.754360 copilothistoryexporter-1.0.3.5/setup.cfg
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      759 2024-06-02 20:21:54.000000 copilothistoryexporter-1.0.3.5/setup.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.752344 copilothistoryexporter-1.0.3.5/src/
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:22:06.753766 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      768 2024-06-02 20:19:26.000000 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/main.py
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       92 2024-06-02 16:13:00.000000 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/sample.md
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2359 2024-06-02 19:54:24.000000 copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/utils.py
```

### Comparing `copilothistoryexporter-1.0.3.4/LICENCE` & `copilothistoryexporter-1.0.3.5/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.4/README.md` & `copilothistoryexporter-1.0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.4/setup.py` & `copilothistoryexporter-1.0.3.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
+
 from setuptools import setup, find_packages
 
 setup(
     name="copilothistoryexporter",
-    version='1.0.3.4',
+    version='1.0.3.5',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kilic',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
     packages=find_packages(),
     package_data={'': ['*.md']},
@@ -16,12 +17,11 @@
         "click",
         "mitmproxy",
         "wheel",
         "setuptools",
     ],
     entry_points={
         'console_scripts': [
-            'copilothistoryexporter = src.copilothistoryexporter.main:main'
+            'copilothistoryexporter = copilothistoryexporter.__main__:main'
         ]
     },
 )
-
```

### Comparing `copilothistoryexporter-1.0.3.4/src/copilothistoryexporter/utils.py` & `copilothistoryexporter-1.0.3.5/src/copilothistoryexporter/utils.py`

 * *Files identical despite different names*

