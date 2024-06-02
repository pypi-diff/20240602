# Comparing `tmp/synthetic_home-2.6.1.tar.gz` & `tmp/synthetic_home-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetic_home-2.6.1.tar", last modified: Thu May 30 06:42:35 2024, max compression
+gzip compressed data, was "synthetic_home-3.0.1.tar", last modified: Sun Jun  2 01:34:42 2024, max compression
```

## Comparing `synthetic_home-2.6.1.tar` & `synthetic_home-3.0.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:42:35.787432 synthetic_home-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-30 06:42:35.787432 synthetic_home-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-30 06:42:35.791432 synthetic_home-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:42:35.783432 synthetic_home-2.6.1/synthetic_home/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:42:35.787432 synthetic_home-2.6.1/synthetic_home/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/door-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/exhaust-fan.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/fan-oscilating.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/garage-door.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/gate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/heat-pump.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/hvac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/light-dimmable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/light-rgbw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/light.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/lock-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/motion-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/smart-blinds.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/smart-lock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/smart-plug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/smart-speaker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/smart-sprinkler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/smart-tv.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/temperature-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/todo-list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/vacuum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/water-valve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/weather-service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/registry/window-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/synthetic_home/synthetic_home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:42:35.787432 synthetic_home-2.6.1/synthetic_home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-30 06:42:35.000000 synthetic_home-2.6.1/synthetic_home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 06:42:35.000000 synthetic_home-2.6.1/synthetic_home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:42:35.000000 synthetic_home-2.6.1/synthetic_home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 06:42:35.000000 synthetic_home-2.6.1/synthetic_home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 06:42:35.000000 synthetic_home-2.6.1/synthetic_home.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:42:35.787432 synthetic_home-2.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/tests/test_device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-30 06:42:24.000000 synthetic_home-2.6.1/tests/test_synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:34:42.848414 synthetic_home-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-06-02 01:34:42.848414 synthetic_home-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-02 01:34:42.848414 synthetic_home-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:34:42.840413 synthetic_home-3.0.1/synthetic_home/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:34:42.844414 synthetic_home-3.0.1/synthetic_home/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/door-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/exhaust-fan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/fan-oscilating.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/garage-door.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/gate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/heat-pump.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/hvac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/light-dimmable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/light-rgbw.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/light.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/lock-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/motion-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/smart-blinds.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/smart-lock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/smart-plug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/smart-speaker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/smart-sprinkler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/smart-tv.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/temperature-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/todo-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/vacuum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/water-valve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/weather-service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/registry/window-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/synthetic_home/synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:34:42.848414 synthetic_home-3.0.1/synthetic_home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-06-02 01:34:42.000000 synthetic_home-3.0.1/synthetic_home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-06-02 01:34:42.000000 synthetic_home-3.0.1/synthetic_home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 01:34:42.000000 synthetic_home-3.0.1/synthetic_home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 01:34:42.000000 synthetic_home-3.0.1/synthetic_home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 01:34:42.000000 synthetic_home-3.0.1/synthetic_home.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:34:42.848414 synthetic_home-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-02 01:34:32.000000 synthetic_home-3.0.1/tests/test_synthetic_home.py
```

### Comparing `synthetic_home-2.6.1/LICENSE` & `synthetic_home-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/PKG-INFO` & `synthetic_home-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_home
-Version: 2.6.1
+Version: 3.0.1
 Summary: Library for managing synthetic home device registry
 Home-page: https://github.com/allenporter/synthetic-home
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synthetic_home-2.6.1/README.md` & `synthetic_home-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/pyproject.toml` & `synthetic_home-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/setup.cfg` & `synthetic_home-3.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = synthetic_home
-version = 2.6.1
+version = 3.0.1
 description = Library for managing synthetic home device registry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/synthetic-home
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `synthetic_home-2.6.1/synthetic_home/device_types.py` & `synthetic_home-3.0.1/synthetic_home/device_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""Data model for home assistant synthetic home."""
+"""Data model for device type definitions.
+
+These device devices and how they map to a set of entities. States can be set
+on a device then translated into how that state affects entities.
+"""
 
 from functools import cache
 from collections.abc import Generator
 from dataclasses import dataclass, field
 from importlib import resources
 from importlib.resources.abc import Traversable
 import logging
@@ -87,15 +91,15 @@
 
     domain: str
     """The domain of the entity."""
 
     key: str
     """The entity key identifying the entity."""
 
-    state: str | bool | dict[str, Any]
+    state: str | dict[str, Any]
     """The values that make up the entity state."""
 
     @property
     def domain_key(self) -> str:
         """Return the full domain.key."""
         return f"{self.domain}.{self.key}"
 
@@ -286,14 +290,15 @@
         if device_type_file.name != f"{device_type.device_type}.yaml":
             raise SyntheticHomeError(
                 f"Device type '{device_type.device_type}' name does not match filename '{device_type_file.name}'"
             )
 
         yield device_type
 
+
 @cache
 def load_device_type_registry() -> DeviceTypeRegistry:
     """Load device types from the yaml configuration files."""
     device_types = {}
     for device_type in _read_device_types(DEVICE_TYPES_RESOURCE_PATH):
         if device_type.device_type in device_types:
             raise SyntheticHomeError(
```

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/README.md` & `synthetic_home-3.0.1/synthetic_home/registry/README.md`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/camera.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/camera.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 ---
 device_type: camera
 desc: A video camera that supports motion detection and other events.
 device_states:
   idle:
+    binary_sensor.motion: false
+    binary_sensor.person: false
+    binary_sensor.sound: false
   motion-detected:
     binary_sensor.motion: true
   person-detected:
     binary_sensor.person: true
   sound-detected:
     binary_sensor.sound: true
 entities:
```

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/door-sensor.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/door-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/exhaust-fan.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/exhaust-fan.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/heat-pump.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/heat-pump.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/hvac.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/hvac.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/lock-sensor.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/lock-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/motion-sensor.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/motion-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/smart-blinds.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/smart-blinds.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/smart-lock.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/smart-lock.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/smart-speaker.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/smart-speaker.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/smart-tv.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/smart-tv.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/temperature-sensor.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/temperature-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/vacuum.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/vacuum.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/water-valve.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/water-valve.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/weather-service.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/weather-service.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home/registry/window-sensor.yaml` & `synthetic_home-3.0.1/synthetic_home/registry/window-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.6.1/synthetic_home.egg-info/PKG-INFO` & `synthetic_home-3.0.1/synthetic_home.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_home
-Version: 2.6.1
+Version: 3.0.1
 Summary: Library for managing synthetic home device registry
 Home-page: https://github.com/allenporter/synthetic-home
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synthetic_home-2.6.1/synthetic_home.egg-info/SOURCES.txt` & `synthetic_home-3.0.1/synthetic_home.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ./synthetic_home/__init__.py
+./synthetic_home/common.py
 ./synthetic_home/device_types.py
 ./synthetic_home/exceptions.py
+./synthetic_home/inventory.py
 ./synthetic_home/py.typed
 ./synthetic_home/synthetic_home.py
 ./synthetic_home/registry/README.md
 ./synthetic_home/registry/__init__.py
 ./synthetic_home/registry/camera.yaml
 ./synthetic_home/registry/door-sensor.yaml
 ./synthetic_home/registry/exhaust-fan.yaml
```

### Comparing `synthetic_home-2.6.1/tests/test_device_types.py` & `synthetic_home-3.0.1/tests/test_device_types.py`

 * *Files identical despite different names*

