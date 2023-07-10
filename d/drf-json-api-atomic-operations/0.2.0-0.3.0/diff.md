# Comparing `tmp/drf-json-api-atomic-operations-0.2.0.tar.gz` & `tmp/drf-json-api-atomic-operations-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-json-api-atomic-operations-0.2.0.tar", last modified: Thu Jul  6 07:21:43 2023, max compression
+gzip compressed data, was "drf-json-api-atomic-operations-0.3.0.tar", last modified: Mon Jul 10 05:56:59 2023, max compression
```

## Comparing `drf-json-api-atomic-operations-0.2.0.tar` & `drf-json-api-atomic-operations-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.583011 drf-json-api-atomic-operations-0.2.0/atomic_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/atomic_operations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 07:21:43.000000 drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:21:43.587011 drf-json-api-atomic-operations-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-07-06 07:21:39.000000 drf-json-api-atomic-operations-0.2.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:56:59.378855 drf-json-api-atomic-operations-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-10 05:56:59.378855 drf-json-api-atomic-operations-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:56:59.374855 drf-json-api-atomic-operations-0.3.0/atomic_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/atomic_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/atomic_operations/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/atomic_operations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/atomic_operations/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/atomic_operations/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/atomic_operations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:56:59.374855 drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-10 05:56:59.000000 drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-10 05:56:59.000000 drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:56:59.000000 drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:56:59.000000 drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 05:56:59.000000 drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 05:56:59.000000 drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-10 05:56:59.378855 drf-json-api-atomic-operations-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:56:59.374855 drf-json-api-atomic-operations-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-07-10 05:56:55.000000 drf-json-api-atomic-operations-0.3.0/tests/test_views.py
```

### Comparing `drf-json-api-atomic-operations-0.2.0/LICENSE` & `drf-json-api-atomic-operations-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.2.0/PKG-INFO` & `drf-json-api-atomic-operations-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-json-api-atomic-operations
-Version: 0.2.0
+Version: 0.3.0
 Summary: Extension for `django-rest-framework-json-api <https://github.com/django-json-api/django-rest-framework-json-api>`_ to support `atomic operations <https://jsonapi.org/ext/atomic/>`_.
 Home-page: https://github.com/jokiefer/drf-json-api-atomic-operations/
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
 License: MIT-License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -43,19 +43,18 @@
 See the `usage <https://drf-json-api-atomic-operations.readthedocs.io/en/latest/usage.html>`_ section of the docs for example integration.
 
 
 
 Implemented Features
 ~~~~~~~~~~~~~~~~~~~~
 
-* creating, updating, removing multiple resources in a single request (sequential db calls)
+* creating, updating, removing multiple resources in a single request (sequential db calls optional bulk db calls for create and delete)
 * `Updating To-One Relationships <https://jsonapi.org/ext/atomic/#auto-id-updating-to-one-relationships>`_
 * `Updating To-Many Relationships <https://jsonapi.org/ext/atomic/#auto-id-updating-to-many-relationships>`_
 * error reporting with json pointer to the concrete operation and the wrong attributes
 
 
 ToDo
 ~~~~
 
 * permission handling
-* use django bulk operations to optimize db execution time
 * `local identity (lid) <https://jsonapi.org/ext/atomic/#operation-objects>`_ handling
```

### Comparing `drf-json-api-atomic-operations-0.2.0/README.rst` & `drf-json-api-atomic-operations-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 See the `usage <https://drf-json-api-atomic-operations.readthedocs.io/en/latest/usage.html>`_ section of the docs for example integration.
 
 
 
 Implemented Features
 ~~~~~~~~~~~~~~~~~~~~
 
-* creating, updating, removing multiple resources in a single request (sequential db calls)
+* creating, updating, removing multiple resources in a single request (sequential db calls optional bulk db calls for create and delete)
 * `Updating To-One Relationships <https://jsonapi.org/ext/atomic/#auto-id-updating-to-one-relationships>`_
 * `Updating To-Many Relationships <https://jsonapi.org/ext/atomic/#auto-id-updating-to-many-relationships>`_
 * error reporting with json pointer to the concrete operation and the wrong attributes
 
 
 ToDo
 ~~~~
 
 * permission handling
-* use django bulk operations to optimize db execution time
 * `local identity (lid) <https://jsonapi.org/ext/atomic/#operation-objects>`_ handling
```

### Comparing `drf-json-api-atomic-operations-0.2.0/atomic_operations/exceptions.py` & `drf-json-api-atomic-operations-0.3.0/atomic_operations/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.2.0/atomic_operations/parsers.py` & `drf-json-api-atomic-operations-0.3.0/atomic_operations/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
             self.check_relation_update(idx, operation)
         else:
             data = operation.get("data")
             if not data:
                 raise MissingPrimaryData(idx)
             elif not isinstance(data, dict):
                 raise InvalidPrimaryDataType(idx, "object")
+            self.check_resource_identifier_object(idx, data, operation["op"])
 
     def check_remove_operation(self, idx, ref):
         if not ref:
             raise JsonApiParseError(
                 id="missing-ref-attribute",
                 detail="`ref` must be part of remove operation",
                 pointer=f"/{ATOMIC_OPERATIONS}/{idx}"
```

### Comparing `drf-json-api-atomic-operations-0.2.0/atomic_operations/renderers.py` & `drf-json-api-atomic-operations-0.3.0/atomic_operations/renderers.py`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/PKG-INFO` & `drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-json-api-atomic-operations
-Version: 0.2.0
+Version: 0.3.0
 Summary: Extension for `django-rest-framework-json-api <https://github.com/django-json-api/django-rest-framework-json-api>`_ to support `atomic operations <https://jsonapi.org/ext/atomic/>`_.
 Home-page: https://github.com/jokiefer/drf-json-api-atomic-operations/
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
 License: MIT-License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -43,19 +43,18 @@
 See the `usage <https://drf-json-api-atomic-operations.readthedocs.io/en/latest/usage.html>`_ section of the docs for example integration.
 
 
 
 Implemented Features
 ~~~~~~~~~~~~~~~~~~~~
 
-* creating, updating, removing multiple resources in a single request (sequential db calls)
+* creating, updating, removing multiple resources in a single request (sequential db calls optional bulk db calls for create and delete)
 * `Updating To-One Relationships <https://jsonapi.org/ext/atomic/#auto-id-updating-to-one-relationships>`_
 * `Updating To-Many Relationships <https://jsonapi.org/ext/atomic/#auto-id-updating-to-many-relationships>`_
 * error reporting with json pointer to the concrete operation and the wrong attributes
 
 
 ToDo
 ~~~~
 
 * permission handling
-* use django bulk operations to optimize db execution time
 * `local identity (lid) <https://jsonapi.org/ext/atomic/#operation-objects>`_ handling
```

### Comparing `drf-json-api-atomic-operations-0.2.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt` & `drf-json-api-atomic-operations-0.3.0/drf_json_api_atomic_operations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.2.0/setup.cfg` & `drf-json-api-atomic-operations-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.2.0/setup.py` & `drf-json-api-atomic-operations-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `drf-json-api-atomic-operations-0.2.0/tests/test_parsers.py` & `drf-json-api-atomic-operations-0.3.0/tests/test_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,35 @@
             self.parser.parse,
             **{
                 "stream": stream,
                 "parser_context": self.parser_context
             }
         )
 
+        data = {
+            ATOMIC_OPERATIONS: [
+                {
+                    "op": "update",
+                    "data": {
+                        "type": "articles",
+                    }
+                }
+            ]
+        }
+        stream = BytesIO(json.dumps(data).encode("utf-8"))
+        self.assertRaisesRegex(
+            JsonApiParseError,
+            "The resource identifier object must contain an `id` member",
+            self.parser.parse,
+            **{
+                "stream": stream,
+                "parser_context": self.parser_context
+            }
+        )
+
     def test_primary_data(self):
         data = {
             ATOMIC_OPERATIONS: [
                 {
                     "op": "update",
                     "id": "1",
                     "data": []
```

