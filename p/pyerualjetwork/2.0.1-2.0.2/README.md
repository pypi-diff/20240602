# Comparing `tmp/pyerualjetwork-2.0.1.tar.gz` & `tmp/pyerualjetwork-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-2.0.1.tar", last modified: Sun Jun  2 19:00:03 2024, max compression
+gzip compressed data, was "pyerualjetwork-2.0.2.tar", last modified: Sun Jun  2 19:04:22 2024, max compression
```

## Comparing `pyerualjetwork-2.0.1.tar` & `pyerualjetwork-2.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:00:03.018756 pyerualjetwork-2.0.1/
--rw-rw-rw-   0        0        0      429 2024-06-02 19:00:03.016760 pyerualjetwork-2.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 19:00:02.994476 pyerualjetwork-2.0.1/plan/
--rw-rw-rw-   0        0        0      381 2024-06-02 18:58:09.000000 pyerualjetwork-2.0.1/plan/__init__.py
--rw-rw-rw-   0        0        0    33061 2024-06-02 18:28:02.000000 pyerualjetwork-2.0.1/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:00:03.013764 pyerualjetwork-2.0.1/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      429 2024-06-02 19:00:02.000000 pyerualjetwork-2.0.1/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-06-02 19:00:02.000000 pyerualjetwork-2.0.1/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:00:02.000000 pyerualjetwork-2.0.1/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-06-02 19:00:02.000000 pyerualjetwork-2.0.1/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 19:00:03.018756 pyerualjetwork-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-06-02 18:59:54.000000 pyerualjetwork-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:04:22.387241 pyerualjetwork-2.0.2/
+-rw-rw-rw-   0        0        0      429 2024-06-02 19:04:22.386244 pyerualjetwork-2.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 19:04:22.361099 pyerualjetwork-2.0.2/plan/
+-rw-rw-rw-   0        0        0      377 2024-06-02 19:03:35.000000 pyerualjetwork-2.0.2/plan/__init__.py
+-rw-rw-rw-   0        0        0    33061 2024-06-02 18:28:02.000000 pyerualjetwork-2.0.2/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:04:22.383254 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      429 2024-06-02 19:04:21.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-06-02 19:04:22.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:04:21.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-06-02 19:04:21.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:04:22.388240 pyerualjetwork-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-06-02 19:04:06.000000 pyerualjetwork-2.0.2/setup.py
```

### Comparing `pyerualjetwork-2.0.1/plan/plan.py` & `pyerualjetwork-2.0.2/plan/plan.py`

 * *Files identical despite different names*

### Comparing `pyerualjetwork-2.0.1/setup.py` & `pyerualjetwork-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "2.0.1",
+      version = "2.0.2",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library. New features: More simple and practical, all functions and variables are snake_case. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
```

