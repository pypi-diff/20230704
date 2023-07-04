# Comparing `tmp/testdwg-0.4.6.tar.gz` & `tmp/testdwg-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-0.4.6.tar", max compression
+gzip compressed data, was "testdwg-0.4.7.tar", max compression
```

## Comparing `testdwg-0.4.6.tar` & `testdwg-0.4.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-04 14:49:35.223205 testdwg-0.4.6/README.md
--rw-r--r--   0        0        0      305 2023-07-04 14:49:52.855515 testdwg-0.4.6/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-04 14:49:35.223205 testdwg-0.4.6/testdwg/__init__.py
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 14:51:25.569934 testdwg-0.4.7/README.md
+-rw-r--r--   0        0        0      305 2023-07-04 14:51:44.706127 testdwg-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-04 14:51:25.569934 testdwg-0.4.7/testdwg/__init__.py
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 testdwg-0.4.7/PKG-INFO
```

