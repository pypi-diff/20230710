# Comparing `tmp/SRgenerator-0.0.5.tar.gz` & `tmp/SRgenerator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRgenerator-0.0.5.tar", last modified: Mon Jul 10 08:20:41 2023, max compression
+gzip compressed data, was "SRgenerator-0.0.6.tar", last modified: Mon Jul 10 08:29:29 2023, max compression
```

## Comparing `SRgenerator-0.0.5.tar` & `SRgenerator-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:20:40.999916 SRgenerator-0.0.5/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)     1536 2023-07-10 07:05:30.000000 SRgenerator-0.0.5/LICENSE.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       55 2023-07-10 07:07:12.000000 SRgenerator-0.0.5/MANIFEST.in
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:20:40.999916 SRgenerator-0.0.5/PKG-INFO
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      186 2023-07-10 07:42:58.000000 SRgenerator-0.0.5/README.txt
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:20:40.999916 SRgenerator-0.0.5/SR_generator/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)    10426 2023-07-10 06:41:03.000000 SRgenerator-0.0.5/SR_generator/SR_generator.py
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       38 2023-07-10 08:19:51.000000 SRgenerator-0.0.5/SR_generator/__init__.py
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:20:40.999916 SRgenerator-0.0.5/SRgenerator.egg-info/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:20:40.000000 SRgenerator-0.0.5/SRgenerator.egg-info/PKG-INFO
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      271 2023-07-10 08:20:40.000000 SRgenerator-0.0.5/SRgenerator.egg-info/SOURCES.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)        1 2023-07-10 08:20:40.000000 SRgenerator-0.0.5/SRgenerator.egg-info/dependency_links.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       31 2023-07-10 08:20:40.000000 SRgenerator-0.0.5/SRgenerator.egg-info/requires.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       13 2023-07-10 08:20:40.000000 SRgenerator-0.0.5/SRgenerator.egg-info/top_level.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       38 2023-07-10 08:20:40.999916 SRgenerator-0.0.5/setup.cfg
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      989 2023-07-10 08:20:20.000000 SRgenerator-0.0.5/setup.py
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)     1536 2023-07-10 07:05:30.000000 SRgenerator-0.0.6/LICENSE.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       55 2023-07-10 07:07:12.000000 SRgenerator-0.0.6/MANIFEST.in
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/PKG-INFO
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      186 2023-07-10 07:42:58.000000 SRgenerator-0.0.6/README.txt
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/SRgenerator/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)    10427 2023-07-10 08:29:04.000000 SRgenerator-0.0.6/SRgenerator/SR_generator.py
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       65 2023-07-10 08:28:55.000000 SRgenerator-0.0.6/SRgenerator/__init__.py
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/SRgenerator.egg-info/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/PKG-INFO
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      269 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)        1 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       31 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/requires.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       12 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/top_level.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       38 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/setup.cfg
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      989 2023-07-10 08:29:15.000000 SRgenerator-0.0.6/setup.py
```

### Comparing `SRgenerator-0.0.5/LICENSE.txt` & `SRgenerator-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SRgenerator-0.0.5/PKG-INFO` & `SRgenerator-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRgenerator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stereo operation for chemicals based on RDkit package
 Author: Mola Lin
 Author-email: acps91012@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `SRgenerator-0.0.5/SR_generator/SR_generator.py` & `SRgenerator-0.0.6/SRgenerator/SR_generator.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -258,8 +258,8 @@
         mol = Chem.MolFromSmiles( smiles )
         mol = Chem.AddHs( mol )
         AllChem.EmbedMolecule( mol )
         mol = Chem.RemoveHs( mol )
         # display( mol )
         # print( Chem.MolToMolBlock( mol ) )
         return mol
-    
+
```

### Comparing `SRgenerator-0.0.5/SRgenerator.egg-info/PKG-INFO` & `SRgenerator-0.0.6/SRgenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRgenerator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stereo operation for chemicals based on RDkit package
 Author: Mola Lin
 Author-email: acps91012@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `SRgenerator-0.0.5/setup.py` & `SRgenerator-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open("README.txt", "r") as fh:
     long_description = fh.read()
 
 setup(
     name                = 'SRgenerator',
-    version             = '0.0.5',
+    version             = '0.0.6',
     description         = "Stereo operation for chemicals based on RDkit package",
     long_description    = long_description,
     author              = 'Mola Lin',
     author_email        = 'acps91012@gmail.com',
     license             = 'BSD',
     packages            = find_packages(),
     install_requires    = ['selfies >= 2.0.0', 'rdkit >= 2023.3.1'],
```

