# Comparing `tmp/NoomSmartKeyboard-0.1.1.tar.gz` & `tmp/NoomSmartKeyboard-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NoomSmartKeyboard-0.1.1.tar", last modified: Mon Jul 10 09:40:04 2023, max compression
+gzip compressed data, was "NoomSmartKeyboard-0.1.2.tar", last modified: Mon Jul 10 09:51:27 2023, max compression
```

## Comparing `NoomSmartKeyboard-0.1.1.tar` & `NoomSmartKeyboard-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:40:04.274494 NoomSmartKeyboard-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-07-10 07:32:34.000000 NoomSmartKeyboard-0.1.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-10 09:40:04.271494 NoomSmartKeyboard-0.1.1/NoomSmartKeyboard.egg-info/
--rw-rw-rw-   0        0        0     1336 2023-07-10 09:40:04.000000 NoomSmartKeyboard-0.1.1/NoomSmartKeyboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-10 09:40:04.000000 NoomSmartKeyboard-0.1.1/NoomSmartKeyboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:40:04.000000 NoomSmartKeyboard-0.1.1/NoomSmartKeyboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-10 09:40:04.000000 NoomSmartKeyboard-0.1.1/NoomSmartKeyboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:40:04.000000 NoomSmartKeyboard-0.1.1/NoomSmartKeyboard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1336 2023-07-10 09:40:04.273493 NoomSmartKeyboard-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      801 2023-07-10 08:42:30.000000 NoomSmartKeyboard-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 09:40:04.274494 NoomSmartKeyboard-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      824 2023-07-10 09:34:32.000000 NoomSmartKeyboard-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 09:51:27.289049 NoomSmartKeyboard-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-07-10 07:32:34.000000 NoomSmartKeyboard-0.1.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-10 09:51:27.287047 NoomSmartKeyboard-0.1.2/NoomSmartKeyboard.egg-info/
+-rw-rw-rw-   0        0        0     1336 2023-07-10 09:51:27.000000 NoomSmartKeyboard-0.1.2/NoomSmartKeyboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-10 09:51:27.000000 NoomSmartKeyboard-0.1.2/NoomSmartKeyboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:51:27.000000 NoomSmartKeyboard-0.1.2/NoomSmartKeyboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 09:51:27.000000 NoomSmartKeyboard-0.1.2/NoomSmartKeyboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 09:51:27.000000 NoomSmartKeyboard-0.1.2/NoomSmartKeyboard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1336 2023-07-10 09:51:27.288049 NoomSmartKeyboard-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2023-07-10 08:42:30.000000 NoomSmartKeyboard-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 09:51:27.290048 NoomSmartKeyboard-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      824 2023-07-10 09:51:07.000000 NoomSmartKeyboard-0.1.2/setup.py
```

### Comparing `NoomSmartKeyboard-0.1.1/LICENSE` & `NoomSmartKeyboard-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NoomSmartKeyboard-0.1.1/NoomSmartKeyboard.egg-info/PKG-INFO` & `NoomSmartKeyboard-0.1.2/NoomSmartKeyboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NoomSmartKeyboard
-Version: 0.1.1
+Version: 0.1.2
 Summary: Description of my package
 Home-page: https://github.com/poommin2543/Noom-Smart-Keyboard
 Author: Noom Poommin
 Author-email: poommin2543@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NoomSmartKeyboard-0.1.1/PKG-INFO` & `NoomSmartKeyboard-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NoomSmartKeyboard
-Version: 0.1.1
+Version: 0.1.2
 Summary: Description of my package
 Home-page: https://github.com/poommin2543/Noom-Smart-Keyboard
 Author: Noom Poommin
 Author-email: poommin2543@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `NoomSmartKeyboard-0.1.1/README.md` & `NoomSmartKeyboard-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `NoomSmartKeyboard-0.1.1/setup.py` & `NoomSmartKeyboard-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name="NoomSmartKeyboard",
-    version="0.1.1",
+    version="0.1.2",
     url="https://github.com/poommin2543/Noom-Smart-Keyboard",
     author="Noom Poommin",
     author_email="poommin2543@gmail.com",
     description="Description of my package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

