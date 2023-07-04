# Comparing `tmp/calculator_beau28713-0.1.1.tar.gz` & `tmp/calculator_beau28713-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculator_beau28713-0.1.1.tar", max compression
+gzip compressed data, was "calculator_beau28713-0.1.2.tar", max compression
```

## Comparing `calculator_beau28713-0.1.1.tar` & `calculator_beau28713-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-04 16:38:45.167898 calculator_beau28713-0.1.1/calculator_beau28713/__init__.py
--rw-r--r--   0        0        0     3400 2023-07-04 16:38:45.168435 calculator_beau28713-0.1.1/calculator_beau28713/__main__.py
--rw-r--r--   0        0        0     1088 2023-07-04 16:38:45.166441 calculator_beau28713-0.1.1/LICENSE
--rw-r--r--   0        0        0      392 2023-07-04 17:11:07.940898 calculator_beau28713-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      434 2023-07-04 16:38:45.166441 calculator_beau28713-0.1.1/README.md
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 calculator_beau28713-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 16:38:45.167898 calculator_beau28713-0.1.2/calculator_beau28713/__init__.py
+-rw-r--r--   0        0        0     3400 2023-07-04 16:38:45.168435 calculator_beau28713-0.1.2/calculator_beau28713/__main__.py
+-rw-r--r--   0        0        0     1088 2023-07-04 16:38:45.166441 calculator_beau28713-0.1.2/LICENSE
+-rw-r--r--   0        0        0      393 2023-07-04 19:52:46.051336 calculator_beau28713-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      434 2023-07-04 16:38:45.166441 calculator_beau28713-0.1.2/README.md
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 calculator_beau28713-0.1.2/PKG-INFO
```

### Comparing `calculator_beau28713-0.1.1/calculator_beau28713/__main__.py` & `calculator_beau28713-0.1.2/calculator_beau28713/__main__.py`

 * *Files identical despite different names*

### Comparing `calculator_beau28713-0.1.1/LICENSE` & `calculator_beau28713-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calculator_beau28713-0.1.1/PKG-INFO` & `calculator_beau28713-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: calculator-beau28713
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple gui calculator that does basic math
 Author: Beau
 Author-email: beau28713@gmail.com
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Kivy (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Title
 GUI Calculator
 
 ## Description
```

