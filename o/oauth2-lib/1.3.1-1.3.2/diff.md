# Comparing `tmp/oauth2_lib-1.3.1.tar.gz` & `tmp/oauth2_lib-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2_lib-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "oauth2_lib-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `oauth2_lib-1.3.1.tar` & `oauth2_lib-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      363 2023-07-03 07:25:16.304500 oauth2_lib-1.3.1/.bumpversion.cfg
--rw-r--r--   0        0        0      550 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0      389 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1894 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1451 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.github/workflows/test-package.yml
--rw-r--r--   0        0        0     1115 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.gitignore
--rw-r--r--   0        0        0     1668 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/LICENSE
--rw-r--r--   0        0        0     1754 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/README.md
--rwxr-xr-x   0        0        0      150 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/fmt_code.sh
--rw-r--r--   0        0        0      671 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/__init__.py
--rw-r--r--   0        0        0     5328 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/async_api_client.py
--rw-r--r--   0        0        0    15661 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/fastapi.py
--rw-r--r--   0        0        0     6098 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/graphql_authentication.py
--rw-r--r--   0        0        0        0 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/py.typed
--rw-r--r--   0        0        0      943 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/oauth2_lib/settings.py
--rw-r--r--   0        0        0     2803 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1151 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/setup.cfg
--rw-r--r--   0        0        0        0 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1540 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/conftest.py
--rw-r--r--   0        0        0     2795 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/conftest.py
--rw-r--r--   0        0        0     1541 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/test_authenticated_federated_field.py
--rw-r--r--   0        0        0     2360 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/test_authenticated_field.py
--rw-r--r--   0        0        0     3052 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/graphql/test_authenticated_mutation_field.py
--rw-r--r--   0        0        0     5708 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_async_api_client.py
--rw-r--r--   0        0        0    13734 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_fastapi.py
--rw-r--r--   0        0        0     6570 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_opa_decision.py
--rw-r--r--   0        0        0     4289 2023-07-03 07:25:16.308500 oauth2_lib-1.3.1/tests/test_opa_graphql_decision.py
--rw-r--r--   0        0        0     4000 1970-01-01 00:00:00.000000 oauth2_lib-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.bumpversion.cfg
+-rw-r--r--   0        0        0      550 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0      389 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1894 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1451 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.github/workflows/test-package.yml
+-rw-r--r--   0        0        0     1115 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1790 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/.stignore
+-rw-r--r--   0        0        0    11358 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1754 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/README.md
+-rwxr-xr-x   0        0        0      150 2023-07-04 12:25:57.049553 oauth2_lib-1.3.2/fmt_code.sh
+-rw-r--r--   0        0        0      671 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/oauth2_lib/__init__.py
+-rw-r--r--   0        0        0     5328 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/oauth2_lib/async_api_client.py
+-rw-r--r--   0        0        0    14839 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/oauth2_lib/fastapi.py
+-rw-r--r--   0        0        0        0 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/oauth2_lib/py.typed
+-rw-r--r--   0        0        0     1062 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/oauth2_lib/settings.py
+-rw-r--r--   0        0        0     7791 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/oauth2_lib/strawberry.py
+-rw-r--r--   0        0        0     2822 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1203 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/setup.cfg
+-rw-r--r--   0        0        0        0 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     2783 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/strawberry/conftest.py
+-rw-r--r--   0        0        0     1541 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/strawberry/test_authenticated_federated_field.py
+-rw-r--r--   0        0        0     2360 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/strawberry/test_authenticated_field.py
+-rw-r--r--   0        0        0     3052 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/strawberry/test_authenticated_mutation_field.py
+-rw-r--r--   0        0        0     5708 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/test_async_api_client.py
+-rw-r--r--   0        0        0    13734 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/test_fastapi.py
+-rw-r--r--   0        0        0     6570 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/test_opa_decision.py
+-rw-r--r--   0        0        0     5118 2023-07-04 12:25:57.053553 oauth2_lib-1.3.2/tests/test_opa_graphql_decision.py
+-rw-r--r--   0        0        0     4027 1970-01-01 00:00:00.000000 oauth2_lib-1.3.2/PKG-INFO
```

### Comparing `oauth2_lib-1.3.1/.github/workflows/publish-release.yml` & `oauth2_lib-1.3.2/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/.github/workflows/scheduled-build.yml` & `oauth2_lib-1.3.2/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/.github/workflows/test-package.yml` & `oauth2_lib-1.3.2/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/.gitignore` & `oauth2_lib-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/.pre-commit-config.yaml` & `oauth2_lib-1.3.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.8.0
     hooks:
       - id: pyupgrade
         args:
           - --py39-plus
           - --keep-runtime-typing
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3.9
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.10.0]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
+        exclude: .bumpversion.cfg
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
         exclude: (charts/*|.gitlab-ci.yml)
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: detect-private-key
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
     rev: v0.0.275
     hooks:
       - id: ruff
+        args: [ --fix, --exit-non-zero-on-fix, --show-fixes ]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         language_version: python3.9
-        additional_dependencies: [pydantic]
+        additional_dependencies: [pydantic<2.0.0, strawberry-graphql]
         args:
           - --no-warn-unused-ignores
           - --allow-untyped-decorators
         exclude: (test/*|migrations/*)
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: python-use-type-annotations
       - id: python-check-mock-methods
       - id: rst-backticks
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.5
     hooks:
       - id: shellcheck
   - repo: https://github.com/andreoliwa/nitpick
-    rev: v0.33.1
+    rev: v0.33.2
     hooks:
       - id: nitpick
```

### Comparing `oauth2_lib-1.3.1/LICENSE` & `oauth2_lib-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/README.md` & `oauth2_lib-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/oauth2_lib/__init__.py` & `oauth2_lib-1.3.2/oauth2_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the SURF Oauth2 module that interfaces with the oauth2 setup."""
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
```

### Comparing `oauth2_lib-1.3.1/oauth2_lib/async_api_client.py` & `oauth2_lib-1.3.2/oauth2_lib/async_api_client.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/oauth2_lib/fastapi.py` & `oauth2_lib-1.3.2/oauth2_lib/fastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import re
-from collections.abc import AsyncGenerator, Coroutine, Mapping
+from collections.abc import AsyncGenerator, Awaitable, Mapping
 from http import HTTPStatus
 from json import JSONDecodeError
 from typing import Any, Callable, Union, cast
 
 from fastapi.exceptions import HTTPException
 from fastapi.param_functions import Depends
 from fastapi.requests import Request
@@ -278,21 +278,48 @@
                 openid_url=self.openid_url,
             )
             raise HTTPException(status_code=HTTPStatus.UNAUTHORIZED, detail=response.text)
 
         return OIDCUserModel(data)
 
 
+async def _get_decision(async_request: AsyncClient, opa_url: str, opa_input: dict) -> OPAResult:
+    logger.debug("Posting input json to Policy agent", opa_url=opa_url, input=opa_input)
+    try:
+        result = await async_request.post(opa_url, json=opa_input)
+    except (NetworkError, TypeError) as exc:
+        logger.debug("Could not get decision from policy agent", error=str(exc))
+        raise HTTPException(status_code=HTTPStatus.SERVICE_UNAVAILABLE, detail="Policy agent is unavailable")
+
+    return OPAResult.parse_obj(result.json())
+
+
+def _evaluate_decision(decision: OPAResult, auto_error: bool, **context: dict[str, Any]) -> bool:
+    did = decision.decision_id
+    if decision.result:
+        logger.debug("User is authorized to access the resource", decision_id=did, **context)
+        return True
+
+    logger.debug("User is not allowed to access the resource", decision_id=did, **context)
+    if not auto_error:
+        return False
+
+    raise HTTPException(
+        status_code=HTTPStatus.FORBIDDEN,
+        detail=f"User is not allowed to access resource: {context.get('resource')} Decision was taken with id: {did}",
+    )
+
+
 def opa_decision(
     opa_url: str,
     oidc_security: OIDCUser,
     enabled: bool = True,
     auto_error: bool = True,
     opa_kwargs: Union[Mapping[str, str], None] = None,
-) -> Callable[[Request, OIDCUserModel, AsyncClient], Coroutine[Any, Any, Union[bool, None]]]:
+) -> Callable[[Request, OIDCUserModel, AsyncClient], Awaitable[Union[bool, None]]]:
     async def _opa_decision(
         request: Request,
         user_info: OIDCUserModel = Depends(oidc_security),
         async_request: AsyncClient = Depends(async_client),
     ) -> Union[bool, None]:
         """Check OIDCUserModel against the OPA policy.
 
@@ -301,84 +328,60 @@
 
         Args:
             request: Request object that will be used to retrieve request metadata.
             user_info: The OIDCUserModel object that will be checked
             async_request: The httpx client.
         """
 
-        if enabled:
-            try:
-                json = await request.json()
-            # Silencing the Decode error or Type error when request.json() does not return anything sane.
-            # Some requests do not have a json response therefore as this code gets called on every request
-            # we need to suppress the `None` case (TypeError) or the `other than json` case (JSONDecodeError)
-            # Suppress AttributeError in case of websocket request, it doesn't have .json
-            except (JSONDecodeError, TypeError, ClientDisconnect, AttributeError):
-                json = {}
-
-            # defaulting to GET request method for WebSocket request, it doesn't have .method
-            requestMethod = request.method if hasattr(request, "method") else "GET"
-            opa_input = {
-                "input": {
-                    **(opa_kwargs or {}),
-                    **user_info,
-                    "resource": request.url.path,
-                    "method": requestMethod,
-                    "arguments": {"path": request.path_params, "query": {**request.query_params}, "json": json},
-                }
-            }
+        if not enabled:
+            return None
 
-            logger.debug("Posting input json to Policy agent", input=opa_input)
-
-            try:
-                result = await async_request.post(opa_url, json=opa_input)
-            except (NetworkError, TypeError):
-                raise HTTPException(status_code=HTTPStatus.SERVICE_UNAVAILABLE, detail="Policy agent is unavailable")
-
-            data = OPAResult.parse_obj(result.json())
-
-            if not data.result and auto_error:
-                logger.debug(
-                    "User is not allowed to access the resource",
-                    decision_id=data.decision_id,
-                    resource=request.url.path,
-                    method=requestMethod,
-                    user_info=user_info,
-                    input=opa_input,
-                    url=request.url,
-                )
-                raise HTTPException(
-                    status_code=HTTPStatus.FORBIDDEN,
-                    detail=f"User is not allowed to access resource: {request.url.path} Decision was taken with id: {data.decision_id}",
-                )
-            if data.result:
-                logger.debug(
-                    "User is authorized to access the resource",
-                    decision_id=data.decision_id,
-                    resource=request.url.path,
-                    method=requestMethod,
-                    user_info=user_info,
-                    input=opa_input,
-                )
+        try:
+            json = await request.json()
+        # Silencing the Decode error or Type error when request.json() does not return anything sane.
+        # Some requests do not have a json response therefore as this code gets called on every request
+        # we need to suppress the `None` case (TypeError) or the `other than json` case (JSONDecodeError)
+        # Suppress AttributeError in case of websocket request, it doesn't have .json
+        except (JSONDecodeError, TypeError, ClientDisconnect, AttributeError):
+            json = {}
+
+        # defaulting to GET request method for WebSocket request, it doesn't have .method
+        request_method = request.method if hasattr(request, "method") else "GET"
+        opa_input = {
+            "input": {
+                **(opa_kwargs or {}),
+                **user_info,
+                "resource": request.url.path,
+                "method": request_method,
+                "arguments": {"path": request.path_params, "query": {**request.query_params}, "json": json},
+            }
+        }
 
-            return data.result
+        decision = await _get_decision(async_request, opa_url, opa_input)
 
-        return None
+        context = {
+            "resource": opa_input["input"]["resource"],
+            "method": opa_input["input"]["method"],
+            "user_info": user_info,
+            "input": opa_input,
+            "url": request.url,
+        }
+        return _evaluate_decision(decision, auto_error, **context)
 
     return _opa_decision
 
 
 def opa_graphql_decision(
     opa_url: str,
     _oidc_security: OIDCUser,
     enabled: bool = True,
-    auto_error: bool = True,
+    auto_error: bool = False,  # By default don't raise HTTP 403 because partial results are preferred
     opa_kwargs: Union[Mapping[str, str], None] = None,
     async_request: Union[AsyncClient, None] = None,
-) -> Callable[[str, OIDCUserModel], Coroutine[Any, Any, Union[bool, None]]]:
+) -> Callable[[str, OIDCUserModel], Awaitable[Union[bool, None]]]:
     async def _opa_decision(
         path: str,
         oidc_user: OIDCUserModel = Depends(_oidc_security),
         async_request_1: Union[AsyncClient, None] = None,
     ) -> Union[bool, None]:
         """Check OIDCUserModel against the OPA policy.
 
@@ -386,51 +389,28 @@
         This method will make an async call towards the Policy agent.
 
         Args:
             path: the graphql path that will be checked against the permissions of the oidc_user
             oidc_user: The OIDCUserModel object that will be checked
             async_request_1: The Async client
         """
-        if enabled:
-            opa_input = {
-                "input": {
-                    **(opa_kwargs or {}),
-                    **oidc_user,
-                    "resource": path,
-                    "method": "POST",
-                }
+        if not enabled:
+            return None
+
+        opa_input = {
+            "input": {
+                **(opa_kwargs or {}),
+                **oidc_user,
+                "resource": path,
+                "method": "POST",
             }
+        }
 
-            logger.debug("Posting input json to Policy agent", input=opa_input)
-            client_request = async_request if async_request else async_request_1
-            client_request = client_request if client_request else AsyncClient(http1=True)
-            try:
-                result = await client_request.post(opa_url, json=opa_input)
-            except (NetworkError, TypeError):
-                raise HTTPException(status_code=HTTPStatus.SERVICE_UNAVAILABLE, detail="Policy agent is unavailable")
-
-            data = OPAResult.parse_obj(result.json())
-
-            resource = opa_input["input"]["resource"]
-
-            if not data.result and auto_error:
-                logger.debug(
-                    "User is not allowed to access the resource",
-                    decision_id=data.decision_id,
-                    path=path,
-                    input=opa_input,
-                )
-                return False
-            if data.result:
-                logger.debug(
-                    "User is authorized to access the resource",
-                    decision_id=data.decision_id,
-                    resource=resource,
-                    path=path,
-                    input=opa_input,
-                )
+        client_request = async_request if async_request else async_request_1
+        client_request = client_request if client_request else AsyncClient(http1=True)
 
-            return data.result
+        decision = await _get_decision(client_request, opa_url, opa_input)
 
-        return None
+        context = {"resource": opa_input["input"]["resource"], "input": opa_input}
+        return _evaluate_decision(decision, auto_error, **context)
 
     return _opa_decision
```

### Comparing `oauth2_lib-1.3.1/oauth2_lib/graphql_authentication.py` & `oauth2_lib-1.3.2/oauth2_lib/strawberry.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,139 +6,194 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from collections.abc import Awaitable
 from typing import Any, Callable, Union
 
+import asyncstdlib
 import strawberry
 import structlog
 from fastapi import HTTPException
 from graphql.pyutils import Path
+from starlette.requests import Request
 from strawberry import BasePermission
 from strawberry.fastapi import BaseContext
 from strawberry.types import Info
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import RootValueType
 
 from oauth2_lib.fastapi import OIDCUserModel
 from oauth2_lib.settings import oauth2lib_settings
 
 logger = structlog.get_logger(__name__)
 
 
 class OauthContext(BaseContext):
+    @asyncstdlib.cached_property
+    async def get_current_user(self) -> Union[OIDCUserModel, None]:
+        """Retrieve the OIDCUserModel once per graphql request.
+
+        Note:
+            This function should not raise exceptions, otherwise it will not be cached.
+        """
+        if not isinstance(self.request, Request):  # it could be None or a WebSocket
+            logger.debug("Can't retrieve OIDCUserModel without a starlette Request", request_type=type(self.request))
+            return None
+
+        if not oauth2lib_settings.OAUTH2_ACTIVE:
+            logger.debug("Not retrieving OIDCUserModel because OAUTH2_ACTIVE=False")
+            return None
+
+        try:
+            return await self._get_current_user(self.request)
+        except HTTPException as exc:
+            logger.debug("User is not authenticated", status_code=exc.status_code, detail=exc.detail)
+            return None
+
     def __init__(
-        self, get_current_user: Callable[[Any], OIDCUserModel], get_opa_decision: Callable[[str, OIDCUserModel], bool]
+        self,
+        get_current_user: Callable[[Request], Awaitable[OIDCUserModel]],
+        get_opa_decision: Callable[[str, OIDCUserModel], Awaitable[Union[bool, None]]],
     ):
-        self.get_current_user = get_current_user
+        self._get_current_user = get_current_user
         self.get_opa_decision = get_opa_decision
         super().__init__()
 
 
 OauthInfo = Info[OauthContext, RootValueType]
 
 
 def get_path_as_string(path: Path) -> str:
     if path.prev:
         return f"{get_path_as_string(path.prev)}/{path.key}"
     return f"{path.key}"
 
 
-class IsAuthenticated(BasePermission):
+def get_query_path(info: OauthInfo) -> str:
+    service_name = oauth2lib_settings.SERVICE_NAME
+    service_name_path = f"/{service_name}" if service_name else ""
+    return f"{service_name_path}/{get_path_as_string(info.path)}/".lower()
+
+
+def get_mutation_path(info: OauthInfo) -> str:
+    service_name = oauth2lib_settings.SERVICE_NAME
+    service_name_path = f"/{service_name}" if service_name else ""
+    return f"{service_name_path}/{info.path.key}"
+
+
+def skip_mutation_auth_checks() -> bool:
+    is_exception = oauth2lib_settings.ENVIRONMENT in oauth2lib_settings.ENVIRONMENT_IGNORE_MUTATION_DISABLED
+    logger.debug(
+        "Mutations are disabled",
+        OAUTH2_ACTIVE=oauth2lib_settings.OAUTH2_ACTIVE,
+        MUTATIONS_ENABLED=oauth2lib_settings.MUTATIONS_ENABLED,
+        is_exception=is_exception,
+    )
+    return is_exception
+
+
+async def is_authenticated(info: OauthInfo) -> bool:
+    """Check that the user has a valid and active authentication token."""
+    current_user = await info.context.get_current_user
+    return current_user is not None
+
+
+async def is_authorized(info: OauthInfo, path: str) -> bool:
+    """Check that the user is allowed to query/mutate this path."""
+    context = info.context
+    current_user = await context.get_current_user
+    if not current_user:
+        return False
+
+    opa_decision = await context.get_opa_decision(path, current_user)
+    authorized = bool(opa_decision)
+    logger.debug("Received opa decision", path=path, opa_decision=opa_decision, is_authorized=authorized)
+
+    return authorized
+
+
+class IsAuthenticatedForQuery(BasePermission):
     message = "User is not authenticated"
 
     async def has_permission(self, source: Any, info: OauthInfo, **kwargs) -> bool:  # type: ignore
         if not oauth2lib_settings.OAUTH2_ACTIVE:
             return True
 
-        service_name = oauth2lib_settings.SERVICE_NAME
-        service_name_path = f"/{service_name}" if service_name else ""
-        path = f"{service_name_path}/{get_path_as_string(info.path)}/".lower()
-
-        context = info.context
-        try:
-            logger.debug("Request headers", headers=context.request.headers)  # type: ignore
-            current_user = await context.get_current_user(context.request)  # type: ignore
-        except HTTPException:
-            self.message = f"User is not authorized to query or has an invalid access token for path: `{path}`"
-            return False
-
-        opa_decision: bool = await context.get_opa_decision(path, current_user)  # type: ignore
-
-        logger.debug("Get opa decision", path=path, opa_decision=opa_decision)
-        if not opa_decision:
-            self.message = f"User is not authorized to query `{path}`"
-
-        return opa_decision
+        return await is_authenticated(info)
 
 
 class IsAuthenticatedForMutation(BasePermission):
     message = "User is not authenticated"
 
     async def has_permission(self, source: Any, info: OauthInfo, **kwargs) -> bool:  # type: ignore
         mutations_active = oauth2lib_settings.OAUTH2_ACTIVE and oauth2lib_settings.MUTATIONS_ENABLED
+        if not mutations_active:
+            return skip_mutation_auth_checks()
+
+        return await is_authenticated(info)
+
 
-        service_name = oauth2lib_settings.SERVICE_NAME
-        service_name_path = f"/{service_name}" if service_name else ""
-        path = f"{service_name_path}/{info.path.key}"
+class IsAuthorizedForQuery(BasePermission):
+    async def has_permission(self, source: Any, info: OauthInfo, **kwargs) -> bool:  # type: ignore
+        if not oauth2lib_settings.OAUTH2_ACTIVE:
+            return True
 
+        path = get_query_path(info)
+        if await is_authorized(info, path):
+            return True
+
+        self.message = f"User is not authorized to query `{path}`"
+        return False
+
+
+class IsAuthorizedForMutation(BasePermission):
+    async def has_permission(self, source: Any, info: OauthInfo, **kwargs) -> bool:  # type: ignore
+        mutations_active = oauth2lib_settings.OAUTH2_ACTIVE and oauth2lib_settings.MUTATIONS_ENABLED
         if not mutations_active:
-            is_exception = oauth2lib_settings.ENVIRONMENT in oauth2lib_settings.ENVIRONMENT_IGNORE_MUTATION_DISABLED
-            logger.debug(
-                "Mutations are disabled",
-                OAUTH2_ACTIVE=oauth2lib_settings.OAUTH2_ACTIVE,
-                MUTATIONS_ENABLED=oauth2lib_settings.MUTATIONS_ENABLED,
-                is_exception=is_exception,
-            )
-            return is_exception
+            return skip_mutation_auth_checks()
 
-        try:
-            current_user = await info.context.get_current_user(info.context.request)  # type: ignore
-        except HTTPException:
-            self.message = f"User is not authorized to query or has an invalid access token for path: `{path}`"
-            return False
-        opa_decision: bool = await info.context.get_opa_decision(path, current_user)  # type: ignore
-
-        logger.debug("Get opa decision", path=path, opa_decision=opa_decision)
-        if not opa_decision:
-            self.message = f"User is not authorized to execute mutation `{path}`"
+        path = get_mutation_path(info)
+        if await is_authorized(info, path):
+            return True
 
-        return opa_decision
+        self.message = f"User is not authorized to execute mutation `{path}`"
+        return False
 
 
 def authenticated_field(
     description: str,
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod, None] = None,
     deprecation_reason: Union[str, None] = None,
     permission_classes: Union[list[type[BasePermission]], None] = None,
 ) -> Any:
     permissions = permission_classes if permission_classes else []
     return strawberry.field(
         description=description,
         resolver=resolver,  # type: ignore
         deprecation_reason=deprecation_reason,
-        permission_classes=[IsAuthenticated] + permissions,
+        permission_classes=[IsAuthenticatedForQuery, IsAuthorizedForQuery] + permissions,
     )
 
 
 def authenticated_mutation_field(
     description: str,
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod, None] = None,
     deprecation_reason: Union[str, None] = None,
     permission_classes: Union[list[type[BasePermission]], None] = None,
 ) -> Any:
     permissions = permission_classes if permission_classes else []
     return strawberry.field(
         description=description,
         resolver=resolver,  # type: ignore
         deprecation_reason=deprecation_reason,
-        permission_classes=[IsAuthenticatedForMutation] + permissions,
+        permission_classes=[IsAuthenticatedForMutation, IsAuthorizedForMutation] + permissions,
     )
 
 
 def authenticated_federated_field(  # type: ignore
     description: str,
     resolver: Union[StrawberryResolver, Callable, staticmethod, classmethod, None] = None,
     deprecation_reason: Union[str, None] = None,
@@ -147,11 +202,11 @@
     **kwargs,
 ) -> Any:
     permissions = permission_classes if permission_classes else []
     return strawberry.federation.field(
         description=description,
         resolver=resolver,  # type: ignore
         deprecation_reason=deprecation_reason,
-        permission_classes=[IsAuthenticated] + permissions,
+        permission_classes=[IsAuthenticatedForQuery, IsAuthorizedForQuery] + permissions,
         requires=requires,
         **kwargs,
     )
```

### Comparing `oauth2_lib-1.3.1/oauth2_lib/settings.py` & `oauth2_lib-1.3.2/oauth2_lib/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from pydantic import BaseSettings
+from pydantic import BaseSettings, Field
 
 
 class Oauth2LibSettings(BaseSettings):
     """Common settings for applications depending on oauth2-lib."""
 
     ENVIRONMENT: str = "local"
     SERVICE_NAME: str = ""
     MUTATIONS_ENABLED: bool = False
-    ENVIRONMENT_IGNORE_MUTATION_DISABLED: list[str] = []
+    ENVIRONMENT_IGNORE_MUTATION_DISABLED: list[str] = Field(
+        default_factory=list, description="Environments for which to allow unauthenticated mutations"
+    )
     OAUTH2_ACTIVE: bool = False
 
 
 oauth2lib_settings = Oauth2LibSettings()
```

### Comparing `oauth2_lib-1.3.1/pyproject.toml` & `oauth2_lib-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,30 @@
 ]
 requires = [
     "requests>=2.19.0",
     "structlog>=20.2.0",
     "fastapi>=0.90.1",
     "httpx[http2]==0.23.0",
     "authlib==1.0.1",
-    "pydantic>=1.8.0",
+    "pydantic>=1.8.0,<2.0.0",
     "strawberry-graphql>=0.171.1",
+    "asyncstdlib",
 ]
 description-file = "README.md"
 requires-python = ">=3.9"
 
 [tool.flit.metadata.urls]
 Documentation = "https://workfloworchestrator.org/"
 
 [tool.flit.metadata.requires-extra]
 test = [
     "apache-license-check",
     "black",
     "ruff",
-    "mypy==1.3.0",
+    "mypy",
     "opentelemetry-instrumentation-urllib3",
     "pygments",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-xdist",
     "requests_mock",
```

### Comparing `oauth2_lib-1.3.1/setup.cfg` & `oauth2_lib-1.3.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 filterwarnings =
 	ignore::DeprecationWarning:werkzeug
 	ignore::DeprecationWarning:jinja2
 	ignore::DeprecationWarning:jsonschema
 	ignore::DeprecationWarning:yaml
 
 [mypy]
+plugins = pydantic.mypy, strawberry.ext.mypy_plugin
 ignore_missing_imports = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 check_untyped_defs = True
 disallow_untyped_decorators = True
 no_implicit_optional = True
```

### Comparing `oauth2_lib-1.3.1/tests/conftest.py` & `oauth2_lib-1.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/tests/graphql/conftest.py` & `oauth2_lib-1.3.2/tests/strawberry/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import strawberry
 from fastapi import Depends, FastAPI
 from starlette.testclient import TestClient
 from strawberry.fastapi import GraphQLRouter
 
 from oauth2_lib.fastapi import opa_graphql_decision
-from oauth2_lib.graphql_authentication import (
+from oauth2_lib.strawberry import (
     OauthContext,
     authenticated_federated_field,
     authenticated_field,
     authenticated_mutation_field,
 )
 from tests.test_fastapi import user_info_matching
```

### Comparing `oauth2_lib-1.3.1/tests/graphql/test_authenticated_federated_field.py` & `oauth2_lib-1.3.2/tests/strawberry/test_authenticated_federated_field.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/tests/graphql/test_authenticated_field.py` & `oauth2_lib-1.3.2/tests/strawberry/test_authenticated_field.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/tests/graphql/test_authenticated_mutation_field.py` & `oauth2_lib-1.3.2/tests/strawberry/test_authenticated_mutation_field.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/tests/test_async_api_client.py` & `oauth2_lib-1.3.2/tests/test_async_api_client.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/tests/test_fastapi.py` & `oauth2_lib-1.3.2/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/tests/test_opa_decision.py` & `oauth2_lib-1.3.2/tests/test_opa_decision.py`

 * *Files identical despite different names*

### Comparing `oauth2_lib-1.3.1/tests/test_opa_graphql_decision.py` & `oauth2_lib-1.3.2/tests/test_opa_graphql_decision.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from http import HTTPStatus
 from typing import cast
 
 import pytest
 from fastapi import HTTPException
 
 from oauth2_lib.fastapi import OIDCUser, opa_graphql_decision
 from tests.test_fastapi import user_info_matching
@@ -14,17 +15,39 @@
 
     opa_decision_security = opa_graphql_decision("https://opa_url.test", cast(OIDCUser, mock_user_info), enabled=False)
 
     assert await opa_decision_security("", None) is None  # type:ignore
 
 
 @pytest.mark.asyncio
-async def test_opa_graphql_decision_user_not_allowed(make_mock_async_client):
+async def test_opa_graphql_decision_user_not_allowed_autoerror_true(make_mock_async_client):
     mock_async_client = make_mock_async_client({"result": False, "decision_id": "hoi"})
-    opa_decision_security = opa_graphql_decision("https://opa_url.test", None)
+    opa_decision_security = opa_graphql_decision(
+        "https://opa_url.test",
+        None,
+        auto_error=True,
+    )
+
+    with pytest.raises(HTTPException) as exception:
+        await opa_decision_security("/test/path", user_info_matching, mock_async_client)
+
+    assert exception.value.status_code == HTTPStatus.FORBIDDEN
+
+    opa_input = {"input": {**user_info_matching, "resource": "/test/path", "method": "POST"}}
+    mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
+
+
+@pytest.mark.asyncio
+async def test_opa_graphql_decision_user_not_allowed_autoerror_false(make_mock_async_client):
+    mock_async_client = make_mock_async_client({"result": False, "decision_id": "hoi"})
+    opa_decision_security = opa_graphql_decision(
+        "https://opa_url.test",
+        None,
+        auto_error=False,
+    )
 
     result = await opa_decision_security("/test/path", user_info_matching, mock_async_client)
 
     assert result is False
     opa_input = {
         "input": {
             **user_info_matching,
@@ -34,15 +57,15 @@
     }
     mock_async_client.post.assert_called_with("https://opa_url.test", json=opa_input)
 
 
 @pytest.mark.asyncio
 async def test_opa_graphql_decision_user_allowed(make_mock_async_client):
     mock_async_client = make_mock_async_client({"result": True, "decision_id": "hoi"})
-    opa_decision_security = opa_graphql_decision("https://opa_url.test", None)
+    opa_decision_security = opa_graphql_decision("https://opa_url.test", None, auto_error=False)
 
     result = await opa_decision_security("/test/path", user_info_matching, mock_async_client)
 
     assert result is True
     opa_input = {
         "input": {
             **user_info_matching,
```

### Comparing `oauth2_lib-1.3.1/PKG-INFO` & `oauth2_lib-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-lib
-Version: 1.3.1
+Version: 1.3.2
 Summary: This is the SURF Oauth2 module that interfaces with the oauth2 setup.
 Home-page: https://github.com/workfloworchestrator/oauth2-lib
 Author: SURF
 Author-email: automation-beheer@surf.nl
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -27,22 +27,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: requests>=2.19.0
 Requires-Dist: structlog>=20.2.0
 Requires-Dist: fastapi>=0.90.1
 Requires-Dist: httpx[http2]==0.23.0
 Requires-Dist: authlib==1.0.1
-Requires-Dist: pydantic>=1.8.0
+Requires-Dist: pydantic>=1.8.0,<2.0.0
 Requires-Dist: strawberry-graphql>=0.171.1
+Requires-Dist: asyncstdlib
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: apache-license-check ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: ruff ; extra == "test"
-Requires-Dist: mypy==1.3.0 ; extra == "test"
+Requires-Dist: mypy ; extra == "test"
 Requires-Dist: opentelemetry-instrumentation-urllib3 ; extra == "test"
 Requires-Dist: pygments ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: requests_mock ; extra == "test"
```

