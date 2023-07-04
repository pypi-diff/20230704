# Comparing `tmp/neosctl-0.8.6.tar.gz` & `tmp/neosctl-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.6.tar", max compression
+gzip compressed data, was "neosctl-0.8.7.tar", max compression
```

## Comparing `neosctl-0.8.6.tar` & `neosctl-0.8.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-06-30 08:38:12.975171 neosctl-0.8.6/README.md
--rw-r--r--   0        0        0       22 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/constant.py
--rw-r--r--   0        0        0     4528 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14331 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-06-30 08:38:12.976172 neosctl-0.8.6/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     5491 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     4556 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3564 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1409 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     5472 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3216 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      141 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     8649 2023-06-30 08:38:12.977172 neosctl-0.8.6/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12292 2023-06-30 08:38:12.978171 neosctl-0.8.6/neosctl/util.py
--rw-r--r--   0        0        0     3050 2023-06-30 08:38:12.978171 neosctl-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-07-04 09:13:12.726821 neosctl-0.8.7/README.md
+-rw-r--r--   0        0        0       22 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-07-04 09:13:12.726821 neosctl-0.8.7/neosctl/constant.py
+-rw-r--r--   0        0        0     4528 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5491 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3564 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-07-04 09:13:12.727821 neosctl-0.8.7/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     5684 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3243 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      122 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     8649 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12390 2023-07-04 09:13:12.728821 neosctl-0.8.7/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-07-04 09:13:12.729821 neosctl-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.7/PKG-INFO
```

### Comparing `neosctl-0.8.6/README.md` & `neosctl-0.8.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.6
+# Core CLI v0.8.7
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.8.6/neosctl/auth.py` & `neosctl-0.8.7/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/cli.py` & `neosctl-0.8.7/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/profile.py` & `neosctl-0.8.7/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/schema.py` & `neosctl-0.8.7/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/__init__.py` & `neosctl-0.8.7/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/data_product.py` & `neosctl-0.8.7/neosctl/services/gateway/data_product.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/data_source.py` & `neosctl-0.8.7/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/data_system.py` & `neosctl-0.8.7/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/data_unit.py` & `neosctl-0.8.7/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/entity.py` & `neosctl-0.8.7/neosctl/services/gateway/entity.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/link.py` & `neosctl-0.8.7/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/output.py` & `neosctl-0.8.7/neosctl/services/gateway/output.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/schema.py` & `neosctl-0.8.7/neosctl/services/gateway/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/secret.py` & `neosctl-0.8.7/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/spark.py` & `neosctl-0.8.7/neosctl/services/gateway/spark.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/gateway/tag.py` & `neosctl-0.8.7/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/iam/iam.py` & `neosctl-0.8.7/neosctl/services/iam/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing
+from uuid import UUID
 
 import httpx
 import typer
 
 from neosctl import constant, util
 from neosctl.services.iam import schema
 from neosctl.util import process_response
@@ -148,31 +149,35 @@
     r = _request(ctx)
     process_response(r)
 
 
 @app.command(name="user-permissions")
 def user_permissions(
     ctx: typer.Context,
-    username: str = typer.Argument(..., help="Keycloak username", callback=util.sanitize),
+    username: str = typer.Option(None, help="Keycloak username", callback=util.sanitize),
+    identifier: UUID = typer.Option(None, help="User or Group identifier", callback=util.sanitize),
 ) -> None:
     """List existing keycloak user permissions."""
 
     @util.ensure_login
     def _request(ctx: typer.Context) -> httpx.Response:
-        r = util.get(
-            ctx,
-            _iam_url(ctx.obj.get_iam_api_url(), "users"),
-            params={"search": username},
-        )
-        if r.status_code >= constant.BAD_REQUEST_CODE:
-            process_response(r)
+        user_id = identifier
 
-        data = r.json()
-        # In case search term matches email/name of another user, filter for specific username
-        user_id = next((user["id"] for user in data["users"] if user["username"] == username), None)
+        if username:
+            r = util.get(
+                ctx,
+                _iam_url(ctx.obj.get_iam_api_url(), "users"),
+                params={"search": username},
+            )
+            if r.status_code >= constant.BAD_REQUEST_CODE:
+                process_response(r)
+
+            data = r.json()
+            # In case search term matches email/name of another user, filter for specific username
+            user_id = next((user["id"] for user in data["users"] if user["username"] == username), None)
 
         if user_id is None:
             typer.echo("User not found.")
             raise typer.Exit(code=1)
 
         return util.get(
             ctx,
```

### Comparing `neosctl-0.8.6/neosctl/services/iam/schema.py` & `neosctl-0.8.7/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/services/registry/registry.py` & `neosctl-0.8.7/neosctl/services/registry/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,18 @@
 
     @util.ensure_login
     def _request(ctx: typer.Context, rc: RegisterCore) -> httpx.Response:
         return util.post(
             ctx,
             _core_url(ctx.obj.get_registry_api_url()),
             json=rc.dict(exclude_none=True),
+            headers={"X-Partition": partition},
         )
 
-    rc = RegisterCore(partition=partition, name=name)
+    rc = RegisterCore(name=name)
 
     r = _request(ctx, rc)
     process_response(r)
 
 
 @app.command(name="list-cores")
 def list_cores(
```

### Comparing `neosctl-0.8.6/neosctl/services/storage/storage.py` & `neosctl-0.8.7/neosctl/services/storage/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.6/neosctl/util.py` & `neosctl-0.8.7/neosctl/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,18 @@
     """Trying to read and parse JSON file into the given data type."""
     fp = get_file_location(filepath)
     obj = load_json_file(fp, file_description)
     return t(**obj)
 
 
 def _request(ctx: click.Context, method: str, url: str, **kwargs: ...) -> httpx.Response:
-    return httpx.request(method=method, url=url, headers=bearer(ctx), verify=not ctx.obj.profile.ignore_tls, **kwargs)
+    headers = bearer(ctx) or {}
+    headers_ = kwargs.pop("headers", {})
+    headers.update(headers_)
+    return httpx.request(method=method, url=url, headers=headers, verify=not ctx.obj.profile.ignore_tls, **kwargs)
 
 
 def _request_and_process(ctx: click.Context, method: str, url: str, **kwargs: ...) -> None:
     @ensure_login
     def internal_request(context: click.Context) -> httpx.Response:
         return _request(context, method, url, **kwargs)
```

### Comparing `neosctl-0.8.6/pyproject.toml` & `neosctl-0.8.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.6"
+version = "0.8.7"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.8.6/PKG-INFO` & `neosctl-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.6
+Version: 0.8.7
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.6
+# Core CLI v0.8.7
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

