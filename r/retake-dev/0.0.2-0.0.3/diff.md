# Comparing `tmp/retake_dev-0.0.2.tar.gz` & `tmp/retake_dev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake_dev-0.0.2.tar", last modified: Tue Jul  4 17:25:36 2023, max compression
+gzip compressed data, was "retake_dev-0.0.3.tar", last modified: Tue Jul  4 18:28:17 2023, max compression
```

## Comparing `retake_dev-0.0.2.tar` & `retake_dev-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 17:25:36.596552 retake_dev-0.0.2/
--rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 17:25:36.596441 retake_dev-0.0.2/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)      527 2023-07-04 17:23:27.000000 retake_dev-0.0.2/build.py
-drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 17:25:36.596271 retake_dev-0.0.2/retake_dev.egg-info/
--rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 17:25:36.000000 retake_dev-0.0.2/retake_dev.egg-info/PKG-INFO
--rw-r--r--   0 mingying   (501) staff       (20)      202 2023-07-04 17:25:36.000000 retake_dev-0.0.2/retake_dev.egg-info/SOURCES.txt
--rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-04 17:25:36.000000 retake_dev-0.0.2/retake_dev.egg-info/dependency_links.txt
--rw-r--r--   0 mingying   (501) staff       (20)       37 2023-07-04 17:25:36.000000 retake_dev-0.0.2/retake_dev.egg-info/requires.txt
--rw-r--r--   0 mingying   (501) staff       (20)       11 2023-07-04 17:25:36.000000 retake_dev-0.0.2/retake_dev.egg-info/top_level.txt
--rw-r--r--   0 mingying   (501) staff       (20)       38 2023-07-04 17:25:36.596586 retake_dev-0.0.2/setup.cfg
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:28:17.959514 retake_dev-0.0.3/
+-rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:28:17.959372 retake_dev-0.0.3/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)     1454 2023-07-03 18:27:36.000000 retake_dev-0.0.3/README.md
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:28:17.958549 retake_dev-0.0.3/interface/
+-rw-r--r--   0 mingying   (501) staff       (20)      214 2023-07-03 18:27:13.000000 retake_dev-0.0.3/interface/__init__.py
+drwxr-xr-x   0 mingying   (501) staff       (20)        0 2023-07-04 18:28:17.959217 retake_dev-0.0.3/retake_dev.egg-info/
+-rw-r--r--   0 mingying   (501) staff       (20)       54 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/PKG-INFO
+-rw-r--r--   0 mingying   (501) staff       (20)      200 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 mingying   (501) staff       (20)        1 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       32 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/requires.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       11 2023-07-04 18:28:17.000000 retake_dev-0.0.3/retake_dev.egg-info/top_level.txt
+-rw-r--r--   0 mingying   (501) staff       (20)       38 2023-07-04 18:28:17.959579 retake_dev-0.0.3/setup.cfg
```

