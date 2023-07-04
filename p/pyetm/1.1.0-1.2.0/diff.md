# Comparing `tmp/pyetm-1.1.0.tar.gz` & `tmp/pyetm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetm-1.1.0.tar", last modified: Wed Apr 26 11:30:47 2023, max compression
+gzip compressed data, was "pyetm-1.2.0.tar", last modified: Tue Jul  4 10:57:30 2023, max compression
```

## Comparing `pyetm-1.1.0.tar` & `pyetm-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.924389 pyetm-1.1.0/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    13827 2023-01-10 21:51:08.000000 pyetm-1.1.0/LICENSE
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-04-26 11:30:47.923390 pyetm-1.1.0/PKG-INFO
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      253 2023-01-10 21:51:08.000000 pyetm-1.1.0/README.md
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1324 2023-04-26 11:28:26.000000 pyetm-1.1.0/pyproject.toml
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       38 2023-04-26 11:30:47.924389 pyetm-1.1.0/setup.cfg
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.917389 pyetm-1.1.0/src/
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.918390 pyetm-1.1.0/src/pyetm/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       50 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/__init__.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.920390 pyetm-1.1.0/src/pyetm/client/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       52 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4631 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/account.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10187 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/client.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6621 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/client/curves.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11611 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/customcurves.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2279 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/gqueries.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4032 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/meritorder.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12654 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/parameters.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12419 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/scenario.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6737 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/session.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2256 2023-02-23 15:22:38.000000 pyetm-1.1.0/src/pyetm/client/transitionpaths.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8278 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/client/utils.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1323 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exceptions.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/exchange/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       45 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8531 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/checks.py
--rwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    27650 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/market.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11632 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/plotting.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    16503 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/exchange/region.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3231 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/logger.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/myc/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       51 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/myc/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    29789 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/myc/model.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3578 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/optional.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/profiles/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      119 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/__init__.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.921389 pyetm-1.1.0/src/pyetm/profiles/capacityfactors/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4770 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/capacityfactors/__init__.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.922390 pyetm-1.1.0/src/pyetm/profiles/weather/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3046 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5718 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/buildings.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2718 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/cooling.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10702 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/households.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5984 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/profiles/weather/smoothing.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.922390 pyetm-1.1.0/src/pyetm/sessions/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      101 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/sessions/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10546 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/sessions/aiohttp.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7600 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/sessions/requests.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.923390 pyetm-1.1.0/src/pyetm/utils/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      278 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/utils/__init__.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4987 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/categorisation.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5131 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/utils/converter.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7153 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/excel.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6207 2023-04-26 11:28:26.000000 pyetm-1.1.0/src/pyetm/utils/interpolation.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      503 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/lookup.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      559 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/loop.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3704 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/profiles.py
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4990 2023-04-24 21:36:47.000000 pyetm-1.1.0/src/pyetm/utils/regionalisation.py
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.919390 pyetm-1.1.0/src/pyetm.egg-info/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/PKG-INFO
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1486 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/SOURCES.txt
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        1 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/dependency_links.txt
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      177 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/requires.txt
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        6 2023-04-26 11:30:47.000000 pyetm-1.1.0/src/pyetm.egg-info/top_level.txt
-drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-04-26 11:30:47.923390 pyetm-1.1.0/tests/
--rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1709 2023-04-24 21:36:47.000000 pyetm-1.1.0/tests/test_utils.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.710732 pyetm-1.2.0/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    13827 2023-01-10 21:51:08.000000 pyetm-1.2.0/LICENSE
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-07-04 10:57:30.710732 pyetm-1.2.0/PKG-INFO
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      253 2023-01-10 21:51:08.000000 pyetm-1.2.0/README.md
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1324 2023-07-04 10:52:27.000000 pyetm-1.2.0/pyproject.toml
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       38 2023-07-04 10:57:30.710732 pyetm-1.2.0/setup.cfg
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.702732 pyetm-1.2.0/src/
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.704732 pyetm-1.2.0/src/pyetm/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       50 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/__init__.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.706732 pyetm-1.2.0/src/pyetm/client/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       52 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/client/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4631 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/client/account.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10066 2023-07-04 10:52:27.000000 pyetm-1.2.0/src/pyetm/client/client.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6621 2023-04-26 11:28:26.000000 pyetm-1.2.0/src/pyetm/client/curves.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11611 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/client/customcurves.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2279 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/client/gqueries.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4032 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/client/meritorder.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12654 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/client/parameters.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    12239 2023-07-04 10:52:27.000000 pyetm-1.2.0/src/pyetm/client/scenario.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7023 2023-07-04 10:52:27.000000 pyetm-1.2.0/src/pyetm/client/session.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2256 2023-02-23 15:22:38.000000 pyetm-1.2.0/src/pyetm/client/transitionpaths.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8278 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/client/utils.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1323 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/exceptions.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.707732 pyetm-1.2.0/src/pyetm/exchange/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       45 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/exchange/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     8531 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/exchange/checks.py
+-rwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    27650 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/exchange/market.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    11632 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/exchange/plotting.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    16503 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/exchange/region.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3231 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/logger.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.707732 pyetm-1.2.0/src/pyetm/myc/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)       51 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/myc/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    31630 2023-07-04 10:52:27.000000 pyetm-1.2.0/src/pyetm/myc/model.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3578 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/optional.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.707732 pyetm-1.2.0/src/pyetm/profiles/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      119 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/profiles/__init__.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.707732 pyetm-1.2.0/src/pyetm/profiles/capacityfactors/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4770 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/profiles/capacityfactors/__init__.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.708732 pyetm-1.2.0/src/pyetm/profiles/weather/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3046 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/profiles/weather/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5718 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/profiles/weather/buildings.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     2718 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/profiles/weather/cooling.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10702 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/profiles/weather/households.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5984 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/profiles/weather/smoothing.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.708732 pyetm-1.2.0/src/pyetm/sessions/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      101 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/sessions/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    10546 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/sessions/aiohttp.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7600 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/sessions/requests.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.710732 pyetm-1.2.0/src/pyetm/utils/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      278 2023-04-26 11:28:26.000000 pyetm-1.2.0/src/pyetm/utils/__init__.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4987 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/utils/categorisation.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     5131 2023-04-26 11:28:26.000000 pyetm-1.2.0/src/pyetm/utils/converter.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     7153 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/utils/excel.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     6207 2023-04-26 11:28:26.000000 pyetm-1.2.0/src/pyetm/utils/interpolation.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      503 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/utils/lookup.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      559 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/utils/loop.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     3704 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/utils/profiles.py
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     4990 2023-04-24 21:36:47.000000 pyetm-1.2.0/src/pyetm/utils/regionalisation.py
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.705732 pyetm-1.2.0/src/pyetm.egg-info/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)    17409 2023-07-04 10:57:30.000000 pyetm-1.2.0/src/pyetm.egg-info/PKG-INFO
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1486 2023-07-04 10:57:30.000000 pyetm-1.2.0/src/pyetm.egg-info/SOURCES.txt
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        1 2023-07-04 10:57:30.000000 pyetm-1.2.0/src/pyetm.egg-info/dependency_links.txt
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)      177 2023-07-04 10:57:30.000000 pyetm-1.2.0/src/pyetm.egg-info/requires.txt
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        6 2023-07-04 10:57:30.000000 pyetm-1.2.0/src/pyetm.egg-info/top_level.txt
+drwxr-xr-x   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)        0 2023-07-04 10:57:30.710732 pyetm-1.2.0/tests/
+-rw-r--r--   0 104063@ontw.alfa.local (978411622) domain users@ontw.alfa.local (978400513)     1709 2023-04-24 21:36:47.000000 pyetm-1.2.0/tests/test_utils.py
```

### Comparing `pyetm-1.1.0/LICENSE` & `pyetm-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/PKG-INFO` & `pyetm-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyetm
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python-ETM Connector
 Author-email: Rob Calon <robcalon@protonmail.com>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
```

### Comparing `pyetm-1.1.0/pyproject.toml` & `pyetm-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyetm"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python-ETM Connector"
 authors = [{name = "Rob Calon", email = "robcalon@protonmail.com"}]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 dependencies = ['requests>=2.26', 'pandas>=2.0']
 keywords = ["ETM", "Energy Transition Model"]
```

### Comparing `pyetm-1.1.0/src/pyetm/client/account.py` & `pyetm-1.2.0/src/pyetm/client/account.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/client/client.py` & `pyetm-1.2.0/src/pyetm/client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -187,37 +187,36 @@
 
         return cls.from_existing_scenario(
             scenario_id, metadata, keep_compatible, private, **kwargs)
 
     def __init__(
         self,
         scenario_id: str | None = None,
-        beta_engine: bool = False,
-        reset: bool = False,
+        engine_url: str | None = None,
+        etm_url: str | None = None,
         token: str | None = None,
         session: RequestsSession | AIOHTTPSession | None = None,
         **kwargs
     ):
         """client object to process ETM requests via its public API
 
         Parameters
         ----------
         scenario_id : str, default None
             The api_session_id to which the client connects. Can only access
             a limited number of methods when scenario_id is set to None.
-        beta_engine : bool, default False
-            Connect to the beta-engine instead of the production-engine.
-        reset : bool, default False
-            Reset scenario on initalization.
         token : str, default None
             Personal access token to authenticate requests to your
             personal account and scenarios. Detects token automatically
-            from environment when assigned to ETM_ACCESS_TOKEN when
-            connected to production or ETM_BETA_ACCESS_TOKEN when
-            connected to beta.
+            from environment when assigned to ETM_ACCESS_TOKEN.
+        engine_url : str, default None
+            Specify URL that points to ETM engine, default to public engine.
+        etm_url : str, default None
+            Specify URL that points to ETM model (pro), default to public
+            energy transition model.
         session: object instance, default None
             session instance that handles requests to ETM's public API.
             Default to use a RequestsSession.
 
         All key-word arguments are passed directly to the init method
         of the default session instance. All key-word arguments are
         ignored when the session argument is not None.
@@ -234,27 +233,24 @@
             session = RequestsSession(**kwargs)
 
         # set session
         self.__kwargs = kwargs
         self._session = session
 
         # set engine and token
-        self.beta_engine = beta_engine
+        self.engine_url = engine_url
+        self.etm_url = etm_url
         self.token = token
 
         # set scenario id
         self.scenario_id = scenario_id
 
         # set default gqueries
         self.gqueries = []
 
-        # reset scenario on intialization
-        if reset and (scenario_id is not None):
-            self.reset_scenario()
-
         # make message
         msg = (
             "Initialised new Client: "
                 f"'scenario_id={self.scenario_id}, "
                 f"area_code={self.area_code}, "
                 f"end_year={self.end_year}'"
         )
@@ -278,15 +274,15 @@
     def __repr__(self):
         """reproduction string"""
 
         # get initialization parameters
         params = {
             **{
                 "scenario_id": self.scenario_id,
-                "beta_engine": self.beta_engine,
+                "engine_url": self.engine_url,
                 "session": self.session
                 },
             **self.__kwargs
             }
 
         # object environment
         env = ", ".join(f'{k}={v}' for k, v in params.items())
```

### Comparing `pyetm-1.1.0/src/pyetm/client/curves.py` & `pyetm-1.2.0/src/pyetm/client/curves.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/client/customcurves.py` & `pyetm-1.2.0/src/pyetm/client/customcurves.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/client/gqueries.py` & `pyetm-1.2.0/src/pyetm/client/gqueries.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/client/meritorder.py` & `pyetm-1.2.0/src/pyetm/client/meritorder.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/client/parameters.py` & `pyetm-1.2.0/src/pyetm/client/parameters.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/client/scenario.py` & `pyetm-1.2.0/src/pyetm/client/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Authentication methods"""
 
 from __future__ import annotations
-# from pathlib import Path
 
 import copy
+from urllib.parse import urljoin
 
 import pandas as pd
 from .session import SessionMethods
 
 
 class ScenarioMethods(SessionMethods):
     """Base scenario methods"""
@@ -83,23 +83,15 @@
         # format header and update
         header = {'private': str(bool(boolean)).lower()}
         self._update_scenario_header(header)
 
     @property
     def pro_url(self) -> str:
         """get pro url for session id"""
-
-        # specify base url
-        base = 'https://energytransitionmodel.com'
-
-        # update to beta server
-        if self.beta_engine:
-            base = base.replace('https://', 'https://beta.')
-
-        return f'{base}/scenarios/{self.scenario_id}/load'
+        return urljoin(self.etm_url, f'scenarios/{self.scenario_id}/load/')
 
     @property
     def scaling(self):
         """applied scaling factor"""
         return self._scenario_header.get('scaling')
 
     @property
```

### Comparing `pyetm-1.1.0/src/pyetm/client/session.py` & `pyetm-1.2.0/src/pyetm/client/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import Literal
 
 import os
 import re
 import copy
 import functools
 
+from urllib.parse import urljoin
+
 import pandas as pd
 
 from pyetm.logger import get_modulelogger
 from pyetm.sessions import RequestsSession, AIOHTTPSession
 
 # get modulelogger
 logger = get_modulelogger(__name__)
@@ -18,48 +20,71 @@
 SCOPE = Literal['public', 'read', 'write', 'delete']
 
 
 class SessionMethods:
     """Core methods for API interaction"""
 
     @property
+    def _default_engine_url(self) -> str:
+        """default engine url"""
+        return "https://engine.energytransitionmodel.com/api/v3/"
+
+    @property
+    def connected_to_default_engine(self) -> bool:
+        """connected to default engine url?"""
+        return self.engine_url == self._default_engine_url
+
+    @property
     def _scenario_header(self) -> dict:
         """get full scenario header"""
         return self._get_scenario_header()
 
     @property
-    def base_url(self) -> str:
-        """"base url for carbon transition model"""
-
-        # return beta engine url
-        if self.beta_engine:
-            return "https://beta-engine.energytransitionmodel.com/api/v3/"
+    def engine_url(self) -> str:
+        """engine URL"""
+        return self._engine_url
 
-        return "https://engine.energytransitionmodel.com/api/v3/"
+    @engine_url.setter
+    def engine_url(self, url: str | None):
 
-    @property
-    def beta_engine(self) -> bool:
-        """connects to beta-engine when True and to production-engine
-        when False."""
-        return self._beta_engine
-
-    @beta_engine.setter
-    def beta_engine(self, boolean: bool) -> None:
-        """set beta engine attribute"""
+        # default url
+        if url is None:
+            url = self._default_engine_url
 
-        # set boolean and reset session
-        self._beta_engine = bool(boolean)
+        # set engine
+        self._engine_url = str(url)
 
-        # set related settings
+        # reset token and change base url
         self.token = None
-        self.session.base_url = self.base_url
+        self.session.base_url = self._engine_url
 
+        # reset cache
         self._reset_cache()
 
     @property
+    def etm_url(self) -> str:
+        """model URL"""
+
+        # raise error
+        if self.etm_url is None:
+            raise ValueError("ETModel URL not set on initialisation.")
+
+        return self._etm_url
+
+    @etm_url.setter
+    def etm_url(self, url: str | None):
+
+        # use default pro location
+        if (url is None) & (self.connected_to_default_engine):
+            url = "https://energytransitionmodel.com/"
+
+        # set etmodel
+        self._etm_url = str(url)
+
+    @property
     def scenario_id(self) -> int | None:
         """scenario id"""
         return self._scenario_id if hasattr(self, '_scenario_id') else None
 
     @scenario_id.setter
     def scenario_id(self, scenario_id: int | None):
 
@@ -109,22 +134,18 @@
         resp['expires_in'] = pd.Timedelta(resp['expires_in'], unit='s')
 
         return pd.Series(resp, name='token')
 
     @token.setter
     def token(self, token: str | None = None):
 
-        # check environment variables for production token
-        if (token is None) & (not self.beta_engine):
+        # check environment variables for token
+        if token is None:
             token = os.getenv('ETM_ACCESS_TOKEN')
 
-        # check environment variables for beta token
-        if (token is None) & self.beta_engine:
-            token = os.getenv('ETM_BETA_ACCESS_TOKEN')
-
         # store token
         self._token = token
 
         # update persistent session headers
         if self._token is None:
 
             # pop authorization if present
@@ -175,19 +196,16 @@
         header = self.session.get(url)
 
         return header
 
     def _get_session_id(self, scenario_id: int) -> int:
         """get a session_id for a pro-environment scenario"""
 
-        # make pro url
-        host = "https://energytransitionmodel.com"
-        url = f"{host}/saved_scenarios/{scenario_id}/load"
-
         # extract content from url
+        url = urljoin(self.etm_url, f'saved_scenarios/{scenario_id}/load/')
         content = self.session.request("get", url, decoder='text')
 
         # get session id from content
         pattern = '"api_session_id":([0-9]{6,7})'
         session_id = re.search(pattern, content)
 
         return int(session_id.group(1))
```

### Comparing `pyetm-1.1.0/src/pyetm/client/transitionpaths.py` & `pyetm-1.2.0/src/pyetm/client/transitionpaths.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/client/utils.py` & `pyetm-1.2.0/src/pyetm/client/utils.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/exceptions.py` & `pyetm-1.2.0/src/pyetm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/exchange/checks.py` & `pyetm-1.2.0/src/pyetm/exchange/checks.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/exchange/market.py` & `pyetm-1.2.0/src/pyetm/exchange/market.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/exchange/plotting.py` & `pyetm-1.2.0/src/pyetm/exchange/plotting.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/exchange/region.py` & `pyetm-1.2.0/src/pyetm/exchange/region.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/logger.py` & `pyetm-1.2.0/src/pyetm/logger.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/myc/model.py` & `pyetm-1.2.0/src/pyetm/myc/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """myc access"""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal
+from urllib.parse import urljoin
 
 import datetime
 import numpy as np
 import pandas as pd
 
 from pyetm import Client
 from pyetm.utils import categorise_curves
@@ -42,14 +43,39 @@
 
     return frame
 
 class MYCClient():
     """Multi Year Chart Client"""
 
     @property
+    def myc_url(self) -> str:
+        """specifies URL that points to mutli-year charts."""
+        return self._myc_url
+
+    @myc_url.setter
+    def myc_url(self, url: str | None):
+
+        if url is None:
+
+            # check for default engine
+            with Client(**self._kwargs) as client:
+                default_engine = client.connected_to_default_engine
+
+            # pass default engine myc URL
+            if default_engine is True:
+                url = "https://myc.energytransitionmodel.com/"
+
+            else:
+                # raise for missing myc URL
+                raise ValueError("must specify the related "
+                    "custom myc_url for the specified custom engine_url.")
+
+        self._myc_url = str(url)
+
+    @property
     def session_ids(self) -> pd.Series:
         """series of scenario_ids"""
         return self.__session_ids
 
     @session_ids.setter
     def session_ids(self, session_ids: pd.Series):
 
@@ -192,14 +218,15 @@
 
     def __init__(
         self,
         session_ids: pd.Series,
         parameters: pd.Series, gqueries: pd.Series,
         mapping: pd.Series | pd.DataFrame | None = None,
         reference: str | None = None,
+        myc_url: str | None = None,
         **kwargs
     ):
         """initialisation logic for Client.
 
         Parameters
         ----------
         session_ids: pd.Series
@@ -212,19 +239,21 @@
             gquery unit.
         mapping : pd.Series or pd.DataFrame
             Optional mapping for carrier curves output keys.
         reference : str, default None
             Key of reference scenario. This scenario will be
             excluded from the MYC links and will always be
             placed in front when sorting results.
+        myc_url : str, default None
+            Specify URL that points to ETM MYC, default to public
+            multi-year charts.
 
         All key-word arguments are passed directly to the Session
         that is used in combination with the pyetm.client. In this
-        module the pyetm.Client uses a Requests Session object as
-        backend.
+        module the pyetm.Client uses a Requests Session object by default.
 
         Keyword Arguments
         -----------------
         base_url: str, default None
             Base url to which the session connects, all request urls
             will be merged with the base url to create a destination.
         proxies: dict, default None
@@ -241,27 +270,50 @@
             your application vulnerable to man-in-the-middle (MitM) attacks.
             Setting verify to False may be useful during local development or
             testing.
         cert: string or tuple, default None
             If string; path to ssl client cert file (.pem).
             If tuple; ('cert', 'key') pair."""
 
+        # set kwargs
+        self._kwargs = kwargs
+
         # set optional parameters
         self.session_ids = session_ids
         self.parameters = parameters
         self.gqueries = gqueries
         self.mapping = mapping
         self.reference = reference
-
-        # set kwargs
-        self._kwargs = kwargs
+        self.myc_url = myc_url
 
     @classmethod
-    def from_excel(cls, filepath: str, **kwargs):
-        """initate from excel file with standard structure"""
+    def from_excel(
+        cls,
+        filepath: str,
+        reference: str | None = None,
+        myc_url: str | None = None,
+        **kwargs
+    ):
+        """initate from excel file with standard structure
+
+        Parameters
+        ----------
+        filepath : str
+            Path to excel file that is red.
+        reference : str, default None
+            Key of reference scenario. This scenario will be
+            excluded from the MYC links and will always be
+            placed in front when sorting results.
+        myc_url : str, default None
+            Specify URL that points to ETM MYC, default to public
+            multi-year charts.
+
+        All key-word arguments are passed directly to the Session that is
+        used in combination with the pyetm.client. In this module the
+        pyetm.Client uses a Requests Session object by default."""
 
         # connect to excel file
         xlsx = pd.ExcelFile(filepath)
 
         # get session ids
         session_ids = pd.read_excel(xlsx, sheet_name='Sessions',
             usecols=[*range(5)], index_col=[*range(4)]).squeeze('columns')
@@ -283,16 +335,23 @@
 
         else:
 
             # default mapping
             mapping = None
 
         # intialize model
-        model = cls(session_ids=session_ids, parameters=parameters,
-            gqueries=gqueries, mapping=mapping, **kwargs)
+        model = cls(
+            session_ids=session_ids,
+            parameters=parameters,
+            gqueries=gqueries,
+            mapping=mapping,
+            reference=reference,
+            myc_url=myc_url,
+            **kwargs
+        )
 
         # set source in model
         model._source = filepath
 
         return model
 
     def _check_for_unmapped_input_parameters(self,
@@ -714,20 +773,18 @@
                 return pd.Series()
 
         _logger.info("making MYC URLS")
 
         levels = "STUDY", "SCENARIO", "REGION"
         grouper = cases.astype(str).groupby(level=levels)
 
-        # convert paths to MYC urls
-        urls = "https://myc.energytransitionmodel.com/"
-        urls += grouper.apply(lambda x: ",".join(x)) + "/inputs"
-
-        # add title
-        urls += "?title=" + urls.index.to_series().str.join("%20")
+        # convert paths to MYC urls and add title
+        urls = grouper.apply(
+            lambda x: urljoin(self.myc_url, ",".join(map(str, x))))
+        urls += "/inputs?title=" + urls.index.to_series().str.join("%20")
 
         return pd.Series(urls, name='URL').sort_index()
 
     def to_excel(self,
         filepath: str | None = None,
         midx: tuple | pd.MultiIndex | None = None,
         input_parameters: bool | pd.DataFrame = True,
```

### Comparing `pyetm-1.1.0/src/pyetm/optional.py` & `pyetm-1.2.0/src/pyetm/optional.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/profiles/capacityfactors/__init__.py` & `pyetm-1.2.0/src/pyetm/profiles/capacityfactors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/profiles/weather/__init__.py` & `pyetm-1.2.0/src/pyetm/profiles/weather/__init__.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/profiles/weather/buildings.py` & `pyetm-1.2.0/src/pyetm/profiles/weather/buildings.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/profiles/weather/cooling.py` & `pyetm-1.2.0/src/pyetm/profiles/weather/cooling.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/profiles/weather/households.py` & `pyetm-1.2.0/src/pyetm/profiles/weather/households.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/profiles/weather/smoothing.py` & `pyetm-1.2.0/src/pyetm/profiles/weather/smoothing.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/sessions/aiohttp.py` & `pyetm-1.2.0/src/pyetm/sessions/aiohttp.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/sessions/requests.py` & `pyetm-1.2.0/src/pyetm/sessions/requests.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/utils/categorisation.py` & `pyetm-1.2.0/src/pyetm/utils/categorisation.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/utils/converter.py` & `pyetm-1.2.0/src/pyetm/utils/converter.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/utils/excel.py` & `pyetm-1.2.0/src/pyetm/utils/excel.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/utils/interpolation.py` & `pyetm-1.2.0/src/pyetm/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/utils/loop.py` & `pyetm-1.2.0/src/pyetm/utils/loop.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/utils/profiles.py` & `pyetm-1.2.0/src/pyetm/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm/utils/regionalisation.py` & `pyetm-1.2.0/src/pyetm/utils/regionalisation.py`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/src/pyetm.egg-info/PKG-INFO` & `pyetm-1.2.0/src/pyetm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyetm
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python-ETM Connector
 Author-email: Rob Calon <robcalon@protonmail.com>
 License:                       EUROPEAN UNION PUBLIC LICENCE v. 1.2
                               EUPL © the European Union 2007, 2016
         
         This European Union Public Licence (the ‘EUPL’) applies to the Work (as defined
         below) which is provided under the terms of this Licence. Any use of the Work,
```

### Comparing `pyetm-1.1.0/src/pyetm.egg-info/SOURCES.txt` & `pyetm-1.2.0/src/pyetm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyetm-1.1.0/tests/test_utils.py` & `pyetm-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

