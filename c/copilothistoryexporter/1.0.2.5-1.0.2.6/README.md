# Comparing `tmp/copilothistoryexporter-1.0.2.5.tar.gz` & `tmp/copilothistoryexporter-1.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.2.5.tar", last modified: Sun Jun  2 18:46:44 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.2.6.tar", last modified: Sun Jun  2 18:53:02 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.2.5.tar` & `copilothistoryexporter-1.0.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:46:44.497400 copilothistoryexporter-1.0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 18:46:44.497400 copilothistoryexporter-1.0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:46:44.497400 copilothistoryexporter-1.0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:46:44.489400 copilothistoryexporter-1.0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:46:44.493400 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:46:44.493400 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/addons/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/addons/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:46:44.493400 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/vote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:46:44.497400 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/model/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/model/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/model/request.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/sample.md
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-06-02 18:46:28.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:46:44.493400 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 18:46:44.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 18:46:44.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:46:44.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 18:46:44.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 18:46:44.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 18:46:44.000000 copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:53:02.177664 copilothistoryexporter-1.0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 18:53:02.177664 copilothistoryexporter-1.0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:53:02.177664 copilothistoryexporter-1.0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:53:02.173664 copilothistoryexporter-1.0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:53:02.173664 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:53:02.177664 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/addons/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:53:02.177664 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:53:02.177664 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/model/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/model/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/sample.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-06-02 18:52:40.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:53:02.177664 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 18:53:02.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 18:53:02.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:53:02.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 18:53:02.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 18:53:02.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 18:53:02.000000 copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/top_level.txt
```

### Comparing `copilothistoryexporter-1.0.2.5/LICENCE` & `copilothistoryexporter-1.0.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/README.md` & `copilothistoryexporter-1.0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/setup.py` & `copilothistoryexporter-1.0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(
     name="copilothistoryexporter",
-    version='1.0.2.5',
+    version='1.0.2.6',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kılıç',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
     package_dir={'': 'src'},
     packages=find_packages('src', include=["*"]),
```

### Comparing `copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/addons/binding.py` & `copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/addons/binding.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/cache.py` & `copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/cache.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/chain.py` & `copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/chain.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/interceptor/vote.py` & `copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/interceptor/vote.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/main.py` & `copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/main.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/src/copilothistoryexporter/utils.py` & `copilothistoryexporter-1.0.2.6/src/copilothistoryexporter/utils.py`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.2.5/src/copilothistoryexporter.egg-info/SOURCES.txt` & `copilothistoryexporter-1.0.2.6/src/copilothistoryexporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

