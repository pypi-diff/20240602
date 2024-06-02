# Comparing `tmp/stockdatamanager-1.1.tar.gz` & `tmp/stockdatamanager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdatamanager-1.1.tar", last modified: Sun Jun  2 11:53:04 2024, max compression
+gzip compressed data, was "stockdatamanager-1.1.1.tar", last modified: Sun Jun  2 13:16:32 2024, max compression
```

## Comparing `stockdatamanager-1.1.tar` & `stockdatamanager-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-02 11:50:56.000000 stockdatamanager-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-06-02 11:53:04.379710 stockdatamanager-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-06-02 11:50:56.000000 stockdatamanager-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 11:53:04.379710 stockdatamanager-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-02 11:50:56.000000 stockdatamanager-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/stockdatamanager/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/customerrors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/datafetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    51839 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    80915 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    26534 2024-06-02 11:50:56.000000 stockdatamanager-1.1/stockdatamanager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/stockdatamanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 11:53:04.000000 stockdatamanager-1.1/stockdatamanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:53:04.379710 stockdatamanager-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-02 11:50:56.000000 stockdatamanager-1.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:16:32.562883 stockdatamanager-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-06-02 13:16:32.562883 stockdatamanager-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 13:16:32.562883 stockdatamanager-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:16:32.558883 stockdatamanager-1.1.1/stockdatamanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/stockdatamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/stockdatamanager/customerrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/stockdatamanager/datafetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51839 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/stockdatamanager/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81998 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/stockdatamanager/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27428 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/stockdatamanager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:16:32.562883 stockdatamanager-1.1.1/stockdatamanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-06-02 13:16:32.000000 stockdatamanager-1.1.1/stockdatamanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-06-02 13:16:32.000000 stockdatamanager-1.1.1/stockdatamanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:16:32.000000 stockdatamanager-1.1.1/stockdatamanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-02 13:16:32.000000 stockdatamanager-1.1.1/stockdatamanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 13:16:32.000000 stockdatamanager-1.1.1/stockdatamanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:16:32.558883 stockdatamanager-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-02 13:14:24.000000 stockdatamanager-1.1.1/tests/test.py
```

### Comparing `stockdatamanager-1.1/LICENSE` & `stockdatamanager-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stockdatamanager-1.1/PKG-INFO` & `stockdatamanager-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdatamanager
-Version: 1.1
+Version: 1.1.1
 Summary: A comprehensive library for financial analysis
 Home-page: https://github.com/GiorgioMB/stockdatafetcher/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,22 +20,20 @@
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: arch>=4.19
 Requires-Dist: optuna>=2.10.0
 Requires-Dist: torch>=2.2.1
 
 # StockDataManager
-This Python library offers a combination of technical analysis tools and fundamental data retrieval functionalities, designed to support investors, researchers, and enthusiasts in the financial markets. 
-
-This Python library provides a comprehensive suite of tools for both technical and fundamental analysis, along with more advanced options analysis features. Utilizing the yfinance library, it provides easy access to historical stock data, financial statements, and key financial metrics from Yahoo Finance, alongside a suite of technical indicators for market analysis as well as options analysis tools.
+This Python library offers a comprehensive suite of tools for technical and fundamental analysis, along with options analysis capabilities. Utilizing the yfinance library, it facilitates access to historical stock data, financial statements, and key financial metrics from Yahoo Finance. It includes over 30 technical indicators and options analysis tools.
 
 ## Features
-- **Technical Analysis (`IndicatorCalculator` Class)**: Over 30 technical indicators, including Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, and more, to dissect stock market trends and volatility.
-- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for fundamental analysis.
-- **Options Analysis** (`Greeks` and `OptionPricing` Classes): Calculate options greeks and simulate option prices using various models. Supports both European and American options.
+- **Technical Analysis (`IndicatorCalculator` Class)**: Offers over 30 technical indicators like Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, etc., for analyzing market trends and volatility.
+- **Fundamental Analysis (`Fetcher` Class)**: Retrieve historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio).
+- **Options Analysis (`Greeks` and `OptionPricing` Classes)**: tools to calculate options greeks and simulate option prices using various models, with enhanced methods to estimate risk-free rates and volatility.
 
 ## Installation
 
 ```bash
 pip install stockdatamanager
 ```
 ## Quick Start
```

### Comparing `stockdatamanager-1.1/README.md` & `stockdatamanager-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # StockDataManager
-This Python library offers a combination of technical analysis tools and fundamental data retrieval functionalities, designed to support investors, researchers, and enthusiasts in the financial markets. 
-
-This Python library provides a comprehensive suite of tools for both technical and fundamental analysis, along with more advanced options analysis features. Utilizing the yfinance library, it provides easy access to historical stock data, financial statements, and key financial metrics from Yahoo Finance, alongside a suite of technical indicators for market analysis as well as options analysis tools.
+This Python library offers a comprehensive suite of tools for technical and fundamental analysis, along with options analysis capabilities. Utilizing the yfinance library, it facilitates access to historical stock data, financial statements, and key financial metrics from Yahoo Finance. It includes over 30 technical indicators and options analysis tools.
 
 ## Features
-- **Technical Analysis (`IndicatorCalculator` Class)**: Over 30 technical indicators, including Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, and more, to dissect stock market trends and volatility.
-- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for fundamental analysis.
-- **Options Analysis** (`Greeks` and `OptionPricing` Classes): Calculate options greeks and simulate option prices using various models. Supports both European and American options.
+- **Technical Analysis (`IndicatorCalculator` Class)**: Offers over 30 technical indicators like Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, etc., for analyzing market trends and volatility.
+- **Fundamental Analysis (`Fetcher` Class)**: Retrieve historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio).
+- **Options Analysis (`Greeks` and `OptionPricing` Classes)**: tools to calculate options greeks and simulate option prices using various models, with enhanced methods to estimate risk-free rates and volatility.
 
 ## Installation
 
 ```bash
 pip install stockdatamanager
 ```
 ## Quick Start
```

### Comparing `stockdatamanager-1.1/setup.py` & `stockdatamanager-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module sets up the package for distribution."""
 from setuptools import setup, find_packages
 
 setup(
     name='stockdatamanager',
-    version='1.1',
+    version='1.1.1',
     packages=find_packages(),
     description='A comprehensive library for financial analysis',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/stockdatafetcher/',
```

### Comparing `stockdatamanager-1.1/stockdatamanager/datafetcher.py` & `stockdatamanager-1.1.1/stockdatamanager/datafetcher.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-1.1/stockdatamanager/indicators.py` & `stockdatamanager-1.1.1/stockdatamanager/indicators.py`

 * *Files identical despite different names*

### Comparing `stockdatamanager-1.1/stockdatamanager/options.py` & `stockdatamanager-1.1.1/stockdatamanager/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This file contains classes and methods for option pricing and analysis, utilizing various financial models and numerical methods. 
 It allows for calculations of option Greeks and prices either using tree methods or finite difference methods among others. 
-It supports both European and American options for price calculation.
-Classes:
+It supports both European and American options for price calculation. 
+Classes include:
 - Greeks: Calculate option Greeks (Delta, Gamma, Vega, etc.) using the Black-Scholes formula.
-- OptionPricing: Main class for option pricing that utilizes different numerical methods and models including GARCH for volatility modeling.
-The design favors flexibility in choosing pricing methods and models, offering tools for both simple and advanced option pricing scenarios.
+- OptionPricing: Main class for option pricing that utilizes different numerical methods and models. This class supports GARCH and AutoEncoder for volatility modeling and risk-free rate approximations using SARIMAX, EMA, and SMA.
+- Helper classes designed for internal use that support the various methods and models implemented.
 """
 import random
 from stockdatamanager.customerrors import MethodError
 from sympy import use
 from .datafetcher import Fetcher
 from .utils import _SMA, _EMA, _SARIMAX_model, _AutoEncoder
 import pandas as pd
@@ -23,25 +23,35 @@
 import seaborn as sns
 import arch
 import optuna
 import math
 from abc import abstractmethod
 import sys
 import torch
-from sklearn.metrics import mean_squared_error
+from sklearn.metrics import mean_absolute_percentage_error
 
 class Greeks(object):
   """
   Class to calculate the greeks for an option
   Inputs:
   - ticker: str, the ticker of the stock
   - call: bool, whether the option is a call or a put
   - identification: Union[str, int], the contract symbol of the option or the index of the option in the option chain
                                      Note: to find the contract identifier, it is written as ticker-YY-MM-DD-C(or P)-strike price (omit the - and the strike price is in a thousands format, so 1000 is $1.00)
   - verbose: int, the verbosity of the output
+
+  Methods:
+  - calculate_delta: calculates the delta of the option
+  - calculate_gamma: calculates the gamma of the option
+  - calculate_vega: calculates the vega of the option
+  - (and nearly all the greeks, as explained in https://en.wikipedia.org/wiki/en:Greeks_(finance)?variant=zh-tw)
+
+  Example usage:
+    greek_calculator = Greeks('MSFT', True, 0, False)
+    delta = greek_calculator.calculate_delta(risk_free_horizon = '13 weeks')
   """
   def __init__(self, 
                ticker: str,
                call: bool,
                identification: Union[str, int],
                verbose: bool = False):
     self.fetcher = Fetcher(ticker)
@@ -1101,14 +1111,21 @@
     - optimization_rounds: int, the number of rounds to optimize the GARCH model
     - verbose: bool, whether to print the steps of the process
     - risk_free_rate_approximation_parameters: dict, the parameters to be passed to the risk-free rate approximation method
     - autoencoder_parameters: dict, the parameters to be passed to the autoencoder model
     - num_of_days_risk_free_rate: int, the number of days to consider for the risk-free rate approximation
     - num_of_days_volatility: int, the number of days to consider for the volatility approximation
     - random_state: int, the random state for reproducibility
+
+    Method:
+    - calculate_option_price: method to calculate the option price using many possible algorithms, including (but not limited to) Finite Differences, Tree Models and Monte Carlo simulations
+
+    Example usage:
+      pricer = OptionPricing('AAPL', True, True, 0)
+      price = pricer.calculate_option_price('monte_carlo', describe = True, display = True)
     """
     self._assertions(ticker, call, american, risk_free_rate, identification, risk_free_rate_approximation, volatility, use_yfinance_volatility, optimize_garch, optimization_rounds, verbose, risk_free_rate_approximation_parameters, num_of_days_risk_free_rate, num_of_days_volatility, use_garch, use_autoencoder, optimize_autoencoder, autoencoder_parameters, random_state)
     self.fetcher = Fetcher(ticker)
     self.random_state = random_state
     self.dataframe, self.yf_ticker = self.fetcher.df, self.fetcher.yf_stock
     self._id = identification
     if isinstance(identification, str):
@@ -1200,19 +1217,24 @@
           self.build_garch_model(**garch_params)
         else:
           self.build_garch_model('GARCH', 'Constant', 1, 1, 'normal', 0, 2, None, None) 
         res = self.garch_model.fit(disp='off')
         sigma = res.conditional_volatility
         self.sigma = sigma[-1]
       else:
+        X = self.dataframe['Close'].pct_change().dropna()
+        y = self.dataframe.loc[X.index, 'Volatility'].dropna()
+        X = X.loc[y.index]
         if num_of_days_volatility >= len(self.dataframe) - 1:
           raise ValueError("Number of days for volatility must be less than the length of the dataframe minus 1, as num_of_days_volatility observations are used for testing and thus not used in training")
         if optimize_autoencoder:
           autoencoder_params = self.optimize_autoencoder_model(optimization_rounds)
           self.build_autoencoder_model(**autoencoder_params)
+          _sarimax = _SARIMAX_model(X, optimize = True)
+          to_predict = _sarimax.forecast(num_of_days_volatility)
         else:
           if verbose:
             print("The Autoencoder method accepts the following optional parameters:\n - input_size: int, the size of the input layer")
             print("- hidden_size: int, the size of the hidden layer")
             print("- num_layers: int, the number of layers")
             print("- epochs: int, the number of epochs")
             print("- batch_size: int, the batch size")
@@ -1227,22 +1249,21 @@
                                       'epochs': 10, 
                                       'batch_size': 32, 
                                       'learning_rate': 1e-3,
                                       'dropout': 0.2,
                                       'test_size': 0.2,
                                       'device': torch.device('cuda' if torch.cuda.is_available() else 'cpu')}
           self.build_autoencoder_model(**autoencoder_parameters)
-        X = self.dataframe['Close'].pct_change().dropna()
-        y = self.dataframe.loc[X.index, 'Volatility'].dropna()
-        X = X.loc[y.index]
-        X_test = X.iloc[-self.num_of_days_volatility:]
-        X_test, _ = self.autoencoder_model.validate_data(X_test, X_test)
+          _sarimax = _SARIMAX_model(X)
+          to_predict = _sarimax.forecast(num_of_days_volatility)
+        X_test, _ = self.autoencoder_model.validate_data(to_predict, to_predict)
         X_test = self.autoencoder_model.window_data(X_test, self.autoencoder_model.input_size)
-        predicted_values = self.autoencoder_model.predict(X_test)[1].to('cpu').detach().numpy().flatten()
-        self.sigma = np.mean(predicted_values)
+        predicted_values = self.autoencoder_model.predict(X_test)[1]
+        print(predicted_values.shape)
+        self.sigma = torch.mean(predicted_values).item()
     if volatility is not None:
       self.sigma = volatility
 
   def _assertions(self, ticker, call, american, risk_free_rate, identification, risk_free_rate_approximation, volatility, use_yfinance_volatility, optimize_garch, optimization_rounds, verbose, risk_free_rate_approximation_parameters, num_of_days_risk_free_rate, num_of_days_volatility, use_garch, use_autoencoder, optimize_autoencoder, autoencoder_parameters, random_state):
     if not isinstance(ticker, str):
       raise ValueError("Ticker must be a string")
     if not isinstance(call, bool):
@@ -1665,21 +1686,21 @@
       batch_size = trial.suggest_int('batch_size', 1, 100)
       device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
       test_size = trial.suggest_float('test_size', 0.1, 0.5)
       if self.verbose: print(f"Optimizing with parameters:\n- input: {input_size},\n- hidden: {hidden_size},\n- layers: {num_layers},\n- dropout: {dropout},\n- learning rate: {learning_rate},\n- epochs: {epochs},\n- batch size:{batch_size},\n- test size:{test_size}")
       try:
         self.build_autoencoder_model(input_size, hidden_size, num_layers, dropout, learning_rate, epochs, batch_size, device, test_size)
         if self.verbose: print("Model built")
-        X_test, y_test = self.autoencoder_model.validate_data(X_test, y_test)
-        y_test = y_test[self.autoencoder_model.input_size-1:]
-        X_test = self.autoencoder_model.window_data(X_test, self.autoencoder_model.input_size)
-        predicted_values = self.autoencoder_model.predict(X_test)[1].to('cpu').detach().numpy().flatten()
+        iteration_X, iteration_y = self.autoencoder_model.validate_data(X_test, y_test)
+        iteration_y = iteration_y[self.autoencoder_model.input_size-1:]
+        iteration_X = self.autoencoder_model.window_data(iteration_X, self.autoencoder_model.input_size)
+        predicted_values = self.autoencoder_model.predict(iteration_X)[1]
         if self.verbose: print("Predicted values")
-        mse = mean_squared_error(predicted_values, y_test)
-        return mse
+        mape = mean_absolute_percentage_error(predicted_values, iteration_y)
+        return mape
       except Exception as e:
         print(f"Error with parameters {input_size}, {hidden_size}, {num_layers}, {dropout}, {learning_rate}, {epochs}, {batch_size}, {test_size}: {e}")
         return float('inf')
     if self.verbose: print("Warning: This function is experimental, and may throw errors in the optimization process. Use at your own risk.")
     study = optuna.create_study(direction='minimize')
     study.optimize(objective, n_trials=optimization_trials)
     if self.verbose: print("Optimization complete")
```

### Comparing `stockdatamanager-1.1/stockdatamanager/utils.py` & `stockdatamanager-1.1.1/stockdatamanager/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-#%%
+"""
+This utility module provides foundational classes and methods for financial time series analysis and prediction within the OptionPricing class. 
+It encompasses a range of statistical models and machine learning techniques to assist in tasks such as risk-free rate approximation and volatility estimation.
+
+Components:
+- _SMA: Implements a Simple Moving Average model for short-term forecasting based on a sliding window approach.
+- _EMA: Utilizes an Exponential Moving Average for weighted forecasting that prioritizes more recent observations.
+- _SARIMAX_model: An advanced model for time series forecasting that includes seasonal adjustments and exogenous variables. This class also supports hyperparameter optimization using Optuna.
+- _AutoEncoder: A neural network based on PyTorch that learns efficient representations for time series data and can be applied to volatility estimation.
+"""
 import pandas as pd
 from statsmodels.tsa.statespace.sarimax import SARIMAX
 import numpy as np
 import optuna
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import roc_auc_score
 import torch
```

### Comparing `stockdatamanager-1.1/stockdatamanager.egg-info/PKG-INFO` & `stockdatamanager-1.1.1/stockdatamanager.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdatamanager
-Version: 1.1
+Version: 1.1.1
 Summary: A comprehensive library for financial analysis
 Home-page: https://github.com/GiorgioMB/stockdatafetcher/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,22 +20,20 @@
 Requires-Dist: scikit-learn>=1.4.1.post1
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: arch>=4.19
 Requires-Dist: optuna>=2.10.0
 Requires-Dist: torch>=2.2.1
 
 # StockDataManager
-This Python library offers a combination of technical analysis tools and fundamental data retrieval functionalities, designed to support investors, researchers, and enthusiasts in the financial markets. 
-
-This Python library provides a comprehensive suite of tools for both technical and fundamental analysis, along with more advanced options analysis features. Utilizing the yfinance library, it provides easy access to historical stock data, financial statements, and key financial metrics from Yahoo Finance, alongside a suite of technical indicators for market analysis as well as options analysis tools.
+This Python library offers a comprehensive suite of tools for technical and fundamental analysis, along with options analysis capabilities. Utilizing the yfinance library, it facilitates access to historical stock data, financial statements, and key financial metrics from Yahoo Finance. It includes over 30 technical indicators and options analysis tools.
 
 ## Features
-- **Technical Analysis (`IndicatorCalculator` Class)**: Over 30 technical indicators, including Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, and more, to dissect stock market trends and volatility.
-- **Fundamental Analysis (`Fetcher` Class)**: Fetch historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio) for fundamental analysis.
-- **Options Analysis** (`Greeks` and `OptionPricing` Classes): Calculate options greeks and simulate option prices using various models. Supports both European and American options.
+- **Technical Analysis (`IndicatorCalculator` Class)**: Offers over 30 technical indicators like Moving Averages, MACD, Bollinger Bands, RSI, Ichimoku Cloud, etc., for analyzing market trends and volatility.
+- **Fundamental Analysis (`Fetcher` Class)**: Retrieve historical stock data, income statements, balance sheets, cash flows, and key financial ratios (e.g., P/E, ROE, current ratio).
+- **Options Analysis (`Greeks` and `OptionPricing` Classes)**: tools to calculate options greeks and simulate option prices using various models, with enhanced methods to estimate risk-free rates and volatility.
 
 ## Installation
 
 ```bash
 pip install stockdatamanager
 ```
 ## Quick Start
```

### Comparing `stockdatamanager-1.1/tests/test.py` & `stockdatamanager-1.1.1/tests/test.py`

 * *Files identical despite different names*

