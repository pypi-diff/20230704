# Comparing `tmp/ecquote-1.5.0.tar.gz` & `tmp/ecquote-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecquote-1.5.0.tar", last modified: Tue Jul  4 14:58:17 2023, max compression
+gzip compressed data, was "ecquote-1.5.1.tar", last modified: Tue Jul  4 16:51:23 2023, max compression
```

## Comparing `ecquote-1.5.0.tar` & `ecquote-1.5.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.313237 ecquote-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 14:58:06.000000 ecquote-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 14:58:06.000000 ecquote-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-04 14:58:17.309237 ecquote-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-04 14:58:06.000000 ecquote-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.301237 ecquote-1.5.0/ecquote/
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/area.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7794 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/cart.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27460 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/costing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4866 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/grib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8211 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea_fixed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea_mask_reduced.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea_mask_regular.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/mars.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7996 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/matching.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2530 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/modify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5650 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35542 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/repres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16707 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.309237 ecquote-1.5.0/ecquote/resources/
--rwxr-xr-x   0 runner    (1001) docker     (123)   106938 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F1280.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    13076 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F160.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    16336 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F200.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    21410 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F256.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    26806 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F320.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    33394 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F400.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    53428 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F640.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6566 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F80.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    10470 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N128.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   106600 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N1280.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    13048 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N160.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    16308 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N200.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    20992 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N256.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    26438 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N320.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    33042 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N400.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    53086 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N640.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6540 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N80.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   106408 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O1280.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    13036 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O160.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    26276 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O320.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    52898 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O640.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     5972 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/accuracy.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/data-values-bands.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2055 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/epu-based.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     7067 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/free-open-data.diss
--rwxr-xr-x   0 runner    (1001) docker     (123)     3910 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/free-wmo-essential.diss
--rwxr-xr-x   0 runner    (1001) docker     (123)    71731 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/params.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/pgen-accuracy.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    42393 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/reduced-0_125.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    20487 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/reduced-0_25.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     9898 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/reduced-0_5.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    42755 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/regular-0_125.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    12384 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/representations.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    24461 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/sets.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      137 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/volume-bands.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)   311505 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/wave-mask-reduced.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   340586 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/wave-mask-regular.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     2042 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/rest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1850 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/sets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.309237 ecquote-1.5.0/ecquote/splitters/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/canonical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/constant.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/destination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      932 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/free_grids.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9463 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/free_sets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2614 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/freebies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/group_by.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2555 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/high_frequency.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/repres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/shgg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1377 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/subset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/validate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/testing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3883 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.305237 ecquote-1.5.0/ecquote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:58:17.313237 ecquote-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-04 14:58:06.000000 ecquote-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:51:23.466428 ecquote-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 16:51:09.000000 ecquote-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 16:51:09.000000 ecquote-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-04 16:51:23.466428 ecquote-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-04 16:51:09.000000 ecquote-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:51:23.426428 ecquote-1.5.1/ecquote/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/area.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7794 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/cart.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28018 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/costing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4866 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/grib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8211 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/landsea.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/landsea_fixed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/landsea_mask_reduced.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/landsea_mask_regular.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/mars.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7996 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/matching.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2530 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/modify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5650 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35542 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/repres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16707 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:51:23.454428 ecquote-1.5.1/ecquote/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106938 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F1280.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13076 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F160.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16336 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F200.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21410 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F256.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26806 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F320.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33394 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F400.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53428 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F640.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6566 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/F80.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10470 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N128.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106600 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N1280.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13048 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N160.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16308 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N200.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20992 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N256.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26438 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N320.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33042 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N400.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53086 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N640.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6540 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/N80.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106408 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/O1280.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13036 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/O160.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26276 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/O320.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52898 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/O640.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5972 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/accuracy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/data-values-bands.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2055 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/epu-based.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7067 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/free-open-data.diss
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3910 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/free-wmo-essential.diss
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71731 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/params.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/pgen-accuracy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42393 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/reduced-0_125.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20487 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/reduced-0_25.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9898 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/reduced-0_5.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42755 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/regular-0_125.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12384 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/representations.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24461 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/sets.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      137 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/volume-bands.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)   311505 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/wave-mask-reduced.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   340586 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources/wave-mask-regular.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2042 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/rest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1850 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/sets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:51:23.462428 ecquote-1.5.1/ecquote/splitters/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/canonical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/constant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/destination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      932 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/free_grids.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9463 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/free_sets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2614 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/freebies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/group_by.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2555 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/high_frequency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/repres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/shgg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1377 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/subset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/splitters/validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/testing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3883 2023-07-04 16:51:09.000000 ecquote-1.5.1/ecquote/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:51:23.430428 ecquote-1.5.1/ecquote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-04 16:51:23.000000 ecquote-1.5.1/ecquote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 16:51:23.000000 ecquote-1.5.1/ecquote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:51:23.000000 ecquote-1.5.1/ecquote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 16:51:23.000000 ecquote-1.5.1/ecquote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 16:51:23.000000 ecquote-1.5.1/ecquote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 16:51:23.000000 ecquote-1.5.1/ecquote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:51:23.000000 ecquote-1.5.1/ecquote.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:51:23.466428 ecquote-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-04 16:51:09.000000 ecquote-1.5.1/setup.py
```

### Comparing `ecquote-1.5.0/LICENSE` & `ecquote-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/PKG-INFO` & `ecquote-1.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecquote
-Version: 1.5.0
+Version: 1.5.1
 Summary: A package to estimate the cost and volume of an ECMWF dissemination feed
 Home-page: https://github.com/ecmwf/ecquote
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ecquote-1.5.0/README.md` & `ecquote-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/__main__.py` & `ecquote-1.5.1/ecquote/__main__.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/area.py` & `ecquote-1.5.1/ecquote/area.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/cart.py` & `ecquote-1.5.1/ecquote/cart.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/costing.py` & `ecquote-1.5.1/ecquote/costing.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,30 @@
         band, euro, error, _ = self.band()
         if error:
             print("   Volume band:     ", error)
         else:
             print("   Volume band:     ", bytes(band * 1024 * 1024 * 1024))
             print("   Volume cost:     ", "EUR {:,}".format(euro))
 
+        if self.experimental:
+            print("   Yearly values:   ", "{:,}".format(self.yearly_data_values))
+
+            band, euro, error, _ = self.data_values_band()
+
+            if error:
+                print("   Values band:     ", error)
+            else:
+                print("   Values band:     ", "{:,}".format(band))
+                print("   Values cost:     ", "EUR {:,}".format(euro))
+
+            print(
+                "   Values ratio:    ",
+                "{:.2f}".format(self.yearly_volume / self.yearly_data_values),
+            )
+
     def band(self):
         return band(self.yearly_volume)
 
     def data_values_band(self):
         return data_values_band(self.yearly_data_values)
```

### Comparing `ecquote-1.5.0/ecquote/grib.py` & `ecquote-1.5.1/ecquote/grib.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/grid.py` & `ecquote-1.5.1/ecquote/grid.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/landsea.py` & `ecquote-1.5.1/ecquote/landsea.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/landsea_fixed.py` & `ecquote-1.5.1/ecquote/landsea_fixed.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/landsea_mask_reduced.py` & `ecquote-1.5.1/ecquote/landsea_mask_reduced.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/landsea_mask_regular.py` & `ecquote-1.5.1/ecquote/landsea_mask_regular.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/mars.py` & `ecquote-1.5.1/ecquote/mars.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/matching.py` & `ecquote-1.5.1/ecquote/matching.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/modify.py` & `ecquote-1.5.1/ecquote/modify.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/parser.py` & `ecquote-1.5.1/ecquote/parser.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/repres.py` & `ecquote-1.5.1/ecquote/repres.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/request.py` & `ecquote-1.5.1/ecquote/request.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F1280.json` & `ecquote-1.5.1/ecquote/resources/F1280.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F160.json` & `ecquote-1.5.1/ecquote/resources/F160.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F200.json` & `ecquote-1.5.1/ecquote/resources/F200.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F256.json` & `ecquote-1.5.1/ecquote/resources/F256.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F320.json` & `ecquote-1.5.1/ecquote/resources/F320.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F400.json` & `ecquote-1.5.1/ecquote/resources/F400.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F640.json` & `ecquote-1.5.1/ecquote/resources/F640.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/F80.json` & `ecquote-1.5.1/ecquote/resources/F80.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N128.json` & `ecquote-1.5.1/ecquote/resources/N128.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N1280.json` & `ecquote-1.5.1/ecquote/resources/N1280.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N160.json` & `ecquote-1.5.1/ecquote/resources/N160.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N200.json` & `ecquote-1.5.1/ecquote/resources/N200.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N256.json` & `ecquote-1.5.1/ecquote/resources/N256.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N320.json` & `ecquote-1.5.1/ecquote/resources/N320.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N400.json` & `ecquote-1.5.1/ecquote/resources/N400.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N640.json` & `ecquote-1.5.1/ecquote/resources/N640.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/N80.json` & `ecquote-1.5.1/ecquote/resources/N80.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/O1280.json` & `ecquote-1.5.1/ecquote/resources/O1280.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/O160.json` & `ecquote-1.5.1/ecquote/resources/O160.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/O320.json` & `ecquote-1.5.1/ecquote/resources/O320.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/O640.json` & `ecquote-1.5.1/ecquote/resources/O640.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/accuracy.yaml` & `ecquote-1.5.1/ecquote/resources/accuracy.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/config.yaml` & `ecquote-1.5.1/ecquote/resources/config.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/epu-based.yaml` & `ecquote-1.5.1/ecquote/resources/epu-based.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/free-open-data.diss` & `ecquote-1.5.1/ecquote/resources/free-open-data.diss`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/free-wmo-essential.diss` & `ecquote-1.5.1/ecquote/resources/free-wmo-essential.diss`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/params.yaml` & `ecquote-1.5.1/ecquote/resources/params.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/pgen-accuracy.yaml` & `ecquote-1.5.1/ecquote/resources/pgen-accuracy.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/reduced-0_125.json` & `ecquote-1.5.1/ecquote/resources/reduced-0_125.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/reduced-0_25.json` & `ecquote-1.5.1/ecquote/resources/reduced-0_25.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/reduced-0_5.json` & `ecquote-1.5.1/ecquote/resources/reduced-0_5.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/regular-0_125.json` & `ecquote-1.5.1/ecquote/resources/regular-0_125.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/representations.yaml` & `ecquote-1.5.1/ecquote/resources/representations.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/sets.yaml` & `ecquote-1.5.1/ecquote/resources/sets.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/wave-mask-reduced.json` & `ecquote-1.5.1/ecquote/resources/wave-mask-reduced.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources/wave-mask-regular.json` & `ecquote-1.5.1/ecquote/resources/wave-mask-regular.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/resources.py` & `ecquote-1.5.1/ecquote/resources.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/rest.py` & `ecquote-1.5.1/ecquote/rest.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/sets.py` & `ecquote-1.5.1/ecquote/sets.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/__init__.py` & `ecquote-1.5.1/ecquote/splitters/__init__.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/canonical.py` & `ecquote-1.5.1/ecquote/splitters/canonical.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/category.py` & `ecquote-1.5.1/ecquote/splitters/category.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/constant.py` & `ecquote-1.5.1/ecquote/splitters/constant.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/destination.py` & `ecquote-1.5.1/ecquote/splitters/destination.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/free_grids.py` & `ecquote-1.5.1/ecquote/splitters/free_grids.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/free_sets.py` & `ecquote-1.5.1/ecquote/splitters/free_sets.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/freebies.py` & `ecquote-1.5.1/ecquote/splitters/freebies.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/group_by.py` & `ecquote-1.5.1/ecquote/splitters/group_by.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/high_frequency.py` & `ecquote-1.5.1/ecquote/splitters/high_frequency.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/repres.py` & `ecquote-1.5.1/ecquote/splitters/repres.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/shgg.py` & `ecquote-1.5.1/ecquote/splitters/shgg.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/subset.py` & `ecquote-1.5.1/ecquote/splitters/subset.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/splitters/validate.py` & `ecquote-1.5.1/ecquote/splitters/validate.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/testing.py` & `ecquote-1.5.1/ecquote/testing.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote/utils.py` & `ecquote-1.5.1/ecquote/utils.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/ecquote.egg-info/PKG-INFO` & `ecquote-1.5.1/ecquote.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecquote
-Version: 1.5.0
+Version: 1.5.1
 Summary: A package to estimate the cost and volume of an ECMWF dissemination feed
 Home-page: https://github.com/ecmwf/ecquote
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ecquote-1.5.0/ecquote.egg-info/SOURCES.txt` & `ecquote-1.5.1/ecquote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecquote-1.5.0/setup.py` & `ecquote-1.5.1/setup.py`

 * *Files identical despite different names*

