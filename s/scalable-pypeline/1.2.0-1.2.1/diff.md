# Comparing `tmp/scalable-pypeline-1.2.0.tar.gz` & `tmp/scalable-pypeline-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalable-pypeline-1.2.0.tar", last modified: Wed Jul  5 20:20:02 2023, max compression
+gzip compressed data, was "scalable-pypeline-1.2.1.tar", last modified: Mon Jul 10 14:46:16 2023, max compression
```

## Comparing `scalable-pypeline-1.2.0.tar` & `scalable-pypeline-1.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4687 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4270 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.250991 scalable-pypeline-1.2.0/pypeline/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9038 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10759 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/celery_beat.py
--rw-rw-rw-   0 root         (0) root         (0)     4185 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/extensions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.251991 scalable-pypeline-1.2.0/pypeline/flask/
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.251991 scalable-pypeline-1.2.0/pypeline/flask/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8821 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/schedules.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5791 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/flask/flask_sermos.py
--rw-rw-rw-   0 root         (0) root         (0)     6776 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     5503 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/logging_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.251991 scalable-pypeline-1.2.0/pypeline/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2887 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline/chained_task.py
--rw-rw-rw-   0 root         (0) root         (0)    11509 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/pipeline_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7385 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/schedule_config_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    17336 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/sermos_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.252991 scalable-pypeline-1.2.0/pypeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13029 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/config_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/graph_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/module_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22222 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/pypeline/utils/task_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4687 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1076 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      590 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 20:20:02.000000 scalable-pypeline-1.2.0/scalable_pypeline.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-05 20:20:02.254991 scalable-pypeline-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6461 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.248991 scalable-pypeline-1.2.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 20:20:02.253991 scalable-pypeline-1.2.0/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2023-07-05 20:19:45.000000 scalable-pypeline-1.2.0/tests/fixtures/s3_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.928554 scalable-pypeline-1.2.1/pypeline/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9038 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10759 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/celery_beat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/extensions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.929554 scalable-pypeline-1.2.1/pypeline/flask/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.929554 scalable-pypeline-1.2.1/pypeline/flask/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8821 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/schedules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5791 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/flask/flask_sermos.py
+-rw-rw-rw-   0 root         (0) root         (0)     6776 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/logging_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.930554 scalable-pypeline-1.2.1/pypeline/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline/chained_task.py
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/pipeline_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     7385 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/schedule_config_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    17336 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/sermos_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.931554 scalable-pypeline-1.2.1/pypeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13029 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/config_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/graph_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/module_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22222 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/pypeline/utils/task_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-10 14:46:16.000000 scalable-pypeline-1.2.1/scalable_pypeline.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-10 14:46:16.933554 scalable-pypeline-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.925554 scalable-pypeline-1.2.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 14:46:16.932554 scalable-pypeline-1.2.1/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-07-10 14:45:58.000000 scalable-pypeline-1.2.1/tests/fixtures/s3_fixtures.py
```

### Comparing `scalable-pypeline-1.2.0/LICENSE` & `scalable-pypeline-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/PKG-INFO` & `scalable-pypeline-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.2.0
+Version: 1.2.1
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.2.0/README.md` & `scalable-pypeline-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/celery.py` & `scalable-pypeline-1.2.1/pypeline/celery.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/celery_beat.py` & `scalable-pypeline-1.2.1/pypeline/celery_beat.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/constants.py` & `scalable-pypeline-1.2.1/pypeline/constants.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/extensions.py` & `scalable-pypeline-1.2.1/pypeline/extensions.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/flask/__init__.py` & `scalable-pypeline-1.2.1/pypeline/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/flask/api/pipelines.py` & `scalable-pypeline-1.2.1/pypeline/flask/api/pipelines.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/flask/api/schedules.py` & `scalable-pypeline-1.2.1/pypeline/flask/api/schedules.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/flask/api/utils.py` & `scalable-pypeline-1.2.1/pypeline/flask/api/utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/flask/decorators.py` & `scalable-pypeline-1.2.1/pypeline/flask/decorators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/flask/flask_sermos.py` & `scalable-pypeline-1.2.1/pypeline/flask/flask_sermos.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/generators.py` & `scalable-pypeline-1.2.1/pypeline/generators.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/logging_config.py` & `scalable-pypeline-1.2.1/pypeline/logging_config.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/pipeline/chained_task.py` & `scalable-pypeline-1.2.1/pypeline/pipeline/chained_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         # pipelines.  It provides a patch in fix for celery's poor
         # implementation of Canvas work-flows
         if self.__name__ == 'workflow_processor':
             kwargs.pop('event', None)
         return super(ChainedTask, self).__call__(*args, **kwargs)
 
     def after_return(self, status, retval, task_id, args, kwargs, einfo):
-        if "event" in kwargs:
+        if "event" in kwargs and "pipeline_id" in kwargs["event"]:
             try:
                 pipeline_run_wrapper: PipelineRunWrapper = \
                     PipelineRunWrapper.from_event(kwargs["event"])
                 current_task_status = pipeline_run_wrapper.get_task_celery_status(task_id)
             except Exception:
                 logger.exception("Unable to retreive Pipeline Run Wrapper")
                 return
@@ -49,15 +49,15 @@
                 current_task_status["status"] = status
             try:
                 pipeline_run_wrapper.save_to_cache()
             except Exception:
                 logger.exception(f"Failed to update celery task status for task {task_id}")
 
     def on_retry(self, exc, task_id, args, kwargs, einfo):
-        if "event" in kwargs:
+        if "event" in kwargs and "pipeline_id" in kwargs["event"]:
             try:
                 pipeline_run_wrapper: PipelineRunWrapper = \
                     PipelineRunWrapper.from_event(kwargs["event"])
                 current_task_status = pipeline_run_wrapper.get_task_celery_status(task_id)
             except Exception:
                 logger.exception("Unable to retreive Pipeline Run Wrapper")
                 return
```

### Comparing `scalable-pypeline-1.2.0/pypeline/pipeline/generator.py` & `scalable-pypeline-1.2.1/pypeline/pipeline/generator.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/pipeline_config_schema.py` & `scalable-pypeline-1.2.1/pypeline/pipeline_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/schedule_config_schema.py` & `scalable-pypeline-1.2.1/pypeline/schedule_config_schema.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/sermos_yaml.py` & `scalable-pypeline-1.2.1/pypeline/sermos_yaml.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/utils/config_utils.py` & `scalable-pypeline-1.2.1/pypeline/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/utils/graph_utils.py` & `scalable-pypeline-1.2.1/pypeline/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/utils/module_utils.py` & `scalable-pypeline-1.2.1/pypeline/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/pypeline/utils/task_utils.py` & `scalable-pypeline-1.2.1/pypeline/utils/task_utils.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/scalable_pypeline.egg-info/PKG-INFO` & `scalable-pypeline-1.2.1/scalable_pypeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalable-pypeline
-Version: 1.2.0
+Version: 1.2.1
 Summary: PypeLine - Python pipelines for the Real World
 Home-page: https://gitlab.com/bravos2/pypeline
 Author: Bravos Power Corporation
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: flask
```

### Comparing `scalable-pypeline-1.2.0/scalable_pypeline.egg-info/SOURCES.txt` & `scalable-pypeline-1.2.1/scalable_pypeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/scalable_pypeline.egg-info/requires.txt` & `scalable-pypeline-1.2.1/scalable_pypeline.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/setup.py` & `scalable-pypeline-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `scalable-pypeline-1.2.0/tests/fixtures/s3_fixtures.py` & `scalable-pypeline-1.2.1/tests/fixtures/s3_fixtures.py`

 * *Files identical despite different names*

