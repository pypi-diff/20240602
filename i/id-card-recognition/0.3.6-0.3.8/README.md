# Comparing `tmp/id_card_recognition-0.3.6.tar.gz` & `tmp/id_card_recognition-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.3.6.tar", last modified: Sun Jun  2 00:31:04 2024, max compression
+gzip compressed data, was "id_card_recognition-0.3.8.tar", last modified: Sun Jun  2 00:33:00 2024, max compression
```

## Comparing `id_card_recognition-0.3.6.tar` & `id_card_recognition-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.274351 id_card_recognition-0.3.6/
--rw-r--r--   0 wangligang   (501) staff       (20)     2143 2024-06-02 00:31:04.273843 id_card_recognition-0.3.6/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)     1625 2024-06-02 00:30:40.000000 id_card_recognition-0.3.6/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.270181 id_card_recognition-0.3.6/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.6/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5355 2024-06-01 13:25:08.000000 id_card_recognition-0.3.6/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.6/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.273308 id_card_recognition-0.3.6/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)     2143 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-02 00:31:04.274498 id_card_recognition-0.3.6/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-02 00:30:40.000000 id_card_recognition-0.3.6/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.272816 id_card_recognition-0.3.6/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.6/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:33:00.058353 id_card_recognition-0.3.8/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2097 2024-06-02 00:33:00.057507 id_card_recognition-0.3.8/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)     1625 2024-06-02 00:30:40.000000 id_card_recognition-0.3.8/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:33:00.053394 id_card_recognition-0.3.8/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.8/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5355 2024-06-01 13:25:08.000000 id_card_recognition-0.3.8/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.8/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:33:00.056956 id_card_recognition-0.3.8/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2097 2024-06-02 00:32:59.000000 id_card_recognition-0.3.8/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-02 00:33:00.000000 id_card_recognition-0.3.8/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-02 00:32:59.000000 id_card_recognition-0.3.8/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-02 00:32:59.000000 id_card_recognition-0.3.8/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-02 00:32:59.000000 id_card_recognition-0.3.8/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-02 00:32:59.000000 id_card_recognition-0.3.8/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-02 00:33:00.058502 id_card_recognition-0.3.8/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      801 2024-06-02 00:32:56.000000 id_card_recognition-0.3.8/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:33:00.056458 id_card_recognition-0.3.8/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.8/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.3.6/PKG-INFO` & `id_card_recognition-0.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.6
-Summary: A package for ID card recognition using OpenAI
-Home-page: https://github.com/freedak-wang/id_card_recognition
+Version: 0.3.8
+Summary: A package for ID card recognition using Moonshot AI
+Home-page: 
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `id_card_recognition-0.3.6/README.md` & `id_card_recognition-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.6/id_card_recognition/recognition.py` & `id_card_recognition-0.3.8/id_card_recognition/recognition.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.6/id_card_recognition/utils.py` & `id_card_recognition-0.3.8/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.6/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.3.8/id_card_recognition.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.6
-Summary: A package for ID card recognition using OpenAI
-Home-page: https://github.com/freedak-wang/id_card_recognition
+Version: 0.3.8
+Summary: A package for ID card recognition using Moonshot AI
+Home-page: 
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `id_card_recognition-0.3.6/setup.py` & `id_card_recognition-0.3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.3.6',
+    version='0.3.8',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
     entry_points={
         'console_scripts': [
             'id_card_recognition = id_card_recognition.recognition:main',
         ],
     },
     author='freedak Wang',
     author_email='freedak@163.com',
-    description='A package for ID card recognition using OpenAI',
+    description='A package for ID card recognition using Moonshot AI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/freedak-wang/id_card_recognition',
+    url='',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

