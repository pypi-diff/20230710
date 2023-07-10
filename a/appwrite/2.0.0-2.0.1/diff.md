# Comparing `tmp/appwrite-2.0.0.tar.gz` & `tmp/appwrite-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appwrite-2.0.0.tar", last modified: Wed Apr 12 10:01:29 2023, max compression
+gzip compressed data, was "appwrite-2.0.1.tar", last modified: Mon Jul 10 15:17:43 2023, max compression
```

## Comparing `appwrite-2.0.0.tar` & `appwrite-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.126136 appwrite-2.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2023-04-12 10:01:09.000000 appwrite-2.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-04-12 10:01:29.126136 appwrite-2.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4238 2023-04-12 10:01:09.000000 appwrite-2.0.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.122136 appwrite-2.0.0/appwrite/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6745 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/id.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      593 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/input_file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/permission.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.126136 appwrite-2.0.0/appwrite/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8488 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/avatars.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39693 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/databases.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12818 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      996 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/graphql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/health.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1875 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/locale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9352 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/storage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7733 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/teams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16087 2023-04-12 10:01:09.000000 appwrite-2.0.0/appwrite/services/users.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-12 10:01:29.122136 appwrite-2.0.0/appwrite.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      691 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-04-12 10:01:29.000000 appwrite-2.0.0/appwrite.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-04-12 10:01:29.126136 appwrite-2.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2023-04-12 10:01:09.000000 appwrite-2.0.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.249048 appwrite-2.0.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2023-07-10 15:16:52.000000 appwrite-2.0.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-07-10 15:17:43.249048 appwrite-2.0.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4238 2023-07-10 15:16:52.000000 appwrite-2.0.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.245049 appwrite-2.0.1/appwrite/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6983 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      128 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/id.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      593 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/input_file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/permission.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/role.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/service.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.249048 appwrite-2.0.1/appwrite/services/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8488 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/avatars.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38739 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/databases.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12818 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      996 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/graphql.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/health.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1875 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/locale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9352 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7733 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/teams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16087 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/users.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.249048 appwrite-2.0.1/appwrite.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      691 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-07-10 15:17:43.249048 appwrite-2.0.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2023-07-10 15:16:52.000000 appwrite-2.0.1/setup.py
```

### Comparing `appwrite-2.0.0/LICENSE` & `appwrite-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/PKG-INFO` & `appwrite-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 2.0.0
+Version: 2.0.1
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.0.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.1.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.3.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.3.2-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
 **This SDK is compatible with Appwrite server version 1.3.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
```

### Comparing `appwrite-2.0.0/README.md` & `appwrite-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.3.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.3.2-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
 **This SDK is compatible with Appwrite server version 1.3.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
```

### Comparing `appwrite-2.0.0/appwrite/client.py` & `appwrite-2.0.1/appwrite/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 class Client:
     def __init__(self):
         self._chunk_size = 5*1024*1024
         self._self_signed = False
         self._endpoint = 'https://HOSTNAME/v1'
         self._global_headers = {
             'content-type': '',
+            'user-agent' : 'AppwritePythonSDK/2.0.1 (${os.uname().sysname}; ${os.uname().version}; ${os.uname().machine})',
             'x-sdk-name': 'Python',
             'x-sdk-platform': 'server',
             'x-sdk-language': 'python',
-            'x-sdk-version': '2.0.0',
+            'x-sdk-version': '2.0.1',
             'X-Appwrite-Response-Format' : '1.0.0',
         }
 
     def set_self_signed(self, status=True):
         self._self_signed = status
         return self
 
@@ -55,14 +56,16 @@
     def call(self, method, path='', headers=None, params=None):
         if headers is None:
             headers = {}
 
         if params is None:
             params = {}
 
+        params = {k: v for k, v in params.items() if v is not None}  # Remove None values from params dictionary
+
         data = {}
         json = {}
         files = {}
         stringify = False
         
         headers = {**self._global_headers, **headers}
```

### Comparing `appwrite-2.0.0/appwrite/input_file.py` & `appwrite-2.0.1/appwrite/input_file.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/query.py` & `appwrite-2.0.1/appwrite/query.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/role.py` & `appwrite-2.0.1/appwrite/role.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/account.py` & `appwrite-2.0.1/appwrite/services/account.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/avatars.py` & `appwrite-2.0.1/appwrite/services/avatars.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/databases.py` & `appwrite-2.0.1/appwrite/services/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,17 +267,14 @@
 
         if key is None:
             raise AppwriteException('Missing required parameter: "key"')
 
         if required is None:
             raise AppwriteException('Missing required parameter: "required"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['default'] = default
 
@@ -329,17 +326,14 @@
 
         if key is None:
             raise AppwriteException('Missing required parameter: "key"')
 
         if required is None:
             raise AppwriteException('Missing required parameter: "required"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['default'] = default
 
@@ -391,17 +385,14 @@
 
         if key is None:
             raise AppwriteException('Missing required parameter: "key"')
 
         if required is None:
             raise AppwriteException('Missing required parameter: "required"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['default'] = default
 
@@ -460,17 +451,14 @@
 
         if elements is None:
             raise AppwriteException('Missing required parameter: "elements"')
 
         if required is None:
             raise AppwriteException('Missing required parameter: "required"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['elements'] = elements
         params['required'] = required
         params['default'] = default
@@ -531,17 +519,14 @@
 
         if min is None:
             raise AppwriteException('Missing required parameter: "min"')
 
         if max is None:
             raise AppwriteException('Missing required parameter: "max"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['min'] = min
         params['max'] = max
@@ -603,17 +588,14 @@
 
         if min is None:
             raise AppwriteException('Missing required parameter: "min"')
 
         if max is None:
             raise AppwriteException('Missing required parameter: "max"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['min'] = min
         params['max'] = max
@@ -667,17 +649,14 @@
 
         if key is None:
             raise AppwriteException('Missing required parameter: "key"')
 
         if required is None:
             raise AppwriteException('Missing required parameter: "required"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['default'] = default
 
@@ -765,17 +744,14 @@
 
         if key is None:
             raise AppwriteException('Missing required parameter: "key"')
 
         if required is None:
             raise AppwriteException('Missing required parameter: "required"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['default'] = default
 
@@ -827,17 +803,14 @@
 
         if key is None:
             raise AppwriteException('Missing required parameter: "key"')
 
         if required is None:
             raise AppwriteException('Missing required parameter: "required"')
 
-        if default is None:
-            raise AppwriteException('Missing required parameter: "default"')
-
         path = path.replace('{databaseId}', database_id)
         path = path.replace('{collectionId}', collection_id)
         path = path.replace('{key}', key)
 
         params['required'] = required
         params['default'] = default
```

### Comparing `appwrite-2.0.0/appwrite/services/functions.py` & `appwrite-2.0.1/appwrite/services/functions.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/graphql.py` & `appwrite-2.0.1/appwrite/services/graphql.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/health.py` & `appwrite-2.0.1/appwrite/services/health.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/locale.py` & `appwrite-2.0.1/appwrite/services/locale.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/storage.py` & `appwrite-2.0.1/appwrite/services/storage.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/teams.py` & `appwrite-2.0.1/appwrite/services/teams.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite/services/users.py` & `appwrite-2.0.1/appwrite/services/users.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/appwrite.egg-info/PKG-INFO` & `appwrite-2.0.1/appwrite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 2.0.0
+Version: 2.0.1
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.0.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.1.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.3.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.3.2-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
 **This SDK is compatible with Appwrite server version 1.3.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
```

### Comparing `appwrite-2.0.0/appwrite.egg-info/SOURCES.txt` & `appwrite-2.0.1/appwrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.0/setup.py` & `appwrite-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 with open("README.md", "r", encoding="utf-8") as readme_file_desc:
     long_description = readme_file_desc.read()
     
 setuptools.setup(
   name = 'appwrite',
   packages = ['appwrite', 'appwrite/services'],
-  version = '2.0.0',
+  version = '2.0.1',
   license='BSD-3-Clause',
   description = 'Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Appwrite Team',
   author_email = 'team@appwrite.io',
   maintainer = 'Appwrite Team',
   maintainer_email = 'team@appwrite.io',
   url = 'https://appwrite.io/support',
-  download_url='https://github.com/appwrite/sdk-for-python/archive/2.0.0.tar.gz',
+  download_url='https://github.com/appwrite/sdk-for-python/archive/2.0.1.tar.gz',
   # keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],
   install_requires=[
           'requests',
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
```

