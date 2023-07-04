# Comparing `tmp/ecquote-1.4.4.tar.gz` & `tmp/ecquote-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecquote-1.4.4.tar", last modified: Mon Mar  6 13:45:37 2023, max compression
+gzip compressed data, was "ecquote-1.5.0.tar", last modified: Tue Jul  4 14:58:17 2023, max compression
```

## Comparing `ecquote-1.4.4.tar` & `ecquote-1.5.0.tar`

### file list

```diff
@@ -1,95 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:45:37.233395 ecquote-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 13:45:29.000000 ecquote-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-06 13:45:29.000000 ecquote-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-03-06 13:45:37.233395 ecquote-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-06 13:45:29.000000 ecquote-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:45:37.225395 ecquote-1.4.4/ecquote/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/area.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/cart.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/costing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/grib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/landsea.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/landsea_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/landsea_mask_reduced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/landsea_mask_regular.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/modify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    35542 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/repres.py
--rw-r--r--   0 runner    (1001) docker     (123)    16624 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:45:37.233395 ecquote-1.4.4/ecquote/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   106938 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F1280.json
--rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F160.json
--rw-r--r--   0 runner    (1001) docker     (123)    16336 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F200.json
--rw-r--r--   0 runner    (1001) docker     (123)    21410 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F256.json
--rw-r--r--   0 runner    (1001) docker     (123)    26806 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F320.json
--rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F400.json
--rw-r--r--   0 runner    (1001) docker     (123)    53428 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F640.json
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/F80.json
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N128.json
--rw-r--r--   0 runner    (1001) docker     (123)   106600 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N1280.json
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N160.json
--rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N200.json
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N256.json
--rw-r--r--   0 runner    (1001) docker     (123)    26438 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N320.json
--rw-r--r--   0 runner    (1001) docker     (123)    33042 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N400.json
--rw-r--r--   0 runner    (1001) docker     (123)    53086 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N640.json
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/N80.json
--rw-r--r--   0 runner    (1001) docker     (123)   106408 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/O1280.json
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/O160.json
--rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/O320.json
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/O640.json
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/accuracy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/data-values-bands.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/epu-based.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/free-open-data.diss
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/free-wmo-essential.diss
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/freebies.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    71731 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/pgen-accuracy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    42393 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/reduced-0_125.json
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/reduced-0_25.json
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/reduced-0_5.json
--rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/regular-0_125.json
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/representations.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    24762 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/sets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/volume-bands.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   311505 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/wave-mask-reduced.json
--rw-r--r--   0 runner    (1001) docker     (123)   340586 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources/wave-mask-regular.json
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/sets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:45:37.233395 ecquote-1.4.4/ecquote/splitters/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/canonical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/destination.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/free_grids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/free_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/freebies.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/group_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/high_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/leg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/repres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/shgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/subset.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/splitters/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-06 13:45:29.000000 ecquote-1.4.4/ecquote/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 13:45:37.229395 ecquote-1.4.4/ecquote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-03-06 13:45:37.000000 ecquote-1.4.4/ecquote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-06 13:45:37.000000 ecquote-1.4.4/ecquote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 13:45:37.000000 ecquote-1.4.4/ecquote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 13:45:37.000000 ecquote-1.4.4/ecquote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-06 13:45:37.000000 ecquote-1.4.4/ecquote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-06 13:45:37.000000 ecquote-1.4.4/ecquote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 13:45:37.000000 ecquote-1.4.4/ecquote.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 13:45:37.233395 ecquote-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-06 13:45:29.000000 ecquote-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.313237 ecquote-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 14:58:06.000000 ecquote-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-04 14:58:06.000000 ecquote-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-04 14:58:17.309237 ecquote-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-04 14:58:06.000000 ecquote-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.301237 ecquote-1.5.0/ecquote/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8104 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/area.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7794 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/cart.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27460 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/costing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4866 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/grib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8211 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea_fixed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2014 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea_mask_reduced.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/landsea_mask_regular.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/mars.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7996 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/matching.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2530 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/modify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5650 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35542 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/repres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16707 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.309237 ecquote-1.5.0/ecquote/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106938 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F1280.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13076 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F160.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16336 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F200.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21410 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F256.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26806 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F320.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33394 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F400.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53428 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F640.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6566 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/F80.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10470 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N128.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106600 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N1280.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13048 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N160.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16308 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N200.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20992 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N256.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26438 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N320.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33042 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N400.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53086 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N640.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6540 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/N80.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106408 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O1280.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13036 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O160.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26276 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O320.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52898 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/O640.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5972 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/accuracy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/data-values-bands.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2055 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/epu-based.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7067 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/free-open-data.diss
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3910 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/free-wmo-essential.diss
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71731 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/params.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1997 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/pgen-accuracy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42393 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/reduced-0_125.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20487 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/reduced-0_25.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9898 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/reduced-0_5.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42755 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/regular-0_125.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12384 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/representations.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24461 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/sets.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      137 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/volume-bands.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)   311505 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/wave-mask-reduced.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   340586 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources/wave-mask-regular.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2042 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/rest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1850 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/sets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.309237 ecquote-1.5.0/ecquote/splitters/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/canonical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/constant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/destination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      932 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/free_grids.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9463 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/free_sets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2614 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/freebies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/group_by.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2555 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/high_frequency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/repres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/shgg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1377 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/subset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/splitters/validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/testing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3883 2023-07-04 14:58:06.000000 ecquote-1.5.0/ecquote/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:58:17.305237 ecquote-1.5.0/ecquote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:58:17.000000 ecquote-1.5.0/ecquote.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:58:17.313237 ecquote-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-04 14:58:06.000000 ecquote-1.5.0/setup.py
```

### Comparing `ecquote-1.4.4/LICENSE` & `ecquote-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/PKG-INFO` & `ecquote-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecquote
-Version: 1.4.4
+Version: 1.5.0
 Summary: A package to estimate the cost and volume of an ECMWF dissemination feed
 Home-page: https://github.com/ecmwf/ecquote
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ecquote-1.4.4/README.md` & `ecquote-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/__main__.py` & `ecquote-1.5.0/ecquote/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,18 @@
     parser.add_argument("--max-charge-high-frequency", type=int)
 
     parser.add_argument("-X", "--experimental", action="store_true")
     parser.add_argument("--commercial", action="store_true")
     parser.add_argument("--non-commercial", action="store_false", dest="commercial")
     parser.set_defaults(commercial=None)
 
+    parser.add_argument(
+        "--unique", action="store_true", help="Generate unique mars requests"
+    )
+
     parser.add_argument("-r", "--request")
     parser.add_argument("files", metavar="FILES-OR-DIRECTORIES", type=str, nargs="*")
     ARGS = parser.parse_args()
 
     level = logging.ERROR
 
     if ARGS.warnings:
@@ -245,14 +249,18 @@
         cart.who_uses(ARGS.who_uses)
         exit(0)
 
     if ARGS.requests:
         cart.dump_requests()
         exit(0)
 
+    if ARGS.unique:
+        cart.unique()
+        exit(0)
+
     if ARGS.statistics:
         cart.statistics()
         exit(0)
 
     if ARGS.number_of_points:
         print(cart.requests[0].repres.number_of_points())
         exit(0)
```

### Comparing `ecquote-1.4.4/ecquote/area.py` & `ecquote-1.5.0/ecquote/area.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/cart.py` & `ecquote-1.5.0/ecquote/cart.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 import itertools
+import json
 import logging
 import os
 from collections import defaultdict
 
 from .costing import costing
 from .parser import parse_request_file, parse_request_string
 from .request import Request, RequestList
@@ -198,14 +199,36 @@
 
     def dump_requests(self, **kwargs):
         all_keys = set()
         for r in self.requests:
             r.dump(all_keys, **kwargs)
             print(**kwargs)  # An extra line for the perl
 
+    def unique(self, **kwargs):
+        seen = set()
+        for r in self.requests:
+            for s in r.unique(
+                ignore=(
+                    "class",
+                    "time",
+                    # "stream",
+                    # "type",
+                    "expver",
+                    "number",
+                    "domain",
+                    "direction",
+                    "frequency",
+                    "step",
+                    "use",
+                )
+            ):
+                if s not in seen:
+                    print(json.dumps(s))
+                    seen.add(s)
+
     def frequency(self):
         f = list(set(r.frequency() for r in self.requests))
         # assert len(f) == 1, f
         return min(f)
 
     def dates(self):
         f = list(set(r.dates() for r in self.requests))
```

### Comparing `ecquote-1.4.4/ecquote/costing.py` & `ecquote-1.5.0/ecquote/costing.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
             A = request.factor_A()
             if request.is_wave():
                 landsea = request.land_sea_ratio()
             else:
                 landsea = 1
 
             R = request.factor_R(self.reference_grid)
-            frequency = request.frequency()
+            frequency = request.chargeable_frequency()
             LOG.debug("EPUs for %s", request)
             LOG.debug(
                 "B=%s D=%s E=%s A=%s R=%s V=%s M=%s number_of_chargeable_items=%s frequency=%s landsea=%s free=%s",
                 B,
                 D,
                 E,
                 A,
```

### Comparing `ecquote-1.4.4/ecquote/grib.py` & `ecquote-1.5.0/ecquote/grib.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/grid.py` & `ecquote-1.5.0/ecquote/grid.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/landsea.py` & `ecquote-1.5.0/ecquote/landsea.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/landsea_fixed.py` & `ecquote-1.5.0/ecquote/landsea_fixed.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/landsea_mask_reduced.py` & `ecquote-1.5.0/ecquote/landsea_mask_reduced.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/landsea_mask_regular.py` & `ecquote-1.5.0/ecquote/landsea_mask_regular.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/mars.py` & `ecquote-1.5.0/ecquote/mars.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/matching.py` & `ecquote-1.5.0/ecquote/matching.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/modify.py` & `ecquote-1.5.0/ecquote/modify.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/parser.py` & `ecquote-1.5.0/ecquote/parser.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/repres.py` & `ecquote-1.5.0/ecquote/repres.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/request.py` & `ecquote-1.5.0/ecquote/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 import datetime
+import itertools
 import logging
 from collections import defaultdict
 
 from .landsea import land_sea_ratio
 from .matching import Matcher
 from .repres import repres
 from .resources import config, resource
-from .utils import cached_method, log_warning_once, plural
+from .utils import cached_method, plural
 
 LOG = logging.getLogger(__name__)
 
 wave_streams = set(config("wave_streams"))
 ml_matcher = Matcher("representations", lambda _, model_levels, **kwargs: model_levels)
 
 
@@ -162,75 +163,40 @@
             result.update(g)
         return result
 
     @cached_method
     def frequency(self):
         use = tuple(sorted(self.use.get("use", [])))
 
-        def default():
+        if len(use) == 0:
             return self.subset.frequency
 
-        def daily():
-            # assert self.subset.frequency == 365, (self.subset, self.subset.frequency)
-
-            if self.subset.frequency != 365:
-                log_warning_once(
-                    LOG,
-                    "Expecting frequency 365 for subset %s, got %s (%s)",
-                    self.subset.name,
-                    self.subset.frequency,
-                    self,
-                )
-
+        if "bc" in use:
+            assert len(use) == 1, use
             return self.subset.frequency
 
-        def weekly():
-            if self.subset.frequency != 104:
-                log_warning_once(
-                    LOG,
-                    "Keyword use=%s is ignored for subset %s %s (%s)",
-                    "/".join(use),
-                    self.subset.name,
-                    self.subset.frequency,
-                    self,
-                )
-                return self.subset.frequency
-            return 52
-
-        def byweekly():
-            if self.subset.frequency != 104:
-                log_warning_once(
-                    LOG,
-                    "Keyword use=%s is ignored for subset %s %s (%s)",
-                    "/".join(use),
-                    self.subset.name,
-                    self.subset.frequency,
-                    self,
-                )
-                return self.subset.frequency
-            return 104
-
-        def monthly():
-            # Here so we can test legacy requests
-            log_warning_once(
-                LOG,
-                "Keyword use=monthly is ignored for subset %s (%s)",
-                self.subset.name,
-                self,
-            )
-            return self.subset.frequency
-
-        return {
-            tuple(): default,
-            ("bc",): daily,
-            ("monday", "thursday"): byweekly,
-            ("monday",): weekly,
-            ("thursday",): weekly,
-            ("monthly",): monthly,
-        }[use]()
+        for day in use:
+            assert day in (
+                "monday",
+                "tuesday",
+                "wednesday",
+                "thursday",
+                "friday",
+                "saturday",
+                "sunday",
+            ), use
+
+        return 52 * len(use)
+
+    @cached_method
+    def chargeable_frequency(self):
+        frequency = self.frequency()
+        if self.subset.ic_frequency is not None:
+            frequency = min(frequency, self.subset.ic_frequency)
+        return frequency
 
     @cached_method
     def number_of_fields(self):
         debug = LOG.isEnabledFor(logging.DEBUG)
         count = 1
         counts = {}
         for k, v in self.fields.items():
@@ -357,14 +323,26 @@
                 continue
             s.update(r)
 
     def sample_mars_request(self):
         date = datetime.datetime.utcnow() - datetime.timedelta(days=1)
         date = date.date()
 
+        # https://confluence.ecmwf.int/display/PGEN/ENS-extended+weekly+means+in+48r1#ENSextendedweeklymeansin48r1-MondaytoSunday
+
+        DOW = [
+            ("0-168", "168-336", "336-504", "504-672", "672-840", " 840-1008"),
+            ("144-312", "312-480", "480-648", "648-816", "816-984"),
+            ("120-288", "288-456", "456-624", "624-792", "792-960"),
+            ("96-264", "264-432", "432-600", "600-768", "768-936", "936-1104 "),
+            ("72-240", "240-408," "408-576", "576-744", "744-912", "912-1080"),
+            ("48-216", "216-384", "384-552", "552-720", "720-888", "888-1056"),
+            ("24-192", "192-360", "360-528", "528-696", "696-864", "864-1032"),
+        ]
+
         r = {k: v[0] for k, v in self.fields.items()}
         r.update(self.use)
         r.setdefault("levtype", "off")
 
         if (r["stream"], r["type"], r["levtype"]) in (
             ("scda", "an", "pv"),
             ("scda", "an", "pt"),
@@ -373,47 +351,56 @@
             r["stream"] = "oper"
 
         if (r["stream"], r["type"], r["levtype"]) in (("enfo", "cs", "pl"),):
             pass
         elif (r["stream"], r["type"], r["levtype"]) in (
             ("enfo", "cf", "ml"),
             ("enfo", "pf", "ml"),
-            ("efov", "cf", "ml"),
-            ("efov", "pf", "ml"),
+            ("eefo", "cf", "ml"),
+            ("eefo", "pf", "ml"),
         ):
             # Not in MARS
             r["param"] = "q/z"
         else:
             # Not all param avalailable at all levels
             if r["levtype"] not in ("sfc", "off"):
                 if r["type"] not in ("an", "fc", "cf", "pf"):
                     r["levelist"] = "all"
                 r["param"] = "all"
 
         if r.get("use") == "bc":
             del r["use"]
 
-        if r.get("use") in ("monday", "thursday", "monthly") or r.get("stream") in (
-            "efov",
+        if r.get("use") or r.get("stream") in (
             "efhs",
             "enfh",
             "enwh",
+            "eefh",
+            "eefo",
         ):
-            while date.weekday() not in (0, 3):
+            dow = 0  # Monday
+            if r.get("stream") == "eefo":
+                s = r.get("step").split("/")[0]
+                for i, d in enumerate(DOW):
+                    if s in d:
+                        dow = i
+
+            while date.weekday() not in (dow,):
                 date = date - datetime.timedelta(days=1)
             r.pop("use", None)
 
+        # print('========= DATE =====', date,date.weekday(), file=sys.stderr)
+
         if r.get("system"):
             # Seasonal run on the first
             date = datetime.date(date.year, date.month, 1)
 
-        r.pop("leg", None)
         assert "use" not in r, r["use"]
 
-        if r["stream"] in ("enfh", "enwh"):  # TODO: add to config
+        if r["stream"] in ("enfh", "enwh", "eefh", "weeh"):  # TODO: add to config
             hdate = datetime.date(date.year - 5, date.month, date.day)
             r["hdate"] = hdate.isoformat()
             r["levtype"] = "sfc"
 
         if "step" in self.subset.mars:
             r["step"] = "/".join(set(str(x) for x in self.subset.mars["step"]))
             r["time"] = "0/12"
@@ -565,14 +552,25 @@
                 continue
 
             v = "/".join(str(x) for x in v)
             t.append(f"{k}={v}")
         print(",\n".join(t), **kwargs)
         print(**kwargs)
 
+    def unique(self, ignore=()):
+        s = dict(self.fields)
+        s.pop("dataset", None)
+        for i in ignore:
+            s.pop(i, None)
+
+        keys, values = zip(*s.items())
+        for p in (dict(zip(keys, v)) for v in itertools.product(*values)):
+            p.update(self.postproc)
+            yield tuple(p.items())
+
     def __eq__(self, other):
         return self._groups == other._groups
 
     def __hash__(self):
         h = tuple((k, hash(tuple(v.items()))) for k, v in self._groups.items())
         return hash(h)
```

### Comparing `ecquote-1.4.4/ecquote/resources/F1280.json` & `ecquote-1.5.0/ecquote/resources/F1280.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/F160.json` & `ecquote-1.5.0/ecquote/resources/F160.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/F200.json` & `ecquote-1.5.0/ecquote/resources/F200.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/F256.json` & `ecquote-1.5.0/ecquote/resources/F256.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/F320.json` & `ecquote-1.5.0/ecquote/resources/F320.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/F400.json` & `ecquote-1.5.0/ecquote/resources/F400.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/F640.json` & `ecquote-1.5.0/ecquote/resources/F640.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/F80.json` & `ecquote-1.5.0/ecquote/resources/F80.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N128.json` & `ecquote-1.5.0/ecquote/resources/N128.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N1280.json` & `ecquote-1.5.0/ecquote/resources/N1280.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N160.json` & `ecquote-1.5.0/ecquote/resources/N160.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N200.json` & `ecquote-1.5.0/ecquote/resources/N200.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N256.json` & `ecquote-1.5.0/ecquote/resources/N256.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N320.json` & `ecquote-1.5.0/ecquote/resources/N320.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N400.json` & `ecquote-1.5.0/ecquote/resources/N400.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N640.json` & `ecquote-1.5.0/ecquote/resources/N640.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/N80.json` & `ecquote-1.5.0/ecquote/resources/N80.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/O1280.json` & `ecquote-1.5.0/ecquote/resources/O1280.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/O160.json` & `ecquote-1.5.0/ecquote/resources/O160.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/O320.json` & `ecquote-1.5.0/ecquote/resources/O320.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/O640.json` & `ecquote-1.5.0/ecquote/resources/O640.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/accuracy.yaml` & `ecquote-1.5.0/ecquote/resources/accuracy.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/config.yaml` & `ecquote-1.5.0/ecquote/resources/config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -72,35 +72,33 @@
 # The 'a' version are a guess and need checking
 
 spherical_harmonics:
   param: [d, etadot, lnsp, r, t, u, v, vo, w, z, gh, da, etadota, lnspa, ra, ta, ua, va, voa, wa, za, gha]
   levtype: [ml, pl, pt, pv]
 ##############################################################################
 
-hindcast_streams: [enfh, enwh]
+hindcast_streams: [enfh, enwh, eehs, weeh, eefh, efhs, wees, wehs]
 hindcast_dates: 20
 
 high_frequency_streams: [scda, scwv]
 
 seasonal_streams: [mmsf, wasf]
 
 wave_streams:
 - wave
 - scwv
 - waef
 - swmm
 - enwh
 - wasf
+- weef
+- weeh
+- wees
+- wehs
 
-need_leg:
-- enfo
-- waef
-- efov
-# - enfh
-# - enwh
 
 constant_fields:
 - levtype: sfc
   param: [lsm, z, wmb, gh, fsr, aluvd, aluvp, anid, anip, anor, cl, cvh, cvl, dl, isor, slor, sdor, laihv, lailv, slt, tvh, tvl]
 - levtype: ml
   param: [z, gh, lnsp]
 #################
@@ -129,17 +127,17 @@
 
 # Modification rules
 modify: null
 
 # Group-by option
 group-by: null
 
-max-charge-core: 100000
-max-charge-high-frequency: 108000
-epu-price: 0.5
+max-charge-core: 70000
+max-charge-high-frequency: 78000
+epu-price: 0.25
 
 # Destination mode, look for XXX:XX
 destinations: False
 
 experimental: False
 commercial: null
```

### Comparing `ecquote-1.4.4/ecquote/resources/epu-based.yaml` & `ecquote-1.5.0/ecquote/resources/epu-based.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,18 @@
   E: 1.4
   D: 1
   M: 1
 VI-v-d:
   E: 1.4
   D: 1
   M: 1
+VI-v-e:
+  E: 1.4
+  D: 1
+  M: 1
 VI-vi-a:
   E: 1
   D: 1
   M: 1
 VI-vi-b:
   E: 1
   D: 1
```

### Comparing `ecquote-1.4.4/ecquote/resources/free-open-data.diss` & `ecquote-1.5.0/ecquote/resources/free-open-data.diss`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/free-wmo-essential.diss` & `ecquote-1.5.0/ecquote/resources/free-wmo-essential.diss`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/params.yaml` & `ecquote-1.5.0/ecquote/resources/params.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/pgen-accuracy.yaml` & `ecquote-1.5.0/ecquote/resources/pgen-accuracy.yaml`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/reduced-0_125.json` & `ecquote-1.5.0/ecquote/resources/reduced-0_125.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/reduced-0_25.json` & `ecquote-1.5.0/ecquote/resources/reduced-0_25.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/reduced-0_5.json` & `ecquote-1.5.0/ecquote/resources/reduced-0_5.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/regular-0_125.json` & `ecquote-1.5.0/ecquote/resources/regular-0_125.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/representations.yaml` & `ecquote-1.5.0/ecquote/resources/representations.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -48,25 +48,25 @@
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pl
     stream: scda
-    type: an
+    type: fc
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pl
     stream: scda
-    type: fc
+    type: an
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
@@ -78,27 +78,27 @@
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: ml
-    stream: scda
-    type: fc
+    stream: oper
+    type: an
   model_levels: 137
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: ml
-    stream: oper
-    type: an
+    stream: scda
+    type: fc
   model_levels: 137
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
@@ -112,85 +112,85 @@
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pv
     stream: oper
-    type: an
+    type: fc
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pv
-    stream: oper
+    stream: scda
     type: fc
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pv
-    stream: scda
-    type: fc
+    stream: oper
+    type: an
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
-    levtype: pt
-    stream: oper
-    type: fc
+    levtype: pv
+    stream: scda
+    type: an
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pt
     stream: oper
-    type: an
+    type: fc
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pt
-    stream: scda
-    type: fc
+    stream: oper
+    type: an
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
-    levtype: pv
+    levtype: pt
     stream: scda
     type: an
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: pt
     stream: scda
-    type: an
+    type: fc
   repres:
     gaussian: O1280
     resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
@@ -204,317 +204,256 @@
     stream: wave
     type: fc
   repres:
     reduced_ll: 0.125
     type: reduced_ll
 - mars:
     levtype: sfc
-    stream: scwv
-    type: fc
+    stream: wave
+    type: an
   repres:
     reduced_ll: 0.125
     type: reduced_ll
 - mars:
     levtype: sfc
-    stream: wave
-    type: an
+    stream: scwv
+    type: fc
   repres:
     reduced_ll: 0.125
     type: reduced_ll
 - mars:
     levtype: sfc
     stream: scwv
     type: an
   repres:
     reduced_ll: 0.125
     type: reduced_ll
 - mars:
-    dataset: III-i-a
     levtype: sfc
     stream: enfo
     type: pf
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
-    dataset: III-i-a-cf
     levtype: sfc
     stream: enfo
     type: cf
   repres:
-    gaussian: O640
+    gaussian: O1280
+    type: reduced_gg
+- mars:
+    levtype: sfc
+    stream: enfh
+    type: pf
+  repres:
+    gaussian: O1280
+    type: reduced_gg
+- mars:
+    levtype: sfc
+    stream: enfh
+    type: cf
+  repres:
+    gaussian: O1280
     type: reduced_gg
 - mars:
-    dataset: III-i-b
     levtype: pl
     stream: enfo
     type: pf
   repres:
-    gaussian: O640
-    resol: 639
+    gaussian: O1280
+    resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
-    dataset: III-i-b-cf
     levtype: pl
     stream: enfo
     type: cf
   repres:
-    gaussian: O640
-    resol: 639
+    gaussian: O1280
+    resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
+    levtype: pl
+    stream: enfh
+    type: pf
+  repres:
+    gaussian: O1280
+    type: reduced_gg
+- mars:
+    levtype: pl
+    stream: enfh
+    type: cf
+  repres:
+    gaussian: O1280
+    type: reduced_gg
+- mars:
     levtype: ml
     stream: enfo
     type: pf
   model_levels: 137
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
     levtype: ml
     stream: enfo
     type: cf
   model_levels: 137
   repres:
-    gaussian: O640
-    type: reduced_gg
+    gaussian: O1280
+    resol: 1279
+    type:
+    - reduced_gg
+    - sh
 - mars:
     levtype: pv
     stream: enfo
     type: pf
   repres:
-    gaussian: O640
-    resol: 639
+    gaussian: O1280
+    resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
-    dataset: III-i-d
-    levtype: pt
-    stream: enfo
-    type: pf
-  repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
     levtype: pv
     stream: enfo
     type: cf
   repres:
-    gaussian: O640
-    resol: 639
+    gaussian: O1280
+    resol: 1279
     type:
     - reduced_gg
     - sh
 - mars:
-    dataset: III-i-d-cf
-    levtype: pt
-    stream: enfo
-    type: cf
-  repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
     levtype: pl
     stream: enfo
-    type: cr
+    type: cm
   repres:
     grid:
     - 1.5
     - 1.5
     type: regular_ll
 - mars:
     levtype: pl
     stream: enfo
-    type: cm
+    type: cr
   repres:
     grid:
     - 1.5
     - 1.5
     type: regular_ll
 - mars:
-    dataset: III-iii-a
     levtype: sfc
     stream: enfo
     type: ep
   repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: III-iii-b
-    levtype: sfc
-    stream: enfo
-    type: ep
-  repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: III-iii-c
-    levtype: pl
-    stream: enfo
-    type: ep
-  repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
-    dataset: III-iii-d
     levtype: pl
     stream: enfo
     type: ep
   repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: III-iii-e
-    levtype: sfc
-    stream: enfo
-    type: ep
-  repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: III-iii-f
-    levtype: sfc
-    stream: enfo
-    type: ep
-  repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: III-v-a
-    levtype: sfc
-    stream: enfo
-    type: efi
-  repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: III-v-a
-    levtype: sfc
-    stream: enfo
-    type: efic
-  repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
-    dataset: III-v-b
     levtype: sfc
     stream: enfo
     type: efi
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
-    dataset: III-v-b
     levtype: sfc
     stream: enfo
     type: efic
   repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: III-v-c
-    levtype: sfc
-    stream: enfo
-    type: sot
-  repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
-    dataset: III-v-d
     levtype: sfc
     stream: enfo
     type: sot
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
     levtype: sfc
     stream: enfo
     type: em
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
     levtype: pl
     stream: enfo
     type: em
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
     levtype: sfc
     stream: enfo
     type: es
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
     levtype: pl
     stream: enfo
     type: es
   repres:
-    gaussian: O640
+    gaussian: O1280
     type: reduced_gg
 - mars:
-    dataset: IV-i
     levtype: sfc
     stream: waef
     type: pf
   repres:
-    reduced_ll: 0.25
+    reduced_ll: 0.125
     type: reduced_ll
 - mars:
-    dataset: IV-i-cf
     levtype: sfc
     stream: waef
     type: cf
   repres:
-    reduced_ll: 0.25
-    type: reduced_ll
-- mars:
-    dataset: IV-ii-a
-    levtype: sfc
-    stream: waef
-    type: ep
-  repres:
-    reduced_ll: 0.25
+    reduced_ll: 0.125
     type: reduced_ll
 - mars:
-    dataset: IV-ii-b
     levtype: sfc
     stream: waef
     type: ep
   repres:
-    reduced_ll: 0.25
+    reduced_ll: 0.125
     type: reduced_ll
 - mars:
     levtype: sfc
     stream: waef
     type: efi
   repres:
-    reduced_ll: 0.25
+    reduced_ll: 0.125
     type: reduced_ll
 - mars:
     levtype: sfc
     stream: waef
     type: efic
   repres:
-    reduced_ll: 0.25
+    reduced_ll: 0.125
     type: reduced_ll
 - mars:
     levtype: sfc
     stream: waef
     type: sot
   repres:
-    reduced_ll: 0.25
+    reduced_ll: 0.125
     type: reduced_ll
 - mars:
     levtype: sfc
     stream: msmm
     type: em
   repres:
     gaussian: O320
@@ -557,45 +496,38 @@
   repres:
     gaussian: O320
     resol: 319
     type:
     - reduced_gg
     - sh
 - mars:
-    levtype: pt
-    stream: mmsa
-    type: em
+    levtype: sfc
+    stream: msmm
+    type: fcmean
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    levtype: sfc
+    levtype: pv
     stream: msmm
     type: fcmean
   repres:
-    gaussian: O320
-    type: reduced_gg
+    resol: 319
+    type: sh
 - mars:
     levtype: pl
     stream: msmm
     type: fcmean
   repres:
     gaussian: O320
     resol: 319
     type:
     - reduced_gg
     - sh
 - mars:
-    levtype: pv
-    stream: msmm
-    type: fcmean
-  repres:
-    resol: 319
-    type: sh
-- mars:
     levtype: pt
     stream: msmm
     type: fcmean
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
@@ -626,23 +558,14 @@
     levtype: pt
     stream: mmsa
     type: fcmean
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: V-v-a
-    levtype: sfc
-    stream: mmsf
-    type: fc
-  repres:
-    gaussian: O320
-    type: reduced_gg
-- mars:
-    dataset: V-v-b
     levtype: sfc
     stream: mmsf
     type: fc
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
@@ -670,337 +593,254 @@
     levtype: sfc
     stream: wasf
     type: fc
   repres:
     reduced_ll: 0.5
     type: reduced_ll
 - mars:
-    dataset: VI-i-a
     levtype: sfc
-    stream: enfo
+    stream: eefo
     type: taem
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: VI-i-b
     levtype: pl
-    stream: enfo
+    stream: eefo
     type: taem
   repres:
     gaussian: O320
     resol: 319
     type:
     - reduced_gg
     - sh
 - mars:
-    dataset: VI-ii-a
     levtype: sfc
-    stream: enfo
-    type: taem
-  repres:
-    gaussian: O320
-    type: reduced_gg
-- mars:
-    dataset: VI-ii-b
-    levtype: pl
-    stream: enfo
-    type: taem
-  repres:
-    resol: 319
-    type: sh
-- mars:
-    dataset: VI-iii-a
-    levtype: sfc
-    stream: enfo
+    stream: eefo
     type: fcmean
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
     dataset: VI-iii-b
     levtype: pl
-    stream: enfo
+    stream: eefo
     type: fcmean
   repres:
     resol: 319
     type: sh
 - mars:
-    dataset: VI-iv-a
-    levtype: sfc
-    stream: enfo
-    type: fcmean
-  repres:
-    gaussian: O320
-    type: reduced_gg
-- mars:
     dataset: VI-iv-b
     levtype: pl
-    stream: enfo
+    stream: eefo
     type: fcmean
   repres:
     gaussian: O320
     resol: 319
     type:
     - reduced_gg
     - sh
 - mars:
-    dataset: VI-v-a
     levtype: sfc
-    stream: enfo
+    stream: eefo
     type: pf
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: VI-v-a-cf
     levtype: sfc
-    stream: enfo
+    stream: eefo
     type: cf
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: VI-v-b
     levtype: pl
-    stream: enfo
+    stream: eefo
     type: pf
   repres:
     gaussian: O320
     resol: 319
     type:
     - reduced_gg
     - sh
 - mars:
-    dataset: VI-v-b-cf
     levtype: pl
-    stream: enfo
+    stream: eefo
     type: cf
   repres:
     gaussian: O320
     resol: 319
     type:
     - reduced_gg
     - sh
 - mars:
-    dataset: VI-v-c
     levtype: sfc
-    stream: waef
+    stream: weef
     type: pf
   repres:
     reduced_ll: 0.5
     type: reduced_ll
 - mars:
-    dataset: VI-v-c-cf
     levtype: sfc
-    stream: waef
+    stream: weef
     type: cf
   repres:
     reduced_ll: 0.5
     type: reduced_ll
 - mars:
-    dataset: VI-v-d
-    levtype: pt
-    stream: enfo
+    levtype: pv
+    stream: eefo
     type: pf
   repres:
     gaussian: O320
-    type: reduced_gg
+    resol: 319
+    type:
+    - reduced_gg
+    - sh
 - mars:
-    dataset: VI-v-d-cf
-    levtype: pt
-    stream: enfo
+    levtype: pv
+    stream: eefo
     type: cf
   repres:
     gaussian: O320
-    type: reduced_gg
+    resol: 319
+    type:
+    - reduced_gg
+    - sh
 - mars:
-    dataset: VI-vi-a
-    levtype: sfc
-    stream: enfo
-    type: ep
+    levtype: ml
+    stream: eefo
+    type: pf
+  model_levels: 137
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: VI-vi-b
-    levtype: sfc
-    stream: enfo
-    type: ep
+    levtype: ml
+    stream: eefo
+    type: cf
+  model_levels: 137
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
     levtype: sfc
-    stream: enfo
-    type: pd
+    stream: eefo
+    type: ep
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
     levtype: pl
-    stream: enfo
+    stream: eefo
     type: pd
   repres:
     gaussian: O160
     type: reduced_gg
 - mars:
     levtype: sfc
-    stream: enfo
-    type: pb
+    stream: eefo
+    type: pd
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: VI-vii-a
     levtype: sfc
-    step:
-    - 264-432
-    - 0-168
-    - 840-1008
-    - 936-1104
-    - 432-600
-    - 96-264
-    - 168-336
-    - 768-936
-    - 504-672
-    - 672-840
-    - 600-768
-    - 336-504
-    stream: enfo
-    type: efi
+    stream: eefo
+    type: pb
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: VI-vii-a
     levtype: sfc
-    step:
-    - 240-360
-    - 0-360
-    stream: enfo
+    stream: eefo
     type: efi
   repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    dataset: VI-vii-b
-    levtype: sfc
-    step:
-    - 264-432
-    - 0-168
-    - 840-1008
-    - 936-1104
-    - 432-600
-    - 96-264
-    - 168-336
-    - 768-936
-    - 504-672
-    - 672-840
-    - 600-768
-    - 336-504
-    stream: enfo
-    type: sot
-  repres:
     gaussian: O320
     type: reduced_gg
 - mars:
-    dataset: VI-vii-b
     levtype: sfc
-    step:
-    - 240-360
-    - 0-360
-    stream: enfo
+    stream: eefo
     type: sot
   repres:
-    gaussian: O640
+    gaussian: O320
     type: reduced_gg
 - mars:
     levtype: sfc
-    stream: efhs
+    stream: eehs
     type: taem
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
     levtype: pl
-    stream: efhs
+    stream: eehs
     type: taem
   repres:
     gaussian: O320
     resol: 319
     type:
     - reduced_gg
     - sh
 - mars:
     levtype: sfc
-    stream: enfh
+    stream: eefh
     type: fcmean
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
     levtype: pl
-    stream: enfh
+    stream: eefh
     type: fcmean
   repres:
     gaussian: O320
-    type: reduced_gg
-- mars:
-    levtype: sfc
-    stream: efov
-    type: cf
-  repres:
-    gaussian: O320
-    type: reduced_gg
+    resol: 319
+    type:
+    - reduced_gg
+    - sh
 - mars:
     levtype: sfc
-    stream: efov
+    stream: eefh
     type: pf
   repres:
     gaussian: O320
     type: reduced_gg
 - mars:
     levtype: sfc
-    stream: enfh
-    type: pf
-  repres:
-    gaussian: O640
-    type: reduced_gg
-- mars:
-    levtype: sfc
-    stream: enfh
+    stream: eefh
     type: cf
   repres:
-    gaussian: O640
+    gaussian: O320
     type: reduced_gg
 - mars:
     levtype: pl
-    stream: enfh
+    stream: eefh
     type: cf
   repres:
-    gaussian: O640
+    gaussian: O320
     type: reduced_gg
 - mars:
     levtype: pl
-    stream: enfh
+    stream: eefh
     type: pf
   repres:
-    gaussian: O640
+    gaussian: O320
     type: reduced_gg
 - mars:
     levtype: sfc
-    stream: enwh
+    stream: weeh
     type: cf
   repres:
     reduced_ll: 0.5
     type: reduced_ll
 - mars:
     levtype: sfc
-    stream: enwh
+    stream: weeh
     type: pf
   repres:
     reduced_ll: 0.5
     type: reduced_ll
 - mars:
     type: wp
   repres:
```

### Comparing `ecquote-1.4.4/ecquote/resources/sets.yaml` & `ecquote-1.5.0/ecquote/resources/sets.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,239 +1,316 @@
 I-i-a:
   description: Single level
+  frequency: 365
   mars:
+    levtype: sfc
     stream:
     - oper
     - scda
     type:
     - an
     - fc
-    levtype: sfc
   set: I
   subset: I-i
-  frequency: 365
 I-i-b:
   description: Pressure levels
+  frequency: 365
   mars:
+    levtype: pl
     stream:
     - oper
     - scda
     type:
     - an
     - fc
-    levtype: pl
   set: I
   subset: I-i
-  frequency: 365
 I-i-c:
   description: Model levels
+  frequency: 365
   mars:
+    levtype: ml
     stream:
     - oper
     - scda
     type:
     - an
     - fc
-    levtype: ml
   set: I
   subset: I-i
-  frequency: 365
 I-i-d:
   description: Potential vorticity levels
+  frequency: 365
   mars:
+    levtype:
+    - pt
+    - pv
     stream:
     - oper
     - scda
     type:
     - an
     - fc
-    levtype:
-    - pv
-    - pt
   set: I
   subset: I-i
+I-i-e:
+  description: Snow depth levels
   frequency: 365
+  mars:
+    levtype:
+    - sol
+    stream:
+    - oper
+    - scda
+    type:
+    - an
+    - fc
+  set: I
+  subset: I-i
 I-ii:
   description: Time series of weather parameters
+  frequency: 365
   mars:
     stream:
     - oper
     - scda
     type: wp
   set: I
   subset: I-ii
-  frequency: 365
 I-iii:
   description: Tropical cyclone tracks
+  frequency: 365
   mars:
     stream:
     - oper
     - scda
     type: tf
   set: I
   subset: I-iii
-  frequency: 365
 I-iv:
   description: Simulated Satellite Images
+  frequency: 365
   mars:
     stream:
     - oper
     - scda
     type: ssd
   set: I
   subset: I-iv
-  frequency: 365
 II-i:
   description: High RESolution WAve Model (HRES-WAM)
+  frequency: 365
   mars:
+    levtype: sfc
     stream:
-    - wave
     - scwv
+    - wave
     type:
     - an
     - fc
-    levtype: sfc
   set: II
   subset: II-i
-  frequency: 365
 III-i-a:
   description: Atmospheric fields - Single level
-  mars:
+  free_data:
+  - levtype: sfc
     stream: enfo
+    type: cf
+  - levtype: sfc
+    stream: enfh
     type: pf
+  - levtype: sfc
+    stream: enfh
+    type: cf
+  frequency: 365
+  mars:
     levtype: sfc
-    leg: 1
+    stream: enfo
+    type: pf
   set: III
   subset: III-i
-  free_data:
-  - stream: enfo
-    type: cf
-    levtype: sfc
-  - stream: oper
-    type: fc
-    levtype: sfc
-  frequency: 365
 III-i-a-cf:
+  description: Free set with III-i-a
+  free_with: III-i-a
+  frequency: 365
   mars:
+    levtype: sfc
     stream: enfo
     type: cf
-    levtype: sfc
-    leg: 1
-  description: Free set with III-i-a
   set: III
   subset: III-i
+III-i-a-hf:
+  description: Free set with III-i-a
   free_with: III-i-a
-  frequency: 365
+  frequency: 104
+  mars:
+    levtype: sfc
+    stream: enfh
+    type:
+    - cf
+    - pf
+  set: III
+  subset: III-i
 III-i-b:
   description: Atmospheric fields - Pressure levels
-  mars:
+  free_data:
+  - levtype: pl
     stream: enfo
+    type: cf
+  - levtype: pl
+    stream: enfh
     type: pf
+  - levtype: pl
+    stream: enfh
+    type: cf
+  frequency: 365
+  mars:
     levtype: pl
-    leg: 1
+    stream: enfo
+    type: pf
   set: III
   subset: III-i
-  free_data:
-  - stream: enfo
-    type: cf
-    levtype: pl
-  - stream: oper
-    type: fc
-    levtype: pl
-  frequency: 365
 III-i-b-cf:
+  description: Free set with III-i-b
+  free_with: III-i-b
+  frequency: 365
   mars:
+    levtype: pl
     stream: enfo
     type: cf
-    levtype: pl
-    leg: 1
-  description: Free set with III-i-b
   set: III
   subset: III-i
+III-i-b-hf:
+  description: Free set with III-i-b
   free_with: III-i-b
-  frequency: 365
+  frequency: 104
+  mars:
+    levtype: pl
+    stream: enfh
+    type:
+    - cf
+    - pf
+  set: III
+  subset: III-i
 III-i-c:
   description: Atmospheric fields - Model levels
-  mars:
+  free_data:
+  - levtype: ml
     stream: enfo
+    type: cf
+  - levtype: ml
+    stream: enfh
     type: pf
+  frequency: 365
+  mars:
     levtype: ml
+    stream: enfo
+    type: pf
   set: III
   subset: III-i
-  free_data:
-  - stream: enfo
-    type: cf
-    levtype: ml
-  - stream: oper
-    type: fc
-    levtype: ml
-  frequency: 365
 III-i-c-cf:
+  description: Free set with III-i-c
+  free_with: III-i-c
+  frequency: 365
   mars:
+    levtype: ml
     stream: enfo
     type: cf
-    levtype: ml
-  description: Free set with III-i-c
   set: III
   subset: III-i
+III-i-c-hf:
+  description: Free set with III-i-c
   free_with: III-i-c
-  frequency: 365
-III-i-d:
-  description: Atmospheric fields - Potential vorticity levels
+  frequency: 104
   mars:
-    stream: enfo
-    type: pf
-    levtype:
-    - pv
-    - pt
-    leg: 1
+    levtype: ml
+    stream: enfh
+    type:
+    - cf
+    - pf
   set: III
   subset: III-i
+III-i-d:
+  description: Atmospheric fields - Potential vorticity levels
   free_data:
-  - stream: enfo
+  - levtype:
+    - pv
+    - pt
+    stream: enfo
     type: cf
-    levtype:
+  - levtype:
     - pv
     - pt
-  - stream: oper
+    stream: oper
     type: fc
-    levtype:
+  - levtype:
+    - pv
+    - pt
+    stream: enfh
+    type: pf
+  - levtype:
     - pv
     - pt
+    stream: enfh
+    type: cf
   frequency: 365
+  mars:
+    levtype:
+    - pt
+    - pv
+    stream: enfo
+    type: pf
+  set: III
+  subset: III-i
 III-i-d-cf:
+  description: Free set with III-i-d
+  free_with: III-i-d
+  frequency: 365
   mars:
+    levtype:
+    - pt
+    - pv
     stream: enfo
     type: cf
+  set: III
+  subset: III-i
+III-i-d-hf:
+  description: Free set with III-i-d
+  free_with: III-i-d
+  frequency: 104
+  mars:
     levtype:
-    - pv
     - pt
-    leg: 1
-  description: Free set with III-i-d
+    - pv
+    stream: enfh
+    type:
+    - cf
+    - pf
   set: III
   subset: III-i
-  free_with: III-i-d
-  frequency: 365
 III-ii:
   description: Clusters
+  frequency: 365
   mars:
+    levtype: pl
     stream: enfo
     type:
     - cm
     - cr
-    levtype: pl
   set: III
   subset: III-ii
-  frequency: 365
 III-iii-a:
   description: Probabilities - Instantaneous weather events - Single level
+  frequency: 365
   mars:
-    stream: enfo
-    type: ep
     levtype: sfc
+    param:
+    - 10spg10
+    - 10spg15
+    - 2tl273
     step:
     - 12
     - 24
     - 36
     - 48
     - 60
     - 72
@@ -257,355 +334,317 @@
     - 288
     - 300
     - 312
     - 324
     - 336
     - 348
     - 360
-    param:
-    - 10spg10
-    - 10spg15
-    - 2tl273
+    stream: enfo
+    type: ep
   set: III
   subset: III-iii
-  frequency: 365
 III-iii-b:
   description: Probabilities - Averaged  weather events - Single level
+  frequency: 365
   mars:
-    stream: enfo
-    type: ep
     levtype: sfc
-    step:
-    - 120-168
-    - 120-240
-    - 168-240
-    - 240-360
     param:
     - 2tl273
     - tpl01
     - tprg3
     - tprg5
     - tprl1
+    step:
+    - 120-168
+    - 120-240
+    - 168-240
+    - 240-360
+    stream: enfo
+    type: ep
   set: III
   subset: III-iii
-  frequency: 365
 III-iii-c:
   description: Probabilities - Instantaneous weather events - Pressure levels
+  frequency: 365
   mars:
-    stream: enfo
-    type: ep
     levtype: pl
     param:
     - ptsa_gt_1p5stdev
     - ptsa_gt_1stdev
     - ptsa_gt_2stdev
     - ptsa_lt_1p5stdev
     - ptsa_lt_1stdev
     - ptsa_lt_2stdev
     - tag4
     - tag8
     - talm4
     - talm8
+    stream: enfo
+    type: ep
   set: III
   subset: III-iii
-  frequency: 365
 III-iii-d:
   description: Probabilities - Averaged  weather events - Pressure levels
+  frequency: 365
   mars:
-    stream: enfo
-    type: ep
     levtype: pl
     param:
     - tag2
     - talm2
+    stream: enfo
+    type: ep
   set: III
   subset: III-iii
-  frequency: 365
 III-iii-e:
   description: Probabilities - Daily weather events - Single level
+  frequency: 365
   mars:
-    stream: enfo
-    type: ep
     levtype: sfc
-    step:
-    - 0-24
-    - 108-132
-    - 12-36
-    - 120-144
-    - 132-156
-    - 144-168
-    - 156-180
-    - 168-192
-    - 180-204
-    - 192-216
-    - 204-228
-    - 216-240
-    - 228-252
-    - 24-48
-    - 240-264
-    - 252-276
-    - 264-288
-    - 276-300
-    - 288-312
-    - 300-324
-    - 312-336
-    - 324-348
-    - 336-360
-    - 36-60
-    - 48-72
-    - 60-84
-    - 72-96
-    - 84-108
-    - 96-120
     param:
     - 10fgg10
     - 10fgg15
     - 10fgg20
     - 10fgg25
     - tpg1
     - tpg10
     - tpg100
     - tpg20
     - tpg25
     - tpg5
     - tpg50
+    stream: enfo
+    type: ep
   set: III
   subset: III-iii
-  frequency: 365
 III-iii-f:
   description: Probabilities - Tropical cyclone probabilities
+  frequency: 365
   mars:
-    stream: enfo
-    type: ep
     levtype: sfc
-    step:
-    - 120-168
-    - 144-192
-    - 168-216
-    - 192-240
-    - 216-264
-    - 24-72
-    - 240-288
-    - 48-96
-    - 72-120
-    - 96-144
     param:
     - ph
     - ptd
     - pts
+    stream: enfo
+    type: ep
   set: III
   subset: III-iii
-  frequency: 365
 III-iv:
   description: Time series of weather parameters
+  frequency: 365
   mars:
     stream: enfo
     type: wp
   set: III
   subset: III-iv
-  frequency: 365
 III-v-a:
   description: Extreme Forecast Index (EFI) 1-day ranges
+  frequency: 365
   mars:
-    stream: enfo
-    type:
-    - efi
-    - efic
     levtype: sfc
     step:
     - 0-24
-    - 108-132
     - 12-36
-    - 120-144
-    - 132-156
-    - 144-168
-    - 156-180
     - 24-48
     - 36-60
     - 48-72
     - 60-84
     - 72-96
     - 84-108
     - 96-120
+    - 108-132
+    - 120-144
+    - 132-156
+    - 144-168
+    - 156-180
+    stream: enfo
+    type:
+    - efi
+    - efic
   set: III
   subset: III-v
-  frequency: 365
 III-v-b:
+  comment: 240-360 and 0-360 are not in the catalogue
   description: Extreme Forecast Index (EFI) 3, 5 and 10-day ranges
+  frequency: 365
   mars:
-    stream: enfo
-    type:
-    - efi
-    - efic
     levtype: sfc
     step:
+    - 0-72
     - 0-120
     - 0-240
-    - 0-72
-    - 108-180
-    - 108-228
-    - 12-132
+    - 0-360
     - 12-84
-    - 120-192
-    - 132-204
-    - 144-216
-    - 156-228
-    - 24-144
+    - 12-132
     - 24-96
+    - 24-144
     - 36-108
     - 36-156
     - 48-120
     - 48-168
     - 60-132
     - 60-180
     - 72-144
     - 72-192
     - 84-156
     - 84-204
     - 96-168
     - 96-216
+    - 108-180
+    - 108-228
+    - 120-192
+    - 132-204
+    - 144-216
+    - 156-228
+    - 240-360
+    stream: enfo
+    type:
+    - efi
+    - efic
   set: III
   subset: III-v
-  frequency: 365
 III-v-c:
   description: Shift of Tails (SOT) 1-day ranges
+  frequency: 365
   mars:
-    stream: enfo
-    type: sot
     levtype: sfc
     step:
     - 0-24
-    - 108-132
     - 12-36
-    - 120-144
-    - 132-156
-    - 144-168
-    - 156-180
     - 24-48
     - 36-60
     - 48-72
     - 60-84
     - 72-96
     - 84-108
     - 96-120
+    - 108-132
+    - 120-144
+    - 132-156
+    - 144-168
+    - 156-180
+    stream: enfo
+    type: sot
   set: III
   subset: III-v
-  frequency: 365
 III-v-d:
+  comment: 240-360 and 0-360 are not in the catalogue
   description: Shift of Tails (SOT) 3, 5 and 10-day ranges
+  frequency: 365
   mars:
-    stream: enfo
-    type: sot
     levtype: sfc
     step:
+    - 0-72
     - 0-120
     - 0-240
-    - 0-72
-    - 108-180
-    - 108-228
-    - 12-132
+    - 0-360
     - 12-84
-    - 120-192
-    - 132-204
-    - 144-216
-    - 156-228
-    - 24-144
+    - 12-132
     - 24-96
+    - 24-144
     - 36-108
     - 36-156
     - 48-120
     - 48-168
     - 60-132
     - 60-180
     - 72-144
     - 72-192
     - 84-156
     - 84-204
     - 96-168
     - 96-216
+    - 108-180
+    - 108-228
+    - 120-192
+    - 132-204
+    - 144-216
+    - 156-228
+    - 240-360
+    stream: enfo
+    type: sot
   set: III
   subset: III-v
-  frequency: 365
 III-vi-a:
   description: Ensemble means - Single level
+  frequency: 365
   mars:
+    levtype: sfc
     stream: enfo
     type: em
-    levtype: sfc
   set: III
   subset: III-vi
-  frequency: 365
 III-vi-b:
   description: Ensemble means - Pressure levels
+  frequency: 365
   mars:
+    levtype: pl
     stream: enfo
     type: em
-    levtype: pl
   set: III
   subset: III-vi
-  frequency: 365
 III-vii-a:
   description: Ensemble standard deviations - Single level
+  frequency: 365
   mars:
+    levtype: sfc
     stream: enfo
     type: es
-    levtype: sfc
   set: III
   subset: III-vii
-  frequency: 365
 III-vii-b:
   description: Ensemble standard deviations - Pressure levels
+  frequency: 365
   mars:
+    levtype: pl
     stream: enfo
     type: es
-    levtype: pl
   set: III
   subset: III-vii
-  frequency: 365
 III-viii:
   description: Tropical Cyclone tracks
+  frequency: 365
   mars:
     stream: enfo
     type: tf
   set: III
   subset: III-viii
-  frequency: 365
 IV-i:
-  description: Wave fields
-  mars:
+  description: Ensemble Wave fields
+  free_data:
+  - levtype: sfc
     stream: waef
+    type: cf
+  - levtype: sfc
+    stream: enwh
+    type: cf
+  - levtype: sfc
+    stream: enwh
     type: pf
+  frequency: 365
+  mars:
     levtype: sfc
-    leg: 1
+    stream: waef
+    type: pf
   set: IV
   subset: IV-i
-  free_data:
-  - stream: waef
-    type: cf
-    levtype: sfc
-  - stream: wave
-    type: fc
-    levtype: sfc
-  frequency: 365
 IV-i-cf:
+  description: Free set with IV-i
+  free_with: IV-i
+  frequency: 365
   mars:
+    levtype: sfc
     stream: waef
     type: cf
-    levtype: sfc
-    leg: 1
-  description: Free set with IV-i
   set: IV
   subset: IV-i
-  free_with: IV-i
-  frequency: 365
 IV-ii-a:
   description: Probabilities - Instantaneous weather events
+  frequency: 365
   mars:
-    stream: waef
-    type: ep
     levtype: sfc
     step:
     - 12
     - 24
     - 36
     - 48
     - 60
@@ -630,208 +669,207 @@
     - 288
     - 300
     - 312
     - 324
     - 336
     - 348
     - 360
+    stream: waef
+    type: ep
   set: IV
   subset: IV-ii
-  frequency: 365
 IV-ii-b:
   description: Probabilities - Averaged  weather events
+  frequency: 365
   mars:
-    stream: waef
-    type: ep
     levtype: sfc
     step:
     - 120-168
     - 120-240
     - 168-240
     - 240-360
+    stream: waef
+    type: ep
   set: IV
   subset: IV-ii
-  frequency: 365
 IV-iii-a:
   description: Extreme Forecast Index (EFI) 1-day ranges
+  frequency: 365
   mars:
+    levtype: sfc
     stream: waef
     type:
     - efi
     - efic
-    levtype: sfc
   set: IV
   subset: IV-iii
-  frequency: 365
 IV-iii-b:
   description: Shift of Tails (SOT) 1-day ranges
+  frequency: 365
   mars:
+    levtype: sfc
     stream: waef
     type: sot
-    levtype: sfc
   set: IV
   subset: IV-iii
-  frequency: 365
 V-i-a:
   description: Monthly means of ensemble means - Single level
+  frequency: 12
   mars:
-    stream: msmm
-    type: em
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
+    stream: msmm
+    system: 5
+    type: em
   set: V
   subset: V-i
-  frequency: 12
 V-i-b:
   description: Monthly means of ensemble means - Pressure levels
+  frequency: 12
   mars:
-    stream: msmm
-    type: em
     levtype:
     - pl
-    - pv
     - pt
-    system: 5
+    - pv
     method: 1
     origin: ecmf
+    stream: msmm
+    system: 5
+    type: em
   set: V
   subset: V-i
-  frequency: 12
 V-ii-a:
   description: Monthly mean anomalies of ensemble means - Single level
+  frequency: 12
   mars:
-    stream: mmsa
-    type: em
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
+    stream: mmsa
+    system: 5
+    type: em
   set: V
   subset: V-ii
-  frequency: 12
 V-ii-b:
   description: Monthly mean anomalies of ensemble means - Pressure levels
+  frequency: 12
   mars:
-    stream: mmsa
-    type: em
     levtype:
     - pl
     - pt
-    system: 5
     method: 1
     origin: ecmf
+    stream: mmsa
+    system: 5
+    type: em
   set: V
   subset: V-ii
-  frequency: 12
 V-iii-a:
   description: Monthly means of individual ensemble members - Single level
-  mars:
-    stream: msmm
-    type: fcmean
+  free_data:
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
-  set: V
-  subset: V-iii
-  free_data:
     stream: msmm
+    system: 5
     type: em
+  frequency: 12
+  mars:
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
-  frequency: 12
-V-iii-b:
-  description: Monthly means of individual ensemble members - Pressure levels
-  mars:
     stream: msmm
+    system: 5
     type: fcmean
+  set: V
+  subset: V-iii
+V-iii-b:
+  description: Monthly means of individual ensemble members - Pressure levels
+  free_data:
     levtype:
     - pl
     - pv
     - pt
-    system: 5
     method: 1
     origin: ecmf
-  set: V
-  subset: V-iii
-  free_data:
     stream: msmm
+    system: 5
     type: em
+  frequency: 12
+  mars:
     levtype:
     - pl
-    - pv
     - pt
-    system: 5
+    - pv
     method: 1
     origin: ecmf
-  frequency: 12
+    stream: msmm
+    system: 5
+    type: fcmean
+  set: V
+  subset: V-iii
 V-iii-c:
   description: Seasonal forecast wave monthly means
+  frequency: 12
   mars:
-    stream: swmm
-    type: fcmean
     levtype: sfc
-    system: 5
     method: 1
+    stream: swmm
+    system: 5
+    type: fcmean
   set: V
   subset: V-iii
-  frequency: 12
 V-iv-a:
   description: Monthly mean anomalies of individual ensemble members - Single level
-  mars:
-    stream: mmsa
-    type: fcmean
+  free_data:
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
-  set: V
-  subset: V-iv
-  free_data:
     stream: mmsa
+    system: 5
     type: em
+  frequency: 12
+  mars:
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
-  frequency: 12
-V-iv-b:
-  description: Monthly mean anomalies of individual ensemble members - Pressure levels
-  mars:
     stream: mmsa
+    system: 5
     type: fcmean
+  set: V
+  subset: V-iv
+V-iv-b:
+  description: Monthly mean anomalies of individual ensemble members - Pressure levels
+  free_data:
     levtype:
     - pl
     - pt
-    system: 5
     method: 1
     origin: ecmf
-  set: V
-  subset: V-iv
-  free_data:
     stream: mmsa
+    system: 5
     type: em
+  frequency: 12
+  mars:
     levtype:
     - pl
     - pt
-    system: 5
     method: 1
     origin: ecmf
-  frequency: 12
+    stream: mmsa
+    system: 5
+    type: fcmean
+  set: V
+  subset: V-iv
 V-v-a:
   description: Individual forecast runs - 6-hourly - Single level
+  frequency: 12
   mars:
-    stream: mmsf
-    type: fc
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
     param:
     - 10u
     - 10v
     - 2d
     - 2t
@@ -841,24 +879,24 @@
     - sf
     - ssrd
     - sst
     - stl1
     - strd
     - tcc
     - tp
+    stream: mmsf
+    system: 5
+    type: fc
   set: V
   subset: V-v
-  frequency: 12
 V-v-b:
   description: Individual forecast runs - 24-hourly - Single level
+  frequency: 12
   mars:
-    stream: mmsf
-    type: fc
     levtype: sfc
-    system: 5
     method: 1
     origin: ecmf
     param:
     - ci
     - cl
     - cp
     - dl
@@ -896,71 +934,67 @@
     - tclw
     - tco3
     - tcwv
     - tisr
     - tsr
     - ttr
     - z
+    stream: mmsf
+    system: 5
+    type: fc
   set: V
   subset: V-v
-  frequency: 12
 V-v-c:
   description: Individual forecast runs - 12-hourly - Pressure levels
+  frequency: 12
   mars:
-    stream: mmsf
-    type: fc
     levtype: pl
-    system: 5
     method: 1
     origin: ecmf
+    stream: mmsf
+    system: 5
+    type: fc
   set: V
   subset: V-v
-  frequency: 12
 V-v-d:
   description: Individual forecast runs - 12-hourly - Model levels
+  frequency: 12
   mars:
-    stream: mmsf
-    type: fc
     levtype: ml
-    system: 5
     method: 1
     origin: ecmf
+    stream: mmsf
+    system: 5
+    type: fc
   set: V
   subset: V-v
-  frequency: 12
 V-v-e:
   description: Wave seasonal forecast - 24-hourly
+  frequency: 12
   mars:
-    stream: wasf
-    type: fc
     levtype: sfc
-    system: 5
     method: 1
+    stream: wasf
+    system: 5
+    type: fc
   set: V
   subset: V-v
-  frequency: 12
 VI-i-a:
   description: Weekly means of ensemble means - Single level
-  mars:
-    stream: enfo
+  free_data:
+  - levtype: sfc
+    stream: eehs
     type: taem
+  - levtype: sfc
+    stream: eehs
+    type: em
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype: sfc
-    step:
-    - 0-168
-    - 168-336
-    - 264-432
-    - 336-504
-    - 432-600
-    - 504-672
-    - 600-768
-    - 672-840
-    - 768-936
-    - 840-1008
-    - 936-1104
-    - 96-264
     param:
     - 100u
     - 100v
     - 10u
     - 10v
     - 2d
     - 2t
@@ -985,68 +1019,57 @@
     - tciw
     - tclw
     - tcw
     - tcwv
     - tprate
     - tps
     - z
+    stream: eefo
+    type: taem
   set: VI
   subset: VI-i
+VI-i-b:
+  description: Weekly means of ensemble means - Pressure levels
   free_data:
-  - stream: efhs
+  - levtype: pl
+    stream: eehs
     type: taem
-    levtype: sfc
-  - stream: efhs
+  - levtype: pl
+    stream: eehs
     type: em
-    levtype: sfc
-  frequency: 104
-VI-i-b:
-  description: Weekly means of ensemble means - Pressure levels
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: taem
     levtype: pl
     param:
     - gh
     - q
     - strf
     - t
     - u
     - v
     - vp
     - z
+    stream: eefo
+    type: taem
   set: VI
   subset: VI-i
+VI-ii-a:
+  description: Weekly mean anomalies of ensemble means - Single level
   free_data:
-  - stream: efhs
+  - levtype: sfc
+    stream: eehs
     type: taem
-    levtype: pl
-  - stream: efhs
+  - levtype: sfc
+    stream: eehs
     type: em
-    levtype: pl
-  frequency: 104
-VI-ii-a:
-  description: Weekly mean anomalies of ensemble means - Single level
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: taem
     levtype: sfc
-    step:
-    - 0-168
-    - 168-336
-    - 264-432
-    - 336-504
-    - 432-600
-    - 504-672
-    - 600-768
-    - 672-840
-    - 768-936
-    - 840-1008
-    - 936-1104
-    - 96-264
     param:
     - 100ua
     - 100va
     - 10ua
     - 10va
     - 2da
     - 2ta
@@ -1064,39 +1087,52 @@
     - sundara
     - tcca
     - tciwa
     - tclwa
     - tcwa
     - tcwva
     - tpara
+    stream: eefo
+    type: taem
   set: VI
   subset: VI-ii
-  frequency: 104
 VI-ii-b:
   description: Weekly mean anomalies of ensemble means - Pressure levels
-  mars:
-    stream: enfo
+  free_data:
+  - levtype: pl
+    stream: eehs
     type: taem
+  - levtype: pl
+    stream: eehs
+    type: em
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype: pl
     param:
     - gha
     - strfa
     - ta
     - ua
     - va
     - vpota
     - za
+    stream: eefo
+    type: taem
   set: VI
   subset: VI-ii
-  frequency: 104
 VI-iii-a:
   description: Weekly means of individual ensemble members - Single level
-  mars:
-    stream: enfo
+  free_data:
+    levtype: sfc
+    stream: eefh
     type: fcmean
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype: sfc
     param:
     - 100u
     - 100v
     - 10u
     - 10v
     - 2d
@@ -1109,47 +1145,49 @@
     - mx2t6
     - rsn
     - sd
     - stl1
     - tcc
     - tprate
     - z
+    stream: eefo
+    type: fcmean
   set: VI
   subset: VI-iii
-  free_data:
-    stream: enfh
-    type: fcmean
-    levtype: sfc
-  frequency: 104
 VI-iii-b:
   description: Weekly means of individual ensemble members - Pressure levels
-  mars:
-    stream: enfo
+  free_data:
+    levtype: pl
+    stream: eefh
     type: fcmean
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype: pl
     param:
     - gh
     - strf
     - t
     - u
     - v
     - vp
     - z
+    stream: eefo
+    type: fcmean
   set: VI
   subset: VI-iii
-  free_data:
-    stream: enfh
-    type: fcmean
-    levtype: pl
-  frequency: 104
 VI-iv-a:
   description: Weekly mean anomalies of individual ensemble members - Single level
-  mars:
-    stream: enfo
+  free_data:
+    levtype: sfc
+    stream: eefh
     type: fcmean
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype: sfc
     param:
     - 100ua
     - 100va
     - 10ua
     - 10va
     - 2da
@@ -1157,492 +1195,403 @@
     - lsma
     - mn2t6a
     - msla
     - mx2t6a
     - rsna
     - sda
     - sfara
-    - stal1a
+    - stal1
     - sundara
     - tcca
     - tpara
     - za
+    stream: eefo
+    type: fcmean
   set: VI
   subset: VI-iv
-  frequency: 104
 VI-iv-b:
   description: Weekly mean anomalies of individual ensemble members - Pressure levels
-  mars:
-    stream: enfo
+  free_data:
+    levtype: pl
+    stream: eefh
     type: fcmean
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype: pl
     param:
     - gha
     - qa
     - strfa
     - ta
     - ua
     - va
     - vpota
     - za
+    stream: eefo
+    type: fcmean
   set: VI
   subset: VI-iv
-  frequency: 104
 VI-v-a:
   description: Individual forecast runs - 6-hourly - Single level
-  mars:
-    stream: enfo
-    type: pf
-    levtype: sfc
-    leg: 2
-  set: VI
-  subset: VI-v
   free_data:
-  - stream: enfo
+  - levtype: sfc
+    stream: eefo
     type: cf
-    levtype: sfc
-  - stream: efov
-    type: cf
-    levtype: sfc
-  - stream: efov
-    type: pf
-    levtype: sfc
-  - stream: enfh
+  - levtype: sfc
+    stream: eefh
     type: pf
-    levtype: sfc
-  - stream: enfh
+  - levtype: sfc
+    stream: eefh
     type: cf
-    levtype: sfc
-  frequency: 104
-VI-v-a-cf:
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: cf
     levtype: sfc
-    leg: 2
-  description: Free set with VI-v-a
+    stream: eefo
+    type: pf
   set: VI
   subset: VI-v
+VI-v-a-cf:
+  description: Free set with VI-v-a
   free_with: VI-v-a
-  frequency: 104
-VI-v-b:
-  description: Individual forecast runs - 12-hourly - Pressure levels
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: pf
-    levtype: pl
-    leg: 2
+    levtype: sfc
+    stream: eefo
+    type: cf
   set: VI
   subset: VI-v
+VI-v-b:
+  description: Individual forecast runs - 12-hourly - Pressure levels
   free_data:
-  - stream: enfh
+  - levtype: pl
+    stream: eefh
     type: cf
-    levtype: pl
-  - stream: enfh
+  - levtype: pl
+    stream: eefh
     type: pf
-    levtype: pl
-  - stream: enfo
-    type: cf
-    levtype: pl
-  - stream: efov
+  - levtype: pl
+    stream: eefo
     type: cf
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype: pl
-  - stream: efov
+    stream: eefo
     type: pf
-    levtype: pl
-  frequency: 104
+  set: VI
+  subset: VI-v
 VI-v-b-cf:
+  description: Free set with VI-v-b
+  free_with: VI-v-b
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: cf
     levtype: pl
-    leg: 2
-  description: Free set with VI-v-b
+    stream: eefo
+    type: cf
   set: VI
   subset: VI-v
-  free_with: VI-v-b
-  frequency: 104
 VI-v-c:
   description: Individual forecast runs - 6-hourly - wave
-  mars:
-    stream: waef
-    type: pf
-    levtype: sfc
-    leg: 2
-  set: VI
-  subset: VI-v
   free_data:
-  - stream: enwh
+  - levtype: sfc
+    stream: weeh
     type: cf
-    levtype: sfc
-  - stream: enwh
+  - levtype: sfc
+    stream: weeh
     type: pf
-    levtype: sfc
-  - stream: waef
+  - levtype: sfc
+    stream: weef
     type: cf
-    levtype: sfc
-  frequency: 104
-VI-v-c-cf:
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: waef
-    type: cf
     levtype: sfc
-    leg: 2
-  description: Free set with VI-v-c
+    stream: weef
+    type: pf
   set: VI
   subset: VI-v
+VI-v-c-cf:
+  description: Free set with VI-v-c
   free_with: VI-v-c
-  frequency: 104
-VI-v-d:
-  description: Individual forecast runs - 12-hourly - potential vorticity levels
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: pf
-    levtype:
-    - pv
-    - pt
-    leg: 2
+    levtype: sfc
+    stream: weef
+    type: cf
   set: VI
   subset: VI-v
+VI-v-d:
+  description: Individual forecast runs - 12-hourly - potential vorticity levels
   free_data:
-  - stream: enfo
-    type: cf
-    levtype:
+  - levtype:
     - pv
     - pt
-  - stream: efov
+    stream: eefo
     type: cf
+  frequency: 365
+  ic_frequency: 104
+  mars:
     levtype:
-    - pv
     - pt
-  - stream: efov
-    type: pf
-    levtype:
     - pv
-    - pt
-  frequency: 104
+    stream: eefo
+    type: pf
+  set: VI
+  subset: VI-v
 VI-v-d-cf:
+  description: Free set with VI-v-d
+  free_with: VI-v-d
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: cf
     levtype:
-    - pv
     - pt
-    leg: 2
-  description: Free set with VI-v-d
+    - pv
+    stream: eefo
+    type: cf
+  set: VI
+  subset: VI-v
+VI-v-e:
+  comment: Not a real subset
+  description: unsupported
+  frequency: 365
+  ic_frequency: 104
+  mars:
+    levtype: ml
+    stream: eefo
+    type: pf
+  set: V
+  subset: VI-v
+VI-v-e-cf:
+  description: Free set with VI-v-e
+  free_with: VI-v-e
+  frequency: 365
+  ic_frequency: 104
+  mars:
+    levtype: ml
+    stream: eefo
+    type: cf
   set: VI
   subset: VI-v
-  free_with: VI-v-d
-  frequency: 104
 VI-vi-a:
   description: Probabilities - Weekly averaged
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: ep
     levtype: sfc
-    step:
-    - 0-168
-    - 168-336
-    - 264-432
-    - 336-504
-    - 432-600
-    - 504-672
-    - 600-768
-    - 672-840
-    - 768-936
-    - 840-1008
-    - 936-1104
-    - 96-264
     param:
     - 2tag0
     - 2tag1
     - 2tag2
     - 2talm1
     - 2talm2
     - mslag0
     - stag0
+    stream: eefo
+    type: ep
   set: VI
   subset: VI-vi
-  frequency: 104
 VI-vi-b:
   description: Probabilities - Weekly accumulated
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: ep
     levtype: sfc
-    step:
-    - 0-168
-    - 168-336
-    - 264-432
-    - 336-504
-    - 432-600
-    - 504-672
-    - 600-768
-    - 672-840
-    - 768-936
-    - 840-1008
-    - 936-1104
-    - 96-264
     param:
     - tpag0
     - tpag10
     - tpag20
+    stream: eefo
+    type: ep
   set: VI
   subset: VI-vi
-  frequency: 104
 VI-vi-c:
   description: Probabilities - Probability distributions
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: pd
     levtype:
-    - sfc
     - pl
+    - sfc
+    stream: eefo
+    type: pd
   set: VI
   subset: VI-vi
-  frequency: 104
 VI-vi-d:
   description: Probabilities - Probability boundaries
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: pb
     levtype:
-    - sfc
     - pl
+    - sfc
+    stream: eefo
+    type: pb
   set: VI
   subset: VI-vi
-  frequency: 104
 VI-vii-a:
   description: Extreme Forecast Index (EFI)
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
+    levtype: sfc
+    stream: eefo
     type:
     - efi
     - efic
-    levtype: sfc
-    step:
-    - 0-168
-    - 0-360
-    - 168-336
-    - 240-360
-    - 264-432
-    - 336-504
-    - 432-600
-    - 504-672
-    - 600-768
-    - 672-840
-    - 768-936
-    - 840-1008
-    - 936-1104
-    - 96-264
   set: VI
   subset: VI-vii
-  frequency: 104
 VI-vii-b:
   description: Shift of Tails (SOT)
+  frequency: 365
+  ic_frequency: 104
   mars:
-    stream: enfo
-    type: sot
     levtype: sfc
-    step:
-    - 0-168
-    - 0-360
-    - 168-336
-    - 240-360
-    - 264-432
-    - 336-504
-    - 432-600
-    - 504-672
-    - 600-768
-    - 672-840
-    - 768-936
-    - 840-1008
-    - 936-1104
-    - 96-264
+    stream: eefo
+    type: sot
   set: VI
   subset: VI-vii
-  frequency: 104
 X-x-a:
+  description: Free set with VI-i-a
+  free_with: VI-i-a
+  frequency: 104
   mars:
     levtype: sfc
-    stream: efhs
+    stream: eehs
     type: taem
-  description: Free set with VI-i-a
   set: X
   subset: X-x
+X-x-b:
+  description: Free set with VI-i-a
   free_with: VI-i-a
   frequency: 104
-X-x-b:
   mars:
     levtype: sfc
-    stream: efhs
+    stream: eehs
     type: em
-  description: Free set with VI-i-a
   set: X
   subset: X-x
-  free_with: VI-i-a
-  frequency: 104
 X-x-c:
+  description: Free set with VI-i-b
+  free_with: VI-i-b
+  frequency: 104
   mars:
     levtype: pl
-    stream: efhs
+    stream: eehs
     type: taem
-  description: Free set with VI-i-b
   set: X
   subset: X-x
+X-x-d:
+  description: Free set with VI-i-b
   free_with: VI-i-b
   frequency: 104
-X-x-d:
   mars:
     levtype: pl
-    stream: efhs
+    stream: eehs
     type: em
-  description: Free set with VI-i-b
   set: X
   subset: X-x
-  free_with: VI-i-b
-  frequency: 104
 X-x-e:
-  mars:
-    levtype: sfc
-    stream: enfh
-    type: fcmean
   description: Free set with VI-iii-a
-  set: X
-  subset: X-x
   free_with: VI-iii-a
   frequency: 104
-X-x-f:
   mars:
-    levtype: pl
-    stream: enfh
+    levtype: sfc
+    stream: eefh
     type: fcmean
-  description: Free set with VI-iii-b
   set: X
   subset: X-x
+X-x-f:
+  description: Free set with VI-iii-b
   free_with: VI-iii-b
   frequency: 104
-X-x-g:
   mars:
-    levtype: sfc
-    stream: efov
-    type: cf
-  description: Free set with VI-v-a
+    levtype: pl
+    stream: eefh
+    type: fcmean
   set: X
   subset: X-x
-  free_with: VI-v-a
-  frequency: 104
-X-x-h:
-  mars:
-    levtype: sfc
-    stream: efov
-    type: pf
+X-x-j:
   description: Free set with VI-v-a
-  set: X
-  subset: X-x
   free_with: VI-v-a
   frequency: 104
-X-x-i:
   mars:
     levtype: sfc
-    stream: enfh
+    stream: eefh
     type: pf
-  description: Free set with VI-v-a
   set: X
   subset: X-x
-  free_with: VI-v-a
-  frequency: 104
-X-x-j:
-  mars:
-    levtype: sfc
-    stream: enfh
-    type: cf
+X-x-k:
   description: Free set with VI-v-a
-  set: X
-  subset: X-x
   free_with: VI-v-a
   frequency: 104
-X-x-k:
   mars:
-    levtype: pl
-    stream: enfh
+    levtype: sfc
+    stream: eefh
     type: cf
-  description: Free set with VI-v-b
   set: X
   subset: X-x
-  free_with: VI-v-b
-  frequency: 104
 X-x-l:
-  mars:
-    levtype: pl
-    stream: enfh
-    type: pf
   description: Free set with VI-v-b
-  set: X
-  subset: X-x
   free_with: VI-v-b
   frequency: 104
-X-x-m:
   mars:
     levtype: pl
-    stream: efov
+    stream: eefh
     type: cf
-  description: Free set with VI-v-b
   set: X
   subset: X-x
+X-x-m:
+  description: Free set with VI-v-b
   free_with: VI-v-b
   frequency: 104
-X-x-n:
   mars:
     levtype: pl
-    stream: efov
+    stream: eefh
     type: pf
-  description: Free set with VI-v-b
   set: X
   subset: X-x
-  free_with: VI-v-b
-  frequency: 104
 X-x-o:
+  description: Free set with VI-v-c
+  free_with: VI-v-c
+  frequency: 104
   mars:
     levtype: sfc
-    stream: enwh
+    stream: weeh
     type: cf
-  description: Free set with VI-v-c
   set: X
   subset: X-x
+X-x-p:
+  description: Free set with VI-v-c
   free_with: VI-v-c
   frequency: 104
-X-x-p:
   mars:
     levtype: sfc
-    stream: enwh
+    stream: weeh
     type: pf
-  description: Free set with VI-v-c
   set: X
   subset: X-x
-  free_with: VI-v-c
-  frequency: 104
 X-x-q:
+  description: Free set with VI-v-a
+  free_with: VI-v-a
+  frequency: 104
   mars:
-    levtype:
-    - pv
-    - pt
-    stream: efov
-    type: cf
-  description: Free set with VI-v-d
+    levtype: sfc
+    stream: eefh
+    type: taem
   set: X
   subset: X-x
-  free_with: VI-v-d
-  frequency: 104
 X-x-r:
+  description: Free set with VI-v-b
+  free_with: VI-v-b
+  frequency: 104
   mars:
-    levtype:
-    - pv
-    - pt
-    stream: efov
-    type: pf
-  description: Free set with VI-v-d
+    levtype: pl
+    stream: eefh
+    type: taem
   set: X
   subset: X-x
-  free_with: VI-v-d
-  frequency: 104
-
```

### Comparing `ecquote-1.4.4/ecquote/resources/wave-mask-reduced.json` & `ecquote-1.5.0/ecquote/resources/wave-mask-reduced.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources/wave-mask-regular.json` & `ecquote-1.5.0/ecquote/resources/wave-mask-regular.json`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/resources.py` & `ecquote-1.5.0/ecquote/resources.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/rest.py` & `ecquote-1.5.0/ecquote/rest.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/sets.py` & `ecquote-1.5.0/ecquote/sets.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,26 @@
         set,
         subset,
         same=None,
         order=0,
         free_data=[],
         free_with=[],
         frequency=365,
+        ic_frequency=None,
+        comment=None,
     ):
         self.name = name
         self.description = description
         self.mars = mars
         self.order = order
         self.set = set
         self.subset = subset
         self.free_with = free_with
         self.frequency = frequency
+        self.ic_frequency = ic_frequency
 
         if isinstance(free_data, dict):
             free_data = [free_data]
 
         self.free_data = []
         for f in free_data:
             for flat in iterate_request(f):
```

### Comparing `ecquote-1.4.4/ecquote/splitters/__init__.py` & `ecquote-1.5.0/ecquote/splitters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from .constant import splitter as constant_splitter
 from .destination import splitter as destination_splitter
 from .free_grids import splitter as free_grid_splitter
 from .free_sets import splitter as free_splitter
 from .freebies import splitter as freebies_splitter
 from .group_by import splitter as group_by_splitter
 from .high_frequency import splitter as high_frequency_splitter
-from .leg import splitter as leg_splitter
 from .repres import splitter as repres_splitter
 from .shgg import splitter as shgg_splitter
 from .subset import splitter as subset_splitter
 from .validate import splitter as validate_splitter
 
 LOG = logging.getLogger(__name__)
 
@@ -32,15 +31,14 @@
 
 
 def first_splitters(requests, categories=None, category=None, **kwargs):
     s = requests
 
     s = canonical_splitter(s)
     s = validate_splitter(s)
-    s = leg_splitter(s)
     s = shgg_splitter(s)
     s = subset_splitter(s)
     s = repres_splitter(s)
 
     if categories:
         s = category_splitter(s, categories, category)
```

### Comparing `ecquote-1.4.4/ecquote/splitters/canonical.py` & `ecquote-1.5.0/ecquote/splitters/canonical.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             e += 360
         area = n, w, s, e
     return tuple(str(x) for x in area)
 
 
 def canonical_time(time):
     time = [int(x) for x in time]
-    return tuple("%02d00" % (x / 100 if x > 100 else x) for x in time)
+    return tuple("%02d00" % (x / 100 if x >= 100 else x) for x in time)
 
 
 def canonical_grid(grid):
     if len(grid) == 2:
         try:
             return tuple(str(float(x)) for x in grid)
         except ValueError:
```

### Comparing `ecquote-1.4.4/ecquote/splitters/category.py` & `ecquote-1.5.0/ecquote/splitters/category.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/constant.py` & `ecquote-1.5.0/ecquote/splitters/constant.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/destination.py` & `ecquote-1.5.0/ecquote/splitters/destination.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/free_grids.py` & `ecquote-1.5.0/ecquote/splitters/free_grids.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/free_sets.py` & `ecquote-1.5.0/ecquote/splitters/free_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,14 @@
     "domain",
     "system",
     "method",
     "origin",
     "time",
     "step",
     "fcmonth",
-    "leg",
     "param",
     "levelist",
     "number",
     "frequency",
     "direction",
     "quantile",
 )
```

### Comparing `ecquote-1.4.4/ecquote/splitters/freebies.py` & `ecquote-1.5.0/ecquote/splitters/freebies.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/group_by.py` & `ecquote-1.5.0/ecquote/splitters/group_by.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/high_frequency.py` & `ecquote-1.5.0/ecquote/splitters/high_frequency.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/repres.py` & `ecquote-1.5.0/ecquote/splitters/repres.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,25 +19,35 @@
 LOG = logging.getLogger(__name__)
 
 
 def error(request):
     if not os.path.exists("tests/representations"):
         return
 
+    patch = False
+
     r = []
     for k, v in sorted(request.fields.items()):
         if k == "dataset":
             continue
         v = "/".join(str(x) for x in v)
+
+        if k == "stream" and v in ("mmsf", "msmm", "mmsa", "wasf"):
+            patch = True
+
         r.append(f"{k}={v}")
     text = ",\n".join(r) + "\n"
 
+    if patch:
+        text = text.replace("0078", "0001")
+
     for p in glob.glob("tests/representations/????.req"):
         with open(p) as f:
             if text == f.read():
+                raise ValueError(f"Duplicate request: {text} {p}")
                 return
 
     n = len(glob.glob("tests/representations/????.req"))
     with open("tests/representations/%04d.req" % (n,), "w") as f:
         f.write(text)
```

### Comparing `ecquote-1.4.4/ecquote/splitters/shgg.py` & `ecquote-1.5.0/ecquote/splitters/shgg.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/subset.py` & `ecquote-1.5.0/ecquote/splitters/subset.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/splitters/validate.py` & `ecquote-1.5.0/ecquote/splitters/validate.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/testing.py` & `ecquote-1.5.0/ecquote/testing.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote/utils.py` & `ecquote-1.5.0/ecquote/utils.py`

 * *Files identical despite different names*

### Comparing `ecquote-1.4.4/ecquote.egg-info/PKG-INFO` & `ecquote-1.5.0/ecquote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecquote
-Version: 1.4.4
+Version: 1.5.0
 Summary: A package to estimate the cost and volume of an ECMWF dissemination feed
 Home-page: https://github.com/ecmwf/ecquote
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ecquote-1.4.4/ecquote.egg-info/SOURCES.txt` & `ecquote-1.5.0/ecquote.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 ecquote/resources/O640.json
 ecquote/resources/accuracy.yaml
 ecquote/resources/config.yaml
 ecquote/resources/data-values-bands.yaml
 ecquote/resources/epu-based.yaml
 ecquote/resources/free-open-data.diss
 ecquote/resources/free-wmo-essential.diss
-ecquote/resources/freebies.yaml
 ecquote/resources/params.yaml
 ecquote/resources/pgen-accuracy.yaml
 ecquote/resources/reduced-0_125.json
 ecquote/resources/reduced-0_25.json
 ecquote/resources/reduced-0_5.json
 ecquote/resources/regular-0_125.json
 ecquote/resources/representations.yaml
@@ -77,12 +76,11 @@
 ecquote/splitters/constant.py
 ecquote/splitters/destination.py
 ecquote/splitters/free_grids.py
 ecquote/splitters/free_sets.py
 ecquote/splitters/freebies.py
 ecquote/splitters/group_by.py
 ecquote/splitters/high_frequency.py
-ecquote/splitters/leg.py
 ecquote/splitters/repres.py
 ecquote/splitters/shgg.py
 ecquote/splitters/subset.py
 ecquote/splitters/validate.py
```

### Comparing `ecquote-1.4.4/setup.py` & `ecquote-1.5.0/setup.py`

 * *Files identical despite different names*

