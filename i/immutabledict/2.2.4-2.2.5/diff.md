# Comparing `tmp/immutabledict-2.2.4.tar.gz` & `tmp/immutabledict-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immutabledict-2.2.4.tar", max compression
+gzip compressed data, was "immutabledict-2.2.5.tar", max compression
```

## Comparing `immutabledict-2.2.4.tar` & `immutabledict-2.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-04-02 19:37:33.336215 immutabledict-2.2.4/LICENSE
--rw-r--r--   0        0        0     2180 2023-04-02 19:37:33.336215 immutabledict-2.2.4/README.md
--rw-r--r--   0        0        0     2473 2023-04-02 19:37:33.336215 immutabledict-2.2.4/immutabledict/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 19:37:33.336215 immutabledict-2.2.4/immutabledict/py.typed
--rw-r--r--   0        0        0     1045 2023-04-02 19:37:33.336215 immutabledict-2.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-02 19:37:33.336215 immutabledict-2.2.4/tests/__init__.py
--rw-r--r--   0        0        0     5392 2023-04-02 19:37:33.336215 immutabledict-2.2.4/tests/test_immutabledict.py
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 immutabledict-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-04 10:37:42.630829 immutabledict-2.2.5/LICENSE
+-rw-r--r--   0        0        0     2180 2023-07-04 10:37:42.630829 immutabledict-2.2.5/README.md
+-rw-r--r--   0        0        0     2481 2023-07-04 10:37:42.630829 immutabledict-2.2.5/immutabledict/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:37:42.630829 immutabledict-2.2.5/immutabledict/py.typed
+-rw-r--r--   0        0        0     1045 2023-07-04 10:37:42.630829 immutabledict-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-04 10:37:42.630829 immutabledict-2.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     5392 2023-07-04 10:37:42.630829 immutabledict-2.2.5/tests/test_immutabledict.py
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 immutabledict-2.2.5/PKG-INFO
```

### Comparing `immutabledict-2.2.4/LICENSE` & `immutabledict-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `immutabledict-2.2.4/README.md` & `immutabledict-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `immutabledict-2.2.4/immutabledict/__init__.py` & `immutabledict-2.2.5/immutabledict/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from collections import OrderedDict
 from typing import Any, Dict, Iterable, Iterator, Mapping, Optional, Type, TypeVar
 
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 
 _K = TypeVar("_K")
 _V = TypeVar("_V")
 
 
 class immutabledict(Mapping[_K, _V]):
     """
@@ -19,15 +19,15 @@
 
     dict_cls: Type[Dict[Any, Any]] = dict
 
     @classmethod
     def fromkeys(
         cls, seq: Iterable[_K], value: Optional[_V] = None
     ) -> "immutabledict[_K, _V]":
-        return cls(dict.fromkeys(seq, value))
+        return cls(cls.dict_cls.fromkeys(seq, value))
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self._dict = self.dict_cls(*args, **kwargs)
         self._hash: Optional[int] = None
 
     def __getitem__(self, key: _K) -> _V:
         return self._dict[key]
```

### Comparing `immutabledict-2.2.4/pyproject.toml` & `immutabledict-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "immutabledict"
-version = "2.2.4"
+version = "2.2.5"
 description = "Immutable wrapper around dictionaries (a fork of frozendict)"
 authors = ["Corentin Garcia <corenting@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/corenting/immutabledict"
 keywords = ["immutable", "dictionary"]
 classifiers = [
```

### Comparing `immutabledict-2.2.4/tests/test_immutabledict.py` & `immutabledict-2.2.5/tests/test_immutabledict.py`

 * *Files identical despite different names*

### Comparing `immutabledict-2.2.4/PKG-INFO` & `immutabledict-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immutabledict
-Version: 2.2.4
+Version: 2.2.5
 Summary: Immutable wrapper around dictionaries (a fork of frozendict)
 Home-page: https://github.com/corenting/immutabledict
 License: MIT
 Keywords: immutable,dictionary
 Author: Corentin Garcia
 Author-email: corenting@gmail.com
 Requires-Python: >=3.7,<4.0
```

