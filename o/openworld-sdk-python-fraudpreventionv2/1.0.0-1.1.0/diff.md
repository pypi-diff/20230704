# Comparing `tmp/openworld-sdk-python-fraudpreventionv2-1.0.0.tar.gz` & `tmp/openworld-sdk-python-fraudpreventionv2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.0.0.tar", last modified: Tue Jun 20 14:50:48 2023, max compression
+gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.1.0.tar", last modified: Tue Jul  4 14:18:44 2023, max compression
```

## Comparing `openworld-sdk-python-fraudpreventionv2-1.0.0.tar` & `openworld-sdk-python-fraudpreventionv2-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:50:48.255576 openworld-sdk-python-fraudpreventionv2-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 14:50:48.255576 openworld-sdk-python-fraudpreventionv2-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:50:48.251576 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:50:48.251576 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:50:48.251576 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/fraudpreventionv2/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-20 14:50:40.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/fraudpreventionv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-06-20 14:50:40.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/fraudpreventionv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89271 2023-06-20 14:50:40.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/fraudpreventionv2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:50:48.255576 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld_sdk_python_fraudpreventionv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 14:50:48.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-20 14:50:48.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:50:48.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-20 14:50:48.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 14:50:48.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:50:48.255576 openworld-sdk-python-fraudpreventionv2-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-20 14:50:28.000000 openworld-sdk-python-fraudpreventionv2-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.367976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.367976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.367976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-04 14:18:35.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-04 14:18:35.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89421 2023-07-04 14:18:35.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-04 14:18:20.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/setup.py
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.0.0/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.0.0
-Summary: Open World Fraud Prevention V2 SDK for Python
+Version: 1.1.0
+Summary: Open World fraudPreventionV2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 
-Open World Fraud Prevention V2 SDK for Python
+Open World fraudPreventionV2 SDK for Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/fraudpreventionv2/__init__.py` & `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/fraudpreventionv2/client.py` & `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 from openworld.sdk.core.client.openworld_auth_client import _OpenWorldAuthClient
 from openworld.sdk.core.configuration.client_config import ClientConfig
 from openworld.sdk.core.constant import header
 
 from .model import *
 
 
-class FraudPreventionV2Client:
+class Fraudpreventionv2Client:
     def __init__(self, client_config: ClientConfig):
-        r"""Fraud Prevention V2 API Client.
+        r"""fraudPreventionV2 API Client.
 
         Args:
             client_config(ClientConfig): SDK Client Configurations Holder.
         """
         python_version = platform.python_version()
         os_name, os_version, *_ = platform.platform().split('-')
-        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.0.0'
+        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.1.0'
 
         self.__api_client = ApiClient(client_config, _OpenWorldAuthClient)
 
         self.__user_agent = f'{sdk_metadata} (Python {python_version}; {os_name} {os_version})'
 
     def screen(
         self, transaction_id: UUID = uuid4(), body: OrderPurchaseScreenRequest = None
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.0.0/openworld/sdk/fraudpreventionv2/model.py` & `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,26 +30,28 @@
         FORBIDDEN(Any): --
         NOT_FOUND(Any): --
         ORDER_PURCHASE_UPDATE_NOT_FOUND(Any): --
         TOO_MANY_REQUESTS(Any): --
         INTERNAL_SERVER_ERROR(Any): --
         BAD_GATEWAY(Any): --
         RETRYABLE_ORDER_PURCHASE_SCREEN_FAILURE(Any): --
+        RETRYABLE_ORDER_PURCHASE_UPDATE_FAILURE(Any): --
         GATEWAY_TIMEOUT(Any): --
         BAD_REQUEST(Any): --
 
     """
     UNAUTHORIZED: Any = 'UNAUTHORIZED'
     FORBIDDEN: Any = 'FORBIDDEN'
     NOT_FOUND: Any = 'NOT_FOUND'
     ORDER_PURCHASE_UPDATE_NOT_FOUND: Any = 'ORDER_PURCHASE_UPDATE_NOT_FOUND'
     TOO_MANY_REQUESTS: Any = 'TOO_MANY_REQUESTS'
     INTERNAL_SERVER_ERROR: Any = 'INTERNAL_SERVER_ERROR'
     BAD_GATEWAY: Any = 'BAD_GATEWAY'
     RETRYABLE_ORDER_PURCHASE_SCREEN_FAILURE: Any = 'RETRYABLE_ORDER_PURCHASE_SCREEN_FAILURE'
+    RETRYABLE_ORDER_PURCHASE_UPDATE_FAILURE: Any = 'RETRYABLE_ORDER_PURCHASE_UPDATE_FAILURE'
     GATEWAY_TIMEOUT: Any = 'GATEWAY_TIMEOUT'
     BAD_REQUEST: Any = 'BAD_REQUEST'
 
 
 class Error(
     BaseModel,
     smart_union=True,
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.0.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.0.0
-Summary: Open World Fraud Prevention V2 SDK for Python
+Version: 1.1.0
+Summary: Open World fraudPreventionV2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 
-Open World Fraud Prevention V2 SDK for Python
+Open World fraudPreventionV2 SDK for Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.0.0/setup.py` & `openworld-sdk-python-fraudpreventionv2-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from setuptools import setup
 
 setup(
     name='openworld-sdk-python-fraudpreventionv2',
-    version='1.0.0',
+    version='1.1.0',
     packages=['openworld.sdk.fraudpreventionv2'],
     package_dir={'openworld-sdk-python-fraudpreventionv2': '.'},
     license='Apache License, Version 2.0',
     author='Expedia Group',
     author_email='oss@expediagroup.com',
     url='https://github.com/ExpediaGroup/openworld-sdk-python',
     classifiers=[
@@ -33,10 +33,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires='>=3.8',
     install_requires=['uri', 'furl', 'openworld-sdk-python-core', 'pydantic', 'pydantic[email]', 'email-validator'],
-    description='Open World Fraud Prevention V2 SDK for Python',
-    long_description='Open World Fraud Prevention V2 SDK for Python',
+    description='Open World fraudPreventionV2 SDK for Python',
+    long_description='Open World fraudPreventionV2 SDK for Python',
 )
```

