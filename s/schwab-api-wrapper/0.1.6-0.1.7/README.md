# Comparing `tmp/schwab_api_wrapper-0.1.6.tar.gz` & `tmp/schwab_api_wrapper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.1.6.tar", last modified: Sun Jun  2 05:35:17 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.1.7.tar", last modified: Sun Jun  2 17:40:24 2024, max compression
```

## Comparing `schwab_api_wrapper-0.1.6.tar` & `schwab_api_wrapper-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:35:17.518130 schwab_api_wrapper-0.1.6/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 05:35:17.517902 schwab_api_wrapper-0.1.6/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-06-02 05:34:46.000000 schwab_api_wrapper-0.1.6/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:35:17.514629 schwab_api_wrapper-0.1.6/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:35:17.516054 schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     2777 2024-06-02 05:34:35.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/instruments_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/oauth_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    38567 2024-06-02 04:00:32.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:35:17.516758 schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8458 2024-06-02 04:08:26.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:35:17.517670 schwab_api_wrapper-0.1.6/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 05:35:17.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      969 2024-06-02 05:35:17.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-06-02 05:35:17.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-06-02 05:35:17.000000 schwab_api_wrapper-0.1.6/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-06-02 05:35:17.518168 schwab_api_wrapper-0.1.6/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 05:35:17.516901 schwab_api_wrapper-0.1.6/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    50238 2024-06-02 04:27:49.000000 schwab_api_wrapper-0.1.6/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 17:40:24.559239 schwab_api_wrapper-0.1.7/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 17:40:24.558984 schwab_api_wrapper-0.1.7/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-06-02 17:39:54.000000 schwab_api_wrapper-0.1.7/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 17:40:24.554110 schwab_api_wrapper-0.1.7/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 17:40:24.555850 schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     2777 2024-06-02 05:34:35.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/instruments_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10370 2024-06-02 17:38:58.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/oauth_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    38567 2024-06-02 04:00:32.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 17:40:24.557669 schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8458 2024-06-02 04:08:26.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 17:40:24.558716 schwab_api_wrapper-0.1.7/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 17:40:24.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      969 2024-06-02 17:40:24.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-06-02 17:40:24.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-06-02 17:40:24.000000 schwab_api_wrapper-0.1.7/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-06-02 17:40:24.559294 schwab_api_wrapper-0.1.7/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 17:40:24.557983 schwab_api_wrapper-0.1.7/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    50238 2024-06-02 04:27:49.000000 schwab_api_wrapper-0.1.7/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.1.6/LICENSE` & `schwab_api_wrapper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/PKG-INFO` & `schwab_api_wrapper-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.6
+Version: 0.1.7
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.6/pyproject.toml` & `schwab_api_wrapper-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/instruments_schemas.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/instruments_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     mark: float  # mark price
     quoteTime: int  # Extended market quote time in milliseconds since Epoch
     totalVolume: int  # Total volume
     tradeTime: int  # Extended market trade time in milliseconds since Epoch
 
 
 class DivFreqOption(Enum):
+    ZERO = 0
     ONE = 1
     TWO = 2
     THREE = 3
     FOUR = 4
     SIX = 6
     ELEVEN = 11
     TWELVE = 12
@@ -44,31 +45,31 @@
     Fundamentals of a security
     """
 
     avg10DaysVolume: float  # Average 10 day volume
     avg1YearVolume: (
         float  # Average 1 day volume  TODO this documentation must be incorrect
     )
-    declarationDate: datetime  # Declaration date in yyyy-mm-ddThh:mm:ssZ
+    declarationDate: datetime | None = None  # Declaration date in yyyy-mm-ddThh:mm:ssZ
     divAmount: float  # Dividend Amount
-    divExDate: str  # Dividend date in yyyy-mm-ddThh:mm:ssZ
+    divExDate: datetime | None = None  # Dividend date in yyyy-mm-ddThh:mm:ssZ
     # 1 - once a year or annually
     # 2 - 2x a year of semi-annualy
     # 3 - 3x a year
     # 4 - 4x a year or quarterly
     # 6 - 6x per yr or every other month
     # 11 - 11x a year
     # 12 - 12x a year or monthly
     divPayAmount: float  # Dividend Pay Amount
-    divPayDate: str  # Dividend pay date in yyyy-mm-ddThh:mm:ssZ
+    divPayDate: datetime | None = None  # Dividend pay date in yyyy-mm-ddThh:mm:ssZ
     divYield: float  # Dividend yield
     eps: float  # Earnings per Share
     fundLeverageFactor: float  # Fund Leverage Factor + > 0 <-
-    nextDivExDate: str  # Next Dividend date in yyyy-MM-ddThh:mm:ssZ
-    nextDivPayDate: str  # Next Dividend pay date in yyyy-MM-ddThh:mm:ssZ
+    nextDivExDate: datetime | None = None # Next Dividend date in yyyy-MM-ddThh:mm:ssZ
+    nextDivPayDate: datetime | None = None  # Next Dividend pay date in yyyy-MM-ddThh:mm:ssZ
     peRatio: float  # P/E Ratio
     divFreq: Optional[DivFreqOption] = None  # Dividend frequency
     fundStrategy: Optional[FundStrategyOption] = None  # FundStrategy
     # "A" - Active
     # "L" - Leveraged
     # "P" - Passive
     # "Q" - Quantitative
```

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/schwab.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.6
+Version: 0.1.7
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.6/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.1.7/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.6/tests/test_schawb_api.py` & `schwab_api_wrapper-0.1.7/tests/test_schawb_api.py`

 * *Files identical despite different names*

