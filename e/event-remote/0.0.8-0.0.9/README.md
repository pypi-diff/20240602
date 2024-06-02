# Comparing `tmp/event-remote-0.0.8.tar.gz` & `tmp/event-remote-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event-remote-0.0.8.tar", last modified: Tue Dec 12 16:19:53 2023, max compression
+gzip compressed data, was "event-remote-0.0.9.tar", last modified: Wed Dec 13 09:12:21 2023, max compression
```

## Comparing `event-remote-0.0.8.tar` & `event-remote-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:19:53.074832 event-remote-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-12 16:19:53.074832 event-remote-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:19:53.074832 event-remote-0.0.8/event_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:19:53.074832 event-remote-0.0.8/event_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 16:19:20.000000 event-remote-0.0.8/event_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-12 16:19:20.000000 event-remote-0.0.8/event_remote/src/event_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2023-12-12 16:19:20.000000 event-remote-0.0.8/event_remote/src/remote_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-12 16:19:20.000000 event-remote-0.0.8/event_remote/src/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 16:19:53.074832 event-remote-0.0.8/event_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-12 16:19:53.000000 event-remote-0.0.8/event_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-12 16:19:53.000000 event-remote-0.0.8/event_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 16:19:53.000000 event-remote-0.0.8/event_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-12 16:19:53.000000 event-remote-0.0.8/event_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-12 16:19:53.000000 event-remote-0.0.8/event_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-12 16:19:20.000000 event-remote-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 16:19:53.074832 event-remote-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-12 16:19:20.000000 event-remote-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:12:21.702689 event-remote-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-13 09:12:21.702689 event-remote-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:12:21.698689 event-remote-0.0.9/event_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:12:21.702689 event-remote-0.0.9/event_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 09:11:45.000000 event-remote-0.0.9/event_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-13 09:11:45.000000 event-remote-0.0.9/event_remote/src/event_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-13 09:11:45.000000 event-remote-0.0.9/event_remote/src/event_remote_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2023-12-13 09:11:45.000000 event-remote-0.0.9/event_remote/src/remote_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 09:12:21.702689 event-remote-0.0.9/event_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2023-12-13 09:12:21.000000 event-remote-0.0.9/event_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-13 09:12:21.000000 event-remote-0.0.9/event_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 09:12:21.000000 event-remote-0.0.9/event_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-13 09:12:21.000000 event-remote-0.0.9/event_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-13 09:12:21.000000 event-remote-0.0.9/event_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-13 09:11:45.000000 event-remote-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 09:12:21.702689 event-remote-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-13 09:11:45.000000 event-remote-0.0.9/setup.py
```

### Comparing `event-remote-0.0.8/PKG-INFO` & `event-remote-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-remote
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles event-remote Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `event-remote-0.0.8/event_remote/src/event_constants.py` & `event-remote-0.0.9/event_remote/src/event_constants.py`

 * *Files identical despite different names*

### Comparing `event-remote-0.0.8/event_remote/src/remote_event.py` & `event-remote-0.0.9/event_remote/src/remote_event.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from sdk.src.utilities import create_http_headers
-from .util import EventRemoteUtil
+from .event_remote_util import EventRemoteUtil
 from url_local.url_circlez import OurUrl
 from url_local.action_name_enum import ActionName
 from url_local.entity_name_enum import EntityName
 from url_local.component_name_enum import ComponentName
 from logger_local.Logger import Logger
 from .event_constants import EventRemoteConstants
 import copy
@@ -71,27 +71,31 @@
             self.logger.end(
                 f"End create event-remote, response: {str(response)}")
             return response
 
         except requests.ConnectionError as e:
             self.logger.exception(
                 "Network problem (e.g. failed to connect)", object=e)
+            self.logger.end("End create event-remote, connection error exception")  # noqa
             raise
 
         except requests.Timeout as e:
             self.logger.exception("Request timed out", e)
+            self.logger.end("End create event-remote, timeout exception")  # noqa
             raise
 
         except requests.RequestException as e:
             self.logger.exception(f"General error: {str(e)}", object=e)
+            self.logger.end("End create event-remote, request exception")  # noqa
             raise
 
         except Exception as e:
             self.logger.exception(
                 f"An unexpected error occurred: {str(e)}", object=e)
+            self.logger.end("End create event-remote, general exception")  # noqa
             raise
 
     def create_external_events(self, external_events_details: list):
         external_events = {
             'external_events_details': external_events_details
         }
         self.logger.start("Start create external events",
@@ -116,33 +120,37 @@
                                                                       subsystem_id=external_event.get('subsystem_id', None),  # noqa
                                                                       url=external_event.get('url'),  # noqa
                                                                       external_event_identifier=external_event.get('external_event_identifier'),  # noqa
                                                                       environment_id=external_event.get('environment_id', 1))  # noqa
                 # TODO add list of event_id and external_id list to return
                 # should be here insert into event_external_event_table
 
-            self.logger.end("End create events-remote")
+            self.logger.end("End create external events-remote")
             return
 
         except requests.ConnectionError as e:
             self.logger.exception(
                 "Network problem (e.g. failed to connect)", object=e)
+            self.logger.end("End create external events-remote connection error exception")  # noqa
             raise
 
         except requests.Timeout as e:
             self.logger.exception("Request timed out", e)
+            self.logger.end("End create external events-remote timeout exception")  # noqa
             raise
 
         except requests.RequestException as e:
             self.logger.exception(f"General error: {str(e)}", object=e)
+            self.logger.end("End create external events-remote request exception")  # noqa
             raise
 
         except Exception as e:
             self.logger.exception(
                 f"An unexpected error occurred: {str(e)}", object=e)
+            self.logger.end("End create external events-remote general exception")  # noqa
             raise
 
     def get_event_by_event_id(self, event_id: int):
         path_parameters = {
             'event_id': event_id
         }
         self.logger.start("Start get event-remote", object=path_parameters)
@@ -159,27 +167,31 @@
             self.logger.end(
                 f"End get event-remote, response: {str(response)}")
             return response
 
         except requests.ConnectionError as e:
             self.logger.exception(
                 "Network problem (e.g. failed to connect)", object=e)
+            self.logger.end("End get event-remote connection error exception")
             raise
 
         except requests.Timeout as e:
             self.logger.exception("Request timed out", e)
+            self.logger.end("End get event-remote timeout exception")
             raise
 
         except requests.RequestException as e:
             self.logger.exception(f"General error: {str(e)}", object=e)
+            self.logger.end("End get event-remote request exception")
             raise
 
         except Exception as e:
             self.logger.exception(
                 f"An unexpected error occurred: {str(e)}", object=e)
+            self.logger.end("End get event-remote general exception")
             raise
 
     def delete_event_by_id(self, event_id: int):
         path_parameters = {
             'event_id': event_id
         }
         self.logger.start("Start delete event-remote", object=path_parameters)
@@ -197,27 +209,31 @@
             self.logger.end(
                 f"End delete event-remote, response: {str(response)}")
             return response
 
         except requests.ConnectionError as e:
             self.logger.exception(
                 "Network problem (e.g. failed to connect)", object=e)
+            self.logger.end("End delete event-remote connection error exception")  # noqa
             raise
 
         except requests.Timeout as e:
             self.logger.exception("Request timed out", e)
+            self.logger.end("End delete event-remote timeout exception")
             raise
 
         except requests.RequestException as e:
             self.logger.exception(f"General error: {str(e)}", object=e)
+            self.logger.end("End delete event-remote request exception")
             raise
 
         except Exception as e:
             self.logger.exception(
                 f"An unexpected error occurred: {str(e)}", object=e)
+            self.logger.end("End delete event-remote general exception")
             raise
 
     def update_event_by_id(self, event_id: int, location_id: int,
                            organizers_profile_id: int, website_url: str,
                            facebook_event_url: str = '',
                            meetup_event_url: str = '',
                            registration_url: str = ''):
@@ -259,21 +275,25 @@
             self.logger.end(
                 f"End update event-remote, response: {str(response)}")
             return response
 
         except requests.ConnectionError as e:
             self.logger.exception(
                 "Network problem (e.g. failed to connect)", object=e)
+            self.logger.end("End update event-remote connection error exception")  # noqa
             raise
 
         except requests.Timeout as e:
             self.logger.exception("Request timed out", e)
+            self.logger.end("End update event-remote timeout exception")
             raise
 
         except requests.RequestException as e:
             self.logger.exception(f"General error: {str(e)}", object=e)
+            self.logger.end("End update event-remote request exception")
             raise
 
         except Exception as e:
             self.logger.exception(
                 f"An unexpected error occurred: {str(e)}", object=e)
+            self.logger.end("End update event-remote general exception")
             raise
```

### Comparing `event-remote-0.0.8/event_remote/src/util.py` & `event-remote-0.0.9/event_remote/src/event_remote_util.py`

 * *Files identical despite different names*

### Comparing `event-remote-0.0.8/event_remote.egg-info/PKG-INFO` & `event-remote-0.0.9/event_remote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-remote
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles event-remote Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `event-remote-0.0.8/pyproject.toml` & `event-remote-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `event-remote-0.0.8/setup.py` & `event-remote-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "event-remote"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles event-remote Python",
     long_description="PyPI Package for Circles event-remote Python",
     long_description_content_type='text/markdown',
     # TODO: Please update the URL below
     url="https://github.com/circles",
```

