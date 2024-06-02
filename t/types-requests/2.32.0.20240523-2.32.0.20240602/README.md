# Comparing `tmp/types-requests-2.32.0.20240523.tar.gz` & `tmp/types-requests-2.32.0.20240602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-requests-2.32.0.20240523.tar", last modified: Thu May 23 02:21:57 2024, max compression
+gzip compressed data, was "types-requests-2.32.0.20240602.tar", last modified: Sun Jun  2 02:27:07 2024, max compression
```

## Comparing `types-requests-2.32.0.20240523.tar` & `types-requests-2.32.0.20240602.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:57.986203 types-requests-2.32.0.20240523/
--rw-r--r--   0 runner    (1001) docker     (127)    15819 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-23 02:21:57.982203 types-requests-2.32.0.20240523/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:57.982203 types-requests-2.32.0.20240523/requests-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/requests-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/adapters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/certs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/help.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/packages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/requests-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/status_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/structures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-23 02:21:41.000000 types-requests-2.32.0.20240523/requests-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 02:21:57.986203 types-requests-2.32.0.20240523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 02:21:57.982203 types-requests-2.32.0.20240523/types_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/types_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/types_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/types_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/types_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 02:21:57.000000 types-requests-2.32.0.20240523/types_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:07.501568 types-requests-2.32.0.20240602/
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-06-02 02:27:06.000000 types-requests-2.32.0.20240602/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 02:27:06.000000 types-requests-2.32.0.20240602/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-06-02 02:27:07.501568 types-requests-2.32.0.20240602/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:07.501568 types-requests-2.32.0.20240602/requests-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 02:27:06.000000 types-requests-2.32.0.20240602/requests-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/certs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/help.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/packages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:06.000000 types-requests-2.32.0.20240602/requests-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/status_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/structures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-06-02 02:26:49.000000 types-requests-2.32.0.20240602/requests-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 02:27:07.501568 types-requests-2.32.0.20240602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-02 02:27:06.000000 types-requests-2.32.0.20240602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:07.501568 types-requests-2.32.0.20240602/types_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-06-02 02:27:07.000000 types-requests-2.32.0.20240602/types_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-06-02 02:27:07.000000 types-requests-2.32.0.20240602/types_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 02:27:07.000000 types-requests-2.32.0.20240602/types_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 02:27:07.000000 types-requests-2.32.0.20240602/types_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 02:27:07.000000 types-requests-2.32.0.20240602/types_requests.egg-info/top_level.txt
```

### Comparing `types-requests-2.32.0.20240523/CHANGELOG.md` & `types-requests-2.32.0.20240602/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.32.0.20240602 (2024-06-02)
+
+[requests] Update to 2.32.3 (#12060)
+
 ## 2.32.0.20240523 (2024-05-23)
 
 [requests] Update to 2.32.2 (#12000)
 
 Also replace some `Any` annotations with `Incomplete` and use `Final` in `requests.__version__`.
 
 ## 2.32.0.20240521 (2024-05-21)
```

### Comparing `types-requests-2.32.0.20240523/PKG-INFO` & `types-requests-2.32.0.20240602/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.32.0.20240523
+Version: 2.32.0.20240602
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `e285e52e1385a3c63a850dd5a2e8b2c744d7293a` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

### Comparing `types-requests-2.32.0.20240523/requests-stubs/__init__.pyi` & `types-requests-2.32.0.20240602/requests-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/adapters.pyi` & `types-requests-2.32.0.20240602/requests-stubs/adapters.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from _typeshed import Incomplete
 from collections.abc import Mapping
-from typing_extensions import deprecated
+from ssl import SSLContext
+from typing import Literal, TypedDict
+from typing_extensions import NotRequired, deprecated
 
+import urllib3
 from urllib3.connectionpool import ConnectionPool
 from urllib3.contrib.socks import SOCKSProxyManager as SOCKSProxyManager
 from urllib3.exceptions import (
     ConnectTimeoutError as ConnectTimeoutError,
     MaxRetryError as MaxRetryError,
     ProtocolError as ProtocolError,
     ReadTimeoutError as ReadTimeoutError,
@@ -30,14 +33,28 @@
     _Uri,
     get_auth_from_url as get_auth_from_url,
     get_encoding_from_headers as get_encoding_from_headers,
     prepend_scheme_if_needed as prepend_scheme_if_needed,
     urldefragauth as urldefragauth,
 )
 
+# Arguments to urllib3 connection_from_host() functions (except pool_kwargs).
+class _HostParams(TypedDict):
+    host: str
+    scheme: str
+    port: int
+
+class _PoolKwargs(TypedDict):
+    ssl_context: NotRequired[SSLContext]
+    ca_certs: NotRequired[str]
+    ca_cert_dir: NotRequired[str]
+    cert_reqs: Literal["CERT_REQUIRED", "CERT_NONE"]
+    cert_file: NotRequired[str]
+    key_file: NotRequired[str]
+
 DEFAULT_POOLBLOCK: bool
 DEFAULT_POOLSIZE: int
 DEFAULT_RETRIES: int
 DEFAULT_POOL_TIMEOUT: float | None
 
 class BaseAdapter:
     def __init__(self) -> None: ...
@@ -60,15 +77,18 @@
     def __init__(
         self, pool_connections: int = 10, pool_maxsize: int = 10, max_retries: Retry | int | None = 0, pool_block: bool = False
     ) -> None: ...
     poolmanager: Incomplete
     def init_poolmanager(self, connections, maxsize, block=False, **pool_kwargs): ...
     def proxy_manager_for(self, proxy, **proxy_kwargs): ...
     def cert_verify(self, conn, url, verify, cert): ...
-    def build_response(self, req, resp): ...
+    def build_response(self, req: PreparedRequest, resp: urllib3.BaseHTTPResponse) -> Response: ...
+    def build_connection_pool_key_attributes(
+        self, request: PreparedRequest, verify: bool | str, cert: str | tuple[str, str] | None = None
+    ) -> tuple[_HostParams, _PoolKwargs]: ...
     def get_connection_with_tls_context(
         self,
         request: PreparedRequest,
         verify: bool | str | None,
         proxies: Mapping[str, str] | None = None,
         cert: tuple[str, str] | str | None = None,
     ) -> ConnectionPool: ...
```

### Comparing `types-requests-2.32.0.20240523/requests-stubs/api.pyi` & `types-requests-2.32.0.20240602/requests-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/auth.pyi` & `types-requests-2.32.0.20240602/requests-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/compat.pyi` & `types-requests-2.32.0.20240602/requests-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/cookies.pyi` & `types-requests-2.32.0.20240602/requests-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/exceptions.pyi` & `types-requests-2.32.0.20240602/requests-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/help.pyi` & `types-requests-2.32.0.20240602/requests-stubs/help.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/models.pyi` & `types-requests-2.32.0.20240602/requests-stubs/models.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from _typeshed import Unused
+from _typeshed import Incomplete, Unused
 from collections.abc import Callable, Iterator
 from json import JSONDecoder
 from typing import Any
 from typing_extensions import Self
 
 from urllib3 import exceptions as urllib3_exceptions, fields, filepost, util
 
@@ -37,38 +37,38 @@
 parse_header_links = utils.parse_header_links
 iter_slices = utils.iter_slices
 guess_json_utf = utils.guess_json_utf
 super_len = utils.super_len
 to_native_string = utils.to_native_string
 codes = status_codes.codes
 
-REDIRECT_STATI: Any
-DEFAULT_REDIRECT_LIMIT: Any
-CONTENT_CHUNK_SIZE: Any
-ITER_CHUNK_SIZE: Any
+REDIRECT_STATI: Incomplete
+DEFAULT_REDIRECT_LIMIT: Incomplete
+CONTENT_CHUNK_SIZE: Incomplete
+ITER_CHUNK_SIZE: Incomplete
 
 class RequestEncodingMixin:
     @property
     def path_url(self) -> str: ...
 
 class RequestHooksMixin:
     def register_hook(self, event, hook): ...
     def deregister_hook(self, event, hook): ...
 
 class Request(RequestHooksMixin):
-    hooks: Any
-    method: Any
-    url: Any
-    headers: Any
-    files: Any
-    data: Any
-    json: Any
-    params: Any
-    auth: Any
-    cookies: Any
+    hooks: Incomplete
+    method: Incomplete
+    url: Incomplete
+    headers: Incomplete
+    files: Incomplete
+    data: Incomplete
+    json: Incomplete
+    params: Incomplete
+    auth: Incomplete
+    cookies: Incomplete
     def __init__(
         self,
         method=None,
         url=None,
         headers=None,
         files=None,
         data=None,
@@ -81,15 +81,15 @@
     def prepare(self) -> PreparedRequest: ...
 
 class PreparedRequest(RequestEncodingMixin, RequestHooksMixin):
     method: str | None
     url: str | None
     headers: CaseInsensitiveDict[str]
     body: bytes | str | None
-    hooks: Any
+    hooks: Incomplete
     def __init__(self) -> None: ...
     def prepare(
         self,
         method=None,
         url=None,
         headers=None,
         files=None,
@@ -107,19 +107,19 @@
     def prepare_body(self, data, files, json=None) -> None: ...
     def prepare_content_length(self, body: bytes | str | None) -> None: ...
     def prepare_auth(self, auth, url="") -> None: ...
     def prepare_cookies(self, cookies) -> None: ...
     def prepare_hooks(self, hooks) -> None: ...
 
 class Response:
-    __attrs__: Any
+    __attrs__: Incomplete
     _content: bytes | None  # undocumented
     status_code: int
     headers: CaseInsensitiveDict[str]
-    raw: Any
+    raw: Incomplete
     url: str
     encoding: str | None
     history: list[Response]
     reason: str
     cookies: RequestsCookieJar
     elapsed: datetime.timedelta
     request: PreparedRequest
@@ -135,18 +135,18 @@
     def ok(self) -> bool: ...
     @property
     def is_redirect(self) -> bool: ...
     @property
     def is_permanent_redirect(self) -> bool: ...
     @property
     def apparent_encoding(self) -> str: ...
-    def iter_content(self, chunk_size: int | None = 1, decode_unicode: bool = False) -> Iterator[Any]: ...
+    def iter_content(self, chunk_size: int | None = 1, decode_unicode: bool = False) -> Iterator[Incomplete]: ...
     def iter_lines(
         self, chunk_size: int | None = 512, decode_unicode: bool = False, delimiter: str | bytes | None = None
-    ) -> Iterator[Any]: ...
+    ) -> Iterator[Incomplete]: ...
     @property
     def content(self) -> bytes: ...
     @property
     def text(self) -> str: ...
     def json(
         self,
         *,
@@ -155,10 +155,10 @@
         parse_float: Callable[[str], Any] | None = ...,
         parse_int: Callable[[str], Any] | None = ...,
         parse_constant: Callable[[str], Any] | None = ...,
         object_pairs_hook: Callable[[list[tuple[Any, Any]]], Any] | None = ...,
         **kwds: Any,
     ) -> Any: ...
     @property
-    def links(self) -> dict[Any, Any]: ...
+    def links(self) -> dict[Incomplete, Incomplete]: ...
     def raise_for_status(self) -> None: ...
     def close(self) -> None: ...
```

### Comparing `types-requests-2.32.0.20240523/requests-stubs/sessions.pyi` & `types-requests-2.32.0.20240602/requests-stubs/sessions.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/structures.pyi` & `types-requests-2.32.0.20240602/requests-stubs/structures.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/requests-stubs/utils.pyi` & `types-requests-2.32.0.20240602/requests-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.32.0.20240523/setup.py` & `types-requests-2.32.0.20240602/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `e285e52e1385a3c63a850dd5a2e8b2c744d7293a` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.32.0.20240523",
+      version="2.32.0.20240602",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md",
```

### Comparing `types-requests-2.32.0.20240523/types_requests.egg-info/PKG-INFO` & `types-requests-2.32.0.20240602/types_requests.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.32.0.20240523
+Version: 2.32.0.20240602
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f7c03486ee01c8ea74823db75e017341bf3c2ad0` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `e285e52e1385a3c63a850dd5a2e8b2c744d7293a` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

### Comparing `types-requests-2.32.0.20240523/types_requests.egg-info/SOURCES.txt` & `types-requests-2.32.0.20240602/types_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

