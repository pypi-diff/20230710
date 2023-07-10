# Comparing `tmp/fastcopilot-0.4.0.tar.gz` & `tmp/fastcopilot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcopilot-0.4.0.tar", max compression
+gzip compressed data, was "fastcopilot-0.5.0.tar", max compression
```

## Comparing `fastcopilot-0.4.0.tar` & `fastcopilot-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-07-09 22:51:06.722205 fastcopilot-0.4.0/LICENSE
--rw-r--r--   0        0        0      508 2023-07-09 23:12:48.281536 fastcopilot-0.4.0/README.md
--rw-r--r--   0        0        0      477 2023-07-09 23:26:00.906855 fastcopilot-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-09 18:57:06.166013 fastcopilot-0.4.0/src/fastcopilot/__init__.py
--rw-r--r--   0        0        0     5260 2023-07-09 23:24:41.974882 fastcopilot-0.4.0/src/fastcopilot/copilot.py
--rw-r--r--   0        0        0      151 2023-07-06 10:19:17.568905 fastcopilot-0.4.0/src/fastcopilot/exceptions.py
--rw-r--r--   0        0        0      214 2023-07-06 10:34:33.901722 fastcopilot-0.4.0/src/fastcopilot/schemas.py
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 fastcopilot-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-09 22:51:06.722205 fastcopilot-0.5.0/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-09 23:12:48.281536 fastcopilot-0.5.0/README.md
+-rw-r--r--   0        0        0      477 2023-07-10 08:43:36.942403 fastcopilot-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-09 18:57:06.166013 fastcopilot-0.5.0/src/fastcopilot/__init__.py
+-rw-r--r--   0        0        0     5338 2023-07-10 08:43:28.857335 fastcopilot-0.5.0/src/fastcopilot/copilot.py
+-rw-r--r--   0        0        0      151 2023-07-06 10:19:17.568905 fastcopilot-0.5.0/src/fastcopilot/exceptions.py
+-rw-r--r--   0        0        0      214 2023-07-06 10:34:33.901722 fastcopilot-0.5.0/src/fastcopilot/schemas.py
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 fastcopilot-0.5.0/PKG-INFO
```

### Comparing `fastcopilot-0.4.0/LICENSE` & `fastcopilot-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcopilot-0.4.0/src/fastcopilot/copilot.py` & `fastcopilot-0.5.0/src/fastcopilot/copilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import functools
 import json
 
 import openai
 from loguru import logger
 
 from .exceptions import (
     AsyncFunctionNotSupported,
@@ -119,15 +120,15 @@
             }
         )
         response = await asyncio.to_thread(
             openai.ChatCompletion.create,
             **self.params
         )
         resp_msg = response["choices"][0]["message"]
-        if function_call := resp_msg.get("function_call"):
+        while function_call := resp_msg.get("function_call"):
             func_name = function_call["name"]
             arguments = json.loads(function_call["arguments"])
             logger.debug(f"<FunctionCall>name: {func_name}, arguments: {arguments}")
             func_spec = self._func_mapping.get(func_name)
             if asyncio.iscoroutinefunction(func_spec.handler):
                 result = await func_spec.handler(**arguments,
                                                  headers=self.headers)
@@ -145,14 +146,16 @@
                     "content": json.dumps(result, ensure_ascii=False)
                 }
             )
             response = await asyncio.to_thread(
                 openai.ChatCompletion.create,
                 **self.params
             )
+            resp_msg = response["choices"][0]["message"]
+
         self.messages.append(
             {
                 "role": "assistant",
                 "content": response["choices"][0]["message"]["content"]
             }
         )
```

### Comparing `fastcopilot-0.4.0/PKG-INFO` & `fastcopilot-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcopilot
-Version: 0.4.0
+Version: 0.5.0
 Summary: Fast Copilot framework, easy to learn, fast to code, fast to build a copilot for your applications.
 Author: Jackson
 Author-email: jackson.zhang@mrs.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
```

