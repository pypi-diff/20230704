# Comparing `tmp/openoligo-0.1.5.tar.gz` & `tmp/openoligo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openoligo-0.1.5.tar", max compression
+gzip compressed data, was "openoligo-0.1.6.tar", max compression
```

## Comparing `openoligo-0.1.5.tar` & `openoligo-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-06-30 17:13:35.712827 openoligo-0.1.5/LICENSE
--rw-r--r--   0        0        0     1099 2023-06-30 17:13:35.712827 openoligo-0.1.5/README.md
--rw-r--r--   0        0        0      433 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/__init__.py
--rw-r--r--   0        0        0      587 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/__init__.py
--rw-r--r--   0        0        0     3978 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/board.py
--rw-r--r--   0        0        0     3564 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/devices.py
--rw-r--r--   0        0        0     3414 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/gpio.py
--rw-r--r--   0        0        0     2235 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/platform.py
--rw-r--r--   0        0        0     3871 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/hal/types.py
--rw-r--r--   0        0        0     4196 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/instrument.py
--rw-r--r--   0        0        0      912 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/log_config.py
--rw-r--r--   0        0        0       52 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/protocols/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/protocols/dna_synthesis.py
--rw-r--r--   0        0        0     1460 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/seq.py
--rw-r--r--   0        0        0      157 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/steps/__init__.py
--rw-r--r--   0        0        0     2341 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/steps/flow.py
--rw-r--r--   0        0        0     1292 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/steps/types.py
--rw-r--r--   0        0        0      237 2023-06-30 17:13:35.716827 openoligo-0.1.5/openoligo/utils/__init__.py
--rw-r--r--   0        0        0      537 2023-06-30 17:13:35.720828 openoligo-0.1.5/openoligo/utils/sim.py
--rw-r--r--   0        0        0      402 2023-06-30 17:13:35.720828 openoligo-0.1.5/openoligo/utils/singleton.py
--rw-r--r--   0        0        0      839 2023-06-30 17:13:35.720828 openoligo-0.1.5/openoligo/utils/wait.py
--rw-r--r--   0        0        0     1373 2023-06-30 17:13:35.720828 openoligo-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 openoligo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-04 18:43:58.136917 openoligo-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1306 2023-07-04 18:43:58.136917 openoligo-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/api/__init__.py
+-rw-r--r--   0        0        0      749 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/api/db.py
+-rw-r--r--   0        0        0     1505 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/api/helpers.py
+-rw-r--r--   0        0        0     2456 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/api/models.py
+-rw-r--r--   0        0        0      678 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/hal/__init__.py
+-rw-r--r--   0        0        0     4193 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/hal/board.py
+-rw-r--r--   0        0        0     4707 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/hal/devices.py
+-rw-r--r--   0        0        0     5121 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/hal/gpio.py
+-rw-r--r--   0        0        0     4196 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/hal/instrument.py
+-rw-r--r--   0        0        0     2235 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/hal/platform.py
+-rw-r--r--   0        0        0     3961 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/hal/types.py
+-rw-r--r--   0        0        0       52 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/protocols/__init__.py
+-rw-r--r--   0        0        0     3131 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/protocols/dna_synthesis.py
+-rw-r--r--   0        0        0     1637 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/seq.py
+-rw-r--r--   0        0        0      157 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/steps/__init__.py
+-rw-r--r--   0        0        0     2356 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/steps/flow.py
+-rw-r--r--   0        0        0     1292 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/steps/types.py
+-rw-r--r--   0        0        0      237 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/utils/__init__.py
+-rw-r--r--   0        0        0     3871 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/utils/logger.py
+-rw-r--r--   0        0        0      537 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/utils/sim.py
+-rw-r--r--   0        0        0      402 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/utils/singleton.py
+-rw-r--r--   0        0        0      839 2023-07-04 18:43:58.140917 openoligo-0.1.6/openoligo/utils/wait.py
+-rw-r--r--   0        0        0     1534 2023-07-04 18:43:58.140917 openoligo-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 openoligo-0.1.6/PKG-INFO
```

### Comparing `openoligo-0.1.5/LICENSE` & `openoligo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.5/README.md` & `openoligo-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,13 @@
 inst = Instrument()
 
 try:
     asyncio.run(synthesize(inst, Seq("ATCGAAATTTTT")))
 except KeyboardInterrupt:
     print("Keyboard interrupt received, exiting...")
 ```
+
+## Firmware
+The firmware for OpenOligo is composed of 
+- OpenOligo Library
+- API server (part of OpenOligo Library)
+- In a minimal linux image ([OligoOS](https://github.com/Technoculture/OligoOs/tree/dev))
```

### Comparing `openoligo-0.1.5/openoligo/hal/board.py` & `openoligo-0.1.6/openoligo/hal/board.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Pins in the Raspberry Pi GPIO header.
 """
 from typing import Dict, TypedDict
 
-from openoligo.hal.devices import Switch, Valve
+from openoligo.hal.devices import DigitalSensor, Switch, Valve
 from openoligo.hal.types import Board, NoSuchPinInPinout, Switchable, ValveRole, board
 from openoligo.utils.singleton import Singleton
 
 
 # Initialize fixed pinout
 class FixedPinoutDict(TypedDict):
     """
@@ -19,26 +19,30 @@
     prod: Valve
     branch: Valve
     rxn_out: Valve
     sol: Valve
     gas: Valve
     valve_pressure: Switch
     gas_pressure: Switch
+    valve_regulator_err: DigitalSensor
+    flow_regulator_err: DigitalSensor
 
 
 fixed_pinout: FixedPinoutDict = {
     "waste": Valve(gpio_pin=board.P7, role=ValveRole.OUTLET),
     "waste_rxn": Valve(gpio_pin=board.P5, role=ValveRole.OUTLET),
     "prod": Valve(gpio_pin=board.P8, role=ValveRole.OUTLET),
     "branch": Valve(gpio_pin=board.P12, role=ValveRole.BRANCH),
     "rxn_out": Valve(gpio_pin=board.P13, role=ValveRole.TRANSIT),
     "sol": Valve(gpio_pin=board.P3),
     "gas": Valve(gpio_pin=board.P10),
     "valve_pressure": Switch(gpio_pin=board.P11),
     "gas_pressure": Switch(gpio_pin=board.P29),
+    "valve_regulator_err": DigitalSensor(gpio_pin=board.P31),
+    "flow_regulator_err": DigitalSensor(gpio_pin=board.P33),
 }
 
 
 def list_configurable_pins() -> dict[str, Board]:
     """
     Returns a list of all configurable pins.
     These ar all pins in the board that are not part of the fiixed pinout.
```

### Comparing `openoligo-0.1.5/openoligo/hal/devices.py` & `openoligo-0.1.6/openoligo/hal/devices.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Switches can be used to control devices that can be turned on and off.
 """
 import logging
 from dataclasses import dataclass, field
 
-from openoligo.hal.gpio import get_gpio
+from openoligo.hal.gpio import GpioMode, get_gpio
 from openoligo.hal.types import Switchable, Valvable, ValveRole, ValveState, ValveType
 
 
 @dataclass
 class Switch(Switchable):
     """
     A switch that actually controls a GPIO pin on the Raspberry Pi.
@@ -54,14 +54,46 @@
         self.set(not self._state)
 
     @property
     def value(self) -> bool:
         """
         Get the current value of the switch.
         """
+        self._state = self.controller.value(self.gpio_pin)
+        return self._state
+
+
+@dataclass
+class DigitalSensor(Switchable):
+    """
+    A digital sensor that actually controls a GPIO pin on the Raspberry Pi.
+    """
+
+    gpio_pin: str
+    _state: bool = field(default=False, init=False)
+
+    def __post_init__(self):
+        """Initialize the switch."""
+        self.controller = get_gpio()
+        self.controller.setup_pin(self.gpio_pin, GpioMode.IN)
+
+    def set(self, _: bool):
+        """A digital sensor cannot be set"""
+        raise NotImplementedError
+
+    def toggle(self):
+        """A digital sensor cannot be toggled"""
+        raise NotImplementedError
+
+    @property
+    def value(self) -> bool:
+        """
+        Get the current value of the switch.
+        """
+        self._state = self.controller.value(self.gpio_pin)
         return self._state
 
 
 @dataclass
 class Valve(Valvable):
     """
     A valve that actually controls a GPIO pin on the Raspberry Pi.
@@ -113,14 +145,19 @@
             self._state,
             extra={"markup": True},
         )
 
     @property
     def value(self) -> bool:
         """Get the current value of the valve."""
+        val = self.controller.value(self.gpio_pin)
+        if self.valve_type == ValveType.NORMALLY_CLOSED:
+            self._state = ValveState.OPEN_FLOW if val else ValveState.CLOSED_FLOW
+        else:
+            self._state = ValveState.CLOSED_FLOW if val else ValveState.OPEN_FLOW
         return self._state == ValveState.OPEN_FLOW
 
     @property
     def get_type(self) -> ValveType:
         """Get the type of the valve."""
         return self.valve_type
```

### Comparing `openoligo-0.1.5/openoligo/hal/platform.py` & `openoligo-0.1.6/openoligo/hal/platform.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.5/openoligo/hal/types.py` & `openoligo-0.1.6/openoligo/hal/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,22 @@
 class GpioMode(Enum):
     """GPIO mode."""
 
     IN = 0
     OUT = 1
 
 
+class GpioEdge(Enum):
+    """GPIO edge."""
+
+    RISING = 0
+    FALLING = 1
+    BOTH = 2
+
+
 class ValveState(Enum):
     """This class represents the state of a valve."""
 
     OPEN_FLOW = 0
     CLOSED_FLOW = 1
```

### Comparing `openoligo-0.1.5/openoligo/instrument.py` & `openoligo-0.1.6/openoligo/hal/instrument.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.5/openoligo/protocols/dna_synthesis.py` & `openoligo-0.1.6/openoligo/protocols/dna_synthesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import logging
 from time import time
 
 from tqdm import tqdm
 
 from openoligo import utils
-from openoligo.instrument import Instrument
+from openoligo.hal.instrument import Instrument
 from openoligo.seq import Seq
 from openoligo.steps.flow import dry_all, send_to_waste_rxn, solvent_wash_all
 from openoligo.steps.types import step
 from openoligo.utils import wait_async
 
 
 @step
```

### Comparing `openoligo-0.1.5/openoligo/seq.py` & `openoligo-0.1.6/openoligo/seq.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Sequence class for DNA, RNA and modified Nucleic Acid sequences.
 """
 import re
+from enum import Enum
 
 
 def is_valid_dna(sequence):
     """
     Check if a sequence is a valid DNA sequence.
     """
     pattern = r"^[ATCGatcg]*$"
@@ -60,7 +61,17 @@
         return len(self.seq)
 
     def __getitem__(self, key) -> str:
         """
         Allows indexing of the sequence.
         """
         return self.seq[key]
+
+
+class SeqCategory(str, Enum):
+    """
+    Enum for the different sequence categories.
+    """
+
+    DNA = "DNA"
+    RNA = "RNA"
+    MODIFIED = "MODIFIED"
```

### Comparing `openoligo-0.1.5/openoligo/steps/flow.py` & `openoligo-0.1.6/openoligo/steps/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions to create various flows from reagents to columns,
 and to clean columns.
 """
 import logging
 
-from openoligo import Instrument
+from openoligo.hal.instrument import Instrument
 from openoligo.steps.types import FlowBranch, substep
 from openoligo.utils.wait import wait_async
 
 
 @substep
 async def send_to_prod(instrument: Instrument, src: str) -> None:
     """
```

### Comparing `openoligo-0.1.5/openoligo/steps/types.py` & `openoligo-0.1.6/openoligo/steps/types.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.5/openoligo/utils/sim.py` & `openoligo-0.1.6/openoligo/utils/sim.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.5/openoligo/utils/wait.py` & `openoligo-0.1.6/openoligo/utils/wait.py`

 * *Files identical despite different names*

### Comparing `openoligo-0.1.5/pyproject.toml` & `openoligo-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 [tool.poetry]
 name = "OpenOligo"
-version = "0.1.5"
+version = "0.1.6"
 description = "An open-source platform for programmatically interacting with and managing Nucleic acid sequences synthesis processes."
 license = "Apache-2.0"
 authors = ["Satyam Tiwary <satyam@technoculture.io>"]
 readme = "README.md"
 keywords = ["DNA", "synthesis", "genetics", "open-source"]
 
 [tool.poetry.scripts]
-oligo-server = 'app.server:main'
-oligo-synth = 'examples.dna_synthesis:main'
+oligo-server = 'scripts.server:main'
+oligo-runner = 'scripts.runner:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^13.4.2"
 python-dotenv = "^1.0.0"
 tqdm = "^4.65.0"
 fastapi = "^0.98.0"
 pdocs = "^1.2.0"
+uvicorn = "^0.22.0"
 "RPi.GPIO" = { version = "^0.7.1", optional = true }
 Adafruit_BBIO = { version = "^1.2.0", optional = true }
+aerich = "^0.7.1"
+types-tqdm = "^4.65.0.1"
+tortoise-orm = "^0.18.1"
+httpx = "^0.24.1"
+sh = "^2.0.4"
+anyio = "^3.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
+pytest-asyncio = "^0.21.0"
 flake8 = "^3.9.2"
 black = "^23.3.0"
 pylint = "^2.17.4"
 mypy = "^1.3.0"
 isort = "^5.12.0"
 coverage-badge = "^1.1.0"
 jupyter = "^1.0.0"
@@ -41,15 +49,15 @@
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 line-length = 100
 
 [tool.pytest.ini_options]
-addopts = "--cov=openoligo --cov-config=pyproject.toml --cov-report=term-missing --cov-fail-under=90"
+addopts = "--cov=openoligo --cov-config=pyproject.toml --cov-report=term-missing --cov-fail-under=70"
 
 [tool.coverage.run]
 source = ["openoligo"]
 #omit = ["**/types.py"]
 
 [tool.poetry.extras]
 rpi = ["RPi.GPIO"]
```

