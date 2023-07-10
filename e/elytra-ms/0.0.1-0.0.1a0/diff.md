# Comparing `tmp/elytra-ms-0.0.1.tar.gz` & `tmp/elytra-ms-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elytra-ms-0.0.1.tar", last modified: Mon Jul 10 04:41:26 2023, max compression
+gzip compressed data, was "elytra-ms-0.0.1a0.tar", last modified: Mon Jul 10 04:49:39 2023, max compression
```

## Comparing `elytra-ms-0.0.1.tar` & `elytra-ms-0.0.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:41:26.464216 elytra-ms-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-10 04:41:26.464216 elytra-ms-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:41:26.464216 elytra-ms-0.0.1/elytra/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/elytra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/elytra/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/elytra/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/elytra/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:41:26.464216 elytra-ms-0.0.1/elytra_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-10 04:41:26.000000 elytra-ms-0.0.1/elytra_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-10 04:41:26.000000 elytra-ms-0.0.1/elytra_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:41:26.000000 elytra-ms-0.0.1/elytra_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 04:41:26.000000 elytra-ms-0.0.1/elytra_ms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 04:41:26.000000 elytra-ms-0.0.1/elytra_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 04:41:26.000000 elytra-ms-0.0.1/elytra_ms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:41:26.464216 elytra-ms-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-10 04:41:11.000000 elytra-ms-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:49:39.831180 elytra-ms-0.0.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-10 04:49:39.831180 elytra-ms-0.0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:49:39.827180 elytra-ms-0.0.1a0/elytra/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/elytra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/elytra/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/elytra/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/elytra/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:49:39.831180 elytra-ms-0.0.1a0/elytra_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-10 04:49:39.000000 elytra-ms-0.0.1a0/elytra_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-10 04:49:39.000000 elytra-ms-0.0.1a0/elytra_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:49:39.000000 elytra-ms-0.0.1a0/elytra_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-10 04:49:39.000000 elytra-ms-0.0.1a0/elytra_ms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 04:49:39.000000 elytra-ms-0.0.1a0/elytra_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 04:49:39.000000 elytra-ms-0.0.1a0/elytra_ms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:49:39.831180 elytra-ms-0.0.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-10 04:49:18.000000 elytra-ms-0.0.1a0/setup.py
```

### Comparing `elytra-ms-0.0.1/LICENSE` & `elytra-ms-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `elytra-ms-0.0.1/PKG-INFO` & `elytra-ms-0.0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elytra-ms
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 Home-page: https://github.com/AstreaTSS/elytra-ms
 Author: AstreaTSS
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elytra-ms-0.0.1/README.md` & `elytra-ms-0.0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `elytra-ms-0.0.1/elytra/core.py` & `elytra-ms-0.0.1a0/elytra/core.py`

 * *Files identical despite different names*

### Comparing `elytra-ms-0.0.1/elytra/protocols.py` & `elytra-ms-0.0.1a0/elytra/protocols.py`

 * *Files identical despite different names*

### Comparing `elytra-ms-0.0.1/elytra_ms.egg-info/PKG-INFO` & `elytra-ms-0.0.1a0/elytra_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elytra-ms
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: A Python Library for various Microsoft APIs, including the Xbox and Bedrock Realms APIs.
 Home-page: https://github.com/AstreaTSS/elytra-ms
 Author: AstreaTSS
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elytra-ms-0.0.1/pyproject.toml` & `elytra-ms-0.0.1a0/pyproject.toml`

 * *Files identical despite different names*

