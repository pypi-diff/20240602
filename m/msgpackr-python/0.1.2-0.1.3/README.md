# Comparing `tmp/msgpackr_python-0.1.2.tar.gz` & `tmp/msgpackr_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgpackr_python-0.1.2.tar", max compression
+gzip compressed data, was "msgpackr_python-0.1.3.tar", max compression
```

## Comparing `msgpackr_python-0.1.2.tar` & `msgpackr_python-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/LICENSE
--rw-r--r--   0        0        0       76 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/README.md
--rwxr-xr-x   0        0        0      147 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/__init__.py
--rwxr-xr-x   0        0        0     1376 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/constants.py
--rwxr-xr-x   0        0        0    10046 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/extension.py
--rw-r--r--   0        0        0        0 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/pack.py
--rwxr-xr-x   0        0        0    17443 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/unpack.py
--rw-r--r--   0        0        0     2143 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 msgpackr_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/LICENSE
+-rw-r--r--   0        0        0       76 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/README.md
+-rwxr-xr-x   0        0        0      158 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/__init__.py
+-rwxr-xr-x   0        0        0     1376 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/constants.py
+-rwxr-xr-x   0        0        0     9901 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/extension.py
+-rw-r--r--   0        0        0        0 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/pack.py
+-rwxr-xr-x   0        0        0    17443 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/msgpackr/unpack.py
+-rw-r--r--   0        0        0     2143 2024-06-01 17:37:35.796431 msgpackr_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 msgpackr_python-0.1.3/PKG-INFO
```

### Comparing `msgpackr_python-0.1.2/LICENSE` & `msgpackr_python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.2/msgpackr/constants.py` & `msgpackr_python-0.1.3/msgpackr/constants.py`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.2/msgpackr/extension.py` & `msgpackr_python-0.1.3/msgpackr/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,21 +271,19 @@
         identifier1 = data[pos]
         if not 0x40 <= identifier1 <= 0x7F:
             raise ValueError(f"Invalid record identifier: {identifier1}")
 
         identifier1 &= 0x3F
 
         if length == 1:
-            print("RecordExtension", identifier1)
             return identifier1
 
         if length == 2:
             identifier2 = data[pos + 1]
             # TODO: do we need to check the range?
-            print("RecordExtension", identifier1, identifier2, identifier2 << 5 + identifier1)
 
             return identifier2 << 5 + identifier1
 
         raise ValueError(f"Invalid record identifier length: {length} bytes")
 
     @classmethod
     def post_unpack(cls, unpacker, data: BytesLike, pos: int, ret: int) -> Tuple[int, Any]:
```

### Comparing `msgpackr_python-0.1.2/msgpackr/unpack.py` & `msgpackr_python-0.1.3/msgpackr/unpack.py`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.2/pyproject.toml` & `msgpackr_python-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msgpackr-python"
-version = "0.1.2"
+version = "0.1.3"
 description = "Re-implementation of kriszyp's msgpackr Javascript module"
 license = "MIT"
 authors = ["Aedial <aedial.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Aedial/msgpackr-python"
 keywords = ["python", "msgpack", "msgpackr"]
 classifiers = [
```

### Comparing `msgpackr_python-0.1.2/PKG-INFO` & `msgpackr_python-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgpackr-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Re-implementation of kriszyp's msgpackr Javascript module
 Home-page: https://github.com/Aedial/msgpackr-python
 License: MIT
 Keywords: python,msgpack,msgpackr
 Author: Aedial
 Author-email: aedial.dev@gmail.com
 Requires-Python: >=3.7.10,<4.0.0
```

