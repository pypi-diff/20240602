# Comparing `tmp/shuttleai-4.0.2.tar.gz` & `tmp/shuttleai-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-4.0.2.tar", max compression
+gzip compressed data, was "shuttleai-4.0.3.tar", max compression
```

## Comparing `shuttleai-4.0.2.tar` & `shuttleai-4.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1750 2024-06-02 04:41:40.143530 shuttleai-4.0.2/pyproject.toml
--rw-r--r--   0        0        0       33 2024-06-02 04:27:14.656264 shuttleai-4.0.2/README.md
--rw-r--r--   0        0        0      167 2024-06-02 04:41:51.612118 shuttleai-4.0.2/shuttleai/__init__.py
--rw-r--r--   0        0        0      824 2024-06-02 00:32:35.919932 shuttleai-4.0.2/shuttleai/_patch.py
--rw-r--r--   0        0        0       76 2024-06-02 02:18:27.148187 shuttleai-4.0.2/shuttleai/client/__init__.py
--rw-r--r--   0        0        0     6648 2024-06-02 04:04:56.617130 shuttleai-4.0.2/shuttleai/client/_async.py
--rw-r--r--   0        0        0     6689 2024-06-02 04:06:06.921779 shuttleai-4.0.2/shuttleai/client/_sync.py
--rw-r--r--   0        0        0     4541 2024-06-02 02:11:48.388511 shuttleai-4.0.2/shuttleai/client/base.py
--rw-r--r--   0        0        0     1823 2024-06-02 00:35:28.615546 shuttleai-4.0.2/shuttleai/exceptions.py
--rw-r--r--   0        0        0        0 2024-06-01 20:20:33.018948 shuttleai-4.0.2/shuttleai/py.typed
--rw-r--r--   0        0        0       50 2024-06-02 02:15:22.440205 shuttleai-4.0.2/shuttleai/resources/__init__.py
--rw-r--r--   0        0        0     5506 2024-06-02 01:46:04.821287 shuttleai-4.0.2/shuttleai/resources/chat.py
--rw-r--r--   0        0        0     1640 2024-06-02 02:14:53.228145 shuttleai-4.0.2/shuttleai/resources/images.py
--rw-r--r--   0        0        0        0 2024-06-01 20:25:06.853579 shuttleai-4.0.2/shuttleai/schemas/__init__.py
--rw-r--r--   0        0        0     1751 2024-06-01 21:04:09.631938 shuttleai-4.0.2/shuttleai/schemas/chat_completion.py
--rw-r--r--   0        0        0      294 2024-06-02 04:02:12.707552 shuttleai-4.0.2/shuttleai/schemas/common.py
--rw-r--r--   0        0        0      391 2024-06-02 01:52:38.540553 shuttleai-4.0.2/shuttleai/schemas/images_generations.py
--rw-r--r--   0        0        0        0 2024-06-01 20:47:13.984891 shuttleai-4.0.2/shuttleai/schemas/models/__init__.py
--rw-r--r--   0        0        0     1006 2024-06-02 01:49:21.629939 shuttleai-4.0.2/shuttleai/schemas/models/capabilities.py
--rw-r--r--   0        0        0     2672 2024-06-02 01:50:20.883859 shuttleai-4.0.2/shuttleai/schemas/models/models.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 shuttleai-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1680 2024-06-02 04:44:11.435576 shuttleai-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0       33 2024-06-02 04:27:14.656264 shuttleai-4.0.3/README.md
+-rw-r--r--   0        0        0      167 2024-06-02 04:44:19.933785 shuttleai-4.0.3/shuttleai/__init__.py
+-rw-r--r--   0        0        0      824 2024-06-02 00:32:35.919932 shuttleai-4.0.3/shuttleai/_patch.py
+-rw-r--r--   0        0        0       76 2024-06-02 02:18:27.148187 shuttleai-4.0.3/shuttleai/client/__init__.py
+-rw-r--r--   0        0        0     6648 2024-06-02 04:04:56.617130 shuttleai-4.0.3/shuttleai/client/_async.py
+-rw-r--r--   0        0        0     6689 2024-06-02 04:06:06.921779 shuttleai-4.0.3/shuttleai/client/_sync.py
+-rw-r--r--   0        0        0     4541 2024-06-02 02:11:48.388511 shuttleai-4.0.3/shuttleai/client/base.py
+-rw-r--r--   0        0        0     1823 2024-06-02 00:35:28.615546 shuttleai-4.0.3/shuttleai/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:20:33.018948 shuttleai-4.0.3/shuttleai/py.typed
+-rw-r--r--   0        0        0       50 2024-06-02 02:15:22.440205 shuttleai-4.0.3/shuttleai/resources/__init__.py
+-rw-r--r--   0        0        0     5506 2024-06-02 01:46:04.821287 shuttleai-4.0.3/shuttleai/resources/chat.py
+-rw-r--r--   0        0        0     1640 2024-06-02 02:14:53.228145 shuttleai-4.0.3/shuttleai/resources/images.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:25:06.853579 shuttleai-4.0.3/shuttleai/schemas/__init__.py
+-rw-r--r--   0        0        0     1751 2024-06-01 21:04:09.631938 shuttleai-4.0.3/shuttleai/schemas/chat_completion.py
+-rw-r--r--   0        0        0      294 2024-06-02 04:02:12.707552 shuttleai-4.0.3/shuttleai/schemas/common.py
+-rw-r--r--   0        0        0      391 2024-06-02 01:52:38.540553 shuttleai-4.0.3/shuttleai/schemas/images_generations.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:47:13.984891 shuttleai-4.0.3/shuttleai/schemas/models/__init__.py
+-rw-r--r--   0        0        0     1006 2024-06-02 01:49:21.629939 shuttleai-4.0.3/shuttleai/schemas/models/capabilities.py
+-rw-r--r--   0        0        0     2672 2024-06-02 01:50:20.883859 shuttleai-4.0.3/shuttleai/schemas/models/models.py
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 shuttleai-4.0.3/PKG-INFO
```

### Comparing `shuttleai-4.0.2/pyproject.toml` & `shuttleai-4.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "shuttleai"
 version = "0"
 description = "Access Shuttle AI's API via an easy-to-use Python wrapper. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai"
 authors = ["Tristan Liu <tristan@shuttleai.app>", "Christian \"Thoth\" Heru <chris@shuttleai.app>"]
 maintainers = ["Christian \"Thoth\" Heru <chris@shuttleai.app>"]
 homepage = "https://github.com/shuttleai"
 repository = "https://github.com/shuttleai/shuttleai-python"
-urls = {docs = "https://docs.shuttleai.app", repository = "https://github.com/shuttleai/shuttleai-python", dashboard = "https://shuttleai.app", discord = "https://discord.gg/shuttleai"}
+urls = { Documentation = "https://docs.shuttleai.app", Dashboard = "https://shuttleai.app", Discord = "https://discord.gg/shuttleai" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["shuttleai", "ai", "gpt", "claude", "api", "free", "chatgpt", "gpt-4"]
@@ -40,15 +40,14 @@
 orjson = "^3.10.3"
 pydantic = "^2.7.2"
 httpx = ">= 0.25.2, < 1"
 python-dateutil = "^2.9.0.post0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.6"
-black = "^24.4.2"
 mypy = "^1.7.1"
 types-requests = "^2.31.0.10"
 pytest = "^7.4.3"
 pytest-asyncio = "^0.23.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `shuttleai-4.0.2/shuttleai/_patch.py` & `shuttleai-4.0.3/shuttleai/_patch.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/client/_async.py` & `shuttleai-4.0.3/shuttleai/client/_async.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/client/_sync.py` & `shuttleai-4.0.3/shuttleai/client/_sync.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/client/base.py` & `shuttleai-4.0.3/shuttleai/client/base.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/exceptions.py` & `shuttleai-4.0.3/shuttleai/exceptions.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/resources/chat.py` & `shuttleai-4.0.3/shuttleai/resources/chat.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/resources/images.py` & `shuttleai-4.0.3/shuttleai/resources/images.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/schemas/chat_completion.py` & `shuttleai-4.0.3/shuttleai/schemas/chat_completion.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/schemas/models/capabilities.py` & `shuttleai-4.0.3/shuttleai/schemas/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/shuttleai/schemas/models/models.py` & `shuttleai-4.0.3/shuttleai/schemas/models/models.py`

 * *Files identical despite different names*

### Comparing `shuttleai-4.0.2/PKG-INFO` & `shuttleai-4.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 4.0.2
+Version: 4.0.3
 Summary: Access Shuttle AI's API via an easy-to-use Python wrapper. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Author: Tristan Liu
 Author-email: tristan@shuttleai.app
 Maintainer: Christian "Thoth" Heru
 Maintainer-email: chris@shuttleai.app
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: httpx (>=0.25.2,<1)
 Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: pydantic (>=2.7.2,<3.0.0)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
+Project-URL: Documentation, https://docs.shuttleai.app
+Project-URL: Dashboard, https://shuttleai.app
+Project-URL: Discord, https://discord.gg/shuttleai
 Project-URL: Repository, https://github.com/shuttleai/shuttleai-python
-Project-URL: docs, https://docs.shuttleai.app
-Project-URL: dashboard, https://shuttleai.app
-Project-URL: discord, https://discord.gg/shuttleai
-Project-URL: repository, https://github.com/shuttleai/shuttleai-python
 Description-Content-Type: text/markdown
 
 # ShuttleAI Python Wrapper Remake
```

