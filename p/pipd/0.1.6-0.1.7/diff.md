# Comparing `tmp/pipd-0.1.6.tar.gz` & `tmp/pipd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.1.6.tar", last modified: Wed Jun  7 23:46:06 2023, max compression
+gzip compressed data, was "pipd-0.1.7.tar", last modified: Sun Jul  9 23:05:41 2023, max compression
```

## Comparing `pipd-0.1.6.tar` & `pipd-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.445006 pipd-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 23:46:06.445006 pipd-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-07 23:45:54.000000 pipd-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.433007 pipd-0.1.6/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.441007 pipd-0.1.6/pipd/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/write_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.441007 pipd-0.1.6/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/tests/test_pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.433007 pipd-0.1.6/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 23:46:06.445006 pipd-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-07 23:45:54.000000 pipd-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 23:05:41.288534 pipd-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-09 23:05:31.000000 pipd-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.284534 pipd-0.1.7/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/pipd/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/functions/write_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/pipd/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/pipes/merged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.288534 pipd-0.1.7/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-09 23:05:31.000000 pipd-0.1.7/pipd/tests/test_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:05:41.284534 pipd-0.1.7/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 23:05:41.000000 pipd-0.1.7/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 23:05:41.288534 pipd-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-09 23:05:31.000000 pipd-0.1.7/setup.py
```

### Comparing `pipd-0.1.6/README.md` & `pipd-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/batch.py` & `pipd-0.1.7/pipd/functions/batch.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/filter.py` & `pipd-0.1.7/pipd/functions/filter.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/filter_cached.py` & `pipd-0.1.7/pipd/functions/filter_cached.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/map.py` & `pipd-0.1.7/pipd/functions/map.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/read_csv.py` & `pipd-0.1.7/pipd/functions/read_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/read_files.py` & `pipd-0.1.7/pipd/functions/read_files.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/read_lines.py` & `pipd-0.1.7/pipd/functions/read_lines.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/shuffle.py` & `pipd-0.1.7/pipd/functions/shuffle.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/side.py` & `pipd-0.1.7/pipd/functions/side.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/tqdm.py` & `pipd-0.1.7/pipd/functions/tqdm.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/functions/write_csv.py` & `pipd-0.1.7/pipd/functions/write_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/pipe.py` & `pipd-0.1.7/pipd/pipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
-import random
 import re
 import traceback
-from typing import Any, Callable, Dict, Iterator, Optional, Sequence, Type
+from typing import Any, Callable, Dict, Iterator, Optional, Type
 
 
 def is_iterable(obj):
     try:
         iter(obj)
         return True
     except TypeError:
         return False
 
 
 def log_traceback_and_continue(exception: Exception):
-    message = "Exception in Pipe, logging traceback continuing:\n"
+    message = "Exception in Pipe, logging trace and continuing:\n"
     message += "".join(
         traceback.format_exception(type(exception), exception, exception.__traceback__)
     )
     print(message)
 
 
 def camelcase_to_snakecase(name):
@@ -35,27 +34,14 @@
         for func in funcs:
             arg = func(arg)
         return arg
 
     return composed
 
 
-def merge_rand(
-    *iterators: Iterator[Any], weights: Optional[Sequence[float]] = None
-) -> Iterator[Any]:
-    iterator_list = list(iterators)
-    weights = [1] * len(iterator_list) if weights is None else weights
-    while iterator_list:
-        next_iter: Iterator = random.choices(iterator_list, weights=weights)[0]
-        try:
-            yield next(next_iter)
-        except StopIteration:
-            break
-
-
 class Function:
     def __call__(self, items) -> Iterator:
         raise NotImplementedError
 
 
 class PipeMeta(type):
     def __getattr__(cls, name):
```

### Comparing `pipd-0.1.6/pipd/tests/test_functions.py` & `pipd-0.1.7/pipd/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd/tests/test_pipe.py` & `pipd-0.1.7/pipd/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.6/pipd.egg-info/SOURCES.txt` & `pipd-0.1.7/pipd.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,10 +19,13 @@
 pipd/functions/shuffle.py
 pipd/functions/side.py
 pipd/functions/sleep.py
 pipd/functions/tqdm.py
 pipd/functions/unbatch.py
 pipd/functions/write_csv.py
 pipd/functions/write_lines.py
+pipd/pipes/__init__.py
+pipd/pipes/merged.py
 pipd/tests/__init__.py
 pipd/tests/test_functions.py
-pipd/tests/test_pipe.py
+pipd/tests/test_pipe.py
+pipd/tests/test_pipes.py
```

