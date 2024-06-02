# Comparing `tmp/websc_client-1.0.2.tar.gz` & `tmp/websc_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websc_client-1.0.2.tar", last modified: Fri May 31 06:33:39 2024, max compression
+gzip compressed data, was "websc_client-1.0.3.tar", last modified: Sun Jun  2 11:12:25 2024, max compression
```

## Comparing `websc_client-1.0.2.tar` & `websc_client-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-31 06:33:39.804592 websc_client-1.0.2/
--rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-05-31 06:33:39.804592 websc_client-1.0.2/PKG-INFO
--rw-rw-r--   0 hell      (1000) hell      (1000)     1581 2024-05-29 20:54:27.000000 websc_client-1.0.2/README.md
--rw-rw-r--   0 hell      (1000) hell      (1000)      512 2024-05-31 06:29:55.000000 websc_client-1.0.2/pyproject.toml
--rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-05-31 06:33:39.804592 websc_client-1.0.2/setup.cfg
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-31 06:33:39.804592 websc_client-1.0.2/websc_client/
--rw-rw-r--   0 hell      (1000) hell      (1000)       84 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/__init__.py
--rw-rw-r--   0 hell      (1000) hell      (1000)     4267 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/client.py
--rw-rw-r--   0 hell      (1000) hell      (1000)      162 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/exceptions.py
--rw-rw-r--   0 hell      (1000) hell      (1000)     4276 2024-05-31 06:29:55.000000 websc_client-1.0.2/websc_client/websc.py
-drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-05-31 06:33:39.804592 websc_client-1.0.2/websc_client.egg-info/
--rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/PKG-INFO
--rw-rw-r--   0 hell      (1000) hell      (1000)      300 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/SOURCES.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/dependency_links.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)       17 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/requires.txt
--rw-rw-r--   0 hell      (1000) hell      (1000)       13 2024-05-31 06:33:39.000000 websc_client-1.0.2/websc_client.egg-info/top_level.txt
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-06-02 11:12:25.657409 websc_client-1.0.3/
+-rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-06-02 11:12:25.657409 websc_client-1.0.3/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)     1581 2024-05-29 20:54:27.000000 websc_client-1.0.3/README.md
+-rw-rw-r--   0 hell      (1000) hell      (1000)      512 2024-06-02 11:12:22.000000 websc_client-1.0.3/pyproject.toml
+-rw-rw-r--   0 hell      (1000) hell      (1000)       38 2024-06-02 11:12:25.657409 websc_client-1.0.3/setup.cfg
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-06-02 11:12:25.657409 websc_client-1.0.3/websc_client/
+-rw-rw-r--   0 hell      (1000) hell      (1000)       84 2024-06-02 11:12:22.000000 websc_client-1.0.3/websc_client/__init__.py
+-rw-rw-r--   0 hell      (1000) hell      (1000)     4424 2024-06-02 11:11:22.000000 websc_client-1.0.3/websc_client/client.py
+-rw-rw-r--   0 hell      (1000) hell      (1000)      162 2024-05-31 06:29:55.000000 websc_client-1.0.3/websc_client/exceptions.py
+-rw-rw-r--   0 hell      (1000) hell      (1000)     4276 2024-05-31 06:29:55.000000 websc_client-1.0.3/websc_client/websc.py
+drwxrwxr-x   0 hell      (1000) hell      (1000)        0 2024-06-02 11:12:25.657409 websc_client-1.0.3/websc_client.egg-info/
+-rw-r--r--   0 hell      (1000) hell      (1000)     2080 2024-06-02 11:12:25.000000 websc_client-1.0.3/websc_client.egg-info/PKG-INFO
+-rw-rw-r--   0 hell      (1000) hell      (1000)      300 2024-06-02 11:12:25.000000 websc_client-1.0.3/websc_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)        1 2024-06-02 11:12:25.000000 websc_client-1.0.3/websc_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       17 2024-06-02 11:12:25.000000 websc_client-1.0.3/websc_client.egg-info/requires.txt
+-rw-rw-r--   0 hell      (1000) hell      (1000)       13 2024-06-02 11:12:25.000000 websc_client-1.0.3/websc_client.egg-info/top_level.txt
```

### Comparing `websc_client-1.0.2/PKG-INFO` & `websc_client-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websc-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for communicate with websc
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Project-URL: homepage, https://ledsc.eu/websc/
 Project-URL: repository, https://gitlab.com/ledsc/websclient
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `websc_client-1.0.2/README.md` & `websc_client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `websc_client-1.0.2/pyproject.toml` & `websc_client-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "websc-client"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Patrik Kratochvil", email="info@ledsc.eu" },
 ]
 description = "Library for communicate with websc"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `websc_client-1.0.2/websc_client/client.py` & `websc_client-1.0.3/websc_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import json
 
 import websockets as websocket
 from websockets import WebSocketClientProtocol
 from websockets.exceptions import ConnectionClosedOK, WebSocketException
 
-from .exceptions import WebSClientConnectionError
+from .exceptions import WebSClientConnectionError, WebSClientError
 from .websc import WebSCAsync, WebSClientAsyncTemplate
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class WebSClientAsync(WebSClientAsyncTemplate):
     def __init__(self, host: str, port: int):
@@ -37,14 +37,16 @@
 
         try:
             self._client = await websocket.connect(f"ws://{self.host}:{self.port}", open_timeout=2)
         except (OSError, WebSocketException) as E:
             raise WebSClientConnectionError(
                 f"LedSClient: Could not connect to websocket at {self.host}:{self.port}"
             ) from E
+        except Exception as E:
+            raise WebSClientError(f"Unknown error while connecting to {self.host}:{self.port} ({E})") from E
         _LOGGER.info(f"LedSClient: Connected to %s:%s", self.host, self.port)
         initial_message = json.loads(await self._client.recv())
 
         if "dev" in initial_message:
             for name, data in initial_message["dev"].items():
                 if name in self.devices:
                     device = self.devices[name]
```

### Comparing `websc_client-1.0.2/websc_client/websc.py` & `websc_client-1.0.3/websc_client/websc.py`

 * *Files identical despite different names*

### Comparing `websc_client-1.0.2/websc_client.egg-info/PKG-INFO` & `websc_client-1.0.3/websc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websc-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for communicate with websc
 Author-email: Patrik Kratochvil <info@ledsc.eu>
 Project-URL: homepage, https://ledsc.eu/websc/
 Project-URL: repository, https://gitlab.com/ledsc/websclient
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

