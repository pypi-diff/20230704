# Comparing `tmp/fal_serverless-0.6.35.tar.gz` & `tmp/fal_serverless-0.6.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_serverless-0.6.35.tar", max compression
+gzip compressed data, was "fal_serverless-0.6.36.tar", max compression
```

## Comparing `fal_serverless-0.6.35.tar` & `fal_serverless-0.6.36.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      213 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/README.md
--rw-r--r--   0        0        0     1013 2023-06-20 00:21:51.807364 fal_serverless-0.6.35/pyproject.toml
--rw-r--r--   0        0        0      335 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/__init__.py
--rw-r--r--   0        0        0    17568 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/api.py
--rw-r--r--   0        0        0     2593 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/auth/__init__.py
--rw-r--r--   0        0        0     5426 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/auth/auth0.py
--rw-r--r--   0        0        0     1786 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/auth/local.py
--rw-r--r--   0        0        0    15650 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/cli.py
--rw-r--r--   0        0        0      132 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/console/__init__.py
--rw-r--r--   0        0        0      108 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/console/icons.py
--rw-r--r--   0        0        0      485 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/console/ux.py
--rw-r--r--   0        0        0      172 2023-06-20 00:21:44.471356 fal_serverless-0.6.35/src/fal_serverless/env.py
--rw-r--r--   0        0        0      938 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/__init__.py
--rw-r--r--   0        0        0      412 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/_base.py
--rw-r--r--   0        0        0      353 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/auth.py
--rw-r--r--   0        0        0     1435 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/exceptions/handlers.py
--rw-r--r--   0        0        0      326 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/flags.py
--rw-r--r--   0        0        0     1649 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/__init__.py
--rw-r--r--   0        0        0     2574 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/datadog.py
--rw-r--r--   0        0        0     2122 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/isolate.py
--rw-r--r--   0        0        0      386 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/style.py
--rw-r--r--   0        0        0     1785 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/trace.py
--rw-r--r--   0        0        0      643 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/logging/user.py
--rw-r--r--   0        0        0    16374 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/sdk.py
--rw-r--r--   0        0        0     6533 2023-06-20 00:21:31.515343 fal_serverless-0.6.35/src/fal_serverless/sync.py
--rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 fal_serverless-0.6.35/setup.py
--rw-r--r--   0        0        0     1613 1970-01-01 00:00:00.000000 fal_serverless-0.6.35/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/README.md
+-rw-r--r--   0        0        0     1012 2023-07-03 23:01:04.624228 fal_serverless-0.6.36/pyproject.toml
+-rw-r--r--   0        0        0      405 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/__init__.py
+-rw-r--r--   0        0        0    23138 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/api.py
+-rw-r--r--   0        0        0     2593 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/auth/__init__.py
+-rw-r--r--   0        0        0     5426 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/auth/auth0.py
+-rw-r--r--   0        0        0     1786 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/auth/local.py
+-rw-r--r--   0        0        0    15556 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/cli.py
+-rw-r--r--   0        0        0      132 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/console/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/console/icons.py
+-rw-r--r--   0        0        0      485 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/console/ux.py
+-rw-r--r--   0        0        0     5387 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/decorators.py
+-rw-r--r--   0        0        0      158 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/env.py
+-rw-r--r--   0        0        0      938 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/_base.py
+-rw-r--r--   0        0        0      353 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/auth.py
+-rw-r--r--   0        0        0     1435 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/exceptions/handlers.py
+-rw-r--r--   0        0        0      578 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/flags.py
+-rw-r--r--   0        0        0     1649 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/__init__.py
+-rw-r--r--   0        0        0     2574 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/datadog.py
+-rw-r--r--   0        0        0     2122 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/isolate.py
+-rw-r--r--   0        0        0      386 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/style.py
+-rw-r--r--   0        0        0     1785 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/trace.py
+-rw-r--r--   0        0        0      643 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/logging/user.py
+-rw-r--r--   0        0        0    17370 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/sdk.py
+-rw-r--r--   0        0        0     4231 2023-07-03 22:59:24.792768 fal_serverless-0.6.36/src/fal_serverless/sync.py
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 fal_serverless-0.6.36/setup.py
+-rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 fal_serverless-0.6.36/PKG-INFO
```

### Comparing `fal_serverless-0.6.35/pyproject.toml` & `fal_serverless-0.6.36/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "fal_serverless"
-version = "0.6.35"
+version = "0.6.36"
 description = "fal Serverless is an easy-to-use Serverless Python Framework"
 authors = ["Features & Labels <hello@fal.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 auth0-python = "^4.1.0"
 requests = "^2.28.1"
 isolate = {version = ">=0.12.2, <1.0", extras = ["build"]}
 grpcio = "^1.50.0"
 dill = ">=0.3.6,<0.3.7"
-isolate-proto = "^0.0.31"
+isolate-proto = "0.0.32"
 typing-extensions = "4.4"
 click = "^8.1.3"
 structlog = "^22.3.0"
 datadog-api-client = "2.12.0"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 grpc-interceptor = "^0.15.0"
```

### Comparing `fal_serverless-0.6.35/src/fal_serverless/auth/__init__.py` & `fal_serverless-0.6.36/src/fal_serverless/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/auth/auth0.py` & `fal_serverless-0.6.36/src/fal_serverless/auth/auth0.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/auth/local.py` & `fal_serverless-0.6.36/src/fal_serverless/auth/local.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/cli.py` & `fal_serverless-0.6.36/src/fal_serverless/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,26 +254,25 @@
 
 
 @function_cli.command("serve")
 @click.option("--alias", default=None)
 @click.option(
     "--auth",
     "auth_mode",
-    # TODO: handle shared auth mode
-    type=click.Choice(["public", "private"]),
+    type=click.Choice(["public", "private", "shared"]),
     default="private",
 )
 @click.argument("file_path", required=True)
 @click.argument("function_name", required=True)
 @click.pass_obj
 def register_application(
     host: api.FalServerlessHost,
     file_path: str,
     function_name: str,
-    auth_mode: Literal["public", "private"],
+    auth_mode: Literal["public", "private", "shared"],
     alias: str | None = None,
 ):
     import runpy
 
     module = runpy.run_path(file_path)
     isolated_function = module[function_name]
     gateway_options = isolated_function.options.gateway
@@ -289,15 +288,15 @@
             "Must expose port 8080 for now. This will be configurable in the future."
         )
 
     id = host.register(
         func=isolated_function.func,
         options=isolated_function.options,
         application_name=alias,
-        application_is_public=auth_mode == "public",
+        application_auth_mode=auth_mode,
     )
     if id:
         # TODO: should we centralize this URL format?
         gateway_host = host.url.replace("api.", "gateway.")
         gateway_host = remove_http_and_port_from_url(gateway_host)
 
         # Encode since user_id can contain special characters
@@ -365,19 +364,15 @@
     with client.connect() as connection:
         table = Table(title="Function Aliases")
         table.add_column("Alias")
         table.add_column("Revision")
         table.add_column("Auth")
 
         for app_alias in connection.list_aliases():
-            table.add_row(
-                app_alias.alias,
-                app_alias.revision,
-                "public" if app_alias.public else "private",
-            )
+            table.add_row(app_alias.alias, app_alias.revision, app_alias.auth_mode)
 
     console.print(table)
 
 
 ##### Crons group #####
 @click.group
 @click.option("--host", default=DEFAULT_HOST, envvar=HOST_ENVVAR)
@@ -484,15 +479,15 @@
         connection.delete_secret(secret_name)
         console.print(f"Secret '{secret_name}' has deleted")
 
 
 cli.add_command(auth_cli, name="auth")
 cli.add_command(key_cli, name="key", aliases=["keys"])
 cli.add_command(function_cli, name="function", aliases=["fn"])
-cli.add_command(alias_cli, name="alias")
+cli.add_command(alias_cli, name="alias", aliases=["aliases"])
 cli.add_command(crons_cli, name="cron", aliases=["crons"])
 cli.add_command(usage_cli, name="usage")
 cli.add_command(secrets_cli, name="secret", aliases=["secrets"])
 
 
 def remove_http_and_port_from_url(url):
     # Remove http://
```

### Comparing `fal_serverless-0.6.35/src/fal_serverless/exceptions/__init__.py` & `fal_serverless-0.6.36/src/fal_serverless/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/exceptions/handlers.py` & `fal_serverless-0.6.36/src/fal_serverless/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/logging/__init__.py` & `fal_serverless-0.6.36/src/fal_serverless/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/logging/datadog.py` & `fal_serverless-0.6.36/src/fal_serverless/logging/datadog.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/logging/isolate.py` & `fal_serverless-0.6.36/src/fal_serverless/logging/isolate.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/logging/trace.py` & `fal_serverless-0.6.36/src/fal_serverless/logging/trace.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/logging/user.py` & `fal_serverless-0.6.36/src/fal_serverless/logging/user.py`

 * *Files identical despite different names*

### Comparing `fal_serverless-0.6.35/src/fal_serverless/sdk.py` & `fal_serverless-0.6.36/src/fal_serverless/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import os
 from contextlib import ExitStack
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from enum import Enum
-from typing import Any, Callable, Generic, Iterator, TypeVar
+from typing import Any, Callable, Generic, Iterator, Literal, TypeVar
 
 import grpc
 import isolate_proto
 from fal_serverless import flags
 from fal_serverless.auth import USER
 from fal_serverless.logging.trace import TraceContextInterceptor
 from isolate.connections.common import is_agent
@@ -69,46 +69,56 @@
 class Credentials:
     # Cannot use `field` because child classes don't have default for all properties.
     server_credentials: ServerCredentials = get_default_server_credentials()
 
     def to_grpc(self) -> grpc.ChannelCredentials:
         return self.server_credentials.to_grpc()
 
+    def to_headers(self) -> dict[str, str]:
+        raise NotImplementedError
+
 
 @dataclass
 class FalServerlessKeyCredentials(Credentials):
     key_id: str
     key_secret: str
 
     def to_grpc(self) -> grpc.ChannelCredentials:
         return grpc.composite_channel_credentials(
             self.server_credentials.to_grpc(),
             grpc.metadata_call_credentials(_GRPCMetadata("auth-key", self.key_secret)),
             grpc.metadata_call_credentials(_GRPCMetadata("auth-key-id", self.key_id)),
         )
 
+    def to_headers(self) -> dict[str, str]:
+        return {"X-Fal-Key-Id": self.key_id, "X-Fal-Key-Secret": self.key_secret}
+
 
 @dataclass
 class AuthenticatedCredentials(Credentials):
     user = USER
 
     def to_grpc(self) -> grpc.ChannelCredentials:
         return grpc.composite_channel_credentials(
             self.server_credentials.to_grpc(),
             grpc.access_token_call_credentials(USER.access_token),
         )
 
+    def to_headers(self) -> dict[str, str]:
+        token = USER.bearer_token
+        return {"Authorization": token}
+
 
 @dataclass
 class ServerlessSecret:
     name: str
     created_at: datetime
 
 
-def _key_credentials() -> FalServerlessKeyCredentials | None:
+def key_credentials() -> FalServerlessKeyCredentials | None:
     # Ignore key credentials when the user forces auth by user.
     if os.environ.get("FAL_FORCE_AUTH_BY_USER") == "1":
         return None
 
     if "FAL_KEY_ID" in os.environ and "FAL_KEY_SECRET" in os.environ:
         return FalServerlessKeyCredentials(
             os.environ["FAL_KEY_ID"],
@@ -118,26 +128,26 @@
         return None
 
 
 def _get_agent_credentials(original_credentials: Credentials) -> Credentials:
     """If running inside a fal Serverless box, use the preconfigured credentials
     instead of the user provided ones."""
 
-    key_creds = _key_credentials()
+    key_creds = key_credentials()
     if is_agent() and key_creds:
         return key_creds
     else:
         return original_credentials
 
 
 def get_default_credentials() -> Credentials:
     if flags.AUTH_DISABLED:
         return Credentials()
 
-    key_creds = _key_credentials()
+    key_creds = key_credentials()
     if key_creds:
         return key_creds
     else:
         return AuthenticatedCredentials()
 
 
 @dataclass
@@ -160,15 +170,15 @@
     state: HostedRunState
 
 
 @dataclass
 class AliasInfo:
     alias: str
     revision: str
-    public: bool
+    auth_mode: str
 
 
 @dataclass(frozen=True)
 class Cron:
     cron_id: str
     cron_string: str
     next_run: datetime
@@ -247,18 +257,27 @@
         next_run=message.next_run.ToDatetime(),
         active=message.is_active,
     )
 
 
 @from_grpc.register(isolate_proto.AliasInfo)
 def _from_grpc_alias_info(message: isolate_proto.AliasInfo) -> AliasInfo:
+    if message.auth_mode is isolate_proto.ApplicationAuthMode.PUBLIC:
+        auth_mode = "public"
+    elif message.auth_mode is isolate_proto.ApplicationAuthMode.PRIVATE:
+        auth_mode = "private"
+    elif message.auth_mode is isolate_proto.ApplicationAuthMode.SHARED:
+        auth_mode = "shared"
+    else:
+        raise ValueError(f"Unknown auth mode: {message.auth_mode}")
+
     return AliasInfo(
         alias=message.alias,
         revision=message.revision,
-        public=message.is_public,
+        auth_mode=auth_mode,
     )
 
 
 @from_grpc.register(isolate_proto.RegisterApplicationResult)
 def _from_grpc_register_application_result(
     message: isolate_proto.RegisterApplicationResult,
 ) -> RegisterApplicationResult:
@@ -385,35 +404,42 @@
         )
 
     def register(
         self,
         function: Callable[..., ResultT],
         environments: list[isolate_proto.EnvironmentDefinition],
         application_name: str | None = None,
-        application_is_public: bool = False,
+        application_auth_mode: Literal["public", "private", "shared"] | None = None,
         *,
         serialization_method: str = _DEFAULT_SERIALIZATION_METHOD,
         machine_requirements: MachineRequirements | None = None,
     ) -> Iterator[isolate_proto.RegisterApplicationResult]:
         wrapped_function = to_serialized_object(function, serialization_method)
         if machine_requirements:
             wrapped_requirements = isolate_proto.MachineRequirements(
                 machine_type=machine_requirements.machine_type,
                 keep_alive=machine_requirements.keep_alive,
                 base_image=machine_requirements.base_image,
             )
         else:
             wrapped_requirements = None
 
+        if application_auth_mode == "public":
+            auth_mode = isolate_proto.ApplicationAuthMode.PUBLIC
+        elif application_auth_mode == "shared":
+            auth_mode = isolate_proto.ApplicationAuthMode.SHARED
+        else:
+            auth_mode = isolate_proto.ApplicationAuthMode.PRIVATE
+
         request = isolate_proto.RegisterApplicationRequest(
             function=wrapped_function,
             environments=environments,
             machine_requirements=wrapped_requirements,
             application_name=application_name,
-            is_public=application_is_public,
+            auth_mode=auth_mode,
         )
         for partial_result in self.stub.RegisterApplication(request):
             yield from_grpc(partial_result)
 
     def run(
         self,
         function: Callable[..., ResultT],
@@ -445,22 +471,20 @@
         for partial_result in self.stub.Run(request):
             yield from_grpc(partial_result)
 
     def schedule_cronjob(
         self,
         application_id: str,
         cron: str,
-    ) -> isolate_proto.RegisterCronResult:
+    ) -> str:
         request = isolate_proto.RegisterCronRequest(
             application_id=application_id, cron=cron
         )
-        response: isolate_proto.RegisterApplicationResultType = self.stub.RegisterCron(
-            request
-        )
-        return response
+        response: isolate_proto.RegisterCronResult = self.stub.RegisterCron(request)
+        return response.result.cron_id
 
     def list_aliases(self) -> list[AliasInfo]:
         request = isolate_proto.ListAliasesRequest()
         response: isolate_proto.ListAliasesResult = self.stub.ListAliases(request)
         return [from_grpc(alias) for alias in response.aliases]
 
     def list_scheduled_runs(self) -> list[Cron]:
```

### Comparing `fal_serverless-0.6.35/setup.py` & `fal_serverless-0.6.36/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['auth0-python>=4.1.0,<5.0.0',
  'click>=8.1.3,<9.0.0',
  'colorama>=0.4.6,<0.5.0',
  'datadog-api-client==2.12.0',
  'dill>=0.3.6,<0.3.7',
  'grpc-interceptor>=0.15.0,<0.16.0',
  'grpcio>=1.50.0,<2.0.0',
- 'isolate-proto>=0.0.31,<0.0.32',
+ 'isolate-proto==0.0.32',
  'isolate[build]>=0.12.2,<1.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'packaging>=21.3',
  'pathspec>=0.11.1,<0.12.0',
  'portalocker>=2.7.0,<3.0.0',
  'requests>=2.28.1,<3.0.0',
@@ -38,15 +38,15 @@
 {':python_version < "3.10"': ['importlib-metadata>=4.4']}
 
 entry_points = \
 {'console_scripts': ['fal-serverless = fal_serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal-serverless',
-    'version': '0.6.35',
+    'version': '0.6.36',
     'description': 'fal Serverless is an easy-to-use Serverless Python Framework',
     'long_description': '# fal-serverless\n\nLibrary to run, serve or schedule your Python functions in the cloud with any machine type you may need.\n\nCheck out to the [docs](https://docs.fal.ai/fal-serverless/quickstart) for more details.\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fal_serverless-0.6.35/PKG-INFO` & `fal_serverless-0.6.36/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal-serverless
-Version: 0.6.35
+Version: 0.6.36
 Summary: fal Serverless is an easy-to-use Serverless Python Framework
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: datadog-api-client (==2.12.0)
 Requires-Dist: dill (>=0.3.6,<0.3.7)
 Requires-Dist: grpc-interceptor (>=0.15.0,<0.16.0)
 Requires-Dist: grpcio (>=1.50.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
-Requires-Dist: isolate-proto (>=0.0.31,<0.0.32)
+Requires-Dist: isolate-proto (==0.0.32)
 Requires-Dist: isolate[build] (>=0.12.2,<1.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
 Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

