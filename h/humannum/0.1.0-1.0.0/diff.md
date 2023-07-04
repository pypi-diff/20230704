# Comparing `tmp/humannum-0.1.0.tar.gz` & `tmp/humannum-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humannum-0.1.0.tar", max compression
+gzip compressed data, was "humannum-1.0.0.tar", max compression
```

## Comparing `humannum-0.1.0.tar` & `humannum-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-07-03 22:08:01.485535 humannum-0.1.0/LICENSE
--rw-r--r--   0        0        0     1196 2023-07-03 22:08:01.485535 humannum-0.1.0/README.md
--rw-r--r--   0        0        0     4376 2023-07-03 22:08:01.485535 humannum-0.1.0/humannum/__init__.py
--rw-r--r--   0        0        0     2960 2023-07-03 22:08:01.485535 humannum-0.1.0/humannum/baseint.py
--rw-r--r--   0        0        0     3390 2023-07-03 22:08:01.485535 humannum-0.1.0/humannum/binary.py
--rw-r--r--   0        0        0     3344 2023-07-03 22:08:01.485535 humannum-0.1.0/humannum/bytes.py
--rw-r--r--   0        0        0     2840 2023-07-03 22:08:01.485535 humannum-0.1.0/humannum/converter.py
--rw-r--r--   0        0        0     3369 2023-07-03 22:08:01.485535 humannum-0.1.0/humannum/hex.py
--rw-r--r--   0        0        0     2137 2023-07-03 22:08:01.485535 humannum-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 humannum-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-04 21:39:11.187154 humannum-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1196 2023-07-04 21:39:11.187154 humannum-1.0.0/README.md
+-rw-r--r--   0        0        0     4376 2023-07-04 21:39:11.187154 humannum-1.0.0/humannum/__init__.py
+-rw-r--r--   0        0        0     2960 2023-07-04 21:39:11.187154 humannum-1.0.0/humannum/baseint.py
+-rw-r--r--   0        0        0     3390 2023-07-04 21:39:11.187154 humannum-1.0.0/humannum/binary.py
+-rw-r--r--   0        0        0     3344 2023-07-04 21:39:11.187154 humannum-1.0.0/humannum/bytes.py
+-rw-r--r--   0        0        0     2840 2023-07-04 21:39:11.187154 humannum-1.0.0/humannum/converter.py
+-rw-r--r--   0        0        0     3369 2023-07-04 21:39:11.191155 humannum-1.0.0/humannum/hex.py
+-rw-r--r--   0        0        0     2195 2023-07-04 21:39:11.191155 humannum-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 humannum-1.0.0/PKG-INFO
```

### Comparing `humannum-0.1.0/LICENSE` & `humannum-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/README.md` & `humannum-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/humannum/__init__.py` & `humannum-1.0.0/humannum/__init__.py`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/humannum/baseint.py` & `humannum-1.0.0/humannum/baseint.py`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/humannum/binary.py` & `humannum-1.0.0/humannum/binary.py`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/humannum/bytes.py` & `humannum-1.0.0/humannum/bytes.py`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/humannum/converter.py` & `humannum-1.0.0/humannum/converter.py`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/humannum/hex.py` & `humannum-1.0.0/humannum/hex.py`

 * *Files identical despite different names*

### Comparing `humannum-0.1.0/pyproject.toml` & `humannum-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "humannum"
-version = "0.1.0"
+version = "1.0.0"
 description = "Human Friendly Numbers"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -28,14 +28,15 @@
 humanfriendly = "^10.0"
 
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
@@ -104,8 +105,9 @@
     poetry run coverage run --source=humannum --branch -m pytest --doctest-glob=docs/*.rst --doctest-modules --ignore-glob=tests/testdata* --ignore=docs/conf.py --log-level=DEBUG -vv --junitxml=report.xml
     poetry run coverage report
     poetry run coverage html
     poetry run coverage xml
     poetry run pylint humannum tests
     poetry run mypy humannum
     poetry run make html -C docs
+    poetry run nbcpychecker check
 """
```

### Comparing `humannum-0.1.0/PKG-INFO` & `humannum-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humannum
-Version: 0.1.0
+Version: 1.0.0
 Summary: Human Friendly Numbers
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

