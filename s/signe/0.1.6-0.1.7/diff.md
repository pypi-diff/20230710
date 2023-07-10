# Comparing `tmp/signe-0.1.6.tar.gz` & `tmp/signe-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signe-0.1.6.tar", last modified: Sat Jul  8 17:46:47 2023, max compression
+gzip compressed data, was "signe-0.1.7.tar", last modified: Mon Jul 10 06:58:28 2023, max compression
```

## Comparing `signe-0.1.6.tar` & `signe-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.984504 signe-0.1.6/
--rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      469 2023-07-08 17:46:47.982508 signe-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 17:46:47.984504 signe-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.943071 signe-0.1.6/signe/
--rw-rw-rw-   0        0        0      223 2023-07-08 17:46:37.000000 signe-0.1.6/signe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.966704 signe-0.1.6/signe/core/
--rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.6/signe/core/__init__.py
--rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.6/signe/core/collections.py
--rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.6/signe/core/consts.py
--rw-rw-rw-   0        0        0     5939 2023-07-08 17:46:06.000000 signe-0.1.6/signe/core/effect.py
--rw-rw-rw-   0        0        0     2840 2023-07-08 17:46:06.000000 signe-0.1.6/signe/core/runtime.py
--rw-rw-rw-   0        0        0     2818 2023-07-08 17:46:06.000000 signe-0.1.6/signe/core/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.970692 signe-0.1.6/signe/reactive/
--rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.6/signe/reactive/__init__.py
--rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.6/signe/reactive/proxy.py
--rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.6/signe/types.py
--rw-rw-rw-   0        0        0     3637 2023-07-08 17:46:06.000000 signe-0.1.6/signe/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:46:47.953043 signe-0.1.6/signe.egg-info/
--rw-rw-rw-   0        0        0      469 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-08 17:46:47.000000 signe-0.1.6/signe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.213555 signe-0.1.7/
+-rw-rw-rw-   0        0        0     1088 2023-06-22 09:11:57.000000 signe-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      469 2023-07-10 06:58:28.194279 signe-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-25 14:01:29.000000 signe-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 06:58:28.213555 signe-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-06-25 12:31:47.000000 signe-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.168317 signe-0.1.7/signe/
+-rw-rw-rw-   0        0        0      225 2023-07-10 06:58:13.000000 signe-0.1.7/signe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.188277 signe-0.1.7/signe/core/
+-rw-rw-rw-   0        0        0        0 2023-06-25 12:24:57.000000 signe-0.1.7/signe/core/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-07-06 05:25:51.000000 signe-0.1.7/signe/core/collections.py
+-rw-rw-rw-   0        0        0      290 2023-06-25 12:24:57.000000 signe-0.1.7/signe/core/consts.py
+-rw-rw-rw-   0        0        0     5939 2023-07-08 17:46:06.000000 signe-0.1.7/signe/core/effect.py
+-rw-rw-rw-   0        0        0     2840 2023-07-08 17:46:06.000000 signe-0.1.7/signe/core/runtime.py
+-rw-rw-rw-   0        0        0     2818 2023-07-08 17:46:06.000000 signe-0.1.7/signe/core/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.192290 signe-0.1.7/signe/reactive/
+-rw-rw-rw-   0        0        0        0 2023-06-27 15:43:57.000000 signe-0.1.7/signe/reactive/__init__.py
+-rw-rw-rw-   0        0        0     7480 2023-06-25 12:24:57.000000 signe-0.1.7/signe/reactive/proxy.py
+-rw-rw-rw-   0        0        0       97 2023-06-25 12:24:57.000000 signe-0.1.7/signe/types.py
+-rw-rw-rw-   0        0        0     5319 2023-07-10 06:58:11.000000 signe-0.1.7/signe/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:58:28.178293 signe-0.1.7/signe.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-10 06:58:27.000000 signe-0.1.7/signe.egg-info/top_level.txt
```

### Comparing `signe-0.1.6/LICENSE` & `signe-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `signe-0.1.6/README.md` & `signe-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `signe-0.1.6/setup.py` & `signe-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.6/signe/core/collections.py` & `signe-0.1.7/signe/core/collections.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.6/signe/core/effect.py` & `signe-0.1.7/signe/core/effect.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.6/signe/core/runtime.py` & `signe-0.1.7/signe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.6/signe/core/signal.py` & `signe-0.1.7/signe/core/signal.py`

 * *Files identical despite different names*

### Comparing `signe-0.1.6/signe/reactive/proxy.py` & `signe-0.1.7/signe/reactive/proxy.py`

 * *Files identical despite different names*

