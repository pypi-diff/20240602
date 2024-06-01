# Comparing `tmp/mktdata-0.0.8.tar.gz` & `tmp/mktdata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktdata-0.0.8.tar", last modified: Sat Jun  1 22:44:52 2024, max compression
+gzip compressed data, was "mktdata-0.0.9.tar", last modified: Sat Jun  1 22:55:32 2024, max compression
```

## Comparing `mktdata-0.0.8.tar` & `mktdata-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.664040 mktdata-0.0.8/
--rw-rw-rw-   0        0        0     7616 2024-06-01 22:44:52.663041 mktdata-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.581531 mktdata-0.0.8/markets/
--rw-rw-rw-   0        0        0        0 2024-05-06 15:31:10.000000 mktdata-0.0.8/markets/__init__.py
--rw-rw-rw-   0        0        0     9789 2024-05-24 12:57:09.000000 mktdata-0.0.8/markets/embeddings.py
--rw-rw-rw-   0        0        0     2927 2024-05-22 14:18:00.000000 mktdata-0.0.8/markets/imps.py
--rw-rw-rw-   0        0        0     9304 2024-06-01 22:44:37.000000 mktdata-0.0.8/markets/option_trades.py
--rw-rw-rw-   0        0        0     2355 2024-05-24 12:19:00.000000 mktdata-0.0.8/markets/stock_trades.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.596531 mktdata-0.0.8/mktdata/
--rw-rw-rw-   0        0        0        0 2024-05-29 23:50:02.000000 mktdata-0.0.8/mktdata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.623530 mktdata-0.0.8/mktdata/embeddings/
--rw-rw-rw-   0        0        0        0 2024-05-25 03:59:58.000000 mktdata-0.0.8/mktdata/embeddings/__init__.py
--rw-rw-rw-   0        0        0     7258 2024-05-31 14:38:08.000000 mktdata-0.0.8/mktdata/embeddings/technical_embeds.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.654534 mktdata-0.0.8/mktdata/feeds/
--rw-rw-rw-   0        0        0        0 2024-05-26 03:57:33.000000 mktdata-0.0.8/mktdata/feeds/__init__.py
--rw-rw-rw-   0        0        0        8 2024-05-26 04:43:41.000000 mktdata-0.0.8/mktdata/feeds/helpers.py
--rw-rw-rw-   0        0        0     7422 2024-05-31 15:02:09.000000 mktdata-0.0.8/mktdata/feeds/option_data.py
--rw-rw-rw-   0        0        0     3474 2024-05-28 04:15:01.000000 mktdata-0.0.8/mktdata/feeds/starter.py
--rw-rw-rw-   0        0        0     6630 2024-05-29 13:22:09.000000 mktdata-0.0.8/mktdata/feeds/stock_data.py
--rw-rw-rw-   0        0        0    32901 2024-05-31 14:54:56.000000 mktdata-0.0.8/mktdata/feeds/technicals.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.655534 mktdata-0.0.8/mktdata/models/
--rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.8/mktdata/models/__init__.py
--rw-rw-rw-   0        0        0    31983 2024-05-29 23:49:38.000000 mktdata-0.0.8/mktdata/optionsdata.py
--rw-rw-rw-   0        0        0    16394 2024-05-29 23:49:08.000000 mktdata-0.0.8/mktdata/stock_data.py
-drwxrwxrwx   0        0        0        0 2024-06-01 22:44:52.615531 mktdata-0.0.8/mktdata.egg-info/
--rw-rw-rw-   0        0        0     7616 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4026 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-06-01 22:44:52.000000 mktdata-0.0.8/mktdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 22:44:52.664040 mktdata-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      375 2024-06-01 22:44:29.000000 mktdata-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:55:32.731304 mktdata-0.0.9/
+-rw-rw-rw-   0        0        0     7616 2024-06-01 22:55:32.730303 mktdata-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 22:55:32.712799 mktdata-0.0.9/markets/
+-rw-rw-rw-   0        0        0        0 2024-05-06 15:31:10.000000 mktdata-0.0.9/markets/__init__.py
+-rw-rw-rw-   0        0        0     9789 2024-05-24 12:57:09.000000 mktdata-0.0.9/markets/embeddings.py
+-rw-rw-rw-   0        0        0     2927 2024-05-22 14:18:00.000000 mktdata-0.0.9/markets/imps.py
+-rw-rw-rw-   0        0        0     9304 2024-06-01 22:44:37.000000 mktdata-0.0.9/markets/option_trades.py
+-rw-rw-rw-   0        0        0     2355 2024-05-24 12:19:00.000000 mktdata-0.0.9/markets/stock_trades.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:55:32.714798 mktdata-0.0.9/mktdata/
+-rw-rw-rw-   0        0        0        0 2024-05-29 23:50:02.000000 mktdata-0.0.9/mktdata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:55:32.717798 mktdata-0.0.9/mktdata/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:59:58.000000 mktdata-0.0.9/mktdata/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     7258 2024-05-31 14:38:08.000000 mktdata-0.0.9/mktdata/embeddings/technical_embeds.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:55:32.721798 mktdata-0.0.9/mktdata/feeds/
+-rw-rw-rw-   0        0        0        0 2024-05-26 03:57:33.000000 mktdata-0.0.9/mktdata/feeds/__init__.py
+-rw-rw-rw-   0        0        0        8 2024-05-26 04:43:41.000000 mktdata-0.0.9/mktdata/feeds/helpers.py
+-rw-rw-rw-   0        0        0     7422 2024-05-31 15:02:09.000000 mktdata-0.0.9/mktdata/feeds/option_data.py
+-rw-rw-rw-   0        0        0     3474 2024-05-28 04:15:01.000000 mktdata-0.0.9/mktdata/feeds/starter.py
+-rw-rw-rw-   0        0        0     6630 2024-05-29 13:22:09.000000 mktdata-0.0.9/mktdata/feeds/stock_data.py
+-rw-rw-rw-   0        0        0    32901 2024-05-31 14:54:56.000000 mktdata-0.0.9/mktdata/feeds/technicals.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:55:32.721798 mktdata-0.0.9/mktdata/models/
+-rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.9/mktdata/models/__init__.py
+-rw-rw-rw-   0        0        0    31983 2024-05-29 23:49:38.000000 mktdata-0.0.9/mktdata/optionsdata.py
+-rw-rw-rw-   0        0        0    16394 2024-05-29 23:49:08.000000 mktdata-0.0.9/mktdata/stock_data.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:55:32.716799 mktdata-0.0.9/mktdata.egg-info/
+-rw-rw-rw-   0        0        0     7616 2024-06-01 22:55:32.000000 mktdata-0.0.9/mktdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-06-01 22:55:32.000000 mktdata-0.0.9/mktdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:55:32.000000 mktdata-0.0.9/mktdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4026 2024-06-01 22:55:32.000000 mktdata-0.0.9/mktdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 22:55:32.000000 mktdata-0.0.9/mktdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 22:55:32.731304 mktdata-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      375 2024-06-01 22:55:23.000000 mktdata-0.0.9/setup.py
```

### Comparing `mktdata-0.0.8/PKG-INFO` & `mktdata-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mktdata
-Version: 0.0.8
+Version: 0.0.9
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.5
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: asgiref==3.7.2
 Requires-Dist: astunparse==1.6.3
 Requires-Dist: async-timeout==4.0.3
@@ -114,15 +114,15 @@
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: namex==0.0.7
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nh3==0.2.14
 Requires-Dist: numpy==1.26.4
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: onnxruntime==1.16.1
-Requires-Dist: openai==1.30.1
+Requires-Dist: openai==1.30.5
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-common==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.20.0
 Requires-Dist: opentelemetry-proto==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
```

### Comparing `mktdata-0.0.8/markets/embeddings.py` & `mktdata-0.0.9/markets/embeddings.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/markets/imps.py` & `mktdata-0.0.9/markets/imps.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/markets/option_trades.py` & `mktdata-0.0.9/markets/option_trades.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/markets/stock_trades.py` & `mktdata-0.0.9/markets/stock_trades.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata/embeddings/technical_embeds.py` & `mktdata-0.0.9/mktdata/embeddings/technical_embeds.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata/feeds/option_data.py` & `mktdata-0.0.9/mktdata/feeds/option_data.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata/feeds/starter.py` & `mktdata-0.0.9/mktdata/feeds/starter.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata/feeds/stock_data.py` & `mktdata-0.0.9/mktdata/feeds/stock_data.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata/feeds/technicals.py` & `mktdata-0.0.9/mktdata/feeds/technicals.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata/optionsdata.py` & `mktdata-0.0.9/mktdata/optionsdata.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata/stock_data.py` & `mktdata-0.0.9/mktdata/stock_data.py`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata.egg-info/PKG-INFO` & `mktdata-0.0.9/mktdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mktdata
-Version: 0.0.8
+Version: 0.0.9
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.5
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: asgiref==3.7.2
 Requires-Dist: astunparse==1.6.3
 Requires-Dist: async-timeout==4.0.3
@@ -114,15 +114,15 @@
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: namex==0.0.7
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nh3==0.2.14
 Requires-Dist: numpy==1.26.4
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: onnxruntime==1.16.1
-Requires-Dist: openai==1.30.1
+Requires-Dist: openai==1.30.5
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-common==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.20.0
 Requires-Dist: opentelemetry-proto==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
```

### Comparing `mktdata-0.0.8/mktdata.egg-info/SOURCES.txt` & `mktdata-0.0.9/mktdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mktdata-0.0.8/mktdata.egg-info/requires.txt` & `mktdata-0.0.9/mktdata.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 absl-py==2.0.0
 aiofiles==23.2.1
-aiohttp==3.9.3
+aiohttp==3.9.5
 aiosignal==1.3.1
 annotated-types==0.6.0
 anyio==3.7.1
 appdirs==1.4.4
 asgiref==3.7.2
 astunparse==1.6.3
 async-timeout==4.0.3
@@ -111,15 +111,15 @@
 mypy-extensions==1.0.0
 namex==0.0.7
 natsort==8.4.0
 nh3==0.2.14
 numpy==1.26.4
 oauthlib==3.2.2
 onnxruntime==1.16.1
-openai==1.30.1
+openai==1.30.5
 opentelemetry-api==1.20.0
 opentelemetry-exporter-otlp-proto-common==1.20.0
 opentelemetry-exporter-otlp-proto-grpc==1.20.0
 opentelemetry-proto==1.20.0
 opentelemetry-sdk==1.20.0
 opentelemetry-semantic-conventions==0.41b0
 opt-einsum==3.3.0
```

