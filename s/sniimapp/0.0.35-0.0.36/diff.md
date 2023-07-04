# Comparing `tmp/sniimapp-0.0.35.tar.gz` & `tmp/sniimapp-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.35.tar", last modified: Tue Jul  4 16:20:24 2023, max compression
+gzip compressed data, was "sniimapp-0.0.36.tar", last modified: Tue Jul  4 16:23:38 2023, max compression
```

## Comparing `sniimapp-0.0.35.tar` & `sniimapp-0.0.36.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 16:20:24.402850 sniimapp-0.0.35/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.35/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-04 16:20:24.398851 sniimapp-0.0.35/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2023-07-02 06:32:13.000000 sniimapp-0.0.35/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-04 16:20:13.000000 sniimapp-0.0.35/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-04 16:20:24.402850 sniimapp-0.0.35/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 16:20:24.398851 sniimapp-0.0.35/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-04 16:20:24.000000 sniimapp-0.0.35/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-07-04 16:20:24.000000 sniimapp-0.0.35/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-04 16:20:24.000000 sniimapp-0.0.35/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-04 16:20:24.000000 sniimapp-0.0.35/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1559 2023-07-04 16:19:55.000000 sniimapp-0.0.35/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 16:23:38.738667 sniimapp-0.0.36/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.36/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-04 16:23:38.738667 sniimapp-0.0.36/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2023-07-02 06:32:13.000000 sniimapp-0.0.36/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-04 16:23:01.000000 sniimapp-0.0.36/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-04 16:23:38.738667 sniimapp-0.0.36/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-04 16:23:38.738667 sniimapp-0.0.36/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-04 16:23:38.000000 sniimapp-0.0.36/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-07-04 16:23:38.000000 sniimapp-0.0.36/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-04 16:23:38.000000 sniimapp-0.0.36/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-04 16:23:38.000000 sniimapp-0.0.36/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1555 2023-07-04 16:23:26.000000 sniimapp-0.0.36/sniimapp.py
```

### Comparing `sniimapp-0.0.35/LICENSE` & `sniimapp-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.35/PKG-INFO` & `sniimapp-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.35
+Version: 0.0.36
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.35/README.md` & `sniimapp-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.35/pyproject.toml` & `sniimapp-0.0.36/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.35"
+version = "0.0.36"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.35/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.36/sniimapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.35
+Version: 0.0.36
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sniimapp-0.0.35/sniimapp.py` & `sniimapp-0.0.36/sniimapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import datetime
 from pymongo import MongoClient
 import os
 import re
 
 class SNIIM():
 
-    #def __init__(self, collection, start_date, end_date, product='.*', origin='.*' ):
-    def __init__(self, collection, start_date, end_date):
+    def __init__(self, collection, start_date, end_date, product='.*', origin='.*' ):
+    #def __init__(self, collection, start_date, end_date):
         self.start_date = datetime.datetime.strptime(start_date, "%Y-%m-%d")
         self.end_date   = datetime.datetime.strptime(end_date,   "%Y-%m-%d")
         self.MONGO_HOST = '18.215.228.120'
         self.MONGO_PORT = 27017    
         self.MONGO_USER = 'sniim_read'  
         self.MONGO_PASSW ='sniim_read_x59m'    
         self.client = MongoClient(self._connection_string)
         self.MONGO_DB = 'sniim'                
         if collection == 'fyh':
             self.db_collection = 'sniim_fyh'
         if collection == 'granos':
             self.db_collection = 'sniim_granos'
         self.db = self.client[self.MONGO_DB]
         self.collection = self.db[self.db_collection]
-        #self.origin = origin
-        #self.product = product
+        self.origin = origin
+        self.product = product
 
     def get_data(self):
-        #product = rgx = re.compile('.*'+str(self.product)+'.*', re.IGNORECASE)  
-        #origin  = rgx = re.compile('.*'+str(self.origin)+'.*', re.IGNORECASE)
-        #return self.collection.find({"fecha":{"$gte":self.start_date,"$lte":self.end_date}, "producto":product, "origen":origin })
-        return self.collection.find({"fecha":{"$gte":self.start_date,"$lte":self.end_date}})
+        product = rgx = re.compile('.*'+str(self.product)+'.*', re.IGNORECASE)  
+        origin  = rgx = re.compile('.*'+str(self.origin)+'.*', re.IGNORECASE)
+        return self.collection.find({"fecha":{"$gte":self.start_date,"$lte":self.end_date}, "producto":product, "origen":origin })
+        #return self.collection.find({"fecha":{"$gte":self.start_date,"$lte":self.end_date}})
 
     @property
     def _connection_string(self):
         return "mongodb://{0}:{1}@{2}:{3}".format(self.MONGO_USER, self.MONGO_PASSW, self.MONGO_HOST, self.MONGO_PORT)
```

