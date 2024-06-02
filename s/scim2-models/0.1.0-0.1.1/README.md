# Comparing `tmp/scim2_models-0.1.0.tar.gz` & `tmp/scim2_models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim2_models-0.1.0.tar", max compression
+gzip compressed data, was "scim2_models-0.1.1.tar", max compression
```

## Comparing `scim2_models-0.1.0.tar` & `scim2_models-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-06-01 18:28:15.903131 scim2_models-0.1.0/LICENSE
--rw-r--r--   0        0        0     1309 2024-06-01 18:28:15.903131 scim2_models-0.1.0/README.md
--rw-r--r--   0        0        0     2654 2024-06-01 18:33:43.850768 scim2_models-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3281 2024-06-01 18:28:15.906465 scim2_models-0.1.0/scim2_models/__init__.py
--rw-r--r--   0        0        0     2949 2024-06-01 18:28:15.906465 scim2_models-0.1.0/scim2_models/attributes.py
--rw-r--r--   0        0        0    20692 2024-06-01 18:28:15.906465 scim2_models-0.1.0/scim2_models/base.py
--rw-r--r--   0        0        0        0 2024-06-01 18:28:15.906465 scim2_models-0.1.0/scim2_models/rfc7643/__init__.py
--rw-r--r--   0        0        0     1615 2024-06-01 18:28:15.906465 scim2_models-0.1.0/scim2_models/rfc7643/enterprise_user.py
--rw-r--r--   0        0        0     1133 2024-06-01 18:28:15.906465 scim2_models-0.1.0/scim2_models/rfc7643/group.py
--rw-r--r--   0        0        0     8001 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7643/resource.py
--rw-r--r--   0        0        0     2180 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7643/resource_type.py
--rw-r--r--   0        0        0     3305 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7643/schema.py
--rw-r--r--   0        0        0     4301 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7643/service_provider.py
--rw-r--r--   0        0        0    10228 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7643/user.py
--rw-r--r--   0        0        0        0 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7644/__init__.py
--rw-r--r--   0        0        0     1974 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7644/bulk.py
--rw-r--r--   0        0        0     5681 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7644/error.py
--rw-r--r--   0        0        0     1120 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7644/list_response.py
--rw-r--r--   0        0        0      991 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7644/patch_op.py
--rw-r--r--   0        0        0     1472 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/rfc7644/search_request.py
--rw-r--r--   0        0        0      137 2024-06-01 18:28:15.909798 scim2_models-0.1.0/scim2_models/utils.py
--rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 scim2_models-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-01 18:28:15.903131 scim2_models-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1309 2024-06-01 18:28:15.903131 scim2_models-0.1.1/README.md
+-rw-r--r--   0        0        0     2654 2024-06-01 19:31:13.979174 scim2_models-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2607 2024-06-01 19:21:52.961916 scim2_models-0.1.1/scim2_models/__init__.py
+-rw-r--r--   0        0        0     2949 2024-06-01 18:28:15.906465 scim2_models-0.1.1/scim2_models/attributes.py
+-rw-r--r--   0        0        0    21131 2024-06-01 19:27:06.172626 scim2_models-0.1.1/scim2_models/base.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:28:15.906465 scim2_models-0.1.1/scim2_models/rfc7643/__init__.py
+-rw-r--r--   0        0        0     1615 2024-06-01 18:28:15.906465 scim2_models-0.1.1/scim2_models/rfc7643/enterprise_user.py
+-rw-r--r--   0        0        0     1133 2024-06-01 18:28:15.906465 scim2_models-0.1.1/scim2_models/rfc7643/group.py
+-rw-r--r--   0        0        0     7584 2024-06-01 19:28:13.786835 scim2_models-0.1.1/scim2_models/rfc7643/resource.py
+-rw-r--r--   0        0        0     2180 2024-06-01 18:28:15.909798 scim2_models-0.1.1/scim2_models/rfc7643/resource_type.py
+-rw-r--r--   0        0        0     3305 2024-06-01 18:28:15.909798 scim2_models-0.1.1/scim2_models/rfc7643/schema.py
+-rw-r--r--   0        0        0     4301 2024-06-01 18:28:15.909798 scim2_models-0.1.1/scim2_models/rfc7643/service_provider.py
+-rw-r--r--   0        0        0    10228 2024-06-01 18:28:15.909798 scim2_models-0.1.1/scim2_models/rfc7643/user.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:28:15.909798 scim2_models-0.1.1/scim2_models/rfc7644/__init__.py
+-rw-r--r--   0        0        0     1989 2024-06-01 19:11:38.597465 scim2_models-0.1.1/scim2_models/rfc7644/bulk.py
+-rw-r--r--   0        0        0     6492 2024-06-01 19:27:02.915917 scim2_models-0.1.1/scim2_models/rfc7644/error.py
+-rw-r--r--   0        0        0     1106 2024-06-01 19:11:14.463833 scim2_models-0.1.1/scim2_models/rfc7644/list_response.py
+-rw-r--r--   0        0        0     1013 2024-06-01 19:11:38.597465 scim2_models-0.1.1/scim2_models/rfc7644/patch_op.py
+-rw-r--r--   0        0        0     1458 2024-06-01 19:11:35.240757 scim2_models-0.1.1/scim2_models/rfc7644/search_request.py
+-rw-r--r--   0        0        0      137 2024-06-01 18:28:15.909798 scim2_models-0.1.1/scim2_models/utils.py
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 scim2_models-0.1.1/PKG-INFO
```

### Comparing `scim2_models-0.1.0/LICENSE` & `scim2_models-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/README.md` & `scim2_models-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/pyproject.toml` & `scim2_models-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scim2-models"
-version = "0.1.0"
+version = "0.1.1"
 description = "SCIM2 models serialization and validation with pydantic"
 authors = ["Yaal Coop <contact@yaal.coop>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["scim", "scim2", "provisioning", "pydantic"]
 documentation = "https://scim2-models.readthedocs.io"
 repository = "https://github.com/yaal-coop/scim2-models"
```

### Comparing `scim2_models-0.1.0/scim2_models/__init__.py` & `scim2_models-0.1.1/scim2_models/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,24 +34,14 @@
 from .rfc7643.user import Role
 from .rfc7643.user import User
 from .rfc7643.user import X509Certificate
 from .rfc7644.bulk import BulkOperation
 from .rfc7644.bulk import BulkRequest
 from .rfc7644.bulk import BulkResponse
 from .rfc7644.error import Error
-from .rfc7644.error import InvalidFilterError
-from .rfc7644.error import InvalidPathError
-from .rfc7644.error import InvalidSyntaxError
-from .rfc7644.error import InvalidValueError
-from .rfc7644.error import InvalidVersionError
-from .rfc7644.error import MutabilityError
-from .rfc7644.error import NoTargetError
-from .rfc7644.error import SensitiveError
-from .rfc7644.error import TooManyError
-from .rfc7644.error import UniquenessError
 from .rfc7644.list_response import ListResponse
 from .rfc7644.patch_op import Op
 from .rfc7644.patch_op import PatchOp
 from .rfc7644.patch_op import PatchOperation
 from .rfc7644.search_request import SearchRequest
 from .rfc7644.search_request import SortOrder
 
@@ -73,26 +63,19 @@
     "EnterpriseUser",
     "Entitlement",
     "Error",
     "Filter",
     "Group",
     "GroupMember",
     "Im",
-    "InvalidFilterError",
-    "InvalidPathError",
-    "InvalidSyntaxError",
-    "InvalidValueError",
-    "InvalidVersionError",
     "ListResponse",
     "Manager",
     "Meta",
     "Mutability",
-    "MutabilityError",
     "Name",
-    "NoTargetError",
     "Op",
     "Patch",
     "PatchOp",
     "PatchOperation",
     "PhoneNumber",
     "Photo",
     "Required",
@@ -100,16 +83,13 @@
     "ResourceType",
     "Returned",
     "Role",
     "Schema",
     "SchemaExtension",
     "SearchRequest",
     "SortOrder",
-    "SensitiveError",
     "ServiceProviderConfiguration",
     "Sort",
-    "TooManyError",
     "Uniqueness",
-    "UniquenessError",
     "User",
     "X509Certificate",
 ]
```

### Comparing `scim2_models-0.1.0/scim2_models/attributes.py` & `scim2_models-0.1.1/scim2_models/attributes.py`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/scim2_models/base.py` & `scim2_models-0.1.1/scim2_models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,24 +268,14 @@
 
         def returned_filter(item):
             return isinstance(item, Returned)
 
         field_returned = next(filter(returned_filter, field_metadata), default_returned)
         return field_returned
 
-    def get_attribute_urn(self, field_name: str) -> Returned:
-        """Build the full URN of the attribute.
-
-        See :rfc:`RFC7644 §3.12 <7644#section-3.12>`.
-
-        .. todo:: Actually *guess* the URN instead of using the hacky `_attribute_urn` attribute.
-        """
-        alias = self.model_fields[field_name].alias or field_name
-        return f"{self._attribute_urn}.{alias}"
-
     @classmethod
     def get_field_root_type(cls, attribute_name: str) -> Type:
         """Extract the root type from a model field.
 
         For example, return 'GroupMember' for
         'Optional[List[GroupMember]]'
         """
@@ -522,14 +512,35 @@
         if scim_ctx:
             kwargs.setdefault("exclude_none", True)
             kwargs.setdefault("by_alias", True)
             kwargs.setdefault("mode", "json")
 
         return super().model_dump(*args, **kwargs)
 
+    def get_attribute_urn(self, field_name: str) -> Returned:
+        """Build the full URN of the attribute.
+
+        See :rfc:`RFC7644 §3.12 <7644#section-3.12>`.
+
+        .. todo:: Actually *guess* the URN instead of using the hacky `_schema` attribute.
+        """
+        main_schema = self.model_fields["schemas"].default[0]
+        alias = self.model_fields[field_name].alias or field_name
+        return f"{main_schema}:{alias}"
+
 
 class ComplexAttribute(BaseModel):
     """A complex attribute as defined in :rfc:`RFC7643 §2.3.8
     <7643#section-2.3.8>`."""
 
+    def get_attribute_urn(self, field_name: str) -> Returned:
+        """Build the full URN of the attribute.
+
+        See :rfc:`RFC7644 §3.12 <7644#section-3.12>`.
+
+        .. todo:: Actually *guess* the URN instead of using the hacky `_attribute_urn` attribute.
+        """
+        alias = self.model_fields[field_name].alias or field_name
+        return f"{self._attribute_urn}.{alias}"
+
 
 AnyModel = TypeVar("AnyModel", bound=BaseModel)
```

### Comparing `scim2_models-0.1.0/scim2_models/rfc7643/enterprise_user.py` & `scim2_models-0.1.1/scim2_models/rfc7643/enterprise_user.py`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/scim2_models/rfc7643/group.py` & `scim2_models-0.1.1/scim2_models/rfc7643/group.py`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/scim2_models/rfc7643/resource.py` & `scim2_models-0.1.1/scim2_models/rfc7643/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pydantic import Discriminator
 from pydantic import Tag
 from pydantic import field_serializer
 from pydantic import model_validator
 from typing_extensions import Self
 
 from ..base import AnyModel
+from ..base import BaseModel
 from ..base import ComplexAttribute
 from ..base import Mutability
 from ..base import Returned
 from ..base import Uniqueness
 
 
 class Meta(ComplexAttribute):
@@ -76,15 +77,15 @@
     characteristics of a strong validator (see Section 2.1 of
     [RFC7232]), then the origin server MUST mark the "version" (entity-
     tag) as weak by prefixing its opaque value with "W/" (case
     sensitive).
     """
 
 
-class Resource(ComplexAttribute, Generic[AnyModel]):
+class Resource(BaseModel, Generic[AnyModel]):
     model_config = ConfigDict(extra="allow")
 
     schemas: List[str]
     """The "schemas" attribute is a REQUIRED attribute and is an array of
     Strings containing URIs that are used to indicate the namespaces of the
     SCIM schemas that define the attributes present in the current JSON
     structure."""
@@ -184,25 +185,14 @@
             ext.model_fields["schemas"].default[0] for ext in extension_models
         ]
         schemas = self.schemas + [
             schema for schema in extension_schemas if schema not in self.schemas
         ]
         return schemas
 
-    def get_attribute_urn(self, field_name: str) -> Returned:
-        """Build the full URN of the attribute.
-
-        See :rfc:`RFC7644 §3.12 <7644#section-3.12>`.
-
-        .. todo:: Actually *guess* the URN instead of using the hacky `_schema` attribute.
-        """
-        main_schema = self.model_fields["schemas"].default[0]
-        alias = self.model_fields[field_name].alias or field_name
-        return f"{main_schema}:{alias}"
-
 
 AnyResource = TypeVar("AnyResource", bound="Resource")
 
 
 def tagged_resource_union(resource_types: Resource):
     """Build Discriminated Unions, so pydantic can guess which class are needed
     to instantiate by inspecting a payload.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scim2_models-0.1.0/scim2_models/rfc7643/resource_type.py` & `scim2_models-0.1.1/scim2_models/rfc7643/resource_type.py`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/scim2_models/rfc7643/schema.py` & `scim2_models-0.1.1/scim2_models/rfc7643/schema.py`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/scim2_models/rfc7643/service_provider.py` & `scim2_models-0.1.1/scim2_models/rfc7643/service_provider.py`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/scim2_models/rfc7643/user.py` & `scim2_models-0.1.1/scim2_models/rfc7643/user.py`

 * *Files identical despite different names*

### Comparing `scim2_models-0.1.0/scim2_models/rfc7644/bulk.py` & `scim2_models-0.1.1/scim2_models/rfc7644/bulk.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any
 from typing import List
 from typing import Optional
 
 from pydantic import Field
 from pydantic import PlainSerializer
 
+from ..base import BaseModel
 from ..base import ComplexAttribute
 from ..utils import int_to_str
 
 
 class BulkOperation(ComplexAttribute):
     class Method(str, Enum):
         post = "POST"
@@ -41,24 +42,24 @@
     response: Optional[Any] = None
     """The HTTP response body for the specified request operation."""
 
     status: Annotated[Optional[int], PlainSerializer(int_to_str)] = None
     """The HTTP response status code for the requested operation."""
 
 
-class BulkRequest(ComplexAttribute):
+class BulkRequest(BaseModel):
     schemas: List[str] = ["urn:ietf:params:scim:api:messages:2.0:BulkRequest"]
 
     fail_on_errors: Optional[int] = None
     """An integer specifying the number of errors that the service provider
     will accept before the operation is terminated and an error response is
     returned."""
 
     operations: List[BulkOperation] = Field(..., alias="Operations")
     """Defines operations within a bulk job."""
 
 
-class BulkResponse(ComplexAttribute):
+class BulkResponse(BaseModel):
     schemas: List[str] = ["urn:ietf:params:scim:api:messages:2.0:BulkResponse"]
 
     operations: List[BulkOperation] = Field(..., alias="Operations")
     """Defines operations within a bulk job."""
```

### Comparing `scim2_models-0.1.0/scim2_models/rfc7644/error.py` & `scim2_models-0.1.1/scim2_models/rfc7644/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Annotated
 from typing import List
 from typing import Optional
 
 from pydantic import PlainSerializer
 
-from ..base import ComplexAttribute
+from ..base import BaseModel
 from ..utils import int_to_str
 
 
-class Error(ComplexAttribute):
+class Error(BaseModel):
     """Representation of SCIM API errors.
 
     Here is the exhaustive list of pre-defined errors:
 
     .. py:data:: pydanti_scim2.InvalidFilterError
 
        The specified filter syntax
@@ -109,67 +109,86 @@
 
     scim_type: Optional[str] = None
     """A SCIM detail error keyword."""
 
     detail: Optional[str] = None
     """A detailed human-readable message."""
 
-
-InvalidFilterError = Error(
-    status=400,
-    scim_type="invalidFilter",
-    detail="""The specified filter syntax was invalid (does not comply with Figure 1 of RFC7644), or the specified attribute and filter comparison combination is not supported.""",
-)
-
-TooManyError = Error(
-    status=400,
-    scim_type="tooMany",
-    detail="""The specified filter yields many more results than the server is willing to calculate or process.  For example, a filter such as "(userName pr)" by itself would return all entries with a "userName" and MAY not be acceptable to the service provider.""",
-)
-
-UniquenessError = Error(
-    status=409,
-    scim_type="uniqueness",
-    detail="""One or more of the attribute values are already in use or are reserved.""",
-)
-
-MutabilityError = Error(
-    status=400,
-    scim_type="mutability",
-    detail="""The attempted modification is not compatible with the target attribute's mutability or current state (e.g., modification of an "immutable" attribute with an existing value).""",
-)
-
-InvalidSyntaxError = Error(
-    status=400,
-    scim_type="invalidSyntax",
-    detail="""The request body message structure was invalid or did not conform to the request schema.""",
-)
-
-InvalidPathError = Error(
-    status=400,
-    scim_type="invalidPath",
-    detail="""The "path" attribute was invalid or malformed (see Figure 7 of RFC7644).""",
-)
-
-NoTargetError = Error(
-    status=400,
-    scim_type="noTarget",
-    detail="""The specified "path" did not yield an attribute or attribute value that could be operated on.  This occurs when the specified "path" value contains a filter that yields no match.""",
-)
-
-InvalidValueError = Error(
-    status=400,
-    scim_type="invalidValue",
-    detail="""A required value was missing, or the value specified was not compatible with the operation or attribute type (see Section 2.2 of RFC7643), or resource schema (see Section 4 of RFC7643).""",
-)
-
-InvalidVersionError = Error(
-    status=400,
-    scim_type="invalidVers",
-    detail="""The specified SCIM protocol version is not supported (see Section 3.13 of RFC7644).""",
-)
-
-SensitiveError = Error(
-    status=400,
-    scim_type="sensitive",
-    detail="""The specified request cannot be completed, due to the passing of sensitive (e.g., personal) information in a request URI.  For example, personal information SHALL NOT be transmitted over request URIs.  See Section 7.5.2. of RFC7644""",
-)
+    @classmethod
+    def make_invalid_filter_error(cls):
+        return Error(
+            status=400,
+            scim_type="invalidFilter",
+            detail="""The specified filter syntax was invalid (does not comply with Figure 1 of RFC7644), or the specified attribute and filter comparison combination is not supported.""",
+        )
+
+    @classmethod
+    def make_too_many_error(cls):
+        return Error(
+            status=400,
+            scim_type="tooMany",
+            detail="""The specified filter yields many more results than the server is willing to calculate or process.  For example, a filter such as "(userName pr)" by itself would return all entries with a "userName" and MAY not be acceptable to the service provider.""",
+        )
+
+    @classmethod
+    def make_uniqueness_error(cls):
+        return Error(
+            status=409,
+            scim_type="uniqueness",
+            detail="""One or more of the attribute values are already in use or are reserved.""",
+        )
+
+    @classmethod
+    def make_mutability_error(cls):
+        return Error(
+            status=400,
+            scim_type="mutability",
+            detail="""The attempted modification is not compatible with the target attribute's mutability or current state (e.g., modification of an "immutable" attribute with an existing value).""",
+        )
+
+    @classmethod
+    def make_invalid_syntaxError(cls):
+        return Error(
+            status=400,
+            scim_type="invalidSyntax",
+            detail="""The request body message structure was invalid or did not conform to the request schema.""",
+        )
+
+    @classmethod
+    def make_invalid_path_error(cls):
+        return Error(
+            status=400,
+            scim_type="invalidPath",
+            detail="""The "path" attribute was invalid or malformed (see Figure 7 of RFC7644).""",
+        )
+
+    @classmethod
+    def make_no_target_error(cls):
+        return Error(
+            status=400,
+            scim_type="noTarget",
+            detail="""The specified "path" did not yield an attribute or attribute value that could be operated on.  This occurs when the specified "path" value contains a filter that yields no match.""",
+        )
+
+    @classmethod
+    def make_invalid_value_error(cls):
+        return Error(
+            status=400,
+            scim_type="invalidValue",
+            detail="""A required value was missing, or the value specified was not compatible with the operation or attribute type (see Section 2.2 of RFC7643), or resource schema (see Section 4 of RFC7643).""",
+        )
+
+    @classmethod
+    def make_invalid_version_error(cls):
+        return Error(
+            status=400,
+            scim_type="invalidVers",
+            detail="""The specified SCIM protocol version is not supported (see Section 3.13 of RFC7644).""",
+        )
+
+    @classmethod
+    def make_sensitive_error(cls):
+        return Error(
+            status=400,
+            scim_type="sensitive",
+            detail="""The specified request cannot be completed, due to the passing of sensitive (e.g., personal) information in a request URI.  For example, personal information SHALL NOT be transmitted over request URIs.  See Section 7.5.2. of RFC7644""",
+        )
```

### Comparing `scim2_models-0.1.0/scim2_models/rfc7644/list_response.py` & `scim2_models-0.1.1/scim2_models/rfc7644/list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Union
 
 from pydantic import Field
 
-from ..base import ComplexAttribute
+from ..base import BaseModel
 from ..rfc7643.resource import AnyResource
 from ..rfc7643.resource import tagged_resource_union
 
 
-class ListResponse(ComplexAttribute, Generic[AnyResource]):
+class ListResponse(BaseModel, Generic[AnyResource]):
     @classmethod
     def of(cls, *resource_types: AnyResource):
         """Build a ListResponse instance that can handle resource_types."""
 
         return cls[tagged_resource_union(Union[resource_types])]
 
     schemas: List[str] = ["urn:ietf:params:scim:api:messages:2.0:ListResponse"]
```

### Comparing `scim2_models-0.1.0/scim2_models/rfc7644/patch_op.py` & `scim2_models-0.1.1/scim2_models/rfc7644/patch_op.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import Any
 from typing import List
 from typing import Optional
 
 from pydantic import Field
 
+from ..base import BaseModel
 from ..base import ComplexAttribute
 
 
 class Op(str, Enum):
     replace = "replace"
     remove = "remove"
     add = "add"
@@ -23,13 +24,13 @@
     path: Optional[str] = None
     """The "path" attribute value is a String containing an attribute path
     describing the target of the operation."""
 
     value: Optional[Any] = None
 
 
-class PatchOp(ComplexAttribute):
+class PatchOp(BaseModel):
     schemas: List[str] = ["urn:ietf:params:scim:api:messages:2.0:PatchOp"]
 
     operations: List[PatchOperation] = Field(..., alias="Operations")
     """The body of an HTTP PATCH request MUST contain the attribute
     "Operations", whose value is an array of one or more PATCH operations."""
```

### Comparing `scim2_models-0.1.0/scim2_models/rfc7644/search_request.py` & `scim2_models-0.1.1/scim2_models/rfc7644/search_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from enum import Enum
 from typing import List
 from typing import Optional
 
-from ..base import ComplexAttribute
+from ..base import BaseModel
 
 
 class SortOrder(str, Enum):
     ascending = "ascending"
     descending = "descending"
 
 
-class SearchRequest(ComplexAttribute):
+class SearchRequest(BaseModel):
     """SearchRequest object defined at https://datatracker.ietf.org/doc/html/rfc7644#section-3.4.3"""
 
     schemas: List[str] = ["urn:ietf:params:scim:api:messages:2.0:SearchRequest"]
 
     attributes: Optional[List[str]] = None
     """A multi-valued list of strings indicating the names of resource
     attributes to return in the response, overriding the set of attributes that
```

### Comparing `scim2_models-0.1.0/PKG-INFO` & `scim2_models-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim2-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: SCIM2 models serialization and validation with pydantic
 Home-page: https://github.com/yaal-coop/scim2-models
 License: Apache
 Keywords: scim,scim2,provisioning,pydantic
 Author: Yaal Coop
 Author-email: contact@yaal.coop
 Requires-Python: >=3.9,<4.0
```

