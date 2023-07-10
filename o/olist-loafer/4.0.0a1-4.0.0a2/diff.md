# Comparing `tmp/olist_loafer-4.0.0a1.tar.gz` & `tmp/olist_loafer-4.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olist_loafer-4.0.0a1.tar", max compression
+gzip compressed data, was "olist_loafer-4.0.0a2.tar", max compression
```

## Comparing `olist_loafer-4.0.0a1.tar` & `olist_loafer-4.0.0a2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1083 2022-11-08 20:03:57.885056 olist_loafer-4.0.0a1/LICENSE
--rw-r--r--   0        0        0     1676 2022-11-08 20:03:57.885056 olist_loafer-4.0.0a1/README.md
--rw-r--r--   0        0        0        0 2022-11-08 20:03:57.895056 olist_loafer-4.0.0a1/loafer/__init__.py
--rw-r--r--   0        0        0     2362 2023-05-12 15:01:11.963967 olist_loafer-4.0.0a1/loafer/dispatchers.py
--rw-r--r--   0        0        0      237 2022-11-08 20:03:57.895056 olist_loafer-4.0.0a1/loafer/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-08 20:03:57.895056 olist_loafer-4.0.0a1/loafer/ext/__init__.py
--rw-r--r--   0        0        0        0 2022-11-08 20:03:57.905057 olist_loafer-4.0.0a1/loafer/ext/aws/__init__.py
--rw-r--r--   0        0        0     1920 2023-04-29 19:25:57.593482 olist_loafer-4.0.0a1/loafer/ext/aws/bases.py
--rw-r--r--   0        0        0     1896 2023-01-11 19:30:20.652969 olist_loafer-4.0.0a1/loafer/ext/aws/handlers.py
--rw-r--r--   0        0        0     1752 2023-03-25 12:20:00.904444 olist_loafer-4.0.0a1/loafer/ext/aws/message_translators.py
--rw-r--r--   0        0        0     3356 2023-04-29 19:25:57.593482 olist_loafer-4.0.0a1/loafer/ext/aws/providers.py
--rw-r--r--   0        0        0     1130 2022-11-08 20:03:57.905057 olist_loafer-4.0.0a1/loafer/ext/aws/routes.py
--rw-r--r--   0        0        0      329 2022-11-08 20:03:57.905057 olist_loafer-4.0.0a1/loafer/ext/sentry.py
--rw-r--r--   0        0        0     2053 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/managers.py
--rw-r--r--   0        0        0      735 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/message_translators.py
--rw-r--r--   0        0        0      890 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/providers.py
--rw-r--r--   0        0        0     2938 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/routes.py
--rw-r--r--   0        0        0     2481 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/runners.py
--rw-r--r--   0        0        0      569 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/utils.py
--rw-r--r--   0        0        0     1727 2023-05-12 15:10:37.873968 olist_loafer-4.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 olist_loafer-4.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/LICENSE
+-rw-r--r--   0        0        0     1676 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/__init__.py
+-rw-r--r--   0        0        0      523 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/compat.py
+-rw-r--r--   0        0        0     2362 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/dispatchers.py
+-rw-r--r--   0        0        0      237 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/aws/__init__.py
+-rw-r--r--   0        0        0     1920 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/aws/bases.py
+-rw-r--r--   0        0        0     1896 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/aws/handlers.py
+-rw-r--r--   0        0        0     1752 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/aws/message_translators.py
+-rw-r--r--   0        0        0     3356 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/aws/providers.py
+-rw-r--r--   0        0        0     1130 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/aws/routes.py
+-rw-r--r--   0        0        0      329 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/ext/sentry.py
+-rw-r--r--   0        0        0     2053 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/managers.py
+-rw-r--r--   0        0        0      735 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/message_translators.py
+-rw-r--r--   0        0        0      890 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/providers.py
+-rw-r--r--   0        0        0     2941 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/routes.py
+-rw-r--r--   0        0        0     2481 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/runners.py
+-rw-r--r--   0        0        0      546 2023-07-02 16:07:53.394738 olist_loafer-4.0.0a2/loafer/utils.py
+-rw-r--r--   0        0        0     1727 2023-07-08 18:24:25.553063 olist_loafer-4.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 olist_loafer-4.0.0a2/PKG-INFO
```

### Comparing `olist_loafer-4.0.0a1/LICENSE` & `olist_loafer-4.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/README.md` & `olist_loafer-4.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/dispatchers.py` & `olist_loafer-4.0.0a2/loafer/dispatchers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/ext/aws/bases.py` & `olist_loafer-4.0.0a2/loafer/ext/aws/bases.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/ext/aws/handlers.py` & `olist_loafer-4.0.0a2/loafer/ext/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/ext/aws/message_translators.py` & `olist_loafer-4.0.0a2/loafer/ext/aws/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/ext/aws/providers.py` & `olist_loafer-4.0.0a2/loafer/ext/aws/providers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/ext/aws/routes.py` & `olist_loafer-4.0.0a2/loafer/ext/aws/routes.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/managers.py` & `olist_loafer-4.0.0a2/loafer/managers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/message_translators.py` & `olist_loafer-4.0.0a2/loafer/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/providers.py` & `olist_loafer-4.0.0a2/loafer/providers.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/routes.py` & `olist_loafer-4.0.0a2/loafer/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from .message_translators import AbstractMessageTranslator
 from .providers import AbstractProvider
-from .utils import run_in_loop_or_executor
+from .utils import ensure_coroutinefunction
 
 logger = logging.getLogger(__name__)
 
 
 class Route:
     def __init__(self, provider, handler, name="default", message_translator=None, error_handler=None):
         self.name = name
@@ -57,21 +57,21 @@
             raise ValueError(f"{self.message_translator} failed to translate message={message}")
 
         return processed_message
 
     async def deliver(self, raw_message):
         message = self.apply_message_translator(raw_message)
         logger.info(f"delivering message route={self}, message={message!r}")
-        return await run_in_loop_or_executor(self.handler, message["content"], message["metadata"])
+        return await ensure_coroutinefunction(self.handler, message["content"], message["metadata"])
 
     async def error_handler(self, exc_info, message):
         logger.info(f"error handler process originated by message={message}")
 
         if self._error_handler is not None:
-            return await run_in_loop_or_executor(self._error_handler, exc_info, message)
+            return await ensure_coroutinefunction(self._error_handler, exc_info, message)
 
         return False
 
     def stop(self):
         logger.info(f"stopping route {self}")
         self.provider.stop()
         # only for class-based handlers
```

### Comparing `olist_loafer-4.0.0a1/loafer/runners.py` & `olist_loafer-4.0.0a2/loafer/runners.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-4.0.0a1/loafer/utils.py` & `olist_loafer-4.0.0a2/loafer/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import asyncio
 import logging
 
+from .compat import iscoroutinefunction, to_thread
+
 logger = logging.getLogger(__name__)
 
 
-async def run_in_loop_or_executor(func, *args):
-    if asyncio.iscoroutinefunction(func):
+async def ensure_coroutinefunction(func, *args):
+    if iscoroutinefunction(func):
         logger.debug(f"handler is coroutine! {func!r}")
         return await func(*args)
 
-    loop = asyncio.get_event_loop()
     logger.debug(f"handler will run in a separate thread: {func!r}")
-    return await loop.run_in_executor(None, func, *args)
+    return await to_thread(func, *args)
 
 
 def calculate_backoff_multiplier(number_of_tries, backoff_factor):
     exponential_factor = backoff_factor**number_of_tries
 
     return exponential_factor
```

### Comparing `olist_loafer-4.0.0a1/pyproject.toml` & `olist_loafer-4.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-vv --cov=loafer --cov-report=term-missing"
 asyncio_mode = "strict"
 
 [tool.poetry]
 name = "olist-loafer"
-version = "4.0.0a1"
+version = "4.0.0a2"
 description = "Asynchronous message dispatcher for concurrent tasks processing"
 license = "MIT"
 authors = ["Olist <developers@olist.com>"]
 readme = "README.md"
 repository = "https://github.com/olist/olist-loafer/"
 keywords = ["asyncio", "message", "dispatcher", "tasks", "microservices"]
 classifiers = [
```

### Comparing `olist_loafer-4.0.0a1/PKG-INFO` & `olist_loafer-4.0.0a2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olist-loafer
-Version: 4.0.0a1
+Version: 4.0.0a2
 Summary: Asynchronous message dispatcher for concurrent tasks processing
 Home-page: https://github.com/olist/olist-loafer/
 License: MIT
 Keywords: asyncio,message,dispatcher,tasks,microservices
 Author: Olist
 Author-email: developers@olist.com
 Requires-Python: >=3.8,<3.12
@@ -16,18 +16,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: aiobotocore[boto3] (>=1.0.0,<3.0.0)
 Project-URL: Download, https://github.com/olist/olist-loafer/releases
 Project-URL: Repository, https://github.com/olist/olist-loafer/
 Description-Content-Type: text/markdown
 
 [![PyPI latest](https://img.shields.io/pypi/v/olist-loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/loafer)
```

