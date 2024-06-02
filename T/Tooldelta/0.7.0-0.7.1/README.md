# Comparing `tmp/tooldelta-0.7.0.tar.gz` & `tmp/tooldelta-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.7.0.tar", max compression
+gzip compressed data, was "tooldelta-0.7.1.tar", max compression
```

## Comparing `tooldelta-0.7.0.tar` & `tooldelta-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1497 2024-06-01 21:51:42.622132 tooldelta-0.7.0/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-06-01 21:51:42.622132 tooldelta-0.7.0/README.md
--rw-r--r--   0        0        0      908 2024-06-01 21:51:51.138192 tooldelta-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0      658 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/auths.py
--rwxr-xr-x   0        0        0    12563 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10441 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/color_print.py
--rw-r--r--   0        0        0     1885 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/constants.py
--rwxr-xr-x   0        0        0    35071 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/frame.py
--rwxr-xr-x   0        0        0    13369 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-06-01 21:51:42.622132 tooldelta-0.7.0/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    23814 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1832 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/logger.py
--rw-r--r--   0        0        0    29752 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1295 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/packets.py
--rwxr-xr-x   0        0        0    16729 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3504 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     9072 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0    10499 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     6318 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/movent.py
--rw-r--r--   0        0        0     7032 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_load/utils.py
--rwxr-xr-x   0        0        0    17204 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16997 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1932 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/starter.py
--rwxr-xr-x   0        0        0     1110 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0    10074 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/urlmethod.py
--rw-r--r--   0        0        0    20711 2024-06-01 21:51:42.626132 tooldelta-0.7.0/tooldelta/utils.py
--rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 tooldelta-0.7.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-06-01 22:12:10.500592 tooldelta-0.7.1/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-06-01 22:12:10.500592 tooldelta-0.7.1/README.md
+-rw-r--r--   0        0        0      908 2024-06-01 22:12:19.684632 tooldelta-0.7.1/pyproject.toml
+-rwxr-xr-x   0        0        0      658 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    12563 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10441 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1885 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/constants.py
+-rwxr-xr-x   0        0        0    35071 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/frame.py
+-rwxr-xr-x   0        0        0    13369 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    23814 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1832 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/logger.py
+-rw-r--r--   0        0        0    29752 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1295 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    16677 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3504 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     9072 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0    10499 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     6318 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/movent.py
+-rw-r--r--   0        0        0     7032 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/utils.py
+-rwxr-xr-x   0        0        0    17350 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    17116 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1932 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/starter.py
+-rwxr-xr-x   0        0        0     1110 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9870 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0    20711 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/utils.py
+-rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 tooldelta-0.7.1/PKG-INFO
```

### Comparing `tooldelta-0.7.0/LICENSE` & `tooldelta-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/README.md` & `tooldelta-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/pyproject.toml` & `tooldelta-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.7.0" # This field is automatically set to the value in the version file
+version = "0.7.1" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.7.0/tooldelta/__init__.py` & `tooldelta-0.7.1/tooldelta/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/auths.py` & `tooldelta-0.7.1/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/cfg.py` & `tooldelta-0.7.1/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/color_print.py` & `tooldelta-0.7.1/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/constants.py` & `tooldelta-0.7.1/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/frame.py` & `tooldelta-0.7.1/tooldelta/frame.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/game_texts.py` & `tooldelta-0.7.1/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/launch_cli.py` & `tooldelta-0.7.1/tooldelta/launch_cli.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/launch_options.py` & `tooldelta-0.7.1/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/logger.py` & `tooldelta-0.7.1/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/neo_conn.py` & `tooldelta-0.7.1/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/packets.py` & `tooldelta-0.7.1/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.7.1/tooldelta/plugin_load/PluginGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,14 @@
             from outer_api import api_cls_xx
             p_api = plugins.instant_plugin_api(api_cls_xx)
         ```
         """
         for v in self.plugins_api.values():
             if isinstance(v, api_cls):
                 return v
-            else:
-                print(api_cls, v)
         raise ValueError(f"无法找到API插件类 {api_cls.__name__}, 有可能是还没有注册")
 
 
     def add_packet_listener(self, pktID: int | list[int]):
         """
         添加数据包监听器
         将下面的方法作为一个MC数据包接收器
```

### Comparing `tooldelta-0.7.0/tooldelta/plugin_load/__init__.py` & `tooldelta-0.7.1/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.7.1/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/plugin_load/utils.py` & `tooldelta-0.7.1/tooldelta/plugin_load/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/plugin_manager.py` & `tooldelta-0.7.1/tooldelta/plugin_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             elif r1 == "u":
                 self.update_all_plugins(
                     self.get_plugin_reg_name_dict_and_datas()[1]
                 )
             else:
                 res = self.search_plugin(r, plugins)
                 if res is None:
-                    input()
+                    input("[Enter键继续..]")
                 else:
                     self.plugin_operation(res)
             clear_screen()
 
     def plugin_operation(self, plugin: PluginRegData) -> None:
         """插件操作
 
@@ -94,15 +94,15 @@
                     return
                 plugin_dir = os.path.join("插件文件", f_dirname, plugin.name)
                 shutil.rmtree(
                     plugin_dir + ("+disabled" if not plugin.is_enabled else "")
                 )
                 Print.clean_print(f"§a已成功删除插件 {plugin.name}, 回车键继续")
                 self.pop_plugin_reg_data(plugin)
-                input()
+                input("[Enter键继续..]")
                 return
             case "2":
                 latest_version = market.get_latest_plugin_version(
                     plugin.plugin_id)
                 if latest_version is None:
                     Print.clean_print("§6无法获取其的最新版本, 回车键继续")
                 elif latest_version == plugin.version_str:
@@ -175,14 +175,15 @@
     def update_plugin_from_market(self, plugin: PluginRegData):
         """
         更新单个插件, 并且删除旧目录
 
         Args:
             plugin (PluginRegData): 插件注册信息, 新旧皆可
         """
+        Print.clean_print(f"§6正在获取插件 §f{plugin.name}§6 的在线插件数据..", end="\r")
         _, old_plugins = self.get_plugin_reg_name_dict_and_datas()
         new_plugin_datas = market.get_plugin_data_from_market(plugin.plugin_id)
         new_plugins = market.download_plugin(new_plugin_datas, False)
         for new_plugin in new_plugins:
             for old_plugin in old_plugins:
                 if new_plugin.plugin_id == old_plugin.plugin_id and new_plugin.name != old_plugin.name:
                     shutil.rmtree(old_plugin.dir)
```

### Comparing `tooldelta-0.7.0/tooldelta/plugin_market.py` & `tooldelta-0.7.1/tooldelta/plugin_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,18 +315,19 @@
         if self.plugin_id_name_map is None:
             self.plugin_id_name_map = self.get_plugin_id_name_map()
         pres = [plugin_data]
         download_paths = self.find_dirs(plugin_data)
         if with_pres:
             for plugin_id in plugin_data.pre_plugins:
                 plugin_name = self.plugin_id_name_map[plugin_id]
-                Print.clean_print(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
+                Print.clean_print(f"§6正在下载 §f{plugin_data.name}§6 的前置插件 §f{plugin_name}")
                 plugin_datas = self.get_plugin_data_from_market(plugin_id)
                 pres += self.download_plugin(plugin_datas)
         cache_dir = tempfile.mkdtemp()
+        Print.clean_print(f"§6正在下载插件 §f{plugin_data.name}§6.." + " "*15, end="\r")
         try:
             for paths in download_paths:
                 if not paths.strip():
                     Print.print_war("下载路径为空, 跳过")
                     continue
                 url = url_join(self.plugins_download_url, paths)
                 # Determine download path based on plugin type
@@ -363,15 +364,15 @@
                         target_path, os.path.relpath(source_file, cache_dir)
                     )
                     os.makedirs(os.path.dirname(target_file), exist_ok=True)
                     shutil.move(source_file, target_file)
             from .plugin_manager import plugin_manager
             plugin_manager.push_plugin_reg_data(
                 self.get_plugin_data_from_market(plugin_data.plugin_id))
-            Print.clean_print(f"§a成功下载插件 §f{plugin_data.name}§a 至插件文件夹")
+            Print.clean_print(f"§a成功下载插件 §f{plugin_data.name}§a 至插件文件夹" + " "*15)
         finally:
             shutil.rmtree(cache_dir)
         return pres
 
     def find_dirs(self, plugin_data: PluginRegData) -> list[str]:
         """查找插件目录
```

### Comparing `tooldelta-0.7.0/tooldelta/starter.py` & `tooldelta-0.7.1/tooldelta/starter.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/sys_args.py` & `tooldelta-0.7.1/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/tooldelta/urlmethod.py` & `tooldelta-0.7.1/tooldelta/urlmethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,28 +150,26 @@
         for chunk in response.iter_content(chunk_size=8192):
             dwnf.write(chunk)
             downloaded_bytes += len(chunk)
         return downloaded_bytes
 
 
 def download_file_singlethreaded(
-    url: str, save_dir: str, ignore_warnings: bool = False
+    url: str, save_dir: str
 ) -> None:
     """下载单个文件
 
     Args:
         url (str): 文件的URL地址
         save_dir (str): 文件保存的目录
         ignore_warnings (bool, optional): 是否忽略警告
     """
     with requests.get(url, stream=True, timeout=10) as res:
         res.raise_for_status()
         filesize = get_file_size(url)
-        if filesize is not None and filesize < 256 and not ignore_warnings:
-            Print.print_war(f"下载 {url} 的文件警告: 文件大小异常，不到 0.25KB")
         chunk_size = 8192
         useSpeed: float = 0
         # nowsize: 当前已下载的字节数
         nowsize: int = 0
         lastime: float = 1
         with open(save_dir + ".tmp", "wb") as dwnf:
             for chk in res.iter_content(chunk_size):
```

### Comparing `tooldelta-0.7.0/tooldelta/utils.py` & `tooldelta-0.7.1/tooldelta/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.0/PKG-INFO` & `tooldelta-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.7.0
+Version: 0.7.1
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.7.0 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.7.1 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: fcwslib (>=3.0.0,<4.0.0) Requires-Dist: flask
```

