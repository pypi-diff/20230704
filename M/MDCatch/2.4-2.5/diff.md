# Comparing `tmp/MDCatch-2.4.tar.gz` & `tmp/MDCatch-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDCatch-2.4.tar", last modified: Thu Jun 16 14:01:42 2022, max compression
+gzip compressed data, was "MDCatch-2.5.tar", last modified: Tue Jul  4 15:04:13 2023, max compression
```

## Comparing `MDCatch-2.4.tar` & `MDCatch-2.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-06-16 14:01:20.000000 MDCatch-2.4/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-06-16 14:01:20.000000 MDCatch-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-06-16 14:01:20.000000 MDCatch-2.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/MDCatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-06-16 14:01:41.000000 MDCatch-2.4/MDCatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-06-16 14:01:41.000000 MDCatch-2.4/MDCatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-16 14:01:41.000000 MDCatch-2.4/MDCatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-16 14:01:41.000000 MDCatch-2.4/MDCatch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-16 14:01:41.000000 MDCatch-2.4/MDCatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-16 14:01:41.000000 MDCatch-2.4/MDCatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-06-16 14:01:42.045187 MDCatch-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9722 2022-06-16 14:01:20.000000 MDCatch-2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.037186 MDCatch-2.4/mdcatch/Schemes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/prep/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/prep/ctffind/
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/prep/ctffind/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/prep/importmovies/
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/prep/importmovies/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/prep/motioncorr/
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/prep/motioncorr/job.star
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/prep/scheme.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/autopick/
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/autopick/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/class2d/
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/class2d/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/extract/
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/extract/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/inimodel3d/
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/inimodel3d/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/refine3d/
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/refine3d/job.star
--rw-r--r--   0 runner    (1001) docker     (121)     4216 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/scheme.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/select_mics/
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/select_mics/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/select_parts/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-cryolo/select_parts/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.041187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/autopick/
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/autopick/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/class2d/
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/class2d/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/extract/
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/extract/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/inimodel3d/
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/inimodel3d/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/refine3d/
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/refine3d/job.star
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/scheme.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/select_mics/
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/select_mics/job.star
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/Schemes/proc-topaz/select_parts/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/Schemes/proc-topaz/select_parts/job.star
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14085 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/external_job_cryolo.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8776 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/external_job_cryolo_train.py
--rw-r--r--   0 runner    (1001) docker     (121)     8305 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    19768 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/run.py
--rw-r--r--   0 runner    (1001) docker     (121)    14949 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     6089 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/template.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/tests/fake_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (121)    14526 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/tests/testdata/FoilHole_18890345_Data_18881924_18881926_20200320_090200.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8976 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/tests/testdata/FoilHole_22011316_Data_19957701_19957703_20200323_100235.xml
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/tests/testdata/img_h1_s2_i374_movie_00001_Jul30_07.56.47.tif.mdoc
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-16 14:01:42.045187 MDCatch-2.4/mdcatch/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3594 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/utils/feimrc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7068 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/utils/feixml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/utils/mdoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5253 2022-06-16 14:01:20.000000 MDCatch-2.4/mdcatch/utils/tiff.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-16 14:01:42.045187 MDCatch-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-06-16 14:01:20.000000 MDCatch-2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-04 15:03:58.000000 MDCatch-2.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 15:03:58.000000 MDCatch-2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 15:03:58.000000 MDCatch-2.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/MDCatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-04 15:04:13.000000 MDCatch-2.5/MDCatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-04 15:04:13.000000 MDCatch-2.5/MDCatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:04:13.000000 MDCatch-2.5/MDCatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-04 15:04:13.000000 MDCatch-2.5/MDCatch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 15:04:13.000000 MDCatch-2.5/MDCatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 15:04:13.000000 MDCatch-2.5/MDCatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-04 15:04:13.305328 MDCatch-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-04 15:03:58.000000 MDCatch-2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/mdcatch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/mdcatch/Schemes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/mdcatch/Schemes/prep/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/mdcatch/Schemes/prep/ctffind/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/prep/ctffind/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/mdcatch/Schemes/prep/importmovies/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/prep/importmovies/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/mdcatch/Schemes/prep/motioncorr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/prep/motioncorr/job.star
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/prep/scheme.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.301328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/autopick/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/autopick/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/class2d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/class2d/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/extract/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/inimodel3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/inimodel3d/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/refine3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/refine3d/job.star
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/scheme.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/select_mics/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/select_mics/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/select_parts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-cryolo/select_parts/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/autopick/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/autopick/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/class2d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/class2d/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/extract/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/inimodel3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/inimodel3d/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/refine3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/refine3d/job.star
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/scheme.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/select_mics/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/select_mics/job.star
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/Schemes/proc-topaz/select_parts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/Schemes/proc-topaz/select_parts/job.star
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14085 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/external_job_cryolo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8776 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/external_job_cryolo_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/tests/fake_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/tests/testdata/FoilHole_18890345_Data_18881924_18881926_20200320_090200.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/tests/testdata/FoilHole_22011316_Data_19957701_19957703_20200323_100235.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/tests/testdata/img_h1_s2_i374_movie_00001_Jul30_07.56.47.tif.mdoc
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:04:13.305328 MDCatch-2.5/mdcatch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/utils/feimrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/utils/feixml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/utils/mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-04 15:03:58.000000 MDCatch-2.5/mdcatch/utils/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:04:13.305328 MDCatch-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-04 15:03:58.000000 MDCatch-2.5/setup.py
```

### Comparing `MDCatch-2.4/CHANGES.txt` & `MDCatch-2.5/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+2.5:
+    - fix Falcon 4(i) EER case: parse frame rate and gain reference name from xml
+    - add EF-Falcon camera type
+    - update cryolo version
+    - added cmd scripts to parse metadata files
+    - fix microscope id parsing from mdoc
+    - remove skip_gridding param (#58)
+    - set 7x5 patches for Gatan detectors (#59)
 2.4:
     - upgrade to PyQt6
 2.3: fix the crash due to zero wait time in prep scheme
 2.2b2: Cryolo script updates:
     1) cryolo 1.8+ required
     2) input is a star file
     3) use scratch SSD for filtered mics
```

### Comparing `MDCatch-2.4/LICENSE` & `MDCatch-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/MDCatch.egg-info/PKG-INFO` & `MDCatch-2.5/MDCatch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: MDCatch
-Version: 2.4
+Version: 2.5
 Summary: Fetch metadata from EPU / SerialEM and launch on-the-fly pre-processing
 Home-page: https://github.com/azazellochg/MDCatch
 Author: Grigory Sharov
 Author-email: gsharov@mrc-lmb.cam.ac.uk
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/azazellochg/MDCatch/issues
 Project-URL: Source, https://github.com/azazellochg/MDCatch
 Keywords: cryo-em python qt6 epu serialem
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 See https://github.com/azazellochg/MDCatch for more details
-
```

### Comparing `MDCatch-2.4/MDCatch.egg-info/SOURCES.txt` & `MDCatch-2.5/MDCatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/PKG-INFO` & `MDCatch-2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: MDCatch
-Version: 2.4
+Version: 2.5
 Summary: Fetch metadata from EPU / SerialEM and launch on-the-fly pre-processing
 Home-page: https://github.com/azazellochg/MDCatch
 Author: Grigory Sharov
 Author-email: gsharov@mrc-lmb.cam.ac.uk
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/azazellochg/MDCatch/issues
 Project-URL: Source, https://github.com/azazellochg/MDCatch
 Keywords: cryo-em python qt6 epu serialem
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 See https://github.com/azazellochg/MDCatch for more details
-
```

### Comparing `MDCatch-2.4/README.rst` & `MDCatch-2.5/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 .. raw:: html
 
    <details>
    <summary><a>Dependencies</a></summary>
 
 Dependencies are installed by pip automatically:
 
- * python3
+ * python
  * pyqt6 (GUI)
  * mrcfile (to parse MRC header)
  * tifffile (to parse TIF header)
  * emtable (STAR file parser)
 
 .. raw:: html
 
@@ -52,18 +52,18 @@
 .. raw:: html
 
    </details>
 
 Screenshots
 -----------
 
-.. image:: https://user-images.githubusercontent.com/6952870/139845150-d1aa465c-98cd-4a11-8c84-df099fbeb397.png
+.. image:: https://github.com/azazellochg/MDCatch/assets/6952870/621deb21-bec7-478e-8b89-61659765a383
    :width: 640 px
 
-.. image:: https://user-images.githubusercontent.com/6952870/139845338-4ee9b0be-0a94-41ee-8710-f730b71f1177.png
+.. image:: https://github.com/azazellochg/MDCatch/assets/6952870/3d7475e5-7c34-42b9-b317-4662482c6c30
    :width: 640 px
 
 
 Running
 -------
 
 To run simply type **mdcatch**.
@@ -81,15 +81,15 @@
    <summary><a>General information</a></summary>
 
 The app is installed on a pre-processing server with GPU(s).
 The server requires the following software installed:
 
     - `RELION 4.0 <https://relion.readthedocs.io/en/release-4.0/>`_ or/and `Scipion 3 <http://scipion.i2pc.es/>`_
     - `CTFFIND4 <https://grigoriefflab.umassmed.edu/ctffind4>`_
-    - `Topaz <https://github.com/tbepler/topaz>`_ or/and `crYOLO 1.8.0+ <https://cryolo.readthedocs.io/>`_ (installed in a separate conda environment)
+    - `Topaz <https://github.com/tbepler/topaz>`_ or/and `crYOLO 1.9+ <https://cryolo.readthedocs.io/>`_ (installed in a separate conda environment)
 
 Relion and/or Scipion should be available from your shell **PATH**. For Relion's schemes you also need to define the following variables:
 
 .. code-block:: bash
 
     export RELION_SCRATCH_DIR="/ssd/$USER"
     export RELION_CTFFIND_EXECUTABLE=/home/gsharov/soft/ctffind
@@ -117,36 +117,41 @@
 
 Most of the configuration is done in **config.py**.
 For the very first time it is useful to set **DEBUG=1** to see additional output and make sure it all works as expected.
 
 Important points to mention:
 
     * camera names in the SCOPE_DICT must match the names in EPU_MOVIES_DICT, GAIN_DICT and MTF_DICT
-    * since in EPU Falcon cameras are called "BM-Falcon" and Gatan cameras are called "EF-CCD", MOVIE_PATH_DICT keys should not be changed, only the values
+    * since in EPU Falcon cameras are called "BM-Falcon" or "EF-Falcon" and Gatan cameras are called "EF-CCD", MOVIE_PATH_DICT keys should not be changed, only the values
     * Relion schemes use two GPUs: 0-1
 
 Below is an example of the folders setup on our server. Data points to movies storage, while Metadata is for EPU sessions.
 
 .. code-block:: bash
 
     /mnt
     ├── Data
-    │   ├── Krios1
-    │   │   ├── Falcon3
-    │   │   └── K2 (with DoseFractions folder inside)
-    │   ├── Krios2
-    │   │   ├── Falcon4
-    │   │   └── K2 (with DoseFractions folder inside)
-    │   └── Krios3
-    │       ├── Falcon3
-    │       └── K3 (with DoseFractions folder inside)
+    │     ├── Krios1
+    │     │     ├── Falcon3
+    │     │     └── K3 (with DoseFractions folder inside)
+    │     ├── Krios2
+    │     │     ├── Falcon4
+    │     │     └── K2 (with DoseFractions folder inside)
+    │     ├── Krios3
+    │     │     ├── Falcon3
+    │     │     └── K3 (with DoseFractions folder inside)
+    │     ├── Krios4
+    │     │     └── Falcon4
+    │     └── Glacios
+    │           └── Falcon3
     └── MetaData
         ├── Krios1
         ├── Krios2
-        └── Krios3
+        ├── Krios3
+        └── Krios4
 
 .. raw:: html
 
    </details>
    <details>
    <summary><a>Working principle</a></summary>
 
@@ -178,15 +183,15 @@
 The metadata folder name (EPU session name) matches the folder name with movies on a storage server.
 
 In case of SerialEM, the movies and metadata (mdoc file) are expected to be in the same folder, so here user must select a folder with movies in the GUI.
 
 SPA vs Helical mode
 ###################
 
-From MDCatch v2.2 onwards crYOLO picker can be run in helical mode (crYOLO v1.8.0+ required). Instead of a particle size, user provides the filament width. A pre-trained crYOLO model is also required.
+From MDCatch v2.2 onwards crYOLO picker can be run in helical mode (crYOLO v1.9+ required). Instead of a particle size, user provides the filament width. A pre-trained crYOLO model is also required.
 The suggested parameters in this case are:
 
     - tube diameter = 1.2 x filament width
     - box size = 1.5 x tube diameter
     - mask size = 0.9 x box size
     - inter-box distance = 0.1 x box size
 
@@ -246,16 +251,26 @@
 
     python -m unittest mdcatch.tests
 
 .. raw:: html
 
    </details>
 
+Extras
+------
+
+The MDCatch package provides extra command-line scripts to parse MRC, XML, MDOC or TIF file headers. Simply use one of the commands below followed by a filename:
+
+* parse-mrc filename.mrc
+* parse-xml filename.xml
+* parse-mdoc filename.mdoc
+* parse-tif filename.tiff
+
 How to cite
 -----------
 
 Kimanius D, Dong L, Sharov G, Nakane T, Scheres SHW. New tools for automated cryo-EM single-particle analysis in RELION-4.0. Biochem J. 2021, 478(24), p. 4169-4185. doi:10.1042/BCJ20210708
 
 Feedback
 --------
 
-Please report bugs and suggestions for improvements as a `Github issue <https://github.com/azazellochg/MDCatch/issues/new/choose>`_.
+Please report bugs and suggestions for improvements as a `Github issue <https://github.com/azazellochg/MDCatch/issues/new>`_.
```

### Comparing `MDCatch-2.4/mdcatch/Schemes/prep/ctffind/job.star` & `MDCatch-2.5/mdcatch/Schemes/prep/ctffind/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/prep/importmovies/job.star` & `MDCatch-2.5/mdcatch/Schemes/prep/importmovies/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/prep/motioncorr/job.star` & `MDCatch-2.5/mdcatch/Schemes/prep/motioncorr/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/prep/scheme.star` & `MDCatch-2.5/mdcatch/Schemes/prep/scheme.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/autopick/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/autopick/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/class2d/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/class2d/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/extract/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/extract/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/inimodel3d/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/inimodel3d/job.star`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,11 @@
 nr_threads         12 
 other_args         ""
 particle_diameter        200 
       qsub       qsub 
 qsubscript /public/EM/RELION/relion/bin/relion_qsub.csh 
  queuename    openmpi 
 scratch_dir       $RELION_SCRATCH_DIR
-skip_gridding        Yes 
   sym_name         C1
    tau_fudge          4
    use_gpu        Yes
```

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/refine3d/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/refine3d/job.star`

 * *Files 6% similar despite different names*

```diff
@@ -62,11 +62,10 @@
  range_psi         10 
  range_rot         -1 
 range_tilt         15 
 ref_correct_greyscale        Yes 
  relax_sym         "" 
   sampling "7.5 degrees" 
 scratch_dir       $RELION_SCRATCH_DIR
-skip_gridding        Yes 
   sym_name         C1
    use_gpu        Yes
```

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/scheme.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/scheme.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/select_mics/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/select_mics/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-cryolo/select_parts/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-cryolo/select_parts/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/autopick/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/autopick/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/class2d/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/class2d/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/extract/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/extract/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/inimodel3d/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/inimodel3d/job.star`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,11 @@
 nr_threads         12 
 other_args         ""
 particle_diameter        200 
       qsub       qsub 
 qsubscript /public/EM/RELION/relion/bin/relion_qsub.csh 
  queuename    openmpi 
 scratch_dir       $RELION_SCRATCH_DIR
-skip_gridding        Yes 
   sym_name         C1
    tau_fudge          4
    use_gpu        Yes
```

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/refine3d/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/refine3d/job.star`

 * *Files 4% similar despite different names*

```diff
@@ -62,11 +62,10 @@
  range_psi         10 
  range_rot         -1 
 range_tilt         15 
 ref_correct_greyscale        Yes 
  relax_sym         "" 
   sampling "7.5 degrees" 
 scratch_dir       $RELION_SCRATCH_DIR
-skip_gridding        Yes 
   sym_name         C1
    use_gpu        Yes
```

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/scheme.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/scheme.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/select_mics/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/select_mics/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/Schemes/proc-topaz/select_parts/job.star` & `MDCatch-2.5/mdcatch/Schemes/proc-topaz/select_parts/job.star`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/__init__.py` & `MDCatch-2.5/mdcatch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'gsharov@mrc-lmb.cam.ac.uk'
 # *
 # **************************************************************************
 
-__version__ = '2.4'
+__version__ = '2.5'
```

### Comparing `MDCatch-2.4/mdcatch/config.py` & `MDCatch-2.5/mdcatch/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,25 +39,26 @@
 # in SerialEM case movies and mdocs are expected in the same folder
 METADATA_PATH = "/mnt/MetaData"
 
 # path where Relion projects are created
 PROJECT_PATH = "/cephfs"
 
 # Folder with Relion 4 template schemes
-SCHEMES_PATH = "/home/gsharov/soft/MDCatch-dev/mdcatch/Schemes"
+SCHEMES_PATH = "/home/gsharov/soft/MDCatch/mdcatch/Schemes"
 
 # Scipion 3 template
-JSON_TEMPLATE = "/home/gsharov/soft/MDCatch-dev/mdcatch/template.json"
+JSON_TEMPLATE = "/home/gsharov/soft/MDCatch/mdcatch/template.json"
 
 # main dictionary
 # instrumentID: [name, Cs, TFS camera, Gatan camera]
 SCOPE_DICT = {
     '3299': ['Krios1', 2.7, 'Falcon3', 'K3'],
     '3413': ['Krios2', 2.7, 'Falcon4', 'K2'],
     '3593': ['Krios3', 2.7, 'Falcon3', 'K3'],
+    '4248': ['Krios4', 2.7, 'Falcon4', None],
     '9952833': ['Glacios', 2.7, 'Falcon3', None]
 }
 
 ###############################################################################
 # EPU params
 
 # EPU-produced movie file patterns per each camera
@@ -67,16 +68,17 @@
     'K2': "Images-Disc*/GridSquare_*/Data/FoilHole_*_Data_*.mrc",
     'K3': "Images-Disc*/GridSquare_*/Data/FoilHole_*_Data_*_fractions.tiff"
 }
 # EPU-produced gain reference file patterns per each camera
 GAIN_DICT = {
     'K2': "FoilHole_*_Data_*-gain-ref.MRC",
     'K3': "FoilHole_*_Data_*_gain.tiff",
-    # Falcon 4 EER gain is not copied by EPU, so we need to provide a full path
-    'Falcon4': "/home/gsharov/20210128_135200_EER_GainReference.gain"
+    # HACK: Falcon 4 EER gain is not copied by EPU, so we need to provide a full path
+    # to a folder with gain files. Filenames should match the names from EPU xml file.
+    'Falcon4': "/home/gsharov/"
 }
 
 # Which EPU session files to parse for metadata (default is xml)
 # change the pattern below if you want to parse movie sums mrc instead
 PATTERN_EPU = "Images-Disc*/GridSquare_*/Data/FoilHole_*_Data_*.xml"
 
 # path to MTF files for Relion, %s is replaced by e.g. 300
@@ -91,46 +93,46 @@
 }
 
 # path to raw movies folder depending on camera name
 # example: /mnt/Data/Krios3/K3/
 # scope and camera names should match SCOPE_DICT
 MOVIE_PATH_DICT = {
     'EF-CCD': '/mnt/Data/%s/%s/',
-    'BM-Falcon': '/mnt/Data/%s/%s/'
+    'BM-Falcon': '/mnt/Data/%s/%s/',
+    'EF-Falcon': '/mnt/Data/%s/%s/'
 }
 
 ###############################################################################
 # SerialEM params
 
 # SerialEM-produced movies pattern
 PATTERN_SEM_MOVIES = "*.tif"
 # Default metadata format is mdoc,
 # change the pattern below if you want to parse movie tif instead
 PATTERN_SEM = "*.tif.mdoc"
 
 # Which SerialEM mdoc variables to parse
 SERIALEM_PARAMS = [
-    'T',  # Microscope ID
     'Voltage',
     'Magnification',
     'ExposureDose',
     'PixelSpacing',
     'ExposureTime',
     'Binning',
     'TargetDefocus',
     'NumSubFrames',
-    # 'DateTime',
+    'DateTime',
     'DefectFile',
     'GainReference'
 ]
 
 # help message for path selection
 help_message = """Select the following folder:\n\n
    For EPU: the EPU session folder on /mnt/MetaData/
    with Images-Disc folder inside.\n
    OR\n
    For SerialEM: the folder on /mnt/Data/ that
    contains tif movies and mdoc files.\n"""
 
 # help message for model selection
 help_message2 = """Select a pretrained model for crYOLO or Topaz.
-If empty, the general model will be used."""
+If empty, the general model will be used."""
```

### Comparing `MDCatch-2.4/mdcatch/external_job_cryolo.py` & `MDCatch-2.5/mdcatch/external_job_cryolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import time
 from glob import glob
 import subprocess
 import math
 from emtable import Table  # run "pip install --user emtable" for system python
 
 
-CONDA_ENV = ". /home/gsharov/rc/conda.rc && conda activate cryolo-1.8.2"
+CONDA_ENV = ". /home/gsharov/rc/conda.rc && conda activate cryolo-1.9.3"
 CRYOLO_PREDICT = "cryolo_predict.py"
 CRYOLO_GEN_MODEL = "/home/gsharov/soft/cryolo/gmodel_phosnet_202005_N63_c17.h5"
 CRYOLO_GEN_JANNI_MODEL = "/home/gsharov/soft/cryolo/gmodel_phosnet_202005_nn_N63_c17.h5"
 CRYOLO_JANNI_MODEL = "/home/gsharov/soft/cryolo/gmodel_janni_20190703.h5"
 SCRATCH_DIR = os.getenv("RELION_SCRATCH_DIR", None)  # SSD scratch space for filtered mics, can be None
 DEBUG = 0
 
@@ -293,15 +293,15 @@
     diff = end - start
     print("Job duration = %dh %dmin %dsec \n" % (diff//3600, diff//60 % 60, diff % 60))
 
 
 def main():
     """Change to the job working directory, then call run_job()"""
     help = """
-External job for calling crYOLO 1.8+ within Relion 4.0. Run it in the Relion project directory, e.g.:
+External job for calling crYOLO 1.9+ within Relion 4.0. Run it in the Relion project directory, e.g.:
     external_job_cryolo.py --o External/cryolo_picking --in_mics CtfFind/job004/micrographs_ctf.star
 """
     parser = argparse.ArgumentParser(usage=help)
     parser.add_argument("--in_mics", help="Input micrographs STAR file")
     parser.add_argument("--o", dest="out_dir", help="Output directory name")
     parser.add_argument("--j", dest="threads", help="Number of CPU threads (default = all)", type=int, default=1)
     parser.add_argument("--box_size", help="Box size (default = 0 means it's estimated)", type=int, default=0)
```

### Comparing `MDCatch-2.4/mdcatch/external_job_cryolo_train.py` & `MDCatch-2.5/mdcatch/external_job_cryolo_train.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import json
 import os
 import time
 import subprocess
 from emtable import Table  # run "pip3 install --user emtable" for system python
 
 
-CONDA_ENV = ". /home/gsharov/rc/conda.rc && conda activate cryolo-1.8.2"
+CONDA_ENV = ". /home/gsharov/rc/conda.rc && conda activate cryolo-1.9.3"
 CRYOLO_TRAIN = "cryolo_train.py"
 CRYOLO_GEN_MODEL = "/home/gsharov/soft/cryolo/gmodel_phosnet_202005_N63_c17.h5"
 CRYOLO_JANNI_MODEL = "/home/gsharov/soft/cryolo/gmodel_janni_20190703.h5"
 TUNE_MODEL = "fine_tuned_model.h5"
 IMG_FOLDER = "train_image"
 ANNOT_FOLDER = "train_annot"
 SCRATCH_DIR = os.getenv("RELION_SCRATCH_DIR", None)  # SSD scratch space for filtered mics, can be None
```

### Comparing `MDCatch-2.4/mdcatch/parser.py` & `MDCatch-2.5/mdcatch/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                 gainFn = next(gainFiles, 'None')
             else:
                 movieDir = os.path.join(p1, session, EPU_MOVIES_DICT[model])
                 movieBaseDir = os.path.join(p1, session)
                 # Falcon 4 EER gain reference
                 if model == "Falcon4":
                     if self.acqDict['Mode'] == "EER":
-                        gainFn = GAIN_DICT[model]
+                        gainFn = os.path.join(GAIN_DICT[model], self.acqDict['GainReference'])
                     else:  # MRC
                         if not EPU_MOVIES_DICT[model].endswith(".mrc"):
                             movieDir = movieDir.replace("_EER.eer", ".mrc")
 
             if not os.path.exists(movieBaseDir) and not testmode:
                 raise FileNotFoundError("Movie folder %s does not exist!" % movieBaseDir)
```

### Comparing `MDCatch-2.4/mdcatch/run.py` & `MDCatch-2.5/mdcatch/run.py`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/schedule.py` & `MDCatch-2.5/mdcatch/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,17 @@
         mapDict.update({
             'prep__motioncorr__bin_factor': 1,
             'prep__motioncorr__group_frames': 1,
             'prep__motioncorr__dose_per_frame': 1.0,
             'prep__motioncorr__eer_grouping': eer_group
         })
 
+    if paramDict['Detector'] in ["K2", "K3"]:
+        mapDict.update({'prep__motioncorr__patch_x': 7})
+
     prjName = getPrjName(paramDict)
     prjPath = os.path.join(paramDict['PrjPath'], prjName)
     os.mkdir(prjPath)
 
     # Create links
     movieDir = os.path.join(prjPath, "Movies")
     if os.path.islink(movieDir):
@@ -314,14 +317,16 @@
     importProt["gainFile"] = (prjPath + "/" + os.path.basename(gain)) if gain else ""
 
     # motioncorr
     movieProt = protocolsList[protNames["ProtRelionMotioncor"]]
     movieProt["binFactor"] = bin
     movieProt["groupFrames"] = group_frames
     movieProt["defectFile"] = (prjPath + "/" + os.path.basename(defect)) if defect else ""
+    if paramDict['Detector'] in ["K2", "K3"]:
+        movieProt['patchX'] = 7
 
     # ctffind
     ctfProt = protocolsList[protNames["CistemProtCTFFind"]]
     ctfProt["findPhaseShift"] = paramDict['PhasePlateUsed']
     ctfProt["streamingBatchSize"] = BATCH_SIZE
 
     # picking
```

### Comparing `MDCatch-2.4/mdcatch/template.json` & `MDCatch-2.5/mdcatch/template.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {'1': "{'sumFrameN': 0}"}*

```diff
@@ -68,15 +68,15 @@
         "patchX": 5,
         "patchY": 5,
         "runMode": 0,
         "runName": null,
         "saveNonDW": false,
         "savePSsum": true,
         "sumFrame0": 1,
-        "sumFrameN": 24
+        "sumFrameN": 0
     },
     {
         "_prerequisites": "",
         "_queueParams": null,
         "_useQueue": false,
         "astigmatism": 100.0,
         "avgFrames": 3,
```

### Comparing `MDCatch-2.4/mdcatch/tests/__init__.py` & `MDCatch-2.5/mdcatch/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/tests/fake_run.py` & `MDCatch-2.5/mdcatch/tests/fake_run.py`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/tests/testdata/FoilHole_18890345_Data_18881924_18881926_20200320_090200.xml` & `MDCatch-2.5/mdcatch/tests/testdata/FoilHole_18890345_Data_18881924_18881926_20200320_090200.xml`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/tests/testdata/FoilHole_22011316_Data_19957701_19957703_20200323_100235.xml` & `MDCatch-2.5/mdcatch/tests/testdata/FoilHole_22011316_Data_19957701_19957703_20200323_100235.xml`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/tests/testdata/img_h1_s2_i374_movie_00001_Jul30_07.56.47.tif.mdoc` & `MDCatch-2.5/mdcatch/tests/testdata/img_h1_s2_i374_movie_00001_Jul30_07.56.47.tif.mdoc`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/tests/tests.py` & `MDCatch-2.5/mdcatch/tests/tests.py`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/utils/__init__.py` & `MDCatch-2.5/mdcatch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/utils/feimrc.py` & `MDCatch-2.5/mdcatch/utils/feimrc.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'gsharov@mrc-lmb.cam.ac.uk'
 # *
 # **************************************************************************
 
 """ This script parses MRC 2014 FEI1/FEI2 file header. """
 
+import os
+import sys
 import mrcfile
 import math
 
 from ..config import DEBUG, SCOPE_DICT
 
 
 def parseMrc(fn):
     acqDict = {}
     with mrcfile.open(fn, header_only=True) as mrc:
         main = mrc.header
-        ext = mrc.extended_header
+        ext = mrc.indexed_extended_header
 
     for item in main.dtype.names:
         acqDict[item] = main[item]
 
     if len(ext):
         for item in ext.dtype.names:
             acqDict[item] = ext[item][0]
@@ -93,7 +95,16 @@
         stdDict['PhasePlatePosition'] = acqDict['Phase plate position index']
 
     # convert all to str
     for key in stdDict:
         stdDict[key] = str(stdDict[key])
 
     return stdDict
+
+
+def main():
+    if len(sys.argv) == 2:
+        result = parseMrc(sys.argv[1])
+        for k, v in sorted(result.items()):
+            print("%s = %s" % (k, v))
+    else:
+        raise ValueError(f"Unrecognized input, please use: {os.path.basename(sys.argv[0])} filename")
```

### Comparing `MDCatch-2.4/mdcatch/utils/feixml.py` & `MDCatch-2.5/mdcatch/utils/feixml.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'gsharov@mrc-lmb.cam.ac.uk'
 # *
 # **************************************************************************
 
 """ This script parses FEI EPU xml file. """
 
+import os
+import sys
 import math
 import xml.etree.ElementTree as ET
 
 from ..config import DEBUG, SCOPE_DICT
 
 
 def parseXml(fn):
@@ -66,39 +68,39 @@
 
     for key in items:
         try:
             acqDict[key] = root.find(items[key].format(**nspace)).text
         except:
             pass
 
-    if acqDict['MicroscopeID'] in SCOPE_DICT:
+    if acqDict.get('MicroscopeID', None) in SCOPE_DICT:
         acqDict['Cs'] = SCOPE_DICT[acqDict['MicroscopeID']][1]
 
-    acqDict['BeamSize'] = float(acqDict['BeamSize']) * math.pow(10, 6)
-    acqDict['Voltage'] = int(acqDict['Voltage']) // 1000
-    acqDict['Binning'] = int(acqDict['Binning'])
+    acqDict['BeamSize'] = float(acqDict.get('BeamSize', 0)) * math.pow(10, 6)
+    acqDict['Voltage'] = int(acqDict.get('Voltage', 0)) // 1000
+    acqDict['Binning'] = int(acqDict.get('Binning', 0))
 
     # get cameraSpecificInput: ElectronCountingEnabled, SuperResolutionFactor etc.
     customDict = dict()
     keys = "./{so}microscopeData/{so}acquisition/{so}camera/{so}CameraSpecificInput/{ar}KeyValueOfstringanyType/{ar}Key"
     values = "./{so}microscopeData/{so}acquisition/{so}camera/{so}CameraSpecificInput/{ar}KeyValueOfstringanyType/{ar}Value"
     for k, v in zip(root.findall(keys.format(**nspace)), root.findall(values.format(**nspace))):
         customDict[k.text] = v.text
 
     # check if counting/super-res is enabled
     sr = 1.0
     acqDict['Mode'] = 'Linear'
-    if customDict['ElectronCountingEnabled'] == 'true':
+    if customDict.get('ElectronCountingEnabled', "false") == 'true':
         sr = float(customDict['SuperResolutionFactor'])  # 1 - counting, 2 - super-res
         acqDict['Mode'] = 'Counting' if sr == 1.0 else 'Super-resolution'
 
     # EPU's pixel size refers to a physical pixel, which is already multiplied by Binning factor
-    acqDict['PixelSpacing'] = float(acqDict['PixelSpacing']) * math.pow(10, 10) / sr
+    acqDict['PixelSpacing'] = float(acqDict.get('PixelSpacing', 0)) * math.pow(10, 10) / sr
 
-    if acqDict['Detector'] == 'EF-CCD':
+    if acqDict.get('Detector', None) == 'EF-CCD':
         elem = "./{so}microscopeData/{so}acquisition/{so}camera/{so}CameraSpecificInput/{ar}KeyValueOfstringanyType/{ar}Value/{fr}NumberOffractions"
         acqDict['NumSubFrames'] = root.find(elem.format(**nspace)).text
     else:
         # count number of DoseFractions for Falcon 3
         elem = "./{so}microscopeData/{so}acquisition/{so}camera/{so}CameraSpecificInput/{ar}KeyValueOfstringanyType/{ar}Value/{fr}DoseFractions"
         try:
             acqDict['NumSubFrames'] = len(root.find(elem.format(**nspace)))
@@ -109,16 +111,21 @@
     customDict = dict()
     keys = "./{so}CustomData/{ar}KeyValueOfstringanyType/{ar}Key"
     values = "./{so}CustomData/{ar}KeyValueOfstringanyType/{ar}Value"
     for k, v in zip(root.findall(keys.format(**nspace)), root.findall(values.format(**nspace))):
         customDict[k.text] = v.text
 
     if 'Detectors[BM-Falcon].EerGainReference' in customDict:
-        acqDict['NumSubFrames'] = int(int(float(acqDict['ExposureTime']) * 248.6943) * 31 / 32)
+        acqDict['NumSubFrames'] = int(int(float(acqDict['ExposureTime']) * float(customDict['Detectors[BM-Falcon].FrameRate'])) * 31 / 32)
         acqDict['Mode'] = "EER"
+        acqDict['GainReference'] = os.path.basename(customDict['Detectors[BM-Falcon].EerGainReference'])
+    elif 'Detectors[EF-Falcon].EerGainReference' in customDict:
+        acqDict['NumSubFrames'] = int(int(float(acqDict['ExposureTime']) * float(customDict['Detectors[EF-Falcon].FrameRate'])) * 31 / 32)
+        acqDict['Mode'] = "EER"
+        acqDict['GainReference'] = os.path.basename(customDict['Detectors[EF-Falcon].EerGainReference'])
     if 'AppliedDefocus' in customDict:
         acqDict['AppliedDefocus'] = float(customDict['AppliedDefocus']) * math.pow(10, 6)
     if 'Dose' in customDict:
         acqDict['Dose'] = float(customDict['Dose']) * math.pow(10, -20)
     if 'PhasePlateUsed' in customDict:
         acqDict['PhasePlateUsed'] = customDict['PhasePlateUsed']
     if 'Aperture[C2].Name' in customDict:
@@ -135,7 +142,16 @@
             print("%s = %s" % (k, v))
 
     # convert all to str
     for key in acqDict:
         acqDict[key] = str(acqDict[key])
 
     return acqDict
+
+
+def main():
+    if len(sys.argv) == 2:
+        result = parseXml(sys.argv[1])
+        for k, v in sorted(result.items()):
+            print("%s = %s" % (k, v))
+    else:
+        raise ValueError(f"Unrecognized input, please use: {os.path.basename(sys.argv[0])} filename")
```

### Comparing `MDCatch-2.4/mdcatch/utils/mdoc.py` & `MDCatch-2.5/mdcatch/utils/mdoc.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,48 +22,49 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'gsharov@mrc-lmb.cam.ac.uk'
 # *
 # **************************************************************************
 
 """ This script parses mdoc files from SerialEM. """
 
+import os
+import sys
 import re
 
 from ..config import DEBUG, SERIALEM_PARAMS, SCOPE_DICT
 
 
-REGEX_MDOC_VAR = "(?P<var>[a-zA-Z0-9]+?) = (?P<value>(.*))"
+REGEX_MDOC_VAR = "(?P<var>[a-zA-Z0-9]+?) = (?P<value>.*)"
 
 
 def parseMdoc(fn):
     # we assume SerialEM is only used for Gatan detectors
     acqDict = {'Detector': 'EF-CCD'}
 
     with open(fn, 'r') as fname:
         regex = re.compile(REGEX_MDOC_VAR)
-
+        scope_id = None
         for line in fname:
-            match = regex.match(line)
-            if match and match.groupdict()['var'] in SERIALEM_PARAMS:
-                key = match.groupdict()['var']
-                acqDict[key] = match.groupdict()['value'].strip()
-
-    # rename a few keys to match EPU
-    # T = SerialEM: Acquired on Titan Krios D3593
-    match = re.search("D[0-9]{3,10}", acqDict['T'])
-    if match:
-        value = match.group().replace('D', '')
-        acqDict['MicroscopeID'] = value
-        acqDict.pop('T')
-        if value in SCOPE_DICT:
-            acqDict['Cs'] = str(SCOPE_DICT[value][1])
+            if "[T = SerialEM" in line:
+                match = re.search("D[0-9]{3,10}", line)
+                scope_id = match.group().replace('D', '')
+            else:
+                match = regex.match(line)
+                if match and match.groupdict()['var'] in SERIALEM_PARAMS:
+                    key = match.groupdict()['var']
+                    acqDict[key] = match.groupdict()['value'].strip()
+
+    if scope_id is not None:
+        acqDict['MicroscopeID'] = scope_id
+        if scope_id in SCOPE_DICT:
+            acqDict['Cs'] = str(SCOPE_DICT[scope_id][1])
     else:
         print("ERROR: Could not detect MicroscopeID (D####) from mdoc!\n"
               "Make sure you have e.g. the following line in the mdoc:\n"
-              "T = SerialEM: Acquired on Titan Krios D3593")
+              "[T = SerialEM: Acquired on Titan Krios D3593]")
         exit(1)
 
     if 'ExposureDose' in acqDict:
         acqDict['Dose'] = acqDict.pop('ExposureDose')
     if 'TargetDefocus' in acqDict:
         acqDict['AppliedDefocus'] = acqDict.pop('TargetDefocus')
     if 'Binning' in acqDict:
@@ -76,7 +77,16 @@
         acqDict['PhasePlateUsed'] = acqDict.pop('PhasePlateInserted')
 
     if DEBUG:
         for k, v in sorted(acqDict.items()):
             print("%s = %s" % (k, v))
 
     return acqDict
+
+
+def main():
+    if len(sys.argv) == 2:
+        result = parseMdoc(sys.argv[1])
+        for k, v in sorted(result.items()):
+            print("%s = %s" % (k, v))
+    else:
+        raise ValueError(f"Unrecognized input, please use: {os.path.basename(sys.argv[0])} filename")
```

### Comparing `MDCatch-2.4/mdcatch/utils/misc.py` & `MDCatch-2.5/mdcatch/utils/misc.py`

 * *Files identical despite different names*

### Comparing `MDCatch-2.4/mdcatch/utils/tiff.py` & `MDCatch-2.5/mdcatch/utils/tiff.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'gsharov@mrc-lmb.cam.ac.uk'
 # *
 # **************************************************************************
 
 """ This script parses TIFF file header. """
 
+import os
+import sys
 from tifffile import TiffFile
 
 from ..config import DEBUG, SCOPE_DICT
 
 
 # See https://www.awaresystems.be/imaging/tiff/tifftags/baseline.html
 
@@ -145,7 +147,16 @@
     stdDict['Cs'] = SCOPE_DICT[stdDict['MicroscopeID']][1]
 
     # convert all to str
     for key in stdDict:
         stdDict[key] = str(stdDict[key])
 
     return stdDict
+
+
+def main():
+    if len(sys.argv) == 2:
+        result = parseTif(sys.argv[1])
+        for k, v in sorted(result.items()):
+            print("%s = %s" % (k, v))
+    else:
+        raise ValueError(f"Unrecognized input, please use: {os.path.basename(sys.argv[0])} filename")
```

### Comparing `MDCatch-2.4/setup.py` & `MDCatch-2.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,13 +49,19 @@
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3'
     ],
     keywords='cryo-em python qt6 epu serialem',
     packages=find_packages(),
     install_requires=['pyqt6', 'mrcfile', 'tifffile', 'emtable'],
-    entry_points={'console_scripts': ['mdcatch=mdcatch.run:main']},
+    entry_points={'console_scripts': [
+        'mdcatch=mdcatch.run:main',
+        'parse-mrc=mdcatch.utils.feimrc:main',
+        'parse-xml=mdcatch.utils.feixml:main',
+        'parse-tif=mdcatch.utils.tiff:main',
+        'parse-mdoc=mdcatch.utils.mdoc:main'
+    ]},
     project_urls={
         'Bug Reports': 'https://github.com/azazellochg/MDCatch/issues',
         'Source': 'https://github.com/azazellochg/MDCatch',
     },
 )
```

