# Comparing `tmp/drf_cookie_jwtauth-0.0.3.tar.gz` & `tmp/drf_cookie_jwtauth-0.0.4.tar.gz`

## Comparing `drf_cookie_jwtauth-0.0.3.tar` & `drf_cookie_jwtauth-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/.gitattributes
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/pytest.ini
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/requirements.txt
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/admin.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/manager.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/middleware.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/models.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/settings.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/tokens.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/utils.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/src/jwtauth/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/tests/test_auth.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/tests/test_tokens.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/tests/test_views/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/tests/test_views/urls.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/tests/test_views/views.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/LICENSE
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.gitattributes
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/pytest.ini
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/admin.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/manager.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/middleware.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/models.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/settings.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/tokens.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/utils.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/src/jwtauth/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_auth.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_tokens.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_views/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_views/urls.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/tests/test_views/views.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 drf_cookie_jwtauth-0.0.4/PKG-INFO
```

### Comparing `drf_cookie_jwtauth-0.0.3/.github/workflows/python-test.yml` & `drf_cookie_jwtauth-0.0.4/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/src/jwtauth/manager.py` & `drf_cookie_jwtauth-0.0.4/src/jwtauth/manager.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/src/jwtauth/middleware.py` & `drf_cookie_jwtauth-0.0.4/src/jwtauth/middleware.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/src/jwtauth/settings.py` & `drf_cookie_jwtauth-0.0.4/src/jwtauth/settings.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/src/jwtauth/tokens.py` & `drf_cookie_jwtauth-0.0.4/src/jwtauth/tokens.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/src/jwtauth/utils.py` & `drf_cookie_jwtauth-0.0.4/src/jwtauth/utils.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/src/jwtauth/migrations/0001_initial.py` & `drf_cookie_jwtauth-0.0.4/src/jwtauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/tests/conftest.py` & `drf_cookie_jwtauth-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/tests/test_auth.py` & `drf_cookie_jwtauth-0.0.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/tests/test_tokens.py` & `drf_cookie_jwtauth-0.0.4/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/tests/test_views/views.py` & `drf_cookie_jwtauth-0.0.4/tests/test_views/views.py`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/LICENSE` & `drf_cookie_jwtauth-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/README.md` & `drf_cookie_jwtauth-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `drf_cookie_jwtauth-0.0.3/pyproject.toml` & `drf_cookie_jwtauth-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/jwtauth"]
 
 [project]
 name = "drf-cookie-jwtauth"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Lorenzo Celli", email="lorenzo.celli00@gmail.com" },
 ]
 description = "JWT-based authentication for Django REST Framework"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `drf_cookie_jwtauth-0.0.3/PKG-INFO` & `drf_cookie_jwtauth-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: drf-cookie-jwtauth
-Version: 0.0.3
+Version: 0.0.4
 Summary: JWT-based authentication for Django REST Framework
 Author-email: Lorenzo Celli <lorenzo.celli00@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

