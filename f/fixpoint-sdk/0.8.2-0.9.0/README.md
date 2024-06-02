# Comparing `tmp/fixpoint_sdk-0.8.2.tar.gz` & `tmp/fixpoint_sdk-0.9.0.tar.gz`

## Comparing `fixpoint_sdk-0.8.2.tar` & `fixpoint_sdk-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/.editorconfig
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/.lintstagedrc.json
--rw-r--r--   0        0        0    21726 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/.pylintrc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/mypy.ini
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/pytest.ini
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/test-requirements.txt
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/.github/workflows/pypi-release-prod.yml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/.github/workflows/pypi-release-test.yml
--rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/bin/pip-freeze
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/bin/pip-install
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/examples/__init__.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/examples/direct_logging.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/examples/function_calling.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/examples/main.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/examples/multi_llm.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/examples/router.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/examples/streaming.py
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/githooks/pre-commit
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/__init__.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/_logging_api.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/_mock_completions.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/client.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/compat.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/completions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/__init__.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/_mock_requests.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/debugging.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/env.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/exc.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/iterwrapper.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/logging.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/requests.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/openapi/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/openapi/exceptions.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/types/__init__.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/types/_utils.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/src/fixpoint_sdk/types/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/mock_completions.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/test_client.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/test_completions.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/test_types.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/lib/test_iterwrapper.py
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/lib/test_requests.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/tests/types/test_openai.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/LICENSE
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/README.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 fixpoint_sdk-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/.editorconfig
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/.lintstagedrc.json
+-rw-r--r--   0        0        0    21726 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/.pylintrc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/mypy.ini
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/pytest.ini
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/test-requirements.txt
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/.github/workflows/pypi-release-prod.yml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/.github/workflows/pypi-release-test.yml
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/bin/pip-freeze
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/bin/pip-install
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/examples/__init__.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/examples/direct_logging.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/examples/function_calling.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/examples/main.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/examples/multi_llm.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/examples/router.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/examples/streaming.py
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/githooks/pre-commit
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/_logging_api.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/_mock_completions.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/client.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/compat.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/completions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/_mock_requests.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/debugging.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/env.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/exc.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/iterwrapper.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/logging.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/requests.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/openapi/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/openapi/exceptions.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/types/__init__.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/types/_utils.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/src/fixpoint_sdk/types/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/mock_completions.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/test_client.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/test_completions.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/test_types.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/lib/test_iterwrapper.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/lib/test_requests.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/tests/types/test_openai.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 fixpoint_sdk-0.9.0/PKG-INFO
```

### Comparing `fixpoint_sdk-0.8.2/.pylintrc` & `fixpoint_sdk-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/mypy.ini` & `fixpoint_sdk-0.9.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/.github/workflows/ci.yml` & `fixpoint_sdk-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/.github/workflows/pypi-release-prod.yml` & `fixpoint_sdk-0.9.0/.github/workflows/pypi-release-prod.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/.github/workflows/pypi-release-test.yml` & `fixpoint_sdk-0.9.0/.github/workflows/pypi-release-test.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/bin/pip-freeze` & `fixpoint_sdk-0.9.0/bin/pip-freeze`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/examples/direct_logging.py` & `fixpoint_sdk-0.9.0/examples/direct_logging.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/examples/function_calling.py` & `fixpoint_sdk-0.9.0/examples/function_calling.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/examples/main.py` & `fixpoint_sdk-0.9.0/examples/main.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/examples/router.py` & `fixpoint_sdk-0.9.0/examples/router.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/examples/streaming.py` & `fixpoint_sdk-0.9.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/__init__.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/_logging_api.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/_logging_api.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/_mock_completions.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/_mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/client.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/client.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/compat.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/compat.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/completions.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/_mock_requests.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/_mock_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/debugging.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/debugging.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/env.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/env.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/exc.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/exc.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/iterwrapper.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/lib/requests.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/lib/requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/types/__init__.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/types/_utils.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/types/_utils.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/src/fixpoint_sdk/types/openai.py` & `fixpoint_sdk-0.9.0/src/fixpoint_sdk/types/openai.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/tests/mock_completions.py` & `fixpoint_sdk-0.9.0/tests/mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/tests/test_client.py` & `fixpoint_sdk-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/tests/test_completions.py` & `fixpoint_sdk-0.9.0/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/tests/test_types.py` & `fixpoint_sdk-0.9.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/tests/lib/test_iterwrapper.py` & `fixpoint_sdk-0.9.0/tests/lib/test_iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/tests/lib/test_requests.py` & `fixpoint_sdk-0.9.0/tests/lib/test_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/tests/types/test_openai.py` & `fixpoint_sdk-0.9.0/tests/types/test_openai.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/LICENSE` & `fixpoint_sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/README.md` & `fixpoint_sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.8.2/pyproject.toml` & `fixpoint_sdk-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fixpoint_sdk"
-version = "0.8.2"
+version = "0.9.0"
 
 authors = [
 { name="Jakub Cichon", email="jakub@fixpoint.co" },
 { name="Dylan Mikus", email="dylan@fixpoint.co" },
 ]
 description = "Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter"
 readme = "README.md"
@@ -21,15 +21,15 @@
 
 dependencies = [
   "openai>=1.6.1",
   "requests==2.31.0",
   "python-dateutil>=2.8.2",
   "pydantic>=2",
   "typing-extensions>=4.7.1",
-  "fixpoint-openapi==0.2.0"
+  "fixpoint-openapi==0.3.0"
 ]
 
 [project.optional-dependencies]
 dev = [
   "black>=24",
   "build>=1.1.1",
   "ipdb>=0.13.13",
```

### Comparing `fixpoint_sdk-0.8.2/PKG-INFO` & `fixpoint_sdk-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: fixpoint_sdk
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter
 Project-URL: Homepage, https://github.com/gofixpoint/python-sdk
 Project-URL: Issues, https://github.com/gofixpoint/python-sdk/issues
 Author-email: Jakub Cichon <jakub@fixpoint.co>, Dylan Mikus <dylan@fixpoint.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: fixpoint-openapi==0.2.0
+Requires-Dist: fixpoint-openapi==0.3.0
 Requires-Dist: openai>=1.6.1
 Requires-Dist: pydantic>=2
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: typing-extensions>=4.7.1
 Provides-Extra: dev
 Requires-Dist: black>=24; extra == 'dev'
```

