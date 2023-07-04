# Comparing `tmp/PDielec-7.1.2.tar.gz` & `tmp/PDielec-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDielec-7.1.2.tar", last modified: Sat Mar 26 09:58:14 2022, max compression
+gzip compressed data, was "PDielec-7.2.1.tar", last modified: Tue Jul  4 12:53:23 2023, max compression
```

## Comparing `PDielec-7.1.2.tar` & `PDielec-7.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-03-26 09:58:14.042193 PDielec-7.1.2/
--rw-rw-r--   0 john      (1000) john      (1000)     1080 2015-11-17 09:07:58.000000 PDielec-7.1.2/LICENSE.md
--rw-r--r--   0 john      (1000) john      (1000)     1080 2018-03-01 08:29:24.000000 PDielec-7.1.2/LICENSE.txt
--rw-r--r--   0 john      (1000) john      (1000)       17 2021-12-04 13:46:41.000000 PDielec-7.1.2/MANIFEST.in
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-03-26 09:58:14.038860 PDielec-7.1.2/PDielec/
--rw-r--r--   0 john      (1000) john      (1000)    10508 2021-11-18 17:01:07.000000 PDielec-7.1.2/PDielec/AbinitOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    71031 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/Calculator.py
--rw-r--r--   0 john      (1000) john      (1000)    15442 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/CastepOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    23360 2021-11-18 17:01:23.000000 PDielec-7.1.2/PDielec/Constants.py
--rw-r--r--   0 john      (1000) john      (1000)    14706 2022-03-25 15:49:33.000000 PDielec-7.1.2/PDielec/CrystalOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    14672 2022-03-25 14:01:39.000000 PDielec-7.1.2/PDielec/DielectricFunction.py
--rw-r--r--   0 john      (1000) john      (1000)    18000 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/ExperimentOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    44231 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/GTMcore.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-03-26 09:58:14.042193 PDielec-7.1.2/PDielec/GUI/
--rw-r--r--   0 john      (1000) john      (1000)    23910 2022-03-24 15:19:32.000000 PDielec-7.1.2/PDielec/GUI/AnalysisTab.py
--rw-r--r--   0 john      (1000) john      (1000)     9703 2022-03-24 15:12:52.000000 PDielec-7.1.2/PDielec/GUI/App.py
--rw-r--r--   0 john      (1000) john      (1000)    38940 2021-12-28 18:32:44.000000 PDielec-7.1.2/PDielec/GUI/FitterTab.py
--rw-r--r--   0 john      (1000) john      (1000)    27046 2022-03-24 14:59:26.000000 PDielec-7.1.2/PDielec/GUI/MainTab.py
--rw-r--r--   0 john      (1000) john      (1000)    21896 2022-02-02 17:08:22.000000 PDielec-7.1.2/PDielec/GUI/NoteBook.py
--rw-r--r--   0 john      (1000) john      (1000)    20745 2022-03-23 16:26:33.000000 PDielec-7.1.2/PDielec/GUI/OpenGLWidget.py
--rw-r--r--   0 john      (1000) john      (1000)    31711 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/GUI/PlottingTab.py
--rw-r--r--   0 john      (1000) john      (1000)    39204 2022-02-02 17:58:16.000000 PDielec-7.1.2/PDielec/GUI/PowderScenarioTab.py
--rw-r--r--   0 john      (1000) john      (1000)     4331 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/GUI/ScenarioTab.py
--rw-r--r--   0 john      (1000) john      (1000)    34276 2022-03-26 09:51:30.000000 PDielec-7.1.2/PDielec/GUI/SettingsTab.py
--rw-r--r--   0 john      (1000) john      (1000)    28557 2022-02-02 17:59:22.000000 PDielec-7.1.2/PDielec/GUI/SingleCrystalScenarioTab.py
--rw-r--r--   0 john      (1000) john      (1000)     2752 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/GUI/SpreadSheetManager.py
--rw-r--r--   0 john      (1000) john      (1000)    33329 2022-03-24 15:43:39.000000 PDielec-7.1.2/PDielec/GUI/ViewerTab.py
--rw-r--r--   0 john      (1000) john      (1000)       80 2022-03-26 09:58:13.000000 PDielec-7.1.2/PDielec/GUI/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    31376 2020-05-05 17:36:05.000000 PDielec-7.1.2/PDielec/GUI/splash.png
--rw-r--r--   0 john      (1000) john      (1000)    23965 2022-02-02 14:29:45.000000 PDielec-7.1.2/PDielec/GenericOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    15555 2021-11-18 17:01:42.000000 PDielec-7.1.2/PDielec/GulpOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)     1078 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/IO.py
--rw-r--r--   0 john      (1000) john      (1000)    20827 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/Mie.py
--rw-r--r--   0 john      (1000) john      (1000)     5676 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/PhonopyOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)     2395 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/Plotter.py
--rw-r--r--   0 john      (1000) john      (1000)    14124 2021-11-18 17:02:14.000000 PDielec-7.1.2/PDielec/QEOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)     7854 2022-03-23 14:21:38.000000 PDielec-7.1.2/PDielec/SuperCell.py
--rw-r--r--   0 john      (1000) john      (1000)    23459 2022-03-23 14:21:43.000000 PDielec-7.1.2/PDielec/UnitCell.py
--rw-r--r--   0 john      (1000) john      (1000)     9784 2022-03-24 15:05:17.000000 PDielec-7.1.2/PDielec/Utilities.py
--rw-r--r--   0 john      (1000) john      (1000)    15876 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/VaspOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)       80 2022-03-26 09:58:13.000000 PDielec-7.1.2/PDielec/__init__.py
--rwxr-xr-x   0 john      (1000) john      (1000)     7283 2022-01-21 11:41:10.000000 PDielec-7.1.2/PDielec/checkcsv.py
--rwxr-xr-x   0 john      (1000) john      (1000)     5880 2022-01-21 11:41:10.000000 PDielec-7.1.2/PDielec/checkexcel.py
--rwxr-xr-x   0 john      (1000) john      (1000)     5188 2021-11-18 17:01:37.000000 PDielec-7.1.2/PDielec/graphdatagenerator.py
--rwxr-xr-x   0 john      (1000) john      (1000)     3741 2021-12-04 12:53:52.000000 PDielec-7.1.2/PDielec/p1reader.py
--rwxr-xr-x   0 john      (1000) john      (1000)     4422 2022-01-21 11:41:10.000000 PDielec-7.1.2/PDielec/p2cif.py
--rwxr-xr-x   0 john      (1000) john      (1000)     6768 2021-11-18 17:01:58.000000 PDielec-7.1.2/PDielec/pdcompare.py
--rwxr-xr-x   0 john      (1000) john      (1000)     2711 2022-02-03 11:08:20.000000 PDielec-7.1.2/PDielec/pdgui.py
--rwxr-xr-x   0 john      (1000) john      (1000)    27650 2022-01-21 14:07:30.000000 PDielec-7.1.2/PDielec/pdmake.py
--rwxr-xr-x   0 john      (1000) john      (1000)     1689 2021-11-18 17:02:06.000000 PDielec-7.1.2/PDielec/pickled_reader.py
--rwxr-xr-x   0 john      (1000) john      (1000)    21219 2022-01-21 11:41:10.000000 PDielec-7.1.2/PDielec/preader.py
--rw-r--r--   0 john      (1000) john      (1000)     3751 2021-12-04 12:53:53.000000 PDielec-7.1.2/PDielec/test_gtm.py
--rw-r--r--   0 john      (1000) john      (1000)    12091 2021-12-04 12:53:53.000000 PDielec-7.1.2/PDielec/test_ttm.py
--rwxr-xr-x   0 john      (1000) john      (1000)    70967 2022-01-21 11:41:10.000000 PDielec-7.1.2/PDielec/vibanalysis.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2022-03-26 09:58:14.038860 PDielec-7.1.2/PDielec.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     4020 2022-03-26 09:58:14.000000 PDielec-7.1.2/PDielec.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1421 2022-03-26 09:58:14.000000 PDielec-7.1.2/PDielec.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2022-03-26 09:58:14.000000 PDielec-7.1.2/PDielec.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)      267 2022-03-26 09:58:14.000000 PDielec-7.1.2/PDielec.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) john      (1000)      167 2022-03-26 09:58:14.000000 PDielec-7.1.2/PDielec.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       20 2022-03-26 09:58:14.000000 PDielec-7.1.2/PDielec.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) john      (1000)     4020 2022-03-26 09:58:14.042193 PDielec-7.1.2/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     2994 2020-05-05 17:36:05.000000 PDielec-7.1.2/README.md
--rw-r--r--   0 john      (1000) john      (1000)       79 2022-03-26 09:58:14.042193 PDielec-7.1.2/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     2681 2022-03-26 09:45:27.000000 PDielec-7.1.2/setup.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.896868 PDielec-7.2.1/
+-rw-rw-r--   0 john      (1000) john      (1000)     1080 2015-11-17 09:07:58.000000 PDielec-7.2.1/LICENSE.md
+-rw-r--r--   0 john      (1000) john      (1000)     1080 2018-03-01 08:29:24.000000 PDielec-7.2.1/LICENSE.txt
+-rw-r--r--   0 john      (1000) john      (1000)       17 2021-12-04 13:46:41.000000 PDielec-7.2.1/MANIFEST.in
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.894868 PDielec-7.2.1/PDielec/
+-rw-r--r--   0 john      (1000) john      (1000)    10508 2021-11-18 17:01:07.000000 PDielec-7.2.1/PDielec/AbinitOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    71022 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/Calculator.py
+-rw-r--r--   0 john      (1000) john      (1000)    15442 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/CastepOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    23360 2021-11-18 17:01:23.000000 PDielec-7.2.1/PDielec/Constants.py
+-rw-r--r--   0 john      (1000) john      (1000)    14706 2022-03-25 15:49:33.000000 PDielec-7.2.1/PDielec/CrystalOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    14648 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/DielectricFunction.py
+-rw-r--r--   0 john      (1000) john      (1000)    17991 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/ExperimentOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    44231 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/GTMcore.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.896868 PDielec-7.2.1/PDielec/GUI/
+-rw-r--r--   0 john      (1000) john      (1000)    23910 2022-03-24 15:19:32.000000 PDielec-7.2.1/PDielec/GUI/AnalysisTab.py
+-rw-r--r--   0 john      (1000) john      (1000)     9875 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/App.py
+-rw-r--r--   0 john      (1000) john      (1000)    38940 2021-12-28 18:32:44.000000 PDielec-7.2.1/PDielec/GUI/FitterTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    27046 2022-03-24 14:59:26.000000 PDielec-7.2.1/PDielec/GUI/MainTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    21764 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/NoteBook.py
+-rw-r--r--   0 john      (1000) john      (1000)    20745 2023-07-03 18:31:52.000000 PDielec-7.2.1/PDielec/GUI/OpenGLWidget.py
+-rw-r--r--   0 john      (1000) john      (1000)    32111 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/PlottingTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    39204 2022-02-02 17:58:16.000000 PDielec-7.2.1/PDielec/GUI/PowderScenarioTab.py
+-rw-r--r--   0 john      (1000) john      (1000)     4331 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/GUI/ScenarioTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    34276 2022-03-26 09:51:30.000000 PDielec-7.2.1/PDielec/GUI/SettingsTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    25673 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/SingleCrystalScenarioTab.py
+-rw-r--r--   0 john      (1000) john      (1000)     2814 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/SpreadSheetManager.py
+-rw-r--r--   0 john      (1000) john      (1000)    33329 2022-03-24 15:43:39.000000 PDielec-7.2.1/PDielec/GUI/ViewerTab.py
+-rw-r--r--   0 john      (1000) john      (1000)       80 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec/GUI/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    31376 2020-05-05 17:36:05.000000 PDielec-7.2.1/PDielec/GUI/splash.png
+-rw-r--r--   0 john      (1000) john      (1000)    23965 2022-02-02 14:29:45.000000 PDielec-7.2.1/PDielec/GenericOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    15555 2021-11-18 17:01:42.000000 PDielec-7.2.1/PDielec/GulpOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)     1078 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/IO.py
+-rw-r--r--   0 john      (1000) john      (1000)    20827 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/Mie.py
+-rw-r--r--   0 john      (1000) john      (1000)     5676 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/PhonopyOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)     2395 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/Plotter.py
+-rw-r--r--   0 john      (1000) john      (1000)    14124 2021-11-18 17:02:14.000000 PDielec-7.2.1/PDielec/QEOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)     7854 2022-03-23 14:21:38.000000 PDielec-7.2.1/PDielec/SuperCell.py
+-rw-r--r--   0 john      (1000) john      (1000)    23459 2022-03-23 14:21:43.000000 PDielec-7.2.1/PDielec/UnitCell.py
+-rw-r--r--   0 john      (1000) john      (1000)     9784 2022-03-24 15:05:17.000000 PDielec-7.2.1/PDielec/Utilities.py
+-rw-r--r--   0 john      (1000) john      (1000)    15876 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/VaspOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)       80 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec/__init__.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     7283 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/checkcsv.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     5880 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/checkexcel.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     5188 2021-11-18 17:01:37.000000 PDielec-7.2.1/PDielec/graphdatagenerator.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     3741 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/p1reader.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     4422 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/p2cif.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     6768 2021-11-18 17:01:58.000000 PDielec-7.2.1/PDielec/pdcompare.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     2711 2022-02-03 11:08:20.000000 PDielec-7.2.1/PDielec/pdgui.py
+-rwxr-xr-x   0 john      (1000) john      (1000)    27840 2023-07-04 12:51:45.000000 PDielec-7.2.1/PDielec/pdmake.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     1689 2021-11-18 17:02:06.000000 PDielec-7.2.1/PDielec/pickled_reader.py
+-rwxr-xr-x   0 john      (1000) john      (1000)    21219 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/preader.py
+-rw-r--r--   0 john      (1000) john      (1000)     3751 2021-12-04 12:53:53.000000 PDielec-7.2.1/PDielec/test_gtm.py
+-rw-r--r--   0 john      (1000) john      (1000)    12091 2021-12-04 12:53:53.000000 PDielec-7.2.1/PDielec/test_ttm.py
+-rwxr-xr-x   0 john      (1000) john      (1000)    70967 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/vibanalysis.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.895868 PDielec-7.2.1/PDielec.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     4000 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1421 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)      266 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) john      (1000)      167 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       20 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) john      (1000)     4000 2023-07-04 12:53:23.896868 PDielec-7.2.1/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     2994 2020-05-05 17:36:05.000000 PDielec-7.2.1/README.md
+-rw-r--r--   0 john      (1000) john      (1000)       79 2023-07-04 12:53:23.896868 PDielec-7.2.1/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     2681 2023-07-04 08:30:08.000000 PDielec-7.2.1/setup.py
```

### Comparing `PDielec-7.1.2/LICENSE.md` & `PDielec-7.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/LICENSE.txt` & `PDielec-7.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/AbinitOutputReader.py` & `PDielec-7.2.1/PDielec/AbinitOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/Calculator.py` & `PDielec-7.2.1/PDielec/Calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,4364 +77,4363 @@
 000004c0: 6973 2061 206c 6973 7420 6f66 2033 2072  is a list of 3 r
 000004d0: 6561 6c20 6e75 6d62 6572 7320 666f 7220  eal numbers for 
 000004e0: 7468 6520 6469 6167 6f6e 616c 732c 2074  the diagonals, t
 000004f0: 6865 2072 6574 7572 6e65 6420 7465 6e73  he returned tens
 00000500: 6f72 2069 7320 616e 2061 7272 6179 2727  or is an array''
 00000510: 270a 2020 2020 7820 3d20 6e70 2e7a 6572  '.    x = np.zer
 00000520: 6f73 2828 332c 2033 292c 2064 7479 7065  os((3, 3), dtype
-00000530: 3d6e 702e 666c 6f61 7429 0a20 2020 2078  =np.float).    x
-00000540: 5b30 2c20 305d 203d 2031 2e30 0a20 2020  [0, 0] = 1.0.   
-00000550: 2078 5b31 2c20 315d 203d 2031 2e30 0a20   x[1, 1] = 1.0. 
-00000560: 2020 2078 5b32 2c20 325d 203d 2031 2e30     x[2, 2] = 1.0
-00000570: 0a20 2020 2072 6574 7572 6e20 780a 0a64  .    return x..d
-00000580: 6566 2069 6e69 7469 616c 6973 655f 636f  ef initialise_co
-00000590: 6d70 6c65 785f 6469 6167 6f6e 616c 5f74  mplex_diagonal_t
-000005a0: 656e 736f 7228 7265 616c 7329 3a0a 2020  ensor(reals):.  
-000005b0: 2020 2727 2749 6e69 7469 616c 6973 6520    '''Initialise 
-000005c0: 6120 3378 3320 7465 6e73 6f72 2c20 7468  a 3x3 tensor, th
-000005d0: 6520 6172 6775 6d65 6e74 2069 7320 6120  e argument is a 
-000005e0: 6c69 7374 206f 6620 3320 7265 616c 206e  list of 3 real n
-000005f0: 756d 6265 7273 2066 6f72 2074 6865 2064  umbers for the d
-00000600: 6961 676f 6e61 6c73 2c20 7468 6520 7265  iagonals, the re
-00000610: 7475 726e 6564 2074 656e 736f 7220 6973  turned tensor is
-00000620: 2061 6e20 6172 7261 7927 2727 0a20 2020   an array'''.   
-00000630: 2078 203d 206e 702e 7a65 726f 7328 2833   x = np.zeros((3
-00000640: 2c20 3329 2c20 6474 7970 653d 6e70 2e63  , 3), dtype=np.c
-00000650: 6f6d 706c 6578 290a 2020 2020 785b 302c  omplex).    x[0,
-00000660: 2030 5d20 3d20 7265 616c 735b 305d 0a20   0] = reals[0]. 
-00000670: 2020 2078 5b31 2c20 315d 203d 2072 6561     x[1, 1] = rea
-00000680: 6c73 5b31 5d0a 2020 2020 785b 322c 2032  ls[1].    x[2, 2
-00000690: 5d20 3d20 7265 616c 735b 325d 0a20 2020  ] = reals[2].   
-000006a0: 2072 6574 7572 6e20 780a 0a64 6566 2069   return x..def i
-000006b0: 6e69 7469 616c 6973 655f 6469 6167 6f6e  nitialise_diagon
-000006c0: 616c 5f74 656e 736f 7228 7265 616c 7329  al_tensor(reals)
-000006d0: 3a0a 2020 2020 2727 2749 6e69 7469 616c  :.    '''Initial
-000006e0: 6973 6520 6120 3378 3320 7465 6e73 6f72  ise a 3x3 tensor
-000006f0: 2c20 7468 6520 6172 6775 6d65 6e74 2069  , the argument i
-00000700: 7320 6120 6c69 7374 206f 6620 3320 7265  s a list of 3 re
-00000710: 616c 206e 756d 6265 7273 2066 6f72 2074  al numbers for t
-00000720: 6865 2064 6961 676f 6e61 6c73 2c20 7468  he diagonals, th
-00000730: 6520 7265 7475 726e 6564 2074 656e 736f  e returned tenso
-00000740: 7220 6973 2061 6e20 6172 7261 7927 2727  r is an array'''
-00000750: 0a20 2020 2078 203d 206e 702e 7a65 726f  .    x = np.zero
-00000760: 7328 2833 2c20 3329 2c20 6474 7970 653d  s((3, 3), dtype=
-00000770: 6e70 2e66 6c6f 6174 290a 2020 2020 785b  np.float).    x[
-00000780: 302c 2030 5d20 3d20 7265 616c 735b 305d  0, 0] = reals[0]
-00000790: 0a20 2020 2078 5b31 2c20 315d 203d 2072  .    x[1, 1] = r
-000007a0: 6561 6c73 5b31 5d0a 2020 2020 785b 322c  eals[1].    x[2,
-000007b0: 2032 5d20 3d20 7265 616c 735b 325d 0a20   2] = reals[2]. 
-000007c0: 2020 2072 6574 7572 6e20 780a 0a64 6566     return x..def
-000007d0: 2063 616c 6375 6c61 7465 5f64 6973 7461   calculate_dista
-000007e0: 6e63 6528 612c 6229 3a0a 2020 2020 2727  nce(a,b):.    ''
-000007f0: 2743 616c 6375 6c61 7465 2074 6865 2064  'Calculate the d
-00000800: 6973 7461 6e63 6520 6265 7477 6565 6e20  istance between 
-00000810: 6120 616e 6420 6227 2727 0a20 2020 2064  a and b'''.    d
-00000820: 203d 2030 2e30 0a20 2020 2066 6f72 2063   = 0.0.    for c
-00000830: 312c 2063 3220 696e 207a 6970 2861 2c62  1, c2 in zip(a,b
-00000840: 293a 0a20 2020 2020 2020 2064 202b 3d20  ):.        d += 
-00000850: 2863 3220 2d20 6331 292a 2863 3220 2d20  (c2 - c1)*(c2 - 
-00000860: 6331 290a 2020 2020 7265 7475 726e 206d  c1).    return m
-00000870: 6174 682e 7371 7274 2864 290a 0a64 6566  ath.sqrt(d)..def
-00000880: 2069 6e69 7469 616c 6973 655f 7261 6e64   initialise_rand
-00000890: 6f6d 5f74 656e 736f 7228 7363 616c 6529  om_tensor(scale)
-000008a0: 3a0a 2020 2020 2727 2749 6e69 7469 616c  :.    '''Initial
-000008b0: 6973 6520 6120 3378 3320 636f 6d70 6c65  ise a 3x3 comple
-000008c0: 7820 7465 6e73 6f72 2c20 7468 6520 6172  x tensor, the ar
-000008d0: 6775 6d65 6e74 2067 6976 6573 2074 6865  gument gives the
-000008e0: 206d 6178 696d 756d 2061 6273 6f6c 7574   maximum absolut
-000008f0: 6520 7661 6c75 6527 2727 0a20 2020 2070  e value'''.    p
-00000900: 7269 6e74 2822 4572 726f 7220 696e 6974  rint("Error init
-00000910: 6961 6c69 7365 5f72 616e 646f 6d5f 7465  ialise_random_te
-00000920: 6e73 6f72 206e 6f74 2077 6f72 6b69 6e67  nsor not working
-00000930: 222c 2066 696c 653d 7379 732e 7374 6465  ", file=sys.stde
-00000940: 7272 290a 2020 2020 6578 6974 2831 290a  rr).    exit(1).
-00000950: 2020 2020 7265 7475 726e 0a0a 6465 6620      return..def 
-00000960: 696e 6974 6961 6c69 7365 5f73 7068 6572  initialise_spher
-00000970: 655f 6465 706f 6c61 7269 7361 7469 6f6e  e_depolarisation
-00000980: 5f6d 6174 7269 7828 293a 0a20 2020 2027  _matrix():.    '
-00000990: 2727 496e 6974 6961 6c69 7365 2061 2033  ''Initialise a 3
-000009a0: 7833 2074 656e 736f 7220 7769 7468 2074  x3 tensor with t
-000009b0: 6865 2073 7068 6572 6520 6465 706f 6c61  he sphere depola
-000009c0: 7269 7361 7469 6f6e 206d 6174 7269 782c  risation matrix,
-000009d0: 2072 6574 7572 6e73 2061 2074 656e 736f   returns a tenso
-000009e0: 7227 2727 0a20 2020 2061 7468 6972 6420  r'''.    athird 
-000009f0: 3d20 312e 3020 2f20 332e 300a 2020 2020  = 1.0 / 3.0.    
-00000a00: 7465 6e73 6f72 203d 2069 6e69 7469 616c  tensor = initial
-00000a10: 6973 655f 6469 6167 6f6e 616c 5f74 656e  ise_diagonal_ten
-00000a20: 736f 7228 5b61 7468 6972 642c 2061 7468  sor([athird, ath
-00000a30: 6972 642c 2061 7468 6972 645d 290a 2020  ird, athird]).  
-00000a40: 2020 7465 6e73 6f72 203d 2074 656e 736f    tensor = tenso
-00000a50: 7220 2f20 6e70 2e74 7261 6365 2874 656e  r / np.trace(ten
-00000a60: 736f 7229 0a20 2020 2072 6574 7572 6e20  sor).    return 
-00000a70: 7465 6e73 6f72 0a0a 6465 6620 696e 6974  tensor..def init
-00000a80: 6961 6c69 7365 5f70 6c61 7465 5f64 6570  ialise_plate_dep
-00000a90: 6f6c 6172 6973 6174 696f 6e5f 6d61 7472  olarisation_matr
-00000aa0: 6978 286e 6f72 6d61 6c29 3a0a 2020 2020  ix(normal):.    
-00000ab0: 2727 2749 6e69 7469 616c 6973 6520 6120  '''Initialise a 
-00000ac0: 3378 3320 7465 6e73 6f72 2077 6974 6820  3x3 tensor with 
-00000ad0: 7468 6520 706c 6174 6520 6465 706f 6c61  the plate depola
-00000ae0: 7269 7361 7469 6f6e 206d 6174 7269 782c  risation matrix,
-00000af0: 2072 6574 7572 6e73 2061 2074 656e 736f   returns a tenso
-00000b00: 7227 2727 0a20 2020 206e 6f72 6d61 6c20  r'''.    normal 
-00000b10: 3d20 6e6f 726d 616c 202f 206e 702e 6c69  = normal / np.li
-00000b20: 6e61 6c67 2e6e 6f72 6d28 6e6f 726d 616c  nalg.norm(normal
-00000b30: 290a 2020 2020 7465 6e73 6f72 203d 206e  ).    tensor = n
-00000b40: 702e 6f75 7465 7228 6e6f 726d 616c 2c20  p.outer(normal, 
-00000b50: 6e6f 726d 616c 290a 2020 2020 7465 6e73  normal).    tens
-00000b60: 6f72 203d 2074 656e 736f 7220 2f20 6e70  or = tensor / np
-00000b70: 2e74 7261 6365 2874 656e 736f 7229 0a20  .trace(tensor). 
-00000b80: 2020 2072 6574 7572 6e20 7465 6e73 6f72     return tensor
-00000b90: 0a0a 6465 6620 696e 6974 6961 6c69 7365  ..def initialise
-00000ba0: 5f6e 6565 646c 655f 6465 706f 6c61 7269  _needle_depolari
-00000bb0: 7361 7469 6f6e 5f6d 6174 7269 7828 756e  sation_matrix(un
-00000bc0: 6971 7565 293a 0a20 2020 2027 2727 496e  ique):.    '''In
-00000bd0: 6974 6961 6c69 7365 2061 2033 7833 2074  itialise a 3x3 t
-00000be0: 656e 736f 7220 7769 7468 2074 6865 206e  ensor with the n
-00000bf0: 6565 646c 6520 6465 706f 6c61 7269 7361  eedle depolarisa
-00000c00: 7469 6f6e 206d 6174 7269 7827 2727 0a20  tion matrix'''. 
-00000c10: 2020 2023 2075 6e69 7175 6520 6973 2074     # unique is t
-00000c20: 6865 2075 6e69 7175 6520 6469 7265 6374  he unique direct
-00000c30: 696f 6e20 6f66 2074 6865 206e 6565 646c  ion of the needl
-00000c40: 650a 2020 2020 2320 6465 706f 6c61 7269  e.    # depolari
-00000c50: 7361 7469 6f6e 206d 6174 7269 7820 6973  sation matrix is
-00000c60: 2074 6865 7265 666f 7265 2068 616c 6620   therefore half 
-00000c70: 7468 6520 7375 6d20 6f66 2074 6865 0a20  the sum of the. 
-00000c80: 2020 2023 2074 776f 206f 7574 6572 2070     # two outer p
-00000c90: 726f 6475 6374 7320 6f66 2074 6865 2064  roducts of the d
-00000ca0: 6972 6563 7469 6f6e 7320 7065 7270 656e  irections perpen
-00000cb0: 6469 6375 6c61 7220 746f 2069 740a 2020  dicular to it.  
-00000cc0: 2020 756e 6971 7565 203d 2075 6e69 7175    unique = uniqu
-00000cd0: 6520 2f20 6e70 2e6c 696e 616c 672e 6e6f  e / np.linalg.no
-00000ce0: 726d 2875 6e69 7175 6529 0a20 2020 2078  rm(unique).    x
-00000cf0: 203d 206e 702e 6172 7261 7928 5b31 2c20   = np.array([1, 
-00000d00: 302c 2030 5d29 0a20 2020 2079 203d 206e  0, 0]).    y = n
-00000d10: 702e 6172 7261 7928 5b30 2c20 312c 2030  p.array([0, 1, 0
-00000d20: 5d29 0a20 2020 207a 203d 206e 702e 6172  ]).    z = np.ar
-00000d30: 7261 7928 5b30 2c20 302c 2031 5d29 0a20  ray([0, 0, 1]). 
-00000d40: 2020 2078 646f 746e 203d 206e 702e 646f     xdotn = np.do
-00000d50: 7428 782c 2075 6e69 7175 6529 0a20 2020  t(x, unique).   
-00000d60: 2079 646f 746e 203d 206e 702e 646f 7428   ydotn = np.dot(
-00000d70: 792c 2075 6e69 7175 6529 0a20 2020 207a  y, unique).    z
-00000d80: 646f 746e 203d 206e 702e 646f 7428 7a2c  dotn = np.dot(z,
-00000d90: 2075 6e69 7175 6529 0a20 2020 2061 6273   unique).    abs
-00000da0: 7864 6f74 6e20 3d20 6e70 2e61 6273 2878  xdotn = np.abs(x
-00000db0: 646f 746e 290a 2020 2020 6162 7379 646f  dotn).    absydo
-00000dc0: 746e 203d 206e 702e 6162 7328 7964 6f74  tn = np.abs(ydot
-00000dd0: 6e29 0a20 2020 2061 6273 7a64 6f74 6e20  n).    abszdotn 
-00000de0: 3d20 6e70 2e61 6273 287a 646f 746e 290a  = np.abs(zdotn).
-00000df0: 2020 2020 2320 6368 6f6f 7365 2074 6865      # choose the
-00000e00: 2064 6972 6563 7469 6f6e 2077 6974 6820   direction with 
-00000e10: 7468 6520 736d 616c 6c65 7374 2070 726f  the smallest pro
-00000e20: 6a65 6374 696f 6e20 616c 6f6e 6720 7468  jection along th
-00000e30: 6520 6e65 6564 6c65 0a20 2020 2023 2074  e needle.    # t
-00000e40: 6865 6e20 7072 6f6a 6563 7420 6f75 7420  hen project out 
-00000e50: 616e 7920 6e65 6564 6c65 2064 6972 6563  any needle direc
-00000e60: 7469 6f6e 0a20 2020 2069 6620 6162 7378  tion.    if absx
-00000e70: 646f 746e 203c 3d20 6162 7379 646f 746e  dotn <= absydotn
-00000e80: 2061 6e64 2061 6273 7864 6f74 6e20 3c3d   and absxdotn <=
-00000e90: 2061 6273 7a64 6f74 6e3a 0a20 2020 2020   abszdotn:.     
-00000ea0: 2020 2064 6972 3120 3d20 7820 2d20 2878     dir1 = x - (x
-00000eb0: 646f 746e 202a 2075 6e69 7175 6529 0a20  dotn * unique). 
-00000ec0: 2020 2065 6c69 6620 6162 7379 646f 746e     elif absydotn
-00000ed0: 203c 3d20 6162 7378 646f 746e 2061 6e64   <= absxdotn and
-00000ee0: 2061 6273 7964 6f74 6e20 3c3d 2061 6273   absydotn <= abs
-00000ef0: 7a64 6f74 6e3a 0a20 2020 2020 2020 2064  zdotn:.        d
-00000f00: 6972 3120 3d20 7920 2d20 2879 646f 746e  ir1 = y - (ydotn
-00000f10: 202a 2075 6e69 7175 6529 0a20 2020 2065   * unique).    e
-00000f20: 6c73 653a 0a20 2020 2020 2020 2064 6972  lse:.        dir
-00000f30: 3120 3d20 7a20 2d20 287a 646f 746e 202a  1 = z - (zdotn *
-00000f40: 2075 6e69 7175 6529 0a20 2020 2064 6972   unique).    dir
-00000f50: 3120 3d20 6469 7231 2f6e 702e 6c69 6e61  1 = dir1/np.lina
-00000f60: 6c67 2e6e 6f72 6d28 6469 7231 290a 2020  lg.norm(dir1).  
-00000f70: 2020 2320 6e6f 7720 6669 6e64 2074 6865    # now find the
-00000f80: 206f 7274 686f 676f 6e61 6c20 6469 7265   orthogonal dire
-00000f90: 6374 696f 6e0a 2020 2020 6469 7232 203d  ction.    dir2 =
-00000fa0: 206e 702e 6372 6f73 7328 756e 6971 7565   np.cross(unique
-00000fb0: 2c20 6469 7231 290a 2020 2020 6469 7232  , dir1).    dir2
-00000fc0: 203d 2064 6972 322f 6e70 2e6c 696e 616c   = dir2/np.linal
-00000fd0: 672e 6e6f 726d 2864 6972 3229 0a20 2020  g.norm(dir2).   
-00000fe0: 2023 2063 6f6d 7075 7465 2074 6865 2063   # compute the c
-00000ff0: 6f6d 706c 6578 2074 656e 736f 7273 2066  omplex tensors f
-00001000: 726f 6d20 7468 6520 6f75 7465 7220 7072  rom the outer pr
-00001010: 6f64 7563 7420 6f66 2065 6163 6820 6469  oduct of each di
-00001020: 7265 6374 696f 6e0a 2020 2020 7465 6e73  rection.    tens
-00001030: 6f72 203d 206e 702e 6f75 7465 7228 6469  or = np.outer(di
-00001040: 7231 2c20 6469 7231 2920 2b20 6e70 2e6f  r1, dir1) + np.o
-00001050: 7574 6572 2864 6972 322c 2064 6972 3229  uter(dir2, dir2)
-00001060: 0a20 2020 2074 656e 736f 7220 3d20 7465  .    tensor = te
-00001070: 6e73 6f72 202f 206e 702e 7472 6163 6528  nsor / np.trace(
-00001080: 7465 6e73 6f72 290a 2020 2020 7265 7475  tensor).    retu
-00001090: 726e 2074 656e 736f 720a 0a64 6566 2069  rn tensor..def i
-000010a0: 6e69 7469 616c 6973 655f 656c 6c69 7073  nitialise_ellips
-000010b0: 6f69 645f 6465 706f 6c61 7269 7361 7469  oid_depolarisati
-000010c0: 6f6e 5f6d 6174 7269 7828 756e 6971 7565  on_matrix(unique
-000010d0: 2c20 616f 7665 7262 293a 0a20 2020 2027  , aoverb):.    '
-000010e0: 2727 496e 6974 6961 6c69 7365 2061 2033  ''Initialise a 3
-000010f0: 7833 2074 656e 736f 7220 7769 7468 2074  x3 tensor with t
-00001100: 6865 2065 6c6c 6970 736f 6964 2064 6570  he ellipsoid dep
-00001110: 6f6c 6172 6973 6174 696f 6e20 6d61 7472  olarisation matr
-00001120: 6978 2727 270a 2020 2020 2320 756e 6971  ix'''.    # uniq
-00001130: 7565 2069 7320 7468 6520 756e 6971 7565  ue is the unique
-00001140: 2064 6972 6563 7469 6f6e 206f 6620 7468   direction of th
-00001150: 6520 656c 6c69 7073 6f69 640a 2020 2020  e ellipsoid.    
-00001160: 2320 6120 616e 6420 6220 6172 6520 7468  # a and b are th
-00001170: 6520 7369 7a65 7320 6f66 2074 6865 2065  e sizes of the e
-00001180: 6c6c 6970 736f 6964 2061 6c6f 6e67 2074  llipsoid along t
-00001190: 6865 2075 6e69 7175 6520 6178 6973 2028  he unique axis (
-000011a0: 6129 2061 6e64 2070 6572 7065 6e64 6963  a) and perpendic
-000011b0: 756c 6172 2074 6f20 6974 2062 0a20 2020  ular to it b.   
-000011c0: 2023 2069 6620 6120 3e20 6220 7468 656e   # if a > b then
-000011d0: 2077 6520 6861 7665 2061 2070 726f 6c61   we have a prola
-000011e0: 7465 2065 6c6c 6970 736f 6964 0a20 2020  te ellipsoid.   
-000011f0: 2075 6e69 7175 6520 3d20 756e 6971 7565   unique = unique
-00001200: 202f 206e 702e 6c69 6e61 6c67 2e6e 6f72   / np.linalg.nor
-00001210: 6d28 756e 6971 7565 290a 2020 2020 7820  m(unique).    x 
-00001220: 3d20 6e70 2e61 7272 6179 285b 312c 2030  = np.array([1, 0
-00001230: 2c20 305d 290a 2020 2020 7920 3d20 6e70  , 0]).    y = np
-00001240: 2e61 7272 6179 285b 302c 2031 2c20 305d  .array([0, 1, 0]
-00001250: 290a 2020 2020 7a20 3d20 6e70 2e61 7272  ).    z = np.arr
-00001260: 6179 285b 302c 2030 2c20 315d 290a 2020  ay([0, 0, 1]).  
-00001270: 2020 7864 6f74 6e20 3d20 6e70 2e64 6f74    xdotn = np.dot
-00001280: 2878 2c20 756e 6971 7565 290a 2020 2020  (x, unique).    
-00001290: 7964 6f74 6e20 3d20 6e70 2e64 6f74 2879  ydotn = np.dot(y
-000012a0: 2c20 756e 6971 7565 290a 2020 2020 7a64  , unique).    zd
-000012b0: 6f74 6e20 3d20 6e70 2e64 6f74 287a 2c20  otn = np.dot(z, 
-000012c0: 756e 6971 7565 290a 2020 2020 6162 7378  unique).    absx
-000012d0: 646f 746e 203d 206e 702e 6162 7328 7864  dotn = np.abs(xd
-000012e0: 6f74 6e29 0a20 2020 2061 6273 7964 6f74  otn).    absydot
-000012f0: 6e20 3d20 6e70 2e61 6273 2879 646f 746e  n = np.abs(ydotn
-00001300: 290a 2020 2020 6162 737a 646f 746e 203d  ).    abszdotn =
-00001310: 206e 702e 6162 7328 7a64 6f74 6e29 0a20   np.abs(zdotn). 
-00001320: 2020 2023 2063 686f 6f73 6520 7468 6520     # choose the 
-00001330: 6469 7265 6374 696f 6e20 7769 7468 2074  direction with t
-00001340: 6865 2073 6d61 6c6c 6573 7420 7072 6f6a  he smallest proj
-00001350: 6563 7469 6f6e 2061 6c6f 6e67 2074 6865  ection along the
-00001360: 2065 6c6c 6970 736f 6964 0a20 2020 2023   ellipsoid.    #
-00001370: 2074 6865 6e20 7072 6f6a 6563 7420 6f75   then project ou
-00001380: 7420 616e 7920 656c 6c69 7073 6f69 6420  t any ellipsoid 
-00001390: 6469 7265 6374 696f 6e0a 2020 2020 6966  direction.    if
-000013a0: 2061 6273 7864 6f74 6e20 3c3d 2061 6273   absxdotn <= abs
-000013b0: 7964 6f74 6e20 616e 6420 6162 7378 646f  ydotn and absxdo
-000013c0: 746e 203c 3d20 6162 737a 646f 746e 3a0a  tn <= abszdotn:.
-000013d0: 2020 2020 2020 2020 6469 7231 203d 2078          dir1 = x
-000013e0: 202d 2028 7864 6f74 6e20 2a20 756e 6971   - (xdotn * uniq
-000013f0: 7565 290a 2020 2020 656c 6966 2061 6273  ue).    elif abs
-00001400: 7964 6f74 6e20 3c3d 2061 6273 7864 6f74  ydotn <= absxdot
-00001410: 6e20 616e 6420 6162 7379 646f 746e 203c  n and absydotn <
-00001420: 3d20 6162 737a 646f 746e 3a0a 2020 2020  = abszdotn:.    
-00001430: 2020 2020 6469 7231 203d 2079 202d 2028      dir1 = y - (
-00001440: 7964 6f74 6e20 2a20 756e 6971 7565 290a  ydotn * unique).
-00001450: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001460: 2020 6469 7231 203d 207a 202d 2028 7a64    dir1 = z - (zd
-00001470: 6f74 6e20 2a20 756e 6971 7565 290a 2020  otn * unique).  
-00001480: 2020 6469 7231 203d 2064 6972 312f 6e70    dir1 = dir1/np
-00001490: 2e6c 696e 616c 672e 6e6f 726d 2864 6972  .linalg.norm(dir
-000014a0: 3129 0a20 2020 2023 206e 6f77 2066 696e  1).    # now fin
-000014b0: 6420 7468 6520 6f72 7468 6f67 6f6e 616c  d the orthogonal
-000014c0: 2064 6972 6563 7469 6f6e 0a20 2020 2064   direction.    d
-000014d0: 6972 3220 3d20 6e70 2e63 726f 7373 2875  ir2 = np.cross(u
-000014e0: 6e69 7175 652c 2064 6972 3129 0a20 2020  nique, dir1).   
-000014f0: 2064 6972 3220 3d20 6469 7232 2f6e 702e   dir2 = dir2/np.
-00001500: 6c69 6e61 6c67 2e6e 6f72 6d28 6469 7232  linalg.norm(dir2
-00001510: 290a 2020 2020 626f 7665 7261 203d 2031  ).    bovera = 1
-00001520: 2e30 202f 2061 6f76 6572 620a 2020 2020  .0 / aoverb.    
-00001530: 736d 616c 6c20 3d20 312e 3045 2d38 0a20  small = 1.0E-8. 
-00001540: 2020 2069 6620 626f 7665 7261 203c 2031     if bovera < 1
-00001550: 2e30 2d73 6d61 6c6c 3a0a 2020 2020 2020  .0-small:.      
-00001560: 2020 6520 3d20 6d61 7468 2e73 7172 7428    e = math.sqrt(
-00001570: 312e 3020 202d 2062 6f76 6572 612a 626f  1.0  - bovera*bo
-00001580: 7665 7261 290a 2020 2020 2020 2020 6e7a  vera).        nz
-00001590: 203d 2028 3120 2d20 652a 6529 202a 2028   = (1 - e*e) * (
-000015a0: 6e70 2e6c 6f67 2828 2831 2b65 2920 2f20  np.log(((1+e) / 
-000015b0: 2831 2d65 2929 2920 2d20 322a 6529 202f  (1-e))) - 2*e) /
-000015c0: 2028 322a 652a 652a 6529 0a20 2020 2065   (2*e*e*e).    e
-000015d0: 6c69 6620 626f 7665 7261 203e 2031 2e30  lif bovera > 1.0
-000015e0: 2b73 6d61 6c6c 3a0a 2020 2020 2020 2020  +small:.        
-000015f0: 6520 3d20 6d61 7468 2e73 7172 7428 626f  e = math.sqrt(bo
-00001600: 7665 7261 2a62 6f76 6572 6120 2d20 312e  vera*bovera - 1.
-00001610: 3029 0a20 2020 2020 2020 206e 7a20 3d20  0).        nz = 
-00001620: 2831 202b 2065 2a65 2920 2a20 2865 202d  (1 + e*e) * (e -
-00001630: 206e 702e 6172 6374 616e 2865 2929 202f   np.arctan(e)) /
-00001640: 2028 652a 652a 6529 0a20 2020 2065 6c73   (e*e*e).    els
-00001650: 653a 0a20 2020 2020 2020 206e 7a20 3d20  e:.        nz = 
-00001660: 312e 302f 332e 300a 2020 2020 6e78 7920  1.0/3.0.    nxy 
-00001670: 3d20 2831 202d 206e 7a29 202a 2030 2e35  = (1 - nz) * 0.5
-00001680: 0a20 2020 2023 0a20 2020 2023 2063 6f6d  .    #.    # com
-00001690: 7075 7465 2074 6865 2074 656e 736f 7273  pute the tensors
-000016a0: 2066 726f 6d20 7468 6520 6f75 7465 7220   from the outer 
-000016b0: 7072 6f64 7563 7420 6f66 2065 6163 6820  product of each 
-000016c0: 6469 7265 6374 696f 6e0a 2020 2020 7465  direction.    te
-000016d0: 6e73 6f72 203d 206e 7a2a 6e70 2e6f 7574  nsor = nz*np.out
-000016e0: 6572 2875 6e69 7175 652c 2075 6e69 7175  er(unique, uniqu
-000016f0: 6529 202b 206e 7879 2a6e 702e 6f75 7465  e) + nxy*np.oute
-00001700: 7228 6469 7231 2c20 6469 7231 2920 2b20  r(dir1, dir1) + 
-00001710: 6e78 792a 6e70 2e6f 7574 6572 2864 6972  nxy*np.outer(dir
-00001720: 322c 2064 6972 3229 0a20 2020 2074 656e  2, dir2).    ten
-00001730: 736f 7220 3d20 7465 6e73 6f72 202f 206e  sor = tensor / n
-00001740: 702e 7472 6163 6528 7465 6e73 6f72 290a  p.trace(tensor).
-00001750: 2020 2020 7265 7475 726e 2074 656e 736f      return tenso
-00001760: 720a 0a64 6566 2066 6962 6f6e 6163 6369  r..def fibonacci
-00001770: 5f73 7068 6572 6528 7361 6d70 6c65 733d  _sphere(samples=
-00001780: 312c 7261 6e64 6f6d 697a 653d 5472 7565  1,randomize=True
-00001790: 293a 0a20 2020 2072 6e64 203d 2031 2e0a  ):.    rnd = 1..
-000017a0: 2020 2020 6966 2072 616e 646f 6d69 7a65      if randomize
-000017b0: 3a0a 2020 2020 2020 2020 726e 6420 3d20  :.        rnd = 
-000017c0: 7261 6e64 6f6d 2e72 616e 646f 6d28 2920  random.random() 
-000017d0: 2a20 7361 6d70 6c65 730a 0a20 2020 2070  * samples..    p
-000017e0: 6f69 6e74 7320 3d20 5b5d 0a20 2020 206f  oints = [].    o
-000017f0: 6666 7365 7420 3d20 322e 2f73 616d 706c  ffset = 2./sampl
-00001800: 6573 0a20 2020 2069 6e63 7265 6d65 6e74  es.    increment
-00001810: 203d 206d 6174 682e 7069 202a 2028 332e   = math.pi * (3.
-00001820: 202d 206d 6174 682e 7371 7274 2835 2e29   - math.sqrt(5.)
-00001830: 293b 0a0a 2020 2020 666f 7220 6920 696e  );..    for i in
-00001840: 2072 616e 6765 2873 616d 706c 6573 293a   range(samples):
-00001850: 0a20 2020 2020 2020 2079 203d 2028 2869  .        y = ((i
-00001860: 202a 206f 6666 7365 7429 202d 2031 2920   * offset) - 1) 
-00001870: 2b20 286f 6666 7365 7420 2f20 3229 3b0a  + (offset / 2);.
-00001880: 2020 2020 2020 2020 7220 3d20 6d61 7468          r = math
-00001890: 2e73 7172 7428 3120 2d20 706f 7728 792c  .sqrt(1 - pow(y,
-000018a0: 3229 290a 0a20 2020 2020 2020 2070 6869  2))..        phi
-000018b0: 203d 2028 2869 202b 2072 6e64 2920 2520   = ((i + rnd) % 
-000018c0: 7361 6d70 6c65 7329 202a 2069 6e63 7265  samples) * incre
-000018d0: 6d65 6e74 0a0a 2020 2020 2020 2020 7820  ment..        x 
-000018e0: 3d20 6d61 7468 2e63 6f73 2870 6869 2920  = math.cos(phi) 
-000018f0: 2a20 720a 2020 2020 2020 2020 7a20 3d20  * r.        z = 
-00001900: 6d61 7468 2e73 696e 2870 6869 2920 2a20  math.sin(phi) * 
-00001910: 720a 0a20 2020 2020 2020 2070 6f69 6e74  r..        point
-00001920: 732e 6170 7065 6e64 285b 782c 792c 7a5d  s.append([x,y,z]
-00001930: 290a 0a20 2020 2072 6574 7572 6e20 706f  )..    return po
-00001940: 696e 7473 0a0a 6465 6620 696f 6e69 635f  ints..def ionic_
-00001950: 7065 726d 6974 7469 7669 7479 286d 6f64  permittivity(mod
-00001960: 655f 6c69 7374 2c20 6f73 6369 6c6c 6174  e_list, oscillat
-00001970: 6f72 5f73 7472 656e 6774 6873 2c20 6672  or_strengths, fr
-00001980: 6571 7565 6e63 6965 732c 2076 6f6c 756d  equencies, volum
-00001990: 6529 3a0a 2020 2020 2222 2243 616c 6375  e):.    """Calcu
-000019a0: 6c61 7465 2074 6865 206c 6f77 2066 7265  late the low fre
-000019b0: 7175 656e 6379 2070 6572 6d69 7474 6976  quency permittiv
-000019c0: 6974 7920 6f72 207a 6572 6f20 6672 6571  ity or zero freq
-000019d0: 7565 6e63 7920 7065 726d 6974 7469 7669  uency permittivi
-000019e0: 7479 0a20 2020 2020 2020 6f73 6369 6c6c  ty.       oscill
-000019f0: 6174 6f72 5f73 7472 656e 6774 6873 2061  ator_strengths a
-00001a00: 7265 2069 6e20 6174 6f6d 6963 2075 6e69  re in atomic uni
-00001a10: 7473 0a20 2020 2020 2020 6672 6571 7565  ts.       freque
-00001a20: 6e63 6965 7320 6172 6520 696e 2061 746f  ncies are in ato
-00001a30: 6d69 6320 756e 6974 730a 2020 2020 2020  mic units.      
-00001a40: 2076 6f6c 756d 6520 6973 2069 6e20 6174   volume is in at
-00001a50: 6f6d 6963 2075 6e69 7473 2222 220a 2020  omic units""".  
-00001a60: 2020 7065 726d 6974 7469 7669 7479 203d    permittivity =
-00001a70: 206e 702e 7a65 726f 7328 2833 2c20 3329   np.zeros((3, 3)
-00001a80: 290a 2020 2020 666f 7220 696d 6f64 6520  ).    for imode 
-00001a90: 696e 206d 6f64 655f 6c69 7374 3a0a 2020  in mode_list:.  
-00001aa0: 2020 2020 2020 7065 726d 6974 7469 7669        permittivi
-00001ab0: 7479 203d 2070 6572 6d69 7474 6976 6974  ty = permittivit
-00001ac0: 7920 2b20 6f73 6369 6c6c 6174 6f72 5f73  y + oscillator_s
-00001ad0: 7472 656e 6774 6873 5b69 6d6f 6465 5d20  trengths[imode] 
-00001ae0: 2f20 2866 7265 7175 656e 6369 6573 5b69  / (frequencies[i
-00001af0: 6d6f 6465 5d20 2a20 6672 6571 7565 6e63  mode] * frequenc
-00001b00: 6965 735b 696d 6f64 655d 290a 2020 2020  ies[imode]).    
-00001b10: 2320 656e 6420 666f 720a 2020 2020 7265  # end for.    re
-00001b20: 7475 726e 2070 6572 6d69 7474 6976 6974  turn permittivit
-00001b30: 7920 2a20 2834 202a 2050 4920 2f20 766f  y * (4 * PI / vo
-00001b40: 6c75 6d65 290a 0a64 6566 2069 6e66 7261  lume)..def infra
-00001b50: 7265 645f 696e 7465 6e73 6974 6965 7328  red_intensities(
-00001b60: 6f73 6369 6c6c 6174 6f72 5f73 7472 656e  oscillator_stren
-00001b70: 6774 6873 293a 0a20 2020 2022 2222 4361  gths):.    """Ca
-00001b80: 6c63 756c 6174 6520 7468 6520 4952 2069  lculate the IR i
-00001b90: 6e74 656e 7369 7469 6573 2066 726f 6d20  ntensities from 
-00001ba0: 7468 6520 7472 6163 6520 6f66 2074 6865  the trace of the
-00001bb0: 206f 7363 696c 6c61 746f 7220 7374 7265   oscillator stre
-00001bc0: 6e67 7468 732c 0a20 2020 2020 2020 5468  ngths,.       Th
-00001bd0: 6520 696e 7465 6e73 6974 6965 7320 6172  e intensities ar
-00001be0: 6520 7265 7475 726e 6564 2069 6e20 756e  e returned in un
-00001bf0: 6974 7320 6f66 2028 442f 4129 5e32 2f61  its of (D/A)^2/a
-00001c00: 6d75 2222 220a 2020 2020 2320 4561 6368  mu""".    # Each
-00001c10: 206d 6f64 6520 6861 7320 6120 3378 3320   mode has a 3x3 
-00001c20: 6f73 6369 6c6c 6174 6f72 2073 7472 656e  oscillator stren
-00001c30: 6774 680a 2020 2020 6e6d 6f64 6573 203d  gth.    nmodes =
-00001c40: 206e 702e 7369 7a65 286f 7363 696c 6c61   np.size(oscilla
-00001c50: 746f 725f 7374 7265 6e67 7468 732c 2030  tor_strengths, 0
-00001c60: 290a 2020 2020 696e 7465 6e73 6974 6965  ).    intensitie
-00001c70: 7320 3d20 6e70 2e7a 6572 6f73 286e 6d6f  s = np.zeros(nmo
-00001c80: 6465 7329 0a20 2020 2066 6f72 2069 6d6f  des).    for imo
-00001c90: 6465 2c20 7374 7265 6e67 7468 2069 6e20  de, strength in 
-00001ca0: 656e 756d 6572 6174 6528 6f73 6369 6c6c  enumerate(oscill
-00001cb0: 6174 6f72 5f73 7472 656e 6774 6873 293a  ator_strengths):
-00001cc0: 0a20 2020 2020 2020 2023 2057 6520 6361  .        # We ca
-00001cd0: 6c63 756c 6174 6520 7468 6520 696e 7465  lculate the inte
-00001ce0: 6e73 6974 7920 6672 6f6d 2074 6865 2074  nsity from the t
-00001cf0: 7261 6365 206f 6620 7468 6520 7374 7265  race of the stre
-00001d00: 6e67 7468 730a 2020 2020 2020 2020 696e  ngths.        in
-00001d10: 7465 6e73 6974 6965 735b 696d 6f64 655d  tensities[imode]
-00001d20: 203d 2069 6e74 656e 7369 7469 6573 5b69   = intensities[i
-00001d30: 6d6f 6465 5d20 2b20 7374 7265 6e67 7468  mode] + strength
-00001d40: 5b30 2c20 305d 202b 2073 7472 656e 6774  [0, 0] + strengt
-00001d50: 685b 312c 2031 5d20 2b20 7374 7265 6e67  h[1, 1] + streng
-00001d60: 7468 5b32 2c20 325d 0a20 2020 2023 2065  th[2, 2].    # e
-00001d70: 6e64 2066 6f72 0a20 2020 206d 6178 696e  nd for.    maxin
-00001d80: 7465 6e73 6974 7920 3d20 6e70 2e6d 6178  tensity = np.max
-00001d90: 2869 6e74 656e 7369 7469 6573 290a 2020  (intensities).  
-00001da0: 2020 636f 6e76 6572 7420 3d20 6d61 7869    convert = maxi
-00001db0: 6e74 656e 7369 7479 0a20 2020 2023 2063  ntensity.    # c
-00001dc0: 6f6e 7665 7274 2074 6865 2069 6e74 656e  onvert the inten
-00001dd0: 7369 7469 6573 2074 6f20 4361 7374 6570  sities to Castep
-00001de0: 2075 6e69 7473 2028 442f 4129 2a2a 322f   units (D/A)**2/
-00001df0: 616d 750a 2020 2020 636f 6e76 6572 7420  amu.    convert 
-00001e00: 3d20 6432 6279 616d 7561 6e67 320a 2020  = d2byamuang2.  
-00001e10: 2020 696e 7465 6e73 6974 6965 7320 3d20    intensities = 
-00001e20: 696e 7465 6e73 6974 6965 7320 2f20 636f  intensities / co
-00001e30: 6e76 6572 740a 2020 2020 7265 7475 726e  nvert.    return
-00001e40: 2069 6e74 656e 7369 7469 6573 0a0a 6465   intensities..de
-00001e50: 6620 6c6f 6e67 6974 7564 696e 616c 5f6d  f longitudinal_m
-00001e60: 6f64 6573 2866 7265 7175 656e 6369 6573  odes(frequencies
-00001e70: 2c20 6e6f 726d 616c 5f6d 6f64 6573 2c20  , normal_modes, 
-00001e80: 626f 726e 5f63 6861 7267 6573 2c20 6d61  born_charges, ma
-00001e90: 7373 6573 2c20 6570 7369 6c6f 6e5f 696e  sses, epsilon_in
-00001ea0: 662c 2076 6f6c 756d 652c 2071 6c69 7374  f, volume, qlist
-00001eb0: 2c20 7265 6164 6572 293a 0a20 2020 2022  , reader):.    "
-00001ec0: 2222 4170 706c 7920 7468 6520 6e6f 6e61  ""Apply the nona
-00001ed0: 6e61 6c79 7469 6320 636f 7272 6563 7469  nalytic correcti
-00001ee0: 6f6e 2074 6f20 7468 6520 6479 6e61 6d69  on to the dynami
-00001ef0: 6361 6c20 6d61 7472 6978 2061 6e64 2063  cal matrix and c
-00001f00: 616c 6375 6c61 7465 2074 6865 204c 4f20  alculate the LO 
-00001f10: 6672 6571 7565 6e63 6965 730a 2020 2020  frequencies.    
-00001f20: 2020 2066 7265 7175 656e 6369 6573 2061     frequencies a
-00001f30: 7265 2074 6865 2066 7265 7175 656e 6369  re the frequenci
-00001f40: 6573 2028 6629 2069 6e20 6174 6f6d 6963  es (f) in atomic
-00001f50: 2075 6e69 7473 0a20 2020 2020 2020 6e6f   units.       no
-00001f60: 726d 616c 5f6d 6f64 6573 2061 7265 2074  rmal_modes are t
-00001f70: 6865 206d 6173 7320 7765 6967 6874 6564  he mass weighted
-00001f80: 206e 6f72 6d61 6c20 6d6f 6465 7320 2855   normal modes (U
-00001f90: 290a 2020 2020 2020 2062 6f72 6e5f 6368  ).       born_ch
-00001fa0: 6172 6765 7320 6172 6520 7468 6520 626f  arges are the bo
-00001fb0: 726e 2063 6861 7267 6573 2028 5a29 2073  rn charges (Z) s
-00001fc0: 746f 7265 6420 6173 0a20 2020 2020 2020  tored as.       
-00001fd0: 2020 205b 5a31 7820 5a31 7920 5a31 7a5d     [Z1x Z1y Z1z]
-00001fe0: 205b 5a32 7820 5a32 7920 5a32 7a5d 205b   [Z2x Z2y Z2z] [
-00001ff0: 5a33 7820 5a33 7920 5a33 7a5d 5d0a 2020  Z3x Z3y Z3z]].  
-00002000: 2020 2020 2020 2020 7768 6572 6520 312c          where 1,
-00002010: 2032 2c20 3320 6172 6520 7468 6520 6469   2, 3 are the di
-00002020: 7265 6374 696f 6e73 206f 6620 7468 6520  rections of the 
-00002030: 6669 656c 6420 616e 6420 782c 2079 2c20  field and x, y, 
-00002040: 7a20 6172 6520 7468 6520 636f 6f72 6469  z are the coordi
-00002050: 6e61 7465 7320 6f66 2074 6865 2061 746f  nates of the ato
-00002060: 6d0a 2020 2020 2020 2071 6c69 7374 2069  m.       qlist i
-00002070: 7320 6120 6c69 7374 206f 6620 6469 7265  s a list of dire
-00002080: 6374 696f 6e20 7665 6374 6f72 730a 2020  ction vectors.  
-00002090: 2020 2020 2054 6865 2073 7562 726f 7574       The subrout
-000020a0: 696e 6520 7265 7475 726e 7320 6120 6c69  ine returns a li
-000020b0: 7374 206f 6620 2872 6561 6c29 2066 7265  st of (real) fre
-000020c0: 7175 656e 6369 6573 2069 6e20 6174 6f6d  quencies in atom
-000020d0: 6963 2075 6e69 7473 0a20 2020 2020 2020  ic units.       
-000020e0: 416e 7920 696d 6167 696e 6172 7920 6672  Any imaginary fr
-000020f0: 6571 7565 6e63 6965 7320 6172 6520 7365  equencies are se
-00002100: 7420 746f 2030 0a20 2020 2020 2020 4966  t to 0.       If
-00002110: 2070 726f 6a65 6374 696f 6e20 7761 7320   projection was 
-00002120: 7265 7175 6573 7465 6420 696e 2074 6865  requested in the
-00002130: 2072 6561 6465 722c 2074 6865 2063 6f72   reader, the cor
-00002140: 7265 6374 696f 6e20 6973 206d 6f64 6966  rection is modif
-00002150: 6965 6420 656e 7375 7265 2074 7261 6e73  ied ensure trans
-00002160: 6c61 7469 6f6e 616c 2069 6e76 6172 6961  lational invaria
-00002170: 6e63 6522 2222 0a20 2020 2023 2055 7365  nce""".    # Use
-00002180: 2061 2073 7172 7420 7468 6174 2072 6574   a sqrt that ret
-00002190: 7572 6e73 2061 2063 6f6d 706c 6578 206e  urns a complex n
-000021a0: 756d 6265 720a 2020 2020 2320 6672 6f6d  umber.    # from
-000021b0: 206e 756d 7079 2e6c 6962 2e73 6369 6d61   numpy.lib.scima
-000021c0: 7468 2069 6d70 6f72 7420 7371 7274 0a20  th import sqrt. 
-000021d0: 2020 2023 2046 6972 7374 2073 7465 7020     # First step 
-000021e0: 6973 2074 6f20 7265 636f 6e73 7472 7563  is to reconstruc
-000021f0: 7420 7468 6520 6479 6e61 6d69 6361 6c20  t the dynamical 
-00002200: 6d61 7472 6978 2028 4429 2066 726f 6d20  matrix (D) from 
-00002210: 7468 6520 6672 6571 7565 6e63 6965 7320  the frequencies 
-00002220: 616e 6420 7468 6520 6569 6765 6e76 6563  and the eigenvec
-00002230: 746f 7273 0a20 2020 2023 2066 5e32 203d  tors.    # f^2 =
-00002240: 2055 5420 2e20 4420 2e20 550a 2020 2020   UT . D . U.    
-00002250: 2320 616e 6420 5520 6973 2061 2068 6572  # and U is a her
-00002260: 6d69 7469 616e 206d 6174 7269 7820 736f  mitian matrix so
-00002270: 2055 2d31 203d 2055 540a 2020 2020 2320   U-1 = UT.    # 
-00002280: 4420 3d20 2855 5429 2d31 2066 5e32 2055  D = (UT)-1 f^2 U
-00002290: 2d31 203d 2055 2066 2055 540a 2020 2020  -1 = U f UT.    
-000022a0: 2320 436f 6e73 7472 7563 7420 5554 2066  # Construct UT f
-000022b0: 726f 6d20 7468 6520 6e6f 726d 616c 206d  rom the normal m
-000022c0: 6f64 6573 0a20 2020 206e 203d 206e 702e  odes.    n = np.
-000022d0: 7369 7a65 286e 6f72 6d61 6c5f 6d6f 6465  size(normal_mode
-000022e0: 732c 2030 290a 2020 2020 6d20 3d20 6e70  s, 0).    m = np
-000022f0: 2e73 697a 6528 6e6f 726d 616c 5f6d 6f64  .size(normal_mod
-00002300: 6573 2c20 3129 2a33 0a20 2020 2055 5420  es, 1)*3.    UT 
-00002310: 3d20 6e70 2e7a 6572 6f73 2828 6e2c 206d  = np.zeros((n, m
-00002320: 2929 0a20 2020 2066 6f72 2069 6d6f 6465  )).    for imode
-00002330: 2c20 6d6f 6465 2069 6e20 656e 756d 6572  , mode in enumer
-00002340: 6174 6528 6e6f 726d 616c 5f6d 6f64 6573  ate(normal_modes
-00002350: 293a 0a20 2020 2020 2020 206e 203d 2030  ):.        n = 0
-00002360: 0a20 2020 2020 2020 2066 6f72 2061 746f  .        for ato
-00002370: 6d20 696e 206d 6f64 653a 0a20 2020 2020  m in mode:.     
-00002380: 2020 2020 2020 2023 2069 6e20 7079 7468         # in pyth
-00002390: 6f6e 2074 6865 2066 6972 7374 2069 6e64  on the first ind
-000023a0: 6578 2069 7320 7468 6520 726f 7720 6f66  ex is the row of
-000023b0: 2074 6865 206d 6174 7269 782c 2074 6865   the matrix, the
-000023c0: 2073 6563 6f6e 6420 6973 2074 6865 2063   second is the c
-000023d0: 6f6c 756d 6e0a 2020 2020 2020 2020 2020  olumn.          
-000023e0: 2020 5554 5b69 6d6f 6465 2c20 6e2b 305d    UT[imode, n+0]
-000023f0: 203d 2061 746f 6d5b 305d 0a20 2020 2020   = atom[0].     
-00002400: 2020 2020 2020 2055 545b 696d 6f64 652c         UT[imode,
-00002410: 206e 2b31 5d20 3d20 6174 6f6d 5b31 5d0a   n+1] = atom[1].
-00002420: 2020 2020 2020 2020 2020 2020 5554 5b69              UT[i
-00002430: 6d6f 6465 2c20 6e2b 325d 203d 2061 746f  mode, n+2] = ato
-00002440: 6d5b 325d 0a20 2020 2020 2020 2020 2020  m[2].           
-00002450: 206e 203d 206e 202b 2033 0a20 2020 2020   n = n + 3.     
-00002460: 2020 2023 2065 6e64 2066 6f72 2061 746f     # end for ato
-00002470: 6d0a 2020 2020 2320 656e 6420 666f 7220  m.    # end for 
-00002480: 696d 6f64 650a 2020 2020 2320 7a65 726f  imode.    # zero
-00002490: 2074 6865 206e 6f6e 616e 616c 7974 6963   the nonanalytic
-000024a0: 616c 2063 6f72 7265 6374 696f 6e0a 2020  al correction.  
-000024b0: 2020 576d 203d 206e 702e 7a65 726f 7328    Wm = np.zeros(
-000024c0: 286e 2c20 6e29 290a 2020 2020 2320 636f  (n, n)).    # co
-000024d0: 6e76 6572 7420 7468 6520 6672 6571 7565  nvert the freque
-000024e0: 6e63 6965 735e 3220 746f 2061 2072 6561  ncies^2 to a rea
-000024f0: 6c20 6469 6167 6f6e 616c 2061 7272 6179  l diagonal array
-00002500: 0a20 2020 2023 2057 6172 6e69 6e67 2077  .    # Warning w
-00002510: 6520 6861 7665 2074 6f20 6d61 6b65 2073  e have to make s
-00002520: 7572 6520 7468 6520 7369 676e 2069 7320  ure the sign is 
-00002530: 636f 7272 6563 7420 6865 7265 0a20 2020  correct here.   
-00002540: 2066 3220 3d20 6e70 2e64 6961 6728 6e70   f2 = np.diag(np
-00002550: 2e73 6967 6e28 6672 6571 7565 6e63 6965  .sign(frequencie
-00002560: 7329 2a6e 702e 7265 616c 2866 7265 7175  s)*np.real(frequ
-00002570: 656e 6369 6573 2a66 7265 7175 656e 6369  encies*frequenci
-00002580: 6573 2929 0a20 2020 2044 6d20 3d20 6e70  es)).    Dm = np
-00002590: 2e64 6f74 286e 702e 646f 7428 5554 2e54  .dot(np.dot(UT.T
-000025a0: 2c20 6632 292c 2055 5429 0a20 2020 2023  , f2), UT).    #
-000025b0: 204d 616b 6520 7375 7265 2074 6865 2064   Make sure the d
-000025c0: 796e 616d 6963 616c 206d 6174 7269 7820  ynamical matrix 
-000025d0: 6973 2072 6561 6c0a 2020 2020 446d 203d  is real.    Dm =
-000025e0: 206e 702e 7265 616c 2844 6d29 0a20 2020   np.real(Dm).   
-000025f0: 2023 2046 696e 6420 6974 7320 6569 6765   # Find its eige
-00002600: 6e76 616c 7565 730a 2020 2020 6569 675f  nvalues.    eig_
-00002610: 7661 6c2c 2065 6967 5f76 6563 203d 206e  val, eig_vec = n
-00002620: 702e 6c69 6e61 6c67 2e65 6967 6828 446d  p.linalg.eigh(Dm
-00002630: 290a 2020 2020 2320 5374 6f72 6520 7468  ).    # Store th
-00002640: 6520 7265 7375 6c74 7320 666f 7220 7265  e results for re
-00002650: 7475 726e 696e 6720 746f 2074 6865 206d  turning to the m
-00002660: 6169 6e20 7072 6f67 7261 6d0a 2020 2020  ain program.    
-00002670: 7265 7375 6c74 7320 3d20 5b5d 0a20 2020  results = [].   
-00002680: 2023 204c 6f6f 7020 6f76 6572 2071 2076   # Loop over q v
-00002690: 616c 7565 730a 2020 2020 666f 7220 7120  alues.    for q 
-000026a0: 696e 2071 6c69 7374 3a0a 2020 2020 2020  in qlist:.      
-000026b0: 2020 2320 4e6f 7720 6361 6c63 756c 6174    # Now calculat
-000026c0: 6520 7468 6520 6e6f 6e61 6e61 6c79 7469  e the nonanalyti
-000026d0: 6320 7061 7274 0a20 2020 2020 2020 2063  c part.        c
-000026e0: 6f6e 7374 616e 7420 3d20 342e 3020 2a20  onstant = 4.0 * 
-000026f0: 5049 202f 2028 6e70 2e64 6f74 286e 702e  PI / (np.dot(np.
-00002700: 646f 7428 712c 2065 7073 696c 6f6e 5f69  dot(q, epsilon_i
-00002710: 6e66 292c 2071 2920 2a20 766f 6c75 6d65  nf), q) * volume
-00002720: 290a 2020 2020 2020 2020 2320 4c6f 6f70  ).        # Loop
-00002730: 206f 7665 7220 6174 6f6d 2061 0a20 2020   over atom a.   
-00002740: 2020 2020 2066 6f72 2061 2c20 7a61 2069       for a, za i
-00002750: 6e20 656e 756d 6572 6174 6528 626f 726e  n enumerate(born
-00002760: 5f63 6861 7267 6573 293a 0a20 2020 2020  _charges):.     
-00002770: 2020 2020 2020 2023 2061 746f 6d20 6973         # atom is
-00002780: 2074 6865 2061 746f 6d20 696e 6465 780a   the atom index.
-00002790: 2020 2020 2020 2020 2020 2020 2320 626f              # bo
-000027a0: 726e 2063 6f6e 7461 696e 7320 7468 6520  rn contains the 
-000027b0: 706f 6c61 7269 7361 6269 6c69 7479 2074  polarisability t
-000027c0: 656e 736f 7220 5b7a 3178 207a 3179 207a  ensor [z1x z1y z
-000027d0: 317a 5d20 5b7a 3278 207a 3279 207a 327a  1z] [z2x z2y z2z
-000027e0: 5d20 5b7a 3378 207a 3379 207a 337a 5d5d  ] [z3x z3y z3z]]
-000027f0: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
-00002800: 6865 7265 2031 2c20 322c 2033 2061 7265  here 1, 2, 3 are
-00002810: 2074 6865 2064 6972 6563 7469 6f6e 7320   the directions 
-00002820: 6f66 2074 6865 2066 6965 6c64 2061 6e64  of the field and
-00002830: 2078 2c20 792c 207a 2061 7265 2074 6865   x, y, z are the
-00002840: 2063 6f6f 7264 696e 6174 6573 206f 6620   coordinates of 
-00002850: 7468 6520 6174 6f6d 0a20 2020 2020 2020  the atom.       
-00002860: 2020 2020 207a 6120 3d20 6e70 2e64 6f74       za = np.dot
-00002870: 2871 2c20 7a61 290a 2020 2020 2020 2020  (q, za).        
-00002880: 2020 2020 2320 4c6f 6f70 206f 7665 7220      # Loop over 
-00002890: 6174 6f6d 2062 0a20 2020 2020 2020 2020  atom b.         
-000028a0: 2020 2066 6f72 2062 2c20 7a62 2069 6e20     for b, zb in 
-000028b0: 656e 756d 6572 6174 6528 626f 726e 5f63  enumerate(born_c
-000028c0: 6861 7267 6573 293a 0a20 2020 2020 2020  harges):.       
-000028d0: 2020 2020 2020 2020 207a 6220 3d20 6e70           zb = np
-000028e0: 2e64 6f74 2871 2c20 7a62 290a 2020 2020  .dot(q, zb).    
-000028f0: 2020 2020 2020 2020 2020 2020 7465 726d              term
-00002900: 7320 3d20 6e70 2e6f 7574 6572 287a 612c  s = np.outer(za,
-00002910: 207a 6229 202a 2063 6f6e 7374 616e 7420   zb) * constant 
-00002920: 2f20 6d61 7468 2e73 7172 7428 6d61 7373  / math.sqrt(mass
-00002930: 6573 5b61 5d2a 6d61 7373 6573 5b62 5d29  es[a]*masses[b])
-00002940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002950: 2069 203d 2061 2a33 0a20 2020 2020 2020   i = a*3.       
-00002960: 2020 2020 2020 2020 2066 6f72 2074 6572           for ter
-00002970: 6d69 2069 6e20 7465 726d 733a 0a20 2020  mi in terms:.   
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 206a 203d 2062 2a33 0a20 2020 2020 2020   j = b*3.       
-000029a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000029b0: 2074 6572 6d20 696e 2074 6572 6d69 3a0a   term in termi:.
-000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029d0: 2020 2020 2020 2020 576d 5b69 2c20 6a5d          Wm[i, j]
-000029e0: 203d 2074 6572 6d0a 2020 2020 2020 2020   = term.        
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 6a20 3d20 6a20 2b20 310a 2020 2020 2020  j = j + 1.      
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00002a20: 656e 6420 666f 7220 7465 726d 0a20 2020  end for term.   
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2069 203d 2069 202b 2031 0a20 2020 2020   i = i + 1.     
-00002a50: 2020 2020 2020 2020 2020 2023 2065 6e64             # end
-00002a60: 2066 6f72 2069 0a20 2020 2020 2020 2020   for i.         
-00002a70: 2020 2023 2065 6e64 206c 6f6f 7020 6f76     # end loop ov
-00002a80: 6572 2062 0a20 2020 2020 2020 2023 2065  er b.        # e
-00002a90: 6e64 206c 6f6f 7020 6f76 6572 2061 0a20  nd loop over a. 
-00002aa0: 2020 2020 2020 2023 2043 6f6e 7374 7275         # Constru
-00002ab0: 6374 2074 6865 2066 756c 6c20 6479 6e61  ct the full dyna
-00002ac0: 6d69 6361 6c20 6d61 7472 6978 2077 6974  mical matrix wit
-00002ad0: 6820 7468 6520 636f 7272 6563 7469 6f6e  h the correction
-00002ae0: 0a20 2020 2020 2020 2044 6d71 203d 2044  .        Dmq = D
-00002af0: 6d20 2b20 576d 0a20 2020 2020 2020 2023  m + Wm.        #
-00002b00: 2049 6620 7072 6f6a 6563 7469 6f6e 2077   If projection w
-00002b10: 6173 2072 6571 7565 7374 6564 2077 6865  as requested whe
-00002b20: 6e20 7468 6520 6d61 7472 6978 2077 6173  n the matrix was
-00002b30: 2072 6561 642c 2070 726f 6a65 6374 206f   read, project o
-00002b40: 7574 2074 7261 6e73 6c61 7469 6f6e 0a20  ut translation. 
-00002b50: 2020 2020 2020 2069 6620 7265 6164 6572         if reader
-00002b60: 2e65 636b 6172 743a 0a20 2020 2020 2020  .eckart:.       
-00002b70: 2020 2020 2072 6561 6465 722e 7072 6f6a       reader.proj
-00002b80: 6563 7428 446d 7129 0a20 2020 2020 2020  ect(Dmq).       
-00002b90: 2065 6967 5f76 616c 2c20 6569 675f 7665   eig_val, eig_ve
-00002ba0: 6320 3d20 6e70 2e6c 696e 616c 672e 6569  c = np.linalg.ei
-00002bb0: 6768 2844 6d71 290a 2020 2020 2020 2020  gh(Dmq).        
-00002bc0: 2320 4966 2065 6967 5f76 616c 206c 6573  # If eig_val les
-00002bd0: 7320 7468 616e 207a 6572 6f20 7765 2073  s than zero we s
-00002be0: 6574 2069 7420 746f 207a 6572 6f0a 2020  et it to zero.  
-00002bf0: 2020 2020 2020 7661 6c75 6573 203d 205b        values = [
-00002c00: 5d0a 2020 2020 2020 2020 666f 7220 6569  ].        for ei
-00002c10: 6720 696e 2065 6967 5f76 616c 3a0a 2020  g in eig_val:.  
-00002c20: 2020 2020 2020 2020 2020 6966 2065 6967            if eig
-00002c30: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
-00002c40: 2020 2020 2020 2076 616c 203d 206d 6174         val = mat
-00002c50: 682e 7371 7274 2865 6967 290a 2020 2020  h.sqrt(eig).    
-00002c60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00002c80: 6c20 3d20 2d6d 6174 682e 7371 7274 282d  l = -math.sqrt(-
-00002c90: 6569 6729 0a20 2020 2020 2020 2020 2020  eig).           
-00002ca0: 2076 616c 7565 732e 6170 7065 6e64 2876   values.append(v
-00002cb0: 616c 290a 2020 2020 2020 2020 2320 656e  al).        # en
-00002cc0: 6420 6f66 2066 6f72 2065 6967 0a20 2020  d of for eig.   
-00002cd0: 2020 2020 2023 2053 6f72 7420 7468 6520       # Sort the 
-00002ce0: 6569 6765 6e20 7661 6c75 6573 2069 6e20  eigen values in 
-00002cf0: 6173 6365 6e64 696e 6720 6f72 6465 7220  ascending order 
-00002d00: 616e 6420 6170 7065 6e64 2074 6f20 7468  and append to th
-00002d10: 6520 7265 7375 6c74 730a 2020 2020 2020  e results.      
-00002d20: 2020 7265 7375 6c74 732e 6170 7065 6e64    results.append
-00002d30: 286e 702e 736f 7274 2876 616c 7565 7329  (np.sort(values)
-00002d40: 290a 2020 2020 2320 656e 6420 6c6f 6f70  ).    # end loop
-00002d50: 206f 7665 7220 710a 2020 2020 7265 7475   over q.    retu
-00002d60: 726e 2072 6573 756c 7473 0a0a 6465 6620  rn results..def 
-00002d70: 6f73 6369 6c6c 6174 6f72 5f73 7472 656e  oscillator_stren
-00002d80: 6774 6873 286e 6f72 6d61 6c5f 6d6f 6465  gths(normal_mode
-00002d90: 732c 2062 6f72 6e5f 6368 6172 6765 7329  s, born_charges)
-00002da0: 3a0a 2020 2020 2222 2243 616c 6375 6c61  :.    """Calcula
-00002db0: 7465 206f 7363 696c 6c61 746f 7220 7374  te oscillator st
-00002dc0: 7265 6e67 7468 7320 6672 6f6d 2074 6865  rengths from the
-00002dd0: 206e 6f72 6d61 6c20 6d6f 6465 7320 616e   normal modes an
-00002de0: 6420 7468 6520 626f 726e 2063 6861 7267  d the born charg
-00002df0: 6573 0a20 2020 2020 2020 6e6f 726d 616c  es.       normal
-00002e00: 5f6d 6f64 6573 2061 7265 2069 6e20 7468  _modes are in th
-00002e10: 6520 6d61 7373 2077 6569 6768 7465 6420  e mass weighted 
-00002e20: 636f 6f72 6469 6e61 7465 2073 7973 7465  coordinate syste
-00002e30: 6d20 616e 6420 6e6f 726d 616c 6973 6564  m and normalised
-00002e40: 0a20 2020 2020 2020 626f 726e 2063 6861  .       born cha
-00002e50: 7267 6573 2061 7265 2069 6e20 656c 6563  rges are in elec
-00002e60: 7472 6f6e 732c 2073 6f20 6174 6f6d 6963  trons, so atomic
-00002e70: 2075 6e69 7473 2222 220a 2020 2020 2320   units""".    # 
-00002e80: 4561 6368 206d 6f64 6520 6861 7320 6120  Each mode has a 
-00002e90: 3378 3320 6f73 6369 6c6c 6174 6f72 2073  3x3 oscillator s
-00002ea0: 7472 656e 6774 680a 2020 2020 6e6d 6f64  trength.    nmod
-00002eb0: 6573 203d 206e 702e 7369 7a65 286e 6f72  es = np.size(nor
-00002ec0: 6d61 6c5f 6d6f 6465 732c 2030 290a 2020  mal_modes, 0).  
-00002ed0: 2020 6f73 6369 6c6c 6174 6f72 5f73 7472    oscillator_str
-00002ee0: 656e 6774 6873 203d 206e 702e 7a65 726f  engths = np.zero
-00002ef0: 7328 286e 6d6f 6465 732c 2033 2c20 3329  s((nmodes, 3, 3)
-00002f00: 290a 2020 2020 666f 7220 696d 6f64 652c  ).    for imode,
-00002f10: 206d 6f64 6520 696e 2065 6e75 6d65 7261   mode in enumera
-00002f20: 7465 286e 6f72 6d61 6c5f 6d6f 6465 7329  te(normal_modes)
-00002f30: 3a0a 2020 2020 2020 2020 2320 5765 2063  :.        # We c
-00002f40: 616c 6375 6c61 7465 2074 6865 2064 6970  alculate the dip
-00002f50: 6f6c 6520 696e 6475 6365 6420 6279 2064  ole induced by d
-00002f60: 6973 706c 6163 656d 656e 7420 6f66 2065  isplacement of e
-00002f70: 6163 6820 6174 6f6d 2061 6c6f 6e67 2074  ach atom along t
-00002f80: 6865 206e 6f72 6d61 6c20 6d6f 6465 0a20  he normal mode. 
-00002f90: 2020 2020 2020 207a 5f69 6d6f 6465 203d         z_imode =
-00002fa0: 206e 702e 7a65 726f 7328 3329 0a20 2020   np.zeros(3).   
-00002fb0: 2020 2020 2066 6f72 2061 746f 6d2c 2062       for atom, b
-00002fc0: 6f72 6e20 696e 2065 6e75 6d65 7261 7465  orn in enumerate
-00002fd0: 2862 6f72 6e5f 6368 6172 6765 7329 3a0a  (born_charges):.
-00002fe0: 2020 2020 2020 2020 2020 2020 2320 6174              # at
-00002ff0: 6f6d 2069 7320 7468 6520 6174 6f6d 2069  om is the atom i
-00003000: 6e64 6578 0a20 2020 2020 2020 2020 2020  ndex.           
-00003010: 2023 2062 6f72 6e20 636f 6e74 6169 6e73   # born contains
-00003020: 2074 6865 2070 6f6c 6172 6973 6162 696c   the polarisabil
-00003030: 6974 7920 7465 6e73 6f72 205b 6131 7820  ity tensor [a1x 
-00003040: 6131 7920 6131 7a5d 205b 6132 7820 6132  a1y a1z] [a2x a2
-00003050: 7920 6132 7a5d 205b 6133 7820 6133 7920  y a2z] [a3x a3y 
-00003060: 6133 7a5d 5d0a 2020 2020 2020 2020 2020  a3z]].          
-00003070: 2020 2320 7768 6572 6520 312c 2032 2c20    # where 1, 2, 
-00003080: 3320 6172 6520 7468 6520 6469 7265 6374  3 are the direct
-00003090: 696f 6e73 206f 6620 7468 6520 6669 656c  ions of the fiel
-000030a0: 6420 616e 6420 782c 2079 2c20 7a20 6172  d and x, y, z ar
-000030b0: 6520 7468 6520 636f 6f72 6469 6e61 7465  e the coordinate
-000030c0: 7320 6f66 2074 6865 2061 746f 6d0a 2020  s of the atom.  
-000030d0: 2020 2020 2020 2020 2020 7a5f 696d 6f64            z_imod
-000030e0: 6520 3d20 7a5f 696d 6f64 6520 2b20 6e70  e = z_imode + np
-000030f0: 2e64 6f74 2862 6f72 6e2c 206d 6f64 655b  .dot(born, mode[
-00003100: 6174 6f6d 5d29 2020 2320 7468 6520 6469  atom])  # the di
-00003110: 7370 6c61 6365 6d65 6e74 2069 7320 616e  splacement is an
-00003120: 2061 7272 6179 205b 782c 2079 2c20 7a5d   array [x, y, z]
-00003130: 0a20 2020 2020 2020 2023 2065 6e64 2066  .        # end f
-00003140: 6f72 0a20 2020 2020 2020 2023 2054 6865  or.        # The
-00003150: 206f 7363 696c 6c61 746f 7220 7374 7265   oscillator stre
-00003160: 6e67 7468 206d 6174 7269 7820 6973 2074  ngth matrix is t
-00003170: 6865 206f 7574 6572 2070 726f 6475 6374  he outer product
-00003180: 206f 6620 7a0a 2020 2020 2020 2020 6f73   of z.        os
-00003190: 6369 6c6c 6174 6f72 5f73 7472 656e 6774  cillator_strengt
-000031a0: 6873 5b69 6d6f 6465 5d20 3d20 6e70 2e6f  hs[imode] = np.o
-000031b0: 7574 6572 287a 5f69 6d6f 6465 2c20 7a5f  uter(z_imode, z_
-000031c0: 696d 6f64 6529 0a20 2020 2023 2065 6e64  imode).    # end
-000031d0: 2066 6f72 0a20 2020 2072 6574 7572 6e20   for.    return 
-000031e0: 6f73 6369 6c6c 6174 6f72 5f73 7472 656e  oscillator_stren
-000031f0: 6774 6873 0a0a 6465 6620 6e6f 726d 616c  gths..def normal
-00003200: 5f6d 6f64 6573 286d 6173 7365 732c 206d  _modes(masses, m
-00003210: 6173 735f 7765 6967 6874 6564 5f6e 6f72  ass_weighted_nor
-00003220: 6d61 6c5f 6d6f 6465 7329 3a0a 2020 2020  mal_modes):.    
-00003230: 2222 2220 5472 616e 7366 6f72 6d20 6672  """ Transform fr
-00003240: 6f6d 206d 6173 7320 7765 6967 6874 6564  om mass weighted
-00003250: 2063 6f6f 7264 696e 6174 6573 2074 6f20   coordinates to 
-00003260: 7879 7a2e 204e 6f74 6520 7468 6973 2072  xyz. Note this r
-00003270: 6574 7572 6e73 2061 6e20 6172 7261 7920  eturns an array 
-00003280: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00003290: 5468 6520 7265 7475 726e 6564 206e 6f72  The returned nor
-000032a0: 6d61 6c20 6d6f 6465 7320 6861 7665 204e  mal modes have N
-000032b0: 4f54 2062 6565 6e20 7265 6e6f 726d 616c  OT been renormal
-000032c0: 6973 6564 2e0a 2020 2020 2020 2020 5468  ised..        Th
-000032d0: 6520 696e 7075 7420 6d61 7373 6573 2061  e input masses a
-000032e0: 7265 2069 6e20 6174 6f6d 6963 2075 6e69  re in atomic uni
-000032f0: 7473 0a20 2020 2020 2020 2074 6865 206f  ts.        the o
-00003300: 7574 7075 7420 6e6f 726d 616c 206d 6f64  utput normal mod
-00003310: 6573 2061 7265 2069 6e20 6174 6f6d 6963  es are in atomic
-00003320: 2075 6e69 7473 2022 2222 0a20 2020 206c   units """.    l
-00003330: 6973 745f 6d20 3d20 5b5d 0a20 2020 206e  ist_m = [].    n
-00003340: 6f72 6d61 6c5f 6d6f 6465 7320 3d20 6e70  ormal_modes = np
-00003350: 2e7a 6572 6f73 5f6c 696b 6528 6d61 7373  .zeros_like(mass
-00003360: 5f77 6569 6768 7465 645f 6e6f 726d 616c  _weighted_normal
-00003370: 5f6d 6f64 6573 290a 2020 2020 6e69 6f6e  _modes).    nion
-00003380: 7320 3d20 6e70 2e73 697a 6528 6d61 7373  s = np.size(mass
-00003390: 6573 290a 2020 2020 666f 7220 6120 696e  es).    for a in
-000033a0: 2072 616e 6765 286e 696f 6e73 293a 0a20   range(nions):. 
-000033b0: 2020 2020 2020 2078 203d 2031 2e30 202f         x = 1.0 /
-000033c0: 206d 6174 682e 7371 7274 286d 6173 7365   math.sqrt(masse
-000033d0: 735b 615d 290a 2020 2020 2020 2020 6174  s[a]).        at
-000033e0: 6f6d 203d 205b 782c 2078 2c20 785d 0a20  om = [x, x, x]. 
-000033f0: 2020 2020 2020 206c 6973 745f 6d2e 6170         list_m.ap
-00003400: 7065 6e64 2861 746f 6d29 0a20 2020 2023  pend(atom).    #
-00003410: 2065 6e64 206f 6620 6c6f 6f70 206f 6620   end of loop of 
-00003420: 696f 6e73 0a20 2020 2061 7272 6179 5f6d  ions.    array_m
-00003430: 203d 206e 702e 6172 7261 7928 6c69 7374   = np.array(list
-00003440: 5f6d 290a 2020 2020 666f 7220 696e 6465  _m).    for inde
-00003450: 782c 206d 6f64 6520 696e 2065 6e75 6d65  x, mode in enume
-00003460: 7261 7465 286d 6173 735f 7765 6967 6874  rate(mass_weight
-00003470: 6564 5f6e 6f72 6d61 6c5f 6d6f 6465 7329  ed_normal_modes)
-00003480: 3a0a 2020 2020 2020 2020 6e6f 726d 616c  :.        normal
-00003490: 5f6d 6f64 6573 5b69 6e64 6578 5d20 3d20  _modes[index] = 
-000034a0: 6d6f 6465 202a 2061 7272 6179 5f6d 0a20  mode * array_m. 
-000034b0: 2020 2072 6574 7572 6e20 6e6f 726d 616c     return normal
-000034c0: 5f6d 6f64 6573 0a0a 6465 6620 7072 6f6a  _modes..def proj
-000034d0: 6563 745f 6669 656c 6428 7368 6170 652c  ect_field(shape,
-000034e0: 2073 6861 7065 5f64 6174 612c 2070 726f   shape_data, pro
-000034f0: 6a65 6374 696f 6e2c 2065 6669 656c 6429  jection, efield)
-00003500: 3a0a 2020 2020 2222 2254 616b 6520 7468  :.    """Take th
-00003510: 6520 6669 656c 6420 6469 7265 6374 696f  e field directio
-00003520: 6e73 2069 6e20 6566 6965 6c64 2061 6e64  ns in efield and
-00003530: 2061 7070 6c79 2073 6861 7065 2070 726f   apply shape pro
-00003540: 6a65 6374 696f 6e2e 2222 220a 2020 2020  jection.""".    
-00003550: 6966 2070 726f 6a65 6374 696f 6e20 3d3d  if projection ==
-00003560: 2022 7261 6e64 6f6d 223a 0a20 2020 2020   "random":.     
-00003570: 2020 2072 6574 7572 6e20 6e70 2e61 7272     return np.arr
-00003580: 6179 2865 6669 656c 6429 0a20 2020 2065  ay(efield).    e
-00003590: 6c69 6620 7072 6f6a 6563 7469 6f6e 203d  lif projection =
-000035a0: 3d20 2270 6172 616c 6c65 6c22 3a0a 2020  = "parallel":.  
-000035b0: 2020 2020 2020 6966 2073 6861 7065 203d        if shape =
-000035c0: 3d20 2273 7068 6572 6522 3a0a 2020 2020  = "sphere":.    
-000035d0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-000035e0: 702e 6172 7261 7928 6566 6965 6c64 290a  p.array(efield).
-000035f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00003600: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003610: 206e 702e 6172 7261 7928 7368 6170 655f   np.array(shape_
-00003620: 6461 7461 290a 2020 2020 656c 6966 2070  data).    elif p
-00003630: 726f 6a65 6374 696f 6e20 3d3d 2022 7065  rojection == "pe
-00003640: 7270 656e 6469 6375 6c61 7222 3a0a 2020  rpendicular":.  
-00003650: 2020 2020 2020 6966 2073 6861 7065 203d        if shape =
-00003660: 3d20 2273 7068 6572 6522 3a0a 2020 2020  = "sphere":.    
-00003670: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00003680: 702e 6172 7261 7928 6566 6965 6c64 290a  p.array(efield).
-00003690: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000036a0: 2020 2020 2020 2020 2020 7072 6f6a 5f66            proj_f
-000036b0: 6965 6c64 203d 205b 5d0a 2020 2020 2020  ield = [].      
-000036c0: 2020 2020 2020 6461 7461 203d 206e 702e        data = np.
-000036d0: 6172 7261 7928 7368 6170 655f 6461 7461  array(shape_data
-000036e0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-000036f0: 7220 6669 656c 6420 696e 2065 6669 656c  r field in efiel
-00003700: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-00003710: 2020 2070 726f 6a20 3d20 6669 656c 6420     proj = field 
-00003720: 2d20 286e 702e 646f 7428 6461 7461 2c20  - (np.dot(data, 
-00003730: 6669 656c 6429 202a 2064 6174 6129 0a20  field) * data). 
-00003740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003750: 697a 6520 3d20 6e70 2e6c 696e 616c 672e  ize = np.linalg.
-00003760: 6e6f 726d 2870 726f 6a5f 6669 656c 6429  norm(proj_field)
-00003770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003780: 2069 6620 7369 7a65 203e 2030 2e30 3030   if size > 0.000
-00003790: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-000037a0: 2020 2020 2020 2070 726f 6a5f 6669 656c         proj_fiel
-000037b0: 642e 6170 7065 6e64 2870 726f 6a29 0a20  d.append(proj). 
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000037d0: 2065 6e64 2069 660a 2020 2020 2020 2020   end if.        
-000037e0: 2020 2020 2320 656e 6420 666f 720a 2020      # end for.  
-000037f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003800: 206e 702e 6172 7261 7928 7072 6f6a 5f66   np.array(proj_f
-00003810: 6965 6c64 290a 2020 2020 656c 7365 3a0a  ield).    else:.
-00003820: 2020 2020 2020 2020 7072 696e 7428 2245          print("E
-00003830: 7272 6f72 2069 6e20 7072 6f6a 6563 745f  rror in project_
-00003840: 6669 656c 642c 2070 726f 6a65 6374 696f  field, projectio
-00003850: 6e20 756e 6b6f 776e 3a20 222c 2070 726f  n unkown: ", pro
-00003860: 6a65 6374 696f 6e2c 2066 696c 653d 7379  jection, file=sy
-00003870: 732e 7374 6465 7272 290a 2020 2020 2020  s.stderr).      
-00003880: 2020 6578 6974 2831 290a 2020 2020 7265    exit(1).    re
-00003890: 7475 726e 0a0a 6465 6620 726f 6772 6964  turn..def rogrid
-000038a0: 6775 6573 5f72 6f74 6174 696f 6e73 2865  gues_rotations(e
-000038b0: 6669 656c 6429 3a0a 2020 2020 2222 2254  field):.    """T
-000038c0: 616b 6520 7468 6520 6669 656c 6420 6469  ake the field di
-000038d0: 7265 6374 696f 6e73 2069 6e20 6566 6965  rections in efie
-000038e0: 6c64 2061 6e64 2075 7365 2065 6163 6820  ld and use each 
-000038f0: 6469 7265 6374 696f 6e20 746f 2063 616c  direction to cal
-00003900: 6375 6c61 7465 2061 2072 616e 646f 6d20  culate a random 
-00003910: 726f 7461 7469 6f6e 2061 626f 7574 2074  rotation about t
-00003920: 6861 7420 6178 6973 2e0a 2020 2020 2020  hat axis..      
-00003930: 2055 7365 2074 6865 2066 6965 6c64 2028   Use the field (
-00003940: 7768 6963 6820 6120 7261 6e64 6f6d 2075  which a random u
-00003950: 6e69 7420 7665 6374 6f72 2069 6e20 7879  nit vector in xy
-00003960: 7a20 7370 6163 6529 2074 6f20 6765 6e65  z space) to gene
-00003970: 7261 7465 2061 6e20 6f72 7468 6f67 6f6e  rate an orthogon
-00003980: 616c 2072 6f74 6174 696f 6e20 6d61 7472  al rotation matr
-00003990: 6978 0a20 2020 2020 2020 526f 6472 6967  ix.       Rodrig
-000039a0: 7565 7320 726f 7461 7469 6f6e 2066 6f72  ues rotation for
-000039b0: 6d75 6c61 2041 203d 2049 332e 2063 6f73  mula A = I3. cos
-000039c0: 2874 6865 7461 2920 2b20 2831 2d63 6f73  (theta) + (1-cos
-000039d0: 2874 6865 7461 2929 2065 202e 2065 5420  (theta)) e . eT 
-000039e0: 2b20 6578 2073 696e 2874 6865 7461 300a  + ex sin(theta0.
-000039f0: 2020 2020 2020 2049 3320 6973 2061 2075         I3 is a u
-00003a00: 6e69 7420 6d61 7472 6978 0a20 2020 2020  nit matrix.     
-00003a10: 2020 6520 6973 2074 6865 2064 6972 6563    e is the direc
-00003a20: 7469 6f6e 0a20 2020 2020 2020 6578 2069  tion.       ex i
-00003a30: 7320 7468 6520 6372 6f73 7320 7072 6f64  s the cross prod
-00003a40: 7563 7420 6d61 7472 6978 0a20 2020 2020  uct matrix.     
-00003a50: 2020 2820 3020 202d 6533 2020 2065 3229    ( 0  -e3   e2)
-00003a60: 0a20 2020 2020 2020 2820 6533 2020 3020  .       ( e3  0 
-00003a70: 2020 2d65 3129 0a20 2020 2020 2020 282d    -e1).       (-
-00003a80: 6532 2020 6531 2020 2030 2029 0a20 2020  e2  e1   0 ).   
-00003a90: 2020 2020 496e 7075 7420 6669 656c 6420      Input field 
-00003aa0: 6973 2072 6561 6c0a 2020 2020 2020 204f  is real.       O
-00003ab0: 7574 7075 7420 6973 2061 206c 6973 7420  utput is a list 
-00003ac0: 6f66 2072 6f74 6174 696f 6e73 0a20 2020  of rotations.   
-00003ad0: 2022 2222 0a20 2020 2072 6f74 6174 696f   """.    rotatio
-00003ae0: 6e73 203d 205b 5d0a 2020 2020 666f 7220  ns = [].    for 
-00003af0: 6669 656c 6420 696e 2065 6669 656c 643a  field in efield:
-00003b00: 0a20 2020 2020 2020 2023 2043 616c 6375  .        # Calcu
-00003b10: 6c61 7465 2061 2072 616e 646f 6d20 616e  late a random an
-00003b20: 676c 6520 6265 7477 6565 6e20 3020 616e  gle between 0 an
-00003b30: 6420 3138 300a 2020 2020 2020 2020 7468  d 180.        th
-00003b40: 6574 6120 3d20 5049 2a6e 702e 7261 6e64  eta = PI*np.rand
-00003b50: 6f6d 2e72 616e 6428 290a 2020 2020 2020  om.rand().      
-00003b60: 2020 636f 7320 2020 3d20 6e70 2e63 6f73    cos   = np.cos
-00003b70: 2874 6865 7461 290a 2020 2020 2020 2020  (theta).        
-00003b80: 7369 6e20 2020 3d20 6e70 2e73 696e 2874  sin   = np.sin(t
-00003b90: 6865 7461 290a 2020 2020 2020 2020 726f  heta).        ro
-00003ba0: 7461 7469 6f6e 203d 206e 702e 7a65 726f  tation = np.zero
-00003bb0: 7328 2833 2c20 3329 290a 2020 2020 2020  s((3, 3)).      
-00003bc0: 2020 6531 203d 2066 6965 6c64 5b30 5d0a    e1 = field[0].
-00003bd0: 2020 2020 2020 2020 6532 203d 2066 6965          e2 = fie
-00003be0: 6c64 5b31 5d0a 2020 2020 2020 2020 6533  ld[1].        e3
-00003bf0: 203d 2066 6965 6c64 5b32 5d0a 2020 2020   = field[2].    
-00003c00: 2020 2020 726f 7461 7469 6f6e 5b30 2c20      rotation[0, 
-00003c10: 305d 203d 2063 6f73 202b 2028 312d 636f  0] = cos + (1-co
-00003c20: 7329 2a65 312a 6531 0a20 2020 2020 2020  s)*e1*e1.       
-00003c30: 2072 6f74 6174 696f 6e5b 302c 2031 5d20   rotation[0, 1] 
-00003c40: 3d20 2831 2d63 6f73 292a 6532 2a65 3120  = (1-cos)*e2*e1 
-00003c50: 2b20 7369 6e2a 6533 0a20 2020 2020 2020  + sin*e3.       
-00003c60: 2072 6f74 6174 696f 6e5b 302c 2032 5d20   rotation[0, 2] 
-00003c70: 3d20 2831 2d63 6f73 292a 6533 2a65 3120  = (1-cos)*e3*e1 
-00003c80: 2d20 7369 6e2a 6532 0a20 2020 2020 2020  - sin*e2.       
-00003c90: 2072 6f74 6174 696f 6e5b 312c 2030 5d20   rotation[1, 0] 
-00003ca0: 3d20 2831 2d63 6f73 292a 6531 2a65 3220  = (1-cos)*e1*e2 
-00003cb0: 2d20 7369 6e2a 6533 0a20 2020 2020 2020  - sin*e3.       
-00003cc0: 2072 6f74 6174 696f 6e5b 312c 2031 5d20   rotation[1, 1] 
-00003cd0: 3d20 636f 7320 2b20 2831 2d63 6f73 292a  = cos + (1-cos)*
-00003ce0: 6532 2a65 320a 2020 2020 2020 2020 726f  e2*e2.        ro
-00003cf0: 7461 7469 6f6e 5b31 2c20 325d 203d 2028  tation[1, 2] = (
-00003d00: 312d 636f 7329 2a65 332a 6532 202b 2073  1-cos)*e3*e2 + s
-00003d10: 696e 2a65 310a 2020 2020 2020 2020 726f  in*e1.        ro
-00003d20: 7461 7469 6f6e 5b32 2c20 305d 203d 2028  tation[2, 0] = (
-00003d30: 312d 636f 7329 2a65 312a 6533 202b 2073  1-cos)*e1*e3 + s
-00003d40: 696e 2a65 320a 2020 2020 2020 2020 726f  in*e2.        ro
-00003d50: 7461 7469 6f6e 5b32 2c20 315d 203d 2028  tation[2, 1] = (
-00003d60: 312d 636f 7329 2a65 322a 6533 202d 2073  1-cos)*e2*e3 - s
-00003d70: 696e 2a65 310a 2020 2020 2020 2020 726f  in*e1.        ro
-00003d80: 7461 7469 6f6e 5b32 2c20 325d 203d 2063  tation[2, 2] = c
-00003d90: 6f73 202b 2028 312d 636f 7329 2a65 332a  os + (1-cos)*e3*
-00003da0: 6533 0a20 2020 2020 2020 2072 6f74 6174  e3.        rotat
-00003db0: 696f 6e73 2e61 7070 656e 6428 726f 7461  ions.append(rota
-00003dc0: 7469 6f6e 290a 2020 2020 7265 7475 726e  tion).    return
-00003dd0: 2072 6f74 6174 696f 6e73 0a0a 6465 6620   rotations..def 
-00003de0: 6162 736f 7270 7469 6f6e 5f66 726f 6d5f  absorption_from_
-00003df0: 6d6f 6465 5f69 6e74 656e 7369 7469 6573  mode_intensities
-00003e00: 2866 2c20 6d6f 6465 732c 2066 7265 7175  (f, modes, frequ
-00003e10: 656e 6369 6573 2c20 7369 676d 6173 2c20  encies, sigmas, 
-00003e20: 696e 7465 6e73 6974 6965 7329 3a0a 2020  intensities):.  
-00003e30: 2020 2222 2243 616c 6375 6c61 7465 2074    """Calculate t
-00003e40: 6865 2061 6273 6f72 7074 696f 6e20 6672  he absorption fr
-00003e50: 6f6d 2074 6865 2066 7265 7175 656e 6369  om the frequenci
-00003e60: 6573 2061 6e64 2069 6e74 656e 7369 7469  es and intensiti
-00003e70: 6573 2075 7369 6e67 2061 204c 6f72 656e  es using a Loren
-00003e80: 747a 6961 6e0a 2020 2020 2020 2066 2069  tzian.       f i
-00003e90: 7320 7468 6520 6672 6571 7565 6e63 7920  s the frequency 
-00003ea0: 6f66 2074 6865 2061 6273 6f72 7074 696f  of the absorptio
-00003eb0: 6e20 696e 2063 6d2d 310a 2020 2020 2020  n in cm-1.      
-00003ec0: 206d 6f64 6573 2061 7265 2061 206c 6973   modes are a lis
-00003ed0: 7420 6f66 2074 6865 206d 6f64 6573 0a20  t of the modes. 
-00003ee0: 2020 2020 2020 6672 6571 7565 6e63 6965        frequencie
-00003ef0: 7328 636d 2d31 292c 2073 6967 6d61 7328  s(cm-1), sigmas(
-00003f00: 636d 2d31 2920 616e 6420 696e 7465 6e73  cm-1) and intens
-00003f10: 6974 6965 7320 2844 322f 4132 2f61 6d75  ities (D2/A2/amu
-00003f20: 290a 2020 2020 2020 2054 6865 206e 756d  ).       The num
-00003f30: 6265 7220 3432 3235 2e36 2063 6f6e 7665  ber 4225.6 conve
-00003f40: 7274 7320 7468 6520 756e 6974 7320 6f66  rts the units of
-00003f50: 2044 322f 4132 2f61 6d75 2074 6f20 4c20   D2/A2/amu to L 
-00003f60: 6d6f 6c65 2d31 2063 6d2d 3120 636d 2d31  mole-1 cm-1 cm-1
-00003f70: 0a20 2020 2020 2020 5468 6520 6f75 7470  .       The outp
-00003f80: 7574 2066 726f 6d20 7468 6973 2069 7320  ut from this is 
-00003f90: 7468 6520 6d6f 6c61 7220 6162 736f 7270  the molar absorp
-00003fa0: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
-00003fb0: 2061 7420 662c 2069 6e20 4c2f 6d6f 6c2f   at f, in L/mol/
-00003fc0: 636d 2222 220a 2020 2020 6162 736f 7270  cm""".    absorp
-00003fd0: 7469 6f6e 203d 2030 2e30 0a20 2020 2066  tion = 0.0.    f
-00003fe0: 6f72 206d 6f64 6520 696e 206d 6f64 6573  or mode in modes
-00003ff0: 3a0a 2020 2020 2020 2020 7620 3d20 6e70  :.        v = np
-00004000: 2e72 6561 6c28 6672 6571 7565 6e63 6965  .real(frequencie
-00004010: 735b 6d6f 6465 5d29 0a20 2020 2020 2020  s[mode]).       
-00004020: 2073 6967 6d61 203d 2073 6967 6d61 735b   sigma = sigmas[
-00004030: 6d6f 6465 5d0a 2020 2020 2020 2020 6963  mode].        ic
-00004040: 6173 7465 7020 3d20 696e 7465 6e73 6974  astep = intensit
-00004050: 6965 735b 6d6f 6465 5d0a 2020 2020 2020  ies[mode].      
-00004060: 2020 6162 736f 7270 7469 6f6e 203d 2061    absorption = a
-00004070: 6273 6f72 7074 696f 6e20 2b20 322e 3020  bsorption + 2.0 
-00004080: 2a20 3432 3235 2e36 202a 2069 6361 7374  * 4225.6 * icast
-00004090: 6570 202f 2050 4920 2a20 2873 6967 6d61  ep / PI * (sigma
-000040a0: 202f 2028 342e 3020 2a20 2866 202d 2076   / (4.0 * (f - v
-000040b0: 292a 2866 202d 2076 2920 2b20 7369 676d  )*(f - v) + sigm
-000040c0: 612a 7369 676d 6129 290a 2020 2020 7265  a*sigma)).    re
-000040d0: 7475 726e 2061 6273 6f72 7074 696f 6e0a  turn absorption.
-000040e0: 0a64 6566 2063 616c 6375 6c61 7465 5f73  .def calculate_s
-000040f0: 697a 655f 6661 6374 6f72 2028 7829 3a0a  ize_factor (x):.
-00004100: 2020 2020 2222 220a 2020 2020 4361 6c63      """.    Calc
-00004110: 756c 6174 6520 6120 7369 7a65 2065 6666  ulate a size eff
-00004120: 6563 7420 7573 696e 6720 4571 7561 7469  ect using Equati
-00004130: 6f6e 7320 3130 2e33 3820 616e 6420 3130  ons 10.38 and 10
-00004140: 2e33 3920 696e 2053 6968 766f 6c61 0a20  .39 in Sihvola. 
-00004150: 2020 2022 2222 0a20 2020 2069 6620 7820     """.    if x 
-00004160: 3c20 312e 3045 2d31 323a 0a20 2020 2020  < 1.0E-12:.     
-00004170: 2020 2072 6573 756c 7420 3d20 312e 300a     result = 1.0.
-00004180: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00004190: 2020 6978 203d 2063 6f6d 706c 6578 2830    ix = complex(0
-000041a0: 2c78 290a 2020 2020 2020 2020 6731 203d  ,x).        g1 =
-000041b0: 2032 2e30 202f 2033 2e30 202a 2028 2028   2.0 / 3.0 * ( (
-000041c0: 2031 2e30 202b 2069 7820 2920 2a20 6e70   1.0 + ix ) * np
-000041d0: 2e65 7870 282d 6978 2920 2d20 312e 3020  .exp(-ix) - 1.0 
-000041e0: 290a 2020 2020 2020 2020 6732 203d 2028  ).        g2 = (
-000041f0: 2031 202b 2069 7820 2d20 2837 2e30 2f31   1 + ix - (7.0/1
-00004200: 352e 3029 202a 2078 2a78 202d 2063 6f6d  5.0) * x*x - com
-00004210: 706c 6578 2830 2c32 2e30 2a78 2a78 2a78  plex(0,2.0*x*x*x
-00004220: 2f31 352e 3029 2029 202a 206e 702e 6578  /15.0) ) * np.ex
-00004230: 7028 2d69 7829 202d 312e 300a 2020 2020  p(-ix) -1.0.    
-00004240: 2020 2020 7265 7375 6c74 203d 2031 202d      result = 1 -
-00004250: 2067 3120 2d20 6732 0a20 2020 2072 6574   g1 - g2.    ret
-00004260: 7572 6e20 7265 7375 6c74 0a0a 6465 6620  urn result..def 
-00004270: 6176 6572 6167 6564 5f70 6572 6d69 7474  averaged_permitt
-00004280: 6976 6974 7928 6469 656c 6563 7472 6963  ivity(dielectric
-00004290: 5f6d 6564 6975 6d2c 2063 7279 7374 616c  _medium, crystal
-000042a0: 5f70 6572 6d69 7474 6976 6974 792c 2073  _permittivity, s
-000042b0: 6861 7065 2c20 4c2c 2076 662c 2073 697a  hape, L, vf, siz
-000042c0: 6529 3a0a 2020 2020 2222 2243 616c 6375  e):.    """Calcu
-000042d0: 6c61 7465 2074 6865 2065 6666 6563 7469  late the effecti
-000042e0: 7665 2063 6f6e 7374 616e 7420 7065 726d  ve constant perm
-000042f0: 6974 7469 7669 7479 2075 7369 6e67 2074  ittivity using t
-00004300: 6865 2061 7665 7261 6765 6420 7065 726d  he averaged perm
-00004310: 6974 7469 7669 7479 206d 6574 686f 640a  ittivity method.
-00004320: 2020 2020 2020 2064 6965 6c65 6374 7269         dielectri
-00004330: 635f 6d65 6469 756d 2069 7320 7468 6520  c_medium is the 
-00004340: 6469 656c 6563 7472 6963 2063 6f6e 7374  dielectric const
-00004350: 616e 7420 7465 6e73 6f72 206f 6620 7468  ant tensor of th
-00004360: 6520 6d65 6469 756d 0a20 2020 2020 2020  e medium.       
-00004370: 6372 7973 7461 6c5f 7065 726d 6974 7469  crystal_permitti
-00004380: 7669 7479 2069 7320 7468 6520 746f 7461  vity is the tota
-00004390: 6c20 6672 6571 7565 6e63 7920 6469 656c  l frequency diel
-000043a0: 6563 7472 6963 2063 6f6e 7374 616e 7420  ectric constant 
-000043b0: 7465 6e73 6f72 2061 7420 7468 6520 6375  tensor at the cu
-000043c0: 7272 656e 7420 6672 6571 7565 6e63 790a  rrent frequency.
-000043d0: 2020 2020 2020 2073 6861 7065 2069 7320         shape is 
-000043e0: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-000043f0: 6375 7272 656e 7420 7368 6170 650a 2020  current shape.  
-00004400: 2020 2020 204c 2069 7320 7468 6520 7368       L is the sh
-00004410: 6170 6573 2064 6570 6f6c 6172 6973 6174  apes depolarisat
-00004420: 696f 6e20 6d61 7472 6978 0a20 2020 2020  ion matrix.     
-00004430: 2020 7369 7a65 2069 7320 7468 6520 6469    size is the di
-00004440: 6d65 6e73 696f 6e6c 6573 7320 7369 7a65  mensionless size
-00004450: 2070 6172 616d 6574 6572 2066 6f72 2074   parameter for t
-00004460: 6865 2066 7265 7175 656e 6379 2075 6e64  he frequency und
-00004470: 6572 2063 6f6e 7369 6465 7261 7469 6f6e  er consideration
-00004480: 2028 6e6f 7420 7573 6564 290a 2020 2020   (not used).    
-00004490: 2020 2054 6865 2072 6f75 7469 6e65 2072     The routine r
-000044a0: 6574 7572 6e73 2074 6865 2065 6666 6563  eturns the effec
-000044b0: 7469 7665 2064 6965 6c65 6374 7269 6320  tive dielectric 
-000044c0: 636f 6e73 7461 6e74 2222 220a 2020 2020  constant""".    
-000044d0: 6566 6664 203d 2076 6620 2a20 6372 7973  effd = vf * crys
-000044e0: 7461 6c5f 7065 726d 6974 7469 7669 7479  tal_permittivity
-000044f0: 202b 2028 312e 302d 7666 2920 2a20 6469   + (1.0-vf) * di
-00004500: 656c 6563 7472 6963 5f6d 6564 6975 6d0a  electric_medium.
-00004510: 2020 2020 7472 6163 6520 3d20 6e70 2e74      trace = np.t
-00004520: 7261 6365 2865 6666 6429 202f 2033 2e30  race(effd) / 3.0
-00004530: 0a20 2020 2065 6666 6469 656c 6563 203d  .    effdielec =
-00004540: 206e 702e 6172 7261 7928 5b5b 7472 6163   np.array([[trac
-00004550: 652c 2030 2c20 305d 2c20 5b30 2c20 7472  e, 0, 0], [0, tr
-00004560: 6163 652c 2030 5d2c 205b 302c 2030 2c20  ace, 0], [0, 0, 
-00004570: 7472 6163 655d 5d29 0a20 2020 2072 6574  trace]]).    ret
-00004580: 7572 6e20 6566 6664 6965 6c65 630a 0a64  urn effdielec..d
-00004590: 6566 2062 616c 616e 2864 6965 6c65 6374  ef balan(dielect
-000045a0: 7269 635f 6d65 6469 756d 2c20 6372 7973  ric_medium, crys
-000045b0: 7461 6c5f 7065 726d 6974 7469 7669 7479  tal_permittivity
-000045c0: 2c20 7368 6170 652c 204c 2c20 7666 2c20  , shape, L, vf, 
-000045d0: 7369 7a65 293a 0a20 2020 2022 2222 4361  size):.    """Ca
-000045e0: 6c63 756c 6174 6520 7468 6520 6566 6665  lculate the effe
-000045f0: 6374 6976 6520 636f 6e73 7461 6e74 2070  ctive constant p
-00004600: 6572 6d69 7474 6976 6974 7920 7573 696e  ermittivity usin
-00004610: 6720 7468 6520 6d65 7468 6f64 206f 6620  g the method of 
-00004620: 6261 6c61 6e0a 2020 2020 2020 2064 6965  balan.       die
-00004630: 6c65 6374 7269 635f 6d65 6469 756d 2069  lectric_medium i
-00004640: 7320 7468 6520 6469 656c 6563 7472 6963  s the dielectric
-00004650: 2063 6f6e 7374 616e 7420 7465 6e73 6f72   constant tensor
-00004660: 206f 6620 7468 6520 6d65 6469 756d 0a20   of the medium. 
-00004670: 2020 2020 2020 6372 7973 7461 6c5f 7065        crystal_pe
-00004680: 726d 6974 7469 7669 7479 2069 7320 7468  rmittivity is th
-00004690: 6520 746f 7461 6c20 6672 6571 7565 6e63  e total frequenc
-000046a0: 7920 6469 656c 6563 7472 6963 2063 6f6e  y dielectric con
-000046b0: 7374 616e 7420 7465 6e73 6f72 2061 7420  stant tensor at 
-000046c0: 7468 6520 6375 7272 656e 7420 6672 6571  the current freq
-000046d0: 7565 6e63 790a 2020 2020 2020 2073 6861  uency.       sha
-000046e0: 7065 2069 7320 7468 6520 6e61 6d65 206f  pe is the name o
-000046f0: 6620 7468 6520 6375 7272 656e 7420 7368  f the current sh
-00004700: 6170 650a 2020 2020 2020 204c 2069 7320  ape.       L is 
-00004710: 7468 6520 7368 6170 6573 2064 6570 6f6c  the shapes depol
-00004720: 6172 6973 6174 696f 6e20 6d61 7472 6978  arisation matrix
-00004730: 0a20 2020 2020 2020 7369 7a65 2069 7320  .       size is 
-00004740: 7468 6520 6469 6d65 6e73 696f 6e6c 6573  the dimensionles
-00004750: 7320 7369 7a65 2070 6172 616d 6574 6572  s size parameter
-00004760: 2066 6f72 2074 6865 2066 7265 7175 656e   for the frequen
-00004770: 6379 2075 6e64 6572 2063 6f6e 7369 6465  cy under conside
-00004780: 7261 7469 6f6e 2028 6e6f 7420 7573 6564  ration (not used
-00004790: 290a 2020 2020 2020 2054 6865 2072 6f75  ).       The rou
-000047a0: 7469 6e65 2072 6574 7572 6e73 2074 6865  tine returns the
-000047b0: 2065 6666 6563 7469 7665 2064 6965 6c65   effective diele
-000047c0: 6374 7269 6320 636f 6e73 7461 6e74 2222  ctric constant""
-000047d0: 220a 2020 2020 756e 6974 203d 2069 6e69  ".    unit = ini
-000047e0: 7469 616c 6973 655f 756e 6974 5f74 656e  tialise_unit_ten
-000047f0: 736f 7228 290a 2020 2020 6469 656c 6563  sor().    dielec
-00004800: 766d 3120 3d20 2863 7279 7374 616c 5f70  vm1 = (crystal_p
-00004810: 6572 6d69 7474 6976 6974 7920 2d20 756e  ermittivity - un
-00004820: 6974 290a 2020 2020 6465 666f 726d 6174  it).    deformat
-00004830: 696f 6e20 203d 206e 702e 646f 7428 6469  ion  = np.dot(di
-00004840: 656c 6563 7472 6963 5f6d 6564 6975 6d2c  electric_medium,
-00004850: 206e 702e 6c69 6e61 6c67 2e69 6e76 2864   np.linalg.inv(d
-00004860: 6965 6c65 6374 7269 635f 6d65 6469 756d  ielectric_medium
-00004870: 202b 206e 702e 646f 7428 4c2c 2028 6372   + np.dot(L, (cr
-00004880: 7973 7461 6c5f 7065 726d 6974 7469 7669  ystal_permittivi
-00004890: 7479 202d 2064 6965 6c65 6374 7269 635f  ty - dielectric_
-000048a0: 6d65 6469 756d 2929 2929 0a20 2020 2065  medium)))).    e
-000048b0: 6666 6420 2020 2020 2020 2020 203d 2075  ffd          = u
-000048c0: 6e69 7420 2b20 6e70 2e64 6f74 2864 6566  nit + np.dot(def
-000048d0: 6f72 6d61 7469 6f6e 2c20 6469 656c 6563  ormation, dielec
-000048e0: 766d 3129 0a20 2020 2074 7261 6365 203d  vm1).    trace =
-000048f0: 2076 6620 2a20 6e70 2e74 7261 6365 2865   vf * np.trace(e
-00004900: 6666 6429 202f 2033 2e30 0a20 2020 2065  ffd) / 3.0.    e
-00004910: 6666 6469 656c 6563 203d 206e 702e 6172  ffdielec = np.ar
-00004920: 7261 7928 5b5b 7472 6163 652c 2030 2c20  ray([[trace, 0, 
-00004930: 305d 2c20 5b30 2c20 7472 6163 652c 2030  0], [0, trace, 0
-00004940: 5d2c 205b 302c 2030 2c20 7472 6163 655d  ], [0, 0, trace]
-00004950: 5d29 0a20 2020 2072 6574 7572 6e20 6566  ]).    return ef
-00004960: 6664 6965 6c65 630a 0a64 6566 2073 7068  fdielec..def sph
-00004970: 6572 6963 616c 5f61 7665 7261 6765 645f  erical_averaged_
-00004980: 6d69 655f 7363 6174 7465 7269 6e67 2864  mie_scattering(d
-00004990: 6965 6c65 6374 7269 635f 6d65 6469 756d  ielectric_medium
-000049a0: 2c20 6372 7973 7461 6c5f 7065 726d 6974  , crystal_permit
-000049b0: 7469 7669 7479 2c20 7368 6170 652c 204c  tivity, shape, L
-000049c0: 2c20 7666 2c20 7369 7a65 2c20 7369 7a65  , vf, size, size
-000049d0: 5f6d 752c 2073 697a 655f 6469 7374 7269  _mu, size_distri
-000049e0: 6275 7469 6f6e 5f73 6967 6d61 293a 0a20  bution_sigma):. 
-000049f0: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
-00004a00: 7468 6520 6566 6665 6374 6976 6520 636f  the effective co
-00004a10: 6e73 7461 6e74 2070 6572 6d69 7474 6976  nstant permittiv
-00004a20: 6974 7920 7573 696e 6720 6120 4d69 6520  ity using a Mie 
-00004a30: 7363 6174 7465 7269 6e67 2061 7070 726f  scattering appro
-00004a40: 6163 680a 2020 2020 2020 2064 6965 6c65  ach.       diele
-00004a50: 6374 7269 635f 6d65 6469 756d 2069 7320  ctric_medium is 
-00004a60: 7468 6520 6469 656c 6563 7472 6963 2063  the dielectric c
-00004a70: 6f6e 7374 616e 7420 7465 6e73 6f72 206f  onstant tensor o
-00004a80: 6620 7468 6520 6d65 6469 756d 0a20 2020  f the medium.   
-00004a90: 2020 2020 6372 7973 7461 6c5f 7065 726d      crystal_perm
-00004aa0: 6974 7469 7669 7479 2069 7320 7468 6520  ittivity is the 
-00004ab0: 746f 7461 6c20 6672 6571 7565 6e63 7920  total frequency 
-00004ac0: 6469 656c 6563 7472 6963 2063 6f6e 7374  dielectric const
-00004ad0: 616e 7420 7465 6e73 6f72 2061 7420 7468  ant tensor at th
-00004ae0: 6520 6375 7272 656e 7420 6672 6571 7565  e current freque
-00004af0: 6e63 790a 2020 2020 2020 2073 6861 7065  ncy.       shape
-00004b00: 2069 7320 7468 6520 6e61 6d65 206f 6620   is the name of 
-00004b10: 7468 6520 6375 7272 656e 7420 7368 6170  the current shap
-00004b20: 6520 284e 4f54 2055 5345 4429 0a20 2020  e (NOT USED).   
-00004b30: 2020 2020 4c20 6973 2074 6865 2073 6861      L is the sha
-00004b40: 7065 7320 6465 706f 6c61 7269 7361 7469  pes depolarisati
-00004b50: 6f6e 206d 6174 7269 7820 284e 4f54 2055  on matrix (NOT U
-00004b60: 5345 4429 0a20 2020 2020 2020 7369 7a65  SED).       size
-00004b70: 2069 7320 7468 6520 6469 6d65 6e73 696f   is the dimensio
-00004b80: 6e6c 6573 7320 7369 7a65 2070 6172 616d  nless size param
-00004b90: 6574 6572 2066 6f72 2074 6865 2066 7265  eter for the fre
-00004ba0: 7175 656e 6379 2075 6e64 6572 2063 6f6e  quency under con
-00004bb0: 7369 6465 7261 7469 6f6e 0a20 2020 2020  sideration.     
-00004bc0: 2020 7369 7a65 5f64 6973 7472 6962 7574    size_distribut
-00004bd0: 696f 6e5f 7369 676d 6120 6973 2074 6865  ion_sigma is the
-00004be0: 206c 6f67 206e 6f72 6d61 6c20 7661 6c75   log normal valu
-00004bf0: 6520 6f66 2073 6967 6d61 0a20 2020 2020  e of sigma.     
-00004c00: 2020 7666 2069 7320 7468 6520 766f 6c75    vf is the volu
-00004c10: 6d65 2066 7261 6374 696f 6e20 6f66 2066  me fraction of f
-00004c20: 696c 6c65 720a 2020 2020 2020 204d 6965  iller.       Mie
-00004c30: 206f 6e6c 7920 776f 726b 7320 666f 7220   only works for 
-00004c40: 7370 6865 7269 6361 6c20 7061 7274 6963  spherical partic
-00004c50: 6c65 732c 2073 6f20 7368 6170 652c 2061  les, so shape, a
-00004c60: 6e64 204c 2070 6172 616d 6574 6572 7320  nd L parameters 
-00004c70: 6172 6520 6967 6e6f 7265 640a 2020 2020  are ignored.    
-00004c80: 2020 2054 6865 2061 6e69 736f 7472 6f70     The anisotrop
-00004c90: 7920 6f66 2074 6865 2070 6572 6d69 7474  y of the permitt
-00004ca0: 6976 6974 7920 6973 2061 6363 6f75 6e74  ivity is account
-00004cb0: 6564 2066 6f72 2062 7920 7361 6d70 6c69  ed for by sampli
-00004cc0: 6e67 206d 616e 7920 6469 7265 6374 696f  ng many directio
-00004cd0: 6e73 0a20 2020 2020 2020 616e 6420 6361  ns.       and ca
-00004ce0: 6c63 756c 6174 696e 6720 7468 6520 7363  lculating the sc
-00004cf0: 6174 7465 7269 6e67 2069 6e20 6561 6368  attering in each
-00004d00: 2064 6972 6563 7469 6f6e 0a20 2020 2020   direction.     
-00004d10: 2020 5468 6520 726f 7574 696e 6520 7265    The routine re
-00004d20: 7475 726e 7320 7468 6520 6566 6665 6374  turns the effect
-00004d30: 6976 6520 6469 656c 6563 7472 6963 2063  ive dielectric c
-00004d40: 6f6e 7374 616e 7422 2222 0a20 2020 2067  onstant""".    g
-00004d50: 6c6f 6261 6c20 706f 696e 7473 5f6f 6e5f  lobal points_on_
-00004d60: 7370 6865 7265 0a20 2020 2023 2064 6566  sphere.    # def
-00004d70: 696e 6520 6920 6173 2061 2063 6f6d 706c  ine i as a compl
-00004d80: 6578 206e 756d 6265 720a 2020 2020 6920  ex number.    i 
-00004d90: 3d20 636f 6d70 6c65 7828 302c 3129 0a20  = complex(0,1). 
-00004da0: 2020 2023 2057 6520 6e65 6564 2074 6f20     # We need to 
-00004db0: 7461 6b65 6e20 6163 636f 756e 7420 6f66  taken account of
-00004dc0: 2074 6865 2063 6861 6e67 6520 696e 2077   the change in w
-00004dd0: 6176 656c 656e 6774 6820 616e 6420 7468  avelength and th
-00004de0: 6520 6368 616e 6765 2069 6e20 7369 7a65  e change in size
-00004df0: 2070 6172 616d 6574 6572 2064 7565 2074   parameter due t
-00004e00: 6f20 7468 650a 2020 2020 2320 4e6f 6e65  o the.    # None
-00004e10: 2075 6e69 7420 7661 6c75 6520 6f66 2074   unit value of t
-00004e20: 6865 2064 6965 6c65 6374 7269 6320 6f66  he dielectric of
-00004e30: 2074 6865 2065 6d62 6564 6469 6e67 206d   the embedding m
-00004e40: 6564 6975 6d0a 2020 2020 2320 5468 6520  edium.    # The 
-00004e50: 7369 7a65 2070 6172 616d 6574 6572 2069  size parameter i
-00004e60: 7320 3270 6920 7220 2f20 6c61 6d62 6461  s 2pi r / lambda
-00004e70: 0a20 2020 2023 2054 6865 2065 6666 6563  .    # The effec
-00004e80: 7469 7665 206c 616d 6264 6120 696e 2074  tive lambda in t
-00004e90: 6865 2073 7570 706f 7274 696e 6720 6d65  he supporting me
-00004ea0: 6469 756d 2069 7320 6c61 6d62 6461 202f  dium is lambda /
-00004eb0: 2073 7172 7428 656d 6564 6975 6d29 0a20   sqrt(emedium). 
-00004ec0: 2020 2023 2057 6865 7265 2074 6865 2072     # Where the r
-00004ed0: 6566 7261 6374 6976 6520 696e 6465 7820  efractive index 
-00004ee0: 6973 2074 616b 656e 2074 6f20 6265 2073  is taken to be s
-00004ef0: 7172 7428 656d 6564 6975 6d29 2028 6e6f  qrt(emedium) (no
-00004f00: 6e20 6d61 676e 6574 6963 206d 6174 6572  n magnetic mater
-00004f10: 6961 6c73 290a 2020 2020 656d 6564 6975  ials).    emediu
-00004f20: 6d20 3d20 6e70 2e74 7261 6365 2864 6965  m = np.trace(die
-00004f30: 6c65 6374 7269 635f 6d65 6469 756d 2920  lectric_medium) 
-00004f40: 2f20 332e 300a 2020 2020 7265 6672 6163  / 3.0.    refrac
-00004f50: 7469 7665 5f69 6e64 6578 5f6d 6564 6975  tive_index_mediu
-00004f60: 6d20 3d20 6e70 2e72 6561 6c28 6e70 2e73  m = np.real(np.s
-00004f70: 7172 7428 656d 6564 6975 6d29 290a 2020  qrt(emedium)).  
-00004f80: 2020 6c61 6d62 6461 5f76 6163 7575 6d5f    lambda_vacuum_
-00004f90: 6d75 203d 2032 202a 2050 4920 2a20 7369  mu = 2 * PI * si
-00004fa0: 7a65 5f6d 7520 2f20 7369 7a65 0a20 2020  ze_mu / size.   
-00004fb0: 2077 6176 656c 656e 6774 685f 6e6d 203d   wavelength_nm =
-00004fc0: 206c 616d 6264 615f 7661 6375 756d 5f6d   lambda_vacuum_m
-00004fd0: 7520 2a20 3130 3030 202f 2072 6566 7261  u * 1000 / refra
-00004fe0: 6374 6976 655f 696e 6465 785f 6d65 6469  ctive_index_medi
-00004ff0: 756d 0a20 2020 2072 6164 6975 735f 6e6d  um.    radius_nm
-00005000: 203d 2073 697a 655f 6d75 202a 2031 3030   = size_mu * 100
-00005010: 300a 2020 2020 2320 5468 6520 7761 7665  0.    # The wave
-00005020: 7665 6374 6f72 2069 6e20 6e6d 2d31 0a20  vector in nm-1. 
-00005030: 2020 206b 5f6e 6d20 3d20 3220 2a20 5049     k_nm = 2 * PI
-00005040: 202f 2077 6176 656c 656e 6774 685f 6e6d   / wavelength_nm
-00005050: 0a20 2020 2023 2076 6f6c 756d 6520 6f66  .    # volume of
-00005060: 2061 2070 6172 7469 636c 6520 696e 206e   a particle in n
-00005070: 6d5e 330a 2020 2020 565f 6e6d 203d 2034  m^3.    V_nm = 4
-00005080: 2e30 2f33 2e30 202a 2050 4920 2a20 7261  .0/3.0 * PI * ra
-00005090: 6469 7573 5f6e 6d20 2a20 7261 6469 7573  dius_nm * radius
-000050a0: 5f6e 6d20 2a20 7261 6469 7573 5f6e 6d0a  _nm * radius_nm.
-000050b0: 2020 2020 2320 4e75 6d62 6572 2064 656e      # Number den
-000050c0: 7369 7479 206f 6620 7061 7274 6963 6c65  sity of particle
-000050d0: 7320 286e 756d 6265 7220 2f20 6e6d 5e33  s (number / nm^3
-000050e0: 290a 2020 2020 4e5f 6e6d 203d 2076 6620  ).    N_nm = vf 
-000050f0: 2f20 565f 6e6d 0a20 2020 2023 2049 6620  / V_nm.    # If 
-00005100: 7468 6572 6520 6973 2061 2073 697a 6520  there is a size 
-00005110: 6469 7374 7269 6275 7469 6f6e 2073 6574  distribution set
-00005120: 2075 7020 746f 2075 7365 2069 740a 2020   up to use it.  
-00005130: 2020 6966 2073 697a 655f 6469 7374 7269    if size_distri
-00005140: 6275 7469 6f6e 5f73 6967 6d61 3a0a 2020  bution_sigma:.  
-00005150: 2020 2020 2020 6c6f 7765 722c 7570 7065        lower,uppe
-00005160: 7220 3d20 6c6f 676e 6f72 6d2e 696e 7465  r = lognorm.inte
-00005170: 7276 616c 2830 2e39 3939 392c 7369 7a65  rval(0.9999,size
-00005180: 5f64 6973 7472 6962 7574 696f 6e5f 7369  _distribution_si
-00005190: 676d 612c 7363 616c 653d 7369 7a65 5f6d  gma,scale=size_m
-000051a0: 7529 0a20 2020 2020 2020 206e 756d 6265  u).        numbe
-000051b0: 724f 6642 696e 7320 3d20 3430 0a20 2020  rOfBins = 40.   
-000051c0: 2020 2020 2064 7020 3d20 6e70 2e6c 6f67       dp = np.log
-000051d0: 7370 6163 6528 6e70 2e6c 6f67 286c 6f77  space(np.log(low
-000051e0: 6572 292c 6e70 2e6c 6f67 2875 7070 6572  er),np.log(upper
-000051f0: 292c 6e75 6d62 6572 4f66 4269 6e73 2c62  ),numberOfBins,b
-00005200: 6173 653d 6e70 2e65 290a 2020 2020 2020  ase=np.e).      
-00005210: 2020 2320 5468 6520 6465 6669 6e69 7469    # The definiti
-00005220: 6f6e 7320 7573 6564 2061 7265 2063 6f6e  ons used are con
-00005230: 6675 7369 6e67 3b0a 2020 2020 2020 2020  fusing;.        
-00005240: 2320 6470 2069 7320 7468 6520 6c6f 6720  # dp is the log 
-00005250: 6f66 2074 6865 2076 6172 6961 626c 650a  of the variable.
-00005260: 2020 2020 2020 2020 2320 7320 6973 2074          # s is t
-00005270: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
-00005280: 6174 696f 6e20 2873 6861 7065 2066 756e  ation (shape fun
-00005290: 6374 696f 6e29 206f 6620 7468 6520 6c6f  ction) of the lo
-000052a0: 6720 6f66 2074 6865 2076 6172 6961 7465  g of the variate
-000052b0: 0a20 2020 2020 2020 2023 2073 6361 6c65  .        # scale
-000052c0: 2069 7320 7468 6520 6d65 616e 206f 6620   is the mean of 
-000052d0: 7468 6520 756e 6465 726c 7969 6e67 206e  the underlying n
-000052e0: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
-000052f0: 6f6e 0a20 2020 2020 2020 206e 6470 203d  on.        ndp =
-00005300: 206c 6f67 6e6f 726d 2e70 6466 2864 702c   lognorm.pdf(dp,
-00005310: 733d 7369 7a65 5f64 6973 7472 6962 7574  s=size_distribut
-00005320: 696f 6e5f 7369 676d 612c 7363 616c 653d  ion_sigma,scale=
-00005330: 7369 7a65 5f6d 7529 0a20 2020 2020 2020  size_mu).       
-00005340: 2023 7072 696e 7428 2244 5022 2c64 7029   #print("DP",dp)
-00005350: 0a20 2020 2020 2020 2023 7072 696e 7428  .        #print(
-00005360: 224e 4450 222c 6e64 7029 0a20 2020 2020  "NDP",ndp).     
-00005370: 2020 2023 7072 696e 7428 2255 7070 6572     #print("Upper
-00005380: 206c 6f77 6572 222c 6c6f 7765 722c 7570   lower",lower,up
-00005390: 7065 7229 0a20 2020 2020 2020 2023 7072  per).        #pr
-000053a0: 696e 7428 2253 697a 655f 4d55 222c 7369  int("Size_MU",si
-000053b0: 7a65 5f6d 7529 0a20 2020 2023 2043 616c  ze_mu).    # Cal
-000053c0: 6375 6c61 7465 2074 6865 2073 616d 706c  culate the sampl
-000053d0: 696e 6720 706f 696e 7473 206f 6e20 6120  ing points on a 
-000053e0: 6669 626f 6e61 6363 6920 7370 6865 7265  fibonacci sphere
-000053f0: 0a20 2020 2069 6620 706f 696e 7473 5f6f  .    if points_o
-00005400: 6e5f 7370 6865 7265 203d 3d20 4e6f 6e65  n_sphere == None
-00005410: 3a0a 2020 2020 2020 2020 706f 696e 7473  :.        points
-00005420: 5f6f 6e5f 7370 6865 7265 203d 2066 6962  _on_sphere = fib
-00005430: 6f6e 6163 6369 5f73 7068 6572 6528 7361  onacci_sphere(sa
-00005440: 6d70 6c65 733d 3530 302c 7261 6e64 6f6d  mples=500,random
-00005450: 697a 653d 5472 7565 290a 2020 2020 7472  ize=True).    tr
-00005460: 6163 6520 3d20 302e 300a 2020 2020 2320  ace = 0.0.    # 
-00005470: 4e6f 7720 7461 6b65 2074 6865 2061 7665  Now take the ave
-00005480: 7261 6765 206f 6620 6561 6368 2064 6972  rage of each dir
-00005490: 6563 7469 6f6e 206f 6e20 7468 6520 7370  ection on the sp
-000054a0: 6865 7265 0a20 2020 2066 6f72 2070 6f69  here.    for poi
-000054b0: 6e74 2069 6e20 706f 696e 7473 5f6f 6e5f  nt in points_on_
-000054c0: 7370 6865 7265 3a0a 2020 2020 2020 2020  sphere:.        
-000054d0: 706f 696e 7420 3d20 6e70 2e61 7272 6179  point = np.array
-000054e0: 2870 6f69 6e74 290a 2020 2020 2020 2020  (point).        
-000054f0: 726f 7461 7465 645f 6469 656c 6563 203d  rotated_dielec =
-00005500: 206e 702e 646f 7428 706f 696e 742c 206e   np.dot(point, n
-00005510: 702e 646f 7428 706f 696e 742c 2063 7279  p.dot(point, cry
-00005520: 7374 616c 5f70 6572 6d69 7474 6976 6974  stal_permittivit
-00005530: 7929 290a 2020 2020 2020 2020 7265 6672  y)).        refr
-00005540: 6163 7469 7665 5f69 6e64 6578 203d 2063  active_index = c
-00005550: 616c 6375 6c61 7465 5f72 6566 7261 6374  alculate_refract
-00005560: 6976 655f 696e 6465 785f 7363 616c 6172  ive_index_scalar
-00005570: 2872 6f74 6174 6564 5f64 6965 6c65 6329  (rotated_dielec)
-00005580: 202f 2072 6566 7261 6374 6976 655f 696e   / refractive_in
-00005590: 6465 785f 6d65 6469 756d 0a20 2020 2020  dex_medium.     
-000055a0: 2020 2023 2070 7269 6e74 2827 7265 6672     # print('refr
-000055b0: 6163 7469 7665 5f69 6e64 6578 272c 2072  active_index', r
-000055c0: 6566 7261 6374 6976 655f 696e 6465 7829  efractive_index)
-000055d0: 0a20 2020 2020 2020 2023 2070 7269 6e74  .        # print
-000055e0: 2827 7265 6672 6163 7469 7665 5f69 6e64  ('refractive_ind
-000055f0: 6578 5f6d 6564 6975 6d27 2c20 7265 6672  ex_medium', refr
-00005600: 6163 7469 7665 5f69 6e64 6578 5f6d 6564  active_index_med
-00005610: 6975 6d29 0a20 2020 2020 2020 2023 2070  ium).        # p
-00005620: 7269 6e74 2827 726f 7461 7465 645f 6469  rint('rotated_di
-00005630: 656c 6563 272c 2072 6f74 6174 6564 5f64  elec', rotated_d
-00005640: 6965 6c65 6329 0a20 2020 2020 2020 2069  ielec).        i
-00005650: 6620 7369 7a65 5f64 6973 7472 6962 7574  f size_distribut
-00005660: 696f 6e5f 7369 676d 613a 0a20 2020 2020  ion_sigma:.     
-00005670: 2020 2020 2020 2023 2043 616c 6375 6c61         # Calcula
-00005680: 7465 2074 6865 2069 6e74 6567 7261 6c20  te the integral 
-00005690: 6f66 2074 6865 2066 6f72 7761 7264 2073  of the forward s
-000056a0: 6361 7474 6572 696e 6720 6661 6374 6f72  cattering factor
-000056b0: 7320 6f76 6572 2074 6865 2064 6973 7472  s over the distr
-000056c0: 6962 7574 696f 6e0a 2020 2020 2020 2020  ibution.        
-000056d0: 2020 2020 7331 5f66 6163 746f 7273 203d      s1_factors =
-000056e0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-000056f0: 666f 7220 7220 696e 2064 703a 0a20 2020  for r in dp:.   
-00005700: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-00005710: 6865 2073 697a 6520 7061 7261 6d65 7465  he size paramete
-00005720: 7220 6973 2032 7069 2072 202f 206c 616d  r is 2pi r / lam
-00005730: 6264 610a 2020 2020 2020 2020 2020 2020  bda.            
-00005740: 2020 2020 7820 3d20 3220 2a20 5049 202a      x = 2 * PI *
-00005750: 2072 202f 206c 616d 6264 615f 7661 6375   r / lambda_vacu
-00005760: 756d 5f6d 750a 2020 2020 2020 2020 2020  um_mu.          
-00005770: 2020 2020 2020 2320 4361 6c63 756c 6174        # Calculat
-00005780: 6520 7468 6520 5331 2061 6e64 2053 3220  e the S1 and S2 
-00005790: 7363 6174 7465 7269 6e67 2066 6163 746f  scattering facto
-000057a0: 7273 2c20 616e 6420 7374 6f72 6520 696e  rs, and store in
-000057b0: 2061 206c 6973 740a 2020 2020 2020 2020   a list.        
-000057c0: 2020 2020 2020 2020 7331 2c73 3220 3d20          s1,s2 = 
-000057d0: 4d69 652e 4d69 6553 3153 3228 7265 6672  Mie.MieS1S2(refr
-000057e0: 6163 7469 7665 5f69 6e64 6578 2c20 782a  active_index, x*
-000057f0: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
-00005800: 5f6d 6564 6975 6d2c 2031 290a 2020 2020  _medium, 1).    
-00005810: 2020 2020 2020 2020 2020 2020 7331 5f66              s1_f
-00005820: 6163 746f 7273 2e61 7070 656e 6428 7331  actors.append(s1
-00005830: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00005840: 4e6f 7720 696e 7465 6772 6174 650a 2020  Now integrate.  
-00005850: 2020 2020 2020 2020 2020 7331 203d 2074            s1 = t
-00005860: 7261 707a 2873 315f 6661 6374 6f72 732a  rapz(s1_factors*
-00005870: 6e64 702c 6470 290a 2020 2020 2020 2020  ndp,dp).        
-00005880: 2020 2020 6e6f 726d 616c 203d 2074 7261      normal = tra
-00005890: 707a 286e 6470 2c64 7029 0a20 2020 2020  pz(ndp,dp).     
-000058a0: 2020 2020 2020 2023 6d65 616e 203d 2074         #mean = t
-000058b0: 7261 707a 286e 6470 2a64 702c 6470 290a  rapz(ndp*dp,dp).
-000058c0: 2020 2020 2020 2020 2020 2020 2374 7275              #tru
-000058d0: 655f 6d65 616e 203d 206e 702e 6578 7028  e_mean = np.exp(
-000058e0: 206e 702e 6c6f 6728 7369 7a65 5f6d 7529   np.log(size_mu)
-000058f0: 202b 2073 697a 655f 6469 7374 7269 6275   + size_distribu
-00005900: 7469 6f6e 5f73 6967 6d61 2a73 697a 655f  tion_sigma*size_
-00005910: 6469 7374 7269 6275 7469 6f6e 5f73 6967  distribution_sig
-00005920: 6d61 2f32 2e30 290a 2020 2020 2020 2020  ma/2.0).        
-00005930: 2020 2020 2376 5f63 6d31 203d 2031 2e30      #v_cm1 = 1.0
-00005940: 4534 2f6c 616d 6264 615f 7661 6375 756d  E4/lambda_vacuum
-00005950: 5f6d 750a 2020 2020 2020 2020 2020 2020  _mu.            
-00005960: 2370 7269 6e74 2822 4672 6571 7565 6e63  #print("Frequenc
-00005970: 792c 6e6f 726d 616c 2c6d 6561 6e22 2c76  y,normal,mean",v
-00005980: 5f63 6d31 2c6e 6f72 6d61 6c2c 7472 7565  _cm1,normal,true
-00005990: 5f6d 6561 6e2c 6d65 616e 290a 2020 2020  _mean,mean).    
-000059a0: 2020 2020 2020 2020 6966 206e 702e 6162          if np.ab
-000059b0: 7328 6e6f 726d 616c 202d 2031 2e30 2920  s(normal - 1.0) 
-000059c0: 3e20 312e 3045 2d32 3a0a 2020 2020 2020  > 1.0E-2:.      
-000059d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000059e0: 2257 6172 6e69 6e67 2069 6e74 6567 7261  "Warning integra
-000059f0: 7469 6f6e 206f 6620 6c6f 672d 6e6f 726d  tion of log-norm
-00005a00: 616c 2064 6973 7472 6962 7574 696f 6e20  al distribution 
-00005a10: 696e 2065 7272 6f72 222c 206e 6f72 6d61  in error", norma
-00005a20: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
-00005a30: 2020 2070 7269 6e74 2822 5374 6f70 7069     print("Stoppi
-00005a40: 6e67 2063 616c 6375 6c61 7469 6f6e 202d  ng calculation -
-00005a50: 206c 696b 656c 7920 7072 6f62 6c65 6d20   likely problem 
-00005a60: 6973 2074 6f6f 206c 6172 6765 2061 2073  is too large a s
-00005a70: 6967 6d61 2066 6f72 206c 6f67 2d6e 6f72  igma for log-nor
-00005a80: 6d61 6c20 6469 7374 7269 6275 7469 6f6e  mal distribution
-00005a90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00005aa0: 2020 2065 6666 6469 656c 6563 203d 206e     effdielec = n
-00005ab0: 702e 6172 7261 7928 5b5b 312c 2030 2c20  p.array([[1, 0, 
-00005ac0: 305d 2c20 5b30 2c20 312c 2030 5d2c 205b  0], [0, 1, 0], [
-00005ad0: 302c 2030 2c20 315d 5d29 0a20 2020 2020  0, 0, 1]]).     
-00005ae0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00005af0: 6e20 6566 6664 6965 6c65 630a 2020 2020  n effdielec.    
-00005b00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00005b10: 2020 2020 2020 2320 4361 6c63 756c 6174        # Calculat
-00005b20: 6520 7468 6520 7363 6174 7465 7269 6e67  e the scattering
-00005b30: 2066 6163 746f 7273 2061 7420 3020 6465   factors at 0 de
-00005b40: 6772 6565 730a 2020 2020 2020 2020 2020  grees.          
-00005b50: 2020 236a 6b20 7072 696e 7428 2272 6566    #jk print("ref
-00005b60: 7261 6374 6976 655f 696e 6465 782c 2073  ractive_index, s
-00005b70: 697a 652c 2072 6566 7261 6374 6976 655f  ize, refractive_
-00005b80: 696e 6465 785f 6d65 6469 756d 222c 2072  index_medium", r
-00005b90: 6566 7261 6374 6976 655f 696e 6465 782c  efractive_index,
-00005ba0: 2073 697a 652c 2072 6566 7261 6374 6976   size, refractiv
-00005bb0: 655f 696e 6465 785f 6d65 6469 756d 290a  e_index_medium).
-00005bc0: 2020 2020 2020 2020 2020 2020 7331 2c73              s1,s
-00005bd0: 3220 3d20 4d69 652e 4d69 6553 3153 3228  2 = Mie.MieS1S2(
-00005be0: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
-00005bf0: 2c20 7369 7a65 2a72 6566 7261 6374 6976  , size*refractiv
-00005c00: 655f 696e 6465 785f 6d65 6469 756d 2c20  e_index_medium, 
-00005c10: 3129 0a20 2020 2020 2020 2023 2053 6565  1).        # See
-00005c20: 2076 616e 2064 6520 4875 6c73 7420 7061   van de Hulst pa
-00005c30: 6765 2031 3239 2c20 3133 300a 2020 2020  ge 129, 130.    
-00005c40: 2020 2020 2320 5265 6672 6163 7469 7665      # Refractive
-00005c50: 2069 6e64 6578 206f 6620 6d61 7465 7269   index of materi
-00005c60: 616c 2069 730a 2020 2020 2020 2020 2320  al is.        # 
-00005c70: 7468 6520 7369 676e 206f 6620 7468 6520  the sign of the 
-00005c80: 696d 6167 696e 6172 7920 636f 6d70 6f6e  imaginary compon
-00005c90: 656e 7420 6861 7320 6368 616e 6765 6420  ent has changed 
-00005ca0: 666f 7220 636f 6d70 6174 6962 696c 6974  for compatibilit
-00005cb0: 7920 7769 7468 204d 472f 4272 7567 6765  y with MG/Brugge
-00005cc0: 6d61 6e0a 2020 2020 2020 2020 7265 6672  man.        refr
-00005cd0: 6163 7469 7665 5f69 6e64 6578 203d 2072  active_index = r
-00005ce0: 6566 7261 6374 6976 655f 696e 6465 785f  efractive_index_
-00005cf0: 6d65 6469 756d 202a 2028 2031 2e30 202b  medium * ( 1.0 +
-00005d00: 2069 202a 2073 3120 2a20 3220 2a20 5049   i * s1 * 2 * PI
-00005d10: 202a 204e 5f6e 6d20 2f20 2820 6b5f 6e6d   * N_nm / ( k_nm
-00005d20: 202a 206b 5f6e 6d20 2a20 6b5f 6e6d 2029   * k_nm * k_nm )
-00005d30: 2029 0a20 2020 2020 2020 2074 7261 6365   ).        trace
-00005d40: 202b 3d20 7265 6672 6163 7469 7665 5f69   += refractive_i
-00005d50: 6e64 6578 0a20 2020 2023 2072 6574 7572  ndex.    # retur
-00005d60: 6e20 616e 2069 736f 7472 6f70 6963 2074  n an isotropic t
-00005d70: 656e 736f 720a 2020 2020 7472 6163 6520  ensor.    trace 
-00005d80: 3d20 7472 6163 6520 2f20 6c65 6e28 706f  = trace / len(po
-00005d90: 696e 7473 5f6f 6e5f 7370 6865 7265 290a  ints_on_sphere).
-00005da0: 2020 2020 6566 6620 3d20 7472 6163 6520      eff = trace 
-00005db0: 2a20 7472 6163 650a 2020 2020 6566 6664  * trace.    effd
-00005dc0: 6965 6c65 6320 3d20 6e70 2e61 7272 6179  ielec = np.array
-00005dd0: 285b 5b65 6666 2c20 302c 2030 5d2c 205b  ([[eff, 0, 0], [
-00005de0: 302c 2065 6666 2c20 305d 2c20 5b30 2c20  0, eff, 0], [0, 
-00005df0: 302c 2065 6666 5d5d 290a 2020 2020 236a  0, eff]]).    #j
-00005e00: 6b20 7072 696e 7428 7261 6469 7573 5f6e  k print(radius_n
-00005e10: 6d2c 206c 616d 6264 615f 7661 6375 756d  m, lambda_vacuum
-00005e20: 5f6d 752a 3130 3030 2e30 2c20 7165 7874  _mu*1000.0, qext
-00005e30: 2c71 7363 612c 7161 6273 2c67 2c71 7072  ,qsca,qabs,g,qpr
-00005e40: 2c71 6261 636b 2c71 7261 7469 6f2c 6e70  ,qback,qratio,np
-00005e50: 2e72 6561 6c28 7331 292c 6e70 2e69 6d61  .real(s1),np.ima
-00005e60: 6728 7331 292c 6e70 2e72 6561 6c28 7472  g(s1),np.real(tr
-00005e70: 6163 6529 2c6e 702e 696d 6167 2874 7261  ace),np.imag(tra
-00005e80: 6365 292c 6e70 2e72 6561 6c28 6566 6629  ce),np.real(eff)
-00005e90: 2c6e 702e 696d 6167 2865 6666 2929 0a20  ,np.imag(eff)). 
-00005ea0: 2020 2023 7072 696e 7420 2822 7261 6469     #print ("radi
-00005eb0: 7573 5f6e 6d2c 2065 6666 222c 2072 6164  us_nm, eff", rad
-00005ec0: 6975 735f 6e6d 2c20 6566 6629 0a20 2020  ius_nm, eff).   
-00005ed0: 2072 6574 7572 6e20 6566 6664 6965 6c65   return effdiele
-00005ee0: 630a 0a0a 6465 6620 6d69 655f 7363 6174  c...def mie_scat
-00005ef0: 7465 7269 6e67 2864 6965 6c65 6374 7269  tering(dielectri
-00005f00: 635f 6d65 6469 756d 2c20 6372 7973 7461  c_medium, crysta
-00005f10: 6c5f 7065 726d 6974 7469 7669 7479 2c20  l_permittivity, 
-00005f20: 7368 6170 652c 204c 2c20 7666 2c20 7369  shape, L, vf, si
-00005f30: 7a65 2c20 7369 7a65 5f6d 752c 2073 697a  ze, size_mu, siz
-00005f40: 655f 6469 7374 7269 6275 7469 6f6e 5f73  e_distribution_s
-00005f50: 6967 6d61 293a 0a20 2020 2022 2222 4361  igma):.    """Ca
-00005f60: 6c63 756c 6174 6520 7468 6520 6566 6665  lculate the effe
-00005f70: 6374 6976 6520 636f 6e73 7461 6e74 2070  ctive constant p
-00005f80: 6572 6d69 7474 6976 6974 7920 7573 696e  ermittivity usin
-00005f90: 6720 6120 4d69 6520 7363 6174 7465 7269  g a Mie scatteri
-00005fa0: 6e67 2061 7070 726f 6163 680a 2020 2020  ng approach.    
-00005fb0: 2020 2064 6965 6c65 6374 7269 635f 6d65     dielectric_me
-00005fc0: 6469 756d 2069 7320 7468 6520 6469 656c  dium is the diel
-00005fd0: 6563 7472 6963 2063 6f6e 7374 616e 7420  ectric constant 
-00005fe0: 7465 6e73 6f72 206f 6620 7468 6520 6d65  tensor of the me
-00005ff0: 6469 756d 0a20 2020 2020 2020 6372 7973  dium.       crys
-00006000: 7461 6c5f 7065 726d 6974 7469 7669 7479  tal_permittivity
-00006010: 2069 7320 7468 6520 746f 7461 6c20 6672   is the total fr
-00006020: 6571 7565 6e63 7920 6469 656c 6563 7472  equency dielectr
-00006030: 6963 2063 6f6e 7374 616e 7420 7465 6e73  ic constant tens
-00006040: 6f72 2061 7420 7468 6520 6375 7272 656e  or at the curren
-00006050: 7420 6672 6571 7565 6e63 790a 2020 2020  t frequency.    
-00006060: 2020 2073 6861 7065 2069 7320 7468 6520     shape is the 
-00006070: 6e61 6d65 206f 6620 7468 6520 6375 7272  name of the curr
-00006080: 656e 7420 7368 6170 6520 284e 4f54 2055  ent shape (NOT U
-00006090: 5345 4429 0a20 2020 2020 2020 4c20 6973  SED).       L is
-000060a0: 2074 6865 2073 6861 7065 7320 6465 706f   the shapes depo
-000060b0: 6c61 7269 7361 7469 6f6e 206d 6174 7269  larisation matri
-000060c0: 7820 284e 4f54 2055 5345 4429 0a20 2020  x (NOT USED).   
-000060d0: 2020 2020 7369 7a65 2069 7320 7468 6520      size is the 
-000060e0: 6469 6d65 6e73 696f 6e6c 6573 7320 7369  dimensionless si
-000060f0: 7a65 2070 6172 616d 6574 6572 2066 6f72  ze parameter for
-00006100: 2074 6865 2066 7265 7175 656e 6379 2075   the frequency u
-00006110: 6e64 6572 2063 6f6e 7369 6465 7261 7469  nder considerati
-00006120: 6f6e 0a20 2020 2020 2020 7369 7a65 5f64  on.       size_d
-00006130: 6973 7472 6962 7574 696f 6e5f 7369 676d  istribution_sigm
-00006140: 6120 6973 2074 6865 206c 6f67 206e 6f72  a is the log nor
-00006150: 6d61 6c20 7661 6c75 6520 6f66 2073 6967  mal value of sig
-00006160: 6d61 0a20 2020 2020 2020 7666 2069 7320  ma.       vf is 
-00006170: 7468 6520 766f 6c75 6d65 2066 7261 6374  the volume fract
-00006180: 696f 6e20 6f66 2066 696c 6c65 720a 2020  ion of filler.  
-00006190: 2020 2020 2049 6e20 7468 6973 206d 6574       In this met
-000061a0: 686f 6420 7468 6520 4d47 206d 6574 686f  hod the MG metho
-000061b0: 6420 6973 2075 7365 6420 746f 2063 616c  d is used to cal
-000061c0: 6375 6c61 7465 2074 6865 2061 7665 7261  culate the avera
-000061d0: 6765 6420 6566 6665 6374 6976 6520 7065  ged effective pe
-000061e0: 726d 6974 7469 7669 7479 0a20 2020 2020  rmittivity.     
-000061f0: 2020 5468 656e 2074 6865 2070 6572 6d69    Then the permi
-00006200: 7474 6976 6974 7920 6f66 2074 6865 2069  ttivity of the i
-00006210: 736f 6474 726f 7069 6320 7370 6865 7265  sodtropic sphere
-00006220: 2074 6861 7420 776f 756c 6420 6769 7665   that would give
-00006230: 2074 6865 2073 616d 6520 6176 6572 6167   the same averag
-00006240: 6520 7065 726d 6974 7469 7669 7479 2069  e permittivity i
-00006250: 7320 6361 6c63 756c 6174 6564 0a20 2020  s calculated.   
-00006260: 2020 2020 5468 656e 2074 6865 204d 6965      Then the Mie
-00006270: 2073 6361 7474 6572 696e 6720 6f66 2074   scattering of t
-00006280: 6861 7420 7370 6865 7265 2069 7320 6361  hat sphere is ca
-00006290: 6c63 756c 6174 6564 0a20 2020 2020 2020  lculated.       
-000062a0: 5468 6520 726f 7574 696e 6520 7265 7475  The routine retu
-000062b0: 726e 7320 7468 6520 6566 6665 6374 6976  rns the effectiv
-000062c0: 6520 6469 656c 6563 7472 6963 2063 6f6e  e dielectric con
-000062d0: 7374 616e 7422 2222 0a20 2020 2023 0a20  stant""".    #. 
-000062e0: 2020 2023 2043 616c 6375 6c61 7465 2074     # Calculate t
-000062f0: 6865 204d 4720 7065 726d 6974 7469 7669  he MG permittivi
-00006300: 7479 2077 6974 6820 6e6f 2073 697a 6520  ty with no size 
-00006310: 6566 6665 6374 730a 2020 2020 230a 2020  effects.    #.  
-00006320: 2020 6d67 5f70 6572 6d69 7474 6976 6974    mg_permittivit
-00006330: 7920 3d20 6d61 7877 656c 6c28 6469 656c  y = maxwell(diel
-00006340: 6563 7472 6963 5f6d 6564 6975 6d2c 2063  ectric_medium, c
-00006350: 7279 7374 616c 5f70 6572 6d69 7474 6976  rystal_permittiv
-00006360: 6974 792c 2073 6861 7065 2c20 4c2c 2076  ity, shape, L, v
-00006370: 662c 2030 2e30 3030 3030 3031 290a 2020  f, 0.0000001).  
-00006380: 2020 2320 5573 6520 7363 616c 6172 2071    # Use scalar q
-00006390: 7561 6e74 6974 6965 7320 746f 2063 616c  uantities to cal
-000063a0: 6375 6c61 7465 2074 6865 2064 6965 6c65  culate the diele
-000063b0: 6374 7269 6320 636f 6e73 7461 6e74 206f  ctric constant o
-000063c0: 6620 7468 6520 6571 7569 7661 6c65 6e74  f the equivalent
-000063d0: 2069 736f 7472 6f70 6963 2073 7068 6572   isotropic spher
-000063e0: 650a 2020 2020 6566 203d 206e 702e 7472  e.    ef = np.tr
-000063f0: 6163 6528 6d67 5f70 6572 6d69 7474 6976  ace(mg_permittiv
-00006400: 6974 7929 202f 2033 2e30 0a20 2020 2065  ity) / 3.0.    e
-00006410: 6d20 3d20 6e70 2e74 7261 6365 2864 6965  m = np.trace(die
-00006420: 6c65 6374 7269 635f 6d65 6469 756d 2920  lectric_medium) 
-00006430: 2f20 332e 300a 2020 2020 2320 7072 696e  / 3.0.    # prin
-00006440: 7428 2763 7279 7374 616c 5f70 6572 6d69  t('crystal_permi
-00006450: 7474 6976 6974 7927 2c63 7279 7374 616c  ttivity',crystal
-00006460: 5f70 6572 6d69 7474 6976 6974 7929 0a20  _permittivity). 
-00006470: 2020 2023 2070 7269 6e74 2827 4d61 7877     # print('Maxw
-00006480: 656c 6c27 2c65 6629 0a20 2020 2023 2070  ell',ef).    # p
-00006490: 7269 6e74 2827 454d 6564 6975 6d27 2c65  rint('EMedium',e
-000064a0: 6d29 0a20 2020 2023 2043 616c 6375 6c61  m).    # Calcula
-000064b0: 7465 2074 6865 2070 6572 6d69 7474 6976  te the permittiv
-000064c0: 6974 7920 6f66 2061 6e20 6973 6f74 726f  ity of an isotro
-000064d0: 7069 6320 7370 6865 7265 2074 6861 7420  pic sphere that 
-000064e0: 6861 7320 7468 6520 7361 6d65 2065 6666  has the same eff
-000064f0: 6563 7469 7665 2070 6572 6d69 7474 6976  ective permittiv
-00006500: 6974 790a 2020 2020 6569 6e63 6c75 7369  ity.    einclusi
-00006510: 6f6e 203d 2028 202d 332a 7666 2a65 6d2a  on = ( -3*vf*em*
-00006520: 656d 202d 2028 6566 202d 2065 6d29 2a65  em - (ef - em)*e
-00006530: 6d2a 2832 2b76 6629 2029 202f 2028 2865  m*(2+vf) ) / ((e
-00006540: 662d 656d 292a 2831 2d76 6629 202d 2033  f-em)*(1-vf) - 3
-00006550: 2a76 662a 656d 290a 2020 2020 2320 7072  *vf*em).    # pr
-00006560: 696e 7428 2745 2069 6e63 6c75 7369 6f6e  int('E inclusion
-00006570: 272c 6569 6e63 6c75 7369 6f6e 290a 2020  ',einclusion).  
-00006580: 2020 6469 656c 6563 7620 3d20 6569 6e63    dielecv = einc
-00006590: 6c75 7369 6f6e 2a6e 702e 6579 6528 3329  lusion*np.eye(3)
-000065a0: 0a20 2020 2023 2070 7269 6e74 2827 4e65  .    # print('Ne
-000065b0: 7720 6469 656c 6563 7627 2c64 6965 6c65  w dielecv',diele
-000065c0: 6376 290a 2020 2020 2320 6465 6669 6e65  cv).    # define
-000065d0: 2069 2061 7320 6120 636f 6d70 6c65 7820   i as a complex 
-000065e0: 6e75 6d62 6572 0a20 2020 2069 203d 2063  number.    i = c
-000065f0: 6f6d 706c 6578 2830 2c31 290a 2020 2020  omplex(0,1).    
-00006600: 2320 5765 206e 6565 6420 746f 2074 616b  # We need to tak
-00006610: 656e 2061 6363 6f75 6e74 206f 6620 7468  en account of th
-00006620: 6520 6368 616e 6765 2069 6e20 7761 7665  e change in wave
-00006630: 6c65 6e67 7468 2061 6e64 2074 6865 2063  length and the c
-00006640: 6861 6e67 6520 696e 2073 697a 6520 7061  hange in size pa
-00006650: 7261 6d65 7465 7220 6475 6520 746f 2074  rameter due to t
-00006660: 6865 0a20 2020 2023 204e 6f6e 6520 756e  he.    # None un
-00006670: 6974 2076 616c 7565 206f 6620 7468 6520  it value of the 
-00006680: 6469 656c 6563 7472 6963 206f 6620 7468  dielectric of th
-00006690: 6520 656d 6265 6464 696e 6720 6d65 6469  e embedding medi
-000066a0: 756d 0a20 2020 2023 2054 6865 2073 697a  um.    # The siz
-000066b0: 6520 7061 7261 6d65 7465 7220 6973 2032  e parameter is 2
-000066c0: 7069 2072 202f 206c 616d 6264 610a 2020  pi r / lambda.  
-000066d0: 2020 2320 5468 6520 6566 6665 6374 6976    # The effectiv
-000066e0: 6520 6c61 6d62 6461 2069 6e20 7468 6520  e lambda in the 
-000066f0: 7375 7070 6f72 7469 6e67 206d 6564 6975  supporting mediu
-00006700: 6d20 6973 206c 616d 6264 6120 2f20 7371  m is lambda / sq
-00006710: 7274 2865 6d65 6469 756d 290a 2020 2020  rt(emedium).    
-00006720: 2320 5768 6572 6520 7468 6520 7265 6672  # Where the refr
-00006730: 6163 7469 7665 2069 6e64 6578 2069 7320  active index is 
-00006740: 7461 6b65 6e20 746f 2062 6520 7371 7274  taken to be sqrt
-00006750: 2865 6d65 6469 756d 2920 286e 6f6e 206d  (emedium) (non m
-00006760: 6167 6e65 7469 6320 6d61 7465 7269 616c  agnetic material
-00006770: 7329 0a20 2020 2065 6d65 6469 756d 203d  s).    emedium =
-00006780: 206e 702e 7472 6163 6528 6469 656c 6563   np.trace(dielec
-00006790: 7472 6963 5f6d 6564 6975 6d29 202f 2033  tric_medium) / 3
-000067a0: 2e30 0a20 2020 2072 6566 7261 6374 6976  .0.    refractiv
-000067b0: 655f 696e 6465 785f 6d65 6469 756d 203d  e_index_medium =
-000067c0: 206e 702e 7265 616c 286e 702e 7371 7274   np.real(np.sqrt
-000067d0: 2865 6d65 6469 756d 2929 0a20 2020 206c  (emedium)).    l
-000067e0: 616d 6264 615f 7661 6375 756d 5f6d 7520  ambda_vacuum_mu 
-000067f0: 3d20 3220 2a20 5049 202a 2073 697a 655f  = 2 * PI * size_
-00006800: 6d75 202f 2073 697a 650a 2020 2020 7761  mu / size.    wa
-00006810: 7665 6c65 6e67 7468 5f6e 6d20 3d20 6c61  velength_nm = la
-00006820: 6d62 6461 5f76 6163 7575 6d5f 6d75 202a  mbda_vacuum_mu *
-00006830: 2031 3030 3020 2f20 7265 6672 6163 7469   1000 / refracti
-00006840: 7665 5f69 6e64 6578 5f6d 6564 6975 6d0a  ve_index_medium.
-00006850: 2020 2020 7261 6469 7573 5f6e 6d20 3d20      radius_nm = 
-00006860: 7369 7a65 5f6d 7520 2a20 3130 3030 0a20  size_mu * 1000. 
-00006870: 2020 2023 2054 6865 2077 6176 6576 6563     # The wavevec
-00006880: 746f 7220 696e 206e 6d2d 310a 2020 2020  tor in nm-1.    
-00006890: 6b5f 6e6d 203d 2032 202a 2050 4920 2f20  k_nm = 2 * PI / 
-000068a0: 7761 7665 6c65 6e67 7468 5f6e 6d0a 2020  wavelength_nm.  
-000068b0: 2020 2320 766f 6c75 6d65 206f 6620 6120    # volume of a 
-000068c0: 7061 7274 6963 6c65 2069 6e20 6e6d 5e33  particle in nm^3
-000068d0: 0a20 2020 2056 5f6e 6d20 3d20 342e 302f  .    V_nm = 4.0/
-000068e0: 332e 3020 2a20 5049 202a 2072 6164 6975  3.0 * PI * radiu
-000068f0: 735f 6e6d 202a 2072 6164 6975 735f 6e6d  s_nm * radius_nm
-00006900: 202a 2072 6164 6975 735f 6e6d 0a20 2020   * radius_nm.   
-00006910: 2023 204e 756d 6265 7220 6465 6e73 6974   # Number densit
-00006920: 7920 6f66 2070 6172 7469 636c 6573 2028  y of particles (
-00006930: 6e75 6d62 6572 202f 206e 6d5e 3329 0a20  number / nm^3). 
-00006940: 2020 204e 5f6e 6d20 3d20 7666 202f 2056     N_nm = vf / V
-00006950: 5f6e 6d0a 2020 2020 2320 4966 2074 6865  _nm.    # If the
-00006960: 7265 2069 7320 6120 7369 7a65 2064 6973  re is a size dis
-00006970: 7472 6962 7574 696f 6e20 7365 7420 7570  tribution set up
-00006980: 2074 6f20 7573 6520 6974 0a20 2020 2069   to use it.    i
-00006990: 6620 7369 7a65 5f64 6973 7472 6962 7574  f size_distribut
-000069a0: 696f 6e5f 7369 676d 613a 0a20 2020 2020  ion_sigma:.     
-000069b0: 2020 206c 6f77 6572 2c75 7070 6572 203d     lower,upper =
-000069c0: 206c 6f67 6e6f 726d 2e69 6e74 6572 7661   lognorm.interva
-000069d0: 6c28 302e 3939 3939 2c73 697a 655f 6469  l(0.9999,size_di
-000069e0: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
-000069f0: 2c73 6361 6c65 3d73 697a 655f 6d75 290a  ,scale=size_mu).
-00006a00: 2020 2020 2020 2020 6e75 6d62 6572 4f66          numberOf
-00006a10: 4269 6e73 203d 2034 300a 2020 2020 2020  Bins = 40.      
-00006a20: 2020 6470 203d 206e 702e 6c6f 6773 7061    dp = np.logspa
-00006a30: 6365 286e 702e 6c6f 6728 6c6f 7765 7229  ce(np.log(lower)
-00006a40: 2c6e 702e 6c6f 6728 7570 7065 7229 2c6e  ,np.log(upper),n
-00006a50: 756d 6265 724f 6642 696e 732c 6261 7365  umberOfBins,base
-00006a60: 3d6e 702e 6529 0a20 2020 2020 2020 2023  =np.e).        #
-00006a70: 2054 6865 2064 6566 696e 6974 696f 6e73   The definitions
-00006a80: 2075 7365 6420 6172 6520 636f 6e66 7573   used are confus
-00006a90: 696e 673b 0a20 2020 2020 2020 2023 2064  ing;.        # d
-00006aa0: 7020 6973 2074 6865 206c 6f67 206f 6620  p is the log of 
-00006ab0: 7468 6520 7661 7269 6162 6c65 0a20 2020  the variable.   
-00006ac0: 2020 2020 2023 2073 2069 7320 7468 6520       # s is the 
-00006ad0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-00006ae0: 6f6e 2028 7368 6170 6520 6675 6e63 7469  on (shape functi
-00006af0: 6f6e 2920 6f66 2074 6865 206c 6f67 206f  on) of the log o
-00006b00: 6620 7468 6520 7661 7269 6174 650a 2020  f the variate.  
-00006b10: 2020 2020 2020 2320 7363 616c 6520 6973        # scale is
-00006b20: 2074 6865 206d 6561 6e20 6f66 2074 6865   the mean of the
-00006b30: 2075 6e64 6572 6c79 696e 6720 6e6f 726d   underlying norm
-00006b40: 616c 2064 6973 7472 6962 7574 696f 6e0a  al distribution.
-00006b50: 2020 2020 2020 2020 6e64 7020 3d20 6c6f          ndp = lo
-00006b60: 676e 6f72 6d2e 7064 6628 6470 2c73 3d73  gnorm.pdf(dp,s=s
-00006b70: 697a 655f 6469 7374 7269 6275 7469 6f6e  ize_distribution
-00006b80: 5f73 6967 6d61 2c73 6361 6c65 3d73 697a  _sigma,scale=siz
-00006b90: 655f 6d75 290a 2020 2020 2020 2020 2370  e_mu).        #p
-00006ba0: 7269 6e74 2822 4450 222c 6470 290a 2020  rint("DP",dp).  
-00006bb0: 2020 2020 2020 2370 7269 6e74 2822 4e44        #print("ND
-00006bc0: 5022 2c6e 6470 290a 2020 2020 2020 2020  P",ndp).        
-00006bd0: 2370 7269 6e74 2822 5570 7065 7220 6c6f  #print("Upper lo
-00006be0: 7765 7222 2c6c 6f77 6572 2c75 7070 6572  wer",lower,upper
-00006bf0: 290a 2020 2020 2020 2020 2370 7269 6e74  ).        #print
-00006c00: 2822 5369 7a65 5f4d 5522 2c73 697a 655f  ("Size_MU",size_
-00006c10: 6d75 290a 2020 2020 7265 6672 6163 7469  mu).    refracti
-00006c20: 7665 5f69 6e64 6578 203d 2063 616c 6375  ve_index = calcu
-00006c30: 6c61 7465 5f72 6566 7261 6374 6976 655f  late_refractive_
-00006c40: 696e 6465 785f 7363 616c 6172 2865 696e  index_scalar(ein
-00006c50: 636c 7573 696f 6e29 202f 2072 6566 7261  clusion) / refra
-00006c60: 6374 6976 655f 696e 6465 785f 6d65 6469  ctive_index_medi
-00006c70: 756d 0a20 2020 2023 6a6b 2070 7269 6e74  um.    #jk print
-00006c80: 2827 7265 6672 6163 7469 7665 5f69 6e64  ('refractive_ind
-00006c90: 6578 272c 2072 6566 7261 6374 6976 655f  ex', refractive_
-00006ca0: 696e 6465 7829 0a20 2020 2023 6a6b 2070  index).    #jk p
-00006cb0: 7269 6e74 2827 7265 6672 6163 7469 7665  rint('refractive
-00006cc0: 5f69 6e64 6578 5f6d 6564 6975 6d27 2c20  _index_medium', 
-00006cd0: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
-00006ce0: 5f6d 6564 6975 6d29 0a20 2020 2023 6a6b  _medium).    #jk
-00006cf0: 2070 7269 6e74 2827 6569 6e63 6c75 7369   print('einclusi
-00006d00: 6f6e 272c 2065 696e 636c 7573 696f 6e29  on', einclusion)
-00006d10: 0a20 2020 2069 6620 7369 7a65 5f64 6973  .    if size_dis
-00006d20: 7472 6962 7574 696f 6e5f 7369 676d 613a  tribution_sigma:
-00006d30: 0a20 2020 2020 2020 2023 2043 616c 6375  .        # Calcu
-00006d40: 6c61 7465 2074 6865 2069 6e74 6567 7261  late the integra
-00006d50: 6c20 6f66 2074 6865 2066 6f72 7761 7264  l of the forward
-00006d60: 2073 6361 7474 6572 696e 6720 6661 6374   scattering fact
-00006d70: 6f72 7320 6f76 6572 2074 6865 2064 6973  ors over the dis
-00006d80: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
-00006d90: 2020 7331 5f66 6163 746f 7273 203d 205b    s1_factors = [
-00006da0: 5d0a 2020 2020 2020 2020 666f 7220 7220  ].        for r 
-00006db0: 696e 2064 703a 0a20 2020 2020 2020 2020  in dp:.         
-00006dc0: 2020 2023 2054 6865 2073 697a 6520 7061     # The size pa
-00006dd0: 7261 6d65 7465 7220 6973 2032 7069 2072  rameter is 2pi r
-00006de0: 202f 206c 616d 6264 610a 2020 2020 2020   / lambda.      
-00006df0: 2020 2020 2020 7820 3d20 3220 2a20 5049        x = 2 * PI
-00006e00: 202a 2072 202f 206c 616d 6264 615f 7661   * r / lambda_va
-00006e10: 6375 756d 5f6d 750a 2020 2020 2020 2020  cuum_mu.        
-00006e20: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
-00006e30: 7468 6520 5331 2061 6e64 2053 3220 7363  the S1 and S2 sc
-00006e40: 6174 7465 7269 6e67 2066 6163 746f 7273  attering factors
-00006e50: 2c20 616e 6420 7374 6f72 6520 696e 2061  , and store in a
-00006e60: 206c 6973 740a 2020 2020 2020 2020 2020   list.          
-00006e70: 2020 7331 2c73 3220 3d20 4d69 652e 4d69    s1,s2 = Mie.Mi
-00006e80: 6553 3153 3228 7265 6672 6163 7469 7665  eS1S2(refractive
-00006e90: 5f69 6e64 6578 2c20 782a 7265 6672 6163  _index, x*refrac
-00006ea0: 7469 7665 5f69 6e64 6578 5f6d 6564 6975  tive_index_mediu
-00006eb0: 6d2c 2031 290a 2020 2020 2020 2020 2020  m, 1).          
-00006ec0: 2020 7331 5f66 6163 746f 7273 2e61 7070    s1_factors.app
-00006ed0: 656e 6428 7331 290a 2020 2020 2020 2020  end(s1).        
-00006ee0: 2320 4e6f 7720 696e 7465 6772 6174 650a  # Now integrate.
-00006ef0: 2020 2020 2020 2020 7331 203d 2074 7261          s1 = tra
-00006f00: 707a 2873 315f 6661 6374 6f72 732a 6e64  pz(s1_factors*nd
-00006f10: 702c 6470 290a 2020 2020 2020 2020 6e6f  p,dp).        no
-00006f20: 726d 616c 203d 2074 7261 707a 286e 6470  rmal = trapz(ndp
-00006f30: 2c64 7029 0a20 2020 2020 2020 2023 6d65  ,dp).        #me
-00006f40: 616e 203d 2074 7261 707a 286e 6470 2a64  an = trapz(ndp*d
-00006f50: 702c 6470 290a 2020 2020 2020 2020 2374  p,dp).        #t
-00006f60: 7275 655f 6d65 616e 203d 206e 702e 6578  rue_mean = np.ex
-00006f70: 7028 206e 702e 6c6f 6728 7369 7a65 5f6d  p( np.log(size_m
-00006f80: 7529 202b 2073 697a 655f 6469 7374 7269  u) + size_distri
-00006f90: 6275 7469 6f6e 5f73 6967 6d61 2a73 697a  bution_sigma*siz
-00006fa0: 655f 6469 7374 7269 6275 7469 6f6e 5f73  e_distribution_s
-00006fb0: 6967 6d61 2f32 2e30 290a 2020 2020 2020  igma/2.0).      
-00006fc0: 2020 2376 5f63 6d31 203d 2031 2e30 4534    #v_cm1 = 1.0E4
-00006fd0: 2f6c 616d 6264 615f 7661 6375 756d 5f6d  /lambda_vacuum_m
-00006fe0: 750a 2020 2020 2020 2020 2370 7269 6e74  u.        #print
-00006ff0: 2822 4672 6571 7565 6e63 792c 6e6f 726d  ("Frequency,norm
-00007000: 616c 2c6d 6561 6e22 2c76 5f63 6d31 2c6e  al,mean",v_cm1,n
-00007010: 6f72 6d61 6c2c 7472 7565 5f6d 6561 6e2c  ormal,true_mean,
-00007020: 6d65 616e 290a 2020 2020 2020 2020 6966  mean).        if
-00007030: 206e 702e 6162 7328 6e6f 726d 616c 202d   np.abs(normal -
-00007040: 2031 2e30 2920 3e20 312e 3045 2d32 3a0a   1.0) > 1.0E-2:.
-00007050: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00007060: 7428 2257 6172 6e69 6e67 2069 6e74 6567  t("Warning integ
-00007070: 7261 7469 6f6e 206f 6620 6c6f 672d 6e6f  ration of log-no
-00007080: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
-00007090: 6e20 696e 2065 7272 6f72 222c 206e 6f72  n in error", nor
-000070a0: 6d61 6c29 0a20 2020 2020 2020 2020 2020  mal).           
-000070b0: 2070 7269 6e74 2822 5374 6f70 7069 6e67   print("Stopping
-000070c0: 2063 616c 6375 6c61 7469 6f6e 202d 206c   calculation - l
-000070d0: 696b 656c 7920 7072 6f62 6c65 6d20 6973  ikely problem is
-000070e0: 2074 6f6f 206c 6172 6765 2061 2073 6967   too large a sig
-000070f0: 6d61 2066 6f72 206c 6f67 2d6e 6f72 6d61  ma for log-norma
-00007100: 6c20 6469 7374 7269 6275 7469 6f6e 2229  l distribution")
-00007110: 0a20 2020 2020 2020 2020 2020 2065 6666  .            eff
-00007120: 6469 656c 6563 203d 206e 702e 6172 7261  dielec = np.arra
-00007130: 7928 5b5b 312c 2030 2c20 305d 2c20 5b30  y([[1, 0, 0], [0
-00007140: 2c20 312c 2030 5d2c 205b 302c 2030 2c20  , 1, 0], [0, 0, 
-00007150: 315d 5d29 0a20 2020 2020 2020 2020 2020  1]]).           
-00007160: 2072 6574 7572 6e20 6566 6664 6965 6c65   return effdiele
-00007170: 630a 2020 2020 656c 7365 3a0a 2020 2020  c.    else:.    
-00007180: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
-00007190: 7468 6520 7363 6174 7465 7269 6e67 2066  the scattering f
-000071a0: 6163 746f 7273 2061 7420 3020 6465 6772  actors at 0 degr
-000071b0: 6565 730a 2020 2020 2020 2020 236a 6b20  ees.        #jk 
-000071c0: 7072 696e 7428 2272 6566 7261 6374 6976  print("refractiv
-000071d0: 655f 696e 6465 782c 2073 697a 652c 2072  e_index, size, r
-000071e0: 6566 7261 6374 6976 655f 696e 6465 785f  efractive_index_
-000071f0: 6d65 6469 756d 222c 2072 6566 7261 6374  medium", refract
-00007200: 6976 655f 696e 6465 782c 2073 697a 652c  ive_index, size,
-00007210: 2072 6566 7261 6374 6976 655f 696e 6465   refractive_inde
-00007220: 785f 6d65 6469 756d 290a 2020 2020 2020  x_medium).      
-00007230: 2020 7331 2c73 3220 3d20 4d69 652e 4d69    s1,s2 = Mie.Mi
-00007240: 6553 3153 3228 7265 6672 6163 7469 7665  eS1S2(refractive
-00007250: 5f69 6e64 6578 2c20 7369 7a65 2a72 6566  _index, size*ref
-00007260: 7261 6374 6976 655f 696e 6465 785f 6d65  ractive_index_me
-00007270: 6469 756d 2c20 3129 0a20 2020 2023 2053  dium, 1).    # S
-00007280: 6565 2076 616e 2064 6520 4875 6c73 7420  ee van de Hulst 
-00007290: 7061 6765 2031 3239 2c20 3133 300a 2020  page 129, 130.  
-000072a0: 2020 2320 5265 6672 6163 7469 7665 2069    # Refractive i
-000072b0: 6e64 6578 206f 6620 6d61 7465 7269 616c  ndex of material
-000072c0: 2069 730a 2020 2020 2320 7468 6520 7369   is.    # the si
-000072d0: 676e 206f 6620 7468 6520 696d 6167 696e  gn of the imagin
-000072e0: 6172 7920 636f 6d70 6f6e 656e 7420 6861  ary component ha
-000072f0: 7320 6368 616e 6765 6420 666f 7220 636f  s changed for co
-00007300: 6d70 6174 6962 696c 6974 7920 7769 7468  mpatibility with
-00007310: 204d 472f 4272 7567 6765 6d61 6e0a 2020   MG/Bruggeman.  
-00007320: 2020 7265 6672 6163 7469 7665 5f69 6e64    refractive_ind
-00007330: 6578 203d 2072 6566 7261 6374 6976 655f  ex = refractive_
-00007340: 696e 6465 785f 6d65 6469 756d 202a 2028  index_medium * (
-00007350: 2031 2e30 202b 2069 202a 2073 3120 2a20   1.0 + i * s1 * 
-00007360: 3220 2a20 5049 202a 204e 5f6e 6d20 2f20  2 * PI * N_nm / 
-00007370: 2820 6b5f 6e6d 202a 206b 5f6e 6d20 2a20  ( k_nm * k_nm * 
-00007380: 6b5f 6e6d 2029 2029 0a20 2020 2065 6666  k_nm ) ).    eff
-00007390: 203d 2072 6566 7261 6374 6976 655f 696e   = refractive_in
-000073a0: 6465 7820 2a20 7265 6672 6163 7469 7665  dex * refractive
-000073b0: 5f69 6e64 6578 0a20 2020 2065 6666 6469  _index.    effdi
-000073c0: 656c 6563 203d 206e 702e 6172 7261 7928  elec = np.array(
-000073d0: 5b5b 6566 662c 2030 2c20 305d 2c20 5b30  [[eff, 0, 0], [0
-000073e0: 2c20 6566 662c 2030 5d2c 205b 302c 2030  , eff, 0], [0, 0
-000073f0: 2c20 6566 665d 5d29 0a20 2020 2023 6a6b  , eff]]).    #jk
-00007400: 2070 7269 6e74 2872 6164 6975 735f 6e6d   print(radius_nm
-00007410: 2c20 6c61 6d62 6461 5f76 6163 7575 6d5f  , lambda_vacuum_
-00007420: 6d75 2a31 3030 302e 302c 2071 6578 742c  mu*1000.0, qext,
-00007430: 7173 6361 2c71 6162 732c 672c 7170 722c  qsca,qabs,g,qpr,
-00007440: 7162 6163 6b2c 7172 6174 696f 2c6e 702e  qback,qratio,np.
-00007450: 7265 616c 2873 3129 2c6e 702e 696d 6167  real(s1),np.imag
-00007460: 2873 3129 2c6e 702e 7265 616c 2872 6566  (s1),np.real(ref
-00007470: 7261 6374 6976 655f 696e 6465 7829 2c6e  ractive_index),n
-00007480: 702e 696d 6167 2872 6566 7261 6374 6976  p.imag(refractiv
-00007490: 655f 696e 6465 7829 2c6e 702e 7265 616c  e_index),np.real
-000074a0: 2865 6666 292c 6e70 2e69 6d61 6728 6566  (eff),np.imag(ef
-000074b0: 6629 290a 2020 2020 2370 7269 6e74 2028  f)).    #print (
-000074c0: 2272 6164 6975 735f 6e6d 2c20 6566 6622  "radius_nm, eff"
-000074d0: 2c20 7261 6469 7573 5f6e 6d2c 2065 6666  , radius_nm, eff
-000074e0: 290a 2020 2020 7265 7475 726e 2065 6666  ).    return eff
-000074f0: 6469 656c 6563 0a0a 6465 6620 616e 6973  dielec..def anis
-00007500: 6f74 726f 7069 635f 6d69 655f 7363 6174  otropic_mie_scat
-00007510: 7465 7269 6e67 2864 6965 6c65 6374 7269  tering(dielectri
-00007520: 635f 6d65 6469 756d 2c20 6372 7973 7461  c_medium, crysta
-00007530: 6c5f 7065 726d 6974 7469 7669 7479 2c20  l_permittivity, 
-00007540: 7368 6170 652c 204c 2c20 7666 2c20 7369  shape, L, vf, si
-00007550: 7a65 2c20 7369 7a65 5f6d 752c 2073 697a  ze, size_mu, siz
-00007560: 655f 6469 7374 7269 6275 7469 6f6e 5f73  e_distribution_s
-00007570: 6967 6d61 293a 0a20 2020 2022 2222 4361  igma):.    """Ca
-00007580: 6c63 756c 6174 6520 7468 6520 6566 6665  lculate the effe
-00007590: 6374 6976 6520 636f 6e73 7461 6e74 2070  ctive constant p
-000075a0: 6572 6d69 7474 6976 6974 7920 7573 696e  ermittivity usin
-000075b0: 6720 6120 4d69 6520 7363 6174 7465 7269  g a Mie scatteri
-000075c0: 6e67 2061 7070 726f 6163 680a 2020 2020  ng approach.    
-000075d0: 2020 2064 6965 6c65 6374 7269 635f 6d65     dielectric_me
-000075e0: 6469 756d 2069 7320 7468 6520 6469 656c  dium is the diel
-000075f0: 6563 7472 6963 2063 6f6e 7374 616e 7420  ectric constant 
-00007600: 7465 6e73 6f72 206f 6620 7468 6520 6d65  tensor of the me
-00007610: 6469 756d 0a20 2020 2020 2020 6372 7973  dium.       crys
-00007620: 7461 6c5f 7065 726d 6974 7469 7669 7479  tal_permittivity
-00007630: 2069 7320 7468 6520 746f 7461 6c20 6672   is the total fr
-00007640: 6571 7565 6e63 7920 6469 656c 6563 7472  equency dielectr
-00007650: 6963 2063 6f6e 7374 616e 7420 7465 6e73  ic constant tens
-00007660: 6f72 2061 7420 7468 6520 6375 7272 656e  or at the curren
-00007670: 7420 6672 6571 7565 6e63 790a 2020 2020  t frequency.    
-00007680: 2020 2073 6861 7065 2069 7320 7468 6520     shape is the 
-00007690: 6e61 6d65 206f 6620 7468 6520 6375 7272  name of the curr
-000076a0: 656e 7420 7368 6170 6520 284e 4f54 2055  ent shape (NOT U
-000076b0: 5345 4429 0a20 2020 2020 2020 4c20 6973  SED).       L is
-000076c0: 2074 6865 2073 6861 7065 7320 6465 706f   the shapes depo
-000076d0: 6c61 7269 7361 7469 6f6e 206d 6174 7269  larisation matri
-000076e0: 7820 284e 4f54 2055 5345 4429 0a20 2020  x (NOT USED).   
-000076f0: 2020 2020 7369 7a65 2069 7320 7468 6520      size is the 
-00007700: 6469 6d65 6e73 696f 6e6c 6573 7320 7369  dimensionless si
-00007710: 7a65 2070 6172 616d 6574 6572 2066 6f72  ze parameter for
-00007720: 2074 6865 2066 7265 7175 656e 6379 2075   the frequency u
-00007730: 6e64 6572 2063 6f6e 7369 6465 7261 7469  nder considerati
-00007740: 6f6e 0a20 2020 2020 2020 7369 7a65 5f64  on.       size_d
-00007750: 6973 7472 6962 7574 696f 6e5f 7369 676d  istribution_sigm
-00007760: 6120 6973 2074 6865 206c 6f67 206e 6f72  a is the log nor
-00007770: 6d61 6c20 7661 6c75 6520 6f66 2073 6967  mal value of sig
-00007780: 6d61 0a20 2020 2020 2020 7666 2069 7320  ma.       vf is 
-00007790: 7468 6520 766f 6c75 6d65 2066 7261 6374  the volume fract
-000077a0: 696f 6e20 6f66 2066 696c 6c65 720a 2020  ion of filler.  
-000077b0: 2020 2020 204d 6965 206f 6e6c 7920 776f       Mie only wo
-000077c0: 726b 7320 666f 7220 7370 6865 7269 6361  rks for spherica
-000077d0: 6c20 7061 7274 6963 6c65 732c 2073 6f20  l particles, so 
-000077e0: 7368 6170 652c 2061 6e64 204c 2070 6172  shape, and L par
-000077f0: 616d 6574 6572 7320 6172 6520 6967 6e6f  ameters are igno
-00007800: 7265 640a 2020 2020 2020 2054 6865 2072  red.       The r
-00007810: 6f75 7469 6e65 2072 6574 7572 6e73 2074  outine returns t
-00007820: 6865 2065 6666 6563 7469 7665 2064 6965  he effective die
-00007830: 6c65 6374 7269 6320 636f 6e73 7461 6e74  lectric constant
-00007840: 2222 220a 2020 2020 2320 6465 6669 6e65  """.    # define
-00007850: 2069 2061 7320 6120 636f 6d70 6c65 7820   i as a complex 
-00007860: 6e75 6d62 6572 0a20 2020 2069 203d 2063  number.    i = c
-00007870: 6f6d 706c 6578 2830 2c31 290a 2020 2020  omplex(0,1).    
-00007880: 2320 5765 206e 6565 6420 746f 2074 616b  # We need to tak
-00007890: 656e 2061 6363 6f75 6e74 206f 6620 7468  en account of th
-000078a0: 6520 6368 616e 6765 2069 6e20 7761 7665  e change in wave
-000078b0: 6c65 6e67 7468 2061 6e64 2074 6865 2063  length and the c
-000078c0: 6861 6e67 6520 696e 2073 697a 6520 7061  hange in size pa
-000078d0: 7261 6d65 7465 7220 6475 6520 746f 2074  rameter due to t
-000078e0: 6865 0a20 2020 2023 204e 6f6e 6520 756e  he.    # None un
-000078f0: 6974 2076 616c 7565 206f 6620 7468 6520  it value of the 
-00007900: 6469 656c 6563 7472 6963 206f 6620 7468  dielectric of th
-00007910: 6520 656d 6265 6464 696e 6720 6d65 6469  e embedding medi
-00007920: 756d 0a20 2020 2023 2054 6865 2073 697a  um.    # The siz
-00007930: 6520 7061 7261 6d65 7465 7220 6973 2032  e parameter is 2
-00007940: 7069 2072 202f 206c 616d 6264 610a 2020  pi r / lambda.  
-00007950: 2020 2320 5468 6520 6566 6665 6374 6976    # The effectiv
-00007960: 6520 6c61 6d62 6461 2069 6e20 7468 6520  e lambda in the 
-00007970: 7375 7070 6f72 7469 6e67 206d 6564 6975  supporting mediu
-00007980: 6d20 6973 206c 616d 6264 6120 2f20 7371  m is lambda / sq
-00007990: 7274 2865 6d65 6469 756d 290a 2020 2020  rt(emedium).    
-000079a0: 2320 5768 6572 6520 7468 6520 7265 6672  # Where the refr
-000079b0: 6163 7469 7665 2069 6e64 6578 2069 7320  active index is 
-000079c0: 7461 6b65 6e20 746f 2062 6520 7371 7274  taken to be sqrt
-000079d0: 2865 6d65 6469 756d 2920 286e 6f6e 206d  (emedium) (non m
-000079e0: 6167 6e65 7469 6320 6d61 7465 7269 616c  agnetic material
-000079f0: 7329 0a20 2020 2065 6d65 6469 756d 203d  s).    emedium =
-00007a00: 206e 702e 7472 6163 6528 6469 656c 6563   np.trace(dielec
-00007a10: 7472 6963 5f6d 6564 6975 6d29 202f 2033  tric_medium) / 3
-00007a20: 2e30 0a20 2020 2072 6566 7261 6374 6976  .0.    refractiv
-00007a30: 655f 696e 6465 785f 6d65 6469 756d 203d  e_index_medium =
-00007a40: 206e 702e 7265 616c 286e 702e 7371 7274   np.real(np.sqrt
-00007a50: 2865 6d65 6469 756d 2929 0a20 2020 206c  (emedium)).    l
-00007a60: 616d 6264 615f 7661 6375 756d 5f6d 7520  ambda_vacuum_mu 
-00007a70: 3d20 3220 2a20 5049 202a 2073 697a 655f  = 2 * PI * size_
-00007a80: 6d75 202f 2073 697a 650a 2020 2020 7761  mu / size.    wa
-00007a90: 7665 6c65 6e67 7468 5f6e 6d20 3d20 6c61  velength_nm = la
-00007aa0: 6d62 6461 5f76 6163 7575 6d5f 6d75 202a  mbda_vacuum_mu *
-00007ab0: 2031 3030 3020 2f20 7265 6672 6163 7469   1000 / refracti
-00007ac0: 7665 5f69 6e64 6578 5f6d 6564 6975 6d0a  ve_index_medium.
-00007ad0: 2020 2020 7261 6469 7573 5f6e 6d20 3d20      radius_nm = 
-00007ae0: 7369 7a65 5f6d 7520 2a20 3130 3030 0a20  size_mu * 1000. 
-00007af0: 2020 2023 2054 6f20 6163 636f 756e 7420     # To account 
-00007b00: 666f 7220 616e 6973 6f74 726f 7079 2077  for anisotropy w
-00007b10: 6520 6469 6167 6f6e 616c 6973 6520 7468  e diagonalise th
-00007b20: 6520 7265 616c 2070 6172 7420 6f66 2074  e real part of t
-00007b30: 6865 2064 6965 6c65 6374 7269 6320 6d61  he dielectric ma
-00007b40: 7472 6978 2061 6e64 2074 7261 6e73 666f  trix and transfo
-00007b50: 726d 0a20 2020 2023 2074 6865 2066 756c  rm.    # the ful
-00007b60: 6c20 6d61 7472 6978 2077 6974 6820 7468  l matrix with th
-00007b70: 6520 6569 6765 6e76 6563 746f 7273 2c20  e eigenvectors, 
-00007b80: 550a 2020 2020 2320 4669 6e64 2055 2061  U.    # Find U a
-00007b90: 6e64 2045 2c20 7375 6368 2074 6861 7420  nd E, such that 
-00007ba0: 5554 2e20 442e 2055 203d 2045 2028 7768  UT. D. U = E (wh
-00007bb0: 6572 6520 4420 6973 2074 6865 2072 6561  ere D is the rea
-00007bc0: 6c20 7061 7274 206f 6620 6372 7973 7461  l part of crysta
-00007bd0: 6c5f 7065 726d 6974 7469 7669 7479 290a  l_permittivity).
-00007be0: 2020 2020 452c 5520 3d20 6e70 2e6c 696e      E,U = np.lin
-00007bf0: 616c 672e 6569 6728 6e70 2e72 6561 6c28  alg.eig(np.real(
-00007c00: 6372 7973 7461 6c5f 7065 726d 6974 7469  crystal_permitti
-00007c10: 7669 7479 2929 0a20 2020 2023 2054 7261  vity)).    # Tra
-00007c20: 6e73 666f 726d 2074 6865 2066 756c 6c20  nsform the full 
-00007c30: 6469 656c 6563 7472 6963 206d 6174 7269  dielectric matri
-00007c40: 780a 2020 2020 726f 7461 7465 645f 6469  x.    rotated_di
-00007c50: 656c 6563 203d 206e 702e 6d61 746d 756c  elec = np.matmul
-00007c60: 2855 2e54 2c6e 702e 6d61 746d 756c 2863  (U.T,np.matmul(c
-00007c70: 7279 7374 616c 5f70 6572 6d69 7474 6976  rystal_permittiv
-00007c80: 6974 792c 5529 290a 2020 2020 2320 5468  ity,U)).    # Th
-00007c90: 6520 7761 7665 7665 6374 6f72 2069 6e20  e wavevector in 
-00007ca0: 6e6d 2d31 0a20 2020 206b 5f6e 6d20 3d20  nm-1.    k_nm = 
-00007cb0: 3220 2a20 5049 202f 2077 6176 656c 656e  2 * PI / wavelen
-00007cc0: 6774 685f 6e6d 0a20 2020 2023 2076 6f6c  gth_nm.    # vol
-00007cd0: 756d 6520 6f66 2061 2070 6172 7469 636c  ume of a particl
-00007ce0: 6520 696e 206e 6d5e 330a 2020 2020 565f  e in nm^3.    V_
-00007cf0: 6e6d 203d 2034 2e30 2f33 2e30 202a 2050  nm = 4.0/3.0 * P
-00007d00: 4920 2a20 7261 6469 7573 5f6e 6d20 2a20  I * radius_nm * 
-00007d10: 7261 6469 7573 5f6e 6d20 2a20 7261 6469  radius_nm * radi
-00007d20: 7573 5f6e 6d0a 2020 2020 2320 4e75 6d62  us_nm.    # Numb
-00007d30: 6572 2064 656e 7369 7479 206f 6620 7061  er density of pa
-00007d40: 7274 6963 6c65 7320 286e 756d 6265 7220  rticles (number 
-00007d50: 2f20 6e6d 5e33 290a 2020 2020 4e5f 6e6d  / nm^3).    N_nm
-00007d60: 203d 2076 6620 2f20 565f 6e6d 0a20 2020   = vf / V_nm.   
-00007d70: 2023 2049 6620 7468 6572 6520 6973 2061   # If there is a
-00007d80: 2073 697a 6520 6469 7374 7269 6275 7469   size distributi
-00007d90: 6f6e 2073 6574 2075 7020 746f 2075 7365  on set up to use
-00007da0: 2069 740a 2020 2020 6966 2073 697a 655f   it.    if size_
-00007db0: 6469 7374 7269 6275 7469 6f6e 5f73 6967  distribution_sig
-00007dc0: 6d61 3a0a 2020 2020 2020 2020 6c6f 7765  ma:.        lowe
-00007dd0: 722c 7570 7065 7220 3d20 6c6f 676e 6f72  r,upper = lognor
-00007de0: 6d2e 696e 7465 7276 616c 2830 2e39 3939  m.interval(0.999
-00007df0: 392c 7369 7a65 5f64 6973 7472 6962 7574  9,size_distribut
-00007e00: 696f 6e5f 7369 676d 612c 7363 616c 653d  ion_sigma,scale=
-00007e10: 7369 7a65 5f6d 7529 0a20 2020 2020 2020  size_mu).       
-00007e20: 206e 756d 6265 724f 6642 696e 7320 3d20   numberOfBins = 
-00007e30: 3430 0a20 2020 2020 2020 2064 7020 3d20  40.        dp = 
-00007e40: 6e70 2e6c 6f67 7370 6163 6528 6e70 2e6c  np.logspace(np.l
-00007e50: 6f67 286c 6f77 6572 292c 6e70 2e6c 6f67  og(lower),np.log
-00007e60: 2875 7070 6572 292c 6e75 6d62 6572 4f66  (upper),numberOf
-00007e70: 4269 6e73 2c62 6173 653d 6e70 2e65 290a  Bins,base=np.e).
-00007e80: 2020 2020 2020 2020 2320 5468 6520 6465          # The de
-00007e90: 6669 6e69 7469 6f6e 7320 7573 6564 2061  finitions used a
-00007ea0: 7265 2063 6f6e 6675 7369 6e67 3b0a 2020  re confusing;.  
-00007eb0: 2020 2020 2020 2320 6470 2069 7320 7468        # dp is th
-00007ec0: 6520 6c6f 6720 6f66 2074 6865 2076 6172  e log of the var
-00007ed0: 6961 626c 650a 2020 2020 2020 2020 2320  iable.        # 
-00007ee0: 7320 6973 2074 6865 2073 7461 6e64 6172  s is the standar
-00007ef0: 6420 6465 7669 6174 696f 6e20 2873 6861  d deviation (sha
-00007f00: 7065 2066 756e 6374 696f 6e29 206f 6620  pe function) of 
-00007f10: 7468 6520 6c6f 6720 6f66 2074 6865 2076  the log of the v
-00007f20: 6172 6961 7465 0a20 2020 2020 2020 2023  ariate.        #
-00007f30: 2073 6361 6c65 2069 7320 7468 6520 6d65   scale is the me
-00007f40: 616e 206f 6620 7468 6520 756e 6465 726c  an of the underl
-00007f50: 7969 6e67 206e 6f72 6d61 6c20 6469 7374  ying normal dist
-00007f60: 7269 6275 7469 6f6e 0a20 2020 2020 2020  ribution.       
-00007f70: 206e 6470 203d 206c 6f67 6e6f 726d 2e70   ndp = lognorm.p
-00007f80: 6466 2864 702c 733d 7369 7a65 5f64 6973  df(dp,s=size_dis
-00007f90: 7472 6962 7574 696f 6e5f 7369 676d 612c  tribution_sigma,
-00007fa0: 7363 616c 653d 7369 7a65 5f6d 7529 0a20  scale=size_mu). 
-00007fb0: 2020 2020 2020 2023 7072 696e 7428 2244         #print("D
-00007fc0: 5022 2c64 7029 0a20 2020 2020 2020 2023  P",dp).        #
-00007fd0: 7072 696e 7428 224e 4450 222c 6e64 7029  print("NDP",ndp)
-00007fe0: 0a20 2020 2020 2020 2023 7072 696e 7428  .        #print(
-00007ff0: 2255 7070 6572 206c 6f77 6572 222c 6c6f  "Upper lower",lo
-00008000: 7765 722c 7570 7065 7229 0a20 2020 2020  wer,upper).     
-00008010: 2020 2023 7072 696e 7428 2253 697a 655f     #print("Size_
-00008020: 4d55 222c 7369 7a65 5f6d 7529 0a20 2020  MU",size_mu).   
-00008030: 2023 2057 6520 6172 6520 6e6f 7720 676f   # We are now go
-00008040: 696e 6720 746f 2069 676e 6f72 6520 616e  ing to ignore an
-00008050: 7920 6f66 662d 6469 6167 6f6e 616c 2065  y off-diagonal e
-00008060: 6c65 6d65 6e74 730a 2020 2020 7472 6163  lements.    trac
-00008070: 6520 3d20 302e 300a 2020 2020 2320 4e6f  e = 0.0.    # No
-00008080: 7720 7461 6b65 2074 6865 2061 7665 7261  w take the avera
-00008090: 6765 206f 6620 6561 6368 2064 6972 6563  ge of each direc
-000080a0: 7469 6f6e 0a20 2020 2066 6f72 2069 6e64  tion.    for ind
-000080b0: 6578 2069 6e20 5b30 2c31 2c32 5d3a 0a20  ex in [0,1,2]:. 
-000080c0: 2020 2020 2020 2072 6566 7261 6374 6976         refractiv
-000080d0: 655f 696e 6465 7820 3d20 6361 6c63 756c  e_index = calcul
-000080e0: 6174 655f 7265 6672 6163 7469 7665 5f69  ate_refractive_i
-000080f0: 6e64 6578 5f73 6361 6c61 7228 726f 7461  ndex_scalar(rota
-00008100: 7465 645f 6469 656c 6563 5b69 6e64 6578  ted_dielec[index
-00008110: 2c69 6e64 6578 5d29 202f 2072 6566 7261  ,index]) / refra
-00008120: 6374 6976 655f 696e 6465 785f 6d65 6469  ctive_index_medi
-00008130: 756d 0a20 2020 2020 2020 2023 6a6b 2070  um.        #jk p
-00008140: 7269 6e74 2827 7265 6672 6163 7469 7665  rint('refractive
-00008150: 5f69 6e64 6578 272c 2072 6566 7261 6374  _index', refract
-00008160: 6976 655f 696e 6465 7829 0a20 2020 2020  ive_index).     
-00008170: 2020 2023 6a6b 2070 7269 6e74 2827 7265     #jk print('re
-00008180: 6672 6163 7469 7665 5f69 6e64 6578 5f6d  fractive_index_m
-00008190: 6564 6975 6d27 2c20 7265 6672 6163 7469  edium', refracti
-000081a0: 7665 5f69 6e64 6578 5f6d 6564 6975 6d29  ve_index_medium)
-000081b0: 0a20 2020 2020 2020 2023 6a6b 2070 7269  .        #jk pri
-000081c0: 6e74 2827 726f 7461 7465 645f 6469 656c  nt('rotated_diel
-000081d0: 6563 272c 2072 6f74 6174 6564 5f64 6965  ec', rotated_die
-000081e0: 6c65 635b 696e 6465 782c 696e 6465 785d  lec[index,index]
-000081f0: 290a 2020 2020 2020 2020 6966 2073 697a  ).        if siz
-00008200: 655f 6469 7374 7269 6275 7469 6f6e 5f73  e_distribution_s
-00008210: 6967 6d61 3a0a 2020 2020 2020 2020 2020  igma:.          
-00008220: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
-00008230: 6520 696e 7465 6772 616c 206f 6620 7468  e integral of th
-00008240: 6520 666f 7277 6172 6420 7363 6174 7465  e forward scatte
-00008250: 7269 6e67 2066 6163 746f 7273 206f 7665  ring factors ove
-00008260: 7220 7468 6520 6469 7374 7269 6275 7469  r the distributi
-00008270: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
-00008280: 315f 6661 6374 6f72 7320 3d20 5b5d 0a20  1_factors = []. 
-00008290: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-000082a0: 2069 6e20 6470 3a0a 2020 2020 2020 2020   in dp:.        
-000082b0: 2020 2020 2020 2020 2320 5468 6520 7369          # The si
-000082c0: 7a65 2070 6172 616d 6574 6572 2069 7320  ze parameter is 
-000082d0: 3270 6920 7220 2f20 6c61 6d62 6461 0a20  2pi r / lambda. 
-000082e0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-000082f0: 203d 2032 202a 2050 4920 2a20 7220 2f20   = 2 * PI * r / 
-00008300: 6c61 6d62 6461 5f76 6163 7575 6d5f 6d75  lambda_vacuum_mu
-00008310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008320: 2023 2043 616c 6375 6c61 7465 2074 6865   # Calculate the
-00008330: 2053 3120 616e 6420 5332 2073 6361 7474   S1 and S2 scatt
-00008340: 6572 696e 6720 6661 6374 6f72 732c 2061  ering factors, a
-00008350: 6e64 2073 746f 7265 2069 6e20 6120 6c69  nd store in a li
-00008360: 7374 0a20 2020 2020 2020 2020 2020 2020  st.             
-00008370: 2020 2073 312c 7332 203d 204d 6965 2e4d     s1,s2 = Mie.M
-00008380: 6965 5331 5332 2872 6566 7261 6374 6976  ieS1S2(refractiv
-00008390: 655f 696e 6465 782c 2078 2a72 6566 7261  e_index, x*refra
-000083a0: 6374 6976 655f 696e 6465 785f 6d65 6469  ctive_index_medi
-000083b0: 756d 2c20 3129 0a20 2020 2020 2020 2020  um, 1).         
-000083c0: 2020 2020 2020 2073 315f 6661 6374 6f72         s1_factor
-000083d0: 732e 6170 7065 6e64 2873 3129 0a20 2020  s.append(s1).   
-000083e0: 2020 2020 2020 2020 2023 204e 6f77 2069           # Now i
-000083f0: 6e74 6567 7261 7465 0a20 2020 2020 2020  ntegrate.       
-00008400: 2020 2020 2073 3120 3d20 7472 6170 7a28       s1 = trapz(
-00008410: 7331 5f66 6163 746f 7273 2a6e 6470 2c64  s1_factors*ndp,d
-00008420: 7029 0a20 2020 2020 2020 2020 2020 206e  p).            n
-00008430: 6f72 6d61 6c20 3d20 7472 6170 7a28 6e64  ormal = trapz(nd
-00008440: 702c 6470 290a 2020 2020 2020 2020 2020  p,dp).          
-00008450: 2020 236d 6561 6e20 3d20 7472 6170 7a28    #mean = trapz(
-00008460: 6e64 702a 6470 2c64 7029 0a20 2020 2020  ndp*dp,dp).     
-00008470: 2020 2020 2020 2023 7472 7565 5f6d 6561         #true_mea
-00008480: 6e20 3d20 6e70 2e65 7870 2820 6e70 2e6c  n = np.exp( np.l
-00008490: 6f67 2873 697a 655f 6d75 2920 2b20 7369  og(size_mu) + si
-000084a0: 7a65 5f64 6973 7472 6962 7574 696f 6e5f  ze_distribution_
-000084b0: 7369 676d 612a 7369 7a65 5f64 6973 7472  sigma*size_distr
-000084c0: 6962 7574 696f 6e5f 7369 676d 612f 322e  ibution_sigma/2.
-000084d0: 3029 0a20 2020 2020 2020 2020 2020 2023  0).            #
-000084e0: 765f 636d 3120 3d20 312e 3045 342f 6c61  v_cm1 = 1.0E4/la
-000084f0: 6d62 6461 5f76 6163 7575 6d5f 6d75 0a20  mbda_vacuum_mu. 
-00008500: 2020 2020 2020 2020 2020 2023 7072 696e             #prin
-00008510: 7428 2246 7265 7175 656e 6379 2c6e 6f72  t("Frequency,nor
-00008520: 6d61 6c2c 6d65 616e 222c 765f 636d 312c  mal,mean",v_cm1,
-00008530: 6e6f 726d 616c 2c74 7275 655f 6d65 616e  normal,true_mean
-00008540: 2c6d 6561 6e29 0a20 2020 2020 2020 2020  ,mean).         
-00008550: 2020 2069 6620 6e70 2e61 6273 286e 6f72     if np.abs(nor
-00008560: 6d61 6c20 2d20 312e 3029 203e 2031 2e30  mal - 1.0) > 1.0
-00008570: 452d 323a 0a20 2020 2020 2020 2020 2020  E-2:.           
-00008580: 2020 2020 2070 7269 6e74 2822 5761 726e       print("Warn
-00008590: 696e 6720 696e 7465 6772 6174 696f 6e20  ing integration 
-000085a0: 6f66 206c 6f67 2d6e 6f72 6d61 6c20 6469  of log-normal di
-000085b0: 7374 7269 6275 7469 6f6e 2069 6e20 6572  stribution in er
-000085c0: 726f 7222 2c20 6e6f 726d 616c 290a 2020  ror", normal).  
-000085d0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000085e0: 696e 7428 2253 746f 7070 696e 6720 6361  int("Stopping ca
-000085f0: 6c63 756c 6174 696f 6e20 2d20 6c69 6b65  lculation - like
-00008600: 6c79 2070 726f 626c 656d 2069 7320 746f  ly problem is to
-00008610: 6f20 6c61 7267 6520 6120 7369 676d 6120  o large a sigma 
-00008620: 666f 7220 6c6f 672d 6e6f 726d 616c 2064  for log-normal d
-00008630: 6973 7472 6962 7574 696f 6e22 290a 2020  istribution").  
-00008640: 2020 2020 2020 2020 2020 2020 2020 6566                ef
-00008650: 6664 6965 6c65 6320 3d20 6e70 2e61 7272  fdielec = np.arr
-00008660: 6179 285b 5b31 2c20 302c 2030 5d2c 205b  ay([[1, 0, 0], [
-00008670: 302c 2031 2c20 305d 2c20 5b30 2c20 302c  0, 1, 0], [0, 0,
-00008680: 2031 5d5d 290a 2020 2020 2020 2020 2020   1]]).          
-00008690: 2020 2020 2020 7265 7475 726e 2065 6666        return eff
-000086a0: 6469 656c 6563 0a20 2020 2020 2020 2065  dielec.        e
-000086b0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000086c0: 2023 2043 616c 6375 6c61 7465 2074 6865   # Calculate the
-000086d0: 2073 6361 7474 6572 696e 6720 6661 6374   scattering fact
-000086e0: 6f72 7320 6174 2030 2064 6567 7265 6573  ors at 0 degrees
-000086f0: 0a20 2020 2020 2020 2020 2020 2023 6a6b  .            #jk
-00008700: 2070 7269 6e74 2822 7265 6672 6163 7469   print("refracti
-00008710: 7665 5f69 6e64 6578 2c20 7369 7a65 2c20  ve_index, size, 
-00008720: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
-00008730: 5f6d 6564 6975 6d22 2c20 7265 6672 6163  _medium", refrac
-00008740: 7469 7665 5f69 6e64 6578 2c20 7369 7a65  tive_index, size
-00008750: 2c20 7265 6672 6163 7469 7665 5f69 6e64  , refractive_ind
-00008760: 6578 5f6d 6564 6975 6d29 0a20 2020 2020  ex_medium).     
-00008770: 2020 2020 2020 2073 312c 7332 203d 204d         s1,s2 = M
-00008780: 6965 2e4d 6965 5331 5332 2872 6566 7261  ie.MieS1S2(refra
-00008790: 6374 6976 655f 696e 6465 782c 2073 697a  ctive_index, siz
-000087a0: 652a 7265 6672 6163 7469 7665 5f69 6e64  e*refractive_ind
-000087b0: 6578 5f6d 6564 6975 6d2c 2031 290a 2020  ex_medium, 1).  
-000087c0: 2020 2020 2020 2320 5365 6520 7661 6e20        # See van 
-000087d0: 6465 2048 756c 7374 2070 6167 6520 3132  de Hulst page 12
-000087e0: 392c 2031 3330 0a20 2020 2020 2020 2023  9, 130.        #
-000087f0: 2052 6566 7261 6374 6976 6520 696e 6465   Refractive inde
-00008800: 7820 6f66 206d 6174 6572 6961 6c20 6973  x of material is
-00008810: 0a20 2020 2020 2020 2023 2074 6865 2073  .        # the s
-00008820: 6967 6e20 6f66 2074 6865 2069 6d61 6769  ign of the imagi
-00008830: 6e61 7279 2063 6f6d 706f 6e65 6e74 2068  nary component h
-00008840: 6173 2063 6861 6e67 6564 2066 6f72 2063  as changed for c
-00008850: 6f6d 7061 7469 6269 6c69 7479 2077 6974  ompatibility wit
-00008860: 6820 4d47 2f42 7275 6767 656d 616e 0a20  h MG/Bruggeman. 
-00008870: 2020 2020 2020 2072 6566 7261 6374 6976         refractiv
-00008880: 655f 696e 6465 7820 3d20 7265 6672 6163  e_index = refrac
-00008890: 7469 7665 5f69 6e64 6578 5f6d 6564 6975  tive_index_mediu
-000088a0: 6d20 2a20 2820 312e 3020 2b20 6920 2a20  m * ( 1.0 + i * 
-000088b0: 7331 202a 2032 202a 2050 4920 2a20 4e5f  s1 * 2 * PI * N_
-000088c0: 6e6d 202f 2028 206b 5f6e 6d20 2a20 6b5f  nm / ( k_nm * k_
-000088d0: 6e6d 202a 206b 5f6e 6d20 2920 290a 2020  nm * k_nm ) ).  
-000088e0: 2020 2020 2020 7472 6163 6520 2b3d 2072        trace += r
-000088f0: 6566 7261 6374 6976 655f 696e 6465 780a  efractive_index.
-00008900: 2020 2020 2320 7265 7475 726e 2061 6e20      # return an 
-00008910: 6973 6f74 726f 7069 6320 7465 6e73 6f72  isotropic tensor
-00008920: 0a20 2020 2074 7261 6365 203d 2074 7261  .    trace = tra
-00008930: 6365 202f 2033 2e30 0a20 2020 2065 6666  ce / 3.0.    eff
-00008940: 203d 2074 7261 6365 202a 2074 7261 6365   = trace * trace
-00008950: 0a20 2020 2065 6666 6469 656c 6563 203d  .    effdielec =
-00008960: 206e 702e 6172 7261 7928 5b5b 6566 662c   np.array([[eff,
-00008970: 2030 2c20 305d 2c20 5b30 2c20 6566 662c   0, 0], [0, eff,
-00008980: 2030 5d2c 205b 302c 2030 2c20 6566 665d   0], [0, 0, eff]
-00008990: 5d29 0a20 2020 2023 6a6b 2070 7269 6e74  ]).    #jk print
-000089a0: 2872 6164 6975 735f 6e6d 2c20 6c61 6d62  (radius_nm, lamb
-000089b0: 6461 5f76 6163 7575 6d5f 6d75 2a31 3030  da_vacuum_mu*100
-000089c0: 302e 302c 2071 6578 742c 7173 6361 2c71  0.0, qext,qsca,q
-000089d0: 6162 732c 672c 7170 722c 7162 6163 6b2c  abs,g,qpr,qback,
-000089e0: 7172 6174 696f 2c6e 702e 7265 616c 2873  qratio,np.real(s
-000089f0: 3129 2c6e 702e 696d 6167 2873 3129 2c6e  1),np.imag(s1),n
-00008a00: 702e 7265 616c 2874 7261 6365 292c 6e70  p.real(trace),np
-00008a10: 2e69 6d61 6728 7472 6163 6529 2c6e 702e  .imag(trace),np.
-00008a20: 7265 616c 2865 6666 292c 6e70 2e69 6d61  real(eff),np.ima
-00008a30: 6728 6566 6629 290a 2020 2020 2370 7269  g(eff)).    #pri
-00008a40: 6e74 2028 2272 6164 6975 735f 6e6d 2c20  nt ("radius_nm, 
-00008a50: 6566 6622 2c20 7261 6469 7573 5f6e 6d2c  eff", radius_nm,
-00008a60: 2065 6666 290a 2020 2020 7265 7475 726e   eff).    return
-00008a70: 2065 6666 6469 656c 6563 0a0a 6465 6620   effdielec..def 
-00008a80: 6d61 7877 656c 6c28 6469 656c 6563 7472  maxwell(dielectr
-00008a90: 6963 5f6d 6564 6975 6d2c 2063 7279 7374  ic_medium, cryst
-00008aa0: 616c 5f70 6572 6d69 7474 6976 6974 792c  al_permittivity,
-00008ab0: 2073 6861 7065 2c20 4c2c 2076 662c 2073   shape, L, vf, s
-00008ac0: 697a 6529 3a0a 2020 2020 2222 2243 616c  ize):.    """Cal
-00008ad0: 6375 6c61 7465 2074 6865 2065 6666 6563  culate the effec
-00008ae0: 7469 7665 2063 6f6e 7374 616e 7420 7065  tive constant pe
-00008af0: 726d 6974 7469 7669 7479 2075 7369 6e67  rmittivity using
-00008b00: 2074 6865 206d 6178 7765 6c6c 2067 6172   the maxwell gar
-00008b10: 6e65 7474 206d 6574 686f 640a 2020 2020  nett method.    
-00008b20: 2020 2064 6965 6c65 6374 7269 635f 6d65     dielectric_me
-00008b30: 6469 756d 2069 7320 7468 6520 6469 656c  dium is the diel
-00008b40: 6563 7472 6963 2063 6f6e 7374 616e 7420  ectric constant 
-00008b50: 7465 6e73 6f72 206f 6620 7468 6520 6d65  tensor of the me
-00008b60: 6469 756d 0a20 2020 2020 2020 6372 7973  dium.       crys
-00008b70: 7461 6c5f 7065 726d 6974 7469 7669 7479  tal_permittivity
-00008b80: 2069 7320 7468 6520 746f 7461 6c20 6672   is the total fr
-00008b90: 6571 7565 6e63 7920 6469 656c 6563 7472  equency dielectr
-00008ba0: 6963 2063 6f6e 7374 616e 7420 7465 6e73  ic constant tens
-00008bb0: 6f72 2061 7420 7468 6520 6375 7272 656e  or at the curren
-00008bc0: 7420 6672 6571 7565 6e63 790a 2020 2020  t frequency.    
-00008bd0: 2020 2073 6861 7065 2069 7320 7468 6520     shape is the 
-00008be0: 6e61 6d65 206f 6620 7468 6520 6375 7272  name of the curr
-00008bf0: 656e 7420 7368 6170 650a 2020 2020 2020  ent shape.      
-00008c00: 204c 2069 7320 7468 6520 7368 6170 6573   L is the shapes
-00008c10: 2064 6570 6f6c 6172 6973 6174 696f 6e20   depolarisation 
-00008c20: 6d61 7472 6978 0a20 2020 2020 2020 7369  matrix.       si
-00008c30: 7a65 2069 7320 7468 6520 6469 6d65 6e73  ze is the dimens
-00008c40: 696f 6e6c 6573 7320 7369 7a65 2070 6172  ionless size par
-00008c50: 616d 6574 6572 2066 6f72 2074 6865 2066  ameter for the f
-00008c60: 7265 7175 656e 6379 2075 6e64 6572 2063  requency under c
-00008c70: 6f6e 7369 6465 7261 7469 6f6e 0a20 2020  onsideration.   
-00008c80: 2020 2020 7666 2069 7320 7468 6520 766f      vf is the vo
-00008c90: 6c75 6d65 2066 7261 6374 696f 6e20 6f66  lume fraction of
-00008ca0: 2066 696c 6c65 720a 2020 2020 2020 2054   filler.       T
-00008cb0: 6865 2072 6f75 7469 6e65 2072 6574 7572  he routine retur
-00008cc0: 6e73 2074 6865 2065 6666 6563 7469 7665  ns the effective
-00008cd0: 2064 6965 6c65 6374 7269 6320 636f 6e73   dielectric cons
-00008ce0: 7461 6e74 2222 220a 2020 2020 756e 6974  tant""".    unit
-00008cf0: 203d 2069 6e69 7469 616c 6973 655f 756e   = initialise_un
-00008d00: 6974 5f74 656e 736f 7228 290a 2020 2020  it_tensor().    
-00008d10: 656d 6564 6975 6d20 3d20 6e70 2e74 7261  emedium = np.tra
-00008d20: 6365 2864 6965 6c65 6374 7269 635f 6d65  ce(dielectric_me
-00008d30: 6469 756d 2920 2f20 332e 300a 2020 2020  dium) / 3.0.    
-00008d40: 2320 4966 2061 7070 726f 7072 6961 7465  # If appropriate
-00008d50: 2063 616c 6375 6c61 7465 2061 2073 697a   calculate a siz
-00008d60: 6520 6566 6665 6374 2075 7369 6e67 2045  e effect using E
-00008d70: 7175 6174 696f 6e73 2031 302e 3338 2061  quations 10.38 a
-00008d80: 6e64 2031 302e 3339 2069 6e20 5369 6876  nd 10.39 in Sihv
-00008d90: 6f6c 610a 2020 2020 7369 7a65 5f66 6163  ola.    size_fac
-00008da0: 746f 7220 3d20 6361 6c63 756c 6174 655f  tor = calculate_
-00008db0: 7369 7a65 5f66 6163 746f 7228 7369 7a65  size_factor(size
-00008dc0: 290a 2020 2020 2320 4571 7561 7469 6f6e  ).    # Equation
-00008dd0: 2035 2e37 3820 696e 2053 6968 766f 6c61   5.78 in Sihvola
-00008de0: 0a20 2020 206e 616c 7068 6120 3d20 656d  .    nalpha = em
-00008df0: 6564 6975 6d2a 7666 2a6e 702e 646f 7428  edium*vf*np.dot(
-00008e00: 2863 7279 7374 616c 5f70 6572 6d69 7474  (crystal_permitt
-00008e10: 6976 6974 7920 2d20 6469 656c 6563 7472  ivity - dielectr
-00008e20: 6963 5f6d 6564 6975 6d29 2c20 6e70 2e6c  ic_medium), np.l
-00008e30: 696e 616c 672e 696e 7628 6469 656c 6563  inalg.inv(dielec
-00008e40: 7472 6963 5f6d 6564 6975 6d20 2b20 7369  tric_medium + si
-00008e50: 7a65 5f66 6163 746f 7220 2a20 6e70 2e64  ze_factor * np.d
-00008e60: 6f74 284c 2c20 2863 7279 7374 616c 5f70  ot(L, (crystal_p
-00008e70: 6572 6d69 7474 6976 6974 792d 6469 656c  ermittivity-diel
-00008e80: 6563 7472 6963 5f6d 6564 6975 6d29 2929  ectric_medium)))
-00008e90: 290a 2020 2020 6e61 6c70 6861 6c20 3d20  ).    nalphal = 
-00008ea0: 6e70 2e64 6f74 2828 6e61 6c70 6861 2f65  np.dot((nalpha/e
-00008eb0: 6d65 6469 756d 292c 204c 290a 2020 2020  medium), L).    
-00008ec0: 2320 6176 6572 6167 6520 7468 6520 706f  # average the po
-00008ed0: 6c61 7269 7361 6269 6c69 7479 206f 7665  larisability ove
-00008ee0: 7220 6f72 6965 6e74 6174 696f 6e0a 2020  r orientation.  
-00008ef0: 2020 6e61 6c70 6861 203d 206e 702e 7472    nalpha = np.tr
-00008f00: 6163 6528 6e61 6c70 6861 2920 2f20 332e  ace(nalpha) / 3.
-00008f10: 3020 2a20 756e 6974 0a20 2020 2023 2061  0 * unit.    # a
-00008f20: 7665 7261 6765 2074 6865 2070 6f6c 6172  verage the polar
-00008f30: 6973 6162 696c 6974 792a 4c20 6f76 6572  isability*L over
-00008f40: 206f 7269 656e 7461 7469 6f6e 0a20 2020   orientation.   
-00008f50: 206e 616c 7068 616c 203d 206e 702e 7472   nalphal = np.tr
-00008f60: 6163 6528 6e61 6c70 6861 6c29 202f 2033  ace(nalphal) / 3
-00008f70: 2e30 202a 2075 6e69 740a 2020 2020 706f  .0 * unit.    po
-00008f80: 6c61 7269 7361 7469 6f6e 203d 206e 702e  larisation = np.
-00008f90: 646f 7428 6e70 2e6c 696e 616c 672e 696e  dot(np.linalg.in
-00008fa0: 7628 756e 6974 202d 206e 616c 7068 616c  v(unit - nalphal
-00008fb0: 292c 206e 616c 7068 6129 0a20 2020 2065  ), nalpha).    e
-00008fc0: 6666 6420 2020 2020 2020 2020 3d20 6469  ffd         = di
-00008fd0: 656c 6563 7472 6963 5f6d 6564 6975 6d20  electric_medium 
-00008fe0: 2b20 706f 6c61 7269 7361 7469 6f6e 0a20  + polarisation. 
-00008ff0: 2020 2074 7261 6365 203d 206e 702e 7472     trace = np.tr
-00009000: 6163 6528 6566 6664 2920 2f20 332e 300a  ace(effd) / 3.0.
-00009010: 2020 2020 6566 6664 6965 6c65 6320 3d20      effdielec = 
-00009020: 6e70 2e61 7272 6179 285b 5b74 7261 6365  np.array([[trace
-00009030: 2c20 302c 2030 5d2c 205b 302c 2074 7261  , 0, 0], [0, tra
-00009040: 6365 2c20 305d 2c20 5b30 2c20 302c 2074  ce, 0], [0, 0, t
-00009050: 7261 6365 5d5d 290a 2020 2020 7265 7475  race]]).    retu
-00009060: 726e 2065 6666 6469 656c 6563 0a0a 6465  rn effdielec..de
-00009070: 6620 6d61 7877 656c 6c5f 7369 6876 6f6c  f maxwell_sihvol
-00009080: 6128 6469 656c 6563 7472 6963 5f6d 6564  a(dielectric_med
-00009090: 6975 6d2c 2063 7279 7374 616c 5f70 6572  ium, crystal_per
-000090a0: 6d69 7474 6976 6974 792c 2073 6861 7065  mittivity, shape
-000090b0: 2c20 4c2c 2076 662c 2073 697a 6529 3a0a  , L, vf, size):.
-000090c0: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
-000090d0: 2074 6865 2065 6666 6563 7469 7665 2063   the effective c
-000090e0: 6f6e 7374 616e 7420 7065 726d 6974 7469  onstant permitti
-000090f0: 7669 7479 2075 7369 6e67 2074 6865 206d  vity using the m
-00009100: 6178 7765 6c6c 2067 6172 6e65 7474 206d  axwell garnett m
-00009110: 6574 686f 640a 2020 2020 2020 2064 6965  ethod.       die
-00009120: 6c65 6374 7269 635f 6d65 6469 756d 2069  lectric_medium i
-00009130: 7320 7468 6520 6469 656c 6563 7472 6963  s the dielectric
-00009140: 2063 6f6e 7374 616e 7420 7465 6e73 6f72   constant tensor
-00009150: 206f 6620 7468 6520 6d65 6469 756d 0a20   of the medium. 
-00009160: 2020 2020 2020 6372 7973 7461 6c5f 7065        crystal_pe
-00009170: 726d 6974 7469 7669 7479 2069 7320 7468  rmittivity is th
-00009180: 6520 746f 7461 6c20 6672 6571 7565 6e63  e total frequenc
-00009190: 7920 6469 656c 6563 7472 6963 2063 6f6e  y dielectric con
-000091a0: 7374 616e 7420 7465 6e73 6f72 2061 7420  stant tensor at 
-000091b0: 7468 6520 6375 7272 656e 7420 6672 6571  the current freq
-000091c0: 7565 6e63 790a 2020 2020 2020 2073 6861  uency.       sha
-000091d0: 7065 2069 7320 7468 6520 6e61 6d65 206f  pe is the name o
-000091e0: 6620 7468 6520 6375 7272 656e 7420 7368  f the current sh
-000091f0: 6170 650a 2020 2020 2020 204c 2069 7320  ape.       L is 
-00009200: 7468 6520 7368 6170 6573 2064 6570 6f6c  the shapes depol
-00009210: 6172 6973 6174 696f 6e20 6d61 7472 6978  arisation matrix
-00009220: 0a20 2020 2020 2020 7369 7a65 2069 7320  .       size is 
-00009230: 7468 6520 6469 6d65 6e73 696f 6e6c 6573  the dimensionles
-00009240: 7320 7369 7a65 2070 6172 616d 6574 6572  s size parameter
-00009250: 2066 6f72 2074 6865 2066 7265 7175 656e   for the frequen
-00009260: 6379 2075 6e64 6572 2063 6f6e 7369 6465  cy under conside
-00009270: 7261 7469 6f6e 0a20 2020 2020 2020 7666  ration.       vf
-00009280: 2069 7320 7468 6520 766f 6c75 6d65 2066   is the volume f
-00009290: 7261 6374 696f 6e20 6f66 2066 696c 6c65  raction of fille
-000092a0: 720a 2020 2020 2020 2054 6865 2072 6f75  r.       The rou
-000092b0: 7469 6e65 2072 6574 7572 6e73 2074 6865  tine returns the
-000092c0: 2065 6666 6563 7469 7665 2064 6965 6c65   effective diele
-000092d0: 6374 7269 6320 636f 6e73 7461 6e74 2222  ctric constant""
-000092e0: 220a 2020 2020 756e 6974 203d 2069 6e69  ".    unit = ini
-000092f0: 7469 616c 6973 655f 756e 6974 5f74 656e  tialise_unit_ten
-00009300: 736f 7228 290a 2020 2020 2320 4571 7561  sor().    # Equa
-00009310: 7469 6f6e 2036 2e32 3920 6f6e 2070 6167  tion 6.29 on pag
-00009320: 6520 3132 3320 6f66 2053 6968 766f 6c61  e 123 of Sihvola
-00009330: 0a20 2020 2023 2045 7175 6174 696f 6e20  .    # Equation 
-00009340: 362e 3430 2067 6976 6573 2074 6865 2061  6.40 gives the a
-00009350: 7665 7261 6769 6e67 206f 7665 7220 7468  veraging over th
-00009360: 6520 6f72 6965 6e74 6174 696f 6e20 6675  e orientation fu
-00009370: 6e63 7469 6f6e 0a20 2020 2023 2053 6565  nction.    # See
-00009380: 2061 6c73 6f20 6571 7561 7469 6f6e 2035   also equation 5
-00009390: 2e38 3020 6f6e 2070 6167 6520 3130 3220  .80 on page 102 
-000093a0: 616e 6420 6571 7561 7469 6f6e 2034 2e33  and equation 4.3
-000093b0: 3120 6f6e 2070 6167 6520 3730 0a20 2020  1 on page 70.   
-000093c0: 204d 6520 3d20 6469 656c 6563 7472 6963   Me = dielectric
-000093d0: 5f6d 6564 6975 6d0a 2020 2020 2320 6173  _medium.    # as
-000093e0: 7375 6d65 2074 6861 7420 7468 6520 6d65  sume that the me
-000093f0: 6469 756d 2069 7320 6973 6f74 726f 7069  dium is isotropi
-00009400: 6320 6361 6c63 756c 6174 6520 7468 6520  c calculate the 
-00009410: 696e 7665 7273 6520 6f66 2074 6865 2064  inverse of the d
-00009420: 6965 6c65 6374 7269 630a 2020 2020 4d65  ielectric.    Me
-00009430: 6d31 203d 2033 2e30 202f 206e 702e 7472  m1 = 3.0 / np.tr
-00009440: 6163 6528 4d65 290a 2020 2020 4d69 203d  ace(Me).    Mi =
-00009450: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
-00009460: 6976 6974 790a 2020 2020 2320 4966 2061  ivity.    # If a
-00009470: 7070 726f 7072 6961 7465 2063 616c 6375  ppropriate calcu
-00009480: 6c61 7465 2061 2073 697a 6520 6566 6665  late a size effe
-00009490: 6374 2075 7369 6e67 2045 7175 6174 696f  ct using Equatio
-000094a0: 6e73 2031 302e 3338 2061 6e64 2031 302e  ns 10.38 and 10.
-000094b0: 3339 2069 6e20 5369 6876 6f6c 610a 2020  39 in Sihvola.  
-000094c0: 2020 7369 7a65 5f66 6163 746f 7220 3d20    size_factor = 
-000094d0: 6361 6c63 756c 6174 655f 7369 7a65 5f66  calculate_size_f
-000094e0: 6163 746f 7228 7369 7a65 290a 2020 2020  actor(size).    
-000094f0: 2320 6361 6c63 756c 6174 6520 7468 6520  # calculate the 
-00009500: 706f 6c61 7269 7361 6269 6c69 7479 206d  polarisability m
-00009510: 6174 7269 7820 7820 7468 6520 6e75 6d62  atrix x the numb
-00009520: 6572 2064 656e 7369 7479 206f 6620 696e  er density of in
-00009530: 636c 7573 696f 6e73 0a20 2020 206e 4120  clusions.    nA 
-00009540: 3d20 7666 2a6e 702e 646f 7428 284d 692d  = vf*np.dot((Mi-
-00009550: 4d65 292c 206e 702e 6c69 6e61 6c67 2e69  Me), np.linalg.i
-00009560: 6e76 2875 6e69 7420 2b20 2873 697a 655f  nv(unit + (size_
-00009570: 6661 6374 6f72 202a 204d 656d 3120 2a20  factor * Mem1 * 
-00009580: 6e70 2e64 6f74 284c 2c20 284d 6920 2d20  np.dot(L, (Mi - 
-00009590: 4d65 2929 2929 290a 2020 2020 6e41 4c20  Me))))).    nAL 
-000095a0: 3d20 6e70 2e64 6f74 2828 6e41 292c 204c  = np.dot((nA), L
-000095b0: 290a 2020 2020 2320 6176 6572 6167 6520  ).    # average 
-000095c0: 7468 6520 706f 6c61 7269 7361 6269 6c69  the polarisabili
-000095d0: 7479 206f 7665 7220 6f72 6965 6e74 6174  ty over orientat
-000095e0: 696f 6e0a 2020 2020 6e41 203d 206e 702e  ion.    nA = np.
-000095f0: 7472 6163 6528 6e41 2920 2f20 332e 3020  trace(nA) / 3.0 
-00009600: 2a20 756e 6974 0a20 2020 2023 2061 7665  * unit.    # ave
-00009610: 7261 6765 2074 6865 2070 6f6c 6172 6973  rage the polaris
-00009620: 6162 696c 6974 792a 4c20 6f76 6572 206f  ability*L over o
-00009630: 7269 656e 7461 7469 6f6e 0a20 2020 206e  rientation.    n
-00009640: 414c 203d 206e 702e 7472 6163 6528 6e41  AL = np.trace(nA
-00009650: 4c29 202f 2033 2e30 202a 204d 656d 3120  L) / 3.0 * Mem1 
-00009660: 2a20 756e 6974 0a20 2020 2023 2043 616c  * unit.    # Cal
-00009670: 6375 6c61 7465 2074 6865 2061 7665 7261  culate the avera
-00009680: 6765 2070 6f6c 6172 6973 6174 696f 6e20  ge polarisation 
-00009690: 6661 6374 6f72 2077 6869 6368 2073 6361  factor which sca
-000096a0: 6c65 7320 7468 6520 6176 6572 6167 6520  les the average 
-000096b0: 6669 656c 640a 2020 2020 2320 6261 7365  field.    # base
-000096c0: 6420 6f6e 2065 7175 6174 696f 6e20 352e  d on equation 5.
-000096d0: 3830 0a20 2020 2023 203c 503e 203d 2070  80.    # <P> = p
-000096e0: 6f6c 202e 203c 453e 0a20 2020 2070 6f6c  ol . <E>.    pol
-000096f0: 203d 206e 702e 646f 7428 6e70 2e6c 696e   = np.dot(np.lin
-00009700: 616c 672e 696e 7628 756e 6974 202d 206e  alg.inv(unit - n
-00009710: 414c 292c 206e 4129 0a20 2020 2023 204d  AL), nA).    # M
-00009720: 6566 6620 2e20 3c45 3e20 3d20 4d65 202e  eff . <E> = Me .
-00009730: 203c 453e 202b 203c 503e 0a20 2020 2023   <E> + <P>.    #
-00009740: 204d 6566 6620 2e20 3c45 3e20 3d20 4d65   Meff . <E> = Me
-00009750: 2e20 3c45 3e20 2b20 706f 6c20 2e20 3c45  . <E> + pol . <E
-00009760: 3e0a 2020 2020 2320 4d65 6666 203d 204d  >.    # Meff = M
-00009770: 6520 2b20 706f 6c0a 2020 2020 6566 6664  e + pol.    effd
-00009780: 2020 2020 2020 2020 203d 2064 6965 6c65           = diele
-00009790: 6374 7269 635f 6d65 6469 756d 202b 2070  ctric_medium + p
-000097a0: 6f6c 0a20 2020 2023 2041 7665 7261 6765  ol.    # Average
-000097b0: 206f 7665 7220 6f72 6965 6e74 6174 696f   over orientatio
-000097c0: 6e0a 2020 2020 7472 6163 6520 3d20 6e70  n.    trace = np
-000097d0: 2e74 7261 6365 2865 6666 6429 202f 2033  .trace(effd) / 3
-000097e0: 2e30 0a20 2020 2065 6666 6469 656c 6563  .0.    effdielec
-000097f0: 203d 206e 702e 6172 7261 7928 5b5b 7472   = np.array([[tr
-00009800: 6163 652c 2030 2c20 305d 2c20 5b30 2c20  ace, 0, 0], [0, 
-00009810: 7472 6163 652c 2030 5d2c 205b 302c 2030  trace, 0], [0, 0
-00009820: 2c20 7472 6163 655d 5d29 0a20 2020 2072  , trace]]).    r
-00009830: 6574 7572 6e20 6566 6664 6965 6c65 630a  eturn effdielec.
-00009840: 0a64 6566 2063 6f68 6572 656e 7428 6469  .def coherent(di
-00009850: 656c 6563 7472 6963 5f6d 6564 6975 6d2c  electric_medium,
-00009860: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
-00009870: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
-00009880: 2076 662c 2073 697a 652c 2064 6965 6c65   vf, size, diele
-00009890: 6374 7269 635f 6170 7061 7265 6e74 293a  ctric_apparent):
-000098a0: 0a20 2020 2022 2222 4472 6976 6572 2066  .    """Driver f
-000098b0: 6f72 2063 6f68 6572 656e 7432 206d 6574  or coherent2 met
-000098c0: 686f 6422 2222 0a20 2020 2066 6f72 2069  hod""".    for i
-000098d0: 2069 6e20 7261 6e67 6528 3130 293a 0a20   in range(10):. 
-000098e0: 2020 2020 2020 2064 6965 6c65 6374 7269         dielectri
-000098f0: 635f 6170 7061 7265 6e74 203d 2030 2e31  c_apparent = 0.1
-00009900: 202a 2064 6965 6c65 6374 7269 635f 6170   * dielectric_ap
-00009910: 7061 7265 6e74 202b 2030 2e39 202a 2063  parent + 0.9 * c
-00009920: 6f68 6572 656e 7432 2864 6965 6c65 6374  oherent2(dielect
-00009930: 7269 635f 6d65 6469 756d 2c20 6469 656c  ric_medium, diel
-00009940: 6563 7472 6963 5f61 7070 6172 656e 742c  ectric_apparent,
-00009950: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
-00009960: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
-00009970: 2076 662c 2073 697a 6529 0a20 2020 2072   vf, size).    r
-00009980: 6574 7572 6e20 6469 656c 6563 7472 6963  eturn dielectric
-00009990: 5f61 7070 6172 656e 740a 0a64 6566 2063  _apparent..def c
-000099a0: 6f68 6572 656e 7432 2864 6965 6c65 6374  oherent2(dielect
-000099b0: 7269 635f 6d65 6469 756d 2c20 6469 656c  ric_medium, diel
-000099c0: 6563 7472 6963 5f61 7070 6172 656e 742c  ectric_apparent,
-000099d0: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
-000099e0: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
-000099f0: 2076 662c 2073 697a 6529 3a0a 2020 2020   vf, size):.    
-00009a00: 2222 2243 616c 6375 6c61 7465 2074 6865  """Calculate the
-00009a10: 2065 6666 6563 7469 7665 2063 6f6e 7374   effective const
-00009a20: 616e 7420 7065 726d 6974 7469 7669 7479  ant permittivity
-00009a30: 2075 7369 6e67 2074 6865 206d 6178 7765   using the maxwe
-00009a40: 6c6c 2067 6172 6e65 7474 206d 6574 686f  ll garnett metho
-00009a50: 640a 2020 2020 2020 2064 6965 6c65 6374  d.       dielect
-00009a60: 7269 635f 6d65 6469 756d 2069 7320 7468  ric_medium is th
-00009a70: 6520 6469 656c 6563 7472 6963 2063 6f6e  e dielectric con
-00009a80: 7374 616e 7420 7465 6e73 6f72 206f 6620  stant tensor of 
-00009a90: 7468 6520 6d65 6469 756d 0a20 2020 2020  the medium.     
-00009aa0: 2020 6372 7973 7461 6c5f 7065 726d 6974    crystal_permit
-00009ab0: 7469 7669 7479 2069 7320 7468 6520 746f  tivity is the to
-00009ac0: 7461 6c20 6672 6571 7565 6e63 7920 6469  tal frequency di
-00009ad0: 656c 6563 7472 6963 2063 6f6e 7374 616e  electric constan
-00009ae0: 7420 7465 6e73 6f72 2061 7420 7468 6520  t tensor at the 
-00009af0: 6375 7272 656e 7420 6672 6571 7565 6e63  current frequenc
-00009b00: 790a 2020 2020 2020 2073 6861 7065 2069  y.       shape i
-00009b10: 7320 7468 6520 6e61 6d65 206f 6620 7468  s the name of th
-00009b20: 6520 6375 7272 656e 7420 7368 6170 650a  e current shape.
-00009b30: 2020 2020 2020 204c 2069 7320 7468 6520         L is the 
-00009b40: 7368 6170 6573 2064 6570 6f6c 6172 6973  shapes depolaris
-00009b50: 6174 696f 6e20 6d61 7472 6978 0a20 2020  ation matrix.   
-00009b60: 2020 2020 7369 7a65 2069 7320 7468 6520      size is the 
-00009b70: 6469 6d65 6e73 696f 6e6c 6573 7320 7369  dimensionless si
-00009b80: 7a65 2070 6172 616d 6574 6572 2066 6f72  ze parameter for
-00009b90: 2074 6865 2066 7265 7175 656e 6379 2075   the frequency u
-00009ba0: 6e64 6572 2063 6f6e 7369 6465 7261 7469  nder considerati
-00009bb0: 6f6e 0a20 2020 2020 2020 7666 2069 7320  on.       vf is 
-00009bc0: 7468 6520 766f 6c75 6d65 2066 7261 6374  the volume fract
-00009bd0: 696f 6e20 6f66 2066 696c 6c65 720a 2020  ion of filler.  
-00009be0: 2020 2020 2054 6865 2072 6f75 7469 6e65       The routine
-00009bf0: 2072 6574 7572 6e73 2074 6865 2065 6666   returns the eff
-00009c00: 6563 7469 7665 2064 6965 6c65 6374 7269  ective dielectri
-00009c10: 6320 636f 6e73 7461 6e74 2222 220a 2020  c constant""".  
-00009c20: 2020 756e 6974 203d 2069 6e69 7469 616c    unit = initial
-00009c30: 6973 655f 756e 6974 5f74 656e 736f 7228  ise_unit_tensor(
-00009c40: 290a 2020 2020 656d 6564 6975 6d20 3d20  ).    emedium = 
-00009c50: 6e70 2e74 7261 6365 2864 6965 6c65 6374  np.trace(dielect
-00009c60: 7269 635f 6d65 6469 756d 2920 2f20 332e  ric_medium) / 3.
-00009c70: 300a 2020 2020 6561 7070 6172 656e 7420  0.    eapparent 
-00009c80: 3d20 6e70 2e74 7261 6365 2864 6965 6c65  = np.trace(diele
-00009c90: 6374 7269 635f 6170 7061 7265 6e74 2920  ctric_apparent) 
-00009ca0: 2f20 332e 300a 2020 2020 2320 4966 2061  / 3.0.    # If a
-00009cb0: 7070 726f 7072 6961 7465 2063 616c 6375  ppropriate calcu
-00009cc0: 6c61 7465 2061 2073 697a 6520 6566 6665  late a size effe
-00009cd0: 6374 2075 7369 6e67 2045 7175 6174 696f  ct using Equatio
-00009ce0: 6e73 2031 302e 3338 2061 6e64 2031 302e  ns 10.38 and 10.
-00009cf0: 3339 2069 6e20 5369 6876 6f6c 610a 2020  39 in Sihvola.  
-00009d00: 2020 7369 7a65 5f66 6163 746f 7220 3d20    size_factor = 
-00009d10: 6361 6c63 756c 6174 655f 7369 7a65 5f66  calculate_size_f
-00009d20: 6163 746f 7228 7369 7a65 290a 2020 2020  actor(size).    
-00009d30: 2320 4571 7561 7469 6f6e 2035 2e37 3820  # Equation 5.78 
-00009d40: 696e 2053 6968 766f 6c61 0a20 2020 206e  in Sihvola.    n
-00009d50: 616c 7068 6120 3d20 656d 6564 6975 6d2a  alpha = emedium*
-00009d60: 7666 2a6e 702e 646f 7428 2863 7279 7374  vf*np.dot((cryst
-00009d70: 616c 5f70 6572 6d69 7474 6976 6974 7920  al_permittivity 
-00009d80: 2d20 6469 656c 6563 7472 6963 5f6d 6564  - dielectric_med
-00009d90: 6975 6d29 2c20 6e70 2e6c 696e 616c 672e  ium), np.linalg.
-00009da0: 696e 7628 6469 656c 6563 7472 6963 5f6d  inv(dielectric_m
-00009db0: 6564 6975 6d20 2b20 7369 7a65 5f66 6163  edium + size_fac
-00009dc0: 746f 7220 2a20 6e70 2e64 6f74 284c 2c20  tor * np.dot(L, 
-00009dd0: 2863 7279 7374 616c 5f70 6572 6d69 7474  (crystal_permitt
-00009de0: 6976 6974 792d 6469 656c 6563 7472 6963  ivity-dielectric
-00009df0: 5f6d 6564 6975 6d29 2929 290a 2020 2020  _medium)))).    
-00009e00: 6e61 6c70 6861 6c20 3d20 6e70 2e64 6f74  nalphal = np.dot
-00009e10: 2828 6e61 6c70 6861 2f65 6170 7061 7265  ((nalpha/eappare
-00009e20: 6e74 292c 204c 290a 2020 2020 2320 6176  nt), L).    # av
-00009e30: 6572 6167 6520 7468 6520 706f 6c61 7269  erage the polari
-00009e40: 7361 6269 6c69 7479 206f 7665 7220 6f72  sability over or
-00009e50: 6965 6e74 6174 696f 6e0a 2020 2020 6e61  ientation.    na
-00009e60: 6c70 6861 203d 206e 702e 7472 6163 6528  lpha = np.trace(
-00009e70: 6e61 6c70 6861 2920 2f20 332e 3020 2a20  nalpha) / 3.0 * 
-00009e80: 756e 6974 0a20 2020 2023 2061 7665 7261  unit.    # avera
-00009e90: 6765 2074 6865 2070 6f6c 6172 6973 6162  ge the polarisab
-00009ea0: 696c 6974 792a 4c20 6f76 6572 206f 7269  ility*L over ori
-00009eb0: 656e 7461 7469 6f6e 0a20 2020 206e 616c  entation.    nal
-00009ec0: 7068 616c 203d 206e 702e 7472 6163 6528  phal = np.trace(
-00009ed0: 6e61 6c70 6861 6c29 202f 2033 2e30 202a  nalphal) / 3.0 *
-00009ee0: 2075 6e69 740a 2020 2020 706f 6c61 7269   unit.    polari
-00009ef0: 7361 7469 6f6e 203d 206e 702e 646f 7428  sation = np.dot(
-00009f00: 6e70 2e6c 696e 616c 672e 696e 7628 756e  np.linalg.inv(un
-00009f10: 6974 202d 206e 616c 7068 616c 292c 206e  it - nalphal), n
-00009f20: 616c 7068 6129 0a20 2020 2065 6666 6420  alpha).    effd 
-00009f30: 2020 2020 2020 2020 3d20 6469 656c 6563          = dielec
-00009f40: 7472 6963 5f6d 6564 6975 6d20 2b20 706f  tric_medium + po
-00009f50: 6c61 7269 7361 7469 6f6e 0a20 2020 2074  larisation.    t
-00009f60: 7261 6365 203d 206e 702e 7472 6163 6528  race = np.trace(
-00009f70: 6566 6664 2920 2f20 332e 300a 2020 2020  effd) / 3.0.    
-00009f80: 6566 6664 6965 6c65 6320 3d20 6e70 2e61  effdielec = np.a
-00009f90: 7272 6179 285b 5b74 7261 6365 2c20 302c  rray([[trace, 0,
-00009fa0: 2030 5d2c 205b 302c 2074 7261 6365 2c20   0], [0, trace, 
-00009fb0: 305d 2c20 5b30 2c20 302c 2074 7261 6365  0], [0, 0, trace
-00009fc0: 5d5d 290a 2020 2020 7265 7475 726e 2065  ]]).    return e
-00009fd0: 6666 6469 656c 6563 0a0a 6465 6620 6272  ffdielec..def br
-00009fe0: 7567 6765 6d61 6e5f 6d69 6e69 6d69 7365  uggeman_minimise
-00009ff0: 2820 6570 7331 2c20 6570 7332 2c20 7368  ( eps1, eps2, sh
-0000a000: 6170 652c 204c 2c20 6632 2c20 7369 7a65  ape, L, f2, size
-0000a010: 2c20 6570 7362 7229 3a0a 2020 2020 2222  , epsbr):.    ""
-0000a020: 2243 616c 6375 6c61 7465 2074 6865 2065  "Calculate the e
-0000a030: 6666 6563 7469 7665 2063 6f6e 7374 616e  ffective constan
-0000a040: 7420 7065 726d 6974 7469 7669 7479 2075  t permittivity u
-0000a050: 7369 6e67 2074 6865 206d 6574 686f 6420  sing the method 
-0000a060: 6f66 2062 7275 6767 656d 616e 0a20 2020  of bruggeman.   
-0000a070: 2020 2020 6570 7331 2069 7320 7468 6520      eps1 is the 
-0000a080: 6469 656c 6563 7472 6963 2063 6f6e 7374  dielectric const
-0000a090: 616e 7420 7465 6e73 6f72 206f 6620 3120  ant tensor of 1 
-0000a0a0: 2854 6865 206d 6564 6975 6d29 0a20 2020  (The medium).   
-0000a0b0: 2020 2020 6570 7332 2069 7320 7468 6520      eps2 is the 
-0000a0c0: 6469 656c 6563 7472 6963 2063 6f6e 7374  dielectric const
-0000a0d0: 616e 7420 7465 6e73 6f72 206f 6620 3220  ant tensor of 2 
-0000a0e0: 2854 6865 2069 6e63 6c75 7369 6f6e 290a  (The inclusion).
-0000a0f0: 2020 2020 2020 2073 6861 7065 2069 7320         shape is 
-0000a100: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-0000a110: 6375 7272 656e 7420 7368 6170 650a 2020  current shape.  
-0000a120: 2020 2020 204c 2069 7320 7468 6520 7368       L is the sh
-0000a130: 6170 6573 2064 6570 6f6c 6172 6973 6174  apes depolarisat
-0000a140: 696f 6e20 6d61 7472 6978 0a20 2020 2020  ion matrix.     
-0000a150: 2020 6632 2069 7320 7468 6520 766f 6c75    f2 is the volu
-0000a160: 6d65 2066 7261 6374 696f 6e20 6f66 2063  me fraction of c
-0000a170: 6f6d 706f 6e65 6e74 2032 0a20 2020 2020  omponent 2.     
-0000a180: 2020 7369 7a65 2069 7320 7468 6520 6469    size is the di
-0000a190: 6d65 6e73 696f 6e6c 6573 7320 7369 7a65  mensionless size
-0000a1a0: 2070 6172 616d 6574 6572 2066 6f72 2074   parameter for t
-0000a1b0: 6865 2066 7265 7175 656e 6379 2075 6e64  he frequency und
-0000a1c0: 6572 2063 6f6e 7369 6465 7261 7469 6f6e  er consideration
-0000a1d0: 0a20 2020 2020 2020 6570 7362 7220 6973  .       epsbr is
-0000a1e0: 2061 6e20 696e 6974 6961 6c20 6775 6573   an initial gues
-0000a1f0: 7320 6174 2074 6865 2073 6f6c 7574 696f  s at the solutio
-0000a200: 6e0a 2020 2020 2020 2054 6865 2072 6f75  n.       The rou
-0000a210: 7469 6e65 2072 6574 7572 6e73 2074 6865  tine returns the
-0000a220: 2065 6666 6563 7469 7665 2064 6965 6c65   effective diele
-0000a230: 6374 7269 6320 636f 6e73 7461 6e74 0a20  ctric constant. 
-0000a240: 2020 2020 2020 4f6e 2074 6865 2061 7070        On the app
-0000a250: 6c69 6361 7469 6f6e 206f 6620 686f 6d6f  lication of homo
-0000a260: 6765 6e69 7a61 7469 6f6e 2066 6f72 6d61  genization forma
-0000a270: 6c69 736d 7320 746f 2061 6374 6976 6520  lisms to active 
-0000a280: 6469 656c 6563 7472 6963 2063 6f6d 706f  dielectric compo
-0000a290: 7369 7465 206d 6174 6572 6961 6c73 0a20  site materials. 
-0000a2a0: 2020 2020 2020 546f 6d20 472e 204d 6163        Tom G. Mac
-0000a2b0: 6b61 792c 2041 6b68 6c65 7368 204c 616b  kay, Akhlesh Lak
-0000a2c0: 6874 616b 6961 2022 2222 0a20 2020 2066  htakia """.    f
-0000a2d0: 3120 3d20 312e 3020 2d20 6632 0a20 2020  1 = 1.0 - f2.   
-0000a2e0: 2023 2077 6520 6e65 6564 2074 6f20 666f   # we need to fo
-0000a2f0: 6f6c 2074 6865 206f 7074 696d 6973 6572  ol the optimiser
-0000a300: 2069 6e74 6f20 7468 696e 6b69 6e67 2074   into thinking t
-0000a310: 6861 7420 6974 2068 6173 2074 776f 2072  hat it has two r
-0000a320: 6561 6c20 7661 7269 6162 6c65 730a 2020  eal variables.  
-0000a330: 2020 2320 696e 2066 6163 7420 7468 6520    # in fact the 
-0000a340: 7365 636f 6e64 2069 7320 696d 6167 696e  second is imagin
-0000a350: 6172 7920 616e 6420 7265 636f 6e73 7472  ary and reconstr
-0000a360: 7563 7465 6420 696e 2074 6865 205f 6272  ucted in the _br
-0000a370: 7567 5f6d 696e 696d 6973 6520 726f 7574  ug_minimise rout
-0000a380: 696e 650a 2020 2020 7472 6163 6520 3d20  ine.    trace = 
-0000a390: 6e70 2e74 7261 6365 2865 7073 6272 2920  np.trace(epsbr) 
-0000a3a0: 2f20 332e 300a 2020 2020 7661 7269 6162  / 3.0.    variab
-0000a3b0: 6c65 7320 3d20 6e70 2e61 7272 6179 285b  les = np.array([
-0000a3c0: 6e70 2e72 6561 6c28 7472 6163 6529 2c20  np.real(trace), 
-0000a3d0: 6e70 2e6c 6f67 2831 2e30 202b 206e 702e  np.log(1.0 + np.
-0000a3e0: 6162 7328 6e70 2e69 6d61 6728 7472 6163  abs(np.imag(trac
-0000a3f0: 6529 2929 5d29 0a20 2020 206f 7074 696f  e)))]).    optio
-0000a400: 6e73 203d 207b 2778 746f 6c27 3a20 312e  ns = {'xtol': 1.
-0000a410: 3065 2d34 2c0a 2020 2020 2020 2020 2020  0e-4,.          
-0000a420: 2020 2020 2027 6674 6f6c 273a 2031 2e30       'ftol': 1.0
-0000a430: 452d 347d 0a20 2020 2073 6f6c 203d 2073  E-4}.    sol = s
-0000a440: 632e 6d69 6e69 6d69 7a65 285f 6272 7567  c.minimize(_brug
-0000a450: 5f6d 696e 696d 6973 655f 7465 6e73 6f72  _minimise_tensor
-0000a460: 2c20 7661 7269 6162 6c65 732c 206d 6574  , variables, met
-0000a470: 686f 643d 2750 6f77 656c 6c27 2c20 6172  hod='Powell', ar
-0000a480: 6773 3d28 6570 7331 2c20 6570 7332 2c20  gs=(eps1, eps2, 
-0000a490: 7368 6170 652c 204c 2c20 6631 2c20 7369  shape, L, f1, si
-0000a4a0: 7a65 292c 206f 7074 696f 6e73 3d6f 7074  ze), options=opt
-0000a4b0: 696f 6e73 290a 2020 2020 6966 206e 6f74  ions).    if not
-0000a4c0: 2073 6f6c 2e73 7563 6365 7373 3a0a 2020   sol.success:.  
-0000a4d0: 2020 2020 2020 7072 696e 7428 2241 2042        print("A B
-0000a4e0: 7275 6767 656d 616e 2073 6f6c 7574 696f  ruggeman solutio
-0000a4f0: 6e20 7761 7320 6e6f 7420 666f 756e 6420  n was not found 
-0000a500: 6174 2074 6869 7320 6672 6571 7565 6e63  at this frequenc
-0000a510: 7922 290a 2020 2020 7661 7269 6162 6c65  y").    variable
-0000a520: 7320 3d20 736f 6c2e 780a 2020 2020 2320  s = sol.x.    # 
-0000a530: 7472 616e 7366 6f72 6d20 7468 6520 696d  transform the im
-0000a540: 6167 696e 6172 7920 7661 7269 6162 6c65  aginary variable
-0000a550: 2062 6163 6b0a 2020 2020 7472 6163 6520   back.    trace 
-0000a560: 3d20 636f 6d70 6c65 7828 7661 7269 6162  = complex(variab
-0000a570: 6c65 735b 305d 2c20 6e70 2e65 7870 2876  les[0], np.exp(v
-0000a580: 6172 6961 626c 6573 5b31 5d29 2d31 2e30  ariables[1])-1.0
-0000a590: 290a 2020 2020 6570 7362 7220 3d20 6e70  ).    epsbr = np
-0000a5a0: 2e61 7272 6179 285b 5b74 7261 6365 2c20  .array([[trace, 
-0000a5b0: 302c 2030 5d2c 205b 302c 2074 7261 6365  0, 0], [0, trace
-0000a5c0: 2c20 305d 2c20 5b30 2c20 302c 2074 7261  , 0], [0, 0, tra
-0000a5d0: 6365 5d5d 290a 2020 2020 7265 7475 726e  ce]]).    return
-0000a5e0: 2065 7073 6272 0a0a 6465 6620 6272 7567   epsbr..def brug
-0000a5f0: 6765 6d61 6e5f 6974 6572 2820 6570 7331  geman_iter( eps1
-0000a600: 2c20 6570 7332 2c20 7368 6170 652c 204c  , eps2, shape, L
-0000a610: 2c20 6632 2c20 7369 7a65 2c20 6570 7362  , f2, size, epsb
-0000a620: 7229 3a0a 2020 2020 2222 2243 616c 6375  r):.    """Calcu
-0000a630: 6c61 7465 2074 6865 2065 6666 6563 7469  late the effecti
-0000a640: 7665 2063 6f6e 7374 616e 7420 7065 726d  ve constant perm
-0000a650: 6974 7469 7669 7479 2075 7369 6e67 2074  ittivity using t
-0000a660: 6865 206d 6574 686f 6420 6f66 2062 7275  he method of bru
-0000a670: 6767 656d 616e 0a20 2020 2020 2020 6570  ggeman.       ep
-0000a680: 7331 2069 7320 7468 6520 6469 656c 6563  s1 is the dielec
-0000a690: 7472 6963 2063 6f6e 7374 616e 7420 7465  tric constant te
-0000a6a0: 6e73 6f72 206f 6620 3120 2854 6865 206d  nsor of 1 (The m
-0000a6b0: 6564 6975 6d29 0a20 2020 2020 2020 6570  edium).       ep
-0000a6c0: 7332 2069 7320 7468 6520 6469 656c 6563  s2 is the dielec
-0000a6d0: 7472 6963 2063 6f6e 7374 616e 7420 7465  tric constant te
-0000a6e0: 6e73 6f72 206f 6620 3220 2854 6865 2069  nsor of 2 (The i
-0000a6f0: 6e63 6c75 7369 6f6e 290a 2020 2020 2020  nclusion).      
-0000a700: 2073 6861 7065 2069 7320 7468 6520 6e61   shape is the na
-0000a710: 6d65 206f 6620 7468 6520 6375 7272 656e  me of the curren
-0000a720: 7420 7368 6170 650a 2020 2020 2020 204c  t shape.       L
-0000a730: 2069 7320 7468 6520 7368 6170 6573 2064   is the shapes d
-0000a740: 6570 6f6c 6172 6973 6174 696f 6e20 6d61  epolarisation ma
-0000a750: 7472 6978 0a20 2020 2020 2020 6632 2069  trix.       f2 i
-0000a760: 7320 7468 6520 766f 6c75 6d65 2066 7261  s the volume fra
-0000a770: 6374 696f 6e20 6f66 2063 6f6d 706f 6e65  ction of compone
-0000a780: 6e74 2032 0a20 2020 2020 2020 7369 7a65  nt 2.       size
-0000a790: 2069 7320 7468 6520 6469 6d65 6e73 696f   is the dimensio
-0000a7a0: 6e6c 6573 7320 7369 7a65 2070 6172 616d  nless size param
-0000a7b0: 6574 6572 2066 6f72 2074 6865 2066 7265  eter for the fre
-0000a7c0: 7175 656e 6379 2075 6e64 6572 2063 6f6e  quency under con
-0000a7d0: 7369 6465 7261 7469 6f6e 0a20 2020 2020  sideration.     
-0000a7e0: 2020 6570 7362 7220 6973 2061 6e20 696e    epsbr is an in
-0000a7f0: 6974 6961 6c20 6775 6573 7320 6174 2074  itial guess at t
-0000a800: 6865 2073 6f6c 7574 696f 6e0a 2020 2020  he solution.    
-0000a810: 2020 2054 6865 2072 6f75 7469 6e65 2072     The routine r
-0000a820: 6574 7572 6e73 2074 6865 2065 6666 6563  eturns the effec
-0000a830: 7469 7665 2064 6965 6c65 6374 7269 6320  tive dielectric 
-0000a840: 636f 6e73 7461 6e74 0a20 2020 2020 2020  constant.       
-0000a850: 4f6e 2074 6865 2061 7070 6c69 6361 7469  On the applicati
-0000a860: 6f6e 206f 6620 686f 6d6f 6765 6e69 7a61  on of homogeniza
-0000a870: 7469 6f6e 2066 6f72 6d61 6c69 736d 7320  tion formalisms 
-0000a880: 746f 2061 6374 6976 6520 6469 656c 6563  to active dielec
-0000a890: 7472 6963 2063 6f6d 706f 7369 7465 206d  tric composite m
-0000a8a0: 6174 6572 6961 6c73 0a20 2020 2020 2020  aterials.       
-0000a8b0: 546f 6d20 472e 204d 6163 6b61 792c 2041  Tom G. Mackay, A
-0000a8c0: 6b68 6c65 7368 204c 616b 6874 616b 6961  khlesh Lakhtakia
-0000a8d0: 2022 2222 0a20 2020 2066 3120 3d20 312e   """.    f1 = 1.
-0000a8e0: 3020 2d20 6632 0a20 2020 2023 2070 6572  0 - f2.    # per
-0000a8f0: 666f 726d 2061 6e20 6974 6572 6174 696f  form an iteratio
-0000a900: 6e0a 2020 2020 636f 6e76 6572 6765 6420  n.    converged 
-0000a910: 3d20 4661 6c73 650a 2020 2020 6e69 7465  = False.    nite
-0000a920: 7273 203d 2030 0a20 2020 2077 6869 6c65  rs = 0.    while
-0000a930: 206e 6f74 2063 6f6e 7665 7267 6564 3a0a   not converged:.
-0000a940: 2020 2020 2020 2020 6e69 7465 7273 202b          niters +
-0000a950: 3d20 310a 2020 2020 2020 2020 6570 7362  = 1.        epsb
-0000a960: 722c 2065 7272 6f72 203d 205f 6272 7567  r, error = _brug
-0000a970: 5f69 7465 725f 6572 726f 7228 6570 7362  _iter_error(epsb
-0000a980: 722c 2065 7073 312c 2065 7073 322c 2073  r, eps1, eps2, s
-0000a990: 6861 7065 2c20 4c2c 2066 312c 2073 697a  hape, L, f1, siz
-0000a9a0: 6529 0a20 2020 2020 2020 2069 6620 6162  e).        if ab
-0000a9b0: 7328 6572 726f 7229 203c 2031 2e30 452d  s(error) < 1.0E-
-0000a9c0: 383a 0a20 2020 2020 2020 2020 2020 2063  8:.            c
-0000a9d0: 6f6e 7665 7267 6564 203d 2054 7275 650a  onverged = True.
-0000a9e0: 2020 2020 2020 2020 6966 206e 6974 6572          if niter
-0000a9f0: 7320 3e20 3330 3030 3a0a 2020 2020 2020  s > 3000:.      
-0000aa00: 2020 2020 2020 7072 696e 7428 2242 7275        print("Bru
-0000aa10: 6767 656d 616e 2069 7465 7261 7469 6f6e  ggeman iteration
-0000aa20: 7320 6661 696c 6564 2c20 6572 726f 723d  s failed, error=
-0000aa30: 222c 2065 7272 6f72 290a 2020 2020 2020  ", error).      
-0000aa40: 2020 2020 2020 636f 6e76 6572 6765 6420        converged 
-0000aa50: 3d20 5472 7565 0a20 2020 2065 7073 6272  = True.    epsbr
-0000aa60: 203d 2061 7665 7261 6765 5f74 656e 736f   = average_tenso
-0000aa70: 7228 6570 7362 7229 0a20 2020 2072 6574  r(epsbr).    ret
-0000aa80: 7572 6e20 6570 7362 720a 0a64 6566 2061  urn epsbr..def a
-0000aa90: 7665 7261 6765 5f74 656e 736f 7228 7429  verage_tensor(t)
-0000aaa0: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
-0000aab0: 7468 6520 6176 6572 6167 6564 2074 656e  the averaged ten
-0000aac0: 736f 7222 2222 0a20 2020 2061 203d 206e  sor""".    a = n
-0000aad0: 702e 7472 6163 6528 7429 202f 2033 2e30  p.trace(t) / 3.0
-0000aae0: 0a20 2020 2072 6574 7572 6e20 6e70 2e61  .    return np.a
-0000aaf0: 7272 6179 285b 5b61 2c20 302c 2030 5d2c  rray([[a, 0, 0],
-0000ab00: 205b 302c 2061 2c20 305d 2c20 5b30 2c20   [0, a, 0], [0, 
-0000ab10: 302c 2061 5d5d 290a 0a64 6566 205f 6272  0, a]])..def _br
-0000ab20: 7567 5f6d 696e 696d 6973 655f 7363 616c  ug_minimise_scal
-0000ab30: 6172 2876 6172 6961 626c 6573 2c20 6570  ar(variables, ep
-0000ab40: 7331 2c20 6570 7332 2c20 7368 6170 652c  s1, eps2, shape,
-0000ab50: 204c 2c20 6631 2c20 7369 7a65 293a 0a20   L, f1, size):. 
-0000ab60: 2020 2022 2222 4272 7567 6765 6d61 6e20     """Bruggeman 
-0000ab70: 6d65 7468 6f64 2075 7369 6e67 2073 6361  method using sca
-0000ab80: 6c61 7220 7175 616e 7469 7469 6573 2222  lar quantities""
-0000ab90: 220a 2020 2020 2320 756e 7061 636b 2074  ".    # unpack t
-0000aba0: 6865 2063 6f6d 706c 6578 206e 756d 6265  he complex numbe
-0000abb0: 7220 6672 6f6d 2074 6865 2076 6172 6961  r from the varia
-0000abc0: 626c 6573 0a20 2020 2023 2074 776f 2074  bles.    # two t
-0000abd0: 6869 6e67 7320 676f 696e 6720 6f6e 2068  hings going on h
-0000abe0: 6572 652e 0a20 2020 2023 2031 2e20 7468  ere..    # 1. th
-0000abf0: 6520 7477 6f20 7661 7269 6162 6c65 7320  e two variables 
-0000ac00: 7265 6665 7220 746f 2074 6865 2072 6561  refer to the rea
-0000ac10: 6c20 616e 6420 696d 6167 696e 6172 7920  l and imaginary 
-0000ac20: 636f 6d70 6f6e 656e 7473 0a20 2020 2023  components.    #
-0000ac30: 2032 2e20 7765 2072 6571 7569 7265 2074   2. we require t
-0000ac40: 6865 2069 6d61 6769 6e61 7279 2063 6f6d  he imaginary com
-0000ac50: 706f 6e65 6e74 2074 6f20 6265 2070 6f73  ponent to be pos
-0000ac60: 6974 6976 650a 2020 2020 7472 6163 6520  itive.    trace 
-0000ac70: 3d20 636f 6d70 6c65 7828 7661 7269 6162  = complex(variab
-0000ac80: 6c65 735b 305d 2c20 6e70 2e65 7870 2876  les[0], np.exp(v
-0000ac90: 6172 6961 626c 6573 5b31 5d29 2d31 2e30  ariables[1])-1.0
-0000aca0: 290a 2020 2020 6570 7362 7220 3d20 6e70  ).    epsbr = np
-0000acb0: 2e61 7272 6179 285b 5b74 7261 6365 2c20  .array([[trace, 
-0000acc0: 302c 2030 5d2c 205b 302c 2074 7261 6365  0, 0], [0, trace
-0000acd0: 2c20 305d 2c20 5b30 2c20 302c 2074 7261  , 0], [0, 0, tra
-0000ace0: 6365 5d5d 290a 2020 2020 6632 203d 2031  ce]]).    f2 = 1
-0000acf0: 2e30 202d 2066 310a 2020 2020 2320 4966  .0 - f1.    # If
-0000ad00: 2061 7070 726f 7072 6961 7465 2063 616c   appropriate cal
-0000ad10: 6375 6c61 7465 2061 2073 697a 6520 6566  culate a size ef
-0000ad20: 6665 6374 2075 7369 6e67 2045 7175 6174  fect using Equat
-0000ad30: 696f 6e73 2031 302e 3338 2061 6e64 2031  ions 10.38 and 1
-0000ad40: 302e 3339 2069 6e20 5369 6876 6f6c 610a  0.39 in Sihvola.
-0000ad50: 2020 2020 7369 7a65 5f66 6163 746f 7220      size_factor 
-0000ad60: 3d20 6361 6c63 756c 6174 655f 7369 7a65  = calculate_size
-0000ad70: 5f66 6163 746f 7228 7369 7a65 290a 2020  _factor(size).  
-0000ad80: 2020 6231 203d 206e 702e 646f 7428 4c2c    b1 = np.dot(L,
-0000ad90: 2028 6570 7331 202d 2065 7073 6272 2929   (eps1 - epsbr))
-0000ada0: 0a20 2020 2062 3220 3d20 7369 7a65 5f66  .    b2 = size_f
-0000adb0: 6163 746f 7220 2a20 6e70 2e64 6f74 284c  actor * np.dot(L
-0000adc0: 2c20 2865 7073 3220 2d20 6570 7362 7229  , (eps2 - epsbr)
-0000add0: 290a 2020 2020 7462 3120 3d20 6e70 2e74  ).    tb1 = np.t
-0000ade0: 7261 6365 2862 3129 2f33 2e30 0a20 2020  race(b1)/3.0.   
-0000adf0: 2074 6232 203d 206e 702e 7472 6163 6528   tb2 = np.trace(
-0000ae00: 6232 292f 332e 300a 2020 2020 7461 3120  b2)/3.0.    ta1 
-0000ae10: 3d20 312e 302f 2831 2e30 202b 2074 6231  = 1.0/(1.0 + tb1
-0000ae20: 290a 2020 2020 7461 3220 3d20 312e 302f  ).    ta2 = 1.0/
-0000ae30: 2831 2e30 202b 2074 6232 290a 2020 2020  (1.0 + tb2).    
-0000ae40: 6331 203d 2065 7073 312d 6570 7362 720a  c1 = eps1-epsbr.
-0000ae50: 2020 2020 6332 203d 2065 7073 322d 6570      c2 = eps2-ep
-0000ae60: 7362 720a 2020 2020 7463 3120 3d20 6e70  sbr.    tc1 = np
-0000ae70: 2e74 7261 6365 2863 3129 2f33 2e30 0a20  .trace(c1)/3.0. 
-0000ae80: 2020 2074 6332 203d 206e 702e 7472 6163     tc2 = np.trac
-0000ae90: 6528 6332 292f 332e 300a 2020 2020 2320  e(c2)/3.0.    # 
-0000aea0: 616c 7068 6131 2061 6e64 2032 2061 7265  alpha1 and 2 are
-0000aeb0: 2074 6865 2070 6f6c 6172 6973 6162 696c   the polarisabil
-0000aec0: 6974 6965 7320 6f66 2031 2061 6e64 2032  ities of 1 and 2
-0000aed0: 2069 6e20 7468 6520 6566 6665 6374 6976   in the effectiv
-0000aee0: 6520 6d65 6469 756d 0a20 2020 2074 616c  e medium.    tal
-0000aef0: 7068 6131 203d 2074 6331 202a 2074 6131  pha1 = tc1 * ta1
-0000af00: 0a20 2020 2074 616c 7068 6132 203d 2074  .    talpha2 = t
-0000af10: 6332 202a 2074 6132 0a20 2020 2065 7272  c2 * ta2.    err
-0000af20: 6f72 203d 2066 312a 7461 6c70 6861 3120  or = f1*talpha1 
-0000af30: 2b20 6632 2a74 616c 7068 6132 0a20 2020  + f2*talpha2.   
-0000af40: 2065 7272 6f72 203d 206e 702e 6162 7328   error = np.abs(
-0000af50: 6572 726f 722e 636f 6e6a 7567 6174 6528  error.conjugate(
-0000af60: 2920 2a20 6572 726f 7229 0a20 2020 2023  ) * error).    #
-0000af70: 204e 6173 7479 2069 7373 7565 2069 6e20   Nasty issue in 
-0000af80: 7468 6520 706f 7765 6c6c 206d 6574 686f  the powell metho
-0000af90: 642c 2074 6865 2063 6f6e 7665 7267 656e  d, the convergen
-0000afa0: 6365 206f 6e20 746f 6c20 6973 2067 6976  ce on tol is giv
-0000afb0: 656e 0a20 2020 2023 2072 656c 6174 6976  en.    # relativ
-0000afc0: 6520 746f 2074 6865 2073 6f6c 7574 696f  e to the solutio
-0000afd0: 6e20 2830 2e30 292e 2020 4f6e 6c79 2061  n (0.0).  Only a
-0000afe0: 2073 6d61 6c6c 206e 756d 6265 7220 6973   small number is
-0000aff0: 2061 6464 6564 2e0a 2020 2020 2320 536f   added..    # So
-0000b000: 2077 6520 7368 6966 7420 7468 6520 736f   we shift the so
-0000b010: 6c75 7469 6f6e 2062 7920 312e 302c 2074  lution by 1.0, t
-0000b020: 6865 2074 6f6c 2069 7320 6e6f 7720 7265  he tol is now re
-0000b030: 6c61 7469 7665 2074 6f20 312e 300a 2020  lative to 1.0.  
-0000b040: 2020 7265 7475 726e 2031 2e30 2b65 7272    return 1.0+err
-0000b050: 6f72 0a0a 6465 6620 5f62 7275 675f 6d69  or..def _brug_mi
-0000b060: 6e69 6d69 7365 5f74 656e 736f 7228 7661  nimise_tensor(va
-0000b070: 7269 6162 6c65 732c 2065 7073 312c 2065  riables, eps1, e
-0000b080: 7073 322c 2073 6861 7065 2c20 4c2c 2066  ps2, shape, L, f
-0000b090: 312c 2073 697a 6529 3a0a 2020 2020 2222  1, size):.    ""
-0000b0a0: 2242 7275 6767 656d 616e 206d 6574 686f  "Bruggeman metho
-0000b0b0: 6420 7573 696e 6720 7465 6e73 6f72 2071  d using tensor q
-0000b0c0: 7561 6e74 6974 6965 7322 2222 0a20 2020  uantities""".   
-0000b0d0: 2023 2075 6e70 6163 6b20 7468 6520 636f   # unpack the co
-0000b0e0: 6d70 6c65 7820 6e75 6d62 6572 2066 726f  mplex number fro
-0000b0f0: 6d20 7468 6520 7661 7269 6162 6c65 730a  m the variables.
-0000b100: 2020 2020 2320 7477 6f20 7468 696e 6773      # two things
-0000b110: 2067 6f69 6e67 206f 6e20 6865 7265 2e0a   going on here..
-0000b120: 2020 2020 2320 312e 2074 6865 2074 776f      # 1. the two
-0000b130: 2076 6172 6961 626c 6573 2072 6566 6572   variables refer
-0000b140: 2074 6f20 7468 6520 7265 616c 2061 6e64   to the real and
-0000b150: 2069 6d61 6769 6e61 7279 2063 6f6d 706f   imaginary compo
-0000b160: 6e65 6e74 730a 2020 2020 2320 322e 2077  nents.    # 2. w
-0000b170: 6520 7265 7175 6972 6520 7468 6520 696d  e require the im
-0000b180: 6167 696e 6172 7920 636f 6d70 6f6e 656e  aginary componen
-0000b190: 7420 746f 2062 6520 706f 7369 7469 7665  t to be positive
-0000b1a0: 0a20 2020 2074 7261 6365 203d 2063 6f6d  .    trace = com
-0000b1b0: 706c 6578 2876 6172 6961 626c 6573 5b30  plex(variables[0
-0000b1c0: 5d2c 206e 702e 6578 7028 7661 7269 6162  ], np.exp(variab
-0000b1d0: 6c65 735b 315d 292d 312e 3029 0a20 2020  les[1])-1.0).   
-0000b1e0: 2065 7073 6272 203d 206e 702e 6172 7261   epsbr = np.arra
-0000b1f0: 7928 5b5b 7472 6163 652c 2020 302c 2030  y([[trace,  0, 0
-0000b200: 5d2c 205b 302c 2074 7261 6365 2c20 305d  ], [0, trace, 0]
-0000b210: 2c20 5b30 2c20 302c 2074 7261 6365 5d5d  , [0, 0, trace]]
-0000b220: 290a 2020 2020 6632 203d 2031 2e30 202d  ).    f2 = 1.0 -
-0000b230: 2066 310a 2020 2020 2320 4966 2061 7070   f1.    # If app
-0000b240: 726f 7072 6961 7465 2063 616c 6375 6c61  ropriate calcula
-0000b250: 7465 2061 2073 697a 6520 6566 6665 6374  te a size effect
-0000b260: 2075 7369 6e67 2045 7175 6174 696f 6e73   using Equations
-0000b270: 2031 302e 3338 2061 6e64 2031 302e 3339   10.38 and 10.39
-0000b280: 2069 6e20 5369 6876 6f6c 610a 2020 2020   in Sihvola.    
-0000b290: 7369 7a65 5f66 6163 746f 7220 3d20 6361  size_factor = ca
-0000b2a0: 6c63 756c 6174 655f 7369 7a65 5f66 6163  lculate_size_fac
-0000b2b0: 746f 7228 7369 7a65 290a 2020 2020 6231  tor(size).    b1
-0000b2c0: 203d 206e 702e 646f 7428 4c2c 2028 6570   = np.dot(L, (ep
-0000b2d0: 7331 202d 2065 7073 6272 2929 0a20 2020  s1 - epsbr)).   
-0000b2e0: 2062 3220 3d20 7369 7a65 5f66 6163 746f   b2 = size_facto
-0000b2f0: 7220 2a20 6e70 2e64 6f74 284c 2c20 2865  r * np.dot(L, (e
-0000b300: 7073 3220 2d20 6570 7362 7229 290a 2020  ps2 - epsbr)).  
-0000b310: 2020 6231 203d 2061 7665 7261 6765 5f74    b1 = average_t
-0000b320: 656e 736f 7228 6231 290a 2020 2020 6232  ensor(b1).    b2
-0000b330: 203d 2061 7665 7261 6765 5f74 656e 736f   = average_tenso
-0000b340: 7228 6232 290a 2020 2020 6131 203d 206e  r(b2).    a1 = n
-0000b350: 702e 6c69 6e61 6c67 2e69 6e76 2865 7073  p.linalg.inv(eps
-0000b360: 6272 202b 2062 3129 0a20 2020 2061 3220  br + b1).    a2 
-0000b370: 3d20 6e70 2e6c 696e 616c 672e 696e 7628  = np.linalg.inv(
-0000b380: 6570 7362 7220 2b20 6232 290a 2020 2020  epsbr + b2).    
-0000b390: 6331 203d 2065 7073 312d 6570 7362 720a  c1 = eps1-epsbr.
-0000b3a0: 2020 2020 6332 203d 2065 7073 322d 6570      c2 = eps2-ep
-0000b3b0: 7362 720a 2020 2020 2320 6331 203d 2061  sbr.    # c1 = a
-0000b3c0: 7665 7261 6765 5f74 656e 736f 7228 6570  verage_tensor(ep
-0000b3d0: 7331 2d65 7073 6272 290a 2020 2020 2320  s1-epsbr).    # 
-0000b3e0: 6332 203d 2061 7665 7261 6765 5f74 656e  c2 = average_ten
-0000b3f0: 736f 7228 6570 7332 2d65 7073 6272 290a  sor(eps2-epsbr).
-0000b400: 2020 2020 616c 7068 6131 203d 206e 702e      alpha1 = np.
-0000b410: 646f 7428 6331 2c20 6131 290a 2020 2020  dot(c1, a1).    
-0000b420: 616c 7068 6132 203d 206e 702e 646f 7428  alpha2 = np.dot(
-0000b430: 6332 2c20 6132 290a 2020 2020 616c 7068  c2, a2).    alph
-0000b440: 6131 203d 2061 7665 7261 6765 5f74 656e  a1 = average_ten
-0000b450: 736f 7228 616c 7068 6131 290a 2020 2020  sor(alpha1).    
-0000b460: 616c 7068 6132 203d 2061 7665 7261 6765  alpha2 = average
-0000b470: 5f74 656e 736f 7228 616c 7068 6132 290a  _tensor(alpha2).
-0000b480: 2020 2020 6572 726f 7220 3d20 6631 2a61      error = f1*a
-0000b490: 6c70 6861 3120 2b20 6632 2a61 6c70 6861  lpha1 + f2*alpha
-0000b4a0: 320a 2020 2020 6672 2020 3d20 302e 300a  2.    fr  = 0.0.
-0000b4b0: 2020 2020 6669 2020 3d20 302e 300a 2020      fi  = 0.0.  
-0000b4c0: 2020 666f 7220 6320 696e 2065 7272 6f72    for c in error
-0000b4d0: 3a0a 2020 2020 2020 2020 666f 7220 6620  :.        for f 
-0000b4e0: 696e 2063 3a0a 2020 2020 2020 2020 2020  in c:.          
-0000b4f0: 2020 6672 202b 3d20 6e70 2e72 6561 6c28    fr += np.real(
-0000b500: 6629 2a2a 320a 2020 2020 2020 2020 2020  f)**2.          
-0000b510: 2020 6669 202b 3d20 6e70 2e69 6d61 6728    fi += np.imag(
-0000b520: 6629 2a2a 320a 2020 2020 6572 726f 7220  f)**2.    error 
-0000b530: 3d20 6e70 2e6c 696e 616c 672e 6e6f 726d  = np.linalg.norm
-0000b540: 2865 7272 6f72 290a 2020 2020 2320 4e61  (error).    # Na
-0000b550: 7374 7920 6973 7375 6520 696e 2074 6865  sty issue in the
-0000b560: 2070 6f77 656c 6c20 6d65 7468 6f64 2c20   powell method, 
-0000b570: 7468 6520 636f 6e76 6572 6765 6e63 6520  the convergence 
-0000b580: 6f6e 2074 6f6c 2069 7320 6769 7665 6e0a  on tol is given.
-0000b590: 2020 2020 2320 7265 6c61 7469 7665 2074      # relative t
-0000b5a0: 6f20 7468 6520 736f 6c75 7469 6f6e 2028  o the solution (
-0000b5b0: 302e 3029 2e20 204f 6e6c 7920 6120 736d  0.0).  Only a sm
-0000b5c0: 616c 6c20 6e75 6d62 6572 2069 7320 6164  all number is ad
-0000b5d0: 6465 642e 0a20 2020 2023 2053 6f20 7765  ded..    # So we
-0000b5e0: 2073 6869 6674 2074 6865 2073 6f6c 7574   shift the solut
-0000b5f0: 696f 6e20 6279 2031 2e30 2c20 7468 6520  ion by 1.0, the 
-0000b600: 746f 6c20 6973 206e 6f77 2072 656c 6174  tol is now relat
-0000b610: 6976 6520 746f 2031 2e30 0a20 2020 2072  ive to 1.0.    r
-0000b620: 6574 7572 6e20 312e 302b 6572 726f 720a  eturn 1.0+error.
-0000b630: 0a64 6566 205f 6272 7567 5f69 7465 725f  .def _brug_iter_
-0000b640: 6572 726f 7228 6570 7362 722c 2065 7073  error(epsbr, eps
-0000b650: 312c 2065 7073 322c 2073 6861 7065 2c20  1, eps2, shape, 
-0000b660: 4c2c 2066 312c 2073 697a 6529 3a0a 2020  L, f1, size):.  
-0000b670: 2020 2222 2252 6f75 7469 6e65 2074 6f20    """Routine to 
-0000b680: 6361 6c63 756c 6174 6520 7468 6520 6572  calculate the er
-0000b690: 726f 7220 696e 2074 6865 2042 7275 6767  ror in the Brugg
-0000b6a0: 656d 616e 206d 6574 686f 6422 2222 0a20  eman method""". 
-0000b6b0: 2020 2066 3220 3d20 312e 3020 2d20 6631     f2 = 1.0 - f1
-0000b6c0: 0a20 2020 2023 2049 6620 6170 7072 6f70  .    # If approp
-0000b6d0: 7269 6174 6520 6361 6c63 756c 6174 6520  riate calculate 
-0000b6e0: 6120 7369 7a65 2065 6666 6563 7420 7573  a size effect us
-0000b6f0: 696e 6720 4571 7561 7469 6f6e 7320 3130  ing Equations 10
-0000b700: 2e33 3820 616e 6420 3130 2e33 3920 696e  .38 and 10.39 in
-0000b710: 2053 6968 766f 6c61 0a20 2020 2073 697a   Sihvola.    siz
-0000b720: 655f 6661 6374 6f72 203d 2063 616c 6375  e_factor = calcu
-0000b730: 6c61 7465 5f73 697a 655f 6661 6374 6f72  late_size_factor
-0000b740: 2873 697a 6529 0a20 2020 206c 6570 7331  (size).    leps1
-0000b750: 203d 206e 702e 646f 7428 4c2c 2028 6570   = np.dot(L, (ep
-0000b760: 7331 202d 2065 7073 6272 2929 0a20 2020  s1 - epsbr)).   
-0000b770: 206c 6570 7332 203d 2073 697a 655f 6661   leps2 = size_fa
-0000b780: 6374 6f72 202a 206e 702e 646f 7428 4c2c  ctor * np.dot(L,
-0000b790: 2028 6570 7332 202d 2065 7073 6272 2929   (eps2 - epsbr))
-0000b7a0: 0a20 2020 206c 6570 7331 203d 2061 7665  .    leps1 = ave
-0000b7b0: 7261 6765 5f74 656e 736f 7228 6c65 7073  rage_tensor(leps
-0000b7c0: 3129 0a20 2020 206c 6570 7332 203d 2061  1).    leps2 = a
-0000b7d0: 7665 7261 6765 5f74 656e 736f 7228 6c65  verage_tensor(le
-0000b7e0: 7073 3229 0a20 2020 2061 3120 3d20 6e70  ps2).    a1 = np
-0000b7f0: 2e6c 696e 616c 672e 696e 7628 6570 7362  .linalg.inv(epsb
-0000b800: 7220 2b20 6c65 7073 3129 0a20 2020 2061  r + leps1).    a
-0000b810: 3220 3d20 6e70 2e6c 696e 616c 672e 696e  2 = np.linalg.in
-0000b820: 7628 6570 7362 7220 2b20 6c65 7073 3229  v(epsbr + leps2)
-0000b830: 0a20 2020 2023 2061 6c70 6861 3120 616e  .    # alpha1 an
-0000b840: 6420 3220 6172 6520 7468 6520 706f 6c61  d 2 are the pola
-0000b850: 7269 7361 6269 6c69 7469 6573 206f 6620  risabilities of 
-0000b860: 3120 616e 6420 3220 696e 2074 6865 2065  1 and 2 in the e
-0000b870: 6666 6563 7469 7665 206d 6564 6975 6d0a  ffective medium.
-0000b880: 2020 2020 6570 7331 6176 203d 2061 7665      eps1av = ave
-0000b890: 7261 6765 5f74 656e 736f 7228 6570 7331  rage_tensor(eps1
-0000b8a0: 290a 2020 2020 6570 7332 6176 203d 2061  ).    eps2av = a
-0000b8b0: 7665 7261 6765 5f74 656e 736f 7228 6570  verage_tensor(ep
-0000b8c0: 7332 290a 2020 2020 616c 7068 6131 203d  s2).    alpha1 =
-0000b8d0: 206e 702e 646f 7428 2865 7073 3161 762d   np.dot((eps1av-
-0000b8e0: 6570 7362 7229 2c20 6131 290a 2020 2020  epsbr), a1).    
-0000b8f0: 616c 7068 6132 203d 206e 702e 646f 7428  alpha2 = np.dot(
-0000b900: 2865 7073 3261 762d 6570 7362 7229 2c20  (eps2av-epsbr), 
-0000b910: 6132 290a 2020 2020 2320 7468 6520 6572  a2).    # the er
-0000b920: 726f 7220 6f72 2072 6573 6964 7561 6c20  ror or residual 
-0000b930: 6d61 7472 6978 2073 686f 756c 6420 6265  matrix should be
-0000b940: 207a 6572 6f20 666f 7220 6120 6272 7567   zero for a brug
-0000b950: 6765 6d61 6e20 736f 6c75 7469 6f6e 0a20  geman solution. 
-0000b960: 2020 2065 7272 6f72 203d 2066 312a 616c     error = f1*al
-0000b970: 7068 6131 202b 2066 322a 616c 7068 6132  pha1 + f2*alpha2
-0000b980: 0a20 2020 2065 7272 6f72 203d 206e 702e  .    error = np.
-0000b990: 6c69 6e61 6c67 2e6e 6f72 6d28 6572 726f  linalg.norm(erro
-0000b9a0: 7229 0a20 2020 206d 3120 3d20 6631 2a6e  r).    m1 = f1*n
-0000b9b0: 702e 646f 7428 6570 7331 2c20 6131 292b  p.dot(eps1, a1)+
-0000b9c0: 6632 2a6e 702e 646f 7428 6570 7332 2c20  f2*np.dot(eps2, 
-0000b9d0: 6132 290a 2020 2020 6d32 203d 206e 702e  a2).    m2 = np.
-0000b9e0: 6c69 6e61 6c67 2e69 6e76 2866 312a 6131  linalg.inv(f1*a1
-0000b9f0: 202b 2066 322a 6132 290a 2020 2020 6461   + f2*a2).    da
-0000ba00: 6d70 203d 2030 2e30 0a20 2020 2065 7073  mp = 0.0.    eps
-0000ba10: 6272 203d 2028 312e 3020 2d20 6461 6d70  br = (1.0 - damp
-0000ba20: 292a 6e70 2e64 6f74 286d 312c 206d 3229  )*np.dot(m1, m2)
-0000ba30: 202b 2064 616d 702a 6570 7362 720a 2020   + damp*epsbr.  
-0000ba40: 2020 7472 6163 6520 3d20 6e70 2e74 7261    trace = np.tra
-0000ba50: 6365 2865 7073 6272 2920 2f20 332e 300a  ce(epsbr) / 3.0.
-0000ba60: 2020 2020 6570 7362 7220 3d20 6e70 2e61      epsbr = np.a
-0000ba70: 7272 6179 285b 5b74 7261 6365 2c20 302c  rray([[trace, 0,
-0000ba80: 2030 5d2c 205b 302c 2074 7261 6365 2c20   0], [0, trace, 
-0000ba90: 305d 2c20 5b30 2c20 302c 2074 7261 6365  0], [0, 0, trace
-0000baa0: 5d5d 290a 2020 2020 7265 7475 726e 2065  ]]).    return e
-0000bab0: 7073 6272 2c20 6572 726f 720a 0a64 6566  psbr, error..def
-0000bac0: 2063 616c 6375 6c61 7465 5f72 6566 7261   calculate_refra
-0000bad0: 6374 6976 655f 696e 6465 7828 6469 656c  ctive_index(diel
-0000bae0: 6563 7472 6963 2c20 6465 6275 673d 4661  ectric, debug=Fa
-0000baf0: 6c73 6529 3a0a 2020 2020 2727 2720 4361  lse):.    ''' Ca
-0000bb00: 6c63 756c 6174 6520 7468 6520 7265 6672  lculate the refr
-0000bb10: 6163 7469 7665 2069 6e64 6578 2066 726f  active index fro
-0000bb20: 6d20 7468 6520 6469 656c 6563 7472 6963  m the dielectric
-0000bb30: 2063 6f6e 7374 616e 742e 0a20 2020 2020   constant..     
-0000bb40: 2020 2043 616c 6375 6c61 7465 2074 6865     Calculate the
-0000bb50: 2074 7261 6365 206f 6620 7468 6520 6469   trace of the di
-0000bb60: 656c 6563 7472 6963 2061 6e64 2063 616c  electric and cal
-0000bb70: 6375 6c61 7465 2062 6f74 6820 7371 7561  culate both squa
-0000bb80: 7265 2072 6f6f 7473 2e0a 2020 2020 2020  re roots..      
-0000bb90: 2020 5468 6520 6368 6f6f 7365 2074 6865    The choose the
-0000bba0: 2072 6f6f 7420 7769 7468 2074 6865 206c   root with the l
-0000bbb0: 6172 6765 7374 2069 6d61 6769 6e61 7279  argest imaginary
-0000bbc0: 2063 6f6d 706f 6e65 6e74 2054 6869 7320   component This 
-0000bbd0: 6f62 6579 7320 7468 6520 4b6f 6e69 6720  obeys the Konig 
-0000bbe0: 4b72 616d 6572 2072 6571 7569 7265 6d65  Kramer requireme
-0000bbf0: 6e74 7327 2727 0a20 2020 2074 7261 6365  nts'''.    trace
-0000bc00: 203d 206e 702e 7472 6163 6528 6469 656c   = np.trace(diel
-0000bc10: 6563 7472 6963 292f 332e 300a 2020 2020  ectric)/3.0.    
-0000bc20: 736f 6c75 7469 6f6e 203d 2063 616c 6375  solution = calcu
-0000bc30: 6c61 7465 5f72 6566 7261 6374 6976 655f  late_refractive_
-0000bc40: 696e 6465 785f 7363 616c 6172 2874 7261  index_scalar(tra
-0000bc50: 6365 2c20 6465 6275 6729 0a20 2020 2072  ce, debug).    r
-0000bc60: 6574 7572 6e20 736f 6c75 7469 6f6e 0a0a  eturn solution..
-0000bc70: 6465 6620 6361 6c63 756c 6174 655f 7265  def calculate_re
-0000bc80: 6672 6163 7469 7665 5f69 6e64 6578 5f73  fractive_index_s
-0000bc90: 6361 6c61 7228 6469 656c 6563 7472 6963  calar(dielectric
-0000bca0: 5f73 6361 6c61 722c 2064 6562 7567 3d46  _scalar, debug=F
-0000bcb0: 616c 7365 293a 0a20 2020 2027 2727 2043  alse):.    ''' C
-0000bcc0: 616c 6375 6c61 7465 2074 6865 2072 6566  alculate the ref
-0000bcd0: 7261 6374 6976 6520 696e 6465 7820 6672  ractive index fr
-0000bce0: 6f6d 2074 6865 2064 6965 6c65 6374 7269  om the dielectri
-0000bcf0: 6320 636f 6e73 7461 6e74 2e0a 2020 2020  c constant..    
-0000bd00: 2020 2020 4361 6c63 756c 6174 6520 7468      Calculate th
-0000bd10: 6520 7472 6163 6520 6f66 2074 6865 2064  e trace of the d
-0000bd20: 6965 6c65 6374 7269 6320 616e 6420 6361  ielectric and ca
-0000bd30: 6c63 756c 6174 6520 626f 7468 2073 7175  lculate both squ
-0000bd40: 6172 6520 726f 6f74 732e 0a20 2020 2020  are roots..     
-0000bd50: 2020 2054 6865 2063 686f 6f73 6520 7468     The choose th
-0000bd60: 6520 726f 6f74 2077 6974 6820 7468 6520  e root with the 
-0000bd70: 6c61 7267 6573 7420 696d 6167 696e 6172  largest imaginar
-0000bd80: 7920 636f 6d70 6f6e 656e 7420 5468 6973  y component This
-0000bd90: 206f 6265 7973 2074 6865 204b 6f6e 6967   obeys the Konig
-0000bda0: 204b 7261 6d65 7220 7265 7175 6972 656d   Kramer requirem
-0000bdb0: 656e 7473 2727 270a 2020 2020 736f 6c75  ents'''.    solu
-0000bdc0: 7469 6f6e 3120 3d20 6e70 2e73 7172 7428  tion1 = np.sqrt(
-0000bdd0: 6469 656c 6563 7472 6963 5f73 6361 6c61  dielectric_scala
-0000bde0: 7229 0a20 2020 2072 2c20 7068 6173 6520  r).    r, phase 
-0000bdf0: 3d20 636d 6174 682e 706f 6c61 7228 736f  = cmath.polar(so
-0000be00: 6c75 7469 6f6e 3129 0a20 2020 2073 6f6c  lution1).    sol
-0000be10: 7574 696f 6e32 203d 2063 6d61 7468 2e72  ution2 = cmath.r
-0000be20: 6563 7428 2d72 2c20 7068 6173 6529 0a20  ect(-r, phase). 
-0000be30: 2020 2069 6d61 6731 203d 206e 702e 696d     imag1 = np.im
-0000be40: 6167 2873 6f6c 7574 696f 6e31 290a 2020  ag(solution1).  
-0000be50: 2020 696d 6167 3220 3d20 6e70 2e69 6d61    imag2 = np.ima
-0000be60: 6728 736f 6c75 7469 6f6e 3229 0a20 2020  g(solution2).   
-0000be70: 2069 6620 696d 6167 3120 3e20 696d 6167   if imag1 > imag
-0000be80: 323a 0a20 2020 2020 2020 2073 6f6c 7574  2:.        solut
-0000be90: 696f 6e20 3d20 736f 6c75 7469 6f6e 310a  ion = solution1.
-0000bea0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000beb0: 2020 736f 6c75 7469 6f6e 203d 2073 6f6c    solution = sol
-0000bec0: 7574 696f 6e32 0a20 2020 2069 6620 6e70  ution2.    if np
-0000bed0: 2e61 6273 2873 6f6c 7574 696f 6e2a 736f  .abs(solution*so
-0000bee0: 6c75 7469 6f6e 2d64 6965 6c65 6374 7269  lution-dielectri
-0000bef0: 635f 7363 616c 6172 292f 2831 2b6e 702e  c_scalar)/(1+np.
-0000bf00: 6162 7328 6469 656c 6563 7472 6963 5f73  abs(dielectric_s
-0000bf10: 6361 6c61 7229 2920 3e20 312e 3045 2d38  calar)) > 1.0E-8
-0000bf20: 206f 7220 6465 6275 673a 0a20 2020 2020   or debug:.     
-0000bf30: 2020 2070 7269 6e74 2822 5468 6572 6520     print("There 
-0000bf40: 6973 2061 6e20 6572 726f 7220 696e 2072  is an error in r
-0000bf50: 6566 7261 6374 6976 6520 696e 6465 7822  efractive index"
-0000bf60: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-0000bf70: 2244 6965 6c65 6374 7269 6320 3d20 222c  "Dielectric = ",
-0000bf80: 2064 6965 6c65 6374 7269 635f 7363 616c   dielectric_scal
-0000bf90: 6172 290a 2020 2020 2020 2020 7072 696e  ar).        prin
-0000bfa0: 7428 2273 6f6c 7574 696f 6e2a 736f 6c75  t("solution*solu
-0000bfb0: 7469 6f6e 203d 2022 2c20 736f 6c75 7469  tion = ", soluti
-0000bfc0: 6f6e 2a73 6f6c 7574 696f 6e2c 206e 702e  on*solution, np.
-0000bfd0: 6162 7328 736f 6c75 7469 6f6e 2a73 6f6c  abs(solution*sol
-0000bfe0: 7574 696f 6e2d 6469 656c 6563 7472 6963  ution-dielectric
-0000bff0: 5f73 6361 6c61 7229 290a 2020 2020 2020  _scalar)).      
-0000c000: 2020 7072 696e 7428 2273 6f6c 7574 696f    print("solutio
-0000c010: 6e20 2020 203d 2022 2c20 736f 6c75 7469  n    = ", soluti
-0000c020: 6f6e 2c20 736f 6c75 7469 6f6e 2a73 6f6c  on, solution*sol
-0000c030: 7574 696f 6e29 0a20 2020 2020 2020 2070  ution).        p
-0000c040: 7269 6e74 2822 736f 6c75 7469 6f6e 3120  rint("solution1 
-0000c050: 2020 3d20 222c 2073 6f6c 7574 696f 6e31    = ", solution1
-0000c060: 2c20 736f 6c75 7469 6f6e 312a 736f 6c75  , solution1*solu
-0000c070: 7469 6f6e 3129 0a20 2020 2020 2020 2070  tion1).        p
-0000c080: 7269 6e74 2822 736f 6c75 7469 6f6e 3220  rint("solution2 
-0000c090: 2020 3d20 222c 2073 6f6c 7574 696f 6e32    = ", solution2
-0000c0a0: 2c20 736f 6c75 7469 6f6e 322a 736f 6c75  , solution2*solu
-0000c0b0: 7469 6f6e 3229 0a20 2020 2072 6574 7572  tion2).    retur
-0000c0c0: 6e20 736f 6c75 7469 6f6e 0a0a 6465 6620  n solution..def 
-0000c0d0: 6469 7265 6374 696f 6e5f 6672 6f6d 5f73  direction_from_s
-0000c0e0: 6861 7065 2864 6174 612c 2072 6561 6465  hape(data, reade
-0000c0f0: 7229 3a0a 2020 2020 2222 2220 4465 7465  r):.    """ Dete
-0000c100: 726d 696e 6520 7468 6520 756e 6971 7565  rmine the unique
-0000c110: 2064 6972 6563 7469 6f6e 206f 6620 7468   direction of th
-0000c120: 6520 7368 6170 6520 6672 6f6d 2064 6174  e shape from dat
-0000c130: 610a 2020 2020 6461 7461 206d 6179 2063  a.    data may c
-0000c140: 6f6e 7461 696e 2061 206d 696c 6c65 7220  ontain a miller 
-0000c150: 696e 6469 6365 7320 7768 6963 6820 6465  indices which de
-0000c160: 6669 6e65 7320 6120 7375 7266 6163 6520  fines a surface 
-0000c170: 6567 2e20 2831 2c31 2c2d 3129 0a20 2020  eg. (1,1,-1).   
-0000c180: 206f 7220 6120 6469 7265 6374 696f 6e20   or a direction 
-0000c190: 6173 2061 206d 696c 6c65 7220 6469 7265  as a miller dire
-0000c1a0: 6374 696f 6e20 7665 6374 6f72 2065 672e  ction vector eg.
-0000c1b0: 205b 312c 302c 2d31 5d20 2222 220a 2020   [1,0,-1] """.  
-0000c1c0: 2020 7375 7266 6163 6520 3d20 4661 6c73    surface = Fals
-0000c1d0: 650a 2020 2020 2320 6f72 6967 696e 616c  e.    # original
-0000c1e0: 203d 2064 6174 610a 2020 2020 6920 3d20   = data.    i = 
-0000c1f0: 6461 7461 2e66 696e 6428 222c 2229 0a20  data.find(","). 
-0000c200: 2020 2063 6f6d 6d61 7320 3d20 4661 6c73     commas = Fals
-0000c210: 650a 2020 2020 6966 2069 203e 3d20 303a  e.    if i >= 0:
-0000c220: 0a20 2020 2020 2020 2063 6f6d 6d61 7320  .        commas 
-0000c230: 3d20 5472 7565 0a20 2020 2069 6620 6461  = True.    if da
-0000c240: 7461 5b30 5d20 3d3d 2022 7b22 3a0a 2020  ta[0] == "{":.  
-0000c250: 2020 2020 2020 7375 7266 6163 6520 3d20        surface = 
-0000c260: 5472 7565 0a20 2020 2020 2020 2064 6174  True.        dat
-0000c270: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
-0000c280: 2822 7b22 2c20 2222 290a 2020 2020 2020  ("{", "").      
-0000c290: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-0000c2a0: 706c 6163 6528 227d 222c 2022 2229 0a20  place("}", ""). 
-0000c2b0: 2020 2065 6c69 6620 6461 7461 5b30 5d20     elif data[0] 
-0000c2c0: 3d3d 2022 2822 3a0a 2020 2020 2020 2020  == "(":.        
-0000c2d0: 7375 7266 6163 6520 3d20 5472 7565 0a20  surface = True. 
-0000c2e0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0000c2f0: 7461 2e72 6570 6c61 6365 2822 2822 2c20  ta.replace("(", 
-0000c300: 2222 290a 2020 2020 2020 2020 6461 7461  "").        data
-0000c310: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-0000c320: 2229 222c 2022 2229 0a20 2020 2065 6c69  ")", "").    eli
-0000c330: 6620 6461 7461 5b30 5d20 3d3d 2022 5b22  f data[0] == "["
-0000c340: 3a0a 2020 2020 2020 2020 7375 7266 6163  :.        surfac
-0000c350: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-0000c360: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-0000c370: 706c 6163 6528 225b 222c 2022 2229 0a20  place("[", ""). 
-0000c380: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0000c390: 7461 2e72 6570 6c61 6365 2822 5d22 2c20  ta.replace("]", 
-0000c3a0: 2222 290a 2020 2020 656c 7365 3a0a 2020  "").    else:.  
-0000c3b0: 2020 2020 2020 7072 696e 7428 2245 7272        print("Err
-0000c3c0: 6f72 2065 6e63 6f75 6e74 6572 6564 2069  or encountered i
-0000c3d0: 6e20 696e 7465 7270 7265 7474 696e 6720  n interpretting 
-0000c3e0: 7468 6520 6d69 6c6c 6572 2073 7572 6661  the miller surfa
-0000c3f0: 6365 202f 2076 6563 746f 7222 2c20 6461  ce / vector", da
-0000c400: 7461 290a 2020 2020 2020 2020 6578 6974  ta).        exit
-0000c410: 2831 290a 2020 2020 6966 2063 6f6d 6d61  (1).    if comma
-0000c420: 733a 0a20 2020 2020 2020 2064 6174 6120  s:.        data 
-0000c430: 3d20 6461 7461 2e72 6570 6c61 6365 2822  = data.replace("
-0000c440: 2c22 2c20 2220 2229 0a20 2020 2020 2020  ,", " ").       
-0000c450: 2068 6b6c 203d 2028 5b69 6e74 2866 2920   hkl = ([int(f) 
-0000c460: 666f 7220 6620 696e 2064 6174 612e 7370  for f in data.sp
-0000c470: 6c69 7428 295d 290a 2020 2020 656c 7365  lit()]).    else
-0000c480: 3a0a 2020 2020 2020 2020 6920 3d20 300a  :.        i = 0.
-0000c490: 2020 2020 2020 2020 686b 6c20 3d20 5b30          hkl = [0
-0000c4a0: 2c20 302c 2030 5d0a 2020 2020 2020 2020  , 0, 0].        
-0000c4b0: 666f 7220 6b20 696e 205b 302c 2031 2c20  for k in [0, 1, 
-0000c4c0: 325d 3a0a 2020 2020 2020 2020 2020 2020  2]:.            
-0000c4d0: 7369 676e 203d 2031 0a20 2020 2020 2020  sign = 1.       
-0000c4e0: 2020 2020 2069 6620 6461 7461 5b69 5d20       if data[i] 
-0000c4f0: 3d3d 2022 2d22 3a0a 2020 2020 2020 2020  == "-":.        
-0000c500: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c520: 6967 6e20 3d20 2d31 0a20 2020 2020 2020  ign = -1.       
-0000c530: 2020 2020 2068 6b6c 5b6b 5d20 3d20 7369       hkl[k] = si
-0000c540: 676e 202a 2069 6e74 2864 6174 615b 695d  gn * int(data[i]
-0000c550: 290a 2020 2020 2020 2020 2020 2020 6920  ).            i 
-0000c560: 2b3d 2031 0a20 2020 2023 2065 6e64 206f  += 1.    # end o
-0000c570: 6620 6861 6e64 6c69 6e67 206e 6f20 636f  f handling no co
-0000c580: 6d6d 6173 0a20 2020 2069 6620 6e6f 7420  mmas.    if not 
-0000c590: 6c65 6e28 686b 6c29 203d 3d20 333a 0a20  len(hkl) == 3:. 
-0000c5a0: 2020 2020 2020 2070 7269 6e74 2822 4572         print("Er
-0000c5b0: 726f 7220 656e 636f 756e 7465 7265 6420  ror encountered 
-0000c5c0: 696e 2069 6e74 6572 7072 6574 7469 6e67  in interpretting
-0000c5d0: 2074 6865 206d 696c 6c65 7220 7375 7266   the miller surf
-0000c5e0: 6163 6520 2f20 7665 6374 6f72 222c 2064  ace / vector", d
-0000c5f0: 6174 6129 0a20 2020 2020 2020 2065 7869  ata).        exi
-0000c600: 7428 3129 0a20 2020 2063 656c 6c20 3d20  t(1).    cell = 
-0000c610: 7265 6164 6572 2e75 6e69 745f 6365 6c6c  reader.unit_cell
-0000c620: 735b 2d31 5d0a 2020 2020 6966 2073 7572  s[-1].    if sur
-0000c630: 6661 6365 3a0a 2020 2020 2020 2020 6469  face:.        di
-0000c640: 7265 6374 696f 6e20 3d20 6365 6c6c 2e63  rection = cell.c
-0000c650: 6f6e 7665 7274 5f68 6b6c 5f74 6f5f 7879  onvert_hkl_to_xy
-0000c660: 7a28 686b 6c29 0a20 2020 2065 6c73 653a  z(hkl).    else:
-0000c670: 0a20 2020 2020 2020 2064 6972 6563 7469  .        directi
-0000c680: 6f6e 203d 2063 656c 6c2e 636f 6e76 6572  on = cell.conver
-0000c690: 745f 6162 635f 746f 5f78 797a 2868 6b6c  t_abc_to_xyz(hkl
-0000c6a0: 290a 2020 2020 6469 7265 6374 696f 6e20  ).    direction 
-0000c6b0: 3d20 6469 7265 6374 696f 6e20 2f20 6e70  = direction / np
-0000c6c0: 2e6c 696e 616c 672e 6e6f 726d 2864 6972  .linalg.norm(dir
-0000c6d0: 6563 7469 6f6e 290a 2020 2020 6461 7461  ection).    data
-0000c6e0: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-0000c6f0: 2722 272c 2027 2729 0a20 2020 2064 6174  '"', '').    dat
-0000c700: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
-0000c710: 2822 222c 2027 2729 0a20 2020 2023 2069  ("", '').    # i
-0000c720: 6620 7375 7266 6163 653a 0a20 2020 2023  f surface:.    #
-0000c730: 2020 2020 2070 7269 6e74 2822 5468 6520       print("The 
-0000c740: 6d69 6c6c 6572 2069 6e64 6963 6573 2066  miller indices f
-0000c750: 6f72 2074 6865 2073 7572 6661 6365 2022  or the surface "
-0000c760: 2c20 6f72 6967 696e 616c 2c20 2268 6173  , original, "has
-0000c770: 2061 206e 6f72 6d61 6c22 2c20 6469 7265   a normal", dire
-0000c780: 6374 696f 6e2c 2022 696e 2078 797a 2229  ction, "in xyz")
-0000c790: 0a20 2020 2023 2065 6c73 653a 0a20 2020  .    # else:.   
-0000c7a0: 2023 2020 2020 7072 696e 7428 2254 6865   #    print("The
-0000c7b0: 206d 696c 6c65 7220 6469 7265 6374 696f   miller directio
-0000c7c0: 6e20 222c 206f 7269 6769 6e61 6c2c 2022  n ", original, "
-0000c7d0: 6973 2022 2c20 6469 7265 6374 696f 6e2c  is ", direction,
-0000c7e0: 2022 696e 2078 797a 2229 0a20 2020 2072   "in xyz").    r
-0000c7f0: 6574 7572 6e20 6469 7265 6374 696f 6e0a  eturn direction.
-0000c800: 0a64 6566 2073 6f6c 7665 5f65 6666 6563  .def solve_effec
-0000c810: 7469 7665 5f6d 6564 6975 6d5f 6571 7561  tive_medium_equa
-0000c820: 7469 6f6e 7328 200a 2020 2020 2020 2020  tions( .        
-0000c830: 6d65 7468 6f64 2020 2020 2020 2020 2020  method          
-0000c840: 2020 2020 2020 2020 202c 0a20 2020 2020           ,.     
-0000c850: 2020 2076 6620 2020 2020 2020 2020 2020     vf           
-0000c860: 2020 2020 2020 2020 2020 2020 2c0a 2020              ,.  
-0000c870: 2020 2020 2020 7369 7a65 5f6d 7520 2020        size_mu   
-0000c880: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
-0000c890: 0a20 2020 2020 2020 2073 697a 655f 6469  .        size_di
-0000c8a0: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
-0000c8b0: 2020 2c0a 2020 2020 2020 2020 6469 656c    ,.        diel
-0000c8c0: 6563 7472 6963 5f6d 6564 6975 6d20 2020  ectric_medium   
-0000c8d0: 2020 2020 202c 0a20 2020 2020 2020 2073       ,.        s
-0000c8e0: 6861 7065 2020 2020 2020 2020 2020 2020  hape            
-0000c8f0: 2020 2020 2020 2020 2c0a 2020 2020 2020          ,.      
-0000c900: 2020 4c20 2020 2020 2020 2020 2020 2020    L             
-0000c910: 2020 2020 2020 2020 2020 202c 0a20 2020             ,.   
-0000c920: 2020 2020 2063 6f6e 6365 6e74 7261 7469       concentrati
-0000c930: 6f6e 2020 2020 2020 2020 2020 2020 2c0a  on            ,.
-0000c940: 2020 2020 2020 2020 6174 7250 6572 6d69          atrPermi
-0000c950: 7474 6976 6974 7920 2020 2020 2020 2020  ttivity         
-0000c960: 202c 0a20 2020 2020 2020 2061 7472 5468   ,.        atrTh
-0000c970: 6574 6120 2020 2020 2020 2020 2020 2020  eta             
-0000c980: 2020 2020 2c0a 2020 2020 2020 2020 6174      ,.        at
-0000c990: 7253 506f 6c20 2020 2020 2020 2020 2020  rSPol           
-0000c9a0: 2020 2020 2020 202c 0a20 2020 2020 2020         ,.       
-0000c9b0: 2062 7562 626c 655f 7666 2020 2020 2020   bubble_vf      
-0000c9c0: 2020 2020 2020 2020 2020 2c0a 2020 2020            ,.    
-0000c9d0: 2020 2020 6275 6262 6c65 5f72 6164 6975      bubble_radiu
-0000c9e0: 7320 2020 2020 2020 2020 2020 202c 0a20  s            ,. 
-0000c9f0: 2020 2020 2020 2070 7265 7669 6f75 735f         previous_
-0000ca00: 736f 6c75 7469 6f6e 5f73 6861 7265 6420  solution_shared 
-0000ca10: 2c0a 2020 2020 2020 2020 7061 7261 6d73  ,.        params
-0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca30: 2020 2c0a 2020 2020 2020 2020 293a 0a20    ,.        ):. 
-0000ca40: 2020 2023 2063 616c 6c5f 7061 7261 6d65     # call_parame
-0000ca50: 7465 7273 2069 7320 616e 2069 6e64 6578  ters is an index
-0000ca60: 2069 6e74 6f20 7468 6520 6672 6571 7565   into the freque
-0000ca70: 6e63 7920 616e 6420 6469 656c 6563 7472  ncy and dielectr
-0000ca80: 6963 2061 7272 6179 730a 2020 2020 2320  ic arrays.    # 
-0000ca90: 496e 2074 6865 2063 6173 6520 6f66 2042  In the case of B
-0000caa0: 7275 6767 656d 616e 2061 6e64 2063 6f68  ruggeman and coh
-0000cab0: 6572 656e 7420 7765 2063 616e 2075 7365  erent we can use
-0000cac0: 2074 6865 2070 7265 7669 6f75 7320 7265   the previous re
-0000cad0: 7375 6c74 2074 6f20 7374 6172 7420 7468  sult to start th
-0000cae0: 6520 6974 6572 6174 696f 6e2f 6d69 6e69  e iteration/mini
-0000caf0: 6d69 7361 7469 6f6e 0a20 2020 2023 2048  misation.    # H
-0000cb00: 6f77 6576 6572 2074 6f20 646f 2074 6869  owever to do thi
-0000cb10: 7320 7765 206e 6565 6420 736f 6d65 2073  s we need some s
-0000cb20: 6861 7265 6420 6d65 6d6f 7279 2c20 7468  hared memory, th
-0000cb30: 6973 2061 6c6c 6f63 6174 6564 2069 6e20  is allocated in 
-0000cb40: 7072 6576 696f 7573 5f73 6f6c 7574 696f  previous_solutio
-0000cb50: 6e5f 7368 6172 6564 0a20 2020 2076 2c63  n_shared.    v,c
-0000cb60: 7279 7374 616c 5f70 6572 6d69 7474 6976  rystal_permittiv
-0000cb70: 6974 7920 3d20 7061 7261 6d73 0a20 2020  ity = params.   
-0000cb80: 2076 6175 203d 2076 202a 2077 6176 656e   vau = v * waven
-0000cb90: 756d 6265 720a 2020 2020 2320 636f 6e76  umber.    # conv
-0000cba0: 6572 7420 7468 6520 7369 7a65 2074 6f20  ert the size to 
-0000cbb0: 6120 6469 6d65 6e73 696f 6e6c 6573 7320  a dimensionless 
-0000cbc0: 6e75 6d62 6572 2077 6869 6368 2069 7320  number which is 
-0000cbd0: 322a 7069 2a73 697a 652f 6c61 6d62 6461  2*pi*size/lambda
-0000cbe0: 0a20 2020 206c 616d 6264 615f 6d75 203d  .    lambda_mu =
-0000cbf0: 2031 2e30 4534 202f 2028 7620 2b20 312e   1.0E4 / (v + 1.
-0000cc00: 3065 2d31 3229 0a20 2020 2069 6620 7369  0e-12).    if si
-0000cc10: 7a65 5f6d 7520 3c20 312e 3065 2d31 323a  ze_mu < 1.0e-12:
-0000cc20: 0a20 2020 2020 2020 2073 697a 655f 6d75  .        size_mu
-0000cc30: 203d 2031 2e30 652d 3132 0a20 2020 2073   = 1.0e-12.    s
-0000cc40: 697a 6520 3d20 322e 302a 6e70 2e70 692a  ize = 2.0*np.pi*
-0000cc50: 7369 7a65 5f6d 7520 2f20 6c61 6d62 6461  size_mu / lambda
-0000cc60: 5f6d 750a 2020 2020 6461 7461 203d 2027  _mu.    data = '
-0000cc70: 270a 2020 2020 2320 4361 6c63 756c 6174  '.    # Calculat
-0000cc80: 6520 7468 6520 6566 6665 6374 206f 6620  e the effect of 
-0000cc90: 6275 6262 6c65 7320 696e 2074 6865 206d  bubbles in the m
-0000cca0: 6174 7269 7820 6279 2061 7373 756d 696e  atrix by assumin
-0000ccb0: 6720 7468 6579 2061 7265 2065 6d62 6564  g they are embed
-0000ccc0: 6465 6420 696e 2061 6e20 6566 6665 6374  ded in an effect
-0000ccd0: 6976 6520 6d65 6469 756d 2064 6566 696e  ive medium defin
-0000cce0: 6564 2061 626f 7665 0a20 2020 2072 6566  ed above.    ref
-0000ccf0: 7261 6374 6976 655f 696e 6465 7820 3d20  ractive_index = 
-0000cd00: 6d61 7468 2e73 7172 7428 6e70 2e74 7261  math.sqrt(np.tra
-0000cd10: 6365 2864 6965 6c65 6374 7269 635f 6d65  ce(dielectric_me
-0000cd20: 6469 756d 292f 332e 3029 0a20 2020 2069  dium)/3.0).    i
-0000cd30: 6620 7265 6672 6163 7469 7665 5f69 6e64  f refractive_ind
-0000cd40: 6578 2e69 6d61 6720 3c20 302e 303a 0a20  ex.imag < 0.0:. 
-0000cd50: 2020 2020 2020 2072 6566 7261 6374 6976         refractiv
-0000cd60: 655f 696e 6465 7820 3d20 7265 6672 6163  e_index = refrac
-0000cd70: 7469 7665 5f69 6e64 6578 2e63 6f6e 6a75  tive_index.conju
-0000cd80: 6761 7465 2829 0a20 2020 2069 6620 6275  gate().    if bu
-0000cd90: 6262 6c65 5f76 6620 3e20 303a 0a20 2020  bble_vf > 0:.   
-0000cda0: 2020 2020 2065 6666 6469 656c 6563 2c72       effdielec,r
-0000cdb0: 6566 7261 6374 6976 655f 696e 6465 7820  efractive_index 
-0000cdc0: 3d20 6361 6c63 756c 6174 655f 6275 6262  = calculate_bubb
-0000cdd0: 6c65 5f72 6566 7261 6374 6976 655f 696e  le_refractive_in
-0000cde0: 6465 7828 762c 2072 6566 7261 6374 6976  dex(v, refractiv
-0000cdf0: 655f 696e 6465 782c 2062 7562 626c 655f  e_index, bubble_
-0000ce00: 7666 2c20 6275 6262 6c65 5f72 6164 6975  vf, bubble_radiu
-0000ce10: 7329 0a20 2020 2020 2020 2064 6965 6c65  s).        diele
-0000ce20: 6374 7269 635f 6d65 6469 756d 203d 2065  ctric_medium = e
-0000ce30: 6666 6469 656c 6563 0a20 2020 2069 6620  ffdielec.    if 
-0000ce40: 6d65 7468 6f64 203d 3d20 2262 616c 616e  method == "balan
-0000ce50: 223a 0a20 2020 2020 2020 2065 6666 6469  ":.        effdi
-0000ce60: 656c 6563 203d 2062 616c 616e 2864 6965  elec = balan(die
-0000ce70: 6c65 6374 7269 635f 6d65 6469 756d 2c20  lectric_medium, 
-0000ce80: 6372 7973 7461 6c5f 7065 726d 6974 7469  crystal_permitti
-0000ce90: 7669 7479 2c20 7368 6170 652c 204c 2c20  vity, shape, L, 
-0000cea0: 7666 2c20 7369 7a65 290a 2020 2020 656c  vf, size).    el
-0000ceb0: 6966 206d 6574 686f 6420 3d3d 2022 6170  if method == "ap
-0000cec0: 2220 6f72 206d 6574 686f 6420 3d3d 2022  " or method == "
-0000ced0: 6176 6572 6167 6564 7065 726d 6974 7469  averagedpermitti
-0000cee0: 7669 7479 2220 6f72 206d 6574 686f 6420  vity" or method 
-0000cef0: 3d3d 2022 6176 6572 6167 6564 2070 6572  == "averaged per
-0000cf00: 6d69 7474 6976 6974 7922 206f 7220 6d65  mittivity" or me
-0000cf10: 7468 6f64 203d 3d20 2261 7665 7261 6765  thod == "average
-0000cf20: 2070 6572 6d69 7474 6976 6974 7922 3a0a   permittivity":.
-0000cf30: 2020 2020 2020 2020 2020 2020 6566 6664              effd
-0000cf40: 6965 6c65 6320 3d20 6176 6572 6167 6564  ielec = averaged
-0000cf50: 5f70 6572 6d69 7474 6976 6974 7928 6469  _permittivity(di
-0000cf60: 656c 6563 7472 6963 5f6d 6564 6975 6d2c  electric_medium,
-0000cf70: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
-0000cf80: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
-0000cf90: 2076 662c 2073 697a 6529 0a20 2020 2065   vf, size).    e
-0000cfa0: 6c69 6620 6d65 7468 6f64 203d 3d20 226d  lif method == "m
-0000cfb0: 6178 7765 6c6c 2220 6f72 206d 6574 686f  axwell" or metho
-0000cfc0: 6420 3d3d 2022 6d61 7877 656c 6c2d 6761  d == "maxwell-ga
-0000cfd0: 726e 6574 7422 3a0a 2020 2020 2020 2020  rnett":.        
-0000cfe0: 6566 6664 6965 6c65 6320 3d20 6d61 7877  effdielec = maxw
-0000cff0: 656c 6c28 6469 656c 6563 7472 6963 5f6d  ell(dielectric_m
-0000d000: 6564 6975 6d2c 2063 7279 7374 616c 5f70  edium, crystal_p
-0000d010: 6572 6d69 7474 6976 6974 792c 2073 6861  ermittivity, sha
-0000d020: 7065 2c20 4c2c 2076 662c 2073 697a 6529  pe, L, vf, size)
-0000d030: 0a20 2020 2065 6c69 6620 6d65 7468 6f64  .    elif method
-0000d040: 203d 3d20 226d 6178 7765 6c6c 5f73 6968   == "maxwell_sih
-0000d050: 766f 6c61 223a 0a20 2020 2020 2020 2065  vola":.        e
-0000d060: 6666 6469 656c 6563 203d 206d 6178 7765  ffdielec = maxwe
-0000d070: 6c6c 5f73 6968 766f 6c61 2864 6965 6c65  ll_sihvola(diele
-0000d080: 6374 7269 635f 6d65 6469 756d 2c20 6372  ctric_medium, cr
-0000d090: 7973 7461 6c5f 7065 726d 6974 7469 7669  ystal_permittivi
-0000d0a0: 7479 2c20 7368 6170 652c 204c 2c20 7666  ty, shape, L, vf
-0000d0b0: 2c20 7369 7a65 290a 2020 2020 656c 6966  , size).    elif
-0000d0c0: 206d 6574 686f 6420 3d3d 2022 636f 6865   method == "cohe
-0000d0d0: 7265 6e74 223a 0a20 2020 2020 2020 2065  rent":.        e
-0000d0e0: 6666 2020 3d20 7072 6576 696f 7573 5f73  ff  = previous_s
-0000d0f0: 6f6c 7574 696f 6e5f 7368 6172 6564 0a20  olution_shared. 
-0000d100: 2020 2020 2020 2069 6620 6e70 2e61 6273         if np.abs
-0000d110: 286e 702e 7472 6163 6528 6566 6629 2920  (np.trace(eff)) 
-0000d120: 3c20 312e 3065 2d38 3a0a 2020 2020 2020  < 1.0e-8:.      
-0000d130: 2020 2020 2020 6566 6620 3d20 6d61 7877        eff = maxw
-0000d140: 656c 6c28 6469 656c 6563 7472 6963 5f6d  ell(dielectric_m
-0000d150: 6564 6975 6d2c 2063 7279 7374 616c 5f70  edium, crystal_p
-0000d160: 6572 6d69 7474 6976 6974 792c 2073 6861  ermittivity, sha
-0000d170: 7065 2c20 4c2c 2076 662c 2073 697a 6529  pe, L, vf, size)
-0000d180: 0a20 2020 2020 2020 2065 6666 6469 656c  .        effdiel
-0000d190: 6563 203d 2063 6f68 6572 656e 7428 6469  ec = coherent(di
-0000d1a0: 656c 6563 7472 6963 5f6d 6564 6975 6d2c  electric_medium,
-0000d1b0: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
-0000d1c0: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
-0000d1d0: 2076 662c 2073 697a 652c 2065 6666 290a   vf, size, eff).
-0000d1e0: 2020 2020 2020 2020 7072 6576 696f 7573          previous
-0000d1f0: 5f73 6f6c 7574 696f 6e5f 7368 6172 6564  _solution_shared
-0000d200: 203d 2065 6666 6469 656c 6563 0a20 2020   = effdielec.   
-0000d210: 2065 6c69 6620 6d65 7468 6f64 203d 3d20   elif method == 
-0000d220: 2262 7275 6767 656d 616e 5f6d 696e 696d  "bruggeman_minim
-0000d230: 6973 6522 3a0a 2020 2020 2020 2020 6566  ise":.        ef
-0000d240: 6620 203d 2070 7265 7669 6f75 735f 736f  f  = previous_so
-0000d250: 6c75 7469 6f6e 5f73 6861 7265 640a 2020  lution_shared.  
-0000d260: 2020 2020 2020 6966 206e 702e 6162 7328        if np.abs(
-0000d270: 6e70 2e74 7261 6365 2865 6666 2929 203c  np.trace(eff)) <
-0000d280: 2031 2e30 652d 383a 0a20 2020 2020 2020   1.0e-8:.       
-0000d290: 2020 2020 2065 6666 203d 206d 6178 7765       eff = maxwe
-0000d2a0: 6c6c 2864 6965 6c65 6374 7269 635f 6d65  ll(dielectric_me
-0000d2b0: 6469 756d 2c20 6372 7973 7461 6c5f 7065  dium, crystal_pe
-0000d2c0: 726d 6974 7469 7669 7479 2c20 7368 6170  rmittivity, shap
-0000d2d0: 652c 204c 2c20 7666 2c20 7369 7a65 290a  e, L, vf, size).
-0000d2e0: 2020 2020 2020 2020 6566 6664 6965 6c65          effdiele
-0000d2f0: 6320 3d20 6272 7567 6765 6d61 6e5f 6d69  c = bruggeman_mi
-0000d300: 6e69 6d69 7365 2864 6965 6c65 6374 7269  nimise(dielectri
-0000d310: 635f 6d65 6469 756d 2c20 6372 7973 7461  c_medium, crysta
-0000d320: 6c5f 7065 726d 6974 7469 7669 7479 2c20  l_permittivity, 
-0000d330: 7368 6170 652c 204c 2c20 7666 2c20 7369  shape, L, vf, si
-0000d340: 7a65 2c20 6566 6629 0a20 2020 2020 2020  ze, eff).       
-0000d350: 2070 7265 7669 6f75 735f 736f 6c75 7469   previous_soluti
-0000d360: 6f6e 5f73 6861 7265 6420 3d20 6566 6664  on_shared = effd
-0000d370: 6965 6c65 630a 2020 2020 656c 6966 206d  ielec.    elif m
-0000d380: 6574 686f 6420 3d3d 2022 6272 7567 6765  ethod == "brugge
-0000d390: 6d61 6e22 206f 7220 6d65 7468 6f64 203d  man" or method =
-0000d3a0: 3d20 2262 7275 6767 656d 616e 5f69 7465  = "bruggeman_ite
-0000d3b0: 7222 3a0a 2020 2020 2020 2020 6566 6620  r":.        eff 
-0000d3c0: 203d 2070 7265 7669 6f75 735f 736f 6c75   = previous_solu
-0000d3d0: 7469 6f6e 5f73 6861 7265 640a 2020 2020  tion_shared.    
-0000d3e0: 2020 2020 6966 206e 702e 6162 7328 6e70      if np.abs(np
-0000d3f0: 2e74 7261 6365 2865 6666 2929 203c 2031  .trace(eff)) < 1
-0000d400: 2e30 652d 383a 0a20 2020 2020 2020 2020  .0e-8:.         
-0000d410: 2020 2065 6666 203d 206d 6178 7765 6c6c     eff = maxwell
-0000d420: 2864 6965 6c65 6374 7269 635f 6d65 6469  (dielectric_medi
-0000d430: 756d 2c20 6372 7973 7461 6c5f 7065 726d  um, crystal_perm
-0000d440: 6974 7469 7669 7479 2c20 7368 6170 652c  ittivity, shape,
-0000d450: 204c 2c20 7666 2c20 7369 7a65 290a 2020   L, vf, size).  
-0000d460: 2020 2020 2020 6566 6664 6965 6c65 6320        effdielec 
-0000d470: 3d20 6272 7567 6765 6d61 6e5f 6974 6572  = bruggeman_iter
-0000d480: 2864 6965 6c65 6374 7269 635f 6d65 6469  (dielectric_medi
-0000d490: 756d 2c20 6372 7973 7461 6c5f 7065 726d  um, crystal_perm
-0000d4a0: 6974 7469 7669 7479 2c20 7368 6170 652c  ittivity, shape,
-0000d4b0: 204c 2c20 7666 2c20 7369 7a65 2c20 6566   L, vf, size, ef
-0000d4c0: 6629 0a20 2020 2020 2020 2070 7265 7669  f).        previ
-0000d4d0: 6f75 735f 736f 6c75 7469 6f6e 5f73 6861  ous_solution_sha
-0000d4e0: 7265 6420 3d20 6566 6664 6965 6c65 630a  red = effdielec.
-0000d4f0: 2020 2020 656c 6966 206d 6574 686f 6420      elif method 
-0000d500: 3d3d 2022 616e 6973 6f74 726f 7069 632d  == "anisotropic-
-0000d510: 6d69 6522 3a0a 2020 2020 2020 2020 6566  mie":.        ef
-0000d520: 6664 6965 6c65 6320 3d20 616e 6973 6f74  fdielec = anisot
-0000d530: 726f 7069 635f 6d69 655f 7363 6174 7465  ropic_mie_scatte
-0000d540: 7269 6e67 2864 6965 6c65 6374 7269 635f  ring(dielectric_
-0000d550: 6d65 6469 756d 2c20 6372 7973 7461 6c5f  medium, crystal_
-0000d560: 7065 726d 6974 7469 7669 7479 2c20 7368  permittivity, sh
-0000d570: 6170 652c 204c 2c20 7666 2c20 7369 7a65  ape, L, vf, size
-0000d580: 2c20 7369 7a65 5f6d 752c 2073 697a 655f  , size_mu, size_
-0000d590: 6469 7374 7269 6275 7469 6f6e 5f73 6967  distribution_sig
-0000d5a0: 6d61 290a 2020 2020 656c 6966 206d 6574  ma).    elif met
-0000d5b0: 686f 6420 3d3d 2022 6d69 6522 3a0a 2020  hod == "mie":.  
-0000d5c0: 2020 2020 2020 6566 6664 6965 6c65 6320        effdielec 
-0000d5d0: 3d20 6d69 655f 7363 6174 7465 7269 6e67  = mie_scattering
-0000d5e0: 2864 6965 6c65 6374 7269 635f 6d65 6469  (dielectric_medi
-0000d5f0: 756d 2c20 6372 7973 7461 6c5f 7065 726d  um, crystal_perm
-0000d600: 6974 7469 7669 7479 2c20 7368 6170 652c  ittivity, shape,
-0000d610: 204c 2c20 7666 2c20 7369 7a65 2c20 7369   L, vf, size, si
-0000d620: 7a65 5f6d 752c 2073 697a 655f 6469 7374  ze_mu, size_dist
-0000d630: 7269 6275 7469 6f6e 5f73 6967 6d61 290a  ribution_sigma).
-0000d640: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d650: 2020 7072 696e 7428 2755 6e6b 6f77 6e20    print('Unkown 
-0000d660: 6469 656c 6563 7472 6963 206d 6574 686f  dielectric metho
-0000d670: 643a 207b 7d27 2e66 6f72 6d61 7428 6d65  d: {}'.format(me
-0000d680: 7468 6f64 2929 0a20 2020 2020 2020 2065  thod)).        e
-0000d690: 7869 7428 3129 0a20 2020 2023 2041 7665  xit(1).    # Ave
-0000d6a0: 7261 6765 206f 7665 7220 616c 6c20 6469  rage over all di
-0000d6b0: 7265 6374 696f 6e73 2062 7920 7461 6b69  rections by taki
-0000d6c0: 6e67 2074 6865 2074 7261 6365 0a20 2020  ng the trace.   
-0000d6d0: 2074 7261 6365 203d 2028 6566 6664 6965   trace = (effdie
-0000d6e0: 6c65 635b 302c 2030 5d20 2b20 6566 6664  lec[0, 0] + effd
-0000d6f0: 6965 6c65 635b 312c 2031 5d20 2b20 6566  ielec[1, 1] + ef
-0000d700: 6664 6965 6c65 635b 322c 2032 5d29 202f  fdielec[2, 2]) /
-0000d710: 2033 2e30 0a20 2020 2072 6566 7261 6374   3.0.    refract
-0000d720: 6976 655f 696e 6465 7820 3d20 6361 6c63  ive_index = calc
-0000d730: 756c 6174 655f 7265 6672 6163 7469 7665  ulate_refractive
-0000d740: 5f69 6e64 6578 2865 6666 6469 656c 6563  _index(effdielec
-0000d750: 290a 2020 2020 230a 2020 2020 2320 6162  ).    #.    # ab
-0000d760: 736f 7270 7469 6f6e 2063 6f65 6666 6963  sorption coeffic
-0000d770: 6965 6e74 2069 7320 6361 6c63 756c 6174  ient is calculat
-0000d780: 6564 2066 726f 6d20 7468 6520 696d 6167  ed from the imag
-0000d790: 696e 6172 7920 7265 6672 6163 7469 7665  inary refractive
-0000d7a0: 2069 6e64 6578 0a20 2020 2023 2073 6565   index.    # see
-0000d7b0: 2048 2e43 2e20 7661 6e20 6465 2048 756c   H.C. van de Hul
-0000d7c0: 7374 204c 6967 6874 2053 6361 7474 6572  st Light Scatter
-0000d7d0: 696e 6720 6279 2053 6d61 6c6c 2050 6172  ing by Small Par
-0000d7e0: 7469 636c 6573 202c 2070 6167 6520 3236  ticles , page 26
-0000d7f0: 370a 2020 2020 2320 5468 6973 2069 7320  7.    # This is 
-0000d800: 6469 6666 6572 656e 7420 6275 7420 7265  different but re
-0000d810: 6c61 7465 6420 746f 2047 656e 7a65 6c20  lated to Genzel 
-0000d820: 616e 6420 4d61 7274 696e 2045 7175 6174  and Martin Equat
-0000d830: 696f 6e20 3136 2c20 5068 7973 2e20 5374  ion 16, Phys. St
-0000d840: 6174 2e20 536f 6c2e 2035 3128 3139 3732  at. Sol. 51(1972
-0000d850: 2920 3931 2d0a 2020 2020 2320 4927 7665  ) 91-.    # I've
-0000d860: 2061 6464 2061 2066 6163 746f 7220 6f66   add a factor of
-0000d870: 206c 6f67 3130 2865 2920 6265 6361 7573   log10(e) becaus
-0000d880: 6520 7765 206e 6565 6420 746f 2061 7373  e we need to ass
-0000d890: 756d 6520 6120 6465 6361 6469 6320 4265  ume a decadic Be
-0000d8a0: 6572 2773 206c 6177 0a20 2020 2023 2075  er's law.    # u
-0000d8b0: 6e69 7473 2061 7265 2063 6d2d 310a 2020  nits are cm-1.  
-0000d8c0: 2020 6162 736f 7270 7469 6f6e 5f63 6f65    absorption_coe
-0000d8d0: 6666 6963 6965 6e74 203d 2076 202a 2034  fficient = v * 4
-0000d8e0: 2a50 4920 2a20 6e70 2e69 6d61 6728 7265  *PI * np.imag(re
-0000d8f0: 6672 6163 7469 7665 5f69 6e64 6578 2920  fractive_index) 
-0000d900: 2a20 6d61 7468 2e6c 6f67 3130 286d 6174  * math.log10(mat
-0000d910: 682e 6529 0a20 2020 2023 2075 6e69 7473  h.e).    # units
-0000d920: 2061 7265 2063 6d2d 3120 4c20 6d6f 6c65   are cm-1 L mole
-0000d930: 732d 310a 2020 2020 6d6f 6c61 725f 6162  s-1.    molar_ab
-0000d940: 736f 7270 7469 6f6e 5f63 6f65 6666 6963  sorption_coeffic
-0000d950: 6965 6e74 203d 2061 6273 6f72 7074 696f  ient = absorptio
-0000d960: 6e5f 636f 6566 6669 6369 656e 7420 2f20  n_coefficient / 
-0000d970: 636f 6e63 656e 7472 6174 696f 6e20 2f20  concentration / 
-0000d980: 7666 0a20 2020 2023 2063 616c 6375 6c61  vf.    # calcula
-0000d990: 7465 2074 6865 2041 5452 2072 6566 6c65  te the ATR refle
-0000d9a0: 6374 616e 6365 0a20 2020 2073 7061 7472  ctance.    spatr
-0000d9b0: 203d 2072 6566 6c65 6374 616e 6365 5f61   = reflectance_a
-0000d9c0: 7472 2872 6566 7261 6374 6976 655f 696e  tr(refractive_in
-0000d9d0: 6465 782c 6174 7250 6572 6d69 7474 6976  dex,atrPermittiv
-0000d9e0: 6974 792c 6174 7254 6865 7461 2c61 7472  ity,atrTheta,atr
-0000d9f0: 5350 6f6c 290a 2020 2020 7265 7475 726e  SPol).    return
-0000da00: 2076 2c6d 6574 686f 642c 7369 7a65 5f6d   v,method,size_m
-0000da10: 752c 7369 7a65 5f64 6973 7472 6962 7574  u,size_distribut
-0000da20: 696f 6e5f 7369 676d 612c 7368 6170 652c  ion_sigma,shape,
-0000da30: 6461 7461 2c74 7261 6365 2c61 6273 6f72  data,trace,absor
-0000da40: 7074 696f 6e5f 636f 6566 6669 6369 656e  ption_coefficien
-0000da50: 742c 6d6f 6c61 725f 6162 736f 7270 7469  t,molar_absorpti
-0000da60: 6f6e 5f63 6f65 6666 6963 6965 6e74 2c73  on_coefficient,s
-0000da70: 7061 7472 0a0a 6465 6620 6361 6c63 756c  patr..def calcul
-0000da80: 6174 655f 6275 6262 6c65 5f72 6566 7261  ate_bubble_refra
-0000da90: 6374 6976 655f 696e 6465 7828 765f 636d  ctive_index(v_cm
-0000daa0: 312c 2072 695f 6d65 6469 756d 2c20 7666  1, ri_medium, vf
-0000dab0: 2c20 7261 6469 7573 5f6d 7529 3a0a 2020  , radius_mu):.  
-0000dac0: 2020 2222 2243 616c 6375 6c61 7465 2074    """Calculate t
-0000dad0: 6865 2073 6361 7474 6572 696e 6720 6672  he scattering fr
-0000dae0: 6f6d 2062 7562 626c 6573 2065 6d62 6564  om bubbles embed
-0000daf0: 6465 6420 696e 2061 2070 6f73 7369 626c  ded in a possibl
-0000db00: 792c 2063 6f6d 706c 6578 2064 6965 6c65  y, complex diele
-0000db10: 6374 7269 6320 6174 2076 5f63 6d31 0a20  ctric at v_cm1. 
-0000db20: 2020 2020 2020 765f 636d 3120 6973 2074        v_cm1 is t
-0000db30: 6865 2066 7265 7175 656e 6379 2069 6e20  he frequency in 
-0000db40: 636d 2d31 0a20 2020 2020 2020 7269 5f6d  cm-1.       ri_m
-0000db50: 6564 6975 6d20 6973 2074 6865 2072 6566  edium is the ref
-0000db60: 7261 6374 6976 6520 696e 6465 7820 6f66  ractive index of
-0000db70: 2074 6865 206d 6564 6975 6d0a 2020 2020   the medium.    
-0000db80: 2020 2076 6620 6973 2074 6865 2076 6f6c     vf is the vol
-0000db90: 756d 6520 6672 6163 7469 6f6e 206f 6620  ume fraction of 
-0000dba0: 6275 6262 6c65 730a 2020 2020 2020 2072  bubbles.       r
-0000dbb0: 6164 6975 735f 6d75 2069 7320 7468 6520  adius_mu is the 
-0000dbc0: 7261 6469 7573 206f 6620 7468 6520 6275  radius of the bu
-0000dbd0: 6262 6c65 7320 696e 206d 6963 726f 6e73  bbles in microns
-0000dbe0: 0a20 2020 2020 2020 5468 6520 726f 7574  .       The rout
-0000dbf0: 696e 6520 7265 7475 726e 7320 7468 6520  ine returns the 
-0000dc00: 6566 6665 6374 6976 6520 6469 656c 6563  effective dielec
-0000dc10: 7472 6963 2063 6f6e 7374 616e 7420 616e  tric constant an
-0000dc20: 6420 7468 6520 6173 736f 6369 6174 6564  d the associated
-0000dc30: 2072 6566 7261 6374 6976 6520 696e 6465   refractive inde
-0000dc40: 7822 2222 0a20 2020 2023 0a20 2020 2023  x""".    #.    #
-0000dc50: 2057 6520 6e65 6564 2074 6f20 7461 6b65   We need to take
-0000dc60: 6e20 6163 636f 756e 7420 6f66 2074 6865  n account of the
-0000dc70: 2063 6861 6e67 6520 696e 2077 6176 656c   change in wavel
-0000dc80: 656e 6774 6820 616e 6420 7468 6520 6368  ength and the ch
-0000dc90: 616e 6765 2069 6e20 7369 7a65 2070 6172  ange in size par
-0000dca0: 616d 6574 6572 2064 7565 2074 6f20 7468  ameter due to th
-0000dcb0: 650a 2020 2020 2320 4e6f 6e65 2075 6e69  e.    # None uni
-0000dcc0: 7420 7661 6c75 6520 6f66 2074 6865 2064  t value of the d
-0000dcd0: 6965 6c65 6374 7269 6320 6f66 2074 6865  ielectric of the
-0000dce0: 2065 6d62 6564 6469 6e67 206d 6564 6975   embedding mediu
-0000dcf0: 6d0a 2020 2020 2320 5468 6520 7369 7a65  m.    # The size
-0000dd00: 2070 6172 616d 6574 6572 2069 7320 3270   parameter is 2p
-0000dd10: 6920 7220 2f20 6c61 6d62 6461 0a20 2020  i r / lambda.   
-0000dd20: 2023 2054 6865 2065 6666 6563 7469 7665   # The effective
-0000dd30: 206c 616d 6264 6120 696e 2074 6865 2073   lambda in the s
-0000dd40: 7570 706f 7274 696e 6720 6d65 6469 756d  upporting medium
-0000dd50: 2069 7320 6c61 6d62 6461 202f 2073 7172   is lambda / sqr
-0000dd60: 7428 656d 6564 6975 6d29 0a20 2020 2023  t(emedium).    #
-0000dd70: 2057 6865 7265 2074 6865 2072 6566 7261   Where the refra
-0000dd80: 6374 6976 6520 696e 6465 7820 6973 2074  ctive index is t
-0000dd90: 616b 656e 2074 6f20 6265 2073 7172 7428  aken to be sqrt(
-0000dda0: 656d 6564 6975 6d29 2028 6e6f 6e20 6d61  emedium) (non ma
-0000ddb0: 676e 6574 6963 206d 6174 6572 6961 6c73  gnetic materials
-0000ddc0: 290a 2020 2020 230a 2020 2020 6966 2076  ).    #.    if v
-0000ddd0: 5f63 6d31 203e 2030 3a0a 2020 2020 2020  _cm1 > 0:.      
-0000dde0: 2020 6c61 6d62 6461 5f76 6163 7575 6d5f    lambda_vacuum_
-0000ddf0: 6e6d 203d 2031 2e30 4533 2a31 2e30 4534  nm = 1.0E3*1.0E4
-0000de00: 202f 2076 5f63 6d31 0a20 2020 2065 6c73   / v_cm1.    els
-0000de10: 653a 0a20 2020 2020 2020 206c 616d 6264  e:.        lambd
-0000de20: 615f 7661 6375 756d 5f6e 6d20 3d20 312e  a_vacuum_nm = 1.
-0000de30: 3045 3939 0a20 2020 2023 2054 7265 6174  0E99.    # Treat
-0000de40: 2074 6865 2062 7562 626c 6520 6173 2074   the bubble as t
-0000de50: 686f 7567 6820 6974 2069 7320 6169 7220  hough it is air 
-0000de60: 696e 206d 6174 7269 780a 2020 2020 2320  in matrix.    # 
-0000de70: 5468 6520 6566 6665 6374 6976 6520 7761  The effective wa
-0000de80: 7665 206e 756d 6265 7220 6b20 3d20 7371  ve number k = sq
-0000de90: 7274 2865 6d65 6469 756d 292a 3270 692a  rt(emedium)*2pi*
-0000dea0: 762f 6320 2863 6f6d 706c 6578 2129 0a20  v/c (complex!). 
-0000deb0: 2020 2072 6164 6975 735f 6e6d 203d 2072     radius_nm = r
-0000dec0: 6164 6975 735f 6d75 202a 2031 3030 300a  adius_mu * 1000.
-0000ded0: 2020 2020 2320 766f 6c75 6d65 206f 6620      # volume of 
-0000dee0: 6120 6275 6262 6c65 2069 6e20 6e6d 5e33  a bubble in nm^3
-0000def0: 0a20 2020 2056 5f6e 6d20 3d20 342e 302f  .    V_nm = 4.0/
-0000df00: 332e 3020 2a20 5049 202a 2072 6164 6975  3.0 * PI * radiu
-0000df10: 735f 6e6d 202a 2072 6164 6975 735f 6e6d  s_nm * radius_nm
-0000df20: 202a 2072 6164 6975 735f 6e6d 0a20 2020   * radius_nm.   
-0000df30: 2023 204e 756d 6265 7220 6465 6e73 6974   # Number densit
-0000df40: 7920 6f66 2062 7562 626c 6573 2028 6e75  y of bubbles (nu
-0000df50: 6d62 6572 202f 206e 6d5e 3329 0a20 2020  mber / nm^3).   
-0000df60: 204e 5f6e 6d20 3d20 7666 202f 2056 5f6e   N_nm = vf / V_n
-0000df70: 6d0a 2020 2020 6b5f 6e6d 203d 2077 6174  m.    k_nm = wat
-0000df80: 6572 6d61 6e5f 7472 7565 6c6c 5f73 6361  erman_truell_sca
-0000df90: 7474 6572 696e 6728 6c61 6d62 6461 5f76  ttering(lambda_v
-0000dfa0: 6163 7575 6d5f 6e6d 2c20 4e5f 6e6d 2c20  acuum_nm, N_nm, 
-0000dfb0: 7261 6469 7573 5f6e 6d2c 2072 695f 6d65  radius_nm, ri_me
-0000dfc0: 6469 756d 290a 2020 2020 2320 6b5f 6e6d  dium).    # k_nm
-0000dfd0: 203d 2066 6f6c 6479 5f73 6361 7474 6572   = foldy_scatter
-0000dfe0: 696e 6728 6c61 6d62 6461 5f76 6163 7575  ing(lambda_vacuu
-0000dff0: 6d5f 6e6d 2c20 4e5f 6e6d 2c20 7261 6469  m_nm, N_nm, radi
-0000e000: 7573 5f6e 6d2c 2072 695f 6d65 6469 756d  us_nm, ri_medium
-0000e010: 290a 2020 2020 7269 5f6d 6564 6975 6d20  ).    ri_medium 
-0000e020: 3d20 6b5f 6e6d 202a 6c61 6d62 6461 5f76  = k_nm *lambda_v
-0000e030: 6163 7575 6d5f 6e6d 202f 2028 322a 5049  acuum_nm / (2*PI
-0000e040: 290a 2020 2020 6566 665f 6d65 6469 756d  ).    eff_medium
-0000e050: 203d 2072 695f 6d65 6469 756d 202a 2072   = ri_medium * r
-0000e060: 695f 6d65 6469 756d 0a20 2020 2065 6666  i_medium.    eff
-0000e070: 6469 656c 6563 203d 206e 702e 6172 7261  dielec = np.arra
-0000e080: 7928 5b5b 6566 665f 6d65 6469 756d 2c20  y([[eff_medium, 
-0000e090: 302c 2030 5d2c 205b 302c 2065 6666 5f6d  0, 0], [0, eff_m
-0000e0a0: 6564 6975 6d2c 2030 5d2c 205b 302c 2030  edium, 0], [0, 0
-0000e0b0: 2c20 6566 665f 6d65 6469 756d 5d5d 290a  , eff_medium]]).
-0000e0c0: 2020 2020 7265 7475 726e 2065 6666 6469      return effdi
-0000e0d0: 656c 6563 2c72 695f 6d65 6469 756d 0a0a  elec,ri_medium..
-0000e0e0: 6465 6620 666f 6c64 795f 7363 6174 7465  def foldy_scatte
-0000e0f0: 7269 6e67 286c 616d 6264 615f 7661 6375  ring(lambda_vacu
-0000e100: 756d 5f6e 6d2c 204e 5f6e 6d2c 7261 6469  um_nm, N_nm,radi
-0000e110: 7573 5f6e 6d2c 7269 5f6d 6564 6975 6d29  us_nm,ri_medium)
-0000e120: 3a0a 2020 2020 230a 2020 2020 2320 536f  :.    #.    # So
-0000e130: 6c76 6520 7468 6520 666f 6c64 7920 6571  lve the foldy eq
-0000e140: 7561 7469 6f6e 2066 6f72 2073 6361 7474  uation for scatt
-0000e150: 6572 696e 6720 6f66 2061 6e20 6169 7220  ering of an air 
-0000e160: 6275 6262 6c65 2065 6d62 6564 6465 6420  bubble embedded 
-0000e170: 696e 2061 206c 6f73 7379 206d 6564 6975  in a lossy mediu
-0000e180: 6d0a 2020 2020 2320 4e5f 6e6d 2069 7320  m.    # N_nm is 
-0000e190: 7468 6520 6e75 6d62 6572 2064 656e 7369  the number densi
-0000e1a0: 7479 206f 6620 6275 6262 6c65 7320 696e  ty of bubbles in
-0000e1b0: 2074 6865 2076 6f6c 756d 6520 6e6d 5e33   the volume nm^3
-0000e1c0: 0a20 2020 2023 206b 5f6e 6d20 6973 2074  .    # k_nm is t
-0000e1d0: 6865 2077 6176 656e 756d 6265 7220 6f66  he wavenumber of
-0000e1e0: 2074 6865 2069 6e63 6f6d 696e 6720 7761   the incoming wa
-0000e1f0: 7665 2028 636f 6d70 6c65 7829 0a20 2020  ve (complex).   
-0000e200: 2023 2072 6164 6975 735f 6e6d 2069 7320   # radius_nm is 
-0000e210: 7468 6520 7261 6469 7573 206f 6620 7468  the radius of th
-0000e220: 6520 6275 6262 6c65 0a20 2020 2023 2072  e bubble.    # r
-0000e230: 695f 6d65 6469 756d 2069 7320 7468 6520  i_medium is the 
-0000e240: 7265 6672 6163 7469 7665 2069 6e64 6578  refractive index
-0000e250: 206f 6620 7468 6520 6d65 6469 756d 2074   of the medium t
-0000e260: 6865 2062 7562 626c 6520 6973 2069 6e0a  he bubble is in.
-0000e270: 2020 2020 230a 2020 2020 230a 2020 2020      #.    #.    
-0000e280: 6b5f 6e6d 203d 2032 2a50 492a 7269 5f6d  k_nm = 2*PI*ri_m
-0000e290: 6564 6975 6d2f 6c61 6d62 6461 5f76 6163  edium/lambda_vac
-0000e2a0: 7575 6d5f 6e6d 0a20 2020 2023 2054 6865  uum_nm.    # The
-0000e2b0: 2073 697a 6520 7061 7261 6d65 7465 7220   size parameter 
-0000e2c0: 6973 206e 6f77 2061 6c73 6f20 636f 6d70  is now also comp
-0000e2d0: 6c65 7820 616e 6420 6469 6d65 6e73 696f  lex and dimensio
-0000e2e0: 6e6c 6573 730a 2020 2020 7369 7a65 203d  nless.    size =
-0000e2f0: 206b 5f6e 6d2a 7261 6469 7573 5f6e 6d0a   k_nm*radius_nm.
-0000e300: 2020 2020 7265 6672 6163 7469 7665 5f69      refractive_i
-0000e310: 6e64 6578 203d 2031 2e30 202f 2072 695f  ndex = 1.0 / ri_
-0000e320: 6d65 6469 756d 0a20 2020 2023 2043 616c  medium.    # Cal
-0000e330: 6375 6c61 7465 2074 6865 2066 6f72 7761  culate the forwa
-0000e340: 7264 2061 6e64 2062 6163 6b77 6172 6420  rd and backward 
-0000e350: 7363 6174 7465 7269 6e67 2061 6d70 6c69  scattering ampli
-0000e360: 7475 6465 0a20 2020 2073 3130 2c73 3230  tude.    s10,s20
-0000e370: 203d 204d 6965 2e4d 6965 5331 5332 2872   = Mie.MieS1S2(r
-0000e380: 6566 7261 6374 6976 655f 696e 6465 782c  efractive_index,
-0000e390: 2073 697a 652a 7269 5f6d 6564 6975 6d2c   size*ri_medium,
-0000e3a0: 2031 290a 2020 2020 6920 3d20 636f 6d70   1).    i = comp
-0000e3b0: 6c65 7828 302c 3129 0a20 2020 2066 3020  lex(0,1).    f0 
-0000e3c0: 3d20 6920 2a20 7331 3020 2f20 6b5f 6e6d  = i * s10 / k_nm
-0000e3d0: 0a20 2020 206e 6577 5f6b 203d 206e 702e  .    new_k = np.
-0000e3e0: 7371 7274 2820 6b5f 6e6d 2a6b 5f6e 6d20  sqrt( k_nm*k_nm 
-0000e3f0: 2b20 342a 5049 2a4e 5f6e 6d2a 6630 2029  + 4*PI*N_nm*f0 )
-0000e400: 0a20 2020 2069 6620 6e65 775f 6b2e 696d  .    if new_k.im
-0000e410: 6167 203c 2030 2e30 3a0a 2020 2020 2020  ag < 0.0:.      
-0000e420: 2020 6e65 775f 6b20 3d20 6e65 775f 6b2e    new_k = new_k.
-0000e430: 636f 6e6a 7567 6174 6528 290a 2020 2020  conjugate().    
-0000e440: 7265 7475 726e 206e 6577 5f6b 0a0a 6465  return new_k..de
-0000e450: 6620 7761 7465 726d 616e 5f74 7275 656c  f waterman_truel
-0000e460: 6c5f 7363 6174 7465 7269 6e67 286c 616d  l_scattering(lam
-0000e470: 6264 615f 7661 6375 756d 5f6e 6d2c 204e  bda_vacuum_nm, N
-0000e480: 5f6e 6d2c 7261 6469 7573 5f6e 6d2c 7269  _nm,radius_nm,ri
-0000e490: 5f6d 6564 6975 6d29 3a0a 2020 2020 230a  _medium):.    #.
-0000e4a0: 2020 2020 2320 536f 6c76 6520 7468 6520      # Solve the 
-0000e4b0: 7761 7465 726d 616e 2074 7275 656c 6c20  waterman truell 
-0000e4c0: 6571 7561 7469 6f6e 2066 6f72 2073 6361  equation for sca
-0000e4d0: 7474 6572 696e 6720 6f66 2061 6e20 6169  ttering of an ai
-0000e4e0: 7220 6275 6262 6c65 2065 6d62 6564 6465  r bubble embedde
-0000e4f0: 6420 696e 2061 206c 6f73 7379 206d 6564  d in a lossy med
-0000e500: 6975 6d0a 2020 2020 2320 4e5f 6e6d 2069  ium.    # N_nm i
-0000e510: 7320 7468 6520 6e75 6d62 6572 2064 656e  s the number den
-0000e520: 7369 7479 206f 6620 6275 6262 6c65 7320  sity of bubbles 
-0000e530: 696e 2074 6865 2076 6f6c 756d 6520 6e6d  in the volume nm
-0000e540: 5e33 0a20 2020 2023 206b 5f6e 6d20 6973  ^3.    # k_nm is
-0000e550: 2074 6865 2077 6176 656e 756d 6265 7220   the wavenumber 
-0000e560: 6f66 2074 6865 2069 6e63 6f6d 696e 6720  of the incoming 
-0000e570: 7761 7665 2028 636f 6d70 6c65 7829 0a20  wave (complex). 
-0000e580: 2020 2023 2072 6164 6975 735f 6e6d 2069     # radius_nm i
-0000e590: 7320 7468 6520 7261 6469 7573 206f 6620  s the radius of 
-0000e5a0: 7468 6520 6275 6262 6c65 0a20 2020 2023  the bubble.    #
-0000e5b0: 2072 695f 6d65 6469 756d 2069 7320 7468   ri_medium is th
-0000e5c0: 6520 7265 6672 6163 7469 7665 2069 6e64  e refractive ind
-0000e5d0: 6578 206f 6620 7468 6520 6d65 6469 756d  ex of the medium
-0000e5e0: 2074 6865 2062 7562 626c 6520 6973 2069   the bubble is i
-0000e5f0: 6e0a 2020 2020 230a 2020 2020 230a 2020  n.    #.    #.  
-0000e600: 2020 6b5f 6e6d 203d 2032 2a50 492a 7269    k_nm = 2*PI*ri
-0000e610: 5f6d 6564 6975 6d2f 6c61 6d62 6461 5f76  _medium/lambda_v
-0000e620: 6163 7575 6d5f 6e6d 0a20 2020 2023 2054  acuum_nm.    # T
-0000e630: 6865 2073 697a 6520 7061 7261 6d65 7465  he size paramete
-0000e640: 7220 6973 206e 6f77 2061 6c73 6f20 636f  r is now also co
-0000e650: 6d70 6c65 7820 616e 6420 6469 6d65 6e73  mplex and dimens
-0000e660: 696f 6e6c 6573 730a 2020 2020 7369 7a65  ionless.    size
-0000e670: 203d 206b 5f6e 6d2a 7261 6469 7573 5f6e   = k_nm*radius_n
-0000e680: 6d0a 2020 2020 7265 6672 6163 7469 7665  m.    refractive
-0000e690: 5f69 6e64 6578 203d 2031 2e30 202f 2072  _index = 1.0 / r
-0000e6a0: 695f 6d65 6469 756d 0a20 2020 2023 2043  i_medium.    # C
-0000e6b0: 616c 6375 6c61 7465 2074 6865 2066 6f72  alculate the for
-0000e6c0: 7761 7264 2061 6e64 2062 6163 6b77 6172  ward and backwar
-0000e6d0: 6420 7363 6174 7465 7269 6e67 2061 6d70  d scattering amp
-0000e6e0: 6c69 7475 6465 0a20 2020 2073 3130 2c73  litude.    s10,s
-0000e6f0: 3230 203d 204d 6965 2e4d 6965 5331 5332  20 = Mie.MieS1S2
-0000e700: 2872 6566 7261 6374 6976 655f 696e 6465  (refractive_inde
-0000e710: 782c 2073 697a 652a 7269 5f6d 6564 6975  x, size*ri_mediu
-0000e720: 6d2c 2031 290a 2020 2020 7331 312c 7332  m, 1).    s11,s2
-0000e730: 3120 3d20 4d69 652e 4d69 6553 3153 3228  1 = Mie.MieS1S2(
-0000e740: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
-0000e750: 2c20 7369 7a65 2a72 695f 6d65 6469 756d  , size*ri_medium
-0000e760: 2c2d 3129 0a20 2020 2023 2074 6865 206e  ,-1).    # the n
-0000e770: 6f72 6d61 6c69 7361 7469 6f6e 2062 7920  ormalisation by 
-0000e780: 312f 6b5f 6e6d 2069 7320 7065 7266 6f72  1/k_nm is perfor
-0000e790: 6d65 6420 7768 656e 2066 2069 7320 6361  med when f is ca
-0000e7a0: 6c63 756c 6174 6564 0a20 2020 2069 203d  lculated.    i =
-0000e7b0: 2063 6f6d 706c 6578 2830 2c31 290a 2020   complex(0,1).  
-0000e7c0: 2020 6630 203d 2069 2a73 3130 0a20 2020    f0 = i*s10.   
-0000e7d0: 2066 3120 3d20 692a 7331 310a 2020 2020   f1 = i*s11.    
-0000e7e0: 2320 7072 696e 7428 2757 6174 6572 6d61  # print('Waterma
-0000e7f0: 6e5f 7472 7565 6c6c 272c 6162 7328 6630  n_truell',abs(f0
-0000e800: 2b66 3129 290a 2020 2020 6b32 203d 206b  +f1)).    k2 = k
-0000e810: 5f6e 6d2a 6b5f 6e6d 0a20 2020 2066 203d  _nm*k_nm.    f =
-0000e820: 2032 2a50 492a 4e5f 6e6d 2f28 6b5f 6e6d   2*PI*N_nm/(k_nm
-0000e830: 2a6b 5f6e 6d2a 6b5f 6e6d 290a 2020 2020  *k_nm*k_nm).    
-0000e840: 6e65 775f 6b20 3d20 6e70 2e73 7172 7428  new_k = np.sqrt(
-0000e850: 206b 3220 2a20 2820 2831 2b66 2a66 3029   k2 * ( (1+f*f0)
-0000e860: 2a28 312b 662a 6630 2920 2d20 662a 6631  *(1+f*f0) - f*f1
-0000e870: 2a66 2a66 3120 2920 290a 2020 2020 6966  *f*f1 ) ).    if
-0000e880: 206e 6577 5f6b 2e69 6d61 6720 3c20 302e   new_k.imag < 0.
-0000e890: 303a 0a20 2020 2020 2020 206e 6577 5f6b  0:.        new_k
-0000e8a0: 203d 206e 6577 5f6b 2e63 6f6e 6a75 6761   = new_k.conjuga
-0000e8b0: 7465 2829 0a20 2020 2072 6574 7572 6e20  te().    return 
-0000e8c0: 6e65 775f 6b0a 0a64 6566 2063 616c 6375  new_k..def calcu
-0000e8d0: 6c61 7465 5f63 656e 7472 655f 6f66 5f6d  late_centre_of_m
-0000e8e0: 6173 7328 7879 7a73 2c20 6d61 7373 6573  ass(xyzs, masses
-0000e8f0: 293a 0a20 2020 2727 2743 616c 6375 6c61  ):.   '''Calcula
-0000e900: 7465 2063 656e 7472 6520 6f66 206d 6173  te centre of mas
-0000e910: 7327 2727 0a20 2020 636d 203d 206e 702e  s'''.   cm = np.
-0000e920: 7a65 726f 7328 3329 0a20 2020 6d61 7373  zeros(3).   mass
-0000e930: 203d 2030 2e30 0a20 2020 666f 7220 6d2c   = 0.0.   for m,
-0000e940: 7879 7a20 696e 207a 6970 286d 6173 7365  xyz in zip(masse
-0000e950: 732c 7879 7a73 293a 0a20 2020 2020 2020  s,xyzs):.       
-0000e960: 6d61 7373 202b 3d20 6d0a 2020 2020 2020  mass += m.      
-0000e970: 2063 6d20 2020 2b3d 206d 2a78 797a 0a20   cm   += m*xyz. 
-0000e980: 2020 636d 202f 3d20 6d61 7373 0a20 2020    cm /= mass.   
-0000e990: 7265 7475 726e 206d 6173 732c 636d 0a0a  return mass,cm..
-0000e9a0: 6465 6620 6f72 7468 6f67 6f6e 616c 6973  def orthogonalis
-0000e9b0: 655f 7072 6f6a 6563 7469 6f6e 5f6f 7065  e_projection_ope
-0000e9c0: 7261 746f 7228 7073 293a 0a20 2020 2727  rator(ps):.   ''
-0000e9d0: 274f 7274 686f 676f 6e61 6c69 7365 2074  'Orthogonalise t
-0000e9e0: 6865 2070 726f 6a65 6374 696f 6e20 6f70  he projection op
-0000e9f0: 6572 6174 6f72 7320 7073 2727 270a 2020  erators ps'''.  
-0000ea00: 2023 2054 6865 2070 726f 6a65 6374 696f   # The projectio
-0000ea10: 6e20 6f70 6572 6174 6f72 2068 6173 2064  n operator has d
-0000ea20: 696d 656e 7369 6f6e 205b 362c 6e61 746f  imension [6,nato
-0000ea30: 6d73 2a33 5d0a 2020 206d 6178 6379 6320  ms*3].   maxcyc 
-0000ea40: 3d20 3130 0a20 2020 6379 636c 6520 3d20  = 10.   cycle = 
-0000ea50: 300a 2020 206d 6178 5f6f 7665 726c 6170  0.   max_overlap
-0000ea60: 203d 2031 2e30 0a20 2020 7768 696c 6520   = 1.0.   while 
-0000ea70: 6379 636c 6520 3c20 6d61 7863 7963 2061  cycle < maxcyc a
-0000ea80: 6e64 206d 6178 5f6f 7665 726c 6170 203e  nd max_overlap >
-0000ea90: 2031 2e30 452d 383a 0a20 2020 2020 2020   1.0E-8:.       
-0000eaa0: 6379 636c 6520 2b3d 2031 0a20 2020 2020  cycle += 1.     
-0000eab0: 2020 6d61 785f 6f76 6572 6c61 7020 3d20    max_overlap = 
-0000eac0: 302e 300a 2020 2020 2020 2066 6f72 2069  0.0.       for i
-0000ead0: 2c70 2069 6e20 656e 756d 6572 6174 6528  ,p in enumerate(
-0000eae0: 7073 293a 0a20 2020 2020 2020 2020 2020  ps):.           
-0000eaf0: 2320 4e6f 726d 616c 6973 6520 7468 6520  # Normalise the 
-0000eb00: 7072 6f6a 6563 7469 6f6e 206f 7065 7261  projection opera
-0000eb10: 746f 720a 2020 2020 2020 2020 2020 2061  tor.           a
-0000eb20: 6e6f 726d 203d 206e 702e 646f 7428 702c  norm = np.dot(p,
-0000eb30: 7029 0a20 2020 2020 2020 2020 2020 7368  p).           sh
-0000eb40: 6966 7420 3d20 302e 300a 2020 2020 2020  ift = 0.0.      
-0000eb50: 2020 2020 2069 6620 616e 6f72 6d20 3c20       if anorm < 
-0000eb60: 312e 3065 2d31 323a 0a20 2020 2020 2020  1.0e-12:.       
-0000eb70: 2020 2020 2020 2020 7368 6966 7420 3d20          shift = 
-0000eb80: 312e 3045 2d31 320a 2020 2020 2020 2020  1.0E-12.        
-0000eb90: 2020 2070 203d 2070 202f 206e 702e 7371     p = p / np.sq
-0000eba0: 7274 286e 702e 646f 7428 702c 7029 202b  rt(np.dot(p,p) +
-0000ebb0: 2073 6869 6674 2029 0a20 2020 2020 2020   shift ).       
-0000ebc0: 2020 2020 7073 5b69 5d20 3d20 700a 2020      ps[i] = p.  
-0000ebd0: 2020 2020 2020 2020 2066 6f72 206a 2c71           for j,q
-0000ebe0: 2069 6e20 656e 756d 6572 6174 6528 7073   in enumerate(ps
-0000ebf0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ec00: 2020 6966 206a 203e 2069 3a0a 2020 2020    if j > i:.    
-0000ec10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ec20: 2047 7261 6d6d 2053 6368 6d69 6474 206f   Gramm Schmidt o
-0000ec30: 7274 686f 676f 6e6f 616c 6973 6174 696f  rthogonoalisatio
-0000ec40: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000ec50: 2020 2020 2064 6f74 7072 6f64 203d 206e       dotprod = n
-0000ec60: 702e 646f 7428 702c 7129 0a20 2020 2020  p.dot(p,q).     
-0000ec70: 2020 2020 2020 2020 2020 2020 2020 7073                ps
-0000ec80: 5b6a 5d20 3d20 7120 2d20 646f 7470 726f  [j] = q - dotpro
-0000ec90: 642a 700a 2020 2020 2020 2020 2020 2020  d*p.            
-0000eca0: 2020 2020 2020 2069 6620 6d61 785f 6f76         if max_ov
-0000ecb0: 6572 6c61 7020 3c20 646f 7470 726f 643a  erlap < dotprod:
-0000ecc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ecd0: 2020 2020 2020 2020 6d61 785f 6f76 6572          max_over
-0000ece0: 6c61 7020 3d20 646f 7470 726f 640a 2020  lap = dotprod.  
-0000ecf0: 2069 6620 6379 636c 6520 3e3d 206d 6178   if cycle >= max
-0000ed00: 6379 633a 0a20 2020 2020 2020 7072 696e  cyc:.       prin
-0000ed10: 7428 2757 4152 4e49 4e47 2053 6368 6d69  t('WARNING Schmi
-0000ed20: 6474 204f 7274 686f 676f 6e61 6c69 7361  dt Orthogonalisa
-0000ed30: 7469 6f6e 2046 6169 6c65 6427 2c20 6d61  tion Failed', ma
-0000ed40: 785f 6f76 6572 6c61 7029 0a20 2020 2020  x_overlap).     
-0000ed50: 2020 6578 6974 2829 0a20 2020 7265 7475    exit().   retu
-0000ed60: 726e 2070 730a 0a64 6566 2063 6f6e 7374  rn ps..def const
-0000ed70: 7275 6374 5f70 726f 6a65 6374 696f 6e5f  ruct_projection_
-0000ed80: 6f70 6572 6174 6f72 2861 746f 6d73 2c20  operator(atoms, 
-0000ed90: 7879 7a73 2c20 6d61 7373 6573 2c20 6e61  xyzs, masses, na
-0000eda0: 7473 293a 0a20 2020 2727 2743 6f6e 7374  ts):.   '''Const
-0000edb0: 7275 6374 2074 6865 2070 726f 6a65 6374  ruct the project
-0000edc0: 696f 6e20 6f70 6572 6174 6f72 2066 6f72  ion operator for
-0000edd0: 2074 6865 206d 6f6c 6563 756c 6520 6465   the molecule de
-0000ede0: 6669 6e65 6420 6279 2061 746f 6d73 2c20  fined by atoms, 
-0000edf0: 7879 7a2c 206d 6173 7365 7327 2727 0a20  xyz, masses'''. 
-0000ee00: 2020 6d61 7373 2c63 6d20 3d20 6361 6c63    mass,cm = calc
-0000ee10: 756c 6174 655f 6365 6e74 7265 5f6f 665f  ulate_centre_of_
-0000ee20: 6d61 7373 2878 797a 732c 6d61 7373 6573  mass(xyzs,masses
-0000ee30: 290a 2020 2023 2054 6865 2070 726f 6a65  ).   # The proje
-0000ee40: 6374 696f 6e20 6f70 6572 6174 6f72 2068  ction operator h
-0000ee50: 6173 2064 696d 656e 7369 6f6e 206e 756d  as dimension num
-0000ee60: 6265 725f 6f66 5f63 6f6e 7374 7261 696e  ber_of_constrain
-0000ee70: 7473 2a6e 6174 6f6d 732a 330a 2020 2070  ts*natoms*3.   p
-0000ee80: 7320 3d20 6e70 2e7a 6572 6f73 2820 2836  s = np.zeros( (6
-0000ee90: 2c6e 6174 732a 3329 2029 0a20 2020 7820  ,nats*3) ).   x 
-0000eea0: 3d20 300a 2020 2079 203d 2031 0a20 2020  = 0.   y = 1.   
-0000eeb0: 7a20 3d20 320a 2020 2066 6f72 2069 2c6d  z = 2.   for i,m
-0000eec0: 6173 732c 7879 7a20 696e 207a 6970 2861  ass,xyz in zip(a
-0000eed0: 746f 6d73 2c6d 6173 7365 732c 7879 7a73  toms,masses,xyzs
-0000eee0: 293a 0a20 2020 2020 2020 7073 5b30 2c69  ):.       ps[0,i
-0000eef0: 2a33 2b78 5d20 3d20 6d61 7468 2e73 7172  *3+x] = math.sqr
-0000ef00: 7428 6d61 7373 290a 2020 2020 2020 2070  t(mass).       p
-0000ef10: 735b 312c 692a 332b 795d 203d 206d 6174  s[1,i*3+y] = mat
-0000ef20: 682e 7371 7274 286d 6173 7329 0a20 2020  h.sqrt(mass).   
-0000ef30: 2020 2020 7073 5b32 2c69 2a33 2b7a 5d20      ps[2,i*3+z] 
-0000ef40: 3d20 6d61 7468 2e73 7172 7428 6d61 7373  = math.sqrt(mass
-0000ef50: 290a 2020 2020 2020 2023 2063 6f6f 7264  ).       # coord
-0000ef60: 696e 6174 6573 2072 656c 6174 6976 6520  inates relative 
-0000ef70: 746f 2074 6865 2063 656e 7472 6520 6f66  to the centre of
-0000ef80: 206d 6173 730a 2020 2020 2020 2072 656c   mass.       rel
-0000ef90: 7879 7a20 3d20 6d61 7468 2e73 7172 7428  xyz = math.sqrt(
-0000efa0: 6d61 7373 2920 2a20 2878 797a 202d 2063  mass) * (xyz - c
-0000efb0: 6d29 0a20 2020 2020 2020 2320 4669 7273  m).       # Firs
-0000efc0: 7420 726f 7461 7469 6f6e 7320 6162 6f75  t rotations abou
-0000efd0: 7420 7820 696e 2074 6865 2079 2f7a 2070  t x in the y/z p
-0000efe0: 6c61 6e65 0a20 2020 2020 2020 2320 7a7a  lane.       # zz
-0000eff0: 2069 7320 7265 616c 6c79 2072 2a73 696e   is really r*sin
-0000f000: 2874 6865 7461 292c 2061 6e64 2073 696e  (theta), and sin
-0000f010: 2874 6865 7461 2920 3d20 7a7a 2f72 0a20  (theta) = zz/r. 
-0000f020: 2020 2020 2020 2320 7979 2069 7320 7265        # yy is re
-0000f030: 616c 6c79 2072 2a63 6f73 2874 6865 7461  ally r*cos(theta
-0000f040: 292c 2061 6e64 2063 6f73 2874 6865 7461  ), and cos(theta
-0000f050: 2920 3d20 7979 2f72 0a20 2020 2020 2020  ) = yy/r.       
-0000f060: 7073 5b33 2c69 2a33 2b78 5d20 3d20 302e  ps[3,i*3+x] = 0.
-0000f070: 300a 2020 2020 2020 2070 735b 332c 692a  0.       ps[3,i*
-0000f080: 332b 795d 203d 202d 7265 6c78 797a 5b7a  3+y] = -relxyz[z
-0000f090: 5d0a 2020 2020 2020 2070 735b 332c 692a  ].       ps[3,i*
-0000f0a0: 332b 7a5d 203d 202b 7265 6c78 797a 5b79  3+z] = +relxyz[y
-0000f0b0: 5d0a 2020 2020 2020 2023 204e 6578 7420  ].       # Next 
-0000f0c0: 726f 7461 7469 6f6e 7320 6162 6f75 7420  rotations about 
-0000f0d0: 7920 696e 2074 6865 2078 2f7a 2070 6c61  y in the x/z pla
-0000f0e0: 6e65 0a20 2020 2020 2020 7073 5b34 2c69  ne.       ps[4,i
-0000f0f0: 2a33 2b78 5d20 3d20 2b72 656c 7879 7a5b  *3+x] = +relxyz[
-0000f100: 7a5d 0a20 2020 2020 2020 7073 5b34 2c69  z].       ps[4,i
-0000f110: 2a33 2b79 5d20 3d20 302e 300a 2020 2020  *3+y] = 0.0.    
-0000f120: 2020 2070 735b 342c 692a 332b 7a5d 203d     ps[4,i*3+z] =
-0000f130: 202d 7265 6c78 797a 5b78 5d0a 2020 2020   -relxyz[x].    
-0000f140: 2020 2023 204e 6578 7420 726f 7461 7469     # Next rotati
-0000f150: 6f6e 7320 6162 6f75 7420 7a20 696e 2074  ons about z in t
-0000f160: 6865 2078 2f79 2070 6c61 6e65 0a20 2020  he x/y plane.   
-0000f170: 2020 2020 7073 5b35 2c69 2a33 2b78 5d20      ps[5,i*3+x] 
-0000f180: 3d20 2d72 656c 7879 7a5b 795d 0a20 2020  = -relxyz[y].   
-0000f190: 2020 2020 7073 5b35 2c69 2a33 2b79 5d20      ps[5,i*3+y] 
-0000f1a0: 3d20 2b72 656c 7879 7a5b 785d 0a20 2020  = +relxyz[x].   
-0000f1b0: 2020 2020 7073 5b35 2c69 2a33 2b7a 5d20      ps[5,i*3+z] 
-0000f1c0: 3d20 302e 300a 2020 2072 6574 7572 6e20  = 0.0.   return 
-0000f1d0: 7073 0a0a 6465 6620 6361 6c63 756c 6174  ps..def calculat
-0000f1e0: 655f 656e 6572 6779 5f64 6973 7472 6962  e_energy_distrib
-0000f1f0: 7574 696f 6e28 6365 6c6c 2c20 6672 6571  ution(cell, freq
-0000f200: 7565 6e63 6965 732c 206e 6f72 6d61 6c5f  uencies, normal_
-0000f210: 6d6f 6465 732c 2064 6562 7567 3d46 616c  modes, debug=Fal
-0000f220: 7365 293a 0a20 2020 2727 2743 616c 6375  se):.   '''Calcu
-0000f230: 6c61 7465 2065 6e65 7267 7920 6469 7374  late energy dist
-0000f240: 7269 6275 7469 6f6e 2069 6e20 7468 6520  ribution in the 
-0000f250: 7068 6f6e 6f6e 206d 6f64 6573 0a20 2020  phonon modes.   
-0000f260: 2020 2066 7265 7175 656e 6369 6573 2061     frequencies a
-0000f270: 7265 2074 6865 2066 7265 7175 656e 6369  re the frequenci
-0000f280: 6573 2069 6e20 636d 2d31 0a20 2020 2020  es in cm-1.     
-0000f290: 206e 6f72 6d61 6c5f 6d6f 6465 7320 6172   normal_modes ar
-0000f2a0: 6520 7468 6520 6d61 7373 2077 6569 6768  e the mass weigh
-0000f2b0: 7465 6420 6e6f 726d 616c 206d 6f64 6573  ted normal modes
-0000f2c0: 2727 270a 2020 206d 6f6c 6563 756c 6573  '''.   molecules
-0000f2d0: 203d 2063 656c 6c2e 6d6f 6c65 6375 6c65   = cell.molecule
-0000f2e0: 730a 2020 2061 746f 6d69 635f 6d61 7373  s.   atomic_mass
-0000f2f0: 6573 203d 2063 656c 6c2e 6174 6f6d 6963  es = cell.atomic
-0000f300: 5f6d 6173 7365 730a 2020 2078 797a 203d  _masses.   xyz =
-0000f310: 2063 656c 6c2e 7879 7a5f 636f 6f72 6469   cell.xyz_coordi
-0000f320: 6e61 7465 730a 2020 206e 6174 7320 3d20  nates.   nats = 
-0000f330: 6c65 6e28 7879 7a29 0a20 2020 2320 4361  len(xyz).   # Ca
-0000f340: 6c63 756c 6174 6520 7468 6520 7072 6f6a  lculate the proj
-0000f350: 6563 7469 6f6e 7320 6f70 6572 6174 6f72  ections operator
-0000f360: 7320 666f 7220 6561 6368 206d 6f6c 6563  s for each molec
-0000f370: 756c 650a 2020 206d 6f6c 6563 756c 6172  ule.   molecular
-0000f380: 5f70 726f 6a65 6374 696f 6e5f 6f70 6572  _projection_oper
-0000f390: 6174 6f72 7320 3d20 5b5d 0a20 2020 6d6f  ators = [].   mo
-0000f3a0: 6c65 6375 6c65 5f6d 6173 6b73 203d 205b  lecule_masks = [
-0000f3b0: 5d0a 2020 2066 6f72 2061 746f 6d73 2069  ].   for atoms i
-0000f3c0: 6e20 6d6f 6c65 6375 6c65 733a 0a20 2020  n molecules:.   
-0000f3d0: 2020 2020 6d6f 6c5f 7879 7a73 2020 3d20      mol_xyzs  = 
-0000f3e0: 5b20 7879 7a5b 6174 6f6d 5d20 666f 7220  [ xyz[atom] for 
-0000f3f0: 6174 6f6d 2069 6e20 6174 6f6d 735d 0a20  atom in atoms]. 
-0000f400: 2020 2020 2020 6d6f 6c5f 6d61 736b 203d        mol_mask =
-0000f410: 206e 702e 7a65 726f 7328 6e61 7473 2a33   np.zeros(nats*3
-0000f420: 290a 2020 2020 2020 2066 6f72 2061 746f  ).       for ato
-0000f430: 6d20 696e 2061 746f 6d73 3a0a 2020 2020  m in atoms:.    
-0000f440: 2020 2020 2020 206d 6f6c 5f6d 6173 6b5b         mol_mask[
-0000f450: 332a 6174 6f6d 2b30 5d20 3d20 310a 2020  3*atom+0] = 1.  
-0000f460: 2020 2020 2020 2020 206d 6f6c 5f6d 6173           mol_mas
-0000f470: 6b5b 332a 6174 6f6d 2b31 5d20 3d20 310a  k[3*atom+1] = 1.
-0000f480: 2020 2020 2020 2020 2020 206d 6f6c 5f6d             mol_m
-0000f490: 6173 6b5b 332a 6174 6f6d 2b32 5d20 3d20  ask[3*atom+2] = 
-0000f4a0: 310a 2020 2020 2020 206d 6f6c 5f6d 6173  1.       mol_mas
-0000f4b0: 7365 7320 3d20 5b20 6174 6f6d 6963 5f6d  ses = [ atomic_m
-0000f4c0: 6173 7365 735b 6174 6f6d 5d20 666f 7220  asses[atom] for 
-0000f4d0: 6174 6f6d 2069 6e20 6174 6f6d 735d 0a20  atom in atoms]. 
-0000f4e0: 2020 2020 2020 7072 6f6a 6563 7469 6f6e        projection
-0000f4f0: 5f6f 7065 7261 746f 7273 203d 2063 6f6e  _operators = con
-0000f500: 7374 7275 6374 5f70 726f 6a65 6374 696f  struct_projectio
-0000f510: 6e5f 6f70 6572 6174 6f72 2861 746f 6d73  n_operator(atoms
-0000f520: 2c6d 6f6c 5f78 797a 732c 6d6f 6c5f 6d61  ,mol_xyzs,mol_ma
-0000f530: 7373 6573 2c6e 6174 7329 0a20 2020 2020  sses,nats).     
-0000f540: 2020 7072 6f6a 6563 7469 6f6e 5f6f 7065    projection_ope
-0000f550: 7261 746f 7273 203d 206f 7274 686f 676f  rators = orthogo
-0000f560: 6e61 6c69 7365 5f70 726f 6a65 6374 696f  nalise_projectio
-0000f570: 6e5f 6f70 6572 6174 6f72 2870 726f 6a65  n_operator(proje
-0000f580: 6374 696f 6e5f 6f70 6572 6174 6f72 7329  ction_operators)
-0000f590: 0a20 2020 2020 2020 6d6f 6c65 6375 6c61  .       molecula
-0000f5a0: 725f 7072 6f6a 6563 7469 6f6e 5f6f 7065  r_projection_ope
-0000f5b0: 7261 746f 7273 2e61 7070 656e 6428 7072  rators.append(pr
-0000f5c0: 6f6a 6563 7469 6f6e 5f6f 7065 7261 746f  ojection_operato
-0000f5d0: 7273 290a 2020 2020 2020 2023 0a20 2020  rs).       #.   
-0000f5e0: 2020 2020 6d6f 6c65 6375 6c65 5f6d 6173      molecule_mas
-0000f5f0: 6b73 2e61 7070 656e 6428 6d6f 6c5f 6d61  ks.append(mol_ma
-0000f600: 736b 290a 2020 2023 2043 616c 6375 6c61  sk).   # Calcula
-0000f610: 7465 2074 6865 2063 6f6e 7472 6962 7574  te the contribut
-0000f620: 696f 6e73 2074 6f20 7468 6520 6b69 6e65  ions to the kine
-0000f630: 7469 6320 656e 6572 6779 2069 6e20 6561  tic energy in ea
-0000f640: 6368 206d 6f64 650a 2020 2065 6e65 7267  ch mode.   energ
-0000f650: 6965 735f 696e 5f6d 6f64 6573 203d 205b  ies_in_modes = [
-0000f660: 5d0a 2020 2066 6f72 2069 6d6f 6465 2c6d  ].   for imode,m
-0000f670: 6f64 6520 696e 2065 6e75 6d65 7261 7465  ode in enumerate
-0000f680: 286e 6f72 6d61 6c5f 6d6f 6465 7329 3a0a  (normal_modes):.
-0000f690: 2020 2020 2020 206d 6f64 655f 636d 203d         mode_cm =
-0000f6a0: 206d 6f64 650a 2020 2020 2020 2063 656e   mode.       cen
-0000f6b0: 7472 655f 6f66 5f6d 6173 735f 656e 6572  tre_of_mass_ener
-0000f6c0: 6779 203d 2030 2e30 0a20 2020 2020 2020  gy = 0.0.       
-0000f6d0: 726f 7461 7469 6f6e 616c 5f65 6e65 7267  rotational_energ
-0000f6e0: 7920 3d20 302e 300a 2020 2020 2020 206d  y = 0.0.       m
-0000f6f0: 6f6c 6563 756c 6172 5f65 6e65 7267 6965  olecular_energie
-0000f700: 7320 3d20 5b5d 0a20 2020 2020 2020 666f  s = [].       fo
-0000f710: 7220 696d 6f6c 2c28 7073 2c6d 6173 6b29  r imol,(ps,mask)
-0000f720: 2069 6e20 656e 756d 6572 6174 6528 7a69   in enumerate(zi
-0000f730: 7028 6d6f 6c65 6375 6c61 725f 7072 6f6a  p(molecular_proj
-0000f740: 6563 7469 6f6e 5f6f 7065 7261 746f 7273  ection_operators
-0000f750: 2c6d 6f6c 6563 756c 655f 6d61 736b 7329  ,molecule_masks)
-0000f760: 293a 0a20 2020 2020 2020 2020 2020 2320  ):.           # 
-0000f770: 4361 6c63 756c 6174 6520 746f 7461 6c20  Calculate total 
-0000f780: 6b69 6e65 7469 6320 656e 6572 6779 0a20  kinetic energy. 
-0000f790: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
-0000f7a0: 656e 6572 6779 203d 206e 702e 646f 7428  energy = np.dot(
-0000f7b0: 6d6f 6465 2c6d 6f64 6529 0a20 2020 2020  mode,mode).     
-0000f7c0: 2020 2020 2020 2320 5072 6f6a 6563 7420        # Project 
-0000f7d0: 6f75 7420 6365 6e74 7265 206f 6620 6d61  out centre of ma
-0000f7e0: 7373 206d 6f74 696f 6e20 6f66 2065 6163  ss motion of eac
-0000f7f0: 6820 6d6f 6c65 6375 6c65 0a20 2020 2020  h molecule.     
-0000f800: 2020 2020 2020 6d6f 6465 5f63 6d20 3d20        mode_cm = 
-0000f810: 6d6f 6465 202d 206e 702e 646f 7428 6d6f  mode - np.dot(mo
-0000f820: 6465 2c70 735b 305d 292a 7073 5b30 5d20  de,ps[0])*ps[0] 
-0000f830: 2d20 6e70 2e64 6f74 286d 6f64 652c 7073  - np.dot(mode,ps
-0000f840: 5b31 5d29 2a70 735b 315d 202d 206e 702e  [1])*ps[1] - np.
-0000f850: 646f 7428 6d6f 6465 2c70 735b 325d 292a  dot(mode,ps[2])*
-0000f860: 7073 5b32 5d0a 2020 2020 2020 2020 2020  ps[2].          
-0000f870: 2063 656e 7472 655f 6f66 5f6d 6173 735f   centre_of_mass_
-0000f880: 656e 6572 6779 202b 3d20 746f 7461 6c5f  energy += total_
-0000f890: 656e 6572 6779 202d 206e 702e 646f 7428  energy - np.dot(
-0000f8a0: 6d6f 6465 5f63 6d2c 6d6f 6465 5f63 6d29  mode_cm,mode_cm)
-0000f8b0: 0a20 2020 2020 2020 2020 2020 2320 5072  .           # Pr
-0000f8c0: 6f6a 6563 7420 6f75 7420 6d6f 6c65 6375  oject out molecu
-0000f8d0: 6c61 7220 726f 7461 7469 6f6e 206f 6620  lar rotation of 
-0000f8e0: 6561 6368 206d 6f6c 6563 756c 650a 2020  each molecule.  
-0000f8f0: 2020 2020 2020 2020 206d 6f64 655f 636d           mode_cm
-0000f900: 203d 206d 6f64 6520 2d20 6e70 2e64 6f74   = mode - np.dot
-0000f910: 286d 6f64 652c 7073 5b33 5d29 2a70 735b  (mode,ps[3])*ps[
-0000f920: 335d 202d 206e 702e 646f 7428 6d6f 6465  3] - np.dot(mode
-0000f930: 2c70 735b 345d 292a 7073 5b34 5d20 2d20  ,ps[4])*ps[4] - 
-0000f940: 6e70 2e64 6f74 286d 6f64 652c 7073 5b35  np.dot(mode,ps[5
-0000f950: 5d29 2a70 735b 355d 0a20 2020 2020 2020  ])*ps[5].       
-0000f960: 2020 2020 726f 7461 7469 6f6e 616c 5f65      rotational_e
-0000f970: 6e65 7267 7920 2b3d 2074 6f74 616c 5f65  nergy += total_e
-0000f980: 6e65 7267 7920 2d20 6e70 2e64 6f74 286d  nergy - np.dot(m
-0000f990: 6f64 655f 636d 2c6d 6f64 655f 636d 290a  ode_cm,mode_cm).
-0000f9a0: 2020 2020 2020 2020 2020 2023 204e 6f77             # Now
-0000f9b0: 2077 6f72 6b20 6f75 7420 7468 6520 656e   work out the en
-0000f9c0: 6572 6779 206f 6620 7468 6520 6d6f 6c65  ergy of the mole
-0000f9d0: 6375 6c65 0a20 2020 2020 2020 2020 2020  cule.           
-0000f9e0: 6d6f 6465 5f63 6d20 3d20 6d61 736b 202a  mode_cm = mask *
-0000f9f0: 206d 6f64 650a 2020 2020 2020 2020 2020   mode.          
-0000fa00: 206d 6f6c 5f65 6e65 7267 7920 3d20 6e70   mol_energy = np
-0000fa10: 2e64 6f74 286d 6f64 655f 636d 2c6d 6f64  .dot(mode_cm,mod
-0000fa20: 655f 636d 290a 2020 2020 2020 2020 2020  e_cm).          
-0000fa30: 206d 6f6c 6563 756c 6172 5f65 6e65 7267   molecular_energ
-0000fa40: 6965 732e 6170 7065 6e64 286d 6f6c 5f65  ies.append(mol_e
-0000fa50: 6e65 7267 7929 0a20 2020 2020 2020 2320  nergy).       # 
-0000fa60: 656e 6420 666f 7220 696d 6f6c 2c70 730a  end for imol,ps.
-0000fa70: 2020 2020 2020 2076 6962 7261 7469 6f6e         vibration
-0000fa80: 616c 5f65 6e65 7267 7920 3d20 746f 7461  al_energy = tota
-0000fa90: 6c5f 656e 6572 6779 202d 2063 656e 7472  l_energy - centr
-0000faa0: 655f 6f66 5f6d 6173 735f 656e 6572 6779  e_of_mass_energy
-0000fab0: 202d 2072 6f74 6174 696f 6e61 6c5f 656e   - rotational_en
-0000fac0: 6572 6779 0a20 2020 2020 2020 656e 6572  ergy.       ener
-0000fad0: 6769 6573 5f69 6e5f 6d6f 6465 732e 6170  gies_in_modes.ap
-0000fae0: 7065 6e64 2820 2874 6f74 616c 5f65 6e65  pend( (total_ene
-0000faf0: 7267 792c 6365 6e74 7265 5f6f 665f 6d61  rgy,centre_of_ma
-0000fb00: 7373 5f65 6e65 7267 792c 726f 7461 7469  ss_energy,rotati
-0000fb10: 6f6e 616c 5f65 6e65 7267 792c 7669 6272  onal_energy,vibr
-0000fb20: 6174 696f 6e61 6c5f 656e 6572 6779 2c6d  ational_energy,m
-0000fb30: 6f6c 6563 756c 6172 5f65 6e65 7267 6965  olecular_energie
-0000fb40: 7329 2029 0a20 2020 2320 656e 6420 666f  s) ).   # end fo
-0000fb50: 7220 6d6f 6465 2069 6e20 6e6f 726d 616c  r mode in normal
-0000fb60: 206d 6f64 6573 0a20 2020 7265 7475 726e   modes.   return
-0000fb70: 2065 6e65 7267 6965 735f 696e 5f6d 6f64   energies_in_mod
-0000fb80: 6573 0a23 2065 6e64 2064 6566 0a0a 0a64  es.# end def...d
-0000fb90: 6566 2068 6f64 7269 636b 5f70 7265 7363  ef hodrick_presc
-0000fba0: 6f74 745f 6669 6c74 6572 2879 2c64 616d  ott_filter(y,dam
-0000fbb0: 7069 6e67 2c6c 616d 6264 615f 7661 6c75  ping,lambda_valu
-0000fbc0: 652c 6e69 7465 7273 293a 0a20 2020 2023  e,niters):.    #
-0000fbd0: 0a20 2020 2023 2041 7070 6c79 2061 2048  .    # Apply a H
-0000fbe0: 6f64 7269 636b 2050 7265 7363 6f74 7420  odrick Prescott 
-0000fbf0: 6669 6c74 6572 2074 6f20 7468 6520 7370  filter to the sp
-0000fc00: 6563 7472 756d 2069 6e20 782c 2079 0a20  ectrum in x, y. 
-0000fc10: 2020 2023 2079 2069 7320 7468 6520 6578     # y is the ex
-0000fc20: 7065 7269 6d65 6e74 616c 2061 6273 6f72  perimental absor
-0000fc30: 7074 696f 6e0a 2020 2020 2320 6461 6d70  ption.    # damp
-0000fc40: 696e 6720 6973 2075 7365 6420 746f 2064  ing is used to d
-0000fc50: 616d 7020 7468 6520 6974 6572 6174 696f  amp the iteratio
-0000fc60: 6e73 0a20 2020 2023 206c 616d 6264 615f  ns.    # lambda_
-0000fc70: 7661 6c75 6520 6973 2074 6865 2063 686f  value is the cho
-0000fc80: 7365 6e20 736d 6f6f 7468 696e 6720 6661  sen smoothing fa
-0000fc90: 6374 6f72 0a20 2020 2023 2042 6173 6564  ctor.    # Based
-0000fca0: 206f 6e20 6964 6561 7320 696e 2074 6865   on ideas in the
-0000fcb0: 2074 6865 7369 7320 6f66 204d 6179 616e   thesis of Mayan
-0000fcc0: 6b20 4b61 7573 6869 6b20 2855 6e69 7665  k Kaushik (Unive
-0000fcd0: 7273 6974 7920 4164 656c 6169 6465 290a  rsity Adelaide).
-0000fce0: 2020 2020 230a 2020 2020 6672 6f6d 2073      #.    from s
-0000fcf0: 6369 7079 2069 6d70 6f72 7420 7370 6172  cipy import spar
-0000fd00: 7365 0a20 2020 2023 0a20 2020 2023 2043  se.    #.    # C
-0000fd10: 7265 6174 6520 6120 7370 6172 7365 2033  reate a sparse 3
-0000fd20: 7264 206f 7264 6572 2064 6966 6665 7265  rd order differe
-0000fd30: 6e63 6520 6f70 6572 6174 6f72 0a20 2020  nce operator.   
-0000fd40: 2023 0a20 2020 206e 203d 206c 656e 2879   #.    n = len(y
-0000fd50: 290a 2020 2020 6469 6167 203d 206e 702e  ).    diag = np.
-0000fd60: 6f6e 6573 286e 2d33 290a 2020 2020 4420  ones(n-3).    D 
-0000fd70: 3d20 7370 6172 7365 2e73 7064 6961 6773  = sparse.spdiags
-0000fd80: 2820 5b2d 312a 6469 6167 2c20 332a 6469  ( [-1*diag, 3*di
-0000fd90: 6167 2c20 2d33 2a64 6961 672c 2031 2a64  ag, -3*diag, 1*d
-0000fda0: 6961 675d 2c0a 2020 2020 2020 2020 2020  iag],.          
-0000fdb0: 2020 2020 2020 2020 2020 2020 2020 5b30                [0
-0000fdc0: 2c20 2d31 2c20 2d32 2c20 2d33 5d2c 206e  , -1, -2, -3], n
-0000fdd0: 2c20 6e2d 3320 292e 746f 6373 6328 290a  , n-3 ).tocsc().
-0000fde0: 2020 2020 7720 3d20 6e70 2e6f 6e65 7328      w = np.ones(
-0000fdf0: 6e29 0a20 2020 2066 6f72 2069 7420 696e  n).    for it in
-0000fe00: 2072 616e 6765 2831 302a 6e69 7465 7273   range(10*niters
-0000fe10: 293a 0a20 2020 2020 2020 2057 203d 2073  ):.        W = s
-0000fe20: 7061 7273 652e 7370 6469 6167 7328 772c  parse.spdiags(w,
-0000fe30: 2030 2c20 6e2c 206e 292e 746f 6373 6328   0, n, n).tocsc(
-0000fe40: 290a 2020 2020 2020 2020 2320 5072 6f62  ).        # Prob
-0000fe50: 6c65 6d73 2077 6974 6820 6f76 6572 666c  lems with overfl
-0000fe60: 6f77 2069 6620 6c61 6d62 6461 2069 7320  ow if lambda is 
-0000fe70: 6c61 7267 650a 2020 2020 2020 2020 7472  large.        tr
-0000fe80: 793a 0a20 2020 2020 2020 2020 2020 205a  y:.            Z
-0000fe90: 203d 2057 202b 2070 6f77 2831 302c 6c61   = W + pow(10,la
-0000fea0: 6d62 6461 5f76 616c 7565 2920 2a20 2844  mbda_value) * (D
-0000feb0: 2e64 6f74 2844 2e74 7261 6e73 706f 7365  .dot(D.transpose
-0000fec0: 2829 2929 0a20 2020 2020 2020 2065 7863  ())).        exc
-0000fed0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-0000fee0: 2070 6173 730a 2020 2020 2020 2020 7a20   pass.        z 
-0000fef0: 3d20 7370 6172 7365 2e6c 696e 616c 672e  = sparse.linalg.
-0000ff00: 7370 736f 6c76 6528 5a2c 2077 2a79 290a  spsolve(Z, w*y).
-0000ff10: 2020 2020 2020 2020 2320 7265 7369 6475          # residu
-0000ff20: 616c 7320 3d20 7920 2d20 7a0a 2020 2020  als = y - z.    
-0000ff30: 2020 2020 2320 6572 726f 7220 3d20 7375      # error = su
-0000ff40: 6d28 2072 2a72 2066 6f72 2072 2069 6e20  m( r*r for r in 
-0000ff50: 7265 7369 6475 616c 7320 6966 2072 203c  residuals if r <
-0000ff60: 2030 2e30 2029 0a20 2020 2020 2020 2023   0.0 ).        #
-0000ff70: 2065 7272 6f72 203d 206d 6174 682e 7371   error = math.sq
-0000ff80: 7274 2865 7272 6f72 2f6e 290a 2020 2020  rt(error/n).    
-0000ff90: 2020 2020 7720 3d20 6461 6d70 696e 672a      w = damping*
-0000ffa0: 2879 3e7a 2920 2b20 2831 2d64 616d 7069  (y>z) + (1-dampi
-0000ffb0: 6e67 292a 2879 3c7a 290a 2020 2020 2020  ng)*(y<z).      
-0000ffc0: 2020 2320 7072 696e 7428 6974 2c20 6572    # print(it, er
-0000ffd0: 726f 7229 0a20 2020 2072 6574 7572 6e20  ror).    return 
-0000ffe0: 792d 7a0a 0a64 6566 2072 6566 6c65 6374  y-z..def reflect
-0000fff0: 616e 6365 5f61 7472 286e 732c 6e30 2c74  ance_atr(ns,n0,t
-00010000: 6865 7461 2c61 7472 5350 6f6c 4672 6163  heta,atrSPolFrac
-00010010: 7469 6f6e 293a 0a20 2020 2023 0a20 2020  tion):.    #.   
-00010020: 2023 2043 616c 6375 6c61 7465 2074 6865   # Calculate the
-00010030: 2061 7472 2073 2061 6e64 2070 2072 6566   atr s and p ref
-00010040: 6c65 6374 616e 6365 0a20 2020 2023 206e  lectance.    # n
-00010050: 7320 6973 2074 6865 2063 6f6d 706c 6578  s is the complex
-00010060: 2070 6572 6d69 7474 6976 6974 7920 6f66   permittivity of
-00010070: 2074 6865 2065 6666 6563 7469 7665 206d   the effective m
-00010080: 6564 6975 6d0a 2020 2020 2320 6e30 2069  edium.    # n0 i
-00010090: 7320 7468 6520 7065 726d 6974 7469 7669  s the permittivi
-000100a0: 7479 206f 6620 6174 7220 6d61 7465 7269  ty of atr materi
-000100b0: 616c 0a20 2020 2023 2074 6865 7461 2069  al.    # theta i
-000100c0: 7320 7468 6520 616e 676c 6520 6f66 2069  s the angle of i
-000100d0: 6e63 6964 656e 6365 2069 6e20 6465 6772  ncidence in degr
-000100e0: 6565 730a 2020 2020 2320 6174 7253 506f  ees.    # atrSPo
-000100f0: 6c46 7261 6374 696f 6e20 6973 2074 6865  lFraction is the
-00010100: 2066 7261 6374 696f 6e20 6f66 2053 2077   fraction of S w
-00010110: 6176 6520 746f 2062 6520 636f 6e73 6964  ave to be consid
-00010120: 6572 6564 0a20 2020 2023 2020 2020 2020  ered.    #      
-00010130: 2020 2020 2020 2020 2020 2054 6865 2061             The a
-00010140: 6d6f 756e 7420 6f66 2050 2077 6176 6520  mount of P wave 
-00010150: 6973 2031 2d61 7472 5350 6f6c 4672 6163  is 1-atrSPolFrac
-00010160: 7469 6f6e 0a20 2020 2023 0a20 2020 2023  tion.    #.    #
-00010170: 2072 7320 6973 2074 6865 2073 2d77 6176   rs is the s-wav
-00010180: 6520 4672 6573 6e65 6c20 616d 706c 6974  e Fresnel amplit
-00010190: 7564 650a 2020 2020 2320 7270 2069 7320  ude.    # rp is 
-000101a0: 7468 6520 702d 7761 7665 0a0a 2020 2020  the p-wave..    
-000101b0: 2320 436f 6e76 6572 7420 7468 6574 6120  # Convert theta 
-000101c0: 746f 2061 6e20 616e 676c 6520 696e 2072  to an angle in r
-000101d0: 6164 6961 6e73 0a20 2020 2074 6865 7461  adians.    theta
-000101e0: 203d 206d 6174 682e 7261 6469 616e 7328   = math.radians(
-000101f0: 7468 6574 6129 0a20 2020 2063 6f73 7468  theta).    costh
-00010200: 6574 6120 3d20 6d61 7468 2e63 6f73 2874  eta = math.cos(t
-00010210: 6865 7461 290a 2020 2020 7369 6e74 6865  heta).    sinthe
-00010220: 7461 203d 206d 6174 682e 7369 6e28 7468  ta = math.sin(th
-00010230: 6574 6129 0a20 2020 2023 2043 616c 6375  eta).    # Calcu
-00010240: 6c61 7465 2074 6865 2046 7265 736e 656c  late the Fresnel
-00010250: 2061 6d70 6c69 7475 6465 7320 666f 7220   amplitudes for 
-00010260: 7265 666c 6563 7469 6f6e 0a20 2020 2023  reflection.    #
-00010270: 2045 7175 6174 696f 6e73 2074 616b 656e   Equations taken
-00010280: 2066 726f 6d20 7033 3638 206f 6620 4150   from p368 of AP
-00010290: 504c 4945 4420 5350 4543 5452 4f53 434f  PLIED SPECTROSCO
-000102a0: 5059 2052 4556 4945 5753 0a20 2020 2023  PY REVIEWS.    #
-000102b0: 2056 6f6c 2e20 3339 2c20 4e6f 2e20 332c   Vol. 39, No. 3,
-000102c0: 2070 702e 2033 3635 e280 9333 3834 2c20   pp. 365...384, 
-000102d0: 3230 3034 0a20 2020 2023 2062 7920 4d69  2004.    # by Mi
-000102e0: 6c61 6e20 4d69 6c6f 7365 7669 630a 2020  lan Milosevic.  
-000102f0: 2020 2320 444f 493a 2031 302e 3130 3831    # DOI: 10.1081
-00010300: 2f41 5352 2d32 3030 3033 3031 3935 0a20  /ASR-200030195. 
-00010310: 2020 2072 7320 3d20 2d31 2e30 2a20 286e     rs = -1.0* (n
-00010320: 302a 636f 7374 6865 7461 202d 2063 6d61  0*costheta - cma
-00010330: 7468 2e73 7172 7428 6e73 2a6e 7320 2d20  th.sqrt(ns*ns - 
-00010340: 6e30 2a6e 302a 7369 6e74 6865 7461 2a73  n0*n0*sintheta*s
-00010350: 696e 7468 6574 6129 2920 2f20 286e 302a  intheta)) / (n0*
-00010360: 636f 7374 6865 7461 202b 2063 6d61 7468  costheta + cmath
-00010370: 2e73 7172 7428 6e73 2a6e 7320 2d20 6e30  .sqrt(ns*ns - n0
-00010380: 2a6e 302a 7369 6e74 6865 7461 2a73 696e  *n0*sintheta*sin
-00010390: 7468 6574 6129 290a 2020 2020 7270 203d  theta)).    rp =
-000103a0: 2028 6e73 2a6e 732f 6e30 2a63 6f73 7468   (ns*ns/n0*costh
-000103b0: 6574 6120 2d20 636d 6174 682e 7371 7274  eta - cmath.sqrt
-000103c0: 286e 732a 6e73 202d 206e 302a 6e30 2a73  (ns*ns - n0*n0*s
-000103d0: 696e 7468 6574 612a 7369 6e74 6865 7461  intheta*sintheta
-000103e0: 2929 202f 2028 6e73 2a6e 732f 6e30 2a63  )) / (ns*ns/n0*c
-000103f0: 6f73 7468 6574 6120 2b20 636d 6174 682e  ostheta + cmath.
-00010400: 7371 7274 286e 732a 6e73 202d 206e 302a  sqrt(ns*ns - n0*
-00010410: 6e30 2a73 696e 7468 6574 612a 7369 6e74  n0*sintheta*sint
-00010420: 6865 7461 2929 0a20 2020 2023 2043 616c  heta)).    # Cal
-00010430: 6375 6c61 7465 2074 6865 2072 6566 6c65  culate the refle
-00010440: 6374 616e 6365 2066 726f 6d20 7468 6520  ctance from the 
-00010450: 616d 706c 6974 7564 6573 202d 2073 746f  amplitudes - sto
-00010460: 7265 2061 7320 6120 7265 616c 0a20 2020  re as a real.   
-00010470: 2052 5320 3d20 6e70 2e72 6561 6c28 7273   RS = np.real(rs
-00010480: 202a 2072 732e 636f 6e6a 7567 6174 6528   * rs.conjugate(
-00010490: 2929 0a20 2020 2052 5020 3d20 6e70 2e72  )).    RP = np.r
-000104a0: 6561 6c28 7270 202a 2072 702e 636f 6e6a  eal(rp * rp.conj
-000104b0: 7567 6174 6528 2929 0a20 2020 2052 5350  ugate()).    RSP
-000104c0: 203d 2061 7472 5350 6f6c 4672 6163 7469   = atrSPolFracti
-000104d0: 6f6e 2a52 5320 2b20 2831 2e30 2d61 7472  on*RS + (1.0-atr
-000104e0: 5350 6f6c 4672 6163 7469 6f6e 292a 5250  SPolFraction)*RP
-000104f0: 0a20 2020 2023 204e 6f77 2072 6574 7572  .    # Now retur
-00010500: 6e20 7468 6520 6578 7469 6e63 7469 6f6e  n the extinction
-00010510: 0a20 2020 2052 5350 203d 202d 6d61 7468  .    RSP = -math
-00010520: 2e6c 6f67 3130 2852 5350 290a 2020 2020  .log10(RSP).    
-00010530: 7265 7475 726e 2052 5350 0a0a 6465 6620  return RSP..def 
-00010540: 736f 6c76 655f 7369 6e67 6c65 5f63 7279  solve_single_cry
-00010550: 7374 616c 5f65 7175 6174 696f 6e73 2820  stal_equations( 
-00010560: 0a20 2020 2020 2020 2073 7570 6572 7374  .        superst
-00010570: 7261 7465 4469 656c 6563 7472 6963 4675  rateDielectricFu
-00010580: 6e63 7469 6f6e 202c 0a20 2020 2020 2020  nction ,.       
-00010590: 2073 7562 7374 7261 7465 4469 656c 6563   substrateDielec
-000105a0: 7472 6963 4675 6e63 7469 6f6e 2020 202c  tricFunction   ,
-000105b0: 0a20 2020 2020 2020 2063 7279 7374 616c  .        crystal
-000105c0: 5065 726d 6974 7469 7669 7479 4675 6e63  PermittivityFunc
-000105d0: 7469 6f6e 2020 202c 0a20 2020 2020 2020  tion   ,.       
-000105e0: 2073 7570 6572 7374 7261 7465 4465 7074   superstrateDept
-000105f0: 6820 2020 2020 2020 2020 2020 2020 202c  h              ,
-00010600: 0a20 2020 2020 2020 2073 7562 7374 7261  .        substra
-00010610: 7465 4465 7074 6820 2020 2020 2020 2020  teDepth         
-00010620: 2020 2020 2020 202c 0a20 2020 2020 2020         ,.       
-00010630: 2063 7279 7374 616c 4465 7074 6820 2020   crystalDepth   
-00010640: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
-00010650: 0a20 2020 2020 2020 206d 6f64 6520 2020  .        mode   
-00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 2020 2020 202c 0a20 2020 2020 2020         ,.       
-00010680: 2074 6865 7461 2020 2020 2020 2020 2020   theta          
-00010690: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
-000106a0: 0a20 2020 2020 2020 2070 6869 2020 2020  .        phi    
-000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2020 2020 202c 0a20 2020 2020 2020         ,.       
-000106d0: 2070 7369 2020 2020 2020 2020 2020 2020   psi            
-000106e0: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
-000106f0: 0a20 2020 2020 2020 2061 6e67 6c65 4f66  .        angleOf
-00010700: 496e 6369 6465 6e63 6520 2020 2020 2020  Incidence       
-00010710: 2020 2020 2020 202c 0a20 2020 2020 2020         ,.       
-00010720: 2076 2029 3a0a 2020 2020 2222 2220 5468   v ):.    """ Th
-00010730: 6973 2069 7320 6120 7061 7261 6c6c 656c  is is a parallel
-00010740: 2063 616c 6c20 746f 2074 6865 2073 696e   call to the sin
-00010750: 676c 6520 6372 7973 7461 6c20 6571 7561  gle crystal equa
-00010760: 7469 6f6e 2073 6f6c 7665 722c 0a20 2020  tion solver,.   
-00010770: 2073 7973 7465 6d20 6973 2061 2047 544d   system is a GTM
-00010780: 2073 7973 7465 6d22 2222 0a20 2020 2023   system""".    #
-00010790: 2043 7265 6174 6520 3320 6c61 7965 7273   Create 3 layers
-000107a0: 2c20 7468 6963 6b6e 6573 7320 6973 2063  , thickness is c
-000107b0: 6f6e 7665 7274 6564 2066 726f 6d20 6d69  onverted from mi
-000107c0: 6372 6f6e 7320 746f 206d 6574 7265 730a  crons to metres.
-000107d0: 2020 2020 7375 7065 7273 7472 6174 6520      superstrate 
-000107e0: 2020 2020 203d 2047 544d 2e4c 6179 6572       = GTM.Layer
-000107f0: 2874 6869 636b 6e65 7373 3d73 7570 6572  (thickness=super
-00010800: 7374 7261 7465 4465 7074 682a 3165 2d36  strateDepth*1e-6
-00010810: 2c65 7073 696c 6f6e 313d 7375 7065 7273  ,epsilon1=supers
-00010820: 7472 6174 6544 6965 6c65 6374 7269 6346  trateDielectricF
-00010830: 756e 6374 696f 6e29 0a20 2020 2073 7562  unction).    sub
-00010840: 7374 7261 7465 2020 2020 2020 2020 3d20  strate        = 
-00010850: 4754 4d2e 4c61 7965 7228 7468 6963 6b6e  GTM.Layer(thickn
-00010860: 6573 733d 7375 6273 7472 6174 6544 6570  ess=substrateDep
-00010870: 7468 2a31 652d 362c 2020 6570 7369 6c6f  th*1e-6,  epsilo
-00010880: 6e31 3d73 7562 7374 7261 7465 4469 656c  n1=substrateDiel
-00010890: 6563 7472 6963 4675 6e63 7469 6f6e 290a  ectricFunction).
-000108a0: 2020 2020 6372 7973 7461 6c20 2020 2020      crystal     
-000108b0: 2020 2020 203d 2047 544d 2e4c 6179 6572       = GTM.Layer
-000108c0: 2874 6869 636b 6e65 7373 3d63 7279 7374  (thickness=cryst
-000108d0: 616c 4465 7074 682a 3165 2d39 2c20 2020  alDepth*1e-9,   
-000108e0: 2065 7073 696c 6f6e 3d63 7279 7374 616c   epsilon=crystal
-000108f0: 5065 726d 6974 7469 7669 7479 4675 6e63  PermittivityFunc
-00010900: 7469 6f6e 290a 2020 2020 2320 4372 6561  tion).    # Crea
-00010910: 7420 7468 6520 7379 7374 656d 2077 6974  t the system wit
-00010920: 6820 7468 6520 6c61 7965 7273 200a 2020  h the layers .  
-00010930: 2020 6966 206d 6f64 6520 3d3d 2027 5468    if mode == 'Th
-00010940: 6963 6b20 736c 6162 273a 0a20 2020 2020  ick slab':.     
-00010950: 2020 2073 7973 7465 6d20 3d20 4754 4d2e     system = GTM.
-00010960: 5379 7374 656d 2873 7562 7374 7261 7465  System(substrate
-00010970: 3d63 7279 7374 616c 2c20 7375 7065 7273  =crystal, supers
-00010980: 7472 6174 653d 7375 7065 7273 7472 6174  trate=superstrat
-00010990: 652c 206c 6179 6572 733d 5b5d 290a 2020  e, layers=[]).  
-000109a0: 2020 656c 6966 206d 6f64 6520 3d3d 2027    elif mode == '
-000109b0: 436f 6865 7265 6e74 2074 6869 6e20 6669  Coherent thin fi
-000109c0: 6c6d 273a 0a20 2020 2020 2020 2073 7973  lm':.        sys
-000109d0: 7465 6d20 3d20 4754 4d2e 5379 7374 656d  tem = GTM.System
-000109e0: 2873 7562 7374 7261 7465 3d73 7562 7374  (substrate=subst
-000109f0: 7261 7465 2c20 7375 7065 7273 7472 6174  rate, superstrat
-00010a00: 653d 7375 7065 7273 7472 6174 652c 206c  e=superstrate, l
-00010a10: 6179 6572 733d 5b63 7279 7374 616c 5d29  ayers=[crystal])
-00010a20: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00010a30: 2020 2073 7973 7465 6d20 3d20 4754 4d2e     system = GTM.
-00010a40: 5379 7374 656d 2873 7562 7374 7261 7465  System(substrate
-00010a50: 3d73 7562 7374 7261 7465 2c20 7375 7065  =substrate, supe
-00010a60: 7273 7472 6174 653d 7375 7065 7273 7472  rstrate=superstr
-00010a70: 6174 652c 206c 6179 6572 733d 5b63 7279  ate, layers=[cry
-00010a80: 7374 616c 5d29 0a20 2020 2023 2052 6f74  stal]).    # Rot
-00010a90: 6174 6520 7468 6520 6469 656c 6563 7472  ate the dielectr
-00010aa0: 6963 2063 6f6e 7374 616e 7473 2074 6f20  ic constants to 
-00010ab0: 7468 6520 6c61 626f 7261 746f 7279 2066  the laboratory f
-00010ac0: 7261 6d65 0a20 2020 2073 7973 7465 6d2e  rame.    system.
-00010ad0: 7375 6273 7472 6174 652e 7365 745f 6575  substrate.set_eu
-00010ae0: 6c65 7228 7468 6574 612c 2070 6869 2c20  ler(theta, phi, 
-00010af0: 7073 6929 0a20 2020 2073 7973 7465 6d2e  psi).    system.
-00010b00: 7375 7065 7273 7472 6174 652e 7365 745f  superstrate.set_
-00010b10: 6575 6c65 7228 7468 6574 612c 2070 6869  euler(theta, phi
-00010b20: 2c20 7073 6929 0a20 2020 2066 6f72 206c  , psi).    for l
-00010b30: 6179 6572 2069 6e20 7379 7374 656d 2e6c  ayer in system.l
-00010b40: 6179 6572 733a 0a20 2020 2020 2020 206c  ayers:.        l
-00010b50: 6179 6572 2e73 6574 5f65 756c 6572 2874  ayer.set_euler(t
-00010b60: 6865 7461 2c20 7068 692c 2070 7369 290a  heta, phi, psi).
-00010b70: 2020 2020 2320 0a20 2020 2023 2063 6f6e      # .    # con
-00010b80: 7665 7274 2063 6d2d 3120 746f 2066 7265  vert cm-1 to fre
-00010b90: 7175 656e 6379 0a20 2020 2023 0a20 2020  quency.    #.   
-00010ba0: 2066 7265 7120 3d20 7620 2a20 7370 6565   freq = v * spee
-00010bb0: 645f 6c69 6768 745f 7369 202a 2031 6532  d_light_si * 1e2
-00010bc0: 0a20 2020 2073 7973 7465 6d2e 696e 6974  .    system.init
-00010bd0: 6961 6c69 7a65 5f73 7973 2866 7265 7129  ialize_sys(freq)
-00010be0: 0a20 2020 207a 6574 615f 7379 7320 3d20  .    zeta_sys = 
-00010bf0: 6e70 2e73 696e 2861 6e67 6c65 4f66 496e  np.sin(angleOfIn
-00010c00: 6369 6465 6e63 6529 2a6e 702e 7371 7274  cidence)*np.sqrt
-00010c10: 2873 7973 7465 6d2e 7375 7065 7273 7472  (system.superstr
-00010c20: 6174 652e 6570 7369 6c6f 6e5b 302c 305d  ate.epsilon[0,0]
-00010c30: 290a 2020 2020 5379 735f 4761 6d6d 6120  ).    Sys_Gamma 
-00010c40: 3d20 7379 7374 656d 2e63 616c 6375 6c61  = system.calcula
-00010c50: 7465 5f47 616d 6d61 5374 6172 2866 7265  te_GammaStar(fre
-00010c60: 712c 207a 6574 615f 7379 7329 0a20 2020  q, zeta_sys).   
-00010c70: 2072 2c20 522c 2074 2c20 5420 3d20 7379   r, R, t, T = sy
-00010c80: 7374 656d 2e63 616c 6375 6c61 7465 5f72  stem.calculate_r
-00010c90: 5f74 287a 6574 615f 7379 7329 0a20 2020  _t(zeta_sys).   
-00010ca0: 2069 6620 6c65 6e28 7379 7374 656d 2e6c   if len(system.l
-00010cb0: 6179 6572 7329 203e 2030 3a0a 2020 2020  ayers) > 0:.    
-00010cc0: 2020 2020 6570 7369 6c6f 6e20 3d20 7379      epsilon = sy
-00010cd0: 7374 656d 2e6c 6179 6572 735b 305d 2e65  stem.layers[0].e
-00010ce0: 7073 696c 6f6e 0a20 2020 2065 6c73 653a  psilon.    else:
-00010cf0: 0a20 2020 2020 2020 2065 7073 696c 6f6e  .        epsilon
-00010d00: 203d 2073 7973 7465 6d2e 7375 6273 7472   = system.substr
-00010d10: 6174 652e 6570 7369 6c6f 6e0a 2020 2020  ate.epsilon.    
-00010d20: 7265 7475 726e 2076 2c72 2c52 2c74 2c54  return v,r,R,t,T
-00010d30: 2c65 7073 696c 6f6e 0a0a 0a64 6566 2063  ,epsilon...def c
-00010d40: 6c65 616e 7570 5f73 796d 626f 6c28 7329  leanup_symbol(s)
-00010d50: 3a0a 2020 2020 2222 2252 6574 7572 6e20  :.    """Return 
-00010d60: 6120 7472 7565 2065 6c65 6d65 6e74 2066  a true element f
-00010d70: 726f 6d20 7468 6520 7379 6d62 6f6c 2222  rom the symbol""
-00010d80: 220a 2020 2020 7320 3d20 732e 6361 7069  ".    s = s.capi
-00010d90: 7461 6c69 7a65 2829 0a20 2020 2073 203d  talize().    s =
-00010da0: 2073 2e72 6570 6c61 6365 2827 5f27 2c27   s.replace('_','
-00010db0: 2729 0a20 2020 2066 6f72 2069 2069 6e20  ').    for i in 
-00010dc0: 7374 7269 6e67 2e64 6967 6974 733a 0a20  string.digits:. 
-00010dd0: 2020 2020 2020 2073 203d 2073 2e72 6570         s = s.rep
-00010de0: 6c61 6365 2869 2c27 2729 0a20 2020 2072  lace(i,'').    r
-00010df0: 6574 7572 6e20 730a 0a64 6566 2065 756c  eturn s..def eul
-00010e00: 6572 5f72 6f74 6174 696f 6e28 7665 6374  er_rotation(vect
-00010e10: 6f72 2c20 7468 6574 612c 2070 6869 2c20  or, theta, phi, 
-00010e20: 7073 6929 3a0a 2020 2020 2022 2222 4170  psi):.     """Ap
-00010e30: 706c 7920 6120 7061 7373 6976 6520 4575  ply a passive Eu
-00010e40: 6c65 7220 726f 7461 7469 6f6e 2074 6f20  ler rotation to 
-00010e50: 7468 6520 7665 6374 6f72 2222 220a 2020  the vector""".  
-00010e60: 2020 2065 756c 6572 203d 206e 702e 7a65     euler = np.ze
-00010e70: 726f 7328 2028 332c 3329 2029 0a20 2020  ros( (3,3) ).   
-00010e80: 2020 6575 6c65 725b 302c 2030 5d20 3d20    euler[0, 0] = 
-00010e90: 206e 702e 636f 7328 7073 6929 202a 206e   np.cos(psi) * n
-00010ea0: 702e 636f 7328 7068 6929 202d 206e 702e  p.cos(phi) - np.
-00010eb0: 636f 7328 7468 6574 6129 202a 206e 702e  cos(theta) * np.
-00010ec0: 7369 6e28 7068 6929 202a 206e 702e 7369  sin(phi) * np.si
-00010ed0: 6e28 7073 6929 0a20 2020 2020 6575 6c65  n(psi).     eule
-00010ee0: 725b 302c 2031 5d20 3d20 2d6e 702e 7369  r[0, 1] = -np.si
-00010ef0: 6e28 7073 6929 202a 206e 702e 636f 7328  n(psi) * np.cos(
-00010f00: 7068 6929 202d 206e 702e 636f 7328 7468  phi) - np.cos(th
-00010f10: 6574 6129 202a 206e 702e 7369 6e28 7068  eta) * np.sin(ph
-00010f20: 6929 202a 206e 702e 636f 7328 7073 6929  i) * np.cos(psi)
-00010f30: 0a20 2020 2020 6575 6c65 725b 302c 2032  .     euler[0, 2
-00010f40: 5d20 3d20 206e 702e 7369 6e28 7468 6574  ] =  np.sin(thet
-00010f50: 6129 202a 206e 702e 7369 6e28 7068 6929  a) * np.sin(phi)
-00010f60: 0a20 2020 2020 6575 6c65 725b 312c 2030  .     euler[1, 0
-00010f70: 5d20 3d20 206e 702e 636f 7328 7073 6929  ] =  np.cos(psi)
-00010f80: 202a 206e 702e 7369 6e28 7068 6929 202b   * np.sin(phi) +
-00010f90: 206e 702e 636f 7328 7468 6574 6129 202a   np.cos(theta) *
-00010fa0: 206e 702e 636f 7328 7068 6929 202a 206e   np.cos(phi) * n
-00010fb0: 702e 7369 6e28 7073 6929 0a20 2020 2020  p.sin(psi).     
-00010fc0: 6575 6c65 725b 312c 2031 5d20 3d20 2d6e  euler[1, 1] = -n
-00010fd0: 702e 7369 6e28 7073 6929 202a 206e 702e  p.sin(psi) * np.
-00010fe0: 7369 6e28 7068 6929 202b 206e 702e 636f  sin(phi) + np.co
-00010ff0: 7328 7468 6574 6129 202a 206e 702e 636f  s(theta) * np.co
-00011000: 7328 7068 6929 202a 206e 702e 636f 7328  s(phi) * np.cos(
-00011010: 7073 6929 0a20 2020 2020 6575 6c65 725b  psi).     euler[
-00011020: 312c 2032 5d20 3d20 2d6e 702e 7369 6e28  1, 2] = -np.sin(
-00011030: 7468 6574 6129 202a 206e 702e 636f 7328  theta) * np.cos(
-00011040: 7068 6929 0a20 2020 2020 6575 6c65 725b  phi).     euler[
-00011050: 322c 2030 5d20 3d20 206e 702e 7369 6e28  2, 0] =  np.sin(
-00011060: 7468 6574 6129 202a 206e 702e 7369 6e28  theta) * np.sin(
-00011070: 7073 6929 0a20 2020 2020 6575 6c65 725b  psi).     euler[
-00011080: 322c 2031 5d20 3d20 206e 702e 7369 6e28  2, 1] =  np.sin(
-00011090: 7468 6574 6129 202a 206e 702e 636f 7328  theta) * np.cos(
-000110a0: 7073 6929 0a20 2020 2020 6575 6c65 725b  psi).     euler[
-000110b0: 322c 2032 5d20 3d20 206e 702e 636f 7328  2, 2] =  np.cos(
-000110c0: 7468 6574 6129 0a20 2020 2020 7265 7375  theta).     resu
-000110d0: 6c74 203d 206e 702e 6d61 746d 756c 2865  lt = np.matmul(e
-000110e0: 756c 6572 2c20 7665 6374 6f72 290a 2020  uler, vector).  
-000110f0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00011100: 0a0a 6465 6620 6765 745f 706f 6f6c 286e  ..def get_pool(n
-00011110: 6370 7573 2c20 7468 7265 6164 696e 672c  cpus, threading,
-00011120: 2069 6e69 7469 616c 697a 6572 3d4e 6f6e   initializer=Non
-00011130: 652c 2069 6e69 7461 7267 733d 4e6f 6e65  e, initargs=None
-00011140: 2c20 6465 6275 6767 6572 3d4e 6f6e 6520  , debugger=None 
-00011150: 293a 0a20 2020 2020 2222 2252 6574 7572  ):.     """Retur
-00011160: 6e20 6120 706f 6f6c 206f 6620 7072 6f63  n a pool of proc
-00011170: 6573 736f 7273 2067 6976 656e 2074 6865  essors given the
-00011180: 206e 756d 6265 7220 6f66 2063 7075 7320   number of cpus 
-00011190: 616e 6420 7768 6574 6865 7220 7468 7265  and whether thre
-000111a0: 6164 696e 6720 6973 2072 6571 7565 7374  ading is request
-000111b0: 6564 2222 220a 2020 2020 2069 6620 6465  ed""".     if de
-000111c0: 6275 6767 6572 2069 7320 6e6f 7420 4e6f  bugger is not No
-000111d0: 6e65 3a0a 2020 2020 2020 2020 2064 6562  ne:.         deb
-000111e0: 7567 6765 722e 7072 696e 7428 2767 6574  ugger.print('get
-000111f0: 5f70 6f6f 6c20 6e63 7075 7320 3d20 272c  _pool ncpus = ',
-00011200: 6e63 7075 7329 0a20 2020 2020 2020 2020  ncpus).         
-00011210: 6465 6275 6767 6572 2e70 7269 6e74 2827  debugger.print('
-00011220: 6765 745f 706f 6f6c 2074 6872 6561 6469  get_pool threadi
-00011230: 6e67 203d 2027 2c74 6872 6561 6469 6e67  ng = ',threading
-00011240: 290a 2020 2020 2020 2020 2064 6562 7567  ).         debug
-00011250: 6765 722e 7072 696e 7428 2767 6574 5f70  ger.print('get_p
-00011260: 6f6f 6c20 696e 6974 6961 6c69 7a65 7220  ool initializer 
-00011270: 3d20 272c 696e 6974 6961 6c69 7a65 7229  = ',initializer)
-00011280: 0a20 2020 2020 2320 5377 6974 6368 206f  .     # Switch o
-00011290: 6666 206d 6b6c 2074 6872 6561 6469 6e67  ff mkl threading
-000112a0: 0a20 2020 2020 7472 793a 0a20 2020 2020  .     try:.     
-000112b0: 2020 2020 696d 706f 7274 206d 6b6c 0a20      import mkl. 
-000112c0: 2020 2020 2020 2020 6d6b 6c2e 7365 745f          mkl.set_
-000112d0: 6e75 6d5f 7468 7265 6164 7328 3129 0a20  num_threads(1). 
-000112e0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-000112f0: 2020 2020 2070 6173 730a 2020 2020 2023       pass.     #
-00011300: 2073 6565 2069 6620 7468 7265 6164 696e   see if threadin
-00011310: 6720 6861 7320 6265 656e 2072 6571 7565  g has been reque
-00011320: 7374 6564 0a20 2020 2020 6966 2074 6872  sted.     if thr
-00011330: 6561 6469 6e67 3a0a 2020 2020 2020 2020  eading:.        
-00011340: 2066 726f 6d20 6d75 6c74 6970 726f 6365   from multiproce
-00011350: 7373 696e 672e 6475 6d6d 7920 696d 706f  ssing.dummy impo
-00011360: 7274 2050 6f6f 6c0a 2020 2020 2020 2020  rt Pool.        
-00011370: 2070 6f6f 6c20 3d20 506f 6f6c 286e 6370   pool = Pool(ncp
-00011380: 7573 2c20 696e 6974 6961 6c69 7a65 723d  us, initializer=
-00011390: 696e 6974 6961 6c69 7a65 722c 2069 6e69  initializer, ini
-000113a0: 7461 7267 733d 696e 6974 6172 6773 290a  targs=initargs).
-000113b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000113c0: 2020 2020 6672 6f6d 206d 756c 7469 7072      from multipr
-000113d0: 6f63 6573 7369 6e67 2069 6d70 6f72 7420  ocessing import 
-000113e0: 506f 6f6c 0a20 2020 2020 2020 2020 706f  Pool.         po
-000113f0: 6f6c 203d 2050 6f6f 6c28 6e63 7075 732c  ol = Pool(ncpus,
-00011400: 2069 6e69 7469 616c 697a 6572 3d69 6e69   initializer=ini
-00011410: 7469 616c 697a 6572 2c20 696e 6974 6172  tializer, initar
-00011420: 6773 3d69 6e69 7461 7267 7320 290a 2020  gs=initargs ).  
-00011430: 2020 2072 6574 7572 6e20 706f 6f6c 0a0a     return pool..
-00011440: 6465 6620 7365 745f 6166 6669 6e69 7479  def set_affinity
-00011450: 5f6f 6e5f 776f 726b 6572 2829 3a0a 2020  _on_worker():.  
-00011460: 2020 2727 2757 6865 6e20 6120 6e65 7720    '''When a new 
-00011470: 776f 726b 6572 2070 726f 6365 7373 2069  worker process i
-00011480: 7320 6372 6561 7465 642c 2074 6865 2061  s created, the a
-00011490: 6666 696e 6974 7920 6973 2073 6574 2074  ffinity is set t
-000114a0: 6f20 616c 6c20 4350 5573 2727 270a 2020  o all CPUs'''.  
-000114b0: 2020 234a 4b20 7072 696e 7428 2749 276d    #JK print('I'm
-000114c0: 2074 6865 2070 726f 6365 7373 2025 642c   the process %d,
-000114d0: 2073 6574 7469 6e67 2061 6666 696e 6974   setting affinit
-000114e0: 7920 746f 2061 6c6c 2043 5055 732e 2720  y to all CPUs.' 
-000114f0: 2520 6f73 2e67 6574 7069 6428 2929 0a20  % os.getpid()). 
-00011500: 2020 2023 4a4b 2043 6f6d 6d65 6e74 6564     #JK Commented
-00011510: 206f 7574 2066 6f72 2074 6865 2074 696d   out for the tim
-00011520: 6520 6265 696e 670a 2020 2020 234a 4b20  e being.    #JK 
-00011530: 6f73 2e73 7973 7465 6d28 2774 6173 6b73  os.system('tasks
-00011540: 6574 202d 7020 3078 6666 2025 6420 3e20  et -p 0xff %d > 
-00011550: 2f64 6576 2f6e 756c 6c27 2025 206f 732e  /dev/null' % os.
-00011560: 6765 7470 6964 2829 290a 2020 2020 7265  getpid()).    re
-00011570: 7475 726e 0a0a 0a                        turn...
+00000530: 3d66 6c6f 6174 290a 2020 2020 785b 302c  =float).    x[0,
+00000540: 2030 5d20 3d20 312e 300a 2020 2020 785b   0] = 1.0.    x[
+00000550: 312c 2031 5d20 3d20 312e 300a 2020 2020  1, 1] = 1.0.    
+00000560: 785b 322c 2032 5d20 3d20 312e 300a 2020  x[2, 2] = 1.0.  
+00000570: 2020 7265 7475 726e 2078 0a0a 6465 6620    return x..def 
+00000580: 696e 6974 6961 6c69 7365 5f63 6f6d 706c  initialise_compl
+00000590: 6578 5f64 6961 676f 6e61 6c5f 7465 6e73  ex_diagonal_tens
+000005a0: 6f72 2872 6561 6c73 293a 0a20 2020 2027  or(reals):.    '
+000005b0: 2727 496e 6974 6961 6c69 7365 2061 2033  ''Initialise a 3
+000005c0: 7833 2074 656e 736f 722c 2074 6865 2061  x3 tensor, the a
+000005d0: 7267 756d 656e 7420 6973 2061 206c 6973  rgument is a lis
+000005e0: 7420 6f66 2033 2072 6561 6c20 6e75 6d62  t of 3 real numb
+000005f0: 6572 7320 666f 7220 7468 6520 6469 6167  ers for the diag
+00000600: 6f6e 616c 732c 2074 6865 2072 6574 7572  onals, the retur
+00000610: 6e65 6420 7465 6e73 6f72 2069 7320 616e  ned tensor is an
+00000620: 2061 7272 6179 2727 270a 2020 2020 7820   array'''.    x 
+00000630: 3d20 6e70 2e7a 6572 6f73 2828 332c 2033  = np.zeros((3, 3
+00000640: 292c 2064 7479 7065 3d63 6f6d 706c 6578  ), dtype=complex
+00000650: 290a 2020 2020 785b 302c 2030 5d20 3d20  ).    x[0, 0] = 
+00000660: 7265 616c 735b 305d 0a20 2020 2078 5b31  reals[0].    x[1
+00000670: 2c20 315d 203d 2072 6561 6c73 5b31 5d0a  , 1] = reals[1].
+00000680: 2020 2020 785b 322c 2032 5d20 3d20 7265      x[2, 2] = re
+00000690: 616c 735b 325d 0a20 2020 2072 6574 7572  als[2].    retur
+000006a0: 6e20 780a 0a64 6566 2069 6e69 7469 616c  n x..def initial
+000006b0: 6973 655f 6469 6167 6f6e 616c 5f74 656e  ise_diagonal_ten
+000006c0: 736f 7228 7265 616c 7329 3a0a 2020 2020  sor(reals):.    
+000006d0: 2727 2749 6e69 7469 616c 6973 6520 6120  '''Initialise a 
+000006e0: 3378 3320 7465 6e73 6f72 2c20 7468 6520  3x3 tensor, the 
+000006f0: 6172 6775 6d65 6e74 2069 7320 6120 6c69  argument is a li
+00000700: 7374 206f 6620 3320 7265 616c 206e 756d  st of 3 real num
+00000710: 6265 7273 2066 6f72 2074 6865 2064 6961  bers for the dia
+00000720: 676f 6e61 6c73 2c20 7468 6520 7265 7475  gonals, the retu
+00000730: 726e 6564 2074 656e 736f 7220 6973 2061  rned tensor is a
+00000740: 6e20 6172 7261 7927 2727 0a20 2020 2078  n array'''.    x
+00000750: 203d 206e 702e 7a65 726f 7328 2833 2c20   = np.zeros((3, 
+00000760: 3329 2c20 6474 7970 653d 666c 6f61 7429  3), dtype=float)
+00000770: 0a20 2020 2078 5b30 2c20 305d 203d 2072  .    x[0, 0] = r
+00000780: 6561 6c73 5b30 5d0a 2020 2020 785b 312c  eals[0].    x[1,
+00000790: 2031 5d20 3d20 7265 616c 735b 315d 0a20   1] = reals[1]. 
+000007a0: 2020 2078 5b32 2c20 325d 203d 2072 6561     x[2, 2] = rea
+000007b0: 6c73 5b32 5d0a 2020 2020 7265 7475 726e  ls[2].    return
+000007c0: 2078 0a0a 6465 6620 6361 6c63 756c 6174   x..def calculat
+000007d0: 655f 6469 7374 616e 6365 2861 2c62 293a  e_distance(a,b):
+000007e0: 0a20 2020 2027 2727 4361 6c63 756c 6174  .    '''Calculat
+000007f0: 6520 7468 6520 6469 7374 616e 6365 2062  e the distance b
+00000800: 6574 7765 656e 2061 2061 6e64 2062 2727  etween a and b''
+00000810: 270a 2020 2020 6420 3d20 302e 300a 2020  '.    d = 0.0.  
+00000820: 2020 666f 7220 6331 2c20 6332 2069 6e20    for c1, c2 in 
+00000830: 7a69 7028 612c 6229 3a0a 2020 2020 2020  zip(a,b):.      
+00000840: 2020 6420 2b3d 2028 6332 202d 2063 3129    d += (c2 - c1)
+00000850: 2a28 6332 202d 2063 3129 0a20 2020 2072  *(c2 - c1).    r
+00000860: 6574 7572 6e20 6d61 7468 2e73 7172 7428  eturn math.sqrt(
+00000870: 6429 0a0a 6465 6620 696e 6974 6961 6c69  d)..def initiali
+00000880: 7365 5f72 616e 646f 6d5f 7465 6e73 6f72  se_random_tensor
+00000890: 2873 6361 6c65 293a 0a20 2020 2027 2727  (scale):.    '''
+000008a0: 496e 6974 6961 6c69 7365 2061 2033 7833  Initialise a 3x3
+000008b0: 2063 6f6d 706c 6578 2074 656e 736f 722c   complex tensor,
+000008c0: 2074 6865 2061 7267 756d 656e 7420 6769   the argument gi
+000008d0: 7665 7320 7468 6520 6d61 7869 6d75 6d20  ves the maximum 
+000008e0: 6162 736f 6c75 7465 2076 616c 7565 2727  absolute value''
+000008f0: 270a 2020 2020 7072 696e 7428 2245 7272  '.    print("Err
+00000900: 6f72 2069 6e69 7469 616c 6973 655f 7261  or initialise_ra
+00000910: 6e64 6f6d 5f74 656e 736f 7220 6e6f 7420  ndom_tensor not 
+00000920: 776f 726b 696e 6722 2c20 6669 6c65 3d73  working", file=s
+00000930: 7973 2e73 7464 6572 7229 0a20 2020 2065  ys.stderr).    e
+00000940: 7869 7428 3129 0a20 2020 2072 6574 7572  xit(1).    retur
+00000950: 6e0a 0a64 6566 2069 6e69 7469 616c 6973  n..def initialis
+00000960: 655f 7370 6865 7265 5f64 6570 6f6c 6172  e_sphere_depolar
+00000970: 6973 6174 696f 6e5f 6d61 7472 6978 2829  isation_matrix()
+00000980: 3a0a 2020 2020 2727 2749 6e69 7469 616c  :.    '''Initial
+00000990: 6973 6520 6120 3378 3320 7465 6e73 6f72  ise a 3x3 tensor
+000009a0: 2077 6974 6820 7468 6520 7370 6865 7265   with the sphere
+000009b0: 2064 6570 6f6c 6172 6973 6174 696f 6e20   depolarisation 
+000009c0: 6d61 7472 6978 2c20 7265 7475 726e 7320  matrix, returns 
+000009d0: 6120 7465 6e73 6f72 2727 270a 2020 2020  a tensor'''.    
+000009e0: 6174 6869 7264 203d 2031 2e30 202f 2033  athird = 1.0 / 3
+000009f0: 2e30 0a20 2020 2074 656e 736f 7220 3d20  .0.    tensor = 
+00000a00: 696e 6974 6961 6c69 7365 5f64 6961 676f  initialise_diago
+00000a10: 6e61 6c5f 7465 6e73 6f72 285b 6174 6869  nal_tensor([athi
+00000a20: 7264 2c20 6174 6869 7264 2c20 6174 6869  rd, athird, athi
+00000a30: 7264 5d29 0a20 2020 2074 656e 736f 7220  rd]).    tensor 
+00000a40: 3d20 7465 6e73 6f72 202f 206e 702e 7472  = tensor / np.tr
+00000a50: 6163 6528 7465 6e73 6f72 290a 2020 2020  ace(tensor).    
+00000a60: 7265 7475 726e 2074 656e 736f 720a 0a64  return tensor..d
+00000a70: 6566 2069 6e69 7469 616c 6973 655f 706c  ef initialise_pl
+00000a80: 6174 655f 6465 706f 6c61 7269 7361 7469  ate_depolarisati
+00000a90: 6f6e 5f6d 6174 7269 7828 6e6f 726d 616c  on_matrix(normal
+00000aa0: 293a 0a20 2020 2027 2727 496e 6974 6961  ):.    '''Initia
+00000ab0: 6c69 7365 2061 2033 7833 2074 656e 736f  lise a 3x3 tenso
+00000ac0: 7220 7769 7468 2074 6865 2070 6c61 7465  r with the plate
+00000ad0: 2064 6570 6f6c 6172 6973 6174 696f 6e20   depolarisation 
+00000ae0: 6d61 7472 6978 2c20 7265 7475 726e 7320  matrix, returns 
+00000af0: 6120 7465 6e73 6f72 2727 270a 2020 2020  a tensor'''.    
+00000b00: 6e6f 726d 616c 203d 206e 6f72 6d61 6c20  normal = normal 
+00000b10: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
+00000b20: 286e 6f72 6d61 6c29 0a20 2020 2074 656e  (normal).    ten
+00000b30: 736f 7220 3d20 6e70 2e6f 7574 6572 286e  sor = np.outer(n
+00000b40: 6f72 6d61 6c2c 206e 6f72 6d61 6c29 0a20  ormal, normal). 
+00000b50: 2020 2074 656e 736f 7220 3d20 7465 6e73     tensor = tens
+00000b60: 6f72 202f 206e 702e 7472 6163 6528 7465  or / np.trace(te
+00000b70: 6e73 6f72 290a 2020 2020 7265 7475 726e  nsor).    return
+00000b80: 2074 656e 736f 720a 0a64 6566 2069 6e69   tensor..def ini
+00000b90: 7469 616c 6973 655f 6e65 6564 6c65 5f64  tialise_needle_d
+00000ba0: 6570 6f6c 6172 6973 6174 696f 6e5f 6d61  epolarisation_ma
+00000bb0: 7472 6978 2875 6e69 7175 6529 3a0a 2020  trix(unique):.  
+00000bc0: 2020 2727 2749 6e69 7469 616c 6973 6520    '''Initialise 
+00000bd0: 6120 3378 3320 7465 6e73 6f72 2077 6974  a 3x3 tensor wit
+00000be0: 6820 7468 6520 6e65 6564 6c65 2064 6570  h the needle dep
+00000bf0: 6f6c 6172 6973 6174 696f 6e20 6d61 7472  olarisation matr
+00000c00: 6978 2727 270a 2020 2020 2320 756e 6971  ix'''.    # uniq
+00000c10: 7565 2069 7320 7468 6520 756e 6971 7565  ue is the unique
+00000c20: 2064 6972 6563 7469 6f6e 206f 6620 7468   direction of th
+00000c30: 6520 6e65 6564 6c65 0a20 2020 2023 2064  e needle.    # d
+00000c40: 6570 6f6c 6172 6973 6174 696f 6e20 6d61  epolarisation ma
+00000c50: 7472 6978 2069 7320 7468 6572 6566 6f72  trix is therefor
+00000c60: 6520 6861 6c66 2074 6865 2073 756d 206f  e half the sum o
+00000c70: 6620 7468 650a 2020 2020 2320 7477 6f20  f the.    # two 
+00000c80: 6f75 7465 7220 7072 6f64 7563 7473 206f  outer products o
+00000c90: 6620 7468 6520 6469 7265 6374 696f 6e73  f the directions
+00000ca0: 2070 6572 7065 6e64 6963 756c 6172 2074   perpendicular t
+00000cb0: 6f20 6974 0a20 2020 2075 6e69 7175 6520  o it.    unique 
+00000cc0: 3d20 756e 6971 7565 202f 206e 702e 6c69  = unique / np.li
+00000cd0: 6e61 6c67 2e6e 6f72 6d28 756e 6971 7565  nalg.norm(unique
+00000ce0: 290a 2020 2020 7820 3d20 6e70 2e61 7272  ).    x = np.arr
+00000cf0: 6179 285b 312c 2030 2c20 305d 290a 2020  ay([1, 0, 0]).  
+00000d00: 2020 7920 3d20 6e70 2e61 7272 6179 285b    y = np.array([
+00000d10: 302c 2031 2c20 305d 290a 2020 2020 7a20  0, 1, 0]).    z 
+00000d20: 3d20 6e70 2e61 7272 6179 285b 302c 2030  = np.array([0, 0
+00000d30: 2c20 315d 290a 2020 2020 7864 6f74 6e20  , 1]).    xdotn 
+00000d40: 3d20 6e70 2e64 6f74 2878 2c20 756e 6971  = np.dot(x, uniq
+00000d50: 7565 290a 2020 2020 7964 6f74 6e20 3d20  ue).    ydotn = 
+00000d60: 6e70 2e64 6f74 2879 2c20 756e 6971 7565  np.dot(y, unique
+00000d70: 290a 2020 2020 7a64 6f74 6e20 3d20 6e70  ).    zdotn = np
+00000d80: 2e64 6f74 287a 2c20 756e 6971 7565 290a  .dot(z, unique).
+00000d90: 2020 2020 6162 7378 646f 746e 203d 206e      absxdotn = n
+00000da0: 702e 6162 7328 7864 6f74 6e29 0a20 2020  p.abs(xdotn).   
+00000db0: 2061 6273 7964 6f74 6e20 3d20 6e70 2e61   absydotn = np.a
+00000dc0: 6273 2879 646f 746e 290a 2020 2020 6162  bs(ydotn).    ab
+00000dd0: 737a 646f 746e 203d 206e 702e 6162 7328  szdotn = np.abs(
+00000de0: 7a64 6f74 6e29 0a20 2020 2023 2063 686f  zdotn).    # cho
+00000df0: 6f73 6520 7468 6520 6469 7265 6374 696f  ose the directio
+00000e00: 6e20 7769 7468 2074 6865 2073 6d61 6c6c  n with the small
+00000e10: 6573 7420 7072 6f6a 6563 7469 6f6e 2061  est projection a
+00000e20: 6c6f 6e67 2074 6865 206e 6565 646c 650a  long the needle.
+00000e30: 2020 2020 2320 7468 656e 2070 726f 6a65      # then proje
+00000e40: 6374 206f 7574 2061 6e79 206e 6565 646c  ct out any needl
+00000e50: 6520 6469 7265 6374 696f 6e0a 2020 2020  e direction.    
+00000e60: 6966 2061 6273 7864 6f74 6e20 3c3d 2061  if absxdotn <= a
+00000e70: 6273 7964 6f74 6e20 616e 6420 6162 7378  bsydotn and absx
+00000e80: 646f 746e 203c 3d20 6162 737a 646f 746e  dotn <= abszdotn
+00000e90: 3a0a 2020 2020 2020 2020 6469 7231 203d  :.        dir1 =
+00000ea0: 2078 202d 2028 7864 6f74 6e20 2a20 756e   x - (xdotn * un
+00000eb0: 6971 7565 290a 2020 2020 656c 6966 2061  ique).    elif a
+00000ec0: 6273 7964 6f74 6e20 3c3d 2061 6273 7864  bsydotn <= absxd
+00000ed0: 6f74 6e20 616e 6420 6162 7379 646f 746e  otn and absydotn
+00000ee0: 203c 3d20 6162 737a 646f 746e 3a0a 2020   <= abszdotn:.  
+00000ef0: 2020 2020 2020 6469 7231 203d 2079 202d        dir1 = y -
+00000f00: 2028 7964 6f74 6e20 2a20 756e 6971 7565   (ydotn * unique
+00000f10: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00000f20: 2020 2020 6469 7231 203d 207a 202d 2028      dir1 = z - (
+00000f30: 7a64 6f74 6e20 2a20 756e 6971 7565 290a  zdotn * unique).
+00000f40: 2020 2020 6469 7231 203d 2064 6972 312f      dir1 = dir1/
+00000f50: 6e70 2e6c 696e 616c 672e 6e6f 726d 2864  np.linalg.norm(d
+00000f60: 6972 3129 0a20 2020 2023 206e 6f77 2066  ir1).    # now f
+00000f70: 696e 6420 7468 6520 6f72 7468 6f67 6f6e  ind the orthogon
+00000f80: 616c 2064 6972 6563 7469 6f6e 0a20 2020  al direction.   
+00000f90: 2064 6972 3220 3d20 6e70 2e63 726f 7373   dir2 = np.cross
+00000fa0: 2875 6e69 7175 652c 2064 6972 3129 0a20  (unique, dir1). 
+00000fb0: 2020 2064 6972 3220 3d20 6469 7232 2f6e     dir2 = dir2/n
+00000fc0: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6469  p.linalg.norm(di
+00000fd0: 7232 290a 2020 2020 2320 636f 6d70 7574  r2).    # comput
+00000fe0: 6520 7468 6520 636f 6d70 6c65 7820 7465  e the complex te
+00000ff0: 6e73 6f72 7320 6672 6f6d 2074 6865 206f  nsors from the o
+00001000: 7574 6572 2070 726f 6475 6374 206f 6620  uter product of 
+00001010: 6561 6368 2064 6972 6563 7469 6f6e 0a20  each direction. 
+00001020: 2020 2074 656e 736f 7220 3d20 6e70 2e6f     tensor = np.o
+00001030: 7574 6572 2864 6972 312c 2064 6972 3129  uter(dir1, dir1)
+00001040: 202b 206e 702e 6f75 7465 7228 6469 7232   + np.outer(dir2
+00001050: 2c20 6469 7232 290a 2020 2020 7465 6e73  , dir2).    tens
+00001060: 6f72 203d 2074 656e 736f 7220 2f20 6e70  or = tensor / np
+00001070: 2e74 7261 6365 2874 656e 736f 7229 0a20  .trace(tensor). 
+00001080: 2020 2072 6574 7572 6e20 7465 6e73 6f72     return tensor
+00001090: 0a0a 6465 6620 696e 6974 6961 6c69 7365  ..def initialise
+000010a0: 5f65 6c6c 6970 736f 6964 5f64 6570 6f6c  _ellipsoid_depol
+000010b0: 6172 6973 6174 696f 6e5f 6d61 7472 6978  arisation_matrix
+000010c0: 2875 6e69 7175 652c 2061 6f76 6572 6229  (unique, aoverb)
+000010d0: 3a0a 2020 2020 2727 2749 6e69 7469 616c  :.    '''Initial
+000010e0: 6973 6520 6120 3378 3320 7465 6e73 6f72  ise a 3x3 tensor
+000010f0: 2077 6974 6820 7468 6520 656c 6c69 7073   with the ellips
+00001100: 6f69 6420 6465 706f 6c61 7269 7361 7469  oid depolarisati
+00001110: 6f6e 206d 6174 7269 7827 2727 0a20 2020  on matrix'''.   
+00001120: 2023 2075 6e69 7175 6520 6973 2074 6865   # unique is the
+00001130: 2075 6e69 7175 6520 6469 7265 6374 696f   unique directio
+00001140: 6e20 6f66 2074 6865 2065 6c6c 6970 736f  n of the ellipso
+00001150: 6964 0a20 2020 2023 2061 2061 6e64 2062  id.    # a and b
+00001160: 2061 7265 2074 6865 2073 697a 6573 206f   are the sizes o
+00001170: 6620 7468 6520 656c 6c69 7073 6f69 6420  f the ellipsoid 
+00001180: 616c 6f6e 6720 7468 6520 756e 6971 7565  along the unique
+00001190: 2061 7869 7320 2861 2920 616e 6420 7065   axis (a) and pe
+000011a0: 7270 656e 6469 6375 6c61 7220 746f 2069  rpendicular to i
+000011b0: 7420 620a 2020 2020 2320 6966 2061 203e  t b.    # if a >
+000011c0: 2062 2074 6865 6e20 7765 2068 6176 6520   b then we have 
+000011d0: 6120 7072 6f6c 6174 6520 656c 6c69 7073  a prolate ellips
+000011e0: 6f69 640a 2020 2020 756e 6971 7565 203d  oid.    unique =
+000011f0: 2075 6e69 7175 6520 2f20 6e70 2e6c 696e   unique / np.lin
+00001200: 616c 672e 6e6f 726d 2875 6e69 7175 6529  alg.norm(unique)
+00001210: 0a20 2020 2078 203d 206e 702e 6172 7261  .    x = np.arra
+00001220: 7928 5b31 2c20 302c 2030 5d29 0a20 2020  y([1, 0, 0]).   
+00001230: 2079 203d 206e 702e 6172 7261 7928 5b30   y = np.array([0
+00001240: 2c20 312c 2030 5d29 0a20 2020 207a 203d  , 1, 0]).    z =
+00001250: 206e 702e 6172 7261 7928 5b30 2c20 302c   np.array([0, 0,
+00001260: 2031 5d29 0a20 2020 2078 646f 746e 203d   1]).    xdotn =
+00001270: 206e 702e 646f 7428 782c 2075 6e69 7175   np.dot(x, uniqu
+00001280: 6529 0a20 2020 2079 646f 746e 203d 206e  e).    ydotn = n
+00001290: 702e 646f 7428 792c 2075 6e69 7175 6529  p.dot(y, unique)
+000012a0: 0a20 2020 207a 646f 746e 203d 206e 702e  .    zdotn = np.
+000012b0: 646f 7428 7a2c 2075 6e69 7175 6529 0a20  dot(z, unique). 
+000012c0: 2020 2061 6273 7864 6f74 6e20 3d20 6e70     absxdotn = np
+000012d0: 2e61 6273 2878 646f 746e 290a 2020 2020  .abs(xdotn).    
+000012e0: 6162 7379 646f 746e 203d 206e 702e 6162  absydotn = np.ab
+000012f0: 7328 7964 6f74 6e29 0a20 2020 2061 6273  s(ydotn).    abs
+00001300: 7a64 6f74 6e20 3d20 6e70 2e61 6273 287a  zdotn = np.abs(z
+00001310: 646f 746e 290a 2020 2020 2320 6368 6f6f  dotn).    # choo
+00001320: 7365 2074 6865 2064 6972 6563 7469 6f6e  se the direction
+00001330: 2077 6974 6820 7468 6520 736d 616c 6c65   with the smalle
+00001340: 7374 2070 726f 6a65 6374 696f 6e20 616c  st projection al
+00001350: 6f6e 6720 7468 6520 656c 6c69 7073 6f69  ong the ellipsoi
+00001360: 640a 2020 2020 2320 7468 656e 2070 726f  d.    # then pro
+00001370: 6a65 6374 206f 7574 2061 6e79 2065 6c6c  ject out any ell
+00001380: 6970 736f 6964 2064 6972 6563 7469 6f6e  ipsoid direction
+00001390: 0a20 2020 2069 6620 6162 7378 646f 746e  .    if absxdotn
+000013a0: 203c 3d20 6162 7379 646f 746e 2061 6e64   <= absydotn and
+000013b0: 2061 6273 7864 6f74 6e20 3c3d 2061 6273   absxdotn <= abs
+000013c0: 7a64 6f74 6e3a 0a20 2020 2020 2020 2064  zdotn:.        d
+000013d0: 6972 3120 3d20 7820 2d20 2878 646f 746e  ir1 = x - (xdotn
+000013e0: 202a 2075 6e69 7175 6529 0a20 2020 2065   * unique).    e
+000013f0: 6c69 6620 6162 7379 646f 746e 203c 3d20  lif absydotn <= 
+00001400: 6162 7378 646f 746e 2061 6e64 2061 6273  absxdotn and abs
+00001410: 7964 6f74 6e20 3c3d 2061 6273 7a64 6f74  ydotn <= abszdot
+00001420: 6e3a 0a20 2020 2020 2020 2064 6972 3120  n:.        dir1 
+00001430: 3d20 7920 2d20 2879 646f 746e 202a 2075  = y - (ydotn * u
+00001440: 6e69 7175 6529 0a20 2020 2065 6c73 653a  nique).    else:
+00001450: 0a20 2020 2020 2020 2064 6972 3120 3d20  .        dir1 = 
+00001460: 7a20 2d20 287a 646f 746e 202a 2075 6e69  z - (zdotn * uni
+00001470: 7175 6529 0a20 2020 2064 6972 3120 3d20  que).    dir1 = 
+00001480: 6469 7231 2f6e 702e 6c69 6e61 6c67 2e6e  dir1/np.linalg.n
+00001490: 6f72 6d28 6469 7231 290a 2020 2020 2320  orm(dir1).    # 
+000014a0: 6e6f 7720 6669 6e64 2074 6865 206f 7274  now find the ort
+000014b0: 686f 676f 6e61 6c20 6469 7265 6374 696f  hogonal directio
+000014c0: 6e0a 2020 2020 6469 7232 203d 206e 702e  n.    dir2 = np.
+000014d0: 6372 6f73 7328 756e 6971 7565 2c20 6469  cross(unique, di
+000014e0: 7231 290a 2020 2020 6469 7232 203d 2064  r1).    dir2 = d
+000014f0: 6972 322f 6e70 2e6c 696e 616c 672e 6e6f  ir2/np.linalg.no
+00001500: 726d 2864 6972 3229 0a20 2020 2062 6f76  rm(dir2).    bov
+00001510: 6572 6120 3d20 312e 3020 2f20 616f 7665  era = 1.0 / aove
+00001520: 7262 0a20 2020 2073 6d61 6c6c 203d 2031  rb.    small = 1
+00001530: 2e30 452d 380a 2020 2020 6966 2062 6f76  .0E-8.    if bov
+00001540: 6572 6120 3c20 312e 302d 736d 616c 6c3a  era < 1.0-small:
+00001550: 0a20 2020 2020 2020 2065 203d 206d 6174  .        e = mat
+00001560: 682e 7371 7274 2831 2e30 2020 2d20 626f  h.sqrt(1.0  - bo
+00001570: 7665 7261 2a62 6f76 6572 6129 0a20 2020  vera*bovera).   
+00001580: 2020 2020 206e 7a20 3d20 2831 202d 2065       nz = (1 - e
+00001590: 2a65 2920 2a20 286e 702e 6c6f 6728 2828  *e) * (np.log(((
+000015a0: 312b 6529 202f 2028 312d 6529 2929 202d  1+e) / (1-e))) -
+000015b0: 2032 2a65 2920 2f20 2832 2a65 2a65 2a65   2*e) / (2*e*e*e
+000015c0: 290a 2020 2020 656c 6966 2062 6f76 6572  ).    elif bover
+000015d0: 6120 3e20 312e 302b 736d 616c 6c3a 0a20  a > 1.0+small:. 
+000015e0: 2020 2020 2020 2065 203d 206d 6174 682e         e = math.
+000015f0: 7371 7274 2862 6f76 6572 612a 626f 7665  sqrt(bovera*bove
+00001600: 7261 202d 2031 2e30 290a 2020 2020 2020  ra - 1.0).      
+00001610: 2020 6e7a 203d 2028 3120 2b20 652a 6529    nz = (1 + e*e)
+00001620: 202a 2028 6520 2d20 6e70 2e61 7263 7461   * (e - np.arcta
+00001630: 6e28 6529 2920 2f20 2865 2a65 2a65 290a  n(e)) / (e*e*e).
+00001640: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001650: 2020 6e7a 203d 2031 2e30 2f33 2e30 0a20    nz = 1.0/3.0. 
+00001660: 2020 206e 7879 203d 2028 3120 2d20 6e7a     nxy = (1 - nz
+00001670: 2920 2a20 302e 350a 2020 2020 230a 2020  ) * 0.5.    #.  
+00001680: 2020 2320 636f 6d70 7574 6520 7468 6520    # compute the 
+00001690: 7465 6e73 6f72 7320 6672 6f6d 2074 6865  tensors from the
+000016a0: 206f 7574 6572 2070 726f 6475 6374 206f   outer product o
+000016b0: 6620 6561 6368 2064 6972 6563 7469 6f6e  f each direction
+000016c0: 0a20 2020 2074 656e 736f 7220 3d20 6e7a  .    tensor = nz
+000016d0: 2a6e 702e 6f75 7465 7228 756e 6971 7565  *np.outer(unique
+000016e0: 2c20 756e 6971 7565 2920 2b20 6e78 792a  , unique) + nxy*
+000016f0: 6e70 2e6f 7574 6572 2864 6972 312c 2064  np.outer(dir1, d
+00001700: 6972 3129 202b 206e 7879 2a6e 702e 6f75  ir1) + nxy*np.ou
+00001710: 7465 7228 6469 7232 2c20 6469 7232 290a  ter(dir2, dir2).
+00001720: 2020 2020 7465 6e73 6f72 203d 2074 656e      tensor = ten
+00001730: 736f 7220 2f20 6e70 2e74 7261 6365 2874  sor / np.trace(t
+00001740: 656e 736f 7229 0a20 2020 2072 6574 7572  ensor).    retur
+00001750: 6e20 7465 6e73 6f72 0a0a 6465 6620 6669  n tensor..def fi
+00001760: 626f 6e61 6363 695f 7370 6865 7265 2873  bonacci_sphere(s
+00001770: 616d 706c 6573 3d31 2c72 616e 646f 6d69  amples=1,randomi
+00001780: 7a65 3d54 7275 6529 3a0a 2020 2020 726e  ze=True):.    rn
+00001790: 6420 3d20 312e 0a20 2020 2069 6620 7261  d = 1..    if ra
+000017a0: 6e64 6f6d 697a 653a 0a20 2020 2020 2020  ndomize:.       
+000017b0: 2072 6e64 203d 2072 616e 646f 6d2e 7261   rnd = random.ra
+000017c0: 6e64 6f6d 2829 202a 2073 616d 706c 6573  ndom() * samples
+000017d0: 0a0a 2020 2020 706f 696e 7473 203d 205b  ..    points = [
+000017e0: 5d0a 2020 2020 6f66 6673 6574 203d 2032  ].    offset = 2
+000017f0: 2e2f 7361 6d70 6c65 730a 2020 2020 696e  ./samples.    in
+00001800: 6372 656d 656e 7420 3d20 6d61 7468 2e70  crement = math.p
+00001810: 6920 2a20 2833 2e20 2d20 6d61 7468 2e73  i * (3. - math.s
+00001820: 7172 7428 352e 2929 3b0a 0a20 2020 2066  qrt(5.));..    f
+00001830: 6f72 2069 2069 6e20 7261 6e67 6528 7361  or i in range(sa
+00001840: 6d70 6c65 7329 3a0a 2020 2020 2020 2020  mples):.        
+00001850: 7920 3d20 2828 6920 2a20 6f66 6673 6574  y = ((i * offset
+00001860: 2920 2d20 3129 202b 2028 6f66 6673 6574  ) - 1) + (offset
+00001870: 202f 2032 293b 0a20 2020 2020 2020 2072   / 2);.        r
+00001880: 203d 206d 6174 682e 7371 7274 2831 202d   = math.sqrt(1 -
+00001890: 2070 6f77 2879 2c32 2929 0a0a 2020 2020   pow(y,2))..    
+000018a0: 2020 2020 7068 6920 3d20 2828 6920 2b20      phi = ((i + 
+000018b0: 726e 6429 2025 2073 616d 706c 6573 2920  rnd) % samples) 
+000018c0: 2a20 696e 6372 656d 656e 740a 0a20 2020  * increment..   
+000018d0: 2020 2020 2078 203d 206d 6174 682e 636f       x = math.co
+000018e0: 7328 7068 6929 202a 2072 0a20 2020 2020  s(phi) * r.     
+000018f0: 2020 207a 203d 206d 6174 682e 7369 6e28     z = math.sin(
+00001900: 7068 6929 202a 2072 0a0a 2020 2020 2020  phi) * r..      
+00001910: 2020 706f 696e 7473 2e61 7070 656e 6428    points.append(
+00001920: 5b78 2c79 2c7a 5d29 0a0a 2020 2020 7265  [x,y,z])..    re
+00001930: 7475 726e 2070 6f69 6e74 730a 0a64 6566  turn points..def
+00001940: 2069 6f6e 6963 5f70 6572 6d69 7474 6976   ionic_permittiv
+00001950: 6974 7928 6d6f 6465 5f6c 6973 742c 206f  ity(mode_list, o
+00001960: 7363 696c 6c61 746f 725f 7374 7265 6e67  scillator_streng
+00001970: 7468 732c 2066 7265 7175 656e 6369 6573  ths, frequencies
+00001980: 2c20 766f 6c75 6d65 293a 0a20 2020 2022  , volume):.    "
+00001990: 2222 4361 6c63 756c 6174 6520 7468 6520  ""Calculate the 
+000019a0: 6c6f 7720 6672 6571 7565 6e63 7920 7065  low frequency pe
+000019b0: 726d 6974 7469 7669 7479 206f 7220 7a65  rmittivity or ze
+000019c0: 726f 2066 7265 7175 656e 6379 2070 6572  ro frequency per
+000019d0: 6d69 7474 6976 6974 790a 2020 2020 2020  mittivity.      
+000019e0: 206f 7363 696c 6c61 746f 725f 7374 7265   oscillator_stre
+000019f0: 6e67 7468 7320 6172 6520 696e 2061 746f  ngths are in ato
+00001a00: 6d69 6320 756e 6974 730a 2020 2020 2020  mic units.      
+00001a10: 2066 7265 7175 656e 6369 6573 2061 7265   frequencies are
+00001a20: 2069 6e20 6174 6f6d 6963 2075 6e69 7473   in atomic units
+00001a30: 0a20 2020 2020 2020 766f 6c75 6d65 2069  .       volume i
+00001a40: 7320 696e 2061 746f 6d69 6320 756e 6974  s in atomic unit
+00001a50: 7322 2222 0a20 2020 2070 6572 6d69 7474  s""".    permitt
+00001a60: 6976 6974 7920 3d20 6e70 2e7a 6572 6f73  ivity = np.zeros
+00001a70: 2828 332c 2033 2929 0a20 2020 2066 6f72  ((3, 3)).    for
+00001a80: 2069 6d6f 6465 2069 6e20 6d6f 6465 5f6c   imode in mode_l
+00001a90: 6973 743a 0a20 2020 2020 2020 2070 6572  ist:.        per
+00001aa0: 6d69 7474 6976 6974 7920 3d20 7065 726d  mittivity = perm
+00001ab0: 6974 7469 7669 7479 202b 206f 7363 696c  ittivity + oscil
+00001ac0: 6c61 746f 725f 7374 7265 6e67 7468 735b  lator_strengths[
+00001ad0: 696d 6f64 655d 202f 2028 6672 6571 7565  imode] / (freque
+00001ae0: 6e63 6965 735b 696d 6f64 655d 202a 2066  ncies[imode] * f
+00001af0: 7265 7175 656e 6369 6573 5b69 6d6f 6465  requencies[imode
+00001b00: 5d29 0a20 2020 2023 2065 6e64 2066 6f72  ]).    # end for
+00001b10: 0a20 2020 2072 6574 7572 6e20 7065 726d  .    return perm
+00001b20: 6974 7469 7669 7479 202a 2028 3420 2a20  ittivity * (4 * 
+00001b30: 5049 202f 2076 6f6c 756d 6529 0a0a 6465  PI / volume)..de
+00001b40: 6620 696e 6672 6172 6564 5f69 6e74 656e  f infrared_inten
+00001b50: 7369 7469 6573 286f 7363 696c 6c61 746f  sities(oscillato
+00001b60: 725f 7374 7265 6e67 7468 7329 3a0a 2020  r_strengths):.  
+00001b70: 2020 2222 2243 616c 6375 6c61 7465 2074    """Calculate t
+00001b80: 6865 2049 5220 696e 7465 6e73 6974 6965  he IR intensitie
+00001b90: 7320 6672 6f6d 2074 6865 2074 7261 6365  s from the trace
+00001ba0: 206f 6620 7468 6520 6f73 6369 6c6c 6174   of the oscillat
+00001bb0: 6f72 2073 7472 656e 6774 6873 2c0a 2020  or strengths,.  
+00001bc0: 2020 2020 2054 6865 2069 6e74 656e 7369       The intensi
+00001bd0: 7469 6573 2061 7265 2072 6574 7572 6e65  ties are returne
+00001be0: 6420 696e 2075 6e69 7473 206f 6620 2844  d in units of (D
+00001bf0: 2f41 295e 322f 616d 7522 2222 0a20 2020  /A)^2/amu""".   
+00001c00: 2023 2045 6163 6820 6d6f 6465 2068 6173   # Each mode has
+00001c10: 2061 2033 7833 206f 7363 696c 6c61 746f   a 3x3 oscillato
+00001c20: 7220 7374 7265 6e67 7468 0a20 2020 206e  r strength.    n
+00001c30: 6d6f 6465 7320 3d20 6e70 2e73 697a 6528  modes = np.size(
+00001c40: 6f73 6369 6c6c 6174 6f72 5f73 7472 656e  oscillator_stren
+00001c50: 6774 6873 2c20 3029 0a20 2020 2069 6e74  gths, 0).    int
+00001c60: 656e 7369 7469 6573 203d 206e 702e 7a65  ensities = np.ze
+00001c70: 726f 7328 6e6d 6f64 6573 290a 2020 2020  ros(nmodes).    
+00001c80: 666f 7220 696d 6f64 652c 2073 7472 656e  for imode, stren
+00001c90: 6774 6820 696e 2065 6e75 6d65 7261 7465  gth in enumerate
+00001ca0: 286f 7363 696c 6c61 746f 725f 7374 7265  (oscillator_stre
+00001cb0: 6e67 7468 7329 3a0a 2020 2020 2020 2020  ngths):.        
+00001cc0: 2320 5765 2063 616c 6375 6c61 7465 2074  # We calculate t
+00001cd0: 6865 2069 6e74 656e 7369 7479 2066 726f  he intensity fro
+00001ce0: 6d20 7468 6520 7472 6163 6520 6f66 2074  m the trace of t
+00001cf0: 6865 2073 7472 656e 6774 6873 0a20 2020  he strengths.   
+00001d00: 2020 2020 2069 6e74 656e 7369 7469 6573       intensities
+00001d10: 5b69 6d6f 6465 5d20 3d20 696e 7465 6e73  [imode] = intens
+00001d20: 6974 6965 735b 696d 6f64 655d 202b 2073  ities[imode] + s
+00001d30: 7472 656e 6774 685b 302c 2030 5d20 2b20  trength[0, 0] + 
+00001d40: 7374 7265 6e67 7468 5b31 2c20 315d 202b  strength[1, 1] +
+00001d50: 2073 7472 656e 6774 685b 322c 2032 5d0a   strength[2, 2].
+00001d60: 2020 2020 2320 656e 6420 666f 720a 2020      # end for.  
+00001d70: 2020 6d61 7869 6e74 656e 7369 7479 203d    maxintensity =
+00001d80: 206e 702e 6d61 7828 696e 7465 6e73 6974   np.max(intensit
+00001d90: 6965 7329 0a20 2020 2063 6f6e 7665 7274  ies).    convert
+00001da0: 203d 206d 6178 696e 7465 6e73 6974 790a   = maxintensity.
+00001db0: 2020 2020 2320 636f 6e76 6572 7420 7468      # convert th
+00001dc0: 6520 696e 7465 6e73 6974 6965 7320 746f  e intensities to
+00001dd0: 2043 6173 7465 7020 756e 6974 7320 2844   Castep units (D
+00001de0: 2f41 292a 2a32 2f61 6d75 0a20 2020 2063  /A)**2/amu.    c
+00001df0: 6f6e 7665 7274 203d 2064 3262 7961 6d75  onvert = d2byamu
+00001e00: 616e 6732 0a20 2020 2069 6e74 656e 7369  ang2.    intensi
+00001e10: 7469 6573 203d 2069 6e74 656e 7369 7469  ties = intensiti
+00001e20: 6573 202f 2063 6f6e 7665 7274 0a20 2020  es / convert.   
+00001e30: 2072 6574 7572 6e20 696e 7465 6e73 6974   return intensit
+00001e40: 6965 730a 0a64 6566 206c 6f6e 6769 7475  ies..def longitu
+00001e50: 6469 6e61 6c5f 6d6f 6465 7328 6672 6571  dinal_modes(freq
+00001e60: 7565 6e63 6965 732c 206e 6f72 6d61 6c5f  uencies, normal_
+00001e70: 6d6f 6465 732c 2062 6f72 6e5f 6368 6172  modes, born_char
+00001e80: 6765 732c 206d 6173 7365 732c 2065 7073  ges, masses, eps
+00001e90: 696c 6f6e 5f69 6e66 2c20 766f 6c75 6d65  ilon_inf, volume
+00001ea0: 2c20 716c 6973 742c 2072 6561 6465 7229  , qlist, reader)
+00001eb0: 3a0a 2020 2020 2222 2241 7070 6c79 2074  :.    """Apply t
+00001ec0: 6865 206e 6f6e 616e 616c 7974 6963 2063  he nonanalytic c
+00001ed0: 6f72 7265 6374 696f 6e20 746f 2074 6865  orrection to the
+00001ee0: 2064 796e 616d 6963 616c 206d 6174 7269   dynamical matri
+00001ef0: 7820 616e 6420 6361 6c63 756c 6174 6520  x and calculate 
+00001f00: 7468 6520 4c4f 2066 7265 7175 656e 6369  the LO frequenci
+00001f10: 6573 0a20 2020 2020 2020 6672 6571 7565  es.       freque
+00001f20: 6e63 6965 7320 6172 6520 7468 6520 6672  ncies are the fr
+00001f30: 6571 7565 6e63 6965 7320 2866 2920 696e  equencies (f) in
+00001f40: 2061 746f 6d69 6320 756e 6974 730a 2020   atomic units.  
+00001f50: 2020 2020 206e 6f72 6d61 6c5f 6d6f 6465       normal_mode
+00001f60: 7320 6172 6520 7468 6520 6d61 7373 2077  s are the mass w
+00001f70: 6569 6768 7465 6420 6e6f 726d 616c 206d  eighted normal m
+00001f80: 6f64 6573 2028 5529 0a20 2020 2020 2020  odes (U).       
+00001f90: 626f 726e 5f63 6861 7267 6573 2061 7265  born_charges are
+00001fa0: 2074 6865 2062 6f72 6e20 6368 6172 6765   the born charge
+00001fb0: 7320 285a 2920 7374 6f72 6564 2061 730a  s (Z) stored as.
+00001fc0: 2020 2020 2020 2020 2020 5b5a 3178 205a            [Z1x Z
+00001fd0: 3179 205a 317a 5d20 5b5a 3278 205a 3279  1y Z1z] [Z2x Z2y
+00001fe0: 205a 327a 5d20 5b5a 3378 205a 3379 205a   Z2z] [Z3x Z3y Z
+00001ff0: 337a 5d5d 0a20 2020 2020 2020 2020 2077  3z]].          w
+00002000: 6865 7265 2031 2c20 322c 2033 2061 7265  here 1, 2, 3 are
+00002010: 2074 6865 2064 6972 6563 7469 6f6e 7320   the directions 
+00002020: 6f66 2074 6865 2066 6965 6c64 2061 6e64  of the field and
+00002030: 2078 2c20 792c 207a 2061 7265 2074 6865   x, y, z are the
+00002040: 2063 6f6f 7264 696e 6174 6573 206f 6620   coordinates of 
+00002050: 7468 6520 6174 6f6d 0a20 2020 2020 2020  the atom.       
+00002060: 716c 6973 7420 6973 2061 206c 6973 7420  qlist is a list 
+00002070: 6f66 2064 6972 6563 7469 6f6e 2076 6563  of direction vec
+00002080: 746f 7273 0a20 2020 2020 2020 5468 6520  tors.       The 
+00002090: 7375 6272 6f75 7469 6e65 2072 6574 7572  subroutine retur
+000020a0: 6e73 2061 206c 6973 7420 6f66 2028 7265  ns a list of (re
+000020b0: 616c 2920 6672 6571 7565 6e63 6965 7320  al) frequencies 
+000020c0: 696e 2061 746f 6d69 6320 756e 6974 730a  in atomic units.
+000020d0: 2020 2020 2020 2041 6e79 2069 6d61 6769         Any imagi
+000020e0: 6e61 7279 2066 7265 7175 656e 6369 6573  nary frequencies
+000020f0: 2061 7265 2073 6574 2074 6f20 300a 2020   are set to 0.  
+00002100: 2020 2020 2049 6620 7072 6f6a 6563 7469       If projecti
+00002110: 6f6e 2077 6173 2072 6571 7565 7374 6564  on was requested
+00002120: 2069 6e20 7468 6520 7265 6164 6572 2c20   in the reader, 
+00002130: 7468 6520 636f 7272 6563 7469 6f6e 2069  the correction i
+00002140: 7320 6d6f 6469 6669 6564 2065 6e73 7572  s modified ensur
+00002150: 6520 7472 616e 736c 6174 696f 6e61 6c20  e translational 
+00002160: 696e 7661 7269 616e 6365 2222 220a 2020  invariance""".  
+00002170: 2020 2320 5573 6520 6120 7371 7274 2074    # Use a sqrt t
+00002180: 6861 7420 7265 7475 726e 7320 6120 636f  hat returns a co
+00002190: 6d70 6c65 7820 6e75 6d62 6572 0a20 2020  mplex number.   
+000021a0: 2023 2066 726f 6d20 6e75 6d70 792e 6c69   # from numpy.li
+000021b0: 622e 7363 696d 6174 6820 696d 706f 7274  b.scimath import
+000021c0: 2073 7172 740a 2020 2020 2320 4669 7273   sqrt.    # Firs
+000021d0: 7420 7374 6570 2069 7320 746f 2072 6563  t step is to rec
+000021e0: 6f6e 7374 7275 6374 2074 6865 2064 796e  onstruct the dyn
+000021f0: 616d 6963 616c 206d 6174 7269 7820 2844  amical matrix (D
+00002200: 2920 6672 6f6d 2074 6865 2066 7265 7175  ) from the frequ
+00002210: 656e 6369 6573 2061 6e64 2074 6865 2065  encies and the e
+00002220: 6967 656e 7665 6374 6f72 730a 2020 2020  igenvectors.    
+00002230: 2320 665e 3220 3d20 5554 202e 2044 202e  # f^2 = UT . D .
+00002240: 2055 0a20 2020 2023 2061 6e64 2055 2069   U.    # and U i
+00002250: 7320 6120 6865 726d 6974 6961 6e20 6d61  s a hermitian ma
+00002260: 7472 6978 2073 6f20 552d 3120 3d20 5554  trix so U-1 = UT
+00002270: 0a20 2020 2023 2044 203d 2028 5554 292d  .    # D = (UT)-
+00002280: 3120 665e 3220 552d 3120 3d20 5520 6620  1 f^2 U-1 = U f 
+00002290: 5554 0a20 2020 2023 2043 6f6e 7374 7275  UT.    # Constru
+000022a0: 6374 2055 5420 6672 6f6d 2074 6865 206e  ct UT from the n
+000022b0: 6f72 6d61 6c20 6d6f 6465 730a 2020 2020  ormal modes.    
+000022c0: 6e20 3d20 6e70 2e73 697a 6528 6e6f 726d  n = np.size(norm
+000022d0: 616c 5f6d 6f64 6573 2c20 3029 0a20 2020  al_modes, 0).   
+000022e0: 206d 203d 206e 702e 7369 7a65 286e 6f72   m = np.size(nor
+000022f0: 6d61 6c5f 6d6f 6465 732c 2031 292a 330a  mal_modes, 1)*3.
+00002300: 2020 2020 5554 203d 206e 702e 7a65 726f      UT = np.zero
+00002310: 7328 286e 2c20 6d29 290a 2020 2020 666f  s((n, m)).    fo
+00002320: 7220 696d 6f64 652c 206d 6f64 6520 696e  r imode, mode in
+00002330: 2065 6e75 6d65 7261 7465 286e 6f72 6d61   enumerate(norma
+00002340: 6c5f 6d6f 6465 7329 3a0a 2020 2020 2020  l_modes):.      
+00002350: 2020 6e20 3d20 300a 2020 2020 2020 2020    n = 0.        
+00002360: 666f 7220 6174 6f6d 2069 6e20 6d6f 6465  for atom in mode
+00002370: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00002380: 696e 2070 7974 686f 6e20 7468 6520 6669  in python the fi
+00002390: 7273 7420 696e 6465 7820 6973 2074 6865  rst index is the
+000023a0: 2072 6f77 206f 6620 7468 6520 6d61 7472   row of the matr
+000023b0: 6978 2c20 7468 6520 7365 636f 6e64 2069  ix, the second i
+000023c0: 7320 7468 6520 636f 6c75 6d6e 0a20 2020  s the column.   
+000023d0: 2020 2020 2020 2020 2055 545b 696d 6f64           UT[imod
+000023e0: 652c 206e 2b30 5d20 3d20 6174 6f6d 5b30  e, n+0] = atom[0
+000023f0: 5d0a 2020 2020 2020 2020 2020 2020 5554  ].            UT
+00002400: 5b69 6d6f 6465 2c20 6e2b 315d 203d 2061  [imode, n+1] = a
+00002410: 746f 6d5b 315d 0a20 2020 2020 2020 2020  tom[1].         
+00002420: 2020 2055 545b 696d 6f64 652c 206e 2b32     UT[imode, n+2
+00002430: 5d20 3d20 6174 6f6d 5b32 5d0a 2020 2020  ] = atom[2].    
+00002440: 2020 2020 2020 2020 6e20 3d20 6e20 2b20          n = n + 
+00002450: 330a 2020 2020 2020 2020 2320 656e 6420  3.        # end 
+00002460: 666f 7220 6174 6f6d 0a20 2020 2023 2065  for atom.    # e
+00002470: 6e64 2066 6f72 2069 6d6f 6465 0a20 2020  nd for imode.   
+00002480: 2023 207a 6572 6f20 7468 6520 6e6f 6e61   # zero the nona
+00002490: 6e61 6c79 7469 6361 6c20 636f 7272 6563  nalytical correc
+000024a0: 7469 6f6e 0a20 2020 2057 6d20 3d20 6e70  tion.    Wm = np
+000024b0: 2e7a 6572 6f73 2828 6e2c 206e 2929 0a20  .zeros((n, n)). 
+000024c0: 2020 2023 2063 6f6e 7665 7274 2074 6865     # convert the
+000024d0: 2066 7265 7175 656e 6369 6573 5e32 2074   frequencies^2 t
+000024e0: 6f20 6120 7265 616c 2064 6961 676f 6e61  o a real diagona
+000024f0: 6c20 6172 7261 790a 2020 2020 2320 5761  l array.    # Wa
+00002500: 726e 696e 6720 7765 2068 6176 6520 746f  rning we have to
+00002510: 206d 616b 6520 7375 7265 2074 6865 2073   make sure the s
+00002520: 6967 6e20 6973 2063 6f72 7265 6374 2068  ign is correct h
+00002530: 6572 650a 2020 2020 6632 203d 206e 702e  ere.    f2 = np.
+00002540: 6469 6167 286e 702e 7369 676e 2866 7265  diag(np.sign(fre
+00002550: 7175 656e 6369 6573 292a 6e70 2e72 6561  quencies)*np.rea
+00002560: 6c28 6672 6571 7565 6e63 6965 732a 6672  l(frequencies*fr
+00002570: 6571 7565 6e63 6965 7329 290a 2020 2020  equencies)).    
+00002580: 446d 203d 206e 702e 646f 7428 6e70 2e64  Dm = np.dot(np.d
+00002590: 6f74 2855 542e 542c 2066 3229 2c20 5554  ot(UT.T, f2), UT
+000025a0: 290a 2020 2020 2320 4d61 6b65 2073 7572  ).    # Make sur
+000025b0: 6520 7468 6520 6479 6e61 6d69 6361 6c20  e the dynamical 
+000025c0: 6d61 7472 6978 2069 7320 7265 616c 0a20  matrix is real. 
+000025d0: 2020 2044 6d20 3d20 6e70 2e72 6561 6c28     Dm = np.real(
+000025e0: 446d 290a 2020 2020 2320 4669 6e64 2069  Dm).    # Find i
+000025f0: 7473 2065 6967 656e 7661 6c75 6573 0a20  ts eigenvalues. 
+00002600: 2020 2065 6967 5f76 616c 2c20 6569 675f     eig_val, eig_
+00002610: 7665 6320 3d20 6e70 2e6c 696e 616c 672e  vec = np.linalg.
+00002620: 6569 6768 2844 6d29 0a20 2020 2023 2053  eigh(Dm).    # S
+00002630: 746f 7265 2074 6865 2072 6573 756c 7473  tore the results
+00002640: 2066 6f72 2072 6574 7572 6e69 6e67 2074   for returning t
+00002650: 6f20 7468 6520 6d61 696e 2070 726f 6772  o the main progr
+00002660: 616d 0a20 2020 2072 6573 756c 7473 203d  am.    results =
+00002670: 205b 5d0a 2020 2020 2320 4c6f 6f70 206f   [].    # Loop o
+00002680: 7665 7220 7120 7661 6c75 6573 0a20 2020  ver q values.   
+00002690: 2066 6f72 2071 2069 6e20 716c 6973 743a   for q in qlist:
+000026a0: 0a20 2020 2020 2020 2023 204e 6f77 2063  .        # Now c
+000026b0: 616c 6375 6c61 7465 2074 6865 206e 6f6e  alculate the non
+000026c0: 616e 616c 7974 6963 2070 6172 740a 2020  analytic part.  
+000026d0: 2020 2020 2020 636f 6e73 7461 6e74 203d        constant =
+000026e0: 2034 2e30 202a 2050 4920 2f20 286e 702e   4.0 * PI / (np.
+000026f0: 646f 7428 6e70 2e64 6f74 2871 2c20 6570  dot(np.dot(q, ep
+00002700: 7369 6c6f 6e5f 696e 6629 2c20 7129 202a  silon_inf), q) *
+00002710: 2076 6f6c 756d 6529 0a20 2020 2020 2020   volume).       
+00002720: 2023 204c 6f6f 7020 6f76 6572 2061 746f   # Loop over ato
+00002730: 6d20 610a 2020 2020 2020 2020 666f 7220  m a.        for 
+00002740: 612c 207a 6120 696e 2065 6e75 6d65 7261  a, za in enumera
+00002750: 7465 2862 6f72 6e5f 6368 6172 6765 7329  te(born_charges)
+00002760: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00002770: 6174 6f6d 2069 7320 7468 6520 6174 6f6d  atom is the atom
+00002780: 2069 6e64 6578 0a20 2020 2020 2020 2020   index.         
+00002790: 2020 2023 2062 6f72 6e20 636f 6e74 6169     # born contai
+000027a0: 6e73 2074 6865 2070 6f6c 6172 6973 6162  ns the polarisab
+000027b0: 696c 6974 7920 7465 6e73 6f72 205b 7a31  ility tensor [z1
+000027c0: 7820 7a31 7920 7a31 7a5d 205b 7a32 7820  x z1y z1z] [z2x 
+000027d0: 7a32 7920 7a32 7a5d 205b 7a33 7820 7a33  z2y z2z] [z3x z3
+000027e0: 7920 7a33 7a5d 5d0a 2020 2020 2020 2020  y z3z]].        
+000027f0: 2020 2020 2320 7768 6572 6520 312c 2032      # where 1, 2
+00002800: 2c20 3320 6172 6520 7468 6520 6469 7265  , 3 are the dire
+00002810: 6374 696f 6e73 206f 6620 7468 6520 6669  ctions of the fi
+00002820: 656c 6420 616e 6420 782c 2079 2c20 7a20  eld and x, y, z 
+00002830: 6172 6520 7468 6520 636f 6f72 6469 6e61  are the coordina
+00002840: 7465 7320 6f66 2074 6865 2061 746f 6d0a  tes of the atom.
+00002850: 2020 2020 2020 2020 2020 2020 7a61 203d              za =
+00002860: 206e 702e 646f 7428 712c 207a 6129 0a20   np.dot(q, za). 
+00002870: 2020 2020 2020 2020 2020 2023 204c 6f6f             # Loo
+00002880: 7020 6f76 6572 2061 746f 6d20 620a 2020  p over atom b.  
+00002890: 2020 2020 2020 2020 2020 666f 7220 622c            for b,
+000028a0: 207a 6220 696e 2065 6e75 6d65 7261 7465   zb in enumerate
+000028b0: 2862 6f72 6e5f 6368 6172 6765 7329 3a0a  (born_charges):.
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 7a62 203d 206e 702e 646f 7428 712c 207a  zb = np.dot(q, z
+000028e0: 6229 0a20 2020 2020 2020 2020 2020 2020  b).             
+000028f0: 2020 2074 6572 6d73 203d 206e 702e 6f75     terms = np.ou
+00002900: 7465 7228 7a61 2c20 7a62 2920 2a20 636f  ter(za, zb) * co
+00002910: 6e73 7461 6e74 202f 206d 6174 682e 7371  nstant / math.sq
+00002920: 7274 286d 6173 7365 735b 615d 2a6d 6173  rt(masses[a]*mas
+00002930: 7365 735b 625d 290a 2020 2020 2020 2020  ses[b]).        
+00002940: 2020 2020 2020 2020 6920 3d20 612a 330a          i = a*3.
+00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002960: 666f 7220 7465 726d 6920 696e 2074 6572  for termi in ter
+00002970: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00002980: 2020 2020 2020 2020 6a20 3d20 622a 330a          j = b*3.
+00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029a0: 2020 2020 666f 7220 7465 726d 2069 6e20      for term in 
+000029b0: 7465 726d 693a 0a20 2020 2020 2020 2020  termi:.         
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+000029d0: 6d5b 692c 206a 5d20 3d20 7465 726d 0a20  m[i, j] = term. 
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 2020 2020 206a 203d 206a 202b 2031         j = j + 1
+00002a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a10: 2020 2020 2023 2065 6e64 2066 6f72 2074       # end for t
+00002a20: 6572 6d0a 2020 2020 2020 2020 2020 2020  erm.            
+00002a30: 2020 2020 2020 2020 6920 3d20 6920 2b20          i = i + 
+00002a40: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00002a50: 2020 2320 656e 6420 666f 7220 690a 2020    # end for i.  
+00002a60: 2020 2020 2020 2020 2020 2320 656e 6420            # end 
+00002a70: 6c6f 6f70 206f 7665 7220 620a 2020 2020  loop over b.    
+00002a80: 2020 2020 2320 656e 6420 6c6f 6f70 206f      # end loop o
+00002a90: 7665 7220 610a 2020 2020 2020 2020 2320  ver a.        # 
+00002aa0: 436f 6e73 7472 7563 7420 7468 6520 6675  Construct the fu
+00002ab0: 6c6c 2064 796e 616d 6963 616c 206d 6174  ll dynamical mat
+00002ac0: 7269 7820 7769 7468 2074 6865 2063 6f72  rix with the cor
+00002ad0: 7265 6374 696f 6e0a 2020 2020 2020 2020  rection.        
+00002ae0: 446d 7120 3d20 446d 202b 2057 6d0a 2020  Dmq = Dm + Wm.  
+00002af0: 2020 2020 2020 2320 4966 2070 726f 6a65        # If proje
+00002b00: 6374 696f 6e20 7761 7320 7265 7175 6573  ction was reques
+00002b10: 7465 6420 7768 656e 2074 6865 206d 6174  ted when the mat
+00002b20: 7269 7820 7761 7320 7265 6164 2c20 7072  rix was read, pr
+00002b30: 6f6a 6563 7420 6f75 7420 7472 616e 736c  oject out transl
+00002b40: 6174 696f 6e0a 2020 2020 2020 2020 6966  ation.        if
+00002b50: 2072 6561 6465 722e 6563 6b61 7274 3a0a   reader.eckart:.
+00002b60: 2020 2020 2020 2020 2020 2020 7265 6164              read
+00002b70: 6572 2e70 726f 6a65 6374 2844 6d71 290a  er.project(Dmq).
+00002b80: 2020 2020 2020 2020 6569 675f 7661 6c2c          eig_val,
+00002b90: 2065 6967 5f76 6563 203d 206e 702e 6c69   eig_vec = np.li
+00002ba0: 6e61 6c67 2e65 6967 6828 446d 7129 0a20  nalg.eigh(Dmq). 
+00002bb0: 2020 2020 2020 2023 2049 6620 6569 675f         # If eig_
+00002bc0: 7661 6c20 6c65 7373 2074 6861 6e20 7a65  val less than ze
+00002bd0: 726f 2077 6520 7365 7420 6974 2074 6f20  ro we set it to 
+00002be0: 7a65 726f 0a20 2020 2020 2020 2076 616c  zero.        val
+00002bf0: 7565 7320 3d20 5b5d 0a20 2020 2020 2020  ues = [].       
+00002c00: 2066 6f72 2065 6967 2069 6e20 6569 675f   for eig in eig_
+00002c10: 7661 6c3a 0a20 2020 2020 2020 2020 2020  val:.           
+00002c20: 2069 6620 6569 6720 3e3d 2030 3a0a 2020   if eig >= 0:.  
+00002c30: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00002c40: 6c20 3d20 6d61 7468 2e73 7172 7428 6569  l = math.sqrt(ei
+00002c50: 6729 0a20 2020 2020 2020 2020 2020 2065  g).            e
+00002c60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00002c70: 2020 2020 2076 616c 203d 202d 6d61 7468       val = -math
+00002c80: 2e73 7172 7428 2d65 6967 290a 2020 2020  .sqrt(-eig).    
+00002c90: 2020 2020 2020 2020 7661 6c75 6573 2e61          values.a
+00002ca0: 7070 656e 6428 7661 6c29 0a20 2020 2020  ppend(val).     
+00002cb0: 2020 2023 2065 6e64 206f 6620 666f 7220     # end of for 
+00002cc0: 6569 670a 2020 2020 2020 2020 2320 536f  eig.        # So
+00002cd0: 7274 2074 6865 2065 6967 656e 2076 616c  rt the eigen val
+00002ce0: 7565 7320 696e 2061 7363 656e 6469 6e67  ues in ascending
+00002cf0: 206f 7264 6572 2061 6e64 2061 7070 656e   order and appen
+00002d00: 6420 746f 2074 6865 2072 6573 756c 7473  d to the results
+00002d10: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00002d20: 2e61 7070 656e 6428 6e70 2e73 6f72 7428  .append(np.sort(
+00002d30: 7661 6c75 6573 2929 0a20 2020 2023 2065  values)).    # e
+00002d40: 6e64 206c 6f6f 7020 6f76 6572 2071 0a20  nd loop over q. 
+00002d50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00002d60: 730a 0a64 6566 206f 7363 696c 6c61 746f  s..def oscillato
+00002d70: 725f 7374 7265 6e67 7468 7328 6e6f 726d  r_strengths(norm
+00002d80: 616c 5f6d 6f64 6573 2c20 626f 726e 5f63  al_modes, born_c
+00002d90: 6861 7267 6573 293a 0a20 2020 2022 2222  harges):.    """
+00002da0: 4361 6c63 756c 6174 6520 6f73 6369 6c6c  Calculate oscill
+00002db0: 6174 6f72 2073 7472 656e 6774 6873 2066  ator strengths f
+00002dc0: 726f 6d20 7468 6520 6e6f 726d 616c 206d  rom the normal m
+00002dd0: 6f64 6573 2061 6e64 2074 6865 2062 6f72  odes and the bor
+00002de0: 6e20 6368 6172 6765 730a 2020 2020 2020  n charges.      
+00002df0: 206e 6f72 6d61 6c5f 6d6f 6465 7320 6172   normal_modes ar
+00002e00: 6520 696e 2074 6865 206d 6173 7320 7765  e in the mass we
+00002e10: 6967 6874 6564 2063 6f6f 7264 696e 6174  ighted coordinat
+00002e20: 6520 7379 7374 656d 2061 6e64 206e 6f72  e system and nor
+00002e30: 6d61 6c69 7365 640a 2020 2020 2020 2062  malised.       b
+00002e40: 6f72 6e20 6368 6172 6765 7320 6172 6520  orn charges are 
+00002e50: 696e 2065 6c65 6374 726f 6e73 2c20 736f  in electrons, so
+00002e60: 2061 746f 6d69 6320 756e 6974 7322 2222   atomic units"""
+00002e70: 0a20 2020 2023 2045 6163 6820 6d6f 6465  .    # Each mode
+00002e80: 2068 6173 2061 2033 7833 206f 7363 696c   has a 3x3 oscil
+00002e90: 6c61 746f 7220 7374 7265 6e67 7468 0a20  lator strength. 
+00002ea0: 2020 206e 6d6f 6465 7320 3d20 6e70 2e73     nmodes = np.s
+00002eb0: 697a 6528 6e6f 726d 616c 5f6d 6f64 6573  ize(normal_modes
+00002ec0: 2c20 3029 0a20 2020 206f 7363 696c 6c61  , 0).    oscilla
+00002ed0: 746f 725f 7374 7265 6e67 7468 7320 3d20  tor_strengths = 
+00002ee0: 6e70 2e7a 6572 6f73 2828 6e6d 6f64 6573  np.zeros((nmodes
+00002ef0: 2c20 332c 2033 2929 0a20 2020 2066 6f72  , 3, 3)).    for
+00002f00: 2069 6d6f 6465 2c20 6d6f 6465 2069 6e20   imode, mode in 
+00002f10: 656e 756d 6572 6174 6528 6e6f 726d 616c  enumerate(normal
+00002f20: 5f6d 6f64 6573 293a 0a20 2020 2020 2020  _modes):.       
+00002f30: 2023 2057 6520 6361 6c63 756c 6174 6520   # We calculate 
+00002f40: 7468 6520 6469 706f 6c65 2069 6e64 7563  the dipole induc
+00002f50: 6564 2062 7920 6469 7370 6c61 6365 6d65  ed by displaceme
+00002f60: 6e74 206f 6620 6561 6368 2061 746f 6d20  nt of each atom 
+00002f70: 616c 6f6e 6720 7468 6520 6e6f 726d 616c  along the normal
+00002f80: 206d 6f64 650a 2020 2020 2020 2020 7a5f   mode.        z_
+00002f90: 696d 6f64 6520 3d20 6e70 2e7a 6572 6f73  imode = np.zeros
+00002fa0: 2833 290a 2020 2020 2020 2020 666f 7220  (3).        for 
+00002fb0: 6174 6f6d 2c20 626f 726e 2069 6e20 656e  atom, born in en
+00002fc0: 756d 6572 6174 6528 626f 726e 5f63 6861  umerate(born_cha
+00002fd0: 7267 6573 293a 0a20 2020 2020 2020 2020  rges):.         
+00002fe0: 2020 2023 2061 746f 6d20 6973 2074 6865     # atom is the
+00002ff0: 2061 746f 6d20 696e 6465 780a 2020 2020   atom index.    
+00003000: 2020 2020 2020 2020 2320 626f 726e 2063          # born c
+00003010: 6f6e 7461 696e 7320 7468 6520 706f 6c61  ontains the pola
+00003020: 7269 7361 6269 6c69 7479 2074 656e 736f  risability tenso
+00003030: 7220 5b61 3178 2061 3179 2061 317a 5d20  r [a1x a1y a1z] 
+00003040: 5b61 3278 2061 3279 2061 327a 5d20 5b61  [a2x a2y a2z] [a
+00003050: 3378 2061 3379 2061 337a 5d5d 0a20 2020  3x a3y a3z]].   
+00003060: 2020 2020 2020 2020 2023 2077 6865 7265           # where
+00003070: 2031 2c20 322c 2033 2061 7265 2074 6865   1, 2, 3 are the
+00003080: 2064 6972 6563 7469 6f6e 7320 6f66 2074   directions of t
+00003090: 6865 2066 6965 6c64 2061 6e64 2078 2c20  he field and x, 
+000030a0: 792c 207a 2061 7265 2074 6865 2063 6f6f  y, z are the coo
+000030b0: 7264 696e 6174 6573 206f 6620 7468 6520  rdinates of the 
+000030c0: 6174 6f6d 0a20 2020 2020 2020 2020 2020  atom.           
+000030d0: 207a 5f69 6d6f 6465 203d 207a 5f69 6d6f   z_imode = z_imo
+000030e0: 6465 202b 206e 702e 646f 7428 626f 726e  de + np.dot(born
+000030f0: 2c20 6d6f 6465 5b61 746f 6d5d 2920 2023  , mode[atom])  #
+00003100: 2074 6865 2064 6973 706c 6163 656d 656e   the displacemen
+00003110: 7420 6973 2061 6e20 6172 7261 7920 5b78  t is an array [x
+00003120: 2c20 792c 207a 5d0a 2020 2020 2020 2020  , y, z].        
+00003130: 2320 656e 6420 666f 720a 2020 2020 2020  # end for.      
+00003140: 2020 2320 5468 6520 6f73 6369 6c6c 6174    # The oscillat
+00003150: 6f72 2073 7472 656e 6774 6820 6d61 7472  or strength matr
+00003160: 6978 2069 7320 7468 6520 6f75 7465 7220  ix is the outer 
+00003170: 7072 6f64 7563 7420 6f66 207a 0a20 2020  product of z.   
+00003180: 2020 2020 206f 7363 696c 6c61 746f 725f       oscillator_
+00003190: 7374 7265 6e67 7468 735b 696d 6f64 655d  strengths[imode]
+000031a0: 203d 206e 702e 6f75 7465 7228 7a5f 696d   = np.outer(z_im
+000031b0: 6f64 652c 207a 5f69 6d6f 6465 290a 2020  ode, z_imode).  
+000031c0: 2020 2320 656e 6420 666f 720a 2020 2020    # end for.    
+000031d0: 7265 7475 726e 206f 7363 696c 6c61 746f  return oscillato
+000031e0: 725f 7374 7265 6e67 7468 730a 0a64 6566  r_strengths..def
+000031f0: 206e 6f72 6d61 6c5f 6d6f 6465 7328 6d61   normal_modes(ma
+00003200: 7373 6573 2c20 6d61 7373 5f77 6569 6768  sses, mass_weigh
+00003210: 7465 645f 6e6f 726d 616c 5f6d 6f64 6573  ted_normal_modes
+00003220: 293a 0a20 2020 2022 2222 2054 7261 6e73  ):.    """ Trans
+00003230: 666f 726d 2066 726f 6d20 6d61 7373 2077  form from mass w
+00003240: 6569 6768 7465 6420 636f 6f72 6469 6e61  eighted coordina
+00003250: 7465 7320 746f 2078 797a 2e20 4e6f 7465  tes to xyz. Note
+00003260: 2074 6869 7320 7265 7475 726e 7320 616e   this returns an
+00003270: 2061 7272 6179 206f 626a 6563 742e 0a20   array object.. 
+00003280: 2020 2020 2020 2054 6865 2072 6574 7572         The retur
+00003290: 6e65 6420 6e6f 726d 616c 206d 6f64 6573  ned normal modes
+000032a0: 2068 6176 6520 4e4f 5420 6265 656e 2072   have NOT been r
+000032b0: 656e 6f72 6d61 6c69 7365 642e 0a20 2020  enormalised..   
+000032c0: 2020 2020 2054 6865 2069 6e70 7574 206d       The input m
+000032d0: 6173 7365 7320 6172 6520 696e 2061 746f  asses are in ato
+000032e0: 6d69 6320 756e 6974 730a 2020 2020 2020  mic units.      
+000032f0: 2020 7468 6520 6f75 7470 7574 206e 6f72    the output nor
+00003300: 6d61 6c20 6d6f 6465 7320 6172 6520 696e  mal modes are in
+00003310: 2061 746f 6d69 6320 756e 6974 7320 2222   atomic units ""
+00003320: 220a 2020 2020 6c69 7374 5f6d 203d 205b  ".    list_m = [
+00003330: 5d0a 2020 2020 6e6f 726d 616c 5f6d 6f64  ].    normal_mod
+00003340: 6573 203d 206e 702e 7a65 726f 735f 6c69  es = np.zeros_li
+00003350: 6b65 286d 6173 735f 7765 6967 6874 6564  ke(mass_weighted
+00003360: 5f6e 6f72 6d61 6c5f 6d6f 6465 7329 0a20  _normal_modes). 
+00003370: 2020 206e 696f 6e73 203d 206e 702e 7369     nions = np.si
+00003380: 7a65 286d 6173 7365 7329 0a20 2020 2066  ze(masses).    f
+00003390: 6f72 2061 2069 6e20 7261 6e67 6528 6e69  or a in range(ni
+000033a0: 6f6e 7329 3a0a 2020 2020 2020 2020 7820  ons):.        x 
+000033b0: 3d20 312e 3020 2f20 6d61 7468 2e73 7172  = 1.0 / math.sqr
+000033c0: 7428 6d61 7373 6573 5b61 5d29 0a20 2020  t(masses[a]).   
+000033d0: 2020 2020 2061 746f 6d20 3d20 5b78 2c20       atom = [x, 
+000033e0: 782c 2078 5d0a 2020 2020 2020 2020 6c69  x, x].        li
+000033f0: 7374 5f6d 2e61 7070 656e 6428 6174 6f6d  st_m.append(atom
+00003400: 290a 2020 2020 2320 656e 6420 6f66 206c  ).    # end of l
+00003410: 6f6f 7020 6f66 2069 6f6e 730a 2020 2020  oop of ions.    
+00003420: 6172 7261 795f 6d20 3d20 6e70 2e61 7272  array_m = np.arr
+00003430: 6179 286c 6973 745f 6d29 0a20 2020 2066  ay(list_m).    f
+00003440: 6f72 2069 6e64 6578 2c20 6d6f 6465 2069  or index, mode i
+00003450: 6e20 656e 756d 6572 6174 6528 6d61 7373  n enumerate(mass
+00003460: 5f77 6569 6768 7465 645f 6e6f 726d 616c  _weighted_normal
+00003470: 5f6d 6f64 6573 293a 0a20 2020 2020 2020  _modes):.       
+00003480: 206e 6f72 6d61 6c5f 6d6f 6465 735b 696e   normal_modes[in
+00003490: 6465 785d 203d 206d 6f64 6520 2a20 6172  dex] = mode * ar
+000034a0: 7261 795f 6d0a 2020 2020 7265 7475 726e  ray_m.    return
+000034b0: 206e 6f72 6d61 6c5f 6d6f 6465 730a 0a64   normal_modes..d
+000034c0: 6566 2070 726f 6a65 6374 5f66 6965 6c64  ef project_field
+000034d0: 2873 6861 7065 2c20 7368 6170 655f 6461  (shape, shape_da
+000034e0: 7461 2c20 7072 6f6a 6563 7469 6f6e 2c20  ta, projection, 
+000034f0: 6566 6965 6c64 293a 0a20 2020 2022 2222  efield):.    """
+00003500: 5461 6b65 2074 6865 2066 6965 6c64 2064  Take the field d
+00003510: 6972 6563 7469 6f6e 7320 696e 2065 6669  irections in efi
+00003520: 656c 6420 616e 6420 6170 706c 7920 7368  eld and apply sh
+00003530: 6170 6520 7072 6f6a 6563 7469 6f6e 2e22  ape projection."
+00003540: 2222 0a20 2020 2069 6620 7072 6f6a 6563  "".    if projec
+00003550: 7469 6f6e 203d 3d20 2272 616e 646f 6d22  tion == "random"
+00003560: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00003570: 206e 702e 6172 7261 7928 6566 6965 6c64   np.array(efield
+00003580: 290a 2020 2020 656c 6966 2070 726f 6a65  ).    elif proje
+00003590: 6374 696f 6e20 3d3d 2022 7061 7261 6c6c  ction == "parall
+000035a0: 656c 223a 0a20 2020 2020 2020 2069 6620  el":.        if 
+000035b0: 7368 6170 6520 3d3d 2022 7370 6865 7265  shape == "sphere
+000035c0: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
+000035d0: 6574 7572 6e20 6e70 2e61 7272 6179 2865  eturn np.array(e
+000035e0: 6669 656c 6429 0a20 2020 2020 2020 2065  field).        e
+000035f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003600: 2072 6574 7572 6e20 6e70 2e61 7272 6179   return np.array
+00003610: 2873 6861 7065 5f64 6174 6129 0a20 2020  (shape_data).   
+00003620: 2065 6c69 6620 7072 6f6a 6563 7469 6f6e   elif projection
+00003630: 203d 3d20 2270 6572 7065 6e64 6963 756c   == "perpendicul
+00003640: 6172 223a 0a20 2020 2020 2020 2069 6620  ar":.        if 
+00003650: 7368 6170 6520 3d3d 2022 7370 6865 7265  shape == "sphere
+00003660: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
+00003670: 6574 7572 6e20 6e70 2e61 7272 6179 2865  eturn np.array(e
+00003680: 6669 656c 6429 0a20 2020 2020 2020 2065  field).        e
+00003690: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000036a0: 2070 726f 6a5f 6669 656c 6420 3d20 5b5d   proj_field = []
+000036b0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000036c0: 6120 3d20 6e70 2e61 7272 6179 2873 6861  a = np.array(sha
+000036d0: 7065 5f64 6174 6129 0a20 2020 2020 2020  pe_data).       
+000036e0: 2020 2020 2066 6f72 2066 6965 6c64 2069       for field i
+000036f0: 6e20 6566 6965 6c64 3a0a 2020 2020 2020  n efield:.      
+00003700: 2020 2020 2020 2020 2020 7072 6f6a 203d            proj =
+00003710: 2066 6965 6c64 202d 2028 6e70 2e64 6f74   field - (np.dot
+00003720: 2864 6174 612c 2066 6965 6c64 2920 2a20  (data, field) * 
+00003730: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+00003740: 2020 2020 2020 7369 7a65 203d 206e 702e        size = np.
+00003750: 6c69 6e61 6c67 2e6e 6f72 6d28 7072 6f6a  linalg.norm(proj
+00003760: 5f66 6965 6c64 290a 2020 2020 2020 2020  _field).        
+00003770: 2020 2020 2020 2020 6966 2073 697a 6520          if size 
+00003780: 3e20 302e 3030 3031 3a0a 2020 2020 2020  > 0.0001:.      
+00003790: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000037a0: 6f6a 5f66 6965 6c64 2e61 7070 656e 6428  oj_field.append(
+000037b0: 7072 6f6a 290a 2020 2020 2020 2020 2020  proj).          
+000037c0: 2020 2020 2020 2320 656e 6420 6966 0a20        # end if. 
+000037d0: 2020 2020 2020 2020 2020 2023 2065 6e64             # end
+000037e0: 2066 6f72 0a20 2020 2020 2020 2020 2020   for.           
+000037f0: 2072 6574 7572 6e20 6e70 2e61 7272 6179   return np.array
+00003800: 2870 726f 6a5f 6669 656c 6429 0a20 2020  (proj_field).   
+00003810: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
+00003820: 7269 6e74 2822 4572 726f 7220 696e 2070  rint("Error in p
+00003830: 726f 6a65 6374 5f66 6965 6c64 2c20 7072  roject_field, pr
+00003840: 6f6a 6563 7469 6f6e 2075 6e6b 6f77 6e3a  ojection unkown:
+00003850: 2022 2c20 7072 6f6a 6563 7469 6f6e 2c20   ", projection, 
+00003860: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
+00003870: 0a20 2020 2020 2020 2065 7869 7428 3129  .        exit(1)
+00003880: 0a20 2020 2072 6574 7572 6e0a 0a64 6566  .    return..def
+00003890: 2072 6f67 7269 6467 7565 735f 726f 7461   rogridgues_rota
+000038a0: 7469 6f6e 7328 6566 6965 6c64 293a 0a20  tions(efield):. 
+000038b0: 2020 2022 2222 5461 6b65 2074 6865 2066     """Take the f
+000038c0: 6965 6c64 2064 6972 6563 7469 6f6e 7320  ield directions 
+000038d0: 696e 2065 6669 656c 6420 616e 6420 7573  in efield and us
+000038e0: 6520 6561 6368 2064 6972 6563 7469 6f6e  e each direction
+000038f0: 2074 6f20 6361 6c63 756c 6174 6520 6120   to calculate a 
+00003900: 7261 6e64 6f6d 2072 6f74 6174 696f 6e20  random rotation 
+00003910: 6162 6f75 7420 7468 6174 2061 7869 732e  about that axis.
+00003920: 0a20 2020 2020 2020 5573 6520 7468 6520  .       Use the 
+00003930: 6669 656c 6420 2877 6869 6368 2061 2072  field (which a r
+00003940: 616e 646f 6d20 756e 6974 2076 6563 746f  andom unit vecto
+00003950: 7220 696e 2078 797a 2073 7061 6365 2920  r in xyz space) 
+00003960: 746f 2067 656e 6572 6174 6520 616e 206f  to generate an o
+00003970: 7274 686f 676f 6e61 6c20 726f 7461 7469  rthogonal rotati
+00003980: 6f6e 206d 6174 7269 780a 2020 2020 2020  on matrix.      
+00003990: 2052 6f64 7269 6775 6573 2072 6f74 6174   Rodrigues rotat
+000039a0: 696f 6e20 666f 726d 756c 6120 4120 3d20  ion formula A = 
+000039b0: 4933 2e20 636f 7328 7468 6574 6129 202b  I3. cos(theta) +
+000039c0: 2028 312d 636f 7328 7468 6574 6129 2920   (1-cos(theta)) 
+000039d0: 6520 2e20 6554 202b 2065 7820 7369 6e28  e . eT + ex sin(
+000039e0: 7468 6574 6130 0a20 2020 2020 2020 4933  theta0.       I3
+000039f0: 2069 7320 6120 756e 6974 206d 6174 7269   is a unit matri
+00003a00: 780a 2020 2020 2020 2065 2069 7320 7468  x.       e is th
+00003a10: 6520 6469 7265 6374 696f 6e0a 2020 2020  e direction.    
+00003a20: 2020 2065 7820 6973 2074 6865 2063 726f     ex is the cro
+00003a30: 7373 2070 726f 6475 6374 206d 6174 7269  ss product matri
+00003a40: 780a 2020 2020 2020 2028 2030 2020 2d65  x.       ( 0  -e
+00003a50: 3320 2020 6532 290a 2020 2020 2020 2028  3   e2).       (
+00003a60: 2065 3320 2030 2020 202d 6531 290a 2020   e3  0   -e1).  
+00003a70: 2020 2020 2028 2d65 3220 2065 3120 2020       (-e2  e1   
+00003a80: 3020 290a 2020 2020 2020 2049 6e70 7574  0 ).       Input
+00003a90: 2066 6965 6c64 2069 7320 7265 616c 0a20   field is real. 
+00003aa0: 2020 2020 2020 4f75 7470 7574 2069 7320        Output is 
+00003ab0: 6120 6c69 7374 206f 6620 726f 7461 7469  a list of rotati
+00003ac0: 6f6e 730a 2020 2020 2222 220a 2020 2020  ons.    """.    
+00003ad0: 726f 7461 7469 6f6e 7320 3d20 5b5d 0a20  rotations = []. 
+00003ae0: 2020 2066 6f72 2066 6965 6c64 2069 6e20     for field in 
+00003af0: 6566 6965 6c64 3a0a 2020 2020 2020 2020  efield:.        
+00003b00: 2320 4361 6c63 756c 6174 6520 6120 7261  # Calculate a ra
+00003b10: 6e64 6f6d 2061 6e67 6c65 2062 6574 7765  ndom angle betwe
+00003b20: 656e 2030 2061 6e64 2031 3830 0a20 2020  en 0 and 180.   
+00003b30: 2020 2020 2074 6865 7461 203d 2050 492a       theta = PI*
+00003b40: 6e70 2e72 616e 646f 6d2e 7261 6e64 2829  np.random.rand()
+00003b50: 0a20 2020 2020 2020 2063 6f73 2020 203d  .        cos   =
+00003b60: 206e 702e 636f 7328 7468 6574 6129 0a20   np.cos(theta). 
+00003b70: 2020 2020 2020 2073 696e 2020 203d 206e         sin   = n
+00003b80: 702e 7369 6e28 7468 6574 6129 0a20 2020  p.sin(theta).   
+00003b90: 2020 2020 2072 6f74 6174 696f 6e20 3d20       rotation = 
+00003ba0: 6e70 2e7a 6572 6f73 2828 332c 2033 2929  np.zeros((3, 3))
+00003bb0: 0a20 2020 2020 2020 2065 3120 3d20 6669  .        e1 = fi
+00003bc0: 656c 645b 305d 0a20 2020 2020 2020 2065  eld[0].        e
+00003bd0: 3220 3d20 6669 656c 645b 315d 0a20 2020  2 = field[1].   
+00003be0: 2020 2020 2065 3320 3d20 6669 656c 645b       e3 = field[
+00003bf0: 325d 0a20 2020 2020 2020 2072 6f74 6174  2].        rotat
+00003c00: 696f 6e5b 302c 2030 5d20 3d20 636f 7320  ion[0, 0] = cos 
+00003c10: 2b20 2831 2d63 6f73 292a 6531 2a65 310a  + (1-cos)*e1*e1.
+00003c20: 2020 2020 2020 2020 726f 7461 7469 6f6e          rotation
+00003c30: 5b30 2c20 315d 203d 2028 312d 636f 7329  [0, 1] = (1-cos)
+00003c40: 2a65 322a 6531 202b 2073 696e 2a65 330a  *e2*e1 + sin*e3.
+00003c50: 2020 2020 2020 2020 726f 7461 7469 6f6e          rotation
+00003c60: 5b30 2c20 325d 203d 2028 312d 636f 7329  [0, 2] = (1-cos)
+00003c70: 2a65 332a 6531 202d 2073 696e 2a65 320a  *e3*e1 - sin*e2.
+00003c80: 2020 2020 2020 2020 726f 7461 7469 6f6e          rotation
+00003c90: 5b31 2c20 305d 203d 2028 312d 636f 7329  [1, 0] = (1-cos)
+00003ca0: 2a65 312a 6532 202d 2073 696e 2a65 330a  *e1*e2 - sin*e3.
+00003cb0: 2020 2020 2020 2020 726f 7461 7469 6f6e          rotation
+00003cc0: 5b31 2c20 315d 203d 2063 6f73 202b 2028  [1, 1] = cos + (
+00003cd0: 312d 636f 7329 2a65 322a 6532 0a20 2020  1-cos)*e2*e2.   
+00003ce0: 2020 2020 2072 6f74 6174 696f 6e5b 312c       rotation[1,
+00003cf0: 2032 5d20 3d20 2831 2d63 6f73 292a 6533   2] = (1-cos)*e3
+00003d00: 2a65 3220 2b20 7369 6e2a 6531 0a20 2020  *e2 + sin*e1.   
+00003d10: 2020 2020 2072 6f74 6174 696f 6e5b 322c       rotation[2,
+00003d20: 2030 5d20 3d20 2831 2d63 6f73 292a 6531   0] = (1-cos)*e1
+00003d30: 2a65 3320 2b20 7369 6e2a 6532 0a20 2020  *e3 + sin*e2.   
+00003d40: 2020 2020 2072 6f74 6174 696f 6e5b 322c       rotation[2,
+00003d50: 2031 5d20 3d20 2831 2d63 6f73 292a 6532   1] = (1-cos)*e2
+00003d60: 2a65 3320 2d20 7369 6e2a 6531 0a20 2020  *e3 - sin*e1.   
+00003d70: 2020 2020 2072 6f74 6174 696f 6e5b 322c       rotation[2,
+00003d80: 2032 5d20 3d20 636f 7320 2b20 2831 2d63   2] = cos + (1-c
+00003d90: 6f73 292a 6533 2a65 330a 2020 2020 2020  os)*e3*e3.      
+00003da0: 2020 726f 7461 7469 6f6e 732e 6170 7065    rotations.appe
+00003db0: 6e64 2872 6f74 6174 696f 6e29 0a20 2020  nd(rotation).   
+00003dc0: 2072 6574 7572 6e20 726f 7461 7469 6f6e   return rotation
+00003dd0: 730a 0a64 6566 2061 6273 6f72 7074 696f  s..def absorptio
+00003de0: 6e5f 6672 6f6d 5f6d 6f64 655f 696e 7465  n_from_mode_inte
+00003df0: 6e73 6974 6965 7328 662c 206d 6f64 6573  nsities(f, modes
+00003e00: 2c20 6672 6571 7565 6e63 6965 732c 2073  , frequencies, s
+00003e10: 6967 6d61 732c 2069 6e74 656e 7369 7469  igmas, intensiti
+00003e20: 6573 293a 0a20 2020 2022 2222 4361 6c63  es):.    """Calc
+00003e30: 756c 6174 6520 7468 6520 6162 736f 7270  ulate the absorp
+00003e40: 7469 6f6e 2066 726f 6d20 7468 6520 6672  tion from the fr
+00003e50: 6571 7565 6e63 6965 7320 616e 6420 696e  equencies and in
+00003e60: 7465 6e73 6974 6965 7320 7573 696e 6720  tensities using 
+00003e70: 6120 4c6f 7265 6e74 7a69 616e 0a20 2020  a Lorentzian.   
+00003e80: 2020 2020 6620 6973 2074 6865 2066 7265      f is the fre
+00003e90: 7175 656e 6379 206f 6620 7468 6520 6162  quency of the ab
+00003ea0: 736f 7270 7469 6f6e 2069 6e20 636d 2d31  sorption in cm-1
+00003eb0: 0a20 2020 2020 2020 6d6f 6465 7320 6172  .       modes ar
+00003ec0: 6520 6120 6c69 7374 206f 6620 7468 6520  e a list of the 
+00003ed0: 6d6f 6465 730a 2020 2020 2020 2066 7265  modes.       fre
+00003ee0: 7175 656e 6369 6573 2863 6d2d 3129 2c20  quencies(cm-1), 
+00003ef0: 7369 676d 6173 2863 6d2d 3129 2061 6e64  sigmas(cm-1) and
+00003f00: 2069 6e74 656e 7369 7469 6573 2028 4432   intensities (D2
+00003f10: 2f41 322f 616d 7529 0a20 2020 2020 2020  /A2/amu).       
+00003f20: 5468 6520 6e75 6d62 6572 2034 3232 352e  The number 4225.
+00003f30: 3620 636f 6e76 6572 7473 2074 6865 2075  6 converts the u
+00003f40: 6e69 7473 206f 6620 4432 2f41 322f 616d  nits of D2/A2/am
+00003f50: 7520 746f 204c 206d 6f6c 652d 3120 636d  u to L mole-1 cm
+00003f60: 2d31 2063 6d2d 310a 2020 2020 2020 2054  -1 cm-1.       T
+00003f70: 6865 206f 7574 7075 7420 6672 6f6d 2074  he output from t
+00003f80: 6869 7320 6973 2074 6865 206d 6f6c 6172  his is the molar
+00003f90: 2061 6273 6f72 7074 696f 6e20 636f 6566   absorption coef
+00003fa0: 6669 6369 656e 7420 6174 2066 2c20 696e  ficient at f, in
+00003fb0: 204c 2f6d 6f6c 2f63 6d22 2222 0a20 2020   L/mol/cm""".   
+00003fc0: 2061 6273 6f72 7074 696f 6e20 3d20 302e   absorption = 0.
+00003fd0: 300a 2020 2020 666f 7220 6d6f 6465 2069  0.    for mode i
+00003fe0: 6e20 6d6f 6465 733a 0a20 2020 2020 2020  n modes:.       
+00003ff0: 2076 203d 206e 702e 7265 616c 2866 7265   v = np.real(fre
+00004000: 7175 656e 6369 6573 5b6d 6f64 655d 290a  quencies[mode]).
+00004010: 2020 2020 2020 2020 7369 676d 6120 3d20          sigma = 
+00004020: 7369 676d 6173 5b6d 6f64 655d 0a20 2020  sigmas[mode].   
+00004030: 2020 2020 2069 6361 7374 6570 203d 2069       icastep = i
+00004040: 6e74 656e 7369 7469 6573 5b6d 6f64 655d  ntensities[mode]
+00004050: 0a20 2020 2020 2020 2061 6273 6f72 7074  .        absorpt
+00004060: 696f 6e20 3d20 6162 736f 7270 7469 6f6e  ion = absorption
+00004070: 202b 2032 2e30 202a 2034 3232 352e 3620   + 2.0 * 4225.6 
+00004080: 2a20 6963 6173 7465 7020 2f20 5049 202a  * icastep / PI *
+00004090: 2028 7369 676d 6120 2f20 2834 2e30 202a   (sigma / (4.0 *
+000040a0: 2028 6620 2d20 7629 2a28 6620 2d20 7629   (f - v)*(f - v)
+000040b0: 202b 2073 6967 6d61 2a73 6967 6d61 2929   + sigma*sigma))
+000040c0: 0a20 2020 2072 6574 7572 6e20 6162 736f  .    return abso
+000040d0: 7270 7469 6f6e 0a0a 6465 6620 6361 6c63  rption..def calc
+000040e0: 756c 6174 655f 7369 7a65 5f66 6163 746f  ulate_size_facto
+000040f0: 7220 2878 293a 0a20 2020 2022 2222 0a20  r (x):.    """. 
+00004100: 2020 2043 616c 6375 6c61 7465 2061 2073     Calculate a s
+00004110: 697a 6520 6566 6665 6374 2075 7369 6e67  ize effect using
+00004120: 2045 7175 6174 696f 6e73 2031 302e 3338   Equations 10.38
+00004130: 2061 6e64 2031 302e 3339 2069 6e20 5369   and 10.39 in Si
+00004140: 6876 6f6c 610a 2020 2020 2222 220a 2020  hvola.    """.  
+00004150: 2020 6966 2078 203c 2031 2e30 452d 3132    if x < 1.0E-12
+00004160: 3a0a 2020 2020 2020 2020 7265 7375 6c74  :.        result
+00004170: 203d 2031 2e30 0a20 2020 2065 6c73 653a   = 1.0.    else:
+00004180: 0a20 2020 2020 2020 2069 7820 3d20 636f  .        ix = co
+00004190: 6d70 6c65 7828 302c 7829 0a20 2020 2020  mplex(0,x).     
+000041a0: 2020 2067 3120 3d20 322e 3020 2f20 332e     g1 = 2.0 / 3.
+000041b0: 3020 2a20 2820 2820 312e 3020 2b20 6978  0 * ( ( 1.0 + ix
+000041c0: 2029 202a 206e 702e 6578 7028 2d69 7829   ) * np.exp(-ix)
+000041d0: 202d 2031 2e30 2029 0a20 2020 2020 2020   - 1.0 ).       
+000041e0: 2067 3220 3d20 2820 3120 2b20 6978 202d   g2 = ( 1 + ix -
+000041f0: 2028 372e 302f 3135 2e30 2920 2a20 782a   (7.0/15.0) * x*
+00004200: 7820 2d20 636f 6d70 6c65 7828 302c 322e  x - complex(0,2.
+00004210: 302a 782a 782a 782f 3135 2e30 2920 2920  0*x*x*x/15.0) ) 
+00004220: 2a20 6e70 2e65 7870 282d 6978 2920 2d31  * np.exp(-ix) -1
+00004230: 2e30 0a20 2020 2020 2020 2072 6573 756c  .0.        resul
+00004240: 7420 3d20 3120 2d20 6731 202d 2067 320a  t = 1 - g1 - g2.
+00004250: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00004260: 740a 0a64 6566 2061 7665 7261 6765 645f  t..def averaged_
+00004270: 7065 726d 6974 7469 7669 7479 2864 6965  permittivity(die
+00004280: 6c65 6374 7269 635f 6d65 6469 756d 2c20  lectric_medium, 
+00004290: 6372 7973 7461 6c5f 7065 726d 6974 7469  crystal_permitti
+000042a0: 7669 7479 2c20 7368 6170 652c 204c 2c20  vity, shape, L, 
+000042b0: 7666 2c20 7369 7a65 293a 0a20 2020 2022  vf, size):.    "
+000042c0: 2222 4361 6c63 756c 6174 6520 7468 6520  ""Calculate the 
+000042d0: 6566 6665 6374 6976 6520 636f 6e73 7461  effective consta
+000042e0: 6e74 2070 6572 6d69 7474 6976 6974 7920  nt permittivity 
+000042f0: 7573 696e 6720 7468 6520 6176 6572 6167  using the averag
+00004300: 6564 2070 6572 6d69 7474 6976 6974 7920  ed permittivity 
+00004310: 6d65 7468 6f64 0a20 2020 2020 2020 6469  method.       di
+00004320: 656c 6563 7472 6963 5f6d 6564 6975 6d20  electric_medium 
+00004330: 6973 2074 6865 2064 6965 6c65 6374 7269  is the dielectri
+00004340: 6320 636f 6e73 7461 6e74 2074 656e 736f  c constant tenso
+00004350: 7220 6f66 2074 6865 206d 6564 6975 6d0a  r of the medium.
+00004360: 2020 2020 2020 2063 7279 7374 616c 5f70         crystal_p
+00004370: 6572 6d69 7474 6976 6974 7920 6973 2074  ermittivity is t
+00004380: 6865 2074 6f74 616c 2066 7265 7175 656e  he total frequen
+00004390: 6379 2064 6965 6c65 6374 7269 6320 636f  cy dielectric co
+000043a0: 6e73 7461 6e74 2074 656e 736f 7220 6174  nstant tensor at
+000043b0: 2074 6865 2063 7572 7265 6e74 2066 7265   the current fre
+000043c0: 7175 656e 6379 0a20 2020 2020 2020 7368  quency.       sh
+000043d0: 6170 6520 6973 2074 6865 206e 616d 6520  ape is the name 
+000043e0: 6f66 2074 6865 2063 7572 7265 6e74 2073  of the current s
+000043f0: 6861 7065 0a20 2020 2020 2020 4c20 6973  hape.       L is
+00004400: 2074 6865 2073 6861 7065 7320 6465 706f   the shapes depo
+00004410: 6c61 7269 7361 7469 6f6e 206d 6174 7269  larisation matri
+00004420: 780a 2020 2020 2020 2073 697a 6520 6973  x.       size is
+00004430: 2074 6865 2064 696d 656e 7369 6f6e 6c65   the dimensionle
+00004440: 7373 2073 697a 6520 7061 7261 6d65 7465  ss size paramete
+00004450: 7220 666f 7220 7468 6520 6672 6571 7565  r for the freque
+00004460: 6e63 7920 756e 6465 7220 636f 6e73 6964  ncy under consid
+00004470: 6572 6174 696f 6e20 286e 6f74 2075 7365  eration (not use
+00004480: 6429 0a20 2020 2020 2020 5468 6520 726f  d).       The ro
+00004490: 7574 696e 6520 7265 7475 726e 7320 7468  utine returns th
+000044a0: 6520 6566 6665 6374 6976 6520 6469 656c  e effective diel
+000044b0: 6563 7472 6963 2063 6f6e 7374 616e 7422  ectric constant"
+000044c0: 2222 0a20 2020 2065 6666 6420 3d20 7666  "".    effd = vf
+000044d0: 202a 2063 7279 7374 616c 5f70 6572 6d69   * crystal_permi
+000044e0: 7474 6976 6974 7920 2b20 2831 2e30 2d76  ttivity + (1.0-v
+000044f0: 6629 202a 2064 6965 6c65 6374 7269 635f  f) * dielectric_
+00004500: 6d65 6469 756d 0a20 2020 2074 7261 6365  medium.    trace
+00004510: 203d 206e 702e 7472 6163 6528 6566 6664   = np.trace(effd
+00004520: 2920 2f20 332e 300a 2020 2020 6566 6664  ) / 3.0.    effd
+00004530: 6965 6c65 6320 3d20 6e70 2e61 7272 6179  ielec = np.array
+00004540: 285b 5b74 7261 6365 2c20 302c 2030 5d2c  ([[trace, 0, 0],
+00004550: 205b 302c 2074 7261 6365 2c20 305d 2c20   [0, trace, 0], 
+00004560: 5b30 2c20 302c 2074 7261 6365 5d5d 290a  [0, 0, trace]]).
+00004570: 2020 2020 7265 7475 726e 2065 6666 6469      return effdi
+00004580: 656c 6563 0a0a 6465 6620 6261 6c61 6e28  elec..def balan(
+00004590: 6469 656c 6563 7472 6963 5f6d 6564 6975  dielectric_mediu
+000045a0: 6d2c 2063 7279 7374 616c 5f70 6572 6d69  m, crystal_permi
+000045b0: 7474 6976 6974 792c 2073 6861 7065 2c20  ttivity, shape, 
+000045c0: 4c2c 2076 662c 2073 697a 6529 3a0a 2020  L, vf, size):.  
+000045d0: 2020 2222 2243 616c 6375 6c61 7465 2074    """Calculate t
+000045e0: 6865 2065 6666 6563 7469 7665 2063 6f6e  he effective con
+000045f0: 7374 616e 7420 7065 726d 6974 7469 7669  stant permittivi
+00004600: 7479 2075 7369 6e67 2074 6865 206d 6574  ty using the met
+00004610: 686f 6420 6f66 2062 616c 616e 0a20 2020  hod of balan.   
+00004620: 2020 2020 6469 656c 6563 7472 6963 5f6d      dielectric_m
+00004630: 6564 6975 6d20 6973 2074 6865 2064 6965  edium is the die
+00004640: 6c65 6374 7269 6320 636f 6e73 7461 6e74  lectric constant
+00004650: 2074 656e 736f 7220 6f66 2074 6865 206d   tensor of the m
+00004660: 6564 6975 6d0a 2020 2020 2020 2063 7279  edium.       cry
+00004670: 7374 616c 5f70 6572 6d69 7474 6976 6974  stal_permittivit
+00004680: 7920 6973 2074 6865 2074 6f74 616c 2066  y is the total f
+00004690: 7265 7175 656e 6379 2064 6965 6c65 6374  requency dielect
+000046a0: 7269 6320 636f 6e73 7461 6e74 2074 656e  ric constant ten
+000046b0: 736f 7220 6174 2074 6865 2063 7572 7265  sor at the curre
+000046c0: 6e74 2066 7265 7175 656e 6379 0a20 2020  nt frequency.   
+000046d0: 2020 2020 7368 6170 6520 6973 2074 6865      shape is the
+000046e0: 206e 616d 6520 6f66 2074 6865 2063 7572   name of the cur
+000046f0: 7265 6e74 2073 6861 7065 0a20 2020 2020  rent shape.     
+00004700: 2020 4c20 6973 2074 6865 2073 6861 7065    L is the shape
+00004710: 7320 6465 706f 6c61 7269 7361 7469 6f6e  s depolarisation
+00004720: 206d 6174 7269 780a 2020 2020 2020 2073   matrix.       s
+00004730: 697a 6520 6973 2074 6865 2064 696d 656e  ize is the dimen
+00004740: 7369 6f6e 6c65 7373 2073 697a 6520 7061  sionless size pa
+00004750: 7261 6d65 7465 7220 666f 7220 7468 6520  rameter for the 
+00004760: 6672 6571 7565 6e63 7920 756e 6465 7220  frequency under 
+00004770: 636f 6e73 6964 6572 6174 696f 6e20 286e  consideration (n
+00004780: 6f74 2075 7365 6429 0a20 2020 2020 2020  ot used).       
+00004790: 5468 6520 726f 7574 696e 6520 7265 7475  The routine retu
+000047a0: 726e 7320 7468 6520 6566 6665 6374 6976  rns the effectiv
+000047b0: 6520 6469 656c 6563 7472 6963 2063 6f6e  e dielectric con
+000047c0: 7374 616e 7422 2222 0a20 2020 2075 6e69  stant""".    uni
+000047d0: 7420 3d20 696e 6974 6961 6c69 7365 5f75  t = initialise_u
+000047e0: 6e69 745f 7465 6e73 6f72 2829 0a20 2020  nit_tensor().   
+000047f0: 2064 6965 6c65 6376 6d31 203d 2028 6372   dielecvm1 = (cr
+00004800: 7973 7461 6c5f 7065 726d 6974 7469 7669  ystal_permittivi
+00004810: 7479 202d 2075 6e69 7429 0a20 2020 2064  ty - unit).    d
+00004820: 6566 6f72 6d61 7469 6f6e 2020 3d20 6e70  eformation  = np
+00004830: 2e64 6f74 2864 6965 6c65 6374 7269 635f  .dot(dielectric_
+00004840: 6d65 6469 756d 2c20 6e70 2e6c 696e 616c  medium, np.linal
+00004850: 672e 696e 7628 6469 656c 6563 7472 6963  g.inv(dielectric
+00004860: 5f6d 6564 6975 6d20 2b20 6e70 2e64 6f74  _medium + np.dot
+00004870: 284c 2c20 2863 7279 7374 616c 5f70 6572  (L, (crystal_per
+00004880: 6d69 7474 6976 6974 7920 2d20 6469 656c  mittivity - diel
+00004890: 6563 7472 6963 5f6d 6564 6975 6d29 2929  ectric_medium)))
+000048a0: 290a 2020 2020 6566 6664 2020 2020 2020  ).    effd      
+000048b0: 2020 2020 3d20 756e 6974 202b 206e 702e      = unit + np.
+000048c0: 646f 7428 6465 666f 726d 6174 696f 6e2c  dot(deformation,
+000048d0: 2064 6965 6c65 6376 6d31 290a 2020 2020   dielecvm1).    
+000048e0: 7472 6163 6520 3d20 7666 202a 206e 702e  trace = vf * np.
+000048f0: 7472 6163 6528 6566 6664 2920 2f20 332e  trace(effd) / 3.
+00004900: 300a 2020 2020 6566 6664 6965 6c65 6320  0.    effdielec 
+00004910: 3d20 6e70 2e61 7272 6179 285b 5b74 7261  = np.array([[tra
+00004920: 6365 2c20 302c 2030 5d2c 205b 302c 2074  ce, 0, 0], [0, t
+00004930: 7261 6365 2c20 305d 2c20 5b30 2c20 302c  race, 0], [0, 0,
+00004940: 2074 7261 6365 5d5d 290a 2020 2020 7265   trace]]).    re
+00004950: 7475 726e 2065 6666 6469 656c 6563 0a0a  turn effdielec..
+00004960: 6465 6620 7370 6865 7269 6361 6c5f 6176  def spherical_av
+00004970: 6572 6167 6564 5f6d 6965 5f73 6361 7474  eraged_mie_scatt
+00004980: 6572 696e 6728 6469 656c 6563 7472 6963  ering(dielectric
+00004990: 5f6d 6564 6975 6d2c 2063 7279 7374 616c  _medium, crystal
+000049a0: 5f70 6572 6d69 7474 6976 6974 792c 2073  _permittivity, s
+000049b0: 6861 7065 2c20 4c2c 2076 662c 2073 697a  hape, L, vf, siz
+000049c0: 652c 2073 697a 655f 6d75 2c20 7369 7a65  e, size_mu, size
+000049d0: 5f64 6973 7472 6962 7574 696f 6e5f 7369  _distribution_si
+000049e0: 676d 6129 3a0a 2020 2020 2222 2243 616c  gma):.    """Cal
+000049f0: 6375 6c61 7465 2074 6865 2065 6666 6563  culate the effec
+00004a00: 7469 7665 2063 6f6e 7374 616e 7420 7065  tive constant pe
+00004a10: 726d 6974 7469 7669 7479 2075 7369 6e67  rmittivity using
+00004a20: 2061 204d 6965 2073 6361 7474 6572 696e   a Mie scatterin
+00004a30: 6720 6170 7072 6f61 6368 0a20 2020 2020  g approach.     
+00004a40: 2020 6469 656c 6563 7472 6963 5f6d 6564    dielectric_med
+00004a50: 6975 6d20 6973 2074 6865 2064 6965 6c65  ium is the diele
+00004a60: 6374 7269 6320 636f 6e73 7461 6e74 2074  ctric constant t
+00004a70: 656e 736f 7220 6f66 2074 6865 206d 6564  ensor of the med
+00004a80: 6975 6d0a 2020 2020 2020 2063 7279 7374  ium.       cryst
+00004a90: 616c 5f70 6572 6d69 7474 6976 6974 7920  al_permittivity 
+00004aa0: 6973 2074 6865 2074 6f74 616c 2066 7265  is the total fre
+00004ab0: 7175 656e 6379 2064 6965 6c65 6374 7269  quency dielectri
+00004ac0: 6320 636f 6e73 7461 6e74 2074 656e 736f  c constant tenso
+00004ad0: 7220 6174 2074 6865 2063 7572 7265 6e74  r at the current
+00004ae0: 2066 7265 7175 656e 6379 0a20 2020 2020   frequency.     
+00004af0: 2020 7368 6170 6520 6973 2074 6865 206e    shape is the n
+00004b00: 616d 6520 6f66 2074 6865 2063 7572 7265  ame of the curre
+00004b10: 6e74 2073 6861 7065 2028 4e4f 5420 5553  nt shape (NOT US
+00004b20: 4544 290a 2020 2020 2020 204c 2069 7320  ED).       L is 
+00004b30: 7468 6520 7368 6170 6573 2064 6570 6f6c  the shapes depol
+00004b40: 6172 6973 6174 696f 6e20 6d61 7472 6978  arisation matrix
+00004b50: 2028 4e4f 5420 5553 4544 290a 2020 2020   (NOT USED).    
+00004b60: 2020 2073 697a 6520 6973 2074 6865 2064     size is the d
+00004b70: 696d 656e 7369 6f6e 6c65 7373 2073 697a  imensionless siz
+00004b80: 6520 7061 7261 6d65 7465 7220 666f 7220  e parameter for 
+00004b90: 7468 6520 6672 6571 7565 6e63 7920 756e  the frequency un
+00004ba0: 6465 7220 636f 6e73 6964 6572 6174 696f  der consideratio
+00004bb0: 6e0a 2020 2020 2020 2073 697a 655f 6469  n.       size_di
+00004bc0: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
+00004bd0: 2069 7320 7468 6520 6c6f 6720 6e6f 726d   is the log norm
+00004be0: 616c 2076 616c 7565 206f 6620 7369 676d  al value of sigm
+00004bf0: 610a 2020 2020 2020 2076 6620 6973 2074  a.       vf is t
+00004c00: 6865 2076 6f6c 756d 6520 6672 6163 7469  he volume fracti
+00004c10: 6f6e 206f 6620 6669 6c6c 6572 0a20 2020  on of filler.   
+00004c20: 2020 2020 4d69 6520 6f6e 6c79 2077 6f72      Mie only wor
+00004c30: 6b73 2066 6f72 2073 7068 6572 6963 616c  ks for spherical
+00004c40: 2070 6172 7469 636c 6573 2c20 736f 2073   particles, so s
+00004c50: 6861 7065 2c20 616e 6420 4c20 7061 7261  hape, and L para
+00004c60: 6d65 7465 7273 2061 7265 2069 676e 6f72  meters are ignor
+00004c70: 6564 0a20 2020 2020 2020 5468 6520 616e  ed.       The an
+00004c80: 6973 6f74 726f 7079 206f 6620 7468 6520  isotropy of the 
+00004c90: 7065 726d 6974 7469 7669 7479 2069 7320  permittivity is 
+00004ca0: 6163 636f 756e 7465 6420 666f 7220 6279  accounted for by
+00004cb0: 2073 616d 706c 696e 6720 6d61 6e79 2064   sampling many d
+00004cc0: 6972 6563 7469 6f6e 730a 2020 2020 2020  irections.      
+00004cd0: 2061 6e64 2063 616c 6375 6c61 7469 6e67   and calculating
+00004ce0: 2074 6865 2073 6361 7474 6572 696e 6720   the scattering 
+00004cf0: 696e 2065 6163 6820 6469 7265 6374 696f  in each directio
+00004d00: 6e0a 2020 2020 2020 2054 6865 2072 6f75  n.       The rou
+00004d10: 7469 6e65 2072 6574 7572 6e73 2074 6865  tine returns the
+00004d20: 2065 6666 6563 7469 7665 2064 6965 6c65   effective diele
+00004d30: 6374 7269 6320 636f 6e73 7461 6e74 2222  ctric constant""
+00004d40: 220a 2020 2020 676c 6f62 616c 2070 6f69  ".    global poi
+00004d50: 6e74 735f 6f6e 5f73 7068 6572 650a 2020  nts_on_sphere.  
+00004d60: 2020 2320 6465 6669 6e65 2069 2061 7320    # define i as 
+00004d70: 6120 636f 6d70 6c65 7820 6e75 6d62 6572  a complex number
+00004d80: 0a20 2020 2069 203d 2063 6f6d 706c 6578  .    i = complex
+00004d90: 2830 2c31 290a 2020 2020 2320 5765 206e  (0,1).    # We n
+00004da0: 6565 6420 746f 2074 616b 656e 2061 6363  eed to taken acc
+00004db0: 6f75 6e74 206f 6620 7468 6520 6368 616e  ount of the chan
+00004dc0: 6765 2069 6e20 7761 7665 6c65 6e67 7468  ge in wavelength
+00004dd0: 2061 6e64 2074 6865 2063 6861 6e67 6520   and the change 
+00004de0: 696e 2073 697a 6520 7061 7261 6d65 7465  in size paramete
+00004df0: 7220 6475 6520 746f 2074 6865 0a20 2020  r due to the.   
+00004e00: 2023 204e 6f6e 6520 756e 6974 2076 616c   # None unit val
+00004e10: 7565 206f 6620 7468 6520 6469 656c 6563  ue of the dielec
+00004e20: 7472 6963 206f 6620 7468 6520 656d 6265  tric of the embe
+00004e30: 6464 696e 6720 6d65 6469 756d 0a20 2020  dding medium.   
+00004e40: 2023 2054 6865 2073 697a 6520 7061 7261   # The size para
+00004e50: 6d65 7465 7220 6973 2032 7069 2072 202f  meter is 2pi r /
+00004e60: 206c 616d 6264 610a 2020 2020 2320 5468   lambda.    # Th
+00004e70: 6520 6566 6665 6374 6976 6520 6c61 6d62  e effective lamb
+00004e80: 6461 2069 6e20 7468 6520 7375 7070 6f72  da in the suppor
+00004e90: 7469 6e67 206d 6564 6975 6d20 6973 206c  ting medium is l
+00004ea0: 616d 6264 6120 2f20 7371 7274 2865 6d65  ambda / sqrt(eme
+00004eb0: 6469 756d 290a 2020 2020 2320 5768 6572  dium).    # Wher
+00004ec0: 6520 7468 6520 7265 6672 6163 7469 7665  e the refractive
+00004ed0: 2069 6e64 6578 2069 7320 7461 6b65 6e20   index is taken 
+00004ee0: 746f 2062 6520 7371 7274 2865 6d65 6469  to be sqrt(emedi
+00004ef0: 756d 2920 286e 6f6e 206d 6167 6e65 7469  um) (non magneti
+00004f00: 6320 6d61 7465 7269 616c 7329 0a20 2020  c materials).   
+00004f10: 2065 6d65 6469 756d 203d 206e 702e 7472   emedium = np.tr
+00004f20: 6163 6528 6469 656c 6563 7472 6963 5f6d  ace(dielectric_m
+00004f30: 6564 6975 6d29 202f 2033 2e30 0a20 2020  edium) / 3.0.   
+00004f40: 2072 6566 7261 6374 6976 655f 696e 6465   refractive_inde
+00004f50: 785f 6d65 6469 756d 203d 206e 702e 7265  x_medium = np.re
+00004f60: 616c 286e 702e 7371 7274 2865 6d65 6469  al(np.sqrt(emedi
+00004f70: 756d 2929 0a20 2020 206c 616d 6264 615f  um)).    lambda_
+00004f80: 7661 6375 756d 5f6d 7520 3d20 3220 2a20  vacuum_mu = 2 * 
+00004f90: 5049 202a 2073 697a 655f 6d75 202f 2073  PI * size_mu / s
+00004fa0: 697a 650a 2020 2020 7761 7665 6c65 6e67  ize.    waveleng
+00004fb0: 7468 5f6e 6d20 3d20 6c61 6d62 6461 5f76  th_nm = lambda_v
+00004fc0: 6163 7575 6d5f 6d75 202a 2031 3030 3020  acuum_mu * 1000 
+00004fd0: 2f20 7265 6672 6163 7469 7665 5f69 6e64  / refractive_ind
+00004fe0: 6578 5f6d 6564 6975 6d0a 2020 2020 7261  ex_medium.    ra
+00004ff0: 6469 7573 5f6e 6d20 3d20 7369 7a65 5f6d  dius_nm = size_m
+00005000: 7520 2a20 3130 3030 0a20 2020 2023 2054  u * 1000.    # T
+00005010: 6865 2077 6176 6576 6563 746f 7220 696e  he wavevector in
+00005020: 206e 6d2d 310a 2020 2020 6b5f 6e6d 203d   nm-1.    k_nm =
+00005030: 2032 202a 2050 4920 2f20 7761 7665 6c65   2 * PI / wavele
+00005040: 6e67 7468 5f6e 6d0a 2020 2020 2320 766f  ngth_nm.    # vo
+00005050: 6c75 6d65 206f 6620 6120 7061 7274 6963  lume of a partic
+00005060: 6c65 2069 6e20 6e6d 5e33 0a20 2020 2056  le in nm^3.    V
+00005070: 5f6e 6d20 3d20 342e 302f 332e 3020 2a20  _nm = 4.0/3.0 * 
+00005080: 5049 202a 2072 6164 6975 735f 6e6d 202a  PI * radius_nm *
+00005090: 2072 6164 6975 735f 6e6d 202a 2072 6164   radius_nm * rad
+000050a0: 6975 735f 6e6d 0a20 2020 2023 204e 756d  ius_nm.    # Num
+000050b0: 6265 7220 6465 6e73 6974 7920 6f66 2070  ber density of p
+000050c0: 6172 7469 636c 6573 2028 6e75 6d62 6572  articles (number
+000050d0: 202f 206e 6d5e 3329 0a20 2020 204e 5f6e   / nm^3).    N_n
+000050e0: 6d20 3d20 7666 202f 2056 5f6e 6d0a 2020  m = vf / V_nm.  
+000050f0: 2020 2320 4966 2074 6865 7265 2069 7320    # If there is 
+00005100: 6120 7369 7a65 2064 6973 7472 6962 7574  a size distribut
+00005110: 696f 6e20 7365 7420 7570 2074 6f20 7573  ion set up to us
+00005120: 6520 6974 0a20 2020 2069 6620 7369 7a65  e it.    if size
+00005130: 5f64 6973 7472 6962 7574 696f 6e5f 7369  _distribution_si
+00005140: 676d 613a 0a20 2020 2020 2020 206c 6f77  gma:.        low
+00005150: 6572 2c75 7070 6572 203d 206c 6f67 6e6f  er,upper = logno
+00005160: 726d 2e69 6e74 6572 7661 6c28 302e 3939  rm.interval(0.99
+00005170: 3939 2c73 697a 655f 6469 7374 7269 6275  99,size_distribu
+00005180: 7469 6f6e 5f73 6967 6d61 2c73 6361 6c65  tion_sigma,scale
+00005190: 3d73 697a 655f 6d75 290a 2020 2020 2020  =size_mu).      
+000051a0: 2020 6e75 6d62 6572 4f66 4269 6e73 203d    numberOfBins =
+000051b0: 2034 300a 2020 2020 2020 2020 6470 203d   40.        dp =
+000051c0: 206e 702e 6c6f 6773 7061 6365 286e 702e   np.logspace(np.
+000051d0: 6c6f 6728 6c6f 7765 7229 2c6e 702e 6c6f  log(lower),np.lo
+000051e0: 6728 7570 7065 7229 2c6e 756d 6265 724f  g(upper),numberO
+000051f0: 6642 696e 732c 6261 7365 3d6e 702e 6529  fBins,base=np.e)
+00005200: 0a20 2020 2020 2020 2023 2054 6865 2064  .        # The d
+00005210: 6566 696e 6974 696f 6e73 2075 7365 6420  efinitions used 
+00005220: 6172 6520 636f 6e66 7573 696e 673b 0a20  are confusing;. 
+00005230: 2020 2020 2020 2023 2064 7020 6973 2074         # dp is t
+00005240: 6865 206c 6f67 206f 6620 7468 6520 7661  he log of the va
+00005250: 7269 6162 6c65 0a20 2020 2020 2020 2023  riable.        #
+00005260: 2073 2069 7320 7468 6520 7374 616e 6461   s is the standa
+00005270: 7264 2064 6576 6961 7469 6f6e 2028 7368  rd deviation (sh
+00005280: 6170 6520 6675 6e63 7469 6f6e 2920 6f66  ape function) of
+00005290: 2074 6865 206c 6f67 206f 6620 7468 6520   the log of the 
+000052a0: 7661 7269 6174 650a 2020 2020 2020 2020  variate.        
+000052b0: 2320 7363 616c 6520 6973 2074 6865 206d  # scale is the m
+000052c0: 6561 6e20 6f66 2074 6865 2075 6e64 6572  ean of the under
+000052d0: 6c79 696e 6720 6e6f 726d 616c 2064 6973  lying normal dis
+000052e0: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
+000052f0: 2020 6e64 7020 3d20 6c6f 676e 6f72 6d2e    ndp = lognorm.
+00005300: 7064 6628 6470 2c73 3d73 697a 655f 6469  pdf(dp,s=size_di
+00005310: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
+00005320: 2c73 6361 6c65 3d73 697a 655f 6d75 290a  ,scale=size_mu).
+00005330: 2020 2020 2020 2020 2370 7269 6e74 2822          #print("
+00005340: 4450 222c 6470 290a 2020 2020 2020 2020  DP",dp).        
+00005350: 2370 7269 6e74 2822 4e44 5022 2c6e 6470  #print("NDP",ndp
+00005360: 290a 2020 2020 2020 2020 2370 7269 6e74  ).        #print
+00005370: 2822 5570 7065 7220 6c6f 7765 7222 2c6c  ("Upper lower",l
+00005380: 6f77 6572 2c75 7070 6572 290a 2020 2020  ower,upper).    
+00005390: 2020 2020 2370 7269 6e74 2822 5369 7a65      #print("Size
+000053a0: 5f4d 5522 2c73 697a 655f 6d75 290a 2020  _MU",size_mu).  
+000053b0: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
+000053c0: 6520 7361 6d70 6c69 6e67 2070 6f69 6e74  e sampling point
+000053d0: 7320 6f6e 2061 2066 6962 6f6e 6163 6369  s on a fibonacci
+000053e0: 2073 7068 6572 650a 2020 2020 6966 2070   sphere.    if p
+000053f0: 6f69 6e74 735f 6f6e 5f73 7068 6572 6520  oints_on_sphere 
+00005400: 3d3d 204e 6f6e 653a 0a20 2020 2020 2020  == None:.       
+00005410: 2070 6f69 6e74 735f 6f6e 5f73 7068 6572   points_on_spher
+00005420: 6520 3d20 6669 626f 6e61 6363 695f 7370  e = fibonacci_sp
+00005430: 6865 7265 2873 616d 706c 6573 3d35 3030  here(samples=500
+00005440: 2c72 616e 646f 6d69 7a65 3d54 7275 6529  ,randomize=True)
+00005450: 0a20 2020 2074 7261 6365 203d 2030 2e30  .    trace = 0.0
+00005460: 0a20 2020 2023 204e 6f77 2074 616b 6520  .    # Now take 
+00005470: 7468 6520 6176 6572 6167 6520 6f66 2065  the average of e
+00005480: 6163 6820 6469 7265 6374 696f 6e20 6f6e  ach direction on
+00005490: 2074 6865 2073 7068 6572 650a 2020 2020   the sphere.    
+000054a0: 666f 7220 706f 696e 7420 696e 2070 6f69  for point in poi
+000054b0: 6e74 735f 6f6e 5f73 7068 6572 653a 0a20  nts_on_sphere:. 
+000054c0: 2020 2020 2020 2070 6f69 6e74 203d 206e         point = n
+000054d0: 702e 6172 7261 7928 706f 696e 7429 0a20  p.array(point). 
+000054e0: 2020 2020 2020 2072 6f74 6174 6564 5f64         rotated_d
+000054f0: 6965 6c65 6320 3d20 6e70 2e64 6f74 2870  ielec = np.dot(p
+00005500: 6f69 6e74 2c20 6e70 2e64 6f74 2870 6f69  oint, np.dot(poi
+00005510: 6e74 2c20 6372 7973 7461 6c5f 7065 726d  nt, crystal_perm
+00005520: 6974 7469 7669 7479 2929 0a20 2020 2020  ittivity)).     
+00005530: 2020 2072 6566 7261 6374 6976 655f 696e     refractive_in
+00005540: 6465 7820 3d20 6361 6c63 756c 6174 655f  dex = calculate_
+00005550: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
+00005560: 5f73 6361 6c61 7228 726f 7461 7465 645f  _scalar(rotated_
+00005570: 6469 656c 6563 2920 2f20 7265 6672 6163  dielec) / refrac
+00005580: 7469 7665 5f69 6e64 6578 5f6d 6564 6975  tive_index_mediu
+00005590: 6d0a 2020 2020 2020 2020 2320 7072 696e  m.        # prin
+000055a0: 7428 2772 6566 7261 6374 6976 655f 696e  t('refractive_in
+000055b0: 6465 7827 2c20 7265 6672 6163 7469 7665  dex', refractive
+000055c0: 5f69 6e64 6578 290a 2020 2020 2020 2020  _index).        
+000055d0: 2320 7072 696e 7428 2772 6566 7261 6374  # print('refract
+000055e0: 6976 655f 696e 6465 785f 6d65 6469 756d  ive_index_medium
+000055f0: 272c 2072 6566 7261 6374 6976 655f 696e  ', refractive_in
+00005600: 6465 785f 6d65 6469 756d 290a 2020 2020  dex_medium).    
+00005610: 2020 2020 2320 7072 696e 7428 2772 6f74      # print('rot
+00005620: 6174 6564 5f64 6965 6c65 6327 2c20 726f  ated_dielec', ro
+00005630: 7461 7465 645f 6469 656c 6563 290a 2020  tated_dielec).  
+00005640: 2020 2020 2020 6966 2073 697a 655f 6469        if size_di
+00005650: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
+00005660: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00005670: 4361 6c63 756c 6174 6520 7468 6520 696e  Calculate the in
+00005680: 7465 6772 616c 206f 6620 7468 6520 666f  tegral of the fo
+00005690: 7277 6172 6420 7363 6174 7465 7269 6e67  rward scattering
+000056a0: 2066 6163 746f 7273 206f 7665 7220 7468   factors over th
+000056b0: 6520 6469 7374 7269 6275 7469 6f6e 0a20  e distribution. 
+000056c0: 2020 2020 2020 2020 2020 2073 315f 6661             s1_fa
+000056d0: 6374 6f72 7320 3d20 5b5d 0a20 2020 2020  ctors = [].     
+000056e0: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
+000056f0: 6470 3a0a 2020 2020 2020 2020 2020 2020  dp:.            
+00005700: 2020 2020 2320 5468 6520 7369 7a65 2070      # The size p
+00005710: 6172 616d 6574 6572 2069 7320 3270 6920  arameter is 2pi 
+00005720: 7220 2f20 6c61 6d62 6461 0a20 2020 2020  r / lambda.     
+00005730: 2020 2020 2020 2020 2020 2078 203d 2032             x = 2
+00005740: 202a 2050 4920 2a20 7220 2f20 6c61 6d62   * PI * r / lamb
+00005750: 6461 5f76 6163 7575 6d5f 6d75 0a20 2020  da_vacuum_mu.   
+00005760: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+00005770: 616c 6375 6c61 7465 2074 6865 2053 3120  alculate the S1 
+00005780: 616e 6420 5332 2073 6361 7474 6572 696e  and S2 scatterin
+00005790: 6720 6661 6374 6f72 732c 2061 6e64 2073  g factors, and s
+000057a0: 746f 7265 2069 6e20 6120 6c69 7374 0a20  tore in a list. 
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000057c0: 312c 7332 203d 204d 6965 2e4d 6965 5331  1,s2 = Mie.MieS1
+000057d0: 5332 2872 6566 7261 6374 6976 655f 696e  S2(refractive_in
+000057e0: 6465 782c 2078 2a72 6566 7261 6374 6976  dex, x*refractiv
+000057f0: 655f 696e 6465 785f 6d65 6469 756d 2c20  e_index_medium, 
+00005800: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+00005810: 2020 2073 315f 6661 6374 6f72 732e 6170     s1_factors.ap
+00005820: 7065 6e64 2873 3129 0a20 2020 2020 2020  pend(s1).       
+00005830: 2020 2020 2023 204e 6f77 2069 6e74 6567       # Now integ
+00005840: 7261 7465 0a20 2020 2020 2020 2020 2020  rate.           
+00005850: 2073 3120 3d20 7472 6170 7a28 7331 5f66   s1 = trapz(s1_f
+00005860: 6163 746f 7273 2a6e 6470 2c64 7029 0a20  actors*ndp,dp). 
+00005870: 2020 2020 2020 2020 2020 206e 6f72 6d61             norma
+00005880: 6c20 3d20 7472 6170 7a28 6e64 702c 6470  l = trapz(ndp,dp
+00005890: 290a 2020 2020 2020 2020 2020 2020 236d  ).            #m
+000058a0: 6561 6e20 3d20 7472 6170 7a28 6e64 702a  ean = trapz(ndp*
+000058b0: 6470 2c64 7029 0a20 2020 2020 2020 2020  dp,dp).         
+000058c0: 2020 2023 7472 7565 5f6d 6561 6e20 3d20     #true_mean = 
+000058d0: 6e70 2e65 7870 2820 6e70 2e6c 6f67 2873  np.exp( np.log(s
+000058e0: 697a 655f 6d75 2920 2b20 7369 7a65 5f64  ize_mu) + size_d
+000058f0: 6973 7472 6962 7574 696f 6e5f 7369 676d  istribution_sigm
+00005900: 612a 7369 7a65 5f64 6973 7472 6962 7574  a*size_distribut
+00005910: 696f 6e5f 7369 676d 612f 322e 3029 0a20  ion_sigma/2.0). 
+00005920: 2020 2020 2020 2020 2020 2023 765f 636d             #v_cm
+00005930: 3120 3d20 312e 3045 342f 6c61 6d62 6461  1 = 1.0E4/lambda
+00005940: 5f76 6163 7575 6d5f 6d75 0a20 2020 2020  _vacuum_mu.     
+00005950: 2020 2020 2020 2023 7072 696e 7428 2246         #print("F
+00005960: 7265 7175 656e 6379 2c6e 6f72 6d61 6c2c  requency,normal,
+00005970: 6d65 616e 222c 765f 636d 312c 6e6f 726d  mean",v_cm1,norm
+00005980: 616c 2c74 7275 655f 6d65 616e 2c6d 6561  al,true_mean,mea
+00005990: 6e29 0a20 2020 2020 2020 2020 2020 2069  n).            i
+000059a0: 6620 6e70 2e61 6273 286e 6f72 6d61 6c20  f np.abs(normal 
+000059b0: 2d20 312e 3029 203e 2031 2e30 452d 323a  - 1.0) > 1.0E-2:
+000059c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059d0: 2070 7269 6e74 2822 5761 726e 696e 6720   print("Warning 
+000059e0: 696e 7465 6772 6174 696f 6e20 6f66 206c  integration of l
+000059f0: 6f67 2d6e 6f72 6d61 6c20 6469 7374 7269  og-normal distri
+00005a00: 6275 7469 6f6e 2069 6e20 6572 726f 7222  bution in error"
+00005a10: 2c20 6e6f 726d 616c 290a 2020 2020 2020  , normal).      
+00005a20: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00005a30: 2253 746f 7070 696e 6720 6361 6c63 756c  "Stopping calcul
+00005a40: 6174 696f 6e20 2d20 6c69 6b65 6c79 2070  ation - likely p
+00005a50: 726f 626c 656d 2069 7320 746f 6f20 6c61  roblem is too la
+00005a60: 7267 6520 6120 7369 676d 6120 666f 7220  rge a sigma for 
+00005a70: 6c6f 672d 6e6f 726d 616c 2064 6973 7472  log-normal distr
+00005a80: 6962 7574 696f 6e22 290a 2020 2020 2020  ibution").      
+00005a90: 2020 2020 2020 2020 2020 6566 6664 6965            effdie
+00005aa0: 6c65 6320 3d20 6e70 2e61 7272 6179 285b  lec = np.array([
+00005ab0: 5b31 2c20 302c 2030 5d2c 205b 302c 2031  [1, 0, 0], [0, 1
+00005ac0: 2c20 305d 2c20 5b30 2c20 302c 2031 5d5d  , 0], [0, 0, 1]]
+00005ad0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005ae0: 2020 7265 7475 726e 2065 6666 6469 656c    return effdiel
+00005af0: 6563 0a20 2020 2020 2020 2065 6c73 653a  ec.        else:
+00005b00: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+00005b10: 616c 6375 6c61 7465 2074 6865 2073 6361  alculate the sca
+00005b20: 7474 6572 696e 6720 6661 6374 6f72 7320  ttering factors 
+00005b30: 6174 2030 2064 6567 7265 6573 0a20 2020  at 0 degrees.   
+00005b40: 2020 2020 2020 2020 2023 6a6b 2070 7269           #jk pri
+00005b50: 6e74 2822 7265 6672 6163 7469 7665 5f69  nt("refractive_i
+00005b60: 6e64 6578 2c20 7369 7a65 2c20 7265 6672  ndex, size, refr
+00005b70: 6163 7469 7665 5f69 6e64 6578 5f6d 6564  active_index_med
+00005b80: 6975 6d22 2c20 7265 6672 6163 7469 7665  ium", refractive
+00005b90: 5f69 6e64 6578 2c20 7369 7a65 2c20 7265  _index, size, re
+00005ba0: 6672 6163 7469 7665 5f69 6e64 6578 5f6d  fractive_index_m
+00005bb0: 6564 6975 6d29 0a20 2020 2020 2020 2020  edium).         
+00005bc0: 2020 2073 312c 7332 203d 204d 6965 2e4d     s1,s2 = Mie.M
+00005bd0: 6965 5331 5332 2872 6566 7261 6374 6976  ieS1S2(refractiv
+00005be0: 655f 696e 6465 782c 2073 697a 652a 7265  e_index, size*re
+00005bf0: 6672 6163 7469 7665 5f69 6e64 6578 5f6d  fractive_index_m
+00005c00: 6564 6975 6d2c 2031 290a 2020 2020 2020  edium, 1).      
+00005c10: 2020 2320 5365 6520 7661 6e20 6465 2048    # See van de H
+00005c20: 756c 7374 2070 6167 6520 3132 392c 2031  ulst page 129, 1
+00005c30: 3330 0a20 2020 2020 2020 2023 2052 6566  30.        # Ref
+00005c40: 7261 6374 6976 6520 696e 6465 7820 6f66  ractive index of
+00005c50: 206d 6174 6572 6961 6c20 6973 0a20 2020   material is.   
+00005c60: 2020 2020 2023 2074 6865 2073 6967 6e20       # the sign 
+00005c70: 6f66 2074 6865 2069 6d61 6769 6e61 7279  of the imaginary
+00005c80: 2063 6f6d 706f 6e65 6e74 2068 6173 2063   component has c
+00005c90: 6861 6e67 6564 2066 6f72 2063 6f6d 7061  hanged for compa
+00005ca0: 7469 6269 6c69 7479 2077 6974 6820 4d47  tibility with MG
+00005cb0: 2f42 7275 6767 656d 616e 0a20 2020 2020  /Bruggeman.     
+00005cc0: 2020 2072 6566 7261 6374 6976 655f 696e     refractive_in
+00005cd0: 6465 7820 3d20 7265 6672 6163 7469 7665  dex = refractive
+00005ce0: 5f69 6e64 6578 5f6d 6564 6975 6d20 2a20  _index_medium * 
+00005cf0: 2820 312e 3020 2b20 6920 2a20 7331 202a  ( 1.0 + i * s1 *
+00005d00: 2032 202a 2050 4920 2a20 4e5f 6e6d 202f   2 * PI * N_nm /
+00005d10: 2028 206b 5f6e 6d20 2a20 6b5f 6e6d 202a   ( k_nm * k_nm *
+00005d20: 206b 5f6e 6d20 2920 290a 2020 2020 2020   k_nm ) ).      
+00005d30: 2020 7472 6163 6520 2b3d 2072 6566 7261    trace += refra
+00005d40: 6374 6976 655f 696e 6465 780a 2020 2020  ctive_index.    
+00005d50: 2320 7265 7475 726e 2061 6e20 6973 6f74  # return an isot
+00005d60: 726f 7069 6320 7465 6e73 6f72 0a20 2020  ropic tensor.   
+00005d70: 2074 7261 6365 203d 2074 7261 6365 202f   trace = trace /
+00005d80: 206c 656e 2870 6f69 6e74 735f 6f6e 5f73   len(points_on_s
+00005d90: 7068 6572 6529 0a20 2020 2065 6666 203d  phere).    eff =
+00005da0: 2074 7261 6365 202a 2074 7261 6365 0a20   trace * trace. 
+00005db0: 2020 2065 6666 6469 656c 6563 203d 206e     effdielec = n
+00005dc0: 702e 6172 7261 7928 5b5b 6566 662c 2030  p.array([[eff, 0
+00005dd0: 2c20 305d 2c20 5b30 2c20 6566 662c 2030  , 0], [0, eff, 0
+00005de0: 5d2c 205b 302c 2030 2c20 6566 665d 5d29  ], [0, 0, eff]])
+00005df0: 0a20 2020 2023 6a6b 2070 7269 6e74 2872  .    #jk print(r
+00005e00: 6164 6975 735f 6e6d 2c20 6c61 6d62 6461  adius_nm, lambda
+00005e10: 5f76 6163 7575 6d5f 6d75 2a31 3030 302e  _vacuum_mu*1000.
+00005e20: 302c 2071 6578 742c 7173 6361 2c71 6162  0, qext,qsca,qab
+00005e30: 732c 672c 7170 722c 7162 6163 6b2c 7172  s,g,qpr,qback,qr
+00005e40: 6174 696f 2c6e 702e 7265 616c 2873 3129  atio,np.real(s1)
+00005e50: 2c6e 702e 696d 6167 2873 3129 2c6e 702e  ,np.imag(s1),np.
+00005e60: 7265 616c 2874 7261 6365 292c 6e70 2e69  real(trace),np.i
+00005e70: 6d61 6728 7472 6163 6529 2c6e 702e 7265  mag(trace),np.re
+00005e80: 616c 2865 6666 292c 6e70 2e69 6d61 6728  al(eff),np.imag(
+00005e90: 6566 6629 290a 2020 2020 2370 7269 6e74  eff)).    #print
+00005ea0: 2028 2272 6164 6975 735f 6e6d 2c20 6566   ("radius_nm, ef
+00005eb0: 6622 2c20 7261 6469 7573 5f6e 6d2c 2065  f", radius_nm, e
+00005ec0: 6666 290a 2020 2020 7265 7475 726e 2065  ff).    return e
+00005ed0: 6666 6469 656c 6563 0a0a 0a64 6566 206d  ffdielec...def m
+00005ee0: 6965 5f73 6361 7474 6572 696e 6728 6469  ie_scattering(di
+00005ef0: 656c 6563 7472 6963 5f6d 6564 6975 6d2c  electric_medium,
+00005f00: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
+00005f10: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
+00005f20: 2076 662c 2073 697a 652c 2073 697a 655f   vf, size, size_
+00005f30: 6d75 2c20 7369 7a65 5f64 6973 7472 6962  mu, size_distrib
+00005f40: 7574 696f 6e5f 7369 676d 6129 3a0a 2020  ution_sigma):.  
+00005f50: 2020 2222 2243 616c 6375 6c61 7465 2074    """Calculate t
+00005f60: 6865 2065 6666 6563 7469 7665 2063 6f6e  he effective con
+00005f70: 7374 616e 7420 7065 726d 6974 7469 7669  stant permittivi
+00005f80: 7479 2075 7369 6e67 2061 204d 6965 2073  ty using a Mie s
+00005f90: 6361 7474 6572 696e 6720 6170 7072 6f61  cattering approa
+00005fa0: 6368 0a20 2020 2020 2020 6469 656c 6563  ch.       dielec
+00005fb0: 7472 6963 5f6d 6564 6975 6d20 6973 2074  tric_medium is t
+00005fc0: 6865 2064 6965 6c65 6374 7269 6320 636f  he dielectric co
+00005fd0: 6e73 7461 6e74 2074 656e 736f 7220 6f66  nstant tensor of
+00005fe0: 2074 6865 206d 6564 6975 6d0a 2020 2020   the medium.    
+00005ff0: 2020 2063 7279 7374 616c 5f70 6572 6d69     crystal_permi
+00006000: 7474 6976 6974 7920 6973 2074 6865 2074  ttivity is the t
+00006010: 6f74 616c 2066 7265 7175 656e 6379 2064  otal frequency d
+00006020: 6965 6c65 6374 7269 6320 636f 6e73 7461  ielectric consta
+00006030: 6e74 2074 656e 736f 7220 6174 2074 6865  nt tensor at the
+00006040: 2063 7572 7265 6e74 2066 7265 7175 656e   current frequen
+00006050: 6379 0a20 2020 2020 2020 7368 6170 6520  cy.       shape 
+00006060: 6973 2074 6865 206e 616d 6520 6f66 2074  is the name of t
+00006070: 6865 2063 7572 7265 6e74 2073 6861 7065  he current shape
+00006080: 2028 4e4f 5420 5553 4544 290a 2020 2020   (NOT USED).    
+00006090: 2020 204c 2069 7320 7468 6520 7368 6170     L is the shap
+000060a0: 6573 2064 6570 6f6c 6172 6973 6174 696f  es depolarisatio
+000060b0: 6e20 6d61 7472 6978 2028 4e4f 5420 5553  n matrix (NOT US
+000060c0: 4544 290a 2020 2020 2020 2073 697a 6520  ED).       size 
+000060d0: 6973 2074 6865 2064 696d 656e 7369 6f6e  is the dimension
+000060e0: 6c65 7373 2073 697a 6520 7061 7261 6d65  less size parame
+000060f0: 7465 7220 666f 7220 7468 6520 6672 6571  ter for the freq
+00006100: 7565 6e63 7920 756e 6465 7220 636f 6e73  uency under cons
+00006110: 6964 6572 6174 696f 6e0a 2020 2020 2020  ideration.      
+00006120: 2073 697a 655f 6469 7374 7269 6275 7469   size_distributi
+00006130: 6f6e 5f73 6967 6d61 2069 7320 7468 6520  on_sigma is the 
+00006140: 6c6f 6720 6e6f 726d 616c 2076 616c 7565  log normal value
+00006150: 206f 6620 7369 676d 610a 2020 2020 2020   of sigma.      
+00006160: 2076 6620 6973 2074 6865 2076 6f6c 756d   vf is the volum
+00006170: 6520 6672 6163 7469 6f6e 206f 6620 6669  e fraction of fi
+00006180: 6c6c 6572 0a20 2020 2020 2020 496e 2074  ller.       In t
+00006190: 6869 7320 6d65 7468 6f64 2074 6865 204d  his method the M
+000061a0: 4720 6d65 7468 6f64 2069 7320 7573 6564  G method is used
+000061b0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+000061c0: 6520 6176 6572 6167 6564 2065 6666 6563  e averaged effec
+000061d0: 7469 7665 2070 6572 6d69 7474 6976 6974  tive permittivit
+000061e0: 790a 2020 2020 2020 2054 6865 6e20 7468  y.       Then th
+000061f0: 6520 7065 726d 6974 7469 7669 7479 206f  e permittivity o
+00006200: 6620 7468 6520 6973 6f64 7472 6f70 6963  f the isodtropic
+00006210: 2073 7068 6572 6520 7468 6174 2077 6f75   sphere that wou
+00006220: 6c64 2067 6976 6520 7468 6520 7361 6d65  ld give the same
+00006230: 2061 7665 7261 6765 2070 6572 6d69 7474   average permitt
+00006240: 6976 6974 7920 6973 2063 616c 6375 6c61  ivity is calcula
+00006250: 7465 640a 2020 2020 2020 2054 6865 6e20  ted.       Then 
+00006260: 7468 6520 4d69 6520 7363 6174 7465 7269  the Mie scatteri
+00006270: 6e67 206f 6620 7468 6174 2073 7068 6572  ng of that spher
+00006280: 6520 6973 2063 616c 6375 6c61 7465 640a  e is calculated.
+00006290: 2020 2020 2020 2054 6865 2072 6f75 7469         The routi
+000062a0: 6e65 2072 6574 7572 6e73 2074 6865 2065  ne returns the e
+000062b0: 6666 6563 7469 7665 2064 6965 6c65 6374  ffective dielect
+000062c0: 7269 6320 636f 6e73 7461 6e74 2222 220a  ric constant""".
+000062d0: 2020 2020 230a 2020 2020 2320 4361 6c63      #.    # Calc
+000062e0: 756c 6174 6520 7468 6520 4d47 2070 6572  ulate the MG per
+000062f0: 6d69 7474 6976 6974 7920 7769 7468 206e  mittivity with n
+00006300: 6f20 7369 7a65 2065 6666 6563 7473 0a20  o size effects. 
+00006310: 2020 2023 0a20 2020 206d 675f 7065 726d     #.    mg_perm
+00006320: 6974 7469 7669 7479 203d 206d 6178 7765  ittivity = maxwe
+00006330: 6c6c 2864 6965 6c65 6374 7269 635f 6d65  ll(dielectric_me
+00006340: 6469 756d 2c20 6372 7973 7461 6c5f 7065  dium, crystal_pe
+00006350: 726d 6974 7469 7669 7479 2c20 7368 6170  rmittivity, shap
+00006360: 652c 204c 2c20 7666 2c20 302e 3030 3030  e, L, vf, 0.0000
+00006370: 3030 3129 0a20 2020 2023 2055 7365 2073  001).    # Use s
+00006380: 6361 6c61 7220 7175 616e 7469 7469 6573  calar quantities
+00006390: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+000063a0: 6520 6469 656c 6563 7472 6963 2063 6f6e  e dielectric con
+000063b0: 7374 616e 7420 6f66 2074 6865 2065 7175  stant of the equ
+000063c0: 6976 616c 656e 7420 6973 6f74 726f 7069  ivalent isotropi
+000063d0: 6320 7370 6865 7265 0a20 2020 2065 6620  c sphere.    ef 
+000063e0: 3d20 6e70 2e74 7261 6365 286d 675f 7065  = np.trace(mg_pe
+000063f0: 726d 6974 7469 7669 7479 2920 2f20 332e  rmittivity) / 3.
+00006400: 300a 2020 2020 656d 203d 206e 702e 7472  0.    em = np.tr
+00006410: 6163 6528 6469 656c 6563 7472 6963 5f6d  ace(dielectric_m
+00006420: 6564 6975 6d29 202f 2033 2e30 0a20 2020  edium) / 3.0.   
+00006430: 2023 2070 7269 6e74 2827 6372 7973 7461   # print('crysta
+00006440: 6c5f 7065 726d 6974 7469 7669 7479 272c  l_permittivity',
+00006450: 6372 7973 7461 6c5f 7065 726d 6974 7469  crystal_permitti
+00006460: 7669 7479 290a 2020 2020 2320 7072 696e  vity).    # prin
+00006470: 7428 274d 6178 7765 6c6c 272c 6566 290a  t('Maxwell',ef).
+00006480: 2020 2020 2320 7072 696e 7428 2745 4d65      # print('EMe
+00006490: 6469 756d 272c 656d 290a 2020 2020 2320  dium',em).    # 
+000064a0: 4361 6c63 756c 6174 6520 7468 6520 7065  Calculate the pe
+000064b0: 726d 6974 7469 7669 7479 206f 6620 616e  rmittivity of an
+000064c0: 2069 736f 7472 6f70 6963 2073 7068 6572   isotropic spher
+000064d0: 6520 7468 6174 2068 6173 2074 6865 2073  e that has the s
+000064e0: 616d 6520 6566 6665 6374 6976 6520 7065  ame effective pe
+000064f0: 726d 6974 7469 7669 7479 0a20 2020 2065  rmittivity.    e
+00006500: 696e 636c 7573 696f 6e20 3d20 2820 2d33  inclusion = ( -3
+00006510: 2a76 662a 656d 2a65 6d20 2d20 2865 6620  *vf*em*em - (ef 
+00006520: 2d20 656d 292a 656d 2a28 322b 7666 2920  - em)*em*(2+vf) 
+00006530: 2920 2f20 2828 6566 2d65 6d29 2a28 312d  ) / ((ef-em)*(1-
+00006540: 7666 2920 2d20 332a 7666 2a65 6d29 0a20  vf) - 3*vf*em). 
+00006550: 2020 2023 2070 7269 6e74 2827 4520 696e     # print('E in
+00006560: 636c 7573 696f 6e27 2c65 696e 636c 7573  clusion',einclus
+00006570: 696f 6e29 0a20 2020 2064 6965 6c65 6376  ion).    dielecv
+00006580: 203d 2065 696e 636c 7573 696f 6e2a 6e70   = einclusion*np
+00006590: 2e65 7965 2833 290a 2020 2020 2320 7072  .eye(3).    # pr
+000065a0: 696e 7428 274e 6577 2064 6965 6c65 6376  int('New dielecv
+000065b0: 272c 6469 656c 6563 7629 0a20 2020 2023  ',dielecv).    #
+000065c0: 2064 6566 696e 6520 6920 6173 2061 2063   define i as a c
+000065d0: 6f6d 706c 6578 206e 756d 6265 720a 2020  omplex number.  
+000065e0: 2020 6920 3d20 636f 6d70 6c65 7828 302c    i = complex(0,
+000065f0: 3129 0a20 2020 2023 2057 6520 6e65 6564  1).    # We need
+00006600: 2074 6f20 7461 6b65 6e20 6163 636f 756e   to taken accoun
+00006610: 7420 6f66 2074 6865 2063 6861 6e67 6520  t of the change 
+00006620: 696e 2077 6176 656c 656e 6774 6820 616e  in wavelength an
+00006630: 6420 7468 6520 6368 616e 6765 2069 6e20  d the change in 
+00006640: 7369 7a65 2070 6172 616d 6574 6572 2064  size parameter d
+00006650: 7565 2074 6f20 7468 650a 2020 2020 2320  ue to the.    # 
+00006660: 4e6f 6e65 2075 6e69 7420 7661 6c75 6520  None unit value 
+00006670: 6f66 2074 6865 2064 6965 6c65 6374 7269  of the dielectri
+00006680: 6320 6f66 2074 6865 2065 6d62 6564 6469  c of the embeddi
+00006690: 6e67 206d 6564 6975 6d0a 2020 2020 2320  ng medium.    # 
+000066a0: 5468 6520 7369 7a65 2070 6172 616d 6574  The size paramet
+000066b0: 6572 2069 7320 3270 6920 7220 2f20 6c61  er is 2pi r / la
+000066c0: 6d62 6461 0a20 2020 2023 2054 6865 2065  mbda.    # The e
+000066d0: 6666 6563 7469 7665 206c 616d 6264 6120  ffective lambda 
+000066e0: 696e 2074 6865 2073 7570 706f 7274 696e  in the supportin
+000066f0: 6720 6d65 6469 756d 2069 7320 6c61 6d62  g medium is lamb
+00006700: 6461 202f 2073 7172 7428 656d 6564 6975  da / sqrt(emediu
+00006710: 6d29 0a20 2020 2023 2057 6865 7265 2074  m).    # Where t
+00006720: 6865 2072 6566 7261 6374 6976 6520 696e  he refractive in
+00006730: 6465 7820 6973 2074 616b 656e 2074 6f20  dex is taken to 
+00006740: 6265 2073 7172 7428 656d 6564 6975 6d29  be sqrt(emedium)
+00006750: 2028 6e6f 6e20 6d61 676e 6574 6963 206d   (non magnetic m
+00006760: 6174 6572 6961 6c73 290a 2020 2020 656d  aterials).    em
+00006770: 6564 6975 6d20 3d20 6e70 2e74 7261 6365  edium = np.trace
+00006780: 2864 6965 6c65 6374 7269 635f 6d65 6469  (dielectric_medi
+00006790: 756d 2920 2f20 332e 300a 2020 2020 7265  um) / 3.0.    re
+000067a0: 6672 6163 7469 7665 5f69 6e64 6578 5f6d  fractive_index_m
+000067b0: 6564 6975 6d20 3d20 6e70 2e72 6561 6c28  edium = np.real(
+000067c0: 6e70 2e73 7172 7428 656d 6564 6975 6d29  np.sqrt(emedium)
+000067d0: 290a 2020 2020 6c61 6d62 6461 5f76 6163  ).    lambda_vac
+000067e0: 7575 6d5f 6d75 203d 2032 202a 2050 4920  uum_mu = 2 * PI 
+000067f0: 2a20 7369 7a65 5f6d 7520 2f20 7369 7a65  * size_mu / size
+00006800: 0a20 2020 2077 6176 656c 656e 6774 685f  .    wavelength_
+00006810: 6e6d 203d 206c 616d 6264 615f 7661 6375  nm = lambda_vacu
+00006820: 756d 5f6d 7520 2a20 3130 3030 202f 2072  um_mu * 1000 / r
+00006830: 6566 7261 6374 6976 655f 696e 6465 785f  efractive_index_
+00006840: 6d65 6469 756d 0a20 2020 2072 6164 6975  medium.    radiu
+00006850: 735f 6e6d 203d 2073 697a 655f 6d75 202a  s_nm = size_mu *
+00006860: 2031 3030 300a 2020 2020 2320 5468 6520   1000.    # The 
+00006870: 7761 7665 7665 6374 6f72 2069 6e20 6e6d  wavevector in nm
+00006880: 2d31 0a20 2020 206b 5f6e 6d20 3d20 3220  -1.    k_nm = 2 
+00006890: 2a20 5049 202f 2077 6176 656c 656e 6774  * PI / wavelengt
+000068a0: 685f 6e6d 0a20 2020 2023 2076 6f6c 756d  h_nm.    # volum
+000068b0: 6520 6f66 2061 2070 6172 7469 636c 6520  e of a particle 
+000068c0: 696e 206e 6d5e 330a 2020 2020 565f 6e6d  in nm^3.    V_nm
+000068d0: 203d 2034 2e30 2f33 2e30 202a 2050 4920   = 4.0/3.0 * PI 
+000068e0: 2a20 7261 6469 7573 5f6e 6d20 2a20 7261  * radius_nm * ra
+000068f0: 6469 7573 5f6e 6d20 2a20 7261 6469 7573  dius_nm * radius
+00006900: 5f6e 6d0a 2020 2020 2320 4e75 6d62 6572  _nm.    # Number
+00006910: 2064 656e 7369 7479 206f 6620 7061 7274   density of part
+00006920: 6963 6c65 7320 286e 756d 6265 7220 2f20  icles (number / 
+00006930: 6e6d 5e33 290a 2020 2020 4e5f 6e6d 203d  nm^3).    N_nm =
+00006940: 2076 6620 2f20 565f 6e6d 0a20 2020 2023   vf / V_nm.    #
+00006950: 2049 6620 7468 6572 6520 6973 2061 2073   If there is a s
+00006960: 697a 6520 6469 7374 7269 6275 7469 6f6e  ize distribution
+00006970: 2073 6574 2075 7020 746f 2075 7365 2069   set up to use i
+00006980: 740a 2020 2020 6966 2073 697a 655f 6469  t.    if size_di
+00006990: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
+000069a0: 3a0a 2020 2020 2020 2020 6c6f 7765 722c  :.        lower,
+000069b0: 7570 7065 7220 3d20 6c6f 676e 6f72 6d2e  upper = lognorm.
+000069c0: 696e 7465 7276 616c 2830 2e39 3939 392c  interval(0.9999,
+000069d0: 7369 7a65 5f64 6973 7472 6962 7574 696f  size_distributio
+000069e0: 6e5f 7369 676d 612c 7363 616c 653d 7369  n_sigma,scale=si
+000069f0: 7a65 5f6d 7529 0a20 2020 2020 2020 206e  ze_mu).        n
+00006a00: 756d 6265 724f 6642 696e 7320 3d20 3430  umberOfBins = 40
+00006a10: 0a20 2020 2020 2020 2064 7020 3d20 6e70  .        dp = np
+00006a20: 2e6c 6f67 7370 6163 6528 6e70 2e6c 6f67  .logspace(np.log
+00006a30: 286c 6f77 6572 292c 6e70 2e6c 6f67 2875  (lower),np.log(u
+00006a40: 7070 6572 292c 6e75 6d62 6572 4f66 4269  pper),numberOfBi
+00006a50: 6e73 2c62 6173 653d 6e70 2e65 290a 2020  ns,base=np.e).  
+00006a60: 2020 2020 2020 2320 5468 6520 6465 6669        # The defi
+00006a70: 6e69 7469 6f6e 7320 7573 6564 2061 7265  nitions used are
+00006a80: 2063 6f6e 6675 7369 6e67 3b0a 2020 2020   confusing;.    
+00006a90: 2020 2020 2320 6470 2069 7320 7468 6520      # dp is the 
+00006aa0: 6c6f 6720 6f66 2074 6865 2076 6172 6961  log of the varia
+00006ab0: 626c 650a 2020 2020 2020 2020 2320 7320  ble.        # s 
+00006ac0: 6973 2074 6865 2073 7461 6e64 6172 6420  is the standard 
+00006ad0: 6465 7669 6174 696f 6e20 2873 6861 7065  deviation (shape
+00006ae0: 2066 756e 6374 696f 6e29 206f 6620 7468   function) of th
+00006af0: 6520 6c6f 6720 6f66 2074 6865 2076 6172  e log of the var
+00006b00: 6961 7465 0a20 2020 2020 2020 2023 2073  iate.        # s
+00006b10: 6361 6c65 2069 7320 7468 6520 6d65 616e  cale is the mean
+00006b20: 206f 6620 7468 6520 756e 6465 726c 7969   of the underlyi
+00006b30: 6e67 206e 6f72 6d61 6c20 6469 7374 7269  ng normal distri
+00006b40: 6275 7469 6f6e 0a20 2020 2020 2020 206e  bution.        n
+00006b50: 6470 203d 206c 6f67 6e6f 726d 2e70 6466  dp = lognorm.pdf
+00006b60: 2864 702c 733d 7369 7a65 5f64 6973 7472  (dp,s=size_distr
+00006b70: 6962 7574 696f 6e5f 7369 676d 612c 7363  ibution_sigma,sc
+00006b80: 616c 653d 7369 7a65 5f6d 7529 0a20 2020  ale=size_mu).   
+00006b90: 2020 2020 2023 7072 696e 7428 2244 5022       #print("DP"
+00006ba0: 2c64 7029 0a20 2020 2020 2020 2023 7072  ,dp).        #pr
+00006bb0: 696e 7428 224e 4450 222c 6e64 7029 0a20  int("NDP",ndp). 
+00006bc0: 2020 2020 2020 2023 7072 696e 7428 2255         #print("U
+00006bd0: 7070 6572 206c 6f77 6572 222c 6c6f 7765  pper lower",lowe
+00006be0: 722c 7570 7065 7229 0a20 2020 2020 2020  r,upper).       
+00006bf0: 2023 7072 696e 7428 2253 697a 655f 4d55   #print("Size_MU
+00006c00: 222c 7369 7a65 5f6d 7529 0a20 2020 2072  ",size_mu).    r
+00006c10: 6566 7261 6374 6976 655f 696e 6465 7820  efractive_index 
+00006c20: 3d20 6361 6c63 756c 6174 655f 7265 6672  = calculate_refr
+00006c30: 6163 7469 7665 5f69 6e64 6578 5f73 6361  active_index_sca
+00006c40: 6c61 7228 6569 6e63 6c75 7369 6f6e 2920  lar(einclusion) 
+00006c50: 2f20 7265 6672 6163 7469 7665 5f69 6e64  / refractive_ind
+00006c60: 6578 5f6d 6564 6975 6d0a 2020 2020 236a  ex_medium.    #j
+00006c70: 6b20 7072 696e 7428 2772 6566 7261 6374  k print('refract
+00006c80: 6976 655f 696e 6465 7827 2c20 7265 6672  ive_index', refr
+00006c90: 6163 7469 7665 5f69 6e64 6578 290a 2020  active_index).  
+00006ca0: 2020 236a 6b20 7072 696e 7428 2772 6566    #jk print('ref
+00006cb0: 7261 6374 6976 655f 696e 6465 785f 6d65  ractive_index_me
+00006cc0: 6469 756d 272c 2072 6566 7261 6374 6976  dium', refractiv
+00006cd0: 655f 696e 6465 785f 6d65 6469 756d 290a  e_index_medium).
+00006ce0: 2020 2020 236a 6b20 7072 696e 7428 2765      #jk print('e
+00006cf0: 696e 636c 7573 696f 6e27 2c20 6569 6e63  inclusion', einc
+00006d00: 6c75 7369 6f6e 290a 2020 2020 6966 2073  lusion).    if s
+00006d10: 697a 655f 6469 7374 7269 6275 7469 6f6e  ize_distribution
+00006d20: 5f73 6967 6d61 3a0a 2020 2020 2020 2020  _sigma:.        
+00006d30: 2320 4361 6c63 756c 6174 6520 7468 6520  # Calculate the 
+00006d40: 696e 7465 6772 616c 206f 6620 7468 6520  integral of the 
+00006d50: 666f 7277 6172 6420 7363 6174 7465 7269  forward scatteri
+00006d60: 6e67 2066 6163 746f 7273 206f 7665 7220  ng factors over 
+00006d70: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
+00006d80: 0a20 2020 2020 2020 2073 315f 6661 6374  .        s1_fact
+00006d90: 6f72 7320 3d20 5b5d 0a20 2020 2020 2020  ors = [].       
+00006da0: 2066 6f72 2072 2069 6e20 6470 3a0a 2020   for r in dp:.  
+00006db0: 2020 2020 2020 2020 2020 2320 5468 6520            # The 
+00006dc0: 7369 7a65 2070 6172 616d 6574 6572 2069  size parameter i
+00006dd0: 7320 3270 6920 7220 2f20 6c61 6d62 6461  s 2pi r / lambda
+00006de0: 0a20 2020 2020 2020 2020 2020 2078 203d  .            x =
+00006df0: 2032 202a 2050 4920 2a20 7220 2f20 6c61   2 * PI * r / la
+00006e00: 6d62 6461 5f76 6163 7575 6d5f 6d75 0a20  mbda_vacuum_mu. 
+00006e10: 2020 2020 2020 2020 2020 2023 2043 616c             # Cal
+00006e20: 6375 6c61 7465 2074 6865 2053 3120 616e  culate the S1 an
+00006e30: 6420 5332 2073 6361 7474 6572 696e 6720  d S2 scattering 
+00006e40: 6661 6374 6f72 732c 2061 6e64 2073 746f  factors, and sto
+00006e50: 7265 2069 6e20 6120 6c69 7374 0a20 2020  re in a list.   
+00006e60: 2020 2020 2020 2020 2073 312c 7332 203d           s1,s2 =
+00006e70: 204d 6965 2e4d 6965 5331 5332 2872 6566   Mie.MieS1S2(ref
+00006e80: 7261 6374 6976 655f 696e 6465 782c 2078  ractive_index, x
+00006e90: 2a72 6566 7261 6374 6976 655f 696e 6465  *refractive_inde
+00006ea0: 785f 6d65 6469 756d 2c20 3129 0a20 2020  x_medium, 1).   
+00006eb0: 2020 2020 2020 2020 2073 315f 6661 6374           s1_fact
+00006ec0: 6f72 732e 6170 7065 6e64 2873 3129 0a20  ors.append(s1). 
+00006ed0: 2020 2020 2020 2023 204e 6f77 2069 6e74         # Now int
+00006ee0: 6567 7261 7465 0a20 2020 2020 2020 2073  egrate.        s
+00006ef0: 3120 3d20 7472 6170 7a28 7331 5f66 6163  1 = trapz(s1_fac
+00006f00: 746f 7273 2a6e 6470 2c64 7029 0a20 2020  tors*ndp,dp).   
+00006f10: 2020 2020 206e 6f72 6d61 6c20 3d20 7472       normal = tr
+00006f20: 6170 7a28 6e64 702c 6470 290a 2020 2020  apz(ndp,dp).    
+00006f30: 2020 2020 236d 6561 6e20 3d20 7472 6170      #mean = trap
+00006f40: 7a28 6e64 702a 6470 2c64 7029 0a20 2020  z(ndp*dp,dp).   
+00006f50: 2020 2020 2023 7472 7565 5f6d 6561 6e20       #true_mean 
+00006f60: 3d20 6e70 2e65 7870 2820 6e70 2e6c 6f67  = np.exp( np.log
+00006f70: 2873 697a 655f 6d75 2920 2b20 7369 7a65  (size_mu) + size
+00006f80: 5f64 6973 7472 6962 7574 696f 6e5f 7369  _distribution_si
+00006f90: 676d 612a 7369 7a65 5f64 6973 7472 6962  gma*size_distrib
+00006fa0: 7574 696f 6e5f 7369 676d 612f 322e 3029  ution_sigma/2.0)
+00006fb0: 0a20 2020 2020 2020 2023 765f 636d 3120  .        #v_cm1 
+00006fc0: 3d20 312e 3045 342f 6c61 6d62 6461 5f76  = 1.0E4/lambda_v
+00006fd0: 6163 7575 6d5f 6d75 0a20 2020 2020 2020  acuum_mu.       
+00006fe0: 2023 7072 696e 7428 2246 7265 7175 656e   #print("Frequen
+00006ff0: 6379 2c6e 6f72 6d61 6c2c 6d65 616e 222c  cy,normal,mean",
+00007000: 765f 636d 312c 6e6f 726d 616c 2c74 7275  v_cm1,normal,tru
+00007010: 655f 6d65 616e 2c6d 6561 6e29 0a20 2020  e_mean,mean).   
+00007020: 2020 2020 2069 6620 6e70 2e61 6273 286e       if np.abs(n
+00007030: 6f72 6d61 6c20 2d20 312e 3029 203e 2031  ormal - 1.0) > 1
+00007040: 2e30 452d 323a 0a20 2020 2020 2020 2020  .0E-2:.         
+00007050: 2020 2070 7269 6e74 2822 5761 726e 696e     print("Warnin
+00007060: 6720 696e 7465 6772 6174 696f 6e20 6f66  g integration of
+00007070: 206c 6f67 2d6e 6f72 6d61 6c20 6469 7374   log-normal dist
+00007080: 7269 6275 7469 6f6e 2069 6e20 6572 726f  ribution in erro
+00007090: 7222 2c20 6e6f 726d 616c 290a 2020 2020  r", normal).    
+000070a0: 2020 2020 2020 2020 7072 696e 7428 2253          print("S
+000070b0: 746f 7070 696e 6720 6361 6c63 756c 6174  topping calculat
+000070c0: 696f 6e20 2d20 6c69 6b65 6c79 2070 726f  ion - likely pro
+000070d0: 626c 656d 2069 7320 746f 6f20 6c61 7267  blem is too larg
+000070e0: 6520 6120 7369 676d 6120 666f 7220 6c6f  e a sigma for lo
+000070f0: 672d 6e6f 726d 616c 2064 6973 7472 6962  g-normal distrib
+00007100: 7574 696f 6e22 290a 2020 2020 2020 2020  ution").        
+00007110: 2020 2020 6566 6664 6965 6c65 6320 3d20      effdielec = 
+00007120: 6e70 2e61 7272 6179 285b 5b31 2c20 302c  np.array([[1, 0,
+00007130: 2030 5d2c 205b 302c 2031 2c20 305d 2c20   0], [0, 1, 0], 
+00007140: 5b30 2c20 302c 2031 5d5d 290a 2020 2020  [0, 0, 1]]).    
+00007150: 2020 2020 2020 2020 7265 7475 726e 2065          return e
+00007160: 6666 6469 656c 6563 0a20 2020 2065 6c73  ffdielec.    els
+00007170: 653a 0a20 2020 2020 2020 2023 2043 616c  e:.        # Cal
+00007180: 6375 6c61 7465 2074 6865 2073 6361 7474  culate the scatt
+00007190: 6572 696e 6720 6661 6374 6f72 7320 6174  ering factors at
+000071a0: 2030 2064 6567 7265 6573 0a20 2020 2020   0 degrees.     
+000071b0: 2020 2023 6a6b 2070 7269 6e74 2822 7265     #jk print("re
+000071c0: 6672 6163 7469 7665 5f69 6e64 6578 2c20  fractive_index, 
+000071d0: 7369 7a65 2c20 7265 6672 6163 7469 7665  size, refractive
+000071e0: 5f69 6e64 6578 5f6d 6564 6975 6d22 2c20  _index_medium", 
+000071f0: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
+00007200: 2c20 7369 7a65 2c20 7265 6672 6163 7469  , size, refracti
+00007210: 7665 5f69 6e64 6578 5f6d 6564 6975 6d29  ve_index_medium)
+00007220: 0a20 2020 2020 2020 2073 312c 7332 203d  .        s1,s2 =
+00007230: 204d 6965 2e4d 6965 5331 5332 2872 6566   Mie.MieS1S2(ref
+00007240: 7261 6374 6976 655f 696e 6465 782c 2073  ractive_index, s
+00007250: 697a 652a 7265 6672 6163 7469 7665 5f69  ize*refractive_i
+00007260: 6e64 6578 5f6d 6564 6975 6d2c 2031 290a  ndex_medium, 1).
+00007270: 2020 2020 2320 5365 6520 7661 6e20 6465      # See van de
+00007280: 2048 756c 7374 2070 6167 6520 3132 392c   Hulst page 129,
+00007290: 2031 3330 0a20 2020 2023 2052 6566 7261   130.    # Refra
+000072a0: 6374 6976 6520 696e 6465 7820 6f66 206d  ctive index of m
+000072b0: 6174 6572 6961 6c20 6973 0a20 2020 2023  aterial is.    #
+000072c0: 2074 6865 2073 6967 6e20 6f66 2074 6865   the sign of the
+000072d0: 2069 6d61 6769 6e61 7279 2063 6f6d 706f   imaginary compo
+000072e0: 6e65 6e74 2068 6173 2063 6861 6e67 6564  nent has changed
+000072f0: 2066 6f72 2063 6f6d 7061 7469 6269 6c69   for compatibili
+00007300: 7479 2077 6974 6820 4d47 2f42 7275 6767  ty with MG/Brugg
+00007310: 656d 616e 0a20 2020 2072 6566 7261 6374  eman.    refract
+00007320: 6976 655f 696e 6465 7820 3d20 7265 6672  ive_index = refr
+00007330: 6163 7469 7665 5f69 6e64 6578 5f6d 6564  active_index_med
+00007340: 6975 6d20 2a20 2820 312e 3020 2b20 6920  ium * ( 1.0 + i 
+00007350: 2a20 7331 202a 2032 202a 2050 4920 2a20  * s1 * 2 * PI * 
+00007360: 4e5f 6e6d 202f 2028 206b 5f6e 6d20 2a20  N_nm / ( k_nm * 
+00007370: 6b5f 6e6d 202a 206b 5f6e 6d20 2920 290a  k_nm * k_nm ) ).
+00007380: 2020 2020 6566 6620 3d20 7265 6672 6163      eff = refrac
+00007390: 7469 7665 5f69 6e64 6578 202a 2072 6566  tive_index * ref
+000073a0: 7261 6374 6976 655f 696e 6465 780a 2020  ractive_index.  
+000073b0: 2020 6566 6664 6965 6c65 6320 3d20 6e70    effdielec = np
+000073c0: 2e61 7272 6179 285b 5b65 6666 2c20 302c  .array([[eff, 0,
+000073d0: 2030 5d2c 205b 302c 2065 6666 2c20 305d   0], [0, eff, 0]
+000073e0: 2c20 5b30 2c20 302c 2065 6666 5d5d 290a  , [0, 0, eff]]).
+000073f0: 2020 2020 236a 6b20 7072 696e 7428 7261      #jk print(ra
+00007400: 6469 7573 5f6e 6d2c 206c 616d 6264 615f  dius_nm, lambda_
+00007410: 7661 6375 756d 5f6d 752a 3130 3030 2e30  vacuum_mu*1000.0
+00007420: 2c20 7165 7874 2c71 7363 612c 7161 6273  , qext,qsca,qabs
+00007430: 2c67 2c71 7072 2c71 6261 636b 2c71 7261  ,g,qpr,qback,qra
+00007440: 7469 6f2c 6e70 2e72 6561 6c28 7331 292c  tio,np.real(s1),
+00007450: 6e70 2e69 6d61 6728 7331 292c 6e70 2e72  np.imag(s1),np.r
+00007460: 6561 6c28 7265 6672 6163 7469 7665 5f69  eal(refractive_i
+00007470: 6e64 6578 292c 6e70 2e69 6d61 6728 7265  ndex),np.imag(re
+00007480: 6672 6163 7469 7665 5f69 6e64 6578 292c  fractive_index),
+00007490: 6e70 2e72 6561 6c28 6566 6629 2c6e 702e  np.real(eff),np.
+000074a0: 696d 6167 2865 6666 2929 0a20 2020 2023  imag(eff)).    #
+000074b0: 7072 696e 7420 2822 7261 6469 7573 5f6e  print ("radius_n
+000074c0: 6d2c 2065 6666 222c 2072 6164 6975 735f  m, eff", radius_
+000074d0: 6e6d 2c20 6566 6629 0a20 2020 2072 6574  nm, eff).    ret
+000074e0: 7572 6e20 6566 6664 6965 6c65 630a 0a64  urn effdielec..d
+000074f0: 6566 2061 6e69 736f 7472 6f70 6963 5f6d  ef anisotropic_m
+00007500: 6965 5f73 6361 7474 6572 696e 6728 6469  ie_scattering(di
+00007510: 656c 6563 7472 6963 5f6d 6564 6975 6d2c  electric_medium,
+00007520: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
+00007530: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
+00007540: 2076 662c 2073 697a 652c 2073 697a 655f   vf, size, size_
+00007550: 6d75 2c20 7369 7a65 5f64 6973 7472 6962  mu, size_distrib
+00007560: 7574 696f 6e5f 7369 676d 6129 3a0a 2020  ution_sigma):.  
+00007570: 2020 2222 2243 616c 6375 6c61 7465 2074    """Calculate t
+00007580: 6865 2065 6666 6563 7469 7665 2063 6f6e  he effective con
+00007590: 7374 616e 7420 7065 726d 6974 7469 7669  stant permittivi
+000075a0: 7479 2075 7369 6e67 2061 204d 6965 2073  ty using a Mie s
+000075b0: 6361 7474 6572 696e 6720 6170 7072 6f61  cattering approa
+000075c0: 6368 0a20 2020 2020 2020 6469 656c 6563  ch.       dielec
+000075d0: 7472 6963 5f6d 6564 6975 6d20 6973 2074  tric_medium is t
+000075e0: 6865 2064 6965 6c65 6374 7269 6320 636f  he dielectric co
+000075f0: 6e73 7461 6e74 2074 656e 736f 7220 6f66  nstant tensor of
+00007600: 2074 6865 206d 6564 6975 6d0a 2020 2020   the medium.    
+00007610: 2020 2063 7279 7374 616c 5f70 6572 6d69     crystal_permi
+00007620: 7474 6976 6974 7920 6973 2074 6865 2074  ttivity is the t
+00007630: 6f74 616c 2066 7265 7175 656e 6379 2064  otal frequency d
+00007640: 6965 6c65 6374 7269 6320 636f 6e73 7461  ielectric consta
+00007650: 6e74 2074 656e 736f 7220 6174 2074 6865  nt tensor at the
+00007660: 2063 7572 7265 6e74 2066 7265 7175 656e   current frequen
+00007670: 6379 0a20 2020 2020 2020 7368 6170 6520  cy.       shape 
+00007680: 6973 2074 6865 206e 616d 6520 6f66 2074  is the name of t
+00007690: 6865 2063 7572 7265 6e74 2073 6861 7065  he current shape
+000076a0: 2028 4e4f 5420 5553 4544 290a 2020 2020   (NOT USED).    
+000076b0: 2020 204c 2069 7320 7468 6520 7368 6170     L is the shap
+000076c0: 6573 2064 6570 6f6c 6172 6973 6174 696f  es depolarisatio
+000076d0: 6e20 6d61 7472 6978 2028 4e4f 5420 5553  n matrix (NOT US
+000076e0: 4544 290a 2020 2020 2020 2073 697a 6520  ED).       size 
+000076f0: 6973 2074 6865 2064 696d 656e 7369 6f6e  is the dimension
+00007700: 6c65 7373 2073 697a 6520 7061 7261 6d65  less size parame
+00007710: 7465 7220 666f 7220 7468 6520 6672 6571  ter for the freq
+00007720: 7565 6e63 7920 756e 6465 7220 636f 6e73  uency under cons
+00007730: 6964 6572 6174 696f 6e0a 2020 2020 2020  ideration.      
+00007740: 2073 697a 655f 6469 7374 7269 6275 7469   size_distributi
+00007750: 6f6e 5f73 6967 6d61 2069 7320 7468 6520  on_sigma is the 
+00007760: 6c6f 6720 6e6f 726d 616c 2076 616c 7565  log normal value
+00007770: 206f 6620 7369 676d 610a 2020 2020 2020   of sigma.      
+00007780: 2076 6620 6973 2074 6865 2076 6f6c 756d   vf is the volum
+00007790: 6520 6672 6163 7469 6f6e 206f 6620 6669  e fraction of fi
+000077a0: 6c6c 6572 0a20 2020 2020 2020 4d69 6520  ller.       Mie 
+000077b0: 6f6e 6c79 2077 6f72 6b73 2066 6f72 2073  only works for s
+000077c0: 7068 6572 6963 616c 2070 6172 7469 636c  pherical particl
+000077d0: 6573 2c20 736f 2073 6861 7065 2c20 616e  es, so shape, an
+000077e0: 6420 4c20 7061 7261 6d65 7465 7273 2061  d L parameters a
+000077f0: 7265 2069 676e 6f72 6564 0a20 2020 2020  re ignored.     
+00007800: 2020 5468 6520 726f 7574 696e 6520 7265    The routine re
+00007810: 7475 726e 7320 7468 6520 6566 6665 6374  turns the effect
+00007820: 6976 6520 6469 656c 6563 7472 6963 2063  ive dielectric c
+00007830: 6f6e 7374 616e 7422 2222 0a20 2020 2023  onstant""".    #
+00007840: 2064 6566 696e 6520 6920 6173 2061 2063   define i as a c
+00007850: 6f6d 706c 6578 206e 756d 6265 720a 2020  omplex number.  
+00007860: 2020 6920 3d20 636f 6d70 6c65 7828 302c    i = complex(0,
+00007870: 3129 0a20 2020 2023 2057 6520 6e65 6564  1).    # We need
+00007880: 2074 6f20 7461 6b65 6e20 6163 636f 756e   to taken accoun
+00007890: 7420 6f66 2074 6865 2063 6861 6e67 6520  t of the change 
+000078a0: 696e 2077 6176 656c 656e 6774 6820 616e  in wavelength an
+000078b0: 6420 7468 6520 6368 616e 6765 2069 6e20  d the change in 
+000078c0: 7369 7a65 2070 6172 616d 6574 6572 2064  size parameter d
+000078d0: 7565 2074 6f20 7468 650a 2020 2020 2320  ue to the.    # 
+000078e0: 4e6f 6e65 2075 6e69 7420 7661 6c75 6520  None unit value 
+000078f0: 6f66 2074 6865 2064 6965 6c65 6374 7269  of the dielectri
+00007900: 6320 6f66 2074 6865 2065 6d62 6564 6469  c of the embeddi
+00007910: 6e67 206d 6564 6975 6d0a 2020 2020 2320  ng medium.    # 
+00007920: 5468 6520 7369 7a65 2070 6172 616d 6574  The size paramet
+00007930: 6572 2069 7320 3270 6920 7220 2f20 6c61  er is 2pi r / la
+00007940: 6d62 6461 0a20 2020 2023 2054 6865 2065  mbda.    # The e
+00007950: 6666 6563 7469 7665 206c 616d 6264 6120  ffective lambda 
+00007960: 696e 2074 6865 2073 7570 706f 7274 696e  in the supportin
+00007970: 6720 6d65 6469 756d 2069 7320 6c61 6d62  g medium is lamb
+00007980: 6461 202f 2073 7172 7428 656d 6564 6975  da / sqrt(emediu
+00007990: 6d29 0a20 2020 2023 2057 6865 7265 2074  m).    # Where t
+000079a0: 6865 2072 6566 7261 6374 6976 6520 696e  he refractive in
+000079b0: 6465 7820 6973 2074 616b 656e 2074 6f20  dex is taken to 
+000079c0: 6265 2073 7172 7428 656d 6564 6975 6d29  be sqrt(emedium)
+000079d0: 2028 6e6f 6e20 6d61 676e 6574 6963 206d   (non magnetic m
+000079e0: 6174 6572 6961 6c73 290a 2020 2020 656d  aterials).    em
+000079f0: 6564 6975 6d20 3d20 6e70 2e74 7261 6365  edium = np.trace
+00007a00: 2864 6965 6c65 6374 7269 635f 6d65 6469  (dielectric_medi
+00007a10: 756d 2920 2f20 332e 300a 2020 2020 7265  um) / 3.0.    re
+00007a20: 6672 6163 7469 7665 5f69 6e64 6578 5f6d  fractive_index_m
+00007a30: 6564 6975 6d20 3d20 6e70 2e72 6561 6c28  edium = np.real(
+00007a40: 6e70 2e73 7172 7428 656d 6564 6975 6d29  np.sqrt(emedium)
+00007a50: 290a 2020 2020 6c61 6d62 6461 5f76 6163  ).    lambda_vac
+00007a60: 7575 6d5f 6d75 203d 2032 202a 2050 4920  uum_mu = 2 * PI 
+00007a70: 2a20 7369 7a65 5f6d 7520 2f20 7369 7a65  * size_mu / size
+00007a80: 0a20 2020 2077 6176 656c 656e 6774 685f  .    wavelength_
+00007a90: 6e6d 203d 206c 616d 6264 615f 7661 6375  nm = lambda_vacu
+00007aa0: 756d 5f6d 7520 2a20 3130 3030 202f 2072  um_mu * 1000 / r
+00007ab0: 6566 7261 6374 6976 655f 696e 6465 785f  efractive_index_
+00007ac0: 6d65 6469 756d 0a20 2020 2072 6164 6975  medium.    radiu
+00007ad0: 735f 6e6d 203d 2073 697a 655f 6d75 202a  s_nm = size_mu *
+00007ae0: 2031 3030 300a 2020 2020 2320 546f 2061   1000.    # To a
+00007af0: 6363 6f75 6e74 2066 6f72 2061 6e69 736f  ccount for aniso
+00007b00: 7472 6f70 7920 7765 2064 6961 676f 6e61  tropy we diagona
+00007b10: 6c69 7365 2074 6865 2072 6561 6c20 7061  lise the real pa
+00007b20: 7274 206f 6620 7468 6520 6469 656c 6563  rt of the dielec
+00007b30: 7472 6963 206d 6174 7269 7820 616e 6420  tric matrix and 
+00007b40: 7472 616e 7366 6f72 6d0a 2020 2020 2320  transform.    # 
+00007b50: 7468 6520 6675 6c6c 206d 6174 7269 7820  the full matrix 
+00007b60: 7769 7468 2074 6865 2065 6967 656e 7665  with the eigenve
+00007b70: 6374 6f72 732c 2055 0a20 2020 2023 2046  ctors, U.    # F
+00007b80: 696e 6420 5520 616e 6420 452c 2073 7563  ind U and E, suc
+00007b90: 6820 7468 6174 2055 542e 2044 2e20 5520  h that UT. D. U 
+00007ba0: 3d20 4520 2877 6865 7265 2044 2069 7320  = E (where D is 
+00007bb0: 7468 6520 7265 616c 2070 6172 7420 6f66  the real part of
+00007bc0: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
+00007bd0: 6976 6974 7929 0a20 2020 2045 2c55 203d  ivity).    E,U =
+00007be0: 206e 702e 6c69 6e61 6c67 2e65 6967 286e   np.linalg.eig(n
+00007bf0: 702e 7265 616c 2863 7279 7374 616c 5f70  p.real(crystal_p
+00007c00: 6572 6d69 7474 6976 6974 7929 290a 2020  ermittivity)).  
+00007c10: 2020 2320 5472 616e 7366 6f72 6d20 7468    # Transform th
+00007c20: 6520 6675 6c6c 2064 6965 6c65 6374 7269  e full dielectri
+00007c30: 6320 6d61 7472 6978 0a20 2020 2072 6f74  c matrix.    rot
+00007c40: 6174 6564 5f64 6965 6c65 6320 3d20 6e70  ated_dielec = np
+00007c50: 2e6d 6174 6d75 6c28 552e 542c 6e70 2e6d  .matmul(U.T,np.m
+00007c60: 6174 6d75 6c28 6372 7973 7461 6c5f 7065  atmul(crystal_pe
+00007c70: 726d 6974 7469 7669 7479 2c55 2929 0a20  rmittivity,U)). 
+00007c80: 2020 2023 2054 6865 2077 6176 6576 6563     # The wavevec
+00007c90: 746f 7220 696e 206e 6d2d 310a 2020 2020  tor in nm-1.    
+00007ca0: 6b5f 6e6d 203d 2032 202a 2050 4920 2f20  k_nm = 2 * PI / 
+00007cb0: 7761 7665 6c65 6e67 7468 5f6e 6d0a 2020  wavelength_nm.  
+00007cc0: 2020 2320 766f 6c75 6d65 206f 6620 6120    # volume of a 
+00007cd0: 7061 7274 6963 6c65 2069 6e20 6e6d 5e33  particle in nm^3
+00007ce0: 0a20 2020 2056 5f6e 6d20 3d20 342e 302f  .    V_nm = 4.0/
+00007cf0: 332e 3020 2a20 5049 202a 2072 6164 6975  3.0 * PI * radiu
+00007d00: 735f 6e6d 202a 2072 6164 6975 735f 6e6d  s_nm * radius_nm
+00007d10: 202a 2072 6164 6975 735f 6e6d 0a20 2020   * radius_nm.   
+00007d20: 2023 204e 756d 6265 7220 6465 6e73 6974   # Number densit
+00007d30: 7920 6f66 2070 6172 7469 636c 6573 2028  y of particles (
+00007d40: 6e75 6d62 6572 202f 206e 6d5e 3329 0a20  number / nm^3). 
+00007d50: 2020 204e 5f6e 6d20 3d20 7666 202f 2056     N_nm = vf / V
+00007d60: 5f6e 6d0a 2020 2020 2320 4966 2074 6865  _nm.    # If the
+00007d70: 7265 2069 7320 6120 7369 7a65 2064 6973  re is a size dis
+00007d80: 7472 6962 7574 696f 6e20 7365 7420 7570  tribution set up
+00007d90: 2074 6f20 7573 6520 6974 0a20 2020 2069   to use it.    i
+00007da0: 6620 7369 7a65 5f64 6973 7472 6962 7574  f size_distribut
+00007db0: 696f 6e5f 7369 676d 613a 0a20 2020 2020  ion_sigma:.     
+00007dc0: 2020 206c 6f77 6572 2c75 7070 6572 203d     lower,upper =
+00007dd0: 206c 6f67 6e6f 726d 2e69 6e74 6572 7661   lognorm.interva
+00007de0: 6c28 302e 3939 3939 2c73 697a 655f 6469  l(0.9999,size_di
+00007df0: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
+00007e00: 2c73 6361 6c65 3d73 697a 655f 6d75 290a  ,scale=size_mu).
+00007e10: 2020 2020 2020 2020 6e75 6d62 6572 4f66          numberOf
+00007e20: 4269 6e73 203d 2034 300a 2020 2020 2020  Bins = 40.      
+00007e30: 2020 6470 203d 206e 702e 6c6f 6773 7061    dp = np.logspa
+00007e40: 6365 286e 702e 6c6f 6728 6c6f 7765 7229  ce(np.log(lower)
+00007e50: 2c6e 702e 6c6f 6728 7570 7065 7229 2c6e  ,np.log(upper),n
+00007e60: 756d 6265 724f 6642 696e 732c 6261 7365  umberOfBins,base
+00007e70: 3d6e 702e 6529 0a20 2020 2020 2020 2023  =np.e).        #
+00007e80: 2054 6865 2064 6566 696e 6974 696f 6e73   The definitions
+00007e90: 2075 7365 6420 6172 6520 636f 6e66 7573   used are confus
+00007ea0: 696e 673b 0a20 2020 2020 2020 2023 2064  ing;.        # d
+00007eb0: 7020 6973 2074 6865 206c 6f67 206f 6620  p is the log of 
+00007ec0: 7468 6520 7661 7269 6162 6c65 0a20 2020  the variable.   
+00007ed0: 2020 2020 2023 2073 2069 7320 7468 6520       # s is the 
+00007ee0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+00007ef0: 6f6e 2028 7368 6170 6520 6675 6e63 7469  on (shape functi
+00007f00: 6f6e 2920 6f66 2074 6865 206c 6f67 206f  on) of the log o
+00007f10: 6620 7468 6520 7661 7269 6174 650a 2020  f the variate.  
+00007f20: 2020 2020 2020 2320 7363 616c 6520 6973        # scale is
+00007f30: 2074 6865 206d 6561 6e20 6f66 2074 6865   the mean of the
+00007f40: 2075 6e64 6572 6c79 696e 6720 6e6f 726d   underlying norm
+00007f50: 616c 2064 6973 7472 6962 7574 696f 6e0a  al distribution.
+00007f60: 2020 2020 2020 2020 6e64 7020 3d20 6c6f          ndp = lo
+00007f70: 676e 6f72 6d2e 7064 6628 6470 2c73 3d73  gnorm.pdf(dp,s=s
+00007f80: 697a 655f 6469 7374 7269 6275 7469 6f6e  ize_distribution
+00007f90: 5f73 6967 6d61 2c73 6361 6c65 3d73 697a  _sigma,scale=siz
+00007fa0: 655f 6d75 290a 2020 2020 2020 2020 2370  e_mu).        #p
+00007fb0: 7269 6e74 2822 4450 222c 6470 290a 2020  rint("DP",dp).  
+00007fc0: 2020 2020 2020 2370 7269 6e74 2822 4e44        #print("ND
+00007fd0: 5022 2c6e 6470 290a 2020 2020 2020 2020  P",ndp).        
+00007fe0: 2370 7269 6e74 2822 5570 7065 7220 6c6f  #print("Upper lo
+00007ff0: 7765 7222 2c6c 6f77 6572 2c75 7070 6572  wer",lower,upper
+00008000: 290a 2020 2020 2020 2020 2370 7269 6e74  ).        #print
+00008010: 2822 5369 7a65 5f4d 5522 2c73 697a 655f  ("Size_MU",size_
+00008020: 6d75 290a 2020 2020 2320 5765 2061 7265  mu).    # We are
+00008030: 206e 6f77 2067 6f69 6e67 2074 6f20 6967   now going to ig
+00008040: 6e6f 7265 2061 6e79 206f 6666 2d64 6961  nore any off-dia
+00008050: 676f 6e61 6c20 656c 656d 656e 7473 0a20  gonal elements. 
+00008060: 2020 2074 7261 6365 203d 2030 2e30 0a20     trace = 0.0. 
+00008070: 2020 2023 204e 6f77 2074 616b 6520 7468     # Now take th
+00008080: 6520 6176 6572 6167 6520 6f66 2065 6163  e average of eac
+00008090: 6820 6469 7265 6374 696f 6e0a 2020 2020  h direction.    
+000080a0: 666f 7220 696e 6465 7820 696e 205b 302c  for index in [0,
+000080b0: 312c 325d 3a0a 2020 2020 2020 2020 7265  1,2]:.        re
+000080c0: 6672 6163 7469 7665 5f69 6e64 6578 203d  fractive_index =
+000080d0: 2063 616c 6375 6c61 7465 5f72 6566 7261   calculate_refra
+000080e0: 6374 6976 655f 696e 6465 785f 7363 616c  ctive_index_scal
+000080f0: 6172 2872 6f74 6174 6564 5f64 6965 6c65  ar(rotated_diele
+00008100: 635b 696e 6465 782c 696e 6465 785d 2920  c[index,index]) 
+00008110: 2f20 7265 6672 6163 7469 7665 5f69 6e64  / refractive_ind
+00008120: 6578 5f6d 6564 6975 6d0a 2020 2020 2020  ex_medium.      
+00008130: 2020 236a 6b20 7072 696e 7428 2772 6566    #jk print('ref
+00008140: 7261 6374 6976 655f 696e 6465 7827 2c20  ractive_index', 
+00008150: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
+00008160: 290a 2020 2020 2020 2020 236a 6b20 7072  ).        #jk pr
+00008170: 696e 7428 2772 6566 7261 6374 6976 655f  int('refractive_
+00008180: 696e 6465 785f 6d65 6469 756d 272c 2072  index_medium', r
+00008190: 6566 7261 6374 6976 655f 696e 6465 785f  efractive_index_
+000081a0: 6d65 6469 756d 290a 2020 2020 2020 2020  medium).        
+000081b0: 236a 6b20 7072 696e 7428 2772 6f74 6174  #jk print('rotat
+000081c0: 6564 5f64 6965 6c65 6327 2c20 726f 7461  ed_dielec', rota
+000081d0: 7465 645f 6469 656c 6563 5b69 6e64 6578  ted_dielec[index
+000081e0: 2c69 6e64 6578 5d29 0a20 2020 2020 2020  ,index]).       
+000081f0: 2069 6620 7369 7a65 5f64 6973 7472 6962   if size_distrib
+00008200: 7574 696f 6e5f 7369 676d 613a 0a20 2020  ution_sigma:.   
+00008210: 2020 2020 2020 2020 2023 2043 616c 6375           # Calcu
+00008220: 6c61 7465 2074 6865 2069 6e74 6567 7261  late the integra
+00008230: 6c20 6f66 2074 6865 2066 6f72 7761 7264  l of the forward
+00008240: 2073 6361 7474 6572 696e 6720 6661 6374   scattering fact
+00008250: 6f72 7320 6f76 6572 2074 6865 2064 6973  ors over the dis
+00008260: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
+00008270: 2020 2020 2020 7331 5f66 6163 746f 7273        s1_factors
+00008280: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+00008290: 2020 666f 7220 7220 696e 2064 703a 0a20    for r in dp:. 
+000082a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000082b0: 2054 6865 2073 697a 6520 7061 7261 6d65   The size parame
+000082c0: 7465 7220 6973 2032 7069 2072 202f 206c  ter is 2pi r / l
+000082d0: 616d 6264 610a 2020 2020 2020 2020 2020  ambda.          
+000082e0: 2020 2020 2020 7820 3d20 3220 2a20 5049        x = 2 * PI
+000082f0: 202a 2072 202f 206c 616d 6264 615f 7661   * r / lambda_va
+00008300: 6375 756d 5f6d 750a 2020 2020 2020 2020  cuum_mu.        
+00008310: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
+00008320: 6174 6520 7468 6520 5331 2061 6e64 2053  ate the S1 and S
+00008330: 3220 7363 6174 7465 7269 6e67 2066 6163  2 scattering fac
+00008340: 746f 7273 2c20 616e 6420 7374 6f72 6520  tors, and store 
+00008350: 696e 2061 206c 6973 740a 2020 2020 2020  in a list.      
+00008360: 2020 2020 2020 2020 2020 7331 2c73 3220            s1,s2 
+00008370: 3d20 4d69 652e 4d69 6553 3153 3228 7265  = Mie.MieS1S2(re
+00008380: 6672 6163 7469 7665 5f69 6e64 6578 2c20  fractive_index, 
+00008390: 782a 7265 6672 6163 7469 7665 5f69 6e64  x*refractive_ind
+000083a0: 6578 5f6d 6564 6975 6d2c 2031 290a 2020  ex_medium, 1).  
+000083b0: 2020 2020 2020 2020 2020 2020 2020 7331                s1
+000083c0: 5f66 6163 746f 7273 2e61 7070 656e 6428  _factors.append(
+000083d0: 7331 290a 2020 2020 2020 2020 2020 2020  s1).            
+000083e0: 2320 4e6f 7720 696e 7465 6772 6174 650a  # Now integrate.
+000083f0: 2020 2020 2020 2020 2020 2020 7331 203d              s1 =
+00008400: 2074 7261 707a 2873 315f 6661 6374 6f72   trapz(s1_factor
+00008410: 732a 6e64 702c 6470 290a 2020 2020 2020  s*ndp,dp).      
+00008420: 2020 2020 2020 6e6f 726d 616c 203d 2074        normal = t
+00008430: 7261 707a 286e 6470 2c64 7029 0a20 2020  rapz(ndp,dp).   
+00008440: 2020 2020 2020 2020 2023 6d65 616e 203d           #mean =
+00008450: 2074 7261 707a 286e 6470 2a64 702c 6470   trapz(ndp*dp,dp
+00008460: 290a 2020 2020 2020 2020 2020 2020 2374  ).            #t
+00008470: 7275 655f 6d65 616e 203d 206e 702e 6578  rue_mean = np.ex
+00008480: 7028 206e 702e 6c6f 6728 7369 7a65 5f6d  p( np.log(size_m
+00008490: 7529 202b 2073 697a 655f 6469 7374 7269  u) + size_distri
+000084a0: 6275 7469 6f6e 5f73 6967 6d61 2a73 697a  bution_sigma*siz
+000084b0: 655f 6469 7374 7269 6275 7469 6f6e 5f73  e_distribution_s
+000084c0: 6967 6d61 2f32 2e30 290a 2020 2020 2020  igma/2.0).      
+000084d0: 2020 2020 2020 2376 5f63 6d31 203d 2031        #v_cm1 = 1
+000084e0: 2e30 4534 2f6c 616d 6264 615f 7661 6375  .0E4/lambda_vacu
+000084f0: 756d 5f6d 750a 2020 2020 2020 2020 2020  um_mu.          
+00008500: 2020 2370 7269 6e74 2822 4672 6571 7565    #print("Freque
+00008510: 6e63 792c 6e6f 726d 616c 2c6d 6561 6e22  ncy,normal,mean"
+00008520: 2c76 5f63 6d31 2c6e 6f72 6d61 6c2c 7472  ,v_cm1,normal,tr
+00008530: 7565 5f6d 6561 6e2c 6d65 616e 290a 2020  ue_mean,mean).  
+00008540: 2020 2020 2020 2020 2020 6966 206e 702e            if np.
+00008550: 6162 7328 6e6f 726d 616c 202d 2031 2e30  abs(normal - 1.0
+00008560: 2920 3e20 312e 3045 2d32 3a0a 2020 2020  ) > 1.0E-2:.    
+00008570: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00008580: 7428 2257 6172 6e69 6e67 2069 6e74 6567  t("Warning integ
+00008590: 7261 7469 6f6e 206f 6620 6c6f 672d 6e6f  ration of log-no
+000085a0: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
+000085b0: 6e20 696e 2065 7272 6f72 222c 206e 6f72  n in error", nor
+000085c0: 6d61 6c29 0a20 2020 2020 2020 2020 2020  mal).           
+000085d0: 2020 2020 2070 7269 6e74 2822 5374 6f70       print("Stop
+000085e0: 7069 6e67 2063 616c 6375 6c61 7469 6f6e  ping calculation
+000085f0: 202d 206c 696b 656c 7920 7072 6f62 6c65   - likely proble
+00008600: 6d20 6973 2074 6f6f 206c 6172 6765 2061  m is too large a
+00008610: 2073 6967 6d61 2066 6f72 206c 6f67 2d6e   sigma for log-n
+00008620: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
+00008630: 6f6e 2229 0a20 2020 2020 2020 2020 2020  on").           
+00008640: 2020 2020 2065 6666 6469 656c 6563 203d       effdielec =
+00008650: 206e 702e 6172 7261 7928 5b5b 312c 2030   np.array([[1, 0
+00008660: 2c20 305d 2c20 5b30 2c20 312c 2030 5d2c  , 0], [0, 1, 0],
+00008670: 205b 302c 2030 2c20 315d 5d29 0a20 2020   [0, 0, 1]]).   
+00008680: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00008690: 7572 6e20 6566 6664 6965 6c65 630a 2020  urn effdielec.  
+000086a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000086b0: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
+000086c0: 6174 6520 7468 6520 7363 6174 7465 7269  ate the scatteri
+000086d0: 6e67 2066 6163 746f 7273 2061 7420 3020  ng factors at 0 
+000086e0: 6465 6772 6565 730a 2020 2020 2020 2020  degrees.        
+000086f0: 2020 2020 236a 6b20 7072 696e 7428 2272      #jk print("r
+00008700: 6566 7261 6374 6976 655f 696e 6465 782c  efractive_index,
+00008710: 2073 697a 652c 2072 6566 7261 6374 6976   size, refractiv
+00008720: 655f 696e 6465 785f 6d65 6469 756d 222c  e_index_medium",
+00008730: 2072 6566 7261 6374 6976 655f 696e 6465   refractive_inde
+00008740: 782c 2073 697a 652c 2072 6566 7261 6374  x, size, refract
+00008750: 6976 655f 696e 6465 785f 6d65 6469 756d  ive_index_medium
+00008760: 290a 2020 2020 2020 2020 2020 2020 7331  ).            s1
+00008770: 2c73 3220 3d20 4d69 652e 4d69 6553 3153  ,s2 = Mie.MieS1S
+00008780: 3228 7265 6672 6163 7469 7665 5f69 6e64  2(refractive_ind
+00008790: 6578 2c20 7369 7a65 2a72 6566 7261 6374  ex, size*refract
+000087a0: 6976 655f 696e 6465 785f 6d65 6469 756d  ive_index_medium
+000087b0: 2c20 3129 0a20 2020 2020 2020 2023 2053  , 1).        # S
+000087c0: 6565 2076 616e 2064 6520 4875 6c73 7420  ee van de Hulst 
+000087d0: 7061 6765 2031 3239 2c20 3133 300a 2020  page 129, 130.  
+000087e0: 2020 2020 2020 2320 5265 6672 6163 7469        # Refracti
+000087f0: 7665 2069 6e64 6578 206f 6620 6d61 7465  ve index of mate
+00008800: 7269 616c 2069 730a 2020 2020 2020 2020  rial is.        
+00008810: 2320 7468 6520 7369 676e 206f 6620 7468  # the sign of th
+00008820: 6520 696d 6167 696e 6172 7920 636f 6d70  e imaginary comp
+00008830: 6f6e 656e 7420 6861 7320 6368 616e 6765  onent has change
+00008840: 6420 666f 7220 636f 6d70 6174 6962 696c  d for compatibil
+00008850: 6974 7920 7769 7468 204d 472f 4272 7567  ity with MG/Brug
+00008860: 6765 6d61 6e0a 2020 2020 2020 2020 7265  geman.        re
+00008870: 6672 6163 7469 7665 5f69 6e64 6578 203d  fractive_index =
+00008880: 2072 6566 7261 6374 6976 655f 696e 6465   refractive_inde
+00008890: 785f 6d65 6469 756d 202a 2028 2031 2e30  x_medium * ( 1.0
+000088a0: 202b 2069 202a 2073 3120 2a20 3220 2a20   + i * s1 * 2 * 
+000088b0: 5049 202a 204e 5f6e 6d20 2f20 2820 6b5f  PI * N_nm / ( k_
+000088c0: 6e6d 202a 206b 5f6e 6d20 2a20 6b5f 6e6d  nm * k_nm * k_nm
+000088d0: 2029 2029 0a20 2020 2020 2020 2074 7261   ) ).        tra
+000088e0: 6365 202b 3d20 7265 6672 6163 7469 7665  ce += refractive
+000088f0: 5f69 6e64 6578 0a20 2020 2023 2072 6574  _index.    # ret
+00008900: 7572 6e20 616e 2069 736f 7472 6f70 6963  urn an isotropic
+00008910: 2074 656e 736f 720a 2020 2020 7472 6163   tensor.    trac
+00008920: 6520 3d20 7472 6163 6520 2f20 332e 300a  e = trace / 3.0.
+00008930: 2020 2020 6566 6620 3d20 7472 6163 6520      eff = trace 
+00008940: 2a20 7472 6163 650a 2020 2020 6566 6664  * trace.    effd
+00008950: 6965 6c65 6320 3d20 6e70 2e61 7272 6179  ielec = np.array
+00008960: 285b 5b65 6666 2c20 302c 2030 5d2c 205b  ([[eff, 0, 0], [
+00008970: 302c 2065 6666 2c20 305d 2c20 5b30 2c20  0, eff, 0], [0, 
+00008980: 302c 2065 6666 5d5d 290a 2020 2020 236a  0, eff]]).    #j
+00008990: 6b20 7072 696e 7428 7261 6469 7573 5f6e  k print(radius_n
+000089a0: 6d2c 206c 616d 6264 615f 7661 6375 756d  m, lambda_vacuum
+000089b0: 5f6d 752a 3130 3030 2e30 2c20 7165 7874  _mu*1000.0, qext
+000089c0: 2c71 7363 612c 7161 6273 2c67 2c71 7072  ,qsca,qabs,g,qpr
+000089d0: 2c71 6261 636b 2c71 7261 7469 6f2c 6e70  ,qback,qratio,np
+000089e0: 2e72 6561 6c28 7331 292c 6e70 2e69 6d61  .real(s1),np.ima
+000089f0: 6728 7331 292c 6e70 2e72 6561 6c28 7472  g(s1),np.real(tr
+00008a00: 6163 6529 2c6e 702e 696d 6167 2874 7261  ace),np.imag(tra
+00008a10: 6365 292c 6e70 2e72 6561 6c28 6566 6629  ce),np.real(eff)
+00008a20: 2c6e 702e 696d 6167 2865 6666 2929 0a20  ,np.imag(eff)). 
+00008a30: 2020 2023 7072 696e 7420 2822 7261 6469     #print ("radi
+00008a40: 7573 5f6e 6d2c 2065 6666 222c 2072 6164  us_nm, eff", rad
+00008a50: 6975 735f 6e6d 2c20 6566 6629 0a20 2020  ius_nm, eff).   
+00008a60: 2072 6574 7572 6e20 6566 6664 6965 6c65   return effdiele
+00008a70: 630a 0a64 6566 206d 6178 7765 6c6c 2864  c..def maxwell(d
+00008a80: 6965 6c65 6374 7269 635f 6d65 6469 756d  ielectric_medium
+00008a90: 2c20 6372 7973 7461 6c5f 7065 726d 6974  , crystal_permit
+00008aa0: 7469 7669 7479 2c20 7368 6170 652c 204c  tivity, shape, L
+00008ab0: 2c20 7666 2c20 7369 7a65 293a 0a20 2020  , vf, size):.   
+00008ac0: 2022 2222 4361 6c63 756c 6174 6520 7468   """Calculate th
+00008ad0: 6520 6566 6665 6374 6976 6520 636f 6e73  e effective cons
+00008ae0: 7461 6e74 2070 6572 6d69 7474 6976 6974  tant permittivit
+00008af0: 7920 7573 696e 6720 7468 6520 6d61 7877  y using the maxw
+00008b00: 656c 6c20 6761 726e 6574 7420 6d65 7468  ell garnett meth
+00008b10: 6f64 0a20 2020 2020 2020 6469 656c 6563  od.       dielec
+00008b20: 7472 6963 5f6d 6564 6975 6d20 6973 2074  tric_medium is t
+00008b30: 6865 2064 6965 6c65 6374 7269 6320 636f  he dielectric co
+00008b40: 6e73 7461 6e74 2074 656e 736f 7220 6f66  nstant tensor of
+00008b50: 2074 6865 206d 6564 6975 6d0a 2020 2020   the medium.    
+00008b60: 2020 2063 7279 7374 616c 5f70 6572 6d69     crystal_permi
+00008b70: 7474 6976 6974 7920 6973 2074 6865 2074  ttivity is the t
+00008b80: 6f74 616c 2066 7265 7175 656e 6379 2064  otal frequency d
+00008b90: 6965 6c65 6374 7269 6320 636f 6e73 7461  ielectric consta
+00008ba0: 6e74 2074 656e 736f 7220 6174 2074 6865  nt tensor at the
+00008bb0: 2063 7572 7265 6e74 2066 7265 7175 656e   current frequen
+00008bc0: 6379 0a20 2020 2020 2020 7368 6170 6520  cy.       shape 
+00008bd0: 6973 2074 6865 206e 616d 6520 6f66 2074  is the name of t
+00008be0: 6865 2063 7572 7265 6e74 2073 6861 7065  he current shape
+00008bf0: 0a20 2020 2020 2020 4c20 6973 2074 6865  .       L is the
+00008c00: 2073 6861 7065 7320 6465 706f 6c61 7269   shapes depolari
+00008c10: 7361 7469 6f6e 206d 6174 7269 780a 2020  sation matrix.  
+00008c20: 2020 2020 2073 697a 6520 6973 2074 6865       size is the
+00008c30: 2064 696d 656e 7369 6f6e 6c65 7373 2073   dimensionless s
+00008c40: 697a 6520 7061 7261 6d65 7465 7220 666f  ize parameter fo
+00008c50: 7220 7468 6520 6672 6571 7565 6e63 7920  r the frequency 
+00008c60: 756e 6465 7220 636f 6e73 6964 6572 6174  under considerat
+00008c70: 696f 6e0a 2020 2020 2020 2076 6620 6973  ion.       vf is
+00008c80: 2074 6865 2076 6f6c 756d 6520 6672 6163   the volume frac
+00008c90: 7469 6f6e 206f 6620 6669 6c6c 6572 0a20  tion of filler. 
+00008ca0: 2020 2020 2020 5468 6520 726f 7574 696e        The routin
+00008cb0: 6520 7265 7475 726e 7320 7468 6520 6566  e returns the ef
+00008cc0: 6665 6374 6976 6520 6469 656c 6563 7472  fective dielectr
+00008cd0: 6963 2063 6f6e 7374 616e 7422 2222 0a20  ic constant""". 
+00008ce0: 2020 2075 6e69 7420 3d20 696e 6974 6961     unit = initia
+00008cf0: 6c69 7365 5f75 6e69 745f 7465 6e73 6f72  lise_unit_tensor
+00008d00: 2829 0a20 2020 2065 6d65 6469 756d 203d  ().    emedium =
+00008d10: 206e 702e 7472 6163 6528 6469 656c 6563   np.trace(dielec
+00008d20: 7472 6963 5f6d 6564 6975 6d29 202f 2033  tric_medium) / 3
+00008d30: 2e30 0a20 2020 2023 2049 6620 6170 7072  .0.    # If appr
+00008d40: 6f70 7269 6174 6520 6361 6c63 756c 6174  opriate calculat
+00008d50: 6520 6120 7369 7a65 2065 6666 6563 7420  e a size effect 
+00008d60: 7573 696e 6720 4571 7561 7469 6f6e 7320  using Equations 
+00008d70: 3130 2e33 3820 616e 6420 3130 2e33 3920  10.38 and 10.39 
+00008d80: 696e 2053 6968 766f 6c61 0a20 2020 2073  in Sihvola.    s
+00008d90: 697a 655f 6661 6374 6f72 203d 2063 616c  ize_factor = cal
+00008da0: 6375 6c61 7465 5f73 697a 655f 6661 6374  culate_size_fact
+00008db0: 6f72 2873 697a 6529 0a20 2020 2023 2045  or(size).    # E
+00008dc0: 7175 6174 696f 6e20 352e 3738 2069 6e20  quation 5.78 in 
+00008dd0: 5369 6876 6f6c 610a 2020 2020 6e61 6c70  Sihvola.    nalp
+00008de0: 6861 203d 2065 6d65 6469 756d 2a76 662a  ha = emedium*vf*
+00008df0: 6e70 2e64 6f74 2828 6372 7973 7461 6c5f  np.dot((crystal_
+00008e00: 7065 726d 6974 7469 7669 7479 202d 2064  permittivity - d
+00008e10: 6965 6c65 6374 7269 635f 6d65 6469 756d  ielectric_medium
+00008e20: 292c 206e 702e 6c69 6e61 6c67 2e69 6e76  ), np.linalg.inv
+00008e30: 2864 6965 6c65 6374 7269 635f 6d65 6469  (dielectric_medi
+00008e40: 756d 202b 2073 697a 655f 6661 6374 6f72  um + size_factor
+00008e50: 202a 206e 702e 646f 7428 4c2c 2028 6372   * np.dot(L, (cr
+00008e60: 7973 7461 6c5f 7065 726d 6974 7469 7669  ystal_permittivi
+00008e70: 7479 2d64 6965 6c65 6374 7269 635f 6d65  ty-dielectric_me
+00008e80: 6469 756d 2929 2929 0a20 2020 206e 616c  dium)))).    nal
+00008e90: 7068 616c 203d 206e 702e 646f 7428 286e  phal = np.dot((n
+00008ea0: 616c 7068 612f 656d 6564 6975 6d29 2c20  alpha/emedium), 
+00008eb0: 4c29 0a20 2020 2023 2061 7665 7261 6765  L).    # average
+00008ec0: 2074 6865 2070 6f6c 6172 6973 6162 696c   the polarisabil
+00008ed0: 6974 7920 6f76 6572 206f 7269 656e 7461  ity over orienta
+00008ee0: 7469 6f6e 0a20 2020 206e 616c 7068 6120  tion.    nalpha 
+00008ef0: 3d20 6e70 2e74 7261 6365 286e 616c 7068  = np.trace(nalph
+00008f00: 6129 202f 2033 2e30 202a 2075 6e69 740a  a) / 3.0 * unit.
+00008f10: 2020 2020 2320 6176 6572 6167 6520 7468      # average th
+00008f20: 6520 706f 6c61 7269 7361 6269 6c69 7479  e polarisability
+00008f30: 2a4c 206f 7665 7220 6f72 6965 6e74 6174  *L over orientat
+00008f40: 696f 6e0a 2020 2020 6e61 6c70 6861 6c20  ion.    nalphal 
+00008f50: 3d20 6e70 2e74 7261 6365 286e 616c 7068  = np.trace(nalph
+00008f60: 616c 2920 2f20 332e 3020 2a20 756e 6974  al) / 3.0 * unit
+00008f70: 0a20 2020 2070 6f6c 6172 6973 6174 696f  .    polarisatio
+00008f80: 6e20 3d20 6e70 2e64 6f74 286e 702e 6c69  n = np.dot(np.li
+00008f90: 6e61 6c67 2e69 6e76 2875 6e69 7420 2d20  nalg.inv(unit - 
+00008fa0: 6e61 6c70 6861 6c29 2c20 6e61 6c70 6861  nalphal), nalpha
+00008fb0: 290a 2020 2020 6566 6664 2020 2020 2020  ).    effd      
+00008fc0: 2020 203d 2064 6965 6c65 6374 7269 635f     = dielectric_
+00008fd0: 6d65 6469 756d 202b 2070 6f6c 6172 6973  medium + polaris
+00008fe0: 6174 696f 6e0a 2020 2020 7472 6163 6520  ation.    trace 
+00008ff0: 3d20 6e70 2e74 7261 6365 2865 6666 6429  = np.trace(effd)
+00009000: 202f 2033 2e30 0a20 2020 2065 6666 6469   / 3.0.    effdi
+00009010: 656c 6563 203d 206e 702e 6172 7261 7928  elec = np.array(
+00009020: 5b5b 7472 6163 652c 2030 2c20 305d 2c20  [[trace, 0, 0], 
+00009030: 5b30 2c20 7472 6163 652c 2030 5d2c 205b  [0, trace, 0], [
+00009040: 302c 2030 2c20 7472 6163 655d 5d29 0a20  0, 0, trace]]). 
+00009050: 2020 2072 6574 7572 6e20 6566 6664 6965     return effdie
+00009060: 6c65 630a 0a64 6566 206d 6178 7765 6c6c  lec..def maxwell
+00009070: 5f73 6968 766f 6c61 2864 6965 6c65 6374  _sihvola(dielect
+00009080: 7269 635f 6d65 6469 756d 2c20 6372 7973  ric_medium, crys
+00009090: 7461 6c5f 7065 726d 6974 7469 7669 7479  tal_permittivity
+000090a0: 2c20 7368 6170 652c 204c 2c20 7666 2c20  , shape, L, vf, 
+000090b0: 7369 7a65 293a 0a20 2020 2022 2222 4361  size):.    """Ca
+000090c0: 6c63 756c 6174 6520 7468 6520 6566 6665  lculate the effe
+000090d0: 6374 6976 6520 636f 6e73 7461 6e74 2070  ctive constant p
+000090e0: 6572 6d69 7474 6976 6974 7920 7573 696e  ermittivity usin
+000090f0: 6720 7468 6520 6d61 7877 656c 6c20 6761  g the maxwell ga
+00009100: 726e 6574 7420 6d65 7468 6f64 0a20 2020  rnett method.   
+00009110: 2020 2020 6469 656c 6563 7472 6963 5f6d      dielectric_m
+00009120: 6564 6975 6d20 6973 2074 6865 2064 6965  edium is the die
+00009130: 6c65 6374 7269 6320 636f 6e73 7461 6e74  lectric constant
+00009140: 2074 656e 736f 7220 6f66 2074 6865 206d   tensor of the m
+00009150: 6564 6975 6d0a 2020 2020 2020 2063 7279  edium.       cry
+00009160: 7374 616c 5f70 6572 6d69 7474 6976 6974  stal_permittivit
+00009170: 7920 6973 2074 6865 2074 6f74 616c 2066  y is the total f
+00009180: 7265 7175 656e 6379 2064 6965 6c65 6374  requency dielect
+00009190: 7269 6320 636f 6e73 7461 6e74 2074 656e  ric constant ten
+000091a0: 736f 7220 6174 2074 6865 2063 7572 7265  sor at the curre
+000091b0: 6e74 2066 7265 7175 656e 6379 0a20 2020  nt frequency.   
+000091c0: 2020 2020 7368 6170 6520 6973 2074 6865      shape is the
+000091d0: 206e 616d 6520 6f66 2074 6865 2063 7572   name of the cur
+000091e0: 7265 6e74 2073 6861 7065 0a20 2020 2020  rent shape.     
+000091f0: 2020 4c20 6973 2074 6865 2073 6861 7065    L is the shape
+00009200: 7320 6465 706f 6c61 7269 7361 7469 6f6e  s depolarisation
+00009210: 206d 6174 7269 780a 2020 2020 2020 2073   matrix.       s
+00009220: 697a 6520 6973 2074 6865 2064 696d 656e  ize is the dimen
+00009230: 7369 6f6e 6c65 7373 2073 697a 6520 7061  sionless size pa
+00009240: 7261 6d65 7465 7220 666f 7220 7468 6520  rameter for the 
+00009250: 6672 6571 7565 6e63 7920 756e 6465 7220  frequency under 
+00009260: 636f 6e73 6964 6572 6174 696f 6e0a 2020  consideration.  
+00009270: 2020 2020 2076 6620 6973 2074 6865 2076       vf is the v
+00009280: 6f6c 756d 6520 6672 6163 7469 6f6e 206f  olume fraction o
+00009290: 6620 6669 6c6c 6572 0a20 2020 2020 2020  f filler.       
+000092a0: 5468 6520 726f 7574 696e 6520 7265 7475  The routine retu
+000092b0: 726e 7320 7468 6520 6566 6665 6374 6976  rns the effectiv
+000092c0: 6520 6469 656c 6563 7472 6963 2063 6f6e  e dielectric con
+000092d0: 7374 616e 7422 2222 0a20 2020 2075 6e69  stant""".    uni
+000092e0: 7420 3d20 696e 6974 6961 6c69 7365 5f75  t = initialise_u
+000092f0: 6e69 745f 7465 6e73 6f72 2829 0a20 2020  nit_tensor().   
+00009300: 2023 2045 7175 6174 696f 6e20 362e 3239   # Equation 6.29
+00009310: 206f 6e20 7061 6765 2031 3233 206f 6620   on page 123 of 
+00009320: 5369 6876 6f6c 610a 2020 2020 2320 4571  Sihvola.    # Eq
+00009330: 7561 7469 6f6e 2036 2e34 3020 6769 7665  uation 6.40 give
+00009340: 7320 7468 6520 6176 6572 6167 696e 6720  s the averaging 
+00009350: 6f76 6572 2074 6865 206f 7269 656e 7461  over the orienta
+00009360: 7469 6f6e 2066 756e 6374 696f 6e0a 2020  tion function.  
+00009370: 2020 2320 5365 6520 616c 736f 2065 7175    # See also equ
+00009380: 6174 696f 6e20 352e 3830 206f 6e20 7061  ation 5.80 on pa
+00009390: 6765 2031 3032 2061 6e64 2065 7175 6174  ge 102 and equat
+000093a0: 696f 6e20 342e 3331 206f 6e20 7061 6765  ion 4.31 on page
+000093b0: 2037 300a 2020 2020 4d65 203d 2064 6965   70.    Me = die
+000093c0: 6c65 6374 7269 635f 6d65 6469 756d 0a20  lectric_medium. 
+000093d0: 2020 2023 2061 7373 756d 6520 7468 6174     # assume that
+000093e0: 2074 6865 206d 6564 6975 6d20 6973 2069   the medium is i
+000093f0: 736f 7472 6f70 6963 2063 616c 6375 6c61  sotropic calcula
+00009400: 7465 2074 6865 2069 6e76 6572 7365 206f  te the inverse o
+00009410: 6620 7468 6520 6469 656c 6563 7472 6963  f the dielectric
+00009420: 0a20 2020 204d 656d 3120 3d20 332e 3020  .    Mem1 = 3.0 
+00009430: 2f20 6e70 2e74 7261 6365 284d 6529 0a20  / np.trace(Me). 
+00009440: 2020 204d 6920 3d20 6372 7973 7461 6c5f     Mi = crystal_
+00009450: 7065 726d 6974 7469 7669 7479 0a20 2020  permittivity.   
+00009460: 2023 2049 6620 6170 7072 6f70 7269 6174   # If appropriat
+00009470: 6520 6361 6c63 756c 6174 6520 6120 7369  e calculate a si
+00009480: 7a65 2065 6666 6563 7420 7573 696e 6720  ze effect using 
+00009490: 4571 7561 7469 6f6e 7320 3130 2e33 3820  Equations 10.38 
+000094a0: 616e 6420 3130 2e33 3920 696e 2053 6968  and 10.39 in Sih
+000094b0: 766f 6c61 0a20 2020 2073 697a 655f 6661  vola.    size_fa
+000094c0: 6374 6f72 203d 2063 616c 6375 6c61 7465  ctor = calculate
+000094d0: 5f73 697a 655f 6661 6374 6f72 2873 697a  _size_factor(siz
+000094e0: 6529 0a20 2020 2023 2063 616c 6375 6c61  e).    # calcula
+000094f0: 7465 2074 6865 2070 6f6c 6172 6973 6162  te the polarisab
+00009500: 696c 6974 7920 6d61 7472 6978 2078 2074  ility matrix x t
+00009510: 6865 206e 756d 6265 7220 6465 6e73 6974  he number densit
+00009520: 7920 6f66 2069 6e63 6c75 7369 6f6e 730a  y of inclusions.
+00009530: 2020 2020 6e41 203d 2076 662a 6e70 2e64      nA = vf*np.d
+00009540: 6f74 2828 4d69 2d4d 6529 2c20 6e70 2e6c  ot((Mi-Me), np.l
+00009550: 696e 616c 672e 696e 7628 756e 6974 202b  inalg.inv(unit +
+00009560: 2028 7369 7a65 5f66 6163 746f 7220 2a20   (size_factor * 
+00009570: 4d65 6d31 202a 206e 702e 646f 7428 4c2c  Mem1 * np.dot(L,
+00009580: 2028 4d69 202d 204d 6529 2929 2929 0a20   (Mi - Me))))). 
+00009590: 2020 206e 414c 203d 206e 702e 646f 7428     nAL = np.dot(
+000095a0: 286e 4129 2c20 4c29 0a20 2020 2023 2061  (nA), L).    # a
+000095b0: 7665 7261 6765 2074 6865 2070 6f6c 6172  verage the polar
+000095c0: 6973 6162 696c 6974 7920 6f76 6572 206f  isability over o
+000095d0: 7269 656e 7461 7469 6f6e 0a20 2020 206e  rientation.    n
+000095e0: 4120 3d20 6e70 2e74 7261 6365 286e 4129  A = np.trace(nA)
+000095f0: 202f 2033 2e30 202a 2075 6e69 740a 2020   / 3.0 * unit.  
+00009600: 2020 2320 6176 6572 6167 6520 7468 6520    # average the 
+00009610: 706f 6c61 7269 7361 6269 6c69 7479 2a4c  polarisability*L
+00009620: 206f 7665 7220 6f72 6965 6e74 6174 696f   over orientatio
+00009630: 6e0a 2020 2020 6e41 4c20 3d20 6e70 2e74  n.    nAL = np.t
+00009640: 7261 6365 286e 414c 2920 2f20 332e 3020  race(nAL) / 3.0 
+00009650: 2a20 4d65 6d31 202a 2075 6e69 740a 2020  * Mem1 * unit.  
+00009660: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
+00009670: 6520 6176 6572 6167 6520 706f 6c61 7269  e average polari
+00009680: 7361 7469 6f6e 2066 6163 746f 7220 7768  sation factor wh
+00009690: 6963 6820 7363 616c 6573 2074 6865 2061  ich scales the a
+000096a0: 7665 7261 6765 2066 6965 6c64 0a20 2020  verage field.   
+000096b0: 2023 2062 6173 6564 206f 6e20 6571 7561   # based on equa
+000096c0: 7469 6f6e 2035 2e38 300a 2020 2020 2320  tion 5.80.    # 
+000096d0: 3c50 3e20 3d20 706f 6c20 2e20 3c45 3e0a  <P> = pol . <E>.
+000096e0: 2020 2020 706f 6c20 3d20 6e70 2e64 6f74      pol = np.dot
+000096f0: 286e 702e 6c69 6e61 6c67 2e69 6e76 2875  (np.linalg.inv(u
+00009700: 6e69 7420 2d20 6e41 4c29 2c20 6e41 290a  nit - nAL), nA).
+00009710: 2020 2020 2320 4d65 6666 202e 203c 453e      # Meff . <E>
+00009720: 203d 204d 6520 2e20 3c45 3e20 2b20 3c50   = Me . <E> + <P
+00009730: 3e0a 2020 2020 2320 4d65 6666 202e 203c  >.    # Meff . <
+00009740: 453e 203d 204d 652e 203c 453e 202b 2070  E> = Me. <E> + p
+00009750: 6f6c 202e 203c 453e 0a20 2020 2023 204d  ol . <E>.    # M
+00009760: 6566 6620 3d20 4d65 202b 2070 6f6c 0a20  eff = Me + pol. 
+00009770: 2020 2065 6666 6420 2020 2020 2020 2020     effd         
+00009780: 3d20 6469 656c 6563 7472 6963 5f6d 6564  = dielectric_med
+00009790: 6975 6d20 2b20 706f 6c0a 2020 2020 2320  ium + pol.    # 
+000097a0: 4176 6572 6167 6520 6f76 6572 206f 7269  Average over ori
+000097b0: 656e 7461 7469 6f6e 0a20 2020 2074 7261  entation.    tra
+000097c0: 6365 203d 206e 702e 7472 6163 6528 6566  ce = np.trace(ef
+000097d0: 6664 2920 2f20 332e 300a 2020 2020 6566  fd) / 3.0.    ef
+000097e0: 6664 6965 6c65 6320 3d20 6e70 2e61 7272  fdielec = np.arr
+000097f0: 6179 285b 5b74 7261 6365 2c20 302c 2030  ay([[trace, 0, 0
+00009800: 5d2c 205b 302c 2074 7261 6365 2c20 305d  ], [0, trace, 0]
+00009810: 2c20 5b30 2c20 302c 2074 7261 6365 5d5d  , [0, 0, trace]]
+00009820: 290a 2020 2020 7265 7475 726e 2065 6666  ).    return eff
+00009830: 6469 656c 6563 0a0a 6465 6620 636f 6865  dielec..def cohe
+00009840: 7265 6e74 2864 6965 6c65 6374 7269 635f  rent(dielectric_
+00009850: 6d65 6469 756d 2c20 6372 7973 7461 6c5f  medium, crystal_
+00009860: 7065 726d 6974 7469 7669 7479 2c20 7368  permittivity, sh
+00009870: 6170 652c 204c 2c20 7666 2c20 7369 7a65  ape, L, vf, size
+00009880: 2c20 6469 656c 6563 7472 6963 5f61 7070  , dielectric_app
+00009890: 6172 656e 7429 3a0a 2020 2020 2222 2244  arent):.    """D
+000098a0: 7269 7665 7220 666f 7220 636f 6865 7265  river for cohere
+000098b0: 6e74 3220 6d65 7468 6f64 2222 220a 2020  nt2 method""".  
+000098c0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+000098d0: 2831 3029 3a0a 2020 2020 2020 2020 6469  (10):.        di
+000098e0: 656c 6563 7472 6963 5f61 7070 6172 656e  electric_apparen
+000098f0: 7420 3d20 302e 3120 2a20 6469 656c 6563  t = 0.1 * dielec
+00009900: 7472 6963 5f61 7070 6172 656e 7420 2b20  tric_apparent + 
+00009910: 302e 3920 2a20 636f 6865 7265 6e74 3228  0.9 * coherent2(
+00009920: 6469 656c 6563 7472 6963 5f6d 6564 6975  dielectric_mediu
+00009930: 6d2c 2064 6965 6c65 6374 7269 635f 6170  m, dielectric_ap
+00009940: 7061 7265 6e74 2c20 6372 7973 7461 6c5f  parent, crystal_
+00009950: 7065 726d 6974 7469 7669 7479 2c20 7368  permittivity, sh
+00009960: 6170 652c 204c 2c20 7666 2c20 7369 7a65  ape, L, vf, size
+00009970: 290a 2020 2020 7265 7475 726e 2064 6965  ).    return die
+00009980: 6c65 6374 7269 635f 6170 7061 7265 6e74  lectric_apparent
+00009990: 0a0a 6465 6620 636f 6865 7265 6e74 3228  ..def coherent2(
+000099a0: 6469 656c 6563 7472 6963 5f6d 6564 6975  dielectric_mediu
+000099b0: 6d2c 2064 6965 6c65 6374 7269 635f 6170  m, dielectric_ap
+000099c0: 7061 7265 6e74 2c20 6372 7973 7461 6c5f  parent, crystal_
+000099d0: 7065 726d 6974 7469 7669 7479 2c20 7368  permittivity, sh
+000099e0: 6170 652c 204c 2c20 7666 2c20 7369 7a65  ape, L, vf, size
+000099f0: 293a 0a20 2020 2022 2222 4361 6c63 756c  ):.    """Calcul
+00009a00: 6174 6520 7468 6520 6566 6665 6374 6976  ate the effectiv
+00009a10: 6520 636f 6e73 7461 6e74 2070 6572 6d69  e constant permi
+00009a20: 7474 6976 6974 7920 7573 696e 6720 7468  ttivity using th
+00009a30: 6520 6d61 7877 656c 6c20 6761 726e 6574  e maxwell garnet
+00009a40: 7420 6d65 7468 6f64 0a20 2020 2020 2020  t method.       
+00009a50: 6469 656c 6563 7472 6963 5f6d 6564 6975  dielectric_mediu
+00009a60: 6d20 6973 2074 6865 2064 6965 6c65 6374  m is the dielect
+00009a70: 7269 6320 636f 6e73 7461 6e74 2074 656e  ric constant ten
+00009a80: 736f 7220 6f66 2074 6865 206d 6564 6975  sor of the mediu
+00009a90: 6d0a 2020 2020 2020 2063 7279 7374 616c  m.       crystal
+00009aa0: 5f70 6572 6d69 7474 6976 6974 7920 6973  _permittivity is
+00009ab0: 2074 6865 2074 6f74 616c 2066 7265 7175   the total frequ
+00009ac0: 656e 6379 2064 6965 6c65 6374 7269 6320  ency dielectric 
+00009ad0: 636f 6e73 7461 6e74 2074 656e 736f 7220  constant tensor 
+00009ae0: 6174 2074 6865 2063 7572 7265 6e74 2066  at the current f
+00009af0: 7265 7175 656e 6379 0a20 2020 2020 2020  requency.       
+00009b00: 7368 6170 6520 6973 2074 6865 206e 616d  shape is the nam
+00009b10: 6520 6f66 2074 6865 2063 7572 7265 6e74  e of the current
+00009b20: 2073 6861 7065 0a20 2020 2020 2020 4c20   shape.       L 
+00009b30: 6973 2074 6865 2073 6861 7065 7320 6465  is the shapes de
+00009b40: 706f 6c61 7269 7361 7469 6f6e 206d 6174  polarisation mat
+00009b50: 7269 780a 2020 2020 2020 2073 697a 6520  rix.       size 
+00009b60: 6973 2074 6865 2064 696d 656e 7369 6f6e  is the dimension
+00009b70: 6c65 7373 2073 697a 6520 7061 7261 6d65  less size parame
+00009b80: 7465 7220 666f 7220 7468 6520 6672 6571  ter for the freq
+00009b90: 7565 6e63 7920 756e 6465 7220 636f 6e73  uency under cons
+00009ba0: 6964 6572 6174 696f 6e0a 2020 2020 2020  ideration.      
+00009bb0: 2076 6620 6973 2074 6865 2076 6f6c 756d   vf is the volum
+00009bc0: 6520 6672 6163 7469 6f6e 206f 6620 6669  e fraction of fi
+00009bd0: 6c6c 6572 0a20 2020 2020 2020 5468 6520  ller.       The 
+00009be0: 726f 7574 696e 6520 7265 7475 726e 7320  routine returns 
+00009bf0: 7468 6520 6566 6665 6374 6976 6520 6469  the effective di
+00009c00: 656c 6563 7472 6963 2063 6f6e 7374 616e  electric constan
+00009c10: 7422 2222 0a20 2020 2075 6e69 7420 3d20  t""".    unit = 
+00009c20: 696e 6974 6961 6c69 7365 5f75 6e69 745f  initialise_unit_
+00009c30: 7465 6e73 6f72 2829 0a20 2020 2065 6d65  tensor().    eme
+00009c40: 6469 756d 203d 206e 702e 7472 6163 6528  dium = np.trace(
+00009c50: 6469 656c 6563 7472 6963 5f6d 6564 6975  dielectric_mediu
+00009c60: 6d29 202f 2033 2e30 0a20 2020 2065 6170  m) / 3.0.    eap
+00009c70: 7061 7265 6e74 203d 206e 702e 7472 6163  parent = np.trac
+00009c80: 6528 6469 656c 6563 7472 6963 5f61 7070  e(dielectric_app
+00009c90: 6172 656e 7429 202f 2033 2e30 0a20 2020  arent) / 3.0.   
+00009ca0: 2023 2049 6620 6170 7072 6f70 7269 6174   # If appropriat
+00009cb0: 6520 6361 6c63 756c 6174 6520 6120 7369  e calculate a si
+00009cc0: 7a65 2065 6666 6563 7420 7573 696e 6720  ze effect using 
+00009cd0: 4571 7561 7469 6f6e 7320 3130 2e33 3820  Equations 10.38 
+00009ce0: 616e 6420 3130 2e33 3920 696e 2053 6968  and 10.39 in Sih
+00009cf0: 766f 6c61 0a20 2020 2073 697a 655f 6661  vola.    size_fa
+00009d00: 6374 6f72 203d 2063 616c 6375 6c61 7465  ctor = calculate
+00009d10: 5f73 697a 655f 6661 6374 6f72 2873 697a  _size_factor(siz
+00009d20: 6529 0a20 2020 2023 2045 7175 6174 696f  e).    # Equatio
+00009d30: 6e20 352e 3738 2069 6e20 5369 6876 6f6c  n 5.78 in Sihvol
+00009d40: 610a 2020 2020 6e61 6c70 6861 203d 2065  a.    nalpha = e
+00009d50: 6d65 6469 756d 2a76 662a 6e70 2e64 6f74  medium*vf*np.dot
+00009d60: 2828 6372 7973 7461 6c5f 7065 726d 6974  ((crystal_permit
+00009d70: 7469 7669 7479 202d 2064 6965 6c65 6374  tivity - dielect
+00009d80: 7269 635f 6d65 6469 756d 292c 206e 702e  ric_medium), np.
+00009d90: 6c69 6e61 6c67 2e69 6e76 2864 6965 6c65  linalg.inv(diele
+00009da0: 6374 7269 635f 6d65 6469 756d 202b 2073  ctric_medium + s
+00009db0: 697a 655f 6661 6374 6f72 202a 206e 702e  ize_factor * np.
+00009dc0: 646f 7428 4c2c 2028 6372 7973 7461 6c5f  dot(L, (crystal_
+00009dd0: 7065 726d 6974 7469 7669 7479 2d64 6965  permittivity-die
+00009de0: 6c65 6374 7269 635f 6d65 6469 756d 2929  lectric_medium))
+00009df0: 2929 0a20 2020 206e 616c 7068 616c 203d  )).    nalphal =
+00009e00: 206e 702e 646f 7428 286e 616c 7068 612f   np.dot((nalpha/
+00009e10: 6561 7070 6172 656e 7429 2c20 4c29 0a20  eapparent), L). 
+00009e20: 2020 2023 2061 7665 7261 6765 2074 6865     # average the
+00009e30: 2070 6f6c 6172 6973 6162 696c 6974 7920   polarisability 
+00009e40: 6f76 6572 206f 7269 656e 7461 7469 6f6e  over orientation
+00009e50: 0a20 2020 206e 616c 7068 6120 3d20 6e70  .    nalpha = np
+00009e60: 2e74 7261 6365 286e 616c 7068 6129 202f  .trace(nalpha) /
+00009e70: 2033 2e30 202a 2075 6e69 740a 2020 2020   3.0 * unit.    
+00009e80: 2320 6176 6572 6167 6520 7468 6520 706f  # average the po
+00009e90: 6c61 7269 7361 6269 6c69 7479 2a4c 206f  larisability*L o
+00009ea0: 7665 7220 6f72 6965 6e74 6174 696f 6e0a  ver orientation.
+00009eb0: 2020 2020 6e61 6c70 6861 6c20 3d20 6e70      nalphal = np
+00009ec0: 2e74 7261 6365 286e 616c 7068 616c 2920  .trace(nalphal) 
+00009ed0: 2f20 332e 3020 2a20 756e 6974 0a20 2020  / 3.0 * unit.   
+00009ee0: 2070 6f6c 6172 6973 6174 696f 6e20 3d20   polarisation = 
+00009ef0: 6e70 2e64 6f74 286e 702e 6c69 6e61 6c67  np.dot(np.linalg
+00009f00: 2e69 6e76 2875 6e69 7420 2d20 6e61 6c70  .inv(unit - nalp
+00009f10: 6861 6c29 2c20 6e61 6c70 6861 290a 2020  hal), nalpha).  
+00009f20: 2020 6566 6664 2020 2020 2020 2020 203d    effd         =
+00009f30: 2064 6965 6c65 6374 7269 635f 6d65 6469   dielectric_medi
+00009f40: 756d 202b 2070 6f6c 6172 6973 6174 696f  um + polarisatio
+00009f50: 6e0a 2020 2020 7472 6163 6520 3d20 6e70  n.    trace = np
+00009f60: 2e74 7261 6365 2865 6666 6429 202f 2033  .trace(effd) / 3
+00009f70: 2e30 0a20 2020 2065 6666 6469 656c 6563  .0.    effdielec
+00009f80: 203d 206e 702e 6172 7261 7928 5b5b 7472   = np.array([[tr
+00009f90: 6163 652c 2030 2c20 305d 2c20 5b30 2c20  ace, 0, 0], [0, 
+00009fa0: 7472 6163 652c 2030 5d2c 205b 302c 2030  trace, 0], [0, 0
+00009fb0: 2c20 7472 6163 655d 5d29 0a20 2020 2072  , trace]]).    r
+00009fc0: 6574 7572 6e20 6566 6664 6965 6c65 630a  eturn effdielec.
+00009fd0: 0a64 6566 2062 7275 6767 656d 616e 5f6d  .def bruggeman_m
+00009fe0: 696e 696d 6973 6528 2065 7073 312c 2065  inimise( eps1, e
+00009ff0: 7073 322c 2073 6861 7065 2c20 4c2c 2066  ps2, shape, L, f
+0000a000: 322c 2073 697a 652c 2065 7073 6272 293a  2, size, epsbr):
+0000a010: 0a20 2020 2022 2222 4361 6c63 756c 6174  .    """Calculat
+0000a020: 6520 7468 6520 6566 6665 6374 6976 6520  e the effective 
+0000a030: 636f 6e73 7461 6e74 2070 6572 6d69 7474  constant permitt
+0000a040: 6976 6974 7920 7573 696e 6720 7468 6520  ivity using the 
+0000a050: 6d65 7468 6f64 206f 6620 6272 7567 6765  method of brugge
+0000a060: 6d61 6e0a 2020 2020 2020 2065 7073 3120  man.       eps1 
+0000a070: 6973 2074 6865 2064 6965 6c65 6374 7269  is the dielectri
+0000a080: 6320 636f 6e73 7461 6e74 2074 656e 736f  c constant tenso
+0000a090: 7220 6f66 2031 2028 5468 6520 6d65 6469  r of 1 (The medi
+0000a0a0: 756d 290a 2020 2020 2020 2065 7073 3220  um).       eps2 
+0000a0b0: 6973 2074 6865 2064 6965 6c65 6374 7269  is the dielectri
+0000a0c0: 6320 636f 6e73 7461 6e74 2074 656e 736f  c constant tenso
+0000a0d0: 7220 6f66 2032 2028 5468 6520 696e 636c  r of 2 (The incl
+0000a0e0: 7573 696f 6e29 0a20 2020 2020 2020 7368  usion).       sh
+0000a0f0: 6170 6520 6973 2074 6865 206e 616d 6520  ape is the name 
+0000a100: 6f66 2074 6865 2063 7572 7265 6e74 2073  of the current s
+0000a110: 6861 7065 0a20 2020 2020 2020 4c20 6973  hape.       L is
+0000a120: 2074 6865 2073 6861 7065 7320 6465 706f   the shapes depo
+0000a130: 6c61 7269 7361 7469 6f6e 206d 6174 7269  larisation matri
+0000a140: 780a 2020 2020 2020 2066 3220 6973 2074  x.       f2 is t
+0000a150: 6865 2076 6f6c 756d 6520 6672 6163 7469  he volume fracti
+0000a160: 6f6e 206f 6620 636f 6d70 6f6e 656e 7420  on of component 
+0000a170: 320a 2020 2020 2020 2073 697a 6520 6973  2.       size is
+0000a180: 2074 6865 2064 696d 656e 7369 6f6e 6c65   the dimensionle
+0000a190: 7373 2073 697a 6520 7061 7261 6d65 7465  ss size paramete
+0000a1a0: 7220 666f 7220 7468 6520 6672 6571 7565  r for the freque
+0000a1b0: 6e63 7920 756e 6465 7220 636f 6e73 6964  ncy under consid
+0000a1c0: 6572 6174 696f 6e0a 2020 2020 2020 2065  eration.       e
+0000a1d0: 7073 6272 2069 7320 616e 2069 6e69 7469  psbr is an initi
+0000a1e0: 616c 2067 7565 7373 2061 7420 7468 6520  al guess at the 
+0000a1f0: 736f 6c75 7469 6f6e 0a20 2020 2020 2020  solution.       
+0000a200: 5468 6520 726f 7574 696e 6520 7265 7475  The routine retu
+0000a210: 726e 7320 7468 6520 6566 6665 6374 6976  rns the effectiv
+0000a220: 6520 6469 656c 6563 7472 6963 2063 6f6e  e dielectric con
+0000a230: 7374 616e 740a 2020 2020 2020 204f 6e20  stant.       On 
+0000a240: 7468 6520 6170 706c 6963 6174 696f 6e20  the application 
+0000a250: 6f66 2068 6f6d 6f67 656e 697a 6174 696f  of homogenizatio
+0000a260: 6e20 666f 726d 616c 6973 6d73 2074 6f20  n formalisms to 
+0000a270: 6163 7469 7665 2064 6965 6c65 6374 7269  active dielectri
+0000a280: 6320 636f 6d70 6f73 6974 6520 6d61 7465  c composite mate
+0000a290: 7269 616c 730a 2020 2020 2020 2054 6f6d  rials.       Tom
+0000a2a0: 2047 2e20 4d61 636b 6179 2c20 416b 686c   G. Mackay, Akhl
+0000a2b0: 6573 6820 4c61 6b68 7461 6b69 6120 2222  esh Lakhtakia ""
+0000a2c0: 220a 2020 2020 6631 203d 2031 2e30 202d  ".    f1 = 1.0 -
+0000a2d0: 2066 320a 2020 2020 2320 7765 206e 6565   f2.    # we nee
+0000a2e0: 6420 746f 2066 6f6f 6c20 7468 6520 6f70  d to fool the op
+0000a2f0: 7469 6d69 7365 7220 696e 746f 2074 6869  timiser into thi
+0000a300: 6e6b 696e 6720 7468 6174 2069 7420 6861  nking that it ha
+0000a310: 7320 7477 6f20 7265 616c 2076 6172 6961  s two real varia
+0000a320: 626c 6573 0a20 2020 2023 2069 6e20 6661  bles.    # in fa
+0000a330: 6374 2074 6865 2073 6563 6f6e 6420 6973  ct the second is
+0000a340: 2069 6d61 6769 6e61 7279 2061 6e64 2072   imaginary and r
+0000a350: 6563 6f6e 7374 7275 6374 6564 2069 6e20  econstructed in 
+0000a360: 7468 6520 5f62 7275 675f 6d69 6e69 6d69  the _brug_minimi
+0000a370: 7365 2072 6f75 7469 6e65 0a20 2020 2074  se routine.    t
+0000a380: 7261 6365 203d 206e 702e 7472 6163 6528  race = np.trace(
+0000a390: 6570 7362 7229 202f 2033 2e30 0a20 2020  epsbr) / 3.0.   
+0000a3a0: 2076 6172 6961 626c 6573 203d 206e 702e   variables = np.
+0000a3b0: 6172 7261 7928 5b6e 702e 7265 616c 2874  array([np.real(t
+0000a3c0: 7261 6365 292c 206e 702e 6c6f 6728 312e  race), np.log(1.
+0000a3d0: 3020 2b20 6e70 2e61 6273 286e 702e 696d  0 + np.abs(np.im
+0000a3e0: 6167 2874 7261 6365 2929 295d 290a 2020  ag(trace)))]).  
+0000a3f0: 2020 6f70 7469 6f6e 7320 3d20 7b27 7874    options = {'xt
+0000a400: 6f6c 273a 2031 2e30 652d 342c 0a20 2020  ol': 1.0e-4,.   
+0000a410: 2020 2020 2020 2020 2020 2020 2766 746f              'fto
+0000a420: 6c27 3a20 312e 3045 2d34 7d0a 2020 2020  l': 1.0E-4}.    
+0000a430: 736f 6c20 3d20 7363 2e6d 696e 696d 697a  sol = sc.minimiz
+0000a440: 6528 5f62 7275 675f 6d69 6e69 6d69 7365  e(_brug_minimise
+0000a450: 5f74 656e 736f 722c 2076 6172 6961 626c  _tensor, variabl
+0000a460: 6573 2c20 6d65 7468 6f64 3d27 506f 7765  es, method='Powe
+0000a470: 6c6c 272c 2061 7267 733d 2865 7073 312c  ll', args=(eps1,
+0000a480: 2065 7073 322c 2073 6861 7065 2c20 4c2c   eps2, shape, L,
+0000a490: 2066 312c 2073 697a 6529 2c20 6f70 7469   f1, size), opti
+0000a4a0: 6f6e 733d 6f70 7469 6f6e 7329 0a20 2020  ons=options).   
+0000a4b0: 2069 6620 6e6f 7420 736f 6c2e 7375 6363   if not sol.succ
+0000a4c0: 6573 733a 0a20 2020 2020 2020 2070 7269  ess:.        pri
+0000a4d0: 6e74 2822 4120 4272 7567 6765 6d61 6e20  nt("A Bruggeman 
+0000a4e0: 736f 6c75 7469 6f6e 2077 6173 206e 6f74  solution was not
+0000a4f0: 2066 6f75 6e64 2061 7420 7468 6973 2066   found at this f
+0000a500: 7265 7175 656e 6379 2229 0a20 2020 2076  requency").    v
+0000a510: 6172 6961 626c 6573 203d 2073 6f6c 2e78  ariables = sol.x
+0000a520: 0a20 2020 2023 2074 7261 6e73 666f 726d  .    # transform
+0000a530: 2074 6865 2069 6d61 6769 6e61 7279 2076   the imaginary v
+0000a540: 6172 6961 626c 6520 6261 636b 0a20 2020  ariable back.   
+0000a550: 2074 7261 6365 203d 2063 6f6d 706c 6578   trace = complex
+0000a560: 2876 6172 6961 626c 6573 5b30 5d2c 206e  (variables[0], n
+0000a570: 702e 6578 7028 7661 7269 6162 6c65 735b  p.exp(variables[
+0000a580: 315d 292d 312e 3029 0a20 2020 2065 7073  1])-1.0).    eps
+0000a590: 6272 203d 206e 702e 6172 7261 7928 5b5b  br = np.array([[
+0000a5a0: 7472 6163 652c 2030 2c20 305d 2c20 5b30  trace, 0, 0], [0
+0000a5b0: 2c20 7472 6163 652c 2030 5d2c 205b 302c  , trace, 0], [0,
+0000a5c0: 2030 2c20 7472 6163 655d 5d29 0a20 2020   0, trace]]).   
+0000a5d0: 2072 6574 7572 6e20 6570 7362 720a 0a64   return epsbr..d
+0000a5e0: 6566 2062 7275 6767 656d 616e 5f69 7465  ef bruggeman_ite
+0000a5f0: 7228 2065 7073 312c 2065 7073 322c 2073  r( eps1, eps2, s
+0000a600: 6861 7065 2c20 4c2c 2066 322c 2073 697a  hape, L, f2, siz
+0000a610: 652c 2065 7073 6272 293a 0a20 2020 2022  e, epsbr):.    "
+0000a620: 2222 4361 6c63 756c 6174 6520 7468 6520  ""Calculate the 
+0000a630: 6566 6665 6374 6976 6520 636f 6e73 7461  effective consta
+0000a640: 6e74 2070 6572 6d69 7474 6976 6974 7920  nt permittivity 
+0000a650: 7573 696e 6720 7468 6520 6d65 7468 6f64  using the method
+0000a660: 206f 6620 6272 7567 6765 6d61 6e0a 2020   of bruggeman.  
+0000a670: 2020 2020 2065 7073 3120 6973 2074 6865       eps1 is the
+0000a680: 2064 6965 6c65 6374 7269 6320 636f 6e73   dielectric cons
+0000a690: 7461 6e74 2074 656e 736f 7220 6f66 2031  tant tensor of 1
+0000a6a0: 2028 5468 6520 6d65 6469 756d 290a 2020   (The medium).  
+0000a6b0: 2020 2020 2065 7073 3220 6973 2074 6865       eps2 is the
+0000a6c0: 2064 6965 6c65 6374 7269 6320 636f 6e73   dielectric cons
+0000a6d0: 7461 6e74 2074 656e 736f 7220 6f66 2032  tant tensor of 2
+0000a6e0: 2028 5468 6520 696e 636c 7573 696f 6e29   (The inclusion)
+0000a6f0: 0a20 2020 2020 2020 7368 6170 6520 6973  .       shape is
+0000a700: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+0000a710: 2063 7572 7265 6e74 2073 6861 7065 0a20   current shape. 
+0000a720: 2020 2020 2020 4c20 6973 2074 6865 2073        L is the s
+0000a730: 6861 7065 7320 6465 706f 6c61 7269 7361  hapes depolarisa
+0000a740: 7469 6f6e 206d 6174 7269 780a 2020 2020  tion matrix.    
+0000a750: 2020 2066 3220 6973 2074 6865 2076 6f6c     f2 is the vol
+0000a760: 756d 6520 6672 6163 7469 6f6e 206f 6620  ume fraction of 
+0000a770: 636f 6d70 6f6e 656e 7420 320a 2020 2020  component 2.    
+0000a780: 2020 2073 697a 6520 6973 2074 6865 2064     size is the d
+0000a790: 696d 656e 7369 6f6e 6c65 7373 2073 697a  imensionless siz
+0000a7a0: 6520 7061 7261 6d65 7465 7220 666f 7220  e parameter for 
+0000a7b0: 7468 6520 6672 6571 7565 6e63 7920 756e  the frequency un
+0000a7c0: 6465 7220 636f 6e73 6964 6572 6174 696f  der consideratio
+0000a7d0: 6e0a 2020 2020 2020 2065 7073 6272 2069  n.       epsbr i
+0000a7e0: 7320 616e 2069 6e69 7469 616c 2067 7565  s an initial gue
+0000a7f0: 7373 2061 7420 7468 6520 736f 6c75 7469  ss at the soluti
+0000a800: 6f6e 0a20 2020 2020 2020 5468 6520 726f  on.       The ro
+0000a810: 7574 696e 6520 7265 7475 726e 7320 7468  utine returns th
+0000a820: 6520 6566 6665 6374 6976 6520 6469 656c  e effective diel
+0000a830: 6563 7472 6963 2063 6f6e 7374 616e 740a  ectric constant.
+0000a840: 2020 2020 2020 204f 6e20 7468 6520 6170         On the ap
+0000a850: 706c 6963 6174 696f 6e20 6f66 2068 6f6d  plication of hom
+0000a860: 6f67 656e 697a 6174 696f 6e20 666f 726d  ogenization form
+0000a870: 616c 6973 6d73 2074 6f20 6163 7469 7665  alisms to active
+0000a880: 2064 6965 6c65 6374 7269 6320 636f 6d70   dielectric comp
+0000a890: 6f73 6974 6520 6d61 7465 7269 616c 730a  osite materials.
+0000a8a0: 2020 2020 2020 2054 6f6d 2047 2e20 4d61         Tom G. Ma
+0000a8b0: 636b 6179 2c20 416b 686c 6573 6820 4c61  ckay, Akhlesh La
+0000a8c0: 6b68 7461 6b69 6120 2222 220a 2020 2020  khtakia """.    
+0000a8d0: 6631 203d 2031 2e30 202d 2066 320a 2020  f1 = 1.0 - f2.  
+0000a8e0: 2020 2320 7065 7266 6f72 6d20 616e 2069    # perform an i
+0000a8f0: 7465 7261 7469 6f6e 0a20 2020 2063 6f6e  teration.    con
+0000a900: 7665 7267 6564 203d 2046 616c 7365 0a20  verged = False. 
+0000a910: 2020 206e 6974 6572 7320 3d20 300a 2020     niters = 0.  
+0000a920: 2020 7768 696c 6520 6e6f 7420 636f 6e76    while not conv
+0000a930: 6572 6765 643a 0a20 2020 2020 2020 206e  erged:.        n
+0000a940: 6974 6572 7320 2b3d 2031 0a20 2020 2020  iters += 1.     
+0000a950: 2020 2065 7073 6272 2c20 6572 726f 7220     epsbr, error 
+0000a960: 3d20 5f62 7275 675f 6974 6572 5f65 7272  = _brug_iter_err
+0000a970: 6f72 2865 7073 6272 2c20 6570 7331 2c20  or(epsbr, eps1, 
+0000a980: 6570 7332 2c20 7368 6170 652c 204c 2c20  eps2, shape, L, 
+0000a990: 6631 2c20 7369 7a65 290a 2020 2020 2020  f1, size).      
+0000a9a0: 2020 6966 2061 6273 2865 7272 6f72 2920    if abs(error) 
+0000a9b0: 3c20 312e 3045 2d38 3a0a 2020 2020 2020  < 1.0E-8:.      
+0000a9c0: 2020 2020 2020 636f 6e76 6572 6765 6420        converged 
+0000a9d0: 3d20 5472 7565 0a20 2020 2020 2020 2069  = True.        i
+0000a9e0: 6620 6e69 7465 7273 203e 2033 3030 303a  f niters > 3000:
+0000a9f0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000aa00: 6e74 2822 4272 7567 6765 6d61 6e20 6974  nt("Bruggeman it
+0000aa10: 6572 6174 696f 6e73 2066 6169 6c65 642c  erations failed,
+0000aa20: 2065 7272 6f72 3d22 2c20 6572 726f 7229   error=", error)
+0000aa30: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0000aa40: 7665 7267 6564 203d 2054 7275 650a 2020  verged = True.  
+0000aa50: 2020 6570 7362 7220 3d20 6176 6572 6167    epsbr = averag
+0000aa60: 655f 7465 6e73 6f72 2865 7073 6272 290a  e_tensor(epsbr).
+0000aa70: 2020 2020 7265 7475 726e 2065 7073 6272      return epsbr
+0000aa80: 0a0a 6465 6620 6176 6572 6167 655f 7465  ..def average_te
+0000aa90: 6e73 6f72 2874 293a 0a20 2020 2022 2222  nsor(t):.    """
+0000aaa0: 5265 7475 726e 2074 6865 2061 7665 7261  Return the avera
+0000aab0: 6765 6420 7465 6e73 6f72 2222 220a 2020  ged tensor""".  
+0000aac0: 2020 6120 3d20 6e70 2e74 7261 6365 2874    a = np.trace(t
+0000aad0: 2920 2f20 332e 300a 2020 2020 7265 7475  ) / 3.0.    retu
+0000aae0: 726e 206e 702e 6172 7261 7928 5b5b 612c  rn np.array([[a,
+0000aaf0: 2030 2c20 305d 2c20 5b30 2c20 612c 2030   0, 0], [0, a, 0
+0000ab00: 5d2c 205b 302c 2030 2c20 615d 5d29 0a0a  ], [0, 0, a]])..
+0000ab10: 6465 6620 5f62 7275 675f 6d69 6e69 6d69  def _brug_minimi
+0000ab20: 7365 5f73 6361 6c61 7228 7661 7269 6162  se_scalar(variab
+0000ab30: 6c65 732c 2065 7073 312c 2065 7073 322c  les, eps1, eps2,
+0000ab40: 2073 6861 7065 2c20 4c2c 2066 312c 2073   shape, L, f1, s
+0000ab50: 697a 6529 3a0a 2020 2020 2222 2242 7275  ize):.    """Bru
+0000ab60: 6767 656d 616e 206d 6574 686f 6420 7573  ggeman method us
+0000ab70: 696e 6720 7363 616c 6172 2071 7561 6e74  ing scalar quant
+0000ab80: 6974 6965 7322 2222 0a20 2020 2023 2075  ities""".    # u
+0000ab90: 6e70 6163 6b20 7468 6520 636f 6d70 6c65  npack the comple
+0000aba0: 7820 6e75 6d62 6572 2066 726f 6d20 7468  x number from th
+0000abb0: 6520 7661 7269 6162 6c65 730a 2020 2020  e variables.    
+0000abc0: 2320 7477 6f20 7468 696e 6773 2067 6f69  # two things goi
+0000abd0: 6e67 206f 6e20 6865 7265 2e0a 2020 2020  ng on here..    
+0000abe0: 2320 312e 2074 6865 2074 776f 2076 6172  # 1. the two var
+0000abf0: 6961 626c 6573 2072 6566 6572 2074 6f20  iables refer to 
+0000ac00: 7468 6520 7265 616c 2061 6e64 2069 6d61  the real and ima
+0000ac10: 6769 6e61 7279 2063 6f6d 706f 6e65 6e74  ginary component
+0000ac20: 730a 2020 2020 2320 322e 2077 6520 7265  s.    # 2. we re
+0000ac30: 7175 6972 6520 7468 6520 696d 6167 696e  quire the imagin
+0000ac40: 6172 7920 636f 6d70 6f6e 656e 7420 746f  ary component to
+0000ac50: 2062 6520 706f 7369 7469 7665 0a20 2020   be positive.   
+0000ac60: 2074 7261 6365 203d 2063 6f6d 706c 6578   trace = complex
+0000ac70: 2876 6172 6961 626c 6573 5b30 5d2c 206e  (variables[0], n
+0000ac80: 702e 6578 7028 7661 7269 6162 6c65 735b  p.exp(variables[
+0000ac90: 315d 292d 312e 3029 0a20 2020 2065 7073  1])-1.0).    eps
+0000aca0: 6272 203d 206e 702e 6172 7261 7928 5b5b  br = np.array([[
+0000acb0: 7472 6163 652c 2030 2c20 305d 2c20 5b30  trace, 0, 0], [0
+0000acc0: 2c20 7472 6163 652c 2030 5d2c 205b 302c  , trace, 0], [0,
+0000acd0: 2030 2c20 7472 6163 655d 5d29 0a20 2020   0, trace]]).   
+0000ace0: 2066 3220 3d20 312e 3020 2d20 6631 0a20   f2 = 1.0 - f1. 
+0000acf0: 2020 2023 2049 6620 6170 7072 6f70 7269     # If appropri
+0000ad00: 6174 6520 6361 6c63 756c 6174 6520 6120  ate calculate a 
+0000ad10: 7369 7a65 2065 6666 6563 7420 7573 696e  size effect usin
+0000ad20: 6720 4571 7561 7469 6f6e 7320 3130 2e33  g Equations 10.3
+0000ad30: 3820 616e 6420 3130 2e33 3920 696e 2053  8 and 10.39 in S
+0000ad40: 6968 766f 6c61 0a20 2020 2073 697a 655f  ihvola.    size_
+0000ad50: 6661 6374 6f72 203d 2063 616c 6375 6c61  factor = calcula
+0000ad60: 7465 5f73 697a 655f 6661 6374 6f72 2873  te_size_factor(s
+0000ad70: 697a 6529 0a20 2020 2062 3120 3d20 6e70  ize).    b1 = np
+0000ad80: 2e64 6f74 284c 2c20 2865 7073 3120 2d20  .dot(L, (eps1 - 
+0000ad90: 6570 7362 7229 290a 2020 2020 6232 203d  epsbr)).    b2 =
+0000ada0: 2073 697a 655f 6661 6374 6f72 202a 206e   size_factor * n
+0000adb0: 702e 646f 7428 4c2c 2028 6570 7332 202d  p.dot(L, (eps2 -
+0000adc0: 2065 7073 6272 2929 0a20 2020 2074 6231   epsbr)).    tb1
+0000add0: 203d 206e 702e 7472 6163 6528 6231 292f   = np.trace(b1)/
+0000ade0: 332e 300a 2020 2020 7462 3220 3d20 6e70  3.0.    tb2 = np
+0000adf0: 2e74 7261 6365 2862 3229 2f33 2e30 0a20  .trace(b2)/3.0. 
+0000ae00: 2020 2074 6131 203d 2031 2e30 2f28 312e     ta1 = 1.0/(1.
+0000ae10: 3020 2b20 7462 3129 0a20 2020 2074 6132  0 + tb1).    ta2
+0000ae20: 203d 2031 2e30 2f28 312e 3020 2b20 7462   = 1.0/(1.0 + tb
+0000ae30: 3229 0a20 2020 2063 3120 3d20 6570 7331  2).    c1 = eps1
+0000ae40: 2d65 7073 6272 0a20 2020 2063 3220 3d20  -epsbr.    c2 = 
+0000ae50: 6570 7332 2d65 7073 6272 0a20 2020 2074  eps2-epsbr.    t
+0000ae60: 6331 203d 206e 702e 7472 6163 6528 6331  c1 = np.trace(c1
+0000ae70: 292f 332e 300a 2020 2020 7463 3220 3d20  )/3.0.    tc2 = 
+0000ae80: 6e70 2e74 7261 6365 2863 3229 2f33 2e30  np.trace(c2)/3.0
+0000ae90: 0a20 2020 2023 2061 6c70 6861 3120 616e  .    # alpha1 an
+0000aea0: 6420 3220 6172 6520 7468 6520 706f 6c61  d 2 are the pola
+0000aeb0: 7269 7361 6269 6c69 7469 6573 206f 6620  risabilities of 
+0000aec0: 3120 616e 6420 3220 696e 2074 6865 2065  1 and 2 in the e
+0000aed0: 6666 6563 7469 7665 206d 6564 6975 6d0a  ffective medium.
+0000aee0: 2020 2020 7461 6c70 6861 3120 3d20 7463      talpha1 = tc
+0000aef0: 3120 2a20 7461 310a 2020 2020 7461 6c70  1 * ta1.    talp
+0000af00: 6861 3220 3d20 7463 3220 2a20 7461 320a  ha2 = tc2 * ta2.
+0000af10: 2020 2020 6572 726f 7220 3d20 6631 2a74      error = f1*t
+0000af20: 616c 7068 6131 202b 2066 322a 7461 6c70  alpha1 + f2*talp
+0000af30: 6861 320a 2020 2020 6572 726f 7220 3d20  ha2.    error = 
+0000af40: 6e70 2e61 6273 2865 7272 6f72 2e63 6f6e  np.abs(error.con
+0000af50: 6a75 6761 7465 2829 202a 2065 7272 6f72  jugate() * error
+0000af60: 290a 2020 2020 2320 4e61 7374 7920 6973  ).    # Nasty is
+0000af70: 7375 6520 696e 2074 6865 2070 6f77 656c  sue in the powel
+0000af80: 6c20 6d65 7468 6f64 2c20 7468 6520 636f  l method, the co
+0000af90: 6e76 6572 6765 6e63 6520 6f6e 2074 6f6c  nvergence on tol
+0000afa0: 2069 7320 6769 7665 6e0a 2020 2020 2320   is given.    # 
+0000afb0: 7265 6c61 7469 7665 2074 6f20 7468 6520  relative to the 
+0000afc0: 736f 6c75 7469 6f6e 2028 302e 3029 2e20  solution (0.0). 
+0000afd0: 204f 6e6c 7920 6120 736d 616c 6c20 6e75   Only a small nu
+0000afe0: 6d62 6572 2069 7320 6164 6465 642e 0a20  mber is added.. 
+0000aff0: 2020 2023 2053 6f20 7765 2073 6869 6674     # So we shift
+0000b000: 2074 6865 2073 6f6c 7574 696f 6e20 6279   the solution by
+0000b010: 2031 2e30 2c20 7468 6520 746f 6c20 6973   1.0, the tol is
+0000b020: 206e 6f77 2072 656c 6174 6976 6520 746f   now relative to
+0000b030: 2031 2e30 0a20 2020 2072 6574 7572 6e20   1.0.    return 
+0000b040: 312e 302b 6572 726f 720a 0a64 6566 205f  1.0+error..def _
+0000b050: 6272 7567 5f6d 696e 696d 6973 655f 7465  brug_minimise_te
+0000b060: 6e73 6f72 2876 6172 6961 626c 6573 2c20  nsor(variables, 
+0000b070: 6570 7331 2c20 6570 7332 2c20 7368 6170  eps1, eps2, shap
+0000b080: 652c 204c 2c20 6631 2c20 7369 7a65 293a  e, L, f1, size):
+0000b090: 0a20 2020 2022 2222 4272 7567 6765 6d61  .    """Bruggema
+0000b0a0: 6e20 6d65 7468 6f64 2075 7369 6e67 2074  n method using t
+0000b0b0: 656e 736f 7220 7175 616e 7469 7469 6573  ensor quantities
+0000b0c0: 2222 220a 2020 2020 2320 756e 7061 636b  """.    # unpack
+0000b0d0: 2074 6865 2063 6f6d 706c 6578 206e 756d   the complex num
+0000b0e0: 6265 7220 6672 6f6d 2074 6865 2076 6172  ber from the var
+0000b0f0: 6961 626c 6573 0a20 2020 2023 2074 776f  iables.    # two
+0000b100: 2074 6869 6e67 7320 676f 696e 6720 6f6e   things going on
+0000b110: 2068 6572 652e 0a20 2020 2023 2031 2e20   here..    # 1. 
+0000b120: 7468 6520 7477 6f20 7661 7269 6162 6c65  the two variable
+0000b130: 7320 7265 6665 7220 746f 2074 6865 2072  s refer to the r
+0000b140: 6561 6c20 616e 6420 696d 6167 696e 6172  eal and imaginar
+0000b150: 7920 636f 6d70 6f6e 656e 7473 0a20 2020  y components.   
+0000b160: 2023 2032 2e20 7765 2072 6571 7569 7265   # 2. we require
+0000b170: 2074 6865 2069 6d61 6769 6e61 7279 2063   the imaginary c
+0000b180: 6f6d 706f 6e65 6e74 2074 6f20 6265 2070  omponent to be p
+0000b190: 6f73 6974 6976 650a 2020 2020 7472 6163  ositive.    trac
+0000b1a0: 6520 3d20 636f 6d70 6c65 7828 7661 7269  e = complex(vari
+0000b1b0: 6162 6c65 735b 305d 2c20 6e70 2e65 7870  ables[0], np.exp
+0000b1c0: 2876 6172 6961 626c 6573 5b31 5d29 2d31  (variables[1])-1
+0000b1d0: 2e30 290a 2020 2020 6570 7362 7220 3d20  .0).    epsbr = 
+0000b1e0: 6e70 2e61 7272 6179 285b 5b74 7261 6365  np.array([[trace
+0000b1f0: 2c20 2030 2c20 305d 2c20 5b30 2c20 7472  ,  0, 0], [0, tr
+0000b200: 6163 652c 2030 5d2c 205b 302c 2030 2c20  ace, 0], [0, 0, 
+0000b210: 7472 6163 655d 5d29 0a20 2020 2066 3220  trace]]).    f2 
+0000b220: 3d20 312e 3020 2d20 6631 0a20 2020 2023  = 1.0 - f1.    #
+0000b230: 2049 6620 6170 7072 6f70 7269 6174 6520   If appropriate 
+0000b240: 6361 6c63 756c 6174 6520 6120 7369 7a65  calculate a size
+0000b250: 2065 6666 6563 7420 7573 696e 6720 4571   effect using Eq
+0000b260: 7561 7469 6f6e 7320 3130 2e33 3820 616e  uations 10.38 an
+0000b270: 6420 3130 2e33 3920 696e 2053 6968 766f  d 10.39 in Sihvo
+0000b280: 6c61 0a20 2020 2073 697a 655f 6661 6374  la.    size_fact
+0000b290: 6f72 203d 2063 616c 6375 6c61 7465 5f73  or = calculate_s
+0000b2a0: 697a 655f 6661 6374 6f72 2873 697a 6529  ize_factor(size)
+0000b2b0: 0a20 2020 2062 3120 3d20 6e70 2e64 6f74  .    b1 = np.dot
+0000b2c0: 284c 2c20 2865 7073 3120 2d20 6570 7362  (L, (eps1 - epsb
+0000b2d0: 7229 290a 2020 2020 6232 203d 2073 697a  r)).    b2 = siz
+0000b2e0: 655f 6661 6374 6f72 202a 206e 702e 646f  e_factor * np.do
+0000b2f0: 7428 4c2c 2028 6570 7332 202d 2065 7073  t(L, (eps2 - eps
+0000b300: 6272 2929 0a20 2020 2062 3120 3d20 6176  br)).    b1 = av
+0000b310: 6572 6167 655f 7465 6e73 6f72 2862 3129  erage_tensor(b1)
+0000b320: 0a20 2020 2062 3220 3d20 6176 6572 6167  .    b2 = averag
+0000b330: 655f 7465 6e73 6f72 2862 3229 0a20 2020  e_tensor(b2).   
+0000b340: 2061 3120 3d20 6e70 2e6c 696e 616c 672e   a1 = np.linalg.
+0000b350: 696e 7628 6570 7362 7220 2b20 6231 290a  inv(epsbr + b1).
+0000b360: 2020 2020 6132 203d 206e 702e 6c69 6e61      a2 = np.lina
+0000b370: 6c67 2e69 6e76 2865 7073 6272 202b 2062  lg.inv(epsbr + b
+0000b380: 3229 0a20 2020 2063 3120 3d20 6570 7331  2).    c1 = eps1
+0000b390: 2d65 7073 6272 0a20 2020 2063 3220 3d20  -epsbr.    c2 = 
+0000b3a0: 6570 7332 2d65 7073 6272 0a20 2020 2023  eps2-epsbr.    #
+0000b3b0: 2063 3120 3d20 6176 6572 6167 655f 7465   c1 = average_te
+0000b3c0: 6e73 6f72 2865 7073 312d 6570 7362 7229  nsor(eps1-epsbr)
+0000b3d0: 0a20 2020 2023 2063 3220 3d20 6176 6572  .    # c2 = aver
+0000b3e0: 6167 655f 7465 6e73 6f72 2865 7073 322d  age_tensor(eps2-
+0000b3f0: 6570 7362 7229 0a20 2020 2061 6c70 6861  epsbr).    alpha
+0000b400: 3120 3d20 6e70 2e64 6f74 2863 312c 2061  1 = np.dot(c1, a
+0000b410: 3129 0a20 2020 2061 6c70 6861 3220 3d20  1).    alpha2 = 
+0000b420: 6e70 2e64 6f74 2863 322c 2061 3229 0a20  np.dot(c2, a2). 
+0000b430: 2020 2061 6c70 6861 3120 3d20 6176 6572     alpha1 = aver
+0000b440: 6167 655f 7465 6e73 6f72 2861 6c70 6861  age_tensor(alpha
+0000b450: 3129 0a20 2020 2061 6c70 6861 3220 3d20  1).    alpha2 = 
+0000b460: 6176 6572 6167 655f 7465 6e73 6f72 2861  average_tensor(a
+0000b470: 6c70 6861 3229 0a20 2020 2065 7272 6f72  lpha2).    error
+0000b480: 203d 2066 312a 616c 7068 6131 202b 2066   = f1*alpha1 + f
+0000b490: 322a 616c 7068 6132 0a20 2020 2066 7220  2*alpha2.    fr 
+0000b4a0: 203d 2030 2e30 0a20 2020 2066 6920 203d   = 0.0.    fi  =
+0000b4b0: 2030 2e30 0a20 2020 2066 6f72 2063 2069   0.0.    for c i
+0000b4c0: 6e20 6572 726f 723a 0a20 2020 2020 2020  n error:.       
+0000b4d0: 2066 6f72 2066 2069 6e20 633a 0a20 2020   for f in c:.   
+0000b4e0: 2020 2020 2020 2020 2066 7220 2b3d 206e           fr += n
+0000b4f0: 702e 7265 616c 2866 292a 2a32 0a20 2020  p.real(f)**2.   
+0000b500: 2020 2020 2020 2020 2066 6920 2b3d 206e           fi += n
+0000b510: 702e 696d 6167 2866 292a 2a32 0a20 2020  p.imag(f)**2.   
+0000b520: 2065 7272 6f72 203d 206e 702e 6c69 6e61   error = np.lina
+0000b530: 6c67 2e6e 6f72 6d28 6572 726f 7229 0a20  lg.norm(error). 
+0000b540: 2020 2023 204e 6173 7479 2069 7373 7565     # Nasty issue
+0000b550: 2069 6e20 7468 6520 706f 7765 6c6c 206d   in the powell m
+0000b560: 6574 686f 642c 2074 6865 2063 6f6e 7665  ethod, the conve
+0000b570: 7267 656e 6365 206f 6e20 746f 6c20 6973  rgence on tol is
+0000b580: 2067 6976 656e 0a20 2020 2023 2072 656c   given.    # rel
+0000b590: 6174 6976 6520 746f 2074 6865 2073 6f6c  ative to the sol
+0000b5a0: 7574 696f 6e20 2830 2e30 292e 2020 4f6e  ution (0.0).  On
+0000b5b0: 6c79 2061 2073 6d61 6c6c 206e 756d 6265  ly a small numbe
+0000b5c0: 7220 6973 2061 6464 6564 2e0a 2020 2020  r is added..    
+0000b5d0: 2320 536f 2077 6520 7368 6966 7420 7468  # So we shift th
+0000b5e0: 6520 736f 6c75 7469 6f6e 2062 7920 312e  e solution by 1.
+0000b5f0: 302c 2074 6865 2074 6f6c 2069 7320 6e6f  0, the tol is no
+0000b600: 7720 7265 6c61 7469 7665 2074 6f20 312e  w relative to 1.
+0000b610: 300a 2020 2020 7265 7475 726e 2031 2e30  0.    return 1.0
+0000b620: 2b65 7272 6f72 0a0a 6465 6620 5f62 7275  +error..def _bru
+0000b630: 675f 6974 6572 5f65 7272 6f72 2865 7073  g_iter_error(eps
+0000b640: 6272 2c20 6570 7331 2c20 6570 7332 2c20  br, eps1, eps2, 
+0000b650: 7368 6170 652c 204c 2c20 6631 2c20 7369  shape, L, f1, si
+0000b660: 7a65 293a 0a20 2020 2022 2222 526f 7574  ze):.    """Rout
+0000b670: 696e 6520 746f 2063 616c 6375 6c61 7465  ine to calculate
+0000b680: 2074 6865 2065 7272 6f72 2069 6e20 7468   the error in th
+0000b690: 6520 4272 7567 6765 6d61 6e20 6d65 7468  e Bruggeman meth
+0000b6a0: 6f64 2222 220a 2020 2020 6632 203d 2031  od""".    f2 = 1
+0000b6b0: 2e30 202d 2066 310a 2020 2020 2320 4966  .0 - f1.    # If
+0000b6c0: 2061 7070 726f 7072 6961 7465 2063 616c   appropriate cal
+0000b6d0: 6375 6c61 7465 2061 2073 697a 6520 6566  culate a size ef
+0000b6e0: 6665 6374 2075 7369 6e67 2045 7175 6174  fect using Equat
+0000b6f0: 696f 6e73 2031 302e 3338 2061 6e64 2031  ions 10.38 and 1
+0000b700: 302e 3339 2069 6e20 5369 6876 6f6c 610a  0.39 in Sihvola.
+0000b710: 2020 2020 7369 7a65 5f66 6163 746f 7220      size_factor 
+0000b720: 3d20 6361 6c63 756c 6174 655f 7369 7a65  = calculate_size
+0000b730: 5f66 6163 746f 7228 7369 7a65 290a 2020  _factor(size).  
+0000b740: 2020 6c65 7073 3120 3d20 6e70 2e64 6f74    leps1 = np.dot
+0000b750: 284c 2c20 2865 7073 3120 2d20 6570 7362  (L, (eps1 - epsb
+0000b760: 7229 290a 2020 2020 6c65 7073 3220 3d20  r)).    leps2 = 
+0000b770: 7369 7a65 5f66 6163 746f 7220 2a20 6e70  size_factor * np
+0000b780: 2e64 6f74 284c 2c20 2865 7073 3220 2d20  .dot(L, (eps2 - 
+0000b790: 6570 7362 7229 290a 2020 2020 6c65 7073  epsbr)).    leps
+0000b7a0: 3120 3d20 6176 6572 6167 655f 7465 6e73  1 = average_tens
+0000b7b0: 6f72 286c 6570 7331 290a 2020 2020 6c65  or(leps1).    le
+0000b7c0: 7073 3220 3d20 6176 6572 6167 655f 7465  ps2 = average_te
+0000b7d0: 6e73 6f72 286c 6570 7332 290a 2020 2020  nsor(leps2).    
+0000b7e0: 6131 203d 206e 702e 6c69 6e61 6c67 2e69  a1 = np.linalg.i
+0000b7f0: 6e76 2865 7073 6272 202b 206c 6570 7331  nv(epsbr + leps1
+0000b800: 290a 2020 2020 6132 203d 206e 702e 6c69  ).    a2 = np.li
+0000b810: 6e61 6c67 2e69 6e76 2865 7073 6272 202b  nalg.inv(epsbr +
+0000b820: 206c 6570 7332 290a 2020 2020 2320 616c   leps2).    # al
+0000b830: 7068 6131 2061 6e64 2032 2061 7265 2074  pha1 and 2 are t
+0000b840: 6865 2070 6f6c 6172 6973 6162 696c 6974  he polarisabilit
+0000b850: 6965 7320 6f66 2031 2061 6e64 2032 2069  ies of 1 and 2 i
+0000b860: 6e20 7468 6520 6566 6665 6374 6976 6520  n the effective 
+0000b870: 6d65 6469 756d 0a20 2020 2065 7073 3161  medium.    eps1a
+0000b880: 7620 3d20 6176 6572 6167 655f 7465 6e73  v = average_tens
+0000b890: 6f72 2865 7073 3129 0a20 2020 2065 7073  or(eps1).    eps
+0000b8a0: 3261 7620 3d20 6176 6572 6167 655f 7465  2av = average_te
+0000b8b0: 6e73 6f72 2865 7073 3229 0a20 2020 2061  nsor(eps2).    a
+0000b8c0: 6c70 6861 3120 3d20 6e70 2e64 6f74 2828  lpha1 = np.dot((
+0000b8d0: 6570 7331 6176 2d65 7073 6272 292c 2061  eps1av-epsbr), a
+0000b8e0: 3129 0a20 2020 2061 6c70 6861 3220 3d20  1).    alpha2 = 
+0000b8f0: 6e70 2e64 6f74 2828 6570 7332 6176 2d65  np.dot((eps2av-e
+0000b900: 7073 6272 292c 2061 3229 0a20 2020 2023  psbr), a2).    #
+0000b910: 2074 6865 2065 7272 6f72 206f 7220 7265   the error or re
+0000b920: 7369 6475 616c 206d 6174 7269 7820 7368  sidual matrix sh
+0000b930: 6f75 6c64 2062 6520 7a65 726f 2066 6f72  ould be zero for
+0000b940: 2061 2062 7275 6767 656d 616e 2073 6f6c   a bruggeman sol
+0000b950: 7574 696f 6e0a 2020 2020 6572 726f 7220  ution.    error 
+0000b960: 3d20 6631 2a61 6c70 6861 3120 2b20 6632  = f1*alpha1 + f2
+0000b970: 2a61 6c70 6861 320a 2020 2020 6572 726f  *alpha2.    erro
+0000b980: 7220 3d20 6e70 2e6c 696e 616c 672e 6e6f  r = np.linalg.no
+0000b990: 726d 2865 7272 6f72 290a 2020 2020 6d31  rm(error).    m1
+0000b9a0: 203d 2066 312a 6e70 2e64 6f74 2865 7073   = f1*np.dot(eps
+0000b9b0: 312c 2061 3129 2b66 322a 6e70 2e64 6f74  1, a1)+f2*np.dot
+0000b9c0: 2865 7073 322c 2061 3229 0a20 2020 206d  (eps2, a2).    m
+0000b9d0: 3220 3d20 6e70 2e6c 696e 616c 672e 696e  2 = np.linalg.in
+0000b9e0: 7628 6631 2a61 3120 2b20 6632 2a61 3229  v(f1*a1 + f2*a2)
+0000b9f0: 0a20 2020 2064 616d 7020 3d20 302e 300a  .    damp = 0.0.
+0000ba00: 2020 2020 6570 7362 7220 3d20 2831 2e30      epsbr = (1.0
+0000ba10: 202d 2064 616d 7029 2a6e 702e 646f 7428   - damp)*np.dot(
+0000ba20: 6d31 2c20 6d32 2920 2b20 6461 6d70 2a65  m1, m2) + damp*e
+0000ba30: 7073 6272 0a20 2020 2074 7261 6365 203d  psbr.    trace =
+0000ba40: 206e 702e 7472 6163 6528 6570 7362 7229   np.trace(epsbr)
+0000ba50: 202f 2033 2e30 0a20 2020 2065 7073 6272   / 3.0.    epsbr
+0000ba60: 203d 206e 702e 6172 7261 7928 5b5b 7472   = np.array([[tr
+0000ba70: 6163 652c 2030 2c20 305d 2c20 5b30 2c20  ace, 0, 0], [0, 
+0000ba80: 7472 6163 652c 2030 5d2c 205b 302c 2030  trace, 0], [0, 0
+0000ba90: 2c20 7472 6163 655d 5d29 0a20 2020 2072  , trace]]).    r
+0000baa0: 6574 7572 6e20 6570 7362 722c 2065 7272  eturn epsbr, err
+0000bab0: 6f72 0a0a 6465 6620 6361 6c63 756c 6174  or..def calculat
+0000bac0: 655f 7265 6672 6163 7469 7665 5f69 6e64  e_refractive_ind
+0000bad0: 6578 2864 6965 6c65 6374 7269 632c 2064  ex(dielectric, d
+0000bae0: 6562 7567 3d46 616c 7365 293a 0a20 2020  ebug=False):.   
+0000baf0: 2027 2727 2043 616c 6375 6c61 7465 2074   ''' Calculate t
+0000bb00: 6865 2072 6566 7261 6374 6976 6520 696e  he refractive in
+0000bb10: 6465 7820 6672 6f6d 2074 6865 2064 6965  dex from the die
+0000bb20: 6c65 6374 7269 6320 636f 6e73 7461 6e74  lectric constant
+0000bb30: 2e0a 2020 2020 2020 2020 4361 6c63 756c  ..        Calcul
+0000bb40: 6174 6520 7468 6520 7472 6163 6520 6f66  ate the trace of
+0000bb50: 2074 6865 2064 6965 6c65 6374 7269 6320   the dielectric 
+0000bb60: 616e 6420 6361 6c63 756c 6174 6520 626f  and calculate bo
+0000bb70: 7468 2073 7175 6172 6520 726f 6f74 732e  th square roots.
+0000bb80: 0a20 2020 2020 2020 2054 6865 2063 686f  .        The cho
+0000bb90: 6f73 6520 7468 6520 726f 6f74 2077 6974  ose the root wit
+0000bba0: 6820 7468 6520 6c61 7267 6573 7420 696d  h the largest im
+0000bbb0: 6167 696e 6172 7920 636f 6d70 6f6e 656e  aginary componen
+0000bbc0: 7420 5468 6973 206f 6265 7973 2074 6865  t This obeys the
+0000bbd0: 204b 6f6e 6967 204b 7261 6d65 7220 7265   Konig Kramer re
+0000bbe0: 7175 6972 656d 656e 7473 2727 270a 2020  quirements'''.  
+0000bbf0: 2020 7472 6163 6520 3d20 6e70 2e74 7261    trace = np.tra
+0000bc00: 6365 2864 6965 6c65 6374 7269 6329 2f33  ce(dielectric)/3
+0000bc10: 2e30 0a20 2020 2073 6f6c 7574 696f 6e20  .0.    solution 
+0000bc20: 3d20 6361 6c63 756c 6174 655f 7265 6672  = calculate_refr
+0000bc30: 6163 7469 7665 5f69 6e64 6578 5f73 6361  active_index_sca
+0000bc40: 6c61 7228 7472 6163 652c 2064 6562 7567  lar(trace, debug
+0000bc50: 290a 2020 2020 7265 7475 726e 2073 6f6c  ).    return sol
+0000bc60: 7574 696f 6e0a 0a64 6566 2063 616c 6375  ution..def calcu
+0000bc70: 6c61 7465 5f72 6566 7261 6374 6976 655f  late_refractive_
+0000bc80: 696e 6465 785f 7363 616c 6172 2864 6965  index_scalar(die
+0000bc90: 6c65 6374 7269 635f 7363 616c 6172 2c20  lectric_scalar, 
+0000bca0: 6465 6275 673d 4661 6c73 6529 3a0a 2020  debug=False):.  
+0000bcb0: 2020 2727 2720 4361 6c63 756c 6174 6520    ''' Calculate 
+0000bcc0: 7468 6520 7265 6672 6163 7469 7665 2069  the refractive i
+0000bcd0: 6e64 6578 2066 726f 6d20 7468 6520 6469  ndex from the di
+0000bce0: 656c 6563 7472 6963 2063 6f6e 7374 616e  electric constan
+0000bcf0: 742e 0a20 2020 2020 2020 2043 616c 6375  t..        Calcu
+0000bd00: 6c61 7465 2074 6865 2074 7261 6365 206f  late the trace o
+0000bd10: 6620 7468 6520 6469 656c 6563 7472 6963  f the dielectric
+0000bd20: 2061 6e64 2063 616c 6375 6c61 7465 2062   and calculate b
+0000bd30: 6f74 6820 7371 7561 7265 2072 6f6f 7473  oth square roots
+0000bd40: 2e0a 2020 2020 2020 2020 5468 6520 6368  ..        The ch
+0000bd50: 6f6f 7365 2074 6865 2072 6f6f 7420 7769  oose the root wi
+0000bd60: 7468 2074 6865 206c 6172 6765 7374 2069  th the largest i
+0000bd70: 6d61 6769 6e61 7279 2063 6f6d 706f 6e65  maginary compone
+0000bd80: 6e74 2054 6869 7320 6f62 6579 7320 7468  nt This obeys th
+0000bd90: 6520 4b6f 6e69 6720 4b72 616d 6572 2072  e Konig Kramer r
+0000bda0: 6571 7569 7265 6d65 6e74 7327 2727 0a20  equirements'''. 
+0000bdb0: 2020 2073 6f6c 7574 696f 6e31 203d 206e     solution1 = n
+0000bdc0: 702e 7371 7274 2864 6965 6c65 6374 7269  p.sqrt(dielectri
+0000bdd0: 635f 7363 616c 6172 290a 2020 2020 722c  c_scalar).    r,
+0000bde0: 2070 6861 7365 203d 2063 6d61 7468 2e70   phase = cmath.p
+0000bdf0: 6f6c 6172 2873 6f6c 7574 696f 6e31 290a  olar(solution1).
+0000be00: 2020 2020 736f 6c75 7469 6f6e 3220 3d20      solution2 = 
+0000be10: 636d 6174 682e 7265 6374 282d 722c 2070  cmath.rect(-r, p
+0000be20: 6861 7365 290a 2020 2020 696d 6167 3120  hase).    imag1 
+0000be30: 3d20 6e70 2e69 6d61 6728 736f 6c75 7469  = np.imag(soluti
+0000be40: 6f6e 3129 0a20 2020 2069 6d61 6732 203d  on1).    imag2 =
+0000be50: 206e 702e 696d 6167 2873 6f6c 7574 696f   np.imag(solutio
+0000be60: 6e32 290a 2020 2020 6966 2069 6d61 6731  n2).    if imag1
+0000be70: 203e 2069 6d61 6732 3a0a 2020 2020 2020   > imag2:.      
+0000be80: 2020 736f 6c75 7469 6f6e 203d 2073 6f6c    solution = sol
+0000be90: 7574 696f 6e31 0a20 2020 2065 6c73 653a  ution1.    else:
+0000bea0: 0a20 2020 2020 2020 2073 6f6c 7574 696f  .        solutio
+0000beb0: 6e20 3d20 736f 6c75 7469 6f6e 320a 2020  n = solution2.  
+0000bec0: 2020 6966 206e 702e 6162 7328 736f 6c75    if np.abs(solu
+0000bed0: 7469 6f6e 2a73 6f6c 7574 696f 6e2d 6469  tion*solution-di
+0000bee0: 656c 6563 7472 6963 5f73 6361 6c61 7229  electric_scalar)
+0000bef0: 2f28 312b 6e70 2e61 6273 2864 6965 6c65  /(1+np.abs(diele
+0000bf00: 6374 7269 635f 7363 616c 6172 2929 203e  ctric_scalar)) >
+0000bf10: 2031 2e30 452d 3820 6f72 2064 6562 7567   1.0E-8 or debug
+0000bf20: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+0000bf30: 2254 6865 7265 2069 7320 616e 2065 7272  "There is an err
+0000bf40: 6f72 2069 6e20 7265 6672 6163 7469 7665  or in refractive
+0000bf50: 2069 6e64 6578 2229 0a20 2020 2020 2020   index").       
+0000bf60: 2070 7269 6e74 2822 4469 656c 6563 7472   print("Dielectr
+0000bf70: 6963 203d 2022 2c20 6469 656c 6563 7472  ic = ", dielectr
+0000bf80: 6963 5f73 6361 6c61 7229 0a20 2020 2020  ic_scalar).     
+0000bf90: 2020 2070 7269 6e74 2822 736f 6c75 7469     print("soluti
+0000bfa0: 6f6e 2a73 6f6c 7574 696f 6e20 3d20 222c  on*solution = ",
+0000bfb0: 2073 6f6c 7574 696f 6e2a 736f 6c75 7469   solution*soluti
+0000bfc0: 6f6e 2c20 6e70 2e61 6273 2873 6f6c 7574  on, np.abs(solut
+0000bfd0: 696f 6e2a 736f 6c75 7469 6f6e 2d64 6965  ion*solution-die
+0000bfe0: 6c65 6374 7269 635f 7363 616c 6172 2929  lectric_scalar))
+0000bff0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000c000: 736f 6c75 7469 6f6e 2020 2020 3d20 222c  solution    = ",
+0000c010: 2073 6f6c 7574 696f 6e2c 2073 6f6c 7574   solution, solut
+0000c020: 696f 6e2a 736f 6c75 7469 6f6e 290a 2020  ion*solution).  
+0000c030: 2020 2020 2020 7072 696e 7428 2273 6f6c        print("sol
+0000c040: 7574 696f 6e31 2020 203d 2022 2c20 736f  ution1   = ", so
+0000c050: 6c75 7469 6f6e 312c 2073 6f6c 7574 696f  lution1, solutio
+0000c060: 6e31 2a73 6f6c 7574 696f 6e31 290a 2020  n1*solution1).  
+0000c070: 2020 2020 2020 7072 696e 7428 2273 6f6c        print("sol
+0000c080: 7574 696f 6e32 2020 203d 2022 2c20 736f  ution2   = ", so
+0000c090: 6c75 7469 6f6e 322c 2073 6f6c 7574 696f  lution2, solutio
+0000c0a0: 6e32 2a73 6f6c 7574 696f 6e32 290a 2020  n2*solution2).  
+0000c0b0: 2020 7265 7475 726e 2073 6f6c 7574 696f    return solutio
+0000c0c0: 6e0a 0a64 6566 2064 6972 6563 7469 6f6e  n..def direction
+0000c0d0: 5f66 726f 6d5f 7368 6170 6528 6461 7461  _from_shape(data
+0000c0e0: 2c20 7265 6164 6572 293a 0a20 2020 2022  , reader):.    "
+0000c0f0: 2222 2044 6574 6572 6d69 6e65 2074 6865  "" Determine the
+0000c100: 2075 6e69 7175 6520 6469 7265 6374 696f   unique directio
+0000c110: 6e20 6f66 2074 6865 2073 6861 7065 2066  n of the shape f
+0000c120: 726f 6d20 6461 7461 0a20 2020 2064 6174  rom data.    dat
+0000c130: 6120 6d61 7920 636f 6e74 6169 6e20 6120  a may contain a 
+0000c140: 6d69 6c6c 6572 2069 6e64 6963 6573 2077  miller indices w
+0000c150: 6869 6368 2064 6566 696e 6573 2061 2073  hich defines a s
+0000c160: 7572 6661 6365 2065 672e 2028 312c 312c  urface eg. (1,1,
+0000c170: 2d31 290a 2020 2020 6f72 2061 2064 6972  -1).    or a dir
+0000c180: 6563 7469 6f6e 2061 7320 6120 6d69 6c6c  ection as a mill
+0000c190: 6572 2064 6972 6563 7469 6f6e 2076 6563  er direction vec
+0000c1a0: 746f 7220 6567 2e20 5b31 2c30 2c2d 315d  tor eg. [1,0,-1]
+0000c1b0: 2022 2222 0a20 2020 2073 7572 6661 6365   """.    surface
+0000c1c0: 203d 2046 616c 7365 0a20 2020 2023 206f   = False.    # o
+0000c1d0: 7269 6769 6e61 6c20 3d20 6461 7461 0a20  riginal = data. 
+0000c1e0: 2020 2069 203d 2064 6174 612e 6669 6e64     i = data.find
+0000c1f0: 2822 2c22 290a 2020 2020 636f 6d6d 6173  (",").    commas
+0000c200: 203d 2046 616c 7365 0a20 2020 2069 6620   = False.    if 
+0000c210: 6920 3e3d 2030 3a0a 2020 2020 2020 2020  i >= 0:.        
+0000c220: 636f 6d6d 6173 203d 2054 7275 650a 2020  commas = True.  
+0000c230: 2020 6966 2064 6174 615b 305d 203d 3d20    if data[0] == 
+0000c240: 227b 223a 0a20 2020 2020 2020 2073 7572  "{":.        sur
+0000c250: 6661 6365 203d 2054 7275 650a 2020 2020  face = True.    
+0000c260: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+0000c270: 7265 706c 6163 6528 227b 222c 2022 2229  replace("{", "")
+0000c280: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0000c290: 6461 7461 2e72 6570 6c61 6365 2822 7d22  data.replace("}"
+0000c2a0: 2c20 2222 290a 2020 2020 656c 6966 2064  , "").    elif d
+0000c2b0: 6174 615b 305d 203d 3d20 2228 223a 0a20  ata[0] == "(":. 
+0000c2c0: 2020 2020 2020 2073 7572 6661 6365 203d         surface =
+0000c2d0: 2054 7275 650a 2020 2020 2020 2020 6461   True.        da
+0000c2e0: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+0000c2f0: 6528 2228 222c 2022 2229 0a20 2020 2020  e("(", "").     
+0000c300: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0000c310: 6570 6c61 6365 2822 2922 2c20 2222 290a  eplace(")", "").
+0000c320: 2020 2020 656c 6966 2064 6174 615b 305d      elif data[0]
+0000c330: 203d 3d20 225b 223a 0a20 2020 2020 2020   == "[":.       
+0000c340: 2073 7572 6661 6365 203d 2046 616c 7365   surface = False
+0000c350: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0000c360: 6461 7461 2e72 6570 6c61 6365 2822 5b22  data.replace("["
+0000c370: 2c20 2222 290a 2020 2020 2020 2020 6461  , "").        da
+0000c380: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+0000c390: 6528 225d 222c 2022 2229 0a20 2020 2065  e("]", "").    e
+0000c3a0: 6c73 653a 0a20 2020 2020 2020 2070 7269  lse:.        pri
+0000c3b0: 6e74 2822 4572 726f 7220 656e 636f 756e  nt("Error encoun
+0000c3c0: 7465 7265 6420 696e 2069 6e74 6572 7072  tered in interpr
+0000c3d0: 6574 7469 6e67 2074 6865 206d 696c 6c65  etting the mille
+0000c3e0: 7220 7375 7266 6163 6520 2f20 7665 6374  r surface / vect
+0000c3f0: 6f72 222c 2064 6174 6129 0a20 2020 2020  or", data).     
+0000c400: 2020 2065 7869 7428 3129 0a20 2020 2069     exit(1).    i
+0000c410: 6620 636f 6d6d 6173 3a0a 2020 2020 2020  f commas:.      
+0000c420: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+0000c430: 706c 6163 6528 222c 222c 2022 2022 290a  place(",", " ").
+0000c440: 2020 2020 2020 2020 686b 6c20 3d20 285b          hkl = ([
+0000c450: 696e 7428 6629 2066 6f72 2066 2069 6e20  int(f) for f in 
+0000c460: 6461 7461 2e73 706c 6974 2829 5d29 0a20  data.split()]). 
+0000c470: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c480: 2069 203d 2030 0a20 2020 2020 2020 2068   i = 0.        h
+0000c490: 6b6c 203d 205b 302c 2030 2c20 305d 0a20  kl = [0, 0, 0]. 
+0000c4a0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+0000c4b0: 5b30 2c20 312c 2032 5d3a 0a20 2020 2020  [0, 1, 2]:.     
+0000c4c0: 2020 2020 2020 2073 6967 6e20 3d20 310a         sign = 1.
+0000c4d0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0000c4e0: 6174 615b 695d 203d 3d20 222d 223a 0a20  ata[i] == "-":. 
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c500: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
+0000c510: 2020 2020 2020 7369 676e 203d 202d 310a        sign = -1.
+0000c520: 2020 2020 2020 2020 2020 2020 686b 6c5b              hkl[
+0000c530: 6b5d 203d 2073 6967 6e20 2a20 696e 7428  k] = sign * int(
+0000c540: 6461 7461 5b69 5d29 0a20 2020 2020 2020  data[i]).       
+0000c550: 2020 2020 2069 202b 3d20 310a 2020 2020       i += 1.    
+0000c560: 2320 656e 6420 6f66 2068 616e 646c 696e  # end of handlin
+0000c570: 6720 6e6f 2063 6f6d 6d61 730a 2020 2020  g no commas.    
+0000c580: 6966 206e 6f74 206c 656e 2868 6b6c 2920  if not len(hkl) 
+0000c590: 3d3d 2033 3a0a 2020 2020 2020 2020 7072  == 3:.        pr
+0000c5a0: 696e 7428 2245 7272 6f72 2065 6e63 6f75  int("Error encou
+0000c5b0: 6e74 6572 6564 2069 6e20 696e 7465 7270  ntered in interp
+0000c5c0: 7265 7474 696e 6720 7468 6520 6d69 6c6c  retting the mill
+0000c5d0: 6572 2073 7572 6661 6365 202f 2076 6563  er surface / vec
+0000c5e0: 746f 7222 2c20 6461 7461 290a 2020 2020  tor", data).    
+0000c5f0: 2020 2020 6578 6974 2831 290a 2020 2020      exit(1).    
+0000c600: 6365 6c6c 203d 2072 6561 6465 722e 756e  cell = reader.un
+0000c610: 6974 5f63 656c 6c73 5b2d 315d 0a20 2020  it_cells[-1].   
+0000c620: 2069 6620 7375 7266 6163 653a 0a20 2020   if surface:.   
+0000c630: 2020 2020 2064 6972 6563 7469 6f6e 203d       direction =
+0000c640: 2063 656c 6c2e 636f 6e76 6572 745f 686b   cell.convert_hk
+0000c650: 6c5f 746f 5f78 797a 2868 6b6c 290a 2020  l_to_xyz(hkl).  
+0000c660: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000c670: 6469 7265 6374 696f 6e20 3d20 6365 6c6c  direction = cell
+0000c680: 2e63 6f6e 7665 7274 5f61 6263 5f74 6f5f  .convert_abc_to_
+0000c690: 7879 7a28 686b 6c29 0a20 2020 2064 6972  xyz(hkl).    dir
+0000c6a0: 6563 7469 6f6e 203d 2064 6972 6563 7469  ection = directi
+0000c6b0: 6f6e 202f 206e 702e 6c69 6e61 6c67 2e6e  on / np.linalg.n
+0000c6c0: 6f72 6d28 6469 7265 6374 696f 6e29 0a20  orm(direction). 
+0000c6d0: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0000c6e0: 6570 6c61 6365 2827 2227 2c20 2727 290a  eplace('"', '').
+0000c6f0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+0000c700: 7265 706c 6163 6528 2222 2c20 2727 290a  replace("", '').
+0000c710: 2020 2020 2320 6966 2073 7572 6661 6365      # if surface
+0000c720: 3a0a 2020 2020 2320 2020 2020 7072 696e  :.    #     prin
+0000c730: 7428 2254 6865 206d 696c 6c65 7220 696e  t("The miller in
+0000c740: 6469 6365 7320 666f 7220 7468 6520 7375  dices for the su
+0000c750: 7266 6163 6520 222c 206f 7269 6769 6e61  rface ", origina
+0000c760: 6c2c 2022 6861 7320 6120 6e6f 726d 616c  l, "has a normal
+0000c770: 222c 2064 6972 6563 7469 6f6e 2c20 2269  ", direction, "i
+0000c780: 6e20 7879 7a22 290a 2020 2020 2320 656c  n xyz").    # el
+0000c790: 7365 3a0a 2020 2020 2320 2020 2070 7269  se:.    #    pri
+0000c7a0: 6e74 2822 5468 6520 6d69 6c6c 6572 2064  nt("The miller d
+0000c7b0: 6972 6563 7469 6f6e 2022 2c20 6f72 6967  irection ", orig
+0000c7c0: 696e 616c 2c20 2269 7320 222c 2064 6972  inal, "is ", dir
+0000c7d0: 6563 7469 6f6e 2c20 2269 6e20 7879 7a22  ection, "in xyz"
+0000c7e0: 290a 2020 2020 7265 7475 726e 2064 6972  ).    return dir
+0000c7f0: 6563 7469 6f6e 0a0a 6465 6620 736f 6c76  ection..def solv
+0000c800: 655f 6566 6665 6374 6976 655f 6d65 6469  e_effective_medi
+0000c810: 756d 5f65 7175 6174 696f 6e73 2820 0a20  um_equations( . 
+0000c820: 2020 2020 2020 206d 6574 686f 6420 2020         method   
+0000c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c840: 2c0a 2020 2020 2020 2020 7666 2020 2020  ,.        vf    
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 202c 0a20 2020 2020 2020 2073 697a     ,.        siz
+0000c870: 655f 6d75 2020 2020 2020 2020 2020 2020  e_mu            
+0000c880: 2020 2020 2020 2c0a 2020 2020 2020 2020        ,.        
+0000c890: 7369 7a65 5f64 6973 7472 6962 7574 696f  size_distributio
+0000c8a0: 6e5f 7369 676d 6120 202c 0a20 2020 2020  n_sigma  ,.     
+0000c8b0: 2020 2064 6965 6c65 6374 7269 635f 6d65     dielectric_me
+0000c8c0: 6469 756d 2020 2020 2020 2020 2c0a 2020  dium        ,.  
+0000c8d0: 2020 2020 2020 7368 6170 6520 2020 2020        shape     
+0000c8e0: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
+0000c8f0: 0a20 2020 2020 2020 204c 2020 2020 2020  .        L      
+0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c910: 2020 2c0a 2020 2020 2020 2020 636f 6e63    ,.        conc
+0000c920: 656e 7472 6174 696f 6e20 2020 2020 2020  entration       
+0000c930: 2020 2020 202c 0a20 2020 2020 2020 2061       ,.        a
+0000c940: 7472 5065 726d 6974 7469 7669 7479 2020  trPermittivity  
+0000c950: 2020 2020 2020 2020 2c0a 2020 2020 2020          ,.      
+0000c960: 2020 6174 7254 6865 7461 2020 2020 2020    atrTheta      
+0000c970: 2020 2020 2020 2020 2020 202c 0a20 2020             ,.   
+0000c980: 2020 2020 2061 7472 5350 6f6c 2020 2020       atrSPol    
+0000c990: 2020 2020 2020 2020 2020 2020 2020 2c0a                ,.
+0000c9a0: 2020 2020 2020 2020 6275 6262 6c65 5f76          bubble_v
+0000c9b0: 6620 2020 2020 2020 2020 2020 2020 2020  f               
+0000c9c0: 202c 0a20 2020 2020 2020 2062 7562 626c   ,.        bubbl
+0000c9d0: 655f 7261 6469 7573 2020 2020 2020 2020  e_radius        
+0000c9e0: 2020 2020 2c0a 2020 2020 2020 2020 7072      ,.        pr
+0000c9f0: 6576 696f 7573 5f73 6f6c 7574 696f 6e5f  evious_solution_
+0000ca00: 7368 6172 6564 202c 0a20 2020 2020 2020  shared ,.       
+0000ca10: 2070 6172 616d 7320 2020 2020 2020 2020   params         
+0000ca20: 2020 2020 2020 2020 202c 0a20 2020 2020           ,.     
+0000ca30: 2020 2029 3a0a 2020 2020 2320 6361 6c6c     ):.    # call
+0000ca40: 5f70 6172 616d 6574 6572 7320 6973 2061  _parameters is a
+0000ca50: 6e20 696e 6465 7820 696e 746f 2074 6865  n index into the
+0000ca60: 2066 7265 7175 656e 6379 2061 6e64 2064   frequency and d
+0000ca70: 6965 6c65 6374 7269 6320 6172 7261 7973  ielectric arrays
+0000ca80: 0a20 2020 2023 2049 6e20 7468 6520 6361  .    # In the ca
+0000ca90: 7365 206f 6620 4272 7567 6765 6d61 6e20  se of Bruggeman 
+0000caa0: 616e 6420 636f 6865 7265 6e74 2077 6520  and coherent we 
+0000cab0: 6361 6e20 7573 6520 7468 6520 7072 6576  can use the prev
+0000cac0: 696f 7573 2072 6573 756c 7420 746f 2073  ious result to s
+0000cad0: 7461 7274 2074 6865 2069 7465 7261 7469  tart the iterati
+0000cae0: 6f6e 2f6d 696e 696d 6973 6174 696f 6e0a  on/minimisation.
+0000caf0: 2020 2020 2320 486f 7765 7665 7220 746f      # However to
+0000cb00: 2064 6f20 7468 6973 2077 6520 6e65 6564   do this we need
+0000cb10: 2073 6f6d 6520 7368 6172 6564 206d 656d   some shared mem
+0000cb20: 6f72 792c 2074 6869 7320 616c 6c6f 6361  ory, this alloca
+0000cb30: 7465 6420 696e 2070 7265 7669 6f75 735f  ted in previous_
+0000cb40: 736f 6c75 7469 6f6e 5f73 6861 7265 640a  solution_shared.
+0000cb50: 2020 2020 762c 6372 7973 7461 6c5f 7065      v,crystal_pe
+0000cb60: 726d 6974 7469 7669 7479 203d 2070 6172  rmittivity = par
+0000cb70: 616d 730a 2020 2020 7661 7520 3d20 7620  ams.    vau = v 
+0000cb80: 2a20 7761 7665 6e75 6d62 6572 0a20 2020  * wavenumber.   
+0000cb90: 2023 2063 6f6e 7665 7274 2074 6865 2073   # convert the s
+0000cba0: 697a 6520 746f 2061 2064 696d 656e 7369  ize to a dimensi
+0000cbb0: 6f6e 6c65 7373 206e 756d 6265 7220 7768  onless number wh
+0000cbc0: 6963 6820 6973 2032 2a70 692a 7369 7a65  ich is 2*pi*size
+0000cbd0: 2f6c 616d 6264 610a 2020 2020 6c61 6d62  /lambda.    lamb
+0000cbe0: 6461 5f6d 7520 3d20 312e 3045 3420 2f20  da_mu = 1.0E4 / 
+0000cbf0: 2876 202b 2031 2e30 652d 3132 290a 2020  (v + 1.0e-12).  
+0000cc00: 2020 6966 2073 697a 655f 6d75 203c 2031    if size_mu < 1
+0000cc10: 2e30 652d 3132 3a0a 2020 2020 2020 2020  .0e-12:.        
+0000cc20: 7369 7a65 5f6d 7520 3d20 312e 3065 2d31  size_mu = 1.0e-1
+0000cc30: 320a 2020 2020 7369 7a65 203d 2032 2e30  2.    size = 2.0
+0000cc40: 2a6e 702e 7069 2a73 697a 655f 6d75 202f  *np.pi*size_mu /
+0000cc50: 206c 616d 6264 615f 6d75 0a20 2020 2064   lambda_mu.    d
+0000cc60: 6174 6120 3d20 2727 0a20 2020 2023 2043  ata = ''.    # C
+0000cc70: 616c 6375 6c61 7465 2074 6865 2065 6666  alculate the eff
+0000cc80: 6563 7420 6f66 2062 7562 626c 6573 2069  ect of bubbles i
+0000cc90: 6e20 7468 6520 6d61 7472 6978 2062 7920  n the matrix by 
+0000cca0: 6173 7375 6d69 6e67 2074 6865 7920 6172  assuming they ar
+0000ccb0: 6520 656d 6265 6464 6564 2069 6e20 616e  e embedded in an
+0000ccc0: 2065 6666 6563 7469 7665 206d 6564 6975   effective mediu
+0000ccd0: 6d20 6465 6669 6e65 6420 6162 6f76 650a  m defined above.
+0000cce0: 2020 2020 7265 6672 6163 7469 7665 5f69      refractive_i
+0000ccf0: 6e64 6578 203d 206d 6174 682e 7371 7274  ndex = math.sqrt
+0000cd00: 286e 702e 7472 6163 6528 6469 656c 6563  (np.trace(dielec
+0000cd10: 7472 6963 5f6d 6564 6975 6d29 2f33 2e30  tric_medium)/3.0
+0000cd20: 290a 2020 2020 6966 2072 6566 7261 6374  ).    if refract
+0000cd30: 6976 655f 696e 6465 782e 696d 6167 203c  ive_index.imag <
+0000cd40: 2030 2e30 3a0a 2020 2020 2020 2020 7265   0.0:.        re
+0000cd50: 6672 6163 7469 7665 5f69 6e64 6578 203d  fractive_index =
+0000cd60: 2072 6566 7261 6374 6976 655f 696e 6465   refractive_inde
+0000cd70: 782e 636f 6e6a 7567 6174 6528 290a 2020  x.conjugate().  
+0000cd80: 2020 6966 2062 7562 626c 655f 7666 203e    if bubble_vf >
+0000cd90: 2030 3a0a 2020 2020 2020 2020 6566 6664   0:.        effd
+0000cda0: 6965 6c65 632c 7265 6672 6163 7469 7665  ielec,refractive
+0000cdb0: 5f69 6e64 6578 203d 2063 616c 6375 6c61  _index = calcula
+0000cdc0: 7465 5f62 7562 626c 655f 7265 6672 6163  te_bubble_refrac
+0000cdd0: 7469 7665 5f69 6e64 6578 2876 2c20 7265  tive_index(v, re
+0000cde0: 6672 6163 7469 7665 5f69 6e64 6578 2c20  fractive_index, 
+0000cdf0: 6275 6262 6c65 5f76 662c 2062 7562 626c  bubble_vf, bubbl
+0000ce00: 655f 7261 6469 7573 290a 2020 2020 2020  e_radius).      
+0000ce10: 2020 6469 656c 6563 7472 6963 5f6d 6564    dielectric_med
+0000ce20: 6975 6d20 3d20 6566 6664 6965 6c65 630a  ium = effdielec.
+0000ce30: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
+0000ce40: 2022 6261 6c61 6e22 3a0a 2020 2020 2020   "balan":.      
+0000ce50: 2020 6566 6664 6965 6c65 6320 3d20 6261    effdielec = ba
+0000ce60: 6c61 6e28 6469 656c 6563 7472 6963 5f6d  lan(dielectric_m
+0000ce70: 6564 6975 6d2c 2063 7279 7374 616c 5f70  edium, crystal_p
+0000ce80: 6572 6d69 7474 6976 6974 792c 2073 6861  ermittivity, sha
+0000ce90: 7065 2c20 4c2c 2076 662c 2073 697a 6529  pe, L, vf, size)
+0000cea0: 0a20 2020 2065 6c69 6620 6d65 7468 6f64  .    elif method
+0000ceb0: 203d 3d20 2261 7022 206f 7220 6d65 7468   == "ap" or meth
+0000cec0: 6f64 203d 3d20 2261 7665 7261 6765 6470  od == "averagedp
+0000ced0: 6572 6d69 7474 6976 6974 7922 206f 7220  ermittivity" or 
+0000cee0: 6d65 7468 6f64 203d 3d20 2261 7665 7261  method == "avera
+0000cef0: 6765 6420 7065 726d 6974 7469 7669 7479  ged permittivity
+0000cf00: 2220 6f72 206d 6574 686f 6420 3d3d 2022  " or method == "
+0000cf10: 6176 6572 6167 6520 7065 726d 6974 7469  average permitti
+0000cf20: 7669 7479 223a 0a20 2020 2020 2020 2020  vity":.         
+0000cf30: 2020 2065 6666 6469 656c 6563 203d 2061     effdielec = a
+0000cf40: 7665 7261 6765 645f 7065 726d 6974 7469  veraged_permitti
+0000cf50: 7669 7479 2864 6965 6c65 6374 7269 635f  vity(dielectric_
+0000cf60: 6d65 6469 756d 2c20 6372 7973 7461 6c5f  medium, crystal_
+0000cf70: 7065 726d 6974 7469 7669 7479 2c20 7368  permittivity, sh
+0000cf80: 6170 652c 204c 2c20 7666 2c20 7369 7a65  ape, L, vf, size
+0000cf90: 290a 2020 2020 656c 6966 206d 6574 686f  ).    elif metho
+0000cfa0: 6420 3d3d 2022 6d61 7877 656c 6c22 206f  d == "maxwell" o
+0000cfb0: 7220 6d65 7468 6f64 203d 3d20 226d 6178  r method == "max
+0000cfc0: 7765 6c6c 2d67 6172 6e65 7474 223a 0a20  well-garnett":. 
+0000cfd0: 2020 2020 2020 2065 6666 6469 656c 6563         effdielec
+0000cfe0: 203d 206d 6178 7765 6c6c 2864 6965 6c65   = maxwell(diele
+0000cff0: 6374 7269 635f 6d65 6469 756d 2c20 6372  ctric_medium, cr
+0000d000: 7973 7461 6c5f 7065 726d 6974 7469 7669  ystal_permittivi
+0000d010: 7479 2c20 7368 6170 652c 204c 2c20 7666  ty, shape, L, vf
+0000d020: 2c20 7369 7a65 290a 2020 2020 656c 6966  , size).    elif
+0000d030: 206d 6574 686f 6420 3d3d 2022 6d61 7877   method == "maxw
+0000d040: 656c 6c5f 7369 6876 6f6c 6122 3a0a 2020  ell_sihvola":.  
+0000d050: 2020 2020 2020 6566 6664 6965 6c65 6320        effdielec 
+0000d060: 3d20 6d61 7877 656c 6c5f 7369 6876 6f6c  = maxwell_sihvol
+0000d070: 6128 6469 656c 6563 7472 6963 5f6d 6564  a(dielectric_med
+0000d080: 6975 6d2c 2063 7279 7374 616c 5f70 6572  ium, crystal_per
+0000d090: 6d69 7474 6976 6974 792c 2073 6861 7065  mittivity, shape
+0000d0a0: 2c20 4c2c 2076 662c 2073 697a 6529 0a20  , L, vf, size). 
+0000d0b0: 2020 2065 6c69 6620 6d65 7468 6f64 203d     elif method =
+0000d0c0: 3d20 2263 6f68 6572 656e 7422 3a0a 2020  = "coherent":.  
+0000d0d0: 2020 2020 2020 6566 6620 203d 2070 7265        eff  = pre
+0000d0e0: 7669 6f75 735f 736f 6c75 7469 6f6e 5f73  vious_solution_s
+0000d0f0: 6861 7265 640a 2020 2020 2020 2020 6966  hared.        if
+0000d100: 206e 702e 6162 7328 6e70 2e74 7261 6365   np.abs(np.trace
+0000d110: 2865 6666 2929 203c 2031 2e30 652d 383a  (eff)) < 1.0e-8:
+0000d120: 0a20 2020 2020 2020 2020 2020 2065 6666  .            eff
+0000d130: 203d 206d 6178 7765 6c6c 2864 6965 6c65   = maxwell(diele
+0000d140: 6374 7269 635f 6d65 6469 756d 2c20 6372  ctric_medium, cr
+0000d150: 7973 7461 6c5f 7065 726d 6974 7469 7669  ystal_permittivi
+0000d160: 7479 2c20 7368 6170 652c 204c 2c20 7666  ty, shape, L, vf
+0000d170: 2c20 7369 7a65 290a 2020 2020 2020 2020  , size).        
+0000d180: 6566 6664 6965 6c65 6320 3d20 636f 6865  effdielec = cohe
+0000d190: 7265 6e74 2864 6965 6c65 6374 7269 635f  rent(dielectric_
+0000d1a0: 6d65 6469 756d 2c20 6372 7973 7461 6c5f  medium, crystal_
+0000d1b0: 7065 726d 6974 7469 7669 7479 2c20 7368  permittivity, sh
+0000d1c0: 6170 652c 204c 2c20 7666 2c20 7369 7a65  ape, L, vf, size
+0000d1d0: 2c20 6566 6629 0a20 2020 2020 2020 2070  , eff).        p
+0000d1e0: 7265 7669 6f75 735f 736f 6c75 7469 6f6e  revious_solution
+0000d1f0: 5f73 6861 7265 6420 3d20 6566 6664 6965  _shared = effdie
+0000d200: 6c65 630a 2020 2020 656c 6966 206d 6574  lec.    elif met
+0000d210: 686f 6420 3d3d 2022 6272 7567 6765 6d61  hod == "bruggema
+0000d220: 6e5f 6d69 6e69 6d69 7365 223a 0a20 2020  n_minimise":.   
+0000d230: 2020 2020 2065 6666 2020 3d20 7072 6576       eff  = prev
+0000d240: 696f 7573 5f73 6f6c 7574 696f 6e5f 7368  ious_solution_sh
+0000d250: 6172 6564 0a20 2020 2020 2020 2069 6620  ared.        if 
+0000d260: 6e70 2e61 6273 286e 702e 7472 6163 6528  np.abs(np.trace(
+0000d270: 6566 6629 2920 3c20 312e 3065 2d38 3a0a  eff)) < 1.0e-8:.
+0000d280: 2020 2020 2020 2020 2020 2020 6566 6620              eff 
+0000d290: 3d20 6d61 7877 656c 6c28 6469 656c 6563  = maxwell(dielec
+0000d2a0: 7472 6963 5f6d 6564 6975 6d2c 2063 7279  tric_medium, cry
+0000d2b0: 7374 616c 5f70 6572 6d69 7474 6976 6974  stal_permittivit
+0000d2c0: 792c 2073 6861 7065 2c20 4c2c 2076 662c  y, shape, L, vf,
+0000d2d0: 2073 697a 6529 0a20 2020 2020 2020 2065   size).        e
+0000d2e0: 6666 6469 656c 6563 203d 2062 7275 6767  ffdielec = brugg
+0000d2f0: 656d 616e 5f6d 696e 696d 6973 6528 6469  eman_minimise(di
+0000d300: 656c 6563 7472 6963 5f6d 6564 6975 6d2c  electric_medium,
+0000d310: 2063 7279 7374 616c 5f70 6572 6d69 7474   crystal_permitt
+0000d320: 6976 6974 792c 2073 6861 7065 2c20 4c2c  ivity, shape, L,
+0000d330: 2076 662c 2073 697a 652c 2065 6666 290a   vf, size, eff).
+0000d340: 2020 2020 2020 2020 7072 6576 696f 7573          previous
+0000d350: 5f73 6f6c 7574 696f 6e5f 7368 6172 6564  _solution_shared
+0000d360: 203d 2065 6666 6469 656c 6563 0a20 2020   = effdielec.   
+0000d370: 2065 6c69 6620 6d65 7468 6f64 203d 3d20   elif method == 
+0000d380: 2262 7275 6767 656d 616e 2220 6f72 206d  "bruggeman" or m
+0000d390: 6574 686f 6420 3d3d 2022 6272 7567 6765  ethod == "brugge
+0000d3a0: 6d61 6e5f 6974 6572 223a 0a20 2020 2020  man_iter":.     
+0000d3b0: 2020 2065 6666 2020 3d20 7072 6576 696f     eff  = previo
+0000d3c0: 7573 5f73 6f6c 7574 696f 6e5f 7368 6172  us_solution_shar
+0000d3d0: 6564 0a20 2020 2020 2020 2069 6620 6e70  ed.        if np
+0000d3e0: 2e61 6273 286e 702e 7472 6163 6528 6566  .abs(np.trace(ef
+0000d3f0: 6629 2920 3c20 312e 3065 2d38 3a0a 2020  f)) < 1.0e-8:.  
+0000d400: 2020 2020 2020 2020 2020 6566 6620 3d20            eff = 
+0000d410: 6d61 7877 656c 6c28 6469 656c 6563 7472  maxwell(dielectr
+0000d420: 6963 5f6d 6564 6975 6d2c 2063 7279 7374  ic_medium, cryst
+0000d430: 616c 5f70 6572 6d69 7474 6976 6974 792c  al_permittivity,
+0000d440: 2073 6861 7065 2c20 4c2c 2076 662c 2073   shape, L, vf, s
+0000d450: 697a 6529 0a20 2020 2020 2020 2065 6666  ize).        eff
+0000d460: 6469 656c 6563 203d 2062 7275 6767 656d  dielec = bruggem
+0000d470: 616e 5f69 7465 7228 6469 656c 6563 7472  an_iter(dielectr
+0000d480: 6963 5f6d 6564 6975 6d2c 2063 7279 7374  ic_medium, cryst
+0000d490: 616c 5f70 6572 6d69 7474 6976 6974 792c  al_permittivity,
+0000d4a0: 2073 6861 7065 2c20 4c2c 2076 662c 2073   shape, L, vf, s
+0000d4b0: 697a 652c 2065 6666 290a 2020 2020 2020  ize, eff).      
+0000d4c0: 2020 7072 6576 696f 7573 5f73 6f6c 7574    previous_solut
+0000d4d0: 696f 6e5f 7368 6172 6564 203d 2065 6666  ion_shared = eff
+0000d4e0: 6469 656c 6563 0a20 2020 2065 6c69 6620  dielec.    elif 
+0000d4f0: 6d65 7468 6f64 203d 3d20 2261 6e69 736f  method == "aniso
+0000d500: 7472 6f70 6963 2d6d 6965 223a 0a20 2020  tropic-mie":.   
+0000d510: 2020 2020 2065 6666 6469 656c 6563 203d       effdielec =
+0000d520: 2061 6e69 736f 7472 6f70 6963 5f6d 6965   anisotropic_mie
+0000d530: 5f73 6361 7474 6572 696e 6728 6469 656c  _scattering(diel
+0000d540: 6563 7472 6963 5f6d 6564 6975 6d2c 2063  ectric_medium, c
+0000d550: 7279 7374 616c 5f70 6572 6d69 7474 6976  rystal_permittiv
+0000d560: 6974 792c 2073 6861 7065 2c20 4c2c 2076  ity, shape, L, v
+0000d570: 662c 2073 697a 652c 2073 697a 655f 6d75  f, size, size_mu
+0000d580: 2c20 7369 7a65 5f64 6973 7472 6962 7574  , size_distribut
+0000d590: 696f 6e5f 7369 676d 6129 0a20 2020 2065  ion_sigma).    e
+0000d5a0: 6c69 6620 6d65 7468 6f64 203d 3d20 226d  lif method == "m
+0000d5b0: 6965 223a 0a20 2020 2020 2020 2065 6666  ie":.        eff
+0000d5c0: 6469 656c 6563 203d 206d 6965 5f73 6361  dielec = mie_sca
+0000d5d0: 7474 6572 696e 6728 6469 656c 6563 7472  ttering(dielectr
+0000d5e0: 6963 5f6d 6564 6975 6d2c 2063 7279 7374  ic_medium, cryst
+0000d5f0: 616c 5f70 6572 6d69 7474 6976 6974 792c  al_permittivity,
+0000d600: 2073 6861 7065 2c20 4c2c 2076 662c 2073   shape, L, vf, s
+0000d610: 697a 652c 2073 697a 655f 6d75 2c20 7369  ize, size_mu, si
+0000d620: 7a65 5f64 6973 7472 6962 7574 696f 6e5f  ze_distribution_
+0000d630: 7369 676d 6129 0a20 2020 2065 6c73 653a  sigma).    else:
+0000d640: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+0000d650: 556e 6b6f 776e 2064 6965 6c65 6374 7269  Unkown dielectri
+0000d660: 6320 6d65 7468 6f64 3a20 7b7d 272e 666f  c method: {}'.fo
+0000d670: 726d 6174 286d 6574 686f 6429 290a 2020  rmat(method)).  
+0000d680: 2020 2020 2020 6578 6974 2831 290a 2020        exit(1).  
+0000d690: 2020 2320 4176 6572 6167 6520 6f76 6572    # Average over
+0000d6a0: 2061 6c6c 2064 6972 6563 7469 6f6e 7320   all directions 
+0000d6b0: 6279 2074 616b 696e 6720 7468 6520 7472  by taking the tr
+0000d6c0: 6163 650a 2020 2020 7472 6163 6520 3d20  ace.    trace = 
+0000d6d0: 2865 6666 6469 656c 6563 5b30 2c20 305d  (effdielec[0, 0]
+0000d6e0: 202b 2065 6666 6469 656c 6563 5b31 2c20   + effdielec[1, 
+0000d6f0: 315d 202b 2065 6666 6469 656c 6563 5b32  1] + effdielec[2
+0000d700: 2c20 325d 2920 2f20 332e 300a 2020 2020  , 2]) / 3.0.    
+0000d710: 7265 6672 6163 7469 7665 5f69 6e64 6578  refractive_index
+0000d720: 203d 2063 616c 6375 6c61 7465 5f72 6566   = calculate_ref
+0000d730: 7261 6374 6976 655f 696e 6465 7828 6566  ractive_index(ef
+0000d740: 6664 6965 6c65 6329 0a20 2020 2023 0a20  fdielec).    #. 
+0000d750: 2020 2023 2061 6273 6f72 7074 696f 6e20     # absorption 
+0000d760: 636f 6566 6669 6369 656e 7420 6973 2063  coefficient is c
+0000d770: 616c 6375 6c61 7465 6420 6672 6f6d 2074  alculated from t
+0000d780: 6865 2069 6d61 6769 6e61 7279 2072 6566  he imaginary ref
+0000d790: 7261 6374 6976 6520 696e 6465 780a 2020  ractive index.  
+0000d7a0: 2020 2320 7365 6520 482e 432e 2076 616e    # see H.C. van
+0000d7b0: 2064 6520 4875 6c73 7420 4c69 6768 7420   de Hulst Light 
+0000d7c0: 5363 6174 7465 7269 6e67 2062 7920 536d  Scattering by Sm
+0000d7d0: 616c 6c20 5061 7274 6963 6c65 7320 2c20  all Particles , 
+0000d7e0: 7061 6765 2032 3637 0a20 2020 2023 2054  page 267.    # T
+0000d7f0: 6869 7320 6973 2064 6966 6665 7265 6e74  his is different
+0000d800: 2062 7574 2072 656c 6174 6564 2074 6f20   but related to 
+0000d810: 4765 6e7a 656c 2061 6e64 204d 6172 7469  Genzel and Marti
+0000d820: 6e20 4571 7561 7469 6f6e 2031 362c 2050  n Equation 16, P
+0000d830: 6879 732e 2053 7461 742e 2053 6f6c 2e20  hys. Stat. Sol. 
+0000d840: 3531 2831 3937 3229 2039 312d 0a20 2020  51(1972) 91-.   
+0000d850: 2023 2049 2776 6520 6164 6420 6120 6661   # I've add a fa
+0000d860: 6374 6f72 206f 6620 6c6f 6731 3028 6529  ctor of log10(e)
+0000d870: 2062 6563 6175 7365 2077 6520 6e65 6564   because we need
+0000d880: 2074 6f20 6173 7375 6d65 2061 2064 6563   to assume a dec
+0000d890: 6164 6963 2042 6565 7227 7320 6c61 770a  adic Beer's law.
+0000d8a0: 2020 2020 2320 756e 6974 7320 6172 6520      # units are 
+0000d8b0: 636d 2d31 0a20 2020 2061 6273 6f72 7074  cm-1.    absorpt
+0000d8c0: 696f 6e5f 636f 6566 6669 6369 656e 7420  ion_coefficient 
+0000d8d0: 3d20 7620 2a20 342a 5049 202a 206e 702e  = v * 4*PI * np.
+0000d8e0: 696d 6167 2872 6566 7261 6374 6976 655f  imag(refractive_
+0000d8f0: 696e 6465 7829 202a 206d 6174 682e 6c6f  index) * math.lo
+0000d900: 6731 3028 6d61 7468 2e65 290a 2020 2020  g10(math.e).    
+0000d910: 2320 756e 6974 7320 6172 6520 636d 2d31  # units are cm-1
+0000d920: 204c 206d 6f6c 6573 2d31 0a20 2020 206d   L moles-1.    m
+0000d930: 6f6c 6172 5f61 6273 6f72 7074 696f 6e5f  olar_absorption_
+0000d940: 636f 6566 6669 6369 656e 7420 3d20 6162  coefficient = ab
+0000d950: 736f 7270 7469 6f6e 5f63 6f65 6666 6963  sorption_coeffic
+0000d960: 6965 6e74 202f 2063 6f6e 6365 6e74 7261  ient / concentra
+0000d970: 7469 6f6e 202f 2076 660a 2020 2020 2320  tion / vf.    # 
+0000d980: 6361 6c63 756c 6174 6520 7468 6520 4154  calculate the AT
+0000d990: 5220 7265 666c 6563 7461 6e63 650a 2020  R reflectance.  
+0000d9a0: 2020 7370 6174 7220 3d20 7265 666c 6563    spatr = reflec
+0000d9b0: 7461 6e63 655f 6174 7228 7265 6672 6163  tance_atr(refrac
+0000d9c0: 7469 7665 5f69 6e64 6578 2c61 7472 5065  tive_index,atrPe
+0000d9d0: 726d 6974 7469 7669 7479 2c61 7472 5468  rmittivity,atrTh
+0000d9e0: 6574 612c 6174 7253 506f 6c29 0a20 2020  eta,atrSPol).   
+0000d9f0: 2072 6574 7572 6e20 762c 6d65 7468 6f64   return v,method
+0000da00: 2c73 697a 655f 6d75 2c73 697a 655f 6469  ,size_mu,size_di
+0000da10: 7374 7269 6275 7469 6f6e 5f73 6967 6d61  stribution_sigma
+0000da20: 2c73 6861 7065 2c64 6174 612c 7472 6163  ,shape,data,trac
+0000da30: 652c 6162 736f 7270 7469 6f6e 5f63 6f65  e,absorption_coe
+0000da40: 6666 6963 6965 6e74 2c6d 6f6c 6172 5f61  fficient,molar_a
+0000da50: 6273 6f72 7074 696f 6e5f 636f 6566 6669  bsorption_coeffi
+0000da60: 6369 656e 742c 7370 6174 720a 0a64 6566  cient,spatr..def
+0000da70: 2063 616c 6375 6c61 7465 5f62 7562 626c   calculate_bubbl
+0000da80: 655f 7265 6672 6163 7469 7665 5f69 6e64  e_refractive_ind
+0000da90: 6578 2876 5f63 6d31 2c20 7269 5f6d 6564  ex(v_cm1, ri_med
+0000daa0: 6975 6d2c 2076 662c 2072 6164 6975 735f  ium, vf, radius_
+0000dab0: 6d75 293a 0a20 2020 2022 2222 4361 6c63  mu):.    """Calc
+0000dac0: 756c 6174 6520 7468 6520 7363 6174 7465  ulate the scatte
+0000dad0: 7269 6e67 2066 726f 6d20 6275 6262 6c65  ring from bubble
+0000dae0: 7320 656d 6265 6464 6564 2069 6e20 6120  s embedded in a 
+0000daf0: 706f 7373 6962 6c79 2c20 636f 6d70 6c65  possibly, comple
+0000db00: 7820 6469 656c 6563 7472 6963 2061 7420  x dielectric at 
+0000db10: 765f 636d 310a 2020 2020 2020 2076 5f63  v_cm1.       v_c
+0000db20: 6d31 2069 7320 7468 6520 6672 6571 7565  m1 is the freque
+0000db30: 6e63 7920 696e 2063 6d2d 310a 2020 2020  ncy in cm-1.    
+0000db40: 2020 2072 695f 6d65 6469 756d 2069 7320     ri_medium is 
+0000db50: 7468 6520 7265 6672 6163 7469 7665 2069  the refractive i
+0000db60: 6e64 6578 206f 6620 7468 6520 6d65 6469  ndex of the medi
+0000db70: 756d 0a20 2020 2020 2020 7666 2069 7320  um.       vf is 
+0000db80: 7468 6520 766f 6c75 6d65 2066 7261 6374  the volume fract
+0000db90: 696f 6e20 6f66 2062 7562 626c 6573 0a20  ion of bubbles. 
+0000dba0: 2020 2020 2020 7261 6469 7573 5f6d 7520        radius_mu 
+0000dbb0: 6973 2074 6865 2072 6164 6975 7320 6f66  is the radius of
+0000dbc0: 2074 6865 2062 7562 626c 6573 2069 6e20   the bubbles in 
+0000dbd0: 6d69 6372 6f6e 730a 2020 2020 2020 2054  microns.       T
+0000dbe0: 6865 2072 6f75 7469 6e65 2072 6574 7572  he routine retur
+0000dbf0: 6e73 2074 6865 2065 6666 6563 7469 7665  ns the effective
+0000dc00: 2064 6965 6c65 6374 7269 6320 636f 6e73   dielectric cons
+0000dc10: 7461 6e74 2061 6e64 2074 6865 2061 7373  tant and the ass
+0000dc20: 6f63 6961 7465 6420 7265 6672 6163 7469  ociated refracti
+0000dc30: 7665 2069 6e64 6578 2222 220a 2020 2020  ve index""".    
+0000dc40: 230a 2020 2020 2320 5765 206e 6565 6420  #.    # We need 
+0000dc50: 746f 2074 616b 656e 2061 6363 6f75 6e74  to taken account
+0000dc60: 206f 6620 7468 6520 6368 616e 6765 2069   of the change i
+0000dc70: 6e20 7761 7665 6c65 6e67 7468 2061 6e64  n wavelength and
+0000dc80: 2074 6865 2063 6861 6e67 6520 696e 2073   the change in s
+0000dc90: 697a 6520 7061 7261 6d65 7465 7220 6475  ize parameter du
+0000dca0: 6520 746f 2074 6865 0a20 2020 2023 204e  e to the.    # N
+0000dcb0: 6f6e 6520 756e 6974 2076 616c 7565 206f  one unit value o
+0000dcc0: 6620 7468 6520 6469 656c 6563 7472 6963  f the dielectric
+0000dcd0: 206f 6620 7468 6520 656d 6265 6464 696e   of the embeddin
+0000dce0: 6720 6d65 6469 756d 0a20 2020 2023 2054  g medium.    # T
+0000dcf0: 6865 2073 697a 6520 7061 7261 6d65 7465  he size paramete
+0000dd00: 7220 6973 2032 7069 2072 202f 206c 616d  r is 2pi r / lam
+0000dd10: 6264 610a 2020 2020 2320 5468 6520 6566  bda.    # The ef
+0000dd20: 6665 6374 6976 6520 6c61 6d62 6461 2069  fective lambda i
+0000dd30: 6e20 7468 6520 7375 7070 6f72 7469 6e67  n the supporting
+0000dd40: 206d 6564 6975 6d20 6973 206c 616d 6264   medium is lambd
+0000dd50: 6120 2f20 7371 7274 2865 6d65 6469 756d  a / sqrt(emedium
+0000dd60: 290a 2020 2020 2320 5768 6572 6520 7468  ).    # Where th
+0000dd70: 6520 7265 6672 6163 7469 7665 2069 6e64  e refractive ind
+0000dd80: 6578 2069 7320 7461 6b65 6e20 746f 2062  ex is taken to b
+0000dd90: 6520 7371 7274 2865 6d65 6469 756d 2920  e sqrt(emedium) 
+0000dda0: 286e 6f6e 206d 6167 6e65 7469 6320 6d61  (non magnetic ma
+0000ddb0: 7465 7269 616c 7329 0a20 2020 2023 0a20  terials).    #. 
+0000ddc0: 2020 2069 6620 765f 636d 3120 3e20 303a     if v_cm1 > 0:
+0000ddd0: 0a20 2020 2020 2020 206c 616d 6264 615f  .        lambda_
+0000dde0: 7661 6375 756d 5f6e 6d20 3d20 312e 3045  vacuum_nm = 1.0E
+0000ddf0: 332a 312e 3045 3420 2f20 765f 636d 310a  3*1.0E4 / v_cm1.
+0000de00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000de10: 2020 6c61 6d62 6461 5f76 6163 7575 6d5f    lambda_vacuum_
+0000de20: 6e6d 203d 2031 2e30 4539 390a 2020 2020  nm = 1.0E99.    
+0000de30: 2320 5472 6561 7420 7468 6520 6275 6262  # Treat the bubb
+0000de40: 6c65 2061 7320 7468 6f75 6768 2069 7420  le as though it 
+0000de50: 6973 2061 6972 2069 6e20 6d61 7472 6978  is air in matrix
+0000de60: 0a20 2020 2023 2054 6865 2065 6666 6563  .    # The effec
+0000de70: 7469 7665 2077 6176 6520 6e75 6d62 6572  tive wave number
+0000de80: 206b 203d 2073 7172 7428 656d 6564 6975   k = sqrt(emediu
+0000de90: 6d29 2a32 7069 2a76 2f63 2028 636f 6d70  m)*2pi*v/c (comp
+0000dea0: 6c65 7821 290a 2020 2020 7261 6469 7573  lex!).    radius
+0000deb0: 5f6e 6d20 3d20 7261 6469 7573 5f6d 7520  _nm = radius_mu 
+0000dec0: 2a20 3130 3030 0a20 2020 2023 2076 6f6c  * 1000.    # vol
+0000ded0: 756d 6520 6f66 2061 2062 7562 626c 6520  ume of a bubble 
+0000dee0: 696e 206e 6d5e 330a 2020 2020 565f 6e6d  in nm^3.    V_nm
+0000def0: 203d 2034 2e30 2f33 2e30 202a 2050 4920   = 4.0/3.0 * PI 
+0000df00: 2a20 7261 6469 7573 5f6e 6d20 2a20 7261  * radius_nm * ra
+0000df10: 6469 7573 5f6e 6d20 2a20 7261 6469 7573  dius_nm * radius
+0000df20: 5f6e 6d0a 2020 2020 2320 4e75 6d62 6572  _nm.    # Number
+0000df30: 2064 656e 7369 7479 206f 6620 6275 6262   density of bubb
+0000df40: 6c65 7320 286e 756d 6265 7220 2f20 6e6d  les (number / nm
+0000df50: 5e33 290a 2020 2020 4e5f 6e6d 203d 2076  ^3).    N_nm = v
+0000df60: 6620 2f20 565f 6e6d 0a20 2020 206b 5f6e  f / V_nm.    k_n
+0000df70: 6d20 3d20 7761 7465 726d 616e 5f74 7275  m = waterman_tru
+0000df80: 656c 6c5f 7363 6174 7465 7269 6e67 286c  ell_scattering(l
+0000df90: 616d 6264 615f 7661 6375 756d 5f6e 6d2c  ambda_vacuum_nm,
+0000dfa0: 204e 5f6e 6d2c 2072 6164 6975 735f 6e6d   N_nm, radius_nm
+0000dfb0: 2c20 7269 5f6d 6564 6975 6d29 0a20 2020  , ri_medium).   
+0000dfc0: 2023 206b 5f6e 6d20 3d20 666f 6c64 795f   # k_nm = foldy_
+0000dfd0: 7363 6174 7465 7269 6e67 286c 616d 6264  scattering(lambd
+0000dfe0: 615f 7661 6375 756d 5f6e 6d2c 204e 5f6e  a_vacuum_nm, N_n
+0000dff0: 6d2c 2072 6164 6975 735f 6e6d 2c20 7269  m, radius_nm, ri
+0000e000: 5f6d 6564 6975 6d29 0a20 2020 2072 695f  _medium).    ri_
+0000e010: 6d65 6469 756d 203d 206b 5f6e 6d20 2a6c  medium = k_nm *l
+0000e020: 616d 6264 615f 7661 6375 756d 5f6e 6d20  ambda_vacuum_nm 
+0000e030: 2f20 2832 2a50 4929 0a20 2020 2065 6666  / (2*PI).    eff
+0000e040: 5f6d 6564 6975 6d20 3d20 7269 5f6d 6564  _medium = ri_med
+0000e050: 6975 6d20 2a20 7269 5f6d 6564 6975 6d0a  ium * ri_medium.
+0000e060: 2020 2020 6566 6664 6965 6c65 6320 3d20      effdielec = 
+0000e070: 6e70 2e61 7272 6179 285b 5b65 6666 5f6d  np.array([[eff_m
+0000e080: 6564 6975 6d2c 2030 2c20 305d 2c20 5b30  edium, 0, 0], [0
+0000e090: 2c20 6566 665f 6d65 6469 756d 2c20 305d  , eff_medium, 0]
+0000e0a0: 2c20 5b30 2c20 302c 2065 6666 5f6d 6564  , [0, 0, eff_med
+0000e0b0: 6975 6d5d 5d29 0a20 2020 2072 6574 7572  ium]]).    retur
+0000e0c0: 6e20 6566 6664 6965 6c65 632c 7269 5f6d  n effdielec,ri_m
+0000e0d0: 6564 6975 6d0a 0a64 6566 2066 6f6c 6479  edium..def foldy
+0000e0e0: 5f73 6361 7474 6572 696e 6728 6c61 6d62  _scattering(lamb
+0000e0f0: 6461 5f76 6163 7575 6d5f 6e6d 2c20 4e5f  da_vacuum_nm, N_
+0000e100: 6e6d 2c72 6164 6975 735f 6e6d 2c72 695f  nm,radius_nm,ri_
+0000e110: 6d65 6469 756d 293a 0a20 2020 2023 0a20  medium):.    #. 
+0000e120: 2020 2023 2053 6f6c 7665 2074 6865 2066     # Solve the f
+0000e130: 6f6c 6479 2065 7175 6174 696f 6e20 666f  oldy equation fo
+0000e140: 7220 7363 6174 7465 7269 6e67 206f 6620  r scattering of 
+0000e150: 616e 2061 6972 2062 7562 626c 6520 656d  an air bubble em
+0000e160: 6265 6464 6564 2069 6e20 6120 6c6f 7373  bedded in a loss
+0000e170: 7920 6d65 6469 756d 0a20 2020 2023 204e  y medium.    # N
+0000e180: 5f6e 6d20 6973 2074 6865 206e 756d 6265  _nm is the numbe
+0000e190: 7220 6465 6e73 6974 7920 6f66 2062 7562  r density of bub
+0000e1a0: 626c 6573 2069 6e20 7468 6520 766f 6c75  bles in the volu
+0000e1b0: 6d65 206e 6d5e 330a 2020 2020 2320 6b5f  me nm^3.    # k_
+0000e1c0: 6e6d 2069 7320 7468 6520 7761 7665 6e75  nm is the wavenu
+0000e1d0: 6d62 6572 206f 6620 7468 6520 696e 636f  mber of the inco
+0000e1e0: 6d69 6e67 2077 6176 6520 2863 6f6d 706c  ming wave (compl
+0000e1f0: 6578 290a 2020 2020 2320 7261 6469 7573  ex).    # radius
+0000e200: 5f6e 6d20 6973 2074 6865 2072 6164 6975  _nm is the radiu
+0000e210: 7320 6f66 2074 6865 2062 7562 626c 650a  s of the bubble.
+0000e220: 2020 2020 2320 7269 5f6d 6564 6975 6d20      # ri_medium 
+0000e230: 6973 2074 6865 2072 6566 7261 6374 6976  is the refractiv
+0000e240: 6520 696e 6465 7820 6f66 2074 6865 206d  e index of the m
+0000e250: 6564 6975 6d20 7468 6520 6275 6262 6c65  edium the bubble
+0000e260: 2069 7320 696e 0a20 2020 2023 0a20 2020   is in.    #.   
+0000e270: 2023 0a20 2020 206b 5f6e 6d20 3d20 322a   #.    k_nm = 2*
+0000e280: 5049 2a72 695f 6d65 6469 756d 2f6c 616d  PI*ri_medium/lam
+0000e290: 6264 615f 7661 6375 756d 5f6e 6d0a 2020  bda_vacuum_nm.  
+0000e2a0: 2020 2320 5468 6520 7369 7a65 2070 6172    # The size par
+0000e2b0: 616d 6574 6572 2069 7320 6e6f 7720 616c  ameter is now al
+0000e2c0: 736f 2063 6f6d 706c 6578 2061 6e64 2064  so complex and d
+0000e2d0: 696d 656e 7369 6f6e 6c65 7373 0a20 2020  imensionless.   
+0000e2e0: 2073 697a 6520 3d20 6b5f 6e6d 2a72 6164   size = k_nm*rad
+0000e2f0: 6975 735f 6e6d 0a20 2020 2072 6566 7261  ius_nm.    refra
+0000e300: 6374 6976 655f 696e 6465 7820 3d20 312e  ctive_index = 1.
+0000e310: 3020 2f20 7269 5f6d 6564 6975 6d0a 2020  0 / ri_medium.  
+0000e320: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
+0000e330: 6520 666f 7277 6172 6420 616e 6420 6261  e forward and ba
+0000e340: 636b 7761 7264 2073 6361 7474 6572 696e  ckward scatterin
+0000e350: 6720 616d 706c 6974 7564 650a 2020 2020  g amplitude.    
+0000e360: 7331 302c 7332 3020 3d20 4d69 652e 4d69  s10,s20 = Mie.Mi
+0000e370: 6553 3153 3228 7265 6672 6163 7469 7665  eS1S2(refractive
+0000e380: 5f69 6e64 6578 2c20 7369 7a65 2a72 695f  _index, size*ri_
+0000e390: 6d65 6469 756d 2c20 3129 0a20 2020 2069  medium, 1).    i
+0000e3a0: 203d 2063 6f6d 706c 6578 2830 2c31 290a   = complex(0,1).
+0000e3b0: 2020 2020 6630 203d 2069 202a 2073 3130      f0 = i * s10
+0000e3c0: 202f 206b 5f6e 6d0a 2020 2020 6e65 775f   / k_nm.    new_
+0000e3d0: 6b20 3d20 6e70 2e73 7172 7428 206b 5f6e  k = np.sqrt( k_n
+0000e3e0: 6d2a 6b5f 6e6d 202b 2034 2a50 492a 4e5f  m*k_nm + 4*PI*N_
+0000e3f0: 6e6d 2a66 3020 290a 2020 2020 6966 206e  nm*f0 ).    if n
+0000e400: 6577 5f6b 2e69 6d61 6720 3c20 302e 303a  ew_k.imag < 0.0:
+0000e410: 0a20 2020 2020 2020 206e 6577 5f6b 203d  .        new_k =
+0000e420: 206e 6577 5f6b 2e63 6f6e 6a75 6761 7465   new_k.conjugate
+0000e430: 2829 0a20 2020 2072 6574 7572 6e20 6e65  ().    return ne
+0000e440: 775f 6b0a 0a64 6566 2077 6174 6572 6d61  w_k..def waterma
+0000e450: 6e5f 7472 7565 6c6c 5f73 6361 7474 6572  n_truell_scatter
+0000e460: 696e 6728 6c61 6d62 6461 5f76 6163 7575  ing(lambda_vacuu
+0000e470: 6d5f 6e6d 2c20 4e5f 6e6d 2c72 6164 6975  m_nm, N_nm,radiu
+0000e480: 735f 6e6d 2c72 695f 6d65 6469 756d 293a  s_nm,ri_medium):
+0000e490: 0a20 2020 2023 0a20 2020 2023 2053 6f6c  .    #.    # Sol
+0000e4a0: 7665 2074 6865 2077 6174 6572 6d61 6e20  ve the waterman 
+0000e4b0: 7472 7565 6c6c 2065 7175 6174 696f 6e20  truell equation 
+0000e4c0: 666f 7220 7363 6174 7465 7269 6e67 206f  for scattering o
+0000e4d0: 6620 616e 2061 6972 2062 7562 626c 6520  f an air bubble 
+0000e4e0: 656d 6265 6464 6564 2069 6e20 6120 6c6f  embedded in a lo
+0000e4f0: 7373 7920 6d65 6469 756d 0a20 2020 2023  ssy medium.    #
+0000e500: 204e 5f6e 6d20 6973 2074 6865 206e 756d   N_nm is the num
+0000e510: 6265 7220 6465 6e73 6974 7920 6f66 2062  ber density of b
+0000e520: 7562 626c 6573 2069 6e20 7468 6520 766f  ubbles in the vo
+0000e530: 6c75 6d65 206e 6d5e 330a 2020 2020 2320  lume nm^3.    # 
+0000e540: 6b5f 6e6d 2069 7320 7468 6520 7761 7665  k_nm is the wave
+0000e550: 6e75 6d62 6572 206f 6620 7468 6520 696e  number of the in
+0000e560: 636f 6d69 6e67 2077 6176 6520 2863 6f6d  coming wave (com
+0000e570: 706c 6578 290a 2020 2020 2320 7261 6469  plex).    # radi
+0000e580: 7573 5f6e 6d20 6973 2074 6865 2072 6164  us_nm is the rad
+0000e590: 6975 7320 6f66 2074 6865 2062 7562 626c  ius of the bubbl
+0000e5a0: 650a 2020 2020 2320 7269 5f6d 6564 6975  e.    # ri_mediu
+0000e5b0: 6d20 6973 2074 6865 2072 6566 7261 6374  m is the refract
+0000e5c0: 6976 6520 696e 6465 7820 6f66 2074 6865  ive index of the
+0000e5d0: 206d 6564 6975 6d20 7468 6520 6275 6262   medium the bubb
+0000e5e0: 6c65 2069 7320 696e 0a20 2020 2023 0a20  le is in.    #. 
+0000e5f0: 2020 2023 0a20 2020 206b 5f6e 6d20 3d20     #.    k_nm = 
+0000e600: 322a 5049 2a72 695f 6d65 6469 756d 2f6c  2*PI*ri_medium/l
+0000e610: 616d 6264 615f 7661 6375 756d 5f6e 6d0a  ambda_vacuum_nm.
+0000e620: 2020 2020 2320 5468 6520 7369 7a65 2070      # The size p
+0000e630: 6172 616d 6574 6572 2069 7320 6e6f 7720  arameter is now 
+0000e640: 616c 736f 2063 6f6d 706c 6578 2061 6e64  also complex and
+0000e650: 2064 696d 656e 7369 6f6e 6c65 7373 0a20   dimensionless. 
+0000e660: 2020 2073 697a 6520 3d20 6b5f 6e6d 2a72     size = k_nm*r
+0000e670: 6164 6975 735f 6e6d 0a20 2020 2072 6566  adius_nm.    ref
+0000e680: 7261 6374 6976 655f 696e 6465 7820 3d20  ractive_index = 
+0000e690: 312e 3020 2f20 7269 5f6d 6564 6975 6d0a  1.0 / ri_medium.
+0000e6a0: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+0000e6b0: 7468 6520 666f 7277 6172 6420 616e 6420  the forward and 
+0000e6c0: 6261 636b 7761 7264 2073 6361 7474 6572  backward scatter
+0000e6d0: 696e 6720 616d 706c 6974 7564 650a 2020  ing amplitude.  
+0000e6e0: 2020 7331 302c 7332 3020 3d20 4d69 652e    s10,s20 = Mie.
+0000e6f0: 4d69 6553 3153 3228 7265 6672 6163 7469  MieS1S2(refracti
+0000e700: 7665 5f69 6e64 6578 2c20 7369 7a65 2a72  ve_index, size*r
+0000e710: 695f 6d65 6469 756d 2c20 3129 0a20 2020  i_medium, 1).   
+0000e720: 2073 3131 2c73 3231 203d 204d 6965 2e4d   s11,s21 = Mie.M
+0000e730: 6965 5331 5332 2872 6566 7261 6374 6976  ieS1S2(refractiv
+0000e740: 655f 696e 6465 782c 2073 697a 652a 7269  e_index, size*ri
+0000e750: 5f6d 6564 6975 6d2c 2d31 290a 2020 2020  _medium,-1).    
+0000e760: 2320 7468 6520 6e6f 726d 616c 6973 6174  # the normalisat
+0000e770: 696f 6e20 6279 2031 2f6b 5f6e 6d20 6973  ion by 1/k_nm is
+0000e780: 2070 6572 666f 726d 6564 2077 6865 6e20   performed when 
+0000e790: 6620 6973 2063 616c 6375 6c61 7465 640a  f is calculated.
+0000e7a0: 2020 2020 6920 3d20 636f 6d70 6c65 7828      i = complex(
+0000e7b0: 302c 3129 0a20 2020 2066 3020 3d20 692a  0,1).    f0 = i*
+0000e7c0: 7331 300a 2020 2020 6631 203d 2069 2a73  s10.    f1 = i*s
+0000e7d0: 3131 0a20 2020 2023 2070 7269 6e74 2827  11.    # print('
+0000e7e0: 5761 7465 726d 616e 5f74 7275 656c 6c27  Waterman_truell'
+0000e7f0: 2c61 6273 2866 302b 6631 2929 0a20 2020  ,abs(f0+f1)).   
+0000e800: 206b 3220 3d20 6b5f 6e6d 2a6b 5f6e 6d0a   k2 = k_nm*k_nm.
+0000e810: 2020 2020 6620 3d20 322a 5049 2a4e 5f6e      f = 2*PI*N_n
+0000e820: 6d2f 286b 5f6e 6d2a 6b5f 6e6d 2a6b 5f6e  m/(k_nm*k_nm*k_n
+0000e830: 6d29 0a20 2020 206e 6577 5f6b 203d 206e  m).    new_k = n
+0000e840: 702e 7371 7274 2820 6b32 202a 2028 2028  p.sqrt( k2 * ( (
+0000e850: 312b 662a 6630 292a 2831 2b66 2a66 3029  1+f*f0)*(1+f*f0)
+0000e860: 202d 2066 2a66 312a 662a 6631 2029 2029   - f*f1*f*f1 ) )
+0000e870: 0a20 2020 2069 6620 6e65 775f 6b2e 696d  .    if new_k.im
+0000e880: 6167 203c 2030 2e30 3a0a 2020 2020 2020  ag < 0.0:.      
+0000e890: 2020 6e65 775f 6b20 3d20 6e65 775f 6b2e    new_k = new_k.
+0000e8a0: 636f 6e6a 7567 6174 6528 290a 2020 2020  conjugate().    
+0000e8b0: 7265 7475 726e 206e 6577 5f6b 0a0a 6465  return new_k..de
+0000e8c0: 6620 6361 6c63 756c 6174 655f 6365 6e74  f calculate_cent
+0000e8d0: 7265 5f6f 665f 6d61 7373 2878 797a 732c  re_of_mass(xyzs,
+0000e8e0: 206d 6173 7365 7329 3a0a 2020 2027 2727   masses):.   '''
+0000e8f0: 4361 6c63 756c 6174 6520 6365 6e74 7265  Calculate centre
+0000e900: 206f 6620 6d61 7373 2727 270a 2020 2063   of mass'''.   c
+0000e910: 6d20 3d20 6e70 2e7a 6572 6f73 2833 290a  m = np.zeros(3).
+0000e920: 2020 206d 6173 7320 3d20 302e 300a 2020     mass = 0.0.  
+0000e930: 2066 6f72 206d 2c78 797a 2069 6e20 7a69   for m,xyz in zi
+0000e940: 7028 6d61 7373 6573 2c78 797a 7329 3a0a  p(masses,xyzs):.
+0000e950: 2020 2020 2020 206d 6173 7320 2b3d 206d         mass += m
+0000e960: 0a20 2020 2020 2020 636d 2020 202b 3d20  .       cm   += 
+0000e970: 6d2a 7879 7a0a 2020 2063 6d20 2f3d 206d  m*xyz.   cm /= m
+0000e980: 6173 730a 2020 2072 6574 7572 6e20 6d61  ass.   return ma
+0000e990: 7373 2c63 6d0a 0a64 6566 206f 7274 686f  ss,cm..def ortho
+0000e9a0: 676f 6e61 6c69 7365 5f70 726f 6a65 6374  gonalise_project
+0000e9b0: 696f 6e5f 6f70 6572 6174 6f72 2870 7329  ion_operator(ps)
+0000e9c0: 3a0a 2020 2027 2727 4f72 7468 6f67 6f6e  :.   '''Orthogon
+0000e9d0: 616c 6973 6520 7468 6520 7072 6f6a 6563  alise the projec
+0000e9e0: 7469 6f6e 206f 7065 7261 746f 7273 2070  tion operators p
+0000e9f0: 7327 2727 0a20 2020 2320 5468 6520 7072  s'''.   # The pr
+0000ea00: 6f6a 6563 7469 6f6e 206f 7065 7261 746f  ojection operato
+0000ea10: 7220 6861 7320 6469 6d65 6e73 696f 6e20  r has dimension 
+0000ea20: 5b36 2c6e 6174 6f6d 732a 335d 0a20 2020  [6,natoms*3].   
+0000ea30: 6d61 7863 7963 203d 2031 300a 2020 2063  maxcyc = 10.   c
+0000ea40: 7963 6c65 203d 2030 0a20 2020 6d61 785f  ycle = 0.   max_
+0000ea50: 6f76 6572 6c61 7020 3d20 312e 300a 2020  overlap = 1.0.  
+0000ea60: 2077 6869 6c65 2063 7963 6c65 203c 206d   while cycle < m
+0000ea70: 6178 6379 6320 616e 6420 6d61 785f 6f76  axcyc and max_ov
+0000ea80: 6572 6c61 7020 3e20 312e 3045 2d38 3a0a  erlap > 1.0E-8:.
+0000ea90: 2020 2020 2020 2063 7963 6c65 202b 3d20         cycle += 
+0000eaa0: 310a 2020 2020 2020 206d 6178 5f6f 7665  1.       max_ove
+0000eab0: 726c 6170 203d 2030 2e30 0a20 2020 2020  rlap = 0.0.     
+0000eac0: 2020 666f 7220 692c 7020 696e 2065 6e75    for i,p in enu
+0000ead0: 6d65 7261 7465 2870 7329 3a0a 2020 2020  merate(ps):.    
+0000eae0: 2020 2020 2020 2023 204e 6f72 6d61 6c69         # Normali
+0000eaf0: 7365 2074 6865 2070 726f 6a65 6374 696f  se the projectio
+0000eb00: 6e20 6f70 6572 6174 6f72 0a20 2020 2020  n operator.     
+0000eb10: 2020 2020 2020 616e 6f72 6d20 3d20 6e70        anorm = np
+0000eb20: 2e64 6f74 2870 2c70 290a 2020 2020 2020  .dot(p,p).      
+0000eb30: 2020 2020 2073 6869 6674 203d 2030 2e30       shift = 0.0
+0000eb40: 0a20 2020 2020 2020 2020 2020 6966 2061  .           if a
+0000eb50: 6e6f 726d 203c 2031 2e30 652d 3132 3a0a  norm < 1.0e-12:.
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eb70: 6869 6674 203d 2031 2e30 452d 3132 0a20  hift = 1.0E-12. 
+0000eb80: 2020 2020 2020 2020 2020 7020 3d20 7020            p = p 
+0000eb90: 2f20 6e70 2e73 7172 7428 6e70 2e64 6f74  / np.sqrt(np.dot
+0000eba0: 2870 2c70 2920 2b20 7368 6966 7420 290a  (p,p) + shift ).
+0000ebb0: 2020 2020 2020 2020 2020 2070 735b 695d             ps[i]
+0000ebc0: 203d 2070 0a20 2020 2020 2020 2020 2020   = p.           
+0000ebd0: 666f 7220 6a2c 7120 696e 2065 6e75 6d65  for j,q in enume
+0000ebe0: 7261 7465 2870 7329 3a0a 2020 2020 2020  rate(ps):.      
+0000ebf0: 2020 2020 2020 2020 2069 6620 6a20 3e20           if j > 
+0000ec00: 693a 0a20 2020 2020 2020 2020 2020 2020  i:.             
+0000ec10: 2020 2020 2020 2320 4772 616d 6d20 5363        # Gramm Sc
+0000ec20: 686d 6964 7420 6f72 7468 6f67 6f6e 6f61  hmidt orthogonoa
+0000ec30: 6c69 7361 7469 6f6e 0a20 2020 2020 2020  lisation.       
+0000ec40: 2020 2020 2020 2020 2020 2020 646f 7470              dotp
+0000ec50: 726f 6420 3d20 6e70 2e64 6f74 2870 2c71  rod = np.dot(p,q
+0000ec60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ec70: 2020 2020 2070 735b 6a5d 203d 2071 202d       ps[j] = q -
+0000ec80: 2064 6f74 7072 6f64 2a70 0a20 2020 2020   dotprod*p.     
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000eca0: 206d 6178 5f6f 7665 726c 6170 203c 2064   max_overlap < d
+0000ecb0: 6f74 7072 6f64 3a0a 2020 2020 2020 2020  otprod:.        
+0000ecc0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000ecd0: 6178 5f6f 7665 726c 6170 203d 2064 6f74  ax_overlap = dot
+0000ece0: 7072 6f64 0a20 2020 6966 2063 7963 6c65  prod.   if cycle
+0000ecf0: 203e 3d20 6d61 7863 7963 3a0a 2020 2020   >= maxcyc:.    
+0000ed00: 2020 2070 7269 6e74 2827 5741 524e 494e     print('WARNIN
+0000ed10: 4720 5363 686d 6964 7420 4f72 7468 6f67  G Schmidt Orthog
+0000ed20: 6f6e 616c 6973 6174 696f 6e20 4661 696c  onalisation Fail
+0000ed30: 6564 272c 206d 6178 5f6f 7665 726c 6170  ed', max_overlap
+0000ed40: 290a 2020 2020 2020 2065 7869 7428 290a  ).       exit().
+0000ed50: 2020 2072 6574 7572 6e20 7073 0a0a 6465     return ps..de
+0000ed60: 6620 636f 6e73 7472 7563 745f 7072 6f6a  f construct_proj
+0000ed70: 6563 7469 6f6e 5f6f 7065 7261 746f 7228  ection_operator(
+0000ed80: 6174 6f6d 732c 2078 797a 732c 206d 6173  atoms, xyzs, mas
+0000ed90: 7365 732c 206e 6174 7329 3a0a 2020 2027  ses, nats):.   '
+0000eda0: 2727 436f 6e73 7472 7563 7420 7468 6520  ''Construct the 
+0000edb0: 7072 6f6a 6563 7469 6f6e 206f 7065 7261  projection opera
+0000edc0: 746f 7220 666f 7220 7468 6520 6d6f 6c65  tor for the mole
+0000edd0: 6375 6c65 2064 6566 696e 6564 2062 7920  cule defined by 
+0000ede0: 6174 6f6d 732c 2078 797a 2c20 6d61 7373  atoms, xyz, mass
+0000edf0: 6573 2727 270a 2020 206d 6173 732c 636d  es'''.   mass,cm
+0000ee00: 203d 2063 616c 6375 6c61 7465 5f63 656e   = calculate_cen
+0000ee10: 7472 655f 6f66 5f6d 6173 7328 7879 7a73  tre_of_mass(xyzs
+0000ee20: 2c6d 6173 7365 7329 0a20 2020 2320 5468  ,masses).   # Th
+0000ee30: 6520 7072 6f6a 6563 7469 6f6e 206f 7065  e projection ope
+0000ee40: 7261 746f 7220 6861 7320 6469 6d65 6e73  rator has dimens
+0000ee50: 696f 6e20 6e75 6d62 6572 5f6f 665f 636f  ion number_of_co
+0000ee60: 6e73 7472 6169 6e74 732a 6e61 746f 6d73  nstraints*natoms
+0000ee70: 2a33 0a20 2020 7073 203d 206e 702e 7a65  *3.   ps = np.ze
+0000ee80: 726f 7328 2028 362c 6e61 7473 2a33 2920  ros( (6,nats*3) 
+0000ee90: 290a 2020 2078 203d 2030 0a20 2020 7920  ).   x = 0.   y 
+0000eea0: 3d20 310a 2020 207a 203d 2032 0a20 2020  = 1.   z = 2.   
+0000eeb0: 666f 7220 692c 6d61 7373 2c78 797a 2069  for i,mass,xyz i
+0000eec0: 6e20 7a69 7028 6174 6f6d 732c 6d61 7373  n zip(atoms,mass
+0000eed0: 6573 2c78 797a 7329 3a0a 2020 2020 2020  es,xyzs):.      
+0000eee0: 2070 735b 302c 692a 332b 785d 203d 206d   ps[0,i*3+x] = m
+0000eef0: 6174 682e 7371 7274 286d 6173 7329 0a20  ath.sqrt(mass). 
+0000ef00: 2020 2020 2020 7073 5b31 2c69 2a33 2b79        ps[1,i*3+y
+0000ef10: 5d20 3d20 6d61 7468 2e73 7172 7428 6d61  ] = math.sqrt(ma
+0000ef20: 7373 290a 2020 2020 2020 2070 735b 322c  ss).       ps[2,
+0000ef30: 692a 332b 7a5d 203d 206d 6174 682e 7371  i*3+z] = math.sq
+0000ef40: 7274 286d 6173 7329 0a20 2020 2020 2020  rt(mass).       
+0000ef50: 2320 636f 6f72 6469 6e61 7465 7320 7265  # coordinates re
+0000ef60: 6c61 7469 7665 2074 6f20 7468 6520 6365  lative to the ce
+0000ef70: 6e74 7265 206f 6620 6d61 7373 0a20 2020  ntre of mass.   
+0000ef80: 2020 2020 7265 6c78 797a 203d 206d 6174      relxyz = mat
+0000ef90: 682e 7371 7274 286d 6173 7329 202a 2028  h.sqrt(mass) * (
+0000efa0: 7879 7a20 2d20 636d 290a 2020 2020 2020  xyz - cm).      
+0000efb0: 2023 2046 6972 7374 2072 6f74 6174 696f   # First rotatio
+0000efc0: 6e73 2061 626f 7574 2078 2069 6e20 7468  ns about x in th
+0000efd0: 6520 792f 7a20 706c 616e 650a 2020 2020  e y/z plane.    
+0000efe0: 2020 2023 207a 7a20 6973 2072 6561 6c6c     # zz is reall
+0000eff0: 7920 722a 7369 6e28 7468 6574 6129 2c20  y r*sin(theta), 
+0000f000: 616e 6420 7369 6e28 7468 6574 6129 203d  and sin(theta) =
+0000f010: 207a 7a2f 720a 2020 2020 2020 2023 2079   zz/r.       # y
+0000f020: 7920 6973 2072 6561 6c6c 7920 722a 636f  y is really r*co
+0000f030: 7328 7468 6574 6129 2c20 616e 6420 636f  s(theta), and co
+0000f040: 7328 7468 6574 6129 203d 2079 792f 720a  s(theta) = yy/r.
+0000f050: 2020 2020 2020 2070 735b 332c 692a 332b         ps[3,i*3+
+0000f060: 785d 203d 2030 2e30 0a20 2020 2020 2020  x] = 0.0.       
+0000f070: 7073 5b33 2c69 2a33 2b79 5d20 3d20 2d72  ps[3,i*3+y] = -r
+0000f080: 656c 7879 7a5b 7a5d 0a20 2020 2020 2020  elxyz[z].       
+0000f090: 7073 5b33 2c69 2a33 2b7a 5d20 3d20 2b72  ps[3,i*3+z] = +r
+0000f0a0: 656c 7879 7a5b 795d 0a20 2020 2020 2020  elxyz[y].       
+0000f0b0: 2320 4e65 7874 2072 6f74 6174 696f 6e73  # Next rotations
+0000f0c0: 2061 626f 7574 2079 2069 6e20 7468 6520   about y in the 
+0000f0d0: 782f 7a20 706c 616e 650a 2020 2020 2020  x/z plane.      
+0000f0e0: 2070 735b 342c 692a 332b 785d 203d 202b   ps[4,i*3+x] = +
+0000f0f0: 7265 6c78 797a 5b7a 5d0a 2020 2020 2020  relxyz[z].      
+0000f100: 2070 735b 342c 692a 332b 795d 203d 2030   ps[4,i*3+y] = 0
+0000f110: 2e30 0a20 2020 2020 2020 7073 5b34 2c69  .0.       ps[4,i
+0000f120: 2a33 2b7a 5d20 3d20 2d72 656c 7879 7a5b  *3+z] = -relxyz[
+0000f130: 785d 0a20 2020 2020 2020 2320 4e65 7874  x].       # Next
+0000f140: 2072 6f74 6174 696f 6e73 2061 626f 7574   rotations about
+0000f150: 207a 2069 6e20 7468 6520 782f 7920 706c   z in the x/y pl
+0000f160: 616e 650a 2020 2020 2020 2070 735b 352c  ane.       ps[5,
+0000f170: 692a 332b 785d 203d 202d 7265 6c78 797a  i*3+x] = -relxyz
+0000f180: 5b79 5d0a 2020 2020 2020 2070 735b 352c  [y].       ps[5,
+0000f190: 692a 332b 795d 203d 202b 7265 6c78 797a  i*3+y] = +relxyz
+0000f1a0: 5b78 5d0a 2020 2020 2020 2070 735b 352c  [x].       ps[5,
+0000f1b0: 692a 332b 7a5d 203d 2030 2e30 0a20 2020  i*3+z] = 0.0.   
+0000f1c0: 7265 7475 726e 2070 730a 0a64 6566 2063  return ps..def c
+0000f1d0: 616c 6375 6c61 7465 5f65 6e65 7267 795f  alculate_energy_
+0000f1e0: 6469 7374 7269 6275 7469 6f6e 2863 656c  distribution(cel
+0000f1f0: 6c2c 2066 7265 7175 656e 6369 6573 2c20  l, frequencies, 
+0000f200: 6e6f 726d 616c 5f6d 6f64 6573 2c20 6465  normal_modes, de
+0000f210: 6275 673d 4661 6c73 6529 3a0a 2020 2027  bug=False):.   '
+0000f220: 2727 4361 6c63 756c 6174 6520 656e 6572  ''Calculate ener
+0000f230: 6779 2064 6973 7472 6962 7574 696f 6e20  gy distribution 
+0000f240: 696e 2074 6865 2070 686f 6e6f 6e20 6d6f  in the phonon mo
+0000f250: 6465 730a 2020 2020 2020 6672 6571 7565  des.      freque
+0000f260: 6e63 6965 7320 6172 6520 7468 6520 6672  ncies are the fr
+0000f270: 6571 7565 6e63 6965 7320 696e 2063 6d2d  equencies in cm-
+0000f280: 310a 2020 2020 2020 6e6f 726d 616c 5f6d  1.      normal_m
+0000f290: 6f64 6573 2061 7265 2074 6865 206d 6173  odes are the mas
+0000f2a0: 7320 7765 6967 6874 6564 206e 6f72 6d61  s weighted norma
+0000f2b0: 6c20 6d6f 6465 7327 2727 0a20 2020 6d6f  l modes'''.   mo
+0000f2c0: 6c65 6375 6c65 7320 3d20 6365 6c6c 2e6d  lecules = cell.m
+0000f2d0: 6f6c 6563 756c 6573 0a20 2020 6174 6f6d  olecules.   atom
+0000f2e0: 6963 5f6d 6173 7365 7320 3d20 6365 6c6c  ic_masses = cell
+0000f2f0: 2e61 746f 6d69 635f 6d61 7373 6573 0a20  .atomic_masses. 
+0000f300: 2020 7879 7a20 3d20 6365 6c6c 2e78 797a    xyz = cell.xyz
+0000f310: 5f63 6f6f 7264 696e 6174 6573 0a20 2020  _coordinates.   
+0000f320: 6e61 7473 203d 206c 656e 2878 797a 290a  nats = len(xyz).
+0000f330: 2020 2023 2043 616c 6375 6c61 7465 2074     # Calculate t
+0000f340: 6865 2070 726f 6a65 6374 696f 6e73 206f  he projections o
+0000f350: 7065 7261 746f 7273 2066 6f72 2065 6163  perators for eac
+0000f360: 6820 6d6f 6c65 6375 6c65 0a20 2020 6d6f  h molecule.   mo
+0000f370: 6c65 6375 6c61 725f 7072 6f6a 6563 7469  lecular_projecti
+0000f380: 6f6e 5f6f 7065 7261 746f 7273 203d 205b  on_operators = [
+0000f390: 5d0a 2020 206d 6f6c 6563 756c 655f 6d61  ].   molecule_ma
+0000f3a0: 736b 7320 3d20 5b5d 0a20 2020 666f 7220  sks = [].   for 
+0000f3b0: 6174 6f6d 7320 696e 206d 6f6c 6563 756c  atoms in molecul
+0000f3c0: 6573 3a0a 2020 2020 2020 206d 6f6c 5f78  es:.       mol_x
+0000f3d0: 797a 7320 203d 205b 2078 797a 5b61 746f  yzs  = [ xyz[ato
+0000f3e0: 6d5d 2066 6f72 2061 746f 6d20 696e 2061  m] for atom in a
+0000f3f0: 746f 6d73 5d0a 2020 2020 2020 206d 6f6c  toms].       mol
+0000f400: 5f6d 6173 6b20 3d20 6e70 2e7a 6572 6f73  _mask = np.zeros
+0000f410: 286e 6174 732a 3329 0a20 2020 2020 2020  (nats*3).       
+0000f420: 666f 7220 6174 6f6d 2069 6e20 6174 6f6d  for atom in atom
+0000f430: 733a 0a20 2020 2020 2020 2020 2020 6d6f  s:.           mo
+0000f440: 6c5f 6d61 736b 5b33 2a61 746f 6d2b 305d  l_mask[3*atom+0]
+0000f450: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+0000f460: 6d6f 6c5f 6d61 736b 5b33 2a61 746f 6d2b  mol_mask[3*atom+
+0000f470: 315d 203d 2031 0a20 2020 2020 2020 2020  1] = 1.         
+0000f480: 2020 6d6f 6c5f 6d61 736b 5b33 2a61 746f    mol_mask[3*ato
+0000f490: 6d2b 325d 203d 2031 0a20 2020 2020 2020  m+2] = 1.       
+0000f4a0: 6d6f 6c5f 6d61 7373 6573 203d 205b 2061  mol_masses = [ a
+0000f4b0: 746f 6d69 635f 6d61 7373 6573 5b61 746f  tomic_masses[ato
+0000f4c0: 6d5d 2066 6f72 2061 746f 6d20 696e 2061  m] for atom in a
+0000f4d0: 746f 6d73 5d0a 2020 2020 2020 2070 726f  toms].       pro
+0000f4e0: 6a65 6374 696f 6e5f 6f70 6572 6174 6f72  jection_operator
+0000f4f0: 7320 3d20 636f 6e73 7472 7563 745f 7072  s = construct_pr
+0000f500: 6f6a 6563 7469 6f6e 5f6f 7065 7261 746f  ojection_operato
+0000f510: 7228 6174 6f6d 732c 6d6f 6c5f 7879 7a73  r(atoms,mol_xyzs
+0000f520: 2c6d 6f6c 5f6d 6173 7365 732c 6e61 7473  ,mol_masses,nats
+0000f530: 290a 2020 2020 2020 2070 726f 6a65 6374  ).       project
+0000f540: 696f 6e5f 6f70 6572 6174 6f72 7320 3d20  ion_operators = 
+0000f550: 6f72 7468 6f67 6f6e 616c 6973 655f 7072  orthogonalise_pr
+0000f560: 6f6a 6563 7469 6f6e 5f6f 7065 7261 746f  ojection_operato
+0000f570: 7228 7072 6f6a 6563 7469 6f6e 5f6f 7065  r(projection_ope
+0000f580: 7261 746f 7273 290a 2020 2020 2020 206d  rators).       m
+0000f590: 6f6c 6563 756c 6172 5f70 726f 6a65 6374  olecular_project
+0000f5a0: 696f 6e5f 6f70 6572 6174 6f72 732e 6170  ion_operators.ap
+0000f5b0: 7065 6e64 2870 726f 6a65 6374 696f 6e5f  pend(projection_
+0000f5c0: 6f70 6572 6174 6f72 7329 0a20 2020 2020  operators).     
+0000f5d0: 2020 230a 2020 2020 2020 206d 6f6c 6563    #.       molec
+0000f5e0: 756c 655f 6d61 736b 732e 6170 7065 6e64  ule_masks.append
+0000f5f0: 286d 6f6c 5f6d 6173 6b29 0a20 2020 2320  (mol_mask).   # 
+0000f600: 4361 6c63 756c 6174 6520 7468 6520 636f  Calculate the co
+0000f610: 6e74 7269 6275 7469 6f6e 7320 746f 2074  ntributions to t
+0000f620: 6865 206b 696e 6574 6963 2065 6e65 7267  he kinetic energ
+0000f630: 7920 696e 2065 6163 6820 6d6f 6465 0a20  y in each mode. 
+0000f640: 2020 656e 6572 6769 6573 5f69 6e5f 6d6f    energies_in_mo
+0000f650: 6465 7320 3d20 5b5d 0a20 2020 666f 7220  des = [].   for 
+0000f660: 696d 6f64 652c 6d6f 6465 2069 6e20 656e  imode,mode in en
+0000f670: 756d 6572 6174 6528 6e6f 726d 616c 5f6d  umerate(normal_m
+0000f680: 6f64 6573 293a 0a20 2020 2020 2020 6d6f  odes):.       mo
+0000f690: 6465 5f63 6d20 3d20 6d6f 6465 0a20 2020  de_cm = mode.   
+0000f6a0: 2020 2020 6365 6e74 7265 5f6f 665f 6d61      centre_of_ma
+0000f6b0: 7373 5f65 6e65 7267 7920 3d20 302e 300a  ss_energy = 0.0.
+0000f6c0: 2020 2020 2020 2072 6f74 6174 696f 6e61         rotationa
+0000f6d0: 6c5f 656e 6572 6779 203d 2030 2e30 0a20  l_energy = 0.0. 
+0000f6e0: 2020 2020 2020 6d6f 6c65 6375 6c61 725f        molecular_
+0000f6f0: 656e 6572 6769 6573 203d 205b 5d0a 2020  energies = [].  
+0000f700: 2020 2020 2066 6f72 2069 6d6f 6c2c 2870       for imol,(p
+0000f710: 732c 6d61 736b 2920 696e 2065 6e75 6d65  s,mask) in enume
+0000f720: 7261 7465 287a 6970 286d 6f6c 6563 756c  rate(zip(molecul
+0000f730: 6172 5f70 726f 6a65 6374 696f 6e5f 6f70  ar_projection_op
+0000f740: 6572 6174 6f72 732c 6d6f 6c65 6375 6c65  erators,molecule
+0000f750: 5f6d 6173 6b73 2929 3a0a 2020 2020 2020  _masks)):.      
+0000f760: 2020 2020 2023 2043 616c 6375 6c61 7465       # Calculate
+0000f770: 2074 6f74 616c 206b 696e 6574 6963 2065   total kinetic e
+0000f780: 6e65 7267 790a 2020 2020 2020 2020 2020  nergy.          
+0000f790: 2074 6f74 616c 5f65 6e65 7267 7920 3d20   total_energy = 
+0000f7a0: 6e70 2e64 6f74 286d 6f64 652c 6d6f 6465  np.dot(mode,mode
+0000f7b0: 290a 2020 2020 2020 2020 2020 2023 2050  ).           # P
+0000f7c0: 726f 6a65 6374 206f 7574 2063 656e 7472  roject out centr
+0000f7d0: 6520 6f66 206d 6173 7320 6d6f 7469 6f6e  e of mass motion
+0000f7e0: 206f 6620 6561 6368 206d 6f6c 6563 756c   of each molecul
+0000f7f0: 650a 2020 2020 2020 2020 2020 206d 6f64  e.           mod
+0000f800: 655f 636d 203d 206d 6f64 6520 2d20 6e70  e_cm = mode - np
+0000f810: 2e64 6f74 286d 6f64 652c 7073 5b30 5d29  .dot(mode,ps[0])
+0000f820: 2a70 735b 305d 202d 206e 702e 646f 7428  *ps[0] - np.dot(
+0000f830: 6d6f 6465 2c70 735b 315d 292a 7073 5b31  mode,ps[1])*ps[1
+0000f840: 5d20 2d20 6e70 2e64 6f74 286d 6f64 652c  ] - np.dot(mode,
+0000f850: 7073 5b32 5d29 2a70 735b 325d 0a20 2020  ps[2])*ps[2].   
+0000f860: 2020 2020 2020 2020 6365 6e74 7265 5f6f          centre_o
+0000f870: 665f 6d61 7373 5f65 6e65 7267 7920 2b3d  f_mass_energy +=
+0000f880: 2074 6f74 616c 5f65 6e65 7267 7920 2d20   total_energy - 
+0000f890: 6e70 2e64 6f74 286d 6f64 655f 636d 2c6d  np.dot(mode_cm,m
+0000f8a0: 6f64 655f 636d 290a 2020 2020 2020 2020  ode_cm).        
+0000f8b0: 2020 2023 2050 726f 6a65 6374 206f 7574     # Project out
+0000f8c0: 206d 6f6c 6563 756c 6172 2072 6f74 6174   molecular rotat
+0000f8d0: 696f 6e20 6f66 2065 6163 6820 6d6f 6c65  ion of each mole
+0000f8e0: 6375 6c65 0a20 2020 2020 2020 2020 2020  cule.           
+0000f8f0: 6d6f 6465 5f63 6d20 3d20 6d6f 6465 202d  mode_cm = mode -
+0000f900: 206e 702e 646f 7428 6d6f 6465 2c70 735b   np.dot(mode,ps[
+0000f910: 335d 292a 7073 5b33 5d20 2d20 6e70 2e64  3])*ps[3] - np.d
+0000f920: 6f74 286d 6f64 652c 7073 5b34 5d29 2a70  ot(mode,ps[4])*p
+0000f930: 735b 345d 202d 206e 702e 646f 7428 6d6f  s[4] - np.dot(mo
+0000f940: 6465 2c70 735b 355d 292a 7073 5b35 5d0a  de,ps[5])*ps[5].
+0000f950: 2020 2020 2020 2020 2020 2072 6f74 6174             rotat
+0000f960: 696f 6e61 6c5f 656e 6572 6779 202b 3d20  ional_energy += 
+0000f970: 746f 7461 6c5f 656e 6572 6779 202d 206e  total_energy - n
+0000f980: 702e 646f 7428 6d6f 6465 5f63 6d2c 6d6f  p.dot(mode_cm,mo
+0000f990: 6465 5f63 6d29 0a20 2020 2020 2020 2020  de_cm).         
+0000f9a0: 2020 2320 4e6f 7720 776f 726b 206f 7574    # Now work out
+0000f9b0: 2074 6865 2065 6e65 7267 7920 6f66 2074   the energy of t
+0000f9c0: 6865 206d 6f6c 6563 756c 650a 2020 2020  he molecule.    
+0000f9d0: 2020 2020 2020 206d 6f64 655f 636d 203d         mode_cm =
+0000f9e0: 206d 6173 6b20 2a20 6d6f 6465 0a20 2020   mask * mode.   
+0000f9f0: 2020 2020 2020 2020 6d6f 6c5f 656e 6572          mol_ener
+0000fa00: 6779 203d 206e 702e 646f 7428 6d6f 6465  gy = np.dot(mode
+0000fa10: 5f63 6d2c 6d6f 6465 5f63 6d29 0a20 2020  _cm,mode_cm).   
+0000fa20: 2020 2020 2020 2020 6d6f 6c65 6375 6c61          molecula
+0000fa30: 725f 656e 6572 6769 6573 2e61 7070 656e  r_energies.appen
+0000fa40: 6428 6d6f 6c5f 656e 6572 6779 290a 2020  d(mol_energy).  
+0000fa50: 2020 2020 2023 2065 6e64 2066 6f72 2069       # end for i
+0000fa60: 6d6f 6c2c 7073 0a20 2020 2020 2020 7669  mol,ps.       vi
+0000fa70: 6272 6174 696f 6e61 6c5f 656e 6572 6779  brational_energy
+0000fa80: 203d 2074 6f74 616c 5f65 6e65 7267 7920   = total_energy 
+0000fa90: 2d20 6365 6e74 7265 5f6f 665f 6d61 7373  - centre_of_mass
+0000faa0: 5f65 6e65 7267 7920 2d20 726f 7461 7469  _energy - rotati
+0000fab0: 6f6e 616c 5f65 6e65 7267 790a 2020 2020  onal_energy.    
+0000fac0: 2020 2065 6e65 7267 6965 735f 696e 5f6d     energies_in_m
+0000fad0: 6f64 6573 2e61 7070 656e 6428 2028 746f  odes.append( (to
+0000fae0: 7461 6c5f 656e 6572 6779 2c63 656e 7472  tal_energy,centr
+0000faf0: 655f 6f66 5f6d 6173 735f 656e 6572 6779  e_of_mass_energy
+0000fb00: 2c72 6f74 6174 696f 6e61 6c5f 656e 6572  ,rotational_ener
+0000fb10: 6779 2c76 6962 7261 7469 6f6e 616c 5f65  gy,vibrational_e
+0000fb20: 6e65 7267 792c 6d6f 6c65 6375 6c61 725f  nergy,molecular_
+0000fb30: 656e 6572 6769 6573 2920 290a 2020 2023  energies) ).   #
+0000fb40: 2065 6e64 2066 6f72 206d 6f64 6520 696e   end for mode in
+0000fb50: 206e 6f72 6d61 6c20 6d6f 6465 730a 2020   normal modes.  
+0000fb60: 2072 6574 7572 6e20 656e 6572 6769 6573   return energies
+0000fb70: 5f69 6e5f 6d6f 6465 730a 2320 656e 6420  _in_modes.# end 
+0000fb80: 6465 660a 0a0a 6465 6620 686f 6472 6963  def...def hodric
+0000fb90: 6b5f 7072 6573 636f 7474 5f66 696c 7465  k_prescott_filte
+0000fba0: 7228 792c 6461 6d70 696e 672c 6c61 6d62  r(y,damping,lamb
+0000fbb0: 6461 5f76 616c 7565 2c6e 6974 6572 7329  da_value,niters)
+0000fbc0: 3a0a 2020 2020 230a 2020 2020 2320 4170  :.    #.    # Ap
+0000fbd0: 706c 7920 6120 486f 6472 6963 6b20 5072  ply a Hodrick Pr
+0000fbe0: 6573 636f 7474 2066 696c 7465 7220 746f  escott filter to
+0000fbf0: 2074 6865 2073 7065 6374 7275 6d20 696e   the spectrum in
+0000fc00: 2078 2c20 790a 2020 2020 2320 7920 6973   x, y.    # y is
+0000fc10: 2074 6865 2065 7870 6572 696d 656e 7461   the experimenta
+0000fc20: 6c20 6162 736f 7270 7469 6f6e 0a20 2020  l absorption.   
+0000fc30: 2023 2064 616d 7069 6e67 2069 7320 7573   # damping is us
+0000fc40: 6564 2074 6f20 6461 6d70 2074 6865 2069  ed to damp the i
+0000fc50: 7465 7261 7469 6f6e 730a 2020 2020 2320  terations.    # 
+0000fc60: 6c61 6d62 6461 5f76 616c 7565 2069 7320  lambda_value is 
+0000fc70: 7468 6520 6368 6f73 656e 2073 6d6f 6f74  the chosen smoot
+0000fc80: 6869 6e67 2066 6163 746f 720a 2020 2020  hing factor.    
+0000fc90: 2320 4261 7365 6420 6f6e 2069 6465 6173  # Based on ideas
+0000fca0: 2069 6e20 7468 6520 7468 6573 6973 206f   in the thesis o
+0000fcb0: 6620 4d61 7961 6e6b 204b 6175 7368 696b  f Mayank Kaushik
+0000fcc0: 2028 556e 6976 6572 7369 7479 2041 6465   (University Ade
+0000fcd0: 6c61 6964 6529 0a20 2020 2023 0a20 2020  laide).    #.   
+0000fce0: 2066 726f 6d20 7363 6970 7920 696d 706f   from scipy impo
+0000fcf0: 7274 2073 7061 7273 650a 2020 2020 230a  rt sparse.    #.
+0000fd00: 2020 2020 2320 4372 6561 7465 2061 2073      # Create a s
+0000fd10: 7061 7273 6520 3372 6420 6f72 6465 7220  parse 3rd order 
+0000fd20: 6469 6666 6572 656e 6365 206f 7065 7261  difference opera
+0000fd30: 746f 720a 2020 2020 230a 2020 2020 6e20  tor.    #.    n 
+0000fd40: 3d20 6c65 6e28 7929 0a20 2020 2064 6961  = len(y).    dia
+0000fd50: 6720 3d20 6e70 2e6f 6e65 7328 6e2d 3329  g = np.ones(n-3)
+0000fd60: 0a20 2020 2044 203d 2073 7061 7273 652e  .    D = sparse.
+0000fd70: 7370 6469 6167 7328 205b 2d31 2a64 6961  spdiags( [-1*dia
+0000fd80: 672c 2033 2a64 6961 672c 202d 332a 6469  g, 3*diag, -3*di
+0000fd90: 6167 2c20 312a 6469 6167 5d2c 0a20 2020  ag, 1*diag],.   
+0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdb0: 2020 2020 205b 302c 202d 312c 202d 322c       [0, -1, -2,
+0000fdc0: 202d 335d 2c20 6e2c 206e 2d33 2029 2e74   -3], n, n-3 ).t
+0000fdd0: 6f63 7363 2829 0a20 2020 2077 203d 206e  ocsc().    w = n
+0000fde0: 702e 6f6e 6573 286e 290a 2020 2020 666f  p.ones(n).    fo
+0000fdf0: 7220 6974 2069 6e20 7261 6e67 6528 3130  r it in range(10
+0000fe00: 2a6e 6974 6572 7329 3a0a 2020 2020 2020  *niters):.      
+0000fe10: 2020 5720 3d20 7370 6172 7365 2e73 7064    W = sparse.spd
+0000fe20: 6961 6773 2877 2c20 302c 206e 2c20 6e29  iags(w, 0, n, n)
+0000fe30: 2e74 6f63 7363 2829 0a20 2020 2020 2020  .tocsc().       
+0000fe40: 2023 2050 726f 626c 656d 7320 7769 7468   # Problems with
+0000fe50: 206f 7665 7266 6c6f 7720 6966 206c 616d   overflow if lam
+0000fe60: 6264 6120 6973 206c 6172 6765 0a20 2020  bda is large.   
+0000fe70: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000fe80: 2020 2020 2020 5a20 3d20 5720 2b20 706f        Z = W + po
+0000fe90: 7728 3130 2c6c 616d 6264 615f 7661 6c75  w(10,lambda_valu
+0000fea0: 6529 202a 2028 442e 646f 7428 442e 7472  e) * (D.dot(D.tr
+0000feb0: 616e 7370 6f73 6528 2929 290a 2020 2020  anspose())).    
+0000fec0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+0000fed0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+0000fee0: 2020 2020 207a 203d 2073 7061 7273 652e       z = sparse.
+0000fef0: 6c69 6e61 6c67 2e73 7073 6f6c 7665 285a  linalg.spsolve(Z
+0000ff00: 2c20 772a 7929 0a20 2020 2020 2020 2023  , w*y).        #
+0000ff10: 2072 6573 6964 7561 6c73 203d 2079 202d   residuals = y -
+0000ff20: 207a 0a20 2020 2020 2020 2023 2065 7272   z.        # err
+0000ff30: 6f72 203d 2073 756d 2820 722a 7220 666f  or = sum( r*r fo
+0000ff40: 7220 7220 696e 2072 6573 6964 7561 6c73  r r in residuals
+0000ff50: 2069 6620 7220 3c20 302e 3020 290a 2020   if r < 0.0 ).  
+0000ff60: 2020 2020 2020 2320 6572 726f 7220 3d20        # error = 
+0000ff70: 6d61 7468 2e73 7172 7428 6572 726f 722f  math.sqrt(error/
+0000ff80: 6e29 0a20 2020 2020 2020 2077 203d 2064  n).        w = d
+0000ff90: 616d 7069 6e67 2a28 793e 7a29 202b 2028  amping*(y>z) + (
+0000ffa0: 312d 6461 6d70 696e 6729 2a28 793c 7a29  1-damping)*(y<z)
+0000ffb0: 0a20 2020 2020 2020 2023 2070 7269 6e74  .        # print
+0000ffc0: 2869 742c 2065 7272 6f72 290a 2020 2020  (it, error).    
+0000ffd0: 7265 7475 726e 2079 2d7a 0a0a 6465 6620  return y-z..def 
+0000ffe0: 7265 666c 6563 7461 6e63 655f 6174 7228  reflectance_atr(
+0000fff0: 6e73 2c6e 302c 7468 6574 612c 6174 7253  ns,n0,theta,atrS
+00010000: 506f 6c46 7261 6374 696f 6e29 3a0a 2020  PolFraction):.  
+00010010: 2020 230a 2020 2020 2320 4361 6c63 756c    #.    # Calcul
+00010020: 6174 6520 7468 6520 6174 7220 7320 616e  ate the atr s an
+00010030: 6420 7020 7265 666c 6563 7461 6e63 650a  d p reflectance.
+00010040: 2020 2020 2320 6e73 2069 7320 7468 6520      # ns is the 
+00010050: 636f 6d70 6c65 7820 7065 726d 6974 7469  complex permitti
+00010060: 7669 7479 206f 6620 7468 6520 6566 6665  vity of the effe
+00010070: 6374 6976 6520 6d65 6469 756d 0a20 2020  ctive medium.   
+00010080: 2023 206e 3020 6973 2074 6865 2070 6572   # n0 is the per
+00010090: 6d69 7474 6976 6974 7920 6f66 2061 7472  mittivity of atr
+000100a0: 206d 6174 6572 6961 6c0a 2020 2020 2320   material.    # 
+000100b0: 7468 6574 6120 6973 2074 6865 2061 6e67  theta is the ang
+000100c0: 6c65 206f 6620 696e 6369 6465 6e63 6520  le of incidence 
+000100d0: 696e 2064 6567 7265 6573 0a20 2020 2023  in degrees.    #
+000100e0: 2061 7472 5350 6f6c 4672 6163 7469 6f6e   atrSPolFraction
+000100f0: 2069 7320 7468 6520 6672 6163 7469 6f6e   is the fraction
+00010100: 206f 6620 5320 7761 7665 2074 6f20 6265   of S wave to be
+00010110: 2063 6f6e 7369 6465 7265 640a 2020 2020   considered.    
+00010120: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00010130: 2020 5468 6520 616d 6f75 6e74 206f 6620    The amount of 
+00010140: 5020 7761 7665 2069 7320 312d 6174 7253  P wave is 1-atrS
+00010150: 506f 6c46 7261 6374 696f 6e0a 2020 2020  PolFraction.    
+00010160: 230a 2020 2020 2320 7273 2069 7320 7468  #.    # rs is th
+00010170: 6520 732d 7761 7665 2046 7265 736e 656c  e s-wave Fresnel
+00010180: 2061 6d70 6c69 7475 6465 0a20 2020 2023   amplitude.    #
+00010190: 2072 7020 6973 2074 6865 2070 2d77 6176   rp is the p-wav
+000101a0: 650a 0a20 2020 2023 2043 6f6e 7665 7274  e..    # Convert
+000101b0: 2074 6865 7461 2074 6f20 616e 2061 6e67   theta to an ang
+000101c0: 6c65 2069 6e20 7261 6469 616e 730a 2020  le in radians.  
+000101d0: 2020 7468 6574 6120 3d20 6d61 7468 2e72    theta = math.r
+000101e0: 6164 6961 6e73 2874 6865 7461 290a 2020  adians(theta).  
+000101f0: 2020 636f 7374 6865 7461 203d 206d 6174    costheta = mat
+00010200: 682e 636f 7328 7468 6574 6129 0a20 2020  h.cos(theta).   
+00010210: 2073 696e 7468 6574 6120 3d20 6d61 7468   sintheta = math
+00010220: 2e73 696e 2874 6865 7461 290a 2020 2020  .sin(theta).    
+00010230: 2320 4361 6c63 756c 6174 6520 7468 6520  # Calculate the 
+00010240: 4672 6573 6e65 6c20 616d 706c 6974 7564  Fresnel amplitud
+00010250: 6573 2066 6f72 2072 6566 6c65 6374 696f  es for reflectio
+00010260: 6e0a 2020 2020 2320 4571 7561 7469 6f6e  n.    # Equation
+00010270: 7320 7461 6b65 6e20 6672 6f6d 2070 3336  s taken from p36
+00010280: 3820 6f66 2041 5050 4c49 4544 2053 5045  8 of APPLIED SPE
+00010290: 4354 524f 5343 4f50 5920 5245 5649 4557  CTROSCOPY REVIEW
+000102a0: 530a 2020 2020 2320 566f 6c2e 2033 392c  S.    # Vol. 39,
+000102b0: 204e 6f2e 2033 2c20 7070 2e20 3336 35e2   No. 3, pp. 365.
+000102c0: 8093 3338 342c 2032 3030 340a 2020 2020  ..384, 2004.    
+000102d0: 2320 6279 204d 696c 616e 204d 696c 6f73  # by Milan Milos
+000102e0: 6576 6963 0a20 2020 2023 2044 4f49 3a20  evic.    # DOI: 
+000102f0: 3130 2e31 3038 312f 4153 522d 3230 3030  10.1081/ASR-2000
+00010300: 3330 3139 350a 2020 2020 7273 203d 202d  30195.    rs = -
+00010310: 312e 302a 2028 6e30 2a63 6f73 7468 6574  1.0* (n0*costhet
+00010320: 6120 2d20 636d 6174 682e 7371 7274 286e  a - cmath.sqrt(n
+00010330: 732a 6e73 202d 206e 302a 6e30 2a73 696e  s*ns - n0*n0*sin
+00010340: 7468 6574 612a 7369 6e74 6865 7461 2929  theta*sintheta))
+00010350: 202f 2028 6e30 2a63 6f73 7468 6574 6120   / (n0*costheta 
+00010360: 2b20 636d 6174 682e 7371 7274 286e 732a  + cmath.sqrt(ns*
+00010370: 6e73 202d 206e 302a 6e30 2a73 696e 7468  ns - n0*n0*sinth
+00010380: 6574 612a 7369 6e74 6865 7461 2929 0a20  eta*sintheta)). 
+00010390: 2020 2072 7020 3d20 286e 732a 6e73 2f6e     rp = (ns*ns/n
+000103a0: 302a 636f 7374 6865 7461 202d 2063 6d61  0*costheta - cma
+000103b0: 7468 2e73 7172 7428 6e73 2a6e 7320 2d20  th.sqrt(ns*ns - 
+000103c0: 6e30 2a6e 302a 7369 6e74 6865 7461 2a73  n0*n0*sintheta*s
+000103d0: 696e 7468 6574 6129 2920 2f20 286e 732a  intheta)) / (ns*
+000103e0: 6e73 2f6e 302a 636f 7374 6865 7461 202b  ns/n0*costheta +
+000103f0: 2063 6d61 7468 2e73 7172 7428 6e73 2a6e   cmath.sqrt(ns*n
+00010400: 7320 2d20 6e30 2a6e 302a 7369 6e74 6865  s - n0*n0*sinthe
+00010410: 7461 2a73 696e 7468 6574 6129 290a 2020  ta*sintheta)).  
+00010420: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
+00010430: 6520 7265 666c 6563 7461 6e63 6520 6672  e reflectance fr
+00010440: 6f6d 2074 6865 2061 6d70 6c69 7475 6465  om the amplitude
+00010450: 7320 2d20 7374 6f72 6520 6173 2061 2072  s - store as a r
+00010460: 6561 6c0a 2020 2020 5253 203d 206e 702e  eal.    RS = np.
+00010470: 7265 616c 2872 7320 2a20 7273 2e63 6f6e  real(rs * rs.con
+00010480: 6a75 6761 7465 2829 290a 2020 2020 5250  jugate()).    RP
+00010490: 203d 206e 702e 7265 616c 2872 7020 2a20   = np.real(rp * 
+000104a0: 7270 2e63 6f6e 6a75 6761 7465 2829 290a  rp.conjugate()).
+000104b0: 2020 2020 5253 5020 3d20 6174 7253 506f      RSP = atrSPo
+000104c0: 6c46 7261 6374 696f 6e2a 5253 202b 2028  lFraction*RS + (
+000104d0: 312e 302d 6174 7253 506f 6c46 7261 6374  1.0-atrSPolFract
+000104e0: 696f 6e29 2a52 500a 2020 2020 2320 4e6f  ion)*RP.    # No
+000104f0: 7720 7265 7475 726e 2074 6865 2065 7874  w return the ext
+00010500: 696e 6374 696f 6e0a 2020 2020 5253 5020  inction.    RSP 
+00010510: 3d20 2d6d 6174 682e 6c6f 6731 3028 5253  = -math.log10(RS
+00010520: 5029 0a20 2020 2072 6574 7572 6e20 5253  P).    return RS
+00010530: 500a 0a64 6566 2073 6f6c 7665 5f73 696e  P..def solve_sin
+00010540: 676c 655f 6372 7973 7461 6c5f 6571 7561  gle_crystal_equa
+00010550: 7469 6f6e 7328 200a 2020 2020 2020 2020  tions( .        
+00010560: 7375 7065 7273 7472 6174 6544 6965 6c65  superstrateDiele
+00010570: 6374 7269 6346 756e 6374 696f 6e20 2c0a  ctricFunction ,.
+00010580: 2020 2020 2020 2020 7375 6273 7472 6174          substrat
+00010590: 6544 6965 6c65 6374 7269 6346 756e 6374  eDielectricFunct
+000105a0: 696f 6e20 2020 2c0a 2020 2020 2020 2020  ion   ,.        
+000105b0: 6372 7973 7461 6c50 6572 6d69 7474 6976  crystalPermittiv
+000105c0: 6974 7946 756e 6374 696f 6e20 2020 2c0a  ityFunction   ,.
+000105d0: 2020 2020 2020 2020 7375 7065 7273 7472          superstr
+000105e0: 6174 6544 6570 7468 2020 2020 2020 2020  ateDepth        
+000105f0: 2020 2020 2020 2c0a 2020 2020 2020 2020        ,.        
+00010600: 7375 6273 7472 6174 6544 6570 7468 2020  substrateDepth  
+00010610: 2020 2020 2020 2020 2020 2020 2020 2c0a                ,.
+00010620: 2020 2020 2020 2020 6372 7973 7461 6c44          crystalD
+00010630: 6570 7468 2020 2020 2020 2020 2020 2020  epth            
+00010640: 2020 2020 2020 2c0a 2020 2020 2020 2020        ,.        
+00010650: 6d6f 6465 2020 2020 2020 2020 2020 2020  mode            
+00010660: 2020 2020 2020 2020 2020 2020 2020 2c0a                ,.
+00010670: 2020 2020 2020 2020 7468 6574 6120 2020          theta   
+00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010690: 2020 2020 2020 2c0a 2020 2020 2020 2020        ,.        
+000106a0: 7068 6920 2020 2020 2020 2020 2020 2020  phi             
+000106b0: 2020 2020 2020 2020 2020 2020 2020 2c0a                ,.
+000106c0: 2020 2020 2020 2020 7073 6920 2020 2020          psi     
+000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106e0: 2020 2020 2020 2c0a 2020 2020 2020 2020        ,.        
+000106f0: 616e 676c 654f 6649 6e63 6964 656e 6365  angleOfIncidence
+00010700: 2020 2020 2020 2020 2020 2020 2020 2c0a                ,.
+00010710: 2020 2020 2020 2020 7620 293a 0a20 2020          v ):.   
+00010720: 2022 2222 2054 6869 7320 6973 2061 2070   """ This is a p
+00010730: 6172 616c 6c65 6c20 6361 6c6c 2074 6f20  arallel call to 
+00010740: 7468 6520 7369 6e67 6c65 2063 7279 7374  the single cryst
+00010750: 616c 2065 7175 6174 696f 6e20 736f 6c76  al equation solv
+00010760: 6572 2c0a 2020 2020 7379 7374 656d 2069  er,.    system i
+00010770: 7320 6120 4754 4d20 7379 7374 656d 2222  s a GTM system""
+00010780: 220a 2020 2020 2320 4372 6561 7465 2033  ".    # Create 3
+00010790: 206c 6179 6572 732c 2074 6869 636b 6e65   layers, thickne
+000107a0: 7373 2069 7320 636f 6e76 6572 7465 6420  ss is converted 
+000107b0: 6672 6f6d 206d 6963 726f 6e73 2074 6f20  from microns to 
+000107c0: 6d65 7472 6573 0a20 2020 2073 7570 6572  metres.    super
+000107d0: 7374 7261 7465 2020 2020 2020 3d20 4754  strate      = GT
+000107e0: 4d2e 4c61 7965 7228 7468 6963 6b6e 6573  M.Layer(thicknes
+000107f0: 733d 7375 7065 7273 7472 6174 6544 6570  s=superstrateDep
+00010800: 7468 2a31 652d 362c 6570 7369 6c6f 6e31  th*1e-6,epsilon1
+00010810: 3d73 7570 6572 7374 7261 7465 4469 656c  =superstrateDiel
+00010820: 6563 7472 6963 4675 6e63 7469 6f6e 290a  ectricFunction).
+00010830: 2020 2020 7375 6273 7472 6174 6520 2020      substrate   
+00010840: 2020 2020 203d 2047 544d 2e4c 6179 6572       = GTM.Layer
+00010850: 2874 6869 636b 6e65 7373 3d73 7562 7374  (thickness=subst
+00010860: 7261 7465 4465 7074 682a 3165 2d36 2c20  rateDepth*1e-6, 
+00010870: 2065 7073 696c 6f6e 313d 7375 6273 7472   epsilon1=substr
+00010880: 6174 6544 6965 6c65 6374 7269 6346 756e  ateDielectricFun
+00010890: 6374 696f 6e29 0a20 2020 2063 7279 7374  ction).    cryst
+000108a0: 616c 2020 2020 2020 2020 2020 3d20 4754  al          = GT
+000108b0: 4d2e 4c61 7965 7228 7468 6963 6b6e 6573  M.Layer(thicknes
+000108c0: 733d 6372 7973 7461 6c44 6570 7468 2a31  s=crystalDepth*1
+000108d0: 652d 392c 2020 2020 6570 7369 6c6f 6e3d  e-9,    epsilon=
+000108e0: 6372 7973 7461 6c50 6572 6d69 7474 6976  crystalPermittiv
+000108f0: 6974 7946 756e 6374 696f 6e29 0a20 2020  ityFunction).   
+00010900: 2023 2043 7265 6174 2074 6865 2073 7973   # Creat the sys
+00010910: 7465 6d20 7769 7468 2074 6865 206c 6179  tem with the lay
+00010920: 6572 7320 0a20 2020 2069 6620 6d6f 6465  ers .    if mode
+00010930: 203d 3d20 2754 6869 636b 2073 6c61 6227   == 'Thick slab'
+00010940: 3a0a 2020 2020 2020 2020 7379 7374 656d  :.        system
+00010950: 203d 2047 544d 2e53 7973 7465 6d28 7375   = GTM.System(su
+00010960: 6273 7472 6174 653d 6372 7973 7461 6c2c  bstrate=crystal,
+00010970: 2073 7570 6572 7374 7261 7465 3d73 7570   superstrate=sup
+00010980: 6572 7374 7261 7465 2c20 6c61 7965 7273  erstrate, layers
+00010990: 3d5b 5d29 0a20 2020 2065 6c69 6620 6d6f  =[]).    elif mo
+000109a0: 6465 203d 3d20 2743 6f68 6572 656e 7420  de == 'Coherent 
+000109b0: 7468 696e 2066 696c 6d27 3a0a 2020 2020  thin film':.    
+000109c0: 2020 2020 7379 7374 656d 203d 2047 544d      system = GTM
+000109d0: 2e53 7973 7465 6d28 7375 6273 7472 6174  .System(substrat
+000109e0: 653d 7375 6273 7472 6174 652c 2073 7570  e=substrate, sup
+000109f0: 6572 7374 7261 7465 3d73 7570 6572 7374  erstrate=superst
+00010a00: 7261 7465 2c20 6c61 7965 7273 3d5b 6372  rate, layers=[cr
+00010a10: 7973 7461 6c5d 290a 2020 2020 656c 7365  ystal]).    else
+00010a20: 3a0a 2020 2020 2020 2020 7379 7374 656d  :.        system
+00010a30: 203d 2047 544d 2e53 7973 7465 6d28 7375   = GTM.System(su
+00010a40: 6273 7472 6174 653d 7375 6273 7472 6174  bstrate=substrat
+00010a50: 652c 2073 7570 6572 7374 7261 7465 3d73  e, superstrate=s
+00010a60: 7570 6572 7374 7261 7465 2c20 6c61 7965  uperstrate, laye
+00010a70: 7273 3d5b 6372 7973 7461 6c5d 290a 2020  rs=[crystal]).  
+00010a80: 2020 2320 526f 7461 7465 2074 6865 2064    # Rotate the d
+00010a90: 6965 6c65 6374 7269 6320 636f 6e73 7461  ielectric consta
+00010aa0: 6e74 7320 746f 2074 6865 206c 6162 6f72  nts to the labor
+00010ab0: 6174 6f72 7920 6672 616d 650a 2020 2020  atory frame.    
+00010ac0: 7379 7374 656d 2e73 7562 7374 7261 7465  system.substrate
+00010ad0: 2e73 6574 5f65 756c 6572 2874 6865 7461  .set_euler(theta
+00010ae0: 2c20 7068 692c 2070 7369 290a 2020 2020  , phi, psi).    
+00010af0: 7379 7374 656d 2e73 7570 6572 7374 7261  system.superstra
+00010b00: 7465 2e73 6574 5f65 756c 6572 2874 6865  te.set_euler(the
+00010b10: 7461 2c20 7068 692c 2070 7369 290a 2020  ta, phi, psi).  
+00010b20: 2020 666f 7220 6c61 7965 7220 696e 2073    for layer in s
+00010b30: 7973 7465 6d2e 6c61 7965 7273 3a0a 2020  ystem.layers:.  
+00010b40: 2020 2020 2020 6c61 7965 722e 7365 745f        layer.set_
+00010b50: 6575 6c65 7228 7468 6574 612c 2070 6869  euler(theta, phi
+00010b60: 2c20 7073 6929 0a20 2020 2023 200a 2020  , psi).    # .  
+00010b70: 2020 2320 636f 6e76 6572 7420 636d 2d31    # convert cm-1
+00010b80: 2074 6f20 6672 6571 7565 6e63 790a 2020   to frequency.  
+00010b90: 2020 230a 2020 2020 6672 6571 203d 2076    #.    freq = v
+00010ba0: 202a 2073 7065 6564 5f6c 6967 6874 5f73   * speed_light_s
+00010bb0: 6920 2a20 3165 320a 2020 2020 7379 7374  i * 1e2.    syst
+00010bc0: 656d 2e69 6e69 7469 616c 697a 655f 7379  em.initialize_sy
+00010bd0: 7328 6672 6571 290a 2020 2020 7a65 7461  s(freq).    zeta
+00010be0: 5f73 7973 203d 206e 702e 7369 6e28 616e  _sys = np.sin(an
+00010bf0: 676c 654f 6649 6e63 6964 656e 6365 292a  gleOfIncidence)*
+00010c00: 6e70 2e73 7172 7428 7379 7374 656d 2e73  np.sqrt(system.s
+00010c10: 7570 6572 7374 7261 7465 2e65 7073 696c  uperstrate.epsil
+00010c20: 6f6e 5b30 2c30 5d29 0a20 2020 2053 7973  on[0,0]).    Sys
+00010c30: 5f47 616d 6d61 203d 2073 7973 7465 6d2e  _Gamma = system.
+00010c40: 6361 6c63 756c 6174 655f 4761 6d6d 6153  calculate_GammaS
+00010c50: 7461 7228 6672 6571 2c20 7a65 7461 5f73  tar(freq, zeta_s
+00010c60: 7973 290a 2020 2020 722c 2052 2c20 742c  ys).    r, R, t,
+00010c70: 2054 203d 2073 7973 7465 6d2e 6361 6c63   T = system.calc
+00010c80: 756c 6174 655f 725f 7428 7a65 7461 5f73  ulate_r_t(zeta_s
+00010c90: 7973 290a 2020 2020 6966 206c 656e 2873  ys).    if len(s
+00010ca0: 7973 7465 6d2e 6c61 7965 7273 2920 3e20  ystem.layers) > 
+00010cb0: 303a 0a20 2020 2020 2020 2065 7073 696c  0:.        epsil
+00010cc0: 6f6e 203d 2073 7973 7465 6d2e 6c61 7965  on = system.laye
+00010cd0: 7273 5b30 5d2e 6570 7369 6c6f 6e0a 2020  rs[0].epsilon.  
+00010ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010cf0: 6570 7369 6c6f 6e20 3d20 7379 7374 656d  epsilon = system
+00010d00: 2e73 7562 7374 7261 7465 2e65 7073 696c  .substrate.epsil
+00010d10: 6f6e 0a20 2020 2072 6574 7572 6e20 762c  on.    return v,
+00010d20: 722c 522c 742c 542c 6570 7369 6c6f 6e0a  r,R,t,T,epsilon.
+00010d30: 0a0a 6465 6620 636c 6561 6e75 705f 7379  ..def cleanup_sy
+00010d40: 6d62 6f6c 2873 293a 0a20 2020 2022 2222  mbol(s):.    """
+00010d50: 5265 7475 726e 2061 2074 7275 6520 656c  Return a true el
+00010d60: 656d 656e 7420 6672 6f6d 2074 6865 2073  ement from the s
+00010d70: 796d 626f 6c22 2222 0a20 2020 2073 203d  ymbol""".    s =
+00010d80: 2073 2e63 6170 6974 616c 697a 6528 290a   s.capitalize().
+00010d90: 2020 2020 7320 3d20 732e 7265 706c 6163      s = s.replac
+00010da0: 6528 275f 272c 2727 290a 2020 2020 666f  e('_','').    fo
+00010db0: 7220 6920 696e 2073 7472 696e 672e 6469  r i in string.di
+00010dc0: 6769 7473 3a0a 2020 2020 2020 2020 7320  gits:.        s 
+00010dd0: 3d20 732e 7265 706c 6163 6528 692c 2727  = s.replace(i,''
+00010de0: 290a 2020 2020 7265 7475 726e 2073 0a0a  ).    return s..
+00010df0: 6465 6620 6575 6c65 725f 726f 7461 7469  def euler_rotati
+00010e00: 6f6e 2876 6563 746f 722c 2074 6865 7461  on(vector, theta
+00010e10: 2c20 7068 692c 2070 7369 293a 0a20 2020  , phi, psi):.   
+00010e20: 2020 2222 2241 7070 6c79 2061 2070 6173    """Apply a pas
+00010e30: 7369 7665 2045 756c 6572 2072 6f74 6174  sive Euler rotat
+00010e40: 696f 6e20 746f 2074 6865 2076 6563 746f  ion to the vecto
+00010e50: 7222 2222 0a20 2020 2020 6575 6c65 7220  r""".     euler 
+00010e60: 3d20 6e70 2e7a 6572 6f73 2820 2833 2c33  = np.zeros( (3,3
+00010e70: 2920 290a 2020 2020 2065 756c 6572 5b30  ) ).     euler[0
+00010e80: 2c20 305d 203d 2020 6e70 2e63 6f73 2870  , 0] =  np.cos(p
+00010e90: 7369 2920 2a20 6e70 2e63 6f73 2870 6869  si) * np.cos(phi
+00010ea0: 2920 2d20 6e70 2e63 6f73 2874 6865 7461  ) - np.cos(theta
+00010eb0: 2920 2a20 6e70 2e73 696e 2870 6869 2920  ) * np.sin(phi) 
+00010ec0: 2a20 6e70 2e73 696e 2870 7369 290a 2020  * np.sin(psi).  
+00010ed0: 2020 2065 756c 6572 5b30 2c20 315d 203d     euler[0, 1] =
+00010ee0: 202d 6e70 2e73 696e 2870 7369 2920 2a20   -np.sin(psi) * 
+00010ef0: 6e70 2e63 6f73 2870 6869 2920 2d20 6e70  np.cos(phi) - np
+00010f00: 2e63 6f73 2874 6865 7461 2920 2a20 6e70  .cos(theta) * np
+00010f10: 2e73 696e 2870 6869 2920 2a20 6e70 2e63  .sin(phi) * np.c
+00010f20: 6f73 2870 7369 290a 2020 2020 2065 756c  os(psi).     eul
+00010f30: 6572 5b30 2c20 325d 203d 2020 6e70 2e73  er[0, 2] =  np.s
+00010f40: 696e 2874 6865 7461 2920 2a20 6e70 2e73  in(theta) * np.s
+00010f50: 696e 2870 6869 290a 2020 2020 2065 756c  in(phi).     eul
+00010f60: 6572 5b31 2c20 305d 203d 2020 6e70 2e63  er[1, 0] =  np.c
+00010f70: 6f73 2870 7369 2920 2a20 6e70 2e73 696e  os(psi) * np.sin
+00010f80: 2870 6869 2920 2b20 6e70 2e63 6f73 2874  (phi) + np.cos(t
+00010f90: 6865 7461 2920 2a20 6e70 2e63 6f73 2870  heta) * np.cos(p
+00010fa0: 6869 2920 2a20 6e70 2e73 696e 2870 7369  hi) * np.sin(psi
+00010fb0: 290a 2020 2020 2065 756c 6572 5b31 2c20  ).     euler[1, 
+00010fc0: 315d 203d 202d 6e70 2e73 696e 2870 7369  1] = -np.sin(psi
+00010fd0: 2920 2a20 6e70 2e73 696e 2870 6869 2920  ) * np.sin(phi) 
+00010fe0: 2b20 6e70 2e63 6f73 2874 6865 7461 2920  + np.cos(theta) 
+00010ff0: 2a20 6e70 2e63 6f73 2870 6869 2920 2a20  * np.cos(phi) * 
+00011000: 6e70 2e63 6f73 2870 7369 290a 2020 2020  np.cos(psi).    
+00011010: 2065 756c 6572 5b31 2c20 325d 203d 202d   euler[1, 2] = -
+00011020: 6e70 2e73 696e 2874 6865 7461 2920 2a20  np.sin(theta) * 
+00011030: 6e70 2e63 6f73 2870 6869 290a 2020 2020  np.cos(phi).    
+00011040: 2065 756c 6572 5b32 2c20 305d 203d 2020   euler[2, 0] =  
+00011050: 6e70 2e73 696e 2874 6865 7461 2920 2a20  np.sin(theta) * 
+00011060: 6e70 2e73 696e 2870 7369 290a 2020 2020  np.sin(psi).    
+00011070: 2065 756c 6572 5b32 2c20 315d 203d 2020   euler[2, 1] =  
+00011080: 6e70 2e73 696e 2874 6865 7461 2920 2a20  np.sin(theta) * 
+00011090: 6e70 2e63 6f73 2870 7369 290a 2020 2020  np.cos(psi).    
+000110a0: 2065 756c 6572 5b32 2c20 325d 203d 2020   euler[2, 2] =  
+000110b0: 6e70 2e63 6f73 2874 6865 7461 290a 2020  np.cos(theta).  
+000110c0: 2020 2072 6573 756c 7420 3d20 6e70 2e6d     result = np.m
+000110d0: 6174 6d75 6c28 6575 6c65 722c 2076 6563  atmul(euler, vec
+000110e0: 746f 7229 0a20 2020 2020 7265 7475 726e  tor).     return
+000110f0: 2072 6573 756c 740a 0a64 6566 2067 6574   result..def get
+00011100: 5f70 6f6f 6c28 6e63 7075 732c 2074 6872  _pool(ncpus, thr
+00011110: 6561 6469 6e67 2c20 696e 6974 6961 6c69  eading, initiali
+00011120: 7a65 723d 4e6f 6e65 2c20 696e 6974 6172  zer=None, initar
+00011130: 6773 3d4e 6f6e 652c 2064 6562 7567 6765  gs=None, debugge
+00011140: 723d 4e6f 6e65 2029 3a0a 2020 2020 2022  r=None ):.     "
+00011150: 2222 5265 7475 726e 2061 2070 6f6f 6c20  ""Return a pool 
+00011160: 6f66 2070 726f 6365 7373 6f72 7320 6769  of processors gi
+00011170: 7665 6e20 7468 6520 6e75 6d62 6572 206f  ven the number o
+00011180: 6620 6370 7573 2061 6e64 2077 6865 7468  f cpus and wheth
+00011190: 6572 2074 6872 6561 6469 6e67 2069 7320  er threading is 
+000111a0: 7265 7175 6573 7465 6422 2222 0a20 2020  requested""".   
+000111b0: 2020 6966 2064 6562 7567 6765 7220 6973    if debugger is
+000111c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000111d0: 2020 2020 6465 6275 6767 6572 2e70 7269      debugger.pri
+000111e0: 6e74 2827 6765 745f 706f 6f6c 206e 6370  nt('get_pool ncp
+000111f0: 7573 203d 2027 2c6e 6370 7573 290a 2020  us = ',ncpus).  
+00011200: 2020 2020 2020 2064 6562 7567 6765 722e         debugger.
+00011210: 7072 696e 7428 2767 6574 5f70 6f6f 6c20  print('get_pool 
+00011220: 7468 7265 6164 696e 6720 3d20 272c 7468  threading = ',th
+00011230: 7265 6164 696e 6729 0a20 2020 2020 2020  reading).       
+00011240: 2020 6465 6275 6767 6572 2e70 7269 6e74    debugger.print
+00011250: 2827 6765 745f 706f 6f6c 2069 6e69 7469  ('get_pool initi
+00011260: 616c 697a 6572 203d 2027 2c69 6e69 7469  alizer = ',initi
+00011270: 616c 697a 6572 290a 2020 2020 2023 2053  alizer).     # S
+00011280: 7769 7463 6820 6f66 6620 6d6b 6c20 7468  witch off mkl th
+00011290: 7265 6164 696e 670a 2020 2020 2074 7279  reading.     try
+000112a0: 3a0a 2020 2020 2020 2020 2069 6d70 6f72  :.         impor
+000112b0: 7420 6d6b 6c0a 2020 2020 2020 2020 206d  t mkl.         m
+000112c0: 6b6c 2e73 6574 5f6e 756d 5f74 6872 6561  kl.set_num_threa
+000112d0: 6473 2831 290a 2020 2020 2065 7863 6570  ds(1).     excep
+000112e0: 743a 0a20 2020 2020 2020 2020 7061 7373  t:.         pass
+000112f0: 0a20 2020 2020 2320 7365 6520 6966 2074  .     # see if t
+00011300: 6872 6561 6469 6e67 2068 6173 2062 6565  hreading has bee
+00011310: 6e20 7265 7175 6573 7465 640a 2020 2020  n requested.    
+00011320: 2069 6620 7468 7265 6164 696e 673a 0a20   if threading:. 
+00011330: 2020 2020 2020 2020 6672 6f6d 206d 756c          from mul
+00011340: 7469 7072 6f63 6573 7369 6e67 2e64 756d  tiprocessing.dum
+00011350: 6d79 2069 6d70 6f72 7420 506f 6f6c 0a20  my import Pool. 
+00011360: 2020 2020 2020 2020 706f 6f6c 203d 2050          pool = P
+00011370: 6f6f 6c28 6e63 7075 732c 2069 6e69 7469  ool(ncpus, initi
+00011380: 616c 697a 6572 3d69 6e69 7469 616c 697a  alizer=initializ
+00011390: 6572 2c20 696e 6974 6172 6773 3d69 6e69  er, initargs=ini
+000113a0: 7461 7267 7329 0a20 2020 2020 656c 7365  targs).     else
+000113b0: 3a0a 2020 2020 2020 2020 2066 726f 6d20  :.         from 
+000113c0: 6d75 6c74 6970 726f 6365 7373 696e 6720  multiprocessing 
+000113d0: 696d 706f 7274 2050 6f6f 6c0a 2020 2020  import Pool.    
+000113e0: 2020 2020 2070 6f6f 6c20 3d20 506f 6f6c       pool = Pool
+000113f0: 286e 6370 7573 2c20 696e 6974 6961 6c69  (ncpus, initiali
+00011400: 7a65 723d 696e 6974 6961 6c69 7a65 722c  zer=initializer,
+00011410: 2069 6e69 7461 7267 733d 696e 6974 6172   initargs=initar
+00011420: 6773 2029 0a20 2020 2020 7265 7475 726e  gs ).     return
+00011430: 2070 6f6f 6c0a 0a64 6566 2073 6574 5f61   pool..def set_a
+00011440: 6666 696e 6974 795f 6f6e 5f77 6f72 6b65  ffinity_on_worke
+00011450: 7228 293a 0a20 2020 2027 2727 5768 656e  r():.    '''When
+00011460: 2061 206e 6577 2077 6f72 6b65 7220 7072   a new worker pr
+00011470: 6f63 6573 7320 6973 2063 7265 6174 6564  ocess is created
+00011480: 2c20 7468 6520 6166 6669 6e69 7479 2069  , the affinity i
+00011490: 7320 7365 7420 746f 2061 6c6c 2043 5055  s set to all CPU
+000114a0: 7327 2727 0a20 2020 2023 4a4b 2070 7269  s'''.    #JK pri
+000114b0: 6e74 2827 4927 6d20 7468 6520 7072 6f63  nt('I'm the proc
+000114c0: 6573 7320 2564 2c20 7365 7474 696e 6720  ess %d, setting 
+000114d0: 6166 6669 6e69 7479 2074 6f20 616c 6c20  affinity to all 
+000114e0: 4350 5573 2e27 2025 206f 732e 6765 7470  CPUs.' % os.getp
+000114f0: 6964 2829 290a 2020 2020 234a 4b20 436f  id()).    #JK Co
+00011500: 6d6d 656e 7465 6420 6f75 7420 666f 7220  mmented out for 
+00011510: 7468 6520 7469 6d65 2062 6569 6e67 0a20  the time being. 
+00011520: 2020 2023 4a4b 206f 732e 7379 7374 656d     #JK os.system
+00011530: 2827 7461 736b 7365 7420 2d70 2030 7866  ('taskset -p 0xf
+00011540: 6620 2564 203e 202f 6465 762f 6e75 6c6c  f %d > /dev/null
+00011550: 2720 2520 6f73 2e67 6574 7069 6428 2929  ' % os.getpid())
+00011560: 0a20 2020 2072 6574 7572 6e0a 0a0a       .    return...
```

### Comparing `PDielec-7.1.2/PDielec/CastepOutputReader.py` & `PDielec-7.2.1/PDielec/CastepOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/Constants.py` & `PDielec-7.2.1/PDielec/Constants.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/CrystalOutputReader.py` & `PDielec-7.2.1/PDielec/CrystalOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/DielectricFunction.py` & `PDielec-7.2.1/PDielec/DielectricFunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,46 +282,46 @@
         """
         Setup a Drude-Lorentz model for a diagonal permittivity 
         """
         eps = np.zeros( (3,3), dtype=complex )
         for xyz,contribution in enumerate(self.parameters):
             for mode in contribution:
                 v_cm1, strength_cm1, sigma_cm1 = mode
-                eps[xyz,xyz] += strength_cm1 * strength_cm1 / np.complex((v_cm1*v_cm1 - f_cm1*f_cm1), -sigma_cm1*f_cm1)
+                eps[xyz,xyz] += strength_cm1 * strength_cm1 / complex((v_cm1*v_cm1 - f_cm1*f_cm1), -sigma_cm1*f_cm1)
         return eps + self.epsilon_infinity
 
     def _epsFromFpsq(self, f_cm1):
         """
         Setup a fpsq model for the permittivity
         """
         #jk print('Setting up fpsq ',self.parameters)
         eps = np.array(self.epsilon_infinity,dtype=complex)
         for xyz,contribution in enumerate(self.parameters):
             for omega_to, gamma_to, omega_lo, gamma_lo  in contribution:
-                contribution = (omega_lo**2 - f_cm1**2 - np.complex(0,gamma_lo)*f_cm1)/(omega_to**2 - f_cm1**2 - np.complex(0,gamma_to)*f_cm1)
+                contribution = (omega_lo**2 - f_cm1**2 - complex(0,gamma_lo)*f_cm1)/(omega_to**2 - f_cm1**2 - complex(0,gamma_to)*f_cm1)
                 # make sure the imaginary component is not negative!
                 real_contribution = np.real(contribution)
                 imag_contribution = max(-1.0E-12,np.imag(contribution))
-                eps[xyz,xyz] *= np.complex(real_contribution,imag_contribution)
+                eps[xyz,xyz] *= complex(real_contribution,imag_contribution)
         return eps 
 
 
     def dielectriContributionsFromDrude(self, f, frequency, sigma, volume):
         """Calculate the dielectric function for a set of a Drude oscillator
         f is the frequency of the dielectric response in au
         frequency(au), sigmas(au) are the plasma frequency and the width
         The output from this calculation is a complex dielectric tensor
         """
-        dielectric = np.zeros((3, 3), dtype=np.complex)
-        unit = identity(3,dtype=np.complex)
+        dielectric = np.zeros((3, 3), dtype=complex)
+        unit = identity(3,dtype=complex)
         # Avoid a divide by zero if f is small
         if f <= 1.0e-8:
             f = 1.0e-8
         # Assume that the drude contribution is isotropic
-        dielectric = dielectric - unit * frequency*frequency / np.complex(-f*f, -sigma*f)
+        dielectric = dielectric - unit * frequency*frequency / complex(-f*f, -sigma*f)
         return dielectric * (4.0*np.pi/volume)
 
 
     def dielectriContributionsFromModes(self, f, modes, frequencies, sigmas, strengths, volume):
         """Calculate the dielectric function for a set of modes with their own widths and strengths
            f is the frequency of the dielectric response in au
            modes are a list of the modes
@@ -329,11 +329,11 @@
            The output from this calculation is a complex dielectric tensor
         """
         dielectric = np.zeros((3, 3), dtype=complex)
         for mode in modes:
             v = frequencies[mode]
             sigma = sigmas[mode]
             strength = strengths[mode].astype(complex)
-            dielectric = dielectric + strength / np.complex((v*v - f*f), -sigma*f)
+            dielectric = dielectric + strength / complex((v*v - f*f), -sigma*f)
         return dielectric * (4.0*np.pi/volume)
```

### Comparing `PDielec-7.1.2/PDielec/ExperimentOutputReader.py` & `PDielec-7.2.1/PDielec/ExperimentOutputReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,19 +400,19 @@
             self.frequencies = np.zeros( (3*self.nions) )
         return
 
     def _read_static_dielectric(self, line):
         # the is epsilon infinity
         od = []
         line = self._read_line()
-        od.append([np.complex(f) for f in line.split()[0:3]])
+        od.append([complex(f) for f in line.split()[0:3]])
         line = self._read_line()
-        od.append([np.complex(f) for f in line.split()[0:3]])
+        od.append([complex(f) for f in line.split()[0:3]])
         line = self._read_line()
-        od.append([np.complex(f) for f in line.split()[0:3]])
+        od.append([complex(f) for f in line.split()[0:3]])
         # If we have complex input return a complex list, otherwise return a real list
         odc = np.array(od,dtype=complex)
         odi = np.absolute(np.imag(odc))
         sumi = np.sum(odi)
         if sumi < 1.0e-12:
             odc = np.real(odc)
         self.zerof_optical_dielectric = odc.tolist()
```

### Comparing `PDielec-7.1.2/PDielec/GTMcore.py` & `PDielec-7.2.1/PDielec/GTMcore.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/AnalysisTab.py` & `PDielec-7.2.1/PDielec/GUI/AnalysisTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/App.py` & `PDielec-7.2.1/PDielec/GUI/App.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,20 @@
         # chdir to the directory that the script is in
         if directory != '':
             os.chdir(directory)
         scriptname = os.path.basename(scriptname)
         # If a script is used there are no prompts for overwriting files etc.
         self.notebook.overwriting = True
         with open(scriptname,'r') as fd:
-            exec(fd.read())
+            lines = fd.readlines()
+            line_no = 0
+            for line in lines:
+                line_no += 1
+                debugger.print('line: ',line_no,line)
+                exec(line)
         debugger.print('readScript finished reading script')
         self.notebook.scripting = False
         debugger.print('readScript notebook scripting set to False')
         if not self.program_exit:
             self.notebook.overwriting = False
             debugger.print('readScript notebook overwriting set to False')
         # The command line excel file overrides that in the script
```

### Comparing `PDielec-7.1.2/PDielec/GUI/FitterTab.py` & `PDielec-7.2.1/PDielec/GUI/FitterTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/MainTab.py` & `PDielec-7.2.1/PDielec/GUI/MainTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/NoteBook.py` & `PDielec-7.2.1/PDielec/GUI/NoteBook.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,17 +152,14 @@
         else:
             # copyFromIndex is default so we find the last scenario of scenarioType in the list
             last = None
             for scenario in self.scenarios:
                 if scenarioType == scenario.scenarioType:
                     last = scenario
             # end for
-            if last is None:
-                debugger.print('Finished:: addScenario unable to add scenario')
-                return
         # Create a new scenario
         if scenarioType == 'Powder':
             self.currentScenarioTab = PowderScenarioTab
         else:
             self.currentScenarioTab = SingleCrystalScenarioTab
         # Add the scenario to the end of the list
         debugger.print('Appending the new scenario')
```

### Comparing `PDielec-7.1.2/PDielec/GUI/OpenGLWidget.py` & `PDielec-7.2.1/PDielec/GUI/OpenGLWidget.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/PlottingTab.py` & `PDielec-7.2.1/PDielec/GUI/PlottingTab.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,21 +369,23 @@
         realPermittivities          = []
         imagPermittivities          = []
         sp_atrs                     = []
         R_ps                        = []
         R_ss                        = []
         T_ps                        = []
         T_ss                        = []
+        A_ps                        = []
+        A_ss                        = []
         powder_legends              = []
         crystal_legends             = []
         # Deal with Scenarios 
         sp = self.notebook.spreadsheet
         sp.selectWorkSheet('Scenarios')
         sp.delete()
-        sp.writeNextRow(['A list of the scenarios used the calculation of the effective medium'],col=1)
+        sp.writeNextRow(['A list of the scenarios used:'],col=1)
         for index,scenario in enumerate(self.notebook.scenarios):
             if scenario.scenarioType == 'Powder':
                 direction = scenario.direction
                 depolarisation = scenario.depolarisation
                 sp.writeNextRow([''],col=1)
                 sp.writeNextRow(['Scenario '+str(index)],col=1,check=1)
                 settings = scenario.settings
@@ -411,14 +413,16 @@
                 sp.writeNextRow(scenario.labframe_b.tolist(), col=2, check=1)
                 sp.writeNextRow(scenario.labframe_c.tolist(), col=2, check=1)
                 # Store the reflectance and transmittance
                 R_ps.append( scenario.get_result(self.vs_cm1,self.plot_types[5] ) )
                 R_ss.append( scenario.get_result(self.vs_cm1,self.plot_types[6] ) )
                 T_ps.append( scenario.get_result(self.vs_cm1,self.plot_types[7] ) )
                 T_ss.append( scenario.get_result(self.vs_cm1,self.plot_types[8] ) )
+                A_ps.append( scenario.get_result(self.vs_cm1,self.plot_types[9] ) )
+                A_ss.append( scenario.get_result(self.vs_cm1,self.plot_types[10] ) )
                 crystal_legends.append(scenario.settings['Legend'])
         # Single crystal Permittivity
         dielecv = self.notebook.settingsTab.get_crystal_permittivity(self.vs_cm1)
         # Powder results
         # Work out what molar units we are using
         if len(molarAbsorptionCoefficients) > 0:
             if self.settings['Molar definition'] == 'Molecules':
@@ -443,14 +447,16 @@
             self.write_powder_results(sp, 'Powder ATR Reflectance',        self.vs_cm1, powder_legends, sp_atrs)
         # Single Crystal results
         if len(R_ps) > 0:
             self.write_crystal_results(sp, 'Crystal R_p', self.vs_cm1, crystal_legends, R_ps)
             self.write_crystal_results(sp, 'Crystal R_s', self.vs_cm1, crystal_legends, R_ss)
             self.write_crystal_results(sp, 'Crystal T_p', self.vs_cm1, crystal_legends, T_ps)
             self.write_crystal_results(sp, 'Crystal T_s', self.vs_cm1, crystal_legends, T_ss)
+            self.write_crystal_results(sp, 'Crystal A_p', self.vs_cm1, crystal_legends, A_ps)
+            self.write_crystal_results(sp, 'Crystal A_s', self.vs_cm1, crystal_legends, A_ss)
 
         if len(dielecv) > 0:
             self.write_eps_results(sp, self.vs_cm1, dielecv)
         debugger.print('Finished::writeSpreadsheet')
         return
 
     def write_eps_results(self, sp, vs, dielecv):
```

### Comparing `PDielec-7.1.2/PDielec/GUI/PowderScenarioTab.py` & `PDielec-7.2.1/PDielec/GUI/PowderScenarioTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/ScenarioTab.py` & `PDielec-7.2.1/PDielec/GUI/ScenarioTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/SettingsTab.py` & `PDielec-7.2.1/PDielec/GUI/SettingsTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/SingleCrystalScenarioTab.py` & `PDielec-7.2.1/PDielec/GUI/SingleCrystalScenarioTab.py`

 * *Files 10% similar despite different names*

```diff
@@ -378,71 +378,22 @@
         debugger.print(self.settings['Legend'],'About to extract results for single crystal scenario')
         for v,r,R,t,T,epsilon in results:
             self.vs_cm1.append(v)
             self.p_reflectance.append(R[0]+R[2])
             self.s_reflectance.append(R[1]+R[3])
             self.p_transmittance.append(T[0])
             self.s_transmittance.append(T[1])
-            self.p_absorbtance.append(R[0]+R[2]+T[0])
-            self.s_absorbtance.append(R[1]+R[3]+T[1])
+            self.p_absorbtance.append(1.0 - R[0]-R[2]-T[0])
+            self.s_absorbtance.append(1.0 - R[1]-R[3]-T[1])
             self.epsilon.append(epsilon)
         self.calculationRequired = False
         QCoreApplication.processEvents()
         debugger.print(self.settings['Legend'],'Finished:: calculate - number of frequencies',len(vs_cm1))
         return
 
-    def writeSpreadsheet(self):
-        debugger.print(self.settings['Legend'],'Start:: writeSpreadsheet')
-        if self.notebook.spreadsheet is None:
-            debugger.print(self.settings['Legend'],'Finished:: writeSpreadsheet')
-            return
-        sp = self.notebook.spreadsheet
-        sp.selectWorkSheet('Single Crystal')
-        sp.delete()
-        sp.writeNextRow(['Settings for the single crystal calculation of absorption and reflection'],col=1)
-        sp.writeNextRow([''],col=1)
-        sp.writeNextRow([ 'Single crystal mode',          self.settings['Mode'] ],col=1)
-        sp.writeNextRow([ 'Minimum frequency',            self.settings['Minimum frequency'] ],col=1)
-        sp.writeNextRow([ 'Maximum frequency',            self.settings['Maximum frequency'] ],col=1)
-        sp.writeNextRow([ 'Frequency increment',          self.settings['Frequency increment'] ],col=1)
-        sp.writeNextRow([ 'Surface definition (h)',       self.settings['Unique direction - h'] ],col=1)
-        sp.writeNextRow([ 'Surface definition (k)',       self.settings['Unique direction - k'] ],col=1)
-        sp.writeNextRow([ 'Surface definition (l)',       self.settings['Unique direction - l'] ],col=1)
-        sp.writeNextRow([ 'Azimuthal angle',              self.settings['Azimuthal angle'] ],col=1)
-        sp.writeNextRow([ 'Angle of incidence',           self.settings['Angle of incidence'] ],col=1)
-        sp.writeNextRow([ 'Superstrate dielectric',       self.settings['Superstrate dielectric'] ],col=1)
-        sp.writeNextRow([ 'Substrate dielectric',         self.settings['Substrate dielectric'] ],col=1)
-        sp.writeNextRow([ 'Film thickness(nm)',           self.settings['Film thickness'] ],col=1)
-        headings = ['R_p', 'R_s', 'T_p', 'T_s']
-        self.write_results(sp, 'Crystal R&T',     self.vs_cm1, [self.p_reflectance, self.s_reflectance, self.p_transmittance, self.s_transmittance], headings)
-        debugger.print(self.settings['Legend'],'Finished:: writeSpreadsheet')
-        return
-
-    def write_results(self, sp, name, vs, yss, headings):
-        """ 
-        sp        is the spreadsheet object
-        name      is the worksheet name used for writing
-        vs        an np.array of the frequencies
-        yss       a list of np.arrays of the reflections and transmittance ] 
-        headings  the heading names for the yss
-        """
-        debugger.print(self.settings['Legend'],'Start:: write_results')
-        sp.selectWorkSheet(name)
-        sp.delete()
-        headers = ['frequencies (cm-1)']
-        headers.extend(headings)
-        sp.writeNextRow(headers,row=0, col=1)
-        for iv,v in enumerate(vs):
-           output = [v]
-           for ys in yss:
-               output.append(ys[iv])
-           sp.writeNextRow(output, col=1,check=1)
-        debugger.print(self.settings['Legend'],'Finished:: write_results')
-        return
-
     def calculate_euler_angles(self):
         '''Calculate the Euler angles for the crystal to lab transformation'''
         debugger.print(self.settings['Legend'],'Start:: calculate_euler_angles')
         # Get plane specification
         hkl = [ self.settings['Unique direction - h'] , self.settings['Unique direction - k'], self.settings['Unique direction - l'] ]
         sum2 = hkl[0]*hkl[0] + hkl[1]*hkl[1] + hkl[2]*hkl[2]
         if sum2 < 1:
```

### Comparing `PDielec-7.1.2/PDielec/GUI/SpreadSheetManager.py` & `PDielec-7.2.1/PDielec/GUI/SpreadSheetManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
                 'Powder Imaginary Permittivity',
                 'Powder ATR Reflectance',
                 'Analysis',
                 'Crystal R_p',
                 'Crystal R_s',
                 'Crystal T_p',
                 'Crystal T_s',
+                'Crystal A_p',
+                'Crystal A_s',
                 'Real Crystal Permittivity',
                 'Imag Crystal Permittivity' ]
         self.worksheets = {}
         # Positions points to where we write to next
         self.positions  = {}
         self.max_col    = {}
         self.max_row    = {}
```

### Comparing `PDielec-7.1.2/PDielec/GUI/ViewerTab.py` & `PDielec-7.2.1/PDielec/GUI/ViewerTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GUI/splash.png` & `PDielec-7.2.1/PDielec/GUI/splash.png`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GenericOutputReader.py` & `PDielec-7.2.1/PDielec/GenericOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/GulpOutputReader.py` & `PDielec-7.2.1/PDielec/GulpOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/IO.py` & `PDielec-7.2.1/PDielec/IO.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/Mie.py` & `PDielec-7.2.1/PDielec/Mie.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/PhonopyOutputReader.py` & `PDielec-7.2.1/PDielec/PhonopyOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/Plotter.py` & `PDielec-7.2.1/PDielec/Plotter.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/QEOutputReader.py` & `PDielec-7.2.1/PDielec/QEOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/SuperCell.py` & `PDielec-7.2.1/PDielec/SuperCell.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/UnitCell.py` & `PDielec-7.2.1/PDielec/UnitCell.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/Utilities.py` & `PDielec-7.2.1/PDielec/Utilities.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/VaspOutputReader.py` & `PDielec-7.2.1/PDielec/VaspOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/checkcsv.py` & `PDielec-7.2.1/PDielec/checkcsv.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/checkexcel.py` & `PDielec-7.2.1/PDielec/checkexcel.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/graphdatagenerator.py` & `PDielec-7.2.1/PDielec/graphdatagenerator.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/p1reader.py` & `PDielec-7.2.1/PDielec/p1reader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/p2cif.py` & `PDielec-7.2.1/PDielec/p2cif.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/pdcompare.py` & `PDielec-7.2.1/PDielec/pdcompare.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/pdgui.py` & `PDielec-7.2.1/PDielec/pdgui.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/pdmake.py` & `PDielec-7.2.1/PDielec/pdmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,15 +631,18 @@
 
 def runPyPi():
     if os.name == 'nt':
         print('Unable to create PyPi installation in Windows')
         return
     print('Creating PyPi distribution files')
     os.chdir(rootDirectory)
-    subprocess.run('rm -rf build dist PDielec.egg-info; python setup.py sdist bdist_wheel',shell=True)
+    # deprecated subprocess.run('rm -rf build dist PDielec.egg-info; python setup.py sdist bdist_wheel',shell=True)
+    # Following command needs an installed copy of setuptools
+    # pip install setuptools
+    subprocess.run('rm -rf build dist PDielec.egg-info; python -m build ',shell=True)
 
 def testForRootDirectory(path):
     test = os.path.join(path,'Examples')
     if not os.path.isdir(test):
         return False
 #    test = os.path.join(path,'PDielec')
 #    if not os.path.isdir(test):
```

### Comparing `PDielec-7.1.2/PDielec/pickled_reader.py` & `PDielec-7.2.1/PDielec/pickled_reader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/preader.py` & `PDielec-7.2.1/PDielec/preader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/test_gtm.py` & `PDielec-7.2.1/PDielec/test_gtm.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/test_ttm.py` & `PDielec-7.2.1/PDielec/test_ttm.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec/vibanalysis.py` & `PDielec-7.2.1/PDielec/vibanalysis.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PDielec.egg-info/PKG-INFO` & `PDielec-7.2.1/PDielec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: PDielec
-Version: 7.1.2
+Version: 7.2.1
 Summary: PDielec package for the calculation of THz and infrared spectra
 Home-page: https://github.com/JohnKendrick/PDielec
 Author: John Kendrick and Andrew Burnett
 Author-email: john@kendrick.co.uk
 License: MIT
 Keywords: Infrared, Infrared Spectroscopy,THz Spectroscopy,Terahertz Spectroscopy,Bruggeman,Maxwell-Garnett,Effective Medium
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -73,9 +72,7 @@
 <https://johnkendrick.github.io/PDielec/>
 
 Installation
 ============
 
 Full documentation of the program and its installation is available
 here; <https://johnkendrick.github.io/PDielec/>
-
-
```

### Comparing `PDielec-7.1.2/PDielec.egg-info/SOURCES.txt` & `PDielec-7.2.1/PDielec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/PKG-INFO` & `PDielec-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: PDielec
-Version: 7.1.2
+Version: 7.2.1
 Summary: PDielec package for the calculation of THz and infrared spectra
 Home-page: https://github.com/JohnKendrick/PDielec
 Author: John Kendrick and Andrew Burnett
 Author-email: john@kendrick.co.uk
 License: MIT
 Keywords: Infrared, Infrared Spectroscopy,THz Spectroscopy,Terahertz Spectroscopy,Bruggeman,Maxwell-Garnett,Effective Medium
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -73,9 +72,7 @@
 <https://johnkendrick.github.io/PDielec/>
 
 Installation
 ============
 
 Full documentation of the program and its installation is available
 here; <https://johnkendrick.github.io/PDielec/>
-
-
```

### Comparing `PDielec-7.1.2/README.md` & `PDielec-7.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PDielec-7.1.2/setup.py` & `PDielec-7.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 # Update this for every PyPi release
-version = "7.1.2"
+version = "7.2.1"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 init_lines = ["# Created by setup.py, whilst creating a new PyPi release\n","__version__ = \"{}\"\n".format(version)]
 with open("PDielec/__init__.py", "w") as fh:
```

