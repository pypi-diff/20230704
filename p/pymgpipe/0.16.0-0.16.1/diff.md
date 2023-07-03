# Comparing `tmp/pymgpipe-0.16.0.tar.gz` & `tmp/pymgpipe-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymgpipe-0.16.0.tar", last modified: Mon Jul  3 22:28:20 2023, max compression
+gzip compressed data, was "pymgpipe-0.16.1.tar", last modified: Mon Jul  3 22:54:40 2023, max compression
```

## Comparing `pymgpipe-0.16.0.tar` & `pymgpipe-0.16.1.tar`

### file list

```diff
@@ -1,77 +1,76 @@
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.549705 pymgpipe-0.16.0/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.517088 pymgpipe-0.16.0/.github/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.520279 pymgpipe-0.16.0/.github/workflows/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1038 2023-04-27 18:57:29.000000 pymgpipe-0.16.0/.github/workflows/docs.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     3080 2023-06-30 20:32:13.000000 pymgpipe-0.16.0/.github/workflows/python-package.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1144 2023-04-27 19:33:13.000000 pymgpipe-0.16.0/.github/workflows/tests.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2059 2023-06-30 20:10:42.000000 pymgpipe-0.16.0/.gitignore
--rw-r--r--   0 yolimeydan   (501) staff       (20)    11389 2023-05-16 14:54:10.000000 pymgpipe-0.16.0/LICENSE
--rw-r--r--   0 yolimeydan   (501) staff       (20)    15498 2023-07-03 22:28:20.549163 pymgpipe-0.16.0/PKG-INFO
--rw-r--r--   0 yolimeydan   (501) staff       (20)    14650 2023-06-30 20:33:06.000000 pymgpipe-0.16.0/README.md
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.521618 pymgpipe-0.16.0/docs/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1162 2023-05-05 20:21:07.000000 pymgpipe-0.16.0/docs/conf.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      451 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/docs/index.rst
--rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/docs/modules.rst
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1212 2023-05-11 17:45:24.000000 pymgpipe-0.16.0/docs/pymgpipe.rst
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.522321 pymgpipe-0.16.0/examples/
--rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-05-11 17:28:05.000000 pymgpipe-0.16.0/examples/test_diet.csv
--rw-r--r--   0 yolimeydan   (501) staff       (20)     8480 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/examples/workflow.ipynb
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.525896 pymgpipe-0.16.0/pymgpipe/
--rw-r--r--   0 yolimeydan   (501) staff       (20)      149 2023-07-03 21:57:55.000000 pymgpipe-0.16.0/pymgpipe/__init__.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2206 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/coupling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    14625 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/diet.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     9847 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/fva.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     5283 2023-07-03 21:59:54.000000 pymgpipe-0.16.0/pymgpipe/io.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      341 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/logger.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    12371 2023-06-30 20:03:36.000000 pymgpipe-0.16.0/pymgpipe/main.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1254 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/metrics.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     8900 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/modeling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     6417 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/nmpc.py
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.527503 pymgpipe-0.16.0/pymgpipe/resources/
--rw-r--r--   0 yolimeydan   (501) staff       (20)        8 2023-07-03 22:26:31.000000 pymgpipe-0.16.0/pymgpipe/resources/.VERSION
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.529526 pymgpipe-0.16.0/pymgpipe/resources/diets/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2656 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/AverageEuropeanDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2681 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/DACHDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2616 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/GlutenFreeDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2639 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/HighFatLowCarbDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2669 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/HighFiberDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2685 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/HighProteinDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2675 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/MediterraneanDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2657 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/Type2DiabetesDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2655 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/UnhealthyDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2624 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/VeganDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2659 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/diets/VegetarianDiet.txt
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.530436 pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaA.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaB.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaC.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaD.xml.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.535535 pymgpipe-0.16.0/pymgpipe/resources/models/
--rw-r--r--   0 yolimeydan   (501) staff       (20)   319554 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.json
--rw-r--r--   0 yolimeydan   (501) staff       (20)   636272 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.mat
--rw-r--r--   0 yolimeydan   (501) staff       (20)  1624449 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.xml
--rw-r--r--   0 yolimeydan   (501) staff       (20)    75498 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.xml.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.538871 pymgpipe-0.16.0/pymgpipe/resources/problems/
--rw-r--r--   0 yolimeydan   (501) staff       (20)   113023 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.lp
--rw-r--r--   0 yolimeydan   (501) staff       (20)    19492 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.lp.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)   185852 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.mps
--rw-r--r--   0 yolimeydan   (501) staff       (20)    24457 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.mps.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.546149 pymgpipe-0.16.0/pymgpipe/tests/
--rw-r--r--   0 yolimeydan   (501) staff       (20)      592 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/tests/conftest.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2092 2023-05-11 17:36:33.000000 pymgpipe-0.16.0/pymgpipe/tests/test_build.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1606 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/tests/test_coupling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2550 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/tests/test_diet.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     6096 2023-06-30 20:03:36.000000 pymgpipe-0.16.0/pymgpipe/tests/test_e2e.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1430 2023-04-27 19:31:46.000000 pymgpipe-0.16.0/pymgpipe/tests/test_fva.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1920 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/tests/test_io.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      723 2023-04-27 18:09:14.000000 pymgpipe-0.16.0/pymgpipe/tests/test_utils.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    11375 2023-05-18 15:36:12.000000 pymgpipe-0.16.0/pymgpipe/utils.py
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:28:20.527380 pymgpipe-0.16.0/pymgpipe.egg-info/
--rw-r--r--   0 yolimeydan   (501) staff       (20)    15498 2023-07-03 22:28:20.000000 pymgpipe-0.16.0/pymgpipe.egg-info/PKG-INFO
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1865 2023-07-03 22:28:20.000000 pymgpipe-0.16.0/pymgpipe.egg-info/SOURCES.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)        1 2023-07-03 22:28:20.000000 pymgpipe-0.16.0/pymgpipe.egg-info/dependency_links.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)       46 2023-07-03 22:28:20.000000 pymgpipe-0.16.0/pymgpipe.egg-info/requires.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)        9 2023-07-03 22:28:20.000000 pymgpipe-0.16.0/pymgpipe.egg-info/top_level.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)      226 2023-06-30 20:03:34.000000 pymgpipe-0.16.0/requirements.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)       38 2023-07-03 22:28:20.549774 pymgpipe-0.16.0/setup.cfg
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1557 2023-07-03 22:28:00.000000 pymgpipe-0.16.0/setup.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.383738 pymgpipe-0.16.1/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.339908 pymgpipe-0.16.1/.github/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.343109 pymgpipe-0.16.1/.github/workflows/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1038 2023-04-27 18:57:29.000000 pymgpipe-0.16.1/.github/workflows/docs.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     3131 2023-07-03 22:51:29.000000 pymgpipe-0.16.1/.github/workflows/python-package.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1144 2023-04-27 19:33:13.000000 pymgpipe-0.16.1/.github/workflows/tests.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2059 2023-06-30 20:10:42.000000 pymgpipe-0.16.1/.gitignore
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    11389 2023-05-16 14:54:10.000000 pymgpipe-0.16.1/LICENSE
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-03 22:54:40.383470 pymgpipe-0.16.1/PKG-INFO
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    14257 2023-07-03 22:41:47.000000 pymgpipe-0.16.1/README.md
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.344541 pymgpipe-0.16.1/docs/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1162 2023-05-05 20:21:07.000000 pymgpipe-0.16.1/docs/conf.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      451 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/docs/index.rst
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/docs/modules.rst
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1212 2023-05-11 17:45:24.000000 pymgpipe-0.16.1/docs/pymgpipe.rst
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.345191 pymgpipe-0.16.1/examples/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-05-11 17:28:05.000000 pymgpipe-0.16.1/examples/test_diet.csv
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     8480 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/examples/workflow.ipynb
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.362163 pymgpipe-0.16.1/pymgpipe/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      149 2023-07-03 21:57:55.000000 pymgpipe-0.16.1/pymgpipe/__init__.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2206 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/coupling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    14625 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/diet.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     9847 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/fva.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     5283 2023-07-03 21:59:54.000000 pymgpipe-0.16.1/pymgpipe/io.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      341 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/logger.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    12371 2023-06-30 20:03:36.000000 pymgpipe-0.16.1/pymgpipe/main.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1254 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/metrics.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     8900 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/modeling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     6417 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/nmpc.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.340576 pymgpipe-0.16.1/pymgpipe/resources/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.364997 pymgpipe-0.16.1/pymgpipe/resources/diets/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2656 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/AverageEuropeanDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2681 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/DACHDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2616 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/GlutenFreeDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2639 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/HighFatLowCarbDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2669 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/HighFiberDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2685 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/HighProteinDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2675 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/MediterraneanDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2657 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/Type2DiabetesDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2655 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/UnhealthyDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2624 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/VeganDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2659 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/diets/VegetarianDiet.txt
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.366496 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaA.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaB.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaC.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaD.xml.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.377566 pymgpipe-0.16.1/pymgpipe/resources/models/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   319554 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.json
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   636272 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.mat
+-rw-r--r--   0 yolimeydan   (501) staff       (20)  1624449 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    75498 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.379632 pymgpipe-0.16.1/pymgpipe/resources/problems/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   113023 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    19492 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   185852 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    24457 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.383078 pymgpipe-0.16.1/pymgpipe/tests/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      592 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/conftest.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2092 2023-05-11 17:36:33.000000 pymgpipe-0.16.1/pymgpipe/tests/test_build.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1606 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_coupling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2550 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_diet.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     6096 2023-06-30 20:03:36.000000 pymgpipe-0.16.1/pymgpipe/tests/test_e2e.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1430 2023-04-27 19:31:46.000000 pymgpipe-0.16.1/pymgpipe/tests/test_fva.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1920 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_io.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      723 2023-04-27 18:09:14.000000 pymgpipe-0.16.1/pymgpipe/tests/test_utils.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    11375 2023-05-18 15:36:12.000000 pymgpipe-0.16.1/pymgpipe/utils.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-03 22:54:40.362912 pymgpipe-0.16.1/pymgpipe.egg-info/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/PKG-INFO
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1837 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)        1 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       46 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/requires.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)        9 2023-07-03 22:54:40.000000 pymgpipe-0.16.1/pymgpipe.egg-info/top_level.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      226 2023-06-30 20:03:34.000000 pymgpipe-0.16.1/requirements.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       38 2023-07-03 22:54:40.383783 pymgpipe-0.16.1/setup.cfg
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1589 2023-07-03 22:53:07.000000 pymgpipe-0.16.1/setup.py
```

### Comparing `pymgpipe-0.16.0/.github/workflows/docs.yml` & `pymgpipe-0.16.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/.github/workflows/python-package.yml` & `pymgpipe-0.16.1/.github/workflows/python-package.yml`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     - name: Update Readme with Coverage Html
       if: ${{ github.ref == 'refs/heads/main' }}
       run: |
         sed -i '/<!-- Pytest Coverage Comment:Begin -->/,/<!-- Pytest Coverage Comment:End -->/c\<!-- Pytest Coverage Comment:Begin -->\n\${{ steps.coverageComment.outputs.coverageHtml }}\n<!-- Pytest Coverage Comment:End -->' ./README.md
   release:
     needs: build
     if: ${{ github.ref == 'refs/heads/main' }}  && ${{ github.event.head_commit.message != 'Github Actions- Push'}}
+    name: Update version
     runs-on: ubuntu-latest
     env:
       GITHUB_TOKEN: ${{ secrets.RELEASE }}
     steps:
       - id: release
         uses: rymndhng/release-on-push-action@master
         with:
@@ -71,18 +72,18 @@
     runs-on: ubuntu-latest
     name: Push changes
     steps:
     - uses: actions/checkout@v3
       with:
         persist-credentials: false 
         fetch-depth: 0 
-    - name: Update version
+    - name: Write version to file
       uses: brettdorrans/write-version-to-file@master
       with:
-        filename: '.VERSION'
+        filename: 'pymgpipe/resources/.VERSION'
         placeholder: '${VERSION}'
     - name: Commit & Push changes to Readme
       if: ${{ github.ref == 'refs/heads/main' }} 
       uses: actions-js/push@master
       with:
         github_token: ${{ secrets.PUSH_README }}
         message: 'Github Actions- Push'
```

### Comparing `pymgpipe-0.16.0/.github/workflows/tests.yml` & `pymgpipe-0.16.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/.gitignore` & `pymgpipe-0.16.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/LICENSE` & `pymgpipe-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/PKG-INFO` & `pymgpipe-0.16.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 Metadata-Version: 2.1
 Name: pymgpipe
-Version: 0.16.0
+Version: 0.16.1
 Summary: Community level microbiome metabolic modeling in Python
 Home-page: https://github.com/korem-lab/pymgpipe
-Author: Yoli Meydan
-Author-email: ym2877@cumc.columbia.edu
+Author: Yoli Meydan, Federico Baldini, Tal Korem
+Author-email: ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0
 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/issues
 Project-URL: Source, https://github.com/korem-lab/pymgpipe
 Project-URL: Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## [pymgpipe](https://korem-lab.github.io/pymgpipe/) | [![DOI](https://zenodo.org/badge/525586335.svg)](https://zenodo.org/badge/latestdoi/525586335) [![status](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871/status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [![Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml)  
+## [pymgpipe](https://korem-lab.github.io/pymgpipe/) | [![DOI](https://zenodo.org/badge/525586335.svg)](https://zenodo.org/badge/latestdoi/525586335) [![status](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871/status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [![Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml) [![PyPI version](https://badge.fury.io/py/pymgpipe.svg)](https://badge.fury.io/py/pymgpipe)  
 <!-- Pytest Coverage Comment:Begin -->
 <a href="https://github.com/korem-lab/pymgpipe/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-77%25-yellow.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>pymgpipe</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py">coupling.py</a></td><td>39</td><td>6</td><td>85%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L20">20</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L43">43</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L46-L47">46&ndash;47</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L52">52</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L67">67</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py">diet.py</a></td><td>103</td><td>19</td><td>82%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L16">16</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L22">22</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L396-L397">396&ndash;397</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L437-L453">437&ndash;453</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L466-L477">466&ndash;477</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L482-L485">482&ndash;485</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L494">494</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L496">496</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L525">525</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py">fva.py</a></td><td>144</td><td>59</td><td>59%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L32">32</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L36">36</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L88-L92">88&ndash;92</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L98">98</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L107-L113">107&ndash;113</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L116-L117">116&ndash;117</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L120-L121">120&ndash;121</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L139-L149">139&ndash;149</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L165">165</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L174-L235">174&ndash;235</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L244">244</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py">io.py</a></td><td>106</td><td>37</td><td>65%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L17">17</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L55">55</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L61-L66">61&ndash;66</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L80-L81">80&ndash;81</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L95-L96">95&ndash;96</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L108">108</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L111">111</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L117-L120">117&ndash;120</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L125-L133">125&ndash;133</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L142">142</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L146-L147">146&ndash;147</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L152-L157">152&ndash;157</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L161-L167">161&ndash;167</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L176-L177">176&ndash;177</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py">main.py</a></td><td>148</td><td>44</td><td>70%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L112">112</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L115">115</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L167">167</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L210-L212">210&ndash;212</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L243-L297">243&ndash;297</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L304">304</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L309-L310">309&ndash;310</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L323">323</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/metrics.py">metrics.py</a></td><td>24</td><td>21</td><td>12%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/metrics.py#L5-L35">5&ndash;35</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py">modeling.py</a></td><td>145</td><td>7</td><td>95%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L36">36</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L39">39</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L54-L57">54&ndash;57</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L129">129</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L131">131</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py">nmpc.py</a></td><td>64</td><td>5</td><td>92%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L95">95</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L132-L134">132&ndash;134</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L136">136</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py">utils.py</a></td><td>235</td><td>107</td><td>54%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L45-L46">45&ndash;46</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L49">49</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L52">52</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L67">67</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L73">73</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L83">83</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L87">87</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L102-L105">102&ndash;105</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L111">111</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L115-L117">115&ndash;117</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L120-L138">120&ndash;138</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L142-L152">142&ndash;152</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L160">160</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L173-L174">173&ndash;174</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L176-L177">176&ndash;177</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L199-L200">199&ndash;200</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L205-L207">205&ndash;207</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L245-L248">245&ndash;248</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L250-L264">250&ndash;264</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L270">270</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L281-L286">281&ndash;286</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L289-L293">289&ndash;293</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L313-L314">313&ndash;314</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L325-L367">325&ndash;367</a></td></tr><tr><td colspan="5"><b>pymgpipe/tests</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/tests/test_e2e.py">test_e2e.py</a></td><td>90</td><td>1</td><td>99%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/tests/test_e2e.py#L197">197</a></td></tr><tr><td><b>TOTAL</b></td><td><b>1309</b></td><td><b>306</b></td><td><b>77%</b></td><td>&nbsp;</td></tr></tbody></table></details>
 <!-- Pytest Coverage Comment:End -->
 
 ### API Docs
 https://korem-lab.github.io/pymgpipe/
 
 ### Installation
-**pympgipe** has been built and tested with python 3.10+. To install and use this package, you can run through the following steps-
-1. Create a new `conda` environment using `conda create --name <env> python=3.10`
-2. Activate this environment using `conda activate <env>`
-3.  Install the required packages using `pip install -r requirements.txt`
-4.  Install **pympgipe** using `pip install 'pymgpipe @ git+https://github.com/korem-lab/pymgpipe'`
-
-You should now just be able to `import pymgpipe`. If you get a **ModuleNotFoundError**, make sure you're using the same python environment you used with `pip`.
+**pympgipe** has been built and tested with python 3.10+. To install and use our PyPi package, run `pip install pymgpipe`
 
 ### Additional Dependencies
 Need at least one of the following solvers (requirements.txt includes **gurobi**)-
 
 -  [cplex](<https://www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>)
 -  [gurobipy](<http://www.gurobi.com>)
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.0 Summary: Community level
+Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.1 Summary: Community level
 microbiome metabolic modeling in Python Home-page: https://github.com/korem-
-lab/pymgpipe Author: Yoli Meydan Author-email: ym2877@cumc.columbia.edu
+lab/pymgpipe Author: Yoli Meydan, Federico Baldini, Tal Korem Author-email:
+ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/
 issues Project-URL: Source, https://github.com/korem-lab/pymgpipe Project-URL:
 Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
@@ -15,16 +16,17 @@
 status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [!
 [Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/
 python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/
 pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/
 korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://
 github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://
 github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://
-github.com/korem-lab/pymgpipe/actions/workflows/docs.yml)  [Coverage]Coverage
-Report
+github.com/korem-lab/pymgpipe/actions/workflows/docs.yml) [![PyPI version]
+(https://badge.fury.io/py/pymgpipe.svg)](https://badge.fury.io/py/pymgpipe)
+[Coverage]Coverage Report
 File         Stmts Miss Cover Missing
 pymgpipe
             39    6    85%   20, 43, 46–47, 52, 67
  coupling.py
    diet.py 103   19   82%   16, 22, 396–397, 437–453, 466–477, 482–485, 494, 496, 525
    fva.py  144   59   59%   32, 36, 88–92, 98, 107–113, 116–117, 120–121, 139–149, 165, 174–235, 244
    io.py   106   37   65%   17, 55, 61–66, 80–81, 95–96, 108, 111, 117–120, 125–133, 142, 146–147, 152–157,
@@ -40,23 +42,17 @@
                               313–314, 325–367
 pymgpipe/tests
             90    1    99%   197
  test_e2e.py
 TOTAL        1309  306  77%    
  ### API Docs https://korem-lab.github.io/pymgpipe/ ### Installation
 **pympgipe** has been built and tested with python 3.10+. To install and use
-this package, you can run through the following steps- 1. Create a new `conda`
-environment using `conda create --name  python=3.10` 2. Activate this
-environment using `conda activate ` 3. Install the required packages using `pip
-install -r requirements.txt` 4. Install **pympgipe** using `pip install
-'pymgpipe @ git+https://github.com/korem-lab/pymgpipe'` You should now just be
-able to `import pymgpipe`. If you get a **ModuleNotFoundError**, make sure
-you're using the same python environment you used with `pip`. ### Additional
-Dependencies Need at least one of the following solvers (requirements.txt
-includes **gurobi**)- - [cplex](
+our PyPi package, run `pip install pymgpipe` ### Additional Dependencies Need
+at least one of the following solvers (requirements.txt includes **gurobi**)- -
+[cplex](
 www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>) - [gurobipy](
 www.gurobi.com>) In order to install the solver interfaces in python, you can
 use `pip install cplex` or `pip install gurobipy`. This does not actually
 create a license, it just installs the python interface to interact with these
 solvers. Both gurobipy and cplex offer free academic licenses. To install the
 licenses themselves, refer to the links provided above. ### Inputs To create
 multi-species community models with **pymgpipe**, you need two things to start-
```

### Comparing `pymgpipe-0.16.0/README.md` & `pymgpipe-0.16.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-## [pymgpipe](https://korem-lab.github.io/pymgpipe/) | [![DOI](https://zenodo.org/badge/525586335.svg)](https://zenodo.org/badge/latestdoi/525586335) [![status](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871/status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [![Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml)  
+## [pymgpipe](https://korem-lab.github.io/pymgpipe/) | [![DOI](https://zenodo.org/badge/525586335.svg)](https://zenodo.org/badge/latestdoi/525586335) [![status](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871/status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [![Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml) [![PyPI version](https://badge.fury.io/py/pymgpipe.svg)](https://badge.fury.io/py/pymgpipe)  
 <!-- Pytest Coverage Comment:Begin -->
 <a href="https://github.com/korem-lab/pymgpipe/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-77%25-yellow.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>pymgpipe</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py">coupling.py</a></td><td>39</td><td>6</td><td>85%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L20">20</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L43">43</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L46-L47">46&ndash;47</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L52">52</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L67">67</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py">diet.py</a></td><td>103</td><td>19</td><td>82%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L16">16</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L22">22</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L396-L397">396&ndash;397</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L437-L453">437&ndash;453</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L466-L477">466&ndash;477</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L482-L485">482&ndash;485</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L494">494</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L496">496</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L525">525</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py">fva.py</a></td><td>144</td><td>59</td><td>59%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L32">32</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L36">36</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L88-L92">88&ndash;92</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L98">98</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L107-L113">107&ndash;113</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L116-L117">116&ndash;117</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L120-L121">120&ndash;121</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L139-L149">139&ndash;149</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L165">165</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L174-L235">174&ndash;235</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L244">244</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py">io.py</a></td><td>106</td><td>37</td><td>65%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L17">17</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L55">55</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L61-L66">61&ndash;66</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L80-L81">80&ndash;81</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L95-L96">95&ndash;96</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L108">108</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L111">111</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L117-L120">117&ndash;120</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L125-L133">125&ndash;133</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L142">142</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L146-L147">146&ndash;147</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L152-L157">152&ndash;157</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L161-L167">161&ndash;167</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L176-L177">176&ndash;177</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py">main.py</a></td><td>148</td><td>44</td><td>70%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L112">112</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L115">115</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L167">167</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L210-L212">210&ndash;212</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L243-L297">243&ndash;297</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L304">304</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L309-L310">309&ndash;310</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L323">323</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/metrics.py">metrics.py</a></td><td>24</td><td>21</td><td>12%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/metrics.py#L5-L35">5&ndash;35</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py">modeling.py</a></td><td>145</td><td>7</td><td>95%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L36">36</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L39">39</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L54-L57">54&ndash;57</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L129">129</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L131">131</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py">nmpc.py</a></td><td>64</td><td>5</td><td>92%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L95">95</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L132-L134">132&ndash;134</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L136">136</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py">utils.py</a></td><td>235</td><td>107</td><td>54%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L45-L46">45&ndash;46</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L49">49</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L52">52</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L67">67</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L73">73</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L83">83</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L87">87</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L102-L105">102&ndash;105</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L111">111</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L115-L117">115&ndash;117</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L120-L138">120&ndash;138</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L142-L152">142&ndash;152</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L160">160</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L173-L174">173&ndash;174</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L176-L177">176&ndash;177</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L199-L200">199&ndash;200</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L205-L207">205&ndash;207</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L245-L248">245&ndash;248</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L250-L264">250&ndash;264</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L270">270</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L281-L286">281&ndash;286</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L289-L293">289&ndash;293</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L313-L314">313&ndash;314</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L325-L367">325&ndash;367</a></td></tr><tr><td colspan="5"><b>pymgpipe/tests</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/tests/test_e2e.py">test_e2e.py</a></td><td>90</td><td>1</td><td>99%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/tests/test_e2e.py#L197">197</a></td></tr><tr><td><b>TOTAL</b></td><td><b>1309</b></td><td><b>306</b></td><td><b>77%</b></td><td>&nbsp;</td></tr></tbody></table></details>
 <!-- Pytest Coverage Comment:End -->
 
 ### API Docs
 https://korem-lab.github.io/pymgpipe/
 
 ### Installation
-**pympgipe** has been built and tested with python 3.10+. To install and use this package, you can run through the following steps-
-1. Create a new `conda` environment using `conda create --name <env> python=3.10`
-2. Activate this environment using `conda activate <env>`
-3.  Install the required packages using `pip install -r requirements.txt`
-4.  Install **pympgipe** using `pip install 'pymgpipe @ git+https://github.com/korem-lab/pymgpipe'`
-
-You should now just be able to `import pymgpipe`. If you get a **ModuleNotFoundError**, make sure you're using the same python environment you used with `pip`.
+**pympgipe** has been built and tested with python 3.10+. To install and use our PyPi package, run `pip install pymgpipe`
 
 ### Additional Dependencies
 Need at least one of the following solvers (requirements.txt includes **gurobi**)-
 
 -  [cplex](<https://www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>)
 -  [gurobipy](<http://www.gurobi.com>)
```

#### html2text {}

```diff
@@ -4,16 +4,17 @@
 status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [!
 [Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/
 python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/
 pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/
 korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://
 github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://
 github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://
-github.com/korem-lab/pymgpipe/actions/workflows/docs.yml)  [Coverage]Coverage
-Report
+github.com/korem-lab/pymgpipe/actions/workflows/docs.yml) [![PyPI version]
+(https://badge.fury.io/py/pymgpipe.svg)](https://badge.fury.io/py/pymgpipe)
+[Coverage]Coverage Report
 File         Stmts Miss Cover Missing
 pymgpipe
             39    6    85%   20, 43, 46–47, 52, 67
  coupling.py
    diet.py 103   19   82%   16, 22, 396–397, 437–453, 466–477, 482–485, 494, 496, 525
    fva.py  144   59   59%   32, 36, 88–92, 98, 107–113, 116–117, 120–121, 139–149, 165, 174–235, 244
    io.py   106   37   65%   17, 55, 61–66, 80–81, 95–96, 108, 111, 117–120, 125–133, 142, 146–147, 152–157,
@@ -29,23 +30,17 @@
                               313–314, 325–367
 pymgpipe/tests
             90    1    99%   197
  test_e2e.py
 TOTAL        1309  306  77%    
  ### API Docs https://korem-lab.github.io/pymgpipe/ ### Installation
 **pympgipe** has been built and tested with python 3.10+. To install and use
-this package, you can run through the following steps- 1. Create a new `conda`
-environment using `conda create --name  python=3.10` 2. Activate this
-environment using `conda activate ` 3. Install the required packages using `pip
-install -r requirements.txt` 4. Install **pympgipe** using `pip install
-'pymgpipe @ git+https://github.com/korem-lab/pymgpipe'` You should now just be
-able to `import pymgpipe`. If you get a **ModuleNotFoundError**, make sure
-you're using the same python environment you used with `pip`. ### Additional
-Dependencies Need at least one of the following solvers (requirements.txt
-includes **gurobi**)- - [cplex](
+our PyPi package, run `pip install pymgpipe` ### Additional Dependencies Need
+at least one of the following solvers (requirements.txt includes **gurobi**)- -
+[cplex](
 www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>) - [gurobipy](
 www.gurobi.com>) In order to install the solver interfaces in python, you can
 use `pip install cplex` or `pip install gurobipy`. This does not actually
 create a license, it just installs the python interface to interact with these
 solvers. Both gurobipy and cplex offer free academic licenses. To install the
 licenses themselves, refer to the links provided above. ### Inputs To create
 multi-species community models with **pymgpipe**, you need two things to start-
```

### Comparing `pymgpipe-0.16.0/docs/conf.py` & `pymgpipe-0.16.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/docs/pymgpipe.rst` & `pymgpipe-0.16.1/docs/pymgpipe.rst`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/examples/workflow.ipynb` & `pymgpipe-0.16.1/examples/workflow.ipynb`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/coupling.py` & `pymgpipe-0.16.1/pymgpipe/coupling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/diet.py` & `pymgpipe-0.16.1/pymgpipe/diet.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/fva.py` & `pymgpipe-0.16.1/pymgpipe/fva.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/io.py` & `pymgpipe-0.16.1/pymgpipe/io.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/main.py` & `pymgpipe-0.16.1/pymgpipe/main.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/metrics.py` & `pymgpipe-0.16.1/pymgpipe/metrics.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/modeling.py` & `pymgpipe-0.16.1/pymgpipe/modeling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/nmpc.py` & `pymgpipe-0.16.1/pymgpipe/nmpc.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/AverageEuropeanDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/AverageEuropeanDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/DACHDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/DACHDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/GlutenFreeDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/GlutenFreeDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/HighFatLowCarbDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/HighFatLowCarbDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/HighFiberDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/HighFiberDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/HighProteinDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/HighProteinDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/MediterraneanDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/MediterraneanDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/Type2DiabetesDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/Type2DiabetesDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/UnhealthyDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/UnhealthyDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/VeganDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/VeganDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/diets/VegetarianDiet.txt` & `pymgpipe-0.16.1/pymgpipe/resources/diets/VegetarianDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaA.xml.gz` & `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaA.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaB.xml.gz` & `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaB.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaC.xml.gz` & `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaC.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/miniTaxa/TaxaD.xml.gz` & `pymgpipe-0.16.1/pymgpipe/resources/miniTaxa/TaxaD.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.json` & `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.json`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.mat` & `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.mat`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.xml` & `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/models/mini_model.xml.gz` & `pymgpipe-0.16.1/pymgpipe/resources/models/mini_model.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.lp` & `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.lp.gz` & `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.lp.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.mps` & `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/resources/problems/mini_model.mps.gz` & `pymgpipe-0.16.1/pymgpipe/resources/problems/mini_model.mps.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/conftest.py` & `pymgpipe-0.16.1/pymgpipe/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/test_build.py` & `pymgpipe-0.16.1/pymgpipe/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/test_coupling.py` & `pymgpipe-0.16.1/pymgpipe/tests/test_coupling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/test_diet.py` & `pymgpipe-0.16.1/pymgpipe/tests/test_diet.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/test_e2e.py` & `pymgpipe-0.16.1/pymgpipe/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/test_fva.py` & `pymgpipe-0.16.1/pymgpipe/tests/test_fva.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/test_io.py` & `pymgpipe-0.16.1/pymgpipe/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/tests/test_utils.py` & `pymgpipe-0.16.1/pymgpipe/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe/utils.py` & `pymgpipe-0.16.1/pymgpipe/utils.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.0/pymgpipe.egg-info/PKG-INFO` & `pymgpipe-0.16.1/pymgpipe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 Metadata-Version: 2.1
 Name: pymgpipe
-Version: 0.16.0
+Version: 0.16.1
 Summary: Community level microbiome metabolic modeling in Python
 Home-page: https://github.com/korem-lab/pymgpipe
-Author: Yoli Meydan
-Author-email: ym2877@cumc.columbia.edu
+Author: Yoli Meydan, Federico Baldini, Tal Korem
+Author-email: ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0
 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/issues
 Project-URL: Source, https://github.com/korem-lab/pymgpipe
 Project-URL: Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## [pymgpipe](https://korem-lab.github.io/pymgpipe/) | [![DOI](https://zenodo.org/badge/525586335.svg)](https://zenodo.org/badge/latestdoi/525586335) [![status](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871/status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [![Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml)  
+## [pymgpipe](https://korem-lab.github.io/pymgpipe/) | [![DOI](https://zenodo.org/badge/525586335.svg)](https://zenodo.org/badge/latestdoi/525586335) [![status](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871/status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [![Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://github.com/korem-lab/pymgpipe/actions/workflows/docs.yml) [![PyPI version](https://badge.fury.io/py/pymgpipe.svg)](https://badge.fury.io/py/pymgpipe)  
 <!-- Pytest Coverage Comment:Begin -->
 <a href="https://github.com/korem-lab/pymgpipe/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-77%25-yellow.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>pymgpipe</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py">coupling.py</a></td><td>39</td><td>6</td><td>85%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L20">20</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L43">43</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L46-L47">46&ndash;47</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L52">52</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/coupling.py#L67">67</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py">diet.py</a></td><td>103</td><td>19</td><td>82%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L16">16</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L22">22</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L396-L397">396&ndash;397</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L437-L453">437&ndash;453</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L466-L477">466&ndash;477</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L482-L485">482&ndash;485</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L494">494</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L496">496</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/diet.py#L525">525</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py">fva.py</a></td><td>144</td><td>59</td><td>59%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L32">32</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L36">36</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L88-L92">88&ndash;92</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L98">98</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L107-L113">107&ndash;113</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L116-L117">116&ndash;117</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L120-L121">120&ndash;121</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L139-L149">139&ndash;149</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L165">165</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L174-L235">174&ndash;235</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/fva.py#L244">244</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py">io.py</a></td><td>106</td><td>37</td><td>65%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L17">17</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L55">55</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L61-L66">61&ndash;66</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L80-L81">80&ndash;81</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L95-L96">95&ndash;96</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L108">108</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L111">111</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L117-L120">117&ndash;120</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L125-L133">125&ndash;133</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L142">142</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L146-L147">146&ndash;147</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L152-L157">152&ndash;157</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L161-L167">161&ndash;167</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/io.py#L176-L177">176&ndash;177</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py">main.py</a></td><td>148</td><td>44</td><td>70%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L112">112</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L115">115</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L167">167</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L210-L212">210&ndash;212</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L243-L297">243&ndash;297</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L304">304</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L309-L310">309&ndash;310</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/main.py#L323">323</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/metrics.py">metrics.py</a></td><td>24</td><td>21</td><td>12%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/metrics.py#L5-L35">5&ndash;35</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py">modeling.py</a></td><td>145</td><td>7</td><td>95%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L36">36</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L39">39</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L54-L57">54&ndash;57</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L129">129</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/modeling.py#L131">131</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py">nmpc.py</a></td><td>64</td><td>5</td><td>92%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L95">95</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L132-L134">132&ndash;134</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/nmpc.py#L136">136</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py">utils.py</a></td><td>235</td><td>107</td><td>54%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L45-L46">45&ndash;46</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L49">49</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L52">52</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L67">67</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L73">73</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L83">83</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L87">87</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L102-L105">102&ndash;105</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L111">111</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L115-L117">115&ndash;117</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L120-L138">120&ndash;138</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L142-L152">142&ndash;152</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L160">160</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L173-L174">173&ndash;174</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L176-L177">176&ndash;177</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L199-L200">199&ndash;200</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L205-L207">205&ndash;207</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L245-L248">245&ndash;248</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L250-L264">250&ndash;264</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L270">270</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L281-L286">281&ndash;286</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L289-L293">289&ndash;293</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L313-L314">313&ndash;314</a>, <a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/utils.py#L325-L367">325&ndash;367</a></td></tr><tr><td colspan="5"><b>pymgpipe/tests</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/tests/test_e2e.py">test_e2e.py</a></td><td>90</td><td>1</td><td>99%</td><td><a href="https://github.com/korem-lab/pymgpipe/blob/main/pymgpipe/tests/test_e2e.py#L197">197</a></td></tr><tr><td><b>TOTAL</b></td><td><b>1309</b></td><td><b>306</b></td><td><b>77%</b></td><td>&nbsp;</td></tr></tbody></table></details>
 <!-- Pytest Coverage Comment:End -->
 
 ### API Docs
 https://korem-lab.github.io/pymgpipe/
 
 ### Installation
-**pympgipe** has been built and tested with python 3.10+. To install and use this package, you can run through the following steps-
-1. Create a new `conda` environment using `conda create --name <env> python=3.10`
-2. Activate this environment using `conda activate <env>`
-3.  Install the required packages using `pip install -r requirements.txt`
-4.  Install **pympgipe** using `pip install 'pymgpipe @ git+https://github.com/korem-lab/pymgpipe'`
-
-You should now just be able to `import pymgpipe`. If you get a **ModuleNotFoundError**, make sure you're using the same python environment you used with `pip`.
+**pympgipe** has been built and tested with python 3.10+. To install and use our PyPi package, run `pip install pymgpipe`
 
 ### Additional Dependencies
 Need at least one of the following solvers (requirements.txt includes **gurobi**)-
 
 -  [cplex](<https://www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>)
 -  [gurobipy](<http://www.gurobi.com>)
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.0 Summary: Community level
+Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.1 Summary: Community level
 microbiome metabolic modeling in Python Home-page: https://github.com/korem-
-lab/pymgpipe Author: Yoli Meydan Author-email: ym2877@cumc.columbia.edu
+lab/pymgpipe Author: Yoli Meydan, Federico Baldini, Tal Korem Author-email:
+ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/
 issues Project-URL: Source, https://github.com/korem-lab/pymgpipe Project-URL:
 Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
@@ -15,16 +16,17 @@
 status.svg)](https://joss.theoj.org/papers/3f284f37987438428fd09ad3d5bd4871) [!
 [Python package](https://github.com/korem-lab/pymgpipe/actions/workflows/
 python-package.yml/badge.svg?branch=main)](https://github.com/korem-lab/
 pymgpipe/actions/workflows/python-package.yml) [![Tests](https://github.com/
 korem-lab/pymgpipe/actions/workflows/tests.yml/badge.svg?branch=main)](https://
 github.com/korem-lab/pymgpipe/actions/workflows/tests.yml) [![Docs](https://
 github.com/korem-lab/pymgpipe/actions/workflows/docs.yml/badge.svg)](https://
-github.com/korem-lab/pymgpipe/actions/workflows/docs.yml)  [Coverage]Coverage
-Report
+github.com/korem-lab/pymgpipe/actions/workflows/docs.yml) [![PyPI version]
+(https://badge.fury.io/py/pymgpipe.svg)](https://badge.fury.io/py/pymgpipe)
+[Coverage]Coverage Report
 File         Stmts Miss Cover Missing
 pymgpipe
             39    6    85%   20, 43, 46–47, 52, 67
  coupling.py
    diet.py 103   19   82%   16, 22, 396–397, 437–453, 466–477, 482–485, 494, 496, 525
    fva.py  144   59   59%   32, 36, 88–92, 98, 107–113, 116–117, 120–121, 139–149, 165, 174–235, 244
    io.py   106   37   65%   17, 55, 61–66, 80–81, 95–96, 108, 111, 117–120, 125–133, 142, 146–147, 152–157,
@@ -40,23 +42,17 @@
                               313–314, 325–367
 pymgpipe/tests
             90    1    99%   197
  test_e2e.py
 TOTAL        1309  306  77%    
  ### API Docs https://korem-lab.github.io/pymgpipe/ ### Installation
 **pympgipe** has been built and tested with python 3.10+. To install and use
-this package, you can run through the following steps- 1. Create a new `conda`
-environment using `conda create --name  python=3.10` 2. Activate this
-environment using `conda activate ` 3. Install the required packages using `pip
-install -r requirements.txt` 4. Install **pympgipe** using `pip install
-'pymgpipe @ git+https://github.com/korem-lab/pymgpipe'` You should now just be
-able to `import pymgpipe`. If you get a **ModuleNotFoundError**, make sure
-you're using the same python environment you used with `pip`. ### Additional
-Dependencies Need at least one of the following solvers (requirements.txt
-includes **gurobi**)- - [cplex](
+our PyPi package, run `pip install pymgpipe` ### Additional Dependencies Need
+at least one of the following solvers (requirements.txt includes **gurobi**)- -
+[cplex](
 www-01.ibm.com/software/commerce/optimization/cplex-optimizer/>) - [gurobipy](
 www.gurobi.com>) In order to install the solver interfaces in python, you can
 use `pip install cplex` or `pip install gurobipy`. This does not actually
 create a license, it just installs the python interface to interact with these
 solvers. Both gurobipy and cplex offer free academic licenses. To install the
 licenses themselves, refer to the links provided above. ### Inputs To create
 multi-species community models with **pymgpipe**, you need two things to start-
```

### Comparing `pymgpipe-0.16.0/pymgpipe.egg-info/SOURCES.txt` & `pymgpipe-0.16.1/pymgpipe.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 pymgpipe/nmpc.py
 pymgpipe/utils.py
 pymgpipe.egg-info/PKG-INFO
 pymgpipe.egg-info/SOURCES.txt
 pymgpipe.egg-info/dependency_links.txt
 pymgpipe.egg-info/requires.txt
 pymgpipe.egg-info/top_level.txt
-pymgpipe/resources/.VERSION
 pymgpipe/resources/diets/AverageEuropeanDiet.txt
 pymgpipe/resources/diets/DACHDiet.txt
 pymgpipe/resources/diets/GlutenFreeDiet.txt
 pymgpipe/resources/diets/HighFatLowCarbDiet.txt
 pymgpipe/resources/diets/HighFiberDiet.txt
 pymgpipe/resources/diets/HighProteinDiet.txt
 pymgpipe/resources/diets/MediterraneanDiet.txt
```

### Comparing `pymgpipe-0.16.0/setup.py` & `pymgpipe-0.16.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
-    author="Yoli Meydan",
-    author_email="ym2877@cumc.columbia.edu",
+    author="Yoli Meydan, Federico Baldini, Tal Korem",
+    author_email="ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu",
     name="pymgpipe",
     description="Community level microbiome metabolic modeling in Python",
-    version=open("pymgpipe/resources/.VERSION").readline().strip()[1:],
+    version="v0.16.1",
     classifiers=[
         "Intended Audience :: Healthcare Industry",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
```

