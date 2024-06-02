# Comparing `tmp/schemafunc-0.3.7.tar.gz` & `tmp/schemafunc-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemafunc-0.3.7.tar", max compression
+gzip compressed data, was "schemafunc-0.3.8.tar", max compression
```

## Comparing `schemafunc-0.3.7.tar` & `schemafunc-0.3.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.7/LICENSE
--rw-r--r--   0        0        0     1140 2024-05-30 22:46:14.259054 schemafunc-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.7/README.md
--rw-r--r--   0        0        0    21542 2024-05-30 22:44:02.104024 schemafunc-0.3.7/src/schemafunc.py
--rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-11 16:31:26.401239 schemafunc-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1140 2024-05-30 23:15:25.008074 schemafunc-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6614 2024-04-14 16:41:56.673792 schemafunc-0.3.8/README.md
+-rw-r--r--   0        0        0    22847 2024-05-30 23:13:53.862529 schemafunc-0.3.8/src/schemafunc.py
+-rw-r--r--   0        0        0     7626 1970-01-01 00:00:00.000000 schemafunc-0.3.8/PKG-INFO
```

### Comparing `schemafunc-0.3.7/LICENSE` & `schemafunc-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.7/pyproject.toml` & `schemafunc-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemafunc"
-version = "0.3.7"
+version = "0.3.8"
 description = "Python function-to-LLM tool maker."
 authors = ["Dustin Wyatt <dustin.wyatt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dmwyatt/schemafunc"
 
 keywords = ["python", "openai", "llm", "language-model", "schema", "function", "tool"]
```

### Comparing `schemafunc-0.3.7/README.md` & `schemafunc-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `schemafunc-0.3.7/src/schemafunc.py` & `schemafunc-0.3.8/src/schemafunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,16 +319,16 @@
 
 
 def resolve_type(param_type: typing.Type) -> dict:
     """
     Resolves a Python type into a JSON Schema dictionary.
 
     This function takes a Python type (such as `int`, `str`, `typing.Union`,
-    `typing.List`, `typing.Dict`, etc.) and returns a dictionary representing the
-    equivalent JSON Schema type.
+    `typing.List`, `typing.Dict`, `typing.TypedDict`, etc.) and returns a dictionary
+    representing the equivalent JSON Schema type.
 
     Args:
         param_type (typing.Type): The Python type to resolve.
 
     Returns:
         dict: A dictionary representing the JSON Schema equivalent of the input type.
 
@@ -344,14 +344,21 @@
 
         >>> resolve_type(typing.Union[int, str])
         {'type': ['integer', 'string']}
 
         >>> resolve_type(typing.Dict[str, int])
         {'type': 'object', 'additionalProperties': {'type': 'integer'}}
 
+        >>> class MyTypedDict(TypedDict):
+        ...     name: str
+        ...     age: int
+        ...
+        >>> resolve_type(MyTypedDict)
+        {'type': 'object', 'properties': {'name': {'type': 'string'}, 'age': {'type': 'integer'}}, 'required': ['name', 'age'], 'additionalProperties': False}
+
     The function supports the following types:
 
     - Basic types (`int`, `float`, `str`, `bool`, `None`): These are converted to the
       corresponding JSON Schema types (`'integer'`, `'number'`, `'string'`,
       `'boolean'`, `'null'`).
 
     - Union types (`typing.Union`): These are converted to a JSON Schema type array,
@@ -363,27 +370,35 @@
 
     - Literal types (`typing.Literal`): These are converted to a JSON Schema
       `'string'` type, with an `enum` property listing the permitted literal values.
 
     - Dictionary types (`typing.Dict`): These are converted to a JSON Schema
       `'object'` type, with the `additionalProperties` property representing the
       type of the dictionary values.
+
+    - TypedDict types (`typing.TypedDict`): These are converted to a JSON Schema
+      `'object'` type, with the `properties` property representing the fields of the
+      TypedDict and their types, the `required` property listing the required fields,
+      and `additionalProperties` set to `False`.
     """
     if param_type is typing.Any:
         return {}
     if is_basic_type(param_type):
         return resolve_basic_type(param_type)
     elif is_union_type(param_type):
         return resolve_union_type(param_type)
     elif is_array_type(param_type):
         return resolve_array_type(param_type)
     elif is_literal_type(param_type):
         return resolve_literal_type(param_type)
+    elif is_typed_dict(param_type):
+        return resolve_typed_dict(param_type)
     elif is_dict_type(param_type):
         return resolve_dict_type(param_type)
+
     else:
         raise UnsupportedTypeError(f"Unsupported type: {param_type}")
 
 
 def is_basic_type(param_type: typing.Type) -> bool:
     return param_type in JSON_SCHEMA_TYPES
 
@@ -614,7 +629,26 @@
     key_type, value_type = typing.get_args(param_type)
     if key_type != str:
         raise UnsupportedTypeError(f"Dictionary keys must be strings, not {key_type}")
     return {
         "type": "object",
         "additionalProperties": resolve_type(value_type),
     }
+
+
+def is_typed_dict(param_type: typing.Type) -> bool:
+    return isinstance(param_type, typing._TypedDictMeta)
+
+
+def resolve_typed_dict(param_type: typing.Type[typing.TypedDict]) -> dict:
+    properties = {}
+    required = []
+    for field_name, field_type in param_type.__annotations__.items():
+        properties[field_name] = resolve_type(field_type)
+        if field_name in param_type.__required_keys__:
+            required.append(field_name)
+    return {
+        "type": "object",
+        "properties": properties,
+        "required": required,
+        "additionalProperties": False,
+    }
```

### Comparing `schemafunc-0.3.7/PKG-INFO` & `schemafunc-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemafunc
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python function-to-LLM tool maker.
 Home-page: https://github.com/dmwyatt/schemafunc
 License: MIT
 Keywords: python,openai,llm,language-model,schema,function,tool
 Author: Dustin Wyatt
 Author-email: dustin.wyatt@gmail.com
 Requires-Python: >=3.10.11,<4.0.0
```

