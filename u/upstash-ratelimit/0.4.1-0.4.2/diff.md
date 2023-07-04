# Comparing `tmp/upstash_ratelimit-0.4.1.tar.gz` & `tmp/upstash_ratelimit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.4.1.tar", max compression
+gzip compressed data, was "upstash_ratelimit-0.4.2.tar", max compression
```

## Comparing `upstash_ratelimit-0.4.1.tar` & `upstash_ratelimit-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-07-04 06:39:50.982071 upstash_ratelimit-0.4.1/LICENSE
--rw-r--r--   0        0        0     7542 2023-07-04 06:39:50.982071 upstash_ratelimit-0.4.1/README.md
--rw-r--r--   0        0        0      475 2023-07-04 06:39:50.986071 upstash_ratelimit-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       73 2023-07-04 06:39:50.986071 upstash_ratelimit-0.4.1/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-04 06:39:50.986071 upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/algorithm.py
--rw-r--r--   0        0        0     3242 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/fixed_window_core.py
--rw-r--r--   0        0        0     5790 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/sliding_window_core.py
--rw-r--r--   0        0        0     5232 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/token_bucket_core.py
--rw-r--r--   0        0        0       81 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/async_blocker.py
--rw-r--r--   0        0        0     3090 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/fixed_window.py
--rw-r--r--   0        0        0     3505 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/limiter.py
--rw-r--r--   0        0        0     4013 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/sliding_window.py
--rw-r--r--   0        0        0     3518 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/token_bucket.py
--rw-r--r--   0        0        0      265 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3489 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0     2918 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/sync/fixed_window.py
--rw-r--r--   0        0        0     3619 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/sync/sliding_window.py
--rw-r--r--   0        0        0     1067 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/sync/sync_blocker.py
--rw-r--r--   0        0        0     3274 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/sync/token_bucket.py
--rw-r--r--   0        0        0      392 2023-07-04 06:39:50.990071 upstash_ratelimit-0.4.1/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0     8163 1970-01-01 00:00:00.000000 upstash_ratelimit-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-04 08:45:40.697860 upstash_ratelimit-0.4.2/LICENSE
+-rw-r--r--   0        0        0     7542 2023-07-04 08:45:40.697860 upstash_ratelimit-0.4.2/README.md
+-rw-r--r--   0        0        0      475 2023-07-04 08:45:40.697860 upstash_ratelimit-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0     1780 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/algorithm.py
+-rw-r--r--   0        0        0     3242 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/fixed_window_core.py
+-rw-r--r--   0        0        0     5790 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/sliding_window_core.py
+-rw-r--r--   0        0        0     5232 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/token_bucket_core.py
+-rw-r--r--   0        0        0       81 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/async_blocker.py
+-rw-r--r--   0        0        0     3012 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/fixed_window.py
+-rw-r--r--   0        0        0     3427 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/limiter.py
+-rw-r--r--   0        0        0     3935 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/sliding_window.py
+-rw-r--r--   0        0        0     3440 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/token_bucket.py
+-rw-r--r--   0        0        0      265 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3411 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0     2840 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/fixed_window.py
+-rw-r--r--   0        0        0     3541 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/sliding_window.py
+-rw-r--r--   0        0        0     1067 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/sync_blocker.py
+-rw-r--r--   0        0        0     3196 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/sync/token_bucket.py
+-rw-r--r--   0        0        0      392 2023-07-04 08:45:40.701860 upstash_ratelimit-0.4.2/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0     8163 1970-01-01 00:00:00.000000 upstash_ratelimit-0.4.2/PKG-INFO
```

### Comparing `upstash_ratelimit-0.4.1/LICENSE` & `upstash_ratelimit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.1/README.md` & `upstash_ratelimit-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/algorithm.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/algorithm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC, abstractmethod
 from upstash_redis.asyncio import Redis
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.config import SDK, PREFIX
 from upstash_ratelimit.schema.response import RateLimitResponse
 from asyncio import sleep
 from time import time_ns
 
 
 # TODO might delete this
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/fixed_window_core.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/fixed_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/sliding_window_core.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/sliding_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/algorithms/token_bucket_core.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/algorithms/token_bucket_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/async_blocker.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/async_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/fixed_window.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/fixed_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from distutils.sysconfig import PREFIX
 from typing import Literal
 from upstash_redis.asyncio import Redis
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.algorithms.fixed_window_core import FixedWindowCore
 from upstash_ratelimit.config import SDK
 from upstash_ratelimit.asyncio.async_blocker import AsyncBlocker
 from upstash_ratelimit.schema.response import RateLimitResponse
 
 
 class FixedWindow(FixedWindowCore, AsyncBlocker):
@@ -29,19 +28,17 @@
         :param window: the number of time units in which requests are limited
         :param unit: the shorthand version of the time measuring unit
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
-
         super().__init__(
             max_number_of_requests=max_number_of_requests,
             window=window,
             unit=unit,
             prefix=prefix,
         )
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/limiter.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/limiter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from upstash_ratelimit.config import PREFIX
 from upstash_redis.asyncio import Redis
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.config import SDK, PREFIX
 from typing import Literal, Optional
 from upstash_ratelimit.asyncio.fixed_window import FixedWindow
 from upstash_ratelimit.asyncio.sliding_window import SlidingWindow
 from upstash_ratelimit.asyncio.token_bucket import TokenBucket
 
 
@@ -18,20 +17,18 @@
         :param redis: the Redis client that will be used to execute the algorithm's commands. If not given, will read from env variables `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN`
         :param prefix: a prefix to distinguish between the keys used for rate limiting and others
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
         self.prefix = prefix
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
-
     def fixed_window(
         self,
         max_number_of_requests: int,
         window: int,
         unit: Literal["ms", "s", "m", "h", "d"] = "ms",
     ) -> FixedWindow:
         """
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/sliding_window.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/sliding_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import ClassVar, Literal
 from upstash_redis.asyncio import Redis
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.algorithms.sliding_window_core import SlidingWindowCore
 from upstash_ratelimit.asyncio.async_blocker import AsyncBlocker
 from upstash_ratelimit.utils.time import to_milliseconds
 from upstash_ratelimit.config import PREFIX, SDK
 from upstash_ratelimit.schema.response import RateLimitResponse
 from time import time_ns
 from math import floor
@@ -33,19 +32,17 @@
         :param window: the number of time units in which requests are limited
         :param unit: the shorthand version of the time measuring unit
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
-
         super().__init__(
             max_number_of_requests=max_number_of_requests,
             window=window,
             unit=unit,
             prefix=prefix,
         )
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/asyncio/token_bucket.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/asyncio/token_bucket.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Literal
 from upstash_redis.asyncio import Redis
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.algorithms.token_bucket_core import TokenBucketCore
 from upstash_ratelimit.asyncio.async_blocker import AsyncBlocker
 from upstash_ratelimit.config import PREFIX, SDK
 from upstash_ratelimit.schema.response import RateLimitResponse
 from math import floor
 
 
@@ -32,19 +31,17 @@
         :param interval: the number of time units between each refill
         :param unit: the shorthand version of the time measuring unit
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
-
         super().__init__(
             max_number_of_tokens=max_number_of_tokens,
             refill_rate=refill_rate,
             interval=interval,
             unit=unit,
             prefix=prefix,
         )
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/limiter.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/sync/token_bucket.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,87 @@
-from upstash_ratelimit.config import PREFIX
+from typing import Literal
 from upstash_redis import Redis
-from upstash_redis.schema.telemetry import TelemetryData
-from upstash_ratelimit.config import SDK, PREFIX
-from typing import Literal, Optional
+from upstash_ratelimit.algorithms.token_bucket_core import TokenBucketCore
+from upstash_ratelimit.sync.sync_blocker import SyncBlocker
+from upstash_ratelimit.config import PREFIX, SDK
+from upstash_ratelimit.schema.response import RateLimitResponse
 
-from upstash_ratelimit.sync.fixed_window import FixedWindow
-from upstash_ratelimit.sync.sliding_window import SlidingWindow
-from upstash_ratelimit.sync.token_bucket import TokenBucket
 
-
-class RateLimit:
+class TokenBucket(TokenBucketCore, SyncBlocker):
     """
-    A class that incorporates all the algorithms to provide a smoother initialisation experience.
+    A bucket is filled with "max_number_of_tokens" that refill at "refill_rate" per "interval".
+    Each request tries to consume one token and if the bucket is empty, the request is rejected.
     """
 
-    def __init__(self, redis: Optional[Redis] = None, prefix: str = PREFIX):
+    def __init__(
+        self,
+        redis: Redis,
+        max_number_of_tokens: int,
+        refill_rate: int,
+        interval: int,
+        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
+        prefix: str = PREFIX,
+    ):
         """
         :param redis: the Redis client that will be used to execute the algorithm's commands. If not given, will read from env variables `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN`
         :param prefix: a prefix to distinguish between the keys used for rate limiting and others
+
+        :param max_number_of_tokens: the maximum number of tokens that can be stored in the bucket
+        :param refill_rate: the number of tokens that are refilled per interval
+        :param interval: the number of time units between each refill
+        :param unit: the shorthand version of the time measuring unit
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
-        self.prefix = prefix
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
+        super().__init__(
+            max_number_of_tokens=max_number_of_tokens,
+            refill_rate=refill_rate,
+            interval=interval,
+            unit=unit,
+            prefix=prefix,
+        )
 
-    def fixed_window(
-        self,
-        max_number_of_requests: int,
-        window: int,
-        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
-    ) -> FixedWindow:
+    def limit(self, identifier: str) -> RateLimitResponse:
         """
-        The time is divided into windows of fixed length and each window has a maximum number of allowed requests.
-
-        :param max_number_of_requests: the number of requests allowed within the window
-        :param window: the number of time units in which requests are limited
-        :param unit: the shorthand version of the time measuring unit
+        Increment identifier's request counter, determine whether it should pass
+        and return additional metadata.
         """
+        remaining_tokens, next_refill_at = self.redis.eval(
+            script=TokenBucketCore.script,
+            keys=[self.get_key(identifier)],
+            args=[
+                self.max_number_of_tokens,
+                self.interval,
+                self.refill_rate,
+                self.current_time_in_milliseconds,
+            ],
+        )
 
-        return FixedWindow(
-            self.redis, max_number_of_requests, window, unit, self.prefix
+        return super().limit(
+            remaining_tokens=remaining_tokens, next_refill_at=next_refill_at
         )
 
-    def sliding_window(
-        self,
-        max_number_of_requests: int,
-        window: int,
-        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
-    ) -> SlidingWindow:
+    def remaining(self, identifier: str) -> int:
         """
-        Combined approach of sliding logs and fixed window with lower storage
-        costs than sliding logs and improved boundary behavior by calculating a
-        weighted score between two windows.
-
-        :param max_number_of_requests: the number of requests allowed within the window
-        :param window: the number of time units in which requests are limited
-        :param unit: the shorthand version of the time measuring unit
+        Determine the number of identifier's remaining requests.
         """
+        bucket = self.redis.hmget(self.get_key(identifier), "updated_at", "tokens")
 
-        return SlidingWindow(
-            self.redis, max_number_of_requests, window, unit, self.prefix
-        )
+        return super().remaining(bucket=bucket)
 
-    def token_bucket(
-        self,
-        max_number_of_tokens: int,
-        refill_rate: int,
-        interval: int,
-        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
-    ) -> TokenBucket:
+    def reset(self, identifier: str) -> int:
         """
-        A bucket is filled with "max_number_of_tokens" that refill at "refill_rate" per "interval".
-        Each request tries to consume one token and if the bucket is empty, the request is rejected.
+        Determine the unix time in milliseconds when the next window begins.
 
-        :param max_number_of_tokens: the maximum number of tokens that the bucket can hold
-        :param refill_rate: the number of tokens that are refilled per interval
-        :param interval: the number of time units between each refill
-        :param unit: the shorthand version of the time measuring unit
+        If the identifier is not rate-limited, the returned value will be -1.
         """
+        updated_at = self.redis.hget(self.get_key(identifier), "updated_at")
 
-        return TokenBucket(
-            self.redis,
-            max_number_of_tokens,
-            refill_rate,
-            interval,
-            unit,
-            self.prefix,
-        )
+        return super().reset(updated_at=updated_at)
+
+    def get_key(self, identifier):
+        return f"{self.prefix}:{identifier}"
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/sync/fixed_window.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/sync/fixed_window.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from distutils.sysconfig import PREFIX
 from typing import Literal
 from upstash_redis import Redis
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.algorithms.fixed_window_core import FixedWindowCore
 from upstash_ratelimit.config import SDK
 from upstash_ratelimit.sync.sync_blocker import SyncBlocker
 from upstash_ratelimit.schema.response import RateLimitResponse
 
 
 class FixedWindow(FixedWindowCore, SyncBlocker):
@@ -29,19 +28,17 @@
         :param window: the number of time units in which requests are limited
         :param unit: the shorthand version of the time measuring unit
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
-
         super().__init__(
             max_number_of_requests=max_number_of_requests,
             window=window,
             unit=unit,
             prefix=prefix,
         )
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/sync/sliding_window.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/sync/sliding_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Literal
 from upstash_redis import Redis
-from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.algorithms.sliding_window_core import SlidingWindowCore
 from upstash_ratelimit.config import PREFIX, SDK
 from upstash_ratelimit.schema.response import RateLimitResponse
 from upstash_ratelimit.sync.sync_blocker import SyncBlocker
 
 
 class SlidingWindow(SlidingWindowCore, SyncBlocker):
@@ -30,19 +29,17 @@
         :param window: the number of time units in which requests are limited
         :param unit: the shorthand version of the time measuring unit
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
-
         super().__init__(
             max_number_of_requests=max_number_of_requests,
             window=window,
             unit=unit,
             prefix=prefix,
         )
```

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/sync/sync_blocker.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/sync/sync_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.4.1/upstash_ratelimit/sync/token_bucket.py` & `upstash_ratelimit-0.4.2/upstash_ratelimit/limiter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,91 @@
-from typing import Literal
+from upstash_ratelimit.config import PREFIX
 from upstash_redis import Redis
-from upstash_redis.schema.telemetry import TelemetryData
-from upstash_ratelimit.algorithms.token_bucket_core import TokenBucketCore
-from upstash_ratelimit.sync.sync_blocker import SyncBlocker
-from upstash_ratelimit.config import PREFIX, SDK
-from upstash_ratelimit.schema.response import RateLimitResponse
+from upstash_ratelimit.config import SDK, PREFIX
+from typing import Literal, Optional
 
+from upstash_ratelimit.sync.fixed_window import FixedWindow
+from upstash_ratelimit.sync.sliding_window import SlidingWindow
+from upstash_ratelimit.sync.token_bucket import TokenBucket
 
-class TokenBucket(TokenBucketCore, SyncBlocker):
+
+class RateLimit:
     """
-    A bucket is filled with "max_number_of_tokens" that refill at "refill_rate" per "interval".
-    Each request tries to consume one token and if the bucket is empty, the request is rejected.
+    A class that incorporates all the algorithms to provide a smoother initialisation experience.
     """
 
-    def __init__(
-        self,
-        redis: Redis,
-        max_number_of_tokens: int,
-        refill_rate: int,
-        interval: int,
-        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
-        prefix: str = PREFIX,
-    ):
+    def __init__(self, redis: Optional[Redis] = None, prefix: str = PREFIX):
         """
         :param redis: the Redis client that will be used to execute the algorithm's commands. If not given, will read from env variables `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN`
         :param prefix: a prefix to distinguish between the keys used for rate limiting and others
-
-        :param max_number_of_tokens: the maximum number of tokens that can be stored in the bucket
-        :param refill_rate: the number of tokens that are refilled per interval
-        :param interval: the number of time units between each refill
-        :param unit: the shorthand version of the time measuring unit
         """
 
         if redis is None:
             redis = Redis.from_env()
 
+        redis._headers["Upstash-Telemetry-Sdk"] = "upstash_ratelimit@python"
         self.redis = redis
+        self.prefix = prefix
 
-        if redis.allow_telemetry:
-            self.redis.telemetry_data = TelemetryData(sdk=SDK)
-
-        super().__init__(
-            max_number_of_tokens=max_number_of_tokens,
-            refill_rate=refill_rate,
-            interval=interval,
-            unit=unit,
-            prefix=prefix,
-        )
-
-    def limit(self, identifier: str) -> RateLimitResponse:
+    def fixed_window(
+        self,
+        max_number_of_requests: int,
+        window: int,
+        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
+    ) -> FixedWindow:
         """
-        Increment identifier's request counter, determine whether it should pass
-        and return additional metadata.
+        The time is divided into windows of fixed length and each window has a maximum number of allowed requests.
+
+        :param max_number_of_requests: the number of requests allowed within the window
+        :param window: the number of time units in which requests are limited
+        :param unit: the shorthand version of the time measuring unit
         """
-        remaining_tokens, next_refill_at = self.redis.eval(
-            script=TokenBucketCore.script,
-            keys=[self.get_key(identifier)],
-            args=[
-                self.max_number_of_tokens,
-                self.interval,
-                self.refill_rate,
-                self.current_time_in_milliseconds,
-            ],
-        )
 
-        return super().limit(
-            remaining_tokens=remaining_tokens, next_refill_at=next_refill_at
+        return FixedWindow(
+            self.redis, max_number_of_requests, window, unit, self.prefix
         )
 
-    def remaining(self, identifier: str) -> int:
+    def sliding_window(
+        self,
+        max_number_of_requests: int,
+        window: int,
+        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
+    ) -> SlidingWindow:
         """
-        Determine the number of identifier's remaining requests.
+        Combined approach of sliding logs and fixed window with lower storage
+        costs than sliding logs and improved boundary behavior by calculating a
+        weighted score between two windows.
+
+        :param max_number_of_requests: the number of requests allowed within the window
+        :param window: the number of time units in which requests are limited
+        :param unit: the shorthand version of the time measuring unit
         """
-        bucket = self.redis.hmget(self.get_key(identifier), "updated_at", "tokens")
 
-        return super().remaining(bucket=bucket)
+        return SlidingWindow(
+            self.redis, max_number_of_requests, window, unit, self.prefix
+        )
 
-    def reset(self, identifier: str) -> int:
+    def token_bucket(
+        self,
+        max_number_of_tokens: int,
+        refill_rate: int,
+        interval: int,
+        unit: Literal["ms", "s", "m", "h", "d"] = "ms",
+    ) -> TokenBucket:
         """
-        Determine the unix time in milliseconds when the next window begins.
+        A bucket is filled with "max_number_of_tokens" that refill at "refill_rate" per "interval".
+        Each request tries to consume one token and if the bucket is empty, the request is rejected.
 
-        If the identifier is not rate-limited, the returned value will be -1.
+        :param max_number_of_tokens: the maximum number of tokens that the bucket can hold
+        :param refill_rate: the number of tokens that are refilled per interval
+        :param interval: the number of time units between each refill
+        :param unit: the shorthand version of the time measuring unit
         """
-        updated_at = self.redis.hget(self.get_key(identifier), "updated_at")
 
-        return super().reset(updated_at=updated_at)
-
-    def get_key(self, identifier):
-        return f"{self.prefix}:{identifier}"
+        return TokenBucket(
+            self.redis,
+            max_number_of_tokens,
+            refill_rate,
+            interval,
+            unit,
+            self.prefix,
+        )
```

### Comparing `upstash_ratelimit-0.4.1/PKG-INFO` & `upstash_ratelimit-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit
-Version: 0.4.1
+Version: 0.4.2
 Summary: Serverless ratelimiting package from Upstash
 Author: Upstash
 Author-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

