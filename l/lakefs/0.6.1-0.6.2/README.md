# Comparing `tmp/lakefs-0.6.1.tar.gz` & `tmp/lakefs-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-0.6.1.tar", last modified: Mon May 20 11:05:18 2024, max compression
+gzip compressed data, was "lakefs-0.6.2.tar", last modified: Sun Jun  2 08:55:33 2024, max compression
```

## Comparing `lakefs-0.6.1.tar` & `lakefs-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0     1001      127        0 2024-05-20 11:05:18.286473 lakefs-0.6.1/
--rw-r--r--   0     1001      127     3630 2024-05-20 11:05:18.286473 lakefs-0.6.1/PKG-INFO
--rw-r--r--   0     1001      127     3199 2024-05-20 11:04:25.000000 lakefs-0.6.1/README.md
-drwxr-xr-x   0     1001      127        0 2024-05-20 11:05:18.278473 lakefs-0.6.1/lakefs/
--rw-r--r--   0     1001      127      931 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/__init__.py
--rw-r--r--   0     1001      127    18144 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/branch.py
--rw-r--r--   0     1001      127     5062 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/client.py
--rw-r--r--   0     1001      127     3172 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/config.py
--rw-r--r--   0     1001      127     4246 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/exceptions.py
--rw-r--r--   0     1001      127     9021 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/import_manager.py
--rw-r--r--   0     1001      127     2810 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/models.py
--rw-r--r--   0     1001      127     1650 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/namedtuple.py
--rw-r--r--   0     1001      127    29651 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/object.py
--rw-r--r--   0     1001      127     8688 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/reference.py
--rw-r--r--   0     1001      127     8167 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/repository.py
--rw-r--r--   0     1001      127     2153 2024-05-20 11:04:25.000000 lakefs-0.6.1/lakefs/tag.py
-drwxr-xr-x   0     1001      127        0 2024-05-20 11:05:18.286473 lakefs-0.6.1/lakefs.egg-info/
--rw-r--r--   0     1001      127     3630 2024-05-20 11:05:18.000000 lakefs-0.6.1/lakefs.egg-info/PKG-INFO
--rw-r--r--   0     1001      127      948 2024-05-20 11:05:18.000000 lakefs-0.6.1/lakefs.egg-info/SOURCES.txt
--rw-r--r--   0     1001      127        1 2024-05-20 11:05:18.000000 lakefs-0.6.1/lakefs.egg-info/dependency_links.txt
--rw-r--r--   0     1001      127       34 2024-05-20 11:05:18.000000 lakefs-0.6.1/lakefs.egg-info/requires.txt
--rw-r--r--   0     1001      127       13 2024-05-20 11:05:18.000000 lakefs-0.6.1/lakefs.egg-info/top_level.txt
--rw-r--r--   0     1001      127       95 2024-05-20 11:05:18.286473 lakefs-0.6.1/setup.cfg
--rw-r--r--   0     1001      127     1130 2024-05-20 11:04:25.000000 lakefs-0.6.1/setup.py
-drwxr-xr-x   0     1001      127        0 2024-05-20 11:05:18.278473 lakefs-0.6.1/tests/
-drwxr-xr-x   0     1001      127        0 2024-05-20 11:05:18.282473 lakefs-0.6.1/tests/integration/
--rw-r--r--   0     1001      127        0 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/__init__.py
--rw-r--r--   0     1001      127     2128 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/conftest.py
--rw-r--r--   0     1001      127     7978 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/test_branch.py
--rw-r--r--   0     1001      127     3284 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/test_import.py
--rw-r--r--   0     1001      127    13965 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/test_object.py
--rw-r--r--   0     1001      127     2754 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/test_reference.py
--rw-r--r--   0     1001      127     1679 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/test_repository.py
--rw-r--r--   0     1001      127     4623 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/integration/test_sanity.py
-drwxr-xr-x   0     1001      127        0 2024-05-20 11:05:18.286473 lakefs-0.6.1/tests/utests/
--rw-r--r--   0     1001      127        0 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/__init__.py
--rw-r--r--   0     1001      127     2373 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/common.py
--rw-r--r--   0     1001      127     6058 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_branch.py
--rw-r--r--   0     1001      127     1665 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_client.py
--rw-r--r--   0     1001      127     1913 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_import.py
--rw-r--r--   0     1001      127     1440 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_namedtuple.py
--rw-r--r--   0     1001      127    10028 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_object.py
--rw-r--r--   0     1001      127     5167 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_reference.py
--rw-r--r--   0     1001      127     5281 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_repository.py
--rw-r--r--   0     1001      127      381 2024-05-20 11:04:25.000000 lakefs-0.6.1/tests/utests/test_tag.py
+drwxr-xr-x   0     1001      127        0 2024-06-02 08:55:33.807839 lakefs-0.6.2/
+-rw-r--r--   0     1001      127     3630 2024-06-02 08:55:33.807839 lakefs-0.6.2/PKG-INFO
+-rw-r--r--   0     1001      127     3199 2024-06-02 08:54:48.000000 lakefs-0.6.2/README.md
+drwxr-xr-x   0     1001      127        0 2024-06-02 08:55:33.799840 lakefs-0.6.2/lakefs/
+-rw-r--r--   0     1001      127      931 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/__init__.py
+-rw-r--r--   0     1001      127    18144 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/branch.py
+-rw-r--r--   0     1001      127     5062 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/client.py
+-rw-r--r--   0     1001      127     3172 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/config.py
+-rw-r--r--   0     1001      127     4246 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/exceptions.py
+-rw-r--r--   0     1001      127     9021 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/import_manager.py
+-rw-r--r--   0     1001      127     2810 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/models.py
+-rw-r--r--   0     1001      127     1650 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/namedtuple.py
+-rw-r--r--   0     1001      127    29651 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/object.py
+-rw-r--r--   0     1001      127     8688 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/reference.py
+-rw-r--r--   0     1001      127     8167 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/repository.py
+-rw-r--r--   0     1001      127     2153 2024-06-02 08:54:48.000000 lakefs-0.6.2/lakefs/tag.py
+drwxr-xr-x   0     1001      127        0 2024-06-02 08:55:33.803840 lakefs-0.6.2/lakefs.egg-info/
+-rw-r--r--   0     1001      127     3630 2024-06-02 08:55:33.000000 lakefs-0.6.2/lakefs.egg-info/PKG-INFO
+-rw-r--r--   0     1001      127      948 2024-06-02 08:55:33.000000 lakefs-0.6.2/lakefs.egg-info/SOURCES.txt
+-rw-r--r--   0     1001      127        1 2024-06-02 08:55:33.000000 lakefs-0.6.2/lakefs.egg-info/dependency_links.txt
+-rw-r--r--   0     1001      127       34 2024-06-02 08:55:33.000000 lakefs-0.6.2/lakefs.egg-info/requires.txt
+-rw-r--r--   0     1001      127       13 2024-06-02 08:55:33.000000 lakefs-0.6.2/lakefs.egg-info/top_level.txt
+-rw-r--r--   0     1001      127       95 2024-06-02 08:55:33.807839 lakefs-0.6.2/setup.cfg
+-rw-r--r--   0     1001      127     1130 2024-06-02 08:54:48.000000 lakefs-0.6.2/setup.py
+drwxr-xr-x   0     1001      127        0 2024-06-02 08:55:33.795840 lakefs-0.6.2/tests/
+drwxr-xr-x   0     1001      127        0 2024-06-02 08:55:33.803840 lakefs-0.6.2/tests/integration/
+-rw-r--r--   0     1001      127        0 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/__init__.py
+-rw-r--r--   0     1001      127     2128 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/conftest.py
+-rw-r--r--   0     1001      127     7978 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/test_branch.py
+-rw-r--r--   0     1001      127     3284 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/test_import.py
+-rw-r--r--   0     1001      127    13965 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/test_object.py
+-rw-r--r--   0     1001      127     3255 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/test_reference.py
+-rw-r--r--   0     1001      127     1679 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/test_repository.py
+-rw-r--r--   0     1001      127     4623 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/integration/test_sanity.py
+drwxr-xr-x   0     1001      127        0 2024-06-02 08:55:33.803840 lakefs-0.6.2/tests/utests/
+-rw-r--r--   0     1001      127        0 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/__init__.py
+-rw-r--r--   0     1001      127     2373 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/common.py
+-rw-r--r--   0     1001      127     6058 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_branch.py
+-rw-r--r--   0     1001      127     1665 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_client.py
+-rw-r--r--   0     1001      127     1913 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_import.py
+-rw-r--r--   0     1001      127     1440 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_namedtuple.py
+-rw-r--r--   0     1001      127    10028 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_object.py
+-rw-r--r--   0     1001      127     5167 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_reference.py
+-rw-r--r--   0     1001      127     5281 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_repository.py
+-rw-r--r--   0     1001      127      381 2024-06-02 08:54:48.000000 lakefs-0.6.2/tests/utests/test_tag.py
```

### Comparing `lakefs-0.6.1/PKG-INFO` & `lakefs-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lakefs
-Version: 0.6.1
+Version: 0.6.2
 Summary: lakeFS Python SDK Wrapper
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python-wrapper
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API,Python Wrapper
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: lakefs-sdk<2,>=1.20
+Requires-Dist: lakefs-sdk<2,>=1.25
 Requires-Dist: pyyaml~=6.0.1
 
 # lakeFS High-Level Python SDK
 
 lakeFS High Level SDK for Python, provides developers with the following features:
 1. Simpler programming interface with less configuration
 2. Inferring identity from environment
```

### Comparing `lakefs-0.6.1/README.md` & `lakefs-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/__init__.py` & `lakefs-0.6.2/lakefs/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/branch.py` & `lakefs-0.6.2/lakefs/branch.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/client.py` & `lakefs-0.6.2/lakefs/client.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/config.py` & `lakefs-0.6.2/lakefs/config.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/exceptions.py` & `lakefs-0.6.2/lakefs/exceptions.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/import_manager.py` & `lakefs-0.6.2/lakefs/import_manager.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/models.py` & `lakefs-0.6.2/lakefs/models.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/namedtuple.py` & `lakefs-0.6.2/lakefs/namedtuple.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/object.py` & `lakefs-0.6.2/lakefs/object.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/reference.py` & `lakefs-0.6.2/lakefs/reference.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/repository.py` & `lakefs-0.6.2/lakefs/repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs/tag.py` & `lakefs-0.6.2/lakefs/tag.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/lakefs.egg-info/PKG-INFO` & `lakefs-0.6.2/lakefs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lakefs
-Version: 0.6.1
+Version: 0.6.2
 Summary: lakeFS Python SDK Wrapper
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python-wrapper
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API,Python Wrapper
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: lakefs-sdk<2,>=1.20
+Requires-Dist: lakefs-sdk<2,>=1.25
 Requires-Dist: pyyaml~=6.0.1
 
 # lakeFS High-Level Python SDK
 
 lakeFS High Level SDK for Python, provides developers with the following features:
 1. Simpler programming interface with less configuration
 2. Inferring identity from environment
```

### Comparing `lakefs-0.6.1/lakefs.egg-info/SOURCES.txt` & `lakefs-0.6.2/lakefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/setup.py` & `lakefs-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 NAME = "lakefs"
-VERSION = "0.6.1"
+VERSION = "0.6.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 PYTHON_REQUIRES = ">=3.9"
 REQUIRES = [
-    "lakefs-sdk >= 1.20, < 2",
+    "lakefs-sdk >= 1.25, < 2",
     "pyyaml ~= 6.0.1",
 ]
 TEST_REQUIRES = [
     "pytest ~= 7.4.3",
     "pytest-datafiles ~= 3.0.0",
     "pandas ~= 2.1.4",
     "pyarrow ~= 14.0.1",
```

### Comparing `lakefs-0.6.1/tests/integration/conftest.py` & `lakefs-0.6.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/integration/test_branch.py` & `lakefs-0.6.2/tests/integration/test_branch.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/integration/test_import.py` & `lakefs-0.6.2/tests/integration/test_import.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/integration/test_object.py` & `lakefs-0.6.2/tests/integration/test_object.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/integration/test_reference.py` & `lakefs-0.6.2/tests/integration/test_reference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import pytest
+
 import lakefs
+from lakefs.exceptions import BadRequestException
 
 
 def test_reference_log(setup_branch_with_commits):
     branch = setup_branch_with_commits
 
     for i, c in enumerate(branch.log(max_amount=199)):
         assert c.message == f"commit {i}"
@@ -43,14 +46,24 @@
 
 
 def test_reference_merge_into(setup_branch_with_commits):
     branch = setup_branch_with_commits
     repo = lakefs.Repository(branch.repo_id)
     main = repo.branch("main")
 
+    # test merging into same branch
+    branch_a = repo.branch("test_branch_merge_into_a").create(branch)
+    branch_b = repo.branch("test_branch_merge_into_b").create(branch)
+
+    with pytest.raises(BadRequestException, match=r'.+no changes.+'):
+        branch_a.merge_into(branch_b, message="MergeNoChanges")
+
+    branch_a.merge_into(branch_b, message="MergeNoChangesWithFlag", allow_empty=True)
+
+    # test merging into other branch
     commits = list(branch.log(max_amount=2))
     other_branch = repo.branch("test_reference_merge_into").create(main)
     ref = repo.ref(commits[1].id)
     ref.merge_into(other_branch, message="Merge1")
     assert other_branch.get_commit().message == "Merge1"
     assert list(other_branch.log(max_amount=2))[1].id == commits[1].id
```

### Comparing `lakefs-0.6.1/tests/integration/test_repository.py` & `lakefs-0.6.2/tests/integration/test_repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/integration/test_sanity.py` & `lakefs-0.6.2/tests/integration/test_sanity.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/common.py` & `lakefs-0.6.2/tests/utests/common.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/test_branch.py` & `lakefs-0.6.2/tests/utests/test_branch.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/test_client.py` & `lakefs-0.6.2/tests/utests/test_client.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/test_import.py` & `lakefs-0.6.2/tests/utests/test_import.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/test_namedtuple.py` & `lakefs-0.6.2/tests/utests/test_namedtuple.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/test_object.py` & `lakefs-0.6.2/tests/utests/test_object.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/test_reference.py` & `lakefs-0.6.2/tests/utests/test_reference.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.6.1/tests/utests/test_repository.py` & `lakefs-0.6.2/tests/utests/test_repository.py`

 * *Files identical despite different names*

