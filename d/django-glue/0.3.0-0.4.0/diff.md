# Comparing `tmp/django-glue-0.3.0.tar.gz` & `tmp/django-glue-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.3.0.tar", last modified: Thu Jun 22 22:14:13 2023, max compression
+gzip compressed data, was "django-glue-0.4.0.tar", last modified: Mon Jul 10 19:18:47 2023, max compression
```

## Comparing `django-glue-0.3.0.tar` & `django-glue-0.4.0.tar`

### file list

```diff
@@ -1,68 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-22 22:14:02.000000 django-glue-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 22:14:02.000000 django-glue-0.3.0/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-22 22:14:02.000000 django-glue-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 22:14:02.000000 django-glue-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-22 22:14:13.025857 django-glue-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-22 22:14:02.000000 django-glue-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.021857 django-glue-0.3.0/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.021857 django-glue-0.3.0/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.017857 django-glue-0.3.0/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.017857 django-glue-0.3.0/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_response.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.017857 django-glue-0.3.0/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-22 22:14:02.000000 django-glue-0.3.0/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.021857 django-glue-0.3.0/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 22:14:12.000000 django-glue-0.3.0/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 22:14:02.000000 django-glue-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 22:14:13.025857 django-glue-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-22 22:14:02.000000 django-glue-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:13.025857 django-glue-0.3.0/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 22:14:02.000000 django-glue-0.3.0/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-10 19:18:36.000000 django-glue-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-10 19:18:36.000000 django-glue-0.4.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 19:18:36.000000 django-glue-0.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 19:18:36.000000 django-glue-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-10 19:18:47.818792 django-glue-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-10 19:18:36.000000 django-glue-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.810792 django-glue-0.4.0/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.810792 django-glue-0.4.0/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.810792 django-glue-0.4.0/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 19:18:36.000000 django-glue-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 19:18:47.818792 django-glue-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-10 19:18:36.000000 django-glue-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/wsgi.py
```

### Comparing `django-glue-0.3.0/CHANGELOG.md` & `django-glue-0.4.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Changelog for Django Glue
 
+## 0.4.1
+
+#### Features
+- Event system implement for responses.
+
+#### Changes
+
+#### Bugs
+
+## 0.4.0
+
+#### Features
+- You can now glue templates by submitting a full template path as a string to add_glue function call.
+- You can now use the experimental load views in your templates with GlueView.
+
+#### Changes
+- All validation moved to server side.
+- Base level of benchmarks complete test at roughly 1ms to run add_glue function.
+
 ## 0.3.0
 
 #### Features
 - You can now glue django model methods (this works on both model objects and query sets).
 - Now works with all javascript not just alpine.
 
 #### Changes
```

### Comparing `django-glue-0.3.0/LICENSE.md` & `django-glue-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/PKG-INFO` & `django-glue-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.3.0
+Version: 0.4.0
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.3.0/README.md` & `django-glue-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue/context_processors.py` & `django-glue-0.4.0/django_glue/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue/data_classes.py` & `django-glue-0.4.0/django_glue/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,23 @@
     def unique_name(self) -> str:
         return self.data['unique_name']
 
 
 @dataclass
 class GlueContextData:
     connection: GlueConnection
-    access: GlueAccess
-    fields: dict[GlueModelFieldData]
-    methods: list[str]
+    access: GlueAccess = None
+    fields: dict[GlueModelFieldData] = None
+    methods: list[str] = None
 
     def to_dict(self) -> dict:
         return asdict(self)
 
 
+
 @dataclass
 class GlueJsonData:
     fields: Optional[dict] = None
     simple_fields: Optional[dict] = None
     method_return: Optional[Any] = None
     custom: Optional[dict] = None
 
@@ -85,18 +86,19 @@
 
     def to_dict(self) -> dict:
         return asdict(self)
 
 
 @dataclass
 class GlueMetaData:
-    app_label: str
-    model: str
+    app_label: str = None
+    model: str = None
     object_pk: int = None
     query_set_str: str = None
+    template: str = None
     fields: Union[list, tuple] = None
     exclude: Union[list, tuple] = None
     methods: Union[list, tuple] = None
 
     @property
     def model_class(self):
         return ContentType.objects.get_by_natural_key(self.app_label, self.model).model_class()
```

### Comparing `django-glue-0.3.0/django_glue/enums.py` & `django-glue-0.4.0/django_glue/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         elif self.value == 'method':
             return GlueAccess.VIEW
 
 
 class GlueConnection(str, Enum):
     MODEL_OBJECT = 'model_object'
     QUERY_SET = 'query_set'
+    TEMPLATE = 'template'
 
     def __str__(self):
         return self.value
 
 
 class GlueJsonResponseType(str, Enum):
     SUCCESS = 'success'
```

### Comparing `django-glue-0.3.0/django_glue/glue.py` & `django-glue-0.4.0/django_glue/glue.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 
 from django_glue.sessions import GlueSession, GlueKeepLiveSession
 
 
 def add_glue(
         request: HttpRequest,
         unique_name: str,
-        target: Union[Model, QuerySet],
+        target: Union[Model, QuerySet, str],
         access: str = 'view',
         fields: Union[list, tuple] = ('__all__',),
         exclude: Union[list, tuple] = ('__none__',),
         methods: Union[list, tuple] = ('__none__',),
 ) -> None:
     if isinstance(fields, (list, tuple)) and isinstance(exclude, (list, tuple)):
         glue_session = GlueSession(request)
 
         if isinstance(target, Model):
             glue_session.add_model_object(unique_name, target, access, fields, exclude, methods)
 
         elif isinstance(target, QuerySet):
             glue_session.add_query_set(unique_name, target, access, fields, exclude, methods)
 
+        elif isinstance(target, str):
+            glue_session.add_template(unique_name, target)
+
         else:
             raise f'target is not a valid type must be a django.db.models.Model or django.db.models.query.QuerySet'
 
         glue_keep_live_session = GlueKeepLiveSession(request)
 
         glue_keep_live_session.set_unique_name(unique_name)
```

### Comparing `django-glue-0.3.0/django_glue/handlers.py` & `django-glue-0.4.0/django_glue/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging, json
 
 from django_glue.services import GlueModelObjectService, GlueQuerySetService
 from django_glue.responses import generate_json_404_response
+from django_glue.services.templates import GlueTemplateService
 from django_glue.sessions import GlueSession
 from django_glue.data_classes import GlueMetaData, GlueBodyData
 from django_glue.enums import GlueConnection, GlueAccess
 
 
 class GlueDataRequestHandler:
     def __init__(self, request):
         self.request = request
 
         self.is_valid_request = True
 
-        if request.content_type == 'application/json':
+        if request.content_type == 'application/json' or request.content_type == 'text/html':
             logging.warning(request.body.decode('utf-8'))
             self.body_data = GlueBodyData(request.body)
         else:
             self.is_valid_request = False
 
         self.unique_name = self.body_data['unique_name']
 
@@ -31,16 +32,14 @@
                 **self.glue_session['meta'][self.unique_name]
             )
 
             self.connection = GlueConnection(self.context[self.unique_name]['connection'])
 
             self.access = GlueAccess(self.context[self.unique_name]['access'])
 
-            self.model_class = self.meta_data.model_class
-
         else:
             self.is_valid_request = False
 
         logging.warning(f'{self.is_valid_request = }')
 
     def process_response(self):
         if self.method == 'QUERY' and self.is_valid_request:
@@ -56,12 +55,20 @@
                 glue_query_set_service = GlueQuerySetService(
                     self.meta_data,
                 )
 
                 json_response_data = glue_query_set_service.process_body_data(self.access, self.body_data)
                 return json_response_data.to_django_json_response()
 
+            elif self.connection == GlueConnection.TEMPLATE:
+                glue_template_service = GlueTemplateService(
+                    self.meta_data,
+                )
+
+                html_response_data = glue_template_service.process_body_data(self.access, self.body_data)
+                return html_response_data
+
             else:
                 return generate_json_404_response()
 
         else:
             return generate_json_404_response()
```

### Comparing `django-glue-0.3.0/django_glue/middleware.py` & `django-glue-0.4.0/django_glue/middleware.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue/responses.py` & `django-glue-0.4.0/django_glue/responses.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue/services/model_objects.py` & `django-glue-0.4.0/django_glue/services/model_objects.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue/services/query_sets.py` & `django-glue-0.4.0/django_glue/services/query_sets.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue/sessions.py` & `django-glue-0.4.0/django_glue/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,33 @@
         ))
 
         self.set_modified()
 
     def add_context(self, unique_name, context_data: GlueContextData) -> None:
         self.session['context'][unique_name] = context_data.to_dict()
 
+    def add_template(
+            self,
+            unique_name: str,
+            template,
+    ):
+
+        self.check_unique_name(unique_name)
+
+        self.add_context(unique_name, GlueContextData(
+            connection=GlueConnection('template'),
+            access=GlueAccess('view'),
+        ))
+
+        self.add_meta(unique_name, GlueMetaData(
+            template=template,
+        ))
+
+        self.set_modified()
+
     def add_meta(self, unique_name, meta_data: GlueMetaData) -> None:
         self.session['meta'][unique_name] = meta_data.to_dict()
 
     def check_unique_name(self, unique_name):
         if self.unique_name_unused(unique_name):
             self.purge_unique_name(unique_name)
```

### Comparing `django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_model_object.js` & `django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,77 +1,62 @@
 class GlueModelObject {
-    constructor(unique_name, load_values = true) {
+    constructor(unique_name) {
         this.unique_name = unique_name
-        this.context_data = null
-
-        console.log(DJANGO_GLUE_CONTEXT_DATA)
-
-        if (unique_name in DJANGO_GLUE_CONTEXT_DATA) {
-            this.context_data = DJANGO_GLUE_CONTEXT_DATA[unique_name]
-            this.load_fields(load_values)
-        } else {
-            console.error('"' + unique_name + '" is and invalid glue unique name.')
+        this.context_data = {
+            fields: {}
         }
     }
 
-    load_fields(load_values = true) {
-        if (load_values) {
-            this.load_values()
-        } else {
-            for (let key in this.context_data.fields) {
-                this[key] = ''
-            }
-        }
-    }
-
-    load_values() {
+    generate_field_data() {
+        let data = {}
         for (let key in this.context_data.fields) {
-            this[key] = this.context_data.fields[key].value
+            data[key] = this[key]
         }
+        return data
     }
 
-    get() {
-        glue_ajax_request(
+    async get(load_value = true) {
+        await glue_ajax_request(
             this.unique_name,
             'get'
         ).then((response) => {
             console.log(response)
             let simple_fields = response.data.simple_fields
             for (let key in simple_fields) {
-                this[key] = simple_fields[key]
+                if (load_value) {
+                    this[key] = simple_fields[key]
+                } else {
+                    this[key] = null
+                }
+
+                this.context_data.fields[key] = simple_fields[key]
             }
         })
     }
 
-    update(field = null) {
+    async update(field = null) {
         let data = {}
 
         if (field) {
             data[field] = this[field]
         } else {
-            for (let key in this.context_data.fields) {
-                data[key] = this[key]
-            }
+            data = this.generate_field_data()
         }
 
-        glue_ajax_request(
+        await glue_ajax_request(
             this.unique_name,
             'update',
             data
         ).then((response) => {
             console.log(response)
         })
     }
 
     async create() {
-        let data = {}
-
-        for (let key in this.context_data.fields) {
-            data[key] = this[key]
-        }
+        let data = this.generate_field_data()
 
         return await glue_ajax_request(
             this.unique_name,
             'create',
             data
         ).then((response) => {
             console.log(response)
```

### Comparing `django-glue-0.3.0/django_glue/static/django_glue/js/django_glue_query_set.js` & `django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,12 @@
 class GlueQuerySet {
     constructor(unique_name) {
         this.unique_name = unique_name
-        this.context_data = null
-        if (unique_name in DJANGO_GLUE_CONTEXT_DATA) {
-            this.context_data = DJANGO_GLUE_CONTEXT_DATA[unique_name]
-            if (this.context_data.connection !== 'query_set') {
-                console.error('"' + unique_name + '" is not a query set')
-            }
-        } else {
-            console.error('"' + unique_name + '" is and invalid glue unique name.')
+        this.context_data = {
+            fields: []
         }
     }
 
     async get(id) {
         let model_object_list = []
         let model_object = null
         return await glue_ajax_request(this.unique_name, 'get', {
```

### Comparing `django-glue-0.3.0/django_glue/templatetags/django_glue.py` & `django-glue-0.4.0/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue/utils.py` & `django-glue-0.4.0/django_glue/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/django_glue.egg-info/PKG-INFO` & `django-glue-0.4.0/django_glue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.3.0
+Version: 0.4.0
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.3.0/django_glue.egg-info/SOURCES.txt` & `django-glue-0.4.0/django_glue.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -28,19 +28,25 @@
 django_glue.egg-info/top_level.txt
 django_glue/core/__init__.py
 django_glue/core/utils.py
 django_glue/services/__init__.py
 django_glue/services/model_objects.py
 django_glue/services/query_sets.py
 django_glue/services/services.py
+django_glue/services/templates.py
 django_glue/static/django_glue/js/django_glue_ajax.js
 django_glue/static/django_glue/js/django_glue_csrf.js
+django_glue/static/django_glue/js/django_glue_event.js
+django_glue/static/django_glue/js/django_glue_message.js
 django_glue/static/django_glue/js/django_glue_model_object.js
 django_glue/static/django_glue/js/django_glue_query_set.js
 django_glue/static/django_glue/js/django_glue_response.js
+django_glue/static/django_glue/js/django_glue_shortcuts.js
+django_glue/static/django_glue/js/django_glue_template.js
+django_glue/static/django_glue/js/django_glue_view.js
 django_glue/templates/django_glue/django_glue.html
 django_glue/templatetags/__init__.py
 django_glue/templatetags/django_glue.py
 tests/__init__.py
 tests/admin.py
 tests/manage.py
 tests/models.py
```

### Comparing `django-glue-0.3.0/setup.py` & `django-glue-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/tests/manage.py` & `django-glue-0.4.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/tests/migrations/0001_initial.py` & `django-glue-0.4.0/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/tests/models.py` & `django-glue-0.4.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/tests/settings.py` & `django-glue-0.4.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.3.0/tests/utils.py` & `django-glue-0.4.0/tests/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,56 +26,77 @@
     'Waldern',
     'Howery',
     'Wilson',
     'Sauer',
 )
 
 DESCRIPTION_WORD_TUPLE = (
-    'I',
     'a',
-    'are'
+    'are',
     'artsy',
     'awesome',
+    'balloon',
     'boring',
     'can',
     'cat',
     'cool',
+    'dripping',
     'dog',
+    'eggs',
+    'extra',
     'fast',
     'finished',
     'fly',
+    'goal',
+    'graduated',
     'handy',
     'has',
     'has',
     'have',
+    'how',
+    'I',
     'it',
+    'junk',
+    'killer',
     'loves cars',
+    'mother',
+    'missle',
     'need',
+    'opposite',
+    'panther',
+    'quiz',
+    'rugged',
     'she',
     'started',
     'stupid',
     'taco',
+    'that',
+    'then',
     'there',
     'to',
     'ugly',
+    'vixen',
     'want',
     'when',
+    'where',
     'when',
-    'wood carving'
+    'wood carving',
+    'xavier',
     'you',
+    'zebra',
 )
 
 
 def custom_test_function(request):
     return 'Hello World'
 
 
 def generate_randomized_test_model(limit=5):
     new_description = ''
-    for x in range(10):
+    for x in range(20):
         new_description += f'{DESCRIPTION_WORD_TUPLE[random.randint(0, (len(DESCRIPTION_WORD_TUPLE) - 1))]} '
 
     test_model_object = TestModel.objects.create(
         first_name=FIRST_NAME_TUPLE[random.randint(0, (len(FIRST_NAME_TUPLE) - 1))],
         last_name=LAST_NAME_TUPLE[random.randint(0, (len(LAST_NAME_TUPLE) - 1))],
         description=new_description,
         favorite_number=random.randint(0, 999),
```

