# Comparing `tmp/burla-0.0.4.tar.gz` & `tmp/burla-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.0.4.tar", max compression
+gzip compressed data, was "burla-0.0.5.tar", max compression
```

## Comparing `burla-0.0.4.tar` & `burla-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      465 2023-07-03 16:18:11.418173 burla-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      192 2023-07-01 19:19:54.254412 burla-0.0.4/src/burla/__init__.py
--rw-r--r--   0        0        0     1364 2023-07-03 01:37:32.807846 burla-0.0.4/src/burla/_logstream.py
--rw-r--r--   0        0        0      914 2023-07-01 19:18:36.678628 burla-0.0.4/src/burla/config.py
--rw-r--r--   0        0        0     3707 2023-07-03 16:17:59.943480 burla-0.0.4/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 burla-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      486 2023-07-04 19:11:58.812772 burla-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-07-01 19:19:54.254412 burla-0.0.5/src/burla/__init__.py
+-rw-r--r--   0        0        0     1364 2023-07-03 01:37:32.807846 burla-0.0.5/src/burla/_logstream.py
+-rw-r--r--   0        0        0      914 2023-07-01 19:18:36.678628 burla-0.0.5/src/burla/config.py
+-rw-r--r--   0        0        0     3921 2023-07-04 19:07:41.736595 burla-0.0.5/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 burla-0.0.5/PKG-INFO
```

### Comparing `burla-0.0.4/src/burla/_logstream.py` & `burla-0.0.5/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.4/src/burla/config.py` & `burla-0.0.5/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.4/src/burla/remote_parallel_map.py` & `burla-0.0.5/src/burla/remote_parallel_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import sys
 import requests
 import threading
 import warnings
+from binascii import hexlify
 from datetime import datetime, timezone
-from typing import Callable
+from typing import Callable, Optional
 from time import sleep, time
 from queue import PriorityQueue
 
-import binascii
 import dill
 
 from burla._logstream import print_logs_from_queue
 from burla.config import load_api_key_from_local_config
 
 BURLA_SERVICE_URL = "https://burla-webservice-gxc7eo4ala-uc.a.run.app"
+JOB_ENV_REPO = "us-east4-docker.pkg.dev/burla-389321/burla-job-environments"
 
 # BURLA_SERVICE_URL = "https://127.0.0.1:5000"
 
 TZ = timezone.utc
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
@@ -45,34 +47,36 @@
             raise e
 
 
 def remote_parallel_map(
     function_: Callable,
     inputs: list,
     cpus: int = 0,
-    image: str = "us-east4-docker.pkg.dev/burla-389321/burla-images/burla:1",
-    api_key: str = None,
+    image: Optional[str] = None,
+    api_key: Optional[str] = None,
 ):
     if not function_.__annotations__.get("return") is str:
         raise AttributeError("Please add the return type annotation 'str' to your input function.")
 
     if cpus > 100:
         raise AttributeError("Currently unable to satisfy requests for >100 computers")
 
     api_key = api_key or load_api_key_from_local_config()
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={"key": api_key})
     response.raise_for_status()
     job_id = response.json()["job_id"]
 
-    func_pkl_hex_ascii = binascii.hexlify(dill.dumps(function_.__code__)).decode("ascii")
+    user_python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
+    default_docker_image = f"{JOB_ENV_REPO}/python{user_python_version}/burla_job_env"
+
     data = {
         "key": api_key,
-        "func_pkl_hex_ascii": func_pkl_hex_ascii,
+        "func_pkl_hex_ascii": hexlify(dill.dumps(function_.__code__)).decode("ascii"),
         "inputs": inputs,
-        "image": image,
+        "image": image or default_docker_image,
         "num_computers": cpus,
     }
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data)
     response.raise_for_status()
 
     job_start_time = time()
     last_timestamp = "2023-07-01T00:00:00.000001Z"
```

### Comparing `burla-0.0.4/PKG-INFO` & `burla-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.0.4
+Version: 0.0.5
 Summary: Make your python script 100x faster
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

