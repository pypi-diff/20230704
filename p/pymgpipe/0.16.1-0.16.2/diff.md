# Comparing `tmp/pymgpipe-0.16.1.tar.gz` & `tmp/pymgpipe-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymgpipe-0.16.1.tar", last modified: Mon Jul  3 22:54:40 2023, max compression
+gzip compressed data, was "pymgpipe-0.16.2.tar", last modified: Tue Jul  4 00:20:21 2023, max compression
```

## Comparing `pymgpipe-0.16.1.tar` & `pymgpipe-0.16.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.383738 pymgpipe-0.16.1/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.339908 pymgpipe-0.16.1/.github/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.343109 pymgpipe-0.16.1/.github/workflows/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1038 2023-04-27 18:57:29.000000 pymgpipe-0.16.1/.github/workflows/docs.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     3131 2023-07-03 22:51:29.000000 pymgpipe-0.16.1/.github/workflows/python-package.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1144 2023-04-27 19:33:13.000000 pymgpipe-0.16.1/.github/workflows/tests.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2059 2023-06-30 20:10:42.000000 pymgpipe-0.16.1/.gitignore
--rw-r--r--   0 yolimeydan   (501) staff       (20)    11389 2023-05-16 14:54:10.000000 pymgpipe-0.16.1/LICENSE
--rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-03 22:54:40.383470 pymgpipe-0.16.1/PKG-INFO
--rw-r--r--   0 yolimeydan   (501) staff       (20)    14257 2023-07-03 22:41:47.000000 pymgpipe-0.16.1/README.md
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.344541 pymgpipe-0.16.1/docs/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1162 2023-05-05 20:21:07.000000 pymgpipe-0.16.1/docs/conf.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      451 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/docs/index.rst
--rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/docs/modules.rst
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1212 2023-05-11 17:45:24.000000 pymgpipe-0.16.1/docs/pymgpipe.rst
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.345191 pymgpipe-0.16.1/examples/
--rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-05-11 17:28:05.000000 pymgpipe-0.16.1/examples/test_diet.csv
--rw-r--r--   0 yolimeydan   (501) staff       (20)     8480 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/examples/workflow.ipynb
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.362163 pymgpipe-0.16.1/pymgpipe/
--rw-r--r--   0 yolimeydan   (501) staff       (20)      149 2023-07-03 21:57:55.000000 pymgpipe-0.16.1/pymgpipe/__init__.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2206 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/coupling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    14625 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/diet.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     9847 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/fva.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     5283 2023-07-03 21:59:54.000000 pymgpipe-0.16.1/pymgpipe/io.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      341 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/logger.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    12371 2023-06-30 20:03:36.000000 pymgpipe-0.16.1/pymgpipe/main.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1254 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/metrics.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     8900 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/modeling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     6417 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/nmpc.py
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.340576 pymgpipe-0.16.1/pymgpipe/resources/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.364997 pymgpipe-0.16.1/pymgpipe/resources/diets/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2656 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/AverageEuropeanDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2681 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/DACHDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2616 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/GlutenFreeDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2639 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/HighFatLowCarbDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2669 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/HighFiberDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2685 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/HighProteinDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2675 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/MediterraneanDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2657 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/Type2DiabetesDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2655 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/UnhealthyDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2624 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/VeganDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2659 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/VegetarianDiet.txt
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.366496 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaA.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaB.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaC.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaD.xml.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.377566 pymgpipe-0.16.1/pymgpipe/resources/models/
--rw-r--r--   0 yolimeydan   (501) staff       (20)   319554 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.json
--rw-r--r--   0 yolimeydan   (501) staff       (20)   636272 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.mat
--rw-r--r--   0 yolimeydan   (501) staff       (20)  1624449 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml
--rw-r--r--   0 yolimeydan   (501) staff       (20)    75498 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.379632 pymgpipe-0.16.1/pymgpipe/resources/problems/
--rw-r--r--   0 yolimeydan   (501) staff       (20)   113023 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp
--rw-r--r--   0 yolimeydan   (501) staff       (20)    19492 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)   185852 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps
--rw-r--r--   0 yolimeydan   (501) staff       (20)    24457 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.383078 pymgpipe-0.16.1/pymgpipe/tests/
--rw-r--r--   0 yolimeydan   (501) staff       (20)      592 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/conftest.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2092 2023-05-11 17:36:33.000000 pymgpipe-0.16.1/pymgpipe/tests/test_build.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1606 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_coupling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2550 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_diet.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     6096 2023-06-30 20:03:36.000000 pymgpipe-0.16.1/pymgpipe/tests/test_e2e.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1430 2023-04-27 19:31:46.000000 pymgpipe-0.16.1/pymgpipe/tests/test_fva.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1920 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_io.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      723 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_utils.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    11375 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/utils.py
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.362912 pymgpipe-0.16.1/pymgpipe.egg-info/
--rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/PKG-INFO
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1837 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/SOURCES.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)        1 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/dependency_links.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)       46 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/requires.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)        9 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/top_level.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)      226 2023-06-30 20:03:34.000000 pymgpipe-0.16.1/requirements.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)       38 2023-07-03 22:54:40.383783 pymgpipe-0.16.1/setup.cfg
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1589 2023-07-03 22:53:07.000000 pymgpipe-0.16.1/setup.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.407652 pymgpipe-0.16.2/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.379306 pymgpipe-0.16.2/.github/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.382350 pymgpipe-0.16.2/.github/workflows/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1038 2023-04-27 18:57:29.000000 pymgpipe-0.16.2/.github/workflows/docs.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2945 2023-07-03 23:03:04.000000 pymgpipe-0.16.2/.github/workflows/python-package.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1144 2023-04-27 19:33:13.000000 pymgpipe-0.16.2/.github/workflows/tests.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2059 2023-06-30 20:10:42.000000 pymgpipe-0.16.2/.gitignore
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    11389 2023-05-16 14:54:10.000000 pymgpipe-0.16.2/LICENSE
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-04 00:20:21.406953 pymgpipe-0.16.2/PKG-INFO
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    14257 2023-07-03 22:41:47.000000 pymgpipe-0.16.2/README.md
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.383517 pymgpipe-0.16.2/docs/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1162 2023-05-05 20:21:07.000000 pymgpipe-0.16.2/docs/conf.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      451 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/docs/index.rst
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/docs/modules.rst
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1212 2023-05-11 17:45:24.000000 pymgpipe-0.16.2/docs/pymgpipe.rst
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.384311 pymgpipe-0.16.2/examples/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-05-11 17:28:05.000000 pymgpipe-0.16.2/examples/test_diet.csv
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    47496 2023-07-04 00:16:04.000000 pymgpipe-0.16.2/examples/workflow.ipynb
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.387719 pymgpipe-0.16.2/pymgpipe/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      149 2023-07-03 21:57:55.000000 pymgpipe-0.16.2/pymgpipe/__init__.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2206 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/coupling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    14625 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/diet.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     9847 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/fva.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     5283 2023-07-03 21:59:54.000000 pymgpipe-0.16.2/pymgpipe/io.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      341 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/logger.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    12371 2023-06-30 20:03:36.000000 pymgpipe-0.16.2/pymgpipe/main.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1254 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/metrics.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     8900 2023-07-04 00:14:08.000000 pymgpipe-0.16.2/pymgpipe/modeling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     6417 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/nmpc.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.379912 pymgpipe-0.16.2/pymgpipe/resources/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.392590 pymgpipe-0.16.2/pymgpipe/resources/diets/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2656 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/AverageEuropeanDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2681 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/DACHDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2616 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/GlutenFreeDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2639 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/HighFatLowCarbDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2669 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/HighFiberDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2685 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/HighProteinDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2675 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/MediterraneanDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2657 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/Type2DiabetesDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2655 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/UnhealthyDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2624 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/VeganDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2659 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/VegetarianDiet.txt
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.393697 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaA.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaB.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaC.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaD.xml.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.400041 pymgpipe-0.16.2/pymgpipe/resources/models/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   319554 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.json
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   636272 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.mat
+-rw-r--r--   0 yolimeydan   (501) staff       (20)  1624449 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    75498 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.403927 pymgpipe-0.16.2/pymgpipe/resources/problems/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   113023 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    19492 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   185852 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    24457 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.406528 pymgpipe-0.16.2/pymgpipe/tests/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      592 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/conftest.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2092 2023-05-11 17:36:33.000000 pymgpipe-0.16.2/pymgpipe/tests/test_build.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1606 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_coupling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2550 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_diet.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     6096 2023-06-30 20:03:36.000000 pymgpipe-0.16.2/pymgpipe/tests/test_e2e.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1430 2023-04-27 19:31:46.000000 pymgpipe-0.16.2/pymgpipe/tests/test_fva.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1920 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_io.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      723 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_utils.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    11375 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/utils.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.388505 pymgpipe-0.16.2/pymgpipe.egg-info/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/PKG-INFO
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1837 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)        1 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       55 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/requires.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)        9 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/top_level.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      226 2023-06-30 20:03:34.000000 pymgpipe-0.16.2/requirements.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       38 2023-07-04 00:20:21.407710 pymgpipe-0.16.2/setup.cfg
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1608 2023-07-04 00:20:01.000000 pymgpipe-0.16.2/setup.py
```

### Comparing `pymgpipe-0.16.1/.github/workflows/docs.yml` & `pymgpipe-0.16.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/.github/workflows/python-package.yml` & `pymgpipe-0.16.2/.github/workflows/python-package.yml`

 * *Files 5% similar despite different names*

```diff
@@ -62,28 +62,23 @@
     env:
       GITHUB_TOKEN: ${{ secrets.RELEASE }}
     steps:
       - id: release
         uses: rymndhng/release-on-push-action@master
         with:
           tag_prefix: "v"
-          bump_version_scheme: norelease
+          bump_version_scheme: patch
           use_github_release_notes: true
   push-changes:
     runs-on: ubuntu-latest
     name: Push changes
     steps:
     - uses: actions/checkout@v3
       with:
         persist-credentials: false 
         fetch-depth: 0 
-    - name: Write version to file
-      uses: brettdorrans/write-version-to-file@master
-      with:
-        filename: 'pymgpipe/resources/.VERSION'
-        placeholder: '${VERSION}'
     - name: Commit & Push changes to Readme
       if: ${{ github.ref == 'refs/heads/main' }} 
       uses: actions-js/push@master
       with:
         github_token: ${{ secrets.PUSH_README }}
         message: 'Github Actions- Push'
```

### Comparing `pymgpipe-0.16.1/.github/workflows/tests.yml` & `pymgpipe-0.16.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/.gitignore` & `pymgpipe-0.16.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/LICENSE` & `pymgpipe-0.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/PKG-INFO` & `pymgpipe-0.16.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymgpipe
-Version: 0.16.1
+Version: 0.16.2
 Summary: Community level microbiome metabolic modeling in Python
 Home-page: https://github.com/korem-lab/pymgpipe
 Author: Yoli Meydan, Federico Baldini, Tal Korem
 Author-email: ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0
 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/issues
 Project-URL: Source, https://github.com/korem-lab/pymgpipe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.1 Summary: Community level
+Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.2 Summary: Community level
 microbiome metabolic modeling in Python Home-page: https://github.com/korem-
 lab/pymgpipe Author: Yoli Meydan, Federico Baldini, Tal Korem Author-email:
 ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/
 issues Project-URL: Source, https://github.com/korem-lab/pymgpipe Project-URL:
 Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `pymgpipe-0.16.1/README.md` & `pymgpipe-0.16.2/README.md`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/docs/conf.py` & `pymgpipe-0.16.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/docs/pymgpipe.rst` & `pymgpipe-0.16.2/docs/pymgpipe.rst`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/coupling.py` & `pymgpipe-0.16.2/pymgpipe/coupling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/diet.py` & `pymgpipe-0.16.2/pymgpipe/diet.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/fva.py` & `pymgpipe-0.16.2/pymgpipe/fva.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/io.py` & `pymgpipe-0.16.2/pymgpipe/io.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/main.py` & `pymgpipe-0.16.2/pymgpipe/main.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/metrics.py` & `pymgpipe-0.16.2/pymgpipe/metrics.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/modeling.py` & `pymgpipe-0.16.2/pymgpipe/modeling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/nmpc.py` & `pymgpipe-0.16.2/pymgpipe/nmpc.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/AverageEuropeanDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/AverageEuropeanDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/DACHDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/DACHDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/GlutenFreeDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/GlutenFreeDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/HighFatLowCarbDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/HighFatLowCarbDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/HighFiberDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/HighFiberDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/HighProteinDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/HighProteinDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/MediterraneanDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/MediterraneanDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/Type2DiabetesDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/Type2DiabetesDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/UnhealthyDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/UnhealthyDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/VeganDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/VeganDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/diets/VegetarianDiet.txt` & `pymgpipe-0.16.2/pymgpipe/resources/diets/VegetarianDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaA.xml.gz` & `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaA.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaB.xml.gz` & `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaB.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaC.xml.gz` & `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaC.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaD.xml.gz` & `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaD.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.json` & `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.json`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.mat` & `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.mat`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml` & `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml.gz` & `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp` & `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp.gz` & `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps` & `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps.gz` & `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/conftest.py` & `pymgpipe-0.16.2/pymgpipe/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/test_build.py` & `pymgpipe-0.16.2/pymgpipe/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/test_coupling.py` & `pymgpipe-0.16.2/pymgpipe/tests/test_coupling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/test_diet.py` & `pymgpipe-0.16.2/pymgpipe/tests/test_diet.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/test_e2e.py` & `pymgpipe-0.16.2/pymgpipe/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/test_fva.py` & `pymgpipe-0.16.2/pymgpipe/tests/test_fva.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/test_io.py` & `pymgpipe-0.16.2/pymgpipe/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/tests/test_utils.py` & `pymgpipe-0.16.2/pymgpipe/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe/utils.py` & `pymgpipe-0.16.2/pymgpipe/utils.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/pymgpipe.egg-info/PKG-INFO` & `pymgpipe-0.16.2/pymgpipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymgpipe
-Version: 0.16.1
+Version: 0.16.2
 Summary: Community level microbiome metabolic modeling in Python
 Home-page: https://github.com/korem-lab/pymgpipe
 Author: Yoli Meydan, Federico Baldini, Tal Korem
 Author-email: ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0
 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/issues
 Project-URL: Source, https://github.com/korem-lab/pymgpipe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.1 Summary: Community level
+Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.2 Summary: Community level
 microbiome metabolic modeling in Python Home-page: https://github.com/korem-
 lab/pymgpipe Author: Yoli Meydan, Federico Baldini, Tal Korem Author-email:
 ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/
 issues Project-URL: Source, https://github.com/korem-lab/pymgpipe Project-URL:
 Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `pymgpipe-0.16.1/pymgpipe.egg-info/SOURCES.txt` & `pymgpipe-0.16.2/pymgpipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.1/setup.py` & `pymgpipe-0.16.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     author="Yoli Meydan, Federico Baldini, Tal Korem",
     author_email="ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu",
     name="pymgpipe",
     description="Community level microbiome metabolic modeling in Python",
-    version="v0.16.1",
+    version="v0.16.2",
     classifiers=[
         "Intended Audience :: Healthcare Industry",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
@@ -17,14 +17,15 @@
     install_requires=[
         "cobra",
         "optlang",
         "scikit_bio",
         "optlang",
         "tqdm",
         "seaborn",
+        "gurobipy"
     ],
     url="https://github.com/korem-lab/pymgpipe",
     package_dir={"pymgpipe": "pymgpipe"},
     packages=find_packages(include=["pymgpipe"]),
     package_data={
         "pymgpipe": [
             "resources/diets/*.txt",
```

