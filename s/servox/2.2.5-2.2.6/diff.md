# Comparing `tmp/servox-2.2.5.tar.gz` & `tmp/servox-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servox-2.2.5.tar", max compression
+gzip compressed data, was "servox-2.2.6.tar", max compression
```

## Comparing `servox-2.2.5.tar` & `servox-2.2.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    36172 2023-06-15 21:31:28.584488 servox-2.2.5/CHANGELOG.md
--rw-r--r--   0        0        0    11385 2023-06-15 21:31:28.584488 servox-2.2.5/LICENSE
--rw-r--r--   0        0        0    51279 2023-06-15 21:31:28.588488 servox-2.2.5/README.md
--rw-r--r--   0        0        0     3639 2023-06-15 21:31:28.588488 servox-2.2.5/pyproject.toml
--rw-r--r--   0        0        0     1832 2023-06-15 21:31:28.588488 servox-2.2.5/servo/__init__.py
--rw-r--r--   0        0        0     9712 2023-06-15 21:31:28.588488 servox-2.2.5/servo/api.py
--rw-r--r--   0        0        0    15480 2023-06-15 21:31:28.588488 servox-2.2.5/servo/assembly.py
--rw-r--r--   0        0        0    44344 2023-06-15 21:31:28.588488 servox-2.2.5/servo/checks.py
--rw-r--r--   0        0        0    78505 2023-06-15 21:31:28.592488 servox-2.2.5/servo/cli.py
--rw-r--r--   0        0        0    27810 2023-06-15 21:31:28.592488 servox-2.2.5/servo/configuration.py
--rw-r--r--   0        0        0    16845 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connector.py
--rw-r--r--   0        0        0      680 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/__init__.py
--rw-r--r--   0        0        0    31949 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kube_metrics.py
--rw-r--r--   0        0        0    95520 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes.py
--rw-r--r--   0        0        0      799 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/__init__.py
--rw-r--r--   0        0        0     2528 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/base.py
--rw-r--r--   0        0        0    11264 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/base_workload.py
--rw-r--r--   0        0        0     5158 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/container.py
--rw-r--r--   0        0        0    14837 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/deployment.py
--rw-r--r--   0        0        0     1195 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/namespace.py
--rw-r--r--   0        0        0    12193 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/pod.py
--rw-r--r--   0        0        0     1779 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/replicaset.py
--rw-r--r--   0        0        0     2722 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/service.py
--rw-r--r--   0        0        0     3702 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/statefulset.py
--rw-r--r--   0        0        0     1625 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/kubernetes_helpers/util.py
--rw-r--r--   0        0        0    47402 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/opsani_dev.py
--rw-r--r--   0        0        0    40511 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/prometheus.py
--rw-r--r--   0        0        0     1708 2023-06-15 21:31:28.592488 servox-2.2.5/servo/connectors/scripts.py
--rw-r--r--   0        0        0    19127 2023-06-15 21:31:28.596489 servox-2.2.5/servo/connectors/vegeta.py
--rw-r--r--   0        0        0      983 2023-06-15 21:31:28.596489 servox-2.2.5/servo/connectors/vegeta_target_schema.json
--rw-r--r--   0        0        0     2665 2023-06-15 21:31:28.596489 servox-2.2.5/servo/connectors/wait.py
--rw-r--r--   0        0        0      607 2023-06-15 21:31:28.596489 servox-2.2.5/servo/encoders.py
--rw-r--r--   0        0        0     1771 2023-06-15 21:31:28.596489 servox-2.2.5/servo/entry_points.py
--rw-r--r--   0        0        0     5335 2023-06-15 21:31:28.596489 servox-2.2.5/servo/errors.py
--rw-r--r--   0        0        0    38440 2023-06-15 21:31:28.596489 servox-2.2.5/servo/events.py
--rw-r--r--   0        0        0    10685 2023-06-15 21:31:28.596489 servox-2.2.5/servo/fast_fail.py
--rw-r--r--   0        0        0    14123 2023-06-15 21:31:28.596489 servox-2.2.5/servo/logging.py
--rw-r--r--   0        0        0    61151 2023-06-15 21:31:28.596489 servox-2.2.5/servo/pubsub.py
--rw-r--r--   0        0        0     6750 2023-06-15 21:31:28.596489 servox-2.2.5/servo/repeating.py
--rw-r--r--   0        0        0    26006 2023-06-15 21:31:28.596489 servox-2.2.5/servo/runner.py
--rw-r--r--   0        0        0    24642 2023-06-15 21:31:28.596489 servox-2.2.5/servo/servo.py
--rw-r--r--   0        0        0     7891 2023-06-15 21:31:28.596489 servox-2.2.5/servo/telemetry.py
--rw-r--r--   0        0        0      808 2023-06-15 21:31:28.596489 servox-2.2.5/servo/types/__init__.py
--rw-r--r--   0        0        0    10891 2023-06-15 21:31:28.596489 servox-2.2.5/servo/types/api.py
--rw-r--r--   0        0        0    32100 2023-06-15 21:31:28.596489 servox-2.2.5/servo/types/core.py
--rw-r--r--   0        0        0     2232 2023-06-15 21:31:28.596489 servox-2.2.5/servo/types/kubernetes.py
--rw-r--r--   0        0        0    23824 2023-06-15 21:31:28.596489 servox-2.2.5/servo/types/settings.py
--rw-r--r--   0        0        0     4575 2023-06-15 21:31:28.596489 servox-2.2.5/servo/types/slo.py
--rw-r--r--   0        0        0      777 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/__init__.py
--rw-r--r--   0        0        0     2854 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/associations.py
--rw-r--r--   0        0        0     5404 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/duration_str.py
--rw-r--r--   0        0        0     2314 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/hashing.py
--rw-r--r--   0        0        0    17660 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/inspect.py
--rw-r--r--   0        0        0     2116 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/key_paths.py
--rw-r--r--   0        0        0     2427 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/pydantic.py
--rw-r--r--   0        0        0     2529 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/strings.py
--rw-r--r--   0        0        0    15189 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/subprocess.py
--rw-r--r--   0        0        0     1016 2023-06-15 21:31:28.596489 servox-2.2.5/servo/utilities/yaml.py
--rw-r--r--   0        0        0    52862 1970-01-01 00:00:00.000000 servox-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0    36555 2023-07-10 18:52:10.512874 servox-2.2.6/CHANGELOG.md
+-rw-r--r--   0        0        0    11385 2023-07-10 18:52:10.512874 servox-2.2.6/LICENSE
+-rw-r--r--   0        0        0    51279 2023-07-10 18:52:10.512874 servox-2.2.6/README.md
+-rw-r--r--   0        0        0     3639 2023-07-10 18:52:10.516873 servox-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1832 2023-07-10 18:52:10.516873 servox-2.2.6/servo/__init__.py
+-rw-r--r--   0        0        0    10136 2023-07-10 18:52:10.516873 servox-2.2.6/servo/api.py
+-rw-r--r--   0        0        0    15480 2023-07-10 18:52:10.516873 servox-2.2.6/servo/assembly.py
+-rw-r--r--   0        0        0    44344 2023-07-10 18:52:10.516873 servox-2.2.6/servo/checks.py
+-rw-r--r--   0        0        0    78505 2023-07-10 18:52:10.520873 servox-2.2.6/servo/cli.py
+-rw-r--r--   0        0        0    28118 2023-07-10 18:52:10.520873 servox-2.2.6/servo/configuration.py
+-rw-r--r--   0        0        0    16845 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connector.py
+-rw-r--r--   0        0        0      680 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/__init__.py
+-rw-r--r--   0        0        0    31949 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kube_metrics.py
+-rw-r--r--   0        0        0    95520 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes.py
+-rw-r--r--   0        0        0      799 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/__init__.py
+-rw-r--r--   0        0        0     2528 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/base.py
+-rw-r--r--   0        0        0    11264 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/base_workload.py
+-rw-r--r--   0        0        0     5158 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/container.py
+-rw-r--r--   0        0        0    14837 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/deployment.py
+-rw-r--r--   0        0        0     1195 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/namespace.py
+-rw-r--r--   0        0        0    12193 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/pod.py
+-rw-r--r--   0        0        0     1779 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/replicaset.py
+-rw-r--r--   0        0        0     2722 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/service.py
+-rw-r--r--   0        0        0     3702 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/statefulset.py
+-rw-r--r--   0        0        0     1625 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/util.py
+-rw-r--r--   0        0        0    47402 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/opsani_dev.py
+-rw-r--r--   0        0        0    40511 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/prometheus.py
+-rw-r--r--   0        0        0     1708 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/scripts.py
+-rw-r--r--   0        0        0    19127 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/vegeta.py
+-rw-r--r--   0        0        0      983 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/vegeta_target_schema.json
+-rw-r--r--   0        0        0     2665 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/wait.py
+-rw-r--r--   0        0        0      607 2023-07-10 18:52:10.524874 servox-2.2.6/servo/encoders.py
+-rw-r--r--   0        0        0     1771 2023-07-10 18:52:10.524874 servox-2.2.6/servo/entry_points.py
+-rw-r--r--   0        0        0     5459 2023-07-10 18:52:10.524874 servox-2.2.6/servo/errors.py
+-rw-r--r--   0        0        0    38440 2023-07-10 18:52:10.524874 servox-2.2.6/servo/events.py
+-rw-r--r--   0        0        0    10685 2023-07-10 18:52:10.524874 servox-2.2.6/servo/fast_fail.py
+-rw-r--r--   0        0        0    14253 2023-07-10 18:52:10.524874 servox-2.2.6/servo/logging.py
+-rw-r--r--   0        0        0    61151 2023-07-10 18:52:10.524874 servox-2.2.6/servo/pubsub.py
+-rw-r--r--   0        0        0     6750 2023-07-10 18:52:10.524874 servox-2.2.6/servo/repeating.py
+-rw-r--r--   0        0        0    29014 2023-07-10 18:52:10.524874 servox-2.2.6/servo/runner.py
+-rw-r--r--   0        0        0    26050 2023-07-10 18:52:10.524874 servox-2.2.6/servo/servo.py
+-rw-r--r--   0        0        0     7891 2023-07-10 18:52:10.524874 servox-2.2.6/servo/telemetry.py
+-rw-r--r--   0        0        0      808 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/__init__.py
+-rw-r--r--   0        0        0    10891 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/api.py
+-rw-r--r--   0        0        0    32100 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/core.py
+-rw-r--r--   0        0        0     2232 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/kubernetes.py
+-rw-r--r--   0        0        0    23824 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/settings.py
+-rw-r--r--   0        0        0     4575 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/slo.py
+-rw-r--r--   0        0        0      777 2023-07-10 18:52:10.524874 servox-2.2.6/servo/utilities/__init__.py
+-rw-r--r--   0        0        0     2854 2023-07-10 18:52:10.524874 servox-2.2.6/servo/utilities/associations.py
+-rw-r--r--   0        0        0     5404 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/duration_str.py
+-rw-r--r--   0        0        0     2314 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/hashing.py
+-rw-r--r--   0        0        0    17660 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/inspect.py
+-rw-r--r--   0        0        0     2116 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/key_paths.py
+-rw-r--r--   0        0        0     2427 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/pydantic.py
+-rw-r--r--   0        0        0     2529 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/strings.py
+-rw-r--r--   0        0        0    15189 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/subprocess.py
+-rw-r--r--   0        0        0     1016 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/yaml.py
+-rw-r--r--   0        0        0    52862 1970-01-01 00:00:00.000000 servox-2.2.6/PKG-INFO
```

### Comparing `servox-2.2.5/CHANGELOG.md` & `servox-2.2.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 Servo is distributed under the terms of the Apache 2.0 license.
 
 This changelog catalogs all notable changes made to the project. The format is
 based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). Releases are
 versioned in accordance with [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.6] "genesis" - 2023-07-10
+
+### Changed
+
+- A unique identifier for each servo deployment is now supported in configuration and sent with every request to the backend
+- A unique identifier for each command received from the backend is now retrieved from the response to the WHATS_NEXT request and included on all servo requests for the given command (progress and completion)
+
 ## [2.2.5] "genesis" - 2023-06-15
 
 ### Changed
 
 - 404 no longer considered fatal status code
 - Checks now support exponential backoff
 - Checks delay configuration now defaults to exponential backoff
```

### Comparing `servox-2.2.5/LICENSE` & `servox-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/README.md` & `servox-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/pyproject.toml` & `servox-2.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servox"
-version = "2.2.5"
+version = "2.2.6"
 description = "Opsani Servo: The Next Generation"
 homepage = "https://opsani.com/"
 repository = "https://github.com/opsani/servox"
 authors = ["Blake Watters <blake@opsani.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [
```

### Comparing `servox-2.2.5/servo/__init__.py` & `servox-2.2.6/servo/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/api.py` & `servox-2.2.6/servo/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,56 +90,64 @@
         else:
             raise ValueError(f"unknown command: {self}")
 
 
 class Request(pydantic.BaseModel):
     event: Union[Events, str]  # TODO: Needs to be rethought -- used adhoc in some cases
     param: Optional[Dict[str, Any]]  # TODO: Switch to a union of supported types
+    servo_uid: Union[str, None] = None
 
     class Config:
         json_encoders = {
             Events: lambda v: str(v),
         }
 
 
 class Status(pydantic.BaseModel):
     status: Statuses
     message: Optional[str] = None
     reason: Optional[str] = None
     state: Optional[Dict[str, Any]] = None
     descriptor: Optional[Dict[str, Any]] = None
+    metrics: Union[dict[str, Any], None] = None
+    annotations: Union[dict[str, str], None] = None
+    command_uid: Union[str, None] = pydantic.Field(default=None, alias="cmd_uid")
 
     @classmethod
     def ok(
         cls, message: Optional[str] = None, reason: str = Reasons.success, **kwargs
     ) -> "Status":
         """Return a success (status="ok") status object."""
         return cls(status=ServoStatuses.ok, message=message, reason=reason, **kwargs)
 
     @classmethod
-    def from_error(cls, error: servo.errors.BaseError) -> "Status":
+    def from_error(cls, error: servo.errors.BaseError, **kwargs) -> "Status":
         """Return a status object representation from the given error."""
         if isinstance(error, servo.errors.AdjustmentRejectedError):
             status = ServoStatuses.rejected
         elif isinstance(error, servo.errors.EventAbortedError):
             status = ServoStatuses.aborted
         elif isinstance(error, servo.errors.EventCancelledError):
             status = ServoStatuses.cancelled
         else:
             status = ServoStatuses.failed
 
-        return cls(status=status, message=str(error), reason=error.reason)
+        return cls(status=status, message=str(error), reason=error.reason, **kwargs)
 
     def dict(
         self,
         *,
         exclude_unset: bool = True,
+        by_alias: bool = True,
         **kwargs,
     ) -> DictStrAny:
-        return super().dict(exclude_unset=exclude_unset, **kwargs)
+        return super().dict(exclude_unset=exclude_unset, by_alias=by_alias, **kwargs)
+
+    class Config:
+        allow_population_by_field_name = True
 
 
 class SleepResponse(pydantic.BaseModel):
     pass
 
 
 # SleepResponse '{"cmd": "SLEEP", "param": {"duration": 60, "data": {"reason": "no active optimization pipeline"}}}'
@@ -164,14 +172,15 @@
             return v.name
 
         return v
 
 
 class CommandResponse(pydantic.BaseModel):
     command: Commands = pydantic.Field(alias="cmd")
+    command_uid: Union[str, None] = pydantic.Field(alias="cmd_uid")
     param: Optional[
         Union[MeasureParams, Dict[str, Any]]
     ]  # TODO: Switch to a union of supported types, remove isinstance check from ServoRunner.measure when done
 
     class Config:
         json_encoders = {
             Commands: lambda v: v.value,
```

### Comparing `servox-2.2.5/servo/assembly.py` & `servox-2.2.6/servo/assembly.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/checks.py` & `servox-2.2.6/servo/checks.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/cli.py` & `servox-2.2.6/servo/cli.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/configuration.py` & `servox-2.2.6/servo/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,20 @@
 
         # Default prefix
         prefix = cls.__config__.env_prefix
         if prefix == "":
             prefix = re.sub(r"(?<!^)(?=[A-Z])", "_", base_name).upper() + "_"
 
         for name, field in cls.__fields__.items():
-            field.field_info.extra["env_names"] = {f"{prefix}{name}".upper()}
+            if (env_override := field.field_info.extra.get("env")) and not isinstance(
+                env_override, list
+            ):
+                field.field_info.extra["env_names"] = {env_override}
+            else:
+                field.field_info.extra["env_names"] = {f"{prefix}{name}".upper()}
 
     def yaml(
         self,
         *,
         include: Union[pydantic.AbstractSetIntStr, pydantic.MappingIntStrAny] = None,
         exclude: Union[pydantic.AbstractSetIntStr, pydantic.MappingIntStrAny] = None,
         by_alias: bool = False,
@@ -614,14 +619,15 @@
     See `Assembly` for details on how the concrete model is built.
 
     NOTE: Inherits from AbstractBaseConfiguration because of optimizer property
     """
 
     name: Optional[str] = None
     description: Optional[str] = None
+    servo_uid: Union[str, None] = pydantic.Field(default=None, env="SERVO_UID")
     optimizer: OptimizerTypes = {}
     connectors: Optional[Union[List[str], Dict[str, str]]] = pydantic.Field(
         None,
         description=(
             "An optional, explicit configuration of the active connectors.\n"
             "\nConfigurable as either an array of connector identifiers (names or class) or\n"
             "a dictionary where the keys specify the key path to the connectors configuration\n"
```

### Comparing `servox-2.2.5/servo/connector.py` & `servox-2.2.6/servo/connector.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/__init__.py` & `servox-2.2.6/servo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kube_metrics.py` & `servox-2.2.6/servo/connectors/kube_metrics.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes.py` & `servox-2.2.6/servo/connectors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/__init__.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/base.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/base.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/base_workload.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/base_workload.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/container.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/container.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/deployment.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/deployment.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/namespace.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/namespace.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/pod.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/pod.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/replicaset.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/replicaset.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/service.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/service.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/statefulset.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/statefulset.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/kubernetes_helpers/util.py` & `servox-2.2.6/servo/connectors/kubernetes_helpers/util.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/opsani_dev.py` & `servox-2.2.6/servo/connectors/opsani_dev.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/prometheus.py` & `servox-2.2.6/servo/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/scripts.py` & `servox-2.2.6/servo/connectors/scripts.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/vegeta.py` & `servox-2.2.6/servo/connectors/vegeta.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/vegeta_target_schema.json` & `servox-2.2.6/servo/connectors/vegeta_target_schema.json`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/connectors/wait.py` & `servox-2.2.6/servo/connectors/wait.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/encoders.py` & `servox-2.2.6/servo/encoders.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/entry_points.py` & `servox-2.2.6/servo/entry_points.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/errors.py` & `servox-2.2.6/servo/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,15 +124,19 @@
 
     @property
     def event(self) -> servo.Event:
         return self._event
 
 
 class UnexpectedEventError(EventError):
-    """The optimizer reported that an unexpected error was submitted."""
+    """The optimizer reported that an unexpected event was submitted."""
+
+
+class UnexpectedCommandIdError(EventError):
+    """The optimizer reported that an unexpected command ID was submitted."""
 
 
 class EventCancelledError(EventError):
     """The event was cancelled and processing was halted."""
 
 
 class MeasurementFailedError(EventError):
```

### Comparing `servox-2.2.5/servo/events.py` & `servox-2.2.6/servo/events.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/fast_fail.py` & `servox-2.2.6/servo/fast_fail.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/logging.py` & `servox-2.2.6/servo/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 import asyncio
 import functools
 import logging
 import pathlib
 import sys
 import time
 import traceback
-from typing import Any, Awaitable, Callable, Optional
+from typing import Any, Awaitable, Callable, Optional, Union
 
 import loguru
 
+import servo
 import servo.assembly
 import servo.events
 
 __all__ = (
     "Mixin",
     "Filter",
     "ProgressHandler",
@@ -131,14 +132,16 @@
             if not event_context:
                 return await self._report_error(
                     "declining request to report progress for record without an operation parameter or inferrable value from event context",
                     record,
                 )
             operation = event_context.operation()
 
+        command_uid: Union[str, None] = servo.current_command_uid()
+
         started_at = extra.get("started_at", None)
         if not started_at:
             if event_context:
                 started_at = event_context.created_at
             else:
                 return await self._report_error(
                     "declining request to report progress for record without a started_at parameter or inferrable value from event context",
@@ -151,14 +154,15 @@
             dict(
                 operation=operation,
                 progress=progress,
                 connector=connector_name,
                 event_context=event_context,
                 started_at=started_at,
                 message=message,
+                command_uid=command_uid,
             )
         )
 
     async def shutdown(self) -> None:
         """Shutdown the progress handler by emptying the queue and releasing the queue processor."""
         await self._queue.join()
```

### Comparing `servox-2.2.5/servo/pubsub.py` & `servox-2.2.6/servo/pubsub.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/repeating.py` & `servox-2.2.6/servo/repeating.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/runner.py` & `servox-2.2.6/servo/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 import servo
 import servo.api
 import servo.telemetry
 import servo.configuration
 import servo.utilities.key_paths
 import servo.utilities.strings
-from servo.servo import _set_current_servo
+from servo.servo import _set_current_servo, set_current_command_uid
 from servo.types import Adjustment, Control, Description, Duration, Measurement
 
 
 class ServoRunner(pydantic.BaseModel, servo.logging.Mixin):
     interactive: bool = False
     _servo: servo.Servo = pydantic.PrivateAttr(None)
     _connected: bool = pydantic.PrivateAttr(False)
@@ -131,66 +131,84 @@
             aggregate_description.components.extend(description.components)
             aggregate_description.metrics.extend(description.metrics)
 
         self.logger.success(f"Adjustment completed {summary}")
         return aggregate_description
 
     async def exec_command(self) -> servo.api.Status:
-        cmd_response = await self.servo.post_event(servo.api.Events.whats_next, None)
-        self.logger.info(f"What's Next? => {cmd_response.command}")
+        cmd_response: Union[
+            servo.api.CommandResponse, servo.api.Status
+        ] = await self.servo.post_event(servo.api.Events.whats_next, None)
         self.logger.trace(devtools.pformat(cmd_response))
+        self.logger.info(f"What's Next? => {cmd_response.command}")
+        set_current_command_uid(cmd_response.command_uid)
 
         if cmd_response.command == servo.api.Commands.describe:
             description = await self.describe(
                 Control(**cmd_response.param.get("control", {}))
             )
             self.logger.success(
                 f"Described: {len(description.components)} components, {len(description.metrics)} metrics"
             )
             self.logger.debug(devtools.pformat(description))
 
-            status = servo.api.Status.ok(descriptor=description.__opsani_repr__())
+            status = servo.api.Status.ok(
+                descriptor=description.__opsani_repr__(),
+                command_uid=cmd_response.command_uid,
+            )
             return await self.servo.post_event(servo.api.Events.describe, status.dict())
 
         elif cmd_response.command == servo.api.Commands.measure:
             try:
                 measurement = await self.measure(cmd_response.param)
                 self.logger.success(
                     f"Measured: {len(measurement.readings)} readings, {len(measurement.annotations)} annotations"
                 )
                 self.logger.trace(devtools.pformat(measurement))
-                param = measurement.__opsani_repr__()
+                status = servo.api.Status.ok(
+                    command_uid=cmd_response.command_uid,
+                    **measurement.__opsani_repr__(),
+                )
             except servo.errors.EventError as error:
                 self.logger.error(f"Measurement failed: {error}")
-                param = servo.api.Status.from_error(error).dict()
-                self.logger.error(f"Responding with {param}")
+                status = servo.api.Status.from_error(
+                    error=error,
+                    command_uid=cmd_response.command_uid,
+                )
+                self.logger.error(f"Responding with {status.dict()}")
                 self.logger.opt(exception=error).debug("Measure failure details")
 
-            return await self.servo.post_event(servo.api.Events.measure, param)
+            return await self.servo.post_event(servo.api.Events.measure, status.dict())
 
         elif cmd_response.command == servo.api.Commands.adjust:
             adjustments = servo.api.descriptor_to_adjustments(
                 cmd_response.param["state"]
             )
             control = Control(**cmd_response.param.get("control", {}))
 
             try:
                 description = await self.adjust(adjustments, control)
-                status = servo.api.Status.ok(state=description.__opsani_repr__())
+                status = servo.api.Status.ok(
+                    state=description.__opsani_repr__(),
+                    command_uid=cmd_response.command_uid,
+                )
 
                 components_count = len(description.components)
                 settings_count = sum(
                     len(component.settings) for component in description.components
                 )
                 self.logger.success(
                     f"Adjusted: {components_count} components, {settings_count} settings"
                 )
             except servo.EventError as error:
                 self.logger.error(f"Adjustment failed: {error}")
-                status = servo.api.Status.from_error(error)
+                status = servo.api.Status.from_error(
+                    error,
+                    command_uid=cmd_response.command_uid,
+                )
                 self.logger.error(f"Responding with {status.dict()}")
                 self.logger.opt(exception=error).debug("Adjust failure details")
 
             return await self.servo.post_event(servo.api.Events.adjust, status.dict())
 
         elif cmd_response.command == servo.api.Commands.sleep:
             # TODO: Model this
@@ -225,19 +243,33 @@
 
                 status = await self.exec_command()
                 if status.status == servo.api.OptimizerStatuses.unexpected_event:
                     self.logger.warning(
                         f"server reported unexpected event: {status.reason}"
                     )
 
-            except (httpx.TimeoutException, httpx.HTTPStatusError) as error:
+            except httpx.TimeoutException as error:
                 self.logger.warning(
-                    f"command execution failed HTTP client error: {error}"
+                    f"command execution failed HTTP client timeout error: {error}"
                 )
 
+            except httpx.HTTPStatusError as error:
+                if (
+                    error.response.status_code == 410
+                    and error.response.json().get("detail") == "unexpected servo_uid"
+                ):
+                    self.logger.warning(
+                        f"servo UID {self.servo.config.servo_uid} is no longer valid. Waiting for deprovisioning (will sleep for 1 hour)"
+                    )
+                    await asyncio.sleep(3600)
+                else:
+                    self.logger.warning(
+                        f"command execution failed HTTP client status error: {error}"
+                    )
+
             except pydantic.ValidationError as error:
                 self.logger.warning(
                     f"command execution failed with model validation error: {error}"
                 )
                 self.logger.opt(exception=error).debug(
                     "Pydantic model failed validation"
                 )
@@ -312,21 +344,34 @@
                 httpx.HTTPError,
                 max_time=lambda: self.config.settings.backoff.max_time(),
                 max_tries=lambda: self.config.settings.backoff.max_tries(),
                 on_giveup=giveup,
             )
             async def connect() -> None:
                 self.logger.info("Saying HELLO.", end=" ")
-                await self.servo.post_event(
-                    servo.api.Events.hello,
-                    dict(
-                        agent=servo.api.user_agent(),
-                        telemetry=self.servo.telemetry.values,
-                    ),
-                )
+                try:
+                    await self.servo.post_event(
+                        servo.api.Events.hello,
+                        dict(
+                            agent=servo.api.user_agent(),
+                            telemetry=self.servo.telemetry.values,
+                        ),
+                    )
+                except httpx.HTTPStatusError as error:
+                    if (
+                        error.response.status_code == 410
+                        and error.response.json().get("detail")
+                        == "unexpected servo_uid"
+                    ):
+                        self.logger.warning(
+                            f"servo UID {self.servo.config.servo_uid} is no longer valid. Waiting for deprovisioning (will sleep for 1 hour)"
+                        )
+                        await asyncio.sleep(3600)
+                    raise
+
                 self._connected = True
 
             self.logger.info(
                 f"Connecting to Opsani Optimizer @ {self.optimizer.url}..."
             )
             if self.interactive:
                 typer.confirm("Connect to the optimizer?", abort=True)
@@ -422,28 +467,47 @@
         async def handle_progress_exception(
             progress: dict[str, Any], error: Exception
         ) -> None:
             # FIXME: This needs to be made multi-servo aware
             # Restart the main event loop if we get out of sync with the server
             if isinstance(
                 error,
-                (servo.errors.UnexpectedEventError, servo.errors.EventCancelledError),
+                (
+                    servo.errors.UnexpectedEventError,
+                    servo.errors.EventCancelledError,
+                    servo.errors.UnexpectedCommandIdError,
+                ),
+            ) or (
+                isinstance(error, httpx.HTTPStatusError)
+                and error.response.status_code == 410
+                and error.response.json().get("detail")
             ):
-                if isinstance(error, servo.errors.UnexpectedEventError):
+                if isinstance(error, httpx.HTTPStatusError):
+                    self.logger.error(
+                        f"servo UID {servo.current_servo().config.servo_uid} is no longer valid: shutting down tasks to commence sleep loop"
+                    )
+                elif isinstance(error, servo.errors.UnexpectedEventError):
                     self.logger.error(
                         "servo has lost synchronization with the optimizer: restarting"
                     )
+                elif isinstance(error, servo.errors.UnexpectedCommandIdError):
+                    self.logger.error(
+                        "servo is processing outdated command: restarting"
+                    )
                 elif isinstance(error, servo.errors.EventCancelledError):
                     self.logger.error(
                         "optimizer has cancelled operation in progress: cancelling and restarting loop"
                     )
 
                     # Post a status to resolve the operation
                     operation = progress["operation"]
-                    status = servo.api.Status.from_error(error)
+                    command_uid = progress["command_uid"]
+                    status = servo.api.Status.from_error(
+                        error=error, command_uid=command_uid
+                    )
                     self.logger.error(f"Responding with {status.dict()}")
                     runner = self._runner_for_servo(servo.current_servo())
                     await runner.servo.post_event(operation, status.dict())
 
                 tasks = [
                     t for t in asyncio.all_tasks() if t is not asyncio.current_task()
                 ]
@@ -562,18 +626,24 @@
         secho(f"connectors:  {', '.join(sorted(names))}")
         secho(
             f"config file: {typer.style(str(self.assembly.config_file), bold=True, fg=typer.colors.YELLOW)}"
         )
 
         if len(self.assembly.servos) == 1:
             servo_ = self.assembly.servos[0]
-            optimizer = servo_.optimizer
 
+            servo_uid = typer.style(
+                servo_.config.servo_uid, bold=True, fg=typer.colors.WHITE
+            )
+            secho(f"servo UID: {servo_uid}")
+
+            optimizer = servo_.optimizer
             id = typer.style(optimizer.id, bold=True, fg=typer.colors.WHITE)
             secho(f"optimizer:   {id}")
+
             if optimizer.base_url != "https://api.opsani.com/":
                 base_url = typer.style(
                     f"{optimizer.base_url}", bold=True, fg=typer.colors.RED
                 )
                 secho(f"base url: {base_url}")
 
             if servo_.config.settings and servo_.config.settings.proxies:
```

### Comparing `servox-2.2.5/servo/servo.py` & `servox-2.2.6/servo/servo.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,25 @@
 import backoff
 import contextlib
 import contextvars
 from datetime import datetime, timedelta
 import devtools
 import enum
 import json
-from typing import cast, Any, Callable, Optional, Protocol, Sequence, Tuple, Union
+from typing import (
+    cast,
+    Any,
+    Callable,
+    Iterable,
+    Optional,
+    Protocol,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 from authlib.integrations.httpx_client import AsyncOAuth2Client
 import httpx
 import pydantic
 import watchfiles
 
 import servo.api
@@ -37,18 +47,21 @@
 import servo.events
 import servo.errors
 import servo.pubsub
 import servo.types
 import servo.utilities
 import servo.utilities.pydantic
 
-__all__ = ["Servo", "Events", "current_servo"]
+__all__ = ["Servo", "Events", "current_servo", "current_command_uid"]
 
 
 _current_context_var = contextvars.ContextVar("servox.current_servo", default=None)
+_current_command_uid_context_var = contextvars.ContextVar(
+    "servox.current_command_uid", default=None
+)
 
 
 def current_servo() -> Optional["Servo"]:
     """Return the active servo for the current execution context.
 
     The value is managed by a contextvar and is concurrency safe.
     """
@@ -59,14 +72,27 @@
     """Set the active servo for the current execution context.
 
     The value is managed by a contextvar and is concurrency safe.
     """
     _current_context_var.set(servo_)
 
 
+def current_command_uid() -> Union[str, None]:
+    """Return the command ID that the current asyncio task was invoked under.
+
+    A new copy is automatically generated on creation of tasks and functions as a closure of the ID even after it is
+    updated by the main loop task
+    """
+    return _current_command_uid_context_var.get()
+
+
+def set_current_command_uid(value: Union[str, None]) -> None:
+    _current_command_uid_context_var.set(value)
+
+
 class Events(str, enum.Enum):
     """An enumeration of the names of standard events defined by the servo."""
 
     # Lifecycle events
     attach = "attach"
     detach = "detach"
     startup = "startup"
@@ -419,25 +445,30 @@
         elif status.status == servo.api.OptimizerStatuses.unexpected_event:
             # We have lost sync with the backend, raise an exception to halt broken execution
             raise servo.errors.UnexpectedEventError(status.reason)
         elif status.status == servo.api.OptimizerStatuses.cancelled:
             # Optimizer wants to cancel the operation
             raise servo.errors.EventCancelledError(status.reason or "Command cancelled")
         elif status.status == servo.api.OptimizerStatuses.invalid:
-            self.logger.warning(f"progress report was rejected as invalid")
+            self.logger.warning(
+                f"progress report was rejected as invalid: {devtools.pformat(status.dict())}"
+            )
+            if status.reason == "unexpected cmd_uid":
+                raise servo.errors.UnexpectedCommandIdError(status.reason)
         else:
             raise ValueError(f'unknown error status: "{status.status}"')
 
     def progress_request(
         self,
         operation: str,
         progress: servo.types.Numeric,
         started_at: datetime,
         message: Optional[str],
         *,
+        command_uid: Union[str, None] = None,
         connector: Optional[str] = None,
         event_context: Optional["servo.events.EventContext"] = None,
         time_remaining: Optional[
             Union[servo.types.Numeric, servo.types.Duration]
         ] = None,
         logs: Optional[list[str]] = None,
     ) -> Tuple[str, dict[str, Any]]:
@@ -461,14 +492,15 @@
                 )
         else:
             time_remaining_in_seconds = None
 
         params = dict(
             progress=float(progress),
             runtime=float(runtime.total_seconds()),
+            cmd_uid=command_uid,
         )
         set_if(params, "message", message)
 
         return (operation, params)
 
     async def post_event(
         self, event: Events, param
@@ -479,15 +511,17 @@
             max_time=lambda: self.config.settings.backoff.max_time(),
             max_tries=lambda: self.config.settings.backoff.max_tries(),
             giveup=servo.api.is_fatal_status_code,
         )
         async def _post_event(
             event: Events, param
         ) -> Union[servo.api.CommandResponse, servo.api.Status]:
-            event_request = servo.api.Request(event=event, param=param)
+            event_request = servo.api.Request(
+                event=event, param=param, servo_uid=self.config.servo_uid
+            )
             self.logger.trace(
                 f"POST event request: {devtools.pformat(event_request.json())}"
             )
 
             try:
                 response = await self._api_client.post(
                     "servo", data=event_request.json()
@@ -641,16 +675,27 @@
             matching: An optional filter to limit the checks that are executed.
             halt_on: The severity level of errors that should halt execution of checks.
 
         Returns:
             A list of check objects that describe the outcomes of the checks that were run.
         """
         try:
-            event_request = servo.api.Request(event=servo.api.Events.hello)
+            event_request = servo.api.Request(
+                event=servo.api.Events.hello, servo_uid=self.config.servo_uid
+            )
             response = await self._api_client.post("servo", data=event_request.json())
+            if (
+                response.status_code == 410
+                and response.json().get("detail") == "unexpected servo_uid"
+            ):
+                self.logger.warning(
+                    f"servo UID {self.config.servo_uid} is no longer valid. Waiting for deprovisioning (will sleep for 1 hour)"
+                )
+                await asyncio.sleep(3600)
+
             success = response.status_code == httpx.codes.OK
             return [
                 servo.checks.Check(
                     name="Opsani API connectivity",
                     success=success,
                     message=f"Response status code: {response.status_code}",
                 )
```

### Comparing `servox-2.2.5/servo/telemetry.py` & `servox-2.2.6/servo/telemetry.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/types/__init__.py` & `servox-2.2.6/servo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/types/api.py` & `servox-2.2.6/servo/types/api.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/types/core.py` & `servox-2.2.6/servo/types/core.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/types/kubernetes.py` & `servox-2.2.6/servo/types/kubernetes.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/types/settings.py` & `servox-2.2.6/servo/types/settings.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/types/slo.py` & `servox-2.2.6/servo/types/slo.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/__init__.py` & `servox-2.2.6/servo/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/associations.py` & `servox-2.2.6/servo/utilities/associations.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/duration_str.py` & `servox-2.2.6/servo/utilities/duration_str.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/hashing.py` & `servox-2.2.6/servo/utilities/hashing.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/inspect.py` & `servox-2.2.6/servo/utilities/inspect.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/key_paths.py` & `servox-2.2.6/servo/utilities/key_paths.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/pydantic.py` & `servox-2.2.6/servo/utilities/pydantic.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/strings.py` & `servox-2.2.6/servo/utilities/strings.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/subprocess.py` & `servox-2.2.6/servo/utilities/subprocess.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/servo/utilities/yaml.py` & `servox-2.2.6/servo/utilities/yaml.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.5/PKG-INFO` & `servox-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servox
-Version: 2.2.5
+Version: 2.2.6
 Summary: Opsani Servo: The Next Generation
 Home-page: https://opsani.com/
 License: Apache-2.0
 Author: Blake Watters
 Author-email: blake@opsani.com
 Requires-Python: >=3.8.1,<=3.9.11
 Classifier: License :: OSI Approved :: Apache Software License
```

