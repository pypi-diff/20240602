# Comparing `tmp/stashconnect-0.8.8.tar.gz` & `tmp/stashconnect-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.8.8.tar", last modified: Sun Jun  2 12:35:50 2024, max compression
+gzip compressed data, was "stashconnect-0.8.9.tar", last modified: Sun Jun  2 12:57:52 2024, max compression
```

## Comparing `stashconnect-0.8.8.tar` & `stashconnect-0.8.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 12:35:50.920920 stashconnect-0.8.8/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.8/LICENSE
--rw-rw-rw-   0        0        0     2263 2024-06-02 12:35:50.916420 stashconnect-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.8/README.md
--rw-rw-rw-   0        0        0       42 2024-06-02 12:35:50.920920 stashconnect-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:35:50.890826 stashconnect-0.8.8/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-06-02 12:35:29.000000 stashconnect-0.8.8/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17824 2024-06-02 12:35:25.000000 stashconnect-0.8.8/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.8/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.8/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.8.8/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.8/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    14069 2024-06-02 11:58:30.000000 stashconnect-0.8.8/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.8/stashconnect/messages.py
--rw-rw-rw-   0        0        0    20940 2024-06-02 12:35:15.000000 stashconnect-0.8.8/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.8/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.8/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.8/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:35:50.912391 stashconnect-0.8.8/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-02 12:35:50.000000 stashconnect-0.8.8/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 12:57:52.861282 stashconnect-0.8.9/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-02 12:57:52.857771 stashconnect-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.8.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:57:52.862287 stashconnect-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:57:52.833834 stashconnect-0.8.9/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-02 12:56:42.000000 stashconnect-0.8.9/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17824 2024-06-02 12:35:25.000000 stashconnect-0.8.9/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.8.9/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.8.9/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     5822 2024-06-02 12:55:36.000000 stashconnect-0.8.9/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.8.9/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    14069 2024-06-02 11:58:30.000000 stashconnect-0.8.9/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.8.9/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    20940 2024-06-02 12:35:15.000000 stashconnect-0.8.9/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.8.9/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.8.9/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.8.9/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:57:52.854965 stashconnect-0.8.9/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-02 12:57:52.000000 stashconnect-0.8.9/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-02 12:57:52.000000 stashconnect-0.8.9/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:57:52.000000 stashconnect-0.8.9/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-02 12:57:52.000000 stashconnect-0.8.9/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 12:57:52.000000 stashconnect-0.8.9/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.8.8/LICENSE` & `stashconnect-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/PKG-INFO` & `stashconnect-0.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.8
+Version: 0.8.9
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

### Comparing `stashconnect-0.8.8/README.md` & `stashconnect-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/setup.py` & `stashconnect-0.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/channels.py` & `stashconnect-0.8.9/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/client.py` & `stashconnect-0.8.9/stashconnect/client.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/companies.py` & `stashconnect-0.8.9/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/crypto_utils.py` & `stashconnect-0.8.9/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/files.py` & `stashconnect-0.8.9/stashconnect/files.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/messages.py` & `stashconnect-0.8.9/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/models.py` & `stashconnect-0.8.9/stashconnect/models.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/settings.py` & `stashconnect-0.8.9/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/tools.py` & `stashconnect-0.8.9/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect/users.py` & `stashconnect-0.8.9/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.8.8/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.8.9/stashconnect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.8.8
+Version: 0.8.9
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

