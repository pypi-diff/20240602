# Comparing `tmp/copilothistoryexporter-1.0.3.1.tar.gz` & `tmp/copilothistoryexporter-1.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.3.1.tar", last modified: Sun Jun  2 19:57:19 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.3.2.tar", last modified: Sun Jun  2 20:01:31 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.3.1.tar` & `copilothistoryexporter-1.0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 19:57:19.697013 copilothistoryexporter-1.0.3.1/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.1/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 19:57:19.696843 copilothistoryexporter-1.0.3.1/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.1/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 19:57:19.696669 copilothistoryexporter-1.0.3.1/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 19:57:19.000000 copilothistoryexporter-1.0.3.1/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      304 2024-06-02 19:57:19.000000 copilothistoryexporter-1.0.3.1/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 19:57:19.000000 copilothistoryexporter-1.0.3.1/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       80 2024-06-02 19:57:19.000000 copilothistoryexporter-1.0.3.1/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 19:57:19.000000 copilothistoryexporter-1.0.3.1/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 19:57:19.000000 copilothistoryexporter-1.0.3.1/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 19:57:19.697048 copilothistoryexporter-1.0.3.1/setup.cfg
--rw-r--r--   0 mustafakilic   (501) staff       (20)      762 2024-06-02 19:55:56.000000 copilothistoryexporter-1.0.3.1/setup.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:01:31.080665 copilothistoryexporter-1.0.3.2/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.2/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:01:31.080499 copilothistoryexporter-1.0.3.2/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.2/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:01:31.080338 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      304 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       57 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:01:31.080698 copilothistoryexporter-1.0.3.2/setup.cfg
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      739 2024-06-02 20:01:21.000000 copilothistoryexporter-1.0.3.2/setup.py
```

### Comparing `copilothistoryexporter-1.0.3.1/LICENCE` & `copilothistoryexporter-1.0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.1/README.md` & `copilothistoryexporter-1.0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.1/setup.py` & `copilothistoryexporter-1.0.3.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
 
     name="copilothistoryexporter",
-    version='1.0.3.1',
+    version='1.0.3.2',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kilic',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
     packages=find_packages(),
     package_data={'': ['*.md']},
@@ -19,12 +19,12 @@
         "click",
         "mitmproxy",
         "wheel",
         "setuptools",
     ],
     entry_points={
         'console_scripts': [
-            'copilothistoryexporter=copilothistoryexporter.main:sys_main',
+            'copilothistoryexporter=main:sys_main',
         ],
     },
 )
```

