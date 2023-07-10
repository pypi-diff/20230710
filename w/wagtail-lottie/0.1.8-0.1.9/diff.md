# Comparing `tmp/wagtail_lottie-0.1.8.tar.gz` & `tmp/wagtail_lottie-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_lottie-0.1.8.tar", last modified: Thu Dec  2 16:26:02 2021, max compression
+gzip compressed data, was "wagtail_lottie-0.1.9.tar", last modified: Thu Dec  2 16:49:18 2021, max compression
```

## Comparing `wagtail_lottie-0.1.8.tar` & `wagtail_lottie-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2021-11-25 10:44:58.000000 wagtail_lottie-0.1.8/LICENSE
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      137 2021-11-28 16:36:58.000000 wagtail_lottie-0.1.8/MANIFEST.in
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3460 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2732 2021-11-29 13:20:59.000000 wagtail_lottie-0.1.8/README.rst
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/app/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.8/app/__init__.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/app/migrations/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      604 2021-11-25 11:01:24.000000 wagtail_lottie-0.1.8/app/migrations/0001_initial.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1740 2021-11-25 12:59:47.000000 wagtail_lottie-0.1.8/app/migrations/0002_create_homepage.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1008 2021-11-28 16:41:07.000000 wagtail_lottie-0.1.8/app/migrations/0003_auto_20211128_1641.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 11:01:24.000000 wagtail_lottie-0.1.8/app/migrations/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      934 2021-11-28 16:30:46.000000 wagtail_lottie-0.1.8/app/models.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/app/settings/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.8/app/settings/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     4501 2021-11-29 17:51:59.000000 wagtail_lottie-0.1.8/app/settings/base.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      461 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.8/app/settings/dev.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       95 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.8/app/settings/production.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1153 2021-11-25 10:54:50.000000 wagtail_lottie-0.1.8/app/urls.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      387 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.8/app/wsgi.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/setup.cfg
--rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1230 2021-11-28 18:20:25.000000 wagtail_lottie-0.1.8/setup.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/wagtail_lottie/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       63 2021-11-25 16:01:43.000000 wagtail_lottie-0.1.8/wagtail_lottie/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      480 2021-11-26 13:51:01.000000 wagtail_lottie-0.1.8/wagtail_lottie/admin.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      159 2021-11-25 11:11:13.000000 wagtail_lottie-0.1.8/wagtail_lottie/apps.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1611 2021-12-02 16:25:35.000000 wagtail_lottie-0.1.8/wagtail_lottie/blocks.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      208 2021-11-26 10:45:42.000000 wagtail_lottie-0.1.8/wagtail_lottie/constants.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      404 2021-11-26 14:35:52.000000 wagtail_lottie-0.1.8/wagtail_lottie/exceptions.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1554 2021-11-30 13:12:27.000000 wagtail_lottie-0.1.8/wagtail_lottie/lottie_zip_file.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/wagtail_lottie/migrations/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2511 2021-11-28 16:41:07.000000 wagtail_lottie-0.1.8/wagtail_lottie/migrations/0001_initial.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 11:11:13.000000 wagtail_lottie-0.1.8/wagtail_lottie/migrations/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3043 2021-11-29 17:54:14.000000 wagtail_lottie-0.1.8/wagtail_lottie/models.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/wagtail_lottie/static/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/wagtail_lottie/static/wagtail_lottie/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1257 2021-11-28 16:36:58.000000 wagtail_lottie-0.1.8/wagtail_lottie/static/wagtail_lottie/lottie-animation.js
--rw-rw-r--   0 ariane    (1000) ariane    (1000)   262029 2021-11-24 14:37:42.000000 wagtail_lottie-0.1.8/wagtail_lottie/static/wagtail_lottie/lottie-player.js
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/wagtail_lottie/templates/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/wagtail_lottie/templates/modeladmin/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/wagtail_lottie/templates/modeladmin/wagtail_lottie/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-05-14 09:29:32.000000 wagtail_lottie-0.1.8/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/create.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       36 2021-05-14 09:29:32.000000 wagtail_lottie-0.1.8/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/edit.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-11-25 12:53:12.000000 wagtail_lottie-0.1.8/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/index.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.968859 wagtail_lottie-0.1.8/wagtail_lottie/templates/wagtail_lottie/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/wagtail_lottie/templates/wagtail_lottie/homepage/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      270 2021-11-28 16:55:58.000000 wagtail_lottie-0.1.8/wagtail_lottie/templates/wagtail_lottie/homepage/site_summary_lottie_animation.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/wagtail_lottie/tests/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 16:01:48.000000 wagtail_lottie-0.1.8/wagtail_lottie/tests/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      136 2021-11-30 13:03:34.000000 wagtail_lottie-0.1.8/wagtail_lottie/tests/_constants.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2126 2021-12-02 16:19:37.000000 wagtail_lottie-0.1.8/wagtail_lottie/tests/test_admin_views.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      910 2021-11-30 13:04:04.000000 wagtail_lottie-0.1.8/wagtail_lottie/tests/test_lottie_zip_file.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2308 2021-11-29 17:52:58.000000 wagtail_lottie-0.1.8/wagtail_lottie/views.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1362 2021-11-26 14:25:17.000000 wagtail_lottie-0.1.8/wagtail_lottie/wagtail_hooks.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      336 2021-11-28 16:49:01.000000 wagtail_lottie-0.1.8/wagtail_lottie/widgets.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:26:02.972859 wagtail_lottie-0.1.8/wagtail_lottie.egg-info/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3460 2021-12-02 16:26:02.000000 wagtail_lottie-0.1.8/wagtail_lottie.egg-info/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1474 2021-12-02 16:26:02.000000 wagtail_lottie-0.1.8/wagtail_lottie.egg-info/SOURCES.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2021-12-02 16:26:02.000000 wagtail_lottie-0.1.8/wagtail_lottie.egg-info/dependency_links.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       31 2021-12-02 16:26:02.000000 wagtail_lottie-0.1.8/wagtail_lottie.egg-info/requires.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       19 2021-12-02 16:26:02.000000 wagtail_lottie-0.1.8/wagtail_lottie.egg-info/top_level.txt
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.374747 wagtail_lottie-0.1.9/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2021-11-25 10:44:58.000000 wagtail_lottie-0.1.9/LICENSE
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      137 2021-11-28 16:36:58.000000 wagtail_lottie-0.1.9/MANIFEST.in
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3460 2021-12-02 16:49:18.374747 wagtail_lottie-0.1.9/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2732 2021-11-29 13:20:59.000000 wagtail_lottie-0.1.9/README.rst
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/app/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.9/app/__init__.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/app/migrations/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      604 2021-11-25 11:01:24.000000 wagtail_lottie-0.1.9/app/migrations/0001_initial.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1740 2021-11-25 12:59:47.000000 wagtail_lottie-0.1.9/app/migrations/0002_create_homepage.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1008 2021-11-28 16:41:07.000000 wagtail_lottie-0.1.9/app/migrations/0003_auto_20211128_1641.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 11:01:24.000000 wagtail_lottie-0.1.9/app/migrations/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      934 2021-11-28 16:30:46.000000 wagtail_lottie-0.1.9/app/models.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/app/settings/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.9/app/settings/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     4501 2021-11-29 17:51:59.000000 wagtail_lottie-0.1.9/app/settings/base.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      461 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.9/app/settings/dev.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       95 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.9/app/settings/production.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1153 2021-11-25 10:54:50.000000 wagtail_lottie-0.1.9/app/urls.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      387 2021-11-25 10:52:26.000000 wagtail_lottie-0.1.9/app/wsgi.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-12-02 16:49:18.374747 wagtail_lottie-0.1.9/setup.cfg
+-rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1230 2021-11-28 18:20:25.000000 wagtail_lottie-0.1.9/setup.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       63 2021-11-25 16:01:43.000000 wagtail_lottie-0.1.9/wagtail_lottie/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      480 2021-11-26 13:51:01.000000 wagtail_lottie-0.1.9/wagtail_lottie/admin.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      159 2021-11-25 11:11:13.000000 wagtail_lottie-0.1.9/wagtail_lottie/apps.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1611 2021-12-02 16:25:35.000000 wagtail_lottie-0.1.9/wagtail_lottie/blocks.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      208 2021-11-26 10:45:42.000000 wagtail_lottie-0.1.9/wagtail_lottie/constants.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      404 2021-11-26 14:35:52.000000 wagtail_lottie-0.1.9/wagtail_lottie/exceptions.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1554 2021-11-30 13:12:27.000000 wagtail_lottie-0.1.9/wagtail_lottie/lottie_zip_file.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie/migrations/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2511 2021-11-28 16:41:07.000000 wagtail_lottie-0.1.9/wagtail_lottie/migrations/0001_initial.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 11:11:13.000000 wagtail_lottie-0.1.9/wagtail_lottie/migrations/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3043 2021-11-29 17:54:14.000000 wagtail_lottie-0.1.9/wagtail_lottie/models.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie/static/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie/static/wagtail_lottie/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1257 2021-11-28 16:36:58.000000 wagtail_lottie-0.1.9/wagtail_lottie/static/wagtail_lottie/lottie-animation.js
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)   262029 2021-11-24 14:37:42.000000 wagtail_lottie-0.1.9/wagtail_lottie/static/wagtail_lottie/lottie-player.js
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie/templates/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie/templates/modeladmin/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie/templates/modeladmin/wagtail_lottie/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.374747 wagtail_lottie-0.1.9/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-05-14 09:29:32.000000 wagtail_lottie-0.1.9/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/create.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       36 2021-05-14 09:29:32.000000 wagtail_lottie-0.1.9/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/edit.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-11-25 12:53:12.000000 wagtail_lottie-0.1.9/wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/index.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.374747 wagtail_lottie-0.1.9/wagtail_lottie/templates/wagtail_lottie/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.374747 wagtail_lottie-0.1.9/wagtail_lottie/templates/wagtail_lottie/homepage/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      270 2021-11-28 16:55:58.000000 wagtail_lottie-0.1.9/wagtail_lottie/templates/wagtail_lottie/homepage/site_summary_lottie_animation.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      312 2021-12-02 16:48:52.000000 wagtail_lottie-0.1.9/wagtail_lottie/templates/wagtail_lottie/lottie_animation.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.374747 wagtail_lottie-0.1.9/wagtail_lottie/tests/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-11-25 16:01:48.000000 wagtail_lottie-0.1.9/wagtail_lottie/tests/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      136 2021-11-30 13:03:34.000000 wagtail_lottie-0.1.9/wagtail_lottie/tests/_constants.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2126 2021-12-02 16:19:37.000000 wagtail_lottie-0.1.9/wagtail_lottie/tests/test_admin_views.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      910 2021-11-30 13:04:04.000000 wagtail_lottie-0.1.9/wagtail_lottie/tests/test_lottie_zip_file.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2308 2021-11-29 17:52:58.000000 wagtail_lottie-0.1.9/wagtail_lottie/views.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1362 2021-11-26 14:25:17.000000 wagtail_lottie-0.1.9/wagtail_lottie/wagtail_hooks.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      336 2021-11-28 16:49:01.000000 wagtail_lottie-0.1.9/wagtail_lottie/widgets.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-12-02 16:49:18.370747 wagtail_lottie-0.1.9/wagtail_lottie.egg-info/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3460 2021-12-02 16:49:18.000000 wagtail_lottie-0.1.9/wagtail_lottie.egg-info/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1536 2021-12-02 16:49:18.000000 wagtail_lottie-0.1.9/wagtail_lottie.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2021-12-02 16:49:18.000000 wagtail_lottie-0.1.9/wagtail_lottie.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       31 2021-12-02 16:49:18.000000 wagtail_lottie-0.1.9/wagtail_lottie.egg-info/requires.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       19 2021-12-02 16:49:18.000000 wagtail_lottie-0.1.9/wagtail_lottie.egg-info/top_level.txt
```

### Comparing `wagtail_lottie-0.1.8/LICENSE` & `wagtail_lottie-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/PKG-INFO` & `wagtail_lottie-0.1.9/wagtail_lottie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail_lottie
-Version: 0.1.8
+Name: wagtail-lottie
+Version: 0.1.9
 Summary: Wagtail Lottie
 Home-page: https://github.com/Aleksi44/wagtail-lottie
 Author: Alexis Le Baron
 Author-email: hello@snoweb.io
 License: GPL-3.0
 Keywords: wagtail lottie
 Platform: linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_lottie Version: 0.1.8 Summary: Wagtail
+Metadata-Version: 2.1 Name: wagtail-lottie Version: 0.1.9 Summary: Wagtail
 Lottie Home-page: https://github.com/Aleksi44/wagtail-lottie Author: Alexis Le
 Baron Author-email: hello@snoweb.io License: GPL-3.0 Keywords: wagtail lottie
 Platform: linux Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Operating System :: OS
```

### Comparing `wagtail_lottie-0.1.8/README.rst` & `wagtail_lottie-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/app/migrations/0001_initial.py` & `wagtail_lottie-0.1.9/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/app/migrations/0002_create_homepage.py` & `wagtail_lottie-0.1.9/app/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/app/migrations/0003_auto_20211128_1641.py` & `wagtail_lottie-0.1.9/app/migrations/0003_auto_20211128_1641.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/app/models.py` & `wagtail_lottie-0.1.9/app/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/app/settings/base.py` & `wagtail_lottie-0.1.9/app/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/app/urls.py` & `wagtail_lottie-0.1.9/app/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/setup.py` & `wagtail_lottie-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/blocks.py` & `wagtail_lottie-0.1.9/wagtail_lottie/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/lottie_zip_file.py` & `wagtail_lottie-0.1.9/wagtail_lottie/lottie_zip_file.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/migrations/0001_initial.py` & `wagtail_lottie-0.1.9/wagtail_lottie/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/models.py` & `wagtail_lottie-0.1.9/wagtail_lottie/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/static/wagtail_lottie/lottie-animation.js` & `wagtail_lottie-0.1.9/wagtail_lottie/static/wagtail_lottie/lottie-animation.js`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/static/wagtail_lottie/lottie-player.js` & `wagtail_lottie-0.1.9/wagtail_lottie/static/wagtail_lottie/lottie-player.js`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/tests/test_admin_views.py` & `wagtail_lottie-0.1.9/wagtail_lottie/tests/test_admin_views.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/tests/test_lottie_zip_file.py` & `wagtail_lottie-0.1.9/wagtail_lottie/tests/test_lottie_zip_file.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/views.py` & `wagtail_lottie-0.1.9/wagtail_lottie/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie/wagtail_hooks.py` & `wagtail_lottie-0.1.9/wagtail_lottie/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie.egg-info/PKG-INFO` & `wagtail_lottie-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wagtail-lottie
-Version: 0.1.8
+Name: wagtail_lottie
+Version: 0.1.9
 Summary: Wagtail Lottie
 Home-page: https://github.com/Aleksi44/wagtail-lottie
 Author: Alexis Le Baron
 Author-email: hello@snoweb.io
 License: GPL-3.0
 Keywords: wagtail lottie
 Platform: linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-lottie Version: 0.1.8 Summary: Wagtail
+Metadata-Version: 2.1 Name: wagtail_lottie Version: 0.1.9 Summary: Wagtail
 Lottie Home-page: https://github.com/Aleksi44/wagtail-lottie Author: Alexis Le
 Baron Author-email: hello@snoweb.io License: GPL-3.0 Keywords: wagtail lottie
 Platform: linux Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Operating System :: OS
```

### Comparing `wagtail_lottie-0.1.8/wagtail_lottie.egg-info/SOURCES.txt` & `wagtail_lottie-0.1.9/wagtail_lottie.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,12 +33,13 @@
 wagtail_lottie/migrations/0001_initial.py
 wagtail_lottie/migrations/__init__.py
 wagtail_lottie/static/wagtail_lottie/lottie-animation.js
 wagtail_lottie/static/wagtail_lottie/lottie-player.js
 wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/create.html
 wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/edit.html
 wagtail_lottie/templates/modeladmin/wagtail_lottie/lottieanimation/index.html
+wagtail_lottie/templates/wagtail_lottie/lottie_animation.html
 wagtail_lottie/templates/wagtail_lottie/homepage/site_summary_lottie_animation.html
 wagtail_lottie/tests/__init__.py
 wagtail_lottie/tests/_constants.py
 wagtail_lottie/tests/test_admin_views.py
 wagtail_lottie/tests/test_lottie_zip_file.py
```

