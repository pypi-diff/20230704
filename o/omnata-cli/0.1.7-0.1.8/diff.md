# Comparing `tmp/omnata_cli-0.1.7.tar.gz` & `tmp/omnata_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_cli-0.1.7.tar", max compression
+gzip compressed data, was "omnata_cli-0.1.8.tar", max compression
```

## Comparing `omnata_cli-0.1.7.tar` & `omnata_cli-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    26526 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/LICENSE
--rw-r--r--   0        0        0       49 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/README.md
--rw-r--r--   0        0        0      534 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1039 2023-06-16 03:46:24.872951 omnata_cli-0.1.7/src/omnata_cli/__init__.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 omnata_cli-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-07-04 06:59:28.026641 omnata_cli-0.1.8/LICENSE
+-rw-r--r--   0        0        0       49 2023-07-04 06:59:28.026641 omnata_cli-0.1.8/README.md
+-rw-r--r--   0        0        0      503 2023-07-04 06:59:28.026641 omnata_cli-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1039 2023-07-04 06:59:28.026641 omnata_cli-0.1.8/src/omnata_cli/__init__.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 omnata_cli-0.1.8/PKG-INFO
```

### Comparing `omnata_cli-0.1.7/LICENSE` & `omnata_cli-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.7/src/omnata_cli/__init__.py` & `omnata_cli-0.1.8/src/omnata_cli/__init__.py`

 * *Files identical despite different names*

