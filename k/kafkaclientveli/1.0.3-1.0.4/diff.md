# Comparing `tmp/kafkaclientveli-1.0.3.tar.gz` & `tmp/kafkaclientveli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafkaclientveli-1.0.3.tar", last modified: Tue Jul  4 09:22:18 2023, max compression
+gzip compressed data, was "kafkaclientveli-1.0.4.tar", last modified: Tue Jul  4 09:23:56 2023, max compression
```

## Comparing `kafkaclientveli-1.0.3.tar` & `kafkaclientveli-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:22:18.693076 kafkaclientveli-1.0.3/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 kafkaclientveli-1.0.3/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:22:18.692973 kafkaclientveli-1.0.3/PKG-INFO
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:22:18.690475 kafkaclientveli-1.0.3/kafkaclientveli.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:22:18.000000 kafkaclientveli-1.0.3/kafkaclientveli.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-04 09:22:18.000000 kafkaclientveli-1.0.3/kafkaclientveli.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-04 09:22:18.000000 kafkaclientveli-1.0.3/kafkaclientveli.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-04 09:22:18.000000 kafkaclientveli-1.0.3/kafkaclientveli.egg-info/top_level.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.3/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-04 09:22:18.693104 kafkaclientveli-1.0.3/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-04 09:22:09.000000 kafkaclientveli-1.0.3/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:22:18.691584 kafkaclientveli-1.0.3/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-04 09:18:27.000000 kafkaclientveli-1.0.3/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2044 2023-07-04 08:42:05.000000 kafkaclientveli-1.0.3/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3485 2023-07-04 08:59:05.000000 kafkaclientveli-1.0.3/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:22:18.692109 kafkaclientveli-1.0.3/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.3/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.3/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1940 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.3/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.3/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1279 2023-07-04 09:22:09.000000 kafkaclientveli-1.0.3/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:22:18.692808 kafkaclientveli-1.0.3/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.3/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.3/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1145 2023-07-04 08:42:00.000000 kafkaclientveli-1.0.3/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:23:56.977974 kafkaclientveli-1.0.4/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 kafkaclientveli-1.0.4/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:23:56.977847 kafkaclientveli-1.0.4/PKG-INFO
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:23:56.976116 kafkaclientveli-1.0.4/kafkaclientveli.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-04 09:23:56.000000 kafkaclientveli-1.0.4/kafkaclientveli.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-04 09:23:56.000000 kafkaclientveli-1.0.4/kafkaclientveli.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-04 09:23:56.000000 kafkaclientveli-1.0.4/kafkaclientveli.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-04 09:23:56.000000 kafkaclientveli-1.0.4/kafkaclientveli.egg-info/top_level.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.4/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-04 09:23:56.978007 kafkaclientveli-1.0.4/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-04 09:23:51.000000 kafkaclientveli-1.0.4/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:23:56.976841 kafkaclientveli-1.0.4/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-04 09:18:27.000000 kafkaclientveli-1.0.4/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2044 2023-07-04 08:42:05.000000 kafkaclientveli-1.0.4/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3485 2023-07-04 08:59:05.000000 kafkaclientveli-1.0.4/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:23:56.977281 kafkaclientveli-1.0.4/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.4/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.4/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1940 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.4/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.4/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1301 2023-07-04 09:23:36.000000 kafkaclientveli-1.0.4/velikafkaclient/producer.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-04 09:23:56.977665 kafkaclientveli-1.0.4/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-19 11:33:35.000000 kafkaclientveli-1.0.4/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-06-23 12:26:50.000000 kafkaclientveli-1.0.4/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1145 2023-07-04 08:42:00.000000 kafkaclientveli-1.0.4/velikafkaclient/topics/triptracker.py
```

### Comparing `kafkaclientveli-1.0.3/PKG-INFO` & `kafkaclientveli-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaclientveli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `kafkaclientveli-1.0.3/kafkaclientveli.egg-info/PKG-INFO` & `kafkaclientveli-1.0.4/kafkaclientveli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafkaclientveli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `kafkaclientveli-1.0.3/kafkaclientveli.egg-info/SOURCES.txt` & `kafkaclientveli-1.0.4/kafkaclientveli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.3/readme.md` & `kafkaclientveli-1.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.3/velikafkaclient/consumer.py` & `kafkaclientveli-1.0.4/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.3/velikafkaclient/eventregistration.py` & `kafkaclientveli-1.0.4/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.3/velikafkaclient/events/triptracker.py` & `kafkaclientveli-1.0.4/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `kafkaclientveli-1.0.3/velikafkaclient/producer.py` & `kafkaclientveli-1.0.4/velikafkaclient/producer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# import json
-#
-# from aiokafka import AIOKafkaProducer
+import json
+
+from aiokafka import AIOKafkaProducer
 #
 # from eventregistration import kafka_topic_events
 # from exceptions import InvalidEventTopicException, InvalidEventModelForTopic
 # from topics.topics import KafkaTopic
 # from events.base import KafkaEvent
 #
 #
@@ -29,8 +29,9 @@
 #         topic_event_model = self.kafka_topic_events.topic_event_models[topic]
 #         if not isinstance(event, topic_event_model):
 #             raise InvalidEventModelForTopic(f"event: {str(event)} topic model: {str(topic_event_model)}")
 #         await self.producer.send(topic, json.dumps(event.dict()).encode())
 class Test:
 
     def print(self, x):
+        AIOKafkaProducer()
         print(x)
```

### Comparing `kafkaclientveli-1.0.3/velikafkaclient/topics/triptracker.py` & `kafkaclientveli-1.0.4/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

