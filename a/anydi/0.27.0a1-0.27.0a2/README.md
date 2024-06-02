# Comparing `tmp/anydi-0.27.0a1.tar.gz` & `tmp/anydi-0.27.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.27.0a1.tar", max compression
+gzip compressed data, was "anydi-0.27.0a2.tar", max compression
```

## Comparing `anydi-0.27.0a1.tar` & `anydi-0.27.0a2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.27.0a1/LICENSE
--rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.27.0a1/README.md
--rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.27.0a1/anydi/__init__.py
--rw-r--r--   0        0        0    29631 2024-06-02 08:09:38.663093 anydi-0.27.0a1/anydi/_container.py
--rw-r--r--   0        0        0    10815 2024-05-28 05:51:36.811241 anydi-0.27.0a1/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.27.0a1/anydi/_logger.py
--rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.27.0a1/anydi/_module.py
--rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.27.0a1/anydi/_scanner.py
--rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.27.0a1/anydi/_types.py
--rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.27.0a1/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.27.0a1/anydi/ext/__init__.py
--rw-r--r--   0        0        0     2691 2024-06-02 08:09:32.972178 anydi-0.27.0a1/anydi/ext/_utils.py
--rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.27.0a1/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.27.0a1/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.27.0a1/anydi/ext/django/_settings.py
--rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.27.0a1/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.27.0a1/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.27.0a1/anydi/ext/django/middleware.py
--rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.27.0a1/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.27.0a1/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.27.0a1/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     2896 2024-06-02 08:09:32.972674 anydi-0.27.0a1/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     1617 2024-06-02 08:09:32.972836 anydi-0.27.0a1/anydi/ext/faststream.py
--rw-r--r--   0        0        0     4477 2024-06-02 08:09:38.664067 anydi-0.27.0a1/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.27.0a1/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.27.0a1/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.27.0a1/anydi/py.typed
--rw-r--r--   0        0        0     3132 2024-06-02 08:10:57.220094 anydi-0.27.0a1/pyproject.toml
--rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 anydi-0.27.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.27.0a2/LICENSE
+-rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.27.0a2/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.27.0a2/anydi/__init__.py
+-rw-r--r--   0        0        0    29631 2024-06-02 14:15:07.268714 anydi-0.27.0a2/anydi/_container.py
+-rw-r--r--   0        0        0    10815 2024-05-28 05:51:36.811241 anydi-0.27.0a2/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.27.0a2/anydi/_logger.py
+-rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.27.0a2/anydi/_module.py
+-rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.27.0a2/anydi/_scanner.py
+-rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.27.0a2/anydi/_types.py
+-rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.27.0a2/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.27.0a2/anydi/ext/__init__.py
+-rw-r--r--   0        0        0     2691 2024-06-02 14:18:27.849442 anydi-0.27.0a2/anydi/ext/_utils.py
+-rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.27.0a2/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.27.0a2/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.27.0a2/anydi/ext/django/_settings.py
+-rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.27.0a2/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.27.0a2/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.27.0a2/anydi/ext/django/middleware.py
+-rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.27.0a2/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.27.0a2/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.27.0a2/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     2896 2024-06-02 14:18:27.850113 anydi-0.27.0a2/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     1617 2024-06-02 14:18:27.850277 anydi-0.27.0a2/anydi/ext/faststream.py
+-rw-r--r--   0        0        0     4242 2024-06-02 14:18:33.987372 anydi-0.27.0a2/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.27.0a2/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.27.0a2/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.27.0a2/anydi/py.typed
+-rw-r--r--   0        0        0     3133 2024-06-02 14:23:12.810713 anydi-0.27.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 anydi-0.27.0a2/PKG-INFO
```

### Comparing `anydi-0.27.0a1/LICENSE` & `anydi-0.27.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/README.md` & `anydi-0.27.0a2/README.md`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/__init__.py` & `anydi-0.27.0a2/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/_container.py` & `anydi-0.27.0a2/anydi/_container.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/_context.py` & `anydi-0.27.0a2/anydi/_context.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/_module.py` & `anydi-0.27.0a2/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/_scanner.py` & `anydi-0.27.0a2/anydi/_scanner.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/_types.py` & `anydi-0.27.0a2/anydi/_types.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/_utils.py` & `anydi-0.27.0a2/anydi/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/_utils.py` & `anydi-0.27.0a2/anydi/ext/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/django/_settings.py` & `anydi-0.27.0a2/anydi/ext/django/_settings.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/django/_utils.py` & `anydi-0.27.0a2/anydi/ext/django/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/django/apps.py` & `anydi-0.27.0a2/anydi/ext/django/apps.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/django/middleware.py` & `anydi-0.27.0a2/anydi/ext/django/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/django/ninja/__init__.py` & `anydi-0.27.0a2/anydi/ext/django/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/django/ninja/_operation.py` & `anydi-0.27.0a2/anydi/ext/django/ninja/_operation.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/django/ninja/_signature.py` & `anydi-0.27.0a2/anydi/ext/django/ninja/_signature.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/fastapi.py` & `anydi-0.27.0a2/anydi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/faststream.py` & `anydi-0.27.0a2/anydi/ext/faststream.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/anydi/ext/pytest_plugin.py` & `anydi-0.27.0a2/anydi/ext/pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import inspect
 from typing import Any, Callable, Iterator, cast
 
 import pytest
 
 from anydi import Container
-from anydi._types import is_marker
 from anydi._utils import get_typed_parameters
 
 
 def pytest_configure(config: pytest.Config) -> None:
     config.addinivalue_line(
         "markers",
         "inject: mark test as needing dependency injection",
@@ -20,20 +19,14 @@
 def pytest_addoption(parser: pytest.Parser) -> None:
     parser.addini(
         "anydi_inject_all",
         help="Inject all dependencies",
         type="bool",
         default=False,
     )
-    parser.addini(
-        "anydi_inject_auto",
-        help="Automatically inject dependencies",
-        type="bool",
-        default=True,
-    )
 
 
 CONTAINER_FIXTURE_NAME = "container"
 
 
 @pytest.fixture
 def anydi_setup_container(
@@ -67,25 +60,23 @@
 
 @pytest.fixture
 def _anydi_injected_parameter_iterator(
     request: pytest.FixtureRequest,
     _anydi_unresolved: list[str],
 ) -> Callable[[], Iterator[tuple[str, Any]]]:
     registered_fixtures = request.session._fixturemanager._arg2fixturedefs  # noqa
-    inject_auto = cast(bool, request.config.getini("anydi_inject_auto"))
 
     def _iterator() -> Iterator[tuple[str, inspect.Parameter]]:
         for parameter in get_typed_parameters(request.function):
             interface = parameter.annotation
-            if interface is parameter.empty:
-                continue
-            if not inject_auto and is_marker(parameter.default):
-                yield parameter.name, interface
-                continue
-            if interface in _anydi_unresolved or parameter.name in registered_fixtures:
+            if (
+                interface is parameter.empty
+                or interface in _anydi_unresolved
+                or parameter.name in registered_fixtures
+            ):
                 continue
             yield parameter.name, interface
 
     return _iterator
 
 
 @pytest.fixture(autouse=True)
@@ -100,25 +91,26 @@
     if inspect.iscoroutinefunction(request.function) or not _anydi_should_inject:
         return
 
     # Setup the container
     container = cast(Container, request.getfixturevalue("anydi_setup_container"))
 
     for argname, interface in _anydi_injected_parameter_iterator():
+        # Skip if the interface is not registered
+        if container.strict and not container.is_registered(interface):
+            continue
+
         # Release the instance if it was already resolved
         if container.is_resolved(interface):
             container.release(interface)
 
         try:
-            # Resolve the instance
-            instance = container.resolve(interface)
-        except LookupError:
+            request.node.funcargs[argname] = container.resolve(interface)
+        except Exception:  # noqa
             _anydi_unresolved.append(interface)
-            continue
-        request.node.funcargs[argname] = instance
 
 
 @pytest.fixture(autouse=True)
 async def _anydi_ainject(
     request: pytest.FixtureRequest,
     _anydi_should_inject: bool,
     _anydi_injected_parameter_iterator: Callable[[], Iterator[tuple[str, Any]]],
@@ -128,18 +120,19 @@
     if not inspect.iscoroutinefunction(request.function) or not _anydi_should_inject:
         return
 
     # Setup the container
     container = cast(Container, request.getfixturevalue("anydi_setup_container"))
 
     for argname, interface in _anydi_injected_parameter_iterator():
+        # Skip if the interface is not registered
+        if container.strict and not container.is_registered(interface):
+            continue
+
         # Release the instance if it was already resolved
         if container.is_resolved(interface):
             container.release(interface)
 
         try:
-            # Resolve the instance
-            instance = await container.aresolve(interface)
-        except LookupError:
+            request.node.funcargs[argname] = await container.aresolve(interface)
+        except Exception:  # noqa
             _anydi_unresolved.append(interface)
-            continue
-        request.node.funcargs[argname] = instance
```

### Comparing `anydi-0.27.0a1/anydi/ext/starlette/middleware.py` & `anydi-0.27.0a2/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.27.0a1/pyproject.toml` & `anydi-0.27.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.27.0a1"
+version = "0.27.0a2"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
@@ -32,18 +32,18 @@
 ]
 packages = [
     { include = "anydi", from = "." },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-typing-extensions = "^4.8.0"
+typing-extensions = "^4.12.1"
 anyio = { version = "^3.6.2", optional = true }
 mkdocs = { version = "^1.4.2", optional = true }
-mkdocs-material = { version = "^9.1.13", optional = true }
+mkdocs-material = { version = "^9.5.21", optional = true }
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-material"]
 async = ["anyio"]
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.10.0"
```

### Comparing `anydi-0.27.0a1/PKG-INFO` & `anydi-0.27.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.27.0a1
+Version: 0.27.0a2
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -29,16 +29,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: async
 Provides-Extra: docs
 Requires-Dist: anyio (>=3.6.2,<4.0.0) ; extra == "async"
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "docs"
-Requires-Dist: mkdocs-material (>=9.1.13,<10.0.0) ; extra == "docs"
-Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
+Requires-Dist: mkdocs-material (>=9.5.21,<10.0.0) ; extra == "docs"
+Requires-Dist: typing-extensions (>=4.12.1,<5.0.0)
 Project-URL: Repository, https://github.com/antonrh/anydi
 Description-Content-Type: text/markdown
 
 # AnyDI
 
 <p align="center">
     <i>Modern, lightweight Dependency Injection library using type annotations.</i>
```
