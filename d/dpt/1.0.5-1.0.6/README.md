# Comparing `tmp/dpt-1.0.5.tar.gz` & `tmp/dpt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-1.0.5.tar", last modified: Sun Jun  2 15:18:58 2024, max compression
+gzip compressed data, was "dpt-1.0.6.tar", last modified: Sun Jun  2 19:32:03 2024, max compression
```

## Comparing `dpt-1.0.5.tar` & `dpt-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.184159 dpt-1.0.5/
--rw-rw-rw-   0        0        0      188 2024-06-02 15:18:58.183127 dpt-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.140282 dpt-1.0.5/dpt/
--rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.5/dpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.172588 dpt-1.0.5/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.5/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.5/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.5/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.5/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.5/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.180584 dpt-1.0.5/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.5/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.5/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.5/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.5/dpt/processor.py
--rw-rw-rw-   0        0        0     7435 2024-06-02 15:16:39.000000 dpt-1.0.5/dpt/storage.py
-drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.165360 dpt-1.0.5/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 15:18:58.184159 dpt-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-06-02 15:18:15.000000 dpt-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.032671 dpt-1.0.6/
+-rw-rw-rw-   0        0        0      188 2024-06-02 19:32:03.031669 dpt-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 19:32:02.954392 dpt-1.0.6/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.6/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.016671 dpt-1.0.6/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.6/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.6/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.6/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.6/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.6/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.027670 dpt-1.0.6/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.6/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.6/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.6/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13690 2024-06-02 19:07:54.000000 dpt-1.0.6/dpt/processor.py
+-rw-rw-rw-   0        0        0     8888 2024-06-02 19:30:53.000000 dpt-1.0.6/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:32:03.000671 dpt-1.0.6/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-06-02 19:32:02.000000 dpt-1.0.6/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:32:03.033671 dpt-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-06-02 19:31:58.000000 dpt-1.0.6/setup.py
```

### Comparing `dpt-1.0.5/dpt/deployment/deploy.py` & `dpt-1.0.6/dpt/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.5/dpt/deployment/extract.py` & `dpt-1.0.6/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.5/dpt/management.py` & `dpt-1.0.6/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.5/dpt/mongo/files.py` & `dpt-1.0.6/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.5/dpt/processor.py` & `dpt-1.0.6/dpt/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .storage import (
     DatabaseInfo,
     ConnectionInfo,
     DbReader,
     DbWriter,
     MemoryReader,
     MemoryWriter,
+    TempCollection,
 )
 import inspect
 from pymongo.database import Database as MongoDatabase
 
 # todo replace print with logging
 
 
@@ -355,14 +356,19 @@
         if self._database != None:
             return self._database
         return self.processor.module.project._get_debug_db()
 
     def set_database(self, value: MongoDatabase):
         self._database = DatabaseInfo(instance=value)
 
+    def temp_coll(self, name):
+        # todo учесть контекст чтобы не затереть данные при параллельном выполнении, и при этом не накапливать неконтролируемо временные данные в БД
+        full_name =  f"sys_qs_flow_{name}"
+        return TempCollection(full_name, self._get_database())
+
     def get_named_reader(self, input_name: str) -> DbReader | MemoryReader:
         if not input_name in self.processor.inputs:
             raise Exception(f"Input '{input_name}' is not declared")
         source = self._input_binding[input_name]
         if isinstance(source, str):
             val = DbReader(source, self._get_database())
         else:
```

### Comparing `dpt-1.0.5/dpt/storage.py` & `dpt-1.0.6/dpt/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,73 +52,29 @@
         #     self.database = Database()
         self._instance = None
 
     def get_count(self):
         if self._count == None:
             self._update_count_from_collection()
         return self._count
-    
-    def get_collection_name(self):
+
+    def get_coll_name(self):
         return self.name
 
     def get_info(self):
         return f"collection '{self.name}'"
 
     def instance(self) -> Collection:
         if self._instance == None:
             self._instance = self.database.instance()[self.name]
         return self._instance
 
     def _update_count_from_collection(self):
         self._count = self.instance().count_documents({})
 
-
-class DbReader(CollectionInfo):
-    def __init__(self, collectionName: str, database: DatabaseInfo = None):
-        super().__init__(collectionName, database)
-
-    def read_all(self):
-        self._count = self.instance().count_documents({})
-        print(f"read {self._count} documents from {self.get_info()}")
-
-        return self.instance().find({})
-
-    def read_one(self):
-        self._count += 1
-        return self.instance().find_one({})
-
-    def _prepare_pipeline(self, pipeline: list[dict])-> list[dict]:
-        orig_pipeline = pipeline
-        new_pipeline: list[dict] = []
-        for step in orig_pipeline:
-            new_pipeline.append(step.copy())
-
-        def bad_ref_text(step, coll_ref):
-            return f'Incorrect collection reference `{coll_ref}`. Use reader object to reference collection, e. g. "from": task.get_named_reader("coll_to_join"). Incorrect step: \n {step}'
-
-        def first_of(d) -> tuple[str, dict]:
-            for key, value in d.items():
-                return key, value
-
-        for step in new_pipeline:
-            step_name, step = first_of(step)
-            if step_name in ["$lookup", "$graphLookup", "$unionWith"]:
-                coll_ref = step.get("from") or step.get("coll")
-                if isinstance(coll_ref, DbReader):
-                    step["from"] = coll_ref._collection_name
-                else:
-                    raise Exception(bad_ref_text(step, coll_ref))
-            if step_name in ["$lookup"]:
-                nested_pipeline = step.get("pipeline")
-                if (nested_pipeline!=None):
-                    step["pipeline"] =  self._prepare_pipeline(nested_pipeline)
-        return new_pipeline
-
-                
-
     def _create_lookup_indexes(self, item: list[dict] | dict):
         objects = []
         if isinstance(item, dict):
             objects = [item]
         if isinstance(item, list):
             objects = item
         for obj in objects:
@@ -130,51 +86,171 @@
                         if "foreignField" in spec:
                             field = spec["foreignField"]
                             coll = self.instance().database[coll_name]
                             ind_opt = (field, 1)
                             coll.create_index([ind_opt])
                     self._create_lookup_indexes(obj[name])
 
-    def aggregate(self, out: DbWriter, pipeline: list[dict[str, Any]]):
-        self._update_count_from_collection()
-        prep_pipeline = self._prepare_pipeline(pipeline)
+    def _aggregate(self, pipeline: list[dict[str, Any]], out: CollectionInfo = None):
+
+        last_step = pipeline[-1]
+
+        bad_step = None
+        if "$out" in last_step:
+            bad_step =  "$out"
+        if "$merge" in last_step:
+            bad_step =  "$merge"
+
+        if bad_step!=None:
+            raise Exception(f'{bad_step} stage is not allowed. Please use "out" parameter instead, e. g. aggregate(out=task.temp_coll("my_temp_coll"),pipeline=[...])')
+
+        if out != None:
+            self._update_count_from_collection()
+            print(f"read {self._count} documents from {self.get_info()}")
+            print("")
+
+        prep_pipeline = _prepare_pipeline(pipeline)
         self._create_lookup_indexes(prep_pipeline)
-        prep_pipeline.append({"$out": out._collection_name})
-        print(f"read {self._count} documents from {self.get_info()}")
-        print("")
-        pipeline_json = json.dumps(prep_pipeline,ensure_ascii=False)
+        if out != None:
+            prep_pipeline.append({"$out": out._collection_name})
+        pipeline_json = json.dumps(prep_pipeline, ensure_ascii=False)
         print("run aggregation:")
         print("")
-        print(f'db.getCollection("{self.instance().name}").aggregate(\n{pipeline_json}\n)')
+        print(
+            f'db.getCollection("{self.instance().name}").aggregate(\n{pipeline_json}\n)'
+        )
         print("")
-        self.instance().aggregate(prep_pipeline)
-        out._update_count_from_collection()
-        out.close()
+        if out != None:
+            self.instance().aggregate(prep_pipeline)
+            out._update_count_from_collection()
+            if isinstance(out, DbWriter):
+                out.close()
+        else:
+            return self.instance().aggregate(prep_pipeline)
+
+    def _read_all(self):
+        self._count = self.instance().count_documents({})
+        print(f"read {self._count} documents from {self.get_info()}")
+        return self.instance().find({})
+
+    def _read_one(self):
+        return self.instance().find_one({})
+
+    def _clear(self):
+        self._count = 0
+        self.instance().delete_many({})
+
+    def _write_many(self, documents: list[dict]):
+        if len(documents) > 0:
+            self.instance().insert_many(documents)
+        self._count += len(documents)
 
     def create_index(
         self,
         keys,
     ) -> str:
         self.instance().create_index(keys=keys)
 
 
+def _prepare_pipeline(pipeline: list[dict]) -> list[dict]:
+    orig_pipeline = pipeline
+    new_pipeline: list[dict] = []
+    for step in orig_pipeline:
+        new_pipeline.append(step.copy())
+
+    def bad_ref_text(step, coll_ref):
+        return f'Incorrect collection reference `{coll_ref}`. Use reader object to reference collection, e. g. "from": task.get_named_reader("coll_to_join"). Incorrect step: \n {step}'
+
+    def first_of(d) -> tuple[str, dict]:
+        for key, value in d.items():
+            return key, value
+
+    for step in new_pipeline:
+        step_name, step = first_of(step)
+        if step_name in ["$lookup", "$graphLookup", "$unionWith"]:
+            coll_ref = step.get("from") or step.get("coll")
+            if isinstance(coll_ref, CollectionInfo):
+                step["from"] = coll_ref._collection_name
+            else:
+                raise Exception(bad_ref_text(step, coll_ref))
+        if step_name in ["$lookup"]:
+            nested_pipeline = step.get("pipeline")
+            if nested_pipeline != None:
+                step["pipeline"] = _prepare_pipeline(nested_pipeline)
+    return new_pipeline
+
+
+class DbReader(CollectionInfo):
+    def __init__(self, collectionName: str, database: DatabaseInfo = None):
+        super().__init__(collectionName, database)
+
+    def read_all(self):
+        return self._read_all()
+
+    def read_one(self):
+        return self._read_one()
+
+    def aggregate(self, pipeline: list[dict[str, Any]], out: DbWriter | TempCollection = None):
+        return self._aggregate(pipeline, out)
+
+
+class DbWriter(CollectionInfo):
+    def __init__(self, collectionName: str, database: DatabaseInfo = None):
+        super().__init__(collectionName, database)
+        self._closed = True
+
+    def clear(self):
+        self._clear()
+
+    def write_many(self, documents: list[dict]):
+        self._write_many(documents)
+        self._closed = False
+
+    def close(self):
+        self._closed = True
+        print(f"loaded {self._count} documents into {self.get_info()}")
+
+    def is_closed(self):
+        return self._closed
+
+
+class TempCollection(CollectionInfo):
+    def __init__(self, collectionName: str, database: DatabaseInfo = None):
+        super().__init__(collectionName, database)
+
+    def clear(self):
+        self._clear()
+
+    def write_many(self, documents: list[dict]):
+        self._write_many(documents)
+
+    def read_all(self):
+        return self._read_all()
+
+    def read_one(self):
+        return self._read_one()
+
+    def aggregate(self, pipeline: list[dict[str, Any]], out: DbWriter | TempCollection = None):
+        return self._aggregate(pipeline, out)
+
+
 class MemoryReader:
     def __init__(self, data: list[dict[str, Any]], schema: dict):
         self._data = data
         self.schema = schema
 
     def _validate(self):
         if self.schema == None:
             return
         for item in self._data:
             jsonschema.validate(instance=item, schema=self.schema)
 
     def get_count(self):
         return len(self._data)
-    
+
     def get_collection_name(self):
         return None
 
     def get_info(self):
         return f"list[]"
 
     def read_all(self):
@@ -185,37 +261,14 @@
     def read_one(self) -> Any | None:
         self._validate()
         if len(self._data) == 0:
             return None
         return self._data[0]
 
 
-class DbWriter(CollectionInfo):
-    def __init__(self, collectionName: str, database: DatabaseInfo = None):
-
-        super().__init__(collectionName, database)
-        self._closed = True
-
-    def clear(self):
-        self.instance().delete_many({})
-
-    def write_many(self, documents: list[dict]):
-        if len(documents) > 0:
-            self.instance().insert_many(documents)
-        self._count += len(documents)
-        self._closed = False
-
-    def close(self):
-        self._closed = True
-        print(f"loaded {self._count} documents into {self.get_info()}")
-
-    def is_closed(self):
-        return self._closed
-
-
 class MemoryWriter:
     def __init__(self, data: list[dict[str, Any]]):
         self._data = data
         self._count = 0
         self._closed = True
 
     def get_info(self):
```

