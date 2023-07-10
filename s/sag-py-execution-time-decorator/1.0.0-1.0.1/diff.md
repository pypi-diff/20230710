# Comparing `tmp/sag-py-execution-time-decorator-1.0.0.tar.gz` & `tmp/sag-py-execution-time-decorator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-execution-time-decorator-1.0.0.tar", last modified: Mon May  8 11:20:01 2023, max compression
+gzip compressed data, was "sag-py-execution-time-decorator-1.0.1.tar", last modified: Mon Jul 10 04:42:39 2023, max compression
```

## Comparing `sag-py-execution-time-decorator-1.0.0.tar` & `sag-py-execution-time-decorator-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/execution_time_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 11:20:01.000000 sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:20:01.092942 sag-py-execution-time-decorator-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-08 11:19:48.000000 sag-py-execution-time-decorator-1.0.0/tests/test_execution_time_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/execution_time_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 04:42:39.197239 sag-py-execution-time-decorator-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/tests/test_execution_time_decorator.py
```

### Comparing `sag-py-execution-time-decorator-1.0.0/LICENSE.txt` & `sag-py-execution-time-decorator-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-1.0.0/PKG-INFO` & `sag-py-execution-time-decorator-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-execution-time-decorator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A decorator for methods to log the execution time (sync and async)
 Home-page: https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_execution_time_decorator/issues
@@ -48,25 +48,27 @@
 
 @log_execution_time()
 def decorated_sync_method(param: str) -> str:
     time.sleep(SLEEP_TIME_MS / 1000)
     return f"test: {param}"
 
 
-@log_execution_time(log_level=logging.ERROR)
+@log_execution_time(log_level=logging.ERROR, log_params=("param",))
 async def decorated_async_method(param: str) -> str:
     await asyncio.sleep(SLEEP_TIME_MS / 1000)
     return f"test: {param}"
+
 ```
 
 Optional arguments:
 | Argument    | Description                                                          | Default                  |
 |-------------|----------------------------------------------------------------------|--------------------------|
 | log_level   | The log level integar. Use logging.* constants                       | logging.INFO             |
 | logger_name | The name of the logger that is internally used for logging.getLogger | execution_time_decorator |
+| log_params  | A tuple of parameter names to be logged with their values in 'extra' | ()                       |
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
```

### Comparing `sag-py-execution-time-decorator-1.0.0/README.md` & `sag-py-execution-time-decorator-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,27 @@
 
 @log_execution_time()
 def decorated_sync_method(param: str) -> str:
     time.sleep(SLEEP_TIME_MS / 1000)
     return f"test: {param}"
 
 
-@log_execution_time(log_level=logging.ERROR)
+@log_execution_time(log_level=logging.ERROR, log_params=("param",))
 async def decorated_async_method(param: str) -> str:
     await asyncio.sleep(SLEEP_TIME_MS / 1000)
     return f"test: {param}"
+
 ```
 
 Optional arguments:
 | Argument    | Description                                                          | Default                  |
 |-------------|----------------------------------------------------------------------|--------------------------|
 | log_level   | The log level integar. Use logging.* constants                       | logging.INFO             |
 | logger_name | The name of the logger that is internally used for logging.getLogger | execution_time_decorator |
+| log_params  | A tuple of parameter names to be logged with their values in 'extra' | ()                       |
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
```

### Comparing `sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/PKG-INFO` & `sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-execution-time-decorator
-Version: 1.0.0
+Version: 1.0.1
 Summary: A decorator for methods to log the execution time (sync and async)
 Home-page: https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_execution_time_decorator/issues
@@ -48,25 +48,27 @@
 
 @log_execution_time()
 def decorated_sync_method(param: str) -> str:
     time.sleep(SLEEP_TIME_MS / 1000)
     return f"test: {param}"
 
 
-@log_execution_time(log_level=logging.ERROR)
+@log_execution_time(log_level=logging.ERROR, log_params=("param",))
 async def decorated_async_method(param: str) -> str:
     await asyncio.sleep(SLEEP_TIME_MS / 1000)
     return f"test: {param}"
+
 ```
 
 Optional arguments:
 | Argument    | Description                                                          | Default                  |
 |-------------|----------------------------------------------------------------------|--------------------------|
 | log_level   | The log level integar. Use logging.* constants                       | logging.INFO             |
 | logger_name | The name of the logger that is internally used for logging.getLogger | execution_time_decorator |
+| log_params  | A tuple of parameter names to be logged with their values in 'extra' | ()                       |
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
```

### Comparing `sag-py-execution-time-decorator-1.0.0/sag_py_execution_time_decorator.egg-info/SOURCES.txt` & `sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-1.0.0/setup.py` & `sag-py-execution-time-decorator-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-execution-time-decorator",
-    version="1.0.0",
+    version="1.0.1",
     description="A decorator for methods to log the execution time (sync and async)",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_execution_time_decorator",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-execution-time-decorator-1.0.0/tests/test_execution_time_decorator.py` & `sag-py-execution-time-decorator-1.0.1/tests/test_execution_time_decorator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import asyncio
 import logging
 from typing import Any, cast
 from unittest import TestCase
 
 from sag_py_execution_time_decorator.execution_time_decorator import _calculate_and_log_execution_time
-from tests.test_data import SLEEP_TIME_MS, decorated_async_method, decorated_sync_method
+from tests.test_data import (
+    SLEEP_TIME_MS,
+    decorated_async_method,
+    decorated_async_method_extra_params,
+    decorated_sync_method,
+    decorated_sync_method_extra_params,
+)
 
 
 class PredictionControllerTest(TestCase):
     def test_log_execution_time_sync_function(self) -> None:
         # Act
         with self.assertLogs() as log_watcher:
             actual = decorated_sync_method("input")
@@ -30,19 +36,51 @@
 
             # Assert
             log_record = cast(Any, log_watcher.records[0])
             self.assertAlmostEqual(log_record.execution_time, SLEEP_TIME_MS, delta=100)
             self.assertEqual(log_record.function_name, "decorated_async_method")
             self.assertEqual(log_record.levelname, "ERROR")
             self.assertEqual(actual, "test: input")
+            self.assertTrue("param" not in log_record.__dict__.keys())
 
     def test__calculate_and_log_execution_time(self) -> None:
         # Act
         with self.assertLogs() as log_watcher:
             _calculate_and_log_execution_time(1683537228701, 1683537229702, "my_logger", logging.INFO, "my_func_name")
 
             # Assert
             log_record = cast(Any, log_watcher.records[0])
             self.assertEqual(log_record.execution_time, 1001)
             self.assertEqual(log_record.name, "my_logger")
             self.assertEqual(log_record.levelname, "INFO")
             self.assertEqual(log_record.function_name, "my_func_name")
+            self.assertTrue("param" not in log_record.__dict__.keys())
+
+    def test_log_execution_time_sync_extra_params_function(self) -> None:
+        # Act
+        with self.assertLogs() as log_watcher:
+            actual = decorated_sync_method_extra_params("input")
+
+            # Assert
+            log_record = cast(Any, log_watcher.records[0])
+            self.assertAlmostEqual(log_record.execution_time, SLEEP_TIME_MS, delta=100)
+            self.assertEqual(log_record.function_name, "decorated_sync_method_extra_params")
+            self.assertEqual(log_record.levelname, "INFO")
+            assert set({"param": "input"}.items()).issubset(set(log_record.__dict__.items()))
+            self.assertTrue("foo" not in log_record.__dict__.keys())
+            self.assertEqual(actual, "test: input")
+
+    def test_log_execution_time_async_extra_params_function(self) -> None:
+        # Arrange
+        loop = asyncio.get_event_loop()
+
+        # Act
+        with self.assertLogs() as log_watcher:
+            actual = loop.run_until_complete(decorated_async_method_extra_params("input"))
+
+            # Assert
+            log_record = cast(Any, log_watcher.records[0])
+            self.assertAlmostEqual(log_record.execution_time, SLEEP_TIME_MS, delta=100)
+            self.assertEqual(log_record.function_name, "decorated_async_method_extra_params")
+            self.assertEqual(log_record.levelname, "INFO")
+            assert set({"param": "input"}.items()).issubset(set(log_record.__dict__.items()))
+            self.assertEqual(actual, "test: input")
```

