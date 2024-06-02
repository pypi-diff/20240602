# Comparing `tmp/aiocloudweather-2024.6.2.tar.gz` & `tmp/aiocloudweather-2024.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocloudweather-2024.6.2.tar", last modified: Sat Jun  1 21:59:13 2024, max compression
+gzip compressed data, was "aiocloudweather-2024.6.3.tar", last modified: Sat Jun  1 22:38:20 2024, max compression
```

## Comparing `aiocloudweather-2024.6.2.tar` & `aiocloudweather-2024.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.190159 aiocloudweather-2024.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:59:13.190159 aiocloudweather-2024.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.186159 aiocloudweather-2024.6.2/aiocloudweather/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/aiocloudweather/station.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.186159 aiocloudweather-2024.6.2/aiocloudweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 21:59:13.000000 aiocloudweather-2024.6.2/aiocloudweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-01 21:59:13.190159 aiocloudweather-2024.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:59:13.186159 aiocloudweather-2024.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 21:59:05.000000 aiocloudweather-2024.6.2/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:38:20.577376 aiocloudweather-2024.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 22:38:20.577376 aiocloudweather-2024.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:38:20.573376 aiocloudweather-2024.6.3/aiocloudweather/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/aiocloudweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/aiocloudweather/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/aiocloudweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/aiocloudweather/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/aiocloudweather/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/aiocloudweather/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/aiocloudweather/station.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:38:20.577376 aiocloudweather-2024.6.3/aiocloudweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 22:38:20.000000 aiocloudweather-2024.6.3/aiocloudweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 22:38:20.000000 aiocloudweather-2024.6.3/aiocloudweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:38:20.000000 aiocloudweather-2024.6.3/aiocloudweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 22:38:20.000000 aiocloudweather-2024.6.3/aiocloudweather.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:38:20.000000 aiocloudweather-2024.6.3/aiocloudweather.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 22:38:20.000000 aiocloudweather-2024.6.3/aiocloudweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 22:38:20.000000 aiocloudweather-2024.6.3/aiocloudweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-01 22:38:20.577376 aiocloudweather-2024.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:38:20.577376 aiocloudweather-2024.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 22:38:12.000000 aiocloudweather-2024.6.3/tests/test_server.py
```

### Comparing `aiocloudweather-2024.6.2/LICENSE` & `aiocloudweather-2024.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/PKG-INFO` & `aiocloudweather-2024.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.6.2
+Version: 2024.6.3
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.6.2/aiocloudweather/__main__.py` & `aiocloudweather-2024.6.3/aiocloudweather/__main__.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/aiocloudweather/const.py` & `aiocloudweather-2024.6.3/aiocloudweather/const.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/aiocloudweather/conversion.py` & `aiocloudweather-2024.6.3/aiocloudweather/conversion.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/aiocloudweather/server.py` & `aiocloudweather-2024.6.3/aiocloudweather/server.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/aiocloudweather/station.py` & `aiocloudweather-2024.6.3/aiocloudweather/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,49 +51,49 @@
     )
     temperature: float = field(
         default=None, metadata={"unit": UnitOfTemperature.FAHRENHEIT, "arg": "tempf"}
     )
     humidity: float = field(
         default=None, metadata={"unit": PERCENTAGE, "arg": "humidity"}
     )
-    indoor_temperature: float = field(
+    indoortemperature: float = field(
         default=None,
         metadata={"unit": UnitOfTemperature.FAHRENHEIT, "arg": "indoortempf"},
     )
-    indoor_humidity: float = field(
+    indoorhumidity: float = field(
         default=None, metadata={"unit": PERCENTAGE, "arg": "indoorhumidity"}
     )
 
     dewpoint: float = field(
         default=None, metadata={"unit": UnitOfTemperature.FAHRENHEIT, "arg": "dewptf"}
     )
     rain: float = field(
         default=None,
         metadata={"unit": UnitOfPrecipitationDepth.INCHES, "arg": "rainin"},
     )
-    daily_rain: float = field(
+    dailyrain: float = field(
         default=None,
         metadata={"unit": UnitOfPrecipitationDepth.INCHES, "arg": "dailyrainin"},
     )
-    wind_direction: float = field(
+    winddirection: float = field(
         default=None, metadata={"unit": DEGREE, "arg": "winddir"}
     )
-    wind_speed: float = field(
+    windspeed: float = field(
         default=None,
         metadata={"unit": UnitOfSpeed.MILES_PER_HOUR, "arg": "windspeedmph"},
     )
-    wind_gust_speed: float = field(
+    windgustspeed: float = field(
         default=None,
         metadata={"unit": UnitOfSpeed.MILES_PER_HOUR, "arg": "windgustmph"},
     )
-    wind_gust_direction: float = field(
+    windgustdirection: float = field(
         default=None, metadata={"unit": DEGREE, "arg": "windgustdir"}
     )
     uv: int = field(default=None, metadata={"unit": UV_INDEX, "arg": "UV"})
-    solar_radiation: float = field(
+    solarradiation: float = field(
         default=None, metadata={"unit": LIGHT_LUX, "arg": "solarRadiation"}
     )
 
 
 @dataclass
 class WeathercloudRawSensor:
     """WeatherCloud API sensor parsed from the query path."""
@@ -106,49 +106,49 @@
     barometer: int = field(
         default=None, metadata={"unit": UnitOfPressure.HPA, "arg": "bar"}
     )
     temperature: int = field(
         default=None, metadata={"unit": UnitOfTemperature.CELSIUS, "arg": "temp"}
     )
     humidity: int = field(default=None, metadata={"unit": PERCENTAGE, "arg": "hum"})
-    indoor_temperature: int = field(
+    indoortemperature: int = field(
         default=None, metadata={"unit": UnitOfTemperature.CELSIUS, "arg": "tempin"}
     )
-    indoor_humidity: int = field(
+    indoorhumidity: int = field(
         default=None, metadata={"unit": PERCENTAGE, "arg": "humin"}
     )
     dewpoint: int = field(
         default=None, metadata={"unit": UnitOfTemperature.CELSIUS, "arg": "dew"}
     )
-    heat_index: int = field(
+    heatindex: int = field(
         default=None, metadata={"unit": UnitOfTemperature.CELSIUS, "arg": "heat"}
     )
-    daily_rain: int = field(
+    dailyrain: int = field(
         default=None,
         metadata={"unit": UnitOfPrecipitationDepth.MILLIMETERS, "arg": "rain"},
     )
     rain: int = field(
         default=None,
         metadata={
             "unit": UnitOfVolumetricFlux.MILLIMETERS_PER_HOUR,
             "arg": "rainrate",
         },
     )
-    wind_direction: int = field(default=None, metadata={"unit": DEGREE, "arg": "wdir"})
-    wind_speed: int = field(
+    winddirection: int = field(default=None, metadata={"unit": DEGREE, "arg": "wdir"})
+    windspeed: int = field(
         default=None, metadata={"unit": UnitOfSpeed.METERS_PER_SECOND, "arg": "wspd"}
     )
-    wind_gust_speed: int = field(
+    windgustspeed: int = field(
         default=None, metadata={"unit": UnitOfSpeed.METERS_PER_SECOND, "arg": "wspdhi"}
     )
-    wind_chill: int = field(
+    windchill: int = field(
         default=None, metadata={"unit": UnitOfTemperature.CELSIUS, "arg": "chill"}
     )
     uv: int = field(default=None, metadata={"unit": UV_INDEX, "arg": "uvi"})
-    solar_radiation: int = field(
+    solarradiation: int = field(
         default=None,
         metadata={"unit": UnitOfIrradiance.WATTS_PER_SQUARE_METER, "arg": "solarrad"},
     )
 
 
 IMPERIAL_TO_METRIC: Final = {
     UnitOfPressure.INHG: inhg_to_hpa,
@@ -192,26 +192,30 @@
     update_time: float = field(default=None)
 
     date_utc: str = field(default=None)
 
     barometer: Sensor = field(default=None, metadata={"name": "Absolute Pressure"})
     temperature: Sensor = field(default=None, metadata={"name": "Outdoor Temperature"})
     humidity: Sensor = field(default=None, metadata={"name": "Outdoor Humidity"})
-    indoor_temperature: Sensor = field(default=None, metadata={"name": "Indoor Temperature"})
-    indoor_humidity: Sensor = field(default=None, metadata={"name": "Indoor Humidity"})
+    indoortemperature: Sensor = field(
+        default=None, metadata={"name": "Indoor Temperature"}
+    )
+    indoorhumidity: Sensor = field(default=None, metadata={"name": "Indoor Humidity"})
     dewpoint: Sensor = field(default=None, metadata={"name": "Outdoor Dewpoint"})
     rain: Sensor = field(default=None, metadata={"name": "Rain Rate"})
-    daily_rain: Sensor = field(default=None, metadata={"name": "Daily Rain Rate"})
-    wind_direction: Sensor = field(default=None, metadata={"name": "Wind Direction"})
-    wind_speed: Sensor = field(default=None, metadata={"name": "Wind Speed"})
-    wind_gust_speed: Sensor = field(default=None, metadata={"name": "Wind Gust"})
-    wind_gust_direction: Sensor = field(default=None, metadata={"name": "Wind Gust Direction"})
+    dailyrain: Sensor = field(default=None, metadata={"name": "Daily Rain Rate"})
+    winddirection: Sensor = field(default=None, metadata={"name": "Wind Direction"})
+    windspeed: Sensor = field(default=None, metadata={"name": "Wind Speed"})
+    windgustspeed: Sensor = field(default=None, metadata={"name": "Wind Gust"})
+    windgustdirection: Sensor = field(
+        default=None, metadata={"name": "Wind Gust Direction"}
+    )
     uv: Sensor = field(default=None, metadata={"name": "UV Index"})
-    solar_radiation: Sensor = field(default=None, metadata={"name": "Solar Radiation"})
-    heat_index: Sensor = field(default=None, metadata={"name": "Heat Index"})
+    solarradiation: Sensor = field(default=None, metadata={"name": "Solar Radiation"})
+    heatindex: Sensor = field(default=None, metadata={"name": "Heat Index"})
 
     @staticmethod
     def from_wunderground(data: WundergroundRawSensor) -> "WeatherStation":
         """
         Converts raw sensor data from the Wunderground API into a WeatherStation object.
 
         Args:
```

### Comparing `aiocloudweather-2024.6.2/aiocloudweather.egg-info/PKG-INFO` & `aiocloudweather-2024.6.3/aiocloudweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.6.2
+Version: 2024.6.3
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.6.2/aiocloudweather.egg-info/SOURCES.txt` & `aiocloudweather-2024.6.3/aiocloudweather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/setup.cfg` & `aiocloudweather-2024.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/setup.py` & `aiocloudweather-2024.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2024.6.2"
+VERSION = "2024.6.3"
 
 
 setup(
     name="aiocloudweather",
     version=VERSION,
     url="https://github.com/lhw/aiocloudweather",
     download_url="https://github.com/lhw/aiocloudweather",
```

### Comparing `aiocloudweather-2024.6.2/tests/test_conversion.py` & `aiocloudweather-2024.6.3/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.6.2/tests/test_sensor.py` & `aiocloudweather-2024.6.3/tests/test_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
         station_id="12345",
         station_key="12345",
         barometer=29.92,
         temperature=72.5,
         humidity=44,
         dewpoint=49.2,
         rain=0,
-        daily_rain=0,
-        wind_direction=249,
-        wind_speed=2.0,
-        wind_gust_speed=2.7,
+        dailyrain=0,
+        winddirection=249,
+        windspeed=2.0,
+        windgustspeed=2.7,
         uv=2,
-        solar_radiation=289.2,
+        solarradiation=289.2,
     )
     weather_station = WeatherStation.from_wunderground(raw_sensor_data)
 
     assert weather_station.station_id == "12345"
     assert weather_station.station_key == "12345"
     assert round(weather_station.barometer.metric, 2) == 1013.21
     assert weather_station.barometer.metric_unit == "hPa"
@@ -44,20 +44,20 @@
         station_id="12345",
         station_key="12345",
         barometer=10130,
         temperature=160,
         humidity=80,
         dewpoint=129,
         rain=0,
-        daily_rain=0,
-        wind_direction=288,
-        wind_speed=0,
-        wind_gust_speed=0,
+        dailyrain=0,
+        winddirection=288,
+        windspeed=0,
+        windgustspeed=0,
         uv=0,
-        solar_radiation=470,
+        solarradiation=470,
     )
     weather_station = WeatherStation.from_weathercloud(raw_sensor_data)
 
     assert weather_station.station_id == "12345"
     assert weather_station.station_key == "12345"
     assert weather_station.barometer.metric == 1013
     assert weather_station.barometer.metric_unit == "hPa"
```

### Comparing `aiocloudweather-2024.6.2/tests/test_server.py` & `aiocloudweather-2024.6.3/tests/test_server.py`

 * *Files identical despite different names*

