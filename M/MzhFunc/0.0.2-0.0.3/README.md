# Comparing `tmp/MzhFunc-0.0.2.tar.gz` & `tmp/MzhFunc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MzhFunc-0.0.2.tar", last modified: Sun Jun  2 12:47:19 2024, max compression
+gzip compressed data, was "MzhFunc-0.0.3.tar", last modified: Sun Jun  2 15:08:32 2024, max compression
```

## Comparing `MzhFunc-0.0.2.tar` & `MzhFunc-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 12:47:19.009369 MzhFunc-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:47:19.007369 MzhFunc-0.0.2/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      398 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-02 12:47:18.000000 MzhFunc-0.0.2/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      398 2024-06-02 12:47:19.009369 MzhFunc-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 12:47:19.008369 MzhFunc-0.0.2/db/
--rw-rw-rw-   0        0        0     6335 2024-06-02 12:42:33.000000 MzhFunc-0.0.2/db/MzhFunc.py
--rw-rw-rw-   0        0        0      207 2024-06-01 17:18:13.000000 MzhFunc-0.0.2/db/__init__.py
--rw-rw-rw-   0        0        0       67 2024-06-02 12:33:29.000000 MzhFunc-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 12:47:19.009369 MzhFunc-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      899 2024-06-02 12:47:15.000000 MzhFunc-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:08:32.655269 MzhFunc-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-06-02 15:08:32.652350 MzhFunc-0.0.3/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      399 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-02 15:08:32.000000 MzhFunc-0.0.3/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      399 2024-06-02 15:08:32.654297 MzhFunc-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 MzhFunc-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 15:08:32.654297 MzhFunc-0.0.3/db/
+-rw-rw-rw-   0        0        0    12412 2024-06-02 15:08:28.000000 MzhFunc-0.0.3/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      207 2024-06-01 17:18:13.000000 MzhFunc-0.0.3/db/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-06-02 13:12:49.000000 MzhFunc-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:08:32.655269 MzhFunc-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2024-06-02 15:08:28.000000 MzhFunc-0.0.3/setup.py
```

### Comparing `MzhFunc-0.0.2/setup.py` & `MzhFunc-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # -*- coding: utf-8 -*-
 r"""
 Created on 2024/6/2 0:57
 rd /S /Q "d:\pybuild"&&mkdir "d:\pybuild"&&pyinstaller D:/python/函数/pip\setup.py.py --workpath d:\pybuild  --distpath d:\pybuild\dist
+
+cd pip & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist && twine upload dist/*
+
 """
 import setuptools
 
 
 setuptools.setup(
     name="MzhFunc",
-    version='0.0.2',
+    version='0.0.3',
     author="Author's name",  # 作者名称
-    author_email="xxxxxxx@163.com",  # 作者邮箱
+    author_email="191891173@qq.com",  # 作者邮箱
     description="Python helper tools",  # 库描述
     long_description='python for mytools',
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/yourtools/",  # 库的官方地址
     packages=setuptools.find_packages(),
     data_files=["requirements.txt"],  # yourtools库依赖的其他库
     classifiers=[
```

