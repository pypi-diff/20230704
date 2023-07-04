# Comparing `tmp/modelcraft-3.1.0.tar.gz` & `tmp/modelcraft-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelcraft-3.1.0.tar", last modified: Wed Mar 29 14:31:23 2023, max compression
+gzip compressed data, was "modelcraft-3.1.1.tar", last modified: Tue Jul  4 08:48:09 2023, max compression
```

## Comparing `modelcraft-3.1.0.tar` & `modelcraft-3.1.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.102265 modelcraft-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-03-29 14:31:12.000000 modelcraft-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-29 14:31:12.000000 modelcraft-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-29 14:31:23.102265 modelcraft-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-29 14:31:12.000000 modelcraft-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.094266 modelcraft-3.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.094266 modelcraft-3.1.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-29 14:31:12.000000 modelcraft-3.1.0/docs/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-03-29 14:31:12.000000 modelcraft-3.1.0/docs/css/milligram.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-29 14:31:12.000000 modelcraft-3.1.0/docs/css/normalize.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.094266 modelcraft-3.1.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    39305 2023-03-29 14:31:12.000000 modelcraft-3.1.0/docs/img/modelcraft.png
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-03-29 14:31:12.000000 modelcraft-3.1.0/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.094266 modelcraft-3.1.0/modelcraft/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/contents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.098266 modelcraft-3.1.0/modelcraft/coot/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/coot/morph.py
--rw-r--r--   0 runner    (1001) docker     (123)    35851 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/coot/prune.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/coot/sidechains.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.098266 modelcraft-3.1.0/modelcraft/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/acedrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/acorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/buccaneer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/comit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/coot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/ctruncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/emda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/findwaters.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/freerflag.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/libg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/molrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/nautilus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/parrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/phasematch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/servalcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/jobs/sheetbend.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/maps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/modelcraftem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12142 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/modelcraftxray.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/monlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/reflections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.098266 modelcraft-3.1.0/modelcraft/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/scripts/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/scripts/copies.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/scripts/modelcraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/solvent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.098266 modelcraft-3.1.0/modelcraft/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.102265 modelcraft-3.1.0/modelcraft/tests/ccp4/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_acedrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_buccaneer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_comit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_coot.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_copies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_ctruncate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_findwaters.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_freerflag.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_libg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_molrep.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_monlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_nautilus.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_parrot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_phasematch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_reflections.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_sheetbend.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_solvent.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccp4/test_xray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.102265 modelcraft-3.1.0/modelcraft/tests/ccpem/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccpem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccpem/test_em.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccpem/test_emda.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccpem/test_refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/ccpem/test_servalcat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.102265 modelcraft-3.1.0/modelcraft/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/unittests/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/tests/unittests/test_reflections.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-29 14:31:12.000000 modelcraft-3.1.0/modelcraft/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 14:31:23.094266 modelcraft-3.1.0/modelcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-29 14:31:22.000000 modelcraft-3.1.0/modelcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-29 14:31:22.000000 modelcraft-3.1.0/modelcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 14:31:22.000000 modelcraft-3.1.0/modelcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-29 14:31:22.000000 modelcraft-3.1.0/modelcraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-29 14:31:22.000000 modelcraft-3.1.0/modelcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 14:31:22.000000 modelcraft-3.1.0/modelcraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-29 14:31:23.102265 modelcraft-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-29 14:31:12.000000 modelcraft-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.172091 modelcraft-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-04 08:47:53.000000 modelcraft-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 08:47:53.000000 modelcraft-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-04 08:48:09.172091 modelcraft-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 08:47:53.000000 modelcraft-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.164091 modelcraft-3.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.164091 modelcraft-3.1.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-04 08:47:53.000000 modelcraft-3.1.1/docs/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-04 08:47:53.000000 modelcraft-3.1.1/docs/css/milligram.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-04 08:47:53.000000 modelcraft-3.1.1/docs/css/normalize.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.164091 modelcraft-3.1.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    39305 2023-07-04 08:47:53.000000 modelcraft-3.1.1/docs/img/modelcraft.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-07-04 08:47:53.000000 modelcraft-3.1.1/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.164091 modelcraft-3.1.1/modelcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/contents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.164091 modelcraft-3.1.1/modelcraft/coot/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/coot/morph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35851 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/coot/prune.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/coot/sidechains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.168091 modelcraft-3.1.1/modelcraft/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/acedrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/acorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/buccaneer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/comit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/coot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/ctruncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/emda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/findwaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/freerflag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/libg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/molrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/nautilus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/parrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/phasematch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/servalcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/jobs/sheetbend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/modelcraftem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12142 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/modelcraftxray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/monlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/reflections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.168091 modelcraft-3.1.1/modelcraft/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/scripts/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/scripts/copies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/scripts/modelcraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/solvent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.168091 modelcraft-3.1.1/modelcraft/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.168091 modelcraft-3.1.1/modelcraft/tests/ccp4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_acedrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_buccaneer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_comit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_coot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_copies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_ctruncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_findwaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_freerflag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_libg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_molrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_monlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_nautilus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_parrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_phasematch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_sheetbend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_solvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccp4/test_xray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.172091 modelcraft-3.1.1/modelcraft/tests/ccpem/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccpem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccpem/test_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccpem/test_emda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccpem/test_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/ccpem/test_servalcat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.172091 modelcraft-3.1.1/modelcraft/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/unittests/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/tests/unittests/test_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-04 08:47:53.000000 modelcraft-3.1.1/modelcraft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:48:09.164091 modelcraft-3.1.1/modelcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-04 08:48:09.000000 modelcraft-3.1.1/modelcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-04 08:48:09.000000 modelcraft-3.1.1/modelcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:48:09.000000 modelcraft-3.1.1/modelcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-04 08:48:09.000000 modelcraft-3.1.1/modelcraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 08:48:09.000000 modelcraft-3.1.1/modelcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 08:48:09.000000 modelcraft-3.1.1/modelcraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-04 08:48:09.172091 modelcraft-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-04 08:47:53.000000 modelcraft-3.1.1/setup.py
```

### Comparing `modelcraft-3.1.0/LICENSE` & `modelcraft-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/PKG-INFO` & `modelcraft-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelcraft
-Version: 3.1.0
+Version: 3.1.1
 Summary: Automated model building pipeline for X-ray crystallography
 Home-page: https://github.com/paulsbond/modelcraft
 Author: Paul Bond
 Author-email: paul.bond@york.ac.uk
 License: LGPL-2.1
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `modelcraft-3.1.0/README.md` & `modelcraft-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/docs/css/milligram.min.css` & `modelcraft-3.1.1/docs/css/milligram.min.css`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/docs/css/normalize.min.css` & `modelcraft-3.1.1/docs/css/normalize.min.css`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/docs/img/modelcraft.png` & `modelcraft-3.1.1/docs/img/modelcraft.png`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/docs/index.html` & `modelcraft-3.1.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/__init__.py` & `modelcraft-3.1.1/modelcraft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 
 from .cell import max_distortion as max_cell_distortion
 from .cell import remove_scale
 from .cell import update_cell
 from .contents import AsuContents
 from .contents import PolymerType
 from .geometry import rmsz
```

### Comparing `modelcraft-3.1.0/modelcraft/arguments.py` & `modelcraft-3.1.1/modelcraft/arguments.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/cell.py` & `modelcraft-3.1.1/modelcraft/cell.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/contents.py` & `modelcraft-3.1.1/modelcraft/contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/coot/morph.py` & `modelcraft-3.1.1/modelcraft/coot/morph.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/coot/prune.py` & `modelcraft-3.1.1/modelcraft/coot/prune.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/coot/sidechains.py` & `modelcraft-3.1.1/modelcraft/coot/sidechains.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/environ.py` & `modelcraft-3.1.1/modelcraft/environ.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/geometry.py` & `modelcraft-3.1.1/modelcraft/geometry.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/job.py` & `modelcraft-3.1.1/modelcraft/job.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/acedrg.py` & `modelcraft-3.1.1/modelcraft/jobs/acedrg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/acorn.py` & `modelcraft-3.1.1/modelcraft/jobs/acorn.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/buccaneer.py` & `modelcraft-3.1.1/modelcraft/jobs/buccaneer.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/comit.py` & `modelcraft-3.1.1/modelcraft/jobs/comit.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/coot.py` & `modelcraft-3.1.1/modelcraft/jobs/coot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/ctruncate.py` & `modelcraft-3.1.1/modelcraft/jobs/ctruncate.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/emda.py` & `modelcraft-3.1.1/modelcraft/jobs/emda.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/findwaters.py` & `modelcraft-3.1.1/modelcraft/jobs/findwaters.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/freerflag.py` & `modelcraft-3.1.1/modelcraft/jobs/freerflag.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/libg.py` & `modelcraft-3.1.1/modelcraft/jobs/libg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/molrep.py` & `modelcraft-3.1.1/modelcraft/jobs/molrep.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/nautilus.py` & `modelcraft-3.1.1/modelcraft/jobs/nautilus.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/parrot.py` & `modelcraft-3.1.1/modelcraft/jobs/parrot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/phasematch.py` & `modelcraft-3.1.1/modelcraft/jobs/phasematch.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/refmac.py` & `modelcraft-3.1.1/modelcraft/jobs/refmac.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     abcd: DataItem
     fphi_best: DataItem
     fphi_diff: DataItem
     fphi_calc: DataItem
     rwork: float
     rfree: float
     fsc: float
+    initial_rwork: float
+    initial_rfree: float
+    initial_fsc: float
     data_completeness: float
     resolution_high: float
     seconds: float
 
 
 class Refmac(Job):
     def __init__(
@@ -64,15 +67,15 @@
                 labin += " HLB=" + self.phases.label(1)
                 labin += " HLC=" + self.phases.label(2)
                 labin += " HLD=" + self.phases.label(3)
             else:
                 labin += " PHIB=" + self.phases.label(0)
                 labin += " FOM=" + self.phases.label(1)
         self._stdin.append("LABIN " + labin)
-        self._stdin.append("NCYCLES %d" % self.cycles)
+        self._stdin.append(f"NCYCLES {self.cycles}")
         self._stdin.append("WEIGHT AUTO")
         if self.jelly_body:
             self._stdin.append("RIDGE DISTANCE SIGMA 0.02")
         if self.twinned:
             self._stdin.append("TWIN")
         self._stdin.append("MAKE HYDR NO")
         self._stdin.append("MAKE NEWLIGAND NOEXIT")
@@ -93,14 +96,17 @@
             abcd=DataItem(mtz, "HLACOMB,HLBCOMB,HLCCOMB,HLDCOMB"),
             fphi_best=DataItem(mtz, "FWT,PHWT"),
             fphi_diff=DataItem(mtz, "DELFWT,PHDELWT"),
             fphi_calc=DataItem(mtz, "FC_ALL_LS,PHIC_ALL_LS"),
             rwork=float(rworks[-1].text),
             rfree=float(rfrees[-1].text),
             fsc=float(fscs[-1].text),
+            initial_rwork=float(rworks[0].text),
+            initial_rfree=float(rfrees[0].text),
+            initial_fsc=float(fscs[0].text),
             data_completeness=float(xml.find("Overall_stats/data_completeness").text),
             resolution_high=float(xml.find("Overall_stats/resolution_high").text),
             seconds=self._seconds,
         )
 
 
 @dataclasses.dataclass
@@ -118,19 +124,19 @@
 
     def _setup(self) -> None:
         self.density.write_ccp4_map(self._path("mapin.ccp4"))
         self._args += ["MAPIN", "mapin.ccp4"]
         self._args += ["HKLOUT", "hklout.mtz"]
         self._stdin.append("MODE SFCALC")
         self._stdin.append("SOURCE EM MB")
-        self._stdin.append("RESOLUTION %f" % self.resolution)
+        self._stdin.append(f"RESOLUTION {self.resolution}")
         if self.blur > 0:
-            self._stdin.append("SFCALC BLUR %f" % self.blur)
+            self._stdin.append(f"SFCALC BLUR {self.blur}")
         elif self.blur < 0:
-            self._stdin.append("SFCALC SHARP %f" % -self.blur)
+            self._stdin.append(f"SFCALC SHARP {-self.blur}")
         self._stdin.append("END")
 
     def _result(self) -> RefmacMapToMtzResult:
         self._check_files_exist("hklout.mtz")
         mtz = gemmi.read_mtz_file(self._path("hklout.mtz"))
         suffix = "0"
         if self.blur > 0:
```

### Comparing `modelcraft-3.1.0/modelcraft/jobs/servalcat.py` & `modelcraft-3.1.1/modelcraft/jobs/servalcat.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/jobs/sheetbend.py` & `modelcraft-3.1.1/modelcraft/jobs/sheetbend.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/modelcraftem.py` & `modelcraft-3.1.1/modelcraft/modelcraftem.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/modelcraftxray.py` & `modelcraft-3.1.1/modelcraft/modelcraftxray.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/monlib.py` & `modelcraft-3.1.1/modelcraft/monlib.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/pipeline.py` & `modelcraft-3.1.1/modelcraft/pipeline.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/reflections.py` & `modelcraft-3.1.1/modelcraft/reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/scripts/contents.py` & `modelcraft-3.1.1/modelcraft/scripts/contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/scripts/copies.py` & `modelcraft-3.1.1/modelcraft/scripts/copies.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/solvent.py` & `modelcraft-3.1.1/modelcraft/solvent.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/structure.py` & `modelcraft-3.1.1/modelcraft/structure.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/__init__.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/__init__.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_acedrg.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_acedrg.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_arguments.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_arguments.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_buccaneer.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_buccaneer.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_cell.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_cell.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_comit.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_comit.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_contents.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_coot.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_coot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_ctruncate.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_ctruncate.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_findwaters.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_findwaters.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_geometry.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_geometry.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_molrep.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_molrep.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_nautilus.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_nautilus.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_parrot.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_parrot.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_phasematch.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_phasematch.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_reflections.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_sheetbend.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_sheetbend.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_solvent.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_solvent.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccp4/test_xray.py` & `modelcraft-3.1.1/modelcraft/tests/ccp4/test_xray.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccpem/__init__.py` & `modelcraft-3.1.1/modelcraft/tests/ccpem/__init__.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccpem/test_em.py` & `modelcraft-3.1.1/modelcraft/tests/ccpem/test_em.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/ccpem/test_servalcat.py` & `modelcraft-3.1.1/modelcraft/tests/ccpem/test_servalcat.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/unittests/test_contents.py` & `modelcraft-3.1.1/modelcraft/tests/unittests/test_contents.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft/tests/unittests/test_reflections.py` & `modelcraft-3.1.1/modelcraft/tests/unittests/test_reflections.py`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/modelcraft.egg-info/PKG-INFO` & `modelcraft-3.1.1/modelcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelcraft
-Version: 3.1.0
+Version: 3.1.1
 Summary: Automated model building pipeline for X-ray crystallography
 Home-page: https://github.com/paulsbond/modelcraft
 Author: Paul Bond
 Author-email: paul.bond@york.ac.uk
 License: LGPL-2.1
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `modelcraft-3.1.0/modelcraft.egg-info/SOURCES.txt` & `modelcraft-3.1.1/modelcraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelcraft-3.1.0/setup.py` & `modelcraft-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setuptools.setup(
     name="modelcraft",
-    version="3.1.0",
+    version="3.1.1",
     author="Paul Bond",
     author_email="paul.bond@york.ac.uk",
     description="Automated model building pipeline for X-ray crystallography",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/paulsbond/modelcraft",
     packages=setuptools.find_packages(),
```

