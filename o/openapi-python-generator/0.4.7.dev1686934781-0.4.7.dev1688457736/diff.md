# Comparing `tmp/openapi_python_generator-0.4.7.dev1686934781.tar.gz` & `tmp/openapi_python_generator-0.4.7.dev1688457736.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_python_generator-0.4.7.dev1686934781.tar", max compression
+gzip compressed data, was "openapi_python_generator-0.4.7.dev1688457736.tar", max compression
```

## Comparing `openapi_python_generator-0.4.7.dev1686934781.tar` & `openapi_python_generator-0.4.7.dev1688457736.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-06-16 16:59:29.219453 openapi_python_generator-0.4.7.dev1686934781/LICENSE
--rw-r--r--   0        0        0     4118 2023-06-16 16:59:29.219453 openapi_python_generator-0.4.7.dev1686934781/README.md
--rw-r--r--   0        0        0     2171 2023-06-16 16:59:41.843634 openapi_python_generator-0.4.7.dev1686934781/pyproject.toml
--rw-r--r--   0        0        0      476 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/__init__.py
--rw-r--r--   0        0        0     1622 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/__main__.py
--rw-r--r--   0        0        0      959 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/common.py
--rw-r--r--   0        0        0     4970 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/generate_data.py
--rw-r--r--   0        0        0        0 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/__init__.py
--rw-r--r--   0        0        0      740 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/api_config_generator.py
--rw-r--r--   0        0        0      921 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/common.py
--rw-r--r--   0        0        0     1296 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/generator.py
--rw-r--r--   0        0        0      426 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/jinja_config.py
--rw-r--r--   0        0        0    12001 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/model_generator.py
--rw-r--r--   0        0        0    13109 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/service_generator.py
--rw-r--r--   0        0        0     1977 2023-06-16 16:59:29.223453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2
--rw-r--r--   0        0        0     1256 2023-06-16 16:59:29.227453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2
--rw-r--r--   0        0        0      242 2023-06-16 16:59:29.227453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/enum.jinja2
--rw-r--r--   0        0        0     2143 2023-06-16 16:59:29.227453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2
--rw-r--r--   0        0        0      671 2023-06-16 16:59:29.227453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/models.jinja2
--rw-r--r--   0        0        0     1874 2023-06-16 16:59:29.227453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/requests.jinja2
--rw-r--r--   0        0        0      202 2023-06-16 16:59:29.227453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/service.jinja2
--rw-r--r--   0        0        0     1726 2023-06-16 16:59:29.227453 openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/models.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.7.dev1686934781/setup.py
--rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.7.dev1686934781/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-04 08:02:02.298473 openapi_python_generator-0.4.7.dev1688457736/LICENSE
+-rw-r--r--   0        0        0     4118 2023-07-04 08:02:02.298473 openapi_python_generator-0.4.7.dev1688457736/README.md
+-rw-r--r--   0        0        0     2171 2023-07-04 08:02:17.310577 openapi_python_generator-0.4.7.dev1688457736/pyproject.toml
+-rw-r--r--   0        0        0      476 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/__init__.py
+-rw-r--r--   0        0        0     1622 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/__main__.py
+-rw-r--r--   0        0        0      959 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/common.py
+-rw-r--r--   0        0        0     4970 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/generate_data.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/api_config_generator.py
+-rw-r--r--   0        0        0      922 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/common.py
+-rw-r--r--   0        0        0     1296 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/generator.py
+-rw-r--r--   0        0        0      426 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/jinja_config.py
+-rw-r--r--   0        0        0    12151 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/model_generator.py
+-rw-r--r--   0        0        0    13135 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/service_generator.py
+-rw-r--r--   0        0        0     1977 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2
+-rw-r--r--   0        0        0     1256 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2
+-rw-r--r--   0        0        0      242 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/enum.jinja2
+-rw-r--r--   0        0        0     2131 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2
+-rw-r--r--   0        0        0      671 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/models.jinja2
+-rw-r--r--   0        0        0     1874 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/requests.jinja2
+-rw-r--r--   0        0        0      202 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/service.jinja2
+-rw-r--r--   0        0        0     1726 2023-07-04 08:02:02.302473 openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/models.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.7.dev1688457736/setup.py
+-rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.7.dev1688457736/PKG-INFO
```

### Comparing `openapi_python_generator-0.4.7.dev1686934781/LICENSE` & `openapi_python_generator-0.4.7.dev1688457736/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/README.md` & `openapi_python_generator-0.4.7.dev1688457736/README.md`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/pyproject.toml` & `openapi_python_generator-0.4.7.dev1688457736/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-python-generator"
-version = "0.4.7.dev.1686934781"
+version = "0.4.7.dev.1688457736"
 description = "Openapi Python Generator"
 authors = ["Marco Müllner <muellnermarco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MarcoMuellner/openapi-python-generator"
 repository = "https://github.com/MarcoMuellner/openapi-python-generator"
 documentation = "https://openapi-python-generator.readthedocs.io"
```

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/__main__.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/common.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/common.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/generate_data.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/generate_data.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/api_config_generator.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/api_config_generator.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/common.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import keyword
 import re
 
+
 _use_orjson: bool = False
 _symbol_ascii_strip_re = re.compile(r"[^A-Za-z0-9_]")
 
 
 def set_use_orjson(value: bool) -> None:
     """
     Set the value of the global variable _use_orjson.
@@ -26,11 +27,11 @@
 def normalize_symbol(symbol: str) -> str:
     """
     Remove invalid characters & keywords in Python symbol names
     :param symbol: name of the identifier
     :return: normalized identifier name
     """
     symbol = symbol.replace("-", "_")
-    normalized_symbol = _symbol_ascii_strip_re.sub('', symbol)
+    normalized_symbol = _symbol_ascii_strip_re.sub("", symbol)
     if normalized_symbol in keyword.kwlist:
-        normalized_symbol = normalized_symbol + '_'
+        normalized_symbol = normalized_symbol + "_"
     return normalized_symbol
```

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/generator.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/generator.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/model_generator.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/model_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,19 @@
     MODELS_TEMPLATE,
 )
 from openapi_python_generator.models import Model
 from openapi_python_generator.models import Property
 from openapi_python_generator.models import TypeConversion
 
 
-def type_converter(schema: Schema,  required: bool = False, model_name: Optional[str] = None,) -> TypeConversion:
+def type_converter(  # noqa: C901
+    schema: Schema,
+    required: bool = False,
+    model_name: Optional[str] = None,
+) -> TypeConversion:
     """
     Converts an OpenAPI type to a Python type.
     :param schema: Schema containing the type to be converted
     :param model_name: Name of the original model on which the type is defined
     :param required: Flag indicating if the type is required by the class
     :return: The converted type
     """
@@ -115,15 +119,19 @@
         )
     # We only want to auto convert to datetime if orjson is used throghout the code, otherwise we can not
     # serialize it to JSON.
     elif schema.type == "string" and (
         schema.schema_format is None or not common.get_use_orjson()
     ):
         converted_type = pre_type + "str" + post_type
-    elif schema.type == "string" and schema.schema_format.startswith("uuid") and common.get_use_orjson():
+    elif (
+        schema.type == "string"
+        and schema.schema_format.startswith("uuid")
+        and common.get_use_orjson()
+    ):
         if len(schema.schema_format) > 4 and schema.schema_format[4].isnumeric():
             uuid_type = schema.schema_format.upper()
             converted_type = pre_type + uuid_type + post_type
             import_types = ["from pydantic import " + uuid_type]
         else:
             converted_type = pre_type + "UUID" + post_type
             import_types = ["from uuid import UUID"]
@@ -135,15 +143,17 @@
     elif schema.type == "number":
         converted_type = pre_type + "float" + post_type
     elif schema.type == "boolean":
         converted_type = pre_type + "bool" + post_type
     elif schema.type == "array":
         retVal = pre_type + "List["
         if isinstance(schema.items, Reference):
-            converted_reference = _generate_property_from_reference(model_name, "", schema.items, schema, required)
+            converted_reference = _generate_property_from_reference(
+                model_name, "", schema.items, schema, required
+            )
             import_types = converted_reference.type.import_types
             original_type = "array<" + converted_reference.type.original_type + ">"
             retVal += converted_reference.type.converted_type
         elif isinstance(schema.items, Schema):
             original_type = "array<" + str(schema.items.type) + ">"
             retVal += type_converter(schema.items, True).converted_type
         else:
@@ -162,15 +172,15 @@
         original_type=original_type,
         converted_type=converted_type,
         import_types=import_types,
     )
 
 
 def _generate_property_from_schema(
-    model_name : str, name: str, schema: Schema, parent_schema: Optional[Schema] = None
+    model_name: str, name: str, schema: Schema, parent_schema: Optional[Schema] = None
 ) -> Property:
     """
     Generates a property from a schema. It takes the type of the schema and converts it to a python type, and then
     creates the according property.
     :param model_name: Name of the model this property belongs to
     :param name: Name of the schema
     :param schema: schema to be converted
@@ -187,15 +197,19 @@
         type=type_converter(schema, required, model_name),
         required=required,
         default=None if required else "None",
     )
 
 
 def _generate_property_from_reference(
-        model_name: str, name: str, reference: Reference, parent_schema: Optional[Schema] = None, force_required: bool = False
+    model_name: str,
+    name: str,
+    reference: Reference,
+    parent_schema: Optional[Schema] = None,
+    force_required: bool = False,
 ) -> Property:
     """
     Generates a property from a reference. It takes the name of the reference as the type, and then
     returns a property type
     :param name: Name of the schema
     :param reference: reference to be converted
     :param parent_schema: Component this belongs to
@@ -208,21 +222,25 @@
         and name in parent_schema.required
     ) or force_required
     import_model = reference.ref.split("/")[-1]
 
     if import_model == model_name:
         type_conv = TypeConversion(
             original_type=reference.ref,
-            converted_type=import_model if required else 'Optional["' + import_model + '"]',
-            import_types=None
+            converted_type=import_model
+            if required
+            else 'Optional["' + import_model + '"]',
+            import_types=None,
         )
     else:
         type_conv = TypeConversion(
             original_type=reference.ref,
-            converted_type=import_model if required else "Optional[" + import_model + "]",
+            converted_type=import_model
+            if required
+            else "Optional[" + import_model + "]",
             import_types=[f"from .{import_model} import {import_model}"],
         )
     return Property(
         name=name,
         type=type_conv,
         required=required,
         default=None if required else "None",
```

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/service_generator.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/service_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
-from typing import Dict, Literal
+from typing import Dict
 from typing import List
+from typing import Literal
 from typing import Tuple
 from typing import Union
 
 import click
 from openapi_schema_pydantic import MediaType
 from openapi_schema_pydantic import Operation
 from openapi_schema_pydantic import Parameter
@@ -155,32 +156,37 @@
 def generate_operation_id(operation: Operation, http_op: str) -> str:
     if operation.operationId is not None:
         return common.normalize_symbol(operation.operationId)
     else:
         raise Exception(f"OperationId is not defined for {http_op}")  # pragma: no cover
 
 
-def _generate_params(operation: Operation, param_in : Literal["query", "header"] = "query"):
+def _generate_params(
+    operation: Operation, param_in: Literal["query", "header"] = "query"
+):
     if operation.parameters is None:
         return []
 
     params = []
     for param in operation.parameters:
         if isinstance(param, Parameter) and param.param_in == param_in:
             param_name_cleaned = common.normalize_symbol(param.name)
-            params.append(f"'{param.name}' : {param_name_cleaned}")
+            params.append(f"{param.name!r} : {param_name_cleaned}")
 
     return params
 
+
 def generate_query_params(operation: Operation) -> List[str]:
     return _generate_params(operation, "query")
 
+
 def generate_header_params(operation: Operation) -> List[str]:
     return _generate_params(operation, "header")
 
+
 def generate_return_type(operation: Operation) -> OpReturnType:
     if operation.responses is None:
         return OpReturnType(type=None, status_code=200, complex_type=False)
 
     good_responses: List[Tuple[int, Union[Response, Reference]]] = [
         (int(status_code), response)
         for status_code, response in operation.responses.items()
```

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         httpx.URL(path),
         headers=headers,
         params=query_params,
         {% if body_param %}
         {% if use_orjson %}
         content=orjson.dumps({{ body_param }})
         {% else %}
-        json = json.dumps({{ body_param }})
+        json = {{ body_param }}
         {% endif %}
         {% endif %}
     )
 
     if response.status_code != {{ return_type.status_code }}:
         raise HTTPException(response.status_code, f'{{ operationId }} failed with status code: {response.status_code}')
```

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/models.jinja2` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/models.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/language_converters/python/templates/requests.jinja2` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/language_converters/python/templates/requests.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/src/openapi_python_generator/models.py` & `openapi_python_generator-0.4.7.dev1688457736/src/openapi_python_generator/models.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1686934781/setup.py` & `openapi_python_generator-0.4.7.dev1688457736/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 entry_points = \
 {'console_scripts': ['openapi-python-generator = '
                      'openapi_python_generator.__main__:main']}
 
 setup_kwargs = {
     'name': 'openapi-python-generator',
-    'version': '0.4.7.dev1686934781',
+    'version': '0.4.7.dev1688457736',
     'description': 'Openapi Python Generator',
     'long_description': "# Openapi Python Generator\n\n[![PyPI](https://img.shields.io/pypi/v/openapi-python-generator.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/openapi-python-generator.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/openapi-python-generator)][python version]\n[![License](https://img.shields.io/pypi/l/openapi-python-generator)][license]\n\n[![](https://img.shields.io/static/v1?label=documentation&message=enabled&color=<COLOR>)][documentation]\n[![Tests](https://github.com/MarcoMuellner/openapi-python-generator/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/MarcoMuellner/openapi-python-generator/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/openapi-python-generator/\n[status]: https://pypi.org/project/openapi-python-generator/\n[python version]: https://pypi.org/project/openapi-python-generator\n[documentation]: https://marcomuellner.github.io/openapi-python-generator/\n[tests]: https://github.com/MarcoMuellner/openapi-python-generator/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/MarcoMuellner/openapi-python-generator\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n![](logo.png)\n\n---\n__Documentation:__ [here][documentation]\n\n---\n\n## Features\n\n- __Ease of use__. Provide input, output and the library, and the generator will do the rest.\n- __Type safety and type hinting.__ __OpenAPI python generator__ makes heavy use of pydantic models to provide type-safe data structures.\n- __Support for multiple rest frameworks.__ __OpenAPI python generator__ currently supports the following:\n    - [httpx](https://pypi.org/project/httpx/)\n    - [requests](https://pypi.org/project/requests/)\n    - [aiohttp](https://pypi.org/project/aiohttp/)\n- __Async and sync code generation support__, depending on the framework. It will automatically create both for frameworks that support both.\n- __Easily extendable using Jinja2 templates__. The code is designed to be easily extendable and should support even more languages and frameworks in the future.\n- __Fully tested__. Every generated code is automatically tested against the OpenAPI spec and we have 100% coverage.\n- __Usage as CLI or as library__.\n\n## Requirements\n\n- Python 3.7+\n\n## Installation\n\nYou can install _Openapi Python Generator_ via [pip] from [PyPI]:\n\n```console\n$ pip install openapi-python-generator\n```\n\n## Usage\n\nPlease see the [Quick start page] for details.\n\n## Roadmap\n\n- Support for all commonly used http libraries in the python ecosystem (~~requests~~, urllib, ...)\n- Support for multiple languages\n- Support for multiple authentication schemes\n- Support custom themes\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Openapi Python Generator_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nSpecial thanks to the peeps from [openapi-schema-pydantic](https://github.com/kuimono/openapi-schema-pydantic),\nwhich already did a lot of the legwork by providing a pydantic schema for the OpenAPI 3.0.0+ specification.\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/MarcoMuellner/openapi-python-generator/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/MarcoMuellner/openapi-python-generator/blob/main/LICENSE\n[contributor guide]: https://github.com/MarcoMuellner/openapi-python-generator/blob/main/CONTRIBUTING.md\n[Quick start page]: https://marcomuellner.github.io/openapi-python-generator/quick_start/\n",
     'author': 'Marco Müllner',
     'author_email': 'muellnermarco@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MarcoMuellner/openapi-python-generator',
```

### Comparing `openapi_python_generator-0.4.7.dev1686934781/PKG-INFO` & `openapi_python_generator-0.4.7.dev1688457736/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-python-generator
-Version: 0.4.7.dev1686934781
+Version: 0.4.7.dev1688457736
 Summary: Openapi Python Generator
 Home-page: https://github.com/MarcoMuellner/openapi-python-generator
 License: MIT
 Keywords: OpenAPI,Generator,Python,async
 Author: Marco Müllner
 Author-email: muellnermarco@gmail.com
 Requires-Python: >=3.7,<4.0
```

