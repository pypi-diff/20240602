# Comparing `tmp/pythreadserver-0.1.6.tar.gz` & `tmp/pythreadserver-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythreadserver-0.1.6.tar", last modified: Fri May 24 17:36:43 2024, max compression
+gzip compressed data, was "pythreadserver-0.1.7.tar", last modified: Sun Jun  2 14:40:56 2024, max compression
```

## Comparing `pythreadserver-0.1.6.tar` & `pythreadserver-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 17:36:43.676557 pythreadserver-0.1.6/
--rw-rw-rw-   0        0        0      559 2024-05-24 17:36:43.671556 pythreadserver-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-22 18:26:53.000000 pythreadserver-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 17:36:43.636567 pythreadserver-0.1.6/pythreadserver/
--rw-rw-rw-   0        0        0       60 2024-05-22 16:58:32.000000 pythreadserver-0.1.6/pythreadserver/__init__.py
--rw-rw-rw-   0        0        0     4558 2024-05-22 17:46:29.000000 pythreadserver-0.1.6/pythreadserver/client.py
--rw-rw-rw-   0        0        0      115 2024-05-22 16:58:32.000000 pythreadserver-0.1.6/pythreadserver/constants.py
--rw-rw-rw-   0        0        0     6307 2024-05-22 17:51:46.000000 pythreadserver-0.1.6/pythreadserver/server.py
--rw-rw-rw-   0        0        0      555 2024-05-22 18:09:18.000000 pythreadserver-0.1.6/pythreadserver/textlog.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:36:43.667556 pythreadserver-0.1.6/pythreadserver.egg-info/
--rw-rw-rw-   0        0        0      559 2024-05-24 17:36:43.000000 pythreadserver-0.1.6/pythreadserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-05-24 17:36:43.000000 pythreadserver-0.1.6/pythreadserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 17:36:43.000000 pythreadserver-0.1.6/pythreadserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-24 17:36:43.000000 pythreadserver-0.1.6/pythreadserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 17:36:43.676557 pythreadserver-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-05-24 17:36:29.000000 pythreadserver-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:40:56.101050 pythreadserver-0.1.7/
+-rw-rw-rw-   0        0        0      559 2024-06-02 14:40:56.095997 pythreadserver-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-22 18:26:53.000000 pythreadserver-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 14:40:56.054486 pythreadserver-0.1.7/pythreadserver/
+-rw-rw-rw-   0        0        0       60 2024-05-22 16:58:32.000000 pythreadserver-0.1.7/pythreadserver/__init__.py
+-rw-rw-rw-   0        0        0     4574 2024-06-02 14:34:01.000000 pythreadserver-0.1.7/pythreadserver/client.py
+-rw-rw-rw-   0        0        0       61 2024-06-02 14:32:33.000000 pythreadserver-0.1.7/pythreadserver/constants.py
+-rw-rw-rw-   0        0        0     5795 2024-06-02 14:37:53.000000 pythreadserver-0.1.7/pythreadserver/server.py
+-rw-rw-rw-   0        0        0      555 2024-05-22 18:09:18.000000 pythreadserver-0.1.7/pythreadserver/textlog.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:40:56.089997 pythreadserver-0.1.7/pythreadserver.egg-info/
+-rw-rw-rw-   0        0        0      559 2024-06-02 14:40:55.000000 pythreadserver-0.1.7/pythreadserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-06-02 14:40:55.000000 pythreadserver-0.1.7/pythreadserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 14:40:55.000000 pythreadserver-0.1.7/pythreadserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-06-02 14:40:55.000000 pythreadserver-0.1.7/pythreadserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 14:40:56.101050 pythreadserver-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-06-02 14:40:40.000000 pythreadserver-0.1.7/setup.py
```

### Comparing `pythreadserver-0.1.6/PKG-INFO` & `pythreadserver-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.6
+Version: 0.1.7
 Summary: Socket-based server package
 Author: rain1107
 Author-email: ryanbays@icloud.com
 Keywords: python,socket,threading
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.6/pythreadserver/client.py` & `pythreadserver-0.1.7/pythreadserver/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,94 +15,90 @@
             log_path = kwargs["log_path"]
 
         self._recv_listeners = []
         self._connection_listeners = []
         self._disconnect_listeners = []
         self.packets = []
         self.log = Log(output_to_console, log_path)
-        self.socket_out = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.socket_in = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.socket= socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.send_loop_thread = None
         self.recv_loop_thread = None
         self.connected = False
         self.runtime = time.time()
 
     def connect(self, ip):
         if ip == "localhost":
             ip = socket.gethostname()
         self.log.log("Connecting to server...")
-        try:
-            self.socket_in.connect((ip, PORT_S_TO_C))
-            self.socket_out.connect((ip, PORT_C_TO_S))
-        except ConnectionRefusedError:
-            self.log.log("Error: Connection refused")
-            return 1
+        while True:
+            try:
+                self.socket.connect((ip, PORT))
+                break
+            except ConnectionRefusedError:
+                self.log.log("Error: Connection refused")
+                return 1
+            except OSError:
+                self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+
         self.log.log("Connected to server.")
         self.connected = True
         self.log.log("Initialising handling threads...")
         self.send_loop_thread = threading.Thread(target=self.send_loop)
         self.send_loop_thread.start()
         self.recv_loop_thread = threading.Thread(target=self.recv_loop)
         self.recv_loop_thread.start()
         self.log.log("Done.")
         for func in self._connection_listeners:
             try:
                 func()
-            except:
-                self.log.log(f"Error occurred in event handler: {func}")
+            except Exception as err:
+                self.log.log(f"{err}\nError occurred in event handler: {func}")
         return 0
 
     def send_loop(self):
         while self.connected:
             try:
-                self.send_server()
+                for packet in self.packets:
+                    self.socket.send(packet)
+                    self.packets = []
             except (ConnectionResetError, ConnectionAbortedError):
-                self.connected = False
+                self.close()
                 break
 
     def recv_loop(self):
         while self.connected:
             try:
-                self.recv_server()
+                data = self.socket.recv(BUFFER_SIZE)
+                if data == b'':
+                    self.close()
+                    return
+                for func in self._recv_listeners:
+                    try:
+                        func(data)
+                    except Exception as err:
+                        self.log.log(f"{err}\nError occurred in event handler: {func}")
             except (ConnectionResetError, ConnectionAbortedError):
                 self.close()
                 break
 
-    def send_server(self):
-        for packet in self.packets:
-            self.socket_out.send(packet)
-        self.packets = []
-
-    def recv_server(self):
-        data = self.socket_in.recv(BUFFER_SIZE)
-        if data == b'':
-            self.close()
-            return
-        for func in self._recv_listeners:
-            try:
-                func(data)
-            except:
-                self.log.log(f"Error occurred in event handler: {func}")
-
     def send(self, data: bytes):
         self.packets.append(data)
 
     def close(self):
         if not self.connected:
             return
         self.log.log("Closing connection...")
         self.connected = False
-        self.socket_in.close()
-        self.socket_out.close()
+        self.socket.close()
         self.log.log("Connection closed.")
         for func in self._disconnect_listeners:
             try:
                 func()
-            except:
-                self.log.log(f"Error occurred in event handler: {func}")
+            except Exception as err:
+                self.log.log(f"{err}\nError occurred in event handler: {func}")
         self.log.close()
 
 
     @property
     def on_receive(self):
         def wrapper(func):
             if func not in self._recv_listeners:
```

### Comparing `pythreadserver-0.1.6/pythreadserver/server.py` & `pythreadserver-0.1.7/pythreadserver/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import socket
 import time
 from .constants import *
 from .textlog import Log
 
 
 class ServerClient:
-    def __init__(self, parent, sock_from, sock_to, addr):
+    def __init__(self, parent, socket, addr):
         self.server = parent
         self.addr = addr
-        self.socket_to = sock_to
-        self.socket_from = sock_from
+        self.socket = socket
         self.connected = True
         self.packets = []
         self.send_loop_thread = None
         self.recv_loop_thread = None
 
     def run(self):
         self.send_loop_thread = threading.Thread(target=self.send_loop)
@@ -42,16 +41,15 @@
 
     def close(self):
         if not self.connected:
             return
         self.connected = False
         if self in self.server.clients:
             self.server.clients.remove(self)
-            self.socket_from.close()
-            self.socket_to.close()
+            self.socket.close()
             self.server.log.log(f"Connection from {self.addr[0]} closed.")
         for func in self.server._disconnect_listeners:
             try:
                 func(self)
             except:
                 self.server.log.log(f"Error occurred during event handler: {func}")
 
@@ -74,56 +72,51 @@
         self.clients = []
         self.threads = []
         self._recv_listeners = []
         self._connection_listeners = []
         self._disconnect_listeners = []
         self.log = Log(output_to_console, log_path)
 
-        self.socket_in = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.socket_out = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         host = ""
         self.log.log("Binding sockets to ports...")
-        self.socket_in.bind((host, PORT_C_TO_S))
-        self.socket_out.bind((host, PORT_S_TO_C))
+        self.socket.bind((host, PORT))
         self.log.log("Done.")
 
     def run(self):
         threading.Thread(target=self.input_check).start()
         self.log.log(f"Listening to connections...")
         try:
-            self.socket_in.listen()
-            self.socket_out.listen()
+            self.socket.listen()
             while self.running:
-                client_from, addr_from = self.socket_in.accept()
-                client_to, addr_to = self.socket_out.accept()
-                self.log.log(f"Handling connection from {addr_from[0]}.")
-                if addr_from[0] == addr_to[0]:
-                    client = ServerClient(self, sock_from=client_from, sock_to=client_to, addr=addr_to)
-                    self.clients.append(client)
-                    for func in self._connection_listeners:
-                        try:
-                            func(client)
-                        except: 
-                            self.log.log(f"Error occured in event handler: {func}")
-                    client.run()
+                client, addr = self.socket.accept()
+                self.log.log(f"Handling connection from {addr[0]}.")
+                client = ServerClient(self, socket=client, addr=addr)
+                self.clients.append(client)
+                for func in self._connection_listeners:
+                    try:
+                        func(client)
+                    except: 
+                        self.log.log(f"Error occured in event handler: {func}")
+                client.run()
         except OSError:
             self.log.log("Sockets closed.")
 
     def client_send(self, client: ServerClient):
         try:
             for packet in client.packets:
-                client.socket_to.send(packet)
+                client.socket.send(packet)
             client.packets = []
         except OSError:
             client.close()
             return
 
     def client_receive(self, client: ServerClient):
         try:
-            data = client.socket_from.recv(BUFFER_SIZE)
+            data = client.socket.recv(BUFFER_SIZE)
         except OSError:
             client.close()
             return
         if data == b'':
             client.close()
             return
         for func in self._recv_listeners:
@@ -139,16 +132,15 @@
     def get_clients(self):
         return self.clients.copy()
 
     def close(self):
         self.running = False
         for client in self.clients.copy():
             client.close()
-        self.socket_in.close()
-        self.socket_out.close()
+        self.socket.close()
         self.log.log("Server closed.")
         self.log.close()
 
     def input_check(self):
         while self.running:
             string = input("")
             if string.lower() == "exit":
```

### Comparing `pythreadserver-0.1.6/pythreadserver/textlog.py` & `pythreadserver-0.1.7/pythreadserver/textlog.py`

 * *Files identical despite different names*

### Comparing `pythreadserver-0.1.6/pythreadserver.egg-info/PKG-INFO` & `pythreadserver-0.1.7/pythreadserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.6
+Version: 0.1.7
 Summary: Socket-based server package
 Author: rain1107
 Author-email: ryanbays@icloud.com
 Keywords: python,socket,threading
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.6/setup.py` & `pythreadserver-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Socket-based server package'
 LONG_DESCRIPTION = 'https://github.com/rain-1107/pythreadserver'
 
 # Setting up
 setup(
     name="pythreadserver",
     version=VERSION,
```

