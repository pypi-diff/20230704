# Comparing `tmp/validio_cli-0.5.1.tar.gz` & `tmp/validio_cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.5.1.tar", max compression
+gzip compressed data, was "validio_cli-0.6.0.tar", max compression
```

## Comparing `validio_cli-0.5.1.tar` & `validio_cli-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11340 2023-06-16 09:49:52.554053 validio_cli-0.5.1/LICENSE
--rw-r--r--   0        0        0      227 2023-06-16 09:49:52.554053 validio_cli-0.5.1/README_PUBLIC.md
--rw-r--r--   0        0        0     1987 2023-06-16 09:50:03.229851 validio_cli-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6274 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/__init__.py
--rw-r--r--   0        0        0     2390 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/channels.py
--rw-r--r--   0        0        0    11640 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/code.py
--rw-r--r--   0        0        0     4335 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/config.py
--rw-r--r--   0        0        0     2499 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/credentials.py
--rw-r--r--   0        0        0     2306 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/destinations.py
--rw-r--r--   0        0        0     7429 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/incidents.py
--rw-r--r--   0        0        0     2336 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/metrics.py
--rw-r--r--   0        0        0     2867 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/notification_rules.py
--rw-r--r--   0        0        0     3334 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/recommendations.py
--rw-r--r--   0        0        0     2913 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/segmentations.py
--rw-r--r--   0        0        0     1902 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/segments.py
--rw-r--r--   0        0        0    26332 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/sources.py
--rw-r--r--   0        0        0     1174 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/users.py
--rw-r--r--   0        0        0     3743 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/validators.py
--rw-r--r--   0        0        0     2806 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/entities/windows.py
--rw-r--r--   0        0        0     3259 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/bin/main.py
--rw-r--r--   0        0        0     2587 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/components.py
--rw-r--r--   0        0        0      265 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/metadata.py
--rw-r--r--   0        0        0      630 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/namespace.py
--rw-r--r--   0        0        0     1382 2023-06-16 09:49:52.554053 validio_cli-0.5.1/validio_cli/schema.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-07-03 15:11:55.867966 validio_cli-0.6.0/LICENSE
+-rw-r--r--   0        0        0      227 2023-07-03 15:11:55.867966 validio_cli-0.6.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     1987 2023-07-03 15:12:08.231920 validio_cli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6274 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/__init__.py
+-rw-r--r--   0        0        0     2390 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    11640 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     4335 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     2506 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     2306 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/destinations.py
+-rw-r--r--   0        0        0     7429 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/incidents.py
+-rw-r--r--   0        0        0     2336 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/metrics.py
+-rw-r--r--   0        0        0     2867 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3334 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     2913 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0     1902 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/segments.py
+-rw-r--r--   0        0        0    26341 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1174 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     3743 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     2806 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     3259 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     2587 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/components.py
+-rw-r--r--   0        0        0      265 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/metadata.py
+-rw-r--r--   0        0        0      630 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/namespace.py
+-rw-r--r--   0        0        0     1382 2023-07-03 15:11:55.871966 validio_cli-0.6.0/validio_cli/schema.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.6.0/PKG-INFO
```

### Comparing `validio_cli-0.5.1/LICENSE` & `validio_cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/pyproject.toml` & `validio_cli-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-cli"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.5.1"
+version = "0.6.0"
 description = "CLI tool to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{include = "validio_cli"}]
 readme = "README_PUBLIC.md"
```

### Comparing `validio_cli-0.5.1/validio_cli/__init__.py` & `validio_cli-0.6.0/validio_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/channels.py` & `validio_cli-0.6.0/validio_cli/bin/entities/channels.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/code.py` & `validio_cli-0.6.0/validio_cli/bin/entities/code.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/config.py` & `validio_cli-0.6.0/validio_cli/bin/entities/config.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/credentials.py` & `validio_cli-0.6.0/validio_cli/bin/entities/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,12 +79,12 @@
         None,
     )
 
     if resolved_id is None:
         print(f"No {identifier_type} with name or id {identifier} found")
         return None
 
-    return None
+    return resolved_id
 
 
 if __name__ == "__main__":
     typer.run(app())
```

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/destinations.py` & `validio_cli-0.6.0/validio_cli/bin/entities/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/incidents.py` & `validio_cli-0.6.0/validio_cli/bin/entities/incidents.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/metrics.py` & `validio_cli-0.6.0/validio_cli/bin/entities/metrics.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/notification_rules.py` & `validio_cli-0.6.0/validio_cli/bin/entities/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/recommendations.py` & `validio_cli-0.6.0/validio_cli/bin/entities/recommendations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/segmentations.py` & `validio_cli-0.6.0/validio_cli/bin/entities/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/segments.py` & `validio_cli-0.6.0/validio_cli/bin/entities/segments.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/sources.py` & `validio_cli-0.6.0/validio_cli/bin/entities/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,15 @@
     resolved_credential_id = await credentials.get_credential_id(
         vc, cfg, credential_id, namespace
     )
     if resolved_credential_id is None:
         return
 
     await _infer_schema_snowflake(
-        vc, filename, credential_id, schema, database, table, role, warehouse
+        vc, filename, resolved_credential_id, schema, database, table, role, warehouse
     )
 
 
 @infer_schema_app.async_command(help="Infer Google BigQuery schema")
 async def bigquery(
     config_dir: str = ConfigDir,
     filename: Path = schema_filename_option("bigquery"),
```

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/users.py` & `validio_cli-0.6.0/validio_cli/bin/entities/users.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/validators.py` & `validio_cli-0.6.0/validio_cli/bin/entities/validators.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/entities/windows.py` & `validio_cli-0.6.0/validio_cli/bin/entities/windows.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/bin/main.py` & `validio_cli-0.6.0/validio_cli/bin/main.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/components.py` & `validio_cli-0.6.0/validio_cli/components.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/namespace.py` & `validio_cli-0.6.0/validio_cli/namespace.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/validio_cli/schema.py` & `validio_cli-0.6.0/validio_cli/schema.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.5.1/PKG-INFO` & `validio_cli-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-cli
-Version: 0.5.1
+Version: 0.6.0
 Summary: CLI tool to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

