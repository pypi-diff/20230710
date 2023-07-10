# Comparing `tmp/robocorp_tasks-2.1.1.tar.gz` & `tmp/robocorp_tasks-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-2.1.1.tar", max compression
+gzip compressed data, was "robocorp_tasks-2.1.2.tar", max compression
```

## Comparing `robocorp_tasks-2.1.1.tar` & `robocorp_tasks-2.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5432 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/README.md
--rw-r--r--   0        0        0     1240 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3502 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1467 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5121 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    10273 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1122 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     5080 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2160 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     3943 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5489 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     2436 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_toml_settings.py
--rw-r--r--   0        0        0      869 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     6211 1970-01-01 00:00:00.000000 robocorp_tasks-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5432 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/README.md
+-rw-r--r--   0        0        0     1240 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1467 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5121 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    10273 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1122 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     5084 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2160 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     4201 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5489 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     2436 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/_toml_settings.py
+-rw-r--r--   0        0        0      869 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-07-10 19:42:36.073083 robocorp_tasks-2.1.2/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     6211 1970-01-01 00:00:00.000000 robocorp_tasks-2.1.2/PKG-INFO
```

### Comparing `robocorp_tasks-2.1.1/README.md` & `robocorp_tasks-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/pyproject.toml` & `robocorp_tasks-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "2.1.1"
+version = "2.1.2"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
 license = "Apache-2.0"
```

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/__init__.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
 
 from ._protocols import ITask
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_callback.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_commands.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_commands.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_config.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_log_auto_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 def _log_before_task_run(task: ITask):
     log.start_task(
         task.name,
         task.module_name,
         task.filename,
-        task.method.__code__.co_firstlineno,
+        task.method.__code__.co_firstlineno + 1,
         getattr(task.method, "__doc__", ""),
     )
 
 
 def _log_after_task_run(task: ITask):
     status = task.status
     log.end_task(task.name, task.module_name, status, task.message)
```

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_protocols.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,21 +25,25 @@
         _: IExpectedProtocol = check_implements(self)
 
     Mypy should complain if `self` is not implementing the IExpectedProtocol.
     """
     return x
 
 
+# Note: this is a bit messy as we're mixing task states with log levels.
+# Note2: This is for the log.html and not really for user APIs.
 class Status:
     NOT_RUN = "NOT_RUN"  # Initial status for a task which is not run.
-    PASS = "PASS"
-    ERROR = "ERROR"
-    FAIL = "FAIL"
-    INFO = "INFO"
-    WARN = "WARN"
+    PASS = "PASS"  # Used for task pass
+    FAIL = "FAIL"  # Used for task failure
+
+    ERROR = "ERROR"  # log.critical
+    INFO = "INFO"  # log.info
+    WARN = "WARN"  # log.warn
+    DEBUG = "DEBUG"  # log.debug
 
 
 @dataclass
 class PyProjectInfo:
     pyproject: Path
     toml_contents: dict
```

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_task.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/_toml_settings.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/_toml_settings.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/src/robocorp/tasks/cli.py` & `robocorp_tasks-2.1.2/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.1/PKG-INFO` & `robocorp_tasks-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 2.1.1
+Version: 2.1.2
 Summary: The automation framework for Python
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

