# Comparing `tmp/aligntext-0.1.0.tar.gz` & `tmp/aligntext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligntext-0.1.0.tar", max compression
+gzip compressed data, was "aligntext-0.1.1.tar", max compression
```

## Comparing `aligntext-0.1.0.tar` & `aligntext-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-07-03 19:22:24.455121 aligntext-0.1.0/LICENSE
--rw-r--r--   0        0        0     1223 2023-07-03 19:22:24.455121 aligntext-0.1.0/README.md
--rw-r--r--   0        0        0    16428 2023-07-03 19:22:24.455121 aligntext-0.1.0/aligntext/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 19:22:24.455121 aligntext-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 aligntext-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 21:48:29.836200 aligntext-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1223 2023-07-04 21:48:29.836200 aligntext-0.1.1/README.md
+-rw-r--r--   0        0        0    16428 2023-07-04 21:48:29.836200 aligntext-0.1.1/aligntext/__init__.py
+-rw-r--r--   0        0        0     2169 2023-07-04 21:48:29.836200 aligntext-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 aligntext-0.1.1/PKG-INFO
```

### Comparing `aligntext-0.1.0/LICENSE` & `aligntext-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aligntext-0.1.0/README.md` & `aligntext-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aligntext-0.1.0/aligntext/__init__.py` & `aligntext-0.1.1/aligntext/__init__.py`

 * *Files identical despite different names*

### Comparing `aligntext-0.1.0/pyproject.toml` & `aligntext-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aligntext"
-version = "0.1.0"
+version = "0.1.1"
 description = "Text Align - Python Text Alignment"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -27,14 +27,15 @@
 python = '^3.7.2'
 
 [tool.poetry.group.test.dependencies]
 black = '^23.3.0'
 coverage = '^6.4.4'
 isort = '^5.9'
 mypy = "^1.3.0"
+nbcpychecker = '^1.0.0'
 pylint = '^2.15'
 pytest = '^7.3'
 
 [tool.poetry.group.doc.dependencies]
 sphinx = '^5.1.1'
 sphinx-rtd-theme = "^1.0.0"
 sphinxemoji = ">=0.2.0"
@@ -102,8 +103,9 @@
     poetry run coverage run --source=aligntext --branch -m pytest --doctest-glob=docs/*.rst --doctest-modules --ignore-glob=tests/testdata* --ignore=docs/conf.py --log-level=DEBUG -vv --junitxml=report.xml
     poetry run coverage report
     poetry run coverage html
     poetry run coverage xml
     poetry run pylint aligntext tests
     poetry run mypy aligntext
     poetry run make html -C docs
+    poetry run nbcpychecker check
 """
```

### Comparing `aligntext-0.1.0/PKG-INFO` & `aligntext-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligntext
-Version: 0.1.0
+Version: 0.1.1
 Summary: Text Align - Python Text Alignment
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

