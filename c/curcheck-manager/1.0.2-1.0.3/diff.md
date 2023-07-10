# Comparing `tmp/curcheck_manager-1.0.2.tar.gz` & `tmp/curcheck_manager-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curcheck_manager-1.0.2.tar", max compression
+gzip compressed data, was "curcheck_manager-1.0.3.tar", max compression
```

## Comparing `curcheck_manager-1.0.2.tar` & `curcheck_manager-1.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       89 2023-02-10 12:25:51.143879 curcheck_manager-1.0.2/curcheck_manager/__main__.py
--rw-r--r--   0        0        0     1077 2023-07-08 10:08:23.187672 curcheck_manager-1.0.2/curcheck_manager/app.py
--rw-r--r--   0        0        0      525 2023-06-24 17:25:28.673796 curcheck_manager-1.0.2/curcheck_manager/config.py
--rw-r--r--   0        0        0      173 2023-06-27 10:54:24.846875 curcheck_manager-1.0.2/curcheck_manager/context.py
--rw-r--r--   0        0        0       78 2023-03-08 07:24:30.482519 curcheck_manager-1.0.2/curcheck_manager/enums.py
--rw-r--r--   0        0        0     1998 2023-06-27 11:10:43.105873 curcheck_manager-1.0.2/curcheck_manager/generator.py
--rw-r--r--   0        0        0        0 2023-02-10 13:56:06.325380 curcheck_manager-1.0.2/curcheck_manager/templates/full/app/__init__.py
--rw-r--r--   0        0        0       53 2023-02-11 09:02:53.545791 curcheck_manager-1.0.2/curcheck_manager/templates/full/app/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-02-10 13:56:38.157436 curcheck_manager-1.0.2/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/__init__.py
--rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.2/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/models.py
--rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.2/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/views.py
--rw-r--r--   0        0        0       61 2023-02-11 08:05:26.713003 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/cookiecutter.json
--rw-r--r--   0        0        0       28 2023-06-23 09:02:15.026394 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/env.env
--rw-r--r--   0        0        0      296 2023-03-05 20:23:17.853251 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/main.py
--rw-r--r--   0        0        0      115 2023-03-05 20:23:17.860255 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.861256 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/readme.md
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.863563 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.872723 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/__init__.py
--rw-r--r--   0        0        0      314 2023-03-05 20:23:17.871723 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/app.py
--rw-r--r--   0        0        0      178 2023-06-23 08:52:42.460993 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.904817 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__init__.py
--rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/models.py
--rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/views.py
--rw-r--r--   0        0        0        0 2023-03-05 20:23:17.944825 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__init__.py
--rw-r--r--   0        0        0      423 2023-06-23 08:46:09.993536 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/bot_app.py
--rw-r--r--   0        0        0      678 2023-03-05 20:23:17.927821 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py
--rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/base.py
--rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
--rw-r--r--   0        0        0      298 2023-06-23 09:03:04.582318 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/settings.py
--rw-r--r--   0        0        0      289 2023-03-05 20:23:17.942824 curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
--rw-r--r--   0        0        0       61 2023-06-24 13:39:32.178390 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-27 08:26:16.394398 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/env.env
--rw-r--r--   0        0        0      824 2023-06-27 08:37:09.075765 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py
--rw-r--r--   0        0        0      337 2023-06-27 08:35:30.708961 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/db.py
--rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/base.py
--rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
--rw-r--r--   0        0        0      298 2023-06-27 08:27:46.134954 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/settings.py
--rw-r--r--   0        0        0      263 2023-06-27 08:31:54.772473 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
--rw-r--r--   0        0        0      168 2023-06-27 08:32:07.404070 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/models.py
--rw-r--r--   0        0        0      253 2023-06-27 08:28:02.541201 curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/router.py
--rw-r--r--   0        0        0     1085 2023-06-27 11:18:05.861249 curcheck_manager-1.0.2/LICENSE
--rw-r--r--   0        0        0      573 2023-07-08 11:49:10.129246 curcheck_manager-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       59 2023-06-27 11:11:21.093016 curcheck_manager-1.0.2/README.md
--rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 curcheck_manager-1.0.2/setup.py
--rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 curcheck_manager-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       89 2023-02-10 12:25:51.143879 curcheck_manager-1.0.3/curcheck_manager/__main__.py
+-rw-r--r--   0        0        0     1228 2023-07-10 09:18:42.466417 curcheck_manager-1.0.3/curcheck_manager/app.py
+-rw-r--r--   0        0        0      525 2023-06-24 17:25:28.673796 curcheck_manager-1.0.3/curcheck_manager/config.py
+-rw-r--r--   0        0        0      173 2023-06-27 10:54:24.846875 curcheck_manager-1.0.3/curcheck_manager/context.py
+-rw-r--r--   0        0        0       78 2023-03-08 07:24:30.482519 curcheck_manager-1.0.3/curcheck_manager/enums.py
+-rw-r--r--   0        0        0     1998 2023-06-27 11:10:43.105873 curcheck_manager-1.0.3/curcheck_manager/generator.py
+-rw-r--r--   0        0        0        0 2023-02-10 13:56:06.325380 curcheck_manager-1.0.3/curcheck_manager/templates/full/app/__init__.py
+-rw-r--r--   0        0        0       53 2023-02-11 09:02:53.545791 curcheck_manager-1.0.3/curcheck_manager/templates/full/app/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-02-10 13:56:38.157436 curcheck_manager-1.0.3/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/__init__.py
+-rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.3/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/models.py
+-rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.3/curcheck_manager/templates/full/app/{{ cookiecutter.app_name }}/views.py
+-rw-r--r--   0        0        0       61 2023-02-11 08:05:26.713003 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/cookiecutter.json
+-rw-r--r--   0        0        0       28 2023-06-23 09:02:15.026394 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/env.env
+-rw-r--r--   0        0        0      296 2023-03-05 20:23:17.853251 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/main.py
+-rw-r--r--   0        0        0      115 2023-03-05 20:23:17.860255 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.861256 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/readme.md
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.863563 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.872723 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/__init__.py
+-rw-r--r--   0        0        0      314 2023-03-05 20:23:17.871723 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/app.py
+-rw-r--r--   0        0        0      178 2023-06-23 08:52:42.460993 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.904817 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/__init__.py
+-rw-r--r--   0        0        0      168 2023-03-05 20:23:17.902824 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/models.py
+-rw-r--r--   0        0        0      253 2023-06-23 08:56:09.139441 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/apps/main/views.py
+-rw-r--r--   0        0        0        0 2023-03-05 20:23:17.944825 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/__init__.py
+-rw-r--r--   0        0        0      423 2023-06-23 08:46:09.993536 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/bot_app.py
+-rw-r--r--   0        0        0      678 2023-03-05 20:23:17.927821 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py
+-rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/base.py
+-rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
+-rw-r--r--   0        0        0      298 2023-06-23 09:03:04.582318 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/settings.py
+-rw-r--r--   0        0        0      289 2023-03-05 20:23:17.942824 curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
+-rw-r--r--   0        0        0       61 2023-06-24 13:39:32.178390 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-06-27 08:26:16.394398 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/env.env
+-rw-r--r--   0        0        0      824 2023-06-27 08:37:09.075765 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py
+-rw-r--r--   0        0        0      337 2023-06-27 08:35:30.708961 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/db.py
+-rw-r--r--   0        0        0      408 2023-03-05 20:23:17.953810 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/base.py
+-rw-r--r--   0        0        0      349 2023-03-05 20:23:17.962097 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/models/timestamp.py
+-rw-r--r--   0        0        0      298 2023-06-27 08:27:46.134954 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/settings.py
+-rw-r--r--   0        0        0      263 2023-06-27 08:31:54.772473 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/core/tortoise_orm.py
+-rw-r--r--   0        0        0      168 2023-06-27 08:32:07.404070 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/models.py
+-rw-r--r--   0        0        0      253 2023-06-27 08:28:02.541201 curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/src/router.py
+-rw-r--r--   0        0        0     1085 2023-06-27 11:18:05.861249 curcheck_manager-1.0.3/LICENSE
+-rw-r--r--   0        0        0      573 2023-07-10 09:19:20.345661 curcheck_manager-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-06-27 11:11:21.093016 curcheck_manager-1.0.3/README.md
+-rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 curcheck_manager-1.0.3/setup.py
+-rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 curcheck_manager-1.0.3/PKG-INFO
```

### Comparing `curcheck_manager-1.0.2/curcheck_manager/app.py` & `curcheck_manager-1.0.3/curcheck_manager/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,14 +32,19 @@
         generate_app(context)
     except TypeError:
         click.echo("Вы находитесь не в директории проекта curcheck!")
 
 
 @cli.command()
 @click.argument("project_name")
-@click.option('--full', '-f', is_flag=True, help="Fullish project")
-def startproject(project_name: str, is_full: bool):
+@click.option('--full', 'project_size', flag_value='full')
+@click.option(
+    '--mini', 'project_size', flag_value='mini', default=True
+)
+def startproject(project_name: str, project_size: str):
+    if project_size == "full": is_full = True
+    else: is_full = False
     context = ProjectContext(
         project_name=project_name,
         is_full=is_full
     )
     generate_project(context)
```

### Comparing `curcheck_manager-1.0.2/curcheck_manager/config.py` & `curcheck_manager-1.0.3/curcheck_manager/config.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.2/curcheck_manager/generator.py` & `curcheck_manager-1.0.3/curcheck_manager/generator.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.2/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py` & `curcheck_manager-1.0.3/curcheck_manager/templates/full/project/{{ cookiecutter.project_name }}/src/core/db.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.2/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py` & `curcheck_manager-1.0.3/curcheck_manager/templates/mini/project/{{ cookiecutter.project_name }}/main.py`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.2/LICENSE` & `curcheck_manager-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `curcheck_manager-1.0.2/pyproject.toml` & `curcheck_manager-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "curcheck-manager"
-version = "1.0.2"
+version = "1.0.3"
 description = "Managing curcheck projects"
 authors = ["BulatXam <Khamdbulat@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `curcheck_manager-1.0.2/setup.py` & `curcheck_manager-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'pydantic>=1.10.4']
 
 entry_points = \
 {'console_scripts': ['curcheck = curcheck_manager.app:cli']}
 
 setup_kwargs = {
     'name': 'curcheck-manager',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'Managing curcheck projects',
     'long_description': '# Curcheck-manager\n___\n\n\nManager for curcheck library\n',
     'author': 'BulatXam',
     'author_email': 'Khamdbulat@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `curcheck_manager-1.0.2/PKG-INFO` & `curcheck_manager-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curcheck-manager
-Version: 1.0.2
+Version: 1.0.3
 Summary: Managing curcheck projects
 License: MIT
 Author: BulatXam
 Author-email: Khamdbulat@yandex.ru
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

