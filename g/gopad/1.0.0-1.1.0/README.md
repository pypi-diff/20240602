# Comparing `tmp/gopad-1.0.0.tar.gz` & `tmp/gopad-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopad-1.0.0.tar", max compression
+gzip compressed data, was "gopad-1.1.0.tar", max compression
```

## Comparing `gopad-1.0.0.tar` & `gopad-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,33 @@
--rw-r--r--   0        0        0    11358 2024-05-27 19:02:11.209372 gopad-1.0.0/LICENSE
--rw-r--r--   0        0        0     1764 2024-05-27 19:02:39.681625 gopad-1.0.0/README.md
--rw-r--r--   0        0        0     1478 2024-05-27 19:02:39.693625 gopad-1.0.0/gopad/__init__.py
--rw-r--r--   0        0        0      165 2024-05-27 19:02:39.697625 gopad-1.0.0/gopad/api/__init__.py
--rw-r--r--   0        0        0    23088 2024-05-27 19:02:39.641625 gopad-1.0.0/gopad/api/auth_api.py
--rw-r--r--   0        0        0   104072 2024-05-27 19:02:39.657625 gopad-1.0.0/gopad/api/team_api.py
--rw-r--r--   0        0        0   104072 2024-05-27 19:02:39.673625 gopad-1.0.0/gopad/api/user_api.py
--rw-r--r--   0        0        0    26277 2024-05-27 19:02:39.705625 gopad-1.0.0/gopad/api_client.py
--rw-r--r--   0        0        0      652 2024-05-27 19:02:39.705625 gopad-1.0.0/gopad/api_response.py
--rw-r--r--   0        0        0    16285 2024-05-27 19:02:39.693625 gopad-1.0.0/gopad/configuration.py
--rw-r--r--   0        0        0     5966 2024-05-27 19:02:39.697625 gopad-1.0.0/gopad/exceptions.py
--rw-r--r--   0        0        0      898 2024-05-27 19:02:39.697625 gopad-1.0.0/gopad/models/__init__.py
--rw-r--r--   0        0        0     3156 2024-05-27 19:02:39.409623 gopad-1.0.0/gopad/models/notification.py
--rw-r--r--   0        0        0     4350 2024-05-27 19:02:39.425623 gopad-1.0.0/gopad/models/team.py
--rw-r--r--   0        0        0     2920 2024-05-27 19:02:39.437623 gopad-1.0.0/gopad/models/team_user_params.py
--rw-r--r--   0        0        0     3326 2024-05-27 19:02:39.445623 gopad-1.0.0/gopad/models/team_users.py
--rw-r--r--   0        0        0     2982 2024-05-27 19:02:39.453623 gopad-1.0.0/gopad/models/teams.py
--rw-r--r--   0        0        0     6717 2024-05-27 19:02:39.461623 gopad-1.0.0/gopad/models/user.py
--rw-r--r--   0        0        0     2975 2024-05-27 19:02:39.469623 gopad-1.0.0/gopad/models/user_auth.py
--rw-r--r--   0        0        0     4090 2024-05-27 19:02:39.477623 gopad-1.0.0/gopad/models/user_team.py
--rw-r--r--   0        0        0     2920 2024-05-27 19:02:39.485623 gopad-1.0.0/gopad/models/user_team_params.py
--rw-r--r--   0        0        0     3326 2024-05-27 19:02:39.489623 gopad-1.0.0/gopad/models/user_teams.py
--rw-r--r--   0        0        0     2982 2024-05-27 19:02:39.497623 gopad-1.0.0/gopad/models/users.py
--rw-r--r--   0        0        0     2649 2024-05-27 19:02:39.505623 gopad-1.0.0/gopad/models/validation.py
--rw-r--r--   0        0        0        0 2024-05-27 19:02:39.689625 gopad-1.0.0/gopad/py.typed
--rw-r--r--   0        0        0     9393 2024-05-27 19:02:39.709625 gopad-1.0.0/gopad/rest.py
--rw-r--r--   0        0        0     1468 2024-05-27 19:02:48.501703 gopad-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 gopad-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-06-02 20:54:26.294689 gopad-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1764 2024-06-02 20:54:47.154484 gopad-1.1.0/README.md
+-rw-r--r--   0        0        0     1704 2024-06-02 20:54:47.154484 gopad-1.1.0/gopad/__init__.py
+-rw-r--r--   0        0        0      210 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/api/__init__.py
+-rw-r--r--   0        0        0    52337 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/api/auth_api.py
+-rw-r--r--   0        0        0    30258 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/api/profile_api.py
+-rw-r--r--   0        0        0   104279 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/api/team_api.py
+-rw-r--r--   0        0        0   104279 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/api/user_api.py
+-rw-r--r--   0        0        0    26277 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/api_client.py
+-rw-r--r--   0        0        0      652 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/api_response.py
+-rw-r--r--   0        0        0    16533 2024-06-02 20:54:47.158484 gopad-1.1.0/gopad/configuration.py
+-rw-r--r--   0        0        0     5966 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/exceptions.py
+-rw-r--r--   0        0        0     1079 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/__init__.py
+-rw-r--r--   0        0        0     2554 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/auth_login.py
+-rw-r--r--   0        0        0     2965 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/auth_token.py
+-rw-r--r--   0        0        0     2984 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/auth_verify.py
+-rw-r--r--   0        0        0     3156 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/notification.py
+-rw-r--r--   0        0        0     6383 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/profile.py
+-rw-r--r--   0        0        0     4350 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/team.py
+-rw-r--r--   0        0        0     2965 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/team_user_params.py
+-rw-r--r--   0        0        0     3326 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/team_users.py
+-rw-r--r--   0        0        0     2982 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/teams.py
+-rw-r--r--   0        0        0     6717 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/user.py
+-rw-r--r--   0        0        0     2975 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/user_auth.py
+-rw-r--r--   0        0        0     4135 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/user_team.py
+-rw-r--r--   0        0        0     2965 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/user_team_params.py
+-rw-r--r--   0        0        0     3326 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/user_teams.py
+-rw-r--r--   0        0        0     2982 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/users.py
+-rw-r--r--   0        0        0     2649 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/models/validation.py
+-rw-r--r--   0        0        0        0 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/py.typed
+-rw-r--r--   0        0        0     9393 2024-06-02 20:54:26.298689 gopad-1.1.0/gopad/rest.py
+-rw-r--r--   0        0        0     1468 2024-06-02 20:54:52.818430 gopad-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 gopad-1.1.0/PKG-INFO
```

### Comparing `gopad-1.0.0/LICENSE` & `gopad-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/README.md` & `gopad-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![General Workflow](https://github.com/gopad/gopad-python/actions/workflows/general.yml/badge.svg)](https://github.com/gopad/gopad-python/actions/workflows/general.yml) [![Join the Matrix chat at https://matrix.to/#/#gopad:matrix.org](https://img.shields.io/badge/matrix-%23gopad%3Amatrix.org-7bc9a4.svg)](https://matrix.to/#/#gopad:matrix.org) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/0581d0652d4d4dddb3fc353f74cd9bed)](https://app.codacy.com/gh/gopad/gopad-python/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![PyPI Version](https://badge.fury.io/py/gopad.svg)](https://badge.fury.io/py/gopad)
 
 This repository provides a client SDK for Python. This SDK is automatically
 generated by the [OpenAPI Generator][generator] project:
 
 -   API version: 1.0.0-alpha1
--   Package version: 1.0.0
+-   Package version: 1.1.0
 -   Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://gopad.eu](https://gopad.eu)
 
 ## Requirements
 
 Python 3.7+
@@ -18,15 +18,15 @@
 ## Installation
 
 If you want to use one of the versions released via PyPi you just need to
 execute the following command within your project directory, after that you can
 import it as other libraries:
 
 ```console
-pip install gopad@1.0.0
+pip install gopad@1.1.0
 ```
 
 ## Tests
 
 ```console
 pytest
 ```
```

### Comparing `gopad-1.0.0/gopad/__init__.py` & `gopad-1.1.0/gopad/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     Contact: gopad@webhippie.de
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 # import apis into sdk package
 from gopad.api.auth_api import AuthApi
+from gopad.api.profile_api import ProfileApi
 from gopad.api.team_api import TeamApi
 from gopad.api.user_api import UserApi
 
 # import ApiClient
 from gopad.api_response import ApiResponse
 from gopad.api_client import ApiClient
 from gopad.configuration import Configuration
@@ -30,15 +31,19 @@
 from gopad.exceptions import ApiTypeError
 from gopad.exceptions import ApiValueError
 from gopad.exceptions import ApiKeyError
 from gopad.exceptions import ApiAttributeError
 from gopad.exceptions import ApiException
 
 # import models into sdk package
+from gopad.models.auth_login import AuthLogin
+from gopad.models.auth_token import AuthToken
+from gopad.models.auth_verify import AuthVerify
 from gopad.models.notification import Notification
+from gopad.models.profile import Profile
 from gopad.models.team import Team
 from gopad.models.team_user_params import TeamUserParams
 from gopad.models.team_users import TeamUsers
 from gopad.models.teams import Teams
 from gopad.models.user import User
 from gopad.models.user_auth import UserAuth
 from gopad.models.user_team import UserTeam
```

### Comparing `gopad-1.0.0/gopad/api/auth_api.py` & `gopad-1.1.0/gopad/api/profile_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,65 +13,56 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr
-from typing import Optional
+from pydantic import Field
 from typing_extensions import Annotated
-from gopad.models.notification import Notification
+from gopad.models.auth_token import AuthToken
+from gopad.models.profile import Profile
 
 from gopad.api_client import ApiClient, RequestSerialized
 from gopad.api_response import ApiResponse
 from gopad.rest import RESTResponseType
 
 
-class AuthApi:
+class ProfileApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def external_callback(
+    def show_profile(
         self,
-        provider: Annotated[StrictStr, Field(description="An identifier for the auth provider")],
-        state: Annotated[Optional[StrictStr], Field(description="Auth state")] = None,
-        code: Annotated[Optional[StrictStr], Field(description="Auth code")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Notification:
-        """Callback for external authentication
+    ) -> Profile:
+        """Fetch profile details of the personal account
 
 
-        :param provider: An identifier for the auth provider (required)
-        :type provider: str
-        :param state: Auth state
-        :type state: str
-        :param code: Auth code
-        :type code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -86,68 +77,56 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._external_callback_serialize(
-            provider=provider,
-            state=state,
-            code=code,
+        _param = self._show_profile_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '307': None,
-            '404': "Notification",
-            '412': "Notification",
+            '200': "Profile",
+            '403': "Notification",
+            '500': "Notification",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def external_callback_with_http_info(
+    def show_profile_with_http_info(
         self,
-        provider: Annotated[StrictStr, Field(description="An identifier for the auth provider")],
-        state: Annotated[Optional[StrictStr], Field(description="Auth state")] = None,
-        code: Annotated[Optional[StrictStr], Field(description="Auth code")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Notification]:
-        """Callback for external authentication
+    ) -> ApiResponse[Profile]:
+        """Fetch profile details of the personal account
 
 
-        :param provider: An identifier for the auth provider (required)
-        :type provider: str
-        :param state: Auth state
-        :type state: str
-        :param code: Auth code
-        :type code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -162,68 +141,56 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._external_callback_serialize(
-            provider=provider,
-            state=state,
-            code=code,
+        _param = self._show_profile_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '307': None,
-            '404': "Notification",
-            '412': "Notification",
+            '200': "Profile",
+            '403': "Notification",
+            '500': "Notification",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def external_callback_without_preload_content(
+    def show_profile_without_preload_content(
         self,
-        provider: Annotated[StrictStr, Field(description="An identifier for the auth provider")],
-        state: Annotated[Optional[StrictStr], Field(description="Auth state")] = None,
-        code: Annotated[Optional[StrictStr], Field(description="Auth code")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Callback for external authentication
+        """Fetch profile details of the personal account
 
 
-        :param provider: An identifier for the auth provider (required)
-        :type provider: str
-        :param state: Auth state
-        :type state: str
-        :param code: Auth code
-        :type code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -238,41 +205,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._external_callback_serialize(
-            provider=provider,
-            state=state,
-            code=code,
+        _param = self._show_profile_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '307': None,
-            '404': "Notification",
-            '412': "Notification",
+            '200': "Profile",
+            '403': "Notification",
+            '500': "Notification",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _external_callback_serialize(
+    def _show_profile_serialize(
         self,
-        provider,
-        state,
-        code,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -284,25 +245,15 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if provider is not None:
-            _path_params['provider'] = provider
         # process the query parameters
-        if state is not None:
-            
-            _query_params.append(('state', state))
-            
-        if code is not None:
-            
-            _query_params.append(('code', code))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -310,19 +261,23 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'Cookie', 
+            'Basic', 
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/auth/{provider}/callback',
+            resource_path='/profile/self',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -331,38 +286,32 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def external_initialize(
+    def token_profile(
         self,
-        provider: Annotated[StrictStr, Field(description="An identifier for the auth provider")],
-        state: Annotated[Optional[StrictStr], Field(description="Auth state")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Notification:
-        """Initialize the external authentication
+    ) -> AuthToken:
+        """Retrieve an unlimited auth token
 
 
-        :param provider: An identifier for the auth provider (required)
-        :type provider: str
-        :param state: Auth state
-        :type state: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -377,64 +326,56 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._external_initialize_serialize(
-            provider=provider,
-            state=state,
+        _param = self._token_profile_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '307': None,
-            '404': "Notification",
-            '412': "Notification",
+            '200': "AuthToken",
+            '403': "Notification",
+            '500': "Notification",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def external_initialize_with_http_info(
+    def token_profile_with_http_info(
         self,
-        provider: Annotated[StrictStr, Field(description="An identifier for the auth provider")],
-        state: Annotated[Optional[StrictStr], Field(description="Auth state")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Notification]:
-        """Initialize the external authentication
+    ) -> ApiResponse[AuthToken]:
+        """Retrieve an unlimited auth token
 
 
-        :param provider: An identifier for the auth provider (required)
-        :type provider: str
-        :param state: Auth state
-        :type state: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -449,64 +390,56 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._external_initialize_serialize(
-            provider=provider,
-            state=state,
+        _param = self._token_profile_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '307': None,
-            '404': "Notification",
-            '412': "Notification",
+            '200': "AuthToken",
+            '403': "Notification",
+            '500': "Notification",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def external_initialize_without_preload_content(
+    def token_profile_without_preload_content(
         self,
-        provider: Annotated[StrictStr, Field(description="An identifier for the auth provider")],
-        state: Annotated[Optional[StrictStr], Field(description="Auth state")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Initialize the external authentication
+        """Retrieve an unlimited auth token
 
 
-        :param provider: An identifier for the auth provider (required)
-        :type provider: str
-        :param state: Auth state
-        :type state: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -521,39 +454,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._external_initialize_serialize(
-            provider=provider,
-            state=state,
+        _param = self._token_profile_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '307': None,
-            '404': "Notification",
-            '412': "Notification",
+            '200': "AuthToken",
+            '403': "Notification",
+            '500': "Notification",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _external_initialize_serialize(
+    def _token_profile_serialize(
         self,
-        provider,
-        state,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -565,21 +494,15 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if provider is not None:
-            _path_params['provider'] = provider
         # process the query parameters
-        if state is not None:
-            
-            _query_params.append(('state', state))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -587,19 +510,299 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'Cookie', 
+            'Basic', 
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/auth/{provider}/initialize',
+            resource_path='/profile/token',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def update_profile(
+        self,
+        profile: Annotated[Profile, Field(description="The profile data to update")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Profile:
+        """Update your own profile information
+
+
+        :param profile: The profile data to update (required)
+        :type profile: Profile
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._update_profile_serialize(
+            profile=profile,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Profile",
+            '403': "Notification",
+            '422': "Notification",
+            '500': "Notification",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def update_profile_with_http_info(
+        self,
+        profile: Annotated[Profile, Field(description="The profile data to update")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[Profile]:
+        """Update your own profile information
+
+
+        :param profile: The profile data to update (required)
+        :type profile: Profile
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._update_profile_serialize(
+            profile=profile,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Profile",
+            '403': "Notification",
+            '422': "Notification",
+            '500': "Notification",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def update_profile_without_preload_content(
+        self,
+        profile: Annotated[Profile, Field(description="The profile data to update")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Update your own profile information
+
+
+        :param profile: The profile data to update (required)
+        :type profile: Profile
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._update_profile_serialize(
+            profile=profile,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Profile",
+            '403': "Notification",
+            '422': "Notification",
+            '500': "Notification",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _update_profile_serialize(
+        self,
+        profile,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if profile is not None:
+            _body_params = profile
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='PUT',
+            resource_path='/profile/self',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `gopad-1.0.0/gopad/api/team_api.py` & `gopad-1.1.0/gopad/api/team_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/teams/{team_id}/users',
             path_params=_path_params,
             query_params=_query_params,
@@ -598,15 +599,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/teams',
             path_params=_path_params,
             query_params=_query_params,
@@ -867,15 +869,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
             resource_path='/teams/{team_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -1164,15 +1167,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
             resource_path='/teams/{team_id}/users',
             path_params=_path_params,
             query_params=_query_params,
@@ -1515,15 +1519,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/teams/{team_id}/users',
             path_params=_path_params,
             query_params=_query_params,
@@ -1848,15 +1853,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/teams',
             path_params=_path_params,
             query_params=_query_params,
@@ -2148,15 +2154,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
             resource_path='/teams/{team_id}/users',
             path_params=_path_params,
             query_params=_query_params,
@@ -2414,15 +2421,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/teams/{team_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -2711,15 +2719,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
             resource_path='/teams/{team_id}',
             path_params=_path_params,
             query_params=_query_params,
```

### Comparing `gopad-1.0.0/gopad/api/user_api.py` & `gopad-1.1.0/gopad/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/users/{user_id}/teams',
             path_params=_path_params,
             query_params=_query_params,
@@ -598,15 +599,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
             resource_path='/users',
             path_params=_path_params,
             query_params=_query_params,
@@ -867,15 +869,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
             resource_path='/users/{user_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -1164,15 +1167,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
             resource_path='/users/{user_id}/teams',
             path_params=_path_params,
             query_params=_query_params,
@@ -1515,15 +1519,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/users/{user_id}/teams',
             path_params=_path_params,
             query_params=_query_params,
@@ -1848,15 +1853,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/users',
             path_params=_path_params,
             query_params=_query_params,
@@ -2148,15 +2154,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
             resource_path='/users/{user_id}/teams',
             path_params=_path_params,
             query_params=_query_params,
@@ -2414,15 +2421,16 @@
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
             resource_path='/users/{user_id}',
             path_params=_path_params,
             query_params=_query_params,
@@ -2711,15 +2719,16 @@
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'Cookie', 
             'Basic', 
-            'Header'
+            'Header', 
+            'Bearer'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
             resource_path='/users/{user_id}',
             path_params=_path_params,
             query_params=_query_params,
```

### Comparing `gopad-1.0.0/gopad/api_client.py` & `gopad-1.1.0/gopad/api_client.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/api_response.py` & `gopad-1.1.0/gopad/api_response.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/configuration.py` & `gopad-1.1.0/gopad/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,51 +392,58 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
-        if 'Cookie' in self.api_key:
-            auth['Cookie'] = {
-                'type': 'api_key',
-                'in': 'header',
-                'key': 'Cookie',
-                'value': self.get_api_key_with_prefix(
-                    'Cookie',
-                ),
-            }
         if 'Header' in self.api_key:
             auth['Header'] = {
                 'type': 'api_key',
                 'in': 'header',
                 'key': 'X-API-Key',
                 'value': self.get_api_key_with_prefix(
                     'Header',
                 ),
             }
+        if self.access_token is not None:
+            auth['Bearer'] = {
+                'type': 'bearer',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
+            }
         if self.username is not None and self.password is not None:
             auth['Basic'] = {
                 'type': 'basic',
                 'in': 'header',
                 'key': 'Authorization',
                 'value': self.get_basic_auth_token()
             }
+        if 'Cookie' in self.api_key:
+            auth['Cookie'] = {
+                'type': 'api_key',
+                'in': 'header',
+                'key': 'Cookie',
+                'value': self.get_api_key_with_prefix(
+                    'Cookie',
+                ),
+            }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0-alpha1\n"\
-               "SDK Package Version: 1.0.0".\
+               "SDK Package Version: 1.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `gopad-1.0.0/gopad/exceptions.py` & `gopad-1.1.0/gopad/exceptions.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/__init__.py` & `gopad-1.1.0/gopad/models/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,19 @@
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
+from gopad.models.auth_login import AuthLogin
+from gopad.models.auth_token import AuthToken
+from gopad.models.auth_verify import AuthVerify
 from gopad.models.notification import Notification
+from gopad.models.profile import Profile
 from gopad.models.team import Team
 from gopad.models.team_user_params import TeamUserParams
 from gopad.models.team_users import TeamUsers
 from gopad.models.teams import Teams
 from gopad.models.user import User
 from gopad.models.user_auth import UserAuth
 from gopad.models.user_team import UserTeam
```

### Comparing `gopad-1.0.0/gopad/models/notification.py` & `gopad-1.1.0/gopad/models/notification.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/team.py` & `gopad-1.1.0/gopad/models/team.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/team_user_params.py` & `gopad-1.1.0/gopad/models/team_user_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class TeamUserParams(BaseModel):
     """
     Parameters to attach or remove team user
     """ # noqa: E501
     user: StrictStr
-    perm: Optional[StrictStr] = None
+    perm: Optional[StrictStr] = 'user'
     __properties: ClassVar[List[str]] = ["user", "perm"]
 
     @field_validator('perm')
     def perm_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -89,12 +89,12 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "user": obj.get("user"),
-            "perm": obj.get("perm")
+            "perm": obj.get("perm") if obj.get("perm") is not None else 'user'
         })
         return _obj
```

### Comparing `gopad-1.0.0/gopad/models/team_users.py` & `gopad-1.1.0/gopad/models/team_users.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/teams.py` & `gopad-1.1.0/gopad/models/teams.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/user.py` & `gopad-1.1.0/gopad/models/user.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/user_auth.py` & `gopad-1.1.0/gopad/models/user_auth.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/user_team.py` & `gopad-1.1.0/gopad/models/user_team.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     Model to represent user team
     """ # noqa: E501
     user_id: StrictStr
     user: Optional[User] = None
     team_id: StrictStr
     team: Optional[Team] = None
-    perm: Optional[StrictStr] = None
+    perm: Optional[StrictStr] = 'user'
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
     __properties: ClassVar[List[str]] = ["user_id", "user", "team_id", "team", "perm", "created_at", "updated_at"]
 
     @field_validator('perm')
     def perm_validate_enum(cls, value):
         """Validates the enum"""
@@ -108,15 +108,15 @@
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "user_id": obj.get("user_id"),
             "user": User.from_dict(obj["user"]) if obj.get("user") is not None else None,
             "team_id": obj.get("team_id"),
             "team": Team.from_dict(obj["team"]) if obj.get("team") is not None else None,
-            "perm": obj.get("perm"),
+            "perm": obj.get("perm") if obj.get("perm") is not None else 'user',
             "created_at": obj.get("created_at"),
             "updated_at": obj.get("updated_at")
         })
         return _obj
 
 from gopad.models.team import Team
 from gopad.models.user import User
```

### Comparing `gopad-1.0.0/gopad/models/user_team_params.py` & `gopad-1.1.0/gopad/models/user_team_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class UserTeamParams(BaseModel):
     """
     Parameters to attach or remove user team
     """ # noqa: E501
     team: StrictStr
-    perm: Optional[StrictStr] = None
+    perm: Optional[StrictStr] = 'user'
     __properties: ClassVar[List[str]] = ["team", "perm"]
 
     @field_validator('perm')
     def perm_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -89,12 +89,12 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "team": obj.get("team"),
-            "perm": obj.get("perm")
+            "perm": obj.get("perm") if obj.get("perm") is not None else 'user'
         })
         return _obj
```

### Comparing `gopad-1.0.0/gopad/models/user_teams.py` & `gopad-1.1.0/gopad/models/user_teams.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/users.py` & `gopad-1.1.0/gopad/models/users.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/models/validation.py` & `gopad-1.1.0/gopad/models/validation.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/gopad/rest.py` & `gopad-1.1.0/gopad/rest.py`

 * *Files identical despite different names*

### Comparing `gopad-1.0.0/pyproject.toml` & `gopad-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gopad"
-version = "1.0.0"
+version = "1.1.0"
 description = "Gopad OpenAPI"
 
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "License :: OSI Approved :: MIT License",
   "Intended Audience :: Developers",
```

### Comparing `gopad-1.0.0/PKG-INFO` & `gopad-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopad
-Version: 1.0.0
+Version: 1.1.0
 Summary: Gopad OpenAPI
 Home-page: https://github.com/gopad/gopad-python
 License: Apache-2.0
 Keywords: OpenAPI,OpenAPI-Generator,Etherpad,Gopad
 Author: Thomas Boerger
 Author-email: thomas@webhippie.de
 Requires-Python: >=3.7,<4.0
@@ -37,15 +37,15 @@
 
 [![General Workflow](https://github.com/gopad/gopad-python/actions/workflows/general.yml/badge.svg)](https://github.com/gopad/gopad-python/actions/workflows/general.yml) [![Join the Matrix chat at https://matrix.to/#/#gopad:matrix.org](https://img.shields.io/badge/matrix-%23gopad%3Amatrix.org-7bc9a4.svg)](https://matrix.to/#/#gopad:matrix.org) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/0581d0652d4d4dddb3fc353f74cd9bed)](https://app.codacy.com/gh/gopad/gopad-python/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![PyPI Version](https://badge.fury.io/py/gopad.svg)](https://badge.fury.io/py/gopad)
 
 This repository provides a client SDK for Python. This SDK is automatically
 generated by the [OpenAPI Generator][generator] project:
 
 -   API version: 1.0.0-alpha1
--   Package version: 1.0.0
+-   Package version: 1.1.0
 -   Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://gopad.eu](https://gopad.eu)
 
 ## Requirements
 
 Python 3.7+
@@ -53,15 +53,15 @@
 ## Installation
 
 If you want to use one of the versions released via PyPi you just need to
 execute the following command within your project directory, after that you can
 import it as other libraries:
 
 ```console
-pip install gopad@1.0.0
+pip install gopad@1.1.0
 ```
 
 ## Tests
 
 ```console
 pytest
 ```
```

