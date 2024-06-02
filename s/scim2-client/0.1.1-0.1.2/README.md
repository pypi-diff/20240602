# Comparing `tmp/scim2_client-0.1.1.tar.gz` & `tmp/scim2_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim2_client-0.1.1.tar", max compression
+gzip compressed data, was "scim2_client-0.1.2.tar", max compression
```

## Comparing `scim2_client-0.1.1.tar` & `scim2_client-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1674 2024-06-01 19:35:02.108808 scim2_client-0.1.1/README.md
--rw-r--r--   0        0        0     2491 2024-06-01 20:29:46.814362 scim2_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      338 2024-06-01 18:36:39.646458 scim2_client-0.1.1/scim2_client/__init__.py
--rw-r--r--   0        0        0    13199 2024-06-01 20:29:55.831143 scim2_client-0.1.1/scim2_client/client.py
--rw-r--r--   0        0        0     1175 2024-06-01 18:36:39.646458 scim2_client-0.1.1/scim2_client/errors.py
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 scim2_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1674 2024-06-01 20:44:18.372214 scim2_client-0.1.2/README.md
+-rw-r--r--   0        0        0     2491 2024-06-02 09:34:55.421471 scim2_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      338 2024-06-01 18:36:39.646458 scim2_client-0.1.2/scim2_client/__init__.py
+-rw-r--r--   0        0        0    16538 2024-06-02 09:32:05.458747 scim2_client-0.1.2/scim2_client/client.py
+-rw-r--r--   0        0        0     1175 2024-06-01 18:36:39.646458 scim2_client-0.1.2/scim2_client/errors.py
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 scim2_client-0.1.2/PKG-INFO
```

### Comparing `scim2_client-0.1.1/README.md` & `scim2_client-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Check the [tutorial](https://scim2-client.readthedocs.io/en/latest/tutorial.html) and the [reference](https://scim2-client.readthedocs.io/en/latest/reference.html) for more details.
 
 Here is an example of usage:
 
 ```python
 import datetime
-from httpx impont Client
+from httpx import Client
 from scim2_models import User, EnterpriseUserUser, Group, Error
 from scim2_client import SCIMClient
 
 client = Client(base_url=f"https://auth.example/scim/v2", headers={"Authorization": "Bearer foobar"})
 scim = SCIMClient(client, resource_types=(User[EnterpriseUser], Group))
 
 # Query resources
```

### Comparing `scim2_client-0.1.1/pyproject.toml` & `scim2_client-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scim2-client"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pythonically build SCIM requests and parse SCIM responses"
 authors = ["Yaal Coop <contact@yaal.coop>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["scim", "scim2", "provisioning", "httpx", "api"]
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `scim2_client-0.1.1/scim2_client/client.py` & `scim2_client-0.1.2/scim2_client/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import json.decoder
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
 
 from httpx import Client
@@ -25,14 +26,79 @@
     "Content-Type": "application/scim+json",
 }
 
 
 class SCIMClient:
     """An object that perform SCIM requests and validate responses."""
 
+    CREATION_RESPONSE_STATUS_CODES: List[int] = [
+        201,
+        409,
+        307,
+        308,
+        400,
+        401,
+        403,
+        404,
+        500,
+    ]
+    """Resource creation HTTP codes defined at :rfc:`RFC7644 §3.3
+    <7644#section-3.3>` and :rfc:`RFC7644 §3.12 <7644#section-3.12>`"""
+
+    QUERY_RESPONSE_STATUS_CODES: List[int] = [200, 400, 307, 308, 401, 403, 404, 500]
+    """Resource querying HTTP codes defined at :rfc:`RFC7644 §3.4.2
+    <7644#section-3.4.2>` and :rfc:`RFC7644 §3.12 <7644#section-3.12>`"""
+
+    SEARCH_RESPONSE_STATUS_CODES: List[int] = [
+        200,
+        307,
+        308,
+        400,
+        401,
+        403,
+        404,
+        409,
+        413,
+        500,
+        501,
+    ]
+    """Resource querying HTTP codes defined at :rfc:`RFC7644 §3.4.3
+    <7644#section-3.4.3>` and :rfc:`RFC7644 §3.12 <7644#section-3.12>`"""
+
+    DELETION_RESPONSE_STATUS_CODES: List[int] = [
+        204,
+        307,
+        308,
+        400,
+        401,
+        403,
+        404,
+        412,
+        500,
+        501,
+    ]
+    """Resource deletion HTTP codes defined at :rfc:`RFC7644 §3.6
+    <7644#section-3.6>` and :rfc:`RFC7644 §3.12 <7644#section-3.12>`"""
+
+    REPLACEMENT_RESPONSE_STATUS_CODES: List[int] = [
+        200,
+        307,
+        308,
+        400,
+        401,
+        403,
+        404,
+        409,
+        412,
+        500,
+        501,
+    ]
+    """Resource querying HTTP codes defined at :rfc:`RFC7644 §3.4.2
+    <7644#section-3.4.2>` and :rfc:`RFC7644 §3.12 <7644#section-3.12>`"""
+
     def __init__(self, client: Client, resource_types: Optional[Tuple[Type]] = None):
         self.client = client
         self.resource_types = resource_types or ()
 
     def check_resource_type(self, resource_type):
         if resource_type not in self.resource_types:
             raise ValueError(f"Unknown resource type: '{resource_type}'")
@@ -43,15 +109,15 @@
     def check_response(
         self,
         response: Response,
         expected_status_codes: List[int],
         expected_type: Optional[Type] = None,
         scim_ctx: Optional[Context] = None,
     ):
-        if response.status_code not in expected_status_codes:
+        if expected_status_codes and response.status_code not in expected_status_codes:
             raise UnexpectedStatusCode(response)
 
         # Interoperability considerations:  The "application/scim+json" media
         # type is intended to identify JSON structure data that conforms to
         # the SCIM protocol and schema specifications.  Older versions of
         # SCIM are known to informally use "application/json".
         # https://datatracker.ietf.org/doc/html/rfc7644.html#section-8.1
@@ -60,318 +126,317 @@
         if response.headers.get("content-type") not in expected_response_content_types:
             raise UnexpectedContentType(response)
 
         # In addition to returning an HTTP response code, implementers MUST return
         # the errors in the body of the response in a JSON format
         # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.12
 
-        if response.status_code in (204, 205):
+        no_content_status_codes = [204, 205]
+        if response.status_code in no_content_status_codes:
             response_payload = None
 
         else:
             try:
                 response_payload = response.json()
             except json.decoder.JSONDecodeError as exc:
                 raise UnexpectedContentFormat(response) from exc
 
         try:
             return Error.model_validate(response_payload)
         except ValidationError:
             pass
 
         if expected_type:
-            return expected_type.model_validate(response_payload, scim_ctx=scim_ctx)
+            try:
+                return expected_type.model_validate(response_payload, scim_ctx=scim_ctx)
+            except ValidationError as exc:
+                exc.response_payload = response_payload
+                raise exc
 
         return response_payload
 
-    def create(self, resource: AnyResource, **kwargs) -> Union[AnyResource, Error]:
+    def create(
+        self,
+        resource: Union[AnyResource, Dict],
+        check_request_payload: bool = True,
+        check_response_payload: bool = True,
+        check_status_code: bool = True,
+        **kwargs,
+    ) -> Union[AnyResource, Error, Dict]:
         """Perform a POST request to create, as defined in :rfc:`RFC7644 §3.3
         <7644#section-3.3>`.
 
         :param resource: The resource to create
+        :param check_request_payload: If :data:`False`,
+            :code:`resource` is expected to be a dict that will be passed as-is in the request.
+        :param check_response_payload: Whether to validate that the response payload is valid.
+            If set, the raw payload will be returned.
+        :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying HTTP request
             library.
 
         :return:
             - An :class:`~scim2_models.Error` object in case of error.
             - The created object as returned by the server in case of success.
         """
 
-        self.check_resource_type(resource.__class__)
-        url = self.resource_endpoint(resource.__class__)
-        dump = resource.model_dump(scim_ctx=Context.RESOURCE_CREATION_REQUEST)
-        response = self.client.post(url, json=dump, **kwargs)
-
-        expected_status_codes = [
-            # Resource creation HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644#section-3.3
-            201,
-            409,
-            # Default HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.12
-            307,
-            308,
-            400,
-            401,
-            403,
-            404,
-            500,
-        ]
+        if not check_request_payload:
+            payload = resource
+            url = kwargs.pop("url", None)
+
+        else:
+            self.check_resource_type(resource.__class__)
+            url = kwargs.pop("url", self.resource_endpoint(resource.__class__))
+            payload = resource.model_dump(scim_ctx=Context.RESOURCE_CREATION_REQUEST)
+
+        response = self.client.post(url, json=payload, **kwargs)
+
         return self.check_response(
             response,
-            expected_status_codes,
-            resource.__class__,
+            self.CREATION_RESPONSE_STATUS_CODES if check_status_code else None,
+            resource.__class__
+            if check_request_payload and check_response_payload
+            else None,
             scim_ctx=Context.RESOURCE_CREATION_RESPONSE,
         )
 
     def query(
         self,
         resource_type: Type,
         id: Optional[str] = None,
-        search_request: Optional[SearchRequest] = None,
+        search_request: Optional[Union[SearchRequest, Dict]] = None,
+        check_request_payload: bool = True,
+        check_response_payload: bool = True,
+        check_status_code: bool = True,
         **kwargs,
-    ) -> Union[AnyResource, ListResponse[AnyResource], Error]:
+    ) -> Union[AnyResource, ListResponse[AnyResource], Error, Dict]:
         """Perform a GET request to read resources, as defined in :rfc:`RFC7644
         §3.4.2 <7644#section-3.4.2>`.
 
         - If `id` is not :data:`None`, the resource with the exact id will be reached.
         - If `id` is :data:`None`, all the resources with the given type will be reached.
 
         :param resource_type: A :class:`~scim2_models.Resource` subtype or :data:`None`
         :param id: The SCIM id of an object to get, or :data:`None`
         :param search_request: An object detailing the search query parameters.
+        :param check_request_payload: If :data:`False`,
+            :code:`search_request` is expected to be a dict that will be passed as-is in the request.
+        :param check_response_payload: Whether to validate that the response payload is valid.
+            If set, the raw payload will be returned.
+        :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying HTTP request library.
 
         :return:
             - A :class:`~scim2_models.Error` object in case of error.
             - A `resource_type` object in case of success if `id` is not :data:`None`
             - A :class:`~scim2_models.ListResponse[resource_type]` object in case of success if `id` is :data:`None`
         """
 
         self.check_resource_type(resource_type)
-        payload = (
-            search_request.model_dump(
-                exclude_unset=True,
-                scim_ctx=Context.RESOURCE_QUERY_REQUEST,
+        if not check_request_payload:
+            payload = search_request
+
+        else:
+            payload = (
+                search_request.model_dump(
+                    exclude_unset=True,
+                    scim_ctx=Context.RESOURCE_QUERY_REQUEST,
+                )
+                if search_request
+                else None
             )
-            if search_request
-            else None
-        )
 
         if not id:
             expected_type = ListResponse[resource_type]
             url = self.resource_endpoint(resource_type)
 
         else:
             expected_type = resource_type
             url = self.resource_endpoint(resource_type) + f"/{id}"
 
-        expected_status_codes = [
-            # Resource querying HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644#section-3.4.2
-            200,
-            400,
-            # Default HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.12
-            307,
-            308,
-            401,
-            403,
-            404,
-            500,
-        ]
         response = self.client.get(url, params=payload, **kwargs)
         return self.check_response(
             response,
-            expected_status_codes,
-            expected_type,
+            self.QUERY_RESPONSE_STATUS_CODES if check_status_code else None,
+            expected_type if check_response_payload else None,
             scim_ctx=Context.RESOURCE_QUERY_RESPONSE,
         )
 
     def query_all(
         self,
         search_request: Optional[SearchRequest] = None,
+        check_request_payload: bool = True,
+        check_response_payload: bool = True,
+        check_status_code: bool = True,
         **kwargs,
-    ) -> Union[AnyResource, ListResponse[AnyResource], Error]:
+    ) -> Union[AnyResource, ListResponse[AnyResource], Error, Dict]:
         """Perform a GET request to read all available resources, as defined in
         :rfc:`RFC7644 §3.4.2.1 <7644#section-3.4.2.1>`.
 
         :param search_request: An object detailing the search query parameters.
+        :param check_request_payload: If :data:`False`,
+            :code:`search_request` is expected to be a dict that will be passed as-is in the request.
+        :param check_response_payload: Whether to validate that the response payload is valid.
+            If set, the raw payload will be returned.
+        :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying
             HTTP request library.
 
         :return:
             - A :class:`~scim2_models.Error` object in case of error.
             - A :class:`~scim2_models.ListResponse[resource_type]` object in case of success.
         """
 
         # A query against a server root indicates that all resources within the
         # server SHALL be included, subject to filtering.
         # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.4.2.1
 
-        payload = (
-            search_request.model_dump(
-                exclude_unset=True, scim_ctx=Context.RESOURCE_QUERY_REQUEST
+        if not check_request_payload:
+            payload = search_request
+
+        else:
+            payload = (
+                search_request.model_dump(
+                    exclude_unset=True, scim_ctx=Context.RESOURCE_QUERY_REQUEST
+                )
+                if search_request
+                else None
             )
-            if search_request
-            else None
-        )
-        response = self.client.get("/", params=payload)
 
-        expected_status_codes = [
-            # Resource querying HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644#section-3.4.2
-            200,
-            400,
-            # Default HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.12
-            307,
-            308,
-            401,
-            403,
-            404,
-            500,
-            501,
-        ]
+        response = self.client.get("/", params=payload)
 
         return self.check_response(
             response,
-            expected_status_codes,
-            ListResponse[Union[self.resource_types]],
+            self.QUERY_RESPONSE_STATUS_CODES if check_status_code else None,
+            ListResponse[Union[self.resource_types]]
+            if check_response_payload
+            else None,
             scim_ctx=Context.RESOURCE_QUERY_RESPONSE,
         )
 
     def search(
         self,
         search_request: Optional[SearchRequest] = None,
+        check_request_payload: bool = True,
+        check_response_payload: bool = True,
+        check_status_code: bool = True,
         **kwargs,
-    ) -> Union[AnyResource, ListResponse[AnyResource], Error]:
+    ) -> Union[AnyResource, ListResponse[AnyResource], Error, Dict]:
         """Perform a POST search request to read all available resources, as
         defined in :rfc:`RFC7644 §3.4.3 <7644#section-3.4.3>`.
 
         :param resource_types: Resource type or union of types expected
             to be read from the response.
         :param search_request: An object detailing the search query parameters.
+        :param check_request_payload: If :data:`False`,
+            :code:`search_request` is expected to be a dict that will be passed as-is in the request.
+        :param check_response_payload: Whether to validate that the response payload is valid.
+            If set, the raw payload will be returned.
+        :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying
             HTTP request library.
 
         :return:
             - A :class:`~scim2_models.Error` object in case of error.
             - A :class:`~scim2_models.ListResponse[resource_type]` object in case of success.
         """
 
-        payload = (
-            search_request.model_dump(
-                exclude_unset=True, scim_ctx=Context.RESOURCE_QUERY_RESPONSE
+        if not check_request_payload:
+            payload = search_request
+
+        else:
+            payload = (
+                search_request.model_dump(
+                    exclude_unset=True, scim_ctx=Context.RESOURCE_QUERY_RESPONSE
+                )
+                if search_request
+                else None
             )
-            if search_request
-            else None
-        )
+
         response = self.client.post("/.search", params=payload)
 
-        expected_status_codes = [
-            # Resource querying HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644#section-3.4.3
-            200,
-            # Default HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.12
-            307,
-            308,
-            400,
-            401,
-            403,
-            404,
-            409,
-            413,
-            500,
-            501,
-        ]
         return self.check_response(
             response,
-            expected_status_codes,
-            ListResponse[Union[self.resource_types]],
+            self.SEARCH_RESPONSE_STATUS_CODES if check_status_code else None,
+            ListResponse[Union[self.resource_types]]
+            if check_response_payload
+            else None,
             scim_ctx=Context.RESOURCE_QUERY_RESPONSE,
         )
 
-    def delete(self, resource_type: Type, id: str, **kwargs) -> Optional[Error]:
+    def delete(
+        self, resource_type: Type, id: str, check_status_code: bool = True, **kwargs
+    ) -> Optional[Union[Error, Dict]]:
         """Perform a DELETE request to create, as defined in :rfc:`RFC7644 §3.6
         <7644#section-3.6>`.
 
+        :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying
             HTTP request library.
 
         :return:
             - A :class:`~scim2_models.Error` object in case of error.
             - :data:`None` in case of success.
         """
 
         self.check_resource_type(resource_type)
         url = self.resource_endpoint(resource_type) + f"/{id}"
         response = self.client.delete(url, **kwargs)
 
-        expected_status_codes = [
-            # Resource deletion HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644#section-3.6
-            204,
-            # Default HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.12
-            307,
-            308,
-            400,
-            401,
-            403,
-            404,
-            412,
-            500,
-            501,
-        ]
-        return self.check_response(response, expected_status_codes)
+        return self.check_response(
+            response, self.DELETION_RESPONSE_STATUS_CODES if check_status_code else None
+        )
 
-    def replace(self, resource: AnyResource, **kwargs) -> Union[AnyResource, Error]:
+    def replace(
+        self,
+        resource: Union[AnyResource, Dict],
+        check_request_payload: bool = True,
+        check_response_payload: bool = True,
+        check_status_code: bool = True,
+        **kwargs,
+    ) -> Union[AnyResource, Error, Dict]:
         """Perform a PUT request to replace a resource, as defined in
         :rfc:`RFC7644 §3.5.1 <7644#section-3.5.1>`.
 
         :param resource: The new state of the resource to replace.
+        :param check_request_payload: If :data:`False`,
+            :code:`resource` is expected to be a dict that will be passed as-is in the request.
+        :param check_response_payload: Whether to validate that the response payload is valid.
+            If set, the raw payload will be returned.
+        :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying
             HTTP request library.
 
         :return:
             - An :class:`~scim2_models.Error` object in case of error.
             - The updated object as returned by the server in case of success.
         """
 
-        self.check_resource_type(resource.__class__)
-        if not resource.id:
-            raise Exception("Resource must have an id")
-
-        dump = resource.model_dump(scim_ctx=Context.RESOURCE_REPLACEMENT_REQUEST)
-        url = self.resource_endpoint(resource.__class__) + f"/{resource.id}"
-        response = self.client.put(url, json=dump, **kwargs)
-
-        expected_status_codes = [
-            # Resource querying HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644#section-3.4.2
-            200,
-            # Default HTTP codes defined at:
-            # https://datatracker.ietf.org/doc/html/rfc7644.html#section-3.12
-            307,
-            308,
-            400,
-            401,
-            403,
-            404,
-            409,
-            412,
-            500,
-            501,
-        ]
+        if not check_request_payload:
+            payload = resource
+            url = kwargs.pop("url")
+
+        else:
+            self.check_resource_type(resource.__class__)
+            if not resource.id:
+                raise Exception("Resource must have an id")
+
+            payload = resource.model_dump(scim_ctx=Context.RESOURCE_REPLACEMENT_REQUEST)
+            url = kwargs.pop(
+                "url", self.resource_endpoint(resource.__class__) + f"/{resource.id}"
+            )
+
+        response = self.client.put(url, json=payload, **kwargs)
+
         return self.check_response(
             response,
-            expected_status_codes,
-            resource.__class__,
+            self.REPLACEMENT_RESPONSE_STATUS_CODES if check_status_code else None,
+            resource.__class__
+            if check_request_payload and check_response_payload
+            else None,
             scim_ctx=Context.RESOURCE_REPLACEMENT_RESPONSE,
         )
 
     def modify(
-        self, resource: AnyResource, op: PatchOp, **kwargs
-    ) -> Optional[AnyResource]:
+        self, resource: Union[AnyResource, Dict], op: PatchOp, **kwargs
+    ) -> Optional[Union[AnyResource, Dict]]:
         raise NotImplementedError()
```

### Comparing `scim2_client-0.1.1/scim2_client/errors.py` & `scim2_client-0.1.2/scim2_client/errors.py`

 * *Files identical despite different names*

### Comparing `scim2_client-0.1.1/PKG-INFO` & `scim2_client-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim2-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pythonically build SCIM requests and parse SCIM responses
 License: MIT
 Keywords: scim,scim2,provisioning,httpx,api
 Author: Yaal Coop
 Author-email: contact@yaal.coop
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -38,15 +38,15 @@
 
 Check the [tutorial](https://scim2-client.readthedocs.io/en/latest/tutorial.html) and the [reference](https://scim2-client.readthedocs.io/en/latest/reference.html) for more details.
 
 Here is an example of usage:
 
 ```python
 import datetime
-from httpx impont Client
+from httpx import Client
 from scim2_models import User, EnterpriseUserUser, Group, Error
 from scim2_client import SCIMClient
 
 client = Client(base_url=f"https://auth.example/scim/v2", headers={"Authorization": "Bearer foobar"})
 scim = SCIMClient(client, resource_types=(User[EnterpriseUser], Group))
 
 # Query resources
```

