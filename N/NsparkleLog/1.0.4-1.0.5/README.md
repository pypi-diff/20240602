# Comparing `tmp/NsparkleLog-1.0.4.tar.gz` & `tmp/NsparkleLog-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NsparkleLog-1.0.4.tar", last modified: Sat Jun  1 10:53:03 2024, max compression
+gzip compressed data, was "NsparkleLog-1.0.5.tar", last modified: Sun Jun  2 05:02:40 2024, max compression
```

## Comparing `NsparkleLog-1.0.4.tar` & `NsparkleLog-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.501192 NsparkleLog-1.0.4/
--rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.4/LICENSE
-drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.385599 NsparkleLog-1.0.4/NsparkleLog/
--rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.4/NsparkleLog/Interfaces.py
--rw-rw-rw-   0        0        0      265 2024-06-01 10:52:21.000000 NsparkleLog-1.0.4/NsparkleLog/__init__.py
--rw-rw-rw-   0        0        0      127 2024-05-31 09:30:54.000000 NsparkleLog-1.0.4/NsparkleLog/_env.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.416515 NsparkleLog-1.0.4/NsparkleLog/core/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.4/NsparkleLog/core/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.4/NsparkleLog/core/_excformat.py
--rw-rw-rw-   0        0        0     2132 2024-06-01 09:45:33.000000 NsparkleLog-1.0.4/NsparkleLog/core/_formatter.py
--rw-rw-rw-   0        0        0     4207 2024-06-01 09:30:32.000000 NsparkleLog-1.0.4/NsparkleLog/core/_handler.py
--rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.4/NsparkleLog/core/_level.py
--rw-rw-rw-   0        0        0     6536 2024-06-01 09:39:38.000000 NsparkleLog-1.0.4/NsparkleLog/core/_logger.py
--rw-rw-rw-   0        0        0     2706 2024-06-01 09:18:53.000000 NsparkleLog-1.0.4/NsparkleLog/core/_manager.py
--rw-rw-rw-   0        0        0      415 2024-06-01 10:39:33.000000 NsparkleLog-1.0.4/NsparkleLog/dependencies.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.443358 NsparkleLog-1.0.4/NsparkleLog/plugins/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.4/NsparkleLog/plugins/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-31 09:49:56.000000 NsparkleLog-1.0.4/NsparkleLog/plugins/helpers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.475280 NsparkleLog-1.0.4/NsparkleLog/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.4/NsparkleLog/utils/__init__.py
--rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.4/NsparkleLog/utils/_color.py
--rw-rw-rw-   0        0        0      770 2024-06-01 10:40:00.000000 NsparkleLog-1.0.4/NsparkleLog/utils/_get_lock.py
--rw-rw-rw-   0        0        0      177 2024-06-01 08:37:29.000000 NsparkleLog-1.0.4/NsparkleLog/utils/_types.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:53:03.477276 NsparkleLog-1.0.4/NsparkleLog.egg-info/
--rw-rw-rw-   0        0        0     3412 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 10:53:02.000000 NsparkleLog-1.0.4/NsparkleLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3412 2024-06-01 10:53:03.500192 NsparkleLog-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-06-01 10:53:03.501192 NsparkleLog-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:02:40.804131 NsparkleLog-1.0.5/
+-rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.5/LICENSE
+drwxrwxrwx   0        0        0        0 2024-06-02 05:02:40.695309 NsparkleLog-1.0.5/NsparkleLog/
+-rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.5/NsparkleLog/Interfaces.py
+-rw-rw-rw-   0        0        0      265 2024-06-02 05:02:19.000000 NsparkleLog-1.0.5/NsparkleLog/__init__.py
+-rw-rw-rw-   0        0        0      236 2024-06-02 04:57:53.000000 NsparkleLog-1.0.5/NsparkleLog/_env.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:02:40.778417 NsparkleLog-1.0.5/NsparkleLog/core/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.5/NsparkleLog/core/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.5/NsparkleLog/core/_excformat.py
+-rw-rw-rw-   0        0        0     2132 2024-06-01 09:45:33.000000 NsparkleLog-1.0.5/NsparkleLog/core/_formatter.py
+-rw-rw-rw-   0        0        0     4472 2024-06-02 04:59:29.000000 NsparkleLog-1.0.5/NsparkleLog/core/_handler.py
+-rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.5/NsparkleLog/core/_level.py
+-rw-rw-rw-   0        0        0     6753 2024-06-01 11:13:22.000000 NsparkleLog-1.0.5/NsparkleLog/core/_logger.py
+-rw-rw-rw-   0        0        0     2666 2024-06-02 05:00:54.000000 NsparkleLog-1.0.5/NsparkleLog/core/_manager.py
+-rw-rw-rw-   0        0        0      415 2024-06-01 10:39:33.000000 NsparkleLog-1.0.5/NsparkleLog/dependencies.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:02:40.780891 NsparkleLog-1.0.5/NsparkleLog/plugins/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.5/NsparkleLog/plugins/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-31 09:49:56.000000 NsparkleLog-1.0.5/NsparkleLog/plugins/helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:02:40.800931 NsparkleLog-1.0.5/NsparkleLog/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.5/NsparkleLog/utils/__init__.py
+-rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.5/NsparkleLog/utils/_color.py
+-rw-rw-rw-   0        0        0      770 2024-06-01 10:40:00.000000 NsparkleLog-1.0.5/NsparkleLog/utils/_get_lock.py
+-rw-rw-rw-   0        0        0      177 2024-06-01 08:37:29.000000 NsparkleLog-1.0.5/NsparkleLog/utils/_types.py
+drwxrwxrwx   0        0        0        0 2024-06-02 05:02:40.802392 NsparkleLog-1.0.5/NsparkleLog.egg-info/
+-rw-rw-rw-   0        0        0     3412 2024-06-02 05:02:39.000000 NsparkleLog-1.0.5/NsparkleLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2024-06-02 05:02:40.000000 NsparkleLog-1.0.5/NsparkleLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 05:02:39.000000 NsparkleLog-1.0.5/NsparkleLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-02 05:02:39.000000 NsparkleLog-1.0.5/NsparkleLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3412 2024-06-02 05:02:40.803250 NsparkleLog-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-06-02 05:02:40.804131 NsparkleLog-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.5/setup.py
```

### Comparing `NsparkleLog-1.0.4/NsparkleLog/core/_excformat.py` & `NsparkleLog-1.0.5/NsparkleLog/core/_excformat.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.4/NsparkleLog/core/_formatter.py` & `NsparkleLog-1.0.5/NsparkleLog/core/_formatter.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.4/NsparkleLog/core/_handler.py` & `NsparkleLog-1.0.5/NsparkleLog/core/_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from NsparkleLog.dependencies import stdout, stderr , threading , queue ,os
 from NsparkleLog.utils._types import Stream, AnyStr, Level
 from NsparkleLog.core._level import Levels, _levelToName
 from NsparkleLog.core._formatter import Formatter
+from NsparkleLog.utils._get_lock import get_current_lock
+from NsparkleLog._env import allowed_lock_type
 
 def isMainThreadAlive():
     return threading.main_thread().is_alive()
 
 class Writer:
     """
     日志写入器
@@ -36,18 +38,14 @@
         """ 设置等级 """
         self.level = level
 
     def setFormatter(self, formatter: Formatter) -> None:
         """ 设置格式 """
         self.formatter = formatter
 
-    def close(self) -> None:
-        """ 关闭方法 """
-        pass
-
     def handle(
         self,
         name: str,
         threadName: str,
         filename: str,
         lineno: int,
         funcName: str,
@@ -70,56 +68,57 @@
 class StreamHandler(Handler, Writer):
     def __init__(self, error: bool = False) -> None:
         super().__init__()
         
     def handle(self, name: str, threadName: str,filename: str, lineno: int, funcName: str, moduleName: str,ProcessId: int, ProcessName: str, message: AnyStr, level: Level, color: str) -> None:
         string =  super().handle(name, threadName,filename, lineno, funcName, moduleName,ProcessId, ProcessName, message, level, color)
         if level >= self.level:
+           if level >= Levels.ERROR:
+               self.write(string, error=True)
            self.write(string, error=False)
         return
 
-    def close(self) -> None:
-        return super().close()
-
 class FileHandler(Handler):
     """
     日志文件写入器
     """
     def __init__(self, filename: str, mode: str = "a+", encoding: str = "utf-8") -> None:
         super().__init__()
         self.filename = filename
         self.mode = mode
         self.encoding = encoding
-        self.lock = threading.Lock()
+        self.lock = get_current_lock()
         self.queue = queue.Queue()
         self.writeThread = threading.Thread(target=self.writeToFile)
         self.writeThread.start()
 
     def handle(self, name: str, threadName: str, filename: str, lineno: int, funcName: str, moduleName: str,ProcessId: int, ProcessName: str, message: AnyStr, level: Level, color: str) -> None:
         string =  super().handle(name, threadName,filename, lineno, funcName, moduleName,ProcessId, ProcessName, message, level, color)
         if level >= self.level:
            self.queue.put(string)
         return
 
     def writeToFile(self) -> None:
-        with open(self.filename, self.mode, encoding=self.encoding) as f:
-            while True:
-                try:
-                    string = self.queue.get(timeout=1)  # 使用timeout来避免忙等
-                    with self.lock:
-                        f.write(f"{string}\n")
-                        f.flush()
-                    self.queue.task_done()
-                except queue.Empty:
-                    if  not isMainThreadAlive():
-                        break
-                    else:
-                        continue
-                except Exception as e:
-                    stderr.write(f"{e}\n")
+        if isinstance(self.lock, allowed_lock_type):
+            with open(self.filename, self.mode, encoding=self.encoding) as f:
+                while True:
+                    try:
+                        string = self.queue.get(timeout=1)  # 使用timeout来避免忙等
+                        with self.lock: #type: ignore
+                            f.write(f"{string}\n")
+                            f.flush()
+                        self.queue.task_done()
+                    except queue.Empty:
+                        if  not isMainThreadAlive():
+                            break
+                        else:
+                            continue
+                    except Exception as e:
+                        stderr.write(f"{e}\n")
+        raise RuntimeError("lock is not a threading.Lock or mulitprocessing.Lock")
         
 
 class RotatingFileHandler(Handler):
     """
     日志文件按大小轮换写入器
     """
     pass
```

### Comparing `NsparkleLog-1.0.4/NsparkleLog/core/_logger.py` & `NsparkleLog-1.0.5/NsparkleLog/core/_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,21 @@
     def info(self, message: AnyStr, **kwargs) -> None:
         """ 记录一个级别为infomation的日志 """
         self._log(Levels.INFO, message, self.colorLevel[Levels.INFO], **kwargs) # type: ignore
 
     def warning(self, message: AnyStr, **kwargs) -> None:
         """ 记录一个级别为warning的日志 """
         self._log(Levels.WARNING, message, self.colorLevel[Levels.WARN], **kwargs) # type: ignore
+    
+    def warn(self,message: AnyStr, **kwargs) -> None:
+        return self.warning(message, **kwargs)
 
     def error(self, message: AnyStr, **kwargs) -> None:
         """ 记录一个级别为error的日志 """
         self._log(Levels.ERROR, message, self.colorLevel[Levels.ERROR], **kwargs) # type: ignore
 
+    def critical(self, message: AnyStr, **kwargs) -> None:
+        return self.fatal(message, **kwargs)
+
     def fatal(self, message: AnyStr, **kwargs) -> None:
         """ 记录一个级别为fatal的日志 """
         self._log(Levels.FATAL, message, self.colorLevel[Levels.FATAL], **kwargs) # type: ignore
```

### Comparing `NsparkleLog-1.0.4/NsparkleLog/core/_manager.py` & `NsparkleLog-1.0.5/NsparkleLog/core/_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from NsparkleLog.core._logger import Logger
 from NsparkleLog.dependencies import threading , Lock , asyncio, multiprocessing
 from NsparkleLog.utils._types import Level
 from NsparkleLog.core._level import Levels
 from NsparkleLog.core._handler import StreamHandler , Formatter
-from NsparkleLog._env import default_format
+from NsparkleLog._env import default_format , allowed_lock_type
 from NsparkleLog.utils._get_lock import get_current_lock
 
 class LogManager:
     loggers: set[Logger] = set()
     lock = get_current_lock()
 
     @classmethod
@@ -19,26 +19,26 @@
         logger.addHandler(console)
         cls.loggers.add(logger)
         return logger
 
     @classmethod
     def GetLogger(cls,
                   name: str,
-                  level: Level = Levels.DEBUG,
+                  level: Level = Levels.ON,
                   colorMode: bool = True,
                   colorLevel: dict[Level, str] = {
                       Levels.TRACE: "bd_grey",
                       Levels.DEBUG: "bd_blue",
                       Levels.INFO: "bd_cyan",
                       Levels.WARNING: "bd_yellow",
                       Levels.ERROR: "bd_red",
                       Levels.FATAL: "bd_background_red",
                   }) -> Logger:  # type: ignore
-        allow_lock = type(threading.Lock()) , type(multiprocessing.Lock)
-        if isinstance(cls.lock, allow_lock):
+        
+        if isinstance(cls.lock, allowed_lock_type):
             with cls.lock: #type: ignore
                 logger = next((logger for logger in cls.loggers if logger.name == name), None)
                 if logger is None:
                     return cls._create_logger(name, level, colorMode, colorLevel)
                 else:
                     return logger
         elif isinstance(cls.lock, asyncio.Lock):
```

### Comparing `NsparkleLog-1.0.4/NsparkleLog/plugins/helpers.py` & `NsparkleLog-1.0.5/NsparkleLog/plugins/helpers.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.4/NsparkleLog/utils/_color.py` & `NsparkleLog-1.0.5/NsparkleLog/utils/_color.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.4/NsparkleLog/utils/_get_lock.py` & `NsparkleLog-1.0.5/NsparkleLog/utils/_get_lock.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.4/NsparkleLog.egg-info/PKG-INFO` & `NsparkleLog-1.0.5/NsparkleLog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.4
+Version: 1.0.5
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NsparkleLog-1.0.4/NsparkleLog.egg-info/SOURCES.txt` & `NsparkleLog-1.0.5/NsparkleLog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.4/PKG-INFO` & `NsparkleLog-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.4
+Version: 1.0.5
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NsparkleLog-1.0.4/setup.py` & `NsparkleLog-1.0.5/setup.py`

 * *Files identical despite different names*

