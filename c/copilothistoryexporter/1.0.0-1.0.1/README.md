# Comparing `tmp/copilothistoryexporter-1.0.0.tar.gz` & `tmp/copilothistoryexporter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.0.tar", last modified: Sun Jun  2 12:56:58 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.1.tar", last modified: Sun Jun  2 16:09:56 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.0.tar` & `copilothistoryexporter-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/copilothistoryexporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 12:56:58.000000 copilothistoryexporter-1.0.0/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-02 12:56:58.000000 copilothistoryexporter-1.0.0/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:56:58.000000 copilothistoryexporter-1.0.0/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 12:56:58.000000 copilothistoryexporter-1.0.0/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 12:56:58.000000 copilothistoryexporter-1.0.0/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-02 12:56:58.000000 copilothistoryexporter-1.0.0/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/src/addons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/addons/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/src/interceptor/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/interceptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/interceptor/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/interceptor/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/interceptor/filte.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/interceptor/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/interceptor/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/interceptor/vote.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:56:58.577957 copilothistoryexporter-1.0.0/src/model/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/model/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/model/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-06-02 12:56:42.000000 copilothistoryexporter-1.0.0/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 16:09:43.000000 copilothistoryexporter-1.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-06-02 16:09:43.000000 copilothistoryexporter-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-02 16:09:43.000000 copilothistoryexporter-1.0.1/setup.py
```

### Comparing `copilothistoryexporter-1.0.0/LICENCE` & `copilothistoryexporter-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.0/README.md` & `copilothistoryexporter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.0/setup.py` & `copilothistoryexporter-1.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
+REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
+
 setup(
     name="copilothistoryexporter",
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kılıç',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=[
-        "click",
-        "requests",
-        "mitmproxy"
-    ],
+    packages=find_packages(
+        include=["sample.md"]
+    ),
+    install_requires=REQUIREMENTS,
     entry_points={
         'console_scripts': [
-            'copilothistoryexporter=src.main:main',
+            'copilothistoryexporter = copilothistoryexporter.main:main',
         ],
     },
 )
```

