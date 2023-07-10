# Comparing `tmp/dbt-workflows-factory-0.1.0.tar.gz` & `tmp/dbt-workflows-factory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-workflows-factory-0.1.0.tar", last modified: Fri Jul  7 14:53:51 2023, max compression
+gzip compressed data, was "dbt-workflows-factory-0.2.0.tar", last modified: Mon Jul 10 07:26:16 2023, max compression
```

## Comparing `dbt-workflows-factory-0.1.0.tar` & `dbt-workflows-factory-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:53:51.642809 dbt-workflows-factory-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-07-07 14:53:51.642809 dbt-workflows-factory-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:53:51.642809 dbt-workflows-factory-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:53:51.642809 dbt-workflows-factory-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:53:51.642809 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/dbt_workflows_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-07 14:53:35.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/yaml_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:53:51.642809 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-07-07 14:53:51.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-07 14:53:51.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:53:51.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:53:51.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 14:53:51.000000 dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:26:16.733691 dbt-workflows-factory-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-07-10 07:26:16.733691 dbt-workflows-factory-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:26:16.733691 dbt-workflows-factory-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:26:16.733691 dbt-workflows-factory-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:26:16.733691 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/dbt_workflows_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-10 07:26:00.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/yaml_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:26:16.733691 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-07-10 07:26:16.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-10 07:26:16.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:26:16.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:26:16.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 07:26:16.000000 dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/top_level.txt
```

### Comparing `dbt-workflows-factory-0.1.0/LICENSE` & `dbt-workflows-factory-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-workflows-factory-0.1.0/PKG-INFO` & `dbt-workflows-factory-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-workflows-factory
-Version: 0.1.0
+Version: 0.2.0
 Summary: DBT workflows factory for Google Cloud Platform
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -235,15 +235,14 @@
 ### How to run
 
 To call from cli, you can
 
 ```bash
 python -m dbt_workflows_factory.cli convert \
     --image-uri my-image-uri \
-    --region europe-west6 \
     --gcs-key-volume-remote-path google-cloud-storage/path/ \
     --gcs-key-volume-mount-path /etc/gcs-key/ \
     --gcs-key-volume-container-mount-path /etc/gcs-key/:/etc/gcs-key/:ro \
     --container-gcp-key-path /etc/gcs-key/path.json \
     --container-gcp-project-id some-project-id \
     --pretty \
     tests/unit/dbt_workflows_factory/test_data/manifest.json > workflow_source.json
```

### Comparing `dbt-workflows-factory-0.1.0/README.md` & `dbt-workflows-factory-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 ### How to run
 
 To call from cli, you can
 
 ```bash
 python -m dbt_workflows_factory.cli convert \
     --image-uri my-image-uri \
-    --region europe-west6 \
     --gcs-key-volume-remote-path google-cloud-storage/path/ \
     --gcs-key-volume-mount-path /etc/gcs-key/ \
     --gcs-key-volume-container-mount-path /etc/gcs-key/:/etc/gcs-key/:ro \
     --container-gcp-key-path /etc/gcs-key/path.json \
     --container-gcp-project-id some-project-id \
     --pretty \
     tests/unit/dbt_workflows_factory/test_data/manifest.json > workflow_source.json
```

### Comparing `dbt-workflows-factory-0.1.0/pyproject.toml` & `dbt-workflows-factory-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/cli.py` & `dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,30 @@
 def cli() -> None:
     """CLI entrypoint."""
 
 
 @cli.command()
 @click.argument("manifest_file", type=click.Path(exists=True))
 @click.option("--image-uri", type=str, help="Docker image URI", required=True)
-@click.option("--region", type=str, help="GCP region", required=True)
+@click.option(
+    "--location",
+    type=str,
+    help="GCP region",
+    required=False,
+    default='${sys.get_env("GOOGLE_CLOUD_LOCATION")}',
+    show_default=True,
+)
+@click.option(
+    "--project-id",
+    type=str,
+    help="GCP project ID",
+    required=False,
+    default='${sys.get_env("GOOGLE_CLOUD_PROJECT_ID")}',
+    show_default=True,
+)
 @click.option("--gcs-key-volume-remote-path", type=str, help="GCS Remote path for private key", required=True)
 @click.option(
     "--gcs-key-volume-mount-path",
     type=str,
     help="Volume mount path for private key",
     required=True,
 )
@@ -59,27 +74,29 @@
     required=False,
     default=False,
     is_flag=True,
 )
 def convert(
     manifest_file: str,
     image_uri: str,
-    region: str,
+    location: str,
+    project_id: str,
     gcs_key_volume_remote_path: str,
     gcs_key_volume_mount_path: str,
     gcs_key_volume_container_mount_path: str,
     container_gcp_key_path: str,
     container_gcp_project_id: str,
     job_id_suffix: str,
     pretty: bool,
 ) -> None:
     """Convert dbt manifest.json to YAML for GCP Workflows."""  # noqa: DCO020
     params = Params(
         image_uri=image_uri,
-        region=region,
+        location=location,
+        project_id=project_id,
         gcs_key_volume_remote_path=gcs_key_volume_remote_path,
         gcs_key_volume_mount_path=gcs_key_volume_mount_path,
         gcs_key_volume_container_mount_path=gcs_key_volume_container_mount_path,
         container_gcp_key_path=container_gcp_key_path,
         container_gcp_project_id=container_gcp_project_id,
         job_id_suffix=job_id_suffix,
     )
```

### Comparing `dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/dbt_workflows_converter.py` & `dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/dbt_workflows_converter.py`

 * *Files identical despite different names*

### Comparing `dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/tasks.py` & `dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import hashlib
 import re
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any
 
 from dbt_graph_builder.node_type import NodeType
 from dbt_graph_builder.workflow import ChainStep, ParallelStep, Step, StepFactory
@@ -52,17 +53,15 @@
             dict[str, Any]: Step result.
         """
         return {
             self.step_name: {
                 "call": "subworkflowBatchJob",
                 "args": {
                     "jobId": self.job_id,
-                    "batchApiUrl": "${batchApiUrl}",
                     "select": self.select,
-                    "imageUri": "${imageUri}",
                     "command": self.command.value,
                 },
                 "result": f"{self.step_name}_RESULT",
             }
         }
 
 
@@ -137,15 +136,16 @@
 
         Raises:
             NotImplementedError: Unsupported node type.
 
         Returns:
             SingleTask: SingleTask instance.
         """
-        job_id: str = self._job_id_replace_pattern.sub("-", node).lower()[0:45]
+        node_id: str = self._job_id_replace_pattern.sub("-", node).lower()[0:36]
+        job_id = f"{node_id}-{hashlib.sha256(node.encode('utf-8')).hexdigest()[0:8].lower()}"
         task_name: str = self._task_name_replace_pattern.sub("_", node)
 
         if node_definition["node_type"] == NodeType.RUN_TEST:
             run_task = NodeStep(f"{task_name}_run", node_definition["select"], DbtCommand.RUN, f"{job_id}-run")
             test_task = NodeStep(f"{task_name}_test", node_definition["select"], DbtCommand.TEST, f"{job_id}-test")
             return WorkflowChainStep(run_task, WorkflowChainStep(test_task))
```

### Comparing `dbt-workflows-factory-0.1.0/src/dbt_workflows_factory/yaml_builder.py` & `dbt-workflows-factory-0.2.0/src/dbt_workflows_factory/yaml_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Any
 
 from dbt_graph_builder.workflow import Step
 
 from .params import Params
-from .tasks import CustomStep, WorkflowChainStep
+from .tasks import WorkflowChainStep
 
 
 class MainChainTask(WorkflowChainStep):
     """Main chain task in workflow."""
 
     def __init__(self, step: Step, next_step: WorkflowChainStep | None = None) -> None:
         """Create a new main chain task.
@@ -41,85 +41,64 @@
 
         Args:
             additional_steps (Step): Additional steps to add to the workflow.
 
         Returns:
             dict[str, Any]: Workflow.
         """
-        maint_chain_task = MainChainTask(self._init_step())
-        maint_chain_task.add_step(additional_steps)
-        yaml_representation = maint_chain_task.get_step()
+        main_chain_task = MainChainTask(additional_steps)
+        yaml_representation = main_chain_task.get_step()
         yaml_representation["subworkflowBatchJob"] = self._subworkflow
         return yaml_representation
 
-    def _init_step(self) -> Step:
-        return CustomStep(
-            {
-                "init": {
-                    "assign": [
-                        {"projectId": '${sys.get_env("GOOGLE_CLOUD_PROJECT_ID")}'},
-                        {"region": self._params.region},
-                        {"batchApi": "batch.googleapis.com/v1"},
-                        {
-                            "batchApiUrl": (
-                                '${"https://" + batchApi + "/projects/" + projectId + "/locations/" + region + "/jobs"}'
-                            )
-                        },
-                        {"imageUri": self._params.image_uri},
-                    ]
-                }
-            }
-        )
-
     @property
     def _subworkflow(self) -> dict[str, Any]:
         return {
             "params": self._subworkflow_job_params,
             "steps": self._subworkflow_job_steps,
         }
 
     @property
     def _subworkflow_job_params(self) -> list[str]:
-        return ["batchApiUrl", "command", "jobId", "imageUri", "select"]
+        return ["jobId", "command", "select"]
 
     @property
     def _subworkflow_job_steps(self) -> list[dict[str, Any]]:
         return [
             self._subwork_init_job,
             self._subwork_main_job,
-            self._subwork_get_job,
         ]
 
     @property
     def _subwork_init_job(self) -> dict[str, Any]:
         return {
             "init": {
                 "assign": [
+                    {"location": self._params.location},
+                    {"projectId": self._params.project_id},
                     {"jobId": f'${{jobId + "-" + {self._params.job_id_suffix}}}'},
                 ]
             }
         }
 
     @property
     def _subwork_main_job(self) -> dict[str, Any]:
         return {
             "createAndRunBatchJob": {
-                "call": "http.post",
+                "call": "googleapis.batch.v1.projects.locations.jobs.create",
                 "args": self._subwork_job_args,
                 "result": "createAndRunBatchJobResponse",
             }
         }
 
     @property
     def _subwork_job_args(self) -> dict[str, Any]:
         return {
-            "url": "${batchApiUrl}",
-            "query": {"jobId": "${jobId}"},
-            "headers": {"Content-Type": "application/json"},
-            "auth": {"type": "OAuth2"},
+            "parent": '${"projects/" + projectId + "/locations/" + location}',
+            "jobId": "${jobId}",
             "body": {
                 "taskGroups": {
                     "taskSpec": {
                         "volumes": self._subwork_job_volumes,
                         "runnables": self._subwork_job_runnables,
                     }
                 },
@@ -137,15 +116,15 @@
         ]
 
     @property
     def _subwork_job_runnables(self) -> list[dict[str, Any]]:
         return [
             {
                 "container": {
-                    "imageUri": "${imageUri}",
+                    "imageUri": self._params.image_uri,
                     "entrypoint": "/bin/bash",
                     "commands": [
                         "-c",
                         '${"dbt --no-write-json " + command + " --target env_execution --project-dir /dbt '
                         '--profiles-dir /root/.dbt --select " + select}',
                     ],
                     "volumes": [self._params.gcs_key_volume_container_mount_path],
@@ -154,20 +133,7 @@
                     "variables": {
                         "GCP_KEY_PATH": self._params.container_gcp_key_path,
                         "GCP_PROJECT": self._params.container_gcp_project_id,
                     }
                 },
             }
         ]
-
-    @property
-    def _subwork_get_job(self) -> dict[str, Any]:
-        return {
-            "getJob": {
-                "call": "http.get",
-                "args": {
-                    "url": '${batchApiUrl + "/" + jobId}',
-                    "auth": {"type": "OAuth2"},
-                },
-                "result": "getJobResult",
-            }
-        }
```

### Comparing `dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/PKG-INFO` & `dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-workflows-factory
-Version: 0.1.0
+Version: 0.2.0
 Summary: DBT workflows factory for Google Cloud Platform
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -235,15 +235,14 @@
 ### How to run
 
 To call from cli, you can
 
 ```bash
 python -m dbt_workflows_factory.cli convert \
     --image-uri my-image-uri \
-    --region europe-west6 \
     --gcs-key-volume-remote-path google-cloud-storage/path/ \
     --gcs-key-volume-mount-path /etc/gcs-key/ \
     --gcs-key-volume-container-mount-path /etc/gcs-key/:/etc/gcs-key/:ro \
     --container-gcp-key-path /etc/gcs-key/path.json \
     --container-gcp-project-id some-project-id \
     --pretty \
     tests/unit/dbt_workflows_factory/test_data/manifest.json > workflow_source.json
```

### Comparing `dbt-workflows-factory-0.1.0/src/dbt_workflows_factory.egg-info/SOURCES.txt` & `dbt-workflows-factory-0.2.0/src/dbt_workflows_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

