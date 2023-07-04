# Comparing `tmp/psd-tools-1.9.8.tar.gz` & `tmp/psd-tools-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psd-tools-1.9.8.tar", last modified: Wed Mar 18 05:59:38 2020, max compression
+gzip compressed data, was "dist/psd-tools-1.9.9.tar", last modified: Mon Mar 30 04:38:14 2020, max compression
```

## Comparing `psd-tools-1.9.8.tar` & `psd-tools-1.9.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.061255 psd-tools-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (115)    18662 2020-03-18 05:59:24.000000 psd-tools-1.9.8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (115)       74 2020-03-18 05:59:24.000000 psd-tools-1.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)    27663 2020-03-18 05:59:38.061255 psd-tools-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1510 2020-03-18 05:59:24.000000 psd-tools-1.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (115)      617 2020-03-18 05:59:38.061255 psd-tools-1.9.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (115)     2390 2020-03-18 05:59:24.000000 psd-tools-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.053254 psd-tools-1.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.057254 psd-tools-1.9.8/src/psd_tools/
--rw-r--r--   0 runner    (1001) docker     (115)      158 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1880 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.057254 psd-tools-1.9.8/src/psd_tools/api/
--rw-r--r--   0 runner    (1001) docker     (115)      502 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     9520 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/adjustments.py
--rw-r--r--   0 runner    (1001) docker     (115)    11901 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/effects.py
--rw-r--r--   0 runner    (1001) docker     (115)    27361 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/layers.py
--rw-r--r--   0 runner    (1001) docker     (115)     3127 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/mask.py
--rw-r--r--   0 runner    (1001) docker     (115)     4897 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/numpy_io.py
--rw-r--r--   0 runner    (1001) docker     (115)     9050 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/pil_io.py
--rw-r--r--   0 runner    (1001) docker     (115)    18361 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/psd_image.py
--rw-r--r--   0 runner    (1001) docker     (115)    11608 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/shape.py
--rw-r--r--   0 runner    (1001) docker     (115)     4105 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/api/smart_object.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.057254 psd-tools-1.9.8/src/psd_tools/composer/
--rw-r--r--   0 runner    (1001) docker     (115)    14192 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     8700 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composer/blend.py
--rw-r--r--   0 runner    (1001) docker     (115)     1876 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composer/effects.py
--rw-r--r--   0 runner    (1001) docker     (115)    12904 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composer/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.057254 psd-tools-1.9.8/src/psd_tools/composite/
--rw-r--r--   0 runner    (1001) docker     (115)    17352 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     9664 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composite/blend.py
--rw-r--r--   0 runner    (1001) docker     (115)     1714 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composite/effects.py
--rw-r--r--   0 runner    (1001) docker     (115)    13546 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/composite/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.057254 psd-tools-1.9.8/src/psd_tools/compression/
--rw-r--r--   0 runner    (1001) docker     (115)     5831 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3590 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/compression/_rle.pyx
--rw-r--r--   0 runner    (1001) docker     (115)     3028 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/compression/rle.py
--rw-r--r--   0 runner    (1001) docker     (115)    11782 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.061255 psd-tools-1.9.8/src/psd_tools/psd/
--rw-r--r--   0 runner    (1001) docker     (115)     3337 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    20329 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/adjustments.py
--rw-r--r--   0 runner    (1001) docker     (115)    15819 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/base.py
--rw-r--r--   0 runner    (1001) docker     (115)     1818 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/color.py
--rw-r--r--   0 runner    (1001) docker     (115)     1803 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/color_mode_data.py
--rw-r--r--   0 runner    (1001) docker     (115)    18481 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (115)    13044 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/effects_layer.py
--rw-r--r--   0 runner    (1001) docker     (115)    11556 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/engine_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     6043 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/filter_effects.py
--rw-r--r--   0 runner    (1001) docker     (115)     2230 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/header.py
--rw-r--r--   0 runner    (1001) docker     (115)     3797 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/image_data.py
--rw-r--r--   0 runner    (1001) docker     (115)    30282 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/image_resources.py
--rw-r--r--   0 runner    (1001) docker     (115)    29680 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/layer_and_mask.py
--rw-r--r--   0 runner    (1001) docker     (115)     5817 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/linked_layer.py
--rw-r--r--   0 runner    (1001) docker     (115)     7229 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/patterns.py
--rw-r--r--   0 runner    (1001) docker     (115)    25405 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/tagged_blocks.py
--rw-r--r--   0 runner    (1001) docker     (115)     8671 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/psd/vector.py
--rw-r--r--   0 runner    (1001) docker     (115)    52949 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/terminology.py
--rw-r--r--   0 runner    (1001) docker     (115)     7746 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     1002 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/validators.py
--rw-r--r--   0 runner    (1001) docker     (115)       22 2020-03-18 05:59:24.000000 psd-tools-1.9.8/src/psd_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-18 05:59:38.057254 psd-tools-1.9.8/src/psd_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)    27663 2020-03-18 05:59:37.000000 psd-tools-1.9.8/src/psd_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1684 2020-03-18 05:59:37.000000 psd-tools-1.9.8/src/psd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-18 05:59:37.000000 psd-tools-1.9.8/src/psd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       55 2020-03-18 05:59:37.000000 psd-tools-1.9.8/src/psd_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)      107 2020-03-18 05:59:37.000000 psd-tools-1.9.8/src/psd_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       10 2020-03-18 05:59:37.000000 psd-tools-1.9.8/src/psd_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.971084 psd-tools-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (115)    18744 2020-03-30 04:38:01.000000 psd-tools-1.9.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (115)       74 2020-03-30 04:38:01.000000 psd-tools-1.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (115)    27785 2020-03-30 04:38:14.971084 psd-tools-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     1510 2020-03-30 04:38:01.000000 psd-tools-1.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (115)      617 2020-03-30 04:38:14.971084 psd-tools-1.9.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (115)     2390 2020-03-30 04:38:01.000000 psd-tools-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.959084 psd-tools-1.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.959084 psd-tools-1.9.9/src/psd_tools/
+-rw-r--r--   0 runner    (1001) docker     (115)      158 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1880 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.967084 psd-tools-1.9.9/src/psd_tools/api/
+-rw-r--r--   0 runner    (1001) docker     (115)      502 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9520 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/adjustments.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11901 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/effects.py
+-rw-r--r--   0 runner    (1001) docker     (115)    27361 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/layers.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3127 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/mask.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4897 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/numpy_io.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9050 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/pil_io.py
+-rw-r--r--   0 runner    (1001) docker     (115)    18361 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/psd_image.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11608 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/shape.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4105 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/api/smart_object.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.967084 psd-tools-1.9.9/src/psd_tools/composer/
+-rw-r--r--   0 runner    (1001) docker     (115)    14192 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8700 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composer/blend.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1876 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composer/effects.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12904 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composer/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.967084 psd-tools-1.9.9/src/psd_tools/composite/
+-rw-r--r--   0 runner    (1001) docker     (115)    17352 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9664 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composite/blend.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1825 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composite/effects.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13546 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/composite/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.971084 psd-tools-1.9.9/src/psd_tools/compression/
+-rw-r--r--   0 runner    (1001) docker     (115)     5831 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3590 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/compression/_rle.pyx
+-rw-r--r--   0 runner    (1001) docker     (115)     3028 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/compression/rle.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11782 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.971084 psd-tools-1.9.9/src/psd_tools/psd/
+-rw-r--r--   0 runner    (1001) docker     (115)     3337 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    20329 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/adjustments.py
+-rw-r--r--   0 runner    (1001) docker     (115)    15819 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1818 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/color.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1803 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/color_mode_data.py
+-rw-r--r--   0 runner    (1001) docker     (115)    18481 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13044 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/effects_layer.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11556 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/engine_data.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6043 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/filter_effects.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2230 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/header.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3797 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/image_data.py
+-rw-r--r--   0 runner    (1001) docker     (115)    30282 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/image_resources.py
+-rw-r--r--   0 runner    (1001) docker     (115)    29680 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/layer_and_mask.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5817 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/linked_layer.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7229 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (115)    25405 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/tagged_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8671 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/psd/vector.py
+-rw-r--r--   0 runner    (1001) docker     (115)    52949 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/terminology.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7746 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1002 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/validators.py
+-rw-r--r--   0 runner    (1001) docker     (115)       22 2020-03-30 04:38:01.000000 psd-tools-1.9.9/src/psd_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-30 04:38:14.963084 psd-tools-1.9.9/src/psd_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)    27785 2020-03-30 04:38:14.000000 psd-tools-1.9.9/src/psd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     1684 2020-03-30 04:38:14.000000 psd-tools-1.9.9/src/psd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-30 04:38:14.000000 psd-tools-1.9.9/src/psd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       55 2020-03-30 04:38:14.000000 psd-tools-1.9.9/src/psd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      107 2020-03-30 04:38:14.000000 psd-tools-1.9.9/src/psd_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       10 2020-03-30 04:38:14.000000 psd-tools-1.9.9/src/psd_tools.egg-info/top_level.txt
```

### Comparing `psd-tools-1.9.8/CHANGES.rst` & `psd-tools-1.9.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.9.9 (2020-03-30)
+------------------
+
+- [composite] Fix stroke effect argument.
+
 1.9.8 (2020-03-18)
 ------------------
 
 - [composite] Fix incorrect fill opacity handling in compositing.
 - [composite] Fix incorrect alpha for patterns.
 
 1.9.7 (2020-03-17)
```

### Comparing `psd-tools-1.9.8/PKG-INFO` & `psd-tools-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: psd-tools
-Version: 1.9.8
+Version: 1.9.9
 Summary: Python package for working with Adobe Photoshop PSD files
 Home-page: https://github.com/psd-tools/psd-tools
 Author: Kota Yamaguchi
 Author-email: KotaYamaguchi1984@gmail.com
 License: MIT License
 Description: psd-tools
         =========
@@ -65,14 +65,19 @@
         ------------
         
         See contributing_ page.
         
         .. _contributing: https://github.com/psd-tools/psd-tools/blob/master/docs/contributing.rst
         
         
+        1.9.9 (2020-03-30)
+        ------------------
+        
+        - [composite] Fix stroke effect argument.
+        
         1.9.8 (2020-03-18)
         ------------------
         
         - [composite] Fix incorrect fill opacity handling in compositing.
         - [composite] Fix incorrect alpha for patterns.
         
         1.9.7 (2020-03-17)
```

### Comparing `psd-tools-1.9.8/README.rst` & `psd-tools-1.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/setup.cfg` & `psd-tools-1.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/setup.py` & `psd-tools-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/__main__.py` & `psd-tools-1.9.9/src/psd_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/adjustments.py` & `psd-tools-1.9.9/src/psd_tools/api/adjustments.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/effects.py` & `psd-tools-1.9.9/src/psd_tools/api/effects.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/layers.py` & `psd-tools-1.9.9/src/psd_tools/api/layers.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/mask.py` & `psd-tools-1.9.9/src/psd_tools/api/mask.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/numpy_io.py` & `psd-tools-1.9.9/src/psd_tools/api/numpy_io.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/pil_io.py` & `psd-tools-1.9.9/src/psd_tools/api/pil_io.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/psd_image.py` & `psd-tools-1.9.9/src/psd_tools/api/psd_image.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/shape.py` & `psd-tools-1.9.9/src/psd_tools/api/shape.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/api/smart_object.py` & `psd-tools-1.9.9/src/psd_tools/api/smart_object.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/composer/__init__.py` & `psd-tools-1.9.9/src/psd_tools/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/composer/blend.py` & `psd-tools-1.9.9/src/psd_tools/composer/blend.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/composer/effects.py` & `psd-tools-1.9.9/src/psd_tools/composer/effects.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/composer/vector.py` & `psd-tools-1.9.9/src/psd_tools/composer/vector.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/composite/__init__.py` & `psd-tools-1.9.9/src/psd_tools/composite/__init__.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/composite/blend.py` & `psd-tools-1.9.9/src/psd_tools/composite/blend.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/composite/effects.py` & `psd-tools-1.9.9/src/psd_tools/composite/effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 def draw_stroke_effect(viewport, shape, desc, psd):
     logger.debug('Stroke effect has limited support')
     height, width = viewport[3] - viewport[1], viewport[2] - viewport[0]
+    if not isinstance(shape, np.ndarray):
+        shape = np.full((height, width, 1), shape, dtype=np.float32)
 
     paint = desc.get(Key.PaintType).enum
     if paint == Enum.SolidColor:
         color, _ = draw_solid_color_fill(viewport, desc)
     elif paint == Enum.Pattern:
         color, _ = draw_pattern_fill(viewport, psd, desc)
     elif paint == Enum.GradientFill:
```

### Comparing `psd-tools-1.9.8/src/psd_tools/composite/vector.py` & `psd-tools-1.9.9/src/psd_tools/composite/vector.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/compression/__init__.py` & `psd-tools-1.9.9/src/psd_tools/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/compression/_rle.pyx` & `psd-tools-1.9.9/src/psd_tools/compression/_rle.pyx`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/compression/rle.py` & `psd-tools-1.9.9/src/psd_tools/compression/rle.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/constants.py` & `psd-tools-1.9.9/src/psd_tools/constants.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/__init__.py` & `psd-tools-1.9.9/src/psd_tools/psd/__init__.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/adjustments.py` & `psd-tools-1.9.9/src/psd_tools/psd/adjustments.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/base.py` & `psd-tools-1.9.9/src/psd_tools/psd/base.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/color.py` & `psd-tools-1.9.9/src/psd_tools/psd/color.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/color_mode_data.py` & `psd-tools-1.9.9/src/psd_tools/psd/color_mode_data.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/descriptor.py` & `psd-tools-1.9.9/src/psd_tools/psd/descriptor.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/effects_layer.py` & `psd-tools-1.9.9/src/psd_tools/psd/effects_layer.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/engine_data.py` & `psd-tools-1.9.9/src/psd_tools/psd/engine_data.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/filter_effects.py` & `psd-tools-1.9.9/src/psd_tools/psd/filter_effects.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/header.py` & `psd-tools-1.9.9/src/psd_tools/psd/header.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/image_data.py` & `psd-tools-1.9.9/src/psd_tools/psd/image_data.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/image_resources.py` & `psd-tools-1.9.9/src/psd_tools/psd/image_resources.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/layer_and_mask.py` & `psd-tools-1.9.9/src/psd_tools/psd/layer_and_mask.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/linked_layer.py` & `psd-tools-1.9.9/src/psd_tools/psd/linked_layer.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/patterns.py` & `psd-tools-1.9.9/src/psd_tools/psd/patterns.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/tagged_blocks.py` & `psd-tools-1.9.9/src/psd_tools/psd/tagged_blocks.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/psd/vector.py` & `psd-tools-1.9.9/src/psd_tools/psd/vector.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/terminology.py` & `psd-tools-1.9.9/src/psd_tools/terminology.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/utils.py` & `psd-tools-1.9.9/src/psd_tools/utils.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools/validators.py` & `psd-tools-1.9.9/src/psd_tools/validators.py`

 * *Files identical despite different names*

### Comparing `psd-tools-1.9.8/src/psd_tools.egg-info/PKG-INFO` & `psd-tools-1.9.9/src/psd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: psd-tools
-Version: 1.9.8
+Version: 1.9.9
 Summary: Python package for working with Adobe Photoshop PSD files
 Home-page: https://github.com/psd-tools/psd-tools
 Author: Kota Yamaguchi
 Author-email: KotaYamaguchi1984@gmail.com
 License: MIT License
 Description: psd-tools
         =========
@@ -65,14 +65,19 @@
         ------------
         
         See contributing_ page.
         
         .. _contributing: https://github.com/psd-tools/psd-tools/blob/master/docs/contributing.rst
         
         
+        1.9.9 (2020-03-30)
+        ------------------
+        
+        - [composite] Fix stroke effect argument.
+        
         1.9.8 (2020-03-18)
         ------------------
         
         - [composite] Fix incorrect fill opacity handling in compositing.
         - [composite] Fix incorrect alpha for patterns.
         
         1.9.7 (2020-03-17)
```

### Comparing `psd-tools-1.9.8/src/psd_tools.egg-info/SOURCES.txt` & `psd-tools-1.9.9/src/psd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

