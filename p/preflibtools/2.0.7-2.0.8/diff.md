# Comparing `tmp/preflibtools-2.0.7.tar.gz` & `tmp/preflibtools-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preflibtools-2.0.7.tar", last modified: Mon Jul  3 12:36:34 2023, max compression
+gzip compressed data, was "preflibtools-2.0.8.tar", last modified: Mon Jul  3 13:11:40 2023, max compression
```

## Comparing `preflibtools-2.0.7.tar` & `preflibtools-2.0.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 12:36:21.000000 preflibtools-2.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 12:36:21.000000 preflibtools-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-03 12:36:34.039065 preflibtools-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-07-03 12:36:21.000000 preflibtools-2.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/output/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/output/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/output/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/output/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/output/_static/plus.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.031065 preflibtools-2.0.7/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/docs/source/reference/instances/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/convert.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/preflibinstance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/sampling.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/instances/sanity.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/docs/source/reference/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/basic.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/distance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/singlecrossing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/reference/properties/singlepeaked.rst
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-03 12:36:21.000000 preflibtools-2.0.7/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools/instances/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    45810 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/preflibinstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/instances/sanity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools/properties/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/singlecrossing.py
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-07-03 12:36:21.000000 preflibtools-2.0.7/preflibtools/properties/singlepeakedness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.035065 preflibtools-2.0.7/preflibtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 12:36:33.000000 preflibtools-2.0.7/preflibtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-03 12:36:34.039065 preflibtools-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-03 12:36:21.000000 preflibtools-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/tests/instance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:34.039065 preflibtools-2.0.7/tests/instance/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_soi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_toc.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_toi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/test_io_wmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/io/write_file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/test_categorical_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/test_order_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/instance/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/runningex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-03 12:36:21.000000 preflibtools-2.0.7/tests/test_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.371492 preflibtools-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 13:11:29.000000 preflibtools-2.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 13:11:29.000000 preflibtools-2.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-03 13:11:40.371492 preflibtools-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-07-03 13:11:29.000000 preflibtools-2.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.363492 preflibtools-2.0.8/docs/output/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/docs/output/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/output/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/output/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/output/_static/plus.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/docs/source/reference/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/instances/convert.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/instances/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/instances/preflibinstance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/instances/sampling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/instances/sanity.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/docs/source/reference/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/properties/basic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/properties/distance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/properties/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/properties/singlecrossing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/reference/properties/singlepeaked.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-03 13:11:29.000000 preflibtools-2.0.8/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/preflibtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/preflibtools/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/instances/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46434 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/instances/preflibinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/instances/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/instances/sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/preflibtools/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/properties/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/properties/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/properties/singlecrossing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-07-03 13:11:29.000000 preflibtools-2.0.8/preflibtools/properties/singlepeakedness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/preflibtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-07-03 13:11:40.000000 preflibtools-2.0.8/preflibtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-03 13:11:40.000000 preflibtools-2.0.8/preflibtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:40.000000 preflibtools-2.0.8/preflibtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:40.000000 preflibtools-2.0.8/preflibtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 13:11:40.000000 preflibtools-2.0.8/preflibtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-03 13:11:40.371492 preflibtools-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-03 13:11:29.000000 preflibtools-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.367492 preflibtools-2.0.8/tests/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:40.371492 preflibtools-2.0.8/tests/instance/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/test_io_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/test_io_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/test_io_soi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/test_io_toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/test_io_toi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/test_io_wmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/io/write_file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/test_categorical_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/test_order_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/instance/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/runningex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-03 13:11:29.000000 preflibtools-2.0.8/tests/test_property.py
```

### Comparing `preflibtools-2.0.7/LICENSE.md` & `preflibtools-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/PKG-INFO` & `preflibtools-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preflibtools
-Version: 2.0.7
+Version: 2.0.8
 Summary: A set of tools to work with preference data from the PrefLib.org website.
 Home-page: https://github.com/PrefLib/preflibtools
 Author: Simon Rey
 Author-email: reysimon@orange.fr
 License: GNU General Public License v3
 Keywords: preflibtools
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `preflibtools-2.0.7/README.rst` & `preflibtools-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/docs/Makefile` & `preflibtools-2.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/docs/make.bat` & `preflibtools-2.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/docs/source/conf.py` & `preflibtools-2.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/docs/source/index.rst` & `preflibtools-2.0.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/docs/source/usage.rst` & `preflibtools-2.0.8/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools/instances/convert.py` & `preflibtools-2.0.8/preflibtools/instances/convert.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools/instances/preflibinstance.py` & `preflibtools-2.0.8/preflibtools/instances/preflibinstance.py`

 * *Files 6% similar despite different names*

```diff
@@ -767,14 +767,24 @@
             if relative_size_truncators is None:
                 relative_size_truncators = []
             else:
                 size_truncators = []
 
         cat_instance = cls()
         cat_instance.file_path = instance.file_path
+        cat_instance.file_name = instance.file_name
+        cat_instance.data_type = "cat"
+        cat_instance.modification_type = instance.modification_type
+        cat_instance.relates_to = instance.relates_to
+        cat_instance.related_files = instance.related_files
+        cat_instance.title = instance.title
+        cat_instance.description = instance.description
+        cat_instance.publication_date = instance.publication_date
+        cat_instance.modification_date = instance.modification_date
+        cat_instance.num_alternatives = instance.num_alternatives
         if len(size_truncators) > 0:
             cat_instance.num_categories = len(size_truncators) + 1
         else:
             cat_instance.num_categories = len(relative_size_truncators)
         cat_instance.categories_name = {}
         cat_instance.preferences = []
         for order, multiplicty in instance.multiplicity.items():
@@ -794,14 +804,15 @@
             if order_index < len(order):
                 preferences.append(tuple(a for indif_class in order[order_index:] for a in indif_class))
             preferences = tuple(preferences)
             cat_instance.preferences.append(preferences)
             cat_instance.multiplicity[preferences] = multiplicty
 
         cat_instance.num_unique_preferences = len(cat_instance.preferences)
+        cat_instance.recompute_cardinality_param()
         return cat_instance
 
     def __str__(self):
         return "Categorical-Instance: {} <{},{}>".format(self.file_name, self.num_voters, self.num_alternatives)
 
 
 class WeightedDiGraph(object):
```

### Comparing `preflibtools-2.0.7/preflibtools/instances/sampling.py` & `preflibtools-2.0.8/preflibtools/instances/sampling.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools/instances/sanity.py` & `preflibtools-2.0.8/preflibtools/instances/sanity.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools/properties/basic.py` & `preflibtools-2.0.8/preflibtools/properties/basic.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools/properties/distances.py` & `preflibtools-2.0.8/preflibtools/properties/distances.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools/properties/singlecrossing.py` & `preflibtools-2.0.8/preflibtools/properties/singlecrossing.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools/properties/singlepeakedness.py` & `preflibtools-2.0.8/preflibtools/properties/singlepeakedness.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/preflibtools.egg-info/PKG-INFO` & `preflibtools-2.0.8/preflibtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preflibtools
-Version: 2.0.7
+Version: 2.0.8
 Summary: A set of tools to work with preference data from the PrefLib.org website.
 Home-page: https://github.com/PrefLib/preflibtools
 Author: Simon Rey
 Author-email: reysimon@orange.fr
 License: GNU General Public License v3
 Keywords: preflibtools
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `preflibtools-2.0.7/preflibtools.egg-info/SOURCES.txt` & `preflibtools-2.0.8/preflibtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/setup.py` & `preflibtools-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     keywords='preflibtools',
     name='preflibtools',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/PrefLib/preflibtools',
-    version='2.0.7',
+    version='2.0.8',
     zip_safe=False,
 )
```

### Comparing `preflibtools-2.0.7/tests/instance/io/test_io_cat.py` & `preflibtools-2.0.8/tests/instance/io/test_io_cat.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/io/test_io_instances.py` & `preflibtools-2.0.8/tests/instance/io/test_io_instances.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/io/test_io_soi.py` & `preflibtools-2.0.8/tests/instance/io/test_io_soi.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/io/test_io_toc.py` & `preflibtools-2.0.8/tests/instance/io/test_io_toc.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/io/test_io_toi.py` & `preflibtools-2.0.8/tests/instance/io/test_io_toi.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/io/test_io_wmd.py` & `preflibtools-2.0.8/tests/instance/io/test_io_wmd.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/io/write_file_test.py` & `preflibtools-2.0.8/tests/instance/io/write_file_test.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/test_categorical_handling.py` & `preflibtools-2.0.8/tests/instance/test_categorical_handling.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/test_order_handling.py` & `preflibtools-2.0.8/tests/instance/test_order_handling.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/instance/test_sampling.py` & `preflibtools-2.0.8/tests/instance/test_sampling.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/runningex.py` & `preflibtools-2.0.8/tests/runningex.py`

 * *Files identical despite different names*

### Comparing `preflibtools-2.0.7/tests/test_property.py` & `preflibtools-2.0.8/tests/test_property.py`

 * *Files identical despite different names*

