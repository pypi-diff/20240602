# Comparing `tmp/krdict.py-3.0.0.tar.gz` & `tmp/krdict.py-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krdict.py-3.0.0.tar", last modified: Sun Oct 23 20:59:44 2022, max compression
+gzip compressed data, was "krdict_py-3.0.1.tar", last modified: Sun Jun  2 17:19:12 2024, max compression
```

## Comparing `krdict.py-3.0.0.tar` & `krdict.py-3.0.1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-10-23 20:59:44.359453 krdict.py-3.0.0/
--rw-rw-rw-   0        0        0     1085 2021-10-03 03:42:17.000000 krdict.py-3.0.0/LICENSE
--rw-rw-rw-   0        0        0      164 2022-09-20 01:41:42.000000 krdict.py-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2410 2022-10-23 20:59:44.359453 krdict.py-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1631 2022-09-25 01:32:36.000000 krdict.py-3.0.0/PYPI_README.md
--rw-rw-rw-   0        0        0     2124 2022-09-25 01:32:47.000000 krdict.py-3.0.0/README.md
--rw-rw-rw-   0        0        0      937 2022-10-23 20:59:44.364442 krdict.py-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-03-19 16:26:08.000000 krdict.py-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-23 20:59:44.272282 krdict.py-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-10-23 20:59:44.282659 krdict.py-3.0.0/src/krdict/
--rw-rw-rw-   0        0        0     1223 2022-09-20 23:39:33.000000 krdict.py-3.0.0/src/krdict/__init__.py
--rw-rw-rw-   0        0        0     5368 2022-03-20 00:07:07.000000 krdict.py-3.0.0/src/krdict/korean-go-kr-chain.pem
--rw-rw-rw-   0        0        0     4448 2022-09-24 17:21:33.000000 krdict.py-3.0.0/src/krdict/main.py
--rw-rw-rw-   0        0        0    33401 2022-09-19 23:19:28.000000 krdict.py-3.0.0/src/krdict/main.pyi
--rw-rw-rw-   0        0        0     5453 2022-09-24 15:58:23.000000 krdict.py-3.0.0/src/krdict/request.py
--rw-rw-rw-   0        0        0      472 2022-09-19 23:50:09.000000 krdict.py-3.0.0/src/krdict/request.pyi
--rw-rw-rw-   0        0        0     3348 2022-09-20 02:17:55.000000 krdict.py-3.0.0/src/krdict/response.py
--rw-rw-rw-   0        0        0      338 2022-09-21 02:00:57.000000 krdict.py-3.0.0/src/krdict/response.pyi
-drwxrwxrwx   0        0        0        0 2022-10-23 20:59:44.302606 krdict.py-3.0.0/src/krdict/scraper/
--rw-rw-rw-   0        0        0     1094 2022-09-20 23:53:15.000000 krdict.py-3.0.0/src/krdict/scraper/__init__.py
--rw-rw-rw-   0        0        0    22254 2022-09-19 23:19:28.000000 krdict.py-3.0.0/src/krdict/scraper/constants.py
--rw-rw-rw-   0        0        0     4975 2022-09-20 23:53:48.000000 krdict.py-3.0.0/src/krdict/scraper/main.py
--rw-rw-rw-   0        0        0     5351 2022-09-24 21:18:23.000000 krdict.py-3.0.0/src/krdict/scraper/main.pyi
--rw-rw-rw-   0        0        0    27452 2022-09-21 00:35:21.000000 krdict.py-3.0.0/src/krdict/scraper/request.py
--rw-rw-rw-   0        0        0    31818 2022-09-19 23:19:28.000000 krdict.py-3.0.0/src/krdict/scraper/response.py
-drwxrwxrwx   0        0        0        0 2022-10-23 20:59:44.310585 krdict.py-3.0.0/src/krdict/types/
--rw-rw-rw-   0        0        0     5340 2022-09-24 22:58:13.000000 krdict.py-3.0.0/src/krdict/types/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-23 20:59:44.358456 krdict.py-3.0.0/src/krdict/types/enums/
--rw-rw-rw-   0        0        0    11266 2022-09-21 00:17:32.000000 krdict.py-3.0.0/src/krdict/types/enums/__init__.py
--rw-rw-rw-   0        0        0     1755 2022-09-20 00:28:35.000000 krdict.py-3.0.0/src/krdict/types/enums/base.py
--rw-rw-rw-   0        0        0     1021 2022-09-19 22:36:13.000000 krdict.py-3.0.0/src/krdict/types/enums/base.pyi
--rw-rw-rw-   0        0        0    20638 2022-09-20 00:37:52.000000 krdict.py-3.0.0/src/krdict/types/enums/semantic_category.py
--rw-rw-rw-   0        0        0    14139 2022-09-20 00:37:56.000000 krdict.py-3.0.0/src/krdict/types/enums/subject_category.py
--rw-rw-rw-   0        0        0      814 2022-09-20 00:05:08.000000 krdict.py-3.0.0/src/krdict/types/exceptions.py
--rw-rw-rw-   0        0        0      100 2021-12-05 21:04:38.000000 krdict.py-3.0.0/src/krdict/types/exceptions.pyi
--rw-rw-rw-   0        0        0    13016 2022-10-23 20:53:15.000000 krdict.py-3.0.0/src/krdict/types/main.py
--rw-rw-rw-   0        0        0    12983 2022-09-24 23:18:00.000000 krdict.py-3.0.0/src/krdict/types/scraper.py
-drwxrwxrwx   0        0        0        0 2022-10-23 20:59:44.292633 krdict.py-3.0.0/src/krdict.py.egg-info/
--rw-rw-rw-   0        0        0     2410 2022-10-23 20:59:44.000000 krdict.py-3.0.0/src/krdict.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2022-10-23 20:59:44.000000 krdict.py-3.0.0/src/krdict.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-23 20:59:44.000000 krdict.py-3.0.0/src/krdict.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-10-23 20:59:44.000000 krdict.py-3.0.0/src/krdict.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2022-09-19 23:20:26.000000 krdict.py-3.0.0/src/py.typed
+drwxrwxrwx   0        0        0        0 2024-06-02 17:19:12.694932 krdict_py-3.0.1/
+-rw-rw-rw-   0        0        0     1085 2021-10-03 03:42:17.000000 krdict_py-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      121 2024-06-02 16:59:10.000000 krdict_py-3.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2410 2024-06-02 17:19:12.693931 krdict_py-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1631 2022-10-28 01:49:54.000000 krdict_py-3.0.1/PYPI_README.md
+-rw-rw-rw-   0        0        0     2148 2024-06-02 17:00:54.000000 krdict_py-3.0.1/README.md
+-rw-rw-rw-   0        0        0      937 2024-06-02 17:19:12.696931 krdict_py-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-03-19 16:26:08.000000 krdict_py-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 17:19:12.602335 krdict_py-3.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 17:19:12.613334 krdict_py-3.0.1/src/krdict/
+-rw-rw-rw-   0        0        0     1223 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/__init__.py
+-rw-rw-rw-   0        0        0     4448 2024-06-02 15:20:45.000000 krdict_py-3.0.1/src/krdict/main.py
+-rw-rw-rw-   0        0        0    33401 2024-06-02 15:20:45.000000 krdict_py-3.0.1/src/krdict/main.pyi
+-rw-rw-rw-   0        0        0     5347 2024-06-02 16:59:10.000000 krdict_py-3.0.1/src/krdict/request.py
+-rw-rw-rw-   0        0        0      472 2024-06-02 15:20:45.000000 krdict_py-3.0.1/src/krdict/request.pyi
+-rw-rw-rw-   0        0        0     3348 2024-06-02 15:20:45.000000 krdict_py-3.0.1/src/krdict/response.py
+-rw-rw-rw-   0        0        0      338 2024-06-02 15:20:45.000000 krdict_py-3.0.1/src/krdict/response.pyi
+drwxrwxrwx   0        0        0        0 2024-06-02 17:19:12.633334 krdict_py-3.0.1/src/krdict/scraper/
+-rw-rw-rw-   0        0        0     1094 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/scraper/__init__.py
+-rw-rw-rw-   0        0        0    22254 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/scraper/constants.py
+-rw-rw-rw-   0        0        0     4975 2024-06-02 15:20:45.000000 krdict_py-3.0.1/src/krdict/scraper/main.py
+-rw-rw-rw-   0        0        0     5351 2024-06-02 15:20:45.000000 krdict_py-3.0.1/src/krdict/scraper/main.pyi
+-rw-rw-rw-   0        0        0    27303 2024-06-02 16:59:34.000000 krdict_py-3.0.1/src/krdict/scraper/request.py
+-rw-rw-rw-   0        0        0    31834 2024-06-02 16:59:34.000000 krdict_py-3.0.1/src/krdict/scraper/response.py
+drwxrwxrwx   0        0        0        0 2024-06-02 17:19:12.642780 krdict_py-3.0.1/src/krdict/types/
+-rw-rw-rw-   0        0        0     5340 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 17:19:12.690932 krdict_py-3.0.1/src/krdict/types/enums/
+-rw-rw-rw-   0        0        0    11266 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/types/enums/__init__.py
+-rw-rw-rw-   0        0        0     1755 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/types/enums/base.py
+-rw-rw-rw-   0        0        0     1021 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/types/enums/base.pyi
+-rw-rw-rw-   0        0        0    20638 2023-08-08 01:56:59.000000 krdict_py-3.0.1/src/krdict/types/enums/semantic_category.py
+-rw-rw-rw-   0        0        0    14139 2023-08-08 01:57:02.000000 krdict_py-3.0.1/src/krdict/types/enums/subject_category.py
+-rw-rw-rw-   0        0        0      814 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/types/exceptions.py
+-rw-rw-rw-   0        0        0      100 2021-12-05 21:04:38.000000 krdict_py-3.0.1/src/krdict/types/exceptions.pyi
+-rw-rw-rw-   0        0        0    13016 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/types/main.py
+-rw-rw-rw-   0        0        0    12983 2022-10-28 01:49:54.000000 krdict_py-3.0.1/src/krdict/types/scraper.py
+drwxrwxrwx   0        0        0        0 2024-06-02 17:19:12.692931 krdict_py-3.0.1/src/krdict.py.egg-info/
+-rw-rw-rw-   0        0        0     2410 2024-06-02 17:19:12.000000 krdict_py-3.0.1/src/krdict.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2024-06-02 17:19:12.000000 krdict_py-3.0.1/src/krdict.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 17:19:12.000000 krdict_py-3.0.1/src/krdict.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-02 17:19:12.000000 krdict_py-3.0.1/src/krdict.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2022-09-19 23:20:26.000000 krdict_py-3.0.1/src/py.typed
```

### Comparing `krdict.py-3.0.0/LICENSE` & `krdict_py-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/PKG-INFO` & `krdict_py-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: krdict.py
-Version: 3.0.0
+Version: 3.0.1
 Summary: A package that helps with querying the Korean Learners' Dictionary API.
 Home-page: https://github.com/omarkmu/krdict.py#readme
 Author: Omar M.
 Author-email: omarkmu@gmail.com
 Project-URL: Source Code, https://github.com/omarkmu/krdict.py
 Project-URL: Bug Tracker, https://github.com/omarkmu/krdict.py/issues
-Project-URL: Documentation, https://krdictpy.readthedocs.io/en/v3.0.0
+Project-URL: Documentation, https://krdictpy.readthedocs.io/en/v3.0.1
 Keywords: korean dictionary api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `krdict.py-3.0.0/PYPI_README.md` & `krdict_py-3.0.1/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/README.md` & `krdict_py-3.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # krdict.py
 
 [![PyPI](https://img.shields.io/pypi/v/krdict.py)](https://pypi.org/project/krdict.py)
 [![Documentation](https://img.shields.io/readthedocs/krdictpy/stable)](https://krdictpy.readthedocs.io/en/stable)
-[![Tests](https://img.shields.io/github/workflow/status/omarkmu/krdict.py/Test?label=tests)](https://github.com/omarkmu/krdict.py/actions/workflows/test.yml)  
+[![Tests](https://img.shields.io/github/actions/workflow/status/omarkmu/krdict.py/test.yml?branch=main&label=tests)](https://github.com/omarkmu/krdict.py/actions/workflows/test.yml)  
 [![krdict.js](https://img.shields.io/npm/v/krdict.js?label=krdict.js)](https://github.com/Fox-Islam/krdict.js)
 
 A python package that helps to query the [API](https://krdict.korean.go.kr/openApi/openApiInfo) of the
 [Korean Learners' Dictionary](https://krdict.korean.go.kr/mainAction), provided by the National Institute of Korean Language.
 
 ## Installation
```

### Comparing `krdict.py-3.0.0/setup.cfg` & `krdict_py-3.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 7264 6963 742e 7079 0d0a 7665   = krdict.py..ve
-00000020: 7273 696f 6e20 3d20 332e 302e 300d 0a61  rsion = 3.0.0..a
+00000020: 7273 696f 6e20 3d20 332e 302e 310d 0a61  rsion = 3.0.1..a
 00000030: 7574 686f 7220 3d20 4f6d 6172 204d 2e0d  uthor = Omar M..
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6f6d 6172 6b6d 7540 676d 6169 6c2e 636f  omarkmu@gmail.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2041 2070 6163 6b61 6765 2074 6861 7420   A package that 
 00000080: 6865 6c70 7320 7769 7468 2071 7565 7279  helps with query
 00000090: 696e 6720 7468 6520 4b6f 7265 616e 204c  ing the Korean L
@@ -28,15 +28,15 @@
 000001b0: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
 000001c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
 000001d0: 6d61 726b 6d75 2f6b 7264 6963 742e 7079  markmu/krdict.py
 000001e0: 2f69 7373 7565 730d 0a09 446f 6375 6d65  /issues...Docume
 000001f0: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
 00000200: 2f2f 6b72 6469 6374 7079 2e72 6561 6474  //krdictpy.readt
 00000210: 6865 646f 6373 2e69 6f2f 656e 2f76 332e  hedocs.io/en/v3.
-00000220: 302e 300d 0a63 6c61 7373 6966 6965 7273  0.0..classifiers
+00000220: 302e 310d 0a63 6c61 7373 6966 6965 7273  0.1..classifiers
 00000230: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
 00000240: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
 00000250: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
 00000260: 650d 0a09 5072 6f67 7261 6d6d 696e 6720  e...Programming 
 00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000280: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
 00000290: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
```

### Comparing `krdict.py-3.0.0/src/krdict/__init__.py` & `krdict_py-3.0.1/src/krdict/__init__.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/main.py` & `krdict_py-3.0.1/src/krdict/main.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/main.pyi` & `krdict_py-3.0.1/src/krdict/main.pyi`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/request.py` & `krdict_py-3.0.1/src/krdict/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         'type': SubjectCategory
     },
     'target_code': {
         'name': 'q'
     }
 }
 _DEFAULTS = { 'API_KEY': '' }
-_PEM_PATH = path.join(path.dirname(path.realpath(__file__)), 'korean-go-kr-chain.pem')
 
 
 def _map_value(mapper, value):
     if isiterable(value, exclude=(str,)):
         return ','.join(map(lambda x: _map_value(mapper, x), value))
 
     if 'type' in mapper:
@@ -144,15 +143,15 @@
     url = _VIEW_URL if search_type == 'view' else _SEARCH_URL
 
     params = _transform_params(kwargs, search_type)
     if advanced:
         params['advanced'] = 'y'
 
     try:
-        response = requests.get(url, params, verify=_PEM_PATH)
+        response = requests.get(url, params)
         response.raise_for_status()
         return (response, params, search_type)
     except requests.exceptions.RequestException as exc:
         raise exc
 
 def set_key(key):
     """
```

### Comparing `krdict.py-3.0.0/src/krdict/response.py` & `krdict_py-3.0.1/src/krdict/response.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/scraper/__init__.py` & `krdict_py-3.0.1/src/krdict/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/scraper/constants.py` & `krdict_py-3.0.1/src/krdict/scraper/constants.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/scraper/main.py` & `krdict_py-3.0.1/src/krdict/scraper/main.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/scraper/main.pyi` & `krdict_py-3.0.1/src/krdict/scraper/main.pyi`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/scraper/request.py` & `krdict_py-3.0.1/src/krdict/scraper/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Handles making requests to the dictionary website.
 """
 
-from os import path
 import requests
 from lxml import html
 from .constants import _VIEW_URL
 from ..types import (
     isiterable,
     Classification,
     SemanticCategory,
@@ -25,38 +24,38 @@
 
 _ADVANCED_SEARCH_URL = (
     'https://krdict.korean.go.kr{}/dicSearchDetail/searchDetailWordsResult?'
     '{}searchFlag=Y&syllablePosition={}'
 )
 _BASE_URL = 'https://krdict.korean.go.kr{}/mainAction'
 _CAT_MEANING_URL = (
-    'https://krdict.korean.go.kr{}/dicSearchDetail/searchDetailSenseCategoryResult?'
+    'https://krdict.korean.go.kr{}/dicSearch/searchDetailSenseCategory?'
     '{}searchFlag=Y&currentPage={}&blockCount={}&sort={}{}'
 )
 _CAT_SUBJECT_URL = (
-    'https://krdict.korean.go.kr{}/dicSearchDetail/searchDetailActCategoryResult?'
+    'https://krdict.korean.go.kr{}/dicSearch/searchDetailActCategory?'
     '{}searchFlag=Y&currentPage={}&blockCount={}&sort={}{}'
 )
 _DEFAULT_ADVANCED_CONDITION = (
     '&searchOp=AND&searchTarget=word&searchOrglanguage=all&wordCondition=wordAll&query='
 )
 _SEARCH_URL = (
-    'https://krdict.korean.go.kr{}/dicSearch/search?'
+    'https://krdict.korean.go.kr{}/dicMarinerSearch/search?'
     '{}mainSearchWord={}&currentPage={}&blockCount={}&sort={}&searchType={}'
 )
 _SEARCH_REQUEST_URL = (
-    'https://krdict.korean.go.kr{}/smallDic/searchResult?'
-    '{}mainSearchWord={}&currentPage={}&blockCount={}&sort={}&searchType={}'
+    'https://krdict.korean.go.kr{}/dicMarinerSearch/search?'
+    '{}mainSearchWord={}&currentPage={}&blockCount={}&sort={}&searchType={}&isSmallDic=Y'
 )
 _IMAGE_URL = (
-    'https://krdict.korean.go.kr/dicSearch/viewImageConfirm?'
+    'https://krdict.korean.go.kr/kor/dicSearch/viewImageConfirm?'
     'searchKindValue=image&ParaWordNo={}&ParaSenseSeq={}&multiMediaSeq={}'
 )
 _VIDEO_URL = (
-    'https://krdict.korean.go.kr/dicSearch/viewMovieConfirm?'
+    'https://krdict.korean.go.kr/kor/dicSearch/viewMovieConfirm?'
     'searchKindValue=video&ParaWordNo={}&ParaSenseSeq={}&multiMediaSeq={}'
 )
 
 _LANG_INFO = (
     ('all', None, None),
     ('eng', 6, '영어'),
     ('jpn', 7, '일본어'),
@@ -172,16 +171,16 @@
     'per_page': {
         'name': 'blockCount'
     },
     'sort': {
         'name': 'sort',
         'type': SortMethod,
         'value': {
-            'dict': 'W',
-            'popular': 'C'
+            'dict': '2',
+            'popular': '1'
         }
     },
     'classification': {
         'name': 'gubun',
         'type': Classification,
         'default': 'all',
         'value': {
@@ -537,16 +536,14 @@
 _SEARCH_TYPE_MAP = {
     'word': 'W',
     'exam': 'E',
     'dfn': 'S',
     'ip': 'P'
 }
 
-_PEM_PATH = path.join(path.dirname(path.realpath(__file__)), path.pardir, 'korean-go-kr-chain.pem')
-
 def _get_advanced_param(adv_mapper, value):
     if adv_mapper.get('name') != 'query' and ',' in value:
         params = []
 
         for val in value.split(','):
             param = _get_advanced_param(adv_mapper, val)
             if val is None:
@@ -651,15 +648,15 @@
         query.append(conditions)
     else:
         query.append(_DEFAULT_ADVANCED_CONDITION)
 
     query = ''.join(query)
     return (
         _ADVANCED_SEARCH_URL.format(*get_language_query(nation, code), query),
-        _ADVANCED_SEARCH_URL.format('', '', query)
+        _ADVANCED_SEARCH_URL.format('/kor', '', query)
     )
 
 def _build_search_url(kwargs, lang_info, search_type):
     nation, code, _ = lang_info
 
     query = kwargs.get('query')
     page = kwargs.get('page', 1)
@@ -675,15 +672,15 @@
         query,
         page,
         per_page,
         sort,
         search_type
     )
     url_kr = _SEARCH_URL.format(
-        '',
+        '/kor',
         '',
         query,
         page,
         per_page,
         sort,
         search_type
     )
@@ -739,26 +736,26 @@
 
     is_semantic = response_type == 'semantic_category'
     query_builder = (
         _build_sense_category_query if is_semantic else _build_subject_category_query
     )
 
     base_url = _CAT_MEANING_URL if is_semantic else _CAT_SUBJECT_URL
-    sort = 'C' if SortMethod.get_value(kwargs.get('sort')) == 'popular' else 'W'
+    sort = '2' if SortMethod.get_value(kwargs.get('sort')) == 'popular' else '1'
     category_query = query_builder(kwargs.get('category', 0))
 
     url = base_url.format(
         *get_language_query(nation, code),
         page,
         per_page,
         sort,
         category_query
     )
 
-    url_kr = base_url.format('', '', page, per_page, sort, category_query)
+    url_kr = base_url.format('/kor', '', page, per_page, sort, category_query)
     return url, url_kr
 
 def _build_translation_language_info(trans_lang, kwargs, response_type):
     trans_language_info = []
     trans_urls = []
 
     info = get_language_info(trans_lang)
@@ -826,23 +823,22 @@
         url, url_kr = _build_advanced_search_url(kwargs, lang_info)
 
     elif response_type == 'view':
         nation, code, _ = lang_info
         target_code = kwargs.get('target_code')
         lang_query = get_language_query(nation, code)
 
-        url_kr = _VIEW_URL.format('', '', target_code)
+        url_kr = _VIEW_URL.format('/kor', '', target_code)
         url = _VIEW_URL.format(*lang_query, target_code)
-        req_url = url
 
     elif response_type == 'word_of_the_day':
         nation, *_ = lang_info
 
-        url_kr = _BASE_URL.format('')
-        url = _BASE_URL.format(f'/{nation}' if nation else '')
+        url_kr = _BASE_URL.format('/kor')
+        url = _BASE_URL.format(f'/{nation}' if nation else '/kor')
 
     elif response_type in ('word', 'exam', 'dfn', 'ip'):
         url, url_kr, req_url = _build_search_url(kwargs, lang_info, response_type)
 
     elif response_type in ('semantic_category', 'subject_category'):
         url, url_kr = _build_category_url(kwargs, lang_info, response_type)
 
@@ -865,26 +861,26 @@
 
 def get_language_query(nation, code):
     """
     Returns query strings given a nation and nation code.
     """
 
     if not nation:
-        return '', ''
+        return '/kor', ''
 
     return f'/{nation}', f'nation={nation}&nationCode={code}&'
 
 def send_scrape_request(url):
     """
     Sends a request to a URL with the necessary headers for scraping,
     and returns an lxml node.
     """
 
     try:
-        response = requests.get(url, headers={'Accept-Language': '*'}, verify=_PEM_PATH)
+        response = requests.get(url, headers={'Accept-Language': '*'})
         response.raise_for_status()
         return html.fromstring(response.text)
     except requests.exceptions.RequestException as exc:
         raise exc
 
 def send_request(kwargs, response_type):
     """
@@ -929,12 +925,12 @@
     url = (_IMAGE_URL if media_type in (1, 2) else _VIDEO_URL).format(
         kwargs.get('target_code'),
         kwargs.get('definition_order'),
         kwargs.get('media_order')
     )
 
     try:
-        response = requests.get(url, headers={'Accept-Language': '*'}, verify=_PEM_PATH)
+        response = requests.get(url, headers={'Accept-Language': '*'})
         response.raise_for_status()
         return html.fromstring(response.text)
     except requests.exceptions.RequestException as exc:
         raise exc
```

### Comparing `krdict.py-3.0.0/src/krdict/scraper/response.py` & `krdict_py-3.0.1/src/krdict/scraper/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     })
 
 def _get_base_result(a_elem, word_text, lang_info):
     target_code = int(_extract_href(a_elem) or 0)
     result = {
         'target_code': target_code,
         'word': word_text,
-        'link': _VIEW_URL.format('', '', target_code)
+        'link': _VIEW_URL.format('/kor', '', target_code)
     }
 
     if lang_info[0]:
         _add_trans_link(result, lang_info)
 
     return result
 
@@ -306,15 +306,15 @@
         dfn_idx = 0 if not nation or len(dd_elems) < 3 else 1
         result = {
             'target_code': int(_extract_href(word_elem) or 0),
             'word': strong_elem.text.strip(),
             'definition': dd_elems[dfn_idx].text_content().strip()
         }
 
-        result['link'] = _VIEW_URL.format('', '', result['target_code'])
+        result['link'] = _VIEW_URL.format('/kor', '', result['target_code'])
         result['sup_no'] = int(sup_elems[0].text_content() or 0 if len(sup_elems) > 0 else 0)
 
     if nation:
         _add_trans_link(result, lang_info)
 
     _read_wotd_details(
         result,
@@ -431,15 +431,15 @@
                 continue
 
             target_code = int(_extract_href(elem) or 0)
             if target_code != 0:
                 obj = {
                     'word': (elem.text or '').strip(),
                     'link_target_code': target_code,
-                    'link': _VIEW_URL.format('', '', target_code),
+                    'link': _VIEW_URL.format('/kor', '', target_code),
                     'trans_link': [{
                         'url': _VIEW_URL.format(
                             *get_language_query(*lang_info[:2]),
                             target_code
                         ),
                         'language': lang_info[2]
                     }] if lang_info[0] is not None else [],
@@ -729,15 +729,15 @@
 
     word_info['subword_info'] = subword_info
 
 def _read_search_results(doc, response_type, lang_info, results=None):
     is_translation = results is not None
     results = results or []
     search_results = doc.cssselect('div.search_result > dl')
-    total_text = doc.cssselect('.search_tit > em')
+    total_text = doc.cssselect('.search_tit > span')
 
     trans_order = 0
     for result_elem in search_results:
         dt_elem = result_elem.cssselect('dt')
         dd_elem = result_elem.cssselect('dd')
 
         if len(dt_elem) == 0 or len(dd_elem) == 0:
@@ -767,15 +767,15 @@
 
     total = _extract_digits(total_text[0].text) if len(total_text) > 0 else 0
     return results, total
 
 def _read_examples(doc, lang_info):
     results = []
     search_results = doc.cssselect('div.search_result > ul > li > a')
-    total_text = doc.cssselect('span.search_tit > em')
+    total_text = doc.cssselect('span.search_tit > span')
 
     for result_elem in search_results:
         text = result_elem.text_content().strip()
         sup_elem = result_elem.cssselect('sup')
 
         if len(text) == 0:
             continue
```

### Comparing `krdict.py-3.0.0/src/krdict/types/__init__.py` & `krdict_py-3.0.1/src/krdict/types/__init__.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/enums/__init__.py` & `krdict_py-3.0.1/src/krdict/types/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/enums/base.py` & `krdict_py-3.0.1/src/krdict/types/enums/base.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/enums/base.pyi` & `krdict_py-3.0.1/src/krdict/types/enums/base.pyi`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/enums/semantic_category.py` & `krdict_py-3.0.1/src/krdict/types/enums/semantic_category.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/enums/subject_category.py` & `krdict_py-3.0.1/src/krdict/types/enums/subject_category.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/exceptions.py` & `krdict_py-3.0.1/src/krdict/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/main.py` & `krdict_py-3.0.1/src/krdict/types/main.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict/types/scraper.py` & `krdict_py-3.0.1/src/krdict/types/scraper.py`

 * *Files identical despite different names*

### Comparing `krdict.py-3.0.0/src/krdict.py.egg-info/PKG-INFO` & `krdict_py-3.0.1/src/krdict.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: krdict.py
-Version: 3.0.0
+Version: 3.0.1
 Summary: A package that helps with querying the Korean Learners' Dictionary API.
 Home-page: https://github.com/omarkmu/krdict.py#readme
 Author: Omar M.
 Author-email: omarkmu@gmail.com
 Project-URL: Source Code, https://github.com/omarkmu/krdict.py
 Project-URL: Bug Tracker, https://github.com/omarkmu/krdict.py/issues
-Project-URL: Documentation, https://krdictpy.readthedocs.io/en/v3.0.0
+Project-URL: Documentation, https://krdictpy.readthedocs.io/en/v3.0.1
 Keywords: korean dictionary api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `krdict.py-3.0.0/src/krdict.py.egg-info/SOURCES.txt` & `krdict_py-3.0.1/src/krdict.py.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 PYPI_README.md
 README.md
 setup.cfg
 setup.py
 src/py.typed
 src/krdict/__init__.py
-src/krdict/korean-go-kr-chain.pem
 src/krdict/main.py
 src/krdict/main.pyi
 src/krdict/request.py
 src/krdict/request.pyi
 src/krdict/response.py
 src/krdict/response.pyi
 src/krdict.py.egg-info/PKG-INFO
```

