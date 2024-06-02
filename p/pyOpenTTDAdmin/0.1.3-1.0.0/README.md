# Comparing `tmp/pyopenttdadmin-0.1.3.tar.gz` & `tmp/pyopenttdadmin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenttdadmin-0.1.3.tar", last modified: Tue May  7 09:57:43 2024, max compression
+gzip compressed data, was "pyopenttdadmin-1.0.0.tar", last modified: Sun Jun  2 01:19:40 2024, max compression
```

## Comparing `pyopenttdadmin-0.1.3.tar` & `pyopenttdadmin-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:43.755354 pyopenttdadmin-0.1.3/
--rw-rw-rw-   0        0        0     1085 2024-04-09 18:25:52.000000 pyopenttdadmin-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       61 2024-05-07 09:38:33.000000 pyopenttdadmin-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2291 2024-05-07 09:57:43.754358 pyopenttdadmin-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2014 2024-05-07 09:51:16.000000 pyopenttdadmin-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:43.753361 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/
--rw-rw-rw-   0        0        0     2291 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 09:57:43.000000 pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:43.751372 pyopenttdadmin-0.1.3/pyopenttdadmin/
--rw-rw-rw-   0        0        0       85 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/__init__.py
--rw-rw-rw-   0        0        0     3958 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/admin.py
--rw-rw-rw-   0        0        0     8561 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/enums.py
--rw-rw-rw-   0        0        0    12189 2024-05-07 09:48:02.000000 pyopenttdadmin-0.1.3/pyopenttdadmin/packet.py
--rw-rw-rw-   0        0        0       42 2024-05-07 09:57:43.755354 pyopenttdadmin-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-05-07 09:53:20.000000 pyopenttdadmin-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 01:19:40.100975 pyopenttdadmin-1.0.0/
+-rw-rw-rw-   0        0        0     1085 2024-04-09 18:25:52.000000 pyopenttdadmin-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-05-07 09:38:33.000000 pyopenttdadmin-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2291 2024-06-02 01:19:40.098732 pyopenttdadmin-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2014 2024-05-07 09:51:16.000000 pyopenttdadmin-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 01:19:40.080309 pyopenttdadmin-1.0.0/aiopyopenttdadmin/
+-rw-rw-rw-   0        0        0      112 2024-05-12 15:47:03.000000 pyopenttdadmin-1.0.0/aiopyopenttdadmin/__init__.py
+-rw-rw-rw-   0        0        0     7351 2024-06-02 01:18:18.000000 pyopenttdadmin-1.0.0/aiopyopenttdadmin/admin.py
+drwxrwxrwx   0        0        0        0 2024-06-02 01:19:40.097226 pyopenttdadmin-1.0.0/pyOpenTTDAdmin.egg-info/
+-rw-rw-rw-   0        0        0     2291 2024-06-02 01:19:40.000000 pyopenttdadmin-1.0.0/pyOpenTTDAdmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-06-02 01:19:40.000000 pyopenttdadmin-1.0.0/pyOpenTTDAdmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 01:19:40.000000 pyopenttdadmin-1.0.0/pyOpenTTDAdmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-06-02 01:19:40.000000 pyopenttdadmin-1.0.0/pyOpenTTDAdmin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 01:19:40.096218 pyopenttdadmin-1.0.0/pyopenttdadmin/
+-rw-rw-rw-   0        0        0       85 2024-05-07 09:48:02.000000 pyopenttdadmin-1.0.0/pyopenttdadmin/__init__.py
+-rw-rw-rw-   0        0        0     6200 2024-06-02 01:18:38.000000 pyopenttdadmin-1.0.0/pyopenttdadmin/admin.py
+-rw-rw-rw-   0        0        0     9004 2024-05-12 15:33:14.000000 pyopenttdadmin-1.0.0/pyopenttdadmin/enums.py
+-rw-rw-rw-   0        0        0    22180 2024-06-01 21:14:36.000000 pyopenttdadmin-1.0.0/pyopenttdadmin/packet.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 01:19:40.100975 pyopenttdadmin-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      526 2024-06-02 01:18:58.000000 pyopenttdadmin-1.0.0/setup.py
```

### Comparing `pyopenttdadmin-0.1.3/LICENSE` & `pyopenttdadmin-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenttdadmin-0.1.3/PKG-INFO` & `pyopenttdadmin-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pyOpenTTDAdmin
-Version: 0.1.3
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
```

### Comparing `pyopenttdadmin-0.1.3/README.md` & `pyopenttdadmin-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: pyOpenTTDAdmin
+Version: 1.0.0
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
```

### Comparing `pyopenttdadmin-0.1.3/pyOpenTTDAdmin.egg-info/PKG-INFO` & `pyopenttdadmin-1.0.0/pyOpenTTDAdmin.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyOpenTTDAdmin
-Version: 0.1.3
+Version: 1.0.0
 Summary: Python library to communicate with OpenTTD Admin port
 Home-page: https://github.com/liki-mc/pyOpenTTDAdmin/
 Author: liki-mc
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyopenttdadmin-0.1.3/pyopenttdadmin/enums.py` & `pyopenttdadmin-1.0.0/pyopenttdadmin/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,70 +40,94 @@
     SERVER_GAMESCRIPT = 0x7C      # The server gives the admin information from the GameScript in JSON.
     SERVER_RCON_END = 0x7D        # The server indicates that the remote console command has completed.
     SERVER_PONG = 0x7E            # The server replies to a ping request from the admin.
     SERVER_CMD_LOGGING = 0x7F     # The server gives the admin copies of incoming command packets.
     
     INVALID_ADMIN_PACKET = 0xFF   # An invalid marker for admin packets.
 
+class Actions(Enum):
+    JOIN = 0x00
+    LEAVE = 0x01
+    SERVER_MESSAGE = 0x02
+    CHAT = 0x03
+    CHAT_COMPANY = 0x04
+    CHAT_CLIENT = 0x05
+    GIVE_MONEY = 0x06
+    NAME_CHANGE = 0x07
+    COMPANY_SPECTATOR = 0x08
+    COMPANY_JOIN = 0x09
+    COMPANY_NEW = 0x0A
+
+class AdminCompanyRemoveReason(Enum):
+    """Reasons for removing a company - communicated to admins"""
+    ADMIN_CRR_MANUAL = 0x00    # The company is manually removed.
+    ADMIN_CRR_AUTOCLEAN = 0x01 # The company is removed due to autoclean.
+    ADMIN_CRR_BANKRUPT = 0x02  # The company went belly-up.
+    
+    ADMIN_CRR_END = 0x03       # Sentinel for end.
+
 class AdminStatus(Enum):
     """Status of an admin."""
     INACTIVE = 0x00 # The admin is not connected nor active.
     ACTIVE = 0x01   # The admin is active.
     END = 0x02      # Must ALWAYS be on the end of this list!! (period)
 
+class AdminUpdateFrequency(Enum):
+    """Update frequencies an admin can register."""
+    POLL = 0x01      # The admin can poll this.
+    DAILY = 0x02     # The admin gets information about this on a daily basis.
+    WEEKLY = 0x04    # The admin gets information about this on a weekly basis.
+    MONTHLY = 0x08   # The admin gets information about this on a monthly basis.
+    QUARTERLY = 0x10 # The admin gets information about this on a quarterly basis.
+    ANUALLY = 0x20   # The admin gets information about this on a yearly basis.
+    AUTOMATIC = 0x40 # The admin gets information about this when it changes.
+
 class AdminUpdateType(Enum):
     """Update types an admin can register a frequency for."""
     DATE = 0x00            # Updates about the date of the game.
     CLIENT_INFO = 0x01     # Updates about the information of clients.
     COMPANY_INFO = 0x02    # Updates about the generic information of companies.
     COMPANY_ECONOMY = 0x03 # Updates about the economy of companies.
     COMPANY_STATS = 0x04   # Updates about the statistics of companies.
     CHAT = 0x05            # The admin would like to have chat messages.
     CONSOLE = 0x06         # The admin would like to have console messages.
     CMD_NAMES = 0x07       # The admin would like a list of all DoCommand names.
     CMD_LOGGING = 0x08     # The admin would like to have DoCommand information.
     GAMESCRIPT = 0x09      # The admin would like to have gamescript messages.
     END = 0x0A             # Must ALWAYS be on the end of this list!! (period)
 
-class AdminUpdateFrequency(Enum):
-    """Update frequencies an admin can register."""
-    POLL = 0x01      # The admin can poll this.
-    DAILY = 0x02     # The admin gets information about this on a daily basis.
-    WEEKLY = 0x04    # The admin gets information about this on a weekly basis.
-    MONTHLY = 0x08   # The admin gets information about this on a monthly basis.
-    QUARTERLY = 0x10 # The admin gets information about this on a quarterly basis.
-    ANUALLY = 0x20   # The admin gets information about this on a yearly basis.
-    AUTOMATIC = 0x40 # The admin gets information about this when it changes.
-
-class AdminCompanyRemoveReason(Enum):
-    """Reasons for removing a company - communicated to admins"""
-    ADMIN_CRR_MANUAL = 0x00    # The company is manually removed.
-    ADMIN_CRR_AUTOCLEAN = 0x01 # The company is removed due to autoclean.
-    ADMIN_CRR_BANKRUPT = 0x02  # The company went belly-up.
-    
-    ADMIN_CRR_END = 0x03       # Sentinel for end.
-
-class Actions(Enum):
-    JOIN = 0x00
-    LEAVE = 0x01
-    SERVER_MESSAGE = 0x02
-    CHAT = 0x03
-    CHAT_COMPANY = 0x04
-    CHAT_CLIENT = 0x05
-    GIVE_MONEY = 0x06
-    NAME_CHANGE = 0x07
-    COMPANY_SPECTATOR = 0x08
-    COMPANY_JOIN = 0x09
-    COMPANY_NEW = 0x0A
-
 class ChatDestTypes(Enum):
     BROADCAST = 0x00
     TEAM = 0x01
     CLIENT = 0x02
 
+class Color(Enum):
+    DARK_BLUE = 0x00
+    PALE_GREEN = 0x01
+    PINK = 0x02
+    YELLOW = 0x03
+    RED = 0x04
+    LIGHT_BLUE = 0x05
+    GREEN = 0x06
+    DARK_GREEN = 0x07
+    BLUE = 0x08
+    CREAM = 0x09
+    MAUVE = 0x0A
+    PURPLE = 0x0B
+    ORANGE = 0x0C
+    BROWN = 0x0D
+    GREY = 0x0E
+    WHITE = 0x0F
+
+class Landscape(Enum):
+    TEMPERATE = 0x00
+    SUB_ARCTIC = 0x01
+    SUB_TROPICAL = 0x02
+    TOYLAND = 0x03
+
 class NetWorkErrorCodes(Enum):
     NETWORK_ERROR_GENERAL = 0x00 # Try to use this one like never
 
 	# Signals from clients 
     NETWORK_ERROR_DESYNC = 0x01
     NETWORK_ERROR_SAVEGAME_FAILED = 0x02
     NETWORK_ERROR_CONNECTION_LOST = 0x03
```

