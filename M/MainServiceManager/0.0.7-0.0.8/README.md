# Comparing `tmp/mainservicemanager-0.0.7.tar.gz` & `tmp/mainservicemanager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainservicemanager-0.0.7.tar", max compression
+gzip compressed data, was "mainservicemanager-0.0.8.tar", max compression
```

## Comparing `mainservicemanager-0.0.7.tar` & `mainservicemanager-0.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.7/README.md
--rwxr-xr-x   0        0        0      736 2024-06-02 10:53:38.000000 mainservicemanager-0.0.7/pyproject.toml
--rwxr-xr-x   0        0        0      391 2024-06-02 10:53:32.000000 mainservicemanager-0.0.7/src/MainServiceManager/__init__.py
--rwxr-xr-x   0        0        0     4291 2024-06-01 11:23:26.000000 mainservicemanager-0.0.7/src/MainServiceManager/__main__.py
--rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.7/src/MainServiceManager/api.py
--rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.7/src/MainServiceManager/server.py
--rwxr-xr-x   0        0        0     7419 2024-06-02 09:54:48.000000 mainservicemanager-0.0.7/src/MainServiceManager/server_utils.py
--rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.8/README.md
+-rwxr-xr-x   0        0        0      736 2024-06-02 10:59:59.000000 mainservicemanager-0.0.8/pyproject.toml
+-rwxr-xr-x   0        0        0      391 2024-06-02 10:59:50.000000 mainservicemanager-0.0.8/src/MainServiceManager/__init__.py
+-rwxr-xr-x   0        0        0     4387 2024-06-02 10:51:09.000000 mainservicemanager-0.0.8/src/MainServiceManager/__main__.py
+-rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.8/src/MainServiceManager/api.py
+-rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.8/src/MainServiceManager/server.py
+-rwxr-xr-x   0        0        0     7419 2024-06-02 09:54:48.000000 mainservicemanager-0.0.8/src/MainServiceManager/server_utils.py
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.8/PKG-INFO
```

### Comparing `mainservicemanager-0.0.7/README.md` & `mainservicemanager-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.7/pyproject.toml` & `mainservicemanager-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MainServiceManager"
-version = "0.0.7"
+version = "0.0.8"
 description = "Пользовательская программа для управления сервисами, аналогично systemd"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainServiceManager.py"
 packages = [
 { include = "MainServiceManager", from = "src" },
 ]
```

### Comparing `mainservicemanager-0.0.7/src/MainServiceManager/__main__.py` & `mainservicemanager-0.0.8/src/MainServiceManager/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,32 +98,32 @@
     if args.action=="stop":
       ms.json.print(launcher.admin_stop())
       return
     print("Unknown action\nAvailable actions for the server: "+", ".join(["kill","list_name","list_svc","reload","status","stop"]),file=sys.stderr)
     return
   else:
     if args.action=="close":
-      ms.json.print(launcher.svc_close())
+      ms.json.print(launcher.svc_close(args.service))
       return
     if args.action=="disable":
-      ms.json.print(launcher.svc_disable())
+      ms.json.print(launcher.svc_disable(args.service))
       return
     if args.action=="enable":
-      ms.json.print(launcher.svc_enable())
+      ms.json.print(launcher.svc_enable(args.service))
       return
     if args.action=="info":
-      ms.json.print(launcher.svc_info())
+      ms.json.print(launcher.svc_info(args.service))
       return
     if args.action=="kill":
-      ms.json.print(launcher.svc_kill())
+      ms.json.print(launcher.svc_kill(args.service))
       return
     if args.action=="restart":
-      ms.json.print(launcher.svc_restart())
+      ms.json.print(launcher.svc_restart(args.service))
       return
     if args.action=="start":
-      ms.json.print(launcher.svc_start())
+      ms.json.print(launcher.svc_start(args.service))
       return
     if args.action=="stop":
-      ms.json.print(launcher.svc_stop())
+      ms.json.print(launcher.svc_stop(args.service))
       return
     print("Unknown action\nAvailable actions for the service: "+", ".join(["close","disable","enable","info","kill","restart","start","stop"]),file=sys.stderr)
     return
```

### Comparing `mainservicemanager-0.0.7/src/MainServiceManager/api.py` & `mainservicemanager-0.0.8/src/MainServiceManager/api.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.7/src/MainServiceManager/server.py` & `mainservicemanager-0.0.8/src/MainServiceManager/server.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.7/src/MainServiceManager/server_utils.py` & `mainservicemanager-0.0.8/src/MainServiceManager/server_utils.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.7/PKG-INFO` & `mainservicemanager-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainServiceManager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Пользовательская программа для управления сервисами, аналогично systemd
 Home-page: https://github.com/MainPlay-TG/MainServiceManager.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

