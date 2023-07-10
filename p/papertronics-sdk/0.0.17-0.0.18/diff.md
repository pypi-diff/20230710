# Comparing `tmp/papertronics-sdk-0.0.17.tar.gz` & `tmp/papertronics-sdk-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.17.tar", last modified: Mon Jul 10 14:09:20 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.18.tar", last modified: Mon Jul 10 14:10:53 2023, max compression
```

## Comparing `papertronics-sdk-0.0.17.tar` & `papertronics-sdk-0.0.18.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:09:20.445729 papertronics-sdk-0.0.17/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.17/LICENSE
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1425 2023-07-10 14:09:20.449729 papertronics-sdk-0.0.17/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      975 2023-07-10 08:17:39.000000 papertronics-sdk-0.0.17/README.md
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:09:20.445729 papertronics-sdk-0.0.17/papertronics_sdk/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.17/papertronics_sdk/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:09:20.445729 papertronics-sdk-0.0.17/papertronics_sdk/lab/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5319 2023-07-10 11:10:36.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/admin_client.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1469 2023-07-10 11:10:36.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/base_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:09:20.445729 papertronics-sdk-0.0.17/papertronics_sdk/lab/exceptions/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/exceptions/StatusException.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/exceptions/__init__.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:09:20.445729 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/__init__.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/cloud_models.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/config.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/database.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/generic.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/models/station_protocol.py
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9139 2023-07-10 12:23:51.000000 papertronics-sdk-0.0.17/papertronics_sdk/lab/user_client.py
-drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:09:20.445729 papertronics-sdk-0.0.17/papertronics_sdk.egg-info/
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1425 2023-07-10 14:09:20.000000 papertronics-sdk-0.0.17/papertronics_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-10 14:09:20.000000 papertronics-sdk-0.0.17/papertronics_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-10 14:09:20.000000 papertronics-sdk-0.0.17/papertronics_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-10 14:09:20.000000 papertronics-sdk-0.0.17/papertronics_sdk.egg-info/requires.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-10 14:09:20.000000 papertronics-sdk-0.0.17/papertronics_sdk.egg-info/top_level.txt
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-10 14:09:20.000000 papertronics-sdk-0.0.17/papertronics_sdk.egg-info/zip-safe
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.17/pyproject.toml
--rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-10 14:09:20.449729 papertronics-sdk-0.0.17/setup.cfg
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      207 2023-07-10 08:19:33.000000 papertronics-sdk-0.0.18/LICENSE
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1425 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      975 2023-07-10 08:17:39.000000 papertronics-sdk-0.0.18/README.md
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:19:48.000000 papertronics-sdk-0.0.18/papertronics_sdk/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/lab/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 08:20:22.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     5319 2023-07-10 11:10:36.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/admin_client.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1469 2023-07-10 11:10:36.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/base_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/lab/exceptions/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      330 2023-07-10 10:48:57.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/exceptions/StatusException.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 10:45:22.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/exceptions/__init__.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        0 2023-05-31 07:21:33.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/__init__.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      288 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1826 2023-06-28 11:09:30.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/cloud_models.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      426 2023-06-12 09:35:19.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/config.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     3368 2023-07-10 08:23:40.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/database.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      965 2023-07-10 08:26:50.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/generic.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     8556 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/models/station_protocol.py
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     9139 2023-07-10 12:23:51.000000 papertronics-sdk-0.0.18/papertronics_sdk/lab/user_client.py
+drwxrwxr-x   0 jobheersink  (1000) jobheersink  (1000)        0 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)     1425 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      841 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       31 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/requires.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       17 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)        1 2023-07-10 14:10:53.000000 papertronics-sdk-0.0.18/papertronics_sdk.egg-info/zip-safe
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)       86 2023-06-28 08:05:09.000000 papertronics-sdk-0.0.18/pyproject.toml
+-rw-rw-r--   0 jobheersink  (1000) jobheersink  (1000)      637 2023-07-10 14:10:53.150778 papertronics-sdk-0.0.18/setup.cfg
```

### Comparing `papertronics-sdk-0.0.17/PKG-INFO` & `papertronics-sdk-0.0.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.17
+Version: 0.0.18
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.17/README.md` & `papertronics-sdk-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.18/papertronics_sdk/lab/admin_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.18/papertronics_sdk/lab/base_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.18/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.18/papertronics_sdk/lab/user_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk.egg-info/PKG-INFO` & `papertronics-sdk-0.0.18/papertronics_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.17
+Version: 0.0.18
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.17/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.18/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.17/setup.cfg` & `papertronics-sdk-0.0.18/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.17
+version = 0.0.18
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```

