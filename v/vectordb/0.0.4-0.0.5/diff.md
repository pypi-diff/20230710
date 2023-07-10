# Comparing `tmp/vectordb-0.0.4.tar.gz` & `tmp/vectordb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vectordb-0.0.4.tar", last modified: Mon Jul 10 09:54:53 2023, max compression
+gzip compressed data, was "dist/vectordb-0.0.5.tar", last modified: Mon Jul 10 10:27:04 2023, max compression
```

## Comparing `vectordb-0.0.4.tar` & `vectordb-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-10 09:54:53.000000 vectordb-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-10 09:54:38.000000 vectordb-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:54:53.000000 vectordb-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-10 09:54:38.000000 vectordb-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/integration/test_hnswlib_vectordb_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/integration/test_inmemory_vectordb_serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/unit/test_hnswlib_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-10 09:54:38.000000 vectordb-0.0.4/tests/unit/test_inmemory_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/db/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/db/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/create_doc_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/pass_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-10 09:54:38.000000 vectordb-0.0.4/vectordb/utils/unify_input_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 09:54:53.000000 vectordb-0.0.4/vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 09:54:52.000000 vectordb-0.0.4/vectordb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-07-10 10:27:04.000000 vectordb-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-10 10:26:50.000000 vectordb-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:27:04.000000 vectordb-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-10 10:26:50.000000 vectordb-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/integration/test_hnswlib_vectordb_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/integration/test_inmemory_vectordb_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/unit/test_hnswlib_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-10 10:26:50.000000 vectordb-0.0.5/tests/unit/test_inmemory_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb/db/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/db/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-10 10:26:50.000000 vectordb-0.0.5/vectordb/utils/unify_input_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 10:27:04.000000 vectordb-0.0.5/vectordb.egg-info/top_level.txt
```

### Comparing `vectordb-0.0.4/README.md` & `vectordb-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/setup.py` & `vectordb-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,31 @@
     version_line = [l.strip() for l in libinfo_content if l.startswith('__version__')][
         0
     ]
     exec(version_line)  # gives __version__
 except FileNotFoundError:
     __version__ = '0.0.0'
 
+try:
+    with open('README.md', encoding='utf-8') as fp:
+        _long_description = fp.read()
+except FileNotFoundError:
+    _long_description = ''
+
+
 # Read the contents of requirements.txt
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='vectordb',
     version=__version__,
     description='The Python VectorDB. Build your vector database from working as a library to scaling as a database in the cloud',
+    long_description=_long_description,
+    long_description_content_type='text/markdown',
     author='Jina AI',
     author_email='hello@jina.ai',
     license='Apache 2.0',
     url='https://github.com/jina-ai/vectordb/',
     download_url='https://github.com/jina-ai/vectordb/tags',
     packages=find_packages(),
     classifiers=[
```

### Comparing `vectordb-0.0.4/tests/integration/test_hnswlib_vectordb_serve.py` & `vectordb-0.0.5/tests/integration/test_hnswlib_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/tests/integration/test_inmemory_vectordb_serve.py` & `vectordb-0.0.5/tests/integration/test_inmemory_vectordb_serve.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/tests/unit/test_hnswlib_vectordb.py` & `vectordb-0.0.5/tests/unit/test_hnswlib_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/tests/unit/test_inmemory_vectordb.py` & `vectordb-0.0.5/tests/unit/test_inmemory_vectordb.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/__main__.py` & `vectordb-0.0.5/vectordb/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/client/client.py` & `vectordb-0.0.5/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/db/base.py` & `vectordb-0.0.5/vectordb/db/base.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/db/executors/hnsw_indexer.py` & `vectordb-0.0.5/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/db/executors/inmemory_exact_indexer.py` & `vectordb-0.0.5/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/db/executors/typed_executor.py` & `vectordb-0.0.5/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/db/service.py` & `vectordb-0.0.5/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/utils/create_doc_type.py` & `vectordb-0.0.5/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/utils/pass_parameters.py` & `vectordb-0.0.5/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/utils/push_to_hubble.py` & `vectordb-0.0.5/vectordb/utils/push_to_hubble.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/utils/sort_matches_by_score.py` & `vectordb-0.0.5/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb/utils/unify_input_output.py` & `vectordb-0.0.5/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vectordb-0.0.4/vectordb.egg-info/SOURCES.txt` & `vectordb-0.0.5/vectordb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

