# Comparing `tmp/NoomSmartKeyboard-0.0.2.tar.gz` & `tmp/NoomSmartKeyboard-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NoomSmartKeyboard-0.0.2.tar", last modified: Mon Jul 10 08:04:28 2023, max compression
+gzip compressed data, was "NoomSmartKeyboard-0.1.0.tar", last modified: Mon Jul 10 08:42:50 2023, max compression
```

## Comparing `NoomSmartKeyboard-0.0.2.tar` & `NoomSmartKeyboard-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 08:04:28.080777 NoomSmartKeyboard-0.0.2/
--rw-rw-rw-   0        0        0     1089 2023-07-10 07:32:34.000000 NoomSmartKeyboard-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-10 08:04:28.075774 NoomSmartKeyboard-0.0.2/NoomSmartKeyboard.egg-info/
--rw-rw-rw-   0        0        0      490 2023-07-10 08:04:27.000000 NoomSmartKeyboard-0.0.2/NoomSmartKeyboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-10 08:04:27.000000 NoomSmartKeyboard-0.0.2/NoomSmartKeyboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:04:27.000000 NoomSmartKeyboard-0.0.2/NoomSmartKeyboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-10 08:04:27.000000 NoomSmartKeyboard-0.0.2/NoomSmartKeyboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:04:27.000000 NoomSmartKeyboard-0.0.2/NoomSmartKeyboard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2023-07-10 08:04:28.079777 NoomSmartKeyboard-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-07-10 07:32:34.000000 NoomSmartKeyboard-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 08:04:28.080777 NoomSmartKeyboard-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-07-10 08:04:21.000000 NoomSmartKeyboard-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:04:28.077777 NoomSmartKeyboard-0.0.2/test/
--rw-rw-rw-   0        0        0      196 2023-07-10 07:59:36.000000 NoomSmartKeyboard-0.0.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-10 08:42:50.041758 NoomSmartKeyboard-0.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-07-10 07:32:34.000000 NoomSmartKeyboard-0.1.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-10 08:42:50.038759 NoomSmartKeyboard-0.1.0/NoomSmartKeyboard.egg-info/
+-rw-rw-rw-   0        0        0     1336 2023-07-10 08:42:49.000000 NoomSmartKeyboard-0.1.0/NoomSmartKeyboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-10 08:42:49.000000 NoomSmartKeyboard-0.1.0/NoomSmartKeyboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:42:49.000000 NoomSmartKeyboard-0.1.0/NoomSmartKeyboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 08:42:49.000000 NoomSmartKeyboard-0.1.0/NoomSmartKeyboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 08:42:49.000000 NoomSmartKeyboard-0.1.0/NoomSmartKeyboard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1336 2023-07-10 08:42:50.040758 NoomSmartKeyboard-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2023-07-10 08:42:30.000000 NoomSmartKeyboard-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 08:42:50.042757 NoomSmartKeyboard-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      824 2023-07-10 08:33:33.000000 NoomSmartKeyboard-0.1.0/setup.py
```

### Comparing `NoomSmartKeyboard-0.0.2/LICENSE` & `NoomSmartKeyboard-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NoomSmartKeyboard-0.0.2/setup.py` & `NoomSmartKeyboard-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
-
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
 setup(
     name="NoomSmartKeyboard",
-    version="0.0.2",
+    version="0.1.0",
     url="https://github.com/poommin2543/Noom-Smart-Keyboard",
     author="Noom Poommin",
     author_email="poommin2543@gmail.com",
     description="Description of my package",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     packages=find_packages(),    
     install_requires=[
         'pywin32',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha', 
         'Intended Audience :: Developers',
```

