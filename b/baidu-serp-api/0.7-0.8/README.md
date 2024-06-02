# Comparing `tmp/baidu_serp_api-0.7.tar.gz` & `tmp/baidu_serp_api-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidu_serp_api-0.7.tar", last modified: Sat Jun  1 16:55:05 2024, max compression
+gzip compressed data, was "baidu_serp_api-0.8.tar", last modified: Sun Jun  2 10:17:46 2024, max compression
```

## Comparing `baidu_serp_api-0.7.tar` & `baidu_serp_api-0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/baidu_serp_api/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/baidu_mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/baidu_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/baidu_serp_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/baidu_serp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 16:55:05.000000 baidu_serp_api-0.7/baidu_serp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:55:05.098178 baidu_serp_api-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:55:05.094179 baidu_serp_api-0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 16:55:00.000000 baidu_serp_api-0.7/tests/test_baidu_serp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:17:46.326171 baidu_serp_api-0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-06-02 10:17:46.326171 baidu_serp_api-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:17:46.326171 baidu_serp_api-0.8/baidu_serp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/baidu_serp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/baidu_serp_api/baidu_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/baidu_serp_api/baidu_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/baidu_serp_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:17:46.326171 baidu_serp_api-0.8/baidu_serp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-06-02 10:17:46.000000 baidu_serp_api-0.8/baidu_serp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-02 10:17:46.000000 baidu_serp_api-0.8/baidu_serp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:17:46.000000 baidu_serp_api-0.8/baidu_serp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-02 10:17:46.000000 baidu_serp_api-0.8/baidu_serp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 10:17:46.000000 baidu_serp_api-0.8/baidu_serp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:17:46.326171 baidu_serp_api-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:17:46.326171 baidu_serp_api-0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-02 10:17:38.000000 baidu_serp_api-0.8/tests/test_baidu_serp_api.py
```

### Comparing `baidu_serp_api-0.7/LICENSE.txt` & `baidu_serp_api-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.7/PKG-INFO` & `baidu_serp_api-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.7
+Version: 0.8
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.7/README.md` & `baidu_serp_api-0.8/README.md`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.7/baidu_serp_api/baidu_mobile.py` & `baidu_serp_api-0.8/baidu_serp_api/baidu_mobile.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.date_range = None
         self.pn = None
         self.proxies = None
 
     def extract_baidum_data(self, html_content):
         search_data = []
         soup = BeautifulSoup(html_content, 'html.parser')
-        search_results = soup.select('div[tpl="www_index"]')
+        search_results = soup.select('div[tpl="www_index"], div[tpl="www_struct"]')
         for result in search_results:
             title_element = result.find('p', class_='cu-title')
 
             url = result.get('data-log')
             if url:
                 url = json.loads(url)['mu']
```

### Comparing `baidu_serp_api-0.7/baidu_serp_api/baidu_pc.py` & `baidu_serp_api-0.8/baidu_serp_api/baidu_pc.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.7/baidu_serp_api/util.py` & `baidu_serp_api-0.8/baidu_serp_api/util.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.7/baidu_serp_api.egg-info/PKG-INFO` & `baidu_serp_api-0.8/baidu_serp_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.7
+Version: 0.8
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.7/setup.py` & `baidu_serp_api-0.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='baidu-serp-api',
-    version='0.7',
+    version='0.8',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `baidu_serp_api-0.7/tests/test_baidu_serp_api.py` & `baidu_serp_api-0.8/tests/test_baidu_serp_api.py`

 * *Files identical despite different names*

