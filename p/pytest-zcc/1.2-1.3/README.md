# Comparing `tmp/pytest_zcc-1.2.tar.gz` & `tmp/pytest_zcc-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_zcc-1.2.tar", last modified: Sun Jun  2 08:08:31 2024, max compression
+gzip compressed data, was "pytest_zcc-1.3.tar", last modified: Sun Jun  2 08:19:44 2024, max compression
```

## Comparing `pytest_zcc-1.2.tar` & `pytest_zcc-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 08:08:31.645018 pytest_zcc-1.2/
--rw-rw-rw-   0        0        0      342 2024-06-02 08:08:31.644020 pytest_zcc-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 08:08:31.644020 pytest_zcc-1.2/pytest_zcc.egg-info/
--rw-rw-rw-   0        0        0      342 2024-06-02 08:08:31.000000 pytest_zcc-1.2/pytest_zcc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-06-02 08:08:31.000000 pytest_zcc-1.2/pytest_zcc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 08:08:31.000000 pytest_zcc-1.2/pytest_zcc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-06-02 08:08:31.000000 pytest_zcc-1.2/pytest_zcc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-06-02 08:08:31.000000 pytest_zcc-1.2/pytest_zcc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-06-02 08:08:31.000000 pytest_zcc-1.2/pytest_zcc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 08:08:31.000000 pytest_zcc-1.2/pytest_zcc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 08:08:31.645018 pytest_zcc-1.2/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-06-02 08:08:28.000000 pytest_zcc-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 08:19:44.839404 pytest_zcc-1.3/
+-rw-rw-rw-   0        0        0      342 2024-06-02 08:19:44.839404 pytest_zcc-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 08:19:44.839404 pytest_zcc-1.3/pytest_zcc.egg-info/
+-rw-rw-rw-   0        0        0      342 2024-06-02 08:19:44.000000 pytest_zcc-1.3/pytest_zcc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-06-02 08:19:44.000000 pytest_zcc-1.3/pytest_zcc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 08:19:44.000000 pytest_zcc-1.3/pytest_zcc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-02 08:19:44.000000 pytest_zcc-1.3/pytest_zcc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-06-02 08:19:44.000000 pytest_zcc-1.3/pytest_zcc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-06-02 08:19:44.000000 pytest_zcc-1.3/pytest_zcc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 08:19:44.000000 pytest_zcc-1.3/pytest_zcc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 08:19:44.839404 pytest_zcc-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      738 2024-06-02 08:19:38.000000 pytest_zcc-1.3/setup.py
```

### Comparing `pytest_zcc-1.2/setup.py` & `pytest_zcc-1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytest_zcc',
     url='https://github.com/xx/',
-    version='1.2',
+    version='1.3',
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
-            'pytest_zcc = pytest_zccdev'
+            'pytest_zcc = devhooks.pytest_zccdev'
         ]
     },
     zip_safe=False
 )
```

