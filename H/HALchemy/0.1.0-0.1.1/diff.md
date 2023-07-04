# Comparing `tmp/HALchemy-0.1.0-py3-none-any.whl.zip` & `tmp/HALchemy-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1563 bytes, number of entries: 5
+Zip file size: 1523 bytes, number of entries: 5
 -rw-rw-rw-  2.0 fat       91 b- defN 23-Jul-04 00:36 halchemy/placeholder.py
--rw-rw-rw-  2.0 fat      785 b- defN 23-Jul-04 00:38 HALchemy-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 00:38 HALchemy-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 00:38 HALchemy-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 23-Jul-04 00:38 HALchemy-0.1.0.dist-info/RECORD
-5 files, 1355 bytes uncompressed, 851 bytes compressed:  37.2%
+-rw-rw-rw-  2.0 fat      679 b- defN 23-Jul-04 00:41 HALchemy-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 00:41 HALchemy-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-04 00:41 HALchemy-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 23-Jul-04 00:41 HALchemy-0.1.1.dist-info/RECORD
+5 files, 1249 bytes uncompressed, 811 bytes compressed:  35.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: halchemy/placeholder.py
 Comment: 
 
-Filename: HALchemy-0.1.0.dist-info/METADATA
+Filename: HALchemy-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: HALchemy-0.1.0.dist-info/WHEEL
+Filename: HALchemy-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: HALchemy-0.1.0.dist-info/top_level.txt
+Filename: HALchemy-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: HALchemy-0.1.0.dist-info/RECORD
+Filename: HALchemy-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `HALchemy-0.1.0.dist-info/METADATA` & `HALchemy-0.1.1.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: HALchemy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolkit for creating clients of HAL based Hypermedia APIs.
 Home-page: https://github.com/pointw-dev/HALchemy
 Author: Michael Ottoson
 Author-email: michael@pointw.com
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # HALchemy
 Toolkit for creating clients of Hypermedia APIs using HAL
```

