# Comparing `tmp/web_ext_helper-1.2.0.tar.gz` & `tmp/web_ext_helper-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.2.0.tar", max compression
+gzip compressed data, was "web_ext_helper-1.2.1.tar", max compression
```

## Comparing `web_ext_helper-1.2.0.tar` & `web_ext_helper-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.2.0/LICENSE
--rw-r--r--   0        0        0      659 2023-07-09 21:14:29.386245 web_ext_helper-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.2.0/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.2.0/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.2.0/web_ext_helper/functions.py
--rw-r--r--   0        0        0    21525 2023-07-09 21:14:12.816226 web_ext_helper-1.2.0/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.2.1/LICENSE
+-rw-r--r--   0        0        0      659 2023-07-10 12:43:08.965202 web_ext_helper-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.2.1/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.2.1/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.2.1/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    21443 2023-07-10 12:44:38.926176 web_ext_helper-1.2.1/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.2.1/PKG-INFO
```

### Comparing `web_ext_helper-1.2.0/LICENSE` & `web_ext_helper-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.2.0/pyproject.toml` & `web_ext_helper-1.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.2.0"
+version = "1.2.1"
 description = "An awesome CLI for building, publishing and running web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.2.0/README.md` & `web_ext_helper-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.2.0/web_ext_helper/functions.py` & `web_ext_helper-1.2.1/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.2.0/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.2.1/web_ext_helper/web_ext_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.2.0"
+__ext_version__ = "1.2.1"
 
 import os
 import sys
 import json
 import shutil
 import typer
 import zipfile
@@ -37,17 +37,15 @@
              \/    \/               \/      \/                     \/     \/     |__|        \/       
 
  Version: {bcolors.PURPLE}{__ext_version__}{bcolors.OKGREEN}
  An awesome CLI for {bcolors.OKCYAN}building{bcolors.OKGREEN}, {bcolors.OKCYAN}publishing {bcolors.OKGREEN}and {bcolors.OKCYAN}running {bcolors.PURPLE}web extensions.{bcolors.ENDC}"""
 
 load_dotenv(cached_app_data_env_dir)
 
-app = typer.Typer(
-    help="An awseome CLI for building, publishing and running web extensions."
-)
+app = typer.Typer()
 
 try:
     with open("src/manifest.json", "r") as manifest_file:
         manifest_data = json.load(manifest_file)
 
     manifest_name = manifest_data["name"]
     manifest_name_lower = manifest_data["name"].lower()
```

### Comparing `web_ext_helper-1.2.0/PKG-INFO` & `web_ext_helper-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.2.0
+Version: 1.2.1
 Summary: An awesome CLI for building, publishing and running web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

