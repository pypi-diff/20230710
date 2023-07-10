# Comparing `tmp/strongmind-canvas-api-client-0.1.1.tar.gz` & `tmp/strongmind-canvas-api-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/strongmind-canvas-api-client-0.1.1.tar", last modified: Thu Jun  9 00:18:04 2022, max compression
+gzip compressed data, was "strongmind-canvas-api-client-0.1.2.tar", last modified: Mon Jul 10 18:49:07 2023, max compression
```

## Comparing `strongmind-canvas-api-client-0.1.1.tar` & `strongmind-canvas-api-client-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      571 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-09 00:15:34.000000 strongmind-canvas-api-client-0.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)      103 2022-06-09 00:15:34.000000 strongmind-canvas-api-client-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      663 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-09 00:15:34.000000 strongmind-canvas-api-client-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/src/canvas_api_client/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-09 00:15:34.000000 strongmind-canvas-api-client-0.1.1/src/canvas_api_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4096 2022-06-09 00:15:34.000000 strongmind-canvas-api-client-0.1.1/src/canvas_api_client/canvas_api_client.py
--rw-r--r--   0 root         (0) root         (0)      286 2022-06-09 00:15:34.000000 strongmind-canvas-api-client-0.1.1/src/canvas_api_client/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      773 2022-06-09 00:15:34.000000 strongmind-canvas-api-client-0.1.1/src/canvas_api_client/secrets_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/src/strongmind_canvas_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      571 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/src/strongmind_canvas_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      421 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/src/strongmind_canvas_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/src/strongmind_canvas_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-06-09 00:18:04.000000 strongmind-canvas-api-client-0.1.1/src/strongmind_canvas_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:49:07.726066 strongmind-canvas-api-client-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-10 18:49:07.726066 strongmind-canvas-api-client-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-10 18:49:07.726066 strongmind-canvas-api-client-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:49:07.722066 strongmind-canvas-api-client-0.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:49:07.726066 strongmind-canvas-api-client-0.1.2/src/canvas_api_client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/src/canvas_api_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/src/canvas_api_client/canvas_api_client.py
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/src/canvas_api_client/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-10 18:48:52.000000 strongmind-canvas-api-client-0.1.2/src/canvas_api_client/secrets_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 18:49:07.726066 strongmind-canvas-api-client-0.1.2/src/strongmind_canvas_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-10 18:49:07.000000 strongmind-canvas-api-client-0.1.2/src/strongmind_canvas_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      429 2023-07-10 18:49:07.000000 strongmind-canvas-api-client-0.1.2/src/strongmind_canvas_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 18:49:07.000000 strongmind-canvas-api-client-0.1.2/src/strongmind_canvas_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-10 18:49:07.000000 strongmind-canvas-api-client-0.1.2/src/strongmind_canvas_api_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `strongmind-canvas-api-client-0.1.1/PKG-INFO` & `strongmind-canvas-api-client-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: strongmind-canvas-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Home-page: https://github.com/StrongMind/canvas_api_client
 Author: The Steakholders
 Author-email: tesla@strongnmind.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/StrongMind/canvas_api_client/issues
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+#TODO:
+
+
```

### Comparing `strongmind-canvas-api-client-0.1.1/setup.cfg` & `strongmind-canvas-api-client-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = strongmind-canvas-api-client
-version = 0.1.1
+version = 0.1.2
 author = The Steakholders
 author_email = tesla@strongnmind.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/StrongMind/canvas_api_client
 project_urls =
```

### Comparing `strongmind-canvas-api-client-0.1.1/src/canvas_api_client/canvas_api_client.py` & `strongmind-canvas-api-client-0.1.2/src/canvas_api_client/canvas_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,9 +117,9 @@
             raise APIKeyNotFoundError(f"Invalid Secret: {secrets_library}")
 
         return returned_secret
 
     @staticmethod
     def validate_and_return_domain(domain):
         if not domain:
-            raise DomainNameNullError(f"DomainNameNullError: Domain - {domain}")
+            raise DomainNameNullError(f"DomainNameNullError: No Domain Provided")
         return domain
```

### Comparing `strongmind-canvas-api-client-0.1.1/src/canvas_api_client/secrets_manager.py` & `strongmind-canvas-api-client-0.1.2/src/canvas_api_client/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `strongmind-canvas-api-client-0.1.1/src/strongmind_canvas_api_client.egg-info/PKG-INFO` & `strongmind-canvas-api-client-0.1.2/src/strongmind_canvas_api_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: strongmind-canvas-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Home-page: https://github.com/StrongMind/canvas_api_client
 Author: The Steakholders
 Author-email: tesla@strongnmind.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/StrongMind/canvas_api_client/issues
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+#TODO:
+
+
```

