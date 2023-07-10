# Comparing `tmp/th2_data_services-2.0.0.dev5410321437.tar.gz` & `tmp/th2_data_services-2.0.0.dev5504842108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5410321437.tar", last modified: Thu Jun 29 08:55:23 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5504842108.tar", last modified: Mon Jul 10 06:33:22 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5410321437.tar` & `th2_data_services-2.0.0.dev5504842108.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23948 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-29 08:55:05.000000 th2_data_services-2.0.0.dev5410321437/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14697 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23948 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-10 06:33:12.000000 th2_data_services-2.0.0.dev5504842108/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5358 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5410321437/PKG-INFO` & `th2_data_services-2.0.0.dev5504842108/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3534 3130 3332 3134 3337 0a53 756d 6d61  5410321437.Summa
+00000040: 3535 3034 3834 3231 3038 0a53 756d 6d61  5504842108.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5410321437/README.md` & `th2_data_services-2.0.0.dev5504842108/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/setup.py` & `th2_data_services-2.0.0.dev5504842108/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/aggregation_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         if rows is not None:
             self.add_rows(rows)
 
     def get_categories(self) -> List[str]:
         """Returns categories."""
         return self.header[1:]  # Skip timestamp.
 
-    def by_category(self, name, exclude_zero_values=True):
+    def by_category(self, name, exclude_zero_values=True) -> "FrequencyCategoryTable":
         """Returns CategoryFrequencies for requested column."""
         header_lst = self.header
         if name not in self.get_categories():
             raise ValueError(f"'{name}' is not categories: {self.get_categories()}")
         col_name_idx = header_lst.index(name)
         timestamp_col_name = header_lst[0]
         fct = FrequencyCategoryTable(header=[timestamp_col_name, name])
@@ -180,15 +180,15 @@
                 if val != 0:
                     fct.add_row([row[self.service_columns["timestamp"]], val])
             else:
                 fct.add_row([row[self.service_columns["timestamp"]], val])
 
         return fct
 
-    def by_categories(self, names: List[str], exclude_zero_values=True):
+    def by_categories(self, names: List[str], exclude_zero_values=True) -> "FrequencyCategoryTable":
         """Returns CategoryFrequencies for requested column."""
         header_lst = self.header
         for name in names:
             if name not in self.get_categories():
                 raise ValueError(f"'{name}' is not categories: {self.get_categories()}")
 
         col_name_idxs = []
@@ -216,18 +216,19 @@
         self.service_columns = {
             "timestamp": 0,
         }  # {'col_name': 'idx'}
         if rows is not None:
             self.add_rows(rows)
 
         self._transposed = False
+        self.count_field_name = "count"
 
     @property
     def total(self):
-        return sum(self["count"])
+        return sum(self[self.count_field_name])
 
     def _totals_line(self):
         totals = []
         for col_name in self.header:
             col_tuple = self[col_name]
 
             try:
@@ -260,15 +261,19 @@
 
     def get_list_repr(self):
         additional_rows = [
             # ['' for i in range(len(self.header) - 1)] + [self.total],
             ["count"] + ["" for _ in range(len(self.header) - 1)] + [len(self.rows)],
             ["totals"] + self._totals_line(),
         ]
-        return [[" "] + list(self.header), *[[" "] + list(row) for row in self.rows], *additional_rows]
+        return [
+            [" "] + list(self.header),
+            *[[" "] + list(row) for row in self.rows],
+            *additional_rows,
+        ]
 
     def transpose_column(self, column_name) -> "TotalCategoryTable":
         """Returns a new table with transposed column.
 
         Look at the example below.
 
         Example:
@@ -351,27 +356,29 @@
             +--------+-------------+----------------+------+------+------+------+
 
 
         """
         static_col_names = []
         dynamic_col_names = set()
         for h in self.header:
-            if h == column_name or h == "count":
+            if h == column_name or h == self.count_field_name:
                 pass
             else:
                 static_col_names.append(h)
 
         new_tbl_dict = {}  # {(static_columns): {dynamic_col: val} }
 
         for row in self.rows:
             new_row = []
             for h in static_col_names:
                 new_row.append(row[h])
 
-            new_tbl_dict.setdefault(tuple(new_row), {})[row[column_name]] = row["count"]
+            new_tbl_dict.setdefault(tuple(new_row), {})[row[column_name]] = row[
+                self.count_field_name
+            ]
             dynamic_col_names.add(row[column_name])
 
         dynamic_col_names_lst = sorted(list(dynamic_col_names))
         new_header = static_col_names + dynamic_col_names_lst
         new_tbl = TotalCategoryTable(header=new_header)
         """
         {('OUT', 'NewOrderSingle'): {'s3': 34},
```

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/frequencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 # STREAMING
 @deprecated(
     reason='Use "get_category_frequencies2" instead. \n'
     "We want to have unification in functions.\n"
     "Tell DS team if you dont agree or have some ideas."
 )
 def get_category_frequencies(
-    events: Iterable[Th2Event], categories: List[str], categorizer: Callable, aggregation_level: str = "seconds"
+    events: Iterable[Th2Event],
+    categories: List[str],
+    categorizer: Callable,
+    aggregation_level: str = "seconds",
 ) -> FrequencyCategoryTable:
     """Returns event frequencies based on event category.
 
     Args:
         events (Iterable[Th2Event]): TH2-Events
         categories (List[str]): Event Categories
         categorizer (Callable): Categorizer Method
@@ -71,16 +74,16 @@
 def get_category_frequencies2(
     events: Iterable[Th2Event], category: Category, aggregation_level: str = "seconds"
 ) -> FrequencyCategoryTable:
     """Returns event frequencies based on event category.
 
     Args:
         events (Iterable[Th2Event]): TH2-Events
-        categories (List[str]): Event Categories
-        categorizer (Callable): Categorizer Method
+        category: The name of the category doesn't make sence.
+            Used just for unification to use general Category class.
         aggregation_level (Optional, str): Aggregation Level
 
     Returns:
         List[List[str]]
 
     Example:
         >>> get_category_frequencies(events=events,
@@ -98,15 +101,17 @@
 
     """
     return misc_utils.get_objects_frequencies2(
         events,
         categories=[],
         categorizer=category.get_func,
         # TODO -- we shouldn't know internal structure!!! - epochSeconds
-        timestamp_function=lambda e: options.EVENT_FIELDS_RESOLVER.get_start_timestamp(e)["epochSecond"],
+        timestamp_function=lambda e: options.EVENT_FIELDS_RESOLVER.get_start_timestamp(e)[
+            "epochSecond"
+        ],
         aggregation_level=aggregation_level,
     )
 
 
 # STREAMING
 # TODO - slava
 #   Do we really need it? Why user cannot just use this one line?
```

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/message_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 import base64
 from collections import defaultdict
 
 # from th2_data_services import MESSAGE_FIELDS_RESOLVER
 from typing import Callable, Dict, Iterable, List, Set
+
+from deprecated.classic import deprecated
+
 import th2_data_services.utils.display
 import th2_data_services.utils.time
 from th2_data_services.utils._types import Th2Message
 
 from th2_data_services.config import options
 
 
@@ -240,17 +243,21 @@
     max_count = max(max_count + 1, len(result))
     for i in range(max_count):
         print_message(result[i])
 
 
 # STREAMABLE
 # TODO - We will not use this in the future, I think, because LwDP can provide JSON_PARSED immediately.
+@deprecated(
+    "This function only make sense if you have data in Protobuf style format.\n"
+    "Use DS-LwDP>=2.0.2.* to get messages in JSON-PARSED format.\n"
+    "Use `th2_data_services.utils.converters.flatten_dict` instead of this function."
+)
 def message_fields_to_flat_dict(message: dict, result: Dict, prefix: str):  # noqa
     # Actual if provider returns data in Protobuf style
-    # TODO: Add Docstings
     for field, content in message["fields"].items():
         if "simpleValue" in content:
             result[prefix + field] = content["simpleValue"]
 
         if "messageValue" in content:
             new_prefix = f"{prefix}{field}."
             message_fields_to_flat_dict(content["messageValue"], result, new_prefix)
```

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from datetime import datetime
 from typing import Dict, Union
-
-
-# TODO - looks ok, but it's better to add such feature to utils.converters
 from deprecated.classic import deprecated
 
 
 def extract_timestamp(timestamp_element: Dict) -> str:
     """Extracts timestamp from argument.
 
     Args:
@@ -29,15 +26,23 @@
         str representation of th2-timestamp(protobuf) e.g. 2023-03-09T05:37:53.263895000
     """
     timestamp = datetime.fromtimestamp(timestamp_element["epochSecond"])
     return f"{timestamp.isoformat()}.{str(timestamp_element['nano']).zfill(9)}"
 
 
 @deprecated("Use `extract_timestamp` instead")
-def extract_time_string(timestamp_element):
+def extract_time_string(timestamp_element) -> str:
+    """Extracts timestamp from argument.
+
+    Args:
+        timestamp_element:
+
+    Returns:
+        str representation of th2-timestamp(protobuf) e.g. 2023-03-09T05:37:53.263895000
+    """
     return extract_timestamp(timestamp_element)
 
 
 # TODO - to be honest, the name of the function is difficult
 def time_interval_filter_seconds_precision(
     timestamp_element: Dict, start_timestamp: Union[int, float], end_timestamp: Union[int, float]
 ) -> bool:
@@ -66,15 +71,17 @@
     """
     seconds_delta = (end_timestamp["epochSecond"] - start_timestamp["epochSecond"]) * 1000000
     nano_delta = (end_timestamp["nano"] - start_timestamp["nano"]) / 1000
     return seconds_delta + nano_delta
 
 
 # TODO - looks ok, but we need to think about unified timestamps
-def time_slice_object_filter(timestamp_field: Dict, timestamp_iso: str, duration_seconds: int):  # noqa
+def time_slice_object_filter(
+    timestamp_field: Dict, timestamp_iso: str, duration_seconds: int
+):  # noqa
     """Filter elements that from time moment  A to  A+duration_seconds.
 
     Args:
         timestamp_field:
         timestamp_iso:
         duration_seconds:
 
@@ -146,16 +153,20 @@
             dynamic_aggr_level = int(num) * 3600 * 24
 
         elif aggregation_level.endswith("d"):
             num = aggregation_level.split("d")[0]
             dynamic_aggr_level = int(num) * 3600 * 24
 
         else:
-            raise KeyError(f"Invalid aggregation level. Available levels: {', '.join(aggregation_levels)}")
+            raise KeyError(
+                f"Invalid aggregation level. Available levels: {', '.join(aggregation_levels)}"
+            )
         aggregation_levels[aggregation_level] = dynamic_aggr_level
 
     try:
         interval = aggregation_levels[aggregation_level]
     except KeyError:
-        raise KeyError(f"Invalid aggregation level. Available levels: {', '.join(aggregation_levels)}")
+        raise KeyError(
+            f"Invalid aggregation level. Available levels: {', '.join(aggregation_levels)}"
+        )
 
     return global_anchor_timestamp + interval * ((timestamp - global_anchor_timestamp) // interval)
```

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/total_category_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         self,
         categories: List[Category],
         combinations: Union[List[Sequence[str]], List[Sequence[Category]]],
     ):
         """Calculates, aggregates to tables and prints categories combinations.
 
         This class allows you to calculate any metrics and their combinations in stream-like way.
+        It calculates how many times do we met some combination of tags.
 
         It does not accumulate all data in memory.
         Keeps calculated metrics only.
 
         categories: [Category('a'), Category(b)]
         combinations: e.g. [(a,),(a,b)].  You can put metric objects or metrics names.
```

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3534 3130 3332 3134 3337 0a53 756d 6d61  5410321437.Summa
+00000040: 3535 3034 3834 3231 3038 0a53 756d 6d61  5504842108.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

