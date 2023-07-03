# Comparing `tmp/testpoetry2-0.1.8.tar.gz` & `tmp/testpoetry2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpoetry2-0.1.8.tar", max compression
+gzip compressed data, was "testpoetry2-0.1.9.tar", max compression
```

## Comparing `testpoetry2-0.1.8.tar` & `testpoetry2-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      461 2023-07-03 11:10:22.662391 testpoetry2-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1438 2023-07-02 13:58:42.684298 testpoetry2-0.1.8/README.md
--rw-r--r--   0        0        0      269 2023-07-02 21:10:54.783989 testpoetry2-0.1.8/testpoetry2/__init__.py
--rw-r--r--   0        0        0      118 2023-07-02 15:03:07.864639 testpoetry2-0.1.8/testpoetry2/__main__.py
--rw-r--r--   0        0        0       23 2023-07-03 11:10:22.656400 testpoetry2-0.1.8/testpoetry2/__version__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:53:06.262853 testpoetry2-0.1.8/testpoetry2/console/__init__.py
--rw-r--r--   0        0        0     4475 2023-07-02 21:10:54.804990 testpoetry2-0.1.8/testpoetry2/console/application.py
--rw-r--r--   0        0        0     7732 2023-07-02 21:10:54.792991 testpoetry2-0.1.8/testpoetry2/pwgen.py
--rw-r--r--   0        0        0    16199 2023-06-30 15:27:00.145251 testpoetry2-0.1.8/testpoetry2/test-pwgen.py
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 testpoetry2-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      463 2023-07-03 11:17:41.126054 testpoetry2-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1438 2023-07-02 13:58:42.684298 testpoetry2-0.1.9/README.md
+-rw-r--r--   0        0        0      269 2023-07-02 21:10:54.783989 testpoetry2-0.1.9/testpoetry2/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-02 15:03:07.864639 testpoetry2-0.1.9/testpoetry2/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-03 11:17:41.121071 testpoetry2-0.1.9/testpoetry2/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:53:06.262853 testpoetry2-0.1.9/testpoetry2/console/__init__.py
+-rw-r--r--   0        0        0     4475 2023-07-02 21:10:54.804990 testpoetry2-0.1.9/testpoetry2/console/application.py
+-rw-r--r--   0        0        0     7732 2023-07-02 21:10:54.792991 testpoetry2-0.1.9/testpoetry2/pwgen.py
+-rw-r--r--   0        0        0    16199 2023-06-30 15:27:00.145251 testpoetry2-0.1.9/testpoetry2/test-pwgen.py
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 testpoetry2-0.1.9/PKG-INFO
```

### Comparing `testpoetry2-0.1.8/README.md` & `testpoetry2-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `testpoetry2-0.1.8/testpoetry2/console/application.py` & `testpoetry2-0.1.9/testpoetry2/console/application.py`

 * *Files identical despite different names*

### Comparing `testpoetry2-0.1.8/testpoetry2/pwgen.py` & `testpoetry2-0.1.9/testpoetry2/pwgen.py`

 * *Files identical despite different names*

### Comparing `testpoetry2-0.1.8/testpoetry2/test-pwgen.py` & `testpoetry2-0.1.9/testpoetry2/test-pwgen.py`

 * *Files identical despite different names*

### Comparing `testpoetry2-0.1.8/PKG-INFO` & `testpoetry2-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpoetry2
-Version: 0.1.8
+Version: 0.1.9
 Summary: Password generator CLI and library
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

