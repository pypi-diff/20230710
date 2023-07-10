# Comparing `tmp/PVNet-2.1.7.tar.gz` & `tmp/PVNet-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-2.1.7.tar", last modified: Mon Jul 10 07:46:51 2023, max compression
+gzip compressed data, was "PVNet-2.1.8.tar", last modified: Mon Jul 10 10:20:34 2023, max compression
```

## Comparing `PVNet-2.1.7.tar` & `PVNet-2.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-10 07:46:41.000000 PVNet-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 07:46:41.000000 PVNet-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 07:46:51.508591 PVNet-2.1.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-10 07:46:41.000000 PVNet-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-10 07:46:41.000000 PVNet-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 07:46:41.000000 PVNet-2.1.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-10 07:46:41.000000 PVNet-2.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:46:51.508591 PVNet-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-10 07:46:41.000000 PVNet-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:41.000000 PVNet-2.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-10 07:46:41.000000 PVNet-2.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 07:46:41.000000 PVNet-2.1.7/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-10 10:20:24.000000 PVNet-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 10:20:24.000000 PVNet-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 10:20:34.405094 PVNet-2.1.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 10:20:34.000000 PVNet-2.1.8/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-10 10:20:24.000000 PVNet-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-10 10:20:24.000000 PVNet-2.1.8/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-10 10:20:24.000000 PVNet-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 10:20:24.000000 PVNet-2.1.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-10 10:20:24.000000 PVNet-2.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:20:34.405094 PVNet-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-10 10:20:24.000000 PVNet-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:34.405094 PVNet-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:20:24.000000 PVNet-2.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-10 10:20:24.000000 PVNet-2.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 10:20:24.000000 PVNet-2.1.8/tests/test_app.py
```

### Comparing `PVNet-2.1.7/LICENSE` & `PVNet-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/PKG-INFO` & `PVNet-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.7
+Version: 2.1.8
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.7/PVNet.egg-info/PKG-INFO` & `PVNet-2.1.8/PVNet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.7
+Version: 2.1.8
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.7/README.md` & `PVNet-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/pvnet/app.py` & `PVNet-2.1.8/pvnet/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,15 @@
     # Batch datapipe
     batch_datapipe = (
         construct_sliced_data_pipeline(
             config_filename=data_config_filename,
             location_pipe=location_pipe,
             t0_datapipe=t0_datapipe,
             production=True,
+            check_satellite_no_zeros=True,
         )
         .batch(batch_size)
         .map(stack_np_examples_into_batch)
     )
 
     # Set up dataloader for parallel loading
     rs = MultiProcessingReadingService(
```

### Comparing `PVNet-2.1.7/pvnet/callbacks.py` & `PVNet-2.1.8/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/pvnet/optimizers.py` & `PVNet-2.1.8/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/pvnet/training.py` & `PVNet-2.1.8/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/pvnet/utils.py` & `PVNet-2.1.8/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/setup.py` & `PVNet-2.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/tests/conftest.py` & `PVNet-2.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.7/tests/test_app.py` & `PVNet-2.1.8/tests/test_app.py`

 * *Files identical despite different names*

