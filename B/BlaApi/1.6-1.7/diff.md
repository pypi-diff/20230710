# Comparing `tmp/BlaApi-1.6.tar.gz` & `tmp/BlaApi-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlaApi-1.6.tar", last modified: Sun Jul  9 14:31:05 2023, max compression
+gzip compressed data, was "BlaApi-1.7.tar", last modified: Mon Jul 10 13:04:20 2023, max compression
```

## Comparing `BlaApi-1.6.tar` & `BlaApi-1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-09 14:31:05.427710 BlaApi-1.6/
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-09 14:31:05.422710 BlaApi-1.6/BlaApi/
--rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.6/BlaApi/__init__.py
--rw-r--r--   0 muddi     (1000) muddi     (1001)     8018 2023-07-09 14:29:50.000000 BlaApi-1.6/BlaApi/client.py
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-09 14:31:05.425710 BlaApi-1.6/BlaApi.egg-info/
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-07-09 14:31:05.000000 BlaApi-1.6/BlaApi.egg-info/SOURCES.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/dependency_links.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)       21 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/requires.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-07-09 14:31:04.000000 BlaApi-1.6/BlaApi.egg-info/top_level.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.6/LICENSE
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-09 14:31:05.426710 BlaApi-1.6/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.6/README.md
--rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-07-09 14:31:05.427710 BlaApi-1.6/setup.cfg
--rw-r--r--   0 muddi     (1000) muddi     (1001)     3583 2023-07-09 14:30:21.000000 BlaApi-1.6/setup.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-10 13:04:20.627675 BlaApi-1.7/
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-10 13:04:20.619675 BlaApi-1.7/BlaApi/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.7/BlaApi/__init__.py
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     8185 2023-07-10 13:03:41.000000 BlaApi-1.7/BlaApi/client.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-10 13:04:20.624675 BlaApi-1.7/BlaApi.egg-info/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/SOURCES.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/dependency_links.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       31 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/requires.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-07-10 13:04:19.000000 BlaApi-1.7/BlaApi.egg-info/top_level.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.7/LICENSE
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-10 13:04:20.626675 BlaApi-1.7/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.7/README.md
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-07-10 13:04:20.627675 BlaApi-1.7/setup.cfg
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     3594 2023-07-10 12:46:26.000000 BlaApi-1.7/setup.py
```

### Comparing `BlaApi-1.6/BlaApi/client.py` & `BlaApi-1.7/BlaApi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import json
 import httpx
 from fake_useragent import UserAgent as ua
+from html2text import html2text as h2t
 import re
 
 class Client:
     client = httpx.Client(verify=False) # instanciate 
     #! BLA credentials must be passed in as string
     def __init__(self, username: str, password: str):
         # Random UserAgent
@@ -109,14 +110,17 @@
             
             # error handling
             if json.loads(response.content).get('success') == False:
                 raise ValueError(json.loads(response.content).get('error'))
             
             # Retrieve diary data from JSON response
             data = json.loads(response.content)['data']
+            # parse diary details by converting to markdown
+            data['details'] = h2t(data.get('details'))
+            
             output.append(data)
 
         return output
     
     def search_by_student(self, passthru=None, student_id=None):
 
         diary = self.get_diary_list()
```

### Comparing `BlaApi-1.6/BlaApi.egg-info/PKG-INFO` & `BlaApi-1.7/BlaApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.6
+Version: 1.7
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.6/LICENSE` & `BlaApi-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BlaApi-1.6/PKG-INFO` & `BlaApi-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.6
+Version: 1.7
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.6/README.md` & `BlaApi-1.7/README.md`

 * *Files identical despite different names*

### Comparing `BlaApi-1.6/setup.py` & `BlaApi-1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 # Package meta-data.
 NAME = 'BlaApi'
 DESCRIPTION = 'A wrapper for the beacon light api.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'deaddogfuneral@gmail.com'
 AUTHOR = 'Omer-Farooqui'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.6'
+VERSION = '1.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-     'httpx', 'fake_useragent',
+     'httpx', 'fake_useragent','html2text'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

