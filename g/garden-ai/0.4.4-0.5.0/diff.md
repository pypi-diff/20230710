# Comparing `tmp/garden_ai-0.4.4.tar.gz` & `tmp/garden_ai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.4.4.tar", max compression
+gzip compressed data, was "garden_ai-0.5.0.tar", max compression
```

## Comparing `garden_ai-0.4.4.tar` & `garden_ai-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1078 2023-06-29 22:03:18.737883 garden_ai-0.4.4/LICENSE
--rw-r--r--   0        0        0      797 2023-06-29 22:03:18.741883 garden_ai-0.4.4/README.md
--rw-r--r--   0        0        0      418 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/__main__.py
--rw-r--r--   0        0        0       97 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/_version.py
--rw-r--r--   0        0        0        0 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/app/__init__.py
--rw-r--r--   0        0        0     2855 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/app/console.py
--rw-r--r--   0        0        0    11506 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/app/garden.py
--rw-r--r--   0        0        0      828 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/app/main.py
--rw-r--r--   0        0        0     3895 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/app/model.py
--rw-r--r--   0        0        0    11770 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0     3493 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/backend_client.py
--rw-r--r--   0        0        0    18030 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/client.py
--rw-r--r--   0        0        0      380 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/constants.py
--rw-r--r--   0        0        0     9394 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/datacite.py
--rw-r--r--   0        0        0        0 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/funcx_bandaid/__init__.py
--rw-r--r--   0        0        0     1247 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/funcx_bandaid/serialization_patch.py
--rw-r--r--   0        0        0    14824 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2802 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0     1603 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/globus_compute/login_manager.py
--rw-r--r--   0        0        0      801 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0        0 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/globus_search/__init__.py
--rw-r--r--   0        0        0     1362 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/globus_search/garden_search.py
--rw-r--r--   0        0        0     7553 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/local_data.py
--rw-r--r--   0        0        0    12544 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/mlmodel.py
--rw-r--r--   0        0        0        0 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/model_file_transfer/__init__.py
--rw-r--r--   0        0        0     1379 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/model_file_transfer/upload.py
--rw-r--r--   0        0        0    19490 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/pipelines.py
--rw-r--r--   0        0        0    10610 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/steps.py
--rw-r--r--   0        0        0     2019 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0    11186 2023-06-29 22:03:18.741883 garden_ai-0.4.4/garden_ai/utils/misc.py
--rw-r--r--   0        0        0     2865 2023-06-29 22:03:31.153944 garden_ai-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 garden_ai-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-10 15:08:02.876141 garden_ai-0.5.0/LICENSE
+-rw-r--r--   0        0        0      797 2023-07-10 15:08:02.876141 garden_ai-0.5.0/README.md
+-rw-r--r--   0        0        0      418 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/__main__.py
+-rw-r--r--   0        0        0     4454 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/_model.py
+-rw-r--r--   0        0        0      180 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/app/console.py
+-rw-r--r--   0        0        0    11506 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/app/main.py
+-rw-r--r--   0        0        0     3895 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/app/model.py
+-rw-r--r--   0        0        0    11770 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0     3493 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/backend_client.py
+-rw-r--r--   0        0        0    18096 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/client.py
+-rw-r--r--   0        0        0      440 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/constants.py
+-rw-r--r--   0        0        0     9394 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/datacite.py
+-rw-r--r--   0        0        0    14824 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2802 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0     1603 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/globus_compute/login_manager.py
+-rw-r--r--   0        0        0      798 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7553 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/local_data.py
+-rw-r--r--   0        0        0     8126 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/model_file_transfer/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/model_file_transfer/upload.py
+-rw-r--r--   0        0        0    19626 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    10745 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/steps.py
+-rw-r--r--   0        0        0     2019 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     5116 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/utils/_meta.py
+-rw-r--r--   0        0        0     1018 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0     8533 2023-07-10 15:08:02.880141 garden_ai-0.5.0/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2866 2023-07-10 15:08:15.864482 garden_ai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 garden_ai-0.5.0/PKG-INFO
```

### Comparing `garden_ai-0.4.4/LICENSE` & `garden_ai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/README.md` & `garden_ai-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/app/console.py` & `garden_ai-0.5.0/garden_ai/app/console.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/app/garden.py` & `garden_ai-0.5.0/garden_ai/app/garden.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/app/main.py` & `garden_ai-0.5.0/garden_ai/app/main.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/app/model.py` & `garden_ai-0.5.0/garden_ai/app/model.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/app/pipeline.py` & `garden_ai-0.5.0/garden_ai/app/pipeline.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/backend_client.py` & `garden_ai-0.5.0/garden_ai/backend_client.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/client.py` & `garden_ai-0.5.0/garden_ai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,46 +5,45 @@
 import time
 from pathlib import Path
 from typing import List, Optional, Union
 from uuid import UUID
 
 import typer
 from globus_compute_sdk import Client
+from globus_compute_sdk.serialize.concretes import DillCode
 from globus_sdk import (
     AuthAPIError,
     AuthClient,
+    ClientCredentialsAuthorizer,
+    ConfidentialAppAuthClient,
     GroupsClient,
     NativeAppAuthClient,
     RefreshTokenAuthorizer,
     SearchClient,
-    ClientCredentialsAuthorizer,
-    ConfidentialAppAuthClient,
 )
 from globus_sdk.scopes import AuthScopes, ScopeBuilder, SearchScopes
 from globus_sdk.tokenstorage import SimpleJSONFileAdapter
 from rich import print
 from rich.prompt import Prompt
 
-import garden_ai.funcx_bandaid.serialization_patch  # type: ignore # noqa: F401
-from garden_ai import local_data, GardenConstants
+from garden_ai import GardenConstants, local_data
+from garden_ai.backend_client import BackendClient
 from garden_ai.gardens import Garden
 from garden_ai.globus_compute.containers import build_container
 from garden_ai.globus_compute.login_manager import ComputeLoginManager
 from garden_ai.globus_compute.remote_functions import register_pipeline
 from garden_ai.globus_search import garden_search
-from garden_ai.backend_client import BackendClient
-from garden_ai.model_file_transfer.upload import upload_mlmodel_to_s3
-
 from garden_ai.local_data import GardenNotFoundException, PipelineNotFoundException
 from garden_ai.mlmodel import (
     LocalModel,
     ModelMetadata,
-    stage_model_for_upload,
     clear_mlflow_staging_directory,
+    stage_model_for_upload,
 )
+from garden_ai.model_file_transfer.upload import upload_mlmodel_to_s3
 from garden_ai.pipelines import Pipeline, RegisteredPipeline
 from garden_ai.utils.misc import extract_email_from_globus_jwt
 
 GARDEN_ENDPOINT = os.environ.get(
     "GARDEN_ENDPOINT",
     "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod",
 )
@@ -156,15 +155,19 @@
     def _make_compute_client(self):
         scope_to_authorizer = {
             AuthScopes.openid: self.openid_authorizer,
             SearchScopes.all: self.search_authorizer,
             Client.FUNCX_SCOPE: self.compute_authorizer,
         }
         compute_login_manager = ComputeLoginManager(scope_to_authorizer)
-        return Client(login_manager=compute_login_manager, do_version_check=False)
+        return Client(
+            login_manager=compute_login_manager,
+            do_version_check=False,
+            code_serialization_strategy=DillCode(),
+        )
 
     def _do_login_flow(self):
         self.auth_client.oauth2_start_flow(
             requested_scopes=[
                 AuthClient.scopes.openid,
                 AuthClient.scopes.email,
                 GroupsClient.scopes.view_my_groups_and_memberships,
```

### Comparing `garden_ai-0.4.4/garden_ai/datacite.py` & `garden_ai-0.5.0/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/gardens.py` & `garden_ai-0.5.0/garden_ai/gardens.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/globus_compute/containers.py` & `garden_ai-0.5.0/garden_ai/globus_compute/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/globus_compute/login_manager.py` & `garden_ai-0.5.0/garden_ai/globus_compute/login_manager.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.5.0/garden_ai/globus_compute/remote_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from globus_compute_sdk import Client  # type: ignore
 from globus_sdk import GlobusAPIError
 
 from garden_ai.pipelines import Pipeline
-from garden_ai.utils.misc import inject_env_kwarg
+from garden_ai.utils._meta import make_func_to_serialize
 
 
 class PipelineRegistrationException(Exception):
     """Exception raised when a container build request fails"""
 
     pass
 
 
 def register_pipeline(
     compute_client: Client,
     pipeline: Pipeline,
     container_uuid: str,
 ) -> str:
     try:
-        to_register = inject_env_kwarg(pipeline._composed_steps)
+        to_register = make_func_to_serialize(pipeline)
         func_uuid = compute_client.register_function(
             to_register, container_uuid=container_uuid, public=True
         )
     except GlobusAPIError as e:
         raise PipelineRegistrationException(
             "Could not register pipeline on Globus Compute"
         ) from e
```

### Comparing `garden_ai-0.4.4/garden_ai/globus_search/garden_search.py` & `garden_ai-0.5.0/garden_ai/globus_search/garden_search.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/local_data.py` & `garden_ai-0.5.0/garden_ai/local_data.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/model_file_transfer/upload.py` & `garden_ai-0.5.0/garden_ai/model_file_transfer/upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
+import os
 import shutil
 
 import requests
 
+from garden_ai.backend_client import BackendClient, PresignedUrlResponse
 from garden_ai.mlmodel import LocalModel
-from garden_ai.backend_client import (
-    BackendClient,
-    PresignedUrlResponse,
-)
 
 
 def upload_mlmodel_to_s3(
     local_directory: str, local_model: LocalModel, backend_client: BackendClient
 ):
     # Get url from Garden API
     presigned_url_response = backend_client.get_model_upload_url(local_model.full_name)
@@ -26,20 +24,22 @@
     Parameters
     ----------
     local_directory : str
         The local directory to upload.
     presigned_url: PresignedUrlResponse
         The url and fields needed to upload, generated by the backend
     """
-    zip_filepath = shutil.make_archive("model.zip", "zip", local_directory)
-
-    with open(zip_filepath, "rb") as f:
-        files = {"file": ("model.zip", f)}
-        http_response = requests.post(
-            presigned_url.url, data=presigned_url.fields, files=files
-        )
+    zip_filepath = shutil.make_archive("model", "zip", local_directory)
+    try:
+        with open(zip_filepath, "rb") as f:
+            files = {"file": ("model.zip", f)}
+            http_response = requests.post(
+                presigned_url.url, data=presigned_url.fields, files=files
+            )
+    finally:
+        os.remove(zip_filepath)
 
     # If successful, returns HTTP status code 204
     if http_response.status_code != 204:
         raise Exception(
             f"Failed to upload model directory {local_directory} to Garden. {http_response.text}"
         )
```

### Comparing `garden_ai-0.4.4/garden_ai/pipelines.py` & `garden_ai-0.5.0/garden_ai/pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-import os
 import json
 import logging
+import os
 import pathlib
 import sys
 from datetime import datetime
 from functools import reduce
 from inspect import signature
 from keyword import iskeyword
 from typing import Any, Dict, List, Optional, Tuple, Union
@@ -15,15 +15,14 @@
 import dparse  # type: ignore
 import globus_compute_sdk  # type: ignore
 from packaging.requirements import InvalidRequirement, Requirement
 from pydantic import BaseModel, Field, PrivateAttr, root_validator, validator
 from pydantic.dataclasses import dataclass
 
 import garden_ai
-from garden_ai._version import __version__
 from garden_ai.app.console import console
 from garden_ai.constants import GardenConstants
 from garden_ai.datacite import (
     Contributor,
     Creator,
     DataciteSchema,
     Description,
@@ -109,15 +108,15 @@
     func_uuid: Optional[UUID] = Field(None)
     description: Optional[str] = Field(None)
     version: Optional[str] = "0.0.1"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     tags: List[str] = Field(default_factory=list, unique_items=True)
     requirements_file: Optional[str] = Field(None)
     python_version: Optional[str] = Field(None)
-    pip_dependencies: List[str] = Field(default=[f"garden-ai=={__version__}"])
+    pip_dependencies: List[str] = Field(default_factory=list)
     conda_dependencies: List[str] = Field(default_factory=list)
     model_full_names: List[str] = Field(default_factory=list)
     short_name: Optional[str] = Field(None)
 
     def _composed_steps(*args, **kwargs):
         """ "This method intentionally left blank"
 
@@ -191,14 +190,24 @@
     def pip_deps_parsable(cls, pip_dep):
         try:
             _ = Requirement(pip_dep)
         except InvalidRequirement as e:
             raise ValueError(f"Could not parse pip dependency '{pip_dep}'") from e
         return pip_dep
 
+    @validator("pip_dependencies", each_item=False)
+    def ensure_minimal_dependencies(cls, pip_deps):
+        import mlflow  # type: ignore
+
+        if not any(req.startswith("mlflow") for req in pip_deps):
+            pip_deps += [f"mlflow-skinny=={mlflow.__version__}"]
+        if not any(req.startswith("pandas") for req in pip_deps):
+            pip_deps += ["pandas<3"]
+        return pip_deps
+
     def _collect_requirements(self):
         """collect requirements to pass to Globus Compute container service.
 
         Populates attributes `self.python_version, self.pip_dependencies, self.conda_dependencies` per
         `self.requirements_file`, as well as `self.model_full_names` from steps' metadata.
         """
         # collect explicit pipeline dependencies for the container
@@ -382,41 +391,35 @@
 
     def __call__(
         self,
         *args: Any,
         endpoint: Union[UUID, str] = None,
         **kwargs: Any,
     ) -> Any:
-        """Remotely execute this ``RegisteredPipeline``'s function from the function uuid. An endpoint must be specified.
+        """Remotely execute this ``RegisteredPipeline``'s function from the function uuid.
 
         Args:
             *args (Any):
                 Input data passed through the first step in the pipeline
             endpoint (UUID | str | None):
                 Where to run the pipeline. Must be a valid Globus Compute endpoint UUID.
+                If no endpoint is specified, the DLHub default compute endpoint is used.
             **kwargs (Any):
                 Additional keyword arguments passed directly to the first step in the pipeline.
 
         Returns:
             Results from the pipeline's composed steps called with the given input data.
 
-        Raises:
-            ValueError:
-                If no endpoint is specified
-            Exception:
-                Any exceptions raised over the course of executing the pipeline
 
         """
         if not endpoint:
-            raise ValueError(
-                "A Globus Compute endpoint uuid must be specified to execute remotely."
-            )
+            endpoint = GardenConstants.DLHUB_ENDPOINT
 
         if self._env_vars:
-            # see: utils.misc.inject_env_kwarg
+            # see: utils._meta.inject_env_kwarg
             kwargs = dict(kwargs)
             kwargs["_env_vars"] = self._env_vars
 
         with globus_compute_sdk.Executor(endpoint_id=str(endpoint)) as gce:
             # TODO: refactor below once the remote-calling interface is settled.
             # console/spinner is good ux but shouldn't live this deep in the
             # sdk.
```

### Comparing `garden_ai-0.4.4/garden_ai/steps.py` & `garden_ai-0.5.0/garden_ai/steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from inspect import Parameter, Signature, signature
 from typing import Any, Callable, Dict, List, Optional
 
 from pydantic import Field, validator
 from pydantic.dataclasses import dataclass
 from typing_extensions import get_type_hints
 
-from garden_ai.mlmodel import _Model
 from garden_ai.utils.misc import JSON, garden_json_encoder
 
 logger = logging.getLogger()
 
 
 class DataclassConfig:
     # pydantic dataclasses read their config via decorator argument, not as
@@ -120,14 +119,20 @@
 
     def _track_models(self):
         """
         If this step's function has a Model as a default argument, like
         ``func(*args, model=Model(...))``, record the model name
         """
 
+        # if `_Model` was never defined in main, there must not be any
+        try:
+            from __main__ import _Model
+        except ImportError:
+            return
+
         sig = signature(self.func)
         for param in sig.parameters.values():
             if isinstance(param.default, _Model):
                 model = param.default
                 self.model_full_names += [model.full_name]
         return
```

### Comparing `garden_ai-0.4.4/garden_ai/templates/pipeline` & `garden_ai-0.5.0/garden_ai/templates/pipeline`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.4/garden_ai/utils/misc.py` & `garden_ai-0.5.0/garden_ai/utils/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,37 @@
 import base64
 import json
 import logging
 import re
 import sys
-from functools import wraps
 from inspect import Parameter, Signature, signature
-from itertools import zip_longest
 from keyword import iskeyword
 from typing import Callable, List, Optional, Tuple
 
 import beartype.door
 import requests
 import yaml
 from packaging.requirements import InvalidRequirement, Requirement
-from typing_extensions import TypeAlias
-
-if sys.version_info < (3, 9):
-    from typing_extensions import get_args, get_origin
-else:
-    from beartype.typing import get_args, get_origin
-
 from pydantic.json import pydantic_encoder
+from typing_extensions import TypeAlias
 
 JSON: TypeAlias = str
 
 logger = logging.getLogger()
 issubtype = beartype.door.is_subhint
 
 
-# for contrast: unsafe_compose = lambda f,g: lambda *args,**kwargs: f(g(*args, **kwargs))
-def safe_compose(f, g):
+def safe_compose(f: Callable, g: Callable):
     """Helper: compose function `f` with function `g`, provided their annotations indicate compatibility.
-
     Arguments with defaults are ignored.
 
-    This is smart enough to figure out whether `g`'s result is meant as an
-    `*args` tuple for `f`, or if it's meant as a plain return value (which might
-    still be a tuple). Complains with an exception if the signatures don't match.
-
-
     Parameters
     ----------
     f : Callable
-        `f` is any callable which:
-            1. Has complete argument and return type annotations (steps are validated for this).
-            2. accepts 1 or more positional arguments, corresponding to `g`'s return type.
-            3. If `g` returns a tuple, `f` should either accept the
-                unpacked *elements* of the tuple as a list of arguments;
-                else `f` should accept a tuple itself.
-
     g : Callable
-        like `f`, `g` can be any callable which:
-            1. Has complete argument and return type annotations.
-            2. When `f` expects a single argument, returns a single python
-                object of the appropriate type.
-            3. When `f` expects multiple arguments, returns a tuple with
-                appropriately-typed elements.
 
     Raises
     ------
     TypeError
         If the annotations for `f`'s argument types and `g`'s return
         type are not equivalent.
     """
@@ -68,66 +40,48 @@
     g_sig: Signature = signature(g)
 
     f_in = tuple(
         p.annotation for p in f_sig.parameters.values() if p.default is Parameter.empty
     )
     g_out = g_sig.return_annotation
 
-    if get_origin(g_out) is tuple and len(f_in) > 1:
-        # case 1: g returns a tuple which, *if unpacked*, may align with f's annotations
-        # for example:
-        # g defined like `def g(...) -> tuple[A, B, C]: ...`, and
-        # f defined like `def f(a: A, b: B, c: C) -> ...`
-        g_returns: tuple = get_args(g_out)
-        if all(
-            issubtype(output_type, input_type)
-            for (output_type, input_type) in zip_longest(g_returns, f_in)
-        ):
-            # note that we unpack g's output
-            def f_of_g(*args, **kwargs):
-                return f(*g(*args, **kwargs))
-
-        else:
-            raise TypeError(
-                (
-                    f"Could not compose step {f.__name__} with step {g.__name__} "
-                    "due to return type signature mismatch: "
-                    f"expected tuple[{f_in}], got {g_out}."
-                )
-            )
-    elif len(f_in) == 1:
-        # case 2: return is a single value; verify that it's the only one
-        # expected by f.
+    if len(f_in) == 1:
         if issubtype(g_out, f_in[0]):
             # note that we do NOT unpack g's output
             def f_of_g(*args, **kwargs):
                 return f(g(*args, **kwargs))
 
         else:
             raise TypeError(
                 (
                     f"Could not compose step {f.__name__} with step {g.__name__} "
-                    "due to return type signature mismatch: "
-                    f"expected {f_in[0]}, got {g_out}."
+                    "due to return type signature mismatch: expected "
+                    f"{f_in[0]}, got {g_out}."
                 )
             )
+    elif len(f_in) > 1:
+        raise TypeError(
+            (
+                f"Could not compose step {f.__name__} with step {g.__name__} "
+                f"{f.__name__} has more than 1 positional (required) argument, "
+                "but only 1 would be given."
+            )
+        )
     else:
-        # case 3: signatures are neither single types nor equivalent tuples
         raise TypeError(
             (
-                f"Could not compose {f.__name__} with step {g.__name__} due to"
-                "return type signature mismatch. Please double-check that its"
-                "return matches the argument expected by the subsequent step."
+                f"Could not compose {f.__name__} with step {g.__name__}. "
+                f"{f.__name__} takes 0 positional arguments, but would be called "
+                f"on {g.__name__}'s return value."
             )
         )
-
     # give the returned function a new signature, corresponding
     # to g's input types and f's return type
-    f_of_g.__signature__ = Signature(
-        parameters=g_sig.parameters.values(),
+    f_of_g.__signature__ = Signature(  # type: ignore
+        parameters=list(g_sig.parameters.values()),
         return_annotation=f_sig.return_annotation,
     )
     f_of_g.__name__ = f.__name__ + "_COMPOSED_WITH_" + g.__name__
     return f_of_g
 
 
 def garden_json_encoder(obj):
@@ -258,34 +212,14 @@
         except InvalidRequirement:
             logger.warning(f"Could not parse requirement line: {line}")
             raise
 
     return [str(r) for r in requirements]
 
 
-def inject_env_kwarg(func: Callable):
-    """
-    Helper: modify a function so that it will accept an ``_env_vars`` keyword argument.
-
-    This can be used to dynamically set environment variables before executing the
-    original function, particularly useful if the function is executing remotely.
-    """
-
-    @wraps(func)
-    def inner(*args, _env_vars=None, **kwargs):
-        if _env_vars:
-            import os
-
-            for k, v in _env_vars.items():
-                os.environ[k] = v
-        return func(*args, **kwargs)
-
-    return inner
-
-
 def clean_identifier(name: str) -> str:
     """Clean the name provided for use as a pipeline's python identifier."""
     orig = name
     # Remove invalid characters, replacing with _
     name = re.sub("[^0-9a-zA-Z_]", "_", name)
 
     # Remove leading characters until we find a letter
```

### Comparing `garden_ai-0.4.4/pyproject.toml` & `garden_ai-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "garden-ai"
-version = "0.4.4" # placeholder
+version = "0.5.0" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
 # note to contributors: feel free to add yourselves to this list 🌱
 maintainers = [
   "Globus Labs <labs@globus.org>",
   "Owen Price Skelly",
   "Will Engler",
   "Ben Blaiszik",
@@ -38,15 +38,15 @@
 # numba is an indirect dep of ML Flow.
 # Specifying a recent version of it helps avoid install issues on M1 Macs
 numba = "^0.56"
 boto3 = "^1.26.77"
 dparse = { extras = ["conda"], version = "^0.6.2" }
 pyyaml = "^6.0"
 packaging = "^23.0"
-globus-compute-sdk = "2.1.0"
+globus-compute-sdk = "^2.2.0"
 # Be sure to add additional flavors as optional below as support is added and update tool.poetry.extras
 torch = { version = "^2.0.0", optional = true }
 tensorflow = { version = "^2.11.0", optional = true, python = ">=3.8,<3.12" }
 
 [tool.poetry.scripts]
 garden-ai = "garden_ai.app.main:app"
```

### Comparing `garden_ai-0.4.4/PKG-INFO` & `garden_ai-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.4.4
+Version: 0.5.0
 Summary: Garden: tools to simplify access to scientific AI advances.
 Home-page: https://thegardens.ai
 License: MIT
 Author: Garden Team
 Author-email: labs@globus.org
 Maintainer: Globus Labs
 Maintainer-email: labs@globus.org
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: tensorflow
 Provides-Extra: torch
 Requires-Dist: beartype (>=0.12.0,<0.13.0)
 Requires-Dist: boto3 (>=1.26.77,<2.0.0)
 Requires-Dist: dparse[conda] (>=0.6.2,<0.7.0)
-Requires-Dist: globus-compute-sdk (==2.1.0)
+Requires-Dist: globus-compute-sdk (>=2.2.0,<3.0.0)
 Requires-Dist: globus-sdk (>=3.12.0,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mlflow (>=2.3.2,<3.0.0)
 Requires-Dist: numba (>=0.56,<0.57)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
```

