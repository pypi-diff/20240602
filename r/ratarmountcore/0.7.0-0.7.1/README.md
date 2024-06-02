# Comparing `tmp/ratarmountcore-0.7.0.tar.gz` & `tmp/ratarmountcore-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratarmountcore-0.7.0.tar", last modified: Sun Apr  7 13:35:31 2024, max compression
+gzip compressed data, was "ratarmountcore-0.7.1.tar", last modified: Sun Jun  2 19:55:06 2024, max compression
```

## Comparing `ratarmountcore-0.7.0.tar` & `ratarmountcore-0.7.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.718862 ratarmountcore-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-07 13:35:31.718862 ratarmountcore-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.710862 ratarmountcore-0.7.0/ratarmountcore/
--rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/AutoMountLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/BlockParallelReaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/FileVersionLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/FolderMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    29124 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/LibarchiveMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/MountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/RarMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SQLiteBlobFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    57126 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SQLiteIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)    78386 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SQLiteIndexedTar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SingleFileMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/StenciledFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SubvolumesMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/UnionMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/ZipMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/compressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.714861 ratarmountcore-0.7.0/ratarmountcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-07 13:35:31.718862 ratarmountcore-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.714861 ratarmountcore-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_AutoMountLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_BlockParallelReaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_LibarchiveMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_RarMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SQLiteBlobFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SQLiteIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)    22938 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SQLiteIndexedTar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_StenciledFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SubvolumesMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_UnionMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_ZipMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_compressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:06.173910 ratarmountcore-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-06-02 19:55:06.173910 ratarmountcore-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:06.169910 ratarmountcore-0.7.1/ratarmountcore/
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/AutoMountLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/BlockParallelReaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/FileVersionLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/FolderMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29592 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/LibarchiveMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/MountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/RarMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/SQLiteBlobFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57170 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/SQLiteIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78394 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/SQLiteIndexedTar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/SingleFileMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/StenciledFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/SubvolumesMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/UnionMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/ZipMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20343 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/compressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/ratarmountcore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:06.173910 ratarmountcore-0.7.1/ratarmountcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-06-02 19:55:06.000000 ratarmountcore-0.7.1/ratarmountcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-06-02 19:55:06.000000 ratarmountcore-0.7.1/ratarmountcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:55:06.000000 ratarmountcore-0.7.1/ratarmountcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-06-02 19:55:06.000000 ratarmountcore-0.7.1/ratarmountcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 19:55:06.000000 ratarmountcore-0.7.1/ratarmountcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-06-02 19:55:06.173910 ratarmountcore-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:55:06.173910 ratarmountcore-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_AutoMountLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_BlockParallelReaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_LibarchiveMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_RarMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_SQLiteBlobFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_SQLiteIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22938 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_SQLiteIndexedTar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_StenciledFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_SubvolumesMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_UnionMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_ZipMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_compressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-06-02 19:54:56.000000 ratarmountcore-0.7.1/tests/test_utils.py
```

### Comparing `ratarmountcore-0.7.0/LICENSE` & `ratarmountcore-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/PKG-INFO` & `ratarmountcore-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratarmountcore
-Version: 0.7.0
+Version: 0.7.1
 Summary: Random Access Read-Only Tar Mount Library
 Home-page: https://github.com/mxmlnkn/ratarmount/ratarmountcore
 Author: Maximilian Knespel
 Author-email: mxmlnkn@github.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ratarmountcore-0.7.0/README.md` & `ratarmountcore-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/AutoMountLayer.py` & `ratarmountcore-0.7.1/ratarmountcore/AutoMountLayer.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/BlockParallelReaders.py` & `ratarmountcore-0.7.1/ratarmountcore/BlockParallelReaders.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/FileVersionLayer.py` & `ratarmountcore-0.7.1/ratarmountcore/FileVersionLayer.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/FolderMountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/FolderMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/LibarchiveMountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/LibarchiveMountSource.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .SQLiteIndex import SQLiteIndex, SQLiteIndexedTarUserData
 from .utils import InvalidIndexError, overrides
 
 try:
     # Use the FFI directly because the higher-level interface does not work sufficiently for our use case.
     import libarchive.ffi as laffi
     from libarchive.exception import ArchiveError
-except ImportError:
+except (ImportError, AttributeError):
     pass
 
 
 class ArchiveEntry:
     def __init__(self, archive, entryIndex: int, encoding: str = 'utf-8'):
         self._archive = archive  # Store for lifetime
         self._entry = laffi.entry_new()
@@ -159,21 +159,23 @@
 
 class IterableArchive:
     """A class that opens an archive with libarchive and can iterate over the entries."""
 
     # Read formats list supported by python-libarchive-c:
     #   '7zip', 'all', 'ar', 'cab', 'cpio', 'empty', 'iso9660', 'lha', 'mtree',
     #   'rar', 'raw', 'tar', 'xar', 'zip', 'warc'
-    # We especially do not want mtree because it has not magic bytes and basically matches anything with newlines,
+    # We especially do not want mtree because it has no magic bytes and basically matches anything with newlines,
     # including some test text files. 'raw', 'empty', and 'all' are special input formats.
     # It seems that 'raw' cannot be combined in an or-manner. It disables all archive format recognitions and only
     # applies the filters.
     # https://github.com/libarchive/libarchive/wiki/FormatRaw#caveat-dont-mix-_raw_-with-other-handlers
     # > aveat: Don't mix _raw_ with other handlers
     # > If you are using the raw handler, you should generally not enable any other handler
+    # Note that the lz4 and zstd filters are not available in the manylinux2014 container (CentOS Linux
+    # release 7.9.2009 (Core))
     ENABLED_FORMATS = ['7zip', 'ar', 'cab', 'cpio', 'iso9660', 'lha', 'rar', 'rar5', 'tar', 'xar', 'warc', 'zip']
 
     def __init__(
         self,
         file: Union[str, IO[bytes]],
         encoding='utf-8',
         passwords: Optional[List[str]] = None,
@@ -212,15 +214,20 @@
         allNames = [laffi.filter_name(self._archive, i) for i in range(laffi.filter_count(self._archive))]
         return [name for name in allNames if name != b'none']
 
     def _tryToOpen(self, allowArchives: bool):
         laffi.get_read_filter_function('all')(self._archive)
 
         for formatToEnable in IterableArchive.ENABLED_FORMATS if allowArchives else ['raw']:
-            laffi.get_read_format_function(formatToEnable)(self._archive)
+            try:
+                laffi.get_read_format_function(formatToEnable)(self._archive)
+            except ValueError as exception:
+                # Ignore exceptions from formats that are not supported such as "rar5" in manylinux2014.
+                if self.printDebug >= 3:
+                    print(f"[Warning] Failed to enable format {formatToEnable} because of: {exception}")
 
         if isinstance(self._file, str):
             laffi.read_open_filename_w(self._archive, self._file, os.stat(self._file).st_blksize)
         elif isinstance(self._file, int):
             laffi.read_open_fd(self._archive, self._file, os.fstat(self._file).st_blksize)
         elif hasattr(self._file, 'readinto'):
             self._openWithFileObject()
```

### Comparing `ratarmountcore-0.7.0/ratarmountcore/MountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/MountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/ProgressBar.py` & `ratarmountcore-0.7.1/ratarmountcore/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/RarMountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/RarMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/SQLiteBlobFile.py` & `ratarmountcore-0.7.1/ratarmountcore/SQLiteBlobFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/SQLiteIndex.py` & `ratarmountcore-0.7.1/ratarmountcore/SQLiteIndex.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,18 +945,18 @@
                 indexVersion = self.sqlConnection.execute(
                     "SELECT major,minor FROM versions WHERE name == 'index';"
                 ).fetchone()
 
                 if indexVersion:
                     indexVersionTuple = _toVersionTuple(indexVersion)
                     indexAPIVersionTuple = _toVersionTuple(SQLiteIndex.__version__)
-                if indexVersionTuple and indexAPIVersionTuple and indexVersionTuple > indexAPIVersionTuple:
-                    print("[Warning] The loaded index was created with a newer version of ratarmount.")
-                    print("[Warning] If there are any problems, please update ratarmount or recreate the index")
-                    print("[Warning] with this ratarmount version using the --recreate-index option!")
+                    if indexVersionTuple and indexAPIVersionTuple and indexVersionTuple > indexAPIVersionTuple:
+                        print("[Warning] The loaded index was created with a newer version of ratarmount.")
+                        print("[Warning] If there are any problems, please update ratarmount or recreate the index")
+                        print("[Warning] with this ratarmount version using the --recreate-index option!")
             except Exception:
                 pass
 
         if self.printDebug >= 1:
             print(f"Successfully loaded offset dictionary from {str(indexFilePath)}")
 
     def _tryLoadIndex(self, indexFilePath: AnyStr) -> bool:
@@ -1033,14 +1033,15 @@
             setBlockOffsets = getattr(fileObject, 'set_block_offsets')
             getBlockOffsets = getattr(fileObject, 'block_offsets')
             if not setBlockOffsets or not getBlockOffsets:
                 print("[Warning] The given file object misses the expected methods for getting/setting")
                 print("[Warning] the block offsets. Subsequent loads might be slow.")
                 return
 
+            table_name = ''
             if compression == 'bz2':
                 table_name = 'bzip2blocks'
             elif compression == 'zst':
                 table_name = 'zstdblocks'
 
             tables = getSqliteTables(db)
             if table_name in tables:
```

### Comparing `ratarmountcore-0.7.0/ratarmountcore/SQLiteIndexedTar.py` & `ratarmountcore-0.7.1/ratarmountcore/SQLiteIndexedTar.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,16 +397,16 @@
                     self._parent._isGnuIncremental = True
                     if self._parent.printDebug >= 1:
                         print("[Warning] A folder metadata entry for GNU incremental archives")
                         print("[Warning] was encountered but this archive was not automatically recognized as such!")
                         print("[Warning] Please call ratarmount with the --gnu-incremental flag if there are problems.")
                         print()
 
-            tarBlocks.append(offset)
-            processedFiles += 1
+                tarBlocks.append(offset)
+                processedFiles += 1
 
             if len(tarBlocks) >= 10000 or (result is None and len(tarBlocks) > 0):
                 if result is None:
                     tarBlocks.append(fileObject.tell())
 
                 startOffset = tarBlocks[0]
                 subSize = tarBlocks[-1] - tarBlocks[0]
```

### Comparing `ratarmountcore-0.7.0/ratarmountcore/SingleFileMountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/SingleFileMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/StenciledFile.py` & `ratarmountcore-0.7.1/ratarmountcore/StenciledFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,16 +310,16 @@
         if whence == io.SEEK_CUR:
             self.offset += offset
         elif whence == io.SEEK_END:
             self.offset = self.cumsizes[-1] + offset
         elif whence == io.SEEK_SET:
             self.offset = offset
 
-        if self.offset < 0:
-            raise ValueError("Trying to seek before the start of the file!")
+        # Same behavior for seeking before the file begin and after the file end as io.BytesIO.
+        self.offset = max(self.offset, 0)
         if self.offset >= self.cumsizes[-1]:
             return self.offset
 
         return self.offset
 
     @overrides(io.RawIOBase)
     def tell(self) -> int:
```

### Comparing `ratarmountcore-0.7.0/ratarmountcore/SubvolumesMountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/SubvolumesMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/UnionMountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/UnionMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/ZipMountSource.py` & `ratarmountcore-0.7.1/ratarmountcore/ZipMountSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,21 +164,14 @@
         self.index.finalize()
 
         t1 = timer()
         if self.printDebug >= 1:
             print(f"Creating offset dictionary for {self.archiveFilePath} took {t1 - t0:.2f}s")
 
     @staticmethod
-    def _cleanPath(path):
-        result = os.path.normpath(path) + ('/' if path.endswith('/') else '')
-        while result.startswith('../'):
-            result = result[3:]
-        return result
-
-    @staticmethod
     def _findPassword(fileobj: "zipfile.ZipFile", passwords):
         # If headers are encrypted, then infolist will simply return an empty list!
         files = fileobj.infolist()
         if not files:
             for password in passwords:
                 fileobj.setpassword(password)
                 files = fileobj.infolist()
```

### Comparing `ratarmountcore-0.7.0/ratarmountcore/__init__.py` & `ratarmountcore-0.7.1/ratarmountcore/__init__.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/compressions.py` & `ratarmountcore-0.7.1/ratarmountcore/compressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     import zipfile
 else:
     zipfile = None
 
 
 try:
     import libarchive
-except ImportError:
+except (ImportError, AttributeError):
     libarchive = None
 
 
 CompressionModuleInfo = collections.namedtuple('CompressionModuleInfo', ['name', 'open'])
 # Defining lambdas does not yet check the names of entities used inside the lambda!
 # "modules" contains a list of CompressionModuleInfo for modules that are available.
 # Those appearing first in this list have priority.
```

### Comparing `ratarmountcore-0.7.0/ratarmountcore/factory.py` & `ratarmountcore-0.7.1/ratarmountcore/factory.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore/utils.py` & `ratarmountcore-0.7.1/ratarmountcore/utils.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore.egg-info/PKG-INFO` & `ratarmountcore-0.7.1/ratarmountcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratarmountcore
-Version: 0.7.0
+Version: 0.7.1
 Summary: Random Access Read-Only Tar Mount Library
 Home-page: https://github.com/mxmlnkn/ratarmount/ratarmountcore
 Author: Maximilian Knespel
 Author-email: mxmlnkn@github.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ratarmountcore-0.7.0/ratarmountcore.egg-info/SOURCES.txt` & `ratarmountcore-0.7.1/ratarmountcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/ratarmountcore.egg-info/requires.txt` & `ratarmountcore-0.7.1/ratarmountcore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/setup.cfg` & `ratarmountcore-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/setup.py` & `ratarmountcore-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_AutoMountLayer.py` & `ratarmountcore-0.7.1/tests/test_AutoMountLayer.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_BlockParallelReaders.py` & `ratarmountcore-0.7.1/tests/test_BlockParallelReaders.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_LibarchiveMountSource.py` & `ratarmountcore-0.7.1/tests/test_LibarchiveMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_RarMountSource.py` & `ratarmountcore-0.7.1/tests/test_RarMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_SQLiteBlobFile.py` & `ratarmountcore-0.7.1/tests/test_SQLiteBlobFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_SQLiteIndex.py` & `ratarmountcore-0.7.1/tests/test_SQLiteIndex.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_SQLiteIndexedTar.py` & `ratarmountcore-0.7.1/tests/test_SQLiteIndexedTar.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_StenciledFile.py` & `ratarmountcore-0.7.1/tests/test_StenciledFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_SubvolumesMountSource.py` & `ratarmountcore-0.7.1/tests/test_SubvolumesMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_UnionMountSource.py` & `ratarmountcore-0.7.1/tests/test_UnionMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_ZipMountSource.py` & `ratarmountcore-0.7.1/tests/test_ZipMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_compressions.py` & `ratarmountcore-0.7.1/tests/test_compressions.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_factory.py` & `ratarmountcore-0.7.1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.7.0/tests/test_utils.py` & `ratarmountcore-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

