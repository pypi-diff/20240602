# Comparing `tmp/prompt_defender-0.0.28.tar.gz` & `tmp/prompt_defender-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "prompt_defender-0.1.1.tar", max compression
```

## Comparing `prompt_defender-0.0.28.tar` & `prompt_defender-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,41 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.coverage
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.coveragerc
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/example.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/requirements.txt
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.github/workflows/deploy-prod.yml
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.github/workflows/python-app.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/drawbridge/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/drawbridge/drawbridge.py
--rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/build.sh
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/deploy-prod.sh
--rwxr-xr-x   0        0        0      225 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/deploy.sh
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/set_version.py
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/tests.sh
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/test_prompt_defender_client.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/test_prompt_validator.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/test_xml_scanner.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/wall_test.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/example.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/prompt_defender_client.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/prompt_defender_client_rapidapi.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/prompt_validator.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/wall_builder.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/wall_executor.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/xml_scanner.py
--rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/README.md
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/pyproject.toml
--rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0     5211 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/README.md
+-rw-r--r--   0        0        0      237 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/__init__.py
+-rw-r--r--   0        0        0      250 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/core/__init__.py
+-rw-r--r--   0        0        0      520 2024-06-02 18:43:07.667898 prompt_defender-0.1.1/prompt_defender/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2178 2024-06-02 18:43:07.759898 prompt_defender-0.1.1/prompt_defender/core/__pycache__/defence.cpython-310.pyc
+-rw-r--r--   0        0        0      995 2024-06-02 18:43:07.671898 prompt_defender-0.1.1/prompt_defender/core/__pycache__/drawbridge_executor.cpython-310.pyc
+-rw-r--r--   0        0        0     1049 2024-06-02 18:43:07.755898 prompt_defender-0.1.1/prompt_defender/core/__pycache__/keep_executor.cpython-310.pyc
+-rw-r--r--   0        0        0     1606 2024-06-02 18:43:07.759898 prompt_defender-0.1.1/prompt_defender/core/__pycache__/wall_executor.cpython-310.pyc
+-rw-r--r--   0        0        0     1977 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/core/defence.py
+-rw-r--r--   0        0        0      413 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/core/drawbridge_executor.py
+-rw-r--r--   0        0        0      507 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/core/keep_executor.py
+-rw-r--r--   0        0        0      802 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/core/wall_executor.py
+-rw-r--r--   0        0        0       77 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/drawbridge/__init__.py
+-rw-r--r--   0        0        0      298 2024-06-02 18:43:07.591899 prompt_defender-0.1.1/prompt_defender/drawbridge/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2416 2024-06-02 18:43:07.591899 prompt_defender-0.1.1/prompt_defender/drawbridge/__pycache__/default_drawbridge_executor.cpython-310.pyc
+-rw-r--r--   0        0        0     1925 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/drawbridge/default_drawbridge_executor.py
+-rw-r--r--   0        0        0       45 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/keep/__init__.py
+-rw-r--r--   0        0        0      250 2024-06-02 18:43:07.763898 prompt_defender-0.1.1/prompt_defender/keep/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2997 2024-06-02 18:43:07.763898 prompt_defender-0.1.1/prompt_defender/keep/__pycache__/remote_keep.cpython-310.pyc
+-rw-r--r--   0        0        0     2513 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/keep/remote_keep.py
+-rw-r--r--   0        0        0      103 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/tests/__init__.py
+-rw-r--r--   0        0        0      319 2024-06-02 18:43:07.779898 prompt_defender-0.1.1/prompt_defender/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2037 2024-06-02 18:43:07.783898 prompt_defender-0.1.1/prompt_defender/tests/__pycache__/test_defence.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1674 2024-06-02 18:43:07.783898 prompt_defender-0.1.1/prompt_defender/tests/__pycache__/test_prompt_defender_client.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1552 2024-06-02 18:43:07.787898 prompt_defender-0.1.1/prompt_defender/tests/__pycache__/test_prompt_validator.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1135 2024-06-02 18:43:07.787898 prompt_defender-0.1.1/prompt_defender/tests/__pycache__/test_xml_scanner.cpython-310-pytest-8.0.2.pyc
+-rw-r--r--   0        0        0     1356 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/tests/test_defence.py
+-rw-r--r--   0        0        0     1216 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/tests/test_prompt_defender_client.py
+-rw-r--r--   0        0        0     1126 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/tests/test_prompt_validator.py
+-rw-r--r--   0        0        0      575 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/tests/test_xml_scanner.py
+-rw-r--r--   0        0        0      159 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/wall/__init__.py
+-rw-r--r--   0        0        0      384 2024-06-02 18:43:07.767898 prompt_defender-0.1.1/prompt_defender/wall/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5267 2024-06-02 18:43:07.771898 prompt_defender-0.1.1/prompt_defender/wall/__pycache__/prompt_defender_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1498 2024-06-02 18:43:07.779898 prompt_defender-0.1.1/prompt_defender/wall/__pycache__/prompt_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1577 2024-06-02 18:43:07.767898 prompt_defender-0.1.1/prompt_defender/wall/__pycache__/xml_scanner.cpython-310.pyc
+-rw-r--r--   0        0        0     5529 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/wall/prompt_defender_client.py
+-rw-r--r--   0        0        0     1179 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/wall/prompt_validator.py
+-rw-r--r--   0        0        0     2634 2024-06-02 18:42:55.811926 prompt_defender-0.1.1/prompt_defender/wall/wall_executor.py
+-rw-r--r--   0        0        0      989 2024-06-02 18:42:55.815926 prompt_defender-0.1.1/prompt_defender/wall/xml_scanner.py
+-rw-r--r--   0        0        0     1156 2024-06-02 18:42:55.815926 prompt_defender-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 prompt_defender-0.1.1/PKG-INFO
```

### Comparing `prompt_defender-0.0.28/drawbridge/drawbridge.py` & `prompt_defender-0.1.1/prompt_defender/drawbridge/default_drawbridge_executor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,51 @@
+from typing import Callable, Optional
+
 import bleach
-from pydantic import BaseModel
+
+from ..core import DrawbridgeExecutor, DrawbridgeResponse
 
 
 def __check_for_canary__(canary: str, llm_response: str) -> bool:
     return canary in llm_response
 
 
-class Drawbridge(BaseModel):
+class DefaultDrawbridgeExecutor(DrawbridgeExecutor):
     """
     Drawbridge is a class that can be used to validate the response of an LLM execution
     """
-    canary: str
+    canary: Optional[str] = None
     allow_unsafe_scripts: bool = False
 
-    def validate_response_and_clean(self, response: str) -> (bool, str):
-        response_ok = __check_for_canary__(self.canary, response)
+    def validate_response_and_clean(self, response: str) -> DrawbridgeResponse:
+        if self.canary:
+            response_ok = __check_for_canary__(self.canary, response)
+        else:
+            response_ok = True
 
         if not self.allow_unsafe_scripts:
             response = bleach.clean(response, strip=True)
 
-        return response_ok, response
+        return DrawbridgeResponse(is_safe=response_ok, cleaned_response=response)
 
 
-def build_drawbridge(canary: str, allow_unsafe_scripts: bool = False) -> Drawbridge:
+def _build_drawbridge(canary: Optional[str], allow_unsafe_scripts: bool = False) -> DrawbridgeExecutor:
     """
     Factory function to build a Drawbridge object
 
     :param canary: what to look for in the response to validate if a canary was returned
     :param allow_unsafe_scripts: whether or not to allow scripts in the response. If False, scripts will be removed
 
     :return: Drawbridge object which you can call validate_response_and_clean oon to validate and clean the response
     """
-    return Drawbridge(canary=canary, allow_unsafe_scripts=allow_unsafe_scripts)
+    return DefaultDrawbridgeExecutor(canary=canary, allow_unsafe_scripts=allow_unsafe_scripts)
+
+
+def build_drawbridge(allow_unsafe_scripts: bool = False) -> Callable[[str], DrawbridgeExecutor]:
+    """
+    Factory function to build a Drawbridge object
+
+    :param allow_unsafe_scripts: whether or not to allow scripts in the response. If False, scripts will be removed
+
+    :return: Drawbridge object which you can call validate_response_and_clean oon to validate and clean the response
+    """
+    return lambda x: _build_drawbridge(x, allow_unsafe_scripts=allow_unsafe_scripts)
```

### Comparing `prompt_defender-0.0.28/tests/test_prompt_defender_client.py` & `prompt_defender-0.1.1/prompt_defender/tests/test_prompt_defender_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import requests_mock
 
-from wall.prompt_defender_client import PromptDefenderClient, WallResponse
+from prompt_defender.wall.prompt_defender_client import PromptDefenderClient, WallResponse
 
 
 class TestPromptDefenderClient(unittest.TestCase):
     def setUp(self):
         self.client = PromptDefenderClient(api_key="test_key")
         self.mock_server = requests_mock.Mocker()
```

### Comparing `prompt_defender-0.0.28/tests/test_prompt_validator.py` & `prompt_defender-0.1.1/prompt_defender/tests/test_prompt_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import unittest
-from wall.prompt_validator import PromptValidator
+from prompt_defender.wall.prompt_validator import PromptValidator
 
 
 class TestPromptValidator(unittest.TestCase):
 
     def test_validate_length(self):
         pv = PromptValidator(max_length=5)
-        self.assertFalse(pv.validate_prompt("This prompt is longer than acceptable"))
+        self.assertTrue(pv.validate_prompt("This prompt is longer than acceptable").unacceptable_prompt)
 
     def test_validate_length_is_ok(self):
         pv = PromptValidator(max_length=100)
-        self.assertTrue(pv.validate_prompt("This prompt is longer than acceptable"))
+        self.assertFalse(pv.validate_prompt("This prompt is not longer than acceptable").unacceptable_prompt)
 
     def test_validate_prompt(self):
         pv = PromptValidator(max_length=100, acceptable_values=['hello', 'world'])
-        self.assertTrue(pv.validate_prompt('hello'))
-        self.assertTrue(pv.validate_prompt('world'))
-        self.assertFalse(pv.validate_prompt('invalid'))
-        self.assertFalse(pv.validate_prompt('hell'))
+        self.assertFalse(pv.validate_prompt('hello').unacceptable_prompt)
+        self.assertFalse(pv.validate_prompt('world').unacceptable_prompt)
+        self.assertTrue(pv.validate_prompt('invalid').unacceptable_prompt)
+        self.assertTrue(pv.validate_prompt('hell').unacceptable_prompt)
 
         pv = PromptValidator(max_length=None, acceptable_values=None)
-        self.assertTrue(pv.validate_prompt('any value'))
+        self.assertFalse(pv.validate_prompt('any value').unacceptable_prompt)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `prompt_defender-0.0.28/wall/wall_executor.py` & `prompt_defender-0.1.1/prompt_defender/wall/wall_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,41 @@
 from typing import Optional
 
-from pydantic import BaseModel
-
+from core import ValidationResult, WallExecutor
 from .prompt_defender_client import PromptDefenderClient, WallResponse
 from .prompt_validator import PromptValidator
 from .xml_scanner import BasicXmlScanner
 
 
-class ValidationResult(BaseModel):
-    contains_pii: Optional[bool] = None
-    potential_jailbreak: bool
-    potential_xml_escaping: Optional[bool] = None
-    suspicious_user: Optional[bool] = None
-    suspicious_session: Optional[bool] = None
-
-
-def should_block_prompt(validation_result: ValidationResult) -> bool:
-    return validation_result.contains_pii or \
-        validation_result.potential_jailbreak or \
-        validation_result.potential_xml_escaping or \
-        validation_result.suspicious_user or \
-        validation_result.suspicious_session
-
-
-class WallExecutor(BaseModel):
+class WallExecutorRemote(WallExecutor):
     xml_scanner: Optional[BasicXmlScanner] = None
     prompt_validator: Optional[PromptValidator] = None
     remote_wall_checker: Optional[PromptDefenderClient] = None
 
     def __execute_xml_scanner__(self, prompt: str) -> bool:
         if self.xml_scanner is not None:
             return self.xml_scanner.check_for_xml_tag(prompt)
         else:
             return False
 
     def __execute_prompt_validator__(self, prompt: str) -> bool:
         if self.prompt_validator is not None:
-            return self.prompt_validator.validate_prompt(prompt)
+            return self.prompt_validator.validate_prompt(prompt).unacceptable_prompt
         else:
             return False
 
     def __execute_remote_wall_checker__(self, prompt: str) -> Optional[WallResponse]:
         if self.remote_wall_checker is not None:
             return self.remote_wall_checker.call_remote_wall(prompt)
         return None
 
-    def validate_prompt(self, prompt: str) -> ValidationResult:
+    def validate_prompt(self, prompt: str,
+                        xml_tag: Optional[str] = None,
+                        user_id: Optional[str] = None,
+                        session_id: Optional[str] = None) -> ValidationResult:
         """
         Validate a prompt
         :param prompt: The prompt to validate
         :return: validation result
         """
         xml_injection_detected = self.__execute_xml_scanner__(prompt)
         prompt_validator_failed = not self.__execute_prompt_validator__(prompt)
```

### Comparing `prompt_defender-0.0.28/README.md` & `prompt_defender-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,49 +6,34 @@
 ## Installation
 
 ```pip install prompt-defender```
 
 ## Quick start
 
 ```python
-from wall.wall_executor import should_block_prompt, create_wall
+from prompt_defender import CompositeWallExecutorBuilder, build_drawbridge, remote_keep_builder, build_xml_scanner, build_remote_wall_executor, build_prompt_validator, Defence
+
+if __name__ == "__main__":
+  compose_wall = CompositeWallExecutorBuilder()
+  compose_wall.add_wall_executor(build_xml_scanner)
+  compose_wall.add_wall_executor(build_remote_wall_executor(fast_check=True))
+  compose_wall.add_wall_executor(build_prompt_validator())
+
+  defence = Defence(
+    wall=compose_wall.build(),
+    keep=remote_keep_builder(),
+    drawbridge=build_drawbridge(allow_unsafe_scripts=True)
+  )
+
+  prepared_prompt = defence.prepare_prompt("Your job is to answer user questions about cats {user_question}")
+
+  print(defence.check_user_input("What is the best cat? " + prepared_prompt.safe_prompt))
+
+  print(defence.check_prompt_output("This should all be okay "))
 
-wall = create_wall(
-    # These options first require you to have a Prompt Defender account which you can sign up for at
-    # https://defender.safetorun.com. Once you have an account you can get an API key  to use with the wall.
-    remote_jailbreak_check=True,
-    api_key="test_key",
-    user_id="test_user",
-    session_id="test_session",
-    allow_pii=False,
-
-    # When you create a prompt, with Prompt Defender - Keep, you will get
-    # an XML tag that wraps user input. Pass this tag to the remote endpoint
-    # in order to check for potential XML escaping which is likely because
-    # someone is trying to attack your system
-    xml_tag="tag",
-
-    # The following are used for prompt validation - if you are only
-    # expecting a certain number of values, or a certain length of prompt
-    # you can use these to enforce that.
-
-    max_prompt_length=100,
-    allowed_prompt_values=["hello", "world"]
-)
-
-validation_response = wall.validate_prompt("hello")
-
-if validation_response.contains_pii:
-    print("Prompt contains PII")
-elif validation_response.suspicious_user:  # etc etc etc
-    print("Prompt is suspicious")
-elif should_block_prompt(validation_response):
-    print("Prompt should be blocked")
-else:
-    print("Prompt is OK")
 ```
 
 ## Wall
 
 Wall is a part of the Prompt Defender project that is responsible for validating prompts. It uses a combination of
 local and remote checks to ensure the safety and validity of the prompts. The main component of the Wall is
 the `create_wall` function, which orchestrates the execution of the different validation checks.
```

### Comparing `prompt_defender-0.0.28/PKG-INFO` & `prompt_defender-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,57 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: prompt-defender
-Version: 0.0.28
+Version: 0.1.1
 Summary: Prompt Defender. A package to help you defend against prompt injection attacks.
-Project-URL: Homepage, https://github.com/safetorun/PromptDefender-py
-Project-URL: Issues, https://github.com/safetorun/PromptDefender-py/issues
-Author-email: Daniel Llewellyn <admin@safetorun.com>
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Author: Daniel Llewellyn
+Author-email: admin@safetorun.com
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: bleach==6.1.0
-Requires-Dist: dataclasses-json==0.6.4
-Requires-Dist: pydantic-core==2.16.3
-Requires-Dist: pydantic==2.6.3
-Requires-Dist: requests==2.31.0
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bleach (>=6.1.0,<7.0.0)
+Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Prompt Defender
 ![PyPI](https://img.shields.io/pypi/v/prompt-defender)
 
 Read the documentation at [Prompt Defender - Docs](https://promptshield.readme.io/docs)
 
 ## Installation
 
 ```pip install prompt-defender```
 
 ## Quick start
 
 ```python
-from wall.wall_executor import should_block_prompt, create_wall
+from prompt_defender import CompositeWallExecutorBuilder, build_drawbridge, remote_keep_builder, build_xml_scanner, build_remote_wall_executor, build_prompt_validator, Defence
+
+if __name__ == "__main__":
+  compose_wall = CompositeWallExecutorBuilder()
+  compose_wall.add_wall_executor(build_xml_scanner)
+  compose_wall.add_wall_executor(build_remote_wall_executor(fast_check=True))
+  compose_wall.add_wall_executor(build_prompt_validator())
+
+  defence = Defence(
+    wall=compose_wall.build(),
+    keep=remote_keep_builder(),
+    drawbridge=build_drawbridge(allow_unsafe_scripts=True)
+  )
+
+  prepared_prompt = defence.prepare_prompt("Your job is to answer user questions about cats {user_question}")
+
+  print(defence.check_user_input("What is the best cat? " + prepared_prompt.safe_prompt))
+
+  print(defence.check_prompt_output("This should all be okay "))
 
-wall = create_wall(
-    # These options first require you to have a Prompt Defender account which you can sign up for at
-    # https://defender.safetorun.com. Once you have an account you can get an API key  to use with the wall.
-    remote_jailbreak_check=True,
-    api_key="test_key",
-    user_id="test_user",
-    session_id="test_session",
-    allow_pii=False,
-
-    # When you create a prompt, with Prompt Defender - Keep, you will get
-    # an XML tag that wraps user input. Pass this tag to the remote endpoint
-    # in order to check for potential XML escaping which is likely because
-    # someone is trying to attack your system
-    xml_tag="tag",
-
-    # The following are used for prompt validation - if you are only
-    # expecting a certain number of values, or a certain length of prompt
-    # you can use these to enforce that.
-
-    max_prompt_length=100,
-    allowed_prompt_values=["hello", "world"]
-)
-
-validation_response = wall.validate_prompt("hello")
-
-if validation_response.contains_pii:
-    print("Prompt contains PII")
-elif validation_response.suspicious_user:  # etc etc etc
-    print("Prompt is suspicious")
-elif should_block_prompt(validation_response):
-    print("Prompt should be blocked")
-else:
-    print("Prompt is OK")
 ```
 
 ## Wall
 
 Wall is a part of the Prompt Defender project that is responsible for validating prompts. It uses a combination of
 local and remote checks to ensure the safety and validity of the prompts. The main component of the Wall is
 the `create_wall` function, which orchestrates the execution of the different validation checks.
@@ -141,7 +126,8 @@
 Next, we have a response string that we want to validate and clean. We pass this response to the
 validate_response_and_clean method of our Drawbridge instance. This method returns two values:
 
 * response_ok: This is a boolean value that indicates whether the canary was found in the response.
 * cleaned_response: This is the cleaned version of the response. If allow_unsafe_scripts is False (which is the
   default),
   any scripts in the response will be removed.
+
```

