# Comparing `tmp/velikafkaclient-1.0.1.tar.gz` & `tmp/velikafkaclient-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.1.tar", last modified: Wed Jul  5 13:40:40 2023, max compression
+gzip compressed data, was "velikafkaclient-1.0.2.tar", last modified: Mon Jul 10 13:03:20 2023, max compression
```

## Comparing `velikafkaclient-1.0.1.tar` & `velikafkaclient-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.651752 velikafkaclient-1.0.1/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-05 13:40:40.651605 velikafkaclient-1.0.1/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-05 13:40:40.651793 velikafkaclient-1.0.1/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-05 13:40:31.000000 velikafkaclient-1.0.1/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.649869 velikafkaclient-1.0.1/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2046 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.650937 velikafkaclient-1.0.1/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      105 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1179 2023-07-05 13:39:50.000000 velikafkaclient-1.0.1/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.651375 velikafkaclient-1.0.1/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.1/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 13:40:40.650421 velikafkaclient-1.0.1/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      547 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-05 13:40:40.000000 velikafkaclient-1.0.1/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.310267 velikafkaclient-1.0.2/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-10 13:03:20.310158 velikafkaclient-1.0.2/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-10 13:03:20.310296 velikafkaclient-1.0.2/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-10 13:03:03.000000 velikafkaclient-1.0.2/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.308621 velikafkaclient-1.0.2/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2046 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      374 2023-07-10 13:02:55.000000 velikafkaclient-1.0.2/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.309446 velikafkaclient-1.0.2/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      126 2023-07-10 12:56:14.000000 velikafkaclient-1.0.2/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-10 12:56:14.000000 velikafkaclient-1.0.2/velikafkaclient/producer.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.309980 velikafkaclient-1.0.2/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.2/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-10 13:03:20.309084 velikafkaclient-1.0.2/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1663 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      577 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-10 13:03:20.000000 velikafkaclient-1.0.2/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.1/PKG-INFO` & `velikafkaclient-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.1/readme.md` & `velikafkaclient-1.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.1/velikafkaclient/consumer.py` & `velikafkaclient-1.0.2/velikafkaclient/consumer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.1/velikafkaclient/eventregistration.py` & `velikafkaclient-1.0.2/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.1/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.0.2/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.1/velikafkaclient/producer.py` & `velikafkaclient-1.0.2/velikafkaclient/producer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from aiokafka import AIOKafkaProducer
 
 from .eventregistration import kafka_topic_events
 from .exceptions import InvalidEventTopicException, InvalidEventModelForTopic
 from .topics.topics import KafkaTopic
 from .events.base import KafkaEvent
-
+from velilogger import get_tracing_id
 
 class AsyncKafkaEventProducer:
 
     def __init__(self, bootstrap_servers):
         self.kafka_topic_events = kafka_topic_events
         self.producer = AIOKafkaProducer(
             bootstrap_servers=bootstrap_servers
@@ -25,8 +25,9 @@
 
     async def produce_event(self, topic: KafkaTopic, event: KafkaEvent):
         if topic not in self.kafka_topic_events.topic_event_models:
             raise InvalidEventTopicException(f"Topic {topic} not found")
         topic_event_model = self.kafka_topic_events.topic_event_models[topic]
         if not isinstance(event, topic_event_model):
             raise InvalidEventModelForTopic(f"event: {str(event)} topic model: {str(topic_event_model)}")
+        event.tracing_id = get_tracing_id()
         await self.producer.send(topic.value, json.dumps(event.dict()).encode())
```

### Comparing `velikafkaclient-1.0.1/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.0.2/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.1/velikafkaclient.egg-info/PKG-INFO` & `velikafkaclient-1.0.2/velikafkaclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velikafkaclient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Veli Kafka Client
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `velikafkaclient-1.0.1/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.0.2/velikafkaclient.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 readme.md
 setup.py
 velikafkaclient/__init__.py
 velikafkaclient/consumer.py
+velikafkaclient/decorators.py
 velikafkaclient/eventregistration.py
 velikafkaclient/exceptions.py
 velikafkaclient/producer.py
 velikafkaclient.egg-info/PKG-INFO
 velikafkaclient.egg-info/SOURCES.txt
 velikafkaclient.egg-info/dependency_links.txt
 velikafkaclient.egg-info/top_level.txt
```

