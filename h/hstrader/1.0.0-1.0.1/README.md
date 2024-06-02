# Comparing `tmp/hstrader-1.0.0.tar.gz` & `tmp/hstrader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstrader-1.0.0.tar", max compression
+gzip compressed data, was "hstrader-1.0.1.tar", max compression
```

## Comparing `hstrader-1.0.0.tar` & `hstrader-1.0.1.tar`

### file list

```diff
@@ -1,68 +1,36 @@
--rw-r--r--   0        0        0       81 2024-05-28 08:57:47.758220 hstrader-1.0.0/hstrader/__init__.py
--rw-r--r--   0        0        0       37 2024-05-28 08:57:47.762220 hstrader-1.0.0/hstrader/config/__init__.py
--rw-r--r--   0        0        0      227 2024-05-28 08:57:47.762220 hstrader-1.0.0/hstrader/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3783 2024-05-28 08:57:47.762220 hstrader-1.0.0/hstrader/config/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     2772 2024-05-28 08:57:47.762220 hstrader-1.0.0/hstrader/config/config.py
--rw-r--r--   0        0        0       62 2024-05-28 08:57:47.766220 hstrader-1.0.0/hstrader/helpers/__init__.py
--rw-r--r--   0        0        0      253 2024-05-28 08:57:47.766220 hstrader-1.0.0/hstrader/helpers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     6315 2024-05-28 08:57:47.766220 hstrader-1.0.0/hstrader/helpers/__pycache__/http.cpython-310.pyc
--rw-r--r--   0        0        0      552 2024-05-28 08:57:47.766220 hstrader-1.0.0/hstrader/helpers/__pycache__/user_agent.cpython-310.pyc
--rw-r--r--   0        0        0     6425 2024-05-28 08:57:47.766220 hstrader-1.0.0/hstrader/helpers/__pycache__/ws.cpython-310.pyc
--rw-r--r--   0        0        0     6566 2024-05-28 08:57:47.766220 hstrader-1.0.0/hstrader/helpers/http.py
--rw-r--r--   0        0        0      359 2024-05-28 08:57:47.770220 hstrader-1.0.0/hstrader/helpers/user_agent.py
--rw-r--r--   0        0        0     6007 2024-05-28 08:57:47.770220 hstrader-1.0.0/hstrader/helpers/ws.py
--rw-r--r--   0        0        0      218 2024-05-28 08:57:47.770220 hstrader-1.0.0/hstrader/hstrader/__init__.py
--rw-r--r--   0        0        0      442 2024-05-28 08:57:47.770220 hstrader-1.0.0/hstrader/hstrader/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3021 2024-05-28 08:57:47.770220 hstrader-1.0.0/hstrader/hstrader/__pycache__/hstrader.cpython-310.pyc
--rw-r--r--   0        0        0     3175 2024-05-28 08:57:47.770220 hstrader-1.0.0/hstrader/hstrader/hstrader.py
--rw-r--r--   0        0        0      243 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__init__.py
--rw-r--r--   0        0        0      374 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2656 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/account.cpython-310.pyc
--rw-r--r--   0        0        0      651 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/auth.cpython-310.pyc
--rw-r--r--   0        0        0      435 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1338 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/base_response.cpython-310.pyc
--rw-r--r--   0        0        0     1557 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/deal.cpython-310.pyc
--rw-r--r--   0        0        0     6026 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/enums.cpython-310.pyc
--rw-r--r--   0        0        0      880 2024-05-28 08:57:47.774220 hstrader-1.0.0/hstrader/models/__pycache__/events.cpython-310.pyc
--rw-r--r--   0        0        0      577 2024-05-28 08:57:47.778220 hstrader-1.0.0/hstrader/models/__pycache__/market.cpython-310.pyc
--rw-r--r--   0        0        0     4465 2024-05-28 08:58:27.566367 hstrader-1.0.0/hstrader/models/__pycache__/order.cpython-310.pyc
--rw-r--r--   0        0        0     2412 2024-05-28 08:57:47.778220 hstrader-1.0.0/hstrader/models/__pycache__/position.cpython-310.pyc
--rw-r--r--   0        0        0     2608 2024-05-28 08:57:47.778220 hstrader-1.0.0/hstrader/models/__pycache__/symbol.cpython-310.pyc
--rw-r--r--   0        0        0     1261 2024-05-28 08:58:30.086376 hstrader-1.0.0/hstrader/models/__pycache__/ws.cpython-310.pyc
--rw-r--r--   0        0        0     2015 2024-05-28 08:57:47.782220 hstrader-1.0.0/hstrader/models/account.py
--rw-r--r--   0        0        0      318 2024-05-28 08:57:47.782220 hstrader-1.0.0/hstrader/models/auth.py
--rw-r--r--   0        0        0      154 2024-05-28 08:57:47.782220 hstrader-1.0.0/hstrader/models/base.py
--rw-r--r--   0        0        0      764 2024-05-28 08:57:47.782220 hstrader-1.0.0/hstrader/models/base_response.py
--rw-r--r--   0        0        0     1079 2024-05-28 08:57:47.782220 hstrader-1.0.0/hstrader/models/deal.py
--rw-r--r--   0        0        0     1163 2024-05-28 08:57:47.782220 hstrader-1.0.0/hstrader/models/deals.py
--rw-r--r--   0        0        0     3282 2024-05-28 08:57:47.782220 hstrader-1.0.0/hstrader/models/enums.py
--rw-r--r--   0        0        0      980 2024-05-28 08:57:47.786220 hstrader-1.0.0/hstrader/models/events.py
--rw-r--r--   0        0        0      229 2024-05-28 08:57:47.786220 hstrader-1.0.0/hstrader/models/market.py
--rw-r--r--   0        0        0     4212 2024-05-28 08:57:47.786220 hstrader-1.0.0/hstrader/models/order.py
--rw-r--r--   0        0        0     1844 2024-05-28 08:57:47.786220 hstrader-1.0.0/hstrader/models/position.py
--rw-r--r--   0        0        0     2039 2024-05-28 08:57:47.786220 hstrader-1.0.0/hstrader/models/symbol.py
--rw-r--r--   0        0        0      534 2024-05-28 08:57:47.786220 hstrader-1.0.0/hstrader/models/ws.py
--rw-r--r--   0        0        0      267 2024-05-28 08:57:47.786220 hstrader-1.0.0/hstrader/services/__init__.py
--rw-r--r--   0        0        0      520 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1055 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/account.cpython-310.pyc
--rw-r--r--   0        0        0     2674 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/auth.cpython-310.pyc
--rw-r--r--   0        0        0     1107 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/deal.cpython-310.pyc
--rw-r--r--   0        0        0     3015 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/market.cpython-310.pyc
--rw-r--r--   0        0        0     2696 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/order.cpython-310.pyc
--rw-r--r--   0        0        0     2286 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/position.cpython-310.pyc
--rw-r--r--   0        0        0     1796 2024-05-28 08:57:47.790220 hstrader-1.0.0/hstrader/services/__pycache__/symbol.cpython-310.pyc
--rw-r--r--   0        0        0     1168 2024-05-28 08:57:47.794220 hstrader-1.0.0/hstrader/services/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0        0        0     3942 2024-05-28 08:58:44.538428 hstrader-1.0.0/hstrader/services/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    12083 2024-05-28 08:58:46.742437 hstrader-1.0.0/hstrader/services/__pycache__/ws.cpython-310.pyc
--rw-r--r--   0        0        0      597 2024-05-28 08:57:47.794220 hstrader-1.0.0/hstrader/services/account.py
--rw-r--r--   0        0        0     2597 2024-05-28 08:57:47.794220 hstrader-1.0.0/hstrader/services/auth.py
--rw-r--r--   0        0        0      646 2024-05-28 08:57:47.794220 hstrader-1.0.0/hstrader/services/deal.py
--rw-r--r--   0        0        0     2892 2024-05-28 08:57:47.794220 hstrader-1.0.0/hstrader/services/market.py
--rw-r--r--   0        0        0     2650 2024-05-28 08:57:47.794220 hstrader-1.0.0/hstrader/services/order.py
--rw-r--r--   0        0        0     2263 2024-05-28 08:57:47.798220 hstrader-1.0.0/hstrader/services/position.py
--rw-r--r--   0        0        0     1295 2024-05-28 08:57:47.798220 hstrader-1.0.0/hstrader/services/symbol.py
--rw-r--r--   0        0        0     1408 2024-05-28 08:57:47.798220 hstrader-1.0.0/hstrader/services/urls.py
--rw-r--r--   0        0        0     4218 2024-05-28 08:57:47.798220 hstrader-1.0.0/hstrader/services/utils.py
--rw-r--r--   0        0        0    11700 2024-05-28 08:57:47.798220 hstrader-1.0.0/hstrader/services/ws.py
--rw-r--r--   0        0        0      354 2024-05-28 09:11:24.648897 hstrader-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 hstrader-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2463 2024-06-02 07:36:55.729379 hstrader-1.0.1/README.md
+-rw-r--r--   0        0        0       81 2024-05-28 08:57:47.758220 hstrader-1.0.1/hstrader/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-28 08:57:47.762220 hstrader-1.0.1/hstrader/config/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-28 08:57:47.762220 hstrader-1.0.1/hstrader/config/config.py
+-rw-r--r--   0        0        0       62 2024-05-28 08:57:47.766220 hstrader-1.0.1/hstrader/helpers/__init__.py
+-rw-r--r--   0        0        0     6566 2024-05-28 08:57:47.766220 hstrader-1.0.1/hstrader/helpers/http.py
+-rw-r--r--   0        0        0      359 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/helpers/user_agent.py
+-rw-r--r--   0        0        0     6007 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/helpers/ws.py
+-rw-r--r--   0        0        0      218 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/hstrader/__init__.py
+-rw-r--r--   0        0        0     3175 2024-05-28 08:57:47.770220 hstrader-1.0.1/hstrader/hstrader/hstrader.py
+-rw-r--r--   0        0        0      243 2024-05-28 08:57:47.774220 hstrader-1.0.1/hstrader/models/__init__.py
+-rw-r--r--   0        0        0     2015 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/account.py
+-rw-r--r--   0        0        0      318 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/auth.py
+-rw-r--r--   0        0        0      154 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/base.py
+-rw-r--r--   0        0        0      764 2024-05-28 08:57:47.782220 hstrader-1.0.1/hstrader/models/base_response.py
+-rw-r--r--   0        0        0     1182 2024-06-02 07:43:18.430213 hstrader-1.0.1/hstrader/models/deal.py
+-rw-r--r--   0        0        0     3311 2024-06-02 07:44:04.426313 hstrader-1.0.1/hstrader/models/enums.py
+-rw-r--r--   0        0        0      980 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/events.py
+-rw-r--r--   0        0        0      229 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/market.py
+-rw-r--r--   0        0        0     4212 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/order.py
+-rw-r--r--   0        0        0     1894 2024-06-02 08:00:30.248551 hstrader-1.0.1/hstrader/models/position.py
+-rw-r--r--   0        0        0     2068 2024-06-02 07:44:06.382317 hstrader-1.0.1/hstrader/models/symbol.py
+-rw-r--r--   0        0        0      534 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/models/ws.py
+-rw-r--r--   0        0        0      267 2024-05-28 08:57:47.786220 hstrader-1.0.1/hstrader/services/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/account.py
+-rw-r--r--   0        0        0     2597 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/auth.py
+-rw-r--r--   0        0        0      646 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/deal.py
+-rw-r--r--   0        0        0     2892 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/market.py
+-rw-r--r--   0        0        0     2650 2024-05-28 08:57:47.794220 hstrader-1.0.1/hstrader/services/order.py
+-rw-r--r--   0        0        0     2263 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/position.py
+-rw-r--r--   0        0        0     1295 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/symbol.py
+-rw-r--r--   0        0        0     1408 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/urls.py
+-rw-r--r--   0        0        0     4218 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/utils.py
+-rw-r--r--   0        0        0    11700 2024-05-28 08:57:47.798220 hstrader-1.0.1/hstrader/services/ws.py
+-rw-r--r--   0        0        0      375 2024-06-02 08:02:35.116705 hstrader-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 hstrader-1.0.1/PKG-INFO
```

### Comparing `hstrader-1.0.0/hstrader/config/config.py` & `hstrader-1.0.1/hstrader/config/config.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/helpers/http.py` & `hstrader-1.0.1/hstrader/helpers/http.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/helpers/ws.py` & `hstrader-1.0.1/hstrader/helpers/ws.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/hstrader/hstrader.py` & `hstrader-1.0.1/hstrader/hstrader/hstrader.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/models/account.py` & `hstrader-1.0.1/hstrader/models/account.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/models/base_response.py` & `hstrader-1.0.1/hstrader/models/base_response.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/models/deal.py` & `hstrader-1.0.1/hstrader/models/deal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from .base import BaseModel
-from .enums import *
-
+from .enums import (
+    SideType,
+    ReasonType,
+    ChannelType,
+    DirectionType,
+    DealStatus,
+    CreationMethod,
+)
 
 
 class Deal(BaseModel):
 
     commission: float = None
     digits: int = None
     position_id: int = None
```

### Comparing `hstrader-1.0.0/hstrader/models/deals.py` & `hstrader-1.0.1/hstrader/models/symbol.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,78 @@
 from .base import BaseModel
-from .enums import *
-from typing import Union
+from .enums import (
+    ExecutionMode,
+    SwapType,
+    CalcType,
+    SymbolStatus,
+    TradeLevel,
+    FillPolicy,
+)
 
-from .account import Account
-from .symbol import Symbol
 
+class Symbol(BaseModel):
 
-class Deal(BaseModel):
-    account: Account = None
-    account_id: int = None
-    channel: int = None
-    close_price: float = None
-    closed_volume: float = None
-    comment: str = None
-    commission: float = None
-    contract_size: float = None
-    created_at: int = None
-    created_by: int = None
-    creation_method: int = None
-    digits: float = None
-    digits_currency: float = None
-    direction: int = None
-    external_id: str = None
-    external_price: str = None
-    external_volume: str = None
     id: int = None
-    market_ask: float = None
-    market_bid: float = None
-    market_last: float = None
-    open_price: float = None
-    order_id: int = None
-    position_id: int = None
-    profit: float = None
-    reason: int = None
-    script_id: int = None
-    side: int = None
-    status: int = None
-    stop_loss: float = None
-    swap: float = None
-    symbol: Symbol = None
-    symbol_id: int = None
-    take_profit: float = None
-    updated_at: int = None
-    updated_by: int = None
+    symbol: str = None
+    isin: str = None
+    desc: str = None
+    base_currency: str = None
+    quote_currency: str = None
+    symbol_scale: int = None
+    quote_scale: int = None
+    broker_fee: float = None
+    maker_fee: float = None
+    leverage: int = None
+    margin_flags: int = None
+    margin_initial: float = None
+
+    margin_maintenance: float = None
+    margin_buy: float = None
+    margin_sell: float = None
+    buy_limit: float = None
+    sell_limit: float = None
+    buy_stop_limit: float = None
+    sell_stop_limit: float = None
+    sell_stop: float = None
+    buy_stop: float = None
+    maintenance_margin_buy: float = None
+    maintenance_margin_sell: float = None
+    maintenance_buy_limit: float = None
+    maintenance_sell_limit: float = None
+    maintenance_buy_stop: float = None
+    maintenance_sell_stop: float = None
+    maintenance_buy_stop_limit: float = None
+    maintenance_sell_stop_limit: float = None
+    enabled: bool = None
+    trade_level: TradeLevel = None
+    execution: ExecutionMode = None
+    gtc: bool = None
+    filling: FillPolicy = None
+    expiration: str = None
+    orders: str = None
+    min_value: float = None
+    max_value: float = None
+    step: float = None
+    swap_mode: int = None
+    swap_type: SwapType = None
+    swap_long: float = None
+    swap_short: float = None
+    digits: int = None
+    spread: float = None
+    spread_balance: float = None
+    stop_level: float = None
+    chart_mode: int = None
+    calculation: CalcType = None
+    contract_size: int = None
+    quote_sessions: str = None
+    trade_sessions: str = None
+    status: SymbolStatus = None
+    last_bid: float = None
+    last_ask: float = None
+    open: float = None
+    close: float = None
+    high_bid: float = None
+    low_bid: float = None
+    high_ask: float = None
+    low_ask: float = None
     volume: float = None
+    ts: int = None
```

### Comparing `hstrader-1.0.0/hstrader/models/enums.py` & `hstrader-1.0.1/hstrader/models/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,36 +123,36 @@
 class ExecutionMode(IntEnum):
     INSTANCE = 0
     REQUEST = 1
     EXECUTE = 2
     EXCHANGE = 3
 
 
-class Swaptype(IntEnum):
+class SwapType(IntEnum):
     POINTS = 0
     BASE_CURRENCY = 1
     MARGIN_CURRENCY = 2
     DEPOSIT_CURRENCY = 3
     CURRENT_PRICE = 4
     OPEN_PRICE = 5
     REOPEN_CLOSE = 6
     REOPEN_BID = 7
 
 
-
 class CalcType(IntEnum):
 
     FOREX = 0
     FOREX_NO_LEVERAGE = 1
     CONTRACTS_EXCHANGE_STOCKS = 2
-    CONTRACTS_LEVERAGE = 3 
+    CONTRACTS_LEVERAGE = 3
     CONTRACTS_INDEX = 4
     FUTURES_EXCHANGE = 5
     EXCHANGE_BONDS = 6
 
+
 class SymbolStatus(IntEnum):
 
     ENABLED = 0
     DISABLED = 1
     SESSIONS_CLOSED = 2
     TRADE_CLOSED_QUOTE_OPENED = 3
     TRADE_OPENED_QUOTE_CLOSED = 4
@@ -160,26 +160,28 @@
     TIME_LIMIT_EXPIRED = 6
 
 
 class TradeLevel(IntEnum):
     FULL = 0
     BUY = 1
     SELL = 2
+    CLOSE = 3
+    DISABLED = 4
 
 
 class AccountStatus(IntEnum):
     READONLY = 0
     PENDING = 1
     ACTIVE = 2
     REJECTED = 3
     LIQUIDATION = 4
     LIQUIDATED = 5
 
 
-class TradeType (IntEnum):
+class TradeType(IntEnum):
     REAL = 0
     DEMO = 1
 
 
 class AccountType(IntEnum):
 
     CLIENT = 0
```

### Comparing `hstrader-1.0.0/hstrader/models/events.py` & `hstrader-1.0.1/hstrader/models/events.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/models/order.py` & `hstrader-1.0.1/hstrader/models/order.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/models/position.py` & `hstrader-1.0.1/hstrader/models/position.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .base import BaseModel
 from .enums import PositionStatus, SideType
-
+from typing import Union
 
 
 class Position(BaseModel):
 
     volume: float = None
     digits_currency: float = None
     side: SideType = None
-    take_profit: float = None
+    take_profit: Union[float, None] = None
     contract_size: float = None
     created_by: int = None
-    stop_loss: float = None
+    stop_loss: Union[float, None] = None
     updated_at: int = None
     updated_by: int = None
     account_id: int = None
     open_price: float = None
     created_at: int = None
     digits: float = None
     id: int = None
```

### Comparing `hstrader-1.0.0/hstrader/models/ws.py` & `hstrader-1.0.1/hstrader/models/ws.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/account.py` & `hstrader-1.0.1/hstrader/services/account.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/auth.py` & `hstrader-1.0.1/hstrader/services/auth.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/deal.py` & `hstrader-1.0.1/hstrader/services/deal.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/market.py` & `hstrader-1.0.1/hstrader/services/market.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/order.py` & `hstrader-1.0.1/hstrader/services/order.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/position.py` & `hstrader-1.0.1/hstrader/services/position.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/symbol.py` & `hstrader-1.0.1/hstrader/services/symbol.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/urls.py` & `hstrader-1.0.1/hstrader/services/urls.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/utils.py` & `hstrader-1.0.1/hstrader/services/utils.py`

 * *Files identical despite different names*

### Comparing `hstrader-1.0.0/hstrader/services/ws.py` & `hstrader-1.0.1/hstrader/services/ws.py`

 * *Files identical despite different names*

