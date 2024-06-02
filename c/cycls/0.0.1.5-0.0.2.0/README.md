# Comparing `tmp/cycls-0.0.1.5.tar.gz` & `tmp/cycls-0.0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycls-0.0.1.5.tar", max compression
+gzip compressed data, was "cycls-0.0.2.0.tar", max compression
```

## Comparing `cycls-0.0.1.5.tar` & `cycls-0.0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.1.5/LICENSE
--rw-r--r--   0        0        0     2204 2024-05-02 06:45:15.624431 cycls-0.0.1.5/README.md
--rw-r--r--   0        0        0      663 2024-05-18 09:30:48.832041 cycls-0.0.1.5/cycls/UI.py
--rw-r--r--   0        0        0      108 2024-05-02 06:45:15.625156 cycls-0.0.1.5/cycls/__init__.py
--rw-r--r--   0        0        0     7014 2024-05-18 09:30:48.832530 cycls-0.0.1.5/cycls/client.py
--rw-r--r--   0        0        0      786 2024-05-18 09:30:48.833323 cycls-0.0.1.5/cycls/configuration.py
--rw-r--r--   0        0        0      160 2024-05-18 09:30:48.833639 cycls-0.0.1.5/cycls/settings.py
--rw-r--r--   0        0        0      120 2024-05-02 06:45:15.626692 cycls-0.0.1.5/cycls/static.py
--rw-r--r--   0        0        0     5123 2024-05-18 09:30:48.833996 cycls-0.0.1.5/cycls/typings.py
--rw-r--r--   0        0        0      728 2024-05-18 09:31:18.857658 cycls-0.0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 cycls-0.0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.2.0/LICENSE
+-rw-r--r--   0        0        0     2204 2024-05-02 06:45:15.624431 cycls-0.0.2.0/README.md
+-rw-r--r--   0        0        0      663 2024-05-29 22:42:44.524280 cycls-0.0.2.0/cycls/UI.py
+-rw-r--r--   0        0        0      171 2024-06-02 15:40:50.122993 cycls-0.0.2.0/cycls/__init__.py
+-rw-r--r--   0        0        0     7105 2024-06-02 16:24:41.473630 cycls-0.0.2.0/cycls/client.py
+-rw-r--r--   0        0        0      785 2024-06-02 15:40:50.123439 cycls-0.0.2.0/cycls/configuration.py
+-rw-r--r--   0        0        0      160 2024-05-18 09:30:48.833639 cycls-0.0.2.0/cycls/settings.py
+-rw-r--r--   0        0        0      120 2024-05-02 06:45:15.626692 cycls-0.0.2.0/cycls/static.py
+-rw-r--r--   0        0        0     7271 2024-06-02 16:24:41.473996 cycls-0.0.2.0/cycls/typings.py
+-rw-r--r--   0        0        0      846 2024-06-02 16:24:41.475408 cycls-0.0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3072 1970-01-01 00:00:00.000000 cycls-0.0.2.0/PKG-INFO
```

### Comparing `cycls-0.0.1.5/LICENSE` & `cycls-0.0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cycls-0.0.1.5/README.md` & `cycls-0.0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cycls-0.0.1.5/cycls/UI.py` & `cycls-0.0.2.0/cycls/UI.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.1.5/cycls/client.py` & `cycls-0.0.2.0/cycls/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
-from inspect import iscoroutinefunction, signature, Parameter, _empty
+from inspect import signature, Parameter, _empty
 from typing import Callable, Any
 from datetime import datetime
 from functools import wraps
 
-from socketio import AsyncClient, Client
+from socketio import AsyncClient, Client  # type: ignore[import-untyped]
 import asyncio
 import re
 
 from .UI import Text, Image
 from .configuration import AppConfiguration
 from .typings import (
     InputTypeHint,
     AsyncContext,
     SyncContext,
     ConversationID,
     ConversationSession,
-    Meta,
     Response,
     Message,
     MessageContent,
 )
 from .static import HANDLER_PATTERN, CYCLS_URL
 
 
@@ -100,16 +99,15 @@
 
     def __extract_handler_name(self, handler: str) -> str:
         name = re.search(rf"^\@({HANDLER_PATTERN})$", handler.strip().lower())
         if not name:
             raise Exception(
                 "Your app handler has to start with @ and composed only of letters, numbers and '-'"
             )
-        name = name.group(1)
-        return re.sub(r"_", "-", name)
+        return re.sub(r"_", "-", name.group(1))
 
     def connection_log(self, data):
         print(
             f"{datetime.now()}: HANDLER|{data.get('handler')} -> {data.get('message')}. STATUS: {data.get('status')}"
         )
 
 
@@ -154,26 +152,24 @@
             transports=["websocket"],
             socketio_path="/app-socket/socket.io",
         )
         self.sio.wait()
 
     def publish(self):
         self._run()
+    def __run_app(self, func, message):
+        func(**self.process_handler_input(func, message))
+        message.send.finish(message.send.user_message_id)
 
     def __call__(self, func):
         @wraps
         @self.sio.on(self.app_config.handler)
         def wrapper(data):
-            message = SyncContext(sio=self.sio, **data)
-            func(**self.process_handler_input(func, message))
-            message.send.send_message(
-                None, message.send.user_message_id, True, "finish"
-            )
-            return 200
-
+            message = SyncContext(sio=self.sio, url=self.server_url, **data)
+            self.sio.start_background_task(self.__run_app, func, message)
         return wrapper
 
 
 class AsyncApp(BaseApp):
     sio: AsyncClient
 
     def __init__(
@@ -194,16 +190,15 @@
             welcome=welcome,
             suggestions=suggestions,
             **kwargs,
         )
         self.sio = AsyncClient(
             reconnection_attempts=0,
             reconnection_delay=1,
-            reconnection_delay_max=25,
-            logger=True,
+            reconnection_delay_max=25
         )
         self.sio.on("connect")(self.re_connect)
         self.sio.on("connection_log")(self.connection_log)
 
     async def re_connect(self):
         await self.sio.emit("connect_app", data=self.app_config.model_dump(mode="json"))
 
@@ -219,19 +214,19 @@
         )
         await self.sio.wait()
 
     def publish(self):
         loop = asyncio.new_event_loop()
         loop.run_until_complete(self._run())
 
+    async def __run_app(self, func, message):
+        await func(**self.process_handler_input(func, message))
+        await asyncio.sleep(0.2)
+        await message.send.finish(message.send.user_message_id)
+
     def __call__(self, func):
         @wraps
         @self.sio.on(self.app_config.handler)
         async def wrapper(data):
-            message = AsyncContext(sio=self.sio, **data)
-            await func(**self.process_handler_input(func, message))
-            await message.send.send_message(
-                None, message.send.user_message_id, True, "finish"
-            )
-            return 200
-
+            message = AsyncContext(sio=self.sio, url=self.server_url, **data)
+            await self.sio.start_background_task(self.__run_app, func, message)
         return wrapper
```

### Comparing `cycls-0.0.1.5/cycls/configuration.py` & `cycls-0.0.2.0/cycls/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     def process_suggestions(cls, suggestions: list[str] | None) -> list[str] | None:
         if not suggestions:
             return None
         elif isinstance(suggestions, list):
             if len(suggestions) <= 4:
                 return suggestions
             else:
-                raise Exception(f"suggestions can be at max 4")
+                raise Exception("suggestions can be at max 4")
 
     # @field_validator("image", mode="before")
     # @classmethod
     # def process_image(cls, image:str | None) -> str:
     #     return image
```

### Comparing `cycls-0.0.1.5/pyproject.toml` & `cycls-0.0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycls"
-version = "0.0.1.5"
+version = "0.0.2.0"
 description = "Publish your chat app with cycls"
 authors = ["Khalid Alrasheed <khalid@cycls.io>"]
 packages = [{ include = "cycls" }]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.cycls.com/"
 documentation = "https://docs.cycls.com/"
@@ -14,14 +14,21 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 asyncio = "^3.4.3"
 certifi = "^2023.11.17"
 httpx = "^0.25.2"
 pydantic = "^2.5.2"
 python-socketio = {extras = ["asyncio-client", "client"], version = "^5.11.2"}
+pydantic-settings = "^2.2.1"
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "^23.11.0", allow-prereleases = true }
+ruff = "^0.4.5"
+mypy = "^1.10.0"
+
+
+[tool.poetry.group.test.dependencies]
+groq = "^0.8.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cycls-0.0.1.5/PKG-INFO` & `cycls-0.0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycls
-Version: 0.0.1.5
+Version: 0.0.2.0
 Summary: Publish your chat app with cycls
 Home-page: https://www.cycls.com/
 License: MIT
 Keywords: AI,chat
 Author: Khalid Alrasheed
 Author-email: khalid@cycls.io
 Requires-Python: >=3.8,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: certifi (>=2023.11.17,<2024.0.0)
 Requires-Dist: httpx (>=0.25.2,<0.26.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-socketio[asyncio-client,client] (>=5.11.2,<6.0.0)
 Project-URL: Documentation, https://docs.cycls.com/
 Description-Content-Type: text/markdown
 
 <!-- 
 <p align="center">
 <img style="height: 75px;" src="https://www.sarya.com/img/logo.svg" alt="logo" />
```

