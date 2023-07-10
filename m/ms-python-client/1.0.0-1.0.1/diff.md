# Comparing `tmp/ms_python_client-1.0.0.tar.gz` & `tmp/ms_python_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-1.0.0.tar", max compression
+gzip compressed data, was "ms_python_client-1.0.1.tar", max compression
```

## Comparing `ms_python_client-1.0.0.tar` & `ms_python_client-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1100 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/LICENSE
--rw-r--r--   0        0        0     5603 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/__init__.py
--rw-r--r--   0        0        0     5551 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/api_client.py
--rw-r--r--   0        0        0     1380 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/cern_ms_api_client.py
--rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0     3856 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/cern_events_component.py
--rw-r--r--   0        0        0     3100 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/events_component.py
--rw-r--r--   0        0        0      874 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/users_component.py
--rw-r--r--   0        0        0     5696 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/ms_api_client.py
--rw-r--r--   0        0        0     1312 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/ms_client_interface.py
--rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0      383 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/error.py
--rw-r--r--   0        0        0     5047 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/event_generator.py
--rw-r--r--   0        0        0       97 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/file_system.py
--rw-r--r--   0        0        0     1276 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/init_from_env.py
--rw-r--r--   0        0        0      729 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1033 2023-07-10 10:07:48.628419 ms_python_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 ms_python_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5657 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5551 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/api_client.py
+-rw-r--r--   0        0        0     1380 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/cern_ms_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     3856 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/cern_events_component.py
+-rw-r--r--   0        0        0     3100 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/events_component.py
+-rw-r--r--   0        0        0      874 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/components/events/users_component.py
+-rw-r--r--   0        0        0     5696 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1312 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/error.py
+-rw-r--r--   0        0        0     5047 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/event_generator.py
+-rw-r--r--   0        0        0       97 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1033 2023-07-10 10:26:06.200168 ms_python_client-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6461 1970-01-01 00:00:00.000000 ms_python_client-1.0.1/PKG-INFO
```

### Comparing `ms_python_client-1.0.0/LICENSE` & `ms_python_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/README.md` & `ms_python_client-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,18 @@
 
 1. get all events
 2. get a single event
 3. create an event
 4. update an event
 5. delete an event
 
+### **users**:
+
+1. get all users
+
 ## CERN specific usage
 
 Instead of using the `MSApiClient` class, you can use the `CERNMSApiClient` class, which is a subclass of the `MSApiClient` class.
 This class will provide you some more utilities but it will only work for CERN users (obviously).
 
 This will be used in the context of synchronizing the events between the CERN Indico system and the calendars of the Zoom Rooms.
 
@@ -135,37 +139,37 @@
 2. get a single event using zoom id
 3. create an event
 4. update an event using zoom id
 5. delete an event using zoom id
 
 You will find useful the `EventParameters` and `PartialEventParameters` classes, which will help you to create the events.
 
-- `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link, is **mandatory** to create an event.
+- `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link. This is **mandatory** to create an event.
 - `USER_ID` is the email of the Zoom Room.
 
 ```python
 from ms_python_client.cern_ms_api_client import CERNMSApiClient
 from ms_python_client.utils.event_generator import (EventParameters, PartialEventParameters)
 
 cern_ms_client = CERNMSApiClient.init_from_dotenv()
 
 USER_ID = os.getenv("USER_ID") # Which is the email of the Zoom Room
-ZOOM = os.getenv("ZOOM")
+ZOOM_ID = os.getenv("ZOOM_ID")
 
 event_parameters = EventParameters(
         subject="Test meeting",
         start_time="2021-10-01T12:00:00",
         end_time="2021-10-01T13:00:00",
         timezone="Europe/Zurich",
-        zoom_id=ZOOM,
+        zoom_id=ZOOM_ID,
         zoom_url="https://cern.zoom.us/******",
 )
 
 partial_event_parameters = PartialEventParameters(
-        zoom_id=ZOOM,
+        zoom_id=ZOOM_ID,
         end_time="2021-10-01T14:00:00",
 ) # You can update only the end_time of the event for example
 
 cern_ms_client.events.create_event(USER_ID, event_parameters)
 cern_ms_client.events.update_event_by_zoom_id(USER_ID, partial_event_parameters)
-cern_ms_client.events.delete_event_by_zoom_id(USER_ID, ZOOM)
+cern_ms_client.events.delete_event_by_zoom_id(USER_ID, ZOOM_ID)
 ```
```

### Comparing `ms_python_client-1.0.0/ms_python_client/api_client.py` & `ms_python_client-1.0.1/ms_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/cern_ms_api_client.py` & `ms_python_client-1.0.1/ms_python_client/cern_ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/components/events/cern_events_component.py` & `ms_python_client-1.0.1/ms_python_client/components/events/cern_events_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/components/events/events_component.py` & `ms_python_client-1.0.1/ms_python_client/components/events/events_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/components/events/users_component.py` & `ms_python_client-1.0.1/ms_python_client/components/events/users_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/ms_api_client.py` & `ms_python_client-1.0.1/ms_python_client/ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/ms_client_interface.py` & `ms_python_client-1.0.1/ms_python_client/ms_client_interface.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/utils/event_generator.py` & `ms_python_client-1.0.1/ms_python_client/utils/event_generator.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/utils/init_from_env.py` & `ms_python_client-1.0.1/ms_python_client/utils/init_from_env.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/ms_python_client/utils/logger.py` & `ms_python_client-1.0.1/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-1.0.0/pyproject.toml` & `ms_python_client-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "1.0.0"
+version = "1.0.1"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
```

### Comparing `ms_python_client-1.0.0/PKG-INFO` & `ms_python_client-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -126,14 +126,18 @@
 
 1. get all events
 2. get a single event
 3. create an event
 4. update an event
 5. delete an event
 
+### **users**:
+
+1. get all users
+
 ## CERN specific usage
 
 Instead of using the `MSApiClient` class, you can use the `CERNMSApiClient` class, which is a subclass of the `MSApiClient` class.
 This class will provide you some more utilities but it will only work for CERN users (obviously).
 
 This will be used in the context of synchronizing the events between the CERN Indico system and the calendars of the Zoom Rooms.
 
@@ -155,38 +159,38 @@
 2. get a single event using zoom id
 3. create an event
 4. update an event using zoom id
 5. delete an event using zoom id
 
 You will find useful the `EventParameters` and `PartialEventParameters` classes, which will help you to create the events.
 
-- `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link, is **mandatory** to create an event.
+- `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link. This is **mandatory** to create an event.
 - `USER_ID` is the email of the Zoom Room.
 
 ```python
 from ms_python_client.cern_ms_api_client import CERNMSApiClient
 from ms_python_client.utils.event_generator import (EventParameters, PartialEventParameters)
 
 cern_ms_client = CERNMSApiClient.init_from_dotenv()
 
 USER_ID = os.getenv("USER_ID") # Which is the email of the Zoom Room
-ZOOM = os.getenv("ZOOM")
+ZOOM_ID = os.getenv("ZOOM_ID")
 
 event_parameters = EventParameters(
         subject="Test meeting",
         start_time="2021-10-01T12:00:00",
         end_time="2021-10-01T13:00:00",
         timezone="Europe/Zurich",
-        zoom_id=ZOOM,
+        zoom_id=ZOOM_ID,
         zoom_url="https://cern.zoom.us/******",
 )
 
 partial_event_parameters = PartialEventParameters(
-        zoom_id=ZOOM,
+        zoom_id=ZOOM_ID,
         end_time="2021-10-01T14:00:00",
 ) # You can update only the end_time of the event for example
 
 cern_ms_client.events.create_event(USER_ID, event_parameters)
 cern_ms_client.events.update_event_by_zoom_id(USER_ID, partial_event_parameters)
-cern_ms_client.events.delete_event_by_zoom_id(USER_ID, ZOOM)
+cern_ms_client.events.delete_event_by_zoom_id(USER_ID, ZOOM_ID)
 ```
```

