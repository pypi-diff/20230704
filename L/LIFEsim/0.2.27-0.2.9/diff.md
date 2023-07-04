# Comparing `tmp/LIFEsim-0.2.27.tar.gz` & `tmp/LIFEsim-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/fdannert/Documents/projects/LIFEsim/LIFEsim/dist/.tmp-9__brsum/LIFEsim-0.2.27.tar", last modified: Tue Jul  4 15:44:36 2023, max compression
+gzip compressed data, was "/home/felix/Documents/MA/LIFEsim/dist/tmp7ho4ei8h/LIFEsim-0.2.9.tar", last modified: Tue Jun  1 11:35:22 2021, max compression
```

## Comparing `LIFEsim-0.2.27.tar` & `LIFEsim-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.325260 LIFEsim-0.2.27/
--rw-r--r--   0 fdannert   (501) staff       (20)    35149 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/LICENSE
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.304770 LIFEsim-0.2.27/LIFEsim.egg-info/
--rw-r--r--   0 fdannert   (501) staff       (20)     1844 2023-07-04 15:44:36.000000 LIFEsim-0.2.27/LIFEsim.egg-info/PKG-INFO
--rw-r--r--   0 fdannert   (501) staff       (20)      718 2023-07-04 15:44:36.000000 LIFEsim-0.2.27/LIFEsim.egg-info/SOURCES.txt
--rw-r--r--   0 fdannert   (501) staff       (20)        1 2023-07-04 15:44:36.000000 LIFEsim-0.2.27/LIFEsim.egg-info/dependency_links.txt
--rw-r--r--   0 fdannert   (501) staff       (20)        1 2021-07-02 07:45:53.000000 LIFEsim-0.2.27/LIFEsim.egg-info/not-zip-safe
--rw-r--r--   0 fdannert   (501) staff       (20)      102 2023-07-04 15:44:36.000000 LIFEsim-0.2.27/LIFEsim.egg-info/requires.txt
--rw-r--r--   0 fdannert   (501) staff       (20)        8 2023-07-04 15:44:36.000000 LIFEsim-0.2.27/LIFEsim.egg-info/top_level.txt
--rw-r--r--   0 fdannert   (501) staff       (20)     1844 2023-07-04 15:44:36.324702 LIFEsim-0.2.27/PKG-INFO
--rw-r--r--   0 fdannert   (501) staff       (20)     1088 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/README.rst
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.305321 LIFEsim-0.2.27/lifesim/
--rw-r--r--   0 fdannert   (501) staff       (20)      549 2023-07-04 15:43:54.000000 LIFEsim-0.2.27/lifesim/__init__.py
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.308545 LIFEsim-0.2.27/lifesim/core/
--rw-r--r--   0 fdannert   (501) staff       (20)    18831 2023-07-04 14:04:57.000000 LIFEsim-0.2.27/lifesim/core/core.py
--rw-r--r--   0 fdannert   (501) staff       (20)    26049 2023-07-04 14:04:57.000000 LIFEsim-0.2.27/lifesim/core/data.py
--rw-r--r--   0 fdannert   (501) staff       (20)     7152 2023-07-04 13:30:01.000000 LIFEsim-0.2.27/lifesim/core/modules.py
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.310807 LIFEsim-0.2.27/lifesim/gui/
--rw-r--r--   0 fdannert   (501) staff       (20)     5346 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/lifesim/gui/custom_widgets.py
--rw-r--r--   0 fdannert   (501) staff       (20)    34726 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/lifesim/gui/spectrum_gui.py
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.316543 LIFEsim-0.2.27/lifesim/instrument/
--rw-r--r--   0 fdannert   (501) staff       (20)    39239 2023-07-04 14:04:57.000000 LIFEsim-0.2.27/lifesim/instrument/instrument.py
--rw-r--r--   0 fdannert   (501) staff       (20)     5637 2023-07-04 13:30:01.000000 LIFEsim-0.2.27/lifesim/instrument/pn_exozodi.py
--rw-r--r--   0 fdannert   (501) staff       (20)     5253 2023-07-04 13:30:01.000000 LIFEsim-0.2.27/lifesim/instrument/pn_localzodi.py
--rw-r--r--   0 fdannert   (501) staff       (20)     4442 2023-07-04 13:30:01.000000 LIFEsim-0.2.27/lifesim/instrument/pn_star.py
--rw-r--r--   0 fdannert   (501) staff       (20)     9546 2023-07-04 13:30:01.000000 LIFEsim-0.2.27/lifesim/instrument/transmission.py
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.318383 LIFEsim-0.2.27/lifesim/optimize/
--rw-r--r--   0 fdannert   (501) staff       (20)     7006 2023-07-04 13:30:01.000000 LIFEsim-0.2.27/lifesim/optimize/ahgs.py
--rw-r--r--   0 fdannert   (501) staff       (20)     4196 2023-07-04 13:30:01.000000 LIFEsim-0.2.27/lifesim/optimize/optimizer.py
-drwxr-xr-x   0 fdannert   (501) staff       (20)        0 2023-07-04 15:44:36.323466 LIFEsim-0.2.27/lifesim/util/
--rw-r--r--   0 fdannert   (501) staff       (20)      181 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/lifesim/util/constants.py
--rw-r--r--   0 fdannert   (501) staff       (20)     2702 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/lifesim/util/habitable.py
--rw-r--r--   0 fdannert   (501) staff       (20)     6088 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/lifesim/util/importer.py
--rw-r--r--   0 fdannert   (501) staff       (20)     7306 2023-07-04 14:04:57.000000 LIFEsim-0.2.27/lifesim/util/options.py
--rw-r--r--   0 fdannert   (501) staff       (20)     5734 2021-07-02 07:44:41.000000 LIFEsim-0.2.27/lifesim/util/radiation.py
--rw-r--r--   0 fdannert   (501) staff       (20)      103 2023-05-17 12:44:11.000000 LIFEsim-0.2.27/pyproject.toml
--rw-r--r--   0 fdannert   (501) staff       (20)       38 2023-07-04 15:44:36.325440 LIFEsim-0.2.27/setup.cfg
--rw-r--r--   0 fdannert   (501) staff       (20)     2040 2023-07-04 14:04:57.000000 LIFEsim-0.2.27/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/
+-rw-r--r--   0 felix     (1000) felix     (1000)    35149 2021-04-01 15:18:54.000000 LIFEsim-0.2.9/LICENSE
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/LIFEsim.egg-info/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1807 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/LIFEsim.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      742 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/LIFEsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/LIFEsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2021-05-18 14:01:36.000000 LIFEsim-0.2.9/LIFEsim.egg-info/not-zip-safe
+-rw-rw-r--   0 felix     (1000) felix     (1000)      356 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/LIFEsim.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        8 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/LIFEsim.egg-info/top_level.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1807 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)     1032 2021-05-18 18:15:18.000000 LIFEsim-0.2.9/README.rst
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/lifesim/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      525 2021-06-01 11:34:53.000000 LIFEsim-0.2.9/lifesim/__init__.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/lifesim/core/
+-rw-rw-r--   0 felix     (1000) felix     (1000)    15823 2021-05-18 11:29:30.000000 LIFEsim-0.2.9/lifesim/core/core.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)    21903 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/core/data.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     6217 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/core/modules.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/lifesim/gui/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     4585 2021-05-17 17:31:55.000000 LIFEsim-0.2.9/lifesim/gui/custom_widgets.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)    27722 2021-06-01 11:34:53.000000 LIFEsim-0.2.9/lifesim/gui/spectrum_gui.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/lifesim/instrument/
+-rw-rw-r--   0 felix     (1000) felix     (1000)    19384 2021-05-18 06:27:06.000000 LIFEsim-0.2.9/lifesim/instrument/instrument.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     5621 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/instrument/pn_exozodi.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     5245 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/instrument/pn_localzodi.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     4434 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/instrument/pn_star.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     9546 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/instrument/transmission.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/lifesim/optimize/
+-rw-rw-r--   0 felix     (1000) felix     (1000)     6178 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/optimize/ahgs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4026 2021-04-01 15:18:54.000000 LIFEsim-0.2.9/lifesim/optimize/optimizer.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/lifesim/util/
+-rw-r--r--   0 felix     (1000) felix     (1000)     4411 2021-02-07 18:07:40.000000 LIFEsim-0.2.9/lifesim/util/analyze.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      181 2021-03-08 13:18:55.000000 LIFEsim-0.2.9/lifesim/util/constants.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2103 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/util/habitable.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     5481 2021-05-18 11:29:30.000000 LIFEsim-0.2.9/lifesim/util/importer.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     7115 2021-05-17 16:42:04.000000 LIFEsim-0.2.9/lifesim/util/options.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5734 2021-01-06 18:30:23.000000 LIFEsim-0.2.9/lifesim/util/radiation.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)      103 2021-05-18 16:19:09.000000 LIFEsim-0.2.9/pyproject.toml
+-rw-rw-r--   0 felix     (1000) felix     (1000)       38 2021-06-01 11:35:22.000000 LIFEsim-0.2.9/setup.cfg
+-rw-rw-r--   0 felix     (1000) felix     (1000)     2391 2021-06-01 11:34:53.000000 LIFEsim-0.2.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `LIFEsim-0.2.27/LICENSE` & `LIFEsim-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LIFEsim-0.2.27/LIFEsim.egg-info/PKG-INFO` & `LIFEsim-0.2.9/LIFEsim.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: LIFEsim
-Version: 0.2.27
+Version: 0.2.9
 Summary: Simulator software for the Large Interferometer For Exoplanets (LIFE)
 Home-page: https://github.com/fdannert/LIFEsim
 Author: Felix Dannert, Maurice Ottiger & Sascha Quanz
 Author-email: fdannert@ethz.ch
 License: GPLv3
 Project-URL: Documentation, https://lifesim.readthedocs.io
 Keywords: lifesim
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: ~=3.8
@@ -40,18 +41,19 @@
 Please visit the `LIFE website <https://www.life-space-mission.com/>`_  to learn more about the
 LIFE mission.
 
 
 Attribution
 -----------
 
-If you use LIFEsim in your work, please cite
-`Dannert & Ottiger et al. 2022 <https://doi.org/10.48550/arXiv.2203.00471>`_.
+If you use LIFEsim in your work, please cite Ottiger et al., 2021.
 
 
 License
 -------
 
-Copyright 2019-2023 Felix Dannert, Maurice Ottiger, Sascha Quanz and contributors.
+Copyright 2019-2020 Felix Dannert, Maurice Ottiger, Sascha Quanz and contributors.
 
 LIFEsim is distributed under the GNU General Public License v3. See the LICENSE file for the terms
 and conditions.
+
+
```

### Comparing `LIFEsim-0.2.27/LIFEsim.egg-info/SOURCES.txt` & `LIFEsim-0.2.9/LIFEsim.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,12 +17,13 @@
 lifesim/instrument/instrument.py
 lifesim/instrument/pn_exozodi.py
 lifesim/instrument/pn_localzodi.py
 lifesim/instrument/pn_star.py
 lifesim/instrument/transmission.py
 lifesim/optimize/ahgs.py
 lifesim/optimize/optimizer.py
+lifesim/util/analyze.py
 lifesim/util/constants.py
 lifesim/util/habitable.py
 lifesim/util/importer.py
 lifesim/util/options.py
 lifesim/util/radiation.py
```

### Comparing `LIFEsim-0.2.27/PKG-INFO` & `LIFEsim-0.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: LIFEsim
-Version: 0.2.27
+Version: 0.2.9
 Summary: Simulator software for the Large Interferometer For Exoplanets (LIFE)
 Home-page: https://github.com/fdannert/LIFEsim
 Author: Felix Dannert, Maurice Ottiger & Sascha Quanz
 Author-email: fdannert@ethz.ch
 License: GPLv3
 Project-URL: Documentation, https://lifesim.readthedocs.io
 Keywords: lifesim
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: ~=3.8
@@ -40,18 +41,19 @@
 Please visit the `LIFE website <https://www.life-space-mission.com/>`_  to learn more about the
 LIFE mission.
 
 
 Attribution
 -----------
 
-If you use LIFEsim in your work, please cite
-`Dannert & Ottiger et al. 2022 <https://doi.org/10.48550/arXiv.2203.00471>`_.
+If you use LIFEsim in your work, please cite Ottiger et al., 2021.
 
 
 License
 -------
 
-Copyright 2019-2023 Felix Dannert, Maurice Ottiger, Sascha Quanz and contributors.
+Copyright 2019-2020 Felix Dannert, Maurice Ottiger, Sascha Quanz and contributors.
 
 LIFEsim is distributed under the GNU General Public License v3. See the LICENSE file for the terms
 and conditions.
+
+
```

### Comparing `LIFEsim-0.2.27/README.rst` & `LIFEsim-0.2.9/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 Please visit the `LIFE website <https://www.life-space-mission.com/>`_  to learn more about the
 LIFE mission.
 
 
 Attribution
 -----------
 
-If you use LIFEsim in your work, please cite
-`Dannert & Ottiger et al. 2022 <https://doi.org/10.48550/arXiv.2203.00471>`_.
+If you use LIFEsim in your work, please cite Ottiger et al., 2021.
 
 
 License
 -------
 
-Copyright 2019-2023 Felix Dannert, Maurice Ottiger, Sascha Quanz and contributors.
+Copyright 2019-2020 Felix Dannert, Maurice Ottiger, Sascha Quanz and contributors.
 
 LIFEsim is distributed under the GNU General Public License v3. See the LICENSE file for the terms
 and conditions.
```

### Comparing `LIFEsim-0.2.27/lifesim/__init__.py` & `LIFEsim-0.2.9/lifesim/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-__version__ = '0.2.27'
-
 from lifesim.core.core import Module, Bus
 
 from lifesim.instrument.instrument import Instrument
 from lifesim.instrument.transmission import TransmissionMap
 from lifesim.instrument.pn_exozodi import PhotonNoiseExozodi
 from lifesim.instrument.pn_localzodi import PhotonNoiseLocalzodi
 from lifesim.instrument.pn_star import PhotonNoiseStar
```

### Comparing `LIFEsim-0.2.27/lifesim/core/core.py` & `LIFEsim-0.2.9/lifesim/core/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import annotations
 import abc
 from abc import ABC
-from typing import Tuple, Union
+from typing import Tuple
 import warnings
-import os
-
-import yaml
-from numpy import ndarray, array
-import git
 
 from lifesim.core.data import Data
 
 
 class Module(ABC):
     """
     A `Module` is the most basic component of LIFEsim. A single `Module` should be used to
@@ -436,87 +431,7 @@
         # add module to the list of modules
         if module.name in self.modules.keys():
             raise ValueError('The module name ' + module.name + ' is already in use in this bus')
         self.modules[module.name] = module
 
         # point module to the data storage class
         module.data = self.data
-
-    def write_config(self):
-        module_dict = {key: str(type(module)) for (key, module) in self.modules.items()}
-
-        # fetch version number and git commit hash if available
-        lifesim_path = os.path.abspath(os.path.join(os.path.dirname( __file__ ), '..', '..'))
-        version_dict = {}
-
-        try:
-            repo = git.Repo(lifesim_path)
-            version_dict['git_sha'] = repo.head.object.hexsha
-            version_dict['git_branch'] = repo.active_branch.name
-        except ValueError:
-            version_dict['git_sha'] = 'not a git repository'
-            version_dict['git_branch'] = 'not a git repository'
-
-        # TODO: This is extremely ugly. Fix this.
-        from lifesim.__init__ import __version__
-        version_dict['version'] = __version__
-
-        config_dict = {'array': convert_to_list(self.data.options.array),
-                       'models': convert_to_list(self.data.options.models),
-                       'optimization': convert_to_list(self.data.options.optimization),
-                       'other': convert_to_list(self.data.options.other),
-                       'modules': module_dict,
-                       'connections': convert_to_list(self.connections),
-                       'version': version_dict}
-
-        with open(self.data.options.other['output_path']
-                  + self.data.options.other['output_filename'] + '.yaml', 'w') as file:
-            documents = yaml.dump(config_dict, file)
-
-    def build_from_config(self,
-                          filename: str):
-        with open(filename) as file:
-            config_dict = yaml.load(file, Loader=yaml.FullLoader)
-
-        self.data.options.array = convert_to_np(config_dict['array'])
-        self.data.options.optimization = convert_to_np(config_dict['optimization'])
-        self.data.options.models = config_dict['models']
-        self.data.options.other = config_dict['other']
-
-        # TODO: Implement methods for rebuilding modules and connections from config file
-
-    def save(self):
-        print('Saving database and config files...')
-        self.write_config()
-        if self.data.catalog is not None:
-            self.data.export_catalog()
-        print('[Done]')
-
-
-def convert_to_list(inp: Union[dict, list]):
-
-    if isinstance(inp, dict):
-        out = {}
-        for k in inp.keys():
-            if isinstance(inp[k], ndarray):
-                out[k] = inp[k].tolist()
-            else:
-                out[k] = inp[k]
-    elif isinstance(inp, list):
-        out = []
-        for el in inp:
-            if isinstance(el, set):
-                out.append(list(el))
-            else:
-                out.append(el)
-    else:
-        raise ValueError('Unsupported input type')
-    return out
-
-def convert_to_np(inp: dict):
-    out = {}
-    for k in inp.keys():
-        if isinstance(inp[k], list):
-            out[k] = array(inp[k])
-        else:
-            out[k] = inp[k]
-    return out
```

### Comparing `LIFEsim-0.2.27/lifesim/core/data.py` & `LIFEsim-0.2.9/lifesim/core/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import warnings
 
 import numpy as np
 import pandas as pd
 from astropy.io import fits
+from astropy.table import Table
 from astropy.coordinates import SkyCoord, BarycentricMeanEcliptic
 
 from lifesim.util.options import Options
 from lifesim.util.habitable import single_habitable_zone
 
 
 # TODO: automatically add data storage for all
@@ -42,16 +43,15 @@
     def catalog_delete(self):
         self.catalog = None
 
     def catalog_from_ppop(self,
                           input_path: str,
                           overwrite: bool = False):
         """
-        Read the contents of the P-Pop output file (in .txt or .fits format) to a catalog. Note that reading catalogs
-        in .fits format is significantly faster.
+        Read the contents of the P-Pop output file (in .txt or .fits format) to a catalog.
 
         Parameters
         ----------
         input_path : str
             Path to the P-Pop output file in a .txt or .fits format.
         overwrite : bool
             If set to true, existing catalogs can overwritten.
@@ -63,14 +63,21 @@
         """
 
         # make sure that no catalog exists
         if (self.catalog is not None) and (not overwrite):
             raise ValueError('A catalog has already been imported. Delete the old catalog or set '
                              'overwrite=True')
 
+        # set keys for the stellar types to avoid type mismatched DataFrames
+        self.other['stype_key'] = {'A': 0,
+                                   'F': 1,
+                                   'G': 2,
+                                   'K': 3,
+                                   'M': 4}
+
         # initialize catalog
         self.catalog = pd.DataFrame(columns=['radius_p',
                                              'p_orb',
                                              'mass_p',
                                              'ecc_p',
                                              'inc_p',
                                              'large_omega_p',
@@ -92,16 +99,15 @@
                                              'temp_s',
                                              'distance_s',
                                              'ra',
                                              'dec',
                                              'nuniverse',
                                              'nstar',
                                              'stype',
-                                             'id',
-                                             'name_s'])
+                                             'id'])
 
         # check the format of the input file
         if input_path[-4:] == '.txt':
             table = open(input_path, 'r')
             table_lines = table.readlines()
 
             nuniverse = []
@@ -128,26 +134,22 @@
             radius_s = []  # Rsun
             mass_s = []  # Msun
             temp_s = []  # K
             distance_s = []  # pc
             stype = []
             ra = []  # deg
             dec = []  # deg
-            name_s = []
 
             nlines = len(table_lines)
 
             # The second line (i = 1) contains the column names of the new
             # Ppop while the first line (i = 0) contains the column names
             # of the old Ppop.
 
             tempLine = table_lines[1].split('\t')
-
-            get_name = ('name' in tempLine)
-
             col_nuniverse = np.where(np.array(tempLine) == 'Nuniverse')[0][0]
             col_radius_p = np.where(np.array(tempLine) == 'Rp')[0][0]
             col_p_orb = np.where(np.array(tempLine) == 'Porb')[0][0]
             col_mass_p = np.where(np.array(tempLine) == 'Mp')[0][0]
             col_ecc_p = np.where(np.array(tempLine) == 'ep')[0][0]
             col_inc_p = np.where(np.array(tempLine) == 'ip')[0][0]
             col_large_omega_p = np.where(np.array(tempLine) == 'Omegap')[0][0]
@@ -169,17 +171,14 @@
             col_mass_s = np.where(np.array(tempLine) == 'Ms')[0][0]
             col_temp_s = np.where(np.array(tempLine) == 'Ts')[0][0]
             col_distance_s = np.where(np.array(tempLine) == 'Ds')[0][0]
             col_stype = np.where(np.array(tempLine) == 'Stype')[0][0]
             col_ra = np.where(np.array(tempLine) == 'RA')[0][0]
             col_dec = np.where(np.array(tempLine) == 'Dec')[0][0]
 
-            if get_name:
-                col_name_s = np.where(np.array(tempLine) == 'name')[0][0]
-
             for i, line in enumerate(table_lines[2:]):
 
                 if (i % 10000) == 0:
                     sys.stdout.write('\rProcessed line %.0f of %.0f' % (i, nlines))
                     sys.stdout.flush()
 
                 tempLine = line.split('\t')
@@ -208,27 +207,18 @@
                 mass_s += [float(tempLine[col_mass_s])]  # Msun
                 temp_s += [float(tempLine[col_temp_s])]  # K
                 distance_s += [float(tempLine[col_distance_s])]  # pc
                 stype += [str(tempLine[col_stype])]
                 ra += [float(tempLine[col_ra])]  # deg
                 dec += [float(tempLine[col_dec])]  # deg
 
-                if get_name:
-                    name_s += [str(tempLine[col_name_s])]
-
             sys.stdout.write('\rProcessed line %.0f of %.0f' % (nlines, nlines))
             sys.stdout.flush()
             print('')
 
-            # remove the newline string from the star names
-            if get_name:
-                name_s = [name.replace('\n', '') for name in name_s]
-            else:
-                name_s = ['None'] * len(dec)
-
             # save the data to the pandas DataFrame
             self.catalog['nuniverse'] = np.array(nuniverse).astype(int)
             self.catalog['radius_p'] = np.array(radius_p).astype(float)
             self.catalog['p_orb'] = np.array(p_orb)
             self.catalog['mass_p'] = np.array(mass_p)
             self.catalog['ecc_p'] = np.array(ecc_p)
             self.catalog['inc_p'] = np.array(inc_p)
@@ -247,108 +237,78 @@
             self.catalog['fp'] = np.array(fp)
             self.catalog['temp_p'] = np.array(temp_p)
             self.catalog['nstar'] = np.array(nstar)
             self.catalog['radius_s'] = np.array(radius_s)
             self.catalog['mass_s'] = np.array(mass_s)
             self.catalog['temp_s'] = np.array(temp_s)
             self.catalog['distance_s'] = np.array(distance_s)
-            self.catalog['stype'] = pd.Series(stype, dtype=pd.StringDtype())
+            self.catalog['stype'] = np.array(stype)
             self.catalog['ra'] = np.array(ra)
             self.catalog['dec'] = np.array(dec)
             self.catalog['id'] = np.arange(0, len(dec), 1)
-            self.catalog['name_s'] = pd.Series(name_s, dtype=pd.StringDtype())
 
         # check the format of the input file
         elif input_path[-5:] == '.fits':
             hdu = fits.open(input_path)
-
-            get_name = ('name' in hdu[1].columns.names)
+            stype_int = np.zeros_like(hdu[1].data.Nstar.astype(int), dtype=int)
+            for _, k in enumerate(self.other['stype_key'].keys()):
+                stype_int[hdu[1].data.Stype.astype(str) == k] = self.other['stype_key'][k]
 
             # save the data to the pandas DataFrame, make sure it is saved in the correct type
             # some errors were produced here by not respecting the endianess of the data (numpy
             # usually works with little endian)
-            if get_name:
-                self.catalog = pd.DataFrame({'nuniverse': hdu[1].data.Nuniverse.astype(int),
-                                             'nstar': hdu[1].data.Nstar.astype(int),
-                                             'stype': pd.Series(hdu[1].data.Stype, dtype=pd.StringDtype()),
-                                             'id': np.arange(0, hdu[1].data.Dec.shape[0], 1).astype(int),
-                                             'radius_p': hdu[1].data.Rp.astype(float),
-                                             'p_orb': hdu[1].data.Porb.astype(float),
-                                             'mass_p': hdu[1].data.Mp.astype(float),
-                                             'ecc_p': hdu[1].data.ep.astype(float),
-                                             'inc_p': hdu[1].data.ip.astype(float),
-                                             'large_omega_p': hdu[1].data.Omegap.astype(float),
-                                             'small_omega_p': hdu[1].data.omegap.astype(float),
-                                             'theta_p': hdu[1].data.thetap.astype(float),
-                                             'albedo_bond': hdu[1].data.Abond.astype(float),
-                                             'albedo_geom_vis': hdu[1].data.AgeomVIS.astype(float),
-                                             'albedo_geom_mir': hdu[1].data.AgeomMIR.astype(float),
-                                             'z': hdu[1].data.z.astype(float),
-                                             'semimajor_p': hdu[1].data.ap.astype(float),
-                                             'sep_p': hdu[1].data.rp.astype(float),
-                                             'angsep': hdu[1].data.AngSep.astype(float),
-                                             'maxangsep': hdu[1].data.maxAngSep.astype(float),
-                                             'flux_p': hdu[1].data.Fp.astype(float),
-                                             'fp': hdu[1].data.fp.astype(float),
-                                             'temp_p': hdu[1].data.Tp.astype(float),
-                                             'radius_s': hdu[1].data.Rs.astype(float),
-                                             'mass_s': hdu[1].data.Ms.astype(float),
-                                             'temp_s': hdu[1].data.Ts.astype(float),
-                                             'distance_s': hdu[1].data.Ds.astype(float),
-                                             'ra': hdu[1].data.RA.astype(float),
-                                             'dec': hdu[1].data.Dec.astype(float),
-                                             'lat': hdu[1].data.lat.astype(float),
-                                             'lon': hdu[1].data.lon.astype(float),
-                                             'name_s': pd.Series(hdu[1].data.name, dtype=pd.StringDtype())})
-            else:
-                self.catalog = pd.DataFrame({'nuniverse': hdu[1].data.Nuniverse.astype(int),
-                                             'nstar': hdu[1].data.Nstar.astype(int),
-                                             'stype': pd.Series(hdu[1].data.Stype, dtype=pd.StringDtype()),
-                                             'id': np.arange(0, hdu[1].data.Dec.shape[0], 1).astype(int),
-                                             'radius_p': hdu[1].data.Rp.astype(float),
-                                             'p_orb': hdu[1].data.Porb.astype(float),
-                                             'mass_p': hdu[1].data.Mp.astype(float),
-                                             'ecc_p': hdu[1].data.ep.astype(float),
-                                             'inc_p': hdu[1].data.ip.astype(float),
-                                             'large_omega_p': hdu[1].data.Omegap.astype(float),
-                                             'small_omega_p': hdu[1].data.omegap.astype(float),
-                                             'theta_p': hdu[1].data.thetap.astype(float),
-                                             'albedo_bond': hdu[1].data.Abond.astype(float),
-                                             'albedo_geom_vis': hdu[1].data.AgeomVIS.astype(float),
-                                             'albedo_geom_mir': hdu[1].data.AgeomMIR.astype(float),
-                                             'z': hdu[1].data.z.astype(float),
-                                             'semimajor_p': hdu[1].data.ap.astype(float),
-                                             'sep_p': hdu[1].data.rp.astype(float),
-                                             'angsep': hdu[1].data.AngSep.astype(float),
-                                             'maxangsep': hdu[1].data.maxAngSep.astype(float),
-                                             'flux_p': hdu[1].data.Fp.astype(float),
-                                             'fp': hdu[1].data.fp.astype(float),
-                                             'temp_p': hdu[1].data.Tp.astype(float),
-                                             'radius_s': hdu[1].data.Rs.astype(float),
-                                             'mass_s': hdu[1].data.Ms.astype(float),
-                                             'temp_s': hdu[1].data.Ts.astype(float),
-                                             'distance_s': hdu[1].data.Ds.astype(float),
-                                             'ra': hdu[1].data.RA.astype(float),
-                                             'dec': hdu[1].data.Dec.astype(float),
-                                             'lat': hdu[1].data.lat.astype(float),
-                                             'lon': hdu[1].data.lon.astype(float),
-                                             'name_s': pd.Series(['None']*hdu[1].data.shape[0], dtype=pd.StringDtype())})
+            self.catalog = pd.DataFrame({'nuniverse': hdu[1].data.Nuniverse.astype(int),
+                                         'nstar': hdu[1].data.Nstar.astype(int),
+                                         'stype': stype_int,
+                                         'id': np.arange(0, hdu[1].data.Dec.shape[0], 1).astype(int),
+                                         'radius_p': hdu[1].data.Rp.astype(float),
+                                         'p_orb': hdu[1].data.Porb.astype(float),
+                                         'mass_p': hdu[1].data.Mp.astype(float),
+                                         'ecc_p': hdu[1].data.ep.astype(float),
+                                         'inc_p': hdu[1].data.ip.astype(float),
+                                         'large_omega_p': hdu[1].data.Omegap.astype(float),
+                                         'small_omega_p': hdu[1].data.omegap.astype(float),
+                                         'theta_p': hdu[1].data.thetap.astype(float),
+                                         'albedo_bond': hdu[1].data.Abond.astype(float),
+                                         'albedo_geom_vis': hdu[1].data.AgeomVIS.astype(float),
+                                         'albedo_geom_mir': hdu[1].data.AgeomMIR.astype(float),
+                                         'z': hdu[1].data.z.astype(float),
+                                         'semimajor_p': hdu[1].data.ap.astype(float),
+                                         'sep_p': hdu[1].data.rp.astype(float),
+                                         'angsep': hdu[1].data.AngSep.astype(float),
+                                         'maxangsep': hdu[1].data.maxAngSep.astype(float),
+                                         'flux_p': hdu[1].data.Fp.astype(float),
+                                         'fp': hdu[1].data.fp.astype(float),
+                                         'temp_p': hdu[1].data.Tp.astype(float),
+                                         'radius_s': hdu[1].data.Rs.astype(float),
+                                         'mass_s': hdu[1].data.Ms.astype(float),
+                                         'temp_s': hdu[1].data.Ts.astype(float),
+                                         'distance_s': hdu[1].data.Ds.astype(float),
+                                         'ra': hdu[1].data.RA.astype(float),
+                                         'dec': hdu[1].data.Dec.astype(float),
+                                         'lat': hdu[1].data.lat.astype(float),
+                                         'lon': hdu[1].data.lon.astype(float)})
             hdu.close()
 
+        # create array saving the stellar types in character format
+        self.other['stype'] = np.zeros_like(self.catalog.nstar, dtype=str)
+        for _, k in enumerate(self.other['stype_key']):
+            self.other['stype'][self.catalog.stype == self.other['stype_key'][k]] = k
+
         # create mask returning only unique stars
         _, temp = np.unique(self.catalog.nstar, return_index=True)
         star_mask = np.zeros_like(self.catalog.nstar, dtype=bool)
         star_mask[temp] = True
 
         # TODO: why is this commented out? AFAIK P-Pop uses equitorial coordinates
         # transform from equitorial to ecliptic coordinates
-        coord = SkyCoord(self.catalog.ra, self.catalog.dec, frame='icrs', unit='deg')
-        coord_ec = coord.transform_to(BarycentricMeanEcliptic())
-        self.catalog['lon'] = np.array(coord_ec.lon.radian)
-        self.catalog['lat'] = np.array(coord_ec.lat.radian)
+        # coord = SkyCoord(self.catalog.ra, self.catalog.dec, frame='icrs', unit='deg')
+        # coord_ec = coord.transform_to(BarycentricMeanEcliptic())
+        # self.catalog['lon'] = np.array(coord_ec.lon.radian)
+        # self.catalog['lat'] = np.array(coord_ec.lat.radian)
 
         # add the inner/ outer edges and centers of the habitable zone
         s_in = np.zeros_like(self.catalog.nstar, dtype=float)
         s_out = np.zeros_like(self.catalog.nstar, dtype=float)
         l_sun = np.zeros_like(self.catalog.nstar, dtype=float)
 
         hz_in = np.zeros_like(self.catalog.nstar, dtype=float)
@@ -378,38 +338,39 @@
             (self.catalog['radius_p'].ge(0.5)).to_numpy(),
             (self.catalog['radius_p'].le(1.5)).to_numpy()))
 
     # TODO: Definition of stype here is wrong. It should be an int not a string.
     #   Think about this a bit more. It is important to keep the ints in the DataFrame, but that
     #   decreases usability. Maybe an option is to use intermediate masks for the stellar types.
     def catalog_remove_distance(self,
-                                stype: str,
+                                stype: int,
                                 dist: float,
                                 mode: str):
         """
         Removes planets around stellar type above or below a certain distance from the sample. A
         warning is raise if the mode is not recognized.
 
         Parameters
         ----------
-        stype : str
+        stype : int
             Planets around stars of the specified stellar type are removed. Possible options are
-            'A, 'F', 'G', 'K' and 'M'.
+            `0` for A-stars, `1` for F-stars, `2` for G-stars, `3` for K-stars and `4` for M-stars.
         dist : float
             Specifies the distance over or under which the planets are removed in pc.
         mode : str
             'larger':   planets around stars with distances larger than the specified distance are
                         removed.
             'smaller':  planets around stars with distances smaller than the specified distance are
                         removed.
         """
 
+        # TODO: Reinstate this check once the int/sting problem is resolved.
         # check if stellar type is valid
-        if not np.isin(stype, np.array(('A', 'F', 'G', 'K', 'M'))):
-            raise ValueError('Stellar type not recognised')
+        # if not np.isin(stype, np.array(('A', 'F', 'G', 'K', 'M'))):
+        #     raise ValueError('Stellar type not recognised')
 
         # create masks selecting closer or more far away planets
         if mode == 'larger':
             mask = np.logical_and(self.catalog.stype == stype,
                                   self.catalog.distance_s >= dist)
         elif mode == 'smaller':
             mask = np.logical_and(self.catalog.stype == stype,
@@ -449,15 +410,16 @@
             raise ValueError('Only one-dimensional data can be added')
         if data.shape[0] != self.catalog.nstar.shape[0]:
             raise ValueError('Creation of ragged database is supressed')
         if name in self.catalog.keys():
             raise ValueError('Data can not be overwritten in safe mode')
         self.catalog[name] = data
 
-    def export_catalog(self):
+    def export_catalog(self,
+                       output_path: str):
         """
         Save the catalog to an file in the hdf-format.
 
         Parameters
         ----------
         output_path : str
             path to the new file.
@@ -465,22 +427,15 @@
         Raises
         ------
         ValueError
             If not catalog exists in this data class.
         """
         if self.catalog is None:
             raise ValueError('No catalog found')
-
-        self.str_to_obj(reverse=False)
-        self.catalog.to_hdf(path_or_buf=self.options.other['output_path']
-                                        + self.options.other['output_filename'] + '_catalog.hdf5',
-                            key='catalog',
-                            mode='w')
-        self.str_to_obj(reverse=True)
-        print('Catalog saved')
+        self.catalog.to_hdf(path_or_buf=output_path, key='catalog', mode='w')
 
     def import_catalog(self,
                        input_path: str,
                        overwrite: bool = False):
         """
         Import catalog from external file of hdf-format.
 
@@ -497,28 +452,8 @@
             If the data class already has an initialized catalog and overwrite is set to False.
         """
         if (self.catalog is not None) and (not overwrite):
             raise ValueError('Can not overwrite existing catalog')
 
         self.catalog = pd.read_hdf(path_or_buf=input_path,
                                    key='catalog')
-        self.str_to_obj(reverse=True)
-
-    def str_to_obj(self,
-                   reverse: bool):
-        """
-        Converts all string type columns in the catalog between type 'object' (needed for saving to hdf5) and type
-        'pandas.StringDtype' (needed for fast computation).
 
-        Parameters
-        ----------
-        name_s : bool
-            if reveres is set true, the type will be converted 'object' -> 'pandas.StringDtype'
-        """
-        if not reverse:
-            for key in list(set(self.catalog.keys()[np.where(self.catalog.dtypes == 'string')])
-                            & {'name_s', 'stype'}):
-                self.catalog[key] = self.catalog[key].astype(object)
-        else:
-            for key in list(set(self.catalog.keys()[np.where(self.catalog.dtypes == 'object')])
-                            & {'name_s', 'stype'}):
-                self.catalog[key] = self.catalog[key].astype(pd.StringDtype())
```

### Comparing `LIFEsim-0.2.27/lifesim/core/modules.py` & `LIFEsim-0.2.9/lifesim/core/modules.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,19 +21,16 @@
                         s_type=TransmissionModule,
                         s_number=1)
 
         # the photon noise from the individual sources in calculated in separate modules. The
         # instrument module needs access to their data and control over when they execute
         # TODO: not optimal to hardcode the s_number like this. Maybe find a way to draw it from
         #   options
-        self.add_socket(s_name='photon_noise_star',
-                        s_type=PhotonNoiseStarModule,
-                        s_number=5)
-        self.add_socket(s_name='photon_noise_universe',
-                        s_type=PhotonNoiseUniverseModule,
+        self.add_socket(s_name='photon_noise',
+                        s_type=PhotonNoiseModule,
                         s_number=5)
 
     @abc.abstractmethod
     def get_snr(self):
         """
         The get_snr function should take the existing P-Pop catalog and add the signal-to-noise
         ratio after one hour of integration to this catalog.
@@ -76,39 +73,18 @@
         integration_time : float
             Time that the LIFE array spends for observing the observed planet in [s]
         """
 
         pass
 
 
-class PhotonNoiseStarModule(Module):
-    """
-    Module for simulating astrophysical sources and their photon shot noise contribution specific
-    to a single star to the interferometric measurement.
-    """
-    @abc.abstractmethod
-    def noise(self,
-              index: Union[int, type(None)]):
-        """
-        Calculates the photon shot noise contribution.
-
-        Parameters
-        ----------
-        index : Union[int, type(None)]
-            If an integer is given, the photon noise of the planet corresponding to the respective
-            interger row position in the catalog is given. If `None` is given, the photon noise is
-            calculated for the parameters found in `bus.data.single`.
-        """
-        pass
-
-
-class PhotonNoiseUniverseModule(Module):
+class PhotonNoiseModule(Module):
     """
-    Module for simulating astrophysical sources and their photon shot noise contribution specific
-    to a single universe to the interferometric measurement.
+    Module for simulating astrophysical sources and their photon shot noise contribution to the
+    interferometric measurement.
     """
     @abc.abstractmethod
     def noise(self,
               index: Union[int, type(None)]):
         """
         Calculates the photon shot noise contribution.
```

### Comparing `LIFEsim-0.2.27/lifesim/gui/custom_widgets.py` & `LIFEsim-0.2.9/lifesim/gui/custom_widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,15 @@
 from PyQt5.QtCore import (Qt, QRegExp)
 from PyQt5.QtWidgets import (QLabel, QLineEdit, QWidget, QHBoxLayout, QDoubleSpinBox, QFileDialog,
-                             QPushButton, QButtonGroup, QRadioButton, QVBoxLayout)
+                             QPushButton)
 from PyQt5.QtGui import (QDoubleValidator,QRegExpValidator)
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 
 
-class RadioButtonWidget(QWidget):
-    def __init__(self, *args, **kwargs):
-        super(RadioButtonWidget, self).__init__(*args, **kwargs)
-        hlayout = QHBoxLayout(self)
-        vlayout = QVBoxLayout()
-        bg = QButtonGroup(self)
-
-        self.label = QLabel('Array Baseline')
-
-        self.bl_HZ = QRadioButton("Optimize for eHZ", self)
-        self.bl_HZ.setChecked(True)
-
-        self.bl_pl = QRadioButton("Optimize for Planet", self)
-
-        bg.addButton(self.bl_HZ)
-        bg.addButton(self.bl_pl)
-
-        vlayout.addWidget(self.bl_HZ)
-        vlayout.addWidget(self.bl_pl)
-        vlayout.setAlignment(Qt.AlignRight)
-
-        hlayout.addWidget(self.label)
-        hlayout.addLayout(vlayout)
 
 class DoubleBoxLabel(QWidget):
     def __init__(self, label, mini, maxi, step, value, suffix, *args, **kwargs):
         super(DoubleBoxLabel, self).__init__(*args, **kwargs)
         self.box = QLineEdit()
         self.label = QLabel(text=label)
 
@@ -122,22 +99,22 @@
         layout.addWidget(self.dash)
         layout.addWidget(self.upper)
 
 
 class FileBrowser(QWidget):
     def __init__(self, label, *args, **kwargs):
         super(FileBrowser, self).__init__(*args, **kwargs)
-        self.label = QLabel(label)
+        label = QLabel(label)
         self.filepath = QLineEdit()
         button = QPushButton('Browse...')
 
         button.clicked.connect(self.open_browse)
 
         layout = QHBoxLayout(self)
-        layout.addWidget(self.label)
+        layout.addWidget(label)
         layout.addWidget(self.filepath)
         layout.addWidget(button)
 
     def open_browse(self):
         data_path, _ = QFileDialog.getOpenFileName(self, 'Open File')
         self.filepath.setText(data_path)
```

### Comparing `LIFEsim-0.2.27/lifesim/gui/spectrum_gui.py` & `LIFEsim-0.2.9/lifesim/gui/spectrum_gui.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import math
 import warnings
 import urllib.request
-from urllib.error import HTTPError, URLError
+from urllib.error import HTTPError
 import os
-import sys
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import (QApplication, QDialog, QGroupBox, QGridLayout, QLabel,
-                             QVBoxLayout, QWidget, QHBoxLayout, QProgressBar,
+                             QVBoxLayout, QWidget, QHBoxLayout,
                              QDoubleSpinBox, QPushButton, QTabWidget, QCheckBox,
                              QProgressBar, QComboBox, QSizePolicy)
-from PyQt5.QtGui import QPixmap, QGuiApplication
+from PyQt5.QtGui import QPixmap
 import numpy as np
 from astropy import units as u
 from astropy.visualization import quantity_support
 
 import lifesim as ls
 from lifesim.util.radiation import black_body
 from lifesim.gui.custom_widgets import (DoubleBoxLabel, BoxLabel, StringBoxLabel, DoubleBoxRange,
-                                        FileBrowser, FileSaver, PlotCanvas, RadioButtonWidget)
+                                        FileBrowser, FileSaver, PlotCanvas)
 
 # change the directory to the path of the spectrum_gui.py file to ensure that the logo is imported
 # correctly
 os.chdir(os.path.dirname(__file__))
 
 quantity_support()
 
 try:
     urllib.request.urlretrieve("https://github.com/fdannert/LIFEsim/raw/master/"
                                "lifesim/gui/logo_blue.png", "logo_blue.png")
-except (HTTPError, URLError) as e:
+except HTTPError:
     pass
 
 
 class Frame(QDialog):
     def __init__(self, parent=None):
         super(Frame, self).__init__(parent)
 
@@ -114,109 +113,79 @@
         body_layout.addWidget(sidebar, 0, 0)
         self.setLayout(body_layout)
 
         self.setWindowTitle('LIFEsim lite: Spectrum Simulator')
 
         self.r_spec = None
 
-        self.change_visibility()
-
     def create_instrument(self):
         self.instrument = QGroupBox('Instrument')
 
         self.diameter = DoubleBoxLabel(label='Aperture Diameter',
                                        maxi=10.,
                                        mini=0.25,
                                        step=0.5,
                                        value=2,
                                        suffix='m')
-        self.diameter.label.setToolTip('Diameter of a single aperture of one of the collector spacecraft. The overall'
-                                       'collecting area is spanned by four collector spacecraft')
 
         self.wl_range = DoubleBoxRange(label='Wavelength Range')
-        self.wl_range.label.setToolTip('Lower and upper wavelength bound of the spectrograph')
 
         self.spec_res = BoxLabel(label='Spectral Resolution',
                                  mini=1,
                                  maxi=100,
                                  value=20,
                                  suffix='')
-        self.spec_res.label.setToolTip('Spectral resolution of the spectrograph')
-
-        self.baseline_mode = RadioButtonWidget()
-        self.baseline_mode.label.setToolTip('The distance between the collector spacecraft (i.e. the baseline) <br> '
-                                            'has a major influence on the detectability of exoplanets. It has to be '
-                                            'adjusted '
-                                            'to match the separation between the target exoplanet and its host star. '
-                                            'If the separation of the exoplanet is assumed to be unkown prior to the '
-                                            'observation, the baseline can be set to optimal for planets in the HZ. '
-                                            'If the separation of the target planet is known, the baseline can be set '
-                                            'optimally for the planet position')
-
-        self.baseline_used = QLabel(text='Baseline Used: ')
 
         layout = QGridLayout(self.instrument)
         layout.addWidget(self.diameter.label, 0, 0)
         layout.addWidget(self.diameter, 0, 1)
         layout.addWidget(self.spec_res. label, 1, 0)
         layout.addWidget(self.spec_res, 1, 1)
         layout.addWidget(self.wl_range.label, 2, 0)
         layout.addWidget(self.wl_range, 2, 1)
-        layout.addWidget(self.baseline_mode.label, 3, 0)
-        layout.addWidget(self.baseline_mode.bl_HZ, 3, 1)
-        layout.addWidget(self.baseline_mode.bl_pl, 4, 1)
-        layout.addWidget(self.baseline_used, 5, 0)
 
     def create_star(self):
         self.star = QGroupBox('Star')
         temp = QWidget()
 
         self.temp_s = DoubleBoxLabel(label='Temperature',
                                      mini=0.,
                                      maxi=100000.,
                                      step=100.,
                                      value=5778.,
                                      suffix='K')
-        self.temp_s.label.setToolTip('Temperature of the host star')
+        self.temp_s.label.setToolTip('Test Tip')
 
         self.radius_s = DoubleBoxLabel(label='Radius',
                                        mini=0.,
                                        maxi=2158.,
                                        step=0.5,
                                        value=1.,
                                        suffix='R☉')
-        self.radius_s.label.setToolTip('Radius of the host star')
 
         self.distance_s = DoubleBoxLabel(label='Distance',
                                          mini=0.,
                                          maxi=50.,
                                          step=1.,
                                          value=10.,
                                          suffix='pc')
-        self.distance_s.label.setToolTip('Distance between the solar system and the host star of the target')
 
         self.lat = DoubleBoxLabel(label='Ecliptic Latitude',
                                   mini=0.,
                                   maxi=2*math.pi,
                                   step=0.1,
                                   value=0.79,
                                   suffix='rad')
-        self.lat.label.setToolTip('Ecliptic latitude of the target. Since the localzodiacal dust lies in the <br>'
-                                  'ecplitic of the solar system, this will influence how much localzodi light will '
-                                  'leak into the measurement')
 
         self.z = DoubleBoxLabel(label='Exozodis',
                                 mini=0.,
                                 maxi=20.,
                                 step=0.5,
                                 value=1.,
                                 suffix='z')
-        self.z.label.setToolTip('Exozodi level in the target system. The zodi-number indicates how much more <br>'
-                                'zodiacal dust is present in the target system when compared to the solar system in '
-                                'terms of surface density')
 
         layout = QGridLayout(temp)
         layout.addWidget(self.temp_s.label, 0, 0)
         layout.addWidget(self.temp_s, 0, 1)
 
         layout.addWidget(self.radius_s.label, 1, 0)
         layout.addWidget(self.radius_s, 1, 1)
@@ -238,24 +207,21 @@
 
         self.angsep = DoubleBoxLabel(label='Angular Separation',
                                      mini=0.,
                                      maxi=1.,
                                      value=0.1,
                                      step=0.1,
                                      suffix='arcsec')
-        self.angsep.label.setToolTip('Angular separation between target exoplanet and its host star')
-
 
         self.radius_p = DoubleBoxLabel(label='Radius',
                                        mini=0.,
                                        maxi=10.,
                                        value=1.,
                                        step=0.5,
                                        suffix='R⊕')
-        self.radius_p.label.setToolTip('Radius of the target exoplanets')
 
         layout = QGridLayout(self.planet)
         layout.addWidget(self.angsep.label, 0, 0)
         layout.addWidget(self.angsep, 0, 1)
         layout.addWidget(self.radius_p.label, 1, 0)
         layout.addWidget(self.radius_p, 1, 1)
 
@@ -272,16 +238,14 @@
 
         layout_t = QHBoxLayout(top)
         layout_t.addWidget(self.prev_kind)
         layout_t.addWidget(button)
 
         self.error_field = QLabel()
         self.error_field.setStyleSheet("QLabel { color : red; }")
-        self.error_field.setWordWrap(True)
-
 
         self.p_plot.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
 
         layout = QVBoxLayout(self.s_preview)
         layout.addWidget(top, alignment=Qt.AlignTop)
         layout.addWidget(self.p_plot)
         layout.addWidget(self.error_field, alignment=Qt.AlignBottom)
@@ -336,25 +300,22 @@
         noise = QWidget()
         n_layout = QVBoxLayout(noise)
         n_layout.addWidget(noise_l)
         n_layout.addWidget(self.box_sl)
         n_layout.addWidget(self.box_lz)
         n_layout.addWidget(self.box_ez)
 
-        self.simulate = QPushButton('Run Simulation')
+        simulate = QPushButton('Run Simulation')
 
-        self.simulate.clicked.connect(self.run_simulation)
-
-        self.progress = QProgressBar()
+        simulate.clicked.connect(self.run_simulation)
 
         layout = QVBoxLayout(self.simulation)
         layout.addWidget(t, alignment=Qt.AlignBottom)
         layout.addWidget(noise, alignment=Qt.AlignBottom)
-        layout.addWidget(self.simulate, alignment=Qt.AlignBottom)
-        layout.addWidget(self.progress, alignment=Qt.AlignHCenter)
+        layout.addWidget(simulate, alignment=Qt.AlignBottom)
 
     def create_scenario(self):
         self.scenario = QGroupBox('Set Scenario')
 
         optimisic = QPushButton('Optimistic')
         optimisic.clicked.connect(self.set_scenario_opt)
         baseline = QPushButton('Baseline')
@@ -394,40 +355,25 @@
     def create_input(self):
         self.input = QWidget()
 
         load = QGroupBox('Import')
 
         self.spec_kind = QComboBox()
         self.spec_kind.addItems(['absolute', 'additive', 'contrast'])
-        self.spec_kind.setToolTip('For absolute, the absolute values of the given spectrum are used. For additive, <br>'
-                                  'the values of the given spectrum are added onto a blackbody spectrum based on the '
-                                  'temperature specified for the target planet. For constrast, the values of the given '
-                                  'spectrum are interpreted as contrast values to a blackbody spectrum of the host '
-                                  'star')
 
         self.browse = FileBrowser(label='Spectrum')
-        self.browse.label.setToolTip('Location of the file containing the spectrum. The file should contain two <br>'
-                                     'space-separated columns. The first column should contain the position of the '
-                                     'wavelength bins. The second should contain the flux-like values corresponding to '
-                                     'these wavelength bins')
 
         self.x_units = StringBoxLabel('x-axis units')
-        self.x_units.label.setToolTip(r'Units of the wavelength bin location in the given spectrum. Units can be typed '
-                                      r'in as free text, e.g. "micron"')
         self.y_units = StringBoxLabel('y-axis units')
-        self.y_units.label.setToolTip(r'Units of the flux-like values in the given spectrum. Units can be typed '
-                                      r'in as free text, e.g. "photon micron-1 s-1 m-2"')
         self.temp_p = DoubleBoxLabel(label='Temperature Planet',
                                      mini=0.,
                                      maxi=10000.,
                                      step=1.,
                                      value=0.,
                                      suffix='K')
-        self.temp_p.label.setToolTip('Temperature of the target planet')
-
         temp = QWidget()
         ly = QHBoxLayout(temp)
         ly.addWidget(self.temp_p.label)
         ly.addWidget(self.temp_p)
 
         layout_l = QVBoxLayout(load)
         layout_l.addWidget(self.spec_kind)
@@ -443,37 +389,28 @@
 
         self.distance_spec = DoubleBoxLabel(label='Distance',
                                             mini=0.,
                                             maxi=50.,
                                             step=1.,
                                             value=0.,
                                             suffix='pc')
-        self.distance_spec.label.setToolTip('If a distance to the target system was used during the creation of <br>'
-                                            ' the spectrum, specify it here. This will allow LIFEsim to simulate the '
-                                            'planet at different distances to the solar system specified in the '
-                                            'settings tab')
 
         self.radius_spec = DoubleBoxLabel(label='Radius Planet',
                                           mini=0.,
                                           maxi=10.,
                                           value=0.,
                                           step=0.5,
                                           suffix='R⊕')
-        self.radius_spec.label.setToolTip('If a radius of the target planet was used during the creation of <br>'
-                                          ' the spectrum, specify it here. This will allow LIFEsim to simulate the '
-                                          'planet in idfferent sizes specified in the settings tab')
 
         self.time_spec = DoubleBoxLabel(label='Integration Time',
                                         mini=0.,
                                         maxi=60.*60.*24.*365.*10.,
                                         step=60.,
                                         value=0.,
                                         suffix='s')
-        self.time_spec.label.setToolTip('If an integration time was used during the creation of the spectrum, specify '
-                                        'it here')
 
         layout_p = QGridLayout(param)
         layout_p.addWidget(self.distance_spec.label, 0, 0)
         layout_p.addWidget(self.distance_spec, 0, 1)
         layout_p.addWidget(self.radius_spec.label, 1, 0)
         layout_p.addWidget(self.radius_spec, 1, 1)
         layout_p.addWidget(self.time_spec.label, 2, 0)
@@ -624,24 +561,16 @@
                                                   (self.bus.data.options.array['wl_max']
                                                    *u.micron))[0])])).value)
 
             self.p_plot.axes.set_yscale('log')
             self.p_plot.axes.grid()
             self.p_plot.axes.ticklabel_format(axis='x', style='sci')
             self.p_plot.draw()
-        except Exception as e:
-            exc_type, exc_obj, exc_tb = sys.exc_info()
-            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            print(exc_type, fname, exc_tb.tb_lineno)
-            self.error_field.setText('Import Error: '
-                                     + str(e) + '; '
-                                     + str(exc_type) + '; '
-                                     + str(fname) + '; '
-                                     + str(exc_tb.tb_lineno))
-
+        except:
+            self.error_field.setText('An error occured during import')
 
     def show_spectrum(self,
                       spectrum,
                       planet,
                       noise):
         self.r_plot.axes.cla()
         self.r_plot.axes.step(spectrum[0] * 1e6, planet / (self.time_b.value()*60*60),
@@ -677,65 +606,43 @@
         ax2a.set_ylim(d_min, d_max)
 
         self.r_plot.draw()
 
         ax2a.remove()
 
     def run_simulation(self):
-        self.progress.setValue(10)
-        QGuiApplication.processEvents()
-
         self.show_preview()
         self.update_options()
 
-        self.progress.setValue(20)
-        QGuiApplication.processEvents()
-
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             self.bus.disconnect(module_names=('life', 'sl'))
             self.bus.disconnect(module_names=('life', 'lz'))
             self.bus.disconnect(module_names=('life', 'ez'))
         if self.box_sl.isChecked():
             self.bus.connect(module_names=('life', 'sl'))
         if self.box_lz.isChecked():
             self.bus.connect(module_names=('life', 'lz'))
         if self.box_ez.isChecked():
             self.bus.connect(module_names=('life', 'ez'))
 
-        self.progress.setValue(30)
-        QGuiApplication.processEvents()
-
         self.r_spec, self.flux_p, self.flux_n = self.bus.modules['life'].get_spectrum(
             temp_s=self.temp_s.value(),
             radius_s=self.radius_s.value(),
             distance_s=self.distance_s.value(),
             flux_planet_spectrum=self.flux_planet_spectrum,
             lat_s=self.lat.value(),
             z=self.z.value(),
             angsep=self.angsep.value(),
-            integration_time=self.time_b.value()*60*60,
-            baseline_to_planet=self.baseline_mode.bl_pl.isChecked(),
-            pbar=self.progress)
-
-        self.progress.setValue(90)
-        QGuiApplication.processEvents()
+            integration_time=self.time_b.value()*60*60)
 
         self.show_spectrum(self.r_spec,
                            self.flux_p,
                            self.flux_n)
 
-        self.baseline_used.setText('Nulling Baseline Used: '
-                                   + str(np.round(self.bus.data.inst['bl'],
-                                                  decimals=1))
-                                   + ' m')
-
-        self.progress.setValue(100)
-        QGuiApplication.processEvents()
-
     def set_values(self):
         self.diameter.set(self.bus.data.options.array['diameter'])
         self.spec_res.set(self.bus.data.options.array['spec_res'])
         self.wl_range.lower.setValue(self.bus.data.options.array['wl_min'])
         self.wl_range.upper.setValue(self.bus.data.options.array['wl_max'])
 
     def set_scenario_opt(self):
@@ -756,52 +663,34 @@
                        X=np.array([self.r_spec[0], self.r_spec[1], self.flux_p]).T,
                        header='Wavelength [m]   SNR per bin for 1h  Input flux')
 
     def change_visibility(self):
         if self.spec_kind.currentText() == 'additive':
             self.temp_p.show()
             self.temp_p.label.setText('Temperature Planet')
-            self.temp_p.label.show()
             self.x_units.show()
-            self.x_units.label.show()
             self.y_units.show()
-            self.y_units.label.show()
             self.distance_spec.show()
-            self.distance_spec.label.show()
             self.radius_spec.show()
-            self.radius_spec.label.show()
             self.time_spec.show()
-            self.time_spec.label.show()
         elif self.spec_kind.currentText() == 'absolute':
             self.temp_p.hide()
-            self.temp_p.label.hide()
             self.x_units.show()
-            self.x_units.label.show()
             self.y_units.show()
-            self.y_units.label.show()
             self.distance_spec.show()
-            self.distance_spec.label.show()
             self.radius_spec.show()
-            self.radius_spec.label.show()
             self.time_spec.show()
-            self.time_spec.label.show()
         elif self.spec_kind.currentText() == 'contrast':
-            self.temp_p.show()
+            self.temp_p.hide()
             self.temp_p.label.setText('Temperature Star')
-            self.temp_p.label.show()
             self.x_units.show()
-            self.x_units.label.show()
             self.y_units.hide()
-            self.y_units.label.hide()
             self.distance_spec.hide()
-            self.distance_spec.label.hide()
             self.radius_spec.hide()
-            self.radius_spec.label.hide()
             self.time_spec.hide()
-            self.time_spec.label.hide()
 
 
 class Gui(object):
     def __init__(self):
         os.chdir(os.path.dirname(__file__))
         quantity_support()
         app = QApplication([])
```

### Comparing `LIFEsim-0.2.27/lifesim/instrument/pn_exozodi.py` & `LIFEsim-0.2.9/lifesim/instrument/pn_exozodi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 from typing import Union
 
-from lifesim.core.modules import PhotonNoiseUniverseModule
+from lifesim.core.modules import PhotonNoiseModule
 from lifesim.util import constants
 from lifesim.util.radiation import black_body
 
 
-class PhotonNoiseExozodi(PhotonNoiseUniverseModule):
+class PhotonNoiseExozodi(PhotonNoiseModule):
     """
     This class simulates the noise contribution of an exozodi disk to the interferometric
     measurement of LIFE.
     """
 
     def __init__(self,
                  name: str):
```

### Comparing `LIFEsim-0.2.27/lifesim/instrument/pn_localzodi.py` & `LIFEsim-0.2.9/lifesim/instrument/pn_localzodi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Union
 
 import numpy as np
 
-from lifesim.core.modules import PhotonNoiseStarModule
+from lifesim.core.modules import PhotonNoiseModule
 from lifesim.util.radiation import black_body
 
 
-class PhotonNoiseLocalzodi(PhotonNoiseStarModule):
+class PhotonNoiseLocalzodi(PhotonNoiseModule):
     """
     This class simulates the noise contribution of the thermal localzodical dust to the
     interferometric measurement of LIFE.
     """
 
     def __init__(self,
                  name: str):
```

### Comparing `LIFEsim-0.2.27/lifesim/instrument/pn_star.py` & `LIFEsim-0.2.9/lifesim/instrument/pn_star.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Union
 
 import numpy as np
 
-from lifesim.core.modules import PhotonNoiseStarModule, TransmissionModule
+from lifesim.core.modules import PhotonNoiseModule, TransmissionModule
 from lifesim.util.radiation import black_body
 
 
-class PhotonNoiseStar(PhotonNoiseStarModule):
+class PhotonNoiseStar(PhotonNoiseModule):
     """
     This class simulates the noise contribution of central star to the interferometric measurement
     of LIFE due to leakage through the null.
     """
 
     def __init__(self,
                  name: str):
```

### Comparing `LIFEsim-0.2.27/lifesim/instrument/transmission.py` & `LIFEsim-0.2.9/lifesim/instrument/transmission.py`

 * *Files identical despite different names*

### Comparing `LIFEsim-0.2.27/lifesim/optimize/ahgs.py` & `LIFEsim-0.2.9/lifesim/optimize/ahgs.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,16 @@
     def __init__(self,
                  name: str):
         super().__init__(name=name)
 
     def obs_array_star(self, nstar):
         mask = self.data.catalog.nstar == nstar
 
-        # return infinity if the detection limit is reached for this stype
         if not bool(np.isin(element=self.data.catalog.stype.loc[mask].iloc[0],
-                            test_elements=np.array(list(self.data.options.optimization['limit'].keys()))[np.invert(
+                            test_elements=self.data.options.optimization['limit'][0][np.invert(
                                 self.data.optm['hit_limit'])])):
             return np.array((np.inf, np.inf))
         else:
             if self.data.options.optimization['habitable']:
                 mask = np.logical_and.reduce((mask,
                                               self.data.catalog.habitable,
                                               np.invert(self.data.catalog.detected)))
@@ -60,17 +59,17 @@
 
             for _, i in enumerate(np.where(mask)[0]):
                 if (not self.data.catalog.detected.iloc[i]) and \
                         (self.data.catalog.snr_current.iloc[i]
                          >= self.data.options.optimization['snr_target']):
                     self.data.catalog.detected.iat[i] = True
                     if self.data.catalog.habitable.iloc[i]:
-                        self.data.optm['sum_detected'][
-                            np.where(np.array(list(self.data.options.optimization['limit'].keys()))
-                                     == self.data.catalog.stype.iloc[i])] += 1
+                        self.data.optm['sum_detected'][np.where(
+                            self.data.options.optimization['limit'][0][:]
+                            == self.data.catalog.stype.iloc[i])] += 1
         else:
             pass
             # self.planets.slew_time[mask_star] = -self.t_slew
             # self.planets.int_time[mask_star] = 0
             # self.planets.SNR_prediction_sum[mask_star] = 0
             # for _, i in enumerate(np.where(mask_star)[0]):
             #     if self.planets.detected[i] and self.planets.habitable[i]:
@@ -89,16 +88,14 @@
             obs[i, :temp.shape[0]] = temp
 
         obs_time = (self.data.options.optimization['t_search']
                     * self.data.options.array['t_efficiency'])
 
         tot_time = 0
 
-        print('Number of planets detected by stellar type:')
-
         while tot_time < obs_time:
             # find the best global slope and observe star
             no_star, ind_t = np.unravel_index(np.argmin(obs), obs.shape)
             if (tot_time + obs[no_star, ind_t] * (ind_t + 1) + 0.01) > obs_time:
                 rem_time = obs_time - tot_time
                 self.observe_star(nstar=stars[no_star],
                                   int_time=rem_time)
@@ -114,33 +111,24 @@
                 self.observe_star(nstar=stars[no_star],
                                   int_time=obs[no_star, ind_t] * (ind_t + 1) + 0.01)
                 temp = self.obs_array_star(nstar=stars[no_star])
                 tot_time += obs[no_star, ind_t] * (ind_t + 1) + 0.01
                 obs[no_star, :] = np.inf
                 obs[no_star, :temp.shape[0]] = temp
 
-            out_string = ''
-            for key in self.data.options.optimization['limit'].keys():
-                out_string += (key + ': '
-                               + str((self.data.optm['sum_detected'] / self.data.optm['num_universe'])[
-                                         np.where(np.array(list(self.data.options.optimization['limit'].keys()))
-                                                  == key)][0])
-                               + '  ')
-            out_string += ('-  (' + str(np.round(tot_time/60/60/24/365.25, 1)) + ' / '
-                           + str(np.round(obs_time/60/60/24/365.25, 1)) + ') yrs observed')
-            print('\r' + out_string, end='')
+            print(self.data.optm['sum_detected']/500)
 
             if np.any(
                     np.logical_and(
                         (self.data.optm['sum_detected'] / self.data.optm['num_universe'])
-                        > np.array(list(self.data.options.optimization['limit'].values())),
+                        > self.data.options.optimization['limit'][1][:],
                         np.invert(self.data.optm['hit_limit']))):
                 print('HIT LIMIT, RECOUNTING -------------------')
                 self.data.optm['hit_limit'] = ((self.data.optm['sum_detected']
-                                                / (self.data.optm['num_universe']))
+                                                / (self.data.optm['num_universe'] + 1))
                                                >= self.data.options.optimization['limit'][1][:])
                 obs = np.zeros((stars.shape[0], np.max(n))) + np.inf
 
                 # fill the observation time array
                 for i, nstar in enumerate(stars):
                     temp = self.obs_array_star(nstar=nstar)
                     obs[i, :temp.shape[0]] = temp
```

### Comparing `LIFEsim-0.2.27/lifesim/optimize/optimizer.py` & `LIFEsim-0.2.9/lifesim/optimize/optimizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,30 +58,25 @@
                         np.cos(self.data.catalog.small_omega_p.iloc[n_p]
                                + self.data.catalog.theta_p.iloc[n_p]) ** 2
                         + np.cos(self.data.catalog.inc_p.iloc[n_p]) ** 2
                         * np.sin(self.data.catalog.small_omega_p.iloc[n_p]
                                  + self.data.catalog.theta_p.iloc[n_p]) ** 2))
             self.data.catalog.snr_new.iat[n_p] = self.data.catalog.snr_phase.iloc[n_p][0][i]
 
+
     def ahgs(self):
-        # set 0 if type limit is not hit
         self.data.optm['hit_limit'] = np.zeros(5)
-
-        # sum of detected planets per stype
         self.data.optm['sum_detected'] = np.zeros(5)
-
-        self.data.optm['num_universe'] = self.data.catalog.nuniverse.max() + 1
+        self.data.optm['num_universe'] = self.data.catalog.nuniverse.max()
         self.data.optm['hit_limit'] = ((self.data.optm['sum_detected']
-                                       / (self.data.optm['num_universe']))
-                                       >= np.array(list(self.data.options.optimization['limit'].values())))
-
-        self.data.optm['tot_time'] = 0  # in sec
+                                       / (self.data.optm['num_universe'] + 1))
+                                       >= self.data.options.optimization['limit'][1][:])
+        self.data.optm['tot_time'] = 0
 
-        # add new columns to catalog
         self.data.catalog['detected'] = False
         self.data.catalog['snr_current'] = 0.
         self.data.catalog['int_time'] = 0.
         self.data.catalog['t_slew'] = -self.data.options.array['t_slew']
-
         self.run_socket(s_name='slope',
                         method='distribute_time')
-        print('')
+
+
```

### Comparing `LIFEsim-0.2.27/lifesim/util/habitable.py` & `LIFEsim-0.2.9/lifesim/util/habitable.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,41 +39,27 @@
     """
     # model based on Kaltenegger+2017
     if model == 'MS':
         s0_in, s0_out = 1.7665, 0.3240
         a_in, a_out = 1.3351E-4, 5.3221E-5
         b_in, b_out = 3.1515E-9, 1.4288E-9
         c_in, c_out = -3.3488E-12, -1.1049E-12
-        d_in, d_out = 0, 0
     elif model == 'POST-MS':
         s0_in, s0_out = 1.1066, 0.3240
         a_in, a_out = 1.2181E-4, 5.3221E-5
         b_in, b_out = 1.5340E-8, 1.4288E-9
         c_in, c_out = -1.5018E-12, -1.1049E-12
-        d_in, d_out = 0, 0
-    elif model == 'Kopparapu-Optimistic':
-        s0_in, s0_out = 1.776, 0.32
-        a_in, a_out = 2.136e-4, 5.547e-5
-        b_in, b_out = 2.533e-8, 1.526e-9
-        c_in, c_out = -1.332e-11, -2.874e-12
-        d_in, d_out = -3.097e-15, -5.011e-16
-    elif model == 'Kopparapu-Conservative':
-        s0_in, s0_out = 1.107, 0.356
-        a_in, a_out = 1.332e-4, 6.171e-5
-        b_in, b_out = 1.58e-8, 1.698e-9
-        c_in, c_out = -8.308e-12, -3.198e-12
-        d_in, d_out = -1.931e-15, -5.575e-16
     else:
         raise ValueError('Unknown model')
 
     t_star = temp_s - 5780
 
     # in units of incoming flux, normalized to stellar flux on earth_0
-    s_in = s0_in + a_in * t_star + b_in * t_star ** 2 + c_in * t_star ** 3 + d_in * t_star ** 4
-    s_out = s0_out + a_out * t_star + b_out * t_star ** 2 + c_out * t_star ** 3 + d_out * t_star ** 4
+    s_in = s0_in + a_in * t_star + b_in * t_star ** 2 + c_in * t_star ** 3
+    s_out = s0_out + a_out * t_star + b_out * t_star ** 2 + c_out * t_star ** 3
     l_sun = radius_s ** 2 * (temp_s / 5780) ** 4  # luminosity in L_sun
 
     hz_in = np.sqrt(l_sun / s_in)  # HZ inner boundery in AU
     hz_out = np.sqrt(l_sun / s_out)  # HZ outer boundery in AU
     hz_center = (hz_in + hz_out) / 2  # HZ center  in AU
 
     return s_in, s_out, l_sun, hz_in, hz_out, hz_center
```

### Comparing `LIFEsim-0.2.27/lifesim/util/importer.py` & `LIFEsim-0.2.9/lifesim/util/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,35 +42,27 @@
 
     def to_per_second(self):
         if self.integration_time != 0.:
             self.y_data = (self.y_data / (self.integration_time * u.s)).decompose()
 
     def adjust_to_target(self):
         if self.distance_s_spectrum == 0:
-            self.y_data = self.y_data / (self.distance_s_target * u.pc)**2 / np.pi
+            self.y_data = self.y_data / (self.distance_s_target * u.pc)**2 / 4
         elif self.distance_s_spectrum is None:
             pass
         else:
             self.y_data = self.y_data * (self.distance_s_spectrum / self.distance_s_target)**2
         if self.radius_p_spectrum == 0:
-            self.y_data = self.y_data * np.pi * (self.radius_p_target * c.R_earth)**2
+            self.y_data = self.y_data * 4 * np.pi * (self.radius_p_target * c.R_earth)**2
         elif self.radius_p_spectrum is None:
             pass
         else:
             self.y_data = self.y_data * (self.radius_p_target / self.radius_p_spectrum)**2
         self.y_data = self.y_data.decompose()
 
-    def remove_sr(self):
-        if u.rad in self.y_data.unit.decompose().bases:
-            if (self.y_data.unit.powers[np.where(np.equal(np.array(self.y_data.unit.decompose().bases), u.rad))[0][0]]
-                    == -2):
-                self.y_data = self.y_data * u.sr * np.pi
-            else:
-                raise ValueError('Given units cannot be converted to units required by LIFEsim')
-
     # TODO: Implement that the user can select which column is x and which is y
     # TODO: Check whether the vector is [N,2] or [2,N] and transpose accordingly
     # TODO: Ignore any non-numeric values during import
     def import_spectrum(self):
         spec = np.loadtxt(self.pathtotxt).T
         self.x_data = (spec[0] * u.Unit(self.x_string)).decompose()
         self.y_data = (spec[1] * u.Unit(self.y_string)).decompose()
@@ -112,20 +104,16 @@
         self.update_pathtotext(pathtotext)
         self.update_x(x_string)
         self.update_y(y_string)
         self.import_spectrum()
         self.to_wavelength()
         self.to_counts()
         self.to_per_second()
-        self.remove_sr()
         self.adjust_to_target()
 
-        if (self.y_data.unit != (u.ph / u.m ** 3 / u.s)) or (self.x_data.unit != u.m):
-            raise ValueError('Given units cannot be converted to units required by LIFEsim')
-
 # all settings
 # in_string = 'erg cm-2 s-1 Hz-1'
 # x_string = 'Hz'
 # radius_p = None
 # observation_time = None
 # distance_s = None
 #
```

### Comparing `LIFEsim-0.2.27/lifesim/util/options.py` & `LIFEsim-0.2.9/lifesim/util/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,17 +69,15 @@
                       'bl_max': 0.,
                       'ratio': 0.,
                       't_slew': 0.,
                       't_efficiency': 0.}
 
         self.other = {'image_size': 0,
                       'wl_optimal': 0.,
-                      'n_plugins': 0,
-                      'output_path': None,
-                      'output_filename': None}
+                      'n_plugins': 0}
 
         self.models = {'localzodi': '',
                        'habitable': ''}
 
         self.optimization = {'N_pf': 0.,
                              'snr_target': 0.,
                              'limit': None,
@@ -113,19 +111,16 @@
         self.other['n_plugins'] = 5
 
         self.models['localzodi'] = 'darwinsim'
         self.models['habitable'] = 'MS'
 
         self.optimization['N_pf'] = 25
         self.optimization['snr_target'] = 7
-        self.optimization['limit'] = {'A': np.inf,
-                                      'F': np.inf,
-                                      'G': np.inf,
-                                      'K': np.inf,
-                                      'M': np.inf}
+        self.optimization['limit'] = np.array(((0, 1, 2, 3, 4),
+                                               (np.inf, np.inf, np.inf, np.inf, np.inf)))
         self.optimization['habitable'] = True
         self.optimization['t_search'] = 2.5 * 365. * 24. * 60. * 60.
 
         if case == 'baseline':
             self.array['diameter'] = 2.
             self.array['wl_min'] = 4.
             self.array['wl_max'] = 18.5
```

### Comparing `LIFEsim-0.2.27/lifesim/util/radiation.py` & `LIFEsim-0.2.9/lifesim/util/radiation.py`

 * *Files identical despite different names*

