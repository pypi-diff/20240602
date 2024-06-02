# Comparing `tmp/NsparkleLog-1.0.3.tar.gz` & `tmp/NsparkleLog-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NsparkleLog-1.0.3.tar", last modified: Fri May 31 13:43:55 2024, max compression
+gzip compressed data, was "NsparkleLog-1.0.4.tar", last modified: Sat Jun  1 10:53:03 2024, max compression
```

## Comparing `NsparkleLog-1.0.3.tar` & `NsparkleLog-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.158206 NsparkleLog-1.0.3/
--rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.105716 NsparkleLog-1.0.3/NsparkleLog/
--rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.3/NsparkleLog/Interfaces.py
--rw-rw-rw-   0        0        0      265 2024-05-31 13:33:31.000000 NsparkleLog-1.0.3/NsparkleLog/__init__.py
--rw-rw-rw-   0        0        0      127 2024-05-31 09:30:54.000000 NsparkleLog-1.0.3/NsparkleLog/_env.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.147899 NsparkleLog-1.0.3/NsparkleLog/core/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.3/NsparkleLog/core/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.3/NsparkleLog/core/_excformat.py
--rw-rw-rw-   0        0        0     1467 2024-05-30 12:50:00.000000 NsparkleLog-1.0.3/NsparkleLog/core/_formatter.py
--rw-rw-rw-   0        0        0     4020 2024-05-31 13:36:13.000000 NsparkleLog-1.0.3/NsparkleLog/core/_handler.py
--rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.3/NsparkleLog/core/_level.py
--rw-rw-rw-   0        0        0     5799 2024-05-30 13:32:46.000000 NsparkleLog-1.0.3/NsparkleLog/core/_logger.py
--rw-rw-rw-   0        0        0     1337 2024-05-30 12:50:46.000000 NsparkleLog-1.0.3/NsparkleLog/core/_manager.py
--rw-rw-rw-   0        0        0      329 2024-05-31 09:32:27.000000 NsparkleLog-1.0.3/NsparkleLog/dependencies.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.149893 NsparkleLog-1.0.3/NsparkleLog/plugins/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.3/NsparkleLog/plugins/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-31 09:49:56.000000 NsparkleLog-1.0.3/NsparkleLog/plugins/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.153748 NsparkleLog-1.0.3/NsparkleLog/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.3/NsparkleLog/utils/__init__.py
--rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.3/NsparkleLog/utils/_color.py
--rw-rw-rw-   0        0        0      177 2024-05-31 09:42:52.000000 NsparkleLog-1.0.3/NsparkleLog/utils/_types.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.154749 NsparkleLog-1.0.3/NsparkleLog.egg-info/
--rw-rw-rw-   0        0        0     3676 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3676 2024-05-31 13:43:55.156211 NsparkleLog-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-31 13:43:55.158206 NsparkleLog-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.501192 NsparkleLog-1.0.4/
+-rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.4/LICENSE
+drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.385599 NsparkleLog-1.0.4/NsparkleLog/
+-rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.4/NsparkleLog/Interfaces.py
+-rw-rw-rw-   0        0        0      265 2024-06-01 10:52:21.000000 NsparkleLog-1.0.4/NsparkleLog/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-05-31 09:30:54.000000 NsparkleLog-1.0.4/NsparkleLog/_env.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.416515 NsparkleLog-1.0.4/NsparkleLog/core/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.4/NsparkleLog/core/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.4/NsparkleLog/core/_excformat.py
+-rw-rw-rw-   0        0        0     2132 2024-06-01 09:45:33.000000 NsparkleLog-1.0.4/NsparkleLog/core/_formatter.py
+-rw-rw-rw-   0        0        0     4207 2024-06-01 09:30:32.000000 NsparkleLog-1.0.4/NsparkleLog/core/_handler.py
+-rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.4/NsparkleLog/core/_level.py
+-rw-rw-rw-   0        0        0     6536 2024-06-01 09:39:38.000000 NsparkleLog-1.0.4/NsparkleLog/core/_logger.py
+-rw-rw-rw-   0        0        0     2706 2024-06-01 09:18:53.000000 NsparkleLog-1.0.4/NsparkleLog/core/_manager.py
+-rw-rw-rw-   0        0        0      415 2024-06-01 10:39:33.000000 NsparkleLog-1.0.4/NsparkleLog/dependencies.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.443358 NsparkleLog-1.0.4/NsparkleLog/plugins/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.4/NsparkleLog/plugins/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-31 09:49:56.000000 NsparkleLog-1.0.4/NsparkleLog/plugins/helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.475280 NsparkleLog-1.0.4/NsparkleLog/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.4/NsparkleLog/utils/__init__.py
+-rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.4/NsparkleLog/utils/_color.py
+-rw-rw-rw-   0        0        0      770 2024-06-01 10:40:00.000000 NsparkleLog-1.0.4/NsparkleLog/utils/_get_lock.py
+-rw-rw-rw-   0        0        0      177 2024-06-01 08:37:29.000000 NsparkleLog-1.0.4/NsparkleLog/utils/_types.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.477276 NsparkleLog-1.0.4/NsparkleLog.egg-info/
+-rw-rw-rw-   0        0        0     3412 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3412 2024-06-01 10:53:03.500192 NsparkleLog-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-06-01 10:53:03.501192 NsparkleLog-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.4/setup.py
```

### Comparing `NsparkleLog-1.0.3/NsparkleLog/core/_excformat.py` & `NsparkleLog-1.0.4/NsparkleLog/core/_excformat.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.3/NsparkleLog/core/_handler.py` & `NsparkleLog-1.0.4/NsparkleLog/core/_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,33 +48,35 @@
         self,
         name: str,
         threadName: str,
         filename: str,
         lineno: int,
         funcName: str,
         moduleName: str,
+        ProcessId: int,
+        ProcessName: str,
         message: AnyStr,
         level: Level,
         color: str,
     ) -> None:
         """ 主要的处理程序 """
         
         if self.formatter is None:
             raise Exception("Formatter not set")
 
-        formatted_msg = self.formatter.format(name, threadName,filename,lineno,funcName,moduleName, message, level, color)
+        formatted_msg = self.formatter.format(name, threadName,filename,lineno,funcName,moduleName,ProcessId, ProcessName, message, level, color)
         
         return formatted_msg #type: ignore
 
 class StreamHandler(Handler, Writer):
     def __init__(self, error: bool = False) -> None:
         super().__init__()
         
-    def handle(self, name: str, threadName: str,filename: str, lineno: int, funcName: str, moduleName: str, message: AnyStr, level: Level, color: str) -> None:
-        string =  super().handle(name, threadName,filename, lineno, funcName, moduleName, message, level, color)
+    def handle(self, name: str, threadName: str,filename: str, lineno: int, funcName: str, moduleName: str,ProcessId: int, ProcessName: str, message: AnyStr, level: Level, color: str) -> None:
+        string =  super().handle(name, threadName,filename, lineno, funcName, moduleName,ProcessId, ProcessName, message, level, color)
         if level >= self.level:
            self.write(string, error=False)
         return
 
     def close(self) -> None:
         return super().close()
 
@@ -88,16 +90,16 @@
         self.mode = mode
         self.encoding = encoding
         self.lock = threading.Lock()
         self.queue = queue.Queue()
         self.writeThread = threading.Thread(target=self.writeToFile)
         self.writeThread.start()
 
-    def handle(self, name: str, threadName: str, filename: str, lineno: int, funcName: str, moduleName: str, message: AnyStr, level: Level, color: str) -> None:
-        string = super().handle(name, threadName, filename, lineno, funcName, moduleName, message, level, color)
+    def handle(self, name: str, threadName: str, filename: str, lineno: int, funcName: str, moduleName: str,ProcessId: int, ProcessName: str, message: AnyStr, level: Level, color: str) -> None:
+        string =  super().handle(name, threadName,filename, lineno, funcName, moduleName,ProcessId, ProcessName, message, level, color)
         if level >= self.level:
            self.queue.put(string)
         return
 
     def writeToFile(self) -> None:
         with open(self.filename, self.mode, encoding=self.encoding) as f:
             while True:
```

### Comparing `NsparkleLog-1.0.3/NsparkleLog/core/_logger.py` & `NsparkleLog-1.0.4/NsparkleLog/core/_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from NsparkleLog.utils._types import Level , AnyStr
 from NsparkleLog.core._level import Levels, _nameToLevel , _levelToName
 from NsparkleLog.core._handler import Handler
-from NsparkleLog.dependencies import threading , stderr , inspect , os , traceback
+from NsparkleLog.dependencies import threading , stderr , inspect , os , traceback , multiprocessing
 from NsparkleLog.utils._color import _Color
+from NsparkleLog.core._formatter import Formatter
 from NsparkleLog.plugins.helpers import Deprecated
+from NsparkleLog.core._handler import StreamHandler
 
 class Logger:
     def __init__(self,
     name: str = "main",
     level = Levels.ON,
     colorLevel: dict[Level, str] = {
         Levels.TRACE: "bd_grey",
@@ -28,31 +30,45 @@
     def addHandler(self, handler: Handler) -> None:
         """
         添加日志处理器
         """
         with self.lock:
            self.handlers.add(handler)
 
+    def __getLogMsg(self) -> tuple[str,str,int,str,str,int,str]:
+        threadName = threading.current_thread().name
+        frame = inspect.currentframe().f_back.f_back.f_back  # type: ignore  
+        filename = os.path.relpath(frame.f_code.co_filename, start=os.getcwd()) # type: ignore
+        lineno = frame.f_lineno # type: ignore
+        moduleName = inspect.getmodule(frame).__name__ # type: ignore
+        funcName = frame.f_code.co_name # type: ignore
+        ProcessID = os.getpid()
+        ProcessName = multiprocessing.current_process().name
+        return threadName , filename , lineno , funcName , moduleName , ProcessID , ProcessName
+
     def _log(self, level: Level, message: AnyStr, color: str, **kwargs) -> None:
         if not self.handlers:
             raise Exception("No handlers found")
         try:
             if level >= self.level:
-                threadName = threading.current_thread().name
-                frame = inspect.currentframe().f_back.f_back  # type: ignore  
-                filename = os.path.relpath(frame.f_code.co_filename, start=os.getcwd()) # type: ignore
-                lineno = frame.f_lineno # type: ignore
-                moduleName = inspect.getmodule(frame).__name__ # type: ignore
-                funcName = frame.f_code.co_name # type: ignore
+                threadName , filename , lineno , funcName , moduleName , ProcessID , ProcessName = self.__getLogMsg()
                 for handler in self.handlers:
-                    handler.handle(self.name, threadName, filename, lineno, funcName, moduleName, message, level, color, **kwargs)
+                    handler.handle(self.name, threadName, filename, lineno, funcName, moduleName,ProcessID,ProcessName, message, level, color, **kwargs)
         except Exception as e:
             err_msg = traceback.format_exc()
             stderr.write(f"{err_msg}\n")
 
+    def setFormatter(self, formatter: Formatter) -> None:
+        """
+        设置日志格式
+        """
+        for handler in self.handlers:
+            if isinstance(handler, StreamHandler):
+                handler.setFormatter(formatter)
+
     def setLevel(self,level:Level):
         """
         设置日志等级
         """
         if level in _levelToName:
             with self.lock:
                 if _levelToName[level] == "OFF":
```

### Comparing `NsparkleLog-1.0.3/NsparkleLog/plugins/helpers.py` & `NsparkleLog-1.0.4/NsparkleLog/plugins/helpers.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.3/NsparkleLog/utils/_color.py` & `NsparkleLog-1.0.4/NsparkleLog/utils/_color.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.3/NsparkleLog.egg-info/PKG-INFO` & `NsparkleLog-1.0.4/NsparkleLog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.3
+Version: 1.0.4
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,19 +15,14 @@
 
 ![Sparkle!](https://github.com/KOKOMI12345/NewSparkleLogging/blob/main/picture_pixiv_116702098_0.jpg)
 
 ## 描述
 
 原来SparkleLogging日志库的新版,新的SparkleLogging日志库是从底层开始写起来的,并没有基于logging标准库往上搭建,所以功能暂时不完善。
 
-# CAUTION
-
-注意，虽然我在需要共享资源的地方使用了 "with lock" 来确保线程安全，但这个日志库是我从底层开始编写的，
-我无法绝对保证在多线程、多进程或异步环境中的绝对安全性。如果在特定环境下遇到问题，请务必审慎考虑并进行适当的调整。
-
 # Get started
 
 一般来说，你只需要简单的
 
 ```python
 from NsparkleLog import logger
 
@@ -37,14 +32,17 @@
 logger.debug("test")
 logger.info("test")
 logger.warning("test")
 logger.error("test")
 logger.fatal("test")
 ```
 
+[2024/6/1 18:51]
+### 完善多线程，多进程，异步的安全
+
 [2024/5/30 21:33]
 # 日志库不用再需要显示调用close方法来释放资源,主线程退出后会自动释放资源
 
 # 更新了setLevel接口用于设置日志级别过滤
 
 - 同时修复了一个addNewLevel可能会覆盖自己日志库定义等级的bug
```

### Comparing `NsparkleLog-1.0.3/NsparkleLog.egg-info/SOURCES.txt` & `NsparkleLog-1.0.4/NsparkleLog.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 NsparkleLog/core/_level.py
 NsparkleLog/core/_logger.py
 NsparkleLog/core/_manager.py
 NsparkleLog/plugins/__init__.py
 NsparkleLog/plugins/helpers.py
 NsparkleLog/utils/__init__.py
 NsparkleLog/utils/_color.py
+NsparkleLog/utils/_get_lock.py
 NsparkleLog/utils/_types.py
```

### Comparing `NsparkleLog-1.0.3/PKG-INFO` & `NsparkleLog-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.3
+Version: 1.0.4
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,19 +15,14 @@
 
 ![Sparkle!](https://github.com/KOKOMI12345/NewSparkleLogging/blob/main/picture_pixiv_116702098_0.jpg)
 
 ## 描述
 
 原来SparkleLogging日志库的新版,新的SparkleLogging日志库是从底层开始写起来的,并没有基于logging标准库往上搭建,所以功能暂时不完善。
 
-# CAUTION
-
-注意，虽然我在需要共享资源的地方使用了 "with lock" 来确保线程安全，但这个日志库是我从底层开始编写的，
-我无法绝对保证在多线程、多进程或异步环境中的绝对安全性。如果在特定环境下遇到问题，请务必审慎考虑并进行适当的调整。
-
 # Get started
 
 一般来说，你只需要简单的
 
 ```python
 from NsparkleLog import logger
 
@@ -37,14 +32,17 @@
 logger.debug("test")
 logger.info("test")
 logger.warning("test")
 logger.error("test")
 logger.fatal("test")
 ```
 
+[2024/6/1 18:51]
+### 完善多线程，多进程，异步的安全
+
 [2024/5/30 21:33]
 # 日志库不用再需要显示调用close方法来释放资源,主线程退出后会自动释放资源
 
 # 更新了setLevel接口用于设置日志级别过滤
 
 - 同时修复了一个addNewLevel可能会覆盖自己日志库定义等级的bug
```

### Comparing `NsparkleLog-1.0.3/setup.py` & `NsparkleLog-1.0.4/setup.py`

 * *Files identical despite different names*

