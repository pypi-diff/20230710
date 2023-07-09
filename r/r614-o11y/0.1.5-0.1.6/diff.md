# Comparing `tmp/r614_o11y-0.1.5.tar.gz` & `tmp/r614_o11y-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r614_o11y-0.1.5.tar", max compression
+gzip compressed data, was "r614_o11y-0.1.6.tar", max compression
```

## Comparing `r614_o11y-0.1.5.tar` & `r614_o11y-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7052 2023-07-09 21:34:00.286073 r614_o11y-0.1.5/LICENSE
--rw-r--r--   0        0        0       14 2023-07-09 21:34:00.286152 r614_o11y-0.1.5/README.md
--rw-r--r--   0        0        0     1239 2023-07-09 22:05:33.914385 r614_o11y-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 21:34:00.286223 r614_o11y-0.1.5/r614_o11y/__init__.py
--rw-r--r--   0        0        0     7047 2023-07-09 22:05:13.133479 r614_o11y-0.1.5/r614_o11y/o11y.py
--rw-r--r--   0        0        0        0 2023-07-09 21:34:00.286378 r614_o11y-0.1.5/r614_o11y/py.typed
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 r614_o11y-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-07-09 21:34:00.286073 r614_o11y-0.1.6/LICENSE
+-rw-r--r--   0        0        0       14 2023-07-09 21:34:00.286152 r614_o11y-0.1.6/README.md
+-rw-r--r--   0        0        0     1239 2023-07-09 22:09:09.910229 r614_o11y-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 21:34:00.286223 r614_o11y-0.1.6/r614_o11y/__init__.py
+-rw-r--r--   0        0        0     7047 2023-07-09 22:05:13.133479 r614_o11y-0.1.6/r614_o11y/o11y.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:34:00.286378 r614_o11y-0.1.6/r614_o11y/py.typed
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 r614_o11y-0.1.6/PKG-INFO
```

### Comparing `r614_o11y-0.1.5/LICENSE` & `r614_o11y-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `r614_o11y-0.1.5/pyproject.toml` & `r614_o11y-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "r614-o11y"
-version = "0.1.5"
+version = "0.1.6"
 description = "Observability modules"
 authors = ["Roshan Pawar <steradian614@gmail.com>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "r614_o11y"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-r614-config = "^0.1.5"
+r614-config = "^0.1.7"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 opentelemetry-exporter-otlp-proto-grpc = "^1.15.0"
 orjson = "^3.8.5"
 structlog = "^22.3.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `r614_o11y-0.1.5/r614_o11y/o11y.py` & `r614_o11y-0.1.6/r614_o11y/o11y.py`

 * *Files identical despite different names*

### Comparing `r614_o11y-0.1.5/PKG-INFO` & `r614_o11y-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: r614-o11y
-Version: 0.1.5
+Version: 0.1.6
 Summary: Observability modules
 License: CC0 1.0
 Author: Roshan Pawar
 Author-email: steradian614@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: orjson (>=3.8.5,<4.0.0)
-Requires-Dist: r614-config (>=0.1.5,<0.2.0)
+Requires-Dist: r614-config (>=0.1.7,<0.2.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Description-Content-Type: text/markdown
 
 # python-o11y
```

