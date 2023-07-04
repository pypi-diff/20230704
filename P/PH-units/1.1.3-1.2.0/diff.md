# Comparing `tmp/PH-units-1.1.3.tar.gz` & `tmp/PH-units-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-units-1.1.3.tar", last modified: Wed Jun 14 23:40:00 2023, max compression
+gzip compressed data, was "dist/PH-units-1.2.0.tar", last modified: Tue Jul  4 16:03:45 2023, max compression
```

## Comparing `PH-units-1.1.3.tar` & `PH-units-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-06-14 23:38:11.000000 PH-units-1.1.3/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1781 2023-06-14 23:38:11.000000 PH-units-1.1.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35129 2023-06-14 23:38:11.000000 PH-units-1.1.3/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/PH_units.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-06-14 23:39:59.000000 PH-units-1.1.3/PH_units.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      638 2023-06-14 23:40:00.000000 PH-units-1.1.3/PH_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-14 23:39:59.000000 PH-units-1.1.3/PH_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-06-14 23:39:59.000000 PH-units-1.1.3/PH_units.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-06-14 23:40:00.000000 PH-units-1.1.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-06-14 23:38:11.000000 PH-units-1.1.3/README.md
--rw-r--r--   0 runner     (501) staff       (20)       50 2023-06-14 23:38:11.000000 PH-units-1.1.3/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/ph_units/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5159 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/converter.py
--rw-r--r--   0 runner     (501) staff       (20)     1908 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/parser.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-14 23:40:00.000000 PH-units-1.1.3/ph_units/unit_types/
--rw-r--r--   0 runner     (501) staff       (20)     2784 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      371 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/_base.py
--rw-r--r--   0 runner     (501) staff       (20)      442 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/area.py
--rw-r--r--   0 runner     (501) staff       (20)     4466 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/energy.py
--rw-r--r--   0 runner     (501) staff       (20)     2571 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/envelope.py
--rw-r--r--   0 runner     (501) staff       (20)     1459 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/length.py
--rw-r--r--   0 runner     (501) staff       (20)     2093 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/power.py
--rw-r--r--   0 runner     (501) staff       (20)     1176 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/speed.py
--rw-r--r--   0 runner     (501) staff       (20)      796 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/temperature.py
--rw-r--r--   0 runner     (501) staff       (20)      917 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/volume.py
--rw-r--r--   0 runner     (501) staff       (20)     1705 2023-06-14 23:38:11.000000 PH-units-1.1.3/ph_units/unit_types/volume_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-06-14 23:38:11.000000 PH-units-1.1.3/sandbox.py
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-06-14 23:40:00.000000 PH-units-1.1.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-06-14 23:38:11.000000 PH-units-1.1.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 16:03:45.000000 PH-units-1.2.0/
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-07-04 16:01:07.000000 PH-units-1.2.0/.gitattributes
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 16:03:44.000000 PH-units-1.2.0/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 16:03:45.000000 PH-units-1.2.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1781 2023-07-04 16:01:07.000000 PH-units-1.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35129 2023-07-04 16:01:07.000000 PH-units-1.2.0/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 16:03:45.000000 PH-units-1.2.0/PH_units.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-07-04 16:03:39.000000 PH-units-1.2.0/PH_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      759 2023-07-04 16:03:44.000000 PH-units-1.2.0/PH_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-04 16:03:39.000000 PH-units-1.2.0/PH_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-07-04 16:03:39.000000 PH-units-1.2.0/PH_units.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-07-04 16:03:45.000000 PH-units-1.2.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-07-04 16:01:07.000000 PH-units-1.2.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       50 2023-07-04 16:01:07.000000 PH-units-1.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 16:03:45.000000 PH-units-1.2.0/ph_units/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5224 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/converter.py
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/parser.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-04 16:03:45.000000 PH-units-1.2.0/ph_units/unit_types/
+-rw-r--r--   0 runner     (501) staff       (20)     2999 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      371 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/_base.py
+-rw-r--r--   0 runner     (501) staff       (20)      605 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/area.py
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/density.py
+-rw-r--r--   0 runner     (501) staff       (20)      763 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/emissions_factors.py
+-rw-r--r--   0 runner     (501) staff       (20)     6566 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/energy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2681 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/envelope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/length.py
+-rw-r--r--   0 runner     (501) staff       (20)      584 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/moisture_vapor_resistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     2249 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     1408 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/speed.py
+-rw-r--r--   0 runner     (501) staff       (20)     1030 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/temperature.py
+-rw-r--r--   0 runner     (501) staff       (20)     1188 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/volume.py
+-rw-r--r--   0 runner     (501) staff       (20)     2354 2023-07-04 16:01:07.000000 PH-units-1.2.0/ph_units/unit_types/volume_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2023-07-04 16:01:07.000000 PH-units-1.2.0/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)      832 2023-07-04 16:03:45.000000 PH-units-1.2.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-04 16:01:07.000000 PH-units-1.2.0/setup.py
```

### Comparing `PH-units-1.1.3/.github/workflows/ci.yaml` & `PH-units-1.2.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.3/LICENSE` & `PH-units-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.3/PH_units.egg-info/PKG-INFO` & `PH-units-1.2.0/PH_units.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.1.3
+Version: 1.2.0
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.1.3/PH_units.egg-info/SOURCES.txt` & `PH-units-1.2.0/PH_units.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 PH_units.egg-info/top_level.txt
 ph_units/__init__.py
 ph_units/converter.py
 ph_units/parser.py
 ph_units/unit_types/__init__.py
 ph_units/unit_types/_base.py
 ph_units/unit_types/area.py
+ph_units/unit_types/density.py
+ph_units/unit_types/emissions_factors.py
 ph_units/unit_types/energy.py
 ph_units/unit_types/envelope.py
 ph_units/unit_types/length.py
+ph_units/unit_types/moisture_vapor_resistance.py
 ph_units/unit_types/power.py
 ph_units/unit_types/speed.py
 ph_units/unit_types/temperature.py
 ph_units/unit_types/volume.py
 ph_units/unit_types/volume_flow.py
```

### Comparing `PH-units-1.1.3/PKG-INFO` & `PH-units-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.1.3
+Version: 1.2.0
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.1.3/README.md` & `PH-units-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.3/ph_units/converter.py` & `PH-units-1.2.0/ph_units/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     """
 
     _input_string = str(_input).upper()
     try:
         input_unit = _unit_type_alias_dict[_input_string]
     except KeyError:
         raise Exception(
-            "\n\tI do not know how to understand the input unit: '{}'?".format(
-                _input_string
+            "\n\tI do not know how to understand the input unit: '{}'?\nValid formats include: {}".format(
+                _input_string, sorted(_unit_type_alias_dict.keys())
             )
         )
 
     return input_unit
 
 
 def _clean_user_inputs(_input_unit, _target_unit, _unit_type_alias_dict):
```

### Comparing `PH-units-1.1.3/ph_units/parser.py` & `PH-units-1.2.0/ph_units/parser.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.3/ph_units/unit_types/__init__.py` & `PH-units-1.2.0/ph_units/unit_types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,32 @@
 from ph_units.unit_types import envelope
 from ph_units.unit_types import length
 from ph_units.unit_types import power
 from ph_units.unit_types import speed
 from ph_units.unit_types import temperature
 from ph_units.unit_types import volume_flow
 from ph_units.unit_types import volume
+from ph_units.unit_types import density
+from ph_units.unit_types import emissions_factors
+from ph_units.unit_types import moisture_vapor_resistance
 
 
 UNIT_TYPE_MODULES = (
     area,
     energy,
     envelope,
     length,
     power,
     speed,
     temperature,
     volume_flow,
     volume,
+    density,
+    emissions_factors,
+    moisture_vapor_resistance,
 )
 
 
 def _is_unit_class(cls):
     # type: (type) -> bool
     """Return True if the type is a Unit."""
     return hasattr(cls, "__symbol__") and hasattr(cls, "__factors__")
```

### Comparing `PH-units-1.1.3/ph_units/unit_types/energy.py` & `PH-units-1.2.0/ph_units/unit_types/energy.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     }
 
 
 class KiloWattHour(Base_UnitType):
     """KWH"""
 
     __symbol__ = "KWH"
-    __aliases__ = []
+    __aliases__ = ["KWH/YR", "KWH/A", "KWH/M", "KWH/MONTH"]
     __factors__ = {
         "WH": "{}*1000",
         "KWH": "{}*1",
         "BTU": "{}*3412.14",
         "KBTU": "{}*3.41214",
         "MJ": "{}*3.6",
         "KJ": "{}*3600",
@@ -150,45 +150,45 @@
     }
 
 
 class KilowattHoursPerMeterSquared(Base_UnitType):
     """KWH/M2"""
 
     __symbol__ = "KWH/M2"
-    __aliases__ = []
+    __aliases__ = ["KWH/M²MONTH", "KWH/M²A", "KWH/M²"]
     __factors__ = {
         "WH/M2": "{}*1000",
         "WH/FT2": "{}*92.903",
         "KWH/M2": "{}*1",
         "KWH/FT2": "{}*0.092903040",
         "BTU/FT2": "{}*316.998",
         "KBTU/FT2": "{}*0.316998286",
     }
 
 
 class KBtuPerFootSquared(Base_UnitType):
     """KBTU/FT2"""
 
     __symbol__ = "KBTU/FT2"
-    __aliases__ = ["KBTU/SF"]
+    __aliases__ = ["KBTU/SF", "KBTU/FT²MONTH", "KBTU/FT²YR", "KBTU/FT²A", "KBTU/FT²"]
     __factors__ = {
         "WH/M2": "{}*3154.59",
         "WH/FT2": "{}*293.071",
         "KWH/M2": "{}*3.15459",
         "KWH/FT2": "{}*0.293071",
         "BTU/FT2": "{}*1000",
         "KBTU/FT2": "{}*1",
     }
 
 
 class BtuPerFootSquared(Base_UnitType):
     """BTU/FT2"""
 
     __symbol__ = "BTU/FT2"
-    __aliases__ = ["BTU/SF"]
+    __aliases__ = ["BTU/SF", "BTU/FT²"]
     __factors__ = {
         "WH/M2": "{}*3.15459",
         "WH/FT2": "{}*0.293071",
         "KWH/M2": "{}*0.00315459",
         "KWH/FT2": "{}*0.000293071",
         "BTU/FT2": "{}*1",
         "KBTU/FT2": "{}*0.001",
@@ -198,17 +198,99 @@
 # ----------------- Energy Per Volume -----------------
 
 
 class WattHoursPerMeterCubed(Base_UnitType):
     """WH/M3"""
 
     __symbol__ = "WH/M3"
-    __aliases__ = []
+    __aliases__ = ["WH/M³"]
     __factors__ = {"WH/M3": "{}*1", "W/CFM": "{}*1.699010796"}
 
 
 class MegaJoulePerMeterCubedKelvin(Base_UnitType):
     """MJ/M3K"""
 
     __symbol__ = "MJ/M3K"
     __aliases__ = []
-    __factors__ = {"MJ/M3K": "{}*1", "BTU/FT3-F": "{}*14.91066014"}
+    __factors__ = {"MJ/M3K": "{}*1", "BTU/FT3F": "{}*14.91066014"}
+
+
+class BtuPerFootCubedDegreeFarenheirt(Base_UnitType):
+    """BTU/FT3F"""
+
+    __symbol__ = "BTU/FT3F"
+    __aliases__ = ["BTU/FT3°F"]
+    __factors__ = {"MJ/M3K": "{}*0.067066112", "BTU/FT3F": "{}*1"}
+
+
+# ----------------- Energy Per Mass -----------------
+
+
+class JoulePerKilogramDegreeKelvin(Base_UnitType):
+    """J/KG-K"""
+
+    __symbol__ = "J/KGK"
+    __aliases__ = ["J/KG-K"]
+    __factors__ = {"J/KGK": "{}*1", "BTU/LBF": "{}*0.000238846"}
+
+
+class BtuPerPoundDegreeFarenheirt(Base_UnitType):
+    """BTU/LB-F"""
+
+    __symbol__ = "BTU/LBF"
+    __aliases__ = ["BTU/LB-F", "BTU/LB°F"]
+    __factors__ = {"J/KGK": "{}*4186.800585", "BTU/LBF": "{}*1"}
+
+
+class WattHoursPerFootSquaredDegreeFarenheirt(Base_UnitType):
+    """WH/FT2F"""
+
+    __symbol__ = "WH/FT2F"
+    __aliases__ = ["WH/FT2-F", "WH/FT2°F", "WH/FT²F"]
+    __factors__ = {
+        "WH/M2K": "{}*19.37503875",
+        "WH/FT2F": "{}*1",
+        "BTU/FT2F": "{}*3.412141156",
+    }
+
+
+class WattHoursPerMeterSqauredPerDegreeKelvin(Base_UnitType):
+    """WH/M2K"""
+
+    __symbol__ = "WH/M2K"
+    __aliases__ = ["WH/M2K", "WH/M²K"]
+    __factors__ = {
+        "WH/M2K": "{}*1",
+        "WH/FT2F": "{}*0.0516128",
+        "BTU/FT2F": "{}*0.1761102",
+    }
+
+
+class BtuPerSquareFootDegreeFarenheirt(Base_UnitType):
+    """BTU/FT2-F"""
+
+    __symbol__ = "BTU/FT2F"
+    __aliases__ = ["BTU/FT2-F", "BTU/FT2°F", "BTU/FT²F"]
+    __factors__ = {
+        "BTU/FT2F": "{}*1",
+        "WH/FT2F": "{}*0.293071111",
+        "WH/M2K": "{}*5.678264134",
+    }
+
+
+# ----------------- Primary Energy Factors -----------------
+
+
+class KiloWattHourPerKiloWattHour(Base_UnitType):
+    """KWH/KWH"""
+
+    __symbol__ = "KWH/KWH"
+    __aliases__ = ["KWH/KWH"]
+    __factors__ = {"KWH/KWH": "{}*1", "BTU/BTU": "{}*3412.14"}
+
+
+class BtuPerBtu(Base_UnitType):
+    """BTU/BTU"""
+
+    __symbol__ = "BTU/BTU"
+    __aliases__ = ["BTU/BTU"]
+    __factors__ = {"KWH/KWH": "{}*0.000293071", "BTU/BTU": "{}*1"}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PH-units-1.1.3/ph_units/unit_types/envelope.py` & `PH-units-1.2.0/ph_units/unit_types/envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 from ph_units.unit_types._base import Base_UnitType
 
 
 class WattsPerMeterSquaredKelvin(Base_UnitType):
     """W/M2K (U-Value)"""
 
     __symbol__ = "W/M2K"
-    __aliases__ = ["U-SI"]
+    __aliases__ = ["U-SI", "W/M²K"]
     __factors__ = {
         "W/M2K": "{}*1",
         "M2K/W": "(1/{})",
         "BTU/HR-FT2-F": "{}*0.176110159",
         "HR-FT2-F/BTU": "(1/{})*5.678264134",
     }
 
 
 class BtuPerHourFootSquaredFahrenheit(Base_UnitType):
     """BTU/HR-FT2-F (U-Value)"""
 
     __symbol__ = "BTU/HR-FT2-F"
-    __aliases__ = ["U-IP", "BTU/HR-SF-F", "BTU/H-SF-F"]
+    __aliases__ = ["U-IP", "BTU/HR-SF-F", "BTU/H-SF-F", "BTU/HRFT²°F"]
     __factors__ = {
         "W/M2K": "{}*5.678264134",
         "M2K/W": "1/({}*5.678264134)",
         "BTU/HR-FT2-F": "{}*1",
         "HR-FT2-F/BTU": "(1/{})",
     }
 
 
 class MeterSquaredKelvinPerWatt(Base_UnitType):
     """M2K/W (R-Value)"""
 
     __symbol__ = "M2K/W"
-    __aliases__ = ["R-SI"]
+    __aliases__ = ["R-SI", "M²K/W"]
     __factors__ = {
         "M2K/W": "{}*1",
         "W/M2K": "(1/{})",
         "HR-FT2-F/BTU": "{}*5.678264134",
         "BTU/HR-FT2-F": "1/({}*5.678264134)",
     }
 
@@ -79,15 +79,15 @@
     }
 
 
 class BtuPerHourFootFahrenheit(Base_UnitType):
     """BTU/HR-FT-F (Psi-Value)"""
 
     __symbol__ = "BTU/HR-FT-F"
-    __aliases__ = []
+    __aliases__ = ["BTU/HRFT°F"]
     __factors__ = {
         "W/MK": "{}*1.730734908",
         "HR-FT2-F/BTU-IN": "1/({}*12)",
         "BTU/HR-FT-F": "{}*1",
     }
 
 
@@ -99,9 +99,9 @@
     __factors__ = {"W/K": "{}*1", "BTU/HR-F": "{}*1.895633976"}
 
 
 class BtuPerHourFahrenheit(Base_UnitType):
     """BTU/HR-F (Chi-Value)"""
 
     __symbol__ = "BTU/HR-F"
-    __aliases__ = []
+    __aliases__ = ["BTU/HRF", "BTU/HR-F", "BTU/HR-F", "BTU/HR°F", "BTU/HR-°F"]
     __factors__ = {"W/K": "{}*0.527528", "BTU/HR-F": "{}*1"}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PH-units-1.1.3/ph_units/unit_types/length.py` & `PH-units-1.2.0/ph_units/unit_types/length.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.3/ph_units/unit_types/power.py` & `PH-units-1.2.0/ph_units/unit_types/power.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,28 +17,28 @@
     }
 
 
 class Watts(Base_UnitType):
     """W"""
 
     __symbol__ = "W"
-    __aliases__ = []
+    __aliases__ = ["WATT", "WATTS"]
     __factors__ = {
         "W": "{}*1",
         "KW": "{}*0.001",
         "BTUH": "{}*3.412141156",
         "KBTUH": "{}*0.003412141",
     }
 
 
 class WattsPerMeterSquared(Base_UnitType):
     """W/M2"""
 
     __symbol__ = "W/M2"
-    __aliases__ = []
+    __aliases__ = ["W/M²"]
     __factors__ = {
         "W/M2": "{}*1",
         "BTU/HR-FT2": "{}*0.316998286",
         "W/FT2": "{}*0.09290304",
     }
 
 
@@ -50,18 +50,19 @@
     __factors__ = {"W/W": "{}*1", "BTUHR/W": "{}*3.412141156"}
 
 
 class WattsPerFootSquared(Base_UnitType):
     """W/FT2"""
 
     __symbol__ = "W/FT2"
-    __aliases__ = []
+    __aliases__ = ["W/SF", "W/FT²"]
     __factors__ = {
+        "W/FT2": "{}*1",
         "W/M2": "{}*10.76391042",
-        "BTU/HR-FT2": "{}/3.412141156",
+        "BTU/HR-FT2": "{}*3.154591186",
     }
 
 
 class WattsPerFootCubedPerMinute(Base_UnitType):
     """W/CFM"""
 
     __symbol__ = "W/CFM"
@@ -69,36 +70,39 @@
     __factors__ = {"W/CFM": "{}*0.588577779", "WH/M3": "{}*0.588577779"}
 
 
 class BtuPerHourFootSquared(Base_UnitType):
     """BTU/HR-FT2"""
 
     __symbol__ = "BTU/HR-FT2"
-    __aliases__ = ["BTUH/FT2", "BTU/H-SF", "BTU/H-FT2"]
+    __aliases__ = ["BTUH/FT2", "BTU/H-SF", "BTU/H-FT2", "BTU/HRFT²"]
     __factors__ = {
+        "BTU/HR-FT2": "{}*1",
         "W/M2": "{}*3.154591186",
         "W/FT2": "{}*0.293071111",
     }
 
 
 class BtuPerHour(Base_UnitType):
     """BTU/H"""
 
     __symbol__ = "BTUH"
     __aliases__ = ["BTU/HR", "BTU/H", "BTUHR"]
     __factors__ = {
+        "BTUH": "{}*1",
         "KBTUH": "{}/1000",
         "W": "{}*0.293071111",
         "KW": "{}*0.000293071",
     }
 
 
 class KiloBtuPerHour(Base_UnitType):
     """KBTU/H"""
 
     __symbol__ = "KBTUH"
     __aliases__ = ["KBTU/HR", "KBTU/H", "KBTUHR"]
     __factors__ = {
+        "KBTUH": "{}*1",
         "BTUH": "{}*1000",
         "W": "{}*293.0711111",
         "KW": "{}*0.293071111",
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PH-units-1.1.3/ph_units/unit_types/speed.py` & `PH-units-1.2.0/ph_units/unit_types/speed.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ph_units.unit_types._base import Base_UnitType
 
 
 class MeterPerDay(Base_UnitType):
     """Meter/Day"""
 
     __symbol__ = "M/DAY"
-    __aliases__ = []
+    __aliases__ = ["M/D", "METER/DAY", "METER/D", "M/DAY"]
     __factors__ = {
         "M/DAY": "{}*1",
         "FT/DAY": "{}*3.280839895",
         "M/S": "{}/24/60/60",
     }
 
 
@@ -21,27 +21,29 @@
 
     __symbol__ = "M/S"
     __aliases__ = ["METER/SEC", "METER/SECOND", "M/SECOND"]
     __factors__ = {
         "M/S": "{}*1",
         "M/DAY": "{}*24*60*60",
         "FT/S": "{}*3.280839895",
-        "FT/DAY": "{}*3.280839895*24*60*60",
+        "FT/DAY": "{}*3.280839895 * 24 * 60 * 60",
         "MPH": "{}/0.44704",
     }
 
 
 class MilesPerHour(Base_UnitType):
     """MPH"""
 
-    __symbol__ = "M/DAY"
+    __symbol__ = "MPH"
     __aliases__ = []
     __factors__ = {
         "M/S": "{}*0.44704",
         "M/DAY": "{}*0.44704*60*60*24",
+        "FT/S": "{}*1.466666667",
+        "FT/DAY": "{}*1.466666667*60*60*24",
     }
 
 
 class FeetPerSecond(Base_UnitType):
     """FT/Second"""
 
     __symbol__ = "FT/S"
@@ -50,8 +52,13 @@
 
 
 class FeetPerDay(Base_UnitType):
     """FT/Day"""
 
     __symbol__ = "FT/DAY"
     __aliases__ = ["FT/D"]
-    __factors__ = {"M/DAY": "{}*0.3048"}
+    __factors__ = {
+        "FT/DAY": "{}*1",
+        "FT/S": "{}*1/24/60/60",
+        "M/DAY": "{}*0.3048",
+        "M/S": "{}*0.3048/24/60/60",
+    }
```

### Comparing `PH-units-1.1.3/ph_units/unit_types/temperature.py` & `PH-units-1.2.0/ph_units/unit_types/temperature.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,36 +4,45 @@
 from ph_units.unit_types._base import Base_UnitType
 
 
 class Celsius(Base_UnitType):
     "Celsius"
 
     __symbol__ = "C"
-    __aliases__ = ["DEG C", "DEG. C", "°C"]
+    __aliases__ = ["DEGC", "DEG.C", "°C"]
     __factors__ = {"C": "{}*1", "F": "{}*1.8+32"}
 
 
 class DeltaCelsius(Base_UnitType):
     "Delta-Celsius"
 
     __symbol__ = "DELTA-C"
     __aliases__ = []
-    __factors__ = {"DELTA-C": "{}*1", "DELTA-F": "{}*1.8"}
+    __factors__ = {"DELTA-C": "{}*1", "DELTA-K": "{}*1", "DELTA-F": "{}*1.8"}
+
+
+class DeltaKelvin(Base_UnitType):
+    "Delta-Kelvin"
+
+    __symbol__ = "DELTA-K"
+    __aliases__ = []
+    __factors__ = {"DELTA-K": "{}*1", "DELTA-C": "{}*1", "DELTA-F": "{}*1.8"}
 
 
 class Fahrenheit(Base_UnitType):
     "Fahrenheit"
 
     __symbol__ = "F"
-    __aliases__ = ["DEG F", "DEG. F", "°F"]
+    __aliases__ = ["DEGF", "DEG.F", "°F"]
     __factors__ = {"C": "({}-32)/1.8"}
 
 
 class DeltaFahrenheit(Base_UnitType):
     "Delta-Fahrenheit"
 
     __symbol__ = "DELTA-F"
     __aliases__ = []
     __factors__ = {
         "DELTA-C": "{}*0.555555556",
+        "DELTA-K": "{}*0.555555556",
         "DELTA-F": "{}*1",
     }
```

### Comparing `PH-units-1.1.3/ph_units/unit_types/volume.py` & `PH-units-1.2.0/ph_units/unit_types/volume.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ph_units.unit_types._base import Base_UnitType
 
 
 class MeterCubed(Base_UnitType):
     """Meter Cubed"""
 
     __symbol__ = "M3"
-    __aliases__ = []
+    __aliases__ = ["M³", "M3", "METERCUBED", "CUBICMETER"]
     __factors__ = {
         "M3": "{}*1",
         "FT3": "{}*35.31466672",
         "L": "{}*1000",
         "GA": "{}*264.1720524",
     }
 
@@ -30,20 +30,27 @@
     }
 
 
 class Gallon(Base_UnitType):
     """Gallon"""
 
     __symbol__ = "GA"
-    __aliases__ = ["GALLON", "G"]
-    __factors__ = {"L": "{}*3.785411784"}
+    __aliases__ = ["GALLON", "G", "GAL"]
+    __factors__ = {
+        "GA": "{}*1",
+        "L": "{}*3.785411784",
+        "M3": "{}*0.003785411784",
+        "FT3": "{}*0.13368055555555556",
+    }
 
 
 class FootCubed(Base_UnitType):
     """Foot Cubed"""
 
     __symbol__ = "FT3"
-    __aliases__ = ["CF"]
+    __aliases__ = ["CF", "FT3", "FT³", "CUBIC FOOT", "CUBIC FEET"]
     __factors__ = {
         "M3": "{}*0.028316847",
         "FT3": "{}*1",
+        "L": "{}*28.316846592",
+        "GA": "{}*7.48051948051948",
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PH-units-1.1.3/ph_units/unit_types/volume_flow.py` & `PH-units-1.2.0/ph_units/unit_types/volume_flow.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,60 +4,77 @@
 from ph_units.unit_types._base import Base_UnitType
 
 
 class MeterCubedPerSecond(Base_UnitType):
     """M3/S"""
 
     __symbol__ = "M3/S"
-    __aliases__ = ["M3/SECOND", "M3/SEC", "CM/S"]
+    __aliases__ = ["M3/SECOND", "M3/SEC", "CM/S", "M³/S"]
     __factors__ = {
         "M3/S": "{}*1",
         "M3/M": "{}*60",
         "M3/HR": "{}*60*60",
         "CFM": "({}*60*60)*0.588577779",
         "CFH": "({}*60*60*60)*0.588577779",
     }
 
 
 class MeterCubedPerMinute(Base_UnitType):
     """M3/M"""
 
     __symbol__ = "M3/M"
-    __aliases__ = ["M3/MIN", "M3/MINUTE", "CM/M"]
+    __aliases__ = ["M3/MIN", "M3/MINUTE", "CM/M", "M³/MIN"]
     __factors__ = {
         "M3/S": "{}/60",
         "M3/M": "{}*1",
         "M3/HR": "{}*60",
         "CFM": "({}*60)*0.588577779",
         "CFH": "({}*60*60)*0.588577779",
     }
 
 
 class MeterCubedPerHour(Base_UnitType):
     """M3/HR"""
 
     __symbol__ = "M3/HR"
-    __aliases__ = ["CM/H", "CMH", "M3/H"]
+    __aliases__ = ["CM/H", "CMH", "M3/H", "M³/H", "M³/HR"]
     __factors__ = {
         "M3/S": "({}/60)/60",
         "M3/M": "{}/60",
         "M3/HR": "{}*1",
         "CFM": "{}*0.588577779",
         "CFH": "({}*60)*0.588577779",
     }
 
 
+class MeterCubedPerHourPerMeterSquared(Base_UnitType):
+    """M3/HR-M2"""
+
+    __symbol__ = "M3/HRM2"
+    __aliases__ = [
+        "M3/HR-M2",
+        "M3/HRM2",
+        "M3/HR-M^2",
+        "M3/HRM^2",
+        "M³/M²H",
+        "M3/M2H",
+        "M3/M²H",
+        "M³/M²H",
+    ]
+    __factors__ = {"M3/HRM2": "{}*1", "CFM/FT2": "{}*0.054680665"}
+
+
 # -- IP
 
 
 class FootCubedPerMinute(Base_UnitType):
     """CFM"""
 
     __symbol__ = "CFM"
-    __aliases__ = ["FT3/M", "FT3M"]
+    __aliases__ = ["FT3/M", "FT3M", "FT³/M", "FT³M", "CF/M"]
     __factors__ = {
         "M3/S": "(({}*1.699010796)/60)/60",
         "M3/M": "({}*1.699010796)/60",
         "M3/HR": "{}*1.699010796",
         "CFM": "{}*1",
         "CFH": "{}*60",
     }
@@ -71,7 +88,15 @@
     __factors__ = {
         "M3/S": "(({}/60)*1.699010796)/60/60",
         "M3/M": "(({}/60)*1.699010796)/60",
         "M3/HR": "(({}/60)*1.699010796)",
         "CFM": "{}/60",
         "CFH": "{}*1",
     }
+
+
+class FootCubedPerMinutePerFootSqaure(Base_UnitType):
+    """CFM/FT2"""
+
+    __symbol__ = "CFM/FT2"
+    __aliases__ = ["CFM/SF", "CFM/FT²", "CFM/SQFT", "CFM/SQFT"]
+    __factors__ = {"CFM/FT2": "{}*1", "M3/HRM2": "{}*18.288"}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PH-units-1.1.3/setup.cfg` & `PH-units-1.2.0/setup.cfg`

 * *Files identical despite different names*

