# Comparing `tmp/real_time_translator-0.1.0.tar.gz` & `tmp/real_time_translator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real_time_translator-0.1.0.tar", last modified: Sun Jun  2 07:28:46 2024, max compression
+gzip compressed data, was "real_time_translator-0.1.1.tar", last modified: Sun Jun  2 07:42:19 2024, max compression
```

## Comparing `real_time_translator-0.1.0.tar` & `real_time_translator-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 07:28:46.159224 real_time_translator-0.1.0/
--rw-rw-rw-   0        0        0     4920 2024-06-02 07:28:46.150104 real_time_translator-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3885 2024-06-02 06:17:20.000000 real_time_translator-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 07:28:46.149296 real_time_translator-0.1.0/real_time_translator.egg-info/
--rw-rw-rw-   0        0        0     4920 2024-06-02 07:28:46.000000 real_time_translator-0.1.0/real_time_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-06-02 07:28:46.000000 real_time_translator-0.1.0/real_time_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 07:28:46.000000 real_time_translator-0.1.0/real_time_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-06-02 07:28:46.000000 real_time_translator-0.1.0/real_time_translator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-06-02 07:28:46.000000 real_time_translator-0.1.0/real_time_translator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 07:28:46.000000 real_time_translator-0.1.0/real_time_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 07:28:46.159224 real_time_translator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1340 2024-06-02 07:26:31.000000 real_time_translator-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:42:19.892420 real_time_translator-0.1.1/
+-rw-rw-rw-   0        0        0     4911 2024-06-02 07:42:19.891422 real_time_translator-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3885 2024-06-02 06:17:20.000000 real_time_translator-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 07:42:19.890525 real_time_translator-0.1.1/real_time_translator.egg-info/
+-rw-rw-rw-   0        0        0     4911 2024-06-02 07:42:19.000000 real_time_translator-0.1.1/real_time_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-06-02 07:42:19.000000 real_time_translator-0.1.1/real_time_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:42:19.000000 real_time_translator-0.1.1/real_time_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-06-02 07:42:19.000000 real_time_translator-0.1.1/real_time_translator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-06-02 07:42:19.000000 real_time_translator-0.1.1/real_time_translator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:42:19.000000 real_time_translator-0.1.1/real_time_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 07:42:19.892420 real_time_translator-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1331 2024-06-02 07:41:57.000000 real_time_translator-0.1.1/setup.py
```

### Comparing `real_time_translator-0.1.0/PKG-INFO` & `real_time_translator-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: real_time_translator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A real-time audio translator using Azure Cognitive Services and PyQt5
-Home-page: https://github.com/your-repo/real-time-translator
+Home-page: https://github.com/jpshag/real-time-translator
 Author: Your Name
-Author-email: your-email@example.com
+Author-email: jpshag@proton.me
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `real_time_translator-0.1.0/README.md` & `real_time_translator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `real_time_translator-0.1.0/real_time_translator.egg-info/PKG-INFO` & `real_time_translator-0.1.1/real_time_translator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: real_time_translator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A real-time audio translator using Azure Cognitive Services and PyQt5
-Home-page: https://github.com/your-repo/real-time-translator
+Home-page: https://github.com/jpshag/real-time-translator
 Author: Your Name
-Author-email: your-email@example.com
+Author-email: jpshag@proton.me
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `real_time_translator-0.1.0/setup.py` & `real_time_translator-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='real_time_translator',
-    version='0.1.0',
+    version='0.1.1',
     description='A real-time audio translator using Azure Cognitive Services and PyQt5',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/your-repo/real-time-translator',
+    url='https://github.com/jpshag/real-time-translator',
     author='Your Name',
-    author_email='your-email@example.com',
+    author_email='jpshag@proton.me',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'PyQt5',
         'pyaudio',
         'numpy',
         'scipy',
```

