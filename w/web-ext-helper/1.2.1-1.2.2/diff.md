# Comparing `tmp/web_ext_helper-1.2.1.tar.gz` & `tmp/web_ext_helper-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.2.1.tar", max compression
+gzip compressed data, was "web_ext_helper-1.2.2.tar", max compression
```

## Comparing `web_ext_helper-1.2.1.tar` & `web_ext_helper-1.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.2.1/LICENSE
--rw-r--r--   0        0        0      659 2023-07-10 12:43:08.965202 web_ext_helper-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.2.1/README.md
--rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.2.1/web_ext_helper/classes.py
--rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.2.1/web_ext_helper/functions.py
--rw-r--r--   0        0        0    21443 2023-07-10 12:44:38.926176 web_ext_helper-1.2.1/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.2.2/LICENSE
+-rw-r--r--   0        0        0      659 2023-07-10 13:07:29.114628 web_ext_helper-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1871 2023-06-19 17:29:34.258602 web_ext_helper-1.2.2/README.md
+-rw-r--r--   0        0        0      262 2023-06-18 17:57:02.181036 web_ext_helper-1.2.2/web_ext_helper/classes.py
+-rw-r--r--   0        0        0      613 2023-06-18 17:49:15.766872 web_ext_helper-1.2.2/web_ext_helper/functions.py
+-rw-r--r--   0        0        0    21453 2023-07-10 13:07:04.966061 web_ext_helper-1.2.2/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2441 1970-01-01 00:00:00.000000 web_ext_helper-1.2.2/PKG-INFO
```

### Comparing `web_ext_helper-1.2.1/LICENSE` & `web_ext_helper-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.2.1/pyproject.toml` & `web_ext_helper-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.2.1"
+version = "1.2.2"
 description = "An awesome CLI for building, publishing and running web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.2.1/README.md` & `web_ext_helper-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.2.1/web_ext_helper/functions.py` & `web_ext_helper-1.2.2/web_ext_helper/functions.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.2.1/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.2.2/web_ext_helper/web_ext_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__ext_version__ = "1.2.1"
+__ext_version__ = "1.2.2"
 
 import os
 import sys
 import json
 import shutil
 import typer
 import zipfile
@@ -30,17 +30,17 @@
 
 web_ext_helper_logo = rf"""{bcolors.OKGREEN}
               ___.                              __            .__           .__                       
 __  _  __ ____\_ |__             ____ ___  ____/  |_          |  |__   ____ |  | ______   ___________ 
 \ \/ \/ // __ \| __ \   ______ _/ __ \\  \/  /\   __\  ______ |  |  \_/ __ \|  | \____ \_/ __ \_  __ \
  \     /\  ___/| \_\ \ /_____/ \  ___/ >    <  |  |   /_____/ |   Y  \  ___/|  |_|  |_> >  ___/|  | \/
   \/\_/  \___  >___  /          \___  >__/\_ \ |__|           |___|  /\___  >____/   __/ \___  >__|   
-             \/    \/               \/      \/                     \/     \/     |__|        \/       
+             \/    \/               \/      \/                     \/     \/     |__|        \/             {bcolors.PURPLE}v{__ext_version__}{bcolors.OKGREEN}
 
- Version: {bcolors.PURPLE}{__ext_version__}{bcolors.OKGREEN}
+             
  An awesome CLI for {bcolors.OKCYAN}building{bcolors.OKGREEN}, {bcolors.OKCYAN}publishing {bcolors.OKGREEN}and {bcolors.OKCYAN}running {bcolors.PURPLE}web extensions.{bcolors.ENDC}"""
 
 load_dotenv(cached_app_data_env_dir)
 
 app = typer.Typer()
 
 try:
```

### Comparing `web_ext_helper-1.2.1/PKG-INFO` & `web_ext_helper-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.2.1
+Version: 1.2.2
 Summary: An awesome CLI for building, publishing and running web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

