# Comparing `tmp/mlserver-huggingface-1.3.5rc1.tar.gz` & `tmp/mlserver-huggingface-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-huggingface-1.3.5rc1.tar", last modified: Tue Jul  4 10:33:47 2023, max compression
+gzip compressed data, was "mlserver-huggingface-1.4.0.dev2.tar", last modified: Thu May  4 09:30:40 2023, max compression
```

## Comparing `mlserver-huggingface-1.3.5rc1.tar` & `mlserver-huggingface-1.4.0.dev2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:33:47.008606 mlserver-huggingface-1.3.5rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-04 10:33:47.008606 mlserver-huggingface-1.3.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:33:47.004606 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:33:47.008606 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/jsonlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/numpylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:33:47.008606 mlserver-huggingface-1.3.5rc1/mlserver_huggingface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-04 10:33:46.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-04 10:33:46.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:33:46.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 10:33:46.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-04 10:33:46.000000 mlserver-huggingface-1.3.5rc1/mlserver_huggingface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:33:47.008606 mlserver-huggingface-1.3.5rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-04 10:33:10.000000 mlserver-huggingface-1.3.5rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.794301 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/jsonlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/numpylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 09:30:40.000000 mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:40.798301 mlserver-huggingface-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-04 09:29:59.000000 mlserver-huggingface-1.4.0.dev2/setup.py
```

### Comparing `mlserver-huggingface-1.3.5rc1/LICENSE` & `mlserver-huggingface-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/PKG-INFO` & `mlserver-huggingface-1.4.0.dev2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-huggingface
-Version: 1.3.5rc1
+Version: 1.4.0.dev2
 Summary: HuggingFace runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # HuggingFace runtime for MLServer
         
@@ -17,24 +17,14 @@
         ```bash
         pip install mlserver mlserver-huggingface
         ```
         
         For further information on how to use MLServer with HuggingFace, you can check
         out this [worked out example](../../docs/examples/huggingface/README.md).
         
-        ## Content Types
-        
-        The HuggingFace runtime will always decode the input request using its own
-        built-in codec.
-        Therefore, [content type annotations](../../docs/user-guide/content-type) at
-        the request level will **be ignored**.
-        Not that this **doesn't include [input-level content
-        type](../../docs/user-guide/content-type#Codecs) annotations**, which will be
-        respected as usual.
-        
         ## Settings
         
         The HuggingFace runtime exposes a couple extra parameters which can be used to
         customise how the runtime behaves.
         These settings can be added under the `parameters.extra` section of your
         `model-settings.json` file, e.g.
```

### Comparing `mlserver-huggingface-1.3.5rc1/README.md` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-# HuggingFace runtime for MLServer
-
-This package provides a MLServer runtime compatible with HuggingFace Transformers.
-
-## Usage
-
-You can install the runtime, alongside `mlserver`, as:
-
-```bash
-pip install mlserver mlserver-huggingface
-```
-
-For further information on how to use MLServer with HuggingFace, you can check
-out this [worked out example](../../docs/examples/huggingface/README.md).
-
-## Content Types
-
-The HuggingFace runtime will always decode the input request using its own
-built-in codec.
-Therefore, [content type annotations](../../docs/user-guide/content-type) at
-the request level will **be ignored**.
-Not that this **doesn't include [input-level content
-type](../../docs/user-guide/content-type#Codecs) annotations**, which will be
-respected as usual.
-
-## Settings
-
-The HuggingFace runtime exposes a couple extra parameters which can be used to
-customise how the runtime behaves.
-These settings can be added under the `parameters.extra` section of your
-`model-settings.json` file, e.g.
-
-```{code-block} json
----
-emphasize-lines: 5-8
----
-{
-  "name": "qa",
-  "implementation": "mlserver_huggingface.HuggingFaceRuntime",
-  "parameters": {
-    "extra": {
-      "task": "question-answering",
-      "optimum_model": true
-    }
-  }
-}
-```
-
-````{note}
-These settings can also be injected through environment variables prefixed with `MLSERVER_MODEL_HUGGINGFACE_`, e.g.
-
-```bash
-MLSERVER_MODEL_HUGGINGFACE_TASK="question-answering"
-MLSERVER_MODEL_HUGGINGFACE_OPTIMUM_MODEL=true
-```
-````
-
-### Reference
-
-You can find the full reference of the accepted extra settings for the
-HuggingFace runtime below:
-
-```{eval-rst}
-
-.. autopydantic_settings:: mlserver_huggingface.settings.HuggingFaceSettings
-```
+Metadata-Version: 2.1
+Name: mlserver-huggingface
+Version: 1.4.0.dev2
+Summary: HuggingFace runtime for MLServer
+Home-page: https://github.com/SeldonIO/MLServer.git
+Author: Seldon Technologies Ltd.
+Author-email: hello@seldon.io
+License: Apache 2.0
+Description: # HuggingFace runtime for MLServer
+        
+        This package provides a MLServer runtime compatible with HuggingFace Transformers.
+        
+        ## Usage
+        
+        You can install the runtime, alongside `mlserver`, as:
+        
+        ```bash
+        pip install mlserver mlserver-huggingface
+        ```
+        
+        For further information on how to use MLServer with HuggingFace, you can check
+        out this [worked out example](../../docs/examples/huggingface/README.md).
+        
+        ## Settings
+        
+        The HuggingFace runtime exposes a couple extra parameters which can be used to
+        customise how the runtime behaves.
+        These settings can be added under the `parameters.extra` section of your
+        `model-settings.json` file, e.g.
+        
+        ```{code-block} json
+        ---
+        emphasize-lines: 5-8
+        ---
+        {
+          "name": "qa",
+          "implementation": "mlserver_huggingface.HuggingFaceRuntime",
+          "parameters": {
+            "extra": {
+              "task": "question-answering",
+              "optimum_model": true
+            }
+          }
+        }
+        ```
+        
+        ````{note}
+        These settings can also be injected through environment variables prefixed with `MLSERVER_MODEL_HUGGINGFACE_`, e.g.
+        
+        ```bash
+        MLSERVER_MODEL_HUGGINGFACE_TASK="question-answering"
+        MLSERVER_MODEL_HUGGINGFACE_OPTIMUM_MODEL=true
+        ```
+        ````
+        
+        ### Reference
+        
+        You can find the full reference of the accepted extra settings for the
+        HuggingFace runtime below:
+        
+        ```{eval-rst}
+        
+        .. autopydantic_settings:: mlserver_huggingface.settings.HuggingFaceSettings
+        ```
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/__init__.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/base.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 class MultiInputRequestCodec(RequestCodec):
     """
     Huggingface codecs is prefered, then mlserver's
     """
 
     DefaultCodec: Type["InputCodecTy"] = StringCodec
     InputCodecsWithPriority: List[Type[InputCodecTy]] = []
-    ContentType = ""
+    ContentType = StringCodec.ContentType
 
     @classmethod
     def _find_encode_codecs(
         cls, payload: Dict[str, Any]
     ) -> Dict[str, Union[Type["InputCodecTy"], "InputCodecTy", None]]:
         field_codec: Dict[str, Union[Type["InputCodecTy"], "InputCodecTy", None]] = {}
         for field, value in payload.items():
@@ -190,9 +190,9 @@
         PILImageCodec,
         HuggingfaceSingleJSONCodec,
         HuggingfaceListJSONCodec,
         HuggingfaceConversationCodec,
         NumpyListCodec,
         RawCodec,
     ]
-    ContentType = "hf"
+    ContentType = StringCodec.ContentType
     DefaultCodec = StringCodec
```

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/conversation.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/conversation.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/image.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/image.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/json.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/json.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/jsonlist.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/jsonlist.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/numpylist.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/numpylist.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/raw.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/raw.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/codecs/utils.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/codecs/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/common.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/common.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/errors.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/metadata.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/metadata.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/runtime.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Now we load the cached model which should not block asyncio
         self._model = load_pipeline_from_settings(self.hf_settings, self.settings)
         self._merge_metadata()
         return True
 
     async def predict(self, payload: InferenceRequest) -> InferenceResponse:
         # TODO: convert and validate?
-        kwargs = HuggingfaceRequestCodec.decode_request(payload)
+        kwargs = self.decode_request(payload, default_codec=HuggingfaceRequestCodec)
         args = kwargs.pop("args", [])
 
         array_inputs = kwargs.pop("array_inputs", [])
         if array_inputs:
             args = [list(array_inputs)] + args
         prediction = self._model(*args, **kwargs)
```

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface/settings.py` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface/settings.py`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/mlserver_huggingface.egg-info/SOURCES.txt` & `mlserver-huggingface-1.4.0.dev2/mlserver_huggingface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlserver-huggingface-1.3.5rc1/setup.py` & `mlserver-huggingface-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

