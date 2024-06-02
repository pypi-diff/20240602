# Comparing `tmp/MzhFunc-0.0.1.tar.gz` & `tmp/MzhFunc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MzhFunc-0.0.1.tar", last modified: Sun Jun  2 12:17:52 2024, max compression
+gzip compressed data, was "MzhFunc-0.0.2.tar", last modified: Sun Jun  2 12:47:19 2024, max compression
```

## Comparing `MzhFunc-0.0.1.tar` & `MzhFunc-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 12:17:52.027535 MzhFunc-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:17:52.023535 MzhFunc-0.0.1/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      398 2024-06-02 12:17:51.000000 MzhFunc-0.0.1/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-06-02 12:17:51.000000 MzhFunc-0.0.1/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 12:17:51.000000 MzhFunc-0.0.1/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-02 12:17:51.000000 MzhFunc-0.0.1/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      398 2024-06-02 12:17:52.027535 MzhFunc-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 12:17:52.026535 MzhFunc-0.0.1/db/
--rw-rw-rw-   0        0        0     6621 2024-06-01 18:41:23.000000 MzhFunc-0.0.1/db/MzhFunc.py
--rw-rw-rw-   0        0        0      207 2024-06-01 17:18:13.000000 MzhFunc-0.0.1/db/__init__.py
--rw-rw-rw-   0        0        0        0 2024-06-01 16:55:46.000000 MzhFunc-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 12:17:52.027535 MzhFunc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      899 2024-06-02 12:17:45.000000 MzhFunc-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:47:19.009369 MzhFunc-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:47:19.007369 MzhFunc-0.0.2/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      398 2024-06-02 12:47:19.009369 MzhFunc-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 12:47:19.008369 MzhFunc-0.0.2/db/
+-rw-rw-rw-   0        0        0     6335 2024-06-02 12:42:33.000000 MzhFunc-0.0.2/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      207 2024-06-01 17:18:13.000000 MzhFunc-0.0.2/db/__init__.py
+-rw-rw-rw-   0        0        0       67 2024-06-02 12:33:29.000000 MzhFunc-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:47:19.009369 MzhFunc-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      899 2024-06-02 12:47:15.000000 MzhFunc-0.0.2/setup.py
```

### Comparing `MzhFunc-0.0.1/db/MzhFunc.py` & `MzhFunc-0.0.2/db/MzhFunc.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,16 @@
 from email.header import Header
 import requests
 import pandas as pd
 import xlrd
 import openpyxl
 import os
 """
-2099cd35d78f6431
-5f9600081ec1b0ea
-6dfe56f9a32582af
-e0dd19d1803a51d7
-da4710f18a9a19ed
-e51e17c80da377b4
-732a3033a742f248
-77fb64e1c22d6ceb
-
-cd pip && python setup.py sdist
+cd pip & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist
 twine upload dist/*
-pypi-AgEIcHlwaS5vcmcCJDRmMGRhNGJiLTM4ZDktNDlkNi1iMjc1LWExNmU3YmIwYmFkMwACKlszLCJjMjQ1NzNhNy01ZjQzLTQ2MDktODFmZi04MjQ5NjY4MmY0MWUiXQAABiDkEBiGZim6aIww1x2eC03oY0MKJdNumwZ8d5Gpd9F1pg
 """
 
 
 def cmd_utf(order):
     proc = Popen(order, stdin=None, stdout=PIPE, stderr=PIPE, shell=True)
     outinfo, errinfo = proc.communicate()
     outinfo = outinfo.decode('utf-8')
```

### Comparing `MzhFunc-0.0.1/setup.py` & `MzhFunc-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 rd /S /Q "d:\pybuild"&&mkdir "d:\pybuild"&&pyinstaller D:/python/函数/pip\setup.py.py --workpath d:\pybuild  --distpath d:\pybuild\dist
 """
 import setuptools
 
 
 setuptools.setup(
     name="MzhFunc",
-    version='0.0.1',
+    version='0.0.2',
     author="Author's name",  # 作者名称
     author_email="xxxxxxx@163.com",  # 作者邮箱
     description="Python helper tools",  # 库描述
     long_description='python for mytools',
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/yourtools/",  # 库的官方地址
     packages=setuptools.find_packages(),
```

