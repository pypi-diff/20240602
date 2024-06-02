# Comparing `tmp/scim2_client-0.1.0.tar.gz` & `tmp/scim2_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim2_client-0.1.0.tar", max compression
+gzip compressed data, was "scim2_client-0.1.1.tar", max compression
```

## Comparing `scim2_client-0.1.0.tar` & `scim2_client-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1622 2024-06-01 18:36:39.643124 scim2_client-0.1.0/README.md
--rw-r--r--   0        0        0     2491 2024-06-01 18:37:08.953520 scim2_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      338 2024-06-01 18:36:39.646458 scim2_client-0.1.0/scim2_client/__init__.py
--rw-r--r--   0        0        0    12635 2024-06-01 18:36:39.646458 scim2_client-0.1.0/scim2_client/client.py
--rw-r--r--   0        0        0     1175 2024-06-01 18:36:39.646458 scim2_client-0.1.0/scim2_client/errors.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 scim2_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1674 2024-06-01 19:35:02.108808 scim2_client-0.1.1/README.md
+-rw-r--r--   0        0        0     2491 2024-06-01 20:29:46.814362 scim2_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      338 2024-06-01 18:36:39.646458 scim2_client-0.1.1/scim2_client/__init__.py
+-rw-r--r--   0        0        0    13199 2024-06-01 20:29:55.831143 scim2_client-0.1.1/scim2_client/client.py
+-rw-r--r--   0        0        0     1175 2024-06-01 18:36:39.646458 scim2_client-0.1.1/scim2_client/errors.py
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 scim2_client-0.1.1/PKG-INFO
```

### Comparing `scim2_client-0.1.0/README.md` & `scim2_client-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # scim2-client
 
-A SCIM client library built upon [scim2-models](https://scim2-models.readthedocs.io), that pythonically build requests and parse responses, following the [RFC7643](https://datatracker.ietf.org/doc/html/rfc7643.html) and [RFC7644](https://datatracker.ietf.org/doc/html/rfc7644.html) specifications.
+A SCIM client Python library built upon [scim2-models](https://scim2-models.readthedocs.io) and [httpx](https://github.com/encode/httpx),
+that pythonically build requests and parse responses,
+following the [RFC7643](https://datatracker.ietf.org/doc/html/rfc7643.html) and [RFC7644](https://datatracker.ietf.org/doc/html/rfc7644.html) specifications.
 ## Installation
 
 ```shell
 pip install scim2-client
 ```
 
 ## Usage
```

### Comparing `scim2_client-0.1.0/pyproject.toml` & `scim2_client-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scim2-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pythonically build SCIM requests and parse SCIM responses"
 authors = ["Yaal Coop <contact@yaal.coop>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["scim", "scim2", "provisioning", "httpx", "api"]
 classifiers = [
     "Intended Audience :: Developers",
@@ -23,15 +23,15 @@
     "Programming Language :: Python",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.27.0"
-scim2-models = "^0.1.0"
+scim2-models = "^0.1.1"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.1"
 pytest-coverage = "^0.0"
```

### Comparing `scim2_client-0.1.0/scim2_client/client.py` & `scim2_client-0.1.1/scim2_client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Type
 from typing import Union
 
 from httpx import Client
 from httpx import Response
 from pydantic import ValidationError
 from scim2_models import AnyResource
+from scim2_models import Context
 from scim2_models import Error
 from scim2_models import ListResponse
 from scim2_models import PatchOp
 from scim2_models import SearchRequest
 
 from .errors import UnexpectedContentFormat
 from .errors import UnexpectedContentType
@@ -40,14 +41,15 @@
         return f"/{resource_type.__name__}s"
 
     def check_response(
         self,
         response: Response,
         expected_status_codes: List[int],
         expected_type: Optional[Type] = None,
+        scim_ctx: Optional[Context] = None,
     ):
         if response.status_code not in expected_status_codes:
             raise UnexpectedStatusCode(response)
 
         # Interoperability considerations:  The "application/scim+json" media
         # type is intended to identify JSON structure data that conforms to
         # the SCIM protocol and schema specifications.  Older versions of
@@ -73,15 +75,16 @@
 
         try:
             return Error.model_validate(response_payload)
         except ValidationError:
             pass
 
         if expected_type:
-            return expected_type.model_validate(response_payload)
+            return expected_type.model_validate(response_payload, scim_ctx=scim_ctx)
+
         return response_payload
 
     def create(self, resource: AnyResource, **kwargs) -> Union[AnyResource, Error]:
         """Perform a POST request to create, as defined in :rfc:`RFC7644 §3.3
         <7644#section-3.3>`.
 
         :param resource: The resource to create
@@ -91,15 +94,15 @@
         :return:
             - An :class:`~scim2_models.Error` object in case of error.
             - The created object as returned by the server in case of success.
         """
 
         self.check_resource_type(resource.__class__)
         url = self.resource_endpoint(resource.__class__)
-        dump = resource.model_dump(exclude_none=True, by_alias=True, mode="json")
+        dump = resource.model_dump(scim_ctx=Context.RESOURCE_CREATION_REQUEST)
         response = self.client.post(url, json=dump, **kwargs)
 
         expected_status_codes = [
             # Resource creation HTTP codes defined at:
             # https://datatracker.ietf.org/doc/html/rfc7644#section-3.3
             201,
             409,
@@ -109,15 +112,20 @@
             308,
             400,
             401,
             403,
             404,
             500,
         ]
-        return self.check_response(response, expected_status_codes, resource.__class__)
+        return self.check_response(
+            response,
+            expected_status_codes,
+            resource.__class__,
+            scim_ctx=Context.RESOURCE_CREATION_RESPONSE,
+        )
 
     def query(
         self,
         resource_type: Type,
         id: Optional[str] = None,
         search_request: Optional[SearchRequest] = None,
         **kwargs,
@@ -138,15 +146,16 @@
             - A `resource_type` object in case of success if `id` is not :data:`None`
             - A :class:`~scim2_models.ListResponse[resource_type]` object in case of success if `id` is :data:`None`
         """
 
         self.check_resource_type(resource_type)
         payload = (
             search_request.model_dump(
-                by_alias=True, exclude_none=True, exclude_unset=True, mode="json"
+                exclude_unset=True,
+                scim_ctx=Context.RESOURCE_QUERY_REQUEST,
             )
             if search_request
             else None
         )
 
         if not id:
             expected_type = ListResponse[resource_type]
@@ -167,15 +176,20 @@
             308,
             401,
             403,
             404,
             500,
         ]
         response = self.client.get(url, params=payload, **kwargs)
-        return self.check_response(response, expected_status_codes, expected_type)
+        return self.check_response(
+            response,
+            expected_status_codes,
+            expected_type,
+            scim_ctx=Context.RESOURCE_QUERY_RESPONSE,
+        )
 
     def query_all(
         self,
         search_request: Optional[SearchRequest] = None,
         **kwargs,
     ) -> Union[AnyResource, ListResponse[AnyResource], Error]:
         """Perform a GET request to read all available resources, as defined in
@@ -192,15 +206,15 @@
 
         # A query against a server root indicates that all resources within the
         # server SHALL be included, subject to filtering.
         # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.4.2.1
 
         payload = (
             search_request.model_dump(
-                by_alias=True, exclude_none=True, exclude_unset=True, mode="json"
+                exclude_unset=True, scim_ctx=Context.RESOURCE_QUERY_REQUEST
             )
             if search_request
             else None
         )
         response = self.client.get("/", params=payload)
 
         expected_status_codes = [
@@ -216,15 +230,18 @@
             403,
             404,
             500,
             501,
         ]
 
         return self.check_response(
-            response, expected_status_codes, ListResponse[Union[self.resource_types]]
+            response,
+            expected_status_codes,
+            ListResponse[Union[self.resource_types]],
+            scim_ctx=Context.RESOURCE_QUERY_RESPONSE,
         )
 
     def search(
         self,
         search_request: Optional[SearchRequest] = None,
         **kwargs,
     ) -> Union[AnyResource, ListResponse[AnyResource], Error]:
@@ -240,15 +257,15 @@
         :return:
             - A :class:`~scim2_models.Error` object in case of error.
             - A :class:`~scim2_models.ListResponse[resource_type]` object in case of success.
         """
 
         payload = (
             search_request.model_dump(
-                by_alias=True, exclude_none=True, exclude_unset=True, mode="json"
+                exclude_unset=True, scim_ctx=Context.RESOURCE_QUERY_RESPONSE
             )
             if search_request
             else None
         )
         response = self.client.post("/.search", params=payload)
 
         expected_status_codes = [
@@ -265,15 +282,18 @@
             404,
             409,
             413,
             500,
             501,
         ]
         return self.check_response(
-            response, expected_status_codes, ListResponse[Union[self.resource_types]]
+            response,
+            expected_status_codes,
+            ListResponse[Union[self.resource_types]],
+            scim_ctx=Context.RESOURCE_QUERY_RESPONSE,
         )
 
     def delete(self, resource_type: Type, id: str, **kwargs) -> Optional[Error]:
         """Perform a DELETE request to create, as defined in :rfc:`RFC7644 §3.6
         <7644#section-3.6>`.
 
         :param kwargs: Additional parameters passed to the underlying
@@ -319,15 +339,15 @@
             - The updated object as returned by the server in case of success.
         """
 
         self.check_resource_type(resource.__class__)
         if not resource.id:
             raise Exception("Resource must have an id")
 
-        dump = resource.model_dump(exclude_none=True, by_alias=True, mode="json")
+        dump = resource.model_dump(scim_ctx=Context.RESOURCE_REPLACEMENT_REQUEST)
         url = self.resource_endpoint(resource.__class__) + f"/{resource.id}"
         response = self.client.put(url, json=dump, **kwargs)
 
         expected_status_codes = [
             # Resource querying HTTP codes defined at:
             # https://datatracker.ietf.org/doc/html/rfc7644#section-3.4.2
             200,
@@ -340,13 +360,18 @@
             403,
             404,
             409,
             412,
             500,
             501,
         ]
-        return self.check_response(response, expected_status_codes, resource.__class__)
+        return self.check_response(
+            response,
+            expected_status_codes,
+            resource.__class__,
+            scim_ctx=Context.RESOURCE_REPLACEMENT_RESPONSE,
+        )
 
     def modify(
         self, resource: AnyResource, op: PatchOp, **kwargs
     ) -> Optional[AnyResource]:
         raise NotImplementedError()
```

### Comparing `scim2_client-0.1.0/scim2_client/errors.py` & `scim2_client-0.1.1/scim2_client/errors.py`

 * *Files identical despite different names*

### Comparing `scim2_client-0.1.0/PKG-INFO` & `scim2_client-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim2-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pythonically build SCIM requests and parse SCIM responses
 License: MIT
 Keywords: scim,scim2,provisioning,httpx,api
 Author: Yaal Coop
 Author-email: contact@yaal.coop
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,20 +16,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: scim2-models (>=0.1.0,<0.2.0)
+Requires-Dist: scim2-models (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # scim2-client
 
-A SCIM client library built upon [scim2-models](https://scim2-models.readthedocs.io), that pythonically build requests and parse responses, following the [RFC7643](https://datatracker.ietf.org/doc/html/rfc7643.html) and [RFC7644](https://datatracker.ietf.org/doc/html/rfc7644.html) specifications.
+A SCIM client Python library built upon [scim2-models](https://scim2-models.readthedocs.io) and [httpx](https://github.com/encode/httpx),
+that pythonically build requests and parse responses,
+following the [RFC7643](https://datatracker.ietf.org/doc/html/rfc7643.html) and [RFC7644](https://datatracker.ietf.org/doc/html/rfc7644.html) specifications.
 ## Installation
 
 ```shell
 pip install scim2-client
 ```
 
 ## Usage
```

