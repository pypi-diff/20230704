# Comparing `tmp/bmsdna_lakeapi-0.9.4.tar.gz` & `tmp/bmsdna_lakeapi-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.9.4.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.9.5.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.9.4.tar` & `bmsdna_lakeapi-0.9.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/LICENSE
--rw-r--r--   0        0        0     9068 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/README.md
--rw-r--r--   0        0        0      380 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1138 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      625 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     7186 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10721 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6256 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11183 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12623 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/datasource.py
--rw-r--r--   0        0        0     6839 2023-07-02 20:44:29.672917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/detail_endpoint.py
--rw-r--r--   0        0        0     9938 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6891 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6813 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4443 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3770 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3040 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2409 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1084 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     2017 2023-07-02 20:44:29.676917 bmsdna_lakeapi-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-04 07:28:40.653923 bmsdna_lakeapi-0.9.5/LICENSE
+-rw-r--r--   0        0        0     9068 2023-07-04 07:28:40.653923 bmsdna_lakeapi-0.9.5/README.md
+-rw-r--r--   0        0        0      380 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      625 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     7186 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10721 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6256 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11183 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12623 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/datasource.py
+-rw-r--r--   0        0        0     6839 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0    10094 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6891 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6813 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4443 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3770 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3040 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2409 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.5/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.9.4/LICENSE` & `bmsdna_lakeapi-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/README.md` & `bmsdna_lakeapi-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/datasource.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/datasource.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/detail_endpoint.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/detail_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,22 +142,23 @@
         limit: Optional[int] = 100,
         offset: Optional[int] = 0,
         select: Union[str, None] = Query(title="$select", alias="$select", default=None, include_in_schema=False),
         distinct: bool = Query(title="$distinct", alias="$distinct", default=False, include_in_schema=False),
         engine: Engines = Query(title="$engine", alias="$engine", default="duckdb", include_in_schema=False),
         format: Optional[OutputFileType] = "json",
         jsonify_complex: bool = Query(title="jsonify_complex", include_in_schema=has_complex, default=False),
+        chunk_size: int | None = Query(title="$chunk_size", include_in_schema=False, default=None),
     ):  # type: ignore
         logger.debug(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
 
         engine = engine or basic_config.default_engine
 
         logger.debug(f"Engine: {engine}")
-
-        with get_context_by_engine(engine, chunk_size=config.chunk_size or basic_config.default_chunk_size) as context:
+        real_chunk_size = chunk_size or config.chunk_size or basic_config.default_chunk_size
+        with get_context_by_engine(engine, chunk_size=real_chunk_size) as context:
             realdataframe = Datasource(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
             expr = await get_params_filter_expr(df.columns(), config, params)
```

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.4/pyproject.toml` & `bmsdna_lakeapi-0.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.9.4"
+version = "0.9.5"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.9.4/PKG-INFO` & `bmsdna_lakeapi-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.9.4
+Version: 0.9.5
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

