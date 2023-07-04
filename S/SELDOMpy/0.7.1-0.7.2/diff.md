# Comparing `tmp/SELDOMpy-0.7.1-cp38-cp38-win_amd64.whl.zip` & `tmp/SELDOMpy-0.7.2-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 297725 bytes, number of entries: 73
+Zip file size: 297744 bytes, number of entries: 73
 -rw-rw-rw-  2.0 fat   265216 b- defN 23-Jul-03 17:15 hello.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 17:23 sim_logic_ode.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat      390 b- defN 23-Jul-03 07:13 SELDOMpy/__init__.py
+-rw-rw-rw-  2.0 fat      405 b- defN 23-Jul-04 07:44 SELDOMpy/__init__.py
 -rw-rw-rw-  2.0 fat     2309 b- defN 23-Jun-22 08:44 SELDOMpy/buildmim.py
 -rw-rw-rw-  2.0 fat     1271 b- defN 23-Apr-14 17:44 SELDOMpy/extras.py
 -rw-rw-rw-  2.0 fat     4159 b- defN 23-Apr-19 14:22 SELDOMpy/gen_exps.py
 -rw-rw-rw-  2.0 fat     4838 b- defN 23-Jun-28 11:33 SELDOMpy/getLBODEmodel.py
 -rw-rw-rw-  2.0 fat     3232 b- defN 23-Apr-24 18:45 SELDOMpy/getRandomLBODEmodel.py
 -rw-rw-rw-  2.0 fat     2460 b- defN 23-Jun-28 11:33 SELDOMpy/opt_mealpy.py
 -rw-rw-rw-  2.0 fat     2460 b- defN 23-Jun-28 11:33 SELDOMpy/optimization.py
@@ -63,13 +63,13 @@
 -rw-rw-rw-  2.0 fat     6225 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_direct.c
 -rw-rw-rw-  2.0 fat     7662 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_iterative.c
 -rw-rw-rw-  2.0 fat     2474 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_math.c
 -rw-rw-rw-  2.0 fat     4702 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_nvector.c
 -rw-rw-rw-  2.0 fat     9663 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_spbcgs.c
 -rw-rw-rw-  2.0 fat    12650 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_spgmr.c
 -rw-rw-rw-  2.0 fat    14744 b- defN 22-Dec-07 11:24 SELDOMpy/src/sundials_sptfqmr.c
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-04 07:31 SELDOMpy-0.7.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      777 b- defN 23-Jul-04 07:31 SELDOMpy-0.7.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-04 07:31 SELDOMpy-0.7.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-04 07:31 SELDOMpy-0.7.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6141 b- defN 23-Jul-04 07:31 SELDOMpy-0.7.1.dist-info/RECORD
-73 files, 1045164 bytes uncompressed, 288067 bytes compressed:  72.4%
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-Jul-04 08:11 SELDOMpy-0.7.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      800 b- defN 23-Jul-04 08:11 SELDOMpy-0.7.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-04 08:11 SELDOMpy-0.7.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-04 08:11 SELDOMpy-0.7.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6141 b- defN 23-Jul-04 08:11 SELDOMpy-0.7.2.dist-info/RECORD
+73 files, 1045202 bytes uncompressed, 288086 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -198,23 +198,23 @@
 
 Filename: SELDOMpy/src/sundials_spgmr.c
 Comment: 
 
 Filename: SELDOMpy/src/sundials_sptfqmr.c
 Comment: 
 
-Filename: SELDOMpy-0.7.1.dist-info/LICENSE.txt
+Filename: SELDOMpy-0.7.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: SELDOMpy-0.7.1.dist-info/METADATA
+Filename: SELDOMpy-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: SELDOMpy-0.7.1.dist-info/WHEEL
+Filename: SELDOMpy-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: SELDOMpy-0.7.1.dist-info/top_level.txt
+Filename: SELDOMpy-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: SELDOMpy-0.7.1.dist-info/RECORD
+Filename: SELDOMpy-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SELDOMpy/__init__.py

```diff
@@ -4,7 +4,8 @@
 from SELDOMpy.buildmim import *
 from SELDOMpy.simulate_logic_based_ode import *
 from SELDOMpy.getLBODEmodel import *
 from SELDOMpy.gen_exps import *
 from SELDOMpy.getRandomLBODEmodel import *
 from SELDOMpy.reduce_fun import *
 from SELDOMpy.optimization import *
+import pickle
```

## Comparing `SELDOMpy-0.7.1.dist-info/LICENSE.txt` & `SELDOMpy-0.7.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `SELDOMpy-0.7.1.dist-info/METADATA` & `SELDOMpy-0.7.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.7.1
+Version: 0.7.2
 Summary: hardware acceleration
 Home-page: https://github.com/voxy/accel.git
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: mealpy
 Requires-Dist: matplotlib
 Requires-Dist: setuptools
 Requires-Dist: openpyxl
+Requires-Dist: pickle
 
 
 The package generates dynamic models of cellular signalling networks from experimental data taken from the nodes that make up the network.
 To install it use: 
 
 `pip install SELDOMpy`
```

## Comparing `SELDOMpy-0.7.1.dist-info/RECORD` & `SELDOMpy-0.7.2.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 hello.cp38-win_amd64.pyd,sha256=xGXrsp2Vk2gg55Ipe0ycGjizk6u-uBBu33rWOxdMVKU,265216
 sim_logic_ode.cp38-win_amd64.pyd,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-SELDOMpy/__init__.py,sha256=nYwHyr1yB_-2FBG4eo6CP2kQWrlsrmrsS3mBFhWihlc,390
+SELDOMpy/__init__.py,sha256=8Wo4RFbJA8dkvM2aUFSTfZrgwtfZihi4x2AzrlPaRhI,405
 SELDOMpy/buildmim.py,sha256=Emoldi9Wbim-AGjddfTOxef0cTmvo_08CnnWyhwqzCA,2309
 SELDOMpy/extras.py,sha256=yVr0jGpS5nE9FmRUFpLLnrith3CvErUx0BNMAUAUCQo,1271
 SELDOMpy/gen_exps.py,sha256=yFQ7AcG5X9B1RTFv3r6iWpSQ03EwCXHwPfjylCax_iA,4159
 SELDOMpy/getLBODEmodel.py,sha256=gDggNkCa9x4WVBTRjuCvTms8mqOp4EogzlARjJGYzNY,4838
 SELDOMpy/getRandomLBODEmodel.py,sha256=jJhhiLuc8ZTfrqV7mHLGdtI1nnf9-ZTBW5pqxvWmVkw,3232
 SELDOMpy/opt_mealpy.py,sha256=p3mezQmWQwgEBmn9Ce4YzqOVZPgXyn6nqlslMUhiwNw,2460
 SELDOMpy/optimization.py,sha256=p3mezQmWQwgEBmn9Ce4YzqOVZPgXyn6nqlslMUhiwNw,2460
@@ -62,12 +62,12 @@
 SELDOMpy/src/sundials_direct.c,sha256=3fTxm9kVfmfj7kbIbOpEPpd0AWQaCydha5uhUoc6WEA,6225
 SELDOMpy/src/sundials_iterative.c,sha256=Okb4iAhwTcj3tsKgJVWPxq2KlbRTQMAdZAwrSL9Bx28,7662
 SELDOMpy/src/sundials_math.c,sha256=18wLmG9SCGyQr1TzcIxuSQQWddHz4M5mYy5RI4TKtlc,2474
 SELDOMpy/src/sundials_nvector.c,sha256=7N9Pol7nbeWut0OHfM8F70iboGcI-BuEA7JIHhJAiBs,4702
 SELDOMpy/src/sundials_spbcgs.c,sha256=Bs3K_hAB5no6aKv5Tppwu8OGOPCpw6bFiAU_E0ePcnY,9663
 SELDOMpy/src/sundials_spgmr.c,sha256=KKRd_fpxv2V3DT0MOZxWZpO3KbXfseSJyV8bOnYeArk,12650
 SELDOMpy/src/sundials_sptfqmr.c,sha256=_d97GsT0yi9Zuh_SO7ZwQHT_Sb3JK-UOy5j9H3HXmTw,14744
-SELDOMpy-0.7.1.dist-info/LICENSE.txt,sha256=Z_R0qA8dBa_UBMGgM1fEedm0wV7CBqwIBaBEOu4iT5w,1077
-SELDOMpy-0.7.1.dist-info/METADATA,sha256=azD2bCIP3vDmFD8kEDfbBCsqQoF2U9iGwkTA3V1a8vE,777
-SELDOMpy-0.7.1.dist-info/WHEEL,sha256=F2aDWtWrilNM3-px1vBtJOEd7aRVTetQfFuDYmYbAUQ,100
-SELDOMpy-0.7.1.dist-info/top_level.txt,sha256=Ob79bfCTj_ucLsKNzB5Bea8oIrbiwekeNGRp4zxCiMg,15
-SELDOMpy-0.7.1.dist-info/RECORD,,
+SELDOMpy-0.7.2.dist-info/LICENSE.txt,sha256=Z_R0qA8dBa_UBMGgM1fEedm0wV7CBqwIBaBEOu4iT5w,1077
+SELDOMpy-0.7.2.dist-info/METADATA,sha256=J6FJXNt_tkLzqWUGN5EwByysMy6H_zzeZfuK-ktQ_DI,800
+SELDOMpy-0.7.2.dist-info/WHEEL,sha256=F2aDWtWrilNM3-px1vBtJOEd7aRVTetQfFuDYmYbAUQ,100
+SELDOMpy-0.7.2.dist-info/top_level.txt,sha256=Ob79bfCTj_ucLsKNzB5Bea8oIrbiwekeNGRp4zxCiMg,15
+SELDOMpy-0.7.2.dist-info/RECORD,,
```

