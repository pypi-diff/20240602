# Comparing `tmp/mplib-0.2.0a0.tar.gz` & `tmp/mplib-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mplib-0.2.0a0.tar", last modified: Tue Apr 16 21:44:44 2024, max compression
+gzip compressed data, was "mplib-0.2.0a1.tar", last modified: Sun Jun  2 00:57:38 2024, max compression
```

## Comparing `mplib-0.2.0a0.tar` & `mplib-0.2.0a1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.789672 mplib-0.2.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-16 21:44:38.000000 mplib-0.2.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-16 21:44:44.789672 mplib-0.2.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-16 21:44:38.000000 mplib-0.2.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.781672 mplib-0.2.0a0/mplib/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.781672 mplib-0.2.0a0/mplib/collision_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/collision_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/collision_detection/fcl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/collision_avoidance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/constrained_planning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/demo_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/detect_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/moving_robot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/examples/two_stage_motion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/kinematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/kinematics/kdl.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/kinematics/pinocchio.py
--rw-r--r--   0 runner    (1001) docker     (127)    32747 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/planning/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/planning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/planning/ompl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/pymp/
--rw-r--r--   0 runner    (1001) docker     (127)    34009 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/pymp/collision_detection/
--rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/collision_detection/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    35215 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/collision_detection/fcl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/pymp/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/kinematics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/kinematics/kdl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/kinematics/pinocchio.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/pymp/planning/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/planning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/pymp/planning/ompl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.785672 mplib-0.2.0a0/mplib/sapien_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/sapien_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18431 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/sapien_utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/sapien_utils/srdf_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/sapien_utils/urdf_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-16 21:44:38.000000 mplib-0.2.0a0/mplib/urdf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.789672 mplib-0.2.0a0/mplib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-16 21:44:44.000000 mplib-0.2.0a0/mplib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-16 21:44:44.000000 mplib-0.2.0a0/mplib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:44:44.000000 mplib-0.2.0a0/mplib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:44:44.000000 mplib-0.2.0a0/mplib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-16 21:44:44.000000 mplib-0.2.0a0/mplib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 21:44:44.000000 mplib-0.2.0a0/mplib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-16 21:44:38.000000 mplib-0.2.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:44:44.789672 mplib-0.2.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-16 21:44:38.000000 mplib-0.2.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:44:44.789672 mplib-0.2.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-16 21:44:38.000000 mplib-0.2.0a0/tests/test_articulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-16 21:44:38.000000 mplib-0.2.0a0/tests/test_fcl_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-16 21:44:38.000000 mplib-0.2.0a0/tests/test_pinocchio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-04-16 21:44:38.000000 mplib-0.2.0a0/tests/test_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.996835 mplib-0.2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-06-02 00:57:31.000000 mplib-0.2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-06-02 00:57:37.996835 mplib-0.2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-06-02 00:57:31.000000 mplib-0.2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.988834 mplib-0.2.0a1/mplib/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/collision_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/collision_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/collision_detection/fcl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/collision_avoidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/constrained_planning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/demo_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/detect_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/moving_robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/examples/two_stage_motion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/kinematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/kinematics/kdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/kinematics/pinocchio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32747 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/planning/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/planning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/planning/ompl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/pymp/
+-rw-r--r--   0 runner    (1001) docker     (127)    34009 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/pymp/collision_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/collision_detection/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35215 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/collision_detection/fcl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/pymp/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/kinematics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/kinematics/kdl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/kinematics/pinocchio.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.992834 mplib-0.2.0a1/mplib/pymp/planning/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/planning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/pymp/planning/ompl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.996835 mplib-0.2.0a1/mplib/sapien_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/sapien_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18431 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/sapien_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/sapien_utils/srdf_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/sapien_utils/urdf_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-06-02 00:57:32.000000 mplib-0.2.0a1/mplib/urdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.996835 mplib-0.2.0a1/mplib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-06-02 00:57:37.000000 mplib-0.2.0a1/mplib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-02 00:57:37.000000 mplib-0.2.0a1/mplib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:57:37.000000 mplib-0.2.0a1/mplib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:57:37.000000 mplib-0.2.0a1/mplib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 00:57:37.000000 mplib-0.2.0a1/mplib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 00:57:37.000000 mplib-0.2.0a1/mplib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-06-02 00:57:32.000000 mplib-0.2.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:57:37.996835 mplib-0.2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-06-02 00:57:32.000000 mplib-0.2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:57:37.996835 mplib-0.2.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-06-02 00:57:32.000000 mplib-0.2.0a1/tests/test_articulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-06-02 00:57:32.000000 mplib-0.2.0a1/tests/test_fcl_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-06-02 00:57:32.000000 mplib-0.2.0a1/tests/test_pinocchio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-06-02 00:57:32.000000 mplib-0.2.0a1/tests/test_planner.py
```

### Comparing `mplib-0.2.0a0/LICENSE` & `mplib-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/PKG-INFO` & `mplib-0.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplib
-Version: 0.2.0a0
+Version: 0.2.0a1
 Summary: A lightweight motion planning library
 Author-email: Minghua Liu <minghua@ucsd.edu>, Jiayuan Gu <jigu@ucsd.edu>, Kolin Guo <ruguo@ucsd.edu>, Xinsong Lin <x8lin@ucsd.edu>
 Maintainer-email: Kolin Guo <ruguo@ucsd.edu>, Xinsong Lin <x8lin@ucsd.edu>
 License: MIT License
         
         Copyright (c) 2021 Hao Su's Lab, UCSD
```

### Comparing `mplib-0.2.0a0/README.md` & `mplib-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/examples/collision_avoidance.py` & `mplib-0.2.0a1/mplib/examples/collision_avoidance.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/examples/constrained_planning.py` & `mplib-0.2.0a1/mplib/examples/constrained_planning.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/examples/demo.py` & `mplib-0.2.0a1/mplib/examples/demo.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/examples/demo_setup.py` & `mplib-0.2.0a1/mplib/examples/demo_setup.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/examples/detect_collision.py` & `mplib-0.2.0a1/mplib/examples/detect_collision.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/examples/moving_robot.py` & `mplib-0.2.0a1/mplib/examples/moving_robot.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/examples/two_stage_motion.py` & `mplib-0.2.0a1/mplib/examples/two_stage_motion.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/planner.py` & `mplib-0.2.0a1/mplib/planner.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/pymp/__init__.pyi` & `mplib-0.2.0a1/mplib/pymp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/pymp/collision_detection/__init__.pyi` & `mplib-0.2.0a1/mplib/pymp/collision_detection/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/pymp/collision_detection/fcl.pyi` & `mplib-0.2.0a1/mplib/pymp/collision_detection/fcl.pyi`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/pymp/kinematics/kdl.pyi` & `mplib-0.2.0a1/mplib/pymp/kinematics/kdl.pyi`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/pymp/kinematics/pinocchio.pyi` & `mplib-0.2.0a1/mplib/pymp/kinematics/pinocchio.pyi`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/pymp/planning/ompl.pyi` & `mplib-0.2.0a1/mplib/pymp/planning/ompl.pyi`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/sapien_utils/conversion.py` & `mplib-0.2.0a1/mplib/sapien_utils/conversion.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/sapien_utils/srdf_exporter.py` & `mplib-0.2.0a1/mplib/sapien_utils/srdf_exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,29 +63,29 @@
         for j in range(i):
             link2 = colliding_links[j]
             if link2 is parent_link:  # already checked for adjacent links
                 continue
 
             shapes1 = link1.collision_shapes
             shapes2 = link2.collision_shapes
-            # TODO: multiple collision shapes
-            assert len(shapes1) == 1, (
-                f"Should only have 1 collision shape, got {len(shapes1)} shapes for "
-                f"entity '{link1.entity.name}'"
-            )
-            assert len(shapes2) == 1, (
-                f"Should only have 1 collision shape, got {len(shapes2)} shapes for "
-                f"entity '{link2.entity.name}'"
-            )
-            shape1 = shapes1[0]
-            shape2 = shapes2[0]
 
-            if not check_collision_group(
-                shape1.collision_groups, shape2.collision_groups
-            ):
+            enabled_collisions = {
+                check_collision_group(shape1.collision_groups, shape2.collision_groups)
+                for shape1 in shapes1
+                for shape2 in shapes2
+            }
+            if len(enabled_collisions) > 1:
+                raise RuntimeError(
+                    "collision_groups of all collision_shapes must be the same for any"
+                    " link, found violating links: "
+                    f"{link1.name}(id={link1.entity.per_scene_id}) "
+                    f"{link2.name}(id={link2.entity.per_scene_id})"
+                )
+
+            if not enabled_collisions.pop():
                 ET.SubElement(
                     elem_robot,
                     "disable_collisions",
                     {"link1": link1.name, "link2": link2.name, "reason": "Default"},
                 )
 
     return elem_robot
```

### Comparing `mplib-0.2.0a0/mplib/sapien_utils/urdf_exporter.py` & `mplib-0.2.0a1/mplib/sapien_utils/urdf_exporter.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib/urdf_utils.py` & `mplib-0.2.0a1/mplib/urdf_utils.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/mplib.egg-info/PKG-INFO` & `mplib-0.2.0a1/mplib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplib
-Version: 0.2.0a0
+Version: 0.2.0a1
 Summary: A lightweight motion planning library
 Author-email: Minghua Liu <minghua@ucsd.edu>, Jiayuan Gu <jigu@ucsd.edu>, Kolin Guo <ruguo@ucsd.edu>, Xinsong Lin <x8lin@ucsd.edu>
 Maintainer-email: Kolin Guo <ruguo@ucsd.edu>, Xinsong Lin <x8lin@ucsd.edu>
 License: MIT License
         
         Copyright (c) 2021 Hao Su's Lab, UCSD
```

### Comparing `mplib-0.2.0a0/mplib.egg-info/SOURCES.txt` & `mplib-0.2.0a1/mplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/pyproject.toml` & `mplib-0.2.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/setup.py` & `mplib-0.2.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/tests/test_articulation.py` & `mplib-0.2.0a1/tests/test_articulation.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/tests/test_fcl_model.py` & `mplib-0.2.0a1/tests/test_fcl_model.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/tests/test_pinocchio.py` & `mplib-0.2.0a1/tests/test_pinocchio.py`

 * *Files identical despite different names*

### Comparing `mplib-0.2.0a0/tests/test_planner.py` & `mplib-0.2.0a1/tests/test_planner.py`

 * *Files identical despite different names*

