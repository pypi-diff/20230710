# Comparing `tmp/ario3s_aiva-0.6.0.tar.gz` & `tmp/ario3s_aiva-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ario3s_aiva-0.6.0.tar", max compression
+gzip compressed data, was "ario3s_aiva-1.0.0.tar", max compression
```

## Comparing `ario3s_aiva-0.6.0.tar` & `ario3s_aiva-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,19 @@
--rw-r--r--   0        0        0      507 2023-01-28 19:05:51.993512 ario3s_aiva-0.6.0/README.md
--rw-r--r--   0        0        0       22 2023-07-10 17:02:31.152014 ario3s_aiva-0.6.0/ario3s_aiva/__init__.py
--rw-r--r--   0        0        0       40 2023-01-14 09:52:31.824096 ario3s_aiva-0.6.0/ario3s_aiva/__main__.py
--rw-r--r--   0        0        0        0 2023-07-10 13:49:28.549551 ario3s_aiva-0.6.0/ario3s_aiva/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 13:50:11.356796 ario3s_aiva-0.6.0/ario3s_aiva/commands/connect.py
--rw-r--r--   0        0        0        0 2023-05-15 08:34:56.748546 ario3s_aiva-0.6.0/ario3s_aiva/commands.py
--rw-r--r--   0        0        0     7664 2023-07-10 17:01:20.807083 ario3s_aiva-0.6.0/ario3s_aiva/main.py
--rw-r--r--   0        0        0        0 2023-07-10 14:19:16.358495 ario3s_aiva-0.6.0/ario3s_aiva/utils/__init__.py
--rw-r--r--   0        0        0      531 2023-07-10 17:02:40.002717 ario3s_aiva-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 ario3s_aiva-0.6.0/setup.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 ario3s_aiva-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      507 2023-01-28 19:05:51.993512 ario3s_aiva-1.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-10 20:39:48.916032 ario3s_aiva-1.0.0/ario3s_aiva/__init__.py
+-rw-r--r--   0        0        0       40 2023-01-14 09:52:31.824096 ario3s_aiva-1.0.0/ario3s_aiva/__main__.py
+-rw-r--r--   0        0        0       37 2023-07-10 19:31:07.815125 ario3s_aiva-1.0.0/ario3s_aiva/commands/__init__.py
+-rw-r--r--   0        0        0     1656 2023-07-10 20:39:01.251714 ario3s_aiva-1.0.0/ario3s_aiva/commands/change_server.py
+-rw-r--r--   0        0        0      891 2023-07-10 19:29:33.646192 ario3s_aiva-1.0.0/ario3s_aiva/commands/connect.py
+-rw-r--r--   0        0        0      555 2023-07-10 19:28:04.957168 ario3s_aiva-1.0.0/ario3s_aiva/commands/disconnect.py
+-rw-r--r--   0        0        0      344 2023-07-10 19:28:13.973280 ario3s_aiva-1.0.0/ario3s_aiva/commands/list_servers.py
+-rw-r--r--   0        0        0      660 2023-07-10 19:28:19.841351 ario3s_aiva-1.0.0/ario3s_aiva/commands/restart.py
+-rw-r--r--   0        0        0      979 2023-07-10 19:28:26.745434 ario3s_aiva-1.0.0/ario3s_aiva/commands/status.py
+-rw-r--r--   0        0        0      132 2023-07-10 18:58:36.624633 ario3s_aiva-1.0.0/ario3s_aiva/config.py
+-rw-r--r--   0        0        0      668 2023-07-10 19:39:09.354250 ario3s_aiva-1.0.0/ario3s_aiva/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 18:53:18.528666 ario3s_aiva-1.0.0/ario3s_aiva/utils/__init__.py
+-rw-r--r--   0        0        0     2617 2023-07-10 19:22:02.230868 ario3s_aiva-1.0.0/ario3s_aiva/utils/config_file.py
+-rw-r--r--   0        0        0      696 2023-07-10 19:21:14.485689 ario3s_aiva-1.0.0/ario3s_aiva/utils/os_commands.py
+-rw-r--r--   0        0        0     2245 2023-07-10 19:30:46.574926 ario3s_aiva-1.0.0/ario3s_aiva/utils/run_command.py
+-rw-r--r--   0        0        0      579 2023-07-10 20:39:58.792093 ario3s_aiva-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 ario3s_aiva-1.0.0/setup.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 ario3s_aiva-1.0.0/PKG-INFO
```

### Comparing `ario3s_aiva-0.6.0/pyproject.toml` & `ario3s_aiva-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [tool.poetry]
 name = "ario3s-aiva"
-version = "0.6.0"
+version = "1.0.0"
 description = ""
 authors = ["ario <cybera.3s@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ario3s_aiva"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tomli = "^2.0.1"
 typer = {extras = ["all"], version = "^0.7.0"}
+toml = "^0.10.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^23.1a1", allow-prereleases = true}
 flake8 = "^6.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-aiva = "ario3s_aiva.main:app" 
+aiva = "ario3s_aiva.main:app" 
+
+[tool.black]
+line-length = 79
```

### Comparing `ario3s_aiva-0.6.0/setup.py` & `ario3s_aiva-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['ario3s_aiva', 'ario3s_aiva.commands', 'ario3s_aiva.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['tomli>=2.0.1,<3.0.0', 'typer[all]>=0.7.0,<0.8.0']
+['toml>=0.10.2,<0.11.0', 'tomli>=2.0.1,<3.0.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['aiva = ario3s_aiva.main:app']}
 
 setup_kwargs = {
     'name': 'ario3s-aiva',
-    'version': '0.6.0',
+    'version': '1.0.0',
     'description': '',
     'long_description': "# aiva cli tool\n\n<p>a tool to connect to server using ssh</p>\n<p>it creates a SOCKS proxy on provided port default to 4321</p>\n\n\n## Configuration\n<p>Default config file path is /home/<username>/.aiva.toml\n\n<b>Config file Format</b>\n\n```\n[server]\nip = <server-ip>\nserver_port = <server-port>\nusername = '<username>'\nlocal_port = <local-port>\n```\n</p>\n\n## Usage\n\nconnects to server using ssh\n```\naiva connect  \n```\n\ndisconnects from server\n```\naiva disconnect  \n```\nget connection status\n```\naiva status  \n```",
     'author': 'ario',
     'author_email': 'cybera.3s@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ario3s_aiva-0.6.0/PKG-INFO` & `ario3s_aiva-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ario3s-aiva
-Version: 0.6.0
+Version: 1.0.0
 Summary: 
 Author: ario
 Author-email: cybera.3s@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # aiva cli tool
 
 <p>a tool to connect to server using ssh</p>
```

