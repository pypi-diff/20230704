# Comparing `tmp/metric_visualizer-0.9.7-py3-none-any.whl.zip` & `tmp/metric_visualizer-0.9.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 24027 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      533 b- defN 23-Apr-12 21:02 metric_visualizer/__init__.py
+Zip file size: 24034 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      533 b- defN 23-Jul-04 16:32 metric_visualizer/__init__.py
 -rw-rw-rw-  2.0 fat     2693 b- defN 23-Jan-26 11:35 metric_visualizer/cli_command.py
 -rw-rw-rw-  2.0 fat    10250 b- defN 23-Feb-08 14:19 metric_visualizer/colalab.py
 -rw-rw-rw-  2.0 fat    74672 b- defN 23-Apr-12 21:02 metric_visualizer/metric_visualizer.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-Feb-16 15:24 metric_visualizer/utils.py
+-rw-rw-rw-  2.0 fat     3400 b- defN 23-Jul-04 16:32 metric_visualizer/utils.py
 -rw-rw-rw-  2.0 fat      379 b- defN 23-Jan-26 11:35 metric_visualizer/external/__init__.py
 -rw-rw-rw-  2.0 fat    10633 b- defN 23-Jan-26 11:35 metric_visualizer/external/scott_knott.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-12 21:02 metric_visualizer-0.9.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    14586 b- defN 23-Apr-12 21:02 metric_visualizer-0.9.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 21:02 metric_visualizer-0.9.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       86 b- defN 23-Apr-12 21:02 metric_visualizer-0.9.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       18 b- defN 23-Apr-12 21:02 metric_visualizer-0.9.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1174 b- defN 23-Apr-12 21:02 metric_visualizer-0.9.7.dist-info/RECORD
-13 files, 119487 bytes uncompressed, 22035 bytes compressed:  81.6%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-04 16:33 metric_visualizer-0.9.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    14586 b- defN 23-Jul-04 16:33 metric_visualizer-0.9.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 16:33 metric_visualizer-0.9.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       86 b- defN 23-Jul-04 16:33 metric_visualizer-0.9.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-04 16:33 metric_visualizer-0.9.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1174 b- defN 23-Jul-04 16:33 metric_visualizer-0.9.8.dist-info/RECORD
+13 files, 119603 bytes uncompressed, 22042 bytes compressed:  81.6%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: metric_visualizer/external/__init__.py
 Comment: 
 
 Filename: metric_visualizer/external/scott_knott.py
 Comment: 
 
-Filename: metric_visualizer-0.9.7.dist-info/LICENSE
+Filename: metric_visualizer-0.9.8.dist-info/LICENSE
 Comment: 
 
-Filename: metric_visualizer-0.9.7.dist-info/METADATA
+Filename: metric_visualizer-0.9.8.dist-info/METADATA
 Comment: 
 
-Filename: metric_visualizer-0.9.7.dist-info/WHEEL
+Filename: metric_visualizer-0.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: metric_visualizer-0.9.7.dist-info/entry_points.txt
+Filename: metric_visualizer-0.9.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: metric_visualizer-0.9.7.dist-info/top_level.txt
+Filename: metric_visualizer-0.9.8.dist-info/top_level.txt
 Comment: 
 
-Filename: metric_visualizer-0.9.7.dist-info/RECORD
+Filename: metric_visualizer-0.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metric_visualizer/__init__.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # file: __init__.py.py
 # time: 03/02/2022
 # author: yangheng <yangheng@m.scnu.edu.cn>
 # github: https://github.com/yangheng95
 # Copyright (C) 2021. All Rights Reserved.
 
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 __name__ = "metric_visualizer"
 
 from .metric_visualizer import MetricVisualizer
 from .colalab import reformat_tikz_format_for_colalab
 
 from update_checker import UpdateChecker
```

## metric_visualizer/utils.py

```diff
@@ -13,26 +13,30 @@
 class MetricList:
     def __init__(self, *args, **kwargs):
         self.data = list(*args, **kwargs)
         try:
             self.avg = np.nanmean(self.data)
             self.std = np.nanstd(self.data)
             self.median = np.nanmedian(self.data)
-            self.mode = stats.mode(self.data, keepdims=True)[0][0]
             self.max = np.nanmax(self.data)
             self.min = np.nanmin(self.data)
             self.var = np.nanvar(self.data)
             self.iqr = stats.iqr(self.data)
-            self.skewness = stats.skew(self.data, keepdims=True)
-            self.kurtosis = stats.kurtosis(self.data, keepdims=True)
             self.sum = np.nansum(self.data)
             self.count = len(self.data)
         except Exception as e:
             print("Can create MetricList with: ", self.data)
 
+        try:
+            # self.mode = stats.mode(self.data, keepdims=True)[0][0]
+            self.skewness = stats.skew(self.data, keepdims=True)
+            self.kurtosis = stats.kurtosis(self.data, keepdims=True)
+        except Exception as e:
+            print("Can not create MetricList with: ", self.data)
+
     def _update(self):
         self.avg = np.nanmean(self.data)
         self.std = np.nanstd(self.data)
         self.median = np.nanmedian(self.data)
         self.mode = stats.mode(self.data)[0][0]
         self.max = np.nanmax(self.data)
         self.min = np.nanmin(self.data)
```

## Comparing `metric_visualizer-0.9.7.dist-info/LICENSE` & `metric_visualizer-0.9.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `metric_visualizer-0.9.7.dist-info/METADATA` & `metric_visualizer-0.9.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metric-visualizer
-Version: 0.9.7
+Version: 0.9.8
 Summary: This is a tool for automated experimental metrics statistics and visualization
 Home-page: https://github.com/yangheng95/metric_visualizer
 Author: yang, Heng
 Author-email: hy345@exeter.ac.uk
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `metric_visualizer-0.9.7.dist-info/RECORD` & `metric_visualizer-0.9.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-metric_visualizer/__init__.py,sha256=hdkLgYMM5hrp6_q8ajnyIoRLjaNxjliYI7LgDS0wYp0,533
+metric_visualizer/__init__.py,sha256=Qq1c109i8iMHz-c1akueKfvDTL6QA3EJWxXQ5J10R3c,533
 metric_visualizer/cli_command.py,sha256=BmHMWQ23Fv9z_f7Cl1fGEktS5hmThYx9-_lQX3vBs-I,2693
 metric_visualizer/colalab.py,sha256=LCnpwqk7qWVMilJWsVPN2UWkXe65_vPDtzwU_RRviFY,10250
 metric_visualizer/metric_visualizer.py,sha256=JeK0dmJczMOVSLAsv4znwBMzP0oozH7FSi-_gj0YKis,74672
-metric_visualizer/utils.py,sha256=4blwkU2cMJGFfbQsiHn5lDNhWRowA6sO3LR0QdSACAw,3284
+metric_visualizer/utils.py,sha256=TCUIUdxvaWx2qxkoVCRbLl5pYbN9-bttEuKwP55kXF4,3400
 metric_visualizer/external/__init__.py,sha256=aH4vIz0vkpZZ9MhjNDro1nxdQ2kaHacnb-_SGD6Pi7A,379
 metric_visualizer/external/scott_knott.py,sha256=E8i9phCZuGu-RcLO54K6EfT3xpUlbyqDRiykkFxW_o4,10633
-metric_visualizer-0.9.7.dist-info/LICENSE,sha256=xH48JJDkixpon7IStNFJAbqhwoLEst__CL6Y3h3jyy0,1087
-metric_visualizer-0.9.7.dist-info/METADATA,sha256=kWJHAgoot_FfaVhYpNhdhJ-qgMgcyeaZAnENk5H0wuY,14586
-metric_visualizer-0.9.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-metric_visualizer-0.9.7.dist-info/entry_points.txt,sha256=ZdI91JzkymX488O1KT_ferQXtnZWx9J7svzwT9og4p8,86
-metric_visualizer-0.9.7.dist-info/top_level.txt,sha256=tK8hrtk_KYQ58VPdt4sJuPBTJBYbwSOw6iDYKuVyIQE,18
-metric_visualizer-0.9.7.dist-info/RECORD,,
+metric_visualizer-0.9.8.dist-info/LICENSE,sha256=xH48JJDkixpon7IStNFJAbqhwoLEst__CL6Y3h3jyy0,1087
+metric_visualizer-0.9.8.dist-info/METADATA,sha256=_yQfbWR50lUwhIRKHorBhvmwNJK-E9sbX6j1t7iH6Sc,14586
+metric_visualizer-0.9.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+metric_visualizer-0.9.8.dist-info/entry_points.txt,sha256=ZdI91JzkymX488O1KT_ferQXtnZWx9J7svzwT9og4p8,86
+metric_visualizer-0.9.8.dist-info/top_level.txt,sha256=tK8hrtk_KYQ58VPdt4sJuPBTJBYbwSOw6iDYKuVyIQE,18
+metric_visualizer-0.9.8.dist-info/RECORD,,
```

