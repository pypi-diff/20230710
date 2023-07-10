# Comparing `tmp/sixth-python-0.1.4.tar.gz` & `tmp/sixth-python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-python-0.1.4.tar", last modified: Mon Jul 10 12:24:44 2023, max compression
+gzip compressed data, was "dist/sixth-python-0.1.5.tar", last modified: Mon Jul 10 13:05:25 2023, max compression
```

## Comparing `sixth-python-0.1.4.tar` & `sixth-python-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:24:44.000000 sixth-python-0.1.4/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 12:24:44.000000 sixth-python-0.1.4/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.4/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-10 12:24:44.000000 sixth-python-0.1.4/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-10 12:24:40.000000 sixth-python-0.1.4/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth/
--rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.4/sixth/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.4/sixth/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-10 11:42:02.000000 sixth-python-0.1.4/sixth/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.4/sixth/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-10 11:42:02.000000 sixth-python-0.1.4/sixth/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     7024 2023-07-10 12:10:24.000000 sixth-python-0.1.4/sixth/middlewares/six_rate_limiter_middleware.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth/pen_test/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.4/sixth/pen_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      143 2023-07-09 17:50:41.000000 sixth-python-0.1.4/sixth/pen_test/auto_pen_test.py
--rw-r--r--   0 mac        (501) staff       (20)      978 2023-07-10 11:22:10.000000 sixth-python-0.1.4/sixth/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     4246 2023-07-10 12:21:29.000000 sixth-python-0.1.4/sixth/sdk.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.4/sixth/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.4/sixth/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.4/sixth/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-10 12:24:44.000000 sixth-python-0.1.4/sixth_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 13:05:25.000000 sixth-python-0.1.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1899 2023-06-23 11:48:40.000000 sixth-python-0.1.5/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-10 13:05:25.000000 sixth-python-0.1.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3760 2023-07-10 13:05:20.000000 sixth-python-0.1.5/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/
+-rw-r--r--   0 mac        (501) staff       (20)       27 2023-06-23 22:29:11.000000 sixth-python-0.1.5/sixth/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-python-0.1.5/sixth/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3703 2023-07-10 11:42:02.000000 sixth-python-0.1.5/sixth/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-python-0.1.5/sixth/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3924 2023-07-10 11:42:02.000000 sixth-python-0.1.5/sixth/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     7024 2023-07-10 12:10:24.000000 sixth-python-0.1.5/sixth/middlewares/six_rate_limiter_middleware.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/pen_test/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-12 15:04:45.000000 sixth-python-0.1.5/sixth/pen_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      143 2023-07-09 17:50:41.000000 sixth-python-0.1.5/sixth/pen_test/auto_pen_test.py
+-rw-r--r--   0 mac        (501) staff       (20)      978 2023-07-10 11:22:10.000000 sixth-python-0.1.5/sixth/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     4246 2023-07-10 13:04:35.000000 sixth-python-0.1.5/sixth/sdk.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-python-0.1.5/sixth/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4254 2023-06-12 02:56:13.000000 sixth-python-0.1.5/sixth/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-python-0.1.5/sixth/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3101 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      604 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-07-10 13:05:25.000000 sixth-python-0.1.5/sixth_python.egg-info/top_level.txt
```

### Comparing `sixth-python-0.1.4/PKG-INFO` & `sixth-python-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.4/README.md` & `sixth-python-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/setup.py` & `sixth-python-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Sixth offical python package'
 LONG_DESCRIPTION = '''
 # **Sixth**
 
 
 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/test-103bf.appspot.com/o/waves.png?alt=media&token=0fa4c489-d9c9-4a3b-9178-593b2b018613)](https://nodesource.com/products/nsolid)
```

### Comparing `sixth-python-0.1.4/sixth/middlewares/encryption_middleware.py` & `sixth-python-0.1.5/sixth/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth/middlewares/six_base_http_middleware.py` & `sixth-python-0.1.5/sixth/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth/middlewares/six_independent_rate_limiter.py` & `sixth-python-0.1.5/sixth/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth/middlewares/six_rate_limiter_middleware.py` & `sixth-python-0.1.5/sixth/middlewares/six_rate_limiter_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth/schemas.py` & `sixth-python-0.1.5/sixth/schemas.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth/sdk.py` & `sixth-python-0.1.5/sixth/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,14 @@
             base_url = "project",
             last_updated=get_time_now(), 
             created_at=get_time_now(), 
             encryption_enabled=config.encryption_enabled if config != None else False, 
             rate_limiter_enabled=config.rate_limiter_enabled if config != None else True
         )
         _base_url = "https://backend.withsix.co"
-        _project_config_resp = requests.post(_base_url+"/project-config/config/sync-user-config", json=_config.json())
+        _project_config_resp = requests.post(_base_url+"/project-config/config/sync-user-config", json=_config.dict())
         if _project_config_resp.status_code == status.HTTP_200_OK:
             return _config
         else: 
             return _config
```

### Comparing `sixth-python-0.1.4/sixth/utils/encryption_utils.py` & `sixth-python-0.1.5/sixth/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth/utils/time_utils.py` & `sixth-python-0.1.5/sixth/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth_python.egg-info/PKG-INFO` & `sixth-python-0.1.5/sixth_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sixth offical python package
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: 
         # **Sixth**
```

### Comparing `sixth-python-0.1.4/sixth_python.egg-info/SOURCES.txt` & `sixth-python-0.1.5/sixth_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sixth-python-0.1.4/sixth_python.egg-info/requires.txt` & `sixth-python-0.1.5/sixth_python.egg-info/requires.txt`

 * *Files identical despite different names*

