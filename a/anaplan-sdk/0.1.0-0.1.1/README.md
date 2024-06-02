# Comparing `tmp/anaplan_sdk-0.1.0.tar.gz` & `tmp/anaplan_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaplan_sdk-0.1.0.tar", max compression
+gzip compressed data, was "anaplan_sdk-0.1.1.tar", max compression
```

## Comparing `anaplan_sdk-0.1.0.tar` & `anaplan_sdk-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0      637 2024-05-30 13:10:49.020625 anaplan_sdk-0.1.0/anaplan_sdk/__init__.py
--rw-r--r--   0        0        0    14851 2024-06-01 10:59:40.846960 anaplan_sdk-0.1.0/anaplan_sdk/_async_client.py
--rw-r--r--   0        0        0     5029 2024-06-01 10:59:40.846960 anaplan_sdk-0.1.0/anaplan_sdk/_auth.py
--rw-r--r--   0        0        0    16587 2024-06-01 10:59:40.853386 anaplan_sdk-0.1.0/anaplan_sdk/_client.py
--rw-r--r--   0        0        0     1612 2024-05-29 16:27:14.773666 anaplan_sdk-0.1.0/anaplan_sdk/_exceptions.py
--rw-r--r--   0        0        0     5397 2024-06-01 10:59:40.853386 anaplan_sdk-0.1.0/anaplan_sdk/_models.py
--rw-r--r--   0        0        0    11558 2024-05-27 16:31:14.513449 anaplan_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0     1641 2024-06-01 11:00:25.476253 anaplan_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2425 2024-05-30 11:53:01.695230 anaplan_sdk-0.1.0/README.md
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 anaplan_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2024-06-02 11:54:35.958338 anaplan_sdk-0.1.1/anaplan_sdk/__init__.py
+-rw-r--r--   0        0        0    13939 2024-06-02 12:52:32.417604 anaplan_sdk-0.1.1/anaplan_sdk/_async_client.py
+-rw-r--r--   0        0        0     3548 2024-06-02 12:49:58.681726 anaplan_sdk-0.1.1/anaplan_sdk/_async_transactional_client.py
+-rw-r--r--   0        0        0     6711 2024-06-02 12:32:51.256809 anaplan_sdk-0.1.1/anaplan_sdk/_auth.py
+-rw-r--r--   0        0        0     3368 2024-06-02 12:33:25.880072 anaplan_sdk-0.1.1/anaplan_sdk/_base.py
+-rw-r--r--   0        0        0    15583 2024-06-02 12:08:24.138197 anaplan_sdk-0.1.1/anaplan_sdk/_client.py
+-rw-r--r--   0        0        0     3345 2024-06-02 12:46:15.508324 anaplan_sdk-0.1.1/anaplan_sdk/_transactional_client.py
+-rw-r--r--   0        0        0     1634 2024-06-02 12:28:22.604324 anaplan_sdk-0.1.1/anaplan_sdk/exceptions.py
+-rw-r--r--   0        0        0    13353 2024-06-02 12:43:42.410930 anaplan_sdk-0.1.1/anaplan_sdk/models.py
+-rw-r--r--   0        0        0    11558 2024-05-27 16:31:14.513449 anaplan_sdk-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1666 2024-06-02 13:31:52.016083 anaplan_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2425 2024-05-30 11:53:01.695230 anaplan_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 anaplan_sdk-0.1.1/PKG-INFO
```

### Comparing `anaplan_sdk-0.1.0/anaplan_sdk/_async_client.py` & `anaplan_sdk-0.1.1/anaplan_sdk/_async_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,28 @@
 """
 Asynchronous Client.
 """
 
-import gzip
 import logging
 import time
 from asyncio import gather
-from typing import Callable, Coroutine, Any
 
 import httpx
-from httpx import HTTPError, Response
 
+from ._async_transactional_client import _AsyncTransactionalClient
 from ._auth import AnaplanCertAuth, get_certificate, get_private_key, AnaplanBasicAuth
-from ._exceptions import (
-    AnaplanActionError,
-    raise_appropriate_error,
-)
-from ._models import (
-    Import,
-    Export,
-    Process,
-    File,
-    Action,
-    List,
-    Workspace,
-    Model,
-    to_workspaces,
-    to_models,
-    to_actions,
-    to_imports,
-    to_exports,
-    to_processes,
-    to_files,
-    to_lists,
-    determine_action_type,
-)
+from ._base import _AsyncBaseClient
+from .exceptions import AnaplanActionError
+from .models import Import, Export, Process, File, Action, Workspace, Model, action_url
 
 logging.getLogger("httpx").setLevel(logging.CRITICAL)
 logger = logging.getLogger("anaplan_sdk")
 
 
-class AsyncClient:
+class AsyncClient(_AsyncBaseClient):
     """
     An asynchronous Client for pythonic access to the Anaplan Integration API v2:
     https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API, so
     you can deal with python objects and simple functions rather than implementation details like
     http, json, compression, chunking etc.
 
 
@@ -85,123 +63,144 @@
         :param password: Password for the given `user_email`. This is not suitable for production
                          setups. If you intend to use this in production, acquire a client
                          certificate as described under: https://help.anaplan.com/procure-ca-certificates-47842267-2cb3-4e38-90bf-13b1632bcd44
         :param certificate: The absolute path to the client certificate file or the certificate
                             itself.
         :param private_key: The absolute path to the private key file or the private key itself.
         :param private_key_password: The password to access the private key if there is one.
-        :param timeout: The timeout for the HTTP requests.
+        :param timeout: The timeout in seconds for the HTTP requests.
         :param retry_count: The number of times to retry an HTTP request if it fails. Set this to 0
                             to never retry. Defaults to 2, meaning each HTTP Operation will be
                             tried a total number of 2 times.
         :param status_poll_delay: The delay between polling the status of a task.
         :param upload_chunk_size: The size of the chunks to upload. This is the maximum size of
                                   each chunk. Defaults to 25MB.
         :param allow_file_creation: Whether to allow the creation of new files. Defaults to False
                             since this is typically unintentional and may well be unwanted
                             behaviour in the API altogether. A file that is created this
                             way will not be referenced by any action in anaplan until
                             manually assigned so there is typically no value in dynamically
                             creating new files and uploading content to them."""
         if not ((user_email and password) or (certificate and private_key)):
             raise ValueError(
-                "Either `certificate` and `private_key` or `user_email` and `password` must be "
-                "provided."
+                "Must provide `certificate` and `private_key` or `user_email` and `password`."
+                "If you Private Key is Password protected, must also pass `private_key_password`."
             )
-        auth = (
-            AnaplanCertAuth(
-                get_certificate(certificate), get_private_key(private_key, private_key_password)
-            )
-            if certificate
-            else AnaplanBasicAuth(user_email=user_email, password=password)
+        client = httpx.AsyncClient(
+            auth=(
+                AnaplanCertAuth(
+                    get_certificate(certificate), get_private_key(private_key, private_key_password)
+                )
+                if certificate
+                else AnaplanBasicAuth(user_email=user_email, password=password)
+            ),
+            timeout=timeout,
+        )
+        self._url = f"https://api.anaplan.com/2/0/workspaces/{workspace_id}/models/{model_id}"
+        self._transactional_client = (
+            _AsyncTransactionalClient(client, model_id, retry_count) if model_id else None
         )
-        self._client = httpx.AsyncClient(auth=auth)
-        self._base_url = "https://api.anaplan.com/2/0/workspaces"
-        self.workspace_id = workspace_id
-        self.model_id = model_id
-        self.timeout = timeout
-        self.retry_count = retry_count
         self.status_poll_delay = status_poll_delay
         self.upload_chunk_size = upload_chunk_size
         self.allow_file_creation = allow_file_creation
+        super().__init__(retry_count, client)
+
+    @property
+    def transactional(self) -> _AsyncTransactionalClient:
+        """
+        The Transactional Client provides access to the Anaplan Transactional API. This is useful
+        for more advanced use cases where you need to interact with the Anaplan Model in a more
+        granular way.
+
+        If you instantiated the client without the field `model_id`, this will raise a
+        :py:class:`ValueError`, since none of the endpoints can be invoked without the model Id.
+        :return: The Transactional Client.
+        """
+        if not self._transactional_client:
+            raise ValueError(
+                "Cannot use the Transactional Client (Anaplan Transactional API) "
+                "without field `model_id`. Make sure the instance you are trying to call this on "
+                "is instantiated correctly with a valid `model_id`."
+            )
+        return self._transactional_client
 
     async def list_workspaces(self) -> list[Workspace]:
         """
         Lists all the Workspaces the authenticated user has access to.
         :return: All Workspaces as a list of :py:class:`Workspace`.
         """
-        return to_workspaces(await self._get(f"{self._base_url}?tenantDetails=true"))
+        return [
+            Workspace.model_validate(e)
+            for e in (
+                await self._get("https://api.anaplan.com/2/0/workspaces?tenantDetails=true")
+            ).get("workspaces")
+        ]
 
     async def list_models(self) -> list[Model]:
         """
         Lists all the Models the authenticated user has access to.
         :return: All Models in the Workspace as a list of :py:class:`Model`.
         """
-        return to_models(
-            await self._get(f"{self._base_url.replace('/workspaces', '/models')}?modelDetails=true")
-        )
+        return [
+            Model.model_validate(e)
+            for e in (await self._get("https://api.anaplan.com/2/0/models?modelDetails=true")).get(
+                "models"
+            )
+        ]
+
+    async def list_files(self) -> list[File]:
+        """
+        Lists all the Files in the Model.
+        :return: All Files on this model as a list of :py:class:`File`.
+        """
+        return [
+            File.model_validate(e) for e in (await self._get(f"{self._url}/files")).get("files")
+        ]
 
     async def list_actions(self) -> list[Action]:
         """
         Lists all the Actions in the Model. This will only return the Actions listed under
         `Other Actions` in Anaplan. For Imports, exports, and processes, see their respective
         methods instead.
-
         :return: All Actions on this model as a list of :py:class:`Action`.
         """
-        return to_actions(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/actions")
-        )
-
-    async def list_imports(self) -> list[Import]:
-        """
-        Lists all the Imports in the Model.
-        :return: All Imports on this model as a list of :py:class:`Import`.
-        """
-        return to_imports(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/imports")
-        )
-
-    async def list_exports(self) -> list[Export]:
-        """
-        Lists all the Exports in the Model.
-        :return: All Exports on this model as a list of :py:class:`Export`.
-        """
-        return to_exports(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/exports")
-        )
+        return [
+            Action.model_validate(e)
+            for e in (await self._get(f"{self._url}/actions")).get("actions")
+        ]
 
     async def list_processes(self) -> list[Process]:
         """
         Lists all the Processes in the Model.
         :return: All Processes on this model as a list of :py:class:`Process`.
         """
-        return to_processes(
-            await self._get(
-                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/processes"
-            )
-        )
+        return [
+            Process.model_validate(e)
+            for e in (await self._get(f"{self._url}/processes")).get("processes")
+        ]
 
-    async def list_files(self) -> list[File]:
+    async def list_imports(self) -> list[Import]:
         """
-        Lists all the Files in the Model.
-        :return: All Files on this model as a list of :py:class:`File`.
+        Lists all the Imports in the Model.
+        :return: All Imports on this model as a list of :py:class:`Import`.
         """
-        return to_files(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files")
-        )
+        return [
+            Import.model_validate(e)
+            for e in (await self._get(f"{self._url}/imports")).get("imports")
+        ]
 
-    async def list_lists(self) -> list[List]:
+    async def list_exports(self) -> list[Export]:
         """
-        Lists all the Lists in the Model.
-        :return: All Lists on this model as a list of :py:class:`List`.
+        Lists all the Exports in the Model.
+        :return: All Exports on this model as a list of :py:class:`Export`.
         """
-        return to_lists(
-            await self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/lists")
-        )
+        return [
+            Export.model_validate(e)
+            for e in (await self._get(f"{self._url}/exports")).get("exports")
+        ]
 
     async def run_action(self, action_id: int) -> None:
         """
         Runs the specified Anaplan Action and validates the spawned task. If the Action fails or
         completes with errors, will raise an :py:class:`AnaplanActionError`. Failed Tasks are
         usually not something you can recover from at runtime and often require manual changes in
         Anaplan, i.e. updating the mapping of an Import or similar. So, for convenience, this will
@@ -228,17 +227,15 @@
 
     async def get_file(self, file_id: int) -> bytes:
         """
         Retrieves the content of the specified file.
         :param file_id: The identifier of the file to retrieve.
         :return: The content of the file.
         """
-        return await self._get_binary(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}"
-        )
+        return await self._get_binary(f"{self._url}/files/{file_id}")
 
     async def upload_file(self, file_id: int, content: str | bytes) -> None:
         """
         Uploads the content to the specified file. If there are several chunks, upload of
         individual chunks are concurrent.
 
         :param file_id: The identifier of the file to upload to.
@@ -265,78 +262,34 @@
         Retrieves the status of the specified task.
         :param action_id: The identifier of the action that was invoked.
         :param task_id: The identifier of the spawned task.
         :return: The status of the task as returned by the API. For more information
                  see: https://anaplan.docs.apiary.io.
         """
         return (
-            await self._get(
-                f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-                f"{determine_action_type(action_id)}/{action_id}/tasks/{task_id}"
-            )
+            await self._get(f"{self._url}/{action_url(action_id)}/{action_id}/tasks/{task_id}")
         ).get("task")
 
     async def invoke_action(self, action_id: int) -> str:
         """
         You may want to consider using `run_action()` instead.
 
         Invokes the specified Anaplan Action and returns the spawned Task identifier. This is
         useful if you want to handle the Task status yourself or if you want to run multiple
         Actions in parallel.
-        :param action_id:
-        :return:
+        :param action_id: The identifier of the Action to run. Can be any Anaplan Invokable.
+        :return: The identifier of the spawned Task.
         """
         response = await self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-            f"{determine_action_type(action_id)}/{action_id}/tasks",
-            json={"localeName": "en_US"},
+            f"{self._url}/{action_url(action_id)}/{action_id}/tasks", json={"localeName": "en_US"}
         )
         task_id = response.get("task").get("taskId")
         logger.info(f"Invoked Action '{action_id}', spawned Task: '{task_id}'.")
         return task_id
 
     async def _upload_chunk(self, file_id: int, index: int, chunk: bytes) -> None:
         await self._run_with_retry(
-            self._client.put,
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}/"
-            f"chunks/{index}",
-            headers={"Content-Type": "application/x-gzip"},
-            content=gzip.compress(chunk),
-            timeout=self.timeout,
+            self._put_binary_gzip, f"{self._url}/files/{file_id}/chunks/{index}", content=chunk
         )
 
     async def _set_chunk_count(self, file_id: int, num_chunks: int) -> None:
-        await self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}",
-            json={"chunkCount": num_chunks},
-        )
-
-    async def _get(self, url: str) -> dict[str, float | int | str | list | dict | bool]:
-        return (await self._run_with_retry(self._client.get, url, timeout=self.timeout)).json()
-
-    async def _get_binary(self, url: str) -> bytes:
-        return (await self._run_with_retry(self._client.get, url, timeout=self.timeout)).content
-
-    async def _post(
-        self, url: str, json: dict | None = None
-    ) -> dict[str, float | int | str | list | dict | bool]:
-        return (
-            await self._run_with_retry(
-                self._client.post,
-                url,
-                headers={"Content-Type": "application/json"},
-                json=json,
-                timeout=self.timeout,
-            )
-        ).json()
-
-    async def _run_with_retry(
-        self, func: Callable[..., Coroutine[Any, Any, Response]], *args, **kwargs
-    ) -> Response:
-        for i in range(max(self.retry_count, 1)):
-            try:
-                response = await func(*args, **kwargs)
-                response.raise_for_status()
-                return response
-            except HTTPError as error:
-                if i >= self.retry_count - 1:
-                    raise_appropriate_error(error)
+        await self._post(f"{self._url}/files/{file_id}", json={"chunkCount": num_chunks})
```

### Comparing `anaplan_sdk-0.1.0/anaplan_sdk/_auth.py` & `anaplan_sdk-0.1.1/anaplan_sdk/_auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,145 @@
 """
 Custom Authentication class to pass to httpx alongside some helper functions.
 """
 
-import base64
 import logging
 import os
+from base64 import b64encode
 
 import httpx
 from cryptography.exceptions import InvalidKey, UnsupportedAlgorithm
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
+from httpx import HTTPError
 
-from ._exceptions import InvalidPrivateKeyException, InvalidCredentialsException
+from .exceptions import InvalidPrivateKeyException, InvalidCredentialsException
 
 logger = logging.getLogger("anaplan_sdk")
 
 
 class AnaplanBasicAuth(httpx.Auth):
     requires_response_body = True
 
     def __init__(
         self,
         user_email: str,
         password: str,
     ):
-        self._token = "none"
         self._user_email = user_email
         self._password = password
+        self._token = self._init_token()
 
     def auth_flow(self, request):
         request.headers["Authorization"] = f"AnaplanAuthToken {self._token}"
         response = yield request
         if response.status_code == 401:
-            logger.info("Token expired or invalid, refreshing.")
+            logger.info("Token expired, refreshing.")
             response = yield self._basic_auth_request()
             if "tokenInfo" not in response.json():
                 raise InvalidCredentialsException
             self._token = response.json().get("tokenInfo").get("tokenValue")
             request.headers["Authorization"] = f"AnaplanAuthToken {self._token}"
             yield request
 
     def _basic_auth_request(self):
-        credentials = base64.b64encode(f"{self._user_email}:{self._password}".encode()).decode()
+        credentials = b64encode(f"{self._user_email}:{self._password}".encode()).decode()
         return httpx.Request(
             method="post",
             url="https://auth.anaplan.com/token/authenticate",
             headers={"Authorization": f"Basic {credentials}"},
         )
 
+    def _init_token(self) -> str:
+        try:
+            logger.info("Creating Authentication Token.")
+            credentials = b64encode(f"{self._user_email}:{self._password}".encode()).decode()
+            return (
+                httpx.post(
+                    url="https://auth.anaplan.com/token/authenticate",
+                    headers={"Authorization": f"Basic {credentials}"},
+                )
+                .json()
+                .get("tokenInfo")
+                .get("tokenValue")
+            )
+        except HTTPError as error:
+            raise InvalidCredentialsException from error
+
 
 class AnaplanCertAuth(httpx.Auth):
     requires_response_body = True
     requires_request_body = True
 
     def __init__(
         self,
         certificate: bytes,
         private_key: RSAPrivateKey,
     ):
-        self._token = "none"
         self._certificate = certificate
         self._private_key = private_key
+        self._token = self._init_token()
 
     def auth_flow(self, request):
         request.headers["Authorization"] = f"AnaplanAuthToken {self._token}"
         response = yield request
         if response.status_code == 401:
             logger.info("Token expired or invalid, refreshing.")
             response = yield self._cert_auth_request()
             if "tokenInfo" not in response.json():
                 raise InvalidCredentialsException
             self._token = response.json().get("tokenInfo").get("tokenValue")
             request.headers["Authorization"] = f"AnaplanAuthToken {self._token}"
             yield request
 
     def _cert_auth_request(self):
-        message = os.urandom(150)
-        encoded_cert = base64.b64encode(self._certificate).decode()
-        encoded_string = base64.b64encode(message).decode()
-        encoded_signed_string = base64.b64encode(
-            self._private_key.sign(message, padding.PKCS1v15(), hashes.SHA512())
-        ).decode()
+        encoded_cert, encoded_string, encoded_signed_string = self._prep_credentials()
         return httpx.Request(
             method="post",
             url="https://auth.anaplan.com/token/authenticate",
             headers={
                 "Authorization": f"CACertificate {encoded_cert}",
                 "Content-Type": "application/json",
             },
             json={"encodedData": encoded_string, "encodedSignedData": encoded_signed_string},
         )
 
+    def _init_token(self) -> str:
+        try:
+            logger.info("Creating Authentication Token.")
+            encoded_cert, encoded_string, encoded_signed_string = self._prep_credentials()
+            return (
+                httpx.post(
+                    url="https://auth.anaplan.com/token/authenticate",
+                    headers={
+                        "Authorization": f"CACertificate {encoded_cert}",
+                        "Content-Type": "application/json",
+                    },
+                    json={
+                        "encodedData": encoded_string,
+                        "encodedSignedData": encoded_signed_string,
+                    },
+                )
+                .json()
+                .get("tokenInfo")
+                .get("tokenValue")
+            )
+        except HTTPError as error:
+            raise InvalidCredentialsException from error
+
+    def _prep_credentials(self) -> tuple[str, str, str]:
+        message = os.urandom(150)
+        return (
+            b64encode(self._certificate).decode(),
+            b64encode(message).decode(),
+            b64encode(self._private_key.sign(message, PKCS1v15(), hashes.SHA512())).decode(),
+        )
+
 
 def get_certificate(certificate: str | bytes) -> bytes:
     """
     Get the certificate from a file or string.
     :param certificate: The certificate to use.
     :return: The certificate as bytes.
     """
```

### Comparing `anaplan_sdk-0.1.0/anaplan_sdk/_client.py` & `anaplan_sdk-0.1.1/anaplan_sdk/_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,31 @@
 """
 Synchronous Client.
 """
 
-import gzip
 import logging
 import time
 from concurrent.futures import ThreadPoolExecutor
-from typing import Callable
 
 import httpx
-from httpx import HTTPError, Response
 
 from ._auth import AnaplanBasicAuth, AnaplanCertAuth, get_certificate, get_private_key
-from ._exceptions import (
+from ._base import _BaseClient
+from ._transactional_client import _TransactionalClient
+from .exceptions import (
     AnaplanActionError,
-    raise_appropriate_error,
     InvalidIdentifierException,
 )
-from ._models import (
-    Import,
-    Export,
-    Process,
-    File,
-    Action,
-    List,
-    Workspace,
-    Model,
-    to_workspaces,
-    to_models,
-    to_actions,
-    to_imports,
-    to_exports,
-    to_processes,
-    to_files,
-    to_lists,
-    determine_action_type,
-)
+from .models import Import, Export, Process, File, Action, Workspace, Model, action_url
 
 logging.getLogger("httpx").setLevel(logging.CRITICAL)
 logger = logging.getLogger("anaplan_sdk")
 
 
-class Client:
+class Client(_BaseClient):
     """
     A synchronous Client for pythonic access to the Anaplan Integration API v2:
     https://anaplan.docs.apiary.io/. This Client provides high-level abstractions over the API, so
     you can deal with python objects and simple functions rather than implementation details like
     http, json, compression, chunking etc.
 
 
@@ -87,15 +67,15 @@
         :param password: Password for the given `user_email`. This is not suitable for production
                          setups. If you intend to use this in production, acquire a client
                          certificate as described under: https://help.anaplan.com/procure-ca-certificates-47842267-2cb3-4e38-90bf-13b1632bcd44
         :param certificate: The absolute path to the client certificate file or the certificate
                             itself.
         :param private_key: The absolute path to the private key file or the private key itself.
         :param private_key_password: The password to access the private key if there is one.
-        :param timeout: The timeout for the HTTP requests.
+        :param timeout: The timeout in seconds for the HTTP requests.
         :param retry_count: The number of times to retry an HTTP request if it fails. Set this to 0
                             to never retry. Defaults to 2, meaning each HTTP Operation will be
                             tried a total number of 2 times.
         :param status_poll_delay: The delay between polling the status of a task.
         :param upload_parallel: Whether to upload the chunks in parallel. Defaults to True. **If
                                 you are heavily network bound or are experiencing rate limiting
                                 issues, set this to False.**
@@ -109,104 +89,120 @@
                                     creating new files and uploading content to them.
         """
         if not ((user_email and password) or (certificate and private_key)):
             raise ValueError(
                 "Either `certificate` and `private_key` or `user_email` and `password` must be "
                 "provided."
             )
-        auth = (
-            AnaplanCertAuth(
-                get_certificate(certificate), get_private_key(private_key, private_key_password)
-            )
-            if certificate
-            else AnaplanBasicAuth(user_email=user_email, password=password)
+        client = httpx.Client(
+            auth=(
+                AnaplanCertAuth(
+                    get_certificate(certificate), get_private_key(private_key, private_key_password)
+                )
+                if certificate
+                else AnaplanBasicAuth(user_email=user_email, password=password)
+            ),
+            timeout=timeout,
+        )
+        self._url = f"https://api.anaplan.com/2/0/workspaces/{workspace_id}/models/{model_id}"
+        self._transactional_client = (
+            _TransactionalClient(client, model_id, retry_count) if model_id else None
         )
-        self._client = httpx.Client(auth=auth)
-        self._base_url = "https://api.anaplan.com/2/0/workspaces"
-        self.workspace_id = workspace_id
-        self.model_id = model_id
-        self.timeout = timeout
-        self.retry_count = retry_count
         self.status_poll_delay = status_poll_delay
         self.upload_parallel = upload_parallel
         self.upload_chunk_size = upload_chunk_size
         self.allow_file_creation = allow_file_creation
+        super().__init__(retry_count, client)
+
+    @property
+    def transactional(self) -> _TransactionalClient:
+        """
+        The Transactional Client provides access to the Anaplan Transactional API. This is useful
+        for more advanced use cases where you need to interact with the Anaplan Model in a more
+        granular way.
+
+        If you instantiated the client without the field `model_id`, this will raise a
+        :py:class:`ValueError`, since none of the endpoints can be invoked without the model Id.
+        :return: The Transactional Client.
+        """
+        if not self._transactional_client:
+            raise ValueError(
+                "Cannot use the Transactional Client (Anaplan Transactional API) "
+                "without field `model_id`. Make sure the instance you are trying to call this on "
+                "is instantiated correctly with a valid `model_id`."
+            )
+        return self._transactional_client
 
     def list_workspaces(self) -> list[Workspace]:
         """
         Lists all the Workspaces the authenticated user has access to.
         :return: All Workspaces as a list of :py:class:`Workspace`.
         """
-        return to_workspaces(self._get(f"{self._base_url}?tenantDetails=true"))
+        return [
+            Workspace.model_validate(e)
+            for e in self._get("https://api.anaplan.com/2/0/workspaces?tenantDetails=true").get(
+                "workspaces"
+            )
+        ]
 
     def list_models(self) -> list[Model]:
         """
         Lists all the Models the authenticated user has access to.
         :return: All Models in the Workspace as a list of :py:class:`Model`.
         """
-        return to_models(
-            self._get(f"{self._base_url.replace('/workspaces', '/models')}?modelDetails=true")
-        )
+        return [
+            Model.model_validate(e)
+            for e in self._get("https://api.anaplan.com/2/0/models?modelDetails=true").get("models")
+        ]
+
+    def list_files(self) -> list[File]:
+        """
+        Lists all the Files in the Model.
+        :return: All Files on this model as a list of :py:class:`File`.
+        """
+        return [File.model_validate(e) for e in self._get(f"{self._url}/files").get("files")]
 
     def list_actions(self) -> list[Action]:
         """
         Lists all the Actions in the Model. This will only return the Actions listed under
         `Other Actions` in Anaplan. For Imports, exports, and processes, see their respective
         methods instead.
-
         :return: All Actions on this model as a list of :py:class:`Action`.
         """
-        return to_actions(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/actions")
-        )
-
-    def list_imports(self) -> list[Import]:
-        """
-        Lists all the Imports in the Model.
-        :return: All Imports on this model as a list of :py:class:`Import`.
-        """
-        return to_imports(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/imports")
-        )
-
-    def list_exports(self) -> list[Export]:
-        """
-        Lists all the Exports in the Model.
-        :return: All Exports on this model as a list of :py:class:`Export`.
-        """
-        return to_exports(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/exports")
-        )
+        return [
+            Action.model_validate(e) for e in (self._get(f"{self._url}/actions")).get("actions")
+        ]
 
     def list_processes(self) -> list[Process]:
         """
         Lists all the Processes in the Model.
         :return: All Processes on this model as a list of :py:class:`Process`.
         """
-        return to_processes(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/processes")
-        )
+        return [
+            Process.model_validate(e)
+            for e in (self._get(f"{self._url}/processes")).get("processes")
+        ]
 
-    def list_files(self) -> list[File]:
+    def list_imports(self) -> list[Import]:
         """
-        Lists all the Files in the Model.
-        :return: All Files on this model as a list of :py:class:`File`.
+        Lists all the Imports in the Model.
+        :return: All Imports on this model as a list of :py:class:`Import`.
         """
-        return to_files(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files")
-        )
+        return [
+            Import.model_validate(e) for e in (self._get(f"{self._url}/imports")).get("imports")
+        ]
 
-    def list_lists(self) -> list[List]:
+    def list_exports(self) -> list[Export]:
         """
-        Lists all the Lists in the Model.
-        :return: All Lists on this model as a list of :py:class:`List`.
+        Lists all the Exports in the Model.
+        :return: All Exports on this model as a list of :py:class:`Export`.
         """
-        return to_lists(
-            self._get(f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/lists")
-        )
+        return [
+            Export.model_validate(e) for e in (self._get(f"{self._url}/exports")).get("exports")
+        ]
 
     def run_action(self, action_id: int) -> None:
         """
         Runs the specified Anaplan Action and validates the spawned task. If the Action fails or
         completes with errors, will raise an :py:class:`AnaplanActionError`. Failed Tasks are
         usually not something you can recover from at runtime and often require manual changes in
         Anaplan, i.e. updating the mapping of an Import or similar. So, for convenience, this will
@@ -233,17 +229,15 @@
 
     def get_file(self, file_id: int) -> bytes:
         """
         Retrieves the content of the specified file.
         :param file_id: The identifier of the file to retrieve.
         :return: The content of the file.
         """
-        return self._get_binary(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}"
-        )
+        return self._get_binary(f"{self._url}/files/{file_id}")
 
     def upload_file(self, file_id: int, content: str | bytes) -> None:
         """
         Uploads the content to the specified file. If `upload_parallel` is set to True on the
         instance you are invoking this from, will attempt to upload the chunks in parallel for
         better performance. If you are network bound or are experiencing rate limiting issues, set
         `upload_parallel` to False.
@@ -276,92 +270,51 @@
         """
         Retrieves the status of the specified task.
         :param action_id: The identifier of the action that was invoked.
         :param task_id: The identifier of the spawned task.
         :return: The status of the task as returned by the API. For more information
                  see: https://anaplan.docs.apiary.io.
         """
-        return self._get(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-            f"{determine_action_type(action_id)}/{action_id}/tasks/{task_id}"
-        ).get("task")
+        return self._get(f"{self._url}/{action_url(action_id)}/{action_id}/tasks/{task_id}").get(
+            "task"
+        )
 
     def invoke_action(self, action_id: int) -> str:
         """
         You may want to consider using `run_action()` instead.
 
         Invokes the specified Anaplan Action and returns the spawned Task identifier. This is
         useful if you want to handle the Task status yourself or if you want to run multiple
         Actions in parallel.
-        :param action_id:
-        :return:
+        :param action_id: The identifier of the Action to run. Can be any Anaplan Invokable.
+        :return: The identifier of the spawned Task.
         """
         response = self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/"
-            f"{determine_action_type(action_id)}/{action_id}/tasks",
+            f"{self._url}/{action_url(action_id)}/{action_id}/tasks",
             json={"localeName": "en_US"},
         )
         task_id = response.get("task").get("taskId")
         logger.info(f"Invoked Action '{action_id}', spawned Task: '{task_id}'.")
         return task_id
 
     def _upload_chunk(self, file_id: int, index: int, chunk: bytes) -> None:
-        self._run_with_retry(
-            self._client.put,
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}/"
-            f"chunks/{index}",
-            headers={"Content-Type": "application/x-gzip"},
-            content=gzip.compress(chunk),
-            timeout=self.timeout,
-        )
+        self._put_binary_gzip(f"{self._url}/files/{file_id}/chunks/{index}", content=chunk)
 
     def _set_chunk_count(self, file_id: int, num_chunks: int) -> None:
         if not self.allow_file_creation and not (113000000000 <= file_id <= 113999999999):
             raise InvalidIdentifierException(
                 f"File with Id {file_id} does not exist. If you want to dynamically create files "
                 "to avoid this error, set `allow_file_creation=True` on the calling instance. "
                 "Make sure you have understood the implications of this before doing so. "
             )
-        response = self._post(
-            f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}",
-            json={"chunkCount": num_chunks},
-        )
+        response = self._post(f"{self._url}/files/{file_id}", json={"chunkCount": num_chunks})
         optionally_new_file = int(response.get("file").get("id"))
         if optionally_new_file != file_id:
             if self.allow_file_creation:
                 logger.info(f"Created new file with name '{file_id}', Id is {optionally_new_file}.")
                 return
             raise InvalidIdentifierException(
                 f"File with Id {file_id} did not exist and was created in Anaplan. You may want to "
                 f"ask a model builder to remove it. If you want to dynamically create files "
                 "to avoid this error, set `allow_file_creation=True` on the calling instance. "
                 "Make sure you have understood the implications of this before doing so."
             )
-
-    def _get(self, url: str) -> dict[str, float | int | str | list | dict | bool]:
-        return self._run_with_retry(self._client.get, url, timeout=self.timeout).json()
-
-    def _get_binary(self, url: str) -> bytes:
-        return self._run_with_retry(self._client.get, url, timeout=self.timeout).content
-
-    def _post(
-        self, url: str, json: dict | None = None
-    ) -> dict[str, float | int | str | list | dict | bool]:
-        return self._run_with_retry(
-            self._client.post,
-            url,
-            headers={"Content-Type": "application/json"},
-            json=json,
-            timeout=self.timeout,
-        ).json()
-
-    def _run_with_retry(self, func: Callable[..., Response], *args, **kwargs) -> Response:
-        for i in range(max(self.retry_count, 1)):
-            try:
-                response = func(*args, **kwargs)
-                response.raise_for_status()
-                return response
-            except HTTPError as error:
-                url = args[0] or kwargs.get("url")
-                if i >= self.retry_count - 1:
-                    raise_appropriate_error(error)
-                logger.info(f"Retrying for: {url}")
```

### Comparing `anaplan_sdk-0.1.0/anaplan_sdk/_exceptions.py` & `anaplan_sdk-0.1.1/anaplan_sdk/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,8 +51,8 @@
         super().__init__(self.message)
 
 
 def raise_appropriate_error(error: HTTPError) -> None:
     if isinstance(error, HTTPStatusError):
         if error.response.status_code == 404:
             raise InvalidIdentifierException from error
-    raise error
+    raise AnaplanException from error
```

### Comparing `anaplan_sdk-0.1.0/LICENSE` & `anaplan_sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.1.0/pyproject.toml` & `anaplan_sdk-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anaplan-sdk"
-version = "0.1.0"
+version = "0.1.1"
 description = "Provides pythonic access to the Anaplan API"
 license = "Apache-2.0"
 authors = ["Vinzenz Klass <vinzenz.klass@ba.valantic.com>"]
 readme = "README.md"
 homepage = "https://vinzenzklass.github.io/anaplan-sdk/"
 repository = "https://github.com/VinzenzKlass/anaplan-sdk"
 documentation = "https://vinzenzklass.github.io/anaplan-sdk/"
@@ -17,14 +17,15 @@
 cryptography = "^42.0.7"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.5"
 pre-commit = "^3.6.1"
 pytest = "^8.2.1"
 pytest-asyncio = "^0.16.0"
+pytest-xdist = "^3.6.1"
 mkdocs = "^1.6.0"
 mkdocs-material = "^9.5.25"
 mkdocstrings = { extras = ["python"], version = "^0.25.1" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `anaplan_sdk-0.1.0/README.md` & `anaplan_sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.1.0/PKG-INFO` & `anaplan_sdk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anaplan-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Provides pythonic access to the Anaplan API
 Home-page: https://vinzenzklass.github.io/anaplan-sdk/
 License: Apache-2.0
 Keywords: anaplan,anaplan-api,anaplan-bulk-api,anaplan integration
 Author: Vinzenz Klass
 Author-email: vinzenz.klass@ba.valantic.com
 Requires-Python: >=3.10.4
```

