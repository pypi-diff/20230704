# Comparing `tmp/dip-python-0.1.4.tar.gz` & `tmp/dip-python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dip-python-0.1.4.tar", last modified: Thu Nov  3 16:47:30 2022, max compression
+gzip compressed data, was "dip-python-0.1.5.tar", last modified: Tue Jul  4 20:56:52 2023, max compression
```

## Comparing `dip-python-0.1.4.tar` & `dip-python-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 yixi       (501) staff       (20)        0 2022-11-03 16:47:30.430631 dip-python-0.1.4/
--rw-r--r--   0 yixi       (501) staff       (20)      664 2022-11-03 16:47:30.430513 dip-python-0.1.4/PKG-INFO
--rw-r--r--   0 yixi       (501) staff       (20)      149 2022-08-24 17:29:34.000000 dip-python-0.1.4/README.md
-drwxr-xr-x   0 yixi       (501) staff       (20)        0 2022-11-03 16:47:30.429595 dip-python-0.1.4/dip_python.egg-info/
--rw-r--r--   0 yixi       (501) staff       (20)      664 2022-11-03 16:47:30.000000 dip-python-0.1.4/dip_python.egg-info/PKG-INFO
--rw-r--r--   0 yixi       (501) staff       (20)      352 2022-11-03 16:47:30.000000 dip-python-0.1.4/dip_python.egg-info/SOURCES.txt
--rw-r--r--   0 yixi       (501) staff       (20)        1 2022-11-03 16:47:30.000000 dip-python-0.1.4/dip_python.egg-info/dependency_links.txt
--rw-r--r--   0 yixi       (501) staff       (20)        6 2022-11-03 16:47:30.000000 dip-python-0.1.4/dip_python.egg-info/requires.txt
--rw-r--r--   0 yixi       (501) staff       (20)       35 2022-11-03 16:47:30.000000 dip-python-0.1.4/dip_python.egg-info/top_level.txt
-drwxr-xr-x   0 yixi       (501) staff       (20)        0 2022-11-03 16:47:30.429698 dip-python-0.1.4/dippy/
--rw-r--r--   0 yixi       (501) staff       (20)      213 2022-08-24 18:19:21.000000 dip-python-0.1.4/dippy/__init__.py
-drwxr-xr-x   0 yixi       (501) staff       (20)        0 2022-11-03 16:47:30.430024 dip-python-0.1.4/dippy/algorithms/
--rw-r--r--   0 yixi       (501) staff       (20)     1762 2022-07-20 16:56:22.000000 dip-python-0.1.4/dippy/algorithms/convert.py
--rw-r--r--   0 yixi       (501) staff       (20)     9945 2022-10-20 05:49:20.000000 dip-python-0.1.4/dippy/algorithms/dithering.py
--rw-r--r--   0 yixi       (501) staff       (20)      624 2022-07-19 10:42:56.000000 dip-python-0.1.4/dippy/algorithms/kmeans.py
-drwxr-xr-x   0 yixi       (501) staff       (20)        0 2022-11-03 16:47:30.430342 dip-python-0.1.4/dippy/utils/
--rw-r--r--   0 yixi       (501) staff       (20)      779 2022-10-19 17:55:44.000000 dip-python-0.1.4/dippy/utils/convert.py
--rw-r--r--   0 yixi       (501) staff       (20)    10028 2022-08-24 21:33:44.000000 dip-python-0.1.4/dippy/utils/io.py
--rw-r--r--   0 yixi       (501) staff       (20)     2587 2022-10-22 20:21:38.000000 dip-python-0.1.4/dippy/utils/print.py
--rw-r--r--   0 yixi       (501) staff       (20)       38 2022-11-03 16:47:30.430671 dip-python-0.1.4/setup.cfg
--rw-r--r--   0 yixi       (501) staff       (20)      844 2022-11-03 16:38:34.000000 dip-python-0.1.4/setup.py
+drwxr-xr-x   0 yixi       (501) staff       (20)        0 2023-07-04 20:56:52.688444 dip-python-0.1.5/
+-rw-r--r--   0 yixi       (501) staff       (20)     3062 2023-07-04 20:56:52.688329 dip-python-0.1.5/PKG-INFO
+-rw-r--r--   0 yixi       (501) staff       (20)     1859 2023-05-04 20:36:22.000000 dip-python-0.1.5/README.md
+drwxr-xr-x   0 yixi       (501) staff       (20)        0 2023-07-04 20:56:52.686946 dip-python-0.1.5/dip_python.egg-info/
+-rw-r--r--   0 yixi       (501) staff       (20)     3062 2023-07-04 20:56:52.000000 dip-python-0.1.5/dip_python.egg-info/PKG-INFO
+-rw-r--r--   0 yixi       (501) staff       (20)      456 2023-07-04 20:56:52.000000 dip-python-0.1.5/dip_python.egg-info/SOURCES.txt
+-rw-r--r--   0 yixi       (501) staff       (20)        1 2023-07-04 20:56:52.000000 dip-python-0.1.5/dip_python.egg-info/dependency_links.txt
+-rw-r--r--   0 yixi       (501) staff       (20)        6 2023-07-04 20:56:52.000000 dip-python-0.1.5/dip_python.egg-info/requires.txt
+-rw-r--r--   0 yixi       (501) staff       (20)       35 2023-07-04 20:56:52.000000 dip-python-0.1.5/dip_python.egg-info/top_level.txt
+drwxr-xr-x   0 yixi       (501) staff       (20)        0 2023-07-04 20:56:52.687047 dip-python-0.1.5/dippy/
+-rw-r--r--   0 yixi       (501) staff       (20)      361 2023-07-04 20:30:33.000000 dip-python-0.1.5/dippy/__init__.py
+drwxr-xr-x   0 yixi       (501) staff       (20)        0 2023-07-04 20:56:52.687842 dip-python-0.1.5/dippy/algorithms/
+-rw-r--r--   0 yixi       (501) staff       (20)     4239 2023-05-04 20:26:09.000000 dip-python-0.1.5/dippy/algorithms/convert.py
+-rw-r--r--   0 yixi       (501) staff       (20)      399 2023-02-08 09:17:14.000000 dip-python-0.1.5/dippy/algorithms/dft.py
+-rw-r--r--   0 yixi       (501) staff       (20)     9945 2023-01-15 19:58:46.000000 dip-python-0.1.5/dippy/algorithms/dithering.py
+-rw-r--r--   0 yixi       (501) staff       (20)      761 2023-01-16 11:39:25.000000 dip-python-0.1.5/dippy/algorithms/filtering.py
+-rw-r--r--   0 yixi       (501) staff       (20)      624 2022-11-26 09:43:35.000000 dip-python-0.1.5/dippy/algorithms/kmeans.py
+-rw-r--r--   0 yixi       (501) staff       (20)      466 2023-07-04 20:37:34.000000 dip-python-0.1.5/dippy/algorithms/match.py
+-rw-r--r--   0 yixi       (501) staff       (20)      990 2023-03-23 18:11:45.000000 dip-python-0.1.5/dippy/algorithms/resize.py
+drwxr-xr-x   0 yixi       (501) staff       (20)        0 2023-07-04 20:56:52.688165 dip-python-0.1.5/dippy/utils/
+-rw-r--r--   0 yixi       (501) staff       (20)    15047 2023-01-17 10:17:35.000000 dip-python-0.1.5/dippy/utils/io.py
+-rw-r--r--   0 yixi       (501) staff       (20)     1555 2023-01-20 19:21:19.000000 dip-python-0.1.5/dippy/utils/jpeg.py
+-rw-r--r--   0 yixi       (501) staff       (20)     2178 2023-01-15 19:59:17.000000 dip-python-0.1.5/dippy/utils/print.py
+-rw-r--r--   0 yixi       (501) staff       (20)       38 2023-07-04 20:56:52.688482 dip-python-0.1.5/setup.cfg
+-rw-r--r--   0 yixi       (501) staff       (20)      844 2023-07-04 20:55:48.000000 dip-python-0.1.5/setup.py
```

### Comparing `dip-python-0.1.4/dippy/algorithms/dithering.py` & `dip-python-0.1.5/dippy/algorithms/dithering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,251 +1,251 @@
 import numpy as np
 
 
 def neighbor(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
-        for x in range(0, src.shape[0]):
+    for y in range(src.shape[0]):
+        for x in range(0, src.shape[1]):
             if dst[y][x] < 127.5:
                 err = dst[y][x] - 0
                 dst[y][x] = 0
             else:
                 err = dst[y][x] - 255
                 dst[y][x] = 255
-            if (x + 1) < src.shape[0]:
+            if (x + 1) < src.shape[1]:
                 dst[y][x+1] += err
     return dst.astype(np.uint8)
 
 
 def neighbor_2way(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
+    for y in range(src.shape[0]):
         if (y % 2) == 0:
-            for x in range(0, src.shape[0]):
+            for x in range(0, src.shape[1]):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
-                if (x + 1) < src.shape[0]:
+                if (x + 1) < src.shape[1]:
                     dst[y][x+1] += err
         else:
-            for x in range(src.shape[0], 0):
+            for x in range(src.shape[1], 0):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
                 if (x - 1) > 0:
                     dst[y][x-1] += err
     return dst.astype(np.uint8)
 
 
 def floyd_steinberg(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
-        for x in range(0, src.shape[0]):
+    for y in range(src.shape[0]):
+        for x in range(0, src.shape[1]):
             if dst[y][x] < 127.5:
                 err = dst[y][x] - 0
                 dst[y][x] = 0
             else:
                 err = dst[y][x] - 255
                 dst[y][x] = 255
-            if (x + 1) < src.shape[0]:
+            if (x + 1) < src.shape[1]:
                 dst[y][x+1] += err * (7 / 16)
-            if ((x - 1) > 0) and ((y + 1) < src.shape[1]):
+            if ((x - 1) > 0) and ((y + 1) < src.shape[0]):
                 dst[y+1][x-1] += err * (3 / 16)
-            if (y + 1) < src.shape[1]:
+            if (y + 1) < src.shape[0]:
                 dst[y+1][x] += err * (5 / 16)
-            if ((x + 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+            if ((x + 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                 dst[y+1][x+1] += err * (1 / 16)
     return dst.astype(np.uint8)
 
 
 def floyd_steinberg_2way(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
+    for y in range(src.shape[0]):
         if (y % 2) == 0:
-            for x in range(0, src.shape[0]):
+            for x in range(0, src.shape[1]):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
-                if (x + 1) < src.shape[0]:
+                if (x + 1) < src.shape[1]:
                     dst[y][x+1] += err * (7 / 16)
-                if ((x - 1) > 0) and ((y + 1) < src.shape[1]):
+                if ((x - 1) > 0) and ((y + 1) < src.shape[0]):
                     dst[y+1][x-1] += err * (3 / 16)
-                if (y + 1) < src.shape[1]:
+                if (y + 1) < src.shape[0]:
                     dst[y+1][x] += err * (5 / 16)
-                if ((x + 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+                if ((x + 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                     dst[y+1][x+1] += err * (1 / 16)
         else:
-            for x in range(src.shape[0], 0):
+            for x in range(src.shape[1], 0):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
                 if (x - 1) > 0:
                     dst[y][x-1] += err * (7 / 16)
-                if ((x + 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+                if ((x + 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                     dst[y+1][x+1] += err * (3 / 16)
-                if (y + 1) < src.shape[1]:
+                if (y + 1) < src.shape[0]:
                     dst[y+1][x] += err * (5 / 16)
-                if ((x - 1) > 0) and ((y + 1) < src.shape[1]):
+                if ((x - 1) > 0) and ((y + 1) < src.shape[0]):
                     dst[y+1][x-1] += err * (1 / 16)
     return dst.astype(np.uint8)
 
 
 def sierra_lite(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
-        for x in range(0, src.shape[0]):
+    for y in range(src.shape[0]):
+        for x in range(0, src.shape[1]):
             if dst[y][x] < 127.5:
                 err = dst[y][x] - 0
                 dst[y][x] = 0
             else:
                 err = dst[y][x] - 255
                 dst[y][x] = 255
-            if (x + 1) < src.shape[0]:
+            if (x + 1) < src.shape[1]:
                 dst[y][x+1] += (err / 4) * 2
-            if ((x - 1) > 0) and ((y + 1) < src.shape[1]):
+            if ((x - 1) > 0) and ((y + 1) < src.shape[0]):
                 dst[y+1][x-1] += err / 4
-            if (y + 1) < src.shape[1]:
+            if (y + 1) < src.shape[0]:
                 dst[y+1][x] += err / 4
     return dst.astype(np.uint8)
 
 
 def sierra_lite_2way(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
+    for y in range(src.shape[0]):
         if (y % 2) == 0:
-            for x in range(0, src.shape[0]):
+            for x in range(0, src.shape[1]):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
-                if (x + 1) < src.shape[0]:
+                if (x + 1) < src.shape[1]:
                     dst[y][x+1] += (err / 4) * 2
                 if ((x - 1) > 0) and ((y + 1) < src.shape[1]):
                     dst[y+1][x-1] += err / 4
-                if (y + 1) < src.shape[1]:
+                if (y + 1) < src.shape[0]:
                     dst[y+1][x] += err / 4
         else:
-            for x in range(src.shape[0], 0):
+            for x in range(src.shape[1], 0):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
                 if (x - 1) > 0:
                     dst[y][x-1] += (err / 4) * 2
-                if ((x + 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+                if ((x + 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                     dst[y+1][x+1] += err / 4
-                if (y + 1) < src.shape[1]:
+                if (y + 1) < src.shape[0]:
                     dst[y+1][x] += err / 4
     return dst.astype(np.uint8)
 
 
 def atkinson(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
-        for x in range(0, src.shape[0]):
+    for y in range(src.shape[0]):
+        for x in range(0, src.shape[1]):
             if dst[y][x] < 127.5:
                 err = dst[y][x] - 0
                 dst[y][x] = 0
             else:
                 err = dst[y][x] - 255
                 dst[y][x] = 255
-            if (x + 2) < src.shape[0]:
+            if (x + 2) < src.shape[1]:
                 dst[y][x+2] += err / 8
-            if (x + 1) < src.shape[0]:
+            if (x + 1) < src.shape[1]:
                 dst[y][x+1] += err / 8
-            if ((x - 1) > 0) and ((y + 1) < src.shape[1]):
+            if ((x - 1) > 0) and ((y + 1) < src.shape[0]):
                 dst[y+1][x-1] += err / 8
-            if (y + 1) < src.shape[1]:
+            if (y + 1) < src.shape[0]:
                 dst[y+1][x] += err / 8
-            if ((x + 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+            if ((x + 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                 dst[y+1][x+1] += err / 8
-            if (y + 2) < src.shape[1]:
+            if (y + 2) < src.shape[0]:
                 dst[y+2][x] += err / 8
     return dst.astype(np.uint8)
 
 
 def atkinson_2way(src: np.ndarray) -> np.ndarray:
     dst = src.copy()
-    for y in range(src.shape[1]):
+    for y in range(src.shape[0]):
         if (y % 2) == 0:
-            for x in range(0, src.shape[0]):
+            for x in range(0, src.shape[1]):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
-                if (x + 2) < src.shape[0]:
+                if (x + 2) < src.shape[1]:
                     dst[y][x+2] += err / 8
-                if (x + 1) < src.shape[0]:
+                if (x + 1) < src.shape[1]:
                     dst[y][x+1] += err / 8
-                if ((x - 1) > 0) and ((y + 1) < src.shape[1]):
+                if ((x - 1) > 0) and ((y + 1) < src.shape[0]):
                     dst[y+1][x-1] += err / 8
-                if (y + 1) < src.shape[1]:
+                if (y + 1) < src.shape[0]:
                     dst[y+1][x] += err / 8
-                if ((x + 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+                if ((x + 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                     dst[y+1][x+1] += err / 8
-                if (y + 2) < src.shape[1]:
+                if (y + 2) < src.shape[0]:
                     dst[y+2][x] += err / 8
         else:
-            for x in range(src.shape[0], 0):
+            for x in range(src.shape[1], 0):
                 if dst[y][x] < 127.5:
                     err = dst[y][x] - 0
                     dst[y][x] = 0
                 else:
                     err = dst[y][x] - 255
                     dst[y][x] = 255
                 if (x - 2) > 0:
                     dst[y][x-2] += err / 8
                 if (x - 1) > 0:
                     dst[y][x-1] += err / 8
-                if ((x + 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+                if ((x + 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                     dst[y+1][x+1] += err / 8
-                if (y + 1) < src.shape[1]:
+                if (y + 1) < src.shape[0]:
                     dst[y+1][x] += err / 8
-                if ((x - 1) < src.shape[0]) and ((y + 1) < src.shape[1]):
+                if ((x - 1) < src.shape[1]) and ((y + 1) < src.shape[0]):
                     dst[y+1][x-1] += err / 8
-                if (y + 2) < src.shape[1]:
+                if (y + 2) < src.shape[0]:
                     dst[y+2][x] += err / 8
     return dst.astype(np.uint8)
 
 
 def dithering(src: np.ndarray, method: str = "random") -> np.ndarray:
     if method == "random":
         dst = np.vectorize(lambda x: 255 if (np.random.rand() < (x/255)) else 0)(src)
     elif method == "bayer":
         dst = src.copy()
         mat = np.array([[0, 2], [3, 1]])
         # mat = np.array([[0, 8, 2, 10], [12, 4, 14, 6], [3, 11, 1, 9], [15, 7, 13, 5]])
         # mat = np.array([[10, 4, 6, 8], [12, 0, 2, 14], [7, 9, 11, 5], [3, 15, 13, 1]])
         # mat = np.array([[13, 7, 6, 12], [8, 1, 0, 5], [9, 2, 3, 4], [14, 10, 11, 15]])
-        for y in range(src.shape[1] // mat.shape[1]):
-            for x in range(src.shape[0] // mat.shape[0]):
-                for i in range(mat.shape[1]):
-                    for j in range(mat.shape[0]):
-                        if dst[(y*mat.shape[1])+j][(x*mat.shape[0])+i] > (mat[j][i] * (255 / (mat.shape[0]*mat.shape[1]))):
-                            dst[(y*mat.shape[1])+j][(x*mat.shape[0])+i] = 255
+        for y in range(src.shape[0] // mat.shape[0]):
+            for x in range(src.shape[1] // mat.shape[1]):
+                for i in range(mat.shape[0]):
+                    for j in range(mat.shape[1]):
+                        if dst[(y*mat.shape[0])+j][(x*mat.shape[1])+i] > (mat[j][i] * (255 / (mat.shape[1]*mat.shape[0]))):
+                            dst[(y*mat.shape[0])+j][(x*mat.shape[1])+i] = 255
                         else:
-                            dst[(y*mat.shape[1])+j][(x*mat.shape[0])+i] = 0
+                            dst[(y*mat.shape[0])+j][(x*mat.shape[1])+i] = 0
     elif method == "neighbor":
         dst = neighbor(src)
     elif method == "floyd_steinberg":
         dst = floyd_steinberg(src)
     elif method == "sierra_lite":
         dst = sierra_lite(src)
     elif method == "atkinson":
```

### Comparing `dip-python-0.1.4/dippy/algorithms/kmeans.py` & `dip-python-0.1.5/dippy/algorithms/kmeans.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def kmeans(src: np.ndarray, N: int = 16) -> np.ndarray:
     dst = src.copy()
     represents = np.random.randint(256, size=(N))
     for _ in range(10):
         distortions = [[0, 0] for _ in range(N)]
-        for y in range(src.shape[1]):
-            for x in range(src.shape[0]):
+        for y in range(src.shape[0]):
+            for x in range(src.shape[1]):
                 idx = np.argmin(np.abs(represents-dst[y][x]))
                 distortions[idx][0] += dst[y][x]
                 distortions[idx][1] += 1
                 dst[y][x] = represents[idx]
         represents = np.array([distortions[i][0]/(distortions[i][1]+1e-12) for i in range(N)])
     return dst.astype(np.uint8)
```

### Comparing `dip-python-0.1.4/setup.py` & `dip-python-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     name="dip-python",
     packages=[
         'dippy',
         'dippy/utils',
         'dippy/algorithms',
     ],
 
-    version="0.1.4",
+    version="0.1.5",
 
     license="MIT",
 
     python_requires=">=3.6",
     install_requires=['numpy'],
 
     author="RinYixi",
```

