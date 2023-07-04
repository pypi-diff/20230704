# Comparing `tmp/testdwg-0.4.8.tar.gz` & `tmp/testdwg-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-0.4.8.tar", max compression
+gzip compressed data, was "testdwg-0.4.9.tar", max compression
```

## Comparing `testdwg-0.4.8.tar` & `testdwg-0.4.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-04 14:58:37.242982 testdwg-0.4.8/README.md
--rw-r--r--   0        0        0      305 2023-07-04 14:58:48.635234 testdwg-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-04 14:58:37.242982 testdwg-0.4.8/testdwg/__init__.py
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 15:03:33.177599 testdwg-0.4.9/README.md
+-rw-r--r--   0        0        0      305 2023-07-04 15:03:47.001868 testdwg-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-04 15:03:33.177599 testdwg-0.4.9/testdwg/__init__.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.9/PKG-INFO
```

