# Comparing `tmp/silvermirror-0.5.tar.gz` & `tmp/silvermirror-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silvermirror-0.5.tar", last modified: Sun Jun  2 20:31:08 2024, max compression
+gzip compressed data, was "silvermirror-0.5.1.tar", last modified: Sun Jun  2 20:33:54 2024, max compression
```

## Comparing `silvermirror-0.5.tar` & `silvermirror-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      248 2024-06-02 20:31:08.004940 silvermirror-0.5/PKG-INFO
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2024-06-02 20:31:08.004940 silvermirror-0.5/setup.cfg
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      806 2024-06-02 20:30:38.000000 silvermirror-0.5/setup.py
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/silvermirror/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/__init__.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     2292 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/config.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     2557 2024-06-02 20:28:40.000000 silvermirror-0.5/silvermirror/hg.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      841 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/interface.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     6469 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/unify.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      800 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/unison.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)      736 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/utils.py
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/silvermirror.egg-info/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      248 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/PKG-INFO
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      440 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/SOURCES.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/dependency_links.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      220 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/entry_points.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-04-12 14:45:45.000000 silvermirror-0.5/silvermirror.egg-info/not-zip-safe
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       44 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/requires.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       13 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/top_level.txt
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/test/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      214 2024-04-12 14:19:20.000000 silvermirror-0.5/test/test_unify.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:33:54.032886 silvermirror-0.5.1/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      268 2024-06-02 20:33:54.032886 silvermirror-0.5.1/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2024-06-02 20:33:54.032886 silvermirror-0.5.1/setup.cfg
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      870 2024-06-02 20:33:39.000000 silvermirror-0.5.1/setup.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:33:54.028886 silvermirror-0.5.1/silvermirror/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2024-04-12 14:19:20.000000 silvermirror-0.5.1/silvermirror/__init__.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     2292 2024-04-12 14:19:20.000000 silvermirror-0.5.1/silvermirror/config.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     2557 2024-06-02 20:28:40.000000 silvermirror-0.5.1/silvermirror/hg.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      841 2024-04-12 14:19:20.000000 silvermirror-0.5.1/silvermirror/interface.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     6469 2024-04-12 14:19:20.000000 silvermirror-0.5.1/silvermirror/unify.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      800 2024-04-12 14:19:20.000000 silvermirror-0.5.1/silvermirror/unison.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)      736 2024-04-12 14:19:20.000000 silvermirror-0.5.1/silvermirror/utils.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:33:54.032886 silvermirror-0.5.1/silvermirror.egg-info/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      268 2024-06-02 20:33:53.000000 silvermirror-0.5.1/silvermirror.egg-info/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      440 2024-06-02 20:33:54.000000 silvermirror-0.5.1/silvermirror.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-06-02 20:33:53.000000 silvermirror-0.5.1/silvermirror.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      220 2024-06-02 20:33:53.000000 silvermirror-0.5.1/silvermirror.egg-info/entry_points.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-04-12 14:45:45.000000 silvermirror-0.5.1/silvermirror.egg-info/not-zip-safe
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       44 2024-06-02 20:33:53.000000 silvermirror-0.5.1/silvermirror.egg-info/requires.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       13 2024-06-02 20:33:53.000000 silvermirror-0.5.1/silvermirror.egg-info/top_level.txt
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:33:54.032886 silvermirror-0.5.1/test/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      214 2024-04-12 14:19:20.000000 silvermirror-0.5.1/test/test_unify.py
```

### Comparing `silvermirror-0.5/setup.py` & `silvermirror-0.5.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import setup
 
-version = '0.5'
+version = '0.5.1'
+description = "mirror files across hosts"
 
 setup(name='silvermirror',
       version=version,
-      description="mirror files across hosts",
+      description=description,
+      long_description=description,
       classifiers=[],
       keywords='mirror unison',
       author='Jeff Hammel',
       author_email='k0scist@gmail.com',
       url='http://k0s.org/hg/silvermirror',
       license='GPL',
       packages=['silvermirror'],
```

### Comparing `silvermirror-0.5/silvermirror/config.py` & `silvermirror-0.5.1/silvermirror/config.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.5/silvermirror/hg.py` & `silvermirror-0.5.1/silvermirror/hg.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.5/silvermirror/interface.py` & `silvermirror-0.5.1/silvermirror/interface.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.5/silvermirror/unify.py` & `silvermirror-0.5.1/silvermirror/unify.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.5/silvermirror/unison.py` & `silvermirror-0.5.1/silvermirror/unison.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.5/silvermirror/utils.py` & `silvermirror-0.5.1/silvermirror/utils.py`

 * *Files identical despite different names*

