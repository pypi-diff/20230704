# Comparing `tmp/zeugvars-0.1.3.tar.gz` & `tmp/zeugvars-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.1.3.tar", max compression
+gzip compressed data, was "zeugvars-0.2.0.tar", max compression
```

## Comparing `zeugvars-0.1.3.tar` & `zeugvars-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.1.3/LICENSE
--rw-r--r--   0        0        0      524 2023-07-01 11:10:05.294301 zeugvars-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2474 2023-07-01 11:09:48.290088 zeugvars-0.1.3/README.md
--rw-r--r--   0        0        0    11260 2023-07-01 11:09:48.282092 zeugvars-0.1.3/zeugvars.py
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 zeugvars-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3450 2023-07-04 18:23:30.006891 zeugvars-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4145 2023-07-04 18:23:30.014888 zeugvars-0.2.0/README.md
+-rw-r--r--   0        0        0    10695 2023-07-04 18:21:07.559831 zeugvars-0.2.0/zeugvars.py
+-rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 zeugvars-0.2.0/PKG-INFO
```

### Comparing `zeugvars-0.1.3/LICENSE` & `zeugvars-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.1.3/zeugvars.py` & `zeugvars-0.2.0/zeugvars.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,85 @@
-"""
-ZeugVars
-~~~~~~~~
+"""`zeugvars`.
+
 A simple & straight-forward Python module for creating context-dependent proxy objects.
 
 (C) bswck, 2023
-
-What is this?
--------------
-`zeugvars` is a Python module for creating context-dependent proxy objects.
-
-By 'proxy' we mean any object that forwards attribute access to another
-object.  By 'context-dependent' we mean that the object to which the proxy
-forwards attribute access can change depending on the context in which the
-proxy is used.
-
-Have you ever wondered how `flask.request` works?
-------------------------------------------------
-How is it possible that `flask.request` is different for each request, despite
-being a global variable?
-
-The answer is that `flask.request` is a proxy object: it forwards attribute
-access to an object that is different for each request. With a little simplification,
-the object to which `flask.request` forwards attribute access is stored
-in a `werkzeug.local.LocalProxy` object. The functionality of `zeugvars.zeugvar()`
-is roughly equivalent to `werkzeug.local.LocalProxy`. The `zeugvar` function
-creates a proxy object that forwards attribute access to an object stored
-in the provided manager, which could be any object that implements the
-`Manager` protocol; for example, a `contextvars.ContextVar` object.
-
-Description
------------
-The `zeugvar` function takes a `Manager` object and class (optional) as arguments.
-The `Manager` object must have `get` and `set` methods. The `get` method returns
-the object to which the proxy forwards attribute access. The `set` method sets
-the object to which the proxy forwards attribute access. `set` is called when
-the proxy is being inplace modified. The class parameter is optional,
-but it is strongly recommended for some corner-cases.
-The user might provide custom `getter` and `setter` functions.
-This might be useful when there is the need to keep track of the tokens
-returned by `ContextVar.set()`, if using `ContextVar` as the manager.
-
-Example
--------
-The following example shows how to use `zeugvar` with `contextvars.ContextVar`:
-
->>> from contextvars import ContextVar
->>> from zeugvars import zeugvar
-...
->>> counter: ContextVar[int] = ContextVar("counter")
->>> count = zeugvar(counter, int)
-...
->>> counter.set(0)
->>> count += 1
->>> count
-1
->>> count -= 1
->>> count
-0
->>> counter.set(1000)
-<Token var=<ContextVar name='counter' at ...> at ...>
->>> count
-1000
 """
 
+from collections.abc import Callable
 from contextlib import suppress
 from functools import partial
-from collections.abc import Callable
-from typing import TypeVar, Any, cast, Protocol, runtime_checkable
+from typing import Any, Protocol, TypeVar, cast, runtime_checkable
 
-__all__ = ("zeugvar",)
+__all__ = ("zeugvar", "proxy")
 
 _T = TypeVar("_T")
 
 
 @runtime_checkable
 class Manager(Protocol[_T]):
+    """Protocol for zeugvars managers.
+
+    Matches `contextvars.ContextVar`.
+    """
+
     def get(self) -> _T:
-        ...
+        """Get the current value of the manager.
+
+        Raises
+        ------
+        LookupError
+            If no object is bound to the manager.
+        """
 
     def set(self, value: _T) -> Any:
-        ...
+        """Set the current value of the manager."""
 
 
 def zeugvar_descriptor(
     cls: type[_T] | None,
     mgr: Manager[_T],
     getter: Callable[[Manager[_T]], _T],
     setter: Callable[[Manager[_T], _T], None],
     *,
     undefined: Callable[..., Any] | None = None,
     fallback: Callable[..., Any] | None = None,
     custom_mro: bool = False,
     inplace: bool = False,
 ) -> Any:
-    """Descriptor factory for zeugvars.zeugvar() proxies."""
+    """Descriptor factory for zeugvars.
+
+    Parameters
+    ----------
+    cls
+        The class of the underlying variable accessed within the manager.
+    mgr
+        Manager object.
+    getter
+        A function that returns the underlying variable from the manager.
+    setter
+        A function that sets the underlying variable within the manager.
+    undefined
+        Callable to be used as a fallback in case the variable is undefined
+        (manager raises a `LookupError`).
+    fallback
+        Callable to be used as a fallback in case the attribute is undefined
+        (the underlying variable raises an `AttributeError`).
+    custom_mro
+        Whether the class implements a custom `mro()` method.
+    inplace
+        Whether to treat the attribute as an inplace operator.
+        Calls the setter with the result of the attribute call.
+
+    Returns
+    -------
+    descriptor
+        A descriptor object that can be used to create zeugvars delegates.
+
+    """
 
     class _ZeugVarDescriptor:
         attr_name: str
 
         def __init__(self) -> None:
             self.attr_name = None  # type: ignore[assignment]
 
@@ -164,29 +146,50 @@
     return lambda obj, op: getattr(obj, op_name)(op)
 
 
 def _cv_getter(mgr: Manager[_T]) -> _T:
     try:
         obj = mgr.get()
     except LookupError:
-        raise RuntimeError("No object in context") from None
+        msg = f"No object in {mgr}"
+        raise RuntimeError(msg) from None
     return obj
 
 
 def _cv_setter(mgr: Manager[_T], value: _T) -> None:
     mgr.set(value)
 
 
 def zeugvar(
     mgr: Manager[_T],
     cls: type[_T] | None = None,
     getter: Callable[[Manager[_T]], _T] = None,  # type: ignore[assignment]
     setter: Callable[[Manager[_T], _T], None] = None,  # type: ignore[assignment]
 ) -> _T:
-    """See `zeugvars` module docstring for usage and example."""
+    """Create a zeugvar proxy object.
+
+    Parameters
+    ----------
+    mgr
+        Manager object. Must implement the `Manager` protocol.
+        Matches `contextvars.ContextVar`.
+    cls
+        The class of the underlying variable accessed within the manager.
+    getter
+        A function that returns the underlying variable from the manager.
+    setter
+        A function that sets the underlying variable within the manager.
+
+    Returns
+    -------
+    proxy
+        A proxy object.
+    """
+
+    # pylint: disable=too-many-statements
 
     if getter is None:
         getter = _cv_getter
 
     if setter is None:
         setter = _cv_setter
 
@@ -197,15 +200,15 @@
     if cls is None:
         custom_mro = False
     else:
         mro: Callable[[], tuple[type[Any], ...]] = object.__getattribute__(cls, "mro")
         custom_mro = not hasattr(mro, "__self__")
 
     descriptor = partial(
-        zeugvar_descriptor, cls, mgr, getter, setter, custom_mro=custom_mro
+        zeugvar_descriptor, cls, mgr, getter, setter, custom_mro=custom_mro,
     )
 
     class _ZeugVarMeta(type):
         __doc__ = descriptor()
         __wrapped__ = descriptor()
         __repr__ = descriptor()
         __str__ = descriptor()
@@ -301,22 +304,23 @@
         __aenter__ = descriptor()
         __aexit__ = descriptor()
         __copy__ = descriptor()
         __deepcopy__ = descriptor()
 
     cls_name = cls.__name__ if cls is not None else f"zeugvar_{id(mgr):x}"
 
-    zv = cast(_T, _ZeugVarMeta(cls_name, (), {}))
+    zv_proxy = cast(_T, _ZeugVarMeta(cls_name, (), {}))
     if not custom_mro:
 
         def _mro_wrapper() -> tuple[type[Any], ...]:
             try:
                 obj = getter(mgr)
             except RuntimeError:
                 return mro()
-            else:
-                raise AttributeError(
-                    f"{type(obj).__name__!r} object has no attribute 'mro'"
-                ) from None
+            msg = f"{type(obj).__name__!r} object has no attribute 'mro'"
+            raise AttributeError(msg) from None
+
+        type.__setattr__(zv_proxy, "mro", _mro_wrapper)
+    return zv_proxy
+
 
-        type.__setattr__(zv, "mro", _mro_wrapper)
-    return zv
+proxy = zeugvar
```

