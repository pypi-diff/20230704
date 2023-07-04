# Comparing `tmp/scw_serverless-1.1.0.tar.gz` & `tmp/scw_serverless-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_serverless-1.1.0.tar", max compression
+gzip compressed data, was "scw_serverless-1.2.0.tar", max compression
```

## Comparing `scw_serverless-1.1.0.tar` & `scw_serverless-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1181 2023-05-11 13:07:19.008204 scw_serverless-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-05-11 13:07:19.008204 scw_serverless-1.1.0/LICENSE
--rw-r--r--   0        0        0     3154 2023-05-11 13:07:19.008204 scw_serverless-1.1.0/README.md
--rw-r--r--   0        0        0     3038 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/__init__.py
--rw-r--r--   0        0        0     5081 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/app.py
--rw-r--r--   0        0        0     4889 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/cli.py
--rw-r--r--   0        0        0       31 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/__init__.py
--rw-r--r--   0        0        0     3831 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/function.py
--rw-r--r--   0        0        0     1320 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/route.py
--rw-r--r--   0        0        0     1405 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/config/triggers.py
--rw-r--r--   0        0        0     3684 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/dependencies_manager.py
--rw-r--r--   0        0        0      261 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/__init__.py
--rw-r--r--   0        0        0     7144 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/api_wrapper.py
--rw-r--r--   0        0        0     1829 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/client.py
--rw-r--r--   0        0        0     8237 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/deployment_manager.py
--rw-r--r--   0        0        0      434 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/exceptions.py
--rw-r--r--   0        0        0      564 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/deployment/runtime.py
--rw-r--r--   0        0        0        0 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/gateway/__init__.py
--rw-r--r--   0        0        0     1359 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/gateway/gateway_api_client.py
--rw-r--r--   0        0        0     2341 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/gateway/gateway_manager.py
--rw-r--r--   0        0        0     1573 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/loader.py
--rw-r--r--   0        0        0     1384 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/local_app.py
--rw-r--r--   0        0        0      430 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/logger.py
--rw-r--r--   0        0        0        0 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/utils/__init__.py
--rw-r--r--   0        0        0      590 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/utils/files.py
--rw-r--r--   0        0        0      427 2023-05-11 13:07:19.012204 scw_serverless-1.1.0/scw_serverless/utils/string.py
--rw-r--r--   0        0        0     4466 1970-01-01 00:00:00.000000 scw_serverless-1.1.0/setup.py
--rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 scw_serverless-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1316 2023-07-03 15:04:31.979197 scw_serverless-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3154 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/README.md
+-rw-r--r--   0        0        0     3075 2023-07-03 15:04:31.979197 scw_serverless-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/scw_serverless/__init__.py
+-rw-r--r--   0        0        0     5081 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/scw_serverless/app.py
+-rw-r--r--   0        0        0     4173 2023-06-26 14:57:27.927026 scw_serverless-1.2.0/scw_serverless/cli.py
+-rw-r--r--   0        0        0       31 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/scw_serverless/config/__init__.py
+-rw-r--r--   0        0        0     3831 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/scw_serverless/config/function.py
+-rw-r--r--   0        0        0      931 2023-06-26 14:57:27.927026 scw_serverless-1.2.0/scw_serverless/config/route.py
+-rw-r--r--   0        0        0     1405 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/scw_serverless/config/triggers.py
+-rw-r--r--   0        0        0     3684 2023-06-22 16:54:07.920796 scw_serverless-1.2.0/scw_serverless/dependencies_manager.py
+-rw-r--r--   0        0        0      261 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/deployment/__init__.py
+-rw-r--r--   0        0        0     7144 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/deployment/api_wrapper.py
+-rw-r--r--   0        0        0     1829 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/deployment/client.py
+-rw-r--r--   0        0        0     8237 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/deployment/deployment_manager.py
+-rw-r--r--   0        0        0      434 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/deployment/exceptions.py
+-rw-r--r--   0        0        0      564 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/deployment/runtime.py
+-rw-r--r--   0        0        0      133 2023-06-26 14:57:27.927026 scw_serverless-1.2.0/scw_serverless/gateway/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-26 14:57:27.927026 scw_serverless-1.2.0/scw_serverless/gateway/gateway_manager.py
+-rw-r--r--   0        0        0     1447 2023-07-03 15:04:31.979197 scw_serverless-1.2.0/scw_serverless/gateway/serverless_gateway.py
+-rw-r--r--   0        0        0     1573 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/loader.py
+-rw-r--r--   0        0        0     1384 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/local_app.py
+-rw-r--r--   0        0        0      430 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/logger.py
+-rw-r--r--   0        0        0        0 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/utils/__init__.py
+-rw-r--r--   0        0        0      590 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/utils/files.py
+-rw-r--r--   0        0        0      427 2023-06-22 16:54:07.924796 scw_serverless-1.2.0/scw_serverless/utils/string.py
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 scw_serverless-1.2.0/setup.py
+-rw-r--r--   0        0        0     4611 1970-01-01 00:00:00.000000 scw_serverless-1.2.0/PKG-INFO
```

### Comparing `scw_serverless-1.1.0/CHANGELOG.md` & `scw_serverless-1.2.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,7 +34,13 @@
 ### Fixed
 
 - Setting `http_option=enabled` will now correctly apply HTTPs-only when deploying with the API
 
 ### Removed
 
 - Removed generating Terraform and Serverless Framework configuration files as those features were mostly unused. This does not break the `scw-serverless` library but it removes a command from the CLI. We think those changes will help improve the overall quality of the tool.
+
+## [1.2.0] - 2023-07-03
+
+### Feature
+
+- Changed the gateway integration to work with latest release of the Serverless Gateway project
```

### Comparing `scw_serverless-1.1.0/LICENSE` & `scw_serverless-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/README.md` & `scw_serverless-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/pyproject.toml` & `scw_serverless-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "scw-serverless"
-version = "1.1.0"
+version = "1.2.0"
 description = "Framework for writing serverless APIs in Python, using Scaleway functions and containers."
 authors = ["Scaleway Serverless Team <opensource@scaleway.com>"]
 readme = "README.md"
 license = "MIT"
-repository = "https://github.com/scaleway/serverless-api-framework-python-python"
+repository = "https://github.com/scaleway/serverless-api-framework-python"
 documentation = "https://serverless-api-project.readthedocs.io/en/latest/"
 keywords = ["serverless", "scaleway", "functions", "cloud", "faas"]
 
 # Should be one of:
 # "Development Status :: 3 - Alpha"
 # "Development Status :: 4 - Beta"
 # "Development Status :: 5 - Production/Stable"
@@ -17,41 +17,41 @@
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Internet",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 packages = [{ include = "scw_serverless" }]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.scripts]
 scw-serverless = "scw_serverless.cli:cli"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+# TODO: investigate this breaking change (can we lower the gateway Python version ?)
+python = ">=3.10,<3.12"
 click = "^8.1.3"
-scaleway = ">=0.7,<0.13"
+scaleway = ">=0.7,<0.15"
 scaleway-functions-python = "^0.2.0"
 requests = "^2.28.2"
 typing-extensions = { version = "^4.4.0", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.21,<4.0"
 pytest = "^7.2.0"
 pytest-xdist = "^3.1.0"
 pylint = "^2.15.10"
 pylint-per-file-ignores = "^1.1.0"
 responses = ">=0.22,<0.24"
-boto3 = "^1.26.130"
+scw-gateway = "^0.4.0"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 myst_parser = "^1.0.0"
 sphinx = "^6.1.0"
```

### Comparing `scw_serverless-1.1.0/scw_serverless/app.py` & `scw_serverless-1.2.0/scw_serverless/app.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/cli.py` & `scw_serverless-1.2.0/scw_serverless/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import click
 from scaleway import ScalewayException
 
 import scw_serverless
 from scw_serverless import app, deployment, loader, local_app, logger
 from scw_serverless.dependencies_manager import DependenciesManager
-from scw_serverless.gateway.gateway_manager import GatewayManager
+from scw_serverless.gateway import GatewayManager, ServerlessGateway
 
 CLICK_ARG_FILE = click.argument(
     "file",
     required=True,
     type=click.Path(
         exists=True,
         file_okay=True,
@@ -40,24 +40,14 @@
     """
     logger.configure_logger(verbose, log_level=getattr(logging, log_level))
 
 
 @cli.command()
 @CLICK_ARG_FILE
 @click.option(
-    "--gateway-url",
-    default=None,
-    help="URL of a deployed API Gateway.",
-)
-@click.option(
-    "--gateway-api-key",
-    default=None,
-    help="API key used to manage the routes of the API Gateway.",
-)
-@click.option(
     "--runtime",
     default=None,
     help="Python runtime to deploy with. Uses your Python version by default.",
 )
 @click.option(
     "--single-source",
     is_flag=True,
@@ -80,16 +70,14 @@
     "--region",
     default=None,
     help="Region to deploy to.",
 )
 # pylint: disable=too-many-arguments
 def deploy(
     file: Path,
-    gateway_url: Optional[str],
-    gateway_api_key: Optional[str],
     runtime: Optional[str],
     single_source: bool,
     profile: Optional[str] = None,
     secret_key: Optional[str] = None,
     project_id: Optional[str] = None,
     region: Optional[str] = None,
 ) -> None:
@@ -101,26 +89,18 @@
     be pulled from your Scaleway configuration.
     """
     # Get the serverless App instance
     app_instance = loader.load_app_instance(file.resolve())
 
     # Check if the application requires a Gateway
     needs_gateway = any(function.gateway_route for function in app_instance.functions)
-    if needs_gateway and not gateway_url:
-        logging.debug("Prompting for Serverless Gateway URL...")
-        gateway_url = click.prompt(
-            "Please enter the URL of your Serverless Gateway", type=str
-        )
-    if needs_gateway and not gateway_api_key:
-        logging.debug("Prompting for Serverless Gateway API key...")
-        gateway_url = click.prompt(
-            "Please enter the API key to your Serverless Gateway",
-            hide_input=True,
-            type=str,
-        )
+    gateway = None
+    if needs_gateway:
+        logging.debug("Checking for Gateway CLI")
+        gateway = ServerlessGateway()
 
     client = deployment.get_scw_client(profile, secret_key, project_id, region)
 
     if not runtime:
         runtime = deployment.get_current_runtime()
 
     logging.info("Packaging dependencies...")
@@ -135,18 +115,19 @@
             single_source=single_source,
         ).deploy()
     except ScalewayException as e:
         logging.debug(e, exc_info=True)
         deployment.log_scaleway_exception(e)
 
     if needs_gateway:
+        assert gateway
+
         manager = GatewayManager(
             app_instance=app_instance,
-            gateway_url=cast(str, gateway_url),
-            gateway_api_key=cast(str, gateway_api_key),
+            gateway=gateway,
             sdk_client=client,
         )
         manager.update_routes()
 
 
 @cli.command()
 @CLICK_ARG_FILE
```

### Comparing `scw_serverless-1.1.0/scw_serverless/config/function.py` & `scw_serverless-1.2.0/scw_serverless/config/function.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/config/route.py` & `scw_serverless-1.2.0/scw_serverless/config/route.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Optional
+from typing import Optional
 
 
 class HTTPMethod(Enum):
     """Enum of supported HTTP methods.
 
     .. seealso:: https://docs.python.org/3/library/http.html#http.HTTPMethod
     """
@@ -29,16 +29,7 @@
         if not self.relative_url:
             raise RuntimeError("Route relative_url must be defined")
         if not self.target:
             raise RuntimeError("Route target must be defined")
         for method in self.http_methods or []:
             if method not in HTTPMethod:
                 raise RuntimeError(f"Route contains invalid method {method.value}")
-
-    def asdict(self) -> dict[str, Any]:
-        """Return a dict representation of a route."""
-        serialized: dict[str, Any] = {"relative_url": self.relative_url}
-        if self.http_methods:
-            serialized["http_methods"] = [method.value for method in self.http_methods]
-        if self.target:
-            serialized["target"] = self.target
-        return serialized
```

### Comparing `scw_serverless-1.1.0/scw_serverless/config/triggers.py` & `scw_serverless-1.2.0/scw_serverless/config/triggers.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/dependencies_manager.py` & `scw_serverless-1.2.0/scw_serverless/dependencies_manager.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/deployment/api_wrapper.py` & `scw_serverless-1.2.0/scw_serverless/deployment/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/deployment/client.py` & `scw_serverless-1.2.0/scw_serverless/deployment/client.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/deployment/deployment_manager.py` & `scw_serverless-1.2.0/scw_serverless/deployment/deployment_manager.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/deployment/runtime.py` & `scw_serverless-1.2.0/scw_serverless/deployment/runtime.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/gateway/gateway_manager.py` & `scw_serverless-1.2.0/scw_serverless/gateway/gateway_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+from typing import Protocol
+
 import scaleway.function.v1beta1 as sdk
 from scaleway import Client
 
 from scw_serverless.app import Serverless
-from scw_serverless.gateway.gateway_api_client import GatewayAPIClient
+from scw_serverless.config.route import GatewayRoute
+
+
+class Gateway(Protocol):
+    """Generic Gateway Implementation."""
+
+    def add_route(self, route: GatewayRoute) -> None:
+        """Add a route to the Gateway."""
 
 
 class GatewayManager:
     """Apply the configured routes to an existing API Gateway."""
 
     def __init__(
         self,
         app_instance: Serverless,
-        gateway_url: str,
-        gateway_api_key: str,
+        gateway: Gateway,
         sdk_client: Client,
     ):
         self.app_instance = app_instance
         self.api = sdk.FunctionV1Beta1API(sdk_client)
-        self.gateway_client = GatewayAPIClient(
-            gateway_url=gateway_url, gateway_api_key=gateway_api_key
-        )
+        self.gateway = gateway
 
     def _list_created_functions(self) -> dict[str, sdk.Function]:
         """Get the list of created functions."""
         namespace_name = self.app_instance.service_name
         namespaces = self.api.list_namespaces_all(name=namespace_name)
         if not namespaces:
             raise RuntimeError(
@@ -57,8 +63,8 @@
                     + "because it was not deployed"
                 )
 
             target = "https://" + created_functions[function.name].domain_name
             function.gateway_route.target = target  # type: ignore
 
         for function in routed_functions:
-            self.gateway_client.create_route(function.gateway_route)  # type: ignore
+            self.gateway.add_route(function.gateway_route)  # type: ignore
```

### Comparing `scw_serverless-1.1.0/scw_serverless/loader.py` & `scw_serverless-1.2.0/scw_serverless/loader.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/local_app.py` & `scw_serverless-1.2.0/scw_serverless/local_app.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/scw_serverless/utils/files.py` & `scw_serverless-1.2.0/scw_serverless/utils/files.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.1.0/setup.py` & `scw_serverless-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'requests>=2.28.2,<3.0.0',
  'scaleway-functions-python>=0.2.0,<0.3.0',
- 'scaleway>=0.7,<0.13']
+ 'scaleway>=0.7,<0.15']
 
 extras_require = \
 {':python_version < "3.11"': ['typing-extensions>=4.4.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['scw-serverless = scw_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'scw-serverless',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': 'Framework for writing serverless APIs in Python, using Scaleway functions and containers.',
     'long_description': '# Serverless API Framework\n\n[![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)\n[![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-framework-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-framework-python/main)\n\nServerless API Framework is a tool that lets you write and deploy serverless functions in Python.\nIt bridges your code with the deployment configuration to make it a breeze to work with serverless functions.\n\nStarts by defining a simple Python function:\n\n```python\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\n\n@app.func(memory_limit=256)\ndef hello_world(event, context):\n    return "Hello World!"\n```\n\nDeploy it with `scw-serverless`:\n\n```console\nscw-serverless deploy app.py\n```\n\n## Quickstart\n\n### Install\n\n```console\npip install scw-serverless\n```\n\nThis will install the `scw-serverless` CLI:\n\n```console\nscw-serverless --help\n```\n\n### Writing and configuring functions\n\nYou can transform your Python functions into serverless functions by using decorators:\n\n```python\nimport os\nimport requests\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\nAPI_URL = os.environ["API_URL"]\n\n@app.func(memory_limit=256, env={"API_URL": API_URL})\ndef hello_world(event, context):\n    return requests.get(API_URL)\n```\n\nThe configuration is done by passing arguments to the decorator.\nTo view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.\n\n### Local testing\n\nBefore deploying, you can run your functions locally with the dev command:\n\n```console\nscw-serverless dev app.py\n```\n\nThis runs a local Flask server with your Serverless handlers. If no `relative_url` is defined for a function, it will be served on `/name` with `name` being the name of your Python function.\n\nBy default, this runs Flask in debug mode which includes hot-reloading. You can disable this behavior by passing the `--no-debug` flag.\n\n### Deploying\n\nWhen you are ready, you can deploy your function with the `scw-serverless` CLI tool:\n\n```console\nscw-serverless deploy app.py\n```\n\nThe tool will use your Scaleway credentials from your environment and config file.\n\n## What’s Next?\n\nTo learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).\nIf you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-framework-python-python/tree/main/examples) to get you started.\n\nTo run your Python functions locally, check out [Scaleway Functions Python](https://github.com/scaleway/serverless-functions-python).\n\n## Contributing\n\nWe welcome all contributions.\n\nThis project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.\n\n```console\npre-commit install\n```\n',
     'author': 'Scaleway Serverless Team',
     'author_email': 'opensource@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/scaleway/serverless-api-framework-python-python',
+    'url': 'https://github.com/scaleway/serverless-api-framework-python',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.12',
+    'python_requires': '>=3.10,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `scw_serverless-1.1.0/PKG-INFO` & `scw_serverless-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: scw-serverless
-Version: 1.1.0
+Version: 1.2.0
 Summary: Framework for writing serverless APIs in Python, using Scaleway functions and containers.
-Home-page: https://github.com/scaleway/serverless-api-framework-python-python
+Home-page: https://github.com/scaleway/serverless-api-framework-python
 License: MIT
 Keywords: serverless,scaleway,functions,cloud,faas
 Author: Scaleway Serverless Team
 Author-email: opensource@scaleway.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: scaleway (>=0.7,<0.13)
+Requires-Dist: scaleway (>=0.7,<0.15)
 Requires-Dist: scaleway-functions-python (>=0.2.0,<0.3.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Documentation, https://serverless-api-project.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/scaleway/serverless-api-framework-python-python
+Project-URL: Repository, https://github.com/scaleway/serverless-api-framework-python
 Description-Content-Type: text/markdown
 
 # Serverless API Framework
 
 [![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)
 [![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-framework-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-framework-python/main)
```

