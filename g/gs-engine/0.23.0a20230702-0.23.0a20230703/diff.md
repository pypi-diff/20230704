# Comparing `tmp/gs_engine-0.23.0a20230702-py2.py3-none-any.whl.zip` & `tmp/gs_engine-0.23.0a20230703-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11896 bytes, number of entries: 9
--rw-r--r--  2.0 unx      398 b- defN 23-Jul-02 19:01 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      503 b- defN 23-Jul-02 19:01 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx     1573 b- defN 23-Jul-02 19:01 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-02 19:01 graphscope.runtime/conf/log4rs.yml
--rw-r--r--  2.0 unx      694 b- defN 23-Jul-02 19:01 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx    21680 b- defN 23-Jul-02 20:46 gs_engine-0.23.0a20230702.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-02 20:46 gs_engine-0.23.0a20230702.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 20:46 gs_engine-0.23.0a20230702.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 23-Jul-02 20:46 gs_engine-0.23.0a20230702.dist-info/RECORD
-9 files, 26012 bytes uncompressed, 10434 bytes compressed:  59.9%
+Zip file size: 11897 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-03 19:02 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      503 b- defN 23-Jul-03 19:02 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jul-03 19:02 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-03 19:02 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-03 19:02 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    21680 b- defN 23-Jul-03 20:36 gs_engine-0.23.0a20230703.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-03 20:36 gs_engine-0.23.0a20230703.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-03 20:36 gs_engine-0.23.0a20230703.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jul-03 20:36 gs_engine-0.23.0a20230703.dist-info/RECORD
+9 files, 26012 bytes uncompressed, 10435 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.23.0a20230702.dist-info/METADATA
+Filename: gs_engine-0.23.0a20230703.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.23.0a20230702.dist-info/WHEEL
+Filename: gs_engine-0.23.0a20230703.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.23.0a20230702.dist-info/top_level.txt
+Filename: gs_engine-0.23.0a20230703.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.23.0a20230702.dist-info/RECORD
+Filename: gs_engine-0.23.0a20230703.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.23.0a20230702.dist-info/METADATA` & `gs_engine-0.23.0a20230703.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.23.0a20230702
+Version: 0.23.0a20230703
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `gs_engine-0.23.0a20230702.dist-info/RECORD` & `gs_engine-0.23.0a20230703.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
 graphscope.runtime/conf/frontend.vineyard.properties,sha256=tMvPMA7q5bw--brMxun_Q24R35j52bs80MhqqFszA-s,503
 graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
 graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
 graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_engine-0.23.0a20230702.dist-info/METADATA,sha256=ruVr0imRUw0owawgOBGI3QsK0-W5PYlpELbufqFTuEY,21680
-gs_engine-0.23.0a20230702.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-gs_engine-0.23.0a20230702.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.23.0a20230702.dist-info/RECORD,,
+gs_engine-0.23.0a20230703.dist-info/METADATA,sha256=CvKkf5UMxX-F5Lx35U7JBbtSCpTAqHfONyOUe4FrwdM,21680
+gs_engine-0.23.0a20230703.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+gs_engine-0.23.0a20230703.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.23.0a20230703.dist-info/RECORD,,
```

