# Comparing `tmp/openapi_python_generator-0.4.7.dev1688499481.tar.gz` & `tmp/openapi_python_generator-0.4.8.dev1688499555.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_python_generator-0.4.7.dev1688499481.tar", max compression
+gzip compressed data, was "openapi_python_generator-0.4.8.dev1688499555.tar", max compression
```

## Comparing `openapi_python_generator-0.4.7.dev1688499481.tar` & `openapi_python_generator-0.4.8.dev1688499555.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-07-04 19:37:49.983162 openapi_python_generator-0.4.7.dev1688499481/LICENSE
--rw-r--r--   0        0        0     4118 2023-07-04 19:37:49.983162 openapi_python_generator-0.4.7.dev1688499481/README.md
--rw-r--r--   0        0        0     2171 2023-07-04 19:38:02.075343 openapi_python_generator-0.4.7.dev1688499481/pyproject.toml
--rw-r--r--   0        0        0      476 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/__init__.py
--rw-r--r--   0        0        0     1622 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/__main__.py
--rw-r--r--   0        0        0      959 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/common.py
--rw-r--r--   0        0        0     4970 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/generate_data.py
--rw-r--r--   0        0        0        0 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/__init__.py
--rw-r--r--   0        0        0      740 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/api_config_generator.py
--rw-r--r--   0        0        0      922 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/common.py
--rw-r--r--   0        0        0     1296 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/generator.py
--rw-r--r--   0        0        0      426 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/jinja_config.py
--rw-r--r--   0        0        0    12151 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/model_generator.py
--rw-r--r--   0        0        0    13135 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/service_generator.py
--rw-r--r--   0        0        0     1977 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2
--rw-r--r--   0        0        0     1256 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2
--rw-r--r--   0        0        0      242 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/enum.jinja2
--rw-r--r--   0        0        0     2131 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2
--rw-r--r--   0        0        0      671 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/models.jinja2
--rw-r--r--   0        0        0     1874 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/requests.jinja2
--rw-r--r--   0        0        0      202 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/service.jinja2
--rw-r--r--   0        0        0     1726 2023-07-04 19:37:49.987162 openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/models.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.7.dev1688499481/setup.py
--rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.7.dev1688499481/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-04 19:38:59.000618 openapi_python_generator-0.4.8.dev1688499555/LICENSE
+-rw-r--r--   0        0        0     4118 2023-07-04 19:38:59.000618 openapi_python_generator-0.4.8.dev1688499555/README.md
+-rw-r--r--   0        0        0     2171 2023-07-04 19:39:16.612638 openapi_python_generator-0.4.8.dev1688499555/pyproject.toml
+-rw-r--r--   0        0        0      476 2023-07-04 19:38:59.004618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/__init__.py
+-rw-r--r--   0        0        0     1622 2023-07-04 19:38:59.004618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/__main__.py
+-rw-r--r--   0        0        0      959 2023-07-04 19:38:59.004618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/common.py
+-rw-r--r--   0        0        0     4970 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/generate_data.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/api_config_generator.py
+-rw-r--r--   0        0        0      922 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/common.py
+-rw-r--r--   0        0        0     1296 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/generator.py
+-rw-r--r--   0        0        0      426 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/jinja_config.py
+-rw-r--r--   0        0        0    12151 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/model_generator.py
+-rw-r--r--   0        0        0    13135 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/service_generator.py
+-rw-r--r--   0        0        0     1977 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2
+-rw-r--r--   0        0        0     1256 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2
+-rw-r--r--   0        0        0      242 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/enum.jinja2
+-rw-r--r--   0        0        0     2131 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2
+-rw-r--r--   0        0        0      671 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/models.jinja2
+-rw-r--r--   0        0        0     1874 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/requests.jinja2
+-rw-r--r--   0        0        0      202 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/service.jinja2
+-rw-r--r--   0        0        0     1726 2023-07-04 19:38:59.008618 openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/models.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.8.dev1688499555/setup.py
+-rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 openapi_python_generator-0.4.8.dev1688499555/PKG-INFO
```

### Comparing `openapi_python_generator-0.4.7.dev1688499481/LICENSE` & `openapi_python_generator-0.4.8.dev1688499555/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/README.md` & `openapi_python_generator-0.4.8.dev1688499555/README.md`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/pyproject.toml` & `openapi_python_generator-0.4.8.dev1688499555/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-python-generator"
-version = "0.4.7.dev.1688499481"
+version = "0.4.8.dev.1688499555"
 description = "Openapi Python Generator"
 authors = ["Marco Müllner <muellnermarco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MarcoMuellner/openapi-python-generator"
 repository = "https://github.com/MarcoMuellner/openapi-python-generator"
 documentation = "https://openapi-python-generator.readthedocs.io"
```

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/__main__.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/common.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/common.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/generate_data.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/generate_data.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/api_config_generator.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/api_config_generator.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/common.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/common.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/generator.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/generator.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/model_generator.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/model_generator.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/service_generator.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/service_generator.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/aiohttp.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/apiconfig.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/httpx.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/models.jinja2` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/models.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/language_converters/python/templates/requests.jinja2` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/language_converters/python/templates/requests.jinja2`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/src/openapi_python_generator/models.py` & `openapi_python_generator-0.4.8.dev1688499555/src/openapi_python_generator/models.py`

 * *Files identical despite different names*

### Comparing `openapi_python_generator-0.4.7.dev1688499481/setup.py` & `openapi_python_generator-0.4.8.dev1688499555/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 entry_points = \
 {'console_scripts': ['openapi-python-generator = '
                      'openapi_python_generator.__main__:main']}
 
 setup_kwargs = {
     'name': 'openapi-python-generator',
-    'version': '0.4.7.dev1688499481',
+    'version': '0.4.8.dev1688499555',
     'description': 'Openapi Python Generator',
     'long_description': "# Openapi Python Generator\n\n[![PyPI](https://img.shields.io/pypi/v/openapi-python-generator.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/openapi-python-generator.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/openapi-python-generator)][python version]\n[![License](https://img.shields.io/pypi/l/openapi-python-generator)][license]\n\n[![](https://img.shields.io/static/v1?label=documentation&message=enabled&color=<COLOR>)][documentation]\n[![Tests](https://github.com/MarcoMuellner/openapi-python-generator/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/MarcoMuellner/openapi-python-generator/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/openapi-python-generator/\n[status]: https://pypi.org/project/openapi-python-generator/\n[python version]: https://pypi.org/project/openapi-python-generator\n[documentation]: https://marcomuellner.github.io/openapi-python-generator/\n[tests]: https://github.com/MarcoMuellner/openapi-python-generator/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/MarcoMuellner/openapi-python-generator\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n![](logo.png)\n\n---\n__Documentation:__ [here][documentation]\n\n---\n\n## Features\n\n- __Ease of use__. Provide input, output and the library, and the generator will do the rest.\n- __Type safety and type hinting.__ __OpenAPI python generator__ makes heavy use of pydantic models to provide type-safe data structures.\n- __Support for multiple rest frameworks.__ __OpenAPI python generator__ currently supports the following:\n    - [httpx](https://pypi.org/project/httpx/)\n    - [requests](https://pypi.org/project/requests/)\n    - [aiohttp](https://pypi.org/project/aiohttp/)\n- __Async and sync code generation support__, depending on the framework. It will automatically create both for frameworks that support both.\n- __Easily extendable using Jinja2 templates__. The code is designed to be easily extendable and should support even more languages and frameworks in the future.\n- __Fully tested__. Every generated code is automatically tested against the OpenAPI spec and we have 100% coverage.\n- __Usage as CLI or as library__.\n\n## Requirements\n\n- Python 3.7+\n\n## Installation\n\nYou can install _Openapi Python Generator_ via [pip] from [PyPI]:\n\n```console\n$ pip install openapi-python-generator\n```\n\n## Usage\n\nPlease see the [Quick start page] for details.\n\n## Roadmap\n\n- Support for all commonly used http libraries in the python ecosystem (~~requests~~, urllib, ...)\n- Support for multiple languages\n- Support for multiple authentication schemes\n- Support custom themes\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Openapi Python Generator_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nSpecial thanks to the peeps from [openapi-schema-pydantic](https://github.com/kuimono/openapi-schema-pydantic),\nwhich already did a lot of the legwork by providing a pydantic schema for the OpenAPI 3.0.0+ specification.\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/MarcoMuellner/openapi-python-generator/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/MarcoMuellner/openapi-python-generator/blob/main/LICENSE\n[contributor guide]: https://github.com/MarcoMuellner/openapi-python-generator/blob/main/CONTRIBUTING.md\n[Quick start page]: https://marcomuellner.github.io/openapi-python-generator/quick_start/\n",
     'author': 'Marco Müllner',
     'author_email': 'muellnermarco@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MarcoMuellner/openapi-python-generator',
```

### Comparing `openapi_python_generator-0.4.7.dev1688499481/PKG-INFO` & `openapi_python_generator-0.4.8.dev1688499555/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-python-generator
-Version: 0.4.7.dev1688499481
+Version: 0.4.8.dev1688499555
 Summary: Openapi Python Generator
 Home-page: https://github.com/MarcoMuellner/openapi-python-generator
 License: MIT
 Keywords: OpenAPI,Generator,Python,async
 Author: Marco Müllner
 Author-email: muellnermarco@gmail.com
 Requires-Python: >=3.7,<4.0
```

