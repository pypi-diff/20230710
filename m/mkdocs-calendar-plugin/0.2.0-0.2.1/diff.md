# Comparing `tmp/mkdocs_calendar_plugin-0.2.0.tar.gz` & `tmp/mkdocs_calendar_plugin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_calendar_plugin-0.2.0.tar", max compression
+gzip compressed data, was "mkdocs_calendar_plugin-0.2.1.tar", max compression
```

## Comparing `mkdocs_calendar_plugin-0.2.0.tar` & `mkdocs_calendar_plugin-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       25 2023-07-10 17:53:29.809741 mkdocs_calendar_plugin-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-10 17:53:29.809741 mkdocs_calendar_plugin-0.2.0/mkdocs_calendar/__init__.py
--rw-r--r--   0        0        0     3230 2023-07-10 17:53:29.809741 mkdocs_calendar_plugin-0.2.0/mkdocs_calendar/plugin.py
--rw-r--r--   0        0        0     1102 2023-07-10 17:53:29.813741 mkdocs_calendar_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/mkdocs_calendar/__init__.py
+-rw-r--r--   0        0        0     3230 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/mkdocs_calendar/plugin.py
+-rw-r--r--   0        0        0     1124 2023-07-10 18:49:47.627514 mkdocs_calendar_plugin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 mkdocs_calendar_plugin-0.2.1/PKG-INFO
```

### Comparing `mkdocs_calendar_plugin-0.2.0/mkdocs_calendar/plugin.py` & `mkdocs_calendar_plugin-0.2.1/mkdocs_calendar/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_calendar_plugin-0.2.0/pyproject.toml` & `mkdocs_calendar_plugin-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-calendar-plugin"
-version = "0.2.0"
+version = "0.2.1"
 description = "An MkDocs plugin to ..."
 authors = ["Jacques Supcik <jacques.supcik@hefr.ch>"]
 repository = "https://github.com/supcik/mkdocs-today-plugin"
 license = "Apache-2"
 readme = "README.md"
 packages = [{ include = "mkdocs_calendar" }]
 keywords = ["mkdocs", "python", "markdown", "wiki"]
@@ -25,14 +25,15 @@
 [tool.poetry.extras]
 test = ["mkdocs-material", "mkdocs-macros-plugin"]
 
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

### Comparing `mkdocs_calendar_plugin-0.2.0/PKG-INFO` & `mkdocs_calendar_plugin-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-calendar-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: An MkDocs plugin to ...
 Home-page: https://github.com/supcik/mkdocs-today-plugin
 License: Apache-2
 Keywords: mkdocs,python,markdown,wiki
 Author: Jacques Supcik
 Author-email: jacques.supcik@hefr.ch
 Requires-Python: >=3.10,<4.0
```

