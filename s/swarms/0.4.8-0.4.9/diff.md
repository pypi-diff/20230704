# Comparing `tmp/swarms-0.4.8.tar.gz` & `tmp/swarms-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.4.8.tar", last modified: Tue Jul  4 18:46:09 2023, max compression
+gzip compressed data, was "swarms-0.4.9.tar", last modified: Tue Jul  4 19:13:28 2023, max compression
```

## Comparing `swarms-0.4.8.tar` & `swarms-0.4.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.011498 swarms-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 18:45:59.000000 swarms-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:46:09.011498 swarms-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 18:45:59.000000 swarms-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:59.000000 swarms-0.4.8/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 18:45:59.000000 swarms-0.4.8/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 18:45:59.000000 swarms-0.4.8/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 18:45:59.000000 swarms-0.4.8/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:46:09.011498 swarms-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 18:45:59.000000 swarms-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/auto_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/metaprompt_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/agents/workers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/agents/workers/omni_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70834 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.011498 swarms-0.4.8/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 18:45:59.000000 swarms-0.4.8/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:46:09.007498 swarms-0.4.8/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 18:46:09.000000 swarms-0.4.8/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 18:46:08.000000 swarms-0.4.8/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.178705 swarms-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 19:13:18.000000 swarms-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 19:13:28.178705 swarms-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-04 19:13:18.000000 swarms-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.174705 swarms-0.4.9/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:18.000000 swarms-0.4.9/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-04 19:13:18.000000 swarms-0.4.9/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-04 19:13:18.000000 swarms-0.4.9/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 19:13:18.000000 swarms-0.4.9/api/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:13:28.178705 swarms-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 19:13:18.000000 swarms-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.174705 swarms-0.4.9/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.174705 swarms-0.4.9/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.174705 swarms-0.4.9/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/workers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/workers/auto_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/workers/metaprompt_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.174705 swarms-0.4.9/swarms/agents/workers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/workers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/workers/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77147 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/agents/workers/omni_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.174705 swarms-0.4.9/swarms/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70834 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.178705 swarms-0.4.9/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-07-04 19:13:18.000000 swarms-0.4.9/swarms/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:13:28.174705 swarms-0.4.9/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-04 19:13:28.000000 swarms-0.4.9/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-04 19:13:28.000000 swarms-0.4.9/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:13:28.000000 swarms-0.4.9/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 19:13:28.000000 swarms-0.4.9/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 19:13:28.000000 swarms-0.4.9/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.4.8/LICENSE` & `swarms-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/PKG-INFO` & `swarms-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.8
+Version: 0.4.9
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.8/README.md` & `swarms-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/api/container.py` & `swarms-0.4.9/api/container.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/api/main.py` & `swarms-0.4.9/api/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/api/worker.py` & `swarms-0.4.9/api/worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/setup.py` & `swarms-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.4.8',
+  version = '0.4.9',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.4.8/swarms/agents/swarms.py` & `swarms-0.4.9/swarms/agents/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/agents/workers/agents.py` & `swarms-0.4.9/swarms/agents/workers/agents.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/agents/workers/auto_agent.py` & `swarms-0.4.9/swarms/agents/workers/auto_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/agents/workers/metaprompt_agent.py` & `swarms-0.4.9/swarms/agents/workers/metaprompt_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/agents/workers/multi_modal.py` & `swarms-0.4.9/swarms/agents/workers/multi_modal.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/agents/workers/omni_agent.py` & `swarms-0.4.9/swarms/agents/workers/omni_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/tools/main.py` & `swarms-0.4.9/swarms/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/utils/ansi.py` & `swarms-0.4.9/swarms/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms/utils/utils.py` & `swarms-0.4.9/swarms/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,37 +203,37 @@
 #+=============================> ANSI Ending
 
 
 #================================> upload base
 
 from abc import ABC, abstractmethod, abstractstaticmethod
 
-from env import DotEnv
+# from env import DotEnv
 
 STATIC_DIR = "static"
 
 
 class AbstractUploader(ABC):
     @abstractmethod
     def upload(self, filepath: str) -> str:
         pass
 
     @abstractstaticmethod
-    def from_settings(settings: DotEnv) -> "AbstractUploader":
+    def from_settings() -> "AbstractUploader":
         pass
 
 #================================> upload end
 
 
 #========================= upload s3
 import os
 
 import boto3
 
-from env import DotEnv
+# from env import DotEnv
 
 
 class S3Uploader(AbstractUploader):
     def __init__(self, accessKey: str, secretKey: str, region: str, bucket: str):
         self.accessKey = accessKey
         self.secretKey = secretKey
         self.region = region
@@ -243,18 +243,18 @@
             aws_access_key_id=self.accessKey,
             aws_secret_access_key=self.secretKey,
         )
 
     @staticmethod
     def from_settings(settings: DotEnv) -> "S3Uploader":
         return S3Uploader(
-            settings["AWS_ACCESS_KEY_ID"],
-            settings["AWS_SECRET_ACCESS_KEY"],
-            settings["AWS_REGION"],
-            settings["AWS_S3_BUCKET"],
+            os.environ["AWS_ACCESS_KEY_ID"],
+            os.environ["AWS_SECRET_ACCESS_KEY"],
+            os.environ["AWS_REGION"],
+            os.environ["AWS_S3_BUCKET"],
         )
 
     def get_url(self, object_name: str) -> str:
         return f"https://{self.bucket}.s3.{self.region}.amazonaws.com/{object_name}"
 
     def upload(self, filepath: str) -> str:
         object_name = os.path.basename(filepath)
@@ -264,15 +264,15 @@
 #========================= upload s3
 
 #========================> upload/static
 import os
 import shutil
 from pathlib import Path
 
-from env import DotEnv
+# from env import DotEnv
 
 
 class StaticUploader(AbstractUploader):
     def __init__(self, server: str, path: Path, endpoint: str):
         self.server = server
         self.path = path
         self.endpoint = endpoint
@@ -300,15 +300,15 @@
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Dict
 
 import requests
 
-from env import settings
+# from env import settings
 
 
 class FileType(Enum):
     IMAGE = "image"
     AUDIO = "audio"
     VIDEO = "video"
     DATAFRAME = "dataframe"
```

### Comparing `swarms-0.4.8/swarms.egg-info/PKG-INFO` & `swarms-0.4.9/swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.4.8
+Version: 0.4.9
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.4.8/swarms.egg-info/SOURCES.txt` & `swarms-0.4.9/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.4.8/swarms.egg-info/requires.txt` & `swarms-0.4.9/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

