# Comparing `tmp/pyfirebird-0.0.76.tar.gz` & `tmp/pyfirebird-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.76.tar", last modified: Sun Jul  9 22:30:02 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.77.tar", last modified: Sun Jul  9 22:41:10 2023, max compression
```

## Comparing `pyfirebird-0.0.76.tar` & `pyfirebird-0.0.77.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.76/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1364 2023-07-09 22:29:24.000000 pyfirebird-0.0.76/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      178 2023-07-09 20:16:41.000000 pyfirebird-0.0.76/src/firebird/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.76/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.76/src/firebird/cmd_tools/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2515 2023-07-07 07:05:58.000000 pyfirebird-0.0.76/src/firebird/cmd_tools/executor.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3747 2023-07-09 22:28:53.000000 pyfirebird-0.0.76/src/firebird/cmd_tools/executor_impl.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.76/src/firebird/cmd_tools/fbconsole.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3505 2023-06-28 09:30:24.000000 pyfirebird-0.0.76/src/firebird/cmd_tools/pipeline.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5032 2023-07-09 21:51:48.000000 pyfirebird-0.0.76/src/firebird/cmd_tools/pipeline_impl.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebird/libs/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       37 2023-07-07 05:29:05.000000 pyfirebird-0.0.76/src/firebird/libs/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1633 2023-07-09 07:20:57.000000 pyfirebird-0.0.76/src/firebird/libs/k8.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      448 2023-07-09 05:28:06.000000 pyfirebird-0.0.76/src/firebird/libs/template.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.76/src/firebird/rabbitmq.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebird/resources/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebird/resources/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2181 2023-07-09 06:36:53.000000 pyfirebird-0.0.76/src/firebird/resources/templates/pipeline.yaml
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebird/utils/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.76/src/firebird/utils/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.76/src/firebird/utils/checkpoint.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6909 2023-07-09 22:25:57.000000 pyfirebird-0.0.76/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/asgi.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/settings.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/wsgi.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/admin.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/apps.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/migrations/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/migrations/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-28 08:49:46.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/models.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.066036 pyfirebird-0.0.76/src/firebirdconsole/ui/static/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/static/images/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/static/images/logo.jpeg
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1558716 2023-07-09 21:54:18.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/home.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1675307 2023-07-09 21:54:18.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/pipeline.js
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/templates/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/templates/application.html
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/templates/index.html
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/templatetags/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/templatetags/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/templatetags/app_filters.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/tests.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-07-09 21:45:44.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/urls.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/view_tools.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/views/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/views/__init__.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/firebirdconsole/ui/views/apis/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       45 2023-07-09 21:39:21.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/views/apis/__init__.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3685 2023-07-09 22:17:22.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/views/apis/main.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/views/home.py
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.76/src/firebirdconsole/ui/views/pipeline.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:30:02.070037 pyfirebird-0.0.76/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 22:30:02.000000 pyfirebird-0.0.76/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1964 2023-07-09 22:30:02.000000 pyfirebird-0.0.76/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-09 22:30:02.000000 pyfirebird-0.0.76/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-07-09 22:30:02.000000 pyfirebird-0.0.76/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       72 2023-07-09 22:30:02.000000 pyfirebird-0.0.76/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-07-09 22:30:02.000000 pyfirebird-0.0.76/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.77/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1364 2023-07-09 22:40:41.000000 pyfirebird-0.0.77/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      178 2023-07-09 20:16:41.000000 pyfirebird-0.0.77/src/firebird/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)    11633 2023-06-26 09:30:32.000000 pyfirebird-0.0.77/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:31.000000 pyfirebird-0.0.77/src/firebird/cmd_tools/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2515 2023-07-07 07:05:58.000000 pyfirebird-0.0.77/src/firebird/cmd_tools/executor.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3747 2023-07-09 22:28:53.000000 pyfirebird-0.0.77/src/firebird/cmd_tools/executor_impl.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      649 2023-06-26 09:30:31.000000 pyfirebird-0.0.77/src/firebird/cmd_tools/fbconsole.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3505 2023-06-28 09:30:24.000000 pyfirebird-0.0.77/src/firebird/cmd_tools/pipeline.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     5142 2023-07-09 22:40:02.000000 pyfirebird-0.0.77/src/firebird/cmd_tools/pipeline_impl.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebird/libs/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       37 2023-07-07 05:29:05.000000 pyfirebird-0.0.77/src/firebird/libs/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1633 2023-07-09 07:20:57.000000 pyfirebird-0.0.77/src/firebird/libs/k8.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      448 2023-07-09 05:28:06.000000 pyfirebird-0.0.77/src/firebird/libs/template.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-06-26 09:30:31.000000 pyfirebird-0.0.77/src/firebird/rabbitmq.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.759349 pyfirebird-0.0.77/src/firebird/resources/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebird/resources/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     2181 2023-07-09 06:36:53.000000 pyfirebird-0.0.77/src/firebird/resources/templates/pipeline.yaml
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebird/utils/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:31.000000 pyfirebird-0.0.77/src/firebird/utils/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-06-26 09:30:31.000000 pyfirebird-0.0.77/src/firebird/utils/checkpoint.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     6909 2023-07-09 22:25:57.000000 pyfirebird-0.0.77/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/asgi.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3803 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/settings.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      836 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      407 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/wsgi.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebirdconsole/ui/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:35.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       63 2023-06-26 09:30:35.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/admin.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-06-26 09:30:35.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/apps.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebirdconsole/ui/migrations/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/migrations/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       57 2023-06-28 08:49:46.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/models.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.759349 pyfirebird-0.0.77/src/firebirdconsole/ui/static/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.763349 pyfirebird-0.0.77/src/firebirdconsole/ui/static/images/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)   126365 2023-06-26 09:30:41.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/static/images/logo.jpeg
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1558716 2023-07-09 21:54:18.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/home.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      271 2023-06-26 09:30:38.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/home.js.LICENSE.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)  1675307 2023-07-09 21:54:18.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/pipeline.js
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      527 2023-06-26 09:30:35.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/src/firebirdconsole/ui/templates/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3817 2023-06-26 09:30:42.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/templates/application.html
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      217 2023-06-26 09:30:42.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/templates/index.html
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/src/firebirdconsole/ui/templatetags/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-06-26 09:30:32.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/templatetags/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      639 2023-06-26 09:30:32.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/templatetags/app_filters.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-06-26 09:30:42.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/tests.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-07-09 21:45:44.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/urls.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      571 2023-06-26 09:30:42.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/view_tools.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/src/firebirdconsole/ui/views/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       54 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/views/__init__.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/src/firebirdconsole/ui/views/apis/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       45 2023-07-09 21:39:21.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/views/apis/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     3686 2023-07-09 22:36:33.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/views/apis/main.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      288 2023-06-26 09:30:42.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/views/home.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      387 2023-06-26 09:30:43.000000 pyfirebird-0.0.77/src/firebirdconsole/ui/views/pipeline.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-07-09 22:41:10.767349 pyfirebird-0.0.77/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      368 2023-07-09 22:41:10.000000 pyfirebird-0.0.77/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1964 2023-07-09 22:41:10.000000 pyfirebird-0.0.77/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-07-09 22:41:10.000000 pyfirebird-0.0.77/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      152 2023-07-09 22:41:10.000000 pyfirebird-0.0.77/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       72 2023-07-09 22:41:10.000000 pyfirebird-0.0.77/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       25 2023-07-09 22:41:10.000000 pyfirebird-0.0.77/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.76/setup.py` & `pyfirebird-0.0.77/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.76",
+    version="0.0.77",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.76/src/firebird/base.py` & `pyfirebird-0.0.77/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.77/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/cmd_tools/executor_impl.py` & `pyfirebird-0.0.77/src/firebird/cmd_tools/executor_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/cmd_tools/fbconsole.py` & `pyfirebird-0.0.77/src/firebird/cmd_tools/fbconsole.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.77/src/firebird/cmd_tools/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.77/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,19 @@
         if input_port_count == 0:
             generator_ids.append(node["id"])
     return generator_ids
 
 
 def stop_command(config:dict, pipeline_id:str):
     with zkdb(**config['zookeeper']) as db:
-        pipeline = db.get_pipeline(pipeline_id)
+        error, pipeline = db.get_pipeline(pipeline_id)
+
+    if error != ZKError.OK:
+        print(f"Unable to get pipeline, error is {error}")
+        return
 
     if not pipeline['is_running']:
         print(f"Pipeline is not running!")
         return
 
     for generator_id in get_generator_ids(pipeline):
         name = f"firebird-pipeline--{pipeline_id}--{generator_id}"
```

### Comparing `pyfirebird-0.0.76/src/firebird/libs/k8.py` & `pyfirebird-0.0.77/src/firebird/libs/k8.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/rabbitmq.py` & `pyfirebird-0.0.77/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/resources/templates/pipeline.yaml` & `pyfirebird-0.0.77/src/firebird/resources/templates/pipeline.yaml`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/utils/checkpoint.py` & `pyfirebird-0.0.77/src/firebird/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebird/zkdb.py` & `pyfirebird-0.0.77/src/firebird/zkdb.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/settings.py` & `pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/settings.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/firebirdconsole/urls.py` & `pyfirebird-0.0.77/src/firebirdconsole/firebirdconsole/urls.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/static/images/logo.jpeg` & `pyfirebird-0.0.77/src/firebirdconsole/ui/static/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/home.js` & `pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/home.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/pipeline.js` & `pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/pipeline.js`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt` & `pyfirebird-0.0.77/src/firebirdconsole/ui/static/js-bundle/pipeline.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/templates/application.html` & `pyfirebird-0.0.77/src/firebirdconsole/ui/templates/application.html`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/templatetags/app_filters.py` & `pyfirebird-0.0.77/src/firebirdconsole/ui/templatetags/app_filters.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/view_tools.py` & `pyfirebird-0.0.77/src/firebirdconsole/ui/view_tools.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.76/src/firebirdconsole/ui/views/apis/main.py` & `pyfirebird-0.0.77/src/firebirdconsole/ui/views/apis/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,11 +90,11 @@
     return JsonResponse({
         "pipeline": pipeline,
         "svg_lr": svgs[0],
         "svg_tb": svgs[1],
     })
 
 class PipelinesAPI(RESTAPIBase):
-    def get(self, request:HttpRequest, **kwargs):
+    def list(self, request:HttpRequest, **kwargs):
         with zkdb(**settings.FIREBIRD_CONFIG['zookeeper']) as db:
             pipelines = db.get_pipelines()
         return {"pipelines": pipelines}
```

### Comparing `pyfirebird-0.0.76/src/pyfirebird.egg-info/SOURCES.txt` & `pyfirebird-0.0.77/src/pyfirebird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

