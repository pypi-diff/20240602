# Comparing `tmp/schwab_api_wrapper-0.1.4.tar.gz` & `tmp/schwab_api_wrapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.1.4.tar", last modified: Sun Jun  2 04:44:48 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.1.5.tar", last modified: Sun Jun  2 05:30:00 2024, max compression
```

## Comparing `schwab_api_wrapper-0.1.4.tar` & `schwab_api_wrapper-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.145539 schwab_api_wrapper-0.1.4/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:44:48.145309 schwab_api_wrapper-0.1.4/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-06-02 04:43:42.000000 schwab_api_wrapper-0.1.4/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.141043 schwab_api_wrapper-0.1.4/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.142603 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     2749 2024-06-02 04:43:08.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/instruments_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/oauth_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    38567 2024-06-02 04:00:32.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.143830 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8458 2024-06-02 04:08:26.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.145088 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      969 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-06-02 04:44:48.145581 schwab_api_wrapper-0.1.4/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.144146 schwab_api_wrapper-0.1.4/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    50238 2024-06-02 04:27:49.000000 schwab_api_wrapper-0.1.4/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:30:00.679215 schwab_api_wrapper-0.1.5/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 05:30:00.678933 schwab_api_wrapper-0.1.5/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-06-02 05:29:26.000000 schwab_api_wrapper-0.1.5/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:30:00.675362 schwab_api_wrapper-0.1.5/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:30:00.676909 schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     2763 2024-06-02 05:28:23.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/instruments_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/oauth_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    38567 2024-06-02 04:00:32.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:30:00.677861 schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8458 2024-06-02 04:08:26.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:30:00.678721 schwab_api_wrapper-0.1.5/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 05:30:00.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      969 2024-06-02 05:30:00.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-06-02 05:30:00.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-06-02 05:30:00.000000 schwab_api_wrapper-0.1.5/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-06-02 05:30:00.679257 schwab_api_wrapper-0.1.5/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:30:00.678025 schwab_api_wrapper-0.1.5/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    50238 2024-06-02 04:27:49.000000 schwab_api_wrapper-0.1.5/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.1.4/LICENSE` & `schwab_api_wrapper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/PKG-INFO` & `schwab_api_wrapper-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.4
+Version: 0.1.5
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.4/pyproject.toml` & `schwab_api_wrapper-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/instruments_schemas.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/instruments_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     bondMultiplier: str
     bondPrice: float
 
 
 class InstrumentResponse(BaseModel):
     cusip: str
     symbol: str
-    description: str
+    description: str | None = None
     exchange: str
     assetType: AssetType
     bondFactor: str | None = None
     bondMultiplier: str | None = None
     bondPrice: float | None = None
     fundamental: FundamentalInst | None = None
     instrumentInfo: Instrument | None = None
```

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/schwab.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.4
+Version: 0.1.5
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.1.5/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.4/tests/test_schawb_api.py` & `schwab_api_wrapper-0.1.5/tests/test_schawb_api.py`

 * *Files identical despite different names*

