# Comparing `tmp/openapi_schemas_pydantic-1.1.0.tar.gz` & `tmp/openapi_schemas_pydantic-2.0.0.tar.gz`

## Comparing `openapi_schemas_pydantic-1.1.0.tar` & `openapi_schemas_pydantic-2.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/py.typed
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/utils/__init__.py
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/utils/constants.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/utils/enums.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/utils/utils.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/callback.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/components.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/contact.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/discriminator.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/encoding.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/example.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/external_documentation.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/header.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/info.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/license.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/link.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/media_type.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/oauth_flow.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/oauth_flows.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/open_api.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/operation.py
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/parameter.py
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/path_item.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/paths.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/reference.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/request_body.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/response.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/responses.py
--rw-r--r--   0        0        0    38415 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/schema.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/security_requirement.py
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/security_scheme.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/server.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/server_variable.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/tag.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/xml.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/LICENSE
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/README.md
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/py.typed
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/utils/__init__.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/utils/constants.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/utils/enums.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/utils/utils.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/callback.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/components.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/contact.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/discriminator.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/encoding.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/example.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/external_documentation.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/header.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/info.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/license.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/link.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/media_type.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/oauth_flow.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/oauth_flows.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/open_api.py
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/operation.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/parameter.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/path_item.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/paths.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/reference.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/request_body.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/response.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/responses.py
+-rw-r--r--   0        0        0    38423 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/schema.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/security_requirement.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/security_scheme.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/server.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/server_variable.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/tag.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/xml.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/README.md
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 openapi_schemas_pydantic-2.0.0/PKG-INFO
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/utils/constants.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import deque
 from datetime import date, datetime, time, timedelta
-from typing import Any, Dict, Pattern, Type, Union
+from typing import Any, Callable, Dict, Pattern, Type, Union
 from uuid import UUID
 
 from pydantic import (
     UUID1,
     UUID3,
     UUID4,
     UUID5,
@@ -20,44 +20,45 @@
     IPvAnyNetwork,
     Json,
     NameEmail,
     NegativeFloat,
     NegativeInt,
     NonNegativeInt,
     NonPositiveFloat,
-    PaymentCardNumber,
     PositiveFloat,
     PositiveInt,
     PostgresDsn,
-    PyObject,
     RedisDsn,
     SecretBytes,
     SecretStr,
     StrictBool,
     StrictBytes,
     StrictFloat,
     StrictInt,
     StrictStr,
 )
-from pydantic.fields import (
+from pydantic.v1.fields import (
     SHAPE_DEFAULTDICT,
     SHAPE_DEQUE,
     SHAPE_DICT,
     SHAPE_FROZENSET,
     SHAPE_ITERABLE,
     SHAPE_LIST,
     SHAPE_SEQUENCE,
     SHAPE_SET,
     SHAPE_TUPLE,
     SHAPE_TUPLE_ELLIPSIS,
 )
+from pydantic_extra_types.payment import PaymentCardNumber
 
 from openapi_schemas_pydantic.utils.enums import OpenAPIFormat, OpenAPIType
 from openapi_schemas_pydantic.v3_1_0.schema import Schema
 
+PyObject = Callable[..., Any]
+
 PYDANTIC_FIELD_SHAPE_MAP: Dict[int, OpenAPIType] = {
     SHAPE_LIST: OpenAPIType.ARRAY,
     SHAPE_SET: OpenAPIType.ARRAY,
     SHAPE_TUPLE: OpenAPIType.ARRAY,
     SHAPE_TUPLE_ELLIPSIS: OpenAPIType.ARRAY,
     SHAPE_SEQUENCE: OpenAPIType.ARRAY,
     SHAPE_FROZENSET: OpenAPIType.ARRAY,
@@ -212,17 +213,15 @@
     "multiple_of": "multipleOf",
     "ge": "minimum",
     "le": "maximum",
     "lt": "exclusiveMaximum",
     "gt": "exclusiveMinimum",
     "max_length": "maxLength",
     "min_length": "minLength",
-    "max_items": "maxItems",
-    "min_items": "minItems",
-    "regex": "pattern",
+    "pattern": "pattern",
     "title": "title",
     "description": "description",
 }
 
 EXTRA_TO_OPENAPI_PROPERTY_MAP: Dict[str, str] = {
     "examples": "examples",
     "external_docs": "externalDocs",
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/utils/enums.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/utils/enums.py`

 * *Files identical despite different names*

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/utils/utils.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import TYPE_CHECKING, Any, Set, Type, TypeVar, cast
 
 from pydantic import BaseModel, create_model
-from pydantic.schema import schema
+from pydantic.json_schema import models_json_schema
 
 from openapi_schemas_pydantic import v3_1_0
 
 if TYPE_CHECKING:
     from typing import Dict
 
 REF_PREFIX = "#/components/schemas/"
 SCHEMA_NAME_ATTRIBUTE = "__schema_name__"
+MODE = "validation"
 
 T = TypeVar("T", bound=v3_1_0.OpenAPI)
 
 
 class OpenAPI310PydanticSchema(v3_1_0.Schema):
     """Special `Schema` class to indicate a reference from pydantic class."""
 
@@ -30,39 +31,41 @@
     Args:
         open_api_schema: An instance of the OpenAPI model.
 
     Returns:
         new OpenAPI object with "#/components/schemas" values updated. If there is no update in
             "#/components/schemas" values, the original `open_api` will be returned.
     """
-    copied_schema = open_api_schema.copy(deep=True)
+    copied_schema = open_api_schema.model_copy(deep=True)
     schema_classes = list(
         extract_pydantic_types_to_openapi_components(obj=copied_schema, ref_class=v3_1_0.Reference)
     )
 
     if not schema_classes:
         return open_api_schema
 
     if not copied_schema.components:
         copied_schema.components = v3_1_0.Components(schemas={})
     if copied_schema.components.schemas is None:  # pragma: no cover
         copied_schema.components.schemas = cast("Dict[str, Any]", {})
 
     schema_classes = [
-        cls
-        if not hasattr(cls, "__schema_name__")
-        else create_model(getattr(cls, SCHEMA_NAME_ATTRIBUTE), __base__=cls)
+        (cls, MODE)
+        if not hasattr(cls, SCHEMA_NAME_ATTRIBUTE)
+        else (create_model(getattr(cls, SCHEMA_NAME_ATTRIBUTE), __base__=cls), MODE)
         for cls in schema_classes
     ]
-    schema_classes.sort(key=lambda x: x.__name__)
-    schema_definitions = schema(schema_classes, ref_prefix=REF_PREFIX)["definitions"]
+
+    schema_classes.sort(key=lambda x: x[0].__name__)
+    _, json_schema = models_json_schema(schema_classes)
+
     copied_schema.components.schemas.update(
         {
-            key: v3_1_0.Schema.parse_obj(schema_dict)
-            for key, schema_dict in schema_definitions.items()
+            key: v3_1_0.Schema.model_validate(schema_dict)
+            for key, schema_dict in json_schema["$defs"].items()
         }
     )
     return copied_schema
 
 
 def extract_pydantic_types_to_openapi_components(
     obj: Any, ref_class: Type[v3_1_0.Reference]
@@ -76,15 +79,15 @@
         ref_class:
 
     Returns:
         set of pydantic schema classes
     """
     pydantic_schemas: Set[Type[BaseModel]] = set()
     if isinstance(obj, BaseModel):
-        fields = obj.__fields_set__
+        fields = obj.model_fields_set
         for field in fields:
             child_obj = getattr(obj, field)
             if isinstance(child_obj, OpenAPI310PydanticSchema):
                 setattr(obj, field, ref_class(ref=create_ref_prefix(child_obj.schema_class)))
                 pydantic_schemas.add(child_obj.schema_class)
             else:
                 pydantic_schemas.update(
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/__init__.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,16 +33,19 @@
 from .security_scheme import SecurityScheme
 from .server import Server
 from .server_variable import ServerVariable
 from .tag import Tag
 from .xml import XML
 
 # resolve forward references
-Encoding.update_forward_refs(Header=Header)
-Schema.update_forward_refs()
+Encoding.model_rebuild()
+Schema.model_rebuild()
+Header.model_rebuild()
+Reference.model_rebuild()
+Operation.model_rebuild()
 
 __all__ = [
     "Callback",
     "Components",
     "Contact",
     "Discriminator",
     "Encoding",
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/callback.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/components.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .callback import Callback
 from .example import Example
 from .header import Header
 from .link import Link
 from .parameter import Parameter
 from .path_item import PathItem
@@ -19,47 +19,17 @@
     """Holds a set of reusable objects for different aspects of the OAS.
 
     All objects defined within the components object will have no effect
     on the API unless they are explicitly referenced from properties
     outside the components object.
     """
 
-    schemas: Optional[Dict[str, Schema]] = None
-    """An object to hold reusable [Schema Objects](https://spec.openapis.org/oas/v3.1.0#schemaObject)."""
-
-    responses: Optional[Dict[str, Union[Response, Reference]]] = None
-    """An object to hold reusable [Response Objects](https://spec.openapis.org/oas/v3.1.0#responseObject)."""
-
-    parameters: Optional[Dict[str, Union[Parameter, Reference]]] = None
-    """An object to hold reusable [Parameter Objects](https://spec.openapis.org/oas/v3.1.0#parameterObject)."""
-
-    examples: Optional[Dict[str, Union[Example, Reference]]] = None
-    """An object to hold reusable [Example Objects](https://spec.openapis.org/oas/v3.1.0#exampleObject)."""
-
-    requestBodies: Optional[Dict[str, Union[RequestBody, Reference]]] = None
-    """An object to hold reusable [Request Body Objects](https://spec.openapis.org/oas/v3.1.0#requestBodyObject)."""
-
-    headers: Optional[Dict[str, Union[Header, Reference]]] = None
-    """An object to hold reusable [Header Objects](https://spec.openapis.org/oas/v3.1.0#headerObject)."""
-
-    securitySchemes: Optional[Dict[str, Union[SecurityScheme, Reference]]] = None
-    """An object to hold reusable [Security Scheme Objects](https://spec.openapis.org/oas/v3.1.0#securitySchemeObject)."""
-
-    links: Optional[Dict[str, Union[Link, Reference]]] = None
-    """An object to hold reusable [Link Objects](https://spec.openapis.org/oas/v3.1.0#linkObject)."""
-
-    callbacks: Optional[Dict[str, Union[Callback, Reference]]] = None
-    """An object to hold reusable [Callback Objects](https://spec.openapis.org/oas/v3.1.0#callbackObject)."""
-
-    pathItems: Optional[Dict[str, Union[PathItem, Reference]]] = None
-    """An object to hold reusable [Path Item Object](https://spec.openapis.org/oas/v3.1.0#pathItemObject)."""
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "schemas": {
                         "GeneralError": {
                             "type": "object",
                             "properties": {
                                 "code": {"type": "integer", "format": "int32"},
@@ -122,8 +92,39 @@
                                     },
                                 }
                             },
                         },
                     },
                 }
             ]
-        }
+        },
+    )
+
+    schemas: Optional[Dict[str, Schema]] = None
+    """An object to hold reusable [Schema Objects](https://spec.openapis.org/oas/v3.1.0#schemaObject)."""
+
+    responses: Optional[Dict[str, Union[Response, Reference]]] = None
+    """An object to hold reusable [Response Objects](https://spec.openapis.org/oas/v3.1.0#responseObject)."""
+
+    parameters: Optional[Dict[str, Union[Parameter, Reference]]] = None
+    """An object to hold reusable [Parameter Objects](https://spec.openapis.org/oas/v3.1.0#parameterObject)."""
+
+    examples: Optional[Dict[str, Union[Example, Reference]]] = None
+    """An object to hold reusable [Example Objects](https://spec.openapis.org/oas/v3.1.0#exampleObject)."""
+
+    requestBodies: Optional[Dict[str, Union[RequestBody, Reference]]] = None
+    """An object to hold reusable [Request Body Objects](https://spec.openapis.org/oas/v3.1.0#requestBodyObject)."""
+
+    headers: Optional[Dict[str, Union[Header, Reference]]] = None
+    """An object to hold reusable [Header Objects](https://spec.openapis.org/oas/v3.1.0#headerObject)."""
+
+    securitySchemes: Optional[Dict[str, Union[SecurityScheme, Reference]]] = None
+    """An object to hold reusable [Security Scheme Objects](https://spec.openapis.org/oas/v3.1.0#securitySchemeObject)."""
+
+    links: Optional[Dict[str, Union[Link, Reference]]] = None
+    """An object to hold reusable [Link Objects](https://spec.openapis.org/oas/v3.1.0#linkObject)."""
+
+    callbacks: Optional[Dict[str, Union[Callback, Reference]]] = None
+    """An object to hold reusable [Callback Objects](https://spec.openapis.org/oas/v3.1.0#callbackObject)."""
+
+    pathItems: Optional[Dict[str, Union[PathItem, Reference]]] = None
+    """An object to hold reusable [Path Item Object](https://spec.openapis.org/oas/v3.1.0#pathItemObject)."""
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/contact.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/example.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,49 @@
-from typing import Optional, Union
+from typing import Any, Optional
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Extra, validator
+from pydantic import BaseModel, ConfigDict
 
 
-class Contact(BaseModel):
-    """Contact information for the exposed API."""
-
-    name: Optional[str] = None
+class Example(BaseModel):
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
+            "examples": [
+                {"summary": "A foo example", "value": {"foo": "bar"}},
+                {
+                    "summary": "This is an example in XML",
+                    "externalValue": "http://example.org/examples/address-example.xml",
+                },
+                {
+                    "summary": "This is a text example",
+                    "externalValue": "http://foo.bar/examples/address-example.txt",
+                },
+            ]
+        },
+    )
+    summary: Optional[str] = None
     """
-    The identifying name of the contact person/organization.
+    Short description for the example.
     """
 
-    url: Optional[AnyUrl] = None
+    description: Optional[str] = None
     """
-    The URL pointing to the contact information.
-    MUST be in the form of a URL.
+    Long description for the example.
+    [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text representation.
     """
 
-    email: Optional[Union[EmailStr, str]] = None
+    value: Optional[Any] = None
     """
-    The email address of the contact person/organization.
-    MUST be in the form of an email address.
+    Embedded literal example.
+    The `value` field and `externalValue` field are mutually exclusive.
+    To represent examples of media types that cannot naturally represented in JSON or YAML,
+    use a string value to contain the example, escaping where necessary.
     """
 
-    @validator("email", pre=True)
-    def validate_email(  # pylint: disable=no-self-argument
-        cls,
-        v: Union[EmailStr, str],
-    ) -> EmailStr:
-        """Validates that email is a valid email address.
-
-        Args:
-            v: Holds the email string to be validated
-
-        Raises:
-            ValueError: Value is not a valid email address
-
-        Returns:
-            Validated email string.
-        """
-        if isinstance(v, str):
-            v = EmailStr(v)
-        return v
+    externalValue: Optional[str] = None
+    """
+    A URL that points to the literal example.
+    This provides the capability to reference examples that cannot easily be included in JSON or YAML documents.
 
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
-            "examples": [
-                {
-                    "name": "API Support",
-                    "url": "http://www.example.com/support",
-                    "email": "support@example.com",
-                }
-            ]
-        }
+    The `value` field and `externalValue` field are mutually exclusive.
+    See the rules for resolving [Relative References](https://spec.openapis.org/oas/v3.1.0#relativeReferencesURI).
+    """
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/discriminator.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/discriminator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 
 class Discriminator(BaseModel):
     """When request bodies or response payloads may be one of a number of
     different schemas, a `discriminator` object can be used to aid in
     serialization, deserialization, and validation.
 
     The discriminator is a specific object in a schema which is used to inform the consumer of the specification
     of an alternative schema based on the value associated with it.
 
     When using the discriminator, _inline_ schemas will not be considered.
     """
 
-    propertyName: str
-    """
-    **REQUIRED**. The name of the property in the payload that will hold the discriminator value.
-    """
-
-    mapping: Optional[Dict[str, str]] = None
-    """
-    An object to hold mappings between payload values and schema names or references.
-    """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "propertyName": "petType",
                     "mapping": {
                         "dog": "#/components/schemas/Dog",
                         "monster": "https://gigantic-server.com/schemas/Monster/schema.json",
                     },
                 }
             ]
-        }
+        },
+    )
+
+    propertyName: str
+    """
+    **REQUIRED**. The name of the property in the payload that will hold the discriminator value.
+    """
+
+    mapping: Optional[Dict[str, str]] = None
+    """
+    An object to hold mappings between payload values and schema names or references.
+    """
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/encoding.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .reference import Reference
 
 if TYPE_CHECKING:
     from openapi_schemas_pydantic.v3_1_0.header import Header
 
 
 class Encoding(BaseModel):
     """A single encoding definition applied to a single schema property."""
 
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
+            "examples": [
+                {
+                    "contentType": "image/png, image/jpeg",
+                    "headers": {
+                        "X-Rate-Limit-Limit": {
+                            "description": "The number of allowed requests in the current period",
+                            "schema": {"type": "integer"},
+                        }
+                    },
+                }
+            ]
+        },
+    )
+
     contentType: Optional[str] = None
     """
     The Content-Type for encoding a specific property.
     Default value depends on the property type:
 
     for `object` - `application/json`;
     for `array` – the default is defined based on the inner type;
@@ -65,23 +82,7 @@
     `:/?#[]@!$&'()*+,;=` to be included without percent-encoding.
     The default value is `false`.
     This property SHALL be ignored if the request body media type
     is not `application/x-www-form-urlencoded` or `multipart/form-data`.
     If a value is explicitly defined,
     then the value of [contentType](https://spec.openapis.org/oas/v3.1.0#encodingContentType) (implicit or explicit) SHALL be ignored.
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
-            "examples": [
-                {
-                    "contentType": "image/png, image/jpeg",
-                    "headers": {
-                        "X-Rate-Limit-Limit": {
-                            "description": "The number of allowed requests in the current period",
-                            "schema": {"type": "integer"},
-                        }
-                    },
-                }
-            ]
-        }
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/example.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,77 @@
-from typing import Any, Optional
+from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import AnyUrl, BaseModel, ConfigDict
 
+from .contact import Contact
+from .license import License
 
-class Example(BaseModel):
+
+class Info(BaseModel):
+    """The object provides metadata about the API.
+
+    The metadata MAY be used by the clients if needed, and MAY be
+    presented in editing or documentation generation tools for
+    convenience.
+    """
+
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
+            "examples": [
+                {
+                    "title": "Sample Pet Store App",
+                    "summary": "A pet store manager.",
+                    "description": "This is a sample server for a pet store.",
+                    "termsOfService": "http://example.com/terms/",
+                    "contact": {
+                        "name": "API Support",
+                        "url": "http://www.example.com/support",
+                        "email": "support@example.com",
+                    },
+                    "license": {
+                        "name": "Apache 2.0",
+                        "url": "https://www.apache.org/licenses/LICENSE-2.0.html",
+                    },
+                    "version": "1.0.1",
+                }
+            ]
+        },
+    )
+
+    title: str
+    """
+    **REQUIRED**. The title of the API.
+    """
 
     summary: Optional[str] = None
     """
-    Short description for the example.
+    A short summary of the API.
     """
 
     description: Optional[str] = None
     """
-    Long description for the example.
+    A description of the API.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text representation.
     """
 
-    value: Optional[Any] = None
+    termsOfService: Optional[AnyUrl] = None
     """
-    Embedded literal example.
-    The `value` field and `externalValue` field are mutually exclusive.
-    To represent examples of media types that cannot naturally represented in JSON or YAML,
-    use a string value to contain the example, escaping where necessary.
+    A URL to the Terms of Service for the API.
+    MUST be in the form of a URL.
     """
 
-    externalValue: Optional[str] = None
+    contact: Optional[Contact] = None
+    """
+    The contact information for the exposed API.
     """
-    A URL that points to the literal example.
-    This provides the capability to reference examples that cannot easily be included in JSON or YAML documents.
 
-    The `value` field and `externalValue` field are mutually exclusive.
-    See the rules for resolving [Relative References](https://spec.openapis.org/oas/v3.1.0#relativeReferencesURI).
+    license: Optional[License] = None
+    """
+    The license information for the exposed API.
     """
 
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
-            "examples": [
-                {"summary": "A foo example", "value": {"foo": "bar"}},
-                {
-                    "summary": "This is an example in XML",
-                    "externalValue": "http://example.org/examples/address-example.xml",
-                },
-                {
-                    "summary": "This is a text example",
-                    "externalValue": "http://foo.bar/examples/address-example.txt",
-                },
-            ]
-        }
+    version: str
+    """
+    **REQUIRED**. The version of the OpenAPI document
+    (which is distinct from the [OpenAPI Specification version](https://spec.openapis.org/oas/v3.1.0#oasVersion)) or the API implementation version).
+    """
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/external_documentation.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/external_documentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import AnyUrl, BaseModel, ConfigDict
 
 
 class ExternalDocumentation(BaseModel):
     """Allows referencing an external resource for extended documentation."""
 
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
+            "examples": [{"description": "Find more info here", "url": "https://example.com"}]
+        },
+    )
+
     description: Optional[str] = None
     """
     A short description of the target documentation.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text representation.
     """
 
     url: AnyUrl
     """
     **REQUIRED**. The URL for the target documentation.
     Value MUST be in the form of a URL.
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
-            "examples": [{"description": "Find more info here", "url": "https://example.com"}]
-        }
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/header.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/server_variable.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from pydantic import Extra, Field
-from typing_extensions import Literal
+from typing import List, Optional
 
-from .parameter import Parameter
+from pydantic import BaseModel, ConfigDict
 
 
-class Header(Parameter):
-    """The Header Object follows the structure of the [Parameter
-    Object](https://spec.openapis.org/oas/v3.1.0#parameterObject) with the
-    following changes:
-
-    1. `name` MUST NOT be specified, it is given in the corresponding `headers` map.
-    2. `in` MUST NOT be specified, it is implicitly in `header`.
-    3. All traits that are affected by the location MUST be applicable to a location of `header`
-       (for example, [style](https://spec.openapis.org/oas/v3.1.0#parameterStyle)).
-    """
-
-    name: Literal[""] = Field(default="", const=True)
-    param_in: Literal["header"] = Field(default="header", const=True, alias="in")
-
-    class Config:
-        extra = Extra.ignore
-        allow_population_by_field_name = True
-        schema_extra = {
-            "examples": [
-                {
-                    "description": "The number of allowed requests in the current period",
-                    "schema": {"type": "integer"},
-                }
-            ]
-        }
+class ServerVariable(BaseModel):
+    """An object representing a Server Variable for server URL template
+    substitution."""
+
+    enum: Optional[List[str]] = None
+    """
+    An enumeration of string values to be used if the substitution options are from a limited set.
+    The array SHOULD NOT be empty.
+    """
+
+    default: str
+    """
+    **REQUIRED**. The default value to use for substitution,
+    which SHALL be sent if an alternate value is _not_ supplied.
+    Note this behavior is different than the [Schema Object's](https://spec.openapis.org/oas/v3.1.0#schemaObject) treatment of default values,
+    because in those cases parameter values are optional.
+    If the [enum](https://spec.openapis.org/oas/v3.1.0#serverVariableEnum) is defined, the value MUST exist in the enum's values.
+    """
+
+    description: Optional[str] = None
+    """
+    An optional description for the server variable.
+    [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text representation.
+    """
+    model_config = ConfigDict(extra="ignore")
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/license.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/license.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import AnyUrl, BaseModel, ConfigDict
 
 
 class License(BaseModel):
     """License information for the exposed API."""
 
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
+            "examples": [
+                {"name": "Apache 2.0", "identifier": "Apache-2.0"},
+                {"name": "Apache 2.0", "url": "https://www.apache.org/licenses/LICENSE-2.0.html"},
+            ]
+        },
+    )
+
     name: str
     """
     **REQUIRED**. The license name used for the API.
     """
 
     identifier: Optional[str] = None
     """
@@ -19,16 +29,7 @@
 
     url: Optional[AnyUrl] = None
     """
     A URL to the license used for the API.
     This MUST be in the form of a URL.
     The `url` field is mutually exclusive of the `identifier` field.
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
-            "examples": [
-                {"name": "Apache 2.0", "identifier": "Apache-2.0"},
-                {"name": "Apache 2.0", "url": "https://www.apache.org/licenses/LICENSE-2.0.html"},
-            ]
-        }
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/link.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .server import Server
 
 
 class Link(BaseModel):
     """The `Link object` represents a possible design-time link for a response.
     The presence of a link does not guarantee the caller's ability to
@@ -58,21 +58,22 @@
     """
 
     server: Optional[Server] = None
     """
     A server object to be used by the target operation.
     """
 
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "operationId": "getUserAddressByUUID",
                     "parameters": {"userUuid": "$response.body#/uuid"},
                 },
                 {
                     "operationRef": "#/paths/~12.0~1repositories~1{username}/get",
                     "parameters": {"username": "$response.body#/username"},
                 },
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/media_type.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/media_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from .encoding import Encoding
 from .example import Example
 from .reference import Reference
 from .schema import Schema
 
 
@@ -45,18 +45,18 @@
     """
     A map between a property name and its encoding information.
     The key, being the property name, MUST exist in the schema as a property.
     The encoding object SHALL only apply to `requestBody` objects
     when the media type is `multipart` or `application/x-www-form-urlencoded`.
     """
 
-    class Config:
-        extra = Extra.ignore
-        allow_population_by_field_name = True
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        populate_by_name=True,
+        json_schema_extra={
             "examples": [
                 {
                     "schema": {"$ref": "#/components/schemas/Pet"},
                     "examples": {
                         "cat": {
                             "summary": "An example of a cat",
                             "value": {
@@ -77,8 +77,9 @@
                                 "breed": "Mixed",
                             },
                         },
                         "frog": {"$ref": "#/components/examples/frog-example"},
                     },
                 }
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/oauth_flow.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/oauth_flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional, Union
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import AnyUrl, BaseModel, ConfigDict
 
 
 class OAuthFlow(BaseModel):
     """Configuration details for a supported OAuth Flow."""
 
     authorizationUrl: Optional[Union[AnyUrl, str]] = None
     """
@@ -32,17 +32,17 @@
     scopes: Optional[Dict[str, str]] = None
     """
     **REQUIRED** for `oauth2`. The available scopes for the OAuth2 security scheme.
     A map between the scope name and a short description for it.
     The map MAY be empty.
     """
 
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "authorizationUrl": "https://example.com/api/oauth/dialog",
                     "scopes": {
                         "write:pets": "modify pets in your account",
                         "read:pets": "read your pets",
                     },
@@ -61,8 +61,9 @@
                     "refreshUrl": "/api/oauth/token",  # issue #5: allow relative path
                     "scopes": {
                         "write:pets": "modify pets in your account",
                         "read:pets": "read your pets",
                     },
                 },
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/oauth_flows.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/oauth_flows.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .oauth_flow import OAuthFlow
 
 
 class OAuthFlows(BaseModel):
     """Allows configuration of the supported OAuth Flows."""
 
@@ -28,9 +28,8 @@
     authorizationCode: Optional[OAuthFlow] = None
     """
     Configuration for the OAuth Authorization Code flow.
 
     Previously called `accessCode` in OpenAPI 2.0.
     """
 
-    class Config:
-        extra = Extra.ignore
+    model_config = ConfigDict(extra="ignore")
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/open_api.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/open_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .components import Components
 from .external_documentation import ExternalDocumentation
 from .info import Info
 from .path_item import PathItem
 from .paths import Paths
 from .reference import Reference
@@ -83,9 +83,8 @@
     """
 
     externalDocs: Optional[ExternalDocumentation] = None
     """
     Additional external documentation.
     """
 
-    class Config:
-        extra = Extra.ignore
+    model_config = ConfigDict(extra="ignore")
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/operation.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .callback import Callback
 from .external_documentation import ExternalDocumentation
 from .parameter import Parameter
 from .reference import Reference
 from .request_body import RequestBody
 from .responses import Responses
@@ -101,18 +101,17 @@
 
     servers: Optional[List[Server]] = None
     """
     An alternative `server` array to service this operation.
     If an alternative `server` object is specified at the Path Item Object or Root level,
     it will be overridden by this value.
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "tags": ["pet"],
                     "summary": "Updates a pet in the store with form data",
                     "operationId": "updatePetWithForm",
                     "parameters": [
                         {
@@ -152,8 +151,9 @@
                             "description": "Method Not Allowed",
                             "content": {"application/json": {}, "application/xml": {}},
                         },
                     },
                     "security": [{"petstore_auth": ["write:pets", "read:pets"]}],
                 }
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/parameter.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from .example import Example
 from .media_type import MediaType
 from .reference import Reference
 from .schema import Schema
 
 
@@ -73,15 +73,15 @@
 
     - for `query` - `form`;
     - for `path` - `simple`;
     - for `header` - `simple`;
     - for `cookie` - `form`.
     """
 
-    explode: bool = False
+    explode: Optional[bool] = None
     """
     When this is true, parameter values of type `array` or `object` generate separate parameters
     for each value of the array or key-value pair of the map.
     For other types of parameters this property has no effect.
     When [style](https://spec.openapis.org/oas/v3.1.0#parameterStyle) is `form`, the default value is `true`.
     For all other styles, the default value is `false`.
     """
@@ -128,19 +128,18 @@
 
     content: Optional[Dict[str, MediaType]] = None
     """
     A map containing the representations for the parameter.
     The key is the media type and the value describes it.
     The map MUST only contain one entry.
     """
-
-    class Config:
-        extra = Extra.ignore
-        allow_population_by_field_name = True
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        populate_by_name=True,
+        json_schema_extra={
             "examples": [
                 {
                     "name": "token",
                     "in": "header",
                     "description": "token to be passed as a header",
                     "required": True,
                     "schema": {"type": "array", "items": {"type": "integer", "format": "int64"}},
@@ -181,8 +180,9 @@
                                     "long": {"type": "number"},
                                 },
                             }
                         }
                     },
                 },
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/path_item.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/path_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from .operation import Operation
 from .parameter import Parameter
 from .reference import Reference
 from .server import Server
 
 
@@ -87,19 +87,18 @@
     A list of parameters that are applicable for all the operations described under this path.
     These parameters can be overridden at the operation level, but cannot be removed there.
     The list MUST NOT include duplicated parameters.
     A unique parameter is defined by a combination of a [name](https://spec.openapis.org/oas/v3.1.0#parameterName) and [location](https://spec.openapis.org/oas/v3.1.0#parameterIn).
     The list can use the [Reference Object](https://spec.openapis.org/oas/v3.1.0#referenceObject) to link to parameters that are defined at the
     [OpenAPI Object's components/parameters](https://spec.openapis.org/oas/v3.1.0#componentsParameters).
     """
-
-    class Config:
-        extra = Extra.ignore
-        allow_population_by_field_name = True
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        populate_by_name=True,
+        json_schema_extra={
             "examples": [
                 {
                     "get": {
                         "description": "Returns pets based on ID",
                         "summary": "Find pets by ID",
                         "operationId": "getPetsById",
                         "responses": {
@@ -132,8 +131,9 @@
                             "required": True,
                             "schema": {"type": "array", "items": {"type": "string"}},
                             "style": "simple",
                         }
                     ],
                 }
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/paths.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/reference.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 
 class Reference(BaseModel):
     """A simple object to allow referencing other components in the OpenAPI
     document, internally and externally.
 
     The `$ref` string value contains a URI [RFC3986](https://tools.ietf.org/html/rfc3986),
@@ -24,18 +24,18 @@
 
     description: Optional[str] = None
     """
     A description which by default SHOULD override that of the referenced component.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text representation.
     If the referenced object-type does not allow a `description` field, then this field has no effect.
     """
-
-    class Config:
-        extra = Extra.ignore
-        allow_population_by_field_name = True
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        populate_by_name=True,
+        json_schema_extra={
             "examples": [
                 {"$ref": "#/components/schemas/Pet"},
                 {"$ref": "Pet.json"},
                 {"$ref": "definitions.json#/Pet"},
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/request_body.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/request_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .media_type import MediaType
 
 
 class RequestBody(BaseModel):
     """Describes a single request body."""
 
@@ -25,18 +25,17 @@
     For requests that match multiple keys, only the most specific key is applicable. e.g. text/plain overrides text/*
     """
 
     required: bool = False
     """
     Determines if the request body is required in the request. Defaults to `false`.
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "description": "user to add to the system",
                     "content": {
                         "application/json": {
                             "schema": {"$ref": "#/components/schemas/User"},
                             "examples": {
@@ -76,8 +75,9 @@
                 {
                     "description": "user to add to the system",
                     "content": {
                         "text/plain": {"schema": {"type": "array", "items": {"type": "string"}}}
                     },
                 },
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/response.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional, Union
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .header import Header
 from .link import Link
 from .media_type import MediaType
 from .reference import Reference
 
 
@@ -36,18 +36,17 @@
 
     links: Optional[Dict[str, Union[Link, Reference]]] = None
     """
     A map of operations links that can be followed from the response.
     The key of the map is a short name for the link,
     following the naming constraints of the names for `Component Objects <https://spec.openapis.org/oas/v3.1.0#componentsObject).
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "description": "A complex object array response",
                     "content": {
                         "application/json": {
                             "schema": {
                                 "type": "array",
@@ -76,8 +75,9 @@
                             "description": "The number of seconds left in the current period",
                             "schema": {"type": "integer"},
                         },
                     },
                 },
                 {"description": "object created"},
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/responses.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/schema.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from .discriminator import Discriminator
 from .external_documentation import ExternalDocumentation
 from .reference import Reference
 from .xml import XML
 
 
@@ -364,15 +364,15 @@
     "boolean", "object", "array", "number", or "string"), or "integer"
     which matches any number with a zero fractional part.
 
     An instance validates if and only if the instance is in any of the
     sets listed for this keyword.
     """
 
-    enum: Optional[List[Any]] = Field(default=None, min_items=1)
+    enum: Optional[List[Any]] = Field(default=None, min_length=1)
     """
     The value of this keyword MUST be an array.  This array SHOULD have
     at least one element.  Elements in the array SHOULD be unique.
 
     An instance validates successfully against this keyword if its value
     is equal to one of the elements in this keyword's array value.
 
@@ -819,19 +819,18 @@
     A free-form property to include an example of an instance for this schema.
     To represent examples that cannot be naturally represented in JSON or YAML,
     a string value can be used to contain the example with escaping where necessary.
 
     Deprecated: The example property has been deprecated in favor of the JSON Schema examples keyword.
     Use of example is discouraged, and later versions of this specification may remove it.
     """
-
-    class Config:
-        extra = Extra.ignore
-        allow_population_by_field_name = True
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        populate_by_name=True,
+        json_schema_extra={
             "examples": [
                 {"type": "string", "format": "email"},
                 {
                     "type": "object",
                     "required": ["name"],
                     "properties": {
                         "name": {"type": "string"},
@@ -913,8 +912,9 @@
                                 }
                             },
                             "required": ["packSize"],
                         },
                     ],
                 },
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/security_requirement.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/security_scheme.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/security_scheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-from pydantic import AnyUrl, BaseModel, Extra, Field
+from pydantic import AnyUrl, BaseModel, ConfigDict, Field
 from typing_extensions import Literal
 
 from .oauth_flows import OAuthFlows
 
 
 class SecurityScheme(BaseModel):
     """Defines a security scheme that can be used by the operations.
@@ -67,19 +67,18 @@
     """
 
     openIdConnectUrl: Optional[Union[AnyUrl, str]] = None
     """
     **REQUIRED** for `openIdConnect`. OpenId Connect URL to discover OAuth2 configuration values.
     This MUST be in the form of a URL. The OpenID Connect standard requires the use of TLS.
     """
-
-    class Config:
-        extra = Extra.ignore
-        allow_population_by_field_name = True
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        populate_by_name=True,
+        json_schema_extra={
             "examples": [
                 {"type": "http", "scheme": "basic"},
                 {"type": "apiKey", "name": "api_key", "in": "header"},
                 {"type": "http", "scheme": "bearer", "bearerFormat": "JWT"},
                 {
                     "type": "oauth2",
                     "flows": {
@@ -94,8 +93,9 @@
                 },
                 {"type": "openIdConnect", "openIdConnectUrl": "https://example.com/openIdConnect"},
                 {
                     "type": "openIdConnect",
                     "openIdConnectUrl": "openIdConnect",
                 },  # issue #5: allow relative path
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/server.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .server_variable import ServerVariable
 
 
 class Server(BaseModel):
     """An object representing a Server."""
 
@@ -25,18 +25,17 @@
 
     variables: Optional[Dict[str, ServerVariable]] = None
     """
     A map between a variable name and its value.
 
     The value is used for substitution in the server's URL template.
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {
                     "url": "https://development.gigantic-server.com/v1",
                     "description": "Development server",
                 },
                 {
                     "url": "https://{username}.gigantic-server.com:{port}/{basePath}",
@@ -48,8 +47,9 @@
                             "in this example `gigantic-server.com`",
                         },
                         "port": {"enum": ["8443", "443"], "default": "8443"},
                         "basePath": {"default": "v2"},
                     },
                 },
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/tag.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 from .external_documentation import ExternalDocumentation
 
 
 class Tag(BaseModel):
     """Adds metadata to a single tag that is used by the [Operation
     Object](https://spec.openapis.org/oas/v3.1.0#operationObject).
@@ -24,11 +24,11 @@
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text representation.
     """
 
     externalDocs: Optional[ExternalDocumentation] = None
     """
     Additional external documentation for this tag.
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {"examples": [{"name": "pet", "description": "Pets operations"}]}
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={"examples": [{"name": "pet", "description": "Pets operations"}]},
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/openapi_schemas_pydantic/v3_1_0/xml.py` & `openapi_schemas_pydantic-2.0.0/openapi_schemas_pydantic/v3_1_0/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel, ConfigDict
 
 
 class XML(BaseModel):
     """A metadata object that allows for more fine-tuned XML model definitions.
 
     When using arrays, XML element names are *not* inferred (for
     singular/plural forms) and the `name` property SHOULD be used to add
@@ -41,19 +41,19 @@
     """
     MAY be used only for an array definition.
     Signifies whether the array is wrapped (for example, `<books><book/><book/></books>`)
     or unwrapped (`<book/><book/>`).
     Default value is `false`.
     The definition takes effect only when defined alongside `type` being `array` (outside the `items`).
     """
-
-    class Config:
-        extra = Extra.ignore
-        schema_extra = {
+    model_config = ConfigDict(
+        extra="ignore",
+        json_schema_extra={
             "examples": [
                 {"name": "animal"},
                 {"attribute": True},
                 {"wrapped": True},
                 {"namespace": "http://example.com/schema/sample", "prefix": "sample"},
                 {"name": "aliens", "wrapped": True},
             ]
-        }
+        },
+    )
```

### Comparing `openapi_schemas_pydantic-1.1.0/LICENSE` & `openapi_schemas_pydantic-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_schemas_pydantic-1.1.0/README.md` & `openapi_schemas_pydantic-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_schemas_pydantic-1.1.0/pyproject.toml` & `openapi_schemas_pydantic-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "openapi-schemas-pydantic"
 dynamic = ['version']
 description = "OpenAPI Schema using pydantic. Forked for Esmerald."
 long_description = "OpenAPI Schema using pydantic. Forked for Esmerald."
-authors = [
-    { name = "Tiago Silva", email = "tiago.silva@dymmond.com" },
-]
-requires-python = ">=3.7"
+authors = [{ name = "Tiago Silva", email = "tiago.silva@dymmond.com" }]
+requires-python = ">=3.8"
 readme = "README.md"
 license = "MIT"
-keywords = ["OpenAPI", "open-api", "esmerald", "pydantic", "schema"]
+keywords = [
+    "OpenAPI",
+    "open-api",
+    "openapi_schemas_pydantic",
+    "pydantic",
+    "schema",
+]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
@@ -28,16 +32,17 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "pydantic >1.10.0,<2.0.0",
-    "email-validator >=1.2.1,<2.0.0"
+    "pydantic>=2.0.0,<3.0.0",
+    "pydantic-extra-types>=2.0.0,<3.0.0",
+    "email-validator >=1.2.1,<2.0.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dymmond/openapi-schemas-pydantic"
 Documentation = "https://openapi-schemas.dymmond.com/"
 Changelog = "https://openapi-schemas.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
@@ -47,47 +52,74 @@
 test = [
     "pytest >=7.1.3,<8.0.0",
     "pytest-cov >=2.12.0,<4.0.0",
     "pytest-asyncio >=0.19.0,<0.20.0",
 ]
 
 dev = [
-    "pre-commit >=2.17.0,<3.0.0",
+    "black>=23.0.0,<30.0.0",
+    "isort>=5.12.0,<6.0.0",
+    "mypy==1.4.1",
+    "pre-commit>=2.17.0,<3.0.0",
+    "ruff>=0.0.275,<1.0.0",
 ]
 
 doc = [
     "mkautodoc >=0.2.0,<0.3.0",
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=8.1.4,<9.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
     "mkdocstrings>=0.19.0,<0.20.0",
     "pyyaml >=5.3.1,<7.0.0",
 ]
 
+[tool.ruff]
+select = [
+    "E", # pycodestyle errors
+    "W", # pycodestyle warnings
+    "F", # pyflakes
+    "C", # flake8-comprehensions
+    "B", # flake8-bugbear
+]
+ignore = [
+    "E501", # line too long, handled by black
+    "B008", # do not perform function calls in argument defaults
+    "C901", # too complex
+]
+
+exclude = ["docs/*"]
+
+
 [tool.hatch.version]
 path = "openapi_schemas_pydantic/__init__.py"
 
 [tool.isort]
 profile = "black"
 known_third_party = ["esmerald", "pydantic", "starlette"]
 
 [tool.mypy]
 strict = true
+warn_unused_configs = true
+warn_unreachable = true
+warn_return_any = true
+disallow_untyped_decorators = true
+disallow_any_generics = false
+implicit_reexport = false
+show_error_codes = true
+disallow_incomplete_defs = true
+disable_error_code = "attr-defined"
+warn_unused_ignores = true
+warn_redundant_casts = true
 
 [[tool.mypy.overrides]]
 module = "openapi-schemas-pydantic.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.pytest.ini_options]
-addopts = [
-  "--strict-config",
-  "--strict-markers",
-]
+addopts = ["--strict-config", "--strict-markers"]
 xfail_strict = true
 junit_family = "xunit2"
 
 [tool.hatch.build.targets.sdist]
-include = [
-    "/openapi_schemas_pydantic",
-]
+include = ["/openapi_schemas_pydantic"]
```

### Comparing `openapi_schemas_pydantic-1.1.0/PKG-INFO` & `openapi_schemas_pydantic-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 Metadata-Version: 2.1
 Name: openapi-schemas-pydantic
-Version: 1.1.0
+Version: 2.0.0
 Summary: OpenAPI Schema using pydantic. Forked for Esmerald.
 Project-URL: Homepage, https://github.com/dymmond/openapi-schemas-pydantic
 Project-URL: Documentation, https://openapi-schemas.dymmond.com/
 Project-URL: Changelog, https://openapi-schemas.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/openapi-schemas-pydantic
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
+License-Expression: MIT
 License-File: LICENSE
-Keywords: OpenAPI,esmerald,open-api,pydantic,schema
+Keywords: OpenAPI,open-api,openapi_schemas_pydantic,pydantic,schema
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: email-validator<2.0.0,>=1.2.1
-Requires-Dist: pydantic<2.0.0,>1.10.0
+Requires-Dist: pydantic-extra-types<3.0.0,>=2.0.0
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Provides-Extra: dev
+Requires-Dist: black<30.0.0,>=23.0.0; extra == 'dev'
+Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'dev'
+Requires-Dist: mypy==1.4.1; extra == 'dev'
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
+Requires-Dist: ruff<1.0.0,>=0.0.275; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
 Requires-Dist: mkdocstrings<0.20.0,>=0.19.0; extra == 'doc'
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1 Name: openapi-schemas-pydantic Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: openapi-schemas-pydantic Version: 2.0.0 Summary:
 OpenAPI Schema using pydantic. Forked for Esmerald. Project-URL: Homepage,
 https://github.com/dymmond/openapi-schemas-pydantic Project-URL: Documentation,
 https://openapi-schemas.dymmond.com/ Project-URL: Changelog, https://openapi-
 schemas.dymmond.com/release-notes/ Project-URL: Funding, https://github.com/
 sponsors/tarsil Project-URL: Source, https://github.com/dymmond/openapi-
 schemas-pydantic Author-email: Tiago Silva
-silva@dymmond.com> License-File: LICENSE Keywords: OpenAPI,esmerald,open-
-api,pydantic,schema Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: English Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
-HTTP Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries Classifier: Typing :: Typed Requires-Python: >=3.7
-Requires-Dist: email-validator<2.0.0,>=1.2.1 Requires-Dist:
-pydantic<2.0.0,>1.10.0 Provides-Extra: dev Requires-Dist: pre-
-commit<3.0.0,>=2.17.0; extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-
-include<2.0.0,>=1.4.1; extra == 'doc' Requires-Dist: mkautodoc<0.3.0,>=0.2.0;
-extra == 'doc' Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7;
-extra == 'doc' Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
-Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc' Requires-Dist:
+silva@dymmond.com> License-Expression: MIT License-File: LICENSE Keywords:
+OpenAPI,open-api,openapi_schemas_pydantic,pydantic,schema Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Web
+Environment Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Software Development Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed Requires-Python: >=3.8 Requires-Dist: email-
+validator<2.0.0,>=1.2.1 Requires-Dist: pydantic-extra-types<3.0.0,>=2.0.0
+Requires-Dist: pydantic<3.0.0,>=2.0.0 Provides-Extra: dev Requires-Dist:
+black<30.0.0,>=23.0.0; extra == 'dev' Requires-Dist: isort<6.0.0,>=5.12.0;
+extra == 'dev' Requires-Dist: mypy==1.4.1; extra == 'dev' Requires-Dist: pre-
+commit<3.0.0,>=2.17.0; extra == 'dev' Requires-Dist: ruff<1.0.0,>=0.0.275;
+extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-include<2.0.0,>=1.4.1;
+extra == 'doc' Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc' Requires-
+Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc' Requires-
+Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist:
+mkdocs<2.0.0,>=1.1.2; extra == 'doc' Requires-Dist:
 mkdocstrings<0.20.0,>=0.19.0; extra == 'doc' Requires-Dist:
 pyyaml<7.0.0,>=5.3.1; extra == 'doc' Provides-Extra: test Requires-Dist:
 pytest-asyncio<0.20.0,>=0.19.0; extra == 'test' Requires-Dist: pytest-
 cov<4.0.0,>=2.12.0; extra == 'test' Requires-Dist: pytest<8.0.0,>=7.1.3; extra
 == 'test' Description-Content-Type: text/markdown # OpenAPI Schemas for
 Pydantic
                                   [Esmerald]
```

