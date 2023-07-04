# Comparing `tmp/pymwalib-0.8.8.tar.gz` & `tmp/pymwalib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymwalib-0.8.8.tar", last modified: Tue Aug  3 02:53:07 2021, max compression
+gzip compressed data, was "dist/pymwalib-0.9.1.tar", last modified: Wed Aug 11 07:36:50 2021, max compression
```

## Comparing `pymwalib-0.8.8.tar` & `pymwalib-0.9.1.tar`

### file list

```diff
@@ -1,55 +1,23 @@
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.730000 pymwalib-0.8.8/
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.710000 pymwalib-0.8.8/.github/
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.720000 pymwalib-0.8.8/.github/workflows/
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     2374 2021-08-03 01:37:34.000000 pymwalib-0.8.8/.github/workflows/ci.yml
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)      111 2021-07-01 08:00:23.000000 pymwalib-0.8.8/.gitignore
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     4880 2021-08-03 02:50:47.000000 pymwalib-0.8.8/CHANGELOG.md
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)      997 2021-08-03 01:38:03.000000 pymwalib-0.8.8/Dockerfile
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    16725 2021-03-05 08:08:47.000000 pymwalib-0.8.8/LICENSE.txt
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)       94 2021-08-03 02:37:51.000000 pymwalib-0.8.8/MANIFEST.in
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1629 2021-08-03 02:53:07.730000 pymwalib-0.8.8/PKG-INFO
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)      667 2021-07-02 02:31:05.000000 pymwalib-0.8.8/README.md
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.720000 pymwalib-0.8.8/examples/
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     2671 2021-08-03 01:10:35.000000 pymwalib-0.8.8/examples/print-context.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3881 2021-08-03 01:10:35.000000 pymwalib-0.8.8/examples/sum-gpuboxes.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     4304 2021-08-03 01:10:35.000000 pymwalib-0.8.8/examples/sum-vcs.py
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.720000 pymwalib-0.8.8/pymwalib/
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)        0 2020-12-17 04:58:03.000000 pymwalib-0.8.8/pymwalib/__init__.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     2970 2021-08-03 01:09:51.000000 pymwalib-0.8.8/pymwalib/antenna.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1739 2021-08-03 01:09:51.000000 pymwalib-0.8.8/pymwalib/baseline.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     4045 2021-08-03 01:09:51.000000 pymwalib-0.8.8/pymwalib/coarse_channel.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1652 2021-08-03 01:09:50.000000 pymwalib-0.8.8/pymwalib/common.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)      692 2021-08-03 01:09:51.000000 pymwalib-0.8.8/pymwalib/constants.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    15915 2021-08-03 01:49:03.000000 pymwalib-0.8.8/pymwalib/correlator_context.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3567 2021-08-03 01:10:14.000000 pymwalib-0.8.8/pymwalib/errors.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3388 2021-08-03 01:15:59.000000 pymwalib-0.8.8/pymwalib/metafits_context.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    11860 2021-08-03 01:10:14.000000 pymwalib-0.8.8/pymwalib/metafits_metadata.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    19856 2021-08-03 01:13:22.000000 pymwalib-0.8.8/pymwalib/mwalib.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3772 2021-08-03 01:10:14.000000 pymwalib-0.8.8/pymwalib/rfinput.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     2428 2021-08-03 01:10:14.000000 pymwalib-0.8.8/pymwalib/timestep.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3000 2021-08-03 02:48:52.000000 pymwalib-0.8.8/pymwalib/version.py
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    17270 2021-08-03 01:49:58.000000 pymwalib-0.8.8/pymwalib/voltage_context.py
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.720000 pymwalib-0.8.8/pymwalib.egg-info/
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1629 2021-08-03 02:53:07.000000 pymwalib-0.8.8/pymwalib.egg-info/PKG-INFO
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1230 2021-08-03 02:53:07.000000 pymwalib-0.8.8/pymwalib.egg-info/SOURCES.txt
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)        1 2021-08-03 02:53:07.000000 pymwalib-0.8.8/pymwalib.egg-info/dependency_links.txt
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)        6 2021-08-03 02:53:07.000000 pymwalib-0.8.8/pymwalib.egg-info/requires.txt
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)        9 2021-08-03 02:53:07.000000 pymwalib-0.8.8/pymwalib.egg-info/top_level.txt
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)        6 2020-12-17 04:58:03.000000 pymwalib-0.8.8/requirements.txt
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)       79 2021-08-03 02:53:07.730000 pymwalib-0.8.8/setup.cfg
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1515 2021-08-03 02:49:31.000000 pymwalib-0.8.8/setup.py
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.720000 pymwalib-0.8.8/tests/
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.710000 pymwalib-0.8.8/tests/data/
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.720000 pymwalib-0.8.8/tests/data/1297526432_mwax/
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    14400 2021-05-04 01:57:11.000000 pymwalib-0.8.8/tests/data/1297526432_mwax/1297526432.metafits
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    25920 2021-05-04 01:57:11.000000 pymwalib-0.8.8/tests/data/1297526432_mwax/1297526432_20210216160014_ch117_000.fits
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    25920 2021-05-04 01:57:11.000000 pymwalib-0.8.8/tests/data/1297526432_mwax/1297526432_20210216160014_ch117_001.fits
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    25920 2021-05-04 01:57:11.000000 pymwalib-0.8.8/tests/data/1297526432_mwax/1297526432_20210216160014_ch118_000.fits
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)    25920 2021-05-04 01:57:11.000000 pymwalib-0.8.8/tests/data/1297526432_mwax/1297526432_20210216160014_ch118_001.fits
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3544 2021-05-04 01:57:11.000000 pymwalib-0.8.8/tests/data/1297526432_mwax/1297526432_dump.csv
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3948 2021-05-04 01:57:11.000000 pymwalib-0.8.8/tests/data/1297526432_mwax/1297526432_dump_hex.csv
--rw-r--r--   0 gsleap    (1000) gsleap    (1000)     7222 2021-08-03 01:50:14.000000 pymwalib-0.8.8/tests/test_correlator_context.py
-drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-03 02:53:07.720000 pymwalib-0.8.8/tools/
--rwxr-xr-x   0 gsleap    (1000) gsleap    (1000)      313 2021-08-03 02:44:17.000000 pymwalib-0.8.8/tools/make_release.sh
--rwxr-xr-x   0 gsleap    (1000) gsleap    (1000)      351 2021-08-03 02:44:17.000000 pymwalib-0.8.8/tools/make_release_and_publish.sh
--rwxr--r--   0 gsleap    (1000) gsleap    (1000)      219 2021-08-03 02:10:05.000000 pymwalib-0.8.8/tools/validate.sh
+drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-11 07:36:50.591263 pymwalib-0.9.1/
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     5363 2021-08-11 07:15:03.231272 pymwalib-0.9.1/CHANGELOG.md
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)    16725 2021-03-05 08:08:47.000000 pymwalib-0.9.1/LICENSE.txt
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1638 2021-08-11 07:36:50.591263 pymwalib-0.9.1/PKG-INFO
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)      667 2021-07-02 02:31:05.000000 pymwalib-0.9.1/README.md
+drwxr-xr-x   0 gsleap    (1000) gsleap    (1000)        0 2021-08-11 07:36:50.591263 pymwalib-0.9.1/pymwalib/
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)        0 2020-12-17 04:58:03.000000 pymwalib-0.9.1/pymwalib/__init__.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     2970 2021-08-03 01:09:51.000000 pymwalib-0.9.1/pymwalib/antenna.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1739 2021-08-03 01:09:51.000000 pymwalib-0.9.1/pymwalib/baseline.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     4045 2021-08-03 01:09:51.000000 pymwalib-0.9.1/pymwalib/coarse_channel.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1652 2021-08-03 01:09:50.000000 pymwalib-0.9.1/pymwalib/common.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)      692 2021-08-03 01:09:51.000000 pymwalib-0.9.1/pymwalib/constants.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)    15915 2021-08-03 01:49:03.000000 pymwalib-0.9.1/pymwalib/correlator_context.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3736 2021-08-11 07:30:24.161266 pymwalib-0.9.1/pymwalib/errors.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     5145 2021-08-11 07:30:43.011266 pymwalib-0.9.1/pymwalib/metafits_context.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)    12603 2021-08-11 05:46:43.921310 pymwalib-0.9.1/pymwalib/metafits_metadata.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)    21375 2021-08-11 07:20:21.391270 pymwalib-0.9.1/pymwalib/mwalib.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     5216 2021-08-11 05:50:32.001308 pymwalib-0.9.1/pymwalib/rfinput.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     2428 2021-08-03 01:10:14.000000 pymwalib-0.9.1/pymwalib/timestep.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     3000 2021-08-03 02:48:52.000000 pymwalib-0.9.1/pymwalib/version.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)    17270 2021-08-03 01:49:58.000000 pymwalib-0.9.1/pymwalib/voltage_context.py
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)       40 2021-03-05 08:08:47.000000 pymwalib-0.9.1/setup.cfg
+-rw-r--r--   0 gsleap    (1000) gsleap    (1000)     1486 2021-08-11 07:31:54.221265 pymwalib-0.9.1/setup.py
```

### Comparing `pymwalib-0.8.8/CHANGELOG.md` & `pymwalib-0.9.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Change Log
 
 Changes in each release are listed below. Please see MWATelescope/mwalib CHANGELOG for more detailed changes to the underlying mwalib library.
 
+## 0.9.1 11-Aug-2021 (Pre-release)
+
+* Requires mwalib 0.9.*.
+* Added mwa_version to MetafitsContext.
+* When working only with a MetafitsContext, None can be passed in lieu of an MWAVersion, and mwalib will attempt to determine the correct MWAVersion based on the MODE keyword from the metafits file.
+* Added method get_expected_volt_filename() function to MetafitsContext.
+* Added digital_gains, dipole_gains and dipole_delays Rfinput.
+* Added receivers, delays to MetafitsContext.
+
 ## 0.8.8 03-Aug-2021 (Pre-release)
 
 * Requires mwalib 0.8.7.
 * Release to fix issue with pypi deployment.
 * Pymwalib now only has to match mwalib major and minor version, not patch version. This allows more flexibility in releases.
 * No other changes.
```

### Comparing `pymwalib-0.8.8/LICENSE.txt` & `pymwalib-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/PKG-INFO` & `pymwalib-0.9.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: pymwalib
-Version: 0.8.8
+Version: 0.9.1
 Summary: A Python interface for mwalib, a library to read Murchison Widefield Array (MWA) raw visibilities, voltages and metadata into a common structure
 Home-page: https://github.com/MWATelescope/pymwalib
 Author: Greg Sleap
 Author-email: greg.sleap@curtin.edu.au
 License: mpl-2.0
-Download-URL: https://github.com/MWATelescope/pymwalib/archive/refs/tags/v0.8.7.tar.gz
+Download-URL: https://github.com/MWATelescope/pymwalib/archive/refs/tags/v0.9.1.tar.gz
+Description: # pymwalib
+        ![Tests](https://github.com/MWATelescope/pymwalib/workflows/Code%20Coverage/badge.svg)
+        [![codecov](https://codecov.io/gh/MWATelescope/pymwalib/branch/master/graph/badge.svg)](https://codecov.io/gh/MWATelescope/pymwalib)
+        A Python interface for [MWATelescope/mwalib](https://github.com/MWATelescope/mwalib) that provides a simple
+        interface for reading MWA correlator raw visibilities, recombined voltages and exposing the relevant metadata. pymwalib and mwalib
+        both support reading data produced by the existing (legacy) MWA and the new MWAX systems.
+        
+        See [pymwalib Wiki](https://github.com/MWATelescope/pymwalib/wiki) for installation and usage infomation.
+        
 Keywords: MWA,radioastronomy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# pymwalib
-![Tests](https://github.com/MWATelescope/pymwalib/workflows/Code%20Coverage/badge.svg)
-[![codecov](https://codecov.io/gh/MWATelescope/pymwalib/branch/master/graph/badge.svg)](https://codecov.io/gh/MWATelescope/pymwalib)
-A Python interface for [MWATelescope/mwalib](https://github.com/MWATelescope/mwalib) that provides a simple
-interface for reading MWA correlator raw visibilities, recombined voltages and exposing the relevant metadata. pymwalib and mwalib
-both support reading data produced by the existing (legacy) MWA and the new MWAX systems.
-
-See [pymwalib Wiki](https://github.com/MWATelescope/pymwalib/wiki) for installation and usage infomation.
-
-
```

### Comparing `pymwalib-0.8.8/README.md` & `pymwalib-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/antenna.py` & `pymwalib-0.9.1/pymwalib/antenna.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/baseline.py` & `pymwalib-0.9.1/pymwalib/baseline.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/coarse_channel.py` & `pymwalib-0.9.1/pymwalib/coarse_channel.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/common.py` & `pymwalib-0.9.1/pymwalib/common.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/constants.py` & `pymwalib-0.9.1/pymwalib/constants.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/correlator_context.py` & `pymwalib-0.9.1/pymwalib/correlator_context.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/errors.py` & `pymwalib-0.9.1/pymwalib/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,19 @@
 
 
 class PymwalibMetafitsContextDisplayError(PymwalibError):
     """Raised when call to C mwalib_metafits_context_display fails"""
     pass
 
 
+class PymwalibMetafitsContextGetExpectedVoltageFilename(PymwalibError):
+    """Raised when call to C mwalib_metafits_get_expected_volt_filename fails"""
+    pass
+
+
 class PymwalibCorrelatorContextDisplayError(PymwalibError):
     """Raised when call to C mwalib_correlator_context_display fails"""
     pass
 
 
 class PymwalibCorrelatorContextGetFineChanFreqsArrayError(PymwalibError):
     """Raised when call to C mwalib_correlator_context_get_fine_chan_freqs_hz_array fails"""
```

### Comparing `pymwalib-0.8.8/pymwalib/metafits_metadata.py` & `pymwalib-0.9.1/pymwalib/metafits_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 import ctypes as ct
 from datetime import datetime
 from .mwalib import mwalib_library, CMetafitsMetadataS, CMetafitsContextS, CCorrelatorContextS, CVoltageContextS, \
     create_string_buffer
-from .common import ERROR_MESSAGE_LEN, MWAMode, GeometricDelaysApplied
+from .common import ERROR_MESSAGE_LEN, MWAMode, MWAVersion, GeometricDelaysApplied
 from .errors import PymwalibMetafitsMetadataGetError
 from .antenna import Antenna
 from .baseline import Baseline
 from .rfinput import RFInput
 from .coarse_channel import CoarseChannel
 from .timestep import TimeStep
 
@@ -37,14 +37,15 @@
                                                        ERROR_MESSAGE_LEN) != 0:
             raise PymwalibMetafitsMetadataGetError(
                 f"Error creating metafits metadata object: {error_message.decode('utf-8').rstrip()}")
         else:
             # Populate all the fields
             c_object = c_object_ptr.contents
 
+            self.mwa_version: MWAVersion = c_object.mwa_version
             self.obs_id: int = c_object.obs_id
             self.global_analogue_attenuation_db: float = c_object.global_analogue_attenuation_db
             self.ra_tile_pointing_deg: float = c_object.ra_tile_pointing_deg
             self.dec_tile_pointing_deg: float = c_object.dec_tile_pointing_deg
             self.ra_phase_center_deg: float = c_object.ra_phase_center_deg
             self.dec_phase_center_deg: float = c_object.dec_phase_center_deg
             self.az_deg: float = c_object.az_deg
@@ -70,14 +71,22 @@
             self.cable_delays_applied: bool = c_object.cable_delays_applied
             self.calibration_delays_and_gains_applied: bool = c_object.calibration_delays_and_gains_applied
             self.corr_fine_chan_width_hz: int = c_object.corr_fine_chan_width_hz
             self.corr_int_time_ms: int = c_object.corr_int_time_ms
             self.num_corr_fine_chans_per_coarse: int = c_object.num_corr_fine_chans_per_coarse
             self.volt_fine_chan_width_hz: int = c_object.volt_fine_chan_width_hz
             self.num_volt_fine_chans_per_coarse: int = c_object.num_volt_fine_chans_per_coarse
+            self.num_receivers = c_object.num_receivers
+            self.receivers = []
+            for r in range(0, self.num_receivers):
+                self.receivers.append(c_object.receivers[r])
+            self.num_delays = c_object.num_delays
+            self.delays = []
+            for d in range(0, self.num_delays):
+                self.delays.append(c_object.delays[d])
             self.sched_start_utc: datetime = datetime.utcfromtimestamp(c_object.sched_start_utc)
             self.sched_end_utc: datetime = datetime.utcfromtimestamp(c_object.sched_end_utc)
             self.sched_start_mjd: float = c_object.sched_start_mjd
             self.sched_end_mjd: float = c_object.sched_end_mjd
             self.sched_start_unix_time_ms: int = c_object.sched_start_unix_time_ms
             self.sched_end_unix_time_ms: int = c_object.sched_end_unix_time_ms
             self.sched_start_gps_time_ms: int = c_object.sched_start_gps_time_ms
@@ -112,26 +121,27 @@
             self.metafits_timesteps = TimeStep.get_metafits_timesteps(c_object)
 
             # Populate coarse channels
             self.metafits_coarse_chans = CoarseChannel.get_metafits_coarse_channels(c_object)
 
             # fine chan frequencies
             self.metafits_fine_chan_freqs_hz = []
-            for i in range(0, 4):
+            for i in range(0, self.num_metafits_fine_chan_freqs):
                 self.metafits_fine_chan_freqs_hz.append(c_object.metafits_fine_chan_freqs_hz[i])
 
             # We're now finished with the C memory, so free it
             mwalib_library.mwalib_metafits_metadata_free(c_object)
 
     def __repr__(self):
         return "%s(%r)" % (self.__class__, self.__dict__)
 
     def __str__(self):
         """Returns a representation of the class"""
         return f"{self.__class__.__name__}(\n" \
+               f"MWA Version                           : {self.mwa_version.name}\n" \
                f"Obs ID                                : {self.obs_id}\n" \
                f"Global attenuation                    : {self.global_analogue_attenuation_db} dB\n" \
                f"RA  (tile pointing)                   : {self.ra_tile_pointing_deg} deg\n" \
                f"Dec (tile pointing)                   : {self.dec_tile_pointing_deg} deg\n" \
                f"RA  (phase centre)                    : {self.ra_phase_center_deg} deg\n" \
                f"Dec (phase centre)                    : {self.dec_phase_center_deg} deg\n" \
                f"Az                                    : {self.az_deg} deg\n" \
@@ -155,14 +165,16 @@
                f"Mode                                  : {self.mode}\n" \
                f"geometric_delays_applied              : {self.geometric_delays_applied}\n" \
                f"cable_delays_applied                  : {self.cable_delays_applied}\n" \
                f"calibration_delays_and_gains_applied  : {self.calibration_delays_and_gains_applied}\n" \
                f"Correlator fine channel width (Hz)    : {self.corr_fine_chan_width_hz}\n" \
                f"Correlator int. time (ms)             : {self.corr_int_time_ms}\n" \
                f"Correlator fine channels per coarse   : {self.num_corr_fine_chans_per_coarse}\n" \
+               f"Receivers                             : {self.receivers}\n" \
+               f"Delays                                : {self.delays}\n" \
                f"Scheduled Start (UTC)                 : {self.sched_start_utc}\n" \
                f"Scheduled End (UTC)                   : {self.sched_end_utc}\n" \
                f"Scheduled Start (UNIX)                : {float(self.sched_start_unix_time_ms) / 1000.} UNIX\n" \
                f"Scheduled End (UNIX)                  : {float(self.sched_end_unix_time_ms) / 1000.} UNIX\n" \
                f"Scheduled Start (MJD)                 : {self.sched_start_mjd} MJD\n" \
                f"Scheduled End (MJD)                   : {self.sched_end_mjd} MJD\n" \
                f"Scheduled Duration                    : {float(self.sched_duration_ms) / 1000.} s\n" \
```

### Comparing `pymwalib-0.8.8/pymwalib/mwalib.py` & `pymwalib-0.9.1/pymwalib/mwalib.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,28 +85,52 @@
     #
     mwalib_library.mwalib_metafits_context_new.argtypes = \
         (ct.c_char_p,  # metafits
          ct.c_uint,  # MWAVersion
          ct.POINTER(ct.POINTER(CMetafitsContextS)),  # Pointer to pointer to CorrelatorContext
          ct.c_char_p,  # error message
          ct.c_size_t)  # length of error message
+    mwalib_library.mwalib_metafits_context_new.restype = ct.c_int32
+
+    #
+    # mwalib_metafits_context_new2()
+    #
+    mwalib_library.mwalib_metafits_context_new2.argtypes = \
+        (ct.c_char_p,  # metafits
+         ct.POINTER(ct.POINTER(CMetafitsContextS)),  # Pointer to pointer to CorrelatorContext
+         ct.c_char_p,  # error message
+         ct.c_size_t)  # length of error message
+    mwalib_library.mwalib_metafits_context_new2.restype = ct.c_int32
 
     #
     # mwalib_metafits_context_free()
     #
     mwalib_library.mwalib_metafits_context_free.argtypes = (ct.POINTER(CMetafitsContextS),)
     mwalib_library.mwalib_metafits_context_free.restype = ct.c_int32
 
     #
     # mwalib_metafits_context_display()
     #
     mwalib_library.mwalib_metafits_context_display.argtypes = (ct.POINTER(CMetafitsContextS),)
     mwalib_library.mwalib_metafits_context_display.restype = ct.c_int32
 
     #
+    # mwalib_metafits_get_expected_volt_filename
+    #
+    mwalib_library.mwalib_metafits_get_expected_volt_filename.argtypes = \
+        (ct.POINTER(CMetafitsContextS),  # metafits context
+         ct.c_size_t,  # timestep_index
+         ct.c_size_t,  # coarse_chan_index
+         ct.c_char_p,  # filename buffer
+         ct.c_size_t,  # length of filename buffer
+         ct.c_char_p,  # error message
+         ct.c_size_t)  # length of error message
+    mwalib_library.mwalib_metafits_get_expected_volt_filename.restype = ct.c_int32
+
+    #
     # C Antenna struct
     #
     class CAntennaS(ct.Structure):
         _fields_ = [('ant', ct.c_uint32),
                     ('tile_id', ct.c_uint32),
                     ('tile_name', ct.c_char_p),
                     ('rfinput_x', ct.c_size_t),
@@ -148,29 +172,36 @@
                     ('electrical_length_m', ct.c_double),
                     ('north_m', ct.c_double),
                     ('east_m', ct.c_double),
                     ('height_m', ct.c_double),
                     ('vcs_order', ct.c_uint32),
                     ('subfile_order', ct.c_uint32),
                     ('flagged', ct.c_bool),
+                    ('digital_gains', ct.POINTER(ct.c_uint32)),
+                    ('num_digital_gains', ct.c_size_t),
+                    ('dipole_delays', ct.POINTER(ct.c_uint32)),
+                    ('num_dipole_delays', ct.c_size_t),
+                    ('dipole_gains', ct.POINTER(ct.c_double)),
+                    ('num_dipole_gains', ct.c_size_t),
                     ('rec_number', ct.c_uint32),
-                    ('rec_slot_number', ct.c_uint32)]
+                    ('rec_slot_number', ct.c_uint32), ]
 
     #
     # C TimeStep struct
     #
     class CTimeStepS(ct.Structure):
         _fields_ = [('unix_time_ms', ct.c_uint64),
                     ('gps_time_ms', ct.c_uint64), ]
 
     #
     # C MetafitsMetadata struct
     #
     class CMetafitsMetadataS(ct.Structure):
-        _fields_ = [('obs_id', ct.c_uint32),
+        _fields_ = [('mwa_version', ct.c_uint32),
+                    ('obs_id', ct.c_uint32),
                     ('global_analogue_attenuation_db', ct.c_double),
                     ('ra_tile_pointing_deg', ct.c_double),
                     ('dec_tile_pointing_deg', ct.c_double),
                     ('ra_phase_center_deg', ct.c_double),
                     ('dec_phase_center_deg', ct.c_double),
                     ('az_deg', ct.c_double),
                     ('alt_deg', ct.c_double),
@@ -196,15 +227,17 @@
                     ('calibration_delays_and_gains_applied', ct.c_bool),
                     ('corr_fine_chan_width_hz', ct.c_uint32),
                     ('corr_int_time_ms', ct.c_uint64),
                     ('num_corr_fine_chans_per_coarse', ct.c_size_t),
                     ('volt_fine_chan_width_hz', ct.c_int32),
                     ('num_volt_fine_chans_per_coarse', ct.c_size_t),
                     ('receivers', ct.POINTER(ct.c_size_t)),
+                    ('num_receivers', ct.c_size_t),
                     ('delays', ct.POINTER(ct.c_uint32)),
+                    ('num_delays', ct.c_size_t),
                     ('sched_start_utc', ct.c_uint64),
                     ('sched_end_utc', ct.c_uint64),
                     ('sched_start_mjd', ct.c_double),
                     ('sched_end_mjd', ct.c_double),
                     ('sched_start_unix_time_ms', ct.c_uint64),
                     ('sched_end_unix_time_ms', ct.c_uint64),
                     ('sched_start_gps_time_ms', ct.c_uint64),
```

### Comparing `pymwalib-0.8.8/pymwalib/rfinput.py` & `pymwalib-0.9.1/pymwalib/rfinput.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,14 +32,20 @@
                  electrical_length_m: float,
                  north_m: float,
                  east_m: float,
                  height_m: float,
                  vcs_order: int,
                  subfile_order: int,
                  flagged: bool,
+                 digital_gains: [],
+                 num_digital_gains: int,
+                 dipole_delays: [],
+                 num_dipole_delays: int,
+                 dipole_gains: [],
+                 num_dipole_gains: int,
                  rec_number: int,
                  rec_slot_number: int):
         """Initialise the class"""
         self.index: int = index
         self.input: int = input
         self.ant: int = ant
         self.tile_id: int = tile_id
@@ -48,14 +54,20 @@
         self.electrical_length_m: float = electrical_length_m
         self.north_m: float = north_m
         self.east_m: float = east_m
         self.height_m: float = height_m
         self.vcs_order: int = vcs_order
         self.subfile_order: int = subfile_order
         self.flagged: bool = flagged
+        self.num_digital_gains = num_digital_gains
+        self.digital_gains = digital_gains
+        self.num_dipole_delays = num_dipole_delays
+        self.dipole_delays = dipole_delays
+        self.num_dipole_gains = num_dipole_gains
+        self.dipole_gains = dipole_gains
         self.rec_number = rec_number
         self.rec_slot_number = rec_slot_number
 
     def __repr__(self):
         """Returns a representation of the class"""
         return f"{self.__class__.__name__}(" \
                f"Index: {self.index}, " \
@@ -67,36 +79,57 @@
                f"Electrical length: {self.electrical_length_m}, " \
                f"north_m: {self.north_m}, " \
                f"east_m: {self.east_m}, " \
                f"height_m: {self.height_m}, " \
                f"vcs_order: {self.vcs_order}, " \
                f"subfile_order: {self.subfile_order}, " \
                f"flagged: {self.flagged}, " \
+               f"digital_gains: {self.digital_gains}, " \
+               f"dipole_delays: {self.dipole_delays}, " \
+               f"dipole_gains: {self.dipole_gains}, " \
                f"rec_number: {self.rec_number}, " \
                f"rec_slot_number: {self.rec_slot_number})"
 
     @staticmethod
     def get_rf_inputs(metafits_metadata: CMetafitsMetadataS) -> []:
         """Retrieve all of the rf_input metadata and populate a list of rf_inputs."""
         rf_inputs = []
 
         for i in range(0, metafits_metadata.num_rf_inputs):
             obj: CRFInputS = metafits_metadata.rf_inputs[i]
 
+            digital_gains = []
+            for i in range(0, obj.num_digital_gains):
+                digital_gains.append(obj.digital_gains[i])
+
+            dipole_delays = []
+            for j in range(0, obj.num_dipole_delays):
+                dipole_delays.append(obj.dipole_delays[j])
+
+            dipole_gains = []
+            for k in range(0, obj.num_dipole_gains):
+                dipole_gains.append(obj.dipole_gains[k])
+
             # Populate all the fields
             rf_inputs.append(RFInput(i,
                                      obj.input,
                                      obj.ant,
                                      obj.tile_id,
                                      obj.tile_name.decode("utf-8"),
                                      obj.pol.decode("utf-8"),
                                      obj.electrical_length_m,
                                      obj.north_m,
                                      obj.east_m,
                                      obj.height_m,
                                      obj.vcs_order,
                                      obj.subfile_order,
                                      obj.flagged,
+                                     digital_gains,
+                                     obj.num_digital_gains,
+                                     dipole_delays,
+                                     obj.num_dipole_delays,
+                                     dipole_gains,
+                                     obj.num_dipole_gains,
                                      obj.rec_number,
                                      obj.rec_slot_number))
 
         return rf_inputs
```

### Comparing `pymwalib-0.8.8/pymwalib/timestep.py` & `pymwalib-0.9.1/pymwalib/timestep.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/version.py` & `pymwalib-0.9.1/pymwalib/version.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/pymwalib/voltage_context.py` & `pymwalib-0.9.1/pymwalib/voltage_context.py`

 * *Files identical despite different names*

### Comparing `pymwalib-0.8.8/setup.py` & `pymwalib-0.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from setuptools import setup
 from distutils.core import setup
 
 # read the contents of your README file
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pymwalib',
     packages=['pymwalib'],
-    version='0.8.8',
+    version='0.9.1',
     license='mpl-2.0',
     description='A Python interface for mwalib, a library to read Murchison Widefield Array (MWA) raw visibilities, '
                 'voltages and metadata into a common structure',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Greg Sleap',
     author_email='greg.sleap@curtin.edu.au',
     url='https://github.com/MWATelescope/pymwalib',
-    download_url='https://github.com/MWATelescope/pymwalib/archive/refs/tags/v0.8.7.tar.gz',
+    download_url='https://github.com/MWATelescope/pymwalib/archive/refs/tags/v0.9.1.tar.gz',
     keywords=['MWA', 'radioastronomy'],
     install_requires=[
         'numpy',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

