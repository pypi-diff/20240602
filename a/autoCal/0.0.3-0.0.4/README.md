# Comparing `tmp/autocal-0.0.3.tar.gz` & `tmp/autocal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocal-0.0.3.tar", last modified: Fri May 31 18:25:40 2024, max compression
+gzip compressed data, was "autocal-0.0.4.tar", last modified: Sun Jun  2 12:16:02 2024, max compression
```

## Comparing `autocal-0.0.3.tar` & `autocal-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 18:25:40.086303 autocal-0.0.3/
--rw-rw-rw-   0        0        0     1093 2024-05-29 03:14:51.000000 autocal-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      737 2024-05-31 18:25:40.086303 autocal-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-05-29 03:14:51.000000 autocal-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 18:25:40.078098 autocal-0.0.3/autoCal/
--rw-rw-rw-   0        0        0       99 2024-05-30 04:06:40.000000 autocal-0.0.3/autoCal/__init__.py
--rw-rw-rw-   0        0        0      500 2024-05-30 04:07:36.000000 autocal-0.0.3/autoCal/helperConverters.py
--rw-rw-rw-   0        0        0     5318 2024-05-31 18:23:55.000000 autocal-0.0.3/autoCal/motorCalculations.py
--rw-rw-rw-   0        0        0     2890 2024-05-30 04:12:24.000000 autocal-0.0.3/autoCal/speedCalculations.py
--rw-rw-rw-   0        0        0      861 2024-04-20 13:21:51.000000 autocal-0.0.3/autoCal/unitConverters.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:25:40.086303 autocal-0.0.3/autoCal.egg-info/
--rw-rw-rw-   0        0        0      737 2024-05-31 18:25:40.000000 autocal-0.0.3/autoCal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-31 18:25:40.000000 autocal-0.0.3/autoCal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 18:25:40.000000 autocal-0.0.3/autoCal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-31 18:25:40.000000 autocal-0.0.3/autoCal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 18:25:40.093115 autocal-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1036 2024-05-31 18:25:15.000000 autocal-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:16:02.692655 autocal-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2024-05-29 03:14:51.000000 autocal-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      737 2024-06-02 12:16:02.692655 autocal-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3067 2024-06-02 11:35:08.000000 autocal-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 12:16:02.682881 autocal-0.0.4/autoCal/
+-rw-rw-rw-   0        0        0       99 2024-05-30 04:06:40.000000 autocal-0.0.4/autoCal/__init__.py
+-rw-rw-rw-   0        0        0      500 2024-05-30 04:07:36.000000 autocal-0.0.4/autoCal/helperConverters.py
+-rw-rw-rw-   0        0        0     5320 2024-06-02 10:35:28.000000 autocal-0.0.4/autoCal/motorCalculations.py
+-rw-rw-rw-   0        0        0     2890 2024-05-30 04:12:24.000000 autocal-0.0.4/autoCal/speedCalculations.py
+-rw-rw-rw-   0        0        0      861 2024-04-20 13:21:51.000000 autocal-0.0.4/autoCal/unitConverters.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:16:02.692655 autocal-0.0.4/autoCal.egg-info/
+-rw-rw-rw-   0        0        0      737 2024-06-02 12:16:02.000000 autocal-0.0.4/autoCal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-06-02 12:16:02.000000 autocal-0.0.4/autoCal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:16:02.000000 autocal-0.0.4/autoCal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 12:16:02.000000 autocal-0.0.4/autoCal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:16:02.692655 autocal-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2024-06-02 10:36:09.000000 autocal-0.0.4/setup.py
```

### Comparing `autocal-0.0.3/LICENSE` & `autocal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autocal-0.0.3/PKG-INFO` & `autocal-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoCal
-Version: 0.0.3
+Version: 0.0.4
 Summary: Collection of automotive calculations
 Author: GladsonThomas
 Author-email: <gladson.thomas.official@gmail.com>
 Keywords: python,calculations,automotive,EV,BLDC
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autocal-0.0.3/autoCal/motorCalculations.py` & `autocal-0.0.4/autoCal/motorCalculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,29 +138,29 @@
     Returns:
         float: returns time interval in seconds
     """
     T = motor_rpm_to_one_motor_rotation_time(motor_rpm)
     hall_event_count = get_hall_events_per_motor_rotation(pole_pairs)
     return T / hall_event_count
 
-def get_hall_event_per_second(motor_rpm: float, pole_pairs: int) -> float:
+def get_hall_events_per_second(motor_rpm: float, pole_pairs: int) -> float:
     """calculates the number of hall events per second
 
     Args:
         motor_rpm (float): RPM of motor
         pole_pairs (int): number of pole pairs
 
     Returns:
         float: returns number of hall events
     """
     rps = motor_rpm / 60
     hall_event_count = get_hall_events_per_motor_rotation(pole_pairs)
     return hall_event_count * rps
 
-def get_hall_event_per_minute(motor_rpm: float, pole_pairs: float) -> float:
+def get_hall_events_per_minute(motor_rpm: float, pole_pairs: float) -> float:
     """Calculates the number of hall events per minute
 
     Args:
         motor_rpm (float): RPM of motor
         pole_pairs (float): number of pole pairs
 
     Returns:
```

### Comparing `autocal-0.0.3/autoCal/speedCalculations.py` & `autocal-0.0.4/autoCal/speedCalculations.py`

 * *Files identical despite different names*

### Comparing `autocal-0.0.3/autoCal/unitConverters.py` & `autocal-0.0.4/autoCal/unitConverters.py`

 * *Files identical despite different names*

### Comparing `autocal-0.0.3/autoCal.egg-info/PKG-INFO` & `autocal-0.0.4/autoCal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoCal
-Version: 0.0.3
+Version: 0.0.4
 Summary: Collection of automotive calculations
 Author: GladsonThomas
 Author-email: <gladson.thomas.official@gmail.com>
 Keywords: python,calculations,automotive,EV,BLDC
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autocal-0.0.3/setup.py` & `autocal-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Collection of automotive calculations'
 LONG_DESCRIPTION = 'This repository provides a collection of mathematical formulas commonly used in the automotive industry, with a particular focus on Brushless DC (BLDC) motors.'
 
 # Setting up
 setup(
     name="autoCal",
     version=VERSION,
```

