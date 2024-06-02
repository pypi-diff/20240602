# Comparing `tmp/stashconnect-0.8.5.tar.gz` & `tmp/stashconnect-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.8.5.tar", last modified: Sun Jun  2 10:43:55 2024, max compression
+gzip compressed data, was "stashconnect-0.8.6.tar", last modified: Sun Jun  2 11:33:38 2024, max compression
```

## Comparing `stashconnect-0.8.5.tar` & `stashconnect-0.8.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 10:43:55.087887 stashconnect-0.8.5/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.5/LICENSE
--rw-rw-rw-   0        0        0     2263 2024-06-02 10:43:55.084362 stashconnect-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.5/README.md
--rw-rw-rw-   0        0        0       42 2024-06-02 10:43:55.087887 stashconnect-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:43:55.058507 stashconnect-0.8.5/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-06-02 10:42:58.000000 stashconnect-0.8.5/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.8.5/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.5/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.5/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.5/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.5/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    13777 2024-06-02 09:49:16.000000 stashconnect-0.8.5/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.5/stashconnect/messages.py
--rw-rw-rw-   0        0        0    20337 2024-06-02 10:42:40.000000 stashconnect-0.8.5/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.5/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.5/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.5/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:43:55.081082 stashconnect-0.8.5/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-06-02 10:43:54.000000 stashconnect-0.8.5/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-06-02 10:43:54.000000 stashconnect-0.8.5/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 10:43:54.000000 stashconnect-0.8.5/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-06-02 10:43:54.000000 stashconnect-0.8.5/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-02 10:43:54.000000 stashconnect-0.8.5/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 11:33:38.893596 stashconnect-0.8.6/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-02 11:33:38.890097 stashconnect-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 11:33:38.894097 stashconnect-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:33:38.865167 stashconnect-0.8.6/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-02 11:33:06.000000 stashconnect-0.8.6/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.8.6/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.6/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.6/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.6/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.6/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    13777 2024-06-02 11:32:51.000000 stashconnect-0.8.6/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.6/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    20524 2024-06-02 11:32:50.000000 stashconnect-0.8.6/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.6/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.6/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.6/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:33:38.886074 stashconnect-0.8.6/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 11:33:38.000000 stashconnect-0.8.6/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.8.5/LICENSE` & `stashconnect-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/PKG-INFO` & `stashconnect-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.5
+Version: 0.8.6
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

### Comparing `stashconnect-0.8.5/README.md` & `stashconnect-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/setup.py` & `stashconnect-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/channels.py` & `stashconnect-0.8.6/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/client.py` & `stashconnect-0.8.6/stashconnect/client.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/companies.py` & `stashconnect-0.8.6/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/conversations.py` & `stashconnect-0.8.6/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/crypto_utils.py` & `stashconnect-0.8.6/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/files.py` & `stashconnect-0.8.6/stashconnect/files.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/messages.py` & `stashconnect-0.8.6/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/models.py` & `stashconnect-0.8.6/stashconnect/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,7 +659,15 @@
         Args:
             name (str): The files new name.
 
         Returns:
             dict: The success status
         """
         self.client.files.rename(self.id, name)
+
+    def shares(self) -> dict:
+        """Get a files shares
+
+        Returns:
+            dict: The files shares as a dict.
+        """
+        self.client.files.shares(self.id)
```

### Comparing `stashconnect-0.8.5/stashconnect/settings.py` & `stashconnect-0.8.6/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/tools.py` & `stashconnect-0.8.6/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect/users.py` & `stashconnect-0.8.6/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.5/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.8.6/stashconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.5
+Version: 0.8.6
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

