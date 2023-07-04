# Comparing `tmp/ghga_datasteward_kit-0.4.0.tar.gz` & `tmp/ghga_datasteward_kit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_datasteward_kit-0.4.0.tar", last modified: Mon Jun 19 13:53:03 2023, max compression
+gzip compressed data, was "ghga_datasteward_kit-0.4.1.tar", last modified: Mon Jul  3 16:04:59 2023, max compression
```

## Comparing `ghga_datasteward_kit-0.4.0.tar` & `ghga_datasteward_kit-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.630051 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/batch_s3_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/catalog_accession_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23226 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.630051 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 13:53:03.000000 ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-19 13:53:03.638051 ghga_datasteward_kit-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:53:03.634051 ghga_datasteward_kit-0.4.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/test_s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-19 13:52:53.000000 ghga_datasteward_kit-0.4.0/tests/test_size_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:04:59.330383 ghga_datasteward_kit-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-03 16:04:59.330383 ghga_datasteward_kit-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:04:59.326383 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/batch_s3_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/catalog_accession_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:04:59.330383 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20869 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:04:59.330383 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-03 16:04:59.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-03 16:04:59.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:04:59.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 16:04:59.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:04:59.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 16:04:59.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 16:04:59.000000 ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 16:04:59.330383 ghga_datasteward_kit-0.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:04:59.330383 ghga_datasteward_kit-0.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:04:59.330383 ghga_datasteward_kit-0.4.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/fixtures/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/test_file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/test_s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-03 16:04:47.000000 ghga_datasteward_kit-0.4.1/tests/test_size_adjustment.py
```

### Comparing `ghga_datasteward_kit-0.4.0/LICENSE` & `ghga_datasteward_kit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/PKG-INFO` & `ghga_datasteward_kit-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_datasteward_kit
-Version: 0.4.0
+Version: 0.4.1
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.0/README.md` & `ghga_datasteward_kit-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__init__.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A utils package for GHGA data stewards."""
+"""The command line interface of the package."""
 
-__version__ = "0.4.0"
+from .main import cli  # noqa: F401
```

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/__main__.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/batch_s3_upload.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/batch_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/catalog_accession_generator.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/catalog_accession_generator.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/__init__.py` & `ghga_datasteward_kit-0.4.1/tests/fixtures/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,10 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""The command line interface of the package."""
-
-from .main import cli  # noqa: F401
+"""Fixtures that are used in both integration and unit tests"""
```

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/file.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/file.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 
 """File related CLI"""
 from pathlib import Path
 
 import typer
 
-from ghga_datasteward_kit import batch_s3_upload, s3_upload
+from ghga_datasteward_kit import batch_s3_upload, file_ingest, s3_upload
 
 cli = typer.Typer()
 
 
 @cli.command()
 def upload(
     input_path: Path = typer.Option(..., help="Local path of the input file"),
@@ -54,7 +54,23 @@
 
     batch_s3_upload.main(
         file_overview_tsv=tsv,
         config_path=config_path,
         parallel_processes=parallel_processes,
         dry_run=dry_run,
     )
+
+
+@cli.command()
+def ingest_upload_metadata(
+    config_path: Path = typer.Option(..., help="Path to a config YAML."),
+):
+    """Upload all output metdata files from the given directory to the file ingest service"""
+
+    errors = file_ingest.main(config_path=config_path)
+
+    if errors:
+        print(f"Encountered {len(errors)} errors during processing.")
+        for file_path, cause in errors.items():
+            print(f" -{file_path}: {cause}")
+    else:
+        print("Sucessfully sent all file upload metadata for ingest.")
```

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/main.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/cli/metadata.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/cli/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Metadata related CLI"""
 from pathlib import Path
 
 import typer
+from ghga_transpiler.cli import transpile
 
 from ghga_datasteward_kit import metadata
 
 cli = typer.Typer()
 
+cli.command()(transpile)
+
 
 @cli.command()
 def submit(
     submission_title: str = typer.Option(..., help="The title of the submission."),
     submission_description: str = typer.Option(
         ..., help="The description of the submission."
     ),
```

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/config.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Collection of all config classes."""
 
+from ghga_datasteward_kit.file_ingest import IngestConfig
 from ghga_datasteward_kit.loading import LoadConfig
 from ghga_datasteward_kit.metadata import MetadataConfig
 from ghga_datasteward_kit.s3_upload import Config as S3UploadConfig
 
 CONFIG_CLASSES = {
     "s3_upload": S3UploadConfig,
     "metadata": MetadataConfig,
     "load": LoadConfig,
+    "ingest": IngestConfig,
 }
```

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/loading.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/loading.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/main.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/metadata.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/s3_upload.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/s3_upload.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,52 +16,46 @@
 
 """
 Custom script to encrypt data using Crypt4GH and directly uploading it to S3
 objectstorage.
 """
 
 import asyncio
-import base64
-import hashlib
-import json
 import logging
 import math
 import os
 import subprocess  # nosec
 import sys
-from dataclasses import dataclass
 from functools import partial
 from io import BufferedReader
 from pathlib import Path
 from time import time
-from typing import Any, Generator
+from typing import Generator
 from uuid import uuid4
 
 import crypt4gh.header  # type: ignore
 import crypt4gh.keys  # type: ignore
 import crypt4gh.lib  # type: ignore
-import requests  # type: ignore
+from ghga_connector.core.client import HttpxClientState, httpx_client
 from ghga_connector.core.file_operations import read_file_parts
-from ghga_connector.core.session import RequestsSession
 from hexkit.providers.s3 import S3Config, S3ObjectStorage  # type: ignore
 from nacl.bindings import crypto_aead_chacha20poly1305_ietf_encrypt
 from pydantic import BaseSettings, Field, SecretStr, validator
 
+from ghga_datasteward_kit import models
 from ghga_datasteward_kit.utils import load_config_yaml
 
 
-def configure_session() -> requests.Session:
+def configure_session():
     """Configure session with exponential backoff retry"""
-    RequestsSession.configure(6)
-    return RequestsSession.session
+    HttpxClientState.configure(6)
 
 
 LOGGER = logging.getLogger("s3_upload")
 PART_SIZE = 16 * 1024**2
-SESSION = configure_session()
 
 
 def expand_env_vars_in_path(path: Path) -> Path:
     """Expand environment variables in a Path."""
 
     with subprocess.Popen(  # nosec
         f"realpath {path}", shell=True, stdout=subprocess.PIPE
@@ -101,47 +95,14 @@
     def expand_env_vars_output_dir(
         cls, output_dir: Path
     ):  # pylint: disable=no-self-argument
         """Expand vars in path"""
         return expand_env_vars_in_path(output_dir)
 
 
-class Checksums:
-    """Container for checksum calculation"""
-
-    def __init__(self):
-        self.unencrypted_sha256 = hashlib.sha256()
-        self.encrypted_md5: list[str] = []
-        self.encrypted_sha256: list[str] = []
-
-    def __repr__(self) -> str:
-        return (
-            f"Unencrypted: {self.unencrypted_sha256.hexdigest()}\n"
-            + f"Encrypted MD5: {self.encrypted_md5}\n"
-            + f"Encrypted SHA256: {self.encrypted_sha256}"
-        )
-
-    def get(self):
-        """Return all checksums at the end of processing"""
-        return (
-            self.unencrypted_sha256.hexdigest(),
-            self.encrypted_md5,
-            self.encrypted_sha256,
-        )
-
-    def update_unencrypted(self, part: bytes):
-        """Update checksum for unencrypted file"""
-        self.unencrypted_sha256.update(part)
-
-    def update_encrypted(self, part: bytes):
-        """Update encrypted part checksums"""
-        self.encrypted_md5.append(hashlib.md5(part, usedforsecurity=False).hexdigest())
-        self.encrypted_sha256.append(hashlib.sha256(part).hexdigest())
-
-
 class ChunkedUploader:
     """Handler class dealing with upload functionality"""
 
     def __init__(
         self, input_path: Path, alias: str, config: Config, unencrypted_file_size: int
     ) -> None:
         self.alias = alias
@@ -200,15 +161,15 @@
     def __init__(  # pylint: disable=too-many-arguments
         self,
         config: Config,
         file_id: str,
         encrypted_file_size: int,
         file_secret: bytes,
         part_size: int,
-        target_checksums: Checksums,
+        target_checksums: models.Checksums,
     ) -> None:
         self.config = config
         self.storage = objectstorage(self.config)
         self.file_id = file_id
         self.file_size = encrypted_file_size
         self.file_secret = file_secret
         self.part_size = part_size
@@ -219,15 +180,16 @@
 
         for part_no, (start, stop) in enumerate(
             get_ranges(file_size=self.file_size, part_size=self.config.part_size),
             start=1,
         ):
             headers = {"Range": f"bytes={start}-{stop}"}
             LOGGER.debug("Downloading part number %i. %s", part_no, headers)
-            response = SESSION.get(download_url, timeout=60, headers=headers)
+            with httpx_client() as client:
+                response = client.get(download_url, timeout=60, headers=headers)
             yield response.content
 
     async def download(self):
         """Download file in parts and validate checksums"""
         LOGGER.info("(4/7) Downloading file %s for validation.", self.file_id)
         download_url = await self.storage.get_object_download_url(
             bucket_id=self.config.bucket_id, object_id=self.file_id
@@ -236,28 +198,28 @@
         decryptor = Decryptor(
             file_secret=self.file_secret, num_parts=num_parts, part_size=self.part_size
         )
         download_func = partial(self._download_parts, download_url=download_url)
         decryptor.process_parts(download_func)
         self.validate_checksums(checkums=decryptor.checksums)
 
-    def validate_checksums(self, checkums: Checksums):
+    def validate_checksums(self, checkums: models.Checksums):
         """Confirm checksums for upload and download match"""
         if not self.target_checksums.get() == checkums.get():
             raise ValueError(
                 f"Checksum mismatch:\nUpload:\n{checkums}\nDownload:\n{self.target_checksums}"
             )
         LOGGER.info("(6/7) Succesfully validated checksums for %s.", self.file_id)
 
 
 class Decryptor:
     """Handles on the fly decryption and checksum calculation"""
 
     def __init__(self, file_secret: bytes, num_parts: int, part_size: int) -> None:
-        self.checksums = Checksums()
+        self.checksums = models.Checksums()
         self.file_secret = file_secret
         self.num_parts = num_parts
         self.part_size = part_size
 
     def _decrypt(self, part: bytes):
         """Decrypt file part"""
         segments, incomplete_segment = get_segments(
@@ -320,15 +282,15 @@
 
 
 class Encryptor:
     """Handles on the fly encryption and checksum calculation"""
 
     def __init__(self, part_size: int):
         self.part_size = part_size
-        self.checksums = Checksums()
+        self.checksums = models.Checksums()
         self.file_secret = os.urandom(32)
         self.encrypted_file_size = 0
 
     def _encrypt(self, part: bytes):
         """Encrypt file part using secret"""
         segments, incomplete_segment = get_segments(
             part=part, segment_size=crypt4gh.lib.SEGMENT_SIZE
@@ -384,61 +346,14 @@
 
         if upload_buffer:
             self.checksums.update_encrypted(upload_buffer)
             self.encrypted_file_size += len(upload_buffer)
             yield upload_buffer
 
 
-@dataclass
-class Metadata:  # pylint: disable=too-many-instance-attributes
-    """Container class for output metadata"""
-
-    alias: str
-    file_uuid: str
-    original_path: Path
-    part_size: int
-    file_secret: bytes
-    checksums: Checksums
-    unencrypted_size: int
-    encrypted_size: int
-
-    def serialize(self, output_dir: Path):
-        """Serialize metadata to file"""
-
-        output: dict[str, Any] = {}
-        output["Alias"] = self.alias
-        output["File UUID"] = self.file_uuid
-        output["Original filesystem path"] = str(self.original_path.resolve())
-        output["Part Size"] = f"{self.part_size // 1024**2} MiB"
-        output["Unencrypted file size"] = self.unencrypted_size
-        output["Encrypted file size"] = self.encrypted_size
-        output["Symmetric file encryption secret"] = base64.b64encode(
-            self.file_secret
-        ).decode("utf-8")
-        (
-            unencrypted_checksum,
-            encrypted_md5_checksums,
-            encrypted_sha256_checksums,
-        ) = self.checksums.get()
-        output["Unencrypted file checksum"] = unencrypted_checksum
-        output["Encrypted file part checksums (MD5)"] = encrypted_md5_checksums
-        output["Encrypted file part checksums (SHA256)"] = encrypted_sha256_checksums
-
-        if not output_dir.exists():
-            output_dir.mkdir(parents=True)
-
-        output_path = output_dir / f"{self.alias}.json"
-
-        LOGGER.info("(7/7) Writing metadata to %s.", output_path)
-        # owner read-only
-        with output_path.open("w") as file:
-            json.dump(output, file, indent=2)
-        os.chmod(path=output_path, mode=0o400)
-
-
 class MultipartUpload:
     """Context manager to handle init + complete/abort for S3 multipart upload"""
 
     def __init__(
         self, config: Config, file_id: str, encrypted_file_size: int, part_size: int
     ) -> None:
         self.config = config
@@ -478,15 +393,16 @@
         try:
             upload_url = await self.storage.get_part_upload_url(
                 upload_id=self.upload_id,
                 bucket_id=self.config.bucket_id,
                 object_id=self.file_id,
                 part_number=part_number,
             )
-            SESSION.put(url=upload_url, data=part)
+            with httpx_client() as client:
+                client.put(url=upload_url, data=part)
         except (  # pylint: disable=broad-except
             Exception,
             KeyboardInterrupt,
         ) as exc:
             await self.storage.abort_multipart_upload(
                 upload_id=self.upload_id,
                 bucket_id=self.config.bucket_id,
@@ -624,25 +540,35 @@
         encrypted_file_size=uploader.encryptor.encrypted_file_size,
         file_secret=uploader.encryptor.file_secret,
         part_size=config.part_size,
         target_checksums=uploader.encryptor.checksums,
     )
     await downloader.download()
 
-    metadata = Metadata(
+    (
+        unencrypted_checksum,
+        encrypted_md5_checksums,
+        encrypted_sha256_checksums,
+    ) = uploader.encryptor.checksums.get()
+
+    metadata = models.OutputMetadata(
         alias=uploader.alias,
         file_uuid=uploader.file_id,
         original_path=input_path,
         part_size=config.part_size,
         file_secret=uploader.encryptor.file_secret,
-        checksums=uploader.encryptor.checksums,
+        unencrypted_checksum=unencrypted_checksum,
+        encrypted_md5_checksums=encrypted_md5_checksums,
+        encrypted_sha256_checksums=encrypted_sha256_checksums,
         unencrypted_size=file_size,
         encrypted_size=uploader.encryptor.encrypted_file_size,
     )
-    metadata.serialize(config.output_dir)
+    output_path = config.output_dir / f"{uploader.alias}.json"
+    LOGGER.info("(7/7) Writing metadata to %s.", output_path)
+    metadata.serialize(output_path)
 
 
 def main(input_path, alias: str, config_path: Path):
     """
     Custom script to encrypt data using Crypt4GH and directly uploading it to S3
     objectstorage.
     """
```

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit/utils.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/PKG-INFO` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-datasteward-kit
-Version: 0.4.0
+Version: 0.4.1
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.0/ghga_datasteward_kit.egg-info/SOURCES.txt` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,30 +3,34 @@
 setup.cfg
 setup.py
 ghga_datasteward_kit/__init__.py
 ghga_datasteward_kit/__main__.py
 ghga_datasteward_kit/batch_s3_upload.py
 ghga_datasteward_kit/catalog_accession_generator.py
 ghga_datasteward_kit/config.py
+ghga_datasteward_kit/file_ingest.py
 ghga_datasteward_kit/loading.py
 ghga_datasteward_kit/main.py
 ghga_datasteward_kit/metadata.py
+ghga_datasteward_kit/models.py
 ghga_datasteward_kit/s3_upload.py
 ghga_datasteward_kit/utils.py
 ghga_datasteward_kit.egg-info/PKG-INFO
 ghga_datasteward_kit.egg-info/SOURCES.txt
 ghga_datasteward_kit.egg-info/dependency_links.txt
 ghga_datasteward_kit.egg-info/entry_points.txt
 ghga_datasteward_kit.egg-info/not-zip-safe
 ghga_datasteward_kit.egg-info/requires.txt
 ghga_datasteward_kit.egg-info/top_level.txt
 ghga_datasteward_kit/cli/__init__.py
 ghga_datasteward_kit/cli/file.py
 ghga_datasteward_kit/cli/main.py
 ghga_datasteward_kit/cli/metadata.py
+tests/test_file_ingest.py
 tests/test_metadata.py
 tests/test_s3_upload.py
 tests/test_size_adjustment.py
 tests/fixtures/__init__.py
 tests/fixtures/config.py
+tests/fixtures/ingest.py
 tests/fixtures/metadata.py
 tests/fixtures/utils.py
```

### Comparing `ghga_datasteward_kit-0.4.0/setup.cfg` & `ghga_datasteward_kit-0.4.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	hexkit[mongodb,s3]==0.10.0
-	httpx==0.23.3
-	ghga-connector==0.3.3
-	metldata==0.2.3
+	ghga-connector==0.3.5
+	ghga-transpiler==1.0.3
+	metldata==0.3.6
 python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	ghga-datasteward-kit = ghga_datasteward_kit.__main__:run
 
 [options.extras_require]
```

### Comparing `ghga_datasteward_kit-0.4.0/setup.py` & `ghga_datasteward_kit-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/tests/fixtures/__init__.py` & `ghga_datasteward_kit-0.4.1/tests/fixtures/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fixtures that are used in both integration and unit tests"""
+"""Metadata paths for tests"""
+
+from tests.fixtures.utils import BASE_DIR
+
+METADATA_CONFIG_PATH = BASE_DIR / "metadata_config.yaml"
+ORIGINAL_METADATA_PATH = BASE_DIR / "original_metadata.yaml"
+ORIGINAL_MODEL_PATH = BASE_DIR / "original_model.yaml"
```

### Comparing `ghga_datasteward_kit-0.4.0/tests/fixtures/config.py` & `ghga_datasteward_kit-0.4.1/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/tests/fixtures/metadata.py` & `ghga_datasteward_kit-0.4.1/ghga_datasteward_kit/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Metadata paths for tests"""
+"""A utils package for GHGA data stewards."""
 
-from tests.fixtures.utils import BASE_DIR
-
-METADATA_CONFIG_PATH = BASE_DIR / "metadata_config.yaml"
-ORIGINAL_METADATA_PATH = BASE_DIR / "original_metadata.yaml"
-ORIGINAL_MODEL_PATH = BASE_DIR / "original_model.yaml"
+__version__ = "0.4.1"
```

### Comparing `ghga_datasteward_kit-0.4.0/tests/fixtures/utils.py` & `ghga_datasteward_kit-0.4.1/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/tests/test_metadata.py` & `ghga_datasteward_kit-0.4.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.0/tests/test_s3_upload.py` & `ghga_datasteward_kit-0.4.1/tests/test_s3_upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 """Testing the whole encryption, upload, validation flow"""
 
 import sys
 from pathlib import Path
 
 import pytest
+from ghga_connector.core.client import HttpxClientState
 from ghga_service_commons.utils.temp_files import big_temp_file  # type: ignore
 from hexkit.providers.s3.testutils import (  # type: ignore
     config_from_localstack_container,
 )
 from pydantic import SecretStr
 from testcontainers.localstack import LocalStackContainer  # type: ignore
 
@@ -32,14 +33,17 @@
 ALIAS = "test_file"
 BUCKET_ID = "test-bucket"
 
 
 @pytest.mark.asyncio
 async def test_process(config_fixture: Config):  # noqa: F811
     """Test whole upload/download process for s3_upload script"""
+
+    HttpxClientState.configure(3)
+
     with LocalStackContainer(image="localstack/localstack:0.14.2").with_services(
         "s3"
     ) as localstack:
         s3_config = config_from_localstack_container(localstack)
 
         config = config_fixture.copy(
             update={
```

### Comparing `ghga_datasteward_kit-0.4.0/tests/test_size_adjustment.py` & `ghga_datasteward_kit-0.4.1/tests/test_size_adjustment.py`

 * *Files identical despite different names*

