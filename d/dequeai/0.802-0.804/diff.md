# Comparing `tmp/dequeai-0.802.tar.gz` & `tmp/dequeai-0.804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.802.tar", last modified: Sat Jul  8 00:17:28 2023, max compression
+gzip compressed data, was "dequeai-0.804.tar", last modified: Mon Jul 10 19:19:58 2023, max compression
```

## Comparing `dequeai-0.802.tar` & `dequeai-0.804.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 00:17:28.146827 dequeai-0.802/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 00:17:28.142827 dequeai-0.802/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 00:17:28.142827 dequeai-0.802/dequeai/
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-05 17:59:58.000000 dequeai-0.802/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.802/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.802/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.802/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-07-05 18:59:08.000000 dequeai-0.802/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    12748 2023-07-08 00:09:40.000000 dequeai-0.802/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32571 2023-06-23 20:59:39.000000 dequeai-0.802/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.802/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.802/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.802/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.802/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 00:17:28.142827 dequeai-0.802/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-08 00:17:27.000000 dequeai-0.802/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-08 00:17:28.000000 dequeai-0.802/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 00:17:27.000000 dequeai-0.802/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-08 00:17:27.000000 dequeai-0.802/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-08 00:17:28.000000 dequeai-0.802/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 00:17:28.146827 dequeai-0.802/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      557 2023-07-08 00:17:14.000000 dequeai-0.802/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:19:58.269517 dequeai-0.804/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-10 19:19:58.269517 dequeai-0.804/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:19:58.269517 dequeai-0.804/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-05 17:59:58.000000 dequeai-0.804/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.804/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.804/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.804/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.804/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    14971 2023-07-10 17:59:55.000000 dequeai-0.804/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.804/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.804/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.804/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.804/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.804/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:19:58.269517 dequeai-0.804/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-10 19:19:57.000000 dequeai-0.804/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 19:19:58.000000 dequeai-0.804/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:19:57.000000 dequeai-0.804/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 19:19:58.000000 dequeai-0.804/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 19:19:58.000000 dequeai-0.804/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 19:19:58.269517 dequeai-0.804/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-10 19:19:44.000000 dequeai-0.804/setup.py
```

### Comparing `dequeai-0.802/dequeai/datatypes.py` & `dequeai-0.804/dequeai/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -282,35 +282,56 @@
         # "The maximum length of a histogram is %i" % cls.MAX_LENGTH
         # )
         # if len(histogram) + 1 != len(bins):
         # raise ValueError("len(bins) must be len(histogram) + 1")
 
         return cls(np_histogram=np_histogram)
 
-
 class Audio:
-    _type = DEQUE_AUDIO
+    _type = 'DEQUE_AUDIO'
 
     def __init__(self, data, sample_rate=None, caption=None):
-        """Accepts a path to an audio file or a numpy array of audio data."""
-
-        self._duration = None
+        """Accepts a numpy array of audio data."""
         self._sample_rate = sample_rate
         self._caption = caption
 
-        if sample_rate is None:
-            raise ValueError(
-                'Argument "sample_rate" is required when instantiating deque.Audio with raw data.'
-            )
-
-        self._validate_size()
-        self._data = data
+        if isinstance(data, np.ndarray):
+            self._data = data
+            if sample_rate is None:
+                raise ValueError(
+                    'Argument "sample_rate" is required when instantiating Audio with raw data.'
+                )
+            self._validate_size()
+        else:
+            raise ValueError('Invalid type for data. Numpy array expected.')
 
     def _validate_size(self):
-        pass
+        # Assuming mono audio, you could extend this to handle multi-channel audio.
+        if self._data.ndim > 1:
+            raise ValueError('Invalid data size. Only mono audio data is supported.')
+
+        if self._data.size == 0:
+            raise ValueError('Audio data is empty.')
+
+        # Add any other validation here
+
+    @property
+    def duration(self):
+        if self._duration is None:
+            self._duration = self._data.size / self._sample_rate
+        return self._duration
+
+    @property
+    def sample_rate(self):
+        return self._sample_rate
+
+    @property
+    def caption(self):
+        return self._caption
+
 
 
 class Video:
     _type = DEQUE_VIDEO
 
 
 class Text:
```

### Comparing `dequeai-0.802/dequeai/dequeai_model.py` & `dequeai-0.804/dequeai/dequeai_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,53 +17,91 @@
 import socket
 import types
 from IPython.display import display, HTML
 from tabulate import tabulate
 import numpy as np
 import json
 from typing import Optional
+
 _RESOURCE_MONITORING_INTERVAL = 60
 
+
 class ModelCard:
+
     def __init__(self):
-        self.task_category: Optional[str] = None
-        self.task: Optional[str] = None
-        self.model_name: Optional[str] = None
-        self.model_architecture: Optional[str] = None
-
-        self.model_description: Optional[str] = None
-        self.model_version: Optional[str] = None
-        self.limitations: Optional[str] = None
-        self.intended_users: Optional[str] = None
-        self.training_data_size: Optional[str] = None
-        self.training_data_size_units: Optional[str] = None
-        self.training_data_description: Optional[str] = None
-        self.training_data_source: Optional[str] = None
-        self.training_date: Optional[str] = None
-        self.license: Optional[str] = None
-        self.citation : Optional[str] = None
+        self._user_name = None
+        self._api_key = None
+        self._project_name = None
+        self._run_id = None
+        self._model_name = None
+        self._task_category = None
+        self._task = None
+        self._model_architecture = None
+        self._model_description = None
+        self._model_version = None
+        self._limitations = None
+        self._intended_users = None
+        self._training_data_size = None
+        self._training_data_size_units = None
+        self._training_data_description = None
+        self._training_data_source = None
+        self._training_date = None
+        self._license = None
+        self._citation = None
+        self._dependencies = None
+        self._pretrained = None
+
+    def init(self, user_name, api_key, run_id, project_name=None):
+        self._user_name = user_name
+        self._api_key = api_key
+        self._project_name = project_name
+        self._run_id = run_id
+
+    def create(self, model_name: str, task_category: str, task: str, model_architecture: str, model_version: str,
+               training_date: str, model_license: str, dependencies: list, pretrained: str,
+               model_description: Optional[str] = None,
+               limitations: Optional[str] = None, intended_users: Optional[str] = None,
+               training_data_size: Optional[str] = None,
+               training_data_size_units: Optional[str] = None, training_data_description: Optional[str] = None,
+               training_data_source: Optional[str] = None,
+               citation: Optional[str] = None):
+        self._model_name = model_name
+        self._task_category = task_category
+        self._task = task
+        self._model_architecture = model_architecture
+        self._model_description = model_description
+        self._model_version = model_version
+        self._limitations = limitations
+        self._intended_users = intended_users
+        self._training_data_size = training_data_size
+        self._training_data_size_units = training_data_size_units
+        self._training_data_description = training_data_description
+        self._training_data_source = training_data_source
+        self._training_date = training_date
+        self._license = model_license
+        self._citation = citation
+        self._dependencies = dependencies
+        self._pretrained = pretrained
 
     def to_dict(self):
         return self.__dict__
 
     def to_json(self):
         return json.dumps(self.__dict__)
 
     def from_dict(self, d):
         self.__dict__ = d
 
     def from_json(self, j):
         self.__dict__ = json.loads(j)
 
-
     @property
     def task_category(self) -> Optional[str]:
         return self._task_category
 
-
     @task_category.setter
     def task_category(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("task_category must be a string or None.")
         self._task_category = value
 
     @property
@@ -202,62 +240,81 @@
 
     @license.setter
     def license(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("license must be a string or None.")
         self._license = value
 
+    @property
+    def dependencies(self) -> Optional[str]:
+        return self._dependencies
+
+    @dependencies.setter
+    def dependencies(self, value: Optional[str]) -> None:
+        if value is not isinstance(value, list):
+            raise ValueError("dependencies must be a list")
+        self._dependencies = value
+
+    @property
+    def pretrained(self) -> Optional[str]:
+        return self._pretrained
+
+    @pretrained.setter
+    def pretrained(self, value: Optional[str]) -> None:
+        if value is not isinstance(value, bool):
+            raise ValueError("pretrained must be a boolean")
+        self._pretrained = value
 
 
 
 
 class Model:
 
-    def __init__(self, user_name, api_key, project_name, run_id):
+    def __init__(self):
         self.model_card = None
+        self.user_name = None
+        self.api_key = None
+        self._project_name = None
+        self._run_id = None
+
+    def init(self, user_name, api_key, run_id, project_name=None):
         self.user_name = user_name
         self.api_key = api_key
         self._project_name = project_name
         self._run_id = run_id
 
-
-    def create(self, model, dependencies, model_card, pretrained=True):
+    def create(self, model, model_card: ModelCard):
         if self.user_name is None:
             raise Exception("Please call dequeai.init(user_name, api_key, project_name) before creating model")
         if model is None:
             raise Exception("Please provide a valid model")
         try:
             import torch
         except ImportError:
             raise ImportError("PyTorch is required for creating model.")
 
             # Check if the model is a PyTorch model
         if not isinstance(model, torch.nn.Module):
             raise Exception('Model should be an instance of a PyTorch nn.Module.')
 
-        if dependencies is None or not isinstance(dependencies, list):
-            raise Exception("Please provide a valid dependencies list")
-
-        p2 = multiprocessing.Process(target=self._create_task, args=(model,  dependencies, model_card, pretrained))
+        p2 = multiprocessing.Process(target=self._create_task, args=(model, model_card))
         p2.start()
 
     def _create_task(self, model, dependencies, model_card, pretrained):
 
         file_name = f"{self._project_name}/.pt"
         try:
             import torch
         except ImportError:
             raise ImportError("PyTorch is required for creating model.")
 
         torch.save(model, file_name)
 
         dest_path = "users/" + self.user_name + "/projects/" + self._project_name + "/runs/" + self._run_id + "/model/" + file_name
 
-
-
         req_data = {"user_name": self.user_name, "destination_path": dest_path}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/appstore/model/upload/presigned_url/read/",
                              json=req_data)
         res = resp.json()
         print(res)
         with open(file_name, 'rb') as f:
             files = {'file': (file_name, f)}
@@ -266,22 +323,23 @@
             else:
                 # TODO: for google we need a different way to save data
                 object_text = f.read()
                 headers = {'Content-type': "application/octet-stream"}
                 http_response = requests.put(url=res['url'], data=object_text, headers=headers)
             print(http_response)
 
-        req_data = {"user_name": self.user_name, "dependencies": dependencies, "pretrained": pretrained,"model":self._project_name,"file_url":dest_path,"bucket_name":res['bucket_name'],"bucket_region":res['bucket_region'],
-                    "project_name": self._project_name, "run_id": self._run_id,"model_card": model_card}
+        req_data = {"user_name": self.user_name, "dependencies": dependencies, "pretrained": pretrained,
+                    "model": self._project_name, "file_url": dest_path, "bucket_name": res['bucket_name'],
+                    "bucket_region": res['bucket_region'],
+                    "project_name": self._project_name, "run_id": self._run_id, "model_card": model_card}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/appstore/model/create/",
                              json=req_data)
         res = resp.json()
         print(res)
-                # we record the meta data
-
+        # we record the meta data
 
     def load(self, model_name, run_id=None):
         if self.user_name is None:
             raise Exception("Please call dequeai.init(user_name, api_key, project_name) before loading model")
         req_data = {
             "user_name": self.user_name,
             "run_id": run_id,
@@ -331,15 +389,13 @@
                 else:
                     raise ValueError(
                         "Invalid type in dictionary. Allowed values include builtin types and Deque data types " + str(
                             type(value)) + " " + str(value.__class__.__module__))
         return new_data
 
 
-
-
 if __name__ == "__main__":
     mc = ModelCard()
     mc.__setattr__("model_name", "test")
     print(mc.model_name)
     print(mc)
-    #mc.init("test", "test", "test")
+    # mc.init("test", "test", "test")
```

### Comparing `dequeai-0.802/dequeai/dequeai_run.py` & `dequeai-0.804/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                                "project_name": self._project_name, "user_name": user_name}
         self._model_logged = False
         self._code_logged = False
         self._environment_logged = False
         self._resources_logged = False
         print(
             f"Run initialized with project name as {self._project_name} for user {self.user_name} and run id {self._run_id}")
+        return self._run_id
 
     def finish(self):
         self._running = False
         os.environ["running"] = "no"
         if self._res_monitor is not None:
             self._res_monitor.terminate()
```

### Comparing `dequeai-0.802/dequeai/parsing_service.py` & `dequeai-0.804/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.802/dequeai/rest_connect.py` & `dequeai-0.804/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.802/dequeai/util.py` & `dequeai-0.804/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.802/setup.py` & `dequeai-0.804/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000802',
+    version='0.00000804',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

