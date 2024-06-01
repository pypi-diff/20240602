# Comparing `tmp/mktdata-0.0.7.tar.gz` & `tmp/mktdata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktdata-0.0.7.tar", last modified: Wed May 29 23:50:15 2024, max compression
+gzip compressed data, was "mktdata-0.0.8.tar", last modified: Sat Jun  1 22:44:52 2024, max compression
```

## Comparing `mktdata-0.0.7.tar` & `mktdata-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 23:50:15.747355 mktdata-0.0.7/
--rw-rw-rw-   0        0        0     7618 2024-05-29 23:50:15.747355 mktdata-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-29 23:50:15.721421 mktdata-0.0.7/mktdata/
--rw-rw-rw-   0        0        0        0 2024-05-29 23:50:02.000000 mktdata-0.0.7/mktdata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 23:50:15.734563 mktdata-0.0.7/mktdata/embeddings/
--rw-rw-rw-   0        0        0        0 2024-05-25 03:59:58.000000 mktdata-0.0.7/mktdata/embeddings/__init__.py
--rw-rw-rw-   0        0        0     8061 2024-05-29 21:36:23.000000 mktdata-0.0.7/mktdata/embeddings/technical_embeds.py
-drwxrwxrwx   0        0        0        0 2024-05-29 23:50:15.738277 mktdata-0.0.7/mktdata/feeds/
--rw-rw-rw-   0        0        0        0 2024-05-26 03:57:33.000000 mktdata-0.0.7/mktdata/feeds/__init__.py
--rw-rw-rw-   0        0        0        8 2024-05-26 04:43:41.000000 mktdata-0.0.7/mktdata/feeds/helpers.py
--rw-rw-rw-   0        0        0    10011 2024-05-28 04:01:01.000000 mktdata-0.0.7/mktdata/feeds/option_data.py
--rw-rw-rw-   0        0        0     3474 2024-05-28 04:15:01.000000 mktdata-0.0.7/mktdata/feeds/starter.py
--rw-rw-rw-   0        0        0     6630 2024-05-29 13:22:09.000000 mktdata-0.0.7/mktdata/feeds/stock_data.py
--rw-rw-rw-   0        0        0    32559 2024-05-29 23:49:15.000000 mktdata-0.0.7/mktdata/feeds/technicals.py
-drwxrwxrwx   0        0        0        0 2024-05-29 23:50:15.739282 mktdata-0.0.7/mktdata/models/
--rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.7/mktdata/models/__init__.py
--rw-rw-rw-   0        0        0    31983 2024-05-29 23:49:38.000000 mktdata-0.0.7/mktdata/optionsdata.py
--rw-rw-rw-   0        0        0    16394 2024-05-29 23:49:08.000000 mktdata-0.0.7/mktdata/stock_data.py
-drwxrwxrwx   0        0        0        0 2024-05-29 23:50:15.732563 mktdata-0.0.7/mktdata.egg-info/
--rw-rw-rw-   0        0        0     7618 2024-05-29 23:50:15.000000 mktdata-0.0.7/mktdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-05-29 23:50:15.000000 mktdata-0.0.7/mktdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 23:50:15.000000 mktdata-0.0.7/mktdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4028 2024-05-29 23:50:15.000000 mktdata-0.0.7/mktdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-29 23:50:15.000000 mktdata-0.0.7/mktdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 23:50:15.748356 mktdata-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      375 2024-05-29 23:50:11.000000 mktdata-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.664040 mktdata-0.0.8/
+-rw-rw-rw-   0        0        0     7616 2024-06-01 22:44:52.663041 mktdata-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.581531 mktdata-0.0.8/markets/
+-rw-rw-rw-   0        0        0        0 2024-05-06 15:31:10.000000 mktdata-0.0.8/markets/__init__.py
+-rw-rw-rw-   0        0        0     9789 2024-05-24 12:57:09.000000 mktdata-0.0.8/markets/embeddings.py
+-rw-rw-rw-   0        0        0     2927 2024-05-22 14:18:00.000000 mktdata-0.0.8/markets/imps.py
+-rw-rw-rw-   0        0        0     9304 2024-06-01 22:44:37.000000 mktdata-0.0.8/markets/option_trades.py
+-rw-rw-rw-   0        0        0     2355 2024-05-24 12:19:00.000000 mktdata-0.0.8/markets/stock_trades.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.596531 mktdata-0.0.8/mktdata/
+-rw-rw-rw-   0        0        0        0 2024-05-29 23:50:02.000000 mktdata-0.0.8/mktdata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.623530 mktdata-0.0.8/mktdata/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:59:58.000000 mktdata-0.0.8/mktdata/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     7258 2024-05-31 14:38:08.000000 mktdata-0.0.8/mktdata/embeddings/technical_embeds.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.654534 mktdata-0.0.8/mktdata/feeds/
+-rw-rw-rw-   0        0        0        0 2024-05-26 03:57:33.000000 mktdata-0.0.8/mktdata/feeds/__init__.py
+-rw-rw-rw-   0        0        0        8 2024-05-26 04:43:41.000000 mktdata-0.0.8/mktdata/feeds/helpers.py
+-rw-rw-rw-   0        0        0     7422 2024-05-31 15:02:09.000000 mktdata-0.0.8/mktdata/feeds/option_data.py
+-rw-rw-rw-   0        0        0     3474 2024-05-28 04:15:01.000000 mktdata-0.0.8/mktdata/feeds/starter.py
+-rw-rw-rw-   0        0        0     6630 2024-05-29 13:22:09.000000 mktdata-0.0.8/mktdata/feeds/stock_data.py
+-rw-rw-rw-   0        0        0    32901 2024-05-31 14:54:56.000000 mktdata-0.0.8/mktdata/feeds/technicals.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.655534 mktdata-0.0.8/mktdata/models/
+-rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.8/mktdata/models/__init__.py
+-rw-rw-rw-   0        0        0    31983 2024-05-29 23:49:38.000000 mktdata-0.0.8/mktdata/optionsdata.py
+-rw-rw-rw-   0        0        0    16394 2024-05-29 23:49:08.000000 mktdata-0.0.8/mktdata/stock_data.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.615531 mktdata-0.0.8/mktdata.egg-info/
+-rw-rw-rw-   0        0        0     7616 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4026 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 22:44:52.664040 mktdata-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      375 2024-06-01 22:44:29.000000 mktdata-0.0.8/setup.py
```

### Comparing `mktdata-0.0.7/PKG-INFO` & `mktdata-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktdata
-Version: 0.0.7
+Version: 0.0.8
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
@@ -126,15 +126,15 @@
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: orjson==3.9.10
 Requires-Dist: outcome==1.3.0.post0
 Requires-Dist: overrides==7.4.0
 Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.2.1
+Requires-Dist: pandas==2.2.2
 Requires-Dist: peewee==3.17.0
 Requires-Dist: Pillow==10.1.0
 Requires-Dist: pkginfo==1.9.6
 Requires-Dist: plotly==5.20.0
 Requires-Dist: polygon==1.1.3
 Requires-Dist: polygon-api-client==1.13.3
 Requires-Dist: posthog==3.0.2
@@ -211,14 +211,14 @@
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: uvicorn==0.23.2
 Requires-Dist: waitress==2.1.2
 Requires-Dist: watchfiles==0.21.0
 Requires-Dist: webcolors==1.13
 Requires-Dist: webencodings==0.5.1
 Requires-Dist: websocket-client==1.6.4
-Requires-Dist: websockets==11.0.3
+Requires-Dist: websockets==12.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.14.1
 Requires-Dist: wsproto==1.2.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yfinance==0.2.32
 Requires-Dist: zipp==3.17.0
```

### Comparing `mktdata-0.0.7/mktdata/embeddings/technical_embeds.py` & `mktdata-0.0.8/mktdata/embeddings/technical_embeds.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,123 +9,93 @@
 from fudstop.apis.webull.webull_trading import WebullTrading
 import asyncio
 db = PolygonDatabase(host='localhost', user='chuck', password='fud', port=5432, database='market_data')
 
 import pandas as pd
 
 
-async def rsi_embed(hook, ticker, status, timespan, rsi,underlying_data: dict, db):
+async def rsi_embed(hook, ticker, status, timespan, rsi,underlying_data: dict):
 
     """Sends RSI feeds to discord."""
+    try:
+        webhook = AsyncDiscordWebhook(hook)
+        color = hex_color_dict.get('red') if status == 'oversold' else hex_color_dict.get('green')
+        print(color)
+        embed = DiscordEmbed(title=f"RSI Feed - {ticker} | {timespan}", description=f"# > {ticker} | {status} | {timespan}\n```py\n{ticker} is currently trading with an RSI of {round(float(rsi),2)}.```", color=color)
+        embed.add_embed_field(name='Latest Underlying:', value=f"> Open: **${underlying_data.get('open')[0]}**\n> High: **${underlying_data.get('high')[0]}**\n> Low: **${underlying_data.get('low')[0]}**\n> Close: **${underlying_data.get('close')[0]}**\n> VWAP: **${underlying_data.get('vwap')[0]}**\n\n> Volume: **{underlying_data.get('volume')[0]}**\n> Num Trades: **{underlying_data.get('num_trades')[0]}**")
+        embed.set_footer(text='Implemented by FUDSTOP | Data by Polygon.io', icon_url = os.environ.get('fudstop_logo'))
 
-    webhook = AsyncDiscordWebhook(hook)
-    color = hex_color_dict.get('red') if status == 'oversold' else hex_color_dict.get('green')
-    print(color)
-    embed = DiscordEmbed(title=f"RSI Feed - {ticker} | {timespan}", description=f"# > {ticker} | {status} | {timespan}\n```py\n{ticker} is currently trading with an RSI of {round(float(rsi),2)}.```", color=color)
-    embed.add_embed_field(name='Latest Underlying:', value=f"> Open: **${underlying_data.get('open')[0]}**\n> High: **${underlying_data.get('high')[0]}**\n> Low: **${underlying_data.get('low')[0]}**\n> Close: **${underlying_data.get('close')[0]}**\n> VWAP: **${underlying_data.get('vwap')[0]}**\n\n> Volume: **{underlying_data.get('volume')[0]}**\n> Num Trades: **{underlying_data.get('num_trades')[0]}**")
-    embed.set_footer(text='Implemented by FUDSTOP | Data by Polygon.io', icon_url = os.environ.get('fudstop_logo'))
+        webhook.add_embed(embed)
 
-    webhook.add_embed(embed)
 
-    df = pd.DataFrame(underlying_data)
-    df['ticker'] = ticker
-    df['status'] = status
-    df['timespan'] = timespan
-    df['rsi'] = rsi
-    await db.batch_insert_dataframe(df, table_name='rsi_feed', unique_columns='ticker, timespan, status')
+        await webhook.execute()
+    except Exception as e:
+        print(e)
 
-    await webhook.execute()
 
-
-
-async def macd_embed(hook, type, ticker, timespan, db):
+async def macd_embed(hook, type, ticker, timespan):
     color = hex_color_dict.get('green') if type == 'bullish' else hex_color_dict.get('red')
     webhhook = AsyncDiscordWebhook(hook)
 
     embed = DiscordEmbed(title=f"MACD {type} - {ticker} | {timespan}", description=f"```py\n{ticker}'s MACD is about to cross {type} on the {timespan} timespan.```", color=color)
     embed.set_footer(text='Implemented by FUDSTOP | data by Polygon.io', icon_url = os.environ.get('fudstop_logo'))
     embed.set_timestamp()
     webhhook.add_embed(embed)
 
-    data_dict = { 
-        'ticker': ticker,
-        'type': type,
-        'timespan': timespan,
-
-    }
-
-    df=  pd.DataFrame(data_dict)
 
-    await db.batch_insert_dataframe(df, table_name='macd_feed', unique_columns='ticker, timespan, type')
+    
 
     await webhhook.execute()
+    #await db.batch_insert_dataframe(df, table_name='macd_feed', unique_columns='ticker, timespan, type')
+#
 
 
 
-async def cost_dist_embed(hook, status, ticker, profit_ratio, db):
+async def cost_dist_embed(hook, status, ticker, profit_ratio):
     color = hex_color_dict.get('green') if status == 'bullish signal' else hex_color_dict.get('red')
     webhhook = AsyncDiscordWebhook(hook)
 
     embed = DiscordEmbed(title=f"PLAYERS PROFITING {status} - {ticker} | {profit_ratio}%", description=f"```py\n{profit_ratio}% of players are currently profiting for {ticker}. This is a {status} because the price is far from the average, which could lead to a sell-off in the near-term. Use with other metrics.```", color=color)
     embed.set_timestamp()
     webhhook.add_embed(embed)
-    data_dict = { 
-        'ticker': ticker,
-        'status': status,
-        'profit_ratio': profit_ratio
-    }
-    df = pd.DataFrame(data_dict, index=[0])
-    await db.batch_insert_dataframe(df, table_name='cost_feed', unique_columns='ticker, status, profit_ratio')
+
     await webhhook.execute()
+   # await db.batch_insert_dataframe(df, table_name='cost_feed', unique_columns='ticker, status, profit_ratio')
 
 
 
-async def td9_embed(hook, timespan, status, ticker, df, db):
+async def td9_embed(hook, timespan, status, ticker, df):
     color = hex_color_dict.get('green') if status == 'bullish_td9' else hex_color_dict.get('red')
     webhhook = AsyncDiscordWebhook(hook)
 
     embed = DiscordEmbed(title=f"{status} - {ticker} | {timespan} TD9", description=f"```py\n{df}```", color=color)
     embed.add_embed_field(name=f"TD9", value='> The TD9 is a reversal indicator. Pair with other indicators for increased likelihood of reversal - such as RSI.')
     embed.set_footer(icon_url=os.environ.get('fudstop_logo'), text='Implemented by FUDSTOP')
     embed.set_timestamp()
     webhhook.add_embed(embed)
 
-    data_dict = { 
-        'ticker': ticker,
-        'timespan': timespan,
-        'status': status,
 
-    }
-    df = pd.DataFrame(data_dict, index=[0])
 
-    await db.batch_insert_dataframe(df, table_name='td9_feed', unique_columns='ticker, timespan, status')
     await webhhook.execute()
+    #await db.batch_insert_dataframe(df, table_name='td9_feed', unique_columns='ticker, timespan, status')
 
 
 
-async def candlestick_embed(hook, timespan, status, ticker, df, db):
+async def candlestick_embed(hook, timespan, status, ticker, df):
     color = hex_color_dict.get('green') if 'bullish' in status else hex_color_dict.get('red')
     webhhook = AsyncDiscordWebhook(hook)
 
     embed = DiscordEmbed(title=f"{status} - {ticker} | {timespan}", description=f"```py\n{df}```", color=color)
     embed.add_embed_field(name=f"{status}", value='> TO DO.')
     embed.set_footer(icon_url=os.environ.get('fudstop_logo'), text='Implemented by FUDSTOP')
     embed.set_timestamp()
     webhhook.add_embed(embed)
 
-    data_dict = { 
-        'ticker': ticker,
-        'timespan': timespan,
-        'pattern': status,
-
-
-    }
-    df = pd.DataFrame(data_dict, index=[0])
-    await db.batch_insert_dataframe(df, table_name='candle_feed', unique_columns='ticker, timespan, pattern')
     await webhhook.execute()
+   # await db.batch_insert_dataframe(df, table_name='candle_feed', unique_columns='ticker, timespan, pattern')
 
 
 
 
 async def option_embed(hook,ticker, strike, cp, expiry, volume, oi, condition, price, bid, mid, ask, chg_pct):
     color = hex_color_dict.get('green') if 'call' in cp else hex_color_dict.get('red')
     webhhook = AsyncDiscordWebhook(hook)
```

### Comparing `mktdata-0.0.7/mktdata/feeds/starter.py` & `mktdata-0.0.8/mktdata/feeds/starter.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.7/mktdata/feeds/stock_data.py` & `mktdata-0.0.8/mktdata/feeds/stock_data.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.7/mktdata/feeds/technicals.py` & `mktdata-0.0.8/mktdata/feeds/technicals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import os 
 from dotenv import load_dotenv
 load_dotenv()
+import os
+import sys
+
+parent_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+sys.path.append(parent_dir)
+
 import asyncio
 import httpx
 from fudstop.apis.helpers import format_large_numbers_in_dataframe
 from datetime import datetime, timedelta
 from embeddings.technical_embeds import rsi_embed, macd_embed, td9_embed, candlestick_embed, option_embed
 from mktdata.stock_data import StockData
 from fudstop.apis.polygonio.async_polygon_sdk import Polygon
@@ -15,34 +21,35 @@
 import pandas as pd
 import time
 import logging
 
 logging.basicConfig(level=logging.INFO)
 poly = Polygon(host='localhost', user='chuck', password='fud', port=5432, database='market_data')
 from .starter import Starter
-f2osob_day="https://discord.com/api/webhooks/1206934896304726087/8ZBH7ZOTi3xr7ouk8SxYx1qccVXBvaBdWQW57hE7ZRjx943oQbcL-efGdZ45ad8jx7jn"
-f2osob_hour="https://discord.com/api/webhooks/1206935054069272586/fCwEere6jiLvIHmSQGWJTsT7wcH26zxxdzFrHo58Uc00hdEdiDZ2x6ZV13PPm8WT1-bW"
-f2osob_week="https://discord.com/api/webhooks/1206935164337389621/-V0EQ9GOWD6qhcxi7sPcfL4blKd81250E4b0f8AMo5EafZjPKmdBPmFt15IasRdEzSTl"
-f2osob_month="https://discord.com/api/webhooks/1206935260433223710/7UHtfwnR8y08YlAQyJzPGtpMc3Xi7xeXgyTRvbvKGMoAuwnNBP9024ZR7A6H9Vx2GljX"
-f2osob_minute="https://discord.com/api/webhooks/1242496945910579322/wf81VQSnLH3I31wLJA4u6yS8RovlWfRlg1cndodr39Ggy_Piyg_67v9C1a6KViwuRtDd"
+f2osob_day="https://discord.com/api/webhooks/1246111093781299231/72hk_LHDwk_DgEIKYEBB456i3_MqGlBUwNbfCcNl8SrW_nWtT6s8tb-NL5pU1bu-a0vr"
+f2osob_hour="https://discord.com/api/webhooks/1246111034595475577/0OKZyHKR3BZOJMJU1frZzEGoCszngOF4bAteYQkNdkspD0EQseuRuc_EZ8-3O8rkYc6X"
+f2osob_week="https://discord.com/api/webhooks/1246110960956215439/q-VQZVak6pbhlLUB-FOckqfuDbX98-8VayyhrQDissaF5Nwbi8789jXROUYknySu7LlP"
+f2osob_month="https://discord.com/api/webhooks/1246110805871824936/mvIQAkWc1MaQSdACXXB-8xIZevbVZpPKMf4w00oMvTn2vBg5XazFaZZTRnJpY7yNKl4O"
+f2osob_minute="https://discord.com/api/webhooks/1246111163507540029/xSAQaGHjPdErKUXcTisIc8oQ2GB77v3sYDTZpjRxrWk0SXScfwyRPD-b12Vye3JcHkuN"
 macd_minute="https://discord.com/api/webhooks/1162153390059561072/cWyUfeWO7-dtKmuQ16jQbtPv-4Cbc64Gyfp6mfjobXLQaFrKWsT8qxePs7-6veNSp_w2"
-macd_hour="https://discord.com/api/webhooks/1207036388999037009/qMP6OLR2MbuUvwCUUAWgvrdxOGcWqpVEBBQe642s3955ywc-O_sdrkygAnSjfCi9_c8t"
-macd_day="https://discord.com/api/webhooks/1207036286011973632/Tg6EHghgPCMBpeIDT4e5GHN6QHokiZluUuIox2L5ZBRwheT-EjmXd59T5rGIziMHB_iz"
-macd_week="https://discord.com/api/webhooks/1207036457668321280/rC3jFaSf6-xdzImejX2hxYPPFl1jHriY3GyluQWpp-6UzNg9tivvluoLvltxSRbAD1e0"
-macd_month="https://discord.com/api/webhooks/1207036529432862740/-GeT46BidLSbfE79aYaJy8SJzZoL5kRVRI_Cn5mrLKLBEHXOBPsoQnHue9aRpwtxizi0"
-engulf_day="https://discord.com/api/webhooks/1212598193032925194/Kp8veREPWv3ZEsGVMkb8zaQ-IVCxA4vwZHFNb0Aqf4hJ3zyI5I6TorKIm6fo8cpuf7TS"
-engulf_week="https://discord.com/api/webhooks/1212598195935248394/VGU_pco8XR7WjqJ99_XdLeIeECHPZyzEGra6SIFITXiI-FlVv_5vB-XCmlDCpNJwz82F"
-engulf_month="https://discord.com/api/webhooks/1212598198057828424/YNJHrw3H6xG2Q_fBTgtGcPSf_Uz1SifxprVv_OAfEugZx4N650gwRXdVnNx_eqPhRDsv"
-engulf_hour="https://discord.com/api/webhooks/1212598201216143401/8YCDXc7Pwd_f51kPHt06GJtJp5baiKOu_KZFebWBeSxZTvX_OfAaBRY8BTj5GtZIJ2Wo"
-engulf_4hour="https://discord.com/api/webhooks/1212598203661291610/mKf3eJAhKbDQ5kt1surt4Bl0mZTrA0MrmLfDADgpy8Xfz5MmnSCySVlbw3lzn9jmY1UN"
+macd_hour="https://discord.com/api/webhooks/1246111457171472476/8KDDX-oMc_saD7MXv3J71guBOqB7P8FQD7qN74gl19X0ZGI0J_2QGPVISpHI1xJxp8Hw"
+macd_day="https://discord.com/api/webhooks/1246111546388516955/80rkahh-swRi5skU-fz8uUuLws9uSqgL3sYq0BuvbojvqpxitJAohFpaKe1bNA2ByTrv"
+macd_week="https://discord.com/api/webhooks/1246111765511671808/psmQz680iEEcb7Glv-LK79klPsM_RfCc-haI-lbZ50d55JGhA8HLosEkL4J1OovtNfLf"
+macd_month="https://discord.com/api/webhooks/1246111837670346823/FenFfGUoPZ1AoWdp1aFvvWRuicfFjEpCsK9UTko9WwHuKnxkHAlURzIGFNSlaqZ6o7qb"
+engulf_day="https://discord.com/api/webhooks/1246113250743947327/NwID5I-nz71A_EALy4Iua2rOkY105r7T-y7RZ3yTBWg_0C-2s4yWCX8c0HK9TKIuxpiW"
+engulf_week="https://discord.com/api/webhooks/1246113175548465233/L8VVFWYBFbEDGApYWj_qBss5yNcGyMdkTn_Ijl0tsMM4doLAT0d_cTHuzl3tWFORlBdZ"
+engulf_month="https://discord.com/api/webhooks/1246113081432604763/JumLEhLkCJMLKh0zMA_zkYh4EuwLm24Q1nilnxEWfWrtZrOV3xNdWuBR5ipLRvTAVmSR"
+engulf_hour="https://discord.com/api/webhooks/1246113376770199563/XPr5nEz-xJiwRDfVMnRcf-XTKQlAarcsqyU3Za1eLCMfZ7hEx-Dfkfz9ShzbPwkWFi_y"
+engulf_4hour="https://discord.com/api/webhooks/1246113307136622653/DwaqJVYhIYAEufkMzP7FakhbL4JIPOGEIzl8uSSAoBsg6RA6m5rZGqFEAF3NPJAMeN7L"
 engulf_minute="https://discord.com/api/webhooks/1213155128161607712/ieF6ektHPErCiXQihgN5CD2JJa2u1GLW2d9SKqGa2HnJTri6S3k4u7_AhzFd3HBkJGWD"
-engulf_30minute="https://discord.com/api/webhooks/1213155275536728115/mISPJIUHt1w7CqW6s7i0c-V0_uOL5aE9QzEATLFApb86ZhkgiAfTf-2Mi-5uxULhmwPC"
-vol1k_25k="https://discord.com/api/webhooks/1210603719519903754/VFz_tr34NPURpE9jM__yvsnTqUb4XwJLpeP9Mz8RzpcNc0uYG5XTFWml8UxxHiiD4GkF"
-vol25k_50k="https://discord.com/api/webhooks/1210604610905964564/8iSoW_QDjOkgjascCIvuiKL__n6KJv2ru6lm9-l9ZeQGRWNBkfPlpjb7TPaDNwNiXqSd"
-vol50k="https://discord.com/api/webhooks/1210604487631437874/X8MvC8n5x7dRfP9pvInhCHTUMiuw3foHPn-UeSmK-iobsOTEMGalwxSyunrdip4a5kZR"
+engulf_30minute="https://discord.com/api/webhooks/1246113524388855818/8snQjoYvZk_oG3MXdsgG7zyN3rYOo13N6XV6HKzI_P4XnuRydhipYotwd6D80WqgY1ov"
+
+vol1k_25k="https://discord.com/api/webhooks/1246112589956775986/_XfVlgu06E0_OFOUQxMdj4paXET_hTxLEjiE_fM9S2WdABe9oJM686QI-xzaH3d0FM80"
+vol10k_25k="https://discord.com/api/webhooks/1246112713671708854/QiDj5eZxKZuLgKckJ9bb0qm_Bbc00qXElhG8zdGSW8CKX1RWiXzGXC7uhMnM_MTjlZMB"
+vol50k="https://discord.com/api/webhooks/1246112864272650382/XQVZTzdZls_k4NXbYLV2Ff3PUh3o3XXKfytB5BLhvMT6yZ0rbyF3GCIkGKHL8TFszjkI"
 
 class TechnicalProcessor:
     def __init__(self, pool):
         self.pool = pool
 
         self.starter = Starter(pool)
         self.timespans = ['minute', 'hour', 'week', 'day', 'month']
@@ -71,25 +78,28 @@
         self.eight_days_ago = (datetime.now() - timedelta(days=8)).strftime('%Y-%m-%d')
         self.processed_tickers = {timespan: {} for timespan in self.timespans}  # Cache for processed tickers
         self.processing_interval = timedelta(minutes=1)  # Interval
 
         self.trading = WebullTrading()
         self.processed_td9_tickers = {timespan: {} for timespan in self.chart_timespans}
         self.interval_dict = {
-            'm': os.environ.get('td9_m', 'https://discord.com/api/webhooks/1207884982647918613/TY0qda6Kr7MMUCiOfNRMKZIqgBZ94EWcN5JVt_wLb3VeDU4vBbt0Pwml1EEIsWfLaub3'),
-            'd': os.environ.get('td9_d', 'https://discord.com/api/webhooks/1207885362526158928/0HaIDN2XLugQvaliFxuiKCYLsXhEBOd4vqiWQt_XkeFXgq2jnXRbVBaPH7C5NDf-FCTr'),
-            'w': os.environ.get('td9_w', 'https://discord.com/api/webhooks/1207885265448738918/vnfuFtm4Yw-NcaYmgziCJJZcLW1UfNEJDn0d7KPk0rY_q7M44W6R98f2fg3y8leKyOvA'),
-            'm1': os.environ.get('td9_m1', 'https://discord.com/api/webhooks/1212540300350988359/e_BX3yWTdZaOyvFC3P1Ir7CAq5LN8IRxCcq9R_VJZvqFDfnSwXOxnyxhctyDpJdVq9ym'),
-            'm5': os.environ.get('td9_m5', 'https://discord.com/api/webhooks/1212540358827835432/EoQKj7Pt0idb0Z0qaAahxXKvpMgVhL6KPGOjIdjxWgOS3P9tJmlFqdAi3MRRBATPayBE'),
-            'm15': os.environ.get('td9_m15', 'https://discord.com/api/webhooks/1212540447919186000/Flqytu4d4I8bZiD8GzZf1j2qb0xiMFQRg9dV96bE9stCIqXGQJ5RkQJB0mIhOCH8gRQ5'),
-            'm30': os.environ.get('td9_m30', 'https://discord.com/api/webhooks/1212540241689190480/SCcvC4GeOYoeodES7zYEMOqyYpwWeBoB3awGAO6Xp6KkeXSJJqemgz7VfSjCscILQxzW'),
-            'm60': os.environ.get('td9_m60', 'https://discord.com/api/webhooks/1212540533151506503/WFu8NiwQi3iH86OH9lBegT-AwJM8rh-fWPuR-EhInWr20T0wJnWEm4VHCzLZ2Ore8SPa'),
-            'm120': os.environ.get('td9_m120', 'https://discord.com/api/webhooks/1212540620833427486/tASJYDyKR7tmsH0MjH8kPG2AuNBgY12Dr_mZ8jHqRUDsyYztHllWuSZM6DB7iVSbLYTj'),
-            'm240': os.environ.get('td9_m240', 'https://discord.com/api/webhooks/1212540713934266438/kMrwDe94JpdZC0oFqsgdaqg3jU3YK2RgXebgHhIKs8jul2LO3HqyFR0aD55OJjB_svjR')
+            'm': os.environ.get('min1_td9', 'https://discord.com/api/webhooks/1207884982647918613/TY0qda6Kr7MMUCiOfNRMKZIqgBZ94EWcN5JVt_wLb3VeDU4vBbt0Pwml1EEIsWfLaub3'),
+            'd': os.environ.get('day_td9', 'https://discord.com/api/webhooks/1207885362526158928/0HaIDN2XLugQvaliFxuiKCYLsXhEBOd4vqiWQt_XkeFXgq2jnXRbVBaPH7C5NDf-FCTr'),
+            'w': os.environ.get('week_td9', 'https://discord.com/api/webhooks/1207885265448738918/vnfuFtm4Yw-NcaYmgziCJJZcLW1UfNEJDn0d7KPk0rY_q7M44W6R98f2fg3y8leKyOvA'),
+            'm1': os.environ.get('min1_td9', 'https://discord.com/api/webhooks/1212540300350988359/e_BX3yWTdZaOyvFC3P1Ir7CAq5LN8IRxCcq9R_VJZvqFDfnSwXOxnyxhctyDpJdVq9ym'),
+            'm5': os.environ.get('min5_td9', 'https://discord.com/api/webhooks/1212540358827835432/EoQKj7Pt0idb0Z0qaAahxXKvpMgVhL6KPGOjIdjxWgOS3P9tJmlFqdAi3MRRBATPayBE'),
+            'm15': os.environ.get('min15_td9', 'https://discord.com/api/webhooks/1212540447919186000/Flqytu4d4I8bZiD8GzZf1j2qb0xiMFQRg9dV96bE9stCIqXGQJ5RkQJB0mIhOCH8gRQ5'),
+            'm30': os.environ.get('min30_td9', 'https://discord.com/api/webhooks/1212540241689190480/SCcvC4GeOYoeodES7zYEMOqyYpwWeBoB3awGAO6Xp6KkeXSJJqemgz7VfSjCscILQxzW'),
+            'm60': os.environ.get('min60_td9', 'https://discord.com/api/webhooks/1212540533151506503/WFu8NiwQi3iH86OH9lBegT-AwJM8rh-fWPuR-EhInWr20T0wJnWEm4VHCzLZ2Ore8SPa'),
+            'm120': os.environ.get('min120_td9', 'https://discord.com/api/webhooks/1212540620833427486/tASJYDyKR7tmsH0MjH8kPG2AuNBgY12Dr_mZ8jHqRUDsyYztHllWuSZM6DB7iVSbLYTj'),
+            'm240': os.environ.get('min240_td9', 'https://discord.com/api/webhooks/1212540713934266438/kMrwDe94JpdZC0oFqsgdaqg3jU3YK2RgXebgHhIKs8jul2LO3HqyFR0aD55OJjB_svjR')
         }
+
+
+
         self.hammer_hooks = { 
             'm1': os.environ.get('hammer_minute'),
             'm30': os.environ.get('hammer_30minute'),
             'm60': os.environ.get('hammer_hour'),
             'm240': os.environ.get('hammer_4hour'),
             'd': os.environ.get('hammer_day'),
             'w': os.environ.get('hammer_week'),
@@ -349,14 +359,26 @@
         :param ticker: The ticker symbol.
         :param timespan: The timespan to fetch RSI for.
         :return: The RSI data.
         """
         await self.db.connect()
         if ticker == 'SPX':
             ticker = 'I:SPX'
+        elif ticker == 'VIX':
+            ticker = 'I:VIX'
+        elif ticker == 'RUT':
+            ticker = 'I:RUT'
+        elif ticker == 'SPXW':
+            ticker = 'I:SPX'
+        elif ticker == 'DJT':
+            ticker = 'I:DJT'
+        elif ticker == 'NDXP':
+            ticker = 'I:NDXP'
+        elif ticker == 'RUTW':
+            ticker = 'I:RUTW'
         status = None
         current_time = datetime.now()
 
         # Check if ticker was processed recently
         if ticker in self.processed_tickers[timespan]:
             last_processed_time = self.processed_tickers[timespan][ticker]
             if (current_time - last_processed_time) < self.processing_interval:
@@ -380,29 +402,29 @@
                         macd_hook = macd_day
                     elif timespan == 'month':
                         macd_hook = macd_month
                     
                     if macd_hook:
                         macd_tasks.append(
                             asyncio.create_task(
-                                macd_embed(hook=macd_hook, type=macd_cross, ticker=ticker, timespan=timespan, db=self.db)
+                                macd_embed(hook=macd_hook, type=macd_cross, ticker=ticker, timespan=timespan)
                             )
                         )
 
             if macd_tasks:
                 await asyncio.gather(*macd_tasks)
 
             if rsi.rsi_value[0] <= 30:
                 status = 'oversold'
             elif rsi.rsi_value[0] >= 70:
                 status = 'overbought'
 
             if status is not None:
                 webhook_url = self.rsi_dict.get(timespan)
-                await rsi_embed(hook=webhook_url, ticker=ticker, status=status, timespan=timespan, rsi=rsi.rsi_value[0], underlying_data=rsi.underlying_dict, db=self.db)
+                await rsi_embed(hook=webhook_url, ticker=ticker, status=status, timespan=timespan, rsi=rsi.rsi_value[0], underlying_data=rsi.underlying_dict)
             
             # Update the last processed time for the ticker
             self.processed_tickers[timespan][ticker] = current_time
             return rsi
 
         except Exception as e:
             logging.error(f"Error fetching RSI for {ticker} ({timespan}): {e}")
@@ -539,59 +561,58 @@
                                     check_bear_task = asyncio.create_task(self.check_td9_bearish(td9_df))
 
                                     results = await asyncio.gather(check_bull_task, check_bear_task)
                                     
                                     if results[0] == True:
                                         print(results[0])
                                         status = 'bullish_td9'
-                                        asyncio.create_task(td9_embed(hook=self.interval_dict.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df, db=self.db))
+                                        asyncio.create_task(td9_embed(hook=self.interval_dict.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df))
 
 
                                     if results[1] == True:
                                         print(results[1])
                                         status = 'bearish_td9'
-                                        asyncio.create_task(td9_embed(hook=self.interval_dict.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df, db=self.db))
-                                    # Checking for additional candlestick patterns
+                                        asyncio.create_task(td9_embed(hook=self.interval_dict.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df))
                                     # async for check_star in self.is_shooting_star(td9_df):
                                     #     if check_star:
                                     #         status = 'shooting_star'
                                     #         await candlestick_embed(hook=self.interval_dict.get(interval), timespan=timespan, status=status, ticker=ticker, df=td9_df)
                                     #         print(f"SHOOTING STAR DETECTED {ticker}")
 
                                     async for check_bull_engulf in self.is_bullish_engulfing(td9_df):
                                         if check_bull_engulf == True:
                                             status = 'bullish_engulfing'
-                                            asyncio.create_task(candlestick_embed(hook=self.engulf_hooks.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df, db=self.db))
+                                            asyncio.create_task(candlestick_embed(hook=self.engulf_hooks.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df))
                                             print(f"BULLISH ENGULFING DETECTED {ticker}")
 
                                     async for check_bear_engulf in self.is_bearish_engulfing(td9_df):
                                         if check_bear_engulf == True:
                                             status = 'bearish_engulfing'
-                                            asyncio.create_task(candlestick_embed(hook=self.engulf_hooks.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df, db=self.db))
+                                            asyncio.create_task(candlestick_embed(hook=self.engulf_hooks.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df))
                                             print(f"BEARISH ENGULFING DETECTED {ticker}")
 
 
 
                                     async for check_hammer in self.is_hammer(td9_df):
                                         if check_hammer == True:
                                             status = 'hammer'
-                                            asyncio.create_task(candlestick_embed(hook=self.hammer_hooks.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df, db=self.db))
+                                            asyncio.create_task(candlestick_embed(hook=self.hammer_hooks.get(interval), timespan=timespan, status=status, ticker=ticker, df=lol_td9_df))
                                             print(f"HAMMER DETECTED {ticker}")
 
 
                                     soldiers_pattern_detected = await self.is_three_white_soldiers(td9_df)
                                     if soldiers_pattern_detected == True:
                                         status = 'bullish_soldiers'
-                                        asyncio.create_task(candlestick_embed(hook="https://discord.com/api/webhooks/1244511042990768169/cD7NmOHJzvxOl81S7Uk3m6ScJFqrXVlyYOIOeEFyxGJfhW0RTnZ4P99MQd2qbf1d63zO", timespan=timespan, status=status, ticker=ticker, df=lol_td9_df, db=self.db))
+                                        asyncio.create_task(candlestick_embed(hook="https://discord.com/api/webhooks/1244511042990768169/cD7NmOHJzvxOl81S7Uk3m6ScJFqrXVlyYOIOeEFyxGJfhW0RTnZ4P99MQd2qbf1d63zO", timespan=timespan, status=status, ticker=ticker, df=lol_td9_df))
                                         print("Three Black Crows pattern detected!")
 
                                     crows_pattern_detected = await self.is_three_black_crows(td9_df)
                                     if crows_pattern_detected == True:
                                         status = 'bearish_crows'
-                                        asyncio.create_task(candlestick_embed(hook="https://discord.com/api/webhooks/1244511114960699474/cXrDi3nfa-9zm35heARDOv4xnGYuaOcjJb-V7ZgJuz_Y0pH_sZqv7fLaA071AJ1N0Qgf", timespan=timespan, status=status, ticker=ticker, df=lol_td9_df, db=self.db))
+                                        asyncio.create_task(candlestick_embed(hook="https://discord.com/api/webhooks/1244511114960699474/cXrDi3nfa-9zm35heARDOv4xnGYuaOcjJb-V7ZgJuz_Y0pH_sZqv7fLaA071AJ1N0Qgf", timespan=timespan, status=status, ticker=ticker, df=lol_td9_df))
                                         print("Three White Soldiers pattern detected!")
 
                                                                                     
                                 except Exception as e:
                                     print(f"Error processing ticker: {e}")        
                         else:
                             # Handle the case where the data is not in the expected format
```

### Comparing `mktdata-0.0.7/mktdata/optionsdata.py` & `mktdata-0.0.8/mktdata/optionsdata.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.7/mktdata/stock_data.py` & `mktdata-0.0.8/mktdata/stock_data.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.7/mktdata.egg-info/PKG-INFO` & `mktdata-0.0.8/mktdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktdata
-Version: 0.0.7
+Version: 0.0.8
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
@@ -126,15 +126,15 @@
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
 Requires-Dist: orjson==3.9.10
 Requires-Dist: outcome==1.3.0.post0
 Requires-Dist: overrides==7.4.0
 Requires-Dist: packaging==23.2
-Requires-Dist: pandas==2.2.1
+Requires-Dist: pandas==2.2.2
 Requires-Dist: peewee==3.17.0
 Requires-Dist: Pillow==10.1.0
 Requires-Dist: pkginfo==1.9.6
 Requires-Dist: plotly==5.20.0
 Requires-Dist: polygon==1.1.3
 Requires-Dist: polygon-api-client==1.13.3
 Requires-Dist: posthog==3.0.2
@@ -211,14 +211,14 @@
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: uvicorn==0.23.2
 Requires-Dist: waitress==2.1.2
 Requires-Dist: watchfiles==0.21.0
 Requires-Dist: webcolors==1.13
 Requires-Dist: webencodings==0.5.1
 Requires-Dist: websocket-client==1.6.4
-Requires-Dist: websockets==11.0.3
+Requires-Dist: websockets==12.0
 Requires-Dist: Werkzeug==3.0.1
 Requires-Dist: wrapt==1.14.1
 Requires-Dist: wsproto==1.2.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: yfinance==0.2.32
 Requires-Dist: zipp==3.17.0
```

### Comparing `mktdata-0.0.7/mktdata.egg-info/requires.txt` & `mktdata-0.0.8/mktdata.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 opentelemetry-sdk==1.20.0
 opentelemetry-semantic-conventions==0.41b0
 opt-einsum==3.3.0
 orjson==3.9.10
 outcome==1.3.0.post0
 overrides==7.4.0
 packaging==23.2
-pandas==2.2.1
+pandas==2.2.2
 peewee==3.17.0
 Pillow==10.1.0
 pkginfo==1.9.6
 plotly==5.20.0
 polygon==1.1.3
 polygon-api-client==1.13.3
 posthog==3.0.2
@@ -208,14 +208,14 @@
 urllib3==1.26.18
 uvicorn==0.23.2
 waitress==2.1.2
 watchfiles==0.21.0
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.6.4
-websockets==11.0.3
+websockets==12.0
 Werkzeug==3.0.1
 wrapt==1.14.1
 wsproto==1.2.0
 yarl==1.9.4
 yfinance==0.2.32
 zipp==3.17.0
```

