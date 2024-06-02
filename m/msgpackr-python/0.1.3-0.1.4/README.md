# Comparing `tmp/msgpackr_python-0.1.3.tar.gz` & `tmp/msgpackr_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgpackr_python-0.1.3.tar", max compression
+gzip compressed data, was "msgpackr_python-0.1.4.tar", max compression
```

## Comparing `msgpackr_python-0.1.3.tar` & `msgpackr_python-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/LICENSE
--rw-r--r--   0        0        0       76 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/README.md
--rwxr-xr-x   0        0        0      158 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/__init__.py
--rwxr-xr-x   0        0        0     1376 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/constants.py
--rwxr-xr-x   0        0        0     9901 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/extension.py
--rw-r--r--   0        0        0        0 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/pack.py
--rwxr-xr-x   0        0        0    17443 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/unpack.py
--rw-r--r--   0        0        0     2143 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 msgpackr_python-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/LICENSE
+-rw-r--r--   0        0        0       76 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/README.md
+-rwxr-xr-x   0        0        0      158 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/msgpackr/__init__.py
+-rwxr-xr-x   0        0        0     1376 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/msgpackr/constants.py
+-rwxr-xr-x   0        0        0     9901 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/msgpackr/extension.py
+-rw-r--r--   0        0        0        0 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/msgpackr/pack.py
+-rwxr-xr-x   0        0        0    17443 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/msgpackr/unpack.py
+-rw-r--r--   0        0        0     2191 2024-06-02 01:55:53.508016 msgpackr_python-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 msgpackr_python-0.1.4/PKG-INFO
```

### Comparing `msgpackr_python-0.1.3/LICENSE` & `msgpackr_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.3/msgpackr/constants.py` & `msgpackr_python-0.1.4/msgpackr/constants.py`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.3/msgpackr/extension.py` & `msgpackr_python-0.1.4/msgpackr/extension.py`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.3/msgpackr/unpack.py` & `msgpackr_python-0.1.4/msgpackr/unpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
 
         self.check_data_length(end, data)
         if isinstance(data, memoryview):
             return end, data[pos:end].tobytes().decode()
 
         return end, data[pos:end].decode()
 
-    def negative_fixint(self, code: int, _data: BytesLike, pos: int) -> tuple[int, int]:
+    def negative_fixint(self, code: int, _data: BytesLike, pos: int) -> Tuple[int, int]:
         return pos, code - 0x100
 
     CODES_RANGES: Dict[int, Callable[["Unpacker", int, BytesLike, int], Tuple[int, Any]]] = {
         POSITIVE_FIXINT: positive_fixint,
         RECORD: record,
         FIXMAP: fixmap,
         FIXARRAY: fixarray,
```

### Comparing `msgpackr_python-0.1.3/pyproject.toml` & `msgpackr_python-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msgpackr-python"
-version = "0.1.3"
+version = "0.1.4"
 description = "Re-implementation of kriszyp's msgpackr Javascript module"
 license = "MIT"
 authors = ["Aedial <aedial.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Aedial/msgpackr-python"
 keywords = ["python", "msgpack", "msgpackr"]
 classifiers = [
@@ -21,14 +21,15 @@
 [tool.poetry.dependencies]
 python = "^3.7.10"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.21.0"
 pylint = "^2.15.5"
 pytest = "^7.3.1"
+poetry = "=1.5.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
 # patched repo to work with relative links
 myst_parser = {git = "https://github.com/Aedial/MyST-Parser", rev = "adcdb9a"}
 linkify-it-py = "^2.0.0"
 sphinx-copybutton = "^0.5.2"
@@ -71,13 +72,15 @@
 from pylint.config import find_default_config_files
 path.extend(p.parent for p in find_default_config_files())
 """
 
 [tool.pytest.ini_options]
 xfail_strict = true
 empty_parameter_set_mark = "fail_at_collect"
-asyncio_mode = "auto"
 addopts = "--tb=short -vv"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+test = "poetry_scripts:test"
```

### Comparing `msgpackr_python-0.1.3/PKG-INFO` & `msgpackr_python-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgpackr-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Re-implementation of kriszyp's msgpackr Javascript module
 Home-page: https://github.com/Aedial/msgpackr-python
 License: MIT
 Keywords: python,msgpack,msgpackr
 Author: Aedial
 Author-email: aedial.dev@gmail.com
 Requires-Python: >=3.7.10,<4.0.0
```

