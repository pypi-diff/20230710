# Comparing `tmp/scalable-pypeline-1.2.1.tar.gz` & `tmp/scalable-pypeline-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalable-pypeline-1.2.1.tar", last modified: Mon Jul 10 14:46:16 2023, max compression
+gzip compressed data, was "scalable-pypeline-1.2.2.tar", last modified: Mon Jul 10 17:35:00 2023, max compression
```

## Comparing `scalable-pypeline-1.2.1.tar` & `scalable-pypeline-1.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4687 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4270 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.928554 scalable-pypeline-1.2.1/pypeline/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9038 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10759 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/celery_beat.py
--rw-rw-rw-   0 root         (0) root         (0)     4185 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/extensions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.929554 scalable-pypeline-1.2.1/pypeline/flask/
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.929554 scalable-pypeline-1.2.1/pypeline/flask/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8821 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/schedules.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5791 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/flask_sermos.py
--rw-rw-rw-   0 root         (0) root         (0)     6776 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     5503 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/logging_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.930554 scalable-pypeline-1.2.1/pypeline/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline/chained_task.py
--rw-rw-rw-   0 root         (0) root         (0)    11509 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7385 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/schedule_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    17336 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/sermos_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.931554 scalable-pypeline-1.2.1/pypeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13029 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/config_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/graph_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/module_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22222 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/task_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4687 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1076 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      590 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-10 14:46:16.933554 scalable-pypeline-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6461 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.925554 scalable-pypeline-1.2.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/tests/fixtures/s3_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.040820 scalable-pypeline-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-10 17:35:00.040820 scalable-pypeline-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.037820 scalable-pypeline-1.2.2/pypeline/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9038 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10759 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/celery_beat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4148 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/extensions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.037820 scalable-pypeline-1.2.2/pypeline/flask/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/flask/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.038820 scalable-pypeline-1.2.2/pypeline/flask/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/flask/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9026 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/flask/api/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/flask/api/schedules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/flask/api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/flask/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5791 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/flask/flask_sermos.py
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/logging_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.038820 scalable-pypeline-1.2.2/pypeline/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/pipeline/chained_task.py
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/pipeline/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8899 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/pipeline_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7385 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/schedule_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    17336 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/sermos_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.039820 scalable-pypeline-1.2.2/pypeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13029 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/utils/config_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/utils/graph_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/utils/module_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22222 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/pypeline/utils/task_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.040820 scalable-pypeline-1.2.2/scalable_pypeline.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-10 17:35:00.000000 scalable-pypeline-1.2.2/scalable_pypeline.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-10 17:35:00.000000 scalable-pypeline-1.2.2/scalable_pypeline.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 17:35:00.000000 scalable-pypeline-1.2.2/scalable_pypeline.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-10 17:35:00.000000 scalable-pypeline-1.2.2/scalable_pypeline.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-10 17:35:00.000000 scalable-pypeline-1.2.2/scalable_pypeline.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 17:35:00.000000 scalable-pypeline-1.2.2/scalable_pypeline.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-10 17:35:00.041820 scalable-pypeline-1.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.034820 scalable-pypeline-1.2.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 17:35:00.040820 scalable-pypeline-1.2.2/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-07-10 17:34:43.000000 scalable-pypeline-1.2.2/tests/fixtures/s3_fixtures.py
```

### Comparing `scalable-pypeline-1.2.1/LICENSE` & `scalable-pypeline-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/PKG-INFO` & `scalable-pypeline-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.2.1
+Version: 1.2.2
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.2.1/README.md` & `scalable-pypeline-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/celery.py` & `scalable-pypeline-1.2.2/pypeline/celery.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/celery_beat.py` & `scalable-pypeline-1.2.2/pypeline/celery_beat.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/constants.py` & `scalable-pypeline-1.2.2/pypeline/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 DEPLOYMENTS_URL = "{}deployments/{}"
 DEPLOYMENTS_DEPLOY_URL = "{}deployments/{}/deploy"
 DEPLOYMENTS_SERVICES_URL = "{}deployments/{}/services"
 DEPLOYMENTS_SERVICE_URL = "{}deployments/{}/services/{}"
 DEFAULT_AUTH_URL = urljoin(DEFAULT_BASE_URL, 'auth')
 USING_SERMOS_CLOUD = DEFAULT_BASE_URL != LOCAL_DEPLOYMENT_VALUE
 DEFAULT_CONFIG_RETRIEVAL_PAGE_SIZE = 25
-WORKFLOW_PROCESSOR_QUEUE = os.environ.get('WORKFLOW_PROCESSOR_QUEUE', 'default')
+WORKFLOW_PROCESSOR_DEFAULT_QUEUE = 'celery'
 
 # Default 'responses' dictionary when decorating endpoints with @api.doc()
 # Extend as necessary.
 API_DOC_RESPONSES = {
     200: {
         'code': 200,
         'description': 'Successful response.'
```

### Comparing `scalable-pypeline-1.2.1/pypeline/extensions.py` & `scalable-pypeline-1.2.2/pypeline/extensions.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/flask/__init__.py` & `scalable-pypeline-1.2.2/pypeline/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/flask/api/pipelines.py` & `scalable-pypeline-1.2.2/pypeline/flask/api/pipelines.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from celery.canvas import _chain
 from celery_dyrygent.workflows import Workflow
 from flask import jsonify, request, abort
 from flask_smorest import Blueprint
 from flask.views import MethodView
 from marshmallow import Schema, fields
 from marshmallow.exceptions import ValidationError
-from pypeline.constants import API_DOC_RESPONSES, API_DOC_PARAMS, API_PATH_V1,\
-    WORKFLOW_PROCESSOR_QUEUE
+from pypeline.constants import API_DOC_RESPONSES, API_DOC_PARAMS, API_PATH_V1, \
+    WORKFLOW_PROCESSOR_DEFAULT_QUEUE
 from pypeline.flask.decorators import require_accesskey
 from pypeline.flask.api.utils import chain_helper
 from pypeline.utils.task_utils import PipelineResult
 from pypeline.utils.config_utils import retrieve_latest_pipeline_config
 from pypeline.pipeline_config_schema import BasePipelineSchema, PipelineSchemaV1
 
 logger = logging.getLogger(__name__)
@@ -160,15 +160,19 @@
                                access_key=access_key,
                                chain_payload=payload)
 
             if gen.chain is None:
                 abort(400, message=gen.loading_message)
 
             chain: _chain = gen.chain
-            wf: Workflow = Workflow({"queue": WORKFLOW_PROCESSOR_QUEUE})
+            work_flow_processor_queue = (
+                pipeline_config["config"]["metadata"]
+                .get("processorQueue", None) or
+                WORKFLOW_PROCESSOR_DEFAULT_QUEUE)
+            wf: Workflow = Workflow({"queue":  work_flow_processor_queue})
             wf.add_celery_canvas(chain)
             wf.apply_async()
 
             celery_task_status = []
             for node in wf.nodes:
                 celery_task = dict(
                     name=wf.nodes[node].signature.name,
```

### Comparing `scalable-pypeline-1.2.1/pypeline/flask/api/schedules.py` & `scalable-pypeline-1.2.2/pypeline/flask/api/schedules.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/flask/api/utils.py` & `scalable-pypeline-1.2.2/pypeline/flask/api/utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/flask/decorators.py` & `scalable-pypeline-1.2.2/pypeline/flask/decorators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/flask/flask_sermos.py` & `scalable-pypeline-1.2.2/pypeline/flask/flask_sermos.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/generators.py` & `scalable-pypeline-1.2.2/pypeline/generators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/logging_config.py` & `scalable-pypeline-1.2.2/pypeline/logging_config.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/pipeline/chained_task.py` & `scalable-pypeline-1.2.2/pypeline/pipeline/chained_task.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/pipeline/generator.py` & `scalable-pypeline-1.2.2/pypeline/pipeline/generator.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/pipeline_config_schema.py` & `scalable-pypeline-1.2.2/pypeline/pipeline_config_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 
 class MetadataSchema(Schema):
     """ Schema for a pipeline's metadata object.
     """
     queue = fields.String(required=True,
                           description="Default queue for all pipeline tasks.",
                           example="default-queue-name")
-
+    processorQueue = fields.String(
+        required=True,
+        description="Default processor queue for all pipeline tasks.",
+        example="default-processor-queue-name",
+        default="celery"
+    )
     maxRetry = fields.Integer(
         required=False,
         description="A number. Maximum number of retries before giving up. "
                     "A value of None means task will retry forever. "
                     "By default, this option is set to 3.",
         default=3,
         example=3)
```

### Comparing `scalable-pypeline-1.2.1/pypeline/schedule_config_schema.py` & `scalable-pypeline-1.2.2/pypeline/schedule_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/sermos_yaml.py` & `scalable-pypeline-1.2.2/pypeline/sermos_yaml.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/utils/config_utils.py` & `scalable-pypeline-1.2.2/pypeline/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/utils/graph_utils.py` & `scalable-pypeline-1.2.2/pypeline/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/utils/module_utils.py` & `scalable-pypeline-1.2.2/pypeline/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/pypeline/utils/task_utils.py` & `scalable-pypeline-1.2.2/pypeline/utils/task_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/scalable_pypeline.egg-info/PKG-INFO` & `scalable-pypeline-1.2.2/scalable_pypeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.2.1
+Version: 1.2.2
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.2.1/scalable_pypeline.egg-info/SOURCES.txt` & `scalable-pypeline-1.2.2/scalable_pypeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/scalable_pypeline.egg-info/requires.txt` & `scalable-pypeline-1.2.2/scalable_pypeline.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/setup.py` & `scalable-pypeline-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.1/tests/fixtures/s3_fixtures.py` & `scalable-pypeline-1.2.2/tests/fixtures/s3_fixtures.py`

 * *Files identical despite different names*

