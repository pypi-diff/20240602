# Comparing `tmp/fast_mime-0.1.0.tar.gz` & `tmp/fast_mime-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_mime-0.1.0.tar", max compression
+gzip compressed data, was "fast_mime-0.1.1.tar", max compression
```

## Comparing `fast_mime-0.1.0.tar` & `fast_mime-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      370 2024-05-17 10:40:31.059708 fast_mime-0.1.0/README.md
--rw-r--r--   0        0        0    19369 2024-05-17 10:47:19.298638 fast_mime-0.1.0/fast_mime/__init__.py
--rw-r--r--   0        0        0     4337 2024-05-17 09:09:07.773517 fast_mime-0.1.0/fast_mime/data/custom.xml
--rw-r--r--   0        0        0     8920 2024-05-17 08:39:44.876303 fast_mime-0.1.0/fast_mime/data/patch.json
--rw-r--r--   0        0        0   279488 2024-05-17 09:14:27.010711 fast_mime-0.1.0/fast_mime/data/tika.xml
--rw-r--r--   0        0        0      425 2024-05-17 10:47:29.200569 fast_mime-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 fast_mime-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-18 10:51:46.909341 fast_mime-0.1.1/LICENSE
+-rw-r--r--   0        0        0      660 2024-05-18 10:49:58.830749 fast_mime-0.1.1/README.md
+-rw-r--r--   0        0        0    19586 2024-06-02 08:46:28.396571 fast_mime-0.1.1/fast_mime/__init__.py
+-rw-r--r--   0        0        0     4337 2024-05-17 09:09:07.773517 fast_mime-0.1.1/fast_mime/data/custom.xml
+-rw-r--r--   0        0        0     8920 2024-05-17 08:39:44.876303 fast_mime-0.1.1/fast_mime/data/patch.json
+-rw-r--r--   0        0        0   279488 2024-05-17 09:14:27.010711 fast_mime-0.1.1/fast_mime/data/tika.xml
+-rw-r--r--   0        0        0      425 2024-06-02 08:46:08.085994 fast_mime-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 fast_mime-0.1.1/PKG-INFO
```

### Comparing `fast_mime-0.1.0/fast_mime/__init__.py` & `fast_mime-0.1.1/fast_mime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from functools import cached_property
 import json
 import os
 from pathlib import Path
 import re
-from typing import IO, Dict, List, Tuple
+from typing import IO, Any, Dict, Generator, List, Tuple
 import xml.etree.ElementTree as ET
 
 from typing import TypeVar
 import logging
 
 logger = logging.getLogger("fast-mime")
 
@@ -360,14 +360,17 @@
         self._extensions = self._build_extensions()
         self._type_exts = self._build_type_exts()
         self._type_mime = self._build_type_mime()
         self._magics = self._build_magics()
         self._bytes_end = max([magic.bytes_end for magic, _ in self._magics], default=0)
         self._patch()
 
+    def exts_of(self, content_type: str) -> List[str] | None:
+        return self._type_exts.get(content_type)
+
     @classmethod
     def _default_patch_file(cls) -> str:
         return os.path.join(os.path.dirname(__file__), "data", "patch.json")
 
     def _patch(self):
         with open(self._default_patch_file()) as fi:
             patches = json.load(fi)
@@ -588,16 +591,18 @@
         if content_type:
             result = CONTENT_TYPE_SPLITTER.split(content_type.lower(), 1)[0]
             if result and result.find("/") > 0:
                 return result
         return None
 
     @contextmanager
-    def _with_io(self, pathname_or_io: Path | str | IO[bytes]):
-        if isinstance(pathname_or_io, IO):
+    def _with_io(
+        self, pathname_or_io: Path | str | IO[bytes]
+    ) -> Generator[IO[bytes], Any, None]:
+        if isinstance(pathname_or_io, Path) or isinstance(pathname_or_io, str):
+            with open(pathname_or_io, "rb") as fi:
+                yield fi
+        else:
             yield pathname_or_io
-            return
-        with open(pathname_or_io, "rb") as fi:
-            yield fi
 
 
 MIME = Mime.from_xmls()
```

### Comparing `fast_mime-0.1.0/fast_mime/data/custom.xml` & `fast_mime-0.1.1/fast_mime/data/custom.xml`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.0/fast_mime/data/patch.json` & `fast_mime-0.1.1/fast_mime/data/patch.json`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.0/fast_mime/data/tika.xml` & `fast_mime-0.1.1/fast_mime/data/tika.xml`

 * *Files identical despite different names*

### Comparing `fast_mime-0.1.0/PKG-INFO` & `fast_mime-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-mime
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Chongchen Chen
 Author-email: chenkovsky@qq.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -12,22 +12,47 @@
 
 # Fast MIME
 
 Support Rails/[Marcel](https://github.com/rails/marcel) style MIME for Python.
 
 It uses Apache Tike's rule.
 
+It's customizable.
+
 ## Install
 
 ```bash
 pip install fast-mime
 ```
 
 ## Usage
 
+### Detect MIME
+
 ```python
 from fast_mime import MIME
 with open("a.pdf") as fi:
     mime = MIME(file=fi, name="a.pdf", declared_type="application/pdf", extension=".pdf")
     # all parameters are optional
+
+```
+
+### Customize MIME rules
+
+```python
+from fast_mime import Mime
+
+# define your own mime rule
+MIME = Mime.from_xmls(your_rule_file_name)
+```
+
+### Patch MIME
+
+```python
+
+class MyMime(Mime):
+    def _patch(self):
+        super()._patch()
+        ...
+
 ```
```

