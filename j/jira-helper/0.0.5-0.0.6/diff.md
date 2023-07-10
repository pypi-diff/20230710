# Comparing `tmp/jira_helper-0.0.5-py3-none-any.whl.zip` & `tmp/jira_helper-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7187 bytes, number of entries: 10
--rw-rw-r--  2.0 unx    13182 b- defN 22-Aug-09 05:02 jira_helper/__init__.py
+Zip file size: 7200 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx    13205 b- defN 22-Aug-18 15:43 jira_helper/__init__.py
 -rw-rw-r--  2.0 unx      825 b- defN 20-Aug-08 20:59 jira_helper/settings.ini
 -rw-rw-r--  2.0 unx        0 b- defN 20-Aug-08 20:59 jira_helper/scripts/__init__.py
 -rw-rw-r--  2.0 unx      196 b- defN 20-Aug-08 20:59 jira_helper/scripts/repl.py
--rw-rw-r--  2.0 unx      608 b- defN 22-Aug-09 05:02 jira_helper-0.0.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      990 b- defN 22-Aug-09 05:02 jira_helper-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Aug-09 05:02 jira_helper-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       61 b- defN 22-Aug-09 05:02 jira_helper-0.0.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 22-Aug-09 05:02 jira_helper-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      836 b- defN 22-Aug-09 05:02 jira_helper-0.0.5.dist-info/RECORD
-10 files, 16802 bytes uncompressed, 5741 bytes compressed:  65.8%
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jul-10 04:44 jira_helper-0.0.6.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jul-10 04:44 jira_helper-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 04:44 jira_helper-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       61 b- defN 23-Jul-10 04:44 jira_helper-0.0.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jul-10 04:44 jira_helper-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      836 b- defN 23-Jul-10 04:44 jira_helper-0.0.6.dist-info/RECORD
+10 files, 16825 bytes uncompressed, 5754 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: jira_helper/scripts/__init__.py
 Comment: 
 
 Filename: jira_helper/scripts/repl.py
 Comment: 
 
-Filename: jira_helper-0.0.5.dist-info/LICENSE.txt
+Filename: jira_helper-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: jira_helper-0.0.5.dist-info/METADATA
+Filename: jira_helper-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: jira_helper-0.0.5.dist-info/WHEEL
+Filename: jira_helper-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: jira_helper-0.0.5.dist-info/entry_points.txt
+Filename: jira_helper-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: jira_helper-0.0.5.dist-info/top_level.txt
+Filename: jira_helper-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: jira_helper-0.0.5.dist-info/RECORD
+Filename: jira_helper-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jira_helper/__init__.py

```diff
@@ -13,15 +13,15 @@
 from io import StringIO
 from functools import partial
 from collections import OrderedDict
 from chloop import GetCharLoop
 from pprint import pprint
 try:
     from ujson import loads
-except ImportError:
+except (ImportError, ModuleNotFoundError):
     from json import loads
 
 
 get_setting = sh.settings_getter(__name__)
 JIRA_URL = get_setting('JIRA_URL')
 JIRA_API_TOKEN = get_setting('JIRA_API_TOKEN')
 JIRA_API_USER = get_setting('JIRA_API_USER')
```

## Comparing `jira_helper-0.0.5.dist-info/LICENSE.txt` & `jira_helper-0.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `jira_helper-0.0.5.dist-info/METADATA` & `jira_helper-0.0.6.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: jira-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLI tools and REPL for passing JQL to a JIRA server and filtering results
 Home-page: https://github.com/kenjyco/jira-helper
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/jira-helper/tarball/v0.0.5
+Download-URL: https://github.com/kenjyco/jira-helper/tarball/v0.0.6
 Keywords: jira,jql,repl,cli,command-line,helper,kenjyco
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `jira_helper-0.0.5.dist-info/RECORD` & `jira_helper-0.0.6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-jira_helper/__init__.py,sha256=WI7BgKoW0GO4vIL-EMYIU57OxPhFY0sRFiepGgoA9nk,13182
+jira_helper/__init__.py,sha256=HeislPaNM8YEj-3lHQVPsD-WZeoR7wBPzXtznB2aI5E,13205
 jira_helper/settings.ini,sha256=Vb0i7WY1B09HHN3xhVPQaOqKyLP2brOLhx3dZvwe4h0,825
 jira_helper/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jira_helper/scripts/repl.py,sha256=QpyPNktQq-OKxtx1_3EQRwAO9np_1FMbPPjYburK2wY,196
-jira_helper-0.0.5.dist-info/LICENSE.txt,sha256=TEfWL0DMfS6p49n4AeLR5CfiihVzu4DFBXxlJKX6e10,608
-jira_helper-0.0.5.dist-info/METADATA,sha256=NnrmfyoOJEZIibHrpH73MnuVya0fAwgBoXSZEzy4qZE,990
-jira_helper-0.0.5.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-jira_helper-0.0.5.dist-info/entry_points.txt,sha256=pzKVOvN7ucU3z1xd9YZez8uUXF9KwAyAwPm__XddlGQ,61
-jira_helper-0.0.5.dist-info/top_level.txt,sha256=6fruvb6JYoPn6PbmQWuHQAKAMPYrTxRPfIlu2Xvj26U,12
-jira_helper-0.0.5.dist-info/RECORD,,
+jira_helper-0.0.6.dist-info/LICENSE.txt,sha256=TEfWL0DMfS6p49n4AeLR5CfiihVzu4DFBXxlJKX6e10,608
+jira_helper-0.0.6.dist-info/METADATA,sha256=fLuTiGoLDFS2MmUbCvAVWH9z0y6nzfYalNXF2wME8FE,990
+jira_helper-0.0.6.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+jira_helper-0.0.6.dist-info/entry_points.txt,sha256=pzKVOvN7ucU3z1xd9YZez8uUXF9KwAyAwPm__XddlGQ,61
+jira_helper-0.0.6.dist-info/top_level.txt,sha256=6fruvb6JYoPn6PbmQWuHQAKAMPYrTxRPfIlu2Xvj26U,12
+jira_helper-0.0.6.dist-info/RECORD,,
```

