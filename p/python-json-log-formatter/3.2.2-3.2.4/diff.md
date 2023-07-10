# Comparing `tmp/python_json_log_formatter-3.2.2.tar.gz` & `tmp/python_json_log_formatter-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_json_log_formatter-3.2.2.tar", last modified: Fri Jun  2 16:01:43 2023, max compression
+gzip compressed data, was "python_json_log_formatter-3.2.4.tar", last modified: Mon Jul 10 12:52:04 2023, max compression
```

## Comparing `python_json_log_formatter-3.2.2.tar` & `python_json_log_formatter-3.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-06-02 16:01:43.024443 python_json_log_formatter-3.2.2/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.2.2/LICENSE
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-06-02 16:01:43.024285 python_json_log_formatter-3.2.2/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2793 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/README.md
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      945 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/pyproject.toml
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-06-02 16:01:43.023209 python_json_log_formatter-3.2.2/python_json_log_formatter/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1195 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/__init__.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       93 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/__init__.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       21 2023-06-02 16:00:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/_version.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       16 2023-06-02 14:51:25.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/_version.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)    12647 2023-06-02 16:00:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      553 2023-06-02 14:51:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/py.typed
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     5397 2023-06-02 14:13:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      574 2023-06-02 14:51:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.pyi
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-06-02 16:01:43.024060 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      617 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/top_level.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-06-02 16:01:43.024490 python_json_log_formatter-3.2.2/setup.cfg
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 12:52:04.405762 python_json_log_formatter-3.2.4/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.2.4/LICENSE
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-07-10 12:52:04.405596 python_json_log_formatter-3.2.4/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2793 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/README.md
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      945 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/pyproject.toml
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 12:52:04.404191 python_json_log_formatter-3.2.4/python_json_log_formatter/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1195 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/__init__.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       93 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/__init__.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       21 2023-07-10 12:42:58.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/_version.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       16 2023-06-02 14:51:25.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/_version.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    13567 2023-07-10 12:48:01.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      605 2023-07-10 12:48:10.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/py.typed
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     5425 2023-07-10 12:45:52.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      574 2023-06-02 14:51:06.000000 python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.pyi
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-07-10 12:52:04.405376 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      617 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-07-10 12:52:04.000000 python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/top_level.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-07-10 12:52:04.405820 python_json_log_formatter-3.2.4/setup.cfg
```

### Comparing `python_json_log_formatter-3.2.2/LICENSE` & `python_json_log_formatter-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.2/PKG-INFO` & `python_json_log_formatter-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_json_log_formatter
-Version: 3.2.2
+Version: 3.2.4
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.2.2 Summary:
+Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.2.4 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
```

### Comparing `python_json_log_formatter-3.2.2/README.md` & `python_json_log_formatter-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.2/pyproject.toml` & `python_json_log_formatter-3.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.2/python_json_log_formatter/__init__.py` & `python_json_log_formatter-3.2.4/python_json_log_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.py` & `python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,25 +28,32 @@
 
 from __future__ import annotations
 
 import json
 from logging import CRITICAL, ERROR, LogRecord, Filter, WARNING, Logger, getLevelName, getLogger
 from pathlib import Path
 import traceback
-from typing import Any, Dict, List, Mapping
+from typing import Any, ClassVar, Dict, List, Mapping
 from os import getenv, getcwd
 
 LOGGER: Logger = getLogger(__name__)
 
 class ContextFilter(Filter):
     """
     This is a filter which transforms log lines with metadata into structured JSON log lines.
     These structured JSON log lines are automatically parsed and indexed by LogDNA.
     """
 
+    @property
+    def message_key(self):
+        return self.__message_key
+
+    __message_key: ClassVar[str] = "msg"
+    """name of the key under which the msg will be saved"""
+
     __job_retry_limit_env = "JOB_RETRY_LIMIT"
     """ENV-Key of the retry limit per job, name defined by Code Engine"""
 
     __job_retry_count_env = "JOB_INDEX_RETRY_COUNT"
     """ENV-Key of the current re-try count per job, name defined by Code Engine"""
 
     __job_remaining_retries = "job_remaining_retries"
@@ -182,23 +189,33 @@
         # add all available attributes of the record
         # copy to ensure to not edit the record itself
         new_dict: Dict[str, Any] = record.__dict__.copy()
 
         for key in self.__excluded_logging_context_keys:
             new_dict.pop(key, None)
 
+        # without specifying this level, the logging service cannot detect its level
+        # so this is super important
         new_dict["level"] = record.levelname
-        new_dict["message"] = record.msg
+        new_dict[self.__message_key] = record.msg
+
+        if self.__message_key != "msg":
+            # remove msg as it is saved in another name
+            # message is used in the formatting string
+            new_dict.pop("msg", None)
 
         # Add arguments individual to the new record message
         if isinstance(record.args, dict):
             for k, v in record.args.items():
                 new_dict[k] = v
+
             # set them to empty, as already included
-            record.args = {}
+            #record.args = {}
+            # Edit: do not remove it, as the record should be left as intact as possible
+
             # remove it from the new_dict, as they are saved individually
             new_dict.pop("args", None)
 
         return new_dict
 
     def __add_available_exec_info(self, new_record_dict: Dict[str, Any], record: LogRecord):
         """Updates the provided context information with exc_information from the log record.
@@ -207,31 +224,33 @@
         Updates the message of the context dict.
 
         Args:
             new_record_dict (Dict[str, Any]): Context dict with existing message and other information
             record (LogRecord): LogRecord with possible exc_info field
         """
 
-        message = new_record_dict['message']
+        message = new_record_dict[self.__message_key]
 
         if record.exc_info:
 
             # get the individual parts
             exc_type, exc_value, exc_traceback = record.exc_info
 
             # only save the trace
             exc_info = ''.join(traceback.format_exception(exc_type, exc_value, exc_traceback))
 
             # delete the info from the saved dict
             new_record_dict.pop("exc_info", None)
+
             # Clear record.exc_info
-            record.exc_info = None
+            #record.exc_info = None
+            # Edit: do not remove it, as the record should be left as intact as possible
 
             # append it to the message to have it displayed as log message
-            new_record_dict['message'] = message + '\n' + exc_info
+            new_record_dict[self.__message_key] = message + '\n' + exc_info
 
     def __check_is_imported_module(self, path_name: str) -> bool:
         work_dir = Path(getcwd())
         log_path = Path(path_name)
 
         # from python 3.9 the main module should always be absolute, but sometimes it is not somehow.
         # make sure the path is absolute
@@ -299,33 +318,38 @@
             new_dict['job_status'] = 'failed'
             new_dict['pipeline_status'] = 'failed'
 
         return new_dict
 
     def filter(self, record: LogRecord) -> bool:
         """Combine message and contextual information into message argument of the record."""
+        try:
 
-        # start with the pre-set context
-        new_record_msg: Dict[str, Any] = self.__context.copy()
+            # start with the pre-set context
+            new_record_msg: Dict[str, Any] = self.__context.copy()
 
-        new_dict = self.__filter_imported_modules(record)
-        new_record_msg.update(new_dict)
+            new_dict = self.__filter_imported_modules(record)
+            new_record_msg.update(new_dict)
 
-        new_dict = self.__add_log_record_info(record)
-        new_record_msg.update(new_dict)
+            new_dict = self.__add_log_record_info(record)
+            new_record_msg.update(new_dict)
 
-        new_dict = self.__check_failed_pipeline_status(record)
-        new_record_msg.update(new_dict)
+            new_dict = self.__check_failed_pipeline_status(record)
+            new_record_msg.update(new_dict)
 
-        # Add exception info to log message
-        self.__add_available_exec_info(new_record_msg, record)
+            # Add exception info to log message
+            self.__add_available_exec_info(new_record_msg, record)
 
-        # Override record message and clear record args
-        dumped_new_dict = json.dumps(new_record_msg)
-        if not self.__disable_log_formatting:
             # Override record message and clear record args
-            record.msg = dumped_new_dict
-        else:
-            # save it in new attribute, will not be shown.
-            record.log_formatting_message = dumped_new_dict
+            dumped_new_dict = json.dumps(new_record_msg)
+            if not self.__disable_log_formatting:
+                # Override record message and clear record args
+                record.msg = dumped_new_dict
+            else:
+                # save it in new attribute, will not be shown.
+                record.log_formatting_message = dumped_new_dict
+
+        except Exception:
+            # ensure it does not stop the program if something does wrong
+            return True
 
         return True
```

### Comparing `python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.pyi` & `python_json_log_formatter-3.2.4/python_json_log_formatter/context_filter.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from logging import Filter, LogRecord, Logger
 from typing import Dict, List, Mapping
 
 LOGGER: Logger
 
 class ContextFilter(Filter):
     @property
+    def message_key(self) -> str: ...
+    @property
     def excluded_logging_context_keys(self) -> List[str]: ...
     @excluded_logging_context_keys.setter
     def excluded_logging_context_keys(self, value: List[str]) -> None: ...
     def __init__(self, context: Dict[str, str], disable_log_formatting: bool = ...) -> None: ...
     def update_context(self, new_context_dict: Mapping[str, str]) -> None: ...
     def filter(self, record: LogRecord) -> bool: ...
```

### Comparing `python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.py` & `python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             context_dict["app"] = app
         context_dict["version"] = version_constant
         context_dict["logger_version"] = __version__
         cls.__context_filter = ContextFilter(context_dict, disable_log_formatting)
         handler.addFilter(cls.__context_filter)
         basicConfig(
             level=logging_level,
-            format="[%(asctime)s %(name)s] %(levelname)s: %(message)s",
+            format=f"[%(asctime)s %(name)s] %(levelname)s: %({cls.__context_filter.message_key})s",
             handlers=[handler]
     )
 
     @classmethod
     def update_context(cls, context: Dict[str, str]) -> None:
         """Updates additional context information added to each log line.
```

### Comparing `python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.pyi` & `python_json_log_formatter-3.2.4/python_json_log_formatter/python_json_log_formatter.pyi`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/PKG-INFO` & `python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-json-log-formatter
-Version: 3.2.2
+Version: 3.2.4
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.2.2 Summary:
+Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.2.4 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
```

### Comparing `python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/SOURCES.txt` & `python_json_log_formatter-3.2.4/python_json_log_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

