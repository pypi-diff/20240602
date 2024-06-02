# Comparing `tmp/netband-2.1.4b1.tar.gz` & `tmp/netband-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netband-2.1.4b1.tar", last modified: Sun Jun  2 15:28:23 2024, max compression
+gzip compressed data, was "netband-2.1.5.tar", last modified: Sun Jun  2 16:27:47 2024, max compression
```

## Comparing `netband-2.1.4b1.tar` & `netband-2.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2024-06-02 15:28:23.467635 netband-2.1.4b1/
--rw-r--r--   0 aniket     (501) staff       (20)    11358 2024-06-02 14:33:35.000000 netband-2.1.4b1/LICENSE
--rw-r--r--   0 aniket     (501) staff       (20)       35 2024-06-02 15:21:25.000000 netband-2.1.4b1/MANIFEST.in
--rw-r--r--   0 aniket     (501) staff       (20)     1385 2024-06-02 15:28:23.467548 netband-2.1.4b1/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)       76 2024-06-02 15:21:22.000000 netband-2.1.4b1/README.md
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2024-06-02 15:28:23.467260 netband-2.1.4b1/netband.egg-info/
--rw-r--r--   0 aniket     (501) staff       (20)     1385 2024-06-02 15:28:23.000000 netband-2.1.4b1/netband.egg-info/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)      219 2024-06-02 15:28:23.000000 netband-2.1.4b1/netband.egg-info/SOURCES.txt
--rw-r--r--   0 aniket     (501) staff       (20)        1 2024-06-02 15:28:23.000000 netband-2.1.4b1/netband.egg-info/dependency_links.txt
--rw-r--r--   0 aniket     (501) staff       (20)       43 2024-06-02 15:28:23.000000 netband-2.1.4b1/netband.egg-info/entry_points.txt
--rw-r--r--   0 aniket     (501) staff       (20)       10 2024-06-02 15:28:23.000000 netband-2.1.4b1/netband.egg-info/top_level.txt
--rw-r--r--   0 aniket     (501) staff       (20)       61 2024-06-02 15:28:23.467915 netband-2.1.4b1/setup.cfg
--rw-r--r--   0 aniket     (501) staff       (20)     3460 2024-06-02 15:27:19.000000 netband-2.1.4b1/setup.py
--rwxr-xr-x   0 aniket     (501) staff       (20)    65381 2024-06-02 15:24:59.000000 netband-2.1.4b1/speedtest.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2024-06-02 16:27:47.589440 netband-2.1.5/
+-rw-r--r--   0 aniket     (501) staff       (20)    11358 2024-06-02 14:33:35.000000 netband-2.1.5/LICENSE
+-rw-r--r--   0 aniket     (501) staff       (20)       35 2024-06-02 16:24:48.000000 netband-2.1.5/MANIFEST.in
+-rw-r--r--   0 aniket     (501) staff       (20)     1391 2024-06-02 16:27:47.589354 netband-2.1.5/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)      447 2024-06-02 16:07:04.000000 netband-2.1.5/README.md
+-rw-r--r--   0 aniket     (501) staff       (20)     3090 2024-06-02 16:23:37.000000 netband-2.1.5/netband.1
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2024-06-02 16:27:47.589065 netband-2.1.5/netband.egg-info/
+-rw-r--r--   0 aniket     (501) staff       (20)     1391 2024-06-02 16:27:47.000000 netband-2.1.5/netband.egg-info/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)      227 2024-06-02 16:27:47.000000 netband-2.1.5/netband.egg-info/SOURCES.txt
+-rw-r--r--   0 aniket     (501) staff       (20)        1 2024-06-02 16:27:47.000000 netband-2.1.5/netband.egg-info/dependency_links.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       41 2024-06-02 16:27:47.000000 netband-2.1.5/netband.egg-info/entry_points.txt
+-rw-r--r--   0 aniket     (501) staff       (20)        8 2024-06-02 16:27:47.000000 netband-2.1.5/netband.egg-info/top_level.txt
+-rwxr-xr-x   0 aniket     (501) staff       (20)    65379 2024-06-02 16:27:14.000000 netband-2.1.5/netband.py
+-rw-r--r--   0 aniket     (501) staff       (20)       61 2024-06-02 16:27:47.589741 netband-2.1.5/setup.cfg
+-rw-r--r--   0 aniket     (501) staff       (20)     3508 2024-06-02 16:27:36.000000 netband-2.1.5/setup.py
```

### Comparing `netband-2.1.4b1/LICENSE` & `netband-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netband-2.1.4b1/PKG-INFO` & `netband-2.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: netband
-Version: 2.1.4b1
+Version: 2.1.5
 Summary: Command line interface for testing internet bandwidth using speedtest.net
 Home-page: https://github.com/xunicatt/netband
 Author: Aniket Biswas
 Author-email: contact.aniket.biswas@gmail.com
 License: Apache License, Version 2.0
-Keywords: speedtest speedtest.net
+Keywords: netband speedtest speedtest.net
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.4
```

### Comparing `netband-2.1.4b1/netband.egg-info/PKG-INFO` & `netband-2.1.5/netband.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: netband
-Version: 2.1.4b1
+Version: 2.1.5
 Summary: Command line interface for testing internet bandwidth using speedtest.net
 Home-page: https://github.com/xunicatt/netband
 Author: Aniket Biswas
 Author-email: contact.aniket.biswas@gmail.com
 License: Apache License, Version 2.0
-Keywords: speedtest speedtest.net
+Keywords: netband speedtest speedtest.net
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.4
```

### Comparing `netband-2.1.4b1/setup.py` & `netband-2.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,29 +56,30 @@
 except:
     long_description = ''
 
 
 setup(
     #new project name
     name='netband',
-    version=find_version('speedtest.py'),
+    version=find_version('netband.py'),
     description=('Command line interface for testing internet bandwidth using '
                  'speedtest.net'),
     long_description=long_description,
-    keywords='speedtest speedtest.net',
+    keywords='netband speedtest speedtest.net',
     author='Aniket Biswas',
     author_email='contact.aniket.biswas@gmail.com',
     url='https://github.com/xunicatt/netband',
     license='Apache License, Version 2.0',
-    py_modules=['speedtest'],
+    py_modules=['netband'],
     entry_points={
         'console_scripts': [
-            'netband=speedtest:main'
+            'netband=netband:main'
         ]
     },
+    data_files=[('man/man1', ['netband.1'])],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Environment :: Console',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2',
```

### Comparing `netband-2.1.4b1/speedtest.py` & `netband-2.1.5/netband.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 try:
     import gzip
     GZIP_BASE = gzip.GzipFile
 except ImportError:
     gzip = None
     GZIP_BASE = object
 
-__version__ = '2.1.4b1'
+__version__ = '2.1.5'
 
 
 class FakeShutdownEvent(object):
     """Class to fake a threading.Event.isSet so that users of this module
     are not required to register their own threading.Event()
     """
```

