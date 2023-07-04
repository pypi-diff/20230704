# Comparing `tmp/lbh15-1.1.1.tar.gz` & `tmp/lbh15-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbh15-1.1.1.tar", last modified: Fri Mar 24 10:49:27 2023, max compression
+gzip compressed data, was "lbh15-1.2.0.tar", last modified: Tue Jul  4 08:32:19 2023, max compression
```

## Comparing `lbh15-1.1.1.tar` & `lbh15-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-03-24 10:49:27.751951 lbh15-1.1.1/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     7651 2022-11-15 12:45:34.000000 lbh15-1.1.1/LICENSE
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       34 2022-11-15 12:45:34.000000 lbh15-1.1.1/MANIFEST.in
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3624 2023-03-24 10:49:27.751951 lbh15-1.1.1/PKG-INFO
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1986 2023-03-24 09:59:16.000000 lbh15-1.1.1/README.rst
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-03-24 10:49:27.751951 lbh15-1.1.1/lbh15/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      386 2023-03-24 10:03:30.000000 lbh15-1.1.1/lbh15/__init__.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      769 2023-01-10 09:14:14.000000 lbh15-1.1.1/lbh15/_constants.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    21142 2023-03-24 09:35:43.000000 lbh15-1.1.1/lbh15/_lbh15.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2144 2023-01-10 09:14:14.000000 lbh15-1.1.1/lbh15/bismuth.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2105 2023-01-10 09:14:14.000000 lbh15-1.1.1/lbh15/lbe.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2431 2023-01-10 09:14:14.000000 lbh15-1.1.1/lbh15/lead.py
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-03-24 10:49:27.751951 lbh15-1.1.1/lbh15/properties/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       54 2023-01-10 09:14:14.000000 lbh15-1.1.1/lbh15/properties/__init__.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    17148 2023-03-24 09:35:43.000000 lbh15-1.1.1/lbh15/properties/bismuth_properties.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     8972 2023-03-24 09:35:43.000000 lbh15-1.1.1/lbh15/properties/interface.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    17074 2023-03-24 09:35:43.000000 lbh15-1.1.1/lbh15/properties/lbe_properties.py
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    18940 2023-03-24 09:35:43.000000 lbh15-1.1.1/lbh15/properties/lead_properties.py
-drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-03-24 10:49:27.751951 lbh15-1.1.1/lbh15.egg-info/
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3624 2023-03-24 10:49:27.000000 lbh15-1.1.1/lbh15.egg-info/PKG-INFO
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      450 2023-03-24 10:49:27.000000 lbh15-1.1.1/lbh15.egg-info/SOURCES.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        1 2023-03-24 10:49:27.000000 lbh15-1.1.1/lbh15.egg-info/dependency_links.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       27 2023-03-24 10:49:27.000000 lbh15-1.1.1/lbh15.egg-info/requires.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        6 2023-03-24 10:49:27.000000 lbh15-1.1.1/lbh15.egg-info/top_level.txt
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       38 2023-03-24 10:49:27.751951 lbh15-1.1.1/setup.cfg
--rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3196 2023-03-24 10:43:48.000000 lbh15-1.1.1/setup.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-07-04 08:32:19.476410 lbh15-1.2.0/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     7651 2023-04-12 12:31:38.000000 lbh15-1.2.0/LICENSE
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       34 2023-04-12 12:31:38.000000 lbh15-1.2.0/MANIFEST.in
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2963 2023-07-04 08:32:19.476410 lbh15-1.2.0/PKG-INFO
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1945 2023-07-04 08:13:45.000000 lbh15-1.2.0/README.rst
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-07-04 08:32:19.476410 lbh15-1.2.0/lbh15/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      352 2023-07-04 08:13:30.000000 lbh15-1.2.0/lbh15/__init__.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      725 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/_commons.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    21215 2023-06-28 09:37:19.000000 lbh15-1.2.0/lbh15/_lbh15.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2159 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/bismuth.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2122 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/lbe.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2448 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/lead.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-07-04 08:32:19.476410 lbh15-1.2.0/lbh15/properties/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       54 2023-04-12 12:31:38.000000 lbh15-1.2.0/lbh15/properties/__init__.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    17108 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/properties/bismuth_properties.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     8951 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/properties/interface.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    17034 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/properties/lbe_properties.py
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)    18898 2023-06-07 13:37:33.000000 lbh15-1.2.0/lbh15/properties/lead_properties.py
+drwxr-xr-x   0 daniele.panico (1881201246) domain users (1881200513)        0 2023-07-04 08:32:19.476410 lbh15-1.2.0/lbh15.egg-info/
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     2963 2023-07-04 08:32:19.000000 lbh15-1.2.0/lbh15.egg-info/PKG-INFO
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)      463 2023-07-04 08:32:19.000000 lbh15-1.2.0/lbh15.egg-info/SOURCES.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        1 2023-07-04 08:32:19.000000 lbh15-1.2.0/lbh15.egg-info/dependency_links.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       27 2023-07-04 08:32:19.000000 lbh15-1.2.0/lbh15.egg-info/requires.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)        6 2023-07-04 08:32:19.000000 lbh15-1.2.0/lbh15.egg-info/top_level.txt
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     1327 2023-07-04 08:24:31.000000 lbh15-1.2.0/pyproject.toml
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)       38 2023-07-04 08:32:19.476410 lbh15-1.2.0/setup.cfg
+-rw-r--r--   0 daniele.panico (1881201246) domain users (1881200513)     3884 2023-07-04 08:25:35.000000 lbh15-1.2.0/setup.py
```

### Comparing `lbh15-1.1.1/LICENSE` & `lbh15-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lbh15-1.1.1/README.rst` & `lbh15-1.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lbh15
 =====
 
 :Author: Daniele Panico, Daniele Tomatis
-:Date: 03/24/2023
+:Date: 07/04/2023
 
 Introduction
 ------------
 
 lbh15 (**L**\ ead **B**\ ismuth **H**\ andbook 20\ **15**) is a Python package that implements the
 thermo-physical properties of lead, bismuth and lead-bismuth eutectic (lbe) metal alloy available from
 the handbook edited by 
@@ -67,12 +67,10 @@
  
   .. code-block:: bash
 
       make html
  
   .. code-block:: bash
 
-      make latex
-      cd _build/latex
-      latexmk -pdf -f
+      make latexpdf
 
 The html documentation is available on GitHub Pages at `newcleo-dev-team.github.io/lbh15 <https://newcleo-dev-team.github.io/lbh15/index.html>`_.
```

### Comparing `lbh15-1.1.1/lbh15/_constants.py` & `lbh15-1.2.0/lbh15/_commons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module with the definition of constants for lbh15 package"""
+"""Module with the definition of common objects for lbh15 package"""
 # KEYWORDS
 GURVICH_KEYWORD = 'gurvich1991'
 SOBOLEV_KEYWORD = 'sobolev2011'
 
 # LEAD CONSTANTS
 LEAD_MELTING_TEMPERATURE = 600.6  # [K]
 LEAD_MELTING_LATENT_HEAT = 23.07e3  # [J/kg]
@@ -16,10 +16,7 @@
 BISMUTH_VAPORISATION_HEAT = 856.2e3  # [J/kg]
 
 # LEAD-BISMUTH-EUTECTIC CONSTANTS
 LBE_MELTING_TEMPERATURE = 398.0  # [K]
 LBE_MELTING_LATENT_HEAT = 38.6e3  # [J/kg]
 LBE_BOILING_TEMPERATURE = 1927  # [K]
 LBE_VAPORISATION_HEAT = 856.6e3  # [J/kg]
-
-# ATMOSPHERIC PRESSURE
-P_ATM = 101325.0  # [Pa]
```

### Comparing `lbh15-1.1.1/lbh15/_lbh15.py` & `lbh15-1.2.0/lbh15/_lbh15.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import warnings
 import sys
 import inspect
 import importlib
 import platform
 import copy
 from abc import ABC, abstractmethod
+from scipy.constants import atm
+from scipy.optimize import fsolve
 from .properties.interface import PropertyInterface
-from ._constants import P_ATM
 
 
 class LiquidMetalInterface(ABC):
     """
     Abstract class that defines liquid metal properties object
 
     Parameters
@@ -46,15 +47,15 @@
     _roots_to_use = {}
     _default_corr_to_use = {}
     _properties_module = ""
     __p = 0
     __T = 0
     __custom_properties_path = {}
 
-    def __init__(self, p=P_ATM, **kwargs):
+    def __init__(self, p=atm, **kwargs):
         self.__assign_p(p)
         self.__properties = {}
         self.__corr2use = copy.deepcopy(self.__class__._correlations_to_use)
         self.__fill_instance_properties()
         self.__fill_class_attributes(kwargs)
 
     @property
@@ -333,16 +334,14 @@
             key = self.__generate_key(input_property)
             if key in self.__properties:
                 function_of_T = self.__properties[key].correlation
                 helper = self.__properties[key].initialization_helper
                 is_injective = self.__properties[key].is_injective
 
             if function_of_T is not None:
-                from scipy.optimize import fsolve
-
                 if helper(input_value) is not None:
                     self._guess = helper(input_value)
 
                 def function_to_solve(T, target):
                     return function_of_T(T, self.__p) - target
 
                 if is_injective:
@@ -579,15 +578,17 @@
             lm_path = cls.__custom_properties_path[cls.__name__]
             for path in lm_path.keys():
                 if path not in sys.path:
                     sys.path.append(path)
                 module_name = lm_path[path]
                 module = importlib.import_module(module_name)
                 for _, obj in inspect.getmembers(module):
-                    if inspect.isclass(obj) and obj is not PropertyInterface:
+                    if (inspect.isclass(obj)
+                            and obj is not PropertyInterface
+                            and not inspect.isabstract(obj)):
                         if issubclass(obj, PropertyInterface):
                             customproperty_obj_list.append(obj())
         return customproperty_obj_list
 
     @abstractmethod
     def _set_constants(self):
         """
```

### Comparing `lbh15-1.1.1/lbh15/bismuth.py` & `lbh15-1.2.0/lbh15/bismuth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module with the definition of bismuth liquid metal object class,
 i.e., Bismuth"""
-from ._constants import BISMUTH_MELTING_TEMPERATURE
-from ._constants import BISMUTH_MELTING_LATENT_HEAT
-from ._constants import BISMUTH_BOILING_TEMPERATURE
-from ._constants import BISMUTH_VAPORISATION_HEAT, P_ATM
+from scipy.constants import atm
+from ._commons import BISMUTH_MELTING_TEMPERATURE
+from ._commons import BISMUTH_MELTING_LATENT_HEAT
+from ._commons import BISMUTH_BOILING_TEMPERATURE
+from ._commons import BISMUTH_VAPORISATION_HEAT
 from ._lbh15 import LiquidMetalInterface
 
 
 class Bismuth(LiquidMetalInterface):
     """
     Class to model liquid bismuth properties at a given temperature
 
@@ -41,15 +42,15 @@
     13.705
     """
     _default_corr_to_use = {}
     _correlations_to_use = {}
     _roots_to_use = {'cp': 0}
     _properties_module = 'lbh15.properties.bismuth_properties'
 
-    def __init__(self, p=P_ATM, **kwargs):
+    def __init__(self, p=atm, **kwargs):
         self._guess = BISMUTH_MELTING_TEMPERATURE*1.5
         super().__init__(p=p, **kwargs)
 
     def _set_constants(self):
         """
         Sets the class constants
         """
```

### Comparing `lbh15-1.1.1/lbh15/lbe.py` & `lbh15-1.2.0/lbh15/lbe.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with the definition of lead-bismuth eutectic
 liquid metal object class, i.e., LBE"""
-from ._constants import LBE_MELTING_TEMPERATURE
-from ._constants import LBE_MELTING_LATENT_HEAT, LBE_BOILING_TEMPERATURE
-from ._constants import LBE_VAPORISATION_HEAT, P_ATM
+from scipy.constants import atm
+from ._commons import LBE_MELTING_TEMPERATURE
+from ._commons import LBE_MELTING_LATENT_HEAT, LBE_BOILING_TEMPERATURE
+from ._commons import LBE_VAPORISATION_HEAT
 from ._lbh15 import LiquidMetalInterface
 
 
 class LBE(LiquidMetalInterface):
     """
     Class to model liquid lead-bismuth eutectic properties
     at a given temperature
@@ -41,15 +42,15 @@
     0.001736052003181349
     """
     _default_corr_to_use = {}
     _correlations_to_use = {}
     _roots_to_use = {'cp': 0}
     _properties_module = 'lbh15.properties.lbe_properties'
 
-    def __init__(self, p=P_ATM, **kwargs):
+    def __init__(self, p=atm, **kwargs):
         self._guess = LBE_MELTING_TEMPERATURE*2.0
         super().__init__(p=p, **kwargs)
 
     def _set_constants(self):
         """
         Sets the class constants
         """
```

### Comparing `lbh15-1.1.1/lbh15/lead.py` & `lbh15-1.2.0/lbh15/lead.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module with the definition of lead liquid metal object class,
 i.e., Lead"""
 import copy
-from ._constants import LEAD_MELTING_TEMPERATURE
-from ._constants import LEAD_MELTING_LATENT_HEAT, LEAD_BOILING_TEMPERATURE
-from ._constants import SOBOLEV_KEYWORD, LEAD_VAPORISATION_HEAT, P_ATM
+from scipy.constants import atm
+from ._commons import LEAD_MELTING_TEMPERATURE
+from ._commons import LEAD_MELTING_LATENT_HEAT, LEAD_BOILING_TEMPERATURE
+from ._commons import SOBOLEV_KEYWORD, LEAD_VAPORISATION_HEAT
 from ._lbh15 import LiquidMetalInterface
 
 
 class Lead(LiquidMetalInterface):
     """
     Class to model liquid lead properties at a given temperature
 
@@ -48,15 +49,15 @@
     144.66006199999998
     """
     _default_corr_to_use = {'cp': SOBOLEV_KEYWORD}
     _correlations_to_use = copy.deepcopy(_default_corr_to_use)
     _roots_to_use = {'cp': 0}
     _properties_module = 'lbh15.properties.lead_properties'
 
-    def __init__(self, p=P_ATM, **kwargs):
+    def __init__(self, p=atm, **kwargs):
         self._guess = LEAD_MELTING_TEMPERATURE*1.7
         super().__init__(p=p, **kwargs)
 
     def _set_constants(self):
         """
         Sets the class constants
         """
```

### Comparing `lbh15-1.1.1/lbh15/properties/bismuth_properties.py` & `lbh15-1.2.0/lbh15/properties/lbe_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-"""Module with the definition of thermophysical property objects for bismuth"""
+"""Module with the definition of thermophysical property objects
+for lead-bismuth eutectic"""
+import numpy as np
+from scipy.constants import atm
 from .interface import PropertyInterface, range_warning
-from .._constants import BISMUTH_MELTING_TEMPERATURE as T_m0
-from .._constants import BISMUTH_BOILING_TEMPERATURE as T_b0
-from .._constants import SOBOLEV_KEYWORD, P_ATM
+from .._commons import LBE_MELTING_TEMPERATURE as T_m0
+from .._commons import LBE_BOILING_TEMPERATURE as T_b0
+from .._commons import SOBOLEV_KEYWORD
 
 
 class p_s(PropertyInterface):
     """
-    Liquid bismuth saturation vapour pressure
+    Liquid lead-bismuth eutectic saturation vapour pressure
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute saturation vapour pressure
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -26,16 +29,15 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         saturation vapour pressure in [Pa] : float
         """
-        import numpy as np
-        return 2.67e10 * np.exp(-22858/T)
+        return 1.22e10 * np.exp(-22552/T)
 
     def initialization_helper(self, property_value):
         """
         Returns a temperature guess according to the value
         of the saturation vapour pressure
 
         Parameters
@@ -89,24 +91,24 @@
         return "saturation vapour pressure"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class sigma(PropertyInterface):
     """
-    Liquid bismuth surface tension
+    Liquid lead-bismuth eutectic surface tension
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute surface tension
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -117,22 +119,22 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         surface tension in [N/m] : float
         """
-        return (420.8 - 0.081*T)*1e-3
+        return (448.5 - 0.0799*T)*1e-3
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
-        return SOBOLEV_KEYWORD
+        return "plevachuk2008"
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, 1400.0]
@@ -152,24 +154,24 @@
         return "surface tension"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class rho(PropertyInterface):
     """
-    Liquid bismuth density
+    Liquid lead-bismuth eutectic density
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute density
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -180,26 +182,19 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         density in [kg/m^3] : float
         """
-        rho_0 = 10725 - 1.22*T
+        rho_0 = 11065 - 1.293*T
         u_s_val = u_s().correlation(T, p)
         cp_val = cp().correlation(T, p)
         alpha_val = alpha().correlation(T, p)
-        return rho_0 + ((u_s_val**-2 + T*alpha_val**2/cp_val) * (p - P_ATM))
-
-    @property
-    def correlation_name(self):
-        """
-        str : name of the correlation
-        """
-        return "imbeni1998"
+        return rho_0 + ((u_s_val**-2 + T*alpha_val**2/cp_val) * (p - atm))
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, T_b0]
@@ -219,24 +214,24 @@
         return "density"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class alpha(PropertyInterface):
     """
-    Liquid bismuth thermal expansion coefficient
+    Liquid lead-bismuth eutectic thermal expansion coefficient
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute thermal expansion coefficient
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -247,15 +242,15 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         thermal expansion coefficient in [1/K] : float
         """
-        return 1/(8791 - T)
+        return 1/(8558 - T)
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, T_b0]
@@ -275,24 +270,24 @@
         return "thermal expansion coefficient"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class u_s(PropertyInterface):
     """
-    Liquid bismuth sound velocity
+    Liquid lead-bismuth eutectic sound velocity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute sound velocity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -303,29 +298,29 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         sound velocity in [m/s] : float
         """
-        return 1616 + 0.187*T - 2.2e-4*T**2
+        return 1855 - 0.212*T
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
         return SOBOLEV_KEYWORD
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [T_m0, 1800.0]
+        return [400.0, 1100.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[m/s]"
@@ -338,24 +333,24 @@
         return "sound velocity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return "Sound velocity in liquid bismuth"
+        return "Sound velocity in liquid lbe"
 
 
 class beta_s(PropertyInterface):
     """
-    Liquid bismuth isentropic compressibility
+    Liquid lead-bismuth eutectic isentropic compressibility
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute isentropic compressibility
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -375,15 +370,15 @@
         return 1/(rho_obj.correlation(T, p) * u_s_obj.correlation(T, p)**2)
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [T_m0, 1800.0]
+        return [400.0, 1100.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[1/Pa]"
@@ -396,24 +391,24 @@
         return "isentropic compressibility"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class cp(PropertyInterface):
     """
-    Liquid bismuth specific heat capacity
+    Liquid lead-bismuth eutectic specific heat capacity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute specific heat capacity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -424,37 +419,38 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         specific heat capacity in [J/(kg*K)] : float
         """
-        return 118.2 + 5.934e-3*T + 7.183e6*T**-2
+        return (164.8 - 3.94e-2*T + 1.25e-5*T**2
+                - 4.56e5*T**-2)
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
-        return "imbeni1998"
+        return SOBOLEV_KEYWORD
 
     @property
     def is_injective(self):
         """
         bool : True if correlation is injective,
         False otherwise
         """
         return False
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [T_m0, T_b0]
+        return [400.0, T_b0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[J/(kg*K)]"
@@ -467,24 +463,24 @@
         return "specific heat capacity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class h(PropertyInterface):
     """
-    Liquid bismuth specific enthalpy
+    Liquid lead-bismuth eutectic specific enthalpy
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute specific enthalpy
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -495,31 +491,32 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         specific enthalpy in [J/kg] : float
         """
-        return (118.2*(T - T_m0)
-                + 2.967e-3*(T**2 - T_m0**2)
-                - 7.183e6*(T**-1 - T_m0**-1))
+        return (164.8*(T - T_m0)
+                - 1.97e-2*(T**2 - T_m0**2)
+                + 4.167e-6*(T**3 - T_m0**3)
+                + 4.56e5*(T**-1 - T_m0**-1))
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
         return SOBOLEV_KEYWORD
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [T_m0, T_b0]
+        return [400.0, T_b0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[J/kg]"
@@ -532,26 +529,26 @@
         return "specific enthalpy"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return (f"Liquid bismuth {self.long_name} "
+        return (f"Liquid lbe {self.long_name} "
                 "(as difference with respect to "
                 "the melting point enthalpy)")
 
 
 class mu(PropertyInterface):
     """
-    Liquid bismuth dynamic viscosity
+    Liquid lead-bismuth eutectic dynamic viscosity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute dynamic viscosity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -562,23 +559,15 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         dynamic viscosity in [Pa*s] : float
         """
-        import numpy as np
-        return 4.456e-4*np.exp(780/T)
-
-    @property
-    def correlation_name(self):
-        """
-        str : name of the correlation
-        """
-        return "lucas1984b"
+        return 4.94e-4*np.exp(754.1/T)
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, 1300.0]
@@ -598,24 +587,24 @@
         return "dynamic viscosity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class r(PropertyInterface):
     """
-    Liquid bismuth electrical resistivity
+    Liquid lead-bismuth eutectic electrical resistivity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute electrical resistivity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -626,22 +615,22 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         electrical resistivity in [Ohm*m] : float
         """
-        return (98.96 + 0.0554*T)*1e-8
+        return (90.9 + 0.048*T)*1e-8
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [545.0, 1423.0]
+        return [400.0, 1100.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[Ohm*m]"
@@ -654,24 +643,24 @@
         return "electrical resistivity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
 
 
 class k(PropertyInterface):
     """
-    Liquid bismuth thermal conductivity
+    Liquid lead-bismuth eutectic thermal conductivity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute thermal conductivity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -682,29 +671,29 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         thermal conductivity in [W/(m*K)] : float
         """
-        return 7.34 + 9.5e-3*T
+        return 3.284 + 1.617e-2*T - 2.305e-6*T**2
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
-        return "touloukian1970b"
+        return SOBOLEV_KEYWORD
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [T_m0, 1000.0]
+        return [T_m0, 1200.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[W/(m*K)]"
@@ -717,8 +706,8 @@
         return "thermal conductivity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid bismuth {self.long_name}"
+        return f"Liquid lbe {self.long_name}"
```

### Comparing `lbh15-1.1.1/lbh15/properties/interface.py` & `lbh15-1.2.0/lbh15/properties/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Module with the definition of thermophysical property object base class,
 i.e., PropertyInterface. Definition of decorator
 for validity range check as well."""
 import warnings
 from abc import ABC, abstractmethod
-from .._constants import P_ATM
+from numpy import nan
+from scipy.optimize import minimize_scalar
+from scipy.constants import atm
 
 
 def range_warning(function):
     """
     Decorator used to check validity range
     of correlation
     """
@@ -51,15 +53,14 @@
         - :attr:`~.PropertyInterface.correlation_name` override this member \
           to set a correlation name different from default one
         - :attr:`~.PropertyInterface.is_injective` override this member \
           if the function is not injective, othwerise it will \
           be considered injective
     """
     def __init__(self):
-        from numpy import nan
         self.__min = -nan
         self.__max = nan
         self.__T_at_min = -nan
         self.__T_at_max = nan
 
     def compute_bounds(self):
         """
@@ -68,15 +69,14 @@
         the validity range, together with the corresponding temperature.
         If this method is not invoked their default value is
         -nan and nan respectively.
         Values are computed using :func:`scipy.optimize.minimize_scalar`
         with "Bounded" solver (for more details please refer to scipy
         documentation)
         """
-        from scipy.optimize import minimize_scalar
         min_vals = minimize_scalar(self.correlation,
                                    bounds=self.range,
                                    method="Bounded")
         self.__min = min_vals.fun
         self.__T_at_min = min_vals.x
         if self.__T_at_min - self.range[0] < 5e-4:
             self.__T_at_min = self.range[0]
@@ -107,25 +107,25 @@
 
         Returns
         -------
         None
         """
         return None
 
-    def info(self, T, p=P_ATM, print_info=True, n_tab=0):
+    def info(self, T, p=atm, print_info=True, n_tab=0):
         """
         Method used to print information about the property
         and the correlation used to compute its value.
 
         Parameters
         ----------
         T : float
             Temperature in [K]
         p : float, optional
-            Pressure in [Pa], by default P_ATM, i.e., 101325.0 Pa
+            Pressure in [Pa], by default atm, i.e., 101325.0 Pa
         print_info : bool, optional
             True to print to console, False for getting the
             string, by default True
         n_tab : int, optional
             Number of tabs used to format the information, by default 0
 
         Returns
@@ -161,15 +161,15 @@
             print(all_info)
         else:
             rvalue = all_info
         return rvalue
 
     @abstractmethod
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Function that implements the property correlation
 
         Parameters
         ----------
         T : float
             Temperature in [K]
```

### Comparing `lbh15-1.1.1/lbh15/properties/lbe_properties.py` & `lbh15-1.2.0/lbh15/properties/bismuth_properties.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""Module with the definition of thermophysical property objects
-for lead-bismuth eutectic"""
+"""Module with the definition of thermophysical property objects for bismuth"""
+import numpy as np
+from scipy.constants import atm
 from .interface import PropertyInterface, range_warning
-from .._constants import LBE_MELTING_TEMPERATURE as T_m0
-from .._constants import LBE_BOILING_TEMPERATURE as T_b0
-from .._constants import SOBOLEV_KEYWORD, P_ATM
+from .._commons import BISMUTH_MELTING_TEMPERATURE as T_m0
+from .._commons import BISMUTH_BOILING_TEMPERATURE as T_b0
+from .._commons import SOBOLEV_KEYWORD
 
 
 class p_s(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic saturation vapour pressure
+    Liquid bismuth saturation vapour pressure
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute saturation vapour pressure
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -27,16 +28,15 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         saturation vapour pressure in [Pa] : float
         """
-        import numpy as np
-        return 1.22e10 * np.exp(-22552/T)
+        return 2.67e10 * np.exp(-22858/T)
 
     def initialization_helper(self, property_value):
         """
         Returns a temperature guess according to the value
         of the saturation vapour pressure
 
         Parameters
@@ -90,24 +90,24 @@
         return "saturation vapour pressure"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class sigma(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic surface tension
+    Liquid bismuth surface tension
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute surface tension
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -118,22 +118,22 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         surface tension in [N/m] : float
         """
-        return (448.5 - 0.0799*T)*1e-3
+        return (420.8 - 0.081*T)*1e-3
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
-        return "plevachuk2008"
+        return SOBOLEV_KEYWORD
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, 1400.0]
@@ -153,24 +153,24 @@
         return "surface tension"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class rho(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic density
+    Liquid bismuth density
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute density
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -181,19 +181,26 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         density in [kg/m^3] : float
         """
-        rho_0 = 11065 - 1.293*T
+        rho_0 = 10725 - 1.22*T
         u_s_val = u_s().correlation(T, p)
         cp_val = cp().correlation(T, p)
         alpha_val = alpha().correlation(T, p)
-        return rho_0 + ((u_s_val**-2 + T*alpha_val**2/cp_val) * (p - P_ATM))
+        return rho_0 + ((u_s_val**-2 + T*alpha_val**2/cp_val) * (p - atm))
+
+    @property
+    def correlation_name(self):
+        """
+        str : name of the correlation
+        """
+        return "imbeni1998"
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, T_b0]
@@ -213,24 +220,24 @@
         return "density"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class alpha(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic thermal expansion coefficient
+    Liquid bismuth thermal expansion coefficient
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute thermal expansion coefficient
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -241,15 +248,15 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         thermal expansion coefficient in [1/K] : float
         """
-        return 1/(8558 - T)
+        return 1/(8791 - T)
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, T_b0]
@@ -269,24 +276,24 @@
         return "thermal expansion coefficient"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class u_s(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic sound velocity
+    Liquid bismuth sound velocity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute sound velocity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -297,29 +304,29 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         sound velocity in [m/s] : float
         """
-        return 1855 - 0.212*T
+        return 1616 + 0.187*T - 2.2e-4*T**2
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
         return SOBOLEV_KEYWORD
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [400.0, 1100.0]
+        return [T_m0, 1800.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[m/s]"
@@ -332,24 +339,24 @@
         return "sound velocity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return "Sound velocity in liquid lbe"
+        return "Sound velocity in liquid bismuth"
 
 
 class beta_s(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic isentropic compressibility
+    Liquid bismuth isentropic compressibility
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute isentropic compressibility
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -369,15 +376,15 @@
         return 1/(rho_obj.correlation(T, p) * u_s_obj.correlation(T, p)**2)
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [400.0, 1100.0]
+        return [T_m0, 1800.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[1/Pa]"
@@ -390,24 +397,24 @@
         return "isentropic compressibility"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class cp(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic specific heat capacity
+    Liquid bismuth specific heat capacity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute specific heat capacity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -418,38 +425,37 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         specific heat capacity in [J/(kg*K)] : float
         """
-        return (164.8 - 3.94e-2*T + 1.25e-5*T**2
-                - 4.56e5*T**-2)
+        return 118.2 + 5.934e-3*T + 7.183e6*T**-2
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
-        return SOBOLEV_KEYWORD
+        return "imbeni1998"
 
     @property
     def is_injective(self):
         """
         bool : True if correlation is injective,
         False otherwise
         """
         return False
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [400.0, T_b0]
+        return [T_m0, T_b0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[J/(kg*K)]"
@@ -462,24 +468,24 @@
         return "specific heat capacity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class h(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic specific enthalpy
+    Liquid bismuth specific enthalpy
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute specific enthalpy
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -490,32 +496,31 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         specific enthalpy in [J/kg] : float
         """
-        return (164.8*(T - T_m0)
-                - 1.97e-2*(T**2 - T_m0**2)
-                + 4.167e-6*(T**3 - T_m0**3)
-                + 4.56e5*(T**-1 - T_m0**-1))
+        return (118.2*(T - T_m0)
+                + 2.967e-3*(T**2 - T_m0**2)
+                - 7.183e6*(T**-1 - T_m0**-1))
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
         return SOBOLEV_KEYWORD
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [400.0, T_b0]
+        return [T_m0, T_b0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[J/kg]"
@@ -528,26 +533,26 @@
         return "specific enthalpy"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return (f"Liquid lbe {self.long_name} "
+        return (f"Liquid bismuth {self.long_name} "
                 "(as difference with respect to "
                 "the melting point enthalpy)")
 
 
 class mu(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic dynamic viscosity
+    Liquid bismuth dynamic viscosity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute dynamic viscosity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -558,16 +563,22 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         dynamic viscosity in [Pa*s] : float
         """
-        import numpy as np
-        return 4.94e-4*np.exp(754.1/T)
+        return 4.456e-4*np.exp(780/T)
+
+    @property
+    def correlation_name(self):
+        """
+        str : name of the correlation
+        """
+        return "lucas1984b"
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
         return [T_m0, 1300.0]
@@ -587,24 +598,24 @@
         return "dynamic viscosity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class r(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic electrical resistivity
+    Liquid bismuth electrical resistivity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute electrical resistivity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -615,22 +626,22 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         electrical resistivity in [Ohm*m] : float
         """
-        return (90.9 + 0.048*T)*1e-8
+        return (98.96 + 0.0554*T)*1e-8
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [400.0, 1100.0]
+        return [545.0, 1423.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[Ohm*m]"
@@ -643,24 +654,24 @@
         return "electrical resistivity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
 
 
 class k(PropertyInterface):
     """
-    Liquid lead-bismuth eutectic thermal conductivity
+    Liquid bismuth thermal conductivity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute thermal conductivity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -671,29 +682,29 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         thermal conductivity in [W/(m*K)] : float
         """
-        return 3.284 + 1.617e-2*T - 2.305e-6*T**2
+        return 7.34 + 9.5e-3*T
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
-        return SOBOLEV_KEYWORD
+        return "touloukian1970b"
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
-        return [T_m0, 1200.0]
+        return [T_m0, 1000.0]
 
     @property
     def units(self):
         """
         str : property units
         """
         return "[W/(m*K)]"
@@ -706,8 +717,8 @@
         return "thermal conductivity"
 
     @property
     def description(self):
         """
         str : property description
         """
-        return f"Liquid lbe {self.long_name}"
+        return f"Liquid bismuth {self.long_name}"
```

### Comparing `lbh15-1.1.1/lbh15/properties/lead_properties.py` & `lbh15-1.2.0/lbh15/properties/lead_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Module with the definition of thermophysical property objects for lead"""
+import numpy as np
+from scipy.constants import atm
 from .interface import PropertyInterface, range_warning
-from .._constants import LEAD_MELTING_TEMPERATURE as T_m0
-from .._constants import LEAD_BOILING_TEMPERATURE as T_b0
-from .._constants import SOBOLEV_KEYWORD, GURVICH_KEYWORD, P_ATM
+from .._commons import LEAD_MELTING_TEMPERATURE as T_m0
+from .._commons import LEAD_BOILING_TEMPERATURE as T_b0
+from .._commons import SOBOLEV_KEYWORD, GURVICH_KEYWORD
 
 
 class p_s(PropertyInterface):
     """
     Liquid lead saturation vapour pressure
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute saturation vapour pressure
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -26,15 +28,14 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         saturation vapour pressure in [Pa] : float
         """
-        import numpy as np
         return 5.76e9 * np.exp(-22131/T)
 
     def initialization_helper(self, property_value):
         """
         Returns a temperature guess according to the value
         of the saturation vapour pressure
 
@@ -98,15 +99,15 @@
 
 class sigma(PropertyInterface):
     """
     Liquid lead surface tension
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute surface tension
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -161,15 +162,15 @@
 
 class rho(PropertyInterface):
     """
     Liquid lead density
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute density. sobolev2011 correlation
         is used as specific heat capacity in pressure dependent
         term of the correlation.
 
         Parameters
         ----------
@@ -186,15 +187,15 @@
         -------
         density in [kg/m^3] : float
         """
         rho_0 = 11441 - 1.2795*T
         u_s_val = u_s().correlation(T, p)
         cp_val = cp_sobolev2011().correlation(T, p)
         alpha_val = alpha().correlation(T, p)
-        return rho_0 + ((u_s_val**-2 + T*alpha_val**2/cp_val) * (p - P_ATM))
+        return rho_0 + ((u_s_val**-2 + T*alpha_val**2/cp_val) * (p - atm))
 
     @property
     def correlation_name(self):
         """
         str : name of the correlation
         """
         return "sobolev2008a"
@@ -230,15 +231,15 @@
 
 class alpha(PropertyInterface):
     """
     Liquid lead thermal expansion coefficient
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute thermal expansion coefficient
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -286,15 +287,15 @@
 
 class u_s(PropertyInterface):
     """
     Liquid lead sound velocity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute sound velocity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -349,15 +350,15 @@
 
 class beta_s(PropertyInterface):
     """
     Liquid lead isentropic compressibility
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute isentropic compressibility
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -407,15 +408,15 @@
 
 class cp_sobolev2011(PropertyInterface):
     """
     Liquid lead specific heat capacity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute specific heat capacity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -486,15 +487,15 @@
 
 class cp_gurvich1991(PropertyInterface):
     """
     Liquid lead specific heat capacity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute specific heat capacity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -565,15 +566,15 @@
 
 class h(PropertyInterface):
     """
     Liquid lead specific enthalpy
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute specific enthalpy
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -633,15 +634,15 @@
 
 class mu(PropertyInterface):
     """
     Liquid lead dynamic viscosity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute dynamic viscosity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -652,15 +653,14 @@
             True to tell decorator to print warning about
             range check failing, False otherwise. By default False
 
         Returns
         -------
         dynamic viscosity in [Pa*s] : float
         """
-        import numpy as np
         return 4.55e-4 * np.exp(1069/T)
 
     @property
     def range(self):
         """
         list : temperature validity range for property correlation
         """
@@ -690,15 +690,15 @@
 
 class r(PropertyInterface):
     """
     Liquid lead electrical resistivity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute electrical resistivity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
@@ -746,15 +746,15 @@
 
 class k(PropertyInterface):
     """
     Liquid lead thermal conductivity
     property class
     """
     @range_warning
-    def correlation(self, T, p=P_ATM, verbose=False):
+    def correlation(self, T, p=atm, verbose=False):
         """
         Correlation used to compute thermal conductivity
 
         Parameters
         ----------
         T : float
             Temperature in [K]
```

### Comparing `lbh15-1.1.1/setup.py` & `lbh15-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,97 @@
 #!/usr/bin/python3
 
 from setuptools import setup
 from setuptools import find_packages
-from lbh15 import __version__
-from lbh15 import __author__
+import codecs
+import os.path
 
-setup(
-    name='lbh15',
-    version=__version__,
-    packages=find_packages(),
-    include_package_data=True,
-    author=__author__,
-    author_email='daniele.panico@newcleo.com, daniele.tomatis@newcleo.com',
-    description='Python implementation of liquid metal properties from '
-                'Handbook on Lead-bismuth Eutectic Alloy and Lead Properties, '
-                'Materials Compatibility, Thermal-hydraulics and Technologies',
-    long_description_content_type='text/x-rst',
-    long_description=open('README.rst', 'r').read(),
-    license='lgpl v3',
-    python_requires='>=3.8.10',
-    install_requires=['scipy>=1.8.1', 'numpy>=1.22.3'],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Education",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Physics",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-)
+
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+
+def get_info(rel_path, info):
+    for line in read(rel_path).splitlines():
+        if line.startswith(f'__{info}__'):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    else:
+        raise RuntimeError(f"Unable to find {info} string.")
+
+
+if __name__ == '__main__':
+
+    setup(
+        name='lbh15',
+        version=get_info('lbh15/__init__.py', 'version'),
+        packages=find_packages(),
+        include_package_data=True,
+        author=get_info('lbh15/__init__.py', 'author'),
+        author_email='daniele.panico@newcleo.com, daniele.tomatis@newcleo.com',
+        description='Python implementation of liquid metal properties from '
+                    'Handbook on Lead-bismuth Eutectic Alloy and '
+                    'Lead Properties, Materials Compatibility, '
+                    'Thermal-hydraulics and Technologies',
+        long_description_content_type='text/x-rst',
+        long_description=open('README.rst', 'r').read(),
+        license='lgpl v3',
+        python_requires='>=3.8.10',
+        install_requires=['scipy>=1.8.1', 'numpy>=1.22.3'],
+        classifiers=[
+            "Development Status :: 5 - Production/Stable",
+            "Intended Audience :: Education",
+            "Intended Audience :: Science/Research",
+            "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+            "Natural Language :: English",
+            "Operating System :: OS Independent",
+            "Programming Language :: Python",
+            "Topic :: Scientific/Engineering",
+            "Topic :: Scientific/Engineering :: Physics",
+            "Topic :: Software Development :: Libraries :: Python Modules",
+        ],
+    )
 
 """
 Developers memo for release:
     1. Update package information (on master):
         - Change version in lbh15/__init__.py
         - Change date in lbh15/__init__.py
         - Change date in README.rst
 
     2. Test the package build and install on test-pypi:
-        a. Change the name of the package in setup.py in 'lbh15-test'
+        a. Change the name of the package in setup.py and pyproject.toml in 'lbh15-test'
         b. python3 setup.py sdist                     # in project directory
         c. twine check dist/*                         # check that package is ok
         d. twine upload --repository testpypi dist/*  # verify upload is successful on test-PyPI
         e. crete a python3 virtual enviroment and verify the correct package installation form test-pypi:
             python3 -m venv venv_install
             source venv_install/bn/activate
             pip3 install wheel
             pip3 install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple lbh15-test
             cd tests/
             <execute tests>
         f. If every thing is ok change back the package name in 'lbh15'
-        
+
     3. Create tag (on master):
-        a. git tag v<version>
-        b. git push <origin_name> <tag_name>
-        c. git diff --stat=200 <previous_tag> <tag_name> > log.diff.<tag_name>
-        d. You should see the tag on github page as well. Then on github do:
+        a. commit previous release info modifications
+        b. git tag v<version>
+        c. git push <origin_name> <tag_name>
+        d. git diff --stat=200 <previous_tag> <tag_name> > log.diff.<tag_name>
+        e. You should see the tag on github page as well. Then on github do:
             - https://github.com/newcleo-dev-team/lbh15/releases
             - Click on "Draft a new release"
             - Choose the tag
             - Insert the title name as "Release v<version>"
             - In the description write:
                 Changelog between v<previous varsion> and v<version>
 
                 ```
                 < content of  log.diff.<tag_name> >
                 ```
 
     4. Upload the package on PyPI:
         a. repeat step 2.b and 2.c
-        b. twine upload dist/*             
-"""
+        b. twine upload dist/*
+"""
```

