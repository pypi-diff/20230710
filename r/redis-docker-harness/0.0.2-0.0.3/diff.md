# Comparing `tmp/redis-docker-harness-0.0.2.tar.gz` & `tmp/redis-docker-harness-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-docker-harness-0.0.2.tar", last modified: Thu Jul  6 23:23:40 2023, max compression
+gzip compressed data, was "redis-docker-harness-0.0.3.tar", last modified: Sun Jul  9 22:46:06 2023, max compression
```

## Comparing `redis-docker-harness-0.0.2.tar` & `redis-docker-harness-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      220 2023-07-06 23:22:44.000000 redis-docker-harness-0.0.2/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      125 2021-09-21 22:04:15.000000 redis-docker-harness-0.0.2/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 redis-docker-harness-0.0.2/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1041 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2021-09-21 23:31:38.000000 redis-docker-harness-0.0.2/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1045 2023-07-06 23:22:44.000000 redis-docker-harness-0.0.2/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/src/rdh/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      185 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.2/src/rdh/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3280 2023-07-06 23:08:51.000000 redis-docker-harness-0.0.2/src/rdh/_argparse.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      203 2021-09-21 22:33:02.000000 redis-docker-harness-0.0.2/src/rdh/_log.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2502 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.2/src/rdh/_redis.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-06 23:23:40.063020 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1041 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      372 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2023-07-06 23:23:39.000000 redis-docker-harness-0.0.2/src/redis_docker_harness.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.527516 redis-docker-harness-0.0.3/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      322 2023-07-09 22:44:55.000000 redis-docker-harness-0.0.3/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      125 2021-09-21 22:04:15.000000 redis-docker-harness-0.0.3/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 redis-docker-harness-0.0.3/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1191 2023-07-09 22:46:06.527516 redis-docker-harness-0.0.3/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2021-09-21 23:31:38.000000 redis-docker-harness-0.0.3/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-09 22:46:06.527516 redis-docker-harness-0.0.3/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1045 2023-07-09 22:44:55.000000 redis-docker-harness-0.0.3/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.523517 redis-docker-harness-0.0.3/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.523517 redis-docker-harness-0.0.3/src/rdh/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      185 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.3/src/rdh/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     3388 2023-07-09 22:42:14.000000 redis-docker-harness-0.0.3/src/rdh/_argparse.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      203 2021-09-21 22:33:02.000000 redis-docker-harness-0.0.3/src/rdh/_log.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2502 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.3/src/rdh/_redis.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.523517 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1191 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      372 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/top_level.txt
```

### Comparing `redis-docker-harness-0.0.2/setup.py` & `redis-docker-harness-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,11 +31,11 @@
     },
     packages=[
         "rdh",
     ],
     install_requires=[
         "redis",
     ],
-    version="0.0.2",
+    version="0.0.3",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
 )
```

### Comparing `redis-docker-harness-0.0.2/src/rdh/_argparse.py` & `redis-docker-harness-0.0.3/src/rdh/_argparse.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,16 +45,17 @@
     :rtype: bool
     """
     if hasattr(ns, "redis_password"):
         if ns.redis_password is not None:
             return True
 
     if hasattr(ns, "redis_password_env"):
-        if os.getenv(ns.redis_password_env) is not None:
-            return True
+        if ns.redis_password_env is not None:
+            if os.getenv(ns.redis_password_env) is not None:
+                return True
 
     return False
 
 
 def get_password(ns):
     """
     Returns the password from the namespace (supplied either directly or via environment variable).
@@ -65,11 +66,12 @@
     :rtype: str
     """
     if hasattr(ns, "redis_password"):
         if ns.redis_password is not None:
             return ns.redis_password
 
     if hasattr(ns, "redis_password_env"):
-        if os.getenv(ns.redis_password_env) is not None:
-            return os.getenv(ns.redis_password_env)
+        if ns.redis_password_env is not None:
+            if os.getenv(ns.redis_password_env) is not None:
+                return os.getenv(ns.redis_password_env)
 
     return None
```

### Comparing `redis-docker-harness-0.0.2/src/rdh/_redis.py` & `redis-docker-harness-0.0.3/src/rdh/_redis.py`

 * *Files identical despite different names*

