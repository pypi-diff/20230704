# Comparing `tmp/vercel_kv-0.1.2.tar.gz` & `tmp/vercel_kv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vercel_kv-0.1.2.tar", last modified: Tue Jul  4 03:03:37 2023, max compression
+gzip compressed data, was "vercel_kv-0.1.3.tar", last modified: Tue Jul  4 03:06:07 2023, max compression
```

## Comparing `vercel_kv-0.1.2.tar` & `vercel_kv-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 03:03:37.180236 vercel_kv-0.1.2/
--rw-rw-rw-   0        0        0     1083 2023-06-30 10:01:11.000000 vercel_kv-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       69 2023-07-03 05:49:13.000000 vercel_kv-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1092 2023-07-04 03:03:37.179235 vercel_kv-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-03 05:18:44.000000 vercel_kv-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 03:03:37.180236 vercel_kv-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-07-04 03:03:30.000000 vercel_kv-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:03:37.146237 vercel_kv-0.1.2/src/
--rw-rw-rw-   0        0        0     2101 2023-06-30 04:22:10.000000 vercel_kv-0.1.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 03:03:37.176259 vercel_kv-0.1.2/src/vercel_kv.egg-info/
--rw-rw-rw-   0        0        0     1092 2023-07-04 03:03:36.000000 vercel_kv-0.1.2/src/vercel_kv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-04 03:03:37.000000 vercel_kv-0.1.2/src/vercel_kv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 03:03:36.000000 vercel_kv-0.1.2/src/vercel_kv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-04 03:03:36.000000 vercel_kv-0.1.2/src/vercel_kv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 03:03:36.000000 vercel_kv-0.1.2/src/vercel_kv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 03:06:07.737156 vercel_kv-0.1.3/
+-rw-rw-rw-   0        0        0     1083 2023-06-30 10:01:11.000000 vercel_kv-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       70 2023-07-04 03:05:41.000000 vercel_kv-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1092 2023-07-04 03:06:07.735156 vercel_kv-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-03 05:18:44.000000 vercel_kv-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 03:06:07.737156 vercel_kv-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-07-04 03:05:51.000000 vercel_kv-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:06:07.718156 vercel_kv-0.1.3/src/
+-rw-rw-rw-   0        0        0     2101 2023-06-30 04:22:10.000000 vercel_kv-0.1.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:06:07.730155 vercel_kv-0.1.3/src/vercel_kv.egg-info/
+-rw-rw-rw-   0        0        0     1092 2023-07-04 03:06:07.000000 vercel_kv-0.1.3/src/vercel_kv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-04 03:06:07.000000 vercel_kv-0.1.3/src/vercel_kv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 03:06:07.000000 vercel_kv-0.1.3/src/vercel_kv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-04 03:06:07.000000 vercel_kv-0.1.3/src/vercel_kv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 03:06:07.000000 vercel_kv-0.1.3/src/vercel_kv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 03:06:07.732154 vercel_kv-0.1.3/tests/
+-rw-rw-rw-   0        0        0      200 2023-06-30 04:04:42.000000 vercel_kv-0.1.3/tests/test.py
```

### Comparing `vercel_kv-0.1.2/LICENSE` & `vercel_kv-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vercel_kv-0.1.2/PKG-INFO` & `vercel_kv-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vercel_kv
-Version: 0.1.2
+Version: 0.1.3
 Summary: https://vercel.com/docs/storage/vercel-kv/rest-api
 Home-page: https://github.com/bestK/python-vercel-kv
 Author: bestk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `vercel_kv-0.1.2/README.md` & `vercel_kv-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vercel_kv-0.1.2/setup.py` & `vercel_kv-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="vercel_kv",
-    version="0.1.2",
+    version="0.1.3",
     description="https://vercel.com/docs/storage/vercel-kv/rest-api",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bestK/python-vercel-kv",
     author="bestk",
     license="MIT",
     classifiers=[
```

### Comparing `vercel_kv-0.1.2/src/__init__.py` & `vercel_kv-0.1.3/src/__init__.py`

 * *Files identical despite different names*

### Comparing `vercel_kv-0.1.2/src/vercel_kv.egg-info/PKG-INFO` & `vercel_kv-0.1.3/src/vercel_kv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vercel-kv
-Version: 0.1.2
+Version: 0.1.3
 Summary: https://vercel.com/docs/storage/vercel-kv/rest-api
 Home-page: https://github.com/bestK/python-vercel-kv
 Author: bestk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

