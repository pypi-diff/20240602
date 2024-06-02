# Comparing `tmp/swc_utils-0.2.1.tar.gz` & `tmp/swc_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swc_utils-0.2.1.tar", last modified: Sat May 25 20:52:19 2024, max compression
+gzip compressed data, was "swc_utils-0.3.1.tar", last modified: Sun Jun  2 21:26:05 2024, max compression
```

## Comparing `swc_utils-0.2.1.tar` & `swc_utils-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.452905 swc_utils-0.2.1/
--rw-rw-rw-   0        0        0     1090 2024-05-18 12:05:04.000000 swc_utils-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      711 2024-05-25 20:52:19.451906 swc_utils-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-05-18 12:04:37.000000 swc_utils-0.2.1/README.md
--rw-rw-rw-   0        0        0      704 2024-05-25 20:52:16.000000 swc_utils-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 20:52:19.452905 swc_utils-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.428903 swc_utils-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.432908 swc_utils-0.2.1/src/swc_utils/
--rw-rw-rw-   0        0        0        0 2024-05-18 12:00:49.000000 swc_utils-0.2.1/src/swc_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.441904 swc_utils-0.2.1/src/swc_utils/database/
--rw-rw-rw-   0        0        0      105 2024-05-18 12:15:55.000000 swc_utils-0.2.1/src/swc_utils/database/__init__.py
--rw-rw-rw-   0        0        0     1068 2024-04-27 15:30:53.000000 swc_utils-0.2.1/src/swc_utils/database/connection_profile.py
--rw-rw-rw-   0        0        0      493 2024-05-18 12:01:51.000000 swc_utils-0.2.1/src/swc_utils/database/database_connection.py
--rw-rw-rw-   0        0        0     3500 2024-05-20 16:55:40.000000 swc_utils-0.2.1/src/swc_utils/database/db_table_care.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.442906 swc_utils-0.2.1/src/swc_utils/other/
--rw-rw-rw-   0        0        0       63 2024-05-18 12:34:45.000000 swc_utils-0.2.1/src/swc_utils/other/__init__.py
--rw-rw-rw-   0        0        0      619 2024-04-25 14:33:38.000000 swc_utils-0.2.1/src/swc_utils/other/generator_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.443903 swc_utils-0.2.1/src/swc_utils/routing/
--rw-rw-rw-   0        0        0        0 2024-05-23 16:26:40.000000 swc_utils-0.2.1/src/swc_utils/routing/__init__.py
--rw-rw-rw-   0        0        0     1671 2024-05-23 17:29:27.000000 swc_utils-0.2.1/src/swc_utils/routing/auth_routes.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.445906 swc_utils-0.2.1/src/swc_utils/tools/
--rw-rw-rw-   0        0        0       67 2024-05-18 12:34:45.000000 swc_utils-0.2.1/src/swc_utils/tools/__init__.py
--rw-rw-rw-   0        0        0      974 2024-05-23 16:57:16.000000 swc_utils-0.2.1/src/swc_utils/tools/config.py
--rw-rw-rw-   0        0        0      512 2024-04-25 14:07:54.000000 swc_utils-0.2.1/src/swc_utils/tools/route_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.448906 swc_utils-0.2.1/src/swc_utils/web/
--rw-rw-rw-   0        0        0      186 2024-05-18 12:34:45.000000 swc_utils-0.2.1/src/swc_utils/web/__init__.py
--rw-rw-rw-   0        0        0      542 2024-05-18 12:34:45.000000 swc_utils-0.2.1/src/swc_utils/web/adv_responses.py
--rw-rw-rw-   0        0        0     1737 2024-05-25 20:52:16.000000 swc_utils-0.2.1/src/swc_utils/web/auth_manager.py
--rw-rw-rw-   0        0        0     2524 2023-02-28 00:29:50.000000 swc_utils-0.2.1/src/swc_utils/web/request_codes.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.449906 swc_utils-0.2.1/src/swc_utils/wsl/
--rw-rw-rw-   0        0        0       87 2024-05-18 12:34:45.000000 swc_utils-0.2.1/src/swc_utils/wsl/__init__.py
--rw-rw-rw-   0        0        0      663 2024-05-18 12:34:45.000000 swc_utils-0.2.1/src/swc_utils/wsl/wsl_compatability.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:52:19.450906 swc_utils-0.2.1/src/swc_utils.egg-info/
--rw-rw-rw-   0        0        0      711 2024-05-25 20:52:19.000000 swc_utils-0.2.1/src/swc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-05-25 20:52:19.000000 swc_utils-0.2.1/src/swc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 20:52:19.000000 swc_utils-0.2.1/src/swc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-25 20:52:19.000000 swc_utils-0.2.1/src/swc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 20:52:19.000000 swc_utils-0.2.1/src/swc_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.850999 swc_utils-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-18 12:05:04.000000 swc_utils-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      711 2024-06-02 21:26:05.850999 swc_utils-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-05-18 12:04:37.000000 swc_utils-0.3.1/README.md
+-rw-rw-rw-   0        0        0      704 2024-06-02 20:05:50.000000 swc_utils-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 21:26:05.850999 swc_utils-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.817902 swc_utils-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.825998 swc_utils-0.3.1/src/swc_utils/
+-rw-rw-rw-   0        0        0        0 2024-05-18 12:00:49.000000 swc_utils-0.3.1/src/swc_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.836998 swc_utils-0.3.1/src/swc_utils/caching/
+-rw-rw-rw-   0        0        0       45 2024-06-02 11:56:26.000000 swc_utils-0.3.1/src/swc_utils/caching/__init__.py
+-rw-rw-rw-   0        0        0      930 2024-06-02 20:10:02.000000 swc_utils-0.3.1/src/swc_utils/caching/cache.py
+-rw-rw-rw-   0        0        0      770 2024-06-02 20:05:50.000000 swc_utils-0.3.1/src/swc_utils/caching/caching_service.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.839999 swc_utils-0.3.1/src/swc_utils/database/
+-rw-rw-rw-   0        0        0      105 2024-05-18 12:15:55.000000 swc_utils-0.3.1/src/swc_utils/database/__init__.py
+-rw-rw-rw-   0        0        0     1075 2024-06-02 12:12:37.000000 swc_utils-0.3.1/src/swc_utils/database/connection_profile.py
+-rw-rw-rw-   0        0        0      493 2024-05-18 12:01:51.000000 swc_utils-0.3.1/src/swc_utils/database/database_connection.py
+-rw-rw-rw-   0        0        0     3516 2024-06-02 12:12:37.000000 swc_utils-0.3.1/src/swc_utils/database/db_table_care.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.842000 swc_utils-0.3.1/src/swc_utils/other/
+-rw-rw-rw-   0        0        0       63 2024-05-18 12:34:45.000000 swc_utils-0.3.1/src/swc_utils/other/__init__.py
+-rw-rw-rw-   0        0        0      619 2024-04-25 14:33:38.000000 swc_utils-0.3.1/src/swc_utils/other/generator_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.842999 swc_utils-0.3.1/src/swc_utils/routing/
+-rw-rw-rw-   0        0        0        0 2024-05-23 16:26:40.000000 swc_utils-0.3.1/src/swc_utils/routing/__init__.py
+-rw-rw-rw-   0        0        0     1671 2024-05-23 17:29:27.000000 swc_utils-0.3.1/src/swc_utils/routing/auth_routes.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.844999 swc_utils-0.3.1/src/swc_utils/tools/
+-rw-rw-rw-   0        0        0       67 2024-05-18 12:34:45.000000 swc_utils-0.3.1/src/swc_utils/tools/__init__.py
+-rw-rw-rw-   0        0        0     1009 2024-06-02 12:12:37.000000 swc_utils-0.3.1/src/swc_utils/tools/config.py
+-rw-rw-rw-   0        0        0      512 2024-04-25 14:07:54.000000 swc_utils-0.3.1/src/swc_utils/tools/route_loader.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.847999 swc_utils-0.3.1/src/swc_utils/web/
+-rw-rw-rw-   0        0        0      186 2024-05-18 12:34:45.000000 swc_utils-0.3.1/src/swc_utils/web/__init__.py
+-rw-rw-rw-   0        0        0      564 2024-06-02 12:12:37.000000 swc_utils-0.3.1/src/swc_utils/web/adv_responses.py
+-rw-rw-rw-   0        0        0     1769 2024-06-02 12:12:37.000000 swc_utils-0.3.1/src/swc_utils/web/auth_manager.py
+-rw-rw-rw-   0        0        0     2524 2023-02-28 00:29:50.000000 swc_utils-0.3.1/src/swc_utils/web/request_codes.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.848998 swc_utils-0.3.1/src/swc_utils/wsl/
+-rw-rw-rw-   0        0        0       87 2024-05-18 12:34:45.000000 swc_utils-0.3.1/src/swc_utils/wsl/__init__.py
+-rw-rw-rw-   0        0        0      685 2024-06-02 12:12:37.000000 swc_utils-0.3.1/src/swc_utils/wsl/wsl_compatability.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:26:05.849999 swc_utils-0.3.1/src/swc_utils.egg-info/
+-rw-rw-rw-   0        0        0      711 2024-06-02 21:26:05.000000 swc_utils-0.3.1/src/swc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      957 2024-06-02 21:26:05.000000 swc_utils-0.3.1/src/swc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 21:26:05.000000 swc_utils-0.3.1/src/swc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-06-02 21:26:05.000000 swc_utils-0.3.1/src/swc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 21:26:05.000000 swc_utils-0.3.1/src/swc_utils.egg-info/top_level.txt
```

### Comparing `swc_utils-0.2.1/LICENSE` & `swc_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swc_utils-0.2.1/PKG-INFO` & `swc_utils-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swc_utils
-Version: 0.2.1
+Version: 0.3.1
 Summary: Provides utility functions for SWC projects
 Author-email: Davis_Software <davissoftware6@gmail.com>
 Project-URL: Homepage, https://gitlab.software-city.org/root/swc_utils
 Project-URL: Issues, https://gitlab.software-city.org/root/swc_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swc_utils-0.2.1/pyproject.toml` & `swc_utils-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swc_utils"
-version = "0.2.1"
+version = "0.3.1"
 authors = [
   { name="Davis_Software", email="davissoftware6@gmail.com" },
 ]
 description = "Provides utility functions for SWC projects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `swc_utils-0.2.1/src/swc_utils/database/connection_profile.py` & `swc_utils-0.3.1/src/swc_utils/database/connection_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         self.mysql_port = port
         self.mysql_database = database
         self.mysql_username = username
         self.mysql_password = password
         self.sql_type = sql_type
         
     @property
-    def connection_uri(self):
+    def connection_uri(self) -> str:
         if self.sql_type == "sqlite":
             uri_elements = [
                 'sqlite:///',
                 self.mysql_database
             ]
         elif self.sql_type == "mysql":
             uri_elements = [
```

### Comparing `swc_utils-0.2.1/src/swc_utils/database/db_table_care.py` & `swc_utils-0.3.1/src/swc_utils/database/db_table_care.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,26 @@
         self.session.close()
         return False
 
     def _log(self, message, level=INFO):
         if self.__flask_app:
             self.__flask_app.logger.log(level, message)
 
-    def find_models(self):
+    def find_models(self) -> list:
         models = list()
 
         def find_subclasses(cls):
             for subclass in cls.__subclasses__():
                 find_subclasses(subclass)
                 models.append(subclass)
 
         find_subclasses(self.base)
         return models
 
-    def find_tables(self):
+    def find_tables(self) -> dict:
         metadata = MetaData()
         metadata.reflect(bind=self.engine)
         return metadata.tables
 
     def _fix_missing_columns(self, model, missing_columns):
         for column in missing_columns:
             column = model.__table__.columns.get(column)
```

### Comparing `swc_utils-0.2.1/src/swc_utils/other/generator_utils.py` & `swc_utils-0.3.1/src/swc_utils/other/generator_utils.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.2.1/src/swc_utils/routing/auth_routes.py` & `swc_utils-0.3.1/src/swc_utils/routing/auth_routes.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.2.1/src/swc_utils/tools/config.py` & `swc_utils-0.3.1/src/swc_utils/tools/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,18 @@
                     key, value = line.split('=')
                     config[key] = value
         return config
 
     def __getitem__(self, item):
         return self.get(item)
 
-    def get(self, key: str, default: str = None):
+    def get(self, key: str, default: str = None) -> str:
         return self.__config.get(key, default)
 
-    def get_bool(self, key: str, default: bool = None):
+    def get_bool(self, key: str, default: bool = None) -> bool:
         return self.get(key, default) in ['True', 'true', '1']
 
-    def get_list(self, key: str, default: list[str] = None):
+    def get_list(self, key: str, default: list[str] = None) -> list[str]:
         return self.get(key, default).split(',')
 
-    def get_int(self, key: str, default: int = None):
+    def get_int(self, key: str, default: int = None) -> int:
         return int(self.get(key, default))
```

### Comparing `swc_utils-0.2.1/src/swc_utils/tools/route_loader.py` & `swc_utils-0.3.1/src/swc_utils/tools/route_loader.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.2.1/src/swc_utils/web/adv_responses.py` & `swc_utils-0.3.1/src/swc_utils/web/adv_responses.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
-from flask import make_response, send_file
+from flask import make_response, send_file, Response
 
 from .request_codes import RequestCode
 
 
-def send_binary_image(data, content_type="image/jpeg", cache_control=3600):
+def send_binary_image(data, content_type="image/jpeg", cache_control=3600) -> Response:
     if data is None:
         return make_response(
             send_file("static/img/noimage.png"),
             # RequestCode.ClientError.NotFound
             RequestCode.Success.OK
         )
```

### Comparing `swc_utils-0.2.1/src/swc_utils/web/auth_manager.py` & `swc_utils-0.3.1/src/swc_utils/web/auth_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from copy import copy
 from functools import wraps
 from .request_codes import RequestCode
 from flask import session, request, abort, redirect
 
 
-def check_auth():
+def check_auth() -> bool:
     return session.get("user") is not None
 
 
-def check_admin():
+def check_admin() -> bool:
     return (session.get("user") or {}).get("admin", False)
 
 
-def get_namespaced_permissions(namespace: str):
+def get_namespaced_permissions(namespace: str) -> list:
     if not check_auth():
         return []
 
     permissions = (session.get("user") or {}).get("permissions", {})
     perm_list = copy(permissions.get(namespace, []))
     perm_list.extend(permissions.get("*", []))
 
     return perm_list
 
 
-def check_permission(namespace: str, permission: str):
+def check_permission(namespace: str, permission: str) -> bool:
     if not check_auth():
         return False
 
     if check_admin():
         return True
 
     namespaced_permissions = get_namespaced_permissions(namespace)
```

### Comparing `swc_utils-0.2.1/src/swc_utils/web/request_codes.py` & `swc_utils-0.3.1/src/swc_utils/web/request_codes.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.2.1/src/swc_utils/wsl/wsl_compatability.py` & `swc_utils-0.3.1/src/swc_utils/wsl/wsl_compatability.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from ..tools.config import Config
 
 
-def get_wsl_path(config: Config, path: str):
+def get_wsl_path(config: Config, path: str) -> str:
     if not config.get_bool("USE_WSL", False):
         return path
 
     path_parts = path.split(":\\")
     return f"/mnt/{path_parts[0].lower()}/" + path_parts[1].replace('\\', '/')
 
 
-def make_wsl_command(config: Config, command: list):
+def make_wsl_command(config: Config, command: list) -> list:
     if not config.get_bool("USE_WSL", False):
         return command
 
     dist = config["WSL_DISTRO"]
     return ["wsl", "-d", dist, *command]
 
 
-def get_local_wsl_temp_dir(config: Config):
+def get_local_wsl_temp_dir(config: Config) -> str:
     if not config.get_bool("USE_WSL", False):
         return "/tmp/"
 
     return f"\\\\wsl.localhost\\{config['WSL_DISTRO']}\\tmp\\"
```

### Comparing `swc_utils-0.2.1/src/swc_utils.egg-info/PKG-INFO` & `swc_utils-0.3.1/src/swc_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swc_utils
-Version: 0.2.1
+Version: 0.3.1
 Summary: Provides utility functions for SWC projects
 Author-email: Davis_Software <davissoftware6@gmail.com>
 Project-URL: Homepage, https://gitlab.software-city.org/root/swc_utils
 Project-URL: Issues, https://gitlab.software-city.org/root/swc_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swc_utils-0.2.1/src/swc_utils.egg-info/SOURCES.txt` & `swc_utils-0.3.1/src/swc_utils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 pyproject.toml
 src/swc_utils/__init__.py
 src/swc_utils.egg-info/PKG-INFO
 src/swc_utils.egg-info/SOURCES.txt
 src/swc_utils.egg-info/dependency_links.txt
 src/swc_utils.egg-info/requires.txt
 src/swc_utils.egg-info/top_level.txt
+src/swc_utils/caching/__init__.py
+src/swc_utils/caching/cache.py
+src/swc_utils/caching/caching_service.py
 src/swc_utils/database/__init__.py
 src/swc_utils/database/connection_profile.py
 src/swc_utils/database/database_connection.py
 src/swc_utils/database/db_table_care.py
 src/swc_utils/other/__init__.py
 src/swc_utils/other/generator_utils.py
 src/swc_utils/routing/__init__.py
```

