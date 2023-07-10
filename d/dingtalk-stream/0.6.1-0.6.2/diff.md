# Comparing `tmp/dingtalk-stream-0.6.1.tar.gz` & `tmp/dingtalk-stream-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.6.1.tar", last modified: Wed Jul  5 07:37:45 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.6.2.tar", last modified: Mon Jul 10 08:12:20 2023, max compression
```

## Comparing `dingtalk-stream-0.6.1.tar` & `dingtalk-stream-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:37:45.344431 dingtalk-stream-0.6.1/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 07:37:45.000000 dingtalk-stream-0.6.1/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:37:45.348431 dingtalk-stream-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-05 07:37:43.000000 dingtalk-stream-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:12:20.875393 dingtalk-stream-0.6.2/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/setup.py
```

### Comparing `dingtalk-stream-0.6.1/LICENSE` & `dingtalk-stream-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/PKG-INFO` & `dingtalk-stream-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.6.1/README.md` & `dingtalk-stream-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/__init__.py` & `dingtalk-stream-0.6.2/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.6.2/dingtalk_stream/card_instance.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.6.2/dingtalk_stream/card_replier.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.6.2/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/frames.py` & `dingtalk-stream-0.6.2/dingtalk_stream/frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 msg.extensions[name] = value
         if data:
             msg.data = json.loads(data)
         return msg
 
 class SystemMessage(object):
     TYPE = 'SYSTEM'
-    TOPIC_DISCONNECT = 'TAG_DISCONNECT'
+    TOPIC_DISCONNECT = 'disconnect'
 
     def __init__(self):
         self.spec_version = ''
         self.type = SystemMessage.TYPE
         self.headers = Headers()
         self.data = {}
         self.extensions = {}
```

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/handlers.py` & `dingtalk-stream-0.6.2/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.6.2/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream/stream.py` & `dingtalk-stream-0.6.2/dingtalk_stream/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,28 +73,29 @@
             async with websockets.connect(uri) as websocket:
                 self.websocket = websocket
                 async for raw_message in websocket:
                     json_message = json.loads(raw_message)
                     route_result = await self.route_message(json_message)
                     if route_result == DingTalkStreamClient.TAG_DISCONNECT:
                         break
-                self.websocket.close()
+                # self.websocket.close()
         return
 
     async def route_message(self, json_message):
         result = ''
         msg_type = json_message.get('type', '')
         headers = json_message.get('headers', {})
         topic = headers.get('topic', '')
         ack = None
         if msg_type == SystemMessage.TYPE:
             msg = SystemMessage.from_dict(json_message)
             ack = await self.system_handler.raw_process(msg)
             if msg.headers.topic == SystemMessage.TOPIC_DISCONNECT:
                 result = DingTalkStreamClient.TAG_DISCONNECT
+                self.logger.info("received disconnect topic=%s, message=%s", msg.headers.topic, json_message)
             else:
                 self.logger.warning("unknown message topic, topic=%s, message=%s", msg.headers.topic, json_message)
         elif msg_type == EventMessage.TYPE:
             msg = EventMessage.from_dict(json_message)
             ack = await self.event_handler.raw_process(msg)
         elif msg_type == CallbackMessage.TYPE:
             msg = CallbackMessage.from_dict(json_message)
```

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.6.2/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.6.1/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.6.2/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.1/setup.py` & `dingtalk-stream-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.6.1',
+    version='0.6.2',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

