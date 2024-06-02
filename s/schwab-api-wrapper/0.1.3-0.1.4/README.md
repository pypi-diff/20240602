# Comparing `tmp/schwab_api_wrapper-0.1.3.tar.gz` & `tmp/schwab_api_wrapper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.1.3.tar", last modified: Sun Jun  2 04:28:42 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.1.4.tar", last modified: Sun Jun  2 04:44:48 2024, max compression
```

## Comparing `schwab_api_wrapper-0.1.3.tar` & `schwab_api_wrapper-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.279652 schwab_api_wrapper-0.1.3/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:28:42.279445 schwab_api_wrapper-0.1.3/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-06-02 04:28:07.000000 schwab_api_wrapper-0.1.3/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.275476 schwab_api_wrapper-0.1.3/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.276993 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     2624 2024-06-02 04:10:18.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/instruments_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/oauth_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    38567 2024-06-02 04:00:32.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.278260 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8458 2024-06-02 04:08:26.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.279242 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      969 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-06-02 04:28:42.279693 schwab_api_wrapper-0.1.3/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.278543 schwab_api_wrapper-0.1.3/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    50238 2024-06-02 04:27:49.000000 schwab_api_wrapper-0.1.3/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.145539 schwab_api_wrapper-0.1.4/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:44:48.145309 schwab_api_wrapper-0.1.4/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-06-02 04:43:42.000000 schwab_api_wrapper-0.1.4/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.141043 schwab_api_wrapper-0.1.4/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.142603 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     2749 2024-06-02 04:43:08.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/instruments_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/oauth_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    38567 2024-06-02 04:00:32.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.143830 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8458 2024-06-02 04:08:26.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.145088 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      969 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-06-02 04:44:48.000000 schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-06-02 04:44:48.145581 schwab_api_wrapper-0.1.4/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:44:48.144146 schwab_api_wrapper-0.1.4/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    50238 2024-06-02 04:27:49.000000 schwab_api_wrapper-0.1.4/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.1.3/LICENSE` & `schwab_api_wrapper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/PKG-INFO` & `schwab_api_wrapper-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.3/pyproject.toml` & `schwab_api_wrapper-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/instruments_schemas.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/instruments_schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pydantic import BaseModel
+from datetime import datetime
 from enum import Enum
 
 
 class AssetType(Enum):
     BOND = "BOND"
     EQUITY = "EQUITY"
     ETF = "ETF"
@@ -19,15 +20,15 @@
 
 
 class FundamentalInst(BaseModel):
     symbol: str
     low52: float
     dividendAmount: float
     dividendYield: float
-    dividendDate: str
+    dividendDate: datetime | None = None
     peRatio: float
     pegRatio: float
     pbRatio: float
     prRatio: float
     pcfRatio: float
     grossMarginTTM: float
     grossMarginMRQ: float
@@ -55,29 +56,29 @@
     marketCapFloat: float
     marketCap: float
     bookValuePerShare: float
     shortIntToFloat: float
     shortIntDayToCover: float
     divGrowthRate3Year: float
     dividendPayAmount: float
-    dividendPayDate: str
+    dividendPayDate: datetime | None = None
     beta: float
     vol1DayAvg: float
     vol10DayAvg: float
     vol3MonthAvg: float
     avg10DaysVolume: int
     avg1DayVolume: int
     avg3MonthVolume: int
-    declarationDate: str
+    declarationDate: datetime | None = None
     dividendFreq: int
     eps: float
     corpactionDate: str | None = None
     dtnVolume: int
-    nextDividendPayDate: str
-    nextDividendDate: str
+    nextDividendPayDate: datetime | None = None
+    nextDividendDate: datetime | None = None
     fundLeverageFactor: float
     fundStrategy: str | None = None
 
 
 class Instrument(BaseModel):
     cusip: str
     symbol: str
```

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/schwab.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.1.4/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.3/tests/test_schawb_api.py` & `schwab_api_wrapper-0.1.4/tests/test_schawb_api.py`

 * *Files identical despite different names*

