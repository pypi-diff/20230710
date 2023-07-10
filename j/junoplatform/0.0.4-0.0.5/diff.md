# Comparing `tmp/junoplatform-0.0.4.tar.gz` & `tmp/junoplatform-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junoplatform-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "junoplatform-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `junoplatform-0.0.4.tar` & `junoplatform-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-10 07:45:23.535265 junoplatform-0.0.4/README.md
--rw-r--r--   0        0        0      622 2023-07-10 08:41:12.261896 junoplatform-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.4/src/junoplatform/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 07:47:41.758337 junoplatform-0.0.4/src/junoplatform/io/__init__.py
--rw-r--r--   0        0        0       26 2023-07-10 07:59:43.895947 junoplatform-0.0.4/src/junoplatform/io/input.py
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 junoplatform-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 07:45:23.535265 junoplatform-0.0.5/README.md
+-rw-r--r--   0        0        0      609 2023-07-10 08:44:22.805652 junoplatform-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.5/src/junoplatform/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:47:41.758337 junoplatform-0.0.5/src/junoplatform/io/__init__.py
+-rw-r--r--   0        0        0       26 2023-07-10 07:59:43.895947 junoplatform-0.0.5/src/junoplatform/io/input.py
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 junoplatform-0.0.5/PKG-INFO
```

### Comparing `junoplatform-0.0.4/pyproject.toml` & `junoplatform-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project.scripts]
-junocli = "junoplatform.tools.cmd:main"
+junocli = "tools.cmd:main"
 
 [project]
 name = "junoplatform"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Bruce.Lu", email="lzbgt@icloud.com" },
 ]
 description = "juno AI platform lib"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

