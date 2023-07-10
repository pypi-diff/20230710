# Comparing `tmp/container_hub-0.1.8.tar.gz` & `tmp/container_hub-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container_hub-0.1.8.tar", last modified: Fri Feb 10 10:23:03 2023, max compression
+gzip compressed data, was "container_hub-0.1.9.tar", last modified: Mon Feb 13 09:57:07 2023, max compression
```

## Comparing `container_hub-0.1.8.tar` & `container_hub-0.1.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.669662 container_hub-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-10 10:22:58.000000 container_hub-0.1.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-02-10 10:22:58.000000 container_hub-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-10 10:22:58.000000 container_hub-0.1.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-10 10:22:58.000000 container_hub-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-10 10:22:58.000000 container_hub-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-10 10:23:03.669662 container_hub-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-02-10 10:22:58.000000 container_hub-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.661662 container_hub-0.1.8/container_hub/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.661662 container_hub-0.1.8/container_hub/carriers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.661662 container_hub-0.1.8/container_hub/carriers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/docker/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.661662 container_hub-0.1.8/container_hub/carriers/docker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/docker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/docker/tests/test_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.661662 container_hub-0.1.8/container_hub/carriers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/kubernetes/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.669662 container_hub-0.1.8/container_hub/carriers/kubernetes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/kubernetes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/kubernetes/tests/test_kubernetes_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.669662 container_hub-0.1.8/container_hub/carriers/marathon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/marathon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/marathon/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.669662 container_hub-0.1.8/container_hub/carriers/marathon/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/marathon/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/carriers/marathon/tests/test_marathon_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-10 10:22:58.000000 container_hub-0.1.8/container_hub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.661662 container_hub-0.1.8/container_hub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-10 10:23:03.000000 container_hub-0.1.8/container_hub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-10 10:23:03.000000 container_hub-0.1.8/container_hub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 10:23:03.000000 container_hub-0.1.8/container_hub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 10:23:03.000000 container_hub-0.1.8/container_hub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-10 10:23:03.000000 container_hub-0.1.8/container_hub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-10 10:23:03.000000 container_hub-0.1.8/container_hub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.669662 container_hub-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-10 10:22:58.000000 container_hub-0.1.8/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-10 10:23:03.673662 container_hub-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-10 10:22:58.000000 container_hub-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.669662 container_hub-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-10 10:22:58.000000 container_hub-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-02-10 10:22:58.000000 container_hub-0.1.8/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 10:23:03.669662 container_hub-0.1.8/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-10 10:22:58.000000 container_hub-0.1.8/tests/test_files/docker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-10 10:22:58.000000 container_hub-0.1.8/tests/test_files/kubernetes_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-10 10:22:58.000000 container_hub-0.1.8/tests/test_files/marathon_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.269664 container_hub-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-13 09:57:02.000000 container_hub-0.1.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-02-13 09:57:02.000000 container_hub-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-13 09:57:02.000000 container_hub-0.1.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-13 09:57:02.000000 container_hub-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-13 09:57:02.000000 container_hub-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-02-13 09:57:07.269664 container_hub-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-02-13 09:57:02.000000 container_hub-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/carriers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/carriers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/docker/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/carriers/docker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/docker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/docker/tests/test_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/carriers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/kubernetes/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/carriers/kubernetes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/kubernetes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/kubernetes/tests/test_kubernetes_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/carriers/marathon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/marathon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/marathon/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub/carriers/marathon/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/marathon/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/carriers/marathon/tests/test_marathon_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-13 09:57:02.000000 container_hub-0.1.9/container_hub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.265664 container_hub-0.1.9/container_hub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-02-13 09:57:07.000000 container_hub-0.1.9/container_hub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-13 09:57:07.000000 container_hub-0.1.9/container_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 09:57:07.000000 container_hub-0.1.9/container_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 09:57:07.000000 container_hub-0.1.9/container_hub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-13 09:57:07.000000 container_hub-0.1.9/container_hub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-13 09:57:07.000000 container_hub-0.1.9/container_hub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.269664 container_hub-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-13 09:57:02.000000 container_hub-0.1.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-13 09:57:07.269664 container_hub-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-02-13 09:57:02.000000 container_hub-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.269664 container_hub-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-13 09:57:02.000000 container_hub-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-02-13 09:57:02.000000 container_hub-0.1.9/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 09:57:07.269664 container_hub-0.1.9/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-13 09:57:02.000000 container_hub-0.1.9/tests/test_files/docker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-13 09:57:02.000000 container_hub-0.1.9/tests/test_files/kubernetes_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-13 09:57:02.000000 container_hub-0.1.9/tests/test_files/marathon_settings.py
```

### Comparing `container_hub-0.1.8/CONTRIBUTING.rst` & `container_hub-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/HISTORY.rst` & `container_hub-0.1.9/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 =======
 History
 =======
 
 
+0.1.9 (2023-02-13)
+------------------
+
+- Added shared `EmptyDirVolumeSource` with name "shared-data" between simulation and scheduler container.
+
+
 0.1.8 (2023-02-10)
 ------------------
 
 - Drop `scheduler-worker` container in Kubernetes.
 
 
 0.1.7 (2022-12-07)
```

### Comparing `container_hub-0.1.8/LICENSE` & `container_hub-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/PKG-INFO` & `container_hub-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: container_hub
-Version: 0.1.8
+Version: 0.1.9
 Summary: The 3Di simulation container hub
 Home-page: https://github.com/nens/container-hub
 Author: Lars Claussen
 Author-email: claussen.lars@nelen-schuurmans.nl
 License: MIT license
 Description: =============
         container-hub
@@ -52,14 +52,20 @@
         
         
         =======
         History
         =======
         
         
+        0.1.9 (2023-02-13)
+        ------------------
+        
+        - Added shared `EmptyDirVolumeSource` with name "shared-data" between simulation and scheduler container.
+        
+        
         0.1.8 (2023-02-10)
         ------------------
         
         - Drop `scheduler-worker` container in Kubernetes.
         
         
         0.1.7 (2022-12-07)
```

### Comparing `container_hub-0.1.8/README.rst` & `container_hub-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/container_hub/__init__.py` & `container_hub-0.1.9/container_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/container_hub/carriers/docker/backend.py` & `container_hub-0.1.9/container_hub/carriers/docker/backend.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/container_hub/carriers/docker/tests/test_docker_backend.py` & `container_hub-0.1.9/container_hub/carriers/docker/tests/test_docker_backend.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/container_hub/carriers/kubernetes/backend.py` & `container_hub-0.1.9/container_hub/carriers/kubernetes/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     HostPathVolumeSource,
     LocalObjectReference,
     Affinity,
     NodeAffinity,
     NodeSelectorTerm,
     NodeSelector,
     NodeSelectorRequirement,
+    EmptyDirVolumeSource
 )
 
 
 # Accessing host (laptop) from within k8s cluster
 K3S_HOST_DNS_NAME = "host.k3d.internal"
 MINIKUBE_HOST_DNS_NAME = "host.minikube.internal"
 
@@ -168,15 +169,15 @@
                         Volume(
                             name=mount.name,
                             hostPath=HostPathVolumeSource(
                                 path=mount.local_path, type="Directory"
                             ),
                         )
                         for mount in cfg.mount_points
-                    ],
+                    ] + [Volume(name='shared-data', emptyDir=EmptyDirVolumeSource())],
                     restartPolicy="Never",
                 ),
             ),
         ),
     )
```

### Comparing `container_hub-0.1.8/container_hub/carriers/kubernetes/tests/test_kubernetes_backend.py` & `container_hub-0.1.9/container_hub/carriers/kubernetes/tests/test_kubernetes_backend.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/container_hub/carriers/marathon/backend.py` & `container_hub-0.1.9/container_hub/carriers/marathon/backend.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/container_hub/carriers/marathon/tests/test_marathon_backend.py` & `container_hub-0.1.9/container_hub/carriers/marathon/tests/test_marathon_backend.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/container_hub/models.py` & `container_hub-0.1.9/container_hub/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         """
         mount_points = []
         for mount_point in (
             self.redis_config.mount_points
             + self.scheduler_config.mount_points
             + self.simulation_config.mount_points
         ):
-            if mount_point not in mount_points:
+            if mount_point not in mount_points and mount_point.name != 'shared-data':
                 mount_points.append(mount_point)
         return mount_points
 
     @classmethod
     def from_settings(
         cls, name: str, settings, prefix="CONTAINER_HUB"
     ) -> "KubernetesJobConfig":
```

### Comparing `container_hub-0.1.8/container_hub.egg-info/PKG-INFO` & `container_hub-0.1.9/container_hub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: container-hub
-Version: 0.1.8
+Version: 0.1.9
 Summary: The 3Di simulation container hub
 Home-page: https://github.com/nens/container-hub
 Author: Lars Claussen
 Author-email: claussen.lars@nelen-schuurmans.nl
 License: MIT license
 Description: =============
         container-hub
@@ -52,14 +52,20 @@
         
         
         =======
         History
         =======
         
         
+        0.1.9 (2023-02-13)
+        ------------------
+        
+        - Added shared `EmptyDirVolumeSource` with name "shared-data" between simulation and scheduler container.
+        
+        
         0.1.8 (2023-02-10)
         ------------------
         
         - Drop `scheduler-worker` container in Kubernetes.
         
         
         0.1.7 (2022-12-07)
```

### Comparing `container_hub-0.1.8/container_hub.egg-info/SOURCES.txt` & `container_hub-0.1.9/container_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/docs/Makefile` & `container_hub-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/docs/conf.py` & `container_hub-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/docs/installation.rst` & `container_hub-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/docs/make.bat` & `container_hub-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/setup.cfg` & `container_hub-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/setup.py` & `container_hub-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/tests/test_config.py` & `container_hub-0.1.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/tests/test_files/docker_settings.py` & `container_hub-0.1.9/tests/test_files/docker_settings.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/tests/test_files/kubernetes_settings.py` & `container_hub-0.1.9/tests/test_files/kubernetes_settings.py`

 * *Files identical despite different names*

### Comparing `container_hub-0.1.8/tests/test_files/marathon_settings.py` & `container_hub-0.1.9/tests/test_files/marathon_settings.py`

 * *Files identical despite different names*

