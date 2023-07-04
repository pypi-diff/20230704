# Comparing `tmp/powertools_oas_validator-0.5.2.tar.gz` & `tmp/powertools_oas_validator-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.5.2.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.5.3.tar", max compression
```

## Comparing `powertools_oas_validator-0.5.2.tar` & `powertools_oas_validator-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-07-04 12:25:36.948770 powertools_oas_validator-0.5.2/LICENSE
--rw-r--r--   0        0        0     2327 2023-07-04 12:25:36.948770 powertools_oas_validator-0.5.2/README.md
--rw-r--r--   0        0        0       13 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      199 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0     1031 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     4508 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/services/error_handler.py
--rw-r--r--   0        0        0     3196 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     2166 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1805 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      975 2023-07-04 12:25:36.952770 powertools_oas_validator-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.2/setup.py
--rw-r--r--   0        0        0     3177 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-04 15:51:03.772420 powertools_oas_validator-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2327 2023-07-04 15:51:03.772420 powertools_oas_validator-0.5.3/README.md
+-rw-r--r--   0        0        0       13 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1031 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     4720 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/error_handler.py
+-rw-r--r--   0        0        0     3196 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     2166 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1805 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      975 2023-07-04 15:51:03.776420 powertools_oas_validator-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.3/setup.py
+-rw-r--r--   0        0        0     3177 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.3/PKG-INFO
```

### Comparing `powertools_oas_validator-0.5.2/LICENSE` & `powertools_oas_validator-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/README.md` & `powertools_oas_validator-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/overrides/validators.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/services/error_handler.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/services/error_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Union
 
 from aws_lambda_powertools.utilities.validation.exceptions import SchemaValidationError
 from openapi_core.templating.security.exceptions import SecurityNotFound
 from openapi_core.validation.request.exceptions import ParameterValidationError
 from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
 
+from powertools_oas_validator.exceptions import UnhandledValidationError
 from powertools_oas_validator.types import Request
 
 
 class ErrorHandler:
     @staticmethod
     def raise_schema_validation_error(
         ex: Union[ParameterValidationError, InvalidSchemaValue, SecurityNotFound],
@@ -20,16 +21,18 @@
         if issubclass(ex_type, ParameterValidationError):
             error = ErrorHandler._handle_parameter_error(ex, request)  # type: ignore
         elif ex_type == InvalidSchemaValue:
             error = ErrorHandler._handle_body_error(ex, request)  # type: ignore
         elif ex_type == SecurityNotFound:
             error = ErrorHandler._handle_security_error(ex, request)  # type: ignore
         else:
-            raise ValueError(
-                f"'{ex_type}' is not mapped to a function. Consider adding it."
+            raise UnhandledValidationError(
+                f"'{ex_type}' is unhandled. Please open an issue on:"
+                + "https://github.com/RasmusFangel/powertools-oas-validator/issues"
+                + " and it will be resolved ASAP!"
             )
         raise error
 
     @staticmethod
     def _handle_security_error(
         ex: SecurityNotFound, request: Request
     ) -> SchemaValidationError:
```

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/powertools_oas_validator/types.py` & `powertools_oas_validator-0.5.3/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.2/pyproject.toml` & `powertools_oas_validator-0.5.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.5.2"
+version = "0.5.3"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 homepage = "https://github.com/RasmusFangel/powertools-oas-validator"
 repository = "https://github.com/RasmusFangel/powertools-oas-validator"
```

### Comparing `powertools_oas_validator-0.5.2/setup.py` & `powertools_oas_validator-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': '',
     'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://badge.fury.io/py/powertools-oas-validator) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Installation\nPoetry:\n`poetry add powertools-oas-validator`\n\nPip:\n`pip install powertools-oas-validator`\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have a nice validation message, in case you rely on piping it straight back to the client.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/RasmusFangel/powertools-oas-validator',
```

### Comparing `powertools_oas_validator-0.5.2/PKG-INFO` & `powertools_oas_validator-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Home-page: https://github.com/RasmusFangel/powertools-oas-validator
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

