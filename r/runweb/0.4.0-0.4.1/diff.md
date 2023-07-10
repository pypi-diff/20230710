# Comparing `tmp/runweb-0.4.0.tar.gz` & `tmp/runweb-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runweb-0.4.0.tar", last modified: Sun Jul  9 14:28:13 2023, max compression
+gzip compressed data, was "runweb-0.4.1.tar", last modified: Mon Jul 10 08:17:46 2023, max compression
```

## Comparing `runweb-0.4.0.tar` & `runweb-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11341 2023-07-09 14:27:53.096817 runweb-0.4.0/LICENSE
--rw-r--r--   0        0        0      729 2023-07-09 14:27:53.096817 runweb-0.4.0/README.md
--rw-r--r--   0        0        0     1295 2023-07-09 14:28:13.704990 runweb-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/__init__.py
--rw-r--r--   0        0        0       29 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/__main__.py
--rw-r--r--   0        0        0       22 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/__version__.py
--rw-r--r--   0        0        0      147 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/logging.py
--rw-r--r--   0        0        0     3572 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/main.py
--rw-r--r--   0        0        0     2205 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/multiprocess.py
--rw-r--r--   0        0        0     1640 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/parse.py
--rw-r--r--   0        0        0        0 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/runner/__init__.py
--rw-r--r--   0        0        0     1006 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/runner/uvicorn.py
--rw-r--r--   0        0        0      983 2023-07-09 14:27:53.096817 runweb-0.4.0/runweb/runner/waitress.py
--rw-r--r--   0        0        0        0 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      930 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/test_uvicorn.py
--rw-r--r--   0        0        0      934 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/test_waitress.py
--rw-r--r--   0        0        0      866 2023-07-09 14:27:53.096817 runweb-0.4.0/tests/utils.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-10 08:17:31.643421 runweb-0.4.1/LICENSE
+-rw-r--r--   0        0        0      729 2023-07-10 08:17:31.643421 runweb-0.4.1/README.md
+-rw-r--r--   0        0        0     1295 2023-07-10 08:17:46.571582 runweb-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/__version__.py
+-rw-r--r--   0        0        0      147 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/logging.py
+-rw-r--r--   0        0        0     3630 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/main.py
+-rw-r--r--   0        0        0     2205 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/multiprocess.py
+-rw-r--r--   0        0        0     1640 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/parse.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/runner/__init__.py
+-rw-r--r--   0        0        0     1006 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/runner/uvicorn.py
+-rw-r--r--   0        0        0      983 2023-07-10 08:17:31.643421 runweb-0.4.1/runweb/runner/waitress.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:17:31.643421 runweb-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-10 08:17:31.643421 runweb-0.4.1/tests/test_uvicorn.py
+-rw-r--r--   0        0        0      934 2023-07-10 08:17:31.643421 runweb-0.4.1/tests/test_waitress.py
+-rw-r--r--   0        0        0      866 2023-07-10 08:17:31.643421 runweb-0.4.1/tests/utils.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.4.1/PKG-INFO
```

### Comparing `runweb-0.4.0/LICENSE` & `runweb-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/README.md` & `runweb-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/pyproject.toml` & `runweb-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "click>=8.1.3",
 ]
 description = "Run web server with one command."
 dynamic = []
 name = "runweb"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.4.0"
+version = "0.4.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 tui = [
     "trogon>=0.4.0",
```

### Comparing `runweb-0.4.0/runweb/main.py` & `runweb-0.4.1/runweb/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import sys
 from typing import Union
 
 import click
 
 from .parse import parse_application
 
 SERVERS = {"wsgi": {}, "asgi": {}}
@@ -72,14 +74,16 @@
     server_name: Union[str, None],
     interface: Union[str, None],
     application: str,
     bind_address: str,
     autoreload: bool,
     workers_num: Union[int, None],
 ) -> None:
+    sys.path.insert(0, os.getcwd())
+
     if ctx.invoked_subcommand is not None:
         return
 
     if application is None:
         raise click.UsageError("Missing option '--application' / '-a'.")
 
     app_object = parse_application(application)
```

### Comparing `runweb-0.4.0/runweb/multiprocess.py` & `runweb-0.4.1/runweb/multiprocess.py`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/runweb/parse.py` & `runweb-0.4.1/runweb/parse.py`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/runweb/runner/uvicorn.py` & `runweb-0.4.1/runweb/runner/uvicorn.py`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/runweb/runner/waitress.py` & `runweb-0.4.1/runweb/runner/waitress.py`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/tests/test_uvicorn.py` & `runweb-0.4.1/tests/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/tests/test_waitress.py` & `runweb-0.4.1/tests/test_waitress.py`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/tests/utils.py` & `runweb-0.4.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `runweb-0.4.0/PKG-INFO` & `runweb-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runweb
-Version: 0.4.0
+Version: 0.4.1
 Summary: Run web server with one command.
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Requires-Dist: click>=8.1.3
 Requires-Dist: trogon>=0.4.0; extra == "tui"
 Requires-Dist: waitress; extra == "waitress"
```

