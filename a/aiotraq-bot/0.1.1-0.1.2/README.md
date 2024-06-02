# Comparing `tmp/aiotraq_bot-0.1.1.tar.gz` & `tmp/aiotraq_bot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotraq_bot-0.1.1.tar", max compression
+gzip compressed data, was "aiotraq_bot-0.1.2.tar", max compression
```

## Comparing `aiotraq_bot-0.1.1.tar` & `aiotraq_bot-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2031 2024-05-17 23:04:35.814594 aiotraq_bot-0.1.1/README.md
--rw-r--r--   0        0        0       56 2024-05-17 16:38:32.117803 aiotraq_bot-0.1.1/aiotraq_bot/__init__.py
--rw-r--r--   0        0        0     6768 2024-05-17 21:04:40.681419 aiotraq_bot-0.1.1/aiotraq_bot/bot.py
--rw-r--r--   0        0        0     2039 2024-05-17 21:01:35.876405 aiotraq_bot-0.1.1/aiotraq_bot/models/__init__.py
--rw-r--r--   0        0        0     4454 2024-05-17 02:13:14.422584 aiotraq_bot-0.1.1/aiotraq_bot/models/common.py
--rw-r--r--   0        0        0     6396 2024-05-17 21:00:25.687801 aiotraq_bot-0.1.1/aiotraq_bot/models/event.py
--rw-r--r--   0        0        0     3182 2024-05-17 21:00:13.643373 aiotraq_bot-0.1.1/aiotraq_bot/models/event_models.py
--rw-r--r--   0        0        0        0 2024-05-15 23:16:09.027514 aiotraq_bot-0.1.1/aiotraq_bot/py.typed
--rw-r--r--   0        0        0     1045 2024-05-17 23:17:23.707417 aiotraq_bot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 aiotraq_bot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2177 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/README.md
+-rw-r--r--   0        0        0       56 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/aiotraq_bot/__init__.py
+-rw-r--r--   0        0        0     6768 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/aiotraq_bot/bot.py
+-rw-r--r--   0        0        0     2039 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/aiotraq_bot/models/__init__.py
+-rw-r--r--   0        0        0     4454 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/aiotraq_bot/models/common.py
+-rw-r--r--   0        0        0     6396 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/aiotraq_bot/models/event.py
+-rw-r--r--   0        0        0     3182 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/aiotraq_bot/models/event_models.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/aiotraq_bot/py.typed
+-rw-r--r--   0        0        0     1116 2024-06-02 10:08:59.285105 aiotraq_bot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 aiotraq_bot-0.1.2/PKG-INFO
```

### Comparing `aiotraq_bot-0.1.1/README.md` & `aiotraq_bot-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # aiotraq-bot
 
 Async ready traQ Bot library written in Python.
 
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/aiotraq-bot)](https://pypi.org/project/aiotraq-bot/)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
+[![CI](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml/badge.svg)](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml)
 
 ## Requirements
 
 aiotraq-bot は以下のライブラリを使用しています。
 
 - [FastAPI](https://fastapi.tiangolo.com/): サーバーの実装
 - [Uvicorn](https://www.uvicorn.org/): サーバーの実行
```

### Comparing `aiotraq_bot-0.1.1/aiotraq_bot/bot.py` & `aiotraq_bot-0.1.2/aiotraq_bot/bot.py`

 * *Files identical despite different names*

### Comparing `aiotraq_bot-0.1.1/aiotraq_bot/models/__init__.py` & `aiotraq_bot-0.1.2/aiotraq_bot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotraq_bot-0.1.1/aiotraq_bot/models/common.py` & `aiotraq_bot-0.1.2/aiotraq_bot/models/common.py`

 * *Files identical despite different names*

### Comparing `aiotraq_bot-0.1.1/aiotraq_bot/models/event.py` & `aiotraq_bot-0.1.2/aiotraq_bot/models/event.py`

 * *Files identical despite different names*

### Comparing `aiotraq_bot-0.1.1/aiotraq_bot/models/event_models.py` & `aiotraq_bot-0.1.2/aiotraq_bot/models/event_models.py`

 * *Files identical despite different names*

### Comparing `aiotraq_bot-0.1.1/pyproject.toml` & `aiotraq_bot-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiotraq-bot"
-version = "0.1.1"
+version = "0.1.2"
 description = "Async ready traQ Bot library"
 authors = ["toshi00"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/toshi-pono/aiotraq"
 packages = [{ include = "aiotraq_bot" }]
 include = ["aiotraq_bot/py.typed"]
@@ -16,14 +16,18 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 fastapi = ">=0.100.0"
 uvicorn = { extras = ["standard"], version = ">=0.12.0" }
 
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.10.0"
+ruff = "^0.4.7"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.mypy]
 show_error_context = true
```

### Comparing `aiotraq_bot-0.1.1/PKG-INFO` & `aiotraq_bot-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotraq-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Async ready traQ Bot library
 Home-page: https://github.com/toshi-pono/aiotraq
 License: MIT
 Keywords: traQ,bot,async,aiotraq
 Author: toshi00
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,16 +18,17 @@
 Project-URL: Source Code, https://github.com/toshi-pono/aiotraq/tree/main/libs/bot
 Description-Content-Type: text/markdown
 
 # aiotraq-bot
 
 Async ready traQ Bot library written in Python.
 
-[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/aiotraq-bot)](https://pypi.org/project/aiotraq-bot/)
+[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/toshi-pono/aiotraq/blob/main/LICENSE)
+[![CI](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml/badge.svg)](https://github.com/toshi-pono/aiotraq/actions/workflows/ci.yml)
 
 ## Requirements
 
 aiotraq-bot は以下のライブラリを使用しています。
 
 - [FastAPI](https://fastapi.tiangolo.com/): サーバーの実装
 - [Uvicorn](https://www.uvicorn.org/): サーバーの実行
```

