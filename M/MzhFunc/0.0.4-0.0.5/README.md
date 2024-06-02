# Comparing `tmp/MzhFunc-0.0.4.tar.gz` & `tmp/MzhFunc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MzhFunc-0.0.4.tar", last modified: Sun Jun  2 15:32:06 2024, max compression
+gzip compressed data, was "MzhFunc-0.0.5.tar", last modified: Sun Jun  2 15:50:52 2024, max compression
```

## Comparing `MzhFunc-0.0.4.tar` & `MzhFunc-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 15:32:06.762478 MzhFunc-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-06-02 15:32:06.757611 MzhFunc-0.0.4/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      397 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-02 15:32:06.000000 MzhFunc-0.0.4/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      397 2024-06-02 15:32:06.762478 MzhFunc-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 15:32:06.761504 MzhFunc-0.0.4/db/
--rw-rw-rw-   0        0        0    12414 2024-06-02 15:09:53.000000 MzhFunc-0.0.4/db/MzhFunc.py
--rw-rw-rw-   0        0        0      207 2024-06-01 17:18:13.000000 MzhFunc-0.0.4/db/__init__.py
--rw-rw-rw-   0        0        0       48 2024-06-02 13:12:49.000000 MzhFunc-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 15:32:06.763451 MzhFunc-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2018 2024-06-02 15:31:59.000000 MzhFunc-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:50:52.214371 MzhFunc-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-06-02 15:50:52.212425 MzhFunc-0.0.5/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      397 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-02 15:50:52.000000 MzhFunc-0.0.5/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      397 2024-06-02 15:50:52.214371 MzhFunc-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 15:50:52.213398 MzhFunc-0.0.5/db/
+-rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 MzhFunc-0.0.5/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 MzhFunc-0.0.5/db/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-06-02 13:12:49.000000 MzhFunc-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:50:52.214371 MzhFunc-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2026 2024-06-02 15:37:07.000000 MzhFunc-0.0.5/setup.py
```

### Comparing `MzhFunc-0.0.4/db/MzhFunc.py` & `MzhFunc-0.0.5/db/MzhFunc.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import requests
 import pandas as pd
 import xlrd
 import openpyxl
 import os
 
 """
-cd pip & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist && twine upload dist/*
+cd MzhFunc & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist && twine upload dist/*
 """
 
 
 def qywx_sendtxt(text, key, all=None):
     """
     向指定企业微信群发送文本信息
     :param text: 发送的文本内容
```

### Comparing `MzhFunc-0.0.4/setup.py` & `MzhFunc-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 r"""
 Created on 2024/6/2 0:57
-rd /S /Q "d:\pybuild"&&mkdir "d:\pybuild"&&pyinstaller D:/python/函数/pip\setup.py.py --workpath d:\pybuild  --distpath d:\pybuild\dist
+rd /S /Q "d:\pybuild"&&mkdir "d:\pybuild"&&pyinstaller D:/python/函数/MzhFunc\setup.py.py --workpath d:\pybuild  --distpath d:\pybuild\dist
 
-cd pip & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist && twine upload dist/*
+cd MzhFunc & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist && twine upload dist/*
 
 """
 import os
 import re
 import requests
 import setuptools
 from bs4 import BeautifulSoup
```

