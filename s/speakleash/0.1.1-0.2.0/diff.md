# Comparing `tmp/speakleash-0.1.1.tar.gz` & `tmp/speakleash-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakleash-0.1.1.tar", last modified: Fri Jun  9 19:59:57 2023, max compression
+gzip compressed data, was "speakleash-0.2.0.tar", last modified: Tue Jul  4 18:34:08 2023, max compression
```

## Comparing `speakleash-0.1.1.tar` & `speakleash-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:59:57.196217 speakleash-0.1.1/
--rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.1.1/LICENSE
--rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-06-09 19:59:57.195922 speakleash-0.1.1/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)     1995 2023-06-09 19:57:52.000000 speakleash-0.1.1/README.md
--rw-r--r--   0 skondracki   (502) staff       (20)       38 2023-06-09 19:59:57.196313 speakleash-0.1.1/setup.cfg
--rw-r--r--   0 skondracki   (502) staff       (20)      571 2023-06-09 19:59:30.000000 speakleash-0.1.1/setup.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:59:57.193348 speakleash-0.1.1/speakleash/
--rw-r--r--   0 skondracki   (502) staff       (20)     6586 2023-06-09 19:27:17.000000 speakleash-0.1.1/speakleash/__init__.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-06-09 19:59:57.195537 speakleash-0.1.1/speakleash.egg-info/
--rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)      218 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/SOURCES.txt
--rw-r--r--   0 skondracki   (502) staff       (20)        1 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/dependency_links.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       28 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/requires.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       11 2023-06-09 19:59:57.000000 speakleash-0.1.1/speakleash.egg-info/top_level.txt
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-04 18:34:08.592823 speakleash-0.2.0/
+-rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.2.0/LICENSE
+-rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-07-04 18:34:08.592534 speakleash-0.2.0/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)     1995 2023-06-09 19:57:52.000000 speakleash-0.2.0/README.md
+-rw-r--r--   0 skondracki   (502) staff       (20)       38 2023-07-04 18:34:08.592919 speakleash-0.2.0/setup.cfg
+-rw-r--r--   0 skondracki   (502) staff       (20)      571 2023-07-04 18:33:01.000000 speakleash-0.2.0/setup.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-04 18:34:08.590305 speakleash-0.2.0/speakleash/
+-rw-r--r--   0 skondracki   (502) staff       (20)    10148 2023-07-04 18:22:29.000000 speakleash-0.2.0/speakleash/__init__.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2023-07-04 18:34:08.592143 speakleash-0.2.0/speakleash.egg-info/
+-rw-r--r--   0 skondracki   (502) staff       (20)     2294 2023-07-04 18:34:08.000000 speakleash-0.2.0/speakleash.egg-info/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)      218 2023-07-04 18:34:08.000000 speakleash-0.2.0/speakleash.egg-info/SOURCES.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)        1 2023-07-04 18:34:08.000000 speakleash-0.2.0/speakleash.egg-info/dependency_links.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       28 2023-07-04 18:34:08.000000 speakleash-0.2.0/speakleash.egg-info/requires.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       11 2023-07-04 18:34:08.000000 speakleash-0.2.0/speakleash.egg-info/top_level.txt
```

### Comparing `speakleash-0.1.1/LICENSE` & `speakleash-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speakleash-0.1.1/PKG-INFO` & `speakleash-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.1.1
+Version: 0.2.0
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `speakleash-0.1.1/README.md` & `speakleash-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `speakleash-0.1.1/setup.py` & `speakleash-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="speakleash",
-    version="0.1.1",
+    version="0.2.0",
     author="SpeakLeash Team",
     author_email="team@speakleash.org",
     description="SpeakLeash agnostic dataset for Polish",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/speakleash/speakleash",
     packages = ["speakleash"],
```

### Comparing `speakleash-0.1.1/speakleash.egg-info/PKG-INFO` & `speakleash-0.2.0/speakleash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.1.1
+Version: 0.2.0
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

