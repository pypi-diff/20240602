# Comparing `tmp/py_alpaca_daily_losers-0.3.4.tar.gz` & `tmp/py_alpaca_daily_losers-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_daily_losers-0.3.4.tar", max compression
+gzip compressed data, was "py_alpaca_daily_losers-1.0.0.tar", max compression
```

## Comparing `py_alpaca_daily_losers-0.3.4.tar` & `py_alpaca_daily_losers-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.4/LICENSE
--rw-r--r--   0        0        0    13887 2024-05-27 04:08:54.588515 py_alpaca_daily_losers-0.3.4/README.md
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/__init__.py
--rw-r--r--   0        0        0    19884 2024-05-29 02:29:44.236574 py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/daily_losers.py
--rw-r--r--   0        0        0        0 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/src/__init__.py
--rw-r--r--   0        0        0      481 2024-05-25 20:55:09.612759 py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/src/global_fuctions.py
--rw-r--r--   0        0        0     2527 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/src/openai.py
--rw-r--r--   0        0        0     1927 2024-05-27 16:15:57.122351 py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/src/slack.py
--rw-r--r--   0        0        0     7686 2024-05-29 02:29:33.773079 py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/src/yahoo.py
--rw-r--r--   0        0        0      740 2024-05-30 22:52:08.554764 py_alpaca_daily_losers-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    14639 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     2267 2024-06-01 22:06:14.046692 py_alpaca_daily_losers-1.0.0/README.md
+-rw-r--r--   0        0        0     1212 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/__init__.py
+-rw-r--r--   0        0        0      902 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/calc.py
+-rw-r--r--   0        0        0    19678 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/daily_losers.py
+-rw-r--r--   0        0        0      460 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/global_functions.py
+-rw-r--r--   0        0        0     2563 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/openai.py
+-rw-r--r--   0        0        0     4550 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/requests.py
+-rw-r--r--   0        0        0     1896 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/slack.py
+-rw-r--r--   0        0        0     7069 2024-06-01 21:36:01.317042 py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/yahoo.py
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 py_alpaca_daily_losers-1.0.0/PKG-INFO
```

### Comparing `py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/daily_losers.py` & `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/daily_losers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import os
+from datetime import datetime, timedelta
+
 import pandas as pd
+from dotenv import load_dotenv
 from py_alpaca_api.alpaca import PyAlpacaApi
-
-from .src.openai import OpenAIAPI
-from .src.yahoo import Yahoo
-from .src.global_fuctions import send_message
-
-from ta.volatility import BollingerBands
+from pytz import timezone
 from ta.momentum import RSIIndicator
-
+from ta.volatility import BollingerBands
 from tqdm import tqdm
-from dotenv import load_dotenv
-from datetime import datetime
-from datetime import timedelta
-from pytz import timezone
+
+from .global_functions import send_message
+from .openai import OpenAIAPI
+from .yahoo import Yahoo
 
 tz = timezone("US/Eastern")
 ctime = datetime.now(tz)
 today = ctime.strftime("%Y-%m-%d")
 previous_day = (ctime - timedelta(days=1)).strftime("%Y-%m-%d")
 year_ago = (ctime - timedelta(days=365)).strftime("%Y-%m-%d")
 
@@ -27,27 +25,26 @@
 api_secret = str(os.getenv("API_SECRET"))
 api_paper = True if os.getenv("API_PAPER") == "True" else False
 
 
 class DailyLosers:
     def __init__(self):
         """
-        This code initializes an instance of the PyAlpacaApi class with the provided API key and API secret.
-        It sets the api_paper parameter to True, indicating that the API should be used in a paper trading environment.
+        This code initializes an instance of the PyAlpacaApi class with the provided API key
+        and API secret. It sets the api_paper parameter to True, indicating that the API
+        should be used in a paper trading environment.
 
         The value of the production variable is derived from the environment variable "PRODUCTION".
         If the value of "PRODUCTION" is "True", the production variable is set to True.
         Otherwise, it is set to False.
 
-        This code is used to configure and set up the PyAlpacaApi for interacting with the Alpaca API in a Python
-        application.
+        This code is used to configure and set up the PyAlpacaApi for interacting with the
+        Alpaca API in a Python application.
         """
-        self.alpaca = PyAlpacaApi(
-            api_key=api_key, api_secret=api_secret, api_paper=True
-        )
+        self.alpaca = PyAlpacaApi(api_key=api_key, api_secret=api_secret, api_paper=True)
         self.production = True if os.getenv("PRODUCTION") == "True" else False
 
     def run(self):
         """
         Executes the main logic of the program.
 
         This method performs the following steps:
@@ -60,104 +57,94 @@
         self.liquidate_positions_for_capital()
         self.check_for_buy_opportunities()
 
     ########################################################
     # Define the sell_positions_from_criteria method
     ########################################################
     def sell_positions_from_criteria(self):
-        """
-        Sell Positions from Criteria
-
-        This method is used to sell positions based on sell criteria. It retrieves sell opportunities, current
-        positions, and then iterates through the sell opportunities to sell the stocks.
-
-        Parameters:
-            - None
-
-        Returns:
-            - None
-
-        """
         print("Selling positions based on sell criteria")
-
         sell_opportunities = self.get_sell_opportunities()
         if not sell_opportunities:
             send_message("No sell opportunities found.")
             return
-
         current_positions = self.alpaca.position.get_all()
-        sold_positions = []
+        sold_positions = self._sell_positions(sell_opportunities, current_positions)
+        self._send_position_messages(sold_positions, "sell")
 
+    def _sell_positions(self, sell_opportunities, current_positions):
+        SYMBOL = "symbol"
+        QTY = "qty"
+        sold_positions = []
         for symbol in sell_opportunities:
             try:
-                qty = current_positions[current_positions["symbol"] == symbol][
-                    "qty"
-                ].values[0]
-
+                qty = current_positions[current_positions[SYMBOL] == symbol][QTY].values[0]
                 self.alpaca.position.close(symbol_or_id=symbol, percentage=100)
+                sold_positions.append({SYMBOL: symbol, QTY: qty})
             except Exception as e:
                 send_message(f"Error selling {symbol}: {e}")
                 continue
-            else:
-                sold_positions.append({"symbol": symbol, "qty": qty})
-
-        self._send_position_messages(sold_positions, "sell")
+        return sold_positions
 
     ########################################################
     # Define the get_sell_opportunities method
     ########################################################
     def get_sell_opportunities(self) -> list:
         """
-        Retrieves a list of symbols representing potential sell opportunities based on specified criteria.
+        Retrieves a list of symbols representing potential sell opportunities based on
+        specified criteria.
 
         Returns:
             sell_list (list): A list of symbols representing potential sell opportunities.
         """
         current_positions = self.alpaca.position.get_all()
         if current_positions[current_positions["symbol"] != "Cash"].empty:
             return []
 
-        current_positions_symbols = current_positions[
-            current_positions["symbol"] != "Cash"
-        ]["symbol"].tolist()
+        current_positions_symbols = current_positions[current_positions["symbol"] != "Cash"][
+            "symbol"
+        ].tolist()
 
         assets_history = self.get_ticker_data(current_positions_symbols)
 
-        sell_criteria = (
-            (assets_history[["rsi14", "rsi30", "rsi50", "rsi200"]] >= 70).any(
-                axis=1
-            )
-        ) | (
-            (
-                assets_history[["bbhi14", "bbhi30", "bbhi50", "bbhi200"]] == 1
-            ).any(axis=1)
-        )
+        RSI_COLUMNS = ["rsi14", "rsi30", "rsi50", "rsi200"]
+        BBHI_COLUMNS = ["bbhi14", "bbhi30", "bbhi50", "bbhi200"]
+
+        criterion1 = assets_history[RSI_COLUMNS] >= 70
+        criterion2 = assets_history[BBHI_COLUMNS] == 1
+        sell_criteria = criterion1.any(axis=1) | criterion2.any(axis=1)
 
         sell_filtered_df = assets_history[sell_criteria]
         sell_list = sell_filtered_df["symbol"].tolist()
 
-        percentage_change_list = current_positions[
-            current_positions["profit_pct"] > 0.1
-        ]["symbol"].tolist()
-
-        for symbol in percentage_change_list:
-            if symbol not in sell_list:
-                sell_list.append(symbol)
+        take_profit_list = current_positions[current_positions["profit_pct"] > 0.1][
+            "symbol"
+        ].tolist()
+
+        stop_loss_list = current_positions[current_positions["profit_pct"] < -0.1][
+            "symbol"
+        ].tolist()
+
+        for take_profit, stop_loss in zip(take_profit_list, stop_loss_list):
+            if take_profit not in sell_list:
+                sell_list.append(take_profit)
+            if stop_loss not in sell_list:
+                sell_list.append(stop_loss)
 
         return sell_list
 
     ########################################################
     # Define the liquidate_positions_for_capital method
     ########################################################
     def liquidate_positions_for_capital(self):
         """
         Liquidates positions to ensure cash is 10% of the portfolio.
 
-        This method calculates the current cash available and compares it to the total holdings in the portfolio.
-        If the cash is less than 10% of the total holdings, it sells the top 25% performing stocks to make cash
+        This method calculates the current cash available and compares it to the total holdings
+        in the portfolio. If the cash is less than 10% of the total holdings, it sells the
+        top 25% performing stocks to make cash
         10% of the portfolio.
 
         Returns:
             None
         """
         print("Liquidating positions to make Cash 10% of the portfolio...")
 
@@ -172,29 +159,22 @@
         sold_positions = []
 
         if cash_row["market_value"][0] / total_holdings < 0.1:
             current_positions = current_positions[
                 current_positions["symbol"] != "Cash"
             ].sort_values(by="profit_pct", ascending=False)
 
-            top_performers = current_positions.iloc[
-                : int(len(current_positions) // 2)
-            ]
+            top_performers = current_positions.iloc[: int(len(current_positions) // 2)]
             top_performers_market_value = top_performers["market_value"].sum()
-            cash_needed = (
-                total_holdings * 0.1 - cash_row["market_value"][0]
-            ) + 5.00
+            cash_needed = (total_holdings * 0.1 - cash_row["market_value"][0]) + 5.00
 
             for index, row in top_performers.iterrows():
-                print(
-                    f"Selling {row['symbol']} to make cash 10% portfolio cash requirement"
-                )
+                print(f"Selling {row['symbol']} to make cash 10% portfolio cash requirement")
                 amount_to_sell = int(
-                    (row["market_value"] / top_performers_market_value)
-                    * cash_needed
+                    (row["market_value"] / top_performers_market_value) * cash_needed
                 )
                 if amount_to_sell == 0:
                     continue
                 try:
                     self.alpaca.order.market(
                         symbol=row["symbol"],
                         notional=amount_to_sell,
@@ -214,35 +194,38 @@
         self._send_position_messages(sold_positions, "liquidate")
 
     ########################################################
     # Define the check_for_buy_opportunities method
     ########################################################
     def check_for_buy_opportunities(self):
         """
-        The following code is a method definition that checks for buy opportunities. It performs the following steps:
+        The following code is a method definition that checks for buy opportunities. It performs
+        the following steps:
 
-        1. Calls the `get_daily_losers()` method to get the list of tickers that have performed poorly on a given day.
-        2. Calls the `get_ticker_data(losers)` method, passing in the list of losers, to get detailed data for each
+        1. Calls the `get_daily_losers()` method to get the list of tickers that have performed
+        poorly on a given day.
+        2. Calls the `get_ticker_data(losers)` method, passing in the list of losers, to get
+        detailed data for each
         ticker.
-        3. Applies buy criteria to the ticker data by calling the `buy_criteria(ticker_data)` method, which returns a
-        filtered list of tickers that meet the buy criteria.
-        4. Filters the list of tickers with news by calling the `filter_tickers_with_news(filter_tickers)` method.
+        3. Applies buy criteria to the ticker data by calling the `buy_criteria(ticker_data)`
+        method, which returns a filtered list of tickers that meet the buy criteria.
+        4. Filters the list of tickers with news by calling the
+        `filter_tickers_with_news(filter_tickers)` method.
         5. Opens positions for the filtered tickers by calling the `open_positions()` method.
 
-        This method assumes that the necessary data and methods required for each step are available within the current
+        This method assumes that the necessary data and methods required for each step are
+        available within the current
         class or its dependencies.
 
         """
         losers = self.get_daily_losers()
         tickers = self.filter_tickers_with_news(losers)
 
         if len(tickers) > 0:
-            print(
-                f"{len(tickers)} buy opportunities found. Opening positions..."
-            )
+            print(f"{len(tickers)} buy opportunities found. Opening positions...")
             self.open_positions(tickers=tickers)
         else:
             print("No buy opportunities found")
 
     ########################################################
     # Define the open_positions method
     ########################################################
@@ -254,15 +237,16 @@
             tickers (list): A list of tickers to buy.
             ticker_limit (int, optional): The maximum number of tickers to buy. Defaults to 8.
 
         Returns:
             None
         """
         print(
-            "Buying orders based on buy opportunities and openai sentiment. Limit to 8 stocks by default"
+            "Buying orders based on buy opportunities and openai sentiment. \
+                Limit to 8 stocks by default"
         )
 
         available_cash = self.alpaca.account.get().cash
 
         if len(tickers) == 0:
             send_message("No tickers to buy.")
             return
@@ -274,17 +258,15 @@
         for ticker in tickers[:ticker_limit]:
             try:
                 self.alpaca.order.market(symbol=ticker, notional=notional)
             except Exception as e:
                 send_message(f"Error buying {ticker}: {e}")
                 continue
             else:
-                bought_positions.append(
-                    {"symbol": ticker, "notional": round(notional, 2)}
-                )
+                bought_positions.append({"symbol": ticker, "notional": round(notional, 2)})
 
         self._send_position_messages(bought_positions, "buy")
 
     ########################################################
     # Define the update_or_create_watchlist method
     ########################################################
     def update_or_create_watchlist(self, name, symbols):
@@ -295,15 +277,16 @@
         - name (str): The name of the watchlist.
         - symbols (list): A list of symbols to include in the watchlist.
 
         Returns:
         None
 
         Raises:
-        ValueError: If an error occurs while updating the watchlist, a new watchlist will be created instead.
+        ValueError: If an error occurs while updating the watchlist,
+        a new watchlist will be created instead.
         """
         try:
             self.alpaca.watchlist.update(watchlist_name=name, symbols=symbols)
         except Exception:
             self.alpaca.watchlist.create(name=name, symbols=symbols)
 
     ########################################################
@@ -343,45 +326,43 @@
                 if bullish > bearish:
                     filtered_tickers.append(ticker)
 
         if len(filtered_tickers) == 0:
             print("No tickers with news found")
             return []
 
-        self.update_or_create_watchlist(
-            name="DailyLosers", symbols=filtered_tickers
-        )
+        self.update_or_create_watchlist(name="DailyLosers", symbols=filtered_tickers)
 
         return self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
 
     ########################################################
     # Define the get_daily_losers method
     ########################################################
     def get_daily_losers(self) -> list:
         """
-        This function is used to retrieve a list of daily losers from the stock market. It uses the Alpaca API to get a
-        list of loser symbols and performs some criteria checks on them before returning the final list of symbols.
+        This function is used to retrieve a list of daily losers from the stock market.
+        It uses the Alpaca API to get a list of loser symbols and performs some
+        criteria checks on them before returning the final list of symbols.
 
         Parameters:
         - None
 
         Returns:
         - A list of stock symbols representing the daily losers.
 
         Note:
         - This function relies on the 'Yahoo' class and its associated methods.
-        - This function depends on the 'get_ticker_data()', 'buy_criteria()', 'send_message()', 'get_sentiment()',
-        'update_or_create_watchlist()', and 'get_assets()' methods from other parts of the code.
+        - This function depends on the 'get_ticker_data()', 'buy_criteria()', 'send_message()',
+        'get_sentiment()', 'update_or_create_watchlist()', and 'get_assets()'
+        methods from other parts of the code.
         - The 'send_message()' function is responsible for sending a message/notification.
         - The 'tqdm' library is used to display a progress bar while processing the symbols.
         """
         yahoo = Yahoo()
-        losers = self.alpaca.screener.losers(total_losers_returned=130)[
-            "symbol"
-        ].to_list()
+        losers = self.alpaca.screener.losers(total_losers_returned=130)["symbol"].to_list()
 
         losers = self.get_ticker_data(losers)
         losers = self.buy_criteria(losers)
 
         if len(losers) == 0:
             send_message("No daily losers found.")
             return []
@@ -414,29 +395,27 @@
         - A list of stock assets that meet the buy criteria.
 
         Example Usage:
         buy_criteria(data)
 
         """
 
-        buy_criteria = (
-            (data[["bblo14", "bblo30", "bblo50", "bblo200"]] == 1).any(axis=1)
-        ) | ((data[["rsi14", "rsi30", "rsi50", "rsi200"]] <= 30).any(axis=1))
+        buy_criteria = ((data[["bblo14", "bblo30", "bblo50", "bblo200"]] == 1).any(axis=1)) | (
+            (data[["rsi14", "rsi30", "rsi50", "rsi200"]] <= 30).any(axis=1)
+        )
 
         buy_filtered_data = data[buy_criteria]
 
         filtered_data = list(buy_filtered_data["symbol"])
 
         if len(filtered_data) == 0:
             print("No tickers meet the buy criteria")
             return []
 
-        self.update_or_create_watchlist(
-            name="DailyLosers", symbols=filtered_data
-        )
+        self.update_or_create_watchlist(name="DailyLosers", symbols=filtered_data)
 
         return self.alpaca.watchlist.get_assets(watchlist_name="DailyLosers")
 
     ########################################################
     # Define the get_ticker_data method
     ########################################################
     def get_ticker_data(self, tickers) -> pd.DataFrame:
@@ -450,30 +429,26 @@
             pd.DataFrame: DataFrame containing technical data for the tickers.
 
         """
         df_tech = []
 
         for i, ticker in tqdm(
             enumerate(tickers),
-            desc="• Analyzing ticker data for "
-            + str(len(tickers))
-            + " symbols from Alpaca API",
+            desc="• Analyzing ticker data for " + str(len(tickers)) + " symbols from Alpaca API",
         ):
             try:
                 history = self.alpaca.history.get_stock_data(
                     symbol=ticker, start=year_ago, end=previous_day
                 )
             except ValueError:
                 continue
 
             try:
                 for n in [14, 30, 50, 200]:
-                    history["rsi" + str(n)] = RSIIndicator(
-                        close=history["close"], window=n
-                    ).rsi()
+                    history["rsi" + str(n)] = RSIIndicator(close=history["close"], window=n).rsi()
                     history["bbhi" + str(n)] = BollingerBands(
                         close=history["close"], window=n, window_dev=2
                     ).bollinger_hband_indicator()
                     history["bblo" + str(n)] = BollingerBands(
                         close=history["close"], window=n, window_dev=2
                     ).bollinger_lband_indicator()
                 df_tech_temp = history.tail(1)
@@ -506,25 +481,23 @@
             "buy": "bought",
             "liquidate": "liquidated",
         }
 
         try:
             position_name = position_names[pos_type]
         except KeyError:
-            raise ValueError(
-                'Invalid type. Must be "sell", "buy", or "liquidate".'
-            )
+            raise ValueError('Invalid type. Must be "sell", "buy", or "liquidate".')
 
         if not positions:
             position_message = f"No positions to {pos_type}"
         else:
-            is_market_open = (
-                "" if self.alpaca.market.clock().is_open else " pretend"
+            is_market_open = "" if self.alpaca.market.clock().is_open else " pretend"
+            position_message = (
+                f"Successfully{is_market_open} {position_name} the following positions:\n"
             )
-            position_message = f"Successfully{is_market_open} {position_name} the following positions:\n"
 
             for position in positions:
 
                 if position_name == "liquidated":
                     qty_key = "notional"
                 elif position_name == "sold":
                     qty_key = "qty"
```

### Comparing `py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/src/openai.py` & `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from openai import OpenAI
 
 from dotenv import load_dotenv
+from openai import OpenAI
 
 load_dotenv()
 
 
 class OpenAIAPI:
     def __init__(self):
         self.api_key = os.getenv("OPENAI_API_KEY")
@@ -16,45 +16,45 @@
     def chat(self, msgs):
         """
         Chat with the OpenAI API
         :param msgs: List of messages
         return: OpenAI response
         """
         openai = OpenAI(api_key=self.api_key)
-        response = openai.chat.completions.create(
-            model="gpt-3.5-turbo", messages=msgs
-        )
+        response = openai.chat.completions.create(model="gpt-3.5-turbo", messages=msgs)
         message = response
         return message
 
     ########################################################
     # Define the get_market_sentiment function
     ########################################################
     def get_sentiment_analysis(self, title, symbol, article):
         """
         get_sentiment_analysis(self, title, symbol, article)
 
-        This method is used to get the sentiment analysis for financial news. It takes in the title, symbol,
-        and article as parameters.
+        This method is used to get the sentiment analysis for financial news.
+        It takes in the title, symbol, and article as parameters.
 
         Parameters:
             - title (str): The title of the news.
             - symbol (str): The stock symbol associated with the news.
             - article (str): The content of the news article.
 
         Returns:
-            - signal (str): The sentiment analysis result as either "BEARISH", "BULLISH", or "NEUTRAL".
+            - signal (str): The sentiment analysis result as either
+            "BEARISH", "BULLISH", or "NEUTRAL".
 
         """
         message_history = []
         sentiments = []
         # Send the system message to the OpenAI API
         system_message = "You will work as a Sentiment Analysis for Financial news. \
-            I will share news headline, stock symbol and article. \
-                You will only answer as:\n\n BEARISH,BULLISH,NEUTRAL. No further explanation. \n Got it?"
+                        I will share news headline, stock symbol and article. \
+                        You will only answer as:\n\n BEARISH,BULLISH,NEUTRAL. \
+                        No further explanation. \n Got it?"
 
         message_history.append({"content": system_message, "role": "user"})
         self.chat(message_history)
 
         # Send the article to the OpenAI API
         user_message = "{}\n{}\n{}".format(title, symbol, article)
```

### Comparing `py_alpaca_daily_losers-0.3.4/py_alpaca_daily_losers/src/slack.py` & `py_alpaca_daily_losers-1.0.0/src/alpaca_daily_losers/slack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 
+from dotenv import load_dotenv
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
-from dotenv import load_dotenv
-
 load_dotenv()
 
 # Load environment variables
 production = os.getenv("PRODUCTION")
 slack_token = os.getenv("SLACK_ACCESS_TOKEN")
 
 
@@ -44,16 +43,14 @@
             response = client.chat_postMessage(
                 channel=channel, text=f"{message}", username=username
             )
             assert response["message"]["text"] == f"{message}"
         except SlackApiError as e:
             # You will get a SlackApiError if "ok" is False
             assert e.response["ok"] is False
-            assert e.response[
-                "error"
-            ]  # str like 'invalid_auth', 'channel_not_found'
+            assert e.response["error"]  # str like 'invalid_auth', 'channel_not_found'
             print(f"Got an error: {e.response['error']}")
             # Also receive a corresponding status_code
             assert isinstance(e.response.status_code, int)
             print(f"Received a response status_code: {e.response.status_code}")
         # else:
         #     print(f"Message sent successfully to {channel}")
```

