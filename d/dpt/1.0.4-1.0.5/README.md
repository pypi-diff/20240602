# Comparing `tmp/dpt-1.0.4.tar.gz` & `tmp/dpt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-1.0.4.tar", last modified: Sat Jun  1 01:11:30 2024, max compression
+gzip compressed data, was "dpt-1.0.5.tar", last modified: Sun Jun  2 15:18:58 2024, max compression
```

## Comparing `dpt-1.0.4.tar` & `dpt-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 01:11:30.066807 dpt-1.0.4/
--rw-rw-rw-   0        0        0      188 2024-06-01 01:11:30.064808 dpt-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 01:11:30.003812 dpt-1.0.4/dpt/
--rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.4/dpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 01:11:30.049817 dpt-1.0.4/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.4/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.4/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.4/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.4/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.4/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-06-01 01:11:30.060818 dpt-1.0.4/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.4/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.4/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.4/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.4/dpt/processor.py
--rw-rw-rw-   0        0        0     7226 2024-06-01 01:09:01.000000 dpt-1.0.4/dpt/storage.py
-drwxrwxrwx   0        0        0        0 2024-06-01 01:11:30.033809 dpt-1.0.4/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-06-01 01:11:29.000000 dpt-1.0.4/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-06-01 01:11:29.000000 dpt-1.0.4/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 01:11:29.000000 dpt-1.0.4/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-06-01 01:11:29.000000 dpt-1.0.4/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-06-01 01:11:29.000000 dpt-1.0.4/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 01:11:30.066807 dpt-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-06-01 01:11:25.000000 dpt-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.184159 dpt-1.0.5/
+-rw-rw-rw-   0        0        0      188 2024-06-02 15:18:58.183127 dpt-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.140282 dpt-1.0.5/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.5/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.172588 dpt-1.0.5/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.5/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.5/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.5/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.5/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.5/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.180584 dpt-1.0.5/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.5/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.5/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.5/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.5/dpt/processor.py
+-rw-rw-rw-   0        0        0     7435 2024-06-02 15:16:39.000000 dpt-1.0.5/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:18:58.165360 dpt-1.0.5/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-06-02 15:18:58.000000 dpt-1.0.5/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:18:58.184159 dpt-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-06-02 15:18:15.000000 dpt-1.0.5/setup.py
```

### Comparing `dpt-1.0.4/dpt/deployment/deploy.py` & `dpt-1.0.5/dpt/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.4/dpt/deployment/extract.py` & `dpt-1.0.5/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.4/dpt/management.py` & `dpt-1.0.5/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.4/dpt/mongo/files.py` & `dpt-1.0.5/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.4/dpt/processor.py` & `dpt-1.0.5/dpt/processor.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.4/dpt/storage.py` & `dpt-1.0.5/dpt/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,26 @@
 
 
 class CollectionInfo:
     def __init__(self, collectionName: str, database: DatabaseInfo):
         self._collection_name = collectionName
         self.name = collectionName
         self.database = database
-        self._count = 0
+        self._count = None
         # if self.database == None:
         #     self.database = Database()
         self._instance = None
 
     def get_count(self):
+        if self._count == None:
+            self._update_count_from_collection()
         return self._count
+    
+    def get_collection_name(self):
+        return self.name
 
     def get_info(self):
         return f"collection '{self.name}'"
 
     def instance(self) -> Collection:
         if self._instance == None:
             self._instance = self.database.instance()[self.name]
@@ -161,14 +166,17 @@
         if self.schema == None:
             return
         for item in self._data:
             jsonschema.validate(instance=item, schema=self.schema)
 
     def get_count(self):
         return len(self._data)
+    
+    def get_collection_name(self):
+        return None
 
     def get_info(self):
         return f"list[]"
 
     def read_all(self):
         self._validate()
         print(f"read {len(self._data)} documents from {self.get_info()}")
```

