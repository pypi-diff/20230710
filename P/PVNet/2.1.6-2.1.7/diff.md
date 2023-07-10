# Comparing `tmp/PVNet-2.1.6.tar.gz` & `tmp/PVNet-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-2.1.6.tar", last modified: Fri Jul  7 15:39:04 2023, max compression
+gzip compressed data, was "PVNet-2.1.7.tar", last modified: Mon Jul 10 07:46:51 2023, max compression
```

## Comparing `PVNet-2.1.6.tar` & `PVNet-2.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:39:04.450158 PVNet-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 15:38:52.000000 PVNet-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 15:38:52.000000 PVNet-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-07 15:39:04.450158 PVNet-2.1.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:39:04.450158 PVNet-2.1.6/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-07 15:39:04.000000 PVNet-2.1.6/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 15:39:04.000000 PVNet-2.1.6/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:39:04.000000 PVNet-2.1.6/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-07 15:39:04.000000 PVNet-2.1.6/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 15:39:04.000000 PVNet-2.1.6/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-07 15:38:52.000000 PVNet-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:39:04.450158 PVNet-2.1.6/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 15:38:52.000000 PVNet-2.1.6/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-07 15:38:52.000000 PVNet-2.1.6/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-07 15:38:52.000000 PVNet-2.1.6/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-07 15:38:52.000000 PVNet-2.1.6/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-07 15:38:52.000000 PVNet-2.1.6/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-07 15:38:52.000000 PVNet-2.1.6/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-07 15:38:52.000000 PVNet-2.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 15:38:52.000000 PVNet-2.1.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-07 15:38:52.000000 PVNet-2.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:39:04.450158 PVNet-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-07 15:38:52.000000 PVNet-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:39:04.450158 PVNet-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:38:52.000000 PVNet-2.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-07 15:38:52.000000 PVNet-2.1.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-07 15:38:52.000000 PVNet-2.1.6/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-10 07:46:41.000000 PVNet-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 07:46:41.000000 PVNet-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 07:46:51.508591 PVNet-2.1.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 07:46:51.000000 PVNet-2.1.7/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-10 07:46:41.000000 PVNet-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-07-10 07:46:41.000000 PVNet-2.1.7/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-10 07:46:41.000000 PVNet-2.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-10 07:46:41.000000 PVNet-2.1.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-10 07:46:41.000000 PVNet-2.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:46:51.508591 PVNet-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-10 07:46:41.000000 PVNet-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:51.508591 PVNet-2.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:46:41.000000 PVNet-2.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-10 07:46:41.000000 PVNet-2.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-10 07:46:41.000000 PVNet-2.1.7/tests/test_app.py
```

### Comparing `PVNet-2.1.6/LICENSE` & `PVNet-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/PKG-INFO` & `PVNet-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.6
+Version: 2.1.7
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.6/PVNet.egg-info/PKG-INFO` & `PVNet-2.1.7/PVNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 2.1.6
+Version: 2.1.7
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-2.1.6/README.md` & `PVNet-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/pvnet/app.py` & `PVNet-2.1.7/pvnet/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,14 +235,20 @@
     gsp_id_to_loc = GSPLocationLookup(ds_gsp.x_osgb, ds_gsp.y_osgb)
 
     # Download satellite data - can't load zipped zarr straight from s3 bucket
     logger.info("Downloading zipped satellite data")
     fs = fsspec.open(os.environ["SATELLITE_ZARR_PATH"]).fs
     fs.get(os.environ["SATELLITE_ZARR_PATH"], "latest.zarr.zip")
 
+    # Also download 15-minute satellite if it exists
+    sat_latest_15 = os.environ["SATELLITE_ZARR_PATH"].replace(".zarr.zip", "_15.zarr.zip")
+    if fs.exists(sat_latest_15):
+        logger.info("Downloading 15-minute satellite data")
+        fs.get(sat_latest_15, "latest_15.zarr.zip")
+
     # ---------------------------------------------------------------------------
     # 2. Set up data loader
     logger.info("Creating DataLoader")
 
     # Location and time datapipes
     location_pipe = IterableWrapper([gsp_id_to_loc(gsp_id) for gsp_id in gsp_ids])
     t0_datapipe = IterableWrapper([t0]).repeat(len(location_pipe))
```

### Comparing `PVNet-2.1.6/pvnet/callbacks.py` & `PVNet-2.1.7/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/pvnet/optimizers.py` & `PVNet-2.1.7/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/pvnet/training.py` & `PVNet-2.1.7/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/pvnet/utils.py` & `PVNet-2.1.7/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/setup.py` & `PVNet-2.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/tests/conftest.py` & `PVNet-2.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-2.1.6/tests/test_app.py` & `PVNet-2.1.7/tests/test_app.py`

 * *Files identical despite different names*

