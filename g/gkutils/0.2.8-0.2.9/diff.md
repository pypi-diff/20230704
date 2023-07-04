# Comparing `tmp/gkutils-0.2.8.tar.gz` & `tmp/gkutils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gkutils-0.2.8.tar", last modified: Tue Nov  9 11:17:00 2021, max compression
+gzip compressed data, was "dist/gkutils-0.2.9.tar", last modified: Fri Nov 19 01:05:54 2021, max compression
```

## Comparing `gkutils-0.2.8.tar` & `gkutils-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-09 11:17:00.785665 gkutils-0.2.8/
--rw-r--r--   0 kws        (502) staff       (20)     1326 2021-11-09 11:17:00.785345 gkutils-0.2.8/PKG-INFO
--rwxr-xr-x   0 kws        (502) staff       (20)      723 2021-11-09 11:03:16.000000 gkutils-0.2.8/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-09 11:17:00.776693 gkutils-0.2.8/gkutils/
--rw-r--r--   0 kws        (502) staff       (20)       26 2020-06-10 15:01:19.000000 gkutils-0.2.8/gkutils/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2021-11-09 11:12:03.000000 gkutils-0.2.8/gkutils/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-09 11:17:00.784462 gkutils-0.2.8/gkutils/commonutils/
--rw-r--r--   0 kws        (502) staff       (20)       51 2020-06-21 19:02:34.000000 gkutils-0.2.8/gkutils/commonutils/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)     7554 2021-05-21 23:34:39.000000 gkutils-0.2.8/gkutils/commonutils/bruteForceConeSearchATLAS.py
--rw-r--r--   0 kws        (502) staff       (20)     8569 2021-08-03 15:48:30.000000 gkutils-0.2.8/gkutils/commonutils/coneSearchCassandra.py
--rw-r--r--   0 kws        (502) staff       (20)    91004 2021-08-01 23:57:17.000000 gkutils-0.2.8/gkutils/commonutils/generalutils.py
--rw-r--r--   0 kws        (502) staff       (20)     2580 2021-07-29 15:53:22.000000 gkutils-0.2.8/gkutils/commonutils/getCSVColumnSubset.py
--rw-r--r--   0 kws        (502) staff       (20)     4824 2020-06-21 19:10:34.000000 gkutils-0.2.8/gkutils/commonutils/mputils.py
--rw-r--r--   0 kws        (502) staff       (20)      375 2021-02-18 18:00:55.000000 gkutils-0.2.8/gkutils/commonutils/test.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-09 11:17:00.779032 gkutils-0.2.8/gkutils.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1326 2021-11-09 11:17:00.000000 gkutils-0.2.8/gkutils.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      510 2021-11-09 11:17:00.000000 gkutils-0.2.8/gkutils.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2021-11-09 11:17:00.000000 gkutils-0.2.8/gkutils.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      230 2021-11-09 11:17:00.000000 gkutils-0.2.8/gkutils.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       14 2021-11-09 11:17:00.000000 gkutils-0.2.8/gkutils.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        8 2021-11-09 11:17:00.000000 gkutils-0.2.8/gkutils.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2021-11-09 11:17:00.785794 gkutils-0.2.8/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1192 2021-11-09 11:12:45.000000 gkutils-0.2.8/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-19 01:05:54.495056 gkutils-0.2.9/
+-rw-r--r--   0 kws        (502) staff       (20)     1326 2021-11-19 01:05:54.494705 gkutils-0.2.9/PKG-INFO
+-rwxr-xr-x   0 kws        (502) staff       (20)      723 2021-11-09 11:03:16.000000 gkutils-0.2.9/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-19 01:05:54.482999 gkutils-0.2.9/gkutils/
+-rw-r--r--   0 kws        (502) staff       (20)       26 2020-06-10 15:01:19.000000 gkutils-0.2.9/gkutils/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2021-11-19 01:01:40.000000 gkutils-0.2.9/gkutils/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-19 01:05:54.493560 gkutils-0.2.9/gkutils/commonutils/
+-rw-r--r--   0 kws        (502) staff       (20)       51 2020-06-21 19:02:34.000000 gkutils-0.2.9/gkutils/commonutils/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)     7554 2021-05-21 23:34:39.000000 gkutils-0.2.9/gkutils/commonutils/bruteForceConeSearchATLAS.py
+-rw-r--r--   0 kws        (502) staff       (20)     8569 2021-08-03 15:48:30.000000 gkutils-0.2.9/gkutils/commonutils/coneSearchCassandra.py
+-rw-r--r--   0 kws        (502) staff       (20)    94039 2021-11-19 01:03:51.000000 gkutils-0.2.9/gkutils/commonutils/generalutils.py
+-rw-r--r--   0 kws        (502) staff       (20)     2580 2021-07-29 15:53:22.000000 gkutils-0.2.9/gkutils/commonutils/getCSVColumnSubset.py
+-rw-r--r--   0 kws        (502) staff       (20)     4824 2020-06-21 19:10:34.000000 gkutils-0.2.9/gkutils/commonutils/mputils.py
+-rw-r--r--   0 kws        (502) staff       (20)      375 2021-02-18 18:00:55.000000 gkutils-0.2.9/gkutils/commonutils/test.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-11-19 01:05:54.486367 gkutils-0.2.9/gkutils.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1326 2021-11-19 01:05:54.000000 gkutils-0.2.9/gkutils.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      510 2021-11-19 01:05:54.000000 gkutils-0.2.9/gkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2021-11-19 01:05:54.000000 gkutils-0.2.9/gkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      230 2021-11-19 01:05:54.000000 gkutils-0.2.9/gkutils.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       14 2021-11-19 01:05:54.000000 gkutils-0.2.9/gkutils.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        8 2021-11-19 01:05:54.000000 gkutils-0.2.9/gkutils.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2021-11-19 01:05:54.495212 gkutils-0.2.9/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1192 2021-11-19 01:01:59.000000 gkutils-0.2.9/setup.py
```

### Comparing `gkutils-0.2.8/PKG-INFO` & `gkutils-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkutils
-Version: 0.2.8
+Version: 0.2.9
 Summary: A collection useful utilities - mostly related to astronomy
 Home-page: https://github.com/genghisken/gkutils
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkutils Package #
```

### Comparing `gkutils-0.2.8/README.md` & `gkutils-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gkutils-0.2.8/gkutils/commonutils/bruteForceConeSearchATLAS.py` & `gkutils-0.2.9/gkutils/commonutils/bruteForceConeSearchATLAS.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.2.8/gkutils/commonutils/coneSearchCassandra.py` & `gkutils-0.2.9/gkutils/commonutils/coneSearchCassandra.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.2.8/gkutils/commonutils/generalutils.py` & `gkutils-0.2.9/gkutils/commonutils/generalutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2791,7 +2791,90 @@
         zp: zeropoint
     """
 
     factor = 10**(-0.4*(zp-23.9))
     uJy = adu/exptime*factor
     return uJy
 
+# 2021-11-18 KWS Added code to grab the SFD extinction for PS1 and ATLAS filters.
+def getSFDPanSTARRSATLASExtinction(ra, dec, dustmapDirectory, download = False):
+    """getPanSTARRSATLASExtinction.
+
+    Args:
+        ra: right ascension in degrees
+        dec: declination in degrees
+        dustmapDirectory: directory where the SFD dustmaps are stored
+        download: download the maps if they don't already exist
+    """
+    import os
+
+    extinction = {}
+
+    try:
+        from astropy.coordinates import SkyCoord
+    except ModuleNotFoundError as e:
+        print (e)
+        print ("Please install the astropy module.")
+        return extinction
+
+    try:
+        from dustmaps.sfd import SFDQuery, fetch
+    except ModuleNotFoundError as e:
+        print (e)
+        print ("Please install the dustmaps module.")
+        return extinction
+
+    from dustmaps.config import config
+    config['data_dir'] = dustmapDirectory
+
+    if not os.path.exists(dustmapDirectory + '/sfd/SFD_dust_4096_sgp.fits') or not os.path.exists(dustmapDirectory + '/sfd/SFD_dust_4096_ngp.fits'):
+        if download == True:
+            print("Downloading the SFD dustmap files...")
+            if not os.path.exists(dustmapDirectory):
+                os.makedirs(dustmapDirectory)
+            try:
+                fetch()
+            except PermissionError as e:
+                print (e)
+                print ("No permission to write into the download directory.")
+                return extinction
+        else:
+            print (e)
+            print("SFD Maps not found! Please elect to download the maps!")
+            return extinction
+
+    coords = SkyCoord(ra, dec, unit='deg', frame='icrs')
+
+    try:
+        sfd = SFDQuery()
+    except OSError as e:
+        print (e)
+        print ("Something went wrong - file is possibly corrupt. Try deleting the files and forcing a re-download.")
+        return extinction
+    except TypeError as e:
+        print (e)
+        print ("Something went wrong - file is possibly corrupt. Try deleting the files and forcing a re-download.")
+        return extinction
+    ebv = sfd(coords)
+
+    # Schlegel, Finkbeiner, Davis PS1 Rv3.1 conversions from
+    # https://ui.adsabs.harvard.edu/abs/1998ApJ...500..525S/abstract
+    # https://ui.adsabs.harvard.edu/abs/2011ApJ...737..103S/abstract
+
+    Rv31_PS1_g = 3.172
+    Rv31_PS1_r = 2.271
+    Rv31_PS1_i = 1.682
+    Rv31_PS1_z = 1.322
+    Rv31_PS1_y = 1.087
+
+    extinction['A_gPS1'] = round(ebv * Rv31_PS1_g,3)
+    extinction['A_rPS1'] = round(ebv * Rv31_PS1_r,3)
+    extinction['A_iPS1'] = round(ebv * Rv31_PS1_i,3)
+    extinction['A_zPS1'] = round(ebv * Rv31_PS1_z,3)
+    extinction['A_yPS1'] = round(ebv * Rv31_PS1_y,3)
+
+    # Calculating the ATLAS "c" and "o" from Tonry et al https://ui.adsabs.harvard.edu/abs/2018PASP..130f4505T/abstract
+    extinction['A_c'] = round((0.49 * extinction['A_gPS1']) + (0.51 * extinction['A_rPS1']),3)
+    extinction['A_o'] = round((0.55 * extinction['A_rPS1']) + (0.45 * extinction['A_iPS1']),3)
+
+    return extinction
+
```

### Comparing `gkutils-0.2.8/gkutils/commonutils/getCSVColumnSubset.py` & `gkutils-0.2.9/gkutils/commonutils/getCSVColumnSubset.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.2.8/gkutils/commonutils/mputils.py` & `gkutils-0.2.9/gkutils/commonutils/mputils.py`

 * *Files identical despite different names*

### Comparing `gkutils-0.2.8/gkutils.egg-info/PKG-INFO` & `gkutils-0.2.9/gkutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkutils
-Version: 0.2.8
+Version: 0.2.9
 Summary: A collection useful utilities - mostly related to astronomy
 Home-page: https://github.com/genghisken/gkutils
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkutils Package #
```

### Comparing `gkutils-0.2.8/setup.py` & `gkutils-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 setup(
     name="gkutils",
     description='A collection useful utilities - mostly related to astronomy',
     long_description=readme(),
     long_description_content_type="text/markdown",
-    version="0.2.8",
+    version="0.2.9",
     author='genghisken',
     author_email='ken.w.smith@gmail.com',
     license='MIT',
     url='https://github.com/genghisken/gkutils',
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
```

