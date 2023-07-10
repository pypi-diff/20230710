# Comparing `tmp/shipyard_fivetran-0.1.2a1.tar.gz` & `tmp/shipyard_fivetran-0.1.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_fivetran-0.1.2a1.tar", max compression
+gzip compressed data, was "shipyard_fivetran-0.1.2a3.tar", max compression
```

## Comparing `shipyard_fivetran-0.1.2a1.tar` & `shipyard_fivetran-0.1.2a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      721 2023-07-10 20:59:28.685073 shipyard_fivetran-0.1.2a1/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.2a1/shipyard_fivetran/__init__.py
--rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/authtest.py
--rw-r--r--   0        0        0     3012 2023-07-10 20:44:53.454669 shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/sync.py
--rw-r--r--   0        0        0     2150 2023-07-10 20:44:53.455303 shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/update_connector.py
--rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.2a1/shipyard_fivetran/fivetran.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.2a1/PKG-INFO
+-rw-r--r--   0        0        0      689 2023-07-10 21:17:38.271191 shipyard_fivetran-0.1.2a3/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.2a3/shipyard_fivetran/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.2a3/shipyard_fivetran/cli/authtest.py
+-rw-r--r--   0        0        0     3012 2023-07-10 20:44:53.454669 shipyard_fivetran-0.1.2a3/shipyard_fivetran/cli/sync.py
+-rw-r--r--   0        0        0     2150 2023-07-10 20:44:53.455303 shipyard_fivetran-0.1.2a3/shipyard_fivetran/cli/update_connector.py
+-rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.2a3/shipyard_fivetran/fivetran.py
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.2a3/PKG-INFO
```

### Comparing `shipyard_fivetran-0.1.2a1/pyproject.toml` & `shipyard_fivetran-0.1.2a3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [tool.poetry]
 name = "shipyard-fivetran"
-version = "0.1.2a1"
+version = "0.1.2a3"
 description = "A local client for connecting and working with Fivetran"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>", "wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 #readme = "README.md"
 packages = [{ include = "shipyard_fivetran" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytz = "2023.3"
 requests = "2.31.0"
-#shipyard-templates = "0.1.6"
-#shipyard-utils = "0.1.4"
-
+shipyard-bp-utils = "0.1.0"
 
 [tool.poetry.group.dev.dependencies]
-#shipyard-bp-utils = { path = "../shipyard-bp-utils", develop = true }
-# shipyard-templates = { path = "../../shipyard-templates", develop = true }
+shipyard-bp-utils = { path = "../shipyard-bp-utils", develop = true }
+shipyard-templates = { path = "../../shipyard-templates", develop = true }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/sync.py` & `shipyard_fivetran-0.1.2a3/shipyard_fivetran/cli/sync.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/update_connector.py` & `shipyard_fivetran-0.1.2a3/shipyard_fivetran/cli/update_connector.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a1/shipyard_fivetran/fivetran.py` & `shipyard_fivetran-0.1.2a3/shipyard_fivetran/fivetran.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a1/PKG-INFO` & `shipyard_fivetran-0.1.2a3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: shipyard-fivetran
-Version: 0.1.2a1
+Version: 0.1.2a3
 Summary: A local client for connecting and working with Fivetran
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytz (==2023.3)
 Requires-Dist: requests (==2.31.0)
+Requires-Dist: shipyard-bp-utils (==0.1.0)
```

