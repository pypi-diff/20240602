# Comparing `tmp/kal_middleware-0.0.8.tar.gz` & `tmp/kal_middleware-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kal_middleware-0.0.8.tar", last modified: Mon May 27 11:00:46 2024, max compression
+gzip compressed data, was "kal_middleware-0.0.9.tar", last modified: Sun Jun  2 11:40:36 2024, max compression
```

## Comparing `kal_middleware-0.0.8.tar` & `kal_middleware-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.884388 kal_middleware-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.876388 kal_middleware-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.880388 kal_middleware-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.880388 kal_middleware-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-27 11:00:46.884388 kal_middleware-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.880388 kal_middleware-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.880388 kal_middleware-0.0.8/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/jwt.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/kal_middleware.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.880388 kal_middleware-0.0.8/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/sts.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.880388 kal_middleware-0.0.8/kal_middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/kal_middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/kal_middleware/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/kal_middleware/kal_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/kal_middleware/sts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.884388 kal_middleware-0.0.8/kal_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-27 11:00:46.000000 kal_middleware-0.0.8/kal_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 11:00:46.000000 kal_middleware-0.0.8/kal_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:00:46.000000 kal_middleware-0.0.8/kal_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 11:00:46.000000 kal_middleware-0.0.8/kal_middleware.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 11:00:46.000000 kal_middleware-0.0.8/kal_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 11:00:46.000000 kal_middleware-0.0.8/kal_middleware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:00:46.884388 kal_middleware-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:00:46.884388 kal_middleware-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-27 11:00:36.000000 kal_middleware-0.0.8/tests/test_kal_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.455433 kal_middleware-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.443432 kal_middleware-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.447433 kal_middleware-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.447433 kal_middleware-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-06-02 11:40:36.455433 kal_middleware-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.451433 kal_middleware-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.451433 kal_middleware-0.0.9/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/jwt.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/kal_middleware.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.451433 kal_middleware-0.0.9/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/sts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.451433 kal_middleware-0.0.9/kal_middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/kal_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/kal_middleware/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/kal_middleware/kal_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/kal_middleware/sts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.451433 kal_middleware-0.0.9/kal_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-06-02 11:40:36.000000 kal_middleware-0.0.9/kal_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-06-02 11:40:36.000000 kal_middleware-0.0.9/kal_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 11:40:36.000000 kal_middleware-0.0.9/kal_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 11:40:36.000000 kal_middleware-0.0.9/kal_middleware.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 11:40:36.000000 kal_middleware-0.0.9/kal_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 11:40:36.000000 kal_middleware-0.0.9/kal_middleware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 11:40:36.455433 kal_middleware-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:40:36.451433 kal_middleware-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-02 11:40:26.000000 kal_middleware-0.0.9/tests/test_kal_middleware.py
```

### Comparing `kal_middleware-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `kal_middleware-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/ISSUE_TEMPLATE/config.yml` & `kal_middleware-0.0.9/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/workflows/docs-build.yml` & `kal_middleware-0.0.9/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/workflows/docs.yml` & `kal_middleware-0.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/workflows/installation.yml` & `kal_middleware-0.0.9/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/workflows/macos.yml` & `kal_middleware-0.0.9/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/workflows/pypi.yml` & `kal_middleware-0.0.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/workflows/ubuntu.yml` & `kal_middleware-0.0.9/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.github/workflows/windows.yml` & `kal_middleware-0.0.9/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/.gitignore` & `kal_middleware-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/LICENSE` & `kal_middleware-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/PKG-INFO` & `kal_middleware-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-middleware
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kaleidoo middleware package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-middleware
 Keywords: kal-middleware
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 1. `user_uid` - The Firebase unique ID.
 2. `user_capabilities` - A list of capabilities for later use in the request processing, if needed.
 3. `user` - If `check_access` is used, the user object will be attached to the request, so the entire process does not need to call the request again.
 
 ```python
 from kal_middleware.jwt import firebase_jwt_authenticated
 from typing import List
-from utils import get_org, get_user_by_fb_uid
+from utils import get_org, get_user_by_fb_uid, get_capability_by_service_action
 
 async def get_user(firebase_uid):
     user = await get_user_by_fb_uid(firebase_uid)
     return user
 
 # if there is specific variable in the body that needed checks of who access its data only
 async def check_access(user: dict, body: dict):
@@ -80,14 +80,19 @@
     if "org_id" in body:
         org = get_org(body["org_id"])
         if not org:
             return False, f"Org not found"
         return True, {"org": org}
     return False, f"User {user.get('id')} from another organization then the one that was requested."
 
+
+async def get_capability(service, action):
+    capability = await get_capability_by_service_action(service, action)
+    return capability
+
 @app.get("/your-route/<service>/<action>")
 @firebase_jwt_authenticated(get_user, check_access)
 async def your_route_function(
         request: Request = None,
         service: Union[str, None] = None,
         action: Union[str, None] = None
 ):
```

### Comparing `kal_middleware-0.0.8/README.md` & `kal_middleware-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 1. `user_uid` - The Firebase unique ID.
 2. `user_capabilities` - A list of capabilities for later use in the request processing, if needed.
 3. `user` - If `check_access` is used, the user object will be attached to the request, so the entire process does not need to call the request again.
 
 ```python
 from kal_middleware.jwt import firebase_jwt_authenticated
 from typing import List
-from utils import get_org, get_user_by_fb_uid
+from utils import get_org, get_user_by_fb_uid, get_capability_by_service_action
 
 async def get_user(firebase_uid):
     user = await get_user_by_fb_uid(firebase_uid)
     return user
 
 # if there is specific variable in the body that needed checks of who access its data only
 async def check_access(user: dict, body: dict):
@@ -52,14 +52,19 @@
     if "org_id" in body:
         org = get_org(body["org_id"])
         if not org:
             return False, f"Org not found"
         return True, {"org": org}
     return False, f"User {user.get('id')} from another organization then the one that was requested."
 
+
+async def get_capability(service, action):
+    capability = await get_capability_by_service_action(service, action)
+    return capability
+
 @app.get("/your-route/<service>/<action>")
 @firebase_jwt_authenticated(get_user, check_access)
 async def your_route_function(
         request: Request = None,
         service: Union[str, None] = None,
         action: Union[str, None] = None
 ):
```

### Comparing `kal_middleware-0.0.8/docs/contributing.md` & `kal_middleware-0.0.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/docs/installation.md` & `kal_middleware-0.0.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/kal_middleware/jwt.py` & `kal_middleware-0.0.9/kal_middleware/jwt.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                     )
             else:
                 return Response(status_code=status.HTTP_401_UNAUTHORIZED, content="Error, token not found.")
 
             # verify that the service and action exists in the config map
             service = kwargs.get('service')
             action = kwargs.get('action')
-            objects = None
+            objects = {}
 
             # verify that the user has the permission to execute the request
             user_uid = decoded_token["uid"]
             user = await get_user_by_fb_uid(user_uid)
             capabilities = [capability.get("id") for capability in user.get("capabilities")]
             capability = await get_capability(service, action)
             access = capability and capability.get("id") in capabilities
@@ -55,15 +55,15 @@
                         return Response(
                             status_code=status.HTTP_403_FORBIDDEN,
                             content=f"User not permitted to perform this action. reason: {objects}",
                         )
 
             request.state.user = user
             for key, value in objects.items():
-                request.state["key"] = value
+                setattr(request.state, key, value)
 
             # Process the request
             response = await func(request, *args, **kwargs)
             return response
 
         return decorated_function
```

### Comparing `kal_middleware-0.0.8/kal_middleware/sts.py` & `kal_middleware-0.0.9/kal_middleware/sts.py`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/kal_middleware.egg-info/PKG-INFO` & `kal_middleware-0.0.9/kal_middleware.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-middleware
-Version: 0.0.8
+Version: 0.0.9
 Summary: Kaleidoo middleware package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-middleware
 Keywords: kal-middleware
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
 1. `user_uid` - The Firebase unique ID.
 2. `user_capabilities` - A list of capabilities for later use in the request processing, if needed.
 3. `user` - If `check_access` is used, the user object will be attached to the request, so the entire process does not need to call the request again.
 
 ```python
 from kal_middleware.jwt import firebase_jwt_authenticated
 from typing import List
-from utils import get_org, get_user_by_fb_uid
+from utils import get_org, get_user_by_fb_uid, get_capability_by_service_action
 
 async def get_user(firebase_uid):
     user = await get_user_by_fb_uid(firebase_uid)
     return user
 
 # if there is specific variable in the body that needed checks of who access its data only
 async def check_access(user: dict, body: dict):
@@ -80,14 +80,19 @@
     if "org_id" in body:
         org = get_org(body["org_id"])
         if not org:
             return False, f"Org not found"
         return True, {"org": org}
     return False, f"User {user.get('id')} from another organization then the one that was requested."
 
+
+async def get_capability(service, action):
+    capability = await get_capability_by_service_action(service, action)
+    return capability
+
 @app.get("/your-route/<service>/<action>")
 @firebase_jwt_authenticated(get_user, check_access)
 async def your_route_function(
         request: Request = None,
         service: Union[str, None] = None,
         action: Union[str, None] = None
 ):
```

### Comparing `kal_middleware-0.0.8/kal_middleware.egg-info/SOURCES.txt` & `kal_middleware-0.0.9/kal_middleware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/mkdocs.yml` & `kal_middleware-0.0.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.8/pyproject.toml` & `kal_middleware-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kal-middleware"
-version = "0.0.8"
+version = "0.0.9"
 dynamic = [
     "dependencies",
 ]
 description = "Kaleidoo middleware package"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.8"
+current_version = "0.0.9"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

