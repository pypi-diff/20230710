# Comparing `tmp/SwarAnuvad-2.4.2.tar.gz` & `tmp/SwarAnuvad-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SwarAnuvad-2.4.2.tar", last modified: Mon Jul 10 06:29:40 2023, max compression
+gzip compressed data, was "SwarAnuvad-2.4.4.tar", last modified: Mon Jul 10 06:32:03 2023, max compression
```

## Comparing `SwarAnuvad-2.4.2.tar` & `SwarAnuvad-2.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:29:40.401200 SwarAnuvad-2.4.2/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 06:29:40.401200 SwarAnuvad-2.4.2/PKG-INFO
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1013 2023-07-10 06:27:32.000000 SwarAnuvad-2.4.2/README.md
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:29:40.401200 SwarAnuvad-2.4.2/SwarAnuvad.egg-info/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 06:29:40.000000 SwarAnuvad-2.4.2/SwarAnuvad.egg-info/PKG-INFO
--rw-rw-r--   0 tejas     (1000) tejas     (1000)      210 2023-07-10 06:29:40.000000 SwarAnuvad-2.4.2/SwarAnuvad.egg-info/SOURCES.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 06:29:40.000000 SwarAnuvad-2.4.2/SwarAnuvad.egg-info/dependency_links.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 06:29:40.000000 SwarAnuvad-2.4.2/SwarAnuvad.egg-info/requires.txt
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 06:29:40.000000 SwarAnuvad-2.4.2/SwarAnuvad.egg-info/top_level.txt
-drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:29:40.401200 SwarAnuvad-2.4.2/sWaraNuvad/
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 SwarAnuvad-2.4.2/sWaraNuvad/__init__.py
--rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 06:29:40.401200 SwarAnuvad-2.4.2/setup.cfg
--rw-rw-r--   0 tejas     (1000) tejas     (1000)     1351 2023-07-10 06:29:24.000000 SwarAnuvad-2.4.2/setup.py
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:32:03.958645 SwarAnuvad-2.4.4/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 06:32:03.958645 SwarAnuvad-2.4.4/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1013 2023-07-10 06:27:32.000000 SwarAnuvad-2.4.4/README.md
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:32:03.954645 SwarAnuvad-2.4.4/SwarAnuvad.egg-info/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1059 2023-07-10 06:32:03.000000 SwarAnuvad-2.4.4/SwarAnuvad.egg-info/PKG-INFO
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)      210 2023-07-10 06:32:03.000000 SwarAnuvad-2.4.4/SwarAnuvad.egg-info/SOURCES.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)        1 2023-07-10 06:32:03.000000 SwarAnuvad-2.4.4/SwarAnuvad.egg-info/dependency_links.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       56 2023-07-10 06:32:03.000000 SwarAnuvad-2.4.4/SwarAnuvad.egg-info/requires.txt
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       11 2023-07-10 06:32:03.000000 SwarAnuvad-2.4.4/SwarAnuvad.egg-info/top_level.txt
+drwxrwxr-x   0 tejas     (1000) tejas     (1000)        0 2023-07-10 06:32:03.954645 SwarAnuvad-2.4.4/sWaraNuvad/
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     5038 2023-07-07 11:19:34.000000 SwarAnuvad-2.4.4/sWaraNuvad/__init__.py
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)       38 2023-07-10 06:32:03.958645 SwarAnuvad-2.4.4/setup.cfg
+-rw-rw-r--   0 tejas     (1000) tejas     (1000)     1351 2023-07-10 06:31:52.000000 SwarAnuvad-2.4.4/setup.py
```

### Comparing `SwarAnuvad-2.4.2/PKG-INFO` & `SwarAnuvad-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwarAnuvad
-Version: 2.4.2
+Version: 2.4.4
 Summary: Speech translation assistant
 Author: Tejas Sonavane
 Keywords: voice translate,voice to text translate,multiple language voice translate,translate,text to voice translate
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `SwarAnuvad-2.4.2/README.md` & `SwarAnuvad-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `SwarAnuvad-2.4.2/SwarAnuvad.egg-info/PKG-INFO` & `SwarAnuvad-2.4.4/SwarAnuvad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwarAnuvad
-Version: 2.4.2
+Version: 2.4.4
 Summary: Speech translation assistant
 Author: Tejas Sonavane
 Keywords: voice translate,voice to text translate,multiple language voice translate,translate,text to voice translate
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `SwarAnuvad-2.4.2/sWaraNuvad/__init__.py` & `SwarAnuvad-2.4.4/sWaraNuvad/__init__.py`

 * *Files identical despite different names*

### Comparing `SwarAnuvad-2.4.2/setup.py` & `SwarAnuvad-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='SwarAnuvad',
-    version='2.4.2',
+    version='2.4.4',
     description='Speech translation assistant',
     author='Tejas Sonavane',
     long_description='''The code uses speech recognition to capture user input through a microphone. It then recognizes the speech using Google's Speech-to-Text API. 
     The user is prompted to specify a language, and their subsequent speech is translated into multiple languages. The translations are displayed in the console.
     The speech translation assistant allows users to communicate in different languages by converting their spoken input into written text and providing translations in various supported languages.''',
     packages=['sWaraNuvad'],
     long_description_content_type="text/markdown",
```

