# Comparing `tmp/pysmartcocoon-0.8.1.tar.gz` & `tmp/pysmartcocoon-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmartcocoon-0.8.1.tar", last modified: Sun Feb 25 19:06:06 2024, max compression
+gzip compressed data, was "pysmartcocoon-1.0.0.tar", last modified: Sat Mar 30 13:58:12 2024, max compression
```

## Comparing `pysmartcocoon-0.8.1.tar` & `pysmartcocoon-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-25 19:06:06.733073 pysmartcocoon-0.8.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1068 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/LICENSE.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3584 2024-02-25 19:06:06.724709 pysmartcocoon-0.8.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1248 2024-02-25 19:05:00.000000 pysmartcocoon-0.8.1/pyproject.toml
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-25 19:06:06.674741 pysmartcocoon-0.8.1/pysmartcocoon/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       35 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       35 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4588 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      990 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      470 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/errors.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13904 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/fan.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1306 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/location.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7179 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2226 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/room.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1940 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/pysmartcocoon/thermostat.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-25 19:06:06.718818 pysmartcocoon-0.8.1/pysmartcocoon.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3584 2024-02-25 19:06:06.000000 pysmartcocoon-0.8.1/pysmartcocoon.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      487 2024-02-25 19:06:06.000000 pysmartcocoon-0.8.1/pysmartcocoon.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-25 19:06:06.000000 pysmartcocoon-0.8.1/pysmartcocoon.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      148 2024-02-25 19:06:06.000000 pysmartcocoon-0.8.1/pysmartcocoon.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2024-02-25 19:06:06.000000 pysmartcocoon-0.8.1/pysmartcocoon.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-02-25 19:06:06.734896 pysmartcocoon-0.8.1/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-25 19:06:06.710318 pysmartcocoon-0.8.1/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1867 2024-02-25 18:39:35.000000 pysmartcocoon-0.8.1/tests/test_integration.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-30 13:58:12.578963 pysmartcocoon-1.0.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1068 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/LICENSE.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3799 2024-03-30 13:58:12.575828 pysmartcocoon-1.0.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2775 2024-03-30 13:51:26.000000 pysmartcocoon-1.0.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1248 2024-03-30 13:52:36.000000 pysmartcocoon-1.0.0/pyproject.toml
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-30 13:58:12.522134 pysmartcocoon-1.0.0/pysmartcocoon/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       35 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       35 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4588 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      990 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      470 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/errors.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13880 2024-03-30 13:51:26.000000 pysmartcocoon-1.0.0/pysmartcocoon/fan.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1306 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/location.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7180 2024-03-30 13:51:26.000000 pysmartcocoon-1.0.0/pysmartcocoon/manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2226 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/room.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1940 2024-02-25 18:39:35.000000 pysmartcocoon-1.0.0/pysmartcocoon/thermostat.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-30 13:58:12.568533 pysmartcocoon-1.0.0/pysmartcocoon.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3799 2024-03-30 13:58:12.000000 pysmartcocoon-1.0.0/pysmartcocoon.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      487 2024-03-30 13:58:12.000000 pysmartcocoon-1.0.0/pysmartcocoon.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-03-30 13:58:12.000000 pysmartcocoon-1.0.0/pysmartcocoon.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      148 2024-03-30 13:58:12.000000 pysmartcocoon-1.0.0/pysmartcocoon.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2024-03-30 13:58:12.000000 pysmartcocoon-1.0.0/pysmartcocoon.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-03-30 13:58:12.579642 pysmartcocoon-1.0.0/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-30 13:58:12.562734 pysmartcocoon-1.0.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1928 2024-03-30 13:51:26.000000 pysmartcocoon-1.0.0/tests/test_integration.py
```

### Comparing `pysmartcocoon-0.8.1/LICENSE.md` & `pysmartcocoon-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysmartcocoon-0.8.1/PKG-INFO` & `pysmartcocoon-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmartcocoon
-Version: 0.8.1
+Version: 1.0.0
 Summary: Library built for Home Assistant to integrate with the SmartCocoon
 Author-email: Dave Pearce <davepearce@live.com>
 Project-URL: Homepage, https://github.com/davecpearce/pysmartcocoon
 Keywords: smartcocoon,fan
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -66,14 +66,22 @@
   - Set Eco mode
 
 ## Examples
 
 You can refer to the tests/test_integration.py to see an example of integration with the
 SmartCocoon API
 
+Copy the tests/template.env* to \_tests/.env* file and update the account information with your your SmartCocoon account information:
+
+```python
+USERNAME="user@domain.com"
+PASSWORD="mypassword"
+FAN_ID="abc123"
+```
+
 ## Work to do
 
 - The fans are using MQTT but this is not being leveraged yet
 - Discovery has not been implemented, not sure if this is possible
 - Fan status will currently require polling if the fan is changed directly in the app
 
 [black]: https://github.com/psf/black
```

### Comparing `pysmartcocoon-0.8.1/README.md` & `pysmartcocoon-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,22 @@
   - Set Eco mode
 
 ## Examples
 
 You can refer to the tests/test_integration.py to see an example of integration with the
 SmartCocoon API
 
+Copy the tests/template.env* to \_tests/.env* file and update the account information with your your SmartCocoon account information:
+
+```python
+USERNAME="user@domain.com"
+PASSWORD="mypassword"
+FAN_ID="abc123"
+```
+
 ## Work to do
 
 - The fans are using MQTT but this is not being leveraged yet
 - Discovery has not been implemented, not sure if this is possible
 - Fan status will currently require polling if the fan is changed directly in the app
 
 [black]: https://github.com/psf/black
```

### Comparing `pysmartcocoon-0.8.1/pyproject.toml` & `pysmartcocoon-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysmartcocoon"
-version = "0.8.1"
+version = "1.0.0"
 
 description = "Library built for Home Assistant to integrate with the SmartCocoon"
 readme = "README.md"
 authors = [{ name = "Dave Pearce", email = "davepearce@live.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 
@@ -44,15 +44,15 @@
     "pytest-cov",
 ]
 
 [project.urls]
 Homepage = "https://github.com/davecpearce/pysmartcocoon"
 
 [tool.bumpver]
-current_version = "0.8.1"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon/api.py` & `pysmartcocoon-1.0.0/pysmartcocoon/api.py`

 * *Files identical despite different names*

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon/const.py` & `pysmartcocoon-1.0.0/pysmartcocoon/const.py`

 * *Files identical despite different names*

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon/fan.py` & `pysmartcocoon-1.0.0/pysmartcocoon/fan.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,15 +428,15 @@
 
         if self.mqtt_username is None:
             _LOGGER.debug(
                 "Fan ID: %s - MQTT username is not provided", self.fan_id
             )
             return False
 
-        client_id = mqtt.base62(uuid.uuid4().int, padding=22)
+        client_id = str(uuid.uuid4())
         self._mqttc = mqtt.Client(client_id, protocol=mqtt.MQTTv311)
         self._mqttc.username_pw_set(
             self.mqtt_username, password=self.mqtt_password
         )
         self._mqttc.on_connect = self._mqtt_on_connect
         self._mqttc.connect(
             MQTT_BROKER, port=MQTT_PORT, keepalive=MQTT_KEEPALIVE
```

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon/location.py` & `pysmartcocoon-1.0.0/pysmartcocoon/location.py`

 * *Files identical despite different names*

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon/manager.py` & `pysmartcocoon-1.0.0/pysmartcocoon/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     @property
     def fans(self):
         """Return list of Fans."""
         return self._fans
 
     async def async_start_services(
-        self, username: str, password: str, use_mqtt: bool = True
+        self, username: str, password: str, use_mqtt: bool = False
     ) -> bool:
         """Start services"""
 
         _LOGGER.debug("Starting services")
 
         # Authenticate with the API
         self._api_connected = await self._api.async_authenticate(
```

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon/room.py` & `pysmartcocoon-1.0.0/pysmartcocoon/room.py`

 * *Files identical despite different names*

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon/thermostat.py` & `pysmartcocoon-1.0.0/pysmartcocoon/thermostat.py`

 * *Files identical despite different names*

### Comparing `pysmartcocoon-0.8.1/pysmartcocoon.egg-info/PKG-INFO` & `pysmartcocoon-1.0.0/pysmartcocoon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmartcocoon
-Version: 0.8.1
+Version: 1.0.0
 Summary: Library built for Home Assistant to integrate with the SmartCocoon
 Author-email: Dave Pearce <davepearce@live.com>
 Project-URL: Homepage, https://github.com/davecpearce/pysmartcocoon
 Keywords: smartcocoon,fan
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -66,14 +66,22 @@
   - Set Eco mode
 
 ## Examples
 
 You can refer to the tests/test_integration.py to see an example of integration with the
 SmartCocoon API
 
+Copy the tests/template.env* to \_tests/.env* file and update the account information with your your SmartCocoon account information:
+
+```python
+USERNAME="user@domain.com"
+PASSWORD="mypassword"
+FAN_ID="abc123"
+```
+
 ## Work to do
 
 - The fans are using MQTT but this is not being leveraged yet
 - Discovery has not been implemented, not sure if this is possible
 - Fan status will currently require polling if the fan is changed directly in the app
 
 [black]: https://github.com/psf/black
```

### Comparing `pysmartcocoon-0.8.1/tests/test_integration.py` & `pysmartcocoon-1.0.0/tests/test_integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Tests SmartCocoon api module."""
 import asyncio
 import logging
 import time
+from os import environ
+from os.path import dirname, join
 
 import aiohttp
 import pytest
+from dotenv import load_dotenv
 
 from pysmartcocoon.fan import Fan
 from pysmartcocoon.manager import SmartCocoonManager
 
-# Enter correct real values here for the tests to complete successfully
-# with real SmartCocoon Server calls.
-USERNAME = "user@domain.com"
-PASSWORD = "password"
-FAN_ID = "1abc23"  # This is the physical fan ID printed from the fan
+# Load the account information
+dotenv_path = join(dirname(__file__), ".env")
+load_dotenv(dotenv_path)
+
+USERNAME = environ.get("USERNAME")
+PASSWORD = environ.get("PASSWORD")
+FAN_ID = environ.get("FAN_ID")
 
 logging.basicConfig(level=logging.DEBUG)
 _LOGGER: logging.Logger = logging.getLogger(__name__)
 
 
 @pytest.mark.skip(
     "Not an automated test but an example of usage with real values."
```

