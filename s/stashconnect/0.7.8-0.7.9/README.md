# Comparing `tmp/stashconnect-0.7.8.tar.gz` & `tmp/stashconnect-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.7.8.tar", last modified: Sat Jun  1 20:58:14 2024, max compression
+gzip compressed data, was "stashconnect-0.7.9.tar", last modified: Sat Jun  1 21:19:00 2024, max compression
```

## Comparing `stashconnect-0.7.8.tar` & `stashconnect-0.7.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 20:58:14.591062 stashconnect-0.7.8/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.8/LICENSE
--rw-rw-rw-   0        0        0     2263 2024-06-01 20:58:14.587032 stashconnect-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.7.8/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 20:58:14.591561 stashconnect-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:58:14.562144 stashconnect-0.7.8/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-06-01 20:55:59.000000 stashconnect-0.7.8/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.8/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.7.8/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.8/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.8/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.8/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    12585 2024-06-01 20:34:55.000000 stashconnect-0.7.8/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.8/stashconnect/messages.py
--rw-rw-rw-   0        0        0    18737 2024-06-01 20:56:20.000000 stashconnect-0.7.8/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.8/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.8/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.8/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-06-01 20:58:14.583516 stashconnect-0.7.8/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 21:19:00.010562 stashconnect-0.7.9/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-01 21:19:00.006055 stashconnect-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.7.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 21:19:00.011063 stashconnect-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:18:59.982459 stashconnect-0.7.9/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-01 21:18:08.000000 stashconnect-0.7.9/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.9/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.7.9/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.9/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.9/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.9/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    12868 2024-06-01 21:18:18.000000 stashconnect-0.7.9/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.9/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    18737 2024-06-01 20:56:20.000000 stashconnect-0.7.9/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.9/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.9/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.9/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:19:00.001012 stashconnect-0.7.9/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.7.8/LICENSE` & `stashconnect-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/PKG-INFO` & `stashconnect-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.8
+Version: 0.7.9
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

### Comparing `stashconnect-0.7.8/README.md` & `stashconnect-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/setup.py` & `stashconnect-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/channels.py` & `stashconnect-0.7.9/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/client.py` & `stashconnect-0.7.9/stashconnect/client.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/companies.py` & `stashconnect-0.7.9/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/conversations.py` & `stashconnect-0.7.9/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/crypto_utils.py` & `stashconnect-0.7.9/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/files.py` & `stashconnect-0.7.9/stashconnect/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             dict: The users quota.
         """
         response = self.client._post(
             "file/quota", data={"type": "personal", "type_id": self.client.user_id}
         )
         return response["quota"]
 
-    def upload(self, target: str | int, filepath: str, encrypted: bool = True) -> dict:
+    def upload(self, target: str | int, filepath: str, encrypted: bool = True) -> File:
         """Uploads a file to a target location
 
         Args:
             target (str | int): The upolads target id.
             filepath (str): The files location path.
             encrypted (bool, optional): Sets wether a file should be encrypted. Defaults to True.
 
@@ -134,15 +134,24 @@
 
             response = self.client._post("security/set_file_access_key", data=data)
 
         self.client.files.store_preview_image(file_id, filepath)
 
         return File(self.client, file)
 
-    def store_preview_image(self, file_id: str | int, filepath: str):
+    def store_preview_image(self, file_id: str | int, filepath: str) -> File | dict:
+        """Stores a preview image for a file
+
+        Args:
+            file_id (str | int): The files id.
+            filepath (str): The images file path.
+
+        Returns:
+            File | dict: A file object or a status: false dict.
+        """
         try:
             with Image.open(filepath) as image:
                 output_size = 100
 
                 image = image.convert("RGB")
                 min_dimension = min(image.width, image.height)
                 scale_factor = output_size / min_dimension
@@ -213,15 +222,15 @@
                 )
                 file.write(decrypted)
             else:
                 file.write(response.content)
 
         return file_path
 
-    def info(self, id: str | int) -> dict:
+    def info(self, id: str | int) -> File:
         """Fetches the info of a file
 
         Args:
             id (str | int): The files id.
 
         Returns:
             File: A file object.
@@ -280,15 +289,15 @@
         return response
 
     def copy(
         self,
         id: str | int,
         folder_id: str | int = 0,
         type_id: str | int = None,
-    ):
+    ) -> File:
         """Copies a file to a folder.
 
         Args:
             id (str | int): The files id.
             folder_id (str | int, optional): The new folders id. Defaults to main.
             type (str, optional): The destinations type. Defaults to "personal".
             type_id (str | int, optional): The destinations type id. Defaults to client.user_id.
```

### Comparing `stashconnect-0.7.8/stashconnect/messages.py` & `stashconnect-0.7.9/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/models.py` & `stashconnect-0.7.9/stashconnect/models.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/settings.py` & `stashconnect-0.7.9/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/tools.py` & `stashconnect-0.7.9/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect/users.py` & `stashconnect-0.7.9/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.8/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.7.9/stashconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.8
+Version: 0.7.9
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

