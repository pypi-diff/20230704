# Comparing `tmp/cloudstorageio-1.2.8.tar.gz` & `tmp/cloudstorageio-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudstorageio-1.2.8.tar", last modified: Thu May  4 17:24:29 2023, max compression
+gzip compressed data, was "cloudstorageio-1.2.9.tar", last modified: Fri May  5 12:14:39 2023, max compression
```

## Comparing `cloudstorageio-1.2.8.tar` & `cloudstorageio-1.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1905 2023-05-04 17:16:09.000000 cloudstorageio-1.2.8/CHANGELOG.md
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1068 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/LICENSE
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5430 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3516 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/README.md
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      220 2023-05-04 17:16:20.000000 cloudstorageio-1.2.8/cloudstorageio/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/configs/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       64 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/configs/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      401 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/configs/configs.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/configs/resources/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/configs/resources/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/enums/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       40 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/enums/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      142 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/enums/enums.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio/exceptions/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       50 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/exceptions/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      196 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/exceptions/exceptions.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/cloudstorageio/interface/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      336 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6654 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/async_cloud.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    12492 2023-05-04 16:51:03.000000 cloudstorageio-1.2.8/cloudstorageio/interface/cloud_interface.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9405 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/drop_box.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    10673 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/google_drive.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9094 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/interface/google_storage.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5535 2023-05-04 16:51:03.000000 cloudstorageio-1.2.8/cloudstorageio/interface/local_storage.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    12626 2023-05-04 17:15:23.000000 cloudstorageio-1.2.8/cloudstorageio/interface/s3.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/cloudstorageio/log/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/log/__init__.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/cloudstorageio/tools/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1033 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/ci_collections.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2951 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/decorators.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      236 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/cloudstorageio/tools/logger.py
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.110721 cloudstorageio-1.2.8/cloudstorageio.egg-info/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5430 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/PKG-INFO
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1045 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/SOURCES.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/dependency_links.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       72 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/requires.txt
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       20 2023-05-04 17:24:29.000000 cloudstorageio-1.2.8/cloudstorageio.egg-info/top_level.txt
-drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/docs/
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/docs/__init__.py
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      792 2022-11-15 07:45:02.000000 cloudstorageio-1.2.8/docs/additional_docs.md
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      725 2023-05-04 17:24:29.114721 cloudstorageio-1.2.8/setup.cfg
--rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       38 2023-05-04 17:14:38.000000 cloudstorageio-1.2.8/setup.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.810422 cloudstorageio-1.2.9/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2043 2023-05-05 10:20:34.000000 cloudstorageio-1.2.9/CHANGELOG.md
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1068 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/LICENSE
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5566 2023-05-05 12:14:39.810422 cloudstorageio-1.2.9/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     3516 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/README.md
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      299 2023-05-05 10:20:00.000000 cloudstorageio-1.2.9/cloudstorageio/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/configs/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      101 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/configs/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      401 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/cloudstorageio/configs/configs.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/configs/resources/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/cloudstorageio/configs/resources/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/enums/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       79 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/enums/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      267 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/enums/enums.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/exceptions/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      111 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/exceptions/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      201 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/exceptions/exceptions.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/interface/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      478 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6715 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/async_cloud.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    13828 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/cloud_interface.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9908 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/drop_box.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    11194 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/google_drive.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     9238 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/google_storage.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     6405 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/local_storage.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)    14627 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/interface/s3.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/log/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/cloudstorageio/log/__init__.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio/tools/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/cloudstorageio/tools/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1034 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/tools/ci_collections.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     2994 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/tools/decorators.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      254 2023-05-05 10:12:58.000000 cloudstorageio-1.2.9/cloudstorageio/tools/logger.py
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.806422 cloudstorageio-1.2.9/cloudstorageio.egg-info/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     5566 2023-05-05 12:14:39.000000 cloudstorageio-1.2.9/cloudstorageio.egg-info/PKG-INFO
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)     1045 2023-05-05 12:14:39.000000 cloudstorageio-1.2.9/cloudstorageio.egg-info/SOURCES.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        1 2023-05-05 12:14:39.000000 cloudstorageio-1.2.9/cloudstorageio.egg-info/dependency_links.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       72 2023-05-05 12:14:39.000000 cloudstorageio-1.2.9/cloudstorageio.egg-info/requires.txt
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       20 2023-05-05 12:14:39.000000 cloudstorageio-1.2.9/cloudstorageio.egg-info/top_level.txt
+drwxrwxr-x   0 atlantx   (1000) atlantx   (1000)        0 2023-05-05 12:14:39.810422 cloudstorageio-1.2.9/docs/
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)        0 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/docs/__init__.py
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      792 2022-11-15 07:45:02.000000 cloudstorageio-1.2.9/docs/additional_docs.md
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)      725 2023-05-05 12:14:39.810422 cloudstorageio-1.2.9/setup.cfg
+-rw-rw-r--   0 atlantx   (1000) atlantx   (1000)       38 2023-05-05 08:34:36.000000 cloudstorageio-1.2.9/setup.py
```

### Comparing `cloudstorageio-1.2.8/CHANGELOG.md` & `cloudstorageio-1.2.9/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -61,7 +61,11 @@
 ### [1.2.4] - 2020-11-10
 - Add option include_files for listdir
 ### [1.2.7] - 2022-10-05
 - Updated build to setuptools
 ### [1.2.8] - 2022-05-04
 - Fix error on listdir for s3 if the folder did not include subfolders
 - Add option include_files for listdir for non-recursive case
+### [1.2.9] - 2022-05-05
+- Add github workflows for merging
+- Update tests to use AWS mocker
+- Move moto dependency to dev-requirements
```

### Comparing `cloudstorageio-1.2.8/LICENSE` & `cloudstorageio-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.8/PKG-INFO` & `cloudstorageio-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstorageio
-Version: 1.2.8
+Version: 1.2.9
 Home-page: https://github.com/cognaize/cloudstorageio
 Author: cognaize
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cloudstorageio
 
@@ -187,7 +187,11 @@
 ### [1.2.4] - 2020-11-10
 - Add option include_files for listdir
 ### [1.2.7] - 2022-10-05
 - Updated build to setuptools
 ### [1.2.8] - 2022-05-04
 - Fix error on listdir for s3 if the folder did not include subfolders
 - Add option include_files for listdir for non-recursive case
+### [1.2.9] - 2022-05-05
+- Add github workflows for merging
+- Update tests to use AWS mocker
+- Move moto dependency to dev-requirements
```

### Comparing `cloudstorageio-1.2.8/README.md` & `cloudstorageio-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.8/cloudstorageio/interface/async_cloud.py` & `cloudstorageio-1.2.9/cloudstorageio/interface/async_cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,101 @@
-import functools
 import itertools
-import multiprocessing
 import os
 import queue
-from multiprocessing.pool import Pool
-
-from typing import Optional
 from threading import Thread
+from typing import Optional
+
 from cloudstorageio.interface.cloud_interface import CloudInterface
-from cloudstorageio.tools.decorators import timer
 from cloudstorageio.tools.logger import logger
 
 
 class AsyncCloudInterface:
 
-    def __init__(self, aws_region_name: Optional[str] = None, aws_access_key_id: Optional[str] = None,
-                 aws_secret_access_key: Optional[str] = None, dropbox_token: Optional[str] = None,
-                 dropbox_root: Optional[bool] = False, google_cloud_credentials_path: Optional[str] = None,
-                 google_drive_credentials_path: Optional[str] = None, **kwargs):
+    def __init__(self, aws_region_name: Optional[str] = None,
+                 aws_access_key_id: Optional[str] = None,
+                 aws_secret_access_key: Optional[str] = None,
+                 dropbox_token: Optional[str] = None,
+                 dropbox_root: Optional[bool] = False,
+                 google_cloud_credentials_path: Optional[str] = None,
+                 google_drive_credentials_path: Optional[str] = None,
+                 **kwargs):
 
         """Initializes AsyncCloudInterface instance
         :param aws_region_name: region name for S3 storage
         :param aws_access_key_id: access key id for S3 storage
         :param aws_secret_access_key: secret access key for S3 storage
         :param dropbox_token: generated token for dropbox app access
-        :param google_cloud_credentials_path: local path of google cloud credentials file (json)
-        :param google_drive_credentials_path: local path of google drive secret credentials file (json)
+        :param google_cloud_credentials_path: local path of
+         google cloud credentials file (json)
+        :param google_drive_credentials_path: local path of
+         Google Drive secret credentials file (json)
         :param kwargs:
         """
 
         self._kwargs = kwargs
         self.aws_region_name = aws_region_name
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.dropbox_token = dropbox_token
         self.dropbox_root = dropbox_root
-        self.google_cloud_credentials_path = google_cloud_credentials_path
-        self.google_drive_credentials_path = google_drive_credentials_path
+        self.google_cloud_creds_path = google_cloud_credentials_path
+        self.google_drive_creds_path = google_drive_credentials_path
 
-    def read_files(self, file_path_list: list, q: queue.Queue, from_folder_path: str):
+    def read_files(self, file_path_list: list, q: queue.Queue,
+                   from_folder_path: str):
         """Reads given files and put content in given queue
         :param file_path_list: list of files' path
         :param q: queue which contains file path and file content
         :param from_folder_path: folder path of files to read
         :return:
         """
-        ci = CloudInterface(aws_region_name=self.aws_region_name, aws_access_key_id=self.aws_access_key_id,
-                            aws_secret_access_key=self.aws_secret_access_key, dropbox_token=self.dropbox_token,
-                            dropbox_root=self.dropbox_root,
-                            google_cloud_credentials_path=self.google_cloud_credentials_path,
-                            google_drive_credentials_path=self.google_drive_credentials_path)
+        ci = CloudInterface(
+            aws_region_name=self.aws_region_name,
+            aws_access_key_id=self.aws_access_key_id,
+            aws_secret_access_key=self.aws_secret_access_key,
+            dropbox_token=self.dropbox_token,
+            dropbox_root=self.dropbox_root,
+            google_cloud_credentials_path=self.google_cloud_creds_path,
+            google_drive_credentials_path=self.google_drive_creds_path)
 
         for file_path in file_path_list:
-            q.put((file_path, ci.fetch(os.path.join(from_folder_path, file_path))))
+            q.put((file_path, ci.fetch(os.path.join(from_folder_path,
+                                                    file_path))))
 
         q.put(('', ''))
 
-    def write_files(self, q: queue.Queue, from_folder_path: str, to_folder_path: str):
+    def write_files(self, q: queue.Queue,
+                    from_folder_path: str,
+                    to_folder_path: str):
         """Writes given file contents to new files
         :param q: queue which contains file path and file content
         :param from_folder_path:folder path of already read files
         :param to_folder_path: folder path of files to write
         :return:
         """
         while True:
-            ci = CloudInterface(aws_region_name=self.aws_region_name, aws_access_key_id=self.aws_access_key_id,
-                                aws_secret_access_key=self.aws_secret_access_key, dropbox_token=self.dropbox_token,
-                                dropbox_root=self.dropbox_root,
-                                google_cloud_credentials_path=self.google_cloud_credentials_path,
-                                google_drive_credentials_path=self.google_drive_credentials_path)
+            ci = CloudInterface(
+                aws_region_name=self.aws_region_name,
+                aws_access_key_id=self.aws_access_key_id,
+                aws_secret_access_key=self.aws_secret_access_key,
+                dropbox_token=self.dropbox_token,
+                dropbox_root=self.dropbox_root,
+                google_cloud_credentials_path=self.google_cloud_creds_path,
+                google_drive_credentials_path=self.google_drive_creds_path)
 
             file_path, content = q.get(block=True)
             # Use Enum for identifying queue progress
             if not file_path:
                 break
 
             to_file_path = os.path.join(to_folder_path, file_path)
             ci.save(to_file_path, content)
-            logger.info(f"Copied file {os.path.join(from_folder_path, file_path)} to {to_file_path}")
+            logger.info(f"Copied file"
+                        f" {os.path.join(from_folder_path, file_path)}"
+                        f" to {to_file_path}")
             q.task_done()
 
     @staticmethod
     def get_chunk(seq: list, n_chunks: int) -> list:
         """
         Divides given sequence to n chunks
         """
@@ -95,29 +109,33 @@
         for idx, chunk in enumerate(itertools.cycle(result_list)):
             if idx == seq_size:
                 break
             chunk.append(seq[idx])
 
         return result_list
 
-    def copy_batch(self, from_path: str, to_path: str, continue_copy: Optional[bool] = False,
+    def copy_batch(self, from_path: str, to_path: str,
+                   continue_copy: Optional[bool] = False,
                    process_amount: int = 10):
         """ Asynchronous copy entire batch(folder) to new destination
         :param from_path: folder/bucket to copy from
         :param to_path: name of folder to copy files
         :param continue_copy:
         :param process_amount:
         :return:
         """
 
-        ci = CloudInterface(aws_region_name=self.aws_region_name, aws_access_key_id=self.aws_access_key_id,
-                            aws_secret_access_key=self.aws_secret_access_key, dropbox_token=self.dropbox_token,
-                            dropbox_root=self.dropbox_root,
-                            google_cloud_credentials_path=self.google_cloud_credentials_path,
-                            google_drive_credentials_path=self.google_drive_credentials_path)
+        ci = CloudInterface(
+            aws_region_name=self.aws_region_name,
+            aws_access_key_id=self.aws_access_key_id,
+            aws_secret_access_key=self.aws_secret_access_key,
+            dropbox_token=self.dropbox_token,
+            dropbox_root=self.dropbox_root,
+            google_cloud_credentials_path=self.google_cloud_creds_path,
+            google_drive_credentials_path=self.google_drive_creds_path)
         if continue_copy:
             from_path_list = ci.listdir(from_path, recursive=True)
             try:
                 to_path_list = ci.listdir(to_path, recursive=True)
             except FileNotFoundError:
                 to_path_list = []
 
@@ -137,15 +155,16 @@
             q = queue.Queue()
 
             read_thread = Thread(target=self.read_files,
                                  args=(chunk, q, from_path))
 
             read_threads.append(read_thread)
 
-            write_thread = Thread(target=self.write_files, args=(q, from_path, to_path))
+            write_thread = Thread(target=self.write_files,
+                                  args=(q, from_path, to_path))
             write_threads.append(write_thread)
 
             read_thread.start()
             write_thread.start()
 
         # join all opened threads
         for r, w in zip(read_threads, write_threads):
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/interface/cloud_interface.py` & `cloudstorageio-1.2.9/cloudstorageio/interface/cloud_interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,145 @@
-""" Class CloudInterface handles with Google Cloud Storage, S3 and Dropbox storage files/folder
+""" Class CloudInterface handles with Google Cloud Storage,
+    S3 and Dropbox storage files/folder
     All methods are for all 4 environments (s3, google cloud, dropbox, local)
 
     Class CloudInterface contains
-                                open method, for opening/creating given file object
-                                isfile and isdir methods for checking object status (file, folder)
-                                listdir method for listing folder's content
-                                remove method for removing file/folder
-                                copy method for copying file from one storage to another
+            open method, for opening/creating given file object
+            isfile and isdir methods for checking object status (file, folder)
+            listdir method for listing folder's content
+            remove method for removing file/folder
+            copy method for copying file from one storage to another
 """
 import functools
 import multiprocessing
 import os
 from multiprocessing.pool import Pool
 from typing import Optional, Callable
 
 from cloudstorageio.enums import PrefixEnums
+from cloudstorageio.enums.enums import StorageIdentifierEnum
+from cloudstorageio.interface import DropBoxInterface
+from cloudstorageio.interface import GoogleDriveInterface
 from cloudstorageio.interface import GoogleStorageInterface
 from cloudstorageio.interface import LocalStorageInterface
 from cloudstorageio.interface import S3Interface
-from cloudstorageio.interface import DropBoxInterface
-from cloudstorageio.interface import GoogleDriveInterface
-
-from cloudstorageio.tools.decorators import timer, storage_cache_factory
 from cloudstorageio.tools.ci_collections import path_formatter
+from cloudstorageio.tools.decorators import timer, storage_cache_factory
 from cloudstorageio.tools.logger import logger
 
 
 class CloudInterface:
 
-    def __init__(self, aws_region_name: Optional[str] = None, aws_access_key_id: Optional[str] = None,
-                 aws_secret_access_key: Optional[str] = None, dropbox_token: Optional[str] = None,
-                 dropbox_root: Optional[bool] = None, google_cloud_credentials_path: Optional[str] = None,
-                 google_drive_credentials_path: Optional[str] = None, **kwargs):
+    def __init__(self, aws_region_name: Optional[str] = None,
+                 aws_access_key_id: Optional[str] = None,
+                 aws_secret_access_key: Optional[str] = None,
+                 dropbox_token: Optional[str] = None,
+                 dropbox_root: Optional[bool] = None,
+                 google_cloud_credentials_path: Optional[str] = None,
+                 google_drive_credentials_path: Optional[str] = None,
+                 **kwargs):
 
         """Initializes CloudInterface instance
         :param aws_region_name: region name for S3 storage
         :param aws_access_key_id: access key id for S3 storage
         :param aws_secret_access_key: secret access key for S3 storage
         :param dropbox_token: generated token for dropbox app access
         :param dropbox_root: namespace id starts from root
-        :param google_cloud_credentials_path: local path of google cloud credentials file (json)
-        :param google_drive_credentials_path: local path of google drive secret credentials file (json)
+        :param google_cloud_credentials_path: local path of
+               google cloud credentials file (json)
+        :param google_drive_credentials_path: local path of
+               Google Drive secret credentials file (json)
         :param kwargs:
         """
 
         self._kwargs = kwargs
         self._kwargs['aws_region_name'] = aws_region_name
         self._kwargs['aws_access_key_id'] = aws_access_key_id
         self._kwargs['aws_secret_access_key'] = aws_secret_access_key
         self._kwargs['dropbox_token'] = dropbox_token
         self._kwargs['dropbox_root'] = dropbox_root
-        self._kwargs['google_cloud_credentials_path'] = google_cloud_credentials_path
-        self._kwargs['google_drive_credentials_path'] = google_drive_credentials_path
+        self._kwargs['google_cloud_credentials_path'] = \
+            google_cloud_credentials_path
+        self._kwargs['google_drive_credentials_path'] = \
+            google_drive_credentials_path
 
         self._filename = None
         self._mode = None
-        self._s3 = None
-        self._gs = None
-        self._local = None
-        self._dbx = None
-        self._dr = None
         self._current_storage = None
         self._path = None
 
+        self._storage_classes = {
+            StorageIdentifierEnum.LOCAL: LocalStorageInterface,
+            StorageIdentifierEnum.S3: S3Interface,
+            StorageIdentifierEnum.GOOGLE_CLOUD: GoogleStorageInterface,
+            StorageIdentifierEnum.DROPBOX: DropBoxInterface,
+            StorageIdentifierEnum.GOOGLE_DRIVE: GoogleDriveInterface
+        }
+
+        self._storage_instances = {}
+
     def identify_path_type(self, path: str):
         """Identifies "type" of given path and create class instance
         :param path: full path of file/folder
         :return: None
         """
 
         self._path = path_formatter(path)
 
         if self.is_local_path(self._path):
-            if self._local is None:
-                self._local = LocalStorageInterface()
-            self._current_storage = self._local
-
-        elif self.is_s3_path(self._path):
-            if self._s3 is None:
-                self._s3 = S3Interface(**self._kwargs)
-            self._current_storage = self._s3
-
-        elif self.is_google_storage_path(self._path):
-            if self._gs is None:
-                self._gs = GoogleStorageInterface(**self._kwargs)
-            self._current_storage = self._gs
-
-        elif self.is_dropbox_path(self._path):
-            if self._dbx is None:
-                self._dbx = DropBoxInterface(**self._kwargs)
-            self._current_storage = self._dbx
-
-        elif self.is_drive_path(self._path):
-            if self._dr is None:
-                self._dr = GoogleDriveInterface(**self._kwargs)
-            self._current_storage = self._dr
-        else:
-            raise ValueError(f"`{path}` is invalid. Please use {PrefixEnums.DROPBOX.value} prefix for dropBox,"
-                             f" {PrefixEnums.S3.value} for S3 storage, "
-                             f" {PrefixEnums.GOOGLE_CLOUD.value} for Google Cloud Storage,"
-                             f"{PrefixEnums.GOOGLE_DRIVE.value} for Google Drive, or VALID local path")
+            self._current_storage = self._get_storage_instance(
+                StorageIdentifierEnum.LOCAL)
+            return None
+
+        if self.is_s3_path(self._path):
+            self._current_storage = self._get_storage_instance(
+                StorageIdentifierEnum.S3)
+            return None
+
+        if self.is_google_storage_path(self._path):
+            self._current_storage = self._get_storage_instance(
+                StorageIdentifierEnum.GOOGLE_CLOUD)
+            return None
+
+        if self.is_dropbox_path(self._path):
+            self._current_storage = self._get_storage_instance(
+                StorageIdentifierEnum.DROPBOX)
+            return None
+
+        if self.is_drive_path(self._path):
+            self._current_storage = self._get_storage_instance(
+                StorageIdentifierEnum.GOOGLE_DRIVE
+            )
+            return None
+
+        raise ValueError(f"`{path}` is invalid. Please use "
+                         f"{PrefixEnums.DROPBOX.value}"
+                         f" prefix for dropBox,"
+                         f" {PrefixEnums.S3.value}"
+                         f" for S3 storage, "
+                         f" {PrefixEnums.GOOGLE_CLOUD.value}"
+                         f" for Google Cloud Storage,"
+                         f"{PrefixEnums.GOOGLE_DRIVE.value} "
+                         f"for Google Drive, or VALID local path")
+
+    def _get_storage_instance(self, storage_id):
+        if storage_id in self._storage_instances:
+            return self._storage_instances[storage_id]
+
+        storage_instance = self._storage_classes[storage_id](**self._kwargs)
+
+        self._storage_instances[storage_id] = storage_instance
+
+        return storage_instance
 
     def _reset_fields(self):
         """Set all instance attributes to none"""
         self._filename = None
         self._mode = None
-        self._s3 = None
-        self._gs = None
-        self._local = None
-        self._dbx = None
-        self._dr = None
+        self._storage_instances = {}
         self._current_storage = None
         self._path = None
 
     @staticmethod
     def is_local_path(path: str) -> bool:
         """Checks if the given path is for local storage"""
         is_dir = False
@@ -126,31 +152,34 @@
     @staticmethod
     def is_s3_path(path: str) -> bool:
         """Checks if the given path is for S3 storage"""
         return path.strip().startswith(PrefixEnums.S3.value)
 
     @staticmethod
     def is_google_storage_path(path: str) -> bool:
-        """Checks if the given path is for google storage"""
+        """Checks if the given path is for Google storage"""
         return path.strip().startswith(PrefixEnums.GOOGLE_CLOUD.value)
 
     @staticmethod
     def is_dropbox_path(path: str) -> bool:
         """Checks if the given path is for dropBox"""
         return path.strip().startswith(PrefixEnums.DROPBOX.value)
 
     @staticmethod
     def is_drive_path(path: str) -> bool:
-        """Checks if the given path is for google drive"""
+        """Checks if the given path is for Google Drive"""
         return path.strip().startswith(PrefixEnums.GOOGLE_DRIVE.value)
 
-    def open(self, file_path: str, mode: Optional[str] = 'rt', *args, **kwargs) -> Callable:
-        """Identifies given file path and return "open" method for detected current storage"""
+    def open(self, file_path: str, mode: Optional[str] = 'rt',
+             *args, **kwargs) -> Callable:
+        """Identifies given file path and return "open" method
+           for detected current storage"""
         self.identify_path_type(file_path)
-        res = self._current_storage.open(path=file_path, mode=mode, *args, **kwargs)
+        res = self._current_storage.open(path=file_path, mode=mode,
+                                         *args, **kwargs)
         self._reset_fields()
         return res
 
     def save(self, path: str, content):
         """Save content to given file"""
         with self.open(path, 'wb') as f:
             f.write(content)
@@ -178,40 +207,47 @@
     def remove(self, path: str) -> Callable:
         """Deletes file/folder"""
         self.identify_path_type(path)
         res = self._current_storage.remove(path)
         self._reset_fields()
         return res
 
-    def listdir(self, path: str, recursive: Optional[bool] = False, exclude_folders: Optional[bool] = False,
+    def listdir(self, path: str, recursive: Optional[bool] = False,
+                exclude_folders: Optional[bool] = False,
                 include_files: Optional[bool] = True) -> list:
         """ Lists all files/folders containing in given folder path
         :param path: the full path of folder (with prefix)
         :param recursive: list folder recursively, (by default no)
-        :param exclude_folders: exclude folders from list (by default no, lists folders too)
-        :param include_files: list files in folders or not (by default no, lists only folders)
+        :param exclude_folders: exclude folders from list
+                                (by default no, lists folders too)
+        :param include_files: list files in folders or not
+                              (by default no, lists only folders)
         :return: list of folder's content (file/folder names)
         """
         self.identify_path_type(path)
-        if self._s3:
-            res = self._current_storage.listdir(path=path, recursive=recursive, exclude_folders=exclude_folders,
-                                                include_files=include_files)
-        else:
-            res = self._current_storage.listdir(path=path, recursive=recursive, exclude_folders=exclude_folders)
+        # EDITED: if condition was removed.
+        res = self._current_storage.listdir(path=path, recursive=recursive,
+                                            exclude_folders=exclude_folders,
+                                            include_files=include_files)
         self._reset_fields()
         return res
 
     @storage_cache_factory()
-    def cache_listdir(self, path: str, recursive: Optional[bool] = False, exclude_folders: Optional[bool] = False):
-        """Cache the listed output of the first call, then use the already cached output (when called again)"""
-        return self.listdir(path=path, recursive=recursive, exclude_folders=exclude_folders)
+    def cache_listdir(self, path: str, recursive: Optional[bool] = False,
+                      exclude_folders: Optional[bool] = False):
+        """Cache the listed output of the first call, then use the
+           already cached output (when called again)"""
+        return self.listdir(path=path,
+                            recursive=recursive,
+                            exclude_folders=exclude_folders)
 
     def copy(self, from_path: str, to_path: str):
         """Copies given file to new destination"""
-        # calling the upload method with multipart configs if a local file is copied to S3
+        # calling the upload method with multipart configs if a
+        # local file is copied to S3
         if self.is_local_path(from_path) and self.is_s3_path(to_path):
             self.identify_path_type(to_path)  # setting up s3 storage
             with self.open(to_path, 'wb') as f:
                 f.upload(from_path)
                 return
 
         content = self.fetch(path=from_path)
@@ -229,57 +265,70 @@
             full_from_path = os.path.join(from_path, p)
             full_to_path = os.path.join(to_path, p)
             self.copy(from_path=full_from_path, to_path=full_to_path)
         except Exception as e:
             logger.error(f'Failed to copy {p} file : {e}')
 
     @timer
-    def copy_dir(self, source_dir: str, dest_dir: str, multiprocess: Optional[bool] = True,
+    def copy_dir(self, source_dir: str, dest_dir: str,
+                 multiprocess: Optional[bool] = True,
                  continue_copy: Optional[bool] = False):
         """ Recursively copy a directory
         :param source_dir: folder/bucket to copy from
-        :param dest_dir: folder/bucket to copy to (dest_dir does not need to exist)
+        :param dest_dir: folder/bucket to copy
+         to (dest_dir does not need to exist)
         :param multiprocess: indicator of multiprocessing
-        :param continue_copy: if True, will ignore the same files existing in both dirs and copy only differing ones
+        :param continue_copy: if True, will ignore the same files existing
+         in both dirs and copy only differing ones
         :return:
         """
+
         if continue_copy:
-            from_path_list = self.listdir(source_dir, recursive=True, exclude_folders=True)
+            from_path_list = self.listdir(source_dir,
+                                          recursive=True,
+                                          exclude_folders=True)
 
             try:
-                to_path_list = self.listdir(dest_dir, recursive=True, exclude_folders=True)
+                to_path_list = self.listdir(dest_dir,
+                                            recursive=True,
+                                            exclude_folders=True)
             except FileNotFoundError:
                 to_path_list = []
 
             full_path_list = list(set(from_path_list) - set(to_path_list))
         else:
-            full_path_list = self.listdir(source_dir, recursive=True, exclude_folders=True)
+            full_path_list = self.listdir(source_dir,
+                                          recursive=True,
+                                          exclude_folders=True)
 
         if multiprocess:
             p = Pool(multiprocessing.cpu_count())
             # for each call from_path & to_path are constants
-            partial_func = functools.partial(self._call_copy, from_path=source_dir, to_path=dest_dir)
+            partial_func = functools.partial(self._call_copy,
+                                             from_path=source_dir,
+                                             to_path=dest_dir)
             p.map(partial_func, full_path_list)
         else:
             for f in full_path_list:
                 self._call_copy(f, source_dir, dest_dir)
 
     def _call_copy_zip(self, from_to_zip: zip):
         try:
             self.copy(from_to_zip[0], from_to_zip[1])
         except Exception as e:
             logger.error(f'Failed to copy {from_to_zip[0]} file : {e}')
 
-    def copy_batch(self, from_batch: list, to_batch: list, multiprocess: Optional[bool] = True):
+    def copy_batch(self, from_batch: list, to_batch: list,
+                   multiprocess: Optional[bool] = True):
         """ Copy entire batch (list)
         :param from_batch: folder/file path list to copy from
         :param to_batch: folder/file path list to copy to
         :param multiprocess: indicator of doing process with multiprocessing
         :return:
         """
         if multiprocess:
             p = Pool(multiprocessing.cpu_count())
             partial_func = functools.partial(self._call_copy_zip)
             p.map(partial_func, zip(from_batch, to_batch))
         else:
             for from_file, to_file in zip(from_batch, to_batch):
-                self.copy(from_path=from_file, to_path=to_file)
+                self.copy(from_path=from_file, to_path=to_file)
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/interface/drop_box.py` & `cloudstorageio-1.2.9/cloudstorageio/interface/drop_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-""" Class DropBoxInterface handles with DropBoxInterface workspace files/folders
+""" Class DropBoxInterface handles with DropBoxInterface
+    workspace files/folders
 
     Class DropBoxInterface has
-                                    read and write methods (can be accessed by open method)
-                                    isfile and isdir methods for checking object status (file, folder)
-                                    listdir method for listing folder's content
-                                    remove method for removing file/folder
+            read and write methods (can be accessed by open method)
+            isfile and isdir methods for checking object status (file, folder)
+            listdir method for listing folder's content
+            remove method for removing file/folder
 """
 
 import os
 import re
-
-import dropbox
 from typing import Union, Optional
 
+import dropbox
 from dropbox.common import PathRoot
-from dropbox.files import FileMetadata, FolderMetadata, WriteMode
 from dropbox.exceptions import ApiError
+from dropbox.files import FileMetadata, FolderMetadata, WriteMode
 from dropbox.stone_validators import ValidationError
 
 from cloudstorageio.configs import CloudInterfaceConfig
 from cloudstorageio.enums.enums import PrefixEnums
 from cloudstorageio.exceptions import CaseInsensitivityError
-from cloudstorageio.tools.logger import logger
 from cloudstorageio.tools.ci_collections import add_slash, str2bool
+from cloudstorageio.tools.logger import logger
 
 
 class DropBoxInterface:
     PREFIX = PrefixEnums.DROPBOX.value
 
     def __init__(self, **kwargs):
         """Initializes DropBoxInterface instance, creates dbx instance
@@ -55,16 +55,18 @@
         self.list_recursive = False
         self.include_folders = False
 
         self.dbx = dropbox.Dropbox(self.token)
 
         # namespace id starts from root
         if self.root:
-            root_namespace_id = self.dbx.users_get_current_account().root_info.root_namespace_id
-            self.dbx = self.dbx.with_path_root(PathRoot.namespace_id(root_namespace_id))
+            root_namespace_id = self.dbx.users_get_current_account().root_info\
+                .root_namespace_id
+            self.dbx = self.dbx.with_path_root(PathRoot.namespace_id(
+                root_namespace_id))
 
     @property
     def path(self):
         if self._current_path is None:
             raise ValueError("Path name is not set")
         return self._current_path
 
@@ -75,19 +77,23 @@
             self._current_path = None
         else:
             value = value.split(self.PREFIX, 1)[-1]
 
             if value in ('.', ''):
                 self._current_path = ''
             else:
-                self._current_path = value if value.startswith('/') else f'/{value}'
-                self._current_path = self._current_path[:-1] if self._current_path.endswith('/') else self._current_path
+                if value.startswith('/'):
+                    self._current_path = value
+                else:
+                    self._current_path = f'/{value}'
+                if self._current_path.endswith('/'):
+                    self._current_path = self._current_path[:-1]
 
     def _detect_path_type(self):
-        """Detects whether given path is file, folder or does not exists"""
+        """Detects whether given path is file, folder or does not exist"""
         if self.path == '':
             self._isdir = True
         try:
             self.metadata = self.dbx.files_get_metadata(self.path)
         except (ApiError, ValidationError):
             self.metadata = None
 
@@ -95,35 +101,42 @@
             self._isfile = True
         if isinstance(self.metadata, FolderMetadata):
             self._isdir = True
 
         if self._isdir or self._isfile:
             self._object_exists = True
             if self.metadata:
-                if self.metadata.path_display != self.path and self.metadata.path_lower == self.path.lower():
-                    raise CaseInsensitivityError(f'DropBox case-insensitivity conflict: The given  {self.path} is'
-                                                 f' the same file(folder) as {self.metadata.path_display}')
+                if self.metadata.path_display != self.path \
+                        and self.metadata.path_lower == self.path.lower():
+                    raise CaseInsensitivityError(
+                        f'DropBox case-insensitivity '
+                        f'conflict: The given  {self.path} is'
+                        f' the same file(folder) as '
+                        f'{self.metadata.path_display}')
 
     def _populate_listdir(self):
         """Appends each file.folder name to self._listdir"""
 
         def __populate_metadata(metadata):
             for f in metadata.entries:
                 try:
-                    full_path = re.split(add_slash(self.path), f.path_display, flags=re.IGNORECASE, maxsplit=1)[1]
+                    full_path = re.split(add_slash(self.path),
+                                         f.path_display, flags=re.IGNORECASE,
+                                         maxsplit=1)[1]
                     if isinstance(f, FolderMetadata):
                         if self.include_folders:
                             self._listdir.append((add_slash(full_path)))
                     else:
                         self._listdir.append(full_path)
                 except IndexError:
                     # failed to split path
                     continue
 
-        folder_metadata = self.dbx.files_list_folder(self.path, recursive=self.list_recursive)
+        folder_metadata = self.dbx.files_list_folder(
+            self.path, recursive=self.list_recursive)
 
         __populate_metadata(metadata=folder_metadata)
 
         while folder_metadata.has_more:
             cur = folder_metadata.cursor
             folder_metadata = self.dbx.files_list_folder_continue(cur)
             __populate_metadata(metadata=folder_metadata)
@@ -152,15 +165,16 @@
         return self._isfile
 
     def isdir(self, path: str):
         """Checks dictionary existence for given path"""
         self._analyse_path(path)
         return self._isdir
 
-    def listdir(self, path: str, recursive: Optional[bool] = False, exclude_folders: Optional[bool] = False):
+    def listdir(self, path: str, recursive: Optional[bool] = False,
+                exclude_folders: Optional[bool] = False):
         """Lists content for given folder path"""
         self.list_recursive = recursive
         self.include_folders = not exclude_folders
         self._analyse_path(path)
         if self._isdir:
             self._populate_listdir()
 
@@ -181,15 +195,16 @@
     def open(self, path: str, mode: Optional[str] = None):
         """Opens a file from dropBox and returns the DropBoxInterface object"""
         self._mode = mode
         self._analyse_path(path)
 
         return self
 
-    def write(self, content: Union[str, bytes], metadata: Optional[dict] = None):
+    def write(self, content: Union[str, bytes],
+              metadata: Optional[dict] = None):
         """Writes content to file on dropBox
         :param content: The content that should be written to a file
         :param metadata:
         :return: String content of the file specified in the file path argument
         """
 
         if self._isfile:
@@ -200,22 +215,28 @@
             content = content.encode('utf8')
         if not metadata:
             metadata = {}
         if self._mode is not None and ('w' not in self._mode and
                                        'a' not in self._mode and
                                        'x' not in self._mode and
                                        '+' not in self._mode):
-            raise ValueError(f"Mode '{self._mode}' does not allow writing the file")
+            raise ValueError(f"Mode '{self._mode}' "
+                             f"does not allow writing the file")
 
         try:
-            res = self.dbx.files_upload(f=content, path=self.path, mode=self._write_mode)
-            if res.path_display != self.path and res.path_lower == self.path.lower():
+            res = self.dbx.files_upload(f=content, path=self.path,
+                                        mode=self._write_mode)
+            if res.path_display != self.path \
+                    and res.path_lower == self.path.lower():
                 self.dbx.files_delete_v2(self.path)
-                raise CaseInsensitivityError(f'DropBox case-insensitivity conflict: The given  {self.path} is'
-                                             f' the same file(folder) as {res.path_display}')
+                raise CaseInsensitivityError(f'DropBox case-insensitivity'
+                                             f' conflict: The given '
+                                             f'{self.path} is the same '
+                                             f'file(folder) as '
+                                             f'{res.path_display}')
         except ApiError:
             logger.info(f'Failed to upload {self.path} to dropbox')
 
     def read(self) -> Union[str, bytes]:
         """Reads dropBox file and returns the bytes
         :return: String content of the file
         """
@@ -228,15 +249,16 @@
 
         if self._mode is not None and 'b' not in self._mode:
             try:
                 res = res.decode(self._encoding)
             except UnicodeDecodeError:
                 raise ValueError(f"The content cannot be decoded into a string"
                                  f" with encoding {self._encoding}."
-                                 f" Include 'b' on read mode to return the original bytes")
+                                 f" Include 'b' on read mode to return "
+                                 f"the original bytes")
         return res
 
     def __enter__(self):
         self._is_open = True
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -245,8 +267,8 @@
 
 
 if __name__ == '__main__':
     my_configs = '/home/vahagn/Dropbox/cognaize/cloudstorageio_creds.json'
     CloudInterfaceConfig.set_configs(config_json_path=my_configs)
     dr = DropBoxInterface()
     res = dr.listdir('dbx://')
-    print(res)
+    print(res)
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/interface/google_drive.py` & `cloudstorageio-1.2.9/cloudstorageio/interface/google_drive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,53 @@
+import logging
 import os
 import shutil
-
-import cloudstorageio
-import logging
-
 from typing import Optional, Union
-from pydrive.drive import GoogleDrive
-from pydrive.auth import GoogleAuth
+
 from googleapiclient.errors import HttpError
+from pydrive.auth import GoogleAuth
+from pydrive.drive import GoogleDrive
 
+import cloudstorageio
+from cloudstorageio.configs import resources
 from cloudstorageio.enums.enums import PrefixEnums
 from cloudstorageio.tools.ci_collections import add_slash
-from cloudstorageio.tools.logger import logger
-from cloudstorageio.tools.decorators import timer
-from cloudstorageio.configs import resources, CloudInterfaceConfig
 
 # avoiding dependencies' warning
 logging.getLogger('googleapiclient.discovery_cache').setLevel(logging.ERROR)
 
 
 class GoogleDriveInterface:
     PREFIX = PrefixEnums.GOOGLE_DRIVE.value
 
     mimetypes_changes = {
         'application/vnd.google-apps.document': 'text/plain',
-        'application/vnd.google-apps.spreadsheet': 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'}
-
-    settings_file = os.path.abspath(os.path.join(os.path.dirname(resources.__file__), 'settings.yaml'))
+        'application/vnd.google-apps.spreadsheet':
+            'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
+    }
+
+    settings_file = os.path.abspath(
+        os.path.join(os.path.dirname(
+            resources.__file__), 'settings.yaml'))
 
     def __init__(self, **kwargs):
 
-        self.config_file_path = kwargs.pop('google_cloud_credentials_path', None)
+        self.config_file_path = kwargs.pop(
+            'google_cloud_credentials_path', None)
 
         if not self.config_file_path:
             self.config_file_path = os.environ.get('GOOGLE_DRIVE_CREDENTIALS')
         if not self.config_file_path:
-            raise ValueError("Please add GOOGLE_DRIVE_CREDENTIALS environment variable"
-                             " or set google_drive_credentials_json_path")
-
-        self.tmp_folder = os.path.join(os.path.dirname(os.path.dirname(cloudstorageio.__file__)), 'gdrive_tmp')
+            raise ValueError("Please add GOOGLE_DRIVE_CREDENTIALS environment"
+                             " variable or set "
+                             "google_drive_credentials_json_path")
+
+        self.tmp_folder = os.path.join(
+            os.path.dirname(os.path.dirname(
+                cloudstorageio.__file__)), 'gdrive_tmp')
         if os.path.isdir(self.tmp_folder):
             shutil.rmtree(self.tmp_folder)
         os.mkdir(path=self.tmp_folder)
 
         self.credentials = self._setup()
         self.drive = GoogleDrive(self.credentials)
         self._encoding = 'utf8'
@@ -62,22 +67,29 @@
         return gauth
 
     def _set_configs(self):
         """"""
         with open(self.settings_file, 'rb') as f:
             yaml_string = f.read().decode()
 
-        client_config_file = yaml_string.split('client_config_file:', 1)[1].split()[0]
+        client_config_file = yaml_string.split(
+            'client_config_file:', 1)[1].split()[0]
 
-        save_credentials_file = yaml_string.split('save_credentials_file:', 1)[1].split()[0]
-        save_credentials_file_new = os.path.abspath(os.path.join(os.path.dirname(resources.__file__), 'credentials.json'))
-        yaml_string = yaml_string.replace(client_config_file, self.config_file_path)
-        yaml_string = yaml_string.replace(save_credentials_file, save_credentials_file_new)
+        save_credentials_file = yaml_string.split(
+            'save_credentials_file:', 1)[1].split()[0]
+        save_credentials_file_new = \
+            os.path.abspath(os.path.join(os.path.dirname(
+                resources.__file__), 'credentials.json'))
+        yaml_string = yaml_string.replace(client_config_file,
+                                          self.config_file_path)
+        yaml_string = yaml_string.replace(save_credentials_file,
+                                          save_credentials_file_new)
 
-        if client_config_file != self.config_file_path and os.path.isfile(save_credentials_file_new):
+        if client_config_file != self.config_file_path \
+                and os.path.isfile(save_credentials_file_new):
             os.remove(save_credentials_file_new)
 
         with open(self.settings_file, 'wb') as f:
             f.write(yaml_string.encode())
 
     @property
     def path(self):
@@ -92,15 +104,18 @@
             self._current_path = None
         else:
             value = value.split(self.PREFIX)[-1]
 
             if value in ('.', ''):
                 self._current_path = ''
             else:
-                self._current_path = value[:-1] if value.endswith('/') else value
+                if value.endswithh('/'):
+                    self._current_path = value[:-1]
+                else:
+                    self._current_path = value
 
     def get_id_from_full_path(self, name: str):
         """Get di from given file/folder full path"""
 
         def _find_id(file_obj_list: list, n):
             for i in file_obj_list:
                 if i['title'] == n:
@@ -111,26 +126,29 @@
         split_name_list = (name.split(self.PREFIX)[-1]).split('/')
         file_list = self.drive.ListFile({'q': "trashed=false"}).GetList()
 
         for file_idx, name in enumerate(split_name_list):
             file_id = _find_id(file_list, name)
             if not file_id:
                 return None
-            file_list = self.drive.ListFile({'q': "'{}' in parents and trashed=false".format(file_id)}).GetList()
+            file_list = self.drive.ListFile(
+                {'q': "'{}' in parents and trashed=false".format(
+                    file_id)}).GetList()
 
         return file_id
 
     def get_full_path_from_id(self, file_id: str):
         """Get full path of given file(folder) id"""
 
         file_name = ''
         while True:
             file = self.drive.CreateFile({'id': file_id})
             # if not file.uploaded:
-            #     raise FileNotFoundError(f'No such file/folder with id: {file_id}')
+            #     raise FileNotFoundError(
+            #     f'No such file/folder with id: {file_id}')
 
             if file['title'] != 'My Drive':
                 file_name = os.path.join(file['title'], file_name)
 
             if file['parents']:
                 parent_id = file['parents'][0]['id']
             else:
@@ -141,23 +159,26 @@
     def _detect_path_type(self):
         """Detects whether given path is file, folder or does not exists"""
 
         if self.path == '':
             self._isdir = True
         if self._object_exists:
             drive_file_obj = self.drive.CreateFile({'id': self.id})
-            if drive_file_obj['mimeType'] == 'application/vnd.google-apps.folder':
+            if drive_file_obj['mimeType'] == \
+                    'application/vnd.google-apps.folder':
                 self._isdir = True
             else:
                 self._isfile = True
 
     def _populate_listdir(self, folder_id: str, parent: Optional[str] = ''):
         """Appends each file.folder name to self._listdir"""
         try:
-            file_list = self.drive.ListFile({'q': "'{}' in parents and trashed=false".format(folder_id)}).GetList()
+            file_list = self.drive.ListFile(
+                {'q': "'{}' in parents and trashed=false".format(
+                    folder_id)}).GetList()
             for f in file_list:
                 if f['mimeType'] == 'application/vnd.google-apps.folder':
                     p = parent + add_slash(f['title'])
                     if self.include_folders:
                         self._listdir.append(p)
                     if self.recursive:
                         self._populate_listdir(f['id'], parent=p)
@@ -190,15 +211,16 @@
         return self._isfile
 
     def isdir(self, path: str):
         """Checks dictionary existence for given path"""
         self._analyse_path(path)
         return self._isdir
 
-    def listdir(self, path: str, recursive: Optional[bool] = False, exclude_folders: Optional[bool] = False):
+    def listdir(self, path: str, recursive: Optional[bool] = False,
+                exclude_folders: Optional[bool] = False):
         """Lists content for given folder path"""
         self.recursive = recursive
         self.include_folders = not exclude_folders
         self._analyse_path(path)
 
         if not self._object_exists:
             raise FileNotFoundError(f'No such file or dictionary: {path}')
@@ -208,23 +230,25 @@
         return self._listdir
 
     def remove(self, path: str):
         self._analyse_path(path)
         # TODO
 
     def open(self, path: str, mode: Optional[str] = None):
-        """Opens a file from Google Drive and returns the GoogleDriveInterface object"""
+        """Opens a file from Google Drive and returns the
+           GoogleDriveInterface object"""
         self._mode = mode
         self._analyse_path(path)
         return self
 
     def _create_folders(self, path: str):
         pass
 
-    def write(self, content: Union[str, bytes], metadata: Optional[dict] = None):
+    def write(self, content: Union[str, bytes],
+              metadata: Optional[dict] = None):
         """Writes content to file on google drive
         :param content: The content that should be written to a file
         :param metadata:
         :return: String content of the file specified in the file path argument
         """
 
         if isinstance(content, str):
@@ -232,26 +256,30 @@
 
         if not metadata:
             metadata = {}
         if self._mode is not None and ('w' not in self._mode and
                                        'a' not in self._mode and
                                        'x' not in self._mode and
                                        '+' not in self._mode):
-            raise ValueError(f"Mode '{self._mode}' does not allow writing the file")
+            raise ValueError(f"Mode '{self._mode}' does not allow "
+                             f"writing the file")
 
         if self._isfile:
             # logger.info('Overwriting {} file'.format(self.path))
             file = self.drive.CreateFile({'id': self.id})
         else:
             folder_id = self.get_id_from_full_path(self.path.rsplit('/', 1)[0])
             if not folder_id:
                 self._create_folders(self.path)
-            file = self.drive.CreateFile({'title': self.path.rsplit('/')[-1], 'parents': [{"id": folder_id}]})
+            file = self.drive.CreateFile(
+                {'title': self.path.rsplit('/')[-1],
+                 'parents': [{"id": folder_id}]})
 
-        tmp_file_path = os.path.join(self.tmp_folder, self.path.rsplit('/')[-1])
+        tmp_file_path = os.path.join(
+            self.tmp_folder, self.path.rsplit('/')[-1])
 
         with open(tmp_file_path, 'wb') as f:
             f.write(content)
 
         file.SetContentFile(tmp_file_path)
         file.Upload()
         os.remove(tmp_file_path)
@@ -260,15 +288,16 @@
         """Reads google drive file and returns the bytes
         :return: String content of the file
         """
         if not self._isfile:
             raise FileNotFoundError('No such file: {}'.format(self.path))
 
         file = self.drive.CreateFile({'id': self.id})
-        tmp_file_path = os.path.join(self.tmp_folder, self.path.rsplit('/')[-1])
+        tmp_file_path = os.path.join(
+            self.tmp_folder, self.path.rsplit('/')[-1])
 
         if file['mimeType'] in self.mimetypes_changes:
             download_mimetype = self.mimetypes_changes[file['mimeType']]
             file.GetContentFile(tmp_file_path, mimetype=download_mimetype)
         else:
             file.GetContentFile(tmp_file_path)
         with open(tmp_file_path, 'rb') as f:
@@ -277,15 +306,16 @@
 
         if self._mode is not None and 'b' not in self._mode:
             try:
                 res = res.decode(self._encoding)
             except UnicodeDecodeError:
                 raise ValueError(f"The content cannot be decoded into a string"
                                  f" with encoding {self._encoding}."
-                                 f" Include 'b' on read mode to return the original bytes")
+                                 f" Include 'b' on read mode to return the "
+                                 f"original bytes")
         return res
 
     def __enter__(self):
         self._is_open = True
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/interface/google_storage.py` & `cloudstorageio-1.2.9/cloudstorageio/interface/google_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-""" Class GoogleStorageInterface handles with Google Cloud Storage files/folders
+""" Class GoogleStorageInterface handles with
+    Google Cloud Storage files/folders
 
     Class GoogleStorageInterface has
-                                    read and write methods (can be accessed by open method)
-                                    isfile and isdir methods for checking object status (file, folder)
-                                    listdir method for listing folder's content
-                                    remove method for removing file/folder
+            read and write methods (can be accessed by open method)
+            isfile and isdir methods for checking object status (file, folder)
+            listdir method for listing folder's content
+            remove method for removing file/folder
     Google Storage API itself doesn't have any concept of a "folder".
-        In GoogleStorageInterface you can differentiate file/folder like in local environment
+    In GoogleStorageInterface you can differentiate file/folder
+    like in local environment
 """
 
 import io
 import os
 from typing import Tuple, Union, Optional
+
 from google.cloud import storage
 
 from cloudstorageio.enums.enums import PrefixEnums
 from cloudstorageio.tools.ci_collections import add_slash
-from cloudstorageio.tools.logger import logger
 
 
 class GoogleStorageInterface:
     PREFIX = PrefixEnums.GOOGLE_CLOUD.value
 
     def __init__(self, **kwargs):
         """Initializes GoogleStorageInterface instance, creates storage client
         :param kwargs:
         """
 
         self.creds = kwargs.pop('google_cloud_credentials_path', None)
         if self.creds:
             os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = self.creds
         if 'GOOGLE_APPLICATION_CREDENTIALS' not in os.environ.keys():
-            raise ConnectionRefusedError("Please add GOOGLE_APPLICATION_CREDENTIALS environment variable"
-                                         " or set google_credentials_json_path")
+            raise ConnectionRefusedError("Please add "
+                                         "GOOGLE_APPLICATION_CREDENTIALS "
+                                         "environment variable or set "
+                                         "google_credentials_json_path")
 
         self._encoding = 'utf8'
         self._mode = None
         self._current_bucket = None
         self._current_path = None
         self._bucket = None
         self._blob = None
@@ -47,25 +51,28 @@
 
     @property
     def path(self):
         if self._current_bucket is None:
             raise ValueError("Bucket name is not set")
         if self._current_path is None:
             raise ValueError("Path name is not set")
-        return f"{GoogleStorageInterface.PREFIX}{self._current_bucket}/{self._current_path}"
+        return f"{GoogleStorageInterface.PREFIX}" \
+               f"{self._current_bucket}/{self._current_path}"
 
     @path.setter
     def path(self, value):
         if value is None:
             self._current_path = None
             self._current_bucket = None
         else:
             value = value[:-1] if value.endswith('/') else value
-            self._current_bucket, self._current_path = self._parse_bucket(value)
-            self._current_path_with_backslash = add_slash(self._current_path)
+            self._current_bucket, self._current_path = \
+                self._parse_bucket(value)
+            self._current_path_with_backslash = \
+                add_slash(self._current_path)
 
     def _detect_blob_object_type(self):
         """Hidden method for detecting given blob object type (file or folder)
         :return:
         """
         if self._current_path in self._blob_key_names_list:
             self._isfile = True
@@ -100,27 +107,30 @@
         self._bucket = self._storage_client.get_bucket(self._current_bucket)
 
         self._blob_objects = self._bucket.list_blobs(prefix=self._current_path)
 
         self._blob_key_names_list = [obj.name for obj in self._blob_objects]
 
     def _analyse_path(self, path: str):
-        """From given path creates bucket, blob objects, lists and detects object type (file/folder)
+        """From given path creates bucket, blob objects, lists and
+        detects object type (file/folder)
         :param path: full path of file/folder
         :return:
         """
 
         self._init_path(path)
 
         if self.only_bucket:
             self._isdir = True
         else:
             self._detect_blob_object_type()
-            self._blob_key_names_list = [f.split(self._current_path_with_backslash, 1)[1] for f in self._blob_key_names_list
-                                         if len(f.split(self._current_path_with_backslash, 1)) == 2]
+            self._blob_key_names_list = [f.split(
+                self._current_path_with_backslash, 1)[1]
+                    for f in self._blob_key_names_list if len(
+                    f.split(self._current_path_with_backslash, 1)) == 2]
 
         while '' in self._blob_key_names_list:
             self._blob_key_names_list.remove('')
 
         for blob in self._blob_key_names_list:
             self._populate_listdir(blob)
 
@@ -133,29 +143,31 @@
         return self._isfile
 
     def isdir(self, path: str):
         """Checks dictionary existence for given path"""
         self._analyse_path(path)
         return self._isdir
 
-    def listdir(self, path: str, recursive: Optional[bool] = False, exclude_folders: Optional[bool] = False) -> list:
+    def listdir(self, path: str, recursive: Optional[bool] = False,
+                exclude_folders: Optional[bool] = False) -> list:
         """Checks given dictionary's existence and lists content
         :param path: full path of gs object (file/folder)
         :param recursive: list content fully
         :param exclude_folders:
         :return:
         """
         self._analyse_path(path)
         include_folders = not exclude_folders
         if recursive:
             if include_folders:
                 folders = [f for f in self._listdir if f.endswith('/')]
                 result = self._blob_key_names_list + folders
             else:
-                result = [f for f in self._blob_key_names_list if not f.endswith('/')]
+                result = [f for f in self._blob_key_names_list
+                          if not f.endswith('/')]
         else:
             if include_folders:
                 result = self._listdir
             else:
                 result = [f for f in self._listdir if not f.endswith('/')]
 
         if not self._object_exists:
@@ -195,34 +207,36 @@
 
         if self._mode is not None and 'b' not in self._mode:
             try:
                 res = res.decode(self._encoding)
             except UnicodeDecodeError:
                 raise ValueError(f"The content cannot be decoded into a string"
                                  f" with encoding {self._encoding}."
-                                 f" Include 'b' on read mode to return the original bytes")
+                                 f" Include 'b' on read mode to return"
+                                 f" the original bytes")
         return res
 
     def write(self, content: Union[str, bytes, io.IOBase]):
-        """ Writes text to a file on google storage
+        """ Writes text to a file on Google storage
         :param content: The content that should be written to a file
         :return: String content of the file specified in the file path argument
         """
 
         if self._isfile:
             ...
             # logger.info('Overwriting {} file'.format(self.path))
         if isinstance(content, str):
             content = content.encode('utf8')
 
         if self._mode is not None and ('w' not in self._mode and
                                        'a' not in self._mode and
                                        'x' not in self._mode and
                                        '+' not in self._mode):
-            raise ValueError(f"Mode '{self._mode}' does not allow writing the file")
+            raise ValueError(f"Mode '{self._mode}' does not allow"
+                             f" writing the file")
         blob = self._bucket.blob(self._current_path)
         blob.upload_from_string(content)
 
     def _parse_bucket(self, path: str) -> Tuple[str, str]:
         """Given a path, return the bucket name and the file path as a tuple"""
         path = path.split(GoogleStorageInterface.PREFIX, 1)[-1]
         try:
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/interface/local_storage.py` & `cloudstorageio-1.2.9/cloudstorageio/interface/local_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """ Class LocalStorageInterface handles with local file/folder objects
 
     Class LocalStorageInterface contains
-                                        open method, which is the same python built-in 'open' method
-                                        isfile and isdir methods for checking object status
-                                        listdir method for listing folder's content
-                                        remove method for removing file or folder
+                open method, which is the same python built-in 'open' method
+                isfile and isdir methods for checking object status
+                listdir method for listing folder's content
+                remove method for removing file or folder
 """
 import os
 import shutil
+import warnings
 from typing import Optional, Union
 
 from cloudstorageio.tools.ci_collections import add_slash
 from cloudstorageio.tools.logger import logger
 
 
 class LocalStorageInterface:
 
     def __init__(self, **kwargs):
         self._mode = None
         self.path = None
         self.recursive = False
         self.include_folders = False
+        # EDITED: New variable was added.
+        self.include_files = True
         self._current_path = None
         self._current_path_with_backslash = None
 
     @property
     def path(self):
         if self._current_path is None:
             raise ValueError("Path name is not set")
@@ -32,34 +35,56 @@
 
     @path.setter
     def path(self, value):
         if value is None:
             self._current_path = None
             self._current_path_with_backslash = None
         else:
-            self._current_path = value[:-1] if (value.endswith('/') and value != '/') else value
+            self._current_path = value[:-1] if (value.endswith('/')
+                                                and value != '/') else value
             self._current_path_with_backslash = add_slash(self._current_path)
 
     def _populate_listdir(self):
-        """Appends each file.folder name to self._listdir"""
+        """Appends each file/folder name to self._listdir"""
+
+        if not self.include_files and not self.include_folders:
+            # EDITED: Warning was added.
+            warnings.warn('Neither folders nor files were included', Warning)
         if self.recursive:
-            for root, dirs, files in os.walk(self.path):
-                for name in files:
-                    self._listdir.append(os.path.join(root, name).split(self._current_path_with_backslash, 1)[1])
-                if self.include_folders:
-                    for name in dirs:
-                        self._listdir.append(str(os.path.join(root, name).split(self._current_path_with_backslash, 1)[1])
-                                             + '/')
+            self._populate_listdir_recursive()
         else:
-            for i in os.listdir(self.path):
-                if os.path.isdir(os.path.join(self.path, i)):
-                    if self.include_folders:
-                        self._listdir.append(add_slash(i))
-                else:
-                    self._listdir.append(i)
+            self._populate_listdir_not_recursive()
+
+    def _populate_listdir_not_recursive(self):
+        for i in os.listdir(self.path):
+            if os.path.isdir(os.path.join(self.path, i)):
+                if self.include_folders:
+                    self._listdir.append(add_slash(i))
+            else:
+                self._listdir.append(i)
+
+    def _populate_listdir_recursive(self):
+        for root, dirs, files in os.walk(self.path):
+            # EDITED: Following if condition was added.
+            if self.include_files:
+                self._include_files_in_listdir(files, root)
+            if self.include_folders:
+                self._include_folders_in_listdir(dirs, root)
+
+    def _include_folders_in_listdir(self, dirs, root):
+        for name in dirs:
+            self._listdir.append(
+                str(os.path.join(root, name).split(
+                    self._current_path_with_backslash, 1)[1]) + '/')
+
+    def _include_files_in_listdir(self, files, root):
+        for name in files:
+            self._listdir.append(
+                os.path.join(root, name).split(
+                    self._current_path_with_backslash, 1)[1])
 
     def _analyse_path(self, path: str):
         """From given path lists and detects object type (file/folder)"""
         self._isfile = False
         self._isdir = False
         self.recursive = False
         self.include_folders = False
@@ -83,35 +108,37 @@
             raise FileNotFoundError('No such file: {}'.format(self.path))
 
         with open(self.path, self._mode) as f:
             res = f.read()
         return res
 
     def write(self, content: Union[str, bytes]):
-        """ Writes text to a file on google storage
+        """ Writes text to a file on Google storage
         :param content: The content that should be written to a file
         :return: String content of the file specified in the file path argument
         """
         try:
             os.makedirs(os.path.dirname(self.path), exist_ok=True)
         except FileExistsError:
-            logger.info(f'File/folder conflict for {os.path.dirname(self.path)} path')
+            logger.info(f'File/folder conflict for '
+                        f'{os.path.dirname(self.path)} path')
             return None
 
         if self.isfile(self.path):
             ...
             # logger.info('Overwriting {} file'.format(self.path))
 
         if isinstance(content, str):
             content = content.encode('utf8')
         try:
             with open(self.path, self._mode) as f:
                 f.write(content)
         except IsADirectoryError:
-            logger.info(f'File/folder conflict for {os.path.dirname(self.path)} path')
+            logger.info(f'File/folder conflict for '
+                        f'{os.path.dirname(self.path)} path')
 
     def isfile(self, path: str):
         """Checks file existence for given path"""
         self._analyse_path(path)
         return self._isfile
 
     def isdir(self, path: str):
@@ -126,20 +153,23 @@
         if self._isfile:
             os.remove(self.path)
         elif self._isdir:
             shutil.rmtree(self.path)
         else:
             raise FileNotFoundError(f'No such file or dictionary: {path}')
 
-    def listdir(self, path: str, recursive: Optional[bool] = False, exclude_folders: Optional[bool] = False):
+    def listdir(self, path: str, recursive: Optional[bool] = False,
+                exclude_folders: Optional[bool] = False,
+                include_files: Optional[bool] = True):
         """Lists all files/folders of dictionary"""
 
         self._analyse_path(path)
         self.recursive = recursive
         self.include_folders = not exclude_folders
+        self.include_files = include_files
 
         if not self._isdir and not self._isfile:
             raise FileNotFoundError(f'No such file or dictionary: {self.path}')
 
         elif not self._isdir:
             raise NotADirectoryError(f"Not a directory: {self.path}")
 
@@ -148,8 +178,8 @@
 
     def __enter__(self):
         self._is_open = True
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._is_open = False
-        self.path = None
+        self.path = None
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/interface/s3.py` & `cloudstorageio-1.2.9/cloudstorageio/interface/s3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 """ Class S3Interface handles with S3 Storage files/folders
     S3Interface has
-                        read and write methods (can be accessed by open method)
-                        isfile and isdir methods for checking object status (file, folder)
-                        listdir method for listing folder's content
-                        remove method for removing file/folder
+            read and write methods (can be accessed by open method)
+            isfile and isdir methods for checking object status (file, folder)
+            listdir method for listing folder's content
+            remove method for removing file/folder
 
     Boto3 API itself doesn't have any concept of a "folder".
-        In S3Interface you can differentiate file/folder like in local environment
+    In S3Interface you can differentiate file/folder like in local environment
 
 """
 
 import io
 import os
+import warnings
 from typing import Tuple, Optional, Union
 
 import boto3
 from boto3.s3.transfer import TransferConfig
 
 from cloudstorageio.enums.enums import PrefixEnums
 from cloudstorageio.tools.ci_collections import add_slash
 
 
 class S3Interface:
     PREFIX = PrefixEnums.S3.value
 
     def __init__(self, **kwargs):
-        """Initializes S3Interface instance, creates session and resources for given credentials
+        """Initializes S3Interface instance, creates session and
+         resources for given credentials
         :param kwargs:
         """
 
-        # try to find necessary parameters from given kwargs, if not, assign none
+        # try to find necessary parameters from given kwargs,
+        # if not, assign none
         self._region = kwargs.pop('aws_region_name', None)
         self._acc_key = kwargs.pop('aws_access_key_id', None)
         self._acc_secret_key = kwargs.pop('aws_secret_access_key', None)
         self._acc_session_token = kwargs.pop('aws_session_token', None)
         if not self._region:
             self._region = os.environ.get('AWS_REGION_NAME')
         if not self._acc_key:
             self._acc_key = os.environ.get('AWS_ACCESS_KEY')
         if not self._acc_secret_key:
             self._acc_secret_key = os.environ.get('AWS_SECRET_ACCESS_KEY')
         if not self._acc_session_token:
             self._acc_session_token = os.environ.get('AWS_SESSION_TOKEN')
 
         # check given two access keys mutually existence
-        if (self._acc_secret_key and not self._acc_key) or (self._acc_key and not self._acc_secret_key):
-            raise ConnectionRefusedError('Please provide both aws_access_key_id and aws_secret_access_key')
-
-        self._session = boto3.session.Session(aws_access_key_id=self._acc_key,
-                                              aws_secret_access_key=self._acc_secret_key,
-                                              aws_session_token=self._acc_session_token,
-                                              region_name=self._region)
+        if (self._acc_secret_key and not self._acc_key) \
+                or (self._acc_key and not self._acc_secret_key):
+            raise ConnectionRefusedError('Please provide both '
+                                         'aws_access_key_id and '
+                                         'aws_secret_access_key')
+
+        self._session = boto3.session.Session(self._acc_key,
+                                              self._acc_secret_key,
+                                              self._acc_session_token,
+                                              self._region)
 
         self._encoding = 'utf8'
         self._s3 = self._session.resource('s3')
         self._client = self._session.client('s3')
         self._mode = None
         self._current_bucket = None
         self._current_path = None
@@ -74,33 +80,36 @@
 
     @property
     def path(self):
         if self._current_bucket is None:
             raise ValueError("Bucket name is not set")
         if self._current_path is None:
             raise ValueError("Path name is not set")
-        return f"{S3Interface.PREFIX}{self._current_bucket}/{self._current_path}"
+        return f"{S3Interface.PREFIX}{self._current_bucket}" \
+               f"{self._current_path}"
 
     @path.setter
     def path(self, value):
         if value is None:
             self._current_path = None
             self._current_bucket = None
         else:
             value = value[:-1] if value.endswith('/') else value
-            self._current_bucket, self._current_path = self._parse_bucket(value)
+            self._current_bucket, self._current_path = \
+                self._parse_bucket(value)
             self._current_path_with_backslash = add_slash(self._current_path)
 
     @staticmethod
     def get_bucket_region(bucket_name):
         """Get region name of specific bucket
         :param bucket_name: name of s3 bucket object
         :return:
         """
-        return boto3.client('s3').get_bucket_location(Bucket=bucket_name)['LocationConstraint']
+        return boto3.client('s3').get_bucket_location(
+            Bucket=bucket_name)['LocationConstraint']
 
     def _detect_blob_object_type(self):
         """Hidden method for detecting given blob object type (file or folder)
         :return:
         """
         if self._current_path in self._object_key_list:
             self._isfile = True
@@ -130,30 +139,33 @@
         self._listdir = list()
         self._object_exists = False
 
         self.path = path
 
         self._bucket = self._s3.Bucket(self._current_bucket)
         self._object = self._bucket.Object(self._current_path)
-        self._object_summary_list = self._bucket.objects.filter(Prefix=self._current_path)
+        self._object_summary_list = self._bucket.objects.filter(
+            Prefix=self._current_path)
 
         self._object_key_list = [obj.key for obj in self._object_summary_list]
 
     def _analyse_path(self, path: str):
-        """From given path create bucket, object, object_summaries, list and identify object type (file/folder)
+        """From given path create bucket, object, object_summaries, list
+         and identify object type (file/folder)
         :param path: full path of file/folder
         :return:
         """
         self._init_path(path)
 
         if self.only_bucket:
             self._isdir = True
         else:
-            self._object_key_list = [f.split(self._current_path_with_backslash, 1)[-1] for f in
-                                     self._object_key_list]
+            self._object_key_list = [f.split(
+                self._current_path_with_backslash, 1)[-1]
+                                     for f in self._object_key_list]
             self._detect_blob_object_type()
 
         while '' in self._object_key_list:
             self._object_key_list.remove('')
 
         for key_name in self._object_key_list:
             self._populate_listdir(key_name)
@@ -169,63 +181,101 @@
     def isdir(self, path: str) -> bool:
         """Checks dictionary existence for given path"""
         self._analyse_path(path)
         return self._isdir
 
     def folder_exists(self, bucket: str, path: str) -> bool:
         path = path.rstrip('/')
-        resp = self._client.list_objects(Bucket=bucket, Prefix=path, Delimiter='/', MaxKeys=1)
+        resp = self._client.list_objects(Bucket=bucket, Prefix=path,
+                                         Delimiter='/', MaxKeys=1)
         return 'CommonPrefixes' in resp
 
-    def listdir(self, path: str, include_files: bool = True, recursive: Optional[bool] = False,
+    def listdir(self, path: str, recursive: Optional[bool] = False,
+                include_files: bool = True,
                 exclude_folders: Optional[bool] = False) -> list:
         """Lists content for given folder path"""
         self._init_path(path)
         paginator = self._client.get_paginator('list_objects')
         folders = list()
         files = list()
+
+        # EDITED: Following variables were added.
+        subfolders_list = list()
+        files_list = list()
+
+        for f in self._object_key_list:
+            if f.endswith('/'):
+                subfolders_list.append(f.split('/')[-2] + '/')
+            else:
+                files_list.append(f.split('/')[-1])
+
         if self._current_path.endswith('/'):
             current_path = self._current_path
         else:
             current_path = self._current_path + '/'
         include_folders = not exclude_folders
         if recursive:
-            self._analyse_path(path)
-            if include_folders:
-                folders_list = [f for f in self._listdir if f.endswith('/')]
-                self._listdir = self._object_key_list + folders_list
-            else:
-                self._listdir = [f for f in self._object_key_list if not f.endswith('/')]
+            self._populate_listdir_recursive(files_list, include_files,
+                                             include_folders, path,
+                                             subfolders_list)
         else:
-            if include_folders:
-                if not self.folder_exists(bucket=self._current_bucket,
-                                          path=self._current_path):
-                    raise FileNotFoundError(
-                        f'No such file or dictionary: {path}')
-                if self._current_bucket == self._current_path:
-                    result = paginator.paginate(Bucket=self._current_bucket,
-                                                Delimiter='/')
-                    for prefix in result.search('CommonPrefixes'):
-                        folders.append(
-                            prefix.get('Prefix').split('/')[-2] + '/')
-                else:
-                    result = paginator.paginate(Bucket=self._current_bucket,
-                                                Delimiter='/',
-                                                Prefix=current_path)
-                    for prefix in result.search('CommonPrefixes'):
-                        if prefix is not None:
-                            folders.append(
-                                prefix.get('Prefix').split('/')[-2] + '/')
-            if include_files:
-                for object_summary in self._bucket.objects.filter(Prefix=current_path, Delimiter='/'):
-                    files.append(object_summary.key.split('/')[-1])
+            self._populate_listdir_not_recursive(current_path, files, folders,
+                                                 include_folders,
+                                                 include_files, paginator,
+                                                 path)
+        return self._listdir
 
-            self._listdir = folders + files
+    def _populate_listdir_not_recursive(self, current_path, files, folders,
+                                        include_folders, include_files,
+                                        paginator, path):
+        if include_folders:
+            if not self.folder_exists(bucket=self._current_bucket,
+                                      path=self._current_path):
+                raise FileNotFoundError(f'No such file or dictionary: {path}')
+            if self._current_bucket == self._current_path:
+                result = paginator.paginate(Bucket=self._current_bucket,
+                                            Delimiter='/')
+                for prefix in result.search('CommonPrefixes'):
+                    folders.append(prefix.get('Prefix').split('/')[-2] + '/')
+            else:
+                result = paginator.paginate(Bucket=self._current_bucket,
+                                            Delimiter='/', Prefix=current_path)
+                for prefix in result.search('CommonPrefixes'):
+                    # EDITED: Since in the absence of subfolders in
+                    # current_path the prefix value will be None,
+                    # calling get() method on NoneType object will
+                    # raise AttributeError.
+                    # Therefore, following if condition was added.
+                    if prefix is None:
+                        break
+                    folders.append(prefix.get('Prefix').split('/')[-2] + '/')
+        if include_files:
+            for object_summary in self._bucket.objects.filter(
+                    Prefix=current_path, Delimiter='/'):
+                files.append(object_summary.key.split('/')[-1])
+        self._listdir = folders + files
 
-        return self._listdir
+    def _populate_listdir_recursive(self, files_list, include_files,
+                                    include_folders, path, subfolders_list):
+        self._analyse_path(path)
+        if include_folders:
+            folders_list = [f for f in self._listdir if f.endswith('/')]
+            # EDITED: Since the case when recursive=True
+            # and include_files=False was not considered,
+            # following changes were made.
+            if include_files:
+                self._listdir = files_list + subfolders_list + folders_list
+            else:
+                self._listdir = subfolders_list + folders_list
+        else:
+            self._listdir = files_list
+            if not include_files:
+                # EDITED: Warning added.
+                warnings.warn('Neither folders nor files were included',
+                              Warning)
 
     def remove(self, path: str) -> None:
         """Deletes file/folder"""
         self._analyse_path(path)
         if not self._object_exists:
             raise FileNotFoundError(f"Object with path {path} does not exists")
 
@@ -248,38 +298,42 @@
         res = self._object.get()['Body'].read()
         if self._mode is not None and 'b' not in self._mode:
             try:
                 res = res.decode(self._encoding)
             except UnicodeDecodeError:
                 raise ValueError(f"The content cannot be decoded into a string"
                                  f" with encoding {self._encoding}."
-                                 f" Include 'b' on read mode to return the original bytes")
+                                 f" Include 'b' on read mode to return the"
+                                 f" original bytes")
         return res
 
-    def write(self, content: Union[str, bytes, io.IOBase], metadata: Optional[dict] = None,
+    def write(self, content: Union[str, bytes, io.IOBase],
+              metadata: Optional[dict] = None,
               acl: Optional[str] = 'private'):
 
         """Writes text to a file on s3
         :param content: The content that should be written to a file
         :param metadata: Metadata for file
-        :param acl: access control permission for written file ('private' by default)
+        :param acl: access control permission for written file
+         ('private' by default)
         :return: String content of the file specified in the file path argument
         """
         if self._isfile:
             ...
             # logger.info('Overwriting {} file'.format(self.path))
         if isinstance(content, str):
             content = content.encode('utf8')
         if not metadata:
             metadata = {}
         if self._mode is not None and ('w' not in self._mode and
                                        'a' not in self._mode and
                                        'x' not in self._mode and
                                        '+' not in self._mode):
-            raise ValueError(f"Mode '{self._mode}' does not allow writing the file")
+            raise ValueError(f"Mode '{self._mode}'"
+                             f" does not allow writing the file")
 
         self._object.put(ACL=acl, Body=content, Metadata=metadata)
 
     def upload(self, path,
                acl: Optional[str] = 'private'):
         """
         Used for uploading files from local to S3.
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/tools/ci_collections.py` & `cloudstorageio-1.2.9/cloudstorageio/tools/ci_collections.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     seq_len = len(seq)
     if n_chunks > seq_len:
         raise ValueError(f"The number of chunks ({n_chunks}) exceeds the"
                          f" length of the sequence ({seq_len})")
     chunk_len = seq_len // n_chunks + bool(seq_len % n_chunks)
     return [seq[i * chunk_len:chunk_len * (i + 1)]
             for i in range(n_chunks)
-            if seq[i * chunk_len:chunk_len * (i + 1)]]
+            if seq[i * chunk_len:chunk_len * (i + 1)]]
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio/tools/decorators.py` & `cloudstorageio-1.2.9/cloudstorageio/tools/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import copy
 import functools
 import hashlib
 import inspect
 import os
 import pickle
-import shutil
 import time
-from typing import Callable, Optional
+from typing import Callable
 
 from cloudstorageio.tools.logger import logger
 
 
 def timer(func) -> Callable:
     """A decorator which prints execution time of the decorated function"""
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         start_time = time.time()
         result = func(*args, **kwargs)
-        logger.info("Executed {} in {:.4f} seconds"
-              .format(func.__name__, (time.time() - start_time)))
+        logger.info("Executed {} in {:.4f} seconds".format(
+            func.__name__, (time.time() - start_time)))
         return result
     return wrapper
 
 
 def storage_cache_factory(path: str = '/tmp/cache') -> Callable:
     """Factory decorator for modifying the decorated function to cache
        and reuse results in a predefined path on the local storage
@@ -34,15 +33,16 @@
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             copy_args = copy.deepcopy(list(args))
 
             all_args = {}
             function_class_type = ''
 
-            # finding name of args and map name to value for having key value pair in the end
+            # finding name of args and map name to value for
+            # having key value pair in the end
             arg_specs = inspect.getfullargspec(func)
 
             # takes care of default arguments
             if arg_specs.defaults:
                 start_idx = len(arg_specs.defaults)
                 default_arg_list = list(arg_specs.defaults)
                 for i, arg_name in enumerate(arg_specs.args[-start_idx:]):
@@ -59,29 +59,30 @@
                     all_args[arg_name] = copy_args.pop(0)
 
             all_args.update(kwargs)
             all_args = ([(k, v) for k, v in all_args.items()])
             all_args = sorted(all_args)
             os.makedirs(path, exist_ok=True)
             hash_ = hashlib.sha256()
-            idx = str([func.__module__, func.__name__, function_class_type,  all_args])
+            idx = str([func.__module__, func.__name__, function_class_type,
+                       all_args])
             hash_.update(idx.encode('utf8'))
             key = hash_.hexdigest()
             filename = key + '.p'
             if filename in os.listdir(path):
                 logger.info('Reading from cache')
-                logger.warning("The output might be changed after being cached")
+                logger.warning("The output might be changed "
+                               "after being cached")
                 with open(os.path.join(path, filename), 'rb') as f:
                     res = pickle.load(f)
             else:
                 res = func(*args, **kwargs)
                 # print('Writing to cache')
                 with open(os.path.join(path, filename), 'wb') as f:
                     pickle.dump(res, f)
             return res
         return wrapper
     return decorator
 
 
 if __name__ == "__main__":
     pass
-
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio.egg-info/PKG-INFO` & `cloudstorageio-1.2.9/cloudstorageio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstorageio
-Version: 1.2.8
+Version: 1.2.9
 Home-page: https://github.com/cognaize/cloudstorageio
 Author: cognaize
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cloudstorageio
 
@@ -187,7 +187,11 @@
 ### [1.2.4] - 2020-11-10
 - Add option include_files for listdir
 ### [1.2.7] - 2022-10-05
 - Updated build to setuptools
 ### [1.2.8] - 2022-05-04
 - Fix error on listdir for s3 if the folder did not include subfolders
 - Add option include_files for listdir for non-recursive case
+### [1.2.9] - 2022-05-05
+- Add github workflows for merging
+- Update tests to use AWS mocker
+- Move moto dependency to dev-requirements
```

### Comparing `cloudstorageio-1.2.8/cloudstorageio.egg-info/SOURCES.txt` & `cloudstorageio-1.2.9/cloudstorageio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.8/docs/additional_docs.md` & `cloudstorageio-1.2.9/docs/additional_docs.md`

 * *Files identical despite different names*

### Comparing `cloudstorageio-1.2.8/setup.cfg` & `cloudstorageio-1.2.9/setup.cfg`

 * *Files identical despite different names*

