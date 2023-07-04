# Comparing `tmp/mlserver-alibi-detect-1.3.5rc1.tar.gz` & `tmp/mlserver-alibi-detect-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-alibi-detect-1.3.5rc1.tar", last modified: Tue Jul  4 10:33:55 2023, max compression
+gzip compressed data, was "mlserver-alibi-detect-1.4.0.dev2.tar", last modified: Thu May  4 09:30:37 2023, max compression
```

## Comparing `mlserver-alibi-detect-1.3.5rc1.tar` & `mlserver-alibi-detect-1.4.0.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:33:55.717546 mlserver-alibi-detect-1.3.5rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-04 10:33:10.000000 mlserver-alibi-detect-1.3.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-04 10:33:55.713545 mlserver-alibi-detect-1.3.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-04 10:33:10.000000 mlserver-alibi-detect-1.3.5rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:33:55.713545 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 10:33:10.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-04 10:33:10.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 10:33:10.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:33:55.713545 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-04 10:33:55.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-04 10:33:55.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:33:55.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 10:33:55.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 10:33:55.000000 mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:33:55.717546 mlserver-alibi-detect-1.3.5rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-04 10:33:10.000000 mlserver-alibi-detect-1.3.5rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/setup.py
```

### Comparing `mlserver-alibi-detect-1.3.5rc1/LICENSE` & `mlserver-alibi-detect-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.3.5rc1/PKG-INFO` & `mlserver-alibi-detect-1.4.0.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-detect
-Version: 1.3.5rc1
+Version: 1.4.0.dev2
 Summary: Alibi-Detect runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Detect runtime for MLServer
```

### Comparing `mlserver-alibi-detect-1.3.5rc1/README.md` & `mlserver-alibi-detect-1.4.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect/runtime.py` & `mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from pydantic.error_wrappers import ValidationError
 from typing import Optional, List, Dict
 from pydantic import BaseSettings, Field
 from functools import cached_property
 
 from alibi_detect.saving import load_detector
 
-import mlserver
 from mlserver.batching import BatchedRequests
 from mlserver.types import InferenceRequest, InferenceResponse
 from mlserver.settings import ModelSettings
 from mlserver.model import MLModel
 from mlserver.codecs import NumpyCodec, NumpyRequestCodec
 from mlserver.utils import get_model_uri
 from mlserver.errors import MLServerError, InferenceError
@@ -66,16 +65,14 @@
         self._batch: List[InferenceRequest] = []
         super().__init__(settings)
 
     async def load(self) -> bool:
         self._model_uri = await get_model_uri(self._settings)
         try:
             self._model = load_detector(self._model_uri)
-            mlserver.register("seldon_model_drift", "Drift metrics")
-
             # Check whether an online drift detector (i.e. has a save_state method)
             self._online = True if hasattr(self._model, "save_state") else False
         except (
             ValueError,
             FileNotFoundError,
             EOFError,
             NotImplementedError,
@@ -124,42 +121,25 @@
             X = [X]  # type: ignore[assignment]
 
         # Run detector inference
         pred = []
         for x in X:
             # Prediction
             try:
-                current_pred = self._model.predict(x, **predict_kwargs)
-                pred.append(current_pred)
-                self._log_metrics(current_pred)
+                pred.append(self._model.predict(x, **predict_kwargs))
             except (ValueError, IndexError) as e:
                 raise InferenceError(
                     f"Invalid predict parameters for model {self._settings.name}: {e}"
                 ) from e
             # Save state if necessary
             if self._should_save_state:
                 self._save_state()
 
         return self._encode_response(self._postproc_pred(pred))
 
-    def _log_metrics(self, current_pred: dict) -> None:
-        if "data" not in current_pred:
-            return
-
-        data = current_pred["data"]
-        if "is_drift" in data:
-            # NOTE: is_drift may be an array larger than 1 (e.g. if drift is
-            # provided per input feature) or a single-value integer
-            is_drift = data["is_drift"]
-            if isinstance(is_drift, int):
-                is_drift = [is_drift]
-
-            for is_drift_instance in is_drift:
-                mlserver.log(seldon_model_drift=is_drift_instance)
-
     def _encode_response(self, y: dict) -> InferenceResponse:
         outputs = []
         for key in y["data"]:
             outputs.append(
                 NumpyCodec.encode_output(name=key, payload=np.array(y["data"][key]))
             )
```

### Comparing `mlserver-alibi-detect-1.3.5rc1/mlserver_alibi_detect.egg-info/PKG-INFO` & `mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-detect
-Version: 1.3.5rc1
+Version: 1.4.0.dev2
 Summary: Alibi-Detect runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Detect runtime for MLServer
```

### Comparing `mlserver-alibi-detect-1.3.5rc1/setup.py` & `mlserver-alibi-detect-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

