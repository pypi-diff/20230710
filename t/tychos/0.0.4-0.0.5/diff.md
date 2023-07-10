# Comparing `tmp/tychos-0.0.4.tar.gz` & `tmp/tychos-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.4.tar", last modified: Thu Jul  6 14:20:49 2023, max compression
+gzip compressed data, was "tychos-0.0.5.tar", last modified: Mon Jul 10 19:51:46 2023, max compression
```

## Comparing `tychos-0.0.4.tar` & `tychos-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:20:49.274849 tychos-0.0.4/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.4/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)     2705 2023-07-06 14:20:49.274678 tychos-0.0.4/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)     2518 2023-07-06 14:19:40.000000 tychos-0.0.4/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-06 14:20:49.274891 tychos-0.0.4/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-06 14:19:40.000000 tychos-0.0.4/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:20:49.272977 tychos-0.0.4/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)       74 2023-06-30 15:48:02.000000 tychos-0.0.4/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1084 2023-07-05 20:35:35.000000 tychos-0.0.4/tychos/cli.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:20:49.274437 tychos-0.0.4/tychos/helpers/
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.4/tychos/helpers/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)     1296 2023-06-30 20:02:27.000000 tychos-0.0.4/tychos/vector.py
--rw-r--r--   0 abe732     (501) staff       (20)     1259 2023-07-05 22:43:42.000000 tychos-0.0.4/tychos/vector_data_store.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-06 14:20:49.274186 tychos-0.0.4/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)     2705 2023-07-06 14:20:49.000000 tychos-0.0.4/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      313 2023-07-06 14:20:49.000000 tychos-0.0.4/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-06 14:20:49.000000 tychos-0.0.4/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-06 14:20:49.000000 tychos-0.0.4/tychos.egg-info/entry_points.txt
--rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-06 14:20:49.000000 tychos-0.0.4/tychos.egg-info/requires.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-06 14:20:49.000000 tychos-0.0.4/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.500985 tychos-0.0.5/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.5/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)     2852 2023-07-10 19:51:46.500818 tychos-0.0.5/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)     2665 2023-07-10 19:50:29.000000 tychos-0.0.5/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-07-10 19:51:46.501026 tychos-0.0.5/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)      502 2023-07-10 19:49:15.000000 tychos-0.0.5/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.499350 tychos-0.0.5/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)      276 2023-07-10 18:55:06.000000 tychos-0.0.5/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1092 2023-07-10 19:02:06.000000 tychos-0.0.5/tychos/cli.py
+-rw-r--r--   0 abe732     (501) staff       (20)      213 2023-07-10 18:12:08.000000 tychos-0.0.5/tychos/config.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.500662 tychos-0.0.5/tychos/helpers/
+-rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-30 14:56:23.000000 tychos-0.0.5/tychos/helpers/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1554 2023-07-10 19:48:44.000000 tychos-0.0.5/tychos/vector.py
+-rw-r--r--   0 abe732     (501) staff       (20)     1734 2023-07-10 19:40:28.000000 tychos-0.0.5/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-07-10 19:51:46.500534 tychos-0.0.5/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)     2852 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      330 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/entry_points.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        9 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/requires.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-07-10 19:51:46.000000 tychos-0.0.5/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.4/LICENSE` & `tychos-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tychos-0.0.4/PKG-INFO` & `tychos-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: tychos
-Version: 0.0.4
-Summary: Python client library for the Tychos API.
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
 You can find usage examples for the Tychos Python library in our [BioMed Demo App](https://demo.tychos.ai/) and the [/demo repo folder](https://github.com/tychos-ai/tychos).
 
 
@@ -31,26 +23,31 @@
 
 -   Python 2.7+ or Python 3.6+
 -   Requests
 
 ## Usage
 
 The library needs to be configured with your account's secret key which is
-available via the [Tychos Website][api-keys]. Set `tychos.api_key` to its
-value:
+available via the [Tychos Website][api-keys]. Either set the TYCHOS_API_KEY environment variable before using the library:
+
+```python
+import tychos
+export TYCHOS_API_KEY='sk_a9adj...'
+```
 
+Or initialize the VectorDataStore using an API key:
 ```python
 import tychos
-tychos.api_key = "sk_a9adji08..."
+data_store = tychos.VectorDataStore(api_key="sk_a9adj...")
 ```
 
 Query live vector datasets
 ```python
-# initialize data store with API key
-data_store = tychos.VectorDataStore(api_key="sk_a9adji08...")
+# initialize data store
+data_store = tychos.VectorDataStore()
 
 # list available datasets
 datasets = data_store.list()
 
 # get name of the first dataset's id
 print(datasets['data'][0]['name'])
```

### Comparing `tychos-0.0.4/README.md` & `tychos-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: tychos
+Version: 0.0.5
+Summary: Python client library for the Tychos API.
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
 applications written in the Python language. The Tychos API allows you to query live, hosted vector datasets in your LLM application without needing to manage your own vector database / embedding pipelines.
 
 You can find usage examples for the Tychos Python library in our [BioMed Demo App](https://demo.tychos.ai/) and the [/demo repo folder](https://github.com/tychos-ai/tychos).
 
 
@@ -23,26 +31,31 @@
 
 -   Python 2.7+ or Python 3.6+
 -   Requests
 
 ## Usage
 
 The library needs to be configured with your account's secret key which is
-available via the [Tychos Website][api-keys]. Set `tychos.api_key` to its
-value:
+available via the [Tychos Website][api-keys]. Either set the TYCHOS_API_KEY environment variable before using the library:
+
+```python
+import tychos
+export TYCHOS_API_KEY='sk_a9adj...'
+```
 
+Or initialize the VectorDataStore using an API key:
 ```python
 import tychos
-tychos.api_key = "sk_a9adji08..."
+data_store = tychos.VectorDataStore(api_key="sk_a9adj...")
 ```
 
 Query live vector datasets
 ```python
-# initialize data store with API key
-data_store = tychos.VectorDataStore(api_key="sk_a9adji08...")
+# initialize data store
+data_store = tychos.VectorDataStore()
 
 # list available datasets
 datasets = data_store.list()
 
 # get name of the first dataset's id
 print(datasets['data'][0]['name'])
```

### Comparing `tychos-0.0.4/tychos/cli.py` & `tychos-0.0.5/tychos/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import argparse
 from .vector_data_store import VectorDataStore
 
 def query(args):
-    tds = VectorDataStore(args.api_key)
+    tds = VectorDataStore(api_key=args.api_key)
     result = tds.query(args.name, args.query_string, args.limit)
     print(result)
 
 def main():
     parser = argparse.ArgumentParser(description='Tychos CLI')
     subparsers = parser.add_subparsers()
```

### Comparing `tychos-0.0.4/tychos.egg-info/PKG-INFO` & `tychos-0.0.5/tychos.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tychos
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python client library for the Tychos API.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tychos Python Library
 The Tychos Python library provides convenient access to the Tychos API from
@@ -31,26 +31,31 @@
 
 -   Python 2.7+ or Python 3.6+
 -   Requests
 
 ## Usage
 
 The library needs to be configured with your account's secret key which is
-available via the [Tychos Website][api-keys]. Set `tychos.api_key` to its
-value:
+available via the [Tychos Website][api-keys]. Either set the TYCHOS_API_KEY environment variable before using the library:
 
 ```python
 import tychos
-tychos.api_key = "sk_a9adji08..."
+export TYCHOS_API_KEY='sk_a9adj...'
+```
+
+Or initialize the VectorDataStore using an API key:
+```python
+import tychos
+data_store = tychos.VectorDataStore(api_key="sk_a9adj...")
 ```
 
 Query live vector datasets
 ```python
-# initialize data store with API key
-data_store = tychos.VectorDataStore(api_key="sk_a9adji08...")
+# initialize data store
+data_store = tychos.VectorDataStore()
 
 # list available datasets
 datasets = data_store.list()
 
 # get name of the first dataset's id
 print(datasets['data'][0]['name'])
```

