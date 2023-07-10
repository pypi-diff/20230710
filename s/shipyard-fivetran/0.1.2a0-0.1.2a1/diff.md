# Comparing `tmp/shipyard_fivetran-0.1.2a0.tar.gz` & `tmp/shipyard_fivetran-0.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_fivetran-0.1.2a0.tar", max compression
+gzip compressed data, was "shipyard_fivetran-0.1.2a1.tar", max compression
```

## Comparing `shipyard_fivetran-0.1.2a0.tar` & `shipyard_fivetran-0.1.2a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      722 2023-07-10 20:51:27.386196 shipyard_fivetran-0.1.2a0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.2a0/shipyard_fivetran/__init__.py
--rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.2a0/shipyard_fivetran/cli/authtest.py
--rw-r--r--   0        0        0     3012 2023-07-10 20:44:53.454669 shipyard_fivetran-0.1.2a0/shipyard_fivetran/cli/sync.py
--rw-r--r--   0        0        0     2150 2023-07-10 20:44:53.455303 shipyard_fivetran-0.1.2a0/shipyard_fivetran/cli/update_connector.py
--rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.2a0/shipyard_fivetran/fivetran.py
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0      721 2023-07-10 20:59:28.685073 shipyard_fivetran-0.1.2a1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.2a1/shipyard_fivetran/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/authtest.py
+-rw-r--r--   0        0        0     3012 2023-07-10 20:44:53.454669 shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/sync.py
+-rw-r--r--   0        0        0     2150 2023-07-10 20:44:53.455303 shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/update_connector.py
+-rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.2a1/shipyard_fivetran/fivetran.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.2a1/PKG-INFO
```

### Comparing `shipyard_fivetran-0.1.2a0/pyproject.toml` & `shipyard_fivetran-0.1.2a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "shipyard-fivetran"
-version = "0.1.2a0"
+version = "0.1.2a1"
 description = "A local client for connecting and working with Fivetran"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>", "wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 #readme = "README.md"
 packages = [{ include = "shipyard_fivetran" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytz = "2023.3"
 requests = "2.31.0"
-shipyard-templates = "0.1.6"
-shipyard-utils = "0.1.4"
+#shipyard-templates = "0.1.6"
+#shipyard-utils = "0.1.4"
 
 
-#[tool.poetry.group.dev.dependencies]
-##shipyard-bp-utils = { path = "../shipyard-bp-utils", develop = true }
-## shipyard-templates = { path = "../../shipyard-templates", develop = true }
+[tool.poetry.group.dev.dependencies]
+#shipyard-bp-utils = { path = "../shipyard-bp-utils", develop = true }
+# shipyard-templates = { path = "../../shipyard-templates", develop = true }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shipyard_fivetran-0.1.2a0/shipyard_fivetran/cli/sync.py` & `shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/sync.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a0/shipyard_fivetran/cli/update_connector.py` & `shipyard_fivetran-0.1.2a1/shipyard_fivetran/cli/update_connector.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a0/shipyard_fivetran/fivetran.py` & `shipyard_fivetran-0.1.2a1/shipyard_fivetran/fivetran.py`

 * *Files identical despite different names*

