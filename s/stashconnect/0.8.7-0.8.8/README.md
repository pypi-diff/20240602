# Comparing `tmp/stashconnect-0.8.7.tar.gz` & `tmp/stashconnect-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.8.7.tar", last modified: Sun Jun  2 12:01:00 2024, max compression
+gzip compressed data, was "stashconnect-0.8.8.tar", last modified: Sun Jun  2 12:35:50 2024, max compression
```

## Comparing `stashconnect-0.8.7.tar` & `stashconnect-0.8.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 12:01:00.125031 stashconnect-0.8.7/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.7/LICENSE
--rw-rw-rw-   0        0        0     2263 2024-06-02 12:01:00.121531 stashconnect-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.7/README.md
--rw-rw-rw-   0        0        0       42 2024-06-02 12:01:00.125532 stashconnect-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:01:00.097523 stashconnect-0.8.7/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-06-02 11:58:50.000000 stashconnect-0.8.7/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.8.7/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.7/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.7/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.7/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.7/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    14069 2024-06-02 11:58:30.000000 stashconnect-0.8.7/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.7/stashconnect/messages.py
--rw-rw-rw-   0        0        0    20680 2024-06-02 11:58:33.000000 stashconnect-0.8.7/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.7/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.7/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.7/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:01:00.117524 stashconnect-0.8.7/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 12:35:50.920920 stashconnect-0.8.8/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-02 12:35:50.916420 stashconnect-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:35:50.920920 stashconnect-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:35:50.890826 stashconnect-0.8.8/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-02 12:35:29.000000 stashconnect-0.8.8/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17824 2024-06-02 12:35:25.000000 stashconnect-0.8.8/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.8/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.8/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.8/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.8/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    14069 2024-06-02 11:58:30.000000 stashconnect-0.8.8/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.8/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    20940 2024-06-02 12:35:15.000000 stashconnect-0.8.8/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.8/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.8/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.8/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:35:50.912391 stashconnect-0.8.8/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.8.7/LICENSE` & `stashconnect-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/PKG-INFO` & `stashconnect-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.7
+Version: 0.8.8
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

### Comparing `stashconnect-0.8.7/README.md` & `stashconnect-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/setup.py` & `stashconnect-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/channels.py` & `stashconnect-0.8.8/stashconnect/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,30 @@
         """
         response = self.client._post(
             "channels/editPassword",
             data={"password": password, "channel_id": channel_id},
         )
         return response
 
+    def _info(self, channel_id: int | str, without_members: bool = True) -> dict:
+        """Gets the info of a channel (dict)
+
+        Args:
+            channel_id (int | str): The channels id.
+            without_members (bool, optional): Returns the members. Defaults to True.
+
+        Returns:
+            dict: The channel info as a dict.
+        """
+        response = self.client._post(
+            "channels/info",
+            data={"channel_id": channel_id, "without_members": without_members},
+        )
+        return response["channels"]
+
     def info(self, channel_id: int | str, without_members: bool = True) -> Channel:
         """Gets the info of a channel
 
         Args:
             channel_id (int | str): The channels id.
             without_members (bool, optional): Returns the members. Defaults to True.
```

### Comparing `stashconnect-0.8.7/stashconnect/client.py` & `stashconnect-0.8.8/stashconnect/client.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/companies.py` & `stashconnect-0.8.8/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/conversations.py` & `stashconnect-0.8.8/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/crypto_utils.py` & `stashconnect-0.8.8/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/files.py` & `stashconnect-0.8.8/stashconnect/files.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/messages.py` & `stashconnect-0.8.8/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/models.py` & `stashconnect-0.8.8/stashconnect/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,18 +113,23 @@
 class User:
     def __init__(self, client, data) -> None:
         self.client = client
         self.id = data["id"]
 
         try:
             self.set_attributes(data)
+
         except KeyError:
             user_data = self.client.users._info(self.id)
             self.set_attributes(user_data)
 
+        except TypeError:
+            user_data = self.client.users._info(self.id)
+            self.set_attributes(user_data)
+
     def set_attributes(self, data):
         self.first_name = data["first_name"]
         self.last_name = data["last_name"]
 
         self.email = data["email"]
         self.status = data["status"]
         self.image = data["image"]
@@ -287,16 +292,21 @@
 class Channel:
     def __init__(self, client, data):
         self.client = client
         self.id = data["id"]
 
         try:
             self.set_attributes(data)
+
         except KeyError:
-            data = self.client.channels.info(self.id)
+            data = self.client.channels._info(self.id)
+            self.set_attributes(data)
+
+        except TypeError:
+            data = self.client.channels._info(self.id)
             self.set_attributes(data)
 
     def set_attributes(self, data):
         self.company = Company(self.client, {"company_id": data["company"]})
 
         self.crypto_properties = data["crypto_properties"]
         self.encrypted = data["encrypted"]
```

### Comparing `stashconnect-0.8.7/stashconnect/settings.py` & `stashconnect-0.8.8/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/tools.py` & `stashconnect-0.8.8/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect/users.py` & `stashconnect-0.8.8/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.7/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.8.8/stashconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.7
+Version: 0.8.8
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

