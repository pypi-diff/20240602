# Comparing `tmp/aixhello-2.0.tar.gz` & `tmp/aixhello-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-2.0.tar", last modified: Sat Jun  1 21:39:51 2024, max compression
+gzip compressed data, was "aixhello-2.1.tar", last modified: Sat Jun  1 21:46:22 2024, max compression
```

## Comparing `aixhello-2.0.tar` & `aixhello-2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:39:51.544172 aixhello-2.0/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.0/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      650 2024-06-01 21:39:51.543169 aixhello-2.0/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:39:51.525078 aixhello-2.0/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.0/aixhello/__init__.py
--rw-rw-rw-   0        0        0   422971 2024-06-01 21:39:43.000000 aixhello-2.0/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 21:39:51.542168 aixhello-2.0/aixhello.egg-info/
--rw-rw-rw-   0        0        0      650 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 21:39:51.000000 aixhello-2.0/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 21:39:51.545168 aixhello-2.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 21:39:18.000000 aixhello-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:46:22.656191 aixhello-2.1/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.1/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:46:22.655192 aixhello-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:46:22.636035 aixhello-2.1/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.1/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   422971 2024-06-01 21:46:16.000000 aixhello-2.1/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 21:46:22.654195 aixhello-2.1/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 21:46:22.658201 aixhello-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 21:45:44.000000 aixhello-2.1/setup.py
```

### Comparing `aixhello-2.0/LICENSE` & `aixhello-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-2.0/PKG-INFO` & `aixhello-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 2.0
+Version: 2.1
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-2.0/aixhello/xyello.c` & `aixhello-2.1/aixhello/xyello.c`

 * *Files identical despite different names*

### Comparing `aixhello-2.0/aixhello.egg-info/PKG-INFO` & `aixhello-2.1/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 2.0
+Version: 2.1
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-2.0/setup.py` & `aixhello-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='2.0',  # Increment the version number
+    version='2.1',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

