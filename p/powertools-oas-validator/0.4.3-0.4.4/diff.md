# Comparing `tmp/powertools_oas_validator-0.4.3.tar.gz` & `tmp/powertools_oas_validator-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.4.3.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.4.4.tar", max compression
```

## Comparing `powertools_oas_validator-0.4.3.tar` & `powertools_oas_validator-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-07-03 16:00:19.793080 powertools_oas_validator-0.4.3/LICENSE
--rw-r--r--   0        0        0     2215 2023-07-03 16:00:19.793080 powertools_oas_validator-0.4.3/README.md
--rw-r--r--   0        0        0       13 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      199 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0      944 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     3196 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     3321 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1805 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      756 2023-07-03 16:00:19.797080 powertools_oas_validator-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.3/setup.py
--rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2218 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/README.md
+-rw-r--r--   0        0        0       13 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1571 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     3196 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     3321 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1805 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      756 2023-07-03 20:54:26.300407 powertools_oas_validator-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.4/setup.py
+-rw-r--r--   0        0        0     2833 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.4/PKG-INFO
```

### Comparing `powertools_oas_validator-0.4.3/LICENSE` & `powertools_oas_validator-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.3/README.md` & `powertools_oas_validator-0.4.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 Decorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.
 
 
 ### Minimal Example
 
 ```python
 from typing import Dict
-from aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse
+from aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response
 from aws_lambda_powertools.utilities.typing import LambdaContext
-from aws_lambda_powertools.middleware import validate_request
+from powertools_oas_validator.middleware import validate_request
 
 
 app = APIGatewayRestResolver()
 
 @app.post("/example")
 def example() -> Response:
   ...
```

### Comparing `powertools_oas_validator-0.4.3/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.4.4/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.3/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.4.4/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.3/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.4.4/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.3/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.4.4/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.3/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.4.4/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.3/powertools_oas_validator/types.py` & `powertools_oas_validator-0.4.4/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.3/pyproject.toml` & `powertools_oas_validator-0.4.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "powertools_oas_validator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `powertools_oas_validator-0.4.3/setup.py` & `powertools_oas_validator-0.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': '',
-    'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://badge.fury.io/py/powertools-oas-validator) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom aws_lambda_powertools.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have a nice validation message, in case you rely on piping it straight back to the client.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
+    'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://badge.fury.io/py/powertools-oas-validator) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have a nice validation message, in case you rely on piping it straight back to the client.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `powertools_oas_validator-0.4.3/PKG-INFO` & `powertools_oas_validator-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,17 +30,17 @@
 Decorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.
 
 
 ### Minimal Example
 
 ```python
 from typing import Dict
-from aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse
+from aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response
 from aws_lambda_powertools.utilities.typing import LambdaContext
-from aws_lambda_powertools.middleware import validate_request
+from powertools_oas_validator.middleware import validate_request
 
 
 app = APIGatewayRestResolver()
 
 @app.post("/example")
 def example() -> Response:
   ...
```

