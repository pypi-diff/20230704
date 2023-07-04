# Comparing `tmp/cachetory-2.2.0.tar.gz` & `tmp/cachetory-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.2.0.tar", max compression
+gzip compressed data, was "cachetory-2.3.0.tar", max compression
```

## Comparing `cachetory-2.2.0.tar` & `cachetory-2.3.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    11355 2023-06-14 11:42:16.295998 cachetory-2.2.0/LICENSE
--rw-r--r--   0        0        0    13566 2023-06-14 11:42:16.295998 cachetory-2.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/__init__.py
--rw-r--r--   0        0        0      999 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     1539 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1727 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2502 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0      993 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2361 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2197 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     2384 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     2273 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3644 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3478 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      255 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/private/datetime.py
--rw-r--r--   0        0        0      205 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/py.typed
--rw-r--r--   0        0        0      402 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2718 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      544 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/json.py
--rw-r--r--   0        0        0      608 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/msgpack.py
--rw-r--r--   0        0        0      538 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-06-14 11:42:16.295998 cachetory-2.2.0/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3220 2023-06-14 11:42:33.471940 cachetory-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    15081 1970-01-01 00:00:00.000000 cachetory-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-07-03 15:19:22.971992 cachetory-2.3.0/LICENSE
+-rw-r--r--   0        0        0    13582 2023-07-03 15:19:22.971992 cachetory-2.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1727 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2502 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0      993 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     1427 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2361 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2197 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3631 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     2978 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     2596 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0      990 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     2302 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3644 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3478 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      255 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      618 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/private/functools.py
+-rw-r--r--   0        0        0      205 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/py.typed
+-rw-r--r--   0        0        0      402 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     2718 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1026 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1248 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      544 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      608 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      538 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1106 2023-07-03 15:19:22.971992 cachetory-2.3.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3237 2023-07-03 15:19:37.396194 cachetory-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    15097 1970-01-01 00:00:00.000000 cachetory-2.3.0/PKG-INFO
```

### Comparing `cachetory-2.2.0/LICENSE` & `cachetory-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/README.md` & `cachetory-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,19 @@
 ### Instantiating a `Cache`
 
 Both sync and async `Cache`s requires at least these parameters to work:
 
 - `backend`: functions as a storage
 - `serializer`: is responsible for converting actual values from and to something that a backend would be able to store
 
-`Cache` may be annotated with a value type, like this: `Cache[ValueT]`, which provides type hints for the cache methods.
+`Cache` may be annotated with a value type like this `Cache[ValueT, WireT]`, which provides type hints for the cache methods.
 
 ### Instantiating a backend
 
-There is a few ways to instantiate a backend:
+There are a few ways to instantiate a backend:
 
 - By **directly instantiating** a backend class via its `__init__`
 - By instantiating a specific backend class **via its `from_url` class method**. In that case the URL is forwarded to underlying client (if any)
 - **By using `cachetory.[sync|async_].from_url` function.** In that case specific backend class is chosen by the URL's scheme (see the scheme badges below), and the URL is forwarded to its `from_url` class method. This is especially useful to configure an arbitrary backend from a single configuration option – instead of hard-coding a specific backend class.
 
 #### Examples
 
@@ -124,16 +124,16 @@
 `@cached` performs [memoization](https://en.wikipedia.org/wiki/Memoization) of a wrapped function:
 
 ```python
 from cachetory.caches.sync import Cache
 from cachetory.decorators.shared import make_default_key
 from cachetory.decorators.sync import cached
 
-cache = Cache[int](backend=..., serializer=...)
-another_cache = Cache[int](backend=..., serializer=...)
+cache = Cache[int, ...](backend=..., serializer=...)
+another_cache = Cache[int, ...](backend=..., serializer=...)
 
 
 @cached(
     cache,  # may also be a callable that returns a specific cache for each call, e.g.:
     # `cache=lambda wrapped_callable, *args, **kwargs: cache if … else another_cache`
 
     # The following parameters are optional (shown the defaults):
```

### Comparing `cachetory-2.2.0/cachetory/backends/async_/__init__.py` & `cachetory-2.3.0/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/backends/async_/dummy.py` & `cachetory-2.3.0/cachetory/backends/async_/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/backends/async_/memory.py` & `cachetory-2.3.0/cachetory/backends/async_/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/backends/async_/redis.py` & `cachetory-2.3.0/cachetory/backends/async_/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/backends/sync/__init__.py` & `cachetory-2.3.0/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/backends/sync/dummy.py` & `cachetory-2.3.0/cachetory/backends/sync/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/backends/sync/memory.py` & `cachetory-2.3.0/cachetory/backends/sync/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/backends/sync/redis.py` & `cachetory-2.3.0/cachetory/backends/sync/redis.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/caches/async_.py` & `cachetory-2.3.0/cachetory/caches/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/caches/sync.py` & `cachetory-2.3.0/cachetory/caches/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/decorators/async_.py` & `cachetory-2.3.0/cachetory/decorators/async_.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,61 @@
+from __future__ import annotations
+
 from datetime import timedelta
 from functools import wraps
 from typing import Awaitable, Callable, Optional, Union
 
 from typing_extensions import ParamSpec
 
 from cachetory.caches.async_ import Cache
 from cachetory.decorators import shared
 from cachetory.interfaces.backends.private import WireT
 from cachetory.interfaces.serializers import ValueT
+from cachetory.private.functools import maybe_awaitable, maybe_callable
 
 P = ParamSpec("P")
 """
 Original wrapped function parameter specification.
 """
 
 
 def cached(
-    cache: Union[Cache[ValueT, WireT], Callable[..., Awaitable[Cache[ValueT, WireT]]]],  # no way to use `P` here
+    cache: Union[
+        Cache[ValueT, WireT],
+        Callable[..., Cache[ValueT, WireT]],
+        Callable[..., Awaitable[Cache[ValueT, WireT]]],
+    ],  # no way to use `P` here
     *,
     make_key: Callable[..., str] = shared.make_default_key,  # no way to use `P` here
-    time_to_live: Optional[Union[timedelta, Callable[..., Awaitable[timedelta]]]] = None,
+    time_to_live: Optional[timedelta | Callable[..., timedelta] | Callable[..., Awaitable[timedelta]]] = None,
     if_not_exists: bool = False,
 ) -> Callable[[Callable[P, Awaitable[ValueT]]], Callable[P, Awaitable[ValueT]]]:
     """
     Apply memoization to the wrapped callable.
 
     Args:
         cache:
-            `Cache` instance or an async callable tha returns a `Cache` instance for each function call.
+            `Cache` instance or a callable (sync or async) that returns a `Cache` instance for each function call.
             In the latter case the specific callable gets called with a wrapped function as the first argument,
             and the rest of the arguments next to it.
         make_key: callable to generate a custom cache key per each call.
         if_not_exists: controls concurrent sets: if `True` – avoids overwriting a cached value.
         time_to_live:
-            cached value expiration time or async callable that returns the expiration time.
+            cached value expiration time or a callable (sync or async) that returns the expiration time.
             The callable needs to accept keyword arguments, and it is given the cache key to
             compute the expiration time.
     """
 
     def wrap(callable_: Callable[P, Awaitable[ValueT]]) -> Callable[P, Awaitable[ValueT]]:
         @wraps(callable_)
         async def cached_callable(*args: P.args, **kwargs: P.kwargs) -> ValueT:
-            cache_ = await cache(callable_, *args, **kwargs) if callable(cache) else cache
+            cache_ = await maybe_awaitable(maybe_callable(cache, callable_, *args, **kwargs))
             key_ = make_key(callable_, *args, **kwargs)
-            time_to_live_ = await time_to_live(key=key_) if callable(time_to_live) else time_to_live
+            time_to_live_ = await maybe_awaitable(maybe_callable(time_to_live, key=key_))
+
             value = await cache_.get(key_)
             if value is None:
                 value = await callable_(*args, **kwargs)
                 await cache_.set(key_, value, time_to_live=time_to_live_, if_not_exists=if_not_exists)
             return value
 
         return cached_callable
```

### Comparing `cachetory-2.2.0/cachetory/decorators/shared.py` & `cachetory-2.3.0/cachetory/decorators/shared.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/decorators/sync.py` & `cachetory-2.3.0/cachetory/decorators/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from __future__ import annotations
+
 from datetime import timedelta
 from functools import wraps
-from typing import Callable, Optional, Union
+from typing import Callable, Optional
 
 from typing_extensions import ParamSpec
 
 from cachetory.caches.sync import Cache
 from cachetory.decorators import shared
 from cachetory.interfaces.backends.private import WireT
 from cachetory.interfaces.serializers import ValueT
+from cachetory.private.functools import maybe_callable
 
 P = ParamSpec("P")
-"""
-Original wrapped function parameter specification.
-"""
+"""Original wrapped function parameter specification."""
 
 
 def cached(
-    cache: Union[Cache[ValueT, WireT], Callable[..., Cache[ValueT, WireT]]],  # no way to use `P` here
+    cache: Cache[ValueT, WireT] | Callable[..., Cache[ValueT, WireT]],  # no way to use `P` here
     *,
     make_key: Callable[..., str] = shared.make_default_key,  # no way to use `P` here
-    time_to_live: Optional[Union[timedelta, Callable[..., timedelta]]] = None,
+    time_to_live: Optional[timedelta | Callable[..., timedelta]] = None,
     if_not_exists: bool = False,
 ) -> Callable[[Callable[P, ValueT]], Callable[P, ValueT]]:
     """
     Apply memoization to the wrapped callable.
 
     Args:
         cache:
@@ -37,17 +38,18 @@
             The callable needs to accept keyword arguments, and it is given the cache key to
             compute the expiration time.
     """
 
     def wrap(callable_: Callable[P, ValueT]) -> Callable[P, ValueT]:
         @wraps(callable_)
         def cached_callable(*args: P.args, **kwargs: P.kwargs) -> ValueT:
-            cache_ = cache(callable_, *args, **kwargs) if callable(cache) else cache
+            cache_ = maybe_callable(cache, callable_, *args, **kwargs)
             key_ = make_key(callable_, *args, **kwargs)
-            time_to_live_ = time_to_live(key=key_) if callable(time_to_live) else time_to_live
+            time_to_live_ = maybe_callable(time_to_live, key=key_)
+
             try:
                 value = cache_[key_]
             except KeyError:
                 value = callable_(*args, **kwargs)
                 cache_.set(key_, value, time_to_live=time_to_live_, if_not_exists=if_not_exists)
             return value
```

### Comparing `cachetory-2.2.0/cachetory/interfaces/backends/async_.py` & `cachetory-2.3.0/cachetory/interfaces/backends/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/interfaces/backends/private.py` & `cachetory-2.3.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/interfaces/backends/sync.py` & `cachetory-2.3.0/cachetory/interfaces/backends/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/interfaces/serializers.py` & `cachetory-2.3.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/serializers/chained.py` & `cachetory-2.3.0/cachetory/serializers/chained.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/serializers/compressors/zlib.py` & `cachetory-2.3.0/cachetory/serializers/compressors/zlib.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/serializers/compressors/zstd.py` & `cachetory-2.3.0/cachetory/serializers/compressors/zstd.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/serializers/json.py` & `cachetory-2.3.0/cachetory/serializers/json.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/serializers/msgpack.py` & `cachetory-2.3.0/cachetory/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/serializers/noop.py` & `cachetory-2.3.0/cachetory/serializers/noop.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/cachetory/serializers/pickle.py` & `cachetory-2.3.0/cachetory/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.2.0/pyproject.toml` & `cachetory-2.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.2.0"
+version = "2.3.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -43,17 +43,17 @@
 zstd = ["zstd"]
 ormsgpack = ["ormsgpack"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
+mypy = "^1.3.0"
 black = "^23.1.0"
-ruff = "^0.0.239"
+ruff = "^0.0.275"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 types-redis = "^4.4.0.4"
 freezegun = "^1.2.2"
 
 [tool.black]
@@ -136,14 +136,15 @@
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
     "except ImportError",
     "if TYPE_CHECKING:",
+    "@overload",
 ]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 pattern = "default-unprefixed"
 style = "pep440"
```

### Comparing `cachetory-2.2.0/PKG-INFO` & `cachetory-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetory
-Version: 2.2.0
+Version: 2.3.0
 Summary: Caching library with support for multiple cache backends
 Home-page: https://github.com/kpn/cachetory
 License: Apache-2.0
 Keywords: cache
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -106,19 +106,19 @@
 ### Instantiating a `Cache`
 
 Both sync and async `Cache`s requires at least these parameters to work:
 
 - `backend`: functions as a storage
 - `serializer`: is responsible for converting actual values from and to something that a backend would be able to store
 
-`Cache` may be annotated with a value type, like this: `Cache[ValueT]`, which provides type hints for the cache methods.
+`Cache` may be annotated with a value type like this `Cache[ValueT, WireT]`, which provides type hints for the cache methods.
 
 ### Instantiating a backend
 
-There is a few ways to instantiate a backend:
+There are a few ways to instantiate a backend:
 
 - By **directly instantiating** a backend class via its `__init__`
 - By instantiating a specific backend class **via its `from_url` class method**. In that case the URL is forwarded to underlying client (if any)
 - **By using `cachetory.[sync|async_].from_url` function.** In that case specific backend class is chosen by the URL's scheme (see the scheme badges below), and the URL is forwarded to its `from_url` class method. This is especially useful to configure an arbitrary backend from a single configuration option – instead of hard-coding a specific backend class.
 
 #### Examples
 
@@ -160,16 +160,16 @@
 `@cached` performs [memoization](https://en.wikipedia.org/wiki/Memoization) of a wrapped function:
 
 ```python
 from cachetory.caches.sync import Cache
 from cachetory.decorators.shared import make_default_key
 from cachetory.decorators.sync import cached
 
-cache = Cache[int](backend=..., serializer=...)
-another_cache = Cache[int](backend=..., serializer=...)
+cache = Cache[int, ...](backend=..., serializer=...)
+another_cache = Cache[int, ...](backend=..., serializer=...)
 
 
 @cached(
     cache,  # may also be a callable that returns a specific cache for each call, e.g.:
     # `cache=lambda wrapped_callable, *args, **kwargs: cache if … else another_cache`
 
     # The following parameters are optional (shown the defaults):
```

