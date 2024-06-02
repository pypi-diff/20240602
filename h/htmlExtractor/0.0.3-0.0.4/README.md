# Comparing `tmp/htmlExtractor-0.0.3.tar.gz` & `tmp/htmlExtractor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmlExtractor-0.0.3.tar", last modified: Sun Jun  2 13:23:45 2024, max compression
+gzip compressed data, was "htmlExtractor-0.0.4.tar", last modified: Sun Jun  2 13:32:05 2024, max compression
```

## Comparing `htmlExtractor-0.0.3.tar` & `htmlExtractor-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 13:23:45.774326 htmlExtractor-0.0.3/
--rw-rw-rw-   0        0        0     2127 2024-06-02 13:23:45.774326 htmlExtractor-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 13:23:45.773326 htmlExtractor-0.0.3/htmlExtractor.egg-info/
--rw-rw-rw-   0        0        0     2127 2024-06-02 13:23:45.000000 htmlExtractor-0.0.3/htmlExtractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-06-02 13:23:45.000000 htmlExtractor-0.0.3/htmlExtractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 13:23:45.000000 htmlExtractor-0.0.3/htmlExtractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-06-02 13:23:45.000000 htmlExtractor-0.0.3/htmlExtractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-02 13:23:45.000000 htmlExtractor-0.0.3/htmlExtractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-02 13:23:45.773326 htmlExtractor-0.0.3/libname/
--rw-rw-rw-   0        0        0       39 2024-06-02 13:23:38.000000 htmlExtractor-0.0.3/libname/__init__.py
--rw-rw-rw-   0        0        0      198 2024-06-02 13:22:31.000000 htmlExtractor-0.0.3/libname/htmlExtractor.py
--rw-rw-rw-   0        0        0       42 2024-06-02 13:23:45.775327 htmlExtractor-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      852 2024-06-02 13:23:18.000000 htmlExtractor-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:32:05.556982 htmlExtractor-0.0.4/
+-rw-rw-rw-   0        0        0     2127 2024-06-02 13:32:05.556982 htmlExtractor-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 13:32:05.555982 htmlExtractor-0.0.4/htmlExtractor.egg-info/
+-rw-rw-rw-   0        0        0     2127 2024-06-02 13:32:05.000000 htmlExtractor-0.0.4/htmlExtractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-06-02 13:32:05.000000 htmlExtractor-0.0.4/htmlExtractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 13:32:05.000000 htmlExtractor-0.0.4/htmlExtractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-06-02 13:32:05.000000 htmlExtractor-0.0.4/htmlExtractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 13:32:05.000000 htmlExtractor-0.0.4/htmlExtractor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 13:32:05.554982 htmlExtractor-0.0.4/libname/
+-rw-rw-rw-   0        0        0       40 2024-06-02 13:31:28.000000 htmlExtractor-0.0.4/libname/__init__.py
+-rw-rw-rw-   0        0        0      198 2024-06-02 13:22:31.000000 htmlExtractor-0.0.4/libname/htmlExtractor.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 13:32:05.556982 htmlExtractor-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      852 2024-06-02 13:31:18.000000 htmlExtractor-0.0.4/setup.py
```

### Comparing `htmlExtractor-0.0.3/PKG-INFO` & `htmlExtractor-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmlExtractor
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple package to fetch HTML data from a website
 Home-page: https://github.com/AnisurRahman06046/fetchHtml_website.git
 Author: Md Anisur Rahman
 Author-email: anisurrahman06046@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `htmlExtractor-0.0.3/htmlExtractor.egg-info/PKG-INFO` & `htmlExtractor-0.0.4/htmlExtractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmlExtractor
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple package to fetch HTML data from a website
 Home-page: https://github.com/AnisurRahman06046/fetchHtml_website.git
 Author: Md Anisur Rahman
 Author-email: anisurrahman06046@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `htmlExtractor-0.0.3/setup.py` & `htmlExtractor-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "readme.MD").read_text()
 # Setting up
 setup(
 name='htmlExtractor',  
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     author='Md Anisur Rahman',
     author_email='anisurrahman06046@gmail.com',
```

