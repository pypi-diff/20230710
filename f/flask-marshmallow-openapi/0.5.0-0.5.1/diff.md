# Comparing `tmp/flask-marshmallow-openapi-0.5.0.tar.gz` & `tmp/flask-marshmallow-openapi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.5.0.tar", last modified: Fri Jul  7 09:17:00 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.5.1.tar", last modified: Mon Jul 10 16:59:13 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.5.0.tar` & `flask-marshmallow-openapi-0.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.220881 flask-marshmallow-openapi-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-07 09:17:00.220881 flask-marshmallow-openapi-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:17:00.220881 flask-marshmallow-openapi-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.208881 flask-marshmallow-openapi-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.212881 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.216881 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/flask_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/schemas_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.216881 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/redoc_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.220881 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.220881 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-07 09:16:50.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:17:00.212881 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-07 09:17:00.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-07 09:17:00.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:17:00.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:16:59.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 09:17:00.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-07 09:17:00.000000 flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.117761 flask-marshmallow-openapi-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-10 16:59:13.113761 flask-marshmallow-openapi-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:59:13.117761 flask-marshmallow-openapi-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.105761 flask-marshmallow-openapi-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.109761 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.109761 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/flask_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/schemas_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.109761 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.113761 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.113761 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-10 16:59:03.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:59:13.109761 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-10 16:59:13.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-10 16:59:13.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:59:13.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:59:12.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-10 16:59:13.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 16:59:13.000000 flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.5.0/.gitignore` & `flask-marshmallow-openapi-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/LICENSE` & `flask-marshmallow-openapi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/MANIFEST.in` & `flask-marshmallow-openapi-0.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/pyproject.toml` & `flask-marshmallow-openapi-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.5.0"
+version = "0.5.1"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_delete.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_get.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_get.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_patch.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 
 def patch(
     request_schema: Type[ma.Schema],
     response_schema: Type[ma.Schema] | None = None,
     *,
     operation_id: str | None = None,
+    has_id_in_path: bool = True,
     errors: dict[int, str] | None = None,
     additional_content: dict[str, dict | MediaTypeObject] | None = None,
     security: Securities = Securities.access_token,
 ):
     """
     Decorator that will inject standard sets of our OpenAPI PATCH docs into decorated
     method.
@@ -77,17 +78,17 @@
         response_schema = request_schema
 
     open_api_data = OperationObject()
 
     open_api_data.operationId = operation_id or FlaskPathsManager.generate_operation_id(
         "patch", False, response_schema
     )
-    has_id = bool(getattr(response_schema.opts, "url_id_field", None))
+    # has_id = bool(getattr(response_schema.opts, "url_id_field", None))
     _parameters_from_schema(
-        response_schema, requires_id_in_path=has_id, open_api_data=open_api_data
+        response_schema, requires_id_in_path=has_id_in_path, open_api_data=open_api_data
     )
 
     if security != Securities.no_token:
         open_api_data.security = [SecurityRequirementObject({f"{security.name}": []})]
 
     open_api_data.responses = ResponsesObject()
     open_api_data.responses["200"] = {
```

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/decorate_post.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/decorate_post.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/decorators/helpers.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/decorators/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/flask_paths.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/flask_paths.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,33 @@
 
 from .flask_paths import FlaskPathsManager
 from .schemas_registry import SchemasRegistry
 from .static_collector import StaticResourcesCollector
 
 _MINIMAL_SPEC = {"title": "Some API", "openapi_version": "3.0.2", "version": "v1"}
 
+_DEFAULT_SECURITIES = {
+    "components": {
+        "securitySchemes": {
+            "access_token": {
+                "scheme": "bearer",
+                "type": "http",
+                "bearerFormat": "JWT",
+                "description": "This endpoint requires [JWT](https://jwt.io/) access token.\n",
+            },
+            "refresh_token": {
+                "scheme": "bearer",
+                "type": "http",
+                "bearerFormat": "JWT",
+                "description": "This endpoint requires [JWT](https://jwt.io/) refresh token.\n",
+            },
+        }
+    },
+}
+
 
 @dataclass
 class OpenAPISettings:
     #: Name string displayed in various places in of API docs
     api_name: str
 
     #: Version string displayed in various places in of API docs
@@ -186,22 +205,15 @@
         full_url_prefix = (
             Path(self.config.mounted_at or "/") / f"./{self.blueprint.url_prefix}"
         )
 
         with app.test_request_context():
             SchemasRegistry.find_all_schemas(self.config.app_package_name)
 
-            initial_swagger_json: dict = _MINIMAL_SPEC
-            if self.config.swagger_json_template_loader:
-                if self.config.swagger_json_template_loader_kwargs:
-                    initial_swagger_json = self.config.swagger_json_template_loader(
-                        **self.config.swagger_json_template_loader_kwargs
-                    )
-                else:
-                    initial_swagger_json = self.config.swagger_json_template_loader()
+            initial_swagger_json = self._load_initial_spec()
 
             ma_plugin = MarshmallowPlugin()
             self._apispec = apispec.APISpec(
                 plugins=[ma_plugin], **(initial_swagger_json)
             )
             for _ in self._map_to_openapi_types:
                 ma_plugin.map_to_openapi_type(*_)
@@ -228,14 +240,33 @@
 
         app.register_blueprint(self.blueprint, url_prefix=str(full_url_prefix))
 
         if not hasattr(app, "extensions"):
             app.extensions = {}
         # app.extensions["open_api"] = self
 
+    def _load_initial_spec(self):
+        initial_swagger_json: dict = _MINIMAL_SPEC
+        if self.config.api_name:
+            _MINIMAL_SPEC["title"] = self.config.api_name
+        if self.config.api_version:
+            _MINIMAL_SPEC["version"] = self.config.api_version
+
+        if self.config.swagger_json_template_loader:
+            if self.config.swagger_json_template_loader_kwargs:
+                initial_swagger_json = self.config.swagger_json_template_loader(
+                    **self.config.swagger_json_template_loader_kwargs
+                )
+            else:
+                initial_swagger_json = self.config.swagger_json_template_loader()
+
+        initial_swagger_json.update(_DEFAULT_SECURITIES)
+
+        return initial_swagger_json
+
     def collect_static(self, destination_dir: str | Path):
         StaticResourcesCollector(self, destination_dir).collect()
 
     def _swagger_ui_template_config(self, config_overrides=None, oauth_config=None):
         # Swagger UI config
         # see: https://github.com/swagger-api/swagger-ui
         config = {
```

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/schemas_registry.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/schemas_registry.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/redoc_favicon.png` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/redoc_favicon.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.5.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.5.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

