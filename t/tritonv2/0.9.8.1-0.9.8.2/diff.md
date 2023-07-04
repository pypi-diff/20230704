# Comparing `tmp/tritonv2-0.9.8.1.tar.gz` & `tmp/tritonv2-0.9.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritonv2-0.9.8.1.tar", last modified: Tue Jul  4 17:56:27 2023, max compression
+gzip compressed data, was "tritonv2-0.9.8.2.tar", last modified: Tue Jul  4 17:57:37 2023, max compression
```

## Comparing `tritonv2-0.9.8.1.tar` & `tritonv2-0.9.8.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 17:56:27.472437 tritonv2-0.9.8.1/
--rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-04 17:56:27.472535 tritonv2-0.9.8.1/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1884 2023-07-04 17:56:26.000000 tritonv2-0.9.8.1/README.md
--rw-r--r--   0 jojo       (501) staff       (20)      772 2023-07-04 17:56:27.472966 tritonv2-0.9.8.1/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-04 17:56:26.000000 tritonv2-0.9.8.1/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 17:56:27.471307 tritonv2-0.9.8.1/tritonv2/
--rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.8.1/tritonv2/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.8.1/tritonv2/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.8.1/tritonv2/client_factory.py
--rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.8.1/tritonv2/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.8.1/tritonv2/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.8.1/tritonv2/grpc_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.8.1/tritonv2/grpc_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.8.1/tritonv2/grpc_interceptor.py
--rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-06-06 13:39:44.000000 tritonv2-0.9.8.1/tritonv2/http_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-06-06 13:39:44.000000 tritonv2-0.9.8.1/tritonv2/http_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     7576 2023-07-04 17:55:53.000000 tritonv2-0.9.8.1/tritonv2/model.py
--rw-r--r--   0 jojo       (501) staff       (20)     4099 2023-07-04 11:53:35.000000 tritonv2-0.9.8.1/tritonv2/model_config.py
--rw-r--r--   0 jojo       (501) staff       (20)      903 2023-07-04 11:53:39.000000 tritonv2-0.9.8.1/tritonv2/module.py
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.8.1/tritonv2/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     4893 2023-07-03 19:07:51.000000 tritonv2-0.9.8.1/tritonv2/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 17:56:27.472323 tritonv2-0.9.8.1/tritonv2.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-04 17:56:27.000000 tritonv2-0.9.8.1/tritonv2.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-04 17:56:27.000000 tritonv2-0.9.8.1/tritonv2.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-04 17:56:27.000000 tritonv2-0.9.8.1/tritonv2.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-04 17:56:27.000000 tritonv2-0.9.8.1/tritonv2.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-04 17:56:27.000000 tritonv2-0.9.8.1/tritonv2.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-04 17:56:27.000000 tritonv2-0.9.8.1/tritonv2.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 17:57:37.197351 tritonv2-0.9.8.2/
+-rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-04 17:57:37.197467 tritonv2-0.9.8.2/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1884 2023-07-04 17:57:36.000000 tritonv2-0.9.8.2/README.md
+-rw-r--r--   0 jojo       (501) staff       (20)      772 2023-07-04 17:57:37.197935 tritonv2-0.9.8.2/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-04 17:57:36.000000 tritonv2-0.9.8.2/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 17:57:37.196193 tritonv2-0.9.8.2/tritonv2/
+-rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.8.2/tritonv2/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.8.2/tritonv2/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.8.2/tritonv2/client_factory.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.8.2/tritonv2/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.8.2/tritonv2/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.8.2/tritonv2/grpc_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.8.2/tritonv2/grpc_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.8.2/tritonv2/grpc_interceptor.py
+-rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-06-06 13:39:44.000000 tritonv2-0.9.8.2/tritonv2/http_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-06-06 13:39:44.000000 tritonv2-0.9.8.2/tritonv2/http_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7581 2023-07-04 17:57:18.000000 tritonv2-0.9.8.2/tritonv2/model.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4099 2023-07-04 11:53:35.000000 tritonv2-0.9.8.2/tritonv2/model_config.py
+-rw-r--r--   0 jojo       (501) staff       (20)      903 2023-07-04 11:53:39.000000 tritonv2-0.9.8.2/tritonv2/module.py
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.8.2/tritonv2/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4893 2023-07-03 19:07:51.000000 tritonv2-0.9.8.2/tritonv2/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 17:57:37.197208 tritonv2-0.9.8.2/tritonv2.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-04 17:57:37.000000 tritonv2-0.9.8.2/tritonv2.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-04 17:57:37.000000 tritonv2-0.9.8.2/tritonv2.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-04 17:57:37.000000 tritonv2-0.9.8.2/tritonv2.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-04 17:57:37.000000 tritonv2-0.9.8.2/tritonv2.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-04 17:57:37.000000 tritonv2-0.9.8.2/tritonv2.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-04 17:57:37.000000 tritonv2-0.9.8.2/tritonv2.egg-info/top_level.txt
```

### Comparing `tritonv2-0.9.8.1/PKG-INFO` & `tritonv2-0.9.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.8.1
+Version: 0.9.8.2
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
-pip install tritonv2==0.9.8.1
+pip install tritonv2==0.9.8.2
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.8.1/README.md` & `tritonv2-0.9.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.8.1
+pip install tritonv2==0.9.8.2
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.8.1/setup.cfg` & `tritonv2-0.9.8.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = tritonv2
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.9.8.1
+version = 0.9.8.2
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

### Comparing `tritonv2-0.9.8.1/tritonv2/client.py` & `tritonv2-0.9.8.2/tritonv2/client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/client_factory.py` & `tritonv2-0.9.8.2/tritonv2/client_factory.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/constants.py` & `tritonv2-0.9.8.2/tritonv2/constants.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/grpc_aio_client.py` & `tritonv2-0.9.8.2/tritonv2/grpc_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/grpc_client.py` & `tritonv2-0.9.8.2/tritonv2/grpc_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/grpc_interceptor.py` & `tritonv2-0.9.8.2/tritonv2/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/http_aio_client.py` & `tritonv2-0.9.8.2/tritonv2/http_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/http_client.py` & `tritonv2-0.9.8.2/tritonv2/http_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/model.py` & `tritonv2-0.9.8.2/tritonv2/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                                                             sequence_id=None,
                                                             sequence_start=None,
                                                             sequence_end=None,
                                                             priority=None,
                                                             timeout=None,
                                                             custom_parameters=None)
             if json_size is not None:
-                return self._save_binary_perf_request(model_inputs)
+                return self._save_binary_benchmark_request(model_inputs)
 
             request_body_list.append(request_body)
             
         result = {'data': []}
         
         for k, body in enumerate(request_body_list):
             infer_req = json.loads(body)
```

### Comparing `tritonv2-0.9.8.1/tritonv2/model_config.py` & `tritonv2-0.9.8.2/tritonv2/model_config.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/module.py` & `tritonv2-0.9.8.2/tritonv2/module.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2/utils.py` & `tritonv2-0.9.8.2/tritonv2/utils.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.8.1/tritonv2.egg-info/PKG-INFO` & `tritonv2-0.9.8.2/tritonv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.8.1
+Version: 0.9.8.2
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
-pip install tritonv2==0.9.8.1
+pip install tritonv2==0.9.8.2
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.8.1/tritonv2.egg-info/SOURCES.txt` & `tritonv2-0.9.8.2/tritonv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

