# Comparing `tmp/rxnSMILES4AtomEco-1.0.0.tar.gz` & `tmp/rxnSMILES4AtomEco-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxnSMILES4AtomEco-1.0.0.tar", last modified: Sat Jun  1 21:33:51 2024, max compression
+gzip compressed data, was "rxnSMILES4AtomEco-1.0.2.tar", last modified: Sat Jun  1 21:48:40 2024, max compression
```

## Comparing `rxnSMILES4AtomEco-1.0.0.tar` & `rxnSMILES4AtomEco-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:33:51.005733 rxnSMILES4AtomEco-1.0.0/
--rw-rw-rw-   0        0        0      633 2024-05-17 18:38:51.000000 rxnSMILES4AtomEco-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      441 2024-06-01 21:33:51.002735 rxnSMILES4AtomEco-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7108 2024-05-28 07:21:33.000000 rxnSMILES4AtomEco-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:33:50.999734 rxnSMILES4AtomEco-1.0.0/rxnSMILES4AtomEco.egg-info/
--rw-rw-rw-   0        0        0      441 2024-06-01 21:33:50.000000 rxnSMILES4AtomEco-1.0.0/rxnSMILES4AtomEco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-06-01 21:33:50.000000 rxnSMILES4AtomEco-1.0.0/rxnSMILES4AtomEco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:33:50.000000 rxnSMILES4AtomEco-1.0.0/rxnSMILES4AtomEco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:33:50.000000 rxnSMILES4AtomEco-1.0.0/rxnSMILES4AtomEco.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 21:33:51.006735 rxnSMILES4AtomEco-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      542 2024-06-01 21:30:21.000000 rxnSMILES4AtomEco-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:48:40.122443 rxnSMILES4AtomEco-1.0.2/
+-rw-rw-rw-   0        0        0      633 2024-05-17 18:38:51.000000 rxnSMILES4AtomEco-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      462 2024-06-01 21:48:40.118444 rxnSMILES4AtomEco-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7108 2024-05-28 07:21:33.000000 rxnSMILES4AtomEco-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:48:40.116443 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/
+-rw-rw-rw-   0        0        0      462 2024-06-01 21:48:39.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-06-01 21:48:40.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:48:39.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:48:39.000000 rxnSMILES4AtomEco-1.0.2/rxnSMILES4AtomEco.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 21:48:40.123443 rxnSMILES4AtomEco-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      563 2024-06-01 21:48:35.000000 rxnSMILES4AtomEco-1.0.2/setup.py
```

### Comparing `rxnSMILES4AtomEco-1.0.0/LICENSE` & `rxnSMILES4AtomEco-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rxnSMILES4AtomEco-1.0.0/README.md` & `rxnSMILES4AtomEco-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rxnSMILES4AtomEco-1.0.0/setup.py` & `rxnSMILES4AtomEco-1.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rxnSMILES4AtomEco',
-    version='1.0.0',
+    version='1.0.2',
     packages=find_packages(),
     description='Calculate atom economy for chemical reactions using reaction SMILES',
     author='Samuele Giani',
     author_email='samuele.giani@empa.ch',
-    url='https://your-package-url.com',
+    url='https://pypi.org/project/rxnSMILES4AtomEco/1.0.0/',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
 )
```

