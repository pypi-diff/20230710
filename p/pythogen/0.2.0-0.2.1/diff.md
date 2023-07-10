# Comparing `tmp/pythogen-0.2.0.tar.gz` & `tmp/pythogen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.0.tar", max compression
+gzip compressed data, was "pythogen-0.2.1.tar", max compression
```

## Comparing `pythogen-0.2.0.tar` & `pythogen-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-07-07 14:39:08.663445 pythogen-0.2.0/LICENSE
--rw-r--r--   0        0        0     2097 2023-07-07 14:39:08.663445 pythogen-0.2.0/README.md
--rw-r--r--   0        0        0     1567 2023-07-07 14:39:08.671445 pythogen-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1585 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/entrypoint.py
--rw-r--r--   0        0        0     7059 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/models.py
--rw-r--r--   0        0        0     2329 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3239 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/response.py
--rw-r--r--   0        0        0    16508 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0     9844 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/renderer.py
--rw-r--r--   0        0        0      172 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/settings.py
--rw-r--r--   0        0        0     5149 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/client/httpx-method.j2
--rw-r--r--   0        0        0     1668 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/client/httpx-request-metrics.j2
--rw-r--r--   0        0        0    10825 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/httpx.j2
--rw-r--r--   0        0        0       33 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/init-py.j2
--rw-r--r--   0        0        0      337 2023-07-07 14:39:08.671445 pythogen-0.2.0/pythogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-10 08:06:02.351284 pythogen-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2097 2023-07-10 08:06:02.351284 pythogen-0.2.1/README.md
+-rw-r--r--   0        0        0     1567 2023-07-10 08:06:02.355284 pythogen-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1585 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/entrypoint.py
+-rw-r--r--   0        0        0     7059 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/models.py
+-rw-r--r--   0        0        0     2329 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3239 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    16508 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0     9844 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/renderer.py
+-rw-r--r--   0        0        0      172 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/settings.py
+-rw-r--r--   0        0        0     5149 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/client/httpx-method.j2
+-rw-r--r--   0        0        0     1668 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/client/httpx-request-metrics.j2
+-rw-r--r--   0        0        0    10825 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/httpx.j2
+-rw-r--r--   0        0        0       33 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-10 08:06:02.355284 pythogen-0.2.1/pythogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pythogen-0.2.1/PKG-INFO
```

### Comparing `pythogen-0.2.0/LICENSE` & `pythogen-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/README.md` & `pythogen-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pyproject.toml` & `pythogen-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.0"
+version = "0.2.1"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
```

### Comparing `pythogen-0.2.0/pythogen/entrypoint.py` & `pythogen-0.2.1/pythogen/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/models.py` & `pythogen-0.2.1/pythogen/models.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/packager.py` & `pythogen-0.2.1/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/document.py` & `pythogen-0.2.1/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.1/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/operations.py` & `pythogen-0.2.1/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/parameters.py` & `pythogen-0.2.1/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/paths.py` & `pythogen-0.2.1/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/references.py` & `pythogen-0.2.1/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/request_body.py` & `pythogen-0.2.1/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/response.py` & `pythogen-0.2.1/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/parsers/schemas.py` & `pythogen-0.2.1/pythogen/parsers/schemas.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/renderer.py` & `pythogen-0.2.1/pythogen/renderer.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/templates/client/httpx-method.j2` & `pythogen-0.2.1/pythogen/templates/client/httpx-method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/templates/client/httpx-request-metrics.j2` & `pythogen-0.2.1/pythogen/templates/client/httpx-request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/pythogen/templates/httpx.j2` & `pythogen-0.2.1/pythogen/templates/httpx.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.0/PKG-INFO` & `pythogen-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
```

