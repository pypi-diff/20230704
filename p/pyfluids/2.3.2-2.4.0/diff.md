# Comparing `tmp/pyfluids-2.3.2.tar.gz` & `tmp/pyfluids-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfluids-2.3.2.tar", max compression
+gzip compressed data, was "pyfluids-2.4.0.tar", max compression
```

## Comparing `pyfluids-2.3.2.tar` & `pyfluids-2.4.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
--rw-r--r--   0        0        0     1078 2022-12-21 12:46:53.725937 pyfluids-2.3.2/LICENSE
--rw-r--r--   0        0        0     1203 2022-12-21 12:46:53.725937 pyfluids-2.3.2/PyPI.md
--rw-r--r--   0        0        0      161 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/__init__.py
--rw-r--r--   0        0        0      130 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/enums/__init__.py
--rw-r--r--   0        0        0    12624 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/enums/fluids_list.py
--rw-r--r--   0        0        0      253 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/enums/mix.py
--rw-r--r--   0        0        0      640 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/enums/phases.py
--rw-r--r--   0        0        0       87 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/fluids/__init__.py
--rw-r--r--   0        0        0    23806 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/fluids/abstract_fluid.py
--rw-r--r--   0        0        0     3148 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/fluids/fluid.py
--rw-r--r--   0        0        0     2304 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/fluids/mixture.py
--rw-r--r--   0        0        0       54 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/humid_air/__init__.py
--rw-r--r--   0        0        0    22447 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/humid_air/humid_air.py
--rw-r--r--   0        0        0      164 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/io/__init__.py
--rw-r--r--   0        0        0      999 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/io/abstract_input.py
--rw-r--r--   0        0        0     2348 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/io/input.py
--rw-r--r--   0        0        0     3972 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/io/input_humid_air.py
--rw-r--r--   0        0        0      481 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyfluids/io/outputs_validator.py
--rw-r--r--   0        0        0     2034 2022-12-21 12:46:53.733936 pyfluids-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 pyfluids-2.3.2/setup.py
--rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 pyfluids-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-04 13:52:39.912248 pyfluids-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1203 2023-07-04 13:52:39.912248 pyfluids-2.4.0/PyPI.md
+-rw-r--r--   0        0        0      208 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/pyfluids_config.py
+-rw-r--r--   0        0        0     3638 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/pyfluids_config_builder.py
+-rw-r--r--   0        0        0      239 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/singleton.py
+-rw-r--r--   0        0        0     1886 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/unit_converter.py
+-rw-r--r--   0        0        0      341 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/config/units_system.py
+-rw-r--r--   0        0        0      130 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/__init__.py
+-rw-r--r--   0        0        0    12938 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/fluids_list.py
+-rw-r--r--   0        0        0      267 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/mix.py
+-rw-r--r--   0        0        0      654 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/enums/phases.py
+-rw-r--r--   0        0        0       87 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/__init__.py
+-rw-r--r--   0        0        0    25819 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/abstract_fluid.py
+-rw-r--r--   0        0        0     3665 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/fluid.py
+-rw-r--r--   0        0        0     3419 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/fluids/mixture.py
+-rw-r--r--   0        0        0       54 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/humid_air/__init__.py
+-rw-r--r--   0        0        0    24476 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/humid_air/humid_air.py
+-rw-r--r--   0        0        0      164 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/abstract_input.py
+-rw-r--r--   0        0        0     2886 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/input.py
+-rw-r--r--   0        0        0     4758 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/input_humid_air.py
+-rw-r--r--   0        0        0      481 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyfluids/io/outputs_validator.py
+-rw-r--r--   0        0        0     2050 2023-07-04 13:52:39.920248 pyfluids-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 pyfluids-2.4.0/PKG-INFO
```

### Comparing `pyfluids-2.3.2/LICENSE` & `pyfluids-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfluids-2.3.2/PyPI.md` & `pyfluids-2.4.0/PyPI.md`

 * *Files identical despite different names*

### Comparing `pyfluids-2.3.2/pyfluids/enums/fluids_list.py` & `pyfluids-2.4.0/pyfluids/enums/fluids_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from enum import Enum
 
 from .mix import Mix
+from ..config import UnitConverter
+
 
 __all__ = ["FluidsList"]
 
 
 class FluidsList(Enum):
     """List of CoolProp fluids.
 
@@ -405,18 +407,18 @@
             backend,
             pure,
             mix_type,
             fraction_min,
             fraction_max,
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.name
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
     @property
     def coolprop_name(self) -> str:
         """CoolProp internal name."""
         return self.__coolprop_name
 
@@ -433,14 +435,20 @@
     @property
     def mix_type(self) -> Mix:
         """Mass-based or volume-based mixture."""
         return self.__mix_type
 
     @property
     def fraction_min(self) -> float:
-        """Minimum possible fraction [%]."""
-        return self.__fraction_min * 1e2
+        """
+        Minimum possible fraction
+        [by default, %; you can change this using the configuration file].
+        """
+        return UnitConverter().convert_decimal_fraction_from_si(self.__fraction_min)
 
     @property
     def fraction_max(self) -> float:
-        """Maximum possible fraction [%]."""
-        return self.__fraction_max * 1e2
+        """
+        Maximum possible fraction
+        [by default, %; you can change this using the configuration file].
+        """
+        return UnitConverter().convert_decimal_fraction_from_si(self.__fraction_max)
```

### Comparing `pyfluids-2.3.2/pyfluids/enums/phases.py` & `pyfluids-2.4.0/pyfluids/enums/phases.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     SupercriticalLiquid = CoolProp.iphase_supercritical_liquid
     CriticalPoint = CoolProp.iphase_critical_point
     Gas = CoolProp.iphase_gas
     TwoPhase = CoolProp.iphase_twophase
     Unknown = CoolProp.iphase_unknown
     NotImposed = CoolProp.iphase_not_imposed
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.name
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
```

### Comparing `pyfluids-2.3.2/pyfluids/fluids/abstract_fluid.py` & `pyfluids-2.4.0/pyfluids/fluids/abstract_fluid.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import json
 from abc import ABC, abstractmethod
 
 import CoolProp
 from CoolProp import AbstractState
 from CoolProp.CoolProp import generate_update_pair
 
+from ..config import UnitConverter, UnitsSystem
 from ..enums import Phases
 from ..io import Input, OutputsValidator
 
 
 class AbstractFluid(ABC):
-    """Fluids base class."""
+    """Base class of fluids."""
 
     @abstractmethod
     def __init__(self):
-        """Fluids base class."""
+        """Base class of fluids."""
         self._backend: AbstractState | None = None
         self._inputs: list[Input] = []
         self.__compressibility: float | None = None
         self.__conductivity: float | None = None
         self.__critical_pressure: float | None = None
         self.__critical_temperature: float | None = None
         self.__density: float | None = None
@@ -40,14 +41,23 @@
         self.__quality: float | None = None
         self.__sound_speed: float | None = None
         self.__specific_heat: float | None = None
         self.__surface_tension: float | None = None
         self.__temperature: float | None = None
         self.__triple_pressure: float | None = None
         self.__triple_temperature: float | None = None
+        self._unit_converter: UnitConverter = UnitConverter()
+        self._fraction_unit: str = (
+            " %" if self.units_system == UnitsSystem.SIWithCelsiusAndPercents else ""
+        )
+
+    @property
+    def units_system(self) -> UnitsSystem:
+        """Configured units system."""
+        return self._unit_converter.units_system
 
     @property
     def compressibility(self) -> float | None:
         """Compressibility factor [-]."""
         if self.__compressibility is None:
             self.__compressibility = self._nullable_keyed_output(CoolProp.iZ)
         return self.__compressibility
@@ -64,18 +74,25 @@
         """Absolute pressure at the critical point [Pa]."""
         if self.__critical_pressure is None:
             self.__critical_pressure = self._nullable_keyed_output(CoolProp.iP_critical)
         return self.__critical_pressure
 
     @property
     def critical_temperature(self) -> float | None:
-        """Temperature at the critical point [°C]."""
+        """
+        Temperature at the critical point
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__critical_temperature is None:
             value = self._nullable_keyed_output(CoolProp.iT_critical)
-            self.__critical_temperature = value - 273.15 if value is not None else None
+            self.__critical_temperature = (
+                self._unit_converter.convert_temperature_from_si(value)
+                if value is not None
+                else None
+            )
         return self.__critical_temperature
 
     @property
     def density(self) -> float:
         """Mass density [kg/m3]."""
         if self.__density is None:
             self.__density = self._keyed_output(CoolProp.iDmass)
@@ -100,18 +117,25 @@
         """Mass specific entropy [J/kg/K]."""
         if self.__entropy is None:
             self.__entropy = self._keyed_output(CoolProp.iSmass)
         return self.__entropy
 
     @property
     def freezing_temperature(self) -> float | None:
-        """Temperature at the freezing point (for incompressible fluids) [°C]."""
+        """
+        Temperature at the freezing point (for incompressible fluids)
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__freezing_temperature is None:
             value = self._nullable_keyed_output(CoolProp.iT_freeze)
-            self.__freezing_temperature = value - 273.15 if value is not None else None
+            self.__freezing_temperature = (
+                self._unit_converter.convert_temperature_from_si(value)
+                if value is not None
+                else None
+            )
         return self.__freezing_temperature
 
     @property
     def internal_energy(self) -> float:
         """Mass specific internal energy [J/kg]."""
         if self.__internal_energy is None:
             self.__internal_energy = self._keyed_output(CoolProp.iUmass)
@@ -131,33 +155,47 @@
         """Maximum pressure limit [Pa]."""
         if self.__max_pressure is None:
             self.__max_pressure = self._nullable_keyed_output(CoolProp.iP_max)
         return self.__max_pressure
 
     @property
     def max_temperature(self) -> float:
-        """Maximum temperature limit [°C]."""
+        """
+        Maximum temperature limit
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__max_temperature is None:
             value = self._keyed_output(CoolProp.iT_max)
-            self.__max_temperature = value - 273.15 if value is not None else None
+            self.__max_temperature = (
+                self._unit_converter.convert_temperature_from_si(value)
+                if value is not None
+                else None
+            )
         return self.__max_temperature
 
     @property
     def min_pressure(self) -> float | None:
         """Minimum pressure limit [Pa]."""
         if self.__min_pressure is None:
             self.__min_pressure = self._nullable_keyed_output(CoolProp.iP_min)
         return self.__min_pressure
 
     @property
     def min_temperature(self) -> float:
-        """Minimum temperature limit [°C]."""
+        """
+        Minimum temperature limit
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__min_temperature is None:
             value = self._keyed_output(CoolProp.iT_min)
-            self.__min_temperature = value - 273.15 if value is not None else None
+            self.__min_temperature = (
+                self._unit_converter.convert_temperature_from_si(value)
+                if value is not None
+                else None
+            )
         return self.__min_temperature
 
     @property
     def molar_mass(self) -> float | None:
         """Molar mass [kg/mol]."""
         if self.__molar_mass is None:
             self.__molar_mass = self._nullable_keyed_output(CoolProp.imolar_mass)
@@ -182,18 +220,25 @@
         """Absolute pressure [Pa]."""
         if self.__pressure is None:
             self.__pressure = self._keyed_output(CoolProp.iP)
         return self.__pressure
 
     @property
     def quality(self) -> float | None:
-        """Mass vapor quality [%]."""
+        """
+        Mass vapor quality
+        [by default, %; you can change this using the configuration file].
+        """
         if self.__quality is None:
             value = self._nullable_keyed_output(CoolProp.iQ)
-            self.__quality = value * 1e2 if value is not None else None
+            self.__quality = (
+                self._unit_converter.convert_decimal_fraction_from_si(value)
+                if value is not None
+                else None
+            )
         return self.__quality
 
     @property
     def sound_speed(self) -> float | None:
         """Sound speed [m/s]."""
         if self.__sound_speed is None:
             self.__sound_speed = self._nullable_keyed_output(CoolProp.ispeed_sound)
@@ -203,43 +248,62 @@
     def specific_heat(self) -> float:
         """Mass specific constant pressure specific heat [J/kg/K]."""
         if self.__specific_heat is None:
             self.__specific_heat = self._keyed_output(CoolProp.iCpmass)
         return self.__specific_heat
 
     @property
+    def specific_volume(self) -> float:
+        """Mass specific volume [m3/kg]."""
+        return 1 / self.density
+
+    @property
     def surface_tension(self) -> float | None:
         """Surface tension [N/m]."""
         if self.__surface_tension is None:
             self.__surface_tension = self._nullable_keyed_output(
                 CoolProp.isurface_tension
             )
         return self.__surface_tension
 
     @property
     def temperature(self) -> float:
-        """Temperature [°C]."""
+        """
+        Temperature
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__temperature is None:
             value = self._keyed_output(CoolProp.iT)
-            self.__temperature = value - 273.15 if value is not None else None
+            self.__temperature = (
+                self._unit_converter.convert_temperature_from_si(value)
+                if value is not None
+                else None
+            )
         return self.__temperature
 
     @property
     def triple_pressure(self) -> float | None:
         """Absolute pressure at the triple point [Pa]."""
         if self.__triple_pressure is None:
             self.__triple_pressure = self._nullable_keyed_output(CoolProp.iP_triple)
         return self.__triple_pressure
 
     @property
     def triple_temperature(self) -> float | None:
-        """Temperature at the triple point [°C]."""
+        """
+        Temperature at the triple point
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__triple_temperature is None:
             value = self._nullable_keyed_output(CoolProp.iT_triple)
-            self.__triple_temperature = value - 273.15 if value is not None else None
+            self.__triple_temperature = (
+                self._unit_converter.convert_temperature_from_si(value)
+                if value is not None
+                else None
+            )
         return self.__triple_temperature
 
     @abstractmethod
     def factory(self) -> AbstractFluid:
         """Returns a new fluid instance with no defined state."""
         raise NotImplementedError  # pragma: no cover
 
@@ -280,14 +344,15 @@
             )
         )
         self._inputs = [first_input, second_input]
 
     # noinspection DuplicatedCode
     def reset(self):
         """Resets all non-trivial properties."""
+        self._inputs.clear()
         self.__compressibility = None
         self.__conductivity = None
         self.__density = None
         self.__dynamic_viscosity = None
         self.__enthalpy = None
         self.__entropy = None
         self.__internal_energy = None
@@ -317,29 +382,33 @@
     def compression_to_pressure(
         self, pressure: float, isentropic_efficiency: float
     ) -> AbstractFluid:
         """
         The process of compression to a given pressure.
 
         :param pressure: Absolute pressure [Pa].
-        :param isentropic_efficiency: Compressor isentropic efficiency [%].
+        :param isentropic_efficiency: Compressor isentropic efficiency
+            [by default, %; you can change this using the configuration file].
         :return: The state of the fluid at the end of the process.
         :raises ValueError: If pressure or isentropic efficiency is invalid.
         """
-        if not 0 < isentropic_efficiency < 100:
+        isentropic_efficiency = self._unit_converter.convert_decimal_fraction_to_si(
+            isentropic_efficiency
+        )
+        if not 0 < isentropic_efficiency < 1:
             raise ValueError("Invalid compressor isentropic efficiency!")
         return self.with_state(
             Input.pressure(pressure),
             Input.enthalpy(
                 self.enthalpy
                 + (
                     self.isentropic_compression_to_pressure(pressure).enthalpy
                     - self.enthalpy
                 )
-                / (isentropic_efficiency * 1e-2)
+                / isentropic_efficiency
             ),
         )
 
     def isenthalpic_expansion_to_pressure(self, pressure: float) -> AbstractFluid:
         """
         The process of isenthalpic expansion to a given pressure.
 
@@ -370,39 +439,44 @@
     def expansion_to_pressure(
         self, pressure: float, isentropic_efficiency: float
     ) -> AbstractFluid:
         """
         The process of expansion to a given pressure.
 
         :param pressure: Absolute pressure [Pa].
-        :param isentropic_efficiency: Expander isentropic efficiency [%].
+        :param isentropic_efficiency: Expander isentropic efficiency
+            [by default, %; you can change this using the configuration file].
         :return: The state of the fluid at the end of the process.
         :raises ValueError: If pressure or isentropic efficiency is invalid.
         """
-        if not 0 < isentropic_efficiency < 100:
+        isentropic_efficiency = self._unit_converter.convert_decimal_fraction_to_si(
+            isentropic_efficiency
+        )
+        if not 0 < isentropic_efficiency < 1:
             raise ValueError("Invalid expander isentropic efficiency!")
         return self.with_state(
             Input.pressure(pressure),
             Input.enthalpy(
                 self.enthalpy
                 - (
                     self.enthalpy
                     - self.isentropic_expansion_to_pressure(pressure).enthalpy
                 )
-                * (isentropic_efficiency * 1e-2)
+                * isentropic_efficiency
             ),
         )
 
     def cooling_to_temperature(
         self, temperature: float, pressure_drop: float = 0
     ) -> AbstractFluid:
         """
         The process of cooling to a given temperature.
 
-        :param temperature: Temperature [°C].
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
         :param pressure_drop: Pressure drop in the heat exchanger (optional) [Pa].
         :return: The state of the fluid at the end of the process.
         :raises ValueError: If temperature or pressure drop is invalid.
         """
         if not temperature < self.temperature:
             raise ValueError(
                 "During the cooling process, the temperature should decrease!"
@@ -428,15 +502,16 @@
 
     def heating_to_temperature(
         self, temperature: float, pressure_drop: float = 0
     ) -> AbstractFluid:
         """
         The process of heating to a given temperature.
 
-        :param temperature: Temperature [°C].
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
         :param pressure_drop: Pressure drop in the heat exchanger (optional) [Pa].
         :return: The state of the fluid at the end of the process.
         :raises ValueError: If temperature or pressure drop is invalid.
         """
         if not temperature > self.temperature:
             raise ValueError(
                 "During the heating process, the temperature should increase!"
@@ -469,45 +544,58 @@
         """
         return self.with_state(Input.pressure(pressure), Input.quality(0))
 
     def bubble_point_at_temperature(self, temperature: float) -> AbstractFluid:
         """
         Bubble point at a given temperature.
 
-        :param temperature: Temperature [°C].
-        :return: TBubble point at a given temperature.
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
+        :return: Bubble point at a given temperature.
         """
         return self.with_state(Input.temperature(temperature), Input.quality(0))
 
     def dew_point_at_pressure(self, pressure: float) -> AbstractFluid:
         """
         Dew point at a given pressure.
 
         :param pressure: Absolute pressure [Pa].
         :return: Dew point at a given pressure.
         """
-        return self.with_state(Input.pressure(pressure), Input.quality(100))
+        return self.with_state(
+            Input.pressure(pressure),
+            Input.quality(
+                100 if self.units_system == UnitsSystem.SIWithCelsiusAndPercents else 1
+            ),
+        )
 
     def dew_point_at_temperature(self, temperature: float) -> AbstractFluid:
         """
         Dew point at a given temperature.
 
-        :param temperature: Temperature [°C].
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
         :return: Dew point at a given temperature.
         """
-        return self.with_state(Input.temperature(temperature), Input.quality(100))
+        return self.with_state(
+            Input.temperature(temperature),
+            Input.quality(
+                100 if self.units_system == UnitsSystem.SIWithCelsiusAndPercents else 1
+            ),
+        )
 
     def two_phase_point_at_pressure(
         self, pressure: float, quality: float
     ) -> AbstractFluid:
         """
         Two phase point at a given pressure.
 
         :param pressure: Absolute pressure [Pa].
-        :param quality: Vapor quality [%].
+        :param quality: Vapor quality
+            [by default, %; you can change this using the configuration file].
         :return: Two phase point at a given pressure.
         """
         return self.with_state(Input.pressure(pressure), Input.quality(quality))
 
     def mixing(
         self,
         first_specific_mass_flow: float,
@@ -551,23 +639,21 @@
         """
         return json.dumps(
             self.as_dict(), indent=4 if indented else None, default=str, sort_keys=False
         )
 
     def as_dict(self) -> dict[str, str | float | None]:
         """Converts the fluid instance to a dict."""
-        dictionary = {
-            self.__select(key): getattr(self, self.__select(key))
-            for key, value in vars(self).items()
-            if not self.__select(key).startswith("_")
-        }
-        return {
-            key: dictionary[key]
-            for key in list(dictionary.keys())[-2:] + list(dictionary.keys())[:-2]
-        }
+        keys = [
+            key
+            for key in dir(self.__class__)
+            if isinstance(getattr(self.__class__, key), property)
+        ]
+        values = [getattr(self, key) for key in keys]
+        return {key: value for key, value in zip(keys, values)}
 
     def _nullable_keyed_output(self, coolprop_key: int) -> float | None:
         try:
             value = self._keyed_output(coolprop_key)
             return (
                 None if coolprop_key == CoolProp.iQ and (not 0 <= value <= 1) else value
             )
@@ -585,39 +671,16 @@
         )
         OutputsValidator(value).validate()
         return value
 
     def __hash__(self) -> int:
         return hash(
             (
-                self.compressibility,
-                self.conductivity,
-                self.critical_pressure,
-                self.critical_temperature,
-                self.density,
-                self.dynamic_viscosity,
-                self.enthalpy,
-                self.entropy,
-                self.freezing_temperature,
-                self.internal_energy,
-                self.max_pressure,
-                self.max_temperature,
-                self.min_pressure,
-                self.min_temperature,
-                self.molar_mass,
-                self.phase,
-                self.prandtl,
-                self.pressure,
-                self.quality,
-                self.sound_speed,
-                self.specific_heat,
-                self.surface_tension,
-                self.temperature,
-                self.triple_pressure,
-                self.triple_temperature,
+                "&".join(str(i.value) for i in self._inputs),
+                "&".join(str(i.coolprop_key) for i in self._inputs),
             )
         )
 
     def __heat_transfer_to_temperature(
         self, temperature: float, pressure_drop: float
     ) -> AbstractFluid:
         self.__check_pressure_drop(pressure_drop)
@@ -635,11 +698,7 @@
             Input.enthalpy(enthalpy),
         )
 
     @staticmethod
     def __check_pressure_drop(pressure_drop: float):
         if pressure_drop < 0:
             raise ValueError("Invalid pressure drop in the heat exchanger!")
-
-    @staticmethod
-    def __select(key: str) -> str:
-        return key.split("__")[-1]
```

### Comparing `pyfluids-2.3.2/pyfluids/fluids/fluid.py` & `pyfluids-2.4.0/pyfluids/fluids/fluid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 from __future__ import annotations
 
 from CoolProp import AbstractState
 
 from .abstract_fluid import AbstractFluid
+from ..config import UnitsSystem
 from ..enums import FluidsList, Mix
 
 __all__ = ["Fluid"]
 
 
 class Fluid(AbstractFluid):
     """Pure/pseudo-pure fluid or binary mixture."""
 
     def __init__(self, name: FluidsList, fraction: float | None = None):
         """
         Pure/pseudo-pure fluid or binary mixture.
 
         :param name: Selected fluid name.
-        :param fraction: Mass-based or volume-based fraction for binary mixtures [%].
+        :param fraction: Mass-based or volume-based fraction for binary mixtures
+            [by default, %; you can change this using the configuration file].
         :raises ValueError: If fraction is invalid.
         """
+        super().__init__()
         if fraction is not None and (
             not name.fraction_min <= fraction <= name.fraction_max
         ):
             raise ValueError(
                 f"Invalid fraction value! It should be in "
                 f"[{'{0:g}'.format(name.fraction_min)};"
-                f"{'{0:g}'.format(name.fraction_max)}] %. "
-                f"Entered value = {'{0:g}'.format(fraction)} %."
+                f"{'{0:g}'.format(name.fraction_max)}]{self._fraction_unit}. "
+                f"Entered value = {'{0:g}'.format(fraction)}{self._fraction_unit}."
             )
         if fraction is None and not name.pure:
             raise ValueError("Need to define fraction!")
-        super().__init__()
         self.__name = name
-        self.__fraction = 100 if self.__name.pure else fraction
+        self.__fraction = (
+            (100 if self.units_system == UnitsSystem.SIWithCelsiusAndPercents else 1)
+            if self.__name.pure
+            else fraction
+        )
         self._backend = AbstractState(
             self.__name.coolprop_backend, self.__name.coolprop_name
         )
         if not self.__name.pure:
             self.__set_fraction()
 
     def factory(self) -> Fluid:
@@ -45,15 +51,18 @@
     @property
     def name(self) -> FluidsList:
         """Selected fluid name."""
         return self.__name
 
     @property
     def fraction(self) -> float:
-        """Mass-based or volume-based fraction for binary mixtures [%]."""
+        """
+        Mass-based or volume-based fraction for binary mixtures
+        [by default, %; you can change this using the configuration file].
+        """
         return self.__fraction
 
     def mixing(
         self,
         first_specific_mass_flow: float,
         first: AbstractFluid,
         second_specific_mass_flow: float,
@@ -63,17 +72,21 @@
             raise ValueError("The mixing process is possible only for the same fluids!")
         return super().mixing(
             first_specific_mass_flow, first, second_specific_mass_flow, second
         )
 
     def __set_fraction(self):
         if self.__name.mix_type == Mix.Mass:
-            self._backend.set_mass_fractions([self.__fraction * 1e-2])
+            self._backend.set_mass_fractions(
+                [self._unit_converter.convert_decimal_fraction_to_si(self.__fraction)]
+            )
         else:
-            self._backend.set_volu_fractions([self.__fraction * 1e-2])
+            self._backend.set_volu_fractions(
+                [self._unit_converter.convert_decimal_fraction_to_si(self.__fraction)]
+            )
 
     def __is_valid_fluids_for_mixing(
         self, first: AbstractFluid, second: AbstractFluid
     ) -> bool:
         return (
             isinstance(first, Fluid)
             and isinstance(second, Fluid)
@@ -86,8 +99,8 @@
     def __eq__(self, other: Fluid) -> bool:
         return isinstance(other, Fluid) and hash(self) == hash(other)
 
     def __ne__(self, other: Fluid) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
-        return hash((super().__hash__(), self.__name, self.__fraction))
+        return hash((self.__name.coolprop_name, self.__fraction, super().__hash__()))
```

### Comparing `pyfluids-2.3.2/pyfluids/fluids/mixture.py` & `pyfluids-2.4.0/pyfluids/fluids/mixture.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,101 @@
 from __future__ import annotations
 
 from CoolProp import AbstractState
 
 from .abstract_fluid import AbstractFluid
+from ..config import UnitsSystem
 from ..enums import FluidsList
 
 __all__ = ["Mixture"]
 
 
 class Mixture(AbstractFluid):
     """Mass-based mixture of pure fluids."""
 
+    __AVAILABLE_BACKEND = "HEOS"
+
     def __init__(self, fluids: list[FluidsList], fractions: list[float]):
         """
         Mass-based mixture of pure fluids.
 
         :param fluids: List of selected names of pure fluids.
-        :param fractions: List of mass-based fractions [%].
+        :param fractions: List of mass-based fractions
+            [by default, %; you can change this using the configuration file].
         :raises ValueError: If fluids or fractions are invalid.
         """
+        super().__init__()
         if len(fluids) != len(fractions):
             raise ValueError(
                 "Invalid input! Fluids and fractions should be of the same length."
             )
-        if not all(fluid.pure and fluid.coolprop_backend == "HEOS" for fluid in fluids):
+        if not all(
+            fluid.pure and fluid.coolprop_backend == self.__AVAILABLE_BACKEND
+            for fluid in fluids
+        ):
             raise ValueError(
                 "Invalid components! All of them should be "
-                "a pure fluid with HEOS backend."
+                f"a pure fluid with {self.__AVAILABLE_BACKEND} backend."
+            )
+        if not all(
+            0 < self._unit_converter.convert_decimal_fraction_to_si(fraction) < 1
+            for fraction in fractions
+        ):
+            fraction_range = (
+                "(0;100) %"
+                if self.units_system == UnitsSystem.SIWithCelsiusAndPercents
+                else "(0;1)"
             )
-        if not all(0 < fraction < 100 for fraction in fractions):
             raise ValueError(
-                "Invalid component mass fractions! All of them should be in (0;100) %."
+                "Invalid components mass fractions! "
+                f"All of them should be in {fraction_range}."
             )
-        if abs(sum(fractions) - 100) > 1e-6:
+        fractions_sum = (
+            100 if self.units_system == UnitsSystem.SIWithCelsiusAndPercents else 1
+        )
+        if abs(sum(fractions) - fractions_sum) > 1e-6:
             raise ValueError(
-                "Invalid component mass fractions! Their sum should be equal to 100 %."
+                "Invalid components mass fractions! "
+                f"Their sum should be equal to {fractions_sum}{self._fraction_unit}."
             )
-        super().__init__()
         self.__fluids, self.__fractions = fluids, fractions
         self._backend = AbstractState(
-            "HEOS", "&".join(fluid.coolprop_name for fluid in self.__fluids)
+            self.__AVAILABLE_BACKEND,
+            "&".join(fluid.coolprop_name for fluid in self.__fluids),
+        )
+        self._backend.set_mass_fractions(
+            [
+                self._unit_converter.convert_decimal_fraction_to_si(fraction)
+                for fraction in self.__fractions
+            ]
         )
-        self._backend.set_mass_fractions(self.__fractions)
 
     def factory(self) -> Mixture:
         return Mixture(self.__fluids, self.__fractions)
 
     @property
     def fluids(self) -> list[FluidsList]:
-        """List of selected pure fluids."""
+        """List of selected names of pure fluids."""
         return self.__fluids
 
     @property
     def fractions(self) -> list[float]:
-        """List of mass-based fractions [%]."""
+        """
+        List of mass-based fractions
+        [by default, %; you can change this using the configuration file].
+        """
         return self.__fractions
 
     def __eq__(self, other: Mixture) -> bool:
         return isinstance(other, Mixture) and hash(self) == hash(other)
 
     def __ne__(self, other: Mixture) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
-        return hash((super().__hash__(), *self.__fluids, *self.__fractions))
+        return hash(
+            (
+                "&".join(str(i.coolprop_name) for i in self.__fluids),
+                "&".join(str(i) for i in self.__fractions),
+                super().__hash__(),
+            )
+        )
```

### Comparing `pyfluids-2.3.2/pyfluids/humid_air/humid_air.py` & `pyfluids-2.4.0/pyfluids/humid_air/humid_air.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from __future__ import annotations
 
 import json
 
 from CoolProp.HumidAirProp import HAPropsSI
 
+from ..config import UnitConverter, UnitsSystem
 from ..io import InputHumidAir, OutputsValidator
 
 __all__ = ["HumidAir"]
 
 
 class HumidAir:
     """Real humid air (see ASHRAE RP-1485)."""
 
     def __init__(self):
         """Real humid air (see ASHRAE RP-1485)."""
         self._inputs: list[InputHumidAir] = []
         self.__compressibility: float | None = None
         self.__conductivity: float | None = None
-        self.__density: float | None = None
         self.__dew_temperature: float | None = None
         self.__dynamic_viscosity: float | None = None
         self.__enthalpy: float | None = None
         self.__entropy: float | None = None
         self.__humidity: float | None = None
         self.__partial_pressure: float | None = None
         self.__pressure: float | None = None
         self.__relative_humidity: float | None = None
         self.__specific_heat: float | None = None
+        self.__specific_volume: float | None = None
         self.__temperature: float | None = None
         self.__wet_bulb_temperature: float | None = None
+        self._unit_converter: UnitConverter = UnitConverter()
+
+    @property
+    def units_system(self) -> UnitsSystem:
+        """Configured units system."""
+        return self._unit_converter.units_system
 
     @property
     def compressibility(self) -> float:
         """Compressibility factor [-]."""
         if self.__compressibility is None:
             self.__compressibility = self._keyed_output("Z")
         return self.__compressibility
@@ -43,23 +50,26 @@
         if self.__conductivity is None:
             self.__conductivity = self._keyed_output("K")
         return self.__conductivity
 
     @property
     def density(self) -> float:
         """Mass density per humid air unit [kg/m3]."""
-        if self.__density is None:
-            self.__density = 1 / self._keyed_output("Vha")
-        return self.__density
+        return 1 / self.specific_volume
 
     @property
     def dew_temperature(self) -> float:
-        """Dew-point temperature [°C]."""
+        """
+        Dew-point temperature
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__dew_temperature is None:
-            self.__dew_temperature = self._keyed_output("D") - 273.15
+            self.__dew_temperature = self._unit_converter.convert_temperature_from_si(
+                self._keyed_output("D")
+            )
         return self.__dew_temperature
 
     @property
     def dynamic_viscosity(self) -> float:
         """Dynamic viscosity [Pa*s]."""
         if self.__dynamic_viscosity is None:
             self.__dynamic_viscosity = self._keyed_output("M")
@@ -108,38 +118,64 @@
         """Absolute pressure [Pa]."""
         if self.__pressure is None:
             self.__pressure = self._keyed_output("P")
         return self.__pressure
 
     @property
     def relative_humidity(self) -> float:
-        """Relative humidity ratio [%]."""
+        """
+        Relative humidity ratio
+        [by default, %; you can change this using the configuration file].
+        """
         if self.__relative_humidity is None:
-            self.__relative_humidity = self._keyed_output("R") * 1e2
+            self.__relative_humidity = (
+                self._unit_converter.convert_decimal_fraction_from_si(
+                    self._keyed_output("R")
+                )
+            )
         return self.__relative_humidity
 
     @property
     def specific_heat(self) -> float:
         """Mass specific constant pressure specific heat per humid air [J/kg/K]."""
         if self.__specific_heat is None:
             self.__specific_heat = self._keyed_output("Cha")
         return self.__specific_heat
 
     @property
+    def specific_volume(self) -> float:
+        """Mass specific volume per humid air unit [m3/kg]."""
+        if self.__specific_volume is None:
+            self.__specific_volume = self._keyed_output("Vha")
+        return self.__specific_volume
+
+    @property
     def temperature(self) -> float:
-        """Dry-bulb temperature [°C]."""
+        """
+        Dry-bulb temperature
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__temperature is None:
-            self.__temperature = self._keyed_output("T") - 273.15
+            self.__temperature = self._unit_converter.convert_temperature_from_si(
+                self._keyed_output("T")
+            )
         return self.__temperature
 
     @property
     def wet_bulb_temperature(self) -> float:
-        """Wet-bulb temperature [°C]."""
+        """
+        Wet-bulb temperature
+        [by default, °C; you can change this using the configuration file].
+        """
         if self.__wet_bulb_temperature is None:
-            self.__wet_bulb_temperature = self._keyed_output("B") - 273.15
+            self.__wet_bulb_temperature = (
+                self._unit_converter.convert_temperature_from_si(
+                    self._keyed_output("B")
+                )
+            )
         return self.__wet_bulb_temperature
 
     def factory(self) -> HumidAir:
         """Returns a new humid air instance with no defined state."""
         return HumidAir()
 
     def clone(self) -> HumidAir:
@@ -176,42 +212,44 @@
 
         :param first_input: First input property.
         :param second_input: Second input property.
         :param third_input: Third input property.
         :raises ValueError: If input is invalid.
         """
         self.reset()
-        self._inputs = (first_input, second_input, third_input)
+        self._inputs = [first_input, second_input, third_input]
         self.__check_inputs()
 
     # noinspection DuplicatedCode
     def reset(self):
         """Resets all properties."""
+        self._inputs.clear()
         self.__compressibility = None
         self.__conductivity = None
-        self.__density = None
         self.__dew_temperature = None
         self.__dynamic_viscosity = None
         self.__enthalpy = None
         self.__entropy = None
         self.__humidity = None
         self.__partial_pressure = None
         self.__pressure = None
         self.__relative_humidity = None
         self.__specific_heat = None
+        self.__specific_volume = None
         self.__temperature = None
         self.__wet_bulb_temperature = None
 
     def dry_cooling_to_temperature(
         self, temperature: float, pressure_drop: float = 0
     ) -> HumidAir:
         """
         The process of cooling without dehumidification to a given temperature.
 
-        :param temperature: Temperature [°C].
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
         :param pressure_drop: Pressure drop in the heat exchanger (optional) [Pa].
         :return: The state of the humid air at the end of the process.
         :raises ValueError: If temperature or pressure drop is invalid.
         """
         return self.__dry_heat_transfer_to_temperature(temperature, True, pressure_drop)
 
     def dry_cooling_to_enthalpy(
@@ -230,16 +268,18 @@
     def wet_cooling_to_temperature_and_relative_humidity(
         self, temperature: float, relative_humidity: float, pressure_drop: float = 0
     ) -> HumidAir:
         """
         The process of cooling with dehumidification
         to a given temperature and relative humidity ratio.
 
-        :param temperature: Temperature [°C].
-        :param relative_humidity: Relative humidity ratio [%].
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
+        :param relative_humidity: Relative humidity ratio
+            [by default, %; you can change this using the configuration file].
         :param pressure_drop: Pressure drop in the heat exchanger (optional) [Pa].
         :return: The state of the humid air at the end of the process.
         :raises ValueError: If temperature, relative humidity ratio or
             pressure drop is invalid.
         """
         return self.__wet_cooling_to(
             InputHumidAir.temperature(temperature),
@@ -250,15 +290,16 @@
     def wet_cooling_to_temperature_and_absolute_humidity(
         self, temperature: float, humidity: float, pressure_drop: float = 0
     ) -> HumidAir:
         """
         The process of cooling with dehumidification
         to a given temperature and absolute humidity ratio.
 
-        :param temperature: Temperature [°C].
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
         :param humidity: Absolute humidity ratio [kg/kg d.a.].
         :param pressure_drop: Pressure drop in the heat exchanger (optional) [Pa].
         :return: The state of the humid air at the end of the process.
         :raises ValueError: If temperature, absolute humidity ratio or
             pressure drop is invalid.
         """
         return self.__wet_cooling_to(
@@ -271,15 +312,16 @@
         self, enthalpy: float, relative_humidity: float, pressure_drop: float = 0
     ) -> HumidAir:
         """
         The process of cooling with dehumidification
         to a given enthalpy and relative humidity ratio.
 
         :param enthalpy: Enthalpy [J/kg].
-        :param relative_humidity: Relative humidity ratio [%].
+        :param relative_humidity: Relative humidity ratio
+            [by default, %; you can change this using the configuration file].
         :param pressure_drop: Pressure drop in the heat exchanger (optional) [Pa].
         :return: The state of the humid air at the end of the process.
         :raises ValueError: If enthalpy, relative humidity ratio or
             pressure drop is invalid.
         """
         return self.__wet_cooling_to(
             InputHumidAir.enthalpy(enthalpy),
@@ -309,15 +351,16 @@
 
     def heating_to_temperature(
         self, temperature: float, pressure_drop: float = 0
     ) -> HumidAir:
         """
         The process of heating to a given temperature.
 
-        :param temperature: Temperature [°C].
+        :param temperature: Temperature
+            [by default, °C; you can change this using the configuration file].
         :param pressure_drop: Pressure drop in the heat exchanger (optional) [Pa].
         :return: The state of the humid air at the end of the process.
         :raises ValueError: If temperature or pressure drop is invalid.
         """
         return self.__dry_heat_transfer_to_temperature(
             temperature, False, pressure_drop
         )
@@ -338,15 +381,16 @@
     def humidification_by_water_to_relative_humidity(
         self, relative_humidity: float
     ) -> HumidAir:
         """
         The process of humidification by water (isenthalpic)
         to a given relative humidity ratio.
 
-        :param relative_humidity: Relative humidity ratio [%].
+        :param relative_humidity: Relative humidity ratio
+            [by default, %; you can change this using the configuration file].
         :return: The state of the humid air at the end of the process.
         :raises ValueError: If relative humidity ratio is invalid.
         """
         return self.__humidification_to(
             InputHumidAir.enthalpy(self.enthalpy),
             InputHumidAir.relative_humidity(relative_humidity),
         )
@@ -368,15 +412,16 @@
     def humidification_by_steam_to_relative_humidity(
         self, relative_humidity: float
     ) -> HumidAir:
         """
         The process of humidification by steam (isothermal)
         to a given relative humidity ratio.
 
-        :param relative_humidity: Relative humidity ratio [%].
+        :param relative_humidity: Relative humidity ratio
+            [by default, %; you can change this using the configuration file].
         :return: The state of the humid air at the end of the process.
         :raises ValueError: If relative humidity ratio is invalid.
         """
         return self.__humidification_to(
             InputHumidAir.temperature(self.temperature),
             InputHumidAir.relative_humidity(relative_humidity),
         )
@@ -445,19 +490,21 @@
         """
         return json.dumps(
             self.as_dict(), indent=4 if indented else None, default=str, sort_keys=False
         )
 
     def as_dict(self) -> dict[str, float]:
         """Converts the humid air to a dict."""
-        return {
-            self.__select(key): getattr(self, self.__select(key))
-            for key, value in vars(self).items()
-            if not self.__select(key).startswith("_")
-        }
+        keys = [
+            key
+            for key in dir(self.__class__)
+            if isinstance(getattr(self.__class__, key), property)
+        ]
+        values = [getattr(self, key) for key in keys]
+        return {key: value for key, value in zip(keys, values)}
 
     def _keyed_output(self, coolprop_key: str) -> float:
         self.__check_inputs()
         cached_input = next(
             (i for i in self._inputs if i.coolprop_key == coolprop_key), None
         )
         value = (
@@ -481,16 +528,16 @@
 
     def __ne__(self, other: HumidAir) -> bool:
         return not self.__eq__(other)
 
     def __hash__(self) -> int:
         return hash(
             (
-                sum(i.value for i in self._inputs),
-                "&".join(i.coolprop_key for i in self._inputs),
+                "&".join(str(i.value) for i in self._inputs),
+                "&".join(str(i.coolprop_key) for i in self._inputs),
             )
         )
 
     def __check_inputs(self):
         unique_keys = set([i.coolprop_key for i in self._inputs])
         if len(self._inputs) != 3 or len(unique_keys) != 3:
             raise ValueError("Need to define 3 unique inputs!")
@@ -522,15 +569,18 @@
     def __wet_cooling_to(
         self,
         first_input: InputHumidAir,
         second_input: InputHumidAir,
         pressure_drop: float = 0,
     ):
         if first_input.coolprop_key == "T":
-            self.__check_temperature(first_input.value - 273.15, True)
+            self.__check_temperature(
+                self._unit_converter.convert_temperature_from_si(first_input.value),
+                True,
+            )
         if first_input.coolprop_key == "Hha":
             self.__check_enthalpy(first_input.value, True)
         self.__check_pressure_drop(pressure_drop)
         result = self.with_state(
             InputHumidAir.pressure(self.pressure - pressure_drop),
             first_input,
             second_input,
@@ -584,23 +634,23 @@
 
     def __check_dew_enthalpy(self, enthalpy: float):
         if (
             enthalpy
             < self.with_state(
                 InputHumidAir.pressure(self.pressure),
                 InputHumidAir.temperature(self.dew_temperature),
-                InputHumidAir.relative_humidity(100),
+                InputHumidAir.relative_humidity(
+                    100
+                    if self.units_system == UnitsSystem.SIWithCelsiusAndPercents
+                    else 1
+                ),
             ).enthalpy
         ):
             raise ValueError(
                 "The outlet enthalpy after dry heat transfer "
                 "should be greater than the dew point enthalpy!"
             )
 
     @staticmethod
     def __check_pressure_drop(pressure_drop: float):
         if pressure_drop < 0:
             raise ValueError("Invalid pressure drop in the heat exchanger!")
-
-    @staticmethod
-    def __select(key: str) -> str:
-        return key.split("__")[-1]
```

### Comparing `pyfluids-2.3.2/pyfluids/io/abstract_input.py` & `pyfluids-2.4.0/pyfluids/io/abstract_input.py`

 * *Files identical despite different names*

### Comparing `pyfluids-2.3.2/pyfluids/io/input.py` & `pyfluids-2.4.0/pyfluids/io/input.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import CoolProp
 
 from .abstract_input import AbstractInput
+from ..config import UnitConverter
 
 __all__ = ["Input"]
 
 
 class Input(AbstractInput):
     """CoolProp keyed input for fluids and mixtures."""
 
@@ -70,21 +71,33 @@
         return cls(CoolProp.iP, value)
 
     @classmethod
     def quality(cls, value: float) -> Input:
         """
         Mass vapor quality.
 
-        :param value: The value of the input [%].
+        :param value: The value of the input
+            [by default, %; you can change this using the configuration file].
         :return: Mass vapor quality for the input.
         """
-        return cls(CoolProp.iQ, value * 1e-2)
+        return cls(CoolProp.iQ, UnitConverter().convert_decimal_fraction_to_si(value))
+
+    @classmethod
+    def specific_volume(cls, value: float) -> Input:
+        """
+        Mass specific volume.
+
+        :param value: The value of the input [m3/kg].
+        :return: Mass specific volume for the input.
+        """
+        return cls(CoolProp.iDmass, 1 / value)
 
     @classmethod
     def temperature(cls, value: float) -> Input:
         """
         Temperature.
 
-        :param value: The value of the input [°C].
+        :param value: The value of the input
+            [by default, °C; you can change this using the configuration file].
         :return: Temperature for the input.
         """
-        return cls(CoolProp.iT, value + 273.15)
+        return cls(CoolProp.iT, UnitConverter().convert_temperature_to_si(value))
```

### Comparing `pyfluids-2.3.2/pyfluids/io/input_humid_air.py` & `pyfluids-2.4.0/pyfluids/io/input_humid_air.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from .abstract_input import AbstractInput
+from ..config import UnitConverter
 
 __all__ = ["InputHumidAir"]
 
 
 class InputHumidAir(AbstractInput):
     """CoolProp keyed input for humid air."""
 
@@ -47,18 +48,19 @@
         return cls("Vha", 1 / value)
 
     @classmethod
     def dew_temperature(cls, value: float) -> InputHumidAir:
         """
         Dew-point temperature.
 
-        :param value: The value of the input [°C].
+        :param value: The value of the input
+            [by default, °C; you can change this using the configuration file].
         :return: Dew-point temperature for the input.
         """
-        return cls("D", value + 273.15)
+        return cls("D", UnitConverter().convert_temperature_to_si(value))
 
     @classmethod
     def enthalpy(cls, value: float) -> InputHumidAir:
         """
         Mass specific enthalpy per humid air.
 
         :param value: The value of the input [J/kg].
@@ -107,31 +109,44 @@
         return cls("P", value)
 
     @classmethod
     def relative_humidity(cls, value: float) -> InputHumidAir:
         """
         Relative humidity.
 
-        :param value: The value of the input [%].
+        :param value: The value of the input
+            [by default, %; you can change this using the configuration file].
         :return: Relative humidity for the input.
         """
-        return cls("R", value * 1e-2)
+        return cls("R", UnitConverter().convert_decimal_fraction_to_si(value))
+
+    @classmethod
+    def specific_volume(cls, value: float) -> InputHumidAir:
+        """
+        Mass specific volume per humid air unit.
+
+        :param value: The value of the input [m3/kg].
+        :return: Mass specific volume per humid air unit for the input.
+        """
+        return cls("Vha", value)
 
     @classmethod
     def temperature(cls, value: float) -> InputHumidAir:
         """
         Temperature.
 
-        :param value: The value of the input [°C].
+        :param value: The value of the input
+            [by default, °C; you can change this using the configuration file].
         :return: Temperature for the input.
         """
-        return cls("T", value + 273.15)
+        return cls("T", UnitConverter().convert_temperature_to_si(value))
 
     @classmethod
     def wet_bulb_temperature(cls, value: float) -> InputHumidAir:
         """
         Wet-bulb temperature.
 
-        :param value: The value of the input [°C].
+        :param value: The value of the input
+            [by default, °C; you can change this using the configuration file].
         :return: Wet-bulb temperature for the input.
         """
-        return cls("B", value + 273.15)
+        return cls("B", UnitConverter().convert_temperature_to_si(value))
```

### Comparing `pyfluids-2.3.2/pyproject.toml` & `pyfluids-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfluids"
-version = "2.3.2"
+version = "2.4.0"
 description = "A simple, full-featured, lightweight CoolProp wrapper for Python"
 authors = [
     "Vladimir Portyanikhin <v.portyanikhin@ya.ru>",
 ]
 license = "MIT"
 readme = "PyPI.md"
 homepage = "https://github.com/portyanikhin/PyFluids"
@@ -51,16 +51,17 @@
 packages = [
     { include = "pyfluids" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7, <3.12"
 CoolProp = "6.4.3.post1"
+tomli = "2.0.1"
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.2.0"
-pytest-asyncio = "0.20.3"
-pytest-cov = "4.0.0"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyfluids-2.3.2/PKG-INFO` & `pyfluids-2.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfluids
-Version: 2.3.2
+Version: 2.4.0
 Summary: A simple, full-featured, lightweight CoolProp wrapper for Python
 Home-page: https://github.com/portyanikhin/PyFluids
 License: MIT
 Keywords: CoolProp,fluids,mixtures,humid,air,thermophysical,properties,thermodynamics
 Author: Vladimir Portyanikhin
 Author-email: v.portyanikhin@ya.ru
 Requires-Python: >=3.7,<3.12
@@ -22,29 +22,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: CoolProp (==6.4.3.post1)
+Requires-Dist: tomli (==2.0.1)
 Project-URL: Documentation, https://github.com/portyanikhin/PyFluids
 Project-URL: Repository, https://github.com/portyanikhin/PyFluids
 Description-Content-Type: text/markdown
 
 # ![PyFluids](https://raw.githubusercontent.com/portyanikhin/PyFluids/main/pictures/header.png)
 
 [![Build & Tests](https://github.com/portyanikhin/PyFluids/actions/workflows/build-tests.yml/badge.svg)](https://github.com/portyanikhin/PyFluids/actions/workflows/build-tests.yml)
```

