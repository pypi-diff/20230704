# Comparing `tmp/cval-lib-0.0.1.2.tar.gz` & `tmp/cval-lib-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.1.2.tar", last modified: Sun Jul  2 18:45:51 2023, max compression
+gzip compressed data, was "cval-lib-0.0.2.3.tar", last modified: Tue Jul  4 09:06:41 2023, max compression
```

## Comparing `cval-lib-0.0.1.2.tar` & `cval-lib-0.0.2.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5555 2023-07-02 18:44:46.000000 cval-lib-0.0.1.2/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.1.2/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.1.2/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1685 2023-07-02 18:45:46.000000 cval-lib-0.0.1.2/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.1.2/cval_lib/examples/embeddings.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.1.2/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2012 2023-07-02 18:34:57.000000 cval-lib-0.0.1.2/cval_lib/examples/on_pemise.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1306 2023-07-02 18:45:46.000000 cval-lib-0.0.1.2/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2743 2023-07-02 18:41:52.000000 cval-lib-0.0.1.2/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5155 2023-07-02 18:28:19.000000 cval-lib-0.0.1.2/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1875 2023-07-02 18:19:25.000000 cval-lib-0.0.1.2/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.1.2/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2478 2023-07-02 18:08:51.000000 cval-lib-0.0.1.2/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3040 2023-07-02 14:57:53.000000 cval-lib-0.0.1.2/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.1.2/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.1.2/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      993 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-02 18:43:19.000000 cval-lib-0.0.1.2/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5555 2023-07-02 18:44:46.000000 cval-lib-0.0.2.3/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.3/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.3/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1685 2023-07-02 18:45:46.000000 cval-lib-0.0.2.3/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.2.3/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.2.3/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2012 2023-07-02 18:34:57.000000 cval-lib-0.0.2.3/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1306 2023-07-02 18:45:46.000000 cval-lib-0.0.2.3/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.008082 cval-lib-0.0.2.3/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2898 2023-07-02 19:12:34.000000 cval-lib-0.0.2.3/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5155 2023-07-02 18:28:19.000000 cval-lib-0.0.2.3/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1884 2023-07-04 09:05:59.000000 cval-lib-0.0.2.3/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.3/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      946 2023-07-02 19:17:24.000000 cval-lib-0.0.2.3/cval_lib/handlers/frame.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2487 2023-07-04 09:05:59.000000 cval-lib-0.0.2.3/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3040 2023-07-02 14:57:53.000000 cval-lib-0.0.2.3/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.3/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.3/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.3/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1022 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-04 09:06:40.000000 cval-lib-0.0.2.3/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-04 09:06:41.012082 cval-lib-0.0.2.3/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-04 09:06:30.000000 cval-lib-0.0.2.3/setup.py
```

### Comparing `cval-lib-0.0.1.2/LICENSE` & `cval-lib-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/README.md` & `cval-lib-0.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/connection.py` & `cval-lib-0.0.2.3/cval_lib/connection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.3/cval_lib/examples/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/examples/embeddings.py` & `cval-lib-0.0.2.3/cval_lib/examples/embeddings.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.3/cval_lib/examples/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.3/cval_lib/examples/on_pemise.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/examples/result.py` & `cval-lib-0.0.2.3/cval_lib/examples/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.3/cval_lib/handlers/__async.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.2.3/cval_lib/handlers/_abstract_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,30 +32,32 @@
             params=None,
             auth=None,
             cookies=None,
             hooks=None,
             json=None,
         )
 
-    def _get(self, url: str, params=None):
+    def _get(self, url: str, params=None, stream=False):
         self.url = url
         self.method = 'get'
         self.params = params
+        self.stream = stream
 
     def _delete(self, url: str, params=None):
         self._get(url, params=params)
         self.method = 'delete'
 
-    def _post(self, url: str, json=None, params=None):
-        self._get(url, params=params)
+    def _post(self, url: str, json=None, params=None, stream=False, **files):
+        self._get(url, params=params, stream=stream)
         self.method = 'post'
         self.json = json
+        self.files = files
 
-    def _put(self, url: str, json=None, params=None):
-        self._post(url, json, params)
+    def _put(self, url: str, json=None, params=None, stream=False, **files):
+        self._post(url, json, params, stream=stream, **files)
         self.method = 'put'
 
     @staticmethod
     def validate_response(resp: Response):
         if resp.status_code >= 400:
             match resp.status_code:
                 case 422:
```

### Comparing `cval-lib-0.0.1.2/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.3/cval_lib/handlers/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/handlers/detection.py` & `cval-lib-0.0.2.3/cval_lib/handlers/detection.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from requests import Session
 
 from cval_lib.configs.main_config import MainConfig
 from cval_lib.handlers._abstract_handler import AbstractHandler
 from cval_lib.handlers.result import Result
 from cval_lib.models.detection import DetectionSamplingOnPremise
-from models.result import ResultResponse
+from cval_lib.models.result import ResultResponse
 
 
 class Detection(AbstractHandler):
     def __init__(
             self,
             session: Session,
     ):
```

### Comparing `cval-lib-0.0.1.2/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.3/cval_lib/handlers/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/handlers/result.py` & `cval-lib-0.0.2.3/cval_lib/handlers/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
 
 from requests import Session
 
-from configs.main_config import MainConfig
+from cval_lib.configs.main_config import MainConfig
 from cval_lib.handlers._abstract_handler import AbstractHandler
 from cval_lib.models.result import ResultResponse
 
 
 class Result(AbstractHandler):
     """
     The result is the entity in which the processing data is stored
```

### Comparing `cval-lib-0.0.1.2/cval_lib/models/dataset.py` & `cval-lib-0.0.2.3/cval_lib/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/models/detection.py` & `cval-lib-0.0.2.3/cval_lib/models/detection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/models/embedding.py` & `cval-lib-0.0.2.3/cval_lib/models/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib/models/result.py` & `cval-lib-0.0.2.3/cval_lib/models/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.1.2/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.2.3/cval_lib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ./cval_lib/examples/result.py
 ./cval_lib/handlers/__async.py
 ./cval_lib/handlers/__init__.py
 ./cval_lib/handlers/_abstract_handler.py
 ./cval_lib/handlers/dataset.py
 ./cval_lib/handlers/detection.py
 ./cval_lib/handlers/embedding.py
+./cval_lib/handlers/frame.py
 ./cval_lib/handlers/result.py
 ./cval_lib/models/__init__.py
 ./cval_lib/models/dataset.py
 ./cval_lib/models/detection.py
 ./cval_lib/models/embedding.py
 ./cval_lib/models/result.py
 ./cval_lib/patterns/__init__.py
```

