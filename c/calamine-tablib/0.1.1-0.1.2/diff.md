# Comparing `tmp/calamine_tablib-0.1.1.tar.gz` & `tmp/calamine_tablib-0.1.2.tar.gz`

## Comparing `calamine_tablib-0.1.1.tar` & `calamine_tablib-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 calamine_tablib-0.1.1/Cargo.toml
--rw-r--r--   0     1000     1000     2807 2023-06-29 04:22:18.000000 calamine_tablib-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000     2199 2023-07-03 14:49:48.000000 calamine_tablib-0.1.1/.gitignore
--rw-r--r--   0     1000     1000      584 2023-07-03 22:43:21.000000 calamine_tablib-0.1.1/README.md
--rw-r--r--   0     1000     1000      106 2023-07-04 02:11:29.000000 calamine_tablib-0.1.1/dev-requirements.txt
--rw-r--r--   0     1000     1000      513 2023-07-04 02:12:09.000000 calamine_tablib-0.1.1/pyproject.toml
--rw-r--r--   0     1000     1000      127 2023-07-03 14:04:59.000000 calamine_tablib-0.1.1/python/calamine_tablib/__init__.py
--rw-r--r--   0     1000     1000      683 2023-07-03 14:07:05.000000 calamine_tablib-0.1.1/python/calamine_tablib/_calamine_tablib.pyi
--rw-r--r--   0     1000     1000     1150 2023-07-03 22:45:40.000000 calamine_tablib-0.1.1/python/calamine_tablib/format.py
--rw-r--r--   0     1000     1000      122 2023-07-03 22:47:07.000000 calamine_tablib-0.1.1/python/calamine_tablib/monkey_patches.py
--rw-r--r--   0     1000     1000        0 2023-07-02 22:17:28.000000 calamine_tablib-0.1.1/python/calamine_tablib/py.typed
--rw-r--r--   0     1000     1000     1418 2023-07-03 22:22:04.000000 calamine_tablib-0.1.1/src/lib.rs
--rw-r--r--   0     1000     1000     3167 2023-07-03 22:23:30.000000 calamine_tablib-0.1.1/src/types/cell.rs
--rw-r--r--   0     1000     1000      256 2023-07-03 22:02:43.000000 calamine_tablib-0.1.1/src/types/mod.rs
--rw-r--r--   0     1000     1000      299 2023-07-03 19:41:49.000000 calamine_tablib-0.1.1/src/types/sheet.rs
--rw-r--r--   0     1000     1000     3467 2023-07-03 19:00:52.000000 calamine_tablib-0.1.1/src/types/workbook.rs
--rw-r--r--   0     1000     1000      281 2023-07-02 22:23:02.000000 calamine_tablib-0.1.1/src/utils.rs
--rw-r--r--   0     1000     1000        0 2023-07-03 14:28:53.000000 calamine_tablib-0.1.1/tests/__init__.py
--rw-r--r--   0     1000     1000       70 2023-07-03 22:27:19.000000 calamine_tablib-0.1.1/tests/data/.~lock.base.xlsx#
--rw-r--r--   0     1000     1000     8452 2023-07-03 14:28:21.000000 calamine_tablib-0.1.1/tests/data/base.xlsx
--rw-r--r--   0     1000     1000      589 2023-07-03 22:29:45.000000 calamine_tablib-0.1.1/tests/test_base.py
--rw-r--r--   0     1000     1000    22775 2023-07-04 02:13:08.000000 calamine_tablib-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 calamine_tablib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 calamine_tablib-0.1.2/Cargo.toml
+-rw-r--r--   0     1000     1000     2807 2023-06-29 04:22:18.000000 calamine_tablib-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000     2199 2023-07-03 14:49:48.000000 calamine_tablib-0.1.2/.gitignore
+-rw-r--r--   0     1000     1000      584 2023-07-03 22:43:21.000000 calamine_tablib-0.1.2/README.md
+-rw-r--r--   0     1000     1000      106 2023-07-04 02:11:29.000000 calamine_tablib-0.1.2/dev-requirements.txt
+-rw-r--r--   0     1000     1000      513 2023-07-04 02:12:09.000000 calamine_tablib-0.1.2/pyproject.toml
+-rw-r--r--   0     1000     1000      165 2023-07-04 02:19:09.000000 calamine_tablib-0.1.2/python/calamine_tablib/__init__.py
+-rw-r--r--   0     1000     1000      684 2023-07-04 02:19:09.000000 calamine_tablib-0.1.2/python/calamine_tablib/_calamine_tablib.pyi
+-rw-r--r--   0     1000     1000     1151 2023-07-04 02:19:09.000000 calamine_tablib-0.1.2/python/calamine_tablib/format.py
+-rw-r--r--   0     1000     1000      122 2023-07-03 22:47:07.000000 calamine_tablib-0.1.2/python/calamine_tablib/monkey_patches.py
+-rw-r--r--   0     1000     1000        0 2023-07-02 22:17:28.000000 calamine_tablib-0.1.2/python/calamine_tablib/py.typed
+-rw-r--r--   0     1000     1000     1418 2023-07-03 22:22:04.000000 calamine_tablib-0.1.2/src/lib.rs
+-rw-r--r--   0     1000     1000     3167 2023-07-03 22:23:30.000000 calamine_tablib-0.1.2/src/types/cell.rs
+-rw-r--r--   0     1000     1000      256 2023-07-03 22:02:43.000000 calamine_tablib-0.1.2/src/types/mod.rs
+-rw-r--r--   0     1000     1000      299 2023-07-03 19:41:49.000000 calamine_tablib-0.1.2/src/types/sheet.rs
+-rw-r--r--   0     1000     1000     3467 2023-07-03 19:00:52.000000 calamine_tablib-0.1.2/src/types/workbook.rs
+-rw-r--r--   0     1000     1000      281 2023-07-02 22:23:02.000000 calamine_tablib-0.1.2/src/utils.rs
+-rw-r--r--   0     1000     1000        0 2023-07-03 14:28:53.000000 calamine_tablib-0.1.2/tests/__init__.py
+-rw-r--r--   0     1000     1000       70 2023-07-03 22:27:19.000000 calamine_tablib-0.1.2/tests/data/.~lock.base.xlsx#
+-rw-r--r--   0     1000     1000     8452 2023-07-03 14:28:21.000000 calamine_tablib-0.1.2/tests/data/base.xlsx
+-rw-r--r--   0     1000     1000      590 2023-07-04 02:19:21.000000 calamine_tablib-0.1.2/tests/test_base.py
+-rw-r--r--   0     1000     1000    22775 2023-07-04 02:20:00.000000 calamine_tablib-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 calamine_tablib-0.1.2/PKG-INFO
```

### Comparing `calamine_tablib-0.1.1/.github/workflows/CI.yml` & `calamine_tablib-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/.gitignore` & `calamine_tablib-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/README.md` & `calamine_tablib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/pyproject.toml` & `calamine_tablib-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/python/calamine_tablib/_calamine_tablib.pyi` & `calamine_tablib-0.1.2/python/calamine_tablib/_calamine_tablib.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from datetime import date, datetime, time
 from os import PathLike
 from typing import Protocol
+
 from tablib.core import Dataset
 
 ValueT = int | float | str | bool | time | date | datetime
 
 class ReadBuffer(Protocol):
     def seek(self) -> int: ...
     def read(self) -> bytes: ...
```

### Comparing `calamine_tablib-0.1.1/python/calamine_tablib/format.py` & `calamine_tablib-0.1.2/python/calamine_tablib/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import itertools
 from io import BytesIO
 
+from calamine_tablib import load_dataset
 from pyexcelerate import Workbook
 from tablib.formats._xlsx import XLSXFormat
-from calamine_tablib import load_dataset
+
 
 class FastXLSXFormat(XLSXFormat):
     """XLSX format."""
 
     title = "fast_xlsx"
 
     @classmethod
```

### Comparing `calamine_tablib-0.1.1/src/lib.rs` & `calamine_tablib-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/src/types/cell.rs` & `calamine_tablib-0.1.2/src/types/cell.rs`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/src/types/workbook.rs` & `calamine_tablib-0.1.2/src/types/workbook.rs`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/tests/data/base.xlsx` & `calamine_tablib-0.1.2/tests/data/base.xlsx`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.1/tests/test_base.py` & `calamine_tablib-0.1.2/tests/test_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from io import BytesIO
 from pathlib import Path
 
 import pytest
-from tablib import Dataset
 from calamine_tablib import load_dataset
+from tablib import Dataset
 
 PATH = Path(__file__).parent / "data"
 
+
 @pytest.mark.parametrize(
     "obj",
     [
         PATH / "base.xlsx",
         (PATH / "base.xlsx").as_posix(),
         open(PATH / "base.xlsx", "rb"),
         BytesIO(open(PATH / "base.xlsx", "rb").read()),
```

### Comparing `calamine_tablib-0.1.1/Cargo.lock` & `calamine_tablib-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
  "quick-xml",
  "serde",
  "zip",
 ]
 
 [[package]]
 name = "calamine-tablib"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "calamine",
  "chrono",
  "pyo3",
  "pyo3-file",
 ]
```

### Comparing `calamine_tablib-0.1.1/PKG-INFO` & `calamine_tablib-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calamine-tablib
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: tablib >=3.5, <4.0
 Requires-Dist: PyExcelerate >=0.10, <1.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

