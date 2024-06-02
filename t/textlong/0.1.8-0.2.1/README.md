# Comparing `tmp/textlong-0.1.8.tar.gz` & `tmp/textlong-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlong-0.1.8.tar", max compression
+gzip compressed data, was "textlong-0.2.1.tar", max compression
```

## Comparing `textlong-0.1.8.tar` & `textlong-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.8/LICENSE
--rw-r--r--   0        0        0     1604 2024-05-18 06:08:22.626599 textlong-0.1.8/README.md
--rw-r--r--   0        0        0      950 2024-05-21 03:40:50.273162 textlong-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.8/textlong/.pypirc
--rw-r--r--   0        0        0      638 2024-05-20 22:20:34.997733 textlong-0.1.8/textlong/__init__.py
--rw-r--r--   0        0        0       22 2024-05-21 03:40:14.226971 textlong-0.1.8/textlong/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.8/textlong/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.8/textlong/agents/base.py
--rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.8/textlong/agents/prompt.py
--rw-r--r--   0        0        0     2370 2024-05-19 07:03:51.711272 textlong-0.1.8/textlong/ai.py
--rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.8/textlong/base.py
--rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.8/textlong/command.py
--rw-r--r--   0        0        0      399 2024-05-20 13:06:13.568404 textlong-0.1.8/textlong/config.py
--rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.8/textlong/docs/__init__.py
--rw-r--r--   0        0        0     3591 2024-05-19 12:16:37.280829 textlong-0.1.8/textlong/docs/writing_help.py
--rw-r--r--   0        0        0      113 2024-05-20 14:16:45.955689 textlong-0.1.8/textlong/document_loaders/__init__.py
--rw-r--r--   0        0        0     5160 2024-05-20 14:00:52.675879 textlong-0.1.8/textlong/document_loaders/base.py
--rw-r--r--   0        0        0     3089 2024-05-20 14:36:58.320633 textlong-0.1.8/textlong/document_loaders/qa_excel.py
--rw-r--r--   0        0        0      813 2024-05-20 14:13:34.220746 textlong-0.1.8/textlong/document_loaders/qa_markdown.py
--rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.8/textlong/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.8/textlong/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.8/textlong/memory/__init__.py
--rw-r--r--   0        0        0     7990 2024-05-21 00:14:39.945505 textlong-0.1.8/textlong/memory/base.py
--rw-r--r--   0        0        0     3320 2024-05-20 02:18:02.245645 textlong-0.1.8/textlong/memory/file_store.py
--rw-r--r--   0        0        0     2708 2024-05-20 01:50:58.318560 textlong-0.1.8/textlong/memory/memory_manager.py
--rw-r--r--   0        0        0    10875 2024-05-19 08:17:29.283447 textlong-0.1.8/textlong/node.py
--rw-r--r--   0        0        0     6673 2024-05-20 22:08:33.246467 textlong-0.1.8/textlong/projects.py
--rw-r--r--   0        0        0      243 2024-05-20 22:39:35.717193 textlong-0.1.8/textlong/prompts/__init__.py
--rw-r--r--   0        0        0     4581 2024-05-21 02:04:23.542824 textlong-0.1.8/textlong/prompts/hub.py
--rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.8/textlong/prompts/main.py
--rw-r--r--   0        0        0     1327 2024-05-20 23:32:21.329587 textlong-0.1.8/textlong/prompts/qa_prompt.py
--rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.8/textlong/prompts/translate.py
--rw-r--r--   0        0        0     6043 2024-05-20 16:58:59.906388 textlong-0.1.8/textlong/prompts/writing_prompt.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.8/textlong/retrievers/__init__.py
--rw-r--r--   0        0        0     3109 2024-05-20 23:14:36.258930 textlong-0.1.8/textlong/retrievers/base.py
--rw-r--r--   0        0        0     3213 2024-05-19 07:30:31.509304 textlong-0.1.8/textlong/serialize.py
--rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.1.8/textlong/state.py
--rw-r--r--   0        0        0     1983 2024-05-19 15:29:28.868426 textlong-0.1.8/textlong/tree.py
--rw-r--r--   0        0        0     3563 2024-05-19 15:30:49.311152 textlong-0.1.8/textlong/writing.py
--rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 textlong-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1609 2024-05-27 06:00:57.025971 textlong-0.2.1/README.md
+-rw-r--r--   0        0        0      950 2024-05-26 03:50:15.583842 textlong-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 08:55:27.442894 textlong-0.2.1/textlong/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-26 03:50:08.210083 textlong-0.2.1/textlong/__version__.py
+-rw-r--r--   0        0        0      119 2024-05-26 06:37:36.690700 textlong-0.2.1/textlong/agents/__init__.py
+-rw-r--r--   0        0        0     2682 2024-05-26 12:27:08.537267 textlong-0.2.1/textlong/agents/base.py
+-rw-r--r--   0        0        0     5465 2024-05-26 12:28:27.746952 textlong-0.2.1/textlong/agents/prompt.py
+-rw-r--r--   0        0        0     5269 2024-05-26 12:27:34.198627 textlong-0.2.1/textlong/agents/tools_calling.py
+-rw-r--r--   0        0        0      561 2024-06-02 13:39:23.535997 textlong-0.2.1/textlong/config.py
+-rw-r--r--   0        0        0     4845 2024-05-26 11:19:16.288548 textlong-0.2.1/textlong/hub.py
+-rw-r--r--   0        0        0      151 2024-06-02 09:28:00.993323 textlong-0.2.1/textlong/md/__init__.py
+-rw-r--r--   0        0        0     4836 2024-05-29 01:30:38.489755 textlong-0.2.1/textlong/md/agent.py
+-rw-r--r--   0        0        0    14158 2024-06-02 14:14:03.347519 textlong-0.2.1/textlong/md/documents.py
+-rw-r--r--   0        0        0     2060 2024-05-29 01:29:05.697202 textlong-0.2.1/textlong/md/output_parser.py
+-rw-r--r--   0        0        0    10514 2024-06-02 09:38:38.450344 textlong-0.2.1/textlong/md/prompt.py
+-rw-r--r--   0        0        0     1530 2024-06-01 01:22:16.863581 textlong-0.2.1/textlong/md/tools.py
+-rw-r--r--   0        0        0    10223 2024-06-02 10:08:16.652718 textlong-0.2.1/textlong/md/writing.py
+-rw-r--r--   0        0        0      170 2024-05-26 06:45:01.498326 textlong-0.2.1/textlong/memory/__init__.py
+-rw-r--r--   0        0        0     7989 2024-05-26 06:33:22.429730 textlong-0.2.1/textlong/memory/base.py
+-rw-r--r--   0        0        0     3218 2024-05-26 06:52:01.455853 textlong-0.2.1/textlong/memory/file_store.py
+-rw-r--r--   0        0        0     2708 2024-05-26 06:53:01.003204 textlong-0.2.1/textlong/memory/memory_manager.py
+-rw-r--r--   0        0        0      254 2024-05-26 08:27:52.839755 textlong-0.2.1/textlong/qa/__init__.py
+-rw-r--r--   0        0        0     5503 2024-06-02 12:43:15.971131 textlong-0.2.1/textlong/qa/local_files.py
+-rw-r--r--   0        0        0     3096 2024-05-26 06:20:08.215444 textlong-0.2.1/textlong/qa/qa_excel.py
+-rw-r--r--   0        0        0     1327 2024-05-20 23:32:21.329587 textlong-0.2.1/textlong/qa/qa_prompt.py
+-rw-r--r--   0        0        0     3055 2024-05-26 07:31:00.597137 textlong-0.2.1/textlong/qa/tool.py
+-rw-r--r--   0        0        0      514 2024-05-26 09:07:01.950794 textlong-0.2.1/textlong/tree/__init__.py
+-rw-r--r--   0        0        0     2377 2024-05-26 06:11:26.953594 textlong-0.2.1/textlong/tree/ai.py
+-rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.2.1/textlong/tree/command.py
+-rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.2.1/textlong/tree/docs/__init__.py
+-rw-r--r--   0        0        0     3591 2024-05-26 06:08:43.258611 textlong-0.2.1/textlong/tree/docs/help.py
+-rw-r--r--   0        0        0    10875 2024-05-26 06:14:47.496354 textlong-0.2.1/textlong/tree/node.py
+-rw-r--r--   0        0        0     6659 2024-05-26 06:14:31.326630 textlong-0.2.1/textlong/tree/projects.py
+-rw-r--r--   0        0        0     3213 2024-05-19 07:30:31.509304 textlong-0.2.1/textlong/tree/serialize.py
+-rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.2.1/textlong/tree/state.py
+-rw-r--r--   0        0        0     1983 2024-05-26 06:25:13.062117 textlong-0.2.1/textlong/tree/tree.py
+-rw-r--r--   0        0        0     3556 2024-05-26 06:15:13.308190 textlong-0.2.1/textlong/tree/writing.py
+-rw-r--r--   0        0        0     6034 2024-05-26 06:10:40.966067 textlong-0.2.1/textlong/tree/writing_prompt.py
+-rw-r--r--   0        0        0      215 2024-06-02 12:24:53.590776 textlong-0.2.1/textlong/utils.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 textlong-0.2.1/PKG-INFO
```

### Comparing `textlong-0.1.8/LICENSE` & `textlong-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/README.md` & `textlong-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv(), override=True)
 ```
 
 **2. 创建`WritingTask`实例：**
 
 ```python
-from textlong import WritingTask
+from textlong.tree import WritingTask
 from langchain_openai import ChatOpenAI
 
 task = WritingTask(llm=ChatOpenAI())
 ```
 
 **3. 使用`auto_write`方法自动生成一段长文：**
```

### Comparing `textlong-0.1.8/pyproject.toml` & `textlong-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textlong"
-version = "0.1.8"
+version = "0.2.1"
 description = "A framework designed to produce long-texts with GPT or other large language models."
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/textlong"
 repository = "https://github.com/arcstep/textlong.git"
 license = "MIT"
 readme = "README.md"
```

### Comparing `textlong-0.1.8/textlong/agents/base.py` & `textlong-0.2.1/textlong/agents/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.pydantic_v1 import BaseModel, Field
 from langchain.agents.agent import AgentOutputParser, AgentAction, AgentFinish
 from langchain.agents.format_scratchpad import format_log_to_str
 from langchain.output_parsers import PydanticOutputParser
 from langchain.prompts import PromptTemplate
 from langchain.tools.render import render_text_description
-from .prompt import PROMPT_COT, PROMPT_REACT
+from .prompt import PROMPT_COT
 
 class Action(BaseModel):
     name: str = Field(
         description="The name of tool or action: FINISH or Other tool names."
         )
     args: Optional[Dict[str, Any]] = Field(
         default=None,
         description="Parameters of tool or action are composed of names and values."
         )
 
 # 解析Action
 _action_output_parser = PydanticOutputParser(pydantic_object=Action)
 _action_parser_format = _action_output_parser.get_format_instructions()
 
-class ReasonOutputParser(AgentOutputParser):
-    """解析单个动作的智能体action和输入参数。
+class AgentOutputParser(AgentOutputParser):
+    """
+    解析单个动作的智能体action和输入参数。
     """
 
     def parse(self, text: str) -> Union[AgentAction, AgentFinish]:
         action: Action = _action_output_parser.invoke(text)
         name: Optional[str] = action.name
         args: Optional[Dict[str, Any]] = action.args if text is not None else "No Args"
         log: str = text if text is not None else ""
@@ -36,37 +37,37 @@
         elif name is not None:
             return AgentAction(name, args, log)
 
     @property
     def _type(self) -> str:
         return "Chain-of-Thought"
 
-def _prompt_creator(prompt: str) -> Callable[[List[str]], str]:
+def _prompt_factory(prompt: str) -> Callable[[List[str]], str]:
     def creator(tools: List[str]) -> str:
         # 请注意，智谱AI等国内大模型对于pydantic的参数解析并不友好，使用JSON描述参数时会误读
         # 因此，不要使用 render_text_description_and_args 来生成工具描述
         tools_format = render_text_description(tools)
 
         template = PromptTemplate.from_template(prompt)
         return template.partial(
             tools=tools_format,
             action_format_instructions=_action_parser_format,
         )
 
     return creator
 
-# 基于 ReAct / CoT 的智能体
-def create_reason_agent(llm: Any, prompt: Optional[str] = None, tools: List[str] = []) -> Any:
-    prompt_creator = _prompt_creator(PROMPT_COT)
+# 智能体
+def create_agent(llm: Any, prompt: Optional[str] = None, tools: List[str] = []) -> Any:
+    prompt_factory = _prompt_factory(PROMPT_COT)
     if prompt is not None:
-        prompt_creator = _prompt_creator(prompt)
+        prompt_factory = _prompt_factory(prompt)
 
     agent = (
         RunnablePassthrough.assign(
             agent_scratchpad=lambda x: format_log_to_str(x["intermediate_steps"])
         )
-        | prompt_creator(tools)
+        | prompt_factory(tools)
         | llm
-        | ReasonOutputParser()
+        | AgentOutputParser()
     )
 
     return agent
```

### Comparing `textlong-0.1.8/textlong/ai.py` & `textlong-0.2.1/textlong/tree/ai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Iterator, List, Optional, Union, Tuple
 from langchain_core.runnables import Runnable
 from langchain_core.output_parsers import JsonOutputParser
 from langchain.schema.output_parser import StrOutputParser
 from langchain.memory.chat_memory import BaseChatMemory
 from langchain.memory import ConversationBufferWindowMemory
-from .prompts import create_writing_help_prompt
+from .writing_prompt import create_writing_help_prompt
 import os
 
 class BaseAI():
     """
     向AI提问。
     """
```

### Comparing `textlong-0.1.8/textlong/command.py` & `textlong-0.2.1/textlong/tree/command.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/docs/writing_help.py` & `textlong-0.2.1/textlong/tree/docs/help.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/document_loaders/base.py` & `textlong-0.2.1/textlong/qa/local_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from typing import Iterator, List, Union
 from langchain_core.documents import Document
+from langchain_community.document_loaders import (
+    TextLoader,
+    PyPDFLoader,
+    Docx2txtLoader,
+    UnstructuredMarkdownLoader,
+)
 from langchain_community.document_loaders.base import BaseLoader
-from langchain_community.document_loaders import TextLoader
-from langchain_community.document_loaders import PyPDFLoader
-from langchain_community.document_loaders import Docx2txtLoader
-from langchain_community.document_loaders import UnstructuredMarkdownLoader
 from langchain_community.document_loaders.excel import UnstructuredExcelLoader
-from ..config import get_textlong_folder, _DOCS_FOLDER_NAME
+from ..config import get_textlong_folder, get_textlong_doc, _DOCS_FOLDER_NAME
+from ..utils import raise_not_install
 
 import os
 import re
 import sys
 # import subprocess
 
-def raise_not_install(packages):
-    print(f"please install package: '{packages}' with pip or poetry")
-    # auto install package
-    # subprocess.check_call([sys.executable, "-m", "pip", "install", package_name])
-
 def get_file_extension(filename: str) -> str:
     """Get File Extension"""
     return filename.split(".")[-1].lower()
 
 class FileLoadFactory:
     @staticmethod
     def get_loader(filename):
@@ -84,14 +82,24 @@
     ):
         self.user_id = user_id or "public"
         self.path_regex = path_regex or ".*"
         self.included_prefixes = included_prefixes
         self.excluded_prefixes = excluded_prefixes
         self.extensions = extensions or ["docx", "pdf", "md", "txt", "xlsx"]
         self.documents_folder = os.path.join(get_textlong_folder(), self.user_id, _DOCS_FOLDER_NAME)
+    
+    def help(self):
+        return "\n".join([
+            item for item in [
+                f"支持为 <{self.user_id}> 从 [{self.documents_folder}] 中加载类型为 {','.join(self.extensions)} 的文件。",
+                f"路径规则应当符合 [{self.path_regex}] 的正则表达式规则检查" if self.path_regex != ".*" else "",
+                f"但仅包含以 [{self.included_prefixes}] 开始的文件夹" if self.included_prefixes else "",
+                f"但必须排除以 [{self.excluded_prefixes}] 开始的文件夹" if self.excluded_prefixes else "",
+            ] if item != ""
+        ])
 
     def get_files(self) -> list[str]:
         """List All Files with Extension"""
         files = []
 
         folders = self.documents_folder
         for dirpath, dirnames, filenames in os.walk(folders):
```

### Comparing `textlong-0.1.8/textlong/document_loaders/qa_excel.py` & `textlong-0.2.1/textlong/qa/qa_excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterator, List, Union
 from langchain_core.documents import Document
 from langchain_community.document_loaders.base import BaseLoader
 from ..config import get_textlong_folder, _QA_FOLDER_NAME
-from .base import LocalFilesLoader
+from .local_files import LocalFilesLoader
 
 import os
 import pandas as pd
 
 class QAExcelsLoader(LocalFilesLoader):
     """
     从本地文件中检索Excel文件，并以QA结构返回 Document 对象。
```

### Comparing `textlong-0.1.8/textlong/langgraph/tools_calling.py` & `textlong-0.2.1/textlong/agents/tools_calling.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/memory/base.py` & `textlong-0.2.1/textlong/memory/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 )
 
 if TYPE_CHECKING:
     from langchain_core.messages import BaseMessage
     from langchain_core.runnables.config import RunnableConfig
     from langchain_core.tracers.schemas import Run
 
-
 MessagesOrDictWithMessages = Union[Sequence["BaseMessage"], Dict[str, Any]]
 GetSessionHistoryCallable = Callable[..., BaseChatMessageHistory]
 
 from .memory_manager import MemoryManager
 
 class WithMemoryBinding(RunnableBindingBase):
     """Runnable that manages memory for another Runnable."""
```

### Comparing `textlong-0.1.8/textlong/memory/file_store.py` & `textlong-0.2.1/textlong/memory/file_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,27 +33,23 @@
         }
         if None in parsed.values():
             raise ValueError(f"None value found in parsed session_id: {session_id}")
         return parsed
     except ValueError:
         raise ValueError(f"Unable to parse session_id: {session_id}")
 
-class LocalFileMessageHistory(BaseChatMessageHistory):
+class LocalFileStore(BaseChatMessageHistory):
     """
     Chat message history that stores history in a local file.
 
     Args:
         file_path: path of the local file to store the messages.
     """
     
     @property
-    def history_folder(self):
-        return self._history_folder
-    
-    @property
     def file_path(self):
         """
         文件路径的构造规则：{history_folder}/{year}/{month}/{session_id}.json
         """
         parsed = parse_session_id(self.session_id)
         path = os.path.join(
             self.history_folder,
@@ -82,15 +78,15 @@
         all_messages = messages_from_dict(items)
         return all_messages
 
     def add_message(self, message: BaseMessage) -> None:
         """Append the message to the record in the local file"""
         all_messages = messages_to_dict(self.messages)
         all_messages.append(messages_to_dict([message])[0])
-        
+
         # 如果不存在就创建文件
         file_path = self.file_path
         if not file_path.parent.exists():
             file_path.parent.mkdir(parents=True)
         if not file_path.exists():
             file_path.touch()
```

### Comparing `textlong-0.1.8/textlong/memory/memory_manager.py` & `textlong-0.2.1/textlong/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/node.py` & `textlong-0.2.1/textlong/tree/node.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/projects.py` & `textlong-0.2.1/textlong/tree/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, Iterator, List, Optional, Union
 from dotenv import find_dotenv
 from .node import ContentNode
 from .serialize import ContentSerialize
-from .config import (
+from ..config import (
     get_textlong_folder,
     _NODES_FOLDER_NAME,
     _PROMPTS_FOLDER_NAME,
     _CONTENTS_FOLDER_NAME,
 )
-from .prompts.hub import load_chat_prompt, save_chat_prompt
-from .prompts.writing_prompt import (
+from ..hub import load_chat_prompt, save_chat_prompt
+from .writing_prompt import (
     create_writing_help_prompt,
     create_writing_init_prompt,
     create_writing_todo_prompt,
 )
 
 import os
 import json
```

### Comparing `textlong-0.1.8/textlong/prompts/hub.py` & `textlong-0.2.1/textlong/hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,29 @@
     ChatPromptTemplate,
     MessagesPlaceholder,
     SystemMessagePromptTemplate,
     AIMessagePromptTemplate,
     HumanMessagePromptTemplate,
     load_prompt as load_str_prompt,
 )
-from ..config import get_textlong_folder, _PROMPTS_FOLDER_NAME
+from .config import get_textlong_folder, _PROMPTS_FOLDER_NAME
 import os
 import json
 
 def save_chat_prompt(template: ChatPromptTemplate, template_id: str, project_id: str="default", id="0", user_id="public"):
     """
-    保存提示语模板。
+    保存对话风格的提示语模板。
+
+    提示语模板中的每一段对话和局部变量都会被保存为独立的`json`格式。
+    具体规则如下：
+        - 系统提示，`{对话序号}_system.json`
+        - 大模型消息，`{对话序号}_ai.json`
+        - 人类消息，`{对话序号}_human.json`
+        - 占位消息，`{对话序号}_placeholder.json`
+        - `partial`变量，`var_{变量名}.md`
     """
     prompt_path = os.path.join(get_textlong_folder(), user_id, project_id, _PROMPTS_FOLDER_NAME, id, template_id)
 
     for i, p in enumerate(template.messages):
         if isinstance(p, SystemMessagePromptTemplate):
             path = os.path.join(prompt_path, f"{i}_system.json")
         elif isinstance(p, AIMessagePromptTemplate):
@@ -43,35 +51,33 @@
 
 def load_chat_prompt(template_id: str, project_id: str="default", id: str="0", user_id: str="public", in_memory: bool=True):
     """
     加载提示语模板和partial变量的字符串。    
     目前不支持在partial中使用嵌套模板。
     """
     prompt_path = os.path.join(get_textlong_folder(), user_id, project_id, _PROMPTS_FOLDER_NAME, id, template_id)
-    if in_memory or not os.path.exists(prompt_path):
+    if in_memory and not os.path.exists(prompt_path):
         if template_id == "qa":
-            from .qa_prompt import create_qa_prompt
+            from .qa import create_qa_prompt
             template = create_qa_prompt()
         elif template_id == "help":
-            from .writing_prompt import create_writing_help_prompt
+            from .tree import create_writing_help_prompt
             template = create_writing_help_prompt()
         elif template_id == "init":
-            from .writing_prompt import create_writing_init_prompt
+            from .tree import create_writing_init_prompt
             template = create_writing_init_prompt()
         elif template_id == "outline":
-            from .writing_prompt import create_writing_todo_prompt
+            from .tree import create_writing_todo_prompt
             template = create_writing_todo_prompt(content_type="outline")
         elif template_id == "paragraph":
-            from .writing_prompt import create_writing_todo_prompt
+            from .tree import create_writing_todo_prompt
             template = create_writing_todo_prompt(content_type="paragraph")
         else:
-            raise ValueError(f"模板ID[{template_id}]不能支持！")
+            raise ValueError(f"模板ID[{template_id}]不是内置模板！")
         
-        if not in_memory:
-            save_chat_prompt(template, template_id, project_id, id, user_id)
         return template
 
     messages = []
     partial_variables = {}
 
     for filename in sorted(os.listdir(prompt_path)):
         path = os.path.join(prompt_path, filename)
```

### Comparing `textlong-0.1.8/textlong/prompts/qa_prompt.py` & `textlong-0.2.1/textlong/qa/qa_prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/prompts/writing_prompt.py` & `textlong-0.2.1/textlong/tree/writing_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Iterator, List, Optional, Union, Tuple
 from langchain.prompts import ChatPromptTemplate, MessagesPlaceholder
-from ..docs.writing_help import WRITING_HELP
+from .docs.help import WRITING_HELP
 
 # help prompt
 HELP_SYSTEM_PROMPT = """
 你只负责根据资料回答关于系统如何使用的提问，禁止回答与此无关的问题。
 如果你发现用户的提问与此无关，可以认为用户误用了指令，并引导用户如何正确使用系统。
 
 1. 你必须严格依据资料回答问题，不能编造除此之外的其他内容；
```

### Comparing `textlong-0.1.8/textlong/retrievers/base.py` & `textlong-0.2.1/textlong/qa/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 问题: {question}
 """
 
 def format_qa_docs(docs: List[str]) -> str:
     """
     如果 Document 中包含的 metadata['answer'] 属性就优先采纳。
     """
-    return "\n\n".join([d.metadata['answer'] or d.page_content for d in docs])
+    return "\n\n".join([
+        d.metadata['answer'] if 'answer' in d.metadata else d.page_content
+        for d in docs
+    ])
 
 def convert_message_to_str(message: Union[BaseMessage, str]) -> str:
     if isinstance(message, BaseMessage):
         return message.content
     else:
         return message
 
@@ -42,16 +45,16 @@
     chain.invoke("textlong是啥？")
     """
 
     _prompt = ChatPromptTemplate.from_template(prompt)
 
     return (
         {
-            "context": (lambda x: convert_message_to_str(x)) | retriever | format_qa_docs,
-            "question": lambda x: convert_message_to_str(x) ,
+            "context": (lambda x: convert_message_to_str(x['query'])) | retriever | format_qa_docs,
+            "question":(lambda x: convert_message_to_str(x['query'])),
         }
         | _prompt
         | llm
     )
 
 def make_safe_tool(func: Callable) -> Callable:
     """Create a new function that wraps the given function with error handling"""
@@ -72,21 +75,18 @@
 class AskDocumentTool(BaseTool):
     name: str = ASK_DOCUMENT_TOOL_NAME
     description: str = """
     根据资料库回答问题。考虑上下文信息，确保问题对相关概念的定义表述完整。
     args:
     - query 类型是str, 用户问题的文字描述的字符串
     """
-    args_schema: Type[BaseModel] = SearchInput
-    qa_chain: Runnable = Field(...)
+    chain: Runnable = Field(...)
 
     def _run(
         self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None
     ) -> str:
         """Use the tool."""
         
-        if isinstance(query, str):
-            query = [query]
-        return self.qa_chain.invoke([convert_message_to_str(q) for q in query])
+        return self.chain.invoke({"query": query})
 
-def create_qa_toolkits(qa_chain: Runnable, name: str = None, description: str = None) -> List[AskDocumentTool]:
-    return [AskDocumentTool(qa_chain, name, description)]
+def create_qa_toolkits(chain: Runnable, name: str = None, description: str = None) -> List[AskDocumentTool]:
+    return [AskDocumentTool(chain=qa_chain, name=name, description=description)]
```

### Comparing `textlong-0.1.8/textlong/serialize.py` & `textlong-0.2.1/textlong/tree/serialize.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/state.py` & `textlong-0.2.1/textlong/tree/state.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/tree.py` & `textlong-0.2.1/textlong/tree/tree.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.8/textlong/writing.py` & `textlong-0.2.1/textlong/tree/writing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     is_content_exist,
     is_prompts_exist,
     load_content,
     save_content,
     load_prompts,
     save_prompts,
 )
-from .prompts.hub import load_chat_prompt, save_chat_prompt
+from ..hub import load_chat_prompt, save_chat_prompt
 
 class WritingTask(BaseCommand):
     """
     长文写作任务。
     """
 
     def __init__(self, project_id: str=None, llm=None, user_id="default_user"):
```

### Comparing `textlong-0.1.8/PKG-INFO` & `textlong-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textlong
-Version: 0.1.8
+Version: 0.2.1
 Summary: A framework designed to produce long-texts with GPT or other large language models.
 Home-page: https://github.com/arcstep/textlong
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,15 @@
 from dotenv import load_dotenv, find_dotenv
 load_dotenv(find_dotenv(), override=True)
 ```
 
 **2. 创建`WritingTask`实例：**
 
 ```python
-from textlong import WritingTask
+from textlong.tree import WritingTask
 from langchain_openai import ChatOpenAI
 
 task = WritingTask(llm=ChatOpenAI())
 ```
 
 **3. 使用`auto_write`方法自动生成一段长文：**
```

