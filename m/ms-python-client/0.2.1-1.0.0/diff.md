# Comparing `tmp/ms_python_client-0.2.1.tar.gz` & `tmp/ms_python_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-0.2.1.tar", max compression
+gzip compressed data, was "ms_python_client-1.0.0.tar", max compression
```

## Comparing `ms_python_client-0.2.1.tar` & `ms_python_client-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1100 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/LICENSE
--rw-r--r--   0        0        0     5658 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/__init__.py
--rw-r--r--   0        0        0     5332 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/api_client.py
--rw-r--r--   0        0        0     1380 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/cern_ms_api_client.py
--rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0     3323 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/cern_events_component.py
--rw-r--r--   0        0        0     2459 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/events_component.py
--rw-r--r--   0        0        0      656 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/users_component.py
--rw-r--r--   0        0        0     5311 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/ms_api_client.py
--rw-r--r--   0        0        0     1023 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/ms_client_interface.py
--rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0      383 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/error.py
--rw-r--r--   0        0        0     4530 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/event_generator.py
--rw-r--r--   0        0        0       97 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/file_system.py
--rw-r--r--   0        0        0     1276 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/init_from_env.py
--rw-r--r--   0        0        0      729 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1033 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 ms_python_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5603 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5551 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/api_client.py
+-rw-r--r--   0        0        0     1380 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/cern_ms_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     3856 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/cern_events_component.py
+-rw-r--r--   0        0        0     3100 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/events_component.py
+-rw-r--r--   0        0        0      874 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/components/events/users_component.py
+-rw-r--r--   0        0        0     5696 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1312 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/error.py
+-rw-r--r--   0        0        0     5047 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/event_generator.py
+-rw-r--r--   0        0        0       97 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-10 10:07:48.624419 ms_python_client-1.0.0/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1033 2023-07-10 10:07:48.628419 ms_python_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 ms_python_client-1.0.0/PKG-INFO
```

### Comparing `ms_python_client-0.2.1/LICENSE` & `ms_python_client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.1/README.md` & `ms_python_client-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -128,44 +128,44 @@
 ```
 
 ### Available endpoints
 
 #### **events**:
 
 1. get all events
-2. get a single event using indico id
+2. get a single event using zoom id
 3. create an event
-4. update an event using indico id
-5. delete an event using indico id
+4. update an event using zoom id
+5. delete an event using zoom id
 
 You will find useful the `EventParameters` and `PartialEventParameters` classes, which will help you to create the events.
 
-- `INDICO_EVENT_ID` is the id of the event in the indico system which is **mandatory** to create an event.
+- `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link, is **mandatory** to create an event.
 - `USER_ID` is the email of the Zoom Room.
 
 ```python
 from ms_python_client.cern_ms_api_client import CERNMSApiClient
 from ms_python_client.utils.event_generator import (EventParameters, PartialEventParameters)
 
 cern_ms_client = CERNMSApiClient.init_from_dotenv()
 
 USER_ID = os.getenv("USER_ID") # Which is the email of the Zoom Room
-INDICO_EVENT_ID = os.getenv("INDICO_EVENT_ID")
+ZOOM = os.getenv("ZOOM")
 
 event_parameters = EventParameters(
         subject="Test meeting",
         start_time="2021-10-01T12:00:00",
         end_time="2021-10-01T13:00:00",
         timezone="Europe/Zurich",
-        indico_event_id=INDICO_EVENT_ID,
+        zoom_id=ZOOM,
         zoom_url="https://cern.zoom.us/******",
 )
 
 partial_event_parameters = PartialEventParameters(
-        indico_event_id=INDICO_EVENT_ID,
+        zoom_id=ZOOM,
         end_time="2021-10-01T14:00:00",
 ) # You can update only the end_time of the event for example
 
 cern_ms_client.events.create_event(USER_ID, event_parameters)
-cern_ms_client.events.update_event_by_indico_id(USER_ID, partial_event_parameters)
-cern_ms_client.events.delete_event_by_indico_id(USER_ID, INDICO_EVENT_ID)
+cern_ms_client.events.update_event_by_zoom_id(USER_ID, partial_event_parameters)
+cern_ms_client.events.delete_event_by_zoom_id(USER_ID, ZOOM)
 ```
```

### Comparing `ms_python_client-0.2.1/ms_python_client/api_client.py` & `ms_python_client-1.0.0/ms_python_client/api_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import logging
+from typing import Any, Mapping, Optional
 
 from requests import RequestException, Response, Session
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 logger = logging.getLogger("ms_python_client")
 
+_Headers = Mapping[str, str]
+_Data = Mapping[str, Any]
+
 
 class ApiClient:
     def __init__(self, api_base_url: str):
         self.api_base_url = api_base_url
         self.timeout = 10
         self.session = Session()
         retry_strategy = Retry(
@@ -18,41 +22,41 @@
             status_forcelist=[429, 500, 502, 503, 504],
             allowed_methods=["HEAD", "GET", "PUT", "DELETE", "OPTIONS"],
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
         self.session.mount("http://", adapter)
         self.session.mount("https://", adapter)
 
-    def build_headers(self, extra_headers=None) -> dict:
+    def build_headers(self, extra_headers: Optional[_Headers] = None) -> dict:
         """Create the headers for a request appending the ones in the params
 
         Args:
-            extra_headers (dict): Dict of headers that will be appended to the default ones
+            extra_headers (dict): Mapping of headers that will be appended to the default ones
 
         Returns:
             dict: All the headers
         """
-        headers = {"Content-type": "application/json"}
+        headers: dict[str, str] = {}
         if extra_headers:
             headers.update(extra_headers)
         return headers
 
-    def make_get_request(self, api_path: str, headers: dict) -> Response:
+    def make_get_request(self, api_path: str, headers: _Headers) -> Response:
         """Makes a GET request using requests
 
         Args:
             api_path (str): The URL path
             headers (dict): The headers of the request
 
         Returns:
             Response: The response of the request
         """
         response = None
         full_url = self.api_base_url + api_path
-        logger.debug("GET %s", api_path)
+        logger.info("GET %s", api_path)
         try:
             response = self.session.get(full_url, headers=headers, timeout=self.timeout)
             response.raise_for_status()
         except RequestException as e:
             logger.error(e)
             if isinstance(response, Response) and response.text:
                 logger.error(response.text)
@@ -61,31 +65,33 @@
             "GET [%s] - %d in %fs",
             api_path,
             response.status_code,
             response.elapsed.total_seconds(),
         )
         return response
 
-    def make_post_request(self, api_path: str, headers=None, data=None) -> Response:
+    def make_post_request(
+        self, api_path: str, headers: _Headers, json: Optional[_Data] = None
+    ) -> Response:
         """Makes a POST request using requests
 
         Args:
             api_path (str): The URL path
             headers (dict): The headers of the request
-            data (dict): The body of the request
+            json (dict): The body of the request
 
         Returns:
             Response: The response of the request
         """
         response = None
         full_url = self.api_base_url + api_path
-        logger.debug("POST %s", api_path)
+        logger.info("POST %s", api_path)
         try:
             response = self.session.post(
-                full_url, headers=headers, data=data, timeout=self.timeout
+                full_url, headers=headers, json=json, timeout=self.timeout
             )
             response.raise_for_status()
         except RequestException as e:
             logger.error(e)
             if isinstance(response, Response) and response.text:
                 logger.error(response.text)
             raise e
@@ -93,31 +99,33 @@
             "POST [%s] - %d in %fs",
             api_path,
             response.status_code,
             response.elapsed.total_seconds(),
         )
         return response
 
-    def make_patch_request(self, api_path: str, headers=None, data=None) -> Response:
+    def make_patch_request(
+        self, api_path: str, headers: _Headers, json: Optional[_Data] = None
+    ) -> Response:
         """Makes a PATCH request using requests
 
         Args:
             api_path (str): The URL path
             headers (dict): The headers of the request
-            data (dict): The body of the request
+            json (dict): The body of the request
 
         Returns:
             Response: The response of the request
         """
         response = None
         full_url = self.api_base_url + api_path
-        logger.debug("PATCH %s", api_path)
+        logger.info("PATCH %s", api_path)
         try:
             response = self.session.patch(
-                full_url, headers=headers, data=data, timeout=self.timeout
+                full_url, headers=headers, json=json, timeout=self.timeout
             )
             response.raise_for_status()
         except RequestException as e:
             logger.error(e)
             if isinstance(response, Response) and response.text:
                 logger.error(response.text)
             raise e
@@ -125,31 +133,33 @@
             "PATCH [%s] - %d in %fs",
             api_path,
             response.status_code,
             response.elapsed.total_seconds(),
         )
         return response
 
-    def make_delete_request(self, api_path: str, headers=None, data=None) -> Response:
+    def make_delete_request(
+        self, api_path: str, headers: _Headers, json: Optional[_Data] = None
+    ) -> Response:
         """Makes a DELETE request using requests
 
         Args:
             api_path (str): The URL path
             headers (dict): The headers of the request
-            data (dict): The body of the request
+            json (dict): The body of the request
 
         Returns:
             Response: The response of the request
         """
         response = None
         full_url = self.api_base_url + api_path
-        logger.debug("DELETE %s", api_path)
+        logger.info("DELETE %s", api_path)
         try:
             response = self.session.delete(
-                full_url, headers=headers, data=data, timeout=self.timeout
+                full_url, headers=headers, json=json, timeout=self.timeout
             )
             response.raise_for_status()
         except RequestException as e:
             logger.error(e)
             if isinstance(response, Response) and response.text:
                 logger.error(response.text)
             raise e
```

### Comparing `ms_python_client-0.2.1/ms_python_client/cern_ms_api_client.py` & `ms_python_client-1.0.0/ms_python_client/cern_ms_api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.1/ms_python_client/components/events/cern_events_component.py` & `ms_python_client-1.0.0/ms_python_client/components/events/cern_events_component.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,86 +24,111 @@
 class CERNEventsComponents:
     """CERN Events component"""
 
     def __init__(self, client: MSClientInterface) -> None:
         self.events_component = EventsComponent(client)
 
     def list_events(
-        self, user_id: str, parameters: Optional[Mapping[str, str]] = None
+        self,
+        user_id: str,
+        parameters: Optional[Mapping[str, str]] = None,
+        extra_headers: Optional[Mapping[str, str]] = None,
     ) -> dict:
         """List all the events of a user
 
         Args:
             user_id (str): The user id
             parameters (dict): Optional parameters for the request
 
         Returns:
             dict: The response of the request
         """
-        return self.events_component.list_events(user_id, parameters)
+        return self.events_component.list_events(user_id, parameters, extra_headers)
 
-    def get_event_by_indico_id(self, user_id: str, indico_id: str) -> dict:
+    def get_event_by_zoom_id(
+        self,
+        user_id: str,
+        zoom_id: str,
+        extra_headers: Optional[Mapping[str, str]] = None,
+    ) -> dict:
         """Get an event of a user
 
         Args:
-            indico_id (str): The event id
+            zoom_id (str): The event id
 
         Returns:
             dict: The response of the request
         """
-        parameters = {"$count": "true", "$filter": f"contains(subject,'{indico_id}')"}
-        response = self.events_component.list_events(user_id, parameters)
+        parameters = {"$count": "true", "$filter": f"contains(subject,'{zoom_id}')"}
+        response = self.events_component.list_events(user_id, parameters, extra_headers)
 
         count = response.get("@odata.count", 0)
         if count == 0:
-            raise NotFoundError(f"Event with indico id {indico_id} not found")
+            raise NotFoundError(f"Event with zoom id {zoom_id} not found")
 
         if count > 1:
             logger.warning(
-                "Found %s events with indico id %s. Returning the first one.",
+                "Found %s events with zoom id %s. Returning the first one.",
                 count,
-                indico_id,
+                zoom_id,
             )
 
         return response.get("value", [])[0]
 
-    def create_event(self, user_id: str, event: EventParameters) -> dict:
+    def create_event(
+        self,
+        user_id: str,
+        event: EventParameters,
+        extra_headers: Optional[Mapping[str, str]] = None,
+    ) -> dict:
         """Create an event for a user
 
         Args:
             user_id (str): The user id
             event (EventParameters): The event data
 
         Returns:
             dict: The response of the request
         """
-        data = create_event_body(event)
-        return self.events_component.create_event(user_id, data)
+        json = create_event_body(event)
+        return self.events_component.create_event(user_id, json, extra_headers)
 
-    def update_event_by_indico_id(
-        self, user_id: str, event: PartialEventParameters
+    def update_event_by_zoom_id(
+        self,
+        user_id: str,
+        event: PartialEventParameters,
+        extra_headers: Optional[Mapping[str, str]] = None,
     ) -> dict:
         """Update an event for a user
 
         Args:
             user_id (str): The user id
             event (EventParameters): The event parameters
 
         Returns:
             dict: The response of the request
         """
-        data = create_partial_event_body(event)
-        event_id = self.get_event_by_indico_id(user_id, event["indico_event_id"])["id"]
-        return self.events_component.update_event(user_id, event_id, data)
-
-    def delete_event_by_indico_id(self, user_id: str, indico_id: str) -> None:
+        json = create_partial_event_body(event)
+        event_id = self.get_event_by_zoom_id(user_id, event["zoom_id"], extra_headers)[
+            "id"
+        ]
+        return self.events_component.update_event(
+            user_id, event_id, json, extra_headers
+        )
+
+    def delete_event_by_zoom_id(
+        self,
+        user_id: str,
+        zoom_id: str,
+        extra_headers: Optional[Mapping[str, str]] = None,
+    ) -> None:
         """Delete an event of a user
 
         Args:
             user_id (str): The user id
-            indico_id (str): The event id
+            zoom_id (str): The event id
 
         Returns:
             dict: The response of the request
         """
-        event_id = self.get_event_by_indico_id(user_id, indico_id)["id"]
-        self.events_component.delete_event(user_id, event_id)
+        event_id = self.get_event_by_zoom_id(user_id, zoom_id, extra_headers)["id"]
+        self.events_component.delete_event(user_id, event_id, extra_headers)
```

### Comparing `ms_python_client-0.2.1/ms_python_client/components/events/events_component.py` & `ms_python_client-1.0.0/ms_python_client/components/events/events_component.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,78 +4,106 @@
 
 
 class EventsComponent:
     def __init__(self, client: MSClientInterface) -> None:
         self.client = client
 
     def list_events(
-        self, user_id: str, parameters: Optional[Mapping[str, str]] = None
+        self,
+        user_id: str,
+        parameters: Optional[Mapping[str, str]] = None,
+        extra_headers: Optional[Mapping[str, str]] = None,
     ) -> dict:
         """List all the events of a user
 
         Args:
             user_id (str): The user id
 
         Returns:
             dict: The response of the request
         """
         api_path = f"/users/{user_id}/calendar/events"
-        response = self.client.make_get_request(api_path, parameters)
+        response = self.client.make_get_request(
+            api_path, parameters, extra_headers=extra_headers
+        )
         return response.json()
 
-    def get_event(self, user_id: str, event_id: str) -> dict:
+    def get_event(
+        self,
+        user_id: str,
+        event_id: str,
+        extra_headers: Optional[Mapping[str, str]] = None,
+    ) -> dict:
         """Get an event of a user
 
         Args:
             user_id (str): The user id
             event_id (str): The event id
 
         Returns:
             dict: The response of the request
         """
         api_path = f"/users/{user_id}/calendar/events/{event_id}"
-        response = self.client.make_get_request(api_path)
+        response = self.client.make_get_request(api_path, extra_headers=extra_headers)
         return response.json()
 
-    def create_event(self, user_id: str, data: Mapping[str, Any]) -> dict:
+    def create_event(
+        self,
+        user_id: str,
+        json: Mapping[str, Any],
+        extra_headers: Optional[Mapping[str, str]] = None,
+    ) -> dict:
         """Create an event for a user
 
         Args:
             user_id (str): The user id
             data (Mapping[str, Any]): The event data
 
         Returns:
             dict: The response of the request
         """
         api_path = f"/users/{user_id}/calendar/events"
-        response = self.client.make_post_request(api_path, data)
+        response = self.client.make_post_request(
+            api_path, json, extra_headers=extra_headers
+        )
         return response.json()
 
     def update_event(
-        self, user_id: str, event_id: str, data: Mapping[str, Any]
+        self,
+        user_id: str,
+        event_id: str,
+        json: Mapping[str, Any],
+        extra_headers: Optional[Mapping[str, str]] = None,
     ) -> dict:
         """Update an event for a user
 
         Args:
             user_id (str): The user id
             event_id (str): The event id
             data (Mapping[str, Any]): The event parameters
 
         Returns:
             dict: The response of the request
         """
         api_path = f"/users/{user_id}/calendar/events/{event_id}"
-        response = self.client.make_patch_request(api_path, data)
+        response = self.client.make_patch_request(
+            api_path, json, extra_headers=extra_headers
+        )
         return response.json()
 
-    def delete_event(self, user_id: str, event_id: str) -> None:
+    def delete_event(
+        self,
+        user_id: str,
+        event_id: str,
+        extra_headers: Optional[Mapping[str, str]] = None,
+    ) -> None:
         """Delete an event of a user
 
         Args:
             user_id (str): The user id
             event_id (str): The event id
 
         Returns:
             dict: The response of the request
         """
         api_path = f"/users/{user_id}/calendar/events/{event_id}"
-        self.client.make_delete_request(api_path)
+        self.client.make_delete_request(api_path, extra_headers=extra_headers)
```

### Comparing `ms_python_client-0.2.1/ms_python_client/ms_api_client.py` & `ms_python_client-1.0.0/ms_python_client/ms_api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import atexit
-import json
 import logging
 import os
 from typing import Any, Mapping, Optional
 
 import requests
 from msal import ConfidentialClientApplication, SerializableTokenCache
 
@@ -12,15 +11,16 @@
 from ms_python_client.components.events.users_component import UsersComponent
 from ms_python_client.ms_client_interface import MSClientInterface
 from ms_python_client.utils import init_from_env
 
 logging.getLogger("ms_python_client").addHandler(logging.NullHandler())
 logger = logging.getLogger("ms_python_client")
 
-TypeData = Mapping[str, Any]
+_Data = Mapping[str, Any]
+_Headers = Mapping[str, str]
 
 
 class MSApiClient(MSClientInterface):
     @staticmethod
     def init_from_env(use_path: Optional[str] = None) -> "MSApiClient":
         values = init_from_env.init_from_env(use_path)
         ms_client = MSApiClient(
@@ -79,15 +79,15 @@
                     self.setup_cache(use_path + "/token_cache.bin")
                     if use_path
                     else None
                 ),
             )
         self.init_components()
 
-    def build_headers(self) -> dict:
+    def build_headers(self, extra_headers: Optional[_Headers] = None) -> _Headers:
         if "MS_ACCESS_TOKEN" in os.environ:
             token = {
                 "access_token": os.environ["MS_ACCESS_TOKEN"],
             }
         else:
             result = self.app.acquire_token_silent(
                 scopes=["https://graph.microsoft.com/.default"], account=None
@@ -100,57 +100,68 @@
                     scopes=["https://graph.microsoft.com/.default"]
                 )
             else:
                 token = result
         headers = self.api_client.build_headers(
             extra_headers={"Authorization": f"Bearer {token['access_token']}"}
         )
+        if extra_headers:
+            headers.update(extra_headers)
         return headers
 
     def build_query_string_from_dict(
         self, parameters: Optional[Mapping[str, str]]
     ) -> str:
         query_string = "?"
         for key, value in parameters.items() if parameters else []:
             if value:
                 query_string += f"{key}={value}&"
         return query_string[:-1]
 
     def make_get_request(
-        self, api_path: str, parameters: Optional[Mapping[str, str]] = None
+        self,
+        api_path: str,
+        parameters: Optional[Mapping[str, str]] = None,
+        extra_headers: Optional[_Headers] = None,
     ) -> requests.Response:
-        headers = self.build_headers()
+        headers = self.build_headers(extra_headers)
         query_string = self.build_query_string_from_dict(parameters)
 
         response = self.api_client.make_get_request(
             api_path=f"{api_path}{query_string}",
             headers=headers,
         )
 
         return response
 
-    def make_post_request(self, api_path: str, data: TypeData) -> requests.Response:
-        headers = self.build_headers()
+    def make_post_request(
+        self, api_path: str, json: _Data, extra_headers: Optional[_Headers] = None
+    ) -> requests.Response:
+        headers = self.build_headers(extra_headers)
 
         response = self.api_client.make_post_request(
-            api_path=api_path, headers=headers, data=json.dumps(data)
+            api_path=api_path, headers=headers, json=json
         )
 
         return response
 
-    def make_patch_request(self, api_path: str, data: TypeData) -> requests.Response:
-        headers = self.build_headers()
+    def make_patch_request(
+        self, api_path: str, json: _Data, extra_headers: Optional[_Headers] = None
+    ) -> requests.Response:
+        headers = self.build_headers(extra_headers)
 
         response = self.api_client.make_patch_request(
-            api_path=api_path, headers=headers, data=json.dumps(data)
+            api_path=api_path, headers=headers, json=json
         )
 
         return response
 
-    def make_delete_request(self, api_path: str) -> requests.Response:
-        headers = self.build_headers()
+    def make_delete_request(
+        self, api_path: str, extra_headers: Optional[_Headers] = None
+    ) -> requests.Response:
+        headers = self.build_headers(extra_headers)
 
         response = self.api_client.make_delete_request(
             api_path=api_path, headers=headers
         )
 
         return response
```

### Comparing `ms_python_client-0.2.1/ms_python_client/utils/event_generator.py` & `ms_python_client-1.0.0/ms_python_client/utils/event_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import TypedDict
 
 
 class BaseEventParameters(TypedDict):
     """Base parameters for creating an event
 
     Args:
-        indico_event_id (str): The indico event id
+        zoom_id (str): The zoom event id
     """
 
-    indico_event_id: str
+    zoom_id: str
 
 
 class OptionalTimezone(TypedDict, total=False):
     """Optional timezone parameter for creating an event
 
     Args:
         timezone (str): The timezone of the event
@@ -62,16 +62,22 @@
 
     Returns:
         Event: The event
     """
 
     timezone = event_parameters.get("timezone", "Europe/Zurich")
 
+    zoom_id_from_url = event_parameters["zoom_url"].split("/")[-1].split("?")[0]
+    if zoom_id_from_url != event_parameters["zoom_id"]:
+        raise ValueError(
+            "The zoom_id from the url does not match the zoom_id from the event parameters"
+        )
+
     return {
-        "subject": f"[{event_parameters['indico_event_id']}] {event_parameters['subject']}",
+        "subject": f"[{event_parameters['zoom_id']}] {event_parameters['subject']}",
         "body": {
             "contentType": "text",
             "content": f"Zoom URL: {event_parameters['zoom_url']}",
         },
         "start": {
             "dateTime": datetime.datetime.fromisoformat(
                 event_parameters["start_time"]
@@ -108,14 +114,19 @@
         Event: The event
     """
     event = {}
 
     timezone = event_parameters.get("timezone", "Europe/Zurich")
 
     if "zoom_url" in event_parameters:
+        zoom_id_from_url = event_parameters["zoom_url"].split("/")[-1].split("?")[0]
+        if zoom_id_from_url != event_parameters["zoom_id"]:
+            raise ValueError(
+                "The zoom_id from the url does not match the zoom_id from the event parameters"
+            )
         event.update(
             {
                 "body": {
                     "contentType": "text",
                     "content": f"Zoom URL: {event_parameters['zoom_url']}",
                 },
                 "location": {
@@ -127,15 +138,15 @@
                 "onlineMeetingUrl": event_parameters["zoom_url"],
             }
         )
 
     if "subject" in event_parameters:
         event.update(
             {
-                "subject": f"[{event_parameters['indico_event_id']}] {event_parameters['subject']}"
+                "subject": f"[{event_parameters['zoom_id']}] {event_parameters['subject']}"
             }
         )
 
     if "start_time" in event_parameters:
         event.update(
             {
                 "start": {
```

### Comparing `ms_python_client-0.2.1/ms_python_client/utils/init_from_env.py` & `ms_python_client-1.0.0/ms_python_client/utils/init_from_env.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.1/ms_python_client/utils/logger.py` & `ms_python_client-1.0.0/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.1/pyproject.toml` & `ms_python_client-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "0.2.1"
+version = "1.0.0"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
```

### Comparing `ms_python_client-0.2.1/PKG-INFO` & `ms_python_client-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 0.2.1
+Version: 1.0.0
 Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -148,45 +148,45 @@
 ```
 
 ### Available endpoints
 
 #### **events**:
 
 1. get all events
-2. get a single event using indico id
+2. get a single event using zoom id
 3. create an event
-4. update an event using indico id
-5. delete an event using indico id
+4. update an event using zoom id
+5. delete an event using zoom id
 
 You will find useful the `EventParameters` and `PartialEventParameters` classes, which will help you to create the events.
 
-- `INDICO_EVENT_ID` is the id of the event in the indico system which is **mandatory** to create an event.
+- `ZOOM_ID` is the id of the zoom meeting, which can be found inside the url of a meeting link, is **mandatory** to create an event.
 - `USER_ID` is the email of the Zoom Room.
 
 ```python
 from ms_python_client.cern_ms_api_client import CERNMSApiClient
 from ms_python_client.utils.event_generator import (EventParameters, PartialEventParameters)
 
 cern_ms_client = CERNMSApiClient.init_from_dotenv()
 
 USER_ID = os.getenv("USER_ID") # Which is the email of the Zoom Room
-INDICO_EVENT_ID = os.getenv("INDICO_EVENT_ID")
+ZOOM = os.getenv("ZOOM")
 
 event_parameters = EventParameters(
         subject="Test meeting",
         start_time="2021-10-01T12:00:00",
         end_time="2021-10-01T13:00:00",
         timezone="Europe/Zurich",
-        indico_event_id=INDICO_EVENT_ID,
+        zoom_id=ZOOM,
         zoom_url="https://cern.zoom.us/******",
 )
 
 partial_event_parameters = PartialEventParameters(
-        indico_event_id=INDICO_EVENT_ID,
+        zoom_id=ZOOM,
         end_time="2021-10-01T14:00:00",
 ) # You can update only the end_time of the event for example
 
 cern_ms_client.events.create_event(USER_ID, event_parameters)
-cern_ms_client.events.update_event_by_indico_id(USER_ID, partial_event_parameters)
-cern_ms_client.events.delete_event_by_indico_id(USER_ID, INDICO_EVENT_ID)
+cern_ms_client.events.update_event_by_zoom_id(USER_ID, partial_event_parameters)
+cern_ms_client.events.delete_event_by_zoom_id(USER_ID, ZOOM)
 ```
```

