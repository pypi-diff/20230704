# Comparing `tmp/crnpy-0.4.0.tar.gz` & `tmp/crnpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.4.0.tar", last modified: Mon Jul  3 20:15:16 2023, max compression
+gzip compressed data, was "crnpy-0.4.1.tar", last modified: Mon Jul  3 22:20:08 2023, max compression
```

## Comparing `crnpy-0.4.0.tar` & `crnpy-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.219850 crnpy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 20:15:05.000000 crnpy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 20:15:16.219850 crnpy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 20:15:05.000000 crnpy-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 20:15:16.219850 crnpy-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 20:15:05.000000 crnpy-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.215850 crnpy-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.215850 crnpy-0.4.0/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-03 20:15:05.000000 crnpy-0.4.0/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58185 2023-07-03 20:15:05.000000 crnpy-0.4.0/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-03 20:15:05.000000 crnpy-0.4.0/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:15:16.219850 crnpy-0.4.0/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 20:15:16.000000 crnpy-0.4.0/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 22:19:59.000000 crnpy-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 22:20:08.664037 crnpy-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 22:19:59.000000 crnpy-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 22:20:08.664037 crnpy-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 22:19:59.000000 crnpy-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-03 22:19:59.000000 crnpy-0.4.1/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58277 2023-07-03 22:19:59.000000 crnpy-0.4.1/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-03 22:19:59.000000 crnpy-0.4.1/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 22:20:08.664037 crnpy-0.4.1/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 22:20:08.000000 crnpy-0.4.1/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.4.0/LICENSE` & `crnpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.4.0/PKG-INFO` & `crnpy-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
 Home-page: https://github.com/soilwater/crnpy
 Author: Joaquin Peraza, Andres Patrignani
 Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crnpy-0.4.0/README.md` & `crnpy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `crnpy-0.4.0/setup.py` & `crnpy-0.4.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # contents of setup.py
 import setuptools
 
 setuptools.setup(
     name="crnpy",
-    version="0.4.0",
+    version="0.4.1",
     packages=['crnpy'],
     package_dir = {"": "src"},
     description="A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.",
     include_package_data=True,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/soilwater/crnpy",
```

### Comparing `crnpy-0.4.0/src/crnpy/crnpy.py` & `crnpy-0.4.1/src/crnpy/crnpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     df.sort_values(by=col, inplace=True)
     df.reset_index(drop=True, inplace=True)
     df.set_index(col, inplace=True)
     return df
 
 def count_time(counts=None, timestamp_col=None):
     """Approximate counting time.
+    The function will calculate the approximate counting time for each observation by taking the difference between
+    consecutive timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
 
     Args:
         counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
         timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
 
     Returns:
         (pandas.Series): Series with the approximate counting time for each observation.
@@ -115,15 +117,15 @@
     raise TypeError('Either counts or timestamp_col must be provided.')
 
 def fill_counts(counts, count_times=None, timestamp_col=None, expected_time=False, threshold=0.25, limit=3):
     """Fill missing neutron counts. Observation periods shorter than threshold are discarded (replaced with NaN).
     
     Args:
         counts (pandas.DataFrame): DataFrame with neutron counts, might have DateTimeIndex.
-        count_time (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as `counts`.
+        count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as `counts`.
         timestamp_col (pandas.Series): Series with timestamps. If counts has a DateTimeIndex, timestamp_col is not needed.
         expected_time (int): Expected counting time in seconds. If not provided, it is calculated as the median of the counting times.
         threshold (float): Minimum fraction of the neutron integration time. Default is 0.25.
 
     Returns:
         (pandas.DataFrame): DataFrame with linearly interpolated neutron counts.
 
@@ -181,15 +183,15 @@
         idx_nan = np.where(count_times < time_threshold)
         counts.loc[idx_nan] = np.nan
 
     # Fill missing values with linear interpolation and round to nearest integer
     counts = counts.interpolate(method='linear', limit=limit, limit_direction='both').round()
     return counts
 
-def adjust_temporal_counts(counts, count_time=3600, count_times=None, timestamp_col=None):
+def adjust_temporal_counts(counts, count_time=None, count_times=None, timestamp_col=None):
     """Normalize neutron counts to the desired counting time.
     
     Args:
         counts (pandas.DataFrame): Dataframe containing only the columns with neutron counts.
         count_time (int): Count time in seconds for normalization. Default is 3600 seconds.
         count_times (pandas.Series or pandas.DataFrame): Counting time in seconds. If a DataFrame is provided, it must have the same number of columns as counts.
         timestamp_col (pandas.Series): Timestamp column, used to calculate count time if count_times is not provided, it must have the same number of rows as counts.
@@ -730,15 +732,15 @@
 
     # Convert neutron counts into vwc
     vwc = (a0 / (counts/N0-a1) - a2 - Wlat - Wsoc) * bulk_density
     return vwc
 
 
 
-def sensing_depth(vwc, pressure, p_ref, bulk_density, Wlat, dist, method='Schron_2017'):
+def sensing_depth(vwc, pressure, p_ref, bulk_density, Wlat, dist=None, method='Schron_2017'):
     # Convert docstring to google format
     """Function that computes the estimated sensing depth of the cosmic-ray neutron probe.
     The function offers several methods to compute the depth at which 86 % of the neutrons
     probe the soil profile.
 
     Args:
         vwc (array or pd.Series or pd.DataFrame): Estimated volumetric water content for each timestamp.
@@ -760,29 +762,30 @@
         Schrön, M., Köhli, M., Scheiffele, L., Iwema, J., Bogena, H. R., Lv, L., et al. (2017).
         Improving calibration and validation of cosmic-ray neutron sensors in the light of spatial sensitivity.
         Hydrol. Earth Syst. Sci. 21, 5009–5030. doi.org/10.5194/hess-21-5009-2017
     """
 
     # Determine sensing depth (D86)
     if method == 'Schron_2017':
-
         # See Appendix A of Schrön et al. (2017)
         Fp = 0.4922 / (0.86 - np.exp(-1 * pressure / p_ref));
         Fveg = 0
         results = []
         for d in dist:
             # Compute r_star
             r_start = d/Fp
 
             # Compute soil depth that accounts for 86% of the neutron flux
             D86 = 1/ bulk_density * (8.321+0.14249*(0.96655 + np.exp(-0.01*r_start))*(20+(Wlat+vwc)) / (0.0429+(Wlat+vwc)))
             results.append(D86)
 
     elif method == 'Franz_2012':
         results = 5.8/(bulk_density*Wlat+vwc+0.0829)
+    else:
+        raise ValueError('Method not recognized. Please select either "Schron_2017" or "Franz_2012".')
 
     return results
 
 def estimate_abs_humidity(RH, temp):
     """
     Compute the actual vapor pressure (e) in g m^-3 using RH (%) and current temperature (c) observations.
 
@@ -939,16 +942,16 @@
     storage_subsurface = (SWI*(sm_max-sm_min) + sm_min)*Z_subsurface
 
     return storage_surface, storage_subsurface
 
 
 def cutoff_rigidity(lat,lon):
     """Function to estimate the approximate cutoff rigidity for any point on Earth according to the
-    tabulated data of Smart and Shea, 2019. Values are approximations so that users have an idea of
-    what neutron detectors from the Neutron Monitor Database (NMD).
+    tabulated data of Smart and Shea, 2019. The returned value can be used to select the appropriate
+    neutron monitor station to estimate the cosmic-ray neutron intensity at the location of interest.
 
     Args:
         lat (float): Geographic latitude in decimal degrees. Value in range -90 to 90
         lon (float): Geographic longitude in decimal degrees. Values in range from 0 to 360.
             Typical negative longitudes in the west hemisphere will fall in the range 180 to 360.
 
     Returns:
@@ -1054,29 +1057,23 @@
 
 def estimate_lattice_water(clay_content, total_carbon=None):
     r"""Estimate the amount of water in the lattice of clay minerals.
 
     ![img1](img/lattice_water_simple.png) | ![img2](img/lattice_water_multiple.png)
     :-------------------------:|:-------------------------:
     $\omega_{lat} = 0.097 * clay(\%)$ | $\omega_{lat} = -0.028 + 0.077 * clay(\%) + 0.459 * carbon(\%)$
-    Linear regression [lattice water (%) as a function of clay (%)] done with data from Soil Water Processes Lab and Dong and Ochsner (2018) |  Multiple linear regression [lattice water (%) as a function of clay (%) and soil carbon (%)] done with data from Soil Water Processes Lab.
+    Linear regression [lattice water (%) as a function of clay (%)] done with data from Kansas Sate University - Soil Water Processes Lab. |  Multiple linear regression [lattice water (%) as a function of clay (%) and soil carbon (%)] done with data from Soil Water Processes Lab.
 
     Args:
         clay_content (float): Clay content in the soil in percent.
         total_carbon (float, optional): Total carbon content in the soil in percent.
             If None, the amount of water is estimated based on clay content only.
 
     Returns:
         (float): Amount of water in the lattice of clay minerals in percent
-
-    References:
-        Dong, J., & Ochsner, T. E. (2018). Soil texture often exerts a stronger influence than precipitation
-         on mesoscale soil moisture patterns. Water Resources Research, 54, 2199– 2211.
-         https://doi.org/10.1002/2017WR021692
-
     """
     if total_carbon is None:
         lattice_water = 0.097 * clay_content
     else:
         lattice_water = -0.028 + 0.077 * clay_content + 0.459 * total_carbon
     return lattice_water
```

### Comparing `crnpy-0.4.0/src/crnpy/data.py` & `crnpy-0.4.1/src/crnpy/data.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.4.0/src/crnpy.egg-info/PKG-INFO` & `crnpy-0.4.1/src/crnpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
 Home-page: https://github.com/soilwater/crnpy
 Author: Joaquin Peraza, Andres Patrignani
 Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

