# Comparing `tmp/schwab_api_wrapper-0.1.2.tar.gz` & `tmp/schwab_api_wrapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.1.2.tar", last modified: Mon May 27 22:37:15 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.1.3.tar", last modified: Sun Jun  2 04:28:42 2024, max compression
```

## Comparing `schwab_api_wrapper-0.1.2.tar` & `schwab_api_wrapper-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.991520 schwab_api_wrapper-0.1.2/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 22:37:15.991251 schwab_api_wrapper-0.1.2/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 22:36:34.000000 schwab_api_wrapper-0.1.2/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.987248 schwab_api_wrapper-0.1.2/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.988828 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/oauth_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    37206 2024-05-27 22:35:28.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.990017 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-27 20:38:24.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.990838 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      915 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 22:37:15.991572 schwab_api_wrapper-0.1.2/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.990284 schwab_api_wrapper-0.1.2/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    46341 2024-05-27 20:52:23.000000 schwab_api_wrapper-0.1.2/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.279652 schwab_api_wrapper-0.1.3/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:28:42.279445 schwab_api_wrapper-0.1.3/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-06-02 04:28:07.000000 schwab_api_wrapper-0.1.3/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.275476 schwab_api_wrapper-0.1.3/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.276993 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     2624 2024-06-02 04:10:18.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/instruments_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/oauth_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    38567 2024-06-02 04:00:32.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.278260 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8458 2024-06-02 04:08:26.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.279242 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      969 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-06-02 04:28:42.000000 schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-06-02 04:28:42.279693 schwab_api_wrapper-0.1.3/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-06-02 04:28:42.278543 schwab_api_wrapper-0.1.3/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    50238 2024-06-02 04:27:49.000000 schwab_api_wrapper-0.1.3/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.1.2/LICENSE` & `schwab_api_wrapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/PKG-INFO` & `schwab_api_wrapper-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.2/pyproject.toml` & `schwab_api_wrapper-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/schwab.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .response_aware_retry import ResponseAwareRetry
 from .utils import *
 
 from .market_data.quotes_schemas import QuoteResponse
 from .market_data.market_hours_schemas import MarketHoursResponse
 from .market_data.price_history_schemas import CandleList
 from .market_data.errors_schema import MarketDataError
+from .market_data.instruments_schemas import InstrumentsRoot
 
 from .trader_api.accounts_schemas import (
     AccountNumbersResponse,
     AccountsResponse,
     Account,
 )
 from .trader_api.transactions_schemas import (
@@ -338,14 +339,51 @@
 
         logging.getLogger(__name__).debug("Response JSON:\n" + pformat(response.json()))
 
         if response.status_code == STATUS_CODE_OK:
             return QuoteResponse(**response.json()), None
         else:
             return None, MarketDataError(**response.json())
+        
+    def instruments(
+        self,
+        symbols: list[str],
+        projection: Projection,
+        retry: bool = False
+    ) -> tuple[Optional[InstrumentsRoot], Optional[MarketDataError]]:
+        """
+        Get Instruments details by using different projections. Get more specific fundamental instrument data by using fundamental as the projection.
+
+        Parameters:
+            symbol: symbol of a security
+            projection: search by available values : symbol-search, symbol-regex, desc-search, desc-regex, search, fundamental
+        """
+
+        params = {
+            "symbol": ",".join(symbols),
+            "projection": projection.value
+        }
+
+        logging.getLogger(__name__).debug("Instruments Params:\n" + pformat(params))
+
+        response = self.__get(
+            INSTRUMENTS_URL, params=params, headers=self.headers, retry=retry
+        )
+
+        logging.getLogger(__name__).info(
+            f"Schwab API | GET `{INSTRUMENTS_URL}` | Status: {response.status_code}"
+        )
+
+        logging.getLogger(__name__).debug("Response JSON:\n" + pformat(response.json()))
+
+        if response.status_code == STATUS_CODE_OK:
+            return InstrumentsRoot(**response.json()), None
+        else:
+            return None, MarketDataError(**response.json())
+
 
     def market_hours(
         self,
         markets: list[MarketID],
         query_date: Optional[date] = None,
         retry: bool = False,
     ) -> tuple[Optional[MarketHoursResponse], Optional[MarketDataError]]:
```

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 AUTH_URL = f"{BASE_URL}/v1/oauth/authorize"
 TOKEN_URL = f"{BASE_URL}/v1/oauth/token"
 
 QUOTES_URL = f"{MARKET_DATA_ENDPOINT}/quotes"
 MARKET_HOURS_URL = f"{MARKET_DATA_ENDPOINT}/markets"
 PRICE_HISTORY_URL = f"{MARKET_DATA_ENDPOINT}/pricehistory"
+INSTRUMENTS_URL = f"{MARKET_DATA_ENDPOINT}/instruments"
 
 ACCOUNT_NUMBERS_URL = f"{TRADER_API_ENDPOINT}/accounts/accountNumbers"
 ACCOUNTS_URL = f"{TRADER_API_ENDPOINT}/accounts"
 ORDERS_URL = f"{TRADER_API_ENDPOINT}/orders"
 
 
 # Parse redirect URL for desired parameters
@@ -57,14 +58,23 @@
     QUOTE = "quote"
     FUNDAMENTAL = "fundamental"
     EXTENDED = "extended"
     REFERENCE = "reference"
     REGULAR = "regular"
 
 
+class Projection(Enum):
+    SYMBOL_SEARCH = "symbol-search"
+    SYMBOL_REGEX = "symbol-regex"
+    DESC_SEARCH = "desc-search"
+    DESC_REGEX = "desc-regex"
+    SEARCH = "search"
+    FUNDAMENTAL = "fundamental"
+
+
 class MarketID(Enum):
     EQUITY = "equity"
     OPTION = "option"
     BOND = "bond"
     FUTURE = "future"
     FOREX = "forex"
```

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.1.3/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 schwab_api_wrapper/utils.py
 schwab_api_wrapper.egg-info/PKG-INFO
 schwab_api_wrapper.egg-info/SOURCES.txt
 schwab_api_wrapper.egg-info/dependency_links.txt
 schwab_api_wrapper.egg-info/top_level.txt
 schwab_api_wrapper/market_data/__init__.py
 schwab_api_wrapper/market_data/errors_schema.py
+schwab_api_wrapper/market_data/instruments_schemas.py
 schwab_api_wrapper/market_data/market_hours_schemas.py
 schwab_api_wrapper/market_data/price_history_schemas.py
 schwab_api_wrapper/market_data/quotes_schemas.py
 schwab_api_wrapper/trader_api/__init__.py
 schwab_api_wrapper/trader_api/accounts_schemas.py
 schwab_api_wrapper/trader_api/errors_schema.py
 schwab_api_wrapper/trader_api/orders_schemas.py
```

### Comparing `schwab_api_wrapper-0.1.2/tests/test_schawb_api.py` & `schwab_api_wrapper-0.1.3/tests/test_schawb_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     TransactionType,
 )
 
 from schwab_api_wrapper.market_data.quotes_schemas import QuoteResponse
 from schwab_api_wrapper.market_data.errors_schema import MarketDataError
 from schwab_api_wrapper.market_data.market_hours_schemas import MarketHoursResponse
 from schwab_api_wrapper.market_data.price_history_schemas import CandleList
+from schwab_api_wrapper.market_data.instruments_schemas import InstrumentsRoot
 
 from schwab_api_wrapper.schwab import SchwabAPI, OAuthException
 
 logging.basicConfig(level=logging.INFO)
 
 
 PARAMETERS_FILE_NAME = "fakefile.json"
@@ -1361,10 +1362,123 @@
         result, error = self.api.get_single_transaction(
             self.encrypted_account_number, self.transaction_id
         )
         self.assertIsNone(result)
         self.assertIsInstance(error, AccountsAndTradingError)
         self.assertEqual(error.message, "Transaction not found")
 
+    @responses.activate
+    def test_instruments_symbol_search(self):
+        responses.add(
+            responses.GET,
+            INSTRUMENTS_URL,
+            json={
+                'instruments': [
+                    {
+                        'cusip': '037833100',
+                        'symbol': 'AAPL',
+                        'description': 'Apple Inc',
+                        'exchange': 'NASDAQ',
+                        'assetType': 'EQUITY',
+                    },
+                    {
+                        'cusip': '00206R102',
+                        'symbol': 'T',
+                        'description': 'A T & T Inc',
+                        'exchange': 'NYSE',
+                        'assetType': 'EQUITY',
+                    },
+                ],
+            },
+            status=200
+        )
+
+        result, error = self.api.instruments(["AAPL", "T"], Projection.SYMBOL_SEARCH)
+
+        self.assertIsInstance(result, InstrumentsRoot)
+        self.assertIsNone(error)
+
+    @responses.activate
+    def test_instruments_fundamentals(self):
+        responses.add(
+            responses.GET,
+            INSTRUMENTS_URL,
+            json=json.load(
+                open(
+                    Path(os.path.dirname(__file__))
+                    / "sample_responses"
+                    / "instruments_fundamentals.json",
+                    "r",
+                )
+            ),
+            status=200,
+        )
+
+        result, error = self.api.instruments(["AAPL", "T"], Projection.FUNDAMENTAL)
+
+        self.assertIsInstance(result, InstrumentsRoot)
+        self.assertIsNone(error)
+
+    @responses.activate
+    def test_instruments_bad_projection(self):
+        responses.add(
+            responses.GET,
+            INSTRUMENTS_URL,
+            json={
+                'errors': [
+                    {
+                        'id': 'cd214562-7489-4c98-af64-e3db04037f09',
+                        'status': '400',
+                        'title': 'Bad Request',
+                        'detail': (
+                            'Projection has to be one of following: symbol-search,symbol-regex,desc-search,desc-regex,search,funda'
+                            'mental'
+                        ),
+                        'source': {
+                            'parameter': 'projection',
+                        },
+                    },
+                ],
+            },
+            status=400
+        )
+
+        result, error = self.api.instruments(["AAPL", "T"], Projection.SYMBOL_SEARCH)
+
+        self.assertIsNone(result)
+        self.assertIsInstance(error, MarketDataError)
+        self.assertEqual(error.errors[0].detail, 'Projection has to be one of following: symbol-search,symbol-regex,desc-search,desc-regex,search,fundamental')
+        self.assertEqual(error.errors[0].source.parameter, 'projection')
+
+
+    @responses.activate
+    def test_instruments_bad_symbol(self):
+        responses.add(
+            responses.GET,
+            INSTRUMENTS_URL,
+            json={
+                'errors': [
+                    {
+                        'id': '4c8591c4-0946-4424-9648-fe7b6e026906',
+                        'status': '400',
+                        'title': 'Bad Request',
+                        'detail': 'Symbol cannot be null or empty.',
+                        'source': {
+                            'parameter': 'symbol',
+                        },
+                    },
+                ],
+            },
+            status=400
+        )
+
+        result, error = self.api.instruments(["AAPL", "T"], Projection.SYMBOL_SEARCH)
+
+        self.assertIsNone(result)
+        self.assertIsInstance(error, MarketDataError)
+        self.assertEqual(error.errors[0].detail, 'Symbol cannot be null or empty.')
+        self.assertEqual(error.errors[0].source.parameter, 'symbol')
+
+
 
 if __name__ == "__main__":
     unittest.main()
```

