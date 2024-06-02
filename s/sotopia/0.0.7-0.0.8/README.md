# Comparing `tmp/sotopia-0.0.7.tar.gz` & `tmp/sotopia-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotopia-0.0.7.tar", max compression
+gzip compressed data, was "sotopia-0.0.8.tar", max compression
```

## Comparing `sotopia-0.0.7.tar` & `sotopia-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1064 2024-05-28 19:13:02.448295 sotopia-0.0.7/LICENSE
--rw-r--r--   0        0        0     9151 2024-05-28 19:13:02.448295 sotopia-0.0.7/README.md
--rw-r--r--   0        0        0     1951 2024-05-28 19:13:02.460296 sotopia-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/__init__.py
--rw-r--r--   0        0        0      494 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/base_agent.py
--rw-r--r--   0        0        0     2914 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/generate_agent_background.py
--rw-r--r--   0        0        0     8021 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/llm_agent.py
--rw-r--r--   0        0        0     6764 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/agents/redis_agent.py
--rw-r--r--   0        0        0     1854 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/__init__.py
--rw-r--r--   0        0        0     4284 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/aggregate_annotations.py
--rw-r--r--   0        0        0      187 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/annotators.py
--rw-r--r--   0        0        0      315 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/auto_expires_mixin.py
--rw-r--r--   0        0        0      248 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/env_agent_combo_storage.py
--rw-r--r--   0        0        0        8 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/handshake.py
--rw-r--r--   0        0        0     3358 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/logs.py
--rw-r--r--   0        0        0     5262 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/persistent_profile.py
--rw-r--r--   0        0        0    21934 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/serialization.py
--rw-r--r--   0        0        0     1398 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/session_transaction.py
--rw-r--r--   0        0        0      406 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/database/waiting_room.py
--rw-r--r--   0        0        0       75 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/envs/__init__.py
--rw-r--r--   0        0        0    30043 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/envs/evaluators.py
--rw-r--r--   0        0        0    22614 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/envs/parallel.py
--rw-r--r--   0        0        0      253 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/__init__.py
--rw-r--r--   0        0        0    35603 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/generate.py
--rw-r--r--   0        0        0     1476 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/langchain_callback_handler.py
--rw-r--r--   0        0        0     6567 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/generation_utils/llama2.py
--rw-r--r--   0        0        0      392 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/messages/__init__.py
--rw-r--r--   0        0        0    13319 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/messages/message_classes.py
--rw-r--r--   0        0        0      325 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/messages/messenger.py
--rw-r--r--   0        0        0        0 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/py.typed
--rw-r--r--   0        0        0      144 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/renderers/__init__.py
--rw-r--r--   0        0        0     1408 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/renderers/base.py
--rw-r--r--   0        0        0     2822 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/renderers/xml_renderer.py
--rw-r--r--   0        0        0      265 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/__init__.py
--rw-r--r--   0        0        0     1986 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/base_sampler.py
--rw-r--r--   0        0        0     6560 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/constraint_based_sampler.py
--rw-r--r--   0        0        0     4095 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/samplers/uniform_sampler.py
--rw-r--r--   0        0        0    16553 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/server.py
--rw-r--r--   0        0        0      167 2024-05-28 19:13:02.464296 sotopia-0.0.7/sotopia/utils.py
--rw-r--r--   0        0        0    11094 1970-01-01 00:00:00.000000 sotopia-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-06-02 21:10:55.534010 sotopia-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8970 2024-06-02 21:10:55.534010 sotopia-0.0.8/README.md
+-rw-r--r--   0        0        0     1951 2024-06-02 21:10:55.546010 sotopia-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/__init__.py
+-rw-r--r--   0        0        0      494 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/agents/__init__.py
+-rw-r--r--   0        0        0     1709 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/agents/base_agent.py
+-rw-r--r--   0        0        0     2914 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/agents/generate_agent_background.py
+-rw-r--r--   0        0        0     8021 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/agents/llm_agent.py
+-rw-r--r--   0        0        0     6764 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/agents/redis_agent.py
+-rw-r--r--   0        0        0     1854 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/__init__.py
+-rw-r--r--   0        0        0     4284 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/aggregate_annotations.py
+-rw-r--r--   0        0        0      187 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/annotators.py
+-rw-r--r--   0        0        0      315 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/auto_expires_mixin.py
+-rw-r--r--   0        0        0      248 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/env_agent_combo_storage.py
+-rw-r--r--   0        0        0        8 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/handshake.py
+-rw-r--r--   0        0        0     3358 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/logs.py
+-rw-r--r--   0        0        0     5262 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/persistent_profile.py
+-rw-r--r--   0        0        0    21934 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/serialization.py
+-rw-r--r--   0        0        0     1398 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/session_transaction.py
+-rw-r--r--   0        0        0      406 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/database/waiting_room.py
+-rw-r--r--   0        0        0       75 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/envs/__init__.py
+-rw-r--r--   0        0        0    30043 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/envs/evaluators.py
+-rw-r--r--   0        0        0    22614 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/envs/parallel.py
+-rw-r--r--   0        0        0      253 2024-06-02 21:10:55.546010 sotopia-0.0.8/sotopia/generation_utils/__init__.py
+-rw-r--r--   0        0        0    35603 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/generation_utils/generate.py
+-rw-r--r--   0        0        0     1476 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/generation_utils/langchain_callback_handler.py
+-rw-r--r--   0        0        0     6567 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/generation_utils/llama2.py
+-rw-r--r--   0        0        0      392 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/messages/__init__.py
+-rw-r--r--   0        0        0    13319 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/messages/message_classes.py
+-rw-r--r--   0        0        0      325 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/messages/messenger.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/py.typed
+-rw-r--r--   0        0        0      144 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/renderers/__init__.py
+-rw-r--r--   0        0        0     1408 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/renderers/base.py
+-rw-r--r--   0        0        0     2822 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/renderers/xml_renderer.py
+-rw-r--r--   0        0        0      265 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/samplers/__init__.py
+-rw-r--r--   0        0        0     1986 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/samplers/base_sampler.py
+-rw-r--r--   0        0        0     6560 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/samplers/constraint_based_sampler.py
+-rw-r--r--   0        0        0     4095 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/samplers/uniform_sampler.py
+-rw-r--r--   0        0        0    16553 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/server.py
+-rw-r--r--   0        0        0      167 2024-06-02 21:10:55.550010 sotopia-0.0.8/sotopia/utils.py
+-rw-r--r--   0        0        0    10914 1970-01-01 00:00:00.000000 sotopia-0.0.8/PKG-INFO
```

### Comparing `sotopia-0.0.7/LICENSE` & `sotopia-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/README.md` & `sotopia-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 <div style="width: 100%;">
   <img src="figs/title.png" style="width: 100%;" alt="sotopia"></img>
 </div>
 
-# Sotopia: an Open-ended Social Learning Environment
+<h1 align="center">Sotopia: an Open-ended Social Learning Environment</h1>
+
+<div align="center">
+
+[![pypi](https://img.shields.io/pypi/v/sotopia.svg)](https://pypi.python.org/pypi/sotopia)
+[![versions](https://img.shields.io/pypi/pyversions/sotopia.svg)](https://github.com/sotopia/sotopia)
+[![CI](https://img.shields.io/github/actions/workflow/status/sotopia-lab/sotopia/tests.yml?branch=main&logo=github&label=CI)](https://github.com/sotopia-lab/sotopia/actions?query=branch%3Amain)
+[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14hJOfzpA37PRUzdlFgiqVzUGIhhngqnz?usp=sharing)
+
 [![Project Page](https://img.shields.io/badge/Project-Page-green.svg)](https://www.sotopia.world/projects/sotopia)
 [![Paper PDF](https://img.shields.io/badge/Paper-PDF-red.svg)](https://arxiv.org/abs/2310.11667)
-[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3109/)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
-<a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![bear-ified](https://raw.githubusercontent.com/beartype/beartype-assets/main/badge/bear-ified.svg)](https://beartype.readthedocs.io)
-[![Github Action](https://github.com/XuhuiZhou/sotopia/actions/workflows/tests.yml/badge.svg?branch=main)]()
-[![Github Action](https://github.com/XuhuiZhou/sotopia/actions/workflows/pre-commit.yml/badge.svg?branch=main)]()
 [![Dataset](https://img.shields.io/badge/%F0%9F%A4%97-Sotopia%20Dataset-yellow)](https://huggingface.co/datasets/cmu-lti/sotopia)
 [![Demo](https://img.shields.io/badge/%F0%9F%A4%97-Sotopia%20Demo-orange)](https://huggingface.co/spaces/cmu-lti/sotopia-space/)
 
+
+
+</div>
+
 ## News
 
-* [05/2024] Sotopia will be presented at ICLR 2024 as a spotlight ⭐!
+* [05/2024] Sotopia is presented at ICLR 2024 as a spotlight ⭐!
 * [05/2024] We release [a simple tutorial](https://colab.research.google.com/drive/14hJOfzpA37PRUzdlFgiqVzUGIhhngqnz?usp=sharing) for you to run sotopia end-to-end on google colab.
 
 
 ## Introduction
 
 Sotopia is an open-ended social learning environment that allows agents to interact with each other and the environment. The environment is designed to be a platform for evaluating and faciliating social intelligence in language agents. The environment is designed to be open-ended, meaning that the environment can be easily extended to include new environments and new agents. The environment is also designed to be scalable, meaning that the environment can be easily scaled to include a large number of agents and environments.
 
@@ -33,14 +38,17 @@
   author = {Zhou*, Xuhui and Zhu*, Hao and Mathur, Leena and Zhang, Ruohong and Qi, Zhengyang and Yu, Haofei and Morency, Louis-Philippe and Bisk, Yonatan and Fried, Daniel and Neubig, Graham and Sap, Maarten},
   journal = {ICLR},
   year = {2024},
   url = {https://openreview.net/forum?id=mM7VurbA4r},
 }
 ```
 
+## Help
+See [documentation](https://docs.sotopia.world) for more details.
+
 
 ## Get started
 ### Use on Google Colab
 
 If you want to try it out on Google Colab first, please check out our Colab Tutorial Series:
 
 <ol>
```

### Comparing `sotopia-0.0.7/pyproject.toml` & `sotopia-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sotopia"
-version = "0.0.7"
+version = "0.0.8"
 description = "A platform for simulating and evaluating social interaction."
 authors = ["Hao Zhu <prokilchu@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "sotopia"}]
 
 [tool.poetry.dependencies]
@@ -20,15 +20,15 @@
 types-tqdm = "*"
 gin-config = "^0.5.0"
 absl-py = "^2.0.0"
 together = "^0.2.4"
 pydantic = "1.10.12"
 beartype = "^0.14.0"
 langchain-openai = "^0.0.5"
-litellm = "^1.23.12"
+litellm = "~1.23.12"
 
 # dependency versions for extras
 fastapi = { version = "^0.109.2", optional = true }
 tabulate = { version = "^0.9.0", optional = true }
 anthropic = { version = "^0.26.0", optional = true }
 xmltodict = { version = "^0.13.0", optional = true }
 groq = { version = "^0.4.2", optional = true }
```

### Comparing `sotopia-0.0.7/sotopia/agents/base_agent.py` & `sotopia-0.0.8/sotopia/agents/base_agent.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/agents/generate_agent_background.py` & `sotopia-0.0.8/sotopia/agents/generate_agent_background.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/agents/llm_agent.py` & `sotopia-0.0.8/sotopia/agents/llm_agent.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/agents/redis_agent.py` & `sotopia-0.0.8/sotopia/agents/redis_agent.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/database/__init__.py` & `sotopia-0.0.8/sotopia/database/__init__.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/database/aggregate_annotations.py` & `sotopia-0.0.8/sotopia/database/aggregate_annotations.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/database/logs.py` & `sotopia-0.0.8/sotopia/database/logs.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/database/persistent_profile.py` & `sotopia-0.0.8/sotopia/database/persistent_profile.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/database/serialization.py` & `sotopia-0.0.8/sotopia/database/serialization.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/database/session_transaction.py` & `sotopia-0.0.8/sotopia/database/session_transaction.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/envs/evaluators.py` & `sotopia-0.0.8/sotopia/envs/evaluators.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/envs/parallel.py` & `sotopia-0.0.8/sotopia/envs/parallel.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/generation_utils/generate.py` & `sotopia-0.0.8/sotopia/generation_utils/generate.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/generation_utils/langchain_callback_handler.py` & `sotopia-0.0.8/sotopia/generation_utils/langchain_callback_handler.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/generation_utils/llama2.py` & `sotopia-0.0.8/sotopia/generation_utils/llama2.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/messages/message_classes.py` & `sotopia-0.0.8/sotopia/messages/message_classes.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/renderers/base.py` & `sotopia-0.0.8/sotopia/renderers/base.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/renderers/xml_renderer.py` & `sotopia-0.0.8/sotopia/renderers/xml_renderer.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/samplers/base_sampler.py` & `sotopia-0.0.8/sotopia/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/samplers/constraint_based_sampler.py` & `sotopia-0.0.8/sotopia/samplers/constraint_based_sampler.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/samplers/uniform_sampler.py` & `sotopia-0.0.8/sotopia/samplers/uniform_sampler.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/sotopia/server.py` & `sotopia-0.0.8/sotopia/server.py`

 * *Files identical despite different names*

### Comparing `sotopia-0.0.7/PKG-INFO` & `sotopia-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 736f 746f  : 2.1.Name: soto
 00000020: 7069 610a 5665 7273 696f 6e3a 2030 2e30  pia.Version: 0.0
-00000030: 2e37 0a53 756d 6d61 7279 3a20 4120 706c  .7.Summary: A pl
+00000030: 2e38 0a53 756d 6d61 7279 3a20 4120 706c  .8.Summary: A pl
 00000040: 6174 666f 726d 2066 6f72 2073 696d 756c  atform for simul
 00000050: 6174 696e 6720 616e 6420 6576 616c 7561  ating and evalua
 00000060: 7469 6e67 2073 6f63 6961 6c20 696e 7465  ting social inte
 00000070: 7261 6374 696f 6e2e 0a4c 6963 656e 7365  raction..License
 00000080: 3a20 4d49 540a 4175 7468 6f72 3a20 4861  : MIT.Author: Ha
 00000090: 6f20 5a68 750a 4175 7468 6f72 2d65 6d61  o Zhu.Author-ema
 000000a0: 696c 3a20 7072 6f6b 696c 6368 7540 676d  il: prokilchu@gm
@@ -74,621 +74,610 @@
 00000490: 726f 7122 0a52 6571 7569 7265 732d 4469  roq".Requires-Di
 000004a0: 7374 3a20 6c61 6e67 6368 6169 6e20 283d  st: langchain (=
 000004b0: 3d30 2e31 2e35 290a 5265 7175 6972 6573  =0.1.5).Requires
 000004c0: 2d44 6973 743a 206c 616e 6763 6861 696e  -Dist: langchain
 000004d0: 2d6f 7065 6e61 6920 283e 3d30 2e30 2e35  -openai (>=0.0.5
 000004e0: 2c3c 302e 302e 3629 0a52 6571 7569 7265  ,<0.0.6).Require
 000004f0: 732d 4469 7374 3a20 6c69 7465 6c6c 6d20  s-Dist: litellm 
-00000500: 283e 3d31 2e32 332e 3132 2c3c 322e 302e  (>=1.23.12,<2.0.
-00000510: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-00000520: 3a20 6c78 6d6c 2028 3e3d 342e 392e 332c  : lxml (>=4.9.3,
-00000530: 3c35 2e30 2e30 290a 5265 7175 6972 6573  <5.0.0).Requires
-00000540: 2d44 6973 743a 206f 7065 6e61 6920 283e  -Dist: openai (>
-00000550: 3d31 2e31 312e 302c 3c32 2e30 2e30 290a  =1.11.0,<2.0.0).
-00000560: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000570: 616e 6461 7320 283e 3d32 2e31 2e31 2c3c  andas (>=2.1.1,<
-00000580: 332e 302e 3029 0a52 6571 7569 7265 732d  3.0.0).Requires-
-00000590: 4469 7374 3a20 7061 6e64 6173 2d73 7475  Dist: pandas-stu
-000005a0: 6273 0a52 6571 7569 7265 732d 4469 7374  bs.Requires-Dist
-000005b0: 3a20 7079 6461 6e74 6963 2028 3d3d 312e  : pydantic (==1.
-000005c0: 3130 2e31 3229 0a52 6571 7569 7265 732d  10.12).Requires-
-000005d0: 4469 7374 3a20 7265 6469 732d 6f6d 2028  Dist: redis-om (
-000005e0: 3e3d 302e 322e 312c 3c30 2e33 2e30 290a  >=0.2.1,<0.3.0).
-000005f0: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
-00000600: 6963 6820 283e 3d31 332e 362e 302c 3c31  ich (>=13.6.0,<1
-00000610: 342e 302e 3029 0a52 6571 7569 7265 732d  4.0.0).Requires-
-00000620: 4469 7374 3a20 7363 6970 7920 283e 3d31  Dist: scipy (>=1
-00000630: 2e31 332e 312c 3c32 2e30 2e30 2920 3b20  .13.1,<2.0.0) ; 
-00000640: 6578 7472 6120 3d3d 2022 6578 616d 706c  extra == "exampl
-00000650: 6573 220a 5265 7175 6972 6573 2d44 6973  es".Requires-Dis
-00000660: 743a 2074 6162 756c 6174 6520 283e 3d30  t: tabulate (>=0
-00000670: 2e39 2e30 2c3c 302e 3130 2e30 290a 5265  .9.0,<0.10.0).Re
-00000680: 7175 6972 6573 2d44 6973 743a 2074 6f67  quires-Dist: tog
-00000690: 6574 6865 7220 283e 3d30 2e32 2e34 2c3c  ether (>=0.2.4,<
-000006a0: 302e 332e 3029 0a52 6571 7569 7265 732d  0.3.0).Requires-
-000006b0: 4469 7374 3a20 746f 7263 6820 283e 3d32  Dist: torch (>=2
-000006c0: 2e33 2e30 2c3c 332e 302e 3029 203b 2065  .3.0,<3.0.0) ; e
-000006d0: 7874 7261 203d 3d20 2265 7861 6d70 6c65  xtra == "example
-000006e0: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
-000006f0: 3a20 7472 616e 7366 6f72 6d65 7273 2028  : transformers (
-00000700: 3e3d 342e 3431 2e30 2c3c 352e 302e 3029  >=4.41.0,<5.0.0)
-00000710: 203b 2065 7874 7261 203d 3d20 2265 7861   ; extra == "exa
-00000720: 6d70 6c65 7322 0a52 6571 7569 7265 732d  mples".Requires-
-00000730: 4469 7374 3a20 7479 7065 732d 7471 646d  Dist: types-tqdm
-00000740: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000750: 786d 6c74 6f64 6963 7420 283e 3d30 2e31  xmltodict (>=0.1
-00000760: 332e 302c 3c30 2e31 342e 3029 0a44 6573  3.0,<0.14.0).Des
-00000770: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000780: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000790: 646f 776e 0a0a 3c64 6976 2073 7479 6c65  down..<div style
-000007a0: 3d22 7769 6474 683a 2031 3030 253b 223e  ="width: 100%;">
-000007b0: 0a20 203c 696d 6720 7372 633d 2266 6967  .  <img src="fig
-000007c0: 732f 7469 746c 652e 706e 6722 2073 7479  s/title.png" sty
-000007d0: 6c65 3d22 7769 6474 683a 2031 3030 253b  le="width: 100%;
-000007e0: 2220 616c 743d 2273 6f74 6f70 6961 223e  " alt="sotopia">
-000007f0: 3c2f 696d 673e 0a3c 2f64 6976 3e0a 0a23  </img>.</div>..#
-00000800: 2053 6f74 6f70 6961 3a20 616e 204f 7065   Sotopia: an Ope
-00000810: 6e2d 656e 6465 6420 536f 6369 616c 204c  n-ended Social L
-00000820: 6561 726e 696e 6720 456e 7669 726f 6e6d  earning Environm
-00000830: 656e 740a 5b21 5b50 726f 6a65 6374 2050  ent.[![Project P
-00000840: 6167 655d 2868 7474 7073 3a2f 2f69 6d67  age](https://img
-00000850: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000860: 652f 5072 6f6a 6563 742d 5061 6765 2d67  e/Project-Page-g
-00000870: 7265 656e 2e73 7667 295d 2868 7474 7073  reen.svg)](https
-00000880: 3a2f 2f77 7777 2e73 6f74 6f70 6961 2e77  ://www.sotopia.w
-00000890: 6f72 6c64 2f70 726f 6a65 6374 732f 736f  orld/projects/so
-000008a0: 746f 7069 6129 0a5b 215b 5061 7065 7220  topia).[![Paper 
-000008b0: 5044 465d 2868 7474 7073 3a2f 2f69 6d67  PDF](https://img
-000008c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000008d0: 652f 5061 7065 722d 5044 462d 7265 642e  e/Paper-PDF-red.
-000008e0: 7376 6729 5d28 6874 7470 733a 2f2f 6172  svg)](https://ar
-000008f0: 7869 762e 6f72 672f 6162 732f 3233 3130  xiv.org/abs/2310
-00000900: 2e31 3136 3637 290a 5b21 5b50 7974 686f  .11667).[![Pytho
-00000910: 6e20 332e 3131 5d28 6874 7470 733a 2f2f  n 3.11](https://
-00000920: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000930: 6164 6765 2f70 7974 686f 6e2d 332e 3131  adge/python-3.11
-00000940: 2d62 6c75 652e 7376 6729 5d28 6874 7470  -blue.svg)](http
-00000950: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-00000960: 7267 2f64 6f77 6e6c 6f61 6473 2f72 656c  rg/downloads/rel
-00000970: 6561 7365 2f70 7974 686f 6e2d 3331 3039  ease/python-3109
-00000980: 2f29 0a5b 215b 7072 652d 636f 6d6d 6974  /).[![pre-commit
-00000990: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000009a0: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-000009b0: 7265 2d2d 636f 6d6d 6974 2d65 6e61 626c  re--commit-enabl
-000009c0: 6564 2d62 7269 6768 7467 7265 656e 3f6c  ed-brightgreen?l
-000009d0: 6f67 6f3d 7072 652d 636f 6d6d 6974 266c  ogo=pre-commit&l
-000009e0: 6f67 6f43 6f6c 6f72 3d77 6869 7465 295d  ogoColor=white)]
-000009f0: 2868 7474 7073 3a2f 2f70 7265 2d63 6f6d  (https://pre-com
-00000a00: 6d69 742e 636f 6d2f 290a 3c61 2068 7265  mit.com/).<a hre
-00000a10: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000a20: 622e 636f 6d2f 7073 662f 626c 6163 6b22  b.com/psf/black"
-00000a30: 3e3c 696d 6720 616c 743d 2243 6f64 6520  ><img alt="Code 
-00000a40: 7374 796c 653a 2062 6c61 636b 2220 7372  style: black" sr
-00000a50: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000a60: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000a70: 636f 6465 2532 3073 7479 6c65 2d62 6c61  code%20style-bla
-00000a80: 636b 2d30 3030 3030 302e 7376 6722 3e3c  ck-000000.svg"><
-00000a90: 2f61 3e0a 5b21 5b43 6865 636b 6564 2077  /a>.[![Checked w
-00000aa0: 6974 6820 6d79 7079 5d28 6874 7470 733a  ith mypy](https:
-00000ab0: 2f2f 7777 772e 6d79 7079 2d6c 616e 672e  //www.mypy-lang.
-00000ac0: 6f72 672f 7374 6174 6963 2f6d 7970 795f  org/static/mypy_
-00000ad0: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-00000ae0: 733a 2f2f 6d79 7079 2d6c 616e 672e 6f72  s://mypy-lang.or
-00000af0: 672f 290a 5b21 5b62 6561 722d 6966 6965  g/).[![bear-ifie
-00000b00: 645d 2868 7474 7073 3a2f 2f72 6177 2e67  d](https://raw.g
-00000b10: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000b20: 2e63 6f6d 2f62 6561 7274 7970 652f 6265  .com/beartype/be
-00000b30: 6172 7479 7065 2d61 7373 6574 732f 6d61  artype-assets/ma
-00000b40: 696e 2f62 6164 6765 2f62 6561 722d 6966  in/badge/bear-if
-00000b50: 6965 642e 7376 6729 5d28 6874 7470 733a  ied.svg)](https:
-00000b60: 2f2f 6265 6172 7479 7065 2e72 6561 6474  //beartype.readt
-00000b70: 6865 646f 6373 2e69 6f29 0a5b 215b 4769  hedocs.io).[![Gi
-00000b80: 7468 7562 2041 6374 696f 6e5d 2868 7474  thub Action](htt
-00000b90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ba0: 5875 6875 695a 686f 752f 736f 746f 7069  XuhuiZhou/sotopi
-00000bb0: 612f 6163 7469 6f6e 732f 776f 726b 666c  a/actions/workfl
-00000bc0: 6f77 732f 7465 7374 732e 796d 6c2f 6261  ows/tests.yml/ba
-00000bd0: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-00000be0: 6169 6e29 5d28 290a 5b21 5b47 6974 6875  ain)]().[![Githu
-00000bf0: 6220 4163 7469 6f6e 5d28 6874 7470 733a  b Action](https:
-00000c00: 2f2f 6769 7468 7562 2e63 6f6d 2f58 7568  //github.com/Xuh
-00000c10: 7569 5a68 6f75 2f73 6f74 6f70 6961 2f61  uiZhou/sotopia/a
-00000c20: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000c30: 2f70 7265 2d63 6f6d 6d69 742e 796d 6c2f  /pre-commit.yml/
-00000c40: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-00000c50: 3d6d 6169 6e29 5d28 290a 5b21 5b44 6174  =main)]().[![Dat
-00000c60: 6173 6574 5d28 6874 7470 733a 2f2f 696d  aset](https://im
-00000c70: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000c80: 6765 2f25 4630 2539 4625 4134 2539 372d  ge/%F0%9F%A4%97-
-00000c90: 536f 746f 7069 6125 3230 4461 7461 7365  Sotopia%20Datase
-00000ca0: 742d 7965 6c6c 6f77 295d 2868 7474 7073  t-yellow)](https
-00000cb0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00000cc0: 6f2f 6461 7461 7365 7473 2f63 6d75 2d6c  o/datasets/cmu-l
-00000cd0: 7469 2f73 6f74 6f70 6961 290a 5b21 5b44  ti/sotopia).[![D
-00000ce0: 656d 6f5d 2868 7474 7073 3a2f 2f69 6d67  emo](https://img
-00000cf0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000d00: 652f 2546 3025 3946 2541 3425 3937 2d53  e/%F0%9F%A4%97-S
-00000d10: 6f74 6f70 6961 2532 3044 656d 6f2d 6f72  otopia%20Demo-or
-00000d20: 616e 6765 295d 2868 7474 7073 3a2f 2f68  ange)](https://h
-00000d30: 7567 6769 6e67 6661 6365 2e63 6f2f 7370  uggingface.co/sp
-00000d40: 6163 6573 2f63 6d75 2d6c 7469 2f73 6f74  aces/cmu-lti/sot
-00000d50: 6f70 6961 2d73 7061 6365 2f29 0a0a 2323  opia-space/)..##
-00000d60: 204e 6577 730a 0a2a 205b 3035 2f32 3032   News..* [05/202
-00000d70: 345d 2053 6f74 6f70 6961 2077 696c 6c20  4] Sotopia will 
-00000d80: 6265 2070 7265 7365 6e74 6564 2061 7420  be presented at 
-00000d90: 4943 4c52 2032 3032 3420 6173 2061 2073  ICLR 2024 as a s
-00000da0: 706f 746c 6967 6874 20e2 ad90 210a 2a20  potlight ...!.* 
-00000db0: 5b30 352f 3230 3234 5d20 5765 2072 656c  [05/2024] We rel
-00000dc0: 6561 7365 205b 6120 7369 6d70 6c65 2074  ease [a simple t
-00000dd0: 7574 6f72 6961 6c5d 2868 7474 7073 3a2f  utorial](https:/
-00000de0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
-00000df0: 676f 6f67 6c65 2e63 6f6d 2f64 7269 7665  google.com/drive
-00000e00: 2f31 3468 4a4f 667a 7041 3337 5052 557a  /14hJOfzpA37PRUz
-00000e10: 646c 4667 6971 567a 5547 4968 686e 6771  dlFgiqVzUGIhhngq
-00000e20: 6e7a 3f75 7370 3d73 6861 7269 6e67 2920  nz?usp=sharing) 
-00000e30: 666f 7220 796f 7520 746f 2072 756e 2073  for you to run s
-00000e40: 6f74 6f70 6961 2065 6e64 2d74 6f2d 656e  otopia end-to-en
-00000e50: 6420 6f6e 2067 6f6f 676c 6520 636f 6c61  d on google cola
-00000e60: 622e 0a0a 0a23 2320 496e 7472 6f64 7563  b....## Introduc
-00000e70: 7469 6f6e 0a0a 536f 746f 7069 6120 6973  tion..Sotopia is
-00000e80: 2061 6e20 6f70 656e 2d65 6e64 6564 2073   an open-ended s
-00000e90: 6f63 6961 6c20 6c65 6172 6e69 6e67 2065  ocial learning e
-00000ea0: 6e76 6972 6f6e 6d65 6e74 2074 6861 7420  nvironment that 
-00000eb0: 616c 6c6f 7773 2061 6765 6e74 7320 746f  allows agents to
-00000ec0: 2069 6e74 6572 6163 7420 7769 7468 2065   interact with e
-00000ed0: 6163 6820 6f74 6865 7220 616e 6420 7468  ach other and th
-00000ee0: 6520 656e 7669 726f 6e6d 656e 742e 2054  e environment. T
-00000ef0: 6865 2065 6e76 6972 6f6e 6d65 6e74 2069  he environment i
-00000f00: 7320 6465 7369 676e 6564 2074 6f20 6265  s designed to be
-00000f10: 2061 2070 6c61 7466 6f72 6d20 666f 7220   a platform for 
-00000f20: 6576 616c 7561 7469 6e67 2061 6e64 2066  evaluating and f
-00000f30: 6163 696c 6961 7469 6e67 2073 6f63 6961  aciliating socia
-00000f40: 6c20 696e 7465 6c6c 6967 656e 6365 2069  l intelligence i
-00000f50: 6e20 6c61 6e67 7561 6765 2061 6765 6e74  n language agent
-00000f60: 732e 2054 6865 2065 6e76 6972 6f6e 6d65  s. The environme
-00000f70: 6e74 2069 7320 6465 7369 676e 6564 2074  nt is designed t
-00000f80: 6f20 6265 206f 7065 6e2d 656e 6465 642c  o be open-ended,
-00000f90: 206d 6561 6e69 6e67 2074 6861 7420 7468   meaning that th
-00000fa0: 6520 656e 7669 726f 6e6d 656e 7420 6361  e environment ca
-00000fb0: 6e20 6265 2065 6173 696c 7920 6578 7465  n be easily exte
-00000fc0: 6e64 6564 2074 6f20 696e 636c 7564 6520  nded to include 
-00000fd0: 6e65 7720 656e 7669 726f 6e6d 656e 7473  new environments
-00000fe0: 2061 6e64 206e 6577 2061 6765 6e74 732e   and new agents.
-00000ff0: 2054 6865 2065 6e76 6972 6f6e 6d65 6e74   The environment
-00001000: 2069 7320 616c 736f 2064 6573 6967 6e65   is also designe
-00001010: 6420 746f 2062 6520 7363 616c 6162 6c65  d to be scalable
-00001020: 2c20 6d65 616e 696e 6720 7468 6174 2074  , meaning that t
-00001030: 6865 2065 6e76 6972 6f6e 6d65 6e74 2063  he environment c
-00001040: 616e 2062 6520 6561 7369 6c79 2073 6361  an be easily sca
-00001050: 6c65 6420 746f 2069 6e63 6c75 6465 2061  led to include a
-00001060: 206c 6172 6765 206e 756d 6265 7220 6f66   large number of
-00001070: 2061 6765 6e74 7320 616e 6420 656e 7669   agents and envi
-00001080: 726f 6e6d 656e 7473 2e0a 0a0a 0a60 6060  ronments.....```
-00001090: 6269 6274 6578 0a40 696e 7072 6f63 6565  bibtex.@inprocee
-000010a0: 6469 6e67 737b 7a68 6f75 3230 3234 736f  dings{zhou2024so
-000010b0: 746f 7069 612c 0a20 2074 6974 6c65 203d  topia,.  title =
-000010c0: 207b 534f 544f 5049 413a 2049 6e74 6572   {SOTOPIA: Inter
-000010d0: 6163 7469 7665 2045 7661 6c75 6174 696f  active Evaluatio
-000010e0: 6e20 666f 7220 536f 6369 616c 2049 6e74  n for Social Int
-000010f0: 656c 6c69 6765 6e63 6520 696e 204c 616e  elligence in Lan
-00001100: 6775 6167 6520 4167 656e 7473 7d2c 0a20  guage Agents},. 
-00001110: 2061 7574 686f 7220 3d20 7b5a 686f 752a   author = {Zhou*
-00001120: 2c20 5875 6875 6920 616e 6420 5a68 752a  , Xuhui and Zhu*
-00001130: 2c20 4861 6f20 616e 6420 4d61 7468 7572  , Hao and Mathur
-00001140: 2c20 4c65 656e 6120 616e 6420 5a68 616e  , Leena and Zhan
-00001150: 672c 2052 756f 686f 6e67 2061 6e64 2051  g, Ruohong and Q
-00001160: 692c 205a 6865 6e67 7961 6e67 2061 6e64  i, Zhengyang and
-00001170: 2059 752c 2048 616f 6665 6920 616e 6420   Yu, Haofei and 
-00001180: 4d6f 7265 6e63 792c 204c 6f75 6973 2d50  Morency, Louis-P
-00001190: 6869 6c69 7070 6520 616e 6420 4269 736b  hilippe and Bisk
-000011a0: 2c20 596f 6e61 7461 6e20 616e 6420 4672  , Yonatan and Fr
-000011b0: 6965 642c 2044 616e 6965 6c20 616e 6420  ied, Daniel and 
-000011c0: 4e65 7562 6967 2c20 4772 6168 616d 2061  Neubig, Graham a
-000011d0: 6e64 2053 6170 2c20 4d61 6172 7465 6e7d  nd Sap, Maarten}
-000011e0: 2c0a 2020 6a6f 7572 6e61 6c20 3d20 7b49  ,.  journal = {I
-000011f0: 434c 527d 2c0a 2020 7965 6172 203d 207b  CLR},.  year = {
-00001200: 3230 3234 7d2c 0a20 2075 726c 203d 207b  2024},.  url = {
-00001210: 6874 7470 733a 2f2f 6f70 656e 7265 7669  https://openrevi
-00001220: 6577 2e6e 6574 2f66 6f72 756d 3f69 643d  ew.net/forum?id=
-00001230: 6d4d 3756 7572 6241 3472 7d2c 0a7d 0a60  mM7VurbA4r},.}.`
-00001240: 6060 0a0a 0a23 2320 4765 7420 7374 6172  ``...## Get star
-00001250: 7465 640a 2323 2320 5573 6520 6f6e 2047  ted.### Use on G
-00001260: 6f6f 676c 6520 436f 6c61 620a 0a49 6620  oogle Colab..If 
-00001270: 796f 7520 7761 6e74 2074 6f20 7472 7920  you want to try 
-00001280: 6974 206f 7574 206f 6e20 476f 6f67 6c65  it out on Google
-00001290: 2043 6f6c 6162 2066 6972 7374 2c20 706c   Colab first, pl
-000012a0: 6561 7365 2063 6865 636b 206f 7574 206f  ease check out o
-000012b0: 7572 2043 6f6c 6162 2054 7574 6f72 6961  ur Colab Tutoria
-000012c0: 6c20 5365 7269 6573 3a0a 0a3c 6f6c 3e0a  l Series:..<ol>.
-000012d0: 3c6c 693e 2042 6173 6963 0a20 203c 6f6c  <li> Basic.  <ol
-000012e0: 3e0a 2020 2020 3c6c 693e 203c 6120 6872  >.    <li> <a hr
-000012f0: 6566 3d22 6874 7470 733a 2f2f 636f 6c61  ef="https://cola
-00001300: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00001310: 652e 636f 6d2f 6472 6976 652f 3134 684a  e.com/drive/14hJ
-00001320: 4f66 7a70 4133 3750 5255 7a64 6c46 6769  OfzpA37PRUzdlFgi
-00001330: 7156 7a55 4749 6868 6e67 716e 7a3f 7573  qVzUGIhhngqnz?us
-00001340: 703d 7368 6172 696e 6722 3e31 2e31 2050  p=sharing">1.1 P
-00001350: 6c61 7969 6e67 2077 6974 6820 536f 746f  laying with Soto
-00001360: 7069 6120 696e 2061 2047 6f6f 676c 6520  pia in a Google 
-00001370: 436f 6c61 6220 4e6f 7465 626f 6f6b 3c2f  Colab Notebook</
-00001380: 613e 203c 2f6c 693e 0a20 2020 203c 6c69  a> </li>.    <li
-00001390: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
-000013a0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-000013b0: 682e 676f 6f67 6c65 2e63 6f6d 2f64 7269  h.google.com/dri
-000013c0: 7665 2f31 4769 3255 3363 4130 4b47 316e  ve/1Gi2U3cA0KG1n
-000013d0: 656b 7731 4130 4e30 445a 7078 3667 4b72  ekw1A0N0DZpx6gKr
-000013e0: 6a38 4e63 3f75 7370 3d73 6861 7269 6e67  j8Nc?usp=sharing
-000013f0: 223e 312e 3220 4272 6f77 7369 6e67 2073  ">1.2 Browsing s
-00001400: 6f74 6f70 6961 2064 6174 613c 2f61 3e20  otopia data</a> 
-00001410: 3c2f 6c69 3e0a 2020 3c2f 6f6c 3e0a 3c2f  </li>.  </ol>.</
-00001420: 6c69 3e0a 3c6c 693e 0a42 7569 6c64 696e  li>.<li>.Buildin
-00001430: 6720 796f 7572 206f 776e 2073 6f63 6961  g your own socia
-00001440: 6c20 6167 656e 7420 2863 6f6d 696e 6720  l agent (coming 
-00001450: 736f 6f6e 2129 0a3c 2f6c 693e 0a3c 2f6f  soon!).</li>.</o
-00001460: 6c3e 0a0a 2323 2320 496e 7374 616c 6c20  l>..### Install 
-00001470: 6c6f 6361 6c6c 790a 5468 6973 2070 6163  locally.This pac
-00001480: 6b61 6765 2073 7570 706f 7274 7320 5079  kage supports Py
-00001490: 7468 6f6e 2033 2e31 3120 616e 6420 6162  thon 3.11 and ab
-000014a0: 6f76 652e 2049 6e20 6f6e 6520 6c69 6e65  ove. In one line
-000014b0: 2c0a 6070 6970 2069 6e73 7461 6c6c 2073  ,.`pip install s
-000014c0: 6f74 6f70 6961 6020 6f72 2060 7069 7020  otopia` or `pip 
-000014d0: 696e 7374 616c 6c20 7576 3b20 7576 2070  install uv; uv p
-000014e0: 6970 2069 6e73 7461 6c6c 2073 6f74 6f70  ip install sotop
-000014f0: 6961 602e 0a0a 4f72 2066 726f 6d20 7363  ia`...Or from sc
-00001500: 7261 7463 682c 2075 7365 2061 2076 6972  ratch, use a vir
-00001510: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00001520: 2c20 652e 672e 2077 6974 6820 616e 6163  , e.g. with anac
-00001530: 6f6e 6461 333a 2060 636f 6e64 6120 6372  onda3: `conda cr
-00001540: 6561 7465 202d 6e20 736f 746f 7069 6120  eate -n sotopia 
-00001550: 7079 7468 6f6e 3d33 2e31 313b 2063 6f6e  python=3.11; con
-00001560: 6461 2061 6374 6976 6174 6520 736f 746f  da activate soto
-00001570: 7069 613b 2063 7572 6c20 2d73 534c 2068  pia; curl -sSL h
-00001580: 7474 7073 3a2f 2f69 6e73 7461 6c6c 2e70  ttps://install.p
-00001590: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
-000015a0: 207c 2070 7974 686f 6e33 602e 2054 6865   | python3`. The
-000015b0: 6e2c 2069 6e73 7461 6c6c 2074 6865 2072  n, install the r
-000015c0: 6571 7569 7265 6d65 6e74 7320 616e 6420  equirements and 
-000015d0: 7468 6973 2070 6163 6b61 6765 2e0a 6060  this package..``
-000015e0: 6062 6173 680a 706f 6574 7279 2069 6e73  `bash.poetry ins
-000015f0: 7461 6c6c 0a60 6060 0a0a 4f70 656e 4149  tall.```..OpenAI
-00001600: 206b 6579 2069 7320 7265 7175 6972 6564   key is required
-00001610: 2074 6f20 7275 6e20 7468 6520 636f 6465   to run the code
-00001620: 2e20 506c 6561 7365 2073 6574 2074 6865  . Please set the
-00001630: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-00001640: 6961 626c 6520 604f 5045 4e41 495f 4150  iable `OPENAI_AP
-00001650: 495f 4b45 5960 2074 6f20 796f 7572 206b  I_KEY` to your k
-00001660: 6579 2e20 5468 6520 7265 636f 6d6d 656e  ey. The recommen
-00001670: 6420 7761 7920 6973 2074 6f20 6164 6420  d way is to add 
-00001680: 7468 6520 6b65 7920 746f 2074 6865 2063  the key to the c
-00001690: 6f6e 6461 2065 6e76 6972 6f6e 6d65 6e74  onda environment
-000016a0: 3a0a 6060 6062 6173 680a 636f 6e64 6120  :.```bash.conda 
-000016b0: 656e 7620 636f 6e66 6967 2076 6172 7320  env config vars 
-000016c0: 7365 7420 4f50 454e 4149 5f41 5049 5f4b  set OPENAI_API_K
-000016d0: 4559 3d79 6f75 725f 6b65 790a 6060 600a  EY=your_key.```.
-000016e0: 0a46 6f72 2073 6f6d 6520 6578 7065 7269  .For some experi
-000016f0: 6d65 6e74 732c 2054 6f67 6574 6865 7241  ments, TogetherA
-00001700: 4920 6b65 7920 6973 2072 6571 7569 7265  I key is require
-00001710: 6420 746f 2072 756e 2074 6865 2063 6f64  d to run the cod
-00001720: 652e 2050 6c65 6173 6520 7365 7420 7468  e. Please set th
-00001730: 6520 656e 7669 726f 6e6d 656e 7420 7661  e environment va
-00001740: 7269 6162 6c65 2060 544f 4745 5448 4552  riable `TOGETHER
-00001750: 5f41 5049 5f4b 4559 6020 746f 2079 6f75  _API_KEY` to you
-00001760: 7220 6b65 792e 2054 6865 2072 6563 6f6d  r key. The recom
-00001770: 6d65 6e64 2077 6179 2069 7320 746f 2061  mend way is to a
-00001780: 6464 2074 6865 206b 6579 2074 6f20 7468  dd the key to th
-00001790: 6520 636f 6e64 6120 656e 7669 726f 6e6d  e conda environm
-000017a0: 656e 743a 0a60 6060 6261 7368 0a63 6f6e  ent:.```bash.con
-000017b0: 6461 2065 6e76 2063 6f6e 6669 6720 7661  da env config va
-000017c0: 7273 2073 6574 2054 4f47 4554 4845 525f  rs set TOGETHER_
-000017d0: 4150 495f 4b45 593d 796f 7572 5f6b 6579  API_KEY=your_key
-000017e0: 0a60 6060 0a0a 4120 7265 6469 732d 7374  .```..A redis-st
-000017f0: 6163 6b20 7365 7276 6572 2069 7320 7265  ack server is re
-00001800: 7175 6972 6564 2074 6f20 7275 6e20 7468  quired to run th
-00001810: 6520 636f 6465 2e20 506c 6561 7365 2066  e code. Please f
-00001820: 6f6c 6c6f 7720 7468 6520 5b69 6e73 7472  ollow the [instr
-00001830: 7563 7469 6f6e 5d28 6874 7470 733a 2f2f  uction](https://
-00001840: 7265 6469 732e 696f 2f64 6f63 732f 7374  redis.io/docs/st
-00001850: 6163 6b2f 6765 742d 7374 6172 7465 642f  ack/get-started/
-00001860: 696e 7374 616c 6c2f 646f 636b 6572 2f29  install/docker/)
-00001870: 2074 6f20 7374 6172 7420 6120 7265 6469   to start a redi
-00001880: 732d 7374 6163 6b20 7365 7276 6572 206f  s-stack server o
-00001890: 7220 7573 6520 616e 2065 7869 7374 696e  r use an existin
-000018a0: 6720 7365 7276 6572 2e20 596f 7520 6361  g server. You ca
-000018b0: 6e20 616c 736f 2063 6865 636b 205b 5126  n also check [Q&
-000018c0: 415d 282f 646f 6373 2f61 6c6c 5f74 6865  A](/docs/all_the
-000018d0: 5f69 7373 7565 732e 6d64 2920 746f 2069  _issues.md) to i
-000018e0: 6e69 7469 6174 6520 7468 6520 7265 6469  nitiate the redi
-000018f0: 7320 7365 7276 6572 2077 6974 6820 7468  s server with th
-00001900: 6520 536f 746f 7069 6120 6461 7461 2e0a  e Sotopia data..
-00001910: 0a54 6865 2060 5245 4449 535f 4f4d 5f55  .The `REDIS_OM_U
-00001920: 524c 6020 6e65 6564 2074 6f20 6265 2073  RL` need to be s
-00001930: 6574 2062 6566 6f72 6520 6c6f 6164 696e  et before loadin
-00001940: 6720 616e 6420 7361 7669 6e67 2061 6765  g and saving age
-00001950: 6e74 733a 0a60 6060 6261 7368 0a63 6f6e  nts:.```bash.con
-00001960: 6461 2065 6e76 2063 6f6e 6669 6720 7661  da env config va
-00001970: 7273 2073 6574 2052 4544 4953 5f4f 4d5f  rs set REDIS_OM_
-00001980: 5552 4c3d 2272 6564 6973 3a2f 2f75 7365  URL="redis://use
-00001990: 723a 7061 7373 776f 7264 4068 6f73 743a  r:password@host:
-000019a0: 706f 7274 220a 6060 600a 0a4d 616b 6520  port".```..Make 
-000019b0: 6120 666f 6c64 6572 2074 6f20 7374 6f72  a folder to stor
-000019c0: 6520 7468 6520 6c6f 6773 3a0a 6060 6062  e the logs:.```b
-000019d0: 6173 680a 6d6b 6469 7220 6c6f 6773 0a60  ash.mkdir logs.`
-000019e0: 6060 0a0a 0a0a 2323 2045 6173 7920 5361  ``....## Easy Sa
-000019f0: 6d70 6c65 2053 6572 7665 720a 596f 7520  mple Server.You 
-00001a00: 6361 6e20 7669 6577 2061 6e20 6570 6973  can view an epis
-00001a10: 6f64 6520 6465 6d6f 2077 6974 6820 6465  ode demo with de
-00001a20: 6661 756c 7420 7061 7261 6d65 7465 7273  fault parameters
-00001a30: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
-00001a40: 696e 673a 0a60 6060 7079 7468 6f6e 0a69  ing:.```python.i
-00001a50: 6d70 6f72 7420 6173 796e 6369 6f0a 6672  mport asyncio.fr
-00001a60: 6f6d 2073 6f74 6f70 6961 2e73 616d 706c  om sotopia.sampl
-00001a70: 6572 7320 696d 706f 7274 2055 6e69 666f  ers import Unifo
-00001a80: 726d 5361 6d70 6c65 720a 6672 6f6d 2073  rmSampler.from s
-00001a90: 6f74 6f70 6961 2e73 6572 7665 7220 696d  otopia.server im
-00001aa0: 706f 7274 2072 756e 5f61 7379 6e63 5f73  port run_async_s
-00001ab0: 6572 7665 720a 0a61 7379 6e63 696f 2e72  erver..asyncio.r
-00001ac0: 756e 280a 2020 2020 7275 6e5f 6173 796e  un(.    run_asyn
-00001ad0: 635f 7365 7276 6572 280a 2020 2020 2020  c_server(.      
-00001ae0: 2020 6d6f 6465 6c5f 6469 6374 3d7b 0a20    model_dict={. 
-00001af0: 2020 2020 2020 2020 2020 2022 656e 7622             "env"
-00001b00: 3a20 2267 7074 2d34 222c 0a20 2020 2020  : "gpt-4",.     
-00001b10: 2020 2020 2020 2022 6167 656e 7431 223a         "agent1":
-00001b20: 2022 6770 742d 332e 352d 7475 7262 6f22   "gpt-3.5-turbo"
-00001b30: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
-00001b40: 6765 6e74 3222 3a20 2267 7074 2d33 2e35  gent2": "gpt-3.5
-00001b50: 2d74 7572 626f 222c 0a20 2020 2020 2020  -turbo",.       
-00001b60: 207d 2c0a 2020 2020 2020 2020 7361 6d70   },.        samp
-00001b70: 6c65 723d 556e 6966 6f72 6d53 616d 706c  ler=UniformSampl
-00001b80: 6572 2829 2c0a 2020 2020 290a 290a 6060  er(),.    ).).``
-00001b90: 600a 6f72 2072 756e 0a60 6060 6261 7368  `.or run.```bash
-00001ba0: 0a70 7974 686f 6e20 6578 616d 706c 6573  .python examples
-00001bb0: 2f6d 696e 696d 616c 6973 745f 6465 6d6f  /minimalist_demo
-00001bc0: 2e70 790a 6060 600a 0a23 2320 436f 6e74  .py.```..## Cont
-00001bd0: 7269 6275 7469 6f6e 0a23 2323 2320 496e  ribution.#### In
-00001be0: 7374 616c 6c20 6465 7620 6f70 7469 6f6e  stall dev option
-00001bf0: 730a 466f 6c6c 6f77 2074 6865 2069 6e73  s.Follow the ins
-00001c00: 7461 6c6c 6174 696f 6e20 696e 7374 7275  tallation instru
-00001c10: 6374 696f 6e20 6162 6f76 6520 616e 6420  ction above and 
-00001c20: 7468 656e 2c20 696e 7374 6561 6420 6f66  then, instead of
-00001c30: 2072 756e 6e69 6e67 2060 7079 7468 6f6e   running `python
-00001c40: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00001c50: 2d65 202e 602c 2072 756e 2074 6865 2066  -e .`, run the f
-00001c60: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00001c70: 733a 0a0a 6060 6062 6173 680a 7079 7468  s:..```bash.pyth
-00001c80: 6f6e 202d 6d20 7069 7020 696e 7374 616c  on -m pip instal
-00001c90: 6c20 2d65 2022 2e5b 6465 765d 220a 6d79  l -e ".[dev]".my
-00001ca0: 7079 202d 2d69 6e73 7461 6c6c 2d74 7970  py --install-typ
-00001cb0: 6573 202d 2d6e 6f6e 2d69 6e74 6572 6163  es --non-interac
-00001cc0: 7469 7665 2073 6f74 6f70 6961 0a70 7974  tive sotopia.pyt
-00001cd0: 686f 6e20 2d6d 2070 6970 2069 6e73 7461  hon -m pip insta
-00001ce0: 6c6c 2070 7265 2d63 6f6d 6d69 740a 7072  ll pre-commit.pr
-00001cf0: 652d 636f 6d6d 6974 2069 6e73 7461 6c6c  e-commit install
-00001d00: 0a60 6060 0a23 2323 2320 4e65 7720 6272  .```.#### New br
-00001d10: 616e 6368 2066 6f72 2065 6163 6820 6665  anch for each fe
-00001d20: 6174 7572 650a 6067 6974 2063 6865 636b  ature.`git check
-00001d30: 6f75 7420 2d62 2066 6561 7475 7265 2f66  out -b feature/f
-00001d40: 6561 7475 7265 2d6e 616d 6560 2061 6e64  eature-name` and
-00001d50: 2050 5220 746f 2060 6d61 696e 6020 6272   PR to `main` br
-00001d60: 616e 6368 2e0a 2323 2323 2042 6566 6f72  anch..#### Befor
-00001d70: 6520 636f 6d6d 6974 7469 6e67 0a52 756e  e committing.Run
-00001d80: 2060 7079 7465 7374 6020 746f 206d 616b   `pytest` to mak
-00001d90: 6520 7375 7265 2061 6c6c 2074 6573 7473  e sure all tests
-00001da0: 2070 6173 7320 2874 6869 7320 7769 6c6c   pass (this will
-00001db0: 2065 6e73 7572 6520 6479 6e61 6d69 6320   ensure dynamic 
-00001dc0: 7479 7069 6e67 2070 6173 7365 6420 7769  typing passed wi
-00001dd0: 7468 2062 6561 7274 7970 6529 2061 6e64  th beartype) and
-00001de0: 2060 6d79 7079 202d 2d73 7472 6963 7420   `mypy --strict 
-00001df0: 2e60 2074 6f20 6368 6563 6b20 7374 6174  .` to check stat
-00001e00: 6963 2074 7970 696e 672e 0a28 596f 7520  ic typing..(You 
-00001e10: 6361 6e20 616c 736f 2072 756e 2060 7072  can also run `pr
-00001e20: 652d 636f 6d6d 6974 2072 756e 202d 2d61  e-commit run --a
-00001e30: 6c6c 2d66 696c 6573 6020 746f 2072 756e  ll-files` to run
-00001e40: 2061 6c6c 2063 6865 636b 7329 0a23 2323   all checks).###
-00001e50: 2320 4368 6563 6b20 6769 7468 7562 2061  # Check github a
-00001e60: 6374 696f 6e20 7265 7375 6c74 0a43 6865  ction result.Che
-00001e70: 636b 2074 6865 2067 6974 6875 6220 6163  ck the github ac
-00001e80: 7469 6f6e 2072 6573 756c 7420 746f 206d  tion result to m
-00001e90: 616b 6520 7375 7265 2061 6c6c 2074 6573  ake sure all tes
-00001ea0: 7473 2070 6173 732e 2049 6620 6e6f 742c  ts pass. If not,
-00001eb0: 2066 6978 2074 6865 2065 7272 6f72 7320   fix the errors 
-00001ec0: 616e 6420 7075 7368 2061 6761 696e 2e0a  and push again..
-00001ed0: 0a23 2320 5275 6e6e 696e 6720 4578 7065  .## Running Expe
-00001ee0: 7269 6d65 6e74 730a 5765 2075 7365 2060  riments.We use `
-00001ef0: 6769 6e2d 636f 6e66 6967 6020 746f 2063  gin-config` to c
-00001f00: 6f6e 6669 6775 7265 2074 6865 2065 7870  onfigure the exp
-00001f10: 6572 696d 656e 7473 2e20 596f 7520 646f  eriments. You do
-00001f20: 6e27 7420 6e65 6564 2074 6f20 6265 2061  n't need to be a
-00001f30: 6e20 6578 7065 7274 2074 6f20 7573 6520  n expert to use 
-00001f40: 6974 2e20 5468 6520 6261 7369 6320 7379  it. The basic sy
-00001f50: 6e74 6178 2069 730a 6060 6062 6173 680a  ntax is.```bash.
-00001f60: 7079 7468 6f6e 203c 636f 6465 5f66 696c  python <code_fil
-00001f70: 652e 7079 3e20 2d2d 6769 6e5f 6669 6c65  e.py> --gin_file
-00001f80: 203c 6769 6e5f 6669 6c65 313e 202d 2d67   <gin_file1> --g
-00001f90: 696e 5f66 696c 6520 3c67 696e 5f66 696c  in_file <gin_fil
-00001fa0: 6532 3e20 272d 2d67 696e 2e50 4152 414d  e2> '--gin.PARAM
-00001fb0: 313d 7661 6c75 6531 2720 272d 2d67 696e  1=value1' '--gin
-00001fc0: 2e50 4152 414d 323d 7661 6c75 6532 270a  .PARAM2=value2'.
-00001fd0: 6060 600a 5468 6520 602d 2d67 696e 5f66  ```.The `--gin_f
-00001fe0: 696c 6560 2069 7320 7573 6564 2074 6f20  ile` is used to 
-00001ff0: 6c6f 6164 2061 6e64 2063 6f6d 706f 7365  load and compose
-00002000: 2074 6865 2064 6566 6175 6c74 2063 6f6e   the default con
-00002010: 6669 6775 7261 7469 6f6e 2e20 5468 6520  figuration. The 
-00002020: 602d 2d67 696e 2e50 4152 414d 313d 7661  `--gin.PARAM1=va
-00002030: 6c75 6531 6020 6973 2075 7365 6420 746f  lue1` is used to
-00002040: 206f 7665 7277 7269 7465 2074 6865 2064   overwrite the d
-00002050: 6566 6175 6c74 2063 6f6e 6669 6775 7261  efault configura
-00002060: 7469 6f6e 2e20 5468 6520 6c61 7465 7220  tion. The later 
-00002070: 636f 6e66 6967 7572 6174 696f 6e20 7769  configuration wi
-00002080: 6c6c 2061 6c77 6179 7320 6f76 6572 7772  ll always overwr
-00002090: 6974 6520 7468 6520 7072 6576 696f 7573  ite the previous
-000020a0: 206f 6e65 2e0a 0a48 6572 6520 6973 2061   one...Here is a
-000020b0: 6e20 6578 616d 706c 6520 6f66 2072 756e  n example of run
-000020c0: 6e69 6e67 2061 6e20 6578 7065 7269 6d65  ning an experime
-000020d0: 6e74 3a0a 0a60 6060 6261 7368 0a70 7974  nt:..```bash.pyt
-000020e0: 686f 6e20 6578 616d 706c 6573 2f65 7870  hon examples/exp
-000020f0: 6572 696d 656e 745f 6576 616c 2e70 7920  eriment_eval.py 
-00002100: 2d2d 6769 6e5f 6669 6c65 2073 6f74 6f70  --gin_file sotop
-00002110: 6961 5f63 6f6e 662f 6765 6e65 7261 7469  ia_conf/generati
-00002120: 6f6e 5f75 7469 6c73 5f63 6f6e 662f 6765  on_utils_conf/ge
-00002130: 6e65 7261 7465 2e67 696e 202d 2d67 696e  nerate.gin --gin
-00002140: 5f66 696c 6520 736f 746f 7069 615f 636f  _file sotopia_co
-00002150: 6e66 2f73 6572 7665 725f 636f 6e66 2f73  nf/server_conf/s
-00002160: 6572 7665 722e 6769 6e20 2d2d 6769 6e5f  erver.gin --gin_
-00002170: 6669 6c65 2073 6f74 6f70 6961 5f63 6f6e  file sotopia_con
-00002180: 662f 7275 6e5f 6173 796e 635f 7365 7276  f/run_async_serv
-00002190: 6572 5f69 6e5f 6261 7463 682e 6769 6e20  er_in_batch.gin 
-000021a0: 272d 2d67 696e 2e45 4e56 5f49 4453 3d5b  '--gin.ENV_IDS=[
-000021b0: 2230 3148 3756 4648 5044 5a56 5643 445a  "01H7VFHPDZVVCDZ
-000021c0: 5233 4141 5241 3534 3743 5922 5d27 2027  R3AARA547CY"]' '
-000021d0: 2d2d 6769 6e2e 4147 454e 5431 5f4d 4f44  --gin.AGENT1_MOD
-000021e0: 454c 3d22 6770 742d 3422 2720 272d 2d67  EL="gpt-4"' '--g
-000021f0: 696e 2e42 4154 4348 5f53 495a 453d 3230  in.BATCH_SIZE=20
-00002200: 2720 272d 2d67 696e 2e50 5553 485f 544f  ' '--gin.PUSH_TO
-00002210: 5f44 423d 4661 6c73 6527 2027 2d2d 6769  _DB=False' '--gi
-00002220: 6e2e 5441 473d 2274 6573 7422 270a 6060  n.TAG="test"'.``
-00002230: 600a 466f 7220 7468 6520 636f 6d70 6c65  `.For the comple
-00002240: 7465 2073 6574 206f 6620 7061 7261 6d65  te set of parame
-00002250: 7465 7273 2c20 706c 6561 7365 2063 6865  ters, please che
-00002260: 636b 2074 6865 2060 736f 746f 7069 615f  ck the `sotopia_
-00002270: 636f 6e66 6020 666f 6c64 6572 2e0a 0a54  conf` folder...T
-00002280: 6f20 7275 6e20 6120 6c61 7267 6520 6261  o run a large ba
-00002290: 7463 6820 6f66 2065 6e76 6972 6f6e 6d65  tch of environme
-000022a0: 6e74 732c 2079 6f75 2063 616e 2063 6861  nts, you can cha
-000022b0: 6e67 6520 7468 6520 6045 4e56 5f49 4453  nge the `ENV_IDS
-000022c0: 6020 7061 7261 6d65 7465 7220 696e 2060  ` parameter in `
-000022d0: 736f 746f 7069 615f 636f 6e66 2f72 756e  sotopia_conf/run
-000022e0: 5f61 7379 6e63 5f73 6572 7665 725f 696e  _async_server_in
-000022f0: 5f62 6174 6368 2e67 696e 6020 746f 2061  _batch.gin` to a
-00002300: 206c 6973 7420 6f66 2065 6e76 6972 6f6e   list of environ
-00002310: 6d65 6e74 2069 6473 2e20 5768 656e 2060  ment ids. When `
-00002320: 6769 6e2e 454e 565f 4944 533d 3d5b 5d60  gin.ENV_IDS==[]`
-00002330: 2c20 616c 6c20 656e 7669 726f 6e6d 656e  , all environmen
-00002340: 7473 206f 6e20 7468 6520 4442 2077 696c  ts on the DB wil
-00002350: 6c20 6265 2075 7365 642e 0a0a 2323 2047  l be used...## G
-00002360: 6574 7469 6e67 2061 6363 6573 7320 746f  etting access to
-00002370: 2079 6f75 7220 7369 6d75 6c61 7469 6f6e   your simulation
-00002380: 0a41 6674 6572 2072 756e 6e69 6e67 2065  .After running e
-00002390: 7870 6572 696d 656e 7473 2c20 796f 7520  xperiments, you 
-000023a0: 6361 6e20 676f 2074 6f20 7468 6520 6065  can go to the `e
-000023b0: 7861 6d70 6c65 732f 7265 6469 735f 7374  xamples/redis_st
-000023c0: 6174 732e 6970 796e 6260 206e 6f74 6562  ats.ipynb` noteb
-000023d0: 6f6f 6b20 746f 2063 6865 636b 2074 6865  ook to check the
-000023e0: 2065 7869 7374 696e 6720 6570 6973 6f64   existing episod
-000023f0: 6573 2028 4570 6973 6f64 6520 4c6f 6720  es (Episode Log 
-00002400: 7365 6374 696f 6e29 2c20 6173 2077 656c  section), as wel
-00002410: 6c20 6173 2063 616c 6375 6c61 7465 2074  l as calculate t
-00002420: 6865 2070 6572 666f 726d 616e 6365 2e0a  he performance..
-00002430: 0a46 6f72 2074 6865 206f 7269 6769 6e61  .For the origina
-00002440: 6c20 536f 746f 7069 6120 7369 6d75 6c61  l Sotopia simula
-00002450: 7469 6f6e 2069 6e20 6f75 7220 7061 7065  tion in our pape
-00002460: 7227 7320 6578 7065 7269 6d65 6e74 732c  r's experiments,
-00002470: 2079 6f75 2063 616e 2066 696e 6420 686f   you can find ho
-00002480: 7720 746f 2067 6574 2074 6865 6d20 696e  w to get them in
-00002490: 2074 6865 205b 5126 415d 282f 646f 6373   the [Q&A](/docs
-000024a0: 2f61 6c6c 5f74 6865 5f69 7373 7565 732e  /all_the_issues.
-000024b0: 6d64 2920 7365 6374 696f 6e20 696e 2074  md) section in t
-000024c0: 6865 2060 2e2f 646f 6373 6020 666f 6c64  he `./docs` fold
-000024d0: 6572 2e0a 0a23 2320 4164 6469 6e67 206e  er...## Adding n
-000024e0: 6577 2063 6861 7261 6374 6572 7320 616e  ew characters an
-000024f0: 6420 656e 7669 726f 6e6d 656e 7473 0a59  d environments.Y
-00002500: 6f75 2063 616e 2075 7365 2074 6865 2066  ou can use the f
-00002510: 6f6c 6c6f 7769 6e67 2066 756e 6374 696f  ollowing functio
-00002520: 6e20 7769 7468 2074 6865 2060 2a2a 6b77  n with the `**kw
-00002530: 6172 6773 6020 6265 696e 6720 7468 6520  args` being the 
-00002540: 7072 6f70 6572 7469 6573 206f 6620 7468  properties of th
-00002550: 6520 6041 6765 6e74 5072 6f66 696c 6560  e `AgentProfile`
-00002560: 2063 6c61 7373 2e20 5468 6973 2069 7320   class. This is 
-00002570: 7468 6520 7361 6d65 2066 6f72 2074 6865  the same for the
-00002580: 2073 6365 6e61 7269 6f73 2f65 6e76 6972   scenarios/envir
-00002590: 6f6e 6d65 6e74 732e 0a60 6060 7079 7468  onments..```pyth
-000025a0: 6f6e 0a63 6c61 7373 2041 6765 6e74 5072  on.class AgentPr
-000025b0: 6f66 696c 6528 4a73 6f6e 4d6f 6465 6c29  ofile(JsonModel)
-000025c0: 3a0a 2020 2020 6669 7273 745f 6e61 6d65  :.    first_name
-000025d0: 3a20 7374 7220 3d20 4669 656c 6428 696e  : str = Field(in
-000025e0: 6465 783d 5472 7565 290a 2020 2020 6c61  dex=True).    la
-000025f0: 7374 5f6e 616d 653a 2073 7472 203d 2046  st_name: str = F
-00002600: 6965 6c64 2869 6e64 6578 3d54 7275 6529  ield(index=True)
-00002610: 0a20 2020 2061 6765 3a20 696e 7420 3d20  .    age: int = 
-00002620: 4669 656c 6428 696e 6465 783d 5472 7565  Field(index=True
-00002630: 2c20 6465 6661 756c 745f 6661 6374 6f72  , default_factor
-00002640: 793d 6c61 6d62 6461 3a20 3029 0a20 2020  y=lambda: 0).   
-00002650: 206f 6363 7570 6174 696f 6e3a 2073 7472   occupation: str
-00002660: 203d 2046 6965 6c64 2869 6e64 6578 3d54   = Field(index=T
-00002670: 7275 652c 2064 6566 6175 6c74 5f66 6163  rue, default_fac
-00002680: 746f 7279 3d6c 616d 6264 613a 2022 2229  tory=lambda: "")
-00002690: 0a20 2020 2067 656e 6465 723a 2073 7472  .    gender: str
-000026a0: 203d 2046 6965 6c64 2869 6e64 6578 3d54   = Field(index=T
-000026b0: 7275 652c 2064 6566 6175 6c74 5f66 6163  rue, default_fac
-000026c0: 746f 7279 3d6c 616d 6264 613a 2022 2229  tory=lambda: "")
-000026d0: 0a20 2020 2067 656e 6465 725f 7072 6f6e  .    gender_pron
-000026e0: 6f75 6e3a 2073 7472 203d 2046 6965 6c64  oun: str = Field
-000026f0: 2869 6e64 6578 3d54 7275 652c 2064 6566  (index=True, def
-00002700: 6175 6c74 5f66 6163 746f 7279 3d6c 616d  ault_factory=lam
-00002710: 6264 613a 2022 2229 0a20 2020 2070 7562  bda: "").    pub
-00002720: 6c69 635f 696e 666f 3a20 7374 7220 3d20  lic_info: str = 
-00002730: 4669 656c 6428 696e 6465 783d 5472 7565  Field(index=True
-00002740: 2c20 6465 6661 756c 745f 6661 6374 6f72  , default_factor
-00002750: 793d 6c61 6d62 6461 3a20 2222 290a 2020  y=lambda: "").  
-00002760: 2020 6269 675f 6669 7665 3a20 7374 7220    big_five: str 
-00002770: 3d20 4669 656c 6428 696e 6465 783d 5472  = Field(index=Tr
-00002780: 7565 2c20 6465 6661 756c 745f 6661 6374  ue, default_fact
-00002790: 6f72 793d 6c61 6d62 6461 3a20 2222 290a  ory=lambda: "").
-000027a0: 2020 2020 6d6f 7261 6c5f 7661 6c75 6573      moral_values
-000027b0: 3a20 6c69 7374 5b73 7472 5d20 3d20 4669  : list[str] = Fi
-000027c0: 656c 6428 696e 6465 783d 4661 6c73 652c  eld(index=False,
-000027d0: 2064 6566 6175 6c74 5f66 6163 746f 7279   default_factory
-000027e0: 3d6c 616d 6264 613a 205b 5d29 0a20 2020  =lambda: []).   
-000027f0: 2073 6368 7761 7274 7a5f 7065 7273 6f6e   schwartz_person
-00002800: 616c 5f76 616c 7565 733a 206c 6973 745b  al_values: list[
-00002810: 7374 725d 203d 2046 6965 6c64 2869 6e64  str] = Field(ind
-00002820: 6578 3d46 616c 7365 2c20 6465 6661 756c  ex=False, defaul
-00002830: 745f 6661 6374 6f72 793d 6c61 6d62 6461  t_factory=lambda
-00002840: 3a20 5b5d 290a 2020 2020 7065 7273 6f6e  : []).    person
-00002850: 616c 6974 795f 616e 645f 7661 6c75 6573  ality_and_values
-00002860: 3a20 7374 7220 3d20 4669 656c 6428 696e  : str = Field(in
-00002870: 6465 783d 5472 7565 2c20 6465 6661 756c  dex=True, defaul
-00002880: 745f 6661 6374 6f72 793d 6c61 6d62 6461  t_factory=lambda
-00002890: 3a20 2222 290a 2020 2020 6465 6369 7369  : "").    decisi
-000028a0: 6f6e 5f6d 616b 696e 675f 7374 796c 653a  on_making_style:
-000028b0: 2073 7472 203d 2046 6965 6c64 2869 6e64   str = Field(ind
-000028c0: 6578 3d54 7275 652c 2064 6566 6175 6c74  ex=True, default
-000028d0: 5f66 6163 746f 7279 3d6c 616d 6264 613a  _factory=lambda:
-000028e0: 2022 2229 0a20 2020 2073 6563 7265 743a   "").    secret:
-000028f0: 2073 7472 203d 2046 6965 6c64 2864 6566   str = Field(def
-00002900: 6175 6c74 5f66 6163 746f 7279 3d6c 616d  ault_factory=lam
-00002910: 6264 613a 2022 2229 0a20 2020 206d 6f64  bda: "").    mod
-00002920: 656c 5f69 643a 2073 7472 203d 2046 6965  el_id: str = Fie
-00002930: 6c64 2864 6566 6175 6c74 5f66 6163 746f  ld(default_facto
-00002940: 7279 3d6c 616d 6264 613a 2022 2229 0a0a  ry=lambda: "")..
-00002950: 636c 6173 7320 456e 7669 726f 6e6d 656e  class Environmen
-00002960: 7450 726f 6669 6c65 284a 736f 6e4d 6f64  tProfile(JsonMod
-00002970: 656c 293a 0a20 2020 2063 6f64 656e 616d  el):.    codenam
-00002980: 653a 2073 7472 203d 2046 6965 6c64 282e  e: str = Field(.
-00002990: 2e2e 290a 2020 2020 736f 7572 6365 3a20  ..).    source: 
-000029a0: 7374 7220 3d20 4669 656c 6428 2e2e 2e29  str = Field(...)
-000029b0: 0a20 2020 2073 6365 6e61 7269 6f3a 2073  .    scenario: s
-000029c0: 7472 203d 2046 6965 6c64 282e 2e2e 290a  tr = Field(...).
-000029d0: 2020 2020 6167 656e 745f 676f 616c 733a      agent_goals:
-000029e0: 206c 6973 745b 7374 725d 203d 2046 6965   list[str] = Fie
-000029f0: 6c64 282e 2e2e 290a 2020 2020 2e2e 2e0a  ld(...).    ....
-00002a00: 6060 600a 0a60 6060 7079 7468 6f6e 0a0a  ```..```python..
-00002a10: 6672 6f6d 2073 6f74 6f70 6961 2e64 6174  from sotopia.dat
-00002a20: 6162 6173 652e 7065 7273 6973 7465 6e74  abase.persistent
-00002a30: 5f70 726f 6669 6c65 2069 6d70 6f72 7420  _profile import 
-00002a40: 4167 656e 7450 726f 6669 6c65 2c20 456e  AgentProfile, En
-00002a50: 7669 726f 6e6d 656e 7450 726f 6669 6c65  vironmentProfile
-00002a60: 0a0a 6465 6620 6164 645f 6167 656e 745f  ..def add_agent_
-00002a70: 746f 5f64 6174 6162 6173 6528 2a2a 6b77  to_database(**kw
-00002a80: 6172 6773 3a20 6469 6374 5b73 7472 2c20  args: dict[str, 
-00002a90: 416e 795d 2920 2d3e 204e 6f6e 653a 0a20  Any]) -> None:. 
-00002aa0: 2020 2061 6765 6e74 203d 2041 6765 6e74     agent = Agent
-00002ab0: 5072 6f66 696c 6528 2a2a 6b77 6172 6773  Profile(**kwargs
-00002ac0: 290a 2020 2020 6167 656e 742e 7361 7665  ).    agent.save
-00002ad0: 2829 0a0a 6465 6620 6164 645f 656e 765f  ()..def add_env_
-00002ae0: 7072 6f66 696c 6528 2a2a 6b77 6172 6773  profile(**kwargs
-00002af0: 3a20 6469 6374 5b73 7472 2c20 416e 795d  : dict[str, Any]
-00002b00: 2920 2d3e 204e 6f6e 653a 0a20 2020 2065  ) -> None:.    e
-00002b10: 6e76 5f70 726f 6669 6c65 203d 2045 6e76  nv_profile = Env
-00002b20: 6972 6f6e 6d65 6e74 5072 6f66 696c 6528  ironmentProfile(
-00002b30: 2a2a 6b77 6172 6773 290a 2020 2020 656e  **kwargs).    en
-00002b40: 765f 7072 6f66 696c 652e 7361 7665 2829  v_profile.save()
-00002b50: 0a60 6060 0a0a                           .```..
+00000500: 283e 3d31 2e32 332e 3132 2c3c 312e 3234  (>=1.23.12,<1.24
+00000510: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+00000520: 743a 206c 786d 6c20 283e 3d34 2e39 2e33  t: lxml (>=4.9.3
+00000530: 2c3c 352e 302e 3029 0a52 6571 7569 7265  ,<5.0.0).Require
+00000540: 732d 4469 7374 3a20 6f70 656e 6169 2028  s-Dist: openai (
+00000550: 3e3d 312e 3131 2e30 2c3c 322e 302e 3029  >=1.11.0,<2.0.0)
+00000560: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000570: 7061 6e64 6173 2028 3e3d 322e 312e 312c  pandas (>=2.1.1,
+00000580: 3c33 2e30 2e30 290a 5265 7175 6972 6573  <3.0.0).Requires
+00000590: 2d44 6973 743a 2070 616e 6461 732d 7374  -Dist: pandas-st
+000005a0: 7562 730a 5265 7175 6972 6573 2d44 6973  ubs.Requires-Dis
+000005b0: 743a 2070 7964 616e 7469 6320 283d 3d31  t: pydantic (==1
+000005c0: 2e31 302e 3132 290a 5265 7175 6972 6573  .10.12).Requires
+000005d0: 2d44 6973 743a 2072 6564 6973 2d6f 6d20  -Dist: redis-om 
+000005e0: 283e 3d30 2e32 2e31 2c3c 302e 332e 3029  (>=0.2.1,<0.3.0)
+000005f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000600: 7269 6368 2028 3e3d 3133 2e36 2e30 2c3c  rich (>=13.6.0,<
+00000610: 3134 2e30 2e30 290a 5265 7175 6972 6573  14.0.0).Requires
+00000620: 2d44 6973 743a 2073 6369 7079 2028 3e3d  -Dist: scipy (>=
+00000630: 312e 3133 2e31 2c3c 322e 302e 3029 203b  1.13.1,<2.0.0) ;
+00000640: 2065 7874 7261 203d 3d20 2265 7861 6d70   extra == "examp
+00000650: 6c65 7322 0a52 6571 7569 7265 732d 4469  les".Requires-Di
+00000660: 7374 3a20 7461 6275 6c61 7465 2028 3e3d  st: tabulate (>=
+00000670: 302e 392e 302c 3c30 2e31 302e 3029 0a52  0.9.0,<0.10.0).R
+00000680: 6571 7569 7265 732d 4469 7374 3a20 746f  equires-Dist: to
+00000690: 6765 7468 6572 2028 3e3d 302e 322e 342c  gether (>=0.2.4,
+000006a0: 3c30 2e33 2e30 290a 5265 7175 6972 6573  <0.3.0).Requires
+000006b0: 2d44 6973 743a 2074 6f72 6368 2028 3e3d  -Dist: torch (>=
+000006c0: 322e 332e 302c 3c33 2e30 2e30 2920 3b20  2.3.0,<3.0.0) ; 
+000006d0: 6578 7472 6120 3d3d 2022 6578 616d 706c  extra == "exampl
+000006e0: 6573 220a 5265 7175 6972 6573 2d44 6973  es".Requires-Dis
+000006f0: 743a 2074 7261 6e73 666f 726d 6572 7320  t: transformers 
+00000700: 283e 3d34 2e34 312e 302c 3c35 2e30 2e30  (>=4.41.0,<5.0.0
+00000710: 2920 3b20 6578 7472 6120 3d3d 2022 6578  ) ; extra == "ex
+00000720: 616d 706c 6573 220a 5265 7175 6972 6573  amples".Requires
+00000730: 2d44 6973 743a 2074 7970 6573 2d74 7164  -Dist: types-tqd
+00000740: 6d0a 5265 7175 6972 6573 2d44 6973 743a  m.Requires-Dist:
+00000750: 2078 6d6c 746f 6469 6374 2028 3e3d 302e   xmltodict (>=0.
+00000760: 3133 2e30 2c3c 302e 3134 2e30 290a 4465  13.0,<0.14.0).De
+00000770: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+00000780: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+00000790: 6b64 6f77 6e0a 0a3c 6469 7620 7374 796c  kdown..<div styl
+000007a0: 653d 2277 6964 7468 3a20 3130 3025 3b22  e="width: 100%;"
+000007b0: 3e0a 2020 3c69 6d67 2073 7263 3d22 6669  >.  <img src="fi
+000007c0: 6773 2f74 6974 6c65 2e70 6e67 2220 7374  gs/title.png" st
+000007d0: 796c 653d 2277 6964 7468 3a20 3130 3025  yle="width: 100%
+000007e0: 3b22 2061 6c74 3d22 736f 746f 7069 6122  ;" alt="sotopia"
+000007f0: 3e3c 2f69 6d67 3e0a 3c2f 6469 763e 0a0a  ></img>.</div>..
+00000800: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000810: 7222 3e53 6f74 6f70 6961 3a20 616e 204f  r">Sotopia: an O
+00000820: 7065 6e2d 656e 6465 6420 536f 6369 616c  pen-ended Social
+00000830: 204c 6561 726e 696e 6720 456e 7669 726f   Learning Enviro
+00000840: 6e6d 656e 743c 2f68 313e 0a0a 3c64 6976  nment</h1>..<div
+00000850: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000860: 0a0a 5b21 5b70 7970 695d 2868 7474 7073  ..[![pypi](https
+00000870: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000880: 6f2f 7079 7069 2f76 2f73 6f74 6f70 6961  o/pypi/v/sotopia
+00000890: 2e73 7667 295d 2868 7474 7073 3a2f 2f70  .svg)](https://p
+000008a0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+000008b0: 7970 692f 736f 746f 7069 6129 0a5b 215b  ypi/sotopia).[![
+000008c0: 7665 7273 696f 6e73 5d28 6874 7470 733a  versions](https:
+000008d0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000008e0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+000008f0: 2f73 6f74 6f70 6961 2e73 7667 295d 2868  /sotopia.svg)](h
+00000900: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000910: 6d2f 736f 746f 7069 612f 736f 746f 7069  m/sotopia/sotopi
+00000920: 6129 0a5b 215b 4349 5d28 6874 7470 733a  a).[![CI](https:
+00000930: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000940: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
+00000950: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
+00000960: 736f 746f 7069 612d 6c61 622f 736f 746f  sotopia-lab/soto
+00000970: 7069 612f 7465 7374 732e 796d 6c3f 6272  pia/tests.yml?br
+00000980: 616e 6368 3d6d 6169 6e26 6c6f 676f 3d67  anch=main&logo=g
+00000990: 6974 6875 6226 6c61 6265 6c3d 4349 295d  ithub&label=CI)]
+000009a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000009b0: 636f 6d2f 736f 746f 7069 612d 6c61 622f  com/sotopia-lab/
+000009c0: 736f 746f 7069 612f 6163 7469 6f6e 733f  sotopia/actions?
+000009d0: 7175 6572 793d 6272 616e 6368 2533 416d  query=branch%3Am
+000009e0: 6169 6e29 0a5b 215b 436f 6c61 625d 2868  ain).[![Colab](h
+000009f0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00000a00: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00000a10: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
+00000a20: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000a30: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00000a40: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00000a50: 652f 3134 684a 4f66 7a70 4133 3750 5255  e/14hJOfzpA37PRU
+00000a60: 7a64 6c46 6769 7156 7a55 4749 6868 6e67  zdlFgiqVzUGIhhng
+00000a70: 716e 7a3f 7573 703d 7368 6172 696e 6729  qnz?usp=sharing)
+00000a80: 0a0a 5b21 5b50 726f 6a65 6374 2050 6167  ..[![Project Pag
+00000a90: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+00000aa0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000ab0: 5072 6f6a 6563 742d 5061 6765 2d67 7265  Project-Page-gre
+00000ac0: 656e 2e73 7667 295d 2868 7474 7073 3a2f  en.svg)](https:/
+00000ad0: 2f77 7777 2e73 6f74 6f70 6961 2e77 6f72  /www.sotopia.wor
+00000ae0: 6c64 2f70 726f 6a65 6374 732f 736f 746f  ld/projects/soto
+00000af0: 7069 6129 0a5b 215b 5061 7065 7220 5044  pia).[![Paper PD
+00000b00: 465d 2868 7474 7073 3a2f 2f69 6d67 2e73  F](https://img.s
+00000b10: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000b20: 5061 7065 722d 5044 462d 7265 642e 7376  Paper-PDF-red.sv
+00000b30: 6729 5d28 6874 7470 733a 2f2f 6172 7869  g)](https://arxi
+00000b40: 762e 6f72 672f 6162 732f 3233 3130 2e31  v.org/abs/2310.1
+00000b50: 3136 3637 290a 5b21 5b44 6174 6173 6574  1667).[![Dataset
+00000b60: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000b70: 6965 6c64 732e 696f 2f62 6164 6765 2f25  ields.io/badge/%
+00000b80: 4630 2539 4625 4134 2539 372d 536f 746f  F0%9F%A4%97-Soto
+00000b90: 7069 6125 3230 4461 7461 7365 742d 7965  pia%20Dataset-ye
+00000ba0: 6c6c 6f77 295d 2868 7474 7073 3a2f 2f68  llow)](https://h
+00000bb0: 7567 6769 6e67 6661 6365 2e63 6f2f 6461  uggingface.co/da
+00000bc0: 7461 7365 7473 2f63 6d75 2d6c 7469 2f73  tasets/cmu-lti/s
+00000bd0: 6f74 6f70 6961 290a 5b21 5b44 656d 6f5d  otopia).[![Demo]
+00000be0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000bf0: 656c 6473 2e69 6f2f 6261 6467 652f 2546  elds.io/badge/%F
+00000c00: 3025 3946 2541 3425 3937 2d53 6f74 6f70  0%9F%A4%97-Sotop
+00000c10: 6961 2532 3044 656d 6f2d 6f72 616e 6765  ia%20Demo-orange
+00000c20: 295d 2868 7474 7073 3a2f 2f68 7567 6769  )](https://huggi
+00000c30: 6e67 6661 6365 2e63 6f2f 7370 6163 6573  ngface.co/spaces
+00000c40: 2f63 6d75 2d6c 7469 2f73 6f74 6f70 6961  /cmu-lti/sotopia
+00000c50: 2d73 7061 6365 2f29 0a0a 0a0a 3c2f 6469  -space/)....</di
+00000c60: 763e 0a0a 2323 204e 6577 730a 0a2a 205b  v>..## News..* [
+00000c70: 3035 2f32 3032 345d 2053 6f74 6f70 6961  05/2024] Sotopia
+00000c80: 2069 7320 7072 6573 656e 7465 6420 6174   is presented at
+00000c90: 2049 434c 5220 3230 3234 2061 7320 6120   ICLR 2024 as a 
+00000ca0: 7370 6f74 6c69 6768 7420 e2ad 9021 0a2a  spotlight ...!.*
+00000cb0: 205b 3035 2f32 3032 345d 2057 6520 7265   [05/2024] We re
+00000cc0: 6c65 6173 6520 5b61 2073 696d 706c 6520  lease [a simple 
+00000cd0: 7475 746f 7269 616c 5d28 6874 7470 733a  tutorial](https:
+00000ce0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00000cf0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00000d00: 652f 3134 684a 4f66 7a70 4133 3750 5255  e/14hJOfzpA37PRU
+00000d10: 7a64 6c46 6769 7156 7a55 4749 6868 6e67  zdlFgiqVzUGIhhng
+00000d20: 716e 7a3f 7573 703d 7368 6172 696e 6729  qnz?usp=sharing)
+00000d30: 2066 6f72 2079 6f75 2074 6f20 7275 6e20   for you to run 
+00000d40: 736f 746f 7069 6120 656e 642d 746f 2d65  sotopia end-to-e
+00000d50: 6e64 206f 6e20 676f 6f67 6c65 2063 6f6c  nd on google col
+00000d60: 6162 2e0a 0a0a 2323 2049 6e74 726f 6475  ab....## Introdu
+00000d70: 6374 696f 6e0a 0a53 6f74 6f70 6961 2069  ction..Sotopia i
+00000d80: 7320 616e 206f 7065 6e2d 656e 6465 6420  s an open-ended 
+00000d90: 736f 6369 616c 206c 6561 726e 696e 6720  social learning 
+00000da0: 656e 7669 726f 6e6d 656e 7420 7468 6174  environment that
+00000db0: 2061 6c6c 6f77 7320 6167 656e 7473 2074   allows agents t
+00000dc0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00000dd0: 6561 6368 206f 7468 6572 2061 6e64 2074  each other and t
+00000de0: 6865 2065 6e76 6972 6f6e 6d65 6e74 2e20  he environment. 
+00000df0: 5468 6520 656e 7669 726f 6e6d 656e 7420  The environment 
+00000e00: 6973 2064 6573 6967 6e65 6420 746f 2062  is designed to b
+00000e10: 6520 6120 706c 6174 666f 726d 2066 6f72  e a platform for
+00000e20: 2065 7661 6c75 6174 696e 6720 616e 6420   evaluating and 
+00000e30: 6661 6369 6c69 6174 696e 6720 736f 6369  faciliating soci
+00000e40: 616c 2069 6e74 656c 6c69 6765 6e63 6520  al intelligence 
+00000e50: 696e 206c 616e 6775 6167 6520 6167 656e  in language agen
+00000e60: 7473 2e20 5468 6520 656e 7669 726f 6e6d  ts. The environm
+00000e70: 656e 7420 6973 2064 6573 6967 6e65 6420  ent is designed 
+00000e80: 746f 2062 6520 6f70 656e 2d65 6e64 6564  to be open-ended
+00000e90: 2c20 6d65 616e 696e 6720 7468 6174 2074  , meaning that t
+00000ea0: 6865 2065 6e76 6972 6f6e 6d65 6e74 2063  he environment c
+00000eb0: 616e 2062 6520 6561 7369 6c79 2065 7874  an be easily ext
+00000ec0: 656e 6465 6420 746f 2069 6e63 6c75 6465  ended to include
+00000ed0: 206e 6577 2065 6e76 6972 6f6e 6d65 6e74   new environment
+00000ee0: 7320 616e 6420 6e65 7720 6167 656e 7473  s and new agents
+00000ef0: 2e20 5468 6520 656e 7669 726f 6e6d 656e  . The environmen
+00000f00: 7420 6973 2061 6c73 6f20 6465 7369 676e  t is also design
+00000f10: 6564 2074 6f20 6265 2073 6361 6c61 626c  ed to be scalabl
+00000f20: 652c 206d 6561 6e69 6e67 2074 6861 7420  e, meaning that 
+00000f30: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
+00000f40: 6361 6e20 6265 2065 6173 696c 7920 7363  can be easily sc
+00000f50: 616c 6564 2074 6f20 696e 636c 7564 6520  aled to include 
+00000f60: 6120 6c61 7267 6520 6e75 6d62 6572 206f  a large number o
+00000f70: 6620 6167 656e 7473 2061 6e64 2065 6e76  f agents and env
+00000f80: 6972 6f6e 6d65 6e74 732e 0a0a 0a0a 6060  ironments.....``
+00000f90: 6062 6962 7465 780a 4069 6e70 726f 6365  `bibtex.@inproce
+00000fa0: 6564 696e 6773 7b7a 686f 7532 3032 3473  edings{zhou2024s
+00000fb0: 6f74 6f70 6961 2c0a 2020 7469 746c 6520  otopia,.  title 
+00000fc0: 3d20 7b53 4f54 4f50 4941 3a20 496e 7465  = {SOTOPIA: Inte
+00000fd0: 7261 6374 6976 6520 4576 616c 7561 7469  ractive Evaluati
+00000fe0: 6f6e 2066 6f72 2053 6f63 6961 6c20 496e  on for Social In
+00000ff0: 7465 6c6c 6967 656e 6365 2069 6e20 4c61  telligence in La
+00001000: 6e67 7561 6765 2041 6765 6e74 737d 2c0a  nguage Agents},.
+00001010: 2020 6175 7468 6f72 203d 207b 5a68 6f75    author = {Zhou
+00001020: 2a2c 2058 7568 7569 2061 6e64 205a 6875  *, Xuhui and Zhu
+00001030: 2a2c 2048 616f 2061 6e64 204d 6174 6875  *, Hao and Mathu
+00001040: 722c 204c 6565 6e61 2061 6e64 205a 6861  r, Leena and Zha
+00001050: 6e67 2c20 5275 6f68 6f6e 6720 616e 6420  ng, Ruohong and 
+00001060: 5169 2c20 5a68 656e 6779 616e 6720 616e  Qi, Zhengyang an
+00001070: 6420 5975 2c20 4861 6f66 6569 2061 6e64  d Yu, Haofei and
+00001080: 204d 6f72 656e 6379 2c20 4c6f 7569 732d   Morency, Louis-
+00001090: 5068 696c 6970 7065 2061 6e64 2042 6973  Philippe and Bis
+000010a0: 6b2c 2059 6f6e 6174 616e 2061 6e64 2046  k, Yonatan and F
+000010b0: 7269 6564 2c20 4461 6e69 656c 2061 6e64  ried, Daniel and
+000010c0: 204e 6575 6269 672c 2047 7261 6861 6d20   Neubig, Graham 
+000010d0: 616e 6420 5361 702c 204d 6161 7274 656e  and Sap, Maarten
+000010e0: 7d2c 0a20 206a 6f75 726e 616c 203d 207b  },.  journal = {
+000010f0: 4943 4c52 7d2c 0a20 2079 6561 7220 3d20  ICLR},.  year = 
+00001100: 7b32 3032 347d 2c0a 2020 7572 6c20 3d20  {2024},.  url = 
+00001110: 7b68 7474 7073 3a2f 2f6f 7065 6e72 6576  {https://openrev
+00001120: 6965 772e 6e65 742f 666f 7275 6d3f 6964  iew.net/forum?id
+00001130: 3d6d 4d37 5675 7262 4134 727d 2c0a 7d0a  =mM7VurbA4r},.}.
+00001140: 6060 600a 0a23 2320 4865 6c70 0a53 6565  ```..## Help.See
+00001150: 205b 646f 6375 6d65 6e74 6174 696f 6e5d   [documentation]
+00001160: 2868 7474 7073 3a2f 2f64 6f63 732e 736f  (https://docs.so
+00001170: 746f 7069 612e 776f 726c 6429 2066 6f72  topia.world) for
+00001180: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
+00001190: 0a23 2320 4765 7420 7374 6172 7465 640a  .## Get started.
+000011a0: 2323 2320 5573 6520 6f6e 2047 6f6f 676c  ### Use on Googl
+000011b0: 6520 436f 6c61 620a 0a49 6620 796f 7520  e Colab..If you 
+000011c0: 7761 6e74 2074 6f20 7472 7920 6974 206f  want to try it o
+000011d0: 7574 206f 6e20 476f 6f67 6c65 2043 6f6c  ut on Google Col
+000011e0: 6162 2066 6972 7374 2c20 706c 6561 7365  ab first, please
+000011f0: 2063 6865 636b 206f 7574 206f 7572 2043   check out our C
+00001200: 6f6c 6162 2054 7574 6f72 6961 6c20 5365  olab Tutorial Se
+00001210: 7269 6573 3a0a 0a3c 6f6c 3e0a 3c6c 693e  ries:..<ol>.<li>
+00001220: 2042 6173 6963 0a20 203c 6f6c 3e0a 2020   Basic.  <ol>.  
+00001230: 2020 3c6c 693e 203c 6120 6872 6566 3d22    <li> <a href="
+00001240: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00001250: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00001260: 6d2f 6472 6976 652f 3134 684a 4f66 7a70  m/drive/14hJOfzp
+00001270: 4133 3750 5255 7a64 6c46 6769 7156 7a55  A37PRUzdlFgiqVzU
+00001280: 4749 6868 6e67 716e 7a3f 7573 703d 7368  GIhhngqnz?usp=sh
+00001290: 6172 696e 6722 3e31 2e31 2050 6c61 7969  aring">1.1 Playi
+000012a0: 6e67 2077 6974 6820 536f 746f 7069 6120  ng with Sotopia 
+000012b0: 696e 2061 2047 6f6f 676c 6520 436f 6c61  in a Google Cola
+000012c0: 6220 4e6f 7465 626f 6f6b 3c2f 613e 203c  b Notebook</a> <
+000012d0: 2f6c 693e 0a20 2020 203c 6c69 3e20 3c61  /li>.    <li> <a
+000012e0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+000012f0: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00001300: 6f67 6c65 2e63 6f6d 2f64 7269 7665 2f31  ogle.com/drive/1
+00001310: 4769 3255 3363 4130 4b47 316e 656b 7731  Gi2U3cA0KG1nekw1
+00001320: 4130 4e30 445a 7078 3667 4b72 6a38 4e63  A0N0DZpx6gKrj8Nc
+00001330: 3f75 7370 3d73 6861 7269 6e67 223e 312e  ?usp=sharing">1.
+00001340: 3220 4272 6f77 7369 6e67 2073 6f74 6f70  2 Browsing sotop
+00001350: 6961 2064 6174 613c 2f61 3e20 3c2f 6c69  ia data</a> </li
+00001360: 3e0a 2020 3c2f 6f6c 3e0a 3c2f 6c69 3e0a  >.  </ol>.</li>.
+00001370: 3c6c 693e 0a42 7569 6c64 696e 6720 796f  <li>.Building yo
+00001380: 7572 206f 776e 2073 6f63 6961 6c20 6167  ur own social ag
+00001390: 656e 7420 2863 6f6d 696e 6720 736f 6f6e  ent (coming soon
+000013a0: 2129 0a3c 2f6c 693e 0a3c 2f6f 6c3e 0a0a  !).</li>.</ol>..
+000013b0: 2323 2320 496e 7374 616c 6c20 6c6f 6361  ### Install loca
+000013c0: 6c6c 790a 5468 6973 2070 6163 6b61 6765  lly.This package
+000013d0: 2073 7570 706f 7274 7320 5079 7468 6f6e   supports Python
+000013e0: 2033 2e31 3120 616e 6420 6162 6f76 652e   3.11 and above.
+000013f0: 2049 6e20 6f6e 6520 6c69 6e65 2c0a 6070   In one line,.`p
+00001400: 6970 2069 6e73 7461 6c6c 2073 6f74 6f70  ip install sotop
+00001410: 6961 6020 6f72 2060 7069 7020 696e 7374  ia` or `pip inst
+00001420: 616c 6c20 7576 3b20 7576 2070 6970 2069  all uv; uv pip i
+00001430: 6e73 7461 6c6c 2073 6f74 6f70 6961 602e  nstall sotopia`.
+00001440: 0a0a 4f72 2066 726f 6d20 7363 7261 7463  ..Or from scratc
+00001450: 682c 2075 7365 2061 2076 6972 7475 616c  h, use a virtual
+00001460: 2065 6e76 6972 6f6e 6d65 6e74 2c20 652e   environment, e.
+00001470: 672e 2077 6974 6820 616e 6163 6f6e 6461  g. with anaconda
+00001480: 333a 2060 636f 6e64 6120 6372 6561 7465  3: `conda create
+00001490: 202d 6e20 736f 746f 7069 6120 7079 7468   -n sotopia pyth
+000014a0: 6f6e 3d33 2e31 313b 2063 6f6e 6461 2061  on=3.11; conda a
+000014b0: 6374 6976 6174 6520 736f 746f 7069 613b  ctivate sotopia;
+000014c0: 2063 7572 6c20 2d73 534c 2068 7474 7073   curl -sSL https
+000014d0: 3a2f 2f69 6e73 7461 6c6c 2e70 7974 686f  ://install.pytho
+000014e0: 6e2d 706f 6574 7279 2e6f 7267 207c 2070  n-poetry.org | p
+000014f0: 7974 686f 6e33 602e 2054 6865 6e2c 2069  ython3`. Then, i
+00001500: 6e73 7461 6c6c 2074 6865 2072 6571 7569  nstall the requi
+00001510: 7265 6d65 6e74 7320 616e 6420 7468 6973  rements and this
+00001520: 2070 6163 6b61 6765 2e0a 6060 6062 6173   package..```bas
+00001530: 680a 706f 6574 7279 2069 6e73 7461 6c6c  h.poetry install
+00001540: 0a60 6060 0a0a 4f70 656e 4149 206b 6579  .```..OpenAI key
+00001550: 2069 7320 7265 7175 6972 6564 2074 6f20   is required to 
+00001560: 7275 6e20 7468 6520 636f 6465 2e20 506c  run the code. Pl
+00001570: 6561 7365 2073 6574 2074 6865 2065 6e76  ease set the env
+00001580: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00001590: 6520 604f 5045 4e41 495f 4150 495f 4b45  e `OPENAI_API_KE
+000015a0: 5960 2074 6f20 796f 7572 206b 6579 2e20  Y` to your key. 
+000015b0: 5468 6520 7265 636f 6d6d 656e 6420 7761  The recommend wa
+000015c0: 7920 6973 2074 6f20 6164 6420 7468 6520  y is to add the 
+000015d0: 6b65 7920 746f 2074 6865 2063 6f6e 6461  key to the conda
+000015e0: 2065 6e76 6972 6f6e 6d65 6e74 3a0a 6060   environment:.``
+000015f0: 6062 6173 680a 636f 6e64 6120 656e 7620  `bash.conda env 
+00001600: 636f 6e66 6967 2076 6172 7320 7365 7420  config vars set 
+00001610: 4f50 454e 4149 5f41 5049 5f4b 4559 3d79  OPENAI_API_KEY=y
+00001620: 6f75 725f 6b65 790a 6060 600a 0a46 6f72  our_key.```..For
+00001630: 2073 6f6d 6520 6578 7065 7269 6d65 6e74   some experiment
+00001640: 732c 2054 6f67 6574 6865 7241 4920 6b65  s, TogetherAI ke
+00001650: 7920 6973 2072 6571 7569 7265 6420 746f  y is required to
+00001660: 2072 756e 2074 6865 2063 6f64 652e 2050   run the code. P
+00001670: 6c65 6173 6520 7365 7420 7468 6520 656e  lease set the en
+00001680: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00001690: 6c65 2060 544f 4745 5448 4552 5f41 5049  le `TOGETHER_API
+000016a0: 5f4b 4559 6020 746f 2079 6f75 7220 6b65  _KEY` to your ke
+000016b0: 792e 2054 6865 2072 6563 6f6d 6d65 6e64  y. The recommend
+000016c0: 2077 6179 2069 7320 746f 2061 6464 2074   way is to add t
+000016d0: 6865 206b 6579 2074 6f20 7468 6520 636f  he key to the co
+000016e0: 6e64 6120 656e 7669 726f 6e6d 656e 743a  nda environment:
+000016f0: 0a60 6060 6261 7368 0a63 6f6e 6461 2065  .```bash.conda e
+00001700: 6e76 2063 6f6e 6669 6720 7661 7273 2073  nv config vars s
+00001710: 6574 2054 4f47 4554 4845 525f 4150 495f  et TOGETHER_API_
+00001720: 4b45 593d 796f 7572 5f6b 6579 0a60 6060  KEY=your_key.```
+00001730: 0a0a 4120 7265 6469 732d 7374 6163 6b20  ..A redis-stack 
+00001740: 7365 7276 6572 2069 7320 7265 7175 6972  server is requir
+00001750: 6564 2074 6f20 7275 6e20 7468 6520 636f  ed to run the co
+00001760: 6465 2e20 506c 6561 7365 2066 6f6c 6c6f  de. Please follo
+00001770: 7720 7468 6520 5b69 6e73 7472 7563 7469  w the [instructi
+00001780: 6f6e 5d28 6874 7470 733a 2f2f 7265 6469  on](https://redi
+00001790: 732e 696f 2f64 6f63 732f 7374 6163 6b2f  s.io/docs/stack/
+000017a0: 6765 742d 7374 6172 7465 642f 696e 7374  get-started/inst
+000017b0: 616c 6c2f 646f 636b 6572 2f29 2074 6f20  all/docker/) to 
+000017c0: 7374 6172 7420 6120 7265 6469 732d 7374  start a redis-st
+000017d0: 6163 6b20 7365 7276 6572 206f 7220 7573  ack server or us
+000017e0: 6520 616e 2065 7869 7374 696e 6720 7365  e an existing se
+000017f0: 7276 6572 2e20 596f 7520 6361 6e20 616c  rver. You can al
+00001800: 736f 2063 6865 636b 205b 5126 415d 282f  so check [Q&A](/
+00001810: 646f 6373 2f61 6c6c 5f74 6865 5f69 7373  docs/all_the_iss
+00001820: 7565 732e 6d64 2920 746f 2069 6e69 7469  ues.md) to initi
+00001830: 6174 6520 7468 6520 7265 6469 7320 7365  ate the redis se
+00001840: 7276 6572 2077 6974 6820 7468 6520 536f  rver with the So
+00001850: 746f 7069 6120 6461 7461 2e0a 0a54 6865  topia data...The
+00001860: 2060 5245 4449 535f 4f4d 5f55 524c 6020   `REDIS_OM_URL` 
+00001870: 6e65 6564 2074 6f20 6265 2073 6574 2062  need to be set b
+00001880: 6566 6f72 6520 6c6f 6164 696e 6720 616e  efore loading an
+00001890: 6420 7361 7669 6e67 2061 6765 6e74 733a  d saving agents:
+000018a0: 0a60 6060 6261 7368 0a63 6f6e 6461 2065  .```bash.conda e
+000018b0: 6e76 2063 6f6e 6669 6720 7661 7273 2073  nv config vars s
+000018c0: 6574 2052 4544 4953 5f4f 4d5f 5552 4c3d  et REDIS_OM_URL=
+000018d0: 2272 6564 6973 3a2f 2f75 7365 723a 7061  "redis://user:pa
+000018e0: 7373 776f 7264 4068 6f73 743a 706f 7274  ssword@host:port
+000018f0: 220a 6060 600a 0a4d 616b 6520 6120 666f  ".```..Make a fo
+00001900: 6c64 6572 2074 6f20 7374 6f72 6520 7468  lder to store th
+00001910: 6520 6c6f 6773 3a0a 6060 6062 6173 680a  e logs:.```bash.
+00001920: 6d6b 6469 7220 6c6f 6773 0a60 6060 0a0a  mkdir logs.```..
+00001930: 0a0a 2323 2045 6173 7920 5361 6d70 6c65  ..## Easy Sample
+00001940: 2053 6572 7665 720a 596f 7520 6361 6e20   Server.You can 
+00001950: 7669 6577 2061 6e20 6570 6973 6f64 6520  view an episode 
+00001960: 6465 6d6f 2077 6974 6820 6465 6661 756c  demo with defaul
+00001970: 7420 7061 7261 6d65 7465 7273 2077 6974  t parameters wit
+00001980: 6820 7468 6520 666f 6c6c 6f77 696e 673a  h the following:
+00001990: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+000019a0: 7420 6173 796e 6369 6f0a 6672 6f6d 2073  t asyncio.from s
+000019b0: 6f74 6f70 6961 2e73 616d 706c 6572 7320  otopia.samplers 
+000019c0: 696d 706f 7274 2055 6e69 666f 726d 5361  import UniformSa
+000019d0: 6d70 6c65 720a 6672 6f6d 2073 6f74 6f70  mpler.from sotop
+000019e0: 6961 2e73 6572 7665 7220 696d 706f 7274  ia.server import
+000019f0: 2072 756e 5f61 7379 6e63 5f73 6572 7665   run_async_serve
+00001a00: 720a 0a61 7379 6e63 696f 2e72 756e 280a  r..asyncio.run(.
+00001a10: 2020 2020 7275 6e5f 6173 796e 635f 7365      run_async_se
+00001a20: 7276 6572 280a 2020 2020 2020 2020 6d6f  rver(.        mo
+00001a30: 6465 6c5f 6469 6374 3d7b 0a20 2020 2020  del_dict={.     
+00001a40: 2020 2020 2020 2022 656e 7622 3a20 2267         "env": "g
+00001a50: 7074 2d34 222c 0a20 2020 2020 2020 2020  pt-4",.         
+00001a60: 2020 2022 6167 656e 7431 223a 2022 6770     "agent1": "gp
+00001a70: 742d 332e 352d 7475 7262 6f22 2c0a 2020  t-3.5-turbo",.  
+00001a80: 2020 2020 2020 2020 2020 2261 6765 6e74            "agent
+00001a90: 3222 3a20 2267 7074 2d33 2e35 2d74 7572  2": "gpt-3.5-tur
+00001aa0: 626f 222c 0a20 2020 2020 2020 207d 2c0a  bo",.        },.
+00001ab0: 2020 2020 2020 2020 7361 6d70 6c65 723d          sampler=
+00001ac0: 556e 6966 6f72 6d53 616d 706c 6572 2829  UniformSampler()
+00001ad0: 2c0a 2020 2020 290a 290a 6060 600a 6f72  ,.    ).).```.or
+00001ae0: 2072 756e 0a60 6060 6261 7368 0a70 7974   run.```bash.pyt
+00001af0: 686f 6e20 6578 616d 706c 6573 2f6d 696e  hon examples/min
+00001b00: 696d 616c 6973 745f 6465 6d6f 2e70 790a  imalist_demo.py.
+00001b10: 6060 600a 0a23 2320 436f 6e74 7269 6275  ```..## Contribu
+00001b20: 7469 6f6e 0a23 2323 2320 496e 7374 616c  tion.#### Instal
+00001b30: 6c20 6465 7620 6f70 7469 6f6e 730a 466f  l dev options.Fo
+00001b40: 6c6c 6f77 2074 6865 2069 6e73 7461 6c6c  llow the install
+00001b50: 6174 696f 6e20 696e 7374 7275 6374 696f  ation instructio
+00001b60: 6e20 6162 6f76 6520 616e 6420 7468 656e  n above and then
+00001b70: 2c20 696e 7374 6561 6420 6f66 2072 756e  , instead of run
+00001b80: 6e69 6e67 2060 7079 7468 6f6e 202d 6d20  ning `python -m 
+00001b90: 7069 7020 696e 7374 616c 6c20 2d65 202e  pip install -e .
+00001ba0: 602c 2072 756e 2074 6865 2066 6f6c 6c6f  `, run the follo
+00001bb0: 7769 6e67 2063 6f6d 6d61 6e64 733a 0a0a  wing commands:..
+00001bc0: 6060 6062 6173 680a 7079 7468 6f6e 202d  ```bash.python -
+00001bd0: 6d20 7069 7020 696e 7374 616c 6c20 2d65  m pip install -e
+00001be0: 2022 2e5b 6465 765d 220a 6d79 7079 202d   ".[dev]".mypy -
+00001bf0: 2d69 6e73 7461 6c6c 2d74 7970 6573 202d  -install-types -
+00001c00: 2d6e 6f6e 2d69 6e74 6572 6163 7469 7665  -non-interactive
+00001c10: 2073 6f74 6f70 6961 0a70 7974 686f 6e20   sotopia.python 
+00001c20: 2d6d 2070 6970 2069 6e73 7461 6c6c 2070  -m pip install p
+00001c30: 7265 2d63 6f6d 6d69 740a 7072 652d 636f  re-commit.pre-co
+00001c40: 6d6d 6974 2069 6e73 7461 6c6c 0a60 6060  mmit install.```
+00001c50: 0a23 2323 2320 4e65 7720 6272 616e 6368  .#### New branch
+00001c60: 2066 6f72 2065 6163 6820 6665 6174 7572   for each featur
+00001c70: 650a 6067 6974 2063 6865 636b 6f75 7420  e.`git checkout 
+00001c80: 2d62 2066 6561 7475 7265 2f66 6561 7475  -b feature/featu
+00001c90: 7265 2d6e 616d 6560 2061 6e64 2050 5220  re-name` and PR 
+00001ca0: 746f 2060 6d61 696e 6020 6272 616e 6368  to `main` branch
+00001cb0: 2e0a 2323 2323 2042 6566 6f72 6520 636f  ..#### Before co
+00001cc0: 6d6d 6974 7469 6e67 0a52 756e 2060 7079  mmitting.Run `py
+00001cd0: 7465 7374 6020 746f 206d 616b 6520 7375  test` to make su
+00001ce0: 7265 2061 6c6c 2074 6573 7473 2070 6173  re all tests pas
+00001cf0: 7320 2874 6869 7320 7769 6c6c 2065 6e73  s (this will ens
+00001d00: 7572 6520 6479 6e61 6d69 6320 7479 7069  ure dynamic typi
+00001d10: 6e67 2070 6173 7365 6420 7769 7468 2062  ng passed with b
+00001d20: 6561 7274 7970 6529 2061 6e64 2060 6d79  eartype) and `my
+00001d30: 7079 202d 2d73 7472 6963 7420 2e60 2074  py --strict .` t
+00001d40: 6f20 6368 6563 6b20 7374 6174 6963 2074  o check static t
+00001d50: 7970 696e 672e 0a28 596f 7520 6361 6e20  yping..(You can 
+00001d60: 616c 736f 2072 756e 2060 7072 652d 636f  also run `pre-co
+00001d70: 6d6d 6974 2072 756e 202d 2d61 6c6c 2d66  mmit run --all-f
+00001d80: 696c 6573 6020 746f 2072 756e 2061 6c6c  iles` to run all
+00001d90: 2063 6865 636b 7329 0a23 2323 2320 4368   checks).#### Ch
+00001da0: 6563 6b20 6769 7468 7562 2061 6374 696f  eck github actio
+00001db0: 6e20 7265 7375 6c74 0a43 6865 636b 2074  n result.Check t
+00001dc0: 6865 2067 6974 6875 6220 6163 7469 6f6e  he github action
+00001dd0: 2072 6573 756c 7420 746f 206d 616b 6520   result to make 
+00001de0: 7375 7265 2061 6c6c 2074 6573 7473 2070  sure all tests p
+00001df0: 6173 732e 2049 6620 6e6f 742c 2066 6978  ass. If not, fix
+00001e00: 2074 6865 2065 7272 6f72 7320 616e 6420   the errors and 
+00001e10: 7075 7368 2061 6761 696e 2e0a 0a23 2320  push again...## 
+00001e20: 5275 6e6e 696e 6720 4578 7065 7269 6d65  Running Experime
+00001e30: 6e74 730a 5765 2075 7365 2060 6769 6e2d  nts.We use `gin-
+00001e40: 636f 6e66 6967 6020 746f 2063 6f6e 6669  config` to confi
+00001e50: 6775 7265 2074 6865 2065 7870 6572 696d  gure the experim
+00001e60: 656e 7473 2e20 596f 7520 646f 6e27 7420  ents. You don't 
+00001e70: 6e65 6564 2074 6f20 6265 2061 6e20 6578  need to be an ex
+00001e80: 7065 7274 2074 6f20 7573 6520 6974 2e20  pert to use it. 
+00001e90: 5468 6520 6261 7369 6320 7379 6e74 6178  The basic syntax
+00001ea0: 2069 730a 6060 6062 6173 680a 7079 7468   is.```bash.pyth
+00001eb0: 6f6e 203c 636f 6465 5f66 696c 652e 7079  on <code_file.py
+00001ec0: 3e20 2d2d 6769 6e5f 6669 6c65 203c 6769  > --gin_file <gi
+00001ed0: 6e5f 6669 6c65 313e 202d 2d67 696e 5f66  n_file1> --gin_f
+00001ee0: 696c 6520 3c67 696e 5f66 696c 6532 3e20  ile <gin_file2> 
+00001ef0: 272d 2d67 696e 2e50 4152 414d 313d 7661  '--gin.PARAM1=va
+00001f00: 6c75 6531 2720 272d 2d67 696e 2e50 4152  lue1' '--gin.PAR
+00001f10: 414d 323d 7661 6c75 6532 270a 6060 600a  AM2=value2'.```.
+00001f20: 5468 6520 602d 2d67 696e 5f66 696c 6560  The `--gin_file`
+00001f30: 2069 7320 7573 6564 2074 6f20 6c6f 6164   is used to load
+00001f40: 2061 6e64 2063 6f6d 706f 7365 2074 6865   and compose the
+00001f50: 2064 6566 6175 6c74 2063 6f6e 6669 6775   default configu
+00001f60: 7261 7469 6f6e 2e20 5468 6520 602d 2d67  ration. The `--g
+00001f70: 696e 2e50 4152 414d 313d 7661 6c75 6531  in.PARAM1=value1
+00001f80: 6020 6973 2075 7365 6420 746f 206f 7665  ` is used to ove
+00001f90: 7277 7269 7465 2074 6865 2064 6566 6175  rwrite the defau
+00001fa0: 6c74 2063 6f6e 6669 6775 7261 7469 6f6e  lt configuration
+00001fb0: 2e20 5468 6520 6c61 7465 7220 636f 6e66  . The later conf
+00001fc0: 6967 7572 6174 696f 6e20 7769 6c6c 2061  iguration will a
+00001fd0: 6c77 6179 7320 6f76 6572 7772 6974 6520  lways overwrite 
+00001fe0: 7468 6520 7072 6576 696f 7573 206f 6e65  the previous one
+00001ff0: 2e0a 0a48 6572 6520 6973 2061 6e20 6578  ...Here is an ex
+00002000: 616d 706c 6520 6f66 2072 756e 6e69 6e67  ample of running
+00002010: 2061 6e20 6578 7065 7269 6d65 6e74 3a0a   an experiment:.
+00002020: 0a60 6060 6261 7368 0a70 7974 686f 6e20  .```bash.python 
+00002030: 6578 616d 706c 6573 2f65 7870 6572 696d  examples/experim
+00002040: 656e 745f 6576 616c 2e70 7920 2d2d 6769  ent_eval.py --gi
+00002050: 6e5f 6669 6c65 2073 6f74 6f70 6961 5f63  n_file sotopia_c
+00002060: 6f6e 662f 6765 6e65 7261 7469 6f6e 5f75  onf/generation_u
+00002070: 7469 6c73 5f63 6f6e 662f 6765 6e65 7261  tils_conf/genera
+00002080: 7465 2e67 696e 202d 2d67 696e 5f66 696c  te.gin --gin_fil
+00002090: 6520 736f 746f 7069 615f 636f 6e66 2f73  e sotopia_conf/s
+000020a0: 6572 7665 725f 636f 6e66 2f73 6572 7665  erver_conf/serve
+000020b0: 722e 6769 6e20 2d2d 6769 6e5f 6669 6c65  r.gin --gin_file
+000020c0: 2073 6f74 6f70 6961 5f63 6f6e 662f 7275   sotopia_conf/ru
+000020d0: 6e5f 6173 796e 635f 7365 7276 6572 5f69  n_async_server_i
+000020e0: 6e5f 6261 7463 682e 6769 6e20 272d 2d67  n_batch.gin '--g
+000020f0: 696e 2e45 4e56 5f49 4453 3d5b 2230 3148  in.ENV_IDS=["01H
+00002100: 3756 4648 5044 5a56 5643 445a 5233 4141  7VFHPDZVVCDZR3AA
+00002110: 5241 3534 3743 5922 5d27 2027 2d2d 6769  RA547CY"]' '--gi
+00002120: 6e2e 4147 454e 5431 5f4d 4f44 454c 3d22  n.AGENT1_MODEL="
+00002130: 6770 742d 3422 2720 272d 2d67 696e 2e42  gpt-4"' '--gin.B
+00002140: 4154 4348 5f53 495a 453d 3230 2720 272d  ATCH_SIZE=20' '-
+00002150: 2d67 696e 2e50 5553 485f 544f 5f44 423d  -gin.PUSH_TO_DB=
+00002160: 4661 6c73 6527 2027 2d2d 6769 6e2e 5441  False' '--gin.TA
+00002170: 473d 2274 6573 7422 270a 6060 600a 466f  G="test"'.```.Fo
+00002180: 7220 7468 6520 636f 6d70 6c65 7465 2073  r the complete s
+00002190: 6574 206f 6620 7061 7261 6d65 7465 7273  et of parameters
+000021a0: 2c20 706c 6561 7365 2063 6865 636b 2074  , please check t
+000021b0: 6865 2060 736f 746f 7069 615f 636f 6e66  he `sotopia_conf
+000021c0: 6020 666f 6c64 6572 2e0a 0a54 6f20 7275  ` folder...To ru
+000021d0: 6e20 6120 6c61 7267 6520 6261 7463 6820  n a large batch 
+000021e0: 6f66 2065 6e76 6972 6f6e 6d65 6e74 732c  of environments,
+000021f0: 2079 6f75 2063 616e 2063 6861 6e67 6520   you can change 
+00002200: 7468 6520 6045 4e56 5f49 4453 6020 7061  the `ENV_IDS` pa
+00002210: 7261 6d65 7465 7220 696e 2060 736f 746f  rameter in `soto
+00002220: 7069 615f 636f 6e66 2f72 756e 5f61 7379  pia_conf/run_asy
+00002230: 6e63 5f73 6572 7665 725f 696e 5f62 6174  nc_server_in_bat
+00002240: 6368 2e67 696e 6020 746f 2061 206c 6973  ch.gin` to a lis
+00002250: 7420 6f66 2065 6e76 6972 6f6e 6d65 6e74  t of environment
+00002260: 2069 6473 2e20 5768 656e 2060 6769 6e2e   ids. When `gin.
+00002270: 454e 565f 4944 533d 3d5b 5d60 2c20 616c  ENV_IDS==[]`, al
+00002280: 6c20 656e 7669 726f 6e6d 656e 7473 206f  l environments o
+00002290: 6e20 7468 6520 4442 2077 696c 6c20 6265  n the DB will be
+000022a0: 2075 7365 642e 0a0a 2323 2047 6574 7469   used...## Getti
+000022b0: 6e67 2061 6363 6573 7320 746f 2079 6f75  ng access to you
+000022c0: 7220 7369 6d75 6c61 7469 6f6e 0a41 6674  r simulation.Aft
+000022d0: 6572 2072 756e 6e69 6e67 2065 7870 6572  er running exper
+000022e0: 696d 656e 7473 2c20 796f 7520 6361 6e20  iments, you can 
+000022f0: 676f 2074 6f20 7468 6520 6065 7861 6d70  go to the `examp
+00002300: 6c65 732f 7265 6469 735f 7374 6174 732e  les/redis_stats.
+00002310: 6970 796e 6260 206e 6f74 6562 6f6f 6b20  ipynb` notebook 
+00002320: 746f 2063 6865 636b 2074 6865 2065 7869  to check the exi
+00002330: 7374 696e 6720 6570 6973 6f64 6573 2028  sting episodes (
+00002340: 4570 6973 6f64 6520 4c6f 6720 7365 6374  Episode Log sect
+00002350: 696f 6e29 2c20 6173 2077 656c 6c20 6173  ion), as well as
+00002360: 2063 616c 6375 6c61 7465 2074 6865 2070   calculate the p
+00002370: 6572 666f 726d 616e 6365 2e0a 0a46 6f72  erformance...For
+00002380: 2074 6865 206f 7269 6769 6e61 6c20 536f   the original So
+00002390: 746f 7069 6120 7369 6d75 6c61 7469 6f6e  topia simulation
+000023a0: 2069 6e20 6f75 7220 7061 7065 7227 7320   in our paper's 
+000023b0: 6578 7065 7269 6d65 6e74 732c 2079 6f75  experiments, you
+000023c0: 2063 616e 2066 696e 6420 686f 7720 746f   can find how to
+000023d0: 2067 6574 2074 6865 6d20 696e 2074 6865   get them in the
+000023e0: 205b 5126 415d 282f 646f 6373 2f61 6c6c   [Q&A](/docs/all
+000023f0: 5f74 6865 5f69 7373 7565 732e 6d64 2920  _the_issues.md) 
+00002400: 7365 6374 696f 6e20 696e 2074 6865 2060  section in the `
+00002410: 2e2f 646f 6373 6020 666f 6c64 6572 2e0a  ./docs` folder..
+00002420: 0a23 2320 4164 6469 6e67 206e 6577 2063  .## Adding new c
+00002430: 6861 7261 6374 6572 7320 616e 6420 656e  haracters and en
+00002440: 7669 726f 6e6d 656e 7473 0a59 6f75 2063  vironments.You c
+00002450: 616e 2075 7365 2074 6865 2066 6f6c 6c6f  an use the follo
+00002460: 7769 6e67 2066 756e 6374 696f 6e20 7769  wing function wi
+00002470: 7468 2074 6865 2060 2a2a 6b77 6172 6773  th the `**kwargs
+00002480: 6020 6265 696e 6720 7468 6520 7072 6f70  ` being the prop
+00002490: 6572 7469 6573 206f 6620 7468 6520 6041  erties of the `A
+000024a0: 6765 6e74 5072 6f66 696c 6560 2063 6c61  gentProfile` cla
+000024b0: 7373 2e20 5468 6973 2069 7320 7468 6520  ss. This is the 
+000024c0: 7361 6d65 2066 6f72 2074 6865 2073 6365  same for the sce
+000024d0: 6e61 7269 6f73 2f65 6e76 6972 6f6e 6d65  narios/environme
+000024e0: 6e74 732e 0a60 6060 7079 7468 6f6e 0a63  nts..```python.c
+000024f0: 6c61 7373 2041 6765 6e74 5072 6f66 696c  lass AgentProfil
+00002500: 6528 4a73 6f6e 4d6f 6465 6c29 3a0a 2020  e(JsonModel):.  
+00002510: 2020 6669 7273 745f 6e61 6d65 3a20 7374    first_name: st
+00002520: 7220 3d20 4669 656c 6428 696e 6465 783d  r = Field(index=
+00002530: 5472 7565 290a 2020 2020 6c61 7374 5f6e  True).    last_n
+00002540: 616d 653a 2073 7472 203d 2046 6965 6c64  ame: str = Field
+00002550: 2869 6e64 6578 3d54 7275 6529 0a20 2020  (index=True).   
+00002560: 2061 6765 3a20 696e 7420 3d20 4669 656c   age: int = Fiel
+00002570: 6428 696e 6465 783d 5472 7565 2c20 6465  d(index=True, de
+00002580: 6661 756c 745f 6661 6374 6f72 793d 6c61  fault_factory=la
+00002590: 6d62 6461 3a20 3029 0a20 2020 206f 6363  mbda: 0).    occ
+000025a0: 7570 6174 696f 6e3a 2073 7472 203d 2046  upation: str = F
+000025b0: 6965 6c64 2869 6e64 6578 3d54 7275 652c  ield(index=True,
+000025c0: 2064 6566 6175 6c74 5f66 6163 746f 7279   default_factory
+000025d0: 3d6c 616d 6264 613a 2022 2229 0a20 2020  =lambda: "").   
+000025e0: 2067 656e 6465 723a 2073 7472 203d 2046   gender: str = F
+000025f0: 6965 6c64 2869 6e64 6578 3d54 7275 652c  ield(index=True,
+00002600: 2064 6566 6175 6c74 5f66 6163 746f 7279   default_factory
+00002610: 3d6c 616d 6264 613a 2022 2229 0a20 2020  =lambda: "").   
+00002620: 2067 656e 6465 725f 7072 6f6e 6f75 6e3a   gender_pronoun:
+00002630: 2073 7472 203d 2046 6965 6c64 2869 6e64   str = Field(ind
+00002640: 6578 3d54 7275 652c 2064 6566 6175 6c74  ex=True, default
+00002650: 5f66 6163 746f 7279 3d6c 616d 6264 613a  _factory=lambda:
+00002660: 2022 2229 0a20 2020 2070 7562 6c69 635f   "").    public_
+00002670: 696e 666f 3a20 7374 7220 3d20 4669 656c  info: str = Fiel
+00002680: 6428 696e 6465 783d 5472 7565 2c20 6465  d(index=True, de
+00002690: 6661 756c 745f 6661 6374 6f72 793d 6c61  fault_factory=la
+000026a0: 6d62 6461 3a20 2222 290a 2020 2020 6269  mbda: "").    bi
+000026b0: 675f 6669 7665 3a20 7374 7220 3d20 4669  g_five: str = Fi
+000026c0: 656c 6428 696e 6465 783d 5472 7565 2c20  eld(index=True, 
+000026d0: 6465 6661 756c 745f 6661 6374 6f72 793d  default_factory=
+000026e0: 6c61 6d62 6461 3a20 2222 290a 2020 2020  lambda: "").    
+000026f0: 6d6f 7261 6c5f 7661 6c75 6573 3a20 6c69  moral_values: li
+00002700: 7374 5b73 7472 5d20 3d20 4669 656c 6428  st[str] = Field(
+00002710: 696e 6465 783d 4661 6c73 652c 2064 6566  index=False, def
+00002720: 6175 6c74 5f66 6163 746f 7279 3d6c 616d  ault_factory=lam
+00002730: 6264 613a 205b 5d29 0a20 2020 2073 6368  bda: []).    sch
+00002740: 7761 7274 7a5f 7065 7273 6f6e 616c 5f76  wartz_personal_v
+00002750: 616c 7565 733a 206c 6973 745b 7374 725d  alues: list[str]
+00002760: 203d 2046 6965 6c64 2869 6e64 6578 3d46   = Field(index=F
+00002770: 616c 7365 2c20 6465 6661 756c 745f 6661  alse, default_fa
+00002780: 6374 6f72 793d 6c61 6d62 6461 3a20 5b5d  ctory=lambda: []
+00002790: 290a 2020 2020 7065 7273 6f6e 616c 6974  ).    personalit
+000027a0: 795f 616e 645f 7661 6c75 6573 3a20 7374  y_and_values: st
+000027b0: 7220 3d20 4669 656c 6428 696e 6465 783d  r = Field(index=
+000027c0: 5472 7565 2c20 6465 6661 756c 745f 6661  True, default_fa
+000027d0: 6374 6f72 793d 6c61 6d62 6461 3a20 2222  ctory=lambda: ""
+000027e0: 290a 2020 2020 6465 6369 7369 6f6e 5f6d  ).    decision_m
+000027f0: 616b 696e 675f 7374 796c 653a 2073 7472  aking_style: str
+00002800: 203d 2046 6965 6c64 2869 6e64 6578 3d54   = Field(index=T
+00002810: 7275 652c 2064 6566 6175 6c74 5f66 6163  rue, default_fac
+00002820: 746f 7279 3d6c 616d 6264 613a 2022 2229  tory=lambda: "")
+00002830: 0a20 2020 2073 6563 7265 743a 2073 7472  .    secret: str
+00002840: 203d 2046 6965 6c64 2864 6566 6175 6c74   = Field(default
+00002850: 5f66 6163 746f 7279 3d6c 616d 6264 613a  _factory=lambda:
+00002860: 2022 2229 0a20 2020 206d 6f64 656c 5f69   "").    model_i
+00002870: 643a 2073 7472 203d 2046 6965 6c64 2864  d: str = Field(d
+00002880: 6566 6175 6c74 5f66 6163 746f 7279 3d6c  efault_factory=l
+00002890: 616d 6264 613a 2022 2229 0a0a 636c 6173  ambda: "")..clas
+000028a0: 7320 456e 7669 726f 6e6d 656e 7450 726f  s EnvironmentPro
+000028b0: 6669 6c65 284a 736f 6e4d 6f64 656c 293a  file(JsonModel):
+000028c0: 0a20 2020 2063 6f64 656e 616d 653a 2073  .    codename: s
+000028d0: 7472 203d 2046 6965 6c64 282e 2e2e 290a  tr = Field(...).
+000028e0: 2020 2020 736f 7572 6365 3a20 7374 7220      source: str 
+000028f0: 3d20 4669 656c 6428 2e2e 2e29 0a20 2020  = Field(...).   
+00002900: 2073 6365 6e61 7269 6f3a 2073 7472 203d   scenario: str =
+00002910: 2046 6965 6c64 282e 2e2e 290a 2020 2020   Field(...).    
+00002920: 6167 656e 745f 676f 616c 733a 206c 6973  agent_goals: lis
+00002930: 745b 7374 725d 203d 2046 6965 6c64 282e  t[str] = Field(.
+00002940: 2e2e 290a 2020 2020 2e2e 2e0a 6060 600a  ..).    ....```.
+00002950: 0a60 6060 7079 7468 6f6e 0a0a 6672 6f6d  .```python..from
+00002960: 2073 6f74 6f70 6961 2e64 6174 6162 6173   sotopia.databas
+00002970: 652e 7065 7273 6973 7465 6e74 5f70 726f  e.persistent_pro
+00002980: 6669 6c65 2069 6d70 6f72 7420 4167 656e  file import Agen
+00002990: 7450 726f 6669 6c65 2c20 456e 7669 726f  tProfile, Enviro
+000029a0: 6e6d 656e 7450 726f 6669 6c65 0a0a 6465  nmentProfile..de
+000029b0: 6620 6164 645f 6167 656e 745f 746f 5f64  f add_agent_to_d
+000029c0: 6174 6162 6173 6528 2a2a 6b77 6172 6773  atabase(**kwargs
+000029d0: 3a20 6469 6374 5b73 7472 2c20 416e 795d  : dict[str, Any]
+000029e0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2061  ) -> None:.    a
+000029f0: 6765 6e74 203d 2041 6765 6e74 5072 6f66  gent = AgentProf
+00002a00: 696c 6528 2a2a 6b77 6172 6773 290a 2020  ile(**kwargs).  
+00002a10: 2020 6167 656e 742e 7361 7665 2829 0a0a    agent.save()..
+00002a20: 6465 6620 6164 645f 656e 765f 7072 6f66  def add_env_prof
+00002a30: 696c 6528 2a2a 6b77 6172 6773 3a20 6469  ile(**kwargs: di
+00002a40: 6374 5b73 7472 2c20 416e 795d 2920 2d3e  ct[str, Any]) ->
+00002a50: 204e 6f6e 653a 0a20 2020 2065 6e76 5f70   None:.    env_p
+00002a60: 726f 6669 6c65 203d 2045 6e76 6972 6f6e  rofile = Environ
+00002a70: 6d65 6e74 5072 6f66 696c 6528 2a2a 6b77  mentProfile(**kw
+00002a80: 6172 6773 290a 2020 2020 656e 765f 7072  args).    env_pr
+00002a90: 6f66 696c 652e 7361 7665 2829 0a60 6060  ofile.save().```
+00002aa0: 0a0a                                     ..
```

