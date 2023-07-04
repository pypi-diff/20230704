# Comparing `tmp/junkie-rfglab-2023.6.5.tar.gz` & `tmp/junkie-rfglab-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junkie-rfglab-2023.6.5.tar", last modified: Fri Jun 16 19:44:29 2023, max compression
+gzip compressed data, was "junkie-rfglab-2023.7.0.tar", last modified: Tue Jul  4 21:39:06 2023, max compression
```

## Comparing `junkie-rfglab-2023.6.5.tar` & `junkie-rfglab-2023.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-16 19:44:29.315070 junkie-rfglab-2023.6.5/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.5/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     3767 2023-06-16 19:44:29.314948 junkie-rfglab-2023.6.5/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     3179 2023-06-16 19:36:37.000000 junkie-rfglab-2023.6.5/README.md
--rw-r--r--   0 rodrigo    (501) staff       (20)    11588 2023-06-12 02:35:00.000000 junkie-rfglab-2023.6.5/junkie.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-16 19:44:29.314813 junkie-rfglab-2023.6.5/junkie_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     3767 2023-06-16 19:44:29.000000 junkie-rfglab-2023.6.5/junkie_rfglab.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)      226 2023-06-16 19:44:29.000000 junkie-rfglab-2023.6.5/junkie_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-06-16 19:44:29.000000 junkie-rfglab-2023.6.5/junkie_rfglab.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-06-16 19:44:29.000000 junkie-rfglab-2023.6.5/junkie_rfglab.egg-info/requires.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-06-16 19:44:29.000000 junkie-rfglab-2023.6.5/junkie_rfglab.egg-info/top_level.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-06-12 01:43:28.000000 junkie-rfglab-2023.6.5/pyproject.toml
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-06-16 19:44:29.315102 junkie-rfglab-2023.6.5/setup.cfg
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-04 21:39:06.943050 junkie-rfglab-2023.7.0/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.7.0/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3807 2023-07-04 21:39:06.942928 junkie-rfglab-2023.7.0/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3219 2023-06-25 21:38:24.000000 junkie-rfglab-2023.7.0/README.md
+-rw-r--r--   0 rodrigo    (501) staff       (20)    12080 2023-07-03 21:16:59.000000 junkie-rfglab-2023.7.0/junkie.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-07-04 21:39:06.942783 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3807 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)      226 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/requires.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-07-04 21:39:06.000000 junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)      840 2023-06-12 01:43:28.000000 junkie-rfglab-2023.7.0/pyproject.toml
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-07-04 21:39:06.943085 junkie-rfglab-2023.7.0/setup.cfg
```

### Comparing `junkie-rfglab-2023.6.5/LICENSE` & `junkie-rfglab-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.6.5/PKG-INFO` & `junkie-rfglab-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.5
+Version: 2023.7.0
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Logo](./docs/junkie_logo_100x100.png)
 [![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/GPL-3.0)
 
 # [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) (a JUpyter NotebooK Image Explorer)
 
 ## Installing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 To install [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), type:
```

### Comparing `junkie-rfglab-2023.6.5/README.md` & `junkie-rfglab-2023.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+![Logo](./docs/junkie_logo_100x100.png)
 [![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/GPL-3.0)
 
 # [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) (a JUpyter NotebooK Image Explorer)
 
 ## Installing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 To install [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), type:
```

### Comparing `junkie-rfglab-2023.6.5/junkie.py` & `junkie-rfglab-2023.7.0/junkie.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import skimage
 import IPython.display as IPyd
 import ipywidgets as ipyw
 import matplotlib.pyplot as plt
 
-__version__: str = '2023.6.5'  # this must be here for pyproject.toml to find it.
+__version__: str = '2023.7.0'  # this must be here for pyproject.toml to find it.
 
 
 # You will need this line in your jupyter notebook: %matplotlib widget
 
 class junkie:
     """ 
     junkie: a JUpyter NotebooK Image Explorer
@@ -152,15 +152,18 @@
             description='minimum pixel value:', style={'description_width': 'auto'})
         self._vmin_slider.observe(self._vmin_slider_change)
         self._vmax_slider = ipyw.IntSlider(min=0, max=self.pix_val_min_max[1], step=1, continuous_update=self.continuous_update, 
             description='maximum pixel value:', style={'description_width': 'auto'})
         self._vmax_slider.value = self.pix_val_min_max[1]
         self._vmax_slider.observe(self._vmax_slider_change, 'value')
 
-        self.new_toolbar = ipyw.VBox([self._channel_slider, self._t_slider, self._plane_selection, self._Z_slider, ipyw.HBox([self._vmin_slider, self._vmax_slider]), ipyw.HBox([self._axes_button, self._invert_button, self._continuousupdate_button])])
+        self._autocontrast_button = ipyw.Button(description='auto', layout=junkie.button_layout, style=junkie.button_style, tooltip='auto contrast')
+        self._autocontrast_button.on_click(self._autocontrast_button_click)
+
+        self.new_toolbar = ipyw.VBox([self._channel_slider, self._t_slider, self._plane_selection, self._Z_slider, ipyw.HBox([self._vmin_slider, self._autocontrast_button, self._vmax_slider]), ipyw.HBox([self._axes_button, self._invert_button, self._continuousupdate_button])])
 
         IPyd.display(self.new_toolbar)
 
     # Enables/disables UI components.
     def _setupUI(self):
         self._channel_slider.disabled = False if self.volume.shape[0] > 1 else True
         self._t_slider.disabled = False if self.volume.shape[1] > 1 else True
@@ -183,14 +186,21 @@
         self.volume = skimage.util.invert(self.volume)
         self.reset_volume()
         self.display_slice(True)
 
         self._vmin_slider.value = new_min
         self._vmax_slider.value = new_max
 
+    def _autocontrast_button_click(self, b):
+        low = np.min(self.image_data[self.curslice,:,:])
+        high = np.max(self.image_data[self.curslice,:,:])
+
+        self._vmin_slider.value = low
+        self._vmax_slider.value = high
+
     def _continuousupdate_button_click(self, b):
         self.continuous_update = not self.continuous_update
         
         self._channel_slider.continuous_update = self.continuous_update
         self._t_slider.continuous_update = self.continuous_update
         self._Z_slider.continuous_update = self.continuous_update
         self._vmin_slider.continuous_update = self.continuous_update
```

### Comparing `junkie-rfglab-2023.6.5/junkie_rfglab.egg-info/PKG-INFO` & `junkie-rfglab-2023.7.0/junkie_rfglab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.5
+Version: 2023.7.0
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Logo](./docs/junkie_logo_100x100.png)
 [![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/GPL-3.0)
 
 # [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/) (a JUpyter NotebooK Image Explorer)
 
 ## Installing [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/)
 
 To install [JuNkIE](https://bitbucket.org/rfg_lab/junkie/src/master/), type:
```

### Comparing `junkie-rfglab-2023.6.5/pyproject.toml` & `junkie-rfglab-2023.7.0/pyproject.toml`

 * *Files identical despite different names*

