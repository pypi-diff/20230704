# Comparing `tmp/calamine_tablib-0.1.0.tar.gz` & `tmp/calamine_tablib-0.1.1.tar.gz`

## Comparing `calamine_tablib-0.1.0.tar` & `calamine_tablib-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 calamine_tablib-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000     2807 2023-06-29 04:22:18.000000 calamine_tablib-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000     2199 2023-07-03 14:49:48.000000 calamine_tablib-0.1.0/.gitignore
--rw-r--r--   0     1000     1000      584 2023-07-03 22:43:21.000000 calamine_tablib-0.1.0/README.md
--rw-r--r--   0     1000     1000       43 2023-07-04 02:07:37.000000 calamine_tablib-0.1.0/dev-requirements.txt
--rw-r--r--   0     1000     1000      484 2023-07-04 02:07:22.000000 calamine_tablib-0.1.0/pyproject.toml
--rw-r--r--   0     1000     1000      127 2023-07-03 14:04:59.000000 calamine_tablib-0.1.0/python/calamine_tablib/__init__.py
--rw-r--r--   0     1000     1000      683 2023-07-03 14:07:05.000000 calamine_tablib-0.1.0/python/calamine_tablib/_calamine_tablib.pyi
--rw-r--r--   0     1000     1000     1150 2023-07-03 22:45:40.000000 calamine_tablib-0.1.0/python/calamine_tablib/format.py
--rw-r--r--   0     1000     1000      122 2023-07-03 22:47:07.000000 calamine_tablib-0.1.0/python/calamine_tablib/monkey_patches.py
--rw-r--r--   0     1000     1000        0 2023-07-02 22:17:28.000000 calamine_tablib-0.1.0/python/calamine_tablib/py.typed
--rw-r--r--   0     1000     1000     1418 2023-07-03 22:22:04.000000 calamine_tablib-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000     3167 2023-07-03 22:23:30.000000 calamine_tablib-0.1.0/src/types/cell.rs
--rw-r--r--   0     1000     1000      256 2023-07-03 22:02:43.000000 calamine_tablib-0.1.0/src/types/mod.rs
--rw-r--r--   0     1000     1000      299 2023-07-03 19:41:49.000000 calamine_tablib-0.1.0/src/types/sheet.rs
--rw-r--r--   0     1000     1000     3467 2023-07-03 19:00:52.000000 calamine_tablib-0.1.0/src/types/workbook.rs
--rw-r--r--   0     1000     1000      281 2023-07-02 22:23:02.000000 calamine_tablib-0.1.0/src/utils.rs
--rw-r--r--   0     1000     1000        0 2023-07-03 14:28:53.000000 calamine_tablib-0.1.0/tests/__init__.py
--rw-r--r--   0     1000     1000       70 2023-07-03 22:27:19.000000 calamine_tablib-0.1.0/tests/data/.~lock.base.xlsx#
--rw-r--r--   0     1000     1000     8452 2023-07-03 14:28:21.000000 calamine_tablib-0.1.0/tests/data/base.xlsx
--rw-r--r--   0     1000     1000      589 2023-07-03 22:29:45.000000 calamine_tablib-0.1.0/tests/test_base.py
--rw-r--r--   0     1000     1000    22775 2023-07-04 02:03:02.000000 calamine_tablib-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 calamine_tablib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 calamine_tablib-0.1.1/Cargo.toml
+-rw-r--r--   0     1000     1000     2807 2023-06-29 04:22:18.000000 calamine_tablib-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000     2199 2023-07-03 14:49:48.000000 calamine_tablib-0.1.1/.gitignore
+-rw-r--r--   0     1000     1000      584 2023-07-03 22:43:21.000000 calamine_tablib-0.1.1/README.md
+-rw-r--r--   0     1000     1000      106 2023-07-04 02:11:29.000000 calamine_tablib-0.1.1/dev-requirements.txt
+-rw-r--r--   0     1000     1000      513 2023-07-04 02:12:09.000000 calamine_tablib-0.1.1/pyproject.toml
+-rw-r--r--   0     1000     1000      127 2023-07-03 14:04:59.000000 calamine_tablib-0.1.1/python/calamine_tablib/__init__.py
+-rw-r--r--   0     1000     1000      683 2023-07-03 14:07:05.000000 calamine_tablib-0.1.1/python/calamine_tablib/_calamine_tablib.pyi
+-rw-r--r--   0     1000     1000     1150 2023-07-03 22:45:40.000000 calamine_tablib-0.1.1/python/calamine_tablib/format.py
+-rw-r--r--   0     1000     1000      122 2023-07-03 22:47:07.000000 calamine_tablib-0.1.1/python/calamine_tablib/monkey_patches.py
+-rw-r--r--   0     1000     1000        0 2023-07-02 22:17:28.000000 calamine_tablib-0.1.1/python/calamine_tablib/py.typed
+-rw-r--r--   0     1000     1000     1418 2023-07-03 22:22:04.000000 calamine_tablib-0.1.1/src/lib.rs
+-rw-r--r--   0     1000     1000     3167 2023-07-03 22:23:30.000000 calamine_tablib-0.1.1/src/types/cell.rs
+-rw-r--r--   0     1000     1000      256 2023-07-03 22:02:43.000000 calamine_tablib-0.1.1/src/types/mod.rs
+-rw-r--r--   0     1000     1000      299 2023-07-03 19:41:49.000000 calamine_tablib-0.1.1/src/types/sheet.rs
+-rw-r--r--   0     1000     1000     3467 2023-07-03 19:00:52.000000 calamine_tablib-0.1.1/src/types/workbook.rs
+-rw-r--r--   0     1000     1000      281 2023-07-02 22:23:02.000000 calamine_tablib-0.1.1/src/utils.rs
+-rw-r--r--   0     1000     1000        0 2023-07-03 14:28:53.000000 calamine_tablib-0.1.1/tests/__init__.py
+-rw-r--r--   0     1000     1000       70 2023-07-03 22:27:19.000000 calamine_tablib-0.1.1/tests/data/.~lock.base.xlsx#
+-rw-r--r--   0     1000     1000     8452 2023-07-03 14:28:21.000000 calamine_tablib-0.1.1/tests/data/base.xlsx
+-rw-r--r--   0     1000     1000      589 2023-07-03 22:29:45.000000 calamine_tablib-0.1.1/tests/test_base.py
+-rw-r--r--   0     1000     1000    22775 2023-07-04 02:13:08.000000 calamine_tablib-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 calamine_tablib-0.1.1/PKG-INFO
```

### Comparing `calamine_tablib-0.1.0/.github/workflows/CI.yml` & `calamine_tablib-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/.gitignore` & `calamine_tablib-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/README.md` & `calamine_tablib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/python/calamine_tablib/_calamine_tablib.pyi` & `calamine_tablib-0.1.1/python/calamine_tablib/_calamine_tablib.pyi`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/python/calamine_tablib/format.py` & `calamine_tablib-0.1.1/python/calamine_tablib/format.py`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/src/lib.rs` & `calamine_tablib-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/src/types/cell.rs` & `calamine_tablib-0.1.1/src/types/cell.rs`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/src/types/workbook.rs` & `calamine_tablib-0.1.1/src/types/workbook.rs`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/tests/data/base.xlsx` & `calamine_tablib-0.1.1/tests/data/base.xlsx`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/tests/test_base.py` & `calamine_tablib-0.1.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `calamine_tablib-0.1.0/Cargo.lock` & `calamine_tablib-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
  "quick-xml",
  "serde",
  "zip",
 ]
 
 [[package]]
 name = "calamine-tablib"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "calamine",
  "chrono",
  "pyo3",
  "pyo3-file",
 ]
```

### Comparing `calamine_tablib-0.1.0/PKG-INFO` & `calamine_tablib-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: calamine-tablib
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: tablib >=3.5, <4.0
+Requires-Dist: PyExcelerate >=0.10, <1.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # `calamine-tablib`
 
 A fast excel format for tablib.
```

