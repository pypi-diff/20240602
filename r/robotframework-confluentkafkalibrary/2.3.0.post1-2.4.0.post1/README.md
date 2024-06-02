# Comparing `tmp/robotframework_confluentkafkalibrary-2.3.0.post1.tar.gz` & `tmp/robotframework_confluentkafkalibrary-2.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_confluentkafkalibrary-2.3.0.post1.tar", last modified: Sat Apr 20 20:50:58 2024, max compression
+gzip compressed data, was "robotframework_confluentkafkalibrary-2.4.0.post1.tar", last modified: Sun Jun  2 06:14:33 2024, max compression
```

## Comparing `robotframework_confluentkafkalibrary-2.3.0.post1.tar` & `robotframework_confluentkafkalibrary-2.4.0.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.422298 robotframework_confluentkafkalibrary-2.3.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-20 20:50:58.418298 robotframework_confluentkafkalibrary-2.3.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:50:58.422298 robotframework_confluentkafkalibrary-2.3.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.414298 robotframework_confluentkafkalibrary-2.3.0.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.418298 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 20:50:52.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:50:58.418298 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:50:58.000000 robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:14:33.762705 robotframework_confluentkafkalibrary-2.4.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-06-02 06:14:33.762705 robotframework_confluentkafkalibrary-2.4.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 06:14:33.762705 robotframework_confluentkafkalibrary-2.4.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:14:33.758705 robotframework_confluentkafkalibrary-2.4.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:14:33.758705 robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 06:14:26.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:14:33.762705 robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-06-02 06:14:33.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-02 06:14:33.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:14:33.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-02 06:14:33.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 06:14:33.000000 robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
```

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/LICENSE` & `robotframework_confluentkafkalibrary-2.4.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/PKG-INFO` & `robotframework_confluentkafkalibrary-2.4.0.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.3.0.post1
+Version: 2.4.0.post1
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE
 Requires-Dist: robotframework>=3.2.1
-Requires-Dist: confluent-kafka==2.3.0
+Requires-Dist: confluent-kafka==2.4.0
 Requires-Dist: requests>=2.25.1
 Provides-Extra: all
 Requires-Dist: fastavro>=1.3.2; extra == "all"
 Requires-Dist: avro>=1.11.1; extra == "all"
 Requires-Dist: fastavro>=1.3.2; extra == "all"
 Requires-Dist: avro-python3>=1.10.1; extra == "all"
 Requires-Dist: jsonschema>=3.2.0; extra == "all"
```

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/README.md` & `robotframework_confluentkafkalibrary-2.4.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/setup.py` & `robotframework_confluentkafkalibrary-2.4.0.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
           "License :: OSI Approved :: Apache Software License",
           "Operating System :: OS Independent",
           "Programming Language :: Python",
           "Topic :: Software Development :: Testing"
       ],
       install_requires = [
           'robotframework >= 3.2.1',
-          'confluent-kafka == 2.3.0',
+          'confluent-kafka == 2.4.0',
           'requests >= 2.25.1',
       ],
       extras_require={
           'all': ALL,
           'avro': AVRO_REQUIRES,
           'legacyavro': LEGACYAVRO_REQUIRES,
           'json': JSON_REQUIRES,
```

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/__init__.py` & `robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/admin_client.py` & `robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/admin_client.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/consumer.py` & `robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/consumer.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/producer.py` & `robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/producer.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/src/ConfluentKafkaLibrary/serialization.py` & `robotframework_confluentkafkalibrary-2.4.0.post1/src/ConfluentKafkaLibrary/serialization.py`

 * *Files identical despite different names*

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO` & `robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.3.0.post1
+Version: 2.4.0.post1
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE
 Requires-Dist: robotframework>=3.2.1
-Requires-Dist: confluent-kafka==2.3.0
+Requires-Dist: confluent-kafka==2.4.0
 Requires-Dist: requests>=2.25.1
 Provides-Extra: all
 Requires-Dist: fastavro>=1.3.2; extra == "all"
 Requires-Dist: avro>=1.11.1; extra == "all"
 Requires-Dist: fastavro>=1.3.2; extra == "all"
 Requires-Dist: avro-python3>=1.10.1; extra == "all"
 Requires-Dist: jsonschema>=3.2.0; extra == "all"
```

### Comparing `robotframework_confluentkafkalibrary-2.3.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt` & `robotframework_confluentkafkalibrary-2.4.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

