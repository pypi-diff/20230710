# Comparing `tmp/microservice-utils-0.9.2.tar.gz` & `tmp/microservice-utils-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservice-utils-0.9.2.tar", last modified: Wed Jul  5 22:45:59 2023, max compression
+gzip compressed data, was "microservice-utils-0.9.3.tar", last modified: Mon Jul 10 20:20:19 2023, max compression
```

## Comparing `microservice-utils-0.9.2.tar` & `microservice-utils-0.9.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.063137 microservice-utils-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-05 22:45:59.063137 microservice-utils-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.051137 microservice-utils-0.9.2/microservice_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.055137 microservice-utils-0.9.2/microservice_utils/google_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/google_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.055137 microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/cloud_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/google_cloud/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.055137 microservice-utils-0.9.2/microservice_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/openai/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.059137 microservice-utils-0.9.2/microservice_utils/pinecone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/pinecone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/microservice_utils/pinecone/adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.055137 microservice-utils-0.9.2/microservice_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-05 22:45:59.000000 microservice-utils-0.9.2/microservice_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-05 22:45:59.000000 microservice-utils-0.9.2/microservice_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:45:59.000000 microservice-utils-0.9.2/microservice_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 22:45:59.000000 microservice-utils-0.9.2/microservice_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 22:45:59.000000 microservice-utils-0.9.2/microservice_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:45:59.063137 microservice-utils-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.059137 microservice-utils-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.059137 microservice-utils-0.9.2/tests/google_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/google_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/google_cloud/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/google_cloud/test_cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:59.059137 microservice-utils-0.9.2/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/openai/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-05 22:44:33.000000 microservice-utils-0.9.2/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.211804 microservice-utils-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-10 20:20:19.211804 microservice-utils-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.203804 microservice-utils-0.9.3/microservice_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.207804 microservice-utils-0.9.3/microservice_utils/google_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/google_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.207804 microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/cloud_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/google_cloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.207804 microservice-utils-0.9.3/microservice_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/openai/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.207804 microservice-utils-0.9.3/microservice_utils/pinecone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/pinecone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/microservice_utils/pinecone/adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.203804 microservice-utils-0.9.3/microservice_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-10 20:20:19.000000 microservice-utils-0.9.3/microservice_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-10 20:20:19.000000 microservice-utils-0.9.3/microservice_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:20:19.000000 microservice-utils-0.9.3/microservice_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-10 20:20:19.000000 microservice-utils-0.9.3/microservice_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 20:20:19.000000 microservice-utils-0.9.3/microservice_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:20:19.211804 microservice-utils-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.207804 microservice-utils-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.207804 microservice-utils-0.9.3/tests/google_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/google_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/google_cloud/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/google_cloud/test_cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:20:19.211804 microservice-utils-0.9.3/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/openai/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-10 20:18:47.000000 microservice-utils-0.9.3/tests/test_events.py
```

### Comparing `microservice-utils-0.9.2/LICENSE` & `microservice-utils-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/PKG-INFO` & `microservice-utils-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservice-utils
-Version: 0.9.2
+Version: 0.9.3
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: events
 Provides-Extra: gcp_cloud_run
 Provides-Extra: gcp_cloud_tasks
 Provides-Extra: gcp_pubsub
```

### Comparing `microservice-utils-0.9.2/README.md` & `microservice-utils-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/events.py` & `microservice-utils-0.9.3/microservice_utils/events.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/cloud_logging.py` & `microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/cloud_logging.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/cloud_run.py` & `microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/cloud_run.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/cloud_tasks.py` & `microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/google_cloud/adapters/pubsub.py` & `microservice-utils-0.9.3/microservice_utils/google_cloud/adapters/pubsub.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/google_cloud/models.py` & `microservice-utils-0.9.3/microservice_utils/google_cloud/models.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/graphql.py` & `microservice-utils-0.9.3/microservice_utils/graphql.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/openai/adapters.py` & `microservice-utils-0.9.3/microservice_utils/openai/adapters.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/microservice_utils/pinecone/adapters.py` & `microservice-utils-0.9.3/microservice_utils/pinecone/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         self._index_name = index_name
         self._namespace = namespace
 
     def _get_index(self):
         pinecone.init(api_key=self._api_key, environment=self._environment)
         return pinecone.Index(index_name=self._index_name)
 
+    def set_namespace(self, namespace: str):
+        self._namespace = namespace
+
     def upsert(
         self,
         items: typing.Union[typing.List[Vector], typing.List[tuple], typing.List[dict]],
     ):
         """Upsert items to the Pinecone index."""
         index = self._get_index()
         index.upsert(items, namespace=self._namespace)
```

### Comparing `microservice-utils-0.9.2/microservice_utils.egg-info/PKG-INFO` & `microservice-utils-0.9.3/microservice_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservice-utils
-Version: 0.9.2
+Version: 0.9.3
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: events
 Provides-Extra: gcp_cloud_run
 Provides-Extra: gcp_cloud_tasks
 Provides-Extra: gcp_pubsub
```

### Comparing `microservice-utils-0.9.2/microservice_utils.egg-info/SOURCES.txt` & `microservice-utils-0.9.3/microservice_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/setup.py` & `microservice-utils-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/tests/google_cloud/test_cloud_run.py` & `microservice-utils-0.9.3/tests/google_cloud/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/tests/graphql.py` & `microservice-utils-0.9.3/tests/graphql.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/tests/openai/test_adapters.py` & `microservice-utils-0.9.3/tests/openai/test_adapters.py`

 * *Files identical despite different names*

### Comparing `microservice-utils-0.9.2/tests/test_events.py` & `microservice-utils-0.9.3/tests/test_events.py`

 * *Files identical despite different names*

