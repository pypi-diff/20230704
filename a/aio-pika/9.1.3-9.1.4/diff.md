# Comparing `tmp/aio_pika-9.1.3.tar.gz` & `tmp/aio_pika-9.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_pika-9.1.3.tar", max compression
+gzip compressed data, was "aio_pika-9.1.4.tar", max compression
```

## Comparing `aio_pika-9.1.3.tar` & `aio_pika-9.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7585 2023-02-18 21:11:58.825819 aio_pika-9.1.3/README.rst
--rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.3/aio_pika/__init__.py
--rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.3/aio_pika/abc.py
--rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.3/aio_pika/channel.py
--rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.3/aio_pika/connection.py
--rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.3/aio_pika/exceptions.py
--rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.3/aio_pika/exchange.py
--rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.3/aio_pika/log.py
--rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.3/aio_pika/message.py
--rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.3/aio_pika/patterns/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.3/aio_pika/patterns/base.py
--rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.3/aio_pika/patterns/master.py
--rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.1.3/aio_pika/patterns/rpc.py
--rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.3/aio_pika/pool.py
--rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.3/aio_pika/py.typed
--rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.3/aio_pika/queue.py
--rw-r--r--   0        0        0     8219 2023-06-01 15:55:44.133275 aio_pika-9.1.3/aio_pika/robust_channel.py
--rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.3/aio_pika/robust_connection.py
--rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.3/aio_pika/robust_exchange.py
--rw-r--r--   0        0        0     4883 2023-06-01 15:55:44.136895 aio_pika-9.1.3/aio_pika/robust_queue.py
--rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.3/aio_pika/tools.py
--rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.3/aio_pika/transaction.py
--rw-r--r--   0        0        0     3269 2023-06-21 09:55:41.970816 aio_pika-9.1.3/pyproject.toml
--rw-r--r--   0        0        0     9488 1970-01-01 00:00:00.000000 aio_pika-9.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7568 2023-07-04 13:02:10.950030 aio_pika-9.1.4/README.rst
+-rw-r--r--   0        0        0     1153 2023-03-09 17:26:20.374813 aio_pika-9.1.4/aio_pika/__init__.py
+-rw-r--r--   0        0        0    24756 2023-06-01 15:55:44.119921 aio_pika-9.1.4/aio_pika/abc.py
+-rw-r--r--   0        0        0    14701 2023-06-01 15:55:44.121581 aio_pika-9.1.4/aio_pika/channel.py
+-rw-r--r--   0        0        0    10892 2023-06-01 15:55:44.123355 aio_pika-9.1.4/aio_pika/connection.py
+-rw-r--r--   0        0        0     1304 2022-05-25 16:48:09.069546 aio_pika-9.1.4/aio_pika/exceptions.py
+-rw-r--r--   0        0        0     6730 2023-06-01 15:55:44.124351 aio_pika-9.1.4/aio_pika/exchange.py
+-rw-r--r--   0        0        0      246 2022-07-06 12:21:30.146673 aio_pika-9.1.4/aio_pika/log.py
+-rw-r--r--   0        0        0    19763 2023-06-01 15:55:44.125260 aio_pika-9.1.4/aio_pika/message.py
+-rw-r--r--   0        0        0      233 2020-05-21 16:45:24.000000 aio_pika-9.1.4/aio_pika/patterns/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-01 15:55:44.126438 aio_pika-9.1.4/aio_pika/patterns/base.py
+-rw-r--r--   0        0        0     6208 2023-06-01 15:55:44.128054 aio_pika-9.1.4/aio_pika/patterns/master.py
+-rw-r--r--   0        0        0    14727 2023-06-07 14:58:48.045474 aio_pika-9.1.4/aio_pika/patterns/rpc.py
+-rw-r--r--   0        0        0     4177 2023-06-01 15:55:44.130894 aio_pika-9.1.4/aio_pika/pool.py
+-rw-r--r--   0        0        0        1 2019-02-24 19:52:26.000000 aio_pika-9.1.4/aio_pika/py.typed
+-rw-r--r--   0        0        0    16598 2023-06-01 15:55:44.131780 aio_pika-9.1.4/aio_pika/queue.py
+-rw-r--r--   0        0        0     8219 2023-06-01 15:55:44.133275 aio_pika-9.1.4/aio_pika/robust_channel.py
+-rw-r--r--   0        0        0    10445 2023-06-01 15:55:44.135097 aio_pika-9.1.4/aio_pika/robust_connection.py
+-rw-r--r--   0        0        0     2889 2023-06-01 15:55:44.136022 aio_pika-9.1.4/aio_pika/robust_exchange.py
+-rw-r--r--   0        0        0     4683 2023-07-04 14:24:49.233661 aio_pika-9.1.4/aio_pika/robust_queue.py
+-rw-r--r--   0        0        0     8639 2023-06-01 15:55:44.138218 aio_pika-9.1.4/aio_pika/tools.py
+-rw-r--r--   0        0        0     2065 2023-06-01 15:55:44.139689 aio_pika-9.1.4/aio_pika/transaction.py
+-rw-r--r--   0        0        0     3269 2023-07-04 14:25:10.969778 aio_pika-9.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9471 1970-01-01 00:00:00.000000 aio_pika-9.1.4/PKG-INFO
```

### Comparing `aio_pika-9.1.3/README.rst` & `aio_pika-9.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 --------
 
 * Completely asynchronous API.
 * Object oriented API.
 * Transparent auto-reconnects with complete state recovery with `connect_robust`
   (e.g. declared queues or exchanges, consuming state and bindings).
 * Python 3.7+ compatible.
-* For python 3.5 users available `aio-pika<7`
-* Transparent `publisher confirms`_ support
-* `Transactions`_ support
-* Completely type-hints coverage.
+* For python 3.5 users, aio-pika is available via `aio-pika<7`.
+* Transparent `publisher confirms`_ support.
+* `Transactions`_ support.
+* Complete type-hints coverage.
 
 
 .. _Transactions: https://www.rabbitmq.com/semantics.html
 .. _publisher confirms: https://www.rabbitmq.com/confirms.html
 
 
 Installation
@@ -246,19 +246,19 @@
 
 
 Running Tests
 _____________
 
 **NOTE: In order to run the tests locally you need to run a RabbitMQ instance with default user/password (guest/guest) and port (5672).**
 
-* ProTip: Use Docker for this:
+The Makefile provides a command to run an appropriate RabbitMQ Docker image:
 
 .. code-block:: bash
 
-    docker run -d -p 5671:5671 -p 5672:5672 -p 15671:15671 -p 15672:15672 mosquito/aiormq-rabbitmq
+    make rabbitmq
 
 To test just run:
 
 .. code-block:: bash
 
     make test
```

### Comparing `aio_pika-9.1.3/aio_pika/__init__.py` & `aio_pika-9.1.4/aio_pika/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/abc.py` & `aio_pika-9.1.4/aio_pika/abc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/channel.py` & `aio_pika-9.1.4/aio_pika/channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/connection.py` & `aio_pika-9.1.4/aio_pika/connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/exceptions.py` & `aio_pika-9.1.4/aio_pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/exchange.py` & `aio_pika-9.1.4/aio_pika/exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/message.py` & `aio_pika-9.1.4/aio_pika/message.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/patterns/base.py` & `aio_pika-9.1.4/aio_pika/patterns/base.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/patterns/master.py` & `aio_pika-9.1.4/aio_pika/patterns/master.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/patterns/rpc.py` & `aio_pika-9.1.4/aio_pika/patterns/rpc.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/pool.py` & `aio_pika-9.1.4/aio_pika/pool.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/queue.py` & `aio_pika-9.1.4/aio_pika/queue.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/robust_channel.py` & `aio_pika-9.1.4/aio_pika/robust_channel.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/robust_connection.py` & `aio_pika-9.1.4/aio_pika/robust_connection.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/robust_exchange.py` & `aio_pika-9.1.4/aio_pika/robust_exchange.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/robust_queue.py` & `aio_pika-9.1.4/aio_pika/robust_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import uuid
 import warnings
-from random import Random
 from typing import Any, Awaitable, Callable, Dict, Optional, Tuple, Union
 
 import aiormq
 from aiormq import ChannelInvalidStateError
 from pamqp.common import Arguments
 
 from .abc import (
@@ -20,35 +20,28 @@
 
 class RobustQueue(Queue, AbstractRobustQueue):
     __slots__ = ("_consumers", "_bindings")
 
     _consumers: Dict[ConsumerTag, Dict[str, Any]]
     _bindings: Dict[Tuple[Union[AbstractExchange, str], str], Dict[str, Any]]
 
-    _rnd_gen: Random = Random()
-
-    @classmethod
-    def _get_random_queue_name(cls) -> str:
-        rnd = cls._rnd_gen.getrandbits(128)
-        return "amq_%s" % hex(rnd).lower()
-
     def __init__(
         self,
         channel: AbstractChannel,
         name: Optional[str],
         durable: bool = False,
         exclusive: bool = False,
         auto_delete: bool = False,
         arguments: Arguments = None,
         passive: bool = False,
     ):
 
         super().__init__(
             channel=channel,
-            name=name or self._get_random_queue_name(),
+            name=name or f"amq_{uuid.uuid4().hex}",
             durable=durable,
             exclusive=exclusive,
             auto_delete=auto_delete,
             arguments=arguments,
             passive=passive,
         )
```

### Comparing `aio_pika-9.1.3/aio_pika/tools.py` & `aio_pika-9.1.4/aio_pika/tools.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/aio_pika/transaction.py` & `aio_pika-9.1.4/aio_pika/transaction.py`

 * *Files identical despite different names*

### Comparing `aio_pika-9.1.3/pyproject.toml` & `aio_pika-9.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-pika"
-version = "9.1.3"
+version = "9.1.4"
 description = "Wrapper around the aiormq for asyncio and humans"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "aiormq"]
 homepage = "https://github.com/mosquito/aio-pika"
 classifiers = [
```

### Comparing `aio_pika-9.1.3/PKG-INFO` & `aio_pika-9.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pika
-Version: 9.1.3
+Version: 9.1.4
 Summary: Wrapper around the aiormq for asyncio and humans
 Home-page: https://github.com/mosquito/aio-pika
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,aiormq
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
@@ -95,18 +95,18 @@
 --------
 
 * Completely asynchronous API.
 * Object oriented API.
 * Transparent auto-reconnects with complete state recovery with `connect_robust`
   (e.g. declared queues or exchanges, consuming state and bindings).
 * Python 3.7+ compatible.
-* For python 3.5 users available `aio-pika<7`
-* Transparent `publisher confirms`_ support
-* `Transactions`_ support
-* Completely type-hints coverage.
+* For python 3.5 users, aio-pika is available via `aio-pika<7`.
+* Transparent `publisher confirms`_ support.
+* `Transactions`_ support.
+* Complete type-hints coverage.
 
 
 .. _Transactions: https://www.rabbitmq.com/semantics.html
 .. _publisher confirms: https://www.rabbitmq.com/confirms.html
 
 
 Installation
@@ -290,19 +290,19 @@
 
 
 Running Tests
 _____________
 
 **NOTE: In order to run the tests locally you need to run a RabbitMQ instance with default user/password (guest/guest) and port (5672).**
 
-* ProTip: Use Docker for this:
+The Makefile provides a command to run an appropriate RabbitMQ Docker image:
 
 .. code-block:: bash
 
-    docker run -d -p 5671:5671 -p 5672:5672 -p 15671:15671 -p 15672:15672 mosquito/aiormq-rabbitmq
+    make rabbitmq
 
 To test just run:
 
 .. code-block:: bash
 
     make test
```

