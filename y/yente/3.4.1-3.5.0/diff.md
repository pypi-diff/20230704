# Comparing `tmp/yente-3.4.1.tar.gz` & `tmp/yente-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.4.1.tar", last modified: Mon Jun  5 10:40:40 2023, max compression
+gzip compressed data, was "yente-3.5.0.tar", last modified: Tue Jul  4 08:39:49 2023, max compression
```

## Comparing `yente-3.4.1.tar` & `yente-3.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-05 10:38:38.000000 yente-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 10:38:38.000000 yente-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-05 10:40:40.241286 yente-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-05 10:38:38.000000 yente-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:40:40.241286 yente-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-05 10:38:38.000000 yente-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:38.000000 yente-3.4.1/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-05 10:38:38.000000 yente-3.4.1/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-05 10:38:38.000000 yente-3.4.1/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/data/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-05 10:38:38.000000 yente-3.4.1/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-05 10:38:38.000000 yente-3.4.1/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 10:38:38.000000 yente-3.4.1/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-05 10:38:38.000000 yente-3.4.1/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-05 10:38:38.000000 yente-3.4.1/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-05 10:38:38.000000 yente-3.4.1/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-05 10:38:38.000000 yente-3.4.1/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 10:38:38.000000 yente-3.4.1/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-05 10:38:38.000000 yente-3.4.1/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-05 10:38:38.000000 yente-3.4.1/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:40:40.241286 yente-3.4.1/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:38:46.000000 yente-3.4.1/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 10:40:40.000000 yente-3.4.1/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-04 08:38:02.000000 yente-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 08:38:02.000000 yente-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-04 08:39:49.863565 yente-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-04 08:38:02.000000 yente-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 08:39:49.863565 yente-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-04 08:38:02.000000 yente-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:38:02.000000 yente-3.5.0/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-04 08:38:02.000000 yente-3.5.0/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-04 08:38:02.000000 yente-3.5.0/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-04 08:38:02.000000 yente-3.5.0/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-04 08:38:02.000000 yente-3.5.0/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 08:38:02.000000 yente-3.5.0/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-04 08:38:02.000000 yente-3.5.0/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-04 08:38:02.000000 yente-3.5.0/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 08:38:02.000000 yente-3.5.0/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-04 08:38:02.000000 yente-3.5.0/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 08:38:02.000000 yente-3.5.0/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-04 08:38:02.000000 yente-3.5.0/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 08:38:02.000000 yente-3.5.0/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:39:49.863565 yente-3.5.0/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:38:17.000000 yente-3.5.0/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 08:39:49.000000 yente-3.5.0/yente.egg-info/top_level.txt
```

### Comparing `yente-3.4.1/LICENSE` & `yente-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/PKG-INFO` & `yente-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.4.1
+Version: 3.5.0
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.4.1/README.md` & `yente-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/setup.py` & `yente-3.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.4.1",
+    version="3.5.0",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
-        "followthemoney==3.4.0",
-        "nomenklatura==2.14.0",
+        "followthemoney==3.4.3",
+        "nomenklatura==3.1.0",
         "asyncstdlib==3.10.8",
         "aiocron==1.8",
         "aiocsv==1.2.4",
         "aiofiles==23.1.0",
-        "types-aiofiles==23.1.0.3",
+        "types-aiofiles==23.1.0.4",
         "aiohttp[speedups]==3.8.4",
         "elasticsearch[async]==8.8.0",
-        "fastapi==0.96.0",
+        "fastapi==0.99.1",
         "uvicorn[standard]==0.22.0",
         "python-multipart==0.0.6",
         "email-validator==2.0.0.post2",
         "structlog==23.1.0",
         "pyicu==2.11",
-        "jellyfish==0.11.2",
-        "orjson==3.9.0",
+        "jellyfish==1.0.0",
+        "orjson==3.9.1",
         "text-unidecode==1.3",
         "click==8.0.4",
         "normality==2.4.0",
         "languagecodes==1.1.1",
         "countrynames==1.15.0",
         "fingerprints==1.1.0",
         "pantomime==0.6.0",
```

### Comparing `yente-3.4.1/yente/app.py` & `yente-3.5.0/yente/app.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/cli.py` & `yente-3.5.0/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/data/__init__.py` & `yente-3.5.0/yente/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/data/common.py` & `yente-3.5.0/yente/data/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,27 +19,29 @@
     schema_: str = Field(..., example="LegalEntity", alias="schema")
     properties: EntityProperties = Field(..., example={"name": ["John Doe"]})
     datasets: List[str] = Field([], example=["us_ofac_sdn"])
     referents: List[str] = Field([], example=["ofac-1234"])
     target: bool = Field(False)
     first_seen: Optional[datetime] = Field(..., example=datetime.utcnow())
     last_seen: Optional[datetime] = Field(..., example=datetime.utcnow())
+    last_change: Optional[datetime] = Field(..., example=datetime.utcnow())
 
     @classmethod
     def from_entity(cls, entity: Entity) -> "EntityResponse":
         return cls.construct(
             id=entity.id,
-            caption=entity.caption,
+            caption=entity._caption,
             schema=entity.schema.name,
             properties=dict(entity.properties),
             datasets=list(entity.datasets),
             referents=list(entity.referents),
             target=entity.target,
-            first_seen=entity._first_seen or entity.first_seen,
-            last_seen=entity._last_seen or entity.last_seen,
+            first_seen=entity.first_seen,
+            last_seen=entity.last_seen,
+            last_change=entity.last_change,
         )
 
 
 EntityResponse.update_forward_refs()
 
 
 class ScoredEntityResponse(EntityResponse):
@@ -49,22 +51,23 @@
 
     @classmethod
     def from_entity_result(
         cls, entity: Entity, result: MatchingResult, threshold: float
     ) -> "ScoredEntityResponse":
         return cls.construct(
             id=entity.id,
-            caption=entity.caption,
+            caption=entity._caption,
             schema=entity.schema.name,
             properties=entity.properties,
             datasets=list(entity.datasets),
             referents=list(entity.referents),
             target=entity.target,
-            first_seen=entity._first_seen or entity.first_seen,
-            last_seen=entity._last_seen or entity.last_seen,
+            first_seen=entity.first_seen,
+            last_seen=entity.last_seen,
+            last_change=entity.last_change,
             score=result["score"],
             match=result["score"] >= threshold,
             features=result["features"],
         )
 
 
 class StatusResponse(BaseModel):
```

### Comparing `yente-3.4.1/yente/data/dataset.py` & `yente-3.5.0/yente/data/dataset.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/data/freebase.py` & `yente-3.5.0/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/data/loader.py` & `yente-3.5.0/yente/data/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 async def fetch_url_to_path(url: str, path: Path) -> None:
     async with http_session() as client:
         async with client.get(url) as resp:
             resp.raise_for_status()
             async with aiofiles.open(path, "wb") as outfh:
-                while chunk := await resp.content.read(BUFFER):
+                async for chunk in resp.content.iter_chunked(BUFFER):
                     await outfh.write(chunk)
 
 
 async def read_path_lines(path: Path) -> AsyncGenerator[Any, None]:
     async with aiofiles.open(path, "rb") as fh:
         async for line in fh:
             yield orjson.loads(line)
```

### Comparing `yente-3.4.1/yente/data/manifest.py` & `yente-3.5.0/yente/data/manifest.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/data/util.py` & `yente-3.5.0/yente/data/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/logs.py` & `yente-3.5.0/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/resources/favicon.ico` & `yente-3.5.0/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/routers/admin.py` & `yente-3.5.0/yente/routers/admin.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/routers/match.py` & `yente-3.5.0/yente/routers/match.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/routers/reconcile.py` & `yente-3.5.0/yente/routers/reconcile.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/routers/search.py` & `yente-3.5.0/yente/routers/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/routers/util.py` & `yente-3.5.0/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/scoring.py` & `yente-3.5.0/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/search/base.py` & `yente-3.5.0/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/search/indexer.py` & `yente-3.5.0/yente/search/indexer.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/search/mapping.py` & `yente-3.5.0/yente/search/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         "caption": make_field("keyword"),
         "datasets": make_keyword(),
         "referents": make_keyword(),
         "target": make_field("boolean"),
         "text": make_field("text"),
         SOUNDEX_FIELD: make_keyword(),
         NAME_PART_FIELD: make_keyword(),
+        "last_change": make_field("date", format=DATE_FORMAT),
         "last_seen": make_field("date", format=DATE_FORMAT),
         "first_seen": make_field("date", format=DATE_FORMAT),
         "properties": {"dynamic": "strict", "properties": prop_mapping},
     }
 
     for t in registry.groups.values():
         if t.group is None:
```

### Comparing `yente-3.4.1/yente/search/nested.py` & `yente-3.5.0/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/search/queries.py` & `yente-3.5.0/yente/search/queries.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/search/search.py` & `yente-3.5.0/yente/search/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente/settings.py` & `yente-3.5.0/yente/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def env_str(name: str, default: Optional[str] = None) -> Optional[str]:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.4.1"
+VERSION = "3.5.0"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE") or "yente"
 DESCRIPTION = """
@@ -124,14 +124,14 @@
 ES_USERNAME = env_str("YENTE_ELASTICSEARCH_USERNAME")
 ES_PASSWORD = env_str("YENTE_ELASTICSEARCH_PASSWORD")
 ES_CLOUD_ID = env_str("YENTE_ELASTICSEARCH_CLOUD_ID")
 ES_SNIFF = as_bool(env_str("YENTE_ELASTICSEARCH_SNIFF") or "false")
 ES_INDEX = env_str("YENTE_ELASTICSEARCH_INDEX", "yente")
 ES_SHARDS = int(env_str("YENTE_ELASTICSEARCH_SHARDS") or "1")
 ENTITY_INDEX = f"{ES_INDEX}-entities"
-INDEX_VERSION = "003"
+INDEX_VERSION = "004"
 
 LOG_JSON = as_bool(env_str("YENTE_LOG_JSON", "false"))
 LOG_LEVEL = logging.DEBUG if DEBUG else logging.INFO
 
 # Used to pad out first_seen, last_seen on static collections
 RUN_TIME = datetime.utcnow().isoformat()[:19]
```

### Comparing `yente-3.4.1/yente/util.py` & `yente-3.5.0/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente.egg-info/PKG-INFO` & `yente-3.5.0/yente.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.4.1
+Version: 3.5.0
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `yente-3.4.1/yente.egg-info/SOURCES.txt` & `yente-3.5.0/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yente-3.4.1/yente.egg-info/requires.txt` & `yente-3.5.0/yente.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-followthemoney==3.4.0
-nomenklatura==2.14.0
+followthemoney==3.4.3
+nomenklatura==3.1.0
 asyncstdlib==3.10.8
 aiocron==1.8
 aiocsv==1.2.4
 aiofiles==23.1.0
-types-aiofiles==23.1.0.3
+types-aiofiles==23.1.0.4
 aiohttp[speedups]==3.8.4
 elasticsearch[async]==8.8.0
-fastapi==0.96.0
+fastapi==0.99.1
 uvicorn[standard]==0.22.0
 python-multipart==0.0.6
 email-validator==2.0.0.post2
 structlog==23.1.0
 pyicu==2.11
-jellyfish==0.11.2
-orjson==3.9.0
+jellyfish==1.0.0
+orjson==3.9.1
 text-unidecode==1.3
 click==8.0.4
 normality==2.4.0
 languagecodes==1.1.1
 countrynames==1.15.0
 fingerprints==1.1.0
 pantomime==0.6.0
```

