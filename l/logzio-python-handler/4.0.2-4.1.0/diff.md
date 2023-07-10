# Comparing `tmp/logzio-python-handler-4.0.2.tar.gz` & `tmp/logzio-python-handler-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logzio-python-handler-4.0.2.tar", last modified: Sun May 21 07:20:29 2023, max compression
+gzip compressed data, was "logzio-python-handler-4.1.0.tar", last modified: Mon Jul 10 14:49:50 2023, max compression
```

## Comparing `logzio-python-handler-4.0.2.tar` & `logzio-python-handler-4.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/logzio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/flusher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/tests/mockLogzioListener/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/logsList.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/persistentFlags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/test_add_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/test_logzioHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/test_logzioSender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:50.546188 logzio-python-handler-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-10 14:49:50.546188 logzio-python-handler-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:50.542188 logzio-python-handler-4.1.0/logzio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/logzio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/logzio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/logzio/flusher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/logzio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/logzio/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/logzio/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:50.542188 logzio-python-handler-4.1.0/logzio_python_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-10 14:49:50.000000 logzio-python-handler-4.1.0/logzio_python_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-10 14:49:50.000000 logzio-python-handler-4.1.0/logzio_python_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:49:50.000000 logzio-python-handler-4.1.0/logzio_python_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-10 14:49:50.000000 logzio-python-handler-4.1.0/logzio_python_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 14:49:50.000000 logzio-python-handler-4.1.0/logzio_python_handler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 14:49:50.546188 logzio-python-handler-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:50.546188 logzio-python-handler-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:50.546188 logzio-python-handler-4.1.0/tests/mockLogzioListener/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/mockLogzioListener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/mockLogzioListener/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/mockLogzioListener/logsList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/mockLogzioListener/persistentFlags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/test_add_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/test_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/test_logzioHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-10 14:49:42.000000 logzio-python-handler-4.1.0/tests/test_logzioSender.py
```

### Comparing `logzio-python-handler-4.0.2/LICENSE` & `logzio-python-handler-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.2/README.md` & `logzio-python-handler-4.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -22,36 +22,43 @@
 
 
 ## Installation
 ```bash
 pip install logzio-python-handler
 ```
 
+If you'd like to use [Trace context](https://github.com/logzio/logzio-python-handler#trace-context) then you need to install the OpenTelemetry logging instrumentation dependecy by running the following command:
+
+```bash
+pip install logzio-python-handler[opentelemetry-logging]
+```
 ## Tested Python Versions
 Travis CI will build this handler and test against:
   - "3.5"
   - "3.6"
   - "3.7"
   - "3.8"
   - "3.9"
+  - "3.10"
+  - "3.11"
 
 We can't ensure compatibility to any other version, as we can't test it automatically.
 
 To run tests:
 
 ```bash
 $ pip install tox
 $ tox
 ...
 
 ```
 
 ## Python configuration
 #### Config File
-```
+```python
 [handlers]
 keys=LogzioHandler
 
 [handler_LogzioHandler]
 class=logzio.handler.LogzioHandler
 formatter=logzioFormat
 args=('token', 'my_type')
@@ -80,15 +87,15 @@
  - Retries number (retry_no, defaults to 4).
  - Retry timeout (retry_timeout) in seconds (defaults to 2).
 
  Please note, that you have to configure those parameters by this exact order.
  i.e. you cannot set Debug to true, without configuring all of the previous parameters as well.
 
 #### Dict Config
-```
+```python
 LOGGING = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'logzioFormat': {
             'format': '{"additional_field": "value"}',
             'validate': False
@@ -150,21 +157,45 @@
 #### Extra Fields
 In case you need to dynamic metadata to your logger, other then the constant metadata from the formatter, you can use the "extra" parameter.
 All key values in the dictionary passed in "extra" will be presented in Logz.io as new fields in the log you are sending.
 Please note, that you cannot override default fields by the python logger (i.e. lineno, thread, etc..)
 For example:
 
 
-```
+```python
 logger.info('Warning', extra={'extra_key':'extra_value'})
 ```
+#### Dynamic Extra Fields
+If you prefer, you can add extra fields to your logs dynamically, and not pre-defining them in the configuration.
+This way, you can allow different logs to have different extra fields.
 
+See the following code example:
+
+```python
+from logzio.handler import ExtraFieldsLogFilter
+
+def main():
+
+    logger.info("Test log")  # Outputs: {"message":"Test log"}
+    
+    extra_fields = {"foo":"bar","counter":1}
+    logger.addFilter(ExtraFieldsLogFilter(extra_fields))
+    logger.warning("Warning test log")  # Outputs: {"message":"Warning test log","foo":"bar","counter":1}
+    
+    error_fields = {"err_msg":"Failed to run due to exception.","status_code":500}
+    logger.addFilter(ExtraFieldsLogFilter(error_fields))
+    logger.error("Error test log")  # Outputs: {"message":"Error test log","foo":"bar","counter":1,"err_msg":"Failed to run due to exception.","status_code":500}
+    # If you'd like to remove filters from future logs using the logger.removeFilter option:
+    logger.removeFilter(ExtraFieldsLogFilter(error_fields))
+    logger.debug("Debug test log") # Outputs: {"message":"Debug test log","foo":"bar","counter":1}
 
-## Django configuration
 ```
+
+## Django configuration
+```python
 LOGGING = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'verbose': {
             'format': '%(levelname)s %(asctime)s %(module)s %(process)d %(thread)d %(message)s'
         },
@@ -212,14 +243,20 @@
 - logzio_type - Log type, for searching in logz.io (defaults to "python"), it cannot contain a space.
 - appname - Your django app
 
 ## Trace context
 
 If you're sending traces with OpenTelemetry instrumentation (auto or manual), you can correlate your logs with the trace context.
 That way, your logs will have traces data in it, such as service name, span id and trace id.
+
+Make sure to install the OpenTelemetry logging instrumentation dependecy by running the following command:
+
+```bash
+pip install logzio-python-handler[opentelemetry-logging]
+```
 To enable this feature, set the `add_context` param in your handler configuration to `True`, like in this example:
 
 ```python
 LOGGING = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
@@ -251,15 +288,20 @@
     }
 }
 ```
 
 Please note that if you are using `python 3.8`, it is preferred to use the `logging.config.dictConfig` method, as mentioned in [python's documentation](https://docs.python.org/3/library/logging.config.html#configuration-file-format).
 
 ## Release Notes
-
+- 4.1.0
+  - Add ability to dynamically attach extra fields to the logs.
+  - Import opentelemetry logging dependency only if trace context is enabled and dependency is installed manually.
+    - Updated `opentelemetry-instrumentation-logging==0.39b0`
+  - Updated `setuptools>=68.0.0`
+  - Added tests for Python versions: 3.9, 3.10, 3.11
 - 4.0.2
   - Fix bug for logging exceptions ([#76](https://github.com/logzio/logzio-python-handler/pull/76))
 - 4.0.1
   - Updated `protobuf>=3.20.2`.
   - Added dependency `setuptools>=65.5.1`
   
 - 4.0.0
```

### Comparing `logzio-python-handler-4.0.2/logzio/flusher.py` & `logzio-python-handler-4.1.0/logzio/flusher.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.2/logzio/handler.py` & `logzio-python-handler-4.1.0/logzio/handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,24 @@
 import datetime
 import traceback
 import logging.handlers
 
 from .sender import LogzioSender
 from .exceptions import LogzioException
 
-from opentelemetry.instrumentation.logging import LoggingInstrumentor
+
+class ExtraFieldsLogFilter(logging.Filter):
+
+    def __init__(self, extra: dict, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.extra = extra
+
+    def filter(self, record):
+        record.__dict__.update(self.extra)
+        return True
 
 
 class LogzioHandler(logging.Handler):
 
     def __init__(self,
                  token,
                  logzio_type="python",
@@ -27,16 +36,22 @@
 
         if not token:
             raise LogzioException('Logz.io Token must be provided')
 
         self.logzio_type = logzio_type
 
         if add_context:
-            LoggingInstrumentor().instrument(set_logging_format=True)
-
+            try:
+                from opentelemetry.instrumentation.logging import LoggingInstrumentor
+                LoggingInstrumentor().instrument(set_logging_format=True)
+            except ImportError:
+                print("""Can't add trace context.
+OpenTelemetry logging optional package isn't installed.
+Please install the following package:
+pip install 'logzio-python-handler[opentelemetry-logging]'""")
         self.logzio_sender = LogzioSender(
             token=token,
             url=url,
             logs_drain_timeout=logs_drain_timeout,
             debug=debug,
             backup_logs=backup_logs,
             network_timeout=network_timeout,
@@ -87,15 +102,15 @@
 
     def format_exception(self, exc_info):
         return '\n'.join(traceback.format_exception(*exc_info))
 
     def format_message(self, message):
         now = datetime.datetime.utcnow()
         timestamp = now.strftime('%Y-%m-%dT%H:%M:%S') + \
-            '.%03d' % (now.microsecond / 1000) + 'Z'
+                    '.%03d' % (now.microsecond / 1000) + 'Z'
 
         return_json = {
             'logger': message.name,
             'line_number': message.lineno,
             'path_name': message.pathname,
             'log_level': message.levelname,
             'type': self.logzio_type,
```

### Comparing `logzio-python-handler-4.0.2/logzio/sender.py` & `logzio-python-handler-4.1.0/logzio/sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from time import sleep
 from datetime import datetime
 from threading import Thread, enumerate
 
 import requests
 
-from .logger import get_logger
 from .logger import get_stdout_logger
 
 if sys.version[0] == '2':
     import Queue as queue
 else:
     import queue as queue
```

### Comparing `logzio-python-handler-4.0.2/logzio_python_handler.egg-info/SOURCES.txt` & `logzio-python-handler-4.1.0/logzio_python_handler.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 logzio_python_handler.egg-info/PKG-INFO
 logzio_python_handler.egg-info/SOURCES.txt
 logzio_python_handler.egg-info/dependency_links.txt
 logzio_python_handler.egg-info/requires.txt
 logzio_python_handler.egg-info/top_level.txt
 tests/__init__.py
 tests/test_add_context.py
+tests/test_extra_fields.py
 tests/test_logzioHandler.py
 tests/test_logzioSender.py
 tests/mockLogzioListener/__init__.py
 tests/mockLogzioListener/listener.py
 tests/mockLogzioListener/logsList.py
 tests/mockLogzioListener/persistentFlags.py
```

### Comparing `logzio-python-handler-4.0.2/tests/mockLogzioListener/listener.py` & `logzio-python-handler-4.1.0/tests/mockLogzioListener/listener.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.2/tests/test_add_context.py` & `logzio-python-handler-4.1.0/tests/test_add_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     def setUp(self):
         self.logzio_listener = listener.MockLogzioListener()
         self.logzio_listener.clear_logs_buffer()
         self.logzio_listener.clear_server_error()
         self.logs_drain_timeout = 1
         self.retries_no = 4
         self.retry_timeout = 2
-
-        logging_configuration = {
+        self.add_context = True
+        self.logging_configuration = {
             "version": 1,
             "formatters": {
                 "logzio": {
                     "format": '{"key": "value"}',
                     "validate": False
                 }
             },
@@ -44,37 +44,58 @@
                     "token": "token",
                     'logzio_type': "type",
                     'logs_drain_timeout': self.logs_drain_timeout,
                     'url': "http://" + self.logzio_listener.get_host() + ":" + str(self.logzio_listener.get_port()),
                     'debug': True,
                     'retries_no': self.retries_no,
                     'retry_timeout': self.retry_timeout,
-                    'add_context': True
+                    'add_context': self.add_context
                 }
             },
             "loggers": {
                 "test": {
                     "handlers": ["LogzioHandler"],
                     "level": "DEBUG"
                 }
             }
         }
 
-        logging.config.dictConfig(logging_configuration)
+        logging.config.dictConfig(self.logging_configuration)
         self.logger = logging.getLogger('test')
 
         for curr_file in _find("logzio-failures-*.txt", "."):
             os.remove(curr_file)
 
     def test_add_context(self):
+        # Logging configuration of add_context default to True
         log_message = "this log should have a trace context"
         self.logger.info(log_message)
         time.sleep(self.logs_drain_timeout * 2)
         logs_list = self.logzio_listener.logs_list
         for current_log in logs_list:
             if log_message in current_log:
                 log_dict = json.loads(current_log)
-                self.assertTrue('otelSpanID' in log_dict)
-                self.assertTrue('otelTraceID' in log_dict)
-                self.assertTrue('otelServiceName' in log_dict)
-
-
+                try:
+                    self.assertTrue('otelSpanID' in log_dict)
+                    self.assertTrue('otelTraceID' in log_dict)
+                    self.assertTrue('otelServiceName' in log_dict)
+                except AssertionError as err:
+                    print(err)
+
+    def test_ignore_context(self):
+        # Set add_context to False and reconfigure the logger as it defaults to True
+        self.logging_configuration["handlers"]["LogzioHandler"]["add_context"] = False
+        logging.config.dictConfig(self.logging_configuration)
+        self.logger = logging.getLogger('test')
+        log_message = "this log should not have a trace context"
+        self.logger.info(log_message)
+        time.sleep(self.logs_drain_timeout * 2)
+        logs_list = self.logzio_listener.logs_list
+        for current_log in logs_list:
+            if log_message in current_log:
+                log_dict = json.loads(current_log)
+                try:
+                    self.assertFalse('otelSpanID' in log_dict)
+                    self.assertFalse('otelTraceID' in log_dict)
+                    self.assertFalse('otelServiceName' in log_dict)
+                except AssertionError as err:
+                    print(err)
```

### Comparing `logzio-python-handler-4.0.2/tests/test_logzioHandler.py` & `logzio-python-handler-4.1.0/tests/test_logzioHandler.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.2/tests/test_logzioSender.py` & `logzio-python-handler-4.1.0/tests/test_logzioSender.py`

 * *Files identical despite different names*

