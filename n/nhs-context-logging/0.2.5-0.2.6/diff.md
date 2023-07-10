# Comparing `tmp/nhs_context_logging-0.2.5.tar.gz` & `tmp/nhs_context_logging-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_context_logging-0.2.5.tar", max compression
+gzip compressed data, was "nhs_context_logging-0.2.6.tar", max compression
```

## Comparing `nhs_context_logging-0.2.5.tar` & `nhs_context_logging-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1159 2023-07-06 19:26:13.111002 nhs_context_logging-0.2.5/LICENSE.md
--rw-r--r--   0        0        0     7970 2023-07-06 19:26:13.111002 nhs_context_logging-0.2.5/README.md
--rw-r--r--   0        0        0     1636 2023-07-06 19:26:34.556195 nhs_context_logging-0.2.5/nhs_context_logging/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/constants.py
--rw-r--r--   0        0        0     1076 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/fixtures.py
--rw-r--r--   0        0        0     6063 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/formatters.py
--rw-r--r--   0        0        0     1685 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/handlers.py
--rw-r--r--   0        0        0    34935 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/logger.py
--rw-r--r--   0        0        0        0 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/py.typed
--rw-r--r--   0        0        0     3830 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/utils.py
--rw-r--r--   0        0        0     2808 2023-07-06 19:26:33.223993 nhs_context_logging-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      486 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0    38463 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/logger_tests.py
--rw-r--r--   0        0        0     4214 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/utils.py
--rw-r--r--   0        0        0     8392 1970-01-01 00:00:00.000000 nhs_context_logging-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1159 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/LICENSE.md
+-rw-r--r--   0        0        0     7970 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/README.md
+-rw-r--r--   0        0        0     1636 2023-07-10 17:21:09.353672 nhs_context_logging-0.2.6/nhs_context_logging/__init__.py
+-rw-r--r--   0        0        0     1487 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/nhs_context_logging/constants.py
+-rw-r--r--   0        0        0     1076 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/nhs_context_logging/fixtures.py
+-rw-r--r--   0        0        0     6063 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/nhs_context_logging/formatters.py
+-rw-r--r--   0        0        0     1685 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/nhs_context_logging/handlers.py
+-rw-r--r--   0        0        0    35287 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/nhs_context_logging/logger.py
+-rw-r--r--   0        0        0        0 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/nhs_context_logging/py.typed
+-rw-r--r--   0        0        0     3830 2023-07-10 17:20:48.257289 nhs_context_logging-0.2.6/nhs_context_logging/utils.py
+-rw-r--r--   0        0        0     2808 2023-07-10 17:21:08.257653 nhs_context_logging-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 17:20:48.261289 nhs_context_logging-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      486 2023-07-10 17:20:48.261289 nhs_context_logging-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0    39437 2023-07-10 17:20:48.261289 nhs_context_logging-0.2.6/tests/logger_tests.py
+-rw-r--r--   0        0        0     4214 2023-07-10 17:20:48.261289 nhs_context_logging-0.2.6/tests/utils.py
+-rw-r--r--   0        0        0     8392 1970-01-01 00:00:00.000000 nhs_context_logging-0.2.6/PKG-INFO
```

### Comparing `nhs_context_logging-0.2.5/LICENSE.md` & `nhs_context_logging-0.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.5/README.md` & `nhs_context_logging-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.5/nhs_context_logging/__init__.py` & `nhs_context_logging-0.2.6/nhs_context_logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nhs_context_logging.logger import (
     LogActionContextManager,
     TemporaryGlobalFieldsContextManager,
 )
 from nhs_context_logging.logger import app_logger as _app_logger
 from nhs_context_logging.logger import logging_context
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 DEFAULT_LOG_LEVEL = Constants.DEFAULT_LOG_LEVEL
 LOG_AT_LEVEL = Constants.LOG_AT_LEVEL
 LOG_LEVEL = Constants.LOG_LEVEL
 
 CRITICAL = _app_logger.CRITICAL
 FATAL = _app_logger.FATAL
```

### Comparing `nhs_context_logging-0.2.5/nhs_context_logging/constants.py` & `nhs_context_logging-0.2.6/nhs_context_logging/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     """provides shared constants for logging"""
 
     DEFAULT_LOG_LEVEL = logging.INFO
     DEFAULT_LOG_AT_LEVEL = "INFO"
 
     LOG_AT_LEVEL = "log_at_level"
     LOG_LEVEL = "log_level"
+    LOGGER_ERROR = "logger_error"
 
     ACTION_DURATION = "action_duration"
     ACTION_FIELD = "action"
     ACTION_STATUS = "action_status"
 
     # The function executed successfully and completed the happy path
     STATUS_SUCCEEDED = "succeeded"
```

### Comparing `nhs_context_logging-0.2.5/nhs_context_logging/fixtures.py` & `nhs_context_logging-0.2.6/nhs_context_logging/fixtures.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.5/nhs_context_logging/formatters.py` & `nhs_context_logging-0.2.6/nhs_context_logging/formatters.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.5/nhs_context_logging/handlers.py` & `nhs_context_logging-0.2.6/nhs_context_logging/handlers.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.5/nhs_context_logging/logger.py` & `nhs_context_logging-0.2.6/nhs_context_logging/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,26 @@
 _DEFAULT_REDACTIONS = {"password", ":password", "nhsnumber", "nhs_number", "authorization", "authorisation"}
 
 
 def uuid4_hex_string() -> str:
     return uuid4().hex
 
 
+class LoggerError(Exception):
+    pass
+
+
+class ActionNotInStack(LoggerError):
+    pass
+
+
+class MismatchedActionError(LoggerError):
+    pass
+
+
 class _Logger:
     CRITICAL = logging.CRITICAL
     FATAL = logging.CRITICAL
     ERROR = logging.ERROR
     AUDIT = 35
     WARNING = logging.WARN
     WARN = WARNING
@@ -516,15 +528,16 @@
             return typing.cast(FuncT, _async_gen_inner)
 
         if inspect.isgeneratorfunction(func):
 
             @wraps(func)
             def _sync_gen_inner(*args, **inner_kwargs):
                 with self._recreate_cm(func, _sync_gen_inner, *args, **inner_kwargs):
-                    yield from func(*args, **inner_kwargs)
+                    for res in func(*args, **inner_kwargs):
+                        yield res
 
             return typing.cast(FuncT, _sync_gen_inner)
 
         if inspect.iscoroutinefunction(func):
 
             @wraps(func)
             async def _async_inner(*args, **inner_kwargs):
@@ -594,21 +607,25 @@
 
         self.start_time = time()
 
         logging_context.push(self)
 
     def _end_action(self, exc_type, exc_val, exc_tb):
 
-        popped_action = logging_context.pop(self)
-        if popped_action != self:
-            raise ValueError("Mismatch action popped from stack!")
-
         message = {}
         message.update(self.fields)
 
+        try:
+            popped_action = logging_context.pop(self)
+            if popped_action != self:
+                raise MismatchedActionError("Mismatch action popped from stack!")
+        except ActionNotInStack as err:
+            message[Constants.LOG_LEVEL] = logging.WARNING
+            message[Constants.LOGGER_ERROR] = err
+
         self.end_time = time()
 
         if self.end_time is not None and self.start_time is not None:
             message[Constants.ACTION_DURATION] = message.get(
                 Constants.ACTION_DURATION, float(f"{(self.end_time - self.start_time):0.7f}")
             )
 
@@ -907,15 +924,15 @@
 
         stack = self.storage.stack
 
         for i in range(len(stack), 0, -1):
             if stack[i - 1] != item:
                 continue
             return typing.cast(LogActionContextManager, stack.pop(i - 1))
-        raise ValueError("item not found")
+        raise ActionNotInStack()
 
     def current(self) -> Optional[LogActionContextManager]:
         return typing.cast(Optional[LogActionContextManager], self.storage.current_context)
 
     def current_internal_id(self) -> str:
 
         current_action = self.current()
```

### Comparing `nhs_context_logging-0.2.5/nhs_context_logging/utils.py` & `nhs_context_logging-0.2.6/nhs_context_logging/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.5/pyproject.toml` & `nhs_context_logging-0.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs_context_logging"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["spinecore"]
 license = "GPLv3"
 packages = [
     { include = "nhs_context_logging" },
     { include = "tests", format = "sdist" },
 ]
```

### Comparing `nhs_context_logging-0.2.5/tests/logger_tests.py` & `nhs_context_logging-0.2.6/tests/logger_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     temporary_global_fields,
 )
 from nhs_context_logging.formatters import (
     JSONFormatter,
     KeyValueFormatter,
     StructuredFormatter,
 )
+from nhs_context_logging.logger import ActionNotInStack
 from tests.utils import concurrent_tasks, create_task, run_in_executor
 
 
 def assert_single_internal_id(log_capture: Tuple[List[dict], List[dict]]):
     internal_ids = {line["internal_id"] for line in (log_capture[0] + log_capture[1])}
     assert len(internal_ids) == 1, internal_ids
 
@@ -532,14 +533,44 @@
     assert_single_internal_id(log_capture)
     std_out, std_err = log_capture
     assert len(std_err) == 0
     assert len(std_out) == 1
     assert std_out[0]["log_info"]["level"] == "INFO"
 
 
+async def test_end_action_when_action_already_popped(log_capture: Tuple[List[dict], List[dict]], tmp_path):
+
+    async with log_action(internal_id="bob") as action:
+        logging_context.pop(action)
+
+    std_out, std_err = log_capture
+
+    assert not std_err
+    assert len(std_out) == 1
+    assert type(std_out[0]["logger_error"]) == ActionNotInStack
+    assert std_out[0]["log_info"]["level"] == "WARNING"
+
+
+async def test_end_action_when_action_already_popped_with_exception(
+    log_capture: Tuple[List[dict], List[dict]], tmp_path
+):
+
+    with pytest.raises(ValueError):
+        async with log_action(internal_id="bob") as action:
+            logging_context.pop(action)
+            raise ValueError()
+
+    std_out, std_err = log_capture
+
+    assert not std_out
+    assert len(std_err) == 1
+    assert type(std_err[0]["logger_error"]) == ActionNotInStack
+    assert std_err[0]["log_info"]["level"] == "ERROR"
+
+
 async def test_async_logging_context_run_in_executor(log_capture: Tuple[List[dict], List[dict]]):
     logging_context.setup_async()
     global_id = uuid4().hex
 
     std_out, std_err = log_capture
 
     @log_action()
```

### Comparing `nhs_context_logging-0.2.5/tests/utils.py` & `nhs_context_logging-0.2.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.5/PKG-INFO` & `nhs_context_logging-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-context-logging
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 License: GPLv3
 Author: spinecore
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

