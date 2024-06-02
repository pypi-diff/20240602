# Comparing `tmp/shuttleai-4.0.0.tar.gz` & `tmp/shuttleai-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-4.0.0.tar", max compression
+gzip compressed data, was "shuttleai-4.0.1.tar", max compression
```

## Comparing `shuttleai-4.0.0.tar` & `shuttleai-4.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1154 2024-06-02 04:27:26.093048 shuttleai-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       33 2024-06-02 04:27:14.656264 shuttleai-4.0.0/README.md
--rw-r--r--   0        0        0      167 2024-06-02 04:26:47.729775 shuttleai-4.0.0/shuttleai/__init__.py
--rw-r--r--   0        0        0      824 2024-06-02 00:32:35.919932 shuttleai-4.0.0/shuttleai/_patch.py
--rw-r--r--   0        0        0       76 2024-06-02 02:18:27.148187 shuttleai-4.0.0/shuttleai/client/__init__.py
--rw-r--r--   0        0        0     6648 2024-06-02 04:04:56.617130 shuttleai-4.0.0/shuttleai/client/_async.py
--rw-r--r--   0        0        0     6689 2024-06-02 04:06:06.921779 shuttleai-4.0.0/shuttleai/client/_sync.py
--rw-r--r--   0        0        0     4541 2024-06-02 02:11:48.388511 shuttleai-4.0.0/shuttleai/client/base.py
--rw-r--r--   0        0        0     1823 2024-06-02 00:35:28.615546 shuttleai-4.0.0/shuttleai/exceptions.py
--rw-r--r--   0        0        0        0 2024-06-01 20:20:33.018948 shuttleai-4.0.0/shuttleai/py.typed
--rw-r--r--   0        0        0       50 2024-06-02 02:15:22.440205 shuttleai-4.0.0/shuttleai/resources/__init__.py
--rw-r--r--   0        0        0     5506 2024-06-02 01:46:04.821287 shuttleai-4.0.0/shuttleai/resources/chat.py
--rw-r--r--   0        0        0     1640 2024-06-02 02:14:53.228145 shuttleai-4.0.0/shuttleai/resources/images.py
--rw-r--r--   0        0        0        0 2024-06-01 20:25:06.853579 shuttleai-4.0.0/shuttleai/schemas/__init__.py
--rw-r--r--   0        0        0     1751 2024-06-01 21:04:09.631938 shuttleai-4.0.0/shuttleai/schemas/chat_completion.py
--rw-r--r--   0        0        0      294 2024-06-02 04:02:12.707552 shuttleai-4.0.0/shuttleai/schemas/common.py
--rw-r--r--   0        0        0      391 2024-06-02 01:52:38.540553 shuttleai-4.0.0/shuttleai/schemas/images_generations.py
--rw-r--r--   0        0        0        0 2024-06-01 20:47:13.984891 shuttleai-4.0.0/shuttleai/schemas/models/__init__.py
--rw-r--r--   0        0        0     1006 2024-06-02 01:49:21.629939 shuttleai-4.0.0/shuttleai/schemas/models/capabilities.py
--rw-r--r--   0        0        0     2672 2024-06-02 01:50:20.883859 shuttleai-4.0.0/shuttleai/schemas/models/models.py
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 shuttleai-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1220 2024-06-02 04:33:57.303731 shuttleai-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2024-06-02 04:27:14.656264 shuttleai-4.0.1/README.md
+-rw-r--r--   0        0        0      167 2024-06-02 04:35:42.144195 shuttleai-4.0.1/shuttleai/__init__.py
+-rw-r--r--   0        0        0      824 2024-06-02 00:32:35.919932 shuttleai-4.0.1/shuttleai/_patch.py
+-rw-r--r--   0        0        0       76 2024-06-02 02:18:27.148187 shuttleai-4.0.1/shuttleai/client/__init__.py
+-rw-r--r--   0        0        0     6648 2024-06-02 04:04:56.617130 shuttleai-4.0.1/shuttleai/client/_async.py
+-rw-r--r--   0        0        0     6689 2024-06-02 04:06:06.921779 shuttleai-4.0.1/shuttleai/client/_sync.py
+-rw-r--r--   0        0        0     4541 2024-06-02 02:11:48.388511 shuttleai-4.0.1/shuttleai/client/base.py
+-rw-r--r--   0        0        0     1823 2024-06-02 00:35:28.615546 shuttleai-4.0.1/shuttleai/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:20:33.018948 shuttleai-4.0.1/shuttleai/py.typed
+-rw-r--r--   0        0        0       50 2024-06-02 02:15:22.440205 shuttleai-4.0.1/shuttleai/resources/__init__.py
+-rw-r--r--   0        0        0     5506 2024-06-02 01:46:04.821287 shuttleai-4.0.1/shuttleai/resources/chat.py
+-rw-r--r--   0        0        0     1640 2024-06-02 02:14:53.228145 shuttleai-4.0.1/shuttleai/resources/images.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:25:06.853579 shuttleai-4.0.1/shuttleai/schemas/__init__.py
+-rw-r--r--   0        0        0     1751 2024-06-01 21:04:09.631938 shuttleai-4.0.1/shuttleai/schemas/chat_completion.py
+-rw-r--r--   0        0        0      294 2024-06-02 04:02:12.707552 shuttleai-4.0.1/shuttleai/schemas/common.py
+-rw-r--r--   0        0        0      391 2024-06-02 01:52:38.540553 shuttleai-4.0.1/shuttleai/schemas/images_generations.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:47:13.984891 shuttleai-4.0.1/shuttleai/schemas/models/__init__.py
+-rw-r--r--   0        0        0     1006 2024-06-02 01:49:21.629939 shuttleai-4.0.1/shuttleai/schemas/models/capabilities.py
+-rw-r--r--   0        0        0     2672 2024-06-02 01:50:20.883859 shuttleai-4.0.1/shuttleai/schemas/models/models.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 shuttleai-4.0.1/PKG-INFO
```

### Comparing `shuttleai-4.0.0/pyproject.toml` & `shuttleai-4.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "shuttleai"
 version = "0"
 description = "Access Shuttle AI's API via an easy-to-use Python wrapper. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai"
 authors = ["Tristan Liu <tristan@shuttleai.app>", "Christian \"Thoth\" Heru <chris@shuttleai.app>"]
+maintainers = ["Christian \"Thoth\" Heru <chris@shuttleai.app>"]
 readme = "README.md"
 
 [tool.poetry-version-plugin]
 source = "init"
 
 [tool.ruff]
 select = ["E", "F", "W", "Q", "I"]
```

### Comparing `shuttleai-4.0.0/shuttleai/_patch.py` & `shuttleai-4.0.1/shuttleai/_patch.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/client/_async.py` & `shuttleai-4.0.1/shuttleai/client/_async.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/client/_sync.py` & `shuttleai-4.0.1/shuttleai/client/_sync.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/client/base.py` & `shuttleai-4.0.1/shuttleai/client/base.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/exceptions.py` & `shuttleai-4.0.1/shuttleai/exceptions.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/resources/chat.py` & `shuttleai-4.0.1/shuttleai/resources/chat.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/resources/images.py` & `shuttleai-4.0.1/shuttleai/resources/images.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/schemas/chat_completion.py` & `shuttleai-4.0.1/shuttleai/schemas/chat_completion.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/schemas/models/capabilities.py` & `shuttleai-4.0.1/shuttleai/schemas/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/shuttleai/schemas/models/models.py` & `shuttleai-4.0.1/shuttleai/schemas/models/models.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.0/PKG-INFO` & `shuttleai-4.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 4.0.0
+Version: 4.0.1
 Summary: Access Shuttle AI's API via an easy-to-use Python wrapper. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Author: Tristan Liu
 Author-email: tristan@shuttleai.app
+Maintainer: Christian "Thoth" Heru
+Maintainer-email: chris@shuttleai.app
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
```

