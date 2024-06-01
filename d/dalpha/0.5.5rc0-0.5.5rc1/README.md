# Comparing `tmp/dalpha-0.5.5rc0.tar.gz` & `tmp/dalpha-0.5.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.5rc0.tar", max compression
+gzip compressed data, was "dalpha-0.5.5rc1.tar", max compression
```

## Comparing `dalpha-0.5.5rc0.tar` & `dalpha-0.5.5rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.5rc0/README.md
--rw-r--r--   0        0        0     2104 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/__init__.py
--rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.5rc0/dalpha/agent.py
--rw-r--r--   0        0        0     7889 2024-05-22 02:06:09.763823 dalpha-0.5.5rc0/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.5rc0/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/context.py
--rw-r--r--   0        0        0     2970 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/data_update_cls.py
--rw-r--r--   0        0        0     3087 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/data_update_consumer.py
--rw-r--r--   0        0        0     1798 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/dto.py
--rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.5rc0/dalpha/exception.py
--rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.5rc0/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.5rc0/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.5rc0/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6689 2024-05-22 02:06:09.767823 dalpha-0.5.5rc0/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.5rc0/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.5rc0/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.5rc0/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.5rc0/dalpha/request.py
--rw-r--r--   0        0        0     2673 2024-05-23 10:37:42.216823 dalpha-0.5.5rc0/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/signal_handler.py
--rw-r--r--   0        0        0     4612 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.5rc0/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.5rc1/README.md
+-rw-r--r--   0        0        0     2159 2024-06-01 20:46:02.704147 dalpha-0.5.5rc1/dalpha/__init__.py
+-rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.5rc1/dalpha/agent.py
+-rw-r--r--   0        0        0     7889 2024-05-22 02:06:09.763823 dalpha-0.5.5rc1/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.5rc1/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.5rc1/dalpha/context.py
+-rw-r--r--   0        0        0     2970 2024-06-01 12:03:50.256168 dalpha-0.5.5rc1/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0     4688 2024-06-01 20:46:02.704147 dalpha-0.5.5rc1/dalpha/data_update_consumer.py
+-rw-r--r--   0        0        0     1798 2024-06-01 12:03:50.256168 dalpha-0.5.5rc1/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.5rc1/dalpha/exception.py
+-rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.5rc1/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.5rc1/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.5rc1/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.5rc1/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.5rc1/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.5rc1/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6689 2024-05-22 02:06:09.767823 dalpha-0.5.5rc1/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.5rc1/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.5rc1/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.5rc1/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.5rc1/dalpha/request.py
+-rw-r--r--   0        0        0     2673 2024-05-23 10:37:42.216823 dalpha-0.5.5rc1/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.5rc1/dalpha/signal_handler.py
+-rw-r--r--   0        0        0     4607 2024-06-01 20:46:02.704147 dalpha-0.5.5rc1/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-06-01 20:46:02.704147 dalpha-0.5.5rc1/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.5rc1/PKG-INFO
```

### Comparing `dalpha-0.5.5rc0/README.md` & `dalpha-0.5.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/__init__.py` & `dalpha-0.5.5rc1/dalpha/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,8 +48,9 @@
 from dalpha.cobra_cls import Cobra
 from dalpha.data_update_cls import DalphaDataUpdater
 from dalpha.inference_cls import DalphaAI
 from dalpha.redis_cls import DalphaRedis
 from dalpha.openai_cls import DalphaOpenAI
 from dalpha.backend_cli import BackendCli, internal_call, slack_alert
 from dalpha.message_consumer import EvaluateItem
+from dalpha.data_update_consumer import DataUpdateItem
 import dalpha.s3 as s3
```

### Comparing `dalpha-0.5.5rc0/dalpha/agent.py` & `dalpha-0.5.5rc1/dalpha/agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/backend_cli.py` & `dalpha-0.5.5rc1/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/cobra_cls.py` & `dalpha-0.5.5rc1/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/context.py` & `dalpha-0.5.5rc1/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/data_update_cls.py` & `dalpha-0.5.5rc1/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/dto.py` & `dalpha-0.5.5rc1/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/exception.py` & `dalpha-0.5.5rc1/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/inference_cls.py` & `dalpha-0.5.5rc1/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/logging/__init__.py` & `dalpha-0.5.5rc1/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/logging/log_formatter.py` & `dalpha-0.5.5rc1/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/logging/utils.py` & `dalpha-0.5.5rc1/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/message_consumer.py` & `dalpha-0.5.5rc1/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/openai_cls.py` & `dalpha-0.5.5rc1/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/redis_cli.py` & `dalpha-0.5.5rc1/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/redis_cls.py` & `dalpha-0.5.5rc1/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/request.py` & `dalpha-0.5.5rc1/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/s3.py` & `dalpha-0.5.5rc1/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5rc0/dalpha/update_agent.py` & `dalpha-0.5.5rc1/dalpha/update_agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,66 +2,64 @@
 import json
 import os
 from typing import List
 from dalpha.logging import logger
 import sentry_sdk
 from dalpha.backend_cli import BackendCli
 from dalpha.context import Context, get_context, set_context
-from dalpha.data_update_consumer import DataUpdateItem, KafkaDataUpdateConsumer
+from dalpha.data_update_consumer import DataUpdateItem, KafkaDataUpdateConsumer, SqsDataUpdateConsumer
 from dalpha.logging.events import Event
 from dalpha.backend_cli import slack_alert
 
 class UpdateAgent:
     def __init__(
         self,
-        kafka_topic: str,
+        target: str,
+        consumer_type: str = "SQS",
         api_id: int = int(os.environ.get('API_ID', 0)),
         dev_server: bool = bool(os.environ.get('DEV_SERVER', 'True') == 'True')
     ):
-        if not isinstance(kafka_topic, str): raise TypeError('kafka_topic is not a str')
+        if not isinstance(target, str): raise TypeError('target is not a str')
         if not isinstance(api_id, int): raise TypeError('api_id is not a int')
         if not isinstance(dev_server, bool): raise TypeError('dev_server is not a bool')
 
-        self.kafka_topic = kafka_topic
+        self.target = target
         self.token = os.environ['TOKEN']
         self.sentry_dsn = os.environ['SENTRY_DSN']
         if dev_server:
             self.sentry_env = "exp"
         else:
             self.sentry_env = "production"
         
         self.backend_cli = BackendCli(
             api_id = api_id,
             dev_server = dev_server,
             token = self.token
         )
-        self.data_update_consumer = KafkaDataUpdateConsumer(
-            api_id = api_id,
-            backend_cli = self.backend_cli,
-            kafka_topic = kafka_topic
-        )
-
-        set_context(Context(
-            inference_id = api_id,
-            service_code = kafka_topic,
-            env = "exp" if dev_server else "prod"
-        ))
+        if consumer_type == "KAFKA":
+            self.data_update_consumer = KafkaDataUpdateConsumer(
+                topic = target,
+                api_id = api_id
+            )
+        else:
+            self.data_update_consumer = SqsDataUpdateConsumer(
+                queue_url = f"https://sqs.ap-northeast-2.amazonaws.com/855014179775/{target}"
+            )
 
         sentry_sdk.set_context("context",asdict(get_context()))
         sentry_sdk.init(
             dsn=self.sentry_dsn,
 
             # Set traces_sample_rate to 1.0 to capture 100%
             # of transactions for performance monitoring.
             # We recommend adjusting this value in production.
             traces_sample_rate=1.0,
             environment = self.sentry_env
         )
         sentry_sdk.set_tag("api_id", api_id)
-        sentry_sdk.set_tag("service_code", kafka_topic)
         sentry_sdk.set_tag("engineer", self.backend_cli.get_internal_slack())
 
     def poll(self):
         '''
         data update의 경우 kafka로부터 data update event가 담긴 메세지를 받아온다.
         '''
         ret: List[DataUpdateItem] = self.data_update_consumer.poll()
```

### Comparing `dalpha-0.5.5rc0/PKG-INFO` & `dalpha-0.5.5rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.5rc0
+Version: 0.5.5rc1
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

