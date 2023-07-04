# Comparing `tmp/PH-Baseliner-1.1.3.tar.gz` & `tmp/PH-Baseliner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-Baseliner-1.1.3.tar", last modified: Sun May 28 15:41:44 2023, max compression
+gzip compressed data, was "dist/PH-Baseliner-1.2.0.tar", last modified: Tue Jul  4 19:15:10 2023, max compression
```

## Comparing `PH-Baseliner-1.1.3.tar` & `PH-Baseliner-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35149 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      616 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PH_Baseliner.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1589 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/README.md
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/ph_baseliner/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/
--rw-r--r--   0 runner     (501) staff       (20)    13031 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/ECCCNYS_2020.json
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2071 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/lighting_space_types.py
--rw-r--r--   0 runner     (501) staff       (20)    17467 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/model.py
--rw-r--r--   0 runner     (501) staff       (20)     1406 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/codes/options.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4647 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     1776 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/components.py
--rw-r--r--   0 runner     (501) staff       (20)     1664 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     5549 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/u_values.py
--rw-r--r--   0 runner     (501) staff       (20)     4952 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/ph_baseliner/phpp/windows.py
--rw-r--r--   0 runner     (501) staff       (20)       19 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      839 2023-05-28 15:41:44.000000 PH-Baseliner-1.1.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-05-28 15:39:46.000000 PH-Baseliner-1.1.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      762 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PH_Baseliner.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/
+-rw-r--r--   0 runner     (501) staff       (20)    13031 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/ECCCNYS_2020.json
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2071 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/lighting_space_types.py
+-rw-r--r--   0 runner     (501) staff       (20)    17467 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     1406 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/codes/options.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4685 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     1484 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/components.py
+-rw-r--r--   0 runner     (501) staff       (20)     1725 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     3285 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/u_values.py
+-rw-r--r--   0 runner     (501) staff       (20)     5410 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phpp/windows.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2526 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     2583 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/constructions.py
+-rw-r--r--   0 runner     (501) staff       (20)      488 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     6056 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/ph_baseliner/phx/windows.py
+-rw-r--r--   0 runner     (501) staff       (20)       87 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      839 2023-07-04 19:15:10.000000 PH-Baseliner-1.2.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-04 19:13:13.000000 PH-Baseliner-1.2.0/setup.py
```

### Comparing `PH-Baseliner-1.1.3/.github/workflows/ci.yaml` & `PH-Baseliner-1.2.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.1.3/LICENSE` & `PH-Baseliner-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.1.3/PH_Baseliner.egg-info/PKG-INFO` & `PH-Baseliner-1.2.0/PH_Baseliner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.1.3
+Version: 1.2.0
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
```

### Comparing `PH-Baseliner-1.1.3/PKG-INFO` & `PH-Baseliner-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.1.3
+Version: 1.2.0
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
```

### Comparing `PH-Baseliner-1.1.3/README.md` & `PH-Baseliner-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/codes/ECCCNYS_2020.json` & `PH-Baseliner-1.2.0/ph_baseliner/codes/ECCCNYS_2020.json`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/codes/lighting_space_types.py` & `PH-Baseliner-1.2.0/ph_baseliner/codes/lighting_space_types.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/codes/model.py` & `PH-Baseliner-1.2.0/ph_baseliner/codes/model.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/codes/options.py` & `PH-Baseliner-1.2.0/ph_baseliner/codes/options.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/phpp/areas.py` & `PH-Baseliner-1.2.0/ph_baseliner/phpp/areas.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from PHX.PHPP import phpp_app
 from PHX.PHPP.phpp_model.areas_surface import ExistingSurfaceRow
 from PHX.model.enums.building import ComponentFaceType, ComponentExposureExterior
 
 from ph_baseliner.codes.model import BaselineCode
 from ph_baseliner.codes.options import ClimateZones, Use_Groups
 from ph_baseliner.phpp.u_values import (
-    create_baseline_constructions,
     add_baseline_constructions_to_phpp,
     BaselineConstructionPHPPids,
 )
+from ph_baseliner.phx.constructions import create_baseline_constructions
 
 
 def set_baseline_envelope_constructions(
     phpp_conn: phpp_app.PHPPConnection,
     baseline_code: BaselineCode,
     climate_zone: ClimateZones,
     use_group: Use_Groups,
```

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/phpp/components.py` & `PH-Baseliner-1.2.0/ph_baseliner/phpp/components.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 """Functions to create and add new baseline PHPP components."""
 
 from PHX.PHPP import phpp_app
 from PHX.model.constructions import PhxConstructionWindow
 from PHX.PHPP.phpp_model.component_glazing import GlazingRow
 from PHX.PHPP.phpp_model.component_frame import FrameRow
 
-def create_new_baseline_window_glazing(u_value: float, shgc: float) -> PhxConstructionWindow:
-    """Create a new baseline PHX window construction."""
-    return PhxConstructionWindow.from_total_u_value(u_value, shgc, "BASELINE: WINDOW")
 
-def add_new_baseline_window_glazing(phpp_conn: phpp_app.PHPPConnection, 
-                                    baseline_phx_window: PhxConstructionWindow
+def add_new_baseline_window_glazing(
+    phpp_conn: phpp_app.PHPPConnection, baseline_phx_window: PhxConstructionWindow
 ) -> str:
     """Add a new baseline PhxConstructionWindow Glazing to the PHPP Components Worksheet.
-    
+
     Returns:
     --------
         str: The PHPP Glazing ID (ie: "01ud-MyGlass", etc..)
     """
     phpp_glazing_row = GlazingRow(phpp_conn.shape.COMPONENTS, baseline_phx_window)
     row_num = phpp_conn.components.first_empty_glazing_row_num
-    phpp_glazing_id = phpp_conn.components.write_single_glazing(row_num, phpp_glazing_row)
+    phpp_glazing_id = phpp_conn.components.write_single_glazing(
+        row_num, phpp_glazing_row
+    )
     return phpp_glazing_id
 
-def add_new_baseline_window_frame(phpp_conn: phpp_app.PHPPConnection, 
-                                  baseline_phx_window: PhxConstructionWindow
+
+def add_new_baseline_window_frame(
+    phpp_conn: phpp_app.PHPPConnection, baseline_phx_window: PhxConstructionWindow
 ) -> str:
     """Add a new baseline PhxConstructionWindow Frame to the PHPP Components Worksheet.
-    
+
     Returns:
     --------
         str: The PHPP Frame ID (ie: "01ud-MyFrame", etc..)
     """
     phpp_frame_row = FrameRow(phpp_conn.shape.COMPONENTS, baseline_phx_window)
     row_num = phpp_conn.components.first_empty_frame_row_num
     phpp_frame_id = phpp_conn.components.write_single_frame(row_num, phpp_frame_row)
-    return phpp_frame_id
+    return phpp_frame_id
```

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/phpp/lighting.py` & `PH-Baseliner-1.2.0/ph_baseliner/phpp/lighting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 # -*- coding: utf-8 -*-
 # -*- Python Version: 3.7 -*-
 
-"""Functions to set baseline PHPP windows."""
+"""Functions to set baseline PHPP lighting."""
 
 from PHX.PHPP.phpp_app import PHPPConnection
 
 from ph_baseliner.codes.model import BaselineCode
 from ph_baseliner.codes.lighting_space_types import space_type_map
 
-def find_lighting_installed_power(_baseline_code: BaselineCode, _program_name: str) -> float:
+
+def find_lighting_installed_power(
+    _baseline_code: BaselineCode, _program_name: str
+) -> float:
     """Find the baseline lighting installed power density for a given PHPP space."""
 
     # -- First, find the building-code name for the PHPP space type
     code_name = space_type_map.get(_program_name, None)
 
     if not code_name:
-        msg = f"Error: The PHPP Space-Type name {_program_name} does not have a "\
-                "corresponding building-code name?"
+        msg = (
+            f"Error: The PHPP Space-Type name {_program_name} does not have a "
+            "corresponding building-code name?"
+        )
         raise Exception(msg)
 
     # -- Then, find the lighting installed power density for that building-code name
     return _baseline_code.tables.lighting_area_method.LPD[code_name]
 
-def set_baseline_lighting_installed_power_density(_phpp_conn: PHPPConnection, _baseline_code: BaselineCode):
+
+def set_baseline_lighting_installed_power_density(
+    _phpp_conn: PHPPConnection, _baseline_code: BaselineCode
+) -> None:
     """Set the PHPP 'Electricity non-res' worksheet baseline lighting installed power density.
 
     Arguments:
     ----------
         _phpp_conn: phpp_app.PHPPConnection
             The PHPPConnection object
         _baseline_code: BaselineCode
             The BaselineCode object
     """
-    
+
     for row_num in _phpp_conn.elec_non_res.lighting.used_lighting_row_numbers:
         row_data = _phpp_conn.elec_non_res.lighting.get_lighting_row_data(row_num)
-        code_LPD = find_lighting_installed_power(_baseline_code, row_data.utilization_profile_name)
-        _phpp_conn.elec_non_res.lighting.set_lighting_power_density(row_num, code_LPD)
+        code_LPD = find_lighting_installed_power(
+            _baseline_code, row_data.utilization_profile_name
+        )
+        _phpp_conn.elec_non_res.lighting.set_lighting_power_density(row_num, code_LPD)
```

### Comparing `PH-Baseliner-1.1.3/ph_baseliner/phpp/windows.py` & `PH-Baseliner-1.2.0/ph_baseliner/phpp/windows.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # -*- Python Version: 3.7 -*-
 
 """Functions to set baseline PHPP windows."""
 
 from PHX.PHPP import phpp_app
+from PHX.model.constructions import PhxConstructionWindow
 
 from ph_baseliner.codes.model import BaselineCode
 from ph_baseliner.codes.options import ClimateZones, PF_Groups, Use_Groups
 from ph_baseliner.phpp.components import (
     add_new_baseline_window_glazing,
     add_new_baseline_window_frame,
-    create_new_baseline_window_glazing,
 )
 
 
-def get_baseline_u_value(
+def get_baseline_window_u_value(
     _baseline_code: BaselineCode, _climate_zone: ClimateZones, _use_group: Use_Groups
 ) -> float:
     """Get the baseline U-Value for the specified climate zone."""
     all_u_values = _baseline_code.get_window_u_values()
     cz_uvalues = all_u_values.get_u_value_for_climate(_climate_zone)
     u_value = cz_uvalues.get_u_values_for_use_group(_use_group)
     return u_value
 
 
-def get_baseline_SHGC(
+def get_baseline_window_SHGC(
     _baseline_code: BaselineCode, _climate_zone: ClimateZones, _pf_group: PF_Groups
 ) -> float:
     """Get the baseline SHGC for the specified climate zone and Projection Factor group."""
     all_shgcs = _baseline_code.get_window_shgcs()
     cz_shgcs = all_shgcs.get_shgcs_for_climate(_climate_zone)
     pf_shgc = cz_shgcs.get_shgc_for_pf(_pf_group)
     return pf_shgc
@@ -48,19 +48,21 @@
         phpp_conn: phpp_app.PHPPConnection
             The PHPPConnection object
         baseline_code: BaselineCode
             The BaselineCode object
     """
 
     # -- Get the baseline values for U-Value and SHGC
-    u_value = get_baseline_u_value(_baseline_code, _climate_zone, _use_group)
-    shgc = get_baseline_SHGC(_baseline_code, _climate_zone, _pf_group)
+    u_value = get_baseline_window_u_value(_baseline_code, _climate_zone, _use_group)
+    shgc = get_baseline_window_SHGC(_baseline_code, _climate_zone, _pf_group)
 
     # -- Create the new baseline window construction
-    baseline_phx_window = create_new_baseline_window_glazing(u_value, shgc)
+    baseline_phx_window = PhxConstructionWindow.from_total_u_value(
+        u_value, shgc, "BASELINE: WINDOW"
+    )
     phpp_glazing_id = add_new_baseline_window_glazing(_phpp_conn, baseline_phx_window)
     phpp_frame_id = add_new_baseline_window_frame(_phpp_conn, baseline_phx_window)
 
     # -- Set the window constructions in the Windows Worksheet
     for row_num in _phpp_conn.windows.used_window_row_numbers:
         _phpp_conn.windows.set_single_window_construction_ids(
             row_num, phpp_glazing_id, phpp_frame_id
@@ -75,18 +77,28 @@
     Arguments:
     ----------
         phpp_conn: phpp_app.PHPPConnection
             The PHPPConnection object
         baseline_code: BaselineCode
             The BaselineCode object
     """
+
+    # -- As per NYS Code, C402.4.1 Maximum Area:
+    #
+    # > "The vertical fenestration area, not including opaque doors and
+    # > opaque spandrel panels, shall be not greater than 30
+    # > percent of the GROSS above-grade wall area."
+    #
+    # -- So be sure to use the GROSS wall area, BEFORE the windows
+    # -- have been punched out of them.
+
     maximum_wwr = _baseline_code.get_baseline_max_wwr()
-    current_wall_area = _phpp_conn.areas.get_total_wall_area()
+    current_net_wall_area = _phpp_conn.areas.get_total_net_wall_area()
     current_window_area = _phpp_conn.windows.get_total_window_area()
-    current_wwr = current_window_area / (current_wall_area + current_window_area)
+    current_wwr = current_window_area / (current_net_wall_area + current_window_area)
 
     if current_wwr < maximum_wwr:
         print(f"Current WWR {current_wwr:.2%} is less than maximum {maximum_wwr:.0%}.")
         return None
 
     print(
         f"Current WWR {current_wwr:.2%} is greater than maximum {maximum_wwr:.0%}. Scaling windows."
@@ -112,15 +124,15 @@
     ----------
         phpp_conn: phpp_app.PHPPConnection
             The PHPPConnection object
         baseline_code: BaselineCode
             The BaselineCode object
     """
     maximum_srr = _baseline_code.get_baseline_max_srr()
-    current_roof_area = _phpp_conn.areas.get_total_roof_area()
+    current_roof_area = _phpp_conn.areas.get_total_net_roof_area()
     current_skylight_area = _phpp_conn.windows.get_total_skylight_area()
     current_srr = current_skylight_area / (current_roof_area + current_skylight_area)
 
     if current_srr < maximum_srr:
         print(f"Current SRR {current_srr:.2%} is less than maximum {maximum_srr:.0%}.")
         return None
```

### Comparing `PH-Baseliner-1.1.3/setup.cfg` & `PH-Baseliner-1.2.0/setup.cfg`

 * *Files identical despite different names*

