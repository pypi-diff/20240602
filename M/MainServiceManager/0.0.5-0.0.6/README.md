# Comparing `tmp/mainservicemanager-0.0.5.tar.gz` & `tmp/mainservicemanager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainservicemanager-0.0.5.tar", max compression
+gzip compressed data, was "mainservicemanager-0.0.6.tar", max compression
```

## Comparing `mainservicemanager-0.0.5.tar` & `mainservicemanager-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.5/README.md
--rwxr-xr-x   0        0        0      736 2024-06-01 11:25:31.000000 mainservicemanager-0.0.5/pyproject.toml
--rwxr-xr-x   0        0        0      391 2024-06-01 11:25:24.000000 mainservicemanager-0.0.5/src/MainServiceManager/__init__.py
--rwxr-xr-x   0        0        0     4331 2024-06-01 11:17:54.000000 mainservicemanager-0.0.5/src/MainServiceManager/__main__.py
--rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.5/src/MainServiceManager/api.py
--rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.5/src/MainServiceManager/server.py
--rwxr-xr-x   0        0        0     6876 2024-06-01 09:36:36.000000 mainservicemanager-0.0.5/src/MainServiceManager/server_utils.py
--rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.6/README.md
+-rwxr-xr-x   0        0        0      736 2024-06-01 11:28:18.000000 mainservicemanager-0.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0      391 2024-06-01 11:28:12.000000 mainservicemanager-0.0.6/src/MainServiceManager/__init__.py
+-rwxr-xr-x   0        0        0     4291 2024-06-01 11:23:27.000000 mainservicemanager-0.0.6/src/MainServiceManager/__main__.py
+-rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.6/src/MainServiceManager/api.py
+-rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.6/src/MainServiceManager/server.py
+-rwxr-xr-x   0        0        0     6876 2024-06-01 09:36:36.000000 mainservicemanager-0.0.6/src/MainServiceManager/server_utils.py
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.6/PKG-INFO
```

### Comparing `mainservicemanager-0.0.5/README.md` & `mainservicemanager-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.5/pyproject.toml` & `mainservicemanager-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MainServiceManager"
-version = "0.0.5"
+version = "0.0.6"
 description = "Пользовательская программа для управления сервисами, аналогично systemd"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainServiceManager.py"
 packages = [
 { include = "MainServiceManager", from = "src" },
 ]
```

### Comparing `mainservicemanager-0.0.5/src/MainServiceManager/__main__.py` & `mainservicemanager-0.0.6/src/MainServiceManager/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,19 +41,17 @@
     )
   argp.add_argument("-P","--pass",
     default=None,
     help="password. If absent, the input from the keyboard will be requested",
     )
   argp.add_argument("action",
     help="the action performed with the service",
-    required=True,
     )
   argp.add_argument("service",
     help='service name. To control the server, write "admin"',
-    required=True,
     )
   args=argp.parse_args()
   try:
     if args.config:
       cfg=ms.json.read(args.config)
     else:
       cfg=ms.json.read(os.path.expanduser("~/.config/MainServiceManager/cfg.json"))
```

### Comparing `mainservicemanager-0.0.5/src/MainServiceManager/api.py` & `mainservicemanager-0.0.6/src/MainServiceManager/api.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.5/src/MainServiceManager/server.py` & `mainservicemanager-0.0.6/src/MainServiceManager/server.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.5/src/MainServiceManager/server_utils.py` & `mainservicemanager-0.0.6/src/MainServiceManager/server_utils.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.5/PKG-INFO` & `mainservicemanager-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainServiceManager
-Version: 0.0.5
+Version: 0.0.6
 Summary: Пользовательская программа для управления сервисами, аналогично systemd
 Home-page: https://github.com/MainPlay-TG/MainServiceManager.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

