# Comparing `tmp/Ruster-2.0.1.tar.gz` & `tmp/Ruster-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-2.0.1.tar", last modified: Sat Jul  8 21:03:04 2023, max compression
+gzip compressed data, was "Ruster-2.0.2.tar", last modified: Mon Jul 10 20:45:45 2023, max compression
```

## Comparing `Ruster-2.0.1.tar` & `Ruster-2.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 21:03:04.828704 Ruster-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-08 21:03:04.828704 Ruster-2.0.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 21:03:04.828704 Ruster-2.0.1/Ruster.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      383 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-07-08 21:03:04.000000 Ruster-2.0.1/Ruster.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-08 21:03:04.828704 Ruster-2.0.1/ruster/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-07 17:26:00.000000 Ruster-2.0.1/ruster/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13358 2023-07-08 20:55:05.000000 Ruster-2.0.1/ruster/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1345 2023-07-06 08:52:08.000000 Ruster-2.0.1/ruster/blueprints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2023-07-04 18:04:16.000000 Ruster-2.0.1/ruster/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3761 2023-07-06 17:39:42.000000 Ruster-2.0.1/ruster/hasher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7955 2023-07-06 17:40:00.000000 Ruster-2.0.1/ruster/jwt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2664 2023-07-06 08:37:16.000000 Ruster-2.0.1/ruster/limiter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2923 2023-07-06 17:39:06.000000 Ruster-2.0.1/ruster/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1089 2023-07-08 20:35:21.000000 Ruster-2.0.1/ruster/sanitizer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-07-05 18:45:58.000000 Ruster-2.0.1/ruster/session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2679 2023-07-06 17:40:22.000000 Ruster-2.0.1/ruster/wtf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-08 21:03:04.828704 Ruster-2.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      788 2023-07-08 21:00:20.000000 Ruster-2.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:45:45.742154 Ruster-2.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-10 20:45:45.742154 Ruster-2.0.2/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:45:45.742154 Ruster-2.0.2/Ruster.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-07-10 20:45:45.000000 Ruster-2.0.2/Ruster.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      383 2023-07-10 20:45:45.000000 Ruster-2.0.2/Ruster.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-10 20:45:45.000000 Ruster-2.0.2/Ruster.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-07-10 20:45:45.000000 Ruster-2.0.2/Ruster.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-07-10 20:45:45.000000 Ruster-2.0.2/Ruster.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-07-10 20:45:45.000000 Ruster-2.0.2/Ruster.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-10 20:45:45.742154 Ruster-2.0.2/ruster/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-07 17:26:00.000000 Ruster-2.0.2/ruster/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13383 2023-07-10 20:43:07.000000 Ruster-2.0.2/ruster/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1345 2023-07-06 08:52:08.000000 Ruster-2.0.2/ruster/blueprints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2023-07-04 18:04:16.000000 Ruster-2.0.2/ruster/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3761 2023-07-06 17:39:42.000000 Ruster-2.0.2/ruster/hasher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7955 2023-07-06 17:40:00.000000 Ruster-2.0.2/ruster/jwt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2664 2023-07-06 08:37:16.000000 Ruster-2.0.2/ruster/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2923 2023-07-06 17:39:06.000000 Ruster-2.0.2/ruster/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1089 2023-07-08 20:35:21.000000 Ruster-2.0.2/ruster/sanitizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-07-05 18:45:58.000000 Ruster-2.0.2/ruster/session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2679 2023-07-06 17:40:22.000000 Ruster-2.0.2/ruster/wtf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-10 20:45:45.742154 Ruster-2.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      788 2023-07-10 20:45:29.000000 Ruster-2.0.2/setup.py
```

### Comparing `Ruster-2.0.1/ruster/app.py` & `Ruster-2.0.2/ruster/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 from werkzeug.exceptions import NotFound, MethodNotAllowed, BadRequest, Unauthorized, Forbidden, HTTPException
 from werkzeug.middleware.dispatcher import DispatcherMiddleware
 from itsdangerous import URLSafeTimedSerializer, BadSignature
 from werkzeug.serving import run_simple
 from werkzeug.urls import url_encode
 from .session import session_manager
 from .limiter import Limiter
+import mimetypes
 
 
 class Rust:
     def __init__(self):
         self.url_map = Map()
         self.error_handlers = {}
         self.before_request_funcs = []
         self.after_request_funcs = []
-        self.template_env = Environment(loader=FileSystemLoader('templates'))
+        self.template_env = Environment(loader=FileSystemLoader('views'))
         self.host = '127.0.0.1'
         self.port = 8000
         self.debug = True
         self.view_functions = {}
         self.blueprints = []
         self.middlewares = []
         self.flash_messages = {}
         self.request_context = None
-        self.static_folder = 'public'
-        self.template_folder = 'templates'
+        self.static_folder = "public"
+        self.template_folder = None
         self.limiter = Limiter()
         self.config = {}
         self.load_config()
 
     def route(self, rule, methods=['GET'], strict_slashes=False, secure=False):
         def decorator(f):
             endpoint = f.__name__
@@ -137,23 +138,14 @@
             return self.handle_forbidden(request, e)
         except Unauthorized as e:
             return self.handle_unauthorized(request, e)
         except HTTPException as e:
             response = await self.handle_exception(e)
         return response
 
-    def serve_static(self, path):
-        static_path = os.path.join(self.static_folder, path)
-        if os.path.exists(static_path):
-            with open(static_path, 'rb') as f:
-                response = self.response(f.read())
-                response.headers['Content-Type'] = 'text/css' if path.endswith('.css') else 'text/javascript'
-                return response
-        return self.handle_not_found()
-
     def handle_not_found(self, request):
         error_template_path = os.path.join(self.template_folder, 'errors', '404.html')
         if os.path.exists(error_template_path):
             with open(error_template_path, 'r') as f:
                 error_template = f.read()
             return Response(error_template, status=404, content_type='text/html')
         else:
@@ -253,18 +245,18 @@
 crust = Rust()
 request = VeloRequest
 
 
 def jsonify(data):
     return Response(json.dumps(data), mimetype='application/json')
 
-
-def render_template(template_name, **context):
+def render_template(template_name, **kwargs):
     template = crust.template_env.get_template(template_name)
-    return Response(template.render(**context), mimetype='text/html')
+    kwargs['url_for_static'] = url_for_static
+    return Response(template.render(**kwargs), mimetype='text/html')
 
 
 def make_response(response):
     if isinstance(response, str):
         return Response(response)
     return response
 
@@ -278,14 +270,16 @@
     else:
         return Response('Invalid redirect location.', status=400)
 
 
 def url_for(endpoint, **values):
     return crust.url_map.bind('').build(endpoint, values)
 
+def url_for_static(filename):
+    return f'/static/{filename}'
 
 def send_file(filename, mimetype=None, as_attachment=False):
     response = Response()
     response.headers['Content-Disposition'] = f'attachment; filename="{filename}"' if as_attachment else f'inline; filename="{filename}"'
     if mimetype is not None:
         response.headers['Content-Type'] = mimetype
     return response
@@ -333,14 +327,21 @@
     crust.static_folder = static_folder
 
 
 def set_template_folder(template_folder):
     crust.template_folder = template_folder
     crust.template_env = Environment(loader=FileSystemLoader(template_folder))
 
+def serve_static(filename):
+        static_path = os.path.join(crust.static_folder, filename)
+        if os.path.isfile(static_path):
+            mimetype, _ = mimetypes.guess_type(static_path)
+            if mimetype:
+                return Response(open(static_path, 'rb').read(), mimetype=mimetype)
+        raise NotFound()
 
 @staticmethod
 def make_secure_token(salt=None, key=None):
     if salt is None:
         salt = crust.config.get('SECRET_KEY', os.urandom(24))
     if key is None:
         key = os.urandom(16)
```

### Comparing `Ruster-2.0.1/ruster/blueprints.py` & `Ruster-2.0.2/ruster/blueprints.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/ruster/hasher.py` & `Ruster-2.0.2/ruster/hasher.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/ruster/jwt.py` & `Ruster-2.0.2/ruster/jwt.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/ruster/limiter.py` & `Ruster-2.0.2/ruster/limiter.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/ruster/mailer.py` & `Ruster-2.0.2/ruster/mailer.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/ruster/sanitizer.py` & `Ruster-2.0.2/ruster/sanitizer.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/ruster/session.py` & `Ruster-2.0.2/ruster/session.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/ruster/wtf.py` & `Ruster-2.0.2/ruster/wtf.py`

 * *Files identical despite different names*

### Comparing `Ruster-2.0.1/setup.py` & `Ruster-2.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Ruster',
-    version='2.0.1',
+    version='2.0.2',
     author='Pawan Kumar',
     author_email='control@vvfin.in',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

