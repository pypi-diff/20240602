# Comparing `tmp/ci_cloudconnector-2.0.tar.gz` & `tmp/ci_cloudconnector-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-2.0.tar", last modified: Thu May 30 08:47:51 2024, max compression
+gzip compressed data, was "ci_cloudconnector-2.2.tar", last modified: Sun Jun  2 06:26:51 2024, max compression
```

## Comparing `ci_cloudconnector-2.0.tar` & `ci_cloudconnector-2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:47:51.887206 ci_cloudconnector-2.0/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:47:51.887206 ci_cloudconnector-2.0/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 08:47:51.000000 ci_cloudconnector-2.0/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 08:47:51.000000 ci_cloudconnector-2.0/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:47:51.000000 ci_cloudconnector-2.0/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 08:47:51.000000 ci_cloudconnector-2.0/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 08:47:51.887206 ci_cloudconnector-2.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-2.0/README.txt
--rw-rw-rw-   0        0        0    39003 2024-05-30 08:47:38.000000 ci_cloudconnector-2.0/logic.py
--rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-2.0/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-2.0/myservice.py
--rw-rw-rw-   0        0        0      964 2024-05-30 08:23:50.000000 ci_cloudconnector-2.0/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 08:47:51.887206 ci_cloudconnector-2.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-30 08:47:44.000000 ci_cloudconnector-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:26:51.361250 ci_cloudconnector-2.2/
+drwxrwxrwx   0        0        0        0 2024-06-02 06:26:51.355439 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-02 06:26:51.000000 ci_cloudconnector-2.2/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-06-02 06:26:51.358201 ci_cloudconnector-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-2.2/README.txt
+-rw-rw-rw-   0        0        0    38161 2024-06-02 06:26:03.000000 ci_cloudconnector-2.2/logic.py
+-rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-2.2/main.py
+-rw-rw-rw-   0        0        0     3384 2024-06-02 06:24:12.000000 ci_cloudconnector-2.2/myservice.py
+-rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.2/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 06:26:51.362209 ci_cloudconnector-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-06-02 06:20:15.000000 ci_cloudconnector-2.2/setup.py
```

### Comparing `ci_cloudconnector-2.0/logic.py` & `ci_cloudconnector-2.2/logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 
-import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
+import logging, time, datetime, sys, socket, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
+from cpppo.server.enip import address, client
+from logging.handlers import RotatingFileHandler
+import os
+import configparser
+import requests
+import json
 
-from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "2.0"
+VER = "2.2"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -38,56 +43,62 @@
 TagStatus = enum(Invalid=10, Valid=20)
 
 def initialize_log(log_level=""):
 
     global VER
     global g_app_log
     try:
+
+        global g_app_log
         if g_app_log:
             return
 
+
         default_log_level = logging.WARNING
         if log_level == "DEBUG":
             default_log_level = logging.DEBUG
         if log_level == "INFO":
             default_log_level = logging.INFO
         if log_level == "ERROR":
             default_log_level = logging.ERROR
 
-        from logging.handlers import RotatingFileHandler
-
+        # Configure log formatter
         log_formatter = logging.Formatter(
-            "%(asctime)s %(levelname)s %(funcName)s(%(lineno)d) %(message)s"
+            '%(asctime)s - %(name)s - %(funcName)s - (%(lineno)d) - %(levelname)s - %(message)s',
         )
-        log_file = "CI_CloudConnector.log"
+
+        # Configure log handler
+        log_file = "CloudConnectorService.log"
         log_handler = RotatingFileHandler(
             log_file,
             mode="a",
             maxBytes=5 * 1024 * 1024,
             backupCount=7,
             encoding=None,
             delay=0,
         )
         log_handler.setFormatter(log_formatter)
 
+        # Configure root logger
         app_logger = logging.getLogger("root")
         app_logger.setLevel(default_log_level)
         app_logger.addHandler(log_handler)
         log_handler.doRollover()
 
+        # Log initialization completion
         app_logger.critical("initialize_log DONE")
         g_app_log = app_logger
 
     except Exception as ex:
-        print("Error in initialize_log " +  str(ex))
+        logging.error("Error in initialize_log: %s", ex, exc_info=True)
 
 
 # ============================
 def read_last_rows_from_log(maxNumberOfRows=10):
-    log_file_path = "CI_CloudConnector.log"
+    log_file_path = "CloudConnectorService.log"
     last_rows = []
     i = maxNumberOfRows
     for line in reversed(open(log_file_path, "r").readlines()):
         last_rows.append(line.rstrip())
         i = i - 1
         if i <= 0:
             return last_rows
@@ -120,66 +131,51 @@
         # print(level+"::"+msg)
     except Exception as inst:
         g_app_log.warning("Main Exception :: " + inst)
 
 
 # ============================
 def SendLogToServer(log):
-
     try:
-        print("send ::") + log
-        ret = addCloudConnectorLog(log, datetime.now)
-    except:
+        ret = addCloudConnectorLog(log, datetime.now())
+        return
+    except Exception as e:
         return
 
 
 
 # ============================
 def handleError(message, err):
     try:
+
         err_desc = str(err)
         exc_type, exc_obj, exc_tb = sys.exc_info()
-        fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+        fname = os.path.basename(exc_tb.tb_frame.f_code.co_filename)
         srtMsg = (
-            message
-            + " , "
-            + str(err_desc)
-            + " , "
-            + str(exc_type)
-            + " , "
-            + str(fname)
-            + " , "
-            + str(exc_tb.tb_lineno)
+            f"{message} , {err_desc} , {exc_type} , {fname} , {exc_tb.tb_lineno}"
         )
-        # print(message, err_desc, exc_type, fname, exc_tb.tb_lineno)
         ci_print(srtMsg, "ERROR")
-    except Exception as errIgnore:
-        ci_print("Error in handleError " + str(errIgnore), "ERROR")
+    except Exception as inner_err:
+        ci_print(f"Error in handleError: {inner_err}", "ERROR")
 
 
 # ============================
 def getAliveFile():
-
     ret = None
     try:
-        fileName = "/" + HomeDir + "/lc_pid.txt"
-        # read alive file
-        f = open(fileName, "r")
-        ret = json.load(f)
-        # print 'getAliveFile file=' + str(ret)
-    except Exception as inst:
-        handleError("Error in getAliveFile", inst)
+        file_path = "/" + HomeDir + "/lc_pid.txt"
+        with open(file_path, "r") as file:
+            ret = json.load(file)
+    except Exception as e:
+        handleError("Error reading alive file: %s", e)
     return ret
 
 
 # ============================
 
-import os
-import configparser
-
 def initialize_config(overwrite=False):
 
     global cfg_server_address
     global cfg_username
     global cfg_password
     global cfg_max_files
     global cfg_log_level
@@ -254,16 +250,15 @@
     except Exception as ex:
         handleError("Error in reboot", ex)
 
 
 
 # Cloud Functions
 # ============================
-import requests
-import json
+
 
 cfg_server_address = "your_server_address"
 g_VerifySSL = True
 currentToken = ""
 cfg_username = "your_username"
 cfg_password = "your_password"
 
@@ -386,22 +381,16 @@
         getVersionTimePass = 0
 
         if g_lastGetCloudVersionFromServer:
             getVersionTimePass = (now - g_lastGetCloudVersionFromServer).total_seconds()
 
         if getVersionTimePass == 0 or getVersionTimePass > GetCloudVersionFromServerMinRateSeconds:
 
-            # print "update pid file for watchdog"
-            # do after clock settings because some times the machine loads with old clock and trigger watchdog
-
-            # print "handleNewRequests"
             handleNewRequests()
 
-            # print 'getting version from server'
-
             g_lastGetCloudVersionFromServer = datetime.now()
             ip_address = socket.gethostbyname(socket.gethostname())
             url = f"{cfg_server_address}/api/CloudConnector/GetVersion/?version={VER}&IpAddress={ip_address}"
 
             ret = ciRequest(url, None, "get", "getCloudVersion", token)
             response = ret["response"]
 
@@ -579,17 +568,14 @@
         payload = []
         logData = {"Log": log, "TimeStamp": str(timeStamp), "RequestId": requestId}
         payload.append(logData)
         # print str(payload)
         ret = ciRequest(url, json.dumps(payload), "post", "SetConnectorLog", token)
         response = ret["response"]
 
-        # print (response.text)
-        # logging.info('setCloudTags response = ' + str(response) + ' : ' + response.text )
-        # print '==' + str(response.status_code)
         updatedSuccessfully = response.status_code == 200
 
     except Exception as inst:
         handleError("Exception in addCloudConnectorLog", inst)
         return False
 
     return updatedSuccessfully
@@ -602,15 +588,15 @@
     token = currentToken
 
 
     ans = None
     try:
         url = cfg_server_address + "/api/CloudConnector/GetCloudConnectorRequests/"
         ret = ciRequest(url, None, "get", "GetCloudConnectorRequests", token)
-        # print "ret=" + str(ret)
+
         response = ret["response"]
         if ret["isOK"] == True:
             ans = json.loads(response.text)
     except Exception as inst:
         handleError("Error getting requests from cloud", inst)
         ans = None
 
@@ -631,26 +617,22 @@
         url = (
             cfg_server_address
             + "/api/CloudConnector/SetCounterRequestStatus/?requestId="
             + str(requestId)
             + "&status="
             + str(status)
         )
-        # print "url="+url
+
         ret = ciRequest(url, "", "post", "SetCounterRequestStatus", token)
         response = ret["response"]
 
-        print(response.text)
-        # logging.info('setCloudTags response = ' + str(response) + ' : ' + response.text )
-        # print '==' + str(response.status_code)
         updatedSuccessfully = response.status_code == 200
 
     except Exception as inst:
         handleError("Exception in addCloudConnectorLog", inst)
-        # handleError("Error setting tags in cloud", inst)
         return False
 
     return updatedSuccessfully
 
 
 # get requests from cloud and handle it
 # ============================
```

### Comparing `ci_cloudconnector-2.0/main.py` & `ci_cloudconnector-2.2/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.0/setup.py` & `ci_cloudconnector-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="2.0",
+    version="2.2",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

