# Comparing `tmp/pyemenu-1.0.1.dev0.tar.gz` & `tmp/pyemenu-1.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemenu-1.0.1.dev0.tar", last modified: Mon Jul 10 18:36:40 2023, max compression
+gzip compressed data, was "pyemenu-1.0.2.dev0.tar", last modified: Mon Jul 10 18:40:59 2023, max compression
```

## Comparing `pyemenu-1.0.1.dev0.tar` & `pyemenu-1.0.2.dev0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:36:40.213234 pyemenu-1.0.1.dev0/
--rw-r--r--   0 freire    (1000) freire    (1000)     1083 2023-05-30 03:04:58.000000 pyemenu-1.0.1.dev0/LICENSE.txt
--rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 18:36:40.213234 pyemenu-1.0.1.dev0/PKG-INFO
--rw-r--r--   0 freire    (1000) freire    (1000)     9406 2023-07-10 17:52:04.000000 pyemenu-1.0.1.dev0/README.md
-drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:36:40.213234 pyemenu-1.0.1.dev0/pyemenu/
--rw-r--r--   0 freire    (1000) freire    (1000)     1359 2023-07-10 18:36:29.000000 pyemenu-1.0.1.dev0/pyemenu/__init__.py
--rw-r--r--   0 freire    (1000) freire    (1000)     7861 2023-07-10 15:58:05.000000 pyemenu-1.0.1.dev0/pyemenu/colors.py
--rw-r--r--   0 freire    (1000) freire    (1000)     3470 2023-07-10 15:58:05.000000 pyemenu-1.0.1.dev0/pyemenu/tools.py
-drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:36:40.213234 pyemenu-1.0.1.dev0/pyemenu.egg-info/
--rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 18:36:40.000000 pyemenu-1.0.1.dev0/pyemenu.egg-info/PKG-INFO
--rw-r--r--   0 freire    (1000) freire    (1000)      239 2023-07-10 18:36:40.000000 pyemenu-1.0.1.dev0/pyemenu.egg-info/SOURCES.txt
--rw-r--r--   0 freire    (1000) freire    (1000)        1 2023-07-10 18:36:40.000000 pyemenu-1.0.1.dev0/pyemenu.egg-info/dependency_links.txt
--rw-r--r--   0 freire    (1000) freire    (1000)        9 2023-07-10 18:36:40.000000 pyemenu-1.0.1.dev0/pyemenu.egg-info/requires.txt
--rw-r--r--   0 freire    (1000) freire    (1000)        8 2023-07-10 18:36:40.000000 pyemenu-1.0.1.dev0/pyemenu.egg-info/top_level.txt
--rw-r--r--   0 freire    (1000) freire    (1000)       38 2023-07-10 18:36:40.213234 pyemenu-1.0.1.dev0/setup.cfg
--rw-r--r--   0 freire    (1000) freire    (1000)     2168 2023-07-10 18:29:18.000000 pyemenu-1.0.1.dev0/setup.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:40:59.973221 pyemenu-1.0.2.dev0/
+-rw-r--r--   0 freire    (1000) freire    (1000)     1083 2023-05-30 03:04:58.000000 pyemenu-1.0.2.dev0/LICENSE.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 18:40:59.973221 pyemenu-1.0.2.dev0/PKG-INFO
+-rw-r--r--   0 freire    (1000) freire    (1000)     9406 2023-07-10 17:52:04.000000 pyemenu-1.0.2.dev0/README.md
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:40:59.963221 pyemenu-1.0.2.dev0/pyemenu/
+-rw-r--r--   0 freire    (1000) freire    (1000)     1185 2023-07-10 18:40:10.000000 pyemenu-1.0.2.dev0/pyemenu/__init__.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     7861 2023-07-10 15:58:05.000000 pyemenu-1.0.2.dev0/pyemenu/colors.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     3470 2023-07-10 15:58:05.000000 pyemenu-1.0.2.dev0/pyemenu/tools.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:40:59.973221 pyemenu-1.0.2.dev0/pyemenu.egg-info/
+-rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 18:40:59.000000 pyemenu-1.0.2.dev0/pyemenu.egg-info/PKG-INFO
+-rw-r--r--   0 freire    (1000) freire    (1000)      239 2023-07-10 18:40:59.000000 pyemenu-1.0.2.dev0/pyemenu.egg-info/SOURCES.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        1 2023-07-10 18:40:59.000000 pyemenu-1.0.2.dev0/pyemenu.egg-info/dependency_links.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        9 2023-07-10 18:40:59.000000 pyemenu-1.0.2.dev0/pyemenu.egg-info/requires.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        8 2023-07-10 18:40:59.000000 pyemenu-1.0.2.dev0/pyemenu.egg-info/top_level.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)       38 2023-07-10 18:40:59.973221 pyemenu-1.0.2.dev0/setup.cfg
+-rw-r--r--   0 freire    (1000) freire    (1000)     2168 2023-07-10 18:40:21.000000 pyemenu-1.0.2.dev0/setup.py
```

### Comparing `pyemenu-1.0.1.dev0/LICENSE.txt` & `pyemenu-1.0.2.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.1.dev0/PKG-INFO` & `pyemenu-1.0.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 1.0.1.dev0
+Version: 1.0.2.dev0
 Summary: Easy and Simple kit for develop Text User Interfaces
 Home-page: https://github.com/FreireAlexander/PyeMenu
 Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/1.0.0
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
```

### Comparing `pyemenu-1.0.1.dev0/README.md` & `pyemenu-1.0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.1.dev0/pyemenu/__init__.py` & `pyemenu-1.0.2.dev0/pyemenu/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,17 +19,13 @@
         1. Colors -> A class with a lot of colors in hexadecimal format
     
     This package was developed by Freire Alexander Palomino Palma
     *Copyright (c) 2014-2023 Freire Alexander Palomino Palma*
 
     PyeMenu version 1.0.0
 """
-from .components.texts import Text
-from .components.titles import Title
-from .components.checkboxs import Checkbox
-from .components.entries import Entry
-from .components.buttons import Button
+import components
 from .widgets import *
 from .tools import clear_screen, getKeyboard
 from .colors import Colors
```

### Comparing `pyemenu-1.0.1.dev0/pyemenu/colors.py` & `pyemenu-1.0.2.dev0/pyemenu/colors.py`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.1.dev0/pyemenu/tools.py` & `pyemenu-1.0.2.dev0/pyemenu/tools.py`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.1.dev0/pyemenu.egg-info/PKG-INFO` & `pyemenu-1.0.2.dev0/pyemenu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 1.0.1.dev0
+Version: 1.0.2.dev0
 Summary: Easy and Simple kit for develop Text User Interfaces
 Home-page: https://github.com/FreireAlexander/PyeMenu
 Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/1.0.0
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
```

### Comparing `pyemenu-1.0.1.dev0/setup.py` & `pyemenu-1.0.2.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 with open("README.md", "r", encoding= "utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
     name = 'pyemenu',         # How you named your package folder (MyLib)
     packages = ['pyemenu'],
-    version = '1.0.1-dev',      # Start with a small number and increase it with every change you make
+    version = '1.0.2-dev',      # Start with a small number and increase it with every change you make
     author = 'Freire Alexander Palomino Palma',                   # Type in your name
     author_email = 'freirealexander0214@gmail.com',      # Type in your E-Mail
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Easy and Simple kit for develop Text User Interfaces',   # Give a short description about your library
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/FreireAlexander/PyeMenu',   # Provide either the link to your github or to your website
```

