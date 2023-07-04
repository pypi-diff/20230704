# Comparing `tmp/gremlin_python_tutorial-0.0.5.tar.gz` & `tmp/gremlin_python_tutorial-0.0.6.tar.gz`

## Comparing `gremlin_python_tutorial-0.0.5.tar` & `gremlin_python_tutorial-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.project
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.pydevproject
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.travis.yml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/setServer.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.github/workflows/build.yaml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/DataStax.yaml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/Neo4j.yaml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/OrientDB.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/TinkerGraph.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/config/server.yaml
--rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/data/air-routes-small.xml
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/data/tinkerpop-modern.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/__init__.py
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/draw.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/examples.py
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/gremlin/remote.py
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/install
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/installAndTest
--rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/run
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/runDataStax
--rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/runNeo4j
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/runOrientDB
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/base_gremlin_test.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/basetest.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/jupyter.ipynb
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_003_connection.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_004_io.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_005_graphviz.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_draw.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_examples.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_modern.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_server.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/tests/test_tutorial.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/LICENSE
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/README.md
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/.project
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/.pydevproject
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/.travis.yml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/setServer.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/config/DataStax.yaml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/config/Neo4j.yaml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/config/OrientDB.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/config/TinkerGraph.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/config/server.yaml
+-rw-r--r--   0        0        0   192201 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/data/air-routes-small.xml
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/data/tinkerpop-modern.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/gremlin/__init__.py
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/gremlin/draw.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/gremlin/examples.py
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/gremlin/remote.py
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/scripts/install
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/scripts/installAndTest
+-rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/scripts/run
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/scripts/runDataStax
+-rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/scripts/runNeo4j
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/scripts/runOrientDB
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/base_gremlin_test.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/basetest.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/jupyter.ipynb
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_003_connection.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_004_io.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_005_graphviz.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_draw.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_examples.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_modern.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_server.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/tests/test_tutorial.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/README.md
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 gremlin_python_tutorial-0.0.6/PKG-INFO
```

### Comparing `gremlin_python_tutorial-0.0.5/.project` & `gremlin_python_tutorial-0.0.6/.project`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/.travis.yml` & `gremlin_python_tutorial-0.0.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/setServer.py` & `gremlin_python_tutorial-0.0.6/setServer.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/.github/workflows/build.yaml` & `gremlin_python_tutorial-0.0.6/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/.github/workflows/upload-to-pypi.yml` & `gremlin_python_tutorial-0.0.6/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/data/air-routes-small.xml` & `gremlin_python_tutorial-0.0.6/data/air-routes-small.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/data/tinkerpop-modern.xml` & `gremlin_python_tutorial-0.0.6/data/tinkerpop-modern.xml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/gremlin/draw.py` & `gremlin_python_tutorial-0.0.6/gremlin/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         
         # get the image of the edge by id
         in_vertex_id = edge.inV.id
         out_vertex_id = edge.outV.id
 
         # draw the edge
         digraph.edge(
-            tail_name = str(in_vertex_id),
-            head_name = str(out_vertex_id),
+            tail_name = str(out_vertex_id),
+            head_name = str(in_vertex_id),
             label = f"{str(edge.id)}\n{edge.label}\n{'─' * 5}\n{properties_label}",
             style = "setlinewidth(3)",
             fontname = "arial"
         )
 
         return digraph
```

### Comparing `gremlin_python_tutorial-0.0.5/gremlin/examples.py` & `gremlin_python_tutorial-0.0.6/gremlin/examples.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/gremlin/remote.py` & `gremlin_python_tutorial-0.0.6/gremlin/remote.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/scripts/installAndTest` & `gremlin_python_tutorial-0.0.6/scripts/installAndTest`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/scripts/run` & `gremlin_python_tutorial-0.0.6/scripts/run`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/scripts/runNeo4j` & `gremlin_python_tutorial-0.0.6/scripts/runNeo4j`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/base_gremlin_test.py` & `gremlin_python_tutorial-0.0.6/tests/base_gremlin_test.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/basetest.py` & `gremlin_python_tutorial-0.0.6/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/jupyter.ipynb` & `gremlin_python_tutorial-0.0.6/tests/jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/test_003_connection.py` & `gremlin_python_tutorial-0.0.6/tests/test_003_connection.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/test_004_io.py` & `gremlin_python_tutorial-0.0.6/tests/test_004_io.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/test_005_graphviz.py` & `gremlin_python_tutorial-0.0.6/tests/test_005_graphviz.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/test_draw.py` & `gremlin_python_tutorial-0.0.6/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/test_examples.py` & `gremlin_python_tutorial-0.0.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/test_modern.py` & `gremlin_python_tutorial-0.0.6/tests/test_modern.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/tests/test_tutorial.py` & `gremlin_python_tutorial-0.0.6/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/.gitignore` & `gremlin_python_tutorial-0.0.6/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -111,7 +111,10 @@
 apache-tinkerpop-gremlin-*
 
 # nohup.out files
 nohup.out
 
 # eclipse settings directory
 .settings
+
+# VSCode files
+.vscode/
```

### Comparing `gremlin_python_tutorial-0.0.5/LICENSE` & `gremlin_python_tutorial-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/README.md` & `gremlin_python_tutorial-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/pyproject.toml` & `gremlin_python_tutorial-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gremlin_python_tutorial-0.0.5/PKG-INFO` & `gremlin_python_tutorial-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlin-python-tutorial
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Home, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Gremlin_python
 Project-URL: Source, https://github.com/WolfgangFahl/gremlin-python-tutorial
 Author-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>, Julian Vollmer <julian.vollmer@rwth-aachen.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
```

