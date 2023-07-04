# Comparing `tmp/ukmon_meteortools-2023.6.2.tar.gz` & `tmp/ukmon_meteortools-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.6.2.tar", last modified: Tue Jun  6 22:05:45 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.7.0.tar", last modified: Tue Jul  4 19:43:00 2023, max compression
```

## Comparing `ukmon_meteortools-2023.6.2.tar` & `ukmon_meteortools-2023.7.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:45.533119 ukmon_meteortools-2023.6.2/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.6.2/LICENSE
--rw-rw-rw-   0        0        0    42725 2023-06-06 22:05:45.518923 ukmon_meteortools-2023.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.6.2/README.md
--rw-rw-rw-   0        0        0     2527 2023-06-06 22:05:16.000000 ukmon_meteortools-2023.6.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 22:05:45.533119 ukmon_meteortools-2023.6.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:44.996218 ukmon_meteortools-2023.6.2/ukmon_meteortools/
--rw-rw-rw-   0        0        0      819 2023-05-07 12:44:14.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:45.171219 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0     8762 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6211 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/UFOCapXML.py
--rw-rw-rw-   0        0        0      664 2023-05-08 13:19:19.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    18716 2023-05-08 11:58:38.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     5630 2023-05-08 12:37:01.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/kmlHandlers.py
--rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:45.271221 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      614 2023-05-08 13:20:18.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/plotRMSOrbits.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:45.300220 ukmon_meteortools-2023.6.2/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:45.380219 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/
--rw-rw-rw-   0        0        0     2094 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/ECSVhandler.py
--rw-rw-rw-   0        0        0      879 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/__init__.py
--rw-rw-rw-   0        0        0     3636 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/apiExampleCode.py
--rw-rw-rw-   0        0        0     1981 2023-05-08 19:28:35.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/getDetections.py
--rw-rw-rw-   0        0        0     4298 2023-05-19 20:56:49.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/getLiveImages.py
--rw-rw-rw-   0        0        0     1478 2023-05-08 21:25:36.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/trajPickle.py
--rw-rw-rw-   0        0        0     1795 2023-05-08 18:58:06.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/trajectoryKML.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:45.516917 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-08 19:57:04.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1556 2023-06-06 19:40:56.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1178 2023-05-08 13:25:56.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/drawFTPfile.py
--rw-rw-rw-   0        0        0     1454 2023-05-07 23:06:43.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/findNearDuplicates.py
--rw-rw-rw-   0        0        0     1405 2023-05-08 13:25:39.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3689 2023-05-08 12:09:09.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3887 2023-05-09 19:39:46.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/plotTrack.py
--rw-rw-rw-   0        0        0     6943 2023-06-06 20:28:23.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:05:45.092221 ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42725 2023-06-06 22:05:44.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1815 2023-06-06 22:05:44.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 22:05:44.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      353 2023-06-06 22:05:44.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-06 22:05:44.000000 ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.568363 ukmon_meteortools-2023.7.0/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.7.0/LICENSE
+-rw-rw-rw-   0        0        0    42725 2023-07-04 19:43:00.568363 ukmon_meteortools-2023.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.7.0/README.md
+-rw-rw-rw-   0        0        0     2627 2023-07-04 19:42:31.000000 ukmon_meteortools-2023.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-04 19:43:00.569364 ukmon_meteortools-2023.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.455365 ukmon_meteortools-2023.7.0/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      819 2023-05-07 12:44:14.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.497364 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0     8762 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6211 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/UFOCapXML.py
+-rw-rw-rw-   0        0        0      664 2023-05-08 13:19:19.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    18716 2023-05-08 11:58:38.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     5630 2023-05-08 12:37:01.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/kmlHandlers.py
+-rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.511364 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      652 2023-06-18 10:17:38.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     1372 2023-06-18 10:15:58.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/pickleToKml.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.528364 ukmon_meteortools-2023.7.0/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.547366 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/
+-rw-rw-rw-   0        0        0     2094 2023-05-09 16:50:40.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/ECSVhandler.py
+-rw-rw-rw-   0        0        0      879 2023-06-13 21:01:49.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/__init__.py
+-rw-rw-rw-   0        0        0     3636 2023-05-09 16:50:10.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/apiExampleCode.py
+-rw-rw-rw-   0        0        0     1981 2023-05-08 19:28:35.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/getDetections.py
+-rw-rw-rw-   0        0        0     4298 2023-05-19 20:56:49.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/getLiveImages.py
+-rw-rw-rw-   0        0        0     1478 2023-05-08 21:25:36.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/trajPickle.py
+-rw-rw-rw-   0        0        0     1795 2023-05-08 18:58:06.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/trajectoryKML.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.566365 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-08 19:57:04.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1614 2023-07-04 17:34:08.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-06-24 14:48:49.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1178 2023-05-08 13:25:56.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1454 2023-05-07 23:06:43.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     1405 2023-05-08 13:25:39.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3689 2023-05-08 12:09:09.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0      910 2023-07-04 17:42:03.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/getRiseSet.py
+-rw-rw-rw-   0        0        0     3887 2023-05-09 19:39:46.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/plotTrack.py
+-rw-rw-rw-   0        0        0     6943 2023-06-06 20:28:23.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-07-04 19:43:00.486422 ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42725 2023-07-04 19:43:00.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1895 2023-07-04 19:43:00.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 19:43:00.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      453 2023-07-04 19:43:00.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-04 19:43:00.000000 ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.6.2/LICENSE` & `ukmon_meteortools-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/PKG-INFO` & `ukmon_meteortools-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.6.2
+Version: 2023.7.0
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.6.2/README.md` & `ukmon_meteortools-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/pyproject.toml` & `ukmon_meteortools-2023.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.06.2"
+version = "2023.07.0"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -22,15 +22,16 @@
 keywords = ["meteors", "ukmon"]
 dependencies = [
     "fastparquet",
     "google-auth",
     "google-auth-oauthlib",
     "google-api-python-client",
     "googleapis-common-protos",
-    "matplotlib==3.3.2",
+    'matplotlib==3.3.2 ; python_version <= "3.8"',
+    'matplotlib; python_version > "3.8"',
     "numpy",
     "oauthlib",
     "pandas",
     "Pillow",
     "pytz",
     "Shapely",
     "simplekml",
@@ -43,15 +44,15 @@
     "opencv-python",
     "imageio",
     "scipy",
     "jplephem",
     "pyephem",
     "gitpython",
     "astropy",
-    "pyqt5",
+    "pyqt5; platform_machine != 'aarch64'",
     "basemap",
     "basemap-data-hires"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["bumpver", "gitpython", "behave", "pytest", "pip-tools"]
@@ -72,15 +73,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.06.2"
+current_version = "2023.07.0"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/UFOAnalyzerXML.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/UFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/UFOCapXML.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/UFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/__init__.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/kmlHandlers.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/kmlHandlers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 
 from .multiDayRadiant import multiDayRadiant
 from .multiTrackStack import multiTrackStack
 from .analyseUFOwithRMS import analyseUFOwithRMS
 from .multiEventGroundMap import multiEventGroundMap
 from .plotCAMSOrbits import plotCAMSOrbits
 from .plotRMSOrbits import plotRMSOrbits
+from .pickleToKml import pickleToKml
```

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/ECSVhandler.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/ECSVhandler.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/__init__.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/apiExampleCode.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/getDetections.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/getDetections.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/getLiveImages.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/trajPickle.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/trajPickle.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/ukmondb/trajectoryKML.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/ukmondb/trajectoryKML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 
 annotateImage, annotateImageArbitrary  
 
 getActiveShowers, getActiveShowersStr, getShowerDets, getShowerPeak  
 
 sendAnEmail, forwardAnEmail
 
+getNextRiseSet
+
 """
 from .Math import jd2Date, date2JD,datetime2JD, jd2DynamicalTimeJD, JULIAN_EPOCH, J2000_JD, jd2LST
 from .Math import greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation
 from .Math import calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec
 from .Math import altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect
 from .annotateImage import annotateImage, annotateImageArbitrary
 from .convertSolLon import sollon2jd
 from .getActiveShowers import getActiveShowers, getActiveShowersStr
 from .getShowerDates import getShowerDets, getShowerPeak
 from .sendAnEmail import sendAnEmail, forwardAnEmail
 from .drawFTPfile import drawFTPFile
 from .plotTrack import trackToDistvsHeight, trackToTimevsVelocity, trackToTimevsHeight
 from .getOverlappingFovs import checkKMLOverlap, pointInsideFov, getOverlapWith, getOverlappingCameras
+from .getRiseSet import getNextRiseSet
 
 #from .findNearDuplicates import findNearDuplicates
```

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/drawFTPfile.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/findNearDuplicates.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/getOverlappingFovs.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/getShowerDates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/plotTrack.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.7.0/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.6.2
+Version: 2023.7.0
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.6.2/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.7.0/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ukmon_meteortools/fileformats/kmlHandlers.py
 ukmon_meteortools/fileformats/platepar.py
 ukmon_meteortools/rmsutils/__init__.py
 ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
 ukmon_meteortools/rmsutils/multiDayRadiant.py
 ukmon_meteortools/rmsutils/multiEventGroundMap.py
 ukmon_meteortools/rmsutils/multiTrackStack.py
+ukmon_meteortools/rmsutils/pickleToKml.py
 ukmon_meteortools/rmsutils/plotCAMSOrbits.py
 ukmon_meteortools/rmsutils/plotRMSOrbits.py
 ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
 ukmon_meteortools/share/__init__.py
 ukmon_meteortools/share/streamfulldata.npy
 ukmon_meteortools/ukmondb/ECSVhandler.py
 ukmon_meteortools/ukmondb/__init__.py
@@ -36,10 +37,11 @@
 ukmon_meteortools/utils/__init__.py
 ukmon_meteortools/utils/annotateImage.py
 ukmon_meteortools/utils/convertSolLon.py
 ukmon_meteortools/utils/drawFTPfile.py
 ukmon_meteortools/utils/findNearDuplicates.py
 ukmon_meteortools/utils/getActiveShowers.py
 ukmon_meteortools/utils/getOverlappingFovs.py
+ukmon_meteortools/utils/getRiseSet.py
 ukmon_meteortools/utils/getShowerDates.py
 ukmon_meteortools/utils/plotTrack.py
 ukmon_meteortools/utils/sendAnEmail.py
```

