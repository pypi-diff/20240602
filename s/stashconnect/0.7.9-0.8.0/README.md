# Comparing `tmp/stashconnect-0.7.9.tar.gz` & `tmp/stashconnect-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.7.9.tar", last modified: Sat Jun  1 21:19:00 2024, max compression
+gzip compressed data, was "stashconnect-0.8.0.tar", last modified: Sun Jun  2 09:53:08 2024, max compression
```

## Comparing `stashconnect-0.7.9.tar` & `stashconnect-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:19:00.010562 stashconnect-0.7.9/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.9/LICENSE
--rw-rw-rw-   0        0        0     2263 2024-06-01 21:19:00.006055 stashconnect-0.7.9/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.7.9/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 21:19:00.011063 stashconnect-0.7.9/setup.cfg
--rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 21:18:59.982459 stashconnect-0.7.9/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-06-01 21:18:08.000000 stashconnect-0.7.9/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.9/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.7.9/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.9/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.9/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.9/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    12868 2024-06-01 21:18:18.000000 stashconnect-0.7.9/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.9/stashconnect/messages.py
--rw-rw-rw-   0        0        0    18737 2024-06-01 20:56:20.000000 stashconnect-0.7.9/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.9/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.9/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.9/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-06-01 21:19:00.001012 stashconnect-0.7.9/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 21:18:59.000000 stashconnect-0.7.9/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 09:53:08.811160 stashconnect-0.8.0/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-02 09:53:08.806659 stashconnect-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 09:53:08.811659 stashconnect-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 09:53:08.782442 stashconnect-0.8.0/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-02 09:52:17.000000 stashconnect-0.8.0/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.8.0/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.0/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.0/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.0/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.0/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    13777 2024-06-02 09:49:16.000000 stashconnect-0.8.0/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.0/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    18942 2024-06-02 09:49:45.000000 stashconnect-0.8.0/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.0/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.0/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.0/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-02 09:53:08.803660 stashconnect-0.8.0/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-02 09:53:08.000000 stashconnect-0.8.0/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-02 09:53:08.000000 stashconnect-0.8.0/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 09:53:08.000000 stashconnect-0.8.0/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-02 09:53:08.000000 stashconnect-0.8.0/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 09:53:08.000000 stashconnect-0.8.0/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.7.9/LICENSE` & `stashconnect-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/PKG-INFO` & `stashconnect-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.9
+Version: 0.8.0
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

### Comparing `stashconnect-0.7.9/README.md` & `stashconnect-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/setup.py` & `stashconnect-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/channels.py` & `stashconnect-0.8.0/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/client.py` & `stashconnect-0.8.0/stashconnect/client.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/companies.py` & `stashconnect-0.8.0/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/conversations.py` & `stashconnect-0.8.0/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/crypto_utils.py` & `stashconnect-0.8.0/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/files.py` & `stashconnect-0.8.0/stashconnect/files.py`

 * *Files 7% similar despite different names*

```diff
@@ -222,26 +222,61 @@
                 )
                 file.write(decrypted)
             else:
                 file.write(response.content)
 
         return file_path
 
+    def _info(self, id: str | int) -> dict:
+        """Fetches the info of a file (dict)
+
+        Args:
+            id (str | int): The files id.
+
+        Returns:
+            dict: The files dict.
+        """
+        response = self.client._post("file/info", data={"file_id": id})
+        return response["file"]
+
     def info(self, id: str | int) -> File:
         """Fetches the info of a file
 
         Args:
             id (str | int): The files id.
 
         Returns:
             File: A file object.
         """
         response = self.client._post("file/info", data={"file_id": id})
         return File(self.client, response["file"])
 
+    def infos(self, ids: str | int | list) -> list:
+        """Fetches mutliple files
+
+        Args:
+            ids (str | int | list): The files ids.
+
+        Returns:
+            list: A list of files.
+        """
+        ids_sent = []
+
+        if isinstance(ids, str | int):
+            ids_sent = [ids]
+        else:
+            ids_sent = ids
+
+        response = self.client._post(
+            "file/infos", data={"file_ids": json.dumps(ids_sent)}
+        )
+
+        files = [File(self.client, file) for file in response["files"]]
+        return files
+
     def delete(self, ids: str | int | list) -> dict:
         """Deletes specified files
 
         Args:
             ids (str | int | list): The file or files ids
 
         Returns:
```

### Comparing `stashconnect-0.7.9/stashconnect/messages.py` & `stashconnect-0.8.0/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/models.py` & `stashconnect-0.8.0/stashconnect/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -560,16 +560,23 @@
 class File:
     def __init__(self, client, data):
         self.client = client
         self.id = data["id"]
 
         try:
             self.set_attributes(data)
+
+        # happens when key is missing
         except KeyError:
-            data = self.client.files.info(self.id)
+            data = self.client.files._info(self.id)
+            self.set_attributes(data)
+
+        # happens when no owner is found
+        except TypeError:
+            data = self.client.files._info(self.id)
             self.set_attributes(data)
 
     def set_attributes(self, data):
         self.name = data["name"]
 
         self.virtual_folder = data["virtual_folder"]
         self.folder_type = data["folder_type"]
```

### Comparing `stashconnect-0.7.9/stashconnect/settings.py` & `stashconnect-0.8.0/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/tools.py` & `stashconnect-0.8.0/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect/users.py` & `stashconnect-0.8.0/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.9/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.8.0/stashconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.9
+Version: 0.8.0
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

