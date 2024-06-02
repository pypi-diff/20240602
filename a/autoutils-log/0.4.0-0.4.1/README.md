# Comparing `tmp/autoutils_log-0.4.0.tar.gz` & `tmp/autoutils_log-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoutils_log-0.4.0.tar", max compression
+gzip compressed data, was "autoutils_log-0.4.1.tar", max compression
```

## Comparing `autoutils_log-0.4.0.tar` & `autoutils_log-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-05-24 09:51:08.459971 autoutils_log-0.4.0/LICENSE
--rw-r--r--   0        0        0       15 2024-05-24 19:58:54.498258 autoutils_log-0.4.0/README.md
--rw-r--r--   0        0        0      145 2024-05-24 20:04:31.716923 autoutils_log-0.4.0/autoutils_log/__init__.py
--rw-r--r--   0        0        0     2770 2024-05-24 11:46:55.901305 autoutils_log-0.4.0/autoutils_log/base.py
--rw-r--r--   0        0        0     6239 2024-05-24 20:06:48.732182 autoutils_log-0.4.0/autoutils_log/colorful_stream_handler.py
--rw-r--r--   0        0        0     1811 2024-06-02 12:06:54.005388 autoutils_log-0.4.0/autoutils_log/kafka_handler.py
--rw-r--r--   0        0        0     1263 2024-05-24 11:45:45.476495 autoutils_log-0.4.0/autoutils_log/logstash_handler.py
--rw-r--r--   0        0        0      740 2024-06-02 12:07:03.006544 autoutils_log-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 autoutils_log-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 09:51:08.459971 autoutils_log-0.4.1/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-24 19:58:54.498258 autoutils_log-0.4.1/README.md
+-rw-r--r--   0        0        0      145 2024-05-24 20:04:31.716923 autoutils_log-0.4.1/autoutils_log/__init__.py
+-rw-r--r--   0        0        0     2770 2024-05-24 11:46:55.901305 autoutils_log-0.4.1/autoutils_log/base.py
+-rw-r--r--   0        0        0     6239 2024-05-24 20:06:48.732182 autoutils_log-0.4.1/autoutils_log/colorful_stream_handler.py
+-rw-r--r--   0        0        0     2001 2024-06-02 13:40:35.611523 autoutils_log-0.4.1/autoutils_log/kafka_handler.py
+-rw-r--r--   0        0        0     1263 2024-05-24 11:45:45.476495 autoutils_log-0.4.1/autoutils_log/logstash_handler.py
+-rw-r--r--   0        0        0      714 2024-06-02 13:44:16.052175 autoutils_log-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 autoutils_log-0.4.1/PKG-INFO
```

### Comparing `autoutils_log-0.4.0/LICENSE` & `autoutils_log-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.4.0/autoutils_log/base.py` & `autoutils_log-0.4.1/autoutils_log/base.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.4.0/autoutils_log/colorful_stream_handler.py` & `autoutils_log-0.4.1/autoutils_log/colorful_stream_handler.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.4.0/autoutils_log/kafka_handler.py` & `autoutils_log-0.4.1/autoutils_log/kafka_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import json
 import logging
 import sys
 
 import pytz
-from confluent_kafka import Producer
+from kafka import KafkaProducer
 
 from .base import BaseLogHandler
 
 
 def delivery_report(err, msg):
     pass
 
@@ -16,31 +16,36 @@
 class KafkaHandler(BaseLogHandler):
     """
         A handler class which send data to logstash.
     """
 
     def __init__(self, log_server: str, topic: str, app_name: str = None, host_name: str = None,
                  extra_data: dict = None,
+                 timeout: int = 0,
                  timezone: str = "Asia/Tehran"):
         super().__init__(app_name=app_name, host_name=host_name, extra_data=extra_data)
         self.log_server = log_server
         self.timezone = timezone
         self.topic = topic
-        self.producer = Producer({'bootstrap.servers': self.log_server}) if self.log_server else None
+        self.timeout = timeout
+        self.producer = KafkaProducer(bootstrap_servers=self.log_server,
+                                      value_serializer=lambda v: json.dumps(v).encode("utf-8"),
+                                      linger_ms=10) if self.log_server else None
 
     def _get_send_data(self, record: logging.LogRecord):
         send_data = super()._get_send_data(record=record)
         send_data["time"] = self.get_now_time_for_elastic()
         return send_data
 
     def send(self, send_data: dict):
         if self.producer is None:
             return
-        self.producer.produce(self.topic, json.dumps(send_data).encode("utf-8"), callback=delivery_report)
-        self.producer.poll(timeout=2)
+        self.producer.send(self.topic, send_data)
+        # self.producer.flush(timeout=1.0)
+        # future.get(timeout=60)
 
     def emit(self, record: logging.LogRecord) -> None:
         if not self.log_server or not self.topic:
             return
         try:
             send_data = self._get_send_data(record=record)
             self.send(send_data=send_data)
```

### Comparing `autoutils_log-0.4.0/autoutils_log/logstash_handler.py` & `autoutils_log-0.4.1/autoutils_log/logstash_handler.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.4.0/pyproject.toml` & `autoutils_log-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoutils-log"
-version = "0.4.0"
+version = "0.4.1"
 description = "Some Good Function For Log"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/autoutils-log"
 repository = "https://github.com/rezazeiny/autoutils-log"
 keywords = ["autoutils_log"]
@@ -19,13 +19,12 @@
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pytz = "*"
 termcolor = ">=2.4.0"
 requests = "~=2.32"
 persiantools = "~=4.0"
-confluent-kafka = "~=2.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoutils_log-0.4.0/PKG-INFO` & `autoutils_log-0.4.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: autoutils-log
-Version: 0.4.0
+Version: 0.4.1
 Summary: Some Good Function For Log
 Home-page: https://github.com/rezazeiny/autoutils-log
 License: MIT
 Keywords: autoutils_log
 Author: Reza Zeiny
 Author-email: rezazeiny1998@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: confluent-kafka (>=2.4,<3.0)
 Requires-Dist: persiantools (>=4.0,<5.0)
 Requires-Dist: pytz
 Requires-Dist: requests (>=2.32,<3.0)
 Requires-Dist: termcolor (>=2.4.0)
 Project-URL: Repository, https://github.com/rezazeiny/autoutils-log
 Description-Content-Type: text/markdown
```

