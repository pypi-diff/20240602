# Comparing `tmp/copilothistoryexporter-1.0.3.2.tar.gz` & `tmp/copilothistoryexporter-1.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.3.2.tar", last modified: Sun Jun  2 20:01:31 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.3.3.tar", last modified: Sun Jun  2 20:07:34 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.3.2.tar` & `copilothistoryexporter-1.0.3.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:01:31.080665 copilothistoryexporter-1.0.3.2/
--rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.2/LICENCE
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:01:31.080499 copilothistoryexporter-1.0.3.2/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.2/README.md
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:01:31.080338 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      304 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       57 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:01:31.000000 copilothistoryexporter-1.0.3.2/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:01:31.080698 copilothistoryexporter-1.0.3.2/setup.cfg
--rw-r--r--   0 mustafakilic   (501) staff       (20)      739 2024-06-02 20:01:21.000000 copilothistoryexporter-1.0.3.2/setup.py
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:07:34.400203 copilothistoryexporter-1.0.3.3/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     1073 2024-06-01 16:20:49.000000 copilothistoryexporter-1.0.3.3/LICENCE
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:07:34.400040 copilothistoryexporter-1.0.3.3/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.3.3/README.md
+drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 20:07:34.399872 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      467 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      255 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       42 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 20:07:34.000000 copilothistoryexporter-1.0.3.3/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 20:07:34.400238 copilothistoryexporter-1.0.3.3/setup.cfg
+-rw-r--r--   0 mustafakilic   (501) staff       (20)      621 2024-06-02 20:07:31.000000 copilothistoryexporter-1.0.3.3/setup.py
```

### Comparing `copilothistoryexporter-1.0.3.2/LICENCE` & `copilothistoryexporter-1.0.3.3/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.2/README.md` & `copilothistoryexporter-1.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.3.2/setup.py` & `copilothistoryexporter-1.0.3.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,29 +2,24 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
 
     name="copilothistoryexporter",
-    version='1.0.3.2',
+    version='1.0.3.3',
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
-    entry_points={
-        'console_scripts': [
-            'copilothistoryexporter=main:sys_main',
-        ],
-    },
 )
```

