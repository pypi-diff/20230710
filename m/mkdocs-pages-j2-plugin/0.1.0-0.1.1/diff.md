# Comparing `tmp/mkdocs_pages_j2_plugin-0.1.0.tar.gz` & `tmp/mkdocs_pages_j2_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_pages_j2_plugin-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_pages_j2_plugin-0.1.1.tar", max compression
```

## Comparing `mkdocs_pages_j2_plugin-0.1.0.tar` & `mkdocs_pages_j2_plugin-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      257 2023-06-15 18:15:52.427592 mkdocs_pages_j2_plugin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 09:13:11.740585 mkdocs_pages_j2_plugin-0.1.0/pagesj2/__init__.py
--rw-r--r--   0        0        0     2376 2023-06-15 19:08:53.798839 mkdocs_pages_j2_plugin-0.1.0/pagesj2/plugin.py
--rw-r--r--   0        0        0     1230 2023-06-15 19:07:28.095160 mkdocs_pages_j2_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 mkdocs_pages_j2_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      257 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/pagesj2/__init__.py
+-rw-r--r--   0        0        0     2376 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/pagesj2/plugin.py
+-rw-r--r--   0        0        0     1252 2023-07-10 19:17:22.635501 mkdocs_pages_j2_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 mkdocs_pages_j2_plugin-0.1.1/PKG-INFO
```

### Comparing `mkdocs_pages_j2_plugin-0.1.0/pagesj2/plugin.py` & `mkdocs_pages_j2_plugin-0.1.1/pagesj2/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_pages_j2_plugin-0.1.0/pyproject.toml` & `mkdocs_pages_j2_plugin-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-pages-j2-plugin"
-version = "0.1.0"
+version = "0.1.1"
 description = "An MkDocs plugin to generate .pages from pages.j2"
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-pages-j2-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "pagesj2" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
@@ -30,14 +30,15 @@
     "mkdocs-awesome-pages-plugin"
 ]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pylint = "^2.17.4"
 isort = "^5.12.0"
+pre-commit = "^3.3.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins]
```

### Comparing `mkdocs_pages_j2_plugin-0.1.0/PKG-INFO` & `mkdocs_pages_j2_plugin-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-pages-j2-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: An MkDocs plugin to generate .pages from pages.j2
 Home-page: https://github.com/supcik/mkdocs-pages-j2-plugin
 License: Apache-2
 Keywords: mkdocs,python,markdown,wiki
 Author: Jacques Supcik
 Author-email: jacques.supcik@hefr.ch
 Requires-Python: >=3.10,<4.0
```

