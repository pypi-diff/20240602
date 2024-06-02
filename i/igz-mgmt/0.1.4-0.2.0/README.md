# Comparing `tmp/igz_mgmt-0.1.4.tar.gz` & `tmp/igz_mgmt-0.2.0.tar.gz`

## Comparing `igz_mgmt-0.1.4.tar` & `igz_mgmt-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/client.py
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/constants.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/operations.py
--rw-r--r--   0        0        0    92483 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/__init__.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/app_services.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/events.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/limits.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/manual_events.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/README.md
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/client.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    92483 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/schemas/events.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/schemas/limits.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/README.md
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 igz_mgmt-0.2.0/PKG-INFO
```

### Comparing `igz_mgmt-0.1.4/igz_mgmt/__init__.py` & `igz_mgmt-0.2.0/igz_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/__version__.py` & `igz_mgmt-0.2.0/igz_mgmt/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 #
 
 # version can be either one of the following:
 # x.y.z
 # x.y.z.rcN
 # x.y.zrcN
 
-__version__ = "0.1.4"
+__version__ = "0.2.0"
```

### Comparing `igz_mgmt-0.1.4/igz_mgmt/client.py` & `igz_mgmt-0.2.0/igz_mgmt/client.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/constants.py` & `igz_mgmt-0.2.0/igz_mgmt/constants.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/cruds.py` & `igz_mgmt-0.2.0/igz_mgmt/cruds.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/exceptions.py` & `igz_mgmt-0.2.0/igz_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/operations.py` & `igz_mgmt-0.2.0/igz_mgmt/operations.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/resources.py` & `igz_mgmt-0.2.0/igz_mgmt/resources.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/common/__init__.py` & `igz_mgmt-0.2.0/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/common/helpers.py` & `igz_mgmt-0.2.0/igz_mgmt/common/helpers.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.2.0/igz_mgmt/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/logger/logger.py` & `igz_mgmt-0.2.0/igz_mgmt/logger/logger.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/schemas/__init__.py` & `igz_mgmt-0.2.0/igz_mgmt/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/schemas/app_services.py` & `igz_mgmt-0.2.0/igz_mgmt/schemas/app_services.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/schemas/events.py` & `igz_mgmt-0.2.0/igz_mgmt/schemas/events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/schemas/limits.py` & `igz_mgmt-0.2.0/igz_mgmt/schemas/limits.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/igz_mgmt/schemas/manual_events.py` & `igz_mgmt-0.2.0/igz_mgmt/schemas/manual_events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/LICENSE` & `igz_mgmt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.4/pyproject.toml` & `igz_mgmt-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 [project]
 name = "igz-mgmt"
 dynamic = ["version"]
 description = "Python SDK For Iguazio Management API"
 readme = "README.md"
 license = "Apache-2.0"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 authors = [
     { name = "Iguazio Platform Team", email = "liranb@iguazio.com" },
 ]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "httpx~=0.24.1",
+    "httpx~=0.27.0",
     "inflection~=0.5.1",
     "pydantic~=1.10.10",
     "semver~=3.0.1",
     "deprecated~=1.2.14",
 ]
 
 [project.optional-dependencies]
```

### Comparing `igz_mgmt-0.1.4/PKG-INFO` & `igz_mgmt-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: igz-mgmt
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Requires-Dist: deprecated~=1.2.14
-Requires-Dist: httpx~=0.24.1
+Requires-Dist: httpx~=0.27.0
 Requires-Dist: inflection~=0.5.1
 Requires-Dist: pydantic~=1.10.10
 Requires-Dist: semver~=3.0.1
 Description-Content-Type: text/markdown
 
 # igz-mgmt-sdk
```

