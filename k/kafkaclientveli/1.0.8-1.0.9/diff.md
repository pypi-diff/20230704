# Comparing `tmp/kafkaclientveli-1.0.8.tar.gz` & `tmp/kafkaclientveli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaclientveli-1.0.8.tar", last modified: Tue Jul  4 09:35:16 2023, max compression
+gzip compressed data, was "kafkaclientveli-1.0.9.tar", last modified: Tue Jul  4 09:36:33 2023, max compression
```

## Comparing `kafkaclientveli-1.0.8.tar` & `kafkaclientveli-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:35:16.539525 kafkaclientveli-1.0.8/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 kafkaclientveli-1.0.8/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:35:16.539401 kafkaclientveli-1.0.8/PKG-INFO
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:35:16.536733 kafkaclientveli-1.0.8/kafkaclientveli.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:35:16.000000 kafkaclientveli-1.0.8/kafkaclientveli.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-04 09:35:16.000000 kafkaclientveli-1.0.8/kafkaclientveli.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-04 09:35:16.000000 kafkaclientveli-1.0.8/kafkaclientveli.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-04 09:35:16.000000 kafkaclientveli-1.0.8/kafkaclientveli.egg-info/top_level.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.8/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-04 09:35:16.539564 kafkaclientveli-1.0.8/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-04 09:35:10.000000 kafkaclientveli-1.0.8/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:35:16.537944 kafkaclientveli-1.0.8/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-04 09:18:27.000000 kafkaclientveli-1.0.8/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2044 2023-07-04 08:42:05.000000 kafkaclientveli-1.0.8/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3485 2023-07-04 08:59:05.000000 kafkaclientveli-1.0.8/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:35:16.538487 kafkaclientveli-1.0.8/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.8/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.8/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1940 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.8/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.8/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1299 2023-07-04 09:34:58.000000 kafkaclientveli-1.0.8/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:35:16.539206 kafkaclientveli-1.0.8/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.8/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.8/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1145 2023-07-04 08:42:00.000000 kafkaclientveli-1.0.8/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:36:33.629212 kafkaclientveli-1.0.9/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 kafkaclientveli-1.0.9/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:36:33.629097 kafkaclientveli-1.0.9/PKG-INFO
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:36:33.626528 kafkaclientveli-1.0.9/kafkaclientveli.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:36:33.000000 kafkaclientveli-1.0.9/kafkaclientveli.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-04 09:36:33.000000 kafkaclientveli-1.0.9/kafkaclientveli.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-04 09:36:33.000000 kafkaclientveli-1.0.9/kafkaclientveli.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-04 09:36:33.000000 kafkaclientveli-1.0.9/kafkaclientveli.egg-info/top_level.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.9/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-04 09:36:33.629242 kafkaclientveli-1.0.9/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-04 09:36:25.000000 kafkaclientveli-1.0.9/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:36:33.627739 kafkaclientveli-1.0.9/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-04 09:18:27.000000 kafkaclientveli-1.0.9/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2044 2023-07-04 08:42:05.000000 kafkaclientveli-1.0.9/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3485 2023-07-04 08:59:05.000000 kafkaclientveli-1.0.9/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:36:33.628296 kafkaclientveli-1.0.9/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.9/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.9/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1940 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.9/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.9/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1123 2023-07-04 09:36:19.000000 kafkaclientveli-1.0.9/velikafkaclient/producer.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:36:33.628936 kafkaclientveli-1.0.9/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.9/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.9/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1145 2023-07-04 08:42:00.000000 kafkaclientveli-1.0.9/velikafkaclient/topics/triptracker.py
```

### Comparing `kafkaclientveli-1.0.8/PKG-INFO` & `kafkaclientveli-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaclientveli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `kafkaclientveli-1.0.8/kafkaclientveli.egg-info/PKG-INFO` & `kafkaclientveli-1.0.9/kafkaclientveli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaclientveli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `kafkaclientveli-1.0.8/kafkaclientveli.egg-info/SOURCES.txt` & `kafkaclientveli-1.0.9/kafkaclientveli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.8/readme.md` & `kafkaclientveli-1.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.8/velikafkaclient/consumer.py` & `kafkaclientveli-1.0.9/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.8/velikafkaclient/eventregistration.py` & `kafkaclientveli-1.0.9/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.8/velikafkaclient/events/triptracker.py` & `kafkaclientveli-1.0.9/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.8/velikafkaclient/producer.py` & `kafkaclientveli-1.0.9/velikafkaclient/producer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 import json
 
 from aiokafka import AIOKafkaProducer
 
-from .exceptions import InvalidEventTopicException
-# from exceptions import InvalidEventTopicException, InvalidEventModelForTopic
-# from topics.topics import KafkaTopic
-# from events.base import KafkaEvent
-#
-#
-# class AsyncKafkaEventProducer:
-#
-#     def __init__(self, bootstrap_servers):
-#         self.kafka_topic_events = kafka_topic_events
-#         self.producer = AIOKafkaProducer(
-#             bootstrap_servers=bootstrap_servers
-#         )
-#
-#     async def start(self):
-#         await self.producer.start()
-#
-#     async def stop(self):
-#         await self.producer.flush()
-#         await self.producer.stop()
-#
-#     async def produce_event(self, topic: KafkaTopic, event: KafkaEvent):
-#         if topic not in self.kafka_topic_events.topic_event_models:
-#             raise InvalidEventTopicException(f"Topic {topic} not found")
-#         topic_event_model = self.kafka_topic_events.topic_event_models[topic]
-#         if not isinstance(event, topic_event_model):
-#             raise InvalidEventModelForTopic(f"event: {str(event)} topic model: {str(topic_event_model)}")
-#         await self.producer.send(topic, json.dumps(event.dict()).encode())
-class Test:
+from .exceptions import InvalidEventTopicException, InvalidEventModelForTopic
+from .topics.topics import KafkaTopic
+from .events.base import KafkaEvent
 
-    def print(self, x):
-        raise InvalidEventTopicException()
+
+class AsyncKafkaEventProducer:
+
+    def __init__(self, bootstrap_servers):
+        self.kafka_topic_events = kafka_topic_events
+        self.producer = AIOKafkaProducer(
+            bootstrap_servers=bootstrap_servers
+        )
+
+    async def start(self):
+        await self.producer.start()
+
+    async def stop(self):
+        await self.producer.flush()
+        await self.producer.stop()
+
+    async def produce_event(self, topic: KafkaTopic, event: KafkaEvent):
+        if topic not in self.kafka_topic_events.topic_event_models:
+            raise InvalidEventTopicException(f"Topic {topic} not found")
+        topic_event_model = self.kafka_topic_events.topic_event_models[topic]
+        if not isinstance(event, topic_event_model):
+            raise InvalidEventModelForTopic(f"event: {str(event)} topic model: {str(topic_event_model)}")
+        await self.producer.send(topic, json.dumps(event.dict()).encode())
```

### Comparing `kafkaclientveli-1.0.8/velikafkaclient/topics/triptracker.py` & `kafkaclientveli-1.0.9/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

