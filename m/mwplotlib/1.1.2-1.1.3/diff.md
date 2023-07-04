# Comparing `tmp/mwplotlib-1.1.2.tar.gz` & `tmp/mwplotlib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwplotlib-1.1.2.tar", last modified: Mon Jul  3 05:58:45 2023, max compression
+gzip compressed data, was "mwplotlib-1.1.3.tar", last modified: Tue Jul  4 02:20:50 2023, max compression
```

## Comparing `mwplotlib-1.1.2.tar` & `mwplotlib-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:58:45.443202 mwplotlib-1.1.2/
--rw-r--r--   0 wenky      (501) staff       (20)     1066 2023-06-27 18:04:42.000000 mwplotlib-1.1.2/LICENSE
--rw-r--r--   0 wenky      (501) staff       (20)     2761 2023-07-03 05:58:45.443015 mwplotlib-1.1.2/PKG-INFO
--rw-r--r--   0 wenky      (501) staff       (20)     2512 2023-07-03 04:22:21.000000 mwplotlib-1.1.2/README.md
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:58:45.440641 mwplotlib-1.1.2/mwplotlib/
--rw-r--r--   0 wenky      (501) staff       (20)       51 2023-06-25 07:35:02.000000 mwplotlib-1.1.2/mwplotlib/__init__.py
--rw-r--r--   0 wenky      (501) staff       (20)     5068 2023-06-27 18:08:59.000000 mwplotlib-1.1.2/mwplotlib/arms_data.py
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:58:45.442638 mwplotlib-1.1.2/mwplotlib/data/
--rw-r--r--   0 wenky      (501) staff       (20)    32784 2023-06-25 04:47:07.000000 mwplotlib-1.1.2/mwplotlib/data/apjacc45ct1_mrt.txt
--rw-r--r--   0 wenky      (501) staff       (20)     1306 2023-06-26 11:18:19.000000 mwplotlib-1.1.2/mwplotlib/data/apjacc45ct2_ascii.txt
--rw-r--r--   0 wenky      (501) staff       (20)    13177 2023-07-03 05:51:20.000000 mwplotlib-1.1.2/mwplotlib/spiral_arms.py
--rw-r--r--   0 wenky      (501) staff       (20)     1454 2023-06-27 16:45:14.000000 mwplotlib-1.1.2/mwplotlib/utilities.py
-drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-03 05:58:45.441701 mwplotlib-1.1.2/mwplotlib.egg-info/
--rw-r--r--   0 wenky      (501) staff       (20)     2761 2023-07-03 05:58:45.000000 mwplotlib-1.1.2/mwplotlib.egg-info/PKG-INFO
--rw-r--r--   0 wenky      (501) staff       (20)      355 2023-07-03 05:58:45.000000 mwplotlib-1.1.2/mwplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 wenky      (501) staff       (20)        1 2023-07-03 05:58:45.000000 mwplotlib-1.1.2/mwplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 wenky      (501) staff       (20)       32 2023-07-03 05:58:45.000000 mwplotlib-1.1.2/mwplotlib.egg-info/requires.txt
--rw-r--r--   0 wenky      (501) staff       (20)       10 2023-07-03 05:58:45.000000 mwplotlib-1.1.2/mwplotlib.egg-info/top_level.txt
--rw-r--r--   0 wenky      (501) staff       (20)       38 2023-07-03 05:58:45.443264 mwplotlib-1.1.2/setup.cfg
--rw-r--r--   0 wenky      (501) staff       (20)      652 2023-07-03 05:58:11.000000 mwplotlib-1.1.2/setup.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-04 02:20:50.011350 mwplotlib-1.1.3/
+-rw-r--r--   0 wenky      (501) staff       (20)     1066 2023-06-27 18:04:42.000000 mwplotlib-1.1.3/LICENSE
+-rw-r--r--   0 wenky      (501) staff       (20)     2761 2023-07-04 02:20:50.011197 mwplotlib-1.1.3/PKG-INFO
+-rw-r--r--   0 wenky      (501) staff       (20)     2512 2023-07-03 04:22:21.000000 mwplotlib-1.1.3/README.md
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-04 02:20:50.009483 mwplotlib-1.1.3/mwplotlib/
+-rw-r--r--   0 wenky      (501) staff       (20)       51 2023-06-25 07:35:02.000000 mwplotlib-1.1.3/mwplotlib/__init__.py
+-rw-r--r--   0 wenky      (501) staff       (20)     5068 2023-06-27 18:08:59.000000 mwplotlib-1.1.3/mwplotlib/arms_data.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-04 02:20:50.010858 mwplotlib-1.1.3/mwplotlib/data/
+-rw-r--r--   0 wenky      (501) staff       (20)    32784 2023-06-25 04:47:07.000000 mwplotlib-1.1.3/mwplotlib/data/apjacc45ct1_mrt.txt
+-rw-r--r--   0 wenky      (501) staff       (20)     1306 2023-06-26 11:18:19.000000 mwplotlib-1.1.3/mwplotlib/data/apjacc45ct2_ascii.txt
+-rw-r--r--   0 wenky      (501) staff       (20)    13290 2023-07-04 02:18:42.000000 mwplotlib-1.1.3/mwplotlib/spiral_arms.py
+-rw-r--r--   0 wenky      (501) staff       (20)     1454 2023-06-27 16:45:14.000000 mwplotlib-1.1.3/mwplotlib/utilities.py
+drwxr-xr-x   0 wenky      (501) staff       (20)        0 2023-07-04 02:20:50.010224 mwplotlib-1.1.3/mwplotlib.egg-info/
+-rw-r--r--   0 wenky      (501) staff       (20)     2761 2023-07-04 02:20:49.000000 mwplotlib-1.1.3/mwplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 wenky      (501) staff       (20)      355 2023-07-04 02:20:49.000000 mwplotlib-1.1.3/mwplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 wenky      (501) staff       (20)        1 2023-07-04 02:20:49.000000 mwplotlib-1.1.3/mwplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       32 2023-07-04 02:20:49.000000 mwplotlib-1.1.3/mwplotlib.egg-info/requires.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       10 2023-07-04 02:20:49.000000 mwplotlib-1.1.3/mwplotlib.egg-info/top_level.txt
+-rw-r--r--   0 wenky      (501) staff       (20)       38 2023-07-04 02:20:50.011400 mwplotlib-1.1.3/setup.cfg
+-rw-r--r--   0 wenky      (501) staff       (20)      652 2023-07-04 02:20:19.000000 mwplotlib-1.1.3/setup.py
```

### Comparing `mwplotlib-1.1.2/LICENSE` & `mwplotlib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.2/PKG-INFO` & `mwplotlib-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwplotlib
-Version: 1.1.2
+Version: 1.1.3
 Summary: The Milky Way Plotting Library
 Home-page: https://github.com/xiawenke/mwplotlib
 Author: Wenky
 Author-email: wxia1@fandm.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mwplotlib-1.1.2/README.md` & `mwplotlib-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.2/mwplotlib/arms_data.py` & `mwplotlib-1.1.3/mwplotlib/arms_data.py`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.2/mwplotlib/data/apjacc45ct1_mrt.txt` & `mwplotlib-1.1.3/mwplotlib/data/apjacc45ct1_mrt.txt`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.2/mwplotlib/data/apjacc45ct2_ascii.txt` & `mwplotlib-1.1.3/mwplotlib/data/apjacc45ct2_ascii.txt`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.2/mwplotlib/spiral_arms.py` & `mwplotlib-1.1.3/mwplotlib/spiral_arms.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             plotData["color"].append(color_codes[plotData["arm"][i]])
         
         # print(plotData["color"])
         self.plt.scatter(plotData["x"], plotData["y"], s=1, c=plotData["color"])
         # plt.show()
         # input()
 
-    def shape(self, unit="kpc", style="region", step=.001, plot_type="polar", config={}, legend=True, offsets=[0, 0], rotate=0, **kwargs):
+    def shape(self, unit="kpc", style="region", step=.001, plot_type="polar", config={}, legend=True, offsets=[0, 0], rotate=0, direction="ccw", **kwargs):
         """
         config in the form of:
         {
             "Outer": {
                 "color": "red", 
                 "lw": 1,
                 ... # Matplotlib kwargs
@@ -146,14 +146,17 @@
 
             if(unit != "kpc"):
                 thisRRange_ = thisRRange * u.kpc
                 thisRRange = thisRRange_.to(u.Unit(unit)).value
                 thisArmWidth_ = thisArmWidth * u.kpc
                 thisArmWidth = thisArmWidth_.to(u.Unit(unit)).value
             
+            if(direction == "cw"):
+                thisBetaRange = - thisBetaRange
+            
             if(plot_type == "polar"):
                 if(thisRow['Spiral Arm'] != lastArm) :
                     # self.plt.plot(thisBetaRange, thisRRange + thisArmWidth / 2, "--", label=thisRow['Spiral Arm'])
                     # self.plt.plot(thisBetaRange, thisRRange - thisArmWidth / 2, "--", label=thisRow['Spiral Arm'], color=self._get_last_color())
                     # Allow for custom kwargs:
                     if(style == "region"):
                         self.plt.plot(thisBetaRange + offsets[0] + rotate, thisRRange + offsets[1] + thisArmWidth / 2, "--", **thisKwargs)
```

### Comparing `mwplotlib-1.1.2/mwplotlib/utilities.py` & `mwplotlib-1.1.3/mwplotlib/utilities.py`

 * *Files identical despite different names*

### Comparing `mwplotlib-1.1.2/mwplotlib.egg-info/PKG-INFO` & `mwplotlib-1.1.3/mwplotlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwplotlib
-Version: 1.1.2
+Version: 1.1.3
 Summary: The Milky Way Plotting Library
 Home-page: https://github.com/xiawenke/mwplotlib
 Author: Wenky
 Author-email: wxia1@fandm.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mwplotlib-1.1.2/setup.py` & `mwplotlib-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwplotlib",
-    version="1.1.2",
+    version="1.1.3",
     author="Wenky",
     author_email="wxia1@fandm.edu",
     description="The Milky Way Plotting Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xiawenke/mwplotlib",
     packages=setuptools.find_packages(),
```

