# Comparing `tmp/gradio_client-0.2.7.tar.gz` & `tmp/gradio_client-0.2.8.tar.gz`

## Comparing `gradio_client-0.2.7.tar` & `gradio_client-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.7/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.7/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/__init__.py
--rw-r--r--   0        0        0    48042 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/client.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/media_data.py
--rw-r--r--   0        0        0    19138 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/types.json
--rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.7/gradio_client/version.txt
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 gradio_client-0.2.7/.gitignore
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 gradio_client-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 gradio_client-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.8/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.8/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/__init__.py
+-rw-r--r--   0        0        0    48736 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/client.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19131 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/types.json
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.8/gradio_client/version.txt
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 gradio_client-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 gradio_client-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 gradio_client-0.2.8/PKG-INFO
```

### Comparing `gradio_client-0.2.7/README.md` & `gradio_client-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.7/gradio_client/client.py` & `gradio_client-0.2.8/gradio_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pathlib import Path
 from threading import Lock
 from typing import Any, Callable, Literal
 
 import huggingface_hub
 import requests
 import websockets
-from huggingface_hub import SpaceStage
+from huggingface_hub import SpaceHardware, SpaceStage
 from huggingface_hub.utils import (
     RepositoryNotFoundError,
     build_hf_headers,
     send_telemetry,
 )
 from packaging import version
 
@@ -141,15 +141,25 @@
     @classmethod
     def duplicate(
         cls,
         from_id: str,
         to_id: str | None = None,
         hf_token: str | None = None,
         private: bool = True,
-        hardware: str | None = None,
+        hardware: Literal[
+            "cpu-basic",
+            "cpu-upgrade",
+            "t4-small",
+            "t4-medium",
+            "a10g-small",
+            "a10g-large",
+            "a100-large",
+        ]
+        | SpaceHardware
+        | None = None,
         secrets: dict[str, str] | None = None,
         sleep_timeout: int = 5,
         max_workers: int = 40,
         verbose: bool = True,
     ):
         """
         Duplicates a Hugging Face Space under your account and returns a Client object
@@ -216,29 +226,32 @@
                 private=private,
             )
             if secrets is not None:
                 for key, value in secrets.items():
                     huggingface_hub.add_space_secret(
                         space_id, key, value, token=hf_token
                     )
-            utils.set_space_timeout(
-                space_id, hf_token=hf_token, timeout_in_seconds=sleep_timeout * 60
-            )
             if verbose:
                 print(f"Created new Space: {utils.SPACE_URL.format(space_id)}")
         current_info = huggingface_hub.get_space_runtime(space_id, token=hf_token)
         current_hardware = (
             current_info.hardware or huggingface_hub.SpaceHardware.CPU_BASIC
         )
         hardware = hardware or original_info.hardware
         if current_hardware != hardware:
             huggingface_hub.request_space_hardware(space_id, hardware)  # type: ignore
             print(
                 f"-------\nNOTE: this Space uses upgraded hardware: {hardware}... see billing info at https://huggingface.co/settings/billing\n-------"
             )
+        # Setting a timeout only works if the hardware is not basic
+        # so set it here after the hardware has been requested
+        if hardware != huggingface_hub.SpaceHardware.CPU_BASIC:
+            utils.set_space_timeout(
+                space_id, hf_token=hf_token, timeout_in_seconds=sleep_timeout * 60
+            )
         if verbose:
             print("")
         client = cls(
             space_id, hf_token=hf_token, max_workers=max_workers, verbose=verbose
         )
         return client
 
@@ -338,15 +351,15 @@
         print_info: bool = True,
         return_format: Literal["dict", "str"] | None = None,
     ) -> dict | str | None:
         """
         Prints the usage info for the API. If the Gradio app has multiple API endpoints, the usage info for each endpoint will be printed separately. If return_format="dict" the info is returned in dictionary format, as shown in the example below.
 
         Parameters:
-            all_endpoints: If True, prints information for both named and unnamed endpoints in the Gradio app. If False, will only print info about named endpoints. If None (default), will only print info about unnamed endpoints if there are no named endpoints.
+            all_endpoints: If True, prints information for both named and unnamed endpoints in the Gradio app. If False, will only print info about named endpoints. If None (default), will print info about named endpoints, unless there aren't any -- in which it will print info about unnamed endpoints.
             print_info: If True, prints the usage info to the console. If False, does not print the usage info.
             return_format: If None, nothing is returned. If "str", returns the same string that would be printed to the console. If "dict", returns the usage info as a dictionary that can be programmatically parsed, and *all endpoints are returned in the dictionary* regardless of the value of `all_endpoints`. The format of the dictionary is in the docstring of this method.
         Example:
             from gradio_client import Client
             client = Client(src="gradio/calculator")
             client.view_api(return_format="dict")
             >> {
@@ -595,24 +608,26 @@
     """Helper class for storing all the information about a single API endpoint."""
 
     def __init__(self, client: Client, fn_index: int, dependency: dict):
         self.client: Client = client
         self.fn_index = fn_index
         self.dependency = dependency
         api_name = dependency.get("api_name")
-        self.api_name: str | None = None if api_name is None else "/" + api_name
+        self.api_name: str | None = (
+            None if (api_name is None or api_name is False) else "/" + api_name
+        )
         self.use_ws = self._use_websocket(self.dependency)
         self.input_component_types = []
         self.output_component_types = []
         self.root_url = client.src + "/" if not client.src.endswith("/") else client.src
         try:
+            # Only a real API endpoint if backend_fn is True (so not just a frontend function), serializers are valid,
+            # and api_name is not False (meaning that the developer has explicitly disabled the API endpoint)
             self.serializers, self.deserializers = self._setup_serializers()
-            self.is_valid = self.dependency[
-                "backend_fn"
-            ]  # Only a real API endpoint if backend_fn is True and serializers are valid
+            self.is_valid = self.dependency["backend_fn"] and self.api_name is not False
         except AssertionError:
             self.is_valid = False
 
     def __repr__(self):
         return f"Endpoint src: {self.client.src}, api_name: {self.api_name}, fn_index: {self.fn_index}"
 
     def __str__(self):
@@ -933,15 +948,15 @@
                 if len(self.communicator.job.outputs) == self._counter + 1:
                     o = self.communicator.job.outputs[self._counter]
                     self._counter += 1
                     return o
                 if self.communicator.job.latest_status.code == Status.FINISHED:
                     raise StopIteration()
 
-    def result(self, timeout=None) -> Any:
+    def result(self, timeout: float | None = None) -> Any:
         """
         Return the result of the call that the future represents. Raises CancelledError: If the future was cancelled, TimeoutError: If the future didn't finish executing before the given timeout, and Exception: If the call raised then that exception will be raised.
 
         Parameters:
             timeout: The number of seconds to wait for the result if the future isn't done. If None, then there is no limit on the wait time.
         Returns:
             The result of the call that the future represents.
```

### Comparing `gradio_client-0.2.7/gradio_client/documentation.py` & `gradio_client-0.2.8/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.7/gradio_client/media_data.py` & `gradio_client-0.2.8/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.7/gradio_client/serializing.py` & `gradio_client-0.2.8/gradio_client/serializing.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,19 +167,19 @@
         """
         Convert from human-friendly version of a file (string filepath) to a serialized
         representation (base64).
         Parameters:
             x: String path to file to serialize
             load_dir: Path to directory containing x
         """
-        if x is None or x == "":
+        if not x:
             return None
-        is_url = utils.is_valid_url(x)
-        path = x if is_url else Path(load_dir) / x
-        return utils.encode_url_or_file_to_base64(path)
+        if utils.is_http_url_like(x):
+            return utils.encode_url_to_base64(x)
+        return utils.encode_file_to_base64(Path(load_dir) / x)
 
     def deserialize(
         self,
         x: str | None,
         save_dir: str | Path | None = None,
         root_url: str | None = None,
         hf_token: str | None = None,
@@ -248,15 +248,15 @@
         }
 
     def _serialize_single(
         self, x: str | FileData | None, load_dir: str | Path = ""
     ) -> FileData | None:
         if x is None or isinstance(x, dict):
             return x
-        if utils.is_valid_url(x):
+        if utils.is_http_url_like(x):
             filename = x
             size = None
         else:
             filename = str(Path(load_dir) / x)
             size = Path(filename).stat().st_size
         return {
             "name": filename,
```

### Comparing `gradio_client-0.2.7/gradio_client/types.json` & `gradio_client-0.2.8/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.7/gradio_client/utils.py` & `gradio_client-0.2.8/gradio_client/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import mimetypes
 import os
 import pkgutil
 import secrets
 import shutil
 import tempfile
+import warnings
 from concurrent.futures import CancelledError
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
 from threading import Lock
 from typing import Any, Callable, Optional
@@ -189,25 +190,47 @@
 
 
 ########################
 # Network utils
 ########################
 
 
-def is_valid_url(possible_url: str) -> bool:
+def is_http_url_like(possible_url: str) -> bool:
+    """
+    Check if the given string looks like an HTTP(S) URL.
+    """
+    return possible_url.startswith(("http://", "https://"))
+
+
+def probe_url(possible_url: str) -> bool:
+    """
+    Probe the given URL to see if it responds with a 200 status code (to HEAD, then to GET).
+    """
     headers = {"User-Agent": "gradio (https://gradio.app/; team@gradio.app)"}
     try:
-        head_request = requests.head(possible_url, headers=headers)
-        if head_request.status_code == 405:
-            return requests.get(possible_url, headers=headers).ok
-        return head_request.ok
+        with requests.session() as sess:
+            head_request = sess.head(possible_url, headers=headers)
+            if head_request.status_code == 405:
+                return sess.get(possible_url, headers=headers).ok
+            return head_request.ok
     except Exception:
         return False
 
 
+def is_valid_url(possible_url: str) -> bool:
+    """
+    Check if the given string is a valid URL.
+    """
+    warnings.warn(
+        "is_valid_url should not be used. "
+        "Use is_http_url_like() and probe_url(), as suitable, instead.",
+    )
+    return is_http_url_like(possible_url) and probe_url(possible_url)
+
+
 async def get_pred_from_ws(
     websocket: WebSocketCommonProtocol,
     data: str,
     hash_data: str,
     helper: Communicator | None = None,
 ) -> dict[str, Any]:
     completed = False
@@ -278,18 +301,18 @@
     if dir is not None:
         os.makedirs(dir, exist_ok=True)
     headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
     directory = Path(dir or tempfile.gettempdir()) / secrets.token_hex(20)
     directory.mkdir(exist_ok=True, parents=True)
     file_path = directory / Path(url_path).name
 
-    with requests.get(url_path, headers=headers, stream=True) as r, open(
-        file_path, "wb"
-    ) as f:
-        shutil.copyfileobj(r.raw, f)
+    with requests.get(url_path, headers=headers, stream=True) as r:
+        r.raise_for_status()
+        with open(file_path, "wb") as f:
+            shutil.copyfileobj(r.raw, f)
     return str(file_path.resolve())
 
 
 def create_tmp_copy_of_file(file_path: str, dir: str | None = None) -> str:
     directory = Path(dir or tempfile.gettempdir()) / secrets.token_hex(20)
     directory.mkdir(exist_ok=True, parents=True)
     dest = directory / Path(file_path).name
@@ -329,28 +352,29 @@
             + (mimetype if mimetype is not None else "")
             + ";base64,"
             + base64_str
         )
 
 
 def encode_url_to_base64(url: str):
-    encoded_string = base64.b64encode(requests.get(url).content)
+    resp = requests.get(url)
+    resp.raise_for_status()
+    encoded_string = base64.b64encode(resp.content)
     base64_str = str(encoded_string, "utf-8")
     mimetype = get_mimetype(url)
     return (
         "data:" + (mimetype if mimetype is not None else "") + ";base64," + base64_str
     )
 
 
 def encode_url_or_file_to_base64(path: str | Path):
     path = str(path)
-    if is_valid_url(path):
+    if is_http_url_like(path):
         return encode_url_to_base64(path)
-    else:
-        return encode_file_to_base64(path)
+    return encode_file_to_base64(path)
 
 
 def decode_base64_to_binary(encoding: str) -> tuple[bytes, str | None]:
     extension = get_extension(encoding)
     data = encoding.rsplit(",", 1)[-1]
     return base64.b64decode(data), extension
 
@@ -440,21 +464,21 @@
     timeout_in_seconds: int = 300,
 ):
     headers = huggingface_hub.utils.build_hf_headers(
         token=hf_token,
         library_name="gradio_client",
         library_version=__version__,
     )
-    r = requests.post(
+    req = requests.post(
         f"https://huggingface.co/api/spaces/{space_id}/sleeptime",
         json={"seconds": timeout_in_seconds},
         headers=headers,
     )
     try:
-        huggingface_hub.utils.hf_raise_for_status(r)
+        huggingface_hub.utils.hf_raise_for_status(req)
     except huggingface_hub.utils.HfHubHTTPError as err:
         raise SpaceDuplicationError(
             f"Could not set sleep timeout on duplicated Space. Please visit {SPACE_URL.format(space_id)} "
             "to set a timeout manually to reduce billing charges."
         ) from err
```

### Comparing `gradio_client-0.2.7/pyproject.toml` & `gradio_client-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.7/PKG-INFO` & `gradio_client-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

