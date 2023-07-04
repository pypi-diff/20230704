# Comparing `tmp/pyzjr-0.0.7.tar.gz` & `tmp/pyzjr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-0.0.7.tar", last modified: Sun Jul  2 08:17:51 2023, max compression
+gzip compressed data, was "dist\pyzjr-0.0.8.tar", last modified: Tue Jul  4 16:18:29 2023, max compression
```

## Comparing `pyzjr-0.0.7.tar` & `pyzjr-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 08:17:51.000000 pyzjr-0.0.7/
--rw-rw-rw-   0        0        0      734 2023-07-02 08:17:51.000000 pyzjr-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-07-02 08:17:25.000000 pyzjr-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr/
--rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-0.0.7/pyzjr/ColorModule.py
--rw-rw-rw-   0        0        0    18261 2023-07-02 08:05:42.000000 pyzjr-0.0.7/pyzjr/Enimage.py
--rw-rw-rw-   0        0        0     3624 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/PIC.py
--rw-rw-rw-   0        0        0     4538 2023-07-02 08:05:25.000000 pyzjr-0.0.7/pyzjr/TrackBar.py
--rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/Z.py
--rw-rw-rw-   0        0        0     1071 2023-07-02 08:17:00.000000 pyzjr-0.0.7/pyzjr/__init__.py
--rw-rw-rw-   0        0        0     5022 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/definition.py
--rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/utils.py
--rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/video.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/
--rw-rw-rw-   0        0        0      734 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 08:17:51.000000 pyzjr-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1734 2023-07-02 08:17:03.000000 pyzjr-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:18:29.000000 pyzjr-0.0.8/
+-rw-rw-rw-   0        0        0     1515 2023-07-04 16:18:29.000000 pyzjr-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-07-04 16:18:21.000000 pyzjr-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr/
+-rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-0.0.8/pyzjr/ColorModule.py
+-rw-rw-rw-   0        0        0    18267 2023-07-04 09:37:15.000000 pyzjr-0.0.8/pyzjr/Enimage.py
+-rw-rw-rw-   0        0        0     3624 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-0.0.8/pyzjr/TrackBar.py
+-rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/Z.py
+-rw-rw-rw-   0        0        0     1330 2023-07-04 16:03:33.000000 pyzjr-0.0.8/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     5028 2023-07-04 09:36:12.000000 pyzjr-0.0.8/pyzjr/definition.py
+-rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.8/pyzjr/video.py
+-rw-rw-rw-   0        0        0     2334 2023-07-04 09:41:55.000000 pyzjr-0.0.8/pyzjr/zmath.py
+drwxrwxrwx   0        0        0        0 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     1515 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 16:18:29.000000 pyzjr-0.0.8/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 16:18:29.000000 pyzjr-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2023-07-04 09:41:57.000000 pyzjr-0.0.8/setup.py
```

### Comparing `pyzjr-0.0.7/pyzjr/ColorModule.py` & `pyzjr-0.0.8/pyzjr/ColorModule.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.7/pyzjr/Enimage.py` & `pyzjr-0.0.8/pyzjr/Enimage.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     - 图像修补 ： repair_Img
 """
 import numpy as np
 import cv2
 import pyzjr.utils as zjr
 from pyzjr.utils import empty
 import random
-import TrackBar as Trace
+import pyzjr.TrackBar as Trace
 import pyzjr.Z as Z
 
 class Filter():
     def median_filtering(self, img,ksize=3):
         """
         中值滤波
         :param img:输入图像
```

### Comparing `pyzjr-0.0.7/pyzjr/PIC.py` & `pyzjr-0.0.8/pyzjr/PIC.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.7/pyzjr/TrackBar.py` & `pyzjr-0.0.8/pyzjr/TrackBar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2
 import numpy as np
-from ColorModule import ColorFinder
+from pyzjr.ColorModule import ColorFinder
 import pyzjr.utils as zjr
 import logging
 
 def HSV(mode):
     """
     * 示例仅供参考，只是为了在调试过程中能够更快的找到相要的颜色
      可以进行调试成功的值进行替换，但也要记住将原来颜色的值注释。
```

### Comparing `pyzjr-0.0.7/pyzjr/__init__.py` & `pyzjr-0.0.8/pyzjr/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,27 +11,37 @@
 
 """
 from pyzjr import pyps as ps  # Using Image Processing
 from pyzjr import pysift as sift  # Using SIFT matching algorithm
 from pyzjr import Color as color
 """
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 import cv2
+
+
 from pyzjr.PIC import download_file,getPhotopath,Pic_rename,read_resize_image,\
                       load_images_from_folder,save_images
 from pyzjr.Enimage import Filter,Enhance,Random_Enhance,Retinex,\
                           repair_Img
 from pyzjr.definition import Fuzzy_image,Clear_quantification
+from pyzjr.ColorModule import *
+from pyzjr.definition import *
+from pyzjr.TrackBar import *
+from pyzjr.utils import *
+from pyzjr.video import *
+from pyzjr.Z import * 
+from pyzjr.zmath import *
+
 repair_TELEA=cv2.INPAINT_TELEA
 repair_NS=cv2.INPAINT_NS
 Lap_64F=cv2.CV_64F
 
-print("test successful")
+# print("test successful")  #仅仅在测试时候使用，其他时候不用
```

### Comparing `pyzjr-0.0.7/pyzjr/definition.py` & `pyzjr-0.0.8/pyzjr/definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 - author:Auorui(夏天是冰红茶)
 - creation time:2022.11.19
 - blog:https://blog.csdn.net/m0_62919535/article/details/127818006
 """
 import cv2
 import math
-from PIC import getPhotopath
+from pyzjr.PIC import getPhotopath
 import numpy as np
 import pyzjr.Z as Z
 
 class Clear_quantification():
     def brenner(self,img):
         '''
         Brenner梯度函数
```

### Comparing `pyzjr-0.0.7/pyzjr/utils.py` & `pyzjr-0.0.8/pyzjr/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.7/pyzjr/video.py` & `pyzjr-0.0.8/pyzjr/video.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.7/setup.py` & `pyzjr-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = ' a computer vision library that supports both Win and Mac '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports both Win and Mac'
 
 setup(
     name="pyzjr",
     version=VERSION,
     author="Auorui",
```

