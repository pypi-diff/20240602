# Comparing `tmp/rxnSMILES4AtomEco-1.0.2.tar.gz` & `tmp/rxnSMILES4AtomEco-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxnSMILES4AtomEco-1.0.2.tar", last modified: Sat Jun  1 21:48:40 2024, max compression
+gzip compressed data, was "rxnSMILES4AtomEco-1.0.4.tar", last modified: Sat Jun  1 22:00:53 2024, max compression
```

## Comparing `rxnSMILES4AtomEco-1.0.2.tar` & `rxnSMILES4AtomEco-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:48:40.122443 rxnSMILES4AtomEco-1.0.2/
--rw-rw-rw-   0        0        0      633 2024-05-17 18:38:51.000000 rxnSMILES4AtomEco-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      462 2024-06-01 21:48:40.118444 rxnSMILES4AtomEco-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7108 2024-05-28 07:21:33.000000 rxnSMILES4AtomEco-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:48:40.116443 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/
--rw-rw-rw-   0        0        0      462 2024-06-01 21:48:39.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-06-01 21:48:40.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:48:39.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:48:39.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 21:48:40.123443 rxnSMILES4AtomEco-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      563 2024-06-01 21:48:35.000000 rxnSMILES4AtomEco-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:00:53.978526 rxnSMILES4AtomEco-1.0.4/
+-rw-rw-rw-   0        0        0      633 2024-05-17 18:38:51.000000 rxnSMILES4AtomEco-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      462 2024-06-01 22:00:53.974477 rxnSMILES4AtomEco-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7108 2024-05-28 07:21:33.000000 rxnSMILES4AtomEco-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:00:53.972477 rxnSMILES4AtomEco-1.0.4/rxnSMILES4AtomEco.egg-info/
+-rw-rw-rw-   0        0        0      462 2024-06-01 22:00:53.000000 rxnSMILES4AtomEco-1.0.4/rxnSMILES4AtomEco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-06-01 22:00:53.000000 rxnSMILES4AtomEco-1.0.4/rxnSMILES4AtomEco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:00:53.000000 rxnSMILES4AtomEco-1.0.4/rxnSMILES4AtomEco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:00:53.000000 rxnSMILES4AtomEco-1.0.4/rxnSMILES4AtomEco.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 22:00:53.978526 rxnSMILES4AtomEco-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      563 2024-06-01 21:59:48.000000 rxnSMILES4AtomEco-1.0.4/setup.py
```

### Comparing `rxnSMILES4AtomEco-1.0.2/LICENSE` & `rxnSMILES4AtomEco-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rxnSMILES4AtomEco-1.0.2/README.md` & `rxnSMILES4AtomEco-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rxnSMILES4AtomEco-1.0.2/setup.py` & `rxnSMILES4AtomEco-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rxnSMILES4AtomEco',
-    version='1.0.2',
+    version='1.0.4',
     packages=find_packages(),
     description='Calculate atom economy for chemical reactions using reaction SMILES',
     author='Samuele Giani',
     author_email='samuele.giani@empa.ch',
     url='https://pypi.org/project/rxnSMILES4AtomEco/1.0.0/',
     classifiers=[
         'Programming Language :: Python :: 3',
```

