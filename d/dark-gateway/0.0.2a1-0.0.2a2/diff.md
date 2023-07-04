# Comparing `tmp/dark-gateway-0.0.2a1.tar.gz` & `tmp/dark-gateway-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark-gateway-0.0.2a1.tar", last modified: Tue Jul  4 18:24:19 2023, max compression
+gzip compressed data, was "dark-gateway-0.0.2a2.tar", last modified: Tue Jul  4 18:24:42 2023, max compression
```

## Comparing `dark-gateway-0.0.2a1.tar` & `dark-gateway-0.0.2a2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:19.350962 dark-gateway-0.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 18:24:19.350962 dark-gateway-0.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:19.350962 dark-gateway-0.0.2a1/dark/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/dark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:19.350962 dark-gateway-0.0.2a1/dark/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/dark/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/dark/gateway/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:19.350962 dark-gateway-0.0.2a1/dark/gateway/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/dark/gateway/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/dark/gateway/util/libs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-04 18:24:16.000000 dark-gateway-0.0.2a1/dark/gateway/util/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:19.350962 dark-gateway-0.0.2a1/dark_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 18:24:19.000000 dark-gateway-0.0.2a1/dark_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-04 18:24:19.000000 dark-gateway-0.0.2a1/dark_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:24:19.000000 dark-gateway-0.0.2a1/dark_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 18:24:19.000000 dark-gateway-0.0.2a1/dark_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:24:19.350962 dark-gateway-0.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-04 18:24:18.000000 dark-gateway-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:42.556662 dark-gateway-0.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 18:24:42.556662 dark-gateway-0.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:42.556662 dark-gateway-0.0.2a2/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:42.556662 dark-gateway-0.0.2a2/dark/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/gateway/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:42.556662 dark-gateway-0.0.2a2/dark/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/util/core_bc_libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/util/libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-04 18:24:37.000000 dark-gateway-0.0.2a2/dark/util/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 18:24:42.556662 dark-gateway-0.0.2a2/dark_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 18:24:42.000000 dark-gateway-0.0.2a2/dark_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-04 18:24:42.000000 dark-gateway-0.0.2a2/dark_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 18:24:42.000000 dark-gateway-0.0.2a2/dark_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 18:24:42.000000 dark-gateway-0.0.2a2/dark_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 18:24:42.556662 dark-gateway-0.0.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-04 18:24:41.000000 dark-gateway-0.0.2a2/setup.py
```

### Comparing `dark-gateway-0.0.2a1/LICENSE` & `dark-gateway-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.2a1/dark/gateway/util/libs.py` & `dark-gateway-0.0.2a2/dark/util/libs.py`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.2a1/dark/gateway/util/setup.py` & `dark-gateway-0.0.2a2/dark/util/setup.py`

 * *Files identical despite different names*

### Comparing `dark-gateway-0.0.2a1/setup.py` & `dark-gateway-0.0.2a2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 local = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(local, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
 # This gets deployed when a new release is made by github actions
-VERSION = '0.0.2a1'
+VERSION = '0.0.2a2'
 # VERSION = '0.0.1'
 
 # CHANGEME VARS
 PACKAGE_NAME = "dark-gateway"
 DESCRIPTION = 'dARK Gateway libs'
 LONG_DESCRIPTION = 'dARK web3 libs to connect applications to the dARK'
 AUTHOR_NAME = "Thiago Nóbrega"
```

