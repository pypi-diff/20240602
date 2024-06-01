# Comparing `tmp/wetrade-0.1.1.tar.gz` & `tmp/wetrade-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wetrade-0.1.1.tar", last modified: Tue May 21 22:10:37 2024, max compression
+gzip compressed data, was "wetrade-0.1.2.tar", last modified: Sat Jun  1 22:01:35 2024, max compression
```

## Comparing `wetrade-0.1.1.tar` & `wetrade-0.1.2.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/
--rw-r--r--   0 mason     (1000) mason     (1000)     1089 2024-05-17 18:51:50.000000 wetrade-0.1.1/LICENSE
--rw-r--r--   0 mason     (1000) mason     (1000)       44 2024-05-17 18:51:50.000000 wetrade-0.1.1/MANIFEST.in
--rw-r--r--   0 mason     (1000) mason     (1000)     5414 2024-05-21 22:10:37.785747 wetrade-0.1.1/PKG-INFO
--rw-r--r--   0 mason     (1000) mason     (1000)     4956 2024-05-21 22:07:33.000000 wetrade-0.1.1/README.rst
--rw-r--r--   0 mason     (1000) mason     (1000)       38 2024-05-21 22:10:37.785747 wetrade-0.1.1/setup.cfg
--rw-r--r--   0 mason     (1000) mason     (1000)      607 2024-05-21 22:10:33.000000 wetrade-0.1.1/setup.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/__init__.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/mock_api/
--rw-r--r--   0 mason     (1000) mason     (1000)       68 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)    17447 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/account_responses.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2272 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/mock_api.py
--rw-r--r--   0 mason     (1000) mason     (1000)     6888 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/order_responses.py
--rw-r--r--   0 mason     (1000) mason     (1000)     1786 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/mock_api/quote_responses.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/order/
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/order/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2034 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/order/test_base_order.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/tests/quote/
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/quote/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)      281 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/quote/test_data_frame_quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/quote/test_quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.1/tests/test_account.py
--rw-r--r--   0 mason     (1000) mason     (1000)     8049 2024-05-21 22:07:33.000000 wetrade-0.1.1/tests/test_api.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/
--rw-r--r--   0 mason     (1000) mason     (1000)      126 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)      223 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/__main__.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2303 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/account.py
--rw-r--r--   0 mason     (1000) mason     (1000)     8927 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/api.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/order/
--rw-r--r--   0 mason     (1000) mason     (1000)      292 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/order/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)    12601 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/order/base_order.py
--rw-r--r--   0 mason     (1000) mason     (1000)     1091 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/order/basic_order_types.py
--rw-r--r--   0 mason     (1000) mason     (1000)     3021 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/order/converting_stop_order.py
--rw-r--r--   0 mason     (1000) mason     (1000)     2139 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/order/lookup_msg.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/project_template/
--rw-r--r--   0 mason     (1000) mason     (1000)      271 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/project_template/Dockerfile
--rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/project_template/__init__.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/project_template/__pycache__/
--rw-r--r--   0 mason     (1000) mason     (1000)      187 2024-05-21 22:10:27.000000 wetrade-0.1.1/wetrade/project_template/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 mason     (1000) mason     (1000)      741 2024-05-21 22:10:27.000000 wetrade-0.1.1/wetrade/project_template/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 mason     (1000) mason     (1000)     1209 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/project_template/main.py
--rw-r--r--   0 mason     (1000) mason     (1000)      362 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/project_template/new_project.py
--rw-r--r--   0 mason     (1000) mason     (1000)        7 2024-05-17 18:51:50.000000 wetrade-0.1.1/wetrade/project_template/requirements.txt
--rw-r--r--   0 mason     (1000) mason     (1000)      827 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/project_template/settings.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade/quote/
--rw-r--r--   0 mason     (1000) mason     (1000)      165 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/__init__.py
--rw-r--r--   0 mason     (1000) mason     (1000)     4151 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/data_frame_quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)     5138 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/multi_quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)     4682 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/quote/quote.py
--rw-r--r--   0 mason     (1000) mason     (1000)     8299 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/user_session.py
--rw-r--r--   0 mason     (1000) mason     (1000)     3689 2024-05-21 22:07:33.000000 wetrade-0.1.1/wetrade/utils.py
-drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-05-21 22:10:37.785747 wetrade-0.1.1/wetrade.egg-info/
--rw-r--r--   0 mason     (1000) mason     (1000)     5414 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/PKG-INFO
--rw-r--r--   0 mason     (1000) mason     (1000)     1283 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/SOURCES.txt
--rw-r--r--   0 mason     (1000) mason     (1000)        1 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/dependency_links.txt
--rw-r--r--   0 mason     (1000) mason     (1000)      123 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/requires.txt
--rw-r--r--   0 mason     (1000) mason     (1000)       14 2024-05-21 22:10:37.000000 wetrade-0.1.1/wetrade.egg-info/top_level.txt
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/
+-rw-r--r--   0 mason     (1000) mason     (1000)     1089 2024-05-17 18:51:50.000000 wetrade-0.1.2/LICENSE
+-rw-r--r--   0 mason     (1000) mason     (1000)       44 2024-05-17 18:51:50.000000 wetrade-0.1.2/MANIFEST.in
+-rw-r--r--   0 mason     (1000) mason     (1000)     5564 2024-06-01 22:01:35.810823 wetrade-0.1.2/PKG-INFO
+-rw-r--r--   0 mason     (1000) mason     (1000)     4975 2024-06-01 21:57:44.000000 wetrade-0.1.2/README.rst
+-rw-r--r--   0 mason     (1000) mason     (1000)       38 2024-06-01 22:01:35.810823 wetrade-0.1.2/setup.cfg
+-rw-r--r--   0 mason     (1000) mason     (1000)      721 2024-06-01 21:58:51.000000 wetrade-0.1.2/setup.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/tests/
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/__init__.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/tests/mock_api/
+-rw-r--r--   0 mason     (1000) mason     (1000)       68 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/mock_api/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)    17447 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/mock_api/account_responses.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2272 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/mock_api/mock_api.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     6888 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/mock_api/order_responses.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     1786 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/mock_api/quote_responses.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/tests/order/
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/order/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2034 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/order/test_base_order.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/tests/quote/
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/quote/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      281 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/quote/test_data_frame_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/quote/test_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      951 2024-05-17 18:51:50.000000 wetrade-0.1.2/tests/test_account.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     8049 2024-05-21 22:07:33.000000 wetrade-0.1.2/tests/test_api.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/wetrade/
+-rw-r--r--   0 mason     (1000) mason     (1000)      126 2024-05-17 18:51:50.000000 wetrade-0.1.2/wetrade/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      223 2024-05-17 18:51:50.000000 wetrade-0.1.2/wetrade/__main__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2303 2024-05-21 22:07:33.000000 wetrade-0.1.2/wetrade/account.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     8927 2024-05-21 22:07:33.000000 wetrade-0.1.2/wetrade/api.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     3302 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/market_hours.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/wetrade/order/
+-rw-r--r--   0 mason     (1000) mason     (1000)      292 2024-05-17 18:51:50.000000 wetrade-0.1.2/wetrade/order/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)    12601 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/order/base_order.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     1091 2024-05-21 22:07:33.000000 wetrade-0.1.2/wetrade/order/basic_order_types.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     3021 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/order/converting_stop_order.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2141 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/order/lookup_msg.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/wetrade/project_template/
+-rw-r--r--   0 mason     (1000) mason     (1000)      271 2024-05-17 18:51:50.000000 wetrade-0.1.2/wetrade/project_template/Dockerfile
+-rw-r--r--   0 mason     (1000) mason     (1000)        0 2024-05-17 18:51:50.000000 wetrade-0.1.2/wetrade/project_template/__init__.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/wetrade/project_template/__pycache__/
+-rw-r--r--   0 mason     (1000) mason     (1000)      187 2024-05-21 22:10:27.000000 wetrade-0.1.2/wetrade/project_template/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 mason     (1000) mason     (1000)      741 2024-05-21 22:10:27.000000 wetrade-0.1.2/wetrade/project_template/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 mason     (1000) mason     (1000)     1227 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/project_template/main.py
+-rw-r--r--   0 mason     (1000) mason     (1000)      384 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/project_template/new_project.py
+-rw-r--r--   0 mason     (1000) mason     (1000)        7 2024-05-17 18:51:50.000000 wetrade-0.1.2/wetrade/project_template/requirements.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)      827 2024-05-21 22:07:33.000000 wetrade-0.1.2/wetrade/project_template/settings.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     2912 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/project_template/trading_session.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/wetrade/quote/
+-rw-r--r--   0 mason     (1000) mason     (1000)      165 2024-05-21 22:07:33.000000 wetrade-0.1.2/wetrade/quote/__init__.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     3814 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/quote/data_frame_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     4884 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/quote/multi_quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     4428 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/quote/quote.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     8707 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/user_session.py
+-rw-r--r--   0 mason     (1000) mason     (1000)     3436 2024-06-01 21:57:44.000000 wetrade-0.1.2/wetrade/utils.py
+drwxr-xr-x   0 mason     (1000) mason     (1000)        0 2024-06-01 22:01:35.810823 wetrade-0.1.2/wetrade.egg-info/
+-rw-r--r--   0 mason     (1000) mason     (1000)     5564 2024-06-01 22:01:35.000000 wetrade-0.1.2/wetrade.egg-info/PKG-INFO
+-rw-r--r--   0 mason     (1000) mason     (1000)     1351 2024-06-01 22:01:35.000000 wetrade-0.1.2/wetrade.egg-info/SOURCES.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)        1 2024-06-01 22:01:35.000000 wetrade-0.1.2/wetrade.egg-info/dependency_links.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)      180 2024-06-01 22:01:35.000000 wetrade-0.1.2/wetrade.egg-info/requires.txt
+-rw-r--r--   0 mason     (1000) mason     (1000)       14 2024-06-01 22:01:35.000000 wetrade-0.1.2/wetrade.egg-info/top_level.txt
```

### Comparing `wetrade-0.1.1/LICENSE` & `wetrade-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/PKG-INFO` & `wetrade-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: wetrade
-Version: 0.1.1
+Version: 0.1.2
 Summary: An E-Trade python library built for active stock trading
 Author: Mason Krause
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: playwright
 Requires-Dist: urllib3==1.26.16
 Requires-Dist: xmltodict
+Requires-Dist: pytz
 Requires-Dist: pyotp==2.9.0
 Requires-Dist: google-cloud-logging
 Requires-Dist: google-cloud-storage
+Requires-Dist: google-cloud-secret-manager
 Requires-Dist: polars
 Requires-Dist: pandas
 Requires-Dist: pyarrow
+Provides-Extra: dev
+Requires-Dist: sphinx_rtd_theme; extra == "dev"
 
 ``wetrade``: An E-Trade Python library built for automated stock trading 
 =========================================================================
 
 ``wetrade`` overview
 --------------------
 
@@ -91,20 +95,20 @@
 
 .. code-block:: python
 
   from wetrade.api import APIClient
   from wetrade.account import Account
   from wetrade.quote import Quote
   from wetrade.order import LimitOrder
-  from wetrade.utils import setup_logging
+  from wetrade.utils import setup_cloud_logging
 
 
   def main():
-    # Setup logging (optional) and APIClient
-    setup_logging()
+    # Setup cloud logging (optional) and APIClient
+    setup_cloud_logging()
     client = APIClient()
 
     # Check out your account
     account = Account(client=client)
     print('My Account Key: ', account.account_key)
     print('My Balance: ', account.check_balance())
 
@@ -150,12 +154,12 @@
 allows you to utilize as much or as little of the library as you'd like. Our goal 
 is to consistently add new functionality to support additional use cases. If you 
 have any comments or suggestions for new features, don't hesitate to create an 
 issue or reach out to: `wetrade.inbox@gmail.com <mailto:wetrade.inbox@gmail.com>`__.
 
 
 **Disclaimer:** *wetrade is an unofficial API library and comes with no warranty
-of any kind. It is in no way endorsed by or affiliated with E*TRADE Financial 
+of any kind. It is in no way endorsed by or affiliated with E\*TRADE Financial 
 or any associated organization. Make sure to read and understand the terms of 
 service of the underlying API before using this package. This authors accept 
 no responsibility for any damage that might stem from use of this package. 
 See the LICENSE file for more details.*
```

### Comparing `wetrade-0.1.1/README.rst` & `wetrade-0.1.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -169,142 +169,143 @@
 00000a80: 7274 2041 6363 6f75 6e74 0a20 2066 726f  rt Account.  fro
 00000a90: 6d20 7765 7472 6164 652e 7175 6f74 6520  m wetrade.quote 
 00000aa0: 696d 706f 7274 2051 756f 7465 0a20 2066  import Quote.  f
 00000ab0: 726f 6d20 7765 7472 6164 652e 6f72 6465  rom wetrade.orde
 00000ac0: 7220 696d 706f 7274 204c 696d 6974 4f72  r import LimitOr
 00000ad0: 6465 720a 2020 6672 6f6d 2077 6574 7261  der.  from wetra
 00000ae0: 6465 2e75 7469 6c73 2069 6d70 6f72 7420  de.utils import 
-00000af0: 7365 7475 705f 6c6f 6767 696e 670a 0a0a  setup_logging...
-00000b00: 2020 6465 6620 6d61 696e 2829 3a0a 2020    def main():.  
-00000b10: 2020 2320 5365 7475 7020 6c6f 6767 696e    # Setup loggin
-00000b20: 6720 286f 7074 696f 6e61 6c29 2061 6e64  g (optional) and
-00000b30: 2041 5049 436c 6965 6e74 0a20 2020 2073   APIClient.    s
-00000b40: 6574 7570 5f6c 6f67 6769 6e67 2829 0a20  etup_logging(). 
-00000b50: 2020 2063 6c69 656e 7420 3d20 4150 4943     client = APIC
-00000b60: 6c69 656e 7428 290a 0a20 2020 2023 2043  lient()..    # C
-00000b70: 6865 636b 206f 7574 2079 6f75 7220 6163  heck out your ac
-00000b80: 636f 756e 740a 2020 2020 6163 636f 756e  count.    accoun
-00000b90: 7420 3d20 4163 636f 756e 7428 636c 6965  t = Account(clie
-00000ba0: 6e74 3d63 6c69 656e 7429 0a20 2020 2070  nt=client).    p
-00000bb0: 7269 6e74 2827 4d79 2041 6363 6f75 6e74  rint('My Account
-00000bc0: 204b 6579 3a20 272c 2061 6363 6f75 6e74   Key: ', account
-00000bd0: 2e61 6363 6f75 6e74 5f6b 6579 290a 2020  .account_key).  
-00000be0: 2020 7072 696e 7428 274d 7920 4261 6c61    print('My Bala
-00000bf0: 6e63 653a 2027 2c20 6163 636f 756e 742e  nce: ', account.
-00000c00: 6368 6563 6b5f 6261 6c61 6e63 6528 2929  check_balance())
-00000c10: 0a0a 2020 2020 2320 4765 7420 6120 7374  ..    # Get a st
-00000c20: 6f63 6b20 7175 6f74 650a 2020 2020 7175  ock quote.    qu
-00000c30: 6f74 6520 3d20 5175 6f74 6528 636c 6965  ote = Quote(clie
-00000c40: 6e74 3d63 6c69 656e 742c 2073 796d 626f  nt=client, symbo
-00000c50: 6c3d 2749 424d 2729 0a20 2020 2070 7269  l='IBM').    pri
-00000c60: 6e74 2866 274c 6173 7420 7b71 756f 7465  nt(f'Last {quote
-00000c70: 2e73 796d 626f 6c7d 2051 756f 7465 2050  .symbol} Quote P
-00000c80: 7269 6365 3a20 272c 2071 756f 7465 2e67  rice: ', quote.g
-00000c90: 6574 5f6c 6173 745f 7072 6963 6528 2929  et_last_price())
-00000ca0: 0a0a 2020 2020 2320 506c 6163 6520 736f  ..    # Place so
-00000cb0: 6d65 206f 7264 6572 7320 616e 6420 7374  me orders and st
-00000cc0: 7566 660a 2020 2020 6f72 6465 7231 203d  uff.    order1 =
-00000cd0: 204c 696d 6974 4f72 6465 7228 0a20 2020   LimitOrder(.   
-00000ce0: 2020 2020 2063 6c69 656e 7420 3d20 636c       client = cl
-00000cf0: 6965 6e74 2c0a 2020 2020 2020 2020 6163  ient,.        ac
-00000d00: 636f 756e 745f 6b65 7920 3d20 6163 636f  count_key = acco
-00000d10: 756e 742e 6163 636f 756e 745f 6b65 792c  unt.account_key,
-00000d20: 0a20 2020 2020 2020 2073 796d 626f 6c20  .        symbol 
-00000d30: 3d20 274e 5644 4127 2c0a 2020 2020 2020  = 'NVDA',.      
-00000d40: 2020 6163 7469 6f6e 203d 2027 4255 5927    action = 'BUY'
-00000d50: 2c0a 2020 2020 2020 2020 7175 616e 7469  ,.        quanti
-00000d60: 7479 203d 2031 2c0a 2020 2020 2020 2020  ty = 1,.        
-00000d70: 7072 6963 6520 3d20 3530 2e30 3029 0a20  price = 50.00). 
-00000d80: 2020 206f 7264 6572 312e 706c 6163 655f     order1.place_
-00000d90: 6f72 6465 7228 290a 2020 2020 6f72 6465  order().    orde
-00000da0: 7231 2e72 756e 5f77 6865 6e5f 7374 6174  r1.run_when_stat
-00000db0: 7573 280a 2020 2020 2020 2020 2743 414e  us(.        'CAN
-00000dc0: 4345 4c4c 4544 272c 200a 2020 2020 2020  CELLED', .      
-00000dd0: 2020 6675 6e63 203d 2070 7269 6e74 2c20    func = print, 
-00000de0: 0a20 2020 2020 2020 2066 756e 635f 6172  .        func_ar
-00000df0: 6773 203d 205b 2754 6573 7420 6d65 7373  gs = ['Test mess
-00000e00: 6167 6527 5d29 0a20 2020 200a 2020 2020  age']).    .    
-00000e10: 6f72 6465 7232 203d 204c 696d 6974 4f72  order2 = LimitOr
-00000e20: 6465 7228 0a20 2020 2020 2020 2063 6c69  der(.        cli
-00000e30: 656e 7420 3d20 636c 6965 6e74 2c0a 2020  ent = client,.  
-00000e40: 2020 2020 2020 6163 636f 756e 745f 6b65        account_ke
-00000e50: 7920 3d20 6163 636f 756e 742e 6163 636f  y = account.acco
-00000e60: 756e 745f 6b65 792c 0a20 2020 2020 2020  unt_key,.       
-00000e70: 2073 796d 626f 6c20 3d20 274e 464c 5827   symbol = 'NFLX'
-00000e80: 2c0a 2020 2020 2020 2020 6163 7469 6f6e  ,.        action
-00000e90: 203d 2027 4255 5927 2c0a 2020 2020 2020   = 'BUY',.      
-00000ea0: 2020 7175 616e 7469 7479 203d 2031 2c0a    quantity = 1,.
-00000eb0: 2020 2020 2020 2020 7072 6963 6520 3d20          price = 
-00000ec0: 3530 2e30 3029 0a20 2020 206f 7264 6572  50.00).    order
-00000ed0: 322e 706c 6163 655f 6f72 6465 7228 290a  2.place_order().
-00000ee0: 2020 2020 6f72 6465 7232 2e72 756e 5f77      order2.run_w
-00000ef0: 6865 6e5f 7374 6174 7573 280a 2020 2020  hen_status(.    
-00000f00: 2020 2020 2743 414e 4345 4c4c 4544 272c      'CANCELLED',
-00000f10: 0a20 2020 2020 2020 206f 7264 6572 312e  .        order1.
-00000f20: 6361 6e63 656c 5f6f 7264 6572 290a 2020  cancel_order).  
-00000f30: 2020 0a20 2020 206f 7264 6572 322e 6361    .    order2.ca
-00000f40: 6e63 656c 5f6f 7264 6572 2829 0a0a 0a4f  ncel_order()...O
-00000f50: 7468 6572 2069 6e66 6f0a 2d2d 2d2d 2d2d  ther info.------
-00000f60: 2d2d 2d2d 2d2d 2d0a 0a60 6077 6574 7261  -------..``wetra
-00000f70: 6465 6060 2077 6173 2069 6e69 7469 616c  de`` was initial
-00000f80: 6c79 2064 6573 6967 6e65 6420 746f 2072  ly designed to r
-00000f90: 756e 2068 6561 646c 6573 736c 7920 616e  un headlessly an
-00000fa0: 6420 6861 7320 6275 696c 742d 696e 2068  d has built-in h
-00000fb0: 616e 646c 696e 6720 666f 7220 0a6d 6f73  andling for .mos
-00000fc0: 7420 6578 7065 6374 6564 2062 726f 6b65  t expected broke
-00000fd0: 7261 6765 2c20 7365 7276 6572 2c20 616e  rage, server, an
-00000fe0: 6420 4150 4920 6572 726f 7273 2e20 5468  d API errors. Th
-00000ff0: 6973 2061 6e64 2074 6865 206d 616a 6f72  is and the major
-00001000: 6974 7920 6f66 206f 7468 6572 200a 6060  ity of other .``
-00001010: 7765 7472 6164 6560 6020 6675 6e63 7469  wetrade`` functi
-00001020: 6f6e 616c 6974 7920 6973 2065 6e74 6972  onality is entir
-00001030: 656c 7920 6f70 7469 6f6e 616c 2074 6f20  ely optional to 
-00001040: 7573 652c 2061 6e64 206f 7572 206d 6f64  use, and our mod
-00001050: 756c 6172 2073 7472 7563 7475 7265 200a  ular structure .
-00001060: 616c 6c6f 7773 2079 6f75 2074 6f20 7574  allows you to ut
-00001070: 696c 697a 6520 6173 206d 7563 6820 6f72  ilize as much or
-00001080: 2061 7320 6c69 7474 6c65 206f 6620 7468   as little of th
-00001090: 6520 6c69 6272 6172 7920 6173 2079 6f75  e library as you
-000010a0: 2764 206c 696b 652e 204f 7572 2067 6f61  'd like. Our goa
-000010b0: 6c20 0a69 7320 746f 2063 6f6e 7369 7374  l .is to consist
-000010c0: 656e 746c 7920 6164 6420 6e65 7720 6675  ently add new fu
-000010d0: 6e63 7469 6f6e 616c 6974 7920 746f 2073  nctionality to s
-000010e0: 7570 706f 7274 2061 6464 6974 696f 6e61  upport additiona
-000010f0: 6c20 7573 6520 6361 7365 732e 2049 6620  l use cases. If 
-00001100: 796f 7520 0a68 6176 6520 616e 7920 636f  you .have any co
-00001110: 6d6d 656e 7473 206f 7220 7375 6767 6573  mments or sugges
-00001120: 7469 6f6e 7320 666f 7220 6e65 7720 6665  tions for new fe
-00001130: 6174 7572 6573 2c20 646f 6e27 7420 6865  atures, don't he
-00001140: 7369 7461 7465 2074 6f20 6372 6561 7465  sitate to create
-00001150: 2061 6e20 0a69 7373 7565 206f 7220 7265   an .issue or re
-00001160: 6163 6820 6f75 7420 746f 3a20 6077 6574  ach out to: `wet
-00001170: 7261 6465 2e69 6e62 6f78 4067 6d61 696c  rade.inbox@gmail
-00001180: 2e63 6f6d 203c 6d61 696c 746f 3a77 6574  .com <mailto:wet
-00001190: 7261 6465 2e69 6e62 6f78 4067 6d61 696c  rade.inbox@gmail
-000011a0: 2e63 6f6d 3e60 5f5f 2e0a 0a0a 2a2a 4469  .com>`__....**Di
-000011b0: 7363 6c61 696d 6572 3a2a 2a20 2a77 6574  sclaimer:** *wet
-000011c0: 7261 6465 2069 7320 616e 2075 6e6f 6666  rade is an unoff
-000011d0: 6963 6961 6c20 4150 4920 6c69 6272 6172  icial API librar
-000011e0: 7920 616e 6420 636f 6d65 7320 7769 7468  y and comes with
-000011f0: 206e 6f20 7761 7272 616e 7479 0a6f 6620   no warranty.of 
-00001200: 616e 7920 6b69 6e64 2e20 4974 2069 7320  any kind. It is 
-00001210: 696e 206e 6f20 7761 7920 656e 646f 7273  in no way endors
-00001220: 6564 2062 7920 6f72 2061 6666 696c 6961  ed by or affilia
-00001230: 7465 6420 7769 7468 2045 2a54 5241 4445  ted with E*TRADE
-00001240: 2046 696e 616e 6369 616c 200a 6f72 2061   Financial .or a
-00001250: 6e79 2061 7373 6f63 6961 7465 6420 6f72  ny associated or
-00001260: 6761 6e69 7a61 7469 6f6e 2e20 4d61 6b65  ganization. Make
-00001270: 2073 7572 6520 746f 2072 6561 6420 616e   sure to read an
-00001280: 6420 756e 6465 7273 7461 6e64 2074 6865  d understand the
-00001290: 2074 6572 6d73 206f 6620 0a73 6572 7669   terms of .servi
-000012a0: 6365 206f 6620 7468 6520 756e 6465 726c  ce of the underl
-000012b0: 7969 6e67 2041 5049 2062 6566 6f72 6520  ying API before 
-000012c0: 7573 696e 6720 7468 6973 2070 6163 6b61  using this packa
-000012d0: 6765 2e20 5468 6973 2061 7574 686f 7273  ge. This authors
-000012e0: 2061 6363 6570 7420 0a6e 6f20 7265 7370   accept .no resp
-000012f0: 6f6e 7369 6269 6c69 7479 2066 6f72 2061  onsibility for a
-00001300: 6e79 2064 616d 6167 6520 7468 6174 206d  ny damage that m
-00001310: 6967 6874 2073 7465 6d20 6672 6f6d 2075  ight stem from u
-00001320: 7365 206f 6620 7468 6973 2070 6163 6b61  se of this packa
-00001330: 6765 2e20 0a53 6565 2074 6865 204c 4943  ge. .See the LIC
-00001340: 454e 5345 2066 696c 6520 666f 7220 6d6f  ENSE file for mo
-00001350: 7265 2064 6574 6169 6c73 2e2a            re details.*
+00000af0: 7365 7475 705f 636c 6f75 645f 6c6f 6767  setup_cloud_logg
+00000b00: 696e 670a 0a0a 2020 6465 6620 6d61 696e  ing...  def main
+00000b10: 2829 3a0a 2020 2020 2320 5365 7475 7020  ():.    # Setup 
+00000b20: 636c 6f75 6420 6c6f 6767 696e 6720 286f  cloud logging (o
+00000b30: 7074 696f 6e61 6c29 2061 6e64 2041 5049  ptional) and API
+00000b40: 436c 6965 6e74 0a20 2020 2073 6574 7570  Client.    setup
+00000b50: 5f63 6c6f 7564 5f6c 6f67 6769 6e67 2829  _cloud_logging()
+00000b60: 0a20 2020 2063 6c69 656e 7420 3d20 4150  .    client = AP
+00000b70: 4943 6c69 656e 7428 290a 0a20 2020 2023  IClient()..    #
+00000b80: 2043 6865 636b 206f 7574 2079 6f75 7220   Check out your 
+00000b90: 6163 636f 756e 740a 2020 2020 6163 636f  account.    acco
+00000ba0: 756e 7420 3d20 4163 636f 756e 7428 636c  unt = Account(cl
+00000bb0: 6965 6e74 3d63 6c69 656e 7429 0a20 2020  ient=client).   
+00000bc0: 2070 7269 6e74 2827 4d79 2041 6363 6f75   print('My Accou
+00000bd0: 6e74 204b 6579 3a20 272c 2061 6363 6f75  nt Key: ', accou
+00000be0: 6e74 2e61 6363 6f75 6e74 5f6b 6579 290a  nt.account_key).
+00000bf0: 2020 2020 7072 696e 7428 274d 7920 4261      print('My Ba
+00000c00: 6c61 6e63 653a 2027 2c20 6163 636f 756e  lance: ', accoun
+00000c10: 742e 6368 6563 6b5f 6261 6c61 6e63 6528  t.check_balance(
+00000c20: 2929 0a0a 2020 2020 2320 4765 7420 6120  ))..    # Get a 
+00000c30: 7374 6f63 6b20 7175 6f74 650a 2020 2020  stock quote.    
+00000c40: 7175 6f74 6520 3d20 5175 6f74 6528 636c  quote = Quote(cl
+00000c50: 6965 6e74 3d63 6c69 656e 742c 2073 796d  ient=client, sym
+00000c60: 626f 6c3d 2749 424d 2729 0a20 2020 2070  bol='IBM').    p
+00000c70: 7269 6e74 2866 274c 6173 7420 7b71 756f  rint(f'Last {quo
+00000c80: 7465 2e73 796d 626f 6c7d 2051 756f 7465  te.symbol} Quote
+00000c90: 2050 7269 6365 3a20 272c 2071 756f 7465   Price: ', quote
+00000ca0: 2e67 6574 5f6c 6173 745f 7072 6963 6528  .get_last_price(
+00000cb0: 2929 0a0a 2020 2020 2320 506c 6163 6520  ))..    # Place 
+00000cc0: 736f 6d65 206f 7264 6572 7320 616e 6420  some orders and 
+00000cd0: 7374 7566 660a 2020 2020 6f72 6465 7231  stuff.    order1
+00000ce0: 203d 204c 696d 6974 4f72 6465 7228 0a20   = LimitOrder(. 
+00000cf0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+00000d00: 636c 6965 6e74 2c0a 2020 2020 2020 2020  client,.        
+00000d10: 6163 636f 756e 745f 6b65 7920 3d20 6163  account_key = ac
+00000d20: 636f 756e 742e 6163 636f 756e 745f 6b65  count.account_ke
+00000d30: 792c 0a20 2020 2020 2020 2073 796d 626f  y,.        symbo
+00000d40: 6c20 3d20 274e 5644 4127 2c0a 2020 2020  l = 'NVDA',.    
+00000d50: 2020 2020 6163 7469 6f6e 203d 2027 4255      action = 'BU
+00000d60: 5927 2c0a 2020 2020 2020 2020 7175 616e  Y',.        quan
+00000d70: 7469 7479 203d 2031 2c0a 2020 2020 2020  tity = 1,.      
+00000d80: 2020 7072 6963 6520 3d20 3530 2e30 3029    price = 50.00)
+00000d90: 0a20 2020 206f 7264 6572 312e 706c 6163  .    order1.plac
+00000da0: 655f 6f72 6465 7228 290a 2020 2020 6f72  e_order().    or
+00000db0: 6465 7231 2e72 756e 5f77 6865 6e5f 7374  der1.run_when_st
+00000dc0: 6174 7573 280a 2020 2020 2020 2020 2743  atus(.        'C
+00000dd0: 414e 4345 4c4c 4544 272c 200a 2020 2020  ANCELLED', .    
+00000de0: 2020 2020 6675 6e63 203d 2070 7269 6e74      func = print
+00000df0: 2c20 0a20 2020 2020 2020 2066 756e 635f  , .        func_
+00000e00: 6172 6773 203d 205b 2754 6573 7420 6d65  args = ['Test me
+00000e10: 7373 6167 6527 5d29 0a20 2020 200a 2020  ssage']).    .  
+00000e20: 2020 6f72 6465 7232 203d 204c 696d 6974    order2 = Limit
+00000e30: 4f72 6465 7228 0a20 2020 2020 2020 2063  Order(.        c
+00000e40: 6c69 656e 7420 3d20 636c 6965 6e74 2c0a  lient = client,.
+00000e50: 2020 2020 2020 2020 6163 636f 756e 745f          account_
+00000e60: 6b65 7920 3d20 6163 636f 756e 742e 6163  key = account.ac
+00000e70: 636f 756e 745f 6b65 792c 0a20 2020 2020  count_key,.     
+00000e80: 2020 2073 796d 626f 6c20 3d20 274e 464c     symbol = 'NFL
+00000e90: 5827 2c0a 2020 2020 2020 2020 6163 7469  X',.        acti
+00000ea0: 6f6e 203d 2027 4255 5927 2c0a 2020 2020  on = 'BUY',.    
+00000eb0: 2020 2020 7175 616e 7469 7479 203d 2031      quantity = 1
+00000ec0: 2c0a 2020 2020 2020 2020 7072 6963 6520  ,.        price 
+00000ed0: 3d20 3530 2e30 3029 0a20 2020 206f 7264  = 50.00).    ord
+00000ee0: 6572 322e 706c 6163 655f 6f72 6465 7228  er2.place_order(
+00000ef0: 290a 2020 2020 6f72 6465 7232 2e72 756e  ).    order2.run
+00000f00: 5f77 6865 6e5f 7374 6174 7573 280a 2020  _when_status(.  
+00000f10: 2020 2020 2020 2743 414e 4345 4c4c 4544        'CANCELLED
+00000f20: 272c 0a20 2020 2020 2020 206f 7264 6572  ',.        order
+00000f30: 312e 6361 6e63 656c 5f6f 7264 6572 290a  1.cancel_order).
+00000f40: 2020 2020 0a20 2020 206f 7264 6572 322e      .    order2.
+00000f50: 6361 6e63 656c 5f6f 7264 6572 2829 0a0a  cancel_order()..
+00000f60: 0a4f 7468 6572 2069 6e66 6f0a 2d2d 2d2d  .Other info.----
+00000f70: 2d2d 2d2d 2d2d 2d2d 2d0a 0a60 6077 6574  ---------..``wet
+00000f80: 7261 6465 6060 2077 6173 2069 6e69 7469  rade`` was initi
+00000f90: 616c 6c79 2064 6573 6967 6e65 6420 746f  ally designed to
+00000fa0: 2072 756e 2068 6561 646c 6573 736c 7920   run headlessly 
+00000fb0: 616e 6420 6861 7320 6275 696c 742d 696e  and has built-in
+00000fc0: 2068 616e 646c 696e 6720 666f 7220 0a6d   handling for .m
+00000fd0: 6f73 7420 6578 7065 6374 6564 2062 726f  ost expected bro
+00000fe0: 6b65 7261 6765 2c20 7365 7276 6572 2c20  kerage, server, 
+00000ff0: 616e 6420 4150 4920 6572 726f 7273 2e20  and API errors. 
+00001000: 5468 6973 2061 6e64 2074 6865 206d 616a  This and the maj
+00001010: 6f72 6974 7920 6f66 206f 7468 6572 200a  ority of other .
+00001020: 6060 7765 7472 6164 6560 6020 6675 6e63  ``wetrade`` func
+00001030: 7469 6f6e 616c 6974 7920 6973 2065 6e74  tionality is ent
+00001040: 6972 656c 7920 6f70 7469 6f6e 616c 2074  irely optional t
+00001050: 6f20 7573 652c 2061 6e64 206f 7572 206d  o use, and our m
+00001060: 6f64 756c 6172 2073 7472 7563 7475 7265  odular structure
+00001070: 200a 616c 6c6f 7773 2079 6f75 2074 6f20   .allows you to 
+00001080: 7574 696c 697a 6520 6173 206d 7563 6820  utilize as much 
+00001090: 6f72 2061 7320 6c69 7474 6c65 206f 6620  or as little of 
+000010a0: 7468 6520 6c69 6272 6172 7920 6173 2079  the library as y
+000010b0: 6f75 2764 206c 696b 652e 204f 7572 2067  ou'd like. Our g
+000010c0: 6f61 6c20 0a69 7320 746f 2063 6f6e 7369  oal .is to consi
+000010d0: 7374 656e 746c 7920 6164 6420 6e65 7720  stently add new 
+000010e0: 6675 6e63 7469 6f6e 616c 6974 7920 746f  functionality to
+000010f0: 2073 7570 706f 7274 2061 6464 6974 696f   support additio
+00001100: 6e61 6c20 7573 6520 6361 7365 732e 2049  nal use cases. I
+00001110: 6620 796f 7520 0a68 6176 6520 616e 7920  f you .have any 
+00001120: 636f 6d6d 656e 7473 206f 7220 7375 6767  comments or sugg
+00001130: 6573 7469 6f6e 7320 666f 7220 6e65 7720  estions for new 
+00001140: 6665 6174 7572 6573 2c20 646f 6e27 7420  features, don't 
+00001150: 6865 7369 7461 7465 2074 6f20 6372 6561  hesitate to crea
+00001160: 7465 2061 6e20 0a69 7373 7565 206f 7220  te an .issue or 
+00001170: 7265 6163 6820 6f75 7420 746f 3a20 6077  reach out to: `w
+00001180: 6574 7261 6465 2e69 6e62 6f78 4067 6d61  etrade.inbox@gma
+00001190: 696c 2e63 6f6d 203c 6d61 696c 746f 3a77  il.com <mailto:w
+000011a0: 6574 7261 6465 2e69 6e62 6f78 4067 6d61  etrade.inbox@gma
+000011b0: 696c 2e63 6f6d 3e60 5f5f 2e0a 0a0a 2a2a  il.com>`__....**
+000011c0: 4469 7363 6c61 696d 6572 3a2a 2a20 2a77  Disclaimer:** *w
+000011d0: 6574 7261 6465 2069 7320 616e 2075 6e6f  etrade is an uno
+000011e0: 6666 6963 6961 6c20 4150 4920 6c69 6272  fficial API libr
+000011f0: 6172 7920 616e 6420 636f 6d65 7320 7769  ary and comes wi
+00001200: 7468 206e 6f20 7761 7272 616e 7479 0a6f  th no warranty.o
+00001210: 6620 616e 7920 6b69 6e64 2e20 4974 2069  f any kind. It i
+00001220: 7320 696e 206e 6f20 7761 7920 656e 646f  s in no way endo
+00001230: 7273 6564 2062 7920 6f72 2061 6666 696c  rsed by or affil
+00001240: 6961 7465 6420 7769 7468 2045 5c2a 5452  iated with E\*TR
+00001250: 4144 4520 4669 6e61 6e63 6961 6c20 0a6f  ADE Financial .o
+00001260: 7220 616e 7920 6173 736f 6369 6174 6564  r any associated
+00001270: 206f 7267 616e 697a 6174 696f 6e2e 204d   organization. M
+00001280: 616b 6520 7375 7265 2074 6f20 7265 6164  ake sure to read
+00001290: 2061 6e64 2075 6e64 6572 7374 616e 6420   and understand 
+000012a0: 7468 6520 7465 726d 7320 6f66 200a 7365  the terms of .se
+000012b0: 7276 6963 6520 6f66 2074 6865 2075 6e64  rvice of the und
+000012c0: 6572 6c79 696e 6720 4150 4920 6265 666f  erlying API befo
+000012d0: 7265 2075 7369 6e67 2074 6869 7320 7061  re using this pa
+000012e0: 636b 6167 652e 2054 6869 7320 6175 7468  ckage. This auth
+000012f0: 6f72 7320 6163 6365 7074 200a 6e6f 2072  ors accept .no r
+00001300: 6573 706f 6e73 6962 696c 6974 7920 666f  esponsibility fo
+00001310: 7220 616e 7920 6461 6d61 6765 2074 6861  r any damage tha
+00001320: 7420 6d69 6768 7420 7374 656d 2066 726f  t might stem fro
+00001330: 6d20 7573 6520 6f66 2074 6869 7320 7061  m use of this pa
+00001340: 636b 6167 652e 200a 5365 6520 7468 6520  ckage. .See the 
+00001350: 4c49 4345 4e53 4520 6669 6c65 2066 6f72  LICENSE file for
+00001360: 206d 6f72 6520 6465 7461 696c 732e 2a     more details.*
```

### Comparing `wetrade-0.1.1/setup.py` & `wetrade-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import setuptools
 
 with open('README.rst', 'r') as f:
   long_description = f.read()
 
 setuptools.setup(
   name = 'wetrade',
-  version = '0.1.1',
+  version = '0.1.2',
   author = 'Mason Krause',
   description = 'An E-Trade python library built for active stock trading',
   long_description = long_description,
   packages = setuptools.find_packages(),
   include_package_data = True,
   python_requires = '>=3.7',
   install_requires = [
     'authlib',
     'playwright',
     'urllib3==1.26.16',
     'xmltodict',
+    'pytz',
     'pyotp==2.9.0',
     'google-cloud-logging', 
     'google-cloud-storage', 
+    'google-cloud-secret-manager',
     'polars', 
     'pandas', 
-    'pyarrow'])
+    'pyarrow'],
+    extras_require={
+      'dev': [
+        'sphinx_rtd_theme']},)
```

### Comparing `wetrade-0.1.1/tests/mock_api/account_responses.py` & `wetrade-0.1.2/tests/mock_api/account_responses.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/tests/mock_api/mock_api.py` & `wetrade-0.1.2/tests/mock_api/mock_api.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/tests/mock_api/order_responses.py` & `wetrade-0.1.2/tests/mock_api/order_responses.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/tests/mock_api/quote_responses.py` & `wetrade-0.1.2/tests/mock_api/quote_responses.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/tests/order/test_base_order.py` & `wetrade-0.1.2/tests/order/test_base_order.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/tests/quote/test_quote.py` & `wetrade-0.1.2/tests/quote/test_quote.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/tests/test_account.py` & `wetrade-0.1.2/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/tests/test_api.py` & `wetrade-0.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/wetrade/account.py` & `wetrade-0.1.2/wetrade/account.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/wetrade/api.py` & `wetrade-0.1.2/wetrade/api.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/wetrade/order/base_order.py` & `wetrade-0.1.2/wetrade/order/base_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
       error_msg = lookup_error_msg(error_code=error_code, msg_ref=msg_ref, order_id=self.order_id)
       log_in_background(
         called_from = '__modify_order',
         tags = ['user-message'], 
         message = time.strftime('%H:%M:%S', time.localtime()) + error_msg,
         account_key = self.account_key,
         symbol = self.symbol)
-      if error_code in [1508, 163, 1524]:
+      if error_code in (1508, 163, 1524):
         time.sleep(1)
         return self.__modify_order(action_type)
 
   def preview_order(self):
     preview_response = self.__modify_order('preview')
     if preview_response:
       self.place_order_request = {
@@ -172,15 +172,15 @@
 
   def cancel_order(self):
     '''Cancels your active, already-placed order'''
     response, status_code = self.client.request_order_cancel(account_key=self.account_key, order_id=self.order_id, symbol=self.symbol)
     msg_num = 0
     with suppress(Exception):
       msg_num = response['CancelOrderResponse']['Messages']['Message'][0]['code']
-    if msg_num in [5011, 4186]:
+    if msg_num in (5011, 4186):
       log_in_background(
         called_from = 'cancel_order',
         tags = ['user-message'], 
         account_key = self.account_key,
         symbol = self.symbol,
         message = '{}: Requested to cancel order {} (Account: {})'.format(
           time.strftime('%H:%M:%S', time.localtime()),
```

### Comparing `wetrade-0.1.1/wetrade/order/basic_order_types.py` & `wetrade-0.1.2/wetrade/order/basic_order_types.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/wetrade/order/converting_stop_order.py` & `wetrade-0.1.2/wetrade/order/converting_stop_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,14 @@
       error_msg = lookup_error_msg(error_code=error_code, msg_ref=msg_ref, order_id=self.order_id)
       log_in_background(
         called_from = '__modify_order',
         tags = ['user-message'], 
         message = time.strftime('%H:%M:%S', time.localtime()) + error_msg,
         account_key = self.account_key,
         symbol = self.symbol)
-      if error_code in [1508, 163, 1524]:
+      if error_code in (1508, 163, 1524):
         time.sleep(1)
         return self.__modify_order(action_type)
-      elif error_code in [2084, 2085]:
+      elif error_code in (2084, 2085):
         self.order_type =  'MARKET'
         self.preview_order_request['PreviewOrderRequest']['Order']['priceType'] = 'MARKET'
         return self.__modify_order(action_type)
```

### Comparing `wetrade-0.1.1/wetrade/order/lookup_msg.py` & `wetrade-0.1.2/wetrade/order/lookup_msg.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 
 def lookup_error_msg(error_code, msg_ref='with', order_id=0):
   default_msg = f': Unknown error {msg_ref} order, check logs for more info'
   msg_dict = {
     1508: f': Price unavailable {msg_ref} (Order ID: {order_id}), waiting 1 sec then retrying',
     163: f': Processing error {msg_ref} (Order ID: {order_id}), waiting 1 sec then retrying',
-    163: f': Stop price out of range (Order ID: {order_id})- changing to market order and replacing',
-    163: f': Stop price out of range (Order ID: {order_id})- changing to market order and replacing',
+    2084: f': Stop price out of range (Order ID: {order_id})- changing to market order and replacing',
+    2085: f': Stop price out of range (Order ID: {order_id})- changing to market order and replacing',
     1524: f': Order {order_id} still updating, waiting 1 sec then retrying' }
   if error_code in msg_dict:
     return msg_dict[error_code]
   else:
     return default_msg
   
 def lookup_user_msg(action, price=0.0, account_key='', order_response={}, old_id=0):
```

### Comparing `wetrade-0.1.1/wetrade/project_template/__pycache__/settings.cpython-311.pyc` & `wetrade-0.1.2/wetrade/project_template/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/wetrade/project_template/main.py` & `wetrade-0.1.2/wetrade/project_template/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from wetrade.api import APIClient
 from wetrade.account import Account
 from wetrade.quote import Quote
 from wetrade.order import LimitOrder
-from wetrade.utils import setup_logging
+from wetrade.utils import setup_cloud_logging
 
 
 def main():
-  # Setup logging (optional) and APIClient
-  setup_logging()
+  # Setup cloud logging (optional) and APIClient
+  setup_cloud_logging()
   client = APIClient()
 
   # Check out your account
   account = Account(client=client)
   print('My Account Key: ', account.account_key)
   print('My Balance: ', account.check_balance())
```

### Comparing `wetrade-0.1.1/wetrade/project_template/settings.py` & `wetrade-0.1.2/wetrade/project_template/settings.py`

 * *Files identical despite different names*

### Comparing `wetrade-0.1.1/wetrade/quote/data_frame_quote.py` & `wetrade-0.1.2/wetrade/quote/data_frame_quote.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime
 import pickle
 import google.cloud.storage
 import polars as pl 
 import pandas as pd
 from .quote import Quote
 from wetrade.api import APIClient
-from wetrade.utils import log_in_background, check_market_hours
+from wetrade.utils import log_in_background
 try:
   import settings
 except ModuleNotFoundError:
   import wetrade.project_template.settings as settings
 
 
 class DataFrameQuote(Quote):
@@ -35,24 +35,17 @@
       'last_trade_time': pl.Int64,
       '30s_average': pl.Float64,
       '10s_average': pl.Float64})
     self.smoothed_price = 0.0
 
   def __monitor_quote(self):
     if self.monitoring_active == False:
-      market_close = check_market_hours()['close']
-      if time.strftime('%H:%M', time.localtime()) > market_close:
-        log_in_background(
-          called_from = '__monitor_quote',
-          tags = ['user-message'], 
-          symbol = self.symbol,
-          message = '{}: Markets are closed'.format(time.strftime('%H:%M:%S', time.localtime())))
-      else:
+      if self.market_hours.market_has_closed() == False:
         self.monitoring_active = True
-      while self.monitoring_active == True and time.strftime('%H:%M', time.localtime()) < market_close:
+      while self.monitoring_active == True and self.market_hours.market_has_closed() == False:
         quote_data = self.get_quote()
         self.last_price = quote_data['All']['lastTrade']
         self.data.extend(pl.DataFrame({
           'datetime': datetime.datetime.strptime(quote_data['dateTime'], '%H:%M:%S %Z %m-%d-%Y'),
           'datetime_epoch': quote_data['dateTimeUTC'],
           'ask': quote_data['All']['ask'],
           'ask_size': quote_data['All']['askSize'],
```

### Comparing `wetrade-0.1.1/wetrade/quote/multi_quote.py` & `wetrade-0.1.2/wetrade/quote/multi_quote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import time
 import datetime
 from wetrade.api import APIClient
-from wetrade.utils import log_in_background, check_market_hours, start_thread
+from wetrade.market_hours import MarketHours
+from wetrade.utils import log_in_background, start_thread
 
 class MultiQuote:
   '''
   An expanded Quote for tracking multiple securities
 
   :param APIClient client: your :ref:`APIClient <api_client>`
   :param tuple symbols: a tuple containing a list of symbols for up to 25 securities
   '''
   def __init__(self, client:APIClient, symbols:tuple):
     self.client = client
     self.symbols = symbols
     self.symbol_str = ', '.join(self.symbols)
     self.last_prices = {}
     self.monitoring_active = False
+    self.market_hours = MarketHours()
 
   def get_quote(self):
     '''
     Gets the most recent quote details for your securities
     '''
     response, status_code = self.client.request_quote(symbol=self.symbol_str)
     try:
@@ -43,24 +45,17 @@
     for quote in quote_data:
       symbol = quote['Product']['symbol']
       self.last_prices[symbol] =  quote['All']['lastTrade'] 
     return self.last_prices
 
   def __monitor_quote(self):
     if self.monitoring_active == False:
-      market_close = check_market_hours()['close']
-      if time.strftime('%H:%M', time.localtime()) > market_close:
-        log_in_background(
-          called_from = '__monitor_quote',
-          tags = ['user-message'], 
-          symbol = self.symbol,
-          message = '{}: Markets are closed'.format(time.strftime('%H:%M:%S', time.localtime())))
-      else:
+      if self.market_hours.market_has_closed() == False:
         self.monitoring_active = True
-      while self.monitoring_active == True and time.strftime('%H:%M', time.localtime()) < market_close:
+      while self.monitoring_active == True and self.market_hours.market_has_closed() == False:
         self.get_last_price()
         time.sleep(.5)
       self.monitoring_active = False
       
   def monitor_in_background(self):
     '''
     Monitors quote details in a new thread to keep Quote.last_price up to date
```

### Comparing `wetrade-0.1.1/wetrade/quote/quote.py` & `wetrade-0.1.2/wetrade/quote/quote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import time
 import datetime
 from wetrade.api import APIClient
-from wetrade.utils import log_in_background, check_market_hours, start_thread
+from wetrade.market_hours import MarketHours
+from wetrade.utils import log_in_background, start_thread
 
 class Quote:
   '''
   A simple Quote for tracking one security
 
   :param APIClient client: your :ref:`APIClient <api_client>`
   :param str symbol: the symbol of your security
   '''
   def __init__(self, client:APIClient, symbol):
     self.client = client
     self.symbol = symbol
     self.last_price = 0.0
     self.monitoring_active = False
+    self.market_hours = MarketHours()
 
   def get_quote(self):
     '''
     Gets the most recent quote details for your security
     '''
     response, status_code = self.client.request_quote(symbol=self.symbol)
     try:
@@ -45,24 +47,17 @@
     Gets the most recent price for your security
     '''
     self.last_price =  self.get_quote()['All']['lastTrade'] 
     return self.last_price
 
   def __monitor_quote(self):
     if self.monitoring_active == False:
-      market_close = check_market_hours()['close']
-      if time.strftime('%H:%M', time.localtime()) > market_close:
-        log_in_background(
-          called_from = '__monitor_quote',
-          tags = ['user-message'], 
-          symbol = self.symbol,
-          message = '{}: Markets are closed'.format(time.strftime('%H:%M:%S', time.localtime())))
-      else:
+      if self.market_hours.market_has_closed() == False:
         self.monitoring_active = True
-      while self.monitoring_active == True and time.strftime('%H:%M', time.localtime()) < market_close:
+      while self.monitoring_active == True and self.market_hours.market_has_closed() == False:
         quote_data = self.get_quote()
         self.last_price = quote_data['All']['lastTrade']
         time.sleep(.5)
       self.monitoring_active = False
       
   def monitor_in_background(self):
     '''
```

### Comparing `wetrade-0.1.1/wetrade/user_session.py` & `wetrade-0.1.2/wetrade/user_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,27 @@
     return new_session(config)
   
 class UserSession:
   def __init__(self, config={}):
     self.config = settings.config if config == {} else config
     self.session = new_session(self.config)
     self.logged_in = True
-    
+
+  def renew_token(self):
+    self.logged_in = False
+    r = self.session.get(url='https://api.etrade.com/oauth/renew_access_token')
+    if r.status_code != 200:
+      self.logged_in = True
+    else:
+      log_in_background(
+        called_from = 'renew_token',
+        tags = ['user-message'], 
+        message = time.strftime('%H:%M:%S', time.localtime()) + ': Error renewing access token')
+      self.login()
+
   def login(self):
     self.logged_in = False
     try:
       self.session = new_session(self.config)
       self.logged_in = True
     except Exception as e:
       log_in_background(
```

### Comparing `wetrade-0.1.1/wetrade/utils.py` & `wetrade-0.1.2/wetrade/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import pprint
 import threading
 import requests
 import time
 import traceback
+import os
+import ast
 import google.cloud.logging
+from google.cloud import secretmanager
 try: 
   import settings
 except ModuleNotFoundError:
   import wetrade.project_template.settings as settings
 
 
 def start_thread(func, name=None, args=[], kwargs={}):
@@ -18,41 +21,39 @@
   try:
     return r.json()
   except: # r.status_code == 204 (no content) and other non-parsable requests 
     return str(r.content)
   
 def log_in_background(called_from, r=None, url='', tags=[], account_key='', symbol='', message='', e=None):
   start_thread(pretty_print, args=[called_from, r, url, tags, account_key, symbol, message, e])
-  if hasattr(settings, 'enable_cloud_logging') and settings.enable_cloud_logging == True:
+  if hasattr(settings, 'enable_logging') and settings.enable_logging == True:
     start_thread(log, args=[called_from, r, url, tags, account_key, symbol, message, e])
 
 def pretty_print(called_from, r=None, url='', tags=[], account_key='', symbol='', message='', e=None):
   if message != '':
     print(message)
   if e:
     print('e', e)
     # traceback.print_exception(type(e), e, e.__traceback__)
   if r != None:
     response = parse_response_data(r)
-    # print('RESPONSE: ')
-    # pprint.pprint(response)
     if 'Error' in response:
       response_tags = ['response', 'error']
       pprint.pprint({
         'called_from': called_from,
         'tags': [*tags, *response_tags],
         'account_key': account_key,
         'config': settings.config_id,
         'symbol': symbol,
         'url': url,
         'status_code': r.status_code, 
         'response': response})
 
-def setup_logging():
-  if hasattr(settings, 'enable_cloud_logging') and settings.enable_cloud_logging == True:
+def setup_cloud_logging():
+  if hasattr(settings, 'enable_logging') and settings.enable_logging == True:
     client = google.cloud.logging.Client()
     client.setup_logging()
 
 def log(called_from, r=None, url='', tags=[], account_key='', symbol='', message='', e=None):
   if r != None:
     response = parse_response_data(r)
     log_level = 30 if 'Error' in response else 20
@@ -81,21 +82,19 @@
     tb_info = traceback.format_exception(etype=type(e), value=e, tb=e.__traceback__)
     tb_str = ''.join(tb_info)
     logging.error({ 
       'called_from': called_from,
       'config': settings.config_id,
       'message': str(e),
       'tb_info': tb_str})
-    
-# This doesn't really belong here but E-trade doesn't have market hours endpoint
-def check_market_hours(day_str=''):
-  day_str = time.strftime('%Y-%m-%d', time.localtime()) if day_str == '' else day_str
-  key = settings.hours_key if hasattr(settings, 'hours_key') else 'PKNL4NZJEHKGDPLL8CVY'
-  secret = settings.hours_secret if hasattr(settings, 'hours_secret') else 'sxMOohHeLG6DODKv0tu237flYuwVaM0rvoea0M2F'
-  params = {'start': day_str, 'end': day_str}
-  headers = {'APCA-API-KEY-ID': key, 'APCA-API-SECRET-KEY': secret}
-  r = requests.get('https://paper-api.alpaca.markets/v2/calendar', params=params, headers=headers)
-  results = parse_response_data(r)
-  if results == []:
-    return {'open': '00:00', 'close': '00:00'}
-  else:
-    return {'open': results[0]['open'], 'close': results[0]['close']}
+  
+def get_gcloud_secret(secret_id, version_id='latest'):
+  gcloud_file = os.getenv('GOOGLE_APPLICATION_CREDENTIALS', '!no-gcloud-file!')
+  if gcloud_file != '!no-gcloud-file!':
+    with open(gcloud_file) as f:
+      data = f.read()
+    gcloud_data = ast.literal_eval(data)
+    project_id = gcloud_data['project_id']
+    secret_name = f'projects/{project_id}/secrets/{secret_id}/versions/{version_id}'
+    client = secretmanager.SecretManagerServiceClient()
+    response = client.access_secret_version(name=secret_name)
+    return response.payload.data.decode('UTF-8')
```

### Comparing `wetrade-0.1.1/wetrade.egg-info/PKG-INFO` & `wetrade-0.1.2/wetrade.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: wetrade
-Version: 0.1.1
+Version: 0.1.2
 Summary: An E-Trade python library built for active stock trading
 Author: Mason Krause
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: authlib
 Requires-Dist: playwright
 Requires-Dist: urllib3==1.26.16
 Requires-Dist: xmltodict
+Requires-Dist: pytz
 Requires-Dist: pyotp==2.9.0
 Requires-Dist: google-cloud-logging
 Requires-Dist: google-cloud-storage
+Requires-Dist: google-cloud-secret-manager
 Requires-Dist: polars
 Requires-Dist: pandas
 Requires-Dist: pyarrow
+Provides-Extra: dev
+Requires-Dist: sphinx_rtd_theme; extra == "dev"
 
 ``wetrade``: An E-Trade Python library built for automated stock trading 
 =========================================================================
 
 ``wetrade`` overview
 --------------------
 
@@ -91,20 +95,20 @@
 
 .. code-block:: python
 
   from wetrade.api import APIClient
   from wetrade.account import Account
   from wetrade.quote import Quote
   from wetrade.order import LimitOrder
-  from wetrade.utils import setup_logging
+  from wetrade.utils import setup_cloud_logging
 
 
   def main():
-    # Setup logging (optional) and APIClient
-    setup_logging()
+    # Setup cloud logging (optional) and APIClient
+    setup_cloud_logging()
     client = APIClient()
 
     # Check out your account
     account = Account(client=client)
     print('My Account Key: ', account.account_key)
     print('My Balance: ', account.check_balance())
 
@@ -150,12 +154,12 @@
 allows you to utilize as much or as little of the library as you'd like. Our goal 
 is to consistently add new functionality to support additional use cases. If you 
 have any comments or suggestions for new features, don't hesitate to create an 
 issue or reach out to: `wetrade.inbox@gmail.com <mailto:wetrade.inbox@gmail.com>`__.
 
 
 **Disclaimer:** *wetrade is an unofficial API library and comes with no warranty
-of any kind. It is in no way endorsed by or affiliated with E*TRADE Financial 
+of any kind. It is in no way endorsed by or affiliated with E\*TRADE Financial 
 or any associated organization. Make sure to read and understand the terms of 
 service of the underlying API before using this package. This authors accept 
 no responsibility for any damage that might stem from use of this package. 
 See the LICENSE file for more details.*
```

### Comparing `wetrade-0.1.1/wetrade.egg-info/SOURCES.txt` & `wetrade-0.1.2/wetrade.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 tests/quote/__init__.py
 tests/quote/test_data_frame_quote.py
 tests/quote/test_quote.py
 wetrade/__init__.py
 wetrade/__main__.py
 wetrade/account.py
 wetrade/api.py
+wetrade/market_hours.py
 wetrade/user_session.py
 wetrade/utils.py
 wetrade.egg-info/PKG-INFO
 wetrade.egg-info/SOURCES.txt
 wetrade.egg-info/dependency_links.txt
 wetrade.egg-info/requires.txt
 wetrade.egg-info/top_level.txt
@@ -33,13 +34,14 @@
 wetrade/order/lookup_msg.py
 wetrade/project_template/Dockerfile
 wetrade/project_template/__init__.py
 wetrade/project_template/main.py
 wetrade/project_template/new_project.py
 wetrade/project_template/requirements.txt
 wetrade/project_template/settings.py
+wetrade/project_template/trading_session.py
 wetrade/project_template/__pycache__/__init__.cpython-311.pyc
 wetrade/project_template/__pycache__/settings.cpython-311.pyc
 wetrade/quote/__init__.py
 wetrade/quote/data_frame_quote.py
 wetrade/quote/multi_quote.py
 wetrade/quote/quote.py
```

