# Comparing `tmp/ass-0.5.3.tar.gz` & `tmp/ass-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ass-0.5.3.tar", last modified: Wed Mar 22 22:56:50 2023, max compression
+gzip compressed data, was "ass-0.5.4.tar", last modified: Tue Jul  4 00:41:52 2023, max compression
```

## Comparing `ass-0.5.3.tar` & `ass-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-03-22 22:56:50.232633 ass-0.5.3/
--rw-r--r--   0 fichte    (1000) users      (100)     1169 2020-02-24 16:45:29.000000 ass-0.5.3/LICENSE
--rw-r--r--   0 fichte    (1000) users      (100)       57 2019-01-26 00:23:54.000000 ass-0.5.3/MANIFEST.in
--rw-r--r--   0 fichte    (1000) users      (100)     4453 2023-03-22 22:56:50.232633 ass-0.5.3/PKG-INFO
--rw-r--r--   0 fichte    (1000) users      (100)     3806 2020-02-24 16:40:47.000000 ass-0.5.3/README.md
-drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-03-22 22:56:50.232633 ass-0.5.3/ass/
--rw-r--r--   0 fichte    (1000) users      (100)      382 2021-03-29 11:49:55.000000 ass-0.5.3/ass/__init__.py
--rw-r--r--   0 fichte    (1000) users      (100)     1314 2020-02-24 16:40:47.000000 ass-0.5.3/ass/_util.py
--rw-r--r--   0 fichte    (1000) users      (100)     5600 2021-03-29 11:49:53.000000 ass-0.5.3/ass/data.py
--rw-r--r--   0 fichte    (1000) users      (100)     5092 2023-03-22 22:52:09.000000 ass-0.5.3/ass/document.py
--rw-r--r--   0 fichte    (1000) users      (100)     6144 2020-02-24 16:40:47.000000 ass-0.5.3/ass/line.py
--rw-r--r--   0 fichte    (1000) users      (100)    15546 2023-03-22 22:52:09.000000 ass-0.5.3/ass/renderer.py
--rw-r--r--   0 fichte    (1000) users      (100)     4497 2020-03-02 18:06:32.000000 ass-0.5.3/ass/section.py
-drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-03-22 22:56:50.232633 ass-0.5.3/ass.egg-info/
--rw-r--r--   0 fichte    (1000) users      (100)     4453 2023-03-22 22:56:50.000000 ass-0.5.3/ass.egg-info/PKG-INFO
--rw-r--r--   0 fichte    (1000) users      (100)      312 2023-03-22 22:56:50.000000 ass-0.5.3/ass.egg-info/SOURCES.txt
--rw-r--r--   0 fichte    (1000) users      (100)        1 2023-03-22 22:56:50.000000 ass-0.5.3/ass.egg-info/dependency_links.txt
--rw-r--r--   0 fichte    (1000) users      (100)       11 2023-03-22 22:56:50.000000 ass-0.5.3/ass.egg-info/requires.txt
--rw-r--r--   0 fichte    (1000) users      (100)        4 2023-03-22 22:56:50.000000 ass-0.5.3/ass.egg-info/top_level.txt
--rw-r--r--   0 fichte    (1000) users      (100)        1 2019-01-26 00:28:35.000000 ass-0.5.3/ass.egg-info/zip-safe
--rw-r--r--   0 fichte    (1000) users      (100)       38 2023-03-22 22:56:50.232633 ass-0.5.3/setup.cfg
--rw-r--r--   0 fichte    (1000) users      (100)      945 2023-03-22 22:56:46.000000 ass-0.5.3/setup.py
-drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-03-22 22:56:50.232633 ass-0.5.3/tests/
--rwxr-xr-x   0 fichte    (1000) users      (100)     3534 2023-03-22 22:52:09.000000 ass-0.5.3/tests/test_ass.py
+drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-07-04 00:41:52.974607 ass-0.5.4/
+-rw-r--r--   0 fichte    (1000) users      (100)     1169 2020-02-24 16:45:29.000000 ass-0.5.4/LICENSE
+-rw-r--r--   0 fichte    (1000) users      (100)       57 2019-01-26 00:23:54.000000 ass-0.5.4/MANIFEST.in
+-rw-r--r--   0 fichte    (1000) users      (100)     4453 2023-07-04 00:41:52.974607 ass-0.5.4/PKG-INFO
+-rw-r--r--   0 fichte    (1000) users      (100)     3806 2020-02-24 16:40:47.000000 ass-0.5.4/README.md
+drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-07-04 00:41:52.974607 ass-0.5.4/ass/
+-rw-r--r--   0 fichte    (1000) users      (100)      382 2021-03-29 11:49:55.000000 ass-0.5.4/ass/__init__.py
+-rw-r--r--   0 fichte    (1000) users      (100)     1314 2020-02-24 16:40:47.000000 ass-0.5.4/ass/_util.py
+-rw-r--r--   0 fichte    (1000) users      (100)     4331 2023-07-04 00:23:51.000000 ass-0.5.4/ass/data.py
+-rw-r--r--   0 fichte    (1000) users      (100)     5092 2023-03-22 22:52:09.000000 ass-0.5.4/ass/document.py
+-rw-r--r--   0 fichte    (1000) users      (100)     4914 2023-07-04 00:23:58.000000 ass-0.5.4/ass/line.py
+-rw-r--r--   0 fichte    (1000) users      (100)    15546 2023-03-22 22:52:09.000000 ass-0.5.4/ass/renderer.py
+-rw-r--r--   0 fichte    (1000) users      (100)     4497 2020-03-02 18:06:32.000000 ass-0.5.4/ass/section.py
+drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-07-04 00:41:52.974607 ass-0.5.4/ass.egg-info/
+-rw-r--r--   0 fichte    (1000) users      (100)     4453 2023-07-04 00:41:52.000000 ass-0.5.4/ass.egg-info/PKG-INFO
+-rw-r--r--   0 fichte    (1000) users      (100)      312 2023-07-04 00:41:52.000000 ass-0.5.4/ass.egg-info/SOURCES.txt
+-rw-r--r--   0 fichte    (1000) users      (100)        1 2023-07-04 00:41:52.000000 ass-0.5.4/ass.egg-info/dependency_links.txt
+-rw-r--r--   0 fichte    (1000) users      (100)       11 2023-07-04 00:41:52.000000 ass-0.5.4/ass.egg-info/requires.txt
+-rw-r--r--   0 fichte    (1000) users      (100)        4 2023-07-04 00:41:52.000000 ass-0.5.4/ass.egg-info/top_level.txt
+-rw-r--r--   0 fichte    (1000) users      (100)        1 2019-01-26 00:28:35.000000 ass-0.5.4/ass.egg-info/zip-safe
+-rw-r--r--   0 fichte    (1000) users      (100)       38 2023-07-04 00:41:52.974607 ass-0.5.4/setup.cfg
+-rw-r--r--   0 fichte    (1000) users      (100)      945 2023-07-04 00:39:57.000000 ass-0.5.4/setup.py
+drwxr-xr-x   0 fichte    (1000) users      (100)        0 2023-07-04 00:41:52.974607 ass-0.5.4/tests/
+-rwxr-xr-x   0 fichte    (1000) users      (100)     3534 2023-03-22 22:52:09.000000 ass-0.5.4/tests/test_ass.py
```

### Comparing `ass-0.5.3/LICENSE` & `ass-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ass-0.5.3/PKG-INFO` & `ass-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ass
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library for parsing and manipulating Advanced SubStation Alpha subtitle files.
 Home-page: http://github.com/chireiden/python-ass
 Author: Tony Young
 License: MIT
 Keywords: ass subtitle substation alpha
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ass-0.5.3/README.md` & `ass-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ass-0.5.3/ass/_util.py` & `ass-0.5.4/ass/_util.py`

 * *Files identical despite different names*

### Comparing `ass-0.5.3/ass/document.py` & `ass-0.5.4/ass/document.py`

 * *Files identical despite different names*

### Comparing `ass-0.5.3/ass/renderer.py` & `ass-0.5.4/ass/renderer.py`

 * *Files identical despite different names*

### Comparing `ass-0.5.3/ass/section.py` & `ass-0.5.4/ass/section.py`

 * *Files identical despite different names*

### Comparing `ass-0.5.3/ass.egg-info/PKG-INFO` & `ass-0.5.4/ass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ass
-Version: 0.5.3
+Version: 0.5.4
 Summary: A library for parsing and manipulating Advanced SubStation Alpha subtitle files.
 Home-page: http://github.com/chireiden/python-ass
 Author: Tony Young
 License: MIT
 Keywords: ass subtitle substation alpha
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ass-0.5.3/setup.py` & `ass-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='ass',
-    version="0.5.3",
+    version="0.5.4",
     description="A library for parsing and manipulating Advanced SubStation Alpha subtitle files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Tony Young",
     # author_email="fichtefoll2@googlemail.com",
     keywords="ass subtitle substation alpha",
     packages=['ass'],
```

### Comparing `ass-0.5.3/tests/test_ass.py` & `ass-0.5.4/tests/test_ass.py`

 * *Files identical despite different names*

