# Comparing `tmp/cndi-2.4.3.tar.gz` & `tmp/cndi-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cndi-2.4.3.tar", last modified: Sun Mar 24 18:48:03 2024, max compression
+gzip compressed data, was "cndi-2.4.4.tar", last modified: Sun Jun  2 00:20:34 2024, max compression
```

## Comparing `cndi-2.4.3.tar` & `cndi-2.4.4.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.569797 cndi-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-24 18:47:59.000000 cndi-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-24 18:48:03.569797 cndi-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-24 18:47:59.000000 cndi-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.561797 cndi-2.4.3/cndi/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/annotations/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/annotations/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/annotations/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/binders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/binders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/binders/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/binders/message/
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/binders/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/binders/message/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/binders/message/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/binders/message/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/events/
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/exception/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/flask/flask_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/http/management/
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/http/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/minio/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/minio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/rasa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/rasa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/rasa/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-24 18:47:59.000000 cndi-2.4.3/cndi/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/cndi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-24 18:48:03.000000 cndi-2.4.3/cndi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-24 18:48:03.000000 cndi-2.4.3/cndi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:48:03.000000 cndi-2.4.3/cndi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-24 18:48:03.000000 cndi-2.4.3/cndi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:48:03.569797 cndi-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-24 18:47:59.000000 cndi-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/tests/cndi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/cndi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/tests/cndi/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/cndi/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/cndi/annotations/test_app_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/cndi/annotations/test_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/tests/cndi/binders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/cndi/binders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:48:03.565797 cndi-2.4.3/tests/cndi/binders/message/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/cndi/binders/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-24 18:47:59.000000 cndi-2.4.3/tests/test_load_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-06-02 00:20:30.000000 cndi-2.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-06-02 00:20:34.463204 cndi-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-06-02 00:20:30.000000 cndi-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/annotations/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/annotations/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/annotations/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/binders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/binders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/binders/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/binders/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/binders/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/binders/message/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/binders/message/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/binders/message/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/flask/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/healthchecks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.459204 cndi-2.4.4/cndi/http/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/http/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/cndi/minio/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/minio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/cndi/rasa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/rasa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/rasa/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/cndi/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 00:20:30.000000 cndi-2.4.4/cndi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/cndi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-06-02 00:20:34.000000 cndi-2.4.4/cndi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-02 00:20:34.000000 cndi-2.4.4/cndi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:20:34.000000 cndi-2.4.4/cndi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 00:20:34.000000 cndi-2.4.4/cndi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:20:34.463204 cndi-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-02 00:20:30.000000 cndi-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/tests/cndi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/cndi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/tests/cndi/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/cndi/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/cndi/annotations/test_app_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/cndi/annotations/test_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/tests/cndi/binders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/cndi/binders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:20:34.463204 cndi-2.4.4/tests/cndi/binders/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/cndi/binders/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-02 00:20:30.000000 cndi-2.4.4/tests/test_load_envs.py
```

### Comparing `cndi-2.4.3/LICENSE` & `cndi-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/PKG-INFO` & `cndi-2.4.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cndi
-Version: 2.4.3
+Version: 2.4.4
 Author: Mayank Shinde
 Author-email: mayank31313@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cndi-2.4.3/README.md` & `cndi-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/annotations/__init__.py` & `cndi-2.4.4/cndi/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/annotations/events.py` & `cndi-2.4.4/cndi/annotations/events.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/binders/message/__init__.py` & `cndi-2.4.4/cndi/binders/message/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.message = message
         return self
 
     def setKey(self, key):
         self.key = key
         return self
 
+
 def Input(channelName):
     def inner_function(func):
         CHANNELS_TO_FUNC_MAP[channelName] = dict(func=func, annotations=func.__annotations__, is_sink=False)
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
         return wrapper
@@ -47,22 +48,22 @@
 def _conditionalRenderDefaultMessageBinder(wrapper):
     defaultMessageBinder = getContextEnvironment("rcn.binders.message.enable",  defaultValue=False, castFunc=bool)
     return defaultMessageBinder
 
 @Component
 @ConditionalRendering(callback=_conditionalRenderDefaultMessageBinder)
 class DefaultMessageBinder:
-    def   __init__(self):
+    def __init__(self):
         self.logger = logging.getLogger('.'.join([self.__class__.__module__, self.__class__.__name__]))
 
         self.binders = dict()
         self.topicConsumers = dict()
         self.callbacks = list()
         self.defaultMessageBinder = getContextEnvironment("rcn.binders.message.default")
-        self.initializeBinders()
+        self.channelBinders = self.initializeBinders()
 
     def start(self):
         for callback in self.callbacks:
             callback()
 
     def performInjection(self):
         for channelName, methodWrapper in CHANNELS_TO_FUNC_MAP.items():
@@ -75,24 +76,26 @@
                 method = methodWrapper['func']
                 methodsClassFullname = f"{method.__module__}.{method.__qualname__.split('.')[0]}"
                 classBean = getBeanObject(methodsClassFullname)
                 method(classBean, binder)
 
     def initializeBinders(self):
         contextEnvs = getContextEnvironments()
-
+        channelBinders = dict()
         if self.defaultMessageBinder.strip().lower() == "rabbitmq":
             from cndi.binders.message.rabbitmq import RabbitMQProducerBinding, RabbitMQBinder
 
             rabbitMqBinder = RabbitMQBinder()
 
             self.binders.update(rabbitMqBinder.bindProducers())
             self.binders.update(rabbitMqBinder.bindSubscribers(CHANNELS_TO_FUNC_MAP=CHANNELS_TO_FUNC_MAP))
             self.callbacks.append(rabbitMqBinder.channelThread.start)
 
+            channelBinders[rabbitMqBinder.name()] = rabbitMqBinder
+
         elif self.defaultMessageBinder.strip().lower() == "mqtt":
             from cndi.binders.message.mqtt import MqttProducerBinding
             from paho.mqtt.client import Client, MQTTMessage
 
             brokerUrl = getContextEnvironment(f"{RCN_MESSAGE_BINDERS}.mqtt.brokerUrl", defaultValue=None)
             brokerPort = getContextEnvironment(f"{RCN_MESSAGE_BINDERS}.mqtt.brokerPort", defaultValue=None)
 
@@ -140,8 +143,10 @@
             def on_message(client, userdata, msg: MQTTMessage):
                 self.topicConsumers[msg.topic](msg)
 
             mqttClient.on_connect = on_connect
             mqttClient.on_message = on_message
 
             mqttClient.connect(brokerUrl, brokerPort)
-            self.callbacks.append(mqttClient.loop_start)
+            self.callbacks.append(mqttClient.loop_start)
+
+        return channelBinders
```

### Comparing `cndi-2.4.3/cndi/binders/message/rabbitmq.py` & `cndi-2.4.4/cndi/binders/message/rabbitmq.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,15 +42,19 @@
     def setTopic(self, topic, group="", channelName=None):
         SubscriberChannel.setTopic(self, topic)
         self.channel.queue_declare(queue=topic  + group)
         self.channel.queue_bind(exchange=topic, queue=topic + group, routing_key="#")
 
 
 
-class RabbitMQBinder():
+class RabbitMQBinder:
+    @staticmethod
+    def name():
+        return "rabbitmq"
+
     def __init__(self):
         self.logger = logging.getLogger('.'.join([self.__class__.__module__, self.__class__.__name__]))
         brokerUrl = getContextEnvironment("rcn.binders.message.rabbitmq.brokerUrl", defaultValue=None)
         brokerPort = getContextEnvironment("rcn.binders.message.rabbitmq.brokerPort", defaultValue=None)
 
         brokerUrl = getContextEnvironment("rcn.binders.message.brokerUrl", required=True, defaultValue=brokerUrl)
         brokerPort = getContextEnvironment("rcn.binders.message.brokerPort", required=True, castFunc=int,
@@ -67,18 +71,39 @@
         self.mqttConsumerChannelBindings = filter(
             lambda key: key.startswith('rcn.binders.message.rabbitmq.consumer') and key.endswith("destination"),
             contextEnvs)
         self.CHANNELS_TO_TOPIC_MAP = dict()
         self.channel = self.connection.channel()
 
         self.channelThread = Thread(target=self.channel.start_consuming)
+        self.producers = {}
+        self.consumers = {}
 
     def stopConsumers(self):
         self.channel.stop_consuming()
 
+    def info(self):
+        producers = []
+        consumers = []
+        for channel, producerBinding in self.producers.items():
+            producers.append(dict(
+                channel=channel,
+                topic=producerBinding.topic
+            ))
+
+        for channel, consumerBinding in self.consumers.items():
+            consumers.append(dict(
+                channel = channel
+            ))
+        return dict(
+            producers = producers
+        )
+    def health(self):
+        return self.channel.is_open and self.connection.is_open
+
     def bindSubscribers(self, CHANNELS_TO_FUNC_MAP):
         subscriptionTopics = list()
         topicConsumers = dict()
         binders = dict()
 
         def consumerMessage(ch: BlockingChannel, method: Basic.Deliver, properties, body):
             topicConsumers[method.exchange](body)
@@ -104,22 +129,23 @@
                 raise KeyError(f"Duplicate topic found {topicName} with {topicConsumers[topicName]}")
 
             topicConsumers[topicName] = consumerBinding
             binders[channelName] = consumerBinding
 
             self.channel.basic_consume(queue=topicName + consumerGroup, auto_ack=True, on_message_callback=consumerMessage)
 
+        self.consumers = binders
         return binders
 
     def bindProducers(self):
         binders = dict()
         for propertyKey in self.rabbotmqProducerChannelBindings:
             channelName = extractChannelNameFromPropertyKey(propertyKey)
             producerBinding = RabbitMQProducerBinding(connection=self.connection)
 
             topicName = getContextEnvironment(propertyKey, required=True)
             self.logger.info("Topic Name: "  + topicName)
             producerBinding.setTopic(topicName)
             self.CHANNELS_TO_TOPIC_MAP[channelName] = topicName
             binders[channelName] = producerBinding
-
+        self.producers=binders
         return binders
```

### Comparing `cndi-2.4.3/cndi/binders/message/utils.py` & `cndi-2.4.4/cndi/binders/message/utils.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/env.py` & `cndi-2.4.4/cndi/env.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/events/__init__.py` & `cndi-2.4.4/cndi/events/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/flask/flask_app.py` & `cndi-2.4.4/cndi/flask/flask_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     This function checks the environment for a variable named 'app.flask.enabled'. If the variable is set to 'True', the function returns True. If the variable is not set or is set to any other value, the function returns False.
 
     Returns:
         True if Flask is enabled, False otherwise.
     """
     try:
         from flask import Flask
-        return getContextEnvironment(RCN_FLASK_APP_ENABLED, castFunc=bool, defaultValue=False);
+        return getContextEnvironment(RCN_FLASK_APP_ENABLED, castFunc=bool, defaultValue=False) \
+            and ContextThreads.isEnabled(f"{FlaskApplication.__module__}.{FlaskApplication.__qualname__}")
     except ImportError:
         return False
 
 @Component
 @ConditionalRendering(callback=__check_flask_enabled__)
 class FlaskApplication:
     """
```

### Comparing `cndi-2.4.3/cndi/http/__init__.py` & `cndi-2.4.4/cndi/http/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/http/management/__init__.py` & `cndi-2.4.4/cndi/http/management/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import threading
 
 
 from cndi.annotations import beans, Component, getBeanObject, ConditionalRendering
 from cndi.annotations.threads import ContextThreads
 from cndi.env import getContextEnvironment
+from cndi.healthchecks import BeanHealthChecker, ChannelHealthChecker
 from cndi.utils import logger
 
 def managementServerSupported(x):
     try:
         from flask import Flask
         from werkzeug.serving import run_simple
-        return getContextEnvironment("rcn.management.server.enabled", defaultValue=False, castFunc=bool)
+        return getContextEnvironment("rcn.management.server.enabled", defaultValue=False, castFunc=bool) \
+            and ContextThreads.isEnabled(f"{ManagementServer.__module__}.{ManagementServer.__qualname__}")
     except ImportError:
         return False
 
 @Component
 @ConditionalRendering(callback=managementServerSupported)
 class ManagementServer:
+    def __init__(self, channelHealthChecker: ChannelHealthChecker):
+        self.healthChecker = BeanHealthChecker()
+        self.channelHealthChecker = channelHealthChecker
+
     def registerEndpoints(self, flaskApp):
         from flask import jsonify
 
         @flaskApp.route("/health")
         def health():
             return jsonify(status="OK")
 
@@ -28,18 +34,26 @@
         def managementBeans():
             targetResponse = list()
             for bean in beans:
                 targetResponse.append({
                     "name": bean['name'],
                     'newInstance': bean['newInstance'],
                     'fullname': bean['fullname'],
-                    'index': bean['index']
+                    'index': bean['index'],
+                    "health": None if bean['newInstance'] else self.healthChecker.check(bean['name'])
                 })
             return jsonify(beans=targetResponse)
 
+        @flaskApp.route("/management/channels")
+        def managementChannels():
+            return jsonify(
+                channels=self.channelHealthChecker.check()
+            )
+
+
     def run(self):
         from flask import Flask
         from werkzeug.serving import run_simple
 
         host = getContextEnvironment("rcn.management.server.host", defaultValue="0.0.0.0")
         port = getContextEnvironment("rcn.management.server.port", defaultValue=9000, castFunc=int)
```

### Comparing `cndi-2.4.3/cndi/initializers.py` & `cndi-2.4.4/cndi/initializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 
 from cndi.annotations import beanStore, workOrder, beans, components, componentStore, autowires, getBeanObject, getBean, \
     validateBean, queryOverideBeanStore, validatedBeans
 from cndi.env import loadEnvFromFile, getContextEnvironment
 from cndi.flask.flask_app import FlaskApplication
 from cndi.http.management import ManagementServer
 from cndi.utils import importSubModules
+from cndi.version import VERSION
 
 logger = logging.getLogger(__name__)
 
 initializerComponents = [
     '.'.join([ManagementServer.__module__, ManagementServer.__name__]),
     '.'.join([FlaskApplication.__module__, FlaskApplication.__name__])
 ]
 
 class AppInitializer:
     def __init__(self):
         """
         Responsible to initialise Dependency Injection for Application
         """
+        logger.info(f"CNDI Version: v{VERSION}")
         self.componentsPath = list()
         applicationYml = "resources/application.yml"
-        self.managementServer = ManagementServer()
 
         if os.path.exists(applicationYml):
             logger.info(f"External Configuration found: {applicationYml}")
             loadEnvFromFile(applicationYml)
 
 
     def componentScan(self, module):
@@ -103,15 +104,15 @@
                                                  object=objectInstance, index=0, newInstance=False,
                                                  fullname=component.func.__name__, kwargs=kwargs)
 
         messageBinderEnabled = getContextEnvironment("rcn.binders.message.enable", defaultValue=False, castFunc=bool)
         defaultMessageBinder = None
 
         if messageBinderEnabled:
-            defaultMessageBinder = DefaultMessageBinder()
+            defaultMessageBinder = getBeanObject(".".join([DefaultMessageBinder.__module__, DefaultMessageBinder.__name__]))
             defaultMessageBinder.performInjection()
 
         for autowire in autowires:
             autowire.dependencyInject()
 
         if defaultMessageBinder is not None:
             defaultMessageBinder.start()
```

### Comparing `cndi-2.4.3/cndi/minio/__init__.py` & `cndi-2.4.4/cndi/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/rasa/configs.py` & `cndi-2.4.4/cndi/rasa/configs.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/resources.py` & `cndi-2.4.4/cndi/resources.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi/utils.py` & `cndi-2.4.4/cndi/utils.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/cndi.egg-info/PKG-INFO` & `cndi-2.4.4/cndi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cndi
-Version: 2.4.3
+Version: 2.4.4
 Author: Mayank Shinde
 Author-email: mayank31313@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cndi-2.4.3/cndi.egg-info/SOURCES.txt` & `cndi-2.4.4/cndi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
 setup.py
 cndi/__init__.py
 cndi/consts.py
 cndi/env.py
+cndi/healthchecks.py
 cndi/initializers.py
 cndi/resources.py
 cndi/utils.py
+cndi/version.py
 cndi.egg-info/PKG-INFO
 cndi.egg-info/SOURCES.txt
 cndi.egg-info/dependency_links.txt
 cndi.egg-info/top_level.txt
 cndi/annotations/__init__.py
 cndi/annotations/component.py
 cndi/annotations/events.py
```

### Comparing `cndi-2.4.3/setup.py` & `cndi-2.4.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "2.4.3"
+from cndi.version import VERSION
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cndi",
     version=VERSION,
```

### Comparing `cndi-2.4.3/tests/cndi/annotations/test_app_initializer.py` & `cndi-2.4.4/tests/cndi/annotations/test_app_initializer.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/tests/cndi/annotations/test_components.py` & `cndi-2.4.4/tests/cndi/annotations/test_components.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/tests/cndi/binders/message/__init__.py` & `cndi-2.4.4/tests/cndi/binders/message/__init__.py`

 * *Files identical despite different names*

### Comparing `cndi-2.4.3/tests/test_load_envs.py` & `cndi-2.4.4/tests/test_load_envs.py`

 * *Files identical despite different names*

