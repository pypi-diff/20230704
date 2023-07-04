# Comparing `tmp/kafkaclientveli-1.0.5.tar.gz` & `tmp/kafkaclientveli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaclientveli-1.0.5.tar", last modified: Tue Jul  4 09:25:52 2023, max compression
+gzip compressed data, was "kafkaclientveli-1.0.6.tar", last modified: Tue Jul  4 09:29:07 2023, max compression
```

## Comparing `kafkaclientveli-1.0.5.tar` & `kafkaclientveli-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,20 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:25:52.415900 kafkaclientveli-1.0.5/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 kafkaclientveli-1.0.5/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:25:52.415784 kafkaclientveli-1.0.5/PKG-INFO
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:25:52.413257 kafkaclientveli-1.0.5/kafkaclientveli.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:25:52.000000 kafkaclientveli-1.0.5/kafkaclientveli.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-04 09:25:52.000000 kafkaclientveli-1.0.5/kafkaclientveli.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-04 09:25:52.000000 kafkaclientveli-1.0.5/kafkaclientveli.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-04 09:25:52.000000 kafkaclientveli-1.0.5/kafkaclientveli.egg-info/top_level.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.5/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-04 09:25:52.415930 kafkaclientveli-1.0.5/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-04 09:25:47.000000 kafkaclientveli-1.0.5/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:25:52.414399 kafkaclientveli-1.0.5/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-04 09:18:27.000000 kafkaclientveli-1.0.5/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2044 2023-07-04 08:42:05.000000 kafkaclientveli-1.0.5/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3485 2023-07-04 08:59:05.000000 kafkaclientveli-1.0.5/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:25:52.414925 kafkaclientveli-1.0.5/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.5/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.5/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1940 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.5/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.5/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1298 2023-07-04 09:25:39.000000 kafkaclientveli-1.0.5/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:25:52.415617 kafkaclientveli-1.0.5/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.5/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.5/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1145 2023-07-04 08:42:00.000000 kafkaclientveli-1.0.5/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:29:07.521127 kafkaclientveli-1.0.6/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 kafkaclientveli-1.0.6/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:29:07.520966 kafkaclientveli-1.0.6/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.6/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-04 09:29:07.521167 kafkaclientveli-1.0.6/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      433 2023-07-04 09:28:56.000000 kafkaclientveli-1.0.6/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:29:07.519327 kafkaclientveli-1.0.6/src/
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:29:07.519965 kafkaclientveli-1.0.6/src/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.6/src/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.6/src/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1940 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.6/src/events/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:29:07.520399 kafkaclientveli-1.0.6/src/kafkaclientveli.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:29:07.000000 kafkaclientveli-1.0.6/src/kafkaclientveli.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      340 2023-07-04 09:29:07.000000 kafkaclientveli-1.0.6/src/kafkaclientveli.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-04 09:29:07.000000 kafkaclientveli-1.0.6/src/kafkaclientveli.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       14 2023-07-04 09:29:07.000000 kafkaclientveli-1.0.6/src/kafkaclientveli.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:29:07.520726 kafkaclientveli-1.0.6/src/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.6/src/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.6/src/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1145 2023-07-04 08:42:00.000000 kafkaclientveli-1.0.6/src/topics/triptracker.py
```

### Comparing `kafkaclientveli-1.0.5/PKG-INFO` & `kafkaclientveli-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaclientveli
-Version: 1.0.5
+Version: 1.0.6
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `kafkaclientveli-1.0.5/kafkaclientveli.egg-info/PKG-INFO` & `kafkaclientveli-1.0.6/src/kafkaclientveli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaclientveli
-Version: 1.0.5
+Version: 1.0.6
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `kafkaclientveli-1.0.5/readme.md` & `kafkaclientveli-1.0.6/readme.md`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.5/velikafkaclient/events/triptracker.py` & `kafkaclientveli-1.0.6/src/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.5/velikafkaclient/topics/triptracker.py` & `kafkaclientveli-1.0.6/src/topics/triptracker.py`

 * *Files identical despite different names*

