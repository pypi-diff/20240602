# Comparing `tmp/pyscopedstorage-0.0.4.tar.gz` & `tmp/pyscopedstorage-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscopedstorage-0.0.4.tar", max compression
+gzip compressed data, was "pyscopedstorage-0.0.5.tar", max compression
```

## Comparing `pyscopedstorage-0.0.4.tar` & `pyscopedstorage-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.4/LICENSE
--rw-r--r--   0        0        0     3200 2024-05-10 01:39:00.228511 pyscopedstorage-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       98 2024-06-03 16:44:53.027181 pyscopedstorage-0.0.4/src/PyScopedStorage/__init__.py
--rw-r--r--   0        0        0      567 2024-06-03 17:34:45.702245 pyscopedstorage-0.0.4/src/PyScopedStorage/android_objects.py
--rw-r--r--   0        0        0     2880 2024-06-03 16:44:30.973180 pyscopedstorage-0.0.4/src/PyScopedStorage/filechooser.py
--rw-r--r--   0        0        0      266 2024-04-13 10:37:21.713902 pyscopedstorage-0.0.4/src/PyScopedStorage/io.py
--rw-r--r--   0        0        0     3319 2024-06-03 17:44:38.840258 pyscopedstorage-0.0.4/src/PyScopedStorage/tools.py
--rw-r--r--   0        0        0     4203 2024-06-03 17:41:27.339254 pyscopedstorage-0.0.4/src/PyScopedStorage/utils.py
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3200 2024-06-03 17:46:56.927260 pyscopedstorage-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-06-03 16:44:53.027181 pyscopedstorage-0.0.5/src/PyScopedStorage/__init__.py
+-rw-r--r--   0        0        0      567 2024-06-03 17:34:45.702245 pyscopedstorage-0.0.5/src/PyScopedStorage/android_objects.py
+-rw-r--r--   0        0        0     2880 2024-06-03 16:44:30.973180 pyscopedstorage-0.0.5/src/PyScopedStorage/filechooser.py
+-rw-r--r--   0        0        0      314 2024-06-03 18:01:06.731279 pyscopedstorage-0.0.5/src/PyScopedStorage/io.py
+-rw-r--r--   0        0        0     3193 2024-06-03 18:01:45.979280 pyscopedstorage-0.0.5/src/PyScopedStorage/tools.py
+-rw-r--r--   0        0        0     4203 2024-06-03 17:45:46.489259 pyscopedstorage-0.0.5/src/PyScopedStorage/utils.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.5/PKG-INFO
```

### Comparing `pyscopedstorage-0.0.4/LICENSE` & `pyscopedstorage-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.4/pyproject.toml` & `pyscopedstorage-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyScopedStorage"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python library to simplify storage interaction in Android apps."
 # readme = "README.md"  # TODO..
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `pyscopedstorage-0.0.4/src/PyScopedStorage/android_objects.py` & `pyscopedstorage-0.0.5/src/PyScopedStorage/android_objects.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.4/src/PyScopedStorage/filechooser.py` & `pyscopedstorage-0.0.5/src/PyScopedStorage/filechooser.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.4/src/PyScopedStorage/tools.py` & `pyscopedstorage-0.0.5/src/PyScopedStorage/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import TYPE_CHECKING
 
 from plyer.utils import platform
 
 if platform == 'android':
 	from .android_objects import ContentProvider, ContentResolver, DCDocument, DocumentsContract
 
-from .io import async_open
-from .utils import generate_file_uri_from_access_uri, get_fd_from_android_uri, scoped_uri_exists
+from .io import async_open, wrap2async
+from .utils import generate_file_uri_from_access_uri, get_fd_from_android_uri, scoped_res_exists
 
 if TYPE_CHECKING:
 	from io import BufferedReader, BufferedWriter, TextIOWrapper
 
 	from aiofiles.threadpool.binary import AsyncBufferedIOBase, AsyncBufferedReader
 	from aiofiles.threadpool.text import AsyncTextIOWrapper
 
@@ -23,15 +23,15 @@
 	name: str,
 	mode: str = 'w',
 	mime: str = '*/*',
 ) -> int:
 	"""Make file using access (usually directory) android uri and return the file descriptor."""
 	# TODO: Optionally return file uri
 	file_uri: 'jni[android.net.Uri]' = generate_file_uri_from_access_uri(access_uri, name)
-	if scoped_uri_exists(file_uri):
+	if scoped_res_exists(file_uri):
 		if mode == 'x':
 			raise FileExistsError
 
 	elif mode in ('r', 'rb', 'r+', 'rb+'):
 		raise FileNotFoundError
 
 	else:
@@ -107,25 +107,18 @@
 	exist_ok: bool = False,
 ) -> 'jni[android.net.Uri]':
 	# Why Google doesn't made separate method for this stuff?
 	uri = DocumentsContract.createDocument(
 		ContentResolver,
 		access_uri, DCDocument.MIME_TYPE_DIR, name,
 	)
-	if scoped_uri_exists(uri) and not exist_ok:
+	if scoped_res_exists(uri) and not exist_ok:
 		# TODO: More informative message..
 		raise DirectoryExistsError
 	return uri
 
 
-async def scoped_mkdir_async(
-	access_uri: 'android.net.Uri',
-	name: str,
-) -> 'jni[android.net.Uri]':
-	return scoped_mkdir_sync(access_uri, name)
-
-
 sfopen_sync = scoped_file_open_sync
 sfopen_async = scoped_file_open_async
 
 smkdir_sync = scoped_mkdir_sync
-smkdir_async = scoped_mkdir_async
+smkdir_async = wrap2async(scoped_mkdir_sync)
```

### Comparing `pyscopedstorage-0.0.4/src/PyScopedStorage/utils.py` & `pyscopedstorage-0.0.5/src/PyScopedStorage/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 if TYPE_CHECKING:
 	from typing import Dict, Final  # noqa: UP035
 
 	from pyslet.rfc2396 import URI
 
 
-def scoped_uri_exists(file_uri: 'jni[android.net.Uri]') -> bool:
+def scoped_res_exists(file_uri: 'jni[android.net.Uri]') -> bool:
 	c: 'jni[android.database.Cursor] | None' = None
 	try:
 		c = ContentResolver.query(
 			file_uri,
 			(DCDocument.COLUMN_DOCUMENT_ID,),
 			# [DCDocument.COLUMN_DOCUMENT_ID],
 			None, None, None,
```

### Comparing `pyscopedstorage-0.0.4/PKG-INFO` & `pyscopedstorage-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScopedStorage
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library to simplify storage interaction in Android apps.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

