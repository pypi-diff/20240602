# Comparing `tmp/vizrecurse-1.1.1a1.tar.gz` & `tmp/vizrecurse-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizrecurse-1.1.1a1.tar", last modified: Sun May 26 21:58:41 2024, max compression
+gzip compressed data, was "vizrecurse-1.1.2.tar", last modified: Sun Jun  2 01:04:33 2024, max compression
```

## Comparing `vizrecurse-1.1.1a1.tar` & `vizrecurse-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 21:58:41.345915 vizrecurse-1.1.1a1/
--rw-r--r--   0 enso       (501) staff       (20)      361 2024-05-26 21:58:41.345766 vizrecurse-1.1.1a1/PKG-INFO
--rw-r--r--   0 enso       (501) staff       (20)     3118 2024-05-26 20:10:38.000000 vizrecurse-1.1.1a1/README.md
--rw-r--r--   0 enso       (501) staff       (20)       38 2024-05-26 21:58:41.345966 vizrecurse-1.1.1a1/setup.cfg
--rw-r--r--   0 enso       (501) staff       (20)     1222 2024-05-26 21:58:36.000000 vizrecurse-1.1.1a1/setup.py
-drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 21:58:41.343006 vizrecurse-1.1.1a1/vizrecurse/
--rw-r--r--   0 enso       (501) staff       (20)      229 2024-05-24 21:05:55.000000 vizrecurse-1.1.1a1/vizrecurse/__init__.py
--rw-r--r--   0 enso       (501) staff       (20)      433 2024-05-25 22:59:24.000000 vizrecurse-1.1.1a1/vizrecurse/debug.py
--rw-r--r--   0 enso       (501) staff       (20)     1573 2024-05-25 21:07:35.000000 vizrecurse-1.1.1a1/vizrecurse/display.py
--rw-r--r--   0 enso       (501) staff       (20)        0 2024-05-26 21:48:19.000000 vizrecurse-1.1.1a1/vizrecurse/py.typed
--rw-r--r--   0 enso       (501) staff       (20)     2393 2024-05-25 23:18:42.000000 vizrecurse-1.1.1a1/vizrecurse/vizzy.py
-drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 21:58:41.345579 vizrecurse-1.1.1a1/vizrecurse.egg-info/
--rw-r--r--   0 enso       (501) staff       (20)      361 2024-05-26 21:58:41.000000 vizrecurse-1.1.1a1/vizrecurse.egg-info/PKG-INFO
--rw-r--r--   0 enso       (501) staff       (20)      292 2024-05-26 21:58:41.000000 vizrecurse-1.1.1a1/vizrecurse.egg-info/SOURCES.txt
--rw-r--r--   0 enso       (501) staff       (20)        1 2024-05-26 21:58:41.000000 vizrecurse-1.1.1a1/vizrecurse.egg-info/dependency_links.txt
--rw-r--r--   0 enso       (501) staff       (20)      394 2024-05-26 21:58:41.000000 vizrecurse-1.1.1a1/vizrecurse.egg-info/requires.txt
--rw-r--r--   0 enso       (501) staff       (20)       11 2024-05-26 21:58:41.000000 vizrecurse-1.1.1a1/vizrecurse.egg-info/top_level.txt
+drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-06-02 01:04:33.421439 vizrecurse-1.1.2/
+-rw-r--r--   0 enso       (501) staff       (20)     3519 2024-06-02 01:04:33.421298 vizrecurse-1.1.2/PKG-INFO
+-rw-r--r--   0 enso       (501) staff       (20)     3118 2024-05-27 02:57:11.000000 vizrecurse-1.1.2/README.md
+-rw-r--r--   0 enso       (501) staff       (20)       38 2024-06-02 01:04:33.421592 vizrecurse-1.1.2/setup.cfg
+-rw-r--r--   0 enso       (501) staff       (20)     1392 2024-06-02 01:04:20.000000 vizrecurse-1.1.2/setup.py
+drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-06-02 01:04:33.420392 vizrecurse-1.1.2/vizrecurse/
+-rw-r--r--   0 enso       (501) staff       (20)      229 2024-05-24 21:05:55.000000 vizrecurse-1.1.2/vizrecurse/__init__.py
+-rw-r--r--   0 enso       (501) staff       (20)      433 2024-05-25 22:59:24.000000 vizrecurse-1.1.2/vizrecurse/debug.py
+-rw-r--r--   0 enso       (501) staff       (20)     1573 2024-05-25 21:07:35.000000 vizrecurse-1.1.2/vizrecurse/display.py
+-rw-r--r--   0 enso       (501) staff       (20)        0 2024-05-26 22:02:46.000000 vizrecurse-1.1.2/vizrecurse/py.typed
+-rw-r--r--   0 enso       (501) staff       (20)     2394 2024-05-27 02:41:33.000000 vizrecurse-1.1.2/vizrecurse/vizzy.py
+drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-06-02 01:04:33.421118 vizrecurse-1.1.2/vizrecurse.egg-info/
+-rw-r--r--   0 enso       (501) staff       (20)     3519 2024-06-02 01:04:33.000000 vizrecurse-1.1.2/vizrecurse.egg-info/PKG-INFO
+-rw-r--r--   0 enso       (501) staff       (20)      292 2024-06-02 01:04:33.000000 vizrecurse-1.1.2/vizrecurse.egg-info/SOURCES.txt
+-rw-r--r--   0 enso       (501) staff       (20)        1 2024-06-02 01:04:33.000000 vizrecurse-1.1.2/vizrecurse.egg-info/dependency_links.txt
+-rw-r--r--   0 enso       (501) staff       (20)      394 2024-06-02 01:04:33.000000 vizrecurse-1.1.2/vizrecurse.egg-info/requires.txt
+-rw-r--r--   0 enso       (501) staff       (20)       11 2024-06-02 01:04:33.000000 vizrecurse-1.1.2/vizrecurse.egg-info/top_level.txt
```

### Comparing `vizrecurse-1.1.1a1/README.md` & `vizrecurse-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### About viz.recurse
 viz.recurse is a bare-bones library to easily visualize recursion without any significant overhead on the part of the user. This library utilizes common graph and visualization libraries (networkx, matplotlib, pygraphviz).
 
-### Latest PyPi release [1.1.0]
-Visit https://pypi.org/project/vizrecurse/1.1.0/
+### Latest PyPi release [1.1.1]
+Visit https://pypi.org/project/vizrecurse/1.1.1/
 
 ### Requirements
 `Python 3.10.13`\
 `pip 23.0.1` (graphviz compatibility)\
 `brew install graphviz` (MacOS)\
 `pip3 install -r requirements.txt`
```

### Comparing `vizrecurse-1.1.1a1/setup.py` & `vizrecurse-1.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """PyPi vizrecurse setup"""
+from pathlib import Path
+
 from setuptools import setup, find_packages
+
 setup(
     name='vizrecurse',
-    version='1.1.1a1',
+    version='1.1.2',
     author='Cody Pedersen',
     description='Bare bones library to vizualize recursion with one line of code.',
+    long_description=(Path(__file__).parent/"README.md").read_text(),
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3.10',
     'Operating System :: OS Independent',
     'Intended Audience :: Developers',
     'Intended Audience :: Education'
     ],
     python_requires='>=3.10',
+    readme="README.md",
     install_requires=[
         "astroid==3.2.2",
         "contourpy==1.2.1",
         "cycler==0.12.1",
         "dill==0.3.8",
         "fonttools==4.51.0",
         "graphviz==0.20.3",
```

### Comparing `vizrecurse-1.1.1a1/vizrecurse/display.py` & `vizrecurse-1.1.2/vizrecurse/display.py`

 * *Files identical despite different names*

### Comparing `vizrecurse-1.1.1a1/vizrecurse/vizzy.py` & `vizrecurse-1.1.2/vizrecurse/vizzy.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     return {
         "node_for_adding":f"{addr}.{fn_label}.{str(ts)}",
         "label": fn_label,
         "addr": addr,
         "ts": ts
     }
 
+
 def visualize(func: Callable[Param, RetType]) -> Callable[Param, RetType]:
     """Decorator for visualization of recursive calls"""
 
     def inner(*args: Param.args, **kwargs: Param.kwargs) -> RetType:
         # function signature for traceability
         fn_timestamp = time.time_ns()
```

