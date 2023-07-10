# Comparing `tmp/ario3s_aiva-0.5.0.tar.gz` & `tmp/ario3s_aiva-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ario3s_aiva-0.5.0.tar", max compression
+gzip compressed data, was "ario3s_aiva-0.6.0.tar", max compression
```

## Comparing `ario3s_aiva-0.5.0.tar` & `ario3s_aiva-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0      507 2023-01-28 19:05:51.993512 ario3s_aiva-0.5.0/README.md
--rw-r--r--   0        0        0       22 2023-01-28 18:59:26.961435 ario3s_aiva-0.5.0/ario3s_aiva/__init__.py
--rw-r--r--   0        0        0       40 2023-01-14 09:52:31.824096 ario3s_aiva-0.5.0/ario3s_aiva/__main__.py
--rw-r--r--   0        0        0     2648 2023-01-28 18:51:36.056691 ario3s_aiva-0.5.0/ario3s_aiva/main.py
--rw-r--r--   0        0        0      513 2023-01-28 18:59:21.805442 ario3s_aiva-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 ario3s_aiva-0.5.0/setup.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 ario3s_aiva-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      507 2023-01-28 19:05:51.993512 ario3s_aiva-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-10 17:02:31.152014 ario3s_aiva-0.6.0/ario3s_aiva/__init__.py
+-rw-r--r--   0        0        0       40 2023-01-14 09:52:31.824096 ario3s_aiva-0.6.0/ario3s_aiva/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-10 13:49:28.549551 ario3s_aiva-0.6.0/ario3s_aiva/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 13:50:11.356796 ario3s_aiva-0.6.0/ario3s_aiva/commands/connect.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:34:56.748546 ario3s_aiva-0.6.0/ario3s_aiva/commands.py
+-rw-r--r--   0        0        0     7664 2023-07-10 17:01:20.807083 ario3s_aiva-0.6.0/ario3s_aiva/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:19:16.358495 ario3s_aiva-0.6.0/ario3s_aiva/utils/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-10 17:02:40.002717 ario3s_aiva-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 ario3s_aiva-0.6.0/setup.py
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 ario3s_aiva-0.6.0/PKG-INFO
```

### Comparing `ario3s_aiva-0.5.0/pyproject.toml` & `ario3s_aiva-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "ario3s-aiva"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["ario <cybera.3s@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ario3s_aiva"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tomli = "^2.0.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^23.1a1", allow-prereleases = true}
+flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 aiva = "ario3s_aiva.main:app"
```

### Comparing `ario3s_aiva-0.5.0/setup.py` & `ario3s_aiva-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['ario3s_aiva']
+['ario3s_aiva', 'ario3s_aiva.commands', 'ario3s_aiva.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['tomli>=2.0.1,<3.0.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['aiva = ario3s_aiva.main:app']}
 
 setup_kwargs = {
     'name': 'ario3s-aiva',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': '',
     'long_description': "# aiva cli tool\n\n<p>a tool to connect to server using ssh</p>\n<p>it creates a SOCKS proxy on provided port default to 4321</p>\n\n\n## Configuration\n<p>Default config file path is /home/<username>/.aiva.toml\n\n<b>Config file Format</b>\n\n```\n[server]\nip = <server-ip>\nserver_port = <server-port>\nusername = '<username>'\nlocal_port = <local-port>\n```\n</p>\n\n## Usage\n\nconnects to server using ssh\n```\naiva connect  \n```\n\ndisconnects from server\n```\naiva disconnect  \n```\nget connection status\n```\naiva status  \n```",
     'author': 'ario',
     'author_email': 'cybera.3s@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ario3s_aiva-0.5.0/PKG-INFO` & `ario3s_aiva-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ario3s-aiva
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: ario
 Author-email: cybera.3s@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

