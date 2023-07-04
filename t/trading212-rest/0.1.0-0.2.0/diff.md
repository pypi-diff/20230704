# Comparing `tmp/trading212-rest-0.1.0.tar.gz` & `tmp/trading212-rest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading212-rest-0.1.0.tar", last modified: Thu Jun 22 22:58:48 2023, max compression
+gzip compressed data, was "trading212-rest-0.2.0.tar", last modified: Tue Jul  4 10:56:29 2023, max compression
```

## Comparing `trading212-rest-0.1.0.tar` & `trading212-rest-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-06-22 22:58:48.483047 trading212-rest-0.1.0/
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)    11347 2023-06-22 22:49:31.000000 trading212-rest-0.1.0/LICENSE
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      262 2023-06-22 22:58:48.483047 trading212-rest-0.1.0/PKG-INFO
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      366 2023-06-22 22:58:23.000000 trading212-rest-0.1.0/pyproject.toml
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)       38 2023-06-22 22:58:48.483047 trading212-rest-0.1.0/setup.cfg
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-06-22 22:58:48.483047 trading212-rest-0.1.0/trading212_rest/
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)     1751 2023-06-22 22:32:52.000000 trading212-rest-0.1.0/trading212_rest/__init__.py
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-06-22 22:58:48.483047 trading212-rest-0.1.0/trading212_rest.egg-info/
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      262 2023-06-22 22:58:48.000000 trading212-rest-0.1.0/trading212_rest.egg-info/PKG-INFO
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      244 2023-06-22 22:58:48.000000 trading212-rest-0.1.0/trading212_rest.egg-info/SOURCES.txt
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)        1 2023-06-22 22:58:48.000000 trading212-rest-0.1.0/trading212_rest.egg-info/dependency_links.txt
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)        9 2023-06-22 22:58:48.000000 trading212-rest-0.1.0/trading212_rest.egg-info/requires.txt
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)       21 2023-06-22 22:58:48.000000 trading212-rest-0.1.0/trading212_rest.egg-info/top_level.txt
+drwxr-xr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-07-04 10:56:29.030229 trading212-rest-0.2.0/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)    11347 2023-07-03 23:04:21.000000 trading212-rest-0.2.0/LICENSE
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      262 2023-07-04 10:56:29.030229 trading212-rest-0.2.0/PKG-INFO
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      366 2023-07-03 23:11:13.000000 trading212-rest-0.2.0/pyproject.toml
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)       38 2023-07-04 10:56:29.030229 trading212-rest-0.2.0/setup.cfg
+drwxr-xr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-07-04 10:56:29.026895 trading212-rest-0.2.0/trading212_rest/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)     2569 2023-07-03 23:23:08.000000 trading212-rest-0.2.0/trading212_rest/__init__.py
+drwxr-xr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-07-04 10:56:29.030229 trading212-rest-0.2.0/trading212_rest.egg-info/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      262 2023-07-04 10:56:29.000000 trading212-rest-0.2.0/trading212_rest.egg-info/PKG-INFO
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      244 2023-07-04 10:56:29.000000 trading212-rest-0.2.0/trading212_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        1 2023-07-04 10:56:29.000000 trading212-rest-0.2.0/trading212_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)        9 2023-07-04 10:56:29.000000 trading212-rest-0.2.0/trading212_rest.egg-info/requires.txt
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)       21 2023-07-04 10:56:29.000000 trading212-rest-0.2.0/trading212_rest.egg-info/top_level.txt
```

### Comparing `trading212-rest-0.1.0/LICENSE` & `trading212-rest-0.2.0/LICENSE`

 * *Files identical despite different names*

