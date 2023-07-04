# Comparing `tmp/SELDOMpy-0.7.3-cp38-cp38-win_amd64.whl.zip` & `tmp/SELDOMpy-0.7.4-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 297743 bytes, number of entries: 73
+Zip file size: 297746 bytes, number of entries: 73
 -rw-rw-rw-  2.0 fat   265216 b- defN 23-Jul-03 17:15 hello.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 17:23 sim_logic_ode.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      390 b- defN 23-Jul-04 08:20 SELDOMpy/__init__.py
 -rw-rw-rw-  2.0 fat     2309 b- defN 23-Jun-22 08:44 SELDOMpy/buildmim.py
 -rw-rw-rw-  2.0 fat     1288 b- defN 23-Jul-04 08:20 SELDOMpy/extras.py
 -rw-rw-rw-  2.0 fat     4159 b- defN 23-Apr-19 14:22 SELDOMpy/gen_exps.py
 -rw-rw-rw-  2.0 fat     4838 b- defN 23-Jun-28 11:33 SELDOMpy/getLBODEmodel.py
@@ -63,13 +63,13 @@
 -rw-rw-rw-  2.0 fat     6225 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_direct.c
 -rw-rw-rw-  2.0 fat     7662 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_iterative.c
 -rw-rw-rw-  2.0 fat     2474 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_math.c
 -rw-rw-rw-  2.0 fat     4702 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_nvector.c
 -rw-rw-rw-  2.0 fat     9663 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_spbcgs.c
 -rw-rw-rw-  2.0 fat    12650 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_spgmr.c
 -rw-rw-rw-  2.0 fat    14744 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_sptfqmr.c
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-04 08:21 SELDOMpy-0.7.3.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      800 b- defN 23-Jul-04 08:21 SELDOMpy-0.7.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-04 08:21 SELDOMpy-0.7.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-04 08:21 SELDOMpy-0.7.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6141 b- defN 23-Jul-04 08:21 SELDOMpy-0.7.3.dist-info/RECORD
-73 files, 1045204 bytes uncompressed, 288085 bytes compressed:  72.4%
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-04 08:25 SELDOMpy-0.7.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      851 b- defN 23-Jul-04 08:25 SELDOMpy-0.7.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-04 08:25 SELDOMpy-0.7.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-04 08:25 SELDOMpy-0.7.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6141 b- defN 23-Jul-04 08:25 SELDOMpy-0.7.4.dist-info/RECORD
+73 files, 1045255 bytes uncompressed, 288088 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -198,23 +198,23 @@
 
 Filename: SELDOMpy/src/sundials_spgmr.c
 Comment: 
 
 Filename: SELDOMpy/src/sundials_sptfqmr.c
 Comment: 
 
-Filename: SELDOMpy-0.7.3.dist-info/LICENSE.txt
+Filename: SELDOMpy-0.7.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: SELDOMpy-0.7.3.dist-info/METADATA
+Filename: SELDOMpy-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: SELDOMpy-0.7.3.dist-info/WHEEL
+Filename: SELDOMpy-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: SELDOMpy-0.7.3.dist-info/top_level.txt
+Filename: SELDOMpy-0.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: SELDOMpy-0.7.3.dist-info/RECORD
+Filename: SELDOMpy-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `SELDOMpy-0.7.3.dist-info/LICENSE.txt` & `SELDOMpy-0.7.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `SELDOMpy-0.7.3.dist-info/METADATA` & `SELDOMpy-0.7.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.7.3
+Version: 0.7.4
 Summary: hardware acceleration
 Home-page: https://github.com/voxy/accel.git
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: mealpy
 Requires-Dist: matplotlib
```

## Comparing `SELDOMpy-0.7.3.dist-info/RECORD` & `SELDOMpy-0.7.4.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -62,12 +62,12 @@
 SELDOMpy/src/sundials_direct.c,sha256=3fTxm9kVfmfj7kbIbOpEPpd0AWQaCydha5uhUoc6WEA,6225
 SELDOMpy/src/sundials_iterative.c,sha256=Okb4iAhwTcj3tsKgJVWPxq2KlbRTQMAdZAwrSL9Bx28,7662
 SELDOMpy/src/sundials_math.c,sha256=18wLmG9SCGyQr1TzcIxuSQQWddHz4M5mYy5RI4TKtlc,2474
 SELDOMpy/src/sundials_nvector.c,sha256=7N9Pol7nbeWut0OHfM8F70iboGcI-BuEA7JIHhJAiBs,4702
 SELDOMpy/src/sundials_spbcgs.c,sha256=Bs3K_hAB5no6aKv5Tppwu8OGOPCpw6bFiAU_E0ePcnY,9663
 SELDOMpy/src/sundials_spgmr.c,sha256=KKRd_fpxv2V3DT0MOZxWZpO3KbXfseSJyV8bOnYeArk,12650
 SELDOMpy/src/sundials_sptfqmr.c,sha256=_d97GsT0yi9Zuh_SO7ZwQHT_Sb3JK-UOy5j9H3HXmTw,14744
-SELDOMpy-0.7.3.dist-info/LICENSE.txt,sha256=Z_R0qA8dBa_UBMGgM1fEedm0wV7CBqwIBaBEOu4iT5w,1077
-SELDOMpy-0.7.3.dist-info/METADATA,sha256=Iqh6bao4qzafECmVAqp8f7bIJ2CVS1_BuQdC-M15ewk,800
-SELDOMpy-0.7.3.dist-info/WHEEL,sha256=F2aDWtWrilNM3-px1vBtJOEd7aRVTetQfFuDYmYbAUQ,100
-SELDOMpy-0.7.3.dist-info/top_level.txt,sha256=Ob79bfCTj_ucLsKNzB5Bea8oIrbiwekeNGRp4zxCiMg,15
-SELDOMpy-0.7.3.dist-info/RECORD,,
+SELDOMpy-0.7.4.dist-info/LICENSE.txt,sha256=Z_R0qA8dBa_UBMGgM1fEedm0wV7CBqwIBaBEOu4iT5w,1077
+SELDOMpy-0.7.4.dist-info/METADATA,sha256=z8YtDxj11gg5HpFUvVTK3D0pMGzRgz79d6VDxNNqki4,851
+SELDOMpy-0.7.4.dist-info/WHEEL,sha256=F2aDWtWrilNM3-px1vBtJOEd7aRVTetQfFuDYmYbAUQ,100
+SELDOMpy-0.7.4.dist-info/top_level.txt,sha256=Ob79bfCTj_ucLsKNzB5Bea8oIrbiwekeNGRp4zxCiMg,15
+SELDOMpy-0.7.4.dist-info/RECORD,,
```

