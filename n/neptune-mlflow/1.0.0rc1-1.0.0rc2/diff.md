# Comparing `tmp/neptune_mlflow-1.0.0rc1.tar.gz` & `tmp/neptune_mlflow-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_mlflow-1.0.0rc1.tar", max compression
+gzip compressed data, was "neptune_mlflow-1.0.0rc2.tar", max compression
```

## Comparing `neptune_mlflow-1.0.0rc1.tar` & `neptune_mlflow-1.0.0rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      287 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     2497 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/README.md
--rw-r--r--   0        0        0     2558 2023-06-23 13:18:08.085669 neptune_mlflow-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2581 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/__init__.py
--rw-r--r--   0        0        0      778 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/__init__.py
--rw-r--r--   0        0        0     3287 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/artifact_strategy.py
--rw-r--r--   0        0        0      873 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/__init__.py
--rw-r--r--   0        0        0      875 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/config.py
--rw-r--r--   0        0        0     3308 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/exporter.py
--rw-r--r--   0        0        0     3141 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/fetcher.py
--rw-r--r--   0        0        0     2139 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/neptune_exporter.py
--rw-r--r--   0        0        0     2470 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/orchestrator.py
--rw-r--r--   0        0        0     1655 2023-06-23 13:17:51.113469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/sync.py
--rw-r--r--   0        0        0     1334 2023-06-23 13:17:51.117469 neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/version.py
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 neptune_mlflow-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      460 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     2497 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/README.md
+-rw-r--r--   0        0        0     2558 2023-06-28 12:46:04.623071 neptune_mlflow-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2581 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/__init__.py
+-rw-r--r--   0        0        0     3287 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/artifact_strategy.py
+-rw-r--r--   0        0        0      873 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/__init__.py
+-rw-r--r--   0        0        0      875 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/config.py
+-rw-r--r--   0        0        0     3359 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/exporter.py
+-rw-r--r--   0        0        0     3127 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/fetcher.py
+-rw-r--r--   0        0        0     2139 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/neptune_exporter.py
+-rw-r--r--   0        0        0     2551 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/orchestrator.py
+-rw-r--r--   0        0        0     1655 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/sync.py
+-rw-r--r--   0        0        0     1334 2023-06-28 12:45:47.098984 neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/version.py
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 neptune_mlflow-1.0.0rc2/PKG-INFO
```

### Comparing `neptune_mlflow-1.0.0rc1/LICENSE` & `neptune_mlflow-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/README.md` & `neptune_mlflow-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/pyproject.toml` & `neptune_mlflow-1.0.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 repository = "https://github.com/neptune-ai/neptune-mlflow"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations/mlflow/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-mlflow"
 readme = "README.md"
-version = "1.0.0-rc.1"
+version = "1.0.0-rc.2"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/__init__.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/__init__.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/artifact_strategy.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/artifact_strategy.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/__init__.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/config.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/config.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/exporter.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     def export_run_info(neptune_run: NeptuneRun, mlflow_run: MlflowRun) -> None:
         info = dict(mlflow_run.info)
 
         info["start_time"] = datetime.fromtimestamp(mlflow_run.info.start_time / 1e3)
         info["end_time"] = datetime.fromtimestamp(mlflow_run.info.end_time / 1e3)
 
         neptune_run["run_info"] = info
+        neptune_run["sys/name"] = info["run_name"]
 
     def export_run_data(self, neptune_run: NeptuneRun, mlflow_run: MlflowRun) -> None:
         data_dict = mlflow_run.data.to_dictionary()
         metric_keys = data_dict["metrics"].keys()
         del data_dict["metrics"]
 
         neptune_run["run_data"] = data_dict
```

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/components/fetcher.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/components/fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 __all__ = ["Fetcher"]
 
-from typing import MutableMapping
 from dataclasses import dataclass
 from typing import (
     List,
+    MutableMapping,
     Set,
 )
 
 import mlflow
 from mlflow.entities import Experiment
 from mlflow.entities import Run as MlflowRun
 from mlflow.entities import ViewType
```

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/neptune_exporter.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/neptune_exporter.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/orchestrator.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/orchestrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,18 @@
             if mlflow_run.info.run_id in fetched_data.neptune_run_ids:
                 click.echo(f"Ignoring mlflow_run '{mlflow_run.info.run_name}' since it already exists")
                 continue
 
             click.echo(f"Loading mlflow_run '{mlflow_run.info.run_name}'")
 
             with NeptuneRun(
-                project=self.config.project_name, api_token=self.config.api_token, custom_run_id=mlflow_run.info.run_id
+                project=self.config.project_name,
+                api_token=self.config.api_token,
+                custom_run_id=mlflow_run.info.run_id,
+                capture_hardware_metrics=False,
             ) as neptune_run:
                 try:
                     experiment = fetched_data.mlflow_experiments[mlflow_run.info.experiment_id]
                     self.exporter.export_experiment_metadata(neptune_run, experiment)
 
                     self.exporter.export_run_info(neptune_run, mlflow_run)
                     self.exporter.export_run_data(neptune_run, mlflow_run)
```

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/sync.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/sync.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/src/neptune_mlflow_exporter/impl/version.py` & `neptune_mlflow-1.0.0rc2/src/neptune_mlflow_exporter/impl/version.py`

 * *Files identical despite different names*

### Comparing `neptune_mlflow-1.0.0rc1/PKG-INFO` & `neptune_mlflow-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-mlflow
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: neptune.ai MLflow integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

