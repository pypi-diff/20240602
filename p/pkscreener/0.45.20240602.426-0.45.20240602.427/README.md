# Comparing `tmp/pkscreener-0.45.20240602.426.tar.gz` & `tmp/pkscreener-0.45.20240602.427.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240602.426.tar", last modified: Sun Jun  2 08:28:22 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240602.427.tar", last modified: Sun Jun  2 14:25:46 2024, max compression
```

## Comparing `pkscreener-0.45.20240602.426.tar` & `pkscreener-0.45.20240602.427.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:28:22.011302 pkscreener-0.45.20240602.426/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-02 08:26:21.000000 pkscreener-0.45.20240602.426/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 08:26:21.000000 pkscreener-0.45.20240602.426/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 08:28:22.011302 pkscreener-0.45.20240602.426/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-06-02 08:26:21.000000 pkscreener-0.45.20240602.426/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:28:22.003302 pkscreener-0.45.20240602.426/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:28:22.011302 pkscreener-0.45.20240602.426/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    35718 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    47369 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   164179 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    56446 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 08:28:15.000000 pkscreener-0.45.20240602.426/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   147055 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    60748 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    34702 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:28:22.007302 pkscreener-0.45.20240602.426/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 08:28:21.000000 pkscreener-0.45.20240602.426/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-02 08:28:21.000000 pkscreener-0.45.20240602.426/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 08:28:21.000000 pkscreener-0.45.20240602.426/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-02 08:28:21.000000 pkscreener-0.45.20240602.426/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 08:28:21.000000 pkscreener-0.45.20240602.426/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 08:28:21.000000 pkscreener-0.45.20240602.426/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 08:28:21.000000 pkscreener-0.45.20240602.426/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 08:28:22.011302 pkscreener-0.45.20240602.426/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-02 08:26:22.000000 pkscreener-0.45.20240602.426/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:25:46.355856 pkscreener-0.45.20240602.427/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 14:25:46.355856 pkscreener-0.45.20240602.427/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:25:46.351856 pkscreener-0.45.20240602.427/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:25:46.355856 pkscreener-0.45.20240602.427/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35718 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47369 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   164179 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56446 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 14:25:39.000000 pkscreener-0.45.20240602.427/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   147406 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    61055 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-06-02 14:23:53.000000 pkscreener-0.45.20240602.427/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:25:46.351856 pkscreener-0.45.20240602.427/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-06-02 14:25:46.000000 pkscreener-0.45.20240602.427/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-02 14:25:46.000000 pkscreener-0.45.20240602.427/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:25:46.000000 pkscreener-0.45.20240602.427/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-02 14:25:46.000000 pkscreener-0.45.20240602.427/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:25:46.000000 pkscreener-0.45.20240602.427/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-02 14:25:46.000000 pkscreener-0.45.20240602.427/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 14:25:46.000000 pkscreener-0.45.20240602.427/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 14:25:46.355856 pkscreener-0.45.20240602.427/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-06-02 14:23:54.000000 pkscreener-0.45.20240602.427/setup.py
```

### Comparing `pkscreener-0.45.20240602.426/LICENSE` & `pkscreener-0.45.20240602.427/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/LICENSE-Others` & `pkscreener-0.45.20240602.427/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/PKG-INFO` & `pkscreener-0.45.20240602.427/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240602.426
+Version: 0.45.20240602.427
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.426.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.427.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.426/README.md` & `pkscreener-0.45.20240602.427/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.426/pkscreener/__init__.py` & `pkscreener-0.45.20240602.427/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/OtaUpdater.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,30 +134,28 @@
         txt = txt.split("## Older Releases")[0]
         txt = txt.replace("* ", "- ").replace("`", "").strip()
         return txt + "\n"
 
     def get_latest_release_info():
         resp = OTAUpdater.fetcher.fetchURL(
             "https://api.github.com/repos/pkjmesra/PKScreener/releases/latest"
-        )
+        )  
+
         if "Windows" in platform.system():
-            OTAUpdater.checkForUpdate.url = resp.json()["assets"][1][
-                "browser_download_url"
-            ]
-            size = int(resp.json()["assets"][1]["size"] / (1024 * 1024))
+            exe_name = "pkscreenercli.exe"
         elif "Darwin" in platform.system():
-            OTAUpdater.checkForUpdate.url = resp.json()["assets"][2][
-                "browser_download_url"
-            ]
-            size = int(resp.json()["assets"][2]["size"] / (1024 * 1024))
+            exe_name = "pkscreenercli.run"
         else:
-            OTAUpdater.checkForUpdate.url = resp.json()["assets"][0][
-                "browser_download_url"
-            ]
-            size = int(resp.json()["assets"][0]["size"] / (1024 * 1024))
+            exe_name = "pkscreenercli.bin"
+        for asset in resp.json()["assets"]:
+            url = asset["browser_download_url"]
+            if url.endswith(exe_name):
+                OTAUpdater.checkForUpdate.url = url
+                size = int(asset["size"] / (1024 * 1024))
+                break
         return resp, size
 
     # Check for update and download if available
     def checkForUpdate(VERSION=VERSION, skipDownload=False):
         OTAUpdater.checkForUpdate.url = None
         resp = None
         updateType = "minor"
```

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/classes/keys.py` & `pkscreener-0.45.20240602.427/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/courbd.ttf` & `pkscreener-0.45.20240602.427/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/globals.py` & `pkscreener-0.45.20240602.427/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -2464,50 +2464,14 @@
 #     df1 =  pd.DataFrame(noColor, index=x.index, columns=x.columns)
 #     #modify values of df1 column by boolean mask
 #     df1.loc[mask_green_bid, 'BidQty'] = green
 #     df1.loc[mask_red_bid, 'AskQty'] = red
 #     df1.loc[mask_green_vwap, 'VWAP'] = green
 #     return df1
 
-def processResultsCallback(resultItem, processedCount,result_df, *otherArgs):
-    global userPassedArgs
-    (menuOption, backtestPeriod, result, lstscreen, lstsave, progressbar, testing,max_allowed) = otherArgs
-    numStocks = processedCount
-    result = resultItem
-    backtest_df = processResults(menuOption, backtestPeriod, result, lstscreen, lstsave, result_df)
-    progressbar()
-    progressbar.text(
-        colorText.BOLD
-        + colorText.GREEN
-        + f"{'Remaining' if userPassedArgs.download else ('Found' if menuOption in ['X'] else 'Analysed')} {len(lstscreen) if not userPassedArgs.download else processedCount} {'Stocks' if menuOption in ['X'] else 'Records'}"
-        + colorText.END
-    )
-    if result is not None:
-        if not userPassedArgs.monitor and len(lstscreen) > 0 and userPassedArgs is not None and userPassedArgs.options.split(":")[2] in ["29"]:
-            scr_df = pd.DataFrame(lstscreen)
-            existingColumns = ["Stock","%Chng","LTP","Volume"]
-            newColumns = ["BidQty","AskQty","LwrCP","UprCP","VWAP","DayVola","Del(%)"]
-            existingColumns.extend(newColumns)
-            scr_df = scr_df[existingColumns]
-            scr_df.sort_values(by=["Volume","BidQty"], ascending=False, inplace=True)
-            tabulated_results = colorText.miniTabulator().tb.tabulate(
-                    scr_df,
-                    headers="keys",
-                    showindex=False,
-                    tablefmt=colorText.No_Pad_GridFormat,
-                    maxcolwidths=Utility.tools.getMaxColumnWidths(scr_df)
-                )
-            tableLength = 2*len(lstscreen)+5
-            OutputControls().printOutput('\n'+tabulated_results)
-            # Move the cursor up, back to the top because we want the progress bar to keep showing at the top
-            sys.stdout.write(f"\x1b[{tableLength}A")  # cursor up one line
-    if keyboardInterruptEventFired:
-        return False, backtest_df
-    return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
-
 def runScanners(
     menuOption,
     items,
     tasks_queue,
     results_queue,
     numStocks,
     backtestPeriod,
@@ -2547,15 +2511,50 @@
         bar, spinner = Utility.tools.getProgressbarStyle()
         with alive_bar(numStocks, bar=bar, spinner=spinner) as progressbar:
             lstscreen = []
             lstsave = []
             result = None
             backtest_df = None
             start_time = time.time()
-            otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave, progressbar, testing,max_allowed)
+            def processResultsCallback(resultItem, processedCount,result_df, *otherArgs):
+                global userPassedArgs
+                (menuOption, backtestPeriod, result, lstscreen, lstsave) = otherArgs
+                numStocks = processedCount
+                result = resultItem
+                backtest_df = processResults(menuOption, backtestPeriod, result, lstscreen, lstsave, result_df)
+                progressbar()
+                progressbar.text(
+                    colorText.BOLD
+                    + colorText.GREEN
+                    + f"{'Remaining' if userPassedArgs.download else ('Found' if menuOption in ['X'] else 'Analysed')} {len(lstscreen) if not userPassedArgs.download else processedCount} {'Stocks' if menuOption in ['X'] else 'Records'}"
+                    + colorText.END
+                )
+                if result is not None:
+                    if not userPassedArgs.monitor and len(lstscreen) > 0 and userPassedArgs is not None and userPassedArgs.options.split(":")[2] in ["29"]:
+                        scr_df = pd.DataFrame(lstscreen)
+                        existingColumns = ["Stock","%Chng","LTP","Volume"]
+                        newColumns = ["BidQty","AskQty","LwrCP","UprCP","VWAP","DayVola","Del(%)"]
+                        existingColumns.extend(newColumns)
+                        scr_df = scr_df[existingColumns]
+                        scr_df.sort_values(by=["Volume","BidQty"], ascending=False, inplace=True)
+                        tabulated_results = colorText.miniTabulator().tb.tabulate(
+                                scr_df,
+                                headers="keys",
+                                showindex=False,
+                                tablefmt=colorText.No_Pad_GridFormat,
+                                maxcolwidths=Utility.tools.getMaxColumnWidths(scr_df)
+                            )
+                        tableLength = 2*len(lstscreen)+5
+                        OutputControls().printOutput('\n'+tabulated_results)
+                        # Move the cursor up, back to the top because we want the progress bar to keep showing at the top
+                        sys.stdout.write(f"\x1b[{tableLength}A")  # cursor up one line
+                if keyboardInterruptEventFired:
+                    return False, backtest_df
+                return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
+            otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave)
             backtest_df, result =PKScanRunner.runScan(userPassedArgs,testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
 
         OutputControls().printOutput(f"\x1b[{3 if OutputControls().enableMultipleLineOutput else 1}A")
         if len(lstscreen) == 0 and userPassedArgs is not None and userPassedArgs.monitor is None:
             OutputControls().printOutput("\x1b[2K") # Delete the progress bar line
         elapsed_time = time.time() - start_time
         if menuOption in ["X", "G", "C"]:
```

### Comparing `pkscreener-0.45.20240602.426/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240602.427/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240602.427/pkscreener/pkscreenerbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 except ImportError:
     import _thread as thread
 
 import traceback
 from datetime import datetime
 from time import sleep
 from telegram import __version__ as TG_VER
-from telegram.constants import ParseMode
+# from telegram.constants import ParseMode
 
 start_time = datetime.now()
 MINUTES_2_IN_SECONDS = 120
 OWNER_USER = "Itsonlypk"
 
 from PKDevTools.classes.Telegram import get_secrets
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
@@ -68,48 +68,58 @@
 from pkscreener.globals import showSendConfigInfo, showSendHelpInfo
 import pkscreener.classes.ConfigManager as ConfigManager
 
 monitor_proc = None
 configManager = ConfigManager.tools()
 bot_available=True
 
-try:
-    from telegram import __version_info__
-except ImportError:
-    __version_info__ = (0, 0, 0, 0, 0)  # type: ignore[assignment]
-
-if __version_info__ < (20, 0, 0, "alpha", 1):
-    raise RuntimeError(
-        f"This example is not compatible with your current PTB version {TG_VER}. To view the "
-        f"{TG_VER} version of this example, "
-        f"visit https://docs.python-telegram-bot.org/en/v{TG_VER}/examples.html"
-    )
+# try:
+#     from telegram import __version_info__
+# except ImportError:
+#     __version_info__ = (0, 0, 0, 0, 0)  # type: ignore[assignment]
+
+# if __version_info__ < (20, 0, 0, "alpha", 1):
+#     raise RuntimeError(
+#         f"This example is not compatible with your current PTB version {TG_VER}. To view the "
+#         f"{TG_VER} version of this example, "
+#         f"visit https://docs.python-telegram-bot.org/en/v{TG_VER}/examples.html"
+#     )
 from telegram import InlineKeyboardButton, InlineKeyboardMarkup, Update
 from telegram.ext import (
-    Application,
+    Updater,
     CallbackQueryHandler,
     CommandHandler,
     ContextTypes,
     ConversationHandler,
     MessageHandler,
-    filters,
+    Filters,
     CallbackContext
 )
 
 # Enable logging
 logging.basicConfig(
     format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=logging.INFO
 )
 # set higher logging level for httpx to avoid all GET and POST requests being logged
 logging.getLogger("httpx").setLevel(logging.WARNING)
 
 logger = logging.getLogger(__name__)
 
+# # State definitions for top level conversation
+# SELECTING_ACTION, ADDING_MEMBER, ADDING_SELF, DESCRIBING_SELF = map(chr, range(4))
+# # State definitions for second level conversation
+# SELECTING_LEVEL, SELECTING_GENDER = map(chr, range(4, 6))
+# # State definitions for descriptions conversation
+# SELECTING_FEATURE, TYPING = map(chr, range(6, 8))
+# # Meta states
+# STOPPING, SHOWING = map(chr, range(8, 10))
+# # Shortcut for ConversationHandler.END
+# END = ConversationHandler.END
 # Stages
-START_ROUTES, END_ROUTES = range(2)
+START_ROUTES, END_ROUTES = map(chr, range(2)) #range(2)
 # Callback data
 ONE, TWO, THREE, FOUR = range(4)
 
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
@@ -147,15 +157,15 @@
                 int_timer.start()
             elif now >= marketStartTime:
                 launchIntradayMonitor()
     except:
         launchIntradayMonitor()
         pass
 
-async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None, monitorIndex=0,chosenBotMenuOption="") -> int:
+def start(update: Update, context: CallbackContext, updatedResults=None, monitorIndex=0,chosenBotMenuOption="") -> str:
     """Send message on `/start`."""
     global bot_available
     updateCarrier = None
     if update is None:
         return
     else:
         if update.callback_query is not None:
@@ -213,26 +223,26 @@
             pass
         menuText = f"{menuText}\n\nClick /start if you want to restart the session."
     else:
         chosenBotMenuOption = f"{chosenBotMenuOption}\nInt. Monitor. MonitorIndex:{monitorIndex}\n{updatedResults}"
         menuText = updatedResults
     # Send message with text and appended InlineKeyboard
     if update.callback_query is not None:
-        await sendUpdatedMenu(
+        sendUpdatedMenu(
             menuText=menuText, update=update, context=context, reply_markup=reply_markup, replaceWhiteSpaces=(updatedResults is None)
         )
     elif update.message is not None:
-        await update.message.reply_text(
+        update.message.reply_text(
             menuText,
             reply_markup=reply_markup,
         )
-    await context.bot.send_message(
+    context.bot.send_message(
         chat_id=int(f"-{Channel_Id}"),
         text=f"Name: {user.first_name}, Username:@{user.username} with ID: {str(user.id)} started using the bot!\n{chosenBotMenuOption}",
-        parse_mode=ParseMode.HTML,
+        parse_mode="HTML",
     )
     # Tell ConversationHandler that we're in state `FIRST` now
     return START_ROUTES
 
 def removeMonitorFile():
     from PKDevTools.classes import Archiver
     configManager.getConfig(ConfigManager.parser)
@@ -288,15 +298,15 @@
     except Exception as e:
         result_outputs = "Hmm...It looks like you caught us taking a break! Try again later :-)"
         logger.info(f"{launcher} -a Y -m 'X' -p --telegram could not be launched")
         logger.info(e)
         pass
     return result_outputs, filePath
 
-async def XDevModeHandler(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
+def XDevModeHandler(update: Update, context: CallbackContext) -> str:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI").replace("CDV","DV")
     if data[0:2] not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     if data.startswith("DV"):
         # Dev Mode
@@ -316,52 +326,52 @@
             if monitor_proc is not None:
                 try:
                     monitor_proc.kill()
                 except:
                     pass
             
             launchIntradayMonitor()
-            await start(update, context,chosenBotMenuOption=chosenBotMenuOption)
+            start(update, context,chosenBotMenuOption=chosenBotMenuOption)
         elif devModeIndex == 1: # Restart the bot service
             resp = run_workflow(None, None,None, workflowType="R")
-            await start(update, context,chosenBotMenuOption=f"{resp.status_code}: {resp.text}")
+            start(update, context,chosenBotMenuOption=f"{resp.status_code}: {resp.text}")
     return START_ROUTES
 
-async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
+def XScanners(update: Update, context: CallbackContext) -> str:
     """Show new choice of buttons"""
     query = update.callback_query
     if query is None:
-        await start(update, context)
+        start(update, context)
         return START_ROUTES
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI")
     if data[0:2] not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     global bot_available
     if not bot_available:
-        await start(update, context)
+        start(update, context)
         return START_ROUTES
     if data.startswith("MI"):
         monitorIndex = int(data.split("_")[1])
         result_outputs, filePath = launchIntradayMonitor()
         filePath = f"{filePath}_{monitorIndex}.txt"
         monitorIndex += 1
         if monitorIndex >= configManager.maxDashboardWidgetsPerRow*configManager.maxNumResultRowsInMonitor:
             monitorIndex = 0
         try:
             if os.path.exists(filePath):
                 f = open(filePath, "r")
                 result_outputs = f.read()
                 f.close()
-            await start(update, context, updatedResults=result_outputs,monitorIndex=monitorIndex)
+            start(update, context, updatedResults=result_outputs,monitorIndex=monitorIndex)
             return START_ROUTES
         except Exception as e:
             result_outputs = "Hmm...It looks like you caught us taking a break! Try again later :-)\nCycleTime shows how much it's taking us to download latest data and then perform each cycle of analysis for all configured scanners. We may be downloading the latest data right now."
             logger.info(e)
             logger.info(f"Could not read {filePath}")
-            await start(update, context, updatedResults=result_outputs,monitorIndex=monitorIndex)
+            start(update, context, updatedResults=result_outputs,monitorIndex=monitorIndex)
             return START_ROUTES
 
     midSkip = "1" if data == "X" else "N"
     skipMenus = [midSkip]
     skipMenus.extend(INDEX_SKIP_MENUS)
     menuText = (
         m1.renderForMenu(
@@ -379,51 +389,51 @@
     mns = m1.renderForMenu(
         m0.find(data),
         skip=skipMenus,
         asList=True,
     )
     mns.append(menu().create("H", "Home", 2))
     inlineMenus = []
-    await query.answer()
+    query.answer()
     for mnu in mns:
         inlineMenus.append(
             InlineKeyboardButton(
                 mnu.menuKey, callback_data=str(f"{query.data}_{mnu.menuKey}")
             )
         )
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
     if query.message.text == menuText:
         menuText = f"{PKDateUtilities.currentDateTime()}:\n{menuText}"
     menuText = f"{menuText}\n\nClick /start if you want to restart the session."
-    await query.edit_message_text(text=menuText, reply_markup=reply_markup)
+    query.edit_message_text(text=menuText, reply_markup=reply_markup)
     return START_ROUTES
 
 
-async def Level2(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
+def Level2(update: Update, context: CallbackContext) -> str:
     """Show new choice of buttons"""
     inlineMenus = []
     menuText = "Hmm...It looks like you caught us taking a break! Try again later :-)"
     mns = []
     query = update.callback_query
-    await query.answer()
+    query.answer()
     preSelection = (
         query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
     )
     selection = preSelection.split("_")
     preSelection = f"{selection[0]}_{selection[1]}"
     if (selection[0].upper() not in TOP_LEVEL_SCANNER_MENUS):
-        await start(update, context)
+        start(update, context)
         return START_ROUTES
     global bot_available
     if not bot_available:
-        await start(update, context)
+        start(update, context)
         return START_ROUTES
     if selection[len(selection)-1].upper() == "H":
-        await start(update, context)
+        start(update, context)
         return START_ROUTES
     if len(selection) == 2 or (len(selection) == 3 and selection[2] == "P"):
         if str(selection[1]).isnumeric():
             # It's only level 2
             menuText = m2.renderForMenu(
                 m1.find(selection[1]),
                 skip=SCANNER_SKIP_MENUS_1_TO_6,
@@ -549,33 +559,33 @@
             f"{selection[0]} > {selection[1]} > {selection[2]} > {selection[3]}"
         )
         expectedTime = f"{'10 to 15' if '> 15' in optionChoices else '1 to 2'}"
         menuText = f"Thank you for choosing {optionChoices}. You will receive the notification/results in about {expectedTime} minutes. It generally takes 1-2 minutes for NSE (2000+) stocks and 10-15 minutes for NASDAQ (7300+).\n\nPKScreener is free and will always remain so for everyone. Consider donating to help cover the basic server costs:\n\nUPI (India): 8007162973@APL \n\nor\nhttps://github.com/sponsors/pkjmesra?frequency=one-time&sponsor=pkjmesra"
 
         reply_markup = default_markup(inlineMenus)
         options = ":".join(selection)
-        await launchScreener(
+        launchScreener(
             options=options,
             user=query.from_user,
             context=context,
             optionChoices=optionChoices,
             update=update,
         )
     try:
         if optionChoices != "":
-            await context.bot.send_message(
+            context.bot.send_message(
                 chat_id=int(f"-{Channel_Id}"),
                 text=f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> submitted scan request <b>{optionChoices}</b> to the bot!",
-                parse_mode=ParseMode.HTML,
+                parse_mode="HTML",
             )
     except Exception:# pragma: no cover
-        await start(update, context)
+        start(update, context)
     menuText =  menuText.replace("\n     ","\n").replace("\n    ","\n").replace(colorText.FAIL,"").replace(colorText.END,"")
     if not str(optionChoices.upper()).startswith("B"):
-        await sendUpdatedMenu(
+        sendUpdatedMenu(
             menuText=menuText, update=update, context=context, reply_markup=reply_markup
         )
     return START_ROUTES
 
 def default_markup(inlineMenus):
     mns = m0.renderForMenu(asList=True)
     for mnu in mns:
@@ -587,51 +597,51 @@
                     )
                 )
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
     return reply_markup
 
 
-async def sendUpdatedMenu(menuText, update: Update, context, reply_markup, replaceWhiteSpaces=True):
+def sendUpdatedMenu(menuText, update: Update, context, reply_markup, replaceWhiteSpaces=True):
     try:
         menuText.replace("     ", "").replace("    ", "").replace("\t", "").replace(colorText.FAIL,"").replace(colorText.END,"") if replaceWhiteSpaces else menuText
         menuText = f"{menuText}\n\nClick /start if you want to restart the session." if "/start" not in menuText else menuText
         if update.callback_query.message.text == menuText:
             menuText = f"{PKDateUtilities.currentDateTime()}:\n{menuText}"
-        await update.callback_query.edit_message_text(
+        update.callback_query.edit_message_text(
             text=menuText,
             parse_mode="HTML",
             reply_markup=reply_markup,
         )
     except Exception as e:# pragma: no cover
         logger.log(e)
-        await start(update, context)
+        start(update, context)
 
 
-async def launchScreener(options, user, context, optionChoices, update):
+def launchScreener(options, user, context, optionChoices, update):
     try:
         if str(optionChoices.upper()).startswith("B"):
             optionChoices = optionChoices.replace(" ", "").replace(">", "_").replace(":","_").replace("_D","")
             while optionChoices.endswith("_"):
                 optionChoices = optionChoices[:-1]
             if str(optionChoices).split("_")[2] == "6" and str(optionChoices).split("_")[3] == "7":
                 optionChoices = f"{optionChoices}_3" # Lorenzian Any/All
             responseText = f"Thank you for choosing {optionChoices}!\n\nHere are the results:\n\nInsights: https://pkjmesra.github.io/PKScreener/Backtest-Reports/PKScreener_{optionChoices}_Insights_DateSorted.html"
             responseText = f"{responseText}\n\nSummary: https://pkjmesra.github.io/PKScreener/Backtest-Reports/PKScreener_{optionChoices}_Summary_StockSorted.html"
             responseText = f"{responseText}\n\nStock-wise: https://pkjmesra.github.io/PKScreener/Backtest-Reports/PKScreener_{optionChoices}_backtest_result_StockSorted.html"
             responseText = f"{responseText}\n\nOther Reports: https://pkjmesra.github.io/PKScreener/BacktestReports.html"
             if update is not None and update.message is not None:
-                await update.message.reply_text(responseText)
+                update.message.reply_text(responseText)
             else:
                 responseText = f"{responseText}\n\nClick /start if you want to restart the session."
-                await update.callback_query.edit_message_text(
+                update.callback_query.edit_message_text(
                     text=responseText,
                     reply_markup=default_markup([]),
                 )
-            await shareUpdateWithChannel(
+            shareUpdateWithChannel(
                 update=update, context=context, optionChoices=optionChoices
             )
             # run_workflow(optionChoices, str(user.id), str(options.upper()))
         elif str(optionChoices.upper()).startswith("X") or str(optionChoices.upper()).startswith("P"):
             optionChoices = optionChoices.replace(" ", "").replace(">", "_")
             while optionChoices.endswith("_"):
                 optionChoices = optionChoices[:-1]
@@ -659,59 +669,59 @@
             #         str(user.id),
             #     ]
             # )
     except Exception as e:
         import traceback
         traceback.print_exc()
         print(e)
-        await start(update, context)
+        start(update, context)
 
 
-async def BBacktests(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
+def BBacktests(update: Update, context: CallbackContext) -> str:
     """Show new choice of buttons"""
     query = update.callback_query
-    await query.answer()
+    query.answer()
     keyboard = [
         [
             InlineKeyboardButton("Try Scanners", callback_data=str("CX")),
             # InlineKeyboardButton("Growth of 10k", callback_data=str("CG")),
         ]
     ]
     reply_markup = InlineKeyboardMarkup(keyboard)
     responseText = "Backtesting NOT implemented yet in this Bot!\n\n\nYou can use backtesting by downloading the software from https://github.com/pkjmesra/PKScreener/"
     responseText = f"{responseText}\n\nClick /start if you want to restart the session."
-    await query.edit_message_text(
+    query.edit_message_text(
         text=responseText,
         reply_markup=reply_markup,
     )
     return START_ROUTES
 
 
-async def end(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
+def end(update: Update, context: CallbackContext) -> str:
     """Returns `ConversationHandler.END`, which tells the
     ConversationHandler that the conversation is over.
     """
     query = update.callback_query
-    await query.answer()
+    query.answer()
     responseText = "See https://github.com/pkjmesra/PKScreener/ for more details or join https://t.me/PKScreener. \n\n\nSee you next time!"
     responseText = f"{responseText}\n\nClick /start if you want to restart the session."
-    await query.edit_message_text(
+    query.edit_message_text(
         text=responseText
     )
     return ConversationHandler.END
 
 
 # This can be your own ID, or one for a developer group/channel.
 # You can use the /start command of this bot to see your chat id.
 chat_idADMIN = 123456789
 Channel_Id = 12345678
 GROUP_CHAT_ID = 1001907892864
 
 
-async def error_handler(update: object, context: ContextTypes.DEFAULT_TYPE) -> None:
+def error_handler(update: object, context: CallbackContext) -> None:
     """Log the error and send a telegram message to notify the developer."""
     # Log the error before we do anything else, so we can see it even if something breaks.
     logger.error("Exception while handling an update:", exc_info=context.error)
 
     # traceback.format_exception returns the usual python message about an exception, but as a
     # list of strings rather than a single string, so we have to join them together.
     tb_list = traceback.format_exception(
@@ -755,54 +765,54 @@
         f"<pre>context.user_data = {html.escape(str(context.user_data))}</pre>\n\n"
         f"<pre>{html.escape(tb_string)}</pre>"
     )
 
     try:
         # Finally, send the message
         if "telegram.error.Conflict" not in message:
-            await context.bot.send_message(
-                chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
+            context.bot.send_message(
+                chat_id=int(f"-{Channel_Id}"), text=message, parse_mode="HTML"
             )
     except Exception:# pragma: no cover
         try:
             if "telegram.error.Conflict" not in tb_string:
-                await context.bot.send_message(
+                context.bot.send_message(
                     chat_id=int(f"-{Channel_Id}"),
                     text=tb_string,
-                    parse_mode=ParseMode.HTML,
+                    parse_mode="HTML",
                 )
         except Exception:# pragma: no cover
             print(tb_string)
 
 
-async def command_handler(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+def command_handler(update: Update, context: CallbackContext) -> None:
     if _shouldAvoidResponse(update):
         return
     msg = update.effective_message
     m = re.match("\s*/([0-9a-zA-Z_-]+)\s*(.*)", msg.text)
     cmd = m.group(1).lower()
     args = [arg for arg in re.split("\s+", m.group(2)) if len(arg)]
     if cmd.startswith("cx_") or cmd.startswith("cb_") or cmd.startswith("cg_"):
-        await Level2(update=update, context=context)
+        Level2(update=update, context=context)
         return START_ROUTES
     if cmd.startswith("cx") or cmd.startswith("cb") or cmd.startswith("cg"):
-        await XScanners(update=update, context=context)
+        XScanners(update=update, context=context)
         return START_ROUTES
     if cmd.startswith("cz"):
-        await end(update=update, context=context)
+        end(update=update, context=context)
         return END_ROUTES
 
     if cmd == "start":
-        await start(update=update, context=context)
+        start(update=update, context=context)
         return START_ROUTES
     if cmd == "help":
-        await help_command(update=update, context=context)
+        help_command(update=update, context=context)
         return START_ROUTES
     if cmd.upper() in TOP_LEVEL_SCANNER_MENUS:
-        await shareUpdateWithChannel(update=update, context=context)
+        shareUpdateWithChannel(update=update, context=context)
         m0.renderForMenu(
             selectedMenu=None,
             skip=TOP_LEVEL_SCANNER_SKIP_MENUS[:len(TOP_LEVEL_SCANNER_SKIP_MENUS)-1],
             asList=True,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         selectedMenu = m0.find(cmd.upper())
@@ -819,52 +829,52 @@
             cmdText = (
                 f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
             )
         if cmd in ["x"]:
             cmdText = f"{cmdText}\n\nFor option 0 <Screen stocks by the stock name>, please type in the command in the following format\n/X_0 SBIN\n or \n/X_0_0 SBIN\nand hit send where SBIN is the NSE stock code.For multiple stocks, you can type in \n/X_0 SBIN,ICICIBANK,OtherStocks\nYou can put in any number of stocks separated by space or comma(,)."
         """Send a message when the command /help is issued."""
         cmdText = f"{cmdText}\n\nClick /start if you want to restart the session."
-        await update.message.reply_text(f"Choose an option:\n{cmdText}")
+        update.message.reply_text(f"Choose an option:\n{cmdText}")
         return START_ROUTES
 
     if update.message is None:
-        await help_command(update=update, context=context)
+        help_command(update=update, context=context)
         return START_ROUTES
     if "x_0" in cmd or "x_0_0" in cmd or "b_0" in cmd or "g_0" in cmd:
-        await shareUpdateWithChannel(update=update, context=context)
+        shareUpdateWithChannel(update=update, context=context)
         shouldScan = False
         if len(args) > 0:
             shouldScan = True
             selection = [
                 cmd.split("_")[0].upper(),
                 "0",
                 "0",
                 f"{','.join(args)}".replace(" ", ""),
             ]
         if shouldScan:
             options = ":".join(selection)
-            await launchScreener(
+            launchScreener(
                 options=options,
                 user=update.message.from_user,
                 context=context,
                 optionChoices=cmd.upper(),
                 update=update,
             )
-            await sendRequestSubmitted(cmd.upper(), update=update, context=context)
+            sendRequestSubmitted(cmd.upper(), update=update, context=context)
             return START_ROUTES
         else:
             if cmd in ["x"]:
                 cmdText = "For option 0 <Screen stocks by the stock name>, please type in the command in the following format\n/X_0 SBIN or /X_0_0 SBIN and hit send where SBIN is the NSE stock code.For multiple stocks, you can type in /X_0 SBIN,ICICIBANK,OtherStocks . You can put in any number of stocks separated by space or comma(,)."
             """Send a message when the command /help is issued."""
             cmdText = f"{cmdText}\n\nClick /start if you want to restart the session."
-            await update.message.reply_text(f"Choose an option:\n{cmdText}")
+            update.message.reply_text(f"Choose an option:\n{cmdText}")
             return START_ROUTES
 
     if "p_" in cmd:
-        await shareUpdateWithChannel(update=update, context=context)
+        shareUpdateWithChannel(update=update, context=context)
         selection = cmd.split("_")
         if len(selection) == 2:
             m0.renderForMenu(
                 selectedMenu=None,
                 skip=TOP_LEVEL_SCANNER_SKIP_MENUS[:len(TOP_LEVEL_SCANNER_SKIP_MENUS)-1],
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
@@ -885,30 +895,30 @@
             )
             cmdText = ""
             for cmd in cmds:
                 cmdText = (
                     f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
                 )
             cmdText = f"{cmdText}\n\nClick /start if you want to restart the session."
-            await update.message.reply_text(f"Choose an option:\n{cmdText}")
+            update.message.reply_text(f"Choose an option:\n{cmdText}")
             return START_ROUTES
         elif len(selection) == 3:
             options = ":".join(selection)
-            await launchScreener(
+            launchScreener(
                 options=options,
                 user=update.message.from_user,
                 context=context,
                 optionChoices=cmd.upper(),
                 update=update,
             )
-            await sendRequestSubmitted(cmd.upper(), update=update, context=context)
+            sendRequestSubmitted(cmd.upper(), update=update, context=context)
             return START_ROUTES
         
     if "x_" in cmd or "b_" in cmd or "g_" in cmd:
-        await shareUpdateWithChannel(update=update, context=context)
+        shareUpdateWithChannel(update=update, context=context)
         selection = cmd.split("_")
         if len(selection) == 2:
             m0.renderForMenu(
                 selectedMenu=None,
                 skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
@@ -923,44 +933,44 @@
                 ),
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             selectedMenu = m1.find(selection[1].upper())
             if "x_" in cmd and selectedMenu.menuKey == "N":  # Nifty prediction
                 options = ":".join(selection)
-                await launchScreener(
+                launchScreener(
                     options=options,
                     user=update.message.from_user,
                     context=context,
                     optionChoices=cmd.upper(),
                     update=update,
                 )
-                await sendRequestSubmitted(cmd.upper(), update=update, context=context)
+                sendRequestSubmitted(cmd.upper(), update=update, context=context)
                 return START_ROUTES
             elif (
                 "x_" in cmd and selectedMenu.menuKey == "0"
             ):  # a specific stock by name
                 cmdText = "For option 0 <Screen stocks by the stock name>, please type in the command in the following format\n/X_0 SBIN or /X_0_0 SBIN and hit send where SBIN is the NSE stock code.For multiple stocks, you can type in /X_0 SBIN,ICICIBANK,OtherStocks. You can put in any number of stocks separated by space or comma(,)."
                 """Send a message when the command /help is issued."""
                 cmdText = f"{cmdText}\n\nClick /start if you want to restart the session."
-                await update.message.reply_text(f"Choose an option:\n{cmdText}")
+                update.message.reply_text(f"Choose an option:\n{cmdText}")
                 return START_ROUTES
             cmds = m2.renderForMenu(
                 selectedMenu=selectedMenu,
                 skip=UNSUPPORTED_COMMAND_MENUS,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
             )
             cmdText = ""
             for cmd in cmds:
                 cmdText = (
                     f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
                 )
             cmdText = f"{cmdText}\n\nClick /start if you want to restart the session."
-            await update.message.reply_text(f"Choose an option:\n{cmdText}")
+            update.message.reply_text(f"Choose an option:\n{cmdText}")
             return START_ROUTES
         elif len(selection) == 3:
             m0.renderForMenu(
                 selectedMenu=None,
                 skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
                 asList=True,
                 renderStyle=MenuRenderStyle.STANDALONE,
@@ -991,15 +1001,15 @@
                     renderStyle=MenuRenderStyle.STANDALONE,
                     skip=["0"],
                 )
                 cmdText = ""
                 for cmd in cmds:
                     cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
                 cmdText = f"{cmdText}\n\nClick /start if you want to restart the session."
-                await update.message.reply_text(f"Choose an option:\n{cmdText}")
+                update.message.reply_text(f"Choose an option:\n{cmdText}")
                 return START_ROUTES
             else:
                 if selection[2] == "4":  # Last N days
                     selection.extend(["D", ""])
                 elif selection[2] == "5":  # RSI range
                     selection.extend(["D", "D"])
                 elif selection[2] == "8":  # CCI range
@@ -1050,90 +1060,90 @@
                             renderStyle=MenuRenderStyle.STANDALONE,
                             skip=["0"],
                         )
                         cmdText = ""
                         for cmd in cmds:
                             cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
                         cmdText = f"{cmdText}\n\nClick /start if you want to restart the session."
-                        await update.message.reply_text(f"Choose an option:\n{cmdText}")
+                        update.message.reply_text(f"Choose an option:\n{cmdText}")
                         return START_ROUTES
 
             options = ":".join(selection)
-            await launchScreener(
+            launchScreener(
                 options=options,
                 user=update.message.from_user,
                 context=context,
                 optionChoices=cmd.upper(),
                 update=update,
             )
-            await sendRequestSubmitted(cmd.upper(), update=update, context=context)
+            sendRequestSubmitted(cmd.upper(), update=update, context=context)
             return START_ROUTES
     if cmd == "y" or cmd == "h":
-        await shareUpdateWithChannel(update=update, context=context)
+        shareUpdateWithChannel(update=update, context=context)
         if cmd == "y":
             showSendConfigInfo(defaultAnswer='Y',user=str(update.message.from_user.id))
         elif cmd == "h":
             showSendHelpInfo(defaultAnswer='Y',user=str(update.message.from_user.id))
-        # await launchScreener(
+        # launchScreener(
         #     options=f"{cmd.upper()}:",
         #     user=update.message.from_user,
         #     context=context,
         #     optionChoices=cmd.upper(),
         #     update=update,
         # )
-        # await sendRequestSubmitted(cmd.upper(), update=update, context=context)
+        # sendRequestSubmitted(cmd.upper(), update=update, context=context)
         return START_ROUTES
-    await update.message.reply_text(f"{cmd.upper()} : Not implemented yet!")
-    await help_command(update=update, context=context)
+    update.message.reply_text(f"{cmd.upper()} : Not implemented yet!")
+    help_command(update=update, context=context)
 
 
-async def sendRequestSubmitted(optionChoices, update, context):
+def sendRequestSubmitted(optionChoices, update, context):
     menuText = f"Thank you for choosing {optionChoices}. You will receive the notification/results in about 1-2 minutes! \n\nConsider donating to help keep this project going:\nUPI: 8007162973@APL \nor\nhttps://github.com/sponsors/pkjmesra?frequency=one-time&sponsor=pkjmesra"
-    await update.message.reply_text(menuText)
-    await help_command(update=update, context=context)
-    await shareUpdateWithChannel(
+    update.message.reply_text(menuText)
+    help_command(update=update, context=context)
+    shareUpdateWithChannel(
         update=update, context=context, optionChoices=optionChoices
     )
 
 
-async def shareUpdateWithChannel(update, context, optionChoices=""):
+def shareUpdateWithChannel(update, context, optionChoices=""):
     query = update.message or update.callback_query
     message = f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using ({optionChoices}) the bot!"
-    await context.bot.send_message(
-        chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
+    context.bot.send_message(
+        chat_id=int(f"-{Channel_Id}"), text=message, parse_mode="HTML"
     )
 
 
-async def help_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+def help_command(update: Update, context: CallbackContext) -> None:
     if _shouldAvoidResponse(update):
         return
     global bot_available
     if not bot_available:
-        await start(update, context)
+        start(update, context)
         return START_ROUTES
     cmds = m0.renderForMenu(
         selectedMenu=None,
         skip=TOP_LEVEL_SCANNER_SKIP_MENUS[:len(TOP_LEVEL_SCANNER_SKIP_MENUS)-1],
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
     reply_markup = default_markup([])
     
     """Send a message when the command /help is issued."""
     if update is not None and update.message is not None:
-        await update.message.reply_text(
+        update.message.reply_text(
             f"You can begin by typing in /start (Recommended) and hit send!\n\nOR\n\nChoose an option:\n{cmdText}\n\nWe recommend you start by clicking on this /start"
         )  #  \n\nThis bot restarts every hour starting at 5:30am IST until 10:30pm IST to keep it running on free servers. If it does not respond, please try again in a minutes to avoid the restart duration!
         query = update.message
         message = f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using the bot!"
-        await context.bot.send_message(
-            chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
+        context.bot.send_message(
+            chat_id=int(f"-{Channel_Id}"), text=message, parse_mode="HTML"
         )
 
 
 def _shouldAvoidResponse(update):
     sentFrom = []
     if update.callback_query is not None:
         sentFrom.append(abs(update.callback_query.from_user.id))
@@ -1282,15 +1292,18 @@
     """Run the bot."""
     # Create the Application and pass it your bot's token.
     global chat_idADMIN, Channel_Id, bot_available
     bot_available = availability
     Channel_Id, TOKEN, chat_idADMIN, GITHUB_TOKEN = get_secrets()
     # TOKEN = '1234567'
     # Channel_Id = 1001785195297
-    application = Application.builder().token(TOKEN).build()
+    # application = Application.builder().token(TOKEN).build()
+    application = Updater(TOKEN)
+    # Get the dispatcher to register handlers
+    dispatcher = application.dispatcher
     # Setup conversation handler with the states FIRST and SECOND
     # Use the pattern parameter to pass CallbackQueries with specific
     # data pattern to the corresponding handlers.
     # ^ means "start of line/string"
     # $ means "end of line/string"
     # So ^ABC$ will only allow 'ABC'
     conv_handler = ConversationHandler(
@@ -1309,27 +1322,34 @@
                 CallbackQueryHandler(end, pattern="^" + str("CZ") + "$"),
                 CallbackQueryHandler(start, pattern="^"),
             ],
             END_ROUTES: [],
         },
         fallbacks=[CommandHandler("start", start)],
     )
-    application.add_handler(CommandHandler("help", help_command))
-    application.add_handler(
-        MessageHandler(filters.TEXT & ~filters.COMMAND, help_command)
+    dispatcher.add_handler(CommandHandler("help", help_command))
+    dispatcher.add_handler(
+        MessageHandler(Filters.text & ~Filters.command, help_command)
     )
     # application.add_handler(MessageHandler(filters.TEXT & filters.COMMAND, command_handler))
     # application.add_handler(MessageHandler(filters.COMMAND, command_handler))
     # Add ConversationHandler to application that will be used for handling updates
-    addCommandsForMenuItems(application)
-    application.add_handler(conv_handler)
+    addCommandsForMenuItems(dispatcher)
+    dispatcher.add_handler(conv_handler)
     # ...and the error handler
-    application.add_error_handler(error_handler)
+    dispatcher.add_error_handler(error_handler)
     if bot_available:
         # Run the intraday monitor
         initializeIntradayTimer()
     # Run the bot until the user presses Ctrl-C
-    application.run_polling(allowed_updates=Update.ALL_TYPES)
+    # application.run_polling(allowed_updates=Update.ALL_TYPES)
+    # Start the Bot
+    application.start_polling()
+
+    # Run the bot until you press Ctrl-C or the process receives SIGINT,
+    # SIGTERM or SIGABRT. This should be used most of the time, since
+    # start_polling() is non-blocking and will stop the bot gracefully.
+    application.idle()
 
 
 if __name__ == "__main__":
     runpkscreenerbot()
```

### Comparing `pkscreener-0.45.20240602.426/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240602.427/pkscreener/pkscreenercli.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,120 +614,121 @@
             if "RUNNER" not in os.environ.keys() and ('PKDevTools_Default_Log_Level' in os.environ.keys() and os.environ["PKDevTools_Default_Log_Level"] != str(log.logging.NOTSET)):
                 OutputControls().printOutput(
                     "[+] RuntimeError with 'multiprocessing'.\n[+] Please contact the Developer, if this does not work!"
                 )
                 OutputControls().printOutput(e)
                 traceback.print_exc()
             pass
-
-    OutputControls(enableMultipleLineOutput=(args.monitor is None)).printOutput("",end="\r")
-    
-    configManager.getConfig(ConfigManager.parser)
-    import atexit
-    atexit.register(exitGracefully)
-    # configManager.restartRequestsCache()
-    # args.monitor = configManager.defaultMonitorOptions
-    if args.monitor is not None:
-        MarketMonitor(monitors=args.monitor.split("~") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split("~"),
-                      maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow,
-                      maxNumColsInEachResult=6,
-                      maxNumRowsInEachResult=10,
-                      maxNumResultRowsInMonitor=configManager.maxNumResultRowsInMonitor)
-
-    if args.log or configManager.logsEnabled:
-        setupLogger(shouldLog=True, trace=args.testbuild)
-        if not args.prodbuild and args.answerdefault is None:
-            input("Press <Enter> to continue...")
-    else:
-        if "PKDevTools_Default_Log_Level" in os.environ.keys():
-            del os.environ['PKDevTools_Default_Log_Level']
-            # os.environ["PKDevTools_Default_Log_Level"] = str(log.logging.NOTSET)
-    if args.simulate:
-        os.environ["simulation"] = json.dumps(args.simulate)
-    elif "simulation" in os.environ.keys():
-        del os.environ['simulation']
-    # Import other dependency here because if we import them at the top
-    # multiprocessing behaves in unpredictable ways
-    import pkscreener.classes.Utility as Utility
-
-    configManager.default_logger = default_logger()
-    if originalStdOut is None:
-        # Clear only if this is the first time it's being called from some
-        # loop within workflowtriggers.
-        Utility.tools.clearScreen(userArgs=args, clearAlways=True)
-    warnAboutDependencies()
-    if args.prodbuild:
-        disableSysOut()
-
-    if not configManager.checkConfigFile():
-        configManager.setConfig(
-            ConfigManager.parser, default=True, showFileCreatedText=False
-        )
-    if args.systemlaunched:
-        args.systemlaunched = args.options
-        
-    if args.telegram:
-        # Launched by bot for intraday monitor?
-        if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()):
-            from PKDevTools.classes import Archiver
-            filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs_1.txt")
-            if os.path.exists(filePath):
-                default_logger().info("monitor_outputs_1.txt already exists! This means an instance may already be running. Exiting now...")
-                # Since the file exists, it means, there is another instance running
+    try:
+        OutputControls(enableMultipleLineOutput=(args is None or args.monitor is None)).printOutput("",end="\r")
+        configManager.getConfig(ConfigManager.parser)
+        import atexit
+        atexit.register(exitGracefully)
+        # configManager.restartRequestsCache()
+        # args.monitor = configManager.defaultMonitorOptions
+        if args.monitor is not None:
+            MarketMonitor(monitors=args.monitor.split("~") if len(args.monitor)>5 else configManager.defaultMonitorOptions.split("~"),
+                        maxNumResultsPerRow=configManager.maxDashboardWidgetsPerRow,
+                        maxNumColsInEachResult=6,
+                        maxNumRowsInEachResult=10,
+                        maxNumResultRowsInMonitor=configManager.maxNumResultRowsInMonitor)
+
+        if args.log or configManager.logsEnabled:
+            setupLogger(shouldLog=True, trace=args.testbuild)
+            if not args.prodbuild and args.answerdefault is None:
+                input("Press <Enter> to continue...")
+        else:
+            if "PKDevTools_Default_Log_Level" in os.environ.keys():
+                del os.environ['PKDevTools_Default_Log_Level']
+                # os.environ["PKDevTools_Default_Log_Level"] = str(log.logging.NOTSET)
+        if args.simulate:
+            os.environ["simulation"] = json.dumps(args.simulate)
+        elif "simulation" in os.environ.keys():
+            del os.environ['simulation']
+        # Import other dependency here because if we import them at the top
+        # multiprocessing behaves in unpredictable ways
+        import pkscreener.classes.Utility as Utility
+
+        configManager.default_logger = default_logger()
+        if originalStdOut is None:
+            # Clear only if this is the first time it's being called from some
+            # loop within workflowtriggers.
+            Utility.tools.clearScreen(userArgs=args, clearAlways=True)
+        warnAboutDependencies()
+        if args.prodbuild:
+            disableSysOut()
+
+        if not configManager.checkConfigFile():
+            configManager.setConfig(
+                ConfigManager.parser, default=True, showFileCreatedText=False
+            )
+        if args.systemlaunched:
+            args.systemlaunched = args.options
+            
+        if args.telegram:
+            # Launched by bot for intraday monitor?
+            if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()):
+                from PKDevTools.classes import Archiver
+                filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs_1.txt")
+                if os.path.exists(filePath):
+                    default_logger().info("monitor_outputs_1.txt already exists! This means an instance may already be running. Exiting now...")
+                    # Since the file exists, it means, there is another instance running
+                    sys.exit(0)
+            else:
+                # It should have been launched only during the trading hours
+                default_logger().info("--telegram option must be launched ONLY during NSE trading hours. Exiting now...")
                 sys.exit(0)
+        # Check and see if we're running only the telegram bot
+        if args.bot:
+            from pkscreener import pkscreenerbot
+            pkscreenerbot.runpkscreenerbot(availability=args.botavailable)
+            return
+        
+        if args.intraday:
+            configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
         else:
-            # It should have been launched only during the trading hours
-            default_logger().info("--telegram option must be launched ONLY during NSE trading hours. Exiting now...")
+            configManager.toggleConfig(candleDuration='1d', clearCache=False)
+        if args.options is not None:
+            if str(args.options) == "0":
+                # Must be from unit tests to be able to break out of loops via eventing
+                args.options = None
+            args.options = args.options.replace("::",":")
+        
+        if args.maxprice:
+            configManager.maxLTP = args.maxprice
+            configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
+        if args.minprice:
+            configManager.minLTP = args.minprice
+            configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
+        if args.testbuild and not args.prodbuild:
+            OutputControls().printOutput(
+                colorText.BOLD
+                + colorText.FAIL
+                + "[+] Started in TestBuild mode!"
+                + colorText.END
+            )
+            runApplication()
+        elif args.download:
+            OutputControls().printOutput(
+                colorText.BOLD
+                + colorText.FAIL
+                + "[+] Download ONLY mode! Stocks will not be screened!"
+                + colorText.END
+            )
+            if args.intraday is None:
+                configManager.toggleConfig(candleDuration="1d", clearCache=False)
+            runApplication()
+            from pkscreener.globals import closeWorkersAndExit
+            closeWorkersAndExit()
+            exitGracefully()
             sys.exit(0)
-    # Check and see if we're running only the telegram bot
-    if args.bot:
-        from pkscreener import pkscreenerbot
-        pkscreenerbot.runpkscreenerbot(availability=args.botavailable)
-        return
-    
-    if args.intraday:
-        configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
-    else:
-        configManager.toggleConfig(candleDuration='1d', clearCache=False)
-    if args.options is not None:
-        if str(args.options) == "0":
-            # Must be from unit tests to be able to break out of loops via eventing
-            args.options = None
-        args.options = args.options.replace("::",":")
-    
-    if args.maxprice:
-        configManager.maxLTP = args.maxprice
-        configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
-    if args.minprice:
-        configManager.minLTP = args.minprice
-        configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
-    if args.testbuild and not args.prodbuild:
-        OutputControls().printOutput(
-            colorText.BOLD
-            + colorText.FAIL
-            + "[+] Started in TestBuild mode!"
-            + colorText.END
-        )
-        runApplication()
-    elif args.download:
-        OutputControls().printOutput(
-            colorText.BOLD
-            + colorText.FAIL
-            + "[+] Download ONLY mode! Stocks will not be screened!"
-            + colorText.END
-        )
-        if args.intraday is None:
-            configManager.toggleConfig(candleDuration="1d", clearCache=False)
-        runApplication()
-        from pkscreener.globals import closeWorkersAndExit
-        closeWorkersAndExit()
-        exitGracefully()
-        sys.exit(0)
-    else:
-        runApplicationForScreening()
+        else:
+            runApplicationForScreening()
+    except:
+        pass
 
 def runLoopOnScheduleOrStdApplication(hasCronInterval):
     if hasCronInterval:
         scheduleNextRun()
     else:
         runApplication()
```

### Comparing `pkscreener-0.45.20240602.426/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240602.427/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240602.426
+Version: 0.45.20240602.427
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.426.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240602.427.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240601.425/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240602.426/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240602.426/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240602.427/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240602.426/setup.py` & `pkscreener-0.45.20240602.427/setup.py`

 * *Files identical despite different names*

