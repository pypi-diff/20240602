# Comparing `tmp/copilothistoryexporter-1.0.1.tar.gz` & `tmp/copilothistoryexporter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copilothistoryexporter-1.0.1.tar", last modified: Sun Jun  2 16:09:56 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.2.tar", last modified: Sun Jun  2 16:53:00 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.1.tar` & `copilothistoryexporter-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 16:09:43.000000 copilothistoryexporter-1.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-06-02 16:09:43.000000 copilothistoryexporter-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:09:56.000000 copilothistoryexporter-1.0.1/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:09:56.175027 copilothistoryexporter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-02 16:09:43.000000 copilothistoryexporter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:53:00.538399 copilothistoryexporter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 16:53:00.538399 copilothistoryexporter-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:53:00.538399 copilothistoryexporter-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:53:00.534399 copilothistoryexporter-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:53:00.534399 copilothistoryexporter-1.0.2/src/copilothistoryexporter/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:53:00.538399 copilothistoryexporter-1.0.2/src/copilothistoryexporter/addons/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/addons/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:53:00.538399 copilothistoryexporter-1.0.2/src/copilothistoryexporter/interceptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/interceptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/interceptor/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/interceptor/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/interceptor/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/interceptor/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/interceptor/vote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:53:00.538399 copilothistoryexporter-1.0.2/src/copilothistoryexporter/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/model/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/model/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/sample.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-06-02 16:52:47.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:53:00.538399 copilothistoryexporter-1.0.2/src/copilothistoryexporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 16:53:00.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 16:53:00.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:53:00.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 16:53:00.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 16:53:00.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 16:53:00.000000 copilothistoryexporter-1.0.2/src/copilothistoryexporter.egg-info/top_level.txt
```

### Comparing `copilothistoryexporter-1.0.1/LICENCE` & `copilothistoryexporter-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `copilothistoryexporter-1.0.1/README.md` & `copilothistoryexporter-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 #### Pip
 ```shell
 pip install copilot-exporter
 ```
 
 #### Brew
 ```ruby
-brew install enciyo/taps/copilotexporter
+brew tap enciyo/taps
+brew install copilothistoryexporter
 ```
 
 ### Notes
 
 - The output keeps track of the chat history after running the script. Previous chat history cannot be exported
 - This project is still in development.
 - This project is not affiliated with GitHub Copilot.
```

### Comparing `copilothistoryexporter-1.0.1/setup.py` & `copilothistoryexporter-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(
     name="copilothistoryexporter",
-    version='1.0.1',
+    version='1.0.2',
     url='https://github.com/enciyo/gh-copilot-history-export',
     author='Mustafa Kılıç',
     author_email='enciyomk61@gmail.com',
     description='This package exports the history of GitHub Copilot chat history.',
     long_description="This package exports the history of GitHub Copilot chat history.",
-    packages=find_packages(
-        include=["sample.md"]
-    ),
+    package_dir={'': 'src'},
+    packages=find_packages('src', include=["*"]),
+    package_data={'': ['*.md']},
     install_requires=REQUIREMENTS,
     entry_points={
         'console_scripts': [
-            'copilothistoryexporter = copilothistoryexporter.main:main',
+            'copilothistoryexporter=copilothistoryexporter.main:sys_main',
         ],
     },
 )
```

