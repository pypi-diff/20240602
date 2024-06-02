# Comparing `tmp/clonellm-0.0.3.tar.gz` & `tmp/clonellm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonellm-0.0.3.tar", max compression
+gzip compressed data, was "clonellm-0.0.4.tar", max compression
```

## Comparing `clonellm-0.0.3.tar` & `clonellm-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2024-06-01 01:45:57.209604 clonellm-0.0.3/LICENSE
--rw-r--r--   0        0        0     9851 2024-06-01 01:45:57.209604 clonellm-0.0.3/README.md
--rw-r--r--   0        0        0     1326 2024-06-01 01:45:57.213604 clonellm-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      209 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/__init__.py
--rw-r--r--   0        0        0      745 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/_base.py
--rw-r--r--   0        0        0     1525 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/_prompt.py
--rw-r--r--   0        0        0     1217 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/_typing.py
--rw-r--r--   0        0        0     9553 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/core.py
--rw-r--r--   0        0        0     3220 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/embed.py
--rw-r--r--   0        0        0     1205 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/memory.py
--rw-r--r--   0        0        0        0 2024-06-01 01:45:57.213604 clonellm-0.0.3/src/clonellm/py.typed
--rw-r--r--   0        0        0    10693 1970-01-01 00:00:00.000000 clonellm-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-02 12:57:48.955288 clonellm-0.0.4/LICENSE
+-rw-r--r--   0        0        0     9851 2024-06-02 12:57:48.955288 clonellm-0.0.4/README.md
+-rw-r--r--   0        0        0     1326 2024-06-02 12:57:48.959288 clonellm-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      209 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/__init__.py
+-rw-r--r--   0        0        0      745 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/_base.py
+-rw-r--r--   0        0        0     1525 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/_prompt.py
+-rw-r--r--   0        0        0     1217 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/_typing.py
+-rw-r--r--   0        0        0     9909 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/core.py
+-rw-r--r--   0        0        0     3220 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/embed.py
+-rw-r--r--   0        0        0     1205 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/memory.py
+-rw-r--r--   0        0        0        0 2024-06-02 12:57:48.959288 clonellm-0.0.4/src/clonellm/py.typed
+-rw-r--r--   0        0        0    10693 1970-01-01 00:00:00.000000 clonellm-0.0.4/PKG-INFO
```

### Comparing `clonellm-0.0.3/LICENSE` & `clonellm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.3/README.md` & `clonellm-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 </h1>
 <p align="center">
     <p align="center">Create an AI clone of yourself using LLMs.</p>
 </p>   
 
 <h4 align="center">
     <a href="https://pypi.org/project/clonellm/" target="_blank">
-        <img src="https://img.shields.io/badge/release-v0.0.3-green" alt="Latest Release">
+        <img src="https://img.shields.io/badge/release-v0.0.4-green" alt="Latest Release">
     </a>
     <a href="https://pypi.org/project/clonellm/" target="_blank">
         <img src="https://img.shields.io/pypi/v/clonellm.svg" alt="PyPI Version">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" alt="Python Versions">
     </a>
@@ -277,15 +277,15 @@
 - [ ] Add support for RAG with no embedding (ingest the entire context into the prompt)
 - [x] Add support for string documents
 - [x] Fix mypy errors
 - [x] Rename `completion` methods to `invoke`
 - [x] Add support for streaming completion
 - [ ] Add support for custom system prompts
 - [x] Make `LiteLLMEmbeddings.all_embedding_models` a property
-- [ ] Add an attribute to `CloneLLM` to return supported models
+- [x] Add an attribute to `CloneLLM` to return supported models
 - [x] Add initial version of README
 - [ ] Describe `CloneLLM.clear_memory` method in README
 - [ ] Add documents
 - [x] Add usage examples
 - [x] Add unit tests for non-core modules
 - [ ] Add unit tests for core module
 - [x] Add GitHub workflow to run tests on PR
```

#### html2text {}

```diff
@@ -108,13 +108,13 @@
 LinkedIn or other social platforms. Thank you for your interest in CloneLLM. We
 look forward to seeing what you'll create with your AI clone! ## TODO - [x] Add
 pre commit configuration file - [x] Add setup.py script - [x] Add support for
 conversation history - [ ] Add support for RAG with no embedding (ingest the
 entire context into the prompt) - [x] Add support for string documents - [x]
 Fix mypy errors - [x] Rename `completion` methods to `invoke` - [x] Add support
 for streaming completion - [ ] Add support for custom system prompts - [x] Make
-`LiteLLMEmbeddings.all_embedding_models` a property - [ ] Add an attribute to
+`LiteLLMEmbeddings.all_embedding_models` a property - [x] Add an attribute to
 `CloneLLM` to return supported models - [x] Add initial version of README - [ ]
 Describe `CloneLLM.clear_memory` method in README - [ ] Add documents - [x] Add
 usage examples - [x] Add unit tests for non-core modules - [ ] Add unit tests
 for core module - [x] Add GitHub workflow to run tests on PR - [x] Add GitHub
 workflow to publish to PyPI on release
```

### Comparing `clonellm-0.0.3/pyproject.toml` & `clonellm-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "clonellm"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python package to create an AI clone of yourself using LLMs."
 packages = [{ from = "src", include = "clonellm" }]
 license = "MIT"
 authors = ["Mehdi Samsami <mehdisamsami@live.com>"]
 readme = "README.md"
 keywords = ["llm", "language models", "nlp", "rag", "ai", "ai clone"]
 repository = "https://github.com/msamsami/clonellm"
```

### Comparing `clonellm-0.0.3/src/clonellm/_base.py` & `clonellm-0.0.4/src/clonellm/_base.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.3/src/clonellm/_prompt.py` & `clonellm-0.0.4/src/clonellm/_prompt.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.3/src/clonellm/_typing.py` & `clonellm-0.0.4/src/clonellm/_typing.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.3/src/clonellm/core.py` & `clonellm-0.0.4/src/clonellm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from langchain_core.embeddings import Embeddings
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.runnables import RunnablePassthrough, RunnableSerializable
 from langchain_core.runnables.history import RunnableWithMessageHistory
 from langchain_core.vectorstores import VectorStoreRetriever
 from langchain_community.chat_models import ChatLiteLLM
 from langchain_community.vectorstores import Chroma
+from litellm import models_by_provider
 
 from ._base import LiteLLMMixin
 from ._prompt import context_prompt, user_profile_prompt, history_prompt, question_prompt
 from ._typing import UserProfile
 from .embed import LiteLLMEmbeddings
 from .memory import get_session_history, clear_session_history
 
@@ -42,15 +43,16 @@
     """
 
     __is_fitted: bool = False
     _splitter: TextSplitter
     _session_id: str
     db: Chroma
 
-    _CHROMA_COLLECTION_NAME = "clonellm"
+    _VECTOR_STORE_COLLECTION_NAME = "clonellm"
+    _TEXT_SPLITTER_CHUNK_SIZE = 2000
 
     def __init__(
         self,
         model: str,
         documents: list[Document | str],
         embedding: LiteLLMEmbeddings | Embeddings,
         user_profile: Optional[UserProfile | dict[str, Any] | str] = None,
@@ -64,15 +66,15 @@
         self.user_profile = user_profile
         self.memory = memory
         self._internal_init()
 
     def _internal_init(self) -> None:
         self._litellm_kwargs.update({f"{self._llm_provider}_api_key": self.api_key})
         self._llm = ChatLiteLLM(model=self.model, model_name=self.model, **self._litellm_kwargs)
-        self._splitter = CharacterTextSplitter(chunk_size=2000, chunk_overlap=100)
+        self._splitter = CharacterTextSplitter(chunk_size=self._TEXT_SPLITTER_CHUNK_SIZE, chunk_overlap=100)
         self._session_id = str(uuid.uuid4())
         self.clear_memory()
 
     @classmethod
     def from_persist_directory(
         cls,
         persist_directory: str,
@@ -80,15 +82,15 @@
         embedding: LiteLLMEmbeddings | Embeddings,
         user_profile: Optional[UserProfile | dict[str, Any] | str] = None,
         memory: Optional[bool] = None,
         api_key: Optional[str] = None,
         **kwargs: Any,
     ) -> Self:
         cls.db = Chroma(
-            collection_name=cls._CHROMA_COLLECTION_NAME, embedding_function=embedding, persist_directory=persist_directory
+            collection_name=cls._VECTOR_STORE_COLLECTION_NAME, embedding_function=embedding, persist_directory=persist_directory
         )
         cls.__is_fitted = True
         return cls(
             model=model, documents=[], embedding=embedding, user_profile=user_profile, memory=memory, api_key=api_key, **kwargs
         )
 
     def _get_documents(self, documents: Optional[list[Document | str]] = None) -> list[Document]:
@@ -98,27 +100,32 @@
                 raise ValueError(f"item at index {i} is not a valid Document or a string")
             documents_.append(Document(page_content=doc) if isinstance(doc, str) else doc)
         return documents_
 
     def fit(self) -> Self:
         documents = self._get_documents()
         documents = self._splitter.split_documents(documents)
-        self.db = Chroma.from_documents(documents, self.embedding, collection_name=self._CHROMA_COLLECTION_NAME)
+        self.db = Chroma.from_documents(documents, self.embedding, collection_name=self._VECTOR_STORE_COLLECTION_NAME)
         self.__is_fitted = True
         return self
 
     async def afit(self) -> Self:
         documents = self._get_documents()
         documents = self._splitter.split_documents(documents)
-        self.db = await Chroma.afrom_documents(documents, self.embedding, collection_name=self._CHROMA_COLLECTION_NAME)
+        self.db = await Chroma.afrom_documents(documents, self.embedding, collection_name=self._VECTOR_STORE_COLLECTION_NAME)
         self.__is_fitted = True
         return self
 
     def _check_is_fitted(self, from_update: bool = False) -> None:
-        if not self.__is_fitted or self.db is None or ((self._splitter is None) if from_update else False):
+        if (
+            not self.__is_fitted
+            or not hasattr(self, "db")
+            or self.db is None
+            or ((not hasattr(self, "_splitter") or self._splitter is None) if from_update else False)
+        ):
             raise AttributeError("This CloneLLM instance is not fitted yet. Call `fit` using this method.")
 
     def update(
         self,
         documents: list[Document | str],
     ) -> Self:
         self._check_is_fitted(from_update=True)
@@ -175,54 +182,58 @@
         )
 
     def invoke(self, prompt: str) -> str:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             response = rag_chain_with_history.invoke({"input": prompt}, config={"configurable": {"session_id": self._session_id}})
-            return cast(str, response.content)
+            return cast(str, response)
         rag_chain = self._get_rag_chain()
         return rag_chain.invoke(prompt)
 
     async def ainvoke(self, prompt: str) -> str:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             response = await rag_chain_with_history.ainvoke(
                 {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
             )
-            return cast(str, response.content)
+            return cast(str, response)
         rag_chain = self._get_rag_chain()
         return await rag_chain.ainvoke(prompt)
 
     def stream(self, prompt: str) -> Iterator[str]:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             for chunk in rag_chain_with_history.stream(
                 {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
             ):
-                yield chunk.content
+                yield chunk
         else:
             rag_chain = self._get_rag_chain()
             for chunk in rag_chain.stream(prompt):
                 yield chunk
 
     async def astream(self, prompt: str) -> AsyncIterator[str]:
         self._check_is_fitted()
         if self.memory:
             rag_chain_with_history = self._get_rag_chain_with_history()
             async for chunk in rag_chain_with_history.astream(
                 {"input": prompt}, config={"configurable": {"session_id": self._session_id}}
             ):
-                yield chunk.content
+                yield chunk
         else:
             rag_chain = self._get_rag_chain()
             async for chunk in rag_chain.astream(prompt):
                 yield chunk
 
     def clear_memory(self) -> None:
         clear_session_history(self._session_id)
         self._session_id = str(uuid.uuid4())
 
+    @property
+    def models_by_provider(self) -> dict[str, list[str]]:
+        return cast(dict[str, list[str]], models_by_provider)
+
     def __repr__(self) -> str:
-        return f"CloneLLM<(model='{self.model}', memory={self.memory})>"
+        return f"CloneLLM<(model='{self.model}', memory={bool(self.memory)})>"
```

### Comparing `clonellm-0.0.3/src/clonellm/embed.py` & `clonellm-0.0.4/src/clonellm/embed.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.3/src/clonellm/memory.py` & `clonellm-0.0.4/src/clonellm/memory.py`

 * *Files identical despite different names*

### Comparing `clonellm-0.0.3/PKG-INFO` & `clonellm-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonellm
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package to create an AI clone of yourself using LLMs.
 Home-page: https://github.com/msamsami/clonellm
 License: MIT
 Keywords: llm,language models,nlp,rag,ai,ai clone
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Requires-Python: >=3.9,<3.13
@@ -28,15 +28,15 @@
 </h1>
 <p align="center">
     <p align="center">Create an AI clone of yourself using LLMs.</p>
 </p>   
 
 <h4 align="center">
     <a href="https://pypi.org/project/clonellm/" target="_blank">
-        <img src="https://img.shields.io/badge/release-v0.0.3-green" alt="Latest Release">
+        <img src="https://img.shields.io/badge/release-v0.0.4-green" alt="Latest Release">
     </a>
     <a href="https://pypi.org/project/clonellm/" target="_blank">
         <img src="https://img.shields.io/pypi/v/clonellm.svg" alt="PyPI Version">
     </a>
     <a target="_blank">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" alt="Python Versions">
     </a>
@@ -299,15 +299,15 @@
 - [ ] Add support for RAG with no embedding (ingest the entire context into the prompt)
 - [x] Add support for string documents
 - [x] Fix mypy errors
 - [x] Rename `completion` methods to `invoke`
 - [x] Add support for streaming completion
 - [ ] Add support for custom system prompts
 - [x] Make `LiteLLMEmbeddings.all_embedding_models` a property
-- [ ] Add an attribute to `CloneLLM` to return supported models
+- [x] Add an attribute to `CloneLLM` to return supported models
 - [x] Add initial version of README
 - [ ] Describe `CloneLLM.clear_memory` method in README
 - [ ] Add documents
 - [x] Add usage examples
 - [x] Add unit tests for non-core modules
 - [ ] Add unit tests for core module
 - [x] Add GitHub workflow to run tests on PR
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clonellm Version: 0.0.3 Summary: Python package to
+Metadata-Version: 2.1 Name: clonellm Version: 0.0.4 Summary: Python package to
 create an AI clone of yourself using LLMs. Home-page: https://github.com/
 msamsami/clonellm License: MIT Keywords: llm,language models,nlp,rag,ai,ai
 clone Author: Mehdi Samsami Author-email: mehdisamsami@live.com Requires-
 Python: >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -120,13 +120,13 @@
 LinkedIn or other social platforms. Thank you for your interest in CloneLLM. We
 look forward to seeing what you'll create with your AI clone! ## TODO - [x] Add
 pre commit configuration file - [x] Add setup.py script - [x] Add support for
 conversation history - [ ] Add support for RAG with no embedding (ingest the
 entire context into the prompt) - [x] Add support for string documents - [x]
 Fix mypy errors - [x] Rename `completion` methods to `invoke` - [x] Add support
 for streaming completion - [ ] Add support for custom system prompts - [x] Make
-`LiteLLMEmbeddings.all_embedding_models` a property - [ ] Add an attribute to
+`LiteLLMEmbeddings.all_embedding_models` a property - [x] Add an attribute to
 `CloneLLM` to return supported models - [x] Add initial version of README - [ ]
 Describe `CloneLLM.clear_memory` method in README - [ ] Add documents - [x] Add
 usage examples - [x] Add unit tests for non-core modules - [ ] Add unit tests
 for core module - [x] Add GitHub workflow to run tests on PR - [x] Add GitHub
 workflow to publish to PyPI on release
```

