# Comparing `tmp/apidownload-2.1.0-py3-none-any.whl.zip` & `tmp/apidownload-2.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4978 bytes, number of entries: 10
+Zip file size: 4990 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat     3049 b- defN 23-Jun-20 19:59 apidownload/__init__.py
 -rw-rw-rw-  2.0 fat      446 b- defN 23-Jun-20 20:10 apidownload/__main__.py
 -rw-rw-rw-  2.0 fat      190 b- defN 23-May-16 19:19 apidownload/apidownload.json
 -rw-rw-rw-  2.0 fat      190 b- defN 23-May-16 19:19 apidownload/default_settings.json
--rw-rw-rw-  2.0 fat     1714 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1317 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      841 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/RECORD
-10 files, 7909 bytes uncompressed, 3528 bytes compressed:  55.4%
+-rw-rw-rw-  2.0 fat     1714 b- defN 23-Jul-04 10:12 apidownload-2.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1328 b- defN 23-Jul-04 10:12 apidownload-2.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 10:12 apidownload-2.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       58 b- defN 23-Jul-04 10:12 apidownload-2.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-04 10:12 apidownload-2.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      841 b- defN 23-Jul-04 10:12 apidownload-2.1.1.dist-info/RECORD
+10 files, 7920 bytes uncompressed, 3540 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: apidownload/apidownload.json
 Comment: 
 
 Filename: apidownload/default_settings.json
 Comment: 
 
-Filename: apidownload-2.1.0.dist-info/LICENSE.txt
+Filename: apidownload-2.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: apidownload-2.1.0.dist-info/METADATA
+Filename: apidownload-2.1.1.dist-info/METADATA
 Comment: 
 
-Filename: apidownload-2.1.0.dist-info/WHEEL
+Filename: apidownload-2.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: apidownload-2.1.0.dist-info/entry_points.txt
+Filename: apidownload-2.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: apidownload-2.1.0.dist-info/top_level.txt
+Filename: apidownload-2.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: apidownload-2.1.0.dist-info/RECORD
+Filename: apidownload-2.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `apidownload-2.1.0.dist-info/LICENSE.txt` & `apidownload-2.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `apidownload-2.1.0.dist-info/METADATA` & `apidownload-2.1.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: apidownload
-Version: 2.1.0
+Version: 2.1.1
 Summary: Download the data from an API endpoint to a file
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/API-Download
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: requests
+Requires-Dist: requests (==2.31.0)
 
 # API Download
 Download the data from an API endpoint to a file
 
 ## Install
 ```cmd
 pip install apidownload
```

## Comparing `apidownload-2.1.0.dist-info/RECORD` & `apidownload-2.1.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 apidownload/__init__.py,sha256=h7qfG0IKM0u-sppkF0e4t-hVjLyp0PvuICgsM84dQmA,3049
 apidownload/__main__.py,sha256=VLr7XjSGM2igYiTqk1yfBxxsOtqiSfWYDr1KJPtcyo4,446
 apidownload/apidownload.json,sha256=B_ORJnUk7167OJoj99o0sDN9a-jj8dId--B1Jk3nvI4,190
 apidownload/default_settings.json,sha256=B_ORJnUk7167OJoj99o0sDN9a-jj8dId--B1Jk3nvI4,190
-apidownload-2.1.0.dist-info/LICENSE.txt,sha256=42KznO94fKWkiywx3MOxyp7ByNDs0OC_Q6LBuyrMhUM,1714
-apidownload-2.1.0.dist-info/METADATA,sha256=Ebs1D94OySWZQfE0oQcEm2l6bQa2410Kx0srUik8Z6g,1317
-apidownload-2.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-apidownload-2.1.0.dist-info/entry_points.txt,sha256=-8MaE44oJC4dsLcy97Ko5PxozatgzhSVhIc3SeGm8lE,58
-apidownload-2.1.0.dist-info/top_level.txt,sha256=EGbn7Bj7I8a2J2SWr8PFU658bi_4YCzE3N2KRzrTd3E,12
-apidownload-2.1.0.dist-info/RECORD,,
+apidownload-2.1.1.dist-info/LICENSE.txt,sha256=42KznO94fKWkiywx3MOxyp7ByNDs0OC_Q6LBuyrMhUM,1714
+apidownload-2.1.1.dist-info/METADATA,sha256=2X56Cbqvx0RoX0MWf4jwX2k6ZYm2izu1Fe0st2rIgVY,1328
+apidownload-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+apidownload-2.1.1.dist-info/entry_points.txt,sha256=-8MaE44oJC4dsLcy97Ko5PxozatgzhSVhIc3SeGm8lE,58
+apidownload-2.1.1.dist-info/top_level.txt,sha256=EGbn7Bj7I8a2J2SWr8PFU658bi_4YCzE3N2KRzrTd3E,12
+apidownload-2.1.1.dist-info/RECORD,,
```

