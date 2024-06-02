# Comparing `tmp/joker-mongodb-0.3.0.tar.gz` & `tmp/joker-mongodb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-mongodb-0.3.0.tar", last modified: Mon May  6 02:57:45 2024, max compression
+gzip compressed data, was "joker-mongodb-0.3.1.tar", last modified: Sun Jun  2 08:09:25 2024, max compression
```

## Comparing `joker-mongodb-0.3.0.tar` & `joker-mongodb-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.697944 joker-mongodb-0.3.0/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2021-07-11 03:40:54.000000 joker-mongodb-0.3.0/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       41 2021-07-11 03:42:23.000000 joker-mongodb-0.3.0/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     2528 2024-05-06 02:57:45.697462 joker-mongodb-0.3.0/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     1574 2022-05-25 12:06:36.000000 joker-mongodb-0.3.0/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.681595 joker-mongodb-0.3.0/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.684970 joker-mongodb-0.3.0/joker/mongodb/
--rw-r--r--   0 Hailong    (502) staff       (20)      163 2024-05-06 02:51:05.000000 joker-mongodb-0.3.0/joker/mongodb/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     6378 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/interfaces.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1857 2024-04-25 06:15:26.000000 joker-mongodb-0.3.0/joker/mongodb/legacy.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.693579 joker-mongodb-0.3.0/joker/mongodb/tools/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-11 03:25:17.000000 joker-mongodb-0.3.0/joker/mongodb/tools/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1329 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/cmdline.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1115 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/dumping.py
--rw-r--r--   0 Hailong    (502) staff       (20)      242 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/experimental.py
--rw-r--r--   0 Hailong    (502) staff       (20)      763 2024-04-25 06:14:37.000000 joker-mongodb-0.3.0/joker/mongodb/tools/filters.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1514 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/integrity.py
--rw-r--r--   0 Hailong    (502) staff       (20)      674 2024-04-25 06:18:35.000000 joker-mongodb-0.3.0/joker/mongodb/tools/kvstore.py
--rw-r--r--   0 Hailong    (502) staff       (20)     9804 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/misc.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1088 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/mongoshell.py
--rw-r--r--   0 Hailong    (502) staff       (20)     5520 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/oplog.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1709 2024-05-06 02:51:05.000000 joker-mongodb-0.3.0/joker/mongodb/tools/paginations.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1161 2024-04-25 06:08:49.000000 joker-mongodb-0.3.0/joker/mongodb/tools/querying.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3917 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/schema.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1207 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/transactional.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3738 2024-04-25 06:13:43.000000 joker-mongodb-0.3.0/joker/mongodb/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.697100 joker-mongodb-0.3.0/joker_mongodb.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     2528 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      872 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-25 12:01:12.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-04-25 05:57:29.000000 joker-mongodb-0.3.0/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-05-06 02:57:45.698008 joker-mongodb-0.3.0/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2147 2024-04-25 06:23:26.000000 joker-mongodb-0.3.0/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 08:09:25.269843 joker-mongodb-0.3.1/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2021-07-11 03:40:54.000000 joker-mongodb-0.3.1/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       41 2021-07-11 03:42:23.000000 joker-mongodb-0.3.1/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     2528 2024-06-02 08:09:25.269343 joker-mongodb-0.3.1/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     1574 2022-05-25 12:06:36.000000 joker-mongodb-0.3.1/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 08:09:25.245587 joker-mongodb-0.3.1/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 08:09:25.253001 joker-mongodb-0.3.1/joker/mongodb/
+-rw-r--r--   0 Hailong    (502) staff       (20)      163 2024-06-02 08:05:37.000000 joker-mongodb-0.3.1/joker/mongodb/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2384 2024-06-02 08:05:24.000000 joker-mongodb-0.3.1/joker/mongodb/batch.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     6396 2024-05-29 08:31:46.000000 joker-mongodb-0.3.1/joker/mongodb/interfaces.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1857 2024-04-25 06:15:26.000000 joker-mongodb-0.3.1/joker/mongodb/legacy.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1741 2024-06-02 07:59:35.000000 joker-mongodb-0.3.1/joker/mongodb/logger.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 08:09:25.264537 joker-mongodb-0.3.1/joker/mongodb/tools/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-11 03:25:17.000000 joker-mongodb-0.3.1/joker/mongodb/tools/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1329 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/cmdline.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1115 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/dumping.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      242 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/experimental.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      763 2024-04-25 06:14:37.000000 joker-mongodb-0.3.1/joker/mongodb/tools/filters.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1514 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/integrity.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      674 2024-04-25 06:18:35.000000 joker-mongodb-0.3.1/joker/mongodb/tools/kvstore.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     9804 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/misc.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1088 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/mongoshell.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     5520 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/oplog.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1661 2024-05-06 03:38:58.000000 joker-mongodb-0.3.1/joker/mongodb/tools/paginations.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1161 2024-04-25 06:08:49.000000 joker-mongodb-0.3.1/joker/mongodb/tools/querying.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3917 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/schema.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1207 2024-04-25 06:16:01.000000 joker-mongodb-0.3.1/joker/mongodb/tools/transactional.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2165 2024-06-02 08:00:09.000000 joker-mongodb-0.3.1/joker/mongodb/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-06-02 08:09:25.268484 joker-mongodb-0.3.1/joker_mongodb.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     2528 2024-06-02 08:09:25.000000 joker-mongodb-0.3.1/joker_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      919 2024-06-02 08:09:25.000000 joker-mongodb-0.3.1/joker_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-06-02 08:09:25.000000 joker-mongodb-0.3.1/joker_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-06-02 08:09:25.000000 joker-mongodb-0.3.1/joker_mongodb.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-25 12:01:12.000000 joker-mongodb-0.3.1/joker_mongodb.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-06-02 08:09:25.000000 joker-mongodb-0.3.1/joker_mongodb.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-06-02 08:09:25.000000 joker-mongodb-0.3.1/joker_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-04-25 05:57:29.000000 joker-mongodb-0.3.1/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-06-02 08:09:25.269946 joker-mongodb-0.3.1/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2147 2024-04-25 06:23:26.000000 joker-mongodb-0.3.1/setup.py
```

### Comparing `joker-mongodb-0.3.0/LICENSE` & `joker-mongodb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/PKG-INFO` & `joker-mongodb-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-mongodb
-Version: 0.3.0
+Version: 0.3.1
 Summary: access mongodb with handy utilities and fun
 Home-page: https://github.com/frozflame/joker-mongodb
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `joker-mongodb-0.3.0/README.md` & `joker-mongodb-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/interfaces.py` & `joker-mongodb-0.3.1/joker/mongodb/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from volkanic.utils import printerr
 
 from joker.mongodb import utils
 from joker.mongodb.tools import kvstore
 
 
 class CollectionInterface:
+    # deprecated!
     def __init__(self, coll: Collection, filtr=None, projection=None):
         self._coll = coll
         self.filtr = filtr or {}
         self.projection = projection
 
     def exist(self, filtr: Union[ObjectId, dict]):
         return self._coll.find_one(filtr, projection=[])
```

### Comparing `joker-mongodb-0.3.0/joker/mongodb/legacy.py` & `joker-mongodb-0.3.1/joker/mongodb/legacy.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/cmdline.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/cmdline.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/dumping.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/dumping.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/filters.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/filters.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/integrity.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/integrity.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/kvstore.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/kvstore.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/misc.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/misc.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/mongoshell.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/mongoshell.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/oplog.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/oplog.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/paginations.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/paginations.py`

 * *Files 19% similar despite different names*

```diff
@@ -51,13 +51,14 @@
         # from typing import Self
         # from_raw(cls: type[Self], raw: Iterable[RawResultDict]) -> Self:
         result: RawResultDict = list(raw)[0]
         counts = result["counts"]
         total = counts[0]["total"] if counts else 0
         return PaginatedResult(items=result["documents"], total=total)
 
+    def to_dict(self) -> dict:
+        return dataclasses.asdict(self)
+
 
 def compact_paginated_result(cursor: Iterable[RawResultDict]) -> PaginatedResult:
-    result: RawResultDict = list(cursor)[0]
-    counts = result["counts"]
-    total = counts[0]["total"] if counts else 0
-    return PaginatedResult(items=result["documents"], total=total)
+    # will be deprecated
+    return PaginatedResult.from_raw(cursor)
```

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/querying.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/querying.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/schema.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/schema.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker/mongodb/tools/transactional.py` & `joker-mongodb-0.3.1/joker/mongodb/tools/transactional.py`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.3.0/joker_mongodb.egg-info/PKG-INFO` & `joker-mongodb-0.3.1/joker_mongodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-mongodb
-Version: 0.3.0
+Version: 0.3.1
 Summary: access mongodb with handy utilities and fun
 Home-page: https://github.com/frozflame/joker-mongodb
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `joker-mongodb-0.3.0/joker_mongodb.egg-info/SOURCES.txt` & `joker-mongodb-0.3.1/joker_mongodb.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 joker/mongodb/__init__.py
+joker/mongodb/batch.py
 joker/mongodb/interfaces.py
 joker/mongodb/legacy.py
+joker/mongodb/logger.py
 joker/mongodb/utils.py
 joker/mongodb/tools/__init__.py
 joker/mongodb/tools/cmdline.py
 joker/mongodb/tools/dumping.py
 joker/mongodb/tools/experimental.py
 joker/mongodb/tools/filters.py
 joker/mongodb/tools/integrity.py
```

### Comparing `joker-mongodb-0.3.0/setup.py` & `joker-mongodb-0.3.1/setup.py`

 * *Files identical despite different names*

