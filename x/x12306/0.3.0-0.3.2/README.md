# Comparing `tmp/x12306-0.3.0.tar.gz` & `tmp/x12306-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x12306-0.3.0.tar", last modified: Thu Apr 25 13:45:49 2024, max compression
+gzip compressed data, was "x12306-0.3.2.tar", last modified: Sun Jun  2 07:53:27 2024, max compression
```

## Comparing `x12306-0.3.0.tar` & `x12306-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.268462 x12306-0.3.0/
--rw-r--r--   0 null       (501) staff       (20)     1060 2024-02-05 11:55:36.000000 x12306-0.3.0/LICENSE
--rw-r--r--   0 null       (501) staff       (20)       25 2024-02-05 12:01:34.000000 x12306-0.3.0/MANIFEST.in
--rw-r--r--   0 null       (501) staff       (20)     4342 2024-04-25 13:45:49.268100 x12306-0.3.0/PKG-INFO
--rw-r--r--   0 null       (501) staff       (20)     3137 2024-04-25 13:43:34.000000 x12306-0.3.0/README.md
--rw-r--r--   0 null       (501) staff       (20)       38 2024-04-25 13:45:49.268571 x12306-0.3.0/setup.cfg
--rw-r--r--   0 null       (501) staff       (20)     2168 2024-02-05 12:50:06.000000 x12306-0.3.0/setup.py
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.263953 x12306-0.3.0/x12306/
--rw-r--r--   0 null       (501) staff       (20)     2226 2024-04-25 13:33:32.000000 x12306-0.3.0/x12306/__init__.py
--rw-r--r--   0 null       (501) staff       (20)      440 2024-04-25 13:21:17.000000 x12306-0.3.0/x12306/__version__.py
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.267481 x12306-0.3.0/x12306/data/
--rw-r--r--   0 null       (501) staff       (20)    31811 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/data/cdn.txt
--rw-r--r--   0 null       (501) staff       (20)        0 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/data/proxies.txt
--rw-r--r--   0 null       (501) staff       (20)    95846 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/data/stations.2019.txt
--rw-r--r--   0 null       (501) staff       (20)   164536 2024-04-25 12:28:49.000000 x12306-0.3.0/x12306/data/stations.txt
--rw-r--r--   0 null       (501) staff       (20)      105 2024-02-05 11:55:36.000000 x12306-0.3.0/x12306/exceptions.py
--rw-r--r--   0 null       (501) staff       (20)     7241 2024-04-25 13:15:35.000000 x12306-0.3.0/x12306/settings.py
--rw-r--r--   0 null       (501) staff       (20)     9557 2024-04-25 13:19:32.000000 x12306-0.3.0/x12306/train.py
--rw-r--r--   0 null       (501) staff       (20)      716 2024-04-25 12:52:51.000000 x12306-0.3.0/x12306/utils.py
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-25 13:45:49.265512 x12306-0.3.0/x12306.egg-info/
--rw-r--r--   0 null       (501) staff       (20)     4342 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/PKG-INFO
--rw-r--r--   0 null       (501) staff       (20)      432 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/SOURCES.txt
--rw-r--r--   0 null       (501) staff       (20)        1 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/dependency_links.txt
--rw-r--r--   0 null       (501) staff       (20)       48 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/entry_points.txt
--rw-r--r--   0 null       (501) staff       (20)       27 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/requires.txt
--rw-r--r--   0 null       (501) staff       (20)        7 2024-04-25 13:45:49.000000 x12306-0.3.0/x12306.egg-info/top_level.txt
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-06-02 07:53:27.585179 x12306-0.3.2/
+-rw-r--r--   0 null       (501) staff       (20)     1060 2024-02-05 11:55:36.000000 x12306-0.3.2/LICENSE
+-rw-r--r--   0 null       (501) staff       (20)       25 2024-02-05 12:01:34.000000 x12306-0.3.2/MANIFEST.in
+-rw-r--r--   0 null       (501) staff       (20)     4342 2024-06-02 07:53:27.584852 x12306-0.3.2/PKG-INFO
+-rw-r--r--   0 null       (501) staff       (20)     3137 2024-04-25 13:43:34.000000 x12306-0.3.2/README.md
+-rw-r--r--   0 null       (501) staff       (20)       38 2024-06-02 07:53:27.585292 x12306-0.3.2/setup.cfg
+-rw-r--r--   0 null       (501) staff       (20)     2178 2024-06-02 06:19:09.000000 x12306-0.3.2/setup.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-06-02 07:53:27.580739 x12306-0.3.2/x12306/
+-rw-r--r--   0 null       (501) staff       (20)     2226 2024-04-25 13:33:32.000000 x12306-0.3.2/x12306/__init__.py
+-rw-r--r--   0 null       (501) staff       (20)      440 2024-06-02 07:53:03.000000 x12306-0.3.2/x12306/__version__.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-06-02 07:53:27.584171 x12306-0.3.2/x12306/data/
+-rw-r--r--   0 null       (501) staff       (20)    31811 2024-02-05 11:55:36.000000 x12306-0.3.2/x12306/data/cdn.txt
+-rw-r--r--   0 null       (501) staff       (20)        0 2024-02-05 11:55:36.000000 x12306-0.3.2/x12306/data/proxies.txt
+-rw-r--r--   0 null       (501) staff       (20)    95846 2024-02-05 11:55:36.000000 x12306-0.3.2/x12306/data/stations.2019.txt
+-rw-r--r--   0 null       (501) staff       (20)   164536 2024-04-25 12:28:49.000000 x12306-0.3.2/x12306/data/stations.txt
+-rw-r--r--   0 null       (501) staff       (20)      105 2024-02-05 11:55:36.000000 x12306-0.3.2/x12306/exceptions.py
+-rw-r--r--   0 null       (501) staff       (20)     7320 2024-06-02 07:45:48.000000 x12306-0.3.2/x12306/settings.py
+-rw-r--r--   0 null       (501) staff       (20)     9833 2024-06-02 07:46:53.000000 x12306-0.3.2/x12306/train.py
+-rw-r--r--   0 null       (501) staff       (20)      716 2024-04-25 12:52:51.000000 x12306-0.3.2/x12306/utils.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-06-02 07:53:27.582195 x12306-0.3.2/x12306.egg-info/
+-rw-r--r--   0 null       (501) staff       (20)     4342 2024-06-02 07:53:27.000000 x12306-0.3.2/x12306.egg-info/PKG-INFO
+-rw-r--r--   0 null       (501) staff       (20)      432 2024-06-02 07:53:27.000000 x12306-0.3.2/x12306.egg-info/SOURCES.txt
+-rw-r--r--   0 null       (501) staff       (20)        1 2024-06-02 07:53:27.000000 x12306-0.3.2/x12306.egg-info/dependency_links.txt
+-rw-r--r--   0 null       (501) staff       (20)       48 2024-06-02 07:53:27.000000 x12306-0.3.2/x12306.egg-info/entry_points.txt
+-rw-r--r--   0 null       (501) staff       (20)       27 2024-06-02 07:53:27.000000 x12306-0.3.2/x12306.egg-info/requires.txt
+-rw-r--r--   0 null       (501) staff       (20)       12 2024-06-02 07:53:27.000000 x12306-0.3.2/x12306.egg-info/top_level.txt
```

### Comparing `x12306-0.3.0/LICENSE` & `x12306-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `x12306-0.3.0/PKG-INFO` & `x12306-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x12306
-Version: 0.3.0
+Version: 0.3.2
 Summary: 12306查票助手，一键查询沿途所有站点，先上车后补票，让你的出行更省心。
 Home-page: https://github.com/0xHJK/x12306
 Author: HJK
 Author-email: HJKdev@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `x12306-0.3.0/README.md` & `x12306-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `x12306-0.3.0/setup.py` & `x12306-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     description=about["__description__"],
     author=about["__author__"],
     author_email=about["__author_email__"],
     url=about["__url__"],
     license=about["__license__"],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_namespace_packages(),
     # package_data={'x12306': ['data']},
     include_package_data=True,
     test_suite="tests",
     entry_points={
         "console_scripts": [
             "x12306 = x12306.__init__:main",
         ],
```

### Comparing `x12306-0.3.0/x12306/__init__.py` & `x12306-0.3.2/x12306/__init__.py`

 * *Files identical despite different names*

### Comparing `x12306-0.3.0/x12306/data/cdn.txt` & `x12306-0.3.2/x12306/data/cdn.txt`

 * *Files identical despite different names*

### Comparing `x12306-0.3.0/x12306/data/stations.2019.txt` & `x12306-0.3.2/x12306/data/stations.2019.txt`

 * *Files identical despite different names*

### Comparing `x12306-0.3.0/x12306/data/stations.txt` & `x12306-0.3.2/x12306/data/stations.txt`

 * *Files identical despite different names*

### Comparing `x12306-0.3.0/x12306/settings.py` & `x12306-0.3.2/x12306/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import re
 import sys
 import platform
 import hashlib
 import secrets
 import requests
 from os import path
+from fake_useragent import UserAgent
 
 # 默认配置
 SEAT_TYPES = {
     "特等座": 25,
     "商务座": 32,
     "一等座": 31,
     "二等座": 30,
@@ -37,16 +38,15 @@
     "Accept": "*/*",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7,ja;q=0.6",
     "Cache-Control": "no-cache",
     "Connection": "keep-alive",
     "Host": "kyfw.12306.cn",
     "Referer": "https://kyfw.12306.cn/otn/leftTicket/init",
-    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_2) AppleWebKit/537.36 (KHTML, like Gecko) "
-    "Chrome/72.0.3626.96 Safari/537.36",
+    "User-Agent": UserAgent().random,
     "X-Requested-With": "XMLHttpRequest",
     "Cookie": "JSESSIONID=" + hashlib.md5(secrets.token_bytes(16)).hexdigest().upper(),
 }
 
 DEFAULT_SEATS = "一等座 二等座 无座"
 DEFAULT_PROXIES_FILE = path.join(path.dirname(__file__), "data", "proxies.txt")
 DEFAULT_STATIONS_FILE = path.join(path.dirname(__file__), "data", "stations.txt")
@@ -140,15 +140,19 @@
 
     @property
     def ts_code(self):
         return self.stations_dict.get(self.ts, "")
 
     @property
     def trains_no_list(self):
-        return self.trains_no.split()
+        if self.trains_no:
+            separators = "[,; ]"  # comma, semicolon, and space
+            return re.split(separators, self.trains_no.upper())
+        else:
+            return []
 
     @property
     def seats_list(self):
         # 获得座位列表
         return [s for s in self.seats.split() if s in SEAT_TYPES]
 
     @property
```

### Comparing `x12306-0.3.0/x12306/train.py` & `x12306-0.3.2/x12306/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,17 @@
     def __eq__(self, other):
         """车次、出发站和目的地相同判断为相等"""
         return (
             self.full_no == other.full_no
             and self._fs == other._fs
             and self._ts == other._ts
         )
+    
+    def __hash__(self) -> int:
+        return hash((self.full_no, self._fs, self._ts))
 
     def __lt__(self, other):
         """根据车次号排序"""
         return self.start_time < other.start_time
 
     def __gt__(self, other):
         """根据车次号排序"""
@@ -183,19 +186,23 @@
         :param url: 查询url
         :param params: 查询参数
         :param retries: 重试次数
         :return: 返回json对象
         """
         s = self.session
         # print("查询中...", " ".join([v for v in params.values()]))
-        if settings.verbose:
-            print(url, params)
+
         try:
             r = s.get(url, params=params, timeout=settings.timeout)
             j = r.json()
+            if settings.verbose:
+                print(url, params)
+                print('\n[REQUEST HEADERS]', s.headers)
+                print('\n[RESPONSE HEADERS]', r.headers)
+                print('\n[RESPONSE TEXT]', r.text)
         except Exception as e:
             print(colorize("第 %i 查询失败" % retries, "red"), e)
             print(url, params)
             print(s.headers)
             if retries < settings.max_retries:
                 time.sleep(retries * settings.timeout)
                 return self._query(url, params, retries + 1)
@@ -292,8 +299,8 @@
         for station in stations_list:
             ts_code = settings.stations_dict.get(station, "")
             if ts_code:
                 trains_list += self._query_trains(
                     fs_code, ts_code, date, trains_no_list
                 )
 
-        return trains_list
+        return list(set(trains_list))
```

### Comparing `x12306-0.3.0/x12306/utils.py` & `x12306-0.3.2/x12306/utils.py`

 * *Files identical despite different names*

### Comparing `x12306-0.3.0/x12306.egg-info/PKG-INFO` & `x12306-0.3.2/x12306.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x12306
-Version: 0.3.0
+Version: 0.3.2
 Summary: 12306查票助手，一键查询沿途所有站点，先上车后补票，让你的出行更省心。
 Home-page: https://github.com/0xHJK/x12306
 Author: HJK
 Author-email: HJKdev@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

