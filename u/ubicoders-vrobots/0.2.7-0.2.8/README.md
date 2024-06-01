# Comparing `tmp/ubicoders-vrobots-0.2.7.tar.gz` & `tmp/ubicoders-vrobots-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubicoders-vrobots-0.2.7.tar", last modified: Tue Mar 19 20:13:01 2024, max compression
+gzip compressed data, was "ubicoders-vrobots-0.2.8.tar", last modified: Sat Jun  1 23:13:42 2024, max compression
```

## Comparing `ubicoders-vrobots-0.2.7.tar` & `ubicoders-vrobots-0.2.8.tar`

### file list

```diff
@@ -1,40 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.142744 ubicoders-vrobots-0.2.7/
--rwxrwxrwx   0 root         (0) root         (0)    35804 2024-02-08 04:08:24.000000 ubicoders-vrobots-0.2.7/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      381 2024-03-19 20:13:01.142567 ubicoders-vrobots-0.2.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      337 2024-03-18 19:20:43.000000 ubicoders-vrobots-0.2.7/README.md
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-03-19 20:13:01.143700 ubicoders-vrobots-0.2.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      462 2024-03-19 20:12:59.000000 ubicoders-vrobots-0.2.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.118982 ubicoders-vrobots-0.2.7/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.124291 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/
--rwxrwxrwx   0 root         (0) root         (0)      328 2024-03-19 20:05:13.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.131222 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-08 04:08:24.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1790 2024-03-19 19:49:36.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py
--rwxrwxrwx   0 root         (0) root         (0)     1760 2024-03-18 22:53:32.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py
--rwxrwxrwx   0 root         (0) root         (0)      664 2024-03-18 22:50:18.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py
--rwxrwxrwx   0 root         (0) root         (0)     1952 2024-02-09 23:50:03.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.135720 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-08 04:08:24.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2337 2024-02-08 22:17:14.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/clientutils.py
--rwxrwxrwx   0 root         (0) root         (0)     3872 2024-02-08 21:16:25.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/msg_helper.py
--rwxrwxrwx   0 root         (0) root         (0)     2720 2024-03-19 20:12:54.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/vrobots_general.py
--rwxrwxrwx   0 root         (0) root         (0)     2177 2024-02-10 00:13:18.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py
--rwxrwxrwx   0 root         (0) root         (0)     2179 2024-02-10 00:13:07.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py
--rwxrwxrwx   0 root         (0) root         (0)     2338 2024-02-10 00:16:19.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.136834 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-10 03:54:16.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1511 2024-02-08 04:08:55.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/gen_all.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.141447 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-02-09 01:02:40.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10471 2024-02-09 01:02:40.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     2297 2024-02-09 01:02:40.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     8501 2024-02-09 01:02:40.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py
--rwxrwxrwx   0 root         (0) root         (0)     7719 2024-02-09 01:02:40.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    11802 2024-02-09 01:02:40.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py
--rwxrwxrwx   0 root         (0) root         (0)    22051 2024-02-09 01:02:40.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-19 20:13:01.127806 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      381 2024-03-19 20:13:01.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1470 2024-03-19 20:13:01.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-03-19 20:13:01.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       62 2024-03-19 20:13:01.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-03-19 20:13:01.000000 ubicoders-vrobots-0.2.7/src/ubicoders_vrobots.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.553772 ubicoders-vrobots-0.2.8/
+-rwxrwxrwx   0 root         (0) root         (0)    35804 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.8/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:13:42.553522 ubicoders-vrobots-0.2.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      460 2024-05-29 02:45:41.000000 ubicoders-vrobots-0.2.8/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-06-01 23:13:42.554686 ubicoders-vrobots-0.2.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      533 2024-06-01 23:09:56.000000 ubicoders-vrobots-0.2.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.517895 ubicoders-vrobots-0.2.8/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.524275 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/
+-rwxrwxrwx   0 root         (0) root         (0)      323 2024-05-27 23:15:35.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.533810 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1819 2024-05-26 02:41:53.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py
+-rwxrwxrwx   0 root         (0) root         (0)     1756 2024-05-29 03:04:27.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py
+-rwxrwxrwx   0 root         (0) root         (0)      608 2024-05-26 02:42:15.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vrb_main.py
+-rwxrwxrwx   0 root         (0) root         (0)     2556 2024-05-29 04:23:15.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.539988 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:33:56.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3488 2024-05-29 04:04:33.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/clientutils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3869 2024-06-01 22:33:41.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/msg_helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     2093 2024-05-29 04:20:09.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/service_client.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-28 00:22:01.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py
+-rwxrwxrwx   0 root         (0) root         (0)     2170 2024-05-29 02:19:43.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py
+-rwxrwxrwx   0 root         (0) root         (0)     1754 2024-05-28 00:18:20.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py
+-rwxrwxrwx   0 root         (0) root         (0)     1529 2024-06-01 22:18:32.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.541214 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-26 02:35:15.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4010 2024-05-28 21:08:29.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/gen_all.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.552191 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/
+-rwxrwxrwx   0 root         (0) root         (0)      414 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/VROBOTS_CMDS.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21240 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     2297 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     8501 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     7719 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    11802 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    17199 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    13344 2024-05-29 00:36:47.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     9341 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)     8454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    12454 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py
+-rwxrwxrwx   0 root         (0) root         (0)    24641 2024-05-29 00:36:48.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-06-01 23:13:42.529831 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      390 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1935 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       71 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-06-01 23:13:42.000000 ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/top_level.txt
```

### Comparing `ubicoders-vrobots-0.2.7/LICENSE` & `ubicoders-vrobots-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 from fastapi import FastAPI
 import uvicorn
 import websockets
 import json
 from fastapi.middleware.cors import CORSMiddleware  # Import CORSMiddleware
 
+
 async def check_alive(uri):
     try:
         async with websockets.connect(uri) as websocket:
-            await websocket.send(b'ping')
+            await websocket.send(b"ping")
             response = await websocket.recv()
-            return response == b'pong'
-            
+            return response == b"pong"
+
     except websockets.exceptions.ConnectionClosed:
         return False
 
+
 # Example FastAPI app definition
 def create_app():
     app = FastAPI()
     app.add_middleware(
         CORSMiddleware,
-        allow_origins=["*"],  # Allows all origins, replace with your specific origins in production
+        allow_origins=[
+            "*"
+        ],  # Allows all origins, replace with your specific origins in production
         allow_credentials=True,
         allow_methods=["*"],  # Allows all methods
         allow_headers=["*"],  # Allows all headers
     )
 
     @app.get("/")
     async def default():
         return "ok"
-    
+
     @app.get("/ping")
     async def default():
         uri = "ws://localhost:12740"  # Replace with your server URI
         try:
             alive = await check_alive(uri)
-            if (alive):
-                return {"status": 1, "data":None, "msg":"ok"}
+            if alive:
+                return {"status": 1, "data": None, "msg": "ok"}
             else:
-                return {"status": 0, "data":None, "msg":"unreachable"}
+                return {"status": 0, "data": None, "msg": "unreachable"}
         except Exception as e:
-            return {"status": -1, "data":None, "msg":"error"}
+            return {"status": -1, "data": None, "msg": "error"}
+
     return app
 
+
 # Function to run a FastAPI app with uvicorn programmatically
 def run_server(port=12741):
     app = create_app()
-    config = uvicorn.Config(app=app, host="0.0.0.0", port=port, loop="asyncio",  log_level="warning")
+    config = uvicorn.Config(
+        app=app, host="0.0.0.0", port=port, loop="asyncio", log_level="warning"
+    )
     server = uvicorn.Server(config)
     # print(f"\033[92mVRobot HC server is running @ port {port}\033[0m")
     server.run()
 
 
 if __name__ == "__main__":
     run_server()
-
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 async def echo(websocket):
     name = None
     try:
         async for message in websocket:
 
-            if message == b'ping':
-                await websocket.send(b'pong')
+            if message == b"ping":
+                await websocket.send(b"pong")
                 continue
 
             if EmptyMsg.EmptyMsgBufferHasIdentifier(message, 0) is True:
                 continue
 
             name = get_name_from_msg(message)
             if name is None:
@@ -52,11 +52,9 @@
 
     print(f"\033[92mVirtual Robots Bridge is running @ port {port}\033[0m")
     start_server = websockets.serve(echo, "0.0.0.0", port)
     loop.run_until_complete(start_server)
     loop.run_forever()
 
 
-
-
 if __name__ == "__main__":
     run_bridge_server()
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_bridge/ws_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from ubicoders_vrobots.vrobots_msgs.python.srv_omr_walls_generated import (
+    SrvOMRWall,
+    SrvOMRWallT,
+)
 from ..vrobots_msgs.python.states_generated import StatesMsg
 from ..vrobots_msgs.python.empty_generated import EmptyMsg
 from ..vrobots_msgs.python.commands_generated import CommandMsg
 
 
 class WebSocketList(list):
     def __init__(self, *args):
@@ -61,16 +65,27 @@
             return
 
 
 def get_name_from_msg(msg):
 
     if StatesMsg.StatesMsgBufferHasIdentifier(msg, 0) is True:
         robots_all = StatesMsg.GetRootAsStatesMsg(msg)
+        if robots_all == None or robots_all.Name() == None:
+            return "unregistered"
         name = robots_all.Name().decode("utf-8")
         return name
 
     if CommandMsg.CommandMsgBufferHasIdentifier(msg, 0) is True:
         cmd = CommandMsg.GetRootAsCommandMsg(msg)
+        if robots_all == None or robots_all.Name() == None:
+            return "unregistered"
         name = cmd.Name().decode("utf-8")
         return name
 
+    if SrvOMRWall.SrvOMRWallBufferHasIdentifier(msg, 0) is True:
+        srv_omr_wall = SrvOMRWall.GetRootAsSrvOMRWall(msg)
+        if robots_all == None or robots_all.Name() == None:
+            return "unregistered"
+        name = srv_omr_wall.Name().decode("utf-8")
+        return name
+
     return None
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/msg_helper.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/msg_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from ..vrobots_msgs.python.states_generated import (
-    Vec3MsgT,
-    Vec4MsgT,
-    StatesMsgT,
-)
+from ..vrobots_msgs.python.states_generated import *
+
 
 import json
 
 
 class Vec4(Vec4MsgT):
     def __init__(self, instance: Vec4MsgT):
         super().__init__()
@@ -88,14 +85,15 @@
         self.lin_pos = Vec3(instance.linPos)
         self.ang_acc = Vec3(instance.angAcc)
         self.ang_vel = Vec3(instance.angVel)
         self.euler = Vec3(instance.euler)
         self.euler_dot = Vec3(instance.eulerDot)
         self.quaternion = Vec4(instance.quaternion)
         self.pwm = instance.pwm
+        self.actuators = instance.actuators
         self.force = Vec3(instance.force)
         self.torque = Vec3(instance.torque)
         self.accelerometer = Vec3(instance.accelerometer)
         self.gyroscope = Vec3(instance.gyroscope)
         self.magnetometer = Vec3(instance.magnetometer)
 
     def get_dict_data(self):
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,40 @@
 import flatbuffers
+from ubicoders_vrobots.vrobots_msgs.python.VROBOTS_CMDS import CMD_DICT
 from .msg_helper import VRobotState
 from ..vrobots_msgs.python.states_generated import *
 from ..vrobots_msgs.python.commands_generated import *
 from .clientutils import VirtualRobot, System
+import time
 
 
 class Helicopter2D(VirtualRobot):
     def __init__(self) -> None:
-        self.states = VRobotState(None)
-        self.force = 0
+        self.states: VRobotState = VRobotState(None)
+        self.force: float = 0
 
     def pack_cmd_force(self) -> bytes:
         builder = flatbuffers.Builder(512)
-        sender = builder.CreateString("python")
-        CommandMsgStart(builder)
-        CommandMsgAddName(builder, sender)
-        CommandMsgAddId(builder, 20)
-        CommandMsgAddFloatVal(builder, self.force)
-        os = CommandMsgEnd(builder)
-        builder.Finish(os, b"CMD0")
-        return builder.Output()
-
-    def pack_cmd_reset(self) -> bytes:
-        builder = flatbuffers.Builder(512)
-        sender = builder.CreateString("python")
-        CommandMsgStart(builder)
-        CommandMsgAddName(builder, sender)
-        CommandMsgAddId(builder, 100)
-        os = CommandMsgEnd(builder)
+        cmdMsgT = CommandMsgT()
+        cmdMsgT.timestamp = time.time()
+        cmdMsgT.name = "python"
+        cmdMsgT.id = CMD_DICT["set_force"]
+        cmdMsgT.float_val = self.force
+        os = cmdMsgT.Pack(builder=builder)
         builder.Finish(os, b"CMD0")
         return builder.Output()
 
     def pack_setup(self) -> List[bytes]:
-        return []
+        ba_reset = self.pack_cmd_reset()
+        return [ba_reset]
 
     def pack(self) -> List[bytes]:
         cmd_force = self.pack_cmd_force()
         return [cmd_force]
 
-    def unpack(self, msg):  # FB_MultirotorMsgAll
-        objdata = StatesMsgT.InitFromPackedBuf(msg, 0)
-        name = objdata.name.decode("utf-8")
-        if (name is not None) and (name != "heli"):
-            return
-        self.states = VRobotState(objdata)
-        # ## TODO onboard pid params
-
 
 # ===============================================================================
 # dev code
 # ===============================================================================
 
 heli = Helicopter2D()
 
@@ -60,16 +45,16 @@
 
     def setup(self):
         # mr.mass = 2 kg
         pass
 
     def loop(self):
         states = heli.states
-        print(states.lin_pos)
-        print(states.lin_vel)
+        # print(states.lin_pos)
+        # print(states.lin_vel)
 
         heli.force = 20
 
 
 if __name__ == "__main__":
     sys = System(heli, UbicodersMain())
     sys.start()
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import flatbuffers
+from ubicoders_vrobots.vrobots_msgs.python.VROBOTS_CMDS import CMD_DICT
 from .msg_helper import VRobotState
 from ..vrobots_msgs.python.states_generated import *
 from ..vrobots_msgs.python.commands_generated import *
 from .clientutils import VirtualRobot, System
 
 
 class Multirotor(VirtualRobot):
@@ -13,46 +14,28 @@
     def set_pwm(self, m0, m1, m2, m3):
         self.pwm = [m0, m1, m2, m3]
 
     def pack_cmd_pwm(self) -> bytes:
         builder = flatbuffers.Builder(512)
         cmd_msg = CommandMsgT()
         cmd_msg.name = "python"
-        cmd_msg.id = 22
+        cmd_msg.id = CMD_DICT["set_pwm"]
         cmd_msg.intArr = [int(num) for num in self.pwm]
         os = cmd_msg.Pack(builder)
         builder.Finish(os, b"CMD0")
         return builder.Output()
 
-    def pack_cmd_reset(self) -> bytes:
-        builder = flatbuffers.Builder(512)
-        sender = builder.CreateString("python")
-        CommandMsgStart(builder)
-        CommandMsgAddName(builder, sender)
-        CommandMsgAddId(builder, 100)
-        os = CommandMsgEnd(builder)
-        builder.Finish(os, b"CMD0")
-        return builder.Output()
-
     def pack_setup(self) -> List[bytes]:
         cmd_reset = self.pack_cmd_reset()
         return [cmd_reset]
 
     def pack(self) -> List[bytes]:
         cmd_pwm = self.pack_cmd_pwm()
         return [cmd_pwm]
 
-    def unpack(self, msg):  # FB_MultirotorMsgAll
-        objdata = StatesMsgT.InitFromPackedBuf(msg, 0)
-        name = objdata.name.decode("utf-8")
-        if (name is not None) and (name != "multirotor"):
-            return
-        self.states = VRobotState(objdata)
-        # ## TODO onboard pid params
-
 
 # ===============================================================================
 # dev code
 # ===============================================================================
 
 mr = Multirotor()
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py`

 * *Files identical despite different names*

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             return self._tab.String(o + self._tab.Pos)
         return None
 
     # PARAM_GlobalMsg
     def Timestamp(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+            return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
         return 0.0
 
     # PARAM_GlobalMsg
     def Scene(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             return self._tab.String(o + self._tab.Pos)
@@ -108,15 +108,15 @@
 def PARAM_GlobalMsgStart(builder):
     builder.StartObject(11)
 
 def PARAM_GlobalMsgAddName(builder, name):
     builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(name), 0)
 
 def PARAM_GlobalMsgAddTimestamp(builder, timestamp):
-    builder.PrependFloat32Slot(1, timestamp, 0.0)
+    builder.PrependFloat64Slot(1, timestamp, 0.0)
 
 def PARAM_GlobalMsgAddScene(builder, scene):
     builder.PrependUOffsetTRelativeSlot(2, flatbuffers.number_types.UOffsetTFlags.py_type(scene), 0)
 
 def PARAM_GlobalMsgAddCmdReportOnce(builder, cmdReportOnce):
     builder.PrependInt32Slot(3, cmdReportOnce, 0)
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             return self._tab.String(o + self._tab.Pos)
         return None
 
     # PARAM_SimulationMsg
     def Timestamp(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+            return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
         return 0.0
 
     # PARAM_SimulationMsg
     def CmdReportOnce(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int32Flags, o + self._tab.Pos)
@@ -101,15 +101,15 @@
 def PARAM_SimulationMsgStart(builder):
     builder.StartObject(10)
 
 def PARAM_SimulationMsgAddName(builder, name):
     builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(name), 0)
 
 def PARAM_SimulationMsgAddTimestamp(builder, timestamp):
-    builder.PrependFloat32Slot(1, timestamp, 0.0)
+    builder.PrependFloat64Slot(1, timestamp, 0.0)
 
 def PARAM_SimulationMsgAddCmdReportOnce(builder, cmdReportOnce):
     builder.PrependInt32Slot(2, cmdReportOnce, 0)
 
 def PARAM_SimulationMsgAddCmdReset(builder, cmdReset):
     builder.PrependInt32Slot(3, cmdReset, 0)
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             return self._tab.String(o + self._tab.Pos)
         return None
 
     # PARAM_WebsocketMsg
     def Timestamp(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+            return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
         return 0.0
 
     # PARAM_WebsocketMsg
     def CmdReportOnce(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int32Flags, o + self._tab.Pos)
@@ -136,15 +136,15 @@
 def PARAM_WebsocketMsgStart(builder):
     builder.StartObject(15)
 
 def PARAM_WebsocketMsgAddName(builder, name):
     builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(name), 0)
 
 def PARAM_WebsocketMsgAddTimestamp(builder, timestamp):
-    builder.PrependFloat32Slot(1, timestamp, 0.0)
+    builder.PrependFloat64Slot(1, timestamp, 0.0)
 
 def PARAM_WebsocketMsgAddCmdReportOnce(builder, cmdReportOnce):
     builder.PrependInt32Slot(2, cmdReportOnce, 0)
 
 def PARAM_WebsocketMsgAddCmdConnect(builder, cmdConnect):
     builder.PrependInt32Slot(3, cmdConnect, 0)
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,230 +251,273 @@
     def Name(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         if o != 0:
             return self._tab.String(o + self._tab.Pos)
         return None
 
     # StatesMsg
-    def Timestamp(self):
+    def Id(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
-            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+            return self._tab.Get(flatbuffers.number_types.Int32Flags, o + self._tab.Pos)
+        return 0
+
+    # StatesMsg
+    def Timestamp(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float64Flags, o + self._tab.Pos)
         return 0.0
 
     # StatesMsg
     def LinAcc(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def LinVel(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def LinPos(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(14))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def AngAcc(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(14))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def AngVel(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(18))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def Euler(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(18))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(20))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def EulerDot(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(20))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(22))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def Quaternion(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(22))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec4Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def Pwm(self, j):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(26))
         if o != 0:
             a = self._tab.Vector(o)
-            return self._tab.Get(flatbuffers.number_types.Int16Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 2))
+            return self._tab.Get(flatbuffers.number_types.Uint32Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 4))
         return 0
 
     # StatesMsg
     def PwmAsNumpy(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(26))
         if o != 0:
-            return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Int16Flags, o)
+            return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Uint32Flags, o)
         return 0
 
     # StatesMsg
     def PwmLength(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(26))
         if o != 0:
             return self._tab.VectorLen(o)
         return 0
 
     # StatesMsg
     def PwmIsNone(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(26))
+        return o == 0
+
+    # StatesMsg
+    def Actuators(self, j):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(28))
+        if o != 0:
+            a = self._tab.Vector(o)
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 4))
+        return 0
+
+    # StatesMsg
+    def ActuatorsAsNumpy(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(28))
+        if o != 0:
+            return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Float32Flags, o)
+        return 0
+
+    # StatesMsg
+    def ActuatorsLength(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(28))
+        if o != 0:
+            return self._tab.VectorLen(o)
+        return 0
+
+    # StatesMsg
+    def ActuatorsIsNone(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(28))
         return o == 0
 
     # StatesMsg
     def Force(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(26))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(30))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def Torque(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(28))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(32))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def Accelerometer(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(30))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(34))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def Gyroscope(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(32))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(36))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
     # StatesMsg
     def Magnetometer(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(34))
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(38))
         if o != 0:
             x = self._tab.Indirect(o + self._tab.Pos)
             obj = Vec3Msg()
             obj.Init(self._tab.Bytes, x)
             return obj
         return None
 
 def StatesMsgStart(builder):
-    builder.StartObject(16)
+    builder.StartObject(18)
 
 def StatesMsgAddName(builder, name):
     builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(name), 0)
 
+def StatesMsgAddId(builder, id):
+    builder.PrependInt32Slot(1, id, 0)
+
 def StatesMsgAddTimestamp(builder, timestamp):
-    builder.PrependFloat32Slot(1, timestamp, 0.0)
+    builder.PrependFloat64Slot(2, timestamp, 0.0)
 
 def StatesMsgAddLinAcc(builder, linAcc):
-    builder.PrependUOffsetTRelativeSlot(2, flatbuffers.number_types.UOffsetTFlags.py_type(linAcc), 0)
+    builder.PrependUOffsetTRelativeSlot(3, flatbuffers.number_types.UOffsetTFlags.py_type(linAcc), 0)
 
 def StatesMsgAddLinVel(builder, linVel):
-    builder.PrependUOffsetTRelativeSlot(3, flatbuffers.number_types.UOffsetTFlags.py_type(linVel), 0)
+    builder.PrependUOffsetTRelativeSlot(4, flatbuffers.number_types.UOffsetTFlags.py_type(linVel), 0)
 
 def StatesMsgAddLinPos(builder, linPos):
-    builder.PrependUOffsetTRelativeSlot(4, flatbuffers.number_types.UOffsetTFlags.py_type(linPos), 0)
+    builder.PrependUOffsetTRelativeSlot(5, flatbuffers.number_types.UOffsetTFlags.py_type(linPos), 0)
 
 def StatesMsgAddAngAcc(builder, angAcc):
-    builder.PrependUOffsetTRelativeSlot(5, flatbuffers.number_types.UOffsetTFlags.py_type(angAcc), 0)
+    builder.PrependUOffsetTRelativeSlot(6, flatbuffers.number_types.UOffsetTFlags.py_type(angAcc), 0)
 
 def StatesMsgAddAngVel(builder, angVel):
-    builder.PrependUOffsetTRelativeSlot(6, flatbuffers.number_types.UOffsetTFlags.py_type(angVel), 0)
+    builder.PrependUOffsetTRelativeSlot(7, flatbuffers.number_types.UOffsetTFlags.py_type(angVel), 0)
 
 def StatesMsgAddEuler(builder, euler):
-    builder.PrependUOffsetTRelativeSlot(7, flatbuffers.number_types.UOffsetTFlags.py_type(euler), 0)
+    builder.PrependUOffsetTRelativeSlot(8, flatbuffers.number_types.UOffsetTFlags.py_type(euler), 0)
 
 def StatesMsgAddEulerDot(builder, eulerDot):
-    builder.PrependUOffsetTRelativeSlot(8, flatbuffers.number_types.UOffsetTFlags.py_type(eulerDot), 0)
+    builder.PrependUOffsetTRelativeSlot(9, flatbuffers.number_types.UOffsetTFlags.py_type(eulerDot), 0)
 
 def StatesMsgAddQuaternion(builder, quaternion):
-    builder.PrependUOffsetTRelativeSlot(9, flatbuffers.number_types.UOffsetTFlags.py_type(quaternion), 0)
+    builder.PrependUOffsetTRelativeSlot(10, flatbuffers.number_types.UOffsetTFlags.py_type(quaternion), 0)
 
 def StatesMsgAddPwm(builder, pwm):
-    builder.PrependUOffsetTRelativeSlot(10, flatbuffers.number_types.UOffsetTFlags.py_type(pwm), 0)
+    builder.PrependUOffsetTRelativeSlot(11, flatbuffers.number_types.UOffsetTFlags.py_type(pwm), 0)
 
 def StatesMsgStartPwmVector(builder, numElems):
-    return builder.StartVector(2, numElems, 2)
+    return builder.StartVector(4, numElems, 4)
+
+def StatesMsgAddActuators(builder, actuators):
+    builder.PrependUOffsetTRelativeSlot(12, flatbuffers.number_types.UOffsetTFlags.py_type(actuators), 0)
+
+def StatesMsgStartActuatorsVector(builder, numElems):
+    return builder.StartVector(4, numElems, 4)
 
 def StatesMsgAddForce(builder, force):
-    builder.PrependUOffsetTRelativeSlot(11, flatbuffers.number_types.UOffsetTFlags.py_type(force), 0)
+    builder.PrependUOffsetTRelativeSlot(13, flatbuffers.number_types.UOffsetTFlags.py_type(force), 0)
 
 def StatesMsgAddTorque(builder, torque):
-    builder.PrependUOffsetTRelativeSlot(12, flatbuffers.number_types.UOffsetTFlags.py_type(torque), 0)
+    builder.PrependUOffsetTRelativeSlot(14, flatbuffers.number_types.UOffsetTFlags.py_type(torque), 0)
 
 def StatesMsgAddAccelerometer(builder, accelerometer):
-    builder.PrependUOffsetTRelativeSlot(13, flatbuffers.number_types.UOffsetTFlags.py_type(accelerometer), 0)
+    builder.PrependUOffsetTRelativeSlot(15, flatbuffers.number_types.UOffsetTFlags.py_type(accelerometer), 0)
 
 def StatesMsgAddGyroscope(builder, gyroscope):
-    builder.PrependUOffsetTRelativeSlot(14, flatbuffers.number_types.UOffsetTFlags.py_type(gyroscope), 0)
+    builder.PrependUOffsetTRelativeSlot(16, flatbuffers.number_types.UOffsetTFlags.py_type(gyroscope), 0)
 
 def StatesMsgAddMagnetometer(builder, magnetometer):
-    builder.PrependUOffsetTRelativeSlot(15, flatbuffers.number_types.UOffsetTFlags.py_type(magnetometer), 0)
+    builder.PrependUOffsetTRelativeSlot(17, flatbuffers.number_types.UOffsetTFlags.py_type(magnetometer), 0)
 
 def StatesMsgEnd(builder):
     return builder.EndObject()
 
 
 try:
     from typing import List, Optional
@@ -482,24 +525,26 @@
     pass
 
 class StatesMsgT(object):
 
     # StatesMsgT
     def __init__(self):
         self.name = None  # type: str
+        self.id = 0  # type: int
         self.timestamp = 0.0  # type: float
         self.linAcc = None  # type: Optional[Vec3MsgT]
         self.linVel = None  # type: Optional[Vec3MsgT]
         self.linPos = None  # type: Optional[Vec3MsgT]
         self.angAcc = None  # type: Optional[Vec3MsgT]
         self.angVel = None  # type: Optional[Vec3MsgT]
         self.euler = None  # type: Optional[Vec3MsgT]
         self.eulerDot = None  # type: Optional[Vec3MsgT]
         self.quaternion = None  # type: Optional[Vec4MsgT]
         self.pwm = None  # type: List[int]
+        self.actuators = None  # type: List[float]
         self.force = None  # type: Optional[Vec3MsgT]
         self.torque = None  # type: Optional[Vec3MsgT]
         self.accelerometer = None  # type: Optional[Vec3MsgT]
         self.gyroscope = None  # type: Optional[Vec3MsgT]
         self.magnetometer = None  # type: Optional[Vec3MsgT]
 
     @classmethod
@@ -520,14 +565,15 @@
         return x
 
     # StatesMsgT
     def _UnPack(self, statesMsg):
         if statesMsg is None:
             return
         self.name = statesMsg.Name()
+        self.id = statesMsg.Id()
         self.timestamp = statesMsg.Timestamp()
         if statesMsg.LinAcc() is not None:
             self.linAcc = Vec3MsgT.InitFromObj(statesMsg.LinAcc())
         if statesMsg.LinVel() is not None:
             self.linVel = Vec3MsgT.InitFromObj(statesMsg.LinVel())
         if statesMsg.LinPos() is not None:
             self.linPos = Vec3MsgT.InitFromObj(statesMsg.LinPos())
@@ -544,14 +590,21 @@
         if not statesMsg.PwmIsNone():
             if np is None:
                 self.pwm = []
                 for i in range(statesMsg.PwmLength()):
                     self.pwm.append(statesMsg.Pwm(i))
             else:
                 self.pwm = statesMsg.PwmAsNumpy()
+        if not statesMsg.ActuatorsIsNone():
+            if np is None:
+                self.actuators = []
+                for i in range(statesMsg.ActuatorsLength()):
+                    self.actuators.append(statesMsg.Actuators(i))
+            else:
+                self.actuators = statesMsg.ActuatorsAsNumpy()
         if statesMsg.Force() is not None:
             self.force = Vec3MsgT.InitFromObj(statesMsg.Force())
         if statesMsg.Torque() is not None:
             self.torque = Vec3MsgT.InitFromObj(statesMsg.Torque())
         if statesMsg.Accelerometer() is not None:
             self.accelerometer = Vec3MsgT.InitFromObj(statesMsg.Accelerometer())
         if statesMsg.Gyroscope() is not None:
@@ -581,29 +634,38 @@
             quaternion = self.quaternion.Pack(builder)
         if self.pwm is not None:
             if np is not None and type(self.pwm) is np.ndarray:
                 pwm = builder.CreateNumpyVector(self.pwm)
             else:
                 StatesMsgStartPwmVector(builder, len(self.pwm))
                 for i in reversed(range(len(self.pwm))):
-                    builder.PrependInt16(self.pwm[i])
+                    builder.PrependUint32(self.pwm[i])
                 pwm = builder.EndVector()
+        if self.actuators is not None:
+            if np is not None and type(self.actuators) is np.ndarray:
+                actuators = builder.CreateNumpyVector(self.actuators)
+            else:
+                StatesMsgStartActuatorsVector(builder, len(self.actuators))
+                for i in reversed(range(len(self.actuators))):
+                    builder.PrependFloat32(self.actuators[i])
+                actuators = builder.EndVector()
         if self.force is not None:
             force = self.force.Pack(builder)
         if self.torque is not None:
             torque = self.torque.Pack(builder)
         if self.accelerometer is not None:
             accelerometer = self.accelerometer.Pack(builder)
         if self.gyroscope is not None:
             gyroscope = self.gyroscope.Pack(builder)
         if self.magnetometer is not None:
             magnetometer = self.magnetometer.Pack(builder)
         StatesMsgStart(builder)
         if self.name is not None:
             StatesMsgAddName(builder, name)
+        StatesMsgAddId(builder, self.id)
         StatesMsgAddTimestamp(builder, self.timestamp)
         if self.linAcc is not None:
             StatesMsgAddLinAcc(builder, linAcc)
         if self.linVel is not None:
             StatesMsgAddLinVel(builder, linVel)
         if self.linPos is not None:
             StatesMsgAddLinPos(builder, linPos)
@@ -615,14 +677,16 @@
             StatesMsgAddEuler(builder, euler)
         if self.eulerDot is not None:
             StatesMsgAddEulerDot(builder, eulerDot)
         if self.quaternion is not None:
             StatesMsgAddQuaternion(builder, quaternion)
         if self.pwm is not None:
             StatesMsgAddPwm(builder, pwm)
+        if self.actuators is not None:
+            StatesMsgAddActuators(builder, actuators)
         if self.force is not None:
             StatesMsgAddForce(builder, force)
         if self.torque is not None:
             StatesMsgAddTorque(builder, torque)
         if self.accelerometer is not None:
             StatesMsgAddAccelerometer(builder, accelerometer)
         if self.gyroscope is not None:
```

### Comparing `ubicoders-vrobots-0.2.7/src/ubicoders_vrobots.egg-info/SOURCES.txt` & `ubicoders-vrobots-0.2.8/src/ubicoders_vrobots.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,27 @@
 src/ubicoders_vrobots/vrobots_bridge/vr_rest_srv.py
 src/ubicoders_vrobots/vrobots_bridge/vr_ws_srv.py
 src/ubicoders_vrobots/vrobots_bridge/vrb_main.py
 src/ubicoders_vrobots/vrobots_bridge/ws_utils.py
 src/ubicoders_vrobots/vrobots_clients/__init__.py
 src/ubicoders_vrobots/vrobots_clients/clientutils.py
 src/ubicoders_vrobots/vrobots_clients/msg_helper.py
-src/ubicoders_vrobots/vrobots_clients/vrobots_general.py
+src/ubicoders_vrobots/vrobots_clients/service_client.py
 src/ubicoders_vrobots/vrobots_clients/vrobots_heli.py
 src/ubicoders_vrobots/vrobots_clients/vrobots_imu.py
 src/ubicoders_vrobots/vrobots_clients/vrobots_multirotor.py
+src/ubicoders_vrobots/vrobots_clients/vrobots_omrover.py
 src/ubicoders_vrobots/vrobots_msgs/__init__.py
 src/ubicoders_vrobots/vrobots_msgs/gen_all.py
+src/ubicoders_vrobots/vrobots_msgs/python/VROBOTS_CMDS.py
 src/ubicoders_vrobots/vrobots_msgs/python/__init__.py
 src/ubicoders_vrobots/vrobots_msgs/python/commands_generated.py
 src/ubicoders_vrobots/vrobots_msgs/python/empty_generated.py
 src/ubicoders_vrobots/vrobots_msgs/python/params_global_generated.py
 src/ubicoders_vrobots/vrobots_msgs/python/params_simulation_generated.py
 src/ubicoders_vrobots/vrobots_msgs/python/params_websocket_generated.py
+src/ubicoders_vrobots/vrobots_msgs/python/srv_imu_replay_generated.py
+src/ubicoders_vrobots/vrobots_msgs/python/srv_omr_walls_generated.py
+src/ubicoders_vrobots/vrobots_msgs/python/srv_params_global_generated.py
+src/ubicoders_vrobots/vrobots_msgs/python/srv_params_sim_generated.py
+src/ubicoders_vrobots/vrobots_msgs/python/srv_params_ws_generated.py
 src/ubicoders_vrobots/vrobots_msgs/python/states_generated.py
```

