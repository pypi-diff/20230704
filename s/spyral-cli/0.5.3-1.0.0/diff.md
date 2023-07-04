# Comparing `tmp/spyral_cli-0.5.3.tar.gz` & `tmp/spyral_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_cli-0.5.3.tar", max compression
+gzip compressed data, was "spyral_cli-1.0.0.tar", max compression
```

## Comparing `spyral_cli-0.5.3.tar` & `spyral_cli-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      540 2023-06-30 12:26:16.543146 spyral_cli-0.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-0.5.3/src/spyral/__init__.py
--rw-r--r--   0        0        0     4148 2023-06-30 12:22:54.974096 spyral_cli-0.5.3/src/spyral/cli.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      691 2023-07-04 07:49:38.767133 spyral_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 09:21:47.934822 spyral_cli-1.0.0/src/spyral/__init__.py
+-rw-r--r--   0        0        0     5497 2023-07-04 07:49:32.356053 spyral_cli-1.0.0/src/spyral/cli.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 spyral_cli-1.0.0/PKG-INFO
```

### Comparing `spyral_cli-0.5.3/PKG-INFO` & `spyral_cli-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: spyral-cli
-Version: 0.5.3
+Version: 1.0.0
 Summary: 
 License: MIT
 Author: Paul Gessinger
 Author-email: hello@paulgessinger.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: backports-strenum (>=1.2.4,<2.0.0)
 Requires-Dist: plotext (>=5.2.8,<6.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

