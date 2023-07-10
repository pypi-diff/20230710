# Comparing `tmp/bondzai.gateway-sdk-0.0.6.tar.gz` & `tmp/bondzai.gateway-sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-sdk-0.0.6.tar", last modified: Tue Jul  4 14:21:00 2023, max compression
+gzip compressed data, was "bondzai.gateway-sdk-0.0.7.tar", last modified: Mon Jul 10 18:00:20 2023, max compression
```

## Comparing `bondzai.gateway-sdk-0.0.6.tar` & `bondzai.gateway-sdk-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:21:00.536608 bondzai.gateway-sdk-0.0.6/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-04 14:21:00.536795 bondzai.gateway-sdk-0.0.6/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      155 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:21:00.526466 bondzai.gateway-sdk-0.0.6/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:21:00.533508 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/
--rw-r--r--   0 theo       (501) staff       (20)      139 2023-07-04 14:20:47.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)    10180 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/agent.py
--rw-r--r--   0 theo       (501) staff       (20)     2497 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/commands.py
--rw-r--r--   0 theo       (501) staff       (20)      255 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/config.py
--rw-r--r--   0 theo       (501) staff       (20)     6661 2023-07-04 14:20:27.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     6937 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/events.py
--rw-r--r--   0 theo       (501) staff       (20)     4429 2023-07-04 14:20:47.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/gateway.py
--rw-r--r--   0 theo       (501) staff       (20)     3288 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/message.py
--rw-r--r--   0 theo       (501) staff       (20)      810 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/request.py
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/responses.py
--rw-r--r--   0 theo       (501) staff       (20)      771 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/timer.py
--rw-r--r--   0 theo       (501) staff       (20)     1396 2023-07-04 14:20:47.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/transcode.py
--rw-r--r--   0 theo       (501) staff       (20)      738 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 14:21:00.536247 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-04 14:21:00.000000 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      770 2023-07-04 14:21:00.000000 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 14:21:00.000000 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 14:21:00.000000 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       61 2023-07-04 14:21:00.000000 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 14:21:00.000000 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 14:21:00.000000 bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)    21241 2023-07-04 14:20:09.000000 bondzai.gateway-sdk-0.0.6/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-04 14:21:00.537798 bondzai.gateway-sdk-0.0.6/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:20.200379 bondzai.gateway-sdk-0.0.7/
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/NOTICE
+-rwxrwxrwx   0 root         (0) root         (0)      604 2023-07-10 18:00:20.201395 bondzai.gateway-sdk-0.0.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      155 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:19.504550 bondzai.gateway-sdk-0.0.7/bondzai/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:19.992056 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/
+-rwxrwxrwx   0 root         (0) root         (0)      139 2023-07-10 18:00:09.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10202 2023-07-10 18:00:09.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/agent.py
+-rwxrwxrwx   0 root         (0) root         (0)     2497 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/commands.py
+-rwxrwxrwx   0 root         (0) root         (0)      255 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     6693 2023-07-10 18:00:09.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)     6937 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     4429 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/gateway.py
+-rwxrwxrwx   0 root         (0) root         (0)     3288 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/message.py
+-rwxrwxrwx   0 root         (0) root         (0)      810 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/request.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/responses.py
+-rwxrwxrwx   0 root         (0) root         (0)      771 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/timer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1396 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/transcode.py
+-rwxrwxrwx   0 root         (0) root         (0)      738 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 18:00:20.173659 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      604 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)       61 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 18:00:19.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 18:00:18.000000 bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)    21241 2023-07-10 17:57:02.000000 bondzai.gateway-sdk-0.0.7/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      775 2023-07-10 18:00:20.205415 bondzai.gateway-sdk-0.0.7/setup.cfg
```

### Comparing `bondzai.gateway-sdk-0.0.6/NOTICE` & `bondzai.gateway-sdk-0.0.7/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/PKG-INFO` & `bondzai.gateway-sdk-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/agent.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,30 +79,30 @@
 
     def on_log(self, callback: Callable[[Agent, str], None]) -> callable:
         cb_id = f"onlog-{len(self._on_log_handlers.keys())}"
         self._on_log_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_log_handlers", cb_id)
 
     def on_event(self, callback: Callable[[Agent, EventOperationID, dict], None]) -> callable:
-        cb_id = f"onevent-{len(self._on_log_handlers.keys())}"
+        cb_id = f"onevent-{len(self._on_event_handlers.keys())}"
         self._on_event_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_event_handlers", cb_id)
 
     def on_training_done(self, callback: Callable[[Agent, dict], None]) -> callable:
-        cb_id = f"ontraindone-{len(self._on_log_handlers.keys())}"
+        cb_id = f"ontraindone-{len(self._on_train_done_handlers.keys())}"
         self._on_train_done_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_train_handlers", cb_id)
 
     def on_inference_done(self, callback: Callable[[Agent, dict], None]) -> callable:
-        cb_id = f"oninferdone-{len(self._on_log_handlers.keys())}"
+        cb_id = f"oninferdone-{len(self._on_infer_done_handlers.keys())}"
         self._on_infer_done_handlers[cb_id] = callback
         return lambda: self.remove_observer("_on_infer_done_handlers", cb_id)
 
     def on_final_process_done(self, callback: Callable[[Agent, dict], None]) -> callable:
-        cb_id = f"onfinaldone-{len(self._on_log_handlers.keys())}"
+        cb_id = f"onfinaldone-{len(self._on_final_process_done.keys())}"
         self._on_final_process_done[cb_id] = callback
         return lambda: self.remove_observer("_on_final_process_done", cb_id)
 
     def send_message(self, message: Message, sync: bool = False):
         self.gateway.send(Request(
             RequestActions.ACT_SEND_TO_DEVICE,
             self.device_name,
```

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/commands.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/commands.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/enums.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
     OP_PARAM_PWSPAN = 0x90001302
     OP_PARAM_COMPRESS = 0x90001402
     OP_PARAM_MATRIX = 0x90001403
     OP_PARAM_EMPTY = 0x90008000
     OP_PARAM_MODE = 0x90008001
     OP_PARAM_REMOVENFIRST = 0x90008003
     OP_PARAM_SHAPE = 0x90008005
+    OP_PARAM_SLICE = 0x90008006
 
 
 class KPITypes(Enum):
     KPI_FREE = 0
     KPI_TRAINING_TIME_START = 1
     KPI_TRAINING_TIME_STOP = 2
     KPI_TRAINING_DATASET_SIZE = 3
```

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/events.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/gateway.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/gateway.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/message.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/message.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/request.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/timer.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/timer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/transcode.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/transcode.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai/gateway_sdk/utils.py` & `bondzai.gateway-sdk-0.0.7/bondzai/gateway_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/PKG-INFO` & `bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.6/bondzai.gateway_sdk.egg-info/SOURCES.txt` & `bondzai.gateway-sdk-0.0.7/bondzai.gateway_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/pyproject.toml` & `bondzai.gateway-sdk-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.6/setup.cfg` & `bondzai.gateway-sdk-0.0.7/setup.cfg`

 * *Files identical despite different names*

