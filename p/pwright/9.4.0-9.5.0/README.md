# Comparing `tmp/pwright-9.4.0.tar.gz` & `tmp/pwright-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwright-9.4.0.tar", last modified: Sun Apr 21 08:33:09 2024, max compression
+gzip compressed data, was "pwright-9.5.0.tar", last modified: Sun Jun  2 16:28:54 2024, max compression
```

## Comparing `pwright-9.4.0.tar` & `pwright-9.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1229 2024-04-21 08:33:09.357124 pwright-9.4.0/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-21 08:32:57.749056 pwright-9.4.0/src/pwright/__init__.py
--rw-r--r--   0        0        0       18 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/__version__.py
--rw-r--r--   0        0        0      575 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/_utils.py
--rw-r--r--   0        0        0     1466 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/async_api/__init__.py
--rw-r--r--   0        0        0      793 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/async_api/_apis.py
--rw-r--r--   0        0        0     2169 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/async_api/_briefs.py
--rw-r--r--   0        0        0     4904 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/async_api/_cms.py
--rw-r--r--   0        0        0      608 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/async_api/_compatibilities.py
--rw-r--r--   0        0        0      908 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/async_api/utils.py
--rw-r--r--   0        0        0      260 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/constants.py
--rw-r--r--   0        0        0     1161 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/sync_api/__init__.py
--rw-r--r--   0        0        0      779 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/sync_api/_apis.py
--rw-r--r--   0        0        0     2115 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/sync_api/_briefs.py
--rw-r--r--   0        0        0     4794 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/sync_api/_cms.py
--rw-r--r--   0        0        0      860 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/sync_api/utils.py
--rw-r--r--   0        0        0      541 2024-04-21 08:32:57.753056 pwright-9.4.0/src/pwright/typealiases.py
--rw-r--r--   0        0        0        0 2024-04-21 08:32:57.753056 pwright-9.4.0/tests/__init__.py
--rw-r--r--   0        0        0      126 2024-04-21 08:32:57.753056 pwright-9.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1635 2024-04-21 08:32:57.753056 pwright-9.4.0/tests/test_apw.py
--rw-r--r--   0        0        0     1387 2024-04-21 08:32:57.753056 pwright-9.4.0/tests/test_pw.py
--rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-9.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1229 2024-06-02 16:28:54.825593 pwright-9.5.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/__init__.py
+-rw-r--r--   0        0        0       18 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/__version__.py
+-rw-r--r--   0        0        0      575 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/_utils.py
+-rw-r--r--   0        0        0     1500 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/async_api/__init__.py
+-rw-r--r--   0        0        0      841 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/async_api/_apis.py
+-rw-r--r--   0        0        0     2169 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/async_api/_briefs.py
+-rw-r--r--   0        0        0     4904 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/async_api/_cms.py
+-rw-r--r--   0        0        0      608 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/async_api/_compatibilities.py
+-rw-r--r--   0        0        0      908 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/async_api/utils.py
+-rw-r--r--   0        0        0      260 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/constants.py
+-rw-r--r--   0        0        0     1195 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      826 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/sync_api/_apis.py
+-rw-r--r--   0        0        0     2115 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/sync_api/_briefs.py
+-rw-r--r--   0        0        0     4794 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/sync_api/_cms.py
+-rw-r--r--   0        0        0      860 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/sync_api/utils.py
+-rw-r--r--   0        0        0      541 2024-06-02 16:28:42.329568 pwright-9.5.0/src/pwright/typealiases.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:28:42.329568 pwright-9.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      126 2024-06-02 16:28:42.329568 pwright-9.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1635 2024-06-02 16:28:42.333568 pwright-9.5.0/tests/test_apw.py
+-rw-r--r--   0        0        0     1387 2024-06-02 16:28:42.333568 pwright-9.5.0/tests/test_pw.py
+-rw-r--r--   0        0        0      108 1970-01-01 00:00:00.000000 pwright-9.5.0/PKG-INFO
```

### Comparing `pwright-9.4.0/pyproject.toml` & `pwright-9.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pwright"
-version = "9.4.0"
+version = "9.5.0"
 requires-python = ">=3.8"
 dependencies = [
     "playwright>=1.34.0",
 ]
 
 [tool.pdm]
 distribution = true
```

### Comparing `pwright-9.4.0/src/pwright/_utils.py` & `pwright-9.5.0/src/pwright/_utils.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/async_api/__init__.py` & `pwright-9.5.0/src/pwright/async_api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ..typealiases import (
     AsyncGeneratorContextManagerAsyncGenerator as AsyncGeneratorContextManagerAsyncGenerator,
 )
 from ._apis import Browser as Browser
 from ._apis import BrowserContext as BrowserContext
 from ._apis import Dialog as Dialog
 from ._apis import ElementHandle as ElementHandle
+from ._apis import Error as Error
 from ._apis import FrameLocator as FrameLocator
 from ._apis import Locator as Locator
 from ._apis import Page as Page
 from ._apis import Playwright as Playwright
 from ._apis import Route as Route
 from ._apis import TimeoutError as TimeoutError
 from ._apis import playwright as playwright
```

### Comparing `pwright-9.4.0/src/pwright/async_api/_apis.py` & `pwright-9.5.0/src/pwright/async_api/_apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from playwright.async_api import Browser as Browser
 from playwright.async_api import BrowserContext as BrowserContext
 from playwright.async_api import BrowserType as BrowserType
 from playwright.async_api import Dialog as Dialog
 from playwright.async_api import ElementHandle as ElementHandle
+from playwright.async_api import Error as Error
 from playwright.async_api import FrameLocator as FrameLocator
 from playwright.async_api import Locator as Locator
 from playwright.async_api import Page as Page
 from playwright.async_api import Playwright as Playwright
 from playwright.async_api import ProxySettings as ProxySettings
 from playwright.async_api import Route as Route
 from playwright.async_api import TimeoutError as TimeoutError
```

### Comparing `pwright-9.4.0/src/pwright/async_api/_briefs.py` & `pwright-9.5.0/src/pwright/async_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/async_api/_cms.py` & `pwright-9.5.0/src/pwright/async_api/_cms.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/async_api/_compatibilities.py` & `pwright-9.5.0/src/pwright/async_api/_compatibilities.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/async_api/utils.py` & `pwright-9.5.0/src/pwright/async_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/sync_api/__init__.py` & `pwright-9.5.0/src/pwright/sync_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ..typealiases import Generator as Generator
 from ..typealiases import GeneratorContextManager as GeneratorContextManager
 from ..typealiases import GeneratorContextManagerGenerator as GeneratorContextManagerGenerator
 from ._apis import Browser as Browser
 from ._apis import BrowserContext as BrowserContext
 from ._apis import Dialog as Dialog
 from ._apis import ElementHandle as ElementHandle
+from ._apis import Error as Error
 from ._apis import FrameLocator as FrameLocator
 from ._apis import Locator as Locator
 from ._apis import Page as Page
 from ._apis import Playwright as Playwright
 from ._apis import Route as Route
 from ._apis import TimeoutError as TimeoutError
 from ._apis import playwright as playwright
```

### Comparing `pwright-9.4.0/src/pwright/sync_api/_apis.py` & `pwright-9.5.0/src/pwright/sync_api/_apis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from playwright.sync_api import Browser as Browser
 from playwright.sync_api import BrowserContext as BrowserContext
 from playwright.sync_api import BrowserType as BrowserType
 from playwright.sync_api import Dialog as Dialog
 from playwright.sync_api import ElementHandle as ElementHandle
+from playwright.sync_api import Error as Error
 from playwright.sync_api import FrameLocator as FrameLocator
 from playwright.sync_api import Locator as Locator
 from playwright.sync_api import Page as Page
 from playwright.sync_api import Playwright as Playwright
 from playwright.sync_api import ProxySettings as ProxySettings
 from playwright.sync_api import Route as Route
 from playwright.sync_api import TimeoutError as TimeoutError
```

### Comparing `pwright-9.4.0/src/pwright/sync_api/_briefs.py` & `pwright-9.5.0/src/pwright/sync_api/_briefs.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/sync_api/_cms.py` & `pwright-9.5.0/src/pwright/sync_api/_cms.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/sync_api/utils.py` & `pwright-9.5.0/src/pwright/sync_api/utils.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/src/pwright/typealiases.py` & `pwright-9.5.0/src/pwright/typealiases.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/tests/test_apw.py` & `pwright-9.5.0/tests/test_apw.py`

 * *Files identical despite different names*

### Comparing `pwright-9.4.0/tests/test_pw.py` & `pwright-9.5.0/tests/test_pw.py`

 * *Files identical despite different names*

