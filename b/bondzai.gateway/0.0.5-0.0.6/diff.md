# Comparing `tmp/bondzai.gateway-0.0.5.tar.gz` & `tmp/bondzai.gateway-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-0.0.5.tar", last modified: Tue Jul  4 09:34:06 2023, max compression
+gzip compressed data, was "bondzai.gateway-0.0.6.tar", last modified: Mon Jul 10 17:59:57 2023, max compression
```

## Comparing `bondzai.gateway-0.0.5.tar` & `bondzai.gateway-0.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.763127 bondzai.gateway-0.0.5/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-04 09:34:06.763260 bondzai.gateway-0.0.5/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      195 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.747844 bondzai.gateway-0.0.5/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.750706 bondzai.gateway-0.0.5/bondzai/gateway/
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)      843 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/config.yml
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.752849 bondzai.gateway-0.0.5/bondzai/gateway/core/
--rw-r--r--   0 theo       (501) staff       (20)     7995 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/application.py
--rw-r--r--   0 theo       (501) staff       (20)      328 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/device.py
--rw-r--r--   0 theo       (501) staff       (20)      577 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/events.py
--rw-r--r--   0 theo       (501) staff       (20)      833 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/fsm.py
--rw-r--r--   0 theo       (501) staff       (20)     2127 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/logger.py
--rw-r--r--   0 theo       (501) staff       (20)     2590 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/manager.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.755313 bondzai.gateway-0.0.5/bondzai/gateway/core/message/
--rw-r--r--   0 theo       (501) staff       (20)     5391 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4968 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/command.py
--rw-r--r--   0 theo       (501) staff       (20)     6661 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     6771 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/event.py
--rw-r--r--   0 theo       (501) staff       (20)      337 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/payload.py
--rw-r--r--   0 theo       (501) staff       (20)     6821 2023-07-04 09:33:57.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/process_dbm.py
--rw-r--r--   0 theo       (501) staff       (20)     7864 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/response.py
--rw-r--r--   0 theo       (501) staff       (20)      942 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/message/utils.py
--rw-r--r--   0 theo       (501) staff       (20)     2276 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.756542 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/
--rw-r--r--   0 theo       (501) staff       (20)     1768 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/client.py
--rw-r--r--   0 theo       (501) staff       (20)     2652 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/connector.py
--rw-r--r--   0 theo       (501) staff       (20)     1731 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/request.py
--rw-r--r--   0 theo       (501) staff       (20)      171 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.758214 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/
--rw-r--r--   0 theo       (501) staff       (20)      201 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4426 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/serial.py
--rw-r--r--   0 theo       (501) staff       (20)     7630 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/socket_server.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.759113 bondzai.gateway-0.0.5/bondzai/gateway/tests/
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/tests/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2280 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/bondzai/gateway/tests/test_observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-04 09:34:06.762886 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1382 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)       57 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/entry_points.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)      117 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-04 09:34:06.000000 bondzai.gateway-0.0.5/bondzai.gateway.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-04 09:32:33.000000 bondzai.gateway-0.0.5/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      913 2023-07-04 09:34:06.764018 bondzai.gateway-0.0.5/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:57.027040 bondzai.gateway-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/NOTICE
+-rwxrwxrwx   0 root         (0) root         (0)      596 2023-07-10 17:59:57.028549 bondzai.gateway-0.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      195 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:55.529660 bondzai.gateway-0.0.6/bondzai/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:55.739199 bondzai.gateway-0.0.6/bondzai/gateway/
+-rwxrwxrwx   0 root         (0) root         (0)      775 2023-07-10 17:59:44.000000 bondzai.gateway-0.0.6/bondzai/gateway/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      843 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/config.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.021670 bondzai.gateway-0.0.6/bondzai/gateway/core/
+-rwxrwxrwx   0 root         (0) root         (0)     7995 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/application.py
+-rwxrwxrwx   0 root         (0) root         (0)      328 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/device.py
+-rwxrwxrwx   0 root         (0) root         (0)      577 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/events.py
+-rwxrwxrwx   0 root         (0) root         (0)      833 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/fsm.py
+-rwxrwxrwx   0 root         (0) root         (0)     2127 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2590 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.396433 bondzai.gateway-0.0.6/bondzai/gateway/core/message/
+-rwxrwxrwx   0 root         (0) root         (0)     5391 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     4968 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/command.py
+-rwxrwxrwx   0 root         (0) root         (0)     6693 2023-07-10 17:59:44.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/enums.py
+-rwxrwxrwx   0 root         (0) root         (0)     6771 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/event.py
+-rwxrwxrwx   0 root         (0) root         (0)      337 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/payload.py
+-rwxrwxrwx   0 root         (0) root         (0)     6821 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/process_dbm.py
+-rwxrwxrwx   0 root         (0) root         (0)     7864 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/response.py
+-rwxrwxrwx   0 root         (0) root         (0)      942 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/message/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2276 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/observer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.564713 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/
+-rwxrwxrwx   0 root         (0) root         (0)     1768 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/client.py
+-rwxrwxrwx   0 root         (0) root         (0)     2652 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/connector.py
+-rwxrwxrwx   0 root         (0) root         (0)     1731 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/request.py
+-rwxrwxrwx   0 root         (0) root         (0)      171 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.677460 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/
+-rwxrwxrwx   0 root         (0) root         (0)      201 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/base.py
+-rwxrwxrwx   0 root         (0) root         (0)     4426 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/serial.py
+-rwxrwxrwx   0 root         (0) root         (0)     7630 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/socket_server.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.751476 bondzai.gateway-0.0.6/bondzai/gateway/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2280 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/bondzai/gateway/tests/test_observer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-10 17:59:56.999090 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      596 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1382 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)      117 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-07-10 17:59:55.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-10 17:59:54.000000 bondzai.gateway-0.0.6/bondzai.gateway.egg-info/zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-07-10 17:56:57.000000 bondzai.gateway-0.0.6/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      913 2023-07-10 17:59:57.033070 bondzai.gateway-0.0.6/setup.cfg
```

### Comparing `bondzai.gateway-0.0.5/NOTICE` & `bondzai.gateway-0.0.6/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/PKG-INFO` & `bondzai.gateway-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.5
+Version: 0.0.6
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/__init__.py` & `bondzai.gateway-0.0.6/bondzai/gateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 from pathlib import Path
 
 from .core.application import Application, CONFIG_DEFAULT_PATH
 
 
 CMD_NAME = "bondzai.gateway"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 def run():
     parser = argparse.ArgumentParser(
         prog=CMD_NAME,
         description="Davinsy Gateway"
     )
```

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/config.yml` & `bondzai.gateway-0.0.6/bondzai/gateway/config.yml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/application.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/application.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/events.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/fsm.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/fsm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/logger.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/logger.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/manager.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/manager.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/message/base.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/message/base.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/message/command.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/message/command.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/message/enums.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/message/enums.py`

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

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/message/event.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/message/event.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/message/process_dbm.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/message/process_dbm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/message/response.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/message/response.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/message/utils.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/message/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/observer.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/client.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/client.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/connector.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/connector.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/core/websocket/request.py` & `bondzai.gateway-0.0.6/bondzai/gateway/core/websocket/request.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/serial.py` & `bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/serial.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/device_connectors/socket_server.py` & `bondzai.gateway-0.0.6/bondzai/gateway/device_connectors/socket_server.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai/gateway/tests/test_observer.py` & `bondzai.gateway-0.0.6/bondzai/gateway/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/bondzai.gateway.egg-info/PKG-INFO` & `bondzai.gateway-0.0.6/bondzai.gateway.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.5
+Version: 0.0.6
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.5/bondzai.gateway.egg-info/SOURCES.txt` & `bondzai.gateway-0.0.6/bondzai.gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.5/setup.cfg` & `bondzai.gateway-0.0.6/setup.cfg`

 * *Files identical despite different names*

