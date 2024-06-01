# Comparing `tmp/ubicoders-vrobots-0.2.8.tar.gz` & `tmp/ubicoders-vrobots-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubicoders-vrobots-0.2.8.tar", last modified: Sat Jun  1 23:13:42 2024, max compression
+gzip compressed data, was "ubicoders-vrobots-0.2.9.tar", last modified: Sat Jun  1 23:16:30 2024, max compression
```

## Comparing `ubicoders-vrobots-0.2.8.tar` & `ubicoders-vrobots-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.553772 ubicoders-vrobots-0.2.8/
--rwxrwxrwx   0 root         (0) root         (0)    35804 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:13:42.553522 ubicoders-vrobots-0.2.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      460 2024-05-29 02:45:41.000000 ubicoders-vrobots-0.2.8/README.md
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-06-01 23:13:42.554686 ubicoders-vrobots-0.2.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      533 2024-06-01 23:09:56.000000 ubicoders-vrobots-0.2.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.517895 ubicoders-vrobots-0.2.8/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.524275 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/
--rwxrwxrwx   0 root         (0) root         (0)      323 2024-05-27 23:15:35.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.533810 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1819 2024-05-26 02:41:53.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py
--rwxrwxrwx   0 root         (0) root         (0)     1756 2024-05-29 03:04:27.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py
--rwxrwxrwx   0 root         (0) root         (0)      608 2024-05-26 02:42:15.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py
--rwxrwxrwx   0 root         (0) root         (0)     2556 2024-05-29 04:23:15.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.539988 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3488 2024-05-29 04:04:33.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/clientutils.py
--rwxrwxrwx   0 root         (0) root         (0)     3869 2024-06-01 22:33:41.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/msg_helper.py
--rwxrwxrwx   0 root         (0) root         (0)     2093 2024-05-29 04:20:09.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/service_client.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-28 00:22:01.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py
--rwxrwxrwx   0 root         (0) root         (0)     2170 2024-05-29 02:19:43.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py
--rwxrwxrwx   0 root         (0) root         (0)     1754 2024-05-28 00:18:20.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py
--rwxrwxrwx   0 root         (0) root         (0)     1529 2024-06-01 22:18:32.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.541214 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:35:15.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4010 2024-05-28 21:08:29.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/gen_all.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.552191 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/
--rwxrwxrwx   0 root         (0) root         (0)      414 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/VROBOTS_CMDS.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    21240 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     2297 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     8501 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     7719 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    11802 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    17199 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    13344 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     9341 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     8454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    12454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    24641 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.529831 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1935 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       71 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.920161 ubicoders-vrobots-0.2.9/
+-rwxrwxrwx   0 root         (0) root         (0)    35804 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:16:30.919939 ubicoders-vrobots-0.2.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      460 2024-05-29 02:45:41.000000 ubicoders-vrobots-0.2.9/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-06-01 23:16:30.921016 ubicoders-vrobots-0.2.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      533 2024-06-01 23:16:27.000000 ubicoders-vrobots-0.2.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.892849 ubicoders-vrobots-0.2.9/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.897120 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/
+-rwxrwxrwx   0 root         (0) root         (0)      337 2024-06-01 23:16:02.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.903312 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1819 2024-05-26 02:41:53.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py
+-rwxrwxrwx   0 root         (0) root         (0)     1756 2024-05-29 03:04:27.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py
+-rwxrwxrwx   0 root         (0) root         (0)      608 2024-05-26 02:42:15.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py
+-rwxrwxrwx   0 root         (0) root         (0)     2556 2024-05-29 04:23:15.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.907941 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3488 2024-05-29 04:04:33.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/clientutils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3869 2024-06-01 22:33:41.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/msg_helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     2093 2024-05-29 04:20:09.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/service_client.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-28 00:22:01.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py
+-rwxrwxrwx   0 root         (0) root         (0)     2170 2024-05-29 02:19:43.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py
+-rwxrwxrwx   0 root         (0) root         (0)     1754 2024-05-28 00:18:20.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py
+-rwxrwxrwx   0 root         (0) root         (0)     1529 2024-06-01 22:18:32.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.908986 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:35:15.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4010 2024-05-28 21:08:29.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/gen_all.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.918528 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/
+-rwxrwxrwx   0 root         (0) root         (0)      414 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/VROBOTS_CMDS.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21240 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     2297 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     8501 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     7719 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    11802 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    17199 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    13344 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     9341 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     8454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    12454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    24641 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:16:30.900259 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:16:30.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1935 2024-06-01 23:16:30.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-06-01 23:16:30.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       71 2024-06-01 23:16:30.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-06-01 23:16:30.000000 ubicoders-vrobots-0.2.9/src/ubicoders_vrobots.egg-info/top_level.txt
```

### Comparing `ubicoders-vrobots-0.2.8/LICENSE` & `ubicoders-vrobots-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/setup.py` & `ubicoders-vrobots-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ubicoders-vrobots",
-    version="0.2.8",
+    version="0.2.9",
     license="GPLv3",
     author="Elliot Lee",
     author_email="info@airnh.ca",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url="https://github.com/ubicoders0/vrobots",
     keywords="ubicoders virtual robots",
```

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/clientutils.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/clientutils.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/msg_helper.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/msg_helper.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/service_client.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/service_client.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/gen_all.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/gen_all.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/SOURCES.txt` & `ubicoders-vrobots-0.2.9/src/ubicoders_vrobots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

