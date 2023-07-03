# Comparing `tmp/hpmoc-1.0a2.tar.gz` & `tmp/hpmoc-1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpmoc-1.0a2.tar", last modified: Mon Jul  3 20:55:47 2023, max compression
+gzip compressed data, was "hpmoc-1.0a3.tar", last modified: Mon Jul  3 21:55:15 2023, max compression
```

## Comparing `hpmoc-1.0a2.tar` & `hpmoc-1.0a3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a2/LICENSE
--rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a2/Makefile
--rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a2/README.md
--rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a2/docs/.gitignore
--rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a2/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a2/docs/make.bat
--rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a2/docs/source/conf.py
--rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a2/docs/source/index.rst
--rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a2/docs/source/jup/plotting-examples.ipynb
--rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a2/hpmoc-dev-win.yml
--rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a2/hpmoc-dev.yml
--rw-r--r--   0        0        0     1032 2023-07-03 20:54:26.431625 hpmoc-1.0a2/hpmoc/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a2/hpmoc/abstract.py
--rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a2/hpmoc/healpy.py
--rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a2/hpmoc/healpy_utils.py
--rw-r--r--   0        0        0     6937 2023-07-03 20:16:09.031605 hpmoc-1.0a2/hpmoc/io/__init__.py
--rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a2/hpmoc/io/abstract.py
--rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a2/hpmoc/io/astroquery.py
--rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a2/hpmoc/io/fits.py
--rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a2/hpmoc/io/gracedb.py
--rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a2/hpmoc/io/ligo.py
--rw-r--r--   0        0        0    53956 2023-07-03 20:43:31.691622 hpmoc-1.0a2/hpmoc/partial.py
--rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a2/hpmoc/plot.py
--rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a2/hpmoc/plotters.py
--rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a2/hpmoc/points.py
--rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a2/hpmoc/psf.py
--rw-r--r--   0        0        0    92991 2023-07-03 20:43:05.981627 hpmoc-1.0a2/hpmoc/utils.py
--rw-r--r--   0        0        0     1670 2023-07-03 20:41:04.301624 hpmoc-1.0a2/pyproject.toml
--rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 hpmoc-1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a3/LICENSE
+-rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a3/Makefile
+-rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a3/README.md
+-rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/.gitignore
+-rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/make.bat
+-rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/source/conf.py
+-rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/source/index.rst
+-rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/source/jup/plotting-examples.ipynb
+-rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a3/hpmoc-dev-win.yml
+-rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a3/hpmoc-dev.yml
+-rw-r--r--   0        0        0     1032 2023-07-03 21:54:52.211627 hpmoc-1.0a3/hpmoc/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a3/hpmoc/abstract.py
+-rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a3/hpmoc/healpy.py
+-rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a3/hpmoc/healpy_utils.py
+-rw-r--r--   0        0        0     6949 2023-07-03 21:54:38.341626 hpmoc-1.0a3/hpmoc/io/__init__.py
+-rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a3/hpmoc/io/abstract.py
+-rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a3/hpmoc/io/astroquery.py
+-rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a3/hpmoc/io/fits.py
+-rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a3/hpmoc/io/gracedb.py
+-rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a3/hpmoc/io/ligo.py
+-rw-r--r--   0        0        0    53953 2023-07-03 21:35:31.821599 hpmoc-1.0a3/hpmoc/partial.py
+-rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a3/hpmoc/plot.py
+-rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a3/hpmoc/plotters.py
+-rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a3/hpmoc/points.py
+-rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a3/hpmoc/psf.py
+-rw-r--r--   0        0        0    92991 2023-07-03 20:43:05.981627 hpmoc-1.0a3/hpmoc/utils.py
+-rw-r--r--   0        0        0     1749 2023-07-03 21:06:24.211608 hpmoc-1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     5413 1970-01-01 00:00:00.000000 hpmoc-1.0a3/PKG-INFO
```

### Comparing `hpmoc-1.0a2/LICENSE` & `hpmoc-1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/Makefile` & `hpmoc-1.0a3/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/README.md` & `hpmoc-1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/docs/Makefile` & `hpmoc-1.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/docs/make.bat` & `hpmoc-1.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/docs/source/conf.py` & `hpmoc-1.0a3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/docs/source/index.rst` & `hpmoc-1.0a3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/docs/source/jup/plotting-examples.ipynb` & `hpmoc-1.0a3/docs/source/jup/plotting-examples.ipynb`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc-dev-win.yml` & `hpmoc-1.0a3/hpmoc-dev-win.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc-dev.yml` & `hpmoc-1.0a3/hpmoc-dev.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/__init__.py` & `hpmoc-1.0a3/hpmoc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 """
 HPMOC is an ultra high-performance, cross-platform toolset for working with
 multi-order coordinate (MOC) HEALPix images (i.e. images with multiple pixel
 resolutions).
 """
 
-__version__ = '1.0a2'
+__version__ = '1.0a3'
 
 from .partial import PartialUniqSkymap as PartialUniqSkymap
```

### Comparing `hpmoc-1.0a2/hpmoc/abstract.py` & `hpmoc-1.0a3/hpmoc/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/healpy.py` & `hpmoc-1.0a3/hpmoc/healpy.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/healpy_utils.py` & `hpmoc-1.0a3/hpmoc/healpy_utils.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/io/__init__.py` & `hpmoc-1.0a3/hpmoc/io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             pt = skymap.point_sources
             m = skymap.u
         else:
             pt = []
             m = np.asarray(skymap, dtype=np.int64)
         m = np.unique(m >> (2*min(uniq2order(m.min()), coarsen)))
         p = read_partial_skymap(file, m, memmap=memmap)
-        return PartialUniqSkymap(p[name],
+        return PartialUniqSkymap(np.squeeze(p[name]),
                                  p['UNIQ'],
                                  name=name, meta=p.meta,
                                  point_sources=pt)
 
     @classmethod
     def write(
         cls,
```

### Comparing `hpmoc-1.0a2/hpmoc/io/abstract.py` & `hpmoc-1.0a3/hpmoc/io/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/io/astroquery.py` & `hpmoc-1.0a3/hpmoc/io/astroquery.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/io/fits.py` & `hpmoc-1.0a3/hpmoc/io/fits.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/io/gracedb.py` & `hpmoc-1.0a3/hpmoc/io/gracedb.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/io/ligo.py` & `hpmoc-1.0a3/hpmoc/io/ligo.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/partial.py` & `hpmoc-1.0a3/hpmoc/partial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1204,15 +1204,15 @@
             one_pt = _one_pt(pts, None)
             if one_pt:
                 projs.append('ARC')
                 widths.append(1)
             kwargs = {'projections': projs, 'bottom': 0.1, 'left': 0.04,
                       'missing_color': 'gray'}
             if 'IPython' in sys.modules:
-                from IPython.utils.io.capture import capture_output
+                from IPython.utils.capture import capture_output
 
                 with capture_output():
                     gs, [[ax], *_] = self.gridplot(**kwargs)
             else:
                 gs, [[ax], *_] = self.gridplot(**kwargs)
             if one_pt:
                 for co in ax.coords:
```

### Comparing `hpmoc-1.0a2/hpmoc/plot.py` & `hpmoc-1.0a3/hpmoc/plot.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/plotters.py` & `hpmoc-1.0a3/hpmoc/plotters.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/points.py` & `hpmoc-1.0a3/hpmoc/points.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/psf.py` & `hpmoc-1.0a3/hpmoc/psf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/hpmoc/utils.py` & `hpmoc-1.0a3/hpmoc/utils.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a2/pyproject.toml` & `hpmoc-1.0a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 maintainers = [
     {name = "Albert Zhang", email = "alchzh@gmail.com"}
 ]
 classifiers = [ "Programming Language :: Python :: 3",
  "Framework :: IPython",
  "Framework :: Jupyter",
  "Intended Audience :: Science/Research",
+ "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
  "Natural Language :: English",
  "Programming Language :: Python :: 3 :: Only",
  "Topic :: Scientific/Engineering :: Astronomy",
  "Topic :: Scientific/Engineering :: Information Analysis",
  "Topic :: Scientific/Engineering :: Physics",
  "Topic :: Scientific/Engineering :: Visualization",
  "Topic :: Software Development :: Libraries",
```

### Comparing `hpmoc-1.0a2/PKG-INFO` & `hpmoc-1.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: hpmoc
-Version: 1.0a2
+Version: 1.0a3
 Summary: HPMOC is an ultra high-performance, cross-platform toolset for working with
 Author-email: Stefan Trklja Countryman <stefan.countryman@gmail.com>
 Maintainer-email: Albert Zhang <alchzh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
```

