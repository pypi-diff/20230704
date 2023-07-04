# Comparing `tmp/testdwg-0.4.0.tar.gz` & `tmp/testdwg-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-0.4.0.tar", max compression
+gzip compressed data, was "testdwg-0.4.1.tar", max compression
```

## Comparing `testdwg-0.4.0.tar` & `testdwg-0.4.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-04 10:32:41.267577 testdwg-0.4.0/README.md
--rw-r--r--   0        0        0      265 2023-07-04 10:32:53.483762 testdwg-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-04 10:32:41.267577 testdwg-0.4.0/testdwg/__init__.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 testdwg-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 14:24:13.540876 testdwg-0.4.1/README.md
+-rw-r--r--   0        0        0      305 2023-07-04 14:24:29.550252 testdwg-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-04 14:24:13.544877 testdwg-0.4.1/testdwg/__init__.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.1/PKG-INFO
```

