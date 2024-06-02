# Comparing `tmp/qstd_core-0.5.2.tar.gz` & `tmp/qstd_core-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_core-0.5.2.tar", last modified: Sun May 12 13:08:34 2024, max compression
+gzip compressed data, was "qstd_core-0.6.0.tar", last modified: Sun Jun  2 17:03:07 2024, max compression
```

## Comparing `qstd_core-0.5.2.tar` & `qstd_core-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.5.2/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-05-12 13:08:34.173718 qstd_core-0.5.2/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.5.2/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.5.2/qstd_core/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/exceptions/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.5.2/qstd_core/exceptions/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.5.2/qstd_core/exceptions/base.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.5.2/qstd_core/exceptions/localization.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/localization/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.5.2/qstd_core/localization/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/logger/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.5.2/qstd_core/logger/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/marshmallow/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-05-01 11:16:49.000000 qstd_core-0.5.2/qstd_core/marshmallow/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9670 2024-05-01 15:31:17.000000 qstd_core-0.5.2/qstd_core/marshmallow/fields.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1664 2024-05-12 13:07:29.000000 qstd_core-0.5.2/qstd_core/marshmallow/schema.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4358 2024-05-01 15:24:31.000000 qstd_core-0.5.2/qstd_core/marshmallow/validate.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/openapi/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.5.2/qstd_core/openapi/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5915 2024-04-26 15:07:56.000000 qstd_core-0.5.2/qstd_core/openapi/decorators.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.5.2/qstd_core/openapi/enum.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.5.2/qstd_core/openapi/router.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9221 2024-04-26 10:28:32.000000 qstd_core-0.5.2/qstd_core/openapi/spec.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8906 2024-05-05 15:59:18.000000 qstd_core-0.5.2/qstd_core/openapi/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/sanic/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.5.2/qstd_core/sanic/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/sanic/request/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.5.2/qstd_core/sanic/request/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/sanic/server/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.5.2/qstd_core/sanic/server/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.5.2/qstd_core/sanic/server/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/validator/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2008 2024-04-25 11:21:18.000000 qstd_core-0.5.2/qstd_core/validator/ValidatorABS.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2693 2024-05-05 16:02:29.000000 qstd_core-0.5.2/qstd_core/validator/ValidatorMarshmallow.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1191 2024-04-25 11:11:00.000000 qstd_core-0.5.2/qstd_core/validator/ValidatorPydantic.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1834 2024-04-23 09:26:58.000000 qstd_core-0.5.2/qstd_core/validator/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.5.2/qstd_core/validator/enums.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-05-05 15:31:12.000000 qstd_core-0.5.2/qstd_core/validator/exceptions.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.5.2/qstd_core/validator/types.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1062 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       65 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/requires.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-12 13:08:34.173718 qstd_core-0.5.2/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      706 2024-05-12 13:08:06.000000 qstd_core-0.5.2/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.6.0/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-06-02 17:03:07.805111 qstd_core-0.6.0/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.6.0/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.6.0/qstd_core/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/exceptions/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.6.0/qstd_core/exceptions/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.6.0/qstd_core/exceptions/base.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.6.0/qstd_core/exceptions/localization.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/localization/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.6.0/qstd_core/localization/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/logger/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.6.0/qstd_core/logger/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/marshmallow/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-05-01 11:16:49.000000 qstd_core-0.6.0/qstd_core/marshmallow/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9633 2024-06-02 15:48:10.000000 qstd_core-0.6.0/qstd_core/marshmallow/fields.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1664 2024-05-12 13:07:29.000000 qstd_core-0.6.0/qstd_core/marshmallow/schema.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4358 2024-05-01 15:24:31.000000 qstd_core-0.6.0/qstd_core/marshmallow/validate.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/openapi/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.6.0/qstd_core/openapi/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     6125 2024-06-02 16:42:07.000000 qstd_core-0.6.0/qstd_core/openapi/decorators.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.6.0/qstd_core/openapi/enum.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.6.0/qstd_core/openapi/router.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9225 2024-06-02 16:39:43.000000 qstd_core-0.6.0/qstd_core/openapi/spec.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8906 2024-05-05 15:59:18.000000 qstd_core-0.6.0/qstd_core/openapi/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/sanic/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.6.0/qstd_core/sanic/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/sanic/request/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.6.0/qstd_core/sanic/request/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/sanic/server/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.6.0/qstd_core/sanic/server/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.6.0/qstd_core/sanic/server/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core/validator/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2042 2024-06-02 16:44:24.000000 qstd_core-0.6.0/qstd_core/validator/ValidatorABS.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     3003 2024-06-02 16:50:27.000000 qstd_core-0.6.0/qstd_core/validator/ValidatorMarshmallow.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1430 2024-06-02 16:46:19.000000 qstd_core-0.6.0/qstd_core/validator/ValidatorPydantic.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2317 2024-06-02 16:47:33.000000 qstd_core-0.6.0/qstd_core/validator/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.6.0/qstd_core/validator/enums.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-05-05 15:31:12.000000 qstd_core-0.6.0/qstd_core/validator/exceptions.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.6.0/qstd_core/validator/types.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-06-02 17:03:07.805111 qstd_core-0.6.0/qstd_core.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-06-02 17:03:07.000000 qstd_core-0.6.0/qstd_core.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1062 2024-06-02 17:03:07.000000 qstd_core-0.6.0/qstd_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-06-02 17:03:07.000000 qstd_core-0.6.0/qstd_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       65 2024-06-02 17:03:07.000000 qstd_core-0.6.0/qstd_core.egg-info/requires.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-06-02 17:03:07.000000 qstd_core-0.6.0/qstd_core.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-06-02 17:03:07.805111 qstd_core-0.6.0/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      706 2024-06-02 16:03:06.000000 qstd_core-0.6.0/setup.py
```

### Comparing `qstd_core-0.5.2/LICENSE` & `qstd_core-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/exceptions/base.py` & `qstd_core-0.6.0/qstd_core/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/exceptions/localization.py` & `qstd_core-0.6.0/qstd_core/exceptions/localization.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/localization/__init__.py` & `qstd_core-0.6.0/qstd_core/localization/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/marshmallow/fields.py` & `qstd_core-0.6.0/qstd_core/marshmallow/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import enum
 from typing import AnyStr
 
 import typing
 from marshmallow import fields, ValidationError
-from . import validate as c_validate
 
 
 def custom_field_factory(field_cls: typing.Type[fields.Field]):
     class CustomField(field_cls):
         _field_name = None
         deprecated = None
         meta_one_of: list
```

### Comparing `qstd_core-0.5.2/qstd_core/marshmallow/schema.py` & `qstd_core-0.6.0/qstd_core/marshmallow/schema.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/marshmallow/validate.py` & `qstd_core-0.6.0/qstd_core/marshmallow/validate.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/openapi/decorators.py` & `qstd_core-0.6.0/qstd_core/openapi/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import typing
 
+from marshmallow import Schema, fields
+from pydantic import BaseModel
+
 from .spec import OpenapiRouteContent, OpenapiRouteParameterEnum
 from .utils import (
     upsert,
     override_handlers,
     webhook_handlers,
     exception_schema_to_response,
     schema_mapper_factory,
     object_schema_to_parameters,
     path_schema_from_raw_parameters
 )
 from .enum import STATUS_TO_DESCRIPTION
-from ..validator.types import SchemaType
+
+
+SchemaType = typing.Union[Schema, fields.Field, typing.Type[BaseModel]]
 
 
 def response_file(content_type='*/*', status=200, description=None):
     if description is None:
         description = STATUS_TO_DESCRIPTION.get(status, None)
 
     def inner(func):
@@ -94,15 +99,15 @@
                 'format': 'binary'
             }
         )
         return func
     return inner
 
 
-def tag(tag_name: str, includes=None, excludes=None):
+def tag(tag_name: str, includes: typing.Optional[str] = None, excludes: typing.Optional[str] = None):
     def inner(func):
         upsert(func).add_tag_fabric(tag_name, includes, excludes)
         return func
     return inner
 
 
 def exclude():
@@ -233,12 +238,12 @@
         return func
     return inner
 
 
 params = path
 
 
-def security(name: str):
+def security(name: str, scopes: typing.Optional[typing.List[str]] = None):
     def inner(func):
-        upsert(func).add_security(name)
+        upsert(func).add_security(name, scopes)
         return func
     return inner
```

### Comparing `qstd_core-0.5.2/qstd_core/openapi/spec.py` & `qstd_core-0.6.0/qstd_core/openapi/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,18 +243,18 @@
             if code not in self.responses:
                 self.responses[code] = content
             else:
                 self.responses[code].merge(content)
         self.security.update(route.security)
         return self
 
-    def add_security(self, name: str, scope: typing.List[str] = None):
-        if scope is None:
-            scope = []
-        self.security[name] = scope
+    def add_security(self, name: str, scopes: typing.List[str] = None):
+        if scopes is None:
+            scopes = []
+        self.security[name] = scopes
 
     def resolve_tags(
         self,
         url: str,
         default_tag: str
     ) -> OpenapiRoute:
         if len(self.tags) == 0 and len(self.tags_options) == 0:
```

### Comparing `qstd_core-0.5.2/qstd_core/openapi/utils.py` & `qstd_core-0.6.0/qstd_core/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/sanic/request/__init__.py` & `qstd_core-0.6.0/qstd_core/sanic/request/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core/validator/ValidatorABS.py` & `qstd_core-0.6.0/qstd_core/validator/ValidatorABS.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,12 +52,12 @@
                 kwargs[self.target_name.value] = validated
             return await func(*args, **kwargs)
         openapi.errors(SchemaValidationException)(func)
         if self.docs:
             getattr(openapi, self.target_name.value)(self.schema)(func)
         return wrapper
 
-    def validate(self, payload: dict):
+    def validate(self, payload: typing.Union[dict, list]) -> typing.Any:
         raise NotImplementedError()
 
     def get_schema_fields(self):
         raise NotImplementedError()
```

### Comparing `qstd_core-0.5.2/qstd_core/validator/ValidatorMarshmallow.py` & `qstd_core-0.6.0/qstd_core/validator/ValidatorMarshmallow.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,28 @@
 
 from . import TargetNameType
 from .exceptions import SchemaValidationException
 from .ValidatorABS import ValidatorABS
 from ..logger import app_core_logger
 
 
-class ValidatorMarshmallow(ValidatorABS):
+TP = typing.TypeVar('TP', bound=dict)
+TR = typing.TypeVar('TR', bound=dict)
+
+
+class ValidatorMarshmallow(ValidatorABS, typing.Generic[TR]):
     schema: Schema
 
-    def validate(self, payload: dict):
+    @typing.overload
+    def validate(self, payload: typing.List[TP]) -> typing.List[TR]: ...
+
+    @typing.overload
+    def validate(self, payload: TP) -> TR: ...
+
+    def validate(self, payload: typing.Union[dict, list]) -> typing.Union[dict, list]:
         try:
             return self.schema.load(payload)
         except ValidationError as ex:
             raise self.errors_mapper(ex.messages)
 
     def errors_mapper(self, errors) -> SchemaValidationException:
         errors_list = []
```

### Comparing `qstd_core-0.5.2/qstd_core/validator/__init__.py` & `qstd_core-0.6.0/qstd_core/validator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,37 @@
 from .ValidatorABS import ValidatorABS
 from .ValidatorPydantic import ValidatorPydantic
 from .ValidatorMarshmallow import ValidatorMarshmallow
 from .types import SchemaType
 from ..marshmallow import Schema
 
 
+TPM = typing.TypeVar("TPM", bound=BaseModel)
+
+
+@typing.overload
+def validator_factory(
+    *,
+    schema: typing.Type[TPM],
+    target: TargetNameType,
+    pass_data: typing.Optional[bool] = True,
+    docs: typing.Optional[bool] = True
+) -> ValidatorPydantic[TPM]: ...
+
+
+@typing.overload
+def validator_factory(
+    *,
+    schema: Schema,
+    target: TargetNameType,
+    pass_data: typing.Optional[bool] = True,
+    docs: typing.Optional[bool] = True
+) -> ValidatorMarshmallow: ...
+
+
 def validator_factory(
     *,
     schema: SchemaType,
     target: TargetNameType,
     pass_data: typing.Optional[bool] = True,
     docs: typing.Optional[bool] = True
 ) -> ValidatorABS:
```

### Comparing `qstd_core-0.5.2/qstd_core/validator/exceptions.py` & `qstd_core-0.6.0/qstd_core/validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/qstd_core.egg-info/SOURCES.txt` & `qstd_core-0.6.0/qstd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.2/setup.py` & `qstd_core-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_core',
-    version='0.5.2',
+    version='0.6.0',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Application core based on sanic',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-core',
     packages=find_packages(exclude=['tmp', 'example']),
```

