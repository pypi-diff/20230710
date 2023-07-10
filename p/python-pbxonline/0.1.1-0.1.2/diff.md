# Comparing `tmp/python-pbxonline-0.1.1.tar.gz` & `tmp/python-pbxonline-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pbxonline-0.1.1.tar", last modified: Mon Jul 10 11:03:38 2023, max compression
+gzip compressed data, was "python-pbxonline-0.1.2.tar", last modified: Mon Jul 10 13:01:35 2023, max compression
```

## Comparing `python-pbxonline-0.1.1.tar` & `python-pbxonline-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.196246 python-pbxonline-0.1.1/
--rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      798 2023-07-10 11:03:38.197244 python-pbxonline-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.152087 python-pbxonline-0.1.1/pbxonline/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/__init__.py
--rw-rw-rw-   0        0        0     7780 2023-07-10 10:42:39.000000 python-pbxonline-0.1.1/pbxonline/api.py
--rw-rw-rw-   0        0        0     3451 2023-07-07 09:09:45.000000 python-pbxonline-0.1.1/pbxonline/auth_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.154087 python-pbxonline-0.1.1/pbxonline/cache/
--rw-rw-rw-   0        0        0        0 2023-04-24 08:42:27.000000 python-pbxonline-0.1.1/pbxonline/cache/__init__.py
--rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.1.1/pbxonline/cache_handler.py
--rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.1.1/pbxonline/config.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.158088 python-pbxonline-0.1.1/pbxonline/constants/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/constants/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.1.1/pbxonline/constants/constants.py
--rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/constants/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.166085 python-pbxonline-0.1.1/pbxonline/endpoints/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-07-07 11:31:06.000000 python-pbxonline-0.1.1/pbxonline/endpoints/action.py
--rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.1.1/pbxonline/endpoints/base.py
--rw-rw-rw-   0        0        0      658 2023-07-07 12:11:14.000000 python-pbxonline-0.1.1/pbxonline/endpoints/pbx.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.173326 python-pbxonline-0.1.1/pbxonline/models/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/models/__init__.py
--rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.1.1/pbxonline/models/base.py
--rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.1.1/pbxonline/models/errors.py
--rw-rw-rw-   0        0        0     2372 2023-07-07 11:24:25.000000 python-pbxonline-0.1.1/pbxonline/models/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.186989 python-pbxonline-0.1.1/python_pbxonline.egg-info/
--rw-rw-rw-   0        0        0      798 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-10 11:03:38.200318 python-pbxonline-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1269 2023-07-10 11:03:31.000000 python-pbxonline-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.195244 python-pbxonline-0.1.1/tests/
--rw-rw-rw-   0        0        0      538 2023-07-07 11:31:21.000000 python-pbxonline-0.1.1/tests/test_action.py
--rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.1.1/tests/test_auth.py
--rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.1.1/tests/test_pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.134664 python-pbxonline-0.1.2/
+-rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      798 2023-07-10 13:01:35.134664 python-pbxonline-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.093620 python-pbxonline-0.1.2/pbxonline/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.2/pbxonline/__init__.py
+-rw-rw-rw-   0        0        0     7780 2023-07-10 10:42:39.000000 python-pbxonline-0.1.2/pbxonline/api.py
+-rw-rw-rw-   0        0        0     3451 2023-07-07 09:09:45.000000 python-pbxonline-0.1.2/pbxonline/auth_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.093620 python-pbxonline-0.1.2/pbxonline/cache/
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:42:27.000000 python-pbxonline-0.1.2/pbxonline/cache/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.1.2/pbxonline/cache_handler.py
+-rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.1.2/pbxonline/config.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.097725 python-pbxonline-0.1.2/pbxonline/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.2/pbxonline/constants/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.1.2/pbxonline/constants/constants.py
+-rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.1.2/pbxonline/constants/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.102460 python-pbxonline-0.1.2/pbxonline/endpoints/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.2/pbxonline/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-07-07 11:31:06.000000 python-pbxonline-0.1.2/pbxonline/endpoints/action.py
+-rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.1.2/pbxonline/endpoints/base.py
+-rw-rw-rw-   0        0        0      658 2023-07-07 12:11:14.000000 python-pbxonline-0.1.2/pbxonline/endpoints/pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.107463 python-pbxonline-0.1.2/pbxonline/models/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.2/pbxonline/models/__init__.py
+-rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.1.2/pbxonline/models/base.py
+-rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.1.2/pbxonline/models/errors.py
+-rw-rw-rw-   0        0        0     2484 2023-07-10 13:01:28.000000 python-pbxonline-0.1.2/pbxonline/models/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.130818 python-pbxonline-0.1.2/python_pbxonline.egg-info/
+-rw-rw-rw-   0        0        0      798 2023-07-10 13:01:34.000000 python-pbxonline-0.1.2/python_pbxonline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-07-10 13:01:35.000000 python-pbxonline-0.1.2/python_pbxonline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:01:34.000000 python-pbxonline-0.1.2/python_pbxonline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-10 13:01:34.000000 python-pbxonline-0.1.2/python_pbxonline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 13:01:34.000000 python-pbxonline-0.1.2/python_pbxonline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-10 13:01:35.142451 python-pbxonline-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2023-07-10 13:01:28.000000 python-pbxonline-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:01:35.134664 python-pbxonline-0.1.2/tests/
+-rw-rw-rw-   0        0        0      538 2023-07-10 11:20:00.000000 python-pbxonline-0.1.2/tests/test_action.py
+-rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.1.2/tests/test_auth.py
+-rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.1.2/tests/test_pbx.py
```

### Comparing `python-pbxonline-0.1.1/LICENSE.txt` & `python-pbxonline-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/PKG-INFO` & `python-pbxonline-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.2.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.1.1/pbxonline/api.py` & `python-pbxonline-0.1.2/pbxonline/api.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/pbxonline/auth_handler.py` & `python-pbxonline-0.1.2/pbxonline/auth_handler.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/pbxonline/cache_handler.py` & `python-pbxonline-0.1.2/pbxonline/cache_handler.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/pbxonline/endpoints/action.py` & `python-pbxonline-0.1.2/pbxonline/endpoints/action.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/pbxonline/endpoints/pbx.py` & `python-pbxonline-0.1.2/pbxonline/endpoints/pbx.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/pbxonline/models/base.py` & `python-pbxonline-0.1.2/pbxonline/models/base.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/pbxonline/models/utils.py` & `python-pbxonline-0.1.2/pbxonline/models/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,16 +46,18 @@
     
     try:
         
         # There are inconsistencies in the API error response. Sometimes the error message is in the 'error_message' key, sometimes it's in the 'error' key.
         # We need to check for both.
         if 'error_message' in data:
             error_message = data['error_message']
-        else:
+        elif 'error' in data and 'errorMessage' in data['error']:
             error_message = data['error']['errorMessage']
+        else:
+            error_message = 'Unknown error'
         
     except KeyError as e:
         raise KeyError(f'Cannot construct error object from data. Missing key: {e}')
     
     object = BaseModel()
     
     object.has_error = True
```

### Comparing `python-pbxonline-0.1.1/python_pbxonline.egg-info/PKG-INFO` & `python-pbxonline-0.1.2/python_pbxonline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.1.1
+Version: 0.1.2
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.2.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.1.1/python_pbxonline.egg-info/SOURCES.txt` & `python-pbxonline-0.1.2/python_pbxonline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.1/setup.py` & `python-pbxonline-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'python-pbxonline',         
   packages=['pbxonline', 'pbxonline.models', 'pbxonline.constants', 'pbxonline.endpoints', 'pbxonline.cache'],
-  version = '0.1.1',
+  version = '0.1.2',
   license='GPL-3.0-or-later',
   description = 'Wrapper for PBX Online API',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@hotmail.com',
   url = 'https://github.com/alexanderlhsglobal/python-pbxonline',
-  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.1.tar.gz',
+  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.2.tar.gz',
   keywords = ['pbxonline'],
   install_requires=[
           'requests',
           'requests_oauthlib'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

### Comparing `python-pbxonline-0.1.1/tests/test_action.py` & `python-pbxonline-0.1.2/tests/test_action.py`

 * *Files identical despite different names*

