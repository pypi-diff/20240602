# Comparing `tmp/ci_cloudconnector-2.4.tar.gz` & `tmp/ci_cloudconnector-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-2.4.tar", last modified: Sun Jun  2 07:22:28 2024, max compression
+gzip compressed data, was "ci_cloudconnector-2.5.tar", last modified: Sun Jun  2 07:26:38 2024, max compression
```

## Comparing `ci_cloudconnector-2.4.tar` & `ci_cloudconnector-2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 07:22:28.181548 ci_cloudconnector-2.4/
-drwxrwxrwx   0        0        0        0 2024-06-02 07:22:28.160689 ci_cloudconnector-2.4/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-06-02 07:22:27.000000 ci_cloudconnector-2.4/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-06-02 07:22:27.000000 ci_cloudconnector-2.4/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 07:22:27.000000 ci_cloudconnector-2.4/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-06-02 07:22:27.000000 ci_cloudconnector-2.4/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-06-02 07:22:28.177492 ci_cloudconnector-2.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-2.4/README.txt
--rw-rw-rw-   0        0        0    36703 2024-06-02 07:18:22.000000 ci_cloudconnector-2.4/logic.py
--rw-rw-rw-   0        0        0     8242 2024-06-02 07:09:11.000000 ci_cloudconnector-2.4/main.py
--rw-rw-rw-   0        0        0     4156 2024-06-02 07:16:02.000000 ci_cloudconnector-2.4/myservice.py
--rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.4/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-06-02 07:22:28.181548 ci_cloudconnector-2.4/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-06-02 07:18:26.000000 ci_cloudconnector-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:26:38.165165 ci_cloudconnector-2.5/
+drwxrwxrwx   0        0        0        0 2024-06-02 07:26:38.159998 ci_cloudconnector-2.5/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-06-02 07:26:37.000000 ci_cloudconnector-2.5/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-06-02 07:26:38.000000 ci_cloudconnector-2.5/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:26:37.000000 ci_cloudconnector-2.5/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-02 07:26:37.000000 ci_cloudconnector-2.5/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-06-02 07:26:38.162165 ci_cloudconnector-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-2.5/README.txt
+-rw-rw-rw-   0        0        0    36703 2024-06-02 07:26:04.000000 ci_cloudconnector-2.5/logic.py
+-rw-rw-rw-   0        0        0     8242 2024-06-02 07:09:11.000000 ci_cloudconnector-2.5/main.py
+-rw-rw-rw-   0        0        0     4155 2024-06-02 07:25:45.000000 ci_cloudconnector-2.5/myservice.py
+-rw-rw-rw-   0        0        0     1601 2024-06-02 05:37:40.000000 ci_cloudconnector-2.5/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 07:26:38.165165 ci_cloudconnector-2.5/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-06-02 07:26:08.000000 ci_cloudconnector-2.5/setup.py
```

### Comparing `ci_cloudconnector-2.4/logic.py` & `ci_cloudconnector-2.5/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from cpppo.server.enip import address, client
 import os
 import configparser
 import requests
 import json
 
-VER = "2.4"
+VER = "2.5"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-2.4/main.py` & `ci_cloudconnector-2.5/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.4/myservice.py` & `ci_cloudconnector-2.5/myservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, args):
         logging.basicConfig(
             level=logging.INFO,
             format='%(asctime)s - %(name)s - %(funcName)s - (%(lineno)d) - %(levelname)s - %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S'
         )
 
-        rotating_handler = logging.handlers.RotatingFileHandler(
+        rotating_handler = logging.Handler.RotatingFileHandler(
             filename='CloudConnectorService.log',
             mode="a",
             maxBytes=5 * 1024 * 1024,
             backupCount=10,
             encoding=None,
             delay=0,
         )
```

### Comparing `ci_cloudconnector-2.4/myservice_installer.py` & `ci_cloudconnector-2.5/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-2.4/setup.py` & `ci_cloudconnector-2.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="2.4",
+    version="2.5",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

