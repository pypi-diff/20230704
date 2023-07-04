# Comparing `tmp/inspectorgadget-1.0.0.tar.gz` & `tmp/inspectorgadget-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspectorgadget-1.0.0.tar", max compression
+gzip compressed data, was "inspectorgadget-1.0.1.tar", max compression
```

## Comparing `inspectorgadget-1.0.0.tar` & `inspectorgadget-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/LICENSE
--rw-r--r--   0        0        0     1324 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/README.md
--rw-r--r--   0        0        0     4843 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/inspectorgadget/__init__.py
--rw-r--r--   0        0        0     2170 2023-07-03 06:58:58.655639 inspectorgadget-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 inspectorgadget-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 21:39:54.885483 inspectorgadget-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1324 2023-07-04 21:39:54.885483 inspectorgadget-1.0.1/README.md
+-rw-r--r--   0        0        0     4843 2023-07-04 21:39:54.885483 inspectorgadget-1.0.1/inspectorgadget/__init__.py
+-rw-r--r--   0        0        0     2228 2023-07-04 21:39:54.885483 inspectorgadget-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 inspectorgadget-1.0.1/PKG-INFO
```

### Comparing `inspectorgadget-1.0.0/LICENSE` & `inspectorgadget-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inspectorgadget-1.0.0/README.md` & `inspectorgadget-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `inspectorgadget-1.0.0/inspectorgadget/__init__.py` & `inspectorgadget-1.0.1/inspectorgadget/__init__.py`

 * *Files identical despite different names*

### Comparing `inspectorgadget-1.0.0/pyproject.toml` & `inspectorgadget-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inspectorgadget"
-version = "1.0.0"
+version = "1.0.1"
 description = "Inspector Gadget - Extended Python Inspection"
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
     poetry run coverage run --source=inspectorgadget --branch -m pytest --doctest-glob=docs/*.rst --doctest-modules --ignore-glob=tests/testdata* --ignore=docs/conf.py --log-level=DEBUG -vv --junitxml=report.xml
     poetry run coverage report
     poetry run coverage html
     poetry run coverage xml
     poetry run pylint inspectorgadget tests
     poetry run mypy inspectorgadget
     poetry run make html -C docs
+    poetry run nbcpychecker check
 """
```

### Comparing `inspectorgadget-1.0.0/PKG-INFO` & `inspectorgadget-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectorgadget
-Version: 1.0.0
+Version: 1.0.1
 Summary: Inspector Gadget - Extended Python Inspection
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

