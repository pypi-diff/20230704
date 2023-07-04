# Comparing `tmp/testdwg-0.4.4.tar.gz` & `tmp/testdwg-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-0.4.4.tar", max compression
+gzip compressed data, was "testdwg-0.4.5.tar", max compression
```

## Comparing `testdwg-0.4.4.tar` & `testdwg-0.4.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-04 14:43:29.715623 testdwg-0.4.4/README.md
--rw-r--r--   0        0        0      305 2023-07-04 14:43:44.216116 testdwg-0.4.4/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-04 14:43:29.715623 testdwg-0.4.4/testdwg/__init__.py
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 14:46:44.538808 testdwg-0.4.5/README.md
+-rw-r--r--   0        0        0      305 2023-07-04 14:47:00.490919 testdwg-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-04 14:46:44.538808 testdwg-0.4.5/testdwg/__init__.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.5/PKG-INFO
```

