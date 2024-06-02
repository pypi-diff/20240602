# Comparing `tmp/open_meteo_solar_forecast-0.1.7.tar.gz` & `tmp/open_meteo_solar_forecast-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.1.7.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.1.8.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.1.7.tar` & `open_meteo_solar_forecast-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.7/LICENSE
--rw-r--r--   0        0        0     3979 2024-05-26 17:44:13.223434 open_meteo_solar_forecast-0.1.7/README.md
--rw-r--r--   0        0        0     3198 2024-05-30 22:10:23.211954 open_meteo_solar_forecast-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0      554 2024-05-30 22:09:29.625038 open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4526 2024-05-30 17:22:12.800223 open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     9546 2024-05-30 22:02:35.889738 open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-06-02 10:29:31.677122 open_meteo_solar_forecast-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3979 2024-06-02 10:29:31.677122 open_meteo_solar_forecast-0.1.8/README.md
+-rw-r--r--   0        0        0     3198 2024-06-02 16:09:05.477607 open_meteo_solar_forecast-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-06-02 10:29:31.680455 open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0      593 2024-06-02 16:06:15.049849 open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-06-02 10:29:31.680455 open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-06-02 10:29:31.680455 open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     8365 2024-06-02 16:06:52.350800 open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:29:31.680455 open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.8/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.1.7/LICENSE` & `open_meteo_solar_forecast-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.7/README.md` & `open_meteo_solar_forecast-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.7/pyproject.toml` & `open_meteo_solar_forecast-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.1.7"
+version = "0.1.8"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Rany <rany@riseup.net>", "Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/constants.py` & `open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Constants for the solar forecast module."""
 
 # STC specifies a cell temperature of 25°C and an irradiance of 1000 W/m².
-# NOCT specifies a cell temperature of 45°C and an irradiance of 800 W/m².
-# The temperature coefficient of the solar panel is 0.004°C⁻¹.
+# NOCT specifies a cell temperature of 45°C, an irradiance of 800 W/m²
+# and an ambient temperature of 20°C.
+#
+# The temperature coefficient of most solar panels is 0.004°C⁻¹.
 #
 # Source: https://www.researchgate.net/publication/372240079_Solar_Prediction_Strategy_for_Managing_Virtual_Power_Stations
 ALPHA_TEMP = -0.004  # °C-1
 G_NOCT = 800.0  # W/m2
 G_STC = 1000.0  # W/m2
 TEMP_NOCT_AMB = 20.0  # °C
 TEMP_NOCT_CELL = 45.0  # °C
```

### Comparing `open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/models.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.7/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.1.8/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,27 +136,26 @@
 
         """
         params = {
             "latitude": str(self.latitude),
             "longitude": str(self.longitude),
             "azimuth": str(self.azimuth),
             "tilt": str(self.declination),
-            "minutely_15": "temperature_2m,cloud_cover_low"
+            "minutely_15": "temperature_2m"
             ",global_tilted_irradiance,global_tilted_irradiance_instant",
             "forecast_days": str(self.forecast_days),
             "past_days": str(self.past_days),
             "timezone": "auto",
         }
         data = await self._request(
             "/v1/forecast",
             params=params,
         )
         gti_avg_arr = data["minutely_15"]["global_tilted_irradiance"]
         gti_instant_arr = data["minutely_15"]["global_tilted_irradiance_instant"]
-        cloud_cover_arr = data["minutely_15"]["cloud_cover_low"]
         temp_arr = data["minutely_15"]["temperature_2m"]
         utc_offset = data["utc_offset_seconds"]
         time_arr = [
             dt.strptime(time, "%Y-%m-%dT%H:%M").replace(
                 tzinfo=timezone(timedelta(seconds=utc_offset))
             )
             for time in data["minutely_15"]["time"]
@@ -164,76 +163,54 @@
 
         peak_power = self.kwp * 1000  # Convert kW to W
 
         power_avg: dict[dt, int] = {}
         watts_instant: dict[dt, int] = {}
         wh_days: dict[dt, int] = {}
 
-        def gen_power(gti: float, t_amb: float, cloud_cover: float = 0) -> int:
+        def gen_power(gti: float, t_amb: float) -> int:
             """Calculate the power generated by a solar panel.
 
             Formulas:
             ---------
-                Power and temperature calculations are based on the following formulas:
-                    Tc=Ta + (NOCT-Tnoct) / Gnoct*G  (p.509)
-                    P=Pmax * (G/Gstc) * (1 + α * (Tc-Tstc)) * ηDC (p.509)
-                    Source: https://www.researchgate.net/publication/372240079_Solar_Prediction_Strategy_for_Managing_Virtual_Power_Stations
-
-                Cloud compensation factor (Kasten-Czeplak) is calculated as follows:
-                    CCF = 1 - 0.75 * (cloud_cover / 100) ^ 3.4
-                    Source: https://www.researchgate.net/publication/319018945_Evaluation_of_Cloud_Cover_Based_Model_for_Simulation_of_Hourly_Global_Solar_Radiation_in_Western_Canada
+                Tc=Ta + (NOCT-Tnoct) / Gnoct*G  (p.509)
+                P=Pmax * (G/Gstc) * (1 + α * (Tc-Tstc)) * ηDC (p.509)
+                Source: https://www.researchgate.net/publication/372240079_Solar_Prediction_Strategy_for_Managing_Virtual_Power_Stations
             """
             temp_cell = t_amb + (TEMP_NOCT_CELL - TEMP_NOCT_AMB) / G_NOCT * gti
-            ccf = 1 - 0.75 * pow(cloud_cover / 100.0, 3.4)
-            gti *= ccf
             power = (
                 peak_power
                 * (gti / G_STC)
                 * (1 + ALPHA_TEMP * (temp_cell - TEMP_STC_CELL))
             ) * self.efficiency_factor
             return round(max(0, power))
 
         for i, time in enumerate(time_arr):
             # If any of the values are missing, skip the iteration
             if None in (
                 gti_avg_arr[i],
                 gti_instant_arr[i],
                 *(temp_arr[i], temp_arr[i - 1] if i > 0 else temp_arr[i]),
-                *(
-                    (cloud_cover_arr[i], cloud_cover_arr[i - 1])
-                    if i > 0
-                    else (cloud_cover_arr[i],)
-                ),
             ):
                 continue
 
             # Total radiation received on a tilted pane
             gti_avg = gti_avg_arr[i]
             gti_instant = gti_instant_arr[i]
 
-            # Get the temperature and cloud cover
+            # Get the temperature
             temp_instant = temp_arr[i - 1] if i > 0 else temp_arr[i]
             temp_avg = (temp_arr[i] + temp_arr[i - 1]) / 2 if i > 0 else temp_arr[i]
-            cloud_cover_instant = (
-                cloud_cover_arr[i - 1] if i > 0 else cloud_cover_arr[i]
-            )
-            cloud_cover_avg = (
-                (cloud_cover_arr[i] + cloud_cover_arr[i - 1]) / 2
-                if i > 0
-                else cloud_cover_arr[i]
-            )
 
             # For minutely data, the time_start is 15 minutes before the current time
             time_start = time - timedelta(minutes=15)
 
             # Calculate and store the power generated
-            power_avg[time_start] = gen_power(gti_avg, temp_avg, cloud_cover_avg)
-            watts_instant[time_start] = gen_power(
-                gti_instant, temp_instant, cloud_cover_instant
-            )
+            power_avg[time_start] = gen_power(gti_avg, temp_avg)
+            watts_instant[time_start] = gen_power(gti_instant, temp_instant)
 
         # Calculate the average power generated per hour
         wh_period: dict[dt, int] = {}
         wh_period_count: dict[dt, int] = {}
         for time, power in power_avg.items():
             hour = time.replace(minute=0, second=0, microsecond=0)
             wh_period[hour] = wh_period.get(hour, 0) + power
```

### Comparing `open_meteo_solar_forecast-0.1.7/PKG-INFO` & `open_meteo_solar_forecast-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.1.7
+Version: 0.1.8
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Rany
 Author-email: rany@riseup.net
 Maintainer: Rany
```

