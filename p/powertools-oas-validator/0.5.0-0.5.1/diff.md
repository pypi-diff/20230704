# Comparing `tmp/powertools_oas_validator-0.5.0.tar.gz` & `tmp/powertools_oas_validator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.5.0.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.5.1.tar", max compression
```

## Comparing `powertools_oas_validator-0.5.0.tar` & `powertools_oas_validator-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-07-04 12:07:20.368748 powertools_oas_validator-0.5.0/LICENSE
--rw-r--r--   0        0        0     2218 2023-07-04 12:07:20.368748 powertools_oas_validator-0.5.0/README.md
--rw-r--r--   0        0        0       13 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      199 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0     1031 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     4508 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/services/error_handler.py
--rw-r--r--   0        0        0     3196 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     2166 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1805 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      756 2023-07-04 12:07:20.372748 powertools_oas_validator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3083 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.0/setup.py
--rw-r--r--   0        0        0     2833 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-04 12:16:00.592444 powertools_oas_validator-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2218 2023-07-04 12:16:00.592444 powertools_oas_validator-0.5.1/README.md
+-rw-r--r--   0        0        0       13 2023-07-04 12:16:00.592444 powertools_oas_validator-0.5.1/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-04 12:16:00.592444 powertools_oas_validator-0.5.1/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-04 12:16:00.596444 powertools_oas_validator-0.5.1/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-04 12:16:00.596444 powertools_oas_validator-0.5.1/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-04 12:16:00.596444 powertools_oas_validator-0.5.1/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0     1031 2023-07-04 12:16:00.596444 powertools_oas_validator-0.5.1/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     4508 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/powertools_oas_validator/services/error_handler.py
+-rw-r--r--   0        0        0     3196 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     2166 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1805 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      975 2023-07-04 12:16:00.600444 powertools_oas_validator-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.1/setup.py
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 powertools_oas_validator-0.5.1/PKG-INFO
```

### Comparing `powertools_oas_validator-0.5.0/LICENSE` & `powertools_oas_validator-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/README.md` & `powertools_oas_validator-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/overrides/validators.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/services/error_handler.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/services/error_handler.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/powertools_oas_validator/types.py` & `powertools_oas_validator-0.5.1/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.5.0/pyproject.toml` & `powertools_oas_validator-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
+
+homepage = "https://github.com/RasmusFangel/powertools-oas-validator"
+repository = "https://github.com/RasmusFangel/powertools-oas-validator"
+documentation = "https://github.com/RasmusFangel/powertools-oas-validator"
+
 packages = [{include = "powertools_oas_validator"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aws-lambda-powertools = "^2.18.0"
 jmespath = "^1.0.1"
 fastjsonschema = "^2.17.1"
```

### Comparing `powertools_oas_validator-0.5.0/setup.py` & `powertools_oas_validator-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': '',
     'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://badge.fury.io/py/powertools-oas-validator) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolver, Response\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom powertools_oas_validator.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have a nice validation message, in case you rely on piping it straight back to the client.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/RasmusFangel/powertools-oas-validator',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `powertools_oas_validator-0.5.0/PKG-INFO` & `powertools_oas_validator-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
+Home-page: https://github.com/RasmusFangel/powertools-oas-validator
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-lambda-powertools (>=2.18.0,<3.0.0)
 Requires-Dist: fastjsonschema (>=2.17.1,<3.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: openapi-core (>=0.17.2,<0.18.0)
+Project-URL: Documentation, https://github.com/RasmusFangel/powertools-oas-validator
+Project-URL: Repository, https://github.com/RasmusFangel/powertools-oas-validator
 Description-Content-Type: text/markdown
 
 # powertools-oas-validator
 <br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://badge.fury.io/py/powertools-oas-validator) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)
 
 ## Introduction
```

