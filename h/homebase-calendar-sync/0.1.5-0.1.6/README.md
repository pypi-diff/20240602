# Comparing `tmp/homebase_calendar_sync-0.1.5.tar.gz` & `tmp/homebase_calendar_sync-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homebase_calendar_sync-0.1.5.tar", last modified: Sun Jun  2 16:09:27 2024, max compression
+gzip compressed data, was "homebase_calendar_sync-0.1.6.tar", last modified: Sun Jun  2 17:12:39 2024, max compression
```

## Comparing `homebase_calendar_sync-0.1.5.tar` & `homebase_calendar_sync-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 16:09:27.835197 homebase_calendar_sync-0.1.5/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 16:09:27.834965 homebase_calendar_sync-0.1.5/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)      477 2024-06-02 14:42:53.000000 homebase_calendar_sync-0.1.5/README.md
--rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-02 16:09:27.835261 homebase_calendar_sync-0.1.5/setup.cfg
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-02 16:08:59.000000 homebase_calendar_sync-0.1.5/setup.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 16:09:27.829290 homebase_calendar_sync-0.1.5/src/
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 16:09:27.830501 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:29.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      123 2024-06-02 13:40:44.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/config.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 16:09:27.831996 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/db/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/db/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/db/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      872 2024-06-02 15:58:26.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/db/models.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 16:09:27.833940 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/__init__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/__main__.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    17970 2024-06-02 15:59:07.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/auth.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/drive_types.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)     9124 2024-06-02 15:59:34.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/google_client.py
--rw-r--r--   0 davidmidlo   (501) staff       (20)    13109 2024-06-02 16:05:07.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/homebase_calendar_sync.py
-drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 16:09:27.834556 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/
--rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 16:09:27.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/PKG-INFO
--rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-02 16:09:27.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/SOURCES.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-02 16:09:27.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/dependency_links.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-02 16:09:27.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/entry_points.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)     1080 2024-06-02 16:09:27.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/requires.txt
--rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-02 16:09:27.000000 homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/top_level.txt
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.365757 homebase_calendar_sync-0.1.6/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:12:39.365549 homebase_calendar_sync-0.1.6/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      477 2024-06-02 14:42:53.000000 homebase_calendar_sync-0.1.6/README.md
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       38 2024-06-02 17:12:39.365799 homebase_calendar_sync-0.1.6/setup.cfg
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1009 2024-06-02 17:12:24.000000 homebase_calendar_sync-0.1.6/setup.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.361645 homebase_calendar_sync-0.1.6/src/
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.362657 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:29.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 13:57:40.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      123 2024-06-02 13:40:44.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/config.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.363832 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:10.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:19.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      872 2024-06-02 15:58:26.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/models.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.364917 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:33.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/__init__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        0 2024-06-02 14:47:49.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/__main__.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    17970 2024-06-02 15:59:07.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/auth.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      106 2024-06-02 04:40:28.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/drive_types.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     9124 2024-06-02 15:59:34.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/google_client.py
+-rw-r--r--   0 davidmidlo   (501) staff       (20)    13108 2024-06-02 17:11:16.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/homebase_calendar_sync.py
+drwxr-xr-x   0 davidmidlo   (501) staff       (20)        0 2024-06-02 17:12:39.365211 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     2927 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/PKG-INFO
+-rw-r--r--   0 davidmidlo   (501) staff       (20)      881 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)        1 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       94 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/entry_points.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)     1080 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/requires.txt
+-rw-r--r--   0 davidmidlo   (501) staff       (20)       23 2024-06-02 17:12:39.000000 homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/top_level.txt
```

### Comparing `homebase_calendar_sync-0.1.5/PKG-INFO` & `homebase_calendar_sync-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homebase_calendar_sync
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple web scraper that reads gethomebase.com's schedule and updates Google Calendar.
 Home-page: https://github.com/dmidlo/homebase_calendar_sync
 Author: David Midlo
 Author-email: dmidlo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `homebase_calendar_sync-0.1.5/setup.py` & `homebase_calendar_sync-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from setuptools import setup, find_packages
 
 setup(
     name='homebase_calendar_sync',
-    version='0.1.5',
+    version='0.1.6',
     author='David Midlo',
     author_email='dmidlo@gmail.com',
     description='A simple web scraper that reads gethomebase.com\'s schedule and updates Google Calendar.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dmidlo/homebase_calendar_sync',  # Update this to your project's URL
     packages=find_packages(where='src'),
```

### Comparing `homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/db/models.py` & `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/db/models.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/auth.py` & `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/auth.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/google_client/google_client.py` & `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/google_client/google_client.py`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.5/src/homebase_calendar_sync/homebase_calendar_sync.py` & `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync/homebase_calendar_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,8 +349,7 @@
         config.DB.commit()
         self.update_events_db_from_remote()
 
 
 def main():
     sync = HomebaseCalendarSync()
     sync()
-
```

### Comparing `homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/PKG-INFO` & `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homebase_calendar_sync
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple web scraper that reads gethomebase.com's schedule and updates Google Calendar.
 Home-page: https://github.com/dmidlo/homebase_calendar_sync
 Author: David Midlo
 Author-email: dmidlo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/SOURCES.txt` & `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homebase_calendar_sync-0.1.5/src/homebase_calendar_sync.egg-info/requires.txt` & `homebase_calendar_sync-0.1.6/src/homebase_calendar_sync.egg-info/requires.txt`

 * *Files identical despite different names*

