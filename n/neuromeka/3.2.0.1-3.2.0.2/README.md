# Comparing `tmp/neuromeka-3.2.0.1.tar.gz` & `tmp/neuromeka-3.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neuromeka-3.2.0.1.tar", last modified: Fri Apr 19 08:49:13 2024, max compression
+gzip compressed data, was "neuromeka-3.2.0.2.tar", last modified: Sun Jun  2 10:10:00 2024, max compression
```

## Comparing `neuromeka-3.2.0.1.tar` & `neuromeka-3.2.0.2.tar`

### file list

```diff
@@ -1,77 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.207540 neuromeka-3.2.0.1/
--rw-rw-rw-   0        0        0     2500 2024-04-19 08:49:13.205583 neuromeka-3.2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.037712 neuromeka-3.2.0.1/neuromeka/
--rw-rw-rw-   0        0        0      152 2024-04-19 05:41:11.000000 neuromeka-3.2.0.1/neuromeka/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.070900 neuromeka-3.2.0.1/neuromeka/common/
--rw-rw-rw-   0        0        0      181 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/__init__.py
--rw-rw-rw-   0        0        0     6513 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/config.py
--rw-rw-rw-   0        0        0     8426 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/dcp_addr.py
--rw-rw-rw-   0        0        0     6425 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/global_timer.py
--rw-rw-rw-   0        0        0     8441 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/jsmin.py
--rw-rw-rw-   0        0        0     2011 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/limits.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.094324 neuromeka-3.2.0.1/neuromeka/common/property/
--rw-rw-rw-   0        0        0      279 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Application.py
--rw-rw-rw-   0        0        0     1142 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Collision.py
--rw-rw-rw-   0        0        0      122 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Log.py
--rw-rw-rw-   0        0        0      346 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Modbus.py
--rw-rw-rw-   0        0        0     3596 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Motion.py
--rw-rw-rw-   0        0        0       69 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Timer.py
--rw-rw-rw-   0        0        0       46 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/TrackConveyor.py
--rw-rw-rw-   0        0        0      462 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Vision.py
--rw-rw-rw-   0        0        0      189 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/__init__.py
--rw-rw-rw-   0        0        0     1270 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/singleton_meta.py
--rw-rw-rw-   0        0        0     6633 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/utils.py
--rw-rw-rw-   0        0        0    22419 2024-04-11 06:51:20.000000 neuromeka-3.2.0.1/neuromeka/ecat.py
--rw-rw-rw-   0        0        0    14613 2024-04-19 06:35:19.000000 neuromeka-3.2.0.1/neuromeka/eye.py
--rw-rw-rw-   0        0        0    10651 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/indy.py
--rw-rw-rw-   0        0        0    74641 2024-04-12 12:54:16.000000 neuromeka-3.2.0.1/neuromeka/indydcp3.py
--rw-rw-rw-   0        0        0    13503 2024-04-11 06:51:20.000000 neuromeka-3.2.0.1/neuromeka/moby.py
--rw-rw-rw-   0        0        0    43010 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/motor.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.202659 neuromeka-3.2.0.1/neuromeka/proto/
--rw-rw-rw-   0        0        0        0 2024-02-06 00:57:07.000000 neuromeka-3.2.0.1/neuromeka/proto/__init__.py
--rw-rw-rw-   0        0        0    25861 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/common_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/common_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    74073 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/config_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/config_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    22023 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/config_pb2.py
--rw-rw-rw-   0        0        0    72800 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/config_pb2_grpc.py
--rw-rw-rw-   0        0        0   177549 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/control_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/control_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    32755 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/control_pb2.py
--rw-rw-rw-   0        0        0   111431 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/control_pb2_grpc.py
--rw-rw-rw-   0        0        0    40034 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/device_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/device_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    12386 2024-04-12 12:54:33.000000 neuromeka-3.2.0.1/neuromeka/proto/device_pb2.py
--rw-rw-rw-   0        0        0    39962 2024-04-12 12:54:33.000000 neuromeka-3.2.0.1/neuromeka/proto/device_pb2_grpc.py
--rw-rw-rw-   0        0        0    77288 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    19026 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2.py
--rw-rw-rw-   0        0        0    62864 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2_grpc.py
--rw-rw-rw-   0        0        0    21736 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2.py
--rw-rw-rw-   0        0        0     6780 2024-04-19 05:39:52.000000 neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2_grpc.py
--rw-rw-rw-   0        0        0      318 2024-02-06 01:43:37.000000 neuromeka-3.2.0.1/neuromeka/proto/grpc_wrapper.py
--rw-rw-rw-   0        0        0    17034 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/linear_pb2.py
--rw-rw-rw-   0        0        0    10079 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/linear_pb2_grpc.py
--rw-rw-rw-   0        0        0    73955 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    16769 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_pb2.py
--rw-rw-rw-   0        0        0    55494 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_pb2_grpc.py
--rw-rw-rw-   0        0        0    12567 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/plotting_pb2.py
--rw-rw-rw-   0        0        0     2569 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/plotting_pb2_grpc.py
--rw-rw-rw-   0        0        0    45795 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0     4929 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2.py
--rw-rw-rw-   0        0        0    13289 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2_grpc.py
--rw-rw-rw-   0        0        0    87158 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/shared_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/shared_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0     6467 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/teleop_dev_pb2.py
--rw-rw-rw-   0        0        0     4133 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/teleop_dev_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.048449 neuromeka-3.2.0.1/neuromeka.egg-info/
--rw-rw-rw-   0        0        0     2500 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2205 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 08:49:13.207540 neuromeka-3.2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1251 2024-04-19 08:47:40.000000 neuromeka-3.2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:10:00.845064 neuromeka-3.2.0.2/
+-rw-rw-rw-   0        0        0     2607 2024-06-02 10:10:00.842136 neuromeka-3.2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2024-02-03 06:42:52.000000 neuromeka-3.2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 10:10:00.629369 neuromeka-3.2.0.2/neuromeka/
+-rw-rw-rw-   0        0        0      416 2024-06-02 09:32:04.000000 neuromeka-3.2.0.2/neuromeka/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:10:00.663528 neuromeka-3.2.0.2/neuromeka/common/
+-rw-rw-rw-   0        0        0       60 2024-05-31 04:07:20.000000 neuromeka-3.2.0.2/neuromeka/common/__init__.py
+-rw-rw-rw-   0        0        0     8441 2024-02-03 06:42:52.000000 neuromeka-3.2.0.2/neuromeka/common/jsmin.py
+-rw-rw-rw-   0        0        0    11876 2024-06-02 07:44:33.000000 neuromeka-3.2.0.2/neuromeka/common/record_plot.py
+-rw-rw-rw-   0        0        0     6461 2024-05-31 04:09:58.000000 neuromeka-3.2.0.2/neuromeka/common/utils.py
+-rw-rw-rw-   0        0        0    19615 2024-06-02 09:28:52.000000 neuromeka-3.2.0.2/neuromeka/ecat.py
+-rw-rw-rw-   0        0        0     8891 2024-06-02 08:56:24.000000 neuromeka-3.2.0.2/neuromeka/enums.py
+-rw-rw-rw-   0        0        0    14607 2024-06-02 09:32:04.000000 neuromeka-3.2.0.2/neuromeka/eye.py
+-rw-rw-rw-   0        0        0    72933 2024-06-02 09:55:25.000000 neuromeka-3.2.0.2/neuromeka/indydcp3.py
+-rw-rw-rw-   0        0        0    13241 2024-06-02 10:07:46.000000 neuromeka-3.2.0.2/neuromeka/moby.py
+-rw-rw-rw-   0        0        0    43010 2024-02-03 06:42:52.000000 neuromeka-3.2.0.2/neuromeka/motor.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:10:00.838232 neuromeka-3.2.0.2/neuromeka/proto/
+-rw-rw-rw-   0        0        0      648 2024-06-02 10:07:38.000000 neuromeka-3.2.0.2/neuromeka/proto/__init__.py
+-rw-rw-rw-   0        0        0    25861 2024-04-12 12:54:38.000000 neuromeka-3.2.0.2/neuromeka/proto/common_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:38.000000 neuromeka-3.2.0.2/neuromeka/proto/common_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    74073 2024-04-12 12:54:36.000000 neuromeka-3.2.0.2/neuromeka/proto/config_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:36.000000 neuromeka-3.2.0.2/neuromeka/proto/config_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    22023 2024-04-12 12:54:35.000000 neuromeka-3.2.0.2/neuromeka/proto/config_pb2.py
+-rw-rw-rw-   0        0        0    72800 2024-04-12 12:54:35.000000 neuromeka-3.2.0.2/neuromeka/proto/config_pb2_grpc.py
+-rw-rw-rw-   0        0        0   177549 2024-04-12 12:54:35.000000 neuromeka-3.2.0.2/neuromeka/proto/control_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:35.000000 neuromeka-3.2.0.2/neuromeka/proto/control_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    32755 2024-04-12 12:54:34.000000 neuromeka-3.2.0.2/neuromeka/proto/control_pb2.py
+-rw-rw-rw-   0        0        0   111431 2024-04-12 12:54:34.000000 neuromeka-3.2.0.2/neuromeka/proto/control_pb2_grpc.py
+-rw-rw-rw-   0        0        0    40034 2024-04-12 12:54:34.000000 neuromeka-3.2.0.2/neuromeka/proto/device_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:34.000000 neuromeka-3.2.0.2/neuromeka/proto/device_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12386 2024-04-12 12:54:33.000000 neuromeka-3.2.0.2/neuromeka/proto/device_pb2.py
+-rw-rw-rw-   0        0        0    39962 2024-04-12 12:54:33.000000 neuromeka-3.2.0.2/neuromeka/proto/device_pb2_grpc.py
+-rw-rw-rw-   0        0        0    77288 2024-04-12 12:54:41.000000 neuromeka-3.2.0.2/neuromeka/proto/ethercat_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:41.000000 neuromeka-3.2.0.2/neuromeka/proto/ethercat_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    19026 2024-04-12 12:54:40.000000 neuromeka-3.2.0.2/neuromeka/proto/ethercat_pb2.py
+-rw-rw-rw-   0        0        0    62864 2024-04-12 12:54:40.000000 neuromeka-3.2.0.2/neuromeka/proto/ethercat_pb2_grpc.py
+-rw-rw-rw-   0        0        0    21736 2024-02-03 06:42:52.000000 neuromeka-3.2.0.2/neuromeka/proto/eyetask_pb2.py
+-rw-rw-rw-   0        0        0     6780 2024-04-19 05:39:52.000000 neuromeka-3.2.0.2/neuromeka/proto/eyetask_pb2_grpc.py
+-rw-rw-rw-   0        0        0    73955 2024-04-12 12:54:42.000000 neuromeka-3.2.0.2/neuromeka/proto/moby_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:42.000000 neuromeka-3.2.0.2/neuromeka/proto/moby_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    16769 2024-04-12 12:54:41.000000 neuromeka-3.2.0.2/neuromeka/proto/moby_pb2.py
+-rw-rw-rw-   0        0        0    55494 2024-04-12 12:54:41.000000 neuromeka-3.2.0.2/neuromeka/proto/moby_pb2_grpc.py
+-rw-rw-rw-   0        0        0    45795 2024-04-12 12:54:37.000000 neuromeka-3.2.0.2/neuromeka/proto/rtde_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:37.000000 neuromeka-3.2.0.2/neuromeka/proto/rtde_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4929 2024-04-12 12:54:36.000000 neuromeka-3.2.0.2/neuromeka/proto/rtde_pb2.py
+-rw-rw-rw-   0        0        0    13289 2024-04-12 12:54:36.000000 neuromeka-3.2.0.2/neuromeka/proto/rtde_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:10:00.645960 neuromeka-3.2.0.2/neuromeka.egg-info/
+-rw-rw-rw-   0        0        0     2607 2024-06-02 10:10:00.000000 neuromeka-3.2.0.2/neuromeka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1436 2024-06-02 10:10:00.000000 neuromeka-3.2.0.2/neuromeka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:10:00.000000 neuromeka-3.2.0.2/neuromeka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-06-02 10:10:00.000000 neuromeka-3.2.0.2/neuromeka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 10:10:00.000000 neuromeka-3.2.0.2/neuromeka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:10:00.845064 neuromeka-3.2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2024-06-02 10:09:42.000000 neuromeka-3.2.0.2/setup.py
```

### Comparing `neuromeka-3.2.0.1/PKG-INFO` & `neuromeka-3.2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: neuromeka
-Version: 3.2.0.1
-Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
+Version: 3.2.0.2
+Summary: Neuromeka client protocols for IndyDCP3, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients3
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: grpcio==1.39.0
 Requires-Dist: grpcio-tools==1.39.0
 Requires-Dist: protobuf==3.17.3
 Requires-Dist: requests==2.22.0
 Requires-Dist: Pillow==9.5.0
```

### Comparing `neuromeka-3.2.0.1/README.md` & `neuromeka-3.2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/common/jsmin.py` & `neuromeka-3.2.0.2/neuromeka/common/jsmin.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/common/utils.py` & `neuromeka-3.2.0.2/neuromeka/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import socket
 import netifaces
 from dataclasses import dataclass, field
 from .jsmin import jsmin
 
 import grpc
-from . import limits as Limits
+from neuromeka.enums import Limits
 
 
 @dataclass
 class GRPCReturn:
     code: grpc.StatusCode = grpc.StatusCode.OK
     details: str = ''
 
@@ -38,21 +38,14 @@
             print('GRPC Exception Forwarder at ' + str(func.__name__) + ' (' + str(ex.code()) + ' - ' + str(
                 ex.details()) + ')')
             return GRPCReturn(code=ex.code(), details=ex.details())
 
     return wrapper
 
 
-# def get_ip():
-#     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-#     s.connect(("8.8.8.8", 80))
-#     r = s.getsockname()[0]
-#     s.close()
-#     return r
-
 def get_ip():
     ip_addr = ''
     interfaces = netifaces.interfaces()
     for interface in interfaces:
         if interface != 'lo':
             ip = netifaces.ifaddresses(interface)
             if netifaces.AF_INET in ip:
```

### Comparing `neuromeka-3.2.0.1/neuromeka/ecat.py` & `neuromeka-3.2.0.2/neuromeka/ecat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,34 @@
-from .proto.grpc_wrapper import *
-from .common import *
-from .proto.ethercat_pb2_grpc import EtherCATStub
-from .proto.common_msgs_pb2 import *
-from .proto.ethercat_msgs_pb2 import *
+from neuromeka.proto import *
+from neuromeka.common import *
+from neuromeka.enums import *
 
 import grpc
 import time
 
-OP_MODE_NO_MODE = 0x00
-OP_MODE_PROFILE_POSITION = 0x01
-OP_MODE_VELOCITY = 0x02
-OP_MODE_PROFILE_VELOCITY = 0x03
-OP_MODE_TORQUE_PROFILE = 0x04
-OP_MODE_HOMING = 0x06
-OP_MODE_INTERPOLATED_POSITION = 0x07
-OP_MODE_CYCLIC_SYNC_POSITION = 0x08
-OP_MODE_CYCLIC_SYNC_VELOCITY = 0x09
-OP_MODE_CYCLIC_SYNC_TORQUE = 0x0a
-
-def status2string(statusword):
-    if (((statusword) & 0x004f) == 0x0000):   # x0xx 0000
-        return "NOT_READY"
-    elif (((statusword) & 0x004f) == 0x0040): # x1xx 0000
-        return "SWITCH_DISABLED"
-    elif (((statusword) & 0x006f) == 0x0021): # x01x 0001
-        return "READY_SWITCH"
-    elif (((statusword) & 0x006f) == 0x0023): # x01x 0011
-        return "SWITCHED_ON"
-    elif (((statusword) & 0x006f) == 0x0027): # x01x 0111
-        return "OPERATION_ENABLED"
-    elif (((statusword) & 0x006f) == 0x0007): # x00x 0111
-        return "QUICK_STOP"
-    elif (((statusword) & 0x004f) == 0x000f): # x0xx 1111
-        return "FAULT_REACTION"
-    elif (((statusword) & 0x004f) == 0x0008): # x0xx 1000
-        return "FAULT"
-    else:
-        return "UNKNOWN"
-
-
-def modeop2string(modeop):
-    if modeop == 0x00:
-        return "None"
-    elif modeop == 0x01:
-        return "PP"
-    elif modeop == 0x03:
-        return "PV"
-    elif modeop == 0x04:
-        return "TP"
-    elif modeop == 0x06:
-        return "Homing"
-    elif modeop == 0x08:
-        return "CSP"
-    elif modeop == 0x09:
-        return "CSV"
-    elif modeop == 0x0a:
-        return "CST"
-
-
-def error_code(mode_op, status_word):
-    string_out = []
-    if mode_op == OP_MODE_PROFILE_POSITION:
-        if (status_word & 0x2000):
-            string_out.append("Following error")
-        if (status_word & 0x1000):
-            string_out.append("Set-point acknowledge")
-        if (status_word & 0x0400):
-            string_out.append("Target reached")
-
-    elif mode_op == OP_MODE_PROFILE_VELOCITY:
-        if (status_word & 0x2000):
-            string_out.append("Max slippage error")
-        if (status_word & 0x1000):
-            string_out.append("Speed")
-        if (status_word & 0x0400):
-            string_out.append("Target reached")
-
-    elif mode_op == OP_MODE_CYCLIC_SYNC_POSITION:
-        if (status_word & 0x2000):
-            string_out.append("Following error")
-        if (status_word & 0x1000):
-            string_out.append("Drive follows command value")
-
-    elif mode_op == OP_MODE_CYCLIC_SYNC_VELOCITY:
-        if (status_word & 0x1000):
-            string_out.append("Drive follows command value")
-
-    elif mode_op == OP_MODE_CYCLIC_SYNC_TORQUE:
-        if (status_word & 0x1000):
-            string_out.append("Drive follows command value")
-    return string_out
+ETHERCAT_PORT = 20000
 
 
-class EcatClient:
+class EtherCAT:
     def __init__(self, ip_addr):
         # initialize RPC
-        ecat_channel = grpc.insecure_channel("{}:{}".format(ip_addr, 20000))
+        ecat_channel = grpc.insecure_channel("{}:{}".format(ip_addr, ETHERCAT_PORT))
         ecat_stub = EtherCATStub(ecat_channel)
 
         self.__ethercat_stub = ecat_stub
 
     
     ###### EtherCAT Communication Task gRPC protocol
-    @Utils.exception_handler
+    # @Utils.exception_handler
     def get_master_status(self):
         """
         Master status
             status -> int
         """
-        status = self.__ethercat_stub.GetMasterStatus(Empty()).status
+        status = self.__ethercat_stub.GetMasterStatus(common_msgs.Empty()).status
         if status == 1:
             return "INIT"
         elif status == 2:
             return "PRE-OP"
         elif status == 4:
             return "SAFE-OP"
         elif status == 8:
@@ -122,15 +38,15 @@
 
     @Utils.exception_handler
     def get_slave_status(self):
         """
         Slave status
 
         """
-        status = (self.__ethercat_stub.GetSlaveStatus(Empty()).status)
+        status = (self.__ethercat_stub.GetSlaveStatus(common_msgs.Empty()).status)
         slave_status = []
         for stat in status:
             if stat == 1:
                 slave_status.append("INIT")
             elif stat == 2:
                 slave_status.append("PRE-OP")
             elif stat == 4:
@@ -142,130 +58,131 @@
         return slave_status
 
     @Utils.exception_handler
     def get_txdomain_status(self):
         """
         PDO Tx Domain status
         """
-        status = self.__ethercat_stub.GetTxDomainStatus(Empty()).status
+        status = self.__ethercat_stub.GetTxDomainStatus(common_msgs.Empty()).status
         if status == 0:
             return "ZERO"
         elif status == 1:
             return "INCOMPLETE"
         elif status == 2:
             return "COMPLETE"
         else:
             return "None"
 
     @Utils.exception_handler
     def get_rxdomain_status(self):
         """
         PDO Rx Domain status
         """
-        status = self.__ethercat_stub.GetRxDomainStatus(Empty()).status
+        status = self.__ethercat_stub.GetRxDomainStatus(common_msgs.Empty()).status
         if status == 0:
             return "ZERO"
         elif status == 1:
             return "INCOMPLETE"
         elif status == 2:
             return "COMPLETE"
         else:
             return "None"
 
     @Utils.exception_handler
-    def is_system_ready(self):
+    def is_system_ready(self) -> list:
         """
         System ready state
         """
-        return list(self.__ethercat_stub.IsSystemReady(Empty()).ready)
+        return list(self.__ethercat_stub.IsSystemReady(common_msgs.Empty()).ready)
 
     @Utils.exception_handler
-    def is_servo_on(self):
+    def is_servo_on(self) -> list:
         """
         Servo on state
         """
-        return list(self.__ethercat_stub.IsServoOn(Empty()).servo)
+        return list(self.__ethercat_stub.IsServoOn(common_msgs.Empty()).servo)
 
     @Utils.exception_handler
     def get_slave_type_num(self):
         """
         Servo on state
         """
-        return self.__ethercat_stub.GetSlaveTypeNum(Empty())
+        return self.__ethercat_stub.GetSlaveTypeNum(common_msgs.Empty())
 
     @Utils.exception_handler
     def reset_overflow_count(self):
         """
         Reset and save overflow count
         """
-        return self.__ethercat_stub.ResetOverflowCount(Empty())
+        return self.__ethercat_stub.ResetOverflowCount(common_msgs.Empty())
 
     @Utils.exception_handler
     def set_servo(self, servo_idx, on):
         """
         Servo on state
         """
         if on:
-            self.__ethercat_stub.SetServoOn(ServoIndex(servoIndex=servo_idx))
+            self.__ethercat_stub.SetServoOn(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
         else:
-            self.__ethercat_stub.SetServoOff(ServoIndex(servoIndex=servo_idx))
+            self.__ethercat_stub.SetServoOff(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
 
     @Utils.exception_handler
     def get_servo_tx(self, servo_idx):
         """
         Get Servo driver's Tx PDO values
         """
-        res = self.__ethercat_stub.GetServoTx(ServoIndex(servoIndex=servo_idx))
-        return [status2string(res.statusWord), modeop2string(res.modeOpDisp), res.actualPosition, res.actualVelocity, res.actualTorque]
+        res = self.__ethercat_stub.GetServoTx(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
+        return [EtherCATStatus.status2string(res.statusWord),
+                EtherCATStatus.modeop2string(res.modeOpDisp), res.actualPosition, res.actualVelocity, res.actualTorque]
 
     @Utils.exception_handler
     def get_servo_tx_raw(self, servo_idx):
         """
         Get Servo driver's Tx PDO values
         """
-        return self.__ethercat_stub.GetServoTx(ServoIndex(servoIndex=servo_idx))
+        return self.__ethercat_stub.GetServoTx(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
 
     @Utils.exception_handler
     def get_servo_tx_keba(self, servo_idx):
         """
         Get Servo (Keba) driver's Tx PDO values
         """
-        res = self.__ethercat_stub.GetServoTxKeba(ServoIndex(servoIndex=servo_idx))
-        res1 = [status2string(res.statusWord), res.actualPosition, res.actualVelocity]
-        res2 = [status2string(res.statusWord2), res.actualPosition2, res.actualVelocity2]
-        res3 = [status2string(res.statusWord3), res.actualPosition3, res.actualVelocity3]
+        res = self.__ethercat_stub.GetServoTxKeba(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
+        res1 = [EtherCATStatus.status2string(res.statusWord), res.actualPosition, res.actualVelocity]
+        res2 = [EtherCATStatus.status2string(res.statusWord2), res.actualPosition2, res.actualVelocity2]
+        res3 = [EtherCATStatus.status2string(res.statusWord3), res.actualPosition3, res.actualVelocity3]
         return [res1, res2, res3]
 
     @Utils.exception_handler
     def get_servo_rx_keba(self, servo_idx):
         """
         Get Servo (Keba) driver's Rx PDO values
         """
-        res = self.__ethercat_stub.GetServoRxKeba(ServoIndex(servoIndex=servo_idx))
+        res = self.__ethercat_stub.GetServoRxKeba(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
         res1 = [res.controlWord, res.targetPosition, res.targetTorque]
         res2 = [res.controlWord2, res.targetPosition2, res.targetTorque2]
         res3 = [res.controlWord3, res.targetPosition3, res.targetTorque3]
         return [res1, res2, res3]
 
     @Utils.exception_handler
     def get_servo_rx(self, servo_idx):
         """
         Get Servo driver's Rx PDO values
         """
-        res = self.__ethercat_stub.GetServoRx(ServoIndex(servoIndex=servo_idx))
+        res = self.__ethercat_stub.GetServoRx(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
         return [res.controlWord, res.modeOp, res.targetPosition, res.targetVelocity, res.targetTorque]
 
     @Utils.exception_handler
     def set_servo_rx(self, servo_idx, control_word, mode_op, target_pos, target_vel, target_tor):
         """
         Set Servo driver's Rx PDO values
         """
         print(servo_idx, control_word, mode_op, target_pos, target_vel, target_tor)
         servo_rx = ServoRx(controlWord=control_word, modeOp=mode_op, targetPosition=target_pos, targetVelocity=target_vel, targetTorque=target_tor)
-        return self.__ethercat_stub.SetServoRx(ServoRxIndex(servoIndex=servo_idx, rx=servo_rx))
+        return self.__ethercat_stub.SetServoRx(ethercat_msgs.ServoRxIndex(servoIndex=servo_idx, rx=servo_rx))
 
     @Utils.exception_handler
     def set_servo_rx_keba(self, servo_idx, rx1, rx2, rx3):
         """
         Set Servo (Keba) driver's Rx PDO values
         """
         control_word = rx1[0]
@@ -278,43 +195,43 @@
 
         target_tor = rx1[2]
         target_tor2 = rx2[2]
         target_tor3 = rx3[2]
         servo_rx = ServoRxKeba(controlWord=control_word, controlWord2=control_word2, controlWord3=control_word3,
                                targetPosition=target_pos, targetPosition2=target_pos2, targetPosition3=target_pos3,
                                targetTorque=target_tor, targetTorque2=target_tor2, targetTorque3=target_tor3)
-        return self.__ethercat_stub.SetServoRx(ServoRxIndexKeba(servoIndex=servo_idx, rx=servo_rx))
+        return self.__ethercat_stub.SetServoRx(ethercat_msgs.ServoRxIndexKeba(servoIndex=servo_idx, rx=servo_rx))
 
     @Utils.exception_handler
     def get_servo_temperature(self, servo_idx):
         """
         Get Servo SDO temperatures
         """
-        return self.__ethercat_stub.GetServoTemperature(ServoIndex(servoIndex=servo_idx)).temperature
+        return self.__ethercat_stub.GetServoTemperature(ethercat_msgs.ServoIndex(servoIndex=servo_idx)).temperature
 
     @Utils.exception_handler
     def get_servo_errorcode(self, servo_idx):
         """
         Get Servo SDO error code
         """
-        return self.__ethercat_stub.GetServoErrorCode(ServoIndex(servoIndex=servo_idx)).errorCode
+        return self.__ethercat_stub.GetServoErrorCode(ethercat_msgs.ServoIndex(servoIndex=servo_idx)).errorCode
 
     @Utils.exception_handler
     def reset_servo(self, servo_idx):
         """
         Reset servo error
         """
-        return self.__ethercat_stub.ResetServo(ServoIndex(servoIndex=servo_idx))
+        return self.__ethercat_stub.ResetServo(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
 
     @Utils.exception_handler
     def set_brake(self, ecat_idx, onoff):
         """
         Manual brake by SDO
         """
-        return self.__ethercat_stub.SetCOREManualBrake(ServoBrake(ecatIndex=ecat_idx, onoff=onoff))
+        return self.__ethercat_stub.SetCOREManualBrake(ethercat_msgs.ServoBrake(ecatIndex=ecat_idx, onoff=onoff))
 
     @Utils.exception_handler
     def set_endtool_rx(self, endtool_rx):
         """
         Set endtool Rx data
         """
         eqc = endtool_rx["eqc"]
@@ -328,15 +245,15 @@
 
     @Utils.exception_handler
     def get_endtool_rx(self):
         """
         Get endtool Rx data
         """
         endtool_rx = {}
-        data = self.__ethercat_stub.GetEndtoolRx(Empty())
+        data = self.__ethercat_stub.GetEndtoolRx(common_msgs.Empty())
         endtool_rx["eqc"] = data.eqc
         endtool_rx["gripper"] = data.gripper
         endtool_rx["ft_param"] = data.ft_param
         endtool_rx["led_mode"] = data.led_mode
         endtool_rx["led_g"] = data.led_g
         endtool_rx["led_r"] = data.led_r
         endtool_rx["led_b"] = data.led_b
@@ -344,43 +261,43 @@
 
     @Utils.exception_handler
     def get_endtool_tx(self):
         """
         Get endtool Tx data
         """
         endtool_tx = {}
-        data = self.__ethercat_stub.GetEndtoolTx(Empty())
+        data = self.__ethercat_stub.GetEndtoolTx(common_msgs.Empty())
         endtool_tx["status"] = data.status
         endtool_tx["button"] = data.button
         endtool_tx["ft_sensor"] = data.ft_sensor
         endtool_tx["ft_state"] = data.ft_state
         endtool_tx["ft_error"] = data.ft_error
         return endtool_tx
 
     @Utils.exception_handler
     def get_ioboard_tx(self):
         """
         Get ioboard Tx data
         """
         ioboard_tx = {}
-        data = self.__ethercat_stub.GetIOBoardTx(Empty())
+        data = self.__ethercat_stub.GetIOBoardTx(common_msgs.Empty())
         ioboard_tx["di5v"] = data.di5v
         ioboard_tx["di24v1"] = data.di24v1
         ioboard_tx["di24v2"] = data.di24v2
         ioboard_tx["ai1"] = data.ai1
         ioboard_tx["ai2"] = data.ai2
         return ioboard_tx
 
     @Utils.exception_handler
     def get_ioboard_rx(self):
         """
         Get ioboard Rx data
         """
         ioboard_rx = {}
-        data = self.__ethercat_stub.GetIOBoardRx(Empty())
+        data = self.__ethercat_stub.GetIOBoardRx(common_msgs.Empty())
         ioboard_rx["do5v"] = data.do5v
         ioboard_rx["do24v1"] = data.do24v1
         ioboard_rx["do24v2"] = data.do24v2
         ioboard_rx["ao1"] = data.ao1
         ioboard_rx["ao2"] = data.ao2
         ioboard_rx["ft_param"] = data.ft_param
         return ioboard_rx
@@ -401,100 +318,100 @@
 
 
     @Utils.exception_handler
     def get_di(self, dio_index):
         """
         Get DIO Tx data
         """
-        return self.__ethercat_stub.GetDI(DIOIndex(dioIndex=dio_index)).di_list
+        return self.__ethercat_stub.GetDI(ethercat_msgs.DIOIndex(dioIndex=dio_index)).di_list
 
     @Utils.exception_handler
     def get_do(self, dio_index):
         """
         Set ioboard Rx data
         """
-        return self.__ethercat_stub.GetDO(DIOIndex(dioIndex=dio_index)).do_list
+        return self.__ethercat_stub.GetDO(ethercat_msgs.DIOIndex(dioIndex=dio_index)).do_list
 
     @Utils.exception_handler
     def set_do(self, dio_index, dio):
         """
         Set ioboard Rx data
         """
-        return self.__ethercat_stub.SetDO(DIODigitalOutput(dioIndex=dio_index, do_list=dio))
+        return self.__ethercat_stub.SetDO(ethercat_msgs.DIODigitalOutput(dioIndex=dio_index, do_list=dio))
 
 
     @Utils.exception_handler
     def set_maxTorque(self, slave_idx, value):
         """
         Set Maximum Torque [ecat idx, torq]
         """
-        return self.__ethercat_stub.SetMaxTorqueSDO(ServoParam(slaveIdx=slave_idx, val=value))
+        return self.__ethercat_stub.SetMaxTorqueSDO(ethercat_msgs.ServoParam(slaveIdx=slave_idx, val=value))
 
     @Utils.exception_handler
     def set_profileVel(self, slave_idx, value):
         """
         Set Profile Velocity [ecat idx, vel]
         """
-        return self.__ethercat_stub.SetProfileVelSDO(ServoParam(slaveIdx=slave_idx, val=value))
+        return self.__ethercat_stub.SetProfileVelSDO(ethercat_msgs.ServoParam(slaveIdx=slave_idx, val=value))
 
     @Utils.exception_handler
     def set_profileAcc(self, slave_idx, value):
         """
         Set Profile Acceleration [ecat idx, acc]
         """
-        return self.__ethercat_stub.SetProfileAccSDO(ServoParam(slaveIdx=slave_idx, val=value))
+        return self.__ethercat_stub.SetProfileAccSDO(ethercat_msgs.ServoParam(slaveIdx=slave_idx, val=value))
 
     @Utils.exception_handler
     def set_profileDec(self, slave_idx, value):
         """
         Set Profile Deceleration [ecat idx, dec]
         """
-        return self.__ethercat_stub.SetProfileDecSDO(ServoParam(slaveIdx=slave_idx, val=value))
+        return self.__ethercat_stub.SetProfileDecSDO(ethercat_msgs.ServoParam(slaveIdx=slave_idx, val=value))
 
     @Utils.exception_handler
     def get_maxTorque(self, slave_idx):
         """
         Get Maximum Torque [ecat idx]
         """
-        return self.__ethercat_stub.GetMaxTorqueSDO(EcatIndex(ecatIndex=slave_idx)).val
+        return self.__ethercat_stub.GetMaxTorqueSDO(ethercat_msgs.EcatIndex(ecatIndex=slave_idx)).val
 
     @Utils.exception_handler
     def get_profileVel(self, slave_idx):
         """
         Get Profile Velocity [ecat idx]
         """
-        return self.__ethercat_stub.GetProfileVelSDO(EcatIndex(ecatIndex=slave_idx)).val
+        return self.__ethercat_stub.GetProfileVelSDO(ethercat_msgs.EcatIndex(ecatIndex=slave_idx)).val
 
     @Utils.exception_handler
     def get_profileAcc(self, slave_idx):
         """
         Get Profile Acceleration [ecat idx]
         """
-        return self.__ethercat_stub.GetProfileAccSDO(EcatIndex(ecatIndex=slave_idx)).val
+        return self.__ethercat_stub.GetProfileAccSDO(ethercat_msgs.EcatIndex(ecatIndex=slave_idx)).val
 
     @Utils.exception_handler
     def get_profileDec(self, slave_idx):
         """
         Get Profile Deceleration [ecat idx]
         """
-        return self.__ethercat_stub.GetProfileDecSDO(EcatIndex(ecatIndex=slave_idx)).val
+        return self.__ethercat_stub.GetProfileDecSDO(ethercat_msgs.EcatIndex(ecatIndex=slave_idx)).val
 
 
     def get_robot_zero_count(self, servo_idx):
         """
         Get robot zero count
         """
-        return self.__ethercat_stub.GetRobotZeroCount(ServoIndex(servoIndex=servo_idx))
+        return self.__ethercat_stub.GetRobotZeroCount(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
 
     @Utils.exception_handler
     def set_robot_zero_as_current(self, servo_idx):
         """
         Set robot zero as current
         """
-        return self.__ethercat_stub.SetRobotZeroAsCurrent(ServoIndex(servoIndex=servo_idx))
+        return self.__ethercat_stub.SetRobotZeroAsCurrent(ethercat_msgs.ServoIndex(servoIndex=servo_idx))
 
 
     ## Conty Linear Ext Servo
     @Utils.exception_handler
     def get_axis_data(self,servo_idx):
         """
         Axis Data:
@@ -598,16 +515,16 @@
 
     @Utils.exception_handler
     def move_axis(self,
                   servo_idx,
                   start_mm,
                   target_mm,
                   is_absolute=True,
-                  vel_ratio=Limits.JogVelRatioDefault,
-                  acc_ratio=Limits.JogAccRatioDefault,
+                  vel_ratio=50,
+                  acc_ratio=100,
                   teaching_mode=True):
         """
         start_mm = [mm, mm, mm] -> pos
         target_mm = [mm, mm, mm] -> pos
         vel_mm : int -> vel_ratio
         acc_mm : int -> acc_ratio
         is_absolute : True if target is absolute -> base_type
@@ -649,25 +566,7 @@
         return linear_target
 
 
     @Utils.exception_handler
     def stop_motion(self, servo_idx):
         print("StopMotion Frome Ethercat_client")
         self.set_servo_rx(servo_idx, 15, 10, 0, 0, 0)
-        pass
-
-############################
-# Main
-############################
-if __name__ == "__main__":
-    ip = '192.168.0.91'
-    ecat = EcatClient(ip)
-    print("Master status: ", ecat.get_master_status())
-    print("Slave status: ", ecat.get_slave_status())
-    print("TxPDO domain: ", ecat.get_txdomain_status())
-    print("RxPDO domain: ", ecat.get_rxdomain_status())
-    print("System ready: ", ecat.is_system_ready())
-    print("Servo state: ", ecat.is_servo_on())
-    print("")
-    print(ecat.get_slave_type_num())
-
-    time.sleep(1)
```

### Comparing `neuromeka-3.2.0.1/neuromeka/eye.py` & `neuromeka-3.2.0.2/neuromeka/eye.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     ERROR_STATE = 'error_state'
     ERROR_MODULE = 'error_module'
     CLASS_NAMES = 'class_names'
 
 ##
 # @class IndyEyeClient
 # @brief Rest API client
-class IndyEyeClient:
+class IndyEye:
     def __init__(self, eye_ip):
         self.session = requests.session()
         self.eye_ip = eye_ip
         self.url = f"http://{eye_ip}:8088"
         self.version = self.get_version()
         if float(".".join(self.version.split(".")[:2])) >= 0.5:
             # initialize gRPC
```

### Comparing `neuromeka-3.2.0.1/neuromeka/indydcp3.py` & `neuromeka-3.2.0.2/neuromeka/indydcp3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,92 +1,37 @@
-from .proto.grpc_wrapper import *
-from .proto.control_pb2_grpc import ControlStub
-from .proto.device_pb2_grpc import DeviceStub
-from .proto.config_pb2_grpc import ConfigStub
-from .proto.rtde_pb2_grpc import RTDataExchangeStub
-
-from .proto import common_msgs_pb2 as common_msgs
-from .proto import control_msgs_pb2 as control_msgs
-from .proto import config_msgs_pb2 as config_msgs
-from .proto import device_msgs_pb2 as device_msgs
-from .proto import rtde_msgs_pb2 as rtde_msgs
+from neuromeka.proto import *
+from neuromeka.common import *
+from neuromeka.enums import *
 
-from .common import *
 
-from operator import add
-import json
 import grpc
 from google.protobuf import json_format
 from google.protobuf.json_format import ParseDict
-import math
-import time
 
 CONTROL_SOCKET_PORT = [20001, 30001]
 DEVICE_SOCKET_PORT = [20002, 30002]
 CONFIG_SOCKET_PORT = [20003, 30003]
 RTDE_SOCKET_PORT = [20004, 30004]
 
 
-def grpc_mapping_call(control_stub, func_name, arg_dict=None):
-    if arg_dict is None:
-        arg_dict = {}
-    grpc_request = getattr(control_msgs, "{}Req".format(func_name))()
-    ParseDict(arg_dict, grpc_request)
-    try:
-        grpc_response = getattr(control_stub, func_name)(grpc_request)
-
-    except grpc.RpcError as rpc_error:
-        print('Robot gRPC: ' + func_name + ': Connection unavailable')
-        grpc_response = None
-
-    except Exception as ex:
-        print(func_name + 'Robot gRPC Exception: ' + str(ex))
-        grpc_response = None
-
-    return grpc_response
-
 class IndyDCP3:
-    ABSOLUTE_JOINT = control_msgs.ABSOLUTE_JOINT
-    RELATIVE_JOINT = control_msgs.RELATIVE_JOINT
-    ABSOLUTE_TASK = control_msgs.ABSOLUTE_TASK
-    RELATIVE_TASK = control_msgs.RELATIVE_TASK
-    TCP_TASK = control_msgs.TCP_TASK
-    CIRCLE_POINT_SET = control_msgs.POINT_SET
-    CIRCLE_CENTER_AXIS = control_msgs.CENTER_AXIS
-    CIRCLE_CONSTANT = control_msgs.CONSTANT
-    CIRCLE_RADIAL = control_msgs.RADIAL
-    CIRCLE_SMOOTH = control_msgs.SMOOTH
-    STOP_IMMEDIATE_BRAKE = 0
-    STOP_SMOOTH_BRAKE = 1
-    STOP_SMOOTH_ONLY = 2
-    NO_BLENDING = 0
-    OVERRIDE_BLENDING = 1
-    DUPLICATE_BLENDING = 2
-
-    COLLISION_NO_DETECT = common_msgs.COLL_NO_DETECT
-    COLLISION_PAUSE = common_msgs.COLL_PAUSE
-    COLLISION_RESUME_AFTER_SLEEP = common_msgs.COLL_RESUME_AFTER_SLEEP
-    COLLISION_STOP = common_msgs.COLL_STOP
-    STOPCAT_IMMEDIATE_BRAKE = common_msgs.IMMEDIATE_BRAKE
-    STOPCAT_SMOOTH_BRAKE = common_msgs.SMOOTH_BRAKE
-    STOPCAT_SMOOTH_ONLY = common_msgs.SMOOTH_ONLY
-
     def __init__(self, robot_ip='127.0.0.1', index=0):
+        if index not in [0, 1]:
+            raise ValueError("Index must be 0 or 1")
+
         self.control_channel = grpc.insecure_channel('{}:{}'.format(robot_ip, CONTROL_SOCKET_PORT[index]))
         self.device_channel = grpc.insecure_channel('{}:{}'.format(robot_ip, DEVICE_SOCKET_PORT[index]))
         self.config_channel = grpc.insecure_channel('{}:{}'.format(robot_ip, CONFIG_SOCKET_PORT[index]))
         self.rtde_channel = grpc.insecure_channel('{}:{}'.format(robot_ip, RTDE_SOCKET_PORT[index]))
 
         self.control = ControlStub(self.control_channel)
         self.device = DeviceStub(self.device_channel)
         self.config = ConfigStub(self.config_channel)
         self.rtde = RTDataExchangeStub(self.rtde_channel)
 
-
-
     def __del__(self):
         if self.control_channel is not None:
             self.control_channel.close()
         if self.device_channel is not None:
             self.device_channel.close()
         if self.config_channel is not None:
             self.config_channel.close()
@@ -104,15 +49,15 @@
         request_list = []
         if analog_signal_list is not None:
             for signal in analog_signal_list:
                 request_list.append(device_msgs.AnalogSignal(address=signal['address'], voltage=signal['voltage']))
         return request_list
 
     ############################
-    # RTDE
+    # IndyDCP3 API protocols
     ############################
     def get_motion_data(self):
         """
         Motion Data:
             traj_state   -> TrajState
             traj_progress   -> int32
             is_in_motion  -> bool
@@ -121,15 +66,14 @@
             is_stopping  -> bool
             has_motion  -> bool
             speed_ratio  -> int32
             motion_id  -> int32
             remain_distance  -> float
             motion_queue_size  -> uint32
             cur_traj_progress  -> int32
-            response  -> Response
         """
         response = self.rtde.GetMotionData(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
@@ -154,67 +98,45 @@
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def get_control_state(self):
         """
         Control Data:
-            q  -> float[6]
-            qdot  -> float[6]
-            qddot  -> float[6]
-            qdes  -> float[6]
-            qdotdes  -> float[6]
-            qddotdes  -> float[6]
-            p  -> float[6]
-            pdot  -> float[6]
-            pddot  -> float[6]
-            pdes  -> float[6]
-            pdotdes  -> float[6]
-            pddotdes  -> float[6]
-
-            tau  -> float[6]
-            tau_act  -> float[6]
-            tau_ext  -> float[6]
-
+            q  -> float[]
+            qdot  -> float[]
+            qddot  -> float[]
+            qdes  -> float[]
+            qdotdes  -> float[]
+            qddotdes  -> float[]
+            p  -> float[]
+            pdot  -> float[]
+            pddot  -> float[]
+            pdes  -> float[]
+            pdotdes  -> float[]
+            pddotdes  -> float[]
+            tau  -> float[]
+            tau_act  -> float[]
+            tau_ext  -> float[]
         """
         response = self.rtde.GetControlState(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_io_data(self):
-        """
-        IO Data:
-            di   -> DigitalSignal[]
-            do   -> DigitalSignal[]
-            ai  -> AnalogSignal[]
-            ao  -> AnalogSignal[]
-            end_di  -> EndtoolSignal[]
-            end_do  -> EndtoolSignal[]
-            end_ai  -> AnalogSignal[]
-            end_ao  -> AnalogSignal[]
-            response  -> Response
-        """
-        response = self.rtde.GetIOData(common_msgs.Empty())
-        return json_format.MessageToDict(response,
-                                         including_default_value_fields=True,
-                                         preserving_proto_field_name=True,
-                                         use_integers_for_enums=True)
-
     def get_servo_data(self):
         """
         Servo Data:
             status_codes   -> string[]
             temperatures   -> float[]
             voltages  -> float[]
             currents  -> float[]
             servo_actives  -> bool[]
             brake_actives  -> bool[]
-            response  -> Response
         """
         response = self.rtde.GetServoData(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
@@ -222,15 +144,14 @@
         """
         Violation Data:
             violation_code   -> uint64
             j_index   -> uint32
             i_args  -> int32[]
             f_args  -> float[]
             violation_str  -> string
-            response  -> Response
         """
         response = self.rtde.GetViolationData(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
@@ -242,37 +163,36 @@
             sub_cmd_id  -> int32
             running_hours  -> int32
             running_mins  -> int32
             running_secs  -> int32
             program_name  -> string
             program_alarm  -> string
             program_annotation  -> string
-            response  -> Response
         """
         response = self.rtde.GetProgramData(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     ############################
-    # Device
+    # IO board and Endtool port interfaces
     ############################
-    def get_di(self) -> list:
+    def get_di(self):
         """
         address = uint32
         state = DigitalState
         """
         response = self.device.GetDI(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_do(self) -> list:
+    def get_do(self):
         """
         signals = index
         address = uint32
         state = DigitalState
         """
         response = self.device.GetDO(common_msgs.Empty())
         return json_format.MessageToDict(response,
@@ -390,15 +310,14 @@
         Device Info:
             num_joints   -> uint32
             robot_serial   -> string
             io_board_fw_ver  -> string
             core_board_fw_vers  -> string[6]
             endtool_board_fw_ver  -> string
             endtool_port_type  -> EndToolPortType
-            response  -> {code: int64, msg: string}
         """
         response = self.device.GetDeviceInfo(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
@@ -415,40 +334,54 @@
         """
         response = self.device.GetFTSensorData(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-
-
     ############################
-    # Motion Control (Move)
+    # Motion Control (Move commands)
     ############################
-    def stop_motion(self, stop_category=STOP_IMMEDIATE_BRAKE) -> dict:
+    def stop_motion(self, stop_category=StopCategory.CAT2) -> dict:
         """
          stop motion element:
-            IMMEDIATE_BRAKE = 0
-            SMOOTH_BRAKE = 1
-            SMOOTH_ONLY = 2
+            stop_category -> StopCategory
+                CAT0  = 0
+                CAT1  = 1
+                CAT2  = 2
         """
         response = self.control.StopMotion(common_msgs.StopCat(category=stop_category))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def movej(self, jtarget,
-              blending_type=NO_BLENDING,
-              base_type=ABSOLUTE_JOINT,
+              blending_type=BlendingType.NONE,
+              base_type=JointBaseType.ABSOLUTE,
               blending_radius=0.0,
               vel_ratio=Limits.JogVelRatioDefault,
               acc_ratio=Limits.JogAccRatioDefault,
-              post_condition=Property.PostCondition(),
+              post_condition=PostCondition(),
               teaching_mode=False) -> dict:
+        """
+         Joint Move:
+            blending_type -> BlendingType.Type
+                NONE
+                OVERRIDE
+                DUPLICATE
+            base_type -> JointBaseType
+                ABSOLUTE
+                RELATIVE
+            vel_ratio (0-100) -> int
+            acc_ratio (0-100) -> int
+            post_condition -> PostCondition
+            teaching_mode -> bool
+
+        """
         jtarget = control_msgs.TargetJ(j_start=[], j_target=list(jtarget), base_type=base_type)
         blending = control_msgs.BlendingType(type=blending_type, blending_radius=blending_radius)
         post_cond = control_msgs.MotionCondition()
         if post_condition is not None:
             post_cond = control_msgs.MotionCondition(
                 type_cond=post_condition.condition_type,
                 type_react=post_condition.reaction_type,
@@ -470,19 +403,19 @@
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def movej_time(self, jtarget,
-                   blending_type=NO_BLENDING,
-                   base_type=ABSOLUTE_JOINT,
+                   blending_type=BlendingType.NONE,
+                   base_type=JointBaseType.ABSOLUTE,
                    blending_radius=0.0,
                    move_time=2.0,
-                   post_condition=Property.PostCondition()) -> dict:
+                   post_condition=PostCondition()) -> dict:
         """
         jtarget = [deg, deg, deg, deg, deg, deg]
         move_time = seconds
         """
         jtarget = control_msgs.TargetJ(j_start=[], j_target=list(jtarget), base_type=base_type)
         blending = control_msgs.BlendingType(type=blending_type, blending_radius=blending_radius)
         post_cond = control_msgs.MotionCondition()
@@ -507,25 +440,29 @@
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def movel(self, ttarget,
-              blending_type=NO_BLENDING,
-              base_type=ABSOLUTE_TASK,
+              blending_type=BlendingType.NONE,
+              base_type=TaskBaseType.ABSOLUTE,
               blending_radius=0.0,
               vel_ratio=Limits.JogVelRatioDefault,
               acc_ratio=Limits.JogAccRatioDefault,
-              post_condition=Property.PostCondition(),
+              post_condition=PostCondition(),
               teaching_mode=False) -> dict:
         """
         tstart = [mm, mm, mm, deg, deg, deg]
         ttarget = [mm, mm, mm, deg, deg, deg]
-         Recover from violation
+
+            base_tye -> TaskBaseType
+                ABSOLUTE
+                RELATIVE
+                TCP
         """
         ptarget = control_msgs.TargetP(t_start=[], t_target=list(ttarget), base_type=base_type)
         blending = control_msgs.BlendingType(type=blending_type, blending_radius=blending_radius)
         post_cond = control_msgs.MotionCondition()
         if post_condition is not None:
             post_cond = control_msgs.MotionCondition(
                 type_cond=post_condition.condition_type,
@@ -548,29 +485,30 @@
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def movec(self, tpos0, tpos1,
-              blending_type=NO_BLENDING,
-              base_type=ABSOLUTE_TASK,
+              blending_type=BlendingType.NONE,
+              base_type=TaskBaseType.ABSOLUTE,
               angle=90.0,
-              setting_type=CIRCLE_POINT_SET,
+              setting_type=CircularSettingType.POINT_SET,
               move_type=control_msgs.CONSTANT,
               blending_radius=0.0,
               vel_ratio=Limits.JogVelRatioDefault,
               acc_ratio=Limits.JogAccRatioDefault,
-              post_condition=Property.PostCondition(),
+              post_condition=PostCondition(),
               teaching_mode=False) -> dict:
         """
         tstart = [mm, mm, mm, deg, deg, deg]
         ttarget = [mm, mm, mm, deg, deg, deg]
          Recover from violation
         """
+
         ctarget = control_msgs.TargetC(t_start=[], t_pos0=list(tpos0), t_pos1=list(tpos1),
                                        base_type=base_type)
         blending = control_msgs.BlendingType(type=blending_type, blending_radius=blending_radius)
         post_cond = control_msgs.MotionCondition()
         if post_condition is not None:
             post_cond = control_msgs.MotionCondition(
                 type_cond=post_condition.condition_type,
@@ -595,14 +533,29 @@
             teaching_mode=teaching_mode
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
+    ############################
+    # Motion Control (Teaching mode)
+    ############################
+    def move_home(self):
+        home_pos = self.get_home_pos()
+        self.movej(home_pos,
+                  blending_type=NO_BLENDING,
+                  base_type=JointBaseType.ABSOLUTE,
+                  blending_radius=0.0,
+                  vel_ratio=Limits.JogVelRatioDefault,
+                  acc_ratio=Limits.JogAccRatioDefault,
+                  post_condition=PostCondition(),
+                  teaching_mode=False)
+
+
 
     ############################
     # Motion Control (Teleoperation)
     ############################
     def start_teleop(self, method):
         """
         Start tele op
@@ -732,14 +685,45 @@
         """
         response = self.control.SetManualRecovery(common_msgs.State(enable=enable))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
+    def calculate_relative_pose(self, start_pos, end_pos,
+                                base_type=TaskBaseType.ABSOLUTE):
+        """
+        Calculate relative pose
+        """
+        response = self.control.CalculateRelativePose(control_msgs.CalculateRelativePoseReq(
+            start_pos=list(start_pos),
+            end_pos=list(end_pos),
+            base_type=base_type
+        ))
+        return json_format.MessageToDict(response,
+                                         including_default_value_fields=True,
+                                         preserving_proto_field_name=True,
+                                         use_integers_for_enums=True)
+
+
+    def calculate_current_pose_rel(self, current_pos, relative_pos,
+                                   base_type=TaskBaseType.ABSOLUTE):
+        """
+        Calculate current pos rel
+        """
+        response = self.control.CalculateCurrentPoseRel(control_msgs.CalculateCurrentPoseRelReq(
+            current_pos=list(current_pos),
+            relative_pos=list(relative_pos),
+            base_type=base_type
+        ))
+        return json_format.MessageToDict(response,
+                                         including_default_value_fields=True,
+                                         preserving_proto_field_name=True,
+                                         use_integers_for_enums=True)
+
     ############################
     # Program control
     ############################
     def play_program(self, prog_name: str = '', prog_idx: int = -1):
         """
          Play program
         """
@@ -778,14 +762,27 @@
         """
         response = self.control.StopProgram(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
+    def set_speed_ratio(self, speed_ratio: int):
+        """
+        Speed Ratio
+            ratio -> uint32 {0 ~ 100}
+        """
+        response = self.config.SetSpeedRatio(config_msgs.Ratio(
+            ratio=speed_ratio
+        ))
+        return json_format.MessageToDict(response,
+                                         including_default_value_fields=True,
+                                         preserving_proto_field_name=True,
+                                         use_integers_for_enums=True)
+
 
     ############################
     # Variables
     ############################
     def get_bool_variable(self):
         """
         Bool Variables:
@@ -980,14 +977,15 @@
             jpos=home_jpos
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
+
     def get_ref_frame(self):
         """
         Reference frame
             fpos -> float[6]
         """
 
         response = self.config.GetRefFrame(common_msgs.Empty())
@@ -1031,22 +1029,25 @@
             fpos=list(fpos)
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def set_speed_ratio(self, speed_ratio: int):
+
+    def get_friction_comp(self):
         """
-        Speed Ratio
-            ratio -> uint32 {0 ~ 100}
+        Friction Compensation Set:
+            joint_idx   -> uint32
+            control_comp_enable   -> bool
+            control_comp_levels   -> int32[6]
+            teaching_comp_enable   -> bool
+            teaching_comp_levels   -> int32[6]
         """
-        response = self.config.SetSpeedRatio(config_msgs.Ratio(
-            ratio=speed_ratio
-        ))
+        response = self.config.GetFrictionComp(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def set_friction_comp(self, control_comp: bool, control_comp_levels: list,
                           dt_comp: bool, dt_comp_levels: list):
@@ -1064,24 +1065,23 @@
         ))
 
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_friction_comp(self):
+
+    def get_tool_property(self):
         """
-        Friction Compensation Set:
-            joint_idx   -> uint32
-            control_comp_enable   -> bool
-            control_comp_levels   -> int32[6]
-            teaching_comp_enable   -> bool
-            teaching_comp_levels   -> int32[6]
+        Tool Properties:
+            mass   -> float
+            center_of_mass   -> float[3]
+            inertia   -> float[6]
         """
-        response = self.config.GetFrictionComp(common_msgs.Empty())
+        response = self.config.GetToolProperty(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def set_tool_property(self, mass: float, center_of_mass: list, inertia: list):
         """
@@ -1094,22 +1094,20 @@
             mass=mass, center_of_mass=list(center_of_mass), inertia=list(inertia)
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_tool_property(self):
+    def get_coll_sens_level(self):
         """
-        Tool Properties:
-            mass   -> float
-            center_of_mass   -> float[3]
-            inertia   -> float[6]
+        Collision Sensitivity Level:
+            level -> uint32
         """
-        response = self.config.GetToolProperty(common_msgs.Empty())
+        response = self.config.GetCollSensLevel(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def set_coll_sens_level(self, level: int):
         """
@@ -1120,20 +1118,29 @@
             level=level
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_coll_sens_level(self):
+    def get_coll_sens_param(self):
         """
-        Collision Sensitivity Level:
-            level -> uint32
+        Collision Params:
+            j_torque_bases                  -> double[6]
+            j_torque_tangents               -> double[6]
+            t_torque_bases                  -> double[6]
+            t_torque_tangents               -> double[6]
+            error_bases                     -> double[6]
+            error_tangents                  -> double[6]
+            t_constvel_torque_bases         -> double[6]
+            t_constvel_torque_tangents      -> double[6]
+            t_conveyor_torque_bases         -> double[6]
+            t_conveyor_torque_tangents      -> double[6]
         """
-        response = self.config.GetCollSensLevel(common_msgs.Empty())
+        response = self.config.GetCollSensParam(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def set_coll_sens_param(self, j_torque_bases, j_torque_tangents,
                             t_torque_bases, t_torque_tangents,
@@ -1163,58 +1170,56 @@
             t_conveyor_torque_tangents=list(t_conveyor_torque_tangents)
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_coll_sens_param(self):
+    def get_coll_policy(self):
         """
-        Collision Params:
-            j_torque_bases                  -> double[6]
-            j_torque_tangents               -> double[6]
-            t_torque_bases                  -> double[6]
-            t_torque_tangents               -> double[6]
-            error_bases                     -> double[6]
-            error_tangents                  -> double[6]
-            t_constvel_torque_bases         -> double[6]
-            t_constvel_torque_tangents      -> double[6]
-            t_conveyor_torque_bases         -> double[6]
-            t_conveyor_torque_tangents      -> double[6]
+        Collision Policy:
+            policy -> uint32
+            sleep_time -> float
+            gravity_time -> float
         """
-        response = self.config.GetCollSensParam(common_msgs.Empty())
+        response = self.config.GetCollPolicy(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def set_coll_policy(self, policy=COLLISION_NO_DETECT,
+    def set_coll_policy(self, policy=CollisionPolicyType.NONE,
                         sleep_time=0, gravity_time=0.1):
         """
         Collision Policies:
             policy -> uint32
             sleep_time -> float
             gravity_time -> float
         """
+        CollisionPolicyType.NONE
         response = self.config.SetCollPolicy(config_msgs.CollisionPolicy(
             policy=policy, sleep_time=sleep_time, gravity_time=gravity_time
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_coll_policy(self):
+    def get_safety_limits(self):
         """
-        Collision Policy:
-            policy -> uint32
-            sleep_time -> float
-            gravity_time -> float
+        Safety Limits:
+            power_limit             -> float
+            power_limit_ratio       -> float
+            tcp_force_limit         -> float
+            tcp_force_limit_ratio   -> float
+            tcp_speed_limit         -> float
+            tcp_speed_limit_ratio   -> float
+            joint_limits   -> float[]
         """
-        response = self.config.GetCollPolicy(common_msgs.Empty())
+        response = self.config.GetSafetyLimits(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def set_safety_limits(self, power_limit: float, power_limit_ratio: float,
                           tcp_force_limit: float, tcp_force_limit_ratio: float,
@@ -1237,49 +1242,14 @@
             # joint_limits=list(joint_limits)
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def get_safety_limits(self):
-        """
-        Safety Limits:
-            power_limit             -> float
-            power_limit_ratio       -> float
-            tcp_force_limit         -> float
-            tcp_force_limit_ratio   -> float
-            tcp_speed_limit         -> float
-            tcp_speed_limit_ratio   -> float
-            joint_limits   -> float[]
-        """
-        response = self.config.GetSafetyLimits(common_msgs.Empty())
-        return json_format.MessageToDict(response,
-                                         including_default_value_fields=True,
-                                         preserving_proto_field_name=True,
-                                         use_integers_for_enums=True)
-
-    def set_coll_tuning(self, precision=config_msgs.CollTuningConfig.MIDDLE_TUNE,
-                        tuning_space=config_msgs.CollTuningConfig.ALL_TUNE,
-                        vel_level_max=3):
-        """
-        Safety Stop Category:
-            precision = LOW(0) | MIDDLE(1) | HIGH(2)
-            tuning_space = NONE(0) | JOINT(1) | TASK(2) | ALL(3)
-            vel_level_max = 1..5
-        """
-        response = self.config.SetCollTuning(config_msgs.CollTuningConfig(
-            precision=precision,
-            tuning_space=tuning_space,
-            vel_level_max=vel_level_max
-        ))
-        return json_format.MessageToDict(response,
-                                         including_default_value_fields=True,
-                                         preserving_proto_field_name=True,
-                                         use_integers_for_enums=True)
 
     ############################
     # IndySDK related
     ############################
     def activate_sdk(self, license_key, expire_date):
         """
         license_key: license key issued by Neuromeka
@@ -1319,14 +1289,33 @@
         response = self.control.GetCustomControlMode(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     ############################
+    # Uility functions
+    ############################
+    def start_log(self):
+        """
+        Start realtime data logging
+        """
+        int_vars_to_set = [{"addr": 300, "value": 1}]
+        self.set_int_variable(int_vars_to_set)
+
+    def end_log(self):
+        """
+        Finish realtime data logging and save the realtime data in STEP
+        saved path:
+            /home/user/release/IndyDeployments/RTlog/RTLog.csv
+        """
+        int_vars_to_set = [{"addr": 300, "value": 2}]
+        self.set_int_variable(int_vars_to_set)
+
+    ############################
     # NOT Yet Released
     ############################
     def wait_time(self, time: float,
                   set_do_signal_list=None, set_end_do_signal_list=None,
                   set_ao_signal_list=None, set_end_ao_signal_list=None):
         """
          Wait time [s]
@@ -1438,15 +1427,15 @@
         response = self.config.GetDOConfigList(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
     def move_recover_joint(self, jtarget,
-                           base_type=ABSOLUTE_JOINT) -> dict:
+                           base_type=JointBaseType.ABSOLUTE) -> dict:
         """
          Move recover joint
          jtarget = [deg, deg, deg, deg, deg, deg]
         """
         response = self.control.MoveRecoverJoint(
             control_msgs.TargetJ(j_target=list(jtarget), base_type=base_type)
         )
@@ -1458,20 +1447,14 @@
     def get_control_info(self):
         response = self.control.GetControlInfo(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def ping_from_conty(self):
-        response = self.control.PingFromConty(common_msgs.Empty())
-        return json_format.MessageToDict(response,
-                                         including_default_value_fields=True,
-                                         preserving_proto_field_name=True,
-                                         use_integers_for_enums=True)
 
     def check_aproach_retract_valid(self, tpos, init_jpos, pre_tpos, post_tpos):
         """
         Check aproach retract valid
         """
         response = self.control.CheckAproachRetractValid(control_msgs.CheckAproachRetractValidReq(
             tpos=list(tpos),
@@ -1498,44 +1481,14 @@
             height=height
         ))
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def calculate_relative_pose(self, start_pos, end_pos,
-                                base_type=ABSOLUTE_TASK):
-        """
-        Calculate relative pose
-        """
-        response = self.control.CalculateRelativePose(control_msgs.CalculateRelativePoseReq(
-            start_pos=list(start_pos),
-            end_pos=list(end_pos),
-            base_type=base_type
-        ))
-        return json_format.MessageToDict(response,
-                                         including_default_value_fields=True,
-                                         preserving_proto_field_name=True,
-                                         use_integers_for_enums=True)
-
-    def calculate_current_pose_rel(self, current_pos, relative_pos,
-                                   base_type=ABSOLUTE_TASK):
-        """
-        Calculate current pos rel
-        """
-        response = self.control.CalculateCurrentPoseRel(control_msgs.CalculateCurrentPoseRelReq(
-            current_pos=list(current_pos),
-            relative_pos=list(relative_pos),
-            base_type=base_type
-        ))
-        return json_format.MessageToDict(response,
-                                         including_default_value_fields=True,
-                                         preserving_proto_field_name=True,
-                                         use_integers_for_enums=True)
-
 
     def play_tuning_program(self, prog_name: str = '', prog_idx: int = -1,
                             tuning_space=common_msgs.TUNE_ALL, precision=common_msgs.HIGH_PRECISION,
                             vel_level_max=9):
         """
         Play tuning program
         """
@@ -1627,20 +1580,20 @@
         """
         response = self.config.GetAutoServoOff(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-    def set_safety_stop_config(self, jpos_limit_stop_cat=STOPCAT_IMMEDIATE_BRAKE,
-                               jvel_limit_stop_cat=STOPCAT_IMMEDIATE_BRAKE,
-                               jtau_limit_stop_cat=STOPCAT_IMMEDIATE_BRAKE,
-                               tvel_limit_stop_cat=STOPCAT_IMMEDIATE_BRAKE,
-                               tforce_limit_stop_cat=STOPCAT_IMMEDIATE_BRAKE,
-                               power_limit_stop_cat=STOPCAT_IMMEDIATE_BRAKE):
+    def set_safety_stop_config(self, jpos_limit_stop_cat=StopCategory.CAT0,
+                               jvel_limit_stop_cat=StopCategory.CAT0,
+                               jtau_limit_stop_cat=StopCategory.CAT0,
+                               tvel_limit_stop_cat=StopCategory.CAT0,
+                               tforce_limit_stop_cat=StopCategory.CAT0,
+                               power_limit_stop_cat=StopCategory.CAT0):
         """
         Safety Stop Category:
             jpos_limit_stop_cat = IMMEDIATE_BRAKE(0) | SMOOTH_BRAKE(1) | SMOOTH_ONLY(2)
             jvel_limit_stop_cat = IMMEDIATE_BRAKE(0) | SMOOTH_BRAKE(1) | SMOOTH_ONLY(2)
             jtau_limit_stop_cat = IMMEDIATE_BRAKE(0) | SMOOTH_BRAKE(1) | SMOOTH_ONLY(2)
             tvel_limit_stop_cat = IMMEDIATE_BRAKE(0) | SMOOTH_BRAKE(1) | SMOOTH_ONLY(2)
             tforce_limit_stop_cat = IMMEDIATE_BRAKE(0) | SMOOTH_BRAKE(1) | SMOOTH_ONLY(2)
@@ -1671,9 +1624,25 @@
         """
         response = self.config.GetSafetyStopConfig(common_msgs.Empty())
         return json_format.MessageToDict(response,
                                          including_default_value_fields=True,
                                          preserving_proto_field_name=True,
                                          use_integers_for_enums=True)
 
-
-
+    def get_io_data(self):
+        """
+        IO Data:
+            di   -> DigitalSignal[]
+            do   -> DigitalSignal[]
+            ai  -> AnalogSignal[]
+            ao  -> AnalogSignal[]
+            end_di  -> EndtoolSignal[]
+            end_do  -> EndtoolSignal[]
+            end_ai  -> AnalogSignal[]
+            end_ao  -> AnalogSignal[]
+            response  -> Response
+        """
+        response = self.rtde.GetIOData(common_msgs.Empty())
+        return json_format.MessageToDict(response,
+                                         including_default_value_fields=True,
+                                         preserving_proto_field_name=True,
+                                         use_integers_for_enums=True)
```

### Comparing `neuromeka-3.2.0.1/neuromeka/moby.py` & `neuromeka-3.2.0.2/neuromeka/moby.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from .proto.grpc_wrapper import *
-from .common import *
-from .proto.common_msgs_pb2 import *
-from .proto.moby_msgs_pb2 import *
-from .proto.moby_pb2_grpc import MobyStub
-import grpc
-import time
+from neuromeka.proto import *
+from neuromeka.common import *
 
+import grpc, time
+
+
+MOBY_PORT = 20200
 
 class MobyClient:
     def __init__(self, ip_addr):
-        moby_channel = grpc.insecure_channel("{}:{}".format(ip_addr, 20200))
+        moby_channel = grpc.insecure_channel("{}:{}".format(ip_addr, MOBY_PORT))
         moby_stub = MobyStub(moby_channel)
 
         self.__moby_stub = moby_stub
 
-
     @Utils.exception_handler
     def get_moby_state(self):
         """
         Get Moby State
         -State
         -is_ready
         -is_enable
@@ -356,14 +354,7 @@
     @Utils.exception_handler
     def end_rt_logging(self):
         """
         End RT logging
         """
         return self.__moby_stub.EndRTLogging(Empty())
 
-############################
-# Main
-############################
-if __name__ == "__main__":
-    ip = '192.168.0.144'
-    moby = MobyClient(ip)
-    time.sleep(1)
```

### Comparing `neuromeka-3.2.0.1/neuromeka/motor.py` & `neuromeka-3.2.0.2/neuromeka/motor.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/common_msgs_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/common_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/config_msgs_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/config_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/config_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/config_pb2_grpc.py` & `neuromeka-3.2.0.2/neuromeka/proto/config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/control_msgs_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/control_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/control_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/control_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/control_pb2_grpc.py` & `neuromeka-3.2.0.2/neuromeka/proto/control_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/device_msgs_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/device_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/device_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/device_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/device_pb2_grpc.py` & `neuromeka-3.2.0.2/neuromeka/proto/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/ethercat_msgs_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/ethercat_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/ethercat_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2_grpc.py` & `neuromeka-3.2.0.2/neuromeka/proto/ethercat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/eyetask_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2_grpc.py` & `neuromeka-3.2.0.2/neuromeka/proto/eyetask_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/linear_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/moby_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,400 +1,409 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: linear.proto
+# source: moby.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import moby_msgs_pb2 as moby__msgs__pb2
 import common_msgs_pb2 as common__msgs__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='linear.proto',
+  name='moby.proto',
   package='Nrmk.IndyFramework',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0clinear.proto\x12\x12Nrmk.IndyFramework\x1a\x11\x63ommon_msgs.proto\"\x7f\n\x0cLinearTarget\x12\x10\n\x08start_mm\x18\x01 \x03(\x02\x12\x11\n\ttarget_mm\x18\x02 \x03(\x02\x12\x0e\n\x06vel_mm\x18\x03 \x01(\x02\x12\x0e\n\x06\x61\x63\x63_mm\x18\x04 \x01(\x02\x12\x13\n\x0bis_absolute\x18\x05 \x01(\x08\x12\x15\n\rteaching_mode\x18\n \x01(\x08\"\x89\x04\n\x08\x41xesInfo\x12\x0e\n\x06\x61\x63tive\x18\x01 \x03(\x08\x12\x0e\n\x06pos_mm\x18\x02 \x03(\x02\x12\x0e\n\x06vel_mm\x18\x03 \x03(\x02\x12\x11\n\tdespos_mm\x18\x04 \x03(\x02\x12\x11\n\tdesvel_mm\x18\x05 \x03(\x02\x12\x11\n\tdesacc_mm\x18\x06 \x03(\x02\x12\x10\n\x08num_axes\x18\n \x01(\r\x12\x36\n\x08op_state\x18\x0b \x01(\x0e\x32$.Nrmk.IndyFramework.AxesInfo.OpState\x12:\n\ntraj_state\x18\x0c \x01(\x0e\x32&.Nrmk.IndyFramework.AxesInfo.TrajState\"o\n\x07OpState\x12\x0e\n\nSYSTEM_OFF\x10\x00\x12\r\n\tSYSTEM_ON\x10\x01\x12\x0b\n\x07VIOLATE\x10\x02\x12\x10\n\x0cRECOVER_HARD\x10\x03\x12\x10\n\x0cRECOVER_SOFT\x10\x04\x12\x08\n\x04IDLE\x10\x05\x12\n\n\x06MOVING\x10\x06\"\x9c\x01\n\tTrajState\x12\r\n\tTRAJ_NONE\x10\x00\x12\r\n\tTRAJ_INIT\x10\x01\x12\r\n\tTRAJ_CALC\x10\x02\x12\r\n\tTRAJ_STBY\x10\x03\x12\x0c\n\x08TRAJ_ACC\x10\x04\x12\x0c\n\x08TRAJ_CRZ\x10\x05\x12\x0c\n\x08TRAJ_DEC\x10\x06\x12\r\n\tTRAJ_CANC\x10\x07\x12\x0c\n\x08TRAJ_FIN\x10\x08\x12\x0c\n\x08TRAJ_ERR\x10\t2\xd6\x03\n\rLinearControl\x12H\n\x0bSetServoAll\x12\x19.Nrmk.IndyFramework.State\x1a\x1c.Nrmk.IndyFramework.Response\"\x00\x12N\n\nMoveLinear\x12 .Nrmk.IndyFramework.LinearTarget\x1a\x1c.Nrmk.IndyFramework.Response\"\x00\x12I\n\nStopMotion\x12\x1b.Nrmk.IndyFramework.StopCat\x1a\x1c.Nrmk.IndyFramework.Response\"\x00\x12K\n\x0bPauseMotion\x12\x1c.Nrmk.IndyFramework.PauseCat\x1a\x1c.Nrmk.IndyFramework.Response\"\x00\x12I\n\x0cResumeMotion\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1c.Nrmk.IndyFramework.Response\"\x00\x12H\n\x0bGetAxesInfo\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1c.Nrmk.IndyFramework.AxesInfo\"\x00\x62\x06proto3'
+  serialized_pb=b'\n\nmoby.proto\x12\x12Nrmk.IndyFramework\x1a\x0fmoby_msgs.proto\x1a\x11\x63ommon_msgs.proto2\x82\x16\n\x04Moby\x12J\n\x0cGetMobyState\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1d.Nrmk.IndyFramework.MobyState\"\x00\x12T\n\x11GetMobyErrorState\x12\x19.Nrmk.IndyFramework.Empty\x1a\".Nrmk.IndyFramework.MobyErrorState\"\x00\x12\x41\n\x07Recover\x12\x19.Nrmk.IndyFramework.Empty\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12H\n\x0bGetMobyPose\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1c.Nrmk.IndyFramework.MobyPose\"\x00\x12\x46\n\nGetMobyVel\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1b.Nrmk.IndyFramework.MobyVel\"\x00\x12G\n\rResetMobyPose\x12\x19.Nrmk.IndyFramework.Empty\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12U\n\x13GetRotationAngleDeg\x12\x19.Nrmk.IndyFramework.Empty\x1a!.Nrmk.IndyFramework.SwerveDoubles\"\x00\x12O\n\rGetDriveSpeed\x12\x19.Nrmk.IndyFramework.Empty\x1a!.Nrmk.IndyFramework.SwerveDoubles\"\x00\x12J\n\x0cGetTargetVel\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1d.Nrmk.IndyFramework.TargetVel\"\x00\x12R\n\x14GetRotationZeroCount\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1d.Nrmk.IndyFramework.ZeroCount\"\x00\x12J\n\x0bGetGyroData\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1e.Nrmk.IndyFramework.DoubleVals\"\x00\x12I\n\x0fResetGyroSensor\x12\x19.Nrmk.IndyFramework.Empty\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12J\n\x0eUseGyroForOdom\x12\x1b.Nrmk.IndyFramework.BoolVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12K\n\x0fGetGyroFullData\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1b.Nrmk.IndyFramework.IMUData\"\x00\x12J\n\x0fGetIRSensorData\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1a.Nrmk.IndyFramework.IRData\"\x00\x12J\n\x0fGetUSSensorData\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1a.Nrmk.IndyFramework.USData\"\x00\x12\x46\n\nGetBMSData\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1b.Nrmk.IndyFramework.BMSData\"\x00\x12L\n\x0eSetStepControl\x12\x1d.Nrmk.IndyFramework.TargetVel\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12\x44\n\nStopMotion\x12\x19.Nrmk.IndyFramework.Empty\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12U\n\x13SetRotationAngleDeg\x12!.Nrmk.IndyFramework.SwerveDoubles\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12L\n\nDriveWheel\x12!.Nrmk.IndyFramework.SwerveDoubles\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12P\n\x16SetZeroPosAsCurrentPos\x12\x19.Nrmk.IndyFramework.Empty\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12P\n\x11SetRotationVelAcc\x12\x1e.Nrmk.IndyFramework.DoubleVals\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12R\n\x17SetRotationInterpolator\x12\x1a.Nrmk.IndyFramework.IntVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12M\n\x0eSetDriveAccDec\x12\x1e.Nrmk.IndyFramework.DoubleVals\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12U\n\x19SetDriveInterpolatorOnOff\x12\x1b.Nrmk.IndyFramework.BoolVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12T\n\x19SetRotationControllerType\x12\x1a.Nrmk.IndyFramework.IntVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12N\n\x12SetForceKinematics\x12\x1b.Nrmk.IndyFramework.BoolVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12N\n\x12GetForceKinematics\x12\x19.Nrmk.IndyFramework.Empty\x1a\x1b.Nrmk.IndyFramework.BoolVal\"\x00\x12G\n\x0bPauseBumper\x12\x1b.Nrmk.IndyFramework.BoolVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12J\n\x0eTurnLightOnOff\x12\x1b.Nrmk.IndyFramework.BoolVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12I\n\rTurnBuzzOnOff\x12\x1b.Nrmk.IndyFramework.BoolVal\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12P\n\x0fSetControlParam\x12 .Nrmk.IndyFramework.RotationGain\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12Q\n\x0fGetControlParam\x12\x1a.Nrmk.IndyFramework.IntVal\x1a .Nrmk.IndyFramework.RotationGain\"\x00\x12H\n\x0eStartRTLogging\x12\x19.Nrmk.IndyFramework.Empty\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x12\x46\n\x0c\x45ndRTLogging\x12\x19.Nrmk.IndyFramework.Empty\x1a\x19.Nrmk.IndyFramework.Empty\"\x00\x62\x06proto3'
   ,
-  dependencies=[common__msgs__pb2.DESCRIPTOR,])
+  dependencies=[moby__msgs__pb2.DESCRIPTOR,common__msgs__pb2.DESCRIPTOR,])
 
 
 
-_AXESINFO_OPSTATE = _descriptor.EnumDescriptor(
-  name='OpState',
-  full_name='Nrmk.IndyFramework.AxesInfo.OpState',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='SYSTEM_OFF', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='SYSTEM_ON', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='VIOLATE', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='RECOVER_HARD', index=3, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='RECOVER_SOFT', index=4, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='IDLE', index=5, number=5,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='MOVING', index=6, number=6,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=436,
-  serialized_end=547,
-)
-_sym_db.RegisterEnumDescriptor(_AXESINFO_OPSTATE)
-
-_AXESINFO_TRAJSTATE = _descriptor.EnumDescriptor(
-  name='TrajState',
-  full_name='Nrmk.IndyFramework.AxesInfo.TrajState',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_NONE', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_INIT', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_CALC', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_STBY', index=3, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_ACC', index=4, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_CRZ', index=5, number=5,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_DEC', index=6, number=6,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_CANC', index=7, number=7,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_FIN', index=8, number=8,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='TRAJ_ERR', index=9, number=9,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=550,
-  serialized_end=706,
-)
-_sym_db.RegisterEnumDescriptor(_AXESINFO_TRAJSTATE)
-
-
-_LINEARTARGET = _descriptor.Descriptor(
-  name='LinearTarget',
-  full_name='Nrmk.IndyFramework.LinearTarget',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='start_mm', full_name='Nrmk.IndyFramework.LinearTarget.start_mm', index=0,
-      number=1, type=2, cpp_type=6, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='target_mm', full_name='Nrmk.IndyFramework.LinearTarget.target_mm', index=1,
-      number=2, type=2, cpp_type=6, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='vel_mm', full_name='Nrmk.IndyFramework.LinearTarget.vel_mm', index=2,
-      number=3, type=2, cpp_type=6, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='acc_mm', full_name='Nrmk.IndyFramework.LinearTarget.acc_mm', index=3,
-      number=4, type=2, cpp_type=6, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='is_absolute', full_name='Nrmk.IndyFramework.LinearTarget.is_absolute', index=4,
-      number=5, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='teaching_mode', full_name='Nrmk.IndyFramework.LinearTarget.teaching_mode', index=5,
-      number=10, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=55,
-  serialized_end=182,
-)
-
-
-_AXESINFO = _descriptor.Descriptor(
-  name='AxesInfo',
-  full_name='Nrmk.IndyFramework.AxesInfo',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='active', full_name='Nrmk.IndyFramework.AxesInfo.active', index=0,
-      number=1, type=8, cpp_type=7, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='pos_mm', full_name='Nrmk.IndyFramework.AxesInfo.pos_mm', index=1,
-      number=2, type=2, cpp_type=6, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='vel_mm', full_name='Nrmk.IndyFramework.AxesInfo.vel_mm', index=2,
-      number=3, type=2, cpp_type=6, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='despos_mm', full_name='Nrmk.IndyFramework.AxesInfo.despos_mm', index=3,
-      number=4, type=2, cpp_type=6, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='desvel_mm', full_name='Nrmk.IndyFramework.AxesInfo.desvel_mm', index=4,
-      number=5, type=2, cpp_type=6, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='desacc_mm', full_name='Nrmk.IndyFramework.AxesInfo.desacc_mm', index=5,
-      number=6, type=2, cpp_type=6, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='num_axes', full_name='Nrmk.IndyFramework.AxesInfo.num_axes', index=6,
-      number=10, type=13, cpp_type=3, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='op_state', full_name='Nrmk.IndyFramework.AxesInfo.op_state', index=7,
-      number=11, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='traj_state', full_name='Nrmk.IndyFramework.AxesInfo.traj_state', index=8,
-      number=12, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-    _AXESINFO_OPSTATE,
-    _AXESINFO_TRAJSTATE,
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=185,
-  serialized_end=706,
-)
-
-_AXESINFO.fields_by_name['op_state'].enum_type = _AXESINFO_OPSTATE
-_AXESINFO.fields_by_name['traj_state'].enum_type = _AXESINFO_TRAJSTATE
-_AXESINFO_OPSTATE.containing_type = _AXESINFO
-_AXESINFO_TRAJSTATE.containing_type = _AXESINFO
-DESCRIPTOR.message_types_by_name['LinearTarget'] = _LINEARTARGET
-DESCRIPTOR.message_types_by_name['AxesInfo'] = _AXESINFO
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-LinearTarget = _reflection.GeneratedProtocolMessageType('LinearTarget', (_message.Message,), {
-  'DESCRIPTOR' : _LINEARTARGET,
-  '__module__' : 'linear_pb2'
-  # @@protoc_insertion_point(class_scope:Nrmk.IndyFramework.LinearTarget)
-  })
-_sym_db.RegisterMessage(LinearTarget)
-
-AxesInfo = _reflection.GeneratedProtocolMessageType('AxesInfo', (_message.Message,), {
-  'DESCRIPTOR' : _AXESINFO,
-  '__module__' : 'linear_pb2'
-  # @@protoc_insertion_point(class_scope:Nrmk.IndyFramework.AxesInfo)
-  })
-_sym_db.RegisterMessage(AxesInfo)
 
 
-
-_LINEARCONTROL = _descriptor.ServiceDescriptor(
-  name='LinearControl',
-  full_name='Nrmk.IndyFramework.LinearControl',
+_MOBY = _descriptor.ServiceDescriptor(
+  name='Moby',
+  full_name='Nrmk.IndyFramework.Moby',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=709,
-  serialized_end=1179,
+  serialized_start=71,
+  serialized_end=2889,
   methods=[
   _descriptor.MethodDescriptor(
-    name='SetServoAll',
-    full_name='Nrmk.IndyFramework.LinearControl.SetServoAll',
+    name='GetMobyState',
+    full_name='Nrmk.IndyFramework.Moby.GetMobyState',
     index=0,
     containing_service=None,
-    input_type=common__msgs__pb2._STATE,
-    output_type=common__msgs__pb2._RESPONSE,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._MOBYSTATE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
-    name='MoveLinear',
-    full_name='Nrmk.IndyFramework.LinearControl.MoveLinear',
+    name='GetMobyErrorState',
+    full_name='Nrmk.IndyFramework.Moby.GetMobyErrorState',
     index=1,
     containing_service=None,
-    input_type=_LINEARTARGET,
-    output_type=common__msgs__pb2._RESPONSE,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._MOBYERRORSTATE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
-    name='StopMotion',
-    full_name='Nrmk.IndyFramework.LinearControl.StopMotion',
+    name='Recover',
+    full_name='Nrmk.IndyFramework.Moby.Recover',
     index=2,
     containing_service=None,
-    input_type=common__msgs__pb2._STOPCAT,
-    output_type=common__msgs__pb2._RESPONSE,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=common__msgs__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
-    name='PauseMotion',
-    full_name='Nrmk.IndyFramework.LinearControl.PauseMotion',
+    name='GetMobyPose',
+    full_name='Nrmk.IndyFramework.Moby.GetMobyPose',
     index=3,
     containing_service=None,
-    input_type=common__msgs__pb2._PAUSECAT,
-    output_type=common__msgs__pb2._RESPONSE,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._MOBYPOSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
-    name='ResumeMotion',
-    full_name='Nrmk.IndyFramework.LinearControl.ResumeMotion',
+    name='GetMobyVel',
+    full_name='Nrmk.IndyFramework.Moby.GetMobyVel',
     index=4,
     containing_service=None,
     input_type=common__msgs__pb2._EMPTY,
-    output_type=common__msgs__pb2._RESPONSE,
+    output_type=moby__msgs__pb2._MOBYVEL,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
-    name='GetAxesInfo',
-    full_name='Nrmk.IndyFramework.LinearControl.GetAxesInfo',
+    name='ResetMobyPose',
+    full_name='Nrmk.IndyFramework.Moby.ResetMobyPose',
     index=5,
     containing_service=None,
     input_type=common__msgs__pb2._EMPTY,
-    output_type=_AXESINFO,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetRotationAngleDeg',
+    full_name='Nrmk.IndyFramework.Moby.GetRotationAngleDeg',
+    index=6,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._SWERVEDOUBLES,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetDriveSpeed',
+    full_name='Nrmk.IndyFramework.Moby.GetDriveSpeed',
+    index=7,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._SWERVEDOUBLES,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetTargetVel',
+    full_name='Nrmk.IndyFramework.Moby.GetTargetVel',
+    index=8,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._TARGETVEL,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetRotationZeroCount',
+    full_name='Nrmk.IndyFramework.Moby.GetRotationZeroCount',
+    index=9,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._ZEROCOUNT,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetGyroData',
+    full_name='Nrmk.IndyFramework.Moby.GetGyroData',
+    index=10,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._DOUBLEVALS,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ResetGyroSensor',
+    full_name='Nrmk.IndyFramework.Moby.ResetGyroSensor',
+    index=11,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='UseGyroForOdom',
+    full_name='Nrmk.IndyFramework.Moby.UseGyroForOdom',
+    index=12,
+    containing_service=None,
+    input_type=moby__msgs__pb2._BOOLVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetGyroFullData',
+    full_name='Nrmk.IndyFramework.Moby.GetGyroFullData',
+    index=13,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._IMUDATA,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetIRSensorData',
+    full_name='Nrmk.IndyFramework.Moby.GetIRSensorData',
+    index=14,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._IRDATA,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetUSSensorData',
+    full_name='Nrmk.IndyFramework.Moby.GetUSSensorData',
+    index=15,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._USDATA,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetBMSData',
+    full_name='Nrmk.IndyFramework.Moby.GetBMSData',
+    index=16,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._BMSDATA,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetStepControl',
+    full_name='Nrmk.IndyFramework.Moby.SetStepControl',
+    index=17,
+    containing_service=None,
+    input_type=moby__msgs__pb2._TARGETVEL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='StopMotion',
+    full_name='Nrmk.IndyFramework.Moby.StopMotion',
+    index=18,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetRotationAngleDeg',
+    full_name='Nrmk.IndyFramework.Moby.SetRotationAngleDeg',
+    index=19,
+    containing_service=None,
+    input_type=moby__msgs__pb2._SWERVEDOUBLES,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='DriveWheel',
+    full_name='Nrmk.IndyFramework.Moby.DriveWheel',
+    index=20,
+    containing_service=None,
+    input_type=moby__msgs__pb2._SWERVEDOUBLES,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetZeroPosAsCurrentPos',
+    full_name='Nrmk.IndyFramework.Moby.SetZeroPosAsCurrentPos',
+    index=21,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetRotationVelAcc',
+    full_name='Nrmk.IndyFramework.Moby.SetRotationVelAcc',
+    index=22,
+    containing_service=None,
+    input_type=moby__msgs__pb2._DOUBLEVALS,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetRotationInterpolator',
+    full_name='Nrmk.IndyFramework.Moby.SetRotationInterpolator',
+    index=23,
+    containing_service=None,
+    input_type=moby__msgs__pb2._INTVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetDriveAccDec',
+    full_name='Nrmk.IndyFramework.Moby.SetDriveAccDec',
+    index=24,
+    containing_service=None,
+    input_type=moby__msgs__pb2._DOUBLEVALS,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetDriveInterpolatorOnOff',
+    full_name='Nrmk.IndyFramework.Moby.SetDriveInterpolatorOnOff',
+    index=25,
+    containing_service=None,
+    input_type=moby__msgs__pb2._BOOLVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetRotationControllerType',
+    full_name='Nrmk.IndyFramework.Moby.SetRotationControllerType',
+    index=26,
+    containing_service=None,
+    input_type=moby__msgs__pb2._INTVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetForceKinematics',
+    full_name='Nrmk.IndyFramework.Moby.SetForceKinematics',
+    index=27,
+    containing_service=None,
+    input_type=moby__msgs__pb2._BOOLVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetForceKinematics',
+    full_name='Nrmk.IndyFramework.Moby.GetForceKinematics',
+    index=28,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=moby__msgs__pb2._BOOLVAL,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='PauseBumper',
+    full_name='Nrmk.IndyFramework.Moby.PauseBumper',
+    index=29,
+    containing_service=None,
+    input_type=moby__msgs__pb2._BOOLVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='TurnLightOnOff',
+    full_name='Nrmk.IndyFramework.Moby.TurnLightOnOff',
+    index=30,
+    containing_service=None,
+    input_type=moby__msgs__pb2._BOOLVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='TurnBuzzOnOff',
+    full_name='Nrmk.IndyFramework.Moby.TurnBuzzOnOff',
+    index=31,
+    containing_service=None,
+    input_type=moby__msgs__pb2._BOOLVAL,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='SetControlParam',
+    full_name='Nrmk.IndyFramework.Moby.SetControlParam',
+    index=32,
+    containing_service=None,
+    input_type=moby__msgs__pb2._ROTATIONGAIN,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetControlParam',
+    full_name='Nrmk.IndyFramework.Moby.GetControlParam',
+    index=33,
+    containing_service=None,
+    input_type=moby__msgs__pb2._INTVAL,
+    output_type=moby__msgs__pb2._ROTATIONGAIN,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='StartRTLogging',
+    full_name='Nrmk.IndyFramework.Moby.StartRTLogging',
+    index=34,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=common__msgs__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='EndRTLogging',
+    full_name='Nrmk.IndyFramework.Moby.EndRTLogging',
+    index=35,
+    containing_service=None,
+    input_type=common__msgs__pb2._EMPTY,
+    output_type=common__msgs__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
 ])
-_sym_db.RegisterServiceDescriptor(_LINEARCONTROL)
+_sym_db.RegisterServiceDescriptor(_MOBY)
 
-DESCRIPTOR.services_by_name['LinearControl'] = _LINEARCONTROL
+DESCRIPTOR.services_by_name['Moby'] = _MOBY
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/moby_msgs_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/moby_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/moby_pb2_grpc.py` & `neuromeka-3.2.0.2/neuromeka/proto/moby_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/rtde_msgs_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/rtde_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2.py` & `neuromeka-3.2.0.2/neuromeka/proto/rtde_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2_grpc.py` & `neuromeka-3.2.0.2/neuromeka/proto/rtde_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0.1/neuromeka.egg-info/PKG-INFO` & `neuromeka-3.2.0.2/neuromeka.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: neuromeka
-Version: 3.2.0.1
-Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
+Version: 3.2.0.2
+Summary: Neuromeka client protocols for IndyDCP3, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients3
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: grpcio==1.39.0
 Requires-Dist: grpcio-tools==1.39.0
 Requires-Dist: protobuf==3.17.3
 Requires-Dist: requests==2.22.0
 Requires-Dist: Pillow==9.5.0
```

### Comparing `neuromeka-3.2.0.1/neuromeka.egg-info/SOURCES.txt` & `neuromeka-3.2.0.2/neuromeka.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 README.md
 setup.py
 neuromeka/__init__.py
 neuromeka/ecat.py
+neuromeka/enums.py
 neuromeka/eye.py
-neuromeka/indy.py
 neuromeka/indydcp3.py
 neuromeka/moby.py
 neuromeka/motor.py
 neuromeka.egg-info/PKG-INFO
 neuromeka.egg-info/SOURCES.txt
 neuromeka.egg-info/dependency_links.txt
 neuromeka.egg-info/requires.txt
 neuromeka.egg-info/top_level.txt
 neuromeka/common/__init__.py
-neuromeka/common/config.py
-neuromeka/common/dcp_addr.py
-neuromeka/common/global_timer.py
 neuromeka/common/jsmin.py
-neuromeka/common/limits.py
-neuromeka/common/singleton_meta.py
+neuromeka/common/record_plot.py
 neuromeka/common/utils.py
-neuromeka/common/property/Application.py
-neuromeka/common/property/Collision.py
-neuromeka/common/property/Log.py
-neuromeka/common/property/Modbus.py
-neuromeka/common/property/Motion.py
-neuromeka/common/property/Timer.py
-neuromeka/common/property/TrackConveyor.py
-neuromeka/common/property/Vision.py
-neuromeka/common/property/__init__.py
 neuromeka/proto/__init__.py
 neuromeka/proto/common_msgs_pb2.py
 neuromeka/proto/common_msgs_pb2_grpc.py
 neuromeka/proto/config_msgs_pb2.py
 neuromeka/proto/config_msgs_pb2_grpc.py
 neuromeka/proto/config_pb2.py
 neuromeka/proto/config_pb2_grpc.py
@@ -46,24 +33,15 @@
 neuromeka/proto/device_pb2_grpc.py
 neuromeka/proto/ethercat_msgs_pb2.py
 neuromeka/proto/ethercat_msgs_pb2_grpc.py
 neuromeka/proto/ethercat_pb2.py
 neuromeka/proto/ethercat_pb2_grpc.py
 neuromeka/proto/eyetask_pb2.py
 neuromeka/proto/eyetask_pb2_grpc.py
-neuromeka/proto/grpc_wrapper.py
-neuromeka/proto/linear_pb2.py
-neuromeka/proto/linear_pb2_grpc.py
 neuromeka/proto/moby_msgs_pb2.py
 neuromeka/proto/moby_msgs_pb2_grpc.py
 neuromeka/proto/moby_pb2.py
 neuromeka/proto/moby_pb2_grpc.py
-neuromeka/proto/plotting_pb2.py
-neuromeka/proto/plotting_pb2_grpc.py
 neuromeka/proto/rtde_msgs_pb2.py
 neuromeka/proto/rtde_msgs_pb2_grpc.py
 neuromeka/proto/rtde_pb2.py
-neuromeka/proto/rtde_pb2_grpc.py
-neuromeka/proto/shared_msgs_pb2.py
-neuromeka/proto/shared_msgs_pb2_grpc.py
-neuromeka/proto/teleop_dev_pb2.py
-neuromeka/proto/teleop_dev_pb2_grpc.py
+neuromeka/proto/rtde_pb2_grpc.py
```

### Comparing `neuromeka-3.2.0.1/setup.py` & `neuromeka-3.2.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,55 @@
 from setuptools import setup, find_packages
+import sys
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
+if sys.version_info < (3, 9):
+    install_requires = [
+        "grpcio==1.39.0",
+        "grpcio-tools==1.39.0",
+        "protobuf==3.17.3",
+        "requests==2.22.0",
+        "Pillow==9.5.0",
+        "numpy==1.21.6",
+        "pyModbusTCP==0.2.1",
+        "netifaces==0.11.0"
+    ]
+else:
+    install_requires = [
+        "grpcio",
+        "grpcio-tools",
+        "protobuf",
+        "requests",
+        "Pillow",
+        "numpy",
+        "pyModbusTCP",
+        "netifaces"
+    ]
+
 setup(
     name="neuromeka",
-    version="3.2.0.1",
+    version="3.2.0.2",
     author="Neuromeka",
     author_email="youngjin.heo@neuromeka.com",
-    description="Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor",
+    description="Neuromeka client protocols for IndyDCP3, IndyEye, Moby, Ecat, and Motor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/neuromeka-robotics/neuromeka-clients3",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10"
     ],
     python_requires=">=3.6",
-    install_requires=[
-        "grpcio==1.39.0",
-        "grpcio-tools==1.39.0",
-        "protobuf==3.17.3",
-        "requests==2.22.0",
-        "Pillow==9.5.0",
-        "numpy==1.21.6",
-        "pyModbusTCP==0.2.1",
-        "netifaces==0.11.0"
-    ],
+    install_requires=install_requires,
 )
```

