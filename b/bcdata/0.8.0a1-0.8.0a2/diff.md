# Comparing `tmp/bcdata-0.8.0a1.tar.gz` & `tmp/bcdata-0.8.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdata-0.8.0a1.tar", last modified: Thu Jun 29 21:34:51 2023, max compression
+gzip compressed data, was "bcdata-0.8.0a2.tar", last modified: Mon Jul  3 22:37:14 2023, max compression
```

## Comparing `bcdata-0.8.0a1.tar` & `bcdata-0.8.0a2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.740166 bcdata-0.8.0a1/
--rw-r--r--   0 snorris    (501) staff       (20)     7126 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/CHANGES.txt
--rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.8.0a1/LICENSE.txt
--rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-06-29 21:34:51.740002 bcdata-0.8.0a1/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)    15657 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/README.md
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.738242 bcdata-0.8.0a1/bcdata/
--rw-r--r--   0 snorris    (501) staff       (20)      351 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/__init__.py
--rw-r--r--   0 snorris    (501) staff       (20)     6196 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.8.0a1/bcdata/bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     9774 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/cli.py
--rw-r--r--   0 snorris    (501) staff       (20)     6337 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/database.py
--rw-r--r--   0 snorris    (501) staff       (20)     3654 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/wcs.py
--rw-r--r--   0 snorris    (501) staff       (20)    11261 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/bcdata/wfs.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.739309 bcdata-0.8.0a1/bcdata.egg-info/
--rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)      474 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/SOURCES.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/dependency_links.txt
--rw-r--r--   0 snorris    (501) staff       (20)       42 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/entry_points.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.8.0a1/bcdata.egg-info/not-zip-safe
--rw-r--r--   0 snorris    (501) staff       (20)      134 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/requires.txt
--rw-r--r--   0 snorris    (501) staff       (20)        7 2023-06-29 21:34:51.000000 bcdata-0.8.0a1/bcdata.egg-info/top_level.txt
--rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.8.0a1/pyproject.toml
--rw-r--r--   0 snorris    (501) staff       (20)      115 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/requirements.txt
--rw-r--r--   0 snorris    (501) staff       (20)       38 2023-06-29 21:34:51.740211 bcdata-0.8.0a1/setup.cfg
--rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.8.0a1/setup.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-29 21:34:51.739818 bcdata-0.8.0a1/tests/
--rw-r--r--   0 snorris    (501) staff       (20)     5033 2023-06-28 23:17:04.000000 bcdata-0.8.0a1/tests/test_bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     6088 2023-06-29 21:33:29.000000 bcdata-0.8.0a1/tests/test_bcdata.py
--rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.8.0a1/tests/test_bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.8.0a1/tests/test_cli.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.847999 bcdata-0.8.0a2/
+-rw-r--r--   0 snorris    (501) staff       (20)     7313 2023-07-03 22:32:31.000000 bcdata-0.8.0a2/CHANGES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.8.0a2/LICENSE.txt
+-rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-03 22:37:14.847743 bcdata-0.8.0a2/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)    15657 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/README.md
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.846099 bcdata-0.8.0a2/bcdata/
+-rw-r--r--   0 snorris    (501) staff       (20)      351 2023-07-03 21:55:43.000000 bcdata-0.8.0a2/bcdata/__init__.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6196 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     4936 2023-07-03 22:27:54.000000 bcdata-0.8.0a2/bcdata/bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     9940 2023-06-29 22:02:05.000000 bcdata-0.8.0a2/bcdata/cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6337 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/database.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3654 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11261 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/bcdata/wfs.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.846991 bcdata-0.8.0a2/bcdata.egg-info/
+-rw-r--r--   0 snorris    (501) staff       (20)    16479 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)      474 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       42 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/entry_points.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.8.0a2/bcdata.egg-info/not-zip-safe
+-rw-r--r--   0 snorris    (501) staff       (20)      134 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/requires.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        7 2023-07-03 22:37:14.000000 bcdata-0.8.0a2/bcdata.egg-info/top_level.txt
+-rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.8.0a2/pyproject.toml
+-rw-r--r--   0 snorris    (501) staff       (20)      115 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/requirements.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       38 2023-07-03 22:37:14.848051 bcdata-0.8.0a2/setup.cfg
+-rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.8.0a2/setup.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-07-03 22:37:14.847435 bcdata-0.8.0a2/tests/
+-rw-r--r--   0 snorris    (501) staff       (20)     5033 2023-06-28 23:17:04.000000 bcdata-0.8.0a2/tests/test_bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6088 2023-06-29 21:33:29.000000 bcdata-0.8.0a2/tests/test_bcdata.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11744 2023-07-03 22:28:46.000000 bcdata-0.8.0a2/tests/test_bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.8.0a2/tests/test_cli.py
```

### Comparing `bcdata-0.8.0a1/CHANGES.txt` & `bcdata-0.8.0a2/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Changes
 =======
 
+0.8.0a2 (2023-07-03)
+------------------
+- handle tables with schema stored in bcdc resource with format='multiple' (#135)
+
 0.8.0a1 (2023-06-29)
 ------------------
 - cache WFS GetCapabilities response for faster requests and fewer http errors
 - retry bc2pg requests on failure
 - move bc2pg download logging to bcdata.log
 - fix dem command default output CRS (#125)
 - upgrade to sqlalchemy v2 (#124)
+- single threaded downloads only (--max_workers option removed)
 
 0.7.12 (2023-06-28)
 ------------------
 - fix bc2pg cli error
 
 0.7.11 (2023-06-28)
 ------------------
```

### Comparing `bcdata-0.8.0a1/LICENSE.txt` & `bcdata-0.8.0a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/PKG-INFO` & `bcdata-0.8.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.8.0a1
+Version: 0.8.0a2
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bcdata-0.8.0a1/README.md` & `bcdata-0.8.0a2/README.md`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/bcdata/bc2pg.py` & `bcdata-0.8.0a2/bcdata/bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/bcdata/bcdc.py` & `bcdata-0.8.0a2/bcdata/bcdc.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,32 +60,48 @@
         return []
     else:
         matches = []
         # iterate through results of search (packages)
         for result in r.json()["result"]["results"]:
             # iterate through resources associated with each package
             for resource in result["resources"]:
+                log.debug(resource)
                 # if resource is wms and url matches provided table name,
                 # extract the metadata
                 if resource["format"] == "wms":
                     if urlparse(resource["url"]).path.split("/")[3] == table_name:
                         if "object_table_comments" in resource.keys():
                             table_comments = resource["object_table_comments"]
                         else:
                             log.info(f"No table comments found for {table_name}")
                             table_comments = None
+                        if "details" in resource.keys() and resource["details"] != "":
+                            table_details = resource["details"]
+                        else:
+                            log.info(f"No details found for {table_name}")
+                            table_details = None
+                        if table_details and table_comments:
+                            matches.append((table_comments, table_details))
+                # some datasets are documented in the resource with format="multiple", not format="wms"
+                # (for example, WHSE_FOREST_VEGETATION.OGSR_PRIORITY_DEF_AREA_CUR_SP)
+                elif resource["format"] == "multiple":
+                    if json.loads(resource["preview_info"])["layer_name"] == table_name:
+                        if "object_table_comments" in resource.keys():
+                            table_comments = resource["object_table_comments"]
+                        else:
+                            log.info(f"No table comments found for {table_name}")
+                            table_comments = None
                         if "details" in resource.keys():
                             table_details = resource["details"]
                         else:
                             log.info(f"No details found for {table_name}")
                             table_details = None
-                        matches.append((table_comments, table_details))
+                        if table_details and table_comments:
+                            matches.append((table_comments, table_details))
         # uniquify the result
-        # (presuming there is only one unique result, but this seems safe as we are
-        # matching on the oracle table name)
         if len(matches) > 0:
             matched = list(set(matches))[0]
             return (matched[0], json.loads(matched[1]))
         else:
             log.warning(
                 f"BCDC search for {table_name} does not return expected details"
             )
```

### Comparing `bcdata-0.8.0a1/bcdata/cli.py` & `bcdata-0.8.0a2/bcdata/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 
 def configure_logging(verbosity):
     log_level = max(10, 30 - 10 * verbosity)
     logging.basicConfig(stream=sys.stderr, level=log_level)
 
 
+def complete_dataset_names(ctx, param, incomplete):
+    return [k for k in bcdata.list_tables() if k.startswith(incomplete)]
+
+
 # bounds handling direct from rasterio
 # https://github.com/mapbox/rasterio/blob/master/rasterio/rio/options.py
 # https://github.com/mapbox/rasterio/blob/master/rasterio/rio/clip.py
 
 
 def from_like_context(ctx, param, value):
     """Return the value for an option from the context if the option
@@ -283,15 +287,15 @@
         pagesize=pagesize,
         lowercase=lowercase,
     ):
         click.echo(json.dumps(feat, **dump_kwds))
 
 
 @cli.command()
-@click.argument("dataset", type=click.STRING)
+@click.argument("dataset", type=click.STRING, shell_complete=complete_dataset_names)
 @click.option(
     "--db_url",
     "-db",
     help="Target database url, defaults to $DATABASE_URL environment variable if set",
     default=os.environ.get("DATABASE_URL"),
 )
 @click.option("--table", help="Destination table name")
```

### Comparing `bcdata-0.8.0a1/bcdata/database.py` & `bcdata-0.8.0a2/bcdata/database.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/bcdata/wcs.py` & `bcdata-0.8.0a2/bcdata/wcs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/bcdata/wfs.py` & `bcdata-0.8.0a2/bcdata/wfs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/bcdata.egg-info/PKG-INFO` & `bcdata-0.8.0a2/bcdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.8.0a1
+Version: 0.8.0a2
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bcdata-0.8.0a1/setup.py` & `bcdata-0.8.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/tests/test_bc2pg.py` & `bcdata-0.8.0a2/tests/test_bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/tests/test_bcdata.py` & `bcdata-0.8.0a2/tests/test_bcdata.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.8.0a1/tests/test_bcdc.py` & `bcdata-0.8.0a2/tests/test_bcdc.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,7 +18,15 @@
     assert table == AIRPORTS_TABLE
 
 
 def test_get_table_definition():
     table = bcdc.get_table_definition(AIRPORTS_TABLE)
     assert table[0] == AIRPORTS_COMMENTS
     assert table[1] == json.loads(AIRPORTS_SCHEMA)
+
+
+def test_get_table_definition_format_multi():
+    table = bcdc.get_table_definition(
+        "WHSE_FOREST_VEGETATION.OGSR_PRIORITY_DEF_AREA_CUR_SP"
+    )
+    assert table[0]
+    assert table[1]
```

### Comparing `bcdata-0.8.0a1/tests/test_cli.py` & `bcdata-0.8.0a2/tests/test_cli.py`

 * *Files identical despite different names*

