# Comparing `tmp/pyemenu-1.0.6.dev0.tar.gz` & `tmp/pyemenu-1.0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemenu-1.0.6.dev0.tar", last modified: Mon Jul 10 19:06:42 2023, max compression
+gzip compressed data, was "pyemenu-1.0.7.dev0.tar", last modified: Mon Jul 10 19:12:45 2023, max compression
```

## Comparing `pyemenu-1.0.6.dev0.tar` & `pyemenu-1.0.7.dev0.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:06:42.073231 pyemenu-1.0.6.dev0/
--rw-r--r--   0 freire    (1000) freire    (1000)     1083 2023-05-30 03:04:58.000000 pyemenu-1.0.6.dev0/LICENSE.txt
--rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 19:06:42.073231 pyemenu-1.0.6.dev0/PKG-INFO
--rw-r--r--   0 freire    (1000) freire    (1000)     9406 2023-07-10 17:52:04.000000 pyemenu-1.0.6.dev0/README.md
-drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:06:42.063231 pyemenu-1.0.6.dev0/pyemenu/
--rw-r--r--   0 freire    (1000) freire    (1000)     1251 2023-07-10 19:06:16.000000 pyemenu-1.0.6.dev0/pyemenu/__init__.py
--rw-r--r--   0 freire    (1000) freire    (1000)     7861 2023-07-10 15:58:05.000000 pyemenu-1.0.6.dev0/pyemenu/colors.py
--rw-r--r--   0 freire    (1000) freire    (1000)     3470 2023-07-10 15:58:05.000000 pyemenu-1.0.6.dev0/pyemenu/tools.py
-drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:06:42.073231 pyemenu-1.0.6.dev0/pyemenu.egg-info/
--rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 19:06:42.000000 pyemenu-1.0.6.dev0/pyemenu.egg-info/PKG-INFO
--rw-r--r--   0 freire    (1000) freire    (1000)      239 2023-07-10 19:06:42.000000 pyemenu-1.0.6.dev0/pyemenu.egg-info/SOURCES.txt
--rw-r--r--   0 freire    (1000) freire    (1000)        1 2023-07-10 19:06:42.000000 pyemenu-1.0.6.dev0/pyemenu.egg-info/dependency_links.txt
--rw-r--r--   0 freire    (1000) freire    (1000)        9 2023-07-10 19:06:42.000000 pyemenu-1.0.6.dev0/pyemenu.egg-info/requires.txt
--rw-r--r--   0 freire    (1000) freire    (1000)        8 2023-07-10 19:06:42.000000 pyemenu-1.0.6.dev0/pyemenu.egg-info/top_level.txt
--rw-r--r--   0 freire    (1000) freire    (1000)       38 2023-07-10 19:06:42.073231 pyemenu-1.0.6.dev0/setup.cfg
--rw-r--r--   0 freire    (1000) freire    (1000)     2168 2023-07-10 19:06:22.000000 pyemenu-1.0.6.dev0/setup.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:12:45.923227 pyemenu-1.0.7.dev0/
+-rw-r--r--   0 freire    (1000) freire    (1000)     1083 2023-05-30 03:04:58.000000 pyemenu-1.0.7.dev0/LICENSE.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 19:12:45.913227 pyemenu-1.0.7.dev0/PKG-INFO
+-rw-r--r--   0 freire    (1000) freire    (1000)     9406 2023-07-10 17:52:04.000000 pyemenu-1.0.7.dev0/README.md
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:12:45.913227 pyemenu-1.0.7.dev0/pyemenu/
+-rw-r--r--   0 freire    (1000) freire    (1000)     1251 2023-07-10 19:06:16.000000 pyemenu-1.0.7.dev0/pyemenu/__init__.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     7861 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/colors.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:12:45.913227 pyemenu-1.0.7.dev0/pyemenu/components/
+-rw-r--r--   0 freire    (1000) freire    (1000)      540 2023-07-10 19:11:58.000000 pyemenu-1.0.7.dev0/pyemenu/components/__init__.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     1668 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/components/buttons.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     2545 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/components/checkboxs.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     8262 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/components/entries.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     4494 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/components/texts.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     5531 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/components/titles.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     3470 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/tools.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:12:45.913227 pyemenu-1.0.7.dev0/pyemenu/widgets/
+-rw-r--r--   0 freire    (1000) freire    (1000)      524 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/widgets/__init__.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     9181 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/widgets/checkboxlists.py
+-rw-r--r--   0 freire    (1000) freire    (1000)    15496 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/widgets/forms.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     6780 2023-07-10 15:58:05.000000 pyemenu-1.0.7.dev0/pyemenu/widgets/menus.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 19:12:45.913227 pyemenu-1.0.7.dev0/pyemenu.egg-info/
+-rw-r--r--   0 freire    (1000) freire    (1000)    10422 2023-07-10 19:12:45.000000 pyemenu-1.0.7.dev0/pyemenu.egg-info/PKG-INFO
+-rw-r--r--   0 freire    (1000) freire    (1000)      530 2023-07-10 19:12:45.000000 pyemenu-1.0.7.dev0/pyemenu.egg-info/SOURCES.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        1 2023-07-10 19:12:45.000000 pyemenu-1.0.7.dev0/pyemenu.egg-info/dependency_links.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        9 2023-07-10 19:12:45.000000 pyemenu-1.0.7.dev0/pyemenu.egg-info/requires.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        8 2023-07-10 19:12:45.000000 pyemenu-1.0.7.dev0/pyemenu.egg-info/top_level.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)       38 2023-07-10 19:12:45.923227 pyemenu-1.0.7.dev0/setup.cfg
+-rw-r--r--   0 freire    (1000) freire    (1000)     2185 2023-07-10 19:12:41.000000 pyemenu-1.0.7.dev0/setup.py
```

### Comparing `pyemenu-1.0.6.dev0/LICENSE.txt` & `pyemenu-1.0.7.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.6.dev0/PKG-INFO` & `pyemenu-1.0.7.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 1.0.6.dev0
+Version: 1.0.7.dev0
 Summary: Easy and Simple kit for develop Text User Interfaces
 Home-page: https://github.com/FreireAlexander/PyeMenu
 Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/1.0.0
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
```

### Comparing `pyemenu-1.0.6.dev0/README.md` & `pyemenu-1.0.7.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.6.dev0/pyemenu/__init__.py` & `pyemenu-1.0.7.dev0/pyemenu/__init__.py`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.6.dev0/pyemenu/colors.py` & `pyemenu-1.0.7.dev0/pyemenu/colors.py`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.6.dev0/pyemenu/tools.py` & `pyemenu-1.0.7.dev0/pyemenu/tools.py`

 * *Files identical despite different names*

### Comparing `pyemenu-1.0.6.dev0/pyemenu.egg-info/PKG-INFO` & `pyemenu-1.0.7.dev0/pyemenu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemenu
-Version: 1.0.6.dev0
+Version: 1.0.7.dev0
 Summary: Easy and Simple kit for develop Text User Interfaces
 Home-page: https://github.com/FreireAlexander/PyeMenu
 Download-URL: https://github.com/FreireAlexander/PyeMenu/releases/tag/1.0.0
 Author: Freire Alexander Palomino Palma
 Author-email: freirealexander0214@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/FreireAlexander/PyeMenu/issues
```

### Comparing `pyemenu-1.0.6.dev0/setup.py` & `pyemenu-1.0.7.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import setuptools
+from setuptools import setup, find_packages
 with open("README.md", "r", encoding= "utf-8") as fh:
   long_description = fh.read()
 
-setuptools.setup(
+setup(
     name = 'pyemenu',         # How you named your package folder (MyLib)
-    packages = ['pyemenu'],
-    version = '1.0.6-dev',      # Start with a small number and increase it with every change you make
+    packages=find_packages(),
+    version = '1.0.7-dev',      # Start with a small number and increase it with every change you make
     author = 'Freire Alexander Palomino Palma',                   # Type in your name
     author_email = 'freirealexander0214@gmail.com',      # Type in your E-Mail
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Easy and Simple kit for develop Text User Interfaces',   # Give a short description about your library
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/FreireAlexander/PyeMenu',   # Provide either the link to your github or to your website
```

