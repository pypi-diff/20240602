# Comparing `tmp/rocketflightsim-0.1.2.tar.gz` & `tmp/rocketflightsim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketflightsim-0.1.2.tar", last modified: Fri May 31 00:00:55 2024, max compression
+gzip compressed data, was "rocketflightsim-0.1.3.tar", last modified: Sun Jun  2 04:46:43 2024, max compression
```

## Comparing `rocketflightsim-0.1.2.tar` & `rocketflightsim-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.857237 rocketflightsim-0.1.2/
--rw-rw-rw-   0        0        0     1095 2024-05-25 02:16:59.000000 rocketflightsim-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1125 2024-05-31 00:00:55.857237 rocketflightsim-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      603 2024-05-29 23:05:15.000000 rocketflightsim-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.803643 rocketflightsim-0.1.2/examples/
--rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.2/examples/__init__.py
--rw-rw-rw-   0        0        0     7941 2024-05-29 22:14:56.000000 rocketflightsim-0.1.2/examples/example_configurations.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.814836 rocketflightsim-0.1.2/rocketflightsim/
--rw-rw-rw-   0        0        0      206 2024-05-30 23:51:47.000000 rocketflightsim-0.1.2/rocketflightsim/__init__.py
--rw-rw-rw-   0        0        0     1481 2024-05-29 23:00:29.000000 rocketflightsim-0.1.2/rocketflightsim/constants.py
--rw-rw-rw-   0        0        0    14283 2024-05-30 23:33:13.000000 rocketflightsim-0.1.2/rocketflightsim/flight_simulation.py
--rw-rw-rw-   0        0        0     8603 2024-05-26 22:52:51.000000 rocketflightsim-0.1.2/rocketflightsim/helper_functions.py
--rw-rw-rw-   0        0        0     9809 2024-05-30 23:59:37.000000 rocketflightsim-0.1.2/rocketflightsim/rocket_classes.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.847288 rocketflightsim-0.1.2/rocketflightsim.egg-info/
--rw-rw-rw-   0        0        0     1125 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-05-31 00:00:55.000000 rocketflightsim-0.1.2/rocketflightsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 00:00:55.858233 rocketflightsim-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      778 2024-05-30 23:53:30.000000 rocketflightsim-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:00:55.854247 rocketflightsim-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0    30808 2024-05-30 23:20:30.000000 rocketflightsim-0.1.2/tests/test_configs.py
--rw-rw-rw-   0        0        0     4273 2024-05-30 23:52:43.000000 rocketflightsim-0.1.2/tests/test_flight_simulation.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:46:43.655986 rocketflightsim-0.1.3/
+-rw-rw-rw-   0        0        0     1095 2024-05-25 02:16:59.000000 rocketflightsim-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1198 2024-06-02 04:46:43.652996 rocketflightsim-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      604 2024-05-31 05:43:49.000000 rocketflightsim-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 04:46:43.590761 rocketflightsim-0.1.3/rocketflightsim/
+-rw-rw-rw-   0        0        0        0 2024-06-02 03:31:08.000000 rocketflightsim-0.1.3/rocketflightsim/__init__.py
+-rw-rw-rw-   0        0        0     1481 2024-05-29 23:00:29.000000 rocketflightsim-0.1.3/rocketflightsim/constants.py
+-rw-rw-rw-   0        0        0    18399 2024-06-02 04:09:52.000000 rocketflightsim-0.1.3/rocketflightsim/flight_simulation.py
+-rw-rw-rw-   0        0        0     8603 2024-05-26 22:52:51.000000 rocketflightsim-0.1.3/rocketflightsim/helper_functions.py
+-rw-rw-rw-   0        0        0    12784 2024-06-02 03:12:05.000000 rocketflightsim-0.1.3/rocketflightsim/rocket_classes.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:46:43.642025 rocketflightsim-0.1.3/rocketflightsim/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-31 02:02:24.000000 rocketflightsim-0.1.3/rocketflightsim/tools/__init__.py
+-rw-rw-rw-   0        0        0     3991 2024-05-29 20:56:31.000000 rocketflightsim-0.1.3/rocketflightsim/tools/fin_flutter.py
+-rw-rw-rw-   0        0        0     2033 2024-05-26 22:52:51.000000 rocketflightsim-0.1.3/rocketflightsim/tools/max_theoretical_g_v.py
+-rw-rw-rw-   0        0        0    14955 2024-06-02 03:24:21.000000 rocketflightsim-0.1.3/rocketflightsim/tools/plotting_functions.py
+-rw-rw-rw-   0        0        0     1217 2024-05-30 23:55:59.000000 rocketflightsim-0.1.3/rocketflightsim/tools/sensitivity_analyses_comparison.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:46:43.651002 rocketflightsim-0.1.3/rocketflightsim.egg-info/
+-rw-rw-rw-   0        0        0     1198 2024-06-02 04:46:43.000000 rocketflightsim-0.1.3/rocketflightsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2024-06-02 04:46:43.000000 rocketflightsim-0.1.3/rocketflightsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 04:46:43.000000 rocketflightsim-0.1.3/rocketflightsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-06-02 04:46:43.000000 rocketflightsim-0.1.3/rocketflightsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 04:46:43.000000 rocketflightsim-0.1.3/rocketflightsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 04:46:43.655986 rocketflightsim-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      826 2024-06-02 04:43:57.000000 rocketflightsim-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:46:43.646013 rocketflightsim-0.1.3/tests/
+-rw-rw-rw-   0        0        0    30808 2024-05-30 23:20:30.000000 rocketflightsim-0.1.3/tests/test_configs.py
+-rw-rw-rw-   0        0        0     4384 2024-06-02 04:29:05.000000 rocketflightsim-0.1.3/tests/test_flight_simulation.py
```

### Comparing `rocketflightsim-0.1.2/LICENSE` & `rocketflightsim-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.2/PKG-INFO` & `rocketflightsim-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: rocketflightsim
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight rocket flight simulator.
 Home-page: https://github.com/werocketry/RocketFlightSim
 Author: Giorgio Chassikos, Western Engineering Rocketry Team
 Author-email: werocketry@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
 
 # RocketFlightSim
 
 RocketFlightSim (RFS) is a light-weight flight simulator for experimental rockets. It is designed to be simple to use, understand, and modify, with the goal of providing a platform for students and hobbyists to learn about rocket flight dynamics.
 
-The simulator currently supports simulation of single-stage rockets in the troposphere, from takeoff to apogee. Simple airbrakes can added to the rocket to induce drag. 
+The simulator currently supports simulation of single-stage rockets in the troposphere, from ignition to apogee. Simple airbrakes can added to the rocket to induce drag. 
 
 A large emphasis is placed on computational efficiency, with the goal of being lightweight enough to run real-time during flight on an onboard microcontroller.
```

### Comparing `rocketflightsim-0.1.2/README.md` & `rocketflightsim-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 # RocketFlightSim
 
 RocketFlightSim (RFS) is a light-weight flight simulator for experimental rockets. It is designed to be simple to use, understand, and modify, with the goal of providing a platform for students and hobbyists to learn about rocket flight dynamics.
 
-The simulator currently supports simulation of single-stage rockets in the troposphere, from takeoff to apogee. Simple airbrakes can added to the rocket to induce drag. 
+The simulator currently supports simulation of single-stage rockets in the troposphere, from ignition to apogee. Simple airbrakes can added to the rocket to induce drag. 
 
 A large emphasis is placed on computational efficiency, with the goal of being lightweight enough to run real-time during flight on an onboard microcontroller.
```

### Comparing `rocketflightsim-0.1.2/rocketflightsim/constants.py` & `rocketflightsim-0.1.3/rocketflightsim/constants.py`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.2/rocketflightsim/flight_simulation.py` & `rocketflightsim-0.1.3/rocketflightsim/flight_simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 import pandas as pd
 import numpy as np
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'examples')))
 from . import helper_functions as hfunc
 from . import constants as con
 
+# TODO: see if Numba can speed up the simulation https://numba.pydata.org/
+
 # Default timestep for the simulation
 default_timestep = 0.02
 """ Notes on timesteps:
 
 The default for OpenRocket sims is 0.01s for the first while, and then somewhere between 0.02 and 0.05 for a while, and then 0.05 for most of the rest of the ascent. It simulates more complicated dynamics than we do
 
 A timestep of 0.02s gives apogees a difference of a few feet for a 10k launch compared to using 0.001s. 0.001s can still be used for one-off sims, but when running many sims, 0.02s is better.
 """
 
 # TODO consider splitting simulator into stages. Could be better for readability, but also for allowing more complex simulations with multiple stages, and going beyond the troposphere with different lapse rates, a different gravity model, and a different wind model. Could even use it for educational purposes like showing the importance of having a launch rail
-# Flight simulation function
+# Flight simulation
 def simulate_flight(rocket, launch_conditions, timestep=default_timestep):
     """
     Simulate the flight of a rocket until its apogee given its specifications and launch conditions.
 
     Args:
     - rocket (Rocket): An instance of the Rocket class.
     - launch_conditions (LaunchConditions): An instance of the LaunchConditions class.
@@ -276,16 +278,16 @@
         liftoff_index,
         launch_rail_cleared_index,
         burnout_index,
         apogee_index
     )
 
 
-# Flight with airbrakes simulation function
-def simulate_airbrakes_flight(pre_brake_flight, rocket, launch_conditions, airbrakes, timestep = default_timestep):
+# Flight simulation with airbrakes - max deployment
+def simulate_airbrakes_flight_max_deployment(pre_brake_flight, rocket, launch_conditions, airbrakes, timestep = default_timestep):
     """
     Simulate the flight of a rocket during its post-burnout ascent with airbrakes deployed until apogee, given its specifications and environmental conditions.
 
     Args:
     - pre_brake_flight (DataFrame): A DataFrame containing the simulation results from the rocket's ascent until burnout. # TODO: maybe change to a tuple of the dataset at the time to start the simulation?
     - rocket (Rocket): An instance of the Rocket class.
     - launch_conditions (LaunchConditions): An instance of the LaunchConditions class.
@@ -390,7 +392,114 @@
             "angle_to_vertical",
             "deployment_angle",
         ],
     )
 
     return airbrakes_ascent
 
+# Flight simulation with airbrakes - deployed as a function of height
+def simulate_airbrakes_flight_deployment_function_of_height(initial_state_vector, rocket, launch_conditions, airbrakes, deployment_function, timestep = default_timestep):
+    """
+    Simulate the flight of a rocket during its post-burnout ascent with airbrakes deployed according to a supplied function of height.
+
+    Args:
+    - initial_state_vector (list): A list containing the initial state of the rocket at the start of the airbrakes simulation.
+    - rocket (Rocket): An instance of the Rocket class.
+    - launch_conditions (LaunchConditions): An instance of the LaunchConditions class.
+    - airbrakes (Airbrakes): An instance of the Airbrakes class.
+    - deployment_function (function): A function that takes the height of the rocket as an argument and returns the angle of the airbrakes deployment at that height.
+    - timestep (float, optional): The time increment for the simulation in seconds.
+
+    Returns:
+    - DataFrame: A DataFrame containing the simulation results from the rocket's post-burnout ascent with airbrakes deployed until apogee.
+    """
+    # Extract rocket parameters
+    mass = rocket.dry_mass
+    Cd_A_rocket_fn = rocket.Cd_A_rocket
+
+    # Extract launch condition parameters
+    launchpad_temp = launch_conditions.launchpad_temp
+    launchpad_pressure = launch_conditions.launchpad_pressure
+    
+    T_lapse_rate = launch_conditions.local_T_lapse_rate    
+    F_gravity = launch_conditions.local_gravity
+
+    # Calculate constants to be used in air density function
+    multiplier = launchpad_pressure / (con.R_specific_air * pow(launchpad_temp, - F_gravity / (con.R_specific_air * T_lapse_rate)))
+    exponent = - F_gravity / (con.R_specific_air * T_lapse_rate) - 1
+
+    # Extract airbrakes parameters
+    Cd_brakes = airbrakes.Cd_brakes
+    A_brakes = airbrakes.num_flaps * airbrakes.A_flap
+    A_Cd_brakes = A_brakes * Cd_brakes
+
+    # Initialize simulation variables
+    time = 0
+    height = initial_state_vector[0]
+    v_y = initial_state_vector[5]
+    v_x = v_y * 0.01
+    speed = np.sqrt(v_y**2 + v_x**2)
+    angle_to_vertical = np.arctan(v_x / v_y)
+    deployment_angle = 0
+
+    simulated_values = []
+    while v_y > 0:
+        time += timestep
+
+        temperature = hfunc.temp_at_height(height, launchpad_temp, lapse_rate = T_lapse_rate)
+        air_density = hfunc.air_density_optimized(temperature, multiplier,exponent)
+        Ma = hfunc.mach_number_fn(speed, temperature)
+        Cd_A_rocket = Cd_A_rocket_fn(Ma)
+        q = hfunc.calculate_dynamic_pressure(air_density, speed)
+
+        deployment_angle = deployment_function(height)
+
+        F_drag = q * (np.sin(deployment_angle) * A_Cd_brakes + Cd_A_rocket)
+        a_y = -F_drag * np.cos(angle_to_vertical) / mass - F_gravity
+        a_x = -F_drag * np.sin(angle_to_vertical) / mass
+        v_y += a_y * timestep
+        v_x += a_x * timestep
+        speed = np.sqrt(v_y**2 + v_x**2)
+        height += v_y * timestep
+
+        angle_to_vertical = np.arctan(v_x / v_y)
+
+        simulated_values.append(
+            [
+                time,
+                height,
+                speed,
+                a_y,
+                a_x,
+                v_y,
+                v_x,
+                temperature,
+                air_density,
+                q,
+                Ma,
+                angle_to_vertical,
+                deployment_angle,
+            ]
+        )
+
+    # simulated_values[-1][11] = simulated_values[-2][11]
+
+    airbrakes_ascent = pd.DataFrame(
+        simulated_values,
+        columns=[
+            "time",
+            "height",
+            "speed",
+            "a_y",
+            "a_x",
+            "v_y",
+            "v_x",
+            "temperature",
+            "air_density",
+            "q",
+            "Ma",
+            "angle_to_vertical",
+            "deployment_angle",
+        ],
+    )
+    
+    return airbrakes_ascent
```

### Comparing `rocketflightsim-0.1.2/rocketflightsim/helper_functions.py` & `rocketflightsim-0.1.3/rocketflightsim/helper_functions.py`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.2/rocketflightsim/rocket_classes.py` & `rocketflightsim-0.1.3/rocketflightsim/rocket_classes.py`

 * *Files 19% similar despite different names*

```diff
@@ -101,14 +101,43 @@
             def Cd_A_rocket_fn(Ma):
                 return Cd_rocket_at_Ma(Ma) * A_rocket
         else:
             def Cd_A_rocket_fn(Ma): return Cd_rocket_at_Ma * A_rocket
             # TODO: make it actually operate as a constant if it's not a function
         self.Cd_A_rocket = Cd_A_rocket_fn
 
+""" TODO Adding wind to the simulation
+
+For first implementation:
+- wind will only act in directions parallel to the ground
+- wind will have a constant speed and direction for the entire flight
+- wind will only affect the rocket's relative airspeed
+    - lateral forces will not be considered
+- wind will not affect flight from ignition to launch rail clearance
+- at launch rail clearance, the rocket will instantly have the wind's velocity added to its velocity vector (instantly weathercock the rocket, keeping the 0 angle of attack assumption used in the simulator)
+
+
+In the simulation, need to add the wind speed to the rocket's velocity vector and have that relative airspeed vector used to determine the drag force and the rocket's angle of attack (but not the rocket's displacement, which should still be calculated using the rocket's velocity vector).
+
+Use this to get data for Spaceport America for the example configuration: https://www.dropbox.com/sh/swi7jrl14evqmap/AADW6GMVIv87KkOBY1-flsoIa?e=1
+    Note that time is in UTC 
+    Also use it to add to the Prometheus launch conditions in the airbrakes repo
+    Remember that launches can't happen if wind > 20mph, so don't consider data with wind speeds above that when trying to find an average
+
+Is it worth describing the wind as None when not specified and having the simulator run faster by not having to add the wind speed to the velocity vector if it's None? 
+
+Could be added later:    
+Varying wind speed and direction with altitude or time, gusts, etc
+    - varying_wind_speed: list of tuples
+        - Each tuple contains the time (s after ignition) and the wind speed (m/s) at that time. Wind speed is relative to the ground.
+    - varying_wind_direction: list of tuples
+        - Each tuple contains the time (s after ignition) and the direction of the wind (deg). 0 is a headwind, 90 is a crosswind from the right, 180 is a tailwind, 270 is a crosswind from the left.
+    - wind_gusts: list of tuples
+        - Each tuple contains the time (s after ignition) and the wind speed (m/s) at that time. Wind speed is relative to the ground.
+"""
 
 class LaunchConditions:
     """The LaunchConditions class is used to store the properties of the launch conditions. 
 
     Attributes
     ----------
     launchpad_pressure : float
@@ -119,26 +148,32 @@
         Length of the launch rail (m).
     launch_angle : float
         Launch angle from horizontal (deg).
     local_gravity : float
         Acceleration due to gravity at the launch site (m/s^2).
     local_T_lapse_rate : float
         Temperature lapse rate at the launch site (°C/m, K/m).
+    mean_wind_speed : float
+        Mean wind speed relative to the ground (m/s).
+    wind_direction : float
+        Direction of the (mean) wind relative to the launch direction (deg). 0 is a headwind, 90 is a crosswind from the right, 180 is a tailwind, 270 is a crosswind from the left.
     """
 
     def __init__(
         self, 
         launchpad_pressure: float,
         launchpad_temp: float,
         L_launch_rail: float,
         launch_angle: float,
         local_gravity: float = None,
         local_T_lapse_rate: float = con.T_lapse_rate,
         latitude: float = None,
         altitude: float = 0,
+        mean_wind_speed = None,
+        wind_direction = 0,
     ):
         """Initializes the LaunchConditions object. 
         
         Parameters
         ----------
         launchpad_pressure : float
             Pressure at the launchpad (Pa).
@@ -152,14 +187,18 @@
             Acceleration due to gravity at the launch site (m/s^2). Defaults to 9.80665.
         local_T_lapse_rate : float, optional
             Temperature lapse rate at the launch site (°C/m, K/m). Defaults to -0.0065.
         latitude : float, optional
             Latitude of the launch site (deg). Used along with altitude to calculate local gravity if local_gravity is not provided. If neither local_gravity nor latitude are provided, local gravity defaults to 9.80665. Defaults to None.
         altitude : float, optional
             Altitude of the launch site (m ASL). Used along with latitude to calculate local gravity if local_gravity is not provided. Defaults to 0.
+        mean_wind_speed : float, optional
+            Mean wind speed relative to the ground (m/s). Defaults to None.
+        wind_direction : float, optional
+            Direction of the (mean) wind relative to the launch direction (deg). 0 is a headwind, 90 is a crosswind from the right, 180 is a tailwind, 270 is a crosswind from the left. Defaults to 0 (headwind).
         """
         self.launchpad_pressure = launchpad_pressure
         self.launchpad_temp = launchpad_temp + 273.15
         self.L_launch_rail = L_launch_rail
         self.launch_angle = launch_angle
 
         self.local_T_lapse_rate = local_T_lapse_rate
@@ -167,14 +206,16 @@
         if local_gravity:
             self.local_gravity = local_gravity
         elif latitude:
             self.local_gravity = hfunc.get_local_gravity(latitude, altitude)
         else:
             self.local_gravity = con.F_gravity
         
+        self.mean_wind_speed = mean_wind_speed
+        self.wind_direction = wind_direction        
 
 class Airbrakes:
     """
     The Airbrakes class is used to store the properties of the airbrakes.
 
     Attributes
     ----------
```

### Comparing `rocketflightsim-0.1.2/rocketflightsim.egg-info/PKG-INFO` & `rocketflightsim-0.1.3/rocketflightsim.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: rocketflightsim
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight rocket flight simulator.
 Home-page: https://github.com/werocketry/RocketFlightSim
 Author: Giorgio Chassikos, Western Engineering Rocketry Team
 Author-email: werocketry@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
 
 # RocketFlightSim
 
 RocketFlightSim (RFS) is a light-weight flight simulator for experimental rockets. It is designed to be simple to use, understand, and modify, with the goal of providing a platform for students and hobbyists to learn about rocket flight dynamics.
 
-The simulator currently supports simulation of single-stage rockets in the troposphere, from takeoff to apogee. Simple airbrakes can added to the rocket to induce drag. 
+The simulator currently supports simulation of single-stage rockets in the troposphere, from ignition to apogee. Simple airbrakes can added to the rocket to induce drag. 
 
 A large emphasis is placed on computational efficiency, with the goal of being lightweight enough to run real-time during flight on an onboard microcontroller.
```

### Comparing `rocketflightsim-0.1.2/tests/test_configs.py` & `rocketflightsim-0.1.3/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.2/tests/test_flight_simulation.py` & `rocketflightsim-0.1.3/tests/test_flight_simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 import unittest
 
 from rocketflightsim.rocket_classes import Motor, Rocket, LaunchConditions
-from rocketflightsim.flight_simulation import simulate_flight, simulate_airbrakes_flight
+from rocketflightsim.flight_simulation import simulate_flight, simulate_airbrakes_flight_max_deployment
 
 from .test_configs import past_flights
 from .test_configs import Juno3_rocket, Juno3_launch_conditions
 
 from example_configurations import default_airbrakes_model
 
 class TestFlightSimulation(unittest.TestCase):
@@ -27,46 +27,48 @@
 
                 assert proportional_difference < 0.1
             print("\n--------------------")
 
 class TestDefaultTimestep(unittest.TestCase):
      def test_default_timestep(self):
             print("Testing default timestep")
+            
             # TODO test to verify slight changes from the default timestep don't have a significant effect on the simulation results
 # from flight simulation file, used to pick the default timestep:
 
 # run a couple hundred different timesteps in logspace between 0.001 and 0.1 to see how it changes to help pick a good timestep
 """apogees = []
 for timestep in np.logspace(-3, -1, 200):
     dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket=Juno3_rocket, timestep=timestep)
-    ascent, time_of_max_deployment = simulate_airbrakes_flight(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, timestep=0.001)
+    ascent, time_of_max_deployment = simulate_airbrakes_flight_max_deployment(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, timestep=0.001)
     apogees.append(ascent["height"].iloc[-1]*3.28084)
     print(len(apogees))
 # plot them
 import matplotlib.pyplot as plt
 plt.plot(np.logspace(-3, -1, 200), apogees)
 plt.xscale("log")
 plt.xlabel("Timestep (s)")
 plt.ylabel("Apogee (ft)")
 plt.title("Apogee vs Timestep")
 plt.show()"""
 
 # add a test to verify that the simulation doesn't take too long to run
 
-class TestAirbrakesFlightSimulation(unittest.TestCase):
-     def test_airbrakes_flight_simulation(self):
+class TestAirbrakesFlightSimulationMaxDeployment(unittest.TestCase):
+     def test_airbrakes_flight_max_deployment_simulation(self):
             print("\n--------------------")
             print("Testing airbrakes flight simulation")
             
             dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, timestep=0.001)
             print(f"Burnout: \n\tHeight: {dataset['height'].iloc[burnout_index - 1]} m\n\tSpeed: {dataset['speed'].iloc[burnout_index - 1]} m/s\n\tTime: {dataset['time'].iloc[burnout_index - 1]} s\n")
             print(f"No-airbraking apogee: \n\tHeight: {dataset['height'].iloc[apogee_index - 1]} m\n\tTime: {dataset['time'].iloc[apogee_index - 1]} s\n")
-            # TODO: make it take the actual flight data at burnout and sim from there
-            ascent = simulate_airbrakes_flight(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, airbrakes=default_airbrakes_model, timestep=0.001)
-            print(f"Airbrakes apogee: \n\tHeight: {ascent['height'].iloc[-1]} m\n\tTime: {ascent['time'].iloc[-1]} s\n\n")
+            # TODO: make it take the actual flight data at burnout and sim from 
+            
+            ascent = simulate_airbrakes_flight_max_deployment(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, airbrakes=default_airbrakes_model, timestep=0.001)
+            print(f"Max deployment airbrakes apogee: \n\tHeight: {ascent['height'].iloc[-1]} m\n\tTime: {ascent['time'].iloc[-1]} s\n\n")
             print("--------------------")
 
             assert ascent["height"].iloc[-1] > 1000
             assert ascent["height"].iloc[-1] < dataset["height"].iloc[apogee_index - 1]
             assert ascent["time"].iloc[-1] < dataset["time"].iloc[apogee_index - 1]
             # assert ascent["speed"].iloc[-1] < dataset["speed"].iloc[apogee_index - 1] ?
```

