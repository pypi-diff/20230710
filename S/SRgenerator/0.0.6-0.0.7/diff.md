# Comparing `tmp/SRgenerator-0.0.6.tar.gz` & `tmp/SRgenerator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRgenerator-0.0.6.tar", last modified: Mon Jul 10 08:29:29 2023, max compression
+gzip compressed data, was "SRgenerator-0.0.7.tar", last modified: Mon Jul 10 08:55:15 2023, max compression
```

## Comparing `SRgenerator-0.0.6.tar` & `SRgenerator-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)     1536 2023-07-10 07:05:30.000000 SRgenerator-0.0.6/LICENSE.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       55 2023-07-10 07:07:12.000000 SRgenerator-0.0.6/MANIFEST.in
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/PKG-INFO
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      186 2023-07-10 07:42:58.000000 SRgenerator-0.0.6/README.txt
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/SRgenerator/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)    10427 2023-07-10 08:29:04.000000 SRgenerator-0.0.6/SRgenerator/SR_generator.py
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       65 2023-07-10 08:28:55.000000 SRgenerator-0.0.6/SRgenerator/__init__.py
-drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/SRgenerator.egg-info/
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/PKG-INFO
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      269 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/SOURCES.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)        1 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/dependency_links.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       31 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/requires.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       12 2023-07-10 08:29:29.000000 SRgenerator-0.0.6/SRgenerator.egg-info/top_level.txt
--rw-rw-r--   0 molalin   (1004) molalin   (1004)       38 2023-07-10 08:29:29.721622 SRgenerator-0.0.6/setup.cfg
--rw-rw-r--   0 molalin   (1004) molalin   (1004)      989 2023-07-10 08:29:15.000000 SRgenerator-0.0.6/setup.py
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:55:15.530956 SRgenerator-0.0.7/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)     1536 2023-07-10 07:05:30.000000 SRgenerator-0.0.7/LICENSE.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       52 2023-07-10 08:53:12.000000 SRgenerator-0.0.7/MANIFEST.in
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:55:15.530956 SRgenerator-0.0.7/PKG-INFO
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      186 2023-07-10 07:42:58.000000 SRgenerator-0.0.7/README.txt
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:55:15.530956 SRgenerator-0.0.7/SRgenerator/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)    10447 2023-07-10 08:48:20.000000 SRgenerator-0.0.7/SRgenerator/SR_generator.py
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       65 2023-07-10 08:28:55.000000 SRgenerator-0.0.7/SRgenerator/__init__.py
+drwxrwxr-x   0 molalin   (1004) molalin   (1004)        0 2023-07-10 08:55:15.530956 SRgenerator-0.0.7/SRgenerator.egg-info/
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      826 2023-07-10 08:55:14.000000 SRgenerator-0.0.7/SRgenerator.egg-info/PKG-INFO
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)      269 2023-07-10 08:55:15.000000 SRgenerator-0.0.7/SRgenerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)        1 2023-07-10 08:55:15.000000 SRgenerator-0.0.7/SRgenerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       31 2023-07-10 08:55:15.000000 SRgenerator-0.0.7/SRgenerator.egg-info/requires.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       12 2023-07-10 08:55:15.000000 SRgenerator-0.0.7/SRgenerator.egg-info/top_level.txt
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)       38 2023-07-10 08:55:15.530956 SRgenerator-0.0.7/setup.cfg
+-rw-rw-r--   0 molalin   (1004) molalin   (1004)     1087 2023-07-10 08:54:57.000000 SRgenerator-0.0.7/setup.py
```

### Comparing `SRgenerator-0.0.6/LICENSE.txt` & `SRgenerator-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SRgenerator-0.0.6/PKG-INFO` & `SRgenerator-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRgenerator
-Version: 0.0.6
+Version: 0.0.7
 Summary: Stereo operation for chemicals based on RDkit package
 Author: Mola Lin
 Author-email: acps91012@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `SRgenerator-0.0.6/SRgenerator/SR_generator.py` & `SRgenerator-0.0.7/SRgenerator/SR_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import itertools, copy, re
 import rdkit
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from typing import Optional
 import selfies as se
+import pandas as pd
 
 class SR_generator() :
     def __init__(
         self,
                 ) :
         self.SR = {0:Chem.ChiralType.CHI_TETRAHEDRAL_CW, 1:Chem.ChiralType.CHI_TETRAHEDRAL_CCW}
         self.CT = { -1:Chem.BondStereo.STEREOANY, 0:Chem.BondStereo.STEREOCIS, 1:Chem.BondStereo.STEREOTRANS }
```

### Comparing `SRgenerator-0.0.6/SRgenerator.egg-info/PKG-INFO` & `SRgenerator-0.0.7/SRgenerator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SRgenerator
-Version: 0.0.6
+Version: 0.0.7
 Summary: Stereo operation for chemicals based on RDkit package
 Author: Mola Lin
 Author-email: acps91012@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `SRgenerator-0.0.6/setup.py` & `SRgenerator-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,22 @@
 ]
 
 with open("README.txt", "r") as fh:
     long_description = fh.read()
 
 setup(
     name                = 'SRgenerator',
-    version             = '0.0.6',
+    version             = '0.0.7',
     description         = "Stereo operation for chemicals based on RDkit package",
     long_description    = long_description,
     author              = 'Mola Lin',
     author_email        = 'acps91012@gmail.com',
     license             = 'BSD',
     packages            = find_packages(),
     install_requires    = ['selfies >= 2.0.0', 'rdkit >= 2023.3.1'],
     classifiers         = classifiers,
+    package_data={
+        '':['*.csv'],
+        'bandwidth_reporter':['*.csv']
+               },
     python_requires='>=3.6',
 )
```

