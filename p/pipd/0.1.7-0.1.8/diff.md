# Comparing `tmp/pipd-0.1.7.tar.gz` & `tmp/pipd-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.1.7.tar", last modified: Sun Jul  9 23:05:41 2023, max compression
+gzip compressed data, was "pipd-0.1.8.tar", last modified: Mon Jul 10 10:01:22 2023, max compression
```

## Comparing `pipd-0.1.7.tar` & `pipd-0.1.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 23:05:41.288534 pipd-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-09 23:05:31.000000 pipd-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.284534 pipd-0.1.7/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/pipd/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/write_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/pipd/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/pipes/merged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/test_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.284534 pipd-0.1.7/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 23:05:41.288534 pipd-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-09 23:05:31.000000 pipd-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:01:22.489855 pipd-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 10:01:22.489855 pipd-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-10 10:01:09.000000 pipd-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:01:22.485855 pipd-0.1.8/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:01:22.489855 pipd-0.1.8/pipd/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/functions/write_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:01:22.489855 pipd-0.1.8/pipd/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/pipes/merged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:01:22.489855 pipd-0.1.8/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-10 10:01:09.000000 pipd-0.1.8/pipd/tests/test_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:01:22.485855 pipd-0.1.8/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 10:01:22.000000 pipd-0.1.8/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-10 10:01:22.000000 pipd-0.1.8/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:01:22.000000 pipd-0.1.8/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 10:01:22.000000 pipd-0.1.8/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:01:22.489855 pipd-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-10 10:01:09.000000 pipd-0.1.8/setup.py
```

### Comparing `pipd-0.1.7/README.md` & `pipd-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/batch.py` & `pipd-0.1.8/pipd/functions/batch.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/filter.py` & `pipd-0.1.8/pipd/functions/filter.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/filter_cached.py` & `pipd-0.1.8/pipd/functions/filter_cached.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/map.py` & `pipd-0.1.8/pipd/functions/map.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/read_csv.py` & `pipd-0.1.8/pipd/functions/read_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/read_files.py` & `pipd-0.1.8/pipd/functions/read_files.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/read_lines.py` & `pipd-0.1.8/pipd/functions/read_lines.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/shuffle.py` & `pipd-0.1.8/pipd/functions/shuffle.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/side.py` & `pipd-0.1.8/pipd/functions/side.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/tqdm.py` & `pipd-0.1.8/pipd/functions/tqdm.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/functions/write_csv.py` & `pipd-0.1.8/pipd/functions/write_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/pipe.py` & `pipd-0.1.8/pipd/pipe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 import traceback
-from typing import Any, Callable, Dict, Iterator, Optional, Type
+from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Type
 
 
 def is_iterable(obj):
     try:
         iter(obj)
         return True
     except TypeError:
@@ -48,50 +48,67 @@
         def method(*args, **kwargs):
             return cls().__getattr__(name)(*args, **kwargs)
 
         return method
 
 
 class Pipe(metaclass=PipeMeta):
-    functions: Dict[str, Type[Function]] = {}
+    _functions: Dict[str, Type[Function]] = {}
 
     def __init__(
         self,
         *iterable,
-        function: Optional[Callable] = identity,
-        handler: Optional[Callable] = log_traceback_and_continue,
+        function: Callable = identity,
+        handler: Callable = log_traceback_and_continue,
     ):
         if len(iterable) == 1 and is_iterable(iterable[0]):
             iterable = iterable[0]
-        self.iterable = iterable
-        self.function = function
-        self.handler = handler
+        self._iterable: Iterable = iterable
+        self._function = function
+        self._handler = handler
 
     def __iter__(self):
-        for item in self.function(iter(self.iterable)):
+        for item in self._function(iter(self._iterable)):
             try:
                 yield item
             except Exception as e:
-                self.handler(e)
+                self._handler(e)
 
-    def close(self):
-        # Necessary to use `yield from` on a Pipe object
-        pass
-
-    def list(self):
-        return list(self)
+    def _new_pipe(
+        self,
+        iterable: Optional[Iterable] = None,
+        function: Optional[Callable] = None,
+        functions: Optional[Dict[str, Type[Function]]] = None,
+        handler: Optional[Callable] = None,
+    ):
+        # This is for composition intead of init so that init can be customized
+        pipe = self.__class__()
+        pipe._iterable = iterable or self._iterable
+        pipe._function = function or self._function
+        pipe._functions = functions or self._functions
+        pipe._handler = handler or self._handler
+        return pipe
 
     def __getattr__(self, name):
         def method(*args, **kwargs):
-            cls = self.__class__
-            function = self.functions[name](*args, **kwargs)
-            return cls(self.iterable, function=compose(self.function, function))
+            return self._new_pipe(
+                function=compose(self._function, self._functions[name](*args, **kwargs))
+            )
 
         return method
 
     def __call__(self, *iterable):
-        return self.__class__(*iterable, function=self.function)
+        if len(iterable) == 1 and is_iterable(iterable[0]):
+            iterable = iterable[0]
+        return self._new_pipe(iterable=iterable)
+
+    def close(self):
+        # Necessary to use `yield from` on a Pipe object
+        pass
+
+    def list(self):
+        return list(self)
 
     @classmethod
     def add_fn(cls, fn: Type[Function], name: Optional[str] = None):
         fn_name = camelcase_to_snakecase(fn.__name__) if name is None else name
-        cls.functions[fn_name] = fn
+        cls._functions[fn_name] = fn
```

### Comparing `pipd-0.1.7/pipd/pipes/merged.py` & `pipd-0.1.8/pipd/pipes/merged.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/tests/test_functions.py` & `pipd-0.1.8/pipd/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/tests/test_pipe.py` & `pipd-0.1.8/pipd/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd/tests/test_pipes.py` & `pipd-0.1.8/pipd/tests/test_pipes.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.7/pipd.egg-info/SOURCES.txt` & `pipd-0.1.8/pipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

