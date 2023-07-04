# Comparing `tmp/crypto-screening-1.8.3.tar.gz` & `tmp/crypto-screening-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.8.3.tar", last modified: Mon Jul  3 15:19:07 2023, max compression
+gzip compressed data, was "crypto-screening-1.9.0.tar", last modified: Tue Jul  4 21:38:57 2023, max compression
```

## Comparing `crypto-screening-1.8.3.tar` & `crypto-screening-1.9.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:19:07.015333 crypto-screening-1.8.3/
--rw-rw-rw-   0        0        0       98 2023-07-03 15:19:06.000000 crypto-screening-1.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-03 15:19:07.015333 crypto-screening-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.8.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.8.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:19:06.994340 crypto-screening-1.8.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-03 15:19:07.006321 crypto-screening-1.8.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.8.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.8.3/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    10119 2023-06-30 15:31:03.000000 crypto-screening-1.8.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18830 2023-07-03 15:11:08.000000 crypto-screening-1.8.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.8.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.8.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.8.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:19:07.007322 crypto-screening-1.8.3/crypto_screening/market/
-drwxrwxrwx   0        0        0        0 2023-07-03 15:19:07.009313 crypto-screening-1.8.3/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10820 2023-07-03 15:11:30.000000 crypto-screening-1.8.3/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      889 2023-06-30 09:21:25.000000 crypto-screening-1.8.3/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     7992 2023-07-03 15:11:53.000000 crypto-screening-1.8.3/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:19:07.013337 crypto-screening-1.8.3/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.8.3/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13672 2023-07-03 15:14:43.000000 crypto-screening-1.8.3/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.8.3/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32777 2023-07-03 15:13:54.000000 crypto-screening-1.8.3/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24986 2023-07-03 15:14:04.000000 crypto-screening-1.8.3/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.8.3/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.8.3/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.8.3/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.8.3/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.8.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:19:07.003345 crypto-screening-1.8.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-03 15:19:06.000000 crypto-screening-1.8.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2023-07-03 15:19:06.000000 crypto-screening-1.8.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 15:19:06.000000 crypto-screening-1.8.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-03 15:19:06.000000 crypto-screening-1.8.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-03 15:19:06.000000 crypto-screening-1.8.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-03 15:19:06.000000 crypto-screening-1.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.8.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.8.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 15:19:07.015333 crypto-screening-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-03 15:18:47.000000 crypto-screening-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.631830 crypto-screening-1.9.0/
+-rw-rw-rw-   0        0        0       98 2023-07-04 21:38:55.000000 crypto-screening-1.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-04 21:38:57.631830 crypto-screening-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-1.9.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.9.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.566414 crypto-screening-1.9.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.604860 crypto-screening-1.9.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-1.9.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-1.9.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0     8905 2023-07-04 21:38:35.000000 crypto-screening-1.9.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    10119 2023-06-30 15:31:03.000000 crypto-screening-1.9.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18830 2023-07-03 15:11:08.000000 crypto-screening-1.9.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-1.9.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.9.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5278 2023-07-03 15:17:16.000000 crypto-screening-1.9.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.609863 crypto-screening-1.9.0/crypto_screening/market/
+drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.612830 crypto-screening-1.9.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1352 2023-07-04 21:19:28.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-1.9.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.630866 crypto-screening-1.9.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-1.9.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-1.9.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-1.9.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9969 2023-07-03 15:16:52.000000 crypto-screening-1.9.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-1.9.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-04 21:38:57.582860 crypto-screening-1.9.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-04 21:38:57.000000 crypto-screening-1.9.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-04 21:38:55.000000 crypto-screening-1.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       99 2023-06-28 09:56:21.000000 crypto-screening-1.9.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 21:38:57.631830 crypto-screening-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-04 21:38:51.000000 crypto-screening-1.9.0/setup.py
```

### Comparing `crypto-screening-1.8.3/PKG-INFO` & `crypto-screening-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.8.3
+Version: 1.9.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.8.3/README.md` & `crypto-screening-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/build.py` & `crypto-screening-1.9.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/collect/assets.py` & `crypto-screening-1.9.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/collect/exchanges.py` & `crypto-screening-1.9.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/collect/screeners.py` & `crypto-screening-1.9.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/collect/symbols.py` & `crypto-screening-1.9.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/dataset.py` & `crypto-screening-1.9.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/interval.py` & `crypto-screening-1.9.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/market/foundation/data.py` & `crypto-screening-1.9.0/crypto_screening/market/foundation/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 from abc import ABCMeta, abstractmethod
 import threading
 from typing import Optional, Union, Dict, Any
 
 from represent import represent, Modifiers
 
 
-from crypto_screening.market.foundation.waiting import WaitingState
-from crypto_screening.market.foundation.protocols import DataCollectorProtocol
+from crypto_screening.market.foundation.state import WaitingState
 
 __all__ = [
     "DataCollector"
 ]
 
 @represent
-class DataCollector(DataCollectorProtocol, metaclass=ABCMeta):
+class DataCollector(metaclass=ABCMeta):
     """A class to represent an abstract parent class of data collectors."""
 
     __modifiers__ = Modifiers()
     __modifiers__.excluded.extend(
         [
             'screening_process', 'timeout_process',
             'saving_process', 'update_process'
         ]
     )
 
     __slots__ = (
         '_screening_process', '_timeout_process',
         '_saving_process', '_update_process',
-        'location', 'cancel', 'delay', 'market'
+        '_updating', '_saving', '_blocking',
+        '_screening', "location", "delay", "cancel"
     )
 
     LOCATION = "datasets"
 
     DELAY = 0.0
     CANCEL = 0
```

### Comparing `crypto-screening-1.8.3/crypto_screening/market/foundation/protocols.py` & `crypto-screening-1.9.0/crypto_screening/market/foundation/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     cancel: Union[float, dt.timedelta]
 # end DataCollectorProtocol
 
 class BaseScreenerProtocol(DataCollectorProtocol):
     """A class for the base screener protocol."""
 
     symbol: str
-    market: str
+    exchange: str
 
     market: pd.DataFrame
 # end BaseScreenerProtocol
 
 class BaseMultiScreenerProtocol(DataCollectorProtocol):
     """A class for the base multi-screener protocol."""
```

### Comparing `crypto-screening-1.8.3/crypto_screening/market/foundation/waiting.py` & `crypto-screening-1.9.0/crypto_screening/market/foundation/waiting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,36 @@
 # waiting.py
 
 import datetime as dt
 import time
-from dataclasses import dataclass
 from typing import (
-    Optional, Union, Iterable, ClassVar,
-    Generic, TypeVar, Callable, List
+    Optional, Union, Iterable, Callable
 )
 
-from represent import represent, Modifiers
-
+from crypto_screening.market.foundation.state import WaitingState
+from crypto_screening.market.foundation.data import DataCollector
 from crypto_screening.market.foundation.protocols import (
-    BaseScreenerProtocol, BaseMultiScreenerProtocol
+    BaseScreenerProtocol
 )
-
 __all__ = [
     "base_wait_for_update",
     "base_wait_for_initialization",
-    "WaitingState",
     "base_wait_for_dynamic_update",
     "base_wait_for_dynamic_initialization"
 ]
 
-_BaseScreener = TypeVar(
-    "_BaseScreener", BaseScreenerProtocol, BaseMultiScreenerProtocol
-)
-
-@dataclass(repr=False, slots=True)
-@represent
-class WaitingState(Generic[_BaseScreener]):
-    """A class to represent the waiting state of screener objects."""
-
-    screeners: Iterable[Union[_BaseScreener]]
-    start: dt.datetime
-    end: dt.datetime
-    stop: Optional[bool] = False
-    delay: Optional[float] = 0
-    count: Optional[int] = 0
-    canceled: Optional[bool] = False
-    cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-
-    __modifiers__: ClassVar[Modifiers] = Modifiers(
-        hidden=["screeners"], properties=["time"]
-    )
-
-    @property
-    def time(self) -> dt.timedelta:
-        """
-        Returns the amount of waited time.
-
-        :return: The waiting time.
-        """
-
-        return self.end - self.start
-    # end time
-# end WaitingState
+Gatherer = Callable[[Iterable[DataCollector]], Iterable[BaseScreenerProtocol]]
 
 def base_wait_for_dynamic_initialization(
-        screeners: Iterable[_BaseScreener],
+        screeners: Iterable[DataCollector],
         stop: Optional[bool] = None,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
-        gatherer: Callable[[Iterable[_BaseScreener]], List[_BaseScreener]] = None
-) -> WaitingState[_BaseScreener]:
+        gatherer: Optional[Gatherer] = None
+) -> WaitingState[DataCollector]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
@@ -137,20 +101,20 @@
         screeners=screeners, delay=delay,
         count=count, end=dt.datetime.now(), start=start,
         cancel=cancel, canceled=canceled
     )
 # end base_wait_for_dynamic_initialization
 
 def base_wait_for_initialization(
-        *screeners: _BaseScreener,
+        *screeners: DataCollector,
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
-        gatherer: Callable[[Iterable[_BaseScreener]], List[_BaseScreener]] = None
-) -> WaitingState[_BaseScreener]:
+        gatherer: Optional[Gatherer] = None
+) -> WaitingState[DataCollector]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
@@ -162,20 +126,20 @@
     return base_wait_for_dynamic_initialization(
         screeners, delay=delay, stop=stop,
         cancel=cancel, gatherer=gatherer
     )
 # end base_wait_for_initialization
 
 def base_wait_for_dynamic_update(
-        screeners: Iterable[_BaseScreener],
+        screeners: Iterable[DataCollector],
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
-        gatherer: Callable[[Iterable[_BaseScreener]], List[_BaseScreener]] = None
-) -> WaitingState[_BaseScreener]:
+        gatherer: Optional[Gatherer] = None
+) -> WaitingState[DataCollector]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
@@ -257,20 +221,20 @@
         screeners=screeners, delay=delay,
         count=count, end=dt.datetime.now(), start=start,
         cancel=cancel, canceled=canceled
     )
 # end base_wait_for_dynamic_update
 
 def base_wait_for_update(
-        *screeners: _BaseScreener,
+        *screeners: DataCollector,
         stop: Optional[bool] = False,
         delay: Optional[Union[float, dt.timedelta]] = None,
         cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
-        gatherer: Callable[[Iterable[_BaseScreener]], List[_BaseScreener]] = None
-) -> WaitingState[_BaseScreener]:
+        gatherer: Optional[Gatherer] = None
+) -> WaitingState[DataCollector]:
     """
     Waits for all the create_screeners to update.
 
     :param screeners: The create_screeners to wait for them to update.
     :param delay: The delay for the waiting.
     :param stop: The value to stop the screener objects.
     :param cancel: The time to cancel the waiting.
```

### Comparing `crypto-screening-1.8.3/crypto_screening/market/screeners/base.py` & `crypto-screening-1.9.0/crypto_screening/market/screeners/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,32 @@
 from represent import Modifiers
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import save_dataset, load_dataset
 from crypto_screening.symbols import Separator
 from crypto_screening.validate import validate_exchange, validate_symbol
+from crypto_screening.market.foundation.state import WaitingState
 from crypto_screening.market.foundation.waiting import (
     base_wait_for_initialization, base_wait_for_dynamic_initialization,
-    base_wait_for_dynamic_update, base_wait_for_update, WaitingState
+    base_wait_for_dynamic_update, base_wait_for_update
 )
 from crypto_screening.market.foundation.data import DataCollector
 from crypto_screening.market.screeners.recorder import (
     MarketRecorder, create_market_dataframe
 )
-from crypto_screening.market.foundation.protocols import (
-    BaseMultiScreenerProtocol, BaseScreenerProtocol
-)
 
 __all__ = [
     "BaseScreener",
     "BaseMultiScreener",
     "structure_screeners_datasets",
     "structure_screener_datasets"
 ]
 
-class BaseScreener(DataCollector, BaseScreenerProtocol):
+class BaseScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -240,15 +238,15 @@
             end = time.time()
 
             time.sleep(max([delay - (end - start), 1]))
         # end while
     # end saving_loop
 # end BaseScreener
 
-class BaseMultiScreener(DataCollector, BaseMultiScreenerProtocol):
+class BaseMultiScreener(DataCollector):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -261,19 +259,19 @@
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
     """
 
     __modifiers__ = Modifiers(**DataCollector.__modifiers__)
-    __modifiers__.hidden.extend(["screeners", 'market'])
+    __modifiers__.hidden.extend(["screeners", 'recorder'])
 
     screeners: List[BaseScreener]
 
-    __slots__ = "screeners", "location", "cancel", "delay", 'recorder'
+    __slots__ = 'recorder', 'screeners'
 
     def __init__(
             self,
             screeners: Optional[Iterable[BaseScreener]] = None,
             recorder: Optional[MarketRecorder] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
```

### Comparing `crypto-screening-1.8.3/crypto_screening/market/screeners/container.py` & `crypto-screening-1.9.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-1.9.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     >>>
     >>>     print(screener.market.iloc[-1].splitlines()[-1])
     """
 
     __modifiers__ = Modifiers(**BaseScreener.__modifiers__)
     __modifiers__.excluded.append('task')
 
-    __slots__ = "interval", "pro", "market", "options", "task"
+    __slots__ = "interval", "pro", "options", "task"
 
     INTERVAL = "1m"
 
     PRO = False
 
     OPTIONS = {}
```

### Comparing `crypto-screening-1.8.3/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-1.9.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
     >>>
     >>> screener = market_orderbook_screener(data=structure)
     >>> screener.run()
     """
 
     __modifiers__ = Modifiers(**BaseMultiScreener.__modifiers__)
     __modifiers__.excluded.extend(
-        ['screening_parameters', 'feeds_parameters', 'handler']
+        ['_run_parameters', '_feeds_parameters', 'handler']
     )
 
     __slots__ = (
         "handler", 'amount', "loop", "limited", "_feeds_parameters",
         "_run_parameters", 'refresh'
     )
```

### Comparing `crypto-screening-1.8.3/crypto_screening/market/screeners/recorder.py` & `crypto-screening-1.9.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/market/waiting.py` & `crypto-screening-1.9.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/process.py` & `crypto-screening-1.9.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/symbols.py` & `crypto-screening-1.9.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening/validate.py` & `crypto-screening-1.9.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.8.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.9.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.8.3
+Version: 1.9.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.8.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.9.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 crypto_screening.egg-info/PKG-INFO
 crypto_screening.egg-info/SOURCES.txt
 crypto_screening.egg-info/dependency_links.txt
 crypto_screening.egg-info/requires.txt
 crypto_screening.egg-info/top_level.txt
 crypto_screening/collect/assets.py
 crypto_screening/collect/exchanges.py
+crypto_screening/collect/market.py
 crypto_screening/collect/screeners.py
 crypto_screening/collect/symbols.py
 crypto_screening/market/waiting.py
 crypto_screening/market/foundation/data.py
 crypto_screening/market/foundation/protocols.py
+crypto_screening/market/foundation/state.py
 crypto_screening/market/foundation/waiting.py
 crypto_screening/market/screeners/__init__.py
 crypto_screening/market/screeners/base.py
 crypto_screening/market/screeners/container.py
 crypto_screening/market/screeners/ohlcv.py
 crypto_screening/market/screeners/orderbook.py
 crypto_screening/market/screeners/recorder.py
```

### Comparing `crypto-screening-1.8.3/pyproject.toml` & `crypto-screening-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.8.3'
+version = '1.9.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.8.3/setup.py` & `crypto-screening-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.8.3',
+        version='1.9.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

