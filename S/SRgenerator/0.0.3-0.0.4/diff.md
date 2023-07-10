# Comparing `tmp/SRgenerator-0.0.3.tar.gz` & `tmp/SRgenerator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRgenerator-0.0.3.tar", last modified: Mon Jul 10 08:07:17 2023, max compression
+gzip compressed data, was "SRgenerator-0.0.4.tar", last modified: Mon Jul 10 08:15:38 2023, max compression
```

## Comparing `SRgenerator-0.0.3.tar` & `SRgenerator-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:07:17.827432 SRgenerator-0.0.3/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)     1536 2023-07-10 07:05:30.000000 SRgenerator-0.0.3/LICENSE.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       55 2023-07-10 07:07:12.000000 SRgenerator-0.0.3/MANIFEST.in
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:07:17.827432 SRgenerator-0.0.3/PKG-INFO
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      186 2023-07-10 07:42:58.000000 SRgenerator-0.0.3/README.txt
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:07:17.827432 SRgenerator-0.0.3/SRgenerator/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)    10426 2023-07-10 06:41:03.000000 SRgenerator-0.0.3/SRgenerator/SR_generator.py
--rw-rw-r--   0 molalin   (1004) molalin   (1004)        0 2023-07-10 07:33:33.000000 SRgenerator-0.0.3/SRgenerator/__init__.py
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:07:17.827432 SRgenerator-0.0.3/SRgenerator.egg-info/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:07:17.000000 SRgenerator-0.0.3/SRgenerator.egg-info/PKG-INFO
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      269 2023-07-10 08:07:17.000000 SRgenerator-0.0.3/SRgenerator.egg-info/SOURCES.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)        1 2023-07-10 08:07:17.000000 SRgenerator-0.0.3/SRgenerator.egg-info/dependency_links.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       31 2023-07-10 08:07:17.000000 SRgenerator-0.0.3/SRgenerator.egg-info/requires.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       12 2023-07-10 08:07:17.000000 SRgenerator-0.0.3/SRgenerator.egg-info/top_level.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       38 2023-07-10 08:07:17.827432 SRgenerator-0.0.3/setup.cfg
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      989 2023-07-10 08:06:59.000000 SRgenerator-0.0.3/setup.py
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:15:38.985227 SRgenerator-0.0.4/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)     1536 2023-07-10 07:05:30.000000 SRgenerator-0.0.4/LICENSE.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       55 2023-07-10 07:07:12.000000 SRgenerator-0.0.4/MANIFEST.in
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:15:38.985227 SRgenerator-0.0.4/PKG-INFO
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      186 2023-07-10 07:42:58.000000 SRgenerator-0.0.4/README.txt
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:15:38.985227 SRgenerator-0.0.4/SRgenerator.egg-info/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:15:38.000000 SRgenerator-0.0.4/SRgenerator.egg-info/PKG-INFO
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      217 2023-07-10 08:15:38.000000 SRgenerator-0.0.4/SRgenerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)        1 2023-07-10 08:15:38.000000 SRgenerator-0.0.4/SRgenerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       31 2023-07-10 08:15:38.000000 SRgenerator-0.0.4/SRgenerator.egg-info/requires.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)        1 2023-07-10 08:15:38.000000 SRgenerator-0.0.4/SRgenerator.egg-info/top_level.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       38 2023-07-10 08:15:38.985227 SRgenerator-0.0.4/setup.cfg
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      989 2023-07-10 08:14:51.000000 SRgenerator-0.0.4/setup.py
```

### Comparing `SRgenerator-0.0.3/LICENSE.txt` & `SRgenerator-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SRgenerator-0.0.3/PKG-INFO` & `SRgenerator-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRgenerator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Stereo operation for chemicals based on RDkit package
 Author: Mola Lin
 Author-email: acps91012@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `SRgenerator-0.0.3/SRgenerator.egg-info/PKG-INFO` & `SRgenerator-0.0.4/SRgenerator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRgenerator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Stereo operation for chemicals based on RDkit package
 Author: Mola Lin
 Author-email: acps91012@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `SRgenerator-0.0.3/setup.py` & `SRgenerator-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open("README.txt", "r") as fh:
     long_description = fh.read()
 
 setup(
     name                = 'SRgenerator',
-    version             = '0.0.3',
+    version             = '0.0.4',
     description         = "Stereo operation for chemicals based on RDkit package",
     long_description    = long_description,
     author              = 'Mola Lin',
     author_email        = 'acps91012@gmail.com',
     license             = 'BSD',
     packages            = find_packages(),
     install_requires    = ['selfies >= 2.0.0', 'rdkit >= 2023.3.1'],
```

