# Comparing `tmp/autocal-0.0.5.tar.gz` & `tmp/autocal-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocal-0.0.5.tar", last modified: Sun Jun  2 12:36:31 2024, max compression
+gzip compressed data, was "autocal-0.0.6.tar", last modified: Sun Jun  2 12:42:07 2024, max compression
```

## Comparing `autocal-0.0.5.tar` & `autocal-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 12:36:31.930631 autocal-0.0.5/
--rw-rw-rw-   0        0        0     1093 2024-05-29 03:14:51.000000 autocal-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3645 2024-06-02 12:36:31.930631 autocal-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3067 2024-06-02 11:35:08.000000 autocal-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 12:36:31.924168 autocal-0.0.5/autoCal/
--rw-rw-rw-   0        0        0       99 2024-05-30 04:06:40.000000 autocal-0.0.5/autoCal/__init__.py
--rw-rw-rw-   0        0        0      500 2024-05-30 04:07:36.000000 autocal-0.0.5/autoCal/helperConverters.py
--rw-rw-rw-   0        0        0     5320 2024-06-02 10:35:28.000000 autocal-0.0.5/autoCal/motorCalculations.py
--rw-rw-rw-   0        0        0     2890 2024-05-30 04:12:24.000000 autocal-0.0.5/autoCal/speedCalculations.py
--rw-rw-rw-   0        0        0      861 2024-04-20 13:21:51.000000 autocal-0.0.5/autoCal/unitConverters.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:36:31.930631 autocal-0.0.5/autoCal.egg-info/
--rw-rw-rw-   0        0        0     3645 2024-06-02 12:36:31.000000 autocal-0.0.5/autoCal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-06-02 12:36:31.000000 autocal-0.0.5/autoCal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 12:36:31.000000 autocal-0.0.5/autoCal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-06-02 12:36:31.000000 autocal-0.0.5/autoCal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 12:36:31.930631 autocal-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1101 2024-06-02 12:36:28.000000 autocal-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:07.097775 autocal-0.0.6/
+-rw-rw-rw-   0        0        0     1093 2024-05-29 03:14:51.000000 autocal-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3655 2024-06-02 12:42:07.097775 autocal-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3077 2024-06-02 12:41:14.000000 autocal-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:07.083582 autocal-0.0.6/autoCal/
+-rw-rw-rw-   0        0        0       99 2024-05-30 04:06:40.000000 autocal-0.0.6/autoCal/__init__.py
+-rw-rw-rw-   0        0        0      500 2024-05-30 04:07:36.000000 autocal-0.0.6/autoCal/helperConverters.py
+-rw-rw-rw-   0        0        0     5320 2024-06-02 10:35:28.000000 autocal-0.0.6/autoCal/motorCalculations.py
+-rw-rw-rw-   0        0        0     2890 2024-05-30 04:12:24.000000 autocal-0.0.6/autoCal/speedCalculations.py
+-rw-rw-rw-   0        0        0      861 2024-04-20 13:21:51.000000 autocal-0.0.6/autoCal/unitConverters.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:07.097236 autocal-0.0.6/autoCal.egg-info/
+-rw-rw-rw-   0        0        0     3655 2024-06-02 12:42:07.000000 autocal-0.0.6/autoCal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-06-02 12:42:07.000000 autocal-0.0.6/autoCal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:42:07.000000 autocal-0.0.6/autoCal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 12:42:07.000000 autocal-0.0.6/autoCal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:42:07.097775 autocal-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2024-06-02 12:41:56.000000 autocal-0.0.6/setup.py
```

### Comparing `autocal-0.0.5/LICENSE` & `autocal-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autocal-0.0.5/PKG-INFO` & `autocal-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoCal
-Version: 0.0.5
+Version: 0.0.6
 Summary: Collection of automotive calculations
 Author: GladsonThomas
 Author-email: <gladson.thomas.official@gmail.com>
 Keywords: python,calculations,automotive,EV,BLDC
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,17 @@
 wheel_rpm_to_mph(wheel_rpm: float, tyre_size: float) -> float:
 kmph_to_wheel_rpm(kmph: float, tyre_size: float) -> float:
 mph_to_wheel_rpm(mph: float, tyre_size: float) -> float:
 wheel_rpm_to_time_required_for_one_wheel_rotation(rpm: float) -> float:
 kmph_to_time_required_for_one_wheel_rotation(kmph: float, tyre_size: float) -> float:
 mph_to_time_required_for_one_wheel_rotation(mph: float, tyre_size: float) -> float:
 ```
-
+<br><br>
 **Motor Calculations**: This contains the formulas related to BLDC motors.
+
 List of functions:
 ```python
 motor_rpm_to_kmph(motor_rpm: float, tyre_size: float, drivetrain_ratio: float) -> float:
 motor_rpm_to_mph(motor_rpm: float, tyre_size: float, drivetrain_ratio: float) -> float:
 kmph_to_motor_rpm(kmph: float, tyre_size: float, drivetrain_ratio: float) -> float:
 mph_to_motor_rpm(mph: float, tyre_size: float, drivetrain_ratio: float) -> float:
 wheel_rpm_to_motor_rpm(wheel_rpm: float, drivetrain_ratio: float) -> float:
```

### Comparing `autocal-0.0.5/README.md` & `autocal-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 wheel_rpm_to_mph(wheel_rpm: float, tyre_size: float) -> float:
 kmph_to_wheel_rpm(kmph: float, tyre_size: float) -> float:
 mph_to_wheel_rpm(mph: float, tyre_size: float) -> float:
 wheel_rpm_to_time_required_for_one_wheel_rotation(rpm: float) -> float:
 kmph_to_time_required_for_one_wheel_rotation(kmph: float, tyre_size: float) -> float:
 mph_to_time_required_for_one_wheel_rotation(mph: float, tyre_size: float) -> float:
 ```
-
+<br><br>
 **Motor Calculations**: This contains the formulas related to BLDC motors.
+
 List of functions:
 ```python
 motor_rpm_to_kmph(motor_rpm: float, tyre_size: float, drivetrain_ratio: float) -> float:
 motor_rpm_to_mph(motor_rpm: float, tyre_size: float, drivetrain_ratio: float) -> float:
 kmph_to_motor_rpm(kmph: float, tyre_size: float, drivetrain_ratio: float) -> float:
 mph_to_motor_rpm(mph: float, tyre_size: float, drivetrain_ratio: float) -> float:
 wheel_rpm_to_motor_rpm(wheel_rpm: float, drivetrain_ratio: float) -> float:
```

### Comparing `autocal-0.0.5/autoCal/motorCalculations.py` & `autocal-0.0.6/autoCal/motorCalculations.py`

 * *Files identical despite different names*

### Comparing `autocal-0.0.5/autoCal/speedCalculations.py` & `autocal-0.0.6/autoCal/speedCalculations.py`

 * *Files identical despite different names*

### Comparing `autocal-0.0.5/autoCal/unitConverters.py` & `autocal-0.0.6/autoCal/unitConverters.py`

 * *Files identical despite different names*

### Comparing `autocal-0.0.5/autoCal.egg-info/PKG-INFO` & `autocal-0.0.6/autoCal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoCal
-Version: 0.0.5
+Version: 0.0.6
 Summary: Collection of automotive calculations
 Author: GladsonThomas
 Author-email: <gladson.thomas.official@gmail.com>
 Keywords: python,calculations,automotive,EV,BLDC
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,17 @@
 wheel_rpm_to_mph(wheel_rpm: float, tyre_size: float) -> float:
 kmph_to_wheel_rpm(kmph: float, tyre_size: float) -> float:
 mph_to_wheel_rpm(mph: float, tyre_size: float) -> float:
 wheel_rpm_to_time_required_for_one_wheel_rotation(rpm: float) -> float:
 kmph_to_time_required_for_one_wheel_rotation(kmph: float, tyre_size: float) -> float:
 mph_to_time_required_for_one_wheel_rotation(mph: float, tyre_size: float) -> float:
 ```
-
+<br><br>
 **Motor Calculations**: This contains the formulas related to BLDC motors.
+
 List of functions:
 ```python
 motor_rpm_to_kmph(motor_rpm: float, tyre_size: float, drivetrain_ratio: float) -> float:
 motor_rpm_to_mph(motor_rpm: float, tyre_size: float, drivetrain_ratio: float) -> float:
 kmph_to_motor_rpm(kmph: float, tyre_size: float, drivetrain_ratio: float) -> float:
 mph_to_motor_rpm(mph: float, tyre_size: float, drivetrain_ratio: float) -> float:
 wheel_rpm_to_motor_rpm(wheel_rpm: float, drivetrain_ratio: float) -> float:
```

### Comparing `autocal-0.0.5/setup.py` & `autocal-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Collection of automotive calculations'
 LONG_DESCRIPTION = 'This repository provides a collection of mathematical formulas commonly used in the automotive industry, with a particular focus on Brushless DC (BLDC) motors.'
 
 with open('README.md') as f:
     long_description = f.read()
 
 # Setting up
```

