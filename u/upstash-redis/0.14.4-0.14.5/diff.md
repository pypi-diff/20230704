# Comparing `tmp/upstash_redis-0.14.4.tar.gz` & `tmp/upstash_redis-0.14.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.14.4.tar", max compression
+gzip compressed data, was "upstash_redis-0.14.5.tar", max compression
```

## Comparing `upstash_redis-0.14.4.tar` & `upstash_redis-0.14.5.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0     1070 2023-07-03 04:41:33.171707 upstash_redis-0.14.4/LICENSE
--rw-r--r--   0        0        0     9173 2023-07-03 04:41:33.171707 upstash_redis-0.14.4/README.md
--rw-r--r--   0        0        0      500 2023-07-03 04:41:33.171707 upstash_redis-0.14.4/pyproject.toml
--rw-r--r--   0        0        0      146 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4896 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     5061 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/client.py
--rw-r--r--   0        0        0       77 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0       79 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    21043 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    71958 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    20072 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0      283 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     6249 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0      752 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      174 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     8861 2023-07-03 04:41:33.175707 upstash_redis-0.14.4/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.14.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-04 06:35:23.850037 upstash_redis-0.14.5/LICENSE
+-rw-r--r--   0        0        0     5266 2023-07-04 06:35:23.850037 upstash_redis-0.14.5/README.md
+-rw-r--r--   0        0        0      500 2023-07-04 06:35:23.850037 upstash_redis-0.14.5/pyproject.toml
+-rw-r--r--   0        0        0      146 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4638 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     4768 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/client.py
+-rw-r--r--   0        0        0       77 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    21043 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    71958 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    20072 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0      283 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/exception.py
+-rw-r--r--   0        0        0     4563 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/http.py
+-rw-r--r--   0        0        0      431 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0      752 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      174 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     8861 2023-07-04 06:35:23.858037 upstash_redis-0.14.5/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 upstash_redis-0.14.5/PKG-INFO
```

### Comparing `upstash_redis-0.14.4/LICENSE` & `upstash_redis-0.14.5/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.4/upstash_redis/asyncio/client.py` & `upstash_redis-0.14.5/upstash_redis/asyncio/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from os import environ
 from typing import Any, List, Type, Union
 
 from aiohttp import ClientSession
+
 from upstash_redis.commands.async_commands import AsyncCommands
 from upstash_redis.config import (
+    ALLOW_TELEMETRY,
+    FORMAT_RETURN,
     REST_ENCODING,
     REST_RETRIES,
     REST_RETRY_INTERVAL,
-    FORMAT_RETURN,
-    ALLOW_TELEMETRY,
 )
-from upstash_redis.http.execute import async_execute
-
+from upstash_redis.http import async_execute, make_headers
 from upstash_redis.schema.http import RESTEncoding, RESTResult
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.utils.format import FormattedResponse
 
 
 class Redis(FormattedResponse, AsyncCommands):
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,  # Seconds.
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
-        telemetry_data: Union[TelemetryData, None] = None,
     ):
         """
         :param url: UPSTASH_REDIS_REST_URL in the console
         :param token: UPSTASH_REDIS_REST_TOKEN in the console
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
@@ -46,26 +44,26 @@
 
         self.format_return = format_return
 
         self.rest_encoding = rest_encoding
         self.rest_retries = rest_retries
         self.rest_retry_interval = rest_retry_interval
 
-        self.telemetry_data = telemetry_data
         self.FORMATTERS = self.__class__.FORMATTERS
 
+        self._headers = make_headers(token, rest_encoding, allow_telemetry)
+
     @classmethod
     def from_env(
         cls,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
-        telemetry_data: Union[TelemetryData, None] = None,
     ):
         """
         Load the credentials from environment.
 
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
@@ -77,15 +75,14 @@
             environ["UPSTASH_REDIS_REST_URL"],
             environ["UPSTASH_REDIS_REST_TOKEN"],
             rest_encoding,
             rest_retries,
             rest_retry_interval,
             format_return,
             allow_telemetry,
-            telemetry_data,
         )
 
     async def __aenter__(self) -> ClientSession:
         """
         Enter the async context.
         """
 
@@ -109,21 +106,19 @@
         """
         Specify the http options and execute the command.
         """
 
         res = await async_execute(
             session=self._session,
             url=self.url,
-            token=self.token,
+            headers=self._headers,
             encoding=self.rest_encoding,
             retries=self.rest_retries,
             retry_interval=self.rest_retry_interval,
             command=command,
-            allow_telemetry=self.allow_telemetry,
-            telemetry_data=self.telemetry_data,
         )
 
         main_command = command[0]
         if len(command) > 1 and (main_command == "PUBSUB" or main_command == "SCRIPT"):
             main_command = f"{main_command} {command[1]}"
 
         if (
```

### Comparing `upstash_redis-0.14.4/upstash_redis/client.py` & `upstash_redis-0.14.5/upstash_redis/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 from os import environ
 from typing import Any, List, Type, Union
 
-from aiohttp import ClientSession
+from requests import Session
+
 from upstash_redis.commands.commands import Commands
 from upstash_redis.config import (
+    ALLOW_TELEMETRY,
+    FORMAT_RETURN,
     REST_ENCODING,
     REST_RETRIES,
     REST_RETRY_INTERVAL,
-    FORMAT_RETURN,
-    ALLOW_TELEMETRY,
 )
-from upstash_redis.http.execute import sync_execute
-
+from upstash_redis.http import make_headers, sync_execute
 from upstash_redis.schema.http import RESTEncoding, RESTResult
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.utils.format import FormattedResponse
-from requests import Session
 
 
 class Redis(FormattedResponse, Commands):
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,  # Seconds.
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
-        telemetry_data: Union[TelemetryData, None] = None,
     ):
         """
         :param url: UPSTASH_REDIS_REST_URL in the console
         :param token: UPSTASH_REDIS_REST_TOKEN in the console
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
@@ -47,17 +44,17 @@
 
         self.format_return = format_return
 
         self.rest_encoding = rest_encoding
         self.rest_retries = rest_retries
         self.rest_retry_interval = rest_retry_interval
 
-        self.telemetry_data = telemetry_data
         self.FORMATTERS = self.__class__.FORMATTERS
 
+        self._headers = make_headers(token, rest_encoding, allow_telemetry)
         self._session = Session()
 
     def __enter__(self):
         """
         Enter the sync context.
         """
         if self._session is None:
@@ -82,15 +79,14 @@
     def from_env(
         cls,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
         rest_retry_interval: int = REST_RETRY_INTERVAL,
         format_return: bool = FORMAT_RETURN,
         allow_telemetry: bool = ALLOW_TELEMETRY,
-        telemetry_data: Union[TelemetryData, None] = None,
     ):
         """
         Load the credentials from environment.
 
         :param rest_encoding: the encoding that can be used by the REST API to parse the response before sending it
         :param rest_retries: how many times an HTTP request will be retried if it fails
         :param rest_retry_interval: how many seconds will be waited between each retry
@@ -102,15 +98,14 @@
             environ["UPSTASH_REDIS_REST_URL"],
             environ["UPSTASH_REDIS_REST_TOKEN"],
             rest_encoding,
             rest_retries,
             rest_retry_interval,
             format_return,
             allow_telemetry,
-            telemetry_data,
         )
 
     def close(self):
         """
         Closes the session.
         """
         if self._session:
@@ -120,21 +115,19 @@
         """
         Specify the http options and execute the command.
         """
 
         res = sync_execute(
             session=self._session,
             url=self.url,
-            token=self.token,
+            headers=self._headers,
             encoding=self.rest_encoding,
             retries=self.rest_retries,
             retry_interval=self.rest_retry_interval,
             command=command,
-            allow_telemetry=self.allow_telemetry,
-            telemetry_data=self.telemetry_data,
         )
 
         main_command = command[0]
         if len(command) > 1 and (main_command == "PUBSUB" or main_command == "SCRIPT"):
             main_command = f"{main_command} {command[1]}"
 
         if (
```

### Comparing `upstash_redis-0.14.4/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.14.5/upstash_redis/commands/async_commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.4/upstash_redis/commands/commands.py` & `upstash_redis-0.14.5/upstash_redis/commands/commands.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.4/upstash_redis/commands/commands.pyi` & `upstash_redis-0.14.5/upstash_redis/commands/commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.4/upstash_redis/schema/http.py` & `upstash_redis-0.14.5/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.4/upstash_redis/utils/exception.py` & `upstash_redis-0.14.5/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.14.4/upstash_redis/utils/format.py` & `upstash_redis-0.14.5/upstash_redis/utils/format.py`

 * *Files identical despite different names*

