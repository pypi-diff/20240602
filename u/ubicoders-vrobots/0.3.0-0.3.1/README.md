# Comparing `tmp/ubicoders-vrobots-0.3.0.tar.gz` & `tmp/ubicoders-vrobots-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubicoders-vrobots-0.3.0.tar", last modified: Sat Jun  1 23:22:36 2024, max compression
+gzip compressed data, was "ubicoders-vrobots-0.3.1.tar", last modified: Sun Jun  2 01:55:06 2024, max compression
```

## Comparing `ubicoders-vrobots-0.3.0.tar` & `ubicoders-vrobots-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.170689 ubicoders-vrobots-0.3.0/
--rwxrwxrwx   0 root         (0) root         (0)    35804 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.3.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:22:36.170262 ubicoders-vrobots-0.3.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      460 2024-05-29 02:45:41.000000 ubicoders-vrobots-0.3.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-06-01 23:22:36.172381 ubicoders-vrobots-0.3.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      533 2024-06-01 23:22:34.000000 ubicoders-vrobots-0.3.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.133039 ubicoders-vrobots-0.3.0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.137190 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/
--rwxrwxrwx   0 root         (0) root         (0)      337 2024-06-01 23:16:02.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.143319 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1819 2024-05-26 02:41:53.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py
--rwxrwxrwx   0 root         (0) root         (0)     1756 2024-05-29 03:04:27.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py
--rwxrwxrwx   0 root         (0) root         (0)      608 2024-05-26 02:42:15.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py
--rwxrwxrwx   0 root         (0) root         (0)     2556 2024-05-29 04:23:15.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.150967 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3488 2024-06-01 23:22:22.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/clientutils.py
--rwxrwxrwx   0 root         (0) root         (0)     3993 2024-06-01 23:22:12.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/msg_helper.py
--rwxrwxrwx   0 root         (0) root         (0)     2093 2024-05-29 04:20:09.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/service_client.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-28 00:22:01.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py
--rwxrwxrwx   0 root         (0) root         (0)     2170 2024-05-29 02:19:43.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py
--rwxrwxrwx   0 root         (0) root         (0)     1754 2024-05-28 00:18:20.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py
--rwxrwxrwx   0 root         (0) root         (0)     1529 2024-06-01 22:18:32.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.152833 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:35:15.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4010 2024-05-28 21:08:29.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/gen_all.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.167796 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/
--rwxrwxrwx   0 root         (0) root         (0)      414 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/VROBOTS_CMDS.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    21240 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     2297 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     8501 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     7719 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    11802 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    17199 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    13344 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     9341 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     8454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    12454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    24641 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:22:36.140348 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:22:36.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1935 2024-06-01 23:22:36.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-06-01 23:22:36.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       71 2024-06-01 23:22:36.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-06-01 23:22:36.000000 ubicoders-vrobots-0.3.0/src/ubicoders_vrobots.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.663146 ubicoders-vrobots-0.3.1/
+-rwxrwxrwx   0 root         (0) root         (0)    35804 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.3.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-02 01:55:06.662862 ubicoders-vrobots-0.3.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      460 2024-05-29 02:45:41.000000 ubicoders-vrobots-0.3.1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-06-02 01:55:06.664374 ubicoders-vrobots-0.3.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      533 2024-06-02 01:55:02.000000 ubicoders-vrobots-0.3.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.619277 ubicoders-vrobots-0.3.1/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.624013 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/
+-rwxrwxrwx   0 root         (0) root         (0)      337 2024-06-01 23:56:30.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.635164 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1819 2024-05-26 02:41:53.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py
+-rwxrwxrwx   0 root         (0) root         (0)     1762 2024-06-02 01:54:41.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py
+-rwxrwxrwx   0 root         (0) root         (0)      608 2024-06-02 00:56:36.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py
+-rwxrwxrwx   0 root         (0) root         (0)     2598 2024-06-02 01:54:51.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.643598 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3488 2024-06-01 23:22:22.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/clientutils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3993 2024-06-01 23:22:12.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/msg_helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     2093 2024-05-29 04:20:09.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/service_client.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-28 00:22:01.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py
+-rwxrwxrwx   0 root         (0) root         (0)     2170 2024-05-29 02:19:43.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py
+-rwxrwxrwx   0 root         (0) root         (0)     1754 2024-05-28 00:18:20.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py
+-rwxrwxrwx   0 root         (0) root         (0)     1529 2024-06-01 22:18:32.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.645649 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:35:15.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4010 2024-05-28 21:08:29.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/gen_all.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.660974 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/
+-rwxrwxrwx   0 root         (0) root         (0)      414 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/VROBOTS_CMDS.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21240 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     2297 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     8501 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     7719 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    11802 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    17199 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    13344 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     9341 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     8454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    12454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    24641 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-02 01:55:06.629604 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-02 01:55:06.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1935 2024-06-02 01:55:06.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-06-02 01:55:06.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       71 2024-06-02 01:55:06.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-06-02 01:55:06.000000 ubicoders-vrobots-0.3.1/src/ubicoders_vrobots.egg-info/top_level.txt
```

### Comparing `ubicoders-vrobots-0.3.0/LICENSE` & `ubicoders-vrobots-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/setup.py` & `ubicoders-vrobots-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ubicoders-vrobots",
-    version="0.3.0",
+    version="0.3.1",
     license="GPLv3",
     author="Elliot Lee",
     author_email="info@airnh.ca",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url="https://github.com/ubicoders0/vrobots",
     keywords="ubicoders virtual robots",
```

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 continue
 
             name = get_name_from_msg(message)
             if name is None:
                 continue
             # print(f"Client connected: {name}")
 
-            upsert_ws_list(name, websocket)
+            await upsert_ws_list(name, websocket)
 
             for named_ws in WSList:
                 # print(f"ws_list: {named_ws.name}")
                 if named_ws.name == name:
                     continue
                 # print(len(WebSocketList))
                 try:
```

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,49 +16,49 @@
 
 
 class NamedWebsocket:
     def __init__(self, name, ws) -> None:
         self.ws = ws
         self.name = name
 
-    def handle_new_msg(self, name, ws):
+    async def handle_new_msg(self, name, ws):
         if name is None or self.name != name:
             return
-        self.handle_dup(ws)
+        await self.handle_dup(ws)
 
-    def handle_dup(self, ws):
+    async def handle_dup(self, ws):
         if self.validate_dup(ws) is True:
             return
         else:
-            self.ws.close()
+            await self.ws.close()
             self.ws = ws
 
     def validate_dup(self, ws):
         if self.ws is ws:
             return True
         else:
             return False
 
     def remove(self):
         print(f"Removing {self.name} from ws_list")
         WSList.remove(self)
 
 
-def upsert_ws_list(name, ws):
+async def upsert_ws_list(name, ws):
     # check if ws_list has name
     for named_ws in WSList:
         if named_ws.name == name:
-            named_ws.handle_new_msg(name, ws)
+            await named_ws.handle_new_msg(name, ws)
             return
 
     # if new, push
     print(f"{name} connected.")
     named_ws = NamedWebsocket(name, ws)
     WSList.append(named_ws)
-    named_ws.handle_new_msg(name, ws)
+    await named_ws.handle_new_msg(name, ws)
 
 
 def remove_ws_list(name):
     for named_ws in WSList:
         if named_ws.name == name:
             print(f"{name} disconnected.")
             named_ws.remove()
```

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/clientutils.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/clientutils.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/msg_helper.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/msg_helper.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/service_client.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/service_client.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/gen_all.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/gen_all.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.3.0/src/ubicoders_vrobots.egg-info/SOURCES.txt` & `ubicoders-vrobots-0.3.1/src/ubicoders_vrobots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

