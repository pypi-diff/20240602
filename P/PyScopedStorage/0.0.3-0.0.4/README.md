# Comparing `tmp/pyscopedstorage-0.0.3.tar.gz` & `tmp/pyscopedstorage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscopedstorage-0.0.3.tar", max compression
+gzip compressed data, was "pyscopedstorage-0.0.4.tar", max compression
```

## Comparing `pyscopedstorage-0.0.3.tar` & `pyscopedstorage-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.3/LICENSE
--rw-r--r--   0        0        0     3200 2024-05-08 01:25:11.149763 pyscopedstorage-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       59 2024-05-08 00:56:10.748860 pyscopedstorage-0.0.3/src/PyScopedStorage/__init__.py
--rw-r--r--   0        0        0      496 2024-05-07 16:10:47.864603 pyscopedstorage-0.0.3/src/PyScopedStorage/android_objects.py
--rw-r--r--   0        0        0     2870 2024-04-29 16:44:18.965900 pyscopedstorage-0.0.3/src/PyScopedStorage/filechooser.py
--rw-r--r--   0        0        0      266 2024-04-13 10:37:21.713902 pyscopedstorage-0.0.3/src/PyScopedStorage/io.py
--rw-r--r--   0        0        0     2617 2024-05-07 23:46:46.622090 pyscopedstorage-0.0.3/src/PyScopedStorage/tools.py
--rw-r--r--   0        0        0     3567 2024-05-10 01:31:20.716536 pyscopedstorage-0.0.3/src/PyScopedStorage/utils.py
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3200 2024-05-10 01:39:00.228511 pyscopedstorage-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-06-03 16:44:53.027181 pyscopedstorage-0.0.4/src/PyScopedStorage/__init__.py
+-rw-r--r--   0        0        0      567 2024-06-03 17:34:45.702245 pyscopedstorage-0.0.4/src/PyScopedStorage/android_objects.py
+-rw-r--r--   0        0        0     2880 2024-06-03 16:44:30.973180 pyscopedstorage-0.0.4/src/PyScopedStorage/filechooser.py
+-rw-r--r--   0        0        0      266 2024-04-13 10:37:21.713902 pyscopedstorage-0.0.4/src/PyScopedStorage/io.py
+-rw-r--r--   0        0        0     3319 2024-06-03 17:44:38.840258 pyscopedstorage-0.0.4/src/PyScopedStorage/tools.py
+-rw-r--r--   0        0        0     4203 2024-06-03 17:41:27.339254 pyscopedstorage-0.0.4/src/PyScopedStorage/utils.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.4/PKG-INFO
```

### Comparing `pyscopedstorage-0.0.3/LICENSE` & `pyscopedstorage-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.3/pyproject.toml` & `pyscopedstorage-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyScopedStorage"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library to simplify storage interaction in Android apps."
 # readme = "README.md"  # TODO..
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `pyscopedstorage-0.0.3/src/PyScopedStorage/filechooser.py` & `pyscopedstorage-0.0.4/src/PyScopedStorage/filechooser.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,28 +45,28 @@
 
 
 def pyss_open_dir(**kwargs: dict[str, Any]) -> None:
 	filechooser._handle_selection = kwargs.pop(  # noqa: SLF001
 		'on_selection', filechooser._handle_selection,  # noqa: SLF001
 	)
 
-	intent: 'android.content.Intent' = Intent(Intent.ACTION_OPEN_DOCUMENT_TREE)
+	intent: 'jni[android.content.Intent]' = Intent(Intent.ACTION_OPEN_DOCUMENT_TREE)
 
 	# TODO: Handle persistent req
 
 	mActivity.startActivityForResult(intent, filechooser.select_code)
 
 	del intent
 
 
 def pyss_on_activity_result(self, request_code: int, result_code: int, data: Intent) -> None:
 	sel = self.selection_raw if not isinstance(self.selection_raw, list) else self.selection_raw[0]
 	# FIXME: Clean `self.selection_raw`
 	# TODO: Ignore on file calls..?
-	resolver: 'android.content.ContentResolver' = mActivity.getContentResolver()
+	resolver: 'jni[android.content.ContentResolver]' = mActivity.getContentResolver()
 	resolver.takePersistableUriPermission(
 		sel,
 		# TODO: Make flags as option..
 		Intent.FLAG_GRANT_READ_URI_PERMISSION | Intent.FLAG_GRANT_WRITE_URI_PERMISSION,
 	)
 
 	del resolver
```

### Comparing `pyscopedstorage-0.0.3/src/PyScopedStorage/tools.py` & `pyscopedstorage-0.0.4/src/PyScopedStorage/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 
 from os import fdopen as os_fdopen
 from typing import TYPE_CHECKING
 
 from plyer.utils import platform
 
 if platform == 'android':
-	from .android_objects import ContentProvider, ContentResolver, DocumentsContract
+	from .android_objects import ContentProvider, ContentResolver, DCDocument, DocumentsContract
 
 from .io import async_open
-from .utils import generate_file_uri_from_access_uri, get_fd_from_android_uri, scoped_file_exists
+from .utils import generate_file_uri_from_access_uri, get_fd_from_android_uri, scoped_uri_exists
 
 if TYPE_CHECKING:
 	from io import BufferedReader, BufferedWriter, TextIOWrapper
 
 	from aiofiles.threadpool.binary import AsyncBufferedIOBase, AsyncBufferedReader
 	from aiofiles.threadpool.text import AsyncTextIOWrapper
 
 
 def scoped_file_open(
-	access_uri: 'android.net.Uri',
+	access_uri: 'jni[android.net.Uri]',
 	name: str,
 	mode: str = 'w',
 	mime: str = '*/*',
 ) -> int:
 	"""Make file using access (usually directory) android uri and return the file descriptor."""
 	# TODO: Optionally return file uri
-	file_uri: 'android.net.Uri' = generate_file_uri_from_access_uri(access_uri, name)
-	if scoped_file_exists(file_uri):
+	file_uri: 'jni[android.net.Uri]' = generate_file_uri_from_access_uri(access_uri, name)
+	if scoped_uri_exists(file_uri):
 		if mode == 'x':
-			del file_uri
 			raise FileExistsError
 
 	elif mode in ('r', 'rb', 'r+', 'rb+'):
 		raise FileNotFoundError
 
 	else:
 		del file_uri
@@ -42,38 +41,37 @@
 		file_uri = dc_make_doc(
 			access_uri,
 			name, mime,
 		)
 
 
 	ret = get_fd_from_android_uri(file_uri, mode)
-	del file_uri
 
 	return ret
 
 
 def dc_make_doc(
-	access_uri: 'android.net.Uri',
+	access_uri: 'jni[android.net.Uri]',
 	name: str,
 	mime: str = '*/*',
-) -> 'android.net.Uri':
+) -> 'jni[android.net.Uri]':
 	"""Make file using access (usually directory) android uri and return the file uri."""
 	# TODO: Optionally return file uri
 	# TODO: Raise error if file exists..
 	return DocumentsContract.createDocument(
 		ContentResolver,
 		access_uri,
 		mime, name,
 	)
 
 
 def dc_open_doc(
-	access_uri: 'android.net.Uri',
+	access_uri: 'jni[android.net.Uri]',
 	name: str,
-) -> 'android.net.Uri':
+) -> 'jni[android.net.Uri]':
 	"""Open file using access (usually directory) android uri and return the file uri."""
 	# TODO: Optionally return file uri
 	# FIXME: Raise error if file exists..
 	return ContentProvider.createDocument(
 		ContentResolver,
 		access_uri,
 		mime, name,
@@ -94,9 +92,40 @@
 	name: str,
 	mode: str = 'w',
 	mime: str = '*/*',
 ) -> AsyncTextIOWrapper | AsyncBufferedReader | AsyncBufferedIOBase:
 	return async_open(scoped_file_open(access_uri, name, mode, mime), mode)
 
 
+class DirectoryExistsError(FileExistsError):
+	pass
+
+
+def scoped_mkdir_sync(
+	access_uri: 'jni[android.net.Uri]',
+	name: str,
+	*,
+	exist_ok: bool = False,
+) -> 'jni[android.net.Uri]':
+	# Why Google doesn't made separate method for this stuff?
+	uri = DocumentsContract.createDocument(
+		ContentResolver,
+		access_uri, DCDocument.MIME_TYPE_DIR, name,
+	)
+	if scoped_uri_exists(uri) and not exist_ok:
+		# TODO: More informative message..
+		raise DirectoryExistsError
+	return uri
+
+
+async def scoped_mkdir_async(
+	access_uri: 'android.net.Uri',
+	name: str,
+) -> 'jni[android.net.Uri]':
+	return scoped_mkdir_sync(access_uri, name)
+
+
 sfopen_sync = scoped_file_open_sync
 sfopen_async = scoped_file_open_async
+
+smkdir_sync = scoped_mkdir_sync
+smkdir_async = scoped_mkdir_async
```

### Comparing `pyscopedstorage-0.0.3/src/PyScopedStorage/utils.py` & `pyscopedstorage-0.0.4/src/PyScopedStorage/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,30 +3,56 @@
 from typing import TYPE_CHECKING
 
 from plyer.utils import platform
 
 if platform == 'android':
 	from jnius.jnius import JavaException
 
-	from .android_objects import ContentResolver, DocumentsContract, Uri
+	from .android_objects import ContentResolver, DCDocument, DocumentsContract, Uri
 
 PYSLET_AVAILABLE: bool = True
 
 try:
 	from pyslet.rfc2396 import URI
 except ImportError:
 	PYSLET_AVAILABLE = False
 
 if TYPE_CHECKING:
 	from typing import Dict, Final  # noqa: UP035
 
 	from pyslet.rfc2396 import URI
 
 
-def scoped_file_exists(file_uri: 'android.net.Uri') -> bool:
+def scoped_uri_exists(file_uri: 'jni[android.net.Uri]') -> bool:
+	c: 'jni[android.database.Cursor] | None' = None
+	try:
+		c = ContentResolver.query(
+			file_uri,
+			(DCDocument.COLUMN_DOCUMENT_ID,),
+			# [DCDocument.COLUMN_DOCUMENT_ID],
+			None, None, None,
+		)
+		return c.getCount() > 0
+	except JavaException as e:
+		if e.innermessage is None or 'java.io.FileNotFoundException' in e.innermessage:
+			# FIXME: Log fail..
+			del e
+			return False
+
+		raise e
+
+	# All's fine
+	# TODO: Quite close like in `DocumentsContractApi19.java`
+	if c is not None:
+		c.close()
+
+	return True
+
+
+def _old_scoped_file_exists(file_uri: 'jni[android.net.Uri]') -> bool:
 	try:
 		ins = ContentResolver.openInputStream(file_uri)
 	except JavaException as e:
 		if 'java.io.FileNotFoundException' in e.innermessage:
 			del e
 			return False
 
@@ -80,15 +106,15 @@
 	"""
 	# TODO: CancellationSignal..
 
 	# Stuff around modes to correctly use in the java descriptor
 	# TODO: Raise another error..
 	jp_mode = py_open2java_openfd[mode]
 
-	fd_obj: 'android.os.ParcelFileDescriptor' = ContentResolver.openFileDescriptor(
+	fd_obj: 'jni[android.os.ParcelFileDescriptor]' = ContentResolver.openFileDescriptor(
 		content_uri,
 		jp_mode,
 	)
 	fd: int = fd_obj.detachFd()
 
 	return fd
 
@@ -107,15 +133,18 @@
 ) -> int:
 	android_uri: 'android.net.Uri' = Uri.parse(struri)
 	return get_fd_from_android_uri(android_uri, mode)
 
 
 # TODO: Speed check..
 # Weak.. Do we really need pyslet's rfc2396?
-# def _pyslet_generate_file_uri_from_access_uri(access_uri: 'android.net.Uri', name: str) -> 'android.net.Uri':
+# def _pyslet_generate_file_uri_from_access_uri(
+	# access_uri: 'jni[android.net.Uri]',
+# 	name: str,
+# ) -> 'jni[android.net.Uri]':
 # 	py_uri: URI = URI(access_uri.toString())
 # 	doc_file: str = f'{py_uri.get_file_name()}/{name}'
 
 # 	# FIXME: Find better ways to natively use rfc2396 Uri..
 # 	# py_file_uri: str = str(py_uri.resolve(doc_file))##
 # 	# ret = Uri.parse(py_file_uri)
 
@@ -123,15 +152,15 @@
 
 # 	del py_uri, doc_file
 
 # 	return ret
 
 
 # TODO: Handle parse errors..
-def generate_file_uri_from_access_uri(access_uri: 'android.net.Uri', name: str) -> 'android.net.Uri':
+def generate_file_uri_from_access_uri(access_uri: 'jni[android.net.Uri]', name: str) -> 'jni[android.net.Uri]':
 	dir_name: str = DocumentsContract.getTreeDocumentId(access_uri)
 	doc_file: str = f'{dir_name}/{name}'
 	del dir_name
 
 	ret = DocumentsContract.buildDocumentUriUsingTree(access_uri, doc_file)
 
 	del doc_file
```

### Comparing `pyscopedstorage-0.0.3/PKG-INFO` & `pyscopedstorage-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScopedStorage
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library to simplify storage interaction in Android apps.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

