# Comparing `tmp/faasmctl-0.2.0.tar.gz` & `tmp/faasmctl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.2.0.tar", last modified: Sun Jul  9 17:59:40 2023, max compression
+gzip compressed data, was "faasmctl-0.2.1.tar", last modified: Mon Jul 10 08:45:48 2023, max compression
```

## Comparing `faasmctl-0.2.0.tar` & `faasmctl-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.503262 faasmctl-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-09 17:59:31.000000 faasmctl-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-09 17:59:40.503262 faasmctl-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-09 17:59:31.000000 faasmctl-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.499262 faasmctl-0.2.0/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.499262 faasmctl-0.2.0/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.503262 faasmctl-0.2.0/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-09 17:59:31.000000 faasmctl-0.2.0/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 17:59:40.499262 faasmctl-0.2.0/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 17:59:40.000000 faasmctl-0.2.0/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-09 17:59:31.000000 faasmctl-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 17:59:40.503262 faasmctl-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:48.265674 faasmctl-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 08:43:45.000000 faasmctl-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-10 08:45:48.265674 faasmctl-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-10 08:43:45.000000 faasmctl-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:48.257674 faasmctl-0.2.1/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:48.261674 faasmctl-0.2.1/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:48.265674 faasmctl-0.2.1/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:48.265674 faasmctl-0.2.1/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-10 08:45:38.000000 faasmctl-0.2.1/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-10 08:45:38.000000 faasmctl-0.2.1/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-10 08:43:45.000000 faasmctl-0.2.1/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:45:48.257674 faasmctl-0.2.1/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-10 08:45:48.000000 faasmctl-0.2.1/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-10 08:45:48.000000 faasmctl-0.2.1/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:45:48.000000 faasmctl-0.2.1/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 08:45:48.000000 faasmctl-0.2.1/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 08:45:48.000000 faasmctl-0.2.1/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 08:45:48.000000 faasmctl-0.2.1/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-10 08:43:45.000000 faasmctl-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:45:48.265674 faasmctl-0.2.1/setup.cfg
```

### Comparing `faasmctl-0.2.0/LICENSE.md` & `faasmctl-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.2.0/PKG-INFO` & `faasmctl-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.2.0
+pip install faasmctl==0.2.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.2.0/README.md` & `faasmctl-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.2.0
+pip install faasmctl==0.2.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.2.0/faasmctl/tasks/flush.py` & `faasmctl-0.2.1/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.2.0/faasmctl/tasks/invoke.py` & `faasmctl-0.2.1/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.2.0/faasmctl/util/config.py` & `faasmctl-0.2.1/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.2.0/faasmctl/util/flush.py` & `faasmctl-0.2.1/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.2.0/faasmctl/util/invoke.py` & `faasmctl-0.2.1/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.2.0/faasmctl/util/planner.py` & `faasmctl-0.2.1/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.2.0/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.2.1/faasmctl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.2.0
+Version: 0.2.1
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.2.0
+pip install faasmctl==0.2.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.2.0/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.2.1/faasmctl.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 faasmctl/util/faasm.py
 faasmctl/util/flush.py
 faasmctl/util/invoke.py
 faasmctl/util/message.py
 faasmctl/util/planner.py
 faasmctl/util/random.py
 faasmctl/util/upload.py
-faasmctl/util/version.py
+faasmctl/util/version.py
+faasmctl/util/gen_proto/faabric_pb2.py
+faasmctl/util/gen_proto/planner_pb2.py
```

### Comparing `faasmctl-0.2.0/pyproject.toml` & `faasmctl-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

