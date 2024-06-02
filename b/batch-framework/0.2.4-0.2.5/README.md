# Comparing `tmp/batch-framework-0.2.4.tar.gz` & `tmp/batch-framework-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-framework-0.2.4.tar", last modified: Sat Jun  1 07:50:15 2024, max compression
+gzip compressed data, was "batch-framework-0.2.5.tar", last modified: Sun Jun  2 13:36:29 2024, max compression
```

## Comparing `batch-framework-0.2.4.tar` & `batch-framework-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-01 07:49:28.000000 batch-framework-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-01 07:50:15.642428 batch-framework-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 07:49:28.000000 batch-framework-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework/filesystem/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/dropbox/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/filesystem/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/parallize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/rdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 07:49:28.000000 batch-framework-0.2.4/batch_framework/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 07:50:15.642428 batch-framework-0.2.4/batch_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 07:50:15.000000 batch-framework-0.2.4/batch_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 07:50:15.642428 batch-framework-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-01 07:49:28.000000 batch-framework-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:36:29.626569 batch-framework-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-02 13:35:46.000000 batch-framework-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-02 13:36:29.626569 batch-framework-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-02 13:35:46.000000 batch-framework-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:36:29.622569 batch-framework-0.2.5/batch_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:36:29.626569 batch-framework-0.2.5/batch_framework/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/filesystem/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:36:29.626569 batch-framework-0.2.5/batch_framework/filesystem/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/filesystem/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/filesystem/dropbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/filesystem/dropbox/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/filesystem/dropbox/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/filesystem/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/parallize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/rdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 13:35:46.000000 batch-framework-0.2.5/batch_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:36:29.626569 batch-framework-0.2.5/batch_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-02 13:36:29.000000 batch-framework-0.2.5/batch_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-06-02 13:36:29.000000 batch-framework-0.2.5/batch_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:36:29.000000 batch-framework-0.2.5/batch_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 13:36:29.000000 batch-framework-0.2.5/batch_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 13:36:29.000000 batch-framework-0.2.5/batch_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 13:36:29.626569 batch-framework-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-02 13:35:46.000000 batch-framework-0.2.5/setup.py
```

### Comparing `batch-framework-0.2.4/LICENSE` & `batch-framework-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/PKG-INFO` & `batch-framework-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.4
+Version: 0.2.5
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.4/batch_framework/adaptor.py` & `batch-framework-0.2.5/batch_framework/adaptor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/base.py` & `batch-framework-0.2.5/batch_framework/base.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/etl.py` & `batch-framework-0.2.5/batch_framework/etl.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/executor.py` & `batch-framework-0.2.5/batch_framework/executor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/filesystem/base.py` & `batch-framework-0.2.5/batch_framework/filesystem/base.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/filesystem/dropbox/config.py` & `batch-framework-0.2.5/batch_framework/filesystem/dropbox/config.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/filesystem/dropbox/dropbox.py` & `batch-framework-0.2.5/batch_framework/filesystem/dropbox/dropbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,24 @@
 
     def __init__(self, directory='/', chunksize=2000000):
         assert directory.startswith('/')
         root_fs = MyDropboxFS()
         super().__init__(DirFileSystem(directory, root_fs))
         self._chunksize = chunksize
 
-    def upload_core(self, file_obj: io.BytesIO, remote_path: str):
+    def upload_core(self, file_obj: io.BytesIO, remote_path: str, check: bool=False):
         """Upload file object
 
         Args:
             file_obj (io.BytesIO): file to be upload
             remote_path (str): remote file path
         """
         self._upload_core(file_obj, remote_path)
-        self._check_upload_success(file_obj, remote_path)
+        if check:
+            self._check_upload_success(file_obj, remote_path)
         file_obj.flush()
         file_obj.close()
 
     def _check_upload_success(self, file_obj: io.BytesIO, remote_path: str):
         download_data = self.download_core(remote_path)
         download_data.seek(0)
         file_obj.seek(0)
```

### Comparing `batch-framework-0.2.4/batch_framework/filesystem/dropbox/util.py` & `batch-framework-0.2.5/batch_framework/filesystem/dropbox/util.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/filesystem/local.py` & `batch-framework-0.2.5/batch_framework/filesystem/local.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/parallize.py` & `batch-framework-0.2.5/batch_framework/parallize.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/rdb.py` & `batch-framework-0.2.5/batch_framework/rdb.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework/storage.py` & `batch-framework-0.2.5/batch_framework/storage.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/batch_framework.egg-info/PKG-INFO` & `batch-framework-0.2.5/batch_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.4
+Version: 0.2.5
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.4/batch_framework.egg-info/SOURCES.txt` & `batch-framework-0.2.5/batch_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.4/setup.py` & `batch-framework-0.2.5/setup.py`

 * *Files identical despite different names*

