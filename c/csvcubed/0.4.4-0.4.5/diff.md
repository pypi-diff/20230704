# Comparing `tmp/csvcubed-0.4.4-py3-none-any.whl.zip` & `tmp/csvcubed-0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 232523 bytes, number of entries: 195
+Zip file size: 232522 bytes, number of entries: 195
 -rw-r--r--  2.0 unx     1515 b- defN 80-Jan-01 00:00 csvcubed/README.md
 -rw-r--r--  2.0 unx      218 b- defN 80-Jan-01 00:00 csvcubed/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/__init__.py
 -rw-r--r--  2.0 unx     2881 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/build.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/__init__.py
 -rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/build_code_list.py
@@ -185,13 +185,13 @@
 -rw-r--r--  2.0 unx    27378 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/qbwriter/urihelper.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/__init__.py
 -rw-r--r--  2.0 unx      157 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/constants.py
 -rw-r--r--  2.0 unx     2437 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py
 -rw-r--r--  2.0 unx    20804 b- defN 80-Jan-01 00:00 csvcubed/writers/qbwriter.py
 -rw-r--r--  2.0 unx     9528 b- defN 80-Jan-01 00:00 csvcubed/writers/skoscodelistwriter.py
 -rw-r--r--  2.0 unx      283 b- defN 80-Jan-01 00:00 csvcubed/writers/writerbase.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3970 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.4.4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    19635 b- defN 16-Jan-01 00:00 csvcubed-0.4.4.dist-info/RECORD
-195 files, 861439 bytes uncompressed, 200315 bytes compressed:  76.7%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.4.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3961 b- defN 80-Jan-01 00:00 csvcubed-0.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.4.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    19635 b- defN 16-Jan-01 00:00 csvcubed-0.4.5.dist-info/RECORD
+195 files, 861430 bytes uncompressed, 200314 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -564,23 +564,23 @@
 
 Filename: csvcubed/writers/skoscodelistwriter.py
 Comment: 
 
 Filename: csvcubed/writers/writerbase.py
 Comment: 
 
-Filename: csvcubed-0.4.4.dist-info/LICENSE
+Filename: csvcubed-0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: csvcubed-0.4.4.dist-info/METADATA
+Filename: csvcubed-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: csvcubed-0.4.4.dist-info/WHEEL
+Filename: csvcubed-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: csvcubed-0.4.4.dist-info/entry_points.txt
+Filename: csvcubed-0.4.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: csvcubed-0.4.4.dist-info/RECORD
+Filename: csvcubed-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `csvcubed-0.4.4.dist-info/LICENSE` & `csvcubed-0.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `csvcubed-0.4.4.dist-info/METADATA` & `csvcubed-0.4.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: csvcubed
-Version: 0.4.4
+Version: 0.4.5
 Summary: A tool to generate RDF Data Cube style CSV-W cubes from tidy CSV files. Part of the csvcubed family.
 License: Apache-2.0
 Author: Integrated Data Service - Dissemination
 Author-email: csvcubed@gsscogs.uk
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: csvcubed-models (==0.1.6)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
-Requires-Dist: pandas (>=1.3.3,<2.0.0)
+Requires-Dist: pandas (>=1.3)
 Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-cache (>=0.9.3,<0.10.0)
 Requires-Dist: treelib (>=1.6.1,<2.0.0)
 Requires-Dist: uritemplate (>=4.1.1,<5.0.0)
 Requires-Dist: urllib3 (>=1.0.0,<2.0.0)
```

## Comparing `csvcubed-0.4.4.dist-info/RECORD` & `csvcubed-0.4.5.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -184,12 +184,12 @@
 csvcubed/writers/helpers/qbwriter/urihelper.py,sha256=BzVnUueyoE1DBncTByKnigeLozePdfFRfxzaguwCtxY,27378
 csvcubed/writers/helpers/skoscodelistwriter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/writers/helpers/skoscodelistwriter/constants.py,sha256=FjVa2JsAc7uIxzQOJgNg3zf8Ha-YZvMzF75sqq_e93g,157
 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py,sha256=DWkL2zO4QsLV8Oo-nVXxS4cxA1ic4stSBp7NZpClbps,2437
 csvcubed/writers/qbwriter.py,sha256=fDesUmhWU1211z_wDQi8xFdfpB0CqdSHG7pM-YlsJQc,20804
 csvcubed/writers/skoscodelistwriter.py,sha256=-ROyhtzqbZjss4XjQkzhQvdjG51oIlkDgOclA3e28uU,9528
 csvcubed/writers/writerbase.py,sha256=lzEHMgqdWBIFbxthYjf5JuE3i5gp5Vbb1Xw359TY3to,283
-csvcubed-0.4.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-csvcubed-0.4.4.dist-info/METADATA,sha256=sVZSsopkHs7Vq6NNT9UyP0LwCPubjnhaoaKp21YNVAY,3970
-csvcubed-0.4.4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-csvcubed-0.4.4.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
-csvcubed-0.4.4.dist-info/RECORD,,
+csvcubed-0.4.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+csvcubed-0.4.5.dist-info/METADATA,sha256=YjLctVCxvrDlxb_7mlVtJ2EmohdYEhtc72nDpF1Wp8Q,3961
+csvcubed-0.4.5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+csvcubed-0.4.5.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
+csvcubed-0.4.5.dist-info/RECORD,,
```

