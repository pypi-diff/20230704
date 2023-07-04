# Comparing `tmp/aporia-3.3.0.tar.gz` & `tmp/aporia-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporia-3.3.0.tar", max compression
+gzip compressed data, was "aporia-3.4.0.tar", max compression
```

## Comparing `aporia-3.3.0.tar` & `aporia-3.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2968 2023-07-02 19:37:33.427724 aporia-3.3.0/README.md
--rw-r--r--   0        0        0      829 2023-07-02 19:37:33.427724 aporia-3.3.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-02 19:37:33.427724 aporia-3.3.0/src/aporia/__init__.py
--rw-r--r--   0        0        0      925 2023-07-02 19:37:33.427724 aporia-3.3.0/src/aporia/as_code/__init__.py
--rw-r--r--   0        0        0     1025 2023-07-02 19:37:33.427724 aporia-3.3.0/src/aporia/as_code/resources/base.py
--rw-r--r--   0        0        0     1706 2023-07-02 19:37:33.427724 aporia-3.3.0/src/aporia/as_code/resources/custom_metrics.py
--rw-r--r--   0        0        0     2370 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/as_code/resources/data_source.py
--rw-r--r--   0        0        0     7465 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/as_code/resources/dataset.py
--rw-r--r--   0        0        0     4660 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/as_code/resources/model.py
--rw-r--r--   0        0        0    12069 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/as_code/resources/monitor.py
--rw-r--r--   0        0        0     3052 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/as_code/resources/segment.py
--rw-r--r--   0        0        0     2187 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/as_code/resources/version.py
--rw-r--r--   0        0        0    37860 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/as_code/stack.py
--rw-r--r--   0        0        0        0 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/__init__.py
--rw-r--r--   0        0        0     3233 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/aporia_api.py
--rw-r--r--   0        0        0      723 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/base.py
--rw-r--r--   0        0        0     1531 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/client.py
--rw-r--r--   0        0        0     2148 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/custom_metrics.py
--rw-r--r--   0        0        0     1822 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/dashboards.py
--rw-r--r--   0        0        0     3610 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/data_sources.py
--rw-r--r--   0        0        0     6709 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/datasets.py
--rw-r--r--   0        0        0     1844 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/messaging.py
--rw-r--r--   0        0        0     6108 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/metrics.py
--rw-r--r--   0        0        0     6326 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/models.py
--rw-r--r--   0        0        0    86057 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/monitors.py
--rw-r--r--   0        0        0     3506 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/segments.py
--rw-r--r--   0        0        0     3048 2023-07-02 19:37:33.431724 aporia-3.3.0/src/aporia/sdk/versions.py
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 aporia-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-07-04 13:25:22.345978 aporia-3.4.0/README.md
+-rw-r--r--   0        0        0      829 2023-07-04 13:25:22.349979 aporia-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/__init__.py
+-rw-r--r--   0        0        0      925 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/__init__.py
+-rw-r--r--   0        0        0     1025 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/base.py
+-rw-r--r--   0        0        0     1706 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/custom_metrics.py
+-rw-r--r--   0        0        0     2370 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/data_source.py
+-rw-r--r--   0        0        0     7465 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/dataset.py
+-rw-r--r--   0        0        0     4660 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/model.py
+-rw-r--r--   0        0        0    12069 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/monitor.py
+-rw-r--r--   0        0        0     3052 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/segment.py
+-rw-r--r--   0        0        0     2187 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/version.py
+-rw-r--r--   0        0        0    37860 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/stack.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/__init__.py
+-rw-r--r--   0        0        0     3233 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/aporia_api.py
+-rw-r--r--   0        0        0      723 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/base.py
+-rw-r--r--   0        0        0     1531 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/client.py
+-rw-r--r--   0        0        0     2148 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/custom_metrics.py
+-rw-r--r--   0        0        0     1822 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/dashboards.py
+-rw-r--r--   0        0        0     3610 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/data_sources.py
+-rw-r--r--   0        0        0     6709 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/datasets.py
+-rw-r--r--   0        0        0     1844 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/messaging.py
+-rw-r--r--   0        0        0     6108 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/metrics.py
+-rw-r--r--   0        0        0     6326 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/models.py
+-rw-r--r--   0        0        0    86057 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/monitors.py
+-rw-r--r--   0        0        0     3506 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/segments.py
+-rw-r--r--   0        0        0     3048 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/versions.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 aporia-3.4.0/PKG-INFO
```

### Comparing `aporia-3.3.0/README.md` & `aporia-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/pyproject.toml` & `aporia-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aporia"
-version = "3.3.0"
+version = "3.4.0"
 description = ""
 authors = ["Aporia <support@aporia.com>"]
 readme = "README.md"
 packages = [
     { include = "aporia", from = "src" }
 ]
```

### Comparing `aporia-3.3.0/src/aporia/as_code/__init__.py` & `aporia-3.4.0/src/aporia/as_code/__init__.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/base.py` & `aporia-3.4.0/src/aporia/as_code/resources/base.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/custom_metrics.py` & `aporia-3.4.0/src/aporia/as_code/resources/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/data_source.py` & `aporia-3.4.0/src/aporia/as_code/resources/data_source.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/dataset.py` & `aporia-3.4.0/src/aporia/as_code/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/model.py` & `aporia-3.4.0/src/aporia/as_code/resources/model.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/monitor.py` & `aporia-3.4.0/src/aporia/as_code/resources/monitor.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/segment.py` & `aporia-3.4.0/src/aporia/as_code/resources/segment.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/resources/version.py` & `aporia-3.4.0/src/aporia/as_code/resources/version.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/as_code/stack.py` & `aporia-3.4.0/src/aporia/as_code/stack.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/aporia_api.py` & `aporia-3.4.0/src/aporia/sdk/aporia_api.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/base.py` & `aporia-3.4.0/src/aporia/sdk/base.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/client.py` & `aporia-3.4.0/src/aporia/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/custom_metrics.py` & `aporia-3.4.0/src/aporia/sdk/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/dashboards.py` & `aporia-3.4.0/src/aporia/sdk/dashboards.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/data_sources.py` & `aporia-3.4.0/src/aporia/sdk/data_sources.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/datasets.py` & `aporia-3.4.0/src/aporia/sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/messaging.py` & `aporia-3.4.0/src/aporia/sdk/messaging.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/metrics.py` & `aporia-3.4.0/src/aporia/sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/models.py` & `aporia-3.4.0/src/aporia/sdk/models.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/monitors.py` & `aporia-3.4.0/src/aporia/sdk/monitors.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/segments.py` & `aporia-3.4.0/src/aporia/sdk/segments.py`

 * *Files identical despite different names*

### Comparing `aporia-3.3.0/src/aporia/sdk/versions.py` & `aporia-3.4.0/src/aporia/sdk/versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,10 +86,10 @@
     def delete(self):
         raise NotImplementedError()
 
     @staticmethod
     def delete_by_id(client: Client, id: str):
         raise NotImplementedError()
 
-    def get_datasets(self) -> list[Dataset]:
+    def get_datasets(self) -> List[Dataset]:
         datasets = Dataset.get_all(client=self.client, model_version_id=self.id)
         return datasets
```

### Comparing `aporia-3.3.0/PKG-INFO` & `aporia-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporia
-Version: 3.3.0
+Version: 3.4.0
 Summary: 
 Author: Aporia
 Author-email: support@aporia.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

