# Comparing `tmp/dj-starter-0.1.8.tar.gz` & `tmp/dj-starter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-starter-0.1.8.tar", max compression
+gzip compressed data, was "dj-starter-0.1.9.tar", max compression
```

## Comparing `dj-starter-0.1.8.tar` & `dj-starter-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       54 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/__init__.py
--rw-r--r--   0        0        0     2700 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/admin.py
--rw-r--r--   0        0        0      125 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/apps.py
--rw-r--r--   0        0        0      868 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/clients.py
--rw-r--r--   0        0        0     3879 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/decorators.py
--rw-r--r--   0        0        0      636 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/exceptions.py
--rw-r--r--   0        0        0        0 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/management/__init__.py
--rw-r--r--   0        0        0        0 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/management/commands/__init__.py
--rw-r--r--   0        0        0     2982 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/management/commands/create_db.py
--rw-r--r--   0        0        0      450 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/management/commands/print_env_vars.py
--rw-r--r--   0        0        0      738 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/managers.py
--rw-r--r--   0        0        0     3848 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/migrations/0001_initial.py
--rw-r--r--   0        0        0     1751 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/migrations/0002_task.py
--rw-r--r--   0        0        0        0 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/migrations/__init__.py
--rw-r--r--   0        0        0     5845 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/models.py
--rw-r--r--   0        0        0        0 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/tests/__init__.py
--rw-r--r--   0        0        0     1771 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/tests/test_clients.py
--rw-r--r--   0        0        0     3044 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/tests/test_decorators.py
--rw-r--r--   0        0        0     1739 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/tests/test_managers.py
--rw-r--r--   0        0        0     3785 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/tests/test_models.py
--rw-r--r--   0        0        0    11621 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/tests/test_utils.py
--rw-r--r--   0        0        0     5827 2022-03-13 19:45:49.161777 dj-starter-0.1.8/djstarter/utils.py
--rw-r--r--   0        0        0      711 2022-03-13 19:45:49.161777 dj-starter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      994 2022-03-13 19:46:34.537176 dj-starter-0.1.8/setup.py
--rw-r--r--   0        0        0      866 2022-03-13 19:46:34.537477 dj-starter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       54 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/__init__.py
+-rw-r--r--   0        0        0     2700 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/admin.py
+-rw-r--r--   0        0        0      125 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/apps.py
+-rw-r--r--   0        0        0      868 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/clients.py
+-rw-r--r--   0        0        0     3893 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/decorators.py
+-rw-r--r--   0        0        0      636 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/exceptions.py
+-rw-r--r--   0        0        0        0 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/management/commands/__init__.py
+-rw-r--r--   0        0        0     2982 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/management/commands/create_db.py
+-rw-r--r--   0        0        0      450 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/management/commands/print_env_vars.py
+-rw-r--r--   0        0        0      738 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/managers.py
+-rw-r--r--   0        0        0     3848 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1751 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/migrations/0002_task.py
+-rw-r--r--   0        0        0        0 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/migrations/__init__.py
+-rw-r--r--   0        0        0     5845 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/models.py
+-rw-r--r--   0        0        0        0 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/tests/__init__.py
+-rw-r--r--   0        0        0     1771 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/tests/test_clients.py
+-rw-r--r--   0        0        0     3044 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/tests/test_decorators.py
+-rw-r--r--   0        0        0     1739 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/tests/test_managers.py
+-rw-r--r--   0        0        0     3785 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/tests/test_models.py
+-rw-r--r--   0        0        0    11621 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/tests/test_utils.py
+-rw-r--r--   0        0        0     5827 2022-03-23 21:30:28.695483 dj-starter-0.1.9/djstarter/utils.py
+-rw-r--r--   0        0        0      711 2022-03-23 21:30:28.695483 dj-starter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      994 2022-03-23 21:31:31.600400 dj-starter-0.1.9/setup.py
+-rw-r--r--   0        0        0      866 2022-03-23 21:31:31.600623 dj-starter-0.1.9/PKG-INFO
```

### Comparing `dj-starter-0.1.8/djstarter/admin.py` & `dj-starter-0.1.9/djstarter/admin.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/clients.py` & `dj-starter-0.1.9/djstarter/clients.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/decorators.py` & `dj-starter-0.1.9/djstarter/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import time
 from functools import wraps
 
 from django.db import connection, connections
-from httpx import HTTPStatusError
+from httpx import codes, HTTPStatusError
 
 from . import utils
 from .exceptions import ApiError, NotAuthorized
 
 logger = logging.getLogger(__name__)
 
 
@@ -50,15 +50,15 @@
 
     @wraps(func)
     def wrapper_func(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except HTTPStatusError as e:
             status_code = e.response.status_code
-            if status_code in (408, 429, 502, 503, 504):     # Retryable status codes
+            if status_code in (408, 429) or status_code >= 500:     # Retryable status codes
                 raise
             if status_code == 401:
                 raise NotAuthorized(*args, **kwargs, **e.__dict__)
 
             raise ApiError(*args, **kwargs, **e.__dict__)
 
     return wrapper_func
```

### Comparing `dj-starter-0.1.8/djstarter/exceptions.py` & `dj-starter-0.1.9/djstarter/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/management/commands/create_db.py` & `dj-starter-0.1.9/djstarter/management/commands/create_db.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/managers.py` & `dj-starter-0.1.9/djstarter/managers.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/migrations/0001_initial.py` & `dj-starter-0.1.9/djstarter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/migrations/0002_task.py` & `dj-starter-0.1.9/djstarter/migrations/0002_task.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/models.py` & `dj-starter-0.1.9/djstarter/models.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/tests/test_clients.py` & `dj-starter-0.1.9/djstarter/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/tests/test_decorators.py` & `dj-starter-0.1.9/djstarter/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/tests/test_managers.py` & `dj-starter-0.1.9/djstarter/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/tests/test_models.py` & `dj-starter-0.1.9/djstarter/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/tests/test_utils.py` & `dj-starter-0.1.9/djstarter/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/djstarter/utils.py` & `dj-starter-0.1.9/djstarter/utils.py`

 * *Files identical despite different names*

### Comparing `dj-starter-0.1.8/pyproject.toml` & `dj-starter-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-starter"
-version = "0.1.8"
+version = "0.1.9"
 description = "Django Project Bootstraper with Common Models and Utilities"
 authors = ["Adrian <adrian@rydeas.com>"]
 repository = "https://github.com/adrianmeraz/dj-starter"
 
 packages = [
     { include = "djstarter" }
 ]
```

### Comparing `dj-starter-0.1.8/setup.py` & `dj-starter-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'jsonpickle>=2.1.0,<3.0.0',
  'psycopg2-binary>=2.9.2,<3.0.0',
  'python-dotenv>=0.19.0,<0.20.0',
  'wheel>=0.36.2,<0.37.0']
 
 setup_kwargs = {
     'name': 'dj-starter',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Django Project Bootstraper with Common Models and Utilities',
     'long_description': None,
     'author': 'Adrian',
     'author_email': 'adrian@rydeas.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/adrianmeraz/dj-starter',
```

### Comparing `dj-starter-0.1.8/PKG-INFO` & `dj-starter-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-starter
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django Project Bootstraper with Common Models and Utilities
 Home-page: https://github.com/adrianmeraz/dj-starter
 Author: Adrian
 Author-email: adrian@rydeas.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

