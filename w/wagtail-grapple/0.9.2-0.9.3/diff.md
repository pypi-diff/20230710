# Comparing `tmp/wagtail-grapple-0.9.2.tar.gz` & `tmp/wagtail-grapple-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-grapple-0.9.2.tar", last modified: Thu Nov 12 15:53:05 2020, max compression
+gzip compressed data, was "dist/wagtail-grapple-0.9.3.tar", last modified: Tue Dec  8 19:04:11 2020, max compression
```

## Comparing `wagtail-grapple-0.9.2.tar` & `wagtail-grapple-0.9.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/
--rw-r--r--   0 dan        (502) staff       (20)     1073 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/LICENCE.txt
--rw-r--r--   0 dan        (502) staff       (20)      184 2020-08-18 19:04:15.000000 wagtail-grapple-0.9.2/MANIFEST.in
--rw-r--r--   0 dan        (502) staff       (20)    14870 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)    11935 2020-11-12 15:48:58.000000 wagtail-grapple-0.9.2/README.md
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/grapple/
--rw-r--r--   0 dan        (502) staff       (20)       67 2020-11-12 15:49:30.000000 wagtail-grapple-0.9.2/grapple/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)    17506 2020-11-12 15:49:06.000000 wagtail-grapple-0.9.2/grapple/actions.py
--rw-r--r--   0 dan        (502) staff       (20)      492 2020-08-18 19:04:15.000000 wagtail-grapple-0.9.2/grapple/apps.py
--rw-r--r--   0 dan        (502) staff       (20)      172 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/grapple/asgi.py
--rw-r--r--   0 dan        (502) staff       (20)     9447 2020-10-26 23:44:43.000000 wagtail-grapple-0.9.2/grapple/helpers.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/grapple/migrations/
--rw-r--r--   0 dan        (502) staff       (20)     1141 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/grapple/migrations/0001_initial.py
--rw-r--r--   0 dan        (502) staff       (20)      236 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/grapple/migrations/0002_delete_pagepreview.py
--rw-r--r--   0 dan        (502) staff       (20)      678 2020-08-01 15:31:55.000000 wagtail-grapple-0.9.2/grapple/migrations/0003_stubmodel.py
--rw-r--r--   0 dan        (502) staff       (20)      290 2020-11-06 10:58:28.000000 wagtail-grapple-0.9.2/grapple/migrations/0004_delete_stubmodel.py
--rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/grapple/migrations/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)     5958 2020-10-20 21:22:14.000000 wagtail-grapple-0.9.2/grapple/models.py
--rw-r--r--   0 dan        (502) staff       (20)     1547 2020-10-25 22:30:25.000000 wagtail-grapple-0.9.2/grapple/registry.py
--rw-r--r--   0 dan        (502) staff       (20)     1623 2020-10-20 19:46:37.000000 wagtail-grapple-0.9.2/grapple/schema.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/grapple/templates/
--rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/grapple/templates/__init__.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/grapple/templates/grapple/
--rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/grapple/templates/grapple/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)     4298 2020-09-02 14:43:03.000000 wagtail-grapple-0.9.2/grapple/templates/grapple/graphiql.html
--rw-r--r--   0 dan        (502) staff       (20)      194 2020-08-18 19:04:15.000000 wagtail-grapple-0.9.2/grapple/templates/grapple/preview.html
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/grapple/templates/wagtailcore/
--rw-r--r--   0 dan        (502) staff       (20)       16 2020-08-10 20:55:13.000000 wagtail-grapple-0.9.2/grapple/templates/wagtailcore/richtext.html
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/grapple/types/
--rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/grapple/types/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)     1512 2020-10-25 22:40:23.000000 wagtail-grapple-0.9.2/grapple/types/collections.py
--rw-r--r--   0 dan        (502) staff       (20)     2609 2020-10-25 22:32:43.000000 wagtail-grapple-0.9.2/grapple/types/documents.py
--rw-r--r--   0 dan        (502) staff       (20)     4952 2020-10-26 22:48:15.000000 wagtail-grapple-0.9.2/grapple/types/images.py
--rw-r--r--   0 dan        (502) staff       (20)     1826 2020-10-25 22:32:34.000000 wagtail-grapple-0.9.2/grapple/types/media.py
--rw-r--r--   0 dan        (502) staff       (20)     9401 2020-10-19 15:02:18.000000 wagtail-grapple-0.9.2/grapple/types/pages.py
--rw-r--r--   0 dan        (502) staff       (20)     1162 2020-09-09 14:57:31.000000 wagtail-grapple-0.9.2/grapple/types/redirects.py
--rw-r--r--   0 dan        (502) staff       (20)     1401 2020-10-19 20:58:28.000000 wagtail-grapple-0.9.2/grapple/types/search.py
--rw-r--r--   0 dan        (502) staff       (20)     1293 2020-08-01 15:31:55.000000 wagtail-grapple-0.9.2/grapple/types/settings.py
--rw-r--r--   0 dan        (502) staff       (20)     1947 2020-10-07 10:55:56.000000 wagtail-grapple-0.9.2/grapple/types/sites.py
--rw-r--r--   0 dan        (502) staff       (20)      767 2020-10-25 22:50:51.000000 wagtail-grapple-0.9.2/grapple/types/snippets.py
--rw-r--r--   0 dan        (502) staff       (20)    14265 2020-11-06 11:50:42.000000 wagtail-grapple-0.9.2/grapple/types/streamfield.py
--rw-r--r--   0 dan        (502) staff       (20)     7070 2020-10-26 23:44:52.000000 wagtail-grapple-0.9.2/grapple/types/structures.py
--rw-r--r--   0 dan        (502) staff       (20)     1201 2020-10-19 13:20:49.000000 wagtail-grapple-0.9.2/grapple/types/tags.py
--rw-r--r--   0 dan        (502) staff       (20)     1323 2020-09-02 14:43:03.000000 wagtail-grapple-0.9.2/grapple/urls.py
--rw-r--r--   0 dan        (502) staff       (20)     5589 2020-10-26 23:45:13.000000 wagtail-grapple-0.9.2/grapple/utils.py
--rw-r--r--   0 dan        (502) staff       (20)     1047 2020-10-25 22:30:25.000000 wagtail-grapple-0.9.2/grapple/wagtail_hooks.py
--rw-r--r--   0 dan        (502) staff       (20)      268 2020-11-12 15:48:58.000000 wagtail-grapple-0.9.2/requirements-channels.txt
--rw-r--r--   0 dan        (502) staff       (20)      226 2020-11-04 14:58:56.000000 wagtail-grapple-0.9.2/requirements.txt
--rw-r--r--   0 dan        (502) staff       (20)     1203 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/setup.cfg
--rw-r--r--   0 dan        (502) staff       (20)       38 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.2/setup.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/wagtail_grapple.egg-info/
--rwxr-xr-x   0 dan        (502) staff       (20)    14870 2020-11-12 15:53:04.000000 wagtail-grapple-0.9.2/wagtail_grapple.egg-info/PKG-INFO
--rwxr-xr-x   0 dan        (502) staff       (20)     1234 2020-11-12 15:53:05.000000 wagtail-grapple-0.9.2/wagtail_grapple.egg-info/SOURCES.txt
--rwxr-xr-x   0 dan        (502) staff       (20)        1 2020-11-12 15:53:04.000000 wagtail-grapple-0.9.2/wagtail_grapple.egg-info/dependency_links.txt
--rwxr-xr-x   0 dan        (502) staff       (20)      182 2020-11-12 15:53:04.000000 wagtail-grapple-0.9.2/wagtail_grapple.egg-info/requires.txt
--rwxr-xr-x   0 dan        (502) staff       (20)        8 2020-11-12 15:53:04.000000 wagtail-grapple-0.9.2/wagtail_grapple.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/
+-rw-r--r--   0 dan        (502) staff       (20)     1073 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/LICENCE.txt
+-rw-r--r--   0 dan        (502) staff       (20)      184 2020-08-18 19:04:15.000000 wagtail-grapple-0.9.3/MANIFEST.in
+-rw-r--r--   0 dan        (502) staff       (20)    14870 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)    11935 2020-11-12 15:48:58.000000 wagtail-grapple-0.9.3/README.md
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/grapple/
+-rw-r--r--   0 dan        (502) staff       (20)       67 2020-12-08 19:02:29.000000 wagtail-grapple-0.9.3/grapple/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)    17506 2020-11-12 15:49:06.000000 wagtail-grapple-0.9.3/grapple/actions.py
+-rw-r--r--   0 dan        (502) staff       (20)      492 2020-08-18 19:04:15.000000 wagtail-grapple-0.9.3/grapple/apps.py
+-rw-r--r--   0 dan        (502) staff       (20)      172 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/grapple/asgi.py
+-rw-r--r--   0 dan        (502) staff       (20)     9446 2020-12-08 18:53:24.000000 wagtail-grapple-0.9.3/grapple/helpers.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/grapple/migrations/
+-rw-r--r--   0 dan        (502) staff       (20)     1141 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/grapple/migrations/0001_initial.py
+-rw-r--r--   0 dan        (502) staff       (20)      236 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/grapple/migrations/0002_delete_pagepreview.py
+-rw-r--r--   0 dan        (502) staff       (20)      678 2020-08-01 15:31:55.000000 wagtail-grapple-0.9.3/grapple/migrations/0003_stubmodel.py
+-rw-r--r--   0 dan        (502) staff       (20)      290 2020-11-06 10:58:28.000000 wagtail-grapple-0.9.3/grapple/migrations/0004_delete_stubmodel.py
+-rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/grapple/migrations/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)     5849 2020-12-08 18:31:57.000000 wagtail-grapple-0.9.3/grapple/models.py
+-rw-r--r--   0 dan        (502) staff       (20)     1547 2020-10-25 22:30:25.000000 wagtail-grapple-0.9.3/grapple/registry.py
+-rw-r--r--   0 dan        (502) staff       (20)     1623 2020-10-20 19:46:37.000000 wagtail-grapple-0.9.3/grapple/schema.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/grapple/templates/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/grapple/templates/__init__.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/grapple/templates/grapple/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/grapple/templates/grapple/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)     4298 2020-09-02 14:43:03.000000 wagtail-grapple-0.9.3/grapple/templates/grapple/graphiql.html
+-rw-r--r--   0 dan        (502) staff       (20)      194 2020-08-18 19:04:15.000000 wagtail-grapple-0.9.3/grapple/templates/grapple/preview.html
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/grapple/templates/wagtailcore/
+-rw-r--r--   0 dan        (502) staff       (20)       16 2020-08-10 20:55:13.000000 wagtail-grapple-0.9.3/grapple/templates/wagtailcore/richtext.html
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/grapple/types/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/grapple/types/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)     1512 2020-10-25 22:40:23.000000 wagtail-grapple-0.9.3/grapple/types/collections.py
+-rw-r--r--   0 dan        (502) staff       (20)     2609 2020-10-25 22:32:43.000000 wagtail-grapple-0.9.3/grapple/types/documents.py
+-rw-r--r--   0 dan        (502) staff       (20)     4952 2020-10-26 22:48:15.000000 wagtail-grapple-0.9.3/grapple/types/images.py
+-rw-r--r--   0 dan        (502) staff       (20)     1826 2020-10-25 22:32:34.000000 wagtail-grapple-0.9.3/grapple/types/media.py
+-rw-r--r--   0 dan        (502) staff       (20)     9401 2020-10-19 15:02:18.000000 wagtail-grapple-0.9.3/grapple/types/pages.py
+-rw-r--r--   0 dan        (502) staff       (20)     1162 2020-09-09 14:57:31.000000 wagtail-grapple-0.9.3/grapple/types/redirects.py
+-rw-r--r--   0 dan        (502) staff       (20)     1401 2020-10-19 20:58:28.000000 wagtail-grapple-0.9.3/grapple/types/search.py
+-rw-r--r--   0 dan        (502) staff       (20)     1293 2020-08-01 15:31:55.000000 wagtail-grapple-0.9.3/grapple/types/settings.py
+-rw-r--r--   0 dan        (502) staff       (20)     1947 2020-10-07 10:55:56.000000 wagtail-grapple-0.9.3/grapple/types/sites.py
+-rw-r--r--   0 dan        (502) staff       (20)      767 2020-10-25 22:50:51.000000 wagtail-grapple-0.9.3/grapple/types/snippets.py
+-rw-r--r--   0 dan        (502) staff       (20)    14265 2020-11-06 11:50:42.000000 wagtail-grapple-0.9.3/grapple/types/streamfield.py
+-rw-r--r--   0 dan        (502) staff       (20)     7070 2020-10-26 23:44:52.000000 wagtail-grapple-0.9.3/grapple/types/structures.py
+-rw-r--r--   0 dan        (502) staff       (20)     1201 2020-10-19 13:20:49.000000 wagtail-grapple-0.9.3/grapple/types/tags.py
+-rw-r--r--   0 dan        (502) staff       (20)     1323 2020-09-02 14:43:03.000000 wagtail-grapple-0.9.3/grapple/urls.py
+-rw-r--r--   0 dan        (502) staff       (20)     5589 2020-10-26 23:45:13.000000 wagtail-grapple-0.9.3/grapple/utils.py
+-rw-r--r--   0 dan        (502) staff       (20)     1047 2020-10-25 22:30:25.000000 wagtail-grapple-0.9.3/grapple/wagtail_hooks.py
+-rw-r--r--   0 dan        (502) staff       (20)      268 2020-11-12 15:48:58.000000 wagtail-grapple-0.9.3/requirements-channels.txt
+-rw-r--r--   0 dan        (502) staff       (20)      226 2020-11-04 14:58:56.000000 wagtail-grapple-0.9.3/requirements.txt
+-rw-r--r--   0 dan        (502) staff       (20)     1203 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/setup.cfg
+-rw-r--r--   0 dan        (502) staff       (20)       38 2019-11-27 17:17:11.000000 wagtail-grapple-0.9.3/setup.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2020-12-08 19:04:11.000000 wagtail-grapple-0.9.3/wagtail_grapple.egg-info/
+-rwxr-xr-x   0 dan        (502) staff       (20)    14870 2020-12-08 19:04:10.000000 wagtail-grapple-0.9.3/wagtail_grapple.egg-info/PKG-INFO
+-rwxr-xr-x   0 dan        (502) staff       (20)     1234 2020-12-08 19:04:10.000000 wagtail-grapple-0.9.3/wagtail_grapple.egg-info/SOURCES.txt
+-rwxr-xr-x   0 dan        (502) staff       (20)        1 2020-12-08 19:04:10.000000 wagtail-grapple-0.9.3/wagtail_grapple.egg-info/dependency_links.txt
+-rwxr-xr-x   0 dan        (502) staff       (20)      182 2020-12-08 19:04:10.000000 wagtail-grapple-0.9.3/wagtail_grapple.egg-info/requires.txt
+-rwxr-xr-x   0 dan        (502) staff       (20)        8 2020-12-08 19:04:10.000000 wagtail-grapple-0.9.3/wagtail_grapple.egg-info/top_level.txt
```

### Comparing `wagtail-grapple-0.9.2/LICENCE.txt` & `wagtail-grapple-0.9.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/PKG-INFO` & `wagtail-grapple-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-grapple
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Django app that speeds up and simplifies implementing a GraphQL endpoint!
 Home-page: https://github.com/GrappleGQL/wagtail-grapple
 Author: Nathan Horrigan
 Author-email: nathan.horrigan@torchbox.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/GrappleGQL/wagtail-grapple">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-grapple Version: 0.9.2 Summary: A Django
+Metadata-Version: 2.1 Name: wagtail-grapple Version: 0.9.3 Summary: A Django
 app that speeds up and simplifies implementing a GraphQL endpoint! Home-page:
 https://github.com/GrappleGQL/wagtail-grapple Author: Nathan Horrigan Author-
 email: nathan.horrigan@torchbox.com License: UNKNOWN Description:
                          [A_red_g_with_a_grapple_hook]
    **** Wagtail Grapple [https://img.shields.io/pypi/v/wagtail-grapple.svg]
     [https://img.shields.io/badge/code%20style-black-000000.svg] [https://
         img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-
```

### Comparing `wagtail-grapple-0.9.2/README.md` & `wagtail-grapple-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/actions.py` & `wagtail-grapple-0.9.3/grapple/actions.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/helpers.py` & `wagtail-grapple-0.9.3/grapple/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
                         if "token" in kwargs and hasattr(
                             cls, "get_page_from_preview_token"
                         ):
                             return cls.get_page_from_preview_token(kwargs["token"])
 
                         return qs.live().public().filter(**kwargs).first()
 
-                    return cls.filter(**kwargs).first()
+                    return qs.filter(**kwargs).first()
                 except:
                     return None
 
             # Create schema and add resolve methods
             schema = type(cls.__name__ + "Query", (), {})
 
             singular_field_type = field_type
```

### Comparing `wagtail-grapple-0.9.2/grapple/migrations/0001_initial.py` & `wagtail-grapple-0.9.3/grapple/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/migrations/0003_stubmodel.py` & `wagtail-grapple-0.9.3/grapple/migrations/0003_stubmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/models.py` & `wagtail-grapple-0.9.3/grapple/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,28 +110,27 @@
 
         return GraphQLField(field_name, get_image_type, **kwargs)
 
     return Mixin
 
 
 def GraphQLDocument(field_name: str, **kwargs):
-    from django.conf import settings
+    def Mixin():
+        from .types.documents import get_document_type
 
-    document_type = "wagtaildocs.Document"
-    if hasattr(settings, "WAGTAILDOCS_DOCUMENT_MODEL"):
-        document_type = settings["WAGTAILDOCS_DOCUMENT_MODEL"]
+        return GraphQLField(field_name, get_document_type, **kwargs)
 
-    return GraphQLForeignKey(field_name, document_type, **kwargs)
+    return Mixin
 
 
 def GraphQLMedia(field_name: str, **kwargs):
     def Mixin():
-        from .types.media import MediaObjectType
+        from .types.media import get_media_type
 
-        return GraphQLField(field_name, MediaObjectType, **kwargs)
+        return GraphQLField(field_name, get_media_type, **kwargs)
 
     return Mixin
 
 
 def GraphQLPage(field_name: str, **kwargs):
     def Mixin():
         from .types.pages import PageInterface
```

### Comparing `wagtail-grapple-0.9.2/grapple/registry.py` & `wagtail-grapple-0.9.3/grapple/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/schema.py` & `wagtail-grapple-0.9.3/grapple/schema.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/templates/grapple/graphiql.html` & `wagtail-grapple-0.9.3/grapple/templates/grapple/graphiql.html`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/collections.py` & `wagtail-grapple-0.9.3/grapple/types/collections.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/documents.py` & `wagtail-grapple-0.9.3/grapple/types/documents.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/images.py` & `wagtail-grapple-0.9.3/grapple/types/images.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/media.py` & `wagtail-grapple-0.9.3/grapple/types/media.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/pages.py` & `wagtail-grapple-0.9.3/grapple/types/pages.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/redirects.py` & `wagtail-grapple-0.9.3/grapple/types/redirects.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/search.py` & `wagtail-grapple-0.9.3/grapple/types/search.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/settings.py` & `wagtail-grapple-0.9.3/grapple/types/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/sites.py` & `wagtail-grapple-0.9.3/grapple/types/sites.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/snippets.py` & `wagtail-grapple-0.9.3/grapple/types/snippets.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/streamfield.py` & `wagtail-grapple-0.9.3/grapple/types/streamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/structures.py` & `wagtail-grapple-0.9.3/grapple/types/structures.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/types/tags.py` & `wagtail-grapple-0.9.3/grapple/types/tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/urls.py` & `wagtail-grapple-0.9.3/grapple/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/utils.py` & `wagtail-grapple-0.9.3/grapple/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/grapple/wagtail_hooks.py` & `wagtail-grapple-0.9.3/grapple/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/setup.cfg` & `wagtail-grapple-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtail-grapple-0.9.2/wagtail_grapple.egg-info/PKG-INFO` & `wagtail-grapple-0.9.3/wagtail_grapple.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-grapple
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Django app that speeds up and simplifies implementing a GraphQL endpoint!
 Home-page: https://github.com/GrappleGQL/wagtail-grapple
 Author: Nathan Horrigan
 Author-email: nathan.horrigan@torchbox.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/GrappleGQL/wagtail-grapple">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-grapple Version: 0.9.2 Summary: A Django
+Metadata-Version: 2.1 Name: wagtail-grapple Version: 0.9.3 Summary: A Django
 app that speeds up and simplifies implementing a GraphQL endpoint! Home-page:
 https://github.com/GrappleGQL/wagtail-grapple Author: Nathan Horrigan Author-
 email: nathan.horrigan@torchbox.com License: UNKNOWN Description:
                          [A_red_g_with_a_grapple_hook]
    **** Wagtail Grapple [https://img.shields.io/pypi/v/wagtail-grapple.svg]
     [https://img.shields.io/badge/code%20style-black-000000.svg] [https://
         img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-
```

### Comparing `wagtail-grapple-0.9.2/wagtail_grapple.egg-info/SOURCES.txt` & `wagtail-grapple-0.9.3/wagtail_grapple.egg-info/SOURCES.txt`

 * *Files identical despite different names*

