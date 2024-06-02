# Comparing `tmp/pyopenttdadmin-0.1.2.tar.gz` & `tmp/pyopenttdadmin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenttdadmin-0.1.2.tar", last modified: Tue May  7 09:19:46 2024, max compression
+gzip compressed data, was "pyopenttdadmin-0.1.3.tar", last modified: Tue May  7 09:57:43 2024, max compression
```

## Comparing `pyopenttdadmin-0.1.2.tar` & `pyopenttdadmin-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:19:46.826830 pyopenttdadmin-0.1.2/
--rw-rw-rw-   0        0        0     1085 2024-04-09 18:25:52.000000 pyopenttdadmin-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       61 2024-05-06 22:23:47.000000 pyopenttdadmin-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2313 2024-05-07 09:19:46.825828 pyopenttdadmin-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2024-05-06 22:23:47.000000 pyopenttdadmin-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:19:46.824271 pyopenttdadmin-0.1.2/pyOpenTTDAdmin.egg-info/
--rw-rw-rw-   0        0        0     2313 2024-05-07 09:19:46.000000 pyopenttdadmin-0.1.2/pyOpenTTDAdmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-07 09:19:46.000000 pyopenttdadmin-0.1.2/pyOpenTTDAdmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:19:46.000000 pyopenttdadmin-0.1.2/pyOpenTTDAdmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 09:19:46.000000 pyopenttdadmin-0.1.2/pyOpenTTDAdmin.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 09:19:46.821278 pyopenttdadmin-0.1.2/pyopenttdadmin/
--rw-rw-rw-   0        0        0       85 2024-05-07 09:16:04.000000 pyopenttdadmin-0.1.2/pyopenttdadmin/__init__.py
--rw-rw-rw-   0        0        0     3958 2024-04-09 18:25:52.000000 pyopenttdadmin-0.1.2/pyopenttdadmin/admin.py
--rw-rw-rw-   0        0        0     8561 2024-04-09 18:25:52.000000 pyopenttdadmin-0.1.2/pyopenttdadmin/enums.py
--rw-rw-rw-   0        0        0    12189 2024-04-09 18:25:52.000000 pyopenttdadmin-0.1.2/pyopenttdadmin/packet.py
--rw-rw-rw-   0        0        0       42 2024-05-07 09:19:46.827844 pyopenttdadmin-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-05-07 09:18:45.000000 pyopenttdadmin-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 09:57:43.755354 pyopenttdadmin-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2024-04-09 18:25:52.000000 pyopenttdadmin-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-05-07 09:38:33.000000 pyopenttdadmin-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2291 2024-05-07 09:57:43.754358 pyopenttdadmin-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2014 2024-05-07 09:51:16.000000 pyopenttdadmin-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 09:57:43.753361 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/
+-rw-rw-rw-   0        0        0     2291 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 09:57:43.751372 pyopenttdadmin-0.1.3/pyopenttdadmin/
+-rw-rw-rw-   0        0        0       85 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/__init__.py
+-rw-rw-rw-   0        0        0     3958 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/admin.py
+-rw-rw-rw-   0        0        0     8561 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/enums.py
+-rw-rw-rw-   0        0        0    12189 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/packet.py
+-rw-rw-rw-   0        0        0       42 2024-05-07 09:57:43.755354 pyopenttdadmin-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-07 09:53:20.000000 pyopenttdadmin-0.1.3/setup.py
```

### Comparing `pyopenttdadmin-0.1.2/LICENSE` & `pyopenttdadmin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenttdadmin-0.1.2/PKG-INFO` & `pyopenttdadmin-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyOpenTTDAdmin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library to communicate with OpenTTD Admin port
 Home-page: https://github.com/liki-mc/pyOpenTTDAdmin/
 Author: liki-mc
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -24,26 +24,24 @@
 
 
 ## Usage
 Example code for an echo bot can be found here:
 ```python
 import os
 
-from src.main import Admin
-from src.packet import ChatPacket
-from src.enums import Actions, ChatDestTypes, AdminUpdateType
+from pyopenttdadmin import Admin, Actions, ChatDestTypes, AdminUpdateType, openttdpacket
 
 PASSWORD = os.getenv('OPENTTD_ADMIN_PASSWORD')
 if PASSWORD is None:
     raise ValueError('OPENTTD_ADMIN_PASSWORD environment variable is not set')
 
 
 class App(Admin):
     def on_packet(self, packet):
-        if isinstance(packet, ChatPacket):
+        if isinstance(packet, openttdpacket.ChatPacket):
             print("ChatPacket")
             if packet.action == Actions.CHAT:
                 if packet.desttype == ChatDestTypes.BROADCAST:
                     self.send_global(packet.message)
 
 with App(password = PASSWORD) as admin:
     admin.send_subscribe(AdminUpdateType.CHAT)
```

### Comparing `pyopenttdadmin-0.1.2/README.md` & `pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: pyOpenTTDAdmin
+Version: 0.1.3
+Summary: Python library to communicate with OpenTTD Admin port
+Home-page: https://github.com/liki-mc/pyOpenTTDAdmin/
+Author: liki-mc
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyOpenTTDAdmin
 
 pyOpenTTDAdmin is a Python library designed to facilitate communication with OpenTTD's Admin port. OpenTTD (Open Transport Tycoon Deluxe) is an open-source simulation game where players manage a transport company.
 
 This library enables developers to interact with an OpenTTD server programmatically, allowing them to perform various administrative tasks and receive real-time updates from the game server.
 
 ## Features
@@ -14,26 +24,24 @@
 
 
 ## Usage
 Example code for an echo bot can be found here:
 ```python
 import os
 
-from src.main import Admin
-from src.packet import ChatPacket
-from src.enums import Actions, ChatDestTypes, AdminUpdateType
+from pyopenttdadmin import Admin, Actions, ChatDestTypes, AdminUpdateType, openttdpacket
 
 PASSWORD = os.getenv('OPENTTD_ADMIN_PASSWORD')
 if PASSWORD is None:
     raise ValueError('OPENTTD_ADMIN_PASSWORD environment variable is not set')
 
 
 class App(Admin):
     def on_packet(self, packet):
-        if isinstance(packet, ChatPacket):
+        if isinstance(packet, openttdpacket.ChatPacket):
             print("ChatPacket")
             if packet.action == Actions.CHAT:
                 if packet.desttype == ChatDestTypes.BROADCAST:
                     self.send_global(packet.message)
 
 with App(password = PASSWORD) as admin:
     admin.send_subscribe(AdminUpdateType.CHAT)
```

### Comparing `pyopenttdadmin-0.1.2/pyOpenTTDAdmin.egg-info/PKG-INFO` & `pyopenttdadmin-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pyOpenTTDAdmin
-Version: 0.1.2
-Summary: Python library to communicate with OpenTTD Admin port
-Home-page: https://github.com/liki-mc/pyOpenTTDAdmin/
-Author: liki-mc
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyOpenTTDAdmin
 
 pyOpenTTDAdmin is a Python library designed to facilitate communication with OpenTTD's Admin port. OpenTTD (Open Transport Tycoon Deluxe) is an open-source simulation game where players manage a transport company.
 
 This library enables developers to interact with an OpenTTD server programmatically, allowing them to perform various administrative tasks and receive real-time updates from the game server.
 
 ## Features
@@ -24,26 +14,24 @@
 
 
 ## Usage
 Example code for an echo bot can be found here:
 ```python
 import os
 
-from src.main import Admin
-from src.packet import ChatPacket
-from src.enums import Actions, ChatDestTypes, AdminUpdateType
+from pyopenttdadmin import Admin, Actions, ChatDestTypes, AdminUpdateType, openttdpacket
 
 PASSWORD = os.getenv('OPENTTD_ADMIN_PASSWORD')
 if PASSWORD is None:
     raise ValueError('OPENTTD_ADMIN_PASSWORD environment variable is not set')
 
 
 class App(Admin):
     def on_packet(self, packet):
-        if isinstance(packet, ChatPacket):
+        if isinstance(packet, openttdpacket.ChatPacket):
             print("ChatPacket")
             if packet.action == Actions.CHAT:
                 if packet.desttype == ChatDestTypes.BROADCAST:
                     self.send_global(packet.message)
 
 with App(password = PASSWORD) as admin:
     admin.send_subscribe(AdminUpdateType.CHAT)
```

### Comparing `pyopenttdadmin-0.1.2/pyopenttdadmin/admin.py` & `pyopenttdadmin-0.1.3/pyopenttdadmin/admin.py`

 * *Files identical despite different names*

### Comparing `pyopenttdadmin-0.1.2/pyopenttdadmin/enums.py` & `pyopenttdadmin-0.1.3/pyopenttdadmin/enums.py`

 * *Files identical despite different names*

### Comparing `pyopenttdadmin-0.1.2/pyopenttdadmin/packet.py` & `pyopenttdadmin-0.1.3/pyopenttdadmin/packet.py`

 * *Files identical despite different names*

