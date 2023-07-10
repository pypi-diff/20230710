# Comparing `tmp/making_with_code_cli-1.1.0.tar.gz` & `tmp/making_with_code_cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making_with_code_cli-1.1.0.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.2.0.tar", max compression
```

## Comparing `making_with_code_cli-1.1.0.tar` & `making_with_code_cli-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.1.0/README.md
--rw-r--r--   0        0        0     6410 2023-07-03 00:30:08.092007 making_with_code_cli-1.1.0/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    14782 2023-07-03 01:17:43.683351 making_with_code_cli-1.1.0/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      530 2023-07-02 19:59:44.714590 making_with_code_cli-1.1.0/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      277 2023-07-02 20:00:38.095929 making_with_code_cli-1.1.0/making_with_code_cli/errors.py
--rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0     2470 2023-06-05 21:06:58.811653 making_with_code_cli-1.1.0/making_with_code_cli/git_backend/mwc_backend.py
--rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.1.0/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     2285 2023-05-30 14:14:06.615841 making_with_code_cli-1.1.0/making_with_code_cli/mwc_api.py
--rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.1.0/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.1.0/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      663 2023-07-03 01:21:16.549208 making_with_code_cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.0/README.md
+-rw-r--r--   0        0        0     8206 2023-07-10 21:40:44.612254 making_with_code_cli-1.2.0/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    15392 2023-07-10 20:16:58.660240 making_with_code_cli-1.2.0/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.0/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.0/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     4024 2023-07-10 20:40:53.894216 making_with_code_cli-1.2.0/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.0/making_with_code_cli/git_wrapper.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.0/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.0/making_with_code_cli/mwc_accounts_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.0/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.0/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-10 21:45:57.855472 making_with_code_cli-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.0/PKG-INFO
```

### Comparing `making_with_code_cli-1.1.0/README.md` & `making_with_code_cli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/cli.py` & `making_with_code_cli-1.2.0/making_with_code_cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import click
 from pprint import pprint
 from pathlib import Path
-from subprocess import run
+from subprocess import run, CalledProcessError
 from importlib.metadata import metadata
 import yaml
 import toml
 import os
 import traceback
-from making_with_code_cli.mwc_api import MakingWithCodeAPI as API
+from making_with_code_cli.mwc_accounts_api import MWCAccountsAPI
 from making_with_code_cli.styles import (
     address,
     question,
     info,
     debug as debug_fmt,
     confirm,
     error,
@@ -24,14 +24,15 @@
 )
 from making_with_code_cli.cli_setup import (
     INTRO_MESSAGE,
     INTRO_NOTES,
     WORK_DIR_PERMISSIONS,
     Platform,
     choose_mwc_username,
+    prompt_mwc_password,
     choose_work_dir,
     choose_mwc_site_url,
     choose_course,
     choose_editor,
     MWCShellConfig,
     InstallCurl,
     InstallHomebrew,
@@ -49,14 +50,17 @@
 )
 from making_with_code_cli.curriculum import (
     get_curriculum,
 )
 from making_with_code_cli.git_backend import (
     get_backend,
 )
+from making_with_code_cli.git_wrapper import (
+    in_repo,
+)
 
 @click.group()
 def cli():
     "Command line interface for Making with Code"
 
 @cli.command()
 def version():
@@ -78,14 +82,27 @@
         click.echo(debug_fmt(f"Reading settings from {sp}"))
     rc_tasks = []
     click.echo(address(INTRO_MESSAGE))
     for note in INTRO_NOTES:
         click.echo(address(note, list_format=True))
     click.echo()
     settings['mwc_username'] = choose_mwc_username(settings.get("mwc_username"))
+    api = MWCAccountsAPI()
+    if settings.get('mwc_accounts_token'):
+        try:
+            status = api.get_status(settings['mwc_accounts_token'])
+        except api.RequestFailed as bad_token:
+            token = prompt_mwc_password(settings['mwc_username'])
+            settings['mwc_accounts_token'] = token
+            status = api.get_status(token)
+    else:
+        token = prompt_mwc_password(settings['mwc_username'])
+        settings['mwc_accounts_token'] = token
+        status = api.get_status(token)
+    settings['mwc_git_token'] = status['git_token']
     settings['role'] = "teacher" if teacher else "student"
     settings['work_dir'] = str(choose_work_dir(settings.get("work_dir")).resolve())
     settings['mwc_site_url'] = choose_mwc_site_url(settings.get('mwc_site_url'))
     curriculum = get_curriculum(settings)
     settings['course'] = choose_course(
         [course['name'] for course in curriculum['courses']], 
         default=settings.get('course')
@@ -116,15 +133,14 @@
         InstallPython3(settings),
         InstallGit(settings),
         InstallTree(settings),
         InstallVSCode(settings),
         InstallImageMagick(settings),
         InstallHttpie(settings),
         InstallScipy(settings),
-        GHAuthentication(settings),
         GitConfiguration(settings),
     ]
     errors = []
     for task in tasks:
         try:
             task.run_task_if_needed()
         except Exception as e:
@@ -132,15 +148,15 @@
     if errors:
         click.echo(error(f"{len(errors)} setup tasks failed:"))
         for task, tb in errors:
             click.echo(error(task.description))
             if debug:
                 click.echo(debug_fmt(tb, preformatted=True))
     else:
-        ctx.invoke(update)
+        ctx.invoke(update, config=config)
 
 def get_course_by_name(name, courses):
     for course in courses:
         if course['name'] == name:
             return course
 
 @cli.command()
@@ -171,16 +187,48 @@
             if module_dir.exists():
                 try:
                     G.update(module, module_dir)
                 except Exception as e:
                     msg =  traceback.format_exception(type(e), e, e.__traceback__)
                     print(error(''.join(msg)))
             else:
-                if 'init_action' in module:
-                    rel_dir = module_dir.resolve().relative_to(mwc_home)
-                    click.echo(confirm(f"Initializing {module['slug']} at {rel_dir}."))
-                    click.echo(confirm(f"See {module['url']} for details."))
-                    try:
-                        G.init_module(module, module_dir)
-                    except Exception as e:
-                        msg =  traceback.format_exception(type(e), e, e.__traceback__)
-                        click.echo(error(''.join(msg)))
+                rel_dir = module_dir.resolve().relative_to(mwc_home)
+                click.echo(confirm(f"Initializing {module['slug']} at {rel_dir}."))
+                click.echo(confirm(f"See {module['url']} for details."))
+                try:
+                    G.init_module(module, module_dir)
+                except Exception as e:
+                    msg =  traceback.format_exception(type(e), e, e.__traceback__)
+                    click.echo(error(''.join(msg)))
+
+@cli.command()
+def submit():
+    """Submit your work.
+    (This is a wrapper for the basic git workflow.)
+    """
+    if in_repo():
+        try:
+            result = run("git diff", shell=True, capture_output=True, text=True, check=True)
+            if not result.stdout:
+                click.echo(info("Everything is already up to date."))
+                return
+            run("git diff", shell=True, check=True)
+            if click.confirm(address("Here are the current changes. Looks OK?")):
+                run("git add -A", shell=True, capture_output=True, check=True)
+                click.echo(info("Write your commit message, then save and exit the window..."))
+                run("git commit", shell=True, capture_output=True, check=True)
+                run("git push", shell=True, capture_output=True, check=True)
+                click.echo(address("Nice job! All your work in this module has been submitted."))
+            else:
+                click.echo(info("Cancelled the submit for now."))
+        except CalledProcessError:
+            click.echo(info("Everything is already up to date."))
+    else:
+        click.echo(error("You are not in a lab, problem set, or project folder."))
+    
+
+
+
+
+
+
+
```

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.2.0/making_with_code_cli/cli_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from pathlib import Path
 from enum import Flag, auto
 from stat import *
 import sys
 import os
 import platform
+from making_with_code_cli.mwc_accounts_api import MWCAccountsAPI
 from making_with_code_cli.styles import (
     address,
     question,
     confirm,
     info,
     success,
     warn,
     error,
 )
+from making_with_code_cli.curriculum import (
+    get_curriculum,
+)
 from making_with_code_cli.errors import (
     CurriculumSiteNotAvailable,
     NoCurriculaAvailable,
 )
 import click
 import requests
 from subprocess import run
@@ -66,14 +70,25 @@
 def choose_mwc_username(default=None):
     """Asks the user to choose their MWC username."""
     return click.prompt(
         question("What is your MWC username?"),
         default=default
     )
 
+def prompt_mwc_password(username):
+    "Asks for the password. Returns a token when successful."
+    api = MWCAccountsAPI()
+    while True:
+        password = click.prompt(question("What is your MWC password?"), hide_input=True)
+        try:
+            response = api.login(username, password)
+            return response['token']
+        except api.RequestFailed:
+            click.echo(error(f"Sorry, that's not the right password for {username}."))
+
 def choose_work_dir(default=None):
     """Asks the user to choose where to save their work. 
     Loops until a valid choice is made, prompts if the directory is to be created, 
     and sets file permissions to 755 (u+rwx, g+x, o+x).
     """
     while True:
         work_dir = click.prompt(
@@ -98,14 +113,15 @@
             question("What's the URL of your Making With Code website?"),
             default=default,
         )
         if url.endswith('/'):
             url = url[:-1]
         try:
             curriculum = get_curriculum({'mwc_site_url': url})
+            return url
         except CurriculumSiteNotAvailable as err:
             click.echo(error(str(err)))
         except requests.exceptions.MissingSchema as e:
             click.echo(error(str(e)))
 
 def choose_course(options, default=None):
     """Asks the user which course they are part of"""
```

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/curriculum.py` & `making_with_code_cli-1.2.0/making_with_code_cli/curriculum.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import json
-from errors import CurriculumSiteNotAvailable
+from making_with_code_cli.errors import CurriculumSiteNotAvailable
 
 LIVE_RELOAD = '<script src="/livereload.js?port=1024&amp;mindelay=10"></script>'
 
 def get_curriculum(settings):
     """Fetches curriculum metadata from the site url specified in settings.
     """
     url = settings["mwc_site_url"] + "/manifest"
```

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.2.0/making_with_code_cli/git_backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/git_backend/github_org_backend.py` & `making_with_code_cli-1.2.0/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/settings.py` & `making_with_code_cli-1.2.0/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.1.0/making_with_code_cli/styles.py` & `making_with_code_cli-1.2.0/making_with_code_cli/styles.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.1.0/pyproject.toml` & `making_with_code_cli-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "1.1.0"
+version = "1.2.0"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
```

### Comparing `making_with_code_cli-1.1.0/PKG-INFO` & `making_with_code_cli-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

