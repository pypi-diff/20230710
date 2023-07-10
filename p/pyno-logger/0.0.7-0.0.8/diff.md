# Comparing `tmp/pyno_logger-0.0.7.tar.gz` & `tmp/pyno_logger-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ben/projects/open-source/pyno-logger/dist/.tmp-v9_eq_ml/pyno_logger-0.0.7.tar", last modified: Sat Jul  8 01:22:30 2023, max compression
+gzip compressed data, was "pyno_logger-0.0.8.tar", last modified: Mon Jul 10 06:02:17 2023, max compression
```

## Comparing `pyno_logger-0.0.7.tar` & `pyno_logger-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:22:30.325380 pyno_logger-0.0.7/
--rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.7/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     5783 2023-07-08 01:22:30.325252 pyno_logger-0.0.7/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     5265 2023-07-08 01:22:18.000000 pyno_logger-0.0.7/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:22:30.324616 pyno_logger-0.0.7/pyno_logger/
--rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.7/pyno_logger/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     5771 2023-07-08 01:15:39.000000 pyno_logger-0.0.7/pyno_logger/pyno_logger.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-08 01:22:30.325088 pyno_logger-0.0.7/pyno_logger.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     5783 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-08 01:22:30.000000 pyno_logger-0.0.7/pyno_logger.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-08 01:22:24.000000 pyno_logger-0.0.7/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-08 01:22:30.325431 pyno_logger-0.0.7/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:02:17.993774 pyno_logger-0.0.8/
+-rw-r--r--   0 ben        (501) staff       (20)     1066 2023-07-07 05:59:36.000000 pyno_logger-0.0.8/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     5981 2023-07-10 06:02:17.993656 pyno_logger-0.0.8/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     5463 2023-07-10 05:59:28.000000 pyno_logger-0.0.8/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:02:17.993000 pyno_logger-0.0.8/pyno_logger/
+-rw-r--r--   0 ben        (501) staff       (20)       30 2023-07-07 19:29:37.000000 pyno_logger-0.0.8/pyno_logger/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     5999 2023-07-10 05:47:16.000000 pyno_logger-0.0.8/pyno_logger/pyno_logger.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-10 06:02:17.993474 pyno_logger-0.0.8/pyno_logger.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     5981 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      223 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-10 06:02:17.000000 pyno_logger-0.0.8/pyno_logger.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      503 2023-07-10 06:00:22.000000 pyno_logger-0.0.8/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2023-07-10 06:02:17.993815 pyno_logger-0.0.8/setup.cfg
```

### Comparing `pyno_logger-0.0.7/LICENSE` & `pyno_logger-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyno_logger-0.0.7/PKG-INFO` & `pyno_logger-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno_logger
-Version: 0.0.7
+Version: 0.0.8
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,20 +36,24 @@
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
 - `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
 - `base` (optional): Dictionary with any base configuration that is applied to all logs.
 
+- `enabled` (optional): Boolean value that sets the enabled state of the logger.
+
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
 
+- `redact_value` (optional): Custom value for any keys that are redacted during a log.
+
 - `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
-- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys.
+- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission.
 - `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
 ### Logging Methods
@@ -62,15 +66,15 @@
 - `debug(data={}, message=None)`: Logs a debug message with the provided data and an optional message.
 - `trace(data={}, message=None)`: Logs a trace message with the provided data and an optional message.
 - `error(data={}, message=None)`: Logs an error message with the provided data and an optional message.
 - `fatal(data={}, message=None)`: Logs a fatal error message with the provided data and an optional message.
 
 Each logging method takes two optional arguments: `data` and `message`. The `data` argument can be a dictionary, list, tuple, string, or Exception object containing additional contextual data. The `message` argument is a string that represents the log message. If not provided, the log message will be automatically generated based on the log level and data.
 
-By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omitted_keys` config param, if desired.
+By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omit` config param, if desired.
 
 ### Log Levels
 
 Pyno uses the following log levels:
 
 - `FATAL`: 60
 - `ERROR`: 50
```

### Comparing `pyno_logger-0.0.7/README.md` & `pyno_logger-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,24 @@
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
 - `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
 - `base` (optional): Dictionary with any base configuration that is applied to all logs.
 
+- `enabled` (optional): Boolean value that sets the enabled state of the logger.
+
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
 
+- `redact_value` (optional): Custom value for any keys that are redacted during a log.
+
 - `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
-- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys.
+- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission.
 - `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
 ### Logging Methods
@@ -48,15 +52,15 @@
 - `debug(data={}, message=None)`: Logs a debug message with the provided data and an optional message.
 - `trace(data={}, message=None)`: Logs a trace message with the provided data and an optional message.
 - `error(data={}, message=None)`: Logs an error message with the provided data and an optional message.
 - `fatal(data={}, message=None)`: Logs a fatal error message with the provided data and an optional message.
 
 Each logging method takes two optional arguments: `data` and `message`. The `data` argument can be a dictionary, list, tuple, string, or Exception object containing additional contextual data. The `message` argument is a string that represents the log message. If not provided, the log message will be automatically generated based on the log level and data.
 
-By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omitted_keys` config param, if desired.
+By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omit` config param, if desired.
 
 ### Log Levels
 
 Pyno uses the following log levels:
 
 - `FATAL`: 60
 - `ERROR`: 50
```

### Comparing `pyno_logger-0.0.7/pyno_logger/pyno_logger.py` & `pyno_logger-0.0.8/pyno_logger/pyno_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,46 +26,49 @@
     name = None
     base_ctx = {
         "hostname": gethostname(),
         "pid": getpid(),
     }
     log_level = getenv("LOG_LEVEL") or "INFO"
 
+    config = {}
     omitted_keys = []
     redacted_keys = []
     newlines = False
     msg_key = "msg"
     error_key = "error"
+    redact_value = "[REDACTED]"
     enabled = True
 
     mixin = None
 
     def __init__(self, config={}, mixin=None, name=None):
         if self.log_level not in LogLevel.keys():
             raise Exception(f"Invalid log level: {self.log_level}")
 
         if isinstance(name, str):
             self.name = name
 
         if isinstance(name, dict):
             self.base_ctx = {**self.base_ctx, **name}
 
-        self.set_config(config, mixin)
+        self.config = config
+        self.mixin = mixin
+        self.__set_config()
 
     def enabled(self, enabled):
         self.enabled = enabled
 
     def child(self, name):
-        child_logger = Pyno(mixin=self.mixin, name=name)
-        child_logger.omitted_keys = self.omitted_keys
-        child_logger.newlines = self.newlines
-        child_logger.log_level = self.log_level
+        child_logger = Pyno(config=self.config, mixin=self.mixin, name=name)
         return child_logger
 
-    def set_config(self, config={}, mixin=None):
+    def __set_config(self):
+        config = self.config
+        mixin = self.mixin
         if config.get("omit"):
             omitted_keys = config["omit"]
             if isinstance(omitted_keys, list):
                 self.omitted_keys = omitted_keys
             elif isinstance(omitted_keys, tuple):
                 self.omitted_keys = list(omitted_keys)
             elif isinstance(omitted_keys, str):
@@ -86,27 +89,32 @@
         if (
             config.get("level")
             and isinstance(config["level"], str)
             and config["level"] in LogLevel.keys()
         ):
             self.log_level = config["level"]
 
-        if mixin and callable(mixin):
-            self.mixin = mixin
+        self.mixin = mixin if mixin and callable(mixin) else None
 
         if config.get("base"):
             if isinstance(config["base"], dict):
                 self.base_ctx = {**self.base_ctx, **config["base"]}
 
         if config.get("msg_key") and isinstance(config["msg_key"], str):
             self.msg_key = config["msg_key"]
 
         if config.get("error_key") and isinstance(config["error_key"], str):
             self.error_key = config["error_key"]
 
+        if config.get("enabled") and isinstance(config["enabled"], bool):
+            self.enabled = config["enabled"]
+
+        if config.get("redact_value") and isinstance(config["redact_value"], str):
+            self.redact_value = config["redact_value"]
+
     def log(self, level, data, message=None):
         level_num = LogLevel.get(level)
 
         if not level_num or not isinstance(level_num, int):
             raise Exception(f"Invalid log level: {level}")
 
         if self.log_level == "SILENT" or level_num == 0 or not self.enabled:
@@ -114,16 +122,15 @@
 
         base_data = {"time": int(time.time())}
 
         if self.name:
             base_data["name"] = self.name
 
         if len(self.base_ctx.keys()):
-            for key, val in self.base_ctx.items():
-                base_data[key] = val
+            base_data = {**base_data, **self.base_ctx}
 
         if level_num >= LogLevel.get(self.log_level):
             ctx = {}
             msg = message
 
             if isinstance(data, list) or isinstance(data, tuple):
                 for index, item in enumerate(data):
@@ -155,15 +162,15 @@
                 for key in self.omitted_keys:
                     if key in to_log:
                         del to_log[key]
 
             if len(self.redacted_keys):
                 for key in self.redacted_keys:
                     if key in to_log:
-                        to_log[key] = "[REDACTED]"
+                        to_log[key] = self.redact_value
 
             try:
                 json_to_log = json.dumps(to_log, cls=DecimalEncoder)
                 if self.newlines:
                     json_to_log += "\n"
                 print(json_to_log)
             except Exception as e:
```

### Comparing `pyno_logger-0.0.7/pyno_logger.egg-info/PKG-INFO` & `pyno_logger-0.0.8/pyno_logger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyno-logger
-Version: 0.0.7
+Version: 0.0.8
 Summary: A JSON logger for Python, inspired by Pino.
 Author-email: Ben Miner <ben@getampt.com>
 Project-URL: Homepage, https://github.com/benminer/pyno-logger
 Project-URL: Bug Tracker, https://github.com/benminer/pyno-logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,20 +36,24 @@
 
 The `Pyno` class takes an optional configuration dictionary as an argument. The configuration options are as follows:
 
 - `level` (optional): Specifies the log level. Valid log levels are "ERROR", "WARNING", "INFO", "DEBUG", "TRACE", "FATAL", and "SILENT". The default log level is "INFO". By default, Pyno uses the `LOG_LEVEL` environment variable if nothing is passed via the `config` dict.
 
 - `base` (optional): Dictionary with any base configuration that is applied to all logs.
 
+- `enabled` (optional): Boolean value that sets the enabled state of the logger.
+
 - `msg_key` (optional): Custom key value for the message value. Defaults to `msg`.
 
 - `error_key` (optional): Custom key value for Exception values. Defaults to `error`.
 
+- `redact_value` (optional): Custom value for any keys that are redacted during a log.
+
 - `omit` (optional): Specifies a list of keys to omit from the logged data. It can be a list, tuple, or comma-separated string.
-- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys.
+- `redact` (optional): Specifies a list of keys to redact from the logged data. It can be a list, tuple, or comma-separated string. Output is printed as `[REDACTED]` for the matching keys. Keys are redacted _after_ omission.
 - `newlines` (optional): Specifies whether to append a newline character to the end of each log message. It should be a boolean value.
 
 The second param, `mixin`, allows for injecting a function that returns additional contextual data. Useful for any global state or dynamic data.
 
 - `mixin` (optional): Specifies a mixin function that returns a dictionary of additional data to include in log messages.
 
 ### Logging Methods
@@ -62,15 +66,15 @@
 - `debug(data={}, message=None)`: Logs a debug message with the provided data and an optional message.
 - `trace(data={}, message=None)`: Logs a trace message with the provided data and an optional message.
 - `error(data={}, message=None)`: Logs an error message with the provided data and an optional message.
 - `fatal(data={}, message=None)`: Logs a fatal error message with the provided data and an optional message.
 
 Each logging method takes two optional arguments: `data` and `message`. The `data` argument can be a dictionary, list, tuple, string, or Exception object containing additional contextual data. The `message` argument is a string that represents the log message. If not provided, the log message will be automatically generated based on the log level and data.
 
-By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omitted_keys` config param, if desired.
+By default, Pyno includes the fields `time`, `pid`, `hostname` and `level`. These can be omitted via the `omit` config param, if desired.
 
 ### Log Levels
 
 Pyno uses the following log levels:
 
 - `FATAL`: 60
 - `ERROR`: 50
```

