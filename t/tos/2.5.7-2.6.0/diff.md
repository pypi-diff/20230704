# Comparing `tmp/tos-2.5.7.tar.gz` & `tmp/tos-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tos-2.5.7.tar", last modified: Thu Mar  9 06:22:24 2023, max compression
+gzip compressed data, was "dist/tos-2.6.0.tar", last modified: Tue Jul  4 03:28:22 2023, max compression
```

## Comparing `tos-2.5.7.tar` & `tos-2.6.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-03-09 06:22:24.065270 tos-2.5.7/
--rw-r--r--   0 bytedance   (501) staff       (20)    29979 2022-07-29 04:55:38.000000 tos-2.5.7/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)     2760 2023-03-09 06:22:24.064735 tos-2.5.7/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     2149 2022-11-30 10:26:39.000000 tos-2.5.7/README.md
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-03-09 06:22:24.065403 tos-2.5.7/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     1755 2022-11-10 15:09:21.000000 tos-2.5.7/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-03-09 06:22:24.061137 tos-2.5.7/tos/
--rw-r--r--   0 bytedance   (501) staff       (20)      759 2022-11-06 07:08:17.000000 tos-2.5.7/tos/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)       23 2023-03-09 02:52:35.000000 tos-2.5.7/tos/__version__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9777 2022-11-14 03:38:33.000000 tos-2.5.7/tos/auth.py
--rw-r--r--   0 bytedance   (501) staff       (20)    24690 2023-02-13 03:39:32.000000 tos-2.5.7/tos/checkpoint.py
--rw-r--r--   0 bytedance   (501) staff       (20)    47182 2022-12-07 15:36:15.000000 tos-2.5.7/tos/client.py
--rw-r--r--   0 bytedance   (501) staff       (20)   162378 2023-03-09 02:47:28.000000 tos-2.5.7/tos/clientv2.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1555 2023-02-13 03:39:32.000000 tos-2.5.7/tos/consts.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11459 2023-02-13 03:39:32.000000 tos-2.5.7/tos/convertor.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3098 2022-09-16 02:25:03.000000 tos-2.5.7/tos/credential.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5917 2023-02-13 03:39:32.000000 tos-2.5.7/tos/enum.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3348 2022-11-21 04:14:10.000000 tos-2.5.7/tos/exceptions.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2327 2022-11-07 02:31:37.000000 tos-2.5.7/tos/http.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15196 2023-02-13 03:39:32.000000 tos-2.5.7/tos/json_utils.py
--rw-r--r--   0 bytedance   (501) staff       (20)      111 2022-08-03 09:17:31.000000 tos-2.5.7/tos/log.py
--rw-r--r--   0 bytedance   (501) staff       (20)    20455 2022-07-29 04:55:38.000000 tos-2.5.7/tos/mine_type.py
--rw-r--r--   0 bytedance   (501) staff       (20)    10701 2022-07-29 04:55:38.000000 tos-2.5.7/tos/models.py
--rw-r--r--   0 bytedance   (501) staff       (20)    65317 2023-02-13 03:39:32.000000 tos-2.5.7/tos/models2.py
--rw-r--r--   0 bytedance   (501) staff       (20)    37789 2023-02-13 03:39:32.000000 tos-2.5.7/tos/utils.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-03-09 06:22:24.063991 tos-2.5.7/tos.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)     2760 2023-03-09 06:22:23.000000 tos-2.5.7/tos.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      434 2023-03-09 06:22:23.000000 tos-2.5.7/tos.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-03-09 06:22:23.000000 tos-2.5.7/tos.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       72 2023-03-09 06:22:23.000000 tos-2.5.7/tos.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        4 2023-03-09 06:22:23.000000 tos-2.5.7/tos.egg-info/top_level.txt
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-04 03:28:22.000000 tos-2.6.0/
+-rw-r--r--   0 bytedance   (502) staff       (20)     3373 2023-07-04 03:28:22.000000 tos-2.6.0/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)     2149 2023-07-04 03:26:55.000000 tos-2.6.0/README.md
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/
+-rw-r--r--   0 bytedance   (502) staff       (20)     3373 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (502) staff       (20)      426 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)       70 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        4 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-04 03:28:22.000000 tos-2.6.0/tos.egg-info/dependency_links.txt
+drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-04 03:28:22.000000 tos-2.6.0/tos/
+-rw-r--r--   0 bytedance   (502) staff       (20)    11053 2023-07-04 03:26:55.000000 tos-2.6.0/tos/auth.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    71060 2023-07-04 03:26:55.000000 tos-2.6.0/tos/models2.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    20455 2022-04-26 02:50:40.000000 tos-2.6.0/tos/mine_type.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    25991 2023-07-04 03:26:55.000000 tos-2.6.0/tos/checkpoint.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    10701 2023-07-04 03:26:55.000000 tos-2.6.0/tos/models.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      111 2023-07-04 03:26:55.000000 tos-2.6.0/tos/log.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    47212 2023-07-04 03:26:55.000000 tos-2.6.0/tos/client.py
+-rw-r--r--   0 bytedance   (502) staff       (20)      759 2023-07-04 03:26:55.000000 tos-2.6.0/tos/__init__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)       23 2023-07-04 03:26:55.000000 tos-2.6.0/tos/__version__.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     1780 2023-07-04 03:26:55.000000 tos-2.6.0/tos/consts.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    37822 2023-07-04 03:26:55.000000 tos-2.6.0/tos/utils.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     2327 2023-07-04 03:26:55.000000 tos-2.6.0/tos/http.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    11459 2023-07-04 03:26:55.000000 tos-2.6.0/tos/convertor.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3348 2023-07-04 03:26:55.000000 tos-2.6.0/tos/exceptions.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     6381 2023-07-04 03:26:55.000000 tos-2.6.0/tos/enum.py
+-rw-r--r--   0 bytedance   (502) staff       (20)   170603 2023-07-04 03:26:55.000000 tos-2.6.0/tos/clientv2.py
+-rw-r--r--   0 bytedance   (502) staff       (20)    18069 2023-07-04 03:26:55.000000 tos-2.6.0/tos/json_utils.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     3098 2023-07-04 03:26:55.000000 tos-2.6.0/tos/credential.py
+-rw-r--r--   0 bytedance   (502) staff       (20)     1754 2023-07-04 03:26:55.000000 tos-2.6.0/setup.py
+-rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-07-04 03:28:22.000000 tos-2.6.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tos-2.5.7/PKG-INFO` & `tos-2.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: tos
-Version: 2.5.7
-Summary: Volc TOS (Tinder Object Storage) SDK
-Home-page: https://www.volcengine.com/
-Author: sunyushan
-Author-email: sunyushan.jason@bytedance.com
-License: UNKNOWN
-Keywords: boilerplate
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # Volcengine TOS SDK for Python
 The TOS Python SDK enables Python developers to easily work with TOS(Tinder Object Storage) service in the volcengine.
 This document will show developers some basic examples about TOS bucket and object operation.
 
 
 ## Install
 ### Requirements
@@ -91,9 +71,8 @@
 assert resp.status_code == 200   
 # call delete_object to delete an object in your bucket
 resp = client.delete_object(bucket_name, key_name)
 assert resp.status_code == 204
 ```
 
 ## License
-[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html)
-
+[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html)
```

### Comparing `tos-2.5.7/README.md` & `tos-2.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,96 @@
-# Volcengine TOS SDK for Python
-The TOS Python SDK enables Python developers to easily work with TOS(Tinder Object Storage) service in the volcengine.
-This document will show developers some basic examples about TOS bucket and object operation.
-
-
-## Install
-### Requirements
-- Python3
-# Quick Start
-
-This section introduces how to create a bucket, upload/download/delete an object in TOS service through our SDK.
-
-## Create a TOS Client
-
-You can interact with TOS service after initiating a TOSClient instance.
-The accesskey and secretkey of your account, endpoint and region are required as params.
-
-```python
-import tos
-
-ak = "your access key"
-sk = "your secret key"
-endpoint = "your endpoint"
-region = "your region"
-bucket_name = "your bucket name"
-object_key = "your object key"
-client = tos.TosClientV2(ak, sk, endpoint, region)     
-```
-
-## Create a bucket
-
-The bucket is a kind of unique namespace in TOS, which is a container to store data.
-This example shows you how to create a bucket.
-
-```python
-import tos
-
-ak = "your access key"
-sk = "your secret key"
-endpoint = "your endpoint"
-region = "your region"
-bucket_name = "your bucket name"
-client = tos.TosClientV2(ak, sk, endpoint, region)
-client.create_bucket(bucket_name)                            
-```
-
-## Put Object
-
-You can put your file as an object into your own bucket.
-
-```python
-# call put_object to upload you data to the TOS                     
-client.put_object(bucket_name, object_key, content="123")
-assert resp.status == 200       
-```
-## Get Object
-You can download objects in the TOS bucket through our SDK.
-
-```python
-# call get_object to download your data from your bucket
-client.get_object(bucket_name, object_key)
-```
-
-## Delete Object
-
-Your can delete your objects in the bucket：
-
-```python
-# call put_object to upload you data to the TOS  
-resp = client.put_object(bucket_name, key_name, content="123")
-assert resp.status_code == 200   
-# call delete_object to delete an object in your bucket
-resp = client.delete_object(bucket_name, key_name)
-assert resp.status_code == 204
-```
-
-## License
-[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html)
+Metadata-Version: 2.1
+Name: tos
+Version: 2.6.0
+Summary: Volc TOS (Tinder Object Storage) SDK
+Home-page: https://www.volcengine.com/
+Author: sunyushan
+Author-email: sunyushan.jason@bytedance.com
+License: UNKNOWN
+Description: 
+        # Volcengine TOS SDK for Python
+        The TOS Python SDK enables Python developers to easily work with TOS(Tinder Object Storage) service in the volcengine.
+        This document will show developers some basic examples about TOS bucket and object operation.
+        
+        
+        ## Install
+        ### Requirements
+        - Python3
+        # Quick Start
+        
+        This section introduces how to create a bucket, upload/download/delete an object in TOS service through our SDK.
+        
+        ## Create a TOS Client
+        
+        You can interact with TOS service after initiating a TOSClient instance.
+        The accesskey and secretkey of your account, endpoint and region are required as params.
+        
+        ```python
+        import tos
+        
+        ak = "your access key"
+        sk = "your secret key"
+        endpoint = "your endpoint"
+        region = "your region"
+        bucket_name = "your bucket name"
+        object_key = "your object key"
+        client = tos.TosClientV2(ak, sk, endpoint, region)     
+        ```
+        
+        ## Create a bucket
+        
+        The bucket is a kind of unique namespace in TOS, which is a container to store data.
+        This example shows you how to create a bucket.
+        
+        ```python
+        import tos
+        
+        ak = "your access key"
+        sk = "your secret key"
+        endpoint = "your endpoint"
+        region = "your region"
+        bucket_name = "your bucket name"
+        client = tos.TosClientV2(ak, sk, endpoint, region)
+        client.create_bucket(bucket_name)                            
+        ```
+        
+        ## Put Object
+        
+        You can put your file as an object into your own bucket.
+        
+        ```python
+        # call put_object to upload you data to the TOS                     
+        client.put_object(bucket_name, object_key, content="123")
+        assert resp.status == 200       
+        ```
+        ## Get Object
+        You can download objects in the TOS bucket through our SDK.
+        
+        ```python
+        # call get_object to download your data from your bucket
+        client.get_object(bucket_name, object_key)
+        ```
+        
+        ## Delete Object
+        
+        Your can delete your objects in the bucket：
+        
+        ```python
+        # call put_object to upload you data to the TOS  
+        resp = client.put_object(bucket_name, key_name, content="123")
+        assert resp.status_code == 200   
+        # call delete_object to delete an object in your bucket
+        resp = client.delete_object(bucket_name, key_name)
+        assert resp.status_code == 204
+        ```
+        
+        ## License
+        [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html)
+Keywords: boilerplate
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
```

### Comparing `tos-2.5.7/setup.py` & `tos-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 EMAIL = 'sunyushan.jason@bytedance.com'
 AUTHOR = 'sunyushan'
 
 # 项目运行需要的依赖
 REQUIRES = [
     'Deprecated>=1.2.13,<2.0.0',
     'pytz',
-    "requests>=2.19.1,<2.26.0",
+    "requests>=2.19.1, ==2.*",
     'crcmod>=1.7',
     'six',
 ]
 
 # 开发、测试过程中需要的依赖
 DEV_REQUIRES = [
     'flake8>=3.5.0,<4.0.0',
```

### Comparing `tos-2.5.7/tos/__init__.py` & `tos-2.6.0/tos/__init__.py`

 * *Files identical despite different names*

### Comparing `tos-2.5.7/tos/auth.py` & `tos-2.6.0/tos/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -240,7 +240,36 @@
     def __init__(self, access_key_id, access_key_secret, region, sts=None):
         super(Auth, self).__init__(StaticCredentials(access_key_id, access_key_secret, sts), region)
 
 
 class FederationAuth(AuthBase):
     def __init__(self, credentials_provider: FederationCredentials, region: str):
         super(FederationAuth, self).__init__(credentials_provider, region)
+
+
+class AnonymousAuth(object):
+    def __init__(self, access_key_id, access_key_secret, region, sts=None):
+        self.region = region.strip()
+
+    def copy(self):
+        return self
+
+    def sign_request(self, req):
+        pass
+
+    def sign_url(self, req, expires):
+        return req.url + '?' + '&'.join(_param_to_quoted_query(k, v) for k, v in req.params.items())
+
+    def post_sign(self, bucket: str, key: str, expires: int, conditions: [],
+                  content_length_range: ContentLengthRange) -> PreSignedPostSignatureOutPut:
+        date = datetime.datetime.utcnow().strftime(DATE_FORMAT)
+        sign = PreSignedPostSignatureOutPut()
+        sign.origin_policy = _get_post_policy(date, expires, sign.algorithm, sign.credential, bucket, key,
+                                              conditions, content_length_range)
+        sign.origin_policy = json.dumps(sign.origin_policy)
+        sign.policy = base64.b64encode(sign.origin_policy.encode('utf-8')).decode('utf-8')
+
+        return sign
+
+    def x_tos_post_sign(self, expires: int, conditions: []):
+        params = {'X-Tos-Policy': base64.b64encode(json.dumps(_get_policy(conditions)).encode('utf-8')).decode('utf-8')}
+        return '&'.join(_param_to_quoted_query(k, v) for k, v in params.items())
```

### Comparing `tos-2.5.7/tos/checkpoint.py` & `tos-2.6.0/tos/checkpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,26 +123,27 @@
                 raise CancelNotWithAbortError('user cancel upload file task not with abort')
 
 
 class BreakpointBase(object):
     def __init__(self, client, bucket, key, store: CheckPointStore, task_num,
                  parts_to_do, record: Dict,
                  size, rate_limiter, cancel_hook,
-                 datatransfer_listener, event_listener):
+                 datatransfer_listener, event_listener, traffic_limit):
         self.client = client
         self.bucket = bucket
         self.key = key
         self.task_num = task_num
         self.parts_to_do = parts_to_do
         self.record = record
         self.size = size
         self.cancel_hook = cancel_hook
         self.datatransfer_listener = datatransfer_listener
         self.event_listener = event_listener
         self.rate_limiter = rate_limiter
+        self.traffic_limit = traffic_limit
         self.need_bytes = 0
         for part in parts_to_do:
             self.need_bytes += part.size
 
         if self.datatransfer_listener:
             self.datatransfer_listener = MergeProcess(self.datatransfer_listener, size,
                                                       len(self.parts_to_do), size - self.need_bytes)
@@ -230,21 +231,22 @@
 
 
 class _BreakpointUploader(BreakpointBase):
     def __init__(self, client, bucket, key, store: CheckPointStore, task_num,
                  parts_to_update, upload_id, record: Dict,
                  size, ssec_algorithm, ssec_key, ssec_key_md5, rate_limiter, cancel_hook,
                  datatransfer_listener, upload_event_listener,
-                 file_path):
+                 file_path, traffic_limit):
 
         super(_BreakpointUploader, self).__init__(client=client, bucket=bucket, key=key, store=store, task_num=task_num,
                                                   parts_to_do=parts_to_update, record=record, size=size,
                                                   rate_limiter=rate_limiter, cancel_hook=cancel_hook,
                                                   datatransfer_listener=datatransfer_listener,
-                                                  event_listener=upload_event_listener)
+                                                  event_listener=upload_event_listener,
+                                                  traffic_limit=traffic_limit)
         self.filename = file_path
         self.task_num = task_num
         self.upload_id = upload_id
         self.cancel_hook = cancel_hook
         self.ssec_algorithm = ssec_algorithm
         self.ssec_key = ssec_key
         self.ssec_key_md5 = ssec_key_md5
@@ -263,15 +265,16 @@
                                                  part_number=part.part_number,
                                                  content=SizeAdapter(f, part.size, init_offset=part.start,
                                                                      can_reset=True),
                                                  data_transfer_listener=self.datatransfer_listener,
                                                  rate_limiter=self.rate_limiter,
                                                  ssec_algorithm=self.ssec_algorithm,
                                                  ssec_key=self.ssec_key,
-                                                 ssec_key_md5=self.ssec_key_md5)
+                                                 ssec_key_md5=self.ssec_key_md5,
+                                                 traffic_limit=self.traffic_limit)
             except Exception as e:
                 self._callback_part_fail(e, part)
                 raise e
 
             self._finish_part(
                 PartInfo(part_number=part.part_number, part_size=part.size, offset=part.start, etag=result.etag,
                          hash_crc64_ecma=result.hash_crc64_ecma, is_completed=True))
@@ -323,21 +326,22 @@
     def __init__(self, client, bucket, key, store: CheckPointStore, task_num,
                  parts_to_update, upload_id, record: Dict,
                  size, ssec_algorithm, ssec_key, ssec_key_md5, rate_limiter, cancel_hook,
                  datatransfer_listener, upload_event_listener,
                  src_bucket, src_object,
                  copy_source_if_match, copy_source_if_modified_since,
                  copy_source_if_none_match, copy_source_if_unmodified_since, src_version_id,
-                 copy_source_ssec_algorithm, copy_source_ssec_key, copy_source_ssec_key_md5):
+                 copy_source_ssec_algorithm, copy_source_ssec_key, copy_source_ssec_key_md5, traffic_limit):
         super(_BreakpointResumableCopyObject, self).__init__(client=client, bucket=bucket, key=key, store=store,
                                                              task_num=task_num,
                                                              parts_to_do=parts_to_update, record=record, size=size,
                                                              rate_limiter=rate_limiter, cancel_hook=cancel_hook,
                                                              datatransfer_listener=datatransfer_listener,
-                                                             event_listener=upload_event_listener)
+                                                             event_listener=upload_event_listener,
+                                                             traffic_limit=traffic_limit)
         self.upload_id = upload_id
         self.src_version_id = src_version_id
         self.ssec_algorithm = ssec_algorithm
         self.ssec_key = ssec_key
         self.ssec_key_md5 = ssec_key_md5
         self.src_bucket = src_bucket
         self.src_object = src_object
@@ -353,27 +357,38 @@
         for p in self.record["parts_info"]:
             self.finished_parts.append(
                 PartInfo(part_number=p['part_number'], part_size=p['part_size'], offset=p['offset'], etag=p['etag'],
                          hash_crc64_ecma=p['hash_crc64ecma'], is_completed=True))
 
     def _do_task(self, part):
         try:
-            result = self.client.upload_part_copy(self.bucket, self.key, self.upload_id, part.part_number,
-                                                  self.src_bucket, self.src_object,
-                                                  src_version_id=self.src_version_id,
-                                                  copy_source_range_start=part.start,
-                                                  # 由于拷贝为闭区间，因此end -1
-                                                  copy_source_range_end=part.start + part.size - 1,
-                                                  copy_source_if_match=self.copy_source_if_match,
-                                                  copy_source_ssec_key=self.copy_source_ssec_key,
-                                                  copy_source_ssec_algorithm=self.copy_source_ssec_algorithm,
-                                                  copy_source_ssec_key_md5=self.copy_source_ssec_key_md5,
-                                                  ssec_key=self.ssec_key,
-                                                  ssec_algorithm=self.ssec_algorithm,
-                                                  ssec_key_md5=self.ssec_key_md5)
+            if part.part_number == -1:
+                # part_number -1 则说明为空分片
+                part.part_number = 1
+                result = self.client.upload_part(bucket=self.bucket, key=self.key, upload_id=self.upload_id,
+                                                 part_number=1,
+                                                 rate_limiter=self.rate_limiter,
+                                                 ssec_algorithm=self.ssec_algorithm,
+                                                 ssec_key=self.ssec_key,
+                                                 ssec_key_md5=self.ssec_key_md5)
+            else:
+                result = self.client.upload_part_copy(self.bucket, self.key, self.upload_id, part.part_number,
+                                                      self.src_bucket, self.src_object,
+                                                      src_version_id=self.src_version_id,
+                                                      copy_source_range_start=part.start,
+                                                      # 由于拷贝为闭区间，因此end -1
+                                                      copy_source_range_end=part.start + part.size - 1,
+                                                      copy_source_if_match=self.copy_source_if_match,
+                                                      copy_source_ssec_key=self.copy_source_ssec_key,
+                                                      copy_source_ssec_algorithm=self.copy_source_ssec_algorithm,
+                                                      copy_source_ssec_key_md5=self.copy_source_ssec_key_md5,
+                                                      ssec_key=self.ssec_key,
+                                                      ssec_algorithm=self.ssec_algorithm,
+                                                      ssec_key_md5=self.ssec_key_md5,
+                                                      traffic_limit=self.traffic_limit)
         except Exception as e:
             self._callback_part_fail(e, part)
             raise e
         self._finish_part(
             PartInfo(part_number=part.part_number, part_size=part.size, offset=part.start, etag=result.etag,
                      hash_crc64_ecma=result.etag, is_completed=True))
 
@@ -426,21 +441,22 @@
 
 
 class _BreakpointDownloader(BreakpointBase):
     def __init__(self, client, bucket, key, file_path: str, store: CheckPointStore, task_num: int,
                  parts_to_download, record: Dict, etag,
                  datatransfer_listener, download_event_listener,
                  rate_limiter, cancel_hook, version_id, size,
-                 ssec_algorithm, ssec_key, ssec_key_md5):
+                 ssec_algorithm, ssec_key, ssec_key_md5, traffic_limit):
         super(_BreakpointDownloader, self).__init__(client=client, bucket=bucket, key=key, store=store,
                                                     task_num=task_num,
                                                     parts_to_do=parts_to_download, record=record, size=size,
                                                     rate_limiter=rate_limiter, cancel_hook=cancel_hook,
                                                     datatransfer_listener=datatransfer_listener,
-                                                    event_listener=download_event_listener)
+                                                    event_listener=download_event_listener,
+                                                    traffic_limit=traffic_limit)
         self.etag = etag
         self.version_id = version_id
         self.file_path = file_path
         self.rate_limiter = rate_limiter
         self.ssec_algorithm = ssec_algorithm
         self.ssec_key = ssec_key
         self.ssec_key_md5 = ssec_key_md5
@@ -468,15 +484,16 @@
                 content = self.client.get_object(bucket=self.bucket, key=self.key, range_start=part.start,
                                                  range_end=part.end - 1, if_match=self.etag,
                                                  data_transfer_listener=self.datatransfer_listener,
                                                  rate_limiter=self.rate_limiter,
                                                  ssec_algorithm=self.ssec_algorithm,
                                                  ssec_key=self.ssec_key,
                                                  ssec_key_md5=self.ssec_key_md5,
-                                                 version_id=self.version_id)
+                                                 version_id=self.version_id,
+                                                 traffic_limit=self.traffic_limit)
                 copy_and_verify_length(content, f, part.end - part.start, request_id=content.request_id)
                 if self.client.enable_crc:
                     part.part_crc = content.content.crc
             except Exception as e:
                 self._callback_part_fail(e, part)
                 raise e
             self._finish_part(part)
```

### Comparing `tos-2.5.7/tos/client.py` & `tos-2.6.0/tos/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         self.host = _get_host(self.endpoint)
         self.scheme = _get_scheme(self.endpoint)
         self.timeout = connect_timeout or CONNECT_TIMEOUT
         self.recognize_content_type = recognize_content_type
 
         self.session = requests.Session()
         self.session.mount('http://', HTTPAdapter(pool_connections=connection_pool_size,
-                                                  pool_maxsize=connection_pool_size))
+                                                  pool_maxsize=connection_pool_size, max_retries=3))
         self.session.mount('https://', HTTPAdapter(pool_connections=connection_pool_size,
-                                                   pool_maxsize=connection_pool_size))
+                                                   pool_maxsize=connection_pool_size, max_retries=3))
 
     @deprecated(version='2.1.0', reason="please use TosClientV2")
     def generate_presigned_url(self, Method: str, Bucket: str = None, Key: str = None, Params: Dict = None,
                                ExpiresIn: int = None):
         """
         生成带签名的url
         :param: Bucket: 桶名
```

### Comparing `tos-2.5.7/tos/clientv2.py` & `tos-2.6.0/tos/clientv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 from requests.structures import CaseInsensitiveDict
 from urllib3.util import connection
 from urllib3.util.connection import allowed_gai_family, _set_socket_options
 
 from . import TosClient
 from . import __version__
 from . import exceptions, utils
-from .auth import Auth
+from .auth import Auth, AnonymousAuth
 from .checkpoint import (CheckPointStore, _BreakpointDownloader,
                          _BreakpointUploader, _BreakpointResumableCopyObject)
 from .client import _make_virtual_host_url, _make_virtual_host_uri, _get_virtual_host, _get_host, _get_scheme
 from .consts import (GMT_DATE_FORMAT, SLEEP_BASE_TIME, UNSIGNED_PAYLOAD,
-                     WHITE_LIST_FUNCTION)
+                     WHITE_LIST_FUNCTION, CALLBACK_FUNCTION)
 from .enum import (ACLType, AzRedundancyType, DataTransferType, HttpMethodType,
                    MetadataDirectiveType, StorageClassType, UploadEventType, VersioningStatusType, CopyEventType)
 from .exceptions import TosClientError, TosServerError, TosError
 from .http import Request, Response
 from .json_utils import (to_complete_multipart_upload_request,
                          to_put_acl_request, to_delete_multi_objects_request, to_put_bucket_cors_request,
                          to_put_bucket_mirror_back, to_put_bucket_lifecycle, to_put_object_tagging, to_fetch_object,
                          to_put_replication, to_put_bucket_website, to_put_bucket_notification, to_put_custom_domain,
-                         to_put_bucket_real_time_log)
+                         to_put_bucket_real_time_log, to_restore_object)
 from .models2 import (AbortMultipartUpload, AppendObjectOutput,
                       CompleteMultipartUploadOutput, CopyObjectOutput,
                       CreateBucketOutput, CreateMultipartUploadOutput,
                       DeleteBucketOutput, DeleteObjectOutput,
                       DeleteObjectsOutput, DownloadPartInfo,
                       GetObjectACLOutput, GetObjectOutput, HeadBucketOutput,
                       HeadObjectOutput, ListBucketsOutput,
@@ -62,29 +62,30 @@
                       DeleteBucketReplicationOutput, PutBucketVersioningOutput, GetBucketVersionOutput,
                       RedirectAllRequestsTo, IndexDocument, ErrorDocument, RoutingRules, PutBucketWebsiteOutput,
                       PutBucketNotificationOutput, GetBucketNotificationOutput, CustomDomainRule,
                       PutBucketCustomDomainOutput, ListBucketCustomDomainOutput, DeleteCustomDomainOutput,
                       PutBucketRealTimeLogOutput, RealTimeLogConfiguration,
                       DeleteBucketRealTimeLog, GetBucketWebsiteOutput, ResumableCopyObjectOutput,
                       PreSignedPolicyURlInputOutput, ListObjectType2Output, ListObjectsIterator, GetBucketRealTimeLog,
-                      PolicySignatureCondition)
+                      PolicySignatureCondition, RestoreObjectOutput, RestoreJobParameters, RenameObjectOutput,
+                      PutBucketRenameOutput, DeleteBucketRenameOutput, GetBucketRenameOutput)
 from .utils import (SizeAdapter, _make_copy_source,
                     _make_range_string, _make_upload_part_file_content,
                     _ReaderAdapter, generate_http_proxies, get_content_type,
                     get_parent_directory_from_File, get_value, init_content,
                     meta_header_encode, to_bytes, to_str,
                     to_unicode, init_path, DnsCacheService, check_enum_type, check_part_size, check_part_number,
                     check_client_encryption_algorithm, check_server_encryption_algorithm, LogInfo, gen_key,
                     try_make_file_dir, _IterableAdapter, init_checkpoint_dir,
                     UploadEventHandler, ResumableCopyObject, DownloadEventHandler)
 
 logger = logging.getLogger(__name__)
 _dns_cache = DnsCacheService()
-USER_AGENT = 'tos-python-sdk/{0}({1}/{2};{3})'.format(__version__.__version__, sys.platform, platform.machine(),
-                                                      platform.python_version())
+USER_AGENT = 've-tos-python-sdk/{0}({1}/{2};{3})'.format(__version__.__version__, sys.platform, platform.machine(),
+                                                         platform.python_version())
 
 BASE_RETRY_DELAY_TIME = 500
 
 
 def _get_create_bucket_headers(ACL: ACLType, AzRedundancy: AzRedundancyType, GrantFullControl, GrantRead, GrantReadACP,
                                GrantWrite,
                                GrantWriteACP, StorageClass: StorageClassType):
@@ -110,15 +111,15 @@
 
 def _get_copy_object_headers(ACL, CacheControl, ContentDisposition, ContentEncoding, ContentLanguage,
                              ContentType, CopySource, CopySourceIfMatch, CopySourceIfModifiedSince,
                              CopySourceIfNoneMatch, CopySourceIfUnmodifiedSince, Expires, GrantFullControl,
                              GrantRead, GrantReadACP, GrantWriteACP, Metadata, MetadataDirective,
                              SSECustomerAlgorithm, SSECustomerKey, SSECustomerKeyMD5, server_side_encryption,
                              website_redirect_location, storage_class: StorageClassType,
-                             SSECAlgorithm, SSECKey, SSECKeyMD5):
+                             SSECAlgorithm, SSECKey, SSECKeyMD5, TrafficLimit):
     headers = {}
     if Metadata:
         for k in Metadata:
             headers['x-tos-meta-' + k] = Metadata[k]
         headers = meta_header_encode(headers)
     if isinstance(CopySource, str):
         headers['x-tos-copy-source'] = CopySource
@@ -173,14 +174,16 @@
         headers['x-tos-storage-class'] = storage_class.value
     if SSECAlgorithm:
         headers['x-tos-server-side-encryption-customer-algorithm'] = SSECAlgorithm
     if SSECKey:
         headers['x-tos-server-side-encryption-customer-key'] = SSECKey
     if SSECKeyMD5:
         headers['x-tos-server-side-encryption-customer-key-MD5'] = SSECKeyMD5
+    if TrafficLimit:
+        headers['x-tos-traffic-limit'] = str(TrafficLimit)
     return headers
 
 
 def _get_list_object_params(Delimiter, EncodingType, Marker, MaxKeys, Prefix, Reverse):
     params = {}
     if Delimiter:
         params['delimiter'] = Delimiter
@@ -258,18 +261,29 @@
     if MaxParts:
         params['max-parts'] = MaxParts
     if PartNumberMarker:
         params['part-number-marker'] = PartNumberMarker
     return params
 
 
+def _get_complete_upload_part_headers(CompleteAll, Callback, CallbackVar):
+    headers = {}
+    if CompleteAll:
+        headers['x-tos-complete-all'] = 'yes'
+    if Callback:
+        headers['x-tos-callback'] = Callback
+    if CallbackVar:
+        headers['x-tos-callback-var'] = CallbackVar
+    return headers
+
+
 def _get_upload_part_copy_headers(CopySource, CopySourceIfMatch, CopySourceIfModifiedSince,
                                   CopySourceIfNoneMatch, CopySourceIfUnmodifiedSince, CopySourceRange,
                                   CopySourceSSECAlgorithm, CopySourceSSECKey, CopySourceSSECKeyMD5,
-                                  SSECAlgorithm, SSECKey, SSECKeyMD5):
+                                  SSECAlgorithm, SSECKey, SSECKeyMD5, TrafficLimit):
     headers = {}
     if isinstance(CopySource, str):
         headers['x-tos-copy-source'] = CopySource
     elif isinstance(CopySource, dict):
         copy_source = CopySource['Bucket'] + '/' + urllib.parse.quote(CopySource['Key'], '/~')
         if 'VersionId' in CopySource:
             copy_source = copy_source + '?versionId=' + CopySource['VersionId']
@@ -294,23 +308,25 @@
 
     if SSECAlgorithm:
         headers['x-tos-server-side-encryption-customer-algorithm'] = SSECAlgorithm
     if SSECKey:
         headers['x-tos-server-side-encryption-customer-key'] = SSECKey
     if SSECKeyMD5:
         headers['x-tos-server-side-encryption-customer-key-MD5'] = SSECKeyMD5
+    if TrafficLimit:
+        headers['x-tos-traffic-limit'] = str(TrafficLimit)
     return headers
 
 
 def _get_put_object_headers(recognize_content_type, ACL, CacheControl, ContentDisposition, ContentEncoding,
                             ContentLanguage,
                             ContentLength, ContentMD5, ContentSha256, ContentType, Expires, GrantFullControl,
                             GrantRead, GrantReadACP, GrantWriteACP, Key, Metadata, SSECustomerAlgorithm,
                             SSECustomerKey, SSECustomerKeyMD5, ServerSideEncryption, StorageClass,
-                            WebsiteRedirectLocation):
+                            WebsiteRedirectLocation, TrafficLimit, Callback, CallbackVar):
     headers = {}
     if Metadata:
         for k in Metadata:
             headers['x-tos-meta-' + k] = Metadata[k]
         headers = meta_header_encode(headers)
     if ContentLength:
         headers['Content-Length'] = str(ContentLength)
@@ -350,19 +366,25 @@
         headers['x-tos-website-redirect-location'] = WebsiteRedirectLocation
     if StorageClass:
         headers['x-tos-storage-class'] = StorageClass.value
     if ServerSideEncryption:
         headers['x-tos-server-side-encryption'] = ServerSideEncryption
     if ContentSha256:
         headers['x-tos-content-sha256'] = ContentSha256
+    if TrafficLimit:
+        headers['x-tos-traffic-limit'] = str(TrafficLimit)
+    if Callback:
+        headers['x-tos-callback'] = Callback
+    if CallbackVar:
+        headers['x-tos-callback-var'] = CallbackVar
     return headers
 
 
 def _get_object_headers(IfMatch, IfModifiedSince, IfNoneMatch, IfUnmodifiedSince, Range, SSECustomerAlgorithm,
-                        SSECustomerKey, SSECustomerKeyMD5):
+                        SSECustomerKey, SSECustomerKeyMD5, TrafficLimit):
     headers = {}
     if IfMatch:
         headers['If-Match'] = IfMatch
     if IfModifiedSince:
         headers['If-Modified-Since'] = IfModifiedSince.strftime(GMT_DATE_FORMAT)
     if IfNoneMatch:
         headers['If-None-Match'] = IfNoneMatch
@@ -372,20 +394,22 @@
         headers['x-tos-server-side-encryption-customer-algorithm'] = SSECustomerAlgorithm
     if SSECustomerKey:
         headers['x-tos-server-side-encryption-customer-key'] = SSECustomerKey
     if SSECustomerKeyMD5:
         headers['x-tos-server-side-encryption-customer-key-md5'] = SSECustomerKeyMD5
     if Range:
         headers['Range'] = Range
+    if TrafficLimit:
+        headers['x-tos-traffic-limit'] = str(TrafficLimit)
 
     return headers
 
 
 def _get_object_params(ResponseCacheControl, ResponseContentDisposition, ResponseContentEncoding,
-                       ResponseContentLanguage, ResponseContentType, ResponseExpires, VersionId):
+                       ResponseContentLanguage, ResponseContentType, ResponseExpires, VersionId, Process):
     params = {}
     if VersionId:
         params['versionId'] = VersionId
     if ResponseCacheControl:
         params['response-cache-control'] = ResponseCacheControl
     if ResponseContentDisposition:
         params['response-content-disposition'] = urllib.parse.quote(ResponseContentDisposition)
@@ -393,23 +417,25 @@
         params['response-content-encoding'] = ResponseContentEncoding
     if ResponseContentLanguage:
         params['response-content-language'] = ResponseContentLanguage
     if ResponseContentType:
         params['response-content-type'] = ResponseContentType
     if ResponseExpires:
         params['response-expires'] = ResponseExpires.strftime(GMT_DATE_FORMAT)
+    if Process:
+        params['x-tos-process'] = Process
 
     return params
 
 
 def _get_append_object_headers_params(recognize_content_type, ACL, CacheControl, ContentDisposition,
                                       ContentEncoding, ContentLanguage,
                                       ContentLength, ContentType, Expires, GrantFullControl, GrantRead,
                                       GrantReadACP, GrantWriteACP, Key, Metadata, StorageClass,
-                                      WebsiteRedirectLocation):
+                                      WebsiteRedirectLocation, TrafficLimit):
     headers = {}
     if Metadata:
         for k in Metadata:
             headers['x-tos-meta-' + k] = Metadata[k]
         headers = meta_header_encode(headers)
     if ACL:
         headers['x-tos-acl'] = ACL.value
@@ -437,14 +463,16 @@
         headers['expires'] = Expires.strftime(GMT_DATE_FORMAT)
     if WebsiteRedirectLocation:
         headers['x-tos-website-redirect-location'] = WebsiteRedirectLocation
     if StorageClass:
         headers['x-tos-storage-class'] = StorageClass.value
     if ContentLength:
         headers['Content-Length'] = str(ContentLength)
+    if TrafficLimit:
+        headers['x-tos-traffic-limit'] = str(TrafficLimit)
     return headers
 
 
 def _get_create_multipart_upload_headers(recognize_content_type, ACL, CacheControl, ContentDisposition, ContentEncoding,
                                          ContentLanguage, ContentType,
                                          Expires, GrantFullControl, GrantRead, GrantReadACP,
                                          GrantWriteACP, Key, Metadata, SSECustomerAlgorithm, SSECustomerKey,
@@ -542,28 +570,30 @@
         headers['x-tos-grant-write'] = GrantWrite
     if GrantWriteACP:
         headers['x-tos-grant-write-acp'] = GrantWriteACP
     return headers
 
 
 def _get_upload_part_headers(content_length, content_md5, server_side_encryption, ssec_algorithm, ssec_key,
-                             ssec_key_md5):
+                             ssec_key_md5, traffic_limit):
     headers = {}
     if content_length:
         headers['Content-Length'] = str(content_length)
     if content_md5:
         headers['Content-MD5'] = content_md5
     if ssec_algorithm:
         headers['x-tos-server-side-encryption-customer-algorithm'] = ssec_algorithm
     if ssec_key:
         headers['x-tos-server-side-encryption-customer-key'] = ssec_key
     if ssec_key_md5:
         headers['x-tos-server-side-encryption-customer-key-md5'] = ssec_key_md5
     if server_side_encryption:
         headers['x-tos-server-side-encryption'] = server_side_encryption
+    if traffic_limit:
+        headers['x-tos-traffic-limit'] = str(traffic_limit)
 
     return headers
 
 
 def _get_fetch_headers(storage_class, acl, grant_full_control,
                        grant_read, grant_read_acp, grant_write_acp, meta,
                        ssec_customer_algorithm,
@@ -655,58 +685,67 @@
 
 
 class TosClientV2(TosClient):
     def __init__(self, ak, sk, endpoint, region,
                  security_token=None,
                  auto_recognize_content_type=True,
                  max_retry_count=3,
-                 request_timeout=60,
+                 request_timeout=120,
                  max_connections=1024,
                  enable_crc=True,
                  connection_time=10,
                  enable_verify_ssl=True,
                  dns_cache_time=0,
                  proxy_host: str = None,
                  proxy_port: int = None,
                  proxy_username: str = None,
                  proxy_password: str = None,
-                 auth=None):
+                 auth=None,
+                 is_custom_domain: bool = False):
 
         """创建client
 
         :param ak: Access Key ID: 访问密钥ID，用于标识用户
         :param sk: Secret Access Key: 与访问密钥ID结合使用的密钥，用于加密签名
         :param security_token: 临时鉴权 Token
         :param endpoint: TOS 服务端域名，完整格式：https://{host}:{port}
         :param region: TOS 服务端所在区域
         :param auto_recognize_content_type: 使用自动识别 MIME 类型，默认为 true，代表开启自动识别 MIME 类型能力
         :param max_retry_count: 请求失败后最大的重试次数。默认3次
-        :param request_timeout: 一次 HTTP 请求总超时时间，单位：毫秒，默认 60000 毫秒
-        :param connection_time: 建立连接超时时间，单位：毫秒，默认 10000 毫秒
+        :param request_timeout: socket收到一次响应的超时时间，单位：秒，默认 120 秒，
+                                参考: https://requests.readthedocs.io/en/latest/user/quickstart/#timeouts
+        :param connection_time: 建立连接超时时间，单位：秒，默认 10 秒
         :param max_connections: 连接池中允许打开的最大 HTTP 连接数，默认 1024
         :param enable_crc: 是否开启上传后客户端 CRC 校验，默认为 true
         :param enable_verify_ssl: 是否开启 SSL 证书校验，默认为 true
         :param dns_cache_time: DNS 缓存的有效期，单位：毫秒，小与等于 0 时代表关闭 DNS 缓存，默认为 0
         :param proxy_host: 代理服务器的主机地址，当前只支持 http 协议
         :param proxy_port: 代理服务器的端口
         :param proxy_username: 连接代理服务器时使用的用户名
         :param proxy_password: 代理服务使用的密码
         :param auth: 用户自定义auth
+        :param is_custom_domain: 是否使用自定义域名，默认为False
         :return TosClientV2:
         """
 
         if 's3' in endpoint:
             raise TosClientError("invalid endpoint, please use Tos endpoint rather than S3 endpoint")
 
         if auth:
             super(TosClientV2, self).__init__(auth=auth,
                                               endpoint=endpoint,
                                               recognize_content_type=auto_recognize_content_type,
                                               connection_pool_size=max_connections,
                                               connect_timeout=connection_time)
+        elif ak == "" and sk == "":
+            super(TosClientV2, self).__init__(auth=AnonymousAuth(ak, sk, region, sts=security_token),
+                                              endpoint=endpoint,
+                                              recognize_content_type=auto_recognize_content_type,
+                                              connection_pool_size=max_connections,
+                                              connect_timeout=connection_time)
         else:
             super(TosClientV2, self).__init__(auth=Auth(ak, sk, region, sts=security_token),
                                               endpoint=endpoint,
                                               recognize_content_type=auto_recognize_content_type,
                                               connection_pool_size=max_connections,
                                               connect_timeout=connection_time)
         self.max_retry_count = max_retry_count
@@ -716,14 +755,15 @@
         self.enable_verify_ssl = enable_verify_ssl
         self.proxy_host = proxy_host
         self.proxy_port = proxy_port
         self.proxy_username = proxy_username
         self.proxy_password = proxy_password
         self.enable_crc = enable_crc
         self.proxies = generate_http_proxies(proxy_host, proxy_port, proxy_username, proxy_password)
+        self.is_custom_domain = is_custom_domain
 
         # 控制动态调整初始参数
         self.lock = threading.RLock()
         # 通过 hook 机制实现in-request log
         self.session.hooks['response'].append(hook_request_log)
 
         # 开启DNS缓存
@@ -762,37 +802,42 @@
     #         self.endpoint = new_endpoint or self.endpoint
 
     def pre_signed_url(self, http_method: HttpMethodType, bucket: str,
                        key: str = None,
                        expires: int = 3600,
                        header: Dict = None,
                        query: Dict = None,
-                       alternative_endpoint: str = None):
+                       alternative_endpoint: str = None,
+                       is_custom_domain: bool = None):
         """生成签名url
 
         :param http_method: http方法
         :param bucket: 桶名
         :param key: 对象名
         :param expires: 过期时间（单位：秒），链接在当前时间再过expires秒后过期
         :param header: 需要签名的头部信息
         :param query: 需要签名的http查询参数
         :param alternative_endpoint: 签名url:如果该参数不为空，则声称的 signed url 使用该参数作为域名，而不是使用 TOS Client 初始化参数中的 endpoint
+        :param is_custom_domain: 是否使用自定义域名，默认为None
         :return
         """
         # if not _is_valid_expires(expires):
         #     raise TosClientError('expires invalid')
         key = to_str(key)
         params = query or {}
         header = header or {}
         endpoint = alternative_endpoint or self.endpoint
+        req_bucket = None if self.is_custom_domain is True else bucket
+        if is_custom_domain is not None:
+            req_bucket = None if is_custom_domain is True else bucket
         req = Request(
             http_method.value,
-            _make_virtual_host_url(_get_host(endpoint), _get_scheme(endpoint), bucket, key),
+            _make_virtual_host_url(_get_host(endpoint), _get_scheme(endpoint), req_bucket, key),
             _make_virtual_host_uri(key),
-            _get_virtual_host(bucket, endpoint),
+            _get_virtual_host(req_bucket, endpoint),
             params=params,
             headers=header
         )
         signed_url = self.auth.sign_url(req, expires)
         signed_header = req.headers.copy()
         signed_header['host'] = signed_header['Host']
         signed_header.pop('Host')
@@ -943,15 +988,16 @@
                     grant_write_acp: str = None,
                     metadata_directive: MetadataDirectiveType = None,
                     meta: Dict = None,
                     website_redirect_location: str = None,
                     storage_class: StorageClassType = None,
                     ssec_algorithm: str = None,
                     ssec_key: str = None,
-                    ssec_key_md5: str = None):
+                    ssec_key_md5: str = None,
+                    traffic_limit: int = None):
         """拷贝对象
 
         此接口用于在同一地域下同一个桶或者不同桶之间对象的拷贝操作。桶开启多版本场景，如果需要恢复对象的早期版本为当前版本，
         您只需将对象的早期版本拷贝到同一个桶中，TOS会将该对象对应早期版本置为当前版本。
 
         :param bucket: 目标桶名
         :param src_bucket: 原桶名
@@ -981,14 +1027,15 @@
         :param copy_source_ssec_key_md5: 密钥md5值
         :param server_side_encryption: TOS管理密钥的加密方式，可扩展，当前只支持 AES256
         :param website_redirect_location: 可以将获取这个对象的请求重定向到桶内另一个对象或一个外部的URL，TOS将这个值从头域中取出，保存在对象的元数据中。
         :param storage_class: 对象存储类型
         :param ssec_algorithm: 目标对象的加密方式
         :param ssec_key: 目标对象的加密 key
         :param ssec_key_md5: 目标对象加密key的md5值
+        :param traffic_limit: 单链接限速
         :return: CopyObjectOutput
         """
         check_enum_type(acl=acl, metadata_directive=metadata_directive, storage_class=storage_class)
 
         check_client_encryption_algorithm(copy_source_ssec_algorithm)
 
         check_client_encryption_algorithm(ssec_algorithm)
@@ -1000,15 +1047,15 @@
         headers = _get_copy_object_headers(acl, cache_control, content_disposition, content_encoding, content_language,
                                            content_type, copy_source, copy_source_if_match,
                                            copy_source_if_modified_since,
                                            copy_source_if_none_match, copy_source_if_unmodified_since, expires,
                                            grant_full_control, grant_read, grant_read_acp, grant_write_acp, meta,
                                            metadata_directive, copy_source_ssec_algorithm, copy_source_ssec_key,
                                            copy_source_ssec_key_md5, server_side_encryption, website_redirect_location,
-                                           storage_class, ssec_algorithm, ssec_key, ssec_key_md5)
+                                           storage_class, ssec_algorithm, ssec_key, ssec_key_md5, traffic_limit)
 
         resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Put.value, headers=headers)
 
         return CopyObjectOutput(resp)
 
     def delete_object(self, bucket: str, key: str, version_id: str = None):
         """删除对象
@@ -1092,15 +1139,15 @@
         :param ssec_key_md5: 密钥md5值
 
         :return: HeadObjectOutput
         """
         check_client_encryption_algorithm(ssec_algorithm)
 
         headers = _get_object_headers(if_match, if_modified_since, if_none_match, if_unmodified_since, None,
-                                      ssec_algorithm, ssec_key, ssec_key_md5)
+                                      ssec_algorithm, ssec_key, ssec_key_md5, None)
 
         params = {}
 
         if version_id:
             params['versionId'] = version_id
         resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Head.value, params=params,
                          headers=headers)
@@ -1226,15 +1273,18 @@
                    ssec_key_md5: str = None,
                    server_side_encryption: str = None,
                    meta: Dict = None,
                    website_redirect_location: str = None,
                    storage_class: StorageClassType = None,
                    data_transfer_listener=None,
                    rate_limiter=None,
-                   content=None) -> PutObjectOutput:
+                   traffic_limit: int = None,
+                   content=None,
+                   callback: str = None,
+                   callback_var: str = None) -> PutObjectOutput:
         """上传对象
 
         :param bucket: 桶名
         :param key: 对象名
         :param acl: 'private'|'public-read'|'public-read-write'|'authenticated-read'|'bucket-owner-read'|
                 'bucket-owner-full-control'
         :param content_length: 消息体大小
@@ -1255,15 +1305,18 @@
         :param ssec_algorithm: 客户自定义密钥的加密方式，可扩展，不定义为枚举，当前只支持 AES256，TOS SDK 会做强校验
         :param ssec_key: 加密密钥
         :param ssec_key_md5: 密钥md5值
         :param storage_class: 对象存储类型
         :param website_redirect_location: 可以将获取这个对象的请求重定向到桶内另一个对象或一个外部的URL，TOS将这个值从头域中取出，保存在对象的元数据中。
         :param data_transfer_listener: 进度条特效
         :param rate_limiter: 客户端限速
+        :param traffic_limit: 单连接限速
         :param content: 数据
+        :param callback: 回调
+        :param callback_var: 回调参数
         :return: PutObjectOutput
         """
         check_client_encryption_algorithm(ssec_algorithm)
 
         check_server_encryption_algorithm(server_side_encryption)
 
         check_enum_type(acl=acl, storage_class=storage_class)
@@ -1271,15 +1324,16 @@
         _is_valid_object_name(key)
 
         headers = _get_put_object_headers(self.recognize_content_type, acl, cache_control, content_disposition,
                                           content_encoding, content_language,
                                           content_length, content_md5, content_sha256, content_type, expires,
                                           grant_full_control, grant_read, grant_read_acp, grant_writeAcp, key, meta,
                                           ssec_algorithm, ssec_key, ssec_key_md5,
-                                          server_side_encryption, storage_class, website_redirect_location)
+                                          server_side_encryption, storage_class, website_redirect_location,
+                                          traffic_limit, callback, callback_var)
 
         if content:
             content = init_content(content)
 
             if data_transfer_listener:
                 content = utils.add_progress_listener_func(content, data_transfer_listener)
 
@@ -1288,15 +1342,15 @@
 
             if self.enable_crc:
                 content = utils.add_crc_func(content)
 
         try:
             resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Put.value, data=content,
                              headers=headers)
-            result = PutObjectOutput(resp)
+            result = PutObjectOutput(resp, callback=callback)
             if self.enable_crc and content:
                 utils.check_crc('put_object', content.crc, result.hash_crc64_ecma, result.request_id)
             return result
 
         except (TosClientError, TosServerError) as e:
             if data_transfer_listener:
                 data_transfer_listener(0, 0, 0, DataTransferType.Data_Transfer_Failed)
@@ -1321,14 +1375,15 @@
                              ssec_key: str = None,
                              ssec_key_md5: str = None,
                              server_side_encryption: str = None,
                              meta: Dict = None,
                              website_redirect_location: str = None,
                              storage_class: StorageClassType = None,
                              data_transfer_listener=None,
+                             traffic_limit: int = None,
                              rate_limiter=None) -> PutObjectOutput:
         """上传对象
 
         :param bucket: 桶名
         :param key: 对象名
         :param acl: 'private'|'public-read'|'public-read-write'|'authenticated-read'|'bucket-owner-read'|
                 'bucket-owner-full-control'
@@ -1351,14 +1406,15 @@
         :param ssec_key: 加密密钥
         :param ssec_key_md5: 密钥md5值
         :param storage_class: 对象存储类型
         :param website_redirect_location: 可以将获取这个对象的请求重定向到桶内另一个对象或一个外部的URL，TOS将这个值从头域中取出，保存在对象的元数据中。
         :param data_transfer_listener: 进度条特效
         :param rate_limiter: 客户端限速
         :param file_path: 文件路径
+        :param traffic_limit: 单连接限速
         :return: PutObjectOutput
         """
         check_client_encryption_algorithm(ssec_algorithm)
 
         check_server_encryption_algorithm(server_side_encryption)
 
         if not os.path.exists(file_path) or (os.path.isdir(file_path)):
@@ -1367,15 +1423,15 @@
         with open(to_unicode(file_path), 'rb') as f:
             f = init_content(f, can_reset=True, init_offset=0)
             return self.put_object(bucket, key, content_length, content_md5, content_sha256, cache_control,
                                    content_disposition, content_encoding, content_language,
                                    content_type, expires, acl, grant_full_control, grant_read, grant_read_acp,
                                    grant_writeAcp, ssec_algorithm, ssec_key,
                                    ssec_key_md5, server_side_encryption, meta, website_redirect_location, storage_class,
-                                   data_transfer_listener, rate_limiter, f)
+                                   data_transfer_listener, rate_limiter, traffic_limit, f)
 
     def append_object(self, bucket: str, key: str, offset: int,
                       content=None,
                       content_length: int = None,
                       cache_control: str = None,
                       content_disposition: str = None,
                       content_encoding: str = None,
@@ -1388,15 +1444,16 @@
                       grant_read_acp: str = None,
                       grant_write_acp: str = None,
                       meta: Dict = None,
                       website_redirect_location: str = None,
                       storage_class: StorageClassType = None,
                       data_transfer_listener=None,
                       rate_limiter=None,
-                      pre_hash_crc64_ecma: int = None):
+                      pre_hash_crc64_ecma: int = None,
+                      traffic_limit: int = None) -> AppendObjectOutput:
         """追加写对象
 
         :param bucket: 桶名
         :param key: 对象名
         :param content: 上传内容
         :param cache_control:	指定该对象被下载时网页的缓存行为
         :param content_disposition: 内容呈现方式
@@ -1412,30 +1469,32 @@
         :param grant_read:  'id="xxx",canned="AllUsers"|"AuthenticatedUsers"'
         :param grant_read_acp:  'id="xxx",canned="AllUsers"|"AuthenticatedUsers"'
         :param grant_write_acp: 'id="xxx",canned="AllUsers"|"AuthenticatedUsers"'
         :param website_redirect_location: 当桶设置了Website配置，可以将获取这个对象的请求重定向到桶内另一个对象或一个外部的URL，TOS将这个值从头域中取出，保存在对象的元数据中。
         :param storage_class: 第一次追加写对象时，可以使用该头域，设置目的对象的存储类型。如果未设置，则目的对象的存储类型，和所在桶的默认存储类型保持一致
         :param data_transfer_listener: 进度条特效
         :param rate_limiter: 客户端限速
+        :param traffic_limit: 单连接限制速
         :param pre_hash_crc64_ecma: 上一次crc值，第一次上传设置为0
+        :return: AppendObjectOutput
         """
 
         check_enum_type(acl=acl, storage_class=storage_class)
 
         _is_valid_object_name(key)
 
         params = {'append': '', 'offset': offset}
 
         headers = _get_append_object_headers_params(self.recognize_content_type, acl, cache_control,
                                                     content_disposition,
                                                     content_encoding,
                                                     content_language, content_length, content_type,
                                                     expires, grant_full_control, grant_read, grant_read_acp,
                                                     grant_write_acp, key, meta, storage_class,
-                                                    website_redirect_location)
+                                                    website_redirect_location, traffic_limit)
 
         if content:
             content = init_content(content)
             if isinstance(content, _ReaderAdapter) and content.size == 0:
                 raise TosClientError('Your proposed append content is smaller than the minimum allowed size')
 
             if data_transfer_listener:
@@ -1510,15 +1569,18 @@
                    response_content_language: str = None,
                    response_content_type: str = None,
                    response_expires: datetime = None,
                    range_start: int = None,
                    range_end: int = None,
                    data_transfer_listener=None,
                    rate_limiter=None,
-                   range: str = None) -> GetObjectOutput:
+                   range: str = None,
+                   traffic_limit: int = None,
+                   process: str = None) -> GetObjectOutput:
+
         """下载对象
 
         :param bucket: 桶名
         :param key: 对象名
         :param if_match: 只有在匹配时，才返回对象
         :param if_modified_since: datetime(2021, 1, 1)
         :param if_none_match: 只有在不匹配时，才返回对象
@@ -1534,26 +1596,30 @@
         :param ssec_key: 加密密钥
         :param ssec_key_md5: 密钥md5值
         :param data_transfer_listener: 进度条回调函数
         :param rate_limiter: 限速接口
         :param range_start: 指定对象的获取下边界
         :param range_end: 指定对象获取的上边界
         :param range: 查询范围 与range_start range_end 互斥优先使用此字段
+        :param traffic_limit: 单连接限速
+        :param process: 图片处理参数
         :return: GetObjectOutput
         """
+
         check_client_encryption_algorithm(ssec_algorithm)
 
         if range is None:
             range = _make_range_string(range_start, range_end)
 
         headers = _get_object_headers(if_match, if_modified_since, if_none_match, if_unmodified_since, range,
-                                      ssec_algorithm, ssec_key, ssec_key_md5)
+                                      ssec_algorithm, ssec_key, ssec_key_md5, traffic_limit)
 
         params = _get_object_params(response_cache_control, response_content_disposition, response_content_encoding,
-                                    response_content_language, response_content_type, response_expires, version_id)
+                                    response_content_language, response_content_type, response_expires, version_id,
+                                    process)
 
         resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Get.value, headers=headers,
                          params=params)
 
         return GetObjectOutput(resp, progress_callback=data_transfer_listener, rate_limiter=rate_limiter,
                                enable_crc=self.enable_crc)
 
@@ -1571,15 +1637,16 @@
                            response_content_encoding: str = None,
                            response_content_language: str = None,
                            response_content_type: str = None,
                            response_expires: datetime = None,
                            range_start: int = None,
                            range_end: int = None,
                            data_transfer_listener=None,
-                           rate_limiter=None):
+                           rate_limiter=None,
+                           traffic_limit: int = None):
         """下载对象到文件
 
         :param bucket: 桶名
         :param key: 对象名
         :param if_match: 只有在匹配时，才返回对象
         :param if_modified_since: datetime(2021, 1, 1)
         :param if_none_match: 只有在不匹配时，才返回对象
@@ -1595,14 +1662,15 @@
         :param ssec_key: 加密密钥
         :param ssec_key_md5: 密钥md5值
         :param data_transfer_listener: 进度条回调函数
         :param rate_limiter: 限速接口
         :param range_start: 指定对象的获取下边界
         :param range_end: 指定对象获取的上边界
         :param file_path: 文件路径
+        :param traffic_limit: 单连接限速
         :return: GetObjectOutput
         """
 
         check_client_encryption_algorithm(ssec_algorithm)
         result = self.get_object(bucket=bucket,
                                  key=key,
                                  version_id=version_id,
@@ -1618,16 +1686,16 @@
                                  response_content_encoding=response_content_encoding,
                                  response_content_language=response_content_language,
                                  response_content_type=response_content_type,
                                  response_expires=response_expires,
                                  range_start=range_start,
                                  range_end=range_end,
                                  data_transfer_listener=data_transfer_listener,
-                                 rate_limiter=rate_limiter
-                                 )
+                                 rate_limiter=rate_limiter,
+                                 traffic_limit=traffic_limit)
 
         if init_path(file_path, key):
             dir = os.path.join(file_path, key)
             os.makedirs(dir, exist_ok=True)
             # 空循环读取数据
             for content in result.content:
                 pass
@@ -1735,15 +1803,16 @@
                     part_size: int = 20 * 1024 * 1024,
                     task_num: int = 1,
                     enable_checkpoint: bool = True,
                     checkpoint_file: str = None,
                     data_transfer_listener=None,
                     upload_event_listener=None,
                     rate_limiter=None,
-                    cancel_hook=None):
+                    cancel_hook=None,
+                    traffic_limit: int = None):
 
         """断点续传上传
 
         :param bucket: 桶名
         :param key: 对象名
         :param encoding_type: 指定对返回的内容进行编码的编码类型
         :param cache_control:  是否开启缓存
@@ -1769,14 +1838,15 @@
         :param enable_checkpoint: 是否启用断点传输
         :param checkpoint_file: 断点传输文件全路径
         :param data_transfer_listener: 进度条特性
         :param upload_event_listener: 上传事件回调
         :param rate_limiter: 客户端限速
         :param storage_class: 存储类型
         :param cancel_hook: 支持取消断点任务
+        :param traffic_limit: 单连接限速
         :return: CreateMultipartUploadOutput
         """
         check_client_encryption_algorithm(ssec_algorithm)
 
         check_server_encryption_algorithm(server_side_encryption)
 
         check_enum_type(acl=acl, storage_class=storage_class)
@@ -1879,15 +1949,15 @@
                 parts = _get_parts_to_upload(size, part_size, [])
 
         uploader = _BreakpointUploader(self, bucket=bucket, key=key, file_path=file_path, store=store,
                                        task_num=task_num, parts_to_update=parts, upload_id=upload_id,
                                        record=record, datatransfer_listener=data_transfer_listener,
                                        upload_event_listener=upload_event_listener, cancel_hook=cancel_hook,
                                        rate_limiter=rate_limiter, size=size, ssec_algorithm=ssec_algorithm,
-                                       ssec_key=ssec_key, ssec_key_md5=ssec_key_md5)
+                                       ssec_key=ssec_key, ssec_key_md5=ssec_key_md5, traffic_limit=traffic_limit)
 
         result = uploader.execute()
 
         return UploadFileOutput(result, ssec_algorithm, ssec_key_md5, upload_id, record['encoding_type'])
 
     def resumable_copy_object(self, bucket: str, key: str, src_bucket: str, src_key: str,
                               encoding_type: str = None,
@@ -1918,15 +1988,16 @@
                               copy_source_ssec_key: str = None,
                               copy_source_ssec_key_md5: str = None,
                               part_size: int = 20 * 1024 * 1024,
                               task_num: int = 1,
                               enable_checkpoint: bool = True,
                               checkpoint_file: str = None,
                               copy_event_listener=None,
-                              cancel_hook=None) -> ResumableCopyObjectOutput:
+                              cancel_hook=None,
+                              traffic_limit: int = None) -> ResumableCopyObjectOutput:
         """断点续传复制
 
         :param bucket: 桶名
         :param key: 对象名
         :param src_bucket: 源桶名
         :param src_key: 源对象名
         :param encoding_type: 指定对返回的内容进行编码的编码类型
@@ -1958,14 +2029,15 @@
         :param copy_source_ssec_key_md5: 密钥md5值
         :param part_size: 分片大小 默认为 20mb
         :param task_num: 执行任务线程数
         :param enable_checkpoint: 是否开启断点续传
         :param checkpoint_file: 断点续传上传文件夹，在该文件夹下生成断点续传文件
         :param copy_event_listener: 断点续传事件回调
         :param cancel_hook: 取消回调
+        :param traffic_limit: 单连接限速
         :return: ResumableCopyObjectOutput
         """
 
         check_client_encryption_algorithm(ssec_algorithm)
 
         check_server_encryption_algorithm(server_side_encryption)
 
@@ -1981,16 +2053,16 @@
                                     if_unmodified_since=copy_source_if_unmodified_since,
                                     ssec_key=copy_source_ssec_key,
                                     ssec_key_md5=copy_source_ssec_key_md5,
                                     ssec_algorithm=copy_source_ssec_algorithm)
 
         size = head_out.content_length
 
-        if size == 0:
-            raise TosClientError('object size is 0, please use copy_object')
+        # if size == 0:
+        #     raise TosClientError('object size is 0, please use copy_object')
 
         check_part_number(size, part_size)
 
         if checkpoint_file:
             dir = init_checkpoint_dir(checkpoint_file)
         else:
             dir = tempfile.gettempdir()
@@ -2070,14 +2142,17 @@
                 'parts_info': []
             }
 
             store.put(bucket, key, record, src_bucket=src_bucket, src_key=src_key, version_id=src_version_id)
 
             parts = _get_parts_to_upload(size, part_size, [])
 
+        # 若源对象大小为0，则直接上传一个空分片
+        if size == 0:
+            parts.append(_PartToDo(part_number=-1, start=0, end=0))
         uploader = _BreakpointResumableCopyObject(self, bucket=bucket, key=key, store=store,
                                                   src_bucket=src_bucket, src_object=src_key,
                                                   src_version_id=src_version_id,
                                                   task_num=task_num, parts_to_update=parts, upload_id=upload_id,
                                                   record=record, size=size, ssec_key=ssec_key,
                                                   ssec_key_md5=ssec_key_md5,
                                                   ssec_algorithm=ssec_algorithm,
@@ -2087,15 +2162,16 @@
                                                   copy_source_ssec_algorithm=copy_source_ssec_algorithm,
                                                   copy_source_ssec_key=copy_source_ssec_key,
                                                   copy_source_ssec_key_md5=copy_source_ssec_key_md5,
                                                   rate_limiter=None,
                                                   datatransfer_listener=None,
                                                   copy_source_if_none_match=copy_source_if_none_match,
                                                   copy_source_if_unmodified_since=copy_source_if_unmodified_since,
-                                                  copy_source_if_modified_since=copy_source_if_modified_since)
+                                                  copy_source_if_modified_since=copy_source_if_modified_since,
+                                                  traffic_limit=traffic_limit)
 
         result = uploader.execute(tos_crc=head_out.hash_crc64_ecma)
 
         return ResumableCopyObjectOutput(result, ssec_algorithm, ssec_key_md5, record['encoding_type'])
 
     def download_file(self, bucket: str, key: str, file_path: str,
                       version_id: str = None,
@@ -2109,15 +2185,16 @@
                       part_size: int = 20 * 1024 * 1024,
                       task_num: int = 1,
                       enable_checkpoint: bool = True,
                       checkpoint_file: str = None,
                       data_transfer_listener=None,
                       download_event_listener=None,
                       rate_limiter=None,
-                      cancel_hook=None):
+                      cancel_hook=None,
+                      traffic_limit: int = None):
         """断点传输下载
 
         :param bucket: 桶名
         :param key: 对象名
         :param file_path: 下载存储路径
         :param if_match: 只有在匹配时，才返回对象
         :param if_modified_since: datetime(2021, 1, 1)
@@ -2131,14 +2208,15 @@
         :param task_num: 并发数
         :param enable_checkpoint: 是否开启断点传输
         :param checkpoint_file: checkpoint 文件
         :param data_transfer_listener: 进度条特性
         :param download_event_listener: 下载事件回调
         :param rate_limiter: 客户端限速
         :param cancel_hook: 取消断点下载任务
+        :param traffic_limit: 单连接限速
         :return: HeadObjectOutput
         """
         check_client_encryption_algorithm(ssec_algorithm)
 
         # 校验待下载的本地文件路径有效性
         if not file_path:
             raise TosClientError('tos: file_path = {0} is invalid'.format(file_path))
@@ -2223,30 +2301,31 @@
 
         downloader = _BreakpointDownloader(client=self, bucket=bucket, key=key, file_path=file_path, store=store,
                                            task_num=task_num, parts_to_download=parts, record=record, etag=result.etag,
                                            datatransfer_listener=data_transfer_listener,
                                            download_event_listener=download_event_listener, rate_limiter=rate_limiter,
                                            cancel_hook=cancel_hook, size=result.content_length,
                                            ssec_algorithm=ssec_algorithm, ssec_key=ssec_key, ssec_key_md5=ssec_key_md5,
-                                           version_id=version_id)
+                                           version_id=version_id, traffic_limit=traffic_limit)
 
         downloader.execute(tos_crc=result.hash_crc64_ecma)
 
         return result
 
     def upload_part(self, bucket: str, key: str, upload_id: str, part_number: int,
                     content_md5: str = None,
                     ssec_algorithm: str = None,
                     ssec_key: str = None,
                     ssec_key_md5: str = None,
                     server_side_encryption: str = None,
                     content_length: int = None,
                     content=None,
                     data_transfer_listener=None,
-                    rate_limiter=None) -> UploadPartOutput:
+                    rate_limiter=None,
+                    traffic_limit: int = None) -> UploadPartOutput:
 
         """上传分片数据
 
         :param bucket: 桶名
         :param key: 对象名称
         :param upload_id: 初始化分片任务返回的分片任务ID，用于唯一标识上传的分片属于哪个对象。
         :param part_number: 上传的分片号，有效取值[1,10000]。
@@ -2255,22 +2334,23 @@
         :param ssec_key: 指定加密目标对象的加密密钥。
         :param ssec_key_md5: 该头域表示加密目标对象使用的密钥的MD5值。MD5值用于消息完整性检查，确认加密密钥传输过程中没有出错。
         :param server_side_encryption: 指定server的加密方式
         :param content_length: 消息体的长度
         :param content: 内容
         :param data_transfer_listener: 进度条
         :param rate_limiter: 限速
+        :param traffic_limit: 单连接限速
         :return: UploadPartOutput
         """
         check_client_encryption_algorithm(ssec_algorithm)
 
         check_server_encryption_algorithm(server_side_encryption)
 
         headers = _get_upload_part_headers(content_length, content_md5, server_side_encryption, ssec_algorithm,
-                                           ssec_key, ssec_key_md5)
+                                           ssec_key, ssec_key_md5, traffic_limit)
 
         if content:
             content = init_content(content)
 
             if data_transfer_listener:
                 content = utils.add_progress_listener_func(content, data_transfer_listener)
 
@@ -2298,15 +2378,16 @@
                               ssec_key: str = None,
                               ssec_key_md5: str = None,
                               server_side_encryption: str = None,
                               data_transfer_listener=None,
                               rate_limiter=None,
                               file_path: str = None,
                               part_size: int = -1,
-                              offset: int = 0) -> UploadPartOutput:
+                              offset: int = 0,
+                              traffic_limit: int = None) -> UploadPartOutput:
         """以文件形式上传分片数据
 
         :param bucket: 桶名
         :param key: 对象名称
         :param upload_id: 初始化分片任务返回的分片任务ID，用于唯一标识上传的分片属于哪个对象。
         :param part_number: 上传的分片号，有效取值[1,10000]。
         :param content_md5: 	消息体的MD5摘要
@@ -2315,14 +2396,15 @@
         :param ssec_key_md5: 该头域表示加密目标对象使用的密钥的MD5值。MD5值用于消息完整性检查，确认加密密钥传输过程中没有出错。
         :param server_side_encryption: 指定server的加密方式
         :param data_transfer_listener: 进度条
         :param rate_limiter: 限速度
         :param file_path: 文件路径
         :param part_size: 当前分段长度
         :param offset: 当前分段在文件中的起始位置
+        :param traffic_limit: 单连接限速
         :return: UploadPartOutput
         """
         check_client_encryption_algorithm(ssec_algorithm)
 
         check_server_encryption_algorithm(server_side_encryption)
 
         with open(file_path, 'rb') as f:
@@ -2339,34 +2421,44 @@
                                     content_md5=content_md5,
                                     ssec_algorithm=ssec_algorithm,
                                     ssec_key=ssec_key,
                                     ssec_key_md5=ssec_key_md5,
                                     server_side_encryption=server_side_encryption,
                                     content=content,
                                     data_transfer_listener=data_transfer_listener,
-                                    rate_limiter=rate_limiter
+                                    rate_limiter=rate_limiter,
+                                    traffic_limit=traffic_limit
                                     )
 
-    def complete_multipart_upload(self, bucket: str, key: str, upload_id: str,
-                                  parts: []) -> CompleteMultipartUploadOutput:
+    def complete_multipart_upload(self, bucket: str, key: str, upload_id: str, parts: [],
+                                  complete_all: bool = False,
+                                  callback: str = None,
+                                  callback_var: str = None) -> CompleteMultipartUploadOutput:
         """ 合并段
 
         :param bucket: 桶名
         :param key: 对象名
         :param upload_id: 分段任务编号
         :param parts: 完成的分段任务
+        :param complete_all: 指定是否合并指定当前UploadId已上传的所有Part
+        :param callback: 回调
+        :param callback_var: 回调参数
         :return: CompleteMultipartUploadOutput
         """
-        body = to_complete_multipart_upload_request(parts)
-        data = json.dumps(body)
+        headers = _get_complete_upload_part_headers(complete_all, callback, callback_var)
+
+        data = None
+        if not complete_all:
+            body = to_complete_multipart_upload_request(parts)
+            data = json.dumps(body)
 
         resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Post.value,
-                         params={'uploadId': upload_id}, data=data)
+                         params={'uploadId': upload_id}, data=data, headers=headers)
 
-        return CompleteMultipartUploadOutput(resp)
+        return CompleteMultipartUploadOutput(resp, callback)
 
     def abort_multipart_upload(self, bucket: str, key: str, upload_id: str) -> AbortMultipartUpload:
         """取消分片上传
 
         :param bucket: 桶名
         :param key: 对象名
         :param upload_id: 分片任务id
@@ -2388,15 +2480,16 @@
                          copy_source_if_unmodified_since: datetime = None,
                          copy_source_ssec_algorithm: str = None,
                          copy_source_ssec_key: str = None,
                          copy_source_ssec_key_md5: str = None,
                          ssec_algorithm: str = None,
                          ssec_key: str = None,
                          ssec_key_md5: str = None,
-                         copy_source_range: str = None) -> UploadPartCopyOutput:
+                         copy_source_range: str = None,
+                         traffic_limit: int = None) -> UploadPartCopyOutput:
         """复制段
 
         :param bucket: 桶名
         :param key: 对象名
         :param upload_id: 初始化分片任务返回的段任务ID，用于唯一标识上传的分片属于哪个对象。
         :param part_number: 上传的分片号，有效取值[1,10000]。
         :param src_bucket: 指定拷贝的源桶名
@@ -2411,27 +2504,29 @@
         :param copy_source_if_unmodified_since: 如果自指定时间以来对象未被修改，则复制该对象。
         :param copy_source_ssec_key: SSE-C方式下使用该头域，指定解密源对象的加密密钥。此头域提供的加密密钥必须是创建源对象时使用的密钥。
         :param copy_source_ssec_key_md5: SSE-C方式下使用该头域，该头域表示解密源对象使用的密钥的MD5值。MD5值用于消息完整性检查，确认加密密钥传输过程中没有出错。
         :param copy_source_ssec_algorithm: ssec 加密算法
         :param ssec_algorithm: 目标对象的加密方式
         :param ssec_key: 目标对象的加密 key
         :param ssec_key_md5: 目标对象加密key的md5值
+        :param traffic_limit: 单连接限速
         return: UploadPartCopyOutput
         """
         check_client_encryption_algorithm(copy_source_ssec_algorithm)
 
         copy_source = _make_copy_source(src_bucket=src_bucket, src_key=src_key, src_version_id=src_version_id)
 
         if copy_source_range is None:
             copy_source_range = _make_range_string(copy_source_range_start, copy_source_range_end)
 
         headers = _get_upload_part_copy_headers(copy_source, copy_source_if_match, copy_source_if_modified_since,
                                                 copy_source_if_none_match, copy_source_if_unmodified_since,
                                                 copy_source_range, copy_source_ssec_algorithm, copy_source_ssec_key,
-                                                copy_source_ssec_key_md5, ssec_algorithm, ssec_key, ssec_key_md5)
+                                                copy_source_ssec_key_md5, ssec_algorithm, ssec_key, ssec_key_md5,
+                                                traffic_limit)
 
         resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Put.value,
                          params={'uploadId': upload_id, 'partNumber': part_number},
                          headers=headers)
 
         return UploadPartCopyOutput(resp, part_number)
 
@@ -2974,22 +3069,24 @@
         """ 删除静态网站配置
         :param bucket: 桶名
         :return: PutBucketWebsiteOutput
         """
         resp = self._req(bucket=bucket, method=HttpMethodType.Http_Method_Delete.value, params={'website': ''})
         return PutBucketWebsiteOutput(resp)
 
-    def put_bucket_notification(self, bucket: str, cloud_function_configurations: []) -> PutBucketNotificationOutput:
+    def put_bucket_notification(self, bucket: str, cloud_function_configurations: [] = None,
+                                rocket_mq_configurations: [] = None) -> PutBucketNotificationOutput:
         """
 
         :param: bucket: 桶名
         :param: cloudFunctionConfigurations: 配置
+        :param: rocket_mq_configurations: rocketMQ 配置
         :return: PutBucketNotificationOutput
         """
-        data = to_put_bucket_notification(cloud_function_configurations)
+        data = to_put_bucket_notification(cloud_function_configurations, rocket_mq_configurations)
         data = json.dumps(data)
         headers = {"Content-MD5": to_str(base64.b64encode(hashlib.md5(to_bytes(data)).digest()))}
         resp = self._req(bucket=bucket, method=HttpMethodType.Http_Method_Put.value, params={'notification': ''},
                          data=data,
                          headers=headers)
         return PutBucketNotificationOutput(resp)
 
@@ -3056,23 +3153,88 @@
 
         :param: bucket: 桶名
         :return: PutBucketRealTimeLogOutput
         """
         resp = self._req(bucket=bucket, method=HttpMethodType.Http_Method_Get.value, params={'realtimeLog': ''})
         return GetBucketRealTimeLog(resp)
 
-    def delete_bucket_real_time_log(self, bucket) -> DeleteBucketRealTimeLog:
+    def delete_bucket_real_time_log(self, bucket: str) -> DeleteBucketRealTimeLog:
         """ 删除桶实时日志配置
 
         :param bucket: 桶名
         :return: DeleteBucketRealTimeLog
         """
         resp = self._req(bucket=bucket, method=HttpMethodType.Http_Method_Delete.value, params={'realtimeLog': ''})
         return DeleteBucketRealTimeLog(resp)
 
+    def restore_object(self, bucket: str, key: str, days: int, version_id: str = None,
+                       restore_job_parameters: RestoreJobParameters = None) -> RestoreObjectOutput:
+        """ 取回对象
+        :param bucket: 桶名
+        :param key: 对象名
+        :param version_id: 版本id
+        :param days: 恢复天数
+        :param restore_job_parameters: 取回方式
+        :return: RestoreObjectOutput
+        """
+        data = to_restore_object(days, restore_job_parameters)
+        data = json.dumps(data)
+
+        headers = {"Content-MD5": to_str(base64.b64encode(hashlib.md5(to_bytes(data)).digest()))}
+        params = {"restore": ""}
+        if version_id:
+            params["versionId"] = version_id
+
+        resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Post.value,
+                         params=params, headers=headers, data=data)
+
+        return RestoreObjectOutput(resp)
+
+    def rename_object(self, bucket: str, key: str, new_key: str):
+        """ 重命名对象
+        :param bucket: 桶名
+        :param key: 对象名
+        :param new_key: 新对象名
+        :return: RenameObjectOutput
+        """
+        _is_valid_object_name(new_key)
+        params = {"rename": "", "name": new_key}
+        resp = self._req(bucket=bucket, key=key, method=HttpMethodType.Http_Method_Put.value, params=params)
+        return RenameObjectOutput(resp)
+
+    def get_bucket_rename(self, bucket: str):
+        """ 获取桶rename是否开启rename功能
+        :param bucket: 桶名
+        :return: GetBucketRenameOutput
+        """
+        resp = self._req(bucket=bucket, method=HttpMethodType.Http_Method_Get.value, params={"rename": ""})
+        return GetBucketRenameOutput(resp)
+
+    def put_bucket_rename(self, bucket: str, rename_enable: bool):
+        """ 设置开启rename功能
+        :param bucket: 桶名
+        :param rename_enable: 是否开启桶rename功能
+        :return: PutBucketRenameOutput
+        """
+        data = {"RenameEnable": rename_enable}
+        data = json.dumps(data)
+
+        headers = {"Content-MD5": to_str(base64.b64encode(hashlib.md5(to_bytes(data)).digest()))}
+        resp = self._req(bucket=bucket, method=HttpMethodType.Http_Method_Put.value, data=data, headers=headers,
+                         params={"rename": ""})
+        return PutBucketRenameOutput(resp)
+
+    def delete_bucket_rename(self, bucket: str):
+        """ 删除桶rename功能
+        :param bucket: 桶名
+        :return: DeleteBucketRenameOutput
+        """
+        resp = self._req(bucket=bucket, method=HttpMethodType.Http_Method_Delete.value, params={"rename": ""})
+        return DeleteBucketRenameOutput(resp)
+
     def _req(self, bucket=None, key=None, method=None, data=None, headers=None, params=None, func=None):
         # 获取调用方法的名称
         func_name = func or traceback.extract_stack()[-2][2]
         exp = None
         info = LogInfo()
         if key is not None:
             _is_valid_object_name(key)
@@ -3082,22 +3244,27 @@
 
         if headers.get('x-tos-content-sha256') is None:
             headers['x-tos-content-sha256'] = UNSIGNED_PAYLOAD
 
         # 通过变量赋值,防止动态调整 auth endpoint 出现并发问题
         auth = self.auth
         endpoint = self.endpoint
-        req = Request(method, self._make_virtual_host_url(bucket, key),
+        req_bucket = None if self.is_custom_domain else bucket
+        req = Request(method, self._make_virtual_host_url(req_bucket, key),
                       _make_virtual_host_uri(key),
-                      _get_virtual_host(bucket, endpoint),
+                      _get_virtual_host(req_bucket, endpoint),
                       data=data,
                       params=params,
                       headers=headers)
 
-        # 若auth 为空即为匿名请求，则计算不签名
+        # 若为网络流对象删除headers中的content-length，防止签名计算错误
+        if isinstance(data, _ReaderAdapter) and headers.get('content-length'):
+            del req.headers['content-length']
+
+        # 若auth 为空即为匿名请求，则不计算签名
         if auth is not None:
             auth.sign_request(req)
 
         # 对于网络流的对象, 删除header中的 host 元素
         # 对于能获取大小的流对象，但size==0, 删除header中的 host 元素
         if isinstance(data, _IterableAdapter) or (isinstance(data, _ReaderAdapter) and data.size == 0):
             del headers['Host']
@@ -3122,15 +3289,15 @@
                                            params=req.params,
                                            stream=True,
                                            timeout=(self.connection_time, self.request_timeout),
                                            verify=self.enable_verify_ssl,
                                            proxies=self.proxies,
                                            allow_redirects=False)
                 rsp = Response(res)
-                if rsp.status >= 300:
+                if rsp.status >= 300 or (rsp.status == 203 and func_name in CALLBACK_FUNCTION):
                     raise exceptions.make_server_error(rsp)
 
                 content_length = get_value(rsp.headers, 'content-length', int)
                 if content_length is not None and content_length == 0:
                     rsp.read()
                 info.success(func_name, rsp)
                 return rsp
```

### Comparing `tos-2.5.7/tos/consts.py` & `tos-2.6.0/tos/consts.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,16 +19,21 @@
                        'abort_multipart_upload', 'set_object_meta', 'put_object_acl', 'delete_object', 'put_object',
                        'upload_part', 'put_bucket_cors', 'delete_bucket_cors', 'put_bucket_storage_class',
                        'put_bucket_lifecycle', 'delete_bucket_lifecycle', 'put_bucket_policy', 'delete_bucket_policy',
                        'put_bucket_mirror_back', 'delete_bucket_mirror_back', 'put_object_tagging',
                        'delete_object_tagging', 'put_bucket_acl', 'put_fetch_task', 'put_bucket_replication',
                        'put_bucket_versioning', 'put_bucket_website', 'delete_bucket_website',
                        'put_bucket_notification', 'put_bucket_custom_domain', 'delete_bucket_custom_domain',
-                       'put_bucket_real_time_log', 'delete_bucket_real_time_log']
+                       'put_bucket_real_time_log', 'delete_bucket_real_time_log', 'restore_object', 'rename_object',
+                       'put_bucket_rename', 'delete_bucket_rename']
 
+CALLBACK_FUNCTION = ['put_object', 'complete_multipart_upload']
 CLIENT_ENCRYPTION_ALGORITHM = ['AES256']
 SERVER_ENCRYPTION_ALGORITHM = ['AES256']
 
 MAX_PART_NUMBER = 10000
 
 MIN_PART_SIZE = 5242880
 MAX_PART_SIZE = 5368709120
+
+MIN_TRAFFIC_LIMIT = 819200
+MAX_TRAFFIC_LIMIT = 838860800
```

### Comparing `tos-2.5.7/tos/convertor.py` & `tos-2.6.0/tos/convertor.py`

 * *Files identical despite different names*

### Comparing `tos-2.5.7/tos/credential.py` & `tos-2.6.0/tos/credential.py`

 * *Files identical despite different names*

### Comparing `tos-2.5.7/tos/enum.py` & `tos-2.6.0/tos/enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,21 @@
 
 class StorageClassType(Enum):
     Storage_Unknown = "Unknown"
     # 标准存储
     Storage_Class_Standard = "STANDARD"
     # 低频访问存储
     Storage_Class_Ia = "IA"
+    Storage_Class_INTELLIGENT_TIERING = "INTELLIGENT_TIERING"
     # 归档闪回存储
     Storage_Class_Archive_Fr = 'ARCHIVE_FR'
+    # 冷归档存储
+    Storage_Class_Cold_Archive = 'COLD_ARCHIVE'
+    # 归档存储
+    Storage_Class_Archive = 'ARCHIVE'
 
 
 def convert_storage_class_type(storage_class: str):
     for t in StorageClassType:
         if t.value == storage_class:
             return t
     return StorageClassType.Storage_Unknown
@@ -227,7 +232,21 @@
     Copy_Event_Create_Multipart_Upload_Succeed = 1
     Copy_Event_Create_Multipart_Upload_Failed = 2
     Copy_Event_Create_Part_Copy_Succeed = 3
     Copy_Event_Create_Part_Copy_Failed = 4
     Copy_Event_Create_Part_Copy_Aborted = 5
     Copy_Event_Completed_Multipart_Upload_Succeed = 6
     Copy_Event_Completed_Multipart_Upload_Failed = 7
+
+
+class TierType(Enum):
+    Tier_Unknown = "Unknown"
+    Tier_Standard = "Standard"
+    Tier_Expedited = "Expedited"
+    Tier_Bulk = "Bulk"
+
+
+def convert_tier_type(s: str):
+    for t in TierType:
+        if t.value == s:
+            return t
+    return TierType.Tier_Unknown
```

### Comparing `tos-2.5.7/tos/exceptions.py` & `tos-2.6.0/tos/exceptions.py`

 * *Files identical despite different names*

### Comparing `tos-2.5.7/tos/http.py` & `tos-2.6.0/tos/http.py`

 * *Files identical despite different names*

### Comparing `tos-2.5.7/tos/json_utils.py` & `tos-2.6.0/tos/json_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .consts import LAST_MODIFY_TIME_DATE_FORMAT
 from .models2 import Owner, RedirectAllRequestsTo, IndexDocument, ErrorDocument, RoutingRules, CustomDomainRule, \
-    RealTimeLogConfiguration
+    RealTimeLogConfiguration, RestoreJobParameters
 from .utils import check_enum_type
 
 
 def to_complete_multipart_upload_request(parts: list):
     dic = {}
     p = []
     for part in parts:
@@ -74,14 +74,18 @@
         info = {}
         if rule.id:
             info['ID'] = rule.id
         if rule.condition:
             info['Condition'] = {}
             if rule.condition.http_code:
                 info['Condition']['HttpCode'] = rule.condition.http_code
+            if rule.condition.key_prefix:
+                info['Condition']['KeyPrefix'] = rule.condition.key_prefix
+            if rule.condition.key_suffix:
+                info['Condition']['KeySuffix'] = rule.condition.key_suffix
         if rule.redirect:
             info['Redirect'] = {}
             if rule.redirect.redirect_type:
                 info['Redirect']['RedirectType'] = rule.redirect.redirect_type.value
             if rule.redirect.fetch_source_on_redirect is not None:
                 info['Redirect']['FetchSourceOnRedirect'] = rule.redirect.fetch_source_on_redirect
             if rule.redirect.public_source:
@@ -90,26 +94,43 @@
                     info['Redirect']['PublicSource']['SourceEndpoint'] = {}
                     if rule.redirect.public_source.source_endpoint.primary:
                         info['Redirect']['PublicSource']['SourceEndpoint'][
                             'Primary'] = rule.redirect.public_source.source_endpoint.primary
                     if rule.redirect.public_source.source_endpoint.follower:
                         info['Redirect']['PublicSource']['SourceEndpoint'][
                             'Follower'] = rule.redirect.public_source.source_endpoint.follower
+                if rule.redirect.public_source.fixed_endpoint is not None:
+                    info['Redirect']['PublicSource']['FixedEndpoint'] = rule.redirect.public_source.fixed_endpoint
             if rule.redirect.pass_query is not None:
                 info['Redirect']['PassQuery'] = rule.redirect.pass_query
             if rule.redirect.follow_redirect is not None:
                 info['Redirect']['FollowRedirect'] = rule.redirect.follow_redirect
             if rule.redirect.mirror_header:
                 info['Redirect']['MirrorHeader'] = {}
                 if rule.redirect.mirror_header.pass_all:
                     info['Redirect']['MirrorHeader']['PassAll'] = rule.redirect.mirror_header.pass_all
                 if rule.redirect.mirror_header.pass_headers:
                     info['Redirect']['MirrorHeader']['Pass'] = rule.redirect.mirror_header.pass_headers
                 if rule.redirect.mirror_header.remove:
                     info['Redirect']['MirrorHeader']['Remove'] = rule.redirect.mirror_header.remove
+            if rule.redirect.transform:
+                info['Redirect']['Transform'] = {}
+                if rule.redirect.transform.with_key_prefix:
+                    info['Redirect']['Transform']['WithKeyPrefix'] = rule.redirect.transform.with_key_prefix
+                if rule.redirect.transform.with_key_suffix:
+                    info['Redirect']['Transform']['WithKeySuffix'] = rule.redirect.transform.with_key_suffix
+                if rule.redirect.transform.replace_key_prefix:
+                    info['Redirect']['Transform']['ReplaceKeyPrefix'] = {}
+                    if rule.redirect.transform.replace_key_prefix.key_prefix:
+                        info['Redirect']['Transform']['ReplaceKeyPrefix'][
+                            'KeyPrefix'] = rule.redirect.transform.replace_key_prefix.key_prefix
+                    if rule.redirect.transform.replace_key_prefix.replace_with:
+                        info['Redirect']['Transform']['ReplaceKeyPrefix'][
+                            'ReplaceWith'] = rule.redirect.transform.replace_key_prefix.replace_with
+
         arr.append(info)
 
     data['Rules'] = arr
 
     return data
 
 
@@ -297,47 +318,70 @@
                     if rule.redirect.replace_key_with:
                         rule_mp['Redirect']['ReplaceKeyWith'] = rule.redirect.replace_key_with
 
                 info['RoutingRules'].append(rule_mp)
     return info
 
 
-def to_put_bucket_notification(cloudFunctionConfigurations: []):
+def to_put_bucket_notification(cloudFunctionConfigurations: [], rocketMQConfigurations: []):
     info = {}
     if cloudFunctionConfigurations:
         info['CloudFunctionConfigurations'] = []
         for cloudFunctionConfiguration in cloudFunctionConfigurations:
             config = {}
             if cloudFunctionConfiguration.events:
                 config['Events'] = cloudFunctionConfiguration.events
             if cloudFunctionConfiguration.id:
                 config['RuleId'] = cloudFunctionConfiguration.id
             if cloudFunctionConfiguration.cloud_function:
                 config['CloudFunction'] = cloudFunctionConfiguration.cloud_function
             if cloudFunctionConfiguration.filter:
-                filter_mp = {}
-                if cloudFunctionConfiguration.filter.key:
-                    filter_mp['TOSKey'] = {}
-                    if cloudFunctionConfiguration.filter.key.rules and len(
-                            cloudFunctionConfiguration.filter.key.rules) >= 1:
-                        filter_mp['TOSKey']['FilterRules'] = []
-                        for rule in cloudFunctionConfiguration.filter.key.rules:
-                            rule_mp = {}
-                            if rule.name:
-                                rule_mp['Name'] = rule.name
-                            if rule.value:
-                                rule_mp['Value'] = rule.value
-                            filter_mp['TOSKey']['FilterRules'].append(rule_mp)
-
-                config['Filter'] = filter_mp
+                config['Filter'] = _get_bucket_notification_filter_map(cloudFunctionConfiguration.filter)
             info['CloudFunctionConfigurations'].append(config)
 
+    if rocketMQConfigurations:
+        info['RocketMQConfigurations'] = []
+        for rocketMQConfiguration in rocketMQConfigurations:
+            config = {}
+            if rocketMQConfiguration.events:
+                config['Events'] = rocketMQConfiguration.events
+            if rocketMQConfiguration.id:
+                config['RuleId'] = rocketMQConfiguration.id
+            if rocketMQConfiguration.role:
+                config['Role'] = rocketMQConfiguration.role
+            if rocketMQConfiguration.rocket_mq:
+                config['RocketMQ'] = {}
+                if rocketMQConfiguration.rocket_mq.topic:
+                    config['RocketMQ']['Topic'] = rocketMQConfiguration.rocket_mq.topic
+                if rocketMQConfiguration.rocket_mq.access_key_id:
+                    config['RocketMQ']['AccessKeyId'] = rocketMQConfiguration.rocket_mq.access_key_id
+                if rocketMQConfiguration.rocket_mq.instance_id:
+                    config['RocketMQ']['InstanceID'] = rocketMQConfiguration.rocket_mq.instance_id
+            if rocketMQConfiguration.filter:
+                config['Filter'] = _get_bucket_notification_filter_map(rocketMQConfiguration.filter)
+            info['RocketMQConfigurations'].append(config)
     return info
 
 
+def _get_bucket_notification_filter_map(filter: {}):
+    filter_mp = {}
+    if filter.key:
+        filter_mp['TOSKey'] = {}
+        if filter.key.rules and len(filter.key.rules) >= 1:
+            filter_mp['TOSKey']['FilterRules'] = []
+            for rule in filter.key.rules:
+                rule_mp = {}
+                if rule.name:
+                    rule_mp['Name'] = rule.name
+                if rule.value:
+                    rule_mp['Value'] = rule.value
+                filter_mp['TOSKey']['FilterRules'].append(rule_mp)
+    return filter_mp
+
+
 def to_put_custom_domain(custom_domain_rule: CustomDomainRule):
     info = {}
     if custom_domain_rule:
         info['CustomDomainRule'] = {}
         if custom_domain_rule.domain:
             info['CustomDomainRule']['Domain'] = custom_domain_rule.domain
         if custom_domain_rule.cname:
@@ -368,7 +412,17 @@
             if configuation.configuration.tls_topic_id:
                 info['RealTimeLogConfiguration']['AccessLogConfiguration'][
                     'TLSTopicID'] = configuation.configuration.tls_topic_id
             if configuation.configuration.tls_project_id:
                 info['RealTimeLogConfiguration']['AccessLogConfiguration'][
                     'TLSProjectID'] = configuation.configuration.tls_project_id
     return info
+
+
+def to_restore_object(days: int, tier: RestoreJobParameters):
+    info = {}
+    if days:
+        info['Days'] = days
+    if tier and tier.tier:
+        info['RestoreJobParameters'] = {"Tier": tier.tier.value}
+
+    return info
```

### Comparing `tos-2.5.7/tos/mine_type.py` & `tos-2.6.0/tos/mine_type.py`

 * *Files identical despite different names*

### Comparing `tos-2.5.7/tos/models.py` & `tos-2.6.0/tos/models.py`

 * *Files identical despite different names*

### Comparing `tos-2.5.7/tos/models2.py` & `tos-2.6.0/tos/models2.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from requests.structures import CaseInsensitiveDict
 
 from . import utils
 from .enum import CannedType, GranteeType, PermissionType, StorageClassType, RedirectType, StatusType, \
     StorageClassInheritDirectiveType, VersioningStatusType, ProtocolType, CertStatus, AzRedundancyType, \
     convert_storage_class_type, convert_az_redundancy_type, convert_permission_type, convert_grantee_type, \
     convert_canned_type, convert_redirect_type, convert_status_type, convert_versioning_status_type, \
-    convert_protocol_type, convert_cert_status
+    convert_protocol_type, convert_cert_status, TierType, convert_tier_type
 from .consts import CHUNK_SIZE
 from .exceptions import TosClientError, make_server_error_with_exception
 from .models import CommonPrefixInfo, DeleteMarkerInfo
 from .utils import (get_etag, get_value, meta_header_decode,
                     parse_gmt_time_to_utc_datetime,
                     parse_modify_time_to_utc_datetime, _param_to_quoted_query, _make_virtual_host_url)
 
@@ -87,21 +87,23 @@
                 get_value(bkt, 'Location'),
                 get_value(bkt, 'CreationDate'),
                 get_value(bkt, 'ExtranetEndpoint'),
                 get_value(bkt, 'IntranetEndpoint')))
 
 
 class PutObjectOutput(ResponseInfo):
-    def __init__(self, resp):
+    def __init__(self, resp, callback=None):
         super(PutObjectOutput, self).__init__(resp)
         self.etag = get_etag(resp.headers)
         self.ssec_algorithm = get_value(resp.headers, "x-tos-server-side-encryption-customer-algorithm")
         self.ssec_key_md5 = get_value(resp.headers, "x-tos-server-side-encryption-customer-key-md5")
         self.version_id = get_value(resp.headers, "x-tos-version-id")
         self.hash_crc64_ecma = get_value(resp.headers, "x-tos-hash-crc64ecma", lambda x: int(x))
+        if callback:
+            self.callback_result = resp.read().decode("utf-8")
 
 
 class CopyObjectOutput(ResponseInfo):
     def __init__(self, resp):
         super(CopyObjectOutput, self).__init__(resp)
         self.copy_source_version_id = get_value(resp.headers, "x-tos-copy-source-version-id")
         self.version_id = get_value(resp.headers, "x-tos-version-id")
@@ -196,14 +198,17 @@
         self.etag = get_etag(resp.headers)
         self.version_id = get_value(resp.headers, "x-tos-version-id")
         self.sse_algorithm = get_value(resp.headers, "x-tos-server-side-encryption-customer-algorithm")
         self.sse_key_md5 = get_value(resp.headers, "x-tos-server-side-encryption-customer-key-MD5")
         self.website_redirect_location = get_value(resp.headers, "x-tos-website-redirect-location")
         self.hash_crc64_ecma = get_value(resp.headers, "x-tos-hash-crc64ecma", lambda x: int(x))
         self.storage_class = get_value(resp.headers, "x-tos-storage-class", lambda x: convert_storage_class_type(x))
+        self.restore = get_value(resp.headers, "x-tos-restore")
+        self.restore_expiry_days = get_value(resp.headers, "x-tos-restore-expiry-days", lambda x: int(x))
+        self.restore_tier = get_value(resp.headers, "x-tos-restore-tier", lambda x: convert_tier_type(x))
         self.meta = CaseInsensitiveDict()
         self.object_type = get_value(resp.headers, "x-tos-object-type")
         if not self.object_type:
             self.object_type = "Normal"
 
         meta = {}
         for k in resp.headers:
@@ -623,24 +628,45 @@
         self.part_number = number
         self.etag = get_etag(resp.headers)
         self.ssec_algorithm = get_value(resp.headers, 'x-tos-server-side-encryption-customer-algorithm')
         self.ssec_key_md5 = get_value(resp.headers, 'x-tos-server-side-encryption-customer-key-md5')
         self.hash_crc64_ecma = get_value(resp.headers, 'x-tos-hash-crc64ecma', lambda x: int(x))
 
 
+class CompletePart(object):
+    def __init__(self, etag, part_number):
+        self.etag = etag
+        self.part_number = part_number
+
+
 class CompleteMultipartUploadOutput(ResponseInfo):
-    def __init__(self, resp):
+    def __init__(self, resp, callback: str = None):
         super(CompleteMultipartUploadOutput, self).__init__(resp)
-        data = resp.json_read()
-        self.bucket = get_value(data, 'Bucket')
-        self.key = get_value(data, 'Key')
-        self.etag = get_etag(data)
-        self.location = get_value(data, 'Location')
+        self.bucket = None
+        self.key = None
+        self.complete_parts = []
+        self.callback_result = None
         self.version_id = get_value(resp.headers, 'x-tos-version-id')
         self.hash_crc64_ecma = get_value(resp.headers, 'x-tos-hash-crc64ecma', lambda x: int(x))
+        if not callback:
+            data = resp.json_read()
+            self.bucket = get_value(data, 'Bucket')
+            self.key = get_value(data, 'Key')
+            self.etag = get_etag(data)
+            self.location = get_value(data, 'Location')
+            complete_part_info = get_value(data, 'CompletedParts') or []
+            for part in complete_part_info:
+                self.complete_parts.append(CompletePart(
+                    etag=get_value(part, 'ETag'),
+                    part_number=get_value(part, 'PartNumber')
+                ))
+        else:
+            self.callback_result = resp.read().decode('utf-8')
+            self.etag = get_etag(resp.headers)
+            self.location = get_value(resp.headers, 'Location')
 
 
 class AbortMultipartUpload(ResponseInfo):
     def __init__(self, resp):
         super(AbortMultipartUpload, self).__init__(resp)
 
 
@@ -785,46 +811,64 @@
 
 class DeleteBucketCorsOutput(ResponseInfo):
     def __init__(self, resp):
         super(DeleteBucketCorsOutput, self).__init__(resp)
 
 
 class Condition(object):
-    def __init__(self, http_code: int = None):
+    def __init__(self, http_code: int = None, key_prefix: str = None, key_suffix: str = None):
         self.http_code = http_code
+        self.key_prefix = key_prefix
+        self.key_suffix = key_suffix
+
+
+class ReplaceKeyPrefix(object):
+    def __init__(self, key_prefix: str = None, replace_with: str = None):
+        self.key_prefix = key_prefix
+        self.replace_with = replace_with
+
+
+class Transform(object):
+    def __init__(self, with_key_prefix: str = None, with_key_suffix: str = None,
+                 replace_key_prefix: ReplaceKeyPrefix = None):
+        self.with_key_prefix = with_key_prefix
+        self.with_key_suffix = with_key_suffix
+        self.replace_key_prefix = replace_key_prefix
 
 
 class SourceEndpoint(object):
     def __init__(self, primary: [] = None, follower: [] = None):
         self.primary = primary
         self.follower = follower
 
 
 class PublicSource(object):
-    def __init__(self, source_endpoint: SourceEndpoint):
+    def __init__(self, source_endpoint: SourceEndpoint = None, fixed_endpoint: bool = None):
         self.source_endpoint = source_endpoint
+        self.fixed_endpoint = fixed_endpoint
 
 
 class MirrorHeader(object):
     def __init__(self, pass_all: bool = None, pass_headers: [] = None, remove: [] = None):
         self.pass_all = pass_all
         self.pass_headers = pass_headers
         self.remove = remove
 
 
 class Redirect(object):
     def __init__(self, redirect_type: RedirectType = None, public_source: PublicSource = None,
                  fetch_source_on_redirect: bool = None, pass_query: bool = None, follow_redirect: bool = None,
-                 mirror_header: MirrorHeader = None):
+                 mirror_header: MirrorHeader = None, transform: Transform = None):
         self.redirect_type = redirect_type
         self.fetch_source_on_redirect = fetch_source_on_redirect
         self.public_source = public_source
         self.pass_query = pass_query
         self.follow_redirect = follow_redirect
         self.mirror_header = mirror_header
+        self.transform = transform
 
 
 class Rule(object):
     def __init__(self, id: str = None, condition: Condition = None, redirect: Redirect = None):
         self.id = id
         self.condition = condition
         self.redirect = redirect
@@ -1064,15 +1108,16 @@
                     tr.non_current_days = get_value(vt, 'NoncurrentDays', int)
                     rule.non_current_version_transitions.append(tr)
 
             if transitions_json:
                 rule.transitions = []
                 for transition_json in transitions_json:
                     ts = BucketLifeCycleTransition()
-                    ts.storage_class = get_value(transition_json, 'StorageClass', lambda x: convert_storage_class_type(x))
+                    ts.storage_class = get_value(transition_json, 'StorageClass',
+                                                 lambda x: convert_storage_class_type(x))
                     ts.days = get_value(transition_json, 'Days', int)
                     if get_value(transition_json, 'Date'):
                         ts.date = parse_modify_time_to_utc_datetime(get_value(transition_json, 'Date'))
                     rule.transitions.append(ts)
 
             if tags_json:
                 rule.tags = []
@@ -1126,35 +1171,51 @@
             id = get_value(rule, 'ID')
             cond = get_value(rule, 'Condition')
             condition = None
             red = get_value(rule, 'Redirect')
             redirect = None
             if cond:
                 condition = Condition(
-                    http_code=get_value(cond, 'HttpCode', int)
+                    http_code=get_value(cond, 'HttpCode', int),
+                    key_prefix=get_value(cond, 'KeyPrefix', str),
+                    key_suffix=get_value(cond, 'KeySuffix', str)
                 )
             if red:
                 redirect = Redirect()
                 redirect.redirect_type = get_value(red, 'RedirectType', lambda x: convert_redirect_type(x))
                 redirect.fetch_source_on_redirect = get_value(red, 'FetchSourceOnRedirect', lambda x: bool(x))
 
-                if get_value(red, 'PublicSource') and get_value(get_value(red, 'PublicSource'), 'SourceEndpoint'):
-                    redirect.public_source = PublicSource(SourceEndpoint(
-                        primary=get_value(get_value(get_value(red, 'PublicSource'), 'SourceEndpoint'), 'Primary'),
-                        follower=get_value(get_value(get_value(red, 'PublicSource'), 'SourceEndpoint'), 'Follower')
-                    ))
-
+                if get_value(red, 'PublicSource'):
+                    redirect.public_source = PublicSource(
+                        fixed_endpoint=get_value(get_value(red, 'PublicSource'), 'FixedEndpoint', lambda x: bool(x)))
+                    if get_value(get_value(red, 'PublicSource'), 'SourceEndpoint'):
+                        redirect.public_source.source_endpoint = SourceEndpoint(
+                            primary=get_value(get_value(get_value(red, 'PublicSource'), 'SourceEndpoint'), 'Primary'),
+                            follower=get_value(get_value(get_value(red, 'PublicSource'), 'SourceEndpoint'), 'Follower')
+                        )
                 redirect.pass_query = get_value(red, 'PassQuery', lambda x: bool(x))
                 redirect.follow_redirect = get_value(red, 'FollowRedirect', lambda x: bool(x))
                 if get_value(red, 'MirrorHeader'):
                     redirect.mirror_header = MirrorHeader(
                         pass_all=get_value(get_value(red, 'MirrorHeader'), 'PassAll', lambda x: bool(x)),
                         pass_headers=get_value(get_value(red, 'MirrorHeader'), 'Pass'),
                         remove=get_value(get_value(red, 'MirrorHeader'), 'Remove')
                     )
+                if get_value(red, 'Transform'):
+                    redirect.transform = Transform(
+                        with_key_prefix=get_value(get_value(red, 'Transform'), 'WithKeyPrefix'),
+                        with_key_suffix=get_value(get_value(red, 'Transform'), 'WithKeySuffix'),
+                    )
+                    if get_value(get_value(red, 'Transform'), 'ReplaceKeyPrefix'):
+                        redirect.transform.replace_key_prefix = ReplaceKeyPrefix(
+                            key_prefix=get_value(get_value(get_value(red, 'Transform'), 'ReplaceKeyPrefix'),
+                                                 'KeyPrefix'),
+                            replace_with=get_value(get_value(get_value(red, 'Transform'), 'ReplaceKeyPrefix'),
+                                                   'ReplaceWith')
+                        )
                 r = Rule(id=id, condition=condition, redirect=redirect)
                 self.rules.append(r)
 
 
 class PutObjectTaggingOutput(ResponseInfo):
     def __init__(self, resp):
         super(PutObjectTaggingOutput, self).__init__(resp)
@@ -1423,19 +1484,20 @@
             condition = get_value(rule_json, 'Condition')
             redirect = get_value(rule_json, 'Redirect')
             if condition:
                 rule.condition = RoutingRuleCondition(
                     http_error_code_returned_equals=get_value(condition, 'HttpErrorCodeReturnedEquals'),
                     key_prefix_equals=get_value(condition, 'KeyPrefixEquals'))
             if redirect:
-                rule.redirect = RoutingRuleRedirect(protocol=get_value(redirect, 'Protocol', lambda x: convert_protocol_type(x)),
-                                                    host_name=get_value(redirect, 'HostName'),
-                                                    replace_key_prefix_with=get_value(redirect, 'ReplaceKeyPrefixWith'),
-                                                    replace_key_with=get_value(redirect, 'ReplaceKeyWith'),
-                                                    http_redirect_code=get_value(redirect, 'HttpRedirectCode'))
+                rule.redirect = RoutingRuleRedirect(
+                    protocol=get_value(redirect, 'Protocol', lambda x: convert_protocol_type(x)),
+                    host_name=get_value(redirect, 'HostName'),
+                    replace_key_prefix_with=get_value(redirect, 'ReplaceKeyPrefixWith'),
+                    replace_key_with=get_value(redirect, 'ReplaceKeyWith'),
+                    http_redirect_code=get_value(redirect, 'HttpRedirectCode'))
             self.routing_rules.append(rule)
 
 
 class FilterRule(object):
     def __init__(self, name: str = None, value: str = None):
         self.name = name
         self.value = value
@@ -1447,50 +1509,91 @@
 
 
 class Filter(object):
     def __init__(self, key: FilterKey):
         self.key = key
 
 
+class RocketMQConf(object):
+    def __init__(self, instance_id: str = None, topic: str = None, access_key_id: str = None):
+        self.instance_id = instance_id
+        self.topic = topic
+        self.access_key_id = access_key_id
+
+
 class CloudFunctionConfiguration(object):
     def __init__(self, id: str = None, events: [] = None, filter: Filter = None, cloud_function: str = None):
         self.id = id
         self.events = events
         self.filter = filter
         self.cloud_function = cloud_function
 
 
+class RocketMQConfiguration(object):
+    def __init__(self, id: str = None, events: [] = None, filter: Filter = None, role: str = None,
+                 rocket_mq: RocketMQConf = None):
+        self.id = id
+        self.events = events
+        self.filter = filter
+        self.role = role
+        self.rocket_mq = rocket_mq
+
+
 class PutBucketNotificationOutput(ResponseInfo):
     def __init__(self, resp):
         super(PutBucketNotificationOutput, self).__init__(resp)
 
 
 class GetBucketNotificationOutput(ResponseInfo):
     def __init__(self, resp):
         super(GetBucketNotificationOutput, self).__init__(resp)
         data = resp.json_read()
         self.cloud_function_configurations = []
+        self.rocket_mq_configurations = []
         cloud_functions = get_value(data, 'CloudFunctionConfigurations') or []
+        rocket_mq_confs = get_value(data, 'RocketMQConfigurations') or []
         for function in cloud_functions:
             config = CloudFunctionConfiguration()
             config.id = get_value(function, 'RuleId')
             config.events = get_value(function, 'Events')
             config.cloud_function = get_value(function, 'CloudFunction')
             filter_json = get_value(function, 'Filter')
             if filter_json:
-                fileter_key = FilterKey([])
-                key_json = get_value(filter_json, 'TOSKey')
-                if key_json:
-                    filter_rules = get_value(key_json, 'FilterRules') or []
-                    for rule in filter_rules:
-                        fileter_key.rules.append(
-                            FilterRule(name=get_value(rule, 'Name'), value=get_value(rule, 'Value')))
-                    config.filter = Filter(fileter_key)
+                config.filter = self._get_filter(filter_json)
             self.cloud_function_configurations.append(config)
 
+        for rocket_mq_conf in rocket_mq_confs:
+            config = RocketMQConfiguration()
+            config.id = get_value(rocket_mq_conf, 'RuleId')
+            config.events = get_value(rocket_mq_conf, 'Events')
+            config.role = get_value(rocket_mq_conf, 'Role')
+            rocket_mq_json = get_value(rocket_mq_conf, 'RocketMQ')
+            if rocket_mq_json:
+                rocket_mq = RocketMQConf(
+                    instance_id=get_value(rocket_mq_json, 'InstanceId'),
+                    topic=get_value(rocket_mq_json, 'Topic'),
+                    access_key_id=get_value(rocket_mq_json, 'AccessKeyId'),
+                )
+                config.rocket_mq = rocket_mq
+            filter_json = get_value(rocket_mq_conf, 'Filter')
+            if filter_json:
+                config.filter = self._get_filter(filter_json)
+            self.rocket_mq_configurations.append(config)
+
+    @staticmethod
+    def _get_filter(filter_json):
+        filter_key = FilterKey([])
+        key_json = get_value(filter_json, 'TOSKey')
+        if key_json:
+            filter_rules = get_value(key_json, 'FilterRules') or []
+            for rule in filter_rules:
+                filter_key.rules.append(
+                    FilterRule(name=get_value(rule, 'Name'), value=get_value(rule, 'Value')))
+        return Filter(filter_key)
+
 
 class CustomDomainRule(object):
     def __init__(self, cert_id: str = None, cert_status: CertStatus = None, domain: str = None, cname: str = None,
                  forbidden: bool = None, forbidden_reason: str = None):
         self.cert_id = cert_id
         self.cert_status = cert_status
         self.domain = domain
@@ -1513,15 +1616,16 @@
         for custom_domain_rule in custom_domain_rules:
             self.rules.append(
                 CustomDomainRule(cert_id=get_value(custom_domain_rule, 'CertId'),
                                  domain=get_value(custom_domain_rule, 'Domain'),
                                  cname=get_value(custom_domain_rule, 'Cname'),
                                  forbidden=get_value(custom_domain_rule, 'Forbidden'),
                                  forbidden_reason=get_value(custom_domain_rule, 'ForbiddenReason'),
-                                 cert_status=get_value(custom_domain_rule, 'CertStatus', lambda x: convert_cert_status(x))))
+                                 cert_status=get_value(custom_domain_rule, 'CertStatus',
+                                                       lambda x: convert_cert_status(x))))
 
 
 class DeleteCustomDomainOutput(ResponseInfo):
     def __init__(self, resp):
         super(DeleteCustomDomainOutput, self).__init__(resp)
 
 
@@ -1588,22 +1692,24 @@
         self._scheme = scheme
         self._bucket = bucket
 
     def get_signed_url_for_list(self, additional_query=None) -> str:
         if additional_query is None:
             return _make_virtual_host_url(self._host, self._scheme, self._bucket, '') + '?' + self.signed_query
 
-        return _make_virtual_host_url(self._host, self._scheme, self._bucket, '') + '?' + self.signed_query + '&' + '&'.join(
+        return _make_virtual_host_url(self._host, self._scheme, self._bucket,
+                                      '') + '?' + self.signed_query + '&' + '&'.join(
             _param_to_quoted_query(k, v) for k, v in additional_query.items())
 
     def get_signed_url_for_get_or_head(self, key: str, additional_query=None) -> str:
         if additional_query is None:
             return _make_virtual_host_url(self._host, self._scheme, self._bucket, key) + '?' + self.signed_query
 
-        return _make_virtual_host_url(self._host, self._scheme, self._bucket, key) + '?' + self.signed_query + '&' + '&'.join(
+        return _make_virtual_host_url(self._host, self._scheme, self._bucket,
+                                      key) + '?' + self.signed_query + '&' + '&'.join(
             _param_to_quoted_query(k, v) for k, v in additional_query.items())
 
 
 class CopyPartInfo(object):
     def __init__(self, part_number, copy_source_range_start, copy_source_range_end, etag=None):
         self.part_number = part_number
         self.copy_source_range_start = copy_source_range_start
@@ -1612,7 +1718,39 @@
 
     def __str__(self):
         info = {'part_number': self.part_number,
                 'copy_source_range_start': self.copy_source_range_start,
                 'copy_source_range_end': self.copy_source_range_end,
                 'etag': self.etag}
         return str(info)
+
+
+class RestoreJobParameters(object):
+    def __init__(self, tier: TierType):
+        self.tier = tier
+
+
+class RestoreObjectOutput(ResponseInfo):
+    def __init__(self, resp):
+        super(RestoreObjectOutput, self).__init__(resp)
+
+
+class RenameObjectOutput(ResponseInfo):
+    def __init__(self, resp):
+        super(RenameObjectOutput, self).__init__(resp)
+
+
+class GetBucketRenameOutput(ResponseInfo):
+    def __init__(self, resp):
+        super(GetBucketRenameOutput, self).__init__(resp)
+        data = resp.json_read()
+        self.rename_enable = get_value(data, 'RenameEnable', bool)
+
+
+class PutBucketRenameOutput(ResponseInfo):
+    def __init__(self, resp):
+        super(PutBucketRenameOutput, self).__init__(resp)
+
+
+class DeleteBucketRenameOutput(ResponseInfo):
+    def __init__(self, resp):
+        super(DeleteBucketRenameOutput, self).__init__(resp)
```

### Comparing `tos-2.5.7/tos/utils.py` & `tos-2.6.0/tos/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pytz
 import six
 from pytz import unicode
 
 from .consts import (DEFAULT_MIMETYPE, GMT_DATE_FORMAT,
                      MAX_PART_NUMBER, MAX_PART_SIZE, MIN_PART_SIZE, CHUNK_SIZE,
                      CLIENT_ENCRYPTION_ALGORITHM, SERVER_ENCRYPTION_ALGORITHM, LAST_MODIFY_TIME_DATE_FORMAT,
-                     EMPTY_SHA256_HASH, PAYLOAD_BUFFER)
+                     EMPTY_SHA256_HASH, PAYLOAD_BUFFER, MIN_TRAFFIC_LIMIT, MAX_TRAFFIC_LIMIT)
 from .enum import DataTransferType, ACLType, StorageClassType, MetadataDirectiveType, AzRedundancyType, PermissionType, \
     GranteeType, CannedType
 from .exceptions import TosClientError
 from .mine_type import TYPES_MAP
 
 logger = logging.getLogger(__name__)
 REGION_MAP = {'cn-beijing': 'tos-cn-beijing.volces.com', 'cn-guangzhou': 'tos-cn-guangzhou.volces.com',
@@ -232,15 +232,15 @@
         if self.can_reset:
             self.offset = 0
             if self.init_offset is not None:
                 self.file_object.seek(self.init_offset, os.SEEK_SET)
 
 
 def meta_header_encode(query, doseq=False, safe='', encoding=None, errors=None,
-                       quote_via=quote_plus):
+                       quote_via=quote):
     headers = {}
     if hasattr(query, "items"):
         query = query.items()
     else:
         # It's a bother at times that strings and string-like objects are
         # sequences.
         try:
```

### Comparing `tos-2.5.7/tos.egg-info/PKG-INFO` & `tos-2.6.0/tos.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,96 @@
 Metadata-Version: 2.1
 Name: tos
-Version: 2.5.7
+Version: 2.6.0
 Summary: Volc TOS (Tinder Object Storage) SDK
 Home-page: https://www.volcengine.com/
 Author: sunyushan
 Author-email: sunyushan.jason@bytedance.com
 License: UNKNOWN
+Description: 
+        # Volcengine TOS SDK for Python
+        The TOS Python SDK enables Python developers to easily work with TOS(Tinder Object Storage) service in the volcengine.
+        This document will show developers some basic examples about TOS bucket and object operation.
+        
+        
+        ## Install
+        ### Requirements
+        - Python3
+        # Quick Start
+        
+        This section introduces how to create a bucket, upload/download/delete an object in TOS service through our SDK.
+        
+        ## Create a TOS Client
+        
+        You can interact with TOS service after initiating a TOSClient instance.
+        The accesskey and secretkey of your account, endpoint and region are required as params.
+        
+        ```python
+        import tos
+        
+        ak = "your access key"
+        sk = "your secret key"
+        endpoint = "your endpoint"
+        region = "your region"
+        bucket_name = "your bucket name"
+        object_key = "your object key"
+        client = tos.TosClientV2(ak, sk, endpoint, region)     
+        ```
+        
+        ## Create a bucket
+        
+        The bucket is a kind of unique namespace in TOS, which is a container to store data.
+        This example shows you how to create a bucket.
+        
+        ```python
+        import tos
+        
+        ak = "your access key"
+        sk = "your secret key"
+        endpoint = "your endpoint"
+        region = "your region"
+        bucket_name = "your bucket name"
+        client = tos.TosClientV2(ak, sk, endpoint, region)
+        client.create_bucket(bucket_name)                            
+        ```
+        
+        ## Put Object
+        
+        You can put your file as an object into your own bucket.
+        
+        ```python
+        # call put_object to upload you data to the TOS                     
+        client.put_object(bucket_name, object_key, content="123")
+        assert resp.status == 200       
+        ```
+        ## Get Object
+        You can download objects in the TOS bucket through our SDK.
+        
+        ```python
+        # call get_object to download your data from your bucket
+        client.get_object(bucket_name, object_key)
+        ```
+        
+        ## Delete Object
+        
+        Your can delete your objects in the bucket：
+        
+        ```python
+        # call put_object to upload you data to the TOS  
+        resp = client.put_object(bucket_name, key_name, content="123")
+        assert resp.status_code == 200   
+        # call delete_object to delete an object in your bucket
+        resp = client.delete_object(bucket_name, key_name)
+        assert resp.status_code == 204
+        ```
+        
+        ## License
+        [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html)
 Keywords: boilerplate
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# Volcengine TOS SDK for Python
-The TOS Python SDK enables Python developers to easily work with TOS(Tinder Object Storage) service in the volcengine.
-This document will show developers some basic examples about TOS bucket and object operation.
-
-
-## Install
-### Requirements
-- Python3
-# Quick Start
-
-This section introduces how to create a bucket, upload/download/delete an object in TOS service through our SDK.
-
-## Create a TOS Client
-
-You can interact with TOS service after initiating a TOSClient instance.
-The accesskey and secretkey of your account, endpoint and region are required as params.
-
-```python
-import tos
-
-ak = "your access key"
-sk = "your secret key"
-endpoint = "your endpoint"
-region = "your region"
-bucket_name = "your bucket name"
-object_key = "your object key"
-client = tos.TosClientV2(ak, sk, endpoint, region)     
-```
-
-## Create a bucket
-
-The bucket is a kind of unique namespace in TOS, which is a container to store data.
-This example shows you how to create a bucket.
-
-```python
-import tos
-
-ak = "your access key"
-sk = "your secret key"
-endpoint = "your endpoint"
-region = "your region"
-bucket_name = "your bucket name"
-client = tos.TosClientV2(ak, sk, endpoint, region)
-client.create_bucket(bucket_name)                            
-```
-
-## Put Object
-
-You can put your file as an object into your own bucket.
-
-```python
-# call put_object to upload you data to the TOS                     
-client.put_object(bucket_name, object_key, content="123")
-assert resp.status == 200       
-```
-## Get Object
-You can download objects in the TOS bucket through our SDK.
-
-```python
-# call get_object to download your data from your bucket
-client.get_object(bucket_name, object_key)
-```
-
-## Delete Object
-
-Your can delete your objects in the bucket：
-
-```python
-# call put_object to upload you data to the TOS  
-resp = client.put_object(bucket_name, key_name, content="123")
-assert resp.status_code == 200   
-# call delete_object to delete an object in your bucket
-resp = client.delete_object(bucket_name, key_name)
-assert resp.status_code == 204
-```
-
-## License
-[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html)
-
```

