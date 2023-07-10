# Comparing `tmp/seventv-2.3.3.tar.gz` & `tmp/seventv-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seventv-2.3.3.tar", last modified: Sun Jul  9 22:01:50 2023, max compression
+gzip compressed data, was "seventv-2.4.0.tar", last modified: Mon Jul 10 09:27:06 2023, max compression
```

## Comparing `seventv-2.3.3.tar` & `seventv-2.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.054420 seventv-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-09 22:01:33.000000 seventv-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 22:01:50.054420 seventv-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-09 22:01:33.000000 seventv-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:01:50.054420 seventv-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 22:01:33.000000 seventv-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.050420 seventv-2.3.3/seventv/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 22:01:33.000000 seventv-2.3.3/seventv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-09 22:01:33.000000 seventv-2.3.3/seventv/seventv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.050420 seventv-2.3.3/seventv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 22:01:50.000000 seventv-2.3.3/seventv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:01:50.054420 seventv-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-09 22:01:33.000000 seventv-2.3.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:27:06.891659 seventv-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-07-10 09:26:53.000000 seventv-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-10 09:27:06.891659 seventv-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-10 09:26:53.000000 seventv-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:27:06.891659 seventv-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-10 09:26:53.000000 seventv-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:27:06.891659 seventv-2.4.0/seventv/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-10 09:26:53.000000 seventv-2.4.0/seventv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-10 09:26:53.000000 seventv-2.4.0/seventv/seventv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:27:06.891659 seventv-2.4.0/seventv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-10 09:27:06.000000 seventv-2.4.0/seventv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-10 09:27:06.000000 seventv-2.4.0/seventv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:27:06.000000 seventv-2.4.0/seventv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 09:27:06.000000 seventv-2.4.0/seventv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 09:27:06.000000 seventv-2.4.0/seventv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:27:06.891659 seventv-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-10 09:26:53.000000 seventv-2.4.0/tests/test.py
```

### Comparing `seventv-2.3.3/LICENSE` & `seventv-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seventv-2.3.3/PKG-INFO` & `seventv-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.3.3
+Version: 2.4.0
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `seventv-2.3.3/README.md` & `seventv-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# seventv
-an asynchronous Python API-wrapper for [7tv.app](https://7tv.app)
+# seventv - an asynchronous Python API-wrapper for 7tv
+[7tv.app](https://7tv.app)
 
 This API-wrapper makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
 
 To get emotes by search query, the wrapper uses the GraphQL endpoint ```https://7tv.io/v3/gql``` because it seems to currently be the only working one for searching emotes. 
 
 <sub>this project is not associated with or owned by 7tv or it's developers<sub>
```

### Comparing `seventv-2.3.3/setup.py` & `seventv-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='seventv',
-    version="2.3.3",
+    version="2.4.0",
     author='Jässin Aouani',
     author_email='jassin@aouani.de',
     description='An asynchronous API-wrapper for 7tv.app',
     long_description = """
         An asynchronous Python API-wrapper for 7tv.app. 
         It makes use of the 7tv API (v3) to make it possible to get emotes, details about them, and soon some more things the API supports.
         To get emotes by search query, the wrapper uses the GraphQL endpoint
```

### Comparing `seventv-2.3.3/seventv/seventv.py` & `seventv-2.4.0/seventv/seventv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import aiohttp
 from typing import Literal
+import re
 
 class Emote:
     def __init__(self, id = None, name = None, owner_username = None, host_url = None):
         self.id = id
         self.name = name
         self.owner_username = owner_username
         self.host_url = host_url
@@ -92,10 +93,15 @@
                 }
             },
             "query": f"{queries.get(query)}"
         }
         async with self.session.post(url, json=payload, headers=headers) as response:
             response_data = await response.json()
             if response_data.get('errors', {}):
-                raise Exception(response_data.get('errors', {})[0].get('message', {}))
+                raise seventvException(response_data.get('errors', {})[0].get('message', {}))
             emote_objects = create_emote_objects(response_data)
-            return emote_objects
+            return emote_objects
+
+class seventvException(Exception):
+    def __init__(self, message):
+        self.message = message
+        super().__init__(f"That didn't work!\n{message}")
```

### Comparing `seventv-2.3.3/seventv.egg-info/PKG-INFO` & `seventv-2.4.0/seventv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seventv
-Version: 2.3.3
+Version: 2.4.0
 Summary: An asynchronous API-wrapper for 7tv.app
 Home-page: https://github.com/probablyjassin/seventv.py
 Author: Jässin Aouani
 Author-email: jassin@aouani.de
 License: GPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

