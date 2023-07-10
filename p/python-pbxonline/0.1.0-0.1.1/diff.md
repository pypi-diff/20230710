# Comparing `tmp/python-pbxonline-0.1.0.tar.gz` & `tmp/python-pbxonline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pbxonline-0.1.0.tar", last modified: Mon Jul 10 10:44:25 2023, max compression
+gzip compressed data, was "python-pbxonline-0.1.1.tar", last modified: Mon Jul 10 11:03:38 2023, max compression
```

## Comparing `python-pbxonline-0.1.0.tar` & `python-pbxonline-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 10:44:25.896685 python-pbxonline-0.1.0/
--rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      798 2023-07-10 10:44:25.896685 python-pbxonline-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 10:44:25.843562 python-pbxonline-0.1.0/pbxonline/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.0/pbxonline/__init__.py
--rw-rw-rw-   0        0        0     7780 2023-07-10 10:42:39.000000 python-pbxonline-0.1.0/pbxonline/api.py
--rw-rw-rw-   0        0        0     3451 2023-07-07 09:09:45.000000 python-pbxonline-0.1.0/pbxonline/auth_handler.py
--rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.1.0/pbxonline/cache_handler.py
--rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.1.0/pbxonline/config.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:44:25.847205 python-pbxonline-0.1.0/pbxonline/constants/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.0/pbxonline/constants/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.1.0/pbxonline/constants/constants.py
--rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.1.0/pbxonline/constants/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:44:25.852733 python-pbxonline-0.1.0/pbxonline/endpoints/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.0/pbxonline/endpoints/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-07-07 11:31:06.000000 python-pbxonline-0.1.0/pbxonline/endpoints/action.py
--rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.1.0/pbxonline/endpoints/base.py
--rw-rw-rw-   0        0        0      658 2023-07-07 12:11:14.000000 python-pbxonline-0.1.0/pbxonline/endpoints/pbx.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:44:25.855518 python-pbxonline-0.1.0/pbxonline/models/
--rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.0/pbxonline/models/__init__.py
--rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.1.0/pbxonline/models/base.py
--rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.1.0/pbxonline/models/errors.py
--rw-rw-rw-   0        0        0     2372 2023-07-07 11:24:25.000000 python-pbxonline-0.1.0/pbxonline/models/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:44:25.884080 python-pbxonline-0.1.0/python_pbxonline.egg-info/
--rw-rw-rw-   0        0        0      798 2023-07-10 10:44:25.000000 python-pbxonline-0.1.0/python_pbxonline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2023-07-10 10:44:25.000000 python-pbxonline-0.1.0/python_pbxonline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 10:44:25.000000 python-pbxonline-0.1.0/python_pbxonline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 10:44:25.000000 python-pbxonline-0.1.0/python_pbxonline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 10:44:25.000000 python-pbxonline-0.1.0/python_pbxonline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-10 10:44:25.896685 python-pbxonline-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-07-10 10:44:15.000000 python-pbxonline-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:44:25.896685 python-pbxonline-0.1.0/tests/
--rw-rw-rw-   0        0        0      538 2023-07-07 11:31:21.000000 python-pbxonline-0.1.0/tests/test_action.py
--rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.1.0/tests/test_auth.py
--rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.1.0/tests/test_pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.196246 python-pbxonline-0.1.1/
+-rw-rw-rw-   0        0        0    35821 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      798 2023-07-10 11:03:38.197244 python-pbxonline-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-07 11:33:48.000000 python-pbxonline-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.152087 python-pbxonline-0.1.1/pbxonline/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/__init__.py
+-rw-rw-rw-   0        0        0     7780 2023-07-10 10:42:39.000000 python-pbxonline-0.1.1/pbxonline/api.py
+-rw-rw-rw-   0        0        0     3451 2023-07-07 09:09:45.000000 python-pbxonline-0.1.1/pbxonline/auth_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.154087 python-pbxonline-0.1.1/pbxonline/cache/
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:42:27.000000 python-pbxonline-0.1.1/pbxonline/cache/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-07-07 08:51:00.000000 python-pbxonline-0.1.1/pbxonline/cache_handler.py
+-rw-rw-rw-   0        0        0      173 2023-07-07 08:50:19.000000 python-pbxonline-0.1.1/pbxonline/config.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.158088 python-pbxonline-0.1.1/pbxonline/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/constants/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 08:35:02.000000 python-pbxonline-0.1.1/pbxonline/constants/constants.py
+-rw-rw-rw-   0        0        0      105 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/constants/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.166085 python-pbxonline-0.1.1/pbxonline/endpoints/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-07-07 11:31:06.000000 python-pbxonline-0.1.1/pbxonline/endpoints/action.py
+-rw-rw-rw-   0        0        0      141 2023-04-24 12:47:39.000000 python-pbxonline-0.1.1/pbxonline/endpoints/base.py
+-rw-rw-rw-   0        0        0      658 2023-07-07 12:11:14.000000 python-pbxonline-0.1.1/pbxonline/endpoints/pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.173326 python-pbxonline-0.1.1/pbxonline/models/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:50:30.000000 python-pbxonline-0.1.1/pbxonline/models/__init__.py
+-rw-rw-rw-   0        0        0     1346 2023-04-27 06:19:09.000000 python-pbxonline-0.1.1/pbxonline/models/base.py
+-rw-rw-rw-   0        0        0      165 2023-07-07 08:33:02.000000 python-pbxonline-0.1.1/pbxonline/models/errors.py
+-rw-rw-rw-   0        0        0     2372 2023-07-07 11:24:25.000000 python-pbxonline-0.1.1/pbxonline/models/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.186989 python-pbxonline-0.1.1/python_pbxonline.egg-info/
+-rw-rw-rw-   0        0        0      798 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 11:03:38.000000 python-pbxonline-0.1.1/python_pbxonline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-10 11:03:38.200318 python-pbxonline-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2023-07-10 11:03:31.000000 python-pbxonline-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 11:03:38.195244 python-pbxonline-0.1.1/tests/
+-rw-rw-rw-   0        0        0      538 2023-07-07 11:31:21.000000 python-pbxonline-0.1.1/tests/test_action.py
+-rw-rw-rw-   0        0        0      266 2023-07-07 08:50:49.000000 python-pbxonline-0.1.1/tests/test_auth.py
+-rw-rw-rw-   0        0        0      410 2023-07-07 12:53:43.000000 python-pbxonline-0.1.1/tests/test_pbx.py
```

### Comparing `python-pbxonline-0.1.0/LICENSE.txt` & `python-pbxonline-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/PKG-INFO` & `python-pbxonline-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.1.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.1.0/pbxonline/api.py` & `python-pbxonline-0.1.1/pbxonline/api.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/pbxonline/auth_handler.py` & `python-pbxonline-0.1.1/pbxonline/auth_handler.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/pbxonline/cache_handler.py` & `python-pbxonline-0.1.1/pbxonline/cache_handler.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/pbxonline/endpoints/action.py` & `python-pbxonline-0.1.1/pbxonline/endpoints/action.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/pbxonline/endpoints/pbx.py` & `python-pbxonline-0.1.1/pbxonline/endpoints/pbx.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/pbxonline/models/base.py` & `python-pbxonline-0.1.1/pbxonline/models/base.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/pbxonline/models/utils.py` & `python-pbxonline-0.1.1/pbxonline/models/utils.py`

 * *Files identical despite different names*

### Comparing `python-pbxonline-0.1.0/python_pbxonline.egg-info/PKG-INFO` & `python-pbxonline-0.1.1/python_pbxonline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-pbxonline
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper for PBX Online API
 Home-page: https://github.com/alexanderlhsglobal/python-pbxonline
-Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.1.tar.gz
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@hotmail.com
 License: GPL-3.0-or-later
 Keywords: pbxonline
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python-pbxonline-0.1.0/python_pbxonline.egg-info/SOURCES.txt` & `python-pbxonline-0.1.1/python_pbxonline.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 pbxonline/__init__.py
 pbxonline/api.py
 pbxonline/auth_handler.py
 pbxonline/cache_handler.py
 pbxonline/config.py
+pbxonline/cache/__init__.py
 pbxonline/constants/__init__.py
 pbxonline/constants/constants.py
 pbxonline/constants/errors.py
 pbxonline/endpoints/__init__.py
 pbxonline/endpoints/action.py
 pbxonline/endpoints/base.py
 pbxonline/endpoints/pbx.py
```

### Comparing `python-pbxonline-0.1.0/setup.py` & `python-pbxonline-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'python-pbxonline',         
-  packages=['pbxonline', 'pbxonline.models', 'pbxonline.constants', 'pbxonline.endpoints'],
-  version = '0.1.0',
+  packages=['pbxonline', 'pbxonline.models', 'pbxonline.constants', 'pbxonline.endpoints', 'pbxonline.cache'],
+  version = '0.1.1',
   license='GPL-3.0-or-later',
   description = 'Wrapper for PBX Online API',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@hotmail.com',
   url = 'https://github.com/alexanderlhsglobal/python-pbxonline',
-  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.0.tar.gz',
+  download_url = 'https://github.com/alexanderlhsglobal/python-pbxonline/archive/refs/tags/0.1.1.tar.gz',
   keywords = ['pbxonline'],
   install_requires=[
           'requests',
           'requests_oauthlib'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

### Comparing `python-pbxonline-0.1.0/tests/test_action.py` & `python-pbxonline-0.1.1/tests/test_action.py`

 * *Files identical despite different names*

