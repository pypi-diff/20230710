# Comparing `tmp/pipd-0.1.9.tar.gz` & `tmp/pipd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.1.9.tar", last modified: Mon Jul 10 12:47:54 2023, max compression
+gzip compressed data, was "pipd-0.2.0.tar", last modified: Mon Jul 10 16:53:56 2023, max compression
```

## Comparing `pipd-0.1.9.tar` & `pipd-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:47:54.729595 pipd-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 12:47:54.729595 pipd-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-10 12:47:44.000000 pipd-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:47:54.725595 pipd-0.1.9/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:47:54.725595 pipd-0.1.9/pipd/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/functions/write_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:47:54.725595 pipd-0.1.9/pipd/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/pipes/merged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:47:54.729595 pipd-0.1.9/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-10 12:47:44.000000 pipd-0.1.9/pipd/tests/test_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 12:47:54.725595 pipd-0.1.9/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 12:47:54.000000 pipd-0.1.9/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-10 12:47:54.000000 pipd-0.1.9/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 12:47:54.000000 pipd-0.1.9/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 12:47:54.000000 pipd-0.1.9/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 12:47:54.729595 pipd-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-10 12:47:44.000000 pipd-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.772686 pipd-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 16:53:56.772686 pipd-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-10 16:53:46.000000 pipd-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.768686 pipd-0.2.0/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.772686 pipd-0.2.0/pipd/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/merged.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/pipes/write_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.772686 pipd-0.2.0/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 16:53:46.000000 pipd-0.2.0/pipd/tests/test_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:53:56.768686 pipd-0.2.0/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 16:53:56.000000 pipd-0.2.0/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:53:56.772686 pipd-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-10 16:53:46.000000 pipd-0.2.0/setup.py
```

### Comparing `pipd-0.1.9/README.md` & `pipd-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pipd-0.1.9/pipd/functions/batch.py` & `pipd-0.2.0/pipd/pipes/batch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable, Iterator, List, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
 T = TypeVar("T")
 
 
-class Batch(Function):
+class Batch(Pipe):
     def __init__(self, size: int, partial: bool = True) -> None:
         self.size = size
         self.partial = partial
 
     def __call__(self, items: Iterable[T]) -> Iterator[List[T]]:
         batch = []
         for item in items:
@@ -17,8 +17,8 @@
             if len(batch) == self.size:
                 yield batch
                 batch = []
         if batch and self.partial:
             yield batch
 
 
-Pipe.add_fn(Batch)
+Pipe.register(Batch)
```

### Comparing `pipd-0.1.9/pipd/functions/filter.py` & `pipd-0.2.0/pipd/pipes/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Callable, Iterable, Iterator, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
 from .map import Map
 
 T = TypeVar("T")
 
 
-class Filter(Function):
+class Filter(Pipe):
     def __init__(self, fn: Callable[[T], bool], *args, **kwargs) -> None:
         self.fn = lambda x: (x, fn(x))
         self.args = args
         self.kwargs = kwargs
 
     def __call__(self, items: Iterable[T]) -> Iterator[T]:
         for item, keep in Map(self.fn, *self.args, **self.kwargs)(items):  # type: ignore
             if keep:  # type: ignore
                 yield item  # type: ignore
 
 
-Pipe.add_fn(Filter)
+Pipe.register(Filter)
```

### Comparing `pipd-0.1.9/pipd/functions/filter_cached.py` & `pipd-0.2.0/pipd/pipes/filter_cached.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from typing import Callable, Iterable, Iterator, Optional, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
 from .read_lines import read_lines
 
 T = TypeVar("T")
 
 
-class FilterCached(Function):
+class FilterCached(Pipe):
     def __init__(self, filepath: str, key: Optional[Callable] = None) -> None:
         self.filepath = filepath
         self.key = key
 
     def __call__(self, items: Iterable[T]) -> Iterator[T]:
         cache = (
             set(read_lines(self.filepath)) if os.path.exists(self.filepath) else set()
@@ -22,8 +22,8 @@
                 value = str(self.key(item) if self.key is not None else item)
                 if value not in cache:
                     cache.add(value)
                     file.write(value + "\n")
                     yield item
 
 
-Pipe.add_fn(FilterCached)
+Pipe.register(FilterCached)
```

### Comparing `pipd-0.1.9/pipd/functions/map.py` & `pipd-0.2.0/pipd/pipes/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,30 @@
     FIRST_COMPLETED,
     ProcessPoolExecutor,
     ThreadPoolExecutor,
     wait,
 )
 from typing import Callable, Iterable, Iterator, Optional, TypeVar
 
-from pipd import Function, Pipe, log_traceback_and_continue
+from pipd import Pipe, log_traceback_and_continue
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-class Map(Function):
+class Map(Pipe):
     def __init__(
         self,
         fn: Callable[[T], U],
         num_workers: int = 0,
         buffer: Optional[int] = None,
         mode: str = "multithread",
         handler: Callable = log_traceback_and_continue,
     ) -> None:
+
         assert mode in ["multithread", "multiprocess"]
         self.fn = fn
         self.num_workers = num_workers
         self.buffer = buffer
         self.mode = mode
         self.handler = handler
 
@@ -56,8 +57,8 @@
             for future in futures:
                 try:
                     yield future.result()
                 except Exception as e:
                     self.handler(e)
 
 
-Pipe.add_fn(Map)
+Pipe.register(Map)
```

### Comparing `pipd-0.1.9/pipd/functions/read_csv.py` & `pipd-0.2.0/pipd/pipes/tqdm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from typing import Dict, Iterable, Iterator, List, Sequence, Union
+from typing import Iterable, Iterator, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
+T = TypeVar("T")
 
-class ReadCSV(Function):
-    def __init__(self, header: Union[bool, Sequence[str]] = False) -> None:
-        self.header = header
 
-    def __call__(self, items: Iterator[str]) -> Iterable[Union[Dict[str, str], List[str]]]:  # type: ignore # noqa
-        import csv
+class Tqdm(Pipe):
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs
 
-        for filepath in items:
-            with open(filepath, "r") as f:
-                if self.header:
-                    fieldnames = (
-                        self.header if isinstance(self.header, Sequence) else None
-                    )
-                    yield from csv.DictReader(f, fieldnames=fieldnames)
-                else:
-                    yield from csv.reader(f)
+    def __call__(self, items: Iterable[T]) -> Iterator[T]:
+        try:
+            from tqdm import tqdm as progressbar
+        except ImportError:
+            raise ImportError("tqdm is required to use tqdm")
 
+        for item in progressbar(items, *self.args, **self.kwargs):
+            yield item
 
-Pipe.add_fn(ReadCSV)
+
+Pipe.register(Tqdm)
```

### Comparing `pipd-0.1.9/pipd/functions/read_files.py` & `pipd-0.2.0/pipd/pipes/read_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import glob
 import os
 import random
 from typing import Iterable, Iterator, Optional, Sequence, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
 from .read_lines import read_lines
 from .write_lines import write_lines
 
 T = TypeVar("T")
 U = TypeVar("U")
 
@@ -24,15 +24,15 @@
     async_generator = awatch(path)
     while True:
         for change, filepath in loop.run_until_complete(async_generator.__anext__()):
             if change in changes:
                 yield filepath
 
 
-class ReadFiles(Function):
+class ReadFiles(Pipe):
     def __init__(
         self,
         cache_filepath: Optional[str] = None,
         watch: bool = False,
         shuffle: bool = False,
     ) -> None:
         self.cache_filepath = cache_filepath
@@ -56,8 +56,8 @@
 
             for file in files:
                 yield file
             if self.watch:
                 yield from watchdir(os.path.dirname(filepath))
 
 
-Pipe.add_fn(ReadFiles)
+Pipe.register(ReadFiles)
```

### Comparing `pipd-0.1.9/pipd/functions/read_lines.py` & `pipd-0.2.0/pipd/pipes/read_lines.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import select
 from typing import Iterable, Iterator
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
 
 def read_lines(filepath: str, watch: bool = False) -> Iterator[str]:
     with open(filepath, "r") as file:
         if watch:
             while True:
                 line = file.readline()
@@ -16,17 +16,17 @@
                         [file], [], []
                     )  # Wait until there is more data to read
         else:
             for line in file:
                 yield line.strip()
 
 
-class ReadLines(Function):
+class ReadLines(Pipe):
     def __init__(self, watch: bool = False) -> None:
         self.watch = watch
 
     def __call__(self, items: Iterable[str]) -> Iterator[str]:
         for filepath in items:
             yield from read_lines(filepath=filepath, watch=self.watch)
 
 
-Pipe.add_fn(ReadLines)
+Pipe.register(ReadLines)
```

### Comparing `pipd-0.1.9/pipd/functions/shuffle.py` & `pipd-0.2.0/pipd/pipes/shuffle.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from random import randint
 from typing import Iterator, List, Optional, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
 T = TypeVar("T")
 
 
 def pick(items: List[T], random: bool = False) -> T:
     idx = randint(0, len(items) - 1) if random else 0
     return items.pop(idx)
 
 
-class Shuffle(Function):
+class Shuffle(Pipe):
     def __init__(self, size: int, start: Optional[int] = None):
         self.size = size
         self.start = start or size
 
-    def __call__(self, items: Iterator[T]) -> Iterator[T]:
+    def __call__(self, items: Iterator[T]) -> Iterator[T]:  # type: ignore
         buffer = []
         for item in items:
             buffer.append(item)
             if len(buffer) < self.size:
                 try:
                     buffer.append(next(items))
                 except StopIteration:
@@ -28,8 +28,8 @@
             if len(buffer) >= self.start:
                 yield pick(buffer, random=True)
         # Empty buffer at the end
         while len(buffer) > 0:
             yield pick(buffer)
 
 
-Pipe.add_fn(Shuffle)
+Pipe.register(Shuffle)
```

### Comparing `pipd-0.1.9/pipd/functions/side.py` & `pipd-0.2.0/pipd/pipes/side.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from typing import Callable, Iterable, Iterator, TypeVar
 
-from pipd import Function, Pipe, log_traceback_and_continue
+from pipd import Pipe, log_traceback_and_continue
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-class Side(Function):
+class Side(Pipe):
     def __init__(
         self,
         fn: Callable[[T], U],
         num_workers: int = 0,
         mode: str = "multithread",
         handler: Callable = log_traceback_and_continue,
     ) -> None:
@@ -36,8 +36,8 @@
         )
         with executors[self.mode](max_workers=self.num_workers) as executor:
             for item in items:
                 executor.submit(self.fn, item)
                 yield item
 
 
-Pipe.add_fn(Side)
+Pipe.register(Side)
```

### Comparing `pipd-0.1.9/pipd/functions/write_csv.py` & `pipd-0.2.0/pipd/pipes/write_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, Iterable, Iterator, Sequence, Union
 
-from pipd import Function, Pipe
+from pipd import Pipe
 
 
-class WriteCSV(Function):
+class WriteCSV(Pipe):
     def __init__(self, filepath: str) -> None:
         self.filepath = filepath
 
     def __call__(
         self, items: Iterable[Union[Dict[str, Any], Sequence[Any]]]
     ) -> Iterator[Union[Dict[str, Any], Sequence[Any]]]:
         import csv
@@ -19,8 +19,8 @@
                     if i == 0:  # Write headers only for the first dictionary item
                         writer.writerow(item.keys())
                     item = item.values()  # type: ignore
                 writer.writerow(item)
                 yield item
 
 
-Pipe.add_fn(WriteCSV)
+Pipe.register(WriteCSV)
```

### Comparing `pipd-0.1.9/pipd/pipe.py` & `pipd-0.2.0/pipd/pipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import re
 import traceback
-from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Type
+from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Type, TypeVar
+
+T = TypeVar("T")
 
 
 def is_iterable(obj):
     try:
         iter(obj)
         return True
     except TypeError:
@@ -25,92 +27,71 @@
     return re.sub(r"([a-z])([A-Z])", r"\1_\2", name).lower()
 
 
 def identity(x: Any) -> Any:
     return x
 
 
-def compose(*funcs: Callable[[Any], Any]) -> Callable[[Any], Any]:
-    def composed(arg: Any) -> Any:
-        for func in funcs:
-            arg = func(arg)
-        return arg
+def compose(source: Callable, target: Callable):
+    def composed(*args):
+        return target(source(*args))
 
     return composed
 
 
-class Function:
-    def __call__(self, items) -> Iterator:
-        raise NotImplementedError
+def unpack_iterable(*iterable: Any) -> Iterable[T]:
+    if len(iterable) == 1 and is_iterable(iterable[0]):
+        iterable = iterable[0]
+    return iterable
 
 
 class PipeMeta(type):
     def __getattr__(cls, name):
         def method(*args, **kwargs):
             return cls().__getattr__(name)(*args, **kwargs)
 
         return method
 
 
 class Pipe(metaclass=PipeMeta):
-    _functions: Dict[str, Type[Function]] = {}
+    _pipes: Dict[str, Type[Pipe]] = {}
 
     def __init__(self, *iterable, handler: Callable = log_traceback_and_continue):
-        self._update(*iterable, handler=handler)
-
-    def _update(
-        self,
-        *iterable,
-        function: Optional[Callable] = None,
-        handler: Optional[Callable] = None,
-    ):
-        if len(iterable) == 1 and is_iterable(iterable[0]):
-            iterable = iterable[0]
-        self._iterable: Iterable = iterable
-        self._function = function or identity
+        self._iterable: Iterable = unpack_iterable(*iterable)
+        self._function = identity
         self._handler = handler or log_traceback_and_continue
-        return self
+
+    def __call__(self, iterable: Iterable[Any]) -> Iterator[Any]:
+        return self._function(iterable)
 
     def __iter__(self):
-        for item in self._function(iter(self._iterable)):
+        for item in self(iter(self._iterable)):
             try:
                 yield item
             except Exception as e:
                 self._handler(e)
 
-    def derive(self):
-        # This can be overridden to derive to different Pipe subclass
+    def new(self):
         return Pipe()
 
-    def _derive(
-        self,
-        *iterable: Iterable,
-        function: Optional[Callable] = None,
-        handler: Optional[Callable] = None,
-    ):
-        return self.derive()._update(
-            *iterable or [self._iterable],
-            function=function or self._function,
-            handler=handler or self._handler,
-        )
-
     def __getattr__(self, name):
         def method(*args, **kwargs):
-            function = compose(self._function, self._functions[name](*args, **kwargs))
-            return self._derive(function=function)
+            pipe_fn = self._pipes[name](*args, **kwargs)
+            pipe = pipe_fn.new()
+            pipe._function = compose(self, pipe_fn)
+            pipe._iterable = self._iterable
+            pipe._handler = self._handler
+            return pipe
 
         return method
 
-    def __call__(self, *iterable):
-        return self._derive(*iterable)
-
     def close(self):
         # Necessary to use `yield from` on a Pipe object
         pass
 
     def list(self):
         return list(self)
 
     @classmethod
-    def add_fn(cls, fn: Type[Function], name: Optional[str] = None):
-        fn_name = camelcase_to_snakecase(fn.__name__) if name is None else name
-        cls._functions[fn_name] = fn
+    def register(cls, pipe_type: Type[Pipe], name: Optional[str] = None):
+        pipe_name = camelcase_to_snakecase(pipe_type.__name__) if name is None else name
+        cls._pipes[pipe_name] = pipe_type
```

### Comparing `pipd-0.1.9/pipd/pipes/merged.py` & `pipd-0.2.0/pipd/pipes/merged.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.9/pipd/tests/test_pipe.py` & `pipd-0.2.0/pipd/tests/test_pipe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pipd import Pipe
 
 
 def test_pipe():
-    pipe = Pipe(0, 1, 2, 3)
+    pipe = Pipe([0, 1, 2, 3])
     assert list(pipe) == [0, 1, 2, 3]
 
     pipe = Pipe([0, 1, 2, 3])
     assert list(pipe) == [0, 1, 2, 3]
 
     pipe = Pipe(range(4))
     assert list(pipe) == [0, 1, 2, 3]
@@ -27,18 +27,18 @@
         yield from pipe
 
     assert list(gen()) == [0, 1, 2, 3]
 
 
 def test_metaclass():
     pipe = Pipe
-    assert list(pipe(0, 1, 2, 3)) == [0, 1, 2, 3]
+    assert list(pipe([0, 1, 2, 3])) == [0, 1, 2, 3]
 
     pipe = Pipe.map(lambda x: x + 1)
-    assert list(pipe(0, 1, 2, 3)) == [1, 2, 3, 4]
+    assert list(pipe([0, 1, 2, 3])) == [1, 2, 3, 4]
 
 
 # def test_merge():
 #     pipe0 = Pipe(0, 0, 0, 0, 0, 0)
 #     pipe1 = Pipe(1, 1, 1, 1, 1, 1)
 #     pipe = Pipe.merge(pipe0, pipe1, weights=[3, 1])
 #     print(list(pipe))
```

