# Comparing `tmp/fintime-0.1.5.tar.gz` & `tmp/fintime-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fintime-0.1.5.tar", max compression
+gzip compressed data, was "fintime-0.1.6.tar", max compression
```

## Comparing `fintime-0.1.5.tar` & `fintime-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11578 2024-03-18 11:59:39.112268 fintime-0.1.5/README.md
--rw-r--r--   0        0        0      134 2024-03-03 17:05:26.498708 fintime-0.1.5/fintime/__init__.py
--rw-r--r--   0        0        0     6234 2024-03-16 20:33:03.683632 fintime-0.1.5/fintime/abc.py
--rw-r--r--   0        0        0      469 2024-03-17 21:10:14.211922 fintime-0.1.5/fintime/artists/__init__.py
--rw-r--r--   0        0        0     4997 2024-03-18 11:55:12.086857 fintime-0.1.5/fintime/artists/candlestick.py
--rw-r--r--   0        0        0     3420 2024-03-18 11:35:10.333485 fintime-0.1.5/fintime/artists/diverging_bar.py
--rw-r--r--   0        0        0     2632 2024-03-16 20:55:23.664778 fintime-0.1.5/fintime/artists/fill_between.py
--rw-r--r--   0        0        0     2480 2024-03-18 10:05:47.932720 fintime-0.1.5/fintime/artists/line.py
--rw-r--r--   0        0        0     6684 2024-03-18 10:58:38.970228 fintime-0.1.5/fintime/artists/trade_annotation.py
--rw-r--r--   0        0        0     1632 2024-03-11 11:32:13.017371 fintime-0.1.5/fintime/artists/utils.py
--rw-r--r--   0        0        0     3403 2024-03-16 20:37:08.248100 fintime-0.1.5/fintime/artists/volume.py
--rw-r--r--   0        0        0     7863 2024-03-18 11:38:36.645686 fintime-0.1.5/fintime/composites.py
--rw-r--r--   0        0        0     8356 2024-03-18 11:34:17.012420 fintime-0.1.5/fintime/config.py
--rw-r--r--   0        0        0     3391 2024-03-18 10:24:35.187032 fintime-0.1.5/fintime/mock/data.py
--rw-r--r--   0        0        0     2631 2024-03-18 11:01:56.166809 fintime-0.1.5/fintime/plot.py
--rw-r--r--   0        0        0     3271 2024-03-10 10:48:37.310486 fintime-0.1.5/fintime/ticks.py
--rw-r--r--   0        0        0     1084 2024-03-18 09:19:44.569976 fintime-0.1.5/fintime/types.py
--rw-r--r--   0        0        0      773 2024-03-10 11:35:46.826382 fintime-0.1.5/fintime/utils.py
--rw-r--r--   0        0        0     3893 2024-03-18 08:55:29.771807 fintime-0.1.5/fintime/validation.py
--rw-r--r--   0        0        0      754 2024-03-18 12:02:28.022237 fintime-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    12597 1970-01-01 00:00:00.000000 fintime-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11578 2024-03-18 11:59:39.112268 fintime-0.1.6/README.md
+-rw-r--r--   0        0        0      134 2024-03-03 17:05:26.498708 fintime-0.1.6/fintime/__init__.py
+-rw-r--r--   0        0        0     6234 2024-03-16 20:33:03.683632 fintime-0.1.6/fintime/abc.py
+-rw-r--r--   0        0        0      469 2024-03-17 21:10:14.211922 fintime-0.1.6/fintime/artists/__init__.py
+-rw-r--r--   0        0        0     4997 2024-03-18 11:55:12.086857 fintime-0.1.6/fintime/artists/candlestick.py
+-rw-r--r--   0        0        0     3420 2024-03-18 11:35:10.333485 fintime-0.1.6/fintime/artists/diverging_bar.py
+-rw-r--r--   0        0        0     2632 2024-03-16 20:55:23.664778 fintime-0.1.6/fintime/artists/fill_between.py
+-rw-r--r--   0        0        0     2480 2024-03-18 10:05:47.932720 fintime-0.1.6/fintime/artists/line.py
+-rw-r--r--   0        0        0     6684 2024-03-18 10:58:38.970228 fintime-0.1.6/fintime/artists/trade_annotation.py
+-rw-r--r--   0        0        0     1632 2024-03-11 11:32:13.017371 fintime-0.1.6/fintime/artists/utils.py
+-rw-r--r--   0        0        0     3403 2024-03-16 20:37:08.248100 fintime-0.1.6/fintime/artists/volume.py
+-rw-r--r--   0        0        0     7863 2024-03-18 11:38:36.645686 fintime-0.1.6/fintime/composites.py
+-rw-r--r--   0        0        0     8356 2024-03-18 11:34:17.012420 fintime-0.1.6/fintime/config.py
+-rw-r--r--   0        0        0     3391 2024-03-18 10:24:35.187032 fintime-0.1.6/fintime/mock/data.py
+-rw-r--r--   0        0        0     2631 2024-03-18 11:01:56.166809 fintime-0.1.6/fintime/plot.py
+-rw-r--r--   0        0        0     3271 2024-03-10 10:48:37.310486 fintime-0.1.6/fintime/ticks.py
+-rw-r--r--   0        0        0     1084 2024-03-18 09:19:44.569976 fintime-0.1.6/fintime/types.py
+-rw-r--r--   0        0        0      773 2024-03-10 11:35:46.826382 fintime-0.1.6/fintime/utils.py
+-rw-r--r--   0        0        0     3893 2024-03-18 08:55:29.771807 fintime-0.1.6/fintime/validation.py
+-rw-r--r--   0        0        0      755 2024-06-02 16:06:16.931848 fintime-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    12602 1970-01-01 00:00:00.000000 fintime-0.1.6/PKG-INFO
```

### Comparing `fintime-0.1.5/README.md` & `fintime-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/abc.py` & `fintime-0.1.6/fintime/abc.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/artists/candlestick.py` & `fintime-0.1.6/fintime/artists/candlestick.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/artists/diverging_bar.py` & `fintime-0.1.6/fintime/artists/diverging_bar.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/artists/fill_between.py` & `fintime-0.1.6/fintime/artists/fill_between.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/artists/line.py` & `fintime-0.1.6/fintime/artists/line.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/artists/trade_annotation.py` & `fintime-0.1.6/fintime/artists/trade_annotation.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/artists/utils.py` & `fintime-0.1.6/fintime/artists/utils.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/artists/volume.py` & `fintime-0.1.6/fintime/artists/volume.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/composites.py` & `fintime-0.1.6/fintime/composites.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/config.py` & `fintime-0.1.6/fintime/config.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/mock/data.py` & `fintime-0.1.6/fintime/mock/data.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/plot.py` & `fintime-0.1.6/fintime/plot.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/ticks.py` & `fintime-0.1.6/fintime/ticks.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/types.py` & `fintime-0.1.6/fintime/types.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/utils.py` & `fintime-0.1.6/fintime/utils.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/fintime/validation.py` & `fintime-0.1.6/fintime/validation.py`

 * *Files identical despite different names*

### Comparing `fintime-0.1.5/pyproject.toml` & `fintime-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fintime"
-version = "0.1.5"
+version = "0.1.6"
 description = "Financial Time Series Plotting Libarary"
 license = "Apache-2.0"
 authors = ["Marcel de Haan <mdehaan35@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/marcel-dehaan/fintime"
 packages = [{ include = "fintime" }]
 classifiers = [
@@ -12,15 +12,15 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 PyYAML = "*"
-matplotlib = "3.0"
+matplotlib = "^3.0"
 nptyping = "*"
 python-dateutil = "*"
 numpy = "*"
 fieldconfig = "^0.1.6"
 
 [tool.poetry.dev-dependencies]
 black = "*"
```

### Comparing `fintime-0.1.5/PKG-INFO` & `fintime-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fintime
-Version: 0.1.5
+Version: 0.1.6
 Summary: Financial Time Series Plotting Libarary
 Home-page: https://github.com/marcel-dehaan/fintime
 License: Apache-2.0
 Author: Marcel de Haan
 Author-email: mdehaan35@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Dist: PyYAML
 Requires-Dist: fieldconfig (>=0.1.6,<0.2.0)
-Requires-Dist: matplotlib (==3.0)
+Requires-Dist: matplotlib (>=3.0,<4.0)
 Requires-Dist: nptyping
 Requires-Dist: numpy
 Requires-Dist: python-dateutil
 Description-Content-Type: text/markdown
 
 # FinTime
 FinTime is a financial time series plotting library built on Matplotlib.
```

