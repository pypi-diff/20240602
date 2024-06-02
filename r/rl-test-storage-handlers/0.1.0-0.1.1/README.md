# Comparing `tmp/rl_test_storage_handlers-0.1.0.tar.gz` & `tmp/rl_test_storage_handlers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_test_storage_handlers-0.1.0.tar", last modified: Sun Jun  2 08:07:33 2024, max compression
+gzip compressed data, was "rl_test_storage_handlers-0.1.1.tar", last modified: Sun Jun  2 15:34:12 2024, max compression
```

## Comparing `rl_test_storage_handlers-0.1.0.tar` & `rl_test_storage_handlers-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:07:33.042869 rl_test_storage_handlers-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 08:07:33.042869 rl_test_storage_handlers-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:07:33.030869 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:07:33.038869 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:07:33.038869 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/params/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/params/file_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/params/file_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/text_file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:07:33.042869 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/params/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/params/storage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/params/storage_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:07:33.042869 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 08:07:33.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-02 08:07:33.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 08:07:33.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 08:07:33.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 08:07:33.000000 rl_test_storage_handlers-0.1.0/rl_test_storage_handlers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 08:07:33.042869 rl_test_storage_handlers-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-06-02 08:07:19.000000 rl_test_storage_handlers-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.456725 rl_test_storage_handlers-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 15:34:12.456725 rl_test_storage_handlers-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.452725 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.456725 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.456725 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/params/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/params/file_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/text_file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.456725 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/params/storage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/params/storage_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:12.456725 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 15:34:12.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-02 15:34:12.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:34:12.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 15:34:12.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 15:34:12.000000 rl_test_storage_handlers-0.1.1/rl_test_storage_handlers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:34:12.456725 rl_test_storage_handlers-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-06-02 15:33:52.000000 rl_test_storage_handlers-0.1.1/setup.py
```

### Comparing `rl_test_storage_handlers-0.1.0/rl_test_storage_handlers/file/file_handler.py` & `rl_test_storage_handlers-0.1.1/rl_test_storage_handlers/file/file_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import logging
 from abc import abstractmethod
 
 from rl_test_common import Common
 
 from ..params.storage_data import StorageData
 from ..params.storage_destination import StorageDestination
 from ..storage_handler import StorageHandler
 from .params.file_data import FileData
 from .params.file_destination import FileDestination
 
 
 class FileHandler(StorageHandler):
+    __logger: logging.Logger = logging.getLogger(__name__)
+
     __common: Common = Common()
 
     @abstractmethod
     def write(self, destination: StorageDestination, data: StorageData) -> None:
         pass
 
     @abstractmethod
@@ -24,16 +27,20 @@
         file_path: str = self.__get_file_path(destination.get())
 
         with open(file_path, mode) as file:
             file.write(data.get())
 
     def _read(self, destination: FileDestination, mode: str) -> FileData:
         file_path: str = self.__get_file_path(destination.get())
-        data: FileData | None = None
+        data: FileData = FileData('')
 
-        with open(file_path, mode) as file:
-            data = FileData(file.read())
+        try:
+            with open(file_path, mode) as file:
+                data = FileData(file.read())
+
+        except FileNotFoundError:
+            self.__logger.error(f'File not found: {file_path}.')
 
         return data
 
     def __get_file_path(self, file_name: str) -> str:
         return f'{self.__common.user_files_root}/{file_name}'
```

### Comparing `rl_test_storage_handlers-0.1.0/rl_test_storage_handlers.egg-info/SOURCES.txt` & `rl_test_storage_handlers-0.1.1/rl_test_storage_handlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

