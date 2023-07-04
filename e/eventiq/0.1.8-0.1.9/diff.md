# Comparing `tmp/eventiq-0.1.8.tar.gz` & `tmp/eventiq-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventiq-0.1.8.tar", max compression
+gzip compressed data, was "eventiq-0.1.9.tar", max compression
```

## Comparing `eventiq-0.1.8.tar` & `eventiq-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    11357 2023-05-15 09:46:25.698861 eventiq-0.1.8/LICENSE
--rw-r--r--   0        0        0     4649 2023-05-15 09:46:25.698861 eventiq-0.1.8/README.md
--rw-r--r--   0        0        0      772 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/__init__.py
--rw-r--r--   0        0        0       59 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/__main__.py
--rw-r--r--   0        0        0       22 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/_version.py
--rw-r--r--   0        0        0      171 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/asyncapi/__init__.py
--rw-r--r--   0        0        0     2636 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/asyncapi/generator.py
--rw-r--r--   0        0        0     1579 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/asyncapi/models.py
--rw-r--r--   0        0        0      426 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/asyncapi/registry.py
--rw-r--r--   0        0        0        0 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/__init__.py
--rw-r--r--   0        0        0       59 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/kafka/__init__.py
--rw-r--r--   0        0        0     3678 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/kafka/broker.py
--rw-r--r--   0        0        0      482 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/kafka/settings.py
--rw-r--r--   0        0        0      163 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/nats/__init__.py
--rw-r--r--   0        0        0     5737 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/nats/broker.py
--rw-r--r--   0        0        0     2809 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/nats/plugins.py
--rw-r--r--   0        0        0      617 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/nats/settings.py
--rw-r--r--   0        0        0       61 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/pubsub/__init__.py
--rw-r--r--   0        0        0     2474 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/pubsub/broker.py
--rw-r--r--   0        0        0      179 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/pubsub/settings.py
--rw-r--r--   0        0        0       65 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/rabbitmq/__init__.py
--rw-r--r--   0        0        0     5382 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/rabbitmq/broker.py
--rw-r--r--   0        0        0      816 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/rabbitmq/middlewares.py
--rw-r--r--   0        0        0      437 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/rabbitmq/settings.py
--rw-r--r--   0        0        0      121 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/redis/__init__.py
--rw-r--r--   0        0        0     1894 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/redis/broker.py
--rw-r--r--   0        0        0     1767 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/redis/plugins.py
--rw-r--r--   0        0        0      305 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/redis/settings.py
--rw-r--r--   0        0        0     2004 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/backends/stub.py
--rw-r--r--   0        0        0     8596 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/broker.py
--rw-r--r--   0        0        0     2466 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/cli.py
--rw-r--r--   0        0        0        0 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/config/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/config/factory.py
--rw-r--r--   0        0        0     1824 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/config/models.py
--rw-r--r--   0        0        0      226 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/config/settings.py
--rw-r--r--   0        0        0     4206 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/consumer.py
--rw-r--r--   0        0        0      558 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/context.py
--rw-r--r--   0        0        0        0 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/contrib/__init__.py
--rw-r--r--   0        0        0     1443 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/contrib/fastapi.py
--rw-r--r--   0        0        0      282 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/encoders/__init__.py
--rw-r--r--   0        0        0      670 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/encoders/json.py
--rw-r--r--   0        0        0      706 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/encoders/msgpack.py
--rw-r--r--   0        0        0      645 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/encoders/orjson.py
--rw-r--r--   0        0        0      494 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/encoders/pickle.py
--rw-r--r--   0        0        0      873 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/exceptions.py
--rw-r--r--   0        0        0     1148 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/logger.py
--rw-r--r--   0        0        0      784 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/message.py
--rw-r--r--   0        0        0     3333 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middleware.py
--rw-r--r--   0        0        0      354 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middlewares/__init__.py
--rw-r--r--   0        0        0      871 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middlewares/debug.py
--rw-r--r--   0        0        0      860 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middlewares/error.py
--rw-r--r--   0        0        0     1729 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middlewares/healthcheck.py
--rw-r--r--   0        0        0     4435 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middlewares/opentelemetry.py
--rw-r--r--   0        0        0     5115 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middlewares/prometheus.py
--rw-r--r--   0        0        0     3926 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/middlewares/retries.py
--rw-r--r--   0        0        0     2519 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/models.py
--rw-r--r--   0        0        0      585 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/plugins.py
--rw-r--r--   0        0        0        0 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/py.typed
--rw-r--r--   0        0        0      740 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/runner.py
--rw-r--r--   0        0        0     4045 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/service.py
--rw-r--r--   0        0        0      643 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/settings.py
--rw-r--r--   0        0        0     1253 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/types.py
--rw-r--r--   0        0        0      216 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/utils/__init__.py
--rw-r--r--   0        0        0      192 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/utils/datetime.py
--rw-r--r--   0        0        0      390 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/utils/enum.py
--rw-r--r--   0        0        0     1862 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/utils/functools.py
--rw-r--r--   0        0        0     1106 2023-05-15 09:46:25.702861 eventiq-0.1.8/eventiq/utils/imports.py
--rw-r--r--   0        0        0     4258 2023-05-15 09:46:25.706861 eventiq-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 eventiq-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 08:19:29.686056 eventiq-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4649 2023-05-16 08:19:29.686056 eventiq-0.1.9/README.md
+-rw-r--r--   0        0        0      772 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/_version.py
+-rw-r--r--   0        0        0      171 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3358 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/asyncapi/generator.py
+-rw-r--r--   0        0        0     2207 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/asyncapi/models.py
+-rw-r--r--   0        0        0      440 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/asyncapi/registry.py
+-rw-r--r--   0        0        0        0 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/kafka/__init__.py
+-rw-r--r--   0        0        0     3839 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/kafka/broker.py
+-rw-r--r--   0        0        0      482 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/kafka/settings.py
+-rw-r--r--   0        0        0      163 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/nats/__init__.py
+-rw-r--r--   0        0        0     5822 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/nats/broker.py
+-rw-r--r--   0        0        0     2809 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/nats/plugins.py
+-rw-r--r--   0        0        0      617 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/nats/settings.py
+-rw-r--r--   0        0        0       61 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/pubsub/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/pubsub/broker.py
+-rw-r--r--   0        0        0      179 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/pubsub/settings.py
+-rw-r--r--   0        0        0       65 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     5430 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/rabbitmq/broker.py
+-rw-r--r--   0        0        0      816 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/rabbitmq/middlewares.py
+-rw-r--r--   0        0        0      437 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/rabbitmq/settings.py
+-rw-r--r--   0        0        0      121 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/redis/__init__.py
+-rw-r--r--   0        0        0     1941 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/redis/broker.py
+-rw-r--r--   0        0        0     1767 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/redis/plugins.py
+-rw-r--r--   0        0        0      305 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/redis/settings.py
+-rw-r--r--   0        0        0     2157 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/backends/stub.py
+-rw-r--r--   0        0        0     9287 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/broker.py
+-rw-r--r--   0        0        0     2466 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/cli.py
+-rw-r--r--   0        0        0        0 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/config/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/config/factory.py
+-rw-r--r--   0        0        0     1824 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/config/models.py
+-rw-r--r--   0        0        0      226 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/config/settings.py
+-rw-r--r--   0        0        0     4206 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/consumer.py
+-rw-r--r--   0        0        0      558 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/context.py
+-rw-r--r--   0        0        0        0 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/contrib/__init__.py
+-rw-r--r--   0        0        0     1443 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/contrib/fastapi.py
+-rw-r--r--   0        0        0      282 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/encoders/__init__.py
+-rw-r--r--   0        0        0      670 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/encoders/json.py
+-rw-r--r--   0        0        0      706 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/encoders/msgpack.py
+-rw-r--r--   0        0        0      645 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/encoders/orjson.py
+-rw-r--r--   0        0        0      494 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/encoders/pickle.py
+-rw-r--r--   0        0        0      873 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/exceptions.py
+-rw-r--r--   0        0        0     1148 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/logger.py
+-rw-r--r--   0        0        0      784 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/message.py
+-rw-r--r--   0        0        0     3333 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middleware.py
+-rw-r--r--   0        0        0      354 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middlewares/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middlewares/debug.py
+-rw-r--r--   0        0        0      860 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middlewares/error.py
+-rw-r--r--   0        0        0     1729 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middlewares/healthcheck.py
+-rw-r--r--   0        0        0     4743 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middlewares/opentelemetry.py
+-rw-r--r--   0        0        0     5115 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middlewares/prometheus.py
+-rw-r--r--   0        0        0     3926 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/middlewares/retries.py
+-rw-r--r--   0        0        0     2729 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/models.py
+-rw-r--r--   0        0        0      585 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/py.typed
+-rw-r--r--   0        0        0      740 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/runner.py
+-rw-r--r--   0        0        0     4141 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/service.py
+-rw-r--r--   0        0        0      503 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/settings.py
+-rw-r--r--   0        0        0     1391 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/types.py
+-rw-r--r--   0        0        0      216 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/utils/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/utils/datetime.py
+-rw-r--r--   0        0        0      390 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/utils/enum.py
+-rw-r--r--   0        0        0     1862 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/utils/functools.py
+-rw-r--r--   0        0        0     1106 2023-05-16 08:19:29.690056 eventiq-0.1.9/eventiq/utils/imports.py
+-rw-r--r--   0        0        0     4258 2023-05-16 08:19:29.694056 eventiq-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 eventiq-0.1.9/PKG-INFO
```

### Comparing `eventiq-0.1.8/LICENSE` & `eventiq-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/README.md` & `eventiq-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.8
+Version: 0.1.9
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
```

### Comparing `eventiq-0.1.8/eventiq/__init__.py` & `eventiq-0.1.9/eventiq/__init__.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/asyncapi/generator.py` & `eventiq-0.1.9/eventiq/asyncapi/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from eventiq.asyncapi.models import (
     AsyncAPI,
     ChannelItem,
     Components,
     Info,
     Message,
     Operation,
+    Parameter,
     PayloadRef,
 )
 
+from ..broker import TOPIC_PATTERN
 from ..service import Service
 from .registry import PUBLISH_REGISTRY
 
 PREFIX = "#/components/schemas/"
 
 
 def normalize(v: str) -> str:
@@ -32,19 +34,31 @@
     all_models = [
         m.event_type  # type: ignore
         for m in chain(service.consumers.values(), PUBLISH_REGISTRY.values())
     ]
     return all_schemas(all_models, ref_prefix=PREFIX).get("definitions", [])
 
 
+def get_topic_parameters(topic: str, **kwargs) -> dict[str, Parameter]:
+    params = {}
+    for k in topic.split("."):
+        if TOPIC_PATTERN.fullmatch(k):
+            param_name = k[1:-1]
+            params[param_name] = kwargs.get(param_name, Parameter())
+    return params
+
+
 def populate_channel_spec(service: Service):
     channels: dict[str, ChannelItem] = defaultdict(ChannelItem)
     # tags = {t["name"]: Tag(**t) for t in service.tags_metadata}
 
     for publishes in PUBLISH_REGISTRY.values():
+        params = get_topic_parameters(publishes.topic, **publishes.kwargs)
+        for k, v in params.items():
+            channels[publishes.topic].parameters.setdefault(k, v)
         channels[publishes.topic].publish = Operation(
             message=Message(
                 message_id=normalize(f"{service.name}_{publishes.event_type.__name__}"),
                 content_type=service.broker.encoder.CONTENT_TYPE,
                 payload=PayloadRef(ref=f"{PREFIX}{publishes.event_type.__name__}"),
                 description=publishes.kwargs.get("description", ""),
             )
@@ -56,14 +70,19 @@
                 message_id=normalize(f"{consumer.name}_{consumer.event_type.__name__}"),
                 content_type=service.broker.encoder.CONTENT_TYPE,
                 payload=PayloadRef(ref=f"{PREFIX}{consumer.event_type.__name__}"),
                 description=consumer.description,
             )
         )
         channels[consumer.topic].subscribe = subscribe
+        params = get_topic_parameters(
+            consumer.topic, **consumer.options.get("params", {})
+        )
+        for k, v in params.items():
+            channels[consumer.topic].parameters.setdefault(k, v)
     return channels
 
 
 @functools.lru_cache
 def get_async_api_spec(service: Service) -> AsyncAPI:
     channels = populate_channel_spec(service)
     definitions = get_all_models_schema(service)
```

### Comparing `eventiq-0.1.8/eventiq/asyncapi/models.py` & `eventiq-0.1.9/eventiq/asyncapi/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Optional, Type
 
 from pydantic import BaseModel as _BaseModel
-from pydantic import Field
+from pydantic import Field, validator
 
 from eventiq.models import CloudEvent
 
 
 class BaseModel(_BaseModel):
     class Config:
         allow_population_by_field_name = True
@@ -13,17 +13,27 @@
 
 class Info(BaseModel):
     title: str
     version: str
 
 
 class PublishInfo(BaseModel):
-    topic: str
     event_type: Type[CloudEvent]
-    kwargs: Dict[str, Any]
+    topic: str
+    kwargs: Dict[str, Any] = {}
+
+    @validator("topic", always=True, pre=True, allow_reuse=True)
+    def set_default_topic(cls, v, values):
+        if v is None:
+            v = values["event_type"].__fields__["topic"].get_default()
+        return v
+
+    @classmethod
+    def s(cls, even_type: Type[CloudEvent], topic: Optional[str] = None, **kwargs: Any):
+        return cls(event_type=even_type, topic=topic, **kwargs)
 
 
 class PayloadRef(BaseModel):
     ref: str = Field(..., alias="$ref")
 
 
 class Message(BaseModel):
@@ -35,17 +45,24 @@
 
 
 class Operation(BaseModel):
     summary: Optional[str] = None
     message: Message
 
 
+class Parameter(BaseModel):
+    description: Optional[str] = None
+    param_schema: Dict[str, Any] = Field({"type": "string"}, alias="schema")
+    location: Optional[str] = None
+
+
 class ChannelItem(BaseModel):
     publish: Optional[Operation] = None
     subscribe: Optional[Operation] = None
+    parameters: Dict[str, Parameter] = {}
 
 
 class Server(BaseModel):
     url: Optional[str] = None
     protocol: str
     description: Optional[str] = None
```

### Comparing `eventiq-0.1.8/eventiq/backends/kafka/broker.py` & `eventiq-0.1.9/eventiq/backends/kafka/broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     Kafka backend
     :param bootstrap_servers: url or list of kafka servers
     :param publisher_options: extra options for AIOKafkaProducer
     :param consumer_options: extra options (defaults) for AIOKafkaConsumer
     :param kwargs: Broker base class parameters
     """
 
+    WILDCARD_MANY = "*"
+    WILDCARD_ONE = r"\w+"
+
     Settings = KafkaSettings
     protocol = "kafka"
 
     def __init__(
         self,
         *,
         bootstrap_servers: str | list[str],
@@ -47,33 +50,35 @@
     @property
     def is_connected(self) -> bool:
         return True
 
     async def _start_consumer(self, service: Service, consumer: Consumer) -> None:
         handler = self.get_handler(service, consumer)
         subscriber = aiokafka.AIOKafkaConsumer(
-            consumer.topic,
             group_id=f"{service.name}:{consumer.name}",
             bootstrap_servers=self.bootstrap_servers,
             enable_auto_commit=False,
             **consumer.options.get("kafka_consumer_options", self._consumer_options),
         )
         await subscriber.start()
+        subscriber.subscribe(pattern=self.format_topic(consumer.topic))
         while self._stopped:
             result = await subscriber.getmany(
                 timeout_ms=consumer.options.get("timeout_ms", 600)
             )
             for tp, messages in result.items():
 
                 if messages:
                     tasks: list[asyncio.Task] = [
                         asyncio.create_task(handler(message)) for message in messages  # type: ignore
                     ]
                     await asyncio.gather(*tasks, return_exceptions=True)
                     await subscriber.commit({tp: messages[-1].offset + 1})
+        if consumer.dynamic:
+            subscriber.unsubscribe()
 
     async def _disconnect(self):
         if self._publisher:
             await self._publisher.stop()
 
     @property
     def publisher(self) -> aiokafka.AIOKafkaProducer:
```

### Comparing `eventiq-0.1.8/eventiq/backends/nats/broker.py` & `eventiq-0.1.9/eventiq/backends/nats/broker.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     :param url: Url to nats server(s)
     :param connection_options: additional connection options passed to nats.connect(...)
     :param auto_flush: auto flush messages on publish
     :param kwargs: options for base class
     """
 
     protocol = "nats"
+    WILDCARD_ONE = "*"
+    WILDCARD_MANY = ">"
 
     def __init__(
         self,
         *,
         url: str = "nats://localhost:4444",
         connection_options: dict[str, Any] | None = None,
         auto_flush: bool = True,
@@ -55,15 +57,15 @@
         return NatsMessageProxy
 
     def parse_incoming_message(self, message: NatsMsg) -> Any:
         return self.encoder.decode(message.data)
 
     async def _start_consumer(self, service: Service, consumer: Consumer) -> None:
         await self.client.subscribe(
-            subject=consumer.topic,
+            subject=self.format_topic(consumer.topic),
             queue=f"{service.name}:{consumer.name}",
             cb=self.get_handler(service, consumer),
         )
 
     async def _disconnect(self) -> None:
         await self.client.close()
 
@@ -137,15 +139,15 @@
         except Exception as e:
             raise PublishError from e
 
     async def _start_consumer(self, service: Service, consumer: Consumer) -> None:
         durable = f"{service.name}:{consumer.name}"
         try:
             subscription = await self.js.pull_subscribe(
-                subject=consumer.topic,
+                subject=self.format_topic(consumer.topic),
                 durable=durable,
                 config=consumer.options.get("config"),
             )
         except Exception as e:
             self.logger.exception(
                 f"Error creating subscription for consumer {consumer.name} and topic {consumer.topic}",
                 exc_info=e,
```

### Comparing `eventiq-0.1.8/eventiq/backends/nats/plugins.py` & `eventiq-0.1.9/eventiq/backends/nats/plugins.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/backends/nats/settings.py` & `eventiq-0.1.9/eventiq/backends/nats/settings.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/backends/pubsub/broker.py` & `eventiq-0.1.9/eventiq/backends/pubsub/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     Google Cloud Pub/Sub broker implementation
     :param service_file: path to the service account (json) file
     :param kwargs: Broker base class parameters
     """
 
     Settings = PubSubSettings
 
+    WILDCARD_ONE = "*"
+    WILDCARD_MANY = "*"
+
     def __init__(
         self,
         *,
         service_file: str,
         **kwargs: Any,
     ) -> None:
```

### Comparing `eventiq-0.1.8/eventiq/backends/rabbitmq/broker.py` & `eventiq-0.1.9/eventiq/backends/rabbitmq/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     :param exchange_name: global exchange name
     :param connection_options: additional connection options passed to aio_pika.connect_robust
     :param kwargs: Broker base class parameters
     """
 
     Settings = RabbitMQSettings
 
+    WILDCARD_ONE = "*"
+    WILDCARD_MANY = "#"
+
     def __init__(
         self,
         *,
         url: str,
         default_prefetch_count: int = 10,
         queue_options: dict[str, Any] | None = None,
         exchange_name: str = "events",
```

### Comparing `eventiq-0.1.8/eventiq/backends/rabbitmq/middlewares.py` & `eventiq-0.1.9/eventiq/backends/rabbitmq/middlewares.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/backends/redis/broker.py` & `eventiq-0.1.9/eventiq/backends/redis/broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     """
     Broker implementation based on redis PUB/SUB and aioredis package
     :param url: connection string to redis
     :param connect_options: additional connection options passed to aioredis.from_url
     :param kwargs: base class arguments
     """
 
+    WILDCARD_ONE = "*"
+    WILDCARD_MANY = "*"
     Settings = RedisSettings
 
     def __init__(
         self,
         *,
         url: str,
         connect_options: dict[str, Any] | None = None,
```

### Comparing `eventiq-0.1.8/eventiq/backends/redis/plugins.py` & `eventiq-0.1.9/eventiq/backends/redis/plugins.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/backends/stub.py` & `eventiq-0.1.9/eventiq/backends/stub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import re
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any
 
 from eventiq.broker import Broker
 from eventiq.middleware import Middleware
 
@@ -21,14 +22,17 @@
 
 
 class StubBroker(Broker[StubMessage]):
     """This is in-memory implementation of a broker class, mainly designed for testing."""
 
     protocol = "in-memory"
 
+    WILDCARD_ONE = r"\w+"
+    WILDCARD_MANY = "*"
+
     def __init__(
         self,
         *,
         encoder: Encoder | None = None,
         middlewares: list[Middleware] | None = None,
         **options: Any,
     ) -> None:
@@ -39,28 +43,29 @@
     def parse_incoming_message(self, message: StubMessage) -> Any:
         return self.encoder.decode(message.data)
 
     async def _disconnect(self) -> None:
         self._stopped = True
 
     async def _start_consumer(self, service: Service, consumer: Consumer):
-        queue = self.topics[consumer.topic]
+        queue = self.topics[self.format_topic(consumer.topic)]
         handler = self.get_handler(service, consumer)
         while not self._stopped:
             message = await queue.get()
             await handler(message)
 
     async def _connect(self) -> None:
         pass
 
     async def _publish(self, message: CloudEvent, **_) -> None:
-        queue = self.topics[message.topic]
         data = self.encoder.encode(message.dict())
-        msg = StubMessage(data=data, queue=queue)
-        await queue.put(msg)
+        for topic, queue in self.topics.items():
+            if re.fullmatch(topic, message.topic):
+                msg = StubMessage(data=data, queue=queue)
+                await queue.put(msg)
 
     async def _ack(self, message: Message) -> None:
         message.queue.task_done()
 
     async def _nack(self, message: Message) -> None:
         await message.queue.put(message)
```

### Comparing `eventiq-0.1.8/eventiq/broker.py` & `eventiq-0.1.9/eventiq/broker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 from __future__ import annotations
 
 import asyncio
+import os
+import re
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Awaitable, Callable, Generic, Type, cast
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Generic
 
 from pydantic import ValidationError
 
 from .context import _current_message, _current_service
 from .exceptions import DecodeError, Fail, Skip
 from .logger import LoggerMixin
 from .message import Message
 from .middleware import Middleware
 from .models import CloudEvent
 from .settings import BrokerSettings
 from .types import Encoder, RawMessage
+from .utils.imports import import_from_string
 
 if TYPE_CHECKING:
     from eventiq import Consumer, Service
 
+TOPIC_PATTERN = re.compile(r"{\w+}")
+
 
 class Broker(Generic[RawMessage], LoggerMixin, ABC):
     """Base broker class
     :param description: Broker (Server) Description
     :param encoder: Encoder (Serializer) class
     :param middlewares: Optional list of middlewares
     """
 
     protocol: str
     Settings = BrokerSettings
 
+    WILDCARD_ONE: str
+    WILDCARD_MANY: str
+
     def __init__(
         self,
         *,
         description: str | None = None,
         encoder: Encoder | None = None,
         middlewares: list[Middleware] | None = None,
     ) -> None:
@@ -193,25 +201,31 @@
         await self._dispatch(f"before_{event}", *args, **kwargs)
 
     async def dispatch_after(self, event: str, *args, **kwargs) -> None:
         await self._dispatch(f"after_{event}", *args, **kwargs)
 
     @classmethod
     def from_settings(cls, settings: BrokerSettings, **kwargs: Any) -> Broker:
-        broker_class: type[Broker] = cast(Type[Broker], settings.broker_class)
-        kw = settings.dict(exclude={"broker_class"})
-        kw.update(kwargs)
-        return broker_class(**kw)
+        return cls(**settings.dict(), **kwargs)
+
+    @classmethod
+    def _from_env(cls, **kwargs) -> Broker:
+        return cls.from_settings(cls.Settings(**kwargs))
 
     @classmethod
     def from_env(
         cls,
         **kwargs,
     ) -> Broker:
-        return cls.from_settings(BrokerSettings(), **kwargs)
+        if cls == Broker:
+            type_name = os.getenv("BROKER_CLASS", "eventiq.backends.stub:StubBroker")
+            broker_type = import_from_string(type_name)
+        else:
+            broker_type = cls
+        return broker_type._from_env(**kwargs)
 
     @abstractmethod
     def parse_incoming_message(self, message: RawMessage) -> Any:
         raise NotImplementedError
 
     @property
     @abstractmethod
@@ -236,7 +250,18 @@
         raise NotImplementedError
 
     async def _ack(self, message: Message) -> None:
         """Empty default implementation for backends that do not support explicit ack"""
 
     async def _nack(self, message: Message) -> None:
         """Same as for ._ack()"""
+
+    def format_topic(self, topic: str) -> str:
+        result = []
+        for k in topic.split("."):
+            if re.fullmatch(TOPIC_PATTERN, k):
+                result.append(self.WILDCARD_ONE)
+            elif k in {"*", ">"}:
+                result.append(self.WILDCARD_MANY)
+            else:
+                result.append(k)
+        return ".".join(filter(None, result))
```

### Comparing `eventiq-0.1.8/eventiq/cli.py` & `eventiq-0.1.9/eventiq/cli.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/config/factory.py` & `eventiq-0.1.9/eventiq/config/factory.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/config/models.py` & `eventiq-0.1.9/eventiq/config/models.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/consumer.py` & `eventiq-0.1.9/eventiq/consumer.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/context.py` & `eventiq-0.1.9/eventiq/context.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/contrib/fastapi.py` & `eventiq-0.1.9/eventiq/contrib/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/encoders/json.py` & `eventiq-0.1.9/eventiq/encoders/json.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/encoders/msgpack.py` & `eventiq-0.1.9/eventiq/encoders/msgpack.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/encoders/orjson.py` & `eventiq-0.1.9/eventiq/encoders/orjson.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/exceptions.py` & `eventiq-0.1.9/eventiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/logger.py` & `eventiq-0.1.9/eventiq/logger.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/message.py` & `eventiq-0.1.9/eventiq/message.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/middleware.py` & `eventiq-0.1.9/eventiq/middleware.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/middlewares/debug.py` & `eventiq-0.1.9/eventiq/middlewares/debug.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/middlewares/error.py` & `eventiq-0.1.9/eventiq/middlewares/error.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/middlewares/healthcheck.py` & `eventiq-0.1.9/eventiq/middlewares/healthcheck.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/middlewares/opentelemetry.py` & `eventiq-0.1.9/eventiq/middlewares/opentelemetry.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,28 +21,28 @@
     from opentelemetry.sdk.trace import Span, TracerProvider
 
     from eventiq import Broker, Consumer, Service
 
 
 class EventiqGetter(Getter[CloudEvent]):
     def get(self, carrier: CloudEvent, key: str) -> list[str] | None:
-        val = carrier.trace_ctx.get(key, None)
+        val = carrier.tracecontext.get(key, None)
         if val is None:
             return None
         if isinstance(val, Iterable) and not isinstance(val, str):
             return list(val)
         return [val]
 
     def keys(self, carrier: CloudEvent) -> list[str]:
-        return list(carrier.trace_ctx.keys())
+        return list(carrier.tracecontext.keys())
 
 
 class EventiqSetter(Setter[CloudEvent]):
     def set(self, carrier: CloudEvent, key: str, value: str) -> None:
-        carrier.trace_ctx[key] = value
+        carrier.tracecontext[key] = value
 
 
 eventiq_getter = EventiqGetter()
 eventiq_setter = EventiqSetter()
 
 
 class OpenTelemetryMiddleware(Middleware):
@@ -64,33 +64,36 @@
         span = self.tracer.start_span(
             name=f"{service.name}.{consumer.name} receive",
             kind=SpanKind.CONSUMER,
             context=trace_ctx,
             attributes={
                 SpanAttributes.MESSAGING_OPERATION: MessagingOperationValues.PROCESS.value,
                 SpanAttributes.MESSAGING_MESSAGE_ID: str(message.id),
+                SpanAttributes.CLOUDEVENTS_EVENT_SOURCE: message.source
+                or "(anonymous)",
+                SpanAttributes.CLOUDEVENTS_EVENT_TYPE: message.type,
             },
         )
         activation = trace.use_span(span, end_on_exit=True)
         activation.__enter__()
-        self.process_span_registry[(service.name, consumer.name, str(message.id))] = (
+        self.process_span_registry[(service.name, consumer.name, message.id)] = (
             span,
             activation,
         )
 
     async def after_process_message(
         self,
         broker: Broker,
         service: Service,
         consumer: Consumer,
         message: CloudEvent,
         result: Any | None = None,
         exc: Exception | None = None,
     ) -> None:
-        key = (service.name, consumer.name, str(message.id))
+        key = (service.name, consumer.name, message.id)
         span, activation = self.process_span_registry.pop(key, (None, None))
         if span is None or activation is None:
             self.logger.warning("No active span was found")
             return
 
         if span.is_recording():
             status = (StatusCode.ERROR, str(exc)) if exc else (StatusCode.OK,)
@@ -105,14 +108,16 @@
         span = self.tracer.start_span(
             f"{source} publish",
             kind=SpanKind.PRODUCER,
             attributes={
                 SpanAttributes.MESSAGING_MESSAGE_ID: str(message.id),
                 SpanAttributes.MESSAGING_DESTINATION_KIND: MessagingDestinationKindValues.TOPIC.value,
                 SpanAttributes.MESSAGING_DESTINATION: message.topic,
+                SpanAttributes.CLOUDEVENTS_EVENT_SOURCE: source,
+                SpanAttributes.CLOUDEVENTS_EVENT_TYPE: message.type,
             },
         )
         activation = trace.use_span(span, end_on_exit=True)
         activation.__enter__()
         self.publish_span_registry[message.id] = (span, activation)
         inject(message, setter=eventiq_setter)
```

### Comparing `eventiq-0.1.8/eventiq/middlewares/prometheus.py` & `eventiq-0.1.9/eventiq/middlewares/prometheus.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/middlewares/retries.py` & `eventiq-0.1.9/eventiq/middlewares/retries.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/models.py` & `eventiq-0.1.9/eventiq/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime, timedelta
+from functools import partial
 from typing import Any, Dict, Generic, Optional
 
-from pydantic import Extra, Field, validator
+from pydantic import AnyUrl, Extra, Field, validator
 from pydantic.fields import PrivateAttr
 from pydantic.generics import GenericModel
 
 from .context import get_current_service
 from .message import Message
 from .types import ID, D
 from .utils import str_uuid
@@ -17,25 +18,26 @@
     content_type: str = Field("application/json", alias="datacontenttype")
     id: ID = Field(default_factory=str_uuid)
     time: datetime = Field(default_factory=utc_now)
     topic: str = Field(..., alias="subject")
     type: Optional[str] = None
     source: Optional[str] = None
     data: D
-    trace_ctx: Dict[str, str] = {}
+    dataschema: Optional[AnyUrl] = None
+    tracecontext: Dict[str, Any] = {}
 
     _raw: Optional[Any] = PrivateAttr()
 
     def __eq__(self, other):
         if not isinstance(other, CloudEvent):
             return False
         return self.id == other.id
 
     @validator("type", allow_reuse=True, always=True, pre=True)
-    def get_type_from_cls_name(cls, v) -> str:
+    def get_type_from_cls_name(cls, v):
         return v or cls.__name__
 
     @property
     def raw(self) -> Message:
         if self._raw is None:
             raise AttributeError("raw property accessible only for incoming messages")
         return self._raw
@@ -62,15 +64,21 @@
         return super().dict(**kwargs)
 
     @classmethod
     def new(cls, obj: D, **kwargs: Any):
         return cls(data=obj, **kwargs)
 
     def copy(self, **kwargs):
-        kwargs.setdefault("exclude", {"id", "trace_ctx"})
+        kwargs.setdefault(
+            "exclude",
+            {
+                "id",
+                "time",
+            },
+        )
         kwargs.setdefault("deep", True)
         return super().copy(**kwargs)
 
     @property
     def age(self) -> timedelta:
         return utc_now() - self.time
 
@@ -79,7 +87,10 @@
 
     class Config:
         use_enum_values = True
         allow_population_by_field_name = True
         extra = Extra.allow
         # events are immutable, however it's sometimes useful to set source or traceid for unpublished events
         allow_mutation = False
+
+
+TopicField = partial(Field, const=True, alias="subject")
```

### Comparing `eventiq-0.1.8/eventiq/plugins.py` & `eventiq-0.1.9/eventiq/plugins.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/runner.py` & `eventiq-0.1.9/eventiq/runner.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/service.py` & `eventiq-0.1.9/eventiq/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import asyncio
-from typing import Any, Callable
+from typing import Any, Callable, Sequence
 
+from .asyncapi.models import PublishInfo
+from .asyncapi.registry import PUBLISH_REGISTRY
 from .broker import Broker
 from .consumer import Consumer, ConsumerGroup, ForwardResponse
 from .logger import LoggerMixin
 from .models import CloudEvent
 from .settings import ServiceSettings
 from .types import TagMeta
 from .utils import generate_instance_id
@@ -21,28 +23,31 @@
         broker: Broker,
         title: str | None = None,
         version: str = "0.1.0",
         description: str = "",
         tags_metadata: list[TagMeta] | None = None,
         instance_id_generator: Callable[[], str] | None = None,
         base_event_class: type[CloudEvent] = CloudEvent,
+        publish_info: Sequence[PublishInfo] = (),
         **context: Any,
     ):
         self.broker = broker
         self.name = name
         self.title = title or name.title()
         self.version = version
         self.description = description
         self.tags_metadata = tags_metadata or []
         self.id = (instance_id_generator or generate_instance_id)()
         self.consumer_group = ConsumerGroup()
         self.context = context
         self.base_event_class = base_event_class
         # TODO: task gathering?
         self._tasks: list[asyncio.Task] = []
+        for p in publish_info:
+            PUBLISH_REGISTRY[p.event_type.__name__] = p
 
     def subscribe(
         self,
         topic: str,
         *,
         name: str | None = None,
         timeout: int = 120,
@@ -114,15 +119,12 @@
         from .runner import ServiceRunner
 
         runner = ServiceRunner([self])
         runner.run(*args, **kwargs)
 
     @classmethod
     def from_settings(cls, settings: ServiceSettings, **kwargs: Any) -> Service:
-        kw = settings.dict(exclude={"broker_settings"})
-        kw.update(**kwargs)
-        broker = Broker.from_settings(settings.broker_settings)
-        return cls(broker=broker, **kw)
+        return cls(**settings.dict(), **kwargs)
 
     @classmethod
     def from_env(cls, **kwargs: Any) -> Service:
         return cls.from_settings(ServiceSettings(), **kwargs)
```

### Comparing `eventiq-0.1.8/eventiq/types.py` & `eventiq-0.1.9/eventiq/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,18 +10,27 @@
     Type,
     TypedDict,
     TypeVar,
     Union,
 )
 from uuid import UUID
 
+from pydantic import ConstrainedStr
+
 if TYPE_CHECKING:
     from . import CloudEvent, GenericConsumer
 
-ID = Union[UUID, int, str]
+
+class StrId(ConstrainedStr):
+    strip_whitespace = True
+    min_length = 1
+    max_length = 64
+
+
+ID = Union[UUID, int, StrId]
 
 
 RawMessage = TypeVar("RawMessage")
 
 T = TypeVar("T", bound="CloudEvent")
 D = TypeVar("D")
```

### Comparing `eventiq-0.1.8/eventiq/utils/functools.py` & `eventiq-0.1.9/eventiq/utils/functools.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/eventiq/utils/imports.py` & `eventiq-0.1.9/eventiq/utils/imports.py`

 * *Files identical despite different names*

### Comparing `eventiq-0.1.8/pyproject.toml` & `eventiq-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventiq"
-version = "0.1.8"
+version = "0.1.9"
 description = "Cloud native framework for building event driven applications in Python."
 authors = ["Radzim Kowalow <radzim.kowalow@performance-media.pl>"]
 readme = "README.md"
 license = "Apache License 2.0"
 documentation = "https://performancemedia.github.io/eventiq/"
 repository = "https://github.com/performancemedia/eventiq"
 classifiers = [
```

### Comparing `eventiq-0.1.8/PKG-INFO` & `eventiq-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventiq
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cloud native framework for building event driven applications in Python.
 Home-page: https://github.com/performancemedia/eventiq
 License: Apache-2.0
 Keywords: framework,asyncio,microservice,event-driven
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
 Requires-Python: >=3.8.1,<4.0
@@ -71,15 +71,15 @@
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 *Note: This package is under active development and is not recommended for production use*
 
 ---
-Version: 0.1.8
+Version: 0.1.9
 
 Documentation: https://performancemedia.github.io/eventiq/
 
 Repository: https://github.com/performancemedia/eventiq
 
 ---
 ## About
```

