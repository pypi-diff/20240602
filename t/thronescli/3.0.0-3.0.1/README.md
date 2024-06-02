# Comparing `tmp/thronescli-3.0.0.tar.gz` & `tmp/thronescli-3.0.1.tar.gz`

## Comparing `thronescli-3.0.0.tar` & `thronescli-3.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    10294 2020-02-02 00:00:00.000000 thronescli-3.0.0/thronescli.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 thronescli-3.0.0/.gitignore
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 thronescli-3.0.0/LICENSE.txt
--rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 thronescli-3.0.0/README.md
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 thronescli-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    10838 2020-02-02 00:00:00.000000 thronescli-3.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0    10165 2020-02-02 00:00:00.000000 thronescli-3.0.1/thronescli.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 thronescli-3.0.1/.gitignore
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 thronescli-3.0.1/LICENSE.txt
+-rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 thronescli-3.0.1/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 thronescli-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 thronescli-3.0.1/PKG-INFO
```

### Comparing `thronescli-3.0.0/thronescli.py` & `thronescli-3.0.1/thronescli.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     DelimitedText,
     FieldBase,
     Flag,
     JsonLineReader,
     MarkupText,
     MissingField,
     ModelBase,
-    Number,
     Text,
     fieldfilter,
 )
 
 if typing.TYPE_CHECKING:
-    from typing import Iterable
+    from typing import Any, Iterable, Mapping
+    import collections
 
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 
 
 CARDS_URL = "https://thronesdb.com/api/public/cards/"
 CARDS_ENV = "THRONESCLI_DATA"
 
 
 class ThronesReader(JsonLineReader):
@@ -246,27 +246,21 @@
 
 class Loyal(Flag):
     def fetch(self, item: Mapping, default: Any | type = MissingField) -> Any:
         if item["faction_code"] == "neutral":
             raise MissingField("Irrelevant for neutral")
         return super().fetch(item, default)
 
-    def is_missing(self, value: Any) -> bool:
-        return value is False
-
 
 class Unique(Flag):
     def fetch(self, item: Mapping, default: Any | type = MissingField) -> Any:
         if item["type_name"] not in {"Character", "Location", "Attachment"}:
             raise MissingField("Irrelevant for type")
         return super().fetch(item, default)
 
-    def is_missing(self, value: Any) -> bool:
-        return value is False
-
 
 class ThronesModel(ModelBase):
     __version__ = __version__
 
     # Basic card properties
     name = Text(optalias="-n", redirect_args=True)
     traits = DelimitedText(
```

### Comparing `thronescli-3.0.0/README.md` & `thronescli-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `thronescli-3.0.0/pyproject.toml` & `thronescli-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 dependencies = [
     "click",
     "clicksearch",
 ]
 requires-python = ">= 3.6"
 
 [project.optional-dependencies]
-dev = ["black", "twine", "build", "hatchling"]
+dev = ["black", "ruff", "twine", "build", "hatchling"]
 
 [project.scripts]
 thronescli = "thronescli:main"
 
 [project.urls]
 Download = "https://github.com/jimorie/thronescli/archive/v3.0.0.tar.gz"
 Homepage = "https://github.com/jimorie/thronescli"
```

### Comparing `thronescli-3.0.0/PKG-INFO` & `thronescli-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: thronescli
-Version: 3.0.0
+Version: 3.0.1
 Summary: A command line interface for the thronesdb.com card database.
 Project-URL: Download, https://github.com/jimorie/thronescli/archive/v3.0.0.tar.gz
 Project-URL: Homepage, https://github.com/jimorie/thronescli
 Author-email: Petter Nyström <jimorie@gmail.com>
 License-File: LICENSE.txt
 Keywords: game of thrones,thrones,thronesdb.com
 Requires-Python: >=3.6
 Requires-Dist: click
 Requires-Dist: clicksearch
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: hatchling; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 Thrones CLI
 ===========
 
 A command line interface for browsing cards from [A Game of Thrones LCG 2nd Ed](https://www.fantasyflightgames.com/en/products/a-game-of-thrones-the-card-game-second-edition/).
```

