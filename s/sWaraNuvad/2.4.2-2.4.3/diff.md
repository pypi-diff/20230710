# Comparing `tmp/sWaraNuvad-2.4.2.tar.gz` & `tmp/sWaraNuvad-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sWaraNuvad-2.4.2.tar", last modified: Mon Jul 10 05:16:06 2023, max compression
+gzip compressed data, was "sWaraNuvad-2.4.3.tar", last modified: Mon Jul 10 05:18:21 2023, max compression
```

## Comparing `sWaraNuvad-2.4.2.tar` & `sWaraNuvad-2.4.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:16:06.667730 sWaraNuvad-2.4.2/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:16:06.667730 sWaraNuvad-2.4.2/PKG-INFO
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:16:06.659730 sWaraNuvad-2.4.2/sWaraNuvad/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 sWaraNuvad-2.4.2/sWaraNuvad/__init__.py
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:16:06.663730 sWaraNuvad-2.4.2/sWaraNuvad.egg-info/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:16:06.000000 sWaraNuvad-2.4.2/sWaraNuvad.egg-info/PKG-INFO
--rw-rw-r--   0 tejas     (1000) tejas     (1000)      200 2023-07-10 05:16:06.000000 sWaraNuvad-2.4.2/sWaraNuvad.egg-info/SOURCES.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 05:16:06.000000 sWaraNuvad-2.4.2/sWaraNuvad.egg-info/dependency_links.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 05:16:06.000000 sWaraNuvad-2.4.2/sWaraNuvad.egg-info/requires.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 05:16:06.000000 sWaraNuvad-2.4.2/sWaraNuvad.egg-info/top_level.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 05:16:06.667730 sWaraNuvad-2.4.2/setup.cfg
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1351 2023-07-10 05:15:59.000000 sWaraNuvad-2.4.2/setup.py
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:18:21.064590 sWaraNuvad-2.4.3/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:18:21.060590 sWaraNuvad-2.4.3/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)      974 2023-07-10 05:14:18.000000 sWaraNuvad-2.4.3/README.txt
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:18:21.060590 sWaraNuvad-2.4.3/sWaraNuvad/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 sWaraNuvad-2.4.3/sWaraNuvad/__init__.py
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:18:21.060590 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)      211 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/SOURCES.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/dependency_links.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/requires.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/top_level.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 05:18:21.064590 sWaraNuvad-2.4.3/setup.cfg
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1351 2023-07-10 05:18:10.000000 sWaraNuvad-2.4.3/setup.py
```

### Comparing `sWaraNuvad-2.4.2/PKG-INFO` & `sWaraNuvad-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sWaraNuvad
-Version: 2.4.2
+Version: 2.4.3
 Summary: Speech translation assistant
 Author: Tejas Sonavane
 Keywords: voice translate,voice to text translate,multiple language voice translate,translate,text to voice translate
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `sWaraNuvad-2.4.2/sWaraNuvad/__init__.py` & `sWaraNuvad-2.4.3/sWaraNuvad/__init__.py`

 * *Files identical despite different names*

### Comparing `sWaraNuvad-2.4.2/sWaraNuvad.egg-info/PKG-INFO` & `sWaraNuvad-2.4.3/sWaraNuvad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sWaraNuvad
-Version: 2.4.2
+Version: 2.4.3
 Summary: Speech translation assistant
 Author: Tejas Sonavane
 Keywords: voice translate,voice to text translate,multiple language voice translate,translate,text to voice translate
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `sWaraNuvad-2.4.2/setup.py` & `sWaraNuvad-2.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sWaraNuvad',
-    version='2.4.2',
+    version='2.4.3',
     description='Speech translation assistant',
     author='Tejas Sonavane',
     long_description='''The code uses speech recognition to capture user input through a microphone. It then recognizes the speech using Google's Speech-to-Text API. 
     The user is prompted to specify a language, and their subsequent speech is translated into multiple languages. The translations are displayed in the console.
     The speech translation assistant allows users to communicate in different languages by converting their spoken input into written text and providing translations in various supported languages.''',
     packages=['sWaraNuvad'],
     long_description_content_type="text/markdown",
```

