# Comparing `tmp/seventv-2.3.2.tar.gz` & `tmp/seventv-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-2.3.2.tar", last modified: Sun Jul  9 21:15:01 2023, max compression
+gzip compressed data, was "seventv-2.3.3.tar", last modified: Sun Jul  9 22:01:50 2023, max compression
```

## Comparing `seventv-2.3.2.tar` & `seventv-2.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 21:14:48.000000 seventv-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 21:15:01.190548 seventv-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 21:14:48.000000 seventv-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 21:15:01.190548 seventv-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 21:14:48.000000 seventv-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 21:14:48.000000 seventv-2.3.2/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-09 21:14:48.000000 seventv-2.3.2/seventv/seventv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 21:15:01.000000 seventv-2.3.2/seventv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:15:01.190548 seventv-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-09 21:14:48.000000 seventv-2.3.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.054420 seventv-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 22:01:33.000000 seventv-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 22:01:50.054420 seventv-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 22:01:33.000000 seventv-2.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:01:50.054420 seventv-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 22:01:33.000000 seventv-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.050420 seventv-2.3.3/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 22:01:33.000000 seventv-2.3.3/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-09 22:01:33.000000 seventv-2.3.3/seventv/seventv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.050420 seventv-2.3.3/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.054420 seventv-2.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-09 22:01:33.000000 seventv-2.3.3/tests/test.py
```

### Comparing `seventv-2.3.2/LICENSE` & `seventv-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-2.3.2/PKG-INFO` & `seventv-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.3.2
+Version: 2.3.3
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `seventv-2.3.2/README.md` & `seventv-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `seventv-2.3.2/setup.py` & `seventv-2.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version="2.3.2",
+    version="2.3.3",
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     long_description = """
         An asynchronous Python API-wrapper for 7tv.app. 
         It makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
         To get emotes by search query, the wrapper uses the GraphQL endpoint
```

### Comparing `seventv-2.3.2/seventv/seventv.py` & `seventv-2.3.3/seventv/seventv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-import aiohttp, json
+import aiohttp
 from typing import Literal
 
 class Emote:
     def __init__(self, id = None, name = None, owner_username = None, host_url = None):
         self.id = id
         self.name = name
         self.owner_username = owner_username
@@ -70,15 +70,15 @@
         }
         headers = {
             "Content-Type": "application/json"
         }
         payload = {
             "operationName": "SearchEmotes",
             "variables": {
-                "query": json.dumps(searchterm),
+                "query": searchterm,
                 "limit": limit,
                 "page": page,
                 "sort": {
                     "value": "popularity",
                     "order": "DESCENDING"
                 },
                 "filter": {
@@ -92,13 +92,10 @@
                 }
             },
             "query": f"{queries.get(query)}"
         }
         async with self.session.post(url, json=payload, headers=headers) as response:
             response_data = await response.json()
             if response_data.get('errors', {}):
-                raise seventvException(response_data.get('errors', {})[0].get('message', {}))
+                raise Exception(response_data.get('errors', {})[0].get('message', {}))
             emote_objects = create_emote_objects(response_data)
-            return emote_objects
-
-class seventvException(Exception):
-        pass
+            return emote_objects
```

### Comparing `seventv-2.3.2/seventv.egg-info/PKG-INFO` & `seventv-2.3.3/seventv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.3.2
+Version: 2.3.3
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

