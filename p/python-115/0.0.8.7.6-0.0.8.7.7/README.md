# Comparing `tmp/python_115-0.0.8.7.6.tar.gz` & `tmp/python_115-0.0.8.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.7.6.tar", max compression
+gzip compressed data, was "python_115-0.0.8.7.7.tar", max compression
```

## Comparing `python_115-0.0.8.7.6.tar` & `python_115-0.0.8.7.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.6/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.6/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.6/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.6/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     2394 2024-06-01 07:45:37.499962 python_115-0.0.8.7.6/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.6/p115/cmd/init.py
--rwxr-xr-x   0        0        0     9484 2024-06-01 07:45:44.611935 python_115-0.0.8.7.6/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2107 2024-06-01 06:14:01.276468 python_115-0.0.8.7.6/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.6/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.6/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.6/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.6/p115/component/cipher.py
--rwxr-xr-x   0        0        0   265176 2024-06-02 07:24:06.942442 python_115-0.0.8.7.6/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.6/p115/component/exception.py
--rwxr-xr-x   0        0        0    69258 2024-06-02 07:24:57.713675 python_115-0.0.8.7.6/p115/component/fs.py
--rwxr-xr-x   0        0        0    49142 2024-06-02 06:13:46.742966 python_115-0.0.8.7.6/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    15205 2024-06-02 05:55:36.365281 python_115-0.0.8.7.6/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10263 2024-06-02 05:51:11.710739 python_115-0.0.8.7.6/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.6/p115/component/labellist.py
--rwxr-xr-x   0        0        0    10286 2024-06-02 06:30:40.250415 python_115-0.0.8.7.6/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.6/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.6/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.6/p115/py.typed
--rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.6/p115/tool/__init__.py
--rw-r--r--   0        0        0     1687 2024-06-02 07:25:34.828005 python_115-0.0.8.7.6/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-06-02 05:53:33.629676 python_115-0.0.8.7.6/readme.md
--rw-r--r--   0        0        0    36409 1970-01-01 00:00:00.000000 python_115-0.0.8.7.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.7/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.7/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.7/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.7/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     2394 2024-06-01 07:45:37.499962 python_115-0.0.8.7.7/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.7/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.7/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.7/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.7/p115/cmd/init.py
+-rwxr-xr-x   0        0        0    10048 2024-06-02 09:13:32.245014 python_115-0.0.8.7.7/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2107 2024-06-01 06:14:01.276468 python_115-0.0.8.7.7/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.7/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.7/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.7/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.7/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.7/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.7/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.7/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   265176 2024-06-02 07:24:06.942442 python_115-0.0.8.7.7/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.7/p115/component/exception.py
+-rwxr-xr-x   0        0        0    69258 2024-06-02 07:24:57.713675 python_115-0.0.8.7.7/p115/component/fs.py
+-rwxr-xr-x   0        0        0    49142 2024-06-02 06:13:46.742966 python_115-0.0.8.7.7/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    15205 2024-06-02 05:55:36.365281 python_115-0.0.8.7.7/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10263 2024-06-02 05:51:11.710739 python_115-0.0.8.7.7/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.7/p115/component/labellist.py
+-rwxr-xr-x   0        0        0    10286 2024-06-02 06:30:40.250415 python_115-0.0.8.7.7/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.7/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.7/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.7/p115/py.typed
+-rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.7/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1687 2024-06-02 09:13:41.166410 python_115-0.0.8.7.7/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-06-02 05:53:33.629676 python_115-0.0.8.7.7/readme.md
+-rw-r--r--   0        0        0    36409 1970-01-01 00:00:00.000000 python_115-0.0.8.7.7/PKG-INFO
```

### Comparing `python_115-0.0.8.7.6/LICENSE` & `python_115-0.0.8.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/cmd/check.py` & `python_115-0.0.8.7.7/p115/cmd/check.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/cmd/iterdir.py` & `python_115-0.0.8.7.7/p115/cmd/iterdir.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__: list[str] = []
 __doc__ = "115 文件夹信息遍历导出"
 
 KEYS = (
-    "id", "parent_id", "name", "path", "relpath", "sha1", "pickcode", "is_directory", 
-    "size", "ctime", "mtime", "atime", "hidden", "violated", "play_long", "thumb", 
-    "star", "score", "labels", "description", 
+    "id", "parent_id", "name", "path", "relpath", "size", "sha1", "pickcode", 
+    "is_directory", "ctime", "mtime", "atime", "hidden", "violated", "play_long", 
+    "thumb", "star", "score", "labels", "description", 
 )
 
 if __name__ == "__main__":
     from argparse import ArgumentParser, RawTextHelpFormatter
     from pathlib import Path
     from sys import path
 
@@ -28,17 +28,17 @@
 def main(args):
     from p115 import P115Client, P115Path, __version__
 
     if args.version:
         print(".".join(map(str, __version__)))
         raise SystemExit(0)
 
+    from collections.abc import Callable, Sequence
     from os.path import expanduser, dirname, join as joinpath, realpath
     from sys import stdout
-    from typing import Callable
 
     cookies = args.cookies
     cookie_path = None
     if not cookies:
         seen = set()
         for dir_ in (".", expanduser("~"), dirname(__file__)):
             dir_ = realpath(dir_)
@@ -58,15 +58,23 @@
         open(cookie_path, "w").write(client.cookies)
 
     fs = client.fs
 
     if args.password and not fs.hidden_mode:
         fs.hidden_switch(True, password=args.password)
 
-    keys = args.keys or KEYS
+    keys: Sequence[str]
+    if args.kind_keys:
+        keys = ["id", "parent_id", "name", "path", "relpath", "size", "sha1", "pickcode", "is_directory"]
+        if args.keys:
+            for k in args.keys:
+                if k not in keys:
+                    keys.append(k)
+    else:
+        keys = args.keys or KEYS
     output_type = args.output_type
 
     path = args.path
     if path.isdecimal():
         fid = int(path)
         attr = fs.attr(fid)
     else:
@@ -159,15 +167,18 @@
             if result:
                 write(result)
                 write(b"\n")
         return
 
     def get_key(path: P115Path, key: str):
         if key == "description":
-            return path.desc
+            if path.get('described'):
+                return path.desc
+            else:
+                return ""
         elif key == "relpath":
             return path["path"][top_start:]
         else:
             return path.get(key)
 
     records = ({k: get_key(p, k) for k in keys} for p in path_it)
 
@@ -222,14 +233,15 @@
     choices=(
         "web", "ios", "115ios", "android", "115android", "115ipad", "tv", "qandroid", 
         "windows", "mac", "linux", "wechatmini", "alipaymini"), 
     help="必要时，选择一个 app 进行扫码登录，默认值 'qandroid'，注意：这会把已经登录的相同 app 踢下线")
 parser.add_argument("-p", "--password", help="密码，用于进入隐藏模式，罗列隐藏文件")
 parser.add_argument("-s", "--select", help="提供一个表达式（会注入一个变量 path，类型是 p115.P115Path），用于对路径进行筛选")
 parser.add_argument("-k", "--keys", nargs="*", choices=KEYS, help=f"选择输出的 key，默认输出所有可选值")
+parser.add_argument("-kk", "--kind-keys", action="store_true", help="帮你选好的一组 key，相当于：-k id parent_id name path size sha1 pickcode is_directory")
 parser.add_argument("-t", "--output-type", choices=("log", "json", "csv"), default="log", help="""\
 输出类型，默认为 log
     - log   每行输出一条数据，每条数据输出为一个 json 的 object
     - json  输出一个 json 的 list，每条数据输出为一个 json 的 object
     - csv   输出一个 csv，第 1 行为表头，以后每行输出一条数据""")
 parser.add_argument("-d", "--dump", default="", help="""\
 (优先级高于 -k/--keys 和 -t/--output-type) 提供一段代码，每次调用，再行输出，尾部会添加一个 b'\n'。
```

### Comparing `python_115-0.0.8.7.6/p115/cmd/qrcode.py` & `python_115-0.0.8.7.7/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/__init__.py` & `python_115-0.0.8.7.7/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/cipher.py` & `python_115-0.0.8.7.7/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/client.py` & `python_115-0.0.8.7.7/p115/component/client.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/fs.py` & `python_115-0.0.8.7.7/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/fs_base.py` & `python_115-0.0.8.7.7/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/fs_share.py` & `python_115-0.0.8.7.7/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/fs_zip.py` & `python_115-0.0.8.7.7/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/labellist.py` & `python_115-0.0.8.7.7/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/offline.py` & `python_115-0.0.8.7.7/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/recyclebin.py` & `python_115-0.0.8.7.7/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/component/sharing.py` & `python_115-0.0.8.7.7/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/p115/tool/__init__.py` & `python_115-0.0.8.7.7/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/pyproject.toml` & `python_115-0.0.8.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.7.6"
+version = "0.0.8.7.7"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.7.6/readme.md` & `python_115-0.0.8.7.7/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.6/PKG-INFO` & `python_115-0.0.8.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.7.6
+Version: 0.0.8.7.7
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

