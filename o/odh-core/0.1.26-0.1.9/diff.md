# Comparing `tmp/odh_core-0.1.26.tar.gz` & `tmp/odh_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odh_core-0.1.26.tar", last modified: Tue Jul  4 06:55:28 2023, max compression
+gzip compressed data, was "odh_core-0.1.9.tar", last modified: Wed May  3 15:19:24 2023, max compression
```

## Comparing `odh_core-0.1.26.tar` & `odh_core-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0      171 2023-05-22 12:03:26.695566 odh_core-0.1.26/README.md
--rw-r--r--   0        0        0      483 2023-07-04 06:53:53.024727 odh_core-0.1.26/odh_core/__init__.py
--rw-r--r--   0        0        0      221 2023-07-04 06:43:36.686789 odh_core-0.1.26/odh_core/akv.py
--rw-r--r--   0        0        0     5754 2023-07-04 06:52:15.279713 odh_core-0.1.26/odh_core/graphql_client.py
--rw-r--r--   0        0        0     2056 2023-04-26 15:09:47.743383 odh_core-0.1.26/odh_core/logger.py
--rw-r--r--   0        0        0     4786 2023-05-25 13:36:19.787616 odh_core-0.1.26/odh_core/logging_settings.py
--rw-r--r--   0        0        0    15013 2023-05-24 06:59:08.969078 odh_core-0.1.26/odh_core/ms_odata.py
--rw-r--r--   0        0        0     2101 2023-05-03 08:33:41.588310 odh_core-0.1.26/odh_core/phonenumber.py
--rw-r--r--   0        0        0     1189 2023-07-04 06:43:36.708808 odh_core-0.1.26/odh_core/ssn.py
--rw-r--r--   0        0        0     1482 2023-07-04 06:55:28.336121 odh_core-0.1.26/pyproject.toml
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 odh_core-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-05-03 14:19:54.886571 odh_core-0.1.9/README.md
+-rw-r--r--   0        0        0      440 2023-05-03 14:46:18.755967 odh_core-0.1.9/odh_core/__init__.py
+-rw-r--r--   0        0        0     2523 2023-05-03 08:43:09.611592 odh_core-0.1.9/odh_core/graphql_client.py
+-rw-r--r--   0        0        0     2056 2023-04-26 08:25:44.881301 odh_core-0.1.9/odh_core/logger.py
+-rw-r--r--   0        0        0     4784 2023-04-26 15:14:15.298371 odh_core-0.1.9/odh_core/logging_settings.py
+-rw-r--r--   0        0        0    12313 2023-04-28 12:42:22.472776 odh_core-0.1.9/odh_core/ms_odata.py
+-rw-r--r--   0        0        0     2101 2023-05-03 13:57:06.837560 odh_core-0.1.9/odh_core/phonenumber.py
+-rw-r--r--   0        0        0     1067 2023-05-03 15:19:24.212108 odh_core-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 odh_core-0.1.9/PKG-INFO
```

### Comparing `odh_core-0.1.26/odh_core/logger.py` & `odh_core-0.1.9/odh_core/logger.py`

 * *Files identical despite different names*

### Comparing `odh_core-0.1.26/odh_core/logging_settings.py` & `odh_core-0.1.9/odh_core/logging_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         },
     },
     # root sets default values and subsequent loggers can override the values
     # "root": {"handlers": ["console"], "level": "DEBUG"},
     "root": {"handlers": ["console"], "level": "INFO"},
     "loggers": {
         "gql.transport.aiohttp": {
-            "level": "WARNING",
+            "level": "DEBUG",
             "filters": ["hide_gql_schema", "hide_gql_IntrospectionQuery"],
             # "handlers": ["file"],
         },
         "odh": {
             "level": "INFO",
             # "handlers": ["console"],
         },
```

### Comparing `odh_core-0.1.26/odh_core/ms_odata.py` & `odh_core-0.1.9/odh_core/ms_odata.py`

 * *Files 17% similar despite different names*

```diff
@@ -286,94 +286,30 @@
         request_retry = 0
         while request_retry < 5:
             # make the request
             url = f"/{endpoint}/{resource}"
             async with self.session.post(url=url, data=data) as resp:
                 if resp.status == 204:
                     resp_json = {}
-                    return resp_json
-                # if we get 200, return the data
-                if resp.status >= 200 and resp.status < 300:
-                    resp_json = await resp.json()
-                    if not resp.ok:
-                        log.error(f'graph error: {resp_json["error"]["message"]}')
-                        log.debug(resp_json)
-                    return resp_json
-                # if we get 401, refresh the token and retry
-                elif resp.status == 401:
-                    # refresh the token
-                    await self.update_token_header()
-                    request_retry += 1
-
-                # if we get 400, raise an error, something is wrong get user code to handle it
-                elif resp.status == 400:
-                    resp_json = await resp.json()
-                    raise GraphError(resp_json["error"]["message"])
-
-                # if we get 429, wait and retry
-                elif resp.status == 429:
-                    delay = float(resp.headers["retry-after"])
-                    log.info(
-                        f"Request to {url} failed with 429, retrying in {delay} seconds"
-                    )
-                    await asyncio.sleep(delay)
-                    request_retry += 1
-                # if we get 503, wait and retry
-                elif resp.status == 503:
-                    delay = float(resp.headers["retry-after"])
-                    log.info(
-                        f"Request to {url} failed with 503, retrying in {delay} seconds"
-                    )
-                    await asyncio.sleep(delay)
-                    request_retry += 1
-                # if we get anything else, log it and return empty
                 else:
                     resp_json = await resp.json()
+                if not resp.ok:
+                    log.error(f'graph error: {resp_json["error"]["message"]}')
                     log.debug(resp_json)
-                    log.error(
-                        f"Request to {url} failed with {resp.status} {resp.reason}"
-                    )
-                    return {}
-
-    async def delete(
-        self,
-        resource: str,
-        endpoint: str = "v1.0",
-    ):
-        """Handles retry logic and token refresh for microsoft graph post request
-
-        Delete data from the graph using the odata protocol
-
-        https://learn.microsoft.com/en-us/graph/errors
-
-        """
-        request_retry = 0
-        while request_retry < 5:
-            # make the request
-            url = f"/{endpoint}/{resource}"
-            async with self.session.delete(url=url) as resp:
-                if resp.status == 204:
-                    resp_json = {}
-                    return resp_json
                 # if we get 200, return the data
                 if resp.status >= 200 and resp.status < 300:
-                    resp_json = await resp.json()
-                    if not resp.ok:
-                        log.error(f'graph error: {resp_json["error"]["message"]}')
-                        log.debug(resp_json)
                     return resp_json
                 # if we get 401, refresh the token and retry
                 elif resp.status == 401:
                     # refresh the token
                     await self.update_token_header()
                     request_retry += 1
 
                 # if we get 400, raise an error, something is wrong get user code to handle it
                 elif resp.status == 400:
-                    resp_json = await resp.json()
                     raise GraphError(resp_json["error"]["message"])
 
                 # if we get 429, wait and retry
                 elif resp.status == 429:
                     delay = float(resp.headers["retry-after"])
                     log.info(
                         f"Request to {url} failed with 429, retrying in {delay} seconds"
@@ -386,13 +322,12 @@
                     log.info(
                         f"Request to {url} failed with 503, retrying in {delay} seconds"
                     )
                     await asyncio.sleep(delay)
                     request_retry += 1
                 # if we get anything else, log it and return empty
                 else:
-                    resp_json = await resp.json()
                     log.debug(resp_json)
                     log.error(
                         f"Request to {url} failed with {resp.status} {resp.reason}"
                     )
                     return {}
```

### Comparing `odh_core-0.1.26/odh_core/phonenumber.py` & `odh_core-0.1.9/odh_core/phonenumber.py`

 * *Files identical despite different names*

### Comparing `odh_core-0.1.26/pyproject.toml` & `odh_core-0.1.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -7,85 +7,52 @@
     "tests/*",
     "test*",
     "*.log",
 ]
 
 [tool.pyright]
 reportGeneralTypeIssues = false
-reportOptionalMemberAccess = false
 reportOptionalSubscript = false
-
-[tool.ruff]
-ignore = [
-    "ANN101",
-    "ANN201",
-    "D100",
-    "D102",
-    "D103",
-    "D203",
-    "D205",
-    "D213",
-    "D417",
-    "E501",
-    "ERA001",
-    "FBT",
-    "G004",
-    "N813",
-    "RET505",
-    "T201",
-]
-select = [
-    "ALL",
-]
-
-[tool.ruff.pydocstyle]
-convention = "google"
-
-[tool.ruff.per-file-ignores]
-"odh_core/__init__.py" = [
-    "F401",
-]
+reportOptionalMemberAccess = false
 
 [project]
 authors = [
     { name = "Jimmy Spets", email = "jimmy.spets@waochurch.com" },
     { name = "Viktor Freiman", email = "viktor.freiman@waochurch.com" },
 ]
 dependencies = [
     "gql[aiohttp]",
-    "personnummer",
     "phonenumbers",
-    "python-dotenv",
     "python-jose[cryptography]",
 ]
 description = "ODH Core, helper functions and classes"
 dynamic = []
 name = "odh-core"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.1.26"
+version = "0.1.9"
 
 [project.optional-dependencies]
 dev = [
-    "azure-identity",
-    "azure-keyvault-secrets",
+    "Sphinx",
     "black",
-    "docs-helper",
-    "pytest-asyncio",
-    "pytest",
+    "flake8",
+    "flake8-bugbear",
+    "flake8-quotes",
     "rinohtype",
-    "ruff",
     "sphinx-autobuild",
     "sphinx-rtd-theme",
-    "Sphinx",
-    "sphinxcontrib-autoprogram",
     "toml",
+    "sphinxcontrib-autoprogram",
+    "docs-helper",
+    "pytest",
+    "pytest-asyncio",
 ]
 
 [project.license]
 text = "MIT"
 
 [build-system]
-build-backend = "pdm.backend"
 requires = [
     "pdm-backend",
 ]
+build-backend = "pdm.backend"
```

