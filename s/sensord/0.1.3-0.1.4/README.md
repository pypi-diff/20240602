# Comparing `tmp/sensord-0.1.3.tar.gz` & `tmp/sensord-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensord-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sensord-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sensord-0.1.3.tar` & `sensord-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3077 2024-05-24 11:02:51.867808 sensord-0.1.3/.gitignore
--rw-r--r--   0        0        0     1066 2024-05-24 10:59:38.675718 sensord-0.1.3/LICENSE
--rw-r--r--   0        0        0     4331 2024-05-31 06:33:58.675532 sensord-0.1.3/README.md
--rw-r--r--   0        0        0      468 2024-05-24 10:59:38.669051 sensord-0.1.3/doc/DEV.md
--rw-r--r--   0        0        0     1214 2024-05-24 10:59:38.669051 sensord-0.1.3/doc/presence-mqtt-schema.json
--rw-r--r--   0        0        0      170 2024-05-30 05:13:19.873371 sensord-0.1.3/examples/mqtt.toml
--rw-r--r--   0        0        0      594 2024-05-26 03:47:12.456778 sensord-0.1.3/examples/sensors.toml
--rw-r--r--   0        0        0      684 2024-05-27 14:40:24.982911 sensord-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      562 2024-05-31 05:54:32.401985 sensord-0.1.3/src/sensord/__init__.py
--rw-r--r--   0        0        0      586 2024-05-26 04:01:57.721386 sensord-0.1.3/src/sensord/cli/__init__.py
--rw-r--r--   0        0        0       66 2024-05-24 10:59:38.675718 sensord-0.1.3/src/sensord/cli/__main__.py
--rw-r--r--   0        0        0     3566 2024-05-28 03:32:22.269765 sensord-0.1.3/src/sensord/cli/client.py
--rw-r--r--   0        0        0     3793 2024-05-28 03:13:12.899985 sensord-0.1.3/src/sensord/cli/sen0395.py
--rw-r--r--   0        0        0      487 2024-05-26 03:44:40.753055 sensord-0.1.3/src/sensord/common/__init__.py
--rw-r--r--   0        0        0     5106 2024-05-26 03:47:12.466778 sensord-0.1.3/src/sensord/common/sen0395.py
--rw-r--r--   0        0        0     7658 2024-05-29 06:45:15.861306 sensord-0.1.3/src/sensord/common/socket.py
--rw-r--r--   0        0        0     4566 2024-05-31 06:27:47.877549 sensord-0.1.3/src/sensord/service/__init__.py
--rw-r--r--   0        0        0       71 2024-05-27 14:40:24.992911 sensord-0.1.3/src/sensord/service/__main__.py
--rw-r--r--   0        0        0     7350 2024-05-29 06:39:33.169337 sensord-0.1.3/src/sensord/service/api.py
--rw-r--r--   0        0        0      575 2024-05-29 06:30:57.726392 sensord-0.1.3/src/sensord/service/err.py
--rw-r--r--   0        0        0     2275 2024-05-27 03:23:21.208976 sensord-0.1.3/src/sensord/service/log.py
--rw-r--r--   0        0        0     2684 2024-05-31 06:21:42.749910 sensord-0.1.3/src/sensord/service/mqtt.py
--rw-r--r--   0        0        0     6060 2024-05-31 04:30:48.055698 sensord-0.1.3/src/sensord/service/paths.py
--rw-r--r--   0        0        0     2517 2024-05-26 04:14:33.109457 sensord-0.1.3/src/sensord/service/sen0395.py
--rw-r--r--   0        0        0     4825 1970-01-01 00:00:00.000000 sensord-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3077 2024-05-24 11:02:51.867808 sensord-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1066 2024-05-24 10:59:38.675718 sensord-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7142 2024-06-01 10:54:06.027094 sensord-0.1.4/README.md
+-rw-r--r--   0        0        0      468 2024-05-24 10:59:38.669051 sensord-0.1.4/doc/DEV.md
+-rw-r--r--   0        0        0     1214 2024-05-24 10:59:38.669051 sensord-0.1.4/doc/presence-mqtt-schema.json
+-rw-r--r--   0        0        0      170 2024-05-30 05:13:19.873371 sensord-0.1.4/examples/mqtt.toml
+-rw-r--r--   0        0        0      594 2024-05-26 03:47:12.456778 sensord-0.1.4/examples/sensors.toml
+-rw-r--r--   0        0        0      684 2024-05-27 14:40:24.982911 sensord-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      562 2024-06-02 02:38:42.477490 sensord-0.1.4/src/sensord/__init__.py
+-rw-r--r--   0        0        0      626 2024-06-01 09:54:18.705451 sensord-0.1.4/src/sensord/cli/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-24 10:59:38.675718 sensord-0.1.4/src/sensord/cli/__main__.py
+-rw-r--r--   0        0        0     3566 2024-05-28 03:32:22.269765 sensord-0.1.4/src/sensord/cli/client.py
+-rw-r--r--   0        0        0     5076 2024-06-01 12:16:38.778367 sensord-0.1.4/src/sensord/cli/sen0395.py
+-rw-r--r--   0        0        0      487 2024-05-26 03:44:40.753055 sensord-0.1.4/src/sensord/common/__init__.py
+-rw-r--r--   0        0        0     5106 2024-05-26 03:47:12.466778 sensord-0.1.4/src/sensord/common/sen0395.py
+-rw-r--r--   0        0        0     7885 2024-06-01 05:19:19.611327 sensord-0.1.4/src/sensord/common/socket.py
+-rw-r--r--   0        0        0     4872 2024-06-01 04:31:06.157193 sensord-0.1.4/src/sensord/service/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-27 14:40:24.992911 sensord-0.1.4/src/sensord/service/__main__.py
+-rw-r--r--   0        0        0     7350 2024-06-01 04:37:42.062242 sensord-0.1.4/src/sensord/service/api.py
+-rw-r--r--   0        0        0      575 2024-05-29 06:30:57.726392 sensord-0.1.4/src/sensord/service/err.py
+-rw-r--r--   0        0        0     2275 2024-05-27 03:23:21.208976 sensord-0.1.4/src/sensord/service/log.py
+-rw-r--r--   0        0        0     2684 2024-05-31 06:21:42.749910 sensord-0.1.4/src/sensord/service/mqtt.py
+-rw-r--r--   0        0        0     6060 2024-05-31 04:30:48.055698 sensord-0.1.4/src/sensord/service/paths.py
+-rw-r--r--   0        0        0     2517 2024-06-01 09:39:05.232120 sensord-0.1.4/src/sensord/service/sen0395.py
+-rw-r--r--   0        0        0     7636 1970-01-01 00:00:00.000000 sensord-0.1.4/PKG-INFO
```

### Comparing `sensord-0.1.3/.gitignore` & `sensord-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/LICENSE` & `sensord-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/doc/presence-mqtt-schema.json` & `sensord-0.1.4/doc/presence-mqtt-schema.json`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/examples/sensors.toml` & `sensord-0.1.4/examples/sensors.toml`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/pyproject.toml` & `sensord-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/__init__.py` & `sensord-0.1.4/src/sensord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 2. Sensor Control (sensorctl) CLI:
    - Provides a command-line tool for controlling and interacting with the Sensor Service.
    - Allows users to start, stop, configure, and monitor sensors through the command line.
    - Offers a convenient way to manage the Sensor Service and connected devices.
 
 """
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `sensord-0.1.3/src/sensord/cli/__init__.py` & `sensord-0.1.4/src/sensord/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
     pass
 
 
 @cli.group()
 def sen0395():
     """
-    Subcommands for SEN0395 sensor.
+    Subcommands for controlling the DFRobot mmWave presence sensor SEN0395.
     """
     pass
 
 
 sen0395.add_command(start)
 sen0395.add_command(stop)
 sen0395.add_command(reset)
```

### Comparing `sensord-0.1.3/src/sensord/cli/client.py` & `sensord-0.1.4/src/sensord/cli/client.py`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/cli/sen0395.py` & `sensord-0.1.4/src/sensord/cli/sen0395.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,95 +15,115 @@
     """
     Subcommand group for controlling the DFRobot mmWave presence sensor SEN0395.
     """
     pass
 
 
 @sen0395.command()
-def start():
-    send_command(Command.SENSOR_START)
+@click.option('--name', help='The name of the specific sensor to start scanning.')
+def start(name):
+    """Start scanning"""
+    send_command(Command.SENSOR_START, sensor_name=name)
 
 
 @sen0395.command()
-def stop():
-    send_command(Command.SENSOR_STOP)
+@click.option('--name', help='The name of the specific sensor to stop scanning.')
+def stop(name):
+    """Stop scanning"""
+    send_command(Command.SENSOR_STOP, sensor_name=name)
 
 
 @sen0395.command()
-def reset():
-    send_command(Command.RESET_SYSTEM)
+@click.option('--name', help='The name of the specific sensor to reset.')
+def reset(name):
+    """Send reset command"""
+    send_command(Command.RESET_SYSTEM, sensor_name=name)
 
 
 @sen0395.command()
 @click.argument('detection_delay', type=click.IntRange(0, 65535))
 @click.argument('disappearance_delay', type=click.IntRange(0, 65535))
-def latency(detection_delay, disappearance_delay):
+@click.option('--name', help='The name of the specific sensor to configure latency.')
+def latency(detection_delay, disappearance_delay, name):
+    """Configure detection and disappearance latencies"""
     delay_detection_ms = detection_delay * 25
     delay_disappearance_ms = disappearance_delay * 25
     console = Console()
     console.print(f"Delay on detection: {delay_detection_ms} ms, "
                   f"Delay after disappearance: {delay_disappearance_ms} ms")
 
-    send_command(Command.LATENCY_CONFIG, [-1, detection_delay, disappearance_delay])
+    send_command(Command.LATENCY_CONFIG, [-1, detection_delay, disappearance_delay], sensor_name=name)
 
 
 @sen0395.command()
 @click.argument('para_s', type=int)
 @click.argument('para_e', type=int)
 @click.argument('parb_s', type=int, required=False, default=None)
 @click.argument('parb_e', type=int, required=False, default=None)
 @click.argument('parc_s', type=int, required=False, default=None)
 @click.argument('parc_e', type=int, required=False, default=None)
 @click.argument('pard_s', type=int, required=False, default=None)
 @click.argument('pard_e', type=int, required=False, default=None)
-def detrange(para_s, para_e, parb_s, parb_e, parc_s, parc_e, pard_s, pard_e):
+@click.option('--name', help='The name of the specific sensor to configure detection range.')
+def detrange(para_s, para_e, parb_s, parb_e, parc_s, parc_e, pard_s, pard_e, name):
+    """Configure detection ranges"""
     params = [p for p in (para_s, para_e, parb_s, parb_e, parc_s, parc_e, pard_s, pard_e) if p is not None]
 
     try:
         segments = range_segments(params)
         console = Console()
         console.print("Sensing distance: " + " ".join(f'<{begin * 15}cm to {end * 15}cm>' for begin, end in segments))
     except ValueError as e:
         raise click.BadParameter(str(e))
 
-    send_command(Command.DETECTION_RANGE_CONFIG, [-1] + params)
+    send_command(Command.DETECTION_RANGE_CONFIG, [-1] + params, sensor_name=name)
+
 
 def service_call(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         console = Console()
         api_socket_path = paths.search_api_socket()
         if not api_socket_path:
             console.print("[bold red]Sensord service is not running:[/bold red] Start the service by `sensord` command")
             raise SystemExit(1)
 
         with APIClient(api_socket_path) as client:
             try:
                 return func(client, console, *args, **kwargs)
+            except PermissionError as e:
+                console.print(f"[bold red]Access Denied: [/bold red]{e}")
             except ServiceException as e:
                 console.print(f"[bold red]Service Error: [/bold red]{e}")
     return wrapper
 
 @sen0395.command()
+@click.option('--name', help='The name of the specific sensor to get the status.')
 @service_call
-def status(client: APIClient, console: Console):
-    statuses = client.send_get_status_sen0395()
+def status(client: APIClient, console: Console, name):
+    """Print status"""
+    statuses = client.send_get_status_sen0395(sensor_name=name)
     console.print(statuses)
 
 
 @sen0395.command()
+@click.option('--name', help='The name of the specific sensor to enable reading and processing.')
 @service_call
-def enable(client: APIClient, console: Console):
-    statuses = client.send_reading_enabled_sen0395(True)
+def enable(client: APIClient, console: Console, name):
+    """Start reading and processing data"""
+    statuses = client.send_reading_enabled_sen0395(True, sensor_name=name)
     console.print(statuses)
 
+
 @sen0395.command()
+@click.option('--name', help='The name of the specific sensor to disable reading and processing.')
 @service_call
-def disable(client: APIClient, console: Console):
-    statuses = client.send_reading_enabled_sen0395(False)
+def disable(client: APIClient, console: Console, name):
+    """Stop reading and processing data"""
+    statuses = client.send_reading_enabled_sen0395(False, sensor_name=name)
     console.print(statuses)
 
 
 @service_call
 def send_command(client: APIClient, console: Console, cmd, params=None, sensor_name=None):
     if cmd.is_config:
         responses = client.send_configure_sen0395(cmd, params, sensor_name)
```

### Comparing `sensord-0.1.3/src/sensord/common/sen0395.py` & `sensord-0.1.4/src/sensord/common/sen0395.py`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/common/socket.py` & `sensord-0.1.4/src/sensord/common/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 import logging
 import os
 import socket
+import stat
 from dataclasses import dataclass
 from enum import Enum, auto
 from pathlib import Path
 from threading import Thread, RLock
 from types import coroutine
 from typing import List, NamedTuple, Optional
 
@@ -54,23 +55,25 @@
             raise SocketServerStoppedAlready
 
         self._server = socket.socket(socket.AF_UNIX, socket.SOCK_DGRAM)
         try:
             self._server.bind(str(self._socket_path))
         except (PermissionError, OSError) as e:
             raise SocketBindException(self._socket_path) from e
-
+        # Allow users from the same group to communicate with the server
+        os.chmod(self._socket_path, stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IWGRP)
 
     def start(self):
         with self._lock:
             self._bind_socket()
             self._serving_thread.start()
 
     def wait(self):
-        self._serving_thread.join()
+        if self._serving_thread.is_alive():
+            self._serving_thread.join()
 
     def serve(self):
         with self._lock:
             self._bind_socket()
         self._serve()
 
     def _serve(self):
```

### Comparing `sensord-0.1.3/src/sensord/service/__init__.py` & `sensord-0.1.4/src/sensord/service/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,18 +45,23 @@
 
 def run():
     logger.info('[service_started]')
     try:
         api.start()
     except SocketBindException as e:
         logger.error(f"[socket_bind_error] reason=[{e}] check=[Is the service already running?]")
-        print(f"You can try removing `/tmp/{paths.API_SOCKET}` if you are absolutely sure the service is not running.")
+        print(f"You can try removing `{paths.API_SOCKET}` if you are absolutely sure the service is not running.")
         exit(1)
     except ServiceAlreadyRunning:
-        logger.warning(f"[service_is_already_running] result=[exiting..]")
+        logger.warning("[service_is_already_running] result=[exiting]")
+        exit(1)
+    except PermissionError as e:
+        logger.warning(f"[socket_permission_error] detail=[{e}] result=[exiting]")
+        print("The service runs restricted under different user. "
+              f"You can try removing `{paths.API_SOCKET}` if you are absolutely sure the service is not running.")
         exit(1)
 
     init_mqtt()
     init_sensors()
 
     signal.signal(signal.SIGTERM, signal_shutdown)
     signal.signal(signal.SIGINT, signal_shutdown)
```

### Comparing `sensord-0.1.3/src/sensord/service/api.py` & `sensord-0.1.4/src/sensord/service/api.py`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/service/err.py` & `sensord-0.1.4/src/sensord/service/err.py`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/service/log.py` & `sensord-0.1.4/src/sensord/service/log.py`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/service/mqtt.py` & `sensord-0.1.4/src/sensord/service/mqtt.py`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/service/paths.py` & `sensord-0.1.4/src/sensord/service/paths.py`

 * *Files identical despite different names*

### Comparing `sensord-0.1.3/src/sensord/service/sen0395.py` & `sensord-0.1.4/src/sensord/service/sen0395.py`

 * *Files identical despite different names*

