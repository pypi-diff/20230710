# Comparing `tmp/databricks-feature-lookup-0.5.1.tar.gz` & `tmp/databricks-feature-lookup-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-feature-lookup-0.5.1.tar", last modified: Fri Jun  2 00:29:56 2023, max compression
+gzip compressed data, was "databricks-feature-lookup-0.6.0.tar", last modified: Mon Jul 10 20:06:26 2023, max compression
```

## Comparing `databricks-feature-lookup-0.5.1.tar` & `databricks-feature-lookup-0.6.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.701452 databricks-feature-lookup-0.5.1/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2414 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.5.1/LICENSE.md
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      426 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.5.1/NOTICE.md
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-06-02 00:29:56.701206 databricks-feature-lookup-0.5.1/PKG-INFO
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3488 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/README.md
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.678924 databricks-feature-lookup-0.5.1/databricks/
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.681159 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.681487 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.5.1/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.682835 databricks-feature-lookup-0.5.1/databricks/feature_store/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1980 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/__init__.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.689335 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1309 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_feature_store_object.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1489 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_proto_enum_entity.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      444 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/cloud.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3039 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      913 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/data_type.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2553 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3971 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_functions_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    19367 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      715 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec_constants.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1544 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_table_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4065 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_tables_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      673 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/function_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1978 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/on_demand_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6817 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_feature_table.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     5484 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_store_for_serving.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      489 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/query_mode.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      855 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/source_data_column_info.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      659 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/entities/store_type.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.689891 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     7556 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_executor.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2817 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_loader.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.690350 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1855 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/codegen_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      139 2023-06-02 00:01:27.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/feature_lookup_version.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.692380 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      753 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     8034 2023-05-31 17:19:14.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    21707 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      923 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2832 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     7533 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2130 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    32490 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2066 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model_constants.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10759 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/online_lookup_client.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.693372 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     6396 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_spec_pb2.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    21337 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_store_serving_pb2.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.699525 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/__init__.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3871 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/converter_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1736 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/cosmosdb_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      803 2023-05-31 17:19:14.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/cosmosdb_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      765 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/data_type_details_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1739 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4955 2023-06-02 00:01:27.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3117 2023-05-26 16:28:51.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_function_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      347 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_serving_patch.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2317 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_spec_test_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2631 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/metrics_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    11740 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/pandas_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     8049 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/serving_test_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1278 2023-01-13 00:15:59.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/sql_type_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      374 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/test_utils_common.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)    10305 2023-04-17 17:28:49.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/uc_utils.py
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     1539 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.5.1/databricks/feature_store/utils/utils_common.py
-drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-06-02 00:29:56.700920 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/PKG-INFO
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     3412 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/SOURCES.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/dependency_links.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)      107 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/requires.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       11 2023-06-02 00:29:56.000000 databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/top_level.txt
--rw-r--r--   0 mingyang.ge   (502) staff       (20)       38 2023-06-02 00:29:56.701519 databricks-feature-lookup-0.5.1/setup.cfg
--rw-r--r--   0 mingyang.ge   (502) staff       (20)     2724 2023-01-13 00:17:50.000000 databricks-feature-lookup-0.5.1/setup.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.683327 databricks-feature-lookup-0.6.0/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2414 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.6.0/LICENSE.md
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       30 2023-06-22 23:44:03.000000 databricks-feature-lookup-0.6.0/MANIFEST.in
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      426 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.6.0/NOTICE.md
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-07-10 20:06:26.683174 databricks-feature-lookup-0.6.0/PKG-INFO
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3488 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/README.md
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.662340 databricks-feature-lookup-0.6.0/databricks/
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.665285 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      166 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.665660 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-10-06 23:48:00.000000 databricks-feature-lookup-0.6.0/databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.667250 databricks-feature-lookup-0.6.0/databricks/feature_store/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1980 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/__init__.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.673682 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1309 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_feature_store_object.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1489 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_proto_enum_entity.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      444 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/cloud.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3524 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      913 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/data_type.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2553 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3971 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_functions_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    19863 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      739 2023-06-08 17:27:16.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec_constants.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1544 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_table_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4065 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_tables_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      673 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/function_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1978 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/on_demand_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6817 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/online_feature_table.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5966 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/online_store_for_serving.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      489 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/query_mode.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      855 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/source_data_column_info.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      659 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/entities/store_type.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.674193 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     7556 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_executor.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2817 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_loader.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.674659 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1855 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/codegen_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      139 2023-07-10 20:03:31.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/feature_lookup_version.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.676420 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      891 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1068 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_brickstore_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     8034 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    21707 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      923 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2832 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     7916 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2130 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    31382 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1766 2023-06-22 23:43:16.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model_constants.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    11426 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/online_lookup_client.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.677124 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2022-07-20 05:31:47.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     6433 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_spec_pb2.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    21337 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_store_serving_pb2.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.681719 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        0 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/__init__.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3871 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/converter_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1736 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      803 2023-05-31 17:19:14.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      765 2023-01-03 23:39:08.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/data_type_details_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1739 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     5030 2023-06-05 18:12:24.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3117 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_function_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2317 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_spec_test_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2631 2023-04-05 21:38:23.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/metrics_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    11740 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/pandas_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     8049 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/serving_test_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1278 2023-07-06 20:12:44.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/sql_type_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      374 2023-05-10 02:23:10.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/test_utils_common.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)    10313 2023-07-08 07:28:45.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/uc_utils.py
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     1539 2023-04-05 21:38:22.000000 databricks-feature-lookup-0.6.0/databricks/feature_store/utils/utils_common.py
+drwxr-xr-x   0 mingyang.ge   (502) staff       (20)        0 2023-07-10 20:06:26.682916 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     4219 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/PKG-INFO
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     3435 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/SOURCES.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)        1 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/dependency_links.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)      107 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/requires.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       11 2023-07-10 20:06:26.000000 databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/top_level.txt
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)       38 2023-07-10 20:06:26.683387 databricks-feature-lookup-0.6.0/setup.cfg
+-rw-r--r--   0 mingyang.ge   (502) staff       (20)     2724 2023-07-06 20:14:18.000000 databricks-feature-lookup-0.6.0/setup.py
```

### Comparing `databricks-feature-lookup-0.5.1/LICENSE.md` & `databricks-feature-lookup-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/PKG-INFO` & `databricks-feature-lookup-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.5.1
+Version: 0.6.0
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.5.1/README.md` & `databricks-feature-lookup-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/__init__.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_feature_store_object.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_feature_store_object.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/_proto_enum_entity.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/_proto_enum_entity.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/column_info.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/column_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import Optional, Union
 
 from databricks.feature_store.entities._feature_store_object import _FeatureStoreObject
 from databricks.feature_store.entities.feature_column_info import FeatureColumnInfo
 from databricks.feature_store.entities.feature_spec_constants import (
     FEATURE_COLUMN_INFO,
     ON_DEMAND_COLUMN_INFO,
     SOURCE_DATA_COLUMN_INFO,
@@ -21,35 +21,44 @@
     ColumnInfo's structure and properties are mapped 1:1 to the ColumnInfo proto message, unless specified otherwise.
     """
 
     def __init__(
         self,
         info: Union[SourceDataColumnInfo, FeatureColumnInfo, OnDemandColumnInfo],
         include: bool,
+        data_type: Optional[str] = None,
     ):
         if not isinstance(
             info, (SourceDataColumnInfo, FeatureColumnInfo, OnDemandColumnInfo)
         ):
             raise ValueError(
                 "info must be one of SourceDataColumnInfo, FeatureColumnInfo, OnDemandColumnInfo."
             )
         self._info = info
         self._include = include
+        self._data_type = data_type
 
     @property
     def info(
         self,
     ) -> Union[SourceDataColumnInfo, FeatureColumnInfo, OnDemandColumnInfo]:
         return self._info
 
     @property
     def include(self) -> bool:
         return self._include
 
     @property
+    def data_type(self) -> Optional[str]:
+        """
+        FeatureSpecs before v7 are not required to have data types.
+        """
+        return self._data_type
+
+    @property
     def output_name(self) -> str:
         """
         This field does not exist in the proto, and is provided for convenience.
         """
         return self.info.output_name
 
     @classmethod
@@ -63,18 +72,25 @@
         elif column_info_proto.HasField(ON_DEMAND_COLUMN_INFO):
             info = OnDemandColumnInfo.from_proto(
                 column_info_proto.on_demand_column_info
             )
         else:
             raise ValueError("Unsupported info type: " + str(column_info_proto))
 
-        return ColumnInfo(info=info, include=column_info_proto.include)
+        data_type = (
+            column_info_proto.data_type
+            if column_info_proto.HasField("data_type")
+            else None
+        )
+        return ColumnInfo(
+            info=info, include=column_info_proto.include, data_type=data_type
+        )
 
     def to_proto(self):
-        column_info = ProtoColumnInfo(include=self.include)
+        column_info = ProtoColumnInfo(include=self.include, data_type=self.data_type)
         if isinstance(self.info, SourceDataColumnInfo):
             column_info.source_data_column_info.CopyFrom(self.info.to_proto())
         elif isinstance(self.info, FeatureColumnInfo):
             column_info.feature_column_info.CopyFrom(self.info.to_proto())
         elif isinstance(self.info, OnDemandColumnInfo):
             column_info.on_demand_column_info.CopyFrom(self.info.to_proto())
         else:
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/data_type.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/data_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_column_info.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_functions_for_serving.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_functions_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from mlflow.utils.file_utils import TempDir, read_yaml, write_yaml
 
 from databricks.feature_store.entities._feature_store_object import _FeatureStoreObject
 from databricks.feature_store.entities.column_info import ColumnInfo
 from databricks.feature_store.entities.feature_column_info import FeatureColumnInfo
 from databricks.feature_store.entities.feature_spec_constants import (
     BOUND_TO,
+    DATA_TYPE,
     FEATURE_COLUMN_INFO,
     FEATURE_STORE,
     INCLUDE,
     INPUT_BINDINGS,
     INPUT_COLUMNS,
     INPUT_FUNCTIONS,
     INPUT_TABLES,
@@ -46,20 +47,21 @@
 # 2. (2021/06/16): Record feature_store_client_version to help us make backward compatible changes in the future.
 # 3. (2021/08/25): Record table_id to handle feature table lineage stability if tables are deleted.
 # 4. (2021/09/25): Record timestamp_lookup_key to handle point-in-time lookups.
 # 5. (2021/02/15): Record include flag for column info if False.
 #                  Record input functions as FunctionInfo and function computation as OnDemandColumnInfo.
 #                  Remove redundant fields: table_name from table_infos, output_name from column_infos.
 # 6. (2023/04/21): Record lookback_window in table info for point-in-time lookups.
+# 7. (2023/05/05): Record the Spark data type for all columns to track model signatures.
 
 
 class FeatureSpec(_FeatureStoreObject):
 
     FEATURE_ARTIFACT_FILE = "feature_spec.yaml"
-    SERIALIZATION_VERSION_NUMBER = 6
+    SERIALIZATION_VERSION_NUMBER = 7
 
     def __init__(
         self,
         column_infos: List[ColumnInfo],
         table_infos: List[FeatureTableInfo],
         function_infos: List[FunctionInfo],
         workspace_id: int,
@@ -267,14 +269,17 @@
         else:
             raise ValueError(
                 f"Expected column_info to be keyed by a valid ColumnInfo.info type. "
                 f"'{column_info}' has key '{list(column_info)[0]}'."
             )
 
         # Parse and insert ColumnInfo level attributes
+        # DATA_TYPE is supported starting FeatureSpec v7 and is not guaranteed to exist.
+        if DATA_TYPE in column_info:
+            column_info_attributes[DATA_TYPE] = column_info[DATA_TYPE]
         if not column_info[INCLUDE]:
             column_info_attributes[INCLUDE] = False
 
         # Insert source; return YAML keyed by column_name
         column_info_attributes[SOURCE] = source
         return {column_name: column_info_attributes}
 
@@ -366,14 +371,17 @@
         else:
             raise ValueError(
                 f"Internal Error: Expected column_info to have source matching oneof ColumnInfo.info. "
                 f"'{column_info}' has source of '{source}'."
             )
 
         # Parse ColumnInfo level attributes
+        # DATA_TYPE is supported starting FeatureSpec v7 and is not guaranteed to exist.
+        if DATA_TYPE in column_data:
+            column_info_dict[DATA_TYPE] = column_data.pop(DATA_TYPE)
         # INCLUDE is supported starting FeatureSpec v5 and only present in the YAML when INCLUDE = False
         if INCLUDE in column_data:
             column_info_dict[INCLUDE] = column_data.pop(INCLUDE)
         return column_info_dict
 
     @classmethod
     def _from_dict(cls, spec_dict):
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_spec_constants.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_spec_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 OUTPUT_NAME = "output_name"
 INPUT_TABLES = "input_tables"
 TABLE_NAME = "table_name"
 TABLE_ID = "table_id"
 SERIALIZATION_VERSION = "serialization_version"
 INPUT_FUNCTIONS = "input_functions"
 INCLUDE = "include"
+DATA_TYPE = "data_type"
 UDF_NAME = "udf_name"
 INPUT_BINDINGS = "input_bindings"
 PARAMETER = "parameter"
 BOUND_TO = "bound_to"
 
 # FeatureSpec YAML source field and allowed values
 SOURCE = "source"
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_table_info.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_table_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/feature_tables_for_serving.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/feature_tables_for_serving.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/function_info.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/function_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/on_demand_column_info.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/on_demand_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_feature_table.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/online_feature_table.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/online_store_for_serving.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/online_store_for_serving.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,28 @@
     DynamoDbConf as ProtoDynamoDbConf,
 )
 from databricks.feature_store.protos.feature_store_serving_pb2 import (
     OnlineStoreForSageMakerServing as ProtoOnlineStoreForSageMakerServing,
 )
 
 
+class BrickstoreConf(_FeatureStoreObject):
+    def __init__(self, host: str, port: int):
+        self._host = host
+        self._port = port
+
+    @property
+    def host(self):
+        return self._host
+
+    @property
+    def port(self):
+        return self._port
+
+
 class MySqlConf(_FeatureStoreObject):
     def __init__(self, host: str, port: int):
         self._host = host
         self._port = port
 
     @property
     def host(self):
@@ -58,15 +72,15 @@
         return self._account_uri
 
 
 class AbstractOnlineStoreForServing(_FeatureStoreObject):
     def __init__(
         self,
         creation_timestamp_ms: int,
-        extra_configs: Union[MySqlConf, SqlServerConf, DynamoDbConf],
+        extra_configs: Union[BrickstoreConf, MySqlConf, SqlServerConf, DynamoDbConf],
         query_mode: QueryMode,
     ):
         self._creation_timestamp_ms = creation_timestamp_ms
         self._extra_configs = extra_configs
         self._query_mode = query_mode
 
     @property
@@ -112,14 +126,18 @@
         conf = None
         if the_proto.WhichOneof("extra_configs") == "mysql_conf":
             conf = MySqlConf(the_proto.mysql_conf.host, the_proto.mysql_conf.port)
         elif the_proto.WhichOneof("extra_configs") == "sql_server_conf":
             conf = SqlServerConf(
                 the_proto.sql_server_conf.host, the_proto.sql_server_conf.port
             )
+        elif the_proto.WhichOneof("extra_configs") == "brickstore_conf":
+            conf = BrickstoreConf(
+                the_proto.brickstore_conf.host, the_proto.brickstore_conf.port
+            )
         elif the_proto.WhichOneof("extra_configs") == "dynamodb_conf":
             conf = DynamoDbConf(the_proto.dynamodb_conf.region)
         elif the_proto.WhichOneof("extra_configs") == "cosmosdb_conf":
             conf = CosmosDbConf(the_proto.cosmosdb_conf.account_uri)
         else:
             raise ValueError("Unsupported Store Type: " + str(the_proto))
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/source_data_column_info.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/source_data_column_info.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/entities/store_type.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/entities/store_type.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_executor.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_executor.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/feature_function_loader.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/feature_function_loader.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/feature_functions/utils/codegen_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/feature_functions/utils/codegen_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/__init__.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from databricks.feature_store.lookup_engine.lookup_brickstore_engine import (
+    LookupBrickstoreEngine,
+)
 from databricks.feature_store.lookup_engine.lookup_cosmosdb_engine import (
     LookupCosmosDbEngine,
 )
 from databricks.feature_store.lookup_engine.lookup_dynamodb_engine import (
     AwsAccessKey,
     LookupDynamoDbEngine,
 )
@@ -15,8 +18,9 @@
 __all__ = [
     "LookupEngine",
     "LookupSqlEngine",
     "LookupMySqlEngine",
     "LookupSqlServerEngine",
     "LookupDynamoDbEngine",
     "LookupCosmosDbEngine",
+    "LookupBrickstoreEngine",
 ]
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_engine.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_mysql_engine.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_mysql_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_engine.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,19 @@
     CONSTRAINT_NAME = "CONSTRAINT_NAME"
 
     @abc.abstractmethod
     def __init__(
         self, online_feature_table: OnlineFeatureTable, ro_user: str, ro_password: str
     ):
         self.online_store = online_feature_table.online_store
-        (
-            self.database_name,
-            self.table_name,
-        ) = online_feature_table.online_feature_table_name.split(".")
+
+        (self.database_name, self.table_name) = self._get_database_and_table_name(
+            online_feature_table.online_feature_table_name
+        )
+
         self.user = ro_user
         self.password = ro_password
         self.host = self.online_store.extra_configs.host
         self.port = self.online_store.extra_configs.port
 
         self.primary_keys = online_feature_table.primary_keys
         self.feature_names_to_feature_details = {
@@ -63,14 +64,22 @@
         self.features_to_type_converter = {
             feature.name: SQL_DATA_TYPE_CONVERTER_FACTORY.get_converter(feature)
             for feature in online_feature_table.features
         }
 
         self._validate_online_feature_table()
 
+    def _get_database_and_table_name(self, online_table_name):
+        name_components = online_table_name.split(".")
+        if len(name_components) != 2:
+            raise ValueError(
+                f"Online table name {online_table_name} is misformatted and must be in 2L format for SQL stores"
+            )
+        return (name_components[0], name_components[1])
+
     @contextmanager
     def _get_connection(self):
         # Everything between here and the yield statement will be executed in contextmanager.__enter__()
 
         # We create a SQL engine instance per required online table in an inference request and dispose it afterwards.
         # A single inference request runs queries sequentially, so a connection pool is not required or beneficial.
         # TODO (ML-23188): Investigate sharing a long lived SQL engine and connection pool across inference requests.
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/lookup_engine/lookup_sql_server_engine.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import functools
 import itertools
 import os
 from collections import Counter, defaultdict
 from typing import Dict, List, Optional, Tuple, Union
 
 import mlflow
 import pandas as pd
@@ -22,27 +21,23 @@
     FeatureTablesForServing,
 )
 from databricks.feature_store.entities.online_feature_table import (
     AbstractOnlineFeatureTable,
     OnlineFeatureTable,
     PrimaryKeyDetails,
 )
-from databricks.feature_store.entities.store_type import StoreType
 from databricks.feature_store.feature_functions.feature_function_executor import (
     FeatureFunctionExecutor,
 )
 from databricks.feature_store.feature_lookup_version import VERSION
 from databricks.feature_store.online_lookup_client import (
     OnlineLookupClient,
     is_primary_key_lookup,
     tables_share_dynamodb_access_keys,
 )
-from databricks.feature_store.utils.feature_serving_patch import (
-    patch_feature_serving_predictions_to_json,
-)
 from databricks.feature_store.utils.metrics_utils import (
     OVERRIDEN_FEATURE_COUNT,
     LookupClientMetrics,
     lookup_call_maybe_with_metrics,
 )
 from databricks.feature_store.utils.uc_utils import (
     get_feature_spec_with_full_table_names,
@@ -57,16 +52,14 @@
 LOOKUP_CLIENT_INSTRUMENTATION_ENABLED_ENV = "LOOKUP_CLIENT_INSTRUMENTATION_ENABLED"
 # should match LOOKUP_CLIENT_FEATURE_FUNCTION_EVALUATION_ENABLED_ENV in
 # model-serving/model-serving-common/src/main/scala/com/databricks/mlflow/utils/serving/FeatureStoreConstants.scala
 LOOKUP_CLIENT_FEATURE_FUNCTION_EVALUATION_ENABLED_ENV = (
     "LOOKUP_CLIENT_FEATURE_FUNCTION_EVALUATION_ENABLED"
 )
 
-FEATURE_SERVING_RESPONSE_FORMAT_ENABLED = False
-
 LookupKeyType = Tuple[str, ...]
 LookupKeyToFeatureColumnInfosType = Dict[LookupKeyType, List[FeatureColumnInfo]]
 
 
 class _FeatureTableMetadata:
     """
     Encapsulates metadata on a feature table, including lookup keys, feature metadata, and online
@@ -732,27 +725,8 @@
         return {ft: all_fts_to_online_ft[ft] for ft in feature_tables}
 
 
 def _load_pyfunc(path):
     """
     Called by ``pyfunc.load_pyfunc``.
     """
-    if FEATURE_SERVING_RESPONSE_FORMAT_ENABLED:
-        raw_model = _load_raw_model(path)
-        try:
-            py_model = raw_model._model_impl.python_model
-            if (
-                hasattr(py_model, "_is_databricks_internal_feature_serving_model")
-                and py_model._is_databricks_internal_feature_serving_model
-            ):
-                from src.mlflowserving import scoring_server
-
-                scoring_server.predictions_to_json = (
-                    patch_feature_serving_predictions_to_json
-                )
-        except AttributeError as ae:
-            # Shouldn't happen when the model is created with feature store client.
-            print(f"Failed when checking model attribute: {repr(ae)}")
-        except ImportError as ie:
-            raise RuntimeError(f"Failed to load feature serving model: {repr(ie)}")
-
     return _FeatureStoreModelWrapper(path)
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/mlflow_model_constants.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/mlflow_model_constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 #
 # - The Feature lookup client major version (eg `{FEATURE_LOOKUP_CLIENT_PIP_PACKAGE}.0.1`)
 # - The pinned major version of the databricks-feature-lookup requirement in logged model's conda.yaml
 #
 # If needed, these can be decoupled into separate constants, but that decision should be carefully considered.
 FEATURE_LOOKUP_CLIENT_MAJOR_VERSION = 0
 
-# The minor.micro version number of the feature lookup client Alpha version. The Alpha version is used
-# by core client when logging model to create Feature Serving Endpoint.
-# Minor version
-FEATURE_LOOKUP_CLIENT_ALPHA_MINOR_VERSION = 3
-# Micro version
-FEATURE_LOOKUP_CLIENT_ALPHA_MICRO_VERSION = 1
-
 DATABRICKS = "Databricks"
 SAGEMAKER = "SageMaker"
 
 # Model artifact directory where we expect Feature Store internal artifacts to live. This must
 # match the directory specified in ModelServingUtils:
 # https://src.dev.databricks.com/databricks/universe@4dff77c752b546579f239815e520d566d2dbda20/-/blob/model-serving/model-serving-common/src/main/scala/com/databricks/modelservingcommon/utils/ModelServingUtils.scala?L117
 FEATURE_STORE_INTERNAL_DATA_DIR = "_databricks_internal/"
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/online_lookup_client.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/online_lookup_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     OnlineFeatureTable,
     OnlineFeatureTableForSageMakerServing,
 )
 from databricks.feature_store.entities.query_mode import QueryMode
 from databricks.feature_store.entities.store_type import StoreType
 from databricks.feature_store.lookup_engine import (
     AwsAccessKey,
+    LookupBrickstoreEngine,
     LookupCosmosDbEngine,
     LookupDynamoDbEngine,
     LookupEngine,
     LookupMySqlEngine,
     LookupSqlEngine,
     LookupSqlServerEngine,
 )
@@ -24,14 +25,18 @@
 
 # The provisioner of this model is expected to set the following environment variable for each
 # feature table if the feature store is SQL based:
 #  (1) <online_store_for_serving.read_secret_prefix>_USER
 #  (2) <online_store_for_serving.read_secret_prefix>_PASSWORD
 USER_SUFFIX = "_USER"
 PASSWORD_SUFFIX = "_PASSWORD"
+# For BRICKSTORE we use a fixed prefix unlike other stores. This is because for Brickstore all
+# permissions are assigned to the same user and password. More details at
+# https://docs.google.com/document/d/10w-r-pGEg9tbA-QDip1TBLeCDqDgxojqg-HBBBNp1h0/edit#heading=h.tijd0n6d441z
+BRICKSTORE_PREFIX = "BRICKSTORE"
 # For DynamoDB the following variables should be set:
 #  (1) <online_store_for_serving.read_secret_prefix>_ACCESS_KEY_ID
 #  (2) <online_store_for_serving.read_secret_prefix>_SECRET_ACCESS_KEY
 ACCESS_KEY_ID_SUFFIX = "_ACCESS_KEY_ID"
 SECRET_ACCESS_KEY_SUFFIX = "_SECRET_ACCESS_KEY"
 # For Cosmos DB the following variable should be set:
 #  (1) <online_store_for_serving.read_secret_prefix>_AUTHORIZATION_KEY
@@ -45,15 +50,17 @@
     ],
     creds: Tuple[str, str],
 ) -> LookupSqlEngine:
     if isinstance(online_feature_table, List):
         raise Exception(f"Internal error: Batch lookup is unsupported in SQL Engine.")
 
     ro_user, ro_password = creds
-    if online_feature_table.online_store.store_type == StoreType.SQL_SERVER:
+    if online_feature_table.online_store.store_type == StoreType.BRICKSTORE:
+        return LookupBrickstoreEngine(online_feature_table, ro_user, ro_password)
+    elif online_feature_table.online_store.store_type == StoreType.SQL_SERVER:
         return LookupSqlServerEngine(online_feature_table, ro_user, ro_password)
     return LookupMySqlEngine(online_feature_table, ro_user, ro_password)
 
 
 def generate_lookup_dynamodb_engine(
     online_feature_table: Union[
         AbstractOnlineFeatureTable, List[AbstractOnlineFeatureTable]
@@ -80,15 +87,19 @@
     if isinstance(online_feature_table, List):
         raise Exception(f"Internal error: Batch lookup is unsupported in Cosmos DB.")
     return LookupCosmosDbEngine(online_feature_table, authorization_key=creds)
 
 
 def load_credentials_from_env(online_ft: OnlineFeatureTable):
     def get_env_var(env_var_suffix: str) -> str:
-        env_var = online_ft.online_store.read_secret_prefix + env_var_suffix
+        env_var = ""
+        if online_ft.online_store.store_type == StoreType.BRICKSTORE:
+            env_var = BRICKSTORE_PREFIX + env_var_suffix
+        else:
+            env_var = online_ft.online_store.read_secret_prefix + env_var_suffix
         if env_var not in os.environ:
             raise Exception(
                 f"Internal error: {env_var} not found for feature table {online_ft.feature_table_name}."
             )
         return os.getenv(env_var)
 
     if online_ft.online_store.store_type == StoreType.DYNAMODB:
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_spec_pb2.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_spec_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from mlflow.protos.scalapb import scalapb_pb2 as scalapb_dot_scalapb__pb2
 from mlflow.protos import databricks_pb2 as databricks__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x66\x65\x61ture_spec.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\x1a\x10\x64\x61tabricks.proto\"$\n\x14SourceDataColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x46\x65\x61tureColumnInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x12\n\nlookup_key\x18\x03 \x03(\t\x12\x13\n\x0boutput_name\x18\x04 \x01(\t\x12\x1c\n\x14timestamp_lookup_key\x18\x05 \x03(\t\"3\n\x0cInputBinding\x12\x11\n\tparameter\x18\x01 \x01(\t\x12\x10\n\x08\x62ound_to\x18\x02 \x01(\t\"u\n\x12OnDemandColumnInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\x12\x38\n\x0einput_bindings\x18\x02 \x03(\x0b\x32 .featurestorecommon.InputBinding\x12\x13\n\x0boutput_name\x18\x03 \x01(\t\"\x87\x02\n\nColumnInfo\x12K\n\x17source_data_column_info\x18\x01 \x01(\x0b\x32(.featurestorecommon.SourceDataColumnInfoH\x00\x12\x44\n\x13\x66\x65\x61ture_column_info\x18\x02 \x01(\x0b\x32%.featurestorecommon.FeatureColumnInfoH\x00\x12G\n\x15on_demand_column_info\x18\x03 \x01(\x0b\x32&.featurestorecommon.OnDemandColumnInfoH\x00\x12\x15\n\x07include\x18\n \x01(\x08:\x04trueB\x06\n\x04info\"Q\n\x10\x46\x65\x61tureTableInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x10\n\x08table_id\x18\x02 \x01(\t\x12\x17\n\x0flookback_window\x18\x03 \x01(\x03\" \n\x0c\x46unctionInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\"\x96\x02\n\x0b\x46\x65\x61tureSpec\x12\x35\n\rinput_columns\x18\x01 \x03(\x0b\x32\x1e.featurestorecommon.ColumnInfo\x12\x1d\n\x15serialization_version\x18\x02 \x01(\x05\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\x03\x12$\n\x1c\x66\x65\x61ture_store_client_version\x18\x04 \x01(\t\x12:\n\x0cinput_tables\x18\x05 \x03(\x0b\x32$.featurestorecommon.FeatureTableInfo\x12\x39\n\x0finput_functions\x18\x06 \x03(\x0b\x32 .featurestorecommon.FunctionInfoBC\n\'com.databricks.proto.featurestorecommonB\x10\x46\x65\x61tureSpecProto\xa0\x01\x01\xe2?\x02\x10\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x66\x65\x61ture_spec.proto\x12\x12\x66\x65\x61turestorecommon\x1a\x15scalapb/scalapb.proto\x1a\x10\x64\x61tabricks.proto\"$\n\x14SourceDataColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x46\x65\x61tureColumnInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\x12\x12\n\nlookup_key\x18\x03 \x03(\t\x12\x13\n\x0boutput_name\x18\x04 \x01(\t\x12\x1c\n\x14timestamp_lookup_key\x18\x05 \x03(\t\"3\n\x0cInputBinding\x12\x11\n\tparameter\x18\x01 \x01(\t\x12\x10\n\x08\x62ound_to\x18\x02 \x01(\t\"u\n\x12OnDemandColumnInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\x12\x38\n\x0einput_bindings\x18\x02 \x03(\x0b\x32 .featurestorecommon.InputBinding\x12\x13\n\x0boutput_name\x18\x03 \x01(\t\"\x9a\x02\n\nColumnInfo\x12K\n\x17source_data_column_info\x18\x01 \x01(\x0b\x32(.featurestorecommon.SourceDataColumnInfoH\x00\x12\x44\n\x13\x66\x65\x61ture_column_info\x18\x02 \x01(\x0b\x32%.featurestorecommon.FeatureColumnInfoH\x00\x12G\n\x15on_demand_column_info\x18\x03 \x01(\x0b\x32&.featurestorecommon.OnDemandColumnInfoH\x00\x12\x15\n\x07include\x18\n \x01(\x08:\x04true\x12\x11\n\tdata_type\x18\x0b \x01(\tB\x06\n\x04info\"Q\n\x10\x46\x65\x61tureTableInfo\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x10\n\x08table_id\x18\x02 \x01(\t\x12\x17\n\x0flookback_window\x18\x03 \x01(\x03\" \n\x0c\x46unctionInfo\x12\x10\n\x08udf_name\x18\x01 \x01(\t\"\x96\x02\n\x0b\x46\x65\x61tureSpec\x12\x35\n\rinput_columns\x18\x01 \x03(\x0b\x32\x1e.featurestorecommon.ColumnInfo\x12\x1d\n\x15serialization_version\x18\x02 \x01(\x05\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\x03\x12$\n\x1c\x66\x65\x61ture_store_client_version\x18\x04 \x01(\t\x12:\n\x0cinput_tables\x18\x05 \x03(\x0b\x32$.featurestorecommon.FeatureTableInfo\x12\x39\n\x0finput_functions\x18\x06 \x03(\x0b\x32 .featurestorecommon.FunctionInfoBC\n\'com.databricks.proto.featurestorecommonB\x10\x46\x65\x61tureSpecProto\xa0\x01\x01\xe2?\x02\x10\x01')
 
 
 
 _SOURCEDATACOLUMNINFO = DESCRIPTOR.message_types_by_name['SourceDataColumnInfo']
 _FEATURECOLUMNINFO = DESCRIPTOR.message_types_by_name['FeatureColumnInfo']
 _INPUTBINDING = DESCRIPTOR.message_types_by_name['InputBinding']
 _ONDEMANDCOLUMNINFO = DESCRIPTOR.message_types_by_name['OnDemandColumnInfo']
@@ -93,15 +93,15 @@
   _FEATURECOLUMNINFO._serialized_start=122
   _FEATURECOLUMNINFO._serialized_end=254
   _INPUTBINDING._serialized_start=256
   _INPUTBINDING._serialized_end=307
   _ONDEMANDCOLUMNINFO._serialized_start=309
   _ONDEMANDCOLUMNINFO._serialized_end=426
   _COLUMNINFO._serialized_start=429
-  _COLUMNINFO._serialized_end=692
-  _FEATURETABLEINFO._serialized_start=694
-  _FEATURETABLEINFO._serialized_end=775
-  _FUNCTIONINFO._serialized_start=777
-  _FUNCTIONINFO._serialized_end=809
-  _FEATURESPEC._serialized_start=812
-  _FEATURESPEC._serialized_end=1090
+  _COLUMNINFO._serialized_end=711
+  _FEATURETABLEINFO._serialized_start=713
+  _FEATURETABLEINFO._serialized_end=794
+  _FUNCTIONINFO._serialized_start=796
+  _FUNCTIONINFO._serialized_end=828
+  _FEATURESPEC._serialized_start=831
+  _FEATURESPEC._serialized_end=1109
 # @@protoc_insertion_point(module_scope)
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/protos/feature_store_serving_pb2.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/protos/feature_store_serving_pb2.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/converter_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/converter_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/cosmosdb_type_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/cosmosdb_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/data_type_details_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/data_type_details_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_type_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/dynamodb_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/dynamodb_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,21 +68,23 @@
 
 
 def get_dynamodb_resource(
     access_key_id: str,
     secret_access_key: str,
     region: str,
     session_token: Optional[str] = None,
+    endpoint_url: Optional[str] = None,
 ):
     return boto3.resource(
         DYNAMODB,
         aws_access_key_id=access_key_id,
         aws_secret_access_key=secret_access_key,
         region_name=region,
         aws_session_token=session_token,
+        endpoint_url=endpoint_url,
     )
 
 
 def paginate_keys(
     batch_keys: Dict[str, List[Any]],
     batch_size_limit: int,
 ) -> List[Dict[str, List[Any]]]:
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_function_type_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_function_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/feature_spec_test_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/feature_spec_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/metrics_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/pandas_type_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/pandas_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/serving_test_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/serving_test_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/sql_type_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/sql_type_utils.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/uc_utils.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/uc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import copy
 import re
 from typing import Set
 
 from databricks.feature_store.entities.feature_spec import FeatureSpec
 
-SINGLE_LEVEL_NAMESPACE_REGEX = r"^[\w_]+$"
-TWO_LEVEL_NAMESPACE_REGEX = r"^[\w_]+(\.[\w_]+)$"
-THREE_LEVEL_NAMESPACE_REGEX = r"^[\w_]+(\.[\w_]+){2}$"
+SINGLE_LEVEL_NAMESPACE_REGEX = r"^[^\. \/\x00-\x1F\x7F]+$"
+TWO_LEVEL_NAMESPACE_REGEX = r"^[^\. \/\x00-\x1F\x7F]+(\.[^\. \/\x00-\x1F\x7F]+)$"
+THREE_LEVEL_NAMESPACE_REGEX = (
+    r"^[^\. \/\x00-\x1F\x7F]+(\.[^\. \/\x00-\x1F\x7F]+)(\.[^\. \/\x00-\x1F\x7F]+)$"
+)
 
 HIVE_METASTORE_NAME = "hive_metastore"
 # these two catalog names both points to the workspace local default HMS (hive metastore).
 LOCAL_METASTORE_NAMES = [HIVE_METASTORE_NAME, "spark_catalog"]
 # samples catalog is managed by databricks for hosting public dataset like NYC taxi dataset.
 # it is neither a UC nor local metastore catalog, accessing samples catalog using feature store client is not allowed.
 SAMPLES_CATALOG_NAME = "samples"
@@ -174,19 +176,16 @@
 def _is_three_level_name(name) -> bool:
     return (
         isinstance(name, str)
         and re.match(THREE_LEVEL_NAMESPACE_REGEX, name) is not None
     )
 
 
-def tagging_for_uc_tables_error(full_table_name):
-    return ValueError(
-        f"Cannot set or delete tags for table {full_table_name}. "
-        f"Tagging for Feature Tables in Unity Catalog is not yet supported."
-    )
+def unsupported_api_error_uc(api_name):
+    return ValueError(f"{api_name} is not supported for Unity Catalog tables.")
 
 
 # check if entity is in UC and not in samples catalog
 def is_uc_entity(full_entity_name) -> bool:
     catalog_name, schema_name, table_name = full_entity_name.split(".")
     return (
         not is_default_hms_table(full_entity_name)
```

### Comparing `databricks-feature-lookup-0.5.1/databricks/feature_store/utils/utils_common.py` & `databricks-feature-lookup-0.6.0/databricks/feature_store/utils/utils_common.py`

 * *Files identical despite different names*

### Comparing `databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/PKG-INFO` & `databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-feature-lookup
-Version: 0.5.1
+Version: 0.6.0
 Summary: Databricks Feature Store Feature Lookup Client
 Author: Databricks
 Author-email: feedback@databricks.com
 License: Databricks Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `databricks-feature-lookup-0.5.1/databricks_feature_lookup.egg-info/SOURCES.txt` & `databricks-feature-lookup-0.6.0/databricks_feature_lookup.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.md
+MANIFEST.in
 NOTICE.md
 README.md
 setup.py
 databricks/_feature_store_pkg_metadata/__init__.py
 databricks/_feature_store_pkg_metadata/_lookup_client_pkg_metadata/__init__.py
 databricks/feature_store/__init__.py
 databricks/feature_store/feature_lookup_version.py
@@ -29,14 +30,15 @@
 databricks/feature_store/entities/source_data_column_info.py
 databricks/feature_store/entities/store_type.py
 databricks/feature_store/feature_functions/feature_function_executor.py
 databricks/feature_store/feature_functions/feature_function_loader.py
 databricks/feature_store/feature_functions/utils/__init__.py
 databricks/feature_store/feature_functions/utils/codegen_utils.py
 databricks/feature_store/lookup_engine/__init__.py
+databricks/feature_store/lookup_engine/lookup_brickstore_engine.py
 databricks/feature_store/lookup_engine/lookup_cosmosdb_engine.py
 databricks/feature_store/lookup_engine/lookup_dynamodb_engine.py
 databricks/feature_store/lookup_engine/lookup_engine.py
 databricks/feature_store/lookup_engine/lookup_mysql_engine.py
 databricks/feature_store/lookup_engine/lookup_sql_engine.py
 databricks/feature_store/lookup_engine/lookup_sql_server_engine.py
 databricks/feature_store/protos/__init__.py
@@ -46,15 +48,14 @@
 databricks/feature_store/utils/converter_utils.py
 databricks/feature_store/utils/cosmosdb_type_utils.py
 databricks/feature_store/utils/cosmosdb_utils.py
 databricks/feature_store/utils/data_type_details_utils.py
 databricks/feature_store/utils/dynamodb_type_utils.py
 databricks/feature_store/utils/dynamodb_utils.py
 databricks/feature_store/utils/feature_function_type_utils.py
-databricks/feature_store/utils/feature_serving_patch.py
 databricks/feature_store/utils/feature_spec_test_utils.py
 databricks/feature_store/utils/metrics_utils.py
 databricks/feature_store/utils/pandas_type_utils.py
 databricks/feature_store/utils/serving_test_utils.py
 databricks/feature_store/utils/sql_type_utils.py
 databricks/feature_store/utils/test_utils_common.py
 databricks/feature_store/utils/uc_utils.py
```

### Comparing `databricks-feature-lookup-0.5.1/setup.py` & `databricks-feature-lookup-0.6.0/setup.py`

 * *Files identical despite different names*

