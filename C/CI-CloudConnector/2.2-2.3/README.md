# Comparing `tmp/ci_cloudconnector-2.2.tar.gz` & `tmp/ci_cloudconnector-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-2.2.tar", last modified: Sun Jun  2 06:26:51 2024, max compression
+gzip compressed data, was "ci_cloudconnector-2.3.tar", last modified: Sun Jun  2 07:02:58 2024, max compression
```

## Comparing `ci_cloudconnector-2.2.tar` & `ci_cloudconnector-2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 06:26:51.361250 ci_cloudconnector-2.2/
-drwxrwxrwx   0        0        0        0 2024-06-02 06:26:51.355439 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-06-02 06:26:51.358201 ci_cloudconnector-2.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-2.2/README.txt
--rw-rw-rw-   0        0        0    38161 2024-06-02 06:26:03.000000 ci_cloudconnector-2.2/logic.py
--rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-2.2/main.py
--rw-rw-rw-   0        0        0     3384 2024-06-02 06:24:12.000000 ci_cloudconnector-2.2/myservice.py
--rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.2/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-06-02 06:26:51.362209 ci_cloudconnector-2.2/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-06-02 06:20:15.000000 ci_cloudconnector-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:02:58.981746 ci_cloudconnector-2.3/
+drwxrwxrwx   0        0        0        0 2024-06-02 07:02:58.981746 ci_cloudconnector-2.3/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-06-02 07:02:58.000000 ci_cloudconnector-2.3/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-06-02 07:02:58.000000 ci_cloudconnector-2.3/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:02:58.000000 ci_cloudconnector-2.3/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-02 07:02:58.000000 ci_cloudconnector-2.3/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-06-02 07:02:58.981746 ci_cloudconnector-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-2.3/README.txt
+-rw-rw-rw-   0        0        0    36755 2024-06-02 06:56:25.000000 ci_cloudconnector-2.3/logic.py
+-rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-2.3/main.py
+-rw-rw-rw-   0        0        0     4157 2024-06-02 06:49:17.000000 ci_cloudconnector-2.3/myservice.py
+-rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.3/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 07:02:58.981746 ci_cloudconnector-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-06-02 06:56:25.000000 ci_cloudconnector-2.3/setup.py
```

### Comparing `ci_cloudconnector-2.2/logic.py` & `ci_cloudconnector-2.3/logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from logging.handlers import RotatingFileHandler
 import os
 import configparser
 import requests
 import json
 
 
-VER = "2.2"
+VER = "2.3"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -31,69 +31,22 @@
 sugestedUpdateVersion = ""
 configFile = "config.ini"
 ScanRateLastRead = {}
 currentToken = ""
 g_connectorTypeName = ""
 g_lastGetTagsFromServer = None
 g_lastGetCloudVersionFromServer = None
-g_app_log = None
 
 def enum(**enums):
     return type("Enum", (), enums)
 
 TagStatus = enum(Invalid=10, Valid=20)
 
-def initialize_log(log_level=""):
-
-    global VER
-    global g_app_log
-    try:
-
-        global g_app_log
-        if g_app_log:
-            return
-
-
-        default_log_level = logging.WARNING
-        if log_level == "DEBUG":
-            default_log_level = logging.DEBUG
-        if log_level == "INFO":
-            default_log_level = logging.INFO
-        if log_level == "ERROR":
-            default_log_level = logging.ERROR
-
-        # Configure log formatter
-        log_formatter = logging.Formatter(
-            '%(asctime)s - %(name)s - %(funcName)s - (%(lineno)d) - %(levelname)s - %(message)s',
-        )
-
-        # Configure log handler
-        log_file = "CloudConnectorService.log"
-        log_handler = RotatingFileHandler(
-            log_file,
-            mode="a",
-            maxBytes=5 * 1024 * 1024,
-            backupCount=7,
-            encoding=None,
-            delay=0,
-        )
-        log_handler.setFormatter(log_formatter)
-
-        # Configure root logger
-        app_logger = logging.getLogger("root")
-        app_logger.setLevel(default_log_level)
-        app_logger.addHandler(log_handler)
-        log_handler.doRollover()
-
-        # Log initialization completion
-        app_logger.critical("initialize_log DONE")
-        g_app_log = app_logger
-
-    except Exception as ex:
-        logging.error("Error in initialize_log: %s", ex, exc_info=True)
+# Retrieve the logger instance
+logger = logging.getLogger(__name__)
 
 
 # ============================
 def read_last_rows_from_log(maxNumberOfRows=10):
     log_file_path = "CloudConnectorService.log"
     last_rows = []
     i = maxNumberOfRows
@@ -113,28 +66,29 @@
 
     except Exception as inst:
         print("Error in setLogLevel", inst)
 
 
 # ============================
 def ci_print(msg, level=""):
-    global g_app_log
     try:
+
         if level == "DEBUG":
-            g_app_log.debug(msg)
+            logger.debug(msg)
         elif level == "INFO":
-            g_app_log.info(msg)
+            logger.info(msg)
         elif level == "ERROR":
-            g_app_log.error(msg)
+            logger.error(msg)
+        elif level == "WARNING":
+            logger.warning(msg)
         else:
-            g_app_log.warning(msg)
+            logger.warning(msg)
 
-        # print(level+"::"+msg)
-    except Exception as inst:
-        g_app_log.warning("Main Exception :: " + inst)
+    except Exception as e:
+        logger.warning(f"An error occurred while logging: {e}")
 
 
 # ============================
 def SendLogToServer(log):
     try:
         ret = addCloudConnectorLog(log, datetime.now())
         return
@@ -191,15 +145,14 @@
 
             cfg_server_address = config.get("Server", "Address")
             cfg_username = config.get("Server", "username")
             cfg_password = config.get("Server", "password")
             cfg_max_files = config.get("Server", "maxFiles")
             log_level = config.get("Logging", "Level", fallback=cfg_log_level)
 
-            initialize_log(log_level)
 
             ci_print(f"Server Address: {cfg_server_address}", "INFO")
             ci_print(f"Username: {cfg_username}", "INFO")
             ci_print(f"Password: {cfg_password}", "INFO")
             ci_print(f"Max Files: {cfg_max_files}", "INFO")
             ci_print(f"VERSION: {getLocalVersion()}")
```

### Comparing `ci_cloudconnector-2.2/main.py` & `ci_cloudconnector-2.3/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.2/myservice_installer.py` & `ci_cloudconnector-2.3/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.2/setup.py` & `ci_cloudconnector-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="2.2",
+    version="2.3",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

