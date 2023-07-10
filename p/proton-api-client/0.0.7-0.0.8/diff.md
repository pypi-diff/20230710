# Comparing `tmp/proton-api-client-0.0.7.tar.gz` & `tmp/proton-api-client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-api-client-0.0.7.tar", last modified: Mon Jun 26 19:17:44 2023, max compression
+gzip compressed data, was "proton-api-client-0.0.8.tar", last modified: Mon Jul 10 18:10:48 2023, max compression
```

## Comparing `proton-api-client-0.0.7.tar` & `proton-api-client-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/
--rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      922 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/proton/
--rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)     6208 2023-06-26 19:12:55.000000 proton-api-client-0.0.7/proton/client.py
--rw-r--r--   0 x         (1000) x         (1000)     2433 2023-06-26 19:15:08.000000 proton-api-client-0.0.7/proton/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     2035 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/helpers.py
--rw-r--r--   0 x         (1000) x         (1000)     2320 2023-06-26 19:12:23.000000 proton-api-client-0.0.7/proton/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/proton_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     1857 2023-06-26 19:15:08.000000 proton-api-client-0.0.7/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-10 18:10:48.766699 proton-api-client-0.0.8/
+-rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-25 17:48:35.000000 proton-api-client-0.0.8/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-07-10 18:10:48.766699 proton-api-client-0.0.8/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      922 2023-06-25 17:48:35.000000 proton-api-client-0.0.8/README.md
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-10 18:10:48.766699 proton-api-client-0.0.8/proton/
+-rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-25 17:48:35.000000 proton-api-client-0.0.8/proton/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-25 17:48:35.000000 proton-api-client-0.0.8/proton/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-25 17:48:35.000000 proton-api-client-0.0.8/proton/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     6208 2023-06-26 19:12:55.000000 proton-api-client-0.0.8/proton/client.py
+-rw-r--r--   0 x         (1000) x         (1000)     2433 2023-06-26 19:15:08.000000 proton-api-client-0.0.8/proton/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     2035 2023-06-25 17:48:35.000000 proton-api-client-0.0.8/proton/helpers.py
+-rw-r--r--   0 x         (1000) x         (1000)     2320 2023-06-26 19:12:23.000000 proton-api-client-0.0.8/proton/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-10 18:10:48.766699 proton-api-client-0.0.8/proton_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-07-10 18:10:48.000000 proton-api-client-0.0.8/proton_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      354 2023-07-10 18:10:48.000000 proton-api-client-0.0.8/proton_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-07-10 18:10:48.000000 proton-api-client-0.0.8/proton_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)      112 2023-07-10 18:10:48.000000 proton-api-client-0.0.8/proton_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        7 2023-07-10 18:10:48.000000 proton-api-client-0.0.8/proton_api_client.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-07-10 18:10:48.766699 proton-api-client-0.0.8/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     1887 2023-07-10 18:10:21.000000 proton-api-client-0.0.8/setup.py
```

### Comparing `proton-api-client-0.0.7/LICENSE` & `proton-api-client-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/PKG-INFO` & `proton-api-client-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `proton-api-client-0.0.7/README.md` & `proton-api-client-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/proton/_ctsrp.py` & `proton-api-client-0.0.8/proton/_ctsrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/proton/_pysrp.py` & `proton-api-client-0.0.8/proton/_pysrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/proton/client.py` & `proton-api-client-0.0.8/proton/client.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/proton/constants.py` & `proton-api-client-0.0.8/proton/constants.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/proton/helpers.py` & `proton-api-client-0.0.8/proton/helpers.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/proton/login.py` & `proton-api-client-0.0.8/proton/login.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.7/proton_api_client.egg-info/PKG-INFO` & `proton-api-client-0.0.8/proton_api_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `proton-api-client-0.0.7/setup.py` & `proton-api-client-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     'bcrypt',
     'python-gnupg',
     'pyopenssl',
     'selectolax',
     'orjson',
     'httpx',
     'tqdm',
-    'uvloop',
+    'uvloop; platform_system != "Windows"',
     'nest_asyncio',
 ]
 
 setup(
     name='proton-api-client',
-    version='0.0.7',
+    version='0.0.8',
     python_requires='>=3.10.10',
     description='Proton Mail API',
     long_description=dedent('''
     
     ### Proton Mail API
     
     #### Examples
```

