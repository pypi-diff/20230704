# Comparing `tmp/dnac_device_list-1.0.1.tar.gz` & `tmp/dnac_device_list-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnac_device_list-1.0.1.tar", last modified: Mon Jul  3 16:13:54 2023, max compression
+gzip compressed data, was "dnac_device_list-1.0.2.tar", last modified: Mon Jul  3 16:22:23 2023, max compression
```

## Comparing `dnac_device_list-1.0.1.tar` & `dnac_device_list-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:54.110890 dnac_device_list-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-03 01:16:23.000000 dnac_device_list-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2204 2023-07-03 16:13:54.110890 dnac_device_list-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1712 2023-07-03 16:13:32.000000 dnac_device_list-1.0.1/README.md
--rw-rw-rw-   0        0        0      635 2023-07-03 16:12:57.000000 dnac_device_list-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-03 16:13:54.110890 dnac_device_list-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:54.069214 dnac_device_list-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:54.085607 dnac_device_list-1.0.1/src/dnac_device_list/
--rw-rw-rw-   0        0        0        0 2023-07-03 01:11:50.000000 dnac_device_list-1.0.1/src/dnac_device_list/__init__.py
--rw-rw-rw-   0        0        0     8320 2023-07-03 16:03:58.000000 dnac_device_list-1.0.1/src/dnac_device_list/device_list.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:54.106537 dnac_device_list-1.0.1/src/dnac_device_list.egg-info/
--rw-rw-rw-   0        0        0     2204 2023-07-03 16:13:54.000000 dnac_device_list-1.0.1/src/dnac_device_list.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-03 16:13:54.000000 dnac_device_list-1.0.1/src/dnac_device_list.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 16:13:54.000000 dnac_device_list-1.0.1/src/dnac_device_list.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-03 16:13:54.000000 dnac_device_list-1.0.1/src/dnac_device_list.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 16:13:54.000000 dnac_device_list-1.0.1/src/dnac_device_list.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 16:22:23.177131 dnac_device_list-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-03 01:16:23.000000 dnac_device_list-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3645 2023-07-03 16:22:23.177131 dnac_device_list-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3153 2023-07-03 16:21:50.000000 dnac_device_list-1.0.2/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-03 16:21:50.000000 dnac_device_list-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 16:22:23.184135 dnac_device_list-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 16:22:23.153394 dnac_device_list-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 16:22:23.163496 dnac_device_list-1.0.2/src/dnac_device_list/
+-rw-rw-rw-   0        0        0        0 2023-07-03 01:11:50.000000 dnac_device_list-1.0.2/src/dnac_device_list/__init__.py
+-rw-rw-rw-   0        0        0     8320 2023-07-03 16:03:58.000000 dnac_device_list-1.0.2/src/dnac_device_list/device_list.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:22:23.177131 dnac_device_list-1.0.2/src/dnac_device_list.egg-info/
+-rw-rw-rw-   0        0        0     3645 2023-07-03 16:22:23.000000 dnac_device_list-1.0.2/src/dnac_device_list.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-03 16:22:23.000000 dnac_device_list-1.0.2/src/dnac_device_list.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:22:23.000000 dnac_device_list-1.0.2/src/dnac_device_list.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-03 16:22:23.000000 dnac_device_list-1.0.2/src/dnac_device_list.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-03 16:22:23.000000 dnac_device_list-1.0.2/src/dnac_device_list.egg-info/top_level.txt
```

### Comparing `dnac_device_list-1.0.1/LICENSE` & `dnac_device_list-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dnac_device_list-1.0.1/pyproject.toml` & `dnac_device_list-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnac_device_list"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Alexios Nersessian", email="nersessian@gmail.com" },
 ]
 description = "Get Device list with location details from DNAC."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dnac_device_list-1.0.1/src/dnac_device_list/device_list.py` & `dnac_device_list-1.0.2/src/dnac_device_list/device_list.py`

 * *Files identical despite different names*

