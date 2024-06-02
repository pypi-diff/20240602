# Comparing `tmp/pyftms-0.2.3.tar.gz` & `tmp/pyftms-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftms-0.2.3.tar", max compression
+gzip compressed data, was "pyftms-0.2.4.tar", max compression
```

## Comparing `pyftms-0.2.3.tar` & `pyftms-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11374 2024-06-02 05:46:35.267073 pyftms-0.2.3/LICENSE
--rw-r--r--   0        0        0      792 2024-06-02 05:46:35.267073 pyftms-0.2.3/README.md
--rw-r--r--   0        0        0     1604 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/__init__.py
--rw-r--r--   0        0        0      939 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/__main__.py
--rw-r--r--   0        0        0     3573 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/__init__.py
--rw-r--r--   0        0        0      695 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/backends/__init__.py
--rw-r--r--   0        0        0     8214 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/backends/controller.py
--rw-r--r--   0        0        0     6245 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/backends/event.py
--rw-r--r--   0        0        0     2039 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/backends/updater.py
--rw-r--r--   0        0        0    11045 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/client.py
--rw-r--r--   0        0        0     4841 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/const.py
--rw-r--r--   0        0        0      867 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/machines/__init__.py
--rw-r--r--   0        0        0      599 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/machines/cross_trainer.py
--rw-r--r--   0        0        0      576 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/machines/indoor_bike.py
--rw-r--r--   0        0        0      542 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/machines/rower.py
--rw-r--r--   0        0        0      553 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/machines/treadmill.py
--rw-r--r--   0        0        0    10480 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/manager.py
--rw-r--r--   0        0        0      685 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/properties/__init__.py
--rw-r--r--   0        0        0     1216 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/properties/device_info.py
--rw-r--r--   0        0        0     5838 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/properties/features.py
--rw-r--r--   0        0        0     2448 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/client/properties/machine_type.py
--rw-r--r--   0        0        0     1117 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/__init__.py
--rw-r--r--   0        0        0     2530 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/common.py
--rw-r--r--   0        0        0     8956 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/control_point.py
--rw-r--r--   0        0        0     6446 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/machine_status.py
--rw-r--r--   0        0        0      374 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/realtime_data/__init__.py
--rw-r--r--   0        0        0     2823 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/realtime_data/common.py
--rw-r--r--   0        0        0     3075 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/realtime_data/cross_trainer.py
--rw-r--r--   0        0        0     2324 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/realtime_data/indoor_bike.py
--rw-r--r--   0        0        0     2973 2024-06-02 05:46:35.267073 pyftms-0.2.3/pyftms/models/realtime_data/rower.py
--rw-r--r--   0        0        0     2701 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/models/realtime_data/treadmill.py
--rw-r--r--   0        0        0     1350 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/models/spin_down.py
--rw-r--r--   0        0        0     2194 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/models/training_status.py
--rw-r--r--   0        0        0      471 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/serializer/__init__.py
--rw-r--r--   0        0        0      783 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/serializer/list.py
--rw-r--r--   0        0        0     7662 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/serializer/model.py
--rw-r--r--   0        0        0     2080 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/serializer/num.py
--rw-r--r--   0        0        0      594 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyftms/serializer/serializer.py
--rw-r--r--   0        0        0      480 2024-06-02 05:46:35.271073 pyftms-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 pyftms-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11374 2024-06-02 15:02:37.402598 pyftms-0.2.4/LICENSE
+-rw-r--r--   0        0        0      792 2024-06-02 15:02:37.402598 pyftms-0.2.4/README.md
+-rw-r--r--   0        0        0     1604 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/__init__.py
+-rw-r--r--   0        0        0      939 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/__main__.py
+-rw-r--r--   0        0        0     3573 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/__init__.py
+-rw-r--r--   0        0        0      695 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/__init__.py
+-rw-r--r--   0        0        0     8214 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/controller.py
+-rw-r--r--   0        0        0     6245 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/event.py
+-rw-r--r--   0        0        0     2039 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/updater.py
+-rw-r--r--   0        0        0    11045 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/client.py
+-rw-r--r--   0        0        0     4841 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/const.py
+-rw-r--r--   0        0        0      867 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/__init__.py
+-rw-r--r--   0        0        0      599 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/cross_trainer.py
+-rw-r--r--   0        0        0      576 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/indoor_bike.py
+-rw-r--r--   0        0        0      542 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/rower.py
+-rw-r--r--   0        0        0      553 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/treadmill.py
+-rw-r--r--   0        0        0    10506 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/manager.py
+-rw-r--r--   0        0        0      685 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/__init__.py
+-rw-r--r--   0        0        0     1216 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/device_info.py
+-rw-r--r--   0        0        0     5838 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/features.py
+-rw-r--r--   0        0        0     2448 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/machine_type.py
+-rw-r--r--   0        0        0     1117 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/__init__.py
+-rw-r--r--   0        0        0     2530 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/common.py
+-rw-r--r--   0        0        0     8956 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/control_point.py
+-rw-r--r--   0        0        0     6446 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/machine_status.py
+-rw-r--r--   0        0        0      374 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/__init__.py
+-rw-r--r--   0        0        0     2823 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/common.py
+-rw-r--r--   0        0        0     3075 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/cross_trainer.py
+-rw-r--r--   0        0        0     2324 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/indoor_bike.py
+-rw-r--r--   0        0        0     2973 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/rower.py
+-rw-r--r--   0        0        0     2701 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/treadmill.py
+-rw-r--r--   0        0        0     1350 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/spin_down.py
+-rw-r--r--   0        0        0     2194 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/training_status.py
+-rw-r--r--   0        0        0      471 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/__init__.py
+-rw-r--r--   0        0        0      783 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/list.py
+-rw-r--r--   0        0        0     7662 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/model.py
+-rw-r--r--   0        0        0     2080 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/num.py
+-rw-r--r--   0        0        0      594 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/serializer.py
+-rw-r--r--   0        0        0      480 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 pyftms-0.2.4/PKG-INFO
```

### Comparing `pyftms-0.2.3/LICENSE` & `pyftms-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/README.md` & `pyftms-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/__init__.py` & `pyftms-0.2.4/pyftms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/__main__.py` & `pyftms-0.2.4/pyftms/__main__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/__init__.py` & `pyftms-0.2.4/pyftms/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/backends/__init__.py` & `pyftms-0.2.4/pyftms/client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/backends/controller.py` & `pyftms-0.2.4/pyftms/client/backends/controller.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/backends/event.py` & `pyftms-0.2.4/pyftms/client/backends/event.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/backends/updater.py` & `pyftms-0.2.4/pyftms/client/backends/updater.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/client.py` & `pyftms-0.2.4/pyftms/client/client.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/const.py` & `pyftms-0.2.4/pyftms/client/const.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/machines/__init__.py` & `pyftms-0.2.4/pyftms/client/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/machines/cross_trainer.py` & `pyftms-0.2.4/pyftms/client/machines/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/machines/indoor_bike.py` & `pyftms-0.2.4/pyftms/client/machines/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/machines/rower.py` & `pyftms-0.2.4/pyftms/client/machines/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/machines/treadmill.py` & `pyftms-0.2.4/pyftms/client/machines/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/manager.py` & `pyftms-0.2.4/pyftms/client/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,18 +50,20 @@
         elif e.event_id == "setup":
             self._settings |= e.event_data
         elif e.event_id == "training_status":
             self._training_status = e.event_data["code"]
 
         return self._cb and self._cb(e)
 
-    def _get_property(self, name: str) -> Any:
+    def get_property(self, name: str) -> Any:
+        """Get property by name."""
         return self._properties.get(name)
 
-    def _get_setting(self, name: str) -> Any:
+    def get_setting(self, name: str) -> Any:
+        """Get setting by name."""
         return self._settings.get(name)
 
     @property
     def properties(self) -> UpdateEventData:
         """Read-only updateable properties mapping."""
         return cast(UpdateEventData, MappingProxyType(self._properties))
 
@@ -88,384 +90,384 @@
     @property
     def cadence_average(self) -> float:
         """
         Average Cadence.
 
         Units: `rpm`.
         """
-        return self._get_property(c.CADENCE_AVERAGE)
+        return self.get_property(c.CADENCE_AVERAGE)
 
     @property
     def cadence_instant(self) -> float:
         """
         Instantaneous Cadence.
 
         Units: `rpm`.
         """
-        return self._get_property(c.CADENCE_INSTANT)
+        return self.get_property(c.CADENCE_INSTANT)
 
     @property
     def distance_total(self) -> int:
         """
         Total Distance.
 
         Units: `m`.
         """
-        return self._get_property(c.DISTANCE_TOTAL)
+        return self.get_property(c.DISTANCE_TOTAL)
 
     @property
     def elevation_gain_negative(self) -> float:
         """
         Negative Elevation Gain.
 
         Units: `m`.
         """
-        return self._get_property(c.ELEVATION_GAIN_NEGATIVE)
+        return self.get_property(c.ELEVATION_GAIN_NEGATIVE)
 
     @property
     def elevation_gain_positive(self) -> float:
         """
         Positive Elevation Gain.
 
         Units: `m`.
         """
-        return self._get_property(c.ELEVATION_GAIN_POSITIVE)
+        return self.get_property(c.ELEVATION_GAIN_POSITIVE)
 
     @property
     def energy_per_hour(self) -> int:
         """
         Energy Per Hour.
 
         Units: `kcal`.
         """
-        return self._get_property(c.ENERGY_PER_HOUR)
+        return self.get_property(c.ENERGY_PER_HOUR)
 
     @property
     def energy_per_minute(self) -> int:
         """
         Energy Per Minute.
 
         Units: `kcal`.
         """
-        return self._get_property(c.ENERGY_PER_MINUTE)
+        return self.get_property(c.ENERGY_PER_MINUTE)
 
     @property
     def energy_total(self) -> int:
         """
         Total Energy.
 
         Units: `kcal`.
         """
-        return self._get_property(c.ENERGY_TOTAL)
+        return self.get_property(c.ENERGY_TOTAL)
 
     @property
     def force_on_belt(self) -> int:
         """
         Force on Belt.
 
         Units: `newton`.
         """
-        return self._get_property(c.FORCE_ON_BELT)
+        return self.get_property(c.FORCE_ON_BELT)
 
     @property
     def heart_rate(self) -> int:
         """
         Heart Rate.
 
         Units: `bpm`.
         """
-        return self._get_property(c.HEART_RATE)
+        return self.get_property(c.HEART_RATE)
 
     @property
     def inclination(self) -> float:
         """
         Inclination.
 
         Units: `%`.
         """
-        return self._get_property(c.INCLINATION)
+        return self.get_property(c.INCLINATION)
 
     @property
     def metabolic_equivalent(self) -> float:
         """
         Metabolic Equivalent.
 
         Units: `meta`.
         """
-        return self._get_property(c.METABOLIC_EQUIVALENT)
+        return self.get_property(c.METABOLIC_EQUIVALENT)
 
     @property
     def movement_direction(self) -> MovementDirection:
         """
         Movement Direction.
 
         Units: `MovementDirection`.
         """
-        return self._get_property(c.MOVEMENT_DIRECTION)
+        return self.get_property(c.MOVEMENT_DIRECTION)
 
     @property
     def pace_average(self) -> int | float:
         """
         Average Pace.
 
         Units: `km/m` or `seconds(500m)` for `Rower`.
         """
-        return self._get_property(c.PACE_AVERAGE)
+        return self.get_property(c.PACE_AVERAGE)
 
     @property
     def pace_instant(self) -> int | float:
         """
         Instantaneous Pace.
 
         Units: `km/m` or `seconds(500m)` for `Rower`.
         """
-        return self._get_property(c.PACE_INSTANT)
+        return self.get_property(c.PACE_INSTANT)
 
     @property
     def power_average(self) -> int:
         """
         Average Power.
 
         Units: `Watt`.
         """
-        return self._get_property(c.POWER_AVERAGE)
+        return self.get_property(c.POWER_AVERAGE)
 
     @property
     def power_instant(self) -> int:
         """
         Instantaneous Power.
 
         Units: `Watt`.
         """
-        return self._get_property(c.POWER_INSTANT)
+        return self.get_property(c.POWER_INSTANT)
 
     @property
     def power_output(self) -> int:
         """
         Power Output.
 
         Units: `Watt`.
         """
-        return self._get_property(c.POWER_OUTPUT)
+        return self.get_property(c.POWER_OUTPUT)
 
     @property
     def ramp_angle(self) -> float:
         """
         Ramp Angle Setting.
 
         Units: `degree`.
         """
-        return self._get_property(c.RAMP_ANGLE)
+        return self.get_property(c.RAMP_ANGLE)
 
     @property
     def resistance_level(self) -> int | float:
         """
         Resistance Level.
 
         Units: `unitless`.
         """
-        return self._get_property(c.RESISTANCE_LEVEL)
+        return self.get_property(c.RESISTANCE_LEVEL)
 
     @property
     def speed_average(self) -> float:
         """
         Average Speed.
 
         Units: `km/h`.
         """
-        return self._get_property(c.SPEED_AVERAGE)
+        return self.get_property(c.SPEED_AVERAGE)
 
     @property
     def speed_instant(self) -> float:
         """
         Instantaneous Speed.
 
         Units: `km/h`.
         """
-        return self._get_property(c.SPEED_INSTANT)
+        return self.get_property(c.SPEED_INSTANT)
 
     @property
     def step_rate_average(self) -> int:
         """
         Average Step Rate.
 
         Units: `step/m`.
         """
-        return self._get_property(c.STEP_RATE_AVERAGE)
+        return self.get_property(c.STEP_RATE_AVERAGE)
 
     @property
     def step_rate_instant(self) -> int:
         """
         Instantaneous Step Rate.
 
         Units: `step/m`.
         """
-        return self._get_property(c.STEP_RATE_INSTANT)
+        return self.get_property(c.STEP_RATE_INSTANT)
 
     @property
     def stride_count(self) -> int:
         """
         Stride Count.
 
         Units: `unitless`.
         """
-        return self._get_property(c.STRIDE_COUNT)
+        return self.get_property(c.STRIDE_COUNT)
 
     @property
     def stroke_count(self) -> int:
         """
         Stroke Count.
 
         Units: `unitless`.
         """
-        return self._get_property(c.STROKE_COUNT)
+        return self.get_property(c.STROKE_COUNT)
 
     @property
     def stroke_rate_average(self) -> float:
         """
         Average Stroke Rate.
 
         Units: `stroke/m`.
         """
-        return self._get_property(c.STROKE_RATE_AVERAGE)
+        return self.get_property(c.STROKE_RATE_AVERAGE)
 
     @property
     def stroke_rate_instant(self) -> float:
         """
         Instantaneous Stroke Rate.
 
         Units: `stroke/m`.
         """
-        return self._get_property(c.STROKE_RATE_INSTANT)
+        return self.get_property(c.STROKE_RATE_INSTANT)
 
     @property
     def time_elapsed(self) -> int:
         """
         Elapsed Time.
 
         Units: `s`.
         """
-        return self._get_property(c.TIME_ELAPSED)
+        return self.get_property(c.TIME_ELAPSED)
 
     @property
     def time_remaining(self) -> int:
         """
         Remaining Time.
 
         Units: `s`.
         """
-        return self._get_property(c.TIME_REMAINING)
+        return self.get_property(c.TIME_REMAINING)
 
     # SETTINGS
 
     @property
     def indoor_bike_simulation(self) -> IndoorBikeSimulationParameters:
         """Indoor Bike Simulation Parameters."""
-        return self._get_setting(c.INDOOR_BIKE_SIMULATION)
+        return self.get_setting(c.INDOOR_BIKE_SIMULATION)
 
     @property
     def target_cadence(self) -> float:
         """
         Targeted cadence.
 
         Units: `rpm`.
         """
-        return self._get_setting(c.TARGET_CADENCE)
+        return self.get_setting(c.TARGET_CADENCE)
 
     @property
     def target_distance(self) -> int:
         """
         Targeted distance.
 
         Units: `m`.
         """
-        return self._get_setting(c.TARGET_DISTANCE)
+        return self.get_setting(c.TARGET_DISTANCE)
 
     @property
     def target_energy(self) -> int:
         """
         Targeted expended energy.
 
         Units: `kcal`.
         """
-        return self._get_setting(c.TARGET_ENERGY)
+        return self.get_setting(c.TARGET_ENERGY)
 
     @property
     def target_heart_rate(self) -> int:
         """
         Targeted heart rate.
 
         Units: `bpm`.
         """
-        return self._get_setting(c.TARGET_HEART_RATE)
+        return self.get_setting(c.TARGET_HEART_RATE)
 
     @property
     def target_inclination(self) -> float:
         """
         Targeted inclination.
 
         Units: `%`.
         """
-        return self._get_setting(c.TARGET_INCLINATION)
+        return self.get_setting(c.TARGET_INCLINATION)
 
     @property
     def target_power(self) -> int:
         """
         Targeted power.
 
         Units: `Watt`.
         """
-        return self._get_setting(c.TARGET_POWER)
+        return self.get_setting(c.TARGET_POWER)
 
     @property
     def target_resistance(self) -> float:
         """
         Targeted resistance level.
 
         Units: `unitless`.
         """
-        return self._get_setting(c.TARGET_RESISTANCE)
+        return self.get_setting(c.TARGET_RESISTANCE)
 
     @property
     def target_speed(self) -> float:
         """
         Targeted speed.
 
         Units: `km/h`.
         """
-        return self._get_setting(c.TARGET_SPEED)
+        return self.get_setting(c.TARGET_SPEED)
 
     @property
     def target_steps(self) -> int:
         """
         Targeted number of steps.
 
         Units: `step`.
         """
-        return self._get_setting(c.TARGET_STEPS)
+        return self.get_setting(c.TARGET_STEPS)
 
     @property
     def target_strides(self) -> int:
         """
         Targeted number of strides.
 
         Units: `stride`.
         """
-        return self._get_setting(c.TARGET_STRIDES)
+        return self.get_setting(c.TARGET_STRIDES)
 
     @property
     def target_time(self) -> tuple[int, ...]:
         """
         Targeted training time.
 
         Units: `s`.
         """
-        return self._get_setting(c.TARGET_TIME)
+        return self.get_setting(c.TARGET_TIME)
 
     @property
     def wheel_circumference(self) -> float:
         """
         Wheel circumference.
 
         Units: `mm`.
         """
-        return self._get_setting(c.WHEEL_CIRCUMFERENCE)
+        return self.get_setting(c.WHEEL_CIRCUMFERENCE)
```

### Comparing `pyftms-0.2.3/pyftms/client/properties/__init__.py` & `pyftms-0.2.4/pyftms/client/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/properties/device_info.py` & `pyftms-0.2.4/pyftms/client/properties/device_info.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/properties/features.py` & `pyftms-0.2.4/pyftms/client/properties/features.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/client/properties/machine_type.py` & `pyftms-0.2.4/pyftms/client/properties/machine_type.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/__init__.py` & `pyftms-0.2.4/pyftms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/common.py` & `pyftms-0.2.4/pyftms/models/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/control_point.py` & `pyftms-0.2.4/pyftms/models/control_point.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/machine_status.py` & `pyftms-0.2.4/pyftms/models/machine_status.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/realtime_data/common.py` & `pyftms-0.2.4/pyftms/models/realtime_data/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/realtime_data/cross_trainer.py` & `pyftms-0.2.4/pyftms/models/realtime_data/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/realtime_data/indoor_bike.py` & `pyftms-0.2.4/pyftms/models/realtime_data/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/realtime_data/rower.py` & `pyftms-0.2.4/pyftms/models/realtime_data/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/realtime_data/treadmill.py` & `pyftms-0.2.4/pyftms/models/realtime_data/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/spin_down.py` & `pyftms-0.2.4/pyftms/models/spin_down.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/models/training_status.py` & `pyftms-0.2.4/pyftms/models/training_status.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/serializer/list.py` & `pyftms-0.2.4/pyftms/serializer/list.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/serializer/model.py` & `pyftms-0.2.4/pyftms/serializer/model.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/serializer/num.py` & `pyftms-0.2.4/pyftms/serializer/num.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/pyftms/serializer/serializer.py` & `pyftms-0.2.4/pyftms/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.3/PKG-INFO` & `pyftms-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftms
-Version: 0.2.3
+Version: 0.2.4
 Summary: PyFTMS - Python Fitness Machine Service client library.
 Author: Sergey V. DUDANOV
 Author-email: sergey.dudanov@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

