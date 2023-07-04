# Comparing `tmp/gundi_client_v2-2.0.0.tar.gz` & `tmp/gundi_client_v2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_client_v2-2.0.0.tar", max compression
+gzip compressed data, was "gundi_client_v2-2.0.1.tar", max compression
```

## Comparing `gundi_client_v2-2.0.0.tar` & `gundi_client_v2-2.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1681 2023-06-14 13:04:46.190963 gundi_client_v2-2.0.0/README.md
--rw-r--r--   0        0        0       53 2023-06-16 14:01:41.406285 gundi_client_v2-2.0.0/gundi_client_v2/__init__.py
--rw-r--r--   0        0        0      684 2023-06-16 13:13:56.285203 gundi_client_v2-2.0.0/gundi_client_v2/auth.py
--rw-r--r--   0        0        0     4749 2023-06-22 16:10:22.388822 gundi_client_v2-2.0.0/gundi_client_v2/client.py
--rw-r--r--   0        0        0        0 2023-06-16 12:38:36.081819 gundi_client_v2-2.0.0/gundi_client_v2/errors.py
--rw-r--r--   0        0        0      657 2023-06-16 12:43:16.414342 gundi_client_v2-2.0.0/gundi_client_v2/settings.py
--rw-r--r--   0        0        0      678 2023-06-26 15:00:44.618185 gundi_client_v2-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 gundi_client_v2-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1542 2023-07-04 12:49:45.871005 gundi_client_v2-2.0.1/README.md
+-rw-r--r--   0        0        0       53 2023-06-16 14:01:41.406285 gundi_client_v2-2.0.1/gundi_client_v2/__init__.py
+-rw-r--r--   0        0        0      684 2023-06-16 13:13:56.285203 gundi_client_v2-2.0.1/gundi_client_v2/auth.py
+-rw-r--r--   0        0        0     4824 2023-07-03 21:19:55.524453 gundi_client_v2-2.0.1/gundi_client_v2/client.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:38:36.081819 gundi_client_v2-2.0.1/gundi_client_v2/errors.py
+-rw-r--r--   0        0        0      657 2023-06-16 12:43:16.414342 gundi_client_v2-2.0.1/gundi_client_v2/settings.py
+-rw-r--r--   0        0        0      678 2023-07-04 12:36:57.916916 gundi_client_v2-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 gundi_client_v2-2.0.1/PKG-INFO
```

### Comparing `gundi_client_v2-2.0.0/gundi_client_v2/auth.py` & `gundi_client_v2-2.0.1/gundi_client_v2/auth.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.0.0/gundi_client_v2/client.py` & `gundi_client_v2-2.0.1/gundi_client_v2/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,18 @@
         self.integrations_endpoint = f"{self.api_base_path}/integrations"
         self.source_states_endpoint = f"{self.api_base_path}/sources/states"
         self.sources_endpoint = f"{self.api_base_path}/sources"
         self.routes_endpoint = f"{self.api_base_path}/routes"
 
         # Authentication settings
         self.ssl_verify = kwargs.get("use_ssl", settings.GUNDI_API_SSL_VERIFY)
-        self.client_id = kwargs.get("KEYCLOAK_CLIENT_ID", settings.KEYCLOAK_CLIENT_ID)
-        self.client_secret = kwargs.get("KEYCLOAK_CLIENT_SECRET", settings.KEYCLOAK_CLIENT_SECRET)
-        self.oauth_token_url = kwargs.get("OAUTH_TOKEN_URL", settings.OAUTH_TOKEN_URL)
-        self.audience = kwargs.get("KEYCLOAK_AUDIENCE", settings.KEYCLOAK_AUDIENCE)
+        self.client_id = kwargs.get("keycloak_client_id", settings.KEYCLOAK_CLIENT_ID)
+        self.client_secret = kwargs.get("keycloak_client_secret", settings.KEYCLOAK_CLIENT_SECRET)
+        self.oauth_token_url = kwargs.get("oauth_token_url", settings.OAUTH_TOKEN_URL)
+        self.audience = kwargs.get("keycloak_audience", settings.KEYCLOAK_AUDIENCE)
         self.cached_token = None
         self.cached_token_expires_at = datetime.min.replace(tzinfo=timezone.utc)
 
         # Retries and timeouts settings
         self.max_retries = kwargs.get('max_http_retries', self.DEFAULT_CONNECTION_RETRIES)
         transport = AsyncHTTPTransport(retries=self.max_retries)
         connect_timeout = kwargs.get('connect_timeout', self.DEFAULT_CONNECT_TIMEOUT_SECONDS)
@@ -95,35 +95,35 @@
     async def get_connection_details(self, integration_id):
         headers = await self.get_auth_header()
         url = f"{self.connections_endpoint}/{integration_id}/"
         response = await self._session.get(
             url,
             headers=headers,
         )
-        # ToDo: Handle errors
+        # ToDo: Add custom exceptions to handle errors
         response.raise_for_status()
         data = response.json()
         return Connection.parse_obj(data)
 
     async def get_route_details(self, route_id):
         headers = await self.get_auth_header()
         url = f"{self.routes_endpoint}/{route_id}/"
         response = await self._session.get(
             url,
             headers=headers,
         )
-        # ToDo: Handle errors
+        # ToDo: Add custom exceptions to handle errors
         response.raise_for_status()
         data = response.json()
         return Route.parse_obj(data)
 
     async def get_integration_details(self, integration_id):
         headers = await self.get_auth_header()
         url = f"{self.integrations_endpoint}/{integration_id}/"
         response = await self._session.get(
             url,
             headers=headers,
         )
-        # ToDo: Handle errors
+        # ToDo: Add custom exceptions to handle errors
         response.raise_for_status()
         data = response.json()
         return Integration.parse_obj(data)
```

### Comparing `gundi_client_v2-2.0.0/gundi_client_v2/settings.py` & `gundi_client_v2-2.0.1/gundi_client_v2/settings.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.0.0/pyproject.toml` & `gundi_client_v2-2.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gundi-client-v2"
-version = "2.0.0"
+version = "2.0.1"
 description = "An async client for Gundi's API"
 authors = [
     "Chris Doehring <chrisdo@earthranger.com>",
     "Mariano M <marianom@earthranger.com>",
     "Victor Garcia <victorg@earthranger.com>"
 ]
 license = "Apache-2.0"
```

### Comparing `gundi_client_v2-2.0.0/PKG-INFO` & `gundi_client_v2-2.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gundi-client-v2
-Version: 2.0.0
+Version: 2.0.1
 Summary: An async client for Gundi's API
 License: Apache-2.0
 Author: Chris Doehring
 Author-email: chrisdo@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -23,58 +23,56 @@
 # Gundi Client
 ## Introduction
 [Gundi](https://www.earthranger.com/), a.k.a "The Portal" is a platform to manage integrations.
 The gundi-client is an async python client to interact with Gundi's REST API.
 
 ## Installation
 ```
-pip install gundi-client
+pip install gundi-client-v2
 ```
 
 ## Usage
 
 ```
-from gundi_client import PortalApi
+from gundi_client_v2 import GundiClient
 import httpx
 
 # You can use it as an async context-managed client
-async with PortalApi() as portal:
+async with GundiClient() as client:
    try:
-    response = await portal.get_outbound_integration_list(
-        session=session, inbound_id=str(inbound_id), device_id=str(device_id)
+    connection = await client.get_connection_details(
+        integration_id="some-integration-uuid"
     )
     except httpx.RequestError as e:
         logger.exception("Request Error")   
         ...
     except httpx.TimeoutException as e:
         logger.exception("Request timed out")
         ...
     except httpx.HTTPStatusError as e:
         logger.exception("Response returned error")
     else:
-        # response contains a list configs as dicts
-        for integration in response:  
+        for integration in connection.destinations:  
             ...
    ...
 
 # Or create an instance and close the client explicitly later
-portal = PortalApi()
+client = GundiClient()
 try:
-    response = await portal.get_outbound_integration_list(
-        session=session, inbound_id=str(inbound_id), device_id=str(device_id)
+    response = await client.get_connection_details(
+        integration_id="some-integration-uuid"
     )
     except httpx.RequestError as e:
         logger.exception("Request Error")   
         ...
     except httpx.TimeoutException as e:
         logger.exception("Request timed out")
         ...
     except httpx.HTTPStatusError as e:
         logger.exception("Response returned error")
     else:
-        # response contains a list configs as dicts
-        for integration in response:  
+        for integration in connection.destinations:
             ...
    ...
-   await portal.close()  # Close the session used to send requests to ER API
+   await client.close()  # Close the session used to send requests to Gundi
 ```
```

