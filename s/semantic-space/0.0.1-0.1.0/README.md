# Comparing `tmp/semantic_space-0.0.1.tar.gz` & `tmp/semantic_space-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_space-0.0.1.tar", max compression
+gzip compressed data, was "semantic_space-0.1.0.tar", max compression
```

## Comparing `semantic_space-0.0.1.tar` & `semantic_space-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0     1068 2024-05-25 10:24:47.840448 semantic_space-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      613 2024-05-26 20:06:51.257200 semantic_space-0.0.1/README.md
--rw-r--r--   0        0        0      563 2024-05-26 20:06:51.253686 semantic_space-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-26 19:40:02.870876 semantic_space-0.0.1/semantic_space/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 09:58:35.728018 semantic_space-0.0.1/semantic_space/models/__init__.py
--rw-r--r--   0        0        0     6994 2024-05-26 19:28:39.850331 semantic_space-0.0.1/semantic_space/models/grams.py
--rw-r--r--   0        0        0        0 2024-05-25 09:57:09.699010 semantic_space-0.0.1/semantic_space/tools/__init__.py
--rw-r--r--   0        0        0     9221 2024-05-26 19:17:02.217015 semantic_space-0.0.1/semantic_space/tools/preprocessing.py
--rw-r--r--   0        0        0    15744 2024-05-26 15:32:00.201400 semantic_space-0.0.1/semantic_space/tools/tokens.py
--rw-r--r--   0        0        0        0 2024-05-25 10:39:29.284710 semantic_space-0.0.1/semantic_space/utils/__init__.py
--rw-r--r--   0        0        0      312 2024-05-26 19:28:39.853965 semantic_space-0.0.1/semantic_space/utils/exceptions.py
--rw-r--r--   0        0        0      984 2024-05-26 15:32:00.192645 semantic_space-0.0.1/semantic_space/utils/types.py
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 semantic_space-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-25 10:24:47.840448 semantic_space-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      613 2024-05-26 20:12:48.743416 semantic_space-0.1.0/README.md
+-rw-r--r--   0        0        0      563 2024-06-02 13:52:09.158353 semantic_space-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-26 19:40:02.870876 semantic_space-0.1.0/semantic_space/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 09:58:35.728018 semantic_space-0.1.0/semantic_space/models/__init__.py
+-rw-r--r--   0        0        0     2516 2024-06-02 13:51:14.179855 semantic_space-0.1.0/semantic_space/models/embeddings.py
+-rw-r--r--   0        0        0     7000 2024-05-26 20:16:18.845084 semantic_space-0.1.0/semantic_space/models/grams.py
+-rw-r--r--   0        0        0        0 2024-05-25 09:57:09.699010 semantic_space-0.1.0/semantic_space/tools/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-26 20:24:49.000134 semantic_space-0.1.0/semantic_space/tools/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    20619 2024-05-26 20:25:28.734489 semantic_space-0.1.0/semantic_space/tools/__pycache__/tokens.cpython-312.pyc
+-rw-r--r--   0        0        0     9223 2024-05-26 20:16:18.849739 semantic_space-0.1.0/semantic_space/tools/preprocessing.py
+-rw-r--r--   0        0        0    15748 2024-05-26 20:16:18.840239 semantic_space-0.1.0/semantic_space/tools/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-25 10:39:29.284710 semantic_space-0.1.0/semantic_space/utils/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-26 20:25:28.924321 semantic_space-0.1.0/semantic_space/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1125 2024-05-26 20:25:28.925044 semantic_space-0.1.0/semantic_space/utils/__pycache__/exceptions.cpython-312.pyc
+-rw-r--r--   0        0        0     1338 2024-05-26 20:25:28.925721 semantic_space-0.1.0/semantic_space/utils/__pycache__/types.cpython-312.pyc
+-rw-r--r--   0        0        0      312 2024-05-26 19:28:39.853965 semantic_space-0.1.0/semantic_space/utils/exceptions.py
+-rw-r--r--   0        0        0      352 2024-06-02 13:48:17.837128 semantic_space-0.1.0/semantic_space/utils/log.py
+-rw-r--r--   0        0        0      984 2024-05-26 15:32:00.192645 semantic_space-0.1.0/semantic_space/utils/types.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 semantic_space-0.1.0/PKG-INFO
```

### Comparing `semantic_space-0.0.1/LICENSE.txt` & `semantic_space-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semantic_space-0.0.1/README.md` & `semantic_space-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# sematnic-space
+# semantic-space
 
 A basic NLP library for modelization and tokenization.
 
 _pip install semantic-space_
 
 ## Project Details
```

### Comparing `semantic_space-0.0.1/pyproject.toml` & `semantic_space-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "semantic-space"
-version = "0.0.1"
+version = "0.1.0"
 description = "A basic NLP library for modelization and tokenization."
 authors = ["Ahmet Erdem <ahmetblk1035@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ahmeterdem1/semantic-space"
 keywords = ["NLP", "Natural Language Processing", "library"]
```

### Comparing `semantic_space-0.0.1/semantic_space/models/grams.py` & `semantic_space-0.1.0/semantic_space/models/grams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     NGram class for n-gram models.
 """
 
-from tools import tokens
-from utils.exceptions import *
-from utils.types import *
+from ..tools import tokens
+from ..utils.exceptions import *
+from ..utils.types import *
 from typing import Union, List
 from numpy import log, exp
 from struct import pack, unpack
 from zlib import compress, decompress
 
 # Will only accept ordered tokens
 class NGram:
```

### Comparing `semantic_space-0.0.1/semantic_space/tools/preprocessing.py` & `semantic_space-0.1.0/semantic_space/tools/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from tokenizers import Tokenizer
 from os import walk
 from os.path import join
 from re import search
 from zlib import compress, decompress
 from typing import List, Union
-from utils.exceptions import *
+from ..utils.exceptions import *
 
 
 DELIMITER = "\x00\x11\x22\x33\x44\x55".encode("utf-8")
 PATTERN = r'^[0-9]{1,2}\.[0-9]{1,2}\.[0-9]{4} [0-9]{,2}:[0-9]{,2} - ([^:]*): '  # Yes.
 DATE_FORMAT = "%d.%m.%Y %H:%M"
 
 def tokenize(textfile: str, tokenizer: Tokenizer, ids: bool = False) -> List[Union[str, int]]:
```

### Comparing `semantic_space-0.0.1/semantic_space/tools/tokens.py` & `semantic_space-0.1.0/semantic_space/tools/tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from struct import pack, unpack
 from zlib import compress, decompress
 from dataclasses import dataclass
 from typing import Union, List, Tuple
 from os.path import abspath
 import numpy as np
-from utils.exceptions import *
-from utils.types import *
+from ..utils.exceptions import *
+from ..utils.types import *
 
 @dataclass
 class utoken16:
     """
         Unordered token type of size 16-bit. Holds the information
         for the amount that the token appears in a given text, and
         the id of the token.
```

### Comparing `semantic_space-0.0.1/semantic_space/utils/types.py` & `semantic_space-0.1.0/semantic_space/utils/types.py`

 * *Files identical despite different names*

### Comparing `semantic_space-0.0.1/PKG-INFO` & `semantic_space-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-space
-Version: 0.0.1
+Version: 0.1.0
 Summary: A basic NLP library for modelization and tokenization.
 Home-page: https://github.com/ahmeterdem1/semantic-space
 License: MIT
 Keywords: NLP,Natural Language Processing,library
 Author: Ahmet Erdem
 Author-email: ahmetblk1035@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: tokenizers (>=0.15.0,<0.16.0)
 Project-URL: Repository, https://github.com/ahmeterdem1/semantic-space
 Description-Content-Type: text/markdown
 
-# sematnic-space
+# semantic-space
 
 A basic NLP library for modelization and tokenization.
 
 _pip install semantic-space_
 
 ## Project Details
```

