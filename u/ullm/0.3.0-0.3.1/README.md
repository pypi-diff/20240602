# Comparing `tmp/ullm-0.3.0.tar.gz` & `tmp/ullm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ullm-0.3.0.tar", last modified: Tue May 28 06:35:17 2024, max compression
+gzip compressed data, was "ullm-0.3.1.tar", last modified: Sun Jun  2 12:29:39 2024, max compression
```

## Comparing `ullm-0.3.0.tar` & `ullm-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.681209 ullm-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-28 06:35:17.681209 ullm-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17551 2024-05-28 06:35:12.000000 ullm-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-28 06:35:12.000000 ullm-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:35:17.681209 ullm-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.677209 ullm-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-28 06:35:12.000000 ullm-0.3.0/tests/test_openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.681209 ullm-0.3.0/ullm/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (127)    24252 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)    20213 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/deepseek.py
--rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/iflytek.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/minimax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/moonshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/skywork.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/stepfun.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/together.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/zero_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-28 06:35:12.000000 ullm-0.3.0/ullm/zhipu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:35:17.681209 ullm-0.3.0/ullm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 06:35:17.000000 ullm-0.3.0/ullm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:29:39.862361 ullm-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-06-02 12:29:39.862361 ullm-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17551 2024-06-02 12:29:35.000000 ullm-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-06-02 12:29:35.000000 ullm-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 12:29:39.862361 ullm-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:29:39.858361 ullm-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-06-02 12:29:35.000000 ullm-0.3.1/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:29:39.862361 ullm-0.3.1/ullm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24252 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/deepseek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/iflytek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/minimax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/moonshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/skywork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/stepfun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/zero_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-06-02 12:29:35.000000 ullm-0.3.1/ullm/zhipu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 12:29:39.862361 ullm-0.3.1/ullm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-06-02 12:29:39.000000 ullm-0.3.1/ullm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-02 12:29:39.000000 ullm-0.3.1/ullm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 12:29:39.000000 ullm-0.3.1/ullm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 12:29:39.000000 ullm-0.3.1/ullm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-02 12:29:39.000000 ullm-0.3.1/ullm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-02 12:29:39.000000 ullm-0.3.1/ullm.egg-info/top_level.txt
```

### Comparing `ullm-0.3.0/PKG-INFO` & `ullm-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.3.0
+Version: 0.3.1
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.3.0 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.3.1 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
```

### Comparing `ullm-0.3.0/README.md` & `ullm-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/pyproject.toml` & `ullm-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ullm"
-version = "0.3.0"
+version = "0.3.1"
 description = "A unified interface for local Large Language Model(LLM) models and online LLM providers."
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
     "pydantic",
     "arrow",
```

### Comparing `ullm-0.3.0/tests/test_openai.py` & `ullm-0.3.1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/__init__.py` & `ullm-0.3.1/ullm/__init__.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/alibaba.py` & `ullm-0.3.1/ullm/alibaba.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/anthropic.py` & `ullm-0.3.1/ullm/anthropic.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/baichuan.py` & `ullm-0.3.1/ullm/baichuan.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/baidu.py` & `ullm-0.3.1/ullm/baidu.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/base.py` & `ullm-0.3.1/ullm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,20 +78,19 @@
 
 class ToolCall(BaseModel):
     id: Optional[str] = Field(default_factory=lambda: uuid4().hex)
     type: Literal["function"] = "function"
     function: Optional[FunctionCall] = None
 
     @model_validator(mode="after")
-    @classmethod
-    def check_tool(cls, data):
-        if data.type == "function" and not data.function:
+    def check_tool(self):
+        if self.type == "function" and not self.function:
             raise ValueError("`function` should not be empty!")
 
-        return data
+        return self
 
 
 class AssistantMessage(BaseModel):
     role: Literal["assistant"] = "assistant"
     content: Optional[str] = ""
     tool_calls: Optional[List[ToolCall]] = None
```

### Comparing `ullm-0.3.0/ullm/cli.py` & `ullm-0.3.1/ullm/cli.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/cloudflare.py` & `ullm-0.3.1/ullm/cloudflare.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/cohere.py` & `ullm-0.3.1/ullm/cohere.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/deepseek.py` & `ullm-0.3.1/ullm/deepseek.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/google.py` & `ullm-0.3.1/ullm/google.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/groq.py` & `ullm-0.3.1/ullm/groq.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/iflytek.py` & `ullm-0.3.1/ullm/iflytek.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         )
         return url
 
     @validate_call
     def chat(
         self,
         messages: conlist(ChatMessage, min_length=1),
-        config: GenerateConfig = None,
+        config: Optional[GenerateConfig] = None,
         system: Optional[str] = None,
     ) -> GenerationResult:
         self._validate_model(messages)
         api_url = self._get_api_url()
 
         messages = [IflyTekChatMessage.from_standard(message) for message in messages]
         if system:
```

### Comparing `ullm-0.3.0/ullm/minimax.py` & `ullm-0.3.1/ullm/minimax.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/moonshot.py` & `ullm-0.3.1/ullm/moonshot.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/ollama.py` & `ullm-0.3.1/ullm/ollama.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/openai.py` & `ullm-0.3.1/ullm/openai.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/openrouter.py` & `ullm-0.3.1/ullm/openrouter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional
 
 from pydantic import BaseModel, confloat, conint, conlist
 
 from .base import (
+    GenerateConfig,
     RemoteLanguageModel,
     RemoteLanguageModelMetaInfo,
 )
 from .openai import (
     OpenAIAssistantMessage,
     OpenAICompatibleModel,
     OpenAIRequestBody,
@@ -267,7 +268,24 @@
         online_models=[
             "llama-3-sonar-large-32k-online",
             "llama-3-sonar-small-32k-online",
         ],
     )
     REQUEST_BODY_CLS = OpenRouterRequestBody
     RESPONSE_BODY_CLS = OpenRouterResponseBody
+
+    def _convert_generation_config(
+        self, config: GenerateConfig, system: Optional[str] = None
+    ) -> Dict[str, Any]:
+        model_prefix = self._MODEL_PREFIX_MAP[self.model]
+        return {
+            "model": f"{model_prefix}/{self.model}",
+            "frequency_penalty": config.frequency_penalty,
+            "max_tokens": config.max_output_tokens or self.config.max_output_tokens,
+            "presence_penalty": config.presence_penalty,
+            "response_format": {"type": config.response_format} if config.response_format else None,
+            "stop": config.stop_sequences or self.config.stop_sequences,
+            "temperature": config.temperature or self.config.temperature,
+            "top_p": config.top_p or self.config.top_p,
+            "top_k": config.top_k or self.config.top_k,
+            "repetition_penalty": config.repetition_penalty,
+        }
```

### Comparing `ullm-0.3.0/ullm/perplexity.py` & `ullm-0.3.1/ullm/perplexity.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/skywork.py` & `ullm-0.3.1/ullm/skywork.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/stepfun.py` & `ullm-0.3.1/ullm/stepfun.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/together.py` & `ullm-0.3.1/ullm/together.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/zero_one.py` & `ullm-0.3.1/ullm/zero_one.py`

 * *Files identical despite different names*

### Comparing `ullm-0.3.0/ullm/zhipu.py` & `ullm-0.3.1/ullm/zhipu.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     web_search: Optional[ZhipuWebSearchTool] = None
     retrieval: Optional[ZhipuRetrievalTool] = None
 
     @model_validator(mode="before")
     @classmethod
     def check_type(cls, data):
         assert data.get(data["type"]) is not None
+        return data
 
     @classmethod
     def from_standard(cls, tool: Tool):
         return cls(type=tool.type, function=OpenAIFunctionObject.from_standard(tool.function))
 
 
 class ZhipuAIRequestBody(OpenAIRequestBody):
@@ -112,19 +113,19 @@
         self, tools: Optional[List[Tool]] = None, tool_choice: Optional[ToolChoice] = None
     ) -> Dict[str, Any]:
         if tools:
             tools = [ZhipuAITool.from_standard(tool) for tool in tools]
 
         if self.is_online_model():
             tools = tools or []
-            tools.append(ZhipuAITool(type="web_search"), web_search=ZhipuWebSearchTool(enable=True))
+            tools.append(ZhipuAITool(type="web_search", web_search=ZhipuWebSearchTool(enable=True)))
         else:
             tools = tools or []
             tools.append(
-                ZhipuAITool(type="web_search"), web_search=ZhipuWebSearchTool(enable=False)
+                ZhipuAITool(type="web_search", web_search=ZhipuWebSearchTool(enable=False))
             )
 
         return {"tools": tools}
 
     def _convert_generation_config(
         self, config: GenerateConfig, system: Optional[str] = None
     ) -> Dict[str, Any]:
```

### Comparing `ullm-0.3.0/ullm.egg-info/PKG-INFO` & `ullm-0.3.1/ullm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ullm
-Version: 0.3.0
+Version: 0.3.1
 Summary: A unified interface for local Large Language Model(LLM) models and online LLM providers.
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/monsternlp/ullm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ullm Version: 0.3.0 Summary: A unified interface
+Metadata-Version: 2.1 Name: ullm Version: 0.3.1 Summary: A unified interface
 for local Large Language Model(LLM) models and online LLM providers. Author-
 email: Linusp
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/monsternlp/
 ullm Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist: pydantic
 Requires-Dist: arrow Requires-Dist: websocket-client Requires-Dist: requests
```

### Comparing `ullm-0.3.0/ullm.egg-info/SOURCES.txt` & `ullm-0.3.1/ullm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

