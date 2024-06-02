# Comparing `tmp/pytest_zcc-1.0.tar.gz` & `tmp/pytest_zcc-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_zcc-1.0.tar", last modified: Sun Jun  2 07:34:45 2024, max compression
+gzip compressed data, was "pytest_zcc-1.1.tar", last modified: Sun Jun  2 08:03:32 2024, max compression
```

## Comparing `pytest_zcc-1.0.tar` & `pytest_zcc-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 07:34:45.015457 pytest_zcc-1.0/
--rw-rw-rw-   0        0        0      342 2024-06-02 07:34:45.015457 pytest_zcc-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 07:34:45.014186 pytest_zcc-1.0/pytest_zcc.egg-info/
--rw-rw-rw-   0        0        0      342 2024-06-02 07:34:44.000000 pytest_zcc-1.0/pytest_zcc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-06-02 07:34:44.000000 pytest_zcc-1.0/pytest_zcc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 07:34:44.000000 pytest_zcc-1.0/pytest_zcc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 07:34:44.000000 pytest_zcc-1.0/pytest_zcc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-06-02 07:34:44.000000 pytest_zcc-1.0/pytest_zcc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-06-02 07:34:44.000000 pytest_zcc-1.0/pytest_zcc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 07:34:44.000000 pytest_zcc-1.0/pytest_zcc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 07:34:45.015457 pytest_zcc-1.0/setup.cfg
--rw-rw-rw-   0        0        0      733 2024-06-02 06:37:42.000000 pytest_zcc-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 08:03:32.473019 pytest_zcc-1.1/
+-rw-rw-rw-   0        0        0      342 2024-06-02 08:03:32.473019 pytest_zcc-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 08:03:32.473019 pytest_zcc-1.1/pytest_zcc.egg-info/
+-rw-rw-rw-   0        0        0      342 2024-06-02 08:03:32.000000 pytest_zcc-1.1/pytest_zcc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-06-02 08:03:32.000000 pytest_zcc-1.1/pytest_zcc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 08:03:32.000000 pytest_zcc-1.1/pytest_zcc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-06-02 08:03:32.000000 pytest_zcc-1.1/pytest_zcc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-06-02 08:03:32.000000 pytest_zcc-1.1/pytest_zcc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-06-02 08:03:32.000000 pytest_zcc-1.1/pytest_zcc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 08:03:32.000000 pytest_zcc-1.1/pytest_zcc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 08:03:32.473019 pytest_zcc-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-06-02 08:03:27.000000 pytest_zcc-1.1/setup.py
```

### Comparing `pytest_zcc-1.0/setup.py` & `pytest_zcc-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytest_zcc',
     url='https://github.com/xx/',
-    version='1.0',
+    version='1.1',
     author='zcc',
     author_email="1059995908@qq.com",
     description='eee',
     long_description='eee',
     classifiers=[
         # pipy搜索索引分类
         'Framework :: Pytest',
@@ -20,12 +20,12 @@
         'pytest', 'py.test', 'pytest_zcc'
     ],
     install_requires=[
         'pytest'
     ],
     entry_points={
         'pytest11':[
-            'pytest_zcc = src.pytest_zccdev'
+            'pytest_zcc = pytest_zccdev'
         ]
     },
     zip_safe=False
 )
```

