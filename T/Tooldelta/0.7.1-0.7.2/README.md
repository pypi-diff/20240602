# Comparing `tmp/tooldelta-0.7.1.tar.gz` & `tmp/tooldelta-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.7.1.tar", max compression
+gzip compressed data, was "tooldelta-0.7.2.tar", max compression
```

## Comparing `tooldelta-0.7.1.tar` & `tooldelta-0.7.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1497 2024-06-01 22:12:10.500592 tooldelta-0.7.1/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-06-01 22:12:10.500592 tooldelta-0.7.1/README.md
--rw-r--r--   0        0        0      908 2024-06-01 22:12:19.684632 tooldelta-0.7.1/pyproject.toml
--rwxr-xr-x   0        0        0      658 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/auths.py
--rwxr-xr-x   0        0        0    12563 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10441 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/color_print.py
--rw-r--r--   0        0        0     1885 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/constants.py
--rwxr-xr-x   0        0        0    35071 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/frame.py
--rwxr-xr-x   0        0        0    13369 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    23814 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1832 2024-06-01 22:12:10.500592 tooldelta-0.7.1/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/logger.py
--rw-r--r--   0        0        0    29752 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1295 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/packets.py
--rwxr-xr-x   0        0        0    16677 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3504 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     9072 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0    10499 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     6318 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/movent.py
--rw-r--r--   0        0        0     7032 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_load/utils.py
--rwxr-xr-x   0        0        0    17350 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    17116 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1932 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/starter.py
--rwxr-xr-x   0        0        0     1110 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9870 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/urlmethod.py
--rw-r--r--   0        0        0    20711 2024-06-01 22:12:10.504592 tooldelta-0.7.1/tooldelta/utils.py
--rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 tooldelta-0.7.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-06-02 06:13:34.141001 tooldelta-0.7.2/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-06-02 06:13:34.141001 tooldelta-0.7.2/README.md
+-rw-r--r--   0        0        0      908 2024-06-02 06:13:49.681093 tooldelta-0.7.2/pyproject.toml
+-rwxr-xr-x   0        0        0      658 2024-06-02 06:13:34.141001 tooldelta-0.7.2/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-06-02 06:13:34.141001 tooldelta-0.7.2/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    12592 2024-06-02 06:13:34.141001 tooldelta-0.7.2/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10441 2024-06-02 06:13:34.141001 tooldelta-0.7.2/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1885 2024-06-02 06:13:34.141001 tooldelta-0.7.2/tooldelta/constants.py
+-rwxr-xr-x   0        0        0    35205 2024-06-02 06:13:34.141001 tooldelta-0.7.2/tooldelta/frame.py
+-rwxr-xr-x   0        0        0    13378 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    23814 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1832 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/logger.py
+-rw-r--r--   0        0        0    29752 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1295 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    16677 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3504 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     9072 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0    10499 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     6318 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_load/injected_plugin/movent.py
+-rw-r--r--   0        0        0     7032 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_load/utils.py
+-rwxr-xr-x   0        0        0    17350 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    17116 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1932 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/starter.py
+-rwxr-xr-x   0        0        0     1110 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9870 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0    20659 2024-06-02 06:13:34.145001 tooldelta-0.7.2/tooldelta/utils.py
+-rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 tooldelta-0.7.2/PKG-INFO
```

### Comparing `tooldelta-0.7.1/LICENSE` & `tooldelta-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/README.md` & `tooldelta-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/pyproject.toml` & `tooldelta-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.7.1" # This field is automatically set to the value in the version file
+version = "0.7.2" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.7.1/tooldelta/__init__.py` & `tooldelta-0.7.2/tooldelta/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/auths.py` & `tooldelta-0.7.2/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/cfg.py` & `tooldelta-0.7.2/tooldelta/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 import ujson
 
 NoneType = type(None)
 
 PLUGINCFG_DEFAULT = {"配置版本": "0.0.1", "配置项": None}
 PLUGINCFG_STANDARD_TYPE = {"配置版本": str, "配置项": [type(None), dict]}
 
-def cfg_isinstance_single(obj, typ: type) -> bool:
+
+def cfg_isinstance_single(obj: Any, typ: type) -> bool:
     if not isinstance(typ, type):
         raise TypeError(f"cfg_isinstance arg 1 must be a type, not {typ}")
     return {
         Cfg.PInt: lambda: isinstance(obj, int) and obj > 0,
         Cfg.NNInt: lambda: isinstance(obj, int) and obj >= 0,
         Cfg.PFloat: lambda: isinstance(obj, float) and obj > 0,
         Cfg.NNFloat: lambda: (isinstance(obj, float) or obj == 0) and obj >= 0,
         Cfg.PNumber: lambda: isinstance(obj, (int, float)) and obj > 0,
         Cfg.NNNumber: lambda: isinstance(obj, (int, float)) and obj >= 0,
-        int: lambda: obj not in (True, False) and isinstance(obj, int)
+        int: lambda: type(obj) == int
     }.get(typ, lambda: isinstance(obj, typ))()
 
+
 def cfg_isinstance(obj: Any, typ: type | tuple[type]):
     """
     专用于Cfg的类型检测
 
     Args:
         obj (Any): 待检测对象
         typ (Any | tuple[Any]): 类型或类型元组
@@ -68,41 +70,43 @@
         int: "整数",
         dict: "json对象",
         list: "列表",
         bool: "true/false",
         NoneType: "null",
     }.get(typ, typ.__name__)
 
+
 class Cfg:
     """配置文件模块"""
     class ConfigError(Exception):
         "配置文件错误"
 
         def __init__(self, errStr: str, errPos: list | None = None):
             if errPos is None:
                 errPos = []
             self.errPos = errPos
             self.args = (errStr,)
 
     class UnneccessaryKV:
         "配置文件的不必要的键"
 
-        def __init__(self, key: str, val_type):
+        def __init__(self, key: str, val_type: Any):
             self.key = key
             self.type = val_type
 
     class JsonList:
         "配置文件的列表类型"
 
-        def __init__(self, patt: type | dict | tuple[type | dict, ...], len_limit = -1):
+        def __init__(self, patt: type | dict | tuple[type | dict, ...], len_limit=-1):
             self.patt = patt
             self.len_limit = len_limit
 
     class AnyKeyValue:
         "配置文件的任意键名键值对类型"
+
         def __init__(self, val_type: type | tuple[type]):
             self.type = val_type
 
     class ConfigKeyError(ConfigError):
         "配置json的键错误"
 
     class ConfigValueError(ConfigError):
@@ -240,32 +244,34 @@
                 try:
                     self.check_auto(single_type, val, fromkey)
                     break
                 except Exception as err:
                     errs.append(err)
             else:
                 reason = "\n".join(str(err) for err in errs)
-                raise self.ConfigValueError(f'JSON键 对应的键"{fromkey}" 类型不正确, 以下为可能的原因: \n{reason}')
+                raise self.ConfigValueError(
+                    f'JSON键 对应的键"{fromkey}" 类型不正确, 以下为可能的原因: \n{reason}')
         elif isinstance(standard, (dict, Cfg.AnyKeyValue, Cfg.UnneccessaryKV)):
             self.check_dict(standard, val, fromkey)
         else:
             raise ValueError(
                 f'JSON键 "{fromkey}" 自动检测的标准类型传入异常: {standard.__class__.__name__}'
             )
 
-    def check_dict(self, pattern: dict | AnyKeyValue | UnneccessaryKV, jsondict: Any, from_key = "?"):
+    def check_dict(self, pattern: dict | AnyKeyValue | UnneccessaryKV, jsondict: Any, from_key="?"):
         """
         按照给定的标准配置样式比对传入的配置文件jsondict, 对不上则引发相应异常
 
         参数:
             pattern: 标准样式dict
             jsondict: 待检测的配置文件dict
         """
         if not isinstance(jsondict, dict):
-            raise ValueError(f'json键"{from_key}" 需要json对象, 而不是 {_CfgShowType(jsondict)}')
+            raise ValueError(
+                f'json键"{from_key}" 需要json对象, 而不是 {_CfgShowType(jsondict)}')
         if isinstance(pattern, Cfg.AnyKeyValue):
             for key, val in jsondict.items():
                 self.check_auto(pattern.type, val, key)
         elif isinstance(pattern, Cfg.UnneccessaryKV):
             val_get = jsondict.get(pattern.key, Cfg.FindNone)
             if val_get != Cfg.FindNone:
                 self.check_auto(pattern.type, val_get, pattern.key)
@@ -333,18 +339,20 @@
             if len(setting_types) == 1:
                 return Cfg.JsonList(setting_types[0])
             return Cfg.JsonList(tuple(setting_types))
         raise ValueError("auto_to_std() 仅接受 dict 与 list 参数")
 
     checkDict = check_dict
 
+
 Config = Cfg()
 
 if __name__ == "__main__":
     # Test Part
     try:
         test_cfg = {"key1": {"b": 2}, "key2": [{"key3": "6"}, 7]}
-        std = {"key1": Cfg.UnneccessaryKV("b", int), "key2": Cfg.JsonList(({"key3": str}, int))}
+        std = {"key1": Cfg.UnneccessaryKV(
+            "b", int), "key2": Cfg.JsonList(({"key3": str}, int))}
         Config.check_auto(std, test_cfg)
     except Cfg.ConfigError:
         import traceback
         print(traceback.format_exc())
```

### Comparing `tooldelta-0.7.1/tooldelta/color_print.py` & `tooldelta-0.7.2/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/constants.py` & `tooldelta-0.7.2/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/frame.py` & `tooldelta-0.7.2/tooldelta/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,16 @@
         except Config.ConfigError as err:
             # 配置文件有误
             r = self.upgrade_cfg()
             if r:
                 Print.print_war("配置文件未升级, 已自动升级, 请重启 ToolDelta")
             else:
                 Print.print_err(f"ToolDelta基本配置有误, 需要更正: {err}")
+                import traceback
+                traceback.print_exc()
             raise SystemExit from err
         if self.serverNumber == 0:
             while 1:
                 try:
                     self.serverNumber = int(input(
                         Print.fmt_info("请输入租赁服号: ", "§b 输入 ")
                     ))
@@ -414,18 +416,20 @@
                 if (result.OutputMessages[0].Message == "commands.generic.syntax") | (
                     result.OutputMessages[0].Message == "commands.generic.unknown"
                 ):
                     Print.print_err(f'未知的MC指令， 可能是指令格式有误： "{cmd}"')
                 else:
                     mjon = self.link_game_ctrl.Game_Data_Handle.Handle_Text_Class1(result.as_dict["OutputMessages"])
                     if not result.SuccessCount:
-                        print_str = "指令执行失败: " + " ".join(mjon); Print.print_war(print_str)
+                        print_str = "指令执行失败: " + " ".join(mjon)
+                        Print.print_war(print_str)
                         Print.print_war(result.as_dict["OutputMessages"])
                     else:
-                        print_str = "指令执行成功: " + " ".join(mjon); Print.print_suc(print_str)
+                        print_str = "指令执行成功: " + " ".join(mjon)
+                        Print.print_suc(print_str)
                         Print.print_suc(result.as_dict["OutputMessages"])
 
             except IndexError as exec_err:
                 if isinstance(result, type(None)):
                     raise ValueError("指令执行失败") from exec_err
                 if result.SuccessCount:
                     Print.print_suc(
@@ -595,29 +599,30 @@
             self.requireUUIDPacket = False
         else:
             self.requireUUIDPacket = True
 
     def set_listen_packets(self) -> None:
         """
         向启动器初始化监听的游戏数据包
-
-        不应该再次调用此方法
+        仅限内部调用
         """
         for pktID in self.require_listen_packets:
             self.launcher.add_listen_packets(pktID)
 
     def add_listen_pkt(self, pkt: int) -> None:
-        """添加监听的数据包
+        """
+        添加监听的数据包
+        仅限内部调用
 
         Args:
             pkt (int): 数据包ID
         """
         self.require_listen_packets.add(pkt)
 
-    @Utils.run_as_new_thread
+    @Utils.thread_func
     def packet_handler(self, pkt_type: int, pkt: dict) -> None:
         """数据包处理分发任务函数
 
         Args:
             pkt_type (int): 数据包类型
             pkt (dict): 数据包内容
         """
```

### Comparing `tooldelta-0.7.1/tooldelta/game_texts.py` & `tooldelta-0.7.2/tooldelta/game_texts.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         Returns:
             Dict[str, str]: 数据
         """
         try:
             all_values: Dict[str, str] = {}
             for file_path in glob(
-                os.path.join(self.base_path, "src", "**", "*.py"), recursive=True
+                pathname=os.path.join(self.base_path, "src", "**", "*.py"), recursive=True
             ):
                 module_name: str = os.path.basename(
                     file_path).replace(".py", "")
                 spec = (
                     util.spec_from_file_location(
                         module_name, file_path)
                 )
```

### Comparing `tooldelta-0.7.1/tooldelta/launch_cli.py` & `tooldelta-0.7.2/tooldelta/launch_cli.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/launch_options.py` & `tooldelta-0.7.2/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/logger.py` & `tooldelta-0.7.2/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/neo_conn.py` & `tooldelta-0.7.2/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/packets.py` & `tooldelta-0.7.2/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.7.2/tooldelta/plugin_load/PluginGroup.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_load/__init__.py` & `tooldelta-0.7.2/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.7.2/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.7.2/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.7.2/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_load/utils.py` & `tooldelta-0.7.2/tooldelta/plugin_load/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_manager.py` & `tooldelta-0.7.2/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/plugin_market.py` & `tooldelta-0.7.2/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/starter.py` & `tooldelta-0.7.2/tooldelta/starter.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/sys_args.py` & `tooldelta-0.7.2/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/urlmethod.py` & `tooldelta-0.7.2/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.7.1/tooldelta/utils.py` & `tooldelta-0.7.2/tooldelta/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             self.stopping = True
             self._thread_id = self.ident
             thread_id = self.get_id()
             res = ctypes.pythonapi.PyThreadState_SetAsyncExc(
                 thread_id, ctypes.py_object(SystemExit))
             if res > 1:
                 ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, 0)
-                Print.print_err("§c终止线程失败")
+                Print.print_err(f"§c终止线程 {self.name} 失败")
 
     createThread = ClassicThread
 
     class TMPJson:
         """提供了加载、卸载、读取和写入JSON文件到缓存区的方法的类."""
         @staticmethod
         def loadPathJson(path: str, needFileExists: bool = True) -> None:
@@ -393,17 +393,14 @@
                     func_or_name,
                     usage="简易线程方法:" + func_or_name.__name__,
                     args=args,
                     **kwargs
                 )
         return thread_fun
 
-    run_as_new_thread = thread_func
-    new_thread = thread_func
-
     @staticmethod
     def try_int(arg: Any) -> Optional[int]:
         """尝试将提供的参数化为int类型并返回, 否则返回None"""
         try:
             return int(arg)
         except Exception:
             return None
```

### Comparing `tooldelta-0.7.1/PKG-INFO` & `tooldelta-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.7.1
+Version: 0.7.2
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
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.7.1 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.7.2 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: fcwslib (>=3.0.0,<4.0.0) Requires-Dist: flask
```

