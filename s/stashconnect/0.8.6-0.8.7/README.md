# Comparing `tmp/stashconnect-0.8.6.tar.gz` & `tmp/stashconnect-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.8.6.tar", last modified: Sun Jun  2 11:33:38 2024, max compression
+gzip compressed data, was "stashconnect-0.8.7.tar", last modified: Sun Jun  2 12:01:00 2024, max compression
```

## Comparing `stashconnect-0.8.6.tar` & `stashconnect-0.8.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 11:33:38.893596 stashconnect-0.8.6/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.6/LICENSE
--rw-rw-rw-   0        0        0     2263 2024-06-02 11:33:38.890097 stashconnect-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.6/README.md
--rw-rw-rw-   0        0        0       42 2024-06-02 11:33:38.894097 stashconnect-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:33:38.865167 stashconnect-0.8.6/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-06-02 11:33:06.000000 stashconnect-0.8.6/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.8.6/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.6/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.6/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.6/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.6/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    13777 2024-06-02 11:32:51.000000 stashconnect-0.8.6/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.6/stashconnect/messages.py
--rw-rw-rw-   0        0        0    20524 2024-06-02 11:32:50.000000 stashconnect-0.8.6/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.6/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.6/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.6/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:33:38.886074 stashconnect-0.8.6/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 12:01:00.125031 stashconnect-0.8.7/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.7/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-02 12:01:00.121531 stashconnect-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:01:00.125532 stashconnect-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:01:00.097523 stashconnect-0.8.7/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-02 11:58:50.000000 stashconnect-0.8.7/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.8.7/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.7/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.7/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.7/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.7/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    14069 2024-06-02 11:58:30.000000 stashconnect-0.8.7/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.7/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    20680 2024-06-02 11:58:33.000000 stashconnect-0.8.7/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.7/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.7/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.7/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:01:00.117524 stashconnect-0.8.7/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 12:00:59.000000 stashconnect-0.8.7/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.8.6/LICENSE` & `stashconnect-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/PKG-INFO` & `stashconnect-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.6
+Version: 0.8.7
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

### Comparing `stashconnect-0.8.6/README.md` & `stashconnect-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/setup.py` & `stashconnect-0.8.7/setup.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/channels.py` & `stashconnect-0.8.7/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/client.py` & `stashconnect-0.8.7/stashconnect/client.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/companies.py` & `stashconnect-0.8.7/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/conversations.py` & `stashconnect-0.8.7/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/crypto_utils.py` & `stashconnect-0.8.7/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/files.py` & `stashconnect-0.8.7/stashconnect/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,28 +178,33 @@
 
             response = self.client._post("file/storePreviewImage", data=data)
             return File(self.client, response["file"])
 
         except Exception:
             return {"success": False}
 
-    def download(self, id: str | int, directory: str = "") -> str:
+    def download(self, id: str | int, directory: str = "", filename: str = None) -> str:
         """Downloads a file to a local location
 
         Args:
             id (str | int): The files id.
             directory (str, optional): The download dir. Defaults to main.
+            filename (str, optional): The new filename. Defaults to the main name.
 
         Returns:
             str: The path of the saved file.
         """
         response = self.client._post(f"file/download?id={id}", data={}, return_all=True)
 
-        file_info = self.client.files.file_info(id)
-        file_path = os.path.join(directory, file_info["name"])
+        if filename is None:
+            file_info = self.client.files._info(id)
+            file_path = os.path.join(directory, file_info["name"])
+        else:
+            file_info = self.client.files._info(id)
+            file_path = os.path.join(directory, filename + "." + file_info["ext"])
 
         with open(file_path, "wb") as file:
 
             if file_info["encrypted"]:
                 if self.client._private_key is None:
                     print(
                         "Could not download encrypted content as no encryption password was provided"
```

### Comparing `stashconnect-0.8.6/stashconnect/messages.py` & `stashconnect-0.8.7/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/models.py` & `stashconnect-0.8.7/stashconnect/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         else:
             self.content = self.content_encrypted
 
         self.timestamp = data["time"]
         self.channel_id = data["channel_id"]
         self.conversation_id = data["conversation_id"]
 
-        self.files = data["files"]
+        self.files = [File(self.client, file) for file in data["files"]]
+
         self.flagged = data["flagged"]
 
         self.liked = data["liked"]
         self.likes = data["likes"]
         self.links = data["links"]
 
         self._decrypt_location(data["location"])
@@ -619,24 +620,25 @@
             filepath (str): The images file path.
 
         Returns:
             File | dict: A file object or a status: false dict.
         """
         self.client.files.store_preview_image(self.id, filepath)
 
-    def download(self, directory: str = "") -> str:
+    def download(self, directory: str = "", filename: str = None) -> str:
         """Downloads a file to a local location
 
         Args:
             directory (str, optional): The download dir. Defaults to main.
+            filename (str, optional): The new filename. Defaults to the main name.
 
         Returns:
             str: The path of the saved file.
         """
-        self.client.files.download(self.id, directory)
+        self.client.files.download(self.id, directory, filename)
 
     def delete(self) -> dict:
         """Deletes specified files
 
         Returns:
             dict: The success status.
         """
```

### Comparing `stashconnect-0.8.6/stashconnect/settings.py` & `stashconnect-0.8.7/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/tools.py` & `stashconnect-0.8.7/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect/users.py` & `stashconnect-0.8.7/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.6/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.8.7/stashconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.6
+Version: 0.8.7
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

