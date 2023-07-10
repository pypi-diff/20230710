# Comparing `tmp/rocketapi-1.0.4.tar.gz` & `tmp/rocketapi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketapi-1.0.4.tar", last modified: Wed May 24 22:15:25 2023, max compression
+gzip compressed data, was "rocketapi-1.0.5.tar", last modified: Mon Jul 10 17:44:03 2023, max compression
```

## Comparing `rocketapi-1.0.4.tar` & `rocketapi-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-05-24 22:15:25.005781 rocketapi-1.0.4/
--rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-05-24 22:15:25.005649 rocketapi-1.0.4/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      317 2022-11-20 19:09:53.000000 rocketapi-1.0.4/README.md
--rw-r--r--   0 sobolev    (501) staff       (20)      792 2023-01-03 14:37:32.000000 rocketapi-1.0.4/pyproject.toml
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-05-24 22:15:25.004673 rocketapi-1.0.4/rocketapi/
--rw-r--r--   0 sobolev    (501) staff       (20)       39 2022-10-08 15:10:45.000000 rocketapi-1.0.4/rocketapi/__init__.py
--rw-r--r--   0 sobolev    (501) staff       (20)       95 2022-10-08 15:05:42.000000 rocketapi-1.0.4/rocketapi/exceptions.py
--rw-r--r--   0 sobolev    (501) staff       (20)    18792 2023-05-24 22:14:25.000000 rocketapi-1.0.4/rocketapi/instagramapi.py
--rw-r--r--   0 sobolev    (501) staff       (20)      759 2023-04-17 13:26:36.000000 rocketapi-1.0.4/rocketapi/rocketapi.py
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-05-24 22:15:25.005459 rocketapi-1.0.4/rocketapi.egg-info/
--rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      292 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/SOURCES.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/dependency_links.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        9 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/requires.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/top_level.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-05-24 22:15:25.005898 rocketapi-1.0.4/setup.cfg
--rw-r--r--   0 sobolev    (501) staff       (20)      414 2023-05-24 22:15:11.000000 rocketapi-1.0.4/setup.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-10 17:44:03.293540 rocketapi-1.0.5/
+-rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-07-10 17:44:03.293427 rocketapi-1.0.5/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      317 2022-11-20 19:09:53.000000 rocketapi-1.0.5/README.md
+-rw-r--r--   0 sobolev    (501) staff       (20)      792 2023-01-03 14:37:32.000000 rocketapi-1.0.5/pyproject.toml
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-10 17:44:03.292745 rocketapi-1.0.5/rocketapi/
+-rw-r--r--   0 sobolev    (501) staff       (20)       74 2023-07-10 17:40:18.000000 rocketapi-1.0.5/rocketapi/__init__.py
+-rw-r--r--   0 sobolev    (501) staff       (20)       95 2022-10-08 15:05:42.000000 rocketapi-1.0.5/rocketapi/exceptions.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    18637 2023-07-10 17:32:21.000000 rocketapi-1.0.5/rocketapi/instagramapi.py
+-rw-r--r--   0 sobolev    (501) staff       (20)      677 2023-07-10 17:32:35.000000 rocketapi-1.0.5/rocketapi/rocketapi.py
+-rw-r--r--   0 sobolev    (501) staff       (20)     6652 2023-07-10 17:39:38.000000 rocketapi-1.0.5/rocketapi/threadsapi.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-07-10 17:44:03.293261 rocketapi-1.0.5/rocketapi.egg-info/
+-rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-07-10 17:44:03.000000 rocketapi-1.0.5/rocketapi.egg-info/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      316 2023-07-10 17:44:03.000000 rocketapi-1.0.5/rocketapi.egg-info/SOURCES.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-07-10 17:44:03.000000 rocketapi-1.0.5/rocketapi.egg-info/dependency_links.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        9 2023-07-10 17:44:03.000000 rocketapi-1.0.5/rocketapi.egg-info/requires.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-07-10 17:44:03.000000 rocketapi-1.0.5/rocketapi.egg-info/top_level.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-07-10 17:44:03.293639 rocketapi-1.0.5/setup.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)      414 2023-07-10 17:28:19.000000 rocketapi-1.0.5/setup.py
```

### Comparing `rocketapi-1.0.4/pyproject.toml` & `rocketapi-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rocketapi-1.0.4/rocketapi/instagramapi.py` & `rocketapi-1.0.5/rocketapi/instagramapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from rocketapi.exceptions import NotFoundException, BadResponseException
 from rocketapi.rocketapi import RocketAPI
 
 
 class InstagramAPI(RocketAPI):
-    def __init__(self, token, threads=1, max_timeout=30):
+    def __init__(self, token, max_timeout=30):
         """
         Instagram API client.
 
         Args:
             token (str): Your RocketAPI token (https://rocketapi.io/dashboard/)
-            threads (int): Number of threads to use for requests (it's beta, use with caution, every thread charges 1 request)
             max_timeout (int): Maximum timeout for requests. Please, don't use values lower than 15 seconds, it may cause problems with API.
 
         For debugging purposes you can use the following variables:
             last_response (dict): contains the last response from the API.
             counter (int): contains the number of requests made in the current session.
 
         For more information, see documentation: https://docs.rocketapi.io/api/
         """
         self.last_response = None
         self.counter = 0
-        super().__init__(token, threads=threads, max_timeout=max_timeout)
+        super().__init__(token, max_timeout=max_timeout)
 
     def request(self, method, data):
         response = super().request(method, data)
         self.last_response = response
         self.counter += 1
         if response["status"] == "done":
             if (
```

### Comparing `rocketapi-1.0.4/rocketapi/rocketapi.py` & `rocketapi-1.0.5/rocketapi/rocketapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import requests
 
 
 class RocketAPI:
-    def __init__(self, token, threads=1, max_timeout=30):
+    def __init__(self, token, max_timeout=30):
         """
         RocketAPI client.
 
         If your base_url is different from the default, you can reassign it after initialization.
 
         For more information, see documentation: https://docs.rocketapi.io/api/
         """
         self.base_url = "https://v1.rocketapi.io/"
         self.token = token
-        self.threads = threads
         self.max_timeout = max_timeout
 
     def request(self, method, data):
-        data["_threads"] = self.threads
         return requests.post(
             url=self.base_url + method,
             json=data,
             headers={"Authorization": f"Token {self.token}"},
             timeout=self.max_timeout,
         ).json()
```

