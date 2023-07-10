# Comparing `tmp/vectordb-0.0.3.dev5.tar.gz` & `tmp/vectordb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb-0.0.3.dev5.tar", last modified: Wed Jul  5 12:41:51 2023, max compression
+gzip compressed data, was "dist/vectordb-0.0.4.tar", last modified: Mon Jul 10 09:54:53 2023, max compression
```

## Comparing `vectordb-0.0.3.dev5.tar` & `vectordb-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/integration/test_hnswlib_vectordb_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/integration/test_inmemory_vectordb_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/unit/test_hnswlib_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/tests/unit/test_inmemory_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-05 12:41:50.000000 vectordb-0.0.3.dev5/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb/db/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/db/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.091257 vectordb-0.0.3.dev5/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/create_doc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/pass_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-05 12:41:45.000000 vectordb-0.0.3.dev5/vectordb/utils/unify_input_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:51.087257 vectordb-0.0.3.dev5/vectordb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 12:41:51.000000 vectordb-0.0.3.dev5/vectordb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-10 09:54:53.000000 vectordb-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-10 09:54:38.000000 vectordb-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:54:53.000000 vectordb-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-10 09:54:38.000000 vectordb-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/integration/test_hnswlib_vectordb_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/integration/test_inmemory_vectordb_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/unit/test_hnswlib_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/unit/test_inmemory_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/db/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/unify_input_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `vectordb-0.0.3.dev5/PKG-INFO` & `vectordb-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.3.dev5
+Version: 0.0.4
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: test
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `vectordb-0.0.3.dev5/README.md` & `vectordb-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/setup.py` & `vectordb-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,10 +50,7 @@
             'pytest-repeat',
             'flaky',
             'pytest-timeout'
         ],
     },
     install_requires=requirements,
 )
-
-import subprocess
-subprocess.run(['pip', 'install', 'docarray[hnswlib]>=0.34.0'])
```

### Comparing `vectordb-0.0.3.dev5/tests/integration/test_hnswlib_vectordb_serve.py` & `vectordb-0.0.4/tests/integration/test_hnswlib_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/tests/integration/test_inmemory_vectordb_serve.py` & `vectordb-0.0.4/tests/integration/test_inmemory_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/tests/unit/test_hnswlib_vectordb.py` & `vectordb-0.0.4/tests/unit/test_hnswlib_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/tests/unit/test_inmemory_vectordb.py` & `vectordb-0.0.4/tests/unit/test_inmemory_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/__main__.py` & `vectordb-0.0.4/vectordb/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/client/client.py` & `vectordb-0.0.4/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/db/base.py` & `vectordb-0.0.4/vectordb/db/base.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/db/executors/hnsw_indexer.py` & `vectordb-0.0.4/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/db/executors/inmemory_exact_indexer.py` & `vectordb-0.0.4/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/db/executors/typed_executor.py` & `vectordb-0.0.4/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/db/service.py` & `vectordb-0.0.4/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/utils/create_doc_type.py` & `vectordb-0.0.4/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/utils/pass_parameters.py` & `vectordb-0.0.4/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/utils/push_to_hubble.py` & `vectordb-0.0.4/vectordb/utils/push_to_hubble.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/utils/sort_matches_by_score.py` & `vectordb-0.0.4/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb/utils/unify_input_output.py` & `vectordb-0.0.4/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.3.dev5/vectordb.egg-info/PKG-INFO` & `vectordb-0.0.4/vectordb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: vectordb
-Version: 0.0.3.dev5
+Version: 0.0.4
 Summary: The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud
 Home-page: https://github.com/jina-ai/vectordb/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/vectordb/tags
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Provides-Extra: test
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `vectordb-0.0.3.dev5/vectordb.egg-info/SOURCES.txt` & `vectordb-0.0.4/vectordb.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/test_hnswlib_vectordb_serve.py
 tests/integration/test_inmemory_vectordb_serve.py
```

