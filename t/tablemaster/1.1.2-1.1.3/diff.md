# Comparing `tmp/tablemaster-1.1.2.tar.gz` & `tmp/tablemaster-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.1.2.tar", last modified: Fri Jun 16 09:19:26 2023, max compression
+gzip compressed data, was "tablemaster-1.1.3.tar", last modified: Tue Jul  4 07:56:49 2023, max compression
```

## Comparing `tablemaster-1.1.2.tar` & `tablemaster-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-16 09:19:26.455368 tablemaster-1.1.2/
--rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.1.2/LICENSE
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-16 09:19:26.455254 tablemaster-1.1.2/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)     1487 2023-06-15 08:49:46.000000 tablemaster-1.1.2/README.md
--rw-r--r--   0 livid      (501) staff       (20)       38 2023-06-16 09:19:26.455401 tablemaster-1.1.2/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      559 2023-06-16 09:19:10.000000 tablemaster-1.1.2/setup.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-16 09:19:26.454439 tablemaster-1.1.2/tablemaster/
--rw-r--r--   0 livid      (501) staff       (20)      554 2023-06-16 08:49:52.000000 tablemaster-1.1.2/tablemaster/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.1.2/tablemaster/gspread.py
--rw-r--r--   0 livid      (501) staff       (20)     3460 2023-06-16 09:17:37.000000 tablemaster-1.1.2/tablemaster/local.py
--rw-r--r--   0 livid      (501) staff       (20)     3523 2023-06-15 07:01:48.000000 tablemaster-1.1.2/tablemaster/mysql.py
--rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.1.2/tablemaster/utils.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-06-16 09:19:26.455114 tablemaster-1.1.2/tablemaster.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-06-16 09:19:26.000000 tablemaster-1.1.2/tablemaster.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      310 2023-06-16 09:19:26.000000 tablemaster-1.1.2/tablemaster.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2023-06-16 09:19:26.000000 tablemaster-1.1.2/tablemaster.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)      108 2023-06-16 09:19:26.000000 tablemaster-1.1.2/tablemaster.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       12 2023-06-16 09:19:26.000000 tablemaster-1.1.2/tablemaster.egg-info/top_level.txt
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-07-04 07:56:49.052387 tablemaster-1.1.3/
+-rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.1.3/LICENSE
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-07-04 07:56:49.052260 tablemaster-1.1.3/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)     1729 2023-07-04 07:26:19.000000 tablemaster-1.1.3/README.md
+-rw-r--r--   0 livid      (501) staff       (20)       38 2023-07-04 07:56:49.052422 tablemaster-1.1.3/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      559 2023-07-04 07:56:02.000000 tablemaster-1.1.3/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-07-04 07:56:49.051411 tablemaster-1.1.3/tablemaster/
+-rw-r--r--   0 livid      (501) staff       (20)      597 2023-07-04 07:53:41.000000 tablemaster-1.1.3/tablemaster/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)      868 2023-07-04 07:53:14.000000 tablemaster-1.1.3/tablemaster/feishu.py
+-rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.1.3/tablemaster/gspread.py
+-rw-r--r--   0 livid      (501) staff       (20)     3334 2023-06-19 10:02:57.000000 tablemaster-1.1.3/tablemaster/local.py
+-rw-r--r--   0 livid      (501) staff       (20)     3523 2023-06-15 07:01:48.000000 tablemaster-1.1.3/tablemaster/mysql.py
+-rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.1.3/tablemaster/utils.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-07-04 07:56:49.052117 tablemaster-1.1.3/tablemaster.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-07-04 07:56:49.000000 tablemaster-1.1.3/tablemaster.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      332 2023-07-04 07:56:49.000000 tablemaster-1.1.3/tablemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2023-07-04 07:56:49.000000 tablemaster-1.1.3/tablemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)      108 2023-07-04 07:56:49.000000 tablemaster-1.1.3/tablemaster.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       12 2023-07-04 07:56:49.000000 tablemaster-1.1.3/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.1.2/LICENSE` & `tablemaster-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.2/README.md` & `tablemaster-1.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,32 @@
 ## query from mysql
 ```
 sql_query = 'SELECT * FROM table_name LIMIT 20'
 df = tm.query(sql_query, tm.cfg.db_name)
 df
 ```
 
+## import one file from local
+```
+df = tm.read("*Part of File Name*")
+df
+```
+
+## batch import and merge
+```
+df = tm.batch_read("*Part of File Name*")
+df
+```
+
+## batch import without merging
+```
+df = tm.read_dfs("*Part of File Name*")
+df
+```
+
 ## change column name
 ```
 sql_query = ('ALTER TABLE table_name RENAME COLUMN column1 TO column2')
 tm.opt(sql_query, tm.cfg.db_name)
 ```
 
 ## create a table in mysql and upload data from dataframe df
```

### Comparing `tablemaster-1.1.2/setup.py` & `tablemaster-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.1.2',
+    version='1.1.3',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy==1.4.46',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.1.2/tablemaster/__init__.py` & `tablemaster-1.1.3/tablemaster/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,29 @@
 import pandas as pd
 
 
 with open('cfg.yaml') as cfg:
     cfg = json.loads(json.dumps(load(cfg, Loader=Loader)), object_hook=lambda d: SimpleNamespace(**d))
 
 from . import utils
+
 from .mysql import (
     query,
     opt,
     Manage_table,
 )
+
 from .gspread import (
     gs_read_df,
     gs_write_df,
 )
 
 from .local import (
     read,
     batch_read,
     read_dfs,
 )
 
+from .feishu import (
+    fs_read_df,
+)
+
```

### Comparing `tablemaster-1.1.2/tablemaster/gspread.py` & `tablemaster-1.1.3/tablemaster/gspread.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.2/tablemaster/local.py` & `tablemaster-1.1.3/tablemaster/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def equal_table(df1, df2, det_col='nan'):
     if(len(df1) != len(df2)):
         return False
     elif df1.equals(df2):
         return True
     else:
         if det_col == 'nan':
-            return all(df1.iloc[:,0].fillna("").sort_values().reset_index(drop=True) == df2.iloc[:,0].fillna("").sort_values().reset_index(drop=True))
+            return False
         else:
             return all(df1[det_col].fillna("").sort_values().reset_index(drop=True).fillna(0) == df2[det_col].fillna("").sort_values().reset_index(drop=True))
 
 def read(file, det_header=True):
     if isinstance(file, pathlib.PosixPath):
         file = str(file)
     file_detect = list(Path().glob(file))
```

### Comparing `tablemaster-1.1.2/tablemaster/mysql.py` & `tablemaster-1.1.3/tablemaster/mysql.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.1.2/tablemaster/utils.py` & `tablemaster-1.1.3/tablemaster/utils.py`

 * *Files identical despite different names*

