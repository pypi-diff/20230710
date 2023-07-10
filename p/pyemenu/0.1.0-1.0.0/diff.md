# Comparing `tmp/pyemenu-0.1.0.tar.gz` & `tmp/pyemenu-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemenu-0.1.0.tar", last modified: Fri May 26 22:37:13 2023, max compression
+gzip compressed data, was "pyemenu-1.0.0.tar", last modified: Mon Jul 10 18:15:45 2023, max compression
```

## Comparing `pyemenu-0.1.0.tar` & `pyemenu-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/
--rw-r--r--   0 zero      (1000) zero      (1000)     1083 2023-05-26 17:53:37.000000 pyemenu-0.1.0/LICENSE.txt
--rw-r--r--   0 zero      (1000) zero      (1000)     4659 2023-05-26 22:37:13.426324 pyemenu-0.1.0/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)     3694 2023-05-26 22:34:11.000000 pyemenu-0.1.0/README.md
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/pyemenu/
--rw-r--r--   0 zero      (1000) zero      (1000)       22 2023-05-26 22:18:14.000000 pyemenu-0.1.0/pyemenu/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     3308 2023-05-26 21:04:58.000000 pyemenu-0.1.0/pyemenu/menu.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/pyemenu.egg-info/
--rw-r--r--   0 zero      (1000) zero      (1000)     4659 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)      234 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/SOURCES.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        1 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/dependency_links.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        9 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/requires.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        8 2023-05-26 22:37:13.000000 pyemenu-0.1.0/pyemenu.egg-info/top_level.txt
--rw-r--r--   0 zero      (1000) zero      (1000)       38 2023-05-26 22:37:13.426324 pyemenu-0.1.0/setup.cfg
--rw-r--r--   0 zero      (1000) zero      (1000)     2112 2023-05-26 22:36:35.000000 pyemenu-0.1.0/setup.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-05-26 22:37:13.426324 pyemenu-0.1.0/tests/
--rw-r--r--   0 zero      (1000) zero      (1000)        2 2023-05-26 19:16:06.000000 pyemenu-0.1.0/tests/test.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:15:45.373232 pyemenu-1.0.0/
+-rw-r--r--   0 freire    (1000) freire    (1000)     1083 2023-05-30 03:04:58.000000 pyemenu-1.0.0/LICENSE.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)    10417 2023-07-10 18:15:45.373232 pyemenu-1.0.0/PKG-INFO
+-rw-r--r--   0 freire    (1000) freire    (1000)     9406 2023-07-10 17:52:04.000000 pyemenu-1.0.0/README.md
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:15:45.373232 pyemenu-1.0.0/pyemenu/
+-rw-r--r--   0 freire    (1000) freire    (1000)     1251 2023-07-10 15:58:05.000000 pyemenu-1.0.0/pyemenu/__init__.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     7861 2023-07-10 15:58:05.000000 pyemenu-1.0.0/pyemenu/colors.py
+-rw-r--r--   0 freire    (1000) freire    (1000)     3470 2023-07-10 15:58:05.000000 pyemenu-1.0.0/pyemenu/tools.py
+drwxr-xr-x   0 freire    (1000) freire    (1000)        0 2023-07-10 18:15:45.373232 pyemenu-1.0.0/pyemenu.egg-info/
+-rw-r--r--   0 freire    (1000) freire    (1000)    10417 2023-07-10 18:15:45.000000 pyemenu-1.0.0/pyemenu.egg-info/PKG-INFO
+-rw-r--r--   0 freire    (1000) freire    (1000)      239 2023-07-10 18:15:45.000000 pyemenu-1.0.0/pyemenu.egg-info/SOURCES.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        1 2023-07-10 18:15:45.000000 pyemenu-1.0.0/pyemenu.egg-info/dependency_links.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        9 2023-07-10 18:15:45.000000 pyemenu-1.0.0/pyemenu.egg-info/requires.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)        8 2023-07-10 18:15:45.000000 pyemenu-1.0.0/pyemenu.egg-info/top_level.txt
+-rw-r--r--   0 freire    (1000) freire    (1000)       38 2023-07-10 18:15:45.373232 pyemenu-1.0.0/setup.cfg
+-rw-r--r--   0 freire    (1000) freire    (1000)     2164 2023-07-10 15:58:05.000000 pyemenu-1.0.0/setup.py
```

### Comparing `pyemenu-0.1.0/LICENSE.txt` & `pyemenu-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemenu-0.1.0/setup.py` & `pyemenu-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 with open("README.md", "r", encoding= "utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
     name = 'pyemenu',         # How you named your package folder (MyLib)
     packages = ['pyemenu'],
-    version = '0.1.0',      # Start with a small number and increase it with every change you make
+    version = '1.0.0',      # Start with a small number and increase it with every change you make
     author = 'Freire Alexander Palomino Palma',                   # Type in your name
     author_email = 'freirealexander0214@gmail.com',      # Type in your E-Mail
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-    description = 'Easy customizable menu for CLI',   # Give a short description about your library
+    description = 'Easy and Simple kit for develop Text User Interfaces',   # Give a short description about your library
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/FreireAlexander/PyeMenu',   # Provide either the link to your github or to your website
-    download_url = 'https://github.com/FreireAlexander/PyeMenu/releases/tag/0.1.0',
+    download_url = 'https://github.com/FreireAlexander/PyeMenu/releases/tag/1.0.0',
     project_urls = {
         "Bug Tracker": "https://github.com/FreireAlexander/PyeMenu/issues",
     },
     #download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
-    keywords = ['MENU', 'CLI', 'command line'],   # Keywords that define your package best
+    keywords = ['MENU', 'CLI', 'command line', 'TUI', 'Text User Interface'],   # Keywords that define your package best
     install_requires=[            # I get to this in a second
             'readchar',
         ],
     classifiers=[
       'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
       'Intended Audience :: Developers',      # Define that your audience are developers
       'Topic :: Software Development :: Build Tools',
```

