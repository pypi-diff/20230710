# Comparing `tmp/coiled-0.8.6.dev1.tar.gz` & `tmp/coiled-0.8.6.dev10.tar.gz`

## Comparing `coiled-0.8.6.dev1.tar` & `coiled-0.8.6.dev10.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/context.py
--rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/exceptions.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/magic.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/run.py
--rw-r--r--   0        0        0    19898 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/types.py
--rw-r--r--   0        0        0    54964 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    45605 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/__init__.py
--rw-r--r--   0        0        0    92333 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/cluster.py
--rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.6.dev1/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/auth.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/context.py
+-rw-r--r--   0        0        0   102249 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/exceptions.py
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/magic.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/run.py
+-rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/scan.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/types.py
+-rw-r--r--   0        0        0    54964 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    45605 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    92578 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    58959 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/pyproject.toml
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 coiled-0.8.6.dev10/PKG-INFO
```

### Comparing `coiled-0.8.6.dev1/coiled/__init__.py` & `coiled-0.8.6.dev10/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/analytics.py` & `coiled-0.8.6.dev10/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/auth.py` & `coiled-0.8.6.dev10/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cluster.py` & `coiled-0.8.6.dev10/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/coiled.yaml` & `coiled-0.8.6.dev10/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/context.py` & `coiled-0.8.6.dev10/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/core.py` & `coiled-0.8.6.dev10/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/exceptions.py` & `coiled-0.8.6.dev10/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/magic.py` & `coiled-0.8.6.dev10/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/run.py` & `coiled-0.8.6.dev10/coiled/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 from __future__ import annotations
 
 import functools
+import sys
 import threading
 from typing import Optional, Union
 
 import dask.distributed
 from dask.base import tokenize
+from dask.utils import parse_timedelta
 
 import coiled
 
+from .shutdown import NoClientShutdown
+
 _clients = {}
 _lock = threading.RLock()
 _clusters = {}
 
 
 class Function:
     """A function that you can run remotely"""
 
-    def __init__(self, function, cluster_kwargs):
+    def __init__(self, function, cluster_kwargs, keepalive):
         self.function = function
         self._cluster_kwargs = cluster_kwargs
+        self.keepalive = parse_timedelta(keepalive)
 
     @functools.cached_property
     def _name(self):
-        token = tokenize(**self._cluster_kwargs)
+        token = tokenize(
+            sys.executable,
+            # TODO: include something about the software environment
+            **self._cluster_kwargs,
+        )
         return f"run-{token[:8]}"
 
     @property
     def cluster(self) -> coiled.Cluster:
         with _lock:
             try:
                 return _clusters[self._name]
@@ -41,22 +50,25 @@
     def client(self) -> dask.distributed.Client:
         with _lock:
             try:
                 return _clients[self._name]
             except KeyError:
                 client = self.cluster.get_client()
                 if self.cluster.shutdown_on_close:
-                    client.register_scheduler_plugin(NoClientShutdown())
+                    client.register_scheduler_plugin(NoClientShutdown(keepalive=self.keepalive))
                 _clients[self._name] = client
                 return client
 
     def __call__(self, *args, **kwargs):
         # TODO, priority and stuff
         return self.client.run_on_scheduler(self.function, *args, **kwargs)
 
+    def local(self, *args, **kwargs):
+        return self.function(*args, **kwargs)
+
     def submit(self, *args, **kwargs) -> dask.distributed.Future:
         """Submit function call for asynchronous execution
 
         This immediately returns a Dask Future, allowing for the submission of
         many tasks in parallel.
 
         Example
@@ -91,14 +103,15 @@
     cpu: Optional[Union[int, list[int]]] = None,
     memory: Optional[Union[str, list[str]]] = None,
     gpu: Optional[bool] = None,
     account: Optional[str] = None,
     region: Optional[str] = None,
     arm: Optional[bool] = None,
     shutdown_on_close: bool = True,
+    keepalive="30 seconds",
 ):
     """
     Decorate a function to run on cloud infrastructure
 
     This creates a ``Function`` object that executes its code on a remote cluster
     with the hardware and software specified in the arguments to the decorator.
     It can run either as a normal function, or it can return Dask Futures for
@@ -149,20 +162,10 @@
             scheduler_gpu=gpu,
             region=region,
             arm=arm,
             shutdown_on_close=shutdown_on_close,
             tags={"coiled-cluster-type": "run/python"},
         )
 
-        return Function(func, cluster_kwargs)
+        return Function(func, cluster_kwargs, keepalive=keepalive)
 
     return decorator
-
-
-class NoClientShutdown(dask.distributed.SchedulerPlugin):
-    """Shut down a scheduler if all of the clients have gone"""
-
-    name = "NoClientShutdown"
-
-    def remove_client(self, scheduler, client):
-        if set(scheduler.clients) == {"fire-and-forget"}:
-            scheduler._ongoing_background_tasks.call_soon(scheduler.close)
```

### Comparing `coiled-0.8.6.dev1/coiled/scan.py` & `coiled-0.8.6.dev10/coiled/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from importlib_metadata import Distribution, PackagePath, PathDistribution
 from packaging.version import InvalidVersion
 from packaging.version import parse as parse_version
 from rich.progress import Progress
 from typing_extensions import Literal
 
 from coiled.types import CondaPackage, CondaPlaceHolder, PackageInfo
-from coiled.utils import COILED_LOCAL_PACKAGE_PREFIX, parse_file_uri
+from coiled.utils import COILED_LOCAL_PACKAGE_PREFIX, parse_file_uri, recurse_importable_python_files
 
 logger = getLogger("coiled.package_sync")
 subdir_datas = {}
 PYTHON_VERSION = platform.python_version_tuple()
 
 
 class ResilientDistribution(PathDistribution):
@@ -446,21 +446,22 @@
 
     # Handle modules that are not installed via pip or conda
     pkg_paths = {pkg["path"].resolve() for pkg in results if pkg["path"]}
     extra_paths = {p.resolve() for p in locations if prefix not in p.parents} - pkg_paths
     for extra_path in extra_paths:
         if not extra_path.is_dir():
             continue
-        results.append(
-            {
-                "name": f"{COILED_LOCAL_PACKAGE_PREFIX}{extra_path.name.replace('-', '_')}",
-                "path": extra_path,
-                "source": "pip",
-                "version": "0.0.0",
-                "channel_url": None,
-                "channel": None,
-                "subdir": None,
-                "conda_name": None,
-                "wheel_target": str(extra_path),
-            }
-        )
+        if any(recurse_importable_python_files(extra_path)):
+            results.append(
+                {
+                    "name": f"{COILED_LOCAL_PACKAGE_PREFIX}{extra_path.name.replace('-', '_')}",
+                    "path": extra_path,
+                    "source": "pip",
+                    "version": "0.0.0",
+                    "channel_url": None,
+                    "channel": None,
+                    "subdir": None,
+                    "conda_name": None,
+                    "wheel_target": str(extra_path),
+                }
+            )
     return sorted(results, key=lambda pkg: pkg["name"])
```

### Comparing `coiled-0.8.6.dev1/coiled/software.py` & `coiled-0.8.6.dev10/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/types.py` & `coiled-0.8.6.dev10/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/utils.py` & `coiled-0.8.6.dev10/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/websockets.py` & `coiled-0.8.6.dev10/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/config.py` & `coiled-0.8.6.dev10/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/core.py` & `coiled-0.8.6.dev10/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/curl.py` & `coiled-0.8.6.dev10/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/env.py` & `coiled-0.8.6.dev10/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/login.py` & `coiled-0.8.6.dev10/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/package_sync.py` & `coiled-0.8.6.dev10/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/prefect.py` & `coiled-0.8.6.dev10/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/run.py` & `coiled-0.8.6.dev10/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/utils.py` & `coiled-0.8.6.dev10/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/cluster/__init__.py` & `coiled-0.8.6.dev10/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/cluster/better_logs.py` & `coiled-0.8.6.dev10/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/cluster/logs.py` & `coiled-0.8.6.dev10/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/cluster/metrics.py` & `coiled-0.8.6.dev10/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/cluster/ssh.py` & `coiled-0.8.6.dev10/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/cluster/utils.py` & `coiled-0.8.6.dev10/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/notebook/__init__.py` & `coiled-0.8.6.dev10/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/notebook/notebook.py` & `coiled-0.8.6.dev10/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/setup/__init__.py` & `coiled-0.8.6.dev10/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/setup/amp.py` & `coiled-0.8.6.dev10/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/setup/aws.py` & `coiled-0.8.6.dev10/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/setup/entry.py` & `coiled-0.8.6.dev10/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/setup/gcp.py` & `coiled-0.8.6.dev10/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/cli/setup/prometheus.py` & `coiled-0.8.6.dev10/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/extensions/prefect/runners.py` & `coiled-0.8.6.dev10/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/extensions/prefect/workers.py` & `coiled-0.8.6.dev10/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/v2/__init__.py` & `coiled-0.8.6.dev10/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/v2/cluster.py` & `coiled-0.8.6.dev10/coiled/v2/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,18 @@
         ``default_cluster_timeout`` set on parent Cloud by default.
     environ
         Dictionary of environment variables.
     send_dask_config
         Whether to send a frozen copy of local dask.config to the cluster.
     backend_options
         Dictionary of backend specific options.
+    show_widget
+        Whether to use the rich-based widget display in IPython/Jupyter (ignored if not in those environments).
+        For use cases involving multiple Clusters at once, show_widget=False is recommended.
+        (Default: True)
     tags
         Dictionary of tags.
     wait_for_workers
         Whether to wait for a number of workers before returning control
         of the prompt back to the user. Usually, computations will run better
         if you wait for most workers before submitting tasks to the cluster.
         You can wait for all workers by passing ``True``, or not wait for any
```

### Comparing `coiled-0.8.6.dev1/coiled/v2/core.py` & `coiled-0.8.6.dev10/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/v2/cwi_log_link.py` & `coiled-0.8.6.dev10/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/v2/states.py` & `coiled-0.8.6.dev10/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/v2/widgets/__init__.py` & `coiled-0.8.6.dev10/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/v2/widgets/rich.py` & `coiled-0.8.6.dev10/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/coiled/v2/widgets/util.py` & `coiled-0.8.6.dev10/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/LICENSE` & `coiled-0.8.6.dev10/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/README.md` & `coiled-0.8.6.dev10/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/pyproject.toml` & `coiled-0.8.6.dev10/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.6.dev1/PKG-INFO` & `coiled-0.8.6.dev10/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.6.dev1
+Version: 0.8.6.dev10
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.8.6.dev1 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.8.6.dev10 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

