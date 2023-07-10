# Comparing `tmp/dequeai-0.808.tar.gz` & `tmp/dequeai-0.8088.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.808.tar", last modified: Mon Jul 10 20:54:17 2023, max compression
+gzip compressed data, was "dequeai-0.8088.tar", last modified: Mon Jul 10 20:58:29 2023, max compression
```

## Comparing `dequeai-0.808.tar` & `dequeai-0.8088.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:54:17.670463 dequeai-0.808/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-10 20:54:17.670463 dequeai-0.808/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:54:17.666463 dequeai-0.808/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.808/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.808/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.808/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.808/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.808/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    14889 2023-07-10 20:53:47.000000 dequeai-0.808/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.808/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.808/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.808/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.808/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.808/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:54:17.670463 dequeai-0.808/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-07-10 20:54:17.000000 dequeai-0.808/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 20:54:17.000000 dequeai-0.808/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:54:17.000000 dequeai-0.808/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 20:54:17.000000 dequeai-0.808/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 20:54:17.000000 dequeai-0.808/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 20:54:17.670463 dequeai-0.808/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      557 2023-07-10 20:54:03.000000 dequeai-0.808/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:58:29.555916 dequeai-0.8088/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-10 20:58:29.555916 dequeai-0.8088/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:58:29.555916 dequeai-0.8088/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8088/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.8088/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8088/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8088/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8088/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    14888 2023-07-10 20:58:04.000000 dequeai-0.8088/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8088/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8088/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8088/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8088/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8088/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 20:58:29.555916 dequeai-0.8088/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-10 20:58:29.000000 dequeai-0.8088/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 20:58:29.000000 dequeai-0.8088/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 20:58:29.000000 dequeai-0.8088/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 20:58:29.000000 dequeai-0.8088/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 20:58:29.000000 dequeai-0.8088/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 20:58:29.555916 dequeai-0.8088/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-10 20:58:16.000000 dequeai-0.8088/setup.py
```

### Comparing `dequeai-0.808/dequeai/datatypes.py` & `dequeai-0.8088/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.808/dequeai/dequeai.py` & `dequeai-0.8088/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.808/dequeai/dequeai_model.py` & `dequeai-0.8088/dequeai/dequeai_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
             raise Exception('Model should be an instance of a PyTorch nn.Module.')
 
         p2 = multiprocessing.Process(target=self._create_task, args=(model, model_card))
         p2.start()
 
     def _create_task(self, model, model_card):
 
-        file_name = f"{self._project_name}/.pt"
+        file_name = f"{self._project_name}.pt"
         try:
             import torch
         except ImportError:
             raise ImportError("PyTorch is required for creating model.")
 
         torch.save(model, file_name)
```

### Comparing `dequeai-0.808/dequeai/dequeai_run.py` & `dequeai-0.8088/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.808/dequeai/parsing_service.py` & `dequeai-0.8088/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.808/dequeai/rest_connect.py` & `dequeai-0.8088/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.808/dequeai/util.py` & `dequeai-0.8088/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.808/setup.py` & `dequeai-0.8088/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000808',
+    version='0.000008088',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

