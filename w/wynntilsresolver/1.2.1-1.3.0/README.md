# Comparing `tmp/wynntilsresolver-1.2.1.tar.gz` & `tmp/wynntilsresolver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wynntilsresolver-1.2.1.tar", last modified: Mon Mar 25 06:40:23 2024, max compression
+gzip compressed data, was "wynntilsresolver-1.3.0.tar", last modified: Sun Jun  2 15:39:06 2024, max compression
```

## Comparing `wynntilsresolver-1.2.1.tar` & `wynntilsresolver-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1090 2024-02-29 02:46:41.721195 wynntilsresolver-1.2.1/LICENSE
--rw-r--r--   0        0        0     1649 2024-03-25 06:40:23.143448 wynntilsresolver-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3926 2024-03-11 02:34:02.090200 wynntilsresolver-1.2.1/readme.md
--rw-r--r--   0        0        0     1250 2024-03-09 16:00:16.124062 wynntilsresolver-1.2.1/tests/test_blocks/test_block.py
--rw-r--r--   0        0        0     3189 2024-03-08 20:56:11.471076 wynntilsresolver-1.2.1/tests/test_item.py
--rw-r--r--   0        0        0     3961 2024-03-08 20:30:10.860356 wynntilsresolver-1.2.1/tests/test_resolver.py
--rw-r--r--   0        0        0     2241 2024-03-07 03:41:08.077304 wynntilsresolver-1.2.1/tests/test_utils.py
--rw-r--r--   0        0        0      393 2024-03-21 17:01:22.070883 wynntilsresolver-1.2.1/wynntilsresolver/__init__.py
--rw-r--r--   0        0        0      861 2024-03-08 20:32:01.648375 wynntilsresolver-1.2.1/wynntilsresolver/blocks/__init__.py
--rw-r--r--   0        0        0     2884 2024-03-21 17:44:37.034597 wynntilsresolver-1.2.1/wynntilsresolver/blocks/block.py
--rw-r--r--   0        0        0      670 2024-03-09 16:00:16.126062 wynntilsresolver-1.2.1/wynntilsresolver/blocks/end.py
--rw-r--r--   0        0        0     4769 2024-03-25 06:40:02.116236 wynntilsresolver-1.2.1/wynntilsresolver/blocks/identification.py
--rw-r--r--   0        0        0      801 2024-03-09 16:00:16.127061 wynntilsresolver-1.2.1/wynntilsresolver/blocks/name.py
--rw-r--r--   0        0        0     1715 2024-03-09 16:00:16.127061 wynntilsresolver-1.2.1/wynntilsresolver/blocks/powder.py
--rw-r--r--   0        0        0      791 2024-03-11 02:18:15.148854 wynntilsresolver-1.2.1/wynntilsresolver/blocks/reroll.py
--rw-r--r--   0        0        0     1763 2024-03-11 03:05:04.718223 wynntilsresolver-1.2.1/wynntilsresolver/blocks/shiny.py
--rw-r--r--   0        0        0     1575 2024-03-25 06:30:53.270440 wynntilsresolver-1.2.1/wynntilsresolver/blocks/type.py
--rw-r--r--   0        0        0      836 2024-03-09 16:00:16.131049 wynntilsresolver-1.2.1/wynntilsresolver/blocks/version.py
--rw-r--r--   0        0        0      926 2024-03-02 01:49:38.989689 wynntilsresolver-1.2.1/wynntilsresolver/exception.py
--rw-r--r--   0        0        0     1653 2024-03-08 20:53:49.753655 wynntilsresolver-1.2.1/wynntilsresolver/item.py
--rw-r--r--   0        0        0        0 2024-03-02 01:49:39.296168 wynntilsresolver-1.2.1/wynntilsresolver/py.typed
--rw-r--r--   0        0        0     5706 2024-03-21 17:41:15.587364 wynntilsresolver-1.2.1/wynntilsresolver/resolver.py
--rw-r--r--   0        0        0     2728 2024-03-21 17:33:40.303094 wynntilsresolver-1.2.1/wynntilsresolver/startup.py
--rw-r--r--   0        0        0     7600 2024-03-21 17:46:11.783884 wynntilsresolver-1.2.1/wynntilsresolver/utils.py
--rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 wynntilsresolver-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-02-29 02:46:41.721195 wynntilsresolver-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1649 2024-06-02 15:39:06.820974 wynntilsresolver-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4385 2024-06-02 15:38:09.592363 wynntilsresolver-1.3.0/readme.md
+-rw-r--r--   0        0        0     1250 2024-06-02 15:24:23.836109 wynntilsresolver-1.3.0/tests/test_blocks/test_block.py
+-rw-r--r--   0        0        0     3189 2024-06-02 15:24:23.837092 wynntilsresolver-1.3.0/tests/test_item.py
+-rw-r--r--   0        0        0     3961 2024-03-08 20:30:10.860356 wynntilsresolver-1.3.0/tests/test_resolver.py
+-rw-r--r--   0        0        0     2241 2024-03-07 03:41:08.077304 wynntilsresolver-1.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0      393 2024-03-21 17:01:22.070883 wynntilsresolver-1.3.0/wynntilsresolver/__init__.py
+-rw-r--r--   0        0        0      861 2024-03-08 20:32:01.648375 wynntilsresolver-1.3.0/wynntilsresolver/blocks/__init__.py
+-rw-r--r--   0        0        0     2884 2024-06-02 15:24:23.839183 wynntilsresolver-1.3.0/wynntilsresolver/blocks/block.py
+-rw-r--r--   0        0        0      670 2024-06-02 15:24:23.839183 wynntilsresolver-1.3.0/wynntilsresolver/blocks/end.py
+-rw-r--r--   0        0        0     4769 2024-06-02 15:24:23.840184 wynntilsresolver-1.3.0/wynntilsresolver/blocks/identification.py
+-rw-r--r--   0        0        0      801 2024-06-02 15:24:23.841210 wynntilsresolver-1.3.0/wynntilsresolver/blocks/name.py
+-rw-r--r--   0        0        0     1715 2024-06-02 15:24:23.842293 wynntilsresolver-1.3.0/wynntilsresolver/blocks/powder.py
+-rw-r--r--   0        0        0      791 2024-06-02 15:24:23.843286 wynntilsresolver-1.3.0/wynntilsresolver/blocks/reroll.py
+-rw-r--r--   0        0        0     1763 2024-06-02 15:24:23.844286 wynntilsresolver-1.3.0/wynntilsresolver/blocks/shiny.py
+-rw-r--r--   0        0        0     1575 2024-06-02 15:24:23.844286 wynntilsresolver-1.3.0/wynntilsresolver/blocks/type.py
+-rw-r--r--   0        0        0      836 2024-06-02 15:24:23.845305 wynntilsresolver-1.3.0/wynntilsresolver/blocks/version.py
+-rw-r--r--   0        0        0      926 2024-03-02 01:49:38.989689 wynntilsresolver-1.3.0/wynntilsresolver/exception.py
+-rw-r--r--   0        0        0     1653 2024-03-08 20:53:49.753655 wynntilsresolver-1.3.0/wynntilsresolver/item.py
+-rw-r--r--   0        0        0        0 2024-03-02 01:49:39.296168 wynntilsresolver-1.3.0/wynntilsresolver/py.typed
+-rw-r--r--   0        0        0     5706 2024-06-02 15:24:23.847286 wynntilsresolver-1.3.0/wynntilsresolver/resolver.py
+-rw-r--r--   0        0        0     3449 2024-06-02 15:35:09.374355 wynntilsresolver-1.3.0/wynntilsresolver/startup.py
+-rw-r--r--   0        0        0     7600 2024-03-21 17:46:11.783884 wynntilsresolver-1.3.0/wynntilsresolver/utils.py
+-rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 wynntilsresolver-1.3.0/PKG-INFO
```

### Comparing `wynntilsresolver-1.2.1/LICENSE` & `wynntilsresolver-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/pyproject.toml` & `wynntilsresolver-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wynntilsresolver"
-version = "1.2.1"
+version = "1.3.0"
 description = "A simple resolver to analyze wynntils' encoded equipment in chat."
 authors = [
     { name = "FYWinds", email = "i@windis.cn" },
 ]
 dependencies = [
     "httpx==0.27.0",
 ]
```

### Comparing `wynntilsresolver-1.2.1/readme.md` & `wynntilsresolver-1.3.0/readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -66,14 +66,23 @@
 
 print(b.name.name) # Warp
 if b.identifications:
     # Identification(id='rawAgility', internal_id=41, base=20, roll=-1, value=20)
     b.identifications.identifications[0]
 ```
 
+
+### Environment Variables
+- `DATA_LOCATION`: The directory to store the cache files. Default: `pathlib.Path.home() / "AppData" / "Local" / "wynntilsresolver"` or
+`pathlib.Path.home() / ".local" / "share" / "wynntilsresolver"`
+- `ITEMDB_PATH`: The path to the itemdb file.
+- `SHINY_TABLE_PATH`: The path to the shiny table file.
+- `ID_TABLE_PATH`: The path to the id table file.
+> Note that setting the path to those files will disable auto update.
+
 ### Benchmark
 
 #### Resolver Creation With Cache
 > [!IMPORTANT]
 > The benchmark is done with data files downloaded to local.
 > For each 24 hours, the cache will be updated and will take several seconds depending on the network speed.
 ```
```

### Comparing `wynntilsresolver-1.2.1/tests/test_blocks/test_block.py` & `wynntilsresolver-1.3.0/tests/test_blocks/test_block.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/tests/test_item.py` & `wynntilsresolver-1.3.0/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/tests/test_resolver.py` & `wynntilsresolver-1.3.0/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/tests/test_utils.py` & `wynntilsresolver-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/__init__.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/block.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/block.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/end.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/end.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/identification.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/identification.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/name.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/name.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/powder.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/powder.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/reroll.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/reroll.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/shiny.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/shiny.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/type.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/type.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/blocks/version.py` & `wynntilsresolver-1.3.0/wynntilsresolver/blocks/version.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/exception.py` & `wynntilsresolver-1.3.0/wynntilsresolver/exception.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/item.py` & `wynntilsresolver-1.3.0/wynntilsresolver/item.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/resolver.py` & `wynntilsresolver-1.3.0/wynntilsresolver/resolver.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/startup.py` & `wynntilsresolver-1.3.0/wynntilsresolver/startup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Author       : FYWinds i@windis.cn
 Date         : 2024-02-29 15:48:21
 LastEditors  : FYWinds i@windis.cn
-LastEditTime : 2024-03-21 13:10:01
+LastEditTime : 2024-06-02 11:34:26
 FilePath     : /wynntilsresolver/startup.py
 """
 
 import asyncio
 import json
 import os
 import pathlib
@@ -17,42 +17,63 @@
 from .utils import run_async
 
 if os.name == "nt":
     DATA_LOCATION = pathlib.Path.home() / "AppData" / "Local" / "wynntilsresolver"
 else:
     DATA_LOCATION = pathlib.Path.home() / ".local" / "share" / "wynntilsresolver"
 
+if data_location := os.environ.get("DATA_LOCATION"):
+    DATA_LOCATION = pathlib.Path(data_location)
+
 DATA_LOCATION.mkdir(parents=True, exist_ok=True)
 
+
 ITEMDB_FULL_URL = "https://api.wynncraft.com/v3/item/database?fullResult"
 SHINY_TABLE_URL = "https://raw.githubusercontent.com/Wynntils/Static-Storage/main/Data-Storage/shiny_stats.json"
 ID_TABLE_URL = "https://raw.githubusercontent.com/Wynntils/Static-Storage/main/Reference/id_keys.json"
 
-ITEMDB_PATH = DATA_LOCATION / "itemdb.json"
-SHINY_TABLE_PATH = DATA_LOCATION / "shiny_stats.json"
-ID_TABLE_PATH = DATA_LOCATION / "id_keys.json"
+itemdb_path = os.environ.get("ITEMDB_PATH")
+shiny_table_path = os.environ.get("SHINY_TABLE_PATH")
+id_table_path = os.environ.get("ID_TABLE_PATH")
+
+itemdb_should_update = True
+shiny_table_should_update = True
+id_table_should_update = True
+
+if itemdb_path:
+    itemdb_should_update = False
+if shiny_table_path:
+    shiny_table_should_update = False
+if id_table_path:
+    id_table_should_update = False
+
+ITEMDB_PATH = pathlib.Path(itemdb_path or DATA_LOCATION / "itemdb.json")
+SHINY_TABLE_PATH = pathlib.Path(shiny_table_path or DATA_LOCATION / "shiny_stats.json")
+ID_TABLE_PATH = pathlib.Path(id_table_path or DATA_LOCATION / "id_keys.json")
 
 # Read proxy from environment variable.
 http_proxy = os.environ.get("http_proxy") or os.environ.get("HTTP_PROXY")
 https_proxy = os.environ.get("https_proxy") or os.environ.get("HTTPS_PROXY")
 all_proxy = os.environ.get("all_proxy") or os.environ.get("ALL_PROXY")
 
 
 @run_async
 async def startup():
     """Fetch all data from Wynncraft API and Artemis Repository."""
     client = httpx.AsyncClient(proxy=http_proxy or https_proxy or all_proxy)
 
     # Fetch the file only if was not updated within 24 hours.
     tasks = []
-    if not ITEMDB_PATH.exists() or time.time() - os.path.getmtime(ITEMDB_PATH) > 86400:
+    if (not ITEMDB_PATH.exists() or time.time() - os.path.getmtime(ITEMDB_PATH) > 86400) and itemdb_should_update:
         tasks += [fetch_item_db(client)]
-    if not SHINY_TABLE_PATH.exists() or time.time() - os.path.getmtime(SHINY_TABLE_PATH) > 86400:
+    if (
+        not SHINY_TABLE_PATH.exists() or time.time() - os.path.getmtime(SHINY_TABLE_PATH) > 86400
+    ) and shiny_table_should_update:
         tasks += [fetch_shiny_table(client)]
-    if not ID_TABLE_PATH.exists() or time.time() - os.path.getmtime(ID_TABLE_PATH) > 86400:
+    if (not ID_TABLE_PATH.exists() or time.time() - os.path.getmtime(ID_TABLE_PATH) > 86400) and id_table_should_update:
         tasks += [fetch_id_table(client)]
     await asyncio.gather(*tasks)
 
     await client.aclose()
 
 
 async def fetch_item_db(client: httpx.AsyncClient):
```

### Comparing `wynntilsresolver-1.2.1/wynntilsresolver/utils.py` & `wynntilsresolver-1.3.0/wynntilsresolver/utils.py`

 * *Files identical despite different names*

### Comparing `wynntilsresolver-1.2.1/PKG-INFO` & `wynntilsresolver-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wynntilsresolver
-Version: 1.2.1
+Version: 1.3.0
 Summary: A simple resolver to analyze wynntils' encoded equipment in chat.
-Keywords: wynntils resolver wynncraft
+Keywords: wynntils,resolver,wynncraft
 Author-Email: FYWinds <i@windis.cn>
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -93,14 +93,23 @@
 
 print(b.name.name) # Warp
 if b.identifications:
     # Identification(id='rawAgility', internal_id=41, base=20, roll=-1, value=20)
     b.identifications.identifications[0]
 ```
 
+
+### Environment Variables
+- `DATA_LOCATION`: The directory to store the cache files. Default: `pathlib.Path.home() / "AppData" / "Local" / "wynntilsresolver"` or
+`pathlib.Path.home() / ".local" / "share" / "wynntilsresolver"`
+- `ITEMDB_PATH`: The path to the itemdb file.
+- `SHINY_TABLE_PATH`: The path to the shiny table file.
+- `ID_TABLE_PATH`: The path to the id table file.
+> Note that setting the path to those files will disable auto update.
+
 ### Benchmark
 
 #### Resolver Creation With Cache
 > [!IMPORTANT]
 > The benchmark is done with data files downloaded to local.
 > For each 24 hours, the cache will be updated and will take several seconds depending on the network speed.
 ```
```

