# Comparing `tmp/spark_plotting_tools-0.2.0.tar.gz` & `tmp/spark_plotting_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_plotting_tools-0.2.0.tar", last modified: Tue Jul  4 02:49:29 2023, max compression
+gzip compressed data, was "spark_plotting_tools-0.3.0.tar", last modified: Tue Jul  4 03:24:53 2023, max compression
```

## Comparing `spark_plotting_tools-0.2.0.tar` & `spark_plotting_tools-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 02:49:29.972831 spark_plotting_tools-0.2.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_plotting_tools-0.2.0/LICENSE
--rw-rw-rw-   0        0        0        4 2023-06-26 03:19:39.000000 spark_plotting_tools-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4272 2023-07-04 02:49:29.972831 spark_plotting_tools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3509 2023-07-03 07:29:25.000000 spark_plotting_tools-0.2.0/README.md
--rw-rw-rw-   0        0        0      623 2023-07-03 09:41:25.000000 spark_plotting_tools-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-04 02:49:29.976831 spark_plotting_tools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-07-04 02:49:05.000000 spark_plotting_tools-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:49:29.949997 spark_plotting_tools-0.2.0/spark_plotting_tools/
--rw-rw-rw-   0        0        0      614 2023-07-03 09:20:17.000000 spark_plotting_tools-0.2.0/spark_plotting_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:49:29.970830 spark_plotting_tools-0.2.0/spark_plotting_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_plotting_tools-0.2.0/spark_plotting_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     5536 2023-07-04 02:48:54.000000 spark_plotting_tools-0.2.0/spark_plotting_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:49:29.972831 spark_plotting_tools-0.2.0/spark_plotting_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_plotting_tools-0.2.0/spark_plotting_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_plotting_tools-0.2.0/spark_plotting_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:49:29.969830 spark_plotting_tools-0.2.0/spark_plotting_tools.egg-info/
--rw-rw-rw-   0        0        0     4272 2023-07-04 02:49:29.000000 spark_plotting_tools-0.2.0/spark_plotting_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-07-04 02:49:29.000000 spark_plotting_tools-0.2.0/spark_plotting_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 02:49:29.000000 spark_plotting_tools-0.2.0/spark_plotting_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2023-07-04 02:49:29.000000 spark_plotting_tools-0.2.0/spark_plotting_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-04 02:49:29.000000 spark_plotting_tools-0.2.0/spark_plotting_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:53.271019 spark_plotting_tools-0.3.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_plotting_tools-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0        4 2023-06-26 03:19:39.000000 spark_plotting_tools-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4272 2023-07-04 03:24:53.271019 spark_plotting_tools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3509 2023-07-03 07:29:25.000000 spark_plotting_tools-0.3.0/README.md
+-rw-rw-rw-   0        0        0      623 2023-07-03 09:41:25.000000 spark_plotting_tools-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-04 03:24:53.271019 spark_plotting_tools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-07-04 03:24:38.000000 spark_plotting_tools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:53.256292 spark_plotting_tools-0.3.0/spark_plotting_tools/
+-rw-rw-rw-   0        0        0      614 2023-07-03 09:20:17.000000 spark_plotting_tools-0.3.0/spark_plotting_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:53.271019 spark_plotting_tools-0.3.0/spark_plotting_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_plotting_tools-0.3.0/spark_plotting_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     6107 2023-07-04 03:24:38.000000 spark_plotting_tools-0.3.0/spark_plotting_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:53.271019 spark_plotting_tools-0.3.0/spark_plotting_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_plotting_tools-0.3.0/spark_plotting_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_plotting_tools-0.3.0/spark_plotting_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:53.271019 spark_plotting_tools-0.3.0/spark_plotting_tools.egg-info/
+-rw-rw-rw-   0        0        0     4272 2023-07-04 03:24:53.000000 spark_plotting_tools-0.3.0/spark_plotting_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-07-04 03:24:53.000000 spark_plotting_tools-0.3.0/spark_plotting_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 03:24:53.000000 spark_plotting_tools-0.3.0/spark_plotting_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-07-04 03:24:53.000000 spark_plotting_tools-0.3.0/spark_plotting_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-04 03:24:53.000000 spark_plotting_tools-0.3.0/spark_plotting_tools.egg-info/top_level.txt
```

### Comparing `spark_plotting_tools-0.2.0/LICENSE` & `spark_plotting_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_plotting_tools-0.2.0/PKG-INFO` & `spark_plotting_tools-0.3.0/spark_plotting_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spark_plotting_tools
-Version: 0.2.0
+Name: spark-plotting-tools
+Version: 0.3.0
 Summary: spark_plotting_tools
 Home-page: https://github.com/jonaqp/spark_plotting_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_plotting_tools/archive/main.zip
 Keywords: spark,plot
```

### Comparing `spark_plotting_tools-0.2.0/README.md` & `spark_plotting_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_plotting_tools-0.2.0/pyproject.toml` & `spark_plotting_tools-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_plotting_tools-0.2.0/setup.py` & `spark_plotting_tools-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_plotting_tools',
     packages=find_packages(),
-    version='0.2.0',
+    version='0.3.0',
     description='spark_plotting_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_plotting_tools/',
     download_url='https://github.com/jonaqp/spark_plotting_tools/archive/main.zip',
```

### Comparing `spark_plotting_tools-0.2.0/spark_plotting_tools/__init__.py` & `spark_plotting_tools-0.3.0/spark_plotting_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_plotting_tools-0.2.0/spark_plotting_tools/functions/generator.py` & `spark_plotting_tools-0.3.0/spark_plotting_tools/functions/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -82,28 +82,40 @@
     ax1.pie(values, labels=names, autopct='%1.2f%%')
     ax1.axis('equal')
     plt.show()
 
     del df
 
 
-def plot_generated_lineplot(df=None, date_col="date_col", col=None, agg_func="count"):
+def plot_generated_lineplot(spark=None, path=None, col=None, months="{01}", years="{2023}", agg_func="count"):
     import matplotlib.pyplot as plt
     from spark_plotting_tools.utils.color import get_color_b
     from pyspark.sql import functions as func
     import seaborn as sns
+    import os
+    import sys
 
     sns.set_style("whitegrid")
     sns.set_palette("Set2")
-    df = df.select(date_col, col)
-    df2 = df.withColumn(date_col, func.col(date_col).cast("date")) \
-        .withColumn("DAY", func.format_string("%02d", func.dayofmonth(date_col))) \
-        .withColumn("YEAR_MONTH", func.concat(func.year(date_col),
+    is_windows = sys.platform.startswith('win')
+    days = "{01,02,03,04,05,06,07,08,09,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31}"
+    cutoff_date = f"{years}-{months}-{days}"
+    path_master = os.path.join(path, f"cutoff_date={cutoff_date}")
+    if is_windows:
+        path_master = path_master.replace("\\", "/")
+
+    df = spark.read.parquet(path_master)
+    df = df.withColumn('date_col', func.regexp_extract(func.input_file_name(), r'(\d{4})-(\d{2})-(\d{2})', 0))
+
+    df = df.select("date_col", col)
+    df2 = df.withColumn("date_col", func.col("date_col").cast("date")) \
+        .withColumn("DAY", func.format_string("%02d", func.dayofmonth("date_col"))) \
+        .withColumn("YEAR_MONTH", func.concat(func.year("date_col"),
                                               func.lit("-"),
-                                              func.format_string("%02d", func.month(date_col))))
+                                              func.format_string("%02d", func.month("date_col"))))
     df2 = df2.groupBy("YEAR_MONTH", "DAY").agg(func.mean(col).alias("mean"),
                                                func.count(col).alias("count"))
     df2 = df2.withColumn("YEAR", func.substring("YEAR_MONTH", 1, 4)) \
         .withColumn("MONTH", func.substring("YEAR_MONTH", 6, 7))
     year_list = [col[0] for col in df2.select("YEAR").distinct().orderBy(func.col("YEAR").desc()).limit(2).collect()]
     df2 = df2.filter(func.col("YEAR").isin(year_list)) \
         .orderBy(func.col("YEAR_MONTH").desc(), func.col("DAY").asc())
```

### Comparing `spark_plotting_tools-0.2.0/spark_plotting_tools.egg-info/PKG-INFO` & `spark_plotting_tools-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spark-plotting-tools
-Version: 0.2.0
+Name: spark_plotting_tools
+Version: 0.3.0
 Summary: spark_plotting_tools
 Home-page: https://github.com/jonaqp/spark_plotting_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_plotting_tools/archive/main.zip
 Keywords: spark,plot
```

