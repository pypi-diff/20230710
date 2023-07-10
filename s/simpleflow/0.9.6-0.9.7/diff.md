# Comparing `tmp/simpleflow-0.9.6.tar.gz` & `tmp/simpleflow-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simpleflow-0.9.6.tar", last modified: Thu Oct 22 09:40:08 2015, max compression
+gzip compressed data, was "dist/simpleflow-0.9.7.tar", last modified: Thu Oct 22 14:54:44 2015, max compression
```

## Comparing `simpleflow-0.9.6.tar` & `simpleflow-0.9.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/
--rw-r--r--   0 jbbarth    (501) staff       (20)      153 2015-03-11 03:03:35.000000 simpleflow-0.9.6/AUTHORS.rst
--rw-r--r--   0 jbbarth    (501) staff       (20)     3118 2015-10-07 03:58:57.000000 simpleflow-0.9.6/CONTRIBUTING.rst
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/examples/
--rw-r--r--   0 jbbarth    (501) staff       (20)        0 2015-10-06 15:57:27.000000 simpleflow-0.9.6/examples/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      799 2015-10-07 08:48:38.000000 simpleflow-0.9.6/examples/basic.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      863 2015-10-07 08:48:38.000000 simpleflow-0.9.6/examples/failing.py
--rw-r--r--   0 jbbarth    (501) staff       (20)       76 2015-03-11 03:03:35.000000 simpleflow-0.9.6/HISTORY.rst
--rw-r--r--   0 jbbarth    (501) staff       (20)     1052 2015-03-11 03:03:35.000000 simpleflow-0.9.6/LICENSE
--rw-r--r--   0 jbbarth    (501) staff       (20)       21 2015-03-11 03:03:35.000000 simpleflow-0.9.6/MANIFEST.in
--rw-r--r--   0 jbbarth    (501) staff       (20)    13373 2015-10-22 09:40:08.000000 simpleflow-0.9.6/PKG-INFO
--rw-r--r--   0 jbbarth    (501) staff       (20)     9599 2015-10-06 15:57:27.000000 simpleflow-0.9.6/README.rst
--rw-r--r--   0 jbbarth    (501) staff       (20)      114 2015-10-22 09:40:08.000000 simpleflow-0.9.6/setup.cfg
--rwxr-xr-x   0 jbbarth    (501) staff       (20)     3109 2015-10-22 09:39:34.000000 simpleflow-0.9.6/setup.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/
--rwxr-xr-x   0 jbbarth    (501) staff       (20)      283 2015-10-22 09:39:34.000000 simpleflow-0.9.6/simpleflow/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     2702 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/activity.py
--rw-r--r--   0 jbbarth    (501) staff       (20)    14138 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/command.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      617 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/compat.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     1482 2015-10-07 08:48:38.000000 simpleflow-0.9.6/simpleflow/exceptions.py
--rw-r--r--   0 jbbarth    (501) staff       (20)    10275 2015-10-07 03:58:57.000000 simpleflow-0.9.6/simpleflow/execute.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     3231 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/executor.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     3062 2015-10-07 08:48:38.000000 simpleflow-0.9.6/simpleflow/futures.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     6659 2015-10-07 04:59:02.000000 simpleflow-0.9.6/simpleflow/history.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/local/
--rw-r--r--   0 jbbarth    (501) staff       (20)       39 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/local/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     1141 2015-10-07 08:48:38.000000 simpleflow-0.9.6/simpleflow/local/executor.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/settings/
--rw-r--r--   0 jbbarth    (501) staff       (20)      104 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/settings/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     1488 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/settings/base.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      965 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/settings/default.py
--rwxr-xr-x   0 jbbarth    (501) staff       (20)       24 2015-03-11 03:03:35.000000 simpleflow-0.9.6/simpleflow/simpleflow.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/swf/
--rw-r--r--   0 jbbarth    (501) staff       (20)        0 2015-03-11 03:03:35.000000 simpleflow-0.9.6/simpleflow/swf/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)       51 2015-08-25 13:16:20.000000 simpleflow-0.9.6/simpleflow/swf/constants.py
--rw-r--r--   0 jbbarth    (501) staff       (20)    13707 2015-10-07 08:48:38.000000 simpleflow-0.9.6/simpleflow/swf/executor.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     2753 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/helpers.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/swf/process/
--rw-r--r--   0 jbbarth    (501) staff       (20)      111 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/process/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     9363 2015-10-08 12:21:42.000000 simpleflow-0.9.6/simpleflow/swf/process/actor.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/swf/process/decider/
--rw-r--r--   0 jbbarth    (501) staff       (20)      134 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/process/decider/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     5356 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/decider/base.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      267 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/decider/command.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      884 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/decider/helpers.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/
--rw-r--r--   0 jbbarth    (501) staff       (20)       23 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     5911 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/base.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      640 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/command.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/
--rw-r--r--   0 jbbarth    (501) staff       (20)       82 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      817 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/by_module.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      137 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/dry_run.py
--rw-r--r--   0 jbbarth    (501) staff       (20)       41 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/exceptions.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      762 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/from_task_registry.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     3397 2015-10-07 03:58:57.000000 simpleflow-0.9.6/simpleflow/swf/process/worker/heartbeat.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/swf/stats/
--rw-r--r--   0 jbbarth    (501) staff       (20)       49 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/stats/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     2504 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/stats/base.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     7318 2015-10-22 09:30:38.000000 simpleflow-0.9.6/simpleflow/swf/stats/pretty.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     2495 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/task.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      442 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/swf/utils.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     2003 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/task.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow/utils/
--rw-r--r--   0 jbbarth    (501) staff       (20)       20 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/utils/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     1714 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/utils/retry.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     2252 2015-10-06 15:57:27.000000 simpleflow-0.9.6/simpleflow/workflow.py
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow.egg-info/
--rw-r--r--   0 jbbarth    (501) staff       (20)        1 2015-10-22 09:40:07.000000 simpleflow-0.9.6/simpleflow.egg-info/dependency_links.txt
--rw-r--r--   0 jbbarth    (501) staff       (20)       55 2015-10-22 09:40:07.000000 simpleflow-0.9.6/simpleflow.egg-info/entry_points.txt
--rw-r--r--   0 jbbarth    (501) staff       (20)        1 2015-10-08 12:22:31.000000 simpleflow-0.9.6/simpleflow.egg-info/not-zip-safe
--rw-r--r--   0 jbbarth    (501) staff       (20)    13373 2015-10-22 09:40:07.000000 simpleflow-0.9.6/simpleflow.egg-info/PKG-INFO
--rw-r--r--   0 jbbarth    (501) staff       (20)       79 2015-10-22 09:40:07.000000 simpleflow-0.9.6/simpleflow.egg-info/requires.txt
--rw-r--r--   0 jbbarth    (501) staff       (20)     1774 2015-10-22 09:40:08.000000 simpleflow-0.9.6/simpleflow.egg-info/SOURCES.txt
--rw-r--r--   0 jbbarth    (501) staff       (20)       20 2015-10-22 09:40:07.000000 simpleflow-0.9.6/simpleflow.egg-info/top_level.txt
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/
+-rw-r--r--   0 jbbarth    (501) staff       (20)      153 2015-03-11 03:03:35.000000 simpleflow-0.9.7/AUTHORS.rst
+-rw-r--r--   0 jbbarth    (501) staff       (20)     3118 2015-10-07 03:58:57.000000 simpleflow-0.9.7/CONTRIBUTING.rst
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/examples/
+-rw-r--r--   0 jbbarth    (501) staff       (20)        0 2015-10-06 15:57:27.000000 simpleflow-0.9.7/examples/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      799 2015-10-07 08:48:38.000000 simpleflow-0.9.7/examples/basic.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      863 2015-10-07 08:48:38.000000 simpleflow-0.9.7/examples/failing.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)       76 2015-03-11 03:03:35.000000 simpleflow-0.9.7/HISTORY.rst
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1052 2015-03-11 03:03:35.000000 simpleflow-0.9.7/LICENSE
+-rw-r--r--   0 jbbarth    (501) staff       (20)       21 2015-03-11 03:03:35.000000 simpleflow-0.9.7/MANIFEST.in
+-rw-r--r--   0 jbbarth    (501) staff       (20)    13373 2015-10-22 14:54:44.000000 simpleflow-0.9.7/PKG-INFO
+-rw-r--r--   0 jbbarth    (501) staff       (20)     9599 2015-10-06 15:57:27.000000 simpleflow-0.9.7/README.rst
+-rw-r--r--   0 jbbarth    (501) staff       (20)      114 2015-10-22 14:54:44.000000 simpleflow-0.9.7/setup.cfg
+-rwxr-xr-x   0 jbbarth    (501) staff       (20)     3109 2015-10-22 09:39:34.000000 simpleflow-0.9.7/setup.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/
+-rwxr-xr-x   0 jbbarth    (501) staff       (20)      283 2015-10-22 14:54:40.000000 simpleflow-0.9.7/simpleflow/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2702 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/activity.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)    14138 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/command.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      617 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/compat.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1482 2015-10-07 08:48:38.000000 simpleflow-0.9.7/simpleflow/exceptions.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)    10365 2015-10-22 14:51:16.000000 simpleflow-0.9.7/simpleflow/execute.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     3231 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/executor.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     3062 2015-10-07 08:48:38.000000 simpleflow-0.9.7/simpleflow/futures.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     6659 2015-10-07 04:59:02.000000 simpleflow-0.9.7/simpleflow/history.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/local/
+-rw-r--r--   0 jbbarth    (501) staff       (20)       39 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/local/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1141 2015-10-07 08:48:38.000000 simpleflow-0.9.7/simpleflow/local/executor.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/settings/
+-rw-r--r--   0 jbbarth    (501) staff       (20)      104 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/settings/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1488 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/settings/base.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      965 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/settings/default.py
+-rwxr-xr-x   0 jbbarth    (501) staff       (20)       24 2015-03-11 03:03:35.000000 simpleflow-0.9.7/simpleflow/simpleflow.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/swf/
+-rw-r--r--   0 jbbarth    (501) staff       (20)        0 2015-03-11 03:03:35.000000 simpleflow-0.9.7/simpleflow/swf/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)       51 2015-08-25 13:16:20.000000 simpleflow-0.9.7/simpleflow/swf/constants.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)    13707 2015-10-07 08:48:38.000000 simpleflow-0.9.7/simpleflow/swf/executor.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2753 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/helpers.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/swf/process/
+-rw-r--r--   0 jbbarth    (501) staff       (20)      111 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/process/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     9363 2015-10-08 12:21:42.000000 simpleflow-0.9.7/simpleflow/swf/process/actor.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/swf/process/decider/
+-rw-r--r--   0 jbbarth    (501) staff       (20)      134 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/process/decider/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     5356 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/decider/base.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      267 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/decider/command.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      884 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/decider/helpers.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/
+-rw-r--r--   0 jbbarth    (501) staff       (20)       23 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     5911 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/base.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      640 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/command.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/
+-rw-r--r--   0 jbbarth    (501) staff       (20)       82 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      817 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/by_module.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      137 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/dry_run.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)       41 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/exceptions.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      762 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/from_task_registry.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     3397 2015-10-07 03:58:57.000000 simpleflow-0.9.7/simpleflow/swf/process/worker/heartbeat.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/swf/stats/
+-rw-r--r--   0 jbbarth    (501) staff       (20)       49 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/stats/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2504 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/stats/base.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     7318 2015-10-22 09:30:38.000000 simpleflow-0.9.7/simpleflow/swf/stats/pretty.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2495 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/task.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      442 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/swf/utils.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2003 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/task.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow/utils/
+-rw-r--r--   0 jbbarth    (501) staff       (20)       20 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/utils/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1714 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/utils/retry.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2252 2015-10-06 15:57:27.000000 simpleflow-0.9.7/simpleflow/workflow.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow.egg-info/
+-rw-r--r--   0 jbbarth    (501) staff       (20)        1 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow.egg-info/dependency_links.txt
+-rw-r--r--   0 jbbarth    (501) staff       (20)       55 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow.egg-info/entry_points.txt
+-rw-r--r--   0 jbbarth    (501) staff       (20)        1 2015-10-08 12:22:31.000000 simpleflow-0.9.7/simpleflow.egg-info/not-zip-safe
+-rw-r--r--   0 jbbarth    (501) staff       (20)    13373 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow.egg-info/PKG-INFO
+-rw-r--r--   0 jbbarth    (501) staff       (20)       78 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow.egg-info/requires.txt
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1774 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow.egg-info/SOURCES.txt
+-rw-r--r--   0 jbbarth    (501) staff       (20)       20 2015-10-22 14:54:44.000000 simpleflow-0.9.7/simpleflow.egg-info/top_level.txt
```

### Comparing `simpleflow-0.9.6/CONTRIBUTING.rst` & `simpleflow-0.9.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/examples/basic.py` & `simpleflow-0.9.7/examples/basic.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/examples/failing.py` & `simpleflow-0.9.7/examples/failing.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/LICENSE` & `simpleflow-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/PKG-INFO` & `simpleflow-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: simpleflow
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python library for dataflow programming with Amazon SWF
 Home-page: https://github.com/botify-labs/simpleflow
 Author: Greg Leclercq
 Author-email: greg@botify.com
 License: Copyright 2014 Greg Leclercq
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `simpleflow-0.9.6/README.rst` & `simpleflow-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/setup.py` & `simpleflow-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/activity.py` & `simpleflow-0.9.7/simpleflow/activity.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/command.py` & `simpleflow-0.9.7/simpleflow/command.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/compat.py` & `simpleflow-0.9.7/simpleflow/compat.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/exceptions.py` & `simpleflow-0.9.7/simpleflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/execute.py` & `simpleflow-0.9.7/simpleflow/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
                     interpreter, '-m', command,  # execute module a script.
                     get_name(func), format_arguments_json(*args, **kwargs),
                 ],
                     # Redirect stderr to stdout to get traceback on error.
                     stderr=subprocess.STDOUT,
                 )
             except subprocess.CalledProcessError as err:
+                logger.info("got a subprocess.CalledProcessError: {}".format(err.output))
                 exclines = err.output.rstrip().rsplit('\n', 2)
                 if len(exclines) == 1:
                     excline = exclines[0]
                 else:
                     excline = exclines[1]
 
                 try:
```

### Comparing `simpleflow-0.9.6/simpleflow/executor.py` & `simpleflow-0.9.7/simpleflow/executor.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/futures.py` & `simpleflow-0.9.7/simpleflow/futures.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/history.py` & `simpleflow-0.9.7/simpleflow/history.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/local/executor.py` & `simpleflow-0.9.7/simpleflow/local/executor.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/settings/base.py` & `simpleflow-0.9.7/simpleflow/settings/base.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/settings/default.py` & `simpleflow-0.9.7/simpleflow/settings/default.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/executor.py` & `simpleflow-0.9.7/simpleflow/swf/executor.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/helpers.py` & `simpleflow-0.9.7/simpleflow/swf/helpers.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/actor.py` & `simpleflow-0.9.7/simpleflow/swf/process/actor.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/decider/base.py` & `simpleflow-0.9.7/simpleflow/swf/process/decider/base.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/decider/helpers.py` & `simpleflow-0.9.7/simpleflow/swf/process/decider/helpers.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/worker/base.py` & `simpleflow-0.9.7/simpleflow/swf/process/worker/base.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/worker/command.py` & `simpleflow-0.9.7/simpleflow/swf/process/worker/command.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/by_module.py` & `simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/by_module.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/worker/dispatch/from_task_registry.py` & `simpleflow-0.9.7/simpleflow/swf/process/worker/dispatch/from_task_registry.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/process/worker/heartbeat.py` & `simpleflow-0.9.7/simpleflow/swf/process/worker/heartbeat.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/stats/base.py` & `simpleflow-0.9.7/simpleflow/swf/stats/base.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/stats/pretty.py` & `simpleflow-0.9.7/simpleflow/swf/stats/pretty.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/swf/task.py` & `simpleflow-0.9.7/simpleflow/swf/task.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/task.py` & `simpleflow-0.9.7/simpleflow/task.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/utils/retry.py` & `simpleflow-0.9.7/simpleflow/utils/retry.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow/workflow.py` & `simpleflow-0.9.7/simpleflow/workflow.py`

 * *Files identical despite different names*

### Comparing `simpleflow-0.9.6/simpleflow.egg-info/PKG-INFO` & `simpleflow-0.9.7/simpleflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: simpleflow
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python library for dataflow programming with Amazon SWF
 Home-page: https://github.com/botify-labs/simpleflow
 Author: Greg Leclercq
 Author-email: greg@botify.com
 License: Copyright 2014 Greg Leclercq
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `simpleflow-0.9.6/simpleflow.egg-info/SOURCES.txt` & `simpleflow-0.9.7/simpleflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

