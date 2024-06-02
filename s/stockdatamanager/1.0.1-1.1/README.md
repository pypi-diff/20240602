# Comparing `tmp/stockdatamanager-1.0.1.tar.gz` & `tmp/stockdatamanager-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdatamanager-1.0.1.tar", last modified: Fri May 31 19:50:28 2024, max compression
+gzip compressed data, was "stockdatamanager-1.1.tar", last modified: Sun Jun  2 11:53:04 2024, max compression
```

## Comparing `stockdatamanager-1.0.1.tar` & `stockdatamanager-1.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:50:28.751527 stockdatamanager-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-31 19:50:28.751527 stockdatamanager-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:50:28.751527 stockdatamanager-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:50:28.747527 stockdatamanager-1.0.1/stockdatamanager/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/stockdatamanager/ToDo.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/stockdatamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/stockdatamanager/customerrors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/stockdatamanager/datafetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    51839 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/stockdatamanager/indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    69771 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/stockdatamanager/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/stockdatamanager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:50:28.747527 stockdatamanager-1.0.1/stockdatamanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-31 19:50:28.000000 stockdatamanager-1.0.1/stockdatamanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-31 19:50:28.000000 stockdatamanager-1.0.1/stockdatamanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:50:28.000000 stockdatamanager-1.0.1/stockdatamanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 19:50:28.000000 stockdatamanager-1.0.1/stockdatamanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 19:50:28.000000 stockdatamanager-1.0.1/stockdatamanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:50:28.747527 stockdatamanager-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-31 19:49:44.000000 stockdatamanager-1.0.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-02 11:50:56.000000 stockdatamanager-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-06-02 11:53:04.379710 stockdatamanager-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-06-02 11:50:56.000000 stockdatamanager-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 11:53:04.379710 stockdatamanager-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-02 11:50:56.000000 stockdatamanager-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/stockdatamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/customerrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/datafetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51839 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80915 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26534 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/stockdatamanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-02 11:50:56.000000 stockdatamanager-1.1/tests/test.py
```

### Comparing `stockdatamanager-1.0.1/LICENSE` & `stockdatamanager-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stockdatamanager-1.0.1/PKG-INFO` & `stockdatamanager-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdatamanager
-Version: 1.0.1
+Version: 1.1
 Summary: A comprehensive library for financial analysis
 Home-page: https://github.com/GiorgioMB/stockdatafetcher/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,23 +17,24 @@
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: matplotlib>=3.4.2
 Requires-Dist: seaborn>=0.11.1
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: arch>=4.19
 Requires-Dist: optuna>=2.10.0
+Requires-Dist: torch>=2.2.1
 
 # StockDataManager
 This Python library offers a combination of technical analysis tools and fundamental data retrieval functionalities, designed to support investors, researchers, and enthusiasts in the financial markets. 
 
 This Python library provides a comprehensive suite of tools for both technical and fundamental analysis, along with more advanced options analysis features. Utilizing the yfinance library, it provides easy access to historical stock data, financial statements, and key financial metrics from Yahoo Finance, alongside a suite of technical indicators for market analysis as well as options analysis tools.
 
 ## Features
 - **Technical Analysis (`IndicatorCalculator` Class)**: Over 30 technical indicators, including Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, and more, to dissect stock market trends and volatility.
-- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for in-depth fundamental analysis.
+- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for fundamental analysis.
 - **Options Analysis** (`Greeks` and `OptionPricing` Classes): Calculate options greeks and simulate option prices using various models. Supports both European and American options.
 
 ## Installation
 
 ```bash
 pip install stockdatamanager
 ```
```

### Comparing `stockdatamanager-1.0.1/README.md` & `stockdatamanager-1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # StockDataManager
 This Python library offers a combination of technical analysis tools and fundamental data retrieval functionalities, designed to support investors, researchers, and enthusiasts in the financial markets. 
 
 This Python library provides a comprehensive suite of tools for both technical and fundamental analysis, along with more advanced options analysis features. Utilizing the yfinance library, it provides easy access to historical stock data, financial statements, and key financial metrics from Yahoo Finance, alongside a suite of technical indicators for market analysis as well as options analysis tools.
 
 ## Features
 - **Technical Analysis (`IndicatorCalculator` Class)**: Over 30 technical indicators, including Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, and more, to dissect stock market trends and volatility.
-- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for in-depth fundamental analysis.
+- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for fundamental analysis.
 - **Options Analysis** (`Greeks` and `OptionPricing` Classes): Calculate options greeks and simulate option prices using various models. Supports both European and American options.
 
 ## Installation
 
 ```bash
 pip install stockdatamanager
 ```
```

### Comparing `stockdatamanager-1.0.1/setup.py` & `stockdatamanager-1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module sets up the package for distribution."""
 from setuptools import setup, find_packages
 
 setup(
     name='stockdatamanager',
-    version='1.0.1',
+    version='1.1',
     packages=find_packages(),
     description='A comprehensive library for financial analysis',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/stockdatafetcher/',
@@ -20,11 +20,12 @@
         'numpy>=1.23',
         'scipy>=1.7.1',
         'matplotlib>=3.4.2',
         'seaborn>=0.11.1',
         'scikit-learn>=1.4.1.post1',
         'statsmodels>=0.14.1',
         'arch>=4.19',
-        'optuna>=2.10.0'
+        'optuna>=2.10.0',
+        'torch>=2.2.1'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `stockdatamanager-1.0.1/stockdatamanager/datafetcher.py` & `stockdatamanager-1.1/stockdatamanager/datafetcher.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-1.0.1/stockdatamanager/indicators.py` & `stockdatamanager-1.1/stockdatamanager/indicators.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-1.0.1/stockdatamanager/options.py` & `stockdatamanager-1.1/stockdatamanager/options.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 It allows for calculations of option Greeks and prices either using tree methods or finite difference methods among others. 
 It supports both European and American options for price calculation.
 Classes:
 - Greeks: Calculate option Greeks (Delta, Gamma, Vega, etc.) using the Black-Scholes formula.
 - OptionPricing: Main class for option pricing that utilizes different numerical methods and models including GARCH for volatility modeling.
 The design favors flexibility in choosing pricing methods and models, offering tools for both simple and advanced option pricing scenarios.
 """
+import random
 from stockdatamanager.customerrors import MethodError
+from sympy import use
 from .datafetcher import Fetcher
-from .utils import _SMA, _EMA, _SARIMAX_model
+from .utils import _SMA, _EMA, _SARIMAX_model, _AutoEncoder
 import pandas as pd
 import numpy as np
 import yfinance as yf
 import re
 from typing import Union
 from scipy.stats import norm
-from scipy import linalg
-from scipy.stats import linregress
+from scipy import linalg, optimize
 import matplotlib.pyplot as plt
 import seaborn as sns
 import arch
 import optuna
 import math
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 import sys
+import torch
+from sklearn.metrics import mean_squared_error
 
 class Greeks(object):
   """
   Class to calculate the greeks for an option
   Inputs:
   - ticker: str, the ticker of the stock
   - call: bool, whether the option is a call or a put
@@ -41,20 +44,22 @@
                call: bool,
                identification: Union[str, int],
                verbose: bool = False):
     self.fetcher = Fetcher(ticker)
     self.df, self.yf_ticker = self.fetcher.df, self.fetcher.yf_stock
     if type(identification) == str:
      self.option_chain = self.yf_ticker.option_chain().calls if call else self.yf_ticker.option_chain().puts
-     self.option = self.option_chain[self.option_chain['contractSymbol'] == identification]
+     self.option = self.option_chain[self.option_chain['contractSymbol'] == identification].reset_index(drop=True)
+     self.option = self.option.iloc[0]
     elif type(identification) == int:
       self.option = self.yf_ticker.option_chain().calls.iloc[identification] if call else self.yf_ticker.option_chain().puts.iloc[identification]
     else:
       raise ValueError('identification must be either a string or an integer')
     self.verbose = verbose
+    self._id = identification
     self.date = self.calculate_expiration()
     self.call = call
 
   def from_name_to_datestr(self, s: str) -> str:
     """Helper function to convert the contract symbol to a date string"""
     if self.verbose:
       print(f"Processing {s}")
@@ -65,15 +70,15 @@
     else:
         return "No date found"
   
   def calculate_expiration(self) -> pd.Timestamp:
     """Function to calculate the expiration date of the option"""
     if self.verbose:
       print("Calculating expiration date")
-    to_process = self.option['contractSymbol']
+    to_process = self.option['contractSymbol'] if isinstance(self._id, int) else self._id
     date_str = self.from_name_to_datestr(to_process)
     date = pd.to_datetime(date_str)
     return date
 
   def calculate_delta(self, risk_free_rate_horizon: str = '13 weeks') -> float:
     """
     Method to calculate the delta of the option fed into the class, using the Black-Scholes formula.
@@ -388,15 +393,15 @@
     self.is_call = call
     self.is_european = not american
     self.verbose = verbose
 
   @property
   def dt(self) -> float:
     """ Single time step, in years """
-    return self.T / float(self.N)
+    return abs(self.T / float(self.N))
 
   @property
   def df(self) -> float:
     """ The discount factor """
     return math.exp(-(self.r - self.div) * self.dt)  
 
 class _FiniteDifferences(object):
@@ -1063,69 +1068,64 @@
                call: bool,
                american: bool,
                risk_free_rate: Union[str, float],
                identification: Union[str, int],
                risk_free_rate_approximation: str = 'last_observed',
                volatility: float = None,
                use_yfinance_volatility: bool = True,
+               use_garch: bool = False,
+               use_autoencoder: bool = False,
                optimize_garch: bool = False,
+               optimize_autoencoder: bool = False,
                optimization_rounds: int = 100,
                verbose: bool = False,
                risk_free_rate_approximation_parameters: dict = {},
+               autoencoder_parameters: dict = {},
                num_of_days_risk_free_rate: int = 252,
                num_of_days_volatility: int = 252,
+               random_state: int = 42,
                ):
     """
     Class to price options using different methods.
     Inputs:
     - ticker: str, can be either the name of the company or the ticker
     - call: bool, whether the option is a call or a put
     - american: bool, whether the option is American or European
     - risk_free_rate: either a string representing the horizon or a value
     - identification: either a string representing the contract symbol or an integer representing the index of the option within the chain
     - risk_free_rate_approximation: str, the method to approximate the risk-free rate, can be 'last_observed', 'SMA', 'EMA', 'SARIMAX'
     - volatility: float, the volatility of the underlying asset
-    - use_yfinance_volatility: bool, whether to use the volatility from Yahoo Finance if no volatility is provided. If False, a GARCH model will be used
+    - use_yfinance_volatility: bool, whether to use the volatility from Yahoo Finance if no volatility is provided
+    - use_garch: bool, whether to use the GARCH model to estimate the volatility
+    - use_autoencoder: bool, whether to use the autoencoder model to estimate the volatility
     - optimize_garch: bool, whether to optimize the GARCH model for the volatility
     - optimization_rounds: int, the number of rounds to optimize the GARCH model
     - verbose: bool, whether to print the steps of the process
     - risk_free_rate_approximation_parameters: dict, the parameters to be passed to the risk-free rate approximation method
+    - autoencoder_parameters: dict, the parameters to be passed to the autoencoder model
     - num_of_days_risk_free_rate: int, the number of days to consider for the risk-free rate approximation
     - num_of_days_volatility: int, the number of days to consider for the volatility approximation
+    - random_state: int, the random state for reproducibility
     """
-    if type(ticker) != str:
-      raise ValueError('ticker must be a string')
-    if type(call) != bool:
-      raise ValueError('call must be a boolean')
-    if type(american) != bool:
-      raise ValueError('american must be a boolean')
-    if (type(volatility) != float) and (volatility is not None) and (type(volatility) != int):
-      raise ValueError('volatility must be a number')
-    if type(use_yfinance_volatility) != bool:
-      raise ValueError('use_yfinance_volatility must be a boolean')
-    if type(optimize_garch) != bool:
-      raise ValueError('optimize_garch must be a boolean')
-    if type(optimization_rounds) != int:
-      raise ValueError('optimization_rounds must be an integer')
-    if type(verbose) != bool:
-      raise ValueError('verbose must be a boolean')
+    self._assertions(ticker, call, american, risk_free_rate, identification, risk_free_rate_approximation, volatility, use_yfinance_volatility, optimize_garch, optimization_rounds, verbose, risk_free_rate_approximation_parameters, num_of_days_risk_free_rate, num_of_days_volatility, use_garch, use_autoencoder, optimize_autoencoder, autoencoder_parameters, random_state)
     self.fetcher = Fetcher(ticker)
+    self.random_state = random_state
     self.dataframe, self.yf_ticker = self.fetcher.df, self.fetcher.yf_stock
-    if type(identification) == str:
+    self._id = identification
+    if isinstance(identification, str):
       self.option_chain = self.yf_ticker.option_chain().calls if call else self.yf_ticker.option_chain().puts
-      self.option = self.option_chain[self.option_chain['contractSymbol'] == identification]
-    elif type(identification) == int:
+      self.option = self.option_chain[self.option_chain['contractSymbol'] == identification].reset_index(drop = True)
+      self.option = self.option.iloc[0]
+    elif isinstance(identification, int):
       self.option = self.yf_ticker.option_chain().calls.iloc[identification] if call else self.yf_ticker.option_chain().puts.iloc[identification]
-    else:
-      raise ValueError('identification must be either a string or an integer')
     self.verbose = verbose
     self.date = self._calculate_expiration()
     self.is_call = call
     self.dividend_yield = self.fetcher.get_dividend_yield()
-    if type(risk_free_rate) == str:
+    if isinstance(risk_free_rate, str):
       self.historical = self.fetcher.get_risk_free_rate(risk_free_rate)['Close'].tail(num_of_days_risk_free_rate)
       if risk_free_rate_approximation == 'last_observed':
         self.risk_free_rate = self.historical.iloc[-1]
       elif risk_free_rate_approximation == 'SMA':
         if 'window' not in risk_free_rate_approximation_parameters.keys():
           print("Window not passed, using default value of 20")
         if 'num_of_steps' not in risk_free_rate_approximation_parameters.keys():
@@ -1141,69 +1141,175 @@
           print("Number of steps not passed, using default value of 1")
         window = risk_free_rate_approximation_parameters.get('window', 20)
         num_of_steps = risk_free_rate_approximation_parameters.get('num_of_steps', 1)
         self.risk_free_rate = _EMA(self.historical, window).predict_val(num_of_steps)
       elif risk_free_rate_approximation == 'SARIMAX':
         if verbose:
           print("The SARIMAX method accepts the following optional parameters:\n - exog: pd.Series, exogenous variable to use in the model")
-          print("- forecast_steps: int, number of forecast steps")
+          print("- forecast_steps: int, number of steps to forecast")
+          print(" - exog: pd.Series, exogenous variable to use in the model")
           print("- optimize: bool, whether to optimize the hyperparameters")
           print("- optimization_rounds: int, number of rounds to optimize the hyperparameters")
           print("- test_size: float, size of the test set")
           print("- random_state: int, random state for reproducibility")
-          print("- p: int, AR order")
-          print("- d: int, differencing order")
-          print("- q: int, MA order")
-          print("- P: int, seasonal AR order")
-          print("- D: int, seasonal differencing order")
-          print("- Q: int, seasonal MA order")
-          print("- s: int, seasonal period")
-          print("- trend: str, trend parameter")
+          print("- verbose: bool, whether to print the steps of the process")
+          print("- p: int, the autoregressive order")
+          print("- d: int, the differencing order")
+          print("- q: int, the moving average order")
+          print("- P: int, the seasonal autoregressive order")
+          print("- D: int, the seasonal differencing order")
+          print("- Q: int, the seasonal moving average order")
+          print("- s: int, the number of periods in a season")
+          print("- trend: str, the trend in the model")
           print("- measure_error: bool, whether to measure the error")
-          print("- time_varying_regression: bool, whether to use time varying regression")
-          print("- mle_regression: bool, whether to use MLE regression")
+          print("- time_varying_regression: bool, whether to use time-varying regression")
+          print("- mle_regression: bool, whether to use maximum likelihood estimation for regression")
           print("- simple_differencing: bool, whether to use simple differencing")
           print("- enforce_stationarity: bool, whether to enforce stationarity")
           print("- enforce_invertibility: bool, whether to enforce invertibility")
-          print("- hamilton_representation: bool, whether to use Hamilton representation")
-          print("- concentrate_scale: bool, whether to concentrate scale")
-          print("- trend_offset: int, trend offset")
-          print("- use_exact_diffuse: bool, whether to use exact diffuse")
+          print("- hamilton_representation: bool, whether to use the Hamilton representation")
+          print("- concentrate_scale: bool, whether to concentrate the scale")
+          print("- trend_offset: bool, whether to use a trend offset")
+          print("- use_exact_diffuse_initialization: bool, whether to use exact diffuse initialization")
+        steps = None
         if 'forecast_steps' in risk_free_rate_approximation_parameters.keys():
           steps = risk_free_rate_approximation_parameters['forecast_steps']
           risk_free_rate_approximation_parameters.pop('forecast_steps')
-        if steps is None or not isinstance(steps, int):
+        if steps is None:
+          steps = 1
+        elif not isinstance(steps, int):
+          print("Warning: forecast_steps must be an integer, using default value of 1")
           steps = 1
         model = _SARIMAX_model(self.historical, **risk_free_rate_approximation_parameters)
         self.risk_free_rate = np.mean(model.forecast(steps))
-
-    elif type(risk_free_rate) == float or type(risk_free_rate) == int:
+    elif isinstance(risk_free_rate, (float, int)):
       self.risk_free_rate = risk_free_rate
-    else:
-      raise ValueError('risk_free_rate must be either a string representing the horizon or a value')
-    self.r = self.risk_free_rate * 100
+    self.r = self.risk_free_rate
     self.S = self.dataframe['Close'].iloc[-1]
     self.T = (self.date - pd.to_datetime('today')).days / 365
     self.K = self.option['strike']
     self.american = american
     self.num_of_days_volatility = num_of_days_volatility
+    if num_of_days_volatility >= len(self.dataframe): 
+      raise ValueError("Number of days for volatility must be less than the length of the dataframe")
     if use_yfinance_volatility:
       self.sigma = self.option['impliedVolatility']
-    else:
-      if optimize_garch:
-        garch_params = self.optimize_garch_model(optimization_rounds)
-        self.build_garch_model(**garch_params)
+    elif use_autoencoder or use_garch:
+      if use_garch:
+        if optimize_garch:
+          garch_params = self.optimize_garch_model(optimization_rounds)
+          self.build_garch_model(**garch_params)
+        else:
+          self.build_garch_model('GARCH', 'Constant', 1, 1, 'normal', 0, 2, None, None) 
+        res = self.garch_model.fit(disp='off')
+        sigma = res.conditional_volatility
+        self.sigma = sigma[-1]
       else:
-        self.build_garch_model('GARCH', 'Constant', 1, 1, 'normal', 0, 2, None, None) 
-      res = self.garch_model.fit(disp='off')
-      sigma = res.conditional_volatility
-      self.sigma = sigma[-1]
+        if num_of_days_volatility >= len(self.dataframe) - 1:
+          raise ValueError("Number of days for volatility must be less than the length of the dataframe minus 1, as num_of_days_volatility observations are used for testing and thus not used in training")
+        if optimize_autoencoder:
+          autoencoder_params = self.optimize_autoencoder_model(optimization_rounds)
+          self.build_autoencoder_model(**autoencoder_params)
+        else:
+          if verbose:
+            print("The Autoencoder method accepts the following optional parameters:\n - input_size: int, the size of the input layer")
+            print("- hidden_size: int, the size of the hidden layer")
+            print("- num_layers: int, the number of layers")
+            print("- epochs: int, the number of epochs")
+            print("- batch_size: int, the batch size")
+            print("- learning_rate: float, the learning rate")
+            print("- dropout: float, the dropout rate")
+            print("- test_size: float, the size of the test set")
+            print("- device: torch.device, the device to use")
+          if len(autoencoder_parameters) == 0:
+            autoencoder_parameters = {'input_size': 10, 
+                                      'hidden_size': 5,
+                                      'num_layers': 3,
+                                      'epochs': 10, 
+                                      'batch_size': 32, 
+                                      'learning_rate': 1e-3,
+                                      'dropout': 0.2,
+                                      'test_size': 0.2,
+                                      'device': torch.device('cuda' if torch.cuda.is_available() else 'cpu')}
+          self.build_autoencoder_model(**autoencoder_parameters)
+        X = self.dataframe['Close'].pct_change().dropna()
+        y = self.dataframe.loc[X.index, 'Volatility'].dropna()
+        X = X.loc[y.index]
+        X_test = X.iloc[-self.num_of_days_volatility:]
+        X_test, _ = self.autoencoder_model.validate_data(X_test, X_test)
+        X_test = self.autoencoder_model.window_data(X_test, self.autoencoder_model.input_size)
+        predicted_values = self.autoencoder_model.predict(X_test)[1].to('cpu').detach().numpy().flatten()
+        self.sigma = np.mean(predicted_values)
     if volatility is not None:
       self.sigma = volatility
 
+  def _assertions(self, ticker, call, american, risk_free_rate, identification, risk_free_rate_approximation, volatility, use_yfinance_volatility, optimize_garch, optimization_rounds, verbose, risk_free_rate_approximation_parameters, num_of_days_risk_free_rate, num_of_days_volatility, use_garch, use_autoencoder, optimize_autoencoder, autoencoder_parameters, random_state):
+    if not isinstance(ticker, str):
+      raise ValueError("Ticker must be a string")
+    if not isinstance(call, bool):
+      raise ValueError("Call must be a boolean")
+    if not isinstance(american, bool):
+      raise ValueError("American must be a boolean")
+    if not isinstance(risk_free_rate, (str, float)):
+      raise ValueError("Risk-Free Rate must be a string or a float")
+    if not isinstance(identification, (str, int)):
+      raise ValueError("Identification must be a string or an integer")
+    if not isinstance(volatility, (float, int)) and volatility is not None:
+      raise ValueError("Volatility must be a number")
+    if not isinstance(use_yfinance_volatility, bool):
+      raise ValueError("Use Yahoo Finance Volatility must be a boolean")
+    if not isinstance(optimize_garch, bool):
+      raise ValueError("Optimize GARCH must be a boolean")
+    if not isinstance(optimization_rounds, int):
+      raise ValueError("Optimization Rounds must be an integer")
+    if optimization_rounds < 1:
+      raise ValueError("Optimization Rounds must be greater than 0")
+    if not isinstance(verbose, bool):
+      raise ValueError("Verbose must be a boolean")
+    if not isinstance(risk_free_rate_approximation_parameters, dict):
+      raise ValueError("Risk-Free Rate Approximation Parameters must be a dictionary")
+    if not isinstance(num_of_days_risk_free_rate, int):
+      raise ValueError("Number of Days Risk-Free Rate must be an integer")
+    if not isinstance(num_of_days_volatility, int):
+      raise ValueError("Number of Days Volatility must be an integer")
+    if risk_free_rate_approximation not in ('last_observed', 'SMA', 'EMA', 'SARIMAX'):
+      raise ValueError("Risk-Free Rate Approximation must be one of 'last_observed', 'SMA', 'EMA', 'SARIMAX'")
+    if not isinstance(use_garch, bool):
+      raise ValueError("Use GARCH must be a boolean")
+    if not isinstance(use_autoencoder, bool):
+      raise ValueError("Use Autoencoder must be a boolean")
+    if use_garch and use_autoencoder:
+      raise ValueError("Only one of GARCH and Autoencoder can be used")
+    if (not use_garch) and (not use_autoencoder) and (not use_yfinance_volatility) and (volatility is None):
+      raise ValueError("At least one method must be used to estimate the volatility")
+    if (use_garch or use_autoencoder or use_yfinance_volatility) and (volatility is not None):
+      print("Warning: Both a volatility and a method to estimate the volatility have been passed, the passed volatility will be used")
+    if not isinstance(optimize_autoencoder, bool):
+      raise ValueError("Optimize Autoencoder must be a boolean")
+    if not isinstance(autoencoder_parameters, dict):
+      raise ValueError("Autoencoder Parameters must be a dictionary")
+    if not isinstance(random_state, int):
+      raise ValueError("Random State must be an integer")
+    if random_state < 0:
+      raise ValueError("Random State must be greater than 0")
+    if len(autoencoder_parameters) > 0 and optimize_autoencoder:
+      print("Warning: Autoencoder parameters have been passed, but the optimization flag is set to True, the parameters will be ignored")
+    if len(risk_free_rate_approximation_parameters) > 0 and risk_free_rate_approximation == 'last_observed':
+      print("Warning: Risk-Free Rate Approximation parameters have been passed, but the method is set to last_observed, the parameters will be ignored")
+    if optimize_garch and not use_garch:
+      print("Warning: Optimize GARCH is set to True, but GARCH is not being used, the optimization will not be performed")
+    if optimize_autoencoder and not use_autoencoder:
+      print("Warning: Optimize Autoencoder is set to True, but Autoencoder is not being used, the optimization will not be performed")
+    if num_of_days_volatility < 1:
+      raise ValueError("Number of Days Volatility must be greater than 0")
+    if (use_autoencoder or use_garch) and use_yfinance_volatility:
+      print("Warning: Both Yahoo Finance Volatility and another method to estimate the volatility have been passed, the Yahoo Finance Volatility will be used")
+    if verbose:
+      print("All assertions passed")
+    
   def _from_name_to_datestr(self, s: str) -> str:
     """Helper function to convert the contract symbol to a date string"""
     if self.verbose:
       print(f"Processing {s}")
     match = re.search(r'[A-Za-z](\d{2})(\d{2})(\d{2})[CP]', s)
     if match:
         year, month, day = match.groups()
@@ -1211,33 +1317,36 @@
     else:
         return "No date found"
   
   def _calculate_expiration(self) -> pd.Timestamp:
     """Function to calculate the expiration date of the option"""
     if self.verbose:
       print("Calculating expiration date")
-    to_process = self.option['contractSymbol']
+    to_process = self.option['contractSymbol'] if isinstance(self._id, int) else self._id
     date_str = self._from_name_to_datestr(to_process)
     date = pd.to_datetime(date_str)
     return date 
   
   def calculate_option_price(self, method: str, describe: bool = False, **kwargs) -> float:
     """
     Main wrapper function to calculate the price of an option using the specified method.
     Inputs:
       - method: str, the method to use for pricing
       - describe: bool, whether to describe the method
       - kwargs: additional arguments to be passed to the method
     
     Accepted methods:
+    - Black-Scholes: Black-Scholes Method
+    - Monte Carlo: Monte Carlo Method
     - Binomial Tree Methods: Binomial Tree, Binomial Lattice Tree, Cox-Ross-Rubinstein, Leisen-Reimer Tree
     - Trinomial Tree Methods: Trinomial Tree, Trinomial Lattice Tree
     - Finite Difference Methods: Explicit Finite Difference, Implicit Finite Difference, Crank-Nicolson Finite Difference
     """
     method = method.replace(' ', '').lower()
+
     if method in ('blackscholes', 'black-scholes', 'bs', 'black_scholes'):
       if self.american:
         raise MethodError("The Black-Scholes method is only available for European options")
       if describe:
         print("The Black-Scholes Method requires no additional values")
       price = self.black_scholes()
       return price
@@ -1523,9 +1632,58 @@
             return float('inf')
     print("Warning: This function is experimental, and may throw errors in the optimization process. Use at your own risk.")
     study = optuna.create_study(direction='minimize')
     study.optimize(objective, n_trials=optimization_trials)
     if self.verbose: print("Optimization complete")
     return study.best_params
   
+  def build_autoencoder_model(self, input_size, hidden_size, num_layers, dropout, learning_rate, epochs, batch_size, device, test_size):
+    if self.verbose: print("Building Autoencoder model")
+    X = self.dataframe['Close'].pct_change().dropna()
+    y = self.dataframe.loc[X.index, 'Volatility'].dropna()
+    X = X.loc[y.index]
+    X_train= X.iloc[:-self.num_of_days_volatility]
+    y_train = y.iloc[:-self.num_of_days_volatility]
+    model = _AutoEncoder(input_size=input_size, hidden_size=hidden_size, num_layers=num_layers, dropout=dropout, test_size = test_size, verbose=self.verbose, device=device, random_state = self.random_state)
+    model = model.fit(X_train, y_train, learning_rate=learning_rate, epochs=epochs, batch_size=batch_size)
+    self.autoencoder_model = model
+
+  def optimize_autoencoder_model(self, optimization_trials) -> dict:
+    X = self.dataframe['Close'].pct_change().dropna()
+    y = self.dataframe.loc[X.index, 'Volatility'].dropna()
+    X = X.loc[y.index]
+    X_test = X.iloc[-self.num_of_days_volatility:]
+    y_test = y.iloc[-self.num_of_days_volatility:]
+    if self.verbose: print(X_test.shape, y_test.shape)
+    def objective(trial):
+      nonlocal X_test, y_test
+      input_size = trial.suggest_int('input_size', 1, 100)
+      hidden_size = trial.suggest_int('hidden_size', 1, input_size)
+      num_layers = trial.suggest_int('num_layers', 1, 10)
+      dropout = trial.suggest_float('dropout', 0, 1)
+      learning_rate = trial.suggest_float('learning_rate', 1e-6, 1e-1)
+      epochs = trial.suggest_int('epochs', 1, 50)
+      batch_size = trial.suggest_int('batch_size', 1, 100)
+      device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+      test_size = trial.suggest_float('test_size', 0.1, 0.5)
+      if self.verbose: print(f"Optimizing with parameters:\n- input: {input_size},\n- hidden: {hidden_size},\n- layers: {num_layers},\n- dropout: {dropout},\n- learning rate: {learning_rate},\n- epochs: {epochs},\n- batch size:{batch_size},\n- test size:{test_size}")
+      try:
+        self.build_autoencoder_model(input_size, hidden_size, num_layers, dropout, learning_rate, epochs, batch_size, device, test_size)
+        if self.verbose: print("Model built")
+        X_test, y_test = self.autoencoder_model.validate_data(X_test, y_test)
+        y_test = y_test[self.autoencoder_model.input_size-1:]
+        X_test = self.autoencoder_model.window_data(X_test, self.autoencoder_model.input_size)
+        predicted_values = self.autoencoder_model.predict(X_test)[1].to('cpu').detach().numpy().flatten()
+        if self.verbose: print("Predicted values")
+        mse = mean_squared_error(predicted_values, y_test)
+        return mse
+      except Exception as e:
+        print(f"Error with parameters {input_size}, {hidden_size}, {num_layers}, {dropout}, {learning_rate}, {epochs}, {batch_size}, {test_size}: {e}")
+        return float('inf')
+    if self.verbose: print("Warning: This function is experimental, and may throw errors in the optimization process. Use at your own risk.")
+    study = optuna.create_study(direction='minimize')
+    study.optimize(objective, n_trials=optimization_trials)
+    if self.verbose: print("Optimization complete")
+    return study.best_params
+
   def __repr__(self) -> str:
     return f"Option of {self.yf_ticker.ticker}\nStrike Price: {self.K}\nRisk-Free Rate: {self.risk_free_rate}\nExpiration Date: {self.date}\nDividend Yield: {self.dividend_yield}\nPrice of the stock: {self.S}\nVolatility: {self.sigma}\nIs Call: {self.is_call}\nIs an american option: {self.american}\n"
```

### Comparing `stockdatamanager-1.0.1/stockdatamanager.egg-info/PKG-INFO` & `stockdatamanager-1.1/stockdatamanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdatamanager
-Version: 1.0.1
+Version: 1.1
 Summary: A comprehensive library for financial analysis
 Home-page: https://github.com/GiorgioMB/stockdatafetcher/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,23 +17,24 @@
 Requires-Dist: scipy>=1.7.1
 Requires-Dist: matplotlib>=3.4.2
 Requires-Dist: seaborn>=0.11.1
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: arch>=4.19
 Requires-Dist: optuna>=2.10.0
+Requires-Dist: torch>=2.2.1
 
 # StockDataManager
 This Python library offers a combination of technical analysis tools and fundamental data retrieval functionalities, designed to support investors, researchers, and enthusiasts in the financial markets. 
 
 This Python library provides a comprehensive suite of tools for both technical and fundamental analysis, along with more advanced options analysis features. Utilizing the yfinance library, it provides easy access to historical stock data, financial statements, and key financial metrics from Yahoo Finance, alongside a suite of technical indicators for market analysis as well as options analysis tools.
 
 ## Features
 - **Technical Analysis (`IndicatorCalculator` Class)**: Over 30 technical indicators, including Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, and more, to dissect stock market trends and volatility.
-- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for in-depth fundamental analysis.
+- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for fundamental analysis.
 - **Options Analysis** (`Greeks` and `OptionPricing` Classes): Calculate options greeks and simulate option prices using various models. Supports both European and American options.
 
 ## Installation
 
 ```bash
 pip install stockdatamanager
 ```
```

### Comparing `stockdatamanager-1.0.1/tests/test.py` & `stockdatamanager-1.1/tests/test.py`

 * *Files identical despite different names*

