# Comparing `tmp/aligntext-0.1.1.tar.gz` & `tmp/aligntext-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligntext-0.1.1.tar", max compression
+gzip compressed data, was "aligntext-1.0.0.tar", max compression
```

## Comparing `aligntext-0.1.1.tar` & `aligntext-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-07-04 21:48:29.836200 aligntext-0.1.1/LICENSE
--rw-r--r--   0        0        0     1223 2023-07-04 21:48:29.836200 aligntext-0.1.1/README.md
--rw-r--r--   0        0        0    16428 2023-07-04 21:48:29.836200 aligntext-0.1.1/aligntext/__init__.py
--rw-r--r--   0        0        0     2169 2023-07-04 21:48:29.836200 aligntext-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 aligntext-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 21:51:28.576808 aligntext-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1223 2023-07-04 21:51:28.576808 aligntext-1.0.0/README.md
+-rw-r--r--   0        0        0    16428 2023-07-04 21:51:28.576808 aligntext-1.0.0/aligntext/__init__.py
+-rw-r--r--   0        0        0     2169 2023-07-04 21:51:28.580808 aligntext-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 aligntext-1.0.0/PKG-INFO
```

### Comparing `aligntext-0.1.1/LICENSE` & `aligntext-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligntext-0.1.1/README.md` & `aligntext-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aligntext-0.1.1/aligntext/__init__.py` & `aligntext-1.0.0/aligntext/__init__.py`

 * *Files identical despite different names*

### Comparing `aligntext-0.1.1/pyproject.toml` & `aligntext-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aligntext"
-version = "0.1.1"
+version = "1.0.0"
 description = "Text Align - Python Text Alignment"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `aligntext-0.1.1/PKG-INFO` & `aligntext-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligntext
-Version: 0.1.1
+Version: 1.0.0
 Summary: Text Align - Python Text Alignment
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

