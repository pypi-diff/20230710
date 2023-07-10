# Comparing `tmp/grizzlaxy-0.0.1.tar.gz` & `tmp/grizzlaxy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzlaxy-0.0.1.tar", max compression
+gzip compressed data, was "grizzlaxy-0.0.2.tar", max compression
```

## Comparing `grizzlaxy-0.0.1.tar` & `grizzlaxy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1061 2023-06-22 00:33:43.206354 grizzlaxy-0.0.1/LICENSE
--rw-r--r--   0        0        0      151 2023-06-26 19:43:56.507337 grizzlaxy-0.0.1/README.md
--rw-r--r--   0        0        0      118 2023-06-26 23:50:12.915343 grizzlaxy-0.0.1/grizzlaxy/__init__.py
--rw-r--r--   0        0        0     2130 2023-06-26 19:44:22.060694 grizzlaxy-0.0.1/grizzlaxy/auth.py
--rw-r--r--   0        0        0     3011 2023-06-29 18:00:44.549760 grizzlaxy-0.0.1/grizzlaxy/cli.py
--rw-r--r--   0        0        0     2006 2023-06-29 18:10:27.015525 grizzlaxy-0.0.1/grizzlaxy/find.py
--rw-r--r--   0        0        0      839 2023-06-26 22:46:58.615100 grizzlaxy-0.0.1/grizzlaxy/index-template.html
--rw-r--r--   0        0        0     1630 2023-06-27 04:56:06.133730 grizzlaxy-0.0.1/grizzlaxy/index.py
--rw-r--r--   0        0        0      157 2023-06-26 23:46:44.866597 grizzlaxy-0.0.1/grizzlaxy/utils.py
--rw-r--r--   0        0        0       18 2023-07-06 04:22:57.635642 grizzlaxy-0.0.1/grizzlaxy/version.py
--rw-r--r--   0        0        0      626 2023-07-06 04:22:57.611476 grizzlaxy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 grizzlaxy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-22 00:33:43.206354 grizzlaxy-0.0.2/LICENSE
+-rw-r--r--   0        0        0      151 2023-06-26 19:43:56.507337 grizzlaxy-0.0.2/README.md
+-rw-r--r--   0        0        0      118 2023-06-26 23:50:12.915343 grizzlaxy-0.0.2/grizzlaxy/__init__.py
+-rw-r--r--   0        0        0     2130 2023-07-10 18:00:10.881785 grizzlaxy-0.0.2/grizzlaxy/auth.py
+-rw-r--r--   0        0        0     3009 2023-07-10 17:45:04.695412 grizzlaxy-0.0.2/grizzlaxy/cli.py
+-rw-r--r--   0        0        0     2231 2023-07-10 18:00:24.649951 grizzlaxy-0.0.2/grizzlaxy/find.py
+-rw-r--r--   0        0        0      839 2023-06-26 22:46:58.615100 grizzlaxy-0.0.2/grizzlaxy/index-template.html
+-rw-r--r--   0        0        0     1630 2023-06-27 04:56:06.133730 grizzlaxy-0.0.2/grizzlaxy/index.py
+-rw-r--r--   0        0        0      157 2023-06-26 23:46:44.866597 grizzlaxy-0.0.2/grizzlaxy/utils.py
+-rw-r--r--   0        0        0       18 2023-07-10 18:00:59.894794 grizzlaxy-0.0.2/grizzlaxy/version.py
+-rw-r--r--   0        0        0      626 2023-07-10 18:00:59.872480 grizzlaxy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 grizzlaxy-0.0.2/PKG-INFO
```

### Comparing `grizzlaxy-0.0.1/LICENSE` & `grizzlaxy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.0.1/grizzlaxy/auth.py` & `grizzlaxy-0.0.2/grizzlaxy/auth.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.0.1/grizzlaxy/cli.py` & `grizzlaxy-0.0.2/grizzlaxy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     if options.root:
         collected = collect_routes(options.root)
     elif options.module:
         collected = collect_routes_from_module(importlib.import_module(options.module))
 
     routes = compile_routes("/", collected)
 
-    app = Starlette(routes=[routes])
+    app = Starlette(routes=routes)
 
     if options.ssl_keyfile:
         # This doesn't seem to do anything?
         app.add_middleware(HTTPSRedirectMiddleware)
 
     if options.secrets:
         config = Config(options.secrets)
```

### Comparing `grizzlaxy-0.0.1/grizzlaxy/find.py` & `grizzlaxy-0.0.2/grizzlaxy/find.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Find spacebears/routes in a file or directory"""
 
 import importlib
 import pkgutil
 import runpy
+from functools import reduce
 from pathlib import Path
 
 from ovld import ovld
 from starbear.serve import MotherBear
 from starlette.routing import Mount, Route
 
 from .index import Index
@@ -29,14 +30,25 @@
             submod = importlib.import_module(info.name)
             path = f"/{submod.__name__.split('.')[-1]}/"
             process_module(path, submod, info.ispkg)
 
     return routes
 
 
+def _flatten(routes):
+    return reduce(list.__iadd__, routes, [])
+
+
+def _mount(path, routes):
+    if path == "/":
+        return routes
+    else:
+        return [Mount(path, routes=routes)]
+
+
 def collect_routes(path):
     path = Path(path)
     if not path.exists():
         raise FileNotFoundError(f"Cannot find route from non-existent path: {path}")
 
     route_path = f"/{path.stem}"
 
@@ -53,22 +65,24 @@
 def compile_routes(path, routes: dict):
     routes = dict(routes)
     if "/" not in routes:
         if "/index/" in routes:
             routes["/"] = routes["/index/"]
         else:
             routes["/"] = Index()
-    routes = [compile_routes(path2, route) for path2, route in routes.items()]
-    return Mount(path, routes=routes)
+    return _mount(
+        path,
+        _flatten([compile_routes(path2, route) for path2, route in routes.items()]),
+    )
 
 
 @ovld
 def compile_routes(path, mb: MotherBear):  # noqa: F811
-    return Mount(path, routes=mb.routes())
+    return _mount(path, mb.routes())
 
 
 @ovld
 def compile_routes(path, obj: object):  # noqa: F811
     if callable(obj):
-        return Route(path, obj)
+        return [Route(path, obj)]
     else:
         raise TypeError(f"Cannot compile route for {path}: {obj}")
```

### Comparing `grizzlaxy-0.0.1/grizzlaxy/index-template.html` & `grizzlaxy-0.0.2/grizzlaxy/index-template.html`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.0.1/grizzlaxy/index.py` & `grizzlaxy-0.0.2/grizzlaxy/index.py`

 * *Files identical despite different names*

### Comparing `grizzlaxy-0.0.1/pyproject.toml` & `grizzlaxy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grizzlaxy"
-version = "0.0.1"
+version = "0.0.2"
 description = "Create an app from a galaxy of starbears"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `grizzlaxy-0.0.1/PKG-INFO` & `grizzlaxy-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzlaxy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create an app from a galaxy of starbears
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

