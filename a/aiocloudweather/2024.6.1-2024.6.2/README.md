# Comparing `tmp/aiocloudweather-2024.6.1.tar.gz` & `tmp/aiocloudweather-2024.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocloudweather-2024.6.1.tar", last modified: Sat Jun  1 21:01:06 2024, max compression
+gzip compressed data, was "aiocloudweather-2024.6.2.tar", last modified: Sat Jun  1 21:59:13 2024, max compression
```

## Comparing `aiocloudweather-2024.6.1.tar` & `aiocloudweather-2024.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/aiocloudweather/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/aiocloudweather/station.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/aiocloudweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 21:01:06.000000 aiocloudweather-2024.6.1/aiocloudweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:01:06.222184 aiocloudweather-2024.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 21:00:58.000000 aiocloudweather-2024.6.1/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.190159 aiocloudweather-2024.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:59:13.190159 aiocloudweather-2024.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.186159 aiocloudweather-2024.6.2/aiocloudweather/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/station.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.186159 aiocloudweather-2024.6.2/aiocloudweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-01 21:59:13.190159 aiocloudweather-2024.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.186159 aiocloudweather-2024.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/tests/test_server.py
```

### Comparing `aiocloudweather-2024.6.1/LICENSE` & `aiocloudweather-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/PKG-INFO` & `aiocloudweather-2024.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.6.1/aiocloudweather/__main__.py` & `aiocloudweather-2024.6.2/aiocloudweather/__main__.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/aiocloudweather/const.py` & `aiocloudweather-2024.6.2/aiocloudweather/const.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/aiocloudweather/conversion.py` & `aiocloudweather-2024.6.2/aiocloudweather/conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,62 +20,62 @@
     return decorator
 
 
 # imperial shenanigans
 @unit(UnitOfTemperature.CELSIUS)
 def fahrenheit_to_celsius(temp_f: float) -> float:
     """Convert Fahrenheit to Celsius."""
-    return round((temp_f - 32) * 5.0 / 9.0, 2)
+    return (temp_f - 32) * 5.0 / 9.0
 
 
 @unit(UnitOfPressure.HPA)
 def inhg_to_hpa(pressure: float) -> float:
     """Convert inches of mercury (inHg) to hectopascals (hPa)."""
-    return round(pressure * 33.864, 2)
+    return pressure * 33.864
 
 
 @unit(UnitOfPrecipitationDepth.MILLIMETERS)
 def in_to_mm(length: float) -> float:
     """Convert inches to millimeters (mm)."""
-    return round(length * 25.4, 2)
+    return length * 25.4
 
 
 @unit(UnitOfIrradiance.WATTS_PER_SQUARE_METER)
 def lux_to_wm2(lux: float) -> float:
     """Convert lux to watts per square meter (W/m²)."""
     return lux * 0.0079
 
 
 @unit(UnitOfSpeed.METERS_PER_SECOND)
 def mph_to_ms(speed: float) -> float:
     """Convert miles per hour (mph) to meters per second (m/s)."""
-    return round(speed * 0.44704, 2)
+    return speed * 0.44704
 
 
 @unit(UnitOfPressure.INHG)
 def hpa_to_inhg(pressure: float) -> float:
     """Convert hectopascals (hPa) to inches of mercury (inHg)."""
-    return round(pressure * 0.02953, 2)
+    return pressure * 0.02953
 
 
 @unit(UnitOfTemperature.FAHRENHEIT)
 def celsius_to_fahrenheit(temp_c: float) -> float:
     """Convert Celsius to Fahrenheit."""
-    return round(temp_c * 9.0 / 5.0 + 32, 2)
+    return temp_c * 9.0 / 5.0 + 32
 
 
 @unit(UnitOfPrecipitationDepth.INCHES)
 def mm_to_in(length: float) -> float:
     """Convert millimeters (mm) to inches."""
-    return round(length * 0.0393701, 2)
+    return length * 0.0393701
 
 
 @unit(LIGHT_LUX)
 def wm2_to_lux(lux: float) -> float:
     """Convert watts per square meter (W/m²) to lux."""
     return lux * 127
 
 
 @unit(UnitOfSpeed.MILES_PER_HOUR)
 def ms_to_mph(speed: float) -> float:
     """Convert meters per second (m/s) to miles per hour (mph)."""
-    return round(speed * 2.23694, 2)
+    return speed * 2.23694
```

### Comparing `aiocloudweather-2024.6.1/aiocloudweather/server.py` & `aiocloudweather-2024.6.2/aiocloudweather/server.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/aiocloudweather/station.py` & `aiocloudweather-2024.6.2/aiocloudweather/station.py`

 * *Files 7% similar despite different names*

```diff
@@ -189,29 +189,29 @@
     station_key: str
     station_sw_version: str = field(default=None)
     station_client_ip: str = field(default=None)
     update_time: float = field(default=None)
 
     date_utc: str = field(default=None)
 
-    barometer: Sensor = field(default=None)
-    temperature: Sensor = field(default=None)
-    humidity: Sensor = field(default=None)
-    indoor_temperature: Sensor = field(default=None)
-    indoor_humidity: Sensor = field(default=None)
-    dewpoint: Sensor = field(default=None)
-    rain: Sensor = field(default=None)
-    daily_rain: Sensor = field(default=None)
-    wind_direction: Sensor = field(default=None)
-    wind_speed: Sensor = field(default=None)
-    wind_gust_speed: Sensor = field(default=None)
-    wind_gust_direction: Sensor = field(default=None)
-    uv: Sensor = field(default=None)
-    solar_radiation: Sensor = field(default=None)
-    heat_index: Sensor = field(default=None)
+    barometer: Sensor = field(default=None, metadata={"name": "Absolute Pressure"})
+    temperature: Sensor = field(default=None, metadata={"name": "Outdoor Temperature"})
+    humidity: Sensor = field(default=None, metadata={"name": "Outdoor Humidity"})
+    indoor_temperature: Sensor = field(default=None, metadata={"name": "Indoor Temperature"})
+    indoor_humidity: Sensor = field(default=None, metadata={"name": "Indoor Humidity"})
+    dewpoint: Sensor = field(default=None, metadata={"name": "Outdoor Dewpoint"})
+    rain: Sensor = field(default=None, metadata={"name": "Rain Rate"})
+    daily_rain: Sensor = field(default=None, metadata={"name": "Daily Rain Rate"})
+    wind_direction: Sensor = field(default=None, metadata={"name": "Wind Direction"})
+    wind_speed: Sensor = field(default=None, metadata={"name": "Wind Speed"})
+    wind_gust_speed: Sensor = field(default=None, metadata={"name": "Wind Gust"})
+    wind_gust_direction: Sensor = field(default=None, metadata={"name": "Wind Gust Direction"})
+    uv: Sensor = field(default=None, metadata={"name": "UV Index"})
+    solar_radiation: Sensor = field(default=None, metadata={"name": "Solar Radiation"})
+    heat_index: Sensor = field(default=None, metadata={"name": "Heat Index"})
 
     @staticmethod
     def from_wunderground(data: WundergroundRawSensor) -> "WeatherStation":
         """
         Converts raw sensor data from the Wunderground API into a WeatherStation object.
 
         Args:
```

### Comparing `aiocloudweather-2024.6.1/aiocloudweather.egg-info/PKG-INFO` & `aiocloudweather-2024.6.2/aiocloudweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.6.1/aiocloudweather.egg-info/SOURCES.txt` & `aiocloudweather-2024.6.2/aiocloudweather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/setup.cfg` & `aiocloudweather-2024.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/setup.py` & `aiocloudweather-2024.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2024.6.1"
+VERSION = "2024.6.2"
 
 
 setup(
     name="aiocloudweather",
     version=VERSION,
     url="https://github.com/lhw/aiocloudweather",
     download_url="https://github.com/lhw/aiocloudweather",
```

### Comparing `aiocloudweather-2024.6.1/tests/test_conversion.py` & `aiocloudweather-2024.6.2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/tests/test_sensor.py` & `aiocloudweather-2024.6.2/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.1/tests/test_server.py` & `aiocloudweather-2024.6.2/tests/test_server.py`

 * *Files identical despite different names*

