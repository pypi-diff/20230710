# Comparing `tmp/yolink-api-0.2.9.tar.gz` & `tmp/yolink-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolink-api-0.2.9.tar", last modified: Sun Apr 23 07:05:46 2023, max compression
+gzip compressed data, was "yolink-api-0.3.0.tar", last modified: Mon Jul 10 11:46:51 2023, max compression
```

## Comparing `yolink-api-0.2.9.tar` & `yolink-api-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:46.460615 yolink-api-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 07:05:40.000000 yolink-api-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-23 07:05:46.460615 yolink-api-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-23 07:05:40.000000 yolink-api-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 07:05:40.000000 yolink-api-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 07:05:46.460615 yolink-api-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-23 07:05:40.000000 yolink-api-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:46.460615 yolink-api-0.2.9/yolink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/auth_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/client_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/home_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/message_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/message_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/outlet_request_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-23 07:05:40.000000 yolink-api-0.2.9/yolink/thermostat_request_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:05:46.460615 yolink-api-0.2.9/yolink_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 07:05:46.000000 yolink-api-0.2.9/yolink_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:46:51.229193 yolink-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 11:46:48.000000 yolink-api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-10 11:46:51.229193 yolink-api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-10 11:46:48.000000 yolink-api-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 11:46:48.000000 yolink-api-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 11:46:51.229193 yolink-api-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-10 11:46:48.000000 yolink-api-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:46:51.229193 yolink-api-0.3.0/yolink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/auth_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/home_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/message_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/message_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/outlet_request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-10 11:46:48.000000 yolink-api-0.3.0/yolink/thermostat_request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 11:46:51.229193 yolink-api-0.3.0/yolink_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-10 11:46:51.000000 yolink-api-0.3.0/yolink_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-10 11:46:51.000000 yolink-api-0.3.0/yolink_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:46:51.000000 yolink-api-0.3.0/yolink_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 11:46:51.000000 yolink-api-0.3.0/yolink_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 11:46:51.000000 yolink-api-0.3.0/yolink_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 11:46:51.000000 yolink-api-0.3.0/yolink_api.egg-info/top_level.txt
```

### Comparing `yolink-api-0.2.9/LICENSE` & `yolink-api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/PKG-INFO` & `yolink-api-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolink-api
-Version: 0.2.9
+Version: 0.3.0
 Summary: A library to authenticate with yolink device
 Home-page: https://github.com/YoSmart-Inc/yolink-api
 Author: YoSmart
 License: MIT
 Project-URL: Bug Tracker, https://github.com/YoSmart-Inc/yolink-api/issues
 Keywords: yolink api
 Platform: UNKNOWN
```

### Comparing `yolink-api-0.2.9/README.md` & `yolink-api-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/setup.py` & `yolink-api-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="yolink-api",
-    version="0.2.9",
+    version="0.3.0",
     author="YoSmart",
     description="A library to authenticate with yolink device",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/YoSmart-Inc/yolink-api",
     project_urls={
         "Bug Tracker": "https://github.com/YoSmart-Inc/yolink-api/issues",
@@ -20,12 +20,12 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
         "aiohttp>=3.8.1",
-        "asyncio-mqtt>=0.16.1",
+        "aiomqtt>=1.0.0",
         "pydantic>=1.9.0",
         "tenacity>=8.1.0",
     ],
 )
```

### Comparing `yolink-api-0.2.9/yolink/auth_mgr.py` & `yolink-api-0.3.0/yolink/auth_mgr.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/yolink/client.py` & `yolink-api-0.3.0/yolink/client.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/yolink/const.py` & `yolink-api-0.3.0/yolink/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,7 +28,8 @@
 ATTR_DEVICE_THERMOSTAT = "Thermostat"
 ATTR_DEVICE_DIMMER = "Dimmer"
 ATTR_GARAGE_DOOR_CONTROLLER = "GarageDoor"
 ATTR_DEVICE_SMART_REMOTER = "SmartRemoter"
 ATTR_DEVICE_POWER_FAILURE_ALARM = "PowerFailureAlarm"
 ATTR_DEVICE_HUB = "Hub"
 ATTR_DEVICE_SPEAKER_HUB = "SpeakerHub"
+ATTR_DEVICE_FINGER = "Finger"
```

### Comparing `yolink-api-0.2.9/yolink/device.py` & `yolink-api-0.3.0/yolink/device.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/yolink/home_manager.py` & `yolink-api-0.3.0/yolink/home_manager.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/yolink/model.py` & `yolink-api-0.3.0/yolink/model.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/yolink/mqtt_client.py` & `yolink-api-0.3.0/yolink/mqtt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """YoLink mqtt client."""
 import asyncio
-import asyncio_mqtt as aiomqtt
 import logging
 from typing import Any
+import aiomqtt
 from pydantic import ValidationError
 from .auth_mgr import YoLinkAuthMgr
 from .const import (
     YOLINK_API_MQTT_BROKER,
     YOLINK_API_MQTT_BROKER_PORT,
     ATTR_DEVICE_SMART_REMOTER,
 )
@@ -60,14 +60,15 @@
                 await asyncio.sleep(reconnect_interval)
                 if isinstance(mqtt_err, aiomqtt.MqttCodeError):
                     if mqtt_err.rc in [4, 5]:
                         _LOGGER.error("token expired or invalid, acquire new one.")
                         await self._auth_mgr.check_and_refresh_token()
 
     async def disconnect(self) -> None:
+        """UnRegister listener"""
         if self._listener_task is None:
             return
         self._listener_task.cancel()
         self._listener_task = None
         self._running = False
 
     def _process_message(self, msg) -> None:
```

### Comparing `yolink-api-0.2.9/yolink/outlet_request_builder.py` & `yolink-api-0.3.0/yolink/outlet_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/yolink/thermostat_request_builder.py` & `yolink-api-0.3.0/yolink/thermostat_request_builder.py`

 * *Files identical despite different names*

### Comparing `yolink-api-0.2.9/yolink_api.egg-info/PKG-INFO` & `yolink-api-0.3.0/yolink_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolink-api
-Version: 0.2.9
+Version: 0.3.0
 Summary: A library to authenticate with yolink device
 Home-page: https://github.com/YoSmart-Inc/yolink-api
 Author: YoSmart
 License: MIT
 Project-URL: Bug Tracker, https://github.com/YoSmart-Inc/yolink-api/issues
 Keywords: yolink api
 Platform: UNKNOWN
```

### Comparing `yolink-api-0.2.9/yolink_api.egg-info/SOURCES.txt` & `yolink-api-0.3.0/yolink_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

