# Comparing `tmp/drf_cookie_jwtauth-0.0.4.tar.gz` & `tmp/drf_cookie_jwtauth-0.0.5.tar.gz`

## Comparing `drf_cookie_jwtauth-0.0.4.tar` & `drf_cookie_jwtauth-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.gitattributes
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/pytest.ini
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/admin.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/manager.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/middleware.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/models.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/settings.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/tokens.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/utils.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_auth.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_tokens.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_views/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_views/urls.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_views/views.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/LICENSE
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/.gitattributes
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/pytest.ini
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/admin.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/manager.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/middleware.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/models.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/settings.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/tokens.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/utils.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/src/jwtauth/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/tests/test_auth.py
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/tests/test_tokens.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/tests/test_views/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/tests/test_views/urls.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/tests/test_views/views.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.5/PKG-INFO
```

### Comparing `drf_cookie_jwtauth-0.0.4/.github/workflows/python-publish.yml` & `drf_cookie_jwtauth-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/.github/workflows/python-test.yml` & `drf_cookie_jwtauth-0.0.5/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/src/jwtauth/manager.py` & `drf_cookie_jwtauth-0.0.5/src/jwtauth/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from rest_framework import exceptions
 from django.conf import settings
 
-from jwtauth.tokens import AccessToken, RefreshToken
 from jwtauth.settings import api_settings
-
+from jwtauth.tokens import AccessToken, RefreshToken
 
 ACCESS_TOKEN_KEY = api_settings.ACCESS_TOKEN_COOKIE_NAME
 REFRESH_TOKEN_KEY = api_settings.REFRESH_TOKEN_COOKIE_NAME
 
 
 class AuthManager:
 
@@ -25,20 +23,20 @@
             # authentication token (even if expired) and a valid refresh token
             return
 
         if not self.access_token.valid() or not self.refresh_token.valid():
             # we end up here if:
             # - one of the tokens was forged by a malicious user
             # - the refresh token was blacklisted
-            raise exceptions.AuthenticationFailed("Invalid tokens")
+            return
 
         if self.access_token.expired():
             if self.refresh_token.expired():
                 # both tokens are expired, the user has to log in again
-                raise exceptions.AuthenticationFailed("Expired tokens")
+                return
 
             # we silently refresh the authentication token and let the user in
             self.silent_refresh = True
             self.access_token = self.refresh_token.gen_access_token()
 
         # the authentication token is valid and not expired
         self.user = self.access_token.user
```

### Comparing `drf_cookie_jwtauth-0.0.4/src/jwtauth/middleware.py` & `drf_cookie_jwtauth-0.0.5/src/jwtauth/middleware.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/src/jwtauth/settings.py` & `drf_cookie_jwtauth-0.0.5/src/jwtauth/settings.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/src/jwtauth/tokens.py` & `drf_cookie_jwtauth-0.0.5/src/jwtauth/tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from calendar import timegm
+from datetime import datetime, timedelta, timezone
 
+import jwt
 from django.contrib.auth import get_user_model
 
-from datetime import datetime, timezone, timedelta
-
-from jwtauth.utils import generate_unique_token
+from jwtauth.models import ActiveToken, BlacklistedToken
 from jwtauth.settings import api_settings
-from jwtauth.models import BlacklistedToken, ActiveToken
-
-import jwt
+from jwtauth.utils import generate_unique_token
 
 IAT = "iat"
 EXP = "exp"
 
 UserModel = get_user_model()
 
 
@@ -161,31 +159,35 @@
             return False
 
         return True
 
 
 class AccessToken(UserToken):
 
-    def __init__(self, from_encoding=None, from_user=None):
+    def __init__(
+        self, from_encoding=None, from_user=None, duration=api_settings.ACCESS_TOKEN_LIFETIME
+    ):
         super().__init__(
             from_encoding=from_encoding,
             from_data=from_user,
-            duration=api_settings.ACCESS_TOKEN_LIFETIME,
+            duration=duration,
         )
 
 
 class RefreshToken(UserToken):
     TOKEN_STRING_KEY = "token_string"
 
-    def __init__(self, from_encoding=None, from_user=None):
+    def __init__(
+        self, from_encoding=None, from_user=None, duration=api_settings.REFRESH_TOKEN_LIFETIME
+    ):
         self.token_string = None
         super().__init__(
             from_encoding=from_encoding,
             from_data=from_user,
-            duration=api_settings.REFRESH_TOKEN_LIFETIME,
+            duration=duration,
         )
 
     def encode(self, user, data=None) -> None:
         self.token_string = generate_unique_token()
         super().encode(user, {self.TOKEN_STRING_KEY: self.token_string})
 
     def decode(self, data) -> bool:
```

### Comparing `drf_cookie_jwtauth-0.0.4/src/jwtauth/utils.py` & `drf_cookie_jwtauth-0.0.5/src/jwtauth/utils.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/src/jwtauth/migrations/0001_initial.py` & `drf_cookie_jwtauth-0.0.5/src/jwtauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/tests/conftest.py` & `drf_cookie_jwtauth-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/tests/test_tokens.py` & `drf_cookie_jwtauth-0.0.5/tests/test_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from jwtauth.tokens import Token, UserToken, AccessToken, RefreshToken
-from datetime import timedelta, datetime, timezone
-from jwtauth.settings import api_settings
-from jwtauth.models import ActiveToken
-import pytest
+from datetime import datetime, timedelta, timezone
+
 import jwt
+import pytest
+
+from jwtauth.models import ActiveToken
+from jwtauth.settings import api_settings
+from jwtauth.tokens import AccessToken, RefreshToken, Token, UserToken
 
 
 def test_valid_token():
     # create a token and verify it is marked as valid and not expired
     token = Token(from_data={"data": 42}, duration=timedelta(minutes=5))
     assert token.valid()
     assert not token.expired()
```

### Comparing `drf_cookie_jwtauth-0.0.4/tests/test_views/views.py` & `drf_cookie_jwtauth-0.0.5/tests/test_views/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django.contrib.auth import authenticate
-from rest_framework.parsers import JSONParser
-
-from rest_framework.views import APIView
 from rest_framework.decorators import api_view, permission_classes
 from rest_framework.exceptions import AuthenticationFailed
+from rest_framework.parsers import JSONParser
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
+from rest_framework.views import APIView
 
 from jwtauth import login, logout
 
 
 @api_view(["POST"])
 def login_view(request):
     body = JSONParser().parse(request)
```

### Comparing `drf_cookie_jwtauth-0.0.4/LICENSE` & `drf_cookie_jwtauth-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.4/README.md` & `drf_cookie_jwtauth-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # jwtauth
 
 A JWT-based authentication system for 
 [Django REST Framework](https://github.com/encode/django-rest-framework/tree/master).
 
 ## 🪄 Installation
 
-This package is not available on the pip registry yet. To install it, download the compressed package from
-[here](https://github.com/lorenzocelli/jwtauth/actions/runs/7941362543/artifacts/1253381430), 
-extract it and then run:
+This package is available on the [pip registry](https://pypi.org/project/drf-cookie-jwtauth/). 
+To install it, you can run:
 ```
-python3 -m pip install jwtauth-0.0.1.tar.gz
+pip install drf-cookie-jwtauth
 ```
 
 ## ⚙️ Configuration
 
 Add `jwtauth` to your `INSTALLED_APPS`:
 
 ```python
```

### Comparing `drf_cookie_jwtauth-0.0.4/pyproject.toml` & `drf_cookie_jwtauth-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/jwtauth"]
 
 [project]
 name = "drf-cookie-jwtauth"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Lorenzo Celli", email="lorenzo.celli00@gmail.com" },
 ]
 description = "JWT-based authentication for Django REST Framework"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `drf_cookie_jwtauth-0.0.4/PKG-INFO` & `drf_cookie_jwtauth-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: drf-cookie-jwtauth
-Version: 0.0.4
+Version: 0.0.5
 Summary: JWT-based authentication for Django REST Framework
 Author-email: Lorenzo Celli <lorenzo.celli00@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -16,19 +16,18 @@
 # jwtauth
 
 A JWT-based authentication system for 
 [Django REST Framework](https://github.com/encode/django-rest-framework/tree/master).
 
 ## 🪄 Installation
 
-This package is not available on the pip registry yet. To install it, download the compressed package from
-[here](https://github.com/lorenzocelli/jwtauth/actions/runs/7941362543/artifacts/1253381430), 
-extract it and then run:
+This package is available on the [pip registry](https://pypi.org/project/drf-cookie-jwtauth/). 
+To install it, you can run:
 ```
-python3 -m pip install jwtauth-0.0.1.tar.gz
+pip install drf-cookie-jwtauth
 ```
 
 ## ⚙️ Configuration
 
 Add `jwtauth` to your `INSTALLED_APPS`:
 
 ```python
```

