# Comparing `tmp/aiocloudweather-2024.6.0.tar.gz` & `tmp/aiocloudweather-2024.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocloudweather-2024.6.0.tar", last modified: Sat Jun  1 20:25:10 2024, max compression
+gzip compressed data, was "aiocloudweather-2024.6.1.tar", last modified: Sat Jun  1 21:01:06 2024, max compression
```

## Comparing `aiocloudweather-2024.6.0.tar` & `aiocloudweather-2024.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/aiocloudweather/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/station.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/aiocloudweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/aiocloudweather/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/station.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/aiocloudweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/tests/test_server.py
```

### Comparing `aiocloudweather-2024.6.0/LICENSE` & `aiocloudweather-2024.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/PKG-INFO` & `aiocloudweather-2024.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.6.0
+Version: 2024.6.1
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.6.0/aiocloudweather/__main__.py` & `aiocloudweather-2024.6.1/aiocloudweather/__main__.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/aiocloudweather/const.py` & `aiocloudweather-2024.6.1/aiocloudweather/const.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/aiocloudweather/conversion.py` & `aiocloudweather-2024.6.1/aiocloudweather/conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 
 @unit(UnitOfPrecipitationDepth.MILLIMETERS)
 def in_to_mm(length: float) -> float:
     """Convert inches to millimeters (mm)."""
     return round(length * 25.4, 2)
 
 
+@unit(UnitOfIrradiance.WATTS_PER_SQUARE_METER)
+def lux_to_wm2(lux: float) -> float:
+    """Convert lux to watts per square meter (W/m²)."""
+    return lux * 0.0079
+
+
 @unit(UnitOfSpeed.METERS_PER_SECOND)
 def mph_to_ms(speed: float) -> float:
     """Convert miles per hour (mph) to meters per second (m/s)."""
     return round(speed * 0.44704, 2)
 
 
 @unit(UnitOfPressure.INHG)
@@ -58,11 +64,18 @@
 
 
 @unit(UnitOfPrecipitationDepth.INCHES)
 def mm_to_in(length: float) -> float:
     """Convert millimeters (mm) to inches."""
     return round(length * 0.0393701, 2)
 
+
+@unit(LIGHT_LUX)
+def wm2_to_lux(lux: float) -> float:
+    """Convert watts per square meter (W/m²) to lux."""
+    return lux * 127
+
+
 @unit(UnitOfSpeed.MILES_PER_HOUR)
 def ms_to_mph(speed: float) -> float:
     """Convert meters per second (m/s) to miles per hour (mph)."""
     return round(speed * 2.23694, 2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiocloudweather-2024.6.0/aiocloudweather/server.py` & `aiocloudweather-2024.6.1/aiocloudweather/server.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/aiocloudweather/station.py` & `aiocloudweather-2024.6.1/aiocloudweather/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,21 +150,23 @@
     )
 
 
 IMPERIAL_TO_METRIC: Final = {
     UnitOfPressure.INHG: inhg_to_hpa,
     UnitOfTemperature.FAHRENHEIT: fahrenheit_to_celsius,
     UnitOfPrecipitationDepth.INCHES: in_to_mm,
+    LIGHT_LUX: lux_to_wm2,
     UnitOfSpeed.MILES_PER_HOUR: mph_to_ms,
 }
 
 METRIC_TO_IMPERIAL: Final = {
     UnitOfPressure.HPA: hpa_to_inhg,
     UnitOfTemperature.CELSIUS: celsius_to_fahrenheit,
     UnitOfPrecipitationDepth.MILLIMETERS: mm_to_in,
+    UnitOfIrradiance.WATTS_PER_SQUARE_METER: wm2_to_lux,
     UnitOfSpeed.METERS_PER_SECOND: ms_to_mph,
 }
 
 
 @dataclass
 class Sensor:
     """Represents a weather sensor."""
```

### Comparing `aiocloudweather-2024.6.0/aiocloudweather.egg-info/PKG-INFO` & `aiocloudweather-2024.6.1/aiocloudweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.6.0
+Version: 2024.6.1
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.6.0/aiocloudweather.egg-info/SOURCES.txt` & `aiocloudweather-2024.6.1/aiocloudweather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/setup.cfg` & `aiocloudweather-2024.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/setup.py` & `aiocloudweather-2024.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2024.6.0"
+VERSION = "2024.6.1"
 
 
 setup(
     name="aiocloudweather",
     version=VERSION,
     url="https://github.com/lhw/aiocloudweather",
     download_url="https://github.com/lhw/aiocloudweather",
```

### Comparing `aiocloudweather-2024.6.0/tests/test_conversion.py` & `aiocloudweather-2024.6.1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/tests/test_sensor.py` & `aiocloudweather-2024.6.1/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.0/tests/test_server.py` & `aiocloudweather-2024.6.1/tests/test_server.py`

 * *Files identical despite different names*

