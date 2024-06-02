# Comparing `tmp/scim2_client-0.1.2.tar.gz` & `tmp/scim2_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim2_client-0.1.2.tar", max compression
+gzip compressed data, was "scim2_client-0.1.3.tar", max compression
```

## Comparing `scim2_client-0.1.2.tar` & `scim2_client-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1674 2024-06-01 20:44:18.372214 scim2_client-0.1.2/README.md
--rw-r--r--   0        0        0     2491 2024-06-02 09:34:55.421471 scim2_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      338 2024-06-01 18:36:39.646458 scim2_client-0.1.2/scim2_client/__init__.py
--rw-r--r--   0        0        0    16538 2024-06-02 09:32:05.458747 scim2_client-0.1.2/scim2_client/client.py
--rw-r--r--   0        0        0     1175 2024-06-01 18:36:39.646458 scim2_client-0.1.2/scim2_client/errors.py
--rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 scim2_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1674 2024-06-01 20:44:18.372214 scim2_client-0.1.3/README.md
+-rw-r--r--   0        0        0     2491 2024-06-02 14:17:48.605239 scim2_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      338 2024-06-01 18:36:39.646458 scim2_client-0.1.3/scim2_client/__init__.py
+-rw-r--r--   0        0        0    17669 2024-06-02 14:15:20.059236 scim2_client-0.1.3/scim2_client/client.py
+-rw-r--r--   0        0        0     1175 2024-06-01 18:36:39.646458 scim2_client-0.1.3/scim2_client/errors.py
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 scim2_client-0.1.3/PKG-INFO
```

### Comparing `scim2_client-0.1.2/README.md` & `scim2_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `scim2_client-0.1.2/pyproject.toml` & `scim2_client-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scim2-client"
-version = "0.1.2"
+version = "0.1.3"
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
-scim2-models = "^0.1.1"
+scim2-models = "^0.1.2"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.1"
 pytest-coverage = "^0.0"
```

### Comparing `scim2_client-0.1.2/scim2_client/client.py` & `scim2_client-0.1.3/scim2_client/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 from httpx import Response
 from pydantic import ValidationError
 from scim2_models import AnyResource
 from scim2_models import Context
 from scim2_models import Error
 from scim2_models import ListResponse
 from scim2_models import PatchOp
+from scim2_models import Resource
 from scim2_models import SearchRequest
 
+from .errors import SCIMClientError
 from .errors import UnexpectedContentFormat
 from .errors import UnexpectedContentType
 from .errors import UnexpectedStatusCode
 
 BASE_HEADERS = {
     "Accept": "application/scim+json",
     "Content-Type": "application/scim+json",
@@ -162,14 +164,15 @@
         check_status_code: bool = True,
         **kwargs,
     ) -> Union[AnyResource, Error, Dict]:
         """Perform a POST request to create, as defined in :rfc:`RFC7644 §3.3
         <7644#section-3.3>`.
 
         :param resource: The resource to create
+            If is a :data:`dict`, the resource type will be guessed from the schema.
         :param check_request_payload: If :data:`False`,
             :code:`resource` is expected to be a dict that will be passed as-is in the request.
         :param check_response_payload: Whether to validate that the response payload is valid.
             If set, the raw payload will be returned.
         :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying HTTP request
             library.
@@ -180,16 +183,28 @@
         """
 
         if not check_request_payload:
             payload = resource
             url = kwargs.pop("url", None)
 
         else:
-            self.check_resource_type(resource.__class__)
-            url = kwargs.pop("url", self.resource_endpoint(resource.__class__))
+            if isinstance(resource, Resource):
+                resource_type = resource.__class__
+
+            else:
+                resource_type = Resource.get_by_payload(self.resource_types, resource)
+                if not resource_type:
+                    raise SCIMClientError(
+                        None, "Cannot guess resource type from the payload"
+                    )
+
+                resource = resource_type.model_validate(resource)
+
+            self.check_resource_type(resource_type)
+            url = kwargs.pop("url", self.resource_endpoint(resource_type))
             payload = resource.model_dump(scim_ctx=Context.RESOURCE_CREATION_REQUEST)
 
         response = self.client.post(url, json=payload, **kwargs)
 
         return self.check_response(
             response,
             self.CREATION_RESPONSE_STATUS_CODES if check_status_code else None,
@@ -348,15 +363,15 @@
                 search_request.model_dump(
                     exclude_unset=True, scim_ctx=Context.RESOURCE_QUERY_RESPONSE
                 )
                 if search_request
                 else None
             )
 
-        response = self.client.post("/.search", params=payload)
+        response = self.client.post("/.search", json=payload)
 
         return self.check_response(
             response,
             self.SEARCH_RESPONSE_STATUS_CODES if check_status_code else None,
             ListResponse[Union[self.resource_types]]
             if check_response_payload
             else None,
@@ -393,15 +408,16 @@
         check_response_payload: bool = True,
         check_status_code: bool = True,
         **kwargs,
     ) -> Union[AnyResource, Error, Dict]:
         """Perform a PUT request to replace a resource, as defined in
         :rfc:`RFC7644 §3.5.1 <7644#section-3.5.1>`.
 
-        :param resource: The new state of the resource to replace.
+        :param resource: The new resource to replace.
+            If is a :data:`dict`, the resource type will be guessed from the schema.
         :param check_request_payload: If :data:`False`,
             :code:`resource` is expected to be a dict that will be passed as-is in the request.
         :param check_response_payload: Whether to validate that the response payload is valid.
             If set, the raw payload will be returned.
         :param check_status_code: Whether to validate that the response status code is valid.
         :param kwargs: Additional parameters passed to the underlying
             HTTP request library.
@@ -409,20 +425,33 @@
         :return:
             - An :class:`~scim2_models.Error` object in case of error.
             - The updated object as returned by the server in case of success.
         """
 
         if not check_request_payload:
             payload = resource
-            url = kwargs.pop("url")
+            url = kwargs.pop("url", None)
 
         else:
-            self.check_resource_type(resource.__class__)
+            if isinstance(resource, Resource):
+                resource_type = resource.__class__
+
+            else:
+                resource_type = Resource.get_by_payload(self.resource_types, resource)
+                if not resource_type:
+                    raise SCIMClientError(
+                        None, "Cannot guess resource type from the payload"
+                    )
+
+                resource = resource_type.model_validate(resource)
+
+            self.check_resource_type(resource_type)
+
             if not resource.id:
-                raise Exception("Resource must have an id")
+                raise SCIMClientError(None, "Resource must have an id")
 
             payload = resource.model_dump(scim_ctx=Context.RESOURCE_REPLACEMENT_REQUEST)
             url = kwargs.pop(
                 "url", self.resource_endpoint(resource.__class__) + f"/{resource.id}"
             )
 
         response = self.client.put(url, json=payload, **kwargs)
```

### Comparing `scim2_client-0.1.2/scim2_client/errors.py` & `scim2_client-0.1.3/scim2_client/errors.py`

 * *Files identical despite different names*

### Comparing `scim2_client-0.1.2/PKG-INFO` & `scim2_client-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim2-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pythonically build SCIM requests and parse SCIM responses
 License: MIT
 Keywords: scim,scim2,provisioning,httpx,api
 Author: Yaal Coop
 Author-email: contact@yaal.coop
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: scim2-models (>=0.1.1,<0.2.0)
+Requires-Dist: scim2-models (>=0.1.2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # scim2-client
 
 A SCIM client Python library built upon [scim2-models](https://scim2-models.readthedocs.io) and [httpx](https://github.com/encode/httpx),
 that pythonically build requests and parse responses,
 following the [RFC7643](https://datatracker.ietf.org/doc/html/rfc7643.html) and [RFC7644](https://datatracker.ietf.org/doc/html/rfc7644.html) specifications.
```

