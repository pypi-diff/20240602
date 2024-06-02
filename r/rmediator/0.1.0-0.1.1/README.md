# Comparing `tmp/rmediator-0.1.0.tar.gz` & `tmp/rmediator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmediator-0.1.0.tar", last modified: Sat Jun  1 06:06:18 2024, max compression
+gzip compressed data, was "rmediator-0.1.1.tar", last modified: Sun Jun  2 08:36:03 2024, max compression
```

## Comparing `rmediator-0.1.0.tar` & `rmediator-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,35 @@
-drwxr-xr-x   0 ffekirnew   (502) staff       (20)        0 2024-06-01 06:06:18.128927 rmediator-0.1.0/
--rw-r--r--   0 ffekirnew   (502) staff       (20)     1073 2024-06-01 04:58:46.000000 rmediator-0.1.0/LICENSE
--rw-r--r--   0 ffekirnew   (502) staff       (20)       85 2024-06-01 05:08:15.000000 rmediator-0.1.0/MANIFEST.in
--rw-r--r--   0 ffekirnew   (502) staff       (20)     1325 2024-06-01 06:06:18.128870 rmediator-0.1.0/PKG-INFO
--rw-r--r--   0 ffekirnew   (502) staff       (20)       30 2024-06-01 04:58:46.000000 rmediator-0.1.0/README.md
--rw-r--r--   0 ffekirnew   (502) staff       (20)       98 2024-06-01 05:08:31.000000 rmediator-0.1.0/pyproject.toml
--rw-r--r--   0 ffekirnew   (502) staff       (20)      112 2024-06-01 06:06:18.129122 rmediator-0.1.0/setup.cfg
--rw-r--r--   0 ffekirnew   (502) staff       (20)     1964 2024-06-01 05:38:12.000000 rmediator-0.1.0/setup.py
-drwxr-xr-x   0 ffekirnew   (502) staff       (20)        0 2024-06-01 06:06:18.126002 rmediator-0.1.0/src/
-drwxr-xr-x   0 ffekirnew   (502) staff       (20)        0 2024-06-01 06:06:18.127642 rmediator-0.1.0/src/rmediator/
--rw-r--r--   0 ffekirnew   (502) staff       (20)       22 2024-06-01 05:07:34.000000 rmediator-0.1.0/src/rmediator/__init__.py
--rw-r--r--   0 ffekirnew   (502) staff       (20)     1310 2024-06-01 05:27:26.000000 rmediator-0.1.0/src/rmediator/decorators.py
--rw-r--r--   0 ffekirnew   (502) staff       (20)      472 2024-06-01 05:22:30.000000 rmediator-0.1.0/src/rmediator/interfaces.py
--rw-r--r--   0 ffekirnew   (502) staff       (20)     2088 2024-06-01 05:24:43.000000 rmediator-0.1.0/src/rmediator/mediator.py
-drwxr-xr-x   0 ffekirnew   (502) staff       (20)        0 2024-06-01 06:06:18.128580 rmediator-0.1.0/src/rmediator.egg-info/
--rw-r--r--   0 ffekirnew   (502) staff       (20)     1325 2024-06-01 06:06:18.000000 rmediator-0.1.0/src/rmediator.egg-info/PKG-INFO
--rw-r--r--   0 ffekirnew   (502) staff       (20)      355 2024-06-01 06:06:18.000000 rmediator-0.1.0/src/rmediator.egg-info/SOURCES.txt
--rw-r--r--   0 ffekirnew   (502) staff       (20)        1 2024-06-01 06:06:18.000000 rmediator-0.1.0/src/rmediator.egg-info/dependency_links.txt
--rw-r--r--   0 ffekirnew   (502) staff       (20)       22 2024-06-01 06:06:18.000000 rmediator-0.1.0/src/rmediator.egg-info/requires.txt
--rw-r--r--   0 ffekirnew   (502) staff       (20)       10 2024-06-01 06:06:18.000000 rmediator-0.1.0/src/rmediator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.764028 rmediator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 08:35:55.000000 rmediator-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 08:35:55.000000 rmediator-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-06-02 08:36:03.764028 rmediator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-02 08:35:55.000000 rmediator-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-02 08:35:55.000000 rmediator-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-02 08:36:03.764028 rmediator-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-06-02 08:35:55.000000 rmediator-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.756028 rmediator-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.760028 rmediator-0.1.1/src/rmediator/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.760028 rmediator-0.1.1/src/rmediator/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/decorators/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/decorators/request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.760028 rmediator-0.1.1/src/rmediator/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/interfaces/request_handler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/interfaces/request_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-06-02 08:35:55.000000 rmediator-0.1.1/src/rmediator/mediator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.764028 rmediator-0.1.1/src/rmediator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-06-02 08:36:03.000000 rmediator-0.1.1/src/rmediator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-06-02 08:36:03.000000 rmediator-0.1.1/src/rmediator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 08:36:03.000000 rmediator-0.1.1/src/rmediator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 08:36:03.000000 rmediator-0.1.1/src/rmediator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 08:36:03.000000 rmediator-0.1.1/src/rmediator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.756028 rmediator-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.760028 rmediator-0.1.1/tests/rmediator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.764028 rmediator-0.1.1/tests/rmediator/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-06-02 08:35:55.000000 rmediator-0.1.1/tests/rmediator/decorators/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-06-02 08:35:55.000000 rmediator-0.1.1/tests/rmediator/decorators/test_request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:36:03.764028 rmediator-0.1.1/tests/rmediator/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-06-02 08:35:55.000000 rmediator-0.1.1/tests/rmediator/interfaces/test_request_handler_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-06-02 08:35:55.000000 rmediator-0.1.1/tests/rmediator/interfaces/test_request_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 08:35:55.000000 rmediator-0.1.1/tests/rmediator/test_mediator.py
```

### Comparing `rmediator-0.1.0/LICENSE` & `rmediator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rmediator-0.1.0/setup.py` & `rmediator-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `rmediator-0.1.0/src/rmediator/decorators.py` & `rmediator-0.1.1/src/rmediator/decorators/request_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-from rmediator.interfaces import RequestHandlerInterface, RequestInterface
-from rmediator.mediator import Mediator
-
-
-def request(cls):
-    if not issubclass(cls, RequestInterface):
-        raise ValueError(
-            f"Request class cannot be registered, {cls} must be a subclass of RequestInterface."
-        )
-
-    if "response" not in cls.__dict__:
-        raise ValueError(
-            f"Request class cannot be registered, {cls} must contain attribute 'response' to signify the response expected for this request."
-        )
-
-    Mediator().register_request(cls)
-
-    return cls
+from src.rmediator import Mediator
+from src.rmediator.interfaces import RequestHandlerInterface
 
 
 def request_handler(cls):
     if not issubclass(cls, RequestHandlerInterface):
         raise ValueError(
             f"Request handler class cannot be registered, {cls} must be a subclass of RequestHandlerInterface."
         )
@@ -30,10 +14,28 @@
         )
 
     if "response" not in cls.__dict__:
         raise ValueError(
             f"Request handler class cannot be registered, {cls} must contain attribute 'response' to signify the response it sends after handling request."
         )
 
-    Mediator().register_handler(cls)
+    if cls.request == None:  # type: ignore
+        raise ValueError(
+            f"Request handler class cannot be registered, {cls} must contain attribute 'request' to signify the request it handles."
+        )
+
+    if cls.handle.__annotations__.get("request", None) != cls.request:  # type: ignore
+        raise ValueError(
+            f"Request handler class cannot be registered, {cls} handle method must have 'request' parameter of type {cls.request}."  # type: ignore
+        )
+
+    if cls.handle.__annotations__.get("return", None) != cls.response:  # type: ignore
+        raise ValueError(
+            f"Request handler class cannot be registered, {cls} handle method must have return type of {cls.response}."  # type: ignore
+        )
+
+    try:
+        Mediator().register_handler(cls)
+    except ValueError as e:
+        raise e
 
     return cls
```

### Comparing `rmediator-0.1.0/src/rmediator/mediator.py` & `rmediator-0.1.1/src/rmediator/mediator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from threading import Lock
+from typing import Any
 
-from rmediator.interfaces import RequestHandlerInterface, RequestInterface
+from src.rmediator.interfaces import RequestHandlerInterface, RequestInterface
 
 
 class SingletonMeta(type):
     _instances = {}
     _lock: Lock = Lock()
 
     def __call__(cls, *args, **kwargs):
@@ -12,48 +13,46 @@
             if cls not in cls._instances:
                 instance = super().__call__(*args, **kwargs)
                 cls._instances[cls] = instance
         return cls._instances[cls]
 
 
 class Mediator(metaclass=SingletonMeta):
-    _instance = None
-
     def __init__(self) -> None:
-        self.requests = {}
-        self.request_handlers = {}
+        self.__requests = {}
+        self.__request_handlers = {}
 
-    def send(self, request: RequestInterface) -> RequestInterface.response:  # type: ignore
-        if type(request) not in self.requests:
+    def send(self, request: RequestInterface) -> Any:
+        if type(request) not in self.__requests:
             raise ValueError(
                 f"Request cannot be handled, Request {type(request)} not registered."
             )
 
-        handler = self.request_handlers.get(type(request))
+        handler = self.__request_handlers.get(type(request))
         if not handler:
             raise ValueError(
                 f"Request cannot be handled, No handler has been registered for {type(request)}."
             )
 
         return handler.handle(request)
 
     def register_request(self, request: type[RequestInterface]) -> None:
-        self.requests[request] = request.response  # type: ignore
+        self.__requests[request] = request.response  # type: ignore
 
     def register_handler(self, handler: type[RequestHandlerInterface]) -> None:
         request, response = handler.request, handler.response  # type: ignore
-        if request not in self.requests:
+        if request not in self.__requests:
             raise ValueError(
                 f"Handler cannot be registered, Request {request} has been not registered."
             )
 
-        if response != self.requests[request]:
+        if response != self.__requests[request]:
             raise ValueError(
-                f"Handler cannot be registered, Handler response {response} does not match request response {self.requests[request]}."
+                f"Handler cannot be registered, Handler response {response} does not match request response {self.__requests[request]}."
             )
 
-        if request in self.request_handlers:
+        if request in self.__request_handlers:
             raise ValueError(
                 f"Handler cannot be registered, Another handler for request type {request} has already been registered."
             )
 
-        self.request_handlers[request] = handler()
+        self.__request_handlers[request] = handler()
```

