# Comparing `tmp/ndbioimage-2023.6.1.tar.gz` & `tmp/ndbioimage-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2023.6.1.tar", max compression
+gzip compressed data, was "ndbioimage-2023.7.0.tar", max compression
```

## Comparing `ndbioimage-2023.6.1.tar` & `ndbioimage-2023.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2023.6.1/LICENSE
--rw-r--r--   0        0        0     2418 2023-06-29 12:27:04.230942 ndbioimage-2023.6.1/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2023.6.1/ndbioimage/.DS_Store
--rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2023.6.1/ndbioimage/AiryScan.xml
--rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2023.6.1/ndbioimage/Elyra_test.xml
--rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2023.6.1/ndbioimage/Elyra_test2.xml
--rwxr-xr-x   0        0        0    55945 2023-06-29 12:01:13.598678 ndbioimage-2023.6.1/ndbioimage/__init__.py
--rw-r--r--   0        0        0     7736 2022-08-01 13:44:51.766744 ndbioimage-2023.6.1/ndbioimage/bf.py
--rw-r--r--   0        0        0     1749 2023-06-29 11:31:54.170380 ndbioimage-2023.6.1/ndbioimage/jvm.py
--rw-r--r--   0        0        0     8677 2023-05-25 09:24:53.290471 ndbioimage-2023.6.1/ndbioimage/ntransforms.py
--rw-r--r--   0        0        0      146 2023-05-25 09:20:54.527861 ndbioimage-2023.6.1/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8187 2023-06-29 12:01:13.546678 ndbioimage-2023.6.1/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    22889 2023-05-26 07:14:19.001535 ndbioimage-2023.6.1/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     1990 2023-06-02 11:04:25.198511 ndbioimage-2023.6.1/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     5302 2023-05-25 14:09:31.628409 ndbioimage-2023.6.1/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     2657 2023-06-12 12:28:43.438524 ndbioimage-2023.6.1/ndbioimage/readers/tifread.py
--rwxr-xr-x   0        0        0      245 2022-08-16 10:57:07.482485 ndbioimage-2023.6.1/ndbioimage/test.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2023.6.1/ndbioimage/transform.txt
--rw-r--r--   0        0        0     9609 2023-05-24 14:11:27.082389 ndbioimage-2023.6.1/ndbioimage/transforms.py
--rw-r--r--   0        0        0      805 2023-06-29 12:31:28.546990 ndbioimage-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 ndbioimage-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2023.7.0/LICENSE
+-rw-r--r--   0        0        0     2356 2023-07-04 14:24:16.158015 ndbioimage-2023.7.0/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2023.7.0/ndbioimage/.DS_Store
+-rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2023.7.0/ndbioimage/AiryScan.xml
+-rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2023.7.0/ndbioimage/Elyra_test.xml
+-rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2023.7.0/ndbioimage/Elyra_test2.xml
+-rwxr-xr-x   0        0        0    55988 2023-07-04 13:53:41.286790 ndbioimage-2023.7.0/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     7736 2022-08-01 13:44:51.766744 ndbioimage-2023.7.0/ndbioimage/bf.py
+-rw-r--r--   0        0        0     1749 2023-06-29 11:31:54.170380 ndbioimage-2023.7.0/ndbioimage/jvm.py
+-rw-r--r--   0        0        0     8677 2023-05-25 09:24:53.290471 ndbioimage-2023.7.0/ndbioimage/ntransforms.py
+-rw-r--r--   0        0        0      146 2023-05-25 09:20:54.527861 ndbioimage-2023.7.0/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8187 2023-06-29 12:01:13.546678 ndbioimage-2023.7.0/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    22889 2023-05-26 07:14:19.001535 ndbioimage-2023.7.0/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     1990 2023-06-02 11:04:25.198511 ndbioimage-2023.7.0/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     5580 2023-07-04 14:24:16.118015 ndbioimage-2023.7.0/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     2657 2023-06-12 12:28:43.438524 ndbioimage-2023.7.0/ndbioimage/readers/tifread.py
+-rwxr-xr-x   0        0        0      245 2022-08-16 10:57:07.482485 ndbioimage-2023.7.0/ndbioimage/test.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2023.7.0/ndbioimage/transform.txt
+-rw-r--r--   0        0        0     9609 2023-05-24 14:11:27.082389 ndbioimage-2023.7.0/ndbioimage/transforms.py
+-rw-r--r--   0        0        0      805 2023-07-04 14:17:45.106181 ndbioimage-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 ndbioimage-2023.7.0/PKG-INFO
```

### Comparing `ndbioimage-2023.6.1/LICENSE` & `ndbioimage-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/README.md` & `ndbioimage-2023.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 # ndbioimage - Work in progress
 
 Exposes (bio) images as a numpy ndarray-like-object, but without loading the whole
-image into memory, reading from the file only when needed. Some metadata is read and
+image into memory, reading from the file only when needed. Some metadata is read
 and stored in an ome structure. Additionally, it can automatically calculate an affine
 transform that corrects for chromatic abberrations etc. and apply it on the fly to the image.
 
-Currently supports imagej tif files, czi files, micromanager tif sequences and anything
+Currently, supports imagej tif files, czi files, micromanager tif sequences and anything
 bioformats can handle. 
 
 ## Installation
 
-    pip install ndbioimage@git+https://github.com/wimpomp/ndbioimage.git
-
+```
+pip install ndbioimage
+```
 
 ## Usage
 
 - Reading an image file and plotting the frame at channel=2, time=1
 
-
-    import matplotlib.pyplot as plt
-    from ndbioimage import Imread
-    with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
-        plt.imshow(im[2, 1])
-
+```
+import matplotlib.pyplot as plt
+from ndbioimage import Imread
+with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
+    plt.imshow(im[2, 1])
+```        
+        
 - Showing some image metadata
 
-
-    from ndbioimage import Imread
-    from pprint import pprint
-    with Imread('image_file.tif') as im:
-        pprint(im)
+```
+from ndbioimage import Imread
+from pprint import pprint
+with Imread('image_file.tif') as im:
+    pprint(im)
+```
 
 - Slicing the image without loading the image into memory
 
-
-    from ndbioimage import Imread
-    with Imread('image_file.tif', axes='cztxy') as im:
-        sliced_im = im[1, :, :, 100:200, 100:200]
+```
+from ndbioimage import Imread
+with Imread('image_file.tif', axes='cztxy') as im:
+    sliced_im = im[1, :, :, 100:200, 100:200]
+```
 
 sliced_im is an instance of Imread which will load any image data from file only when needed
 
 
 - Converting (part) of the image to a numpy ndarray
 
-
-    from ndbioimage import Imread
-    import numpy as np
-    with Imread('image_file.tif', axes='cztxy') as im:
-        array = np.asarray(im[0, 0])
+```
+from ndbioimage import Imread
+import numpy as np
+with Imread('image_file.tif', axes='cztxy') as im:
+    array = np.asarray(im[0, 0])
+```
 
 ## Adding more formats
 Readers for image formats subclass Imread. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 subclass Imread and are required to implement the following methods:
 
 - staticmethod _can_open(path): return True if path can be opened by this reader
```

### Comparing `ndbioimage-2023.6.1/ndbioimage/.DS_Store` & `ndbioimage-2023.7.0/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/AiryScan.xml` & `ndbioimage-2023.7.0/ndbioimage/AiryScan.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/Elyra_test.xml` & `ndbioimage-2023.7.0/ndbioimage/Elyra_test.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/Elyra_test2.xml` & `ndbioimage-2023.7.0/ndbioimage/Elyra_test2.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/__init__.py` & `ndbioimage-2023.7.0/ndbioimage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,14 +535,15 @@
             self.objective = find(instrument.objectives, id=self.ome.images[0].objective_settings.id)
         else:
             self.objective = None
         self.timeval = [find(image.pixels.planes, the_c=0, the_t=t, the_z=0).delta_t for t in range(self.shape['t'])]
         self.timeinterval = np.diff(self.timeval).mean() if len(self.timeval) > 1 else 0
         try:
             self.binning = [int(i) for i in image.pixels.channels[0].detector_settings.binning.value.split('x')]
+            self.pxsize *= self.binning[0]
         except (Exception,):
             self.binning = None
         self.cnamelist = [channel.name for channel in image.pixels.channels]
         optovars = [objective for objective in instrument.objectives if 'tubelens' in objective.id.lower()]
         if len(optovars) == 0:
             self.tubelens = None
         else:
```

### Comparing `ndbioimage-2023.6.1/ndbioimage/bf.py` & `ndbioimage-2023.7.0/ndbioimage/bf.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/jvm.py` & `ndbioimage-2023.7.0/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/ntransforms.py` & `ndbioimage-2023.7.0/ndbioimage/ntransforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/readers/bfread.py` & `ndbioimage-2023.7.0/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/readers/cziread.py` & `ndbioimage-2023.7.0/ndbioimage/readers/cziread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/readers/ndread.py` & `ndbioimage-2023.7.0/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/readers/seqread.py` & `ndbioimage-2023.7.0/ndbioimage/readers/seqread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-from abc import ABC
-
 import tifffile
 import yaml
 import re
 from ndbioimage import Imread
 from pathlib import Path
 from functools import cached_property
 from ome_types import model
 from itertools import product
 from datetime import datetime
+from abc import ABC
+from parfor import pmap
 
 
 class Reader(Imread, ABC):
     priority = 10
 
     @staticmethod
     def _can_open(path):
         return isinstance(path, Path) and path.suffix == ""
 
-    def get_metadata(self, c, z, t):
-        with tifffile.TiffFile(self.filedict[c, z, t]) as tif:
-            return {key: yaml.safe_load(value) for key, value in tif.pages[0].tags[50839].value.items()}
-
     @cached_property
     def ome(self):
         ome = model.OME()
-        metadata = self.get_metadata(0, 0, 0)
+        with tifffile.TiffFile(self.filedict[0, 0, 0]) as tif:
+            metadata = {key: yaml.safe_load(value) for key, value in tif.pages[0].tags[50839].value.items()}
         ome.experimenters.append(
             model.Experimenter(id="Experimenter:0", user_name=metadata["Info"]["Summary"]["UserName"]))
         objective_str = metadata["Info"]["ZeissObjectiveTurret-Label"]
         ome.instruments.append(model.Instrument())
         ome.instruments[0].objectives.append(
             model.Objective(
                 id="Objective:0", manufacturer="Zeiss", model=objective_str,
@@ -63,20 +60,28 @@
             model.Image(
                 pixels=model.Pixels(
                     size_c=size_c, size_z=size_z, size_t=size_t,
                     size_x=metadata['Info']['Width'], size_y=metadata['Info']['Height'],
                     dimension_order="XYCZT", type=pixel_type, physical_size_x=pxsize, physical_size_y=pxsize,
                     physical_size_z=metadata["Info"]["Summary"]["z-step_um"]),
                 objective_settings=model.ObjectiveSettings(id="Objective:0")))
-        for c, z, t in product(range(size_c), range(size_z), range(size_t)):
+
+        def timeval_fun(i):
+            with tifffile.TiffFile(self.filedict[i]) as tif:
+                info = yaml.safe_load(tif.pages[0].tags[50839].value['Info'])
+            return (datetime.strptime(info["Time"], "%Y-%m-%d %H:%M:%S %z") - t0).seconds
+
+        length = size_c * size_z * size_t
+        timeval = pmap(timeval_fun, product(range(size_c), range(size_z), range(size_t)), length=length,
+                       serial=length <= 24, desc='Reading metadata')
+
+        for (c, z, t), time in zip(product(range(size_c), range(size_z), range(size_t)), timeval):
             ome.images[0].pixels.planes.append(
                 model.Plane(
-                    the_c=c, the_z=z, the_t=t, exposure_time=metadata["Info"]["Exposure-ms"] / 1000,
-                    delta_t=(datetime.strptime(self.get_metadata(c, z, t)["Info"]["Time"],
-                                               "%Y-%m-%d %H:%M:%S %z") - t0).seconds))
+                    the_c=c, the_z=z, the_t=t, exposure_time=metadata["Info"]["Exposure-ms"] / 1000, delta_t=time))
 
         # compare channel names from metadata with filenames
         pattern_c = re.compile(r"img_\d{3,}_(.*)_\d{3,}$")
         for c in range(size_c):
             ome.images[0].pixels.channels.append(
                 model.Channel(
                     id=f"Channel:{c}", name=pattern_c.findall(self.filedict[c, 0, 0].stem)[0],
@@ -95,16 +100,16 @@
         with tifffile.TiffFile(self.path / filelist[0]) as tif:
             metadata = {key: yaml.safe_load(value) for key, value in tif.pages[0].tags[50839].value.items()}
 
         # compare channel names from metadata with filenames
         cnamelist = metadata["Info"]["Summary"]["ChNames"]
         cnamelist = [c for c in cnamelist if any([c in f.name for f in filelist])]
 
-        pattern_t = re.compile(r"img_(\d{3,})")
         pattern_c = re.compile(r"img_\d{3,}_(.*)_\d{3,}$")
         pattern_z = re.compile(r"(\d{3,})$")
-        self.filedict = {(int(pattern_t.findall(file.stem)[0]),
+        pattern_t = re.compile(r"img_(\d{3,})")
+        self.filedict = {(cnamelist.index(pattern_c.findall(file.stem)[0]),
                           int(pattern_z.findall(file.stem)[0]),
-                          cnamelist.index(pattern_c.findall(file.stem)[0])): file for file in filelist}
+                          int(pattern_t.findall(file.stem)[0])): file for file in filelist}
 
     def __frame__(self, c=0, z=0, t=0):
         return tifffile.imread(self.path / self.filedict[(c, z, t)])
```

### Comparing `ndbioimage-2023.6.1/ndbioimage/readers/tifread.py` & `ndbioimage-2023.7.0/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/ndbioimage/transforms.py` & `ndbioimage-2023.7.0/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.6.1/pyproject.toml` & `ndbioimage-2023.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2023.6.1"
+version = "2023.7.0"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2023.6.1/PKG-INFO` & `ndbioimage-2023.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.8,<4.0
@@ -31,61 +31,66 @@
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/wimpomp/ndbioimage
 Description-Content-Type: text/markdown
 
 # ndbioimage - Work in progress
 
 Exposes (bio) images as a numpy ndarray-like-object, but without loading the whole
-image into memory, reading from the file only when needed. Some metadata is read and
+image into memory, reading from the file only when needed. Some metadata is read
 and stored in an ome structure. Additionally, it can automatically calculate an affine
 transform that corrects for chromatic abberrations etc. and apply it on the fly to the image.
 
-Currently supports imagej tif files, czi files, micromanager tif sequences and anything
+Currently, supports imagej tif files, czi files, micromanager tif sequences and anything
 bioformats can handle. 
 
 ## Installation
 
-    pip install ndbioimage@git+https://github.com/wimpomp/ndbioimage.git
-
+```
+pip install ndbioimage
+```
 
 ## Usage
 
 - Reading an image file and plotting the frame at channel=2, time=1
 
-
-    import matplotlib.pyplot as plt
-    from ndbioimage import Imread
-    with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
-        plt.imshow(im[2, 1])
-
+```
+import matplotlib.pyplot as plt
+from ndbioimage import Imread
+with Imread('image_file.tif', axes='ctxy', dtype=int) as im:
+    plt.imshow(im[2, 1])
+```        
+        
 - Showing some image metadata
 
-
-    from ndbioimage import Imread
-    from pprint import pprint
-    with Imread('image_file.tif') as im:
-        pprint(im)
+```
+from ndbioimage import Imread
+from pprint import pprint
+with Imread('image_file.tif') as im:
+    pprint(im)
+```
 
 - Slicing the image without loading the image into memory
 
-
-    from ndbioimage import Imread
-    with Imread('image_file.tif', axes='cztxy') as im:
-        sliced_im = im[1, :, :, 100:200, 100:200]
+```
+from ndbioimage import Imread
+with Imread('image_file.tif', axes='cztxy') as im:
+    sliced_im = im[1, :, :, 100:200, 100:200]
+```
 
 sliced_im is an instance of Imread which will load any image data from file only when needed
 
 
 - Converting (part) of the image to a numpy ndarray
 
-
-    from ndbioimage import Imread
-    import numpy as np
-    with Imread('image_file.tif', axes='cztxy') as im:
-        array = np.asarray(im[0, 0])
+```
+from ndbioimage import Imread
+import numpy as np
+with Imread('image_file.tif', axes='cztxy') as im:
+    array = np.asarray(im[0, 0])
+```
 
 ## Adding more formats
 Readers for image formats subclass Imread. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 subclass Imread and are required to implement the following methods:
 
 - staticmethod _can_open(path): return True if path can be opened by this reader
```

