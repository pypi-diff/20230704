# Comparing `tmp/lesscode_charts-0.0.5.tar.gz` & `tmp/lesscode_charts-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_charts-0.0.5.tar", last modified: Mon Jun  5 10:18:21 2023, max compression
+gzip compressed data, was "dist/lesscode_charts-0.0.6.tar", last modified: Tue Jul  4 08:45:23 2023, max compression
```

## Comparing `lesscode_charts-0.0.5.tar` & `lesscode_charts-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.5/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.5/lesscode_charts/__init__.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts/utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.5/lesscode_charts/utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.5/lesscode_charts/utils/common_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts/v1/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.5/lesscode_charts/v1/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.5/lesscode_charts/v1/forest_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3459 2023-06-05 09:16:34.000000 lesscode_charts-0.0.5/lesscode_charts/v1/histogram_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.5/lesscode_charts/v1/k_line_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1441 2023-06-05 10:18:19.000000 lesscode_charts-0.0.5/lesscode_charts/v1/pie_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1058 2023-05-19 07:29:22.000000 lesscode_charts-0.0.5/lesscode_charts/v1/pyramid_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.5/lesscode_charts/v1/radar_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 11:03:04.000000 lesscode_charts-0.0.5/lesscode_charts/v1/sankey_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.5/lesscode_charts/v1/table_chart.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-05 10:18:19.000000 lesscode_charts-0.0.5/lesscode_charts/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      611 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/lesscode_charts.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-05 10:18:21.000000 lesscode_charts-0.0.5/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.5/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.6/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.6/lesscode_charts/__init__.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts/utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.6/lesscode_charts/utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.6/lesscode_charts/utils/common_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts/v1/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.6/lesscode_charts/v1/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.6/lesscode_charts/v1/forest_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3459 2023-06-05 09:16:34.000000 lesscode_charts-0.0.6/lesscode_charts/v1/histogram_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.6/lesscode_charts/v1/k_line_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1444 2023-07-04 08:44:48.000000 lesscode_charts-0.0.6/lesscode_charts/v1/pie_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1143 2023-07-04 08:44:48.000000 lesscode_charts-0.0.6/lesscode_charts/v1/pyramid_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.6/lesscode_charts/v1/radar_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 11:03:04.000000 lesscode_charts-0.0.6/lesscode_charts/v1/sankey_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.6/lesscode_charts/v1/table_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-04 08:45:12.000000 lesscode_charts-0.0.6/lesscode_charts/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      611 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.6/setup.py
```

### Comparing `lesscode_charts-0.0.5/lesscode_charts/utils/common_utils.py` & `lesscode_charts-0.0.6/lesscode_charts/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/forest_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/forest_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/histogram_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/histogram_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/k_line_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/k_line_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/pie_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/pie_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             total = sum([_ for _ in new_data.values()])
         if total == 0:
             total = 1
         result = {
             "title": title,
             "series": [
                 {
-                    "name": "",
+                    "name": title,
                     "data": [
                         {"name": k, "value": v, "unit": unit,
                          "proportion": round(v / total * 100, decimal_place)} for k, v in
                         new_data.items()
                     ],
                     "unit": unit,
                 }
```

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/pyramid_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/pyramid_chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 """
 金字塔处理
 """
 
 
 class PyramidChart:
     @staticmethod
-    def pyramid(data: List[dict], unit="", title: str = "", decimal_place: int = 2, **kwargs):
+    def pyramid(data: List[dict], unit="", title: str = "", decimal_place: int = 2, total:int=None,**kwargs):
         """
+        :param total: 计算比例的总数
         :param data: 数据，示例:[{"name":"上市企业","value":1}]
         :param unit: 数据单位
         :param title: 图题
         :param decimal_place: 小数点位数
         :param kwargs: 设置pool
         :return:
         """
-        total = sum([_.get("value") for _ in data if _.get("value")])
+        if not total:
+            total = sum([_.get("value") for _ in data if _.get("value")])
         if total == 0:
             total = 1
         result = {
             "title": title,
             "series": [
                 {
                     "name": title,
```

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/radar_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/radar_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/sankey_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/sankey_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/lesscode_charts/v1/table_chart.py` & `lesscode_charts-0.0.6/lesscode_charts/v1/table_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/lesscode_charts.egg-info/SOURCES.txt` & `lesscode_charts-0.0.6/lesscode_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.5/setup.py` & `lesscode_charts-0.0.6/setup.py`

 * *Files identical despite different names*

