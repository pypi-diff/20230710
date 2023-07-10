# Comparing `tmp/sWaraNuvad-2.4.3.tar.gz` & `tmp/sWaraNuvad-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sWaraNuvad-2.4.3.tar", last modified: Mon Jul 10 05:18:21 2023, max compression
+gzip compressed data, was "sWaraNuvad-2.4.5.tar", last modified: Mon Jul 10 05:22:31 2023, max compression
```

## Comparing `sWaraNuvad-2.4.3.tar` & `sWaraNuvad-2.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:18:21.064590 sWaraNuvad-2.4.3/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:18:21.060590 sWaraNuvad-2.4.3/PKG-INFO
--rw-rw-r--   0 tejas     (1000) tejas     (1000)      974 2023-07-10 05:14:18.000000 sWaraNuvad-2.4.3/README.txt
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:18:21.060590 sWaraNuvad-2.4.3/sWaraNuvad/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 sWaraNuvad-2.4.3/sWaraNuvad/__init__.py
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:18:21.060590 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/PKG-INFO
--rw-rw-r--   0 tejas     (1000) tejas     (1000)      211 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/SOURCES.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/dependency_links.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/requires.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 05:18:21.000000 sWaraNuvad-2.4.3/sWaraNuvad.egg-info/top_level.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 05:18:21.064590 sWaraNuvad-2.4.3/setup.cfg
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1351 2023-07-10 05:18:10.000000 sWaraNuvad-2.4.3/setup.py
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:22:31.904878 sWaraNuvad-2.4.5/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:22:31.904878 sWaraNuvad-2.4.5/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)      974 2023-07-10 05:14:18.000000 sWaraNuvad-2.4.5/README.md
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:22:31.900877 sWaraNuvad-2.4.5/sWaraNuvad/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 sWaraNuvad-2.4.5/sWaraNuvad/__init__.py
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 05:22:31.904878 sWaraNuvad-2.4.5/sWaraNuvad.egg-info/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 05:22:31.000000 sWaraNuvad-2.4.5/sWaraNuvad.egg-info/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)      210 2023-07-10 05:22:31.000000 sWaraNuvad-2.4.5/sWaraNuvad.egg-info/SOURCES.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 05:22:31.000000 sWaraNuvad-2.4.5/sWaraNuvad.egg-info/dependency_links.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 05:22:31.000000 sWaraNuvad-2.4.5/sWaraNuvad.egg-info/requires.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 05:22:31.000000 sWaraNuvad-2.4.5/sWaraNuvad.egg-info/top_level.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 05:22:31.904878 sWaraNuvad-2.4.5/setup.cfg
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1351 2023-07-10 05:22:22.000000 sWaraNuvad-2.4.5/setup.py
```

### Comparing `sWaraNuvad-2.4.3/PKG-INFO` & `sWaraNuvad-2.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sWaraNuvad
-Version: 2.4.3
+Version: 2.4.5
 Summary: Speech translation assistant
 Author: Tejas Sonavane
 Keywords: voice translate,voice to text translate,multiple language voice translate,translate,text to voice translate
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `sWaraNuvad-2.4.3/README.txt` & `sWaraNuvad-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sWaraNuvad-2.4.3/sWaraNuvad/__init__.py` & `sWaraNuvad-2.4.5/sWaraNuvad/__init__.py`

 * *Files identical despite different names*

### Comparing `sWaraNuvad-2.4.3/sWaraNuvad.egg-info/PKG-INFO` & `sWaraNuvad-2.4.5/sWaraNuvad.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sWaraNuvad
-Version: 2.4.3
+Version: 2.4.5
 Summary: Speech translation assistant
 Author: Tejas Sonavane
 Keywords: voice translate,voice to text translate,multiple language voice translate,translate,text to voice translate
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `sWaraNuvad-2.4.3/setup.py` & `sWaraNuvad-2.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sWaraNuvad',
-    version='2.4.3',
+    version='2.4.5',
     description='Speech translation assistant',
     author='Tejas Sonavane',
     long_description='''The code uses speech recognition to capture user input through a microphone. It then recognizes the speech using Google's Speech-to-Text API. 
     The user is prompted to specify a language, and their subsequent speech is translated into multiple languages. The translations are displayed in the console.
     The speech translation assistant allows users to communicate in different languages by converting their spoken input into written text and providing translations in various supported languages.''',
     packages=['sWaraNuvad'],
     long_description_content_type="text/markdown",
```

