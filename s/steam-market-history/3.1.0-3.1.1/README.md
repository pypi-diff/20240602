# Comparing `tmp/steam_market_history-3.1.0.tar.gz` & `tmp/steam_market_history-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steam_market_history-3.1.0.tar", max compression
+gzip compressed data, was "steam_market_history-3.1.1.tar", max compression
```

## Comparing `steam_market_history-3.1.0.tar` & `steam_market_history-3.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-04-18 20:49:45.785180 steam_market_history-3.1.0/LICENSE
--rw-r--r--   0        0        0     6631 2023-04-18 20:49:45.785180 steam_market_history-3.1.0/README.md
--rw-r--r--   0        0        0      706 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      196 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/__init__.py
--rw-r--r--   0        0        0     2897 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/main.py
--rw-r--r--   0        0        0        0 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/modules/__init__.py
--rw-r--r--   0        0        0     1699 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/modules/exporter.py
--rw-r--r--   0        0        0     3572 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/modules/steam.py
--rw-r--r--   0        0        0     6175 2023-04-18 20:49:45.795180 steam_market_history-3.1.0/steam_market_history/templates/index.html
--rw-r--r--   0        0        0     7527 1970-01-01 00:00:00.000000 steam_market_history-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/LICENSE
+-rw-r--r--   0        0        0     6631 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/README.md
+-rw-r--r--   0        0        0      706 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/steam_market_history/__init__.py
+-rw-r--r--   0        0        0     2897 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/steam_market_history/main.py
+-rw-r--r--   0        0        0        0 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/steam_market_history/modules/__init__.py
+-rw-r--r--   0        0        0     1699 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/steam_market_history/modules/exporter.py
+-rw-r--r--   0        0        0     3572 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/steam_market_history/modules/steam.py
+-rw-r--r--   0        0        0     6175 2024-06-02 19:55:06.000000 steam_market_history-3.1.1/steam_market_history/templates/index.html
+-rw-r--r--   0        0        0     7527 1970-01-01 00:00:00.000000 steam_market_history-3.1.1/PKG-INFO
```

### Comparing `steam_market_history-3.1.0/LICENSE` & `steam_market_history-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.1.0/README.md` & `steam_market_history-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.1.0/pyproject.toml` & `steam_market_history-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "steam-market-history"
-version = "3.1.0"
+version = "3.1.1"
 description = "An easy-to-use CLI to export your steam market history to various formats"
 authors = ["Fabian Eulitz <dev@sustineo.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/fabieu/steam-market-history"
 keywords = ["steam", "CLI"]
```

### Comparing `steam_market_history-3.1.0/steam_market_history/main.py` & `steam_market_history-3.1.1/steam_market_history/main.py`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.1.0/steam_market_history/modules/exporter.py` & `steam_market_history-3.1.1/steam_market_history/modules/exporter.py`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.1.0/steam_market_history/modules/steam.py` & `steam_market_history-3.1.1/steam_market_history/modules/steam.py`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.1.0/steam_market_history/templates/index.html` & `steam_market_history-3.1.1/steam_market_history/templates/index.html`

 * *Files identical despite different names*

### Comparing `steam_market_history-3.1.0/PKG-INFO` & `steam_market_history-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steam-market-history
-Version: 3.1.0
+Version: 3.1.1
 Summary: An easy-to-use CLI to export your steam market history to various formats
 Home-page: https://github.com/fabieu/steam-market-history
 License: MIT
 Keywords: steam,CLI
 Author: Fabian Eulitz
 Author-email: dev@sustineo.de
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: steam-market-history Version: 3.1.0 Summary: An
+Metadata-Version: 2.1 Name: steam-market-history Version: 3.1.1 Summary: An
 easy-to-use CLI to export your steam market history to various formats Home-
 page: https://github.com/fabieu/steam-market-history License: MIT Keywords:
 steam,CLI Author: Fabian Eulitz Author-email: dev@sustineo.de Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

