# Comparing `tmp/loopquest-0.2.8.tar.gz` & `tmp/loopquest-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.2.8.tar", last modified: Wed May 22 05:54:07 2024, max compression
+gzip compressed data, was "loopquest-0.2.9.tar", last modified: Sun Jun  2 18:29:26 2024, max compression
```

## Comparing `loopquest-0.2.8.tar` & `loopquest-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.216314 loopquest-0.2.8/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.8/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-22 05:54:07.216314 loopquest-0.2.8/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5380 2024-05-21 03:41:05.000000 loopquest-0.2.8/README.md
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.212314 loopquest-0.2.8/loopquest/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.8/loopquest/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1465 2024-05-21 03:27:00.000000 loopquest-0.2.8/loopquest/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9814 2024-05-21 05:03:28.000000 loopquest-0.2.8/loopquest/crud.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1943 2024-05-21 03:39:28.000000 loopquest-0.2.8/loopquest/datasets.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.212314 loopquest-0.2.8/loopquest/env/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.8/loopquest/env/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.8/loopquest/env/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6400 2024-05-22 05:47:04.000000 loopquest-0.2.8/loopquest/env/gym_wrappers.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/env/space_utils.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6321 2024-05-18 04:12:03.000000 loopquest-0.2.8/loopquest/eval.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.216314 loopquest-0.2.8/loopquest/policy/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/policy/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      281 2024-05-17 06:20:02.000000 loopquest-0.2.8/loopquest/policy/base.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/policy/sb3_policy.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1961 2024-05-22 05:53:20.000000 loopquest-0.2.8/loopquest/private_api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5916 2024-05-21 03:48:15.000000 loopquest-0.2.8/loopquest/schema.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/typing.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.8/loopquest/ui.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-19 04:55:08.000000 loopquest-0.2.8/loopquest/utils.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.216314 loopquest-0.2.8/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/SOURCES.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/dependency_links.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/requires.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/top_level.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-22 05:54:07.216314 loopquest-0.2.8/setup.cfg
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-22 05:51:43.000000 loopquest-0.2.8/setup.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-06-02 18:29:26.885941 loopquest-0.2.9/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.9/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-06-02 18:29:26.885941 loopquest-0.2.9/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5380 2024-05-21 03:41:05.000000 loopquest-0.2.9/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-06-02 18:29:26.881941 loopquest-0.2.9/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.9/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1233 2024-06-02 17:08:59.000000 loopquest-0.2.9/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9776 2024-06-02 17:10:49.000000 loopquest-0.2.9/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     2464 2024-06-02 17:15:05.000000 loopquest-0.2.9/loopquest/datasets.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-06-02 18:29:26.885941 loopquest-0.2.9/loopquest/env/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.9/loopquest/env/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.9/loopquest/env/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6400 2024-05-23 14:19:40.000000 loopquest-0.2.9/loopquest/env/gym_wrappers.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.9/loopquest/env/space_utils.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6321 2024-05-18 04:12:03.000000 loopquest-0.2.9/loopquest/eval.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-06-02 18:29:26.885941 loopquest-0.2.9/loopquest/policy/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.9/loopquest/policy/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      281 2024-05-17 06:20:02.000000 loopquest-0.2.9/loopquest/policy/base.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.9/loopquest/policy/sb3_policy.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1803 2024-06-02 17:09:55.000000 loopquest-0.2.9/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5916 2024-06-02 17:07:15.000000 loopquest-0.2.9/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.9/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.9/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-19 04:55:08.000000 loopquest-0.2.9/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-06-02 18:29:26.885941 loopquest-0.2.9/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-06-02 18:29:26.000000 loopquest-0.2.9/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-06-02 18:29:26.000000 loopquest-0.2.9/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-06-02 18:29:26.000000 loopquest-0.2.9/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-06-02 18:29:26.000000 loopquest-0.2.9/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-06-02 18:29:26.000000 loopquest-0.2.9/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-06-02 18:29:26.885941 loopquest-0.2.9/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-06-02 17:15:21.000000 loopquest-0.2.9/setup.py
```

### Comparing `loopquest-0.2.8/LICENSE` & `loopquest-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/PKG-INFO` & `loopquest-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.8/README.md` & `loopquest-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/loopquest/api.py` & `loopquest-0.2.9/loopquest/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,20 +25,15 @@
         token = getpass.getpass("Enter your LoopQuest user token: ").strip()
         if verify_token(token):
             print("Token is verified.")
             break
         else:
             print("Token is invalid. Please try again.")
 
-    print(
-        "Saving the token to .env file... Please keep your token safe. DO NOT share this token with others!"
-    )
     save_token_to_env(token)
-    print("In case .env file is tracked by git, Adding .env to .gitignore...")
-    add_env_to_gitignore()
     print("LoopQuest is initialized.")
 
 
 def is_initialized():
     return is_cloud_instance_initialized()
```

### Comparing `loopquest-0.2.8/loopquest/crud.py` & `loopquest-0.2.9/loopquest/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,29 +18,27 @@
     replace_special_chars_with_dash,
 )
 import numpy as np
 import gymnasium
 from PIL import Image
 from io import BytesIO
 from .private_api import TOKEN_ENV_VAR_NAME
-from dotenv import load_dotenv
+
 import os
 from requests.exceptions import HTTPError
 
-load_dotenv()
-
 
 def make_request(method: str, url: str, skip_auth_check=False, **kwargs):
     if not skip_auth_check:
         if TOKEN_ENV_VAR_NAME not in os.environ:
             raise Exception(
                 f"Please run loopquest.init() before calling other loopquest functions."
             )
         headers = kwargs.get("headers", {})
-        headers["Authorization"] = f"{os.getenv(TOKEN_ENV_VAR_NAME)}"
+        headers["Authorization"] = f"Bearer {os.getenv(TOKEN_ENV_VAR_NAME)}"
         kwargs["headers"] = headers
 
     try:
         response = requests.request(method, url, **kwargs)
         response.raise_for_status()
     except HTTPError as e:
         if e.response.status_code == 500:
```

### Comparing `loopquest-0.2.8/loopquest/datasets.py` & `loopquest-0.2.9/loopquest/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 from datasets import Dataset
-from .crud import get_steps_by_experiment, get_image_by_id
+from .crud import (
+    get_steps_by_experiment,
+    get_image_by_id,
+    get_environment,
+    get_experiment,
+)
 from .api import get_backend_url
 from .env.space_utils import recover_from_space_val
-from PIL import Image
 
 
 def dataset_gen(experiment_ids: list[str]):
     for experiment_id in experiment_ids:
         # TODO: this can be further optimized by fetching a batch of steps at a
         # time. Maybe this is already considered by huggingface datasets?
+        exp = get_experiment(get_backend_url(), experiment_id)
+        envs = {}
+        for env_id in exp.environment_ids:
+            envs[env_id] = get_environment(get_backend_url(), env_id)
+
         steps = get_steps_by_experiment(get_backend_url(), experiment_id)
         for step in steps:
             step_dict = step.model_dump()
             step_dict["observation"] = recover_from_space_val(step.observation)
             if step.action is not None:
                 step_dict["action"] = recover_from_space_val(step.action)
+            step_dict["env_metadata"] = envs[step.environment_id].metadata
+            # step_dict["action_metadata"] = envs[step.environment_id].action_metadata
+            # step_dict["observation_metadata"] = envs[
+            #     step.environment_id
+            # ].observation_metadata
+
             yield step_dict
 
 
 def to_pilow(examples):
     image_ids_across_examples = examples["image_ids"]
     images = [
         [get_image_by_id(get_backend_url(), id) for id in image_ids]
```

### Comparing `loopquest-0.2.8/loopquest/env/api.py` & `loopquest-0.2.9/loopquest/env/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/loopquest/env/gym_wrappers.py` & `loopquest-0.2.9/loopquest/env/gym_wrappers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -126,20 +126,20 @@
             ),
         )
         return observation, info
 
     def close(self):
         self.env.close()
         self.executor.shutdown()
+        self._try_update_env_profile_image()
         update_experiment(
             self.backend_url,
             self.exp_id,
             ExperimentUpdate(status=ExperimentStatus.FINISHED),
         )
-        self._try_update_env_profile_image()
         # TODO: add a callback to compute custom metrics.
 
     def _try_update_env_profile_image(self):
         env_info = get_environment(self.backend_url, self.cloud_env_id)
         env_update = EnvironmentUpdate()
         if env_info.profile_image_id is None:
             image_ids = get_image_ids_by_step(
```

### Comparing `loopquest-0.2.8/loopquest/env/space_utils.py` & `loopquest-0.2.9/loopquest/env/space_utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/loopquest/eval.py` & `loopquest-0.2.9/loopquest/eval.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/loopquest/policy/sb3_policy.py` & `loopquest-0.2.9/loopquest/policy/sb3_policy.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/loopquest/private_api.py` & `loopquest-0.2.9/loopquest/private_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,23 @@
     except Exception as e:
         return False
 
 
 def verify_token(token):
     try:
         response = requests.get(
-            f"{CLOUD_BACKEND_URL}/user_id", headers={"Authorization": f"{token}"}
+            f"{CLOUD_BACKEND_URL}/user_id", headers={"Authorization": f"Bearer {token}"}
         )
         response.raise_for_status()
         return True
     except:
         return False
 
 
 def save_token_to_env(token):
-    update_or_append_env_var(
-        TOKEN_ENV_VAR_NAME,
-        token,
-        comment="WARNING: This token is very sensitive. Do not publish it anywhere!",
-    )
     os.environ[TOKEN_ENV_VAR_NAME] = token
 
 
 def add_env_to_gitignore():
     gitignore_path = os.path.join(os.getcwd(), ".gitignore")
     if os.path.exists(gitignore_path):
         if is_dotenv_in_gitignore(gitignore_path):
```

### Comparing `loopquest-0.2.8/loopquest/schema.py` & `loopquest-0.2.9/loopquest/schema.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/loopquest/utils.py` & `loopquest-0.2.9/loopquest/utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/loopquest.egg-info/PKG-INFO` & `loopquest-0.2.9/loopquest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.8/loopquest.egg-info/SOURCES.txt` & `loopquest-0.2.9/loopquest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.8/setup.py` & `loopquest-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.2.8",
+    version="0.2.9",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
     packages=find_packages(),
```

