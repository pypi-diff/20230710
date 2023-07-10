# Comparing `tmp/storey-1.4.3.tar.gz` & `tmp/storey-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-o0b9u66t/storey-1.4.3.tar", last modified: Mon Jun 19 05:31:15 2023, max compression
+gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-zb0_k6rx/storey-1.4.4.tar", last modified: Mon Jul 10 06:23:46 2023, max compression
```

## Comparing `storey-1.4.3.tar` & `storey-1.4.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 05:26:44.000000 storey-1.4.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 05:26:44.000000 storey-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 05:26:44.000000 storey-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-19 05:31:15.000000 storey-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-19 05:26:44.000000 storey-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 05:26:44.000000 storey-1.4.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-19 05:26:44.000000 storey-1.4.3/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-19 05:26:44.000000 storey-1.4.3/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-19 05:26:44.000000 storey-1.4.3/integration/integration_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_aggregation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_filesystems_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_flow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_kafka_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_redis_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-06-19 05:26:44.000000 storey-1.4.3/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-19 05:26:44.000000 storey-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 05:31:15.000000 storey-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-19 05:26:44.000000 storey-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-19 05:31:10.000000 storey-1.4.3/storey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-19 05:26:44.000000 storey-1.4.3/storey/aggregation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-06-19 05:26:44.000000 storey-1.4.3/storey/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-19 05:26:44.000000 storey-1.4.3/storey/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-06-19 05:26:44.000000 storey-1.4.3/storey/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-06-19 05:26:44.000000 storey-1.4.3/storey/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    50622 2023-06-19 05:26:44.000000 storey-1.4.3/storey/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-19 05:26:44.000000 storey-1.4.3/storey/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-06-19 05:26:44.000000 storey-1.4.3/storey/redis_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    37793 2023-06-19 05:26:44.000000 storey-1.4.3/storey/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-19 05:26:44.000000 storey-1.4.3/storey/sql_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-19 05:26:44.000000 storey-1.4.3/storey/steps/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-06-19 05:26:44.000000 storey-1.4.3/storey/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    50757 2023-06-19 05:26:44.000000 storey-1.4.3/storey/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-19 05:26:44.000000 storey-1.4.3/storey/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-19 05:26:44.000000 storey-1.4.3/storey/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-19 05:26:44.000000 storey-1.4.3/storey/windowed_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 05:31:15.000000 storey-1.4.3/storey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:31:15.000000 storey-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-19 05:26:44.000000 storey-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_aggregate_by_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_aggregate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   125163 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_v3io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-19 05:26:44.000000 storey-1.4.3/tests/test_windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 06:15:48.000000 storey-1.4.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 06:15:48.000000 storey-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 06:15:48.000000 storey-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-10 06:23:46.000000 storey-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-10 06:15:48.000000 storey-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 06:15:48.000000 storey-1.4.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-10 06:15:48.000000 storey-1.4.4/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-10 06:15:48.000000 storey-1.4.4/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-10 06:15:48.000000 storey-1.4.4/integration/integration_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_aggregation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_filesystems_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_flow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_kafka_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_redis_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-10 06:15:48.000000 storey-1.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 06:23:46.000000 storey-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-10 06:15:48.000000 storey-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-10 06:23:40.000000 storey-1.4.4/storey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-10 06:15:48.000000 storey-1.4.4/storey/aggregation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-07-10 06:15:48.000000 storey-1.4.4/storey/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-10 06:15:48.000000 storey-1.4.4/storey/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-07-10 06:15:48.000000 storey-1.4.4/storey/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-07-10 06:15:48.000000 storey-1.4.4/storey/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50622 2023-07-10 06:15:48.000000 storey-1.4.4/storey/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-10 06:15:48.000000 storey-1.4.4/storey/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-07-10 06:15:48.000000 storey-1.4.4/storey/redis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37793 2023-07-10 06:15:48.000000 storey-1.4.4/storey/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-10 06:15:48.000000 storey-1.4.4/storey/sql_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-07-10 06:15:48.000000 storey-1.4.4/storey/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51037 2023-07-10 06:15:48.000000 storey-1.4.4/storey/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-10 06:15:48.000000 storey-1.4.4/storey/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-10 06:15:48.000000 storey-1.4.4/storey/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-10 06:15:48.000000 storey-1.4.4/storey/windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-10 06:15:48.000000 storey-1.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_aggregate_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_aggregate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125240 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_v3io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_windowed_store.py
```

### Comparing `storey-1.4.3/LICENSE` & `storey-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/PKG-INFO` & `storey-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.3
+Version: 1.4.4
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.3/README.md` & `storey-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/__init__.py` & `storey-1.4.4/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/conftest.py` & `storey-1.4.4/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/integration_test_utils.py` & `storey-1.4.4/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/test_aggregation_integration.py` & `storey-1.4.4/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/test_azure_filesystem_integration.py` & `storey-1.4.4/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/test_filesystems_integration.py` & `storey-1.4.4/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/test_flow_integration.py` & `storey-1.4.4/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/test_kafka_integration.py` & `storey-1.4.4/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/test_redis_specific.py` & `storey-1.4.4/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/integration/test_s3_filesystem_integration.py` & `storey-1.4.4/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/setup.py` & `storey-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/__init__.py` & `storey-1.4.4/storey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.3"
+__version__ = "1.4.4"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.4.3/storey/aggregation_utils.py` & `storey-1.4.4/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/aggregations.py` & `storey-1.4.4/storey/aggregations.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/dataframe.py` & `storey-1.4.4/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/drivers.py` & `storey-1.4.4/storey/drivers.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/dtypes.py` & `storey-1.4.4/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/flow.py` & `storey-1.4.4/storey/flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/queue.py` & `storey-1.4.4/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/redis_driver.py` & `storey-1.4.4/storey/redis_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/sources.py` & `storey-1.4.4/storey/sources.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/sql_driver.py` & `storey-1.4.4/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/steps/__init__.py` & `storey-1.4.4/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/steps/assertion.py` & `storey-1.4.4/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/steps/flatten.py` & `storey-1.4.4/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/steps/foreach.py` & `storey-1.4.4/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/steps/partition.py` & `storey-1.4.4/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/steps/sample.py` & `storey-1.4.4/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/table.py` & `storey-1.4.4/storey/table.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/targets.py` & `storey-1.4.4/storey/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,24 @@
                 )
 
         self._time_field = time_field
         self._time_format = time_format
 
     _type_string_to_pyarrow_type = {
         "str": pyarrow.string(),
+        "int8": pyarrow.int8(),
+        "int16": pyarrow.int16(),
         "int32": pyarrow.int32(),
+        "int64": pyarrow.int64(),
+        "uint8": pyarrow.uint8(),
+        "uint16": pyarrow.uint16(),
+        "uint32": pyarrow.uint32(),
+        "uint64": pyarrow.uint64(),
         "int": pyarrow.int64(),
+        "float16": pyarrow.float16(),
         "float32": pyarrow.float32(),
         "float": pyarrow.float64(),
         "bool": pyarrow.bool_(),
         "datetime": pyarrow.timestamp("ns"),
     }
 
     def _init(self):
```

### Comparing `storey-1.4.3/storey/transformations/__init__.py` & `storey-1.4.4/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/utils.py` & `storey-1.4.4/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey/windowed_store.py` & `storey-1.4.4/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/storey.egg-info/PKG-INFO` & `storey-1.4.4/storey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.3
+Version: 1.4.4
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.3/storey.egg-info/SOURCES.txt` & `storey-1.4.4/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/tests/__init__.py` & `storey-1.4.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/tests/test_aggregate_by_key.py` & `storey-1.4.4/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/tests/test_aggregate_store.py` & `storey-1.4.4/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/tests/test_flow.py` & `storey-1.4.4/tests/test_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -2266,15 +2266,15 @@
     assert read_back_df.equals(expected_df)
 
 
 def test_write_to_parquet_string_as_datetime(tmpdir):
     out_dir = f"{tmpdir}/test_write_to_parquet_string_to_datetime/{uuid.uuid4().hex}/"
     columns = ["my_int", "my_string", "my_datetime"]
     columns_with_type = [
-        ("my_int", "int"),
+        ("my_int", "int8"),  # ML-4162
         ("my_string", "str"),
         ("my_datetime", "datetime"),
     ]
     controller = build_flow(
         [
             SyncEmitSource(),
             # set time_field="" to test for ML-3544 regression
@@ -2285,14 +2285,15 @@
     my_time = datetime(2020, 2, 15)
 
     expected = []
     for i in range(10):
         controller.emit([i, f"this is {i}", my_time.isoformat()])
         expected.append([i, f"this is {i}", my_time.isoformat(sep=" ")])
     expected_df = pd.DataFrame(expected, columns=columns)
+    expected_df["my_int"] = expected_df["my_int"].astype("int8")
     expected_df["my_datetime"] = expected_df["my_datetime"].astype("datetime64[us]")
     controller.terminate()
     controller.await_termination()
 
     read_back_df = pd.read_parquet(out_dir, columns=columns)
     read_back_df.sort_values("my_int", inplace=True)
     read_back_df.reset_index(drop=True, inplace=True)
```

### Comparing `storey-1.4.3/tests/test_steps.py` & `storey-1.4.4/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/tests/test_types.py` & `storey-1.4.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/tests/test_v3io.py` & `storey-1.4.4/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.3/tests/test_windowed_store.py` & `storey-1.4.4/tests/test_windowed_store.py`

 * *Files identical despite different names*

