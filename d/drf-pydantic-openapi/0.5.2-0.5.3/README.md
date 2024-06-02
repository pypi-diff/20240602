# Comparing `tmp/drf_pydantic_openapi-0.5.2.tar.gz` & `tmp/drf_pydantic_openapi-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic_openapi-0.5.2.tar", max compression
+gzip compressed data, was "drf_pydantic_openapi-0.5.3.tar", max compression
```

## Comparing `drf_pydantic_openapi-0.5.2.tar` & `drf_pydantic_openapi-0.5.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.5.2/LICENSE
--rw-r--r--   0        0        0     2596 2024-01-03 15:57:34.663479 drf_pydantic_openapi-0.5.2/README.md
--rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/__init__.py
--rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/apps.py
--rw-r--r--   0        0        0     1231 2024-03-25 08:02:56.918321 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/errors.py
--rw-r--r--   0        0        0      463 2024-03-22 09:25:15.545564 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/exception_handler.py
--rw-r--r--   0        0        0     6611 2024-03-01 13:37:01.449746 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/generator.py
--rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/path.py
--rw-r--r--   0        0        0      767 2024-03-01 13:37:01.450733 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/ref_source.py
--rw-r--r--   0        0        0     3744 2024-03-14 10:26:02.924573 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/ref_utils.py
--rw-r--r--   0        0        0     1441 2024-03-01 11:53:39.608761 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/settings.py
--rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
--rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
--rw-r--r--   0        0        0      950 2023-09-18 10:02:53.847974 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/swagger.html
--rw-r--r--   0        0        0      246 2023-07-24 13:38:54.240481 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/urls.py
--rw-r--r--   0        0        0     4253 2024-03-25 08:03:02.151629 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/utils.py
--rw-r--r--   0        0        0     2657 2024-02-27 10:01:04.063948 drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/views.py
--rw-r--r--   0        0        0     1250 2024-03-25 08:03:40.496175 drf_pydantic_openapi-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-27 13:44:08.423219 drf_pydantic_openapi-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2596 2024-01-03 15:57:34.663479 drf_pydantic_openapi-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 10:00:59.144732 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-27 14:01:32.336379 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/apps.py
+-rw-r--r--   0        0        0     1231 2024-03-25 08:02:56.918321 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/errors.py
+-rw-r--r--   0        0        0      581 2024-04-05 09:32:25.547118 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/exception_handler.py
+-rw-r--r--   0        0        0     6611 2024-03-01 13:37:01.449746 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/generator.py
+-rw-r--r--   0        0        0     1476 2023-06-02 09:32:06.456794 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/path.py
+-rw-r--r--   0        0        0      778 2024-04-17 14:37:54.568356 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/ref_source.py
+-rw-r--r--   0        0        0     3746 2024-06-02 20:48:28.629869 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/ref_utils.py
+-rw-r--r--   0        0        0     1441 2024-03-01 11:53:39.608761 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/settings.py
+-rw-r--r--   0        0        0      435 2023-06-01 16:41:18.204945 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/rapidoc.html
+-rw-r--r--   0        0        0      534 2023-06-01 15:09:21.868622 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html
+-rw-r--r--   0        0        0      950 2023-09-18 10:02:53.847974 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/swagger.html
+-rw-r--r--   0        0        0      246 2023-07-24 13:38:54.240481 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/urls.py
+-rw-r--r--   0        0        0     5777 2024-04-05 09:31:54.817585 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/utils.py
+-rw-r--r--   0        0        0     2657 2024-02-27 10:01:04.063948 drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/views.py
+-rw-r--r--   0        0        0     1250 2024-04-05 09:32:15.499422 drf_pydantic_openapi-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 drf_pydantic_openapi-0.5.3/PKG-INFO
```

### Comparing `drf_pydantic_openapi-0.5.2/LICENSE` & `drf_pydantic_openapi-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/README.md` & `drf_pydantic_openapi-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/errors.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/errors.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/generator.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/generator.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/path.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/path.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/ref_source.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/ref_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     schemas_: dict = Field(default={}, repr=False)
     components_: dict = Field(default={}, repr=False)
     initialized: bool = Field(default=False, repr=False)
 
     def init(self):
         if self.initialized:
             return
-        r = requests.get(self.url)
+        r = requests.get(self.url, timeout=5)
         data = jsonref.loads(r.text)
         # self.replace_refs_with_empty_dict(data)
         self.schemas_ = data["components"]["schemas"]
         self.components_ = defaultdict(str)
         for k, v in self.schemas_.items():
             self.components_.setdefault(k, v)
         self.initialized = True
```

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/ref_utils.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/ref_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             rename_fields.add(val)
 
     properties = schema["properties"]
     # Find the reference source schema
     if ref_source := config.get_source(model._ref_source):
         ref_component = ref_source.components_[model._ref_model_name]
         if not isinstance(ref_component, dict):
-            logger.debug(f"Can't extend type: {type(ref_component)}")
+            logger.warning(f"Can't extend type: {type(ref_component)}")
             return
 
         ref_component = ref_component.copy()
         ref_properties = ref_component.get("properties", {})
         ref_required = ref_component.get("required", [])
 
         for field in exclude_fields:
```

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/settings.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/settings.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/redoc.html`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/templates/drf_pydantic_openapi/swagger.html` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/templates/drf_pydantic_openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/utils.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import builtins
 import re
+from datetime import date, datetime, time
 from enum import Enum
 from inspect import isclass
+from types import NoneType, UnionType
+from typing import Annotated, Any, get_args, get_origin
+from uuid import UUID
 
 import docstring_parser
-from openapi_pydantic import Parameter, PathItem, Schema
+import openapi_pydantic as openapi
+from openapi_pydantic import Parameter, PathItem
 from openapi_pydantic.util import PydanticSchema
 from pydantic import BaseModel
 from rest_framework import exceptions
 
 from .errors import HttpError
 
 method_mapping = {
@@ -16,23 +21,46 @@
     "post": "create",
     "put": "update",
     "patch": "partial_update",
     "delete": "destroy",
 }
 
 _builtin_openapi_map = {
-    builtins.bool: "boolean",
-    builtins.str: "string",
-    builtins.int: "integer",
-    builtins.float: "number",
+    builtins.bool: openapi.Schema(type=openapi.DataType.BOOLEAN),
+    builtins.str: openapi.Schema(type=openapi.DataType.STRING),
+    builtins.int: openapi.Schema(type=openapi.DataType.INTEGER),
+    builtins.float: openapi.Schema(type=openapi.DataType.NUMBER),
+    datetime: openapi.Schema(type=openapi.DataType.STRING, format="date-time"),
+    date: openapi.Schema(type=openapi.DataType.STRING, format="date"),
+    time: openapi.Schema(type=openapi.DataType.STRING, format="time"),
+    UUID: openapi.Schema(type=openapi.DataType.STRING, format="uuid"),
 }
 
 
-def get_builtin_type(ty: type):
-    return _builtin_openapi_map.get(ty)
+def get_builtin_type(ty: type) -> openapi.Schema | None:
+    ty = get_actual_type(ty)
+    if schema := _builtin_openapi_map.get(ty):
+        return schema.model_copy()
+    return None
+
+
+def get_actual_type(param_type: type) -> Any | type:
+    actual_type = None
+    origin_type = get_origin(param_type)
+    if origin_type is UnionType:
+        for alternate_type in get_args(param_type):
+            if alternate_type is NoneType:
+                continue
+            if actual_type is not None:
+                raise Exception("Multiple argument types are provided")
+            actual_type = alternate_type
+    else:
+        actual_type = param_type
+
+    return actual_type
 
 
 class ParameterLocation(str, Enum):
     PATH = "path"
     QUERY = "query"
     HEADER = "header"
     COOKIE = "cookie"
@@ -65,18 +93,25 @@
             data = self.body
         else:
             raise Exception(f"Invalid parameter location: {parameter_location}!")
 
         if data and isclass(data) and issubclass(data, BaseModel):
             for name, field_info in data.model_fields.items():
                 field_annotation = field_info.annotation
+                if field_annotation is None:
+                    raise TypeError(f"No type annotation is provided for parameter: {name}")
+
+                if get_origin(field_annotation) == Annotated:
+                    metadata = get_args(field_annotation)
+                    field_annotation = metadata[0]
+
                 if isclass(field_annotation) and issubclass(field_annotation, BaseModel):
                     schema = PydanticSchema(schema_class=field_annotation)
                 else:
-                    schema = Schema(type=get_builtin_type(field_annotation))
+                    schema = get_builtin_type(field_annotation)
 
                 description = field_info.description
 
                 params.append(
                     Parameter(
                         name=name,
                         description=description if description else "",
```

### Comparing `drf_pydantic_openapi-0.5.2/drf_pydantic_openapi/views.py` & `drf_pydantic_openapi-0.5.3/drf_pydantic_openapi/views.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic_openapi-0.5.2/pyproject.toml` & `drf_pydantic_openapi-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pydantic-openapi"
-version = "0.5.2"
+version = "0.5.3"
 description = "OpenAPI (v3) schema generation via Pydantic models using Django REST Framework."
 authors = ["iKlotho <umutkahrimanedu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drf_pydantic_openapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `drf_pydantic_openapi-0.5.2/PKG-INFO` & `drf_pydantic_openapi-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pydantic-openapi
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenAPI (v3) schema generation via Pydantic models using Django REST Framework.
 Author: iKlotho
 Author-email: umutkahrimanedu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

