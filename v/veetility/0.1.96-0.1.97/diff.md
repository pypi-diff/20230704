# Comparing `tmp/veetility-0.1.96.tar.gz` & `tmp/veetility-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.96.tar", last modified: Tue Jul  4 10:10:43 2023, max compression
+gzip compressed data, was "veetility-0.1.97.tar", last modified: Tue Jul  4 10:25:05 2023, max compression
```

## Comparing `veetility-0.1.96.tar` & `veetility-0.1.97.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:10:43.436262 veetility-0.1.96/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-04 10:10:43.436077 veetility-0.1.96/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.96/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-04 10:10:43.436327 veetility-0.1.96/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-04 10:10:14.000000 veetility-0.1.96/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:10:43.428464 veetility-0.1.96/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.96/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.96/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.96/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:10:43.434725 veetility-0.1.96/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.96/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.96/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.96/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.96/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    31383 2023-07-04 10:05:41.000000 veetility-0.1.96/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.96/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53704 2023-07-04 10:08:58.000000 veetility-0.1.96/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.96/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.96/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:10:43.435851 veetility-0.1.96/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-04 10:10:43.000000 veetility-0.1.96/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-04 10:10:43.000000 veetility-0.1.96/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-04 10:10:43.000000 veetility-0.1.96/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-04 10:10:43.000000 veetility-0.1.96/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-04 10:10:43.000000 veetility-0.1.96/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.119838 veetility-0.1.97/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-04 10:25:05.119674 veetility-0.1.97/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.97/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-04 10:25:05.119903 veetility-0.1.97/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-04 10:25:01.000000 veetility-0.1.97/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.114960 veetility-0.1.97/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.97/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.97/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.97/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.118344 veetility-0.1.97/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.97/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.97/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.97/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.97/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    31537 2023-07-04 10:24:35.000000 veetility-0.1.97/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.97/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    53704 2023-07-04 10:08:58.000000 veetility-0.1.97/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.97/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.97/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-04 10:25:05.119458 veetility-0.1.97/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-04 10:25:04.000000 veetility-0.1.97/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-04 10:25:05.000000 veetility-0.1.97/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-04 10:25:04.000000 veetility-0.1.97/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-04 10:25:04.000000 veetility-0.1.97/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-04 10:25:05.000000 veetility-0.1.97/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.96/PKG-INFO` & `veetility-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.96
+Version: 0.1.97
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.96/README.md` & `veetility-0.1.97/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/setup.py` & `veetility-0.1.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.96",
+    version="0.1.97",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.96/tests/test_best_fuzzy_match_dict.py` & `veetility-0.1.97/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/tests/test_identify_match_multi_cols.py` & `veetility-0.1.97/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/tests/test_prepare_string_matching.py` & `veetility-0.1.97/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility/cleaning_functions.py` & `veetility-0.1.97/veetility/cleaning_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility/generic_functions.py` & `veetility-0.1.97/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility/point_to_point_regressor.py` & `veetility-0.1.97/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility/quality_assessments.py` & `veetility-0.1.97/veetility/quality_assessments.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,19 @@
         logger.info(f'Num of rows in {name_of_df} = {num_rows}')
         paid_or_organic = self.util.identify_paid_or_organic(df)
         
         if cols_to_check == None:
             if paid_or_organic == 'Paid':
                 #Include date in paid duplicate check because the same ad is repeated across consequitve days
                 #Spend is a good indicator of duplicates in paid data
-                cols_to_check = ['date', 'platform', 'country', 'media_type', 'cohort', 'message', 'ad_name', 'spend']
+                if 'spend_usd' in df.columns:
+                    spend_col = 'spend_usd'
+                else:
+                    spend_col = 'spend'
+                cols_to_check = ['date', 'platform', 'country', 'media_type', 'cohort', 'message', 'ad_name', spend_col]
                 
             elif paid_or_organic == 'Organic':
                 cols_to_check = ['platform', 'country', 'media_type' , 'message', 'url']
                 if 'date_row_added' in df.columns:
                     cols_to_check.append('date_row_added')
         
         if cols_to_add != None:
```

### Comparing `veetility-0.1.96/veetility/snowflake.py` & `veetility-0.1.97/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility/utility_functions.py` & `veetility-0.1.97/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility/v_lift.py` & `veetility-0.1.97/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility/view_through_rate.py` & `veetility-0.1.97/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.96/veetility.egg-info/PKG-INFO` & `veetility-0.1.97/veetility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.96
+Version: 0.1.97
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.96/veetility.egg-info/SOURCES.txt` & `veetility-0.1.97/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

