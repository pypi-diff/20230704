# Comparing `tmp/apache-airflow-providers-sktvane-0.2.2.tar.gz` & `tmp/apache-airflow-providers-sktvane-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.2.2.tar", last modified: Tue Jun 13 05:57:57 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-1.0.0.tar", last modified: Tue Jul  4 09:00:03 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.2.2.tar` & `apache-airflow-providers-sktvane-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.351462 apache-airflow-providers-sktvane-0.2.2/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.351462 apache-airflow-providers-sktvane-0.2.2/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.351462 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/operator_nes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.704770 apache-airflow-providers-sktvane-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-04 09:00:03.704770 apache-airflow-providers-sktvane-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.692770 apache-airflow-providers-sktvane-1.0.0/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.692770 apache-airflow-providers-sktvane-1.0.0/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.696770 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.696770 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.700770 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.700770 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.700770 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/tests/operator_nes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:00:03.704770 apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-04 09:00:03.000000 apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-04 09:00:03.000000 apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:00:03.000000 apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-04 09:00:03.000000 apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 09:00:03.000000 apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 09:00:03.704770 apache-airflow-providers-sktvane-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 08:59:57.000000 apache-airflow-providers-sktvane-1.0.0/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.2.2/PKG-INFO` & `apache-airflow-providers-sktvane-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.2.2
+Version: 1.0.0
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.2.2/README.md` & `apache-airflow-providers-sktvane-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack_notifier.py` & `apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/macros/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/operators/nes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import logging
+import uuid
 from abc import ABCMeta, abstractmethod
+from datetime import datetime
 from time import sleep
 
 import requests
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.utils.context import Context
 from airflow.utils.decorators import apply_defaults
 
+from ..macros import gcp
+
 logger = logging.getLogger(name=__name__)
 
 
 class BaseProcessor(metaclass=ABCMeta):
     @abstractmethod
     def pre_process(self):
         pass
@@ -43,29 +48,21 @@
         return self.input_nb
 
     def post_process(self) -> None:
         pass
 
 
 class GCSProcessor(BaseProcessor):
-    import uuid
-    from datetime import datetime
-
-    from airflow.configuration import conf
-
-    from ..macros import gcp
-
-    _client = gcp.gcs_client()
-    _bucket = _client.get_bucket("nes_notebooks_seoul_28d")
-    _filename = f"{datetime.now().date()}/{uuid.uuid4()}.ipynb"
-    _gcs_blob = _bucket.blob(_filename)
-    _dags_folder = conf.get("core", "dags_folder")
-
     def __init__(self, input_nb: str):
         self.input_nb = input_nb
+        self._client = gcp.gcs_client()
+        self._bucket = self._client.get_bucket("nes_notebooks_seoul_28d")
+        self._filename = f"{datetime.now().date()}/{uuid.uuid4()}.ipynb"
+        self._gcs_blob = self._bucket.blob(self._filename)
+        self._dags_folder = conf.get("core", "dags_folder")
 
     def pre_process(self) -> None:
         self._gcs_blob.upload_from_filename(f"{self._dags_folder}/{self.input_nb}")
 
     def notebook_path(self) -> str:
         return f"gs://{self._bucket.name}/{self._filename}"
```

### Comparing `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/operator_nes_test.py` & `apache-airflow-providers-sktvane-1.0.0/airflow/providers/sktvane/tests/operator_nes_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.2.2
+Version: 1.0.0
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-1.0.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.2/setup.py` & `apache-airflow-providers-sktvane-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="0.2.2",
+    version="1.0.0",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

