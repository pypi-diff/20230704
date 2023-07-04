# Comparing `tmp/whitson_tool_helper-0.2.0.tar.gz` & `tmp/whitson_tool_helper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitson_tool_helper-0.2.0.tar", last modified: Tue Jun 20 19:53:59 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.2.1.tar", last modified: Tue Jul  4 08:20:10 2023, max compression
```

## Comparing `whitson_tool_helper-0.2.0.tar` & `whitson_tool_helper-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      705 2023-06-20 19:53:53.000000 whitson_tool_helper-0.2.0/pyproject.toml
--rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/setup.cfg
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.635835 whitson_tool_helper-0.2.0/src/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.635835 whitson_tool_helper-0.2.0/src/whitson_tool_helper/
--rw-rw-r--   0 markus    (1000) markus    (1000)      107 2023-04-26 09:25:11.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)       66 2023-04-26 13:06:47.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/logger.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/
--rw-rw-r--   0 markus    (1000) markus    (1000)      370 2023-05-28 08:36:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/helper.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2737 2023-06-20 19:52:57.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/main.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3746 2023-06-12 08:05:49.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/pubsub.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4201 2023-06-20 19:48:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/timeout.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      704 2023-04-26 12:57:07.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/whitson_exceptions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.635835 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      575 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)      116 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-07-04 08:20:10.924577 whitson_tool_helper-0.2.1/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-07-04 08:20:10.924577 whitson_tool_helper-0.2.1/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      705 2023-07-04 08:20:03.000000 whitson_tool_helper-0.2.1/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-07-04 08:20:10.924577 whitson_tool_helper-0.2.1/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-07-04 08:20:10.920577 whitson_tool_helper-0.2.1/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-07-04 08:20:10.924577 whitson_tool_helper-0.2.1/src/whitson_tool_helper/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      107 2023-04-26 09:25:11.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)       66 2023-04-26 13:06:47.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/logger.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-07-04 08:20:10.924577 whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      370 2023-05-28 08:36:59.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/helper.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2737 2023-06-20 19:52:57.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/main.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3746 2023-06-12 08:05:49.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/pubsub.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4247 2023-07-04 08:17:06.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/timeout.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      704 2023-04-26 12:57:07.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper/whitson_exceptions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-07-04 08:20:10.924577 whitson_tool_helper-0.2.1/src/whitson_tool_helper.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-07-04 08:20:10.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      575 2023-07-04 08:20:10.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-07-04 08:20:10.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      116 2023-07-04 08:20:10.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-07-04 08:20:10.000000 whitson_tool_helper-0.2.1/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.2.0/pyproject.toml` & `whitson_tool_helper-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-version =  "0.2.0"
+version =  "0.2.1"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 dependencies = ["pika==1.3.1", "google-auth==2.16.0","google-cloud-pubsub==2.14.0", "google-cloud-storage==2.7.0","google-cloud-logging==3.5.0"]
```

### Comparing `whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/main.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.2.1/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     credentials = pika.PlainCredentials(
         os.environ["RABBITMQ_USER"], os.environ["RABBITMQ_PASSWORD"]
     )
     return pika.ConnectionParameters(
         host=os.environ["RABBITMQ_HOST"],
         port=os.environ["RABBITMQ_PORT"],
         credentials=credentials,
+        heartbeat=1200,
     )
 
 
 class RabbitMQConsumer:
     def __init__(self, process_function):
         self.process_function = process_function
         self.well_id = None
@@ -64,15 +65,17 @@
         if subscription.endswith("-calculated"):
             exchange = "clients"
 
         self.channel.queue_bind(
             queue=subscription, exchange=exchange, routing_key=subscription
         )
         self.channel.basic_qos(prefetch_count=1)
-        self.channel.basic_consume(queue=subscription, on_message_callback=self._callback)
+        self.channel.basic_consume(
+            queue=subscription, on_message_callback=self._callback
+        )
 
     def ack_and_close_connection(self):
         LOGGER.critical(f"Destroyed calc {self.model} for well {self.well_id}")
         self.channel.basic_ack(delivery_tag=self.delivery_tag)
         self.channel.stop_consuming()
 
     def work(self):
```

### Comparing `whitson_tool_helper-0.2.0/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.2.1/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.2.0/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.2.1/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.2.1/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

