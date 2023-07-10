# Comparing `tmp/dynamic-service-1.4.2.tar.gz` & `tmp/dynamic-service-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.4.2.tar", last modified: Sun Jul  9 08:27:10 2023, max compression
+gzip compressed data, was "dynamic-service-1.4.3.tar", last modified: Mon Jul 10 07:19:45 2023, max compression
```

## Comparing `dynamic-service-1.4.2.tar` & `dynamic-service-1.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.416180 dynamic-service-1.4.2/
--rw-rw-rw-   0        0        0      236 2023-07-09 08:27:10.000000 dynamic-service-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-09 08:27:10.416180 dynamic-service-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.4.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.4.2/build.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.360178 dynamic-service-1.4.2/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.4.2/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.407179 dynamic-service-1.4.2/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.4.2/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.4.2/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.4.2/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.4.2/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.4.2/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.413179 dynamic-service-1.4.2/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.4.2/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20814 2023-07-09 08:27:06.000000 dynamic-service-1.4.2/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.4.2/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.350503 dynamic-service-1.4.2/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.350503 dynamic-service-1.4.2/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.415179 dynamic-service-1.4.2/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.4.2/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.4.2/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-09 08:27:10.378178 dynamic-service-1.4.2/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-09 08:27:10.000000 dynamic-service-1.4.2/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-09 08:27:10.000000 dynamic-service-1.4.2/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 08:27:10.000000 dynamic-service-1.4.2/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-09 08:27:10.000000 dynamic-service-1.4.2/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 08:27:10.000000 dynamic-service-1.4.2/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-09 08:27:10.000000 dynamic-service-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.4.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.4.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 08:27:10.416180 dynamic-service-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-09 08:27:06.000000 dynamic-service-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.756045 dynamic-service-1.4.3/
+-rw-rw-rw-   0        0        0      236 2023-07-10 07:19:44.000000 dynamic-service-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-10 07:19:45.755541 dynamic-service-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/build.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.696094 dynamic-service-1.4.3/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.738286 dynamic-service-1.4.3/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.4.3/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.4.3/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.4.3/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.4.3/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.748915 dynamic-service-1.4.3/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20624 2023-07-10 07:19:23.000000 dynamic-service-1.4.3/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.4.3/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.686496 dynamic-service-1.4.3/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.686496 dynamic-service-1.4.3/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.753427 dynamic-service-1.4.3/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-10 07:19:45.710348 dynamic-service-1.4.3/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-10 07:19:45.000000 dynamic-service-1.4.3/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-10 07:19:44.000000 dynamic-service-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.4.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.4.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 07:19:45.756045 dynamic-service-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-10 07:19:39.000000 dynamic-service-1.4.3/setup.py
```

### Comparing `dynamic-service-1.4.2/PKG-INFO` & `dynamic-service-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.4.2
+Version: 1.4.3
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.4.2/README.md` & `dynamic-service-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/build.py` & `dynamic-service-1.4.3/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/base.py` & `dynamic-service-1.4.3/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/endpoints/data.py` & `dynamic-service-1.4.3/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/endpoints/engine.py` & `dynamic-service-1.4.3/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.4.3/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/endpoints/process.py` & `dynamic-service-1.4.3/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/service/rest.py` & `dynamic-service-1.4.3/dynamic_service/service/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,18 +177,15 @@
 
         self._root: Optional[str] = None
 
         _Base = type(self)
 
         self.endpoints: Dict[str, BaseEndpoint[_Base]] = {}
 
-        if (
-            (isinstance(home, bool) and home) or
-            (debug and (home is None))
-        ):
+        if (home is True) or (debug and (home is None)):
             home = True
         # end if
 
         self.app: Optional[FastAPI] = None
         self.server: Optional[Server] = None
 
         self._serving_process: Optional[threading.Thread] = None
@@ -490,35 +487,34 @@
                     path, command,
                     methods=endpoint.methods, description=endpoint.description,
                     **endpoint.options
                 )
             # end try
         # end for
 
+        root = "/" + self.root if self.root else ''
+
         if (self.icon is not None) and os.path.exists(self.icon):
             router.add_api_route(
-                ("/" + self.root if self.root else '') + FAVICON,
-                lambda: EndpointFileResponse(self.icon),
+                root + FAVICON, lambda: EndpointFileResponse(self.icon),
                 methods=[GET], include_in_schema=False
             )
         # end if
 
         if isinstance(self.home, bool) and self.home:
             router.add_api_route(
-                ("/" + self.root if self.root else '') + '/',
-                lambda: EndpointRedirectResponse(DOCS),
+                root + '/', lambda: EndpointRedirectResponse(DOCS),
                 methods=[GET], include_in_schema=False
             )
         # end if
 
         if DOCS not in self.endpoints:
             router.add_api_route(
-                ("/" + self.root if self.root else '') + DOCS,
-                DocsEndpoint(
-                    icon=("/" + self.root if self.root else '') + FAVICON,
+                root + DOCS, DocsEndpoint(
+                    icon=root + FAVICON,
                     methods=[GET], title=self.name
                 ).endpoint, methods=[GET], include_in_schema=False
             )
         # end if
 
         self.app.include_router(router)
     # end build
```

### Comparing `dynamic-service-1.4.2/dynamic_service/service/sockets.py` & `dynamic-service-1.4.3/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.4.3/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.4.3/dynamic_service.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.4.2
+Version: 1.4.3
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.4.2/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.4.3/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.2/pyproject.toml` & `dynamic-service-1.4.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.4.2'
+version = '1.4.3'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.4.2/setup.py` & `dynamic-service-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.4.2',
+        version='1.4.3',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

