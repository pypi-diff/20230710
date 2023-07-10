# Comparing `tmp/pypipypipypipypipypipypipypi-0.1.tar.gz` & `tmp/pypipypipypipypipypipypipypi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipypipypipypipypipypipypi-0.1.tar", last modified: Mon Jul 10 13:39:36 2023, max compression
+gzip compressed data, was "pypipypipypipypipypipypipypi-0.2.tar", last modified: Mon Jul 10 14:09:57 2023, max compression
```

## Comparing `pypipypipypipypipypipypipypi-0.1.tar` & `pypipypipypipypipypipypipypi-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-10 13:39:36.088200 pypipypipypipypipypipypipypi-0.1/
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-10 13:15:14.000000 pypipypipypipypipypipypipypi-0.1/LICENSE.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)      796 2023-07-10 13:39:36.088457 pypipypipypipypipypipypipypi-0.1/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)       13 2023-07-10 12:46:08.000000 pypipypipypipypipypipypipypi-0.1/README.md
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-10 13:39:36.085618 pypipypipypipypipypipypipypi-0.1/pypipypipypipypipypipypipypi.egg-info/
--rw-r--r--   0 vedantrathi   (501) staff       (20)      796 2023-07-10 13:39:35.000000 pypipypipypipypipypipypipypi-0.1/pypipypipypipypipypipypipypi.egg-info/PKG-INFO
--rw-r--r--   0 vedantrathi   (501) staff       (20)      346 2023-07-10 13:39:35.000000 pypipypipypipypipypipypipypi-0.1/pypipypipypipypipypipypipypi.egg-info/SOURCES.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-10 13:39:35.000000 pypipypipypipypipypipypipypi-0.1/pypipypipypipypipypipypipypi.egg-info/dependency_links.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)        6 2023-07-10 13:39:35.000000 pypipypipypipypipypipypipypi-0.1/pypipypipypipypipypipypipypi.egg-info/requires.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       12 2023-07-10 13:39:35.000000 pypipypipypipypipypipypipypi-0.1/pypipypipypipypipypipypipypi.egg-info/top_level.txt
--rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-10 13:39:36.089411 pypipypipypipypipypipypipypi-0.1/setup.cfg
--rw-r--r--   0 vedantrathi   (501) staff       (20)     1668 2023-07-10 13:38:35.000000 pypipypipypipypipypipypipypi-0.1/setup.py
-drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-10 13:39:36.086871 pypipypipypipypipypipypipypi-0.1/testpackage/
--rw-r--r--   0 vedantrathi   (501) staff       (20)        0 2023-07-10 12:39:56.000000 pypipypipypipypipypipypipypi-0.1/testpackage/__init__.py
--rw-r--r--   0 vedantrathi   (501) staff       (20)      304 2023-07-10 12:44:59.000000 pypipypipypipypipypipypipypi-0.1/testpackage/example.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-10 14:09:57.328661 pypipypipypipypipypipypipypi-0.2/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1065 2023-07-10 13:15:14.000000 pypipypipypipypipypipypipypi-0.2/LICENSE.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      796 2023-07-10 14:09:57.328884 pypipypipypipypipypipypipypi-0.2/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       13 2023-07-10 12:46:08.000000 pypipypipypipypipypipypipypi-0.2/README.md
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-10 14:09:57.326734 pypipypipypipypipypipypipypi-0.2/pypipypipypipypipypipypipypi.egg-info/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      796 2023-07-10 14:09:57.000000 pypipypipypipypipypipypipypi-0.2/pypipypipypipypipypipypipypi.egg-info/PKG-INFO
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      346 2023-07-10 14:09:57.000000 pypipypipypipypipypipypipypi-0.2/pypipypipypipypipypipypipypi.egg-info/SOURCES.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        1 2023-07-10 14:09:57.000000 pypipypipypipypipypipypipypi-0.2/pypipypipypipypipypipypipypi.egg-info/dependency_links.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)        6 2023-07-10 14:09:57.000000 pypipypipypipypipypipypipypi-0.2/pypipypipypipypipypipypipypi.egg-info/requires.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       12 2023-07-10 14:09:57.000000 pypipypipypipypipypipypipypi-0.2/pypipypipypipypipypipypipypi.egg-info/top_level.txt
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       79 2023-07-10 14:09:57.329685 pypipypipypipypipypipypipypi-0.2/setup.cfg
+-rw-r--r--   0 vedantrathi   (501) staff       (20)     1668 2023-07-10 14:09:03.000000 pypipypipypipypipypipypipypi-0.2/setup.py
+drwxr-xr-x   0 vedantrathi   (501) staff       (20)        0 2023-07-10 14:09:57.328113 pypipypipypipypipypipypipypi-0.2/testpackage/
+-rw-r--r--   0 vedantrathi   (501) staff       (20)       22 2023-07-10 13:55:13.000000 pypipypipypipypipypipypipypi-0.2/testpackage/__init__.py
+-rw-r--r--   0 vedantrathi   (501) staff       (20)      304 2023-07-10 12:44:59.000000 pypipypipypipypipypipypipypi-0.2/testpackage/example.py
```

### Comparing `pypipypipypipypipypipypipypi-0.1/LICENSE.txt` & `pypipypipypipypipypipypipypi-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypipypipypipypipypipypipypi-0.1/PKG-INFO` & `pypipypipypipypipypipypipypi-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypipypipypipypipypipypipypi
-Version: 0.1
+Version: 0.2
 Summary: sample package
 Home-page: https://github.com/vrathi101/pypipypipypipypipypipypipypi.git
-Download-URL: https://github.com/vrathi101/pypipypipypipypipypipypipypi/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/vrathi101/pypipypipypipypipypipypipypi/archive/refs/tags/v_02.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pypipypipypipypipypipypipypi-0.1/pypipypipypipypipypipypipypi.egg-info/PKG-INFO` & `pypipypipypipypipypipypipypi-0.2/pypipypipypipypipypipypipypi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pypipypipypipypipypipypipypi
-Version: 0.1
+Version: 0.2
 Summary: sample package
 Home-page: https://github.com/vrathi101/pypipypipypipypipypipypipypi.git
-Download-URL: https://github.com/vrathi101/pypipypipypipypipypipypipypi/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/vrathi101/pypipypipypipypipypipypipypi/archive/refs/tags/v_02.tar.gz
 Author: VEDANT RATHI
 Author-email: vedrathi10@gmail.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pypipypipypipypipypipypipypi-0.1/setup.py` & `pypipypipypipypipypipypipypi-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 setuptools.setup(
   name = 'pypipypipypipypipypipypipypi',         # How you named your package 
   packages = ['testpackage'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'sample package',   # Give a short description about your library
   author = 'VEDANT RATHI',                   # Type in your name
   author_email = 'vedrathi10@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/vrathi101/pypipypipypipypipypipypipypi.git',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/vrathi101/pypipypipypipypipypipypipypi/archive/refs/tags/v_01.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/vrathi101/pypipypipypipypipypipypipypi/archive/refs/tags/v_02.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

