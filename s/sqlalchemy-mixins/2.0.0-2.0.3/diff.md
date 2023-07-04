# Comparing `tmp/sqlalchemy_mixins-2.0.0.tar.gz` & `tmp/sqlalchemy_mixins-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mixins-2.0.0.tar", last modified: Mon Apr  3 21:04:01 2023, max compression
+gzip compressed data, was "sqlalchemy_mixins-2.0.3.tar", last modified: Tue Jul  4 14:34:18 2023, max compression
```

## Comparing `sqlalchemy_mixins-2.0.0.tar` & `sqlalchemy_mixins-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:04:01.601474 sqlalchemy_mixins-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-03 21:04:01.597474 sqlalchemy_mixins-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23491 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 21:04:01.601474 sqlalchemy_mixins-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:04:01.597474 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/activerecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/activerecord.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/eagerload.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/eagerload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/inspection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/repr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/serialize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/smartquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/smartquery.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-03 21:03:49.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:04:01.597474 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-03 21:04:01.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-03 21:04:01.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 21:04:01.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 21:04:01.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-03 21:04:01.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-03 21:04:01.000000 sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23491 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:18.961732 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/repr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/serialize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/top_level.txt
```

### Comparing `sqlalchemy_mixins-2.0.0/LICENSE.txt` & `sqlalchemy_mixins-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/PKG-INFO` & `sqlalchemy_mixins-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_mixins
-Version: 2.0.0
+Version: 2.0.3
 Summary: Active Record, Django-like queries, nested eager load and beauty __repr__ for SQLAlchemy
 Home-page: https://github.com/absent1706/sqlalchemy-mixins
 Download-URL: https://github.com/absent1706/sqlalchemy-mixins/archive/master.tar.gz
 Author: Alexander Litvinenko
 Author-email: litvinenko1706@gmail.com
 License: MIT
 Keywords: sqlalchemy,active record,activerecord,orm,django-like,django,eager load,eagerload,repr,__repr__,mysql,postgresql,pymysql,sqlite
```

### Comparing `sqlalchemy_mixins-2.0.0/README.md` & `sqlalchemy_mixins-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/setup.py` & `sqlalchemy_mixins-2.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def requirements():
     import os
     filename = os.path.join(os.path.dirname(__file__), 'requirements.txt')
     return [line.rstrip('\n') for line in open(filename).readlines()]
 
 setup(name='sqlalchemy_mixins',
-      version='2.0.0',
+      version='2.0.3',
       description='Active Record, Django-like queries, nested eager load '
                   'and beauty __repr__ for SQLAlchemy',
       url='https://github.com/absent1706/sqlalchemy-mixins',
       download_url='https://github.com/absent1706/sqlalchemy-mixins/archive/master.tar.gz',
       author='Alexander Litvinenko',
       author_email='litvinenko1706@gmail.com',
       license='MIT',
```

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/activerecord.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/activerecord.pyi` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/eagerload.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/eagerload.pyi` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/inspection.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/inspection.pyi` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/repr.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/repr.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/serialize.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/serialize.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/session.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/smartquery.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/smartquery.pyi` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/timestamp.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/timestamp.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins/utils.py` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/PKG-INFO` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mixins
-Version: 2.0.0
+Version: 2.0.3
 Summary: Active Record, Django-like queries, nested eager load and beauty __repr__ for SQLAlchemy
 Home-page: https://github.com/absent1706/sqlalchemy-mixins
 Download-URL: https://github.com/absent1706/sqlalchemy-mixins/archive/master.tar.gz
 Author: Alexander Litvinenko
 Author-email: litvinenko1706@gmail.com
 License: MIT
 Keywords: sqlalchemy,active record,activerecord,orm,django-like,django,eager load,eagerload,repr,__repr__,mysql,postgresql,pymysql,sqlite
```

### Comparing `sqlalchemy_mixins-2.0.0/sqlalchemy_mixins.egg-info/SOURCES.txt` & `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

