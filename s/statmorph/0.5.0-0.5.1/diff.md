# Comparing `tmp/statmorph-0.5.0.tar.gz` & `tmp/statmorph-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statmorph-0.5.0.tar", last modified: Fri Jan  6 22:39:39 2023, max compression
+gzip compressed data, was "statmorph-0.5.1.tar", last modified: Tue Jul  4 07:14:14 2023, max compression
```

## Comparing `statmorph-0.5.0.tar` & `statmorph-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.912071 statmorph-0.5.0/
--rw-r--r--   0 vrg       (1000) users      (985)     1528 2023-01-02 20:02:18.000000 statmorph-0.5.0/LICENSE
--rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.0/MANIFEST.in
--rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-01-06 22:39:39.912071 statmorph-0.5.0/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.0/README.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.908738 statmorph-0.5.0/docs/
--rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/Makefile
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.908738 statmorph-0.5.0/docs/_static/
--rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/_static/banner.svg
--rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/_static/favicon.ico
--rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/_static/logo.png
--rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/api.rst
--rw-r--r--   0 vrg       (1000) users      (985)     2613 2023-01-06 20:40:16.000000 statmorph-0.5.0/docs/conf.py
--rw-r--r--   0 vrg       (1000) users      (985)     4210 2023-01-06 20:26:43.000000 statmorph-0.5.0/docs/description.rst
--rw-r--r--   0 vrg       (1000) users      (985)     1412 2023-01-06 19:48:09.000000 statmorph-0.5.0/docs/index.rst
--rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/installation.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.908738 statmorph-0.5.0/docs/notebooks/
--rw-r--r--   0 vrg       (1000) users      (985)    13954 2023-01-06 19:31:51.000000 statmorph-0.5.0/docs/notebooks/tutorial.ipynb
--rw-r--r--   0 vrg       (1000) users      (985)     1884 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/overview.rst
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.0/docs/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.0/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       38 2023-01-06 22:39:39.912071 statmorph-0.5.0/setup.cfg
--rw-r--r--   0 vrg       (1000) users      (985)     1363 2023-01-06 20:39:25.000000 statmorph-0.5.0/setup.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.908738 statmorph-0.5.0/statmorph/
--rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.0/statmorph/__init__.py
--rw-r--r--   0 vrg       (1000) users      (985)    92936 2023-01-06 20:38:59.000000 statmorph-0.5.0/statmorph/statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.908738 statmorph-0.5.0/statmorph/tests/
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.0/statmorph/tests/__init__.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.908738 statmorph-0.5.0/statmorph/tests/data/
--rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.0/statmorph/tests/data/slice.fits
--rw-r--r--   0 vrg       (1000) users      (985)    13959 2023-01-06 18:58:02.000000 statmorph-0.5.0/statmorph/tests/test_statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.912071 statmorph-0.5.0/statmorph/utils/
--rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.0/statmorph/utils/__init__.py
--rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.0/statmorph/utils/image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.912071 statmorph-0.5.0/statmorph/utils/tests/
--rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.0/statmorph/utils/tests/test_image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-01-06 22:39:39.908738 statmorph-0.5.0/statmorph.egg-info/
--rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-01-06 22:39:39.000000 statmorph-0.5.0/statmorph.egg-info/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)      711 2023-01-06 22:39:39.000000 statmorph-0.5.0/statmorph.egg-info/SOURCES.txt
--rw-r--r--   0 vrg       (1000) users      (985)        1 2023-01-06 22:39:39.000000 statmorph-0.5.0/statmorph.egg-info/dependency_links.txt
--rw-r--r--   0 vrg       (1000) users      (985)      103 2023-01-06 22:39:39.000000 statmorph-0.5.0/statmorph.egg-info/requires.txt
--rw-r--r--   0 vrg       (1000) users      (985)       10 2023-01-06 22:39:39.000000 statmorph-0.5.0/statmorph.egg-info/top_level.txt
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/
+-rw-r--r--   0 vrg       (1000) users      (985)     1528 2023-01-02 20:02:18.000000 statmorph-0.5.1/LICENSE
+-rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.1/MANIFEST.in
+-rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-07-04 07:14:14.543779 statmorph-0.5.1/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.1/README.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/docs/
+-rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/Makefile
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/docs/_static/
+-rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/_static/banner.svg
+-rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/_static/favicon.ico
+-rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/_static/logo.png
+-rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/api.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     2613 2023-07-04 06:46:23.000000 statmorph-0.5.1/docs/conf.py
+-rw-r--r--   0 vrg       (1000) users      (985)     4210 2023-01-06 20:26:43.000000 statmorph-0.5.1/docs/description.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     1412 2023-01-06 19:48:09.000000 statmorph-0.5.1/docs/index.rst
+-rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/installation.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/docs/notebooks/
+-rw-r--r--   0 vrg       (1000) users      (985)    13954 2023-01-06 19:31:51.000000 statmorph-0.5.1/docs/notebooks/tutorial.ipynb
+-rw-r--r--   0 vrg       (1000) users      (985)     1884 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/overview.rst
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.1/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       38 2023-07-04 07:14:14.543779 statmorph-0.5.1/setup.cfg
+-rw-r--r--   0 vrg       (1000) users      (985)     1363 2023-07-04 06:44:51.000000 statmorph-0.5.1/setup.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/statmorph/
+-rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/__init__.py
+-rw-r--r--   0 vrg       (1000) users      (985)    97512 2023-07-04 06:45:09.000000 statmorph-0.5.1/statmorph/statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/tests/__init__.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/tests/data/
+-rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/tests/data/slice.fits
+-rw-r--r--   0 vrg       (1000) users      (985)    13959 2023-07-04 02:09:35.000000 statmorph-0.5.1/statmorph/tests/test_statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/utils/
+-rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/utils/__init__.py
+-rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.1/statmorph/utils/image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/utils/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/utils/tests/test_image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph.egg-info/
+-rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)      711 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/SOURCES.txt
+-rw-r--r--   0 vrg       (1000) users      (985)        1 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/dependency_links.txt
+-rw-r--r--   0 vrg       (1000) users      (985)      103 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/requires.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       10 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/top_level.txt
```

### Comparing `statmorph-0.5.0/LICENSE` & `statmorph-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/PKG-INFO` & `statmorph-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `statmorph-0.5.0/README.rst` & `statmorph-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/Makefile` & `statmorph-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/_static/banner.svg` & `statmorph-0.5.1/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/_static/favicon.ico` & `statmorph-0.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/_static/logo.png` & `statmorph-0.5.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/conf.py` & `statmorph-0.5.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'statmorph'
 copyright = '2017-2023, Vicente Rodriguez-Gomez'
 author = 'Vicente Rodriguez-Gomez'
 
 # The full version, including alpha/beta/rc tags
-release = '0.5.0'
+release = '0.5.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `statmorph-0.5.0/docs/description.rst` & `statmorph-0.5.1/docs/description.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/index.rst` & `statmorph-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/installation.rst` & `statmorph-0.5.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/notebooks/tutorial.ipynb` & `statmorph-0.5.1/docs/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/docs/overview.rst` & `statmorph-0.5.1/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/setup.py` & `statmorph-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='statmorph',
-    version='0.5.0',
+    version='0.5.1',
     description='Non-parametric morphological diagnostics of galaxy images',
     long_description=long_description,
     url='https://github.com/vrodgom/statmorph',
     author='Vicente Rodriguez-Gomez',
     author_email='vrodgom.astro@gmail.com',
     license='BSD',
     classifiers=[
```

### Comparing `statmorph-0.5.0/statmorph/statmorph.py` & `statmorph-0.5.1/statmorph/statmorph.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 import skimage.measure
 import skimage.transform
 import skimage.feature
 import skimage.segmentation
 from astropy.utils import lazyproperty
 from astropy.stats import sigma_clipped_stats
 from astropy.modeling import models, fitting
-from astropy.utils.exceptions import AstropyUserWarning
+from astropy.utils.exceptions import (
+    AstropyUserWarning, AstropyDeprecationWarning)
 from astropy.convolution import convolve
 import photutils
 
 __all__ = ['ConvolvedSersic2D', 'SourceMorphology', 'source_morphology',
            '__version__']
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 # A list of all the quantities that are calculated by SourceMorphology:
 _quantity_names = [
     'xc_centroid',
     'yc_centroid',
     'ellipticity_centroid',
     'elongation_centroid',
@@ -134,16 +135,19 @@
     contains a given fraction of the light within ``r_total``.
     """
     flag = 0
 
     ap_total = photutils.aperture.CircularAperture(center, r_total)
 
     total_sum = ap_total.do_photometry(image, method='exact')[0][0]
-    assert total_sum != 0
-    if total_sum < 0:
+    if total_sum == 0:
+        warnings.warn('[r_circ] Total flux sum is zero.', AstropyUserWarning)
+        flag = 2
+        return r_total, flag
+    elif total_sum < 0:
         warnings.warn('[r_circ] Total flux sum is negative.', AstropyUserWarning)
         flag = 2
         total_sum = np.abs(total_sum)
 
     # Find appropriate range for root finder
     npoints = 100
     r_grid = np.linspace(0.0, r_total, num=npoints)
@@ -192,16 +196,19 @@
     flag = 0
 
     b_total = a_total / elongation
     ap_total = photutils.aperture.EllipticalAperture(
         center, a_total, b_total, theta=theta)
 
     total_sum = ap_total.do_photometry(image, method='exact')[0][0]
-    assert total_sum != 0
-    if total_sum < 0:
+    if total_sum == 0:
+        warnings.warn('[r_ellip] Total flux sum is zero.', AstropyUserWarning)
+        flag = 2
+        return a_total, flag
+    elif total_sum < 0:
         warnings.warn('[r_ellip] Total flux sum is negative.', AstropyUserWarning)
         flag = 2
         total_sum = np.abs(total_sum)
 
     # Find appropriate range for root finder
     npoints = 100
     a_grid = np.linspace(0.0, a_total, num=npoints)
@@ -350,17 +357,29 @@
         "radius" of the elliptical aperture used to estimate the sky
         background in the shape asymmetry calculation. Following SDSS,
         the default value is 2.0.
     boxcar_size_shape_asym : float, optional
         When calculating the shape asymmetry segmap, this is the size
         (in pixels) of the constant kernel used to regularize the segmap.
         The default value is 3.0.
+    sersic_fitting_args : dict, optional
+        A dictionary of keyword arguments passed to Astropy's
+        `LevMarLSQFitter`, which cannot include ``z`` or ``weights``
+        (these are handled internally by statmorph). The default is
+        {'maxiter': 500, 'acc': 1e-5}.
+    sersic_model_args : dict, optional
+        A dictionary of keyword arguments passed to Astropy's
+        `Sersic2D`. The default is {'bounds': {'n': (0.01, None)}},
+        which sets a lower bound for the fitted Sersic index.
+        Note that, by default, statmorph will make reasonable
+        initial guesses for all the model parameters (recommended),
+        although this functionality can be overridden for more
+        customized fits.
     sersic_maxiter : int, optional
-        The maximum number of iterations during the Sersic profile
-        fitting.
+        Deprecated. Please use ``sersic_fitting_args`` instead.
     segmap_overlap_ratio : float, optional
         The minimum ratio (in order to have a "good" measurement)
         between the area of the intersection of the Gini and MID segmaps
         and the area of the largest of these two segmaps.
     verbose : bool, optional
         If ``True``, this prints various minor warnings (which do not
         result in "bad" measurements) during the calculations.
@@ -368,21 +387,23 @@
 
     References
     ----------
     See `README.rst` for a list of references.
 
     """
     def __init__(self, image, segmap, label, mask=None, weightmap=None,
-                 gain=None, psf=None, cutout_extent=1.5, min_cutout_size=48,
+                 gain=None, psf=None, cutout_extent=2.5, min_cutout_size=48,
                  n_sigma_outlier=10, annulus_width=1.0,
                  eta=0.2, petro_fraction_gini=0.2, skybox_size=32,
                  petro_extent_cas=1.5, petro_fraction_cas=0.25,
                  boxcar_size_mid=3.0, niter_bh_mid=5, sigma_mid=1.0,
                  petro_extent_flux=2.0, boxcar_size_shape_asym=3.0,
-                 sersic_maxiter=500, segmap_overlap_ratio=0.25, verbose=False):
+                 sersic_fitting_args={'maxiter': 500, 'acc': 1e-5},
+                 sersic_model_args={'bounds': {'n': (0.01, None)}},
+                 sersic_maxiter=None, segmap_overlap_ratio=0.25, verbose=False):
         self._image = image
         self._segmap = segmap
         self.label = label
         self._mask = mask
         self._weightmap = weightmap
         self._gain = gain
         self._psf = psf
@@ -396,24 +417,32 @@
         self._petro_extent_cas = petro_extent_cas
         self._petro_fraction_cas = petro_fraction_cas
         self._boxcar_size_mid = boxcar_size_mid
         self._niter_bh_mid = niter_bh_mid
         self._sigma_mid = sigma_mid
         self._petro_extent_flux = petro_extent_flux
         self._boxcar_size_shape_asym = boxcar_size_shape_asym
-        self._sersic_maxiter = sersic_maxiter
+        self._sersic_fitting_args = sersic_fitting_args.copy()
+        self._sersic_model_args = sersic_model_args.copy()
         self._segmap_overlap_ratio = segmap_overlap_ratio
         self._verbose = verbose
 
         # Measure runtime
         start = time.time()
 
         if not isinstance(self._segmap, photutils.segmentation.SegmentationImage):
             self._segmap = photutils.segmentation.SegmentationImage(self._segmap)
 
+        # Check deprecated arguments
+        if sersic_maxiter is not None:
+            warnings.warn(
+                "The argument sersic_maxiter is deprecated. Please use "
+                "sersic_fitting_args instead.", AstropyDeprecationWarning)
+            self._sersic_fitting_args['maxiter'] = sersic_maxiter
+
         # Check sanity of input data
         self._segmap.check_labels([self.label])
         assert self._segmap.data.shape == self._image.shape
         if self._mask is not None:
             assert self._mask.shape == self._image.shape
             assert self._mask.dtype == np.bool_
         if self._weightmap is not None:
@@ -2315,88 +2344,148 @@
     # SERSIC MODEL FIT #
     ####################
 
     @lazyproperty
     def _sersic_model(self):
         """
         Fit a 2D Sersic profile using Astropy's model fitting library.
+        An initial guess for the Sersic model will be generated based on
+        other statmorph measurements, although users can provide their
+        own initial values (and optionally keep them fixed) via the
+        ``sersic_model_args`` keyword argument.
+
         Return the fitted model object.
         """
         image = self._cutout_stamp_maskzeroed
         ny, nx = image.shape
-        center = self._asymmetry_center
-        theta = self.orientation_asymmetry
 
-        # Get flux at the "effective radius"
-        a_in = self.rhalf_ellip - 0.5 * self._annulus_width
-        a_out = self.rhalf_ellip + 0.5 * self._annulus_width
+        # Start from approximate relation between n and concentration
+        empirical_n = 10.0**(-1.5) * self.concentration**3.5
+        empirical_n = min(max(empirical_n, 1.0), 3.5)  # limit to range [1, 3.5]
+
+        # Create initial guesses for some model parameters (amplitude later)
+        if 'r_eff' not in self._sersic_model_args:
+            self._sersic_model_args['r_eff'] = self.rhalf_ellip
+        if 'n' not in self._sersic_model_args:
+            self._sersic_model_args['n'] = empirical_n
+        if 'x_0' not in self._sersic_model_args:
+            self._sersic_model_args['x_0'] = self.xc_asymmetry
+        if 'y_0' not in self._sersic_model_args:
+            self._sersic_model_args['y_0'] = self.yc_asymmetry
+        if 'ellip' not in self._sersic_model_args:
+            self._sersic_model_args['ellip'] = self.ellipticity_asymmetry
+        if 'theta' not in self._sersic_model_args:
+            self._sersic_model_args['theta'] = self.orientation_asymmetry
+
+        # Get position of center with respect to image cutout
+        self._sersic_model_args['x_0'] -= self.xmin_stamp
+        self._sersic_model_args['y_0'] -= self.ymin_stamp
+
+        # For readability
+        guess_r_eff = self._sersic_model_args['r_eff']
+        guess_center = np.array([self._sersic_model_args['x_0'],
+                                 self._sersic_model_args['y_0']])
+        guess_ellip = self._sersic_model_args['ellip']
+        guess_theta = self._sersic_model_args['theta']
+
+        # Get mean flux at the effective "radius"
+        a_in = guess_r_eff - 0.5 * self._annulus_width
+        a_out = guess_r_eff + 0.5 * self._annulus_width
         if a_in < 0:
-            warnings.warn('[sersic] rhalf_ellip < annulus_width.',
+            warnings.warn('[sersic] guess_r_eff < annulus_width.',
                           AstropyUserWarning)
             self.flag_sersic = 1
-            a_in = self.rhalf_ellip
-        b_out = a_out / self.elongation_asymmetry
+            a_in = guess_r_eff
+        b_out = (1 - guess_ellip) * a_out
         ellip_annulus = photutils.aperture.EllipticalAnnulus(
-            center, a_in, a_out, b_out, theta=theta)
+            guess_center, a_in, a_out, b_out, theta=guess_theta)
         ellip_annulus_mean_flux = _aperture_mean_nomask(
             ellip_annulus, image, method='exact')
         if ellip_annulus_mean_flux <= 0.0:
             warnings.warn('[sersic] Nonpositive flux at r_e.', AstropyUserWarning)
             self.flag_sersic = 1
             ellip_annulus_mean_flux = np.abs(ellip_annulus_mean_flux)
 
+        # Final parameter
+        if 'amplitude' not in self._sersic_model_args:
+            self._sersic_model_args['amplitude'] = ellip_annulus_mean_flux
+
+        # Create initial model
+        if self._psf is None:
+            sersic_init = models.Sersic2D(**self._sersic_model_args)
+        else:
+            sersic_init = ConvolvedSersic2D(**self._sersic_model_args)
+            sersic_init.set_psf(self._psf)
+
         # Prepare data for fitting
         z = image.copy()
         y, x = np.mgrid[0:ny, 0:nx]
         weightmap = self._weightmap_stamp
         # Exclude pixels with image == 0 or weightmap == 0 from the fit.
         fit_weights = np.zeros_like(z)
         locs = (image != 0) & (weightmap != 0)
         # The sky background noise is already included in the weightmap:
         fit_weights[locs] = 1.0 / weightmap[locs]
 
-        # Initial guess
-        guess_n = 10.0**(-1.5) * self.concentration**3.5  # empirical
-        guess_n = min(max(guess_n, 1.0), 3.5)  # limit to range [1.0, 3.5]
-        xc, yc = self._asymmetry_center
-        if self._psf is None:
-            sersic_init = models.Sersic2D(
-                amplitude=ellip_annulus_mean_flux, r_eff=self.rhalf_ellip,
-                n=guess_n, x_0=xc, y_0=yc, ellip=self.ellipticity_asymmetry, theta=theta)
-        else:
-            sersic_init = ConvolvedSersic2D(
-                amplitude=ellip_annulus_mean_flux, r_eff=self.rhalf_ellip,
-                n=guess_n, x_0=xc, y_0=yc, ellip=self.ellipticity_asymmetry, theta=theta)
-            sersic_init.set_psf(self._psf)
-
         # The number of data points cannot be smaller than the number of
         # free parameters (7 in the case of Sersic2D)
         if z.size < sersic_init.parameters.size:
             warnings.warn('[sersic] Not enough data for fit.',
                           AstropyUserWarning)
             self.flag_sersic = 1
             return sersic_init
 
         # Since model fitting can be computationally expensive (especially
         # with a large PSF), only do it when the other measurements are OK.
-        if self.flag == 2:
+        if self.flag >= 2:
             warnings.warn('[sersic] Skipping Sersic fit...',
                           AstropyUserWarning)
             self.flag_sersic = 1
             return sersic_init
 
         # Try to fit model
         fit_sersic = fitting.LevMarLSQFitter()
-        sersic_model = fit_sersic(sersic_init, x, y, z, weights=fit_weights,
-                                  maxiter=self._sersic_maxiter, acc=1e-5)
+        sersic_model = fit_sersic(sersic_init, x, y, z=z, weights=fit_weights,
+                                  **self._sersic_fitting_args)
         if fit_sersic.fit_info['ierr'] not in [1, 2, 3, 4]:
             warnings.warn("fit_info['message']: " + fit_sersic.fit_info['message'],
                           AstropyUserWarning)
             self.flag_sersic = 1
 
+        # Make sure the effective radius is positive:
+        if sersic_model.r_eff.value <= 0:
+            warnings.warn('[sersic] Nonpositive effective radius?',
+                          AstropyUserWarning)
+            self.flag_sersic = 1
+            return sersic_init
+
+        # In some rare cases, the fitted ellipticity is outside the
+        # range [0, 1]. While we could constrain this parameter during
+        # the fit using the ``bounds`` keyword argument in `Sersic2D`, a less
+        # aggressive solution is to create an equivalent model as follows:
+        if sersic_model.ellip.value > 1:
+            # Note that the semiminor axis is given by
+            # b = (1 - ellip) * a.
+            # This would yield a negative value for b, but since only b^2
+            # appears in the code, we can define an equivalent ellipticity as
+            # 1 - ellip' = -(1 - ellip)  =>  ellip' = 2 - ellip.
+            sersic_model.ellip.value = 2.0 - sersic_model.ellip.value
+        if sersic_model.ellip.value < 0:
+            # This can be interpreted as a, b being flipped (a < b), so we
+            # switch them and define an equivalent ellipticity as
+            # 1 - ellip' = 1 / (1 - ellip)  =>  ellip' = ellip / (ellip - 1).
+            e = sersic_model.ellip.value
+            sersic_model.r_eff.value = (1 - e) * sersic_model.r_eff.value
+            sersic_model.ellip.value = e / (e - 1)
+            # We also need to rotate the model by 90 degrees:
+            sersic_model.theta.value += np.pi/2
+        # Finally, note that the two cases above are not mutually exclusive.
+        # If a Sersic model has ellipticity > 2, then both "corrections" are
+        # applied successively.
+
         return sersic_model
 
     @lazyproperty
     def sersic_amplitude(self):
         """
         The amplitude of the 2D Sersic fit at the effective (half-light)
         radius (`astropy.modeling.models.Sersic2D`).
```

### Comparing `statmorph-0.5.0/statmorph/tests/data/slice.fits` & `statmorph-0.5.1/statmorph/tests/data/slice.fits`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/statmorph/tests/test_statmorph.py` & `statmorph-0.5.1/statmorph/tests/test_statmorph.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/statmorph/utils/image_diagnostics.py` & `statmorph-0.5.1/statmorph/utils/image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/statmorph/utils/tests/test_image_diagnostics.py` & `statmorph-0.5.1/statmorph/utils/tests/test_image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.0/statmorph.egg-info/PKG-INFO` & `statmorph-0.5.1/statmorph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `statmorph-0.5.0/statmorph.egg-info/SOURCES.txt` & `statmorph-0.5.1/statmorph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

