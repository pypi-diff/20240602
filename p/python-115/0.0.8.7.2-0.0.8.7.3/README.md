# Comparing `tmp/python_115-0.0.8.7.2.tar.gz` & `tmp/python_115-0.0.8.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.7.2.tar", max compression
+gzip compressed data, was "python_115-0.0.8.7.3.tar", max compression
```

## Comparing `python_115-0.0.8.7.2.tar` & `python_115-0.0.8.7.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.2/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.2/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.2/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.2/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     2140 2024-05-30 07:46:16.964139 python_115-0.0.8.7.2/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.2/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.2/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.2/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.2/p115/cmd/init.py
--rwxr-xr-x   0        0        0     9236 2024-05-30 07:46:53.430209 python_115-0.0.8.7.2/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2106 2024-05-30 07:46:42.588507 python_115-0.0.8.7.2/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.2/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.2/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.2/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.2/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.2/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.2/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.2/p115/component/cipher.py
--rwxr-xr-x   0        0        0   259970 2024-05-30 10:53:37.994316 python_115-0.0.8.7.2/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.2/p115/component/exception.py
--rwxr-xr-x   0        0        0    66130 2024-05-28 15:26:11.565966 python_115-0.0.8.7.2/p115/component/fs.py
--rwxr-xr-x   0        0        0    48262 2024-05-28 15:24:40.699422 python_115-0.0.8.7.2/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.7.2/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.7.2/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.2/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.7.2/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.2/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.2/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.2/p115/py.typed
--rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.2/p115/tool/__init__.py
--rw-r--r--   0        0        0     1681 2024-05-30 17:44:35.526874 python_115-0.0.8.7.2/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.7.2/readme.md
--rw-r--r--   0        0        0    36399 1970-01-01 00:00:00.000000 python_115-0.0.8.7.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.3/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.3/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.3/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.3/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     2394 2024-06-01 07:45:37.499962 python_115-0.0.8.7.3/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.3/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.3/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.3/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.3/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     9484 2024-06-01 07:45:44.611935 python_115-0.0.8.7.3/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2107 2024-06-01 06:14:01.276468 python_115-0.0.8.7.3/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.3/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.3/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.3/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.3/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.3/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.3/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.3/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   260065 2024-06-01 14:51:20.075255 python_115-0.0.8.7.3/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.3/p115/component/exception.py
+-rwxr-xr-x   0        0        0    66187 2024-06-02 01:30:47.597931 python_115-0.0.8.7.3/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48262 2024-05-28 15:24:40.699422 python_115-0.0.8.7.3/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.7.3/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.7.3/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.3/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.7.3/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.3/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.3/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.3/p115/py.typed
+-rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.3/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1687 2024-06-02 01:31:52.953245 python_115-0.0.8.7.3/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.7.3/readme.md
+-rw-r--r--   0        0        0    36409 1970-01-01 00:00:00.000000 python_115-0.0.8.7.3/PKG-INFO
```

### Comparing `python_115-0.0.8.7.2/LICENSE` & `python_115-0.0.8.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/cmd/check.py` & `python_115-0.0.8.7.3/p115/cmd/check.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,34 +22,41 @@
 def main(args):
     from p115 import P115Client, __version__
 
     if args.version:
         print(".".join(map(str, __version__)))
         raise SystemExit(0)
 
-    from os.path import expanduser, dirname, join as joinpath
+    from os.path import expanduser, dirname, join as joinpath, realpath
     from sys import stdout
 
     cookies = args.cookies
+    cookie_path = None
     if not cookies:
+        seen = set()
         for dir_ in (".", expanduser("~"), dirname(__file__)):
+            dir_ = realpath(dir_)
+            if dir_ in seen:
+                continue
+            seen.add(dir_)
             try:
                 cookies = open(joinpath(dir_, "115-cookies.txt")).read()
                 if cookies:
+                    cookie_path = joinpath(dir_, "115-cookies.txt")
                     break
             except FileNotFoundError:
                 pass
 
     client = P115Client(cookies, app=args.app)
-    if client.cookies != cookies:
+    if cookie_path and client.cookies != cookies:
         open("115-cookies.txt", "w").write(client.cookies)
     print(client.user_points_sign_post())
 
 
-parser.add_argument("-c", "--cookies", help="115 登录 cookie，如果缺失，则从 115-cookies.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
+parser.add_argument("-c", "--cookies", help="115 登录 cookies，如果缺失，则从 115-cookies.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
 parser.add_argument(
     "-a", "--app", default="qandroid", 
     choices=(
         "web", "ios", "115ios", "android", "115android", "115ipad", "tv", "qandroid", 
         "windows", "mac", "linux", "wechatmini", "alipaymini"), 
     help="必要时，选择一个 app 进行扫码登录，默认值 'qandroid'，注意：这会把已经登录的相同 app 踢下线")
 parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
```

### Comparing `python_115-0.0.8.7.2/p115/cmd/iterdir.py` & `python_115-0.0.8.7.3/p115/cmd/iterdir.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,31 +28,38 @@
 def main(args):
     from p115 import P115Client, P115Path, __version__
 
     if args.version:
         print(".".join(map(str, __version__)))
         raise SystemExit(0)
 
-    from os.path import expanduser, dirname, join as joinpath
+    from os.path import expanduser, dirname, join as joinpath, realpath
     from sys import stdout
     from typing import Callable
 
     cookies = args.cookies
+    cookie_path = None
     if not cookies:
+        seen = set()
         for dir_ in (".", expanduser("~"), dirname(__file__)):
+            dir_ = realpath(dir_)
+            if dir_ in seen:
+                continue
+            seen.add(dir_)
             try:
                 cookies = open(joinpath(dir_, "115-cookies.txt")).read()
                 if cookies:
+                    cookie_path = joinpath(dir_, "115-cookies.txt")
                     break
             except FileNotFoundError:
                 pass
 
     client = P115Client(cookies, app=args.app)
-    if client.cookies != cookies:
-        open("115-cookies.txt", "w").write(client.cookies)
+    if cookie_path and cookies != client.cookies:
+        open(cookie_path, "w").write(client.cookies)
 
     fs = client.fs
 
     if args.password and not fs.hidden_mode:
         fs.hidden_switch(True, password=args.password)
 
     keys = args.keys or KEYS
@@ -205,15 +212,15 @@
         from sys import stderr
         stderr.close()
     finally:
         file.close()
 
 
 parser.add_argument("path", nargs="?", default="0", help="文件夹路径或 id，默认值 0，即根目录")
-parser.add_argument("-c", "--cookies", help="115 登录 cookie，如果缺失，则从 115-cookies.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
+parser.add_argument("-c", "--cookies", help="115 登录 cookies，如果缺失，则从 115-cookies.txt 文件中获取，此文件可以在 当前工作目录、此脚本所在目录 或 用户根目录 下")
 parser.add_argument(
     "-a", "--app", default="qandroid", 
     choices=(
         "web", "ios", "115ios", "android", "115android", "115ipad", "tv", "qandroid", 
         "windows", "mac", "linux", "wechatmini", "alipaymini"), 
     help="必要时，选择一个 app 进行扫码登录，默认值 'qandroid'，注意：这会把已经登录的相同 app 踢下线")
 parser.add_argument("-p", "--password", help="密码，用于进入隐藏模式，罗列隐藏文件")
```

### Comparing `python_115-0.0.8.7.2/p115/cmd/qrcode.py` & `python_115-0.0.8.7.3/p115/cmd/qrcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 parser.add_argument(
     "app", nargs="?", default="qandroid", 
     choices=(
         "web", "ios", "115ios", "android", "115android", "115ipad", "tv", "qandroid", 
         "windows", "mac", "linux", "wechatmini", "alipaymini"),        
     help="选择一个 app 进行登录，默认值 'qandroid'，注意：这会把已经登录的相同 app 踢下线")
 parser.add_argument("-o", "--output-file", help="保存到文件，未指定时输出到 stdout")
-parser.add_argument("-c", "--cookies", help="115 登录 cookie，如果提供了，就可以用这个 cookies 进行自动扫码，否则需要你用手机来手动扫码")
+parser.add_argument("-c", "--cookies", help="115 登录 cookies，如果提供了，就可以用这个 cookies 进行自动扫码，否则需要你用手机来手动扫码")
 parser.add_argument("-v", "--version", action="store_true", help="输出版本号")
 parser.set_defaults(func=main)
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     main(args)
```

### Comparing `python_115-0.0.8.7.2/p115/component/__init__.py` & `python_115-0.0.8.7.3/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/cipher.py` & `python_115-0.0.8.7.3/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/client.py` & `python_115-0.0.8.7.3/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 
 RequestVarT = TypeVar("RequestVarT", dict, Callable)
 RSA_ENCODER: Final = P115RSACipher()
 ECDH_ENCODER: Final = P115ECDHCipher()
 CRE_SHARE_LINK_search = re_compile(r"/s/(?P<share_code>\w+)(\?password=(?P<receive_code>\w+))?").search
 APP_VERSION: Final = "99.99.99.99"
 
-request = partial(httpx_request, parse=lambda _, content: loads(content), timeout=60)
+# TODO: 一部分 POST 请求也要在 ReadTimeout时重试
+request = partial(httpx_request, parse=lambda _, content: loads(content), timeout=(5, 60, 60, 5), raise_for_status=True)
 
 
 def to_base64(s: bytes | str, /) -> str:
     if isinstance(s, str):
         s = bytes(s, "utf-8")
     return str(b64encode(s), "ascii")
```

### Comparing `python_115-0.0.8.7.2/p115/component/fs.py` & `python_115-0.0.8.7.3/p115/component/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         info2["described"] = bool(info["fdes"])
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
```

### Comparing `python_115-0.0.8.7.2/p115/component/fs_base.py` & `python_115-0.0.8.7.3/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/fs_share.py` & `python_115-0.0.8.7.3/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/fs_zip.py` & `python_115-0.0.8.7.3/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/labellist.py` & `python_115-0.0.8.7.3/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/offline.py` & `python_115-0.0.8.7.3/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/recyclebin.py` & `python_115-0.0.8.7.3/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/component/sharing.py` & `python_115-0.0.8.7.3/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/p115/tool/__init__.py` & `python_115-0.0.8.7.3/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/pyproject.toml` & `python_115-0.0.8.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.7.2"
+version = "0.0.8.7.3"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
@@ -28,15 +28,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 cachetools = "*"
 ecdsa = "*"
 glob_pattern = "*"
 http_response = "*"
 httpx = "*"
-httpx_request = "*"
+httpx_request = ">=0.0.6"
 lz4 = "*"
 magnet2torrent = "*"
 multidict = "*"
 posixpatht = "*"
 pycryptodome = "*"
 python-asynctools = "*"
 python-concurrenttools = "*"
```

### Comparing `python_115-0.0.8.7.2/readme.md` & `python_115-0.0.8.7.3/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.2/PKG-INFO` & `python_115-0.0.8.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.7.2
+Version: 0.0.8.7.3
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cachetools
 Requires-Dist: ecdsa
 Requires-Dist: glob_pattern
 Requires-Dist: http_response
 Requires-Dist: httpx
-Requires-Dist: httpx_request
+Requires-Dist: httpx_request (>=0.0.6)
 Requires-Dist: lz4
 Requires-Dist: magnet2torrent
 Requires-Dist: multidict
 Requires-Dist: posixpatht
 Requires-Dist: pycryptodome
 Requires-Dist: python-asynctools
 Requires-Dist: python-concurrenttools
```

