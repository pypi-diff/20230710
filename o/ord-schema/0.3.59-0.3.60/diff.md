# Comparing `tmp/ord-schema-0.3.59.tar.gz` & `tmp/ord-schema-0.3.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.59.tar", last modified: Sat Jul  8 23:12:02 2023, max compression
+gzip compressed data, was "ord-schema-0.3.60.tar", last modified: Mon Jul 10 14:10:55 2023, max compression
```

## Comparing `ord-schema-0.3.59.tar` & `ord-schema-0.3.60.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.889325 ord-schema-0.3.59/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-08 23:11:37.000000 ord-schema-0.3.59/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 23:11:37.000000 ord-schema-0.3.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 23:11:37.000000 ord-schema-0.3.59/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-08 23:12:02.889325 ord-schema-0.3.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 23:11:37.000000 ord-schema-0.3.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.877325 ord-schema-0.3.59/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.881325 ord-schema-0.3.59/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.881325 ord-schema-0.3.59/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.881325 ord-schema-0.3.59/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49139 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.889325 ord-schema-0.3.59/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45196 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-08 23:11:37.000000 ord-schema-0.3.59/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.877325 ord-schema-0.3.59/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 23:12:02.000000 ord-schema-0.3.59/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:12:02.889325 ord-schema-0.3.59/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-08 23:11:37.000000 ord-schema-0.3.59/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (123)    46287 2023-07-08 23:11:37.000000 ord-schema-0.3.59/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-08 23:11:37.000000 ord-schema-0.3.59/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-08 23:11:37.000000 ord-schema-0.3.59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:12:02.889325 ord-schema-0.3.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-08 23:11:41.000000 ord-schema-0.3.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.092354 ord-schema-0.3.60/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-10 14:10:26.000000 ord-schema-0.3.60/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 14:10:26.000000 ord-schema-0.3.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 14:10:26.000000 ord-schema-0.3.60/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-10 14:10:55.092354 ord-schema-0.3.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-10 14:10:26.000000 ord-schema-0.3.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.076354 ord-schema-0.3.60/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.080354 ord-schema-0.3.60/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36155 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.084354 ord-schema-0.3.60/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.084354 ord-schema-0.3.60/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49196 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.088354 ord-schema-0.3.60/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45675 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-07-10 14:10:26.000000 ord-schema-0.3.60/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.080354 ord-schema-0.3.60/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 14:10:55.000000 ord-schema-0.3.60/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:55.092354 ord-schema-0.3.60/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-10 14:10:26.000000 ord-schema-0.3.60/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-07-10 14:10:26.000000 ord-schema-0.3.60/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-10 14:10:26.000000 ord-schema-0.3.60/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-10 14:10:26.000000 ord-schema-0.3.60/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:10:55.092354 ord-schema-0.3.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-10 14:10:32.000000 ord-schema-0.3.60/setup.py
```

### Comparing `ord-schema-0.3.59/LICENSE` & `ord-schema-0.3.60/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/PKG-INFO` & `ord-schema-0.3.60/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.59
+Version: 0.3.60
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -51,7 +51,24 @@
 $ git clone https://github.com/open-reaction-database/ord-schema.git
 $ cd ord-schema
 $ pip install -e .
 ```
 
 If you make changes to the protocol buffer definitions, [install](https://grpc.io/docs/protoc-installation/) `protoc`
 and run `./compile_proto_wrappers.sh` to rebuild the wrappers.
+
+## Conventions
+
+### 1. convention: compound stoichiometry
+
+##### Created: 2023.07.04
+
+##### Last updated: 2023.07.04
+
+##### Description: 
+1. The preferred field for compound stoichiometry is the map `Compound.features` or `ProductCompound.features`.
+2. The key should be "stoichiometric_coefficient" or "stoichiometric_ratio".
+3. The value should be a Data mesaage with its float_value representing the compound's stoichiometric coefficient or ratio.SInformation about also put stoichiometry ratio/coefficient here
+
+##### Related links: 
+[#683](https://github.com/open-reaction-database/ord-schema/issues/683) 
+[#684](https://github.com/open-reaction-database/ord-schema/pull/684)
```

### Comparing `ord-schema-0.3.59/README.md` & `ord-schema-0.3.60/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -35,7 +35,24 @@
 $ git clone https://github.com/open-reaction-database/ord-schema.git
 $ cd ord-schema
 $ pip install -e .
 ```
 
 If you make changes to the protocol buffer definitions, [install](https://grpc.io/docs/protoc-installation/) `protoc`
 and run `./compile_proto_wrappers.sh` to rebuild the wrappers.
+
+## Conventions
+
+### 1. convention: compound stoichiometry
+
+##### Created: 2023.07.04
+
+##### Last updated: 2023.07.04
+
+##### Description: 
+1. The preferred field for compound stoichiometry is the map `Compound.features` or `ProductCompound.features`.
+2. The key should be "stoichiometric_coefficient" or "stoichiometric_ratio".
+3. The value should be a Data mesaage with its float_value representing the compound's stoichiometric coefficient or ratio.SInformation about also put stoichiometry ratio/coefficient here
+
+##### Related links: 
+[#683](https://github.com/open-reaction-database/ord-schema/issues/683) 
+[#684](https://github.com/open-reaction-database/ord-schema/pull/684)
```

### Comparing `ord-schema-0.3.59/ord_schema/__init__.py` & `ord-schema-0.3.60/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/frozen_message.py` & `ord-schema-0.3.60/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/frozen_message_test.py` & `ord-schema-0.3.60/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/logging.py` & `ord-schema-0.3.60/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/macros/__init__.py` & `ord-schema-0.3.60/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/macros/solutions.py` & `ord-schema-0.3.60/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.60/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/macros/workups.py` & `ord-schema-0.3.60/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/message_helpers.py` & `ord-schema-0.3.60/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/message_helpers_test.py` & `ord-schema-0.3.60/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/__init__.py` & `ord-schema-0.3.60/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/conftest.py` & `ord-schema-0.3.60/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/database.py` & `ord-schema-0.3.60/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/database_test.py` & `ord-schema-0.3.60/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/mappers.py` & `ord-schema-0.3.60/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.60/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.60/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.60/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/proto/__init__.py` & `ord-schema-0.3.60/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.60/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.60/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.60/ord_schema/proto/reaction_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ford-schema/proto/reaction.proto\x12\x03ord\"\xd9\x03\n\x08Reaction\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.ReactionIdentifier\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x19.ord.Reaction.InputsEntry\x12!\n\x05setup\x18\x03 \x01(\x0b\x32\x12.ord.ReactionSetup\x12+\n\nconditions\x18\x04 \x01(\x0b\x32\x17.ord.ReactionConditions\x12!\n\x05notes\x18\x05 \x01(\x0b\x32\x12.ord.ReactionNotes\x12.\n\x0cobservations\x18\x06 \x03(\x0b\x32\x18.ord.ReactionObservation\x12$\n\x07workups\x18\x07 \x03(\x0b\x32\x13.ord.ReactionWorkup\x12&\n\x08outcomes\x18\x08 \x03(\x0b\x32\x14.ord.ReactionOutcome\x12+\n\nprovenance\x18\t \x01(\x0b\x32\x17.ord.ReactionProvenance\x12\x13\n\x0breaction_id\x18\n \x01(\t\x1a\x41\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.ord.ReactionInput:\x02\x38\x01\"\xa7\x02\n\x12ReactionIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.ReactionIdentifier.ReactionIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x16\n\tis_mapped\x18\x04 \x01(\x08H\x00\x88\x01\x01\"\x8c\x01\n\x16ReactionIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x13\n\x0fREACTION_SMILES\x10\x02\x12\x15\n\x11REACTION_CXSMILES\x10\x06\x12\n\n\x06RDFILE\x10\x03\x12\n\n\x06RINCHI\x10\x04\x12\x11\n\rREACTION_TYPE\x10\x05\x42\x0c\n\n_is_mapped\"\xbc\x06\n\rReactionInput\x12!\n\ncomponents\x18\x01 \x03(\x0b\x32\r.ord.Compound\x12-\n\x10\x63rude_components\x18\x02 \x03(\x0b\x32\x13.ord.CrudeComponent\x12\x16\n\x0e\x61\x64\x64ition_order\x18\x03 \x01(\x05\x12 \n\raddition_time\x18\x04 \x01(\x0b\x32\t.ord.Time\x12\x38\n\x0e\x61\x64\x64ition_speed\x18\x05 \x01(\x0b\x32 .ord.ReactionInput.AdditionSpeed\x12$\n\x11\x61\x64\x64ition_duration\x18\x06 \x01(\x0b\x32\t.ord.Time\x12 \n\tflow_rate\x18\x07 \x01(\x0b\x32\r.ord.FlowRate\x12:\n\x0f\x61\x64\x64ition_device\x18\x08 \x01(\x0b\x32!.ord.ReactionInput.AdditionDevice\x12.\n\x14\x61\x64\x64ition_temperature\x18\t \x01(\x0b\x32\x10.ord.Temperature\x1a\xdc\x01\n\rAdditionSpeed\x12@\n\x04type\x18\x01 \x01(\x0e\x32\x32.ord.ReactionInput.AdditionSpeed.AdditionSpeedType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"x\n\x11\x41\x64\x64itionSpeedType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0f\n\x0b\x41LL_AT_ONCE\x10\x01\x12\x08\n\x04\x46\x41ST\x10\x02\x12\x08\n\x04SLOW\x10\x03\x12\x0c\n\x08\x44ROPWISE\x10\x04\x12\x0e\n\nCONTINUOUS\x10\x05\x12\x0f\n\x0bPORTIONWISE\x10\x06\x1a\xd1\x01\n\x0e\x41\x64\x64itionDevice\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ReactionInput.AdditionDevice.AdditionDeviceType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"j\n\x12\x41\x64\x64itionDeviceType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0b\n\x07SYRINGE\x10\x03\x12\x0b\n\x07\x43\x41NNULA\x10\x04\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\x05\"\xd6\x01\n\x06\x41mount\x12\x19\n\x04mass\x18\x01 \x01(\x0b\x32\t.ord.MassH\x00\x12\x1b\n\x05moles\x18\x02 \x01(\x0b\x32\n.ord.MolesH\x00\x12\x1d\n\x06volume\x18\x03 \x01(\x0b\x32\x0b.ord.VolumeH\x00\x12+\n\nunmeasured\x18\x05 \x01(\x0b\x32\x15.ord.UnmeasuredAmountH\x00\x12$\n\x17volume_includes_solutes\x18\x04 \x01(\x08H\x01\x88\x01\x01\x42\x06\n\x04kindB\x1a\n\x18_volume_includes_solutes\"\xbe\x01\n\x10UnmeasuredAmount\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.UnmeasuredAmount.UnmeasuredAmountType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"_\n\x14UnmeasuredAmountType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tSATURATED\x10\x02\x12\r\n\tCATALYTIC\x10\x03\x12\x0c\n\x08TITRATED\x10\x04\"\xac\x01\n\x0e\x43rudeComponent\x12\x13\n\x0breaction_id\x18\x01 \x01(\t\x12\x1c\n\x0fincludes_workup\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1f\n\x12has_derived_amount\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x1b\n\x06\x61mount\x18\x04 \x01(\x0b\x32\x0b.ord.AmountB\x12\n\x10_includes_workupB\x15\n\x13_has_derived_amount\"\xa5\x04\n\x08\x43ompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1b\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x0b.ord.Amount\x12\x39\n\rreaction_role\x18\x03 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x12\x18\n\x0bis_limiting\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12.\n\x0cpreparations\x18\x05 \x03(\x0b\x32\x18.ord.CompoundPreparation\x12$\n\x06source\x18\x06 \x01(\x0b\x32\x14.ord.Compound.Source\x12-\n\x08\x66\x65\x61tures\x18\x07 \x03(\x0b\x32\x1b.ord.Compound.FeaturesEntry\x12-\n\x08\x61nalyses\x18\x08 \x03(\x0b\x32\x1b.ord.Compound.AnalysesEntry\x1a\x39\n\x06Source\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\x12\n\ncatalog_id\x18\x02 \x01(\t\x12\x0b\n\x03lot\x18\x03 \x01(\t\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\x42\x0e\n\x0c_is_limiting\"\xb2\x01\n\x0cReactionRole\"\xa1\x01\n\x10ReactionRoleType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08REACTANT\x10\x01\x12\x0b\n\x07REAGENT\x10\x02\x12\x0b\n\x07SOLVENT\x10\x03\x12\x0c\n\x08\x43\x41TALYST\x10\x04\x12\n\n\x06WORKUP\x10\x05\x12\x15\n\x11INTERNAL_STANDARD\x10\x06\x12\x16\n\x12\x41UTHENTIC_STANDARD\x10\x07\x12\x0b\n\x07PRODUCT\x10\x08\"\xf6\x01\n\x13\x43ompoundPreparation\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.ord.CompoundPreparation.CompoundPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x13\n\x0breaction_id\x18\x03 \x01(\t\"y\n\x17\x43ompoundPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nREPURIFIED\x10\x03\x12\x0b\n\x07SPARGED\x10\x04\x12\t\n\x05\x44RIED\x10\x05\x12\x0f\n\x0bSYNTHESIZED\x10\x06\"\x82\x03\n\x12\x43ompoundIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.CompoundIdentifier.CompoundIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x8d\x02\n\x16\x43ompoundIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06SMILES\x10\x02\x12\t\n\x05INCHI\x10\x03\x12\x0c\n\x08MOLBLOCK\x10\x04\x12\x0e\n\nIUPAC_NAME\x10\x05\x12\x08\n\x04NAME\x10\x06\x12\x0e\n\nCAS_NUMBER\x10\x07\x12\x0f\n\x0bPUBCHEM_CID\x10\x08\x12\x11\n\rCHEMSPIDER_ID\x10\t\x12\x0c\n\x08\x43XSMILES\x10\n\x12\r\n\tINCHI_KEY\x10\x0b\x12\x07\n\x03XYZ\x10\x0c\x12\x0e\n\nUNIPROT_ID\x10\r\x12\n\n\x06PDB_ID\x10\x0e\x12\x17\n\x13\x41MINO_ACID_SEQUENCE\x10\x0f\x12\x08\n\x04HELM\x10\x10\"\xa7\x04\n\x06Vessel\x12$\n\x04type\x18\x01 \x01(\x0e\x32\x16.ord.Vessel.VesselType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12%\n\x08material\x18\x03 \x01(\x0b\x32\x13.ord.VesselMaterial\x12,\n\x0cpreparations\x18\x04 \x03(\x0b\x32\x16.ord.VesselPreparation\x12*\n\x0b\x61ttachments\x18\x05 \x03(\x0b\x32\x15.ord.VesselAttachment\x12\x1b\n\x06volume\x18\x06 \x01(\x0b\x32\x0b.ord.Volume\x12\x11\n\tvessel_id\x18\x07 \x01(\t\x12\x10\n\x08position\x18\x08 \x01(\t\x12\x0b\n\x03row\x18\t \x01(\t\x12\x0b\n\x03\x63ol\x18\n \x01(\t\"\x88\x02\n\nVesselType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x16\n\x12ROUND_BOTTOM_FLASK\x10\x02\x12\x08\n\x04VIAL\x10\x03\x12\x0e\n\nWELL_PLATE\x10\x04\x12\x12\n\x0eMICROWAVE_VIAL\x10\x05\x12\x08\n\x04TUBE\x10\x06\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x07\x12\x16\n\x12PACKED_BED_REACTOR\x10\x08\x12\x0c\n\x08NMR_TUBE\x10\t\x12\x12\n\x0ePRESSURE_FLASK\x10\n\x12\x14\n\x10PRESSURE_REACTOR\x10\x0b\x12\x18\n\x14\x45LECTROCHEMICAL_CELL\x10\x0c\"\xcc\x01\n\x0eVesselMaterial\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.VesselMaterial.VesselMaterialType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"s\n\x12VesselMaterialType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05GLASS\x10\x02\x12\x11\n\rPOLYPROPYLENE\x10\x03\x12\x0b\n\x07PLASTIC\x10\x04\x12\t\n\x05METAL\x10\x05\x12\n\n\x06QUARTZ\x10\x06\"\x97\x03\n\x10VesselAttachment\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.VesselAttachment.VesselAttachmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xb7\x02\n\x14VesselAttachmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\n\n\x06SEPTUM\x10\x03\x12\x07\n\x03\x43\x41P\x10\x04\x12\x07\n\x03MAT\x10\x05\x12\x14\n\x10REFLUX_CONDENSER\x10\x06\x12\x0f\n\x0bVENT_NEEDLE\x10\x07\x12\x0e\n\nDEAN_STARK\x10\x08\x12\x0f\n\x0bVACUUM_TUBE\x10\t\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\n\x12\x0f\n\x0b\x44RYING_TUBE\x10\x0b\x12\x11\n\rALUMINUM_FOIL\x10\x0c\x12\x10\n\x0cTHERMOCOUPLE\x10\r\x12\x0b\n\x07\x42\x41LLOON\x10\x0e\x12\x0f\n\x0bGAS_ADAPTER\x10\x0f\x12\x16\n\x12PRESSURE_REGULATOR\x10\x10\x12\x11\n\rRELEASE_VALVE\x10\x11\"\xe8\x01\n\x11VesselPreparation\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.VesselPreparation.VesselPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x85\x01\n\x15VesselPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nOVEN_DRIED\x10\x03\x12\x0f\n\x0b\x46LAME_DRIED\x10\x04\x12\x18\n\x14\x45VACUATED_BACKFILLED\x10\x05\x12\n\n\x06PURGED\x10\x06\"\xa0\x04\n\rReactionSetup\x12\x1b\n\x06vessel\x18\x01 \x01(\x0b\x32\x0b.ord.Vessel\x12\x19\n\x0cis_automated\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1b\n\x13\x61utomation_platform\x18\x03 \x01(\t\x12?\n\x0f\x61utomation_code\x18\x04 \x03(\x0b\x32&.ord.ReactionSetup.AutomationCodeEntry\x12;\n\x0b\x65nvironment\x18\x05 \x01(\x0b\x32&.ord.ReactionSetup.ReactionEnvironment\x1a@\n\x13\x41utomationCodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a\xe8\x01\n\x13ReactionEnvironment\x12L\n\x04type\x18\x01 \x01(\x0e\x32>.ord.ReactionSetup.ReactionEnvironment.ReactionEnvironmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"r\n\x17ReactionEnvironmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tFUME_HOOD\x10\x02\x12\r\n\tBENCH_TOP\x10\x03\x12\r\n\tGLOVE_BOX\x10\x04\x12\r\n\tGLOVE_BAG\x10\x05\x42\x0f\n\r_is_automated\"\xb5\x03\n\x12ReactionConditions\x12/\n\x0btemperature\x18\x01 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12)\n\x08pressure\x18\x02 \x01(\x0b\x32\x17.ord.PressureConditions\x12)\n\x08stirring\x18\x03 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x31\n\x0cillumination\x18\x04 \x01(\x0b\x32\x1b.ord.IlluminationConditions\x12\x39\n\x10\x65lectrochemistry\x18\x05 \x01(\x0b\x32\x1f.ord.ElectrochemistryConditions\x12!\n\x04\x66low\x18\x06 \x01(\x0b\x32\x13.ord.FlowConditions\x12\x13\n\x06reflux\x18\x07 \x01(\x08H\x00\x88\x01\x01\x12\x0f\n\x02ph\x18\x08 \x01(\x02H\x01\x88\x01\x01\x12#\n\x16\x63onditions_are_dynamic\x18\t \x01(\x08H\x02\x88\x01\x01\x12\x0f\n\x07\x64\x65tails\x18\n \x01(\tB\t\n\x07_refluxB\x05\n\x03_phB\x19\n\x17_conditions_are_dynamic\"\xe2\x06\n\x15TemperatureConditions\x12>\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32-.ord.TemperatureConditions.TemperatureControl\x12\"\n\x08setpoint\x18\x02 \x01(\x0b\x32\x10.ord.Temperature\x12G\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x31.ord.TemperatureConditions.TemperatureMeasurement\x1a\xd4\x02\n\x12TemperatureControl\x12R\n\x04type\x18\x01 \x01(\x0e\x32\x44.ord.TemperatureConditions.TemperatureControl.TemperatureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd8\x01\n\x16TemperatureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x0c\n\x08OIL_BATH\x10\x03\x12\x0e\n\nWATER_BATH\x10\x04\x12\r\n\tSAND_BATH\x10\x05\x12\x0c\n\x08ICE_BATH\x10\x06\x12\x16\n\x12\x44RY_ALUMINUM_PLATE\x10\x07\x12\r\n\tMICROWAVE\x10\x08\x12\x10\n\x0c\x44RY_ICE_BATH\x10\t\x12\x0b\n\x07\x41IR_FAN\x10\n\x12\x13\n\x0fLIQUID_NITROGEN\x10\x0b\x1a\xc4\x02\n\x16TemperatureMeasurement\x12Z\n\x04type\x18\x01 \x01(\x0e\x32L.ord.TemperatureConditions.TemperatureMeasurement.TemperatureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12%\n\x0btemperature\x18\x04 \x01(\x0b\x32\x10.ord.Temperature\"}\n\x1aTemperatureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x19\n\x15THERMOCOUPLE_INTERNAL\x10\x02\x12\x19\n\x15THERMOCOUPLE_EXTERNAL\x10\x03\x12\x0c\n\x08INFRARED\x10\x04\"\x8c\x08\n\x12PressureConditions\x12\x38\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32\'.ord.PressureConditions.PressureControl\x12\x1f\n\x08setpoint\x18\x02 \x01(\x0b\x32\r.ord.Pressure\x12\x36\n\natmosphere\x18\x03 \x01(\x0b\x32\".ord.PressureConditions.Atmosphere\x12\x41\n\x0cmeasurements\x18\x04 \x03(\x0b\x32+.ord.PressureConditions.PressureMeasurement\x1a\xe0\x01\n\x0fPressureControl\x12I\n\x04type\x18\x01 \x01(\x0e\x32;.ord.PressureConditions.PressureControl.PressureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"q\n\x13PressureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x13\n\x0fSLIGHT_POSITIVE\x10\x03\x12\n\n\x06SEALED\x10\x04\x12\x0f\n\x0bPRESSURIZED\x10\x05\x1a\xb5\x02\n\nAtmosphere\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.ord.PressureConditions.Atmosphere.AtmosphereType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd4\x01\n\x0e\x41tmosphereType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03\x41IR\x10\x02\x12\x0c\n\x08NITROGEN\x10\x03\x12\t\n\x05\x41RGON\x10\x04\x12\n\n\x06OXYGEN\x10\x05\x12\x0c\n\x08HYDROGEN\x10\x06\x12\x13\n\x0f\x43\x41RBON_MONOXIDE\x10\x07\x12\x12\n\x0e\x43\x41RBON_DIOXIDE\x10\x08\x12\x0b\n\x07METHANE\x10\t\x12\x0b\n\x07\x41MMONIA\x10\n\x12\t\n\x05OZONE\x10\x0b\x12\x0c\n\x08\x45THYLENE\x10\x0c\x12\r\n\tACETYLENE\x10\r\x1a\x84\x02\n\x13PressureMeasurement\x12Q\n\x04type\x18\x01 \x01(\x0e\x32\x43.ord.PressureConditions.PressureMeasurement.PressureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12\x1f\n\x08pressure\x18\x04 \x01(\x0b\x32\r.ord.Pressure\"O\n\x17PressureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x17\n\x13PRESSURE_TRANSDUCER\x10\x02\"\xdc\x03\n\x12StirringConditions\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.StirringConditions.StirringMethodType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x32\n\x04rate\x18\x03 \x01(\x0b\x32$.ord.StirringConditions.StirringRate\x1a\xb5\x01\n\x0cStirringRate\x12\x43\n\x04type\x18\x01 \x01(\x0e\x32\x35.ord.StirringConditions.StirringRate.StirringRateType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0b\n\x03rpm\x18\x03 \x01(\x05\"B\n\x10StirringRateType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04HIGH\x10\x01\x12\n\n\x06MEDIUM\x10\x02\x12\x07\n\x03LOW\x10\x03\"\x8e\x01\n\x12StirringMethodType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0c\n\x08STIR_BAR\x10\x03\x12\x12\n\x0eOVERHEAD_MIXER\x10\x04\x12\r\n\tAGITATION\x10\x05\x12\x10\n\x0c\x42\x41LL_MILLING\x10\x06\x12\x0e\n\nSONICATION\x10\x07\"\xe8\x02\n\x16IlluminationConditions\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.IlluminationConditions.IlluminationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12(\n\x0fpeak_wavelength\x18\x03 \x01(\x0b\x32\x0f.ord.Wavelength\x12\r\n\x05\x63olor\x18\x04 \x01(\t\x12\'\n\x12\x64istance_to_vessel\x18\x05 \x01(\x0b\x32\x0b.ord.Length\"\x9e\x01\n\x10IlluminationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x08\n\x04\x44\x41RK\x10\x03\x12\x07\n\x03LED\x10\x04\x12\x10\n\x0cHALOGEN_LAMP\x10\x05\x12\x12\n\x0e\x44\x45UTERIUM_LAMP\x10\x06\x12\x13\n\x0fSOLAR_SIMULATOR\x10\x07\x12\x12\n\x0e\x42ROAD_SPECTRUM\x10\x08\"\xe0\x06\n\x1a\x45lectrochemistryConditions\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x07\x63urrent\x18\x03 \x01(\x0b\x32\x0c.ord.Current\x12\x1d\n\x07voltage\x18\x04 \x01(\x0b\x32\x0c.ord.Voltage\x12\x16\n\x0e\x61node_material\x18\x05 \x01(\t\x12\x18\n\x10\x63\x61thode_material\x18\x06 \x01(\t\x12)\n\x14\x65lectrode_separation\x18\x07 \x01(\x0b\x32\x0b.ord.Length\x12Q\n\x0cmeasurements\x18\x08 \x03(\x0b\x32;.ord.ElectrochemistryConditions.ElectrochemistryMeasurement\x12\x42\n\x04\x63\x65ll\x18\t \x01(\x0b\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryCell\x1at\n\x1b\x45lectrochemistryMeasurement\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x1d\n\x07\x63urrent\x18\x02 \x01(\x0b\x32\x0c.ord.Current\x12\x1d\n\x07voltage\x18\x03 \x01(\x0b\x32\x0c.ord.Voltage\x1a\xe3\x01\n\x14\x45lectrochemistryCell\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.ord.ElectrochemistryConditions.ElectrochemistryCell.ElectrochemistryCellType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"]\n\x18\x45lectrochemistryCellType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x10\n\x0c\x44IVIDED_CELL\x10\x02\x12\x12\n\x0eUNDIVIDED_CELL\x10\x03\"_\n\x14\x45lectrochemistryType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x14\n\x10\x43ONSTANT_CURRENT\x10\x02\x12\x14\n\x10\x43ONSTANT_VOLTAGE\x10\x03\"\x94\x04\n\x0e\x46lowConditions\x12*\n\x04type\x18\x01 \x01(\x0e\x32\x1c.ord.FlowConditions.FlowType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x11\n\tpump_type\x18\x03 \x01(\t\x12*\n\x06tubing\x18\x04 \x01(\x0b\x32\x1a.ord.FlowConditions.Tubing\x1a\x88\x02\n\x06Tubing\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.ord.FlowConditions.Tubing.TubingType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x08\x64iameter\x18\x03 \x01(\x0b\x32\x0b.ord.Length\"\x98\x01\n\nTubingType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05STEEL\x10\x02\x12\n\n\x06\x43OPPER\x10\x03\x12\x07\n\x03PFA\x10\x04\x12\x07\n\x03\x46\x45P\x10\x05\x12\x0c\n\x08TEFLONAF\x10\x06\x12\x08\n\x04PTFE\x10\x07\x12\t\n\x05GLASS\x10\x08\x12\n\n\x06QUARTZ\x10\t\x12\x0b\n\x07SILICON\x10\n\x12\x08\n\x04PDMS\x10\x0b\"{\n\x08\x46lowType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x15\n\x11PLUG_FLOW_REACTOR\x10\x02\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x03\x12\x16\n\x12PACKED_BED_REACTOR\x10\x04\"\xc0\x03\n\rReactionNotes\x12\x1d\n\x10is_heterogeneous\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x1e\n\x11\x66orms_precipitate\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_exothermic\x18\x03 \x01(\x08H\x02\x88\x01\x01\x12\x16\n\toffgasses\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12%\n\x18is_sensitive_to_moisture\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12#\n\x16is_sensitive_to_oxygen\x18\x06 \x01(\x08H\x05\x88\x01\x01\x12\"\n\x15is_sensitive_to_light\x18\x07 \x01(\x08H\x06\x88\x01\x01\x12\x14\n\x0csafety_notes\x18\x08 \x01(\t\x12\x19\n\x11procedure_details\x18\t \x01(\tB\x13\n\x11_is_heterogeneousB\x14\n\x12_forms_precipitateB\x10\n\x0e_is_exothermicB\x0c\n\n_offgassesB\x1b\n\x19_is_sensitive_to_moistureB\x19\n\x17_is_sensitive_to_oxygenB\x18\n\x16_is_sensitive_to_light\"Y\n\x13ReactionObservation\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x0f\n\x07\x63omment\x18\x02 \x01(\t\x12\x18\n\x05image\x18\x03 \x01(\x0b\x32\t.ord.Data\"\xcb\x05\n\x0eReactionWorkup\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.ReactionWorkup.ReactionWorkupType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.ord.Time\x12!\n\x05input\x18\x04 \x01(\x0b\x32\x12.ord.ReactionInput\x12\x1b\n\x06\x61mount\x18\x05 \x01(\x0b\x32\x0b.ord.Amount\x12/\n\x0btemperature\x18\x06 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12\x12\n\nkeep_phase\x18\x07 \x01(\t\x12)\n\x08stirring\x18\x08 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x16\n\ttarget_ph\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x19\n\x0cis_automated\x18\n \x01(\x08H\x01\x88\x01\x01\"\xd2\x02\n\x12ReactionWorkupType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08\x41\x44\x44ITION\x10\x02\x12\x0b\n\x07\x41LIQUOT\x10\x03\x12\x0f\n\x0bTEMPERATURE\x10\x04\x12\x11\n\rCONCENTRATION\x10\x05\x12\x0e\n\nEXTRACTION\x10\x06\x12\x0e\n\nFILTRATION\x10\x07\x12\x08\n\x04WASH\x10\x08\x12\x11\n\rDRY_IN_VACUUM\x10\t\x12\x15\n\x11\x44RY_WITH_MATERIAL\x10\n\x12\x18\n\x14\x46LASH_CHROMATOGRAPHY\x10\x0b\x12\x18\n\x14OTHER_CHROMATOGRAPHY\x10\x0c\x12\x0e\n\nSCAVENGING\x10\r\x12\x08\n\x04WAIT\x10\x0e\x12\x0c\n\x08STIRRING\x10\x0f\x12\r\n\tPH_ADJUST\x10\x10\x12\x0f\n\x0b\x44ISSOLUTION\x10\x11\x12\x10\n\x0c\x44ISTILLATION\x10\x12\x42\x0c\n\n_target_phB\x0f\n\r_is_automated\"\xf6\x01\n\x0fReactionOutcome\x12 \n\rreaction_time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12#\n\nconversion\x18\x02 \x01(\x0b\x32\x0f.ord.Percentage\x12&\n\x08products\x18\x03 \x03(\x0b\x32\x14.ord.ProductCompound\x12\x34\n\x08\x61nalyses\x18\x04 \x03(\x0b\x32\".ord.ReactionOutcome.AnalysesEntry\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\"\x8d\x05\n\x0fProductCompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1f\n\x12is_desired_product\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12-\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x17.ord.ProductMeasurement\x12\x16\n\x0eisolated_color\x18\x04 \x01(\t\x12-\n\x07texture\x18\x05 \x01(\x0b\x32\x1c.ord.ProductCompound.Texture\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".ord.ProductCompound.FeaturesEntry\x12\x39\n\rreaction_role\x18\x07 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x1a\xf0\x01\n\x07Texture\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.ord.ProductCompound.Texture.TextureType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x9b\x01\n\x0bTextureType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06POWDER\x10\x02\x12\x0b\n\x07\x43RYSTAL\x10\x03\x12\x07\n\x03OIL\x10\x04\x12\x13\n\x0f\x41MORPHOUS_SOLID\x10\x05\x12\x08\n\x04\x46OAM\x10\x06\x12\x07\n\x03WAX\x10\x07\x12\x0e\n\nSEMI_SOLID\x10\x08\x12\t\n\x05SOLID\x10\t\x12\n\n\x06LIQUID\x10\n\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x42\x15\n\x13_is_desired_product\"\xfb\n\n\x12ProductMeasurement\x12\x14\n\x0c\x61nalysis_key\x18\x01 \x01(\t\x12<\n\x04type\x18\x02 \x01(\x0e\x32..ord.ProductMeasurement.ProductMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12#\n\x16uses_internal_standard\x18\x04 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_normalized\x18\x05 \x01(\x08H\x02\x88\x01\x01\x12$\n\x17uses_authentic_standard\x18\x06 \x01(\x08H\x03\x88\x01\x01\x12)\n\x12\x61uthentic_standard\x18\x07 \x01(\x0b\x32\r.ord.Compound\x12%\n\npercentage\x18\x08 \x01(\x0b\x32\x0f.ord.PercentageH\x00\x12&\n\x0b\x66loat_value\x18\t \x01(\x0b\x32\x0f.ord.FloatValueH\x00\x12\x16\n\x0cstring_value\x18\n \x01(\tH\x00\x12\x1d\n\x06\x61mount\x18\x0b \x01(\x0b\x32\x0b.ord.AmountH\x00\x12!\n\x0eretention_time\x18\x0c \x01(\x0b\x32\t.ord.Time\x12M\n\x11mass_spec_details\x18\r \x01(\x0b\x32\x32.ord.ProductMeasurement.MassSpecMeasurementDetails\x12\x38\n\x0bselectivity\x18\x0e \x01(\x0b\x32#.ord.ProductMeasurement.Selectivity\x12#\n\nwavelength\x18\x0f \x01(\x0b\x32\x0f.ord.Wavelength\x1a\xe9\x02\n\x1aMassSpecMeasurementDetails\x12X\n\x04type\x18\x01 \x01(\x0e\x32J.ord.ProductMeasurement.MassSpecMeasurementDetails.MassSpecMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x0etic_minimum_mz\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0etic_maximum_mz\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\neic_masses\x18\x05 \x03(\x02\"l\n\x17MassSpecMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03TIC\x10\x02\x12\x10\n\x0cTIC_POSITIVE\x10\x03\x12\x10\n\x0cTIC_NEGATIVE\x10\x04\x12\x07\n\x03\x45IC\x10\x05\x42\x11\n\x0f_tic_minimum_mzB\x11\n\x0f_tic_maximum_mz\x1a\xb9\x01\n\x0bSelectivity\x12\x41\n\x04type\x18\x01 \x01(\x0e\x32\x33.ord.ProductMeasurement.Selectivity.SelectivityType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"V\n\x0fSelectivityType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02\x45\x45\x10\x02\x12\x06\n\x02\x45R\x10\x03\x12\x06\n\x02\x44R\x10\x04\x12\x06\n\x02\x45Z\x10\x05\x12\x06\n\x02ZE\x10\x06\"\x9c\x01\n\x16ProductMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08IDENTITY\x10\x02\x12\t\n\x05YIELD\x10\x03\x12\x0f\n\x0bSELECTIVITY\x10\x04\x12\n\n\x06PURITY\x10\x05\x12\x08\n\x04\x41REA\x10\x06\x12\n\n\x06\x43OUNTS\x10\x07\x12\r\n\tINTENSITY\x10\x08\x12\n\n\x06\x41MOUNT\x10\tB\x07\n\x05valueB\x19\n\x17_uses_internal_standardB\x10\n\x0e_is_normalizedB\x1a\n\x18_uses_authentic_standard\"\x19\n\x08\x44\x61teTime\x12\r\n\x05value\x18\x01 \x01(\t\"\xcc\x04\n\x08\x41nalysis\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.ord.Analysis.AnalysisType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0f\n\x07\x63hmo_id\x18\x03 \x01(\x05\x12#\n\x16is_of_isolated_species\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12%\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x17.ord.Analysis.DataEntry\x12\x1f\n\x17instrument_manufacturer\x18\x06 \x01(\t\x12\x31\n\x1ainstrument_last_calibrated\x18\x07 \x01(\x0b\x32\r.ord.DateTime\x1a\x36\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\"\x80\x02\n\x0c\x41nalysisType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02LC\x10\x02\x12\x06\n\x02GC\x10\x03\x12\x06\n\x02IR\x10\x04\x12\n\n\x06NMR_1H\x10\x05\x12\x0b\n\x07NMR_13C\x10\x06\x12\r\n\tNMR_OTHER\x10\x07\x12\x06\n\x02MP\x10\x08\x12\x06\n\x02UV\x10\t\x12\x07\n\x03TLC\x10\n\x12\x06\n\x02MS\x10\x0b\x12\x08\n\x04HRMS\x10\x0c\x12\x08\n\x04MSMS\x10\r\x12\n\n\x06WEIGHT\x10\x0e\x12\x08\n\x04LCMS\x10\x0f\x12\x08\n\x04GCMS\x10\x10\x12\x08\n\x04\x45LSD\x10\x11\x12\x06\n\x02\x43\x44\x10\x12\x12\x07\n\x03SFC\x10\x13\x12\x07\n\x03\x45PR\x10\x14\x12\x07\n\x03XRD\x10\x15\x12\t\n\x05RAMAN\x10\x16\x12\x06\n\x02\x45\x44\x10\x17\x42\x19\n\x17_is_of_isolated_species\"\xab\x03\n\x12ReactionProvenance\x12!\n\x0c\x65xperimenter\x18\x01 \x01(\x0b\x32\x0b.ord.Person\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\'\n\x10\x65xperiment_start\x18\x03 \x01(\x0b\x32\r.ord.DateTime\x12\x0b\n\x03\x64oi\x18\x04 \x01(\t\x12\x0e\n\x06patent\x18\x05 \x01(\t\x12\x17\n\x0fpublication_url\x18\x06 \x01(\t\x12(\n\x0erecord_created\x18\x07 \x01(\x0b\x32\x10.ord.RecordEvent\x12)\n\x0frecord_modified\x18\x08 \x03(\x0b\x32\x10.ord.RecordEvent\x12H\n\x11reaction_metadata\x18\t \x03(\x0b\x32-.ord.ReactionProvenance.ReactionMetadataEntry\x12\x15\n\x08is_mined\x18\n \x01(\x08H\x00\x88\x01\x01\x1a\x42\n\x15ReactionMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x42\x0b\n\t_is_mined\"\\\n\x06Person\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05orcid\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x01(\t\"X\n\x0bRecordEvent\x12\x1b\n\x04time\x18\x01 \x01(\x0b\x32\r.ord.DateTime\x12\x1b\n\x06person\x18\x02 \x01(\x0b\x32\x0b.ord.Person\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\"\xb5\x01\n\x04Time\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Time.TimeUnit\"F\n\x08TimeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x01\x12\n\n\x06MINUTE\x10\x02\x12\n\n\x06SECOND\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc0\x01\n\x04Mass\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Mass.MassUnit\"Q\n\x08MassUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08KILOGRAM\x10\x01\x12\x08\n\x04GRAM\x10\x02\x12\r\n\tMILLIGRAM\x10\x03\x12\r\n\tMICROGRAM\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc4\x01\n\x05Moles\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12#\n\x05units\x18\x03 \x01(\x0e\x32\x14.ord.Moles.MolesUnit\"R\n\tMolesUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04MOLE\x10\x01\x12\r\n\tMILLIMOLE\x10\x02\x12\r\n\tMICROMOLE\x10\x03\x12\x0c\n\x08NANOMOLE\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcc\x01\n\x06Volume\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Volume.VolumeUnit\"W\n\nVolumeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05LITER\x10\x01\x12\x0e\n\nMILLILITER\x10\x02\x12\x0e\n\nMICROLITER\x10\x03\x12\r\n\tNANOLITER\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd9\x01\n\rConcentration\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x33\n\x05units\x18\x03 \x01(\x0e\x32$.ord.Concentration.ConcentrationUnit\"O\n\x11\x43oncentrationUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05MOLAR\x10\x01\x12\x0e\n\nMILLIMOLAR\x10\x02\x12\x0e\n\nMICROMOLAR\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xf7\x01\n\x08Pressure\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.Pressure.PressureUnit\"|\n\x0cPressureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x42\x41R\x10\x01\x12\x0e\n\nATMOSPHERE\x10\x02\x12\x07\n\x03PSI\x10\x03\x12\x08\n\x04KPSI\x10\x04\x12\n\n\x06PASCAL\x10\x05\x12\x0e\n\nKILOPASCAL\x10\x06\x12\x08\n\x04TORR\x10\x07\x12\t\n\x05MM_HG\x10\x08\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcf\x01\n\x0bTemperature\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12/\n\x05units\x18\x03 \x01(\x0e\x32 .ord.Temperature.TemperatureUnit\"K\n\x0fTemperatureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07\x43\x45LSIUS\x10\x01\x12\x0e\n\nFAHRENHEIT\x10\x02\x12\n\n\x06KELVIN\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xb3\x01\n\x07\x43urrent\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Current.CurrentUnit\";\n\x0b\x43urrentUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x41MPERE\x10\x01\x12\x0f\n\x0bMILLIAMPERE\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xaf\x01\n\x07Voltage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Voltage.VoltageUnit\"7\n\x0bVoltageUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04VOLT\x10\x01\x12\r\n\tMILLIVOLT\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd1\x01\n\x06Length\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Length.LengthUnit\"\\\n\nLengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nCENTIMETER\x10\x01\x12\x0e\n\nMILLIMETER\x10\x02\x12\t\n\x05METER\x10\x03\x12\x08\n\x04INCH\x10\x04\x12\x08\n\x04\x46OOT\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc1\x01\n\nWavelength\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12-\n\x05units\x18\x03 \x01(\x0e\x32\x1e.ord.Wavelength.WavelengthUnit\"@\n\x0eWavelengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\r\n\tNANOMETER\x10\x01\x12\x0e\n\nWAVENUMBER\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa0\x02\n\x08\x46lowRate\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.FlowRate.FlowRateUnit\"\xa4\x01\n\x0c\x46lowRateUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x19\n\x15MICROLITER_PER_MINUTE\x10\x01\x12\x19\n\x15MICROLITER_PER_SECOND\x10\x02\x12\x19\n\x15MILLILITER_PER_MINUTE\x10\x03\x12\x19\n\x15MILLILITER_PER_SECOND\x10\x04\x12\x17\n\x13MICROLITER_PER_HOUR\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nPercentage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nFloatValue\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa1\x01\n\x04\x44\x61ta\x12\x15\n\x0b\x66loat_value\x18\x01 \x01(\x02H\x00\x12\x17\n\rinteger_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x62ytes_value\x18\x03 \x01(\x0cH\x00\x12\x16\n\x0cstring_value\x18\x04 \x01(\tH\x00\x12\r\n\x03url\x18\x05 \x01(\tH\x00\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\tB\x06\n\x04kindb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ford-schema/proto/reaction.proto\x12\x03ord\"\xd9\x03\n\x08Reaction\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.ReactionIdentifier\x12)\n\x06inputs\x18\x02 \x03(\x0b\x32\x19.ord.Reaction.InputsEntry\x12!\n\x05setup\x18\x03 \x01(\x0b\x32\x12.ord.ReactionSetup\x12+\n\nconditions\x18\x04 \x01(\x0b\x32\x17.ord.ReactionConditions\x12!\n\x05notes\x18\x05 \x01(\x0b\x32\x12.ord.ReactionNotes\x12.\n\x0cobservations\x18\x06 \x03(\x0b\x32\x18.ord.ReactionObservation\x12$\n\x07workups\x18\x07 \x03(\x0b\x32\x13.ord.ReactionWorkup\x12&\n\x08outcomes\x18\x08 \x03(\x0b\x32\x14.ord.ReactionOutcome\x12+\n\nprovenance\x18\t \x01(\x0b\x32\x17.ord.ReactionProvenance\x12\x13\n\x0breaction_id\x18\n \x01(\t\x1a\x41\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.ord.ReactionInput:\x02\x38\x01\"\xa7\x02\n\x12ReactionIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.ReactionIdentifier.ReactionIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x16\n\tis_mapped\x18\x04 \x01(\x08H\x00\x88\x01\x01\"\x8c\x01\n\x16ReactionIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x13\n\x0fREACTION_SMILES\x10\x02\x12\x15\n\x11REACTION_CXSMILES\x10\x06\x12\n\n\x06RDFILE\x10\x03\x12\n\n\x06RINCHI\x10\x04\x12\x11\n\rREACTION_TYPE\x10\x05\x42\x0c\n\n_is_mapped\"\xbc\x06\n\rReactionInput\x12!\n\ncomponents\x18\x01 \x03(\x0b\x32\r.ord.Compound\x12-\n\x10\x63rude_components\x18\x02 \x03(\x0b\x32\x13.ord.CrudeComponent\x12\x16\n\x0e\x61\x64\x64ition_order\x18\x03 \x01(\x05\x12 \n\raddition_time\x18\x04 \x01(\x0b\x32\t.ord.Time\x12\x38\n\x0e\x61\x64\x64ition_speed\x18\x05 \x01(\x0b\x32 .ord.ReactionInput.AdditionSpeed\x12$\n\x11\x61\x64\x64ition_duration\x18\x06 \x01(\x0b\x32\t.ord.Time\x12 \n\tflow_rate\x18\x07 \x01(\x0b\x32\r.ord.FlowRate\x12:\n\x0f\x61\x64\x64ition_device\x18\x08 \x01(\x0b\x32!.ord.ReactionInput.AdditionDevice\x12.\n\x14\x61\x64\x64ition_temperature\x18\t \x01(\x0b\x32\x10.ord.Temperature\x1a\xdc\x01\n\rAdditionSpeed\x12@\n\x04type\x18\x01 \x01(\x0e\x32\x32.ord.ReactionInput.AdditionSpeed.AdditionSpeedType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"x\n\x11\x41\x64\x64itionSpeedType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0f\n\x0b\x41LL_AT_ONCE\x10\x01\x12\x08\n\x04\x46\x41ST\x10\x02\x12\x08\n\x04SLOW\x10\x03\x12\x0c\n\x08\x44ROPWISE\x10\x04\x12\x0e\n\nCONTINUOUS\x10\x05\x12\x0f\n\x0bPORTIONWISE\x10\x06\x1a\xd1\x01\n\x0e\x41\x64\x64itionDevice\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ReactionInput.AdditionDevice.AdditionDeviceType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"j\n\x12\x41\x64\x64itionDeviceType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0b\n\x07SYRINGE\x10\x03\x12\x0b\n\x07\x43\x41NNULA\x10\x04\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\x05\"\xd6\x01\n\x06\x41mount\x12\x19\n\x04mass\x18\x01 \x01(\x0b\x32\t.ord.MassH\x00\x12\x1b\n\x05moles\x18\x02 \x01(\x0b\x32\n.ord.MolesH\x00\x12\x1d\n\x06volume\x18\x03 \x01(\x0b\x32\x0b.ord.VolumeH\x00\x12+\n\nunmeasured\x18\x05 \x01(\x0b\x32\x15.ord.UnmeasuredAmountH\x00\x12$\n\x17volume_includes_solutes\x18\x04 \x01(\x08H\x01\x88\x01\x01\x42\x06\n\x04kindB\x1a\n\x18_volume_includes_solutes\"\xbe\x01\n\x10UnmeasuredAmount\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.UnmeasuredAmount.UnmeasuredAmountType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"_\n\x14UnmeasuredAmountType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tSATURATED\x10\x02\x12\r\n\tCATALYTIC\x10\x03\x12\x0c\n\x08TITRATED\x10\x04\"\xac\x01\n\x0e\x43rudeComponent\x12\x13\n\x0breaction_id\x18\x01 \x01(\t\x12\x1c\n\x0fincludes_workup\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1f\n\x12has_derived_amount\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x1b\n\x06\x61mount\x18\x04 \x01(\x0b\x32\x0b.ord.AmountB\x12\n\x10_includes_workupB\x15\n\x13_has_derived_amount\"\xa5\x04\n\x08\x43ompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1b\n\x06\x61mount\x18\x02 \x01(\x0b\x32\x0b.ord.Amount\x12\x39\n\rreaction_role\x18\x03 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x12\x18\n\x0bis_limiting\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12.\n\x0cpreparations\x18\x05 \x03(\x0b\x32\x18.ord.CompoundPreparation\x12$\n\x06source\x18\x06 \x01(\x0b\x32\x14.ord.Compound.Source\x12-\n\x08\x66\x65\x61tures\x18\x07 \x03(\x0b\x32\x1b.ord.Compound.FeaturesEntry\x12-\n\x08\x61nalyses\x18\x08 \x03(\x0b\x32\x1b.ord.Compound.AnalysesEntry\x1a\x39\n\x06Source\x12\x0e\n\x06vendor\x18\x01 \x01(\t\x12\x12\n\ncatalog_id\x18\x02 \x01(\t\x12\x0b\n\x03lot\x18\x03 \x01(\t\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\x42\x0e\n\x0c_is_limiting\"\xd3\x01\n\x0cReactionRole\"\xc2\x01\n\x10ReactionRoleType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08REACTANT\x10\x01\x12\x0b\n\x07REAGENT\x10\x02\x12\x0b\n\x07SOLVENT\x10\x03\x12\x0c\n\x08\x43\x41TALYST\x10\x04\x12\n\n\x06WORKUP\x10\x05\x12\x15\n\x11INTERNAL_STANDARD\x10\x06\x12\x16\n\x12\x41UTHENTIC_STANDARD\x10\x07\x12\x0b\n\x07PRODUCT\x10\x08\x12\r\n\tBYPRODUCT\x10\t\x12\x10\n\x0cSIDE_PRODUCT\x10\n\"\xf6\x01\n\x13\x43ompoundPreparation\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.ord.CompoundPreparation.CompoundPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x13\n\x0breaction_id\x18\x03 \x01(\t\"y\n\x17\x43ompoundPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nREPURIFIED\x10\x03\x12\x0b\n\x07SPARGED\x10\x04\x12\t\n\x05\x44RIED\x10\x05\x12\x0f\n\x0bSYNTHESIZED\x10\x06\"\x82\x03\n\x12\x43ompoundIdentifier\x12<\n\x04type\x18\x01 \x01(\x0e\x32..ord.CompoundIdentifier.CompoundIdentifierType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\"\x8d\x02\n\x16\x43ompoundIdentifierType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06SMILES\x10\x02\x12\t\n\x05INCHI\x10\x03\x12\x0c\n\x08MOLBLOCK\x10\x04\x12\x0e\n\nIUPAC_NAME\x10\x05\x12\x08\n\x04NAME\x10\x06\x12\x0e\n\nCAS_NUMBER\x10\x07\x12\x0f\n\x0bPUBCHEM_CID\x10\x08\x12\x11\n\rCHEMSPIDER_ID\x10\t\x12\x0c\n\x08\x43XSMILES\x10\n\x12\r\n\tINCHI_KEY\x10\x0b\x12\x07\n\x03XYZ\x10\x0c\x12\x0e\n\nUNIPROT_ID\x10\r\x12\n\n\x06PDB_ID\x10\x0e\x12\x17\n\x13\x41MINO_ACID_SEQUENCE\x10\x0f\x12\x08\n\x04HELM\x10\x10\"\xa7\x04\n\x06Vessel\x12$\n\x04type\x18\x01 \x01(\x0e\x32\x16.ord.Vessel.VesselType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12%\n\x08material\x18\x03 \x01(\x0b\x32\x13.ord.VesselMaterial\x12,\n\x0cpreparations\x18\x04 \x03(\x0b\x32\x16.ord.VesselPreparation\x12*\n\x0b\x61ttachments\x18\x05 \x03(\x0b\x32\x15.ord.VesselAttachment\x12\x1b\n\x06volume\x18\x06 \x01(\x0b\x32\x0b.ord.Volume\x12\x11\n\tvessel_id\x18\x07 \x01(\t\x12\x10\n\x08position\x18\x08 \x01(\t\x12\x0b\n\x03row\x18\t \x01(\t\x12\x0b\n\x03\x63ol\x18\n \x01(\t\"\x88\x02\n\nVesselType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x16\n\x12ROUND_BOTTOM_FLASK\x10\x02\x12\x08\n\x04VIAL\x10\x03\x12\x0e\n\nWELL_PLATE\x10\x04\x12\x12\n\x0eMICROWAVE_VIAL\x10\x05\x12\x08\n\x04TUBE\x10\x06\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x07\x12\x16\n\x12PACKED_BED_REACTOR\x10\x08\x12\x0c\n\x08NMR_TUBE\x10\t\x12\x12\n\x0ePRESSURE_FLASK\x10\n\x12\x14\n\x10PRESSURE_REACTOR\x10\x0b\x12\x18\n\x14\x45LECTROCHEMICAL_CELL\x10\x0c\"\xcc\x01\n\x0eVesselMaterial\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.VesselMaterial.VesselMaterialType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"s\n\x12VesselMaterialType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05GLASS\x10\x02\x12\x11\n\rPOLYPROPYLENE\x10\x03\x12\x0b\n\x07PLASTIC\x10\x04\x12\t\n\x05METAL\x10\x05\x12\n\n\x06QUARTZ\x10\x06\"\x97\x03\n\x10VesselAttachment\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.VesselAttachment.VesselAttachmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xb7\x02\n\x14VesselAttachmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\n\n\x06SEPTUM\x10\x03\x12\x07\n\x03\x43\x41P\x10\x04\x12\x07\n\x03MAT\x10\x05\x12\x14\n\x10REFLUX_CONDENSER\x10\x06\x12\x0f\n\x0bVENT_NEEDLE\x10\x07\x12\x0e\n\nDEAN_STARK\x10\x08\x12\x0f\n\x0bVACUUM_TUBE\x10\t\x12\x13\n\x0f\x41\x44\x44ITION_FUNNEL\x10\n\x12\x0f\n\x0b\x44RYING_TUBE\x10\x0b\x12\x11\n\rALUMINUM_FOIL\x10\x0c\x12\x10\n\x0cTHERMOCOUPLE\x10\r\x12\x0b\n\x07\x42\x41LLOON\x10\x0e\x12\x0f\n\x0bGAS_ADAPTER\x10\x0f\x12\x16\n\x12PRESSURE_REGULATOR\x10\x10\x12\x11\n\rRELEASE_VALVE\x10\x11\"\xe8\x01\n\x11VesselPreparation\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.VesselPreparation.VesselPreparationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x85\x01\n\x15VesselPreparationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0e\n\nOVEN_DRIED\x10\x03\x12\x0f\n\x0b\x46LAME_DRIED\x10\x04\x12\x18\n\x14\x45VACUATED_BACKFILLED\x10\x05\x12\n\n\x06PURGED\x10\x06\"\xa0\x04\n\rReactionSetup\x12\x1b\n\x06vessel\x18\x01 \x01(\x0b\x32\x0b.ord.Vessel\x12\x19\n\x0cis_automated\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1b\n\x13\x61utomation_platform\x18\x03 \x01(\t\x12?\n\x0f\x61utomation_code\x18\x04 \x03(\x0b\x32&.ord.ReactionSetup.AutomationCodeEntry\x12;\n\x0b\x65nvironment\x18\x05 \x01(\x0b\x32&.ord.ReactionSetup.ReactionEnvironment\x1a@\n\x13\x41utomationCodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x1a\xe8\x01\n\x13ReactionEnvironment\x12L\n\x04type\x18\x01 \x01(\x0e\x32>.ord.ReactionSetup.ReactionEnvironment.ReactionEnvironmentType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"r\n\x17ReactionEnvironmentType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\r\n\tFUME_HOOD\x10\x02\x12\r\n\tBENCH_TOP\x10\x03\x12\r\n\tGLOVE_BOX\x10\x04\x12\r\n\tGLOVE_BAG\x10\x05\x42\x0f\n\r_is_automated\"\xb5\x03\n\x12ReactionConditions\x12/\n\x0btemperature\x18\x01 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12)\n\x08pressure\x18\x02 \x01(\x0b\x32\x17.ord.PressureConditions\x12)\n\x08stirring\x18\x03 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x31\n\x0cillumination\x18\x04 \x01(\x0b\x32\x1b.ord.IlluminationConditions\x12\x39\n\x10\x65lectrochemistry\x18\x05 \x01(\x0b\x32\x1f.ord.ElectrochemistryConditions\x12!\n\x04\x66low\x18\x06 \x01(\x0b\x32\x13.ord.FlowConditions\x12\x13\n\x06reflux\x18\x07 \x01(\x08H\x00\x88\x01\x01\x12\x0f\n\x02ph\x18\x08 \x01(\x02H\x01\x88\x01\x01\x12#\n\x16\x63onditions_are_dynamic\x18\t \x01(\x08H\x02\x88\x01\x01\x12\x0f\n\x07\x64\x65tails\x18\n \x01(\tB\t\n\x07_refluxB\x05\n\x03_phB\x19\n\x17_conditions_are_dynamic\"\xe2\x06\n\x15TemperatureConditions\x12>\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32-.ord.TemperatureConditions.TemperatureControl\x12\"\n\x08setpoint\x18\x02 \x01(\x0b\x32\x10.ord.Temperature\x12G\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x31.ord.TemperatureConditions.TemperatureMeasurement\x1a\xd4\x02\n\x12TemperatureControl\x12R\n\x04type\x18\x01 \x01(\x0e\x32\x44.ord.TemperatureConditions.TemperatureControl.TemperatureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd8\x01\n\x16TemperatureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x0c\n\x08OIL_BATH\x10\x03\x12\x0e\n\nWATER_BATH\x10\x04\x12\r\n\tSAND_BATH\x10\x05\x12\x0c\n\x08ICE_BATH\x10\x06\x12\x16\n\x12\x44RY_ALUMINUM_PLATE\x10\x07\x12\r\n\tMICROWAVE\x10\x08\x12\x10\n\x0c\x44RY_ICE_BATH\x10\t\x12\x0b\n\x07\x41IR_FAN\x10\n\x12\x13\n\x0fLIQUID_NITROGEN\x10\x0b\x1a\xc4\x02\n\x16TemperatureMeasurement\x12Z\n\x04type\x18\x01 \x01(\x0e\x32L.ord.TemperatureConditions.TemperatureMeasurement.TemperatureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12%\n\x0btemperature\x18\x04 \x01(\x0b\x32\x10.ord.Temperature\"}\n\x1aTemperatureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x19\n\x15THERMOCOUPLE_INTERNAL\x10\x02\x12\x19\n\x15THERMOCOUPLE_EXTERNAL\x10\x03\x12\x0c\n\x08INFRARED\x10\x04\"\x8c\x08\n\x12PressureConditions\x12\x38\n\x07\x63ontrol\x18\x01 \x01(\x0b\x32\'.ord.PressureConditions.PressureControl\x12\x1f\n\x08setpoint\x18\x02 \x01(\x0b\x32\r.ord.Pressure\x12\x36\n\natmosphere\x18\x03 \x01(\x0b\x32\".ord.PressureConditions.Atmosphere\x12\x41\n\x0cmeasurements\x18\x04 \x03(\x0b\x32+.ord.PressureConditions.PressureMeasurement\x1a\xe0\x01\n\x0fPressureControl\x12I\n\x04type\x18\x01 \x01(\x0e\x32;.ord.PressureConditions.PressureControl.PressureControlType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"q\n\x13PressureControlType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x13\n\x0fSLIGHT_POSITIVE\x10\x03\x12\n\n\x06SEALED\x10\x04\x12\x0f\n\x0bPRESSURIZED\x10\x05\x1a\xb5\x02\n\nAtmosphere\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.ord.PressureConditions.Atmosphere.AtmosphereType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\xd4\x01\n\x0e\x41tmosphereType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03\x41IR\x10\x02\x12\x0c\n\x08NITROGEN\x10\x03\x12\t\n\x05\x41RGON\x10\x04\x12\n\n\x06OXYGEN\x10\x05\x12\x0c\n\x08HYDROGEN\x10\x06\x12\x13\n\x0f\x43\x41RBON_MONOXIDE\x10\x07\x12\x12\n\x0e\x43\x41RBON_DIOXIDE\x10\x08\x12\x0b\n\x07METHANE\x10\t\x12\x0b\n\x07\x41MMONIA\x10\n\x12\t\n\x05OZONE\x10\x0b\x12\x0c\n\x08\x45THYLENE\x10\x0c\x12\r\n\tACETYLENE\x10\r\x1a\x84\x02\n\x13PressureMeasurement\x12Q\n\x04type\x18\x01 \x01(\x0e\x32\x43.ord.PressureConditions.PressureMeasurement.PressureMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x17\n\x04time\x18\x03 \x01(\x0b\x32\t.ord.Time\x12\x1f\n\x08pressure\x18\x04 \x01(\x0b\x32\r.ord.Pressure\"O\n\x17PressureMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x17\n\x13PRESSURE_TRANSDUCER\x10\x02\"\xdc\x03\n\x12StirringConditions\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.ord.StirringConditions.StirringMethodType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x32\n\x04rate\x18\x03 \x01(\x0b\x32$.ord.StirringConditions.StirringRate\x1a\xb5\x01\n\x0cStirringRate\x12\x43\n\x04type\x18\x01 \x01(\x0e\x32\x35.ord.StirringConditions.StirringRate.StirringRateType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0b\n\x03rpm\x18\x03 \x01(\x05\"B\n\x10StirringRateType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04HIGH\x10\x01\x12\n\n\x06MEDIUM\x10\x02\x12\x07\n\x03LOW\x10\x03\"\x8e\x01\n\x12StirringMethodType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04NONE\x10\x02\x12\x0c\n\x08STIR_BAR\x10\x03\x12\x12\n\x0eOVERHEAD_MIXER\x10\x04\x12\r\n\tAGITATION\x10\x05\x12\x10\n\x0c\x42\x41LL_MILLING\x10\x06\x12\x0e\n\nSONICATION\x10\x07\"\xe8\x02\n\x16IlluminationConditions\x12:\n\x04type\x18\x01 \x01(\x0e\x32,.ord.IlluminationConditions.IlluminationType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12(\n\x0fpeak_wavelength\x18\x03 \x01(\x0b\x32\x0f.ord.Wavelength\x12\r\n\x05\x63olor\x18\x04 \x01(\t\x12\'\n\x12\x64istance_to_vessel\x18\x05 \x01(\x0b\x32\x0b.ord.Length\"\x9e\x01\n\x10IlluminationType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0b\n\x07\x41MBIENT\x10\x02\x12\x08\n\x04\x44\x41RK\x10\x03\x12\x07\n\x03LED\x10\x04\x12\x10\n\x0cHALOGEN_LAMP\x10\x05\x12\x12\n\x0e\x44\x45UTERIUM_LAMP\x10\x06\x12\x13\n\x0fSOLAR_SIMULATOR\x10\x07\x12\x12\n\x0e\x42ROAD_SPECTRUM\x10\x08\"\xe0\x06\n\x1a\x45lectrochemistryConditions\x12\x42\n\x04type\x18\x01 \x01(\x0e\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x07\x63urrent\x18\x03 \x01(\x0b\x32\x0c.ord.Current\x12\x1d\n\x07voltage\x18\x04 \x01(\x0b\x32\x0c.ord.Voltage\x12\x16\n\x0e\x61node_material\x18\x05 \x01(\t\x12\x18\n\x10\x63\x61thode_material\x18\x06 \x01(\t\x12)\n\x14\x65lectrode_separation\x18\x07 \x01(\x0b\x32\x0b.ord.Length\x12Q\n\x0cmeasurements\x18\x08 \x03(\x0b\x32;.ord.ElectrochemistryConditions.ElectrochemistryMeasurement\x12\x42\n\x04\x63\x65ll\x18\t \x01(\x0b\x32\x34.ord.ElectrochemistryConditions.ElectrochemistryCell\x1at\n\x1b\x45lectrochemistryMeasurement\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x1d\n\x07\x63urrent\x18\x02 \x01(\x0b\x32\x0c.ord.Current\x12\x1d\n\x07voltage\x18\x03 \x01(\x0b\x32\x0c.ord.Voltage\x1a\xe3\x01\n\x14\x45lectrochemistryCell\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.ord.ElectrochemistryConditions.ElectrochemistryCell.ElectrochemistryCellType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"]\n\x18\x45lectrochemistryCellType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x10\n\x0c\x44IVIDED_CELL\x10\x02\x12\x12\n\x0eUNDIVIDED_CELL\x10\x03\"_\n\x14\x45lectrochemistryType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x14\n\x10\x43ONSTANT_CURRENT\x10\x02\x12\x14\n\x10\x43ONSTANT_VOLTAGE\x10\x03\"\x94\x04\n\x0e\x46lowConditions\x12*\n\x04type\x18\x01 \x01(\x0e\x32\x1c.ord.FlowConditions.FlowType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x11\n\tpump_type\x18\x03 \x01(\t\x12*\n\x06tubing\x18\x04 \x01(\x0b\x32\x1a.ord.FlowConditions.Tubing\x1a\x88\x02\n\x06Tubing\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.ord.FlowConditions.Tubing.TubingType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1d\n\x08\x64iameter\x18\x03 \x01(\x0b\x32\x0b.ord.Length\"\x98\x01\n\nTubingType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\t\n\x05STEEL\x10\x02\x12\n\n\x06\x43OPPER\x10\x03\x12\x07\n\x03PFA\x10\x04\x12\x07\n\x03\x46\x45P\x10\x05\x12\x0c\n\x08TEFLONAF\x10\x06\x12\x08\n\x04PTFE\x10\x07\x12\t\n\x05GLASS\x10\x08\x12\n\n\x06QUARTZ\x10\t\x12\x0b\n\x07SILICON\x10\n\x12\x08\n\x04PDMS\x10\x0b\"{\n\x08\x46lowType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x15\n\x11PLUG_FLOW_REACTOR\x10\x02\x12#\n\x1f\x43ONTINUOUS_STIRRED_TANK_REACTOR\x10\x03\x12\x16\n\x12PACKED_BED_REACTOR\x10\x04\"\xc0\x03\n\rReactionNotes\x12\x1d\n\x10is_heterogeneous\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x1e\n\x11\x66orms_precipitate\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_exothermic\x18\x03 \x01(\x08H\x02\x88\x01\x01\x12\x16\n\toffgasses\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12%\n\x18is_sensitive_to_moisture\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12#\n\x16is_sensitive_to_oxygen\x18\x06 \x01(\x08H\x05\x88\x01\x01\x12\"\n\x15is_sensitive_to_light\x18\x07 \x01(\x08H\x06\x88\x01\x01\x12\x14\n\x0csafety_notes\x18\x08 \x01(\t\x12\x19\n\x11procedure_details\x18\t \x01(\tB\x13\n\x11_is_heterogeneousB\x14\n\x12_forms_precipitateB\x10\n\x0e_is_exothermicB\x0c\n\n_offgassesB\x1b\n\x19_is_sensitive_to_moistureB\x19\n\x17_is_sensitive_to_oxygenB\x18\n\x16_is_sensitive_to_light\"Y\n\x13ReactionObservation\x12\x17\n\x04time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12\x0f\n\x07\x63omment\x18\x02 \x01(\t\x12\x18\n\x05image\x18\x03 \x01(\x0b\x32\t.ord.Data\"\xcb\x05\n\x0eReactionWorkup\x12\x34\n\x04type\x18\x01 \x01(\x0e\x32&.ord.ReactionWorkup.ReactionWorkupType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.ord.Time\x12!\n\x05input\x18\x04 \x01(\x0b\x32\x12.ord.ReactionInput\x12\x1b\n\x06\x61mount\x18\x05 \x01(\x0b\x32\x0b.ord.Amount\x12/\n\x0btemperature\x18\x06 \x01(\x0b\x32\x1a.ord.TemperatureConditions\x12\x12\n\nkeep_phase\x18\x07 \x01(\t\x12)\n\x08stirring\x18\x08 \x01(\x0b\x32\x17.ord.StirringConditions\x12\x16\n\ttarget_ph\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x19\n\x0cis_automated\x18\n \x01(\x08H\x01\x88\x01\x01\"\xd2\x02\n\x12ReactionWorkupType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08\x41\x44\x44ITION\x10\x02\x12\x0b\n\x07\x41LIQUOT\x10\x03\x12\x0f\n\x0bTEMPERATURE\x10\x04\x12\x11\n\rCONCENTRATION\x10\x05\x12\x0e\n\nEXTRACTION\x10\x06\x12\x0e\n\nFILTRATION\x10\x07\x12\x08\n\x04WASH\x10\x08\x12\x11\n\rDRY_IN_VACUUM\x10\t\x12\x15\n\x11\x44RY_WITH_MATERIAL\x10\n\x12\x18\n\x14\x46LASH_CHROMATOGRAPHY\x10\x0b\x12\x18\n\x14OTHER_CHROMATOGRAPHY\x10\x0c\x12\x0e\n\nSCAVENGING\x10\r\x12\x08\n\x04WAIT\x10\x0e\x12\x0c\n\x08STIRRING\x10\x0f\x12\r\n\tPH_ADJUST\x10\x10\x12\x0f\n\x0b\x44ISSOLUTION\x10\x11\x12\x10\n\x0c\x44ISTILLATION\x10\x12\x42\x0c\n\n_target_phB\x0f\n\r_is_automated\"\xf6\x01\n\x0fReactionOutcome\x12 \n\rreaction_time\x18\x01 \x01(\x0b\x32\t.ord.Time\x12#\n\nconversion\x18\x02 \x01(\x0b\x32\x0f.ord.Percentage\x12&\n\x08products\x18\x03 \x03(\x0b\x32\x14.ord.ProductCompound\x12\x34\n\x08\x61nalyses\x18\x04 \x03(\x0b\x32\".ord.ReactionOutcome.AnalysesEntry\x1a>\n\rAnalysesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.ord.Analysis:\x02\x38\x01\"\x8d\x05\n\x0fProductCompound\x12,\n\x0bidentifiers\x18\x01 \x03(\x0b\x32\x17.ord.CompoundIdentifier\x12\x1f\n\x12is_desired_product\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12-\n\x0cmeasurements\x18\x03 \x03(\x0b\x32\x17.ord.ProductMeasurement\x12\x16\n\x0eisolated_color\x18\x04 \x01(\t\x12-\n\x07texture\x18\x05 \x01(\x0b\x32\x1c.ord.ProductCompound.Texture\x12\x34\n\x08\x66\x65\x61tures\x18\x06 \x03(\x0b\x32\".ord.ProductCompound.FeaturesEntry\x12\x39\n\rreaction_role\x18\x07 \x01(\x0e\x32\".ord.ReactionRole.ReactionRoleType\x1a\xf0\x01\n\x07Texture\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.ord.ProductCompound.Texture.TextureType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x9b\x01\n\x0bTextureType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\n\n\x06POWDER\x10\x02\x12\x0b\n\x07\x43RYSTAL\x10\x03\x12\x07\n\x03OIL\x10\x04\x12\x13\n\x0f\x41MORPHOUS_SOLID\x10\x05\x12\x08\n\x04\x46OAM\x10\x06\x12\x07\n\x03WAX\x10\x07\x12\x0e\n\nSEMI_SOLID\x10\x08\x12\t\n\x05SOLID\x10\t\x12\n\n\x06LIQUID\x10\n\x1a:\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x42\x15\n\x13_is_desired_product\"\xfb\n\n\x12ProductMeasurement\x12\x14\n\x0c\x61nalysis_key\x18\x01 \x01(\t\x12<\n\x04type\x18\x02 \x01(\x0e\x32..ord.ProductMeasurement.ProductMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\x12#\n\x16uses_internal_standard\x18\x04 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\ris_normalized\x18\x05 \x01(\x08H\x02\x88\x01\x01\x12$\n\x17uses_authentic_standard\x18\x06 \x01(\x08H\x03\x88\x01\x01\x12)\n\x12\x61uthentic_standard\x18\x07 \x01(\x0b\x32\r.ord.Compound\x12%\n\npercentage\x18\x08 \x01(\x0b\x32\x0f.ord.PercentageH\x00\x12&\n\x0b\x66loat_value\x18\t \x01(\x0b\x32\x0f.ord.FloatValueH\x00\x12\x16\n\x0cstring_value\x18\n \x01(\tH\x00\x12\x1d\n\x06\x61mount\x18\x0b \x01(\x0b\x32\x0b.ord.AmountH\x00\x12!\n\x0eretention_time\x18\x0c \x01(\x0b\x32\t.ord.Time\x12M\n\x11mass_spec_details\x18\r \x01(\x0b\x32\x32.ord.ProductMeasurement.MassSpecMeasurementDetails\x12\x38\n\x0bselectivity\x18\x0e \x01(\x0b\x32#.ord.ProductMeasurement.Selectivity\x12#\n\nwavelength\x18\x0f \x01(\x0b\x32\x0f.ord.Wavelength\x1a\xe9\x02\n\x1aMassSpecMeasurementDetails\x12X\n\x04type\x18\x01 \x01(\x0e\x32J.ord.ProductMeasurement.MassSpecMeasurementDetails.MassSpecMeasurementType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x1b\n\x0etic_minimum_mz\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0etic_maximum_mz\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\neic_masses\x18\x05 \x03(\x02\"l\n\x17MassSpecMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x07\n\x03TIC\x10\x02\x12\x10\n\x0cTIC_POSITIVE\x10\x03\x12\x10\n\x0cTIC_NEGATIVE\x10\x04\x12\x07\n\x03\x45IC\x10\x05\x42\x11\n\x0f_tic_minimum_mzB\x11\n\x0f_tic_maximum_mz\x1a\xb9\x01\n\x0bSelectivity\x12\x41\n\x04type\x18\x01 \x01(\x0e\x32\x33.ord.ProductMeasurement.Selectivity.SelectivityType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"V\n\x0fSelectivityType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02\x45\x45\x10\x02\x12\x06\n\x02\x45R\x10\x03\x12\x06\n\x02\x44R\x10\x04\x12\x06\n\x02\x45Z\x10\x05\x12\x06\n\x02ZE\x10\x06\"\x9c\x01\n\x16ProductMeasurementType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x0c\n\x08IDENTITY\x10\x02\x12\t\n\x05YIELD\x10\x03\x12\x0f\n\x0bSELECTIVITY\x10\x04\x12\n\n\x06PURITY\x10\x05\x12\x08\n\x04\x41REA\x10\x06\x12\n\n\x06\x43OUNTS\x10\x07\x12\r\n\tINTENSITY\x10\x08\x12\n\n\x06\x41MOUNT\x10\tB\x07\n\x05valueB\x19\n\x17_uses_internal_standardB\x10\n\x0e_is_normalizedB\x1a\n\x18_uses_authentic_standard\"\x19\n\x08\x44\x61teTime\x12\r\n\x05value\x18\x01 \x01(\t\"\xcc\x04\n\x08\x41nalysis\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.ord.Analysis.AnalysisType\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\x12\x0f\n\x07\x63hmo_id\x18\x03 \x01(\x05\x12#\n\x16is_of_isolated_species\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12%\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x17.ord.Analysis.DataEntry\x12\x1f\n\x17instrument_manufacturer\x18\x06 \x01(\t\x12\x31\n\x1ainstrument_last_calibrated\x18\x07 \x01(\x0b\x32\r.ord.DateTime\x1a\x36\n\tDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\"\x80\x02\n\x0c\x41nalysisType\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x43USTOM\x10\x01\x12\x06\n\x02LC\x10\x02\x12\x06\n\x02GC\x10\x03\x12\x06\n\x02IR\x10\x04\x12\n\n\x06NMR_1H\x10\x05\x12\x0b\n\x07NMR_13C\x10\x06\x12\r\n\tNMR_OTHER\x10\x07\x12\x06\n\x02MP\x10\x08\x12\x06\n\x02UV\x10\t\x12\x07\n\x03TLC\x10\n\x12\x06\n\x02MS\x10\x0b\x12\x08\n\x04HRMS\x10\x0c\x12\x08\n\x04MSMS\x10\r\x12\n\n\x06WEIGHT\x10\x0e\x12\x08\n\x04LCMS\x10\x0f\x12\x08\n\x04GCMS\x10\x10\x12\x08\n\x04\x45LSD\x10\x11\x12\x06\n\x02\x43\x44\x10\x12\x12\x07\n\x03SFC\x10\x13\x12\x07\n\x03\x45PR\x10\x14\x12\x07\n\x03XRD\x10\x15\x12\t\n\x05RAMAN\x10\x16\x12\x06\n\x02\x45\x44\x10\x17\x42\x19\n\x17_is_of_isolated_species\"\xab\x03\n\x12ReactionProvenance\x12!\n\x0c\x65xperimenter\x18\x01 \x01(\x0b\x32\x0b.ord.Person\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\'\n\x10\x65xperiment_start\x18\x03 \x01(\x0b\x32\r.ord.DateTime\x12\x0b\n\x03\x64oi\x18\x04 \x01(\t\x12\x0e\n\x06patent\x18\x05 \x01(\t\x12\x17\n\x0fpublication_url\x18\x06 \x01(\t\x12(\n\x0erecord_created\x18\x07 \x01(\x0b\x32\x10.ord.RecordEvent\x12)\n\x0frecord_modified\x18\x08 \x03(\x0b\x32\x10.ord.RecordEvent\x12H\n\x11reaction_metadata\x18\t \x03(\x0b\x32-.ord.ReactionProvenance.ReactionMetadataEntry\x12\x15\n\x08is_mined\x18\n \x01(\x08H\x00\x88\x01\x01\x1a\x42\n\x15ReactionMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x18\n\x05value\x18\x02 \x01(\x0b\x32\t.ord.Data:\x02\x38\x01\x42\x0b\n\t_is_mined\"\\\n\x06Person\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05orcid\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\r\n\x05\x65mail\x18\x05 \x01(\t\"X\n\x0bRecordEvent\x12\x1b\n\x04time\x18\x01 \x01(\x0b\x32\r.ord.DateTime\x12\x1b\n\x06person\x18\x02 \x01(\x0b\x32\x0b.ord.Person\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\t\"\xb5\x01\n\x04Time\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Time.TimeUnit\"F\n\x08TimeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x44\x41Y\x10\x04\x12\x08\n\x04HOUR\x10\x01\x12\n\n\x06MINUTE\x10\x02\x12\n\n\x06SECOND\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc0\x01\n\x04Mass\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12!\n\x05units\x18\x03 \x01(\x0e\x32\x12.ord.Mass.MassUnit\"Q\n\x08MassUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0c\n\x08KILOGRAM\x10\x01\x12\x08\n\x04GRAM\x10\x02\x12\r\n\tMILLIGRAM\x10\x03\x12\r\n\tMICROGRAM\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc4\x01\n\x05Moles\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12#\n\x05units\x18\x03 \x01(\x0e\x32\x14.ord.Moles.MolesUnit\"R\n\tMolesUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04MOLE\x10\x01\x12\r\n\tMILLIMOLE\x10\x02\x12\r\n\tMICROMOLE\x10\x03\x12\x0c\n\x08NANOMOLE\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcc\x01\n\x06Volume\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Volume.VolumeUnit\"W\n\nVolumeUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05LITER\x10\x01\x12\x0e\n\nMILLILITER\x10\x02\x12\x0e\n\nMICROLITER\x10\x03\x12\r\n\tNANOLITER\x10\x04\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd9\x01\n\rConcentration\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x33\n\x05units\x18\x03 \x01(\x0e\x32$.ord.Concentration.ConcentrationUnit\"O\n\x11\x43oncentrationUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\t\n\x05MOLAR\x10\x01\x12\x0e\n\nMILLIMOLAR\x10\x02\x12\x0e\n\nMICROMOLAR\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xf7\x01\n\x08Pressure\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.Pressure.PressureUnit\"|\n\x0cPressureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x07\n\x03\x42\x41R\x10\x01\x12\x0e\n\nATMOSPHERE\x10\x02\x12\x07\n\x03PSI\x10\x03\x12\x08\n\x04KPSI\x10\x04\x12\n\n\x06PASCAL\x10\x05\x12\x0e\n\nKILOPASCAL\x10\x06\x12\x08\n\x04TORR\x10\x07\x12\t\n\x05MM_HG\x10\x08\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xcf\x01\n\x0bTemperature\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12/\n\x05units\x18\x03 \x01(\x0e\x32 .ord.Temperature.TemperatureUnit\"K\n\x0fTemperatureUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07\x43\x45LSIUS\x10\x01\x12\x0e\n\nFAHRENHEIT\x10\x02\x12\n\n\x06KELVIN\x10\x03\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xb3\x01\n\x07\x43urrent\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Current.CurrentUnit\";\n\x0b\x43urrentUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x41MPERE\x10\x01\x12\x0f\n\x0bMILLIAMPERE\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xaf\x01\n\x07Voltage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\'\n\x05units\x18\x03 \x01(\x0e\x32\x18.ord.Voltage.VoltageUnit\"7\n\x0bVoltageUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x08\n\x04VOLT\x10\x01\x12\r\n\tMILLIVOLT\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xd1\x01\n\x06Length\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12%\n\x05units\x18\x03 \x01(\x0e\x32\x16.ord.Length.LengthUnit\"\\\n\nLengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nCENTIMETER\x10\x01\x12\x0e\n\nMILLIMETER\x10\x02\x12\t\n\x05METER\x10\x03\x12\x08\n\x04INCH\x10\x04\x12\x08\n\x04\x46OOT\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xc1\x01\n\nWavelength\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12-\n\x05units\x18\x03 \x01(\x0e\x32\x1e.ord.Wavelength.WavelengthUnit\"@\n\x0eWavelengthUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\r\n\tNANOMETER\x10\x01\x12\x0e\n\nWAVENUMBER\x10\x02\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa0\x02\n\x08\x46lowRate\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12)\n\x05units\x18\x03 \x01(\x0e\x32\x1a.ord.FlowRate.FlowRateUnit\"\xa4\x01\n\x0c\x46lowRateUnit\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x19\n\x15MICROLITER_PER_MINUTE\x10\x01\x12\x19\n\x15MICROLITER_PER_SECOND\x10\x02\x12\x19\n\x15MILLILITER_PER_MINUTE\x10\x03\x12\x19\n\x15MILLILITER_PER_SECOND\x10\x04\x12\x17\n\x13MICROLITER_PER_HOUR\x10\x05\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nPercentage\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"P\n\nFloatValue\x12\x12\n\x05value\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x16\n\tprecision\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x08\n\x06_valueB\x0c\n\n_precision\"\xa1\x01\n\x04\x44\x61ta\x12\x15\n\x0b\x66loat_value\x18\x01 \x01(\x02H\x00\x12\x17\n\rinteger_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x62ytes_value\x18\x03 \x01(\x0cH\x00\x12\x16\n\x0cstring_value\x18\x04 \x01(\tH\x00\x12\r\n\x03url\x18\x05 \x01(\tH\x00\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x07 \x01(\tB\x06\n\x04kindb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ord_schema.proto.reaction_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -82,201 +82,201 @@
   _globals['_COMPOUND_SOURCE']._serialized_start=2583
   _globals['_COMPOUND_SOURCE']._serialized_end=2640
   _globals['_COMPOUND_FEATURESENTRY']._serialized_start=2642
   _globals['_COMPOUND_FEATURESENTRY']._serialized_end=2700
   _globals['_COMPOUND_ANALYSESENTRY']._serialized_start=2702
   _globals['_COMPOUND_ANALYSESENTRY']._serialized_end=2764
   _globals['_REACTIONROLE']._serialized_start=2783
-  _globals['_REACTIONROLE']._serialized_end=2961
+  _globals['_REACTIONROLE']._serialized_end=2994
   _globals['_REACTIONROLE_REACTIONROLETYPE']._serialized_start=2800
-  _globals['_REACTIONROLE_REACTIONROLETYPE']._serialized_end=2961
-  _globals['_COMPOUNDPREPARATION']._serialized_start=2964
-  _globals['_COMPOUNDPREPARATION']._serialized_end=3210
-  _globals['_COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE']._serialized_start=3089
-  _globals['_COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE']._serialized_end=3210
-  _globals['_COMPOUNDIDENTIFIER']._serialized_start=3213
-  _globals['_COMPOUNDIDENTIFIER']._serialized_end=3599
-  _globals['_COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE']._serialized_start=3330
-  _globals['_COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE']._serialized_end=3599
-  _globals['_VESSEL']._serialized_start=3602
-  _globals['_VESSEL']._serialized_end=4153
-  _globals['_VESSEL_VESSELTYPE']._serialized_start=3889
-  _globals['_VESSEL_VESSELTYPE']._serialized_end=4153
-  _globals['_VESSELMATERIAL']._serialized_start=4156
-  _globals['_VESSELMATERIAL']._serialized_end=4360
-  _globals['_VESSELMATERIAL_VESSELMATERIALTYPE']._serialized_start=4245
-  _globals['_VESSELMATERIAL_VESSELMATERIALTYPE']._serialized_end=4360
-  _globals['_VESSELATTACHMENT']._serialized_start=4363
-  _globals['_VESSELATTACHMENT']._serialized_end=4770
-  _globals['_VESSELATTACHMENT_VESSELATTACHMENTTYPE']._serialized_start=4459
-  _globals['_VESSELATTACHMENT_VESSELATTACHMENTTYPE']._serialized_end=4770
-  _globals['_VESSELPREPARATION']._serialized_start=4773
-  _globals['_VESSELPREPARATION']._serialized_end=5005
-  _globals['_VESSELPREPARATION_VESSELPREPARATIONTYPE']._serialized_start=4872
-  _globals['_VESSELPREPARATION_VESSELPREPARATIONTYPE']._serialized_end=5005
-  _globals['_REACTIONSETUP']._serialized_start=5008
-  _globals['_REACTIONSETUP']._serialized_end=5552
-  _globals['_REACTIONSETUP_AUTOMATIONCODEENTRY']._serialized_start=5236
-  _globals['_REACTIONSETUP_AUTOMATIONCODEENTRY']._serialized_end=5300
-  _globals['_REACTIONSETUP_REACTIONENVIRONMENT']._serialized_start=5303
-  _globals['_REACTIONSETUP_REACTIONENVIRONMENT']._serialized_end=5535
-  _globals['_REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE']._serialized_start=5421
-  _globals['_REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE']._serialized_end=5535
-  _globals['_REACTIONCONDITIONS']._serialized_start=5555
-  _globals['_REACTIONCONDITIONS']._serialized_end=5992
-  _globals['_TEMPERATURECONDITIONS']._serialized_start=5995
-  _globals['_TEMPERATURECONDITIONS']._serialized_end=6861
-  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL']._serialized_start=6194
-  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL']._serialized_end=6534
-  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE']._serialized_start=6318
-  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE']._serialized_end=6534
-  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT']._serialized_start=6537
-  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT']._serialized_end=6861
-  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE']._serialized_start=6736
-  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE']._serialized_end=6861
-  _globals['_PRESSURECONDITIONS']._serialized_start=6864
-  _globals['_PRESSURECONDITIONS']._serialized_end=7900
-  _globals['_PRESSURECONDITIONS_PRESSURECONTROL']._serialized_start=7101
-  _globals['_PRESSURECONDITIONS_PRESSURECONTROL']._serialized_end=7325
-  _globals['_PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE']._serialized_start=7212
-  _globals['_PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE']._serialized_end=7325
-  _globals['_PRESSURECONDITIONS_ATMOSPHERE']._serialized_start=7328
-  _globals['_PRESSURECONDITIONS_ATMOSPHERE']._serialized_end=7637
-  _globals['_PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE']._serialized_start=7425
-  _globals['_PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE']._serialized_end=7637
-  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT']._serialized_start=7640
-  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT']._serialized_end=7900
-  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE']._serialized_start=7821
-  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE']._serialized_end=7900
-  _globals['_STIRRINGCONDITIONS']._serialized_start=7903
-  _globals['_STIRRINGCONDITIONS']._serialized_end=8379
-  _globals['_STIRRINGCONDITIONS_STIRRINGRATE']._serialized_start=8053
-  _globals['_STIRRINGCONDITIONS_STIRRINGRATE']._serialized_end=8234
-  _globals['_STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE']._serialized_start=8168
-  _globals['_STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE']._serialized_end=8234
-  _globals['_STIRRINGCONDITIONS_STIRRINGMETHODTYPE']._serialized_start=8237
-  _globals['_STIRRINGCONDITIONS_STIRRINGMETHODTYPE']._serialized_end=8379
-  _globals['_ILLUMINATIONCONDITIONS']._serialized_start=8382
-  _globals['_ILLUMINATIONCONDITIONS']._serialized_end=8742
-  _globals['_ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE']._serialized_start=8584
-  _globals['_ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE']._serialized_end=8742
-  _globals['_ELECTROCHEMISTRYCONDITIONS']._serialized_start=8745
-  _globals['_ELECTROCHEMISTRYCONDITIONS']._serialized_end=9609
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT']._serialized_start=9166
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT']._serialized_end=9282
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL']._serialized_start=9285
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL']._serialized_end=9512
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE']._serialized_start=9419
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE']._serialized_end=9512
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE']._serialized_start=9514
-  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE']._serialized_end=9609
-  _globals['_FLOWCONDITIONS']._serialized_start=9612
-  _globals['_FLOWCONDITIONS']._serialized_end=10144
-  _globals['_FLOWCONDITIONS_TUBING']._serialized_start=9755
-  _globals['_FLOWCONDITIONS_TUBING']._serialized_end=10019
-  _globals['_FLOWCONDITIONS_TUBING_TUBINGTYPE']._serialized_start=9867
-  _globals['_FLOWCONDITIONS_TUBING_TUBINGTYPE']._serialized_end=10019
-  _globals['_FLOWCONDITIONS_FLOWTYPE']._serialized_start=10021
-  _globals['_FLOWCONDITIONS_FLOWTYPE']._serialized_end=10144
-  _globals['_REACTIONNOTES']._serialized_start=10147
-  _globals['_REACTIONNOTES']._serialized_end=10595
-  _globals['_REACTIONOBSERVATION']._serialized_start=10597
-  _globals['_REACTIONOBSERVATION']._serialized_end=10686
-  _globals['_REACTIONWORKUP']._serialized_start=10689
-  _globals['_REACTIONWORKUP']._serialized_end=11404
-  _globals['_REACTIONWORKUP_REACTIONWORKUPTYPE']._serialized_start=11035
-  _globals['_REACTIONWORKUP_REACTIONWORKUPTYPE']._serialized_end=11373
-  _globals['_REACTIONOUTCOME']._serialized_start=11407
-  _globals['_REACTIONOUTCOME']._serialized_end=11653
+  _globals['_REACTIONROLE_REACTIONROLETYPE']._serialized_end=2994
+  _globals['_COMPOUNDPREPARATION']._serialized_start=2997
+  _globals['_COMPOUNDPREPARATION']._serialized_end=3243
+  _globals['_COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE']._serialized_start=3122
+  _globals['_COMPOUNDPREPARATION_COMPOUNDPREPARATIONTYPE']._serialized_end=3243
+  _globals['_COMPOUNDIDENTIFIER']._serialized_start=3246
+  _globals['_COMPOUNDIDENTIFIER']._serialized_end=3632
+  _globals['_COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE']._serialized_start=3363
+  _globals['_COMPOUNDIDENTIFIER_COMPOUNDIDENTIFIERTYPE']._serialized_end=3632
+  _globals['_VESSEL']._serialized_start=3635
+  _globals['_VESSEL']._serialized_end=4186
+  _globals['_VESSEL_VESSELTYPE']._serialized_start=3922
+  _globals['_VESSEL_VESSELTYPE']._serialized_end=4186
+  _globals['_VESSELMATERIAL']._serialized_start=4189
+  _globals['_VESSELMATERIAL']._serialized_end=4393
+  _globals['_VESSELMATERIAL_VESSELMATERIALTYPE']._serialized_start=4278
+  _globals['_VESSELMATERIAL_VESSELMATERIALTYPE']._serialized_end=4393
+  _globals['_VESSELATTACHMENT']._serialized_start=4396
+  _globals['_VESSELATTACHMENT']._serialized_end=4803
+  _globals['_VESSELATTACHMENT_VESSELATTACHMENTTYPE']._serialized_start=4492
+  _globals['_VESSELATTACHMENT_VESSELATTACHMENTTYPE']._serialized_end=4803
+  _globals['_VESSELPREPARATION']._serialized_start=4806
+  _globals['_VESSELPREPARATION']._serialized_end=5038
+  _globals['_VESSELPREPARATION_VESSELPREPARATIONTYPE']._serialized_start=4905
+  _globals['_VESSELPREPARATION_VESSELPREPARATIONTYPE']._serialized_end=5038
+  _globals['_REACTIONSETUP']._serialized_start=5041
+  _globals['_REACTIONSETUP']._serialized_end=5585
+  _globals['_REACTIONSETUP_AUTOMATIONCODEENTRY']._serialized_start=5269
+  _globals['_REACTIONSETUP_AUTOMATIONCODEENTRY']._serialized_end=5333
+  _globals['_REACTIONSETUP_REACTIONENVIRONMENT']._serialized_start=5336
+  _globals['_REACTIONSETUP_REACTIONENVIRONMENT']._serialized_end=5568
+  _globals['_REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE']._serialized_start=5454
+  _globals['_REACTIONSETUP_REACTIONENVIRONMENT_REACTIONENVIRONMENTTYPE']._serialized_end=5568
+  _globals['_REACTIONCONDITIONS']._serialized_start=5588
+  _globals['_REACTIONCONDITIONS']._serialized_end=6025
+  _globals['_TEMPERATURECONDITIONS']._serialized_start=6028
+  _globals['_TEMPERATURECONDITIONS']._serialized_end=6894
+  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL']._serialized_start=6227
+  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL']._serialized_end=6567
+  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE']._serialized_start=6351
+  _globals['_TEMPERATURECONDITIONS_TEMPERATURECONTROL_TEMPERATURECONTROLTYPE']._serialized_end=6567
+  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT']._serialized_start=6570
+  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT']._serialized_end=6894
+  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE']._serialized_start=6769
+  _globals['_TEMPERATURECONDITIONS_TEMPERATUREMEASUREMENT_TEMPERATUREMEASUREMENTTYPE']._serialized_end=6894
+  _globals['_PRESSURECONDITIONS']._serialized_start=6897
+  _globals['_PRESSURECONDITIONS']._serialized_end=7933
+  _globals['_PRESSURECONDITIONS_PRESSURECONTROL']._serialized_start=7134
+  _globals['_PRESSURECONDITIONS_PRESSURECONTROL']._serialized_end=7358
+  _globals['_PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE']._serialized_start=7245
+  _globals['_PRESSURECONDITIONS_PRESSURECONTROL_PRESSURECONTROLTYPE']._serialized_end=7358
+  _globals['_PRESSURECONDITIONS_ATMOSPHERE']._serialized_start=7361
+  _globals['_PRESSURECONDITIONS_ATMOSPHERE']._serialized_end=7670
+  _globals['_PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE']._serialized_start=7458
+  _globals['_PRESSURECONDITIONS_ATMOSPHERE_ATMOSPHERETYPE']._serialized_end=7670
+  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT']._serialized_start=7673
+  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT']._serialized_end=7933
+  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE']._serialized_start=7854
+  _globals['_PRESSURECONDITIONS_PRESSUREMEASUREMENT_PRESSUREMEASUREMENTTYPE']._serialized_end=7933
+  _globals['_STIRRINGCONDITIONS']._serialized_start=7936
+  _globals['_STIRRINGCONDITIONS']._serialized_end=8412
+  _globals['_STIRRINGCONDITIONS_STIRRINGRATE']._serialized_start=8086
+  _globals['_STIRRINGCONDITIONS_STIRRINGRATE']._serialized_end=8267
+  _globals['_STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE']._serialized_start=8201
+  _globals['_STIRRINGCONDITIONS_STIRRINGRATE_STIRRINGRATETYPE']._serialized_end=8267
+  _globals['_STIRRINGCONDITIONS_STIRRINGMETHODTYPE']._serialized_start=8270
+  _globals['_STIRRINGCONDITIONS_STIRRINGMETHODTYPE']._serialized_end=8412
+  _globals['_ILLUMINATIONCONDITIONS']._serialized_start=8415
+  _globals['_ILLUMINATIONCONDITIONS']._serialized_end=8775
+  _globals['_ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE']._serialized_start=8617
+  _globals['_ILLUMINATIONCONDITIONS_ILLUMINATIONTYPE']._serialized_end=8775
+  _globals['_ELECTROCHEMISTRYCONDITIONS']._serialized_start=8778
+  _globals['_ELECTROCHEMISTRYCONDITIONS']._serialized_end=9642
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT']._serialized_start=9199
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYMEASUREMENT']._serialized_end=9315
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL']._serialized_start=9318
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL']._serialized_end=9545
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE']._serialized_start=9452
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYCELL_ELECTROCHEMISTRYCELLTYPE']._serialized_end=9545
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE']._serialized_start=9547
+  _globals['_ELECTROCHEMISTRYCONDITIONS_ELECTROCHEMISTRYTYPE']._serialized_end=9642
+  _globals['_FLOWCONDITIONS']._serialized_start=9645
+  _globals['_FLOWCONDITIONS']._serialized_end=10177
+  _globals['_FLOWCONDITIONS_TUBING']._serialized_start=9788
+  _globals['_FLOWCONDITIONS_TUBING']._serialized_end=10052
+  _globals['_FLOWCONDITIONS_TUBING_TUBINGTYPE']._serialized_start=9900
+  _globals['_FLOWCONDITIONS_TUBING_TUBINGTYPE']._serialized_end=10052
+  _globals['_FLOWCONDITIONS_FLOWTYPE']._serialized_start=10054
+  _globals['_FLOWCONDITIONS_FLOWTYPE']._serialized_end=10177
+  _globals['_REACTIONNOTES']._serialized_start=10180
+  _globals['_REACTIONNOTES']._serialized_end=10628
+  _globals['_REACTIONOBSERVATION']._serialized_start=10630
+  _globals['_REACTIONOBSERVATION']._serialized_end=10719
+  _globals['_REACTIONWORKUP']._serialized_start=10722
+  _globals['_REACTIONWORKUP']._serialized_end=11437
+  _globals['_REACTIONWORKUP_REACTIONWORKUPTYPE']._serialized_start=11068
+  _globals['_REACTIONWORKUP_REACTIONWORKUPTYPE']._serialized_end=11406
+  _globals['_REACTIONOUTCOME']._serialized_start=11440
+  _globals['_REACTIONOUTCOME']._serialized_end=11686
   _globals['_REACTIONOUTCOME_ANALYSESENTRY']._serialized_start=2702
   _globals['_REACTIONOUTCOME_ANALYSESENTRY']._serialized_end=2764
-  _globals['_PRODUCTCOMPOUND']._serialized_start=11656
-  _globals['_PRODUCTCOMPOUND']._serialized_end=12309
-  _globals['_PRODUCTCOMPOUND_TEXTURE']._serialized_start=11986
-  _globals['_PRODUCTCOMPOUND_TEXTURE']._serialized_end=12226
-  _globals['_PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE']._serialized_start=12071
-  _globals['_PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE']._serialized_end=12226
+  _globals['_PRODUCTCOMPOUND']._serialized_start=11689
+  _globals['_PRODUCTCOMPOUND']._serialized_end=12342
+  _globals['_PRODUCTCOMPOUND_TEXTURE']._serialized_start=12019
+  _globals['_PRODUCTCOMPOUND_TEXTURE']._serialized_end=12259
+  _globals['_PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE']._serialized_start=12104
+  _globals['_PRODUCTCOMPOUND_TEXTURE_TEXTURETYPE']._serialized_end=12259
   _globals['_PRODUCTCOMPOUND_FEATURESENTRY']._serialized_start=2642
   _globals['_PRODUCTCOMPOUND_FEATURESENTRY']._serialized_end=2700
-  _globals['_PRODUCTMEASUREMENT']._serialized_start=12312
-  _globals['_PRODUCTMEASUREMENT']._serialized_end=13715
-  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS']._serialized_start=12925
-  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS']._serialized_end=13286
-  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE']._serialized_start=13140
-  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE']._serialized_end=13248
-  _globals['_PRODUCTMEASUREMENT_SELECTIVITY']._serialized_start=13289
-  _globals['_PRODUCTMEASUREMENT_SELECTIVITY']._serialized_end=13474
-  _globals['_PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE']._serialized_start=13388
-  _globals['_PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE']._serialized_end=13474
-  _globals['_PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE']._serialized_start=13477
-  _globals['_PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE']._serialized_end=13633
-  _globals['_DATETIME']._serialized_start=13717
-  _globals['_DATETIME']._serialized_end=13742
-  _globals['_ANALYSIS']._serialized_start=13745
-  _globals['_ANALYSIS']._serialized_end=14333
-  _globals['_ANALYSIS_DATAENTRY']._serialized_start=13993
-  _globals['_ANALYSIS_DATAENTRY']._serialized_end=14047
-  _globals['_ANALYSIS_ANALYSISTYPE']._serialized_start=14050
-  _globals['_ANALYSIS_ANALYSISTYPE']._serialized_end=14306
-  _globals['_REACTIONPROVENANCE']._serialized_start=14336
-  _globals['_REACTIONPROVENANCE']._serialized_end=14763
-  _globals['_REACTIONPROVENANCE_REACTIONMETADATAENTRY']._serialized_start=14684
-  _globals['_REACTIONPROVENANCE_REACTIONMETADATAENTRY']._serialized_end=14750
-  _globals['_PERSON']._serialized_start=14765
-  _globals['_PERSON']._serialized_end=14857
-  _globals['_RECORDEVENT']._serialized_start=14859
-  _globals['_RECORDEVENT']._serialized_end=14947
-  _globals['_TIME']._serialized_start=14950
-  _globals['_TIME']._serialized_end=15131
-  _globals['_TIME_TIMEUNIT']._serialized_start=15037
-  _globals['_TIME_TIMEUNIT']._serialized_end=15107
-  _globals['_MASS']._serialized_start=15134
-  _globals['_MASS']._serialized_end=15326
-  _globals['_MASS_MASSUNIT']._serialized_start=15221
-  _globals['_MASS_MASSUNIT']._serialized_end=15302
-  _globals['_MOLES']._serialized_start=15329
-  _globals['_MOLES']._serialized_end=15525
-  _globals['_MOLES_MOLESUNIT']._serialized_start=15419
-  _globals['_MOLES_MOLESUNIT']._serialized_end=15501
-  _globals['_VOLUME']._serialized_start=15528
-  _globals['_VOLUME']._serialized_end=15732
-  _globals['_VOLUME_VOLUMEUNIT']._serialized_start=15621
-  _globals['_VOLUME_VOLUMEUNIT']._serialized_end=15708
-  _globals['_CONCENTRATION']._serialized_start=15735
-  _globals['_CONCENTRATION']._serialized_end=15952
-  _globals['_CONCENTRATION_CONCENTRATIONUNIT']._serialized_start=15849
-  _globals['_CONCENTRATION_CONCENTRATIONUNIT']._serialized_end=15928
-  _globals['_PRESSURE']._serialized_start=15955
-  _globals['_PRESSURE']._serialized_end=16202
-  _globals['_PRESSURE_PRESSUREUNIT']._serialized_start=16054
-  _globals['_PRESSURE_PRESSUREUNIT']._serialized_end=16178
-  _globals['_TEMPERATURE']._serialized_start=16205
-  _globals['_TEMPERATURE']._serialized_end=16412
-  _globals['_TEMPERATURE_TEMPERATUREUNIT']._serialized_start=16313
-  _globals['_TEMPERATURE_TEMPERATUREUNIT']._serialized_end=16388
-  _globals['_CURRENT']._serialized_start=16415
-  _globals['_CURRENT']._serialized_end=16594
-  _globals['_CURRENT_CURRENTUNIT']._serialized_start=16511
-  _globals['_CURRENT_CURRENTUNIT']._serialized_end=16570
-  _globals['_VOLTAGE']._serialized_start=16597
-  _globals['_VOLTAGE']._serialized_end=16772
-  _globals['_VOLTAGE_VOLTAGEUNIT']._serialized_start=16693
-  _globals['_VOLTAGE_VOLTAGEUNIT']._serialized_end=16748
-  _globals['_LENGTH']._serialized_start=16775
-  _globals['_LENGTH']._serialized_end=16984
-  _globals['_LENGTH_LENGTHUNIT']._serialized_start=16868
-  _globals['_LENGTH_LENGTHUNIT']._serialized_end=16960
-  _globals['_WAVELENGTH']._serialized_start=16987
-  _globals['_WAVELENGTH']._serialized_end=17180
-  _globals['_WAVELENGTH_WAVELENGTHUNIT']._serialized_start=17092
-  _globals['_WAVELENGTH_WAVELENGTHUNIT']._serialized_end=17156
-  _globals['_FLOWRATE']._serialized_start=17183
-  _globals['_FLOWRATE']._serialized_end=17471
-  _globals['_FLOWRATE_FLOWRATEUNIT']._serialized_start=17283
-  _globals['_FLOWRATE_FLOWRATEUNIT']._serialized_end=17447
-  _globals['_PERCENTAGE']._serialized_start=17473
-  _globals['_PERCENTAGE']._serialized_end=17553
-  _globals['_FLOATVALUE']._serialized_start=17555
-  _globals['_FLOATVALUE']._serialized_end=17635
-  _globals['_DATA']._serialized_start=17638
-  _globals['_DATA']._serialized_end=17799
+  _globals['_PRODUCTMEASUREMENT']._serialized_start=12345
+  _globals['_PRODUCTMEASUREMENT']._serialized_end=13748
+  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS']._serialized_start=12958
+  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS']._serialized_end=13319
+  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE']._serialized_start=13173
+  _globals['_PRODUCTMEASUREMENT_MASSSPECMEASUREMENTDETAILS_MASSSPECMEASUREMENTTYPE']._serialized_end=13281
+  _globals['_PRODUCTMEASUREMENT_SELECTIVITY']._serialized_start=13322
+  _globals['_PRODUCTMEASUREMENT_SELECTIVITY']._serialized_end=13507
+  _globals['_PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE']._serialized_start=13421
+  _globals['_PRODUCTMEASUREMENT_SELECTIVITY_SELECTIVITYTYPE']._serialized_end=13507
+  _globals['_PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE']._serialized_start=13510
+  _globals['_PRODUCTMEASUREMENT_PRODUCTMEASUREMENTTYPE']._serialized_end=13666
+  _globals['_DATETIME']._serialized_start=13750
+  _globals['_DATETIME']._serialized_end=13775
+  _globals['_ANALYSIS']._serialized_start=13778
+  _globals['_ANALYSIS']._serialized_end=14366
+  _globals['_ANALYSIS_DATAENTRY']._serialized_start=14026
+  _globals['_ANALYSIS_DATAENTRY']._serialized_end=14080
+  _globals['_ANALYSIS_ANALYSISTYPE']._serialized_start=14083
+  _globals['_ANALYSIS_ANALYSISTYPE']._serialized_end=14339
+  _globals['_REACTIONPROVENANCE']._serialized_start=14369
+  _globals['_REACTIONPROVENANCE']._serialized_end=14796
+  _globals['_REACTIONPROVENANCE_REACTIONMETADATAENTRY']._serialized_start=14717
+  _globals['_REACTIONPROVENANCE_REACTIONMETADATAENTRY']._serialized_end=14783
+  _globals['_PERSON']._serialized_start=14798
+  _globals['_PERSON']._serialized_end=14890
+  _globals['_RECORDEVENT']._serialized_start=14892
+  _globals['_RECORDEVENT']._serialized_end=14980
+  _globals['_TIME']._serialized_start=14983
+  _globals['_TIME']._serialized_end=15164
+  _globals['_TIME_TIMEUNIT']._serialized_start=15070
+  _globals['_TIME_TIMEUNIT']._serialized_end=15140
+  _globals['_MASS']._serialized_start=15167
+  _globals['_MASS']._serialized_end=15359
+  _globals['_MASS_MASSUNIT']._serialized_start=15254
+  _globals['_MASS_MASSUNIT']._serialized_end=15335
+  _globals['_MOLES']._serialized_start=15362
+  _globals['_MOLES']._serialized_end=15558
+  _globals['_MOLES_MOLESUNIT']._serialized_start=15452
+  _globals['_MOLES_MOLESUNIT']._serialized_end=15534
+  _globals['_VOLUME']._serialized_start=15561
+  _globals['_VOLUME']._serialized_end=15765
+  _globals['_VOLUME_VOLUMEUNIT']._serialized_start=15654
+  _globals['_VOLUME_VOLUMEUNIT']._serialized_end=15741
+  _globals['_CONCENTRATION']._serialized_start=15768
+  _globals['_CONCENTRATION']._serialized_end=15985
+  _globals['_CONCENTRATION_CONCENTRATIONUNIT']._serialized_start=15882
+  _globals['_CONCENTRATION_CONCENTRATIONUNIT']._serialized_end=15961
+  _globals['_PRESSURE']._serialized_start=15988
+  _globals['_PRESSURE']._serialized_end=16235
+  _globals['_PRESSURE_PRESSUREUNIT']._serialized_start=16087
+  _globals['_PRESSURE_PRESSUREUNIT']._serialized_end=16211
+  _globals['_TEMPERATURE']._serialized_start=16238
+  _globals['_TEMPERATURE']._serialized_end=16445
+  _globals['_TEMPERATURE_TEMPERATUREUNIT']._serialized_start=16346
+  _globals['_TEMPERATURE_TEMPERATUREUNIT']._serialized_end=16421
+  _globals['_CURRENT']._serialized_start=16448
+  _globals['_CURRENT']._serialized_end=16627
+  _globals['_CURRENT_CURRENTUNIT']._serialized_start=16544
+  _globals['_CURRENT_CURRENTUNIT']._serialized_end=16603
+  _globals['_VOLTAGE']._serialized_start=16630
+  _globals['_VOLTAGE']._serialized_end=16805
+  _globals['_VOLTAGE_VOLTAGEUNIT']._serialized_start=16726
+  _globals['_VOLTAGE_VOLTAGEUNIT']._serialized_end=16781
+  _globals['_LENGTH']._serialized_start=16808
+  _globals['_LENGTH']._serialized_end=17017
+  _globals['_LENGTH_LENGTHUNIT']._serialized_start=16901
+  _globals['_LENGTH_LENGTHUNIT']._serialized_end=16993
+  _globals['_WAVELENGTH']._serialized_start=17020
+  _globals['_WAVELENGTH']._serialized_end=17213
+  _globals['_WAVELENGTH_WAVELENGTHUNIT']._serialized_start=17125
+  _globals['_WAVELENGTH_WAVELENGTHUNIT']._serialized_end=17189
+  _globals['_FLOWRATE']._serialized_start=17216
+  _globals['_FLOWRATE']._serialized_end=17504
+  _globals['_FLOWRATE_FLOWRATEUNIT']._serialized_start=17316
+  _globals['_FLOWRATE_FLOWRATEUNIT']._serialized_end=17480
+  _globals['_PERCENTAGE']._serialized_start=17506
+  _globals['_PERCENTAGE']._serialized_end=17586
+  _globals['_FLOATVALUE']._serialized_start=17588
+  _globals['_FLOATVALUE']._serialized_end=17668
+  _globals['_DATA']._serialized_start=17671
+  _globals['_DATA']._serialized_end=17832
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ord-schema-0.3.59/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.60/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.60/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/resolvers.py` & `ord-schema-0.3.60/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/resolvers_test.py` & `ord-schema-0.3.60/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/__init__.py` & `ord-schema-0.3.60/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.60/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.60/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.60/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.60/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.60/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.60/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.60/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.60/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.60/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.60/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/templating.py` & `ord-schema-0.3.60/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/templating_test.py` & `ord-schema-0.3.60/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/units.py` & `ord-schema-0.3.60/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/units_test.py` & `ord-schema-0.3.60/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/updates.py` & `ord-schema-0.3.60/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/updates_test.py` & `ord-schema-0.3.60/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema/validations.py` & `ord-schema-0.3.60/ord_schema/validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,17 +779,26 @@
             "Workup amount should only be specified if workup type is ALIQUOT or CUSTOM",
             ValidationWarning,
         )
 
 
 def validate_reaction_outcome(message: reaction_pb2.ReactionOutcome):
     # pylint: disable=singleton-comparison
-    # Can only have one desired product
-    if sum(product.is_desired_product for product in message.products) > 1:
-        warnings.warn("Cannot have more than one desired product!", ValidationError)
+    # *Usually* there should be at most one PRODUCT & is_desired_product
+    ndp = sum(
+        product.is_desired_product
+        for product in message.products
+        if product.reaction_role == reaction_pb2.ReactionRole.ReactionRoleType.PRODUCT
+    )
+    if ndp > 1:
+        warnings.warn(
+            f"Usually at most one (reaction_role == PRODUCT & is_desired_product) product, but we have: {ndp}",
+            ValidationWarning,
+        )
+
     # Check key values for product analyses
     # NOTE(ccoley): Could use any(), but using expanded loops for clarity
     analysis_keys = list(message.analyses.keys())
     for product in message.products:
         for measurement in product.measurements:
             if measurement.analysis_key and measurement.analysis_key not in analysis_keys:
                 warnings.warn(
@@ -816,14 +825,18 @@
             ValidationWarning,
         )
     try:
         message_helpers.check_compound_identifiers(message)
     except ValueError as error:
         warnings.warn(str(error), ValidationWarning)
 
+    if message.is_desired_product:
+        if message.reaction_role == reaction_pb2.ReactionRole.ReactionRoleType.SIDE_PRODUCT:
+            warnings.warn("a product cannot be (SIDE_PRODUCT & is_desired_product)", ValidationError)
+
 
 def validate_texture(message: reaction_pb2.ProductCompound.Texture):
     check_type_and_details(message)
 
 
 def validate_product_measurement(message: reaction_pb2.ProductMeasurement):
     check_type_and_details(message)
```

### Comparing `ord-schema-0.3.59/ord_schema/validations_test.py` & `ord-schema-0.3.60/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.60/ord_schema.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.59
+Version: 0.3.60
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -51,7 +51,24 @@
 $ git clone https://github.com/open-reaction-database/ord-schema.git
 $ cd ord-schema
 $ pip install -e .
 ```
 
 If you make changes to the protocol buffer definitions, [install](https://grpc.io/docs/protoc-installation/) `protoc`
 and run `./compile_proto_wrappers.sh` to rebuild the wrappers.
+
+## Conventions
+
+### 1. convention: compound stoichiometry
+
+##### Created: 2023.07.04
+
+##### Last updated: 2023.07.04
+
+##### Description: 
+1. The preferred field for compound stoichiometry is the map `Compound.features` or `ProductCompound.features`.
+2. The key should be "stoichiometric_coefficient" or "stoichiometric_ratio".
+3. The value should be a Data mesaage with its float_value representing the compound's stoichiometric coefficient or ratio.SInformation about also put stoichiometry ratio/coefficient here
+
+##### Related links: 
+[#683](https://github.com/open-reaction-database/ord-schema/issues/683) 
+[#684](https://github.com/open-reaction-database/ord-schema/pull/684)
```

### Comparing `ord-schema-0.3.59/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.60/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.60/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/proto/dataset.proto` & `ord-schema-0.3.60/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/proto/reaction.proto` & `ord-schema-0.3.60/proto/reaction.proto`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,22 @@
     // added prior to the start of the reaction) or as part of a workup
     // step of addition.
     INTERNAL_STANDARD = 6;
     AUTHENTIC_STANDARD = 7;
     // A product can be any species produced by the reaction, whether desired
     // or undesired.
     PRODUCT = 8;
+    // When there is one intended chemical equation:
+    // - Set `is_desired_product=True` to indicate a desired product.
+    // - Use BYPRODUCT to indicate a chemical species that is an expected result
+    // of the reaction but is not the product of interest.
+    // - Use SIDE_PRODUCT to indicate the product of a side reaction.
+    // - See https://doi.org/10.1021/op300317g for a discussion of these terms.
+    BYPRODUCT = 9;
+    SIDE_PRODUCT = 10;
   }
 }
 
 /**
  * Compounds may undergo additional preparation before being used in a
  * reaction after being received from a supplier or vendor. We encourage
  * the use of the 'preparation' enum when possible, even if the description
```

### Comparing `ord-schema-0.3.59/proto/test.proto` & `ord-schema-0.3.60/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.59/setup.py` & `ord-schema-0.3.60/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.59",
+    version="0.3.60",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

