# Comparing `tmp/rxnSMILES4AtomEco-1.0.5.tar.gz` & `tmp/rxnSMILES4AtomEco-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxnSMILES4AtomEco-1.0.5.tar", last modified: Sat Jun  1 22:04:13 2024, max compression
+gzip compressed data, was "rxnSMILES4AtomEco-1.0.6.tar", last modified: Sat Jun  1 22:10:26 2024, max compression
```

## Comparing `rxnSMILES4AtomEco-1.0.5.tar` & `rxnSMILES4AtomEco-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:04:13.689368 rxnSMILES4AtomEco-1.0.5/
--rw-rw-rw-   0        0        0      633 2024-05-17 18:38:51.000000 rxnSMILES4AtomEco-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      455 2024-06-01 22:04:13.684314 rxnSMILES4AtomEco-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7108 2024-05-28 07:21:33.000000 rxnSMILES4AtomEco-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 22:04:13.680313 rxnSMILES4AtomEco-1.0.5/rxnSMILES4AtomEco.egg-info/
--rw-rw-rw-   0        0        0      455 2024-06-01 22:04:13.000000 rxnSMILES4AtomEco-1.0.5/rxnSMILES4AtomEco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-06-01 22:04:13.000000 rxnSMILES4AtomEco-1.0.5/rxnSMILES4AtomEco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:04:13.000000 rxnSMILES4AtomEco-1.0.5/rxnSMILES4AtomEco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:04:13.000000 rxnSMILES4AtomEco-1.0.5/rxnSMILES4AtomEco.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 22:04:13.689368 rxnSMILES4AtomEco-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      556 2024-06-01 22:04:10.000000 rxnSMILES4AtomEco-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:10:26.425024 rxnSMILES4AtomEco-1.0.6/
+-rw-rw-rw-   0        0        0      633 2024-05-17 18:38:51.000000 rxnSMILES4AtomEco-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      455 2024-06-01 22:10:26.422113 rxnSMILES4AtomEco-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7108 2024-05-28 07:21:33.000000 rxnSMILES4AtomEco-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:10:26.406994 rxnSMILES4AtomEco-1.0.6/rxn4SMILESAtomEco/
+-rw-rw-rw-   0        0        0      114 2024-06-01 22:09:47.000000 rxnSMILES4AtomEco-1.0.6/rxn4SMILESAtomEco/__init__.py
+-rw-rw-rw-   0        0        0     4285 2024-06-01 21:47:38.000000 rxnSMILES4AtomEco-1.0.6/rxn4SMILESAtomEco/rxnSMILES4AtomEco.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:10:26.418990 rxnSMILES4AtomEco-1.0.6/rxnSMILES4AtomEco.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-06-01 22:10:26.000000 rxnSMILES4AtomEco-1.0.6/rxnSMILES4AtomEco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-06-01 22:10:26.000000 rxnSMILES4AtomEco-1.0.6/rxnSMILES4AtomEco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:10:26.000000 rxnSMILES4AtomEco-1.0.6/rxnSMILES4AtomEco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-06-01 22:10:26.000000 rxnSMILES4AtomEco-1.0.6/rxnSMILES4AtomEco.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 22:10:26.425024 rxnSMILES4AtomEco-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      556 2024-06-01 22:10:23.000000 rxnSMILES4AtomEco-1.0.6/setup.py
```

### Comparing `rxnSMILES4AtomEco-1.0.5/LICENSE` & `rxnSMILES4AtomEco-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rxnSMILES4AtomEco-1.0.5/README.md` & `rxnSMILES4AtomEco-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rxnSMILES4AtomEco-1.0.5/setup.py` & `rxnSMILES4AtomEco-1.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rxnSMILES4AtomEco',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     description='Calculate atom economy for chemical reactions using reaction SMILES',
     author='Samuele Giani',
     author_email='samuele.giani@empa.ch',
     url='https://pypi.org/project/rxnSMILES4AtomEco',
     classifiers=[
         'Programming Language :: Python :: 3',
```

