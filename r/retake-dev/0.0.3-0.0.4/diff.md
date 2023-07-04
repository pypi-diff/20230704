# Comparing `tmp/retake_dev-0.0.3.tar.gz` & `tmp/retake_dev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake_dev-0.0.3.tar", last modified: Tue Jul  4 18:28:17 2023, max compression
+gzip compressed data, was "retake_dev-0.0.4.tar", last modified: Tue Jul  4 18:34:28 2023, max compression
```

## Comparing `retake_dev-0.0.3.tar` & `retake_dev-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,26 @@
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:28:17.959514 retake_dev-0.0.3/
--rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:28:17.959372 retake_dev-0.0.3/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)     1454 2023-07-03 18:27:36.000000 retake_dev-0.0.3/README.md
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:28:17.958549 retake_dev-0.0.3/interface/
--rw-r--r--   0 mingying   (501) staff       (20)      214 2023-07-03 18:27:13.000000 retake_dev-0.0.3/interface/__init__.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:28:17.959217 retake_dev-0.0.3/retake_dev.egg-info/
--rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)      200 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/SOURCES.txt
--rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/dependency_links.txt
--rw-r--r--   0 mingying   (501) staff       (20)       32 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/requires.txt
--rw-r--r--   0 mingying   (501) staff       (20)       11 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/top_level.txt
--rw-r--r--   0 mingying   (501) staff       (20)       38 2023-07-04 18:28:17.959579 retake_dev-0.0.3/setup.cfg
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.320221 retake_dev-0.0.4/
+-rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:34:28.320106 retake_dev-0.0.4/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)     1454 2023-07-03 18:27:36.000000 retake_dev-0.0.4/README.md
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.317884 retake_dev-0.0.4/cdc/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:36.000000 retake_dev-0.0.4/cdc/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3052 2023-07-04 17:10:36.000000 retake_dev-0.0.4/cdc/consumer_postgres.py
+-rw-r--r--   0 mingying   (501) staff       (20)    16136 2023-07-03 18:27:36.000000 retake_dev-0.0.4/cdc/pgoutput.py
+-rw-r--r--   0 mingying   (501) staff       (20)      691 2023-07-04 17:12:53.000000 retake_dev-0.0.4/cdc/run.py
+-rw-r--r--   0 mingying   (501) staff       (20)     3872 2023-07-04 17:12:53.000000 retake_dev-0.0.4/cdc/source_postgres.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.318873 retake_dev-0.0.4/client/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:13.000000 retake_dev-0.0.4/client/__init__.py
+-rw-r--r--   0 mingying   (501) staff       (20)     1914 2023-07-04 18:10:57.000000 retake_dev-0.0.4/client/collection.py
+-rw-r--r--   0 mingying   (501) staff       (20)      235 2023-07-03 18:27:13.000000 retake_dev-0.0.4/client/embedding.py
+-rw-r--r--   0 mingying   (501) staff       (20)      384 2023-07-03 18:27:13.000000 retake_dev-0.0.4/client/source.py
+-rw-r--r--   0 mingying   (501) staff       (20)      752 2023-07-04 18:01:08.000000 retake_dev-0.0.4/client/transform.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.319085 retake_dev-0.0.4/core/
+-rw-r--r--   0 mingying   (501) staff       (20)        0 2023-07-03 18:27:36.000000 retake_dev-0.0.4/core/__init__.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.319178 retake_dev-0.0.4/interface/
+-rw-r--r--   0 mingying   (501) staff       (20)      214 2023-07-03 18:27:13.000000 retake_dev-0.0.4/interface/__init__.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:34:28.319917 retake_dev-0.0.4/retake_dev.egg-info/
+-rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)      405 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       32 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/requires.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       26 2023-07-04 18:34:28.000000 retake_dev-0.0.4/retake_dev.egg-info/top_level.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       38 2023-07-04 18:34:28.320259 retake_dev-0.0.4/setup.cfg
```

### Comparing `retake_dev-0.0.3/README.md` & `retake_dev-0.0.4/README.md`

 * *Files identical despite different names*

