# Comparing `tmp/r614_config-0.1.6.tar.gz` & `tmp/r614_config-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r614_config-0.1.6.tar", max compression
+gzip compressed data, was "r614_config-0.1.7.tar", max compression
```

## Comparing `r614_config-0.1.6.tar` & `r614_config-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7052 2023-07-09 21:23:33.908234 r614_config-0.1.6/LICENSE
--rw-r--r--   0        0        0       16 2023-07-09 21:23:33.908290 r614_config-0.1.6/README.md
--rw-r--r--   0        0        0     1068 2023-07-09 21:24:27.383602 r614_config-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 21:23:33.908353 r614_config-0.1.6/r614_config/__init__.py
--rw-r--r--   0        0        0     2026 2023-07-09 21:23:33.908444 r614_config-0.1.6/r614_config/config.py
--rw-r--r--   0        0        0        0 2023-07-09 21:23:33.908472 r614_config-0.1.6/r614_config/py.typed
--rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 r614_config-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-07-09 21:23:33.908234 r614_config-0.1.7/LICENSE
+-rw-r--r--   0        0        0       16 2023-07-09 21:23:33.908290 r614_config-0.1.7/README.md
+-rw-r--r--   0        0        0     1068 2023-07-09 22:05:27.731058 r614_config-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 21:23:33.908353 r614_config-0.1.7/r614_config/__init__.py
+-rw-r--r--   0        0        0     2026 2023-07-09 21:23:33.908444 r614_config-0.1.7/r614_config/config.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:23:33.908472 r614_config-0.1.7/r614_config/py.typed
+-rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 r614_config-0.1.7/PKG-INFO
```

### Comparing `r614_config-0.1.6/LICENSE` & `r614_config-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `r614_config-0.1.6/pyproject.toml` & `r614_config-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "r614-config"
-version = "0.1.6"
+version = "0.1.7"
 description = "Shared config module"
 authors = ["Roshan Pawar <steradian614@gmail.com>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "r614_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `r614_config-0.1.6/r614_config/config.py` & `r614_config-0.1.7/r614_config/config.py`

 * *Files identical despite different names*

