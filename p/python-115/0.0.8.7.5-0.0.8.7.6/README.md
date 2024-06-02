# Comparing `tmp/python_115-0.0.8.7.5.tar.gz` & `tmp/python_115-0.0.8.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.7.5.tar", max compression
+gzip compressed data, was "python_115-0.0.8.7.6.tar", max compression
```

## Comparing `python_115-0.0.8.7.5.tar` & `python_115-0.0.8.7.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.5/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.5/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.5/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.5/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     2394 2024-06-01 07:45:37.499962 python_115-0.0.8.7.5/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.5/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.5/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.5/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.5/p115/cmd/init.py
--rwxr-xr-x   0        0        0     9484 2024-06-01 07:45:44.611935 python_115-0.0.8.7.5/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2107 2024-06-01 06:14:01.276468 python_115-0.0.8.7.5/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.5/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.5/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.5/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.5/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.5/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.5/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.5/p115/component/cipher.py
--rwxr-xr-x   0        0        0   260065 2024-06-01 14:51:20.075255 python_115-0.0.8.7.5/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.5/p115/component/exception.py
--rwxr-xr-x   0        0        0    66187 2024-06-02 01:30:47.597931 python_115-0.0.8.7.5/p115/component/fs.py
--rwxr-xr-x   0        0        0    48250 2024-06-02 03:28:28.910469 python_115-0.0.8.7.5/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.7.5/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.7.5/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.5/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.7.5/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.5/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.5/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.5/p115/py.typed
--rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.5/p115/tool/__init__.py
--rw-r--r--   0        0        0     1687 2024-06-02 03:28:05.245667 python_115-0.0.8.7.5/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.7.5/readme.md
--rw-r--r--   0        0        0    36409 1970-01-01 00:00:00.000000 python_115-0.0.8.7.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.6/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.6/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.6/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.6/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     2394 2024-06-01 07:45:37.499962 python_115-0.0.8.7.6/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.6/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     9484 2024-06-01 07:45:44.611935 python_115-0.0.8.7.6/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2107 2024-06-01 06:14:01.276468 python_115-0.0.8.7.6/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.6/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.6/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.6/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   265176 2024-06-02 07:24:06.942442 python_115-0.0.8.7.6/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.6/p115/component/exception.py
+-rwxr-xr-x   0        0        0    69258 2024-06-02 07:24:57.713675 python_115-0.0.8.7.6/p115/component/fs.py
+-rwxr-xr-x   0        0        0    49142 2024-06-02 06:13:46.742966 python_115-0.0.8.7.6/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    15205 2024-06-02 05:55:36.365281 python_115-0.0.8.7.6/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10263 2024-06-02 05:51:11.710739 python_115-0.0.8.7.6/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.6/p115/component/labellist.py
+-rwxr-xr-x   0        0        0    10286 2024-06-02 06:30:40.250415 python_115-0.0.8.7.6/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.6/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.6/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.6/p115/py.typed
+-rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.6/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1687 2024-06-02 07:25:34.828005 python_115-0.0.8.7.6/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-06-02 05:53:33.629676 python_115-0.0.8.7.6/readme.md
+-rw-r--r--   0        0        0    36409 1970-01-01 00:00:00.000000 python_115-0.0.8.7.6/PKG-INFO
```

### Comparing `python_115-0.0.8.7.5/LICENSE` & `python_115-0.0.8.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/cmd/check.py` & `python_115-0.0.8.7.6/p115/cmd/check.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/cmd/iterdir.py` & `python_115-0.0.8.7.6/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/cmd/qrcode.py` & `python_115-0.0.8.7.6/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/component/__init__.py` & `python_115-0.0.8.7.6/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/component/cipher.py` & `python_115-0.0.8.7.6/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/component/client.py` & `python_115-0.0.8.7.6/p115/component/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1718,61 +1718,61 @@
             payload = {"file_id": payload}
         request_kwargs.pop("parse", None)
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     @overload
     def fs_files(
         self, 
-        payload: dict, 
+        payload: int | dict, 
         /,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def fs_files(
         self, 
-        payload: dict, 
+        payload: int | dict, 
         /,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def fs_files(
         self, 
-        payload: dict = {}, 
+        payload: int | dict = 0, 
         /,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """获取文件夹的中的文件列表和基本信息
         GET https://webapi.115.com/files
         payload:
             - cid: int | str = 0 # 文件夹 id
             - limit: int = 32    # 一页大小，意思就是 page_size
             - offset: int = 0    # 索引偏移，索引从 0 开始计算
-            - asc: 0 | 1 = 1     # 是否升序排列
-            - o: str = "file_name"
-                # 用某字段排序：
-                # - 文件名："file_name"
-                # - 文件大小："file_size"
-                # - 文件种类："file_type"
-                # - 修改时间："user_utime"
-                # - 创建时间："user_ptime"
-                # - 上次打开时间："user_otime"
 
             - aid: int | str = 1
+            - asc: 0 | 1 = <default> # 是否升序排列
             - code: int | str = <default>
             - count_folders: 0 | 1 = 1
             - custom_order: int | str = <default>
             - fc_mix: 0 | 1 = <default> # 是否文件夹置顶，0 为置顶
             - format: str = "json"
             - is_q: 0 | 1 = <default>
             - is_share: 0 | 1 = <default>
             - natsort: 0 | 1 = <default>
+            - o: str = <default>
+                # 用某字段排序：
+                # - 文件名："file_name"
+                # - 文件大小："file_size"
+                # - 文件种类："file_type"
+                # - 修改时间："user_utime"
+                # - 创建时间："user_ptime"
+                # - 上次打开时间："user_otime"
             - record_open_time: 0 | 1 = 1
             - scid: int | str = <default>
             - show_dir: 0 | 1 = 1
             - snap: 0 | 1 = <default>
             - source: str = <default>
             - star: 0 | 1 = <default> # 是否星标文件
             - suffix: str = <default> # 后缀名
@@ -1784,71 +1784,159 @@
                 # - 音频: 3
                 # - 视频: 4
                 # - 压缩包: 5
                 # - 应用: 6
                 # - 书籍: 7
         """
         api = "https://webapi.115.com/files"
-        payload = {
-            "aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", 
-            "offset": 0, "record_open_time": 1, "show_dir": 1, **payload, 
-        }
+        if isinstance(payload, int):
+            payload = {
+                "aid": 1, "count_folders": 1, "limit": 32, "offset": 0, 
+                "record_open_time": 1, "show_dir": 1, "cid": payload, 
+            }
+        else:
+            payload = {
+                "aid": 1, "cid": 0, "count_folders": 1, "limit": 32, "offset": 0, 
+                "record_open_time": 1, "show_dir": 1, **payload, 
+            }
         request_kwargs.pop("parse", None)
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     @overload
     def fs_files2(
         self, 
-        payload: dict, 
+        payload: int | dict, 
         /,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def fs_files2(
         self, 
-        payload: dict, 
+        payload: int | dict, 
         /,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def fs_files2(
         self, 
-        payload: dict = {}, 
+        payload: int | dict = 0, 
         /,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """获取文件夹的中的文件列表和基本信息
         GET https://aps.115.com/natsort/files.php
         payload:
             - cid: int | str = 0 # 文件夹 id
             - limit: int = 32    # 一页大小，意思就是 page_size
             - offset: int = 0    # 索引偏移，索引从 0 开始计算
-            - asc: 0 | 1 = 1     # 是否升序排列
-            - o: str = "file_name"
+
+            - aid: int | str = 1
+            - asc: 0 | 1 = <default> # 是否升序排列
+            - code: int | str = <default>
+            - count_folders: 0 | 1 = 1
+            - custom_order: int | str = <default>
+            - fc_mix: 0 | 1 = <default> # 是否文件夹置顶，0 为置顶
+            - format: str = "json"
+            - is_q: 0 | 1 = <default>
+            - is_share: 0 | 1 = <default>
+            - natsort: 0 | 1 = <default>
+            - o: str = <default>
                 # 用某字段排序：
                 # - 文件名："file_name"
                 # - 文件大小："file_size"
                 # - 文件种类："file_type"
                 # - 修改时间："user_utime"
                 # - 创建时间："user_ptime"
                 # - 上次打开时间："user_otime"
+            - record_open_time: 0 | 1 = 1
+            - scid: int | str = <default>
+            - show_dir: 0 | 1 = 1
+            - snap: 0 | 1 = <default>
+            - source: str = <default>
+            - star: 0 | 1 = <default> # 是否星标文件
+            - suffix: str = <default> # 后缀名
+            - type: int | str = <default>
+                # 文件类型：
+                # - 所有: 0
+                # - 文档: 1
+                # - 图片: 2
+                # - 音频: 3
+                # - 视频: 4
+                # - 压缩包: 5
+                # - 应用: 6
+                # - 书籍: 7
+        """
+        api = "https://aps.115.com/natsort/files.php"
+        if isinstance(payload, int):
+            payload = {
+                "aid": 1, "count_folders": 1, "limit": 32, "offset": 0, 
+                "record_open_time": 1, "show_dir": 1, "cid": payload, 
+            }
+        else:
+            payload = {
+                "aid": 1, "cid": 0, "count_folders": 1, "limit": 32, "offset": 0, 
+                "record_open_time": 1, "show_dir": 1, **payload, 
+            }
+        request_kwargs.pop("parse", None)
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def fs_files3(
+        self, 
+        payload: int | dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def fs_files3(
+        self, 
+        payload: int | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def fs_files3(
+        self, 
+        payload: int | dict = 0, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """获取文件夹的中的文件列表和基本信息
+        GET https://proapi.115.com/android/2.0/ufile/files
+        payload:
+            - cid: int | str = 0 # 文件夹 id
+            - limit: int = 32    # 一页大小，意思就是 page_size
+            - offset: int = 0    # 索引偏移，索引从 0 开始计算
 
             - aid: int | str = 1
+            - asc: 0 | 1 = <default> # 是否升序排列
             - code: int | str = <default>
             - count_folders: 0 | 1 = 1
             - custom_order: int | str = <default>
             - fc_mix: 0 | 1 = <default> # 是否文件夹置顶，0 为置顶
             - format: str = "json"
             - is_q: 0 | 1 = <default>
             - is_share: 0 | 1 = <default>
             - natsort: 0 | 1 = <default>
+            - o: str = <default>
+                # 用某字段排序：
+                # - 文件名："file_name"
+                # - 文件大小："file_size"
+                # - 文件种类："file_type"
+                # - 修改时间："user_utime"
+                # - 创建时间："user_ptime"
+                # - 上次打开时间："user_otime"
             - record_open_time: 0 | 1 = 1
             - scid: int | str = <default>
             - show_dir: 0 | 1 = 1
             - snap: 0 | 1 = <default>
             - source: str = <default>
             - star: 0 | 1 = <default> # 是否星标文件
             - suffix: str = <default> # 后缀名
@@ -1859,23 +1947,77 @@
                 # - 图片: 2
                 # - 音频: 3
                 # - 视频: 4
                 # - 压缩包: 5
                 # - 应用: 6
                 # - 书籍: 7
         """
-        api = "https://aps.115.com/natsort/files.php"
-        payload = {
-            "aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", 
-            "offset": 0, "record_open_time": 1, "show_dir": 1, **payload, 
-        }
+        api = "https://proapi.115.com/android/2.0/ufile/files"
+        if isinstance(payload, int):
+            payload = {
+                "aid": 1, "count_folders": 1, "limit": 32, "offset": 0, 
+                "record_open_time": 1, "show_dir": 1, "cid": payload, 
+            }
+        else:
+            payload = {
+                "aid": 1, "cid": 0, "count_folders": 1, "limit": 32, "offset": 0, 
+                "record_open_time": 1, "show_dir": 1, **payload, 
+            }
         request_kwargs.pop("parse", None)
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     @overload
+    def fs_files_order(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def fs_files_order(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def fs_files_order(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """获取文件夹的中的文件列表和基本信息
+        POST https://webapi.115.com/files/order
+        payload:
+            - user_order: str
+                # 用某字段排序：
+                # - 文件名："file_name"
+                # - 文件大小："file_size"
+                # - 文件种类："file_type"
+                # - 修改时间："user_utime"
+                # - 创建时间："user_ptime"
+                # - 上次打开时间："user_otime"
+            - file_id: int | str = 0 # 目录 id
+            - user_asc: 0 | 1 = <default> # 是否升序排列
+            - fc_mix: 0 | 1 = <default>   # 是否文件夹置顶，0 为置顶
+        """
+        api = "https://webapi.115.com/files/order"
+        if isinstance(payload, str):
+            payload = {"file_id": 0, "user_order": payload}
+        else:
+            payload = {"file_id": 0, **payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+
+    @overload
     def fs_files_type(
         self, 
         payload: Literal[1,2,3,4,5,6,7] | dict, 
         /,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
@@ -4634,14 +4776,15 @@
     def user_id(self, /) -> int:
         return self.upload_info["user_id"]
 
     @property
     def user_key(self, /) -> str:
         return self.upload_info["userkey"]
 
+    # TODO: 返回一个 DictAttr，这个类型会在一个公共模块中实现
     @cached_property
     def upload_url(self, /) -> dict:
         """获取用于上传的一些 http 接口，此接口具有一定幂等性，请求一次，然后把响应记下来即可
         GET https://uplb.115.com/3.0/getuploadinfo.php
         response:
             - endpoint: 此接口用于上传文件到阿里云 OSS 
             - gettokenurl: 上传前需要用此接口获取 token
```

### Comparing `python_115-0.0.8.7.5/p115/component/fs.py` & `python_115-0.0.8.7.6/p115/component/fs.py`

 * *Files 3% similar despite different names*

```diff
@@ -375,23 +375,34 @@
                 raise FileNotFoundError(result)
             # {'state': False, 'code': 990002, 'message': '参数错误。'}
             case 990002:
                 raise OSError(errno.EINVAL, result)
             case _:
                 raise OSError(errno.EIO, result)
 
-    def fs_files(self, /, payload: dict) -> AttrDict:
-        id = int(payload["cid"])
+    def fs_files(
+        self, 
+        /, 
+        payload: None | int | dict = None, 
+    ) -> AttrDict:
+        if payload is None:
+            payload = self.id
+        if isinstance(payload, int):
+            id = payload
+        else:
+            id = int(payload["cid"])
         resp = check_response(self.client.fs_files(payload))
         if int(resp["path"][-1]["cid"]) != id:
             raise NotADirectoryError(errno.ENOTDIR, f"{id!r} is not a directory")
         return resp
 
     @check_response
     def fs_search(self, payload: str | dict, /) -> AttrDict:
+        if isinstance(payload, str):
+            payload = {"cid": self.id, "search_value": payload}
         return self.client.fs_search(payload)
 
     @check_response
     def space_summury(self, /) -> AttrDict:
         return self.client.fs_space_summury()
 
     def _upload(
@@ -666,38 +677,39 @@
             return self._attr_path(id_or_path, pid)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
-        refresh: bool = False, 
+        start: int = 0, 
+        stop: None | int = None, 
         page_size: int = 1_000, 
+        refresh: bool = False, 
         **payload, 
     ) -> Iterator[AttrDict]:
         """迭代获取目录内直属的文件或目录的信息
         payload:
-            - asc: 0 | 1 = 1     # 是否升序排列
+            - asc: 0 | 1 = <default> # 是否升序排列
             - code: int | str = <default>
             - count_folders: 0 | 1 = 1
             - custom_order: int | str = <default>
             - fc_mix: 0 | 1 = <default> # 是否文件夹置顶，0 为置顶
             - format: str = "json"
             - is_q: 0 | 1 = <default>
             - is_share: 0 | 1 = <default>
             - natsort: 0 | 1 = <default>
-            - o: str = "file_name"
+            - o: str = <default>
                 # 用某字段排序：
                 # - 文件名："file_name"
                 # - 文件大小："file_size"
                 # - 文件种类："file_type"
                 # - 修改时间："user_utime"
                 # - 创建时间："user_ptime"
                 # - 上次打开时间："user_otime"
-            - offset: int = 0    # 索引偏移，索引从 0 开始计算
             - record_open_time: 0 | 1 = 1
             - scid: int | str = <default>
             - show_dir: 0 | 1 = 1
             - snap: 0 | 1 = <default>
             - source: str = <default>
             - star: 0 | 1 = <default> # 是否星标文件
             - suffix: str = <default> # 后缀名
@@ -772,39 +784,108 @@
                             if path != old_attr["path"] and path_to_id is not None:
                                 try:
                                     del path_to_id[old_attr["path"]]
                                 except LookupError:
                                     pass
                             old_attr.update(attr)
                 return attr
-            def iterdir():
+            def iterdir(fetch_all: bool = True) -> Iterator[dict]:
+                nonlocal start, stop
                 get_files = self.fs_files
+                count = -1
+                total = -1
+                if fetch_all:
+                    payload["offset"] = 0
+                else:
+                    if start is None:
+                        start = 0
+                    elif start < 0:
+                        count = self.dirlen(id)
+                        start += count
+                        if start < 0:
+                            start = 0
+                    if stop is None or stop < 0:
+                        if count < 0:
+                            count = self.dirlen(id)
+                        if stop is None:
+                            stop = count
+                        else:
+                            stop += count
+                    if start >= stop or stop <= 0 or count >= 0 and start >= count:
+                        return
+                    payload["offset"] = start
+                    total = stop - start
+                    if total < page_size:
+                        payload["limit"] = total
+                    set_order_payload = {}
+                    if "o" in payload:
+                        set_order_payload["user_order"] = payload["o"]
+                    if "asc" in payload:
+                        set_order_payload["user_asc"] = payload["asc"]
+                    if set_order_payload:
+                        set_order_payload["file_id"] = id
+                        if "fc_mix" in payload:
+                            set_order_payload["fc_mix"] = payload["fc_mix"]
+                        self.client.fs_files_order(set_order_payload)
                 resp = get_files(payload)
                 dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
                 if path_to_id is not None:
                     path_to_id[dirname] = id
                 count = resp["count"]
                 for attr in resp["data"]:
                     yield normalize_attr(attr, dirname, fs=self)
-                for offset in range(page_size, count, page_size):
-                    payload["offset"] = offset
+                if total < 0:
+                    total = count
+                if total <= page_size:
+                    return
+                for _ in range((total - 1) // page_size + 1):
+                    payload["offset"] += page_size
                     resp = get_files(payload)
                     if resp["count"] != count:
                         raise RuntimeError(f"{id} detected count changes during iteration")
                     for attr in resp["data"]:
                         yield normalize_attr(attr, dirname, fs=self)
             if attr_cache is None:
-                return iterdir()
+                return iterdir(False)
             else:
-                payload["offset"] = 0
                 children = {a["id"]: a for a in iterdir()}
                 attrs = attr_cache[id] = {"version": version, "attr": attr, "children": children}
         else:
             children = pid_attrs["children"]
-        return islice(children.values(), offset, None)
+        count = len(children)
+        if start is None:
+            start = 0
+        elif start < 0:
+            start += count
+            if start < 0:
+                start = 0
+        if stop is None:
+            stop = count
+        elif stop < 0:
+            stop += count
+        if start >= stop or stop <= 0 or start >= count:
+            return iter(())
+        match payload.get("o"):
+            case "file_name":
+                key = lambda attr: attr["name"]
+            case "file_size":
+                key = lambda attr: attr.get("size") or 0
+            case "file_type":
+                key = lambda attr: attr.get("ico", "")
+            case "user_utime":
+                key = lambda attr: attr["utime"]
+            case "user_ptime":
+                key = lambda attr: attr["ptime"]
+            case "user_otime":
+                key = lambda attr: attr["open_time"]
+            case _:
+                return islice(children.values(), start, stop)
+        return iter(sorted(
+            children.values(), key=key, reverse=payload.get("asc", True), 
+        )[start:stop])
 
     def copy(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
@@ -1028,15 +1109,15 @@
         attr = self.attr(id_or_path, pid)
         ls = self._dir_get_ancestors(attr["parent_id"])
         ls.append({"name": attr["name"], "id": attr["id"], "parent_id": attr["parent_id"], "is_directory": attr["is_directory"]})
         return ls
 
     def dirlen(
         self, 
-        id_or_path: IDOrPathType, 
+        id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> int:
         "文件夹中的项目数（直属的文件和目录计数）"
         return self.fs_files({"cid": self.get_id(id_or_path, pid), "limit": 1})["count"]
 
     def get_id_from_pickcode(self, /, pickcode: str = "") -> int:
@@ -1047,15 +1128,15 @@
 
     def get_info_from_pickcode(self, /, pickcode: str) -> AttrDict:
         "由 pickcode 获取一些目录信息"
         return self.client.download_url(pickcode, strict=False, detail=True).__dict__
 
     def get_pickcode(
         self, 
-        id_or_path: IDOrPathType, 
+        id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> str:
         "获取 pickcode"
         return self.attr(id_or_path, pid).get("pickcode", "")
 
     def get_url(
```

### Comparing `python_115-0.0.8.7.5/p115/component/fs_base.py` & `python_115-0.0.8.7.6/p115/component/fs_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from os import fsdecode, fspath, lstat, makedirs, scandir, stat, stat_result, PathLike
 from os import path as ospath
 from posixpath import join as joinpath, splitext
 from re import compile as re_compile, escape as re_escape
 from stat import S_IFDIR, S_IFREG # TODO: common stat method
 from time import time
 from typing import (
-    cast, Any, Generic, IO, Literal, Never, Optional, Self, TypeAlias, TypeVar, 
+    cast, Any, Generic, IO, Literal, Never, Self, TypeAlias, TypeVar, 
 )
 from types import MappingProxyType
 from urllib.parse import parse_qsl, urlparse
 
 from download import DownloadTask
 from filewrap import SupportsWrite
 from httpfile import HTTPFileReader
@@ -158,46 +158,49 @@
     def download(
         self, 
         /, 
         local_dir: bytes | str | PathLike = "", 
         write_mode: Literal["a", "w", "x", "i"] = "a", 
         submit: None | bool | Callable[[Callable], Any] = None, 
         no_root: bool = False, 
-        predicate: Optional[Callable[[P115PathType], bool]] = None, 
+        predicate: None | Callable[[P115PathType], bool] = None, 
         onerror: None | bool | Callable[[BaseException], Any] = None, 
     ) -> Iterator[tuple[P115PathType, str, DownloadTask]]:
         return self.fs.download_tree(
             self, 
             local_dir, 
             write_mode=write_mode, 
             submit=submit, 
             no_root=no_root, 
             predicate=predicate, 
             onerror=onerror, 
         )
 
+    def enumdir(self, /, **kwargs) -> Iterator[str]:
+        return self.fs.enumdir(self if self.is_dir() else self["parent_id"], **kwargs)
+
     def exists(self, /) -> bool:
         return self.fs.exists(self)
 
     @property
-    def file_extension(self, /) -> Optional[str]:
+    def file_extension(self, /) -> None | str:
         if not self.is_file():
             return None
         return splitext(basename(self.path))[1]
 
     def glob(
         self, 
         /, 
         pattern: str = "*", 
         ignore_case: bool = False, 
         allow_escaped_slash: bool = True, 
     ) -> Iterator[Self]:
         return self.fs.glob(
             pattern, 
-            self if self.is_dir() else self.parent, 
+            self if self.is_dir() else self["parent_id"], 
             ignore_case=ignore_case, 
             allow_escaped_slash=allow_escaped_slash, 
         )
 
     def is_absolute(self, /) -> bool:
         return True
 
@@ -228,31 +231,34 @@
 
     def inode(self, /) -> int:
         return self.id
 
     def iter(
         self, 
         /, 
-        topdown: Optional[bool] = True, 
+        topdown: None | bool = True, 
         min_depth: int = 1, 
         max_depth: int = 1, 
-        predicate: Optional[Callable[[Self], Optional[bool]]] = None, 
+        predicate: None | Callable[[Self], None | bool] = None, 
         onerror: bool | Callable[[OSError], bool] = False, 
         **kwargs, 
     ) -> Iterator[Self]:
         return self.fs.iter(
-            self, 
+            self if self.is_dir() else self["parent_id"], 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             predicate=predicate, 
             onerror=onerror, 
             **kwargs, 
         )
 
+    def iterdir(self, /, **kwargs) -> Iterator[AttrDict]:
+        return self.fs.iterdir(self if self.is_dir() else self["parent_id"], **kwargs)
+
     def join(self, *names: str) -> Self:
         if not names:
             return self
         attr = self.fs.attr(names, self.id)
         return type(self)(attr)
 
     def joinpath(self, *paths: str | PathLike[str]) -> Self:
@@ -271,21 +277,21 @@
     @property
     def length(self, /) -> int:
         if self.is_dir():
             return len(tuple(self.fs.iterdir()))
         return self["size"]
 
     def listdir(self, /, **kwargs) -> list[str]:
-        return self.fs.listdir(self, **kwargs)
+        return self.fs.listdir(self if self.is_dir() else self["parent_id"], **kwargs)
 
     def listdir_attr(self, /, **kwargs) -> list[AttrDict]:
-        return self.fs.listdir_attr(self, **kwargs)
+        return self.fs.listdir_attr(self if self.is_dir() else self["parent_id"], **kwargs)
 
     def listdir_path(self, /, **kwargs) -> list[Self]:
-        return self.fs.listdir_path(self, **kwargs)
+        return self.fs.listdir_path(self if self.is_dir() else self["parent_id"], **kwargs)
 
     def match(
         self, 
         /, 
         path_pattern: str, 
         ignore_case: bool = False, 
         allow_escaped_slash: bool = True, 
@@ -294,32 +300,32 @@
             t[0] for t in translate_iter(
                 path_pattern, allow_escaped_slash=allow_escaped_slash))
         if ignore_case:
             pattern = "(?i:%s)" % pattern
         return re_compile(pattern).fullmatch(self.path) is not None
 
     @property
-    def media_type(self, /) -> Optional[str]:
+    def media_type(self, /) -> None | str:
         if not self.is_file():
             return None
         return guess_type(self.path)[0] or "application/octet-stream"
 
     @property
     def name(self, /) -> str:
         return basename(self.path)
 
     def open(
         self, 
         /, 
         mode: str = "r", 
-        buffering: Optional[int] = None, 
-        encoding: Optional[str] = None, 
-        errors: Optional[str] = None, 
-        newline: Optional[str] = None, 
-        headers: Optional[Mapping] = None, 
+        buffering: None | int = None, 
+        encoding: None | str = None, 
+        errors: None | str = None, 
+        newline: None | str = None, 
+        headers: None | Mapping = None, 
         start: int = 0, 
         seek_threshold: int = 1 << 20, 
     ) -> HTTPFileReader | IO:
         return self.fs.open(
             self, 
             mode=mode, 
             buffering=buffering, 
@@ -355,15 +361,15 @@
     def patht(self, /) -> tuple[str, ...]:
         return tuple(splits(self.path)[0])
 
     def read_bytes(
         self, 
         /, 
         start: int = 0, 
-        stop: Optional[int] = None, 
+        stop: None | int = None, 
     ) -> bytes:
         return self.fs.read_bytes(self, start, stop)
 
     def read_bytes_range(self, /, bytes_range: str = "0-") -> bytes:
         return self.fs.read_bytes_range(self, bytes_range)
 
     def read_block(
@@ -375,17 +381,17 @@
         if size <= 0:
             return b""
         return self.fs.read_block(self, size, offset)
 
     def read_text(
         self, 
         /, 
-        encoding: Optional[str] = None, 
-        errors: Optional[str] = None, 
-        newline: Optional[str] = None, 
+        encoding: None | str = None, 
+        errors: None | str = None, 
+        newline: None | str = None, 
     ) -> str:
         return self.fs.read_text(self, encoding=encoding, errors=errors, newline=newline)
 
     def relative_to(self, other: str | Self, /) -> str:
         if type(self) is type(other):
             other = cast(Self, other)
             other = other.path
@@ -416,28 +422,31 @@
         /, 
         pattern: str = "", 
         ignore_case: bool = False, 
         allow_escaped_slash: bool = True, 
     ) -> Iterator[Self]:
         return self.fs.rglob(
             pattern, 
-            self if self.is_dir() else self.parent, 
+            self if self.is_dir() else self["parent_id"], 
             ignore_case=ignore_case, 
             allow_escaped_slash=allow_escaped_slash, 
         )
 
     @cached_property
     def root(self, /) -> Self:
         return type(self)(self.fs.attr(0))
 
     def samefile(self, path: str | PathLike[str], /) -> bool:
         if type(self) is type(path):
             return self == path
         return path in ("", ".") or self.path == self.fs.abspath(path)
 
+    def scandir(self, /, **kwargs) -> Iterator[Self]:
+        return self.fs.scandir(self if self.is_dir() else self["parent_id"], **kwargs)
+
     def stat(self, /) -> stat_result:
         return self.fs.stat(self)
 
     @property
     def stem(self, /) -> str:
         return splitext(basename(self.path))[0]
 
@@ -461,58 +470,58 @@
         url = ns["url"] = self.fs.get_url(self)
         ns["url_expire_time"] = int(parse_qsl(urlparse(url).query)[0][1])
         return url
 
     def walk(
         self, 
         /, 
-        topdown: Optional[bool] = True, 
+        topdown: None | bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[str], list[str]]]:
         return self.fs.walk(
-            self, 
+            self if self.is_dir() else self["parent_id"], 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             onerror=onerror, 
             **kwargs, 
         )
 
     def walk_attr(
         self, 
         /, 
-        topdown: Optional[bool] = True, 
+        topdown: None | bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         return self.fs.walk_attr(
-            self, 
+            self if self.is_dir() else self["parent_id"], 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             onerror=onerror, 
             **kwargs, 
         )
 
     def walk_path(
         self, 
         /, 
-        topdown: Optional[bool] = True, 
+        topdown: None | bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[Self], list[Self]]]:
         return self.fs.walk_path(
-            self, 
+            self if self.is_dir() else self["parent_id"], 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             onerror=onerror, 
             **kwargs, 
         )
 
@@ -560,46 +569,46 @@
         return f"<{name}(client={self.client!r}, id={self.id!r}, path={self.path!r}) at {hex(id(self))}>"
 
     @abstractmethod
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> AttrDict:
         ...
 
     @abstractmethod
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
-        headers: Optional[Mapping] = None, 
+        pid: None | int = None, 
+        headers: None | Mapping = None, 
     ) -> str:
         ...
 
     @abstractmethod
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         **kwargs, 
     ) -> Iterator[AttrDict]:
         ...
 
     def abspath(self, path: str | PathLike[str] = "", /) -> str:
         return self.get_path(path, self.id)
 
     def as_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> P115PathType:
         path_class = type(self).path_class
         attr: AttrDict
         if isinstance(id_or_path, path_class):
             return id_or_path
         elif isinstance(id_or_path, dict):
             attr = cast(AttrDict, id_or_path)
@@ -610,15 +619,15 @@
         attr["fs"] = self
         return path_class(attr)
 
     def chdir(
         self, 
         id_or_path: IDOrPathType = 0, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> int:
         path_class = type(self).path_class
         if isinstance(id_or_path, path_class):
             id = id_or_path.id
             self.__dict__.update(
                 id = id, 
                 path = id_or_path["path"], 
@@ -644,51 +653,51 @@
             raise NotADirectoryError(
                 errno.ENOTDIR, f"{id_or_path!r} (in {pid!r}) is not a directory")
 
     def dictdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         full_path: bool = False, 
         **kwargs, 
     ) -> dict[int, str]:
         if full_path:
             return {attr["id"]: attr["path"] for attr in self.iterdir(id_or_path, pid, **kwargs)}
         else:
             return {attr["id"]: attr["name"] for attr in self.iterdir(id_or_path, pid, **kwargs)}
 
     def dictdir_attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         **kwargs, 
     ) -> dict[int, AttrDict]:
         return {attr["id"]: attr for attr in self.iterdir(id_or_path, pid, **kwargs)}
 
     def dictdir_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         **kwargs, 
     ) -> dict[int, P115PathType]:
         path_class = type(self).path_class
         return {attr["id"]: path_class(attr) for attr in self.iterdir(id_or_path, pid, **kwargs)}
 
     def download(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         local_path_or_file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         write_mode: Literal["a", "w", "x", "i"] = "a", 
         submit: bool | Callable[[Callable], Any] = True, 
-    ) -> Optional[DownloadTask]:
+    ) -> None | DownloadTask:
         if not isinstance(local_path_or_file, SupportsWrite):
             path = cast(bytes | str | PathLike, local_path_or_file)
             if not path:
                 path = self.attr(id_or_path, pid)["name"]
             if ospath.lexists(path):
                 if write_mode == "x":
                     raise FileExistsError(
@@ -716,19 +725,19 @@
         return task
 
     def download_tree(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         local_dir: bytes | str | PathLike = "", 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         write_mode: Literal["i", "x", "w", "a"] = "a", 
         submit: None | bool | Callable[[Callable], Any] = None, 
         no_root: bool = False, 
-        predicate: Optional[Callable[[P115PathType], bool]] = None, 
+        predicate: None | Callable[[P115PathType], bool] = None, 
         onerror: None | bool | Callable[[BaseException], Any] = None, 
     ) -> Iterator[tuple[P115PathType, str, DownloadTask]]:
         local_dir = fsdecode(local_dir)
         if local_dir:
             makedirs(local_dir, exist_ok=True)
         attr = self.attr(id_or_path, pid)
         pathes: Iterable[P115PathType]
@@ -782,19 +791,32 @@
                         onerror(exc)
                 else:
                     if task is not None:
                         yield subpath, download_path, task
                         if submit is None:
                             task.run_wait()
 
+    def enumdir(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: None | int = None, 
+        full_path: bool = False, 
+        **kwargs, 
+    ) -> Iterator[str]:
+        if full_path:
+            return (attr["path"] for attr in self.iterdir(id_or_path, pid, **kwargs))
+        else:
+            return (attr["name"] for attr in self.iterdir(id_or_path, pid, **kwargs))
+
     def exists(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> bool:
         path_class = type(self).path_class
         try:
             if isinstance(id_or_path, path_class):
                 id_or_path()
             else:
                 self.attr(id_or_path, pid)
@@ -810,15 +832,15 @@
             return self.attr(self.id)["path"]
         return self.path
 
     def get_id(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> int:
         path_class = type(self).path_class
         if pid is None and (not id_or_path or id_or_path == "."):
             return self.id
         elif isinstance(id_or_path, path_class):
             return id_or_path.id
         elif isinstance(id_or_path, int):
@@ -834,15 +856,15 @@
             pass
         return self.attr(id_or_path, pid)["id"]
 
     def get_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> str:
         path_class = type(self).path_class
         if pid is None and (not id_or_path or id_or_path == "."):
             return self.path
         elif isinstance(id_or_path, path_class):
             return id_or_path.path
         elif isinstance(id_or_path, dict):
@@ -869,15 +891,15 @@
                 path = joinpath(ppath, path)
         return path
 
     def get_patht(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> list[str]:
         path_class = type(self).path_class
         if pid is None and (not id_or_path or id_or_path == "."):
             return splits(self.path)[0]
         elif isinstance(id_or_path, path_class):
             return splits(id_or_path.path)[0]
         elif isinstance(id_or_path, dict):
@@ -1038,46 +1060,46 @@
         path = path_class(attr)
         return glob_step_match(path, i)
 
     def isdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> bool:
         path_class = type(self).path_class
         if isinstance(id_or_path, path_class):
             return id_or_path["is_directory"]
         try:
             return self.attr(id_or_path, pid)["is_directory"]
         except FileNotFoundError:
             return False
 
     def isfile(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> bool:
         path_class = type(self).path_class
         if isinstance(id_or_path, path_class):
             return not id_or_path["is_directory"]
         try:
             return not self.attr(id_or_path, pid)["is_directory"]
         except FileNotFoundError:
             return False
 
     def _iter_bfs(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         min_depth: int = 1, 
         max_depth: int = 1, 
-        predicate: Optional[Callable[[P115PathType], Optional[bool]]] = None, 
+        predicate: None | Callable[[P115PathType], None | bool] = None, 
         onerror: bool | Callable[[OSError], bool] = False, 
         **kwargs, 
     ) -> Iterator[P115PathType]:
         dq: deque[tuple[int, P115PathType]] = deque()
         push, pop = dq.append, dq.popleft
         path_class = type(self).path_class
         path = self.as_path(top, pid)
@@ -1110,19 +1132,19 @@
                 elif onerror:
                     raise
 
     def _iter_dfs(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         topdown: bool = True, 
         min_depth: int = 1, 
         max_depth: int = 1, 
-        predicate: Optional[Callable[[P115PathType], Optional[bool]]] = None, 
+        predicate: None | Callable[[P115PathType], None | bool] = None, 
         onerror: bool | Callable[[OSError], bool] = False, 
         **kwargs, 
     ) -> Iterator[P115PathType]:
         if not max_depth:
             return
         global_yield_me = True
         if min_depth > 1:
@@ -1170,19 +1192,19 @@
             elif onerror:
                 raise
 
     def iter(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
-        topdown: Optional[bool] = True, 
+        pid: None | int = None, 
+        topdown: None | bool = True, 
         min_depth: int = 1, 
         max_depth: int = 1, 
-        predicate: Optional[Callable[[P115PathType], Optional[bool]]] = None, 
+        predicate: None | Callable[[P115PathType], None | bool] = None, 
         onerror: bool | Callable[[OSError], bool] = False, 
         **kwargs, 
     ) -> Iterator[P115PathType]:
         if topdown is None:
             return self._iter_bfs(
                 top, 
                 pid, 
@@ -1204,55 +1226,55 @@
                 **kwargs, 
             )
 
     def listdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         full_path: bool = False, 
         **kwargs, 
     ) -> list[str]:
         if full_path:
             return [attr["path"] for attr in self.iterdir(id_or_path, pid, **kwargs)]
         else:
             return [attr["name"] for attr in self.iterdir(id_or_path, pid, **kwargs)]
 
     def listdir_attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         **kwargs, 
     ) -> list[AttrDict]:
         return list(self.iterdir(id_or_path, pid, **kwargs))
 
     def listdir_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         **kwargs, 
     ) -> list[P115PathType]:
         path_class = type(self).path_class
         return [path_class(attr) for attr in self.iterdir(id_or_path, pid, **kwargs)]
 
     def open(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         mode: str = "r", 
-        buffering: Optional[int] = None, 
-        encoding: Optional[str] = None, 
-        errors: Optional[str] = None, 
-        newline: Optional[str] = None, 
-        headers: Optional[Mapping] = None, 
+        buffering: None | int = None, 
+        encoding: None | str = None, 
+        errors: None | str = None, 
+        newline: None | str = None, 
+        headers: None | Mapping = None, 
         start: int = 0, 
         seek_threshold: int = 1 << 20, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> HTTPFileReader | IO:
         if mode not in ("r", "rt", "tr", "rb", "br"):
             raise OSError(errno.EINVAL, f"invalid (or unsupported) mode: {mode!r}")
         url = self.get_url(id_or_path, pid)
         return self.client.open(
             url, 
             headers=headers, 
@@ -1267,51 +1289,51 @@
         )
 
     def read_bytes(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         start: int = 0, 
-        stop: Optional[int] = None, 
-        pid: Optional[int] = None, 
+        stop: None | int = None, 
+        pid: None | int = None, 
     ) -> bytes:
         url = self.get_url(id_or_path, pid)
         return self.client.read_bytes(url, start, stop)
 
     def read_bytes_range(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         bytes_range: str = "0-", 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> bytes:
         url = self.get_url(id_or_path, pid)
         return self.client.read_bytes_range(url, bytes_range)
 
     def read_block(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         size: int = 0, 
         offset: int = 0, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> bytes:
         if size <= 0:
             return b""
         url = self.get_url(id_or_path, pid)
         return self.client.read_block(url, size, offset)
 
     def read_text(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        encoding: Optional[str] = None, 
-        errors: Optional[str] = None, 
-        newline: Optional[str] = None, 
-        pid: Optional[int] = None, 
+        encoding: None | str = None, 
+        errors: None | str = None, 
+        newline: None | str = None, 
+        pid: None | int = None, 
     ):
         return self.open(
             id_or_path, 
             encoding=encoding, 
             errors=errors, 
             newline=newline, 
             pid=pid, 
@@ -1333,34 +1355,34 @@
             pattern = joinpath("**", pattern)
         return self.glob(pattern, dirname, ignore_case=ignore_case, allow_escaped_slash=allow_escaped_slash)
 
     def scandir(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         **kwargs, 
     ) -> Iterator[P115PathType]:
         return map(type(self).path_class, self.iterdir(id_or_path, pid, **kwargs))
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> stat_result:
         raise UnsupportedOperation(errno.ENOSYS, 
             "`stat()` is currently not supported, use `attr()` instead."
         )
 
     def _walk_bfs(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         dq: deque[tuple[int, AttrDict]] = deque()
         push, pop = dq.append, dq.popleft
@@ -1391,15 +1413,15 @@
                 elif onerror:
                     raise
 
     def _walk_dfs(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         topdown: bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         if not max_depth:
@@ -1435,16 +1457,16 @@
             elif onerror:
                 raise
 
     def walk(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
-        topdown: Optional[bool] = True, 
+        pid: None | int = None, 
+        topdown: None | bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[str], list[str]]]:
         for path, dirs, files in self.walk_attr(
             top, 
@@ -1457,16 +1479,16 @@
         ):
             yield path, [a["name"] for a in dirs], [a["name"] for a in files]
 
     def walk_attr(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
-        topdown: Optional[bool] = True, 
+        pid: None | int = None, 
+        topdown: None | bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[AttrDict], list[AttrDict]]]:
         if topdown is None:
             return self._walk_bfs(
@@ -1488,16 +1510,16 @@
                 **kwargs, 
             )
 
     def walk_path(
         self, 
         top: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
-        topdown: Optional[bool] = True, 
+        pid: None | int = None, 
+        topdown: None | bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable[[OSError], bool] = None, 
         **kwargs, 
     ) -> Iterator[tuple[str, list[P115PathType], list[P115PathType]]]:
         path_class = type(self).path_class
         for path, dirs, files in self.walk_attr(
```

### Comparing `python_115-0.0.8.7.5/p115/component/fs_share.py` & `python_115-0.0.8.7.6/p115/component/fs_share.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["P115SharePath", "P115ShareFileSystem"]
 
 import errno
 
 from collections import deque
 from collections.abc import (
-    Iterable, Iterator, Mapping, MutableMapping, Sequence
+    Callable, Iterable, Iterator, Mapping, MutableMapping, Sequence
 )
 from datetime import datetime
 from functools import cached_property
-from itertools import islice
 from os import fspath, stat_result, PathLike
 from posixpath import join as joinpath
 from re import compile as re_compile
 from stat import S_IFDIR, S_IFREG
 from time import time
 from typing import cast, Never, Optional, Self
 
@@ -60,25 +59,28 @@
         info2["labels"] = info["fl"]
     if "c" in info:
         info2["violated"] = bool(info["c"])
     if "u" in info:
         info2["thumb"] = info["u"]
     if "play_long" in info:
         info2["play_long"] = info["play_long"]
+    if "ico" in info:
+        info2["ico"] = info["ico"]
     if keep_raw:
         info2["raw"] = info
     if extra_data:
         info2.update(extra_data)
     return info2
 
 
 class P115SharePath(P115PathBase):
     fs: P115ShareFileSystem
 
 
+# TODO: 默认应该是没有缓存
 class P115ShareFileSystem(P115FileSystemBase[P115SharePath]):
     share_link: str
     share_code: str
     receive_code: str
     path_to_id: MutableMapping[str, int]
     id_to_attr: MutableMapping[int, AttrDict]
     attr_cache: MutableMapping[int, tuple[AttrDict]]
@@ -298,14 +300,16 @@
         }, headers=headers)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
+        start: int = 0, 
+        stop: None | int = None, 
         page_size: int = 1_000, 
         **payload, 
     ) -> Iterator[AttrDict]:
         """迭代获取目录内直属的文件或目录的信息
         :param payload:
             - limit: int = 32
             - offset: int = 0
@@ -332,24 +336,52 @@
             attr = self.attr(id_or_path, pid)
         if not attr["is_directory"]:
             raise NotADirectoryError(
                 errno.ENOTDIR, 
                 f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
             )
         id = attr["id"]
-        payload["cid"] = id
-        payload["limit"] = page_size
-        offset = int(payload.setdefault("offset", 0))
-        if offset < 0:
-            offset = payload["offset"] = 0
-        else:
-            payload["offset"] = 0
+        children: Sequence[AttrDict]
         try:
-            return islice(self.attr_cache[id], offset, None)
+            children = self.attr_cache[id]
+            count = len(children)
+            if start is None:
+                start = 0
+            elif start < 0:
+                start += count
+                if start < 0:
+                    start = 0
+            if stop is None:
+                stop = count
+            elif stop < 0:
+                stop += count
+            if start >= stop or stop <= 0 or start >= count:
+                return iter(())
+            key: None | Callable
+            match payload.get("o"):
+                case "file_name":
+                    key = lambda attr: attr["name"]
+                case "file_size":
+                    key = lambda attr: attr.get("size") or 0
+                case "file_type":
+                    key = lambda attr: attr.get("ico", "")
+                case "user_utime" | "user_ptime" | "user_otime":
+                    key = lambda attr: attr["time"]
+                case _:
+                    key = None
+            if key:
+                children = sorted(children, key=key, reverse=payload.get("asc", True))
         except KeyError:
+            payload["cid"] = id
+            payload["limit"] = page_size
+            offset = int(payload.setdefault("offset", 0))
+            if offset < 0:
+                offset = payload["offset"] = 0
+            else:
+                payload["offset"] = 0
             dirname = attr["path"]
             def iterdir():
                 get_files = self.fs_files
                 path_to_id = self.path_to_id
                 data = get_files(payload)["data"]
                 for attr in map(normalize_info, data["list"]):
                     attr["fs"] = self
@@ -360,17 +392,17 @@
                     payload["offset"] = offset
                     data = get_files(payload)["data"]
                     for attr in map(normalize_info, data["list"]):
                         attr["fs"] = self
                         path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                         path_to_id[path] = attr["id"]
                         yield attr
-            t = self.attr_cache[id] = tuple(iterdir())
-            self.id_to_attr.update((attr["id"], attr) for attr in t)
-            return iter(t)
+            children = self.attr_cache[id] = tuple(iterdir())
+            self.id_to_attr.update((attr["id"], attr) for attr in children)
+        return iter(children[start:stop])
 
     def receive(
         self, 
         ids: int | str | Iterable[int | str], 
         /, 
         to_pid: int = 0, 
     ) -> dict:
@@ -399,19 +431,19 @@
         pid: Optional[int] = None, 
     ) -> stat_result:
         "检查路径的属性，就像 `os.stat`"
         attr = self.attr(id_or_path, pid)
         is_dir = attr["is_directory"]
         timestamp: float = attr["timestamp"]
         return stat_result((
-            (S_IFDIR if is_dir else S_IFREG) | 0o444, 
-            cast(int, attr["id"]), 
-            cast(int, attr["parent_id"]), 
-            1, 
-            self.user_id, 
-            1, 
-            cast(int, 0 if is_dir else attr["size"]), 
-            timestamp, 
-            timestamp, 
-            timestamp, 
+            (S_IFDIR if is_dir else S_IFREG) | 0o444, # mode
+            cast(int, attr["id"]), # ino
+            cast(int, attr["parent_id"]), # dev
+            1, # nlink
+            self.user_id, # uid
+            1, # gid
+            cast(int, 0 if is_dir else attr["size"]), # size
+            timestamp, # atime
+            timestamp, # mtime
+            timestamp, # ctime
         ))
```

### Comparing `python_115-0.0.8.7.5/p115/component/fs_zip.py` & `python_115-0.0.8.7.6/p115/component/fs_zip.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ) -> dict:
     timestamp = info.get("time") or 0
     return {
         "name": info["file_name"], 
         "is_directory": info["file_category"] == 0, 
         "file_category": info["file_category"], 
         "size": info["size"], 
+        "ico": info["ico"], 
         "time": datetime.fromtimestamp(timestamp), 
         "timestamp": timestamp, 
         **extra_data, 
     }
 
 
 # TODO: 兼容 pathlib.Path 和 zipfile.Path 的接口
@@ -230,14 +231,16 @@
         return self.client.extract_download_url(self.pickcode, attr["path"], headers=headers)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
+        start: int = 0, 
+        stop: None | int = None, 
         page_size: int = 999, 
         **kwargs, 
     ) -> Iterator[AttrDict]:
         """迭代获取目录内直属的文件或目录的信息
         """
         if page_size <= 0 or page_size > 999:
             page_size = 999
@@ -245,15 +248,15 @@
         if not attr["is_directory"]:
             raise NotADirectoryError(
                 errno.ENOTDIR, 
                 f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
             )
         id = attr["id"]
         try:
-            return iter(self.attr_cache[id])
+            children = self.attr_cache[id]
         except KeyError:
             nextid = self.__dict__["_nextid"]
             dirname = attr["path"]
             def iterdir():
                 get_files = self.fs_files
                 path_to_id = self.path_to_id
                 data = get_files(path=dirname, page_count=page_size)["data"]
@@ -269,34 +272,35 @@
                     for info in data["list"]:
                         attr = normalize_info(info, fs=self)
                         path = joinpath(dirname, escape(attr["name"]))
                         attr.update(id=nextid(), parent_id=id, path=path)
                         path_to_id[path] = attr["id"]
                         yield attr
                     next_marker = data["next_marker"]
-            t = self.attr_cache[id] = tuple(iterdir())
-            self.id_to_attr.update((attr["id"], attr) for attr in t)
-            return iter(t)
+            children = self.attr_cache[id] = tuple(iterdir())
+            self.id_to_attr.update((attr["id"], attr) for attr in children)
+        count = len(children)
+        return iter(children[start:stop])
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> stat_result:
         "检查路径的属性，就像 `os.stat`"
         attr = self.attr(id_or_path, pid)
         is_dir = attr["is_directory"]
         timestamp: float = attr["timestamp"]
         return stat_result((
-            (S_IFDIR if is_dir else S_IFREG) | 0o444, 
-            cast(int, attr["id"]), 
-            cast(int, attr["parent_id"]), 
-            1, 
-            self.client.user_id, 
-            1, 
-            cast(int, 0 if is_dir else attr["size"]), 
-            timestamp, 
-            timestamp, 
-            timestamp, 
+            (S_IFDIR if is_dir else S_IFREG) | 0o444, # mode
+            cast(int, attr["id"]), # ino
+            cast(int, attr["parent_id"]), # dev
+            1, # nlink
+            self.client.user_id, # uid
+            1, # gid
+            cast(int, 0 if is_dir else attr["size"]), # size
+            timestamp, # atime
+            timestamp, # mtime
+            timestamp, # ctime
         ))
```

### Comparing `python_115-0.0.8.7.5/p115/component/labellist.py` & `python_115-0.0.8.7.6/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/component/offline.py` & `python_115-0.0.8.7.6/p115/component/offline.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def __contains__(self, hash: str, /) -> bool:
         return any(item["info_hash"] == hash for item in self)
 
     def __delitem__(self, hash: str, /):
         return self.remove(hash)
 
-    def __getitem__(self, hash: str, /) -> dict:
+    def __getitem__(self, index_or_hash: str, /) -> dict:
         for item in self:
             if item["info_hash"] == hash:
                 return item
         raise LookupError(f"no such hash: {hash!r}")
 
     def __iter__(self, /) -> Iterator[dict]:
         return self.iter()
@@ -85,23 +85,39 @@
     @property
     def download_paths(self, /) -> list[P115Path]:
         "离线下载的目录列表"
         as_path = self.client.fs.as_path
         return [as_path(int(attr["file_id"])) for attr in self.download_paths_raw]
 
     @property
+    @check_response
+    def info(self, /) -> dict:
+        "获取关于离线的限制的信息"
+        return self.client.offline_info()
+
+    @property
+    def quota_info(self, /) -> dict:
+        "获取当前离线配额信息（简略）"
+        return self.client.offline_quota_info()
+
+    @property
+    def quota_package_info(self, /) -> dict:
+        "获取当前离线配额信息（详细）"
+        return self.client.offline_quota_package_info()
+
+    @property
     def sign_time(self, /) -> MappingProxyType:
         "签名和时间等信息"
         try:
             sign_time = self._sign_time
             if time() - sign_time["time"] < 30 * 60:
                 return sign_time
         except AttributeError:
             pass
-        info = check_response(self.client.offline_info())
+        info = self.info
         sign_time = self._sign_time = MappingProxyType({"sign": info["sign"], "time": info["time"]})
         return sign_time
 
     @property
     def torrent_path(self, /) -> P115Path:
         "添加 BT 种子任务的默认上传路径"
         client = self.client
```

### Comparing `python_115-0.0.8.7.5/p115/component/recyclebin.py` & `python_115-0.0.8.7.6/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/component/sharing.py` & `python_115-0.0.8.7.6/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/p115/tool/__init__.py` & `python_115-0.0.8.7.6/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/pyproject.toml` & `python_115-0.0.8.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.7.5"
+version = "0.0.8.7.6"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.7.5/readme.md` & `python_115-0.0.8.7.6/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.5/PKG-INFO` & `python_115-0.0.8.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.7.5
+Version: 0.0.8.7.6
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

