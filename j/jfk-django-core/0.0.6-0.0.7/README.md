# Comparing `tmp/jfk_django_core-0.0.6.tar.gz` & `tmp/jfk_django_core-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jfk_django_core-0.0.6.tar", last modified: Wed May 29 18:29:57 2024, max compression
+gzip compressed data, was "jfk_django_core-0.0.7.tar", last modified: Sun Jun  2 11:49:55 2024, max compression
```

## Comparing `jfk_django_core-0.0.6.tar` & `jfk_django_core-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.392773 jfk_django_core-0.0.6/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.387773 jfk_django_core-0.0.6/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/.vscode/launch.json
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      874 2024-05-29 18:29:57.391773 jfk_django_core-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.389773 jfk_django_core-0.0.6/jfk_django_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.390773 jfk_django_core-0.0.6/jfk_django_core/admin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/admin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.390773 jfk_django_core-0.0.6/jfk_django_core/apis/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/apis/jfk_authentication.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.391773 jfk_django_core-0.0.6/jfk_django_core/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.391773 jfk_django_core-0.0.6/jfk_django_core/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     7207 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/jfk_django_core/viewsets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:29:57.391773 jfk_django_core-0.0.6/jfk_django_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)      874 2024-05-29 18:29:57.000000 jfk_django_core-0.0.6/jfk_django_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-29 18:29:57.000000 jfk_django_core-0.0.6/jfk_django_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 18:29:57.000000 jfk_django_core-0.0.6/jfk_django_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-29 18:29:57.000000 jfk_django_core-0.0.6/jfk_django_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-29 18:29:57.000000 jfk_django_core-0.0.6/jfk_django_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 18:29:57.392773 jfk_django_core-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-29 18:29:49.000000 jfk_django_core-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.917635 jfk_django_core-0.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.913635 jfk_django_core-0.0.7/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/.vscode/launch.json
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      874 2024-06-02 11:49:55.916635 jfk_django_core-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.914635 jfk_django_core-0.0.7/jfk_django_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.915635 jfk_django_core-0.0.7/jfk_django_core/admin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/admin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.915635 jfk_django_core-0.0.7/jfk_django_core/apis/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/apis/jfk_authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.916635 jfk_django_core-0.0.7/jfk_django_core/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.916635 jfk_django_core-0.0.7/jfk_django_core/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7207 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/jfk_django_core/viewsets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 11:49:55.916635 jfk_django_core-0.0.7/jfk_django_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      874 2024-06-02 11:49:55.000000 jfk_django_core-0.0.7/jfk_django_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      628 2024-06-02 11:49:55.000000 jfk_django_core-0.0.7/jfk_django_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 11:49:55.000000 jfk_django_core-0.0.7/jfk_django_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      391 2024-06-02 11:49:55.000000 jfk_django_core-0.0.7/jfk_django_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-06-02 11:49:55.000000 jfk_django_core-0.0.7/jfk_django_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-02 11:49:55.917635 jfk_django_core-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-06-02 11:49:48.000000 jfk_django_core-0.0.7/setup.py
```

### Comparing `jfk_django_core-0.0.6/LICENSE` & `jfk_django_core-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.6/PKG-INFO` & `jfk_django_core-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfk-django-core
-Version: 0.0.6
+Version: 0.0.7
 Summary: JFK Django Core
 Author: JFK344
 License: All-Rights-Reserved
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=5.0.0
```

### Comparing `jfk_django_core-0.0.6/jfk_django_core/apis/jfk_authentication.py` & `jfk_django_core-0.0.7/jfk_django_core/apis/jfk_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from rest_framework.authentication import BasicAuthentication
 
 @extend_schema_view(
     post=extend_schema(operation_id='login')
 )
 class TokenLoginView(LoginView):
     authentication_classes = [BasicAuthentication]
+    permission_classes = []
     pass
 
 
 @extend_schema_view(
     post=extend_schema(operation_id='logout')
 )
 class TokenLogoutView(LogoutView):
```

### Comparing `jfk_django_core-0.0.6/jfk_django_core/settings.py` & `jfk_django_core-0.0.7/jfk_django_core/settings.py`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.6/jfk_django_core/urls.py` & `jfk_django_core-0.0.7/jfk_django_core/urls.py`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.6/jfk_django_core.egg-info/PKG-INFO` & `jfk_django_core-0.0.7/jfk_django_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfk-django-core
-Version: 0.0.6
+Version: 0.0.7
 Summary: JFK Django Core
 Author: JFK344
 License: All-Rights-Reserved
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=5.0.0
```

### Comparing `jfk_django_core-0.0.6/jfk_django_core.egg-info/SOURCES.txt` & `jfk_django_core-0.0.7/jfk_django_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.6/pyproject.toml` & `jfk_django_core-0.0.7/pyproject.toml`

 * *Files identical despite different names*

