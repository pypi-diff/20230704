# Comparing `tmp/veetility-0.1.94.tar.gz` & `tmp/veetility-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.94.tar", last modified: Mon Jul  3 13:10:51 2023, max compression
+gzip compressed data, was "veetility-0.1.95.tar", last modified: Mon Jul  3 14:30:08 2023, max compression
```

## Comparing `veetility-0.1.94.tar` & `veetility-0.1.95.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.598542 veetility-0.1.94/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-03 13:10:51.598381 veetility-0.1.94/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.94/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-03 13:10:51.598599 veetility-0.1.94/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-03 13:10:47.000000 veetility-0.1.94/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.593708 veetility-0.1.94/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.94/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.94/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.94/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.596959 veetility-0.1.94/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.94/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.94/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.94/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.94/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    31242 2023-07-03 13:10:09.000000 veetility-0.1.94/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.94/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-26 09:44:14.000000 veetility-0.1.94/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.94/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.94/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 13:10:51.598015 veetility-0.1.94/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-03 13:10:51.000000 veetility-0.1.94/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 14:30:08.610565 veetility-0.1.95/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-03 14:30:08.610423 veetility-0.1.95/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.95/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-07-03 14:30:08.610628 veetility-0.1.95/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-07-03 14:30:02.000000 veetility-0.1.95/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 14:30:08.606963 veetility-0.1.95/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.95/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.95/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.95/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 14:30:08.609361 veetility-0.1.95/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.95/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-27 09:01:02.000000 veetility-0.1.95/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.95/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.95/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    31382 2023-07-03 14:29:18.000000 veetility-0.1.95/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.95/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-26 09:44:14.000000 veetility-0.1.95/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.95/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.95/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-07-03 14:30:08.610225 veetility-0.1.95/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-07-03 14:30:08.000000 veetility-0.1.95/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-07-03 14:30:08.000000 veetility-0.1.95/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-07-03 14:30:08.000000 veetility-0.1.95/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-07-03 14:30:08.000000 veetility-0.1.95/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-07-03 14:30:08.000000 veetility-0.1.95/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.94/PKG-INFO` & `veetility-0.1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.94
+Version: 0.1.95
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.94/README.md` & `veetility-0.1.95/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/setup.py` & `veetility-0.1.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.94",
+    version="0.1.95",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.94/tests/test_best_fuzzy_match_dict.py` & `veetility-0.1.95/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/tests/test_identify_match_multi_cols.py` & `veetility-0.1.95/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/tests/test_prepare_string_matching.py` & `veetility-0.1.95/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility/cleaning_functions.py` & `veetility-0.1.95/veetility/cleaning_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility/generic_functions.py` & `veetility-0.1.95/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility/point_to_point_regressor.py` & `veetility-0.1.95/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility/quality_assessments.py` & `veetility-0.1.95/veetility/quality_assessments.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,16 @@
             #Turn the most recent entry in the historic db into a dict
             old_dict = historic_db.sort_values(by='Date', ascending=False).iloc[0].to_dict()
 
             # for each key in the old dict, check if it is in the new dict and if it is, check if it has increased or decreased too much
             for key, value in old_dict.items():
 
                 if key == 'Columns':
+                    value = value.replace('{', '').replace('}', '')
+                    value = [part.strip() for part in value.split(',')]
                     if set(value) != set(new_dict['Columns']):
                         error_occured = True
                         columns_removed = list(set(value) - set(new_dict['Columns']))
                         columns_added = list(set(new_dict['Columns']) - set(value))
                         error_message = error_message + '  ' + f'The columns seems to have changed from last time,\n'\
                                                 f' Columns that were added = {columns_added}\n' \
                                                 f' Columns that were removed = {columns_removed}\n'
```

### Comparing `veetility-0.1.94/veetility/snowflake.py` & `veetility-0.1.95/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility/utility_functions.py` & `veetility-0.1.95/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility/v_lift.py` & `veetility-0.1.95/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility/view_through_rate.py` & `veetility-0.1.95/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.94/veetility.egg-info/PKG-INFO` & `veetility-0.1.95/veetility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.94
+Version: 0.1.95
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.94/veetility.egg-info/SOURCES.txt` & `veetility-0.1.95/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

