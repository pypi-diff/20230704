# Comparing `tmp/dms-influx2-0.2.9.tar.gz` & `tmp/dms-influx2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.2.9.tar", last modified: Mon Jul  3 09:38:48 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.3.0.tar", last modified: Tue Jul  4 18:28:42 2023, max compression
```

## Comparing `dms-influx2-0.2.9.tar` & `dms-influx2-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.623565 dms-influx2-0.2.9/
--rw-rw-rw-   0        0        0      556 2023-07-03 09:38:48.623565 dms-influx2-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.611539 dms-influx2-0.2.9/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.2.9/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.2.9/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.2.9/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.2.9/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    21500 2023-04-11 13:17:17.000000 dms-influx2-0.2.9/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     7217 2023-04-11 05:18:02.000000 dms-influx2-0.2.9/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.2.9/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.2.9/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.2.9/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.621564 dms-influx2-0.2.9/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 09:38:48.000000 dms-influx2-0.2.9/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 09:38:48.624564 dms-influx2-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-07-03 09:38:14.000000 dms-influx2-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 09:38:48.623565 dms-influx2-0.2.9/tests/
--rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.2.9/tests/test_auth.py
--rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.2.9/tests/test_buckets.py
--rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.2.9/tests/test_copy-values.py
--rw-rw-rw-   0        0        0    11926 2023-07-03 09:34:27.000000 dms-influx2-0.2.9/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:28:42.575109 dms-influx2-0.3.0/
+-rw-rw-rw-   0        0        0      556 2023-07-04 18:28:42.574107 dms-influx2-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 18:28:42.544001 dms-influx2-0.3.0/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.0/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.0/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.0/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.0/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    21500 2023-04-11 13:17:17.000000 dms-influx2-0.3.0/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7216 2023-07-04 18:26:30.000000 dms-influx2-0.3.0/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.0/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.0/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.0/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:28:42.556511 dms-influx2-0.3.0/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-07-04 18:28:42.000000 dms-influx2-0.3.0/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-04 18:28:42.000000 dms-influx2-0.3.0/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 18:28:42.000000 dms-influx2-0.3.0/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-04 18:28:42.000000 dms-influx2-0.3.0/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 18:28:42.000000 dms-influx2-0.3.0/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 18:28:42.575109 dms-influx2-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-07-04 18:27:57.000000 dms-influx2-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 18:28:42.574107 dms-influx2-0.3.0/tests/
+-rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.0/tests/test_auth.py
+-rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.0/tests/test_buckets.py
+-rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.0/tests/test_copy-values.py
+-rw-rw-rw-   0        0        0    11926 2023-07-03 09:34:27.000000 dms-influx2-0.3.0/tests/test_data.py
```

### Comparing `dms-influx2-0.2.9/PKG-INFO` & `dms-influx2-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.9
+Version: 0.3.0
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.9/dms_influx2/authorizations.py` & `dms-influx2-0.3.0/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/buckets.py` & `dms-influx2-0.3.0/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/checks.py` & `dms-influx2-0.3.0/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/decorators.py` & `dms-influx2-0.3.0/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/delete.py` & `dms-influx2-0.3.0/dms_influx2/delete.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/dtv_files.py` & `dms-influx2-0.3.0/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/lib.py` & `dms-influx2-0.3.0/dms_influx2/lib.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/notifications.py` & `dms-influx2-0.3.0/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/organisations.py` & `dms-influx2-0.3.0/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/query.py` & `dms-influx2-0.3.0/dms_influx2/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     if bucket is None:
         raise ValueError("Invalid value for `bucket`, must not be `None`")
 
     stop = None
 
     if time_range == 'all':
-        time_range = '100y'
+        time_range = '50y'
 
     if time_range is not None:
         start = f"-{time_range}"
     else:
         start = "-1h"
 
     if time_from is not None:
```

### Comparing `dms-influx2-0.2.9/dms_influx2/tasks.py` & `dms-influx2-0.3.0/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2/utils.py` & `dms-influx2-0.3.0/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.3.0/dms_influx2.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.2.9
+Version: 0.3.0
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.2.9/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.3.0/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/setup.py` & `dms-influx2-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.2.9'
+VERSION = '0.3.0'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `dms-influx2-0.2.9/tests/test_auth.py` & `dms-influx2-0.3.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/tests/test_buckets.py` & `dms-influx2-0.3.0/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/tests/test_copy-values.py` & `dms-influx2-0.3.0/tests/test_copy-values.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.2.9/tests/test_data.py` & `dms-influx2-0.3.0/tests/test_data.py`

 * *Files identical despite different names*

