# Comparing `tmp/bohrium-sdk-0.3.0.tar.gz` & `tmp/bohrium-sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.3.0.tar", last modified: Tue Jul  4 08:46:59 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.3.1.tar", last modified: Tue Jul  4 09:43:31 2023, max compression
```

## Comparing `bohrium-sdk-0.3.0.tar` & `bohrium-sdk-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.495921 bohrium-sdk-0.3.0/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 08:46:59.495668 bohrium-sdk-0.3.0/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.490716 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-07-04 08:46:59.000000 bohrium-sdk-0.3.0/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.494688 bohrium-sdk-0.3.0/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     7031 2023-07-04 03:12:10.000000 bohrium-sdk-0.3.0/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/database.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4121 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     8428 2023-07-04 03:26:27.000000 bohrium-sdk-0.3.0/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 08:46:59.495379 bohrium-sdk-0.3.0/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4649 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.0/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-07-04 08:46:59.495970 bohrium-sdk-0.3.0/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-07-04 08:46:38.000000 bohrium-sdk-0.3.0/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:43:31.724447 bohrium-sdk-0.3.1/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 09:43:31.723765 bohrium-sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:43:31.716284 bohrium-sdk-0.3.1/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 09:43:31.000000 bohrium-sdk-0.3.1/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      478 2023-07-04 09:43:31.000000 bohrium-sdk-0.3.1/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-07-04 09:43:31.000000 bohrium-sdk-0.3.1/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       28 2023-07-04 09:43:31.000000 bohrium-sdk-0.3.1/bohrium_sdk.egg-info/requires.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-07-04 09:43:31.000000 bohrium-sdk-0.3.1/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:43:31.722161 bohrium-sdk-0.3.1/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     7031 2023-07-04 03:12:10.000000 bohrium-sdk-0.3.1/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/database.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4121 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     8428 2023-07-04 03:26:27.000000 bohrium-sdk-0.3.1/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:43:31.722908 bohrium-sdk-0.3.1/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4649 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.1/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-07-04 09:43:31.724636 bohrium-sdk-0.3.1/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      420 2023-07-04 09:43:19.000000 bohrium-sdk-0.3.1/setup.py
```

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/client.py` & `bohrium-sdk-0.3.1/bohriumsdk/client.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/database.py` & `bohrium-sdk-0.3.1/bohriumsdk/database.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/image.py` & `bohrium-sdk-0.3.1/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/job.py` & `bohrium-sdk-0.3.1/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/node.py` & `bohrium-sdk-0.3.1/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/project.py` & `bohrium-sdk-0.3.1/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/storage.py` & `bohrium-sdk-0.3.1/bohriumsdk/storage.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/test.py` & `bohrium-sdk-0.3.1/bohriumsdk/test.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.0/bohriumsdk/util.py` & `bohrium-sdk-0.3.1/bohriumsdk/util.py`

 * *Files identical despite different names*

