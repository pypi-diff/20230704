# Comparing `tmp/dq_module-1.1.3.tar.gz` & `tmp/dq_module-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dq_module-1.1.3.tar", last modified: Fri Jun 30 08:42:58 2023, max compression
+gzip compressed data, was "dist/dq_module-1.1.4.tar", last modified: Tue Jul  4 10:27:28 2023, max compression
```

## Comparing `dq_module-1.1.3.tar` & `dq_module-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-06-30 08:42:58.000000 dq_module-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11346 2023-06-30 08:42:41.000000 dq_module-1.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/dataqualitycheck/
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10482 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/consistencycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    37781 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/dataprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/dataqualitycheck/datasources/
--rw-rw-rw-   0 root         (0) root         (0)     7917 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/azureblobdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5534 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/databricksfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/databrickssqldf.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/datasources/localfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     5366 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/enumfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    42396 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckpolars.py
--rw-rw-rw-   0 root         (0) root         (0)    38755 2023-06-30 08:42:41.000000 dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckspark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-30 08:42:58.000000 dq_module-1.1.3/dq_module.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 08:42:58.000000 dq_module-1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-06-30 08:42:41.000000 dq_module-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-07-04 10:27:28.000000 dq_module-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2023-07-04 10:27:11.000000 dq_module-1.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/dataqualitycheck/
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10482 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/consistencycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    37781 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/dataprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/dataqualitycheck/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)     7917 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/azureblobdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5534 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/databricksfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/databrickssqldf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/localfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5366 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/enumfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    42396 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckpolars.py
+-rw-rw-rw-   0 root         (0) root         (0)    40543 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckspark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 10:27:28.000000 dq_module-1.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-04 10:27:11.000000 dq_module-1.1.4/setup.py
```

### Comparing `dq_module-1.1.3/PKG-INFO` & `dq_module-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_module
-Version: 1.1.3
+Version: 1.1.4
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.3/README.md` & `dq_module-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/commonutilities.py` & `dq_module-1.1.4/dataqualitycheck/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/consistencycheck.py` & `dq_module-1.1.4/dataqualitycheck/consistencycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/dataprofile.py` & `dq_module-1.1.4/dataqualitycheck/dataprofile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/datasources/azureblobdf.py` & `dq_module-1.1.4/dataqualitycheck/datasources/azureblobdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/datasources/commonutilities.py` & `dq_module-1.1.4/dataqualitycheck/datasources/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/datasources/databricksfilesystemdf.py` & `dq_module-1.1.4/dataqualitycheck/datasources/databricksfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/datasources/databrickssqldf.py` & `dq_module-1.1.4/dataqualitycheck/datasources/databrickssqldf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/datasources/localfilesystemdf.py` & `dq_module-1.1.4/dataqualitycheck/datasources/localfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/enumfile.py` & `dq_module-1.1.4/dataqualitycheck/enumfile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheck.py` & `dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckpolars.py` & `dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckpolars.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/dataqualitycheck/singledatasetqualitycheckspark.py` & `dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckspark.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,49 @@
 
             total_records_df = self.spark.createDataFrame(total_records_rows, schema=eval(
                 schema_enforce_structure(column_names, ",".join(['str']*len(column_names.split(','))))))
             total_records_df = total_records_df.dropDuplicates(total_records_df.columns)
         except Exception as e:
             raise Exception(e)
         return total_records_df
+    
+    def null_check_V1(self,df, rule, write_failed_records_flag):
+        run_date = date.today().strftime("%Y/%m/%d")
+        start = time.time()
+        total_row_count = df.count()
+        columnList = list(rule["column_to_be_checked"].split(","))
+
+        result = self.spark.createDataFrame([], df.schema)
+        column_passed = []
+        column_failed = []
+        for column in columnList:
+            failed_results = df.filter(col(column).isNull())
+            result = result.union(failed_results)
+            result = result.dropDuplicates()
+            failed_records_count = failed_results.count()
+            failed_records_write_location = 'N/A'
+            if failed_records_count == 0:
+                column_passed.append(column)
+            else:
+                column_failed.append(column)
+        
+        total_failed_records_count = result.count()
+
+        if len(column_passed) == len(columnList):
+            test_status = "PASS"
+        elif len(column_passed) < len(columnList):
+            test_status = "Passed: {} and Failed: {}".format(", ".join(column_passed), ", ".join(column_failed))
+        else:
+            test_status = "FAIL"
+
+        failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
+     
+        failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
+
+        return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if column have any null value.
     def null_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(col(rule["column_to_be_checked"]).isNull())
@@ -534,17 +569,18 @@
                     if 'active' in rule and int(rule['active']) == 0:
                         run_date = date.today().strftime("%Y/%m/%d")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "", "", "", "", 0, run_date))
                         continue
 
                     if rule["rule_name"] == "null_check":
-                        result_df = self.null_check(
+                        result_df = self.null_check_V1(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
+                    
                     elif rule["rule_name"] == "schema_check":
                         result_df = self.schema_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "range_min_check":
                         result_df = self.range_min_check(
                             self.dataframes[source], rule, write_failed_records_flag)
```

### Comparing `dq_module-1.1.3/dq_module.egg-info/PKG-INFO` & `dq_module-1.1.4/dq_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq-module
-Version: 1.1.3
+Version: 1.1.4
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.3/dq_module.egg-info/SOURCES.txt` & `dq_module-1.1.4/dq_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.3/setup.py` & `dq_module-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COMMAND ----------
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read() 
     
 setuptools.setup(
     name="dq_module",
-    version="1.1.3",
+    version="1.1.4",
     author="Sweta",
     author_email="sweta.swami@decisionpoint.in",
     description="data profiling and basic data quality rules check",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=setuptools.find_packages(include=['*']),
     packages=['dataqualitycheck', 'dataqualitycheck.datasources'],
```

