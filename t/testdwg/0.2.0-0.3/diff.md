# Comparing `tmp/testdwg-0.2.0.tar.gz` & `tmp/testdwg-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-0.2.0.tar", max compression
+gzip compressed data, was "testdwg-0.3.tar", max compression
```

## Comparing `testdwg-0.2.0.tar` & `testdwg-0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-04 10:02:47.043297 testdwg-0.2.0/README.md
--rw-r--r--   0        0        0      265 2023-07-04 10:03:01.771585 testdwg-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-04 10:02:47.043297 testdwg-0.2.0/testdwg/__init__.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 testdwg-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 10:03:42.670500 testdwg-0.3/README.md
+-rw-r--r--   0        0        0      263 2023-07-04 10:03:56.298378 testdwg-0.3/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-04 10:03:42.670500 testdwg-0.3/testdwg/__init__.py
+-rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 testdwg-0.3/PKG-INFO
```

