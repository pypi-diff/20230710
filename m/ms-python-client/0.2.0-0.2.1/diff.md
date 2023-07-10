# Comparing `tmp/ms_python_client-0.2.0.tar.gz` & `tmp/ms_python_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_python_client-0.2.0.tar", max compression
+gzip compressed data, was "ms_python_client-0.2.1.tar", max compression
```

## Comparing `ms_python_client-0.2.0.tar` & `ms_python_client-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1100 2023-07-07 19:29:16.862865 ms_python_client-0.2.0/LICENSE
--rw-r--r--   0        0        0     5658 2023-07-07 19:29:16.862865 ms_python_client-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/__init__.py
--rw-r--r--   0        0        0     5332 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/api_client.py
--rw-r--r--   0        0        0     1493 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/cern_ms_api_client.py
--rw-r--r--   0        0        0        0 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/components/events/__init__.py
--rw-r--r--   0        0        0     3323 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/components/events/cern_events_component.py
--rw-r--r--   0        0        0     2459 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/components/events/events_component.py
--rw-r--r--   0        0        0     5222 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/ms_api_client.py
--rw-r--r--   0        0        0     1023 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/ms_client_interface.py
--rw-r--r--   0        0        0        0 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/utils/__init__.py
--rw-r--r--   0        0        0     4530 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/utils/event_generator.py
--rw-r--r--   0        0        0       97 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/utils/file_system.py
--rw-r--r--   0        0        0     1276 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/utils/init_from_env.py
--rw-r--r--   0        0        0      729 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/ms_python_client/utils/logger.py
--rw-r--r--   0        0        0     1034 2023-07-07 19:29:16.866865 ms_python_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 ms_python_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5658 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/__init__.py
+-rw-r--r--   0        0        0     5332 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/api_client.py
+-rw-r--r--   0        0        0     1380 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/cern_ms_api_client.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/__init__.py
+-rw-r--r--   0        0        0     3323 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/cern_events_component.py
+-rw-r--r--   0        0        0     2459 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/events_component.py
+-rw-r--r--   0        0        0      656 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/components/events/users_component.py
+-rw-r--r--   0        0        0     5311 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/ms_api_client.py
+-rw-r--r--   0        0        0     1023 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/ms_client_interface.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      383 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/error.py
+-rw-r--r--   0        0        0     4530 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/event_generator.py
+-rw-r--r--   0        0        0       97 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/file_system.py
+-rw-r--r--   0        0        0     1276 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/init_from_env.py
+-rw-r--r--   0        0        0      729 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/ms_python_client/utils/logger.py
+-rw-r--r--   0        0        0     1033 2023-07-10 08:25:01.297641 ms_python_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 ms_python_client-0.2.1/PKG-INFO
```

### Comparing `ms_python_client-0.2.0/LICENSE` & `ms_python_client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/README.md` & `ms_python_client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/ms_python_client/api_client.py` & `ms_python_client-0.2.1/ms_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/ms_python_client/cern_ms_api_client.py` & `ms_python_client-0.2.1/ms_python_client/cern_ms_api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Optional
 
-from ms_python_client.api_client import ApiClient
 from ms_python_client.components.events.cern_events_component import (
     CERNEventsComponents,
 )
 from ms_python_client.ms_api_client import MSApiClient
 from ms_python_client.utils import init_from_env
 
 
@@ -14,15 +13,14 @@
         account_id: str,
         client_id: str,
         client_secret: str,
         api_endpoint: str = "https://graph.microsoft.com/v1.0",
         use_path: Optional[str] = None,
     ):
         super().__init__(account_id, client_id, client_secret, api_endpoint, use_path)
-        self.api_client = ApiClient(api_base_url=api_endpoint)
         self.init_components()
 
     def init_components(self):
         # Add all the new components here
         self.events = CERNEventsComponents(self)
 
     @staticmethod
```

### Comparing `ms_python_client-0.2.0/ms_python_client/components/events/cern_events_component.py` & `ms_python_client-0.2.1/ms_python_client/components/events/cern_events_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/ms_python_client/components/events/events_component.py` & `ms_python_client-0.2.1/ms_python_client/components/events/events_component.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/ms_python_client/ms_api_client.py` & `ms_python_client-0.2.1/ms_python_client/ms_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Mapping, Optional
 
 import requests
 from msal import ConfidentialClientApplication, SerializableTokenCache
 
 from ms_python_client.api_client import ApiClient
 from ms_python_client.components.events.events_component import EventsComponent
+from ms_python_client.components.events.users_component import UsersComponent
 from ms_python_client.ms_client_interface import MSClientInterface
 from ms_python_client.utils import init_from_env
 
 logging.getLogger("ms_python_client").addHandler(logging.NullHandler())
 logger = logging.getLogger("ms_python_client")
 
 TypeData = Mapping[str, Any]
@@ -54,14 +55,15 @@
     def _write_cache(self, cache_path: str, cache: SerializableTokenCache) -> None:
         with open(cache_path, "w", encoding="utf-8") as f:
             f.write(cache.serialize())
 
     def init_components(self):
         # Add all the new components here
         self.events = EventsComponent(self)
+        self.users = UsersComponent(self)
 
     def __init__(
         self,
         account_id: str,
         client_id: str,
         client_secret: str,
         api_endpoint: str = "https://graph.microsoft.com/v1.0",
@@ -133,15 +135,15 @@
             api_path=api_path, headers=headers, data=json.dumps(data)
         )
 
         return response
 
     def make_patch_request(self, api_path: str, data: TypeData) -> requests.Response:
         headers = self.build_headers()
-        print(json.dumps(data))
+
         response = self.api_client.make_patch_request(
             api_path=api_path, headers=headers, data=json.dumps(data)
         )
 
         return response
 
     def make_delete_request(self, api_path: str) -> requests.Response:
```

### Comparing `ms_python_client-0.2.0/ms_python_client/ms_client_interface.py` & `ms_python_client-0.2.1/ms_python_client/ms_client_interface.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/ms_python_client/utils/event_generator.py` & `ms_python_client-0.2.1/ms_python_client/utils/event_generator.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/ms_python_client/utils/init_from_env.py` & `ms_python_client-0.2.1/ms_python_client/utils/init_from_env.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/ms_python_client/utils/logger.py` & `ms_python_client-0.2.1/ms_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_python_client-0.2.0/pyproject.toml` & `ms_python_client-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "ms-python-client"
-version = "0.2.0"
+version = "0.2.1"
 exclude = ["tests*", "example*", ".github*", ".git*", ".vscode*"]
 description = "This package is used to interact with the microsoft graph API"
 authors = ["Samuel Guillemet <samuel.guillemet@telecom-sudparis.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ms_python_client"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 python-dotenv = "^0.21.0"
 typing_extensions = "^4.3.0"
 msal = "^1.22.0"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 black = "23.3.0"
```

### Comparing `ms_python_client-0.2.0/PKG-INFO` & `ms_python_client-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ms-python-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: This package is used to interact with the microsoft graph API
 License: MIT
 Author: Samuel Guillemet
 Author-email: samuel.guillemet@telecom-sudparis.eu
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msal (>=1.22.0,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/SamuelGuillemet/ms-python-client/issues
```

