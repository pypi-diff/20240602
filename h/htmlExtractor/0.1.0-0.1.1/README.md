# Comparing `tmp/htmlExtractor-0.1.0.tar.gz` & `tmp/htmlExtractor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmlExtractor-0.1.0.tar", last modified: Sun Jun  2 13:10:45 2024, max compression
+gzip compressed data, was "htmlExtractor-0.1.1.tar", last modified: Sun Jun  2 13:21:26 2024, max compression
```

## Comparing `htmlExtractor-0.1.0.tar` & `htmlExtractor-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 13:10:45.695850 htmlExtractor-0.1.0/
--rw-rw-rw-   0        0        0      490 2024-06-02 13:10:45.694853 htmlExtractor-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 13:10:45.694853 htmlExtractor-0.1.0/htmlExtractor.egg-info/
--rw-rw-rw-   0        0        0      490 2024-06-02 13:10:45.000000 htmlExtractor-0.1.0/htmlExtractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-06-02 13:10:45.000000 htmlExtractor-0.1.0/htmlExtractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 13:10:45.000000 htmlExtractor-0.1.0/htmlExtractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-06-02 13:10:45.000000 htmlExtractor-0.1.0/htmlExtractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-02 13:10:45.000000 htmlExtractor-0.1.0/htmlExtractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-02 13:10:45.693848 htmlExtractor-0.1.0/libname/
--rw-rw-rw-   0        0        0       33 2024-06-02 13:03:55.000000 htmlExtractor-0.1.0/libname/__init__.py
--rw-rw-rw-   0        0        0      192 2024-06-02 13:03:17.000000 htmlExtractor-0.1.0/libname/htmlExtractor.py
--rw-rw-rw-   0        0        0       42 2024-06-02 13:10:45.695850 htmlExtractor-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-06-02 13:09:07.000000 htmlExtractor-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:21:26.722235 htmlExtractor-0.1.1/
+-rw-rw-rw-   0        0        0     2127 2024-06-02 13:21:26.721234 htmlExtractor-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 13:21:26.721234 htmlExtractor-0.1.1/htmlExtractor.egg-info/
+-rw-rw-rw-   0        0        0     2127 2024-06-02 13:21:26.000000 htmlExtractor-0.1.1/htmlExtractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-06-02 13:21:26.000000 htmlExtractor-0.1.1/htmlExtractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 13:21:26.000000 htmlExtractor-0.1.1/htmlExtractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-06-02 13:21:26.000000 htmlExtractor-0.1.1/htmlExtractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 13:21:26.000000 htmlExtractor-0.1.1/htmlExtractor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:21:26.720233 htmlExtractor-0.1.1/libname/
+-rw-rw-rw-   0        0        0       33 2024-06-02 13:03:55.000000 htmlExtractor-0.1.1/libname/__init__.py
+-rw-rw-rw-   0        0        0      192 2024-06-02 13:03:17.000000 htmlExtractor-0.1.1/libname/htmlExtractor.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 13:21:26.722235 htmlExtractor-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      852 2024-06-02 13:20:12.000000 htmlExtractor-0.1.1/setup.py
```

### Comparing `htmlExtractor-0.1.0/setup.py` & `htmlExtractor-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
+import pathlib
 
-
-
+HERE = pathlib.Path(__file__).parent
+README = (HERE / "readme.MD").read_text()
 # Setting up
 setup(
 name='htmlExtractor',  
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     author='Md Anisur Rahman',
     author_email='anisurrahman06046@gmail.com',
     description='A simple package to fetch HTML data from a website',
+    long_description=README,
+    long_description_content_type='text/markdown',
     url='https://github.com/AnisurRahman06046/fetchHtml_website.git',  # Your GitHub URL
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
```

