# Comparing `tmp/bipl-0.3.1.tar.gz` & `tmp/bipl-0.3.2.tar.gz`

## Comparing `bipl-0.3.1.tar` & `bipl-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_gdal.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    14028 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/io/_util.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.3.1/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.1/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.1/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.1/hatch_build.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 bipl-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 bipl-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/_env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_gdal.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    14028 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_util.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.2/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.2/hatch_build.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 bipl-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 bipl-0.3.2/PKG-INFO
```

### Comparing `bipl-0.3.1/src/bipl/io/__init__.py` & `bipl-0.3.2/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/io/_dzi.py` & `bipl-0.3.2/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/io/_gdal.py` & `bipl-0.3.2/src/bipl/io/_gdal.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/io/_libs.py` & `bipl-0.3.2/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/io/_openslide.py` & `bipl-0.3.2/src/bipl/io/_openslide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/io/_slide.py` & `bipl-0.3.2/src/bipl/io/_slide.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,42 +7,43 @@
 from pathlib import Path
 from typing import final
 
 import cv2
 import numpy as np
 from glow import memoize, shared_call, weak_memoize
 
+from bipl import env
+
 from ._openslide import Openslide
 from ._slide_bases import REGISTRY, Driver, Item, Lod, normalize
 from ._tiff import Tiff
 
 # TODO: inside Slide.open import ._slide.registry,
 # TODO: and in ._slide.registry do registration and DLL loading
 # TODO: to make Slide export not require DLL presence
 
 try:
     from ._gdal import Gdal
 except ImportError:
     Gdal = None  # type: ignore[assignment,misc]
 
+_drv: type[Driver] | None
 for _drv, _regex in [  # LIFO, last driver takes priority
     (Gdal, r'^.*\.(tif|tiff)$'),
     (Openslide, r'^.*\.(bif|mrxs|ndpi|scn|svs|svsslide|tif|tiff|vms|vmu)$'),
     (Tiff, r'^.*\.(svs|tif|tiff)$'),
     (Gdal, r'^(/vsicurl.*|(http|https)://.*)$'),
 ]:
-    if _drv is not None:
+    if _drv is not None and _drv.__name__.lower() in env.BIPL_DRIVERS:
         _drv.register(_regex)
 
-_MAX_BYTES = int(os.environ.get('GLOW_SLIDE_BYTES') or 102_400)
-
 
 @shared_call  # merge duplicate calls
 @weak_memoize  # reuse result if it's already exist, but used by someone else
-@memoize(capacity=_MAX_BYTES, policy='lru')  # keep LRU for unused results
+@memoize(capacity=env.BIPL_CACHE, policy='lru')  # keep LRU for unused results
 def _cached_open(path: str) -> Slide:
     last_exc = BaseException()
     matches = (tp for pat, tps_ in REGISTRY.items() if pat.match(path)
                for tp in tps_)
     tps = [*dict.fromkeys(matches)]
     if tps:
         for tp in reversed(tps):  # Loop over types to find non-failing
```

### Comparing `bipl-0.3.1/src/bipl/io/_slide_bases.py` & `bipl-0.3.2/src/bipl/io/_slide_bases.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/io/_tiff.py` & `bipl-0.3.2/src/bipl/io/_tiff.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/io/_util.py` & `bipl-0.3.2/src/bipl/io/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/ops/_mosaic.py` & `bipl-0.3.2/src/bipl/ops/_mosaic.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/src/bipl/ops/_util.py` & `bipl-0.3.2/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/LICENSE` & `bipl-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/README.md` & `bipl-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/hatch_build.py` & `bipl-0.3.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.1/pyproject.toml` & `bipl-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.3.1"
+version = "0.3.2"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -36,23 +36,23 @@
 
 dependencies = [
     "glow~=0.12.7",
     "imagecodecs",
     "lxml",
     "numpy~=1.21",
     "opencv-python~=4.0",
+    "pydantic~=1.2",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 gdal = [
     # For Windows, pick GDAL from here https://www.lfd.uci.edu/~gohlke/pythonlibs/#gdal and install manually
     # "gdal @ https://download.lfd.uci.edu/pythonlibs/archived/GDAL-3.4.3-cp310-cp310-win_amd64.whl ; python_version == '3.10' and platform_system == 'Windows'",
-    "gdal~=3.4.3",
-    "pydantic~=1.2",
+    "gdal~=3.0",
 ]
 dev-core = [
     "flake8~=6.0.0",
     "flake8-pie",
     "flake8-pyi",
     "flake8-pyproject",
     "flake8-simplify",
```

### Comparing `bipl-0.3.1/PKG-INFO` & `bipl-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.3.1
+Version: 0.3.2
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
@@ -38,14 +38,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: glow~=0.12.7
 Requires-Dist: imagecodecs
 Requires-Dist: lxml
 Requires-Dist: numpy~=1.21
 Requires-Dist: opencv-python~=4.0
+Requires-Dist: pydantic~=1.2
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: bipl[dev-core]; extra == 'dev'
 Requires-Dist: flake8-alphabetize; extra == 'dev'
 Requires-Dist: typing-extensions~=4.6; extra == 'dev'
 Provides-Extra: dev-core
 Requires-Dist: flake8-pie; extra == 'dev-core'
@@ -58,16 +59,15 @@
 Requires-Dist: pytest~=7.3; extra == 'dev-core'
 Requires-Dist: ruff~=0.0.270; extra == 'dev-core'
 Requires-Dist: yapf~=0.33.0; extra == 'dev-core'
 Provides-Extra: dev-wemake
 Requires-Dist: bipl[dev-core]; extra == 'dev-wemake'
 Requires-Dist: wemake-python-styleguide~=0.15.0; extra == 'dev-wemake'
 Provides-Extra: gdal
-Requires-Dist: gdal~=3.4.3; extra == 'gdal'
-Requires-Dist: pydantic~=1.2; extra == 'gdal'
+Requires-Dist: gdal~=3.0; extra == 'gdal'
 Description-Content-Type: text/markdown
 
 # BIPL is a Big Image Python Library
 
 Library to read big pyramidal images like in formats like BigTiff, Aperio SVS, Leica MRXS.
 
 ## `bipl.Slide` - ndarray-like reader for multiscale images (svs, tiff, etc...)
```

