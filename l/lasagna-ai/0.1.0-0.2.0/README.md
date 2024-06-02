# Comparing `tmp/lasagna_ai-0.1.0.tar.gz` & `tmp/lasagna_ai-0.2.0.tar.gz`

## Comparing `lasagna_ai-0.1.0.tar` & `lasagna_ai-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/__init__.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/agent_runner.py
--rw-r--r--   0        0        0    18142 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/lasagna_openai.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/registrar.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/stream.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/types.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/src/lasagna/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_agent_runner.py
--rw-r--r--   0        0        0    38083 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_lasagna_openai.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_registrar.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_stream.py
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/tests/test_util.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/README.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 lasagna_ai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/Makefile
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0    27615 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/logos/lasagna-ai.png
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/__init__.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/agent_runner.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/known_providers.py
+-rw-r--r--   0        0        0    18287 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/lasagna_openai.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/registrar.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/stream.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/types.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/src/lasagna/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/tests/test_agent_runner.py
+-rw-r--r--   0        0        0    37960 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/tests/test_lasagna_openai.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/tests/test_registrar.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/tests/test_stream.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/tests/test_util.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/README.md
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 lasagna_ai-0.2.0/PKG-INFO
```

### Comparing `lasagna_ai-0.1.0/.github/workflows/publish.yml` & `lasagna_ai-0.2.0/.github/workflows/publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -13,24 +13,23 @@
     name: Publish to PyPI
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Install Hatch
-      run: |
-        pip install --upgrade hatch
+      uses: pypa/hatch@install
 
     - name: Check type correctness
       run: |
-        hatch run types:check
+        make checkall
 
     - name: Run tests
       run: |
-        hatch test --all --cover --randomize
+        make testall
 
     - name: Build
       run: hatch build
 
     - name: Publish
       env:
         HATCH_INDEX_USER: ${{ secrets.HATCH_INDEX_USER }}
```

### Comparing `lasagna_ai-0.1.0/src/lasagna/agent_runner.py` & `lasagna_ai-0.2.0/src/lasagna/agent_runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,64 @@
-from .registrar import AGENTS, MODEL_PROVIDERS
+from .registrar import AGENTS, PROVIDERS
 
 from .types import (
     AgentSpec,
+    AgentRun,
     AgentCallable,
-    ProviderFactory,
-    ChatMessage,
+    ModelFactory,
     EventCallback,
 )
 
+from .known_providers import attempt_load_known_providers
+
 from typing import List
 
 
 async def run(
     agent_spec: AgentSpec,
     event_callback: EventCallback,
-    messages: List[ChatMessage],
-) -> List[ChatMessage]:
+    prev_runs: List[AgentRun],
+) -> AgentRun:
     agent: AgentCallable
+    agent_name: str
     if isinstance(agent_spec['agent'], str):
-        agent = AGENTS[agent_spec['agent']]['runner']
+        agent_name = agent_spec['agent']
+        agent = AGENTS[agent_name]['runner']
     else:
         agent = agent_spec['agent']
+        agent_name = agent.__name__
 
-    provider: ProviderFactory
-    if isinstance(agent_spec['provider'], str):
-        provider = MODEL_PROVIDERS[agent_spec['provider']]['factory']
-    else:
-        provider = agent_spec['provider']
+    model_name = agent_spec['model']
 
-    kwargs = agent_spec.get('model_kwargs', None)
-    if kwargs is None:
-        kwargs = {}
+    model_kwargs = agent_spec.get('model_kwargs', None)
+    if model_kwargs is None:
+        model_kwargs = {}
 
-    llm = provider(model=agent_spec['model'], **kwargs)
+    model_factory: ModelFactory
+    provider_str: str
+    if isinstance(agent_spec['provider'], str):
+        provider_str = agent_spec['provider']
+        if provider_str not in PROVIDERS:
+            attempt_load_known_providers(provider_str)
+        model_factory = PROVIDERS[provider_str]['factory']
+        model = model_factory(model=model_name, **model_kwargs)
+    else:
+        model_factory = agent_spec['provider']
+        model = model_factory(model=model_name, **model_kwargs)
+        provider_str = model.__class__.__name__
 
-    return await agent(
-        llm,
+    agent_run = await agent(
+        model,
         event_callback,
-        messages,
+        prev_runs,
     )
+
+    if 'agent' not in agent_run:
+        agent_run['agent'] = agent_name
+    if 'provider' not in agent_run:
+        agent_run['provider'] = provider_str
+    if 'model' not in agent_run:
+        agent_run['model'] = model_name
+    if 'model_kwargs' not in agent_run and 'model_kwargs' in agent_spec:
+        agent_run['model_kwargs'] = model_kwargs
+
+    return agent_run
```

### Comparing `lasagna_ai-0.1.0/src/lasagna/lasagna_openai.py` & `lasagna_ai-0.2.0/src/lasagna/lasagna_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .types import (
-    ChatMessage,
-    ChatMessageContent,
-    ChatMessageToolCall,
-    ChatMessageRole,
+    Message,
+    MessageContent,
+    MessageToolCall,
     EventCallback,
     EventPayload,
-    LLM,
+    Model,
     ToolCall,
     ToolParam,
     ToolResult,
     ModelRecord,
     Cost,
 )
 
@@ -21,16 +20,14 @@
 
 from .util import (
     parse_docstring,
     combine_pairs,
     convert_to_image_url,
 )
 
-from .registrar import register_model_provider
-
 from openai import AsyncOpenAI, NOT_GIVEN, NotGiven
 from openai.types.chat import (
     ChatCompletionChunk,
     ChatCompletionToolParam,
     ChatCompletionToolChoiceOptionParam,
     ChatCompletionMessageParam,
     ChatCompletionContentPartParam,
@@ -43,16 +40,20 @@
 )
 
 import asyncio
 import copy
 import json
 import inspect
 
+import logging
+
+_LOG = logging.getLogger(__name__)
 
-_KNOWN_MODELS: List[ModelRecord] = [
+
+OPENAI_KNOWN_MODELS: List[ModelRecord] = [
     {
         'formal_name': 'gpt-4o-2024-05-13',
         'display_name': 'GPT-4o',
     },
     {
         'formal_name': 'gpt-4-turbo-2024-04-09',
         'display_name': 'GPT-4',
@@ -67,41 +68,41 @@
 async def _process_text_stream(
     stream: AsyncIterator[Tuple[ChoiceDelta, Union[str, None]]],
 ) -> AsyncIterator[EventPayload]:
     async for delta, finish_reason in stream:
         text = delta.content
         if finish_reason is not None:
             if text is not None:
-                yield ChatMessageRole.AI, 'text', str(text)
+                yield 'ai', 'text_event', str(text)
             return
         if text is None:
             # The model is switching from text to tools!
-            yield ChatMessageRole.AI, 'text', "\n\n"
+            yield 'ai', 'text_event', "\n\n"
             put_back_val: Tuple[ChoiceDelta, Union[str, None]] = (delta, finish_reason)
             fixed_stream = prefix_stream([put_back_val], stream)
             substream = _process_tool_call_stream(fixed_stream)
             async for subval in substream:
                 yield subval
             return
-        yield ChatMessageRole.AI, 'text', str(text)
+        yield 'ai', 'text_event', str(text)
 
 
 async def _process_tool_call_stream(
     stream: AsyncIterator[Tuple[ChoiceDelta, Union[str, None]]],
 ) -> AsyncIterator[EventPayload]:
     recs_by_index: Dict[int, ToolCall] = {}
     args_by_index: Dict[int, List[str]] = {}
     last_index: Optional[int] = None
     async for delta, _ in stream:
         if not delta.tool_calls:
             continue
         for tc in delta.tool_calls:
             index = tc.index
             if index != last_index and last_index is not None:
-                yield ChatMessageRole.TOOL_CALL, 'text', ")\n"   # <-- again, assumes no index-interleave
+                yield 'tool_call', 'text_event', ")\n"   # <-- again, assumes no index-interleave
             last_index = index
             if index not in recs_by_index:
                 assert tc.type == 'function', f"The only tool type we can do is a function! But got: {tc.type}"
                 assert tc.function
                 assert tc.function.name
                 assert tc.id
                 n: str = tc.function.name
@@ -111,30 +112,30 @@
                     'call_type': 'function',
                     'function': {
                         'name': n,
                         'arguments': '',  # will be filled in at the end
                     },
                 }
                 args_by_index[index] = [a]
-                yield ChatMessageRole.TOOL_CALL, 'text', f"{n}("   # <-- assumes no index-interleave
+                yield 'tool_call', 'text_event', f"{n}("   # <-- assumes no index-interleave
             else:
                 # assumes nothing but the argument is in the delta message...
                 args = args_by_index[index]
                 assert tc.function
                 assert tc.function.arguments
                 assert not tc.function.name
                 a_delta: str = tc.function.arguments
                 args.append(a_delta)
-                yield ChatMessageRole.TOOL_CALL, 'text', a_delta
+                yield 'tool_call', 'text_event', a_delta
     if last_index is not None:
-        yield ChatMessageRole.TOOL_CALL, 'text', ")"   # <-- again, assumes no index-interleave
+        yield 'tool_call', 'text_event', ")"   # <-- again, assumes no index-interleave
     for index in sorted(recs_by_index.keys()):
         rec = recs_by_index[index]
         rec['function']['arguments'] = ''.join(args_by_index[index])
-        yield ChatMessageRole.TOOL_CALL, 'tool_call', rec
+        yield 'tool_call', 'tool_call_event', rec
 
 
 async def _process_output_stream(
     stream: AsyncIterator[Tuple[ChoiceDelta, Union[str, None]]],
 ) -> AsyncIterator[EventPayload]:
     first, stream = await apeek(stream, n=1)
     first_delta, _ = first[0]
@@ -147,14 +148,18 @@
         yield v
 
 
 async def _extract_deltas(
     stream: AsyncIterator[ChatCompletionChunk],
 ) -> AsyncIterator[Tuple[ChoiceDelta, Union[str, None]]]:
     async for v in stream:
+        if len(v.choices) == 0:
+            # The final message that has the `usage` has zero choices.
+            # So just skip it here!
+            continue
         assert len(v.choices) == 1, f"Why do we have {len(v.choices)} choices?"
         single_choice = v.choices[0]
         yield single_choice.delta, single_choice.finish_reason
 
 
 def _convert_to_json_schema(params: List[ToolParam]) -> Dict[str, object]:
     def convert_type(t: str) -> Dict[str, object]:
@@ -205,23 +210,23 @@
     if len(tools) == 0:
         return NOT_GIVEN
     specs = [_convert_to_openai_tool(tool) for tool in tools]
     return specs
 
 
 async def _make_openai_content(
-    message: ChatMessageContent,
+    message: MessageContent,
 ) -> List[ChatCompletionContentPartParam]:
     ret: List[ChatCompletionContentPartParam] = []
     if message['text']:
         ret.append({
             'type': 'text',
             'text': message['text'],
         })
-    if message['media']:
+    if 'media' in message:
         for m in message['media']:
             if m['media_type'] == 'image':
                 ret.append({
                     'type': 'image_url',
                     'image_url': {
                         'url': (await convert_to_image_url(m['image'])),
                     },
@@ -229,18 +234,18 @@
             else:
                 raise ValueError(f"unknown media type: {m['media_type']}")
     if len(ret) == 0:
         raise ValueError('no content in this message!')
     return ret
 
 
-async def _convert_to_openai_messages(messages: List[ChatMessage]) -> List[ChatCompletionMessageParam]:
+async def _convert_to_openai_messages(messages: List[Message]) -> List[ChatCompletionMessageParam]:
     ms: List[ChatCompletionMessageParam] = []
     for m in messages:
-        if m['role'] == ChatMessageRole.TOOL_CALL:
+        if m['role'] == 'tool_call':
             tool_calls = m['tools']
             ms.append({
                 'role': 'assistant',
                 'content': None,
                 'tool_calls': [
                     {
                         'id': t['call_id'],
@@ -249,36 +254,36 @@
                             'name': t['function']['name'],
                             'arguments': t['function']['arguments'],
                         },
                     }
                     for t in tool_calls
                 ],
             })
-        elif m['role'] == ChatMessageRole.TOOL_RES:
+        elif m['role'] == 'tool_res':
             tool_results = m['tools']
             for t in tool_results:
                 ms.append({
                     'role': 'tool',
                     'content': str(t['result']),
                     'tool_call_id': t['call_id'],
                 })
-        elif m['role'] == ChatMessageRole.SYSTEM:
-            if m['media']:
+        elif m['role'] == 'system':
+            if 'media' in m and len(m['media']) > 0:
                 raise ValueError('This model does not support media in the system prompt.')
             ms.append({
                 'role': 'system',
                 'content': m['text'] or '',
             })
-        elif m['role'] == ChatMessageRole.HUMAN:
+        elif m['role'] == 'human':
             ms.append({
                 'role': 'user',
                 'content': (await _make_openai_content(m)),
             })
-        elif m['role'] == ChatMessageRole.AI:
-            if m['media']:
+        elif m['role'] == 'ai':
+            if 'media' in m and len(m['media']) > 0:
                 raise ValueError('This model does not support media in AI messages.')
             ms.append({
                 'role': 'assistant',
                 'content': m['text'],
             })
         else:
             raise ValueError(f"unknown message role: {m['role']}")
@@ -286,16 +291,16 @@
         m1: ChatCompletionMessageParam,
         m2: ChatCompletionMessageParam,
     ) -> Union[Literal[False], Tuple[Literal[True], ChatCompletionMessageParam]]:
         if m1['role'] == 'assistant' and m2['role'] == 'assistant':
             # This is the case where the model started with text and switched
             # to tool-calling part-way-through. We need to combine these
             # messages.
-            assert m1.get('content') and not m1.get('tool_calls')
-            assert not m2.get('content') and m2.get('tool_calls')
+            assert ('content' in m1 and m1['content']) and ('tool_calls' not in m1 or not m1['tool_calls'])
+            assert ('content' not in m2 or not m2['content']) and ('tool_calls' in m2 and m2['tool_calls'])
             m_combined: ChatCompletionMessageParam = {
                 'role': 'assistant',
                 'content': m1['content'],
                 'tool_calls': m2['tool_calls'],
             }
             return True, m_combined
         return False
@@ -309,50 +314,48 @@
     if not usages:
         return None
     usage = usages[-1]
     return {
         'input_tokens': usage.prompt_tokens,
         'output_tokens': usage.completion_tokens,
         'total_tokens': usage.total_tokens,
-        'cost_usd_cents': None,   # API doesn't give this, unfortunately
     }
 
 
 def _build_messages_from_openai_payload(
     payload: List[ChatCompletionChunk],
     events: List[EventPayload],
-) -> List[ChatMessage]:
+) -> List[Message]:
     """
     We either have:
      - all AI events
      - all TOOL_CALL events
      - some AI events then it switches to TOOL_CALL events
     """
     cost = _get_cost(payload)
     raw = [p.to_dict() for p in payload]
     ai_events = [
         event
         for event in events
-        if event[0] == ChatMessageRole.AI
+        if event[0] == 'ai'
     ]
     tool_events = [
         event
         for event in events
-        if event[0] == ChatMessageRole.TOOL_CALL
+        if event[0] == 'tool_call'
     ]
-    ai_message: Optional[ChatMessage] = {
-        'role': ChatMessageRole.AI,
-        'text': ''.join([e[2] for e in ai_events if e[1] == 'text']),
-        'media': None, # <-- the chat API doesn't know how to generate images (it only _reads_ images)
+    ai_message: Optional[Message] = {
+        'role': 'ai',
+        'text': ''.join([e[2] for e in ai_events if e[1] == 'text_event']),
         'cost': cost,
         'raw': raw,
     } if len(ai_events) > 0 else None
-    tool_message: Optional[ChatMessageToolCall] = {
-        'role': ChatMessageRole.TOOL_CALL,
-        'tools': [e[2] for e in tool_events if e[1] == 'tool_call'],
+    tool_message: Optional[MessageToolCall] = {
+        'role': 'tool_call',
+        'tools': [e[2] for e in tool_events if e[1] == 'tool_call_event'],
         'cost': cost,
         'raw': raw,
     } if len(tool_events) > 0 else None
     if ai_message and tool_message:
         ai_message['cost'] = None  # <-- we don't want to double-count this
         ai_message['raw'] = None
         return [ai_message, tool_message]
@@ -361,20 +364,20 @@
     elif tool_message:
         return [tool_message]
     else:
         raise ValueError('no events')
 
 
 async def _handle_tools(
-    messages: List[ChatMessage],
+    messages: List[Message],
     tools_map: Dict[str, Callable],
 ) -> Union[List[ToolResult], None]:
     assert len(messages) > 0
     message = messages[-1]   # <-- the tool message will be last, if at all
-    if message['role'] != ChatMessageRole.TOOL_CALL:
+    if message['role'] != 'tool_call':
         return None
     to_gather: List[asyncio.Task[ToolResult]] = []
     for t in message['tools']:
         assert t['call_type'] == 'function'
         async def _go(t: ToolCall) -> ToolResult:
             call_id = 'unknown'
             try:
@@ -392,63 +395,74 @@
             except Exception as e:
                 error = f"{type(e).__name__}: {e}"
                 return {'call_id': call_id, 'result': error}
         to_gather.append(asyncio.create_task(_go(t)))
     return await asyncio.gather(*to_gather)
 
 
-def _build_tool_response_message(tool_results: List[ToolResult]) -> ChatMessage:
+def _build_tool_response_message(tool_results: List[ToolResult]) -> Message:
     return {
-        'role': ChatMessageRole.TOOL_RES,
+        'role': 'tool_res',
         'tools': tool_results,
         'cost': None,
         'raw': None,
     }
 
 
-class LasagnaOpenAI(LLM):
+def _log_dumps(val: Any) -> str:
+    if isinstance(val, dict):
+        return json.dumps(val)
+    else:
+        return str(val)
+
+
+class LasagnaOpenAI(Model):
     def __init__(self, model: str, **model_kwargs: Dict[str, Any]):
-        known_model_names = [m['formal_name'] for m in _KNOWN_MODELS]
+        known_model_names = [m['formal_name'] for m in OPENAI_KNOWN_MODELS]
         if model not in known_model_names:
             raise ValueError(f'unknown model: {model}')
         self.model = model
         self.model_kwargs = copy.deepcopy(model_kwargs or {})
         self.client = AsyncOpenAI()
 
     async def _run_once(
         self,
         event_callback: EventCallback,
-        messages: List[ChatMessage],
+        messages: List[Message],
         tools: List[Callable],
         force_tool: bool = False,
-    ) -> List[ChatMessage]:
+    ) -> List[Message]:
         tool_choice: Union[ChatCompletionToolChoiceOptionParam, NotGiven]
         if force_tool:
             if len(tools) != 1:
                 raise ValueError(f"When `force_tool` is set, you must pass exactly one tool, not {len(tools)}.")
             tool_choice = {
                 "type": "function",
                 "function": {"name": tools[0].__name__},
             }
         else:
             tool_choice = NOT_GIVEN
 
         tools_spec = _convert_to_openai_tools(tools)
 
+        openai_messages = await _convert_to_openai_messages(messages)
+
         frequency_penalty: Union[float, NotGiven] = cast(float, self.model_kwargs['frequency_penalty']) if 'frequency_penalty' in self.model_kwargs else NOT_GIVEN
         presence_penalty: Union[float, NotGiven] = cast(float, self.model_kwargs['presence_penalty']) if 'presence_penalty' in self.model_kwargs else NOT_GIVEN
         max_tokens: Union[int, NotGiven] = cast(int, self.model_kwargs['max_tokens']) if 'max_tokens' in self.model_kwargs else NOT_GIVEN
         stop: Union[List[str], NotGiven] = cast(List[str], self.model_kwargs['stop']) if 'stop' in self.model_kwargs else NOT_GIVEN
         temperature: Union[float, NotGiven] = cast(float, self.model_kwargs['temperature']) if 'temperature' in self.model_kwargs else NOT_GIVEN
         top_p: Union[float, NotGiven] = cast(float, self.model_kwargs['top_p']) if 'top_p' in self.model_kwargs else NOT_GIVEN
         user: Union[str, NotGiven] = cast(str, self.model_kwargs['user']) if 'user' in self.model_kwargs else NOT_GIVEN
 
+        _LOG.info(f"Invoking {self.model} with:\n  messages: {_log_dumps(openai_messages)}\n  tools: {_log_dumps(tools_spec)}\n  tool_choice: {tool_choice}")
+
         completion: AsyncIterator[ChatCompletionChunk] = await self.client.chat.completions.create(
             model        = self.model,
-            messages     = (await _convert_to_openai_messages(messages)),
+            messages     = openai_messages,
             tools        = tools_spec,
             tool_choice  = tool_choice,
             stream       = True,
             stream_options = {'include_usage': True},
             logprobs     = True,
             top_logprobs = 20,
             frequency_penalty = frequency_penalty,
@@ -468,46 +482,40 @@
             events.append(event)
             await event_callback(event)
 
         raw_payload = [v async for v in raw_stream]
 
         new_messages = _build_messages_from_openai_payload(raw_payload, events)
 
+        _LOG.info(f"Finished {self.model} with usage: {_log_dumps(new_messages[-1]['cost'])}")
+
         return new_messages
 
     async def run(
         self,
         event_callback: EventCallback,
-        messages: List[ChatMessage],
+        messages: List[Message],
         tools: List[Callable],
         force_tool: bool = False,
         max_tool_iters: int = 5,
-    ) -> List[ChatMessage]:
+    ) -> List[Message]:
         messages = [*messages]  # shallow copy
-        new_messages: List[ChatMessage] = []
+        new_messages: List[Message] = []
         for _ in range(max_tool_iters):
             new_messages_here = await self._run_once(
                 event_callback = event_callback,
                 messages       = messages,
                 tools          = tools,
                 force_tool     = force_tool,
             )
             tools_map = {tool.__name__: tool for tool in tools}
             new_messages.extend(new_messages_here)
             messages.extend(new_messages_here)
             tools_results = await _handle_tools(new_messages_here, tools_map)
             if tools_results is None:
                 break
             for tool_result in tools_results:
-                await event_callback((ChatMessageRole.TOOL_RES, 'tool_res', tool_result))
+                await event_callback(('tool_res', 'tool_res_event', tool_result))
             tool_response_message = _build_tool_response_message(tools_results)
             new_messages.append(tool_response_message)
             messages.append(tool_response_message)
         return new_messages
-
-
-register_model_provider(
-    key  = 'openai',
-    name = 'OpenAI',
-    factory = LasagnaOpenAI,
-    models = _KNOWN_MODELS,
-)
```

### Comparing `lasagna_ai-0.1.0/src/lasagna/registrar.py` & `lasagna_ai-0.2.0/src/lasagna/registrar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from .types import (
     AgentRecord,
     AgentCallable,
-    ModelProviderRecord,
-    ProviderFactory,
+    ProviderRecord,
+    ModelFactory,
     ModelRecord,
 )
 
 from typing import Dict, List
 
 
 AGENTS: Dict[str, AgentRecord] = {}
 
-MODEL_PROVIDERS: Dict[str, ModelProviderRecord] = {}
+PROVIDERS: Dict[str, ProviderRecord] = {}
 
 
 def register_agent(
     key: str,
     name: str,
     runner: AgentCallable,
 ) -> None:
@@ -23,20 +23,20 @@
         raise RuntimeError(f"An agent with this key is already registered: {key}")
     AGENTS[key] = {
         'name': name,
         'runner': runner,
     }
 
 
-def register_model_provider(
+def register_provider(
     key: str,
     name: str,
-    factory: ProviderFactory,
+    factory: ModelFactory,
     models: List[ModelRecord],
 ) -> None:
-    if key in MODEL_PROVIDERS:
+    if key in PROVIDERS:
         raise RuntimeError(f"A model provider with this key is already registered: {key}")
-    MODEL_PROVIDERS[key] = {
+    PROVIDERS[key] = {
         'name': name,
         'factory': factory,
         'models': models,
     }
```

### Comparing `lasagna_ai-0.1.0/src/lasagna/stream.py` & `lasagna_ai-0.2.0/src/lasagna/stream.py`

 * *Files identical despite different names*

### Comparing `lasagna_ai-0.1.0/src/lasagna/types.py` & `lasagna_ai-0.2.0/src/lasagna/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,16 @@
+from __future__ import annotations
 import abc
 
-from enum import Enum
-
 from typing import (
     TypedDict, Dict, List, Any, Optional, Literal,
     Callable, Tuple, Awaitable, Union, Protocol,
 )
 
-
-class ChatMessageRole(Enum):
-    SYSTEM    = "system"
-    HUMAN     = "human"
-    AI        = "ai"
-    TOOL_CALL = "tool_call"
-    TOOL_RES  = "tool_res"
+from typing_extensions import NotRequired
 
 
 class ToolCallFunction(TypedDict):
     name: str
     arguments: str   # <-- JSON-encoded arguments (kept as a string for reproducibility reasons)
 
 
@@ -32,111 +25,141 @@
     result: Any
 
 
 class Cost(TypedDict):
     input_tokens: Optional[int]
     output_tokens: Optional[int]
     total_tokens: Optional[int]
-    cost_usd_cents: Optional[int]
 
 
 class MediaImage(TypedDict):
     media_type: Literal['image']
     image: str   # <-- either a local filepath or a remote URL
 
 
 Media = MediaImage   # note: this will become a Union[MediaImage, ...] in the future as needed
 
 
-class ChatMessageBase(TypedDict):
+class MessageBase(TypedDict):
     cost: Optional[Cost]   # <-- cost of generating this message (for messages generated by an external service)
     raw: Any               # <-- the raw payload(s) from the API (before being converted our our schema; only for messages generated by an external service)
 
 
-class ChatMessageContent(ChatMessageBase):
-    role: Literal[ChatMessageRole.SYSTEM, ChatMessageRole.HUMAN, ChatMessageRole.AI]
+class MessageContent(MessageBase):
+    role: Literal['system', 'human', 'ai']
     text: Optional[str]
-    media: Optional[List[Media]]
+    media: NotRequired[List[Media]]
 
 
-class ChatMessageToolCall(ChatMessageBase):
-    role: Literal[ChatMessageRole.TOOL_CALL]
+class MessageToolCall(MessageBase):
+    role: Literal['tool_call']
     tools: List[ToolCall]
 
 
-class ChatMessageToolResult(ChatMessageBase):
-    role: Literal[ChatMessageRole.TOOL_RES]
+class MessageToolResult(MessageBase):
+    role: Literal['tool_res']
     tools: List[ToolResult]
 
 
-ChatMessage = Union[ChatMessageContent, ChatMessageToolCall, ChatMessageToolResult]
+Message = Union[MessageContent, MessageToolCall, MessageToolResult]
 
 
 EventPayload = Union[
-    Tuple[Literal[ChatMessageRole.AI], Literal['text'], str],
-    Tuple[Literal[ChatMessageRole.TOOL_CALL], Literal['text'], str],
-    Tuple[Literal[ChatMessageRole.TOOL_CALL], Literal['tool_call'], ToolCall],
-    Tuple[Literal[ChatMessageRole.TOOL_RES], Literal['tool_res'], ToolResult],
+    Tuple[Literal['ai'],        Literal['text_event'],      str],
+    Tuple[Literal['tool_call'], Literal['text_event'],      str],
+    Tuple[Literal['tool_call'], Literal['tool_call_event'], ToolCall],
+    Tuple[Literal['tool_res'],  Literal['tool_res_event'],  ToolResult],
+    Tuple[Literal['progress'],  Literal['start'],           Tuple[str, str]],    # payload is `(key, details)`
+    Tuple[Literal['progress'],  Literal['update'],          Tuple[str, float]],  # payload is `(key, progress_0_to_1)`
+    Tuple[Literal['progress'],  Literal['end'],             str],                # payload is `key`
 ]
 
 
 EventCallback = Callable[[EventPayload], Awaitable[None]]
 
 
-class LLM(abc.ABC):
+class Model(abc.ABC):
     """
-    Interface for all Large Language Models (LLMs).
+    Interface for an AI model.
+
+    In many cases this will be an LLM (when you're in pure-text use-cases). But
+    this interface also supports AI models that operate on multimodal content,
+    thus we'll use the phrase "AI model" to be more general.
     """
 
     @abc.abstractmethod
     async def run(
         self,
         event_callback: EventCallback,
-        messages: List[ChatMessage],
+        messages: List[Message],
         tools: List[Callable],
         force_tool: bool = False,
         max_tool_iters: int = 5,
-    ) -> List[ChatMessage]:
+    ) -> List[Message]:
         """
         Generate one-or-more responses from the AI. More than one response
         is generated when tools are used. This method will respond to tool-
         use requests until the AI generates a non-tool response (up to
         `max_tool_iters`, then it halts).
         """
         pass
 
 
-AgentCallable = Callable[[LLM, EventCallback, List[ChatMessage]], Awaitable[List[ChatMessage]]]
+class AgentRunBase(TypedDict):
+    agent: NotRequired[str]
+    provider: NotRequired[str]
+    model: NotRequired[str]
+    model_kwargs: NotRequired[Dict[str, Any]]
+
+
+class AgentRunMessageList(AgentRunBase):
+    type: Literal['messages']
+    messages: List[Message]
+
+
+class AgentRunParallel(AgentRunBase):
+    type: Literal['parallel']
+    runs: List[AgentRun]
+
+
+class AgentRunChained(AgentRunBase):
+    type: Literal['chain']
+    runs: List[AgentRun]
+
+
+AgentRun = Union[AgentRunMessageList, AgentRunParallel, AgentRunChained]
+
+
+AgentCallable = Callable[[Model, EventCallback, List[AgentRun]], Awaitable[AgentRun]]
 
 
 class AgentRecord(TypedDict):
     name: str
     runner: AgentCallable
 
 
 class ModelRecord(TypedDict):
     formal_name: str
     display_name: str
 
 
-class ProviderFactory(Protocol):
-    def __call__(self, model: str, **model_kwargs: Dict[str, Any]) -> LLM: ...
+class ModelFactory(Protocol):
+    def __call__(self, model: str, **model_kwargs: Dict[str, Any]) -> Model: ...
 
 
-class ModelProviderRecord(TypedDict):
+class ProviderRecord(TypedDict):
     name: str
-    factory: ProviderFactory
+    factory: ModelFactory
     models: List[ModelRecord]
 
 
 class AgentSpec(TypedDict):
     agent: Union[str, AgentCallable]
-    provider: Union[str, ProviderFactory]
+    provider: Union[str, ModelFactory]
     model: str
-    model_kwargs: Optional[Dict[str, Any]]
-    # TODO: make it hierarchical!
+    model_kwargs: NotRequired[Dict[str, Any]]
 
 
 class ToolParam(TypedDict):
     name: str
     type: str
     description: str
```

### Comparing `lasagna_ai-0.1.0/src/lasagna/util.py` & `lasagna_ai-0.2.0/src/lasagna/util.py`

 * *Files identical despite different names*

### Comparing `lasagna_ai-0.1.0/tests/test_lasagna_openai.py` & `lasagna_ai-0.2.0/tests/test_lasagna_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
 from lasagna.types import (
-    ChatMessage,
-    ChatMessageRole,
+    Message,
     ToolCall,
     ToolResult,
     EventPayload,
 )
 
 from lasagna.stream import fake_async
 
@@ -279,15 +278,24 @@
                     "logprobs": None
                 }
             ],
             "created": 1713739736,
             "model": "gpt-3.5-turbo-0125",
             "object": "chat.completion.chunk",
             "system_fingerprint": "fp_c2295e73ad"
-        }
+        },
+        {
+            'id': 'chatcmpl-9ViswdADZmieYlPfvYf7J2UgTgFC7',
+            'choices': [],
+            'created': 1717347734,
+            'model': 'gpt-3.5-turbo-0125',
+            'object': 'chat.completion.chunk',
+            'system_fingerprint': None,
+            'usage': {'completion_tokens': 22, 'prompt_tokens': 21, 'total_tokens': 43},
+        },
     ]
 ]
 
 
 SAMPLE_TOOL_STREAM: List[ChatCompletionChunk] = [
     ChatCompletionChunk.model_validate(v)
     for v in [
@@ -592,15 +600,15 @@
         "call_type": "function"
     }
 ]
 
 
 @pytest.mark.asyncio
 async def test_extract_deltas():
-    stream = fake_async(SAMPLE_TEXT_STREAM[:2] + SAMPLE_TEXT_STREAM[-1:])
+    stream = fake_async(SAMPLE_TEXT_STREAM[:2] + SAMPLE_TEXT_STREAM[-2:])
     vals = [(d.to_dict(), s) async for d, s in _extract_deltas(stream)]
     assert vals == [
         ({'content': '', 'role': 'assistant'}, None),
         ({'content': 'Hello'}, None),
         ({}, 'stop'),
     ]
 
@@ -619,71 +627,71 @@
 
 
 @pytest.mark.asyncio
 async def test_process_output_stream__text():
     stream = _process_output_stream(_extract_deltas(fake_async(SAMPLE_TEXT_STREAM)))
     texts: List[str] = []
     async for role, type_, text in stream:
-        assert role == ChatMessageRole.AI
-        assert type_ == 'text'
+        assert role == 'ai'
+        assert type_ == 'text_event'
         assert isinstance(text, str)
         texts.append(text)
     text = ''.join(texts)
     assert text == 'Hello Ryan! 5 multiplied by 7 is 35.'
 
 
 @pytest.mark.asyncio
 async def test_process_output_stream__tool():
     stream = _process_output_stream(_extract_deltas(fake_async(SAMPLE_TOOL_STREAM)))
     texts: List[str] = []
     tool_calls: List[ToolCall] = []
     async for event in stream:
-        assert event[0] == ChatMessageRole.TOOL_CALL
-        if event[1] == 'text':
+        assert event[0] == 'tool_call'
+        if event[1] == 'text_event':
             texts.append(event[2])
-        elif event[1] == 'tool_call':
+        elif event[1] == 'tool_call_event':
             tool_calls.append(event[2])
         else:
             assert False, event[1]
     text = ''.join(texts)
     assert text == 'multiply({"a": 5, "b": 7})\nmultiply({"a": 8, "b": 101})'
     assert tool_calls == CORRECT_PARSED_TOOLS
 
     stream = _process_output_stream(_extract_deltas(fake_async(SAMPLE_TOOL_STREAM[:6])))
     texts: List[str] = []
     tool_calls: List[ToolCall] = []
     async for event in stream:
-        assert event[0] == ChatMessageRole.TOOL_CALL
-        if event[1] == 'text':
+        assert event[0] == 'tool_call'
+        if event[1] == 'text_event':
             texts.append(event[2])
-        elif event[1] == 'tool_call':
+        elif event[1] == 'tool_call_event':
             tool_calls.append(event[2])
         else:
             assert False, event[1]
     text = ''.join(texts)
     assert text == 'multiply({"a": 5, "b": 7})'
     assert tool_calls == CORRECT_PARSED_TOOLS[:1]
 
 
 @pytest.mark.asyncio
 async def test_process_output_stream__text_and_tool():
     # The model can start with text and switch to tools!
     stream = _process_output_stream(_extract_deltas(fake_async(
-        SAMPLE_TEXT_STREAM[:-1] + SAMPLE_TOOL_STREAM[1:]
+        SAMPLE_TEXT_STREAM[:-2] + SAMPLE_TOOL_STREAM[1:]
     )))
     texts: List[str] = []
     tool_calls: List[ToolCall] = []
     async for event in stream:
-        if event[0] == ChatMessageRole.AI:
-            assert event[1] == 'text'
+        if event[0] == 'ai':
+            assert event[1] == 'text_event'
             texts.append(event[2])
-        elif event[0] == ChatMessageRole.TOOL_CALL:
-            if event[1] == 'text':
+        elif event[0] == 'tool_call':
+            if event[1] == 'text_event':
                 texts.append(event[2])
-            elif event[1] == 'tool_call':
+            elif event[1] == 'tool_call_event':
                 tool_calls.append(event[2])
             else:
                 assert False, event[1]
         else:
             assert False, event[0]
     text = ''.join(texts)
     assert text == 'Hello Ryan! 5 multiplied by 7 is 35.\n\nmultiply({"a": 5, "b": 7})\nmultiply({"a": 8, "b": 101})'
@@ -780,47 +788,47 @@
             },
         },
     }
 
 
 @pytest.mark.asyncio
 async def test_convert_to_openai_messages():
-    messages: List[ChatMessage] = [
+    messages: List[Message] = [
         {
             'role': 'INVALID', # type: ignore
             'text': 'bla',
             'cost': None,
             'raw': None,
         },
     ]
     with pytest.raises(ValueError):
         await _convert_to_openai_messages(messages)
 
-    messages: List[ChatMessage] = [
-        {'role': ChatMessageRole.SYSTEM, 'text': 'be nice', 'media': None, 'cost': None, 'raw': None},
-        {'role': ChatMessageRole.HUMAN, 'text': 'hi', 'media': None, 'cost': None, 'raw': None},
-        {'role': ChatMessageRole.AI, 'text': 'oh hi', 'media': None, 'cost': None, 'raw': None},
-        {'role': ChatMessageRole.HUMAN, 'text': 'here is a picture', 'media': [{'media_type': 'image', 'image': 'http://example.com/img.png'}], 'cost': None, 'raw': None},
-        {'role': ChatMessageRole.AI, 'text': 'thanks!', 'media': None, 'cost': None, 'raw': None},
-        {'role': ChatMessageRole.HUMAN, 'text': 'here are two', 'media': [{'media_type': 'image', 'image': 'http://example.com/img.png'}, {'media_type': 'image', 'image': 'http://example.com/img2.png'}], 'cost': None, 'raw': None},
-        {'role': ChatMessageRole.AI, 'text': 'double thanks!', 'media': None, 'cost': None, 'raw': None},
+    messages: List[Message] = [
+        {'role': 'system', 'text': 'be nice', 'cost': None, 'raw': None},
+        {'role': 'human', 'text': 'hi', 'cost': None, 'raw': None},
+        {'role': 'ai', 'text': 'oh hi', 'cost': None, 'raw': None},
+        {'role': 'human', 'text': 'here is a picture', 'media': [{'media_type': 'image', 'image': 'http://example.com/img.png'}], 'cost': None, 'raw': None},
+        {'role': 'ai', 'text': 'thanks!', 'cost': None, 'raw': None},
+        {'role': 'human', 'text': 'here are two', 'media': [{'media_type': 'image', 'image': 'http://example.com/img.png'}, {'media_type': 'image', 'image': 'http://example.com/img2.png'}], 'cost': None, 'raw': None},
+        {'role': 'ai', 'text': 'double thanks!', 'cost': None, 'raw': None},
     ]
     ms = await _convert_to_openai_messages(messages)
     assert ms == [
         {'role': 'system', 'content': 'be nice'},
         {'role': 'user', 'content': [{'type': 'text', 'text': 'hi'}]},
         {'role': 'assistant', 'content': 'oh hi'},
         {'role': 'user', 'content': [{'type': 'text', 'text': 'here is a picture'}, {'type': 'image_url', 'image_url': {'url': 'http://example.com/img.png'}}]},
         {'role': 'assistant', 'content': 'thanks!'},
         {'role': 'user', 'content': [{'type': 'text', 'text': 'here are two'}, {'type': 'image_url', 'image_url': {'url': 'http://example.com/img.png'}}, {'type': 'image_url', 'image_url': {'url': 'http://example.com/img2.png'}}]},
         {'role': 'assistant', 'content': 'double thanks!'},
     ]
 
-    messages: List[ChatMessage] = [{
-        'role': ChatMessageRole.TOOL_CALL,
+    messages: List[Message] = [{
+        'role': 'tool_call',
         'tools': [
             {'call_id': 'call_x7zmzwKI0LrwDF2xVMcfzXzN', 'function': {'arguments': '{"a": 5, "b": 7}', 'name': 'multiply'}, 'call_type': 'function'},
             {'call_id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'call_type': 'function'},
         ],
         'cost': None,
         'raw': None,
     }]
@@ -830,16 +838,16 @@
         'content': None,
         'tool_calls': [
             {'id': 'call_x7zmzwKI0LrwDF2xVMcfzXzN', 'function': {'arguments': '{"a": 5, "b": 7}', 'name': 'multiply'}, 'type': 'function'},
             {'id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'type': 'function'},
         ],
     }]
 
-    messages: List[ChatMessage] = [{
-        'role': ChatMessageRole.TOOL_RES,
+    messages: List[Message] = [{
+        'role': 'tool_res',
         'tools': [
             {'call_id': '1002', 'result': 10.8 },
             {'call_id': '1003', 'result': "hihi" },
         ],
         'cost': None,
         'raw': None,
     }]
@@ -853,24 +861,23 @@
         {
             'role': 'tool',
             'content': "hihi",
             'tool_call_id': "1003",
         },
     ]
 
-    messages: List[ChatMessage] = [
+    messages: List[Message] = [
         {
-            'role': ChatMessageRole.AI,
+            'role': 'ai',
             'text': "I'll use my tools!",
-            'media': None,
             'cost': None,
             'raw': None,
         },
         {
-            'role': ChatMessageRole.TOOL_CALL,
+            'role': 'tool_call',
             'tools': [
                 {'call_id': 'call_x7zmzwKI0LrwDF2xVMcfzXzN', 'function': {'arguments': '{"a": 5, "b": 7}', 'name': 'multiply'}, 'call_type': 'function'},
                 {'call_id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'call_type': 'function'},
             ],
             'cost': None,
             'raw': None,
         },
@@ -884,96 +891,101 @@
             {'id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'type': 'function'},
         ],
     }]
 
 
 def test_build_messages_from_openai_payload():
     events: List[EventPayload] = [
-        (ChatMessageRole.AI, 'text', 'Hello'),
-        (ChatMessageRole.AI, 'text', ' Ryan'),
+        ('ai', 'text_event', 'Hello'),
+        ('ai', 'text_event', ' Ryan'),
     ]
     messages = _build_messages_from_openai_payload([], events)
     assert messages == [{
-        'role': ChatMessageRole.AI,
+        'role': 'ai',
         'text': 'Hello Ryan',
-        'media': None,
         'cost': None,
         'raw': [],
     }]
 
     tool_calls: List[ToolCall] = [
         {'call_id': 'call_x7zmzwKI0LrwDF2xVMcfzXzN', 'function': {'arguments': '{"a": 5, "b": 7}', 'name': 'multiply'}, 'call_type': 'function'},
         {'call_id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'call_type': 'function'},
     ]
     events: List[EventPayload] = [
-        (ChatMessageRole.TOOL_CALL, 'text', 'multiply('),
-        (ChatMessageRole.TOOL_CALL, 'text', '{"a"'),
-        (ChatMessageRole.TOOL_CALL, 'text', ': 5, '),
-        (ChatMessageRole.TOOL_CALL, 'text', '"b": 7'),
-        (ChatMessageRole.TOOL_CALL, 'text', '}'),
-        (ChatMessageRole.TOOL_CALL, 'text', ')\n'),
-        (ChatMessageRole.TOOL_CALL, 'text', 'multiply('),
-        (ChatMessageRole.TOOL_CALL, 'text', '{"a"'),
-        (ChatMessageRole.TOOL_CALL, 'text', ': 8, '),
-        (ChatMessageRole.TOOL_CALL, 'text', '"b": 1'),
-        (ChatMessageRole.TOOL_CALL, 'text', '01}'),
-        (ChatMessageRole.TOOL_CALL, 'text', ')'),
-        (ChatMessageRole.TOOL_CALL, 'tool_call', tool_calls[0]),
-        (ChatMessageRole.TOOL_CALL, 'tool_call', tool_calls[1]),
+        ('tool_call', 'text_event', 'multiply('),
+        ('tool_call', 'text_event', '{"a"'),
+        ('tool_call', 'text_event', ': 5, '),
+        ('tool_call', 'text_event', '"b": 7'),
+        ('tool_call', 'text_event', '}'),
+        ('tool_call', 'text_event', ')\n'),
+        ('tool_call', 'text_event', 'multiply('),
+        ('tool_call', 'text_event', '{"a"'),
+        ('tool_call', 'text_event', ': 8, '),
+        ('tool_call', 'text_event', '"b": 1'),
+        ('tool_call', 'text_event', '01}'),
+        ('tool_call', 'text_event', ')'),
+        ('tool_call', 'tool_call_event', tool_calls[0]),
+        ('tool_call', 'tool_call_event', tool_calls[1]),
     ]
     messages = _build_messages_from_openai_payload([], events)
     assert messages == [{
-        'role': ChatMessageRole.TOOL_CALL,
+        'role': 'tool_call',
         'tools': [
             {'call_id': 'call_x7zmzwKI0LrwDF2xVMcfzXzN', 'function': {'arguments': '{"a": 5, "b": 7}', 'name': 'multiply'}, 'call_type': 'function'},
             {'call_id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'call_type': 'function'},
         ],
         'cost': None,
         'raw': [],
     }]
 
     tool_calls: List[ToolCall] = [
         {'call_id': 'call_x7zmzwKI0LrwDF2xVMcfzXzN', 'function': {'arguments': '{"a": 5, "b": 7}', 'name': 'multiply'}, 'call_type': 'function'},
         {'call_id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'call_type': 'function'},
     ]
     events: List[EventPayload] = [
-        (ChatMessageRole.AI, 'text', 'Hello'),
-        (ChatMessageRole.AI, 'text', ' Ryan'),
-        (ChatMessageRole.TOOL_CALL, 'text', 'multiply('),
-        (ChatMessageRole.TOOL_CALL, 'text', '{"a"'),
-        (ChatMessageRole.TOOL_CALL, 'text', ': 5, '),
-        (ChatMessageRole.TOOL_CALL, 'text', '"b": 7'),
-        (ChatMessageRole.TOOL_CALL, 'text', '}'),
-        (ChatMessageRole.TOOL_CALL, 'text', ')\n'),
-        (ChatMessageRole.TOOL_CALL, 'text', 'multiply('),
-        (ChatMessageRole.TOOL_CALL, 'text', '{"a"'),
-        (ChatMessageRole.TOOL_CALL, 'text', ': 8, '),
-        (ChatMessageRole.TOOL_CALL, 'text', '"b": 1'),
-        (ChatMessageRole.TOOL_CALL, 'text', '01}'),
-        (ChatMessageRole.TOOL_CALL, 'text', ')'),
-        (ChatMessageRole.TOOL_CALL, 'tool_call', tool_calls[0]),
-        (ChatMessageRole.TOOL_CALL, 'tool_call', tool_calls[1]),
+        ('ai', 'text_event', 'Hello'),
+        ('ai', 'text_event', ' Ryan'),
+        ('tool_call', 'text_event', 'multiply('),
+        ('tool_call', 'text_event', '{"a"'),
+        ('tool_call', 'text_event', ': 5, '),
+        ('tool_call', 'text_event', '"b": 7'),
+        ('tool_call', 'text_event', '}'),
+        ('tool_call', 'text_event', ')\n'),
+        ('tool_call', 'text_event', 'multiply('),
+        ('tool_call', 'text_event', '{"a"'),
+        ('tool_call', 'text_event', ': 8, '),
+        ('tool_call', 'text_event', '"b": 1'),
+        ('tool_call', 'text_event', '01}'),
+        ('tool_call', 'text_event', ')'),
+        ('tool_call', 'tool_call_event', tool_calls[0]),
+        ('tool_call', 'tool_call_event', tool_calls[1]),
     ]
-    messages = _build_messages_from_openai_payload([], events)
+    messages = _build_messages_from_openai_payload(SAMPLE_TEXT_STREAM[-3:], events)
     assert messages == [
         {
-            'role': ChatMessageRole.AI,
+            'role': 'ai',
             'text': 'Hello Ryan',
-            'media': None,
             'cost': None,
             'raw': None,
         },
         {
-            'role': ChatMessageRole.TOOL_CALL,
+            'role': 'tool_call',
             'tools': [
                 {'call_id': 'call_x7zmzwKI0LrwDF2xVMcfzXzN', 'function': {'arguments': '{"a": 5, "b": 7}', 'name': 'multiply'}, 'call_type': 'function'},
                 {'call_id': 'call_33vMBGeVd96A9BhW6H3r8jHb', 'function': {'arguments': '{"a": 8, "b": 101}', 'name': 'multiply'}, 'call_type': 'function'},
             ],
-            'cost': None,
-            'raw': [],
+            'cost': {
+                'input_tokens': 21,
+                'output_tokens': 22,
+                'total_tokens': 43,
+            },
+            'raw': [
+                v.to_dict()
+                for v in SAMPLE_TEXT_STREAM[-3:]
+            ],
         },
     ]
 
 
 def tool_a(first, second, third=5):
     return first + second + third
 
@@ -995,16 +1007,16 @@
     tool_map: Dict[str, Callable] = {
         'tool_a': tool_a,
         'tool_b': tool_b,
         'tool_c': tool_c,
         'tool_async_a': tool_async_a,
         'tool_async_b': tool_async_b,
     }
-    message: ChatMessage = {
-        'role': ChatMessageRole.TOOL_CALL,
+    message: Message = {
+        'role': 'tool_call',
         'tools': [
             {'call_id': '1001', 'function': {'arguments': '{"x": 8}', 'name': 'tool_b'}, 'call_type': 'function'},
             {'call_id': '1002', 'function': {'arguments': '{"x": 5.4}', 'name': 'tool_b'}, 'call_type': 'function'},
             {'call_id': '1003', 'function': {'arguments': '{"x": "hi"}', 'name': 'tool_b'}, 'call_type': 'function'},
             {'call_id': '1004', 'function': {'arguments': '{}', 'name': 'tool_b'}, 'call_type': 'function'},
             {'call_id': '1005', 'function': {'arguments': '{"y": "hi"}', 'name': 'tool_b'}, 'call_type': 'function'},
             {'call_id': '1006', 'function': {'arguments': '{"x": 4, "y": "hi"}', 'name': 'tool_b'}, 'call_type': 'function'},
@@ -1047,12 +1059,12 @@
 def test_build_tool_response_message():
     res: List[ToolResult] = [
         {'call_id': '1002', 'result': 10.8 },
         {'call_id': '1003', 'result': "hihi" },
     ]
     message = _build_tool_response_message(res)
     assert message == {
-        'role': ChatMessageRole.TOOL_RES,
+        'role': 'tool_res',
         'tools': res,
         'cost': None,
         'raw': None,
     }
```

### Comparing `lasagna_ai-0.1.0/tests/test_registrar.py` & `lasagna_ai-0.2.0/tests/test_registrar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 
 from lasagna.registrar import (
     register_agent,
-    register_model_provider,
+    register_provider,
     AGENTS,
-    MODEL_PROVIDERS,
+    PROVIDERS,
 )
 
-from lasagna.types import AgentCallable, ProviderFactory, ModelRecord
+from lasagna.types import AgentCallable, ModelFactory, ModelRecord
 
 from typing import List
 
 
 def test_register_agent():
     AGENTS.clear()
     runner: AgentCallable = 'mock'   # type: ignore
@@ -23,25 +23,25 @@
         },
     }
     with pytest.raises(RuntimeError):
         register_agent('myagent', 'My Agent', runner)
 
 
 def test_register_model_provider():
-    MODEL_PROVIDERS.clear()
-    factory: ProviderFactory = 'mock'   # type: ignore
+    PROVIDERS.clear()
+    factory: ModelFactory = 'mock'   # type: ignore
     models: List[ModelRecord] = [
         {
             'formal_name': 'mymodel',
             'display_name': 'My Model',
         }
     ]
-    register_model_provider('myprovider', 'My Provider', factory, models)
-    assert MODEL_PROVIDERS == {
+    register_provider('myprovider', 'My Provider', factory, models)
+    assert PROVIDERS == {
         'myprovider': {
             'name': 'My Provider',
             'factory': factory,
             'models': models,
         },
     }
     with pytest.raises(RuntimeError):
-        register_model_provider('myprovider', 'My Provider', factory, models)
+        register_provider('myprovider', 'My Provider', factory, models)
```

### Comparing `lasagna_ai-0.1.0/tests/test_stream.py` & `lasagna_ai-0.2.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `lasagna_ai-0.1.0/tests/test_util.py` & `lasagna_ai-0.2.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `lasagna_ai-0.1.0/.gitignore` & `lasagna_ai-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lasagna_ai-0.1.0/LICENSE.txt` & `lasagna_ai-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lasagna_ai-0.1.0/README.md` & `lasagna_ai-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,47 @@
+![Lasagna AI Logo](./logos/lasagna-ai.png)
+
 # Lasagna AI
 
 [![PyPI - Version](https://img.shields.io/pypi/v/lasagna-ai.svg)](https://pypi.org/project/lasagna-ai)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lasagna-ai.svg)](https://pypi.org/project/lasagna-ai)
-![Test Status](https://github.com/Rhobota/lasagna-ai/workflows/Test%20Matrix/badge.svg)
-
-TODO: More badges:
- - Linux, MacOS, Windows
- - Code coverage %
+![Test Status](https://github.com/Rhobota/lasagna-ai/actions/workflows/test.yml/badge.svg?branch=main)
 
-**Agents for your agents!**
+- 🥞  **Layered agents!**
+  - Agents for your agents!
+  - Tool-use and layering FTW 💪
+  - Built-in parallel tool-calling.
+  - Fully asyncio.
+  - Ever wanted a recursive agent? 🤯
+  - Strongly typed (if you're into that).
+
+- 🚣  **Streamable!**
+  - Event streams for everything.
+
+- 🗃️ **Easy database integration!**
+  - Don't rage when trying to store raw messages and token counts. 😡 🤬
+
+- ↔️ **Provider/model agnostic and interoperable!**
+  - Native support for OpenAI, Anthropic, MistralAI (+ more to come).
+  - Message representations are canonized. 😇
+  - Supports vision!
+  - Easily build committees!
+  - Swap providers or models mid-conversation.
+  - Delegate tasks among model providers or model sizes.
+  - Parallelize all the things.
 
 -----
 
-## Highlights
-
-- Canonizes OpenAI, Anthropic, MistralAI (and more in the future)
-   - easily swap between them
-   - build comities
-   - etc
-- Everything is streamable.
-- Also easy to integrate with a database.
-- Lasagna has layers. Now your agents can too!
-   - Build hierarchical (or even recursive) agents! Lasagna has layers!
-- Fully asyncio (with threadpools where appropriate)
-   - Parallel tool calling (your tools can by either sync or async, no prob!)
-- Supports _vision_!
-- Strongly typed
-- 90% test coverage
-
 ## Table of Contents
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
-pip install lasagna-ai[openai,anthropic]
+pip install -U lasagna-ai[openai,anthropic]
 ```
 
 ## License
 
 `lasagna-ai` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lasagna_ai-0.1.0/pyproject.toml` & `lasagna_ai-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lasagna-ai"
 dynamic = ["version"]
-description = 'Agents for your agents!'
+description = 'Layered agents!'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = ["ai", "agents", "llm", "hierarchical"]
+keywords = ["ai", "agent", "agents", "llm", "hierarchical", "layers", "layered"]
 authors = [
   { name = "Ryan Henning", email = "ryan@rhobota.com" },
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -28,15 +28,15 @@
 [project.urls]
 Documentation = "https://github.com/Rhobota/lasagna-ai#readme"
 Issues = "https://github.com/Rhobota/lasagna-ai/issues"
 Source = "https://github.com/Rhobota/lasagna-ai"
 
 [project.optional-dependencies]
 openai = [
-  "openai>=1.23.2",
+  "openai>=1.30.3",
 ]
 anthropic = [
   "anthropic>=0.26.1",
 ]
 dev = [
   "mypy>=1.10.0",
   "pytest>=8.1.1",
```

### Comparing `lasagna_ai-0.1.0/PKG-INFO` & `lasagna_ai-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: lasagna-ai
-Version: 0.1.0
-Summary: Agents for your agents!
+Version: 0.2.0
+Summary: Layered agents!
 Project-URL: Documentation, https://github.com/Rhobota/lasagna-ai#readme
 Project-URL: Issues, https://github.com/Rhobota/lasagna-ai/issues
 Project-URL: Source, https://github.com/Rhobota/lasagna-ai
 Author-email: Ryan Henning <ryan@rhobota.com>
 License-Expression: MIT
 License-File: LICENSE.txt
-Keywords: agents,ai,hierarchical,llm
+Keywords: agent,agents,ai,hierarchical,layered,layers,llm
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -21,54 +21,57 @@
 Provides-Extra: anthropic
 Requires-Dist: anthropic>=0.26.1; extra == 'anthropic'
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == 'dev'
 Requires-Dist: pytest-asyncio>=0.23.6; extra == 'dev'
 Requires-Dist: pytest>=8.1.1; extra == 'dev'
 Provides-Extra: openai
-Requires-Dist: openai>=1.23.2; extra == 'openai'
+Requires-Dist: openai>=1.30.3; extra == 'openai'
 Description-Content-Type: text/markdown
 
+![Lasagna AI Logo](./logos/lasagna-ai.png)
+
 # Lasagna AI
 
 [![PyPI - Version](https://img.shields.io/pypi/v/lasagna-ai.svg)](https://pypi.org/project/lasagna-ai)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lasagna-ai.svg)](https://pypi.org/project/lasagna-ai)
-![Test Status](https://github.com/Rhobota/lasagna-ai/workflows/Test%20Matrix/badge.svg)
-
-TODO: More badges:
- - Linux, MacOS, Windows
- - Code coverage %
+![Test Status](https://github.com/Rhobota/lasagna-ai/actions/workflows/test.yml/badge.svg?branch=main)
 
-**Agents for your agents!**
+- 🥞  **Layered agents!**
+  - Agents for your agents!
+  - Tool-use and layering FTW 💪
+  - Built-in parallel tool-calling.
+  - Fully asyncio.
+  - Ever wanted a recursive agent? 🤯
+  - Strongly typed (if you're into that).
+
+- 🚣  **Streamable!**
+  - Event streams for everything.
+
+- 🗃️ **Easy database integration!**
+  - Don't rage when trying to store raw messages and token counts. 😡 🤬
+
+- ↔️ **Provider/model agnostic and interoperable!**
+  - Native support for OpenAI, Anthropic, MistralAI (+ more to come).
+  - Message representations are canonized. 😇
+  - Supports vision!
+  - Easily build committees!
+  - Swap providers or models mid-conversation.
+  - Delegate tasks among model providers or model sizes.
+  - Parallelize all the things.
 
 -----
 
-## Highlights
-
-- Canonizes OpenAI, Anthropic, MistralAI (and more in the future)
-   - easily swap between them
-   - build comities
-   - etc
-- Everything is streamable.
-- Also easy to integrate with a database.
-- Lasagna has layers. Now your agents can too!
-   - Build hierarchical (or even recursive) agents! Lasagna has layers!
-- Fully asyncio (with threadpools where appropriate)
-   - Parallel tool calling (your tools can by either sync or async, no prob!)
-- Supports _vision_!
-- Strongly typed
-- 90% test coverage
-
 ## Table of Contents
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
-pip install lasagna-ai[openai,anthropic]
+pip install -U lasagna-ai[openai,anthropic]
 ```
 
 ## License
 
 `lasagna-ai` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

