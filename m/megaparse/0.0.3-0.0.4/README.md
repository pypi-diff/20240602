# Comparing `tmp/megaparse-0.0.3.tar.gz` & `tmp/megaparse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megaparse-0.0.3.tar", last modified: Thu May 30 16:23:17 2024, max compression
+gzip compressed data, was "megaparse-0.0.4.tar", last modified: Sun Jun  2 10:23:19 2024, max compression
```

## Comparing `megaparse-0.0.3.tar` & `megaparse-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:17.538246 megaparse-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 16:23:08.000000 megaparse-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-30 16:23:17.538246 megaparse-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-30 16:23:08.000000 megaparse-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:17.534246 megaparse-0.0.3/megaparse/
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/Converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/markdown_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-30 16:23:08.000000 megaparse-0.0.3/megaparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:23:17.538246 megaparse-0.0.3/megaparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 16:23:17.000000 megaparse-0.0.3/megaparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:23:17.538246 megaparse-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-30 16:23:08.000000 megaparse-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:19.574667 megaparse-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 10:23:11.000000 megaparse-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-06-02 10:23:19.574667 megaparse-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-06-02 10:23:11.000000 megaparse-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:19.574667 megaparse-0.0.4/megaparse/
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/markdown_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-02 10:23:11.000000 megaparse-0.0.4/megaparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:23:19.574667 megaparse-0.0.4/megaparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 10:23:19.000000 megaparse-0.0.4/megaparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:23:19.574667 megaparse-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-06-02 10:23:11.000000 megaparse-0.0.4/setup.py
```

### Comparing `megaparse-0.0.3/LICENSE` & `megaparse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.3/PKG-INFO` & `megaparse-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaparse
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parse complex files (PDF,Docx,PPTX) for LLM consumption
 Author: Quivr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-docx
 Requires-Dist: mammoth
 Requires-Dist: python-pptx
@@ -41,36 +41,48 @@
 
 ```bash
 pip install megaparse
 ```
 
 ## Usage
 
-1. Create an account on [Llama Cloud](https://cloud.llamaindex.ai/) and get your API key.
-
-2. Create a new file in the root directory of the project and name it `.env`.
+Add your OpenAI API key to the .env file
 
-3. Add the following line to the `.env` file and replace `llx-your_api_key` with your actual API key.
+```python
+from megaparse import MegaParse
 
-```bash
-LLAMA_CLOUD_API_KEY=llx-your_api_key
+megaparse = MegaParse(file_path="./test.pdf")
+content = megaparse.convert()
+print(content)
+megaparse.save_md(content, "./test.md")
 ```
 
-4. Now you can use the following code to convert a PDF to Markdown and save it to a file.
+### Use LlamaParse
+
+1. Create an account on [Llama Cloud](https://cloud.llamaindex.ai/) and get your API key.
+
+2. Call Megaparse with the `llama_parse_api_key` parameter
 
 ```python
 from megaparse import MegaParse
 
-megaparse = MegaParse(file_path="./test.pdf")
+megaparse = MegaParse(file_path="./test.pdf", llama_parse_api_key="llx-your_api_key")
 content = megaparse.convert()
 print(content)
-megaparse.save_md(content, "./test.md")
 ```
 
+## BenchMark
+
+**Diff megaparse unstructured:** 120
+**Diff llama parse:** 31
+**Diff megaparse llama:** 26
+
+
+*Lower is better*
+
 ## Next Steps
 
-- [ ] Add Unstructured Parser Support
 - [ ] Improve Table Parsing
 - [ ] Improve Image Parsing and description
 - [ ] Add TOC for Docx
 - [ ] Add Hyperlinks for Docx
 - [ ] Order Headers for Docx to Markdown
```

### Comparing `megaparse-0.0.3/README.md` & `megaparse-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,36 +27,48 @@
 
 ```bash
 pip install megaparse
 ```
 
 ## Usage
 
-1. Create an account on [Llama Cloud](https://cloud.llamaindex.ai/) and get your API key.
-
-2. Create a new file in the root directory of the project and name it `.env`.
+Add your OpenAI API key to the .env file
 
-3. Add the following line to the `.env` file and replace `llx-your_api_key` with your actual API key.
+```python
+from megaparse import MegaParse
 
-```bash
-LLAMA_CLOUD_API_KEY=llx-your_api_key
+megaparse = MegaParse(file_path="./test.pdf")
+content = megaparse.convert()
+print(content)
+megaparse.save_md(content, "./test.md")
 ```
 
-4. Now you can use the following code to convert a PDF to Markdown and save it to a file.
+### Use LlamaParse
+
+1. Create an account on [Llama Cloud](https://cloud.llamaindex.ai/) and get your API key.
+
+2. Call Megaparse with the `llama_parse_api_key` parameter
 
 ```python
 from megaparse import MegaParse
 
-megaparse = MegaParse(file_path="./test.pdf")
+megaparse = MegaParse(file_path="./test.pdf", llama_parse_api_key="llx-your_api_key")
 content = megaparse.convert()
 print(content)
-megaparse.save_md(content, "./test.md")
 ```
 
+## BenchMark
+
+**Diff megaparse unstructured:** 120
+**Diff llama parse:** 31
+**Diff megaparse llama:** 26
+
+
+*Lower is better*
+
 ## Next Steps
 
-- [ ] Add Unstructured Parser Support
 - [ ] Improve Table Parsing
 - [ ] Improve Image Parsing and description
 - [ ] Add TOC for Docx
 - [ ] Add Hyperlinks for Docx
 - [ ] Order Headers for Docx to Markdown
```

### Comparing `megaparse-0.0.3/megaparse/Converter.py` & `megaparse-0.0.4/megaparse/Converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 from pptx import Presentation
 from pptx.presentation import Presentation as PresentationObject
 from pptx.enum.shapes import MSO_SHAPE_TYPE
 from typing import List, Set
 from llama_parse import LlamaParse
 from llama_parse.utils import ResultType, Language
 from llama_index.core.schema import Document as LlamaDocument
-from markdown_processor import MarkdownProcessor
+from megaparse.markdown_processor import MarkdownProcessor
+from megaparse.unstructured import UnstructuredParser
+from pathlib import Path
+from llama_index.core import download_loader
+from unstructured.partition.auto import partition
+
 
 import nest_asyncio
 
 nest_asyncio.apply()
 
 
 class Converter:
@@ -197,33 +202,47 @@
     def save_md(self, md_content: str, file_path: Path | str) -> None:
         with open(file_path, "w") as f:
             f.write(md_content)
 
 
 class PDFConverter:
     def __init__(
-        self, api_key: str, handle_pagination: bool = True, handle_header: bool = True
+        self,
+        llama_parse_api_key: str,
+        handle_pagination: bool = True,
+        handle_header: bool = True,
     ) -> None:
         self.handle_pagination = handle_pagination
         self.handle_header = handle_header
-        self.api_key = api_key
+        self.llama_parse_api_key = llama_parse_api_key
 
+    def _llama_parse(self, api_key: str, file_path: str):
         parsing_instructions = "Do not take into account the page breaks (no --- between pages), do not repeat the header and the footer so the tables are merged. Keep the same format for similar tables."
         self.parser = LlamaParse(
             api_key=str(api_key),
             result_type=ResultType.MD,
             gpt4o_mode=True,
             verbose=True,
             language=Language.FRENCH,
             parsing_instruction=parsing_instructions,  # Optionally you can define a parsing instruction
         )
-
-    def convert(self, file_path: str) -> str:
         documents: List[LlamaDocument] = self.parser.load_data(file_path)
         parsed_md = documents[0].get_content()
+        return parsed_md
+
+    def _unstructured_parse(self, file_path: str):
+        unstructured_parser = UnstructuredParser()
+        return unstructured_parser.convert(file_path)
+
+    def convert(self, file_path: str) -> str:
+        parsed_md = ""
+        if self.llama_parse_api_key:
+            parsed_md = self._llama_parse(self.llama_parse_api_key, file_path)
+        else:
+            parsed_md = self._unstructured_parse(file_path)
 
         if not (self.handle_pagination or self.handle_header):
             return parsed_md
         else:
             md_processor = MarkdownProcessor(
                 parsed_md,
                 strict=self.handle_header,
@@ -234,32 +253,33 @@
 
     def save_md(self, md_content: str, file_path: Path | str) -> None:
         with open(file_path, "w") as f:
             f.write(md_content)
 
 
 class MegaParse:
-    def __init__(self, file_path: str) -> None:
+    def __init__(self, file_path: str, llama_parse_api_key: str | None = None) -> None:
         self.file_path = file_path
-        self.api_key = os.getenv("LLAMA_CLOUD_API_KEY")
+        self.llama_parse_api_key = llama_parse_api_key
 
     def convert(self) -> str:
         file_extension: str = os.path.splitext(self.file_path)[1]
 
         if file_extension == ".docx":
             converter = DOCXConverter(
                 file_path=self.file_path, file_extension=file_extension
             )
         elif file_extension == ".pptx":
             converter = PPTXConverter(
                 file_path=self.file_path, file_extension=file_extension
             )
         elif file_extension == ".pdf":
-            converter = PDFConverter(api_key=self.api_key)
+            converter = PDFConverter(llama_parse_api_key=self.llama_parse_api_key)
         else:
             print(self.file_path, file_extension)
             raise ValueError(f"Unsupported file extension: {file_extension}")
         return converter.convert(self.file_path)
 
     def save_md(self, md_content: str, file_path: Path | str) -> None:
-        with open(file_path, "w") as f:
+        os.makedirs(os.path.dirname(file_path), exist_ok=True)
+        with open(file_path, "w+") as f:
             f.write(md_content)
```

### Comparing `megaparse-0.0.3/megaparse/markdown_processor.py` & `megaparse-0.0.4/megaparse/markdown_processor.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.3/megaparse/utils.py` & `megaparse-0.0.4/megaparse/utils.py`

 * *Files identical despite different names*

### Comparing `megaparse-0.0.3/megaparse.egg-info/PKG-INFO` & `megaparse-0.0.4/megaparse.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megaparse
-Version: 0.0.3
+Version: 0.0.4
 Summary: Parse complex files (PDF,Docx,PPTX) for LLM consumption
 Author: Quivr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-docx
 Requires-Dist: mammoth
 Requires-Dist: python-pptx
@@ -41,36 +41,48 @@
 
 ```bash
 pip install megaparse
 ```
 
 ## Usage
 
-1. Create an account on [Llama Cloud](https://cloud.llamaindex.ai/) and get your API key.
-
-2. Create a new file in the root directory of the project and name it `.env`.
+Add your OpenAI API key to the .env file
 
-3. Add the following line to the `.env` file and replace `llx-your_api_key` with your actual API key.
+```python
+from megaparse import MegaParse
 
-```bash
-LLAMA_CLOUD_API_KEY=llx-your_api_key
+megaparse = MegaParse(file_path="./test.pdf")
+content = megaparse.convert()
+print(content)
+megaparse.save_md(content, "./test.md")
 ```
 
-4. Now you can use the following code to convert a PDF to Markdown and save it to a file.
+### Use LlamaParse
+
+1. Create an account on [Llama Cloud](https://cloud.llamaindex.ai/) and get your API key.
+
+2. Call Megaparse with the `llama_parse_api_key` parameter
 
 ```python
 from megaparse import MegaParse
 
-megaparse = MegaParse(file_path="./test.pdf")
+megaparse = MegaParse(file_path="./test.pdf", llama_parse_api_key="llx-your_api_key")
 content = megaparse.convert()
 print(content)
-megaparse.save_md(content, "./test.md")
 ```
 
+## BenchMark
+
+**Diff megaparse unstructured:** 120
+**Diff llama parse:** 31
+**Diff megaparse llama:** 26
+
+
+*Lower is better*
+
 ## Next Steps
 
-- [ ] Add Unstructured Parser Support
 - [ ] Improve Table Parsing
 - [ ] Improve Image Parsing and description
 - [ ] Add TOC for Docx
 - [ ] Add Hyperlinks for Docx
 - [ ] Order Headers for Docx to Markdown
```

