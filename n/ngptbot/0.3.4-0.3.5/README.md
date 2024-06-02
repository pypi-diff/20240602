# Comparing `tmp/ngptbot-0.3.4.tar.gz` & `tmp/ngptbot-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngptbot-0.3.4.tar", max compression
+gzip compressed data, was "ngptbot-0.3.5.tar", max compression
```

## Comparing `ngptbot-0.3.4.tar` & `ngptbot-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2024-02-10 11:29:22.496858 ngptbot-0.3.4/LICENSE
--rw-r--r--   0        0        0     2882 2024-02-16 08:00:33.007208 ngptbot-0.3.4/README.md
--rw-r--r--   0        0        0       68 2024-02-21 05:45:27.117455 ngptbot-0.3.4/gptbot/__init__.py
--rw-r--r--   0        0        0    10236 2024-02-21 05:45:15.413490 ngptbot-0.3.4/gptbot/__main__.py
--rw-r--r--   0        0        0    24305 2024-02-21 05:45:55.273369 ngptbot-0.3.4/gptbot/bot.py
--rw-r--r--   0        0        0       47 2024-02-11 11:02:44.852455 ngptbot-0.3.4/gptbot/cli.py
--rw-r--r--   0        0        0     3417 2024-03-06 14:13:40.270188 ngptbot-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4098 1970-01-01 00:00:00.000000 ngptbot-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-10 11:29:22.496858 ngptbot-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3451 2024-06-02 15:39:03.854187 ngptbot-0.3.5/README.md
+-rw-r--r--   0        0        0       68 2024-02-21 05:45:27.117455 ngptbot-0.3.5/gptbot/__init__.py
+-rw-r--r--   0        0        0    10236 2024-06-02 15:45:01.683569 ngptbot-0.3.5/gptbot/__main__.py
+-rw-r--r--   0        0        0    30480 2024-06-02 15:43:53.336545 ngptbot-0.3.5/gptbot/bot.py
+-rw-r--r--   0        0        0       47 2024-02-11 11:02:44.852455 ngptbot-0.3.5/gptbot/cli.py
+-rw-r--r--   0        0        0     3417 2024-06-02 15:45:14.023404 ngptbot-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 ngptbot-0.3.5/PKG-INFO
```

### Comparing `ngptbot-0.3.4/LICENSE` & `ngptbot-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ngptbot-0.3.4/README.md` & `ngptbot-0.3.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 # Simple Wrapper For The ChatGPT API
 
-This module is designed for asynchronous usage and provides a simple interface to the OpenAI ChatGPT API.
+This module is designed for asynchronous usage and provides a simple interface to the OpenAI ChatGPT API
 
 It also provides a command-line interface for interactive usage.
 
 While it does provide synchronous methods, it is recommended to use the asynchronous methods for better performance.
 
+## Features
+
+- Asynchronous API
+- Get/Stream responses
+- Save/Load session history
+- Change parameters on the fly
+- Embed images in messages
+- Register functions to `tool_calls` with ease
+- Interactive command-line interface
+
 ## Installation
 
 ```bash
 pip install -U ngptbot
 ```
 
 ## Usage
@@ -100,7 +110,18 @@
     async for r in session.stream("Hello!"):
         print(r, end='')
 
     print(await session.send("Goodbye!"))
 
 asyncio.run(main())
 ```
+
+### Registering Functions
+
+Functions are under `Bot.funcs` and can be registered with the `add_func` decorator.
+
+```python
+@bot.add_func
+def my_func(data: str, default:int = 123):  # parameters must be annotated, variadic parameters are not supported
+    """Documentation goes here"""
+    return data  # return value must be stringifiable
+```
```

### Comparing `ngptbot-0.3.4/gptbot/__main__.py` & `ngptbot-0.3.5/gptbot/__main__.py`

 * *Files identical despite different names*

### Comparing `ngptbot-0.3.4/gptbot/bot.py` & `ngptbot-0.3.5/gptbot/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,31 +3,42 @@
 """
 
 from __future__ import annotations
 import httpx
 import ujson as json
 import tiktoken
 import math
+import inspect
+import asyncio
+import warnings
 from typing import Any, Iterable, Self, AsyncGenerator, Literal, Generator, overload
-from typing import TypeAlias, cast, Sequence
+from typing import TypeAlias, cast, Sequence, TypeVar, get_origin, get_args
 from enum import Enum
 from datetime import datetime
 from warnings import warn
 from pydantic import BaseModel, Field, validate_call, PrivateAttr
 from pydantic import field_validator, model_validator, ConfigDict
-from pydantic import field_serializer
+from pydantic import field_serializer, computed_field
 from vermils.asynctools import sync_await
 from PIL import Image, UnidentifiedImageError
 from pathlib import Path
+from itertools import chain
 from base64 import b64encode, b64decode
 from io import BytesIO
 from vermils.io import aio
 
 
+T = TypeVar('T')
+
+
 class Model(str, Enum):
+    GPT4o = "gpt-4o"
+    GPT4o_2024_05_13 = "gpt-4o-2024-05-13"
+    GPT4Turbo = "gpt-4-turbo"
+    GPT4Turbo_2024_04_09 = "gpt-4-turbo-2024-04-09"
     GPT4_0125_Preview = "gpt-4-0125-preview"
     GPT4TurboPreview = "gpt-4-turbo-preview"
     GPT4_1106_Preview = "gpt-4-1106-preview"
     GPT4VisionPreview = "gpt-4-vision-preview"
     GPT4_1106_VisionPreview = "gpt-4-1106-vision-preview"
     GPT4 = "gpt-4"
     GPT4_0613 = "gpt-4-0613"
@@ -47,14 +58,18 @@
 class ModelInfo(BaseModel):
     max_tokens: int
     updated_at: datetime
     legacy: bool = False
 
 
 INFO_MAP: dict[Model, ModelInfo] = {
+    Model.GPT4o: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 10, 1)),
+    Model.GPT4o_2024_05_13: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 10, 1)),
+    Model.GPT4Turbo: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 12, 1)),
+    Model.GPT4Turbo_2024_04_09: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 12, 1)),
     Model.GPT4_0125_Preview: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 4, 1)),
     Model.GPT4TurboPreview: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 4, 1)),
     Model.GPT4_1106_Preview: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 4, 1)),
     Model.GPT4VisionPreview: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 4, 1)),
     Model.GPT4_1106_VisionPreview: ModelInfo(max_tokens=128000, updated_at=datetime(2023, 4, 1)),
     Model.GPT4: ModelInfo(max_tokens=8192, updated_at=datetime(2021, 9, 1)),
     Model.GPT4_0613: ModelInfo(max_tokens=8192, updated_at=datetime(2021, 9, 1)),
@@ -71,14 +86,15 @@
 }
 
 
 class Role(str, Enum):
     User = "user"
     Assistant = "assistant"
     System = "system"
+    Tool = "tool"
 
 
 class Message(BaseModel):
     model_config = ConfigDict(validate_assignment=True, extra="allow")
 
     class BaseSegment(BaseModel):
         model_config = ConfigDict(extra="allow")
@@ -128,22 +144,23 @@
             return self.ImageURL(url=url, detail=img_url.detail).model_dump(mode="json")
 
         def __str__(self):
             return f"#image({self.image_url.url[:10]}...{self.image_url.url[-10:]})"
 
     role: Role
     name: str | None = None
-    content: str | list[TextSegment | ImageSegment] = ''
+    content: None | str | list[TextSegment | ImageSegment] = ''
     function_call: Any | None = None
-    tool_calls: Any | None = None
+    tool_calls: list | None = None
+    tool_call_id: str | None = None
 
     def __str__(self):
         if isinstance(self.content, str):
             return self.content
-        return ''.join(str(seg) for seg in self.content)
+        return ''.join(str(seg) for seg in self.content or '')
 
 
 SegTypes: TypeAlias = Message.TextSegment | Message.ImageSegment
 Prompt: TypeAlias = str | list[SegTypes]
 
 
 class FullChunkResponse(BaseModel):
@@ -223,25 +240,104 @@
     logprobs: bool | None = None
     top_logprobs: int | None = None
     presence_penalty: float | None = None
     seed: int | None = None
     stop: list[str] | None = None
     temperature: float = 0.5
     top_p: float = 1.0
-    tools: list[dict[str, Any]] | None = None
     tool_choice: Literal["auto", "none"] | dict[str, Any] = "auto"
     user: str | None = None
 
     proxy: str | None = None
     timeout: float | None = None
     # retries: int = 5
     # backoff: float = 1.5
     _cli: httpx.AsyncClient = PrivateAttr(default=None)
     _last_proxy: str | None = PrivateAttr(default=None)
     _last_timeout: float | None = PrivateAttr(default=None)
+    _funcs: list[Any] = PrivateAttr(default_factory=list)
+
+    @property
+    def funcs(self):
+        return self._funcs
+
+    @computed_field
+    def tools(self) -> list[dict[str, Any]] | None:
+        if not self._funcs:
+            return None
+
+        def _2typename(t):
+            if not issubclass(t, (int, float, str, bool)):
+                raise ValueError(f"Invalid type {t}")
+            return {
+                int: "integer",
+                float: "number",
+                str: "string",
+                bool: "boolean"
+            }[t]
+
+        ret = list[dict[str, Any]]()
+        for f in self.funcs:
+            d: dict[str, Any] = {
+                "type": "function",
+                "function": {
+                    "name": f.__name__,
+                    "description": f.__doc__ or '',
+                    "parameters": {
+                        "type": "object",
+                        "properties": {},
+                        "required": [],
+                    },
+                }
+            }
+            argspecs = inspect.getfullargspec(f)
+            defaults = argspecs.defaults or tuple()
+            kwonlydefaults = argspecs.kwonlydefaults or dict()
+            annotations = argspecs.annotations or dict()
+            if argspecs.varargs is not None or argspecs.varkw is not None:
+                warnings.warn(
+                    "Variadic arguments are not supported in tools", UserWarning)
+            for arg in chain(argspecs.args, argspecs.kwonlyargs):
+                if arg not in annotations:
+                    raise ValueError(f"Missing annotation for {arg}")
+                enums: tuple[Any, ...] | None = None
+                type_ = annotations[arg]
+                optional = False
+
+                if get_origin(type_) is Literal:
+                    enums = get_args(type_)
+                elif issubclass(type_, Enum):
+                    enums = tuple(e.value for e in type_)
+                if enums is not None:
+                    if not enums:
+                        raise ValueError(f"Empty enum/literals for {arg}")
+                    type_ = type(enums[0])
+
+                if arg in argspecs.kwonlyargs:
+                    optional = arg in kwonlydefaults
+                else:
+                    optional = arg in argspecs.args[-len(defaults):]
+
+                p = {
+                    "type": _2typename(type_),
+                    "description": "",
+                }
+                if enums is not None:
+                    p["enum"] = enums
+
+                d["function"]["parameters"]["properties"][arg] = p
+                if not optional:
+                    d["function"]["parameters"]["required"].append(arg)
+            ret.append(d)
+
+        return ret
+
+    def add_func(self, f: T) -> T:
+        self._funcs.append(f)
+        return f
 
     @model_validator(mode="after")
     def post_init(self) -> Self:
         if (cast(None | httpx.AsyncClient, self._cli) is None
                 or self.proxy != self._last_proxy or self.timeout != self._last_timeout):
             self.respawn_cli()
         return self
@@ -268,23 +364,18 @@
                                       **kw)
 
     def new_session(
             self, messages: Iterable[Message] = tuple()) -> Session:
         return Session(bot=self, messages=list(messages))
 
     async def stream_raw(self,
-                         prompt: Prompt,
-                         role: Role = Role.User,
+                         session: Session,
                          ensure_json: bool = False,
                          choices: int = 1,
-                         session: Session | None = None
                          ) -> AsyncGenerator[FullChunkResponse, None]:
-        session = self.new_session() if session is None else session
-        session.append(Message(
-            role=role.value, content=await self._proc_prompt(prompt)))
         used_tokens = session.trim(bot=self)
 
         async with self._cli.stream(
             "POST",
             self.api_url,
             headers={"Authorization": "Bearer " + self.api_key},
             json=self._get_json(
@@ -320,43 +411,62 @@
         - `prompt` (str): What to say
         - `role` (Role): Role of the speaker
         - `ensure_json` (bool): Ensure the response is a valid JSON object
         - `session` (Session): Session to use
         """
 
         content = ''
-        async for r in self.stream_raw(prompt, role, ensure_json, 1, session):
-            choice = r.choices[0]
-            if choice.finish_reason is not None:
+        session = self.new_session() if session is None else session
+        session.append(Message(
+            role=role.value, content=await self._proc_prompt(prompt)))
+        tool_calls: None | list[dict[str, Any]] = None
+        choice: None | FullChunkResponse.Choice = None
+        while True:
+            async for r in self.stream_raw(session, ensure_json, 1):
+                choice = r.choices[0]
+                if choice.delta.tool_calls is not None:
+                    for i, tc in enumerate(choice.delta.tool_calls):
+                        if tool_calls is None:
+                            tool_calls = []
+                        if len(tool_calls) <= i:
+                            if tc["type"] != "function":
+                                continue
+                            tool_calls.append(tc)
+                        tool_calls[i]["function"]["arguments"] += tc["function"]["arguments"]
+                if choice.delta.role is not None:
+                    role = choice.delta.role
+                if choice.delta.content is not None:
+                    content += choice.delta.content
+                    yield choice.delta.content
+            session.append(
+                Message(role=role.value, content=content, tool_calls=tool_calls))
+            if choice is not None and choice.finish_reason == "tool_calls":
+                rets = await self._proc_toolcalls(tool_calls or [])
+                for fname, id_, ret in rets:
+                    session.append(Message(
+                        role=Role.Tool.value,
+                        name=fname,
+                        content=await self._proc_prompt(str(ret)),
+                        tool_call_id=id_)
+                    )
                 continue
-            if choice.delta.role is not None:
-                role = choice.delta.role
-            if choice.delta.content is not None:
-                content += choice.delta.content
-                yield choice.delta.content
-        if session is not None:
-            session.append(Message(role=role.value, content=content))
+            break
 
     def stream_sync(self,
                     prompt: Prompt,
                     role: Role = Role.User,
                     ensure_json: bool = False,
                     ) -> Generator[str, None, None]:
         raise NotImplementedError
 
     async def send_raw(self,
-                       prompt: Prompt,
-                       role: Role = Role.User,
+                       session: Session,
                        ensure_json: bool = False,
                        choices: int = 1,
-                       session: Session | None = None
                        ) -> FullResponse:
-        session = self.new_session() if session is None else session
-        session.append(Message(
-            role=role.value, content=await self._proc_prompt(prompt)))
         used_tokens = session.trim(bot=self)
 
         r = await self._cli.post(
             self.api_url,
             headers={"Authorization": "Bearer " + self.api_key},
             json=self._get_json(
                 session,
@@ -380,19 +490,35 @@
 
         ## Parameters
         - `prompt` (str): What to say
         - `role` (Role): Role of the speaker
         - `ensure_json` (bool): Ensure the response is a valid JSON object
         - `session` (Session): Session to use
         """
-        r = await self.send_raw(prompt, role, ensure_json, 1, session)
-        content = cast(str, r.choices[0].message.content)
-        if session is not None:
-            session.append(Message(role=role.value, content=content))
-        return content
+        session = self.new_session() if session is None else session
+        session.append(Message(
+            role=role.value, content=await self._proc_prompt(prompt)))
+        while True:
+            r = await self.send_raw(session, ensure_json, 1)
+            choice = r.choices[0]
+            message = choice.message
+            content = cast(str, choice.message.content)
+            session.append(Message(
+                role=message.role.value, content=content, tool_calls=message.tool_calls))
+            if choice.finish_reason == "tool_calls":
+                rets = await self._proc_toolcalls(message.tool_calls or [])
+                for fname, id_, ret in rets:
+                    session.append(Message(
+                        role=Role.Tool.value,
+                        name=fname,
+                        content=await self._proc_prompt(str(ret)),
+                        tool_call_id=id_)
+                    )
+                continue
+            return content
 
     def send_sync(self,
                   prompt: str,
                   role: Role = Role.User,
                   ensure_json: bool = False,
                   ) -> str | list[SegTypes]:
         """
@@ -492,16 +618,17 @@
                 elif isinstance(v, list | tuple):
                     for i in v:
                         if isinstance(i, dict):
                             remove_null(i)
 
         remove_null(ret)
 
-        if self.tools is not None:
-            ret["tools"] = self.tools
+        tools = self.tools
+        if tools is not None:
+            ret["tools"] = tools
             ret["tool_choice"] = self.tool_choice
 
         if (ensure_json):
             ret["response_format"] = {
                 "type": "json_object"
             }
 
@@ -514,14 +641,40 @@
         for seg in prompt:
             if isinstance(seg, Message.ImageSegment):
                 await self.cache_image_seg(seg)
             ret.append(seg)
 
         return ret
 
+    async def _proc_toolcalls(self, tool_calls: list[dict[str, Any]]) -> list[tuple[str, str, Any]]:
+        ret = list[tuple[str, str, Any]]()
+        func_map = {f.__name__: f for f in self.funcs}
+        async_funcs = list[Any]()
+
+        async def wrap(id_, afunc, kw):
+            return afunc.__name__, id_, (await afunc(**kw))
+        for tc in tool_calls:
+            if tc["type"] != "function":
+                continue
+            f = func_map.get(tc["function"]["name"])
+            if f is None:
+                raise ValueError(f"Function not found: {tc["function"]["name"]}")
+            try:
+                args = json.loads(tc["function"]["arguments"])
+            except json.JSONDecodeError:
+                raise RuntimeError(f"GPT returned invalid JSON for tool calls: {
+                                   tc["function"]["arguments"]}")
+            if inspect.iscoroutinefunction(f):
+                async_funcs.append(wrap(tc["id"], f, args))
+            else:
+                ret.append((f.__name__, tc["id"], f(**args)))
+        if async_funcs:
+            ret.extend(await asyncio.gather(*async_funcs))
+        return ret
+
 
 class Session(BaseModel, Sequence[Message]):
     model_config = ConfigDict(validate_assignment=True)
     bot: Bot | None = Field(exclude=True)
     messages: list[Message] = Field(default_factory=list)
 
     def trim(self, target_max: int | None = None, bot: Bot | None = None) -> int:
@@ -569,15 +722,16 @@
         msg_cnt = 0
         for message in reversed(self.messages):
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
             this_tokens = 4
             if message.name is not None:
                 this_tokens -= 1
             this_tokens += sizeof_prompt(message.role)
-            this_tokens += sizeof_prompt(message.content)
+            this_tokens += sizeof_prompt(message.content or '')
+            this_tokens += sizeof_prompt(json.dumps(message.tool_calls or []))
             if num_tokens + this_tokens >= target_max:
                 break
             msg_cnt += 1
             num_tokens += this_tokens
         self.messages = self.messages[len(self.messages)-msg_cnt:]
         return num_tokens
```

### Comparing `ngptbot-0.3.4/pyproject.toml` & `ngptbot-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ngptbot"
-version = "0.3.4"
+version = "0.3.5"
 description = "Wrapper for ChatGPT API"
 authors = ["VermiIIi0n <dungeon.behind0t@icloud.com>"]
 readme = "README.md"
 packages = [{ include = "gptbot" }]
 license = "MIT"
 homepage = "https://github.com/VermiIIi0n/GPTBot"
```

### Comparing `ngptbot-0.3.4/PKG-INFO` & `ngptbot-0.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngptbot
-Version: 0.3.4
+Version: 0.3.5
 Summary: Wrapper for ChatGPT API
 Home-page: https://github.com/VermiIIi0n/GPTBot
 License: MIT
 Keywords: utilities
 Author: VermiIIi0n
 Author-email: dungeon.behind0t@icloud.com
 Requires-Python: >=3.12,<4.0
@@ -28,20 +28,30 @@
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Requires-Dist: vermils (>=0.3.4,<0.4.0)
 Project-URL: Issues, https://github.com/VermiIIi0n/GPTBot/issues
 Description-Content-Type: text/markdown
 
 # Simple Wrapper For The ChatGPT API
 
-This module is designed for asynchronous usage and provides a simple interface to the OpenAI ChatGPT API.
+This module is designed for asynchronous usage and provides a simple interface to the OpenAI ChatGPT API
 
 It also provides a command-line interface for interactive usage.
 
 While it does provide synchronous methods, it is recommended to use the asynchronous methods for better performance.
 
+## Features
+
+- Asynchronous API
+- Get/Stream responses
+- Save/Load session history
+- Change parameters on the fly
+- Embed images in messages
+- Register functions to `tool_calls` with ease
+- Interactive command-line interface
+
 ## Installation
 
 ```bash
 pip install -U ngptbot
 ```
 
 ## Usage
@@ -133,7 +143,18 @@
         print(r, end='')
 
     print(await session.send("Goodbye!"))
 
 asyncio.run(main())
 ```
 
+### Registering Functions
+
+Functions are under `Bot.funcs` and can be registered with the `add_func` decorator.
+
+```python
+@bot.add_func
+def my_func(data: str, default:int = 123):  # parameters must be annotated, variadic parameters are not supported
+    """Documentation goes here"""
+    return data  # return value must be stringifiable
+```
+
```

