# Comparing `tmp/tritonv2-0.9.6.tar.gz` & `tmp/tritonv2-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritonv2-0.9.6.tar", last modified: Thu May 18 07:24:38 2023, max compression
+gzip compressed data, was "tritonv2-0.9.7.tar", last modified: Mon Jul  3 19:08:25 2023, max compression
```

## Comparing `tritonv2-0.9.6.tar` & `tritonv2-0.9.7.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-18 07:24:38.114636 tritonv2-0.9.6/
--rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-05-18 07:24:38.114712 tritonv2-0.9.6/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1882 2023-05-18 07:24:37.000000 tritonv2-0.9.6/README.md
--rw-r--r--   0 jojo       (501) staff       (20)      763 2023-05-18 07:24:38.115101 tritonv2-0.9.6/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-05-18 07:24:37.000000 tritonv2-0.9.6/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-18 07:24:38.113601 tritonv2-0.9.6/tritonv2/
--rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.6/tritonv2/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-05-17 18:28:29.000000 tritonv2-0.9.6/tritonv2/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-05-17 18:34:37.000000 tritonv2-0.9.6/tritonv2/client_factory.py
--rw-r--r--   0 jojo       (501) staff       (20)     1246 2023-05-17 20:16:45.000000 tritonv2-0.9.6/tritonv2/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.6/tritonv2/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)    16981 2023-05-17 20:12:01.000000 tritonv2-0.9.6/tritonv2/grpc_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    14354 2023-05-18 07:24:08.000000 tritonv2-0.9.6/tritonv2/grpc_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-05-17 19:53:45.000000 tritonv2-0.9.6/tritonv2/grpc_interceptor.py
--rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-05-17 18:27:25.000000 tritonv2-0.9.6/tritonv2/http_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-05-17 18:28:44.000000 tritonv2-0.9.6/tritonv2/http_client.py
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.6/tritonv2/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     1238 2023-05-18 06:48:12.000000 tritonv2-0.9.6/tritonv2/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-05-18 07:24:38.114510 tritonv2-0.9.6/tritonv2.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-05-18 07:24:38.000000 tritonv2-0.9.6/tritonv2.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      499 2023-05-18 07:24:38.000000 tritonv2-0.9.6/tritonv2.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-18 07:24:38.000000 tritonv2-0.9.6/tritonv2.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-05-18 07:24:38.000000 tritonv2-0.9.6/tritonv2.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)      121 2023-05-18 07:24:38.000000 tritonv2-0.9.6/tritonv2.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        9 2023-05-18 07:24:38.000000 tritonv2-0.9.6/tritonv2.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-03 19:08:25.465580 tritonv2-0.9.7/
+-rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-07-03 19:08:25.465683 tritonv2-0.9.7/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1882 2023-07-03 19:08:24.000000 tritonv2-0.9.7/README.md
+-rw-r--r--   0 jojo       (501) staff       (20)      770 2023-07-03 19:08:25.466145 tritonv2-0.9.7/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-03 19:08:24.000000 tritonv2-0.9.7/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-03 19:08:25.464556 tritonv2-0.9.7/tritonv2/
+-rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.7/tritonv2/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.7/tritonv2/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.7/tritonv2/client_factory.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.7/tritonv2/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.7/tritonv2/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.7/tritonv2/grpc_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.7/tritonv2/grpc_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.7/tritonv2/grpc_interceptor.py
+-rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-06-06 13:39:44.000000 tritonv2-0.9.7/tritonv2/http_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-06-06 13:39:44.000000 tritonv2-0.9.7/tritonv2/http_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7081 2023-07-03 19:07:54.000000 tritonv2-0.9.7/tritonv2/model.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4099 2023-07-03 19:07:52.000000 tritonv2-0.9.7/tritonv2/model_config.py
+-rw-r--r--   0 jojo       (501) staff       (20)      950 2023-07-03 18:55:46.000000 tritonv2-0.9.7/tritonv2/module.py
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.7/tritonv2/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4893 2023-07-03 19:07:51.000000 tritonv2-0.9.7/tritonv2/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-03 19:08:25.465453 tritonv2-0.9.7/tritonv2.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)     2406 2023-07-03 19:08:25.000000 tritonv2-0.9.7/tritonv2.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-03 19:08:25.000000 tritonv2-0.9.7/tritonv2.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-03 19:08:25.000000 tritonv2-0.9.7/tritonv2.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-03 19:08:25.000000 tritonv2-0.9.7/tritonv2.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-03 19:08:25.000000 tritonv2-0.9.7/tritonv2.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-03 19:08:25.000000 tritonv2-0.9.7/tritonv2.egg-info/top_level.txt
```

### Comparing `tritonv2-0.9.6/PKG-INFO` & `tritonv2-0.9.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.6
+Version: 0.9.7
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.6
+pip install tritonv2==0.9.7
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.6/README.md` & `tritonv2-0.9.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.6
+pip install tritonv2==0.9.7
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.6/setup.cfg` & `tritonv2-0.9.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = tritonv2
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.9.6
+version = 0.9.7
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
@@ -20,14 +20,15 @@
 install_requires = 
 	numpy>=1.23.5
 	tenacity>=8.1.0
 	tritonclient[all]>=2.25.0
 	pydantic>=1.10.2
 	pyrate-limiter>=2.10.0
 	grpc-interceptor>=0.15.1
+	boto3
 python_requires = >=3.7
 include_package_data = True
 zip_safe = False
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tritonv2-0.9.6/tritonv2/client.py` & `tritonv2-0.9.7/tritonv2/client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.6/tritonv2/client_factory.py` & `tritonv2-0.9.7/tritonv2/client_factory.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.6/tritonv2/constants.py` & `tritonv2-0.9.7/tritonv2/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 """
 from __future__ import annotations
 from typing import List
 from pydantic import BaseModel
 
 GRPC_SERVICE = "inference.GRPCInferenceService"
 
+BENCHMARK_TASK = "benchmark"
+TESTING_TASK = "testing"
 
 class LimiterConfig(BaseModel):
     # ratelimit limit, the max request number per interval
     limit: int
     # ratelimit interval, with units as RequestRateDuration
     interval: int
     # ratelimit delay, if delay is True, the request will be delayed until the ratelimit is passed
```

### Comparing `tritonv2-0.9.6/tritonv2/grpc_aio_client.py` & `tritonv2-0.9.7/tritonv2/grpc_aio_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,23 +71,24 @@
             private_key=private_key,
             certificate_chain=certificate_chain,
             creds=creds,
             keepalive_options=keepalive_options,
             channel_args=channel_args,
         )
 
-        self._client._channel = grpc.aio.insecure_channel(server_url, options=channel_args, interceptors=[async_rate_limit_interceptor(
-            self._identifier,
-            self._limiter,
-            self._limiter_delay,
-            self._limiter_max_delay,
-        )])
+        if limiter_config is not None:
+            self._client._channel = grpc.aio.insecure_channel(server_url, options=channel_args, interceptors=[async_rate_limit_interceptor(
+                self._identifier,
+                self._limiter,
+                self._limiter_delay,
+                self._limiter_max_delay,
+            )])
 
-        self._client._client_stub = service_pb2_grpc.GRPCInferenceServiceStub(
-            self._client._channel)
+            self._client._client_stub = service_pb2_grpc.GRPCInferenceServiceStub(
+                self._client._channel)
 
     async def close(self):
         """
         Close the client
         :return:
         """
         await self._client.close()
```

### Comparing `tritonv2-0.9.6/tritonv2/grpc_client.py` & `tritonv2-0.9.7/tritonv2/grpc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,23 +70,23 @@
             root_certificates=root_certificates,
             private_key=private_key,
             certificate_chain=certificate_chain,
             creds=creds,
             keepalive_options=keepalive_options,
             channel_args=channel_args,
         )
-
-        self._client._channel = grpc.intercept_channel(self._client._channel, *[rate_limit_interceptor(
-            self._identifier,
-            self._limiter,
-            self._limiter_delay,
-            self._limiter_max_delay,
-        )])
-        self._client._client_stub = service_pb2_grpc.GRPCInferenceServiceStub(
-            self._client._channel)
+        if limiter_config is not None:
+            self._client._channel = grpc.intercept_channel(self._client._channel, *[rate_limit_interceptor(
+                self._identifier,
+                self._limiter,
+                self._limiter_delay,
+                self._limiter_max_delay,
+            )])
+            self._client._client_stub = service_pb2_grpc.GRPCInferenceServiceStub(
+                self._client._channel)
 
     def model_infer(self,
                     model_name,
                     inputs,
                     model_version="",
                     outputs=None,
                     request_id="",
```

### Comparing `tritonv2-0.9.6/tritonv2/grpc_interceptor.py` & `tritonv2-0.9.7/tritonv2/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.6/tritonv2/http_aio_client.py` & `tritonv2-0.9.7/tritonv2/http_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.6/tritonv2/http_client.py` & `tritonv2-0.9.7/tritonv2/http_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.6/tritonv2.egg-info/PKG-INFO` & `tritonv2-0.9.7/tritonv2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.6
+Version: 0.9.7
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.6
+pip install tritonv2==0.9.7
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

