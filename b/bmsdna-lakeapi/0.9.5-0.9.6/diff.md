# Comparing `tmp/bmsdna_lakeapi-0.9.5.tar.gz` & `tmp/bmsdna_lakeapi-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.9.5.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.9.6.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.9.5.tar` & `bmsdna_lakeapi-0.9.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-07-04 07:28:40.653923 bmsdna_lakeapi-0.9.5/LICENSE
--rw-r--r--   0        0        0     9068 2023-07-04 07:28:40.653923 bmsdna_lakeapi-0.9.5/README.md
--rw-r--r--   0        0        0      380 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1138 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      625 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     7186 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10721 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6256 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11183 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12623 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/datasource.py
--rw-r--r--   0        0        0     6839 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/detail_endpoint.py
--rw-r--r--   0        0        0    10094 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6891 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6813 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4443 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3770 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3040 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2409 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1084 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     2017 2023-07-04 07:28:40.657923 bmsdna_lakeapi-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/LICENSE
+-rw-r--r--   0        0        0     9235 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/README.md
+-rw-r--r--   0        0        0      380 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:39:00.683609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      625 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     7186 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10721 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6256 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11332 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12623 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/datasource.py
+-rw-r--r--   0        0        0     6889 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0    10169 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6891 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6813 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4553 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3813 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3040 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2409 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-07-04 13:39:00.687609 bmsdna_lakeapi-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    10434 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.6/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.9.5/LICENSE` & `bmsdna_lakeapi-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/README.md` & `bmsdna_lakeapi-0.9.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
 ## Even more features
 
 - Built-in paging, you can use limit/offset to control what you get
 - Full-text search using DuckDB's full-text search feature
 - jsonify_complex parameter to convert structs/lists to json, the client cannot handle structs/lists
 - Metadata endpoints to retrieve data types, string lengths and more
 - Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
+- Config in delta table as json, by using the lakeapi.config Table property. Example in the tests. This allows to have the config for the lakeapi along with your data
 - Good test coverage
 
 ## Further projects
 
 - [lakeapi2sql](https://github.com/bmsuisse/lakeapi2sql) Allows you to read from lake api and write to MS SQL Server
 
 ## Work in progress
```

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -100,15 +100,16 @@
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
 
 
 @dataclass
 class Config:
     name: str
     tag: str
-    datasource: DatasourceConfig
+    datasource: Optional[DatasourceConfig] = None
+    config_from_delta: Optional[bool] = False
     version: Optional[int] = 1
     api_method: Union[Literal["get", "post"], List[Literal["get", "post"]]] = "get"
     params: Optional[List[Union[Param, str]]] = None
     timestamp: Optional[datetime] = None
     cache_expiration_time_seconds: Optional[int] = CACHE_EXPIRATION_TIME_SECONDS
     allow_get_all_pages: Optional[bool] = False
     search: Optional[List[SearchConfig]] = None
@@ -126,26 +127,43 @@
         return "{}({})".format(type(self).__name__, ", ".join(kws))
 
     def __str__(self) -> str:
         kws = [f"{key}={value!r}" for key, value in self.__dict__.items()]
         return "{}({})".format(type(self).__name__, ", ".join(kws))
 
     @classmethod
-    def from_dict(
-        cls, config: Dict, basic_config: BasicConfig, table_names: List[tuple[int, str, str]]
-    ) -> List["Config"]:
+    def _from_dict(cls, config: Dict, basic_config: BasicConfig):
         name = config["name"]
         tag = config["tag"]
+        datasource: dict[str, Any] = config.get("datasource", {})
+        file_type: FileTypes = datasource.get("file_type", "delta")
+        uri = datasource.get("uri", tag + "/" + name)
+        if config.get("config_from_delta"):
+            assert file_type == "delta"
+            real_path = os.path.join(basic_config.data_path, uri)
+            if not os.path.exists(os.path.join(real_path, "_delta_log")):
+                logger.warning(f"Not a real delta path: {real_path}")
+            else:
+                import deltalake
+                import json
+
+                try:
+                    dt = deltalake.DeltaTable(real_path)
+                    cfg = json.loads(dt.metadata().configuration.get("lakeapi.config", "{}"))
+                    config = config | cfg  # simple merge. in that case we expect config to be in delta mainly
+                    datasource = config.get(
+                        "datasource", {"uri": uri, "file_type": file_type}
+                    )  # get data source again, could have select, columns etc
+                except json.JSONDecodeError as err:
+                    logger.warning(f"Not correct json: {real_path}\n{err}")
+
         version = config.get("version", 1)
         api_method = cast(Literal["post", "get"], config.get("api_method", "get"))
         params = config.get("params")
-        datasource = config["datasource"]
-        uri = datasource["uri"]
         assert isinstance(uri, str)
-        file_type = cast(FileTypes, datasource.get("file_type", "delta") if datasource else "delta")
         columns = datasource.get("columns") if datasource else None
         select = datasource.get("select") if datasource else None
         exclude = datasource.get("exclude") if datasource else None
         sortby = datasource.get("sortby") if datasource else None
         cache_expiration_time_seconds = (
             datasource.get("cache_expiration_time_seconds", CACHE_EXPIRATION_TIME_SECONDS) if datasource else None
         )
@@ -165,83 +183,71 @@
             sortby = [SortBy(by=s.get("by"), direction=s.get("direction")) for s in sortby]
 
         select = columns if columns else select
 
         if select:
             select = [Column(name=c.get("name"), alias=c.get("alias")) for c in select]
 
+        datasource_obj = DatasourceConfig(
+            uri=uri,
+            file_type=file_type,
+            select=select,
+            exclude=exclude,
+            in_memory=datasource.get("in_memory", False),
+            sortby=sortby,
+            filters=None,
+            cache_expiration_time_seconds=cache_expiration_time_seconds,
+        )
+        new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource_obj.uri)
+
+        return cls(
+            name=name,
+            tag=tag,
+            version=version,
+            search=search_config,
+            api_method=api_method,
+            engine=config.get("engine", None),
+            chunk_size=config.get("chunk_size", None),
+            params=new_params,  # type: ignore
+            allow_get_all_pages=config.get("allow_get_all_pages", False),
+            datasource=datasource_obj,
+            cache_expiration_time_seconds=cache_expiration_time_seconds,
+        )
+
+    @classmethod
+    def from_dict(
+        cls, config: Dict, basic_config: BasicConfig, table_names: List[tuple[int, str, str]]
+    ) -> List["Config"]:
+        name = config["name"]
+        tag = config["tag"]
+
         if name == "*":
+            uri = config.get("datasource", {}).get("uri", tag + "/*")
             assert uri.endswith("/*")
             folder = uri.rstrip("/*")
             root_folder = os.path.join(basic_config.data_path, folder)
             if not os.path.exists(root_folder):
                 logger.warning("Path not existing: " + root_folder)
                 return []
             else:
                 ls = []
                 for it in os.scandir(root_folder):
-                    res_name = (version, tag, it.name)
-                    if res_name not in table_names and (
+                    config_sub = config.copy()
+                    config_sub["name"] = it.name
+                    config_sub["datasource"]["uri"] = config["datasource"]["uri"].replace("/*", "/" + it.name)
+                    tbl_name = (config_sub.get("version", 1), config_sub["tag"], config_sub["name"])
+                    file_type = config_sub["datasource"].get("file_type", "delta")
+                    res_name = config_sub
+                    if tbl_name not in table_names and (
                         (it.is_dir() and file_type == "delta") or (it.is_file() and file_type != "delta")
                     ):
-                        datasource_obj = DatasourceConfig(
-                            uri=folder + "/" + it.name,
-                            file_type=file_type,
-                            select=select,
-                            exclude=exclude,
-                            in_memory=datasource.get("in_memory", False),
-                            sortby=sortby,
-                            filters=None,
-                            cache_expiration_time_seconds=cache_expiration_time_seconds,
-                        )
-                        new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource_obj.uri)
-                        ls.append(
-                            cls(
-                                name=it.name,
-                                tag=tag,
-                                version=version,
-                                engine=config.get("engine", None),
-                                chunk_size=config.get("chunk_size", None),
-                                api_method=api_method,
-                                search=search_config,
-                                params=new_params,  # type: ignore
-                                allow_get_all_pages=config.get("allow_get_all_pages", False),
-                                datasource=datasource_obj,
-                                cache_expiration_time_seconds=cache_expiration_time_seconds,
-                            )
-                        )
+                        ls.append(cls._from_dict(config_sub, basic_config))
             return ls
         else:
-            datasource_obj = DatasourceConfig(
-                uri=uri,
-                file_type=file_type,
-                select=select,
-                exclude=exclude,
-                in_memory=datasource.get("in_memory", False),
-                sortby=sortby,
-                filters=None,
-                cache_expiration_time_seconds=cache_expiration_time_seconds,
-            )
-            new_params = _with_implicit_parameters(_params, file_type, basic_config, datasource_obj.uri)
-
-            return [
-                cls(
-                    name=name,
-                    tag=tag,
-                    version=version,
-                    search=search_config,
-                    api_method=api_method,
-                    engine=config.get("engine", None),
-                    chunk_size=config.get("chunk_size", None),
-                    params=new_params,  # type: ignore
-                    allow_get_all_pages=config.get("allow_get_all_pages", False),
-                    datasource=datasource_obj,
-                    cache_expiration_time_seconds=cache_expiration_time_seconds,
-                )
-            ]
+            return [cls._from_dict(config, basic_config)]
 
     async def to_dict(self) -> dict:
         return self.__dict__
 
 
 class HttpConfig(TypedDict):
     bind: NotRequired[str]
```

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/datasource.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/datasource.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/detail_endpoint.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/detail_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     ) -> MetadataDetailResult:
         import json
 
         req.state.lake_api_basic_config = basic_config
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
         with DuckDbExecutionContext(basic_config.default_chunk_size) as context:
+            assert config.datasource is not None
             realdataframe = Datasource(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
 
             if not realdataframe.file_exists():
                 raise HTTPException(404)
             partition_columns = []
```

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 async def get_partitions(datasource: Datasource, params: BaseModel, config: Config) -> Optional[list]:
     parts = (
         await filter_partitions_based_on_params(
             DeltaTable(datasource.uri).metadata(),
             params.dict(exclude_unset=True) if params else {},
             config.params or [],
         )
-        if config.datasource.file_type == "delta"
+        if not config.datasource or config.datasource.file_type == "delta"
         else None
     )
     return parts
 
 
 def remove_search(prm_dict: dict, config: Config):
     if not config.search or len(prm_dict) == 0:
@@ -151,14 +151,15 @@
         logger.debug(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
 
         engine = engine or basic_config.default_engine
 
         logger.debug(f"Engine: {engine}")
         real_chunk_size = chunk_size or config.chunk_size or basic_config.default_chunk_size
         with get_context_by_engine(engine, chunk_size=real_chunk_size) as context:
+            assert config.datasource is not None
             realdataframe = Datasource(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
             expr = await get_params_filter_expr(df.columns(), config, params)
```

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/route.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                 cast(list[Literal["get", "post"]], [config.api_method])
                 if isinstance(config.api_method, str)
                 else config.api_method
             )
             try:
                 from bmsdna.lakeapi.core.datasource import Datasource
 
+                assert config.datasource is not None
                 realdataframe = Datasource(
                     config.version_str, config.tag, config.name, config.datasource, context, basic_config
                 )
                 if not realdataframe.file_exists():
                     logger.warning(
                         f"Could not get response type for f{config.route}. Path does not exist:{realdataframe.uri}"
                     )
@@ -97,14 +98,15 @@
         @router.on_event("startup")
         @_repeat_every(seconds=60 * 60)  # 1 hour
         def _persist_search_endpoints() -> None:
             for config in configs:
                 if config.search:
                     from bmsdna.lakeapi.core.datasource import Datasource
 
+                    assert config.datasource is not None
                     realdataframe = Datasource(
                         config.version_str, config.tag, config.name, config.datasource, context, basic_config
                     )
                     if realdataframe.file_exists():
                         with get_context_by_engine(
                             basic_config.default_engine, basic_config.default_chunk_size
                         ) as ctx:
```

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from bmsdna.lakeapi.context import get_context_by_engine, Engines
 
 sql_contexts: dict[str, ExecutionContext] = {}
 
 
 def init_duck_con(con: ExecutionContext, basic_config: BasicConfig, configs: Configs):
     for cfg in configs:
+        assert cfg.datasource is not None
         df = Datasource(cfg.version_str, cfg.tag, cfg.name, cfg.datasource, con, basic_config)
         if df.file_exists():
             con.register_datasource(df.tablename, df.uri, df.config.file_type, None)
 
 
 def get_sql_context(engine: Engines, basic_config: BasicConfig, configs: Configs):
     global sql_contexts
```

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.9.6/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.5/pyproject.toml` & `bmsdna_lakeapi-0.9.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.9.5"
+version = "0.9.6"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.9.5/PKG-INFO` & `bmsdna_lakeapi-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.9.5
+Version: 0.9.6
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -247,14 +247,15 @@
 ## Even more features
 
 - Built-in paging, you can use limit/offset to control what you get
 - Full-text search using DuckDB's full-text search feature
 - jsonify_complex parameter to convert structs/lists to json, the client cannot handle structs/lists
 - Metadata endpoints to retrieve data types, string lengths and more
 - Easily expose entire folders by using a "\*" wildcard in both the name and the datasource.uri config, see example in the config above
+- Config in delta table as json, by using the lakeapi.config Table property. Example in the tests. This allows to have the config for the lakeapi along with your data
 - Good test coverage
 
 ## Further projects
 
 - [lakeapi2sql](https://github.com/bmsuisse/lakeapi2sql) Allows you to read from lake api and write to MS SQL Server
 
 ## Work in progress
```

