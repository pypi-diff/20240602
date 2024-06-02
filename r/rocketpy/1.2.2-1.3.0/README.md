# Comparing `tmp/rocketpy-1.2.2.tar.gz` & `tmp/rocketpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketpy-1.2.2.tar", last modified: Fri Mar 22 09:44:42 2024, max compression
+gzip compressed data, was "rocketpy-1.3.0.tar", last modified: Sun Jun  2 13:31:28 2024, max compression
```

## Comparing `rocketpy-1.2.2.tar` & `rocketpy-1.3.0.tar`

### file list

```diff
@@ -1,99 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.766666 rocketpy-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-22 09:44:36.000000 rocketpy-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17434 2024-03-22 09:44:42.766666 rocketpy-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-03-22 09:44:36.000000 rocketpy-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.750666 rocketpy-1.2.2/rocketpy/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.750666 rocketpy-1.2.2/rocketpy/control/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/control/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.750666 rocketpy-1.2.2/rocketpy/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   152625 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/environment/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)   105954 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/environment/environment_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.750666 rocketpy-1.2.2/rocketpy/mathutils/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   134864 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/mathutils/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/mathutils/vector_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.754666 rocketpy-1.2.2/rocketpy/motors/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/fluid.py
--rw-r--r--   0 runner    (1001) docker     (127)    25788 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/hybrid_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19940 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/liquid_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53785 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28516 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/solid_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53153 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/tank.py
--rw-r--r--   0 runner    (1001) docker     (127)    15006 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/motors/tank_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.754666 rocketpy-1.2.2/rocketpy/plots/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14130 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/aero_surface_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.754666 rocketpy-1.2.2/rocketpy/plots/compare/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/compare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/compare/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)    57569 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/compare/compare_flights.py
--rw-r--r--   0 runner    (1001) docker     (127)    65061 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/environment_analysis_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/environment_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    28824 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/flight_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/fluid_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/hybrid_motor_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/liquid_motor_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    19456 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/motor_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/rocket_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/solid_motor_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/tank_geometry_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/plots/tank_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.758666 rocketpy-1.2.2/rocketpy/prints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/aero_surface_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/compare_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/controller_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/environment_analysis_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/environment_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/flight_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/fluid_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/hybrid_motor_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/liquid_motor_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/motor_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/parachute_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/rocket_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/solid_motor_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/tank_geometry_prints.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/prints/tank_prints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.758666 rocketpy-1.2.2/rocketpy/rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74921 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/rocket/aero_surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/rocket/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/rocket/parachute.py
--rw-r--r--   0 runner    (1001) docker     (127)    62622 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/rocket/rocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.758666 rocketpy-1.2.2/rocketpy/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   157049 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/simulation/flight.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/simulation/flight_data_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    22351 2024-03-22 09:44:37.000000 rocketpy-1.2.2/rocketpy/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.762666 rocketpy-1.2.2/rocketpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17434 2024-03-22 09:44:42.000000 rocketpy-1.2.2/rocketpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-22 09:44:42.000000 rocketpy-1.2.2/rocketpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 09:44:42.000000 rocketpy-1.2.2/rocketpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-22 09:44:42.000000 rocketpy-1.2.2/rocketpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-22 09:44:42.000000 rocketpy-1.2.2/rocketpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 09:44:42.766666 rocketpy-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-22 09:44:37.000000 rocketpy-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:42.762666 rocketpy-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36836 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_environment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    28596 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_flight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_flight_data_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18223 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_genericmotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_hybridmotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_liquidmotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_rocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_solidmotor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28159 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_tank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_tools_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-22 09:44:37.000000 rocketpy-1.2.2/tests/test_tools_vector.py
+drwxr-xr-x   0 phmb      (1000) phmb      (1000)        0 2024-06-02 13:31:28.371206 rocketpy-1.3.0/
+-rw-r--r--   0 phmb      (1000) phmb      (1000)     1079 2024-06-01 17:04:48.000000 rocketpy-1.3.0/LICENSE
+-rw-r--r--   0 phmb      (1000) phmb      (1000)    17419 2024-06-02 13:31:28.371206 rocketpy-1.3.0/PKG-INFO
+-rw-r--r--   0 phmb      (1000) phmb      (1000)    15912 2024-06-01 17:04:48.000000 rocketpy-1.3.0/README.md
+-rw-r--r--   0 phmb      (1000) phmb      (1000)     1624 2024-06-02 13:16:43.000000 rocketpy-1.3.0/pyproject.toml
+drwxr-xr-x   0 phmb      (1000) phmb      (1000)        0 2024-06-02 13:31:28.367206 rocketpy-1.3.0/rocketpy.egg-info/
+-rw-r--r--   0 phmb      (1000) phmb      (1000)    17419 2024-06-02 13:31:28.000000 rocketpy-1.3.0/rocketpy.egg-info/PKG-INFO
+-rw-r--r--   0 phmb      (1000) phmb      (1000)      191 2024-06-02 13:31:28.000000 rocketpy-1.3.0/rocketpy.egg-info/SOURCES.txt
+-rw-r--r--   0 phmb      (1000) phmb      (1000)        1 2024-06-02 13:31:28.000000 rocketpy-1.3.0/rocketpy.egg-info/dependency_links.txt
+-rw-r--r--   0 phmb      (1000) phmb      (1000)      277 2024-06-02 13:31:28.000000 rocketpy-1.3.0/rocketpy.egg-info/requires.txt
+-rw-r--r--   0 phmb      (1000) phmb      (1000)        9 2024-06-02 13:31:28.000000 rocketpy-1.3.0/rocketpy.egg-info/top_level.txt
+-rw-r--r--   0 phmb      (1000) phmb      (1000)       38 2024-06-02 13:31:28.371206 rocketpy-1.3.0/setup.cfg
```

### Comparing `rocketpy-1.2.2/LICENSE` & `rocketpy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketpy-1.2.2/PKG-INFO` & `rocketpy-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 Metadata-Version: 2.1
 Name: rocketpy
-Version: 1.2.2
+Version: 1.3.0
 Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
-Home-page: https://github.com/RocketPy-Team/RocketPy
-Author: Giovani Hidalgo Ceotto
-Author-email: ghceotto@gmail.com
-Maintainer: RocketPy Developers
+Author-email: Giovani Hidalgo Ceotto <ghceotto@gmail.com>
+Project-URL: homepage, https://rocketpy.org/
+Project-URL: documentation, https://docs.rocketpy.org/
+Project-URL: repository, https://github.com/RocketPy-Team/RocketPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.13
-Requires-Dist: scipy>=1.0
-Requires-Dist: matplotlib>=3.0
-Requires-Dist: netCDF4>=1.6.4
-Requires-Dist: requests
-Requires-Dist: pytz
-Requires-Dist: simplekml
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-coverage; extra == "tests"
+Requires-Dist: black[jupyter]; extra == "tests"
+Requires-Dist: flake8-black; extra == "tests"
+Requires-Dist: flake8-pyproject; extra == "tests"
+Requires-Dist: pandas; extra == "tests"
+Requires-Dist: numericalunits==1.25; extra == "tests"
+Requires-Dist: pylint; extra == "tests"
+Requires-Dist: isort; extra == "tests"
 Provides-Extra: env-analysis
-Requires-Dist: timezonefinder; extra == "env-analysis"
 Requires-Dist: windrose>=1.6.8; extra == "env-analysis"
-Requires-Dist: IPython; extra == "env-analysis"
-Requires-Dist: ipywidgets>=7.6.3; extra == "env-analysis"
+Requires-Dist: timezonefinder; extra == "env-analysis"
 Requires-Dist: jsonpickle; extra == "env-analysis"
+Requires-Dist: ipython; extra == "env-analysis"
+Requires-Dist: ipywidgets>=7.6.3; extra == "env-analysis"
+Provides-Extra: monte-carlo
+Requires-Dist: imageio; extra == "monte-carlo"
 Provides-Extra: all
-Requires-Dist: numpy>=1.13; extra == "all"
-Requires-Dist: scipy>=1.0; extra == "all"
-Requires-Dist: matplotlib>=3.0; extra == "all"
-Requires-Dist: netCDF4>=1.6.4; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: pytz; extra == "all"
-Requires-Dist: simplekml; extra == "all"
-Requires-Dist: timezonefinder; extra == "all"
-Requires-Dist: windrose>=1.6.8; extra == "all"
-Requires-Dist: IPython; extra == "all"
-Requires-Dist: ipywidgets>=7.6.3; extra == "all"
-Requires-Dist: jsonpickle; extra == "all"
+Requires-Dist: rocketpy[env-analysis]; extra == "all"
+Requires-Dist: rocketpy[monte-carlo]; extra == "all"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_white.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_black.png">
   <img alt="RocketPy Logo" src="https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_black.png">
 </picture>
```

### Comparing `rocketpy-1.2.2/README.md` & `rocketpy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rocketpy-1.2.2/rocketpy.egg-info/PKG-INFO` & `rocketpy-1.3.0/rocketpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 Metadata-Version: 2.1
 Name: rocketpy
-Version: 1.2.2
+Version: 1.3.0
 Summary: Advanced 6-DOF trajectory simulation for High-Power Rocketry.
-Home-page: https://github.com/RocketPy-Team/RocketPy
-Author: Giovani Hidalgo Ceotto
-Author-email: ghceotto@gmail.com
-Maintainer: RocketPy Developers
+Author-email: Giovani Hidalgo Ceotto <ghceotto@gmail.com>
+Project-URL: homepage, https://rocketpy.org/
+Project-URL: documentation, https://docs.rocketpy.org/
+Project-URL: repository, https://github.com/RocketPy-Team/RocketPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.13
-Requires-Dist: scipy>=1.0
-Requires-Dist: matplotlib>=3.0
-Requires-Dist: netCDF4>=1.6.4
-Requires-Dist: requests
-Requires-Dist: pytz
-Requires-Dist: simplekml
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-coverage; extra == "tests"
+Requires-Dist: black[jupyter]; extra == "tests"
+Requires-Dist: flake8-black; extra == "tests"
+Requires-Dist: flake8-pyproject; extra == "tests"
+Requires-Dist: pandas; extra == "tests"
+Requires-Dist: numericalunits==1.25; extra == "tests"
+Requires-Dist: pylint; extra == "tests"
+Requires-Dist: isort; extra == "tests"
 Provides-Extra: env-analysis
-Requires-Dist: timezonefinder; extra == "env-analysis"
 Requires-Dist: windrose>=1.6.8; extra == "env-analysis"
-Requires-Dist: IPython; extra == "env-analysis"
-Requires-Dist: ipywidgets>=7.6.3; extra == "env-analysis"
+Requires-Dist: timezonefinder; extra == "env-analysis"
 Requires-Dist: jsonpickle; extra == "env-analysis"
+Requires-Dist: ipython; extra == "env-analysis"
+Requires-Dist: ipywidgets>=7.6.3; extra == "env-analysis"
+Provides-Extra: monte-carlo
+Requires-Dist: imageio; extra == "monte-carlo"
 Provides-Extra: all
-Requires-Dist: numpy>=1.13; extra == "all"
-Requires-Dist: scipy>=1.0; extra == "all"
-Requires-Dist: matplotlib>=3.0; extra == "all"
-Requires-Dist: netCDF4>=1.6.4; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: pytz; extra == "all"
-Requires-Dist: simplekml; extra == "all"
-Requires-Dist: timezonefinder; extra == "all"
-Requires-Dist: windrose>=1.6.8; extra == "all"
-Requires-Dist: IPython; extra == "all"
-Requires-Dist: ipywidgets>=7.6.3; extra == "all"
-Requires-Dist: jsonpickle; extra == "all"
+Requires-Dist: rocketpy[env-analysis]; extra == "all"
+Requires-Dist: rocketpy[monte-carlo]; extra == "all"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_white.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_black.png">
   <img alt="RocketPy Logo" src="https://raw.githubusercontent.com/RocketPy-Team/RocketPy/master/docs/static/RocketPy_Logo_black.png">
 </picture>
```

