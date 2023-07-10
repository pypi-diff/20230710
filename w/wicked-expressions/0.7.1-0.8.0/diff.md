# Comparing `tmp/wicked_expressions-0.7.1.tar.gz` & `tmp/wicked_expressions-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.7.1.tar", max compression
+gzip compressed data, was "wicked_expressions-0.8.0.tar", max compression
```

## Comparing `wicked_expressions-0.7.1.tar` & `wicked_expressions-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-06-07 23:15:25.309006 wicked_expressions-0.7.1/LICENSE
--rw-r--r--   0        0        0     2119 2023-06-07 23:15:25.309006 wicked_expressions-0.7.1/README.md
--rw-r--r--   0        0        0     1219 2023-06-07 23:16:58.194575 wicked_expressions-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-06-07 23:16:58.174575 wicked_expressions-0.7.1/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      714 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     9084 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     1850 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      360 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8436 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1333 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     6303 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-10 19:15:59.395522 wicked_expressions-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2166 2023-07-10 19:15:59.395522 wicked_expressions-0.8.0/README.md
+-rw-r--r--   0        0        0     1219 2023-07-10 19:17:39.854281 wicked_expressions-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-10 19:17:39.838281 wicked_expressions-0.8.0/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     9084 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      402 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8436 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1460 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     6454 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-07-10 19:15:59.403523 wicked_expressions-0.8.0/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 wicked_expressions-0.8.0/PKG-INFO
```

### Comparing `wicked_expressions-0.7.1/LICENSE` & `wicked_expressions-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.1/README.md` & `wicked_expressions-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -36,35 +36,39 @@
 
 ```bash
 pip install wicked_expressions
 ```
 
 ## Getting started
 
-This package is designed to be used within any `bolt` script (either a `.mcfunction` or `bolt` file) inside a `bolt` enabled project.
+The library is designed to be used within any `bolt` script (either a `.mcfunction` or `bolt` file) inside a `bolt` enabled project.
+
 ```yaml
 require:
     - bolt
     - wicked_expressions
 
 pipeline:
     - mecha
 ```
 
-Once you've required `bolt` and `wicked_expressions`, you are able to import the python package's `api` module directly inside your bolt scripts.
+Once you've required `bolt` and `wicked_expressions`, you are able to import the package's `api` module directly inside your bolt script.
+
+Most of the imports come from the `wicked_expressions:api` module as shown below.
 
 ```py
-from wicked_expressions:api import Scoreboard, Data
+from wicked_expressions:api import Scoreboard
 ```
 
-Now you're free to use the API objects. Create simple and complex expressions, compare storages with scores, scores with scores, check if scores exist and more.
+Now you're free to use the API. Use simple and complex expressions, compare expressions and have access to many more features of the library!
+
 
 ## Documentation
 
-Check the docs out [here](./docs/home.md).
+Docs available [here](./docs/home.md).
 
 ## Features
 
 - Most if not all the functionality of [bolt-expressions](https://github.com/rx-modules/bolt-expressions).
 - Built in score & data comparison using python's comparison operators.
 - Useful functions and methods especially for bolt library developers such as `.store()` and `.get()`.
 - Anonymous runtime variables.
```

### Comparing `wicked_expressions-0.7.1/pyproject.toml` & `wicked_expressions-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.7.1"
+version = "0.8.0"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/api.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from bolt_expressions.node import ExpressionNode
 from bolt_expressions import Expression
 
 from ./sources import ScoreSource, DataSource
 from ./comparison import ExpressionComparison
 from ./raw_operations import StoreExpressionValue, GetExpressionValue
 from ./var import Var, StaticVar
-from ./nbtlib import Any, Bool, Byte, Short, Int, Long, Float, Double, String, List
+from ./nbtlib import Any, Bool, Byte, Short, Int, Long, Float, Double, String, List, IntArray
 # from ./datastash import DataStash
 from ./rebindable import Rebindable
 
 import ./internal_api as internal_api
 
 
 Scoreboard = ctx.inject(internal_api.Scoreboard)
 Data = ctx.inject(internal_api.Data)
 
 this = Data.entity('@s')
 
 
 ExpressionComparison.monkeypatch(Scoreboard, Data, ScoreSource, DataSource)
 # DataStash.monkeypatch(Scoreboard, Data)
+
```

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/comparison.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/var.bolt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ./var_sources as sources
-from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List, Any
+from ./nbtlib import Bool, Byte, Short, Int, Long, Float, Double, String, List, Any, IntArray
 
 
 class Var:
     is_static = False
 
     def __new__(self, type_annotation):
         if type_annotation == Any:
@@ -22,10 +22,12 @@
             return sources.FloatSource.create(is_static=self.is_static)
         elif type_annotation == Double:
             return sources.DoubleSource.create(is_static=self.is_static)
         elif type_annotation == String:
             return sources.StringSource.create(is_static=self.is_static)
         elif type_annotation == List:
             return sources.ListSource.create(is_static=self.is_static)
+        elif type_annotation == IntArray:
+            return sources.IntArraySource.create(is_static=self.is_static)
 
 class StaticVar(Var):
     is_static = True
```

### Comparing `wicked_expressions-0.7.1/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.8.0/wicked_expressions/modules/var_sources.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -189,9 +189,14 @@
         return super()._rebind(source, value)
 
 class ListSource(VarStorageSource):
     _default_nbt_type = 'list'
     _var_type = 'list'
     _default_slot_value = []
 
+class IntArraySource(VarStorageSource):
+    _default_nbt_type = 'int_array'
+    _var_type = 'int_array'
+    _default_slot_value = nbtlib.IntArray([])
+
 def base64_encode(s: str) -> str:
     return base64.b64encode(s.encode()).decode()
```

### Comparing `wicked_expressions-0.7.1/PKG-INFO` & `wicked_expressions-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.7.1
+Version: 0.8.0
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -56,35 +56,39 @@
 
 ```bash
 pip install wicked_expressions
 ```
 
 ## Getting started
 
-This package is designed to be used within any `bolt` script (either a `.mcfunction` or `bolt` file) inside a `bolt` enabled project.
+The library is designed to be used within any `bolt` script (either a `.mcfunction` or `bolt` file) inside a `bolt` enabled project.
+
 ```yaml
 require:
     - bolt
     - wicked_expressions
 
 pipeline:
     - mecha
 ```
 
-Once you've required `bolt` and `wicked_expressions`, you are able to import the python package's `api` module directly inside your bolt scripts.
+Once you've required `bolt` and `wicked_expressions`, you are able to import the package's `api` module directly inside your bolt script.
+
+Most of the imports come from the `wicked_expressions:api` module as shown below.
 
 ```py
-from wicked_expressions:api import Scoreboard, Data
+from wicked_expressions:api import Scoreboard
 ```
 
-Now you're free to use the API objects. Create simple and complex expressions, compare storages with scores, scores with scores, check if scores exist and more.
+Now you're free to use the API. Use simple and complex expressions, compare expressions and have access to many more features of the library!
+
 
 ## Documentation
 
-Check the docs out [here](./docs/home.md).
+Docs available [here](./docs/home.md).
 
 ## Features
 
 - Most if not all the functionality of [bolt-expressions](https://github.com/rx-modules/bolt-expressions).
 - Built in score & data comparison using python's comparison operators.
 - Useful functions and methods especially for bolt library developers such as `.store()` and `.get()`.
 - Anonymous runtime variables.
```

