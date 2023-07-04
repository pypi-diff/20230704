# Comparing `tmp/flxtrd-0.2.1.tar.gz` & `tmp/flxtrd-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.2.1.tar", max compression
+gzip compressed data, was "flxtrd-0.2.2.tar", max compression
```

## Comparing `flxtrd-0.2.1.tar` & `flxtrd-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.1/LICENSE
--rw-r--r--   0        0        0     8795 2023-07-03 13:55:44.727340 flxtrd-0.2.1/README.md
--rw-r--r--   0        0        0     2255 2023-07-03 14:06:20.391319 flxtrd-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-03 13:51:39.979348 flxtrd-0.2.1/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0      580 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0     4911 2023-07-03 13:51:39.979348 flxtrd-0.2.1/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/devices.py
--rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0     5261 2023-07-03 13:51:39.979348 flxtrd-0.2.1/src/flxtrd/core/types.py
--rw-r--r--   0        0        0     1552 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0    10095 2023-07-03 14:05:46.907321 flxtrd-0.2.1/src/flxtrd/protocols/ampq.py
--rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.1/src/flxtrd/protocols/restapi.py
--rw-r--r--   0        0        0     9536 1970-01-01 00:00:00.000000 flxtrd-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8726 2023-07-04 06:14:54.741883 flxtrd-0.2.2/README.md
+-rw-r--r--   0        0        0     2211 2023-07-04 06:17:04.181879 flxtrd-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     7470 2023-07-04 06:14:54.745883 flxtrd-0.2.2/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      580 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4911 2023-07-03 13:51:39.979348 flxtrd-0.2.2/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     5261 2023-07-03 13:51:39.979348 flxtrd-0.2.2/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0     1552 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0    10763 2023-07-04 06:17:45.849878 flxtrd-0.2.2/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.2/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     9468 1970-01-01 00:00:00.000000 flxtrd-0.2.2/PKG-INFO
```

### Comparing `flxtrd-0.2.1/LICENSE` & `flxtrd-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/README.md` & `flxtrd-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -173,16 +173,15 @@
                     access_token="<your_device_access_token>"
                     )
 
 
     market = FlexMarket(market_url=GLOCALFLEX_MARKET_URL)
 
     # Create a AMPQ client that connects to the message broker
-    trading_client = FlexAPIClient(base_url=GLOCALFLEX_MARKET_URL,
-                                   user=user,
+    trading_client = FlexAPIClient(user=user,
                                    market=market
                                    )
 
     # Send a request to the GLocalFlex with REST API
     response, err = trading_client.make_request(method="POST",
                                                 endpoint="/users/login",
                                                 data={"email": user.name, "password": user.password},
@@ -197,17 +196,17 @@
 if __name__ == "__main__":
     main()
 
 ```
 
 
 ## Listen to market ticker messages
+Example usage of the trading client to just listen to market ticker messages
 
 ```py
-Example usage of the trading client to just listen to market ticker messages
 
 from logging import ERROR, INFO
 
 from flxtrd import (
     FlexAPIClient,
     FlexMarket,
     FlexUser,
@@ -255,10 +254,8 @@
 
 
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         log(INFO, "Keyboard interrupt received. Closing connection to the market broker")
-
-
 ```
```

### Comparing `flxtrd-0.2.1/pyproject.toml` & `flxtrd-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.2.1"
+version = "0.2.2"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
 #   {include = "examples"},
 # ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8,<3.12"
 pika = "^1.3.1"
 requests = ">=2.28.0"
 
+
+
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-mypy = "^0.981"
-pre-commit = "^2.20.0"
-tox = "^3.25.1"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+mypy = "^1.4.1"
+pre-commit = "^3.3.3"
+tox = "^4.6.3"
+
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.4.2"
-mkdocs-material = "^8.5.10"
-mkdocs-include-markdown-plugin = "^4.0.4"
 mike = "^1.1.2"
-mkdocs-glightbox = {version = ">=0.3.4"}
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.18"
+mkdocs-include-markdown-plugin = "^4.0.4"
+mkdocs-glightbox = "^0.3.4"
+mkdocstrings = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # [tool.poetry.scripts]
 # gflex-trading-bot = "gflex.client:main"
```

### Comparing `flxtrd-0.2.1/src/flxtrd/__init__.py` & `flxtrd-0.2.2/src/flxtrd/__init__.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/src/flxtrd/core/api_client.py` & `flxtrd-0.2.2/src/flxtrd/core/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from logging import DEBUG, INFO, WARNING
+import sys
 from typing import List, Optional, Tuple
 from warnings import warn
 
 from flxtrd.core.logger import log
 from flxtrd.core.plugins.auth import AuthPlugin
 from flxtrd.core.plugins.base import BasePlugin
 from flxtrd.core.types import (
@@ -42,14 +43,17 @@
         if base_url is not None:
             warn(
                 "Argument base_url is deprecated in favor of market.market_url v0.2.0",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
+        if user is None or market is None:
+            raise TypeError("User and market must be provided")
+        
         self.user = user
         self.market = market
         self.request_protocol = request_protocol(base_url=market.market_url)
 
         # By default the Auth Plugin is added
         self.plugins = plugins or [AuthPlugin(user=user, market=market)]
 
@@ -76,21 +80,21 @@
 
         for _plugin in self.plugins:
             log(INFO, f"Execute plugin {_plugin}")
             plugin_data[f"{_plugin}_before"] = _plugin.before_request(
                 endpoint, params=params, data=data
             )
 
-        # Check is connection is alive
+        # Check if connection exists
         if not self.trade_protocol.is_connected():
-            self.trade_protocol.connect(verify_ssl=verify_ssl)
-
-        if not self.trade_protocol.is_connected():
-            raise FlexError("Connection for context is not established")
+            err = self.trade_protocol.connect(verify_ssl=verify_ssl)
 
+            if err:
+                return (None, err)
+            
         response, err = self.trade_protocol.send_request(
             method=method,
             endpoint=endpoint,
             data=data,
             ssl=ssl,
             context=self.context,
             user=self.user,
@@ -166,26 +170,28 @@
 
         self.trade_protocol.checkreplies()
         if not self.trade_protocol.callback_responses:
             log(DEBUG, "No responses from the market")
             return None
         return self.trade_protocol.callback_responses
     
-    def connect(self):
+    def connect(self) -> None:
         """Connect to the market"""
         if self.user.app_key is None:
             # TODO just a temporary solution
             self.plugins[0].before_request()
-        self.trade_protocol.connect()
+        err = self.trade_protocol.connect()
+        if err:
+            raise err
     
-    def disconnect(self):
+    def disconnect(self) -> None:
         """Disconnect from the market"""
         self.trade_protocol.close_connection()
 
-    def sleep(self, seconds: int):
+    def sleep(self, seconds: int) -> None:
         """Sleep for a number of seconds"""
         self.trade_protocol.connection.sleep(seconds)
 
 
 class MarketMessages:
     """Market messages class to store the market messages, closed deals, ticks"""
```

### Comparing `flxtrd-0.2.1/src/flxtrd/core/logger.py` & `flxtrd-0.2.2/src/flxtrd/core/logger.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/src/flxtrd/core/plugins/auth.py` & `flxtrd-0.2.2/src/flxtrd/core/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/src/flxtrd/core/plugins/devices.py` & `flxtrd-0.2.2/src/flxtrd/core/plugins/devices.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/src/flxtrd/core/types.py` & `flxtrd-0.2.2/src/flxtrd/core/types.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/src/flxtrd/core/utils.py` & `flxtrd-0.2.2/src/flxtrd/core/utils.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/src/flxtrd/protocols/ampq.py` & `flxtrd-0.2.2/src/flxtrd/protocols/ampq.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,21 +135,22 @@
         # based on what the user provided different methods
         #  to connect to the server can be selected
         ssl_options = self._ssl_context(verify_ssl)
         err = self._connecttobrokerWithAppToken(
             user=self.user, broker=self.broker, ssl_options=ssl_options
         )
 
-        if not err:
-            self.set_consumer(
-                callback=self.callback_on_response,
-                callback_queue=self.callback_queue_id,
-                channel=self.channel,
-            )
-        return err
+        if err:
+            return err
+        
+        self.set_consumer(
+            callback=self.callback_on_response,
+            callback_queue=self.callback_queue_id,
+            channel=self.channel,
+        )
 
     def close_connection(self):
         """Close connection gracefully to message broker"""
         if self.connection is not None:
             self.connection.close()
             log(INFO, "Connection closed")
         else:
@@ -165,16 +166,18 @@
         try:
             self.channel.basic_publish(
                 exchange=exchangename,
                 routing_key=routingkey,
                 properties=props,
                 body=message,
             )
-        except Exception as error:
-            raise FlexError(str(error))
+        except pika.exceptions.ChannelWrongStateError as error:
+            if 'Channel is closed' in str(error):
+                raise FlexError('Channel is closed. Connection to broker is not possible.')
+
 
     def checkreplies(self):
         self.connection.process_data_events(time_limit=1)
 
     def is_connected(self):
         if self.connection is None:
             return False
@@ -200,27 +203,31 @@
             )
 
         credentials = pika.PlainCredentials(userid, accessToken)
         parameters = pika.ConnectionParameters(
             brokerip, brokerport, "/", credentials, ssl_options=ssl_options
         )
 
-        # Todo check which exceptions can occur
         try:
             self.connection = pika.BlockingConnection(parameters)
-            self.channel = self.connection.channel()
-            self.callback_queue_id = declareReplyToQueue(
-                self.channel, applicationKey, tickeroutexname
-            )
         except Exception as excep:
-            err = FlexError(str(excep))
-            raise excep
-        return err
+            # Todo check which exceptions can occur
+            raise FlexError(str(excep))
 
+        self.channel = self.connection.channel()
+        self.callback_queue_id = declare_reply_queue(
+            self.channel, applicationKey, tickeroutexname
+        )
+        if self.callback_queue_id is None:
+            return FlexError("No callback queue declared, That usually happens if more than one connection to the broker is opened", )
+        return None
+    
     def set_consumer(self, callback, callback_queue, channel):
+        if callback_queue is None:
+            raise FlexError("No callback queue declared, That usually happens if more than one connection to the broker is opened", )
         channel.basic_consume(queue=callback_queue, on_message_callback=callback, auto_ack=True)
 
     def checkreplies(self):
         if self.connection is None:
             raise FlexError("No connection to broker established")
         self.connection.process_data_events()
 
@@ -255,22 +262,30 @@
             log(ERROR, "RECEIVED A NON JSON MESSAGE:", body)
 
 
 def get_current_time_ms():
     return int(time.time() * 1000)
 
 
-def declareReplyToQueue(
+def declare_reply_queue(
     channel: pika.adapters.blocking_connection.BlockingChannel,
     applicationKey: str,
     tickeroutexname: str,
 ) -> str:
     """Create a queue for the reply to messages from the broker
     The provided applicationKey is used as the queue name"""
     try:
         dec_res = channel.queue_declare(applicationKey, exclusive=True)
-        callback_queue_id: str = dec_res.method.queue
-        channel.queue_bind(callback_queue_id, tickeroutexname)
-        log(INFO, f"Created queue with ID {callback_queue_id}")
-        return callback_queue_id
-    except pika.exceptions.ChannelClosedByBroker:
-        log(ERROR, "ReplyTo queue creation failed " + applicationKey)
+    except pika.exceptions.ChannelClosedByBroker as error:
+        if "RESOURCE_LOCKED" in str(error):
+            log(ERROR, "A connection from user with specific access token already exists")
+            return None
+        else:
+            log(ERROR, "ReplyTo queue creation failed " + applicationKey)
+            log(ERROR, error)
+            raise error
+
+    
+    callback_queue_id: str = dec_res.method.queue
+    channel.queue_bind(callback_queue_id, tickeroutexname)
+    log(INFO, f"Created queue with ID {callback_queue_id}")
+    return callback_queue_id
```

### Comparing `flxtrd-0.2.1/src/flxtrd/protocols/restapi.py` & `flxtrd-0.2.2/src/flxtrd/protocols/restapi.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.1/PKG-INFO` & `flxtrd-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.2.1
+Version: 0.2.2
 Summary: Public client API for the flexible energy trading market GLocalFlex.
 Home-page: https://github.com/glocalflex/GLocalFlexTrade
 Author: glocalflex
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: requests (>=2.28.0)
@@ -191,16 +191,15 @@
                     access_token="<your_device_access_token>"
                     )
 
 
     market = FlexMarket(market_url=GLOCALFLEX_MARKET_URL)
 
     # Create a AMPQ client that connects to the message broker
-    trading_client = FlexAPIClient(base_url=GLOCALFLEX_MARKET_URL,
-                                   user=user,
+    trading_client = FlexAPIClient(user=user,
                                    market=market
                                    )
 
     # Send a request to the GLocalFlex with REST API
     response, err = trading_client.make_request(method="POST",
                                                 endpoint="/users/login",
                                                 data={"email": user.name, "password": user.password},
@@ -215,17 +214,17 @@
 if __name__ == "__main__":
     main()
 
 ```
 
 
 ## Listen to market ticker messages
+Example usage of the trading client to just listen to market ticker messages
 
 ```py
-Example usage of the trading client to just listen to market ticker messages
 
 from logging import ERROR, INFO
 
 from flxtrd import (
     FlexAPIClient,
     FlexMarket,
     FlexUser,
@@ -273,10 +272,8 @@
 
 
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         log(INFO, "Keyboard interrupt received. Closing connection to the market broker")
-
-
 ```
```

