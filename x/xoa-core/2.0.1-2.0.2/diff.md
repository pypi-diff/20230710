# Comparing `tmp/xoa-core-2.0.1.tar.gz` & `tmp/xoa-core-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-core-2.0.1.tar", last modified: Fri Jun 30 11:47:39 2023, max compression
+gzip compressed data, was "xoa-core-2.0.2.tar", last modified: Mon Jul 10 09:30:11 2023, max compression
```

## Comparing `xoa-core-2.0.1.tar` & `xoa-core-2.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-30 11:47:29.000000 xoa-core-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-30 11:47:39.321982 xoa-core-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-30 11:47:29.000000 xoa-core-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-30 11:47:29.000000 xoa-core-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 11:47:39.321982 xoa-core-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-30 11:47:29.000000 xoa-core-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.313982 xoa-core-2.0.1/xoa_core/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.313982 xoa-core-2.0.1/xoa_core/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/executor_state_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/executors/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/generic_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/messenger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/messenger/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/plugin_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.317982 xoa-core-2.0.1/xoa_core/core/resources/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/xoa_core/core/resources/resource/models/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/__decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/resource/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/resources/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/xoa_core/core/test_suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/test_suites/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.321982 xoa-core-2.0.1/xoa_core/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/utils/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/core/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 11:47:29.000000 xoa-core-2.0.1/xoa_core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:47:39.313982 xoa-core-2.0.1/xoa_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 11:47:39.000000 xoa-core-2.0.1/xoa_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.373297 xoa-core-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-10 09:30:00.000000 xoa-core-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-07-10 09:30:11.373297 xoa-core-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-10 09:30:00.000000 xoa-core-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 09:30:00.000000 xoa-core-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 09:30:11.377297 xoa-core-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-10 09:30:00.000000 xoa-core-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.369296 xoa-core-2.0.2/xoa_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.369296 xoa-core-2.0.2/xoa_core/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.369296 xoa-core-2.0.2/xoa_core/core/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/executor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/executor_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/executor_state_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/executors/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/generic_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.373297 xoa-core-2.0.2/xoa_core/core/messenger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/messenger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/messenger/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/messenger/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/messenger/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/plugin_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.373297 xoa-core-2.0.2/xoa_core/core/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.373297 xoa-core-2.0.2/xoa_core/core/resources/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.373297 xoa-core-2.0.2/xoa_core/core/resources/resource/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/models/__decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/models/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/models/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/models/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/resource/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/resources/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.373297 xoa-core-2.0.2/xoa_core/core/test_suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/test_suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/test_suites/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/test_suites/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/test_suites/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.373297 xoa-core-2.0.2/xoa_core/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/utils/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/core/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-10 09:30:00.000000 xoa-core-2.0.2/xoa_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:30:11.369296 xoa-core-2.0.2/xoa_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-07-10 09:30:11.000000 xoa-core-2.0.2/xoa_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-10 09:30:11.000000 xoa-core-2.0.2/xoa_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:30:11.000000 xoa-core-2.0.2/xoa_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 09:30:11.000000 xoa-core-2.0.2/xoa_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 09:30:11.000000 xoa-core-2.0.2/xoa_core.egg-info/top_level.txt
```

### Comparing `xoa-core-2.0.1/LICENSE` & `xoa-core-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/PKG-INFO` & `xoa-core-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-core
-Version: 2.0.1
+Version: 2.0.2
 Summary: Xena Open Automation framework for Xena test suite execution, integration, and development.
 Home-page: https://github.com/xenanetworks/open-automation-core
 Author: Artem Constantinov, Leonard Yu
 Author-email: aco@xenanetworks.com, hyu@xenanewtorks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-core-2.0.1/README.md` & `xoa-core-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/setup.py` & `xoa-core-2.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         author="Artem Constantinov, Leonard Yu",
         author_email="aco@xenanetworks.com, hyu@xenanewtorks.com",
         maintainer="Xena Networks",
         maintainer_email="support@xenanetworks.com",
         url="https://github.com/xenanetworks/open-automation-core",
         packages=setuptools.find_packages(),
         license='Apache 2.0',
-        install_requires=["xoa_driver>=2.0", "pydantic", "semver", "oyaml", "loguru"],
+        install_requires=["xoa_driver>=2.0", "pydantic==1.10.2", "semver", "oyaml",],
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
             "Topic :: Software Development :: Libraries :: Application Frameworks",
             "License :: OSI Approved :: Apache Software License",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
```

### Comparing `xoa-core-2.0.1/xoa_core/controller.py` & `xoa-core-2.0.2/xoa_core/controller.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/exceptions.py` & `xoa-core-2.0.2/xoa_core/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/executors/executor.py` & `xoa-core-2.0.2/xoa_core/core/executors/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,22 +36,24 @@
     @property
     def id(self) -> str:
         return self.__id
 
     def __on_execution_terminated(self, task: "asyncio.Task") -> None:
         if not self.state.is_stoped:
             self.state.set_stop()
+        err = None
+        with contextlib.suppress(asyncio.CancelledError, exceptions.StopPlugin):
+            err = task.exception()
+            if err is not None:
+                self.__msg_pipe.transmit_err(err)
+                self.__observer.emit(Event.ERROR, task.get_name(), err)  # only notify of the Execution manager.
         self.__observer.emit(Event.STOPPED, self.id)
         asyncio.create_task(self.__msg_pipe.disable())  # In rare case raise error but it's not break anything.
-        with contextlib.suppress(asyncio.CancelledError, exceptions.StopPlugin):
-            e = task.exception()
-            if e is None:
-                return None
-            self.__observer.emit(Event.ERROR, task.get_name(), e)
-            raise e
+        if err:
+            raise exceptions.ExecutionError(task.get_name()) from err
 
     def get_info(self) -> ExecutorInfo:
         return ExecutorInfo(
             id=self.__id,
             suite_name=self.suite_name,
             state=self.state.current_state,
         )
```

### Comparing `xoa-core-2.0.1/xoa_core/core/executors/executor_state.py` & `xoa-core-2.0.2/xoa_core/core/executors/executor_state.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/executors/executor_state_conditions.py` & `xoa-core-2.0.2/xoa_core/core/executors/executor_state_conditions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/executors/manager.py` & `xoa-core-2.0.2/xoa_core/core/executors/manager.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/generic_types.py` & `xoa-core-2.0.2/xoa_core/core/generic_types.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/messenger/handler.py` & `xoa-core-2.0.2/xoa_core/core/messenger/handler.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/messenger/misc.py` & `xoa-core-2.0.2/xoa_core/core/messenger/misc.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/messenger/pipe.py` & `xoa-core-2.0.2/xoa_core/core/messenger/pipe.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/plugin_abstract.py` & `xoa-core-2.0.2/xoa_core/core/plugin_abstract.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/controller.py` & `xoa-core-2.0.2/xoa_core/core/resources/controller.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/pool.py` & `xoa-core-2.0.2/xoa_core/core/resources/pool.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/resource/exceptions.py` & `xoa-core-2.0.2/xoa_core/core/resources/resource/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/resource/facade.py` & `xoa-core-2.0.2/xoa_core/core/resources/resource/facade.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/resource/misc.py` & `xoa-core-2.0.2/xoa_core/core/resources/resource/misc.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/resource/models/module.py` & `xoa-core-2.0.2/xoa_core/core/resources/resource/models/module.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/resource/models/port.py` & `xoa-core-2.0.2/xoa_core/core/resources/resource/models/port.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/resource/models/tester.py` & `xoa-core-2.0.2/xoa_core/core/resources/resource/models/tester.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/resource/models/types.py` & `xoa-core-2.0.2/xoa_core/core/resources/resource/models/types.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/resources/storage.py` & `xoa-core-2.0.2/xoa_core/core/resources/storage.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/test_suites/_loader.py` & `xoa-core-2.0.2/xoa_core/core/test_suites/_loader.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/test_suites/controller.py` & `xoa-core-2.0.2/xoa_core/core/test_suites/controller.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/test_suites/datasets.py` & `xoa-core-2.0.2/xoa_core/core/test_suites/datasets.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/utils/observer.py` & `xoa-core-2.0.2/xoa_core/core/utils/observer.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/core/utils/validators.py` & `xoa-core-2.0.2/xoa_core/core/utils/validators.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/exceptions.py` & `xoa-core-2.0.2/xoa_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core/types.py` & `xoa-core-2.0.2/xoa_core/types.py`

 * *Files identical despite different names*

### Comparing `xoa-core-2.0.1/xoa_core.egg-info/PKG-INFO` & `xoa-core-2.0.2/xoa_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-core
-Version: 2.0.1
+Version: 2.0.2
 Summary: Xena Open Automation framework for Xena test suite execution, integration, and development.
 Home-page: https://github.com/xenanetworks/open-automation-core
 Author: Artem Constantinov, Leonard Yu
 Author-email: aco@xenanetworks.com, hyu@xenanewtorks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-core-2.0.1/xoa_core.egg-info/SOURCES.txt` & `xoa-core-2.0.2/xoa_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

