# Comparing `tmp/MzhFunc-0.0.3.tar.gz` & `tmp/MzhFunc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MzhFunc-0.0.3.tar", last modified: Sun Jun  2 15:08:32 2024, max compression
+gzip compressed data, was "MzhFunc-0.0.4.tar", last modified: Sun Jun  2 15:32:06 2024, max compression
```

## Comparing `MzhFunc-0.0.3.tar` & `MzhFunc-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 15:08:32.655269 MzhFunc-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-06-02 15:08:32.652350 MzhFunc-0.0.3/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      399 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      399 2024-06-02 15:08:32.654297 MzhFunc-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 15:08:32.654297 MzhFunc-0.0.3/db/
--rw-rw-rw-   0        0        0    12412 2024-06-02 15:08:28.000000 MzhFunc-0.0.3/db/MzhFunc.py
--rw-rw-rw-   0        0        0      207 2024-06-01 17:18:13.000000 MzhFunc-0.0.3/db/__init__.py
--rw-rw-rw-   0        0        0       48 2024-06-02 13:12:49.000000 MzhFunc-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 15:08:32.655269 MzhFunc-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1001 2024-06-02 15:08:28.000000 MzhFunc-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:32:06.762478 MzhFunc-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-06-02 15:32:06.757611 MzhFunc-0.0.4/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      397 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      397 2024-06-02 15:32:06.762478 MzhFunc-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 15:32:06.761504 MzhFunc-0.0.4/db/
+-rw-rw-rw-   0        0        0    12414 2024-06-02 15:09:53.000000 MzhFunc-0.0.4/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      207 2024-06-01 17:18:13.000000 MzhFunc-0.0.4/db/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-06-02 13:12:49.000000 MzhFunc-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:32:06.763451 MzhFunc-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2018 2024-06-02 15:31:59.000000 MzhFunc-0.0.4/setup.py
```

### Comparing `MzhFunc-0.0.3/db/MzhFunc.py` & `MzhFunc-0.0.4/db/MzhFunc.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 import requests
 import pandas as pd
 import xlrd
 import openpyxl
 import os
 
 """
-cd pip & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist
-twine upload dist/*
+cd pip & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist && twine upload dist/*
 """
 
 
 def qywx_sendtxt(text, key, all=None):
     """
     向指定企业微信群发送文本信息
     :param text: 发送的文本内容
```

