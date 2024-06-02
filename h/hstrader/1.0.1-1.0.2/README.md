# Comparing `tmp/hstrader-1.0.1.tar.gz` & `tmp/hstrader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstrader-1.0.1.tar", max compression
+gzip compressed data, was "hstrader-1.0.2.tar", max compression
```

## Comparing `hstrader-1.0.1.tar` & `hstrader-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2463 2024-06-02 07:36:55.729379 hstrader-1.0.1/README.md
--rw-r--r--   0        0        0       81 2024-05-28 08:57:47.758220 hstrader-1.0.1/hstrader/__init__.py
--rw-r--r--   0        0        0       37 2024-05-28 08:57:47.762220 hstrader-1.0.1/hstrader/config/__init__.py
--rw-r--r--   0        0        0     2772 2024-05-28 08:57:47.762220 hstrader-1.0.1/hstrader/config/config.py
--rw-r--r--   0        0        0       62 2024-05-28 08:57:47.766220 hstrader-1.0.1/hstrader/helpers/__init__.py
--rw-r--r--   0        0        0     6566 2024-05-28 08:57:47.766220 hstrader-1.0.1/hstrader/helpers/http.py
--rw-r--r--   0        0        0      359 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/helpers/user_agent.py
--rw-r--r--   0        0        0     6007 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/helpers/ws.py
--rw-r--r--   0        0        0      218 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/hstrader/__init__.py
--rw-r--r--   0        0        0     3175 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/hstrader/hstrader.py
--rw-r--r--   0        0        0      243 2024-05-28 08:57:47.774220 hstrader-1.0.1/hstrader/models/__init__.py
--rw-r--r--   0        0        0     2015 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/account.py
--rw-r--r--   0        0        0      318 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/auth.py
--rw-r--r--   0        0        0      154 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/base.py
--rw-r--r--   0        0        0      764 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/base_response.py
--rw-r--r--   0        0        0     1182 2024-06-02 07:43:18.430213 hstrader-1.0.1/hstrader/models/deal.py
--rw-r--r--   0        0        0     3311 2024-06-02 07:44:04.426313 hstrader-1.0.1/hstrader/models/enums.py
--rw-r--r--   0        0        0      980 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/events.py
--rw-r--r--   0        0        0      229 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/market.py
--rw-r--r--   0        0        0     4212 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/order.py
--rw-r--r--   0        0        0     1894 2024-06-02 08:00:30.248551 hstrader-1.0.1/hstrader/models/position.py
--rw-r--r--   0        0        0     2068 2024-06-02 07:44:06.382317 hstrader-1.0.1/hstrader/models/symbol.py
--rw-r--r--   0        0        0      534 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/ws.py
--rw-r--r--   0        0        0      267 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/services/__init__.py
--rw-r--r--   0        0        0      597 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/account.py
--rw-r--r--   0        0        0     2597 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/auth.py
--rw-r--r--   0        0        0      646 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/deal.py
--rw-r--r--   0        0        0     2892 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/market.py
--rw-r--r--   0        0        0     2650 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/order.py
--rw-r--r--   0        0        0     2263 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/position.py
--rw-r--r--   0        0        0     1295 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/symbol.py
--rw-r--r--   0        0        0     1408 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/urls.py
--rw-r--r--   0        0        0     4218 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/utils.py
--rw-r--r--   0        0        0    11700 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/ws.py
--rw-r--r--   0        0        0      375 2024-06-02 08:02:35.116705 hstrader-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 hstrader-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2529 2024-06-02 08:05:54.221123 hstrader-1.0.2/README.md
+-rw-r--r--   0        0        0       81 2024-05-28 08:57:47.758220 hstrader-1.0.2/hstrader/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-28 08:57:47.762220 hstrader-1.0.2/hstrader/config/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-28 08:57:47.762220 hstrader-1.0.2/hstrader/config/config.py
+-rw-r--r--   0        0        0       62 2024-05-28 08:57:47.766220 hstrader-1.0.2/hstrader/helpers/__init__.py
+-rw-r--r--   0        0        0     6566 2024-05-28 08:57:47.766220 hstrader-1.0.2/hstrader/helpers/http.py
+-rw-r--r--   0        0        0      359 2024-05-28 08:57:47.770220 hstrader-1.0.2/hstrader/helpers/user_agent.py
+-rw-r--r--   0        0        0     6007 2024-05-28 08:57:47.770220 hstrader-1.0.2/hstrader/helpers/ws.py
+-rw-r--r--   0        0        0      218 2024-05-28 08:57:47.770220 hstrader-1.0.2/hstrader/hstrader/__init__.py
+-rw-r--r--   0        0        0     3175 2024-05-28 08:57:47.770220 hstrader-1.0.2/hstrader/hstrader/hstrader.py
+-rw-r--r--   0        0        0      243 2024-05-28 08:57:47.774220 hstrader-1.0.2/hstrader/models/__init__.py
+-rw-r--r--   0        0        0     2015 2024-05-28 08:57:47.782220 hstrader-1.0.2/hstrader/models/account.py
+-rw-r--r--   0        0        0      318 2024-05-28 08:57:47.782220 hstrader-1.0.2/hstrader/models/auth.py
+-rw-r--r--   0        0        0      154 2024-05-28 08:57:47.782220 hstrader-1.0.2/hstrader/models/base.py
+-rw-r--r--   0        0        0      764 2024-05-28 08:57:47.782220 hstrader-1.0.2/hstrader/models/base_response.py
+-rw-r--r--   0        0        0     1182 2024-06-02 07:43:18.430213 hstrader-1.0.2/hstrader/models/deal.py
+-rw-r--r--   0        0        0     3311 2024-06-02 07:44:04.426313 hstrader-1.0.2/hstrader/models/enums.py
+-rw-r--r--   0        0        0      980 2024-05-28 08:57:47.786220 hstrader-1.0.2/hstrader/models/events.py
+-rw-r--r--   0        0        0      229 2024-05-28 08:57:47.786220 hstrader-1.0.2/hstrader/models/market.py
+-rw-r--r--   0        0        0     4383 2024-06-02 08:09:14.357725 hstrader-1.0.2/hstrader/models/order.py
+-rw-r--r--   0        0        0     1894 2024-06-02 08:00:30.248551 hstrader-1.0.2/hstrader/models/position.py
+-rw-r--r--   0        0        0     2068 2024-06-02 07:44:06.382317 hstrader-1.0.2/hstrader/models/symbol.py
+-rw-r--r--   0        0        0      534 2024-05-28 08:57:47.786220 hstrader-1.0.2/hstrader/models/ws.py
+-rw-r--r--   0        0        0      267 2024-05-28 08:57:47.786220 hstrader-1.0.2/hstrader/services/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-28 08:57:47.794220 hstrader-1.0.2/hstrader/services/account.py
+-rw-r--r--   0        0        0     2597 2024-05-28 08:57:47.794220 hstrader-1.0.2/hstrader/services/auth.py
+-rw-r--r--   0        0        0      646 2024-05-28 08:57:47.794220 hstrader-1.0.2/hstrader/services/deal.py
+-rw-r--r--   0        0        0     2892 2024-05-28 08:57:47.794220 hstrader-1.0.2/hstrader/services/market.py
+-rw-r--r--   0        0        0     2650 2024-05-28 08:57:47.794220 hstrader-1.0.2/hstrader/services/order.py
+-rw-r--r--   0        0        0     2263 2024-05-28 08:57:47.798220 hstrader-1.0.2/hstrader/services/position.py
+-rw-r--r--   0        0        0     1295 2024-05-28 08:57:47.798220 hstrader-1.0.2/hstrader/services/symbol.py
+-rw-r--r--   0        0        0     1408 2024-05-28 08:57:47.798220 hstrader-1.0.2/hstrader/services/urls.py
+-rw-r--r--   0        0        0     4218 2024-05-28 08:57:47.798220 hstrader-1.0.2/hstrader/services/utils.py
+-rw-r--r--   0        0        0    11700 2024-05-28 08:57:47.798220 hstrader-1.0.2/hstrader/services/ws.py
+-rw-r--r--   0        0        0      398 2024-06-02 08:09:30.989779 hstrader-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 hstrader-1.0.2/PKG-INFO
```

### Comparing `hstrader-1.0.1/README.md` & `hstrader-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -85,13 +85,13 @@
 
 # Start listening to real-time data
 client.start()
 
 
 ```
 
-For more examples, please refer to the [examples](/examples/) directory.
+For more examples, please refer to the [examples]([/examples/](https://github.com/hstrader/hstrader-sdk-py/tree/main/examples)) directory.
 ## Contributing
 
 Contributions are welcome.<br/>
 If you've found a bug within this project, please open an issue to discuss what you would like to change.<br/>
 If it's an issue with the API, please open a topic at [Contact Us]().
```

### Comparing `hstrader-1.0.1/hstrader/config/config.py` & `hstrader-1.0.2/hstrader/config/config.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/helpers/http.py` & `hstrader-1.0.2/hstrader/helpers/http.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/helpers/ws.py` & `hstrader-1.0.2/hstrader/helpers/ws.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/hstrader/hstrader.py` & `hstrader-1.0.2/hstrader/hstrader/hstrader.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/account.py` & `hstrader-1.0.2/hstrader/models/account.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/base_response.py` & `hstrader-1.0.2/hstrader/models/base_response.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/deal.py` & `hstrader-1.0.2/hstrader/models/deal.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/enums.py` & `hstrader-1.0.2/hstrader/models/enums.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/events.py` & `hstrader-1.0.2/hstrader/models/events.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/order.py` & `hstrader-1.0.2/hstrader/models/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 from .base import BaseModel
-from .enums import *
+from .enums import (
+    ApproveStatus,
+    ChannelType,
+    DirectionType,
+    ExpirationPolicy,
+    FillPolicy,
+    FillType,
+    OrderStatus,
+    OrderType,
+    ReasonType,
+    SideType,
+)
 from .position import Position
 from .symbol import Symbol
 from typing import Union
 
 
 class Order(BaseModel):
```

### Comparing `hstrader-1.0.1/hstrader/models/position.py` & `hstrader-1.0.2/hstrader/models/position.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/symbol.py` & `hstrader-1.0.2/hstrader/models/symbol.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/models/ws.py` & `hstrader-1.0.2/hstrader/models/ws.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/account.py` & `hstrader-1.0.2/hstrader/services/account.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/auth.py` & `hstrader-1.0.2/hstrader/services/auth.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/deal.py` & `hstrader-1.0.2/hstrader/services/deal.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/market.py` & `hstrader-1.0.2/hstrader/services/market.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/order.py` & `hstrader-1.0.2/hstrader/services/order.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/position.py` & `hstrader-1.0.2/hstrader/services/position.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/symbol.py` & `hstrader-1.0.2/hstrader/services/symbol.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/urls.py` & `hstrader-1.0.2/hstrader/services/urls.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/utils.py` & `hstrader-1.0.2/hstrader/services/utils.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/hstrader/services/ws.py` & `hstrader-1.0.2/hstrader/services/ws.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.1/PKG-INFO` & `hstrader-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: hstrader
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
+License: Apache-2.0
 Author: Hybrid Solutions
 Author-email: dev@hybridsolutions.com
 Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -104,14 +106,14 @@
 
 # Start listening to real-time data
 client.start()
 
 
 ```
 
-For more examples, please refer to the [examples](/examples/) directory.
+For more examples, please refer to the [examples]([/examples/](https://github.com/hstrader/hstrader-sdk-py/tree/main/examples)) directory.
 ## Contributing
 
 Contributions are welcome.<br/>
 If you've found a bug within this project, please open an issue to discuss what you would like to change.<br/>
 If it's an issue with the API, please open a topic at [Contact Us]().
```

