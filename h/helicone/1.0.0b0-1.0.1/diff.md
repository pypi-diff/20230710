# Comparing `tmp/helicone-1.0.0b0.tar.gz` & `tmp/helicone-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicone-1.0.0b0.tar", max compression
+gzip compressed data, was "helicone-1.0.1.tar", max compression
```

## Comparing `helicone-1.0.0b0.tar` & `helicone-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.0b0/LICENSE
--rw-r--r--   0        0        0        1 2023-07-06 18:54:19.040110 helicone-1.0.0b0/helicone/async_logger/__init__.py
--rw-r--r--   0        0        0     2993 2023-07-06 18:54:19.040496 helicone-1.0.0b0/helicone/async_logger/async_logger.py
--rw-r--r--   0        0        0       52 2023-07-06 18:54:19.040834 helicone-1.0.0b0/helicone/globals/__init__.py
--rw-r--r--   0        0        0      883 2023-07-06 22:10:20.407271 helicone-1.0.0b0/helicone/globals/helicone.py
--rw-r--r--   0        0        0       36 2023-07-06 18:54:19.041222 helicone-1.0.0b0/helicone/openai/__init__.py
--rw-r--r--   0        0        0     8256 2023-07-06 22:10:01.218294 helicone-1.0.0b0/helicone/openai/openai_injector.py
--rw-r--r--   0        0        0    10392 2023-07-06 18:54:19.042076 helicone-1.0.0b0/helicone/openai_proxy/__init__.py
--rw-r--r--   0        0        0       20 2023-07-03 21:17:48.000891 helicone-1.0.0b0/helicone/requirements.txt
--rw-r--r--   0        0        0    11232 2023-07-03 21:17:48.000970 helicone-1.0.0b0/helicone/test.py
--rw-r--r--   0        0        0      381 2023-07-07 05:21:31.861028 helicone-1.0.0b0/pyproject.toml
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 helicone-1.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.1/LICENSE
+-rw-r--r--   0        0        0        1 2023-07-10 04:44:07.860264 helicone-1.0.1/helicone/async_logger/__init__.py
+-rw-r--r--   0        0        0     3165 2023-07-10 04:44:07.860522 helicone-1.0.1/helicone/async_logger/async_logger.py
+-rw-r--r--   0        0        0       52 2023-07-10 04:44:07.860863 helicone-1.0.1/helicone/globals/__init__.py
+-rw-r--r--   0        0        0     1350 2023-07-10 04:44:07.861152 helicone-1.0.1/helicone/globals/helicone.py
+-rw-r--r--   0        0        0      102 2023-07-10 04:44:07.861504 helicone-1.0.1/helicone/openai_async/__init__.py
+-rw-r--r--   0        0        0     8835 2023-07-10 04:44:07.861726 helicone-1.0.1/helicone/openai_async/openai_injector.py
+-rw-r--r--   0        0        0     9942 2023-07-10 04:44:07.861894 helicone-1.0.1/helicone/openai_proxy/__init__.py
+-rw-r--r--   0        0        0       20 2023-07-03 21:17:48.000891 helicone-1.0.1/helicone/requirements.txt
+-rw-r--r--   0        0        0    11545 2023-07-10 04:44:07.862095 helicone-1.0.1/helicone/test.py
+-rw-r--r--   0        0        0      380 2023-07-10 04:44:07.862921 helicone-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-1.0.1/PKG-INFO
```

### Comparing `helicone-1.0.0b0/LICENSE` & `helicone-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helicone-1.0.0b0/helicone/async_logger/async_logger.py` & `helicone-1.0.1/helicone/async_logger/async_logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,14 +53,20 @@
 @dataclass
 class HeliconeAyncLogRequest:
     providerRequest: ProviderRequest
     providerResponse: ProviderResponse
     timing: Timing
 
 
+@dataclass
+class HeliconeMeta:
+    custom_properties: Optional[dict]
+    user_id: Optional[str]
+
+
 class Provider(Enum):
     OPENAI = "openai"
     AZURE_OPENAI = "azure-openai"
     ANTHROPIC = "anthropic"
 
 
 class HeliconeAsyncLogger:
@@ -89,15 +95,18 @@
             }
         )
         if (res.status_code != 200):
             raise ValueError(
                 f"Failed to log to {url}. Status code {res.status_code}")
         return res
 
-    def log(self, request: HeliconeAyncLogRequest, provider: Provider):
+    def log(self, request: HeliconeAyncLogRequest,
+            provider: Provider,
+            meta: Optional[HeliconeMeta] = None
+            ):
         print("logging", request, provider)
         if provider == Provider.OPENAI:
             self._request(
                 body=dataclasses.asdict(request),
                 url=f"{self.base_url}/oai/v1/log"
             )
         elif provider == Provider.AZURE_OPENAI:
```

### Comparing `helicone-1.0.0b0/helicone/globals/helicone.py` & `helicone-1.0.1/helicone/globals/helicone.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,36 +7,51 @@
 
 logger = logging.getLogger(__name__)
 
 
 class HeliconeGlobal:
     _api_key: Optional[str]
     _base_url: Optional[str]
+    _proxy_url: Optional[str]
 
     def __init__(self,
                  api_key: Optional[str] = None,
-                 base_url: Optional[str] = None
+                 base_url: Optional[str] = None,
+                 proxy_url: Optional[str] = None
                  ):
         self._api_key = api_key
         self._base_url = base_url
+        self._proxy_url = proxy_url
 
     @property
     def api_key(self) -> Optional[str]:
         if (self._api_key is None):
-            self._api_key = os.environ.get("HELICONE_API_KEY")
+            return os.environ.get("HELICONE_API_KEY")
 
         return self._api_key
 
     @api_key.setter
     def api_key(self, value: Optional[str]):
         self._api_key = value
 
     @property
     def base_url(self) -> Optional[str]:
+        if (self._base_url is None):
+            return "https://api.hconeai.com/v1"
         return self._base_url
 
     @base_url.setter
     def base_url(self, value: Optional[str]):
         self._base_url = value
 
+    @property
+    def proxy_url(self) -> Optional[str]:
+        if (self._proxy_url is None):
+            return "http://oai.hconeai.com/v1"
+        return self._proxy_url
+
+    @proxy_url.setter
+    def proxy_url(self, value: Optional[str]):
+        self._proxy_url = value
+
 
 helicone_global = HeliconeGlobal()
```

### Comparing `helicone-1.0.0b0/helicone/openai/openai_injector.py` & `helicone-1.0.1/helicone/openai_async/openai_injector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,42 @@
+from dataclasses import dataclass
 import datetime
 import functools
 import inspect
 import json
-import logging
-import os
-import threading
-import uuid
-import warnings
-from typing import Callable, Mapping
-
-import aiohttp
-import openai
-import requests
+from typing import Callable, Optional
+import openai  # noqa
 from openai.api_resources import (ChatCompletion, Completion, Edit, Embedding,
                                   Image, Moderation)
 
 from helicone.async_logger.async_logger import (HeliconeAsyncLogger,
                                                 HeliconeAyncLogRequest,
                                                 Provider, ProviderRequest,
-                                                ProviderResponse, Timing,
-                                                UnixTimeStamp)
-from helicone.globals import helicone_global
+                                                ProviderResponse, Timing)
 
-helicone_global.base_url = "https://oai.hconeai.com/v1"
+
+@dataclass
+class HeliconeMeta:
+    custom_properties: Optional[dict] = None
+    user_id: Optional[str] = None
+
+    def build(self) -> dict:
+        meta = {}
+        if self.custom_properties:
+            for key, value in self.custom_properties.items():
+                meta[f"Helicone-Property-{key}"] = value
+
+        if self.user_id:
+            meta["Helicone-User-Id"] = self.user_id
+        print("METAAAAA", meta)
+        return meta
 
 
 class CreateArgsExtractor:
+    _helicone_meta: Optional[HeliconeMeta]
 
     def __init__(self,
                  api_key=None,
                  api_base=None,
                  api_type=None,
                  request_id=None,
                  api_version=None,
@@ -38,21 +45,28 @@
         self.kwargs = kwargs
         self.kwargs["api_key"] = api_key
         self.kwargs["api_base"] = api_base
         self.kwargs["api_type"] = api_type
         self.kwargs["request_id"] = request_id
         self.kwargs["api_version"] = api_version
         self.kwargs["organization"] = organization
+        self._helicone_meta = kwargs.get("helicone_meta")
+        self.kwargs.pop("helicone_meta", None)
 
     def get_args(self):
         return self.kwargs
 
     def get_body(self):
         return self.kwargs
 
+    def get_helicone_meta(self) -> dict:
+        if (self._helicone_meta is None):
+            return {}
+        return self._helicone_meta.build()
+
 
 class OpenAIInjector:
     def __init__(self):
         pass
 
     def update_response_headers(self, result, helicone_request_id):
         result["helicone_request_id"] = helicone_request_id
@@ -108,15 +122,15 @@
 
             arg_extractor = CreateArgsExtractor(*args, **kwargs)
             now = datetime.datetime.now()
 
             providerRequest = ProviderRequest(
                 url="N/A",
                 json=arg_extractor.get_body(),
-                meta={}
+                meta=arg_extractor.get_helicone_meta()
             )
             try:
                 result = func(**arg_extractor.get_args())
             except Exception as e:
                 later = datetime.datetime.now()
                 async_log = HeliconeAyncLogRequest(
                     providerRequest=providerRequest,
@@ -166,15 +180,15 @@
 
             arg_extractor = CreateArgsExtractor(*args, **kwargs)
             now = datetime.datetime.now()
 
             providerRequest = ProviderRequest(
                 url="N/A",
                 json=arg_extractor.get_body(),
-                meta={}
+                meta=arg_extractor.get_helicone_meta()
             )
             try:
                 result = await func(**arg_extractor.get_args())
             except Exception as e:
                 later = datetime.datetime.now()
                 async_log = HeliconeAyncLogRequest(
                     providerRequest=providerRequest,
```

### Comparing `helicone-1.0.0b0/helicone/openai_proxy/__init__.py` & `helicone-1.0.1/helicone/openai_proxy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 import functools
 import uuid
 import inspect
-import os
+from helicone.globals import helicone_global
 import openai
 import requests
-import warnings
 from openai.api_resources import (
     ChatCompletion,
     Completion,
     Edit,
     Embedding,
     Image,
     Moderation,
 )
 import logging
 import threading
 
 logger = logging.getLogger(__name__)
 
-api_key = os.environ.get("HELICONE_API_KEY", None)
-if (api_key is None):
-    warnings.warn("Helicone API key is not set as an environment variable.")
-
-proxy_url = os.environ.get("HELICONE_PROXY_URL", "https://oai.hconeai.com/v1")
-
 global_headers = {}
 
 
 class AttributeDict(dict):
     def __init__(self, *args, **kwargs):
         super(AttributeDict, self).__init__(*args, **kwargs)
         self.__dict__ = self
@@ -50,87 +43,67 @@
             "Invalid data_type provided. Please use a valid data type or string.")
 
 
 def prepare_api_base(**kwargs):
     original_api_base = openai.api_base
     kwargs["headers"].update({"Helicone-OpenAI-Api-Base": original_api_base})
 
-    openai.api_base = proxy_url
+    openai.api_base = helicone_global.proxy_url
 
     if openai.api_type == "azure":
-        if proxy_url.endswith('/v1'):
-            if proxy_url != "https://oai.hconeai.com/v1":
+        if helicone_global.proxy_url.endswith('/v1'):
+            if helicone_global.proxy_url != "https://oai.hconeai.com/v1":
                 logging.warning(
-                    f"Detected likely invalid Azure API URL when proxying Helicone with proxy url {proxy_url}. Removing '/v1' from the end.")
-            openai.api_base = proxy_url[:-3]
+                    f"Detected likely invalid Azure API URL when proxying Helicone with proxy url {helicone_global.proxy_url}. Removing '/v1' from the end.")
+            openai.api_base = helicone_global.proxy_url[:-3]
 
     return original_api_base, kwargs
 
 
 class Helicone:
     def __init__(self):
         self.openai = openai
         self.apply_helicone_auth()
         self.headers_store = {}
 
-    @property
-    def api_key(self):
-        global api_key
-        return api_key
-
-    @api_key.setter
-    def api_key(self, value):
-        global api_key
-        api_key = value
-
-    @property
-    def proxy_url(self):
-        global proxy_url
-        return proxy_url
-
-    @proxy_url.setter
-    def proxy_url(self, value):
-        global proxy_url
-        proxy_url = value
-
     def log_feedback(self, response, name, value, data_type=None):
         helicone_id = response.get("helicone", {}).get("id")
         if not helicone_id:
             raise ValueError(
                 "The provided response does not have a valid Helicone ID.")
 
         feedback_data = {
             "helicone-id": helicone_id,
             "name": name,
             "value": value,
         }
         if data_type:
             feedback_data["data-type"] = normalize_data_type(data_type)
 
-        url = f"{proxy_url}/feedback"
+        url = f"{helicone_global.proxy_url}/feedback"
 
         headers = {
             "Content-Type": "application/json",
-            "Helicone-Auth": f"Bearer {api_key}",
+            "Helicone-Auth": f"Bearer {helicone_global.api_key}",
         }
 
         response = requests.post(url, headers=headers, json=feedback_data)
         if response.status_code != 200:
             logger.error(f"HTTP error occurred: {response.status_code}")
             logger.error(
                 f"Response content: {response.content.decode('utf-8', 'ignore')}")
 
             response.raise_for_status()
         return response.json()
 
     def _prepare_headers(self, **kwargs):
         headers = kwargs.get("headers", {})
 
-        if "Helicone-Auth" not in headers and api_key:
-            headers["Helicone-Auth"] = f"Bearer {api_key}"
+        if "Helicone-Auth" not in headers and helicone_global.api_key:
+            headers["Helicone-Auth"] = f"Bearer {helicone_global.api_key}"
 
         # Generate a UUID and add it to the headers
         helicone_request_id = str(uuid.uuid4())
         headers["helicone-request-id"] = helicone_request_id
 
         headers.update(self._get_property_headers(
             kwargs.pop("properties", {})))
@@ -287,9 +260,9 @@
                     self_parent._with_helicone_auth(create_method))
 
             async_create_method = getattr(api_resource_class, async_method)
             setattr(api_resource_class, async_method,
                     self_parent._with_helicone_auth_async(async_create_method))
 
 
-# helicone = Helicone()
-# log_feedback = helicone.log_feedback
+helicone = Helicone()
+log_feedback = helicone.log_feedback
```

### Comparing `helicone-1.0.0b0/helicone/test.py` & `helicone-1.0.1/helicone/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 from dotenv import load_dotenv
-import helicone
-from helicone import openai, log_feedback
+from helicone.openai_proxy import openai, log_feedback
+from helicone.globals import helicone_global
 import uuid
 from supabase import create_client
 import hashlib
 import pytest
 
-helicone.proxy_url = "http://127.0.0.1:8787/v1"
-helicone.api_key = os.getenv("HELICONE_API_KEY_LOCAL")
+helicone_global.proxy_url = "http://127.0.0.1:8787/v1"
+helicone_global.api_key = os.getenv("HELICONE_API_KEY_LOCAL")
 
 SUPABASE_SERVICE_ROLE_KEY = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZS1kZW1vIiwicm9sZSI6InNlcnZpY2Vfcm9sZSIsImV4cCI6MTk4MzgxMjk5Nn0.EGIM96RAZx35lJzdJsyH-qQwv8Hdp7fsn3W0YpN81IU"
 SUPABASE_URL = "http://localhost:54321"
 
 sb = create_client(SUPABASE_URL, SUPABASE_SERVICE_ROLE_KEY)
 
 load_dotenv()
 
+
 def test_cache_completion():
     unique_id = str(uuid.uuid4())
     prompt = f"Cache test with UUID: {unique_id}"
 
     response1 = openai.Completion.create(
         model="text-ada-001",
         prompt=prompt,
@@ -41,14 +42,15 @@
     response2_copy = response2.copy()
 
     del response1_copy['helicone']['cache']
     del response2_copy['helicone']['cache']
 
     assert response1_copy == response2_copy
 
+
 def test_cache_embedding():
     unique_id = str(uuid.uuid4())
     prompt = f"Cache test with UUID: {unique_id}"
 
     response1 = openai.Embedding.create(
         model="text-embedding-ada-002",
         input=prompt,
@@ -77,24 +79,25 @@
     rate_limit_policy_str = "10;w=60"
 
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[{"role": "user", "content": "Rate limit policy test"}],
         rate_limit_policy=rate_limit_policy_dict
     )
-    assert response.helicone.rate_limit.policy.startswith(rate_limit_policy_str)
+    assert response.helicone.rate_limit.policy.startswith(
+        rate_limit_policy_str)
 
     openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[{"role": "user", "content": "Rate limit policy test"}],
         rate_limit_policy=rate_limit_policy_str
     )
     # Assert the prefix of the policy is equal to the str
-    assert response.helicone.rate_limit.policy.startswith(rate_limit_policy_str)
-
+    assert response.helicone.rate_limit.policy.startswith(
+        rate_limit_policy_str)
 
 
 def test_custom_properties():
     properties = {
         "Session": "24",
         "Conversation": "support_issue_2",
         "App": "mobile",
@@ -165,17 +168,16 @@
         feedback = feedback_result.data
 
         feedback_data.extend(feedback)
 
     return feedback_data
 
 
+@pytest.mark.skip(reason="Skipping until feedback is reimplemented")
 def test_log_feedback():
-    helicone.proxy_url = "http://127.0.0.1:8787/v1"
-    helicone.api_key = os.getenv("HELICONE_API_KEY_LOCAL")
     prompt = "Integration test for logging feedback"
 
     response = openai.Completion.create(
         model="text-ada-001",
         prompt=prompt,
         max_tokens=10,
     )
@@ -188,14 +190,15 @@
     assert len(feedback_data) == 1
     assert feedback_data[0]["boolean_value"] is True
     assert feedback_data[0]["float_value"] is None
     assert feedback_data[0]["string_value"] is None
     assert feedback_data[0]["categorical_value"] is None
 
 
+@pytest.mark.skip(reason="Skipping until feedback is reimplemented")
 def test_sync_nostream():
     response = openai.ChatCompletion.create(
         model='gpt-3.5-turbo',
         messages=[{
             'role': 'user',
             'content': "Hello World!"
         }],
@@ -211,14 +214,15 @@
     assert len(feedback_data) == 1
     assert feedback_data[0]["boolean_value"] is None
     assert feedback_data[0]["float_value"] is None
     assert feedback_data[0]["string_value"] == "create_and_stream_false"
     assert feedback_data[0]["categorical_value"] is None
 
 
+@pytest.mark.skip(reason="Skipping until feedback is reimplemented")
 def test_sync_stream():
     from collections import deque
 
     iterator = openai.ChatCompletion.create(
         model='gpt-3.5-turbo',
         messages=[{
             'role': 'user',
@@ -237,14 +241,15 @@
     assert len(feedback_data) == 1
     assert feedback_data[0]["boolean_value"] is None
     assert feedback_data[0]["float_value"] is None
     assert feedback_data[0]["string_value"] == "create_and_stream_true"
     assert feedback_data[0]["categorical_value"] is None
 
 
+@pytest.mark.skip(reason="Skipping until feedback is reimplemented")
 @pytest.mark.asyncio
 async def test_async_nostream():
     response = (await openai.ChatCompletion.acreate(
         model='gpt-3.5-turbo',
         messages=[{
             'role': 'user',
             'content': "Hello World!"
@@ -261,14 +266,15 @@
     assert len(feedback_data) == 1
     assert feedback_data[0]["boolean_value"] is None
     assert feedback_data[0]["float_value"] is None
     assert feedback_data[0]["string_value"] == "acreate_and_stream_false"
     assert feedback_data[0]["categorical_value"] is None
 
 
+@pytest.mark.skip(reason="Skipping until feedback is reimplemented")
 @pytest.mark.asyncio
 async def test_async_stream():
     async for chunk in await openai.ChatCompletion.acreate(
         model='gpt-3.5-turbo',
         messages=[{
             'role': 'user',
             'content': "Hello World!"
@@ -285,14 +291,15 @@
 
     assert len(feedback_data) == 1
     assert feedback_data[0]["boolean_value"] is None
     assert feedback_data[0]["float_value"] is None
     assert feedback_data[0]["string_value"] == "acreate_and_stream_true"
     assert feedback_data[0]["categorical_value"] is None
 
+
 def test_sync_nostream_cache():
     unique_id = str(uuid.uuid4())
     message = f"Sync NoStream Cache test with UUID: {unique_id}"
 
     response1 = openai.ChatCompletion.create(
         model='gpt-3.5-turbo',
         messages=[{
@@ -319,14 +326,15 @@
     response2_copy = response2.copy()
 
     del response1_copy['helicone']['cache']
     del response2_copy['helicone']['cache']
 
     assert response1_copy == response2_copy
 
+
 @pytest.mark.asyncio
 async def test_async_nostream_cache():
     unique_id = str(uuid.uuid4())
     message = f"Async NoStream Cache test with UUID: {unique_id}"
 
     response1 = (await openai.ChatCompletion.acreate(
         model='gpt-3.5-turbo',
@@ -354,24 +362,25 @@
     response2_copy = response2.copy()
 
     del response1_copy['helicone']['cache']
     del response2_copy['helicone']['cache']
 
     assert response1_copy == response2_copy
 
+
 def test_azure():
     openai.api_type = "azure"
     openai.api_base = f"https://{os.environ['AZURE_OPENAI_ENDPOINT']}"
     openai.api_version = "2023-03-15-preview"
     openai.api_key = os.environ["AZURE_OPENAI_API_KEY"]
 
     openai.ChatCompletion.create(
         engine="gpt-4",
         messages=[
             {
                 "role": "user",
-                "content":"Say hi!",
+                "content": "Say hi!",
             },
         ],
         temperature=1,
         max_tokens=10,
     )
```

### Comparing `helicone-1.0.0b0/PKG-INFO` & `helicone-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helicone
-Version: 1.0.0b0
+Version: 1.0.1
 Summary: A Python wrapper for the OpenAI API that logs all requests to Helicone.
 Home-page: https://www.helicone.ai
 License: Apache-2.0
 Author: Helicone, Inc.
 Author-email: help@helicone.ai
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: Apache Software License
```

