# Comparing `tmp/reportportal-client-5.3.5.tar.gz` & `tmp/reportportal-client-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportportal-client-5.3.5.tar", last modified: Wed Jun  7 14:25:32 2023, max compression
+gzip compressed data, was "reportportal-client-5.4.0.tar", last modified: Mon Jul 10 13:33:28 2023, max compression
```

## Comparing `reportportal-client-5.3.5.tar` & `reportportal-client-5.4.0.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-07 14:25:32.206095 reportportal-client-5.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.194094 reportportal-client-5.3.5/reportportal_client/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/_local/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21241 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/client.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/core/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/rp_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/core/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/item_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_base_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.198094 reportportal-client-5.3.5/reportportal_client/items/rp_log_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_log_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_log_items/rp_log_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_base_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_child_test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_root_test_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/logs/log_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/services/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/services/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/static/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/static/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/reportportal_client/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/reportportal_client/steps/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.194094 reportportal-client-5.3.5/reportportal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 14:25:32.000000 reportportal-client-5.3.5/reportportal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-07 14:25:32.206095 reportportal-client-5.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:25:32.202095 reportportal-client-5.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-07 14:25:27.000000 reportportal-client-5.3.5/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.313135 reportportal-client-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-10 13:33:28.313135 reportportal-client-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23553 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/core/rp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/core/rp_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/core/rp_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/core/rp_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/core/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/core/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/item_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/rp_base_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/items/rp_log_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/rp_log_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/rp_log_items/rp_log_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/items/rp_test_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/rp_test_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/rp_test_items/rp_base_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/rp_test_items/rp_child_test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/items/rp_test_items/rp_root_test_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/logs/log_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/services/client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/services/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/services/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.313135 reportportal-client-5.4.0/reportportal_client/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/static/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/static/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/static/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.313135 reportportal-client-5.4.0/reportportal_client/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/reportportal_client/steps/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.309135 reportportal-client-5.4.0/reportportal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-10 13:33:28.000000 reportportal-client-5.4.0/reportportal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-10 13:33:28.000000 reportportal-client-5.4.0/reportportal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:33:28.000000 reportportal-client-5.4.0/reportportal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 13:33:28.000000 reportportal-client-5.4.0/reportportal_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-10 13:33:28.000000 reportportal-client-5.4.0/reportportal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 13:33:28.313135 reportportal-client-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:33:28.313135 reportportal-client-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/tests/test_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-10 13:33:22.000000 reportportal-client-5.4.0/tests/test_statistics.py
```

### Comparing `reportportal-client-5.3.5/CONTRIBUTING.rst` & `reportportal-client-5.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/LICENSE.md` & `reportportal-client-5.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/PKG-INFO` & `reportportal-client-5.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.5
+Version: 5.4.0
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.5
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.4.0
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reportportal-client-5.3.5/README.md` & `reportportal-client-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/__init__.py` & `reportportal-client-5.4.0/reportportal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/_local/__init__.py` & `reportportal-client-5.4.0/reportportal_client/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/client.py` & `reportportal-client-5.4.0/reportportal_client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
 import logging
+import sys
 import warnings
 from os import getenv
+from typing import Union, Tuple, List, Dict, Any, Optional, TextIO
 
 import requests
 from requests.adapters import HTTPAdapter, Retry, DEFAULT_RETRIES
 
 from ._local import set_current
+from .core.rp_issues import Issue
 from .core.rp_requests import (
     HttpRequest,
     ItemStartRequest,
     ItemFinishRequest,
     LaunchStartRequest,
     LaunchFinishRequest
 )
@@ -34,39 +37,67 @@
 from .static.defines import NOT_FOUND
 from .steps import StepReporter
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
-class RPClient(object):
+class RPClient:
     """Report portal client.
 
     The class is supposed to use by Report Portal agents: both custom and
     official to make calls to Report Portal. It handles HTTP request and
     response bodies generation and serialization, connection retries and log
     batching.
     NOTICE: the class is not thread-safe, use new class instance for every new
     thread to avoid request/response messing and other issues.
     """
 
-    def __init__(self,
-                 endpoint,
-                 project,
-                 api_key=None,
-                 log_batch_size=20,
-                 is_skipped_an_issue=True,
-                 verify_ssl=True,
-                 retries=None,
-                 max_pool_size=50,
-                 launch_id=None,
-                 http_timeout=(10, 10),
-                 log_batch_payload_size=MAX_LOG_BATCH_PAYLOAD_SIZE,
-                 mode='DEFAULT',
-                 **kwargs):
+    _log_manager: LogManager = ...
+    api_v1: str = ...
+    api_v2: str = ...
+    base_url_v1: str = ...
+    base_url_v2: str = ...
+    endpoint: str = ...
+    is_skipped_an_issue: bool = ...
+    launch_id: str = ...
+    log_batch_size: int = ...
+    log_batch_payload_size: int = ...
+    project: str = ...
+    api_key: str = ...
+    verify_ssl: Union[bool, str] = ...
+    retries: int = ...
+    max_pool_size: int = ...
+    http_timeout: Union[float, Tuple[float, float]] = ...
+    session: requests.Session = ...
+    step_reporter: StepReporter = ...
+    mode: str = ...
+    launch_uuid_print: Optional[bool] = ...
+    print_output: Optional[TextIO] = ...
+    _skip_analytics: str = ...
+    _item_stack: List[str] = ...
+
+    def __init__(
+            self,
+            endpoint: str,
+            project: str,
+            api_key: str = None,
+            log_batch_size: int = 20,
+            is_skipped_an_issue: bool = True,
+            verify_ssl: bool = True,
+            retries: int = None,
+            max_pool_size: int = 50,
+            launch_id: str = None,
+            http_timeout: Union[float, Tuple[float, float]] = (10, 10),
+            log_batch_payload_size: int = MAX_LOG_BATCH_PAYLOAD_SIZE,
+            mode: str = 'DEFAULT',
+            launch_uuid_print: bool = False,
+            print_output: Optional[TextIO] = None,
+            **kwargs: Any
+    ) -> None:
         """Initialize required attributes.
 
         :param endpoint:               Endpoint of the report portal service
         :param project:                Project name to report to
         :param api_key:                Authorization API key
         :param log_batch_size:         Option to set the maximum number of
                                        logs that can be processed in one batch
@@ -101,41 +132,43 @@
         self.retries = retries
         self.max_pool_size = max_pool_size
         self.http_timeout = http_timeout
         self.step_reporter = StepReporter(self)
         self._item_stack = []
         self.mode = mode
         self._skip_analytics = getenv('AGENT_NO_ANALYTICS')
+        self.launch_uuid_print = launch_uuid_print
+        self.print_output = print_output or sys.stdout
 
         self.api_key = api_key
         if not self.api_key:
             if 'token' in kwargs:
                 warnings.warn(
-                    message="Argument `token` is deprecated since 5.3.5 and "
-                            "will be subject for removing in the next major "
-                            "version. Use `api_key` argument instead.",
+                    message='Argument `token` is deprecated since 5.3.5 and '
+                            'will be subject for removing in the next major '
+                            'version. Use `api_key` argument instead.',
                     category=DeprecationWarning,
                     stacklevel=2
                 )
                 self.api_key = kwargs['token']
 
             if not self.api_key:
                 warnings.warn(
-                    message="Argument `api_key` is `None` or empty string, "
-                            "that's not supposed to happen because Report "
-                            "Portal is usually requires an authorization key. "
-                            "Please check your code.",
+                    message='Argument `api_key` is `None` or empty string, '
+                            'that is not supposed to happen because Report '
+                            'Portal is usually requires an authorization key. '
+                            'Please check your code.',
                     category=RuntimeWarning,
                     stacklevel=2
                 )
 
         self.__init_session()
         self.__init_log_manager()
 
-    def __init_session(self):
+    def __init_session(self) -> None:
         retry_strategy = Retry(
             total=self.retries,
             backoff_factor=0.1,
             status_forcelist=[429, 500, 502, 503, 504]
         ) if self.retries else DEFAULT_RETRIES
         session = requests.Session()
         session.mount('https://', HTTPAdapter(
@@ -144,36 +177,36 @@
         session.mount('http://', HTTPAdapter(
             max_retries=retry_strategy, pool_maxsize=self.max_pool_size))
         if self.api_key:
             session.headers['Authorization'] = 'Bearer {0}'.format(
                 self.api_key)
         self.session = session
 
-    def __init_log_manager(self):
+    def __init_log_manager(self) -> None:
         self._log_manager = LogManager(
             self.endpoint, self.session, self.api_v2, self.launch_id,
             self.project, max_entry_number=self.log_batch_size,
             max_payload_size=self.log_batch_payload_size,
             verify_ssl=self.verify_ssl)
 
     def finish_launch(self,
-                      end_time,
-                      status=None,
-                      attributes=None,
-                      **kwargs):
+                      end_time: str,
+                      status: str = None,
+                      attributes: Optional[Union[List, Dict]] = None,
+                      **kwargs: Any) -> Optional[str]:
         """Finish launch.
 
         :param end_time:    Launch end time
         :param status:      Launch status. Can be one of the followings:
                             PASSED, FAILED, STOPPED, SKIPPED, RESETED,
                             CANCELLED
         :param attributes:  Launch attributes
         """
         if self.launch_id is NOT_FOUND or not self.launch_id:
-            logger.warning("Attempt to finish non-existent launch")
+            logger.warning('Attempt to finish non-existent launch')
             return
         url = uri_join(self.base_url_v2, 'launch', self.launch_id, 'finish')
         request_payload = LaunchFinishRequest(
             end_time,
             status=status,
             attributes=attributes,
             description=kwargs.get('description')
@@ -184,22 +217,22 @@
         if not response:
             return
         logger.debug('finish_launch - ID: %s', self.launch_id)
         logger.debug('response message: %s', response.message)
         return response.message
 
     def finish_test_item(self,
-                         item_id,
-                         end_time,
-                         status=None,
-                         issue=None,
-                         attributes=None,
-                         description=None,
-                         retry=False,
-                         **kwargs):
+                         item_id: str,
+                         end_time: str,
+                         status: str = None,
+                         issue: Optional[Issue] = None,
+                         attributes: Optional[Union[List, Dict]] = None,
+                         description: str = None,
+                         retry: bool = False,
+                         **kwargs: Any) -> Optional[str]:
         """Finish suite/case/step/nested step item.
 
         :param item_id:     ID of the test item
         :param end_time:    The item end time
         :param status:      Test status. Allowable values: "passed",
                             "failed", "stopped", "skipped", "interrupted",
                             "cancelled" or None
@@ -208,15 +241,15 @@
         :param description: Test item description. Overrides description
                             from start request.
         :param issue:       Issue of the current test item
         :param retry:       Used to report retry of the test. Allowable values:
                            "True" or "False"
         """
         if item_id is NOT_FOUND or not item_id:
-            logger.warning("Attempt to finish non-existent item")
+            logger.warning('Attempt to finish non-existent item')
             return
         url = uri_join(self.base_url_v2, 'item', item_id)
         request_payload = ItemFinishRequest(
             end_time,
             self.launch_id,
             status,
             attributes=attributes,
@@ -230,26 +263,26 @@
         if not response:
             return
         self._item_stack.pop() if len(self._item_stack) > 0 else None
         logger.debug('finish_test_item - ID: %s', item_id)
         logger.debug('response message: %s', response.message)
         return response.message
 
-    def get_item_id_by_uuid(self, uuid):
+    def get_item_id_by_uuid(self, uuid: str) -> Optional[str]:
         """Get test item ID by the given UUID.
 
         :param uuid: UUID returned on the item start
         :return:     Test item ID
         """
         url = uri_join(self.base_url_v1, 'item', 'uuid', uuid)
         response = HttpRequest(self.session.get, url=url,
                                verify_ssl=self.verify_ssl).make()
         return response.id if response else None
 
-    def get_launch_info(self):
+    def get_launch_info(self) -> Optional[Dict]:
         """Get the current launch information.
 
         :return dict: Launch information in dictionary
         """
         if self.launch_id is None:
             return {}
         url = uri_join(self.base_url_v1, 'launch', 'uuid', self.launch_id)
@@ -264,77 +297,78 @@
                 'get_launch_info - Launch info: %s', response.json)
         else:
             logger.warning('get_launch_info - Launch info: '
                            'Failed to fetch launch ID from the API.')
             launch_info = {}
         return launch_info
 
-    def get_launch_ui_id(self):
+    def get_launch_ui_id(self) -> Optional[Dict]:
         """Get UI ID of the current launch.
 
         :return: UI ID of the given launch. None if UI ID has not been found.
         """
         launch_info = self.get_launch_info()
         return launch_info.get('id') if launch_info else None
 
-    def get_launch_ui_url(self):
+    def get_launch_ui_url(self) -> Optional[str]:
         """Get UI URL of the current launch.
 
         :return: launch URL or all launches URL.
         """
         launch_info = self.get_launch_info()
         ui_id = launch_info.get('id') if launch_info else None
         if not ui_id:
             return
         mode = launch_info.get('mode') if launch_info else None
         if not mode:
             mode = self.mode
 
-        launch_type = "launches" if mode.upper() == 'DEFAULT' else 'userdebug'
+        launch_type = 'launches' if mode.upper() == 'DEFAULT' else 'userdebug'
 
         path = 'ui/#{project_name}/{launch_type}/all/{launch_id}'.format(
             project_name=self.project.lower(), launch_type=launch_type,
             launch_id=ui_id)
         url = uri_join(self.endpoint, path)
         logger.debug('get_launch_ui_url - ID: %s', self.launch_id)
         return url
 
-    def get_project_settings(self):
+    def get_project_settings(self) -> Optional[Dict]:
         """Get project settings.
 
         :return: HTTP response in dictionary
         """
         url = uri_join(self.base_url_v1, 'settings')
         response = HttpRequest(self.session.get, url=url,
                                verify_ssl=self.verify_ssl).make()
         return response.json if response else None
 
-    def log(self, time, message, level=None, attachment=None, item_id=None):
+    def log(self, time: str, message: str, level: Optional[Union[int, str]] = None,
+            attachment: Optional[Dict] = None, item_id: Optional[str] = None) -> None:
         """Send log message to the Report Portal.
 
         :param time:       Time in UTC
         :param message:    Log message text
         :param level:      Message's log level
         :param attachment: Message's attachments
         :param item_id:    ID of the RP item the message belongs to
         """
         self._log_manager.log(time, message, level, attachment, item_id)
 
-    def start(self):
+    def start(self) -> None:
         """Start the client."""
         self._log_manager.start()
 
     def start_launch(self,
-                     name,
-                     start_time,
-                     description=None,
-                     attributes=None,
-                     rerun=False,
-                     rerun_of=None,
-                     **kwargs):
+                     name: str,
+                     start_time: str,
+                     description: Optional[str] = None,
+                     attributes: Optional[Union[List, Dict]] = None,
+                     rerun: bool = False,
+                     rerun_of: Optional[str] = None,
+                     **kwargs) -> Optional[str]:
         """Start a new launch with the given parameters.
 
         :param name:        Launch name
         :param start_time:  Launch start time
         :param description: Launch description
         :param attributes:  Launch attributes
         :param rerun:       Start launch in rerun mode
@@ -342,20 +376,24 @@
                             re-run. Should be used with the 'rerun' option.
         """
         url = uri_join(self.base_url_v2, 'launch')
 
         # We are moving 'mode' param to the constructor, next code for the
         # transition period only.
         my_kwargs = dict(kwargs)
-        if 'mode' in my_kwargs.keys():
-            mode = my_kwargs['mode']
+        mode = my_kwargs.get('mode')
+        if 'mode' in my_kwargs:
+            warnings.warn(
+                message='Argument `mode` is deprecated since 5.2.5 and will be subject for removing in the '
+                        'next major version. Use `mode` argument in the class constructor instead.',
+                category=DeprecationWarning,
+                stacklevel=2
+            )
             del my_kwargs['mode']
-            if not mode:
-                mode = self.mode
-        else:
+        if not mode:
             mode = self.mode
 
         request_payload = LaunchStartRequest(
             name=name,
             start_time=start_time,
             attributes=attributes,
             description=description,
@@ -379,29 +417,31 @@
             if len(agent_attribute) > 0 and agent_attribute[0].get('value'):
                 agent_name, agent_version = agent_attribute[0]['value'].split(
                     '|')
             send_event('start_launch', agent_name, agent_version)
 
         self._log_manager.launch_id = self.launch_id = response.id
         logger.debug('start_launch - ID: %s', self.launch_id)
+        if self.launch_uuid_print and self.print_output:
+            print(f'Report Portal Launch UUID: {self.launch_id}', file=self.print_output)
         return self.launch_id
 
     def start_test_item(self,
-                        name,
-                        start_time,
-                        item_type,
-                        description=None,
-                        attributes=None,
-                        parameters=None,
-                        parent_item_id=None,
-                        has_stats=True,
-                        code_ref=None,
-                        retry=False,
-                        test_case_id=None,
-                        **kwargs):
+                        name: str,
+                        start_time: str,
+                        item_type: str,
+                        description: Optional[str] = None,
+                        attributes: Optional[List[Dict]] = None,
+                        parameters: Optional[Dict] = None,
+                        parent_item_id: Optional[str] = None,
+                        has_stats: bool = True,
+                        code_ref: Optional[str] = None,
+                        retry: bool = False,
+                        test_case_id: Optional[str] = None,
+                        **_: Any) -> Optional[str]:
         """Start case/step/nested step item.
 
         :param name:           Name of the test item
         :param start_time:     The item start time
         :param item_type:      Type of the test item. Allowable values:
                                "suite", "story", "test", "scenario", "step",
                                "before_class", "before_groups",
@@ -415,16 +455,15 @@
         :param parameters:     Set of parameters (for parametrized test items)
         :param parent_item_id: An ID of a parent SUITE / STEP
         :param retry:          Used to report retry of the test. Allowable
                                values: "True" or "False"
         :param test_case_id: A unique ID of the current step
         """
         if parent_item_id is NOT_FOUND:
-            logger.warning("Attempt to start item for non-existent parent "
-                           "item")
+            logger.warning('Attempt to start item for non-existent parent item.')
             return
         if parent_item_id:
             url = uri_join(self.base_url_v2, 'item', parent_item_id)
         else:
             url = uri_join(self.base_url_v2, 'item')
         request_payload = ItemStartRequest(
             name,
@@ -451,19 +490,20 @@
             logger.debug('start_test_item - ID: %s', item_id)
             self._item_stack.append(item_id)
         else:
             logger.warning('start_test_item - invalid response: %s',
                            str(response.json))
         return item_id
 
-    def terminate(self, *args, **kwargs):
+    def terminate(self, *_: Any, **__: Any) -> None:
         """Call this to terminate the client."""
         self._log_manager.stop()
 
-    def update_test_item(self, item_uuid, attributes=None, description=None):
+    def update_test_item(self, item_uuid: str, attributes: Optional[Union[List, Dict]] = None,
+                         description: Optional[str] = None) -> Optional[str]:
         """Update existing test item at the Report Portal.
 
         :param str item_uuid:   Test item UUID returned on the item start
         :param str description: Test item description
         :param list attributes: Test item attributes
                                 [{'key': 'k_name', 'value': 'k_value'}, ...]
         """
@@ -476,19 +516,19 @@
         response = HttpRequest(self.session.put, url=url, json=data,
                                verify_ssl=self.verify_ssl).make()
         if not response:
             return
         logger.debug('update_test_item - Item: %s', item_id)
         return response.message
 
-    def current_item(self):
+    def current_item(self) -> Optional[str]:
         """Retrieve the last item reported by the client."""
         return self._item_stack[-1] if len(self._item_stack) > 0 else None
 
-    def clone(self):
+    def clone(self) -> 'RPClient':
         """Clone the client object, set current Item ID as cloned item ID.
 
         :returns: Cloned client object
         :rtype: RPClient
         """
         cloned = RPClient(
             endpoint=self.endpoint,
@@ -505,28 +545,28 @@
             mode=self.mode
         )
         current_item = self.current_item()
         if current_item:
             cloned._item_stack.append(current_item)
         return cloned
 
-    def __getstate__(self):
+    def __getstate__(self) -> Dict[str, Any]:
         """Control object pickling and return object fields as Dictionary.
 
         :returns: object state dictionary
         :rtype: dict
         """
         state = self.__dict__.copy()
         # Don't pickle 'session' field, since it contains unpickling 'socket'
         del state['session']
         # Don't pickle '_log_manager' field, since it uses 'session' field
         del state['_log_manager']
         return state
 
-    def __setstate__(self, state):
+    def __setstate__(self, state: Dict[str, Any]) -> None:
         """Control object pickling, receives object state as Dictionary.
 
         :param dict state: object state dictionary
         """
         self.__dict__.update(state)
         # Restore 'session' field
         self.__init_session()
```

### Comparing `reportportal-client-5.3.5/reportportal_client/core/__init__.py` & `reportportal-client-5.4.0/reportportal_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/core/rp_file.py` & `reportportal-client-5.4.0/reportportal_client/core/rp_file.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/core/rp_issues.py` & `reportportal-client-5.4.0/reportportal_client/core/rp_issues.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/core/rp_requests.py` & `reportportal-client-5.4.0/reportportal_client/core/rp_requests.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/core/rp_responses.py` & `reportportal-client-5.4.0/reportportal_client/core/rp_responses.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/core/test_manager.py` & `reportportal-client-5.4.0/reportportal_client/core/test_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/core/worker.py` & `reportportal-client-5.4.0/reportportal_client/core/worker.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/errors.py` & `reportportal-client-5.4.0/reportportal_client/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/helpers.py` & `reportportal-client-5.4.0/reportportal_client/helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/helpers.pyi` & `reportportal-client-5.4.0/reportportal_client/helpers.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/__init__.py` & `reportportal-client-5.4.0/reportportal_client/items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/item_weight.py` & `reportportal-client-5.4.0/reportportal_client/items/item_weight.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/rp_base_item.py` & `reportportal-client-5.4.0/reportportal_client/items/rp_base_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/rp_log_items/__init__.py` & `reportportal-client-5.4.0/reportportal_client/items/rp_log_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/rp_log_items/rp_log_item.py` & `reportportal-client-5.4.0/reportportal_client/items/rp_log_items/rp_log_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/__init__.py` & `reportportal-client-5.4.0/reportportal_client/items/rp_test_items/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_base_test_item.py` & `reportportal-client-5.4.0/reportportal_client/items/rp_test_items/rp_base_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_child_test_item.py` & `reportportal-client-5.4.0/reportportal_client/items/rp_test_items/rp_child_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/items/rp_test_items/rp_root_test_item.py` & `reportportal-client-5.4.0/reportportal_client/items/rp_test_items/rp_root_test_item.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/logs/__init__.py` & `reportportal-client-5.4.0/reportportal_client/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/logs/log_manager.py` & `reportportal-client-5.4.0/reportportal_client/logs/log_manager.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/services/__init__.py` & `reportportal-client-5.4.0/reportportal_client/services/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/services/client_id.py` & `reportportal-client-5.4.0/reportportal_client/services/client_id.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/services/constants.py` & `reportportal-client-5.4.0/reportportal_client/services/constants.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/services/statistics.py` & `reportportal-client-5.4.0/reportportal_client/services/statistics.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/static/__init__.py` & `reportportal-client-5.4.0/reportportal_client/static/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/static/abstract.py` & `reportportal-client-5.4.0/reportportal_client/static/abstract.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/static/defines.py` & `reportportal-client-5.4.0/reportportal_client/static/defines.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/static/errors.py` & `reportportal-client-5.4.0/reportportal_client/static/errors.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/steps/__init__.py` & `reportportal-client-5.4.0/reportportal_client/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client/steps/__init__.pyi` & `reportportal-client-5.4.0/reportportal_client/steps/__init__.pyi`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/reportportal_client.egg-info/PKG-INFO` & `reportportal-client-5.4.0/reportportal_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: reportportal-client
-Version: 5.3.5
+Version: 5.4.0
 Summary: Python client for Report Portal v5.
 Home-page: https://github.com/reportportal/client-Python
-Download-URL: https://github.com/reportportal/client-Python/tarball/5.3.5
+Download-URL: https://github.com/reportportal/client-Python/tarball/5.4.0
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0.
 Keywords: testing,reporting,reportportal,client
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `reportportal-client-5.3.5/reportportal_client.egg-info/SOURCES.txt` & `reportportal-client-5.4.0/reportportal_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 reportportal_client/__init__.py
 reportportal_client/client.py
-reportportal_client/client.pyi
 reportportal_client/errors.py
 reportportal_client/helpers.py
 reportportal_client/helpers.pyi
 reportportal_client.egg-info/PKG-INFO
 reportportal_client.egg-info/SOURCES.txt
 reportportal_client.egg-info/dependency_links.txt
 reportportal_client.egg-info/requires.txt
```

### Comparing `reportportal-client-5.3.5/setup.py` & `reportportal-client-5.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Config for setup package client Python."""
 
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = '5.3.5'
+__version__ = '5.4.0'
 
 TYPE_STUBS = ['*.pyi']
 
 
 def read_file(fname):
     """Read the given file.
```

### Comparing `reportportal-client-5.3.5/tests/test_client.py` & `reportportal-client-5.4.0/tests/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 #  https://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
+from io import StringIO
 
 import pytest
 from requests import Response
 from requests.exceptions import ReadTimeout
 from six.moves import mock
 
-from reportportal_client.helpers import timestamp
 from reportportal_client import RPClient
+from reportportal_client.helpers import timestamp
 
 
 def connection_error(*args, **kwargs):
     raise ReadTimeout()
 
 
 def response_error(*args, **kwargs):
@@ -192,7 +193,49 @@
 def test_empty_api_key_argument(warn):
     api_key = ''
     client = RPClient(endpoint='http://endpoint', project='project',
                       api_key=api_key)
 
     assert warn.call_count == 1
     assert client.api_key == api_key
+
+
+def test_launch_uuid_print():
+    str_io = StringIO()
+    client = RPClient(endpoint='http://endpoint', project='project',
+                      api_key='test', launch_uuid_print=True, print_output=str_io)
+    client.session = mock.Mock()
+    client._skip_analytics = True
+    client.start_launch('Test Launch', timestamp())
+    assert 'Report Portal Launch UUID: ' in str_io.getvalue()
+
+
+def test_no_launch_uuid_print():
+    str_io = StringIO()
+    client = RPClient(endpoint='http://endpoint', project='project',
+                      api_key='test', launch_uuid_print=False, print_output=str_io)
+    client.session = mock.Mock()
+    client._skip_analytics = True
+    client.start_launch('Test Launch', timestamp())
+    assert 'Report Portal Launch UUID: ' not in str_io.getvalue()
+
+
+@mock.patch('reportportal_client.client.sys.stdout', new_callable=StringIO)
+def test_launch_uuid_print_default_io(mock_stdout):
+    client = RPClient(endpoint='http://endpoint', project='project',
+                      api_key='test', launch_uuid_print=True)
+    client.session = mock.Mock()
+    client._skip_analytics = True
+    client.start_launch('Test Launch', timestamp())
+
+    assert 'Report Portal Launch UUID: ' in mock_stdout.getvalue()
+
+
+@mock.patch('reportportal_client.client.sys.stdout', new_callable=StringIO)
+def test_launch_uuid_print_default_print(mock_stdout):
+    client = RPClient(endpoint='http://endpoint', project='project',
+                      api_key='test')
+    client.session = mock.Mock()
+    client._skip_analytics = True
+    client.start_launch('Test Launch', timestamp())
+
+    assert 'Report Portal Launch UUID: ' not in mock_stdout.getvalue()
```

### Comparing `reportportal-client-5.3.5/tests/test_client_id.py` & `reportportal-client-5.4.0/tests/test_client_id.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/tests/test_helpers.py` & `reportportal-client-5.4.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `reportportal-client-5.3.5/tests/test_statistics.py` & `reportportal-client-5.4.0/tests/test_statistics.py`

 * *Files identical despite different names*

