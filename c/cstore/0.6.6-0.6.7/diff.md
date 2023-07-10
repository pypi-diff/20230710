# Comparing `tmp/cstore-0.6.6.tar.gz` & `tmp/cstore-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstore-0.6.6.tar", last modified: Wed Jun 28 22:02:04 2023, max compression
+gzip compressed data, was "cstore-0.6.7.tar", last modified: Mon Jul 10 11:06:09 2023, max compression
```

## Comparing `cstore-0.6.6.tar` & `cstore-0.6.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 22:02:04.576137 cstore-0.6.6/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.6/LICENSE
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-06-28 22:02:04.572137 cstore-0.6.6/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     5529 2023-06-28 19:59:47.000000 cstore-0.6.6/README.md
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 22:02:04.572137 cstore-0.6.6/cstore/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       21 2023-06-28 21:59:24.000000 cstore-0.6.6/cstore/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15491 2023-06-28 22:01:24.000000 cstore-0.6.6/cstore/cli.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.6/cstore/constants.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      481 2023-06-27 12:02:50.000000 cstore-0.6.6/cstore/database.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1007 2023-06-28 10:47:25.000000 cstore-0.6.6/cstore/models.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 22:02:04.572137 cstore-0.6.6/cstore/repo/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 10:48:25.000000 cstore-0.6.6/cstore/repo/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2931 2023-06-28 21:58:54.000000 cstore-0.6.6/cstore/repo/repo_command.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1341 2023-06-28 21:57:57.000000 cstore-0.6.6/cstore/repo/repo_tag.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1757 2023-06-25 23:16:56.000000 cstore-0.6.6/cstore/schemes.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.6/cstore/verbose.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 22:02:04.572137 cstore-0.6.6/cstore.egg-info/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-06-28 22:02:04.000000 cstore-0.6.6/cstore.egg-info/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-06-28 22:02:04.000000 cstore-0.6.6/cstore.egg-info/SOURCES.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-06-28 22:02:04.000000 cstore-0.6.6/cstore.egg-info/dependency_links.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-06-28 22:02:04.000000 cstore-0.6.6/cstore.egg-info/entry_points.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       74 2023-06-28 22:02:04.000000 cstore-0.6.6/cstore.egg-info/requires.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-06-28 22:02:04.000000 cstore-0.6.6/cstore.egg-info/top_level.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      926 2023-06-28 21:59:33.000000 cstore-0.6.6/pyproject.toml
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-06-28 22:02:04.576137 cstore-0.6.6/setup.cfg
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:06:09.470382 cstore-0.6.7/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.7/LICENSE
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-07-10 11:06:09.466382 cstore-0.6.7/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     5529 2023-07-10 11:04:36.000000 cstore-0.6.7/README.md
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:06:09.466382 cstore-0.6.7/cstore/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       21 2023-06-28 21:59:24.000000 cstore-0.6.7/cstore/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15491 2023-07-10 11:03:50.000000 cstore-0.6.7/cstore/cli.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.7/cstore/constants.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      481 2023-06-27 12:02:50.000000 cstore-0.6.7/cstore/database.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1007 2023-06-28 10:47:25.000000 cstore-0.6.7/cstore/models.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:06:09.466382 cstore-0.6.7/cstore/repo/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 10:48:25.000000 cstore-0.6.7/cstore/repo/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2931 2023-06-28 21:58:54.000000 cstore-0.6.7/cstore/repo/repo_command.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1341 2023-06-28 21:57:57.000000 cstore-0.6.7/cstore/repo/repo_tag.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1757 2023-06-25 23:16:56.000000 cstore-0.6.7/cstore/schemes.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.7/cstore/verbose.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:06:09.466382 cstore-0.6.7/cstore.egg-info/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-07-10 11:06:09.000000 cstore-0.6.7/cstore.egg-info/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-07-10 11:06:09.000000 cstore-0.6.7/cstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-07-10 11:06:09.000000 cstore-0.6.7/cstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-07-10 11:06:09.000000 cstore-0.6.7/cstore.egg-info/entry_points.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       74 2023-07-10 11:06:09.000000 cstore-0.6.7/cstore.egg-info/requires.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-07-10 11:06:09.000000 cstore-0.6.7/cstore.egg-info/top_level.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      926 2023-07-10 11:04:58.000000 cstore-0.6.7/pyproject.toml
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-07-10 11:06:09.470382 cstore-0.6.7/setup.cfg
```

### Comparing `cstore-0.6.6/LICENSE` & `cstore-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cstore-0.6.6/PKG-INFO` & `cstore-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.6
+Version: 0.6.7
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Documentation, https://github.com/navidved/ctore
 Project-URL: Repository, https://github.com/navidved/ctore
 Classifier: Programming Language :: Python :: 3
@@ -105,11 +105,11 @@
 ( Code structure and comments: Enhancing code structure and adding comprehensive comments.
 * Join us in shaping the future of "CStore" by contributing to these exciting features and improvements. Stay tuned for updates!
 
 > Special thanks to the developers of the following packages:
   - pydantic
   - typer
   - cryptocode
-  - pyperclip
+  - clipboard
   - simple_term_menu
   - rich
   - SQLAlchemy
```

### Comparing `cstore-0.6.6/README.md` & `cstore-0.6.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -89,11 +89,11 @@
 ( Code structure and comments: Enhancing code structure and adding comprehensive comments.
 * Join us in shaping the future of "CStore" by contributing to these exciting features and improvements. Stay tuned for updates!
 
 > Special thanks to the developers of the following packages:
   - pydantic
   - typer
   - cryptocode
-  - pyperclip
+  - clipboard
   - simple_term_menu
   - rich
   - SQLAlchemy
```

### Comparing `cstore-0.6.6/cstore/cli.py` & `cstore-0.6.7/cstore/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 from typing import Optional, List
 from typing_extensions import Annotated
 from os.path import exists
-import pyperclip
+import clipboard
 from rich.console import Console
 from rich.prompt import Prompt
 from rich import print
 from typer import Typer, Option, Exit, Context, confirm, Abort, prompt
 from simple_term_menu import TerminalMenu
 import cryptocode
 
@@ -70,17 +70,17 @@
                     f"please enter a password to decrypt '{selected_command.body}'", hide_input=True)
                 decrypted_command = cryptocode.decrypt(
                     selected_command.description, password)
                 if not decrypted_command:
                     print("invalid password!")
                     raise Exit()
 
-                pyperclip.copy(decrypted_command)
+                clipboard.copy(decrypted_command)
             else:
-                pyperclip.copy(selected_command.body)
+                clipboard.copy(selected_command.body)
             print(
                 f"Command id {selected_command.id} copied to clipboard!")
 
 
 class ConcreteAddAction(BaseAction):
     def execute(self):
         command: Command = None
```

### Comparing `cstore-0.6.6/cstore/models.py` & `cstore-0.6.7/cstore/models.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.6/cstore/repo/repo_command.py` & `cstore-0.6.7/cstore/repo/repo_command.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.6/cstore/repo/repo_tag.py` & `cstore-0.6.7/cstore/repo/repo_tag.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.6/cstore/schemes.py` & `cstore-0.6.7/cstore/schemes.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.6/cstore/verbose.py` & `cstore-0.6.7/cstore/verbose.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.6/cstore.egg-info/PKG-INFO` & `cstore-0.6.7/cstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.6
+Version: 0.6.7
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Documentation, https://github.com/navidved/ctore
 Project-URL: Repository, https://github.com/navidved/ctore
 Classifier: Programming Language :: Python :: 3
@@ -105,11 +105,11 @@
 ( Code structure and comments: Enhancing code structure and adding comprehensive comments.
 * Join us in shaping the future of "CStore" by contributing to these exciting features and improvements. Stay tuned for updates!
 
 > Special thanks to the developers of the following packages:
   - pydantic
   - typer
   - cryptocode
-  - pyperclip
+  - clipboard
   - simple_term_menu
   - rich
   - SQLAlchemy
```

### Comparing `cstore-0.6.6/pyproject.toml` & `cstore-0.6.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cstore"
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
     "pydantic",
     "typer[all]",
     "rich",
     "simple_term_menu",
     "SQLAlchemy",
-    "pyperclip",
+    "clipboard",
     "cryptocode",
 ]
 authors = [
   { name="Navid Arabi", email="navidved@gmail.com" },
 ]
 description = "A tools to store and recall useful commands, specifically created to assist forgetful individuals"
 readme = "README.md"
```

