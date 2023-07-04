# Comparing `tmp/inductance-0.1.1a3.tar.gz` & `tmp/inductance-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductance-0.1.1a3.tar", max compression
+gzip compressed data, was "inductance-0.1.2.tar", max compression
```

## Comparing `inductance-0.1.1a3.tar` & `inductance-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-02 17:50:10.046386 inductance-0.1.1a3/LICENSE
--rw-r--r--   0        0        0     2522 2023-07-02 17:50:10.046386 inductance-0.1.1a3/README.md
--rw-r--r--   0        0        0     1810 2023-07-02 17:50:26.526601 inductance-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0      151 2023-07-02 17:50:26.526601 inductance-0.1.1a3/src/inductance/__init__.py
--rw-r--r--   0        0        0    28091 2023-07-02 17:50:10.050387 inductance-0.1.1a3/src/inductance/elliptics.py
--rw-r--r--   0        0        0     4297 2023-07-02 17:50:10.050387 inductance-0.1.1a3/src/inductance/filaments.py
--rw-r--r--   0        0        0    34787 2023-07-02 17:50:10.050387 inductance-0.1.1a3/src/inductance/inductance.py
--rw-r--r--   0        0        0     3384 1970-01-01 00:00:00.000000 inductance-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-04 08:01:17.006365 inductance-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4348 2023-07-04 08:01:17.006365 inductance-0.1.2/README.md
+-rw-r--r--   0        0        0     1807 2023-07-04 08:01:39.174371 inductance-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-07-04 08:01:17.010365 inductance-0.1.2/src/inductance/__init__.py
+-rw-r--r--   0        0        0     1484 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/_numba.py
+-rw-r--r--   0        0        0     5201 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/coils.py
+-rw-r--r--   0        0        0    27861 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/elliptics.py
+-rw-r--r--   0        0        0    14865 2023-07-04 08:01:39.174371 inductance-0.1.2/src/inductance/filaments.py
+-rw-r--r--   0        0        0     5476 2023-07-04 08:01:39.178371 inductance-0.1.2/src/inductance/mutual.py
+-rw-r--r--   0        0        0    19164 2023-07-04 08:01:39.178371 inductance-0.1.2/src/inductance/self.py
+-rw-r--r--   0        0        0     5208 1970-01-01 00:00:00.000000 inductance-0.1.2/PKG-INFO
```

### Comparing `inductance-0.1.1a3/LICENSE` & `inductance-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inductance-0.1.1a3/pyproject.toml` & `inductance-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inductance"
-version = "v0.1.1a3"
+version = "0.1.2"
 description = "Code for 2D inductance calculations"
 authors = ["Darren Garnier <dgarnier@reinrag.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dgarnier/inductance"
 repository = "https://github.com/dgarnier/inductance"
 documentation = "https://inductance.readthedocs.io"
```

### Comparing `inductance-0.1.1a3/src/inductance/elliptics.py` & `inductance-0.1.2/src/inductance/elliptics.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,16 @@
 With Numba, this runs ~10x faster than scipy.special if you need both k and e
 so.. don't need numba_scipy which lags numba and scipy often.
 """
 
 from math import log
 from typing import Tuple
 
-# use numba if its installed
-try:
-    from numba import njit
+from ._numba import njit
 
-except ImportError:  # pragma: no cover
-    from warnings import warn
-
-    WARNING = "Couldn't import Numba. Elliptic integrals will run slower than expected."
-    warn(WARNING, RuntimeWarning)
 
 # fmt: off
 @njit("UniTuple(float64, 2)(float64)")
 def celbd(mc):
     """Complete elliptic integrals of second kind, B(m) and D(m).
 
     Args:
```

