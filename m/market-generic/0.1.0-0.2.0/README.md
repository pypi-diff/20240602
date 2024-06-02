# Comparing `tmp/market_generic-0.1.0.tar.gz` & `tmp/market_generic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market_generic-0.1.0.tar", last modified: Sun May 26 16:23:11 2024, max compression
+gzip compressed data, was "market_generic-0.2.0.tar", last modified: Sun Jun  2 06:17:43 2024, max compression
```

## Comparing `market_generic-0.1.0.tar` & `market_generic-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.096953 market_generic-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-26 16:23:11.096953 market_generic-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-26 16:22:57.000000 market_generic-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.096953 market_generic-0.1.0/market_generic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-26 16:22:57.000000 market_generic-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 16:23:11.096953 market_generic-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-26 16:22:57.000000 market_generic-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/calendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/calendar/calendar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/calendar/calendar_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/nse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/nse_all_stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/nse_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/nse_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/ticker/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/market.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/stock_generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/yf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.096953 market_generic-0.1.0/trade/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/df_market_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/gsheet_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/html_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/log_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/op_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/telegram_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-06-02 06:17:43.030336 market_generic-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-02 06:17:28.000000 market_generic-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/market_generic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 06:17:42.000000 market_generic-0.2.0/market_generic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-02 06:17:28.000000 market_generic-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 06:17:43.030336 market_generic-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-02 06:17:28.000000 market_generic-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.026336 market_generic-0.2.0/trade/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.026336 market_generic-0.2.0/trade/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/calendar/calendar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/calendar/calendar_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.026336 market_generic-0.2.0/trade/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/exchange/yf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/nse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/data_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/nse/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/indices/nse_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/indices/nse_indices_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/nse_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/nse_fno.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/nse/stocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/stocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/stocks/nse_all_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/nse/stocks/nse_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/option_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/generic_option_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/index_option_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/option_chain/stock_option_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:17:43.030336 market_generic-0.2.0/trade/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/df_market_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/gsheet_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/html_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/log_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/op_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/telegram_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-02 06:17:28.000000 market_generic-0.2.0/trade/utils/utility_enabler.py
```

### Comparing `market_generic-0.1.0/PKG-INFO` & `market_generic-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-generic
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Generic Python Package for Stock Market Analysis and Trading
 Home-page: https://github.com/sharmasourab93/market-generic
 Author: Sourab S Sharma
 Author-email: sharmasourab93@gmail.com
 Keywords: Market,Trade,Analysis
 Description-Content-Type: text/markdown
 Requires-Dist: black==24.4.2
```

### Comparing `market_generic-0.1.0/README.md` & `market_generic-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/market_generic.egg-info/PKG-INFO` & `market_generic-0.2.0/market_generic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-generic
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Generic Python Package for Stock Market Analysis and Trading
 Home-page: https://github.com/sharmasourab93/market-generic
 Author: Sourab S Sharma
 Author-email: sharmasourab93@gmail.com
 Keywords: Market,Trade,Analysis
 Description-Content-Type: text/markdown
 Requires-Dist: black==24.4.2
```

### Comparing `market_generic-0.1.0/setup.py` & `market_generic-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 NAME = "market-generic"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 DESCRITPION = "A Generic Python Package for Stock Market Analysis and Trading"
 URL = "https://github.com/sharmasourab93/market-generic"
 AUTHOR = "Sourab S Sharma"
 EMAIL = "sharmasourab93@gmail.com"
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
@@ -21,11 +21,12 @@
     author=AUTHOR,
     author_email=EMAIL,
     description=DESCRITPION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url=URL,
     packages=find_packages(exclude=["tests", ".github"]),
+    package_data={"market-generic": ["configs/nse.json"]},
     setup_requires=["wheel"],
     install_requires=INSTALL_REQUIRES,
     keywords=KEYWORDS,
 )
```

### Comparing `market_generic-0.1.0/trade/calendar/calendar_data.py` & `market_generic-0.2.0/trade/calendar/calendar_data.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/calendar/calendar_tool.py` & `market_generic-0.2.0/trade/calendar/calendar_tool.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/nse/nse_config.py` & `market_generic-0.2.0/trade/nse/nse_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from collections.abc import Sequence
 from dataclasses import dataclass, field
 from datetime import date, datetime, time
 from functools import cache, cached_property
 from io import BytesIO
 from pathlib import Path
 from typing import Dict, List, Optional, Union
@@ -13,17 +14,19 @@
 from trade.calendar.calendar_data import (
     DateObj,
     MarketHolidayType,
     MarketTimings,
     MarketTimingType,
     WorkingDayDate,
 )
-from trade.ticker import Exchange, ExchangeArgs
+from trade.exchange import Exchange, ExchangeArgs
+from trade.nse.nse_fno import NSEFNO
 from trade.utils import LoggingType, operations
 from trade.utils.network_tools import CustomHTTPException
+from trade.utils.utility_enabler import UtilityEnabler
 
 DATE_FMT = "%d-%b-%Y"
 TODAY = datetime.today().date().strftime(DATE_FMT)
 TZ = "Asia/Kolkata"
 CONFIG_FILE = Path(__file__).parent.parent.parent / Path("configs/nse.json")
 NSE_START_TIME, NSE_CLOSE_TIME, TIME_CUTOFF = "0915", "1530", "1600"
 MARKET, COUNTRY = "NSE", "INDIA"
@@ -32,42 +35,58 @@
 NSE_TOP = 1000
 TIMINGS = MarketTimings(
     start_time=NSE_START_TIME,
     close_time=NSE_CLOSE_TIME,
     time_zone=TZ,
     time_cutoff=TIME_CUTOFF,
 )
+TOP_BOTTOM_TYPE = Dict[str, Dict[str, float]]
+ENABLE_TIME = bool(os.getenv("ENABLE_TIME", False))
+ENABLE_PROFILE = bool(os.getenv("ENABLE_PROFILE", False))
 
 
-class NSEConfig(Exchange):
+class NSEConfig(Exchange, NSEFNO):
+    __metaclass__ = UtilityEnabler
 
     def __init__(
         self,
         today: str,
         date_fmt: str = DATE_FMT,
         config: Union[Path, str] = CONFIG_FILE,
         market: str = MARKET,
         country: str = COUNTRY,
         market_timings: MarketTimingType = TIMINGS,
         ticker_mod: Optional[Dict[str, str]] = None,
         log_config: Optional[LoggingType] = None,
+        enable_time: bool = ENABLE_TIME,
+        enable_profile: bool = ENABLE_PROFILE,
     ):
 
         super().__init__(
             today,
             date_fmt,
             config,
             market,
             country,
             self.get_market_holidays,
             market_timings,
             ticker_mod,
             log_config,
         )
 
+    def get_top_bottom(self, nos: int = 5, nse_top: int = 200) -> TOP_BOTTOM_TYPE:
+        symbols = self.get_nse_stocks()
+        get_tops_bottoms = [(i.symbol, i.pct_change, i.diff) for i in symbols[:nse_top]]
+
+        top_nos = nlargest(get_tops_bottoms, nos, key=lambda x: x[1])
+        top_nos = {key: {"pct_change": v1, "diff": v2} for key, v1, v2 in top_nos}
+        small_nos = nsmallest(get_tops_bottoms, nos, key=lambda x: x[1])
+        small_nos = {key: {"pct_change": v1, "diff": v2} for key, v1, v2 in small_nos}
+        return {"top": top_nos, "bottom": small_nos}
+
     @property
     def advanced_header(self) -> Dict[str, str]:
         return self.headers["advanced"]
 
     @property
     def simple_headers(self) -> Dict[str, str]:
         return self.headers["simple"]
@@ -119,14 +138,15 @@
 
         response = self.get_request_api(url, self.advanced_header)
         content = response.json()
         content = None if content == {} else content
 
         return content
 
+    @cache
     def get_eq_bhavcopy(self) -> BytesIO:
         headers = self.advanced_header
         url = self.eq_bhavcopy["url"] + self.eq_bhavcopy["url_params"]
         today = self.working_day.day.as_str
         url = url.format(today)
         result = self.download_data(url, headers)
 
@@ -171,27 +191,57 @@
     def apply_nse_data_preprocessing(self, data) -> pd.DataFrame:
         data = data.loc[:, ~data.columns.str.contains("^Unnamed")]
         data.columns = [i.lower() for i in data.columns]
         data = data.loc[data.series == "EQ", :]
         data = self.apply_mcap(data)
         return data
 
+    @cache
     def get_eq_listed_stocks(self) -> List[str]:
         data = self.get_eq_bhavcopy()
         data = self.apply_nse_data_preprocessing(data)
         return data.symbol.unique().tolist()
 
+    @cache
     def get_eq_stocks_by_mcap(self) -> pd.DataFrame:
 
         data = self.get_eq_bhavcopy()
         data = self.apply_nse_data_preprocessing(data)
 
         return data
 
+    @cache
     def get_nse_stocks(self, nse_top: Optional[int] = None) -> List[str]:
 
         stock_list = self.get_eq_listed_stocks()
 
         if nse_top is None:
             return stock_list
 
         return stock_list[:nse_top]
+
+    @cache
+    def get_all_sectors_industries(self) -> pd.DataFrame:
+        """A Dataframe of All stocks and its relevant sectors/industry."""
+
+        sectors = self.sectoral_indices
+
+        sectoral_data = {
+            sector: self.download_data(url) for sector, url in sectors.items()
+        }
+
+        sectoral_list = list()
+
+        for sector, data in sectoral_data.items():
+            data["index"] = sector
+            sectoral_list.append(data)
+
+        data = pd.concat(sectoral_list)
+
+        return data
+
+    def get_all_etfs(self):
+
+        url = self.main_domain + self.etf_all
+        data = self.get_request_api(url, self.advanced_header).json()
+
+        return data
```

### Comparing `market_generic-0.1.0/trade/nse/nse_stock.py` & `market_generic-0.2.0/trade/nse/stocks/nse_stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 from warnings import simplefilter
 
 import pandas as pd
 from yfinance import Ticker
 
 from trade.calendar import DateObj
 from trade.nse.nse_config import DATE_FMT, NSE_TOP, NSEConfig
-from trade.ticker import StockGenerics
 from trade.utils import operations
 
 MARKET_API_QUOTE_TYPE = Dict[str, Union[list, str, bool]]
 TICKER_MODIFICATION = {"HDFC": "HDFCBANK"}
 simplefilter(action="ignore", category=pd.errors.SettingWithCopyWarning)
 simplefilter(action="ignore", category=RuntimeWarning)
 
 
 @dataclass
-class NSEStock(StockGenerics):
+class NSEStock:
     symbol: str
     dated: str
     tf: Optional[str] = "1d"
 
     def __post_init__(self):
         self._nse_config = NSEConfig(self.dated)
 
         if self.symbol in TICKER_MODIFICATION.keys():
             self.symbol = TICKER_MODIFICATION[self.symbol]
 
+        self.symbol = self.symbol.upper()
         self._yfsymbol = self._nse_config.adjust_yfin_ticker_by_market(self.symbol)
         self.get_curr_bhav()
         self._curr_ohlc = {
             "open": self.open,
             "low": self.low,
             "high": self.high,
             "close": self.close,
@@ -53,14 +53,18 @@
 
     def __str__(self):
         return self.symbol
 
     def __eq__(self, other):
         return self.symbol == other
 
+    @property
+    def is_fno(self) -> bool:
+        return self.symbol in self.get_fno_stocks
+
     @cached_property
     def get_meta_data(self) -> MARKET_API_QUOTE_TYPE:
         return self._nse_config.get_equity_meta(self.symbol)
 
     @property
     def ticker(self) -> Ticker:
         return self._nse_config.yf.Ticker(self._yfsymbol)
```

### Comparing `market_generic-0.1.0/trade/ticker/api_config.py` & `market_generic-0.2.0/trade/exchange/api_config.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/ticker/market.py` & `market_generic-0.2.0/trade/exchange/market.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 from trade.calendar import MarketCalendar, MarketHolidayType, MarketTimingType
-from trade.ticker.api_config import APIConfig
-from trade.ticker.yf import YFinance
+from trade.exchange.api_config import APIConfig
+from trade.exchange.yf import YFinance
 from trade.utils import DownloadTools, Logger, LoggingType
 
 
 @dataclass
 class ExchangeArgs:
     today: str
     date_fmt: str
```

### Comparing `market_generic-0.1.0/trade/ticker/yf.py` & `market_generic-0.2.0/trade/exchange/yf.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/utils/df_market_utils.py` & `market_generic-0.2.0/trade/utils/df_market_utils.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/utils/gsheet_util.py` & `market_generic-0.2.0/trade/utils/gsheet_util.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/utils/html_parsing.py` & `market_generic-0.2.0/trade/utils/html_parsing.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/utils/network_tools.py` & `market_generic-0.2.0/trade/utils/network_tools.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/utils/op_utils.py` & `market_generic-0.2.0/trade/utils/op_utils.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.1.0/trade/utils/telegram_api.py` & `market_generic-0.2.0/trade/utils/telegram_api.py`

 * *Files identical despite different names*

