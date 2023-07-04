# Comparing `tmp/zeugvars-0.2.5.tar.gz` & `tmp/zeugvars-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.2.5.tar", max compression
+gzip compressed data, was "zeugvars-0.2.6.tar", max compression
```

## Comparing `zeugvars-0.2.5.tar` & `zeugvars-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.5/LICENSE
--rw-r--r--   0        0        0     3450 2023-07-04 18:43:20.243992 zeugvars-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4160 2023-07-04 18:43:08.544957 zeugvars-0.2.5/README.md
--rw-r--r--   0        0        0    10696 2023-07-04 18:43:08.536953 zeugvars-0.2.5/zeugvars/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 zeugvars-0.2.5/zeugvars/py.typed
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 zeugvars-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3450 2023-07-04 18:59:26.237845 zeugvars-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4160 2023-07-04 18:43:08.544957 zeugvars-0.2.6/README.md
+-rw-r--r--   0        0        0    10756 2023-07-04 18:57:13.132379 zeugvars-0.2.6/zeugvars/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 zeugvars-0.2.6/zeugvars/py.typed
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 zeugvars-0.2.6/PKG-INFO
```

### Comparing `zeugvars-0.2.5/LICENSE` & `zeugvars-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.5/pyproject.toml` & `zeugvars-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeugvars"
-version = "0.2.5"
+version = "0.2.6"
 description = "A simple & straight-forward Python module for creating context-dependent proxy objects."
 authors = ["bswck <bswck.dev@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/bswck/zeugvars"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `zeugvars-0.2.5/README.md` & `zeugvars-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.5/zeugvars/__init__.py` & `zeugvars-0.2.6/zeugvars/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,16 +195,20 @@
 
     if cls is None:
         with suppress(RuntimeError):
             cls = type(getter(mgr))
 
     if cls is None:
         custom_mro = False
+
+        def mro() -> list[type[Any]]:
+            return [object]
+
     else:
-        mro: Callable[[], tuple[type[Any], ...]] = object.__getattribute__(cls, "mro")
+        mro: Callable[[], list[type[Any]]] = object.__getattribute__(cls, "mro")
         custom_mro = not hasattr(mro, "__self__")
 
     descriptor = partial(
         zeugvar_descriptor, cls, mgr, getter, setter, custom_mro=custom_mro,
     )
 
     class _ZeugVarMeta(type):
@@ -307,15 +311,15 @@
         __deepcopy__ = descriptor()
 
     cls_name = cls.__name__ if cls is not None else f"zeugvar_{id(mgr):x}"
 
     zv_proxy = cast(_T, _ZeugVarMeta(cls_name, (), {}))
     if not custom_mro:
 
-        def _mro_wrapper() -> tuple[type[Any], ...]:
+        def _mro_wrapper() -> list[type[Any]]:
             try:
                 obj = getter(mgr)
             except RuntimeError:
                 return mro()
             msg = f"{type(obj).__name__!r} object has no attribute 'mro'"
             raise AttributeError(msg) from None
```

### Comparing `zeugvars-0.2.5/PKG-INFO` & `zeugvars-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeugvars
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
 Home-page: https://github.com/bswck/zeugvars
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

