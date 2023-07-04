# Comparing `tmp/inference-server-1.0.4.tar.gz` & `tmp/inference-server-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference-server-1.0.4.tar", last modified: Wed Jun 28 09:20:04 2023, max compression
+gzip compressed data, was "inference-server-1.0.5.tar", last modified: Tue Jul  4 10:05:26 2023, max compression
```

## Comparing `inference-server-1.0.4.tar` & `inference-server-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.721482 inference-server-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-28 09:19:51.000000 inference-server-1.0.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-28 09:19:51.000000 inference-server-1.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.717482 inference-server-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.717482 inference-server-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-28 09:19:51.000000 inference-server-1.0.4/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-28 09:19:51.000000 inference-server-1.0.4/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-28 09:19:51.000000 inference-server-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-28 09:19:51.000000 inference-server-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-28 09:19:51.000000 inference-server-1.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-28 09:19:51.000000 inference-server-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-28 09:19:51.000000 inference-server-1.0.4/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-06-28 09:20:04.721482 inference-server-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-28 09:19:51.000000 inference-server-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.721482 inference-server-1.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.721482 inference-server-1.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/inference_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/inference_server_testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-28 09:19:51.000000 inference-server-1.0.4/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-28 09:19:51.000000 inference-server-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 09:20:04.721482 inference-server-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.717482 inference-server-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.721482 inference-server-1.0.4/src/inference_server/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-28 09:19:51.000000 inference-server-1.0.4/src/inference_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-28 09:19:51.000000 inference-server-1.0.4/src/inference_server/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-28 09:19:51.000000 inference-server-1.0.4/src/inference_server/default_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 09:19:51.000000 inference-server-1.0.4/src/inference_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-28 09:19:51.000000 inference-server-1.0.4/src/inference_server/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.721482 inference-server-1.0.4/src/inference_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-06-28 09:20:04.000000 inference-server-1.0.4/src/inference_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-28 09:20:04.000000 inference-server-1.0.4/src/inference_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 09:20:04.000000 inference-server-1.0.4/src/inference_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-28 09:20:04.000000 inference-server-1.0.4/src/inference_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 09:20:04.000000 inference-server-1.0.4/src/inference_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 09:20:04.721482 inference-server-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-28 09:19:51.000000 inference-server-1.0.4/tests/test_inference_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-28 09:19:51.000000 inference-server-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.839121 inference-server-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 10:05:05.000000 inference-server-1.0.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-04 10:05:05.000000 inference-server-1.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.831121 inference-server-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.835121 inference-server-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-04 10:05:05.000000 inference-server-1.0.5/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-04 10:05:05.000000 inference-server-1.0.5/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-04 10:05:05.000000 inference-server-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-04 10:05:05.000000 inference-server-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-04 10:05:05.000000 inference-server-1.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-04 10:05:05.000000 inference-server-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-04 10:05:05.000000 inference-server-1.0.5/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-04 10:05:26.839121 inference-server-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-04 10:05:05.000000 inference-server-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.835121 inference-server-1.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.839121 inference-server-1.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/inference_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/inference_server_testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-04 10:05:05.000000 inference-server-1.0.5/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-04 10:05:05.000000 inference-server-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 10:05:26.839121 inference-server-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.835121 inference-server-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.839121 inference-server-1.0.5/src/inference_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-04 10:05:05.000000 inference-server-1.0.5/src/inference_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-04 10:05:05.000000 inference-server-1.0.5/src/inference_server/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-04 10:05:05.000000 inference-server-1.0.5/src/inference_server/default_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-04 10:05:05.000000 inference-server-1.0.5/src/inference_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-04 10:05:05.000000 inference-server-1.0.5/src/inference_server/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.839121 inference-server-1.0.5/src/inference_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-04 10:05:26.000000 inference-server-1.0.5/src/inference_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-04 10:05:26.000000 inference-server-1.0.5/src/inference_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:05:26.000000 inference-server-1.0.5/src/inference_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-04 10:05:26.000000 inference-server-1.0.5/src/inference_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-04 10:05:26.000000 inference-server-1.0.5/src/inference_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:05:26.839121 inference-server-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-04 10:05:05.000000 inference-server-1.0.5/tests/test_inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-04 10:05:05.000000 inference-server-1.0.5/tox.ini
```

### Comparing `inference-server-1.0.4/.flake8` & `inference-server-1.0.5/.flake8`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/.github/workflows/release-package.yml` & `inference-server-1.0.5/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/.github/workflows/test-package.yml` & `inference-server-1.0.5/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/.gitignore` & `inference-server-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/.pre-commit-config.yaml` & `inference-server-1.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/.readthedocs.yaml` & `inference-server-1.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/LICENSE` & `inference-server-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/LICENSE_HEADER.txt` & `inference-server-1.0.5/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/PKG-INFO` & `inference-server-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.0.4/README.md` & `inference-server-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/docs/conf.py` & `inference-server-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/docs/deployment.rst` & `inference-server-1.0.5/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/docs/hooks.rst` & `inference-server-1.0.5/docs/hooks.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/docs/introduction.rst` & `inference-server-1.0.5/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/docs/testing.rst` & `inference-server-1.0.5/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/pyproject.toml` & `inference-server-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     "wsgi-server",
 ]
 
 # Minimum supported Python version
 requires-python = ">=3.7"
 # All runtime dependencies that must be packaged, pin major version only.
 dependencies = [
+    "codetiming~=1.4",
     "importlib-metadata<4; python_version<'3.8'",
     "pluggy~=1.0",
     "werkzeug~=2.0",
 ]
 
 
 [project.urls]
```

### Comparing `inference-server-1.0.4/src/inference_server/__init__.py` & `inference-server-1.0.5/src/inference_server/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """
 
 import functools
 import http
 import logging
 from typing import TYPE_CHECKING
 
+import codetiming
 import werkzeug
 import werkzeug.exceptions
 from werkzeug.datastructures import MIMEAccept
 
 import inference_server._plugin
 from inference_server._plugin import hook as plugin_hook
 
@@ -72,22 +73,23 @@
 
 def _handle_invocations(request: werkzeug.Request) -> werkzeug.Response:
     """
     Handle an incoming inference POST request
 
     :param request: HTTP request data
     """
-    pm = inference_server._plugin.manager()
-    # Deserialize HTTP body payload (bytes) into input features
-    data = pm.hook.input_fn(input_data=request.data, content_type=request.content_type)
-    # Then use the model to make a prediction
-    prediction = pm.hook.predict_fn(data=data, model=_model())
-    # Then serialize the data as bytes. This is often (but not necessarily) JSON bytes.
-    prediction_bytes, content_type = pm.hook.output_fn(prediction=prediction, accept=request.accept_mimetypes)
-    return werkzeug.Response(prediction_bytes, mimetype=content_type)
+    with codetiming.Timer(text="Invocation took {:.3f} seconds", logger=logger.debug):
+        pm = inference_server._plugin.manager()
+        # Deserialize HTTP body payload (bytes) into input features
+        data = pm.hook.input_fn(input_data=request.data, content_type=request.content_type)
+        # Then use the model to make a prediction
+        prediction = pm.hook.predict_fn(data=data, model=_model())
+        # Then serialize the data as bytes. This is often (but not necessarily) JSON bytes.
+        prediction_bytes, content_type = pm.hook.output_fn(prediction=prediction, accept=request.accept_mimetypes)
+        return werkzeug.Response(prediction_bytes, mimetype=content_type)
 
 
 def _handle_ping(request: werkzeug.Request) -> werkzeug.Response:
     """
     Handle an incoming ping HEAD request
 
     :param request: HTTP request data
```

### Comparing `inference-server-1.0.4/src/inference_server/_plugin.py` & `inference-server-1.0.5/src/inference_server/_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/src/inference_server/default_plugin.py` & `inference-server-1.0.5/src/inference_server/default_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/src/inference_server/testing.py` & `inference-server-1.0.5/src/inference_server/testing.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/src/inference_server.egg-info/PKG-INFO` & `inference-server-1.0.5/src/inference_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.0.4/src/inference_server.egg-info/SOURCES.txt` & `inference-server-1.0.5/src/inference_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/tests/test_inference_server.py` & `inference-server-1.0.5/tests/test_inference_server.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.4/tox.ini` & `inference-server-1.0.5/tox.ini`

 * *Files identical despite different names*

