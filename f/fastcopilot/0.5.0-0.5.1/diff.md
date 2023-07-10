# Comparing `tmp/fastcopilot-0.5.0.tar.gz` & `tmp/fastcopilot-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcopilot-0.5.0.tar", max compression
+gzip compressed data, was "fastcopilot-0.5.1.tar", max compression
```

## Comparing `fastcopilot-0.5.0.tar` & `fastcopilot-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-07-09 22:51:06.722205 fastcopilot-0.5.0/LICENSE
--rw-r--r--   0        0        0      508 2023-07-09 23:12:48.281536 fastcopilot-0.5.0/README.md
--rw-r--r--   0        0        0      477 2023-07-10 08:43:36.942403 fastcopilot-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-09 18:57:06.166013 fastcopilot-0.5.0/src/fastcopilot/__init__.py
--rw-r--r--   0        0        0     5338 2023-07-10 08:43:28.857335 fastcopilot-0.5.0/src/fastcopilot/copilot.py
--rw-r--r--   0        0        0      151 2023-07-06 10:19:17.568905 fastcopilot-0.5.0/src/fastcopilot/exceptions.py
--rw-r--r--   0        0        0      214 2023-07-06 10:34:33.901722 fastcopilot-0.5.0/src/fastcopilot/schemas.py
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 fastcopilot-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-09 22:51:06.722205 fastcopilot-0.5.1/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-09 23:12:48.281536 fastcopilot-0.5.1/README.md
+-rw-r--r--   0        0        0      511 2023-07-10 09:06:58.094530 fastcopilot-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-09 18:57:06.166013 fastcopilot-0.5.1/src/fastcopilot/__init__.py
+-rw-r--r--   0        0        0     5537 2023-07-10 09:09:15.038301 fastcopilot-0.5.1/src/fastcopilot/copilot.py
+-rw-r--r--   0        0        0      151 2023-07-06 10:19:17.568905 fastcopilot-0.5.1/src/fastcopilot/exceptions.py
+-rw-r--r--   0        0        0      214 2023-07-06 10:34:33.901722 fastcopilot-0.5.1/src/fastcopilot/schemas.py
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 fastcopilot-0.5.1/PKG-INFO
```

### Comparing `fastcopilot-0.5.0/LICENSE` & `fastcopilot-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcopilot-0.5.0/src/fastcopilot/copilot.py` & `fastcopilot-0.5.1/src/fastcopilot/copilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
                 "role": "system",
                 "content": self.system_prompt
             }]
         self._functions = None  # type: list[dict] | None
         self._func_mapping = {}  # type: dict[str, FuncSpec]
 
     def register_functions(self, *specs: FuncSpec):
+        """
+        Add functions for OpenAI function_call.
+        """
         if not self._functions:
             self._functions = []
         for spec in specs:
             func_name = spec.json_schema.get("name")
             if not func_name:
                 raise InvalidFuncSpecSchema("`name` is required in json_schema")
             if self._func_mapping.get(spec.json_schema["name"]):
@@ -65,14 +68,17 @@
             "timeout": self.timeout
         }
         if self._functions:
             p["functions"] = self._functions
         return p
 
     def run(self, ipt: str) -> tuple[str, dict]:
+        """
+        Get reply from copilot.
+        """
         if not self.messages:
             self.messages = []
 
         self.messages.append(
             {
                 "role": "user",
                 "content": ipt.strip()
@@ -106,14 +112,17 @@
         )
 
         usage = response["usage"]
 
         return response["choices"][0]["message"]["content"], usage
 
     async def arun(self, ipt: str) -> tuple[str, dict]:
+        """
+        Get reply asynchronously from copilot.
+        """
         if not self.messages:
             self.messages = []
 
         self.messages.append(
             {
                 "role": "user",
                 "content": ipt.strip()
```

### Comparing `fastcopilot-0.5.0/PKG-INFO` & `fastcopilot-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fastcopilot
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fast Copilot framework, easy to learn, fast to code, fast to build a copilot for your applications.
 Author: Jackson
-Author-email: jackson.zhang@mrs.ai
+Author-email: jackson.zhang0429@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Description-Content-Type: text/markdown
```

