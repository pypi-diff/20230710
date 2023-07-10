# Comparing `tmp/appwrite-2.0.1.tar.gz` & `tmp/appwrite-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appwrite-2.0.1.tar", last modified: Mon Jul 10 15:17:43 2023, max compression
+gzip compressed data, was "appwrite-2.0.2.tar", last modified: Mon Jul 10 17:41:05 2023, max compression
```

## Comparing `appwrite-2.0.1.tar` & `appwrite-2.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.249048 appwrite-2.0.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2023-07-10 15:16:52.000000 appwrite-2.0.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-07-10 15:17:43.249048 appwrite-2.0.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4238 2023-07-10 15:16:52.000000 appwrite-2.0.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.245049 appwrite-2.0.1/appwrite/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6983 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/id.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      593 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/input_file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/permission.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.249048 appwrite-2.0.1/appwrite/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8488 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/avatars.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38739 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/databases.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12818 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      996 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/graphql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/health.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1875 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/locale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9352 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/storage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7733 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/teams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16087 2023-07-10 15:16:52.000000 appwrite-2.0.1/appwrite/services/users.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 15:17:43.249048 appwrite-2.0.1/appwrite.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      691 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-07-10 15:17:43.000000 appwrite-2.0.1/appwrite.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-07-10 15:17:43.249048 appwrite-2.0.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2023-07-10 15:16:52.000000 appwrite-2.0.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 17:41:05.526069 appwrite-2.0.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2023-07-10 17:40:17.000000 appwrite-2.0.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-07-10 17:41:05.526069 appwrite-2.0.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4238 2023-07-10 17:40:17.000000 appwrite-2.0.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 17:41:05.522069 appwrite-2.0.2/appwrite/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6983 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      128 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/id.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      593 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/input_file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/permission.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/role.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/service.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 17:41:05.526069 appwrite-2.0.2/appwrite/services/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8488 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3590 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/avatars.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38739 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/databases.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12818 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      996 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/graphql.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/health.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1875 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/locale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9352 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7733 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/teams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16087 2023-07-10 17:40:17.000000 appwrite-2.0.2/appwrite/services/users.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-10 17:41:05.522069 appwrite-2.0.2/appwrite.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5251 2023-07-10 17:41:05.000000 appwrite-2.0.2/appwrite.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      691 2023-07-10 17:41:05.000000 appwrite-2.0.2/appwrite.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-10 17:41:05.000000 appwrite-2.0.2/appwrite.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-07-10 17:41:05.000000 appwrite-2.0.2/appwrite.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-07-10 17:41:05.000000 appwrite-2.0.2/appwrite.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2023-07-10 17:41:05.526069 appwrite-2.0.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2023-07-10 17:40:17.000000 appwrite-2.0.2/setup.py
```

### Comparing `appwrite-2.0.1/LICENSE` & `appwrite-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/PKG-INFO` & `appwrite-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 2.0.1
+Version: 2.0.2
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.1.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.2.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `appwrite-2.0.1/README.md` & `appwrite-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/client.py` & `appwrite-2.0.2/appwrite/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 class Client:
     def __init__(self):
         self._chunk_size = 5*1024*1024
         self._self_signed = False
         self._endpoint = 'https://HOSTNAME/v1'
         self._global_headers = {
             'content-type': '',
-            'user-agent' : 'AppwritePythonSDK/2.0.1 (${os.uname().sysname}; ${os.uname().version}; ${os.uname().machine})',
+            'user-agent' : 'AppwritePythonSDK/2.0.2 (${os.uname().sysname}; ${os.uname().version}; ${os.uname().machine})',
             'x-sdk-name': 'Python',
             'x-sdk-platform': 'server',
             'x-sdk-language': 'python',
-            'x-sdk-version': '2.0.1',
+            'x-sdk-version': '2.0.2',
             'X-Appwrite-Response-Format' : '1.0.0',
         }
 
     def set_self_signed(self, status=True):
         self._self_signed = status
         return self
```

### Comparing `appwrite-2.0.1/appwrite/input_file.py` & `appwrite-2.0.2/appwrite/input_file.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/query.py` & `appwrite-2.0.2/appwrite/query.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/role.py` & `appwrite-2.0.2/appwrite/role.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/account.py` & `appwrite-2.0.2/appwrite/services/account.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/avatars.py` & `appwrite-2.0.2/appwrite/services/avatars.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/databases.py` & `appwrite-2.0.2/appwrite/services/databases.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/functions.py` & `appwrite-2.0.2/appwrite/services/functions.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/graphql.py` & `appwrite-2.0.2/appwrite/services/graphql.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/health.py` & `appwrite-2.0.2/appwrite/services/health.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/locale.py` & `appwrite-2.0.2/appwrite/services/locale.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/storage.py` & `appwrite-2.0.2/appwrite/services/storage.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/teams.py` & `appwrite-2.0.2/appwrite/services/teams.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite/services/users.py` & `appwrite-2.0.2/appwrite/services/users.py`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/appwrite.egg-info/PKG-INFO` & `appwrite-2.0.2/appwrite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 2.0.1
+Version: 2.0.2
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.1.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/2.0.2.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `appwrite-2.0.1/appwrite.egg-info/SOURCES.txt` & `appwrite-2.0.2/appwrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appwrite-2.0.1/setup.py` & `appwrite-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 with open("README.md", "r", encoding="utf-8") as readme_file_desc:
     long_description = readme_file_desc.read()
     
 setuptools.setup(
   name = 'appwrite',
   packages = ['appwrite', 'appwrite/services'],
-  version = '2.0.1',
+  version = '2.0.2',
   license='BSD-3-Clause',
   description = 'Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Appwrite Team',
   author_email = 'team@appwrite.io',
   maintainer = 'Appwrite Team',
   maintainer_email = 'team@appwrite.io',
   url = 'https://appwrite.io/support',
-  download_url='https://github.com/appwrite/sdk-for-python/archive/2.0.1.tar.gz',
+  download_url='https://github.com/appwrite/sdk-for-python/archive/2.0.2.tar.gz',
   # keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],
   install_requires=[
           'requests',
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
```

