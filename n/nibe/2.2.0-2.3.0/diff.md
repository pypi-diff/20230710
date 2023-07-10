# Comparing `tmp/nibe-2.2.0.tar.gz` & `tmp/nibe-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibe-2.2.0.tar", last modified: Wed May  3 19:17:51 2023, max compression
+gzip compressed data, was "nibe-2.3.0.tar", last modified: Mon Jul 10 14:57:28 2023, max compression
```

## Comparing `nibe-2.2.0.tar` & `nibe-2.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.245375 nibe-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 19:17:41.000000 nibe-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42067 2023-05-03 19:17:51.245375 nibe-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-03 19:17:41.000000 nibe-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/coil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/coil_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/modbus.py
--rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/nibegw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/console_scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/console_scripts/convert_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.245375 nibe-2.2.0/nibe/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)   349736 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1145_f1245.json
--rw-r--r--   0 runner    (1001) docker     (123)   235740 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1155_f1255.json
--rw-r--r--   0 runner    (1001) docker     (123)   363580 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1345.json
--rw-r--r--   0 runner    (1001) docker     (123)   370969 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1355.json
--rw-r--r--   0 runner    (1001) docker     (123)   112227 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f370_f470.json
--rw-r--r--   0 runner    (1001) docker     (123)   132739 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f730.json
--rw-r--r--   0 runner    (1001) docker     (123)   147755 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f750.json
--rw-r--r--   0 runner    (1001) docker     (123)   233725 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s1155_s1255.json
--rw-r--r--   0 runner    (1001) docker     (123)   152307 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s2125.json
--rw-r--r--   0 runner    (1001) docker     (123)   151836 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s320_s325.json
--rw-r--r--   0 runner    (1001) docker     (123)   183682 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s735.json
--rw-r--r--   0 runner    (1001) docker     (123)    81905 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/smo20.json
--rw-r--r--   0 runner    (1001) docker     (123)   302299 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/smo40.json
--rw-r--r--   0 runner    (1001) docker     (123)   230143 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/smos40.json
--rw-r--r--   0 runner    (1001) docker     (123)   210957 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/vvm225_vvm320_vvm325.json
--rw-r--r--   0 runner    (1001) docker     (123)   206217 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/vvm310_vvm500.json
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/event_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/heatpump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42067 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-03 19:17:41.000000 nibe-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-03 19:17:51.249375 nibe-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.245375 nibe-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-05-03 19:17:41.000000 nibe-2.2.0/tests/test_coil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-03 19:17:41.000000 nibe-2.2.0/tests/test_heatpump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:28.659866 nibe-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 14:57:19.000000 nibe-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42067 2023-07-10 14:57:28.659866 nibe-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-10 14:57:19.000000 nibe-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:28.647865 nibe-2.3.0/nibe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/coil_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:28.647865 nibe-2.3.0/nibe/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/connection/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/connection/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/connection/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/connection/nibegw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:28.651865 nibe-2.3.0/nibe/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/console_scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/console_scripts/convert_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:28.655866 nibe-2.3.0/nibe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   349665 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/f1145_f1245.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235740 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/f1155_f1255.json
+-rw-r--r--   0 runner    (1001) docker     (123)   363580 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/f1345.json
+-rw-r--r--   0 runner    (1001) docker     (123)   370969 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/f1355.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112227 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/f370_f470.json
+-rw-r--r--   0 runner    (1001) docker     (123)   132739 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/f730.json
+-rw-r--r--   0 runner    (1001) docker     (123)   148155 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/f750.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233725 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/s1155_s1255.json
+-rw-r--r--   0 runner    (1001) docker     (123)   152307 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/s2125.json
+-rw-r--r--   0 runner    (1001) docker     (123)   167434 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/s320_s325.json
+-rw-r--r--   0 runner    (1001) docker     (123)   183682 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/s735.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81905 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/smo20.json
+-rw-r--r--   0 runner    (1001) docker     (123)   302299 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/smo40.json
+-rw-r--r--   0 runner    (1001) docker     (123)   242966 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/smos40.json
+-rw-r--r--   0 runner    (1001) docker     (123)   210957 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/vvm225_vvm320_vvm325.json
+-rw-r--r--   0 runner    (1001) docker     (123)   206217 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/data/vvm310_vvm500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/event_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/heatpump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:19.000000 nibe-2.3.0/nibe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:28.647865 nibe-2.3.0/nibe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42067 2023-07-10 14:57:28.000000 nibe-2.3.0/nibe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-10 14:57:28.000000 nibe-2.3.0/nibe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:57:28.000000 nibe-2.3.0/nibe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 14:57:28.000000 nibe-2.3.0/nibe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-10 14:57:28.000000 nibe-2.3.0/nibe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 14:57:28.000000 nibe-2.3.0/nibe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:57:28.000000 nibe-2.3.0/nibe.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-10 14:57:19.000000 nibe-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-10 14:57:28.659866 nibe-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:57:28.655866 nibe-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-10 14:57:19.000000 nibe-2.3.0/tests/test_coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-10 14:57:19.000000 nibe-2.3.0/tests/test_heatpump.py
```

### Comparing `nibe-2.2.0/LICENSE` & `nibe-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/PKG-INFO` & `nibe-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibe
-Version: 2.2.0
+Version: 2.3.0
 Summary: Nibe heatpump communication library
 Home-page: https://github.com/yozik04/nibe
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/nibe/issues
 Keywords: nibe modbus library nibegw
```

### Comparing `nibe-2.2.0/README.md` & `nibe-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/coil.py` & `nibe-2.3.0/nibe/coil.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/coil_groups.py` & `nibe-2.3.0/nibe/coil_groups.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/connection/__init__.py` & `nibe-2.3.0/nibe/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/connection/encoders.py` & `nibe-2.3.0/nibe/connection/encoders.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/connection/mixins.py` & `nibe-2.3.0/nibe/connection/mixins.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/connection/modbus.py` & `nibe-2.3.0/nibe/connection/modbus.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/connection/nibegw.py` & `nibe-2.3.0/nibe/connection/nibegw.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/console_scripts/cli.py` & `nibe-2.3.0/nibe/console_scripts/cli.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/console_scripts/convert_csv.py` & `nibe-2.3.0/nibe/console_scripts/convert_csv.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/extensions.json` & `nibe-2.3.0/nibe/data/extensions.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {'11': "{'files': {insert: [(1, 'f1145_f1245.json')]}}",*

 * * '4': "{'files': {insert: [(1, 'f750.json')]}}"}*

```diff
@@ -118,14 +118,15 @@
                 "size": "u8",
                 "title": "Fan Mode",
                 "write": true
             }
         },
         "files": [
             "f370_f470.json",
+            "f750.json",
             "vvm225_vvm320_vvm325.json"
         ]
     },
     {
         "data": {
             "48852": {
                 "default": 1.0,
@@ -251,11 +252,12 @@
             "47377": {
                 "mappings": null,
                 "size": "s16"
             }
         },
         "description": "Allow for numerical selection for Outdoor Filter Time",
         "files": [
-            "smo40.json"
+            "smo40.json",
+            "f1145_f1245.json"
         ]
     }
 ]
```

### Comparing `nibe-2.2.0/nibe/data/f1145_f1245.json` & `nibe-2.3.0/nibe/data/f1145_f1245.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999554075747666%*

 * *Differences: {"'47377'": "{'size': 's16', delete: ['mappings']}"}*

```diff
@@ -9113,22 +9113,18 @@
         "unit": "\u00b0C",
         "write": true
     },
     "47377": {
         "default": 24.0,
         "factor": 1,
         "info": " 12=12 Hours 24=24 Hours",
-        "mappings": {
-            "12": "12 Hours",
-            "24": "24 Hours"
-        },
         "max": 48.0,
         "min": 0.0,
         "name": "outdoor-filter-time-47377",
-        "size": "u8",
+        "size": "s16",
         "title": "Outdoor Filter Time",
         "unit": "h",
         "write": true
     },
     "47378": {
         "default": 100.0,
         "factor": 10,
```

### Comparing `nibe-2.2.0/nibe/data/f1155_f1255.json` & `nibe-2.3.0/nibe/data/f1155_f1255.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/f1345.json` & `nibe-2.3.0/nibe/data/f1345.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/f1355.json` & `nibe-2.3.0/nibe/data/f1355.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/f370_f470.json` & `nibe-2.3.0/nibe/data/f370_f470.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/f730.json` & `nibe-2.3.0/nibe/data/f730.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/f750.json` & `nibe-2.3.0/nibe/data/f750.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984399375975039%*

 * *Differences: {"'47260'": "OrderedDict([('title', 'Fan Mode'), ('info', '0=Normal 1=Fan speed 1, 2=Fan speed 2, "*

 * *            "3=Fan speed 3, 4=Fan speed 4'), ('size', 'u8'), ('factor', 1), ('min', 0), ('max', "*

 * *            "4), ('default', 0), ('name', 'fan-mode-47260'), ('write', True), ('mappings', "*

 * *            "OrderedDict([('0', 'Normal'), ('1', 'Fan mode 1'), ('2', 'Fan mode 2'), ('3', 'Fan "*

 * *            "mode 3'), ('4', 'Fan mode 4')]))])"}*

```diff
@@ -3316,14 +3316,32 @@
         "min": 1.0,
         "name": "fuse-47214",
         "size": "u16",
         "title": "Fuse",
         "unit": "A",
         "write": true
     },
+    "47260": {
+        "default": 0,
+        "factor": 1,
+        "info": "0=Normal 1=Fan speed 1, 2=Fan speed 2, 3=Fan speed 3, 4=Fan speed 4",
+        "mappings": {
+            "0": "Normal",
+            "1": "Fan mode 1",
+            "2": "Fan mode 2",
+            "3": "Fan mode 3",
+            "4": "Fan mode 4"
+        },
+        "max": 4,
+        "min": 0,
+        "name": "fan-mode-47260",
+        "size": "u8",
+        "title": "Fan Mode",
+        "write": true
+    },
     "47261": {
         "default": 100.0,
         "factor": 1,
         "max": 100.0,
         "min": 0.0,
         "name": "exhaust-fan-speed-4-47261",
         "size": "u8",
```

### Comparing `nibe-2.2.0/nibe/data/s1155_s1255.json` & `nibe-2.3.0/nibe/data/s1155_s1255.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/s2125.json` & `nibe-2.3.0/nibe/data/s2125.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/s320_s325.json` & `nibe-2.3.0/nibe/data/s320_s325.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9125554591049384%*

 * *Differences: {"'30001'": "OrderedDict([('title', 'Relay status'), ('factor', 1), ('size', 'u8'), ('name', "*

 * *            "'relay-status-30001')])",*

 * * "'30020'": "OrderedDict([('title', 'Exh. air (AZ30-BT20)'), ('factor', 10), ('unit', '°C'), "*

 * *            "('size', 's16'), ('name', 'exh-air-az30-bt20-30020')])",*

 * * "'30021'": "OrderedDict([('title', 'Extr. air (AZ30-BT21)'), ('factor', 10), ('unit', '°C'), "*

 * *            "('size', 's16'), ('name', 'extr-air-az30-bt21-30021')])",*

 * * "'30043'": "OrderedDict([('title', 'Supp. air […]*

```diff
@@ -1,8 +1,14 @@
 {
+    "30001": {
+        "factor": 1,
+        "name": "relay-status-30001",
+        "size": "u8",
+        "title": "Relay status"
+    },
     "30002": {
         "factor": 10,
         "name": "current-outdoor-temperature-bt1-30002",
         "size": "s16",
         "title": "Current outdoor temperature (BT1)",
         "unit": "\u00b0C"
     },
@@ -51,14 +57,28 @@
     "30010": {
         "factor": 10,
         "name": "hot-water-charging-bt6-30010",
         "size": "s16",
         "title": "Hot water charging (BT6)",
         "unit": "\u00b0C"
     },
+    "30020": {
+        "factor": 10,
+        "name": "exh-air-az30-bt20-30020",
+        "size": "s16",
+        "title": "Exh. air (AZ30-BT20)",
+        "unit": "\u00b0C"
+    },
+    "30021": {
+        "factor": 10,
+        "name": "extr-air-az30-bt21-30021",
+        "size": "s16",
+        "title": "Extr. air (AZ30-BT21)",
+        "unit": "\u00b0C"
+    },
     "30027": {
         "factor": 10,
         "name": "roomsensor-1-1-30027",
         "size": "s16",
         "title": "Roomsensor 1-1",
         "unit": "\u00b0C"
     },
@@ -91,14 +111,21 @@
     },
     "30042": {
         "factor": 1,
         "name": "electrical-anode-eb100-fr1-30042",
         "size": "s16",
         "title": "Electrical anode (EB100-FR1)"
     },
+    "30043": {
+        "factor": 10,
+        "name": "supp-air-az30-bt22-30043",
+        "size": "s16",
+        "title": "Supp. air (AZ30-BT22)",
+        "unit": "\u00b0C"
+    },
     "30047": {
         "factor": 10,
         "name": "current-be3-30047",
         "size": "u32",
         "title": "Current (BE3)",
         "unit": "A"
     },
@@ -112,14 +139,56 @@
     "30051": {
         "factor": 10,
         "name": "current-be1-30051",
         "size": "u32",
         "title": "Current (BE1)",
         "unit": "A"
     },
+    "30061": {
+        "factor": 10,
+        "name": "exh-air-az33-bt20-30061",
+        "size": "s16",
+        "title": "Exh. air (AZ33-BT20)",
+        "unit": "\u00b0C"
+    },
+    "30062": {
+        "factor": 10,
+        "name": "exh-air-az32-bt20-30062",
+        "size": "s16",
+        "title": "Exh. air (AZ32-BT20)",
+        "unit": "\u00b0C"
+    },
+    "30063": {
+        "factor": 10,
+        "name": "exh-air-az31-bt20-30063",
+        "size": "s16",
+        "title": "Exh. air (AZ31-BT20)",
+        "unit": "\u00b0C"
+    },
+    "30064": {
+        "factor": 10,
+        "name": "extract-air-az33-bt21-30064",
+        "size": "s16",
+        "title": "Extract air (AZ33-BT21)",
+        "unit": "\u00b0C"
+    },
+    "30065": {
+        "factor": 10,
+        "name": "extract-air-az32-bt21-30065",
+        "size": "s16",
+        "title": "Extract air (AZ32-BT21)",
+        "unit": "\u00b0C"
+    },
+    "30066": {
+        "factor": 10,
+        "name": "extract-air-az31-bt21-30066",
+        "size": "s16",
+        "title": "Extract air (AZ31-BT21)",
+        "unit": "\u00b0C"
+    },
     "30073": {
         "factor": 10,
         "name": "additional-heat-bt63-30073",
         "size": "s16",
         "title": "Additional heat (BT63)",
         "unit": "\u00b0C"
     },
@@ -210,14 +279,21 @@
     "30102": {
         "factor": 10,
         "name": "return-line-ep44-bt3-30102",
         "size": "s16",
         "title": "Return line (EP44-BT3)",
         "unit": "\u00b0C"
     },
+    "30108": {
+        "factor": 10,
+        "name": "outd-temperature-az30-bt23-30108",
+        "size": "s16",
+        "title": "Outd temperature (AZ30-BT23)",
+        "unit": "\u00b0C"
+    },
     "30110": {
         "factor": 10,
         "name": "room-average-temp-clim-system-8-bt50-30110",
         "size": "s16",
         "title": "Room average temp. clim. system 8 (BT50)",
         "unit": "\u00b0C"
     },
@@ -762,28 +838,55 @@
     },
     "30394": {
         "factor": 1,
         "name": "seconds-of-blank-time-left-charge-pump-0-30394",
         "size": "u8",
         "title": "Seconds of blank time left, charge pump 0"
     },
+    "30401": {
+        "factor": 1,
+        "name": "alarm-number-from-outdoor-air-heat-pump-eb101-30401",
+        "size": "u8",
+        "title": "Alarm number from outdoor air heat pump (EB101)"
+    },
+    "30402": {
+        "factor": 1,
+        "name": "fan-speed-eb101-30402",
+        "size": "u16",
+        "title": "Fan speed (EB101)",
+        "unit": "rpm"
+    },
     "30403": {
         "factor": 1,
         "name": "max-fan-speed-eb101-30403",
         "size": "u16",
         "title": "Max fan speed (EB101)",
         "unit": "rpm"
     },
     "30404": {
         "factor": 1,
         "name": "min-fan-speed-eb101-30404",
         "size": "u16",
         "title": "Min fan speed (EB101)",
         "unit": "rpm"
     },
+    "30405": {
+        "factor": 10,
+        "name": "max-compressor-speed-eb101-30405",
+        "size": "u16",
+        "title": "Max compressor speed (EB101)",
+        "unit": "Hz"
+    },
+    "30406": {
+        "factor": 10,
+        "name": "min-compressor-speed-eb101-30406",
+        "size": "u16",
+        "title": "Min compressor speed (EB101)",
+        "unit": "Hz"
+    },
     "30407": {
         "factor": 10,
         "name": "power-eb101-30407",
         "size": "u16",
         "title": "Power (EB101)",
         "unit": "kW"
     },
@@ -940,14 +1043,21 @@
     "30555": {
         "factor": 10,
         "name": "evi-pressure-eb101-ep14-bp11-dew-30555",
         "size": "s16",
         "title": "EVI pressure (EB101-EP14-BP11 dew)",
         "unit": "\u00b0C"
     },
+    "30556": {
+        "factor": 10,
+        "name": "evaporator-eb101-bt84-30556",
+        "size": "s16",
+        "title": "Evaporator (EB101-BT84)",
+        "unit": "\u00b0C"
+    },
     "30557": {
         "factor": 1,
         "name": "fan-status-eb101-ep14-30557",
         "size": "u8",
         "title": "Fan status (EB101-EP14)"
     },
     "30558": {
@@ -1976,14 +2086,21 @@
     },
     "31562": {
         "factor": 1,
         "name": "date-periodic-hot-water-31562",
         "size": "u16",
         "title": "Date, periodic hot water"
     },
+    "31568": {
+        "factor": 10,
+        "name": "calculated-cooling-supply-climate-system-1-31568",
+        "size": "s16",
+        "title": "Calculated cooling supply climate system 1",
+        "unit": "\u00b0C"
+    },
     "31576": {
         "default": 0.0,
         "factor": 10,
         "max": 9999999.0,
         "min": 0.0,
         "name": "hot-water-including-int-add-heat-31576",
         "size": "u32",
@@ -1996,14 +2113,24 @@
         "max": 9999999.0,
         "min": 0.0,
         "name": "heating-including-int-add-heat-31578",
         "size": "u32",
         "title": "Heating, including int. add. heat",
         "unit": "kWh"
     },
+    "31580": {
+        "default": 0.0,
+        "factor": 10,
+        "max": 9999999.0,
+        "min": 0.0,
+        "name": "cooling-compressor-only-31580",
+        "size": "u32",
+        "title": "Cooling, compressor only",
+        "unit": "kWh"
+    },
     "31584": {
         "default": 0.0,
         "factor": 10,
         "max": 9999999.0,
         "min": 0.0,
         "name": "hot-water-compressor-only-31584",
         "size": "u32",
@@ -2306,14 +2433,29 @@
     },
     "32129": {
         "factor": 1,
         "name": "pump-heating-medium-gp6-32129",
         "size": "u8",
         "title": "Pump: Heating medium (GP6)"
     },
+    "32148": {
+        "factor": 1,
+        "name": "version-inverter-eb101-32148",
+        "size": "u8",
+        "title": "Version, inverter (EB101)"
+    },
+    "32159": {
+        "default": 255.0,
+        "factor": 1,
+        "max": 255.0,
+        "min": 0.0,
+        "name": "last-defrost-heat-pump-1-32159",
+        "size": "u8",
+        "title": "Last defrost, heat pump 1"
+    },
     "32169": {
         "factor": 1,
         "name": "fan-mode-5-32169",
         "size": "u8",
         "title": "Fan mode 5",
         "unit": "%"
     },
@@ -2394,14 +2536,138 @@
     },
     "32197": {
         "factor": 1,
         "name": "reversing-valve-hot-water-qn10-32197",
         "size": "u8",
         "title": "Reversing valve hot water (QN10)"
     },
+    "32252": {
+        "factor": 1,
+        "name": "fan-speed-ers1-gq2-32252",
+        "size": "u8",
+        "title": "Fan speed ERS1 (GQ2)",
+        "unit": "%"
+    },
+    "32253": {
+        "factor": 1,
+        "name": "fan-speed-ers1-gq3-32253",
+        "size": "u8",
+        "title": "Fan speed ERS1 (GQ3)",
+        "unit": "%"
+    },
+    "32284": {
+        "factor": 100,
+        "name": "energy-log-energy-produced-for-heat-during-past-hour-32284",
+        "size": "u32",
+        "title": "Energy log - Energy produced for heat during past hour",
+        "unit": "kWh"
+    },
+    "32286": {
+        "factor": 100,
+        "name": "energy-log-energy-produced-for-hot-water-during-past-hour-32286",
+        "size": "u32",
+        "title": "Energy log - Energy produced for hot water during past hour",
+        "unit": "kWh"
+    },
+    "32290": {
+        "factor": 100,
+        "name": "energy-log-energy-produced-for-cooling-during-past-hour-32290",
+        "size": "u32",
+        "title": "Energy log - Energy produced for cooling during past hour",
+        "unit": "kWh"
+    },
+    "32292": {
+        "factor": 100,
+        "name": "energy-log-energy-used-for-heat-during-past-hour-32292",
+        "size": "u32",
+        "title": "Energy log - Energy used for heat during past hour",
+        "unit": "kWh"
+    },
+    "32294": {
+        "factor": 100,
+        "name": "energy-log-energy-used-for-hot-water-during-past-hour-32294",
+        "size": "u32",
+        "title": "Energy log - Energy used for hot water during past hour",
+        "unit": "kWh"
+    },
+    "32298": {
+        "factor": 100,
+        "name": "energy-log-energy-used-for-cooling-during-past-hour-32298",
+        "size": "u32",
+        "title": "Energy log - Energy used for cooling during past hour",
+        "unit": "kWh"
+    },
+    "32300": {
+        "factor": 100,
+        "name": "energy-log-energy-used-by-additional-heater-for-heat-during-past-hour-32300",
+        "size": "u32",
+        "title": "Energy log - Energy used by additional heater for heat during past hour",
+        "unit": "kWh"
+    },
+    "32302": {
+        "factor": 100,
+        "name": "energy-log-energy-used-by-additional-heater-for-hot-water-during-past-hour-32302",
+        "size": "u32",
+        "title": "Energy log - Energy used by additional heater for hot water during past hour",
+        "unit": "kWh"
+    },
+    "32306": {
+        "factor": 100,
+        "name": "energy-log-current-power-consumption-32306",
+        "size": "u32",
+        "title": "Energy log - Current power consumption",
+        "unit": "kW"
+    },
+    "32308": {
+        "factor": 100,
+        "name": "energy-log-current-power-consumption-components-32308",
+        "size": "u32",
+        "title": "Energy log - Current power consumption, components",
+        "unit": "kW"
+    },
+    "32336": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-main-unit-ep14-32336",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, main unit (EP14)",
+        "unit": "h"
+    },
+    "32338": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-main-unit-ep15-32338",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, main unit (EP15)",
+        "unit": "h"
+    },
+    "32340": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-1-ep14-32340",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 1 (EP14)",
+        "unit": "h"
+    },
+    "32342": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-1-ep15-32342",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 1 (EP15)",
+        "unit": "h"
+    },
     "40001": {
         "default": 1.0,
         "factor": 1,
         "max": 50.0,
         "min": 1.0,
         "name": "temperature-overload-pool-40001",
         "size": "u8",
@@ -2656,37 +2922,37 @@
         "min": 0.0,
         "name": "hot-water-demand-mode-40057",
         "size": "s8",
         "title": "Hot water demand mode",
         "write": true
     },
     "40059": {
-        "default": 450.0,
+        "default": 440.0,
         "factor": 10,
         "max": 700.0,
         "min": 50.0,
         "name": "start-temperature-hw-high-temperature-40059",
         "size": "s16",
         "title": "Start temperature HW high temperature",
         "unit": "\u00b0C",
         "write": true
     },
     "40060": {
-        "default": 420.0,
+        "default": 410.0,
         "factor": 10,
         "max": 700.0,
         "min": 50.0,
         "name": "start-temperature-hw-normal-temperature-40060",
         "size": "s16",
         "title": "Start temperature HW normal temperature",
         "unit": "\u00b0C",
         "write": true
     },
     "40061": {
-        "default": 390.0,
+        "default": 380.0,
         "factor": 10,
         "max": 700.0,
         "min": 50.0,
         "name": "start-temperature-hw-low-temperature-40061",
         "size": "s16",
         "title": "Start temperature HW low temperature",
         "unit": "\u00b0C",
@@ -2824,14 +3090,78 @@
         "min": 1.0,
         "name": "fuse-40104",
         "size": "u16",
         "title": "Fuse",
         "unit": "A",
         "write": true
     },
+    "40105": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 4.0,
+        "min": 0.0,
+        "name": "ventilation-mode-40105",
+        "size": "u8",
+        "title": "Ventilation mode",
+        "write": true
+    },
+    "40116": {
+        "default": 4.0,
+        "factor": 1,
+        "max": 24.0,
+        "min": 1.0,
+        "name": "return-time-fan-4-40116",
+        "size": "u8",
+        "title": "Return time fan 4",
+        "unit": "h",
+        "write": true
+    },
+    "40117": {
+        "default": 4.0,
+        "factor": 1,
+        "max": 24.0,
+        "min": 1.0,
+        "name": "return-time-fan-3-40117",
+        "size": "u8",
+        "title": "Return time fan 3",
+        "unit": "h",
+        "write": true
+    },
+    "40118": {
+        "default": 4.0,
+        "factor": 1,
+        "max": 24.0,
+        "min": 1.0,
+        "name": "return-time-fan-2-40118",
+        "size": "u8",
+        "title": "Return time fan 2",
+        "unit": "h",
+        "write": true
+    },
+    "40119": {
+        "default": 4.0,
+        "factor": 1,
+        "max": 24.0,
+        "min": 1.0,
+        "name": "return-time-fan-1-40119",
+        "size": "u8",
+        "title": "Return time fan 1",
+        "unit": "h",
+        "write": true
+    },
+    "40120": {
+        "default": 3.0,
+        "factor": 1,
+        "max": 24.0,
+        "min": 1.0,
+        "name": "time-between-filter-replacement-40120",
+        "size": "u8",
+        "title": "Time between filter replacement",
+        "write": true
+    },
     "40121": {
         "default": 0.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "floor-drying-40121",
         "size": "u8",
@@ -3436,65 +3766,65 @@
         "size": "u8",
         "title": "Room sensor factor climate system 1",
         "write": true
     },
     "40212": {
         "default": 0.0,
         "factor": 1,
-        "max": 61.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux5-40212",
         "size": "u8",
         "title": "Input AUX5",
         "write": true
     },
     "40213": {
         "default": 0.0,
         "factor": 1,
-        "max": 61.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux4-40213",
         "size": "u8",
         "title": "Input AUX4",
         "write": true
     },
     "40214": {
         "default": 0.0,
         "factor": 1,
-        "max": 61.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux3-40214",
         "size": "u8",
         "title": "Input AUX3",
         "write": true
     },
     "40215": {
         "default": 0.0,
         "factor": 1,
-        "max": 61.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux2-40215",
         "size": "u8",
         "title": "Input AUX2",
         "write": true
     },
     "40216": {
         "default": 0.0,
         "factor": 1,
-        "max": 61.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux1-40216",
         "size": "u8",
         "title": "Input AUX1",
         "write": true
     },
     "40217": {
         "default": 0.0,
         "factor": 1,
-        "max": 26.0,
+        "max": 28.0,
         "min": 0.0,
         "name": "output-aux1-40217",
         "size": "u8",
         "title": "Output AUX1",
         "write": true
     },
     "40224": {
@@ -3510,14 +3840,24 @@
     "40226": {
         "factor": 10,
         "name": "more-hot-water-40226",
         "size": "u16",
         "title": "More hot water",
         "write": true
     },
+    "40228": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "night-cooling-1-40228",
+        "size": "u8",
+        "title": "Night cooling 1",
+        "write": true
+    },
     "40238": {
         "factor": 1,
         "name": "oper-mode-40238",
         "size": "u8",
         "title": "Oper. mode",
         "write": true
     },
@@ -3585,21 +3925,90 @@
         "max": 1.0,
         "min": 0.0,
         "name": "external-cooling-accessory-40710",
         "size": "u8",
         "title": "External cooling accessory",
         "write": true
     },
+    "40721": {
+        "default": 18.0,
+        "factor": 1,
+        "max": 30.0,
+        "min": 18.0,
+        "name": "min-supply-temp-cooling-climate-system-1-40721",
+        "size": "s8",
+        "title": "Min. supply temp. cooling climate system 1",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40722": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p3-40722",
+        "size": "s8",
+        "title": "Own curve, cooling P3",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40723": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p5-40723",
+        "size": "s8",
+        "title": "Own curve, cooling P5",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "40727": {
+        "default": 1.0,
         "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
         "name": "cooling-connected-climate-system-1-40727",
         "size": "u8",
         "title": "Cooling connected, climate system 1",
         "write": true
     },
+    "40737": {
+        "default": 30.0,
+        "factor": 1,
+        "max": 180.0,
+        "min": 0.0,
+        "name": "period-time-cooling-40737",
+        "size": "u8",
+        "title": "Period time cooling",
+        "unit": "min",
+        "write": true
+    },
+    "40739": {
+        "default": 3.0,
+        "factor": 1,
+        "max": 10.0,
+        "min": 3.0,
+        "name": "cooling-delta-temp-20degc-40739",
+        "size": "s8",
+        "title": "Cooling delta temp. 20\u00b0C",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40740": {
+        "default": 6.0,
+        "factor": 1,
+        "max": 20.0,
+        "min": 3.0,
+        "name": "cooling-delta-temp-40degc-40740",
+        "size": "s8",
+        "title": "Cooling delta temp. 40\u00b0C",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "40749": {
         "default": 1.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "operating-mode-charge-pump-climate-system-1-40749",
         "size": "u8",
@@ -3615,15 +4024,15 @@
         "size": "u8",
         "title": "Heating (SG Ready)",
         "write": true
     },
     "40768": {
         "default": 0.0,
         "factor": 1,
-        "max": 61.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux5-40768",
         "size": "u8",
         "title": "Input AUX5",
         "write": true
     },
     "40784": {
@@ -3642,14 +4051,35 @@
         "max": 1.0,
         "min": 0.0,
         "name": "operating-mode-circulation-pump-hot-water-heat-pump-1-40800",
         "size": "u8",
         "title": "Operating mode circulation pump hot water heat pump 1",
         "write": true
     },
+    "40824": {
+        "default": 70.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 1.0,
+        "name": "speed-circulation-pump-cooling-heat-pump-1-40824",
+        "size": "u8",
+        "title": "Speed circulation pump cooling heat pump 1",
+        "unit": "%",
+        "write": true
+    },
+    "40833": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "operating-mode-circulation-pump-cooling-heat-pump-1-40833",
+        "size": "u8",
+        "title": "Operating mode circulation pump cooling heat pump 1",
+        "write": true
+    },
     "40842": {
         "default": 30.0,
         "factor": 1,
         "max": 100.0,
         "min": 1.0,
         "name": "speed-circulation-pump-waiting-mode-heat-pump-1-40842",
         "size": "u8",
@@ -3973,14 +4403,67 @@
         "max": 60.0,
         "min": 0.0,
         "name": "room-sensor-factor-climate-system-5-40960",
         "size": "u8",
         "title": "Room sensor factor climate system 5",
         "write": true
     },
+    "40968": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 9.0,
+        "min": 0.0,
+        "name": "cooling-curve-climate-system-1-40968",
+        "size": "s8",
+        "title": "Cooling curve climate system 1",
+        "write": true
+    },
+    "40976": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 10.0,
+        "min": -10.0,
+        "name": "cooling-offset-climate-system-1-40976",
+        "size": "s8",
+        "title": "Cooling offset climate system 1",
+        "write": true
+    },
+    "40977": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p4-40977",
+        "size": "s8",
+        "title": "Own curve, cooling P4",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40978": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p2-40978",
+        "size": "s8",
+        "title": "Own curve, cooling P2",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40979": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p1-40979",
+        "size": "s8",
+        "title": "Own curve, cooling P1",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "40981": {
         "default": 300.0,
         "factor": 1,
         "max": 3000.0,
         "min": 300.0,
         "name": "current-transformer-ratio-40981",
         "size": "u16",
@@ -4279,14 +4762,80 @@
         "min": 1.0,
         "name": "pump-speed-s135-41037",
         "size": "u8",
         "title": "Pump speed (S135)",
         "unit": "%",
         "write": true
     },
+    "41039": {
+        "default": 100.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 0.0,
+        "name": "supply-air-fan-speed-4-ers-1-41039",
+        "size": "u8",
+        "title": "Supply air fan speed 4 (ERS 1)",
+        "unit": "%",
+        "write": true
+    },
+    "41040": {
+        "default": 80.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 0.0,
+        "name": "supply-air-fan-speed-3-ers-1-41040",
+        "size": "u8",
+        "title": "Supply air fan speed 3 (ERS 1)",
+        "unit": "%",
+        "write": true
+    },
+    "41041": {
+        "default": 30.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 0.0,
+        "name": "supply-air-fan-speed-2-ers-1-41041",
+        "size": "u8",
+        "title": "Supply air fan speed 2 (ERS 1)",
+        "unit": "%",
+        "write": true
+    },
+    "41042": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 0.0,
+        "name": "supply-air-fan-speed-1-ers-1-41042",
+        "size": "u8",
+        "title": "Supply air fan speed 1 (ERS 1)",
+        "unit": "%",
+        "write": true
+    },
+    "41043": {
+        "default": 60.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 1.0,
+        "name": "supply-air-fan-speed-normal-ers-1-41043",
+        "size": "u8",
+        "title": "Supply air fan speed normal (ERS 1)",
+        "unit": "%",
+        "write": true
+    },
+    "41044": {
+        "default": 3.0,
+        "factor": 1,
+        "max": 10.0,
+        "min": 0.0,
+        "name": "min-vent-temp-ers-1-41044",
+        "size": "u8",
+        "title": "Min. vent temp. (ERS 1)",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "41045": {
         "default": 4.0,
         "factor": 1,
         "max": 10.0,
         "min": 2.0,
         "name": "bypass-temp-ers-1-41045",
         "size": "u8",
@@ -5937,15 +6486,15 @@
         "size": "u8",
         "title": "Time between filter replacement",
         "write": true
     },
     "42741": {
         "default": 0.0,
         "factor": 1,
-        "max": 61.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "aux-from-modbus-42741",
         "size": "u8",
         "title": "AUX from Modbus",
         "write": true
     },
     "42742": {
@@ -6198,14 +6747,24 @@
         "max": 1.0,
         "min": 0.0,
         "name": "heating-auto-43060",
         "size": "u8",
         "title": "Heating, auto",
         "write": true
     },
+    "43061": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "cooling-auto-43061",
+        "size": "u8",
+        "title": "Cooling, auto",
+        "write": true
+    },
     "43067": {
         "default": 0.0,
         "factor": 1,
         "max": 127.0,
         "min": 0.0,
         "name": "active-days-43067",
         "size": "u8",
@@ -6282,15 +6841,15 @@
         "size": "u8",
         "title": "Period",
         "write": true
     },
     "43090": {
         "default": 1.0,
         "factor": 1,
-        "max": 5.0,
+        "max": 10.0,
         "min": 1.0,
         "name": "number-of-years-43090",
         "size": "u8",
         "title": "Number of years",
         "write": true
     },
     "43091": {
@@ -6355,14 +6914,41 @@
         "min": 1.0,
         "name": "minimum-permitted-speed-eb101-gp12-43244",
         "size": "u8",
         "title": "Minimum permitted speed (EB101 GP12)",
         "unit": "%",
         "write": true
     },
+    "43252": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "start-fan-de-icing-eb101-43252",
+        "size": "s8",
+        "title": "Start fan de-icing (EB101)",
+        "write": true
+    },
+    "43628": {
+        "factor": 1,
+        "name": "increased-ventilation-1-43628",
+        "size": "u8",
+        "title": "Increased ventilation 1",
+        "write": true
+    },
+    "43629": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "disable-emergency-restart-gp1-43629",
+        "size": "u8",
+        "title": "Disable emergency restart GP1",
+        "write": true
+    },
     "43987": {
         "default": 0.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "disable-emergency-restart-gp1-43987",
         "size": "u8",
@@ -6426,14 +7012,45 @@
         "max": 1.0,
         "min": 0.0,
         "name": "ers-4-44079",
         "size": "u8",
         "title": "ERS 4",
         "write": true
     },
+    "44086": {
+        "default": 25.0,
+        "factor": 1,
+        "max": 30.0,
+        "min": 5.0,
+        "name": "bypass-set-point-value-ers-1-44086",
+        "size": "u8",
+        "title": "Bypass set point value (ERS 1)",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "44090": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "bypass-during-heating-ers-1-44090",
+        "size": "u8",
+        "title": "Bypass during heating (ERS 1)",
+        "write": true
+    },
+    "44095": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "ers-1-44095",
+        "size": "u8",
+        "title": "ERS 1",
+        "write": true
+    },
     "44101": {
         "default": 2.0,
         "factor": 1,
         "max": 2.0,
         "min": 0.0,
         "name": "blocking-actions-ers-3-44101",
         "size": "u8",
@@ -6720,9 +7337,62 @@
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "disable-emergency-restart-gp1-45026",
         "size": "u8",
         "title": "Disable emergency restart GP1",
         "write": true
+    },
+    "45027": {
+        "factor": 1,
+        "name": "forced-control-az30-eb17-45027",
+        "size": "u8",
+        "title": "Forced control (AZ30-EB17)",
+        "write": true
+    },
+    "45028": {
+        "factor": 1,
+        "name": "forced-control-az30-qn37-open-45028",
+        "size": "u8",
+        "title": "Forced control (AZ30-QN37) (open)",
+        "write": true
+    },
+    "45029": {
+        "factor": 1,
+        "name": "forced-control-az30-qn37-close-45029",
+        "size": "u8",
+        "title": "Forced control (AZ30-QN37) (close)",
+        "write": true
+    },
+    "45030": {
+        "default": 50.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 0.0,
+        "name": "forced-control-az30-gq2-45030",
+        "size": "u8",
+        "title": "Forced control (AZ30-GQ2)",
+        "unit": "%",
+        "write": true
+    },
+    "45031": {
+        "default": 50.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 0.0,
+        "name": "forced-control-az30-gq3-45031",
+        "size": "u8",
+        "title": "Forced control (AZ30-GQ3)",
+        "unit": "%",
+        "write": true
+    },
+    "45102": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "heat-pump-test-silent-mode-eb101-eb102-45102",
+        "size": "u8",
+        "title": "Heat pump test - Silent mode (EB101/EB102)",
+        "write": true
     }
 }
```

### Comparing `nibe-2.2.0/nibe/data/s735.json` & `nibe-2.3.0/nibe/data/s735.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/smo20.json` & `nibe-2.3.0/nibe/data/smo20.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/smo40.json` & `nibe-2.3.0/nibe/data/smo40.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/smos40.json` & `nibe-2.3.0/nibe/data/smos40.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9561433281613654%*

 * *Differences: {"'30001'": "OrderedDict([('title', 'Relay status'), ('factor', 1), ('size', 'u8'), ('name', "*

 * *            "'id-30001-relay-status-30001-relay-status-name-title-dtype-object-id-30001-30001-30001-30001-name-id-dtype-string')])",*

 * * "'30540'": "OrderedDict([('title', 'Evaporator (EB102-BT84)'), ('factor', 10), ('unit', '°C'), "*

 * *            "('size', 's16'), ('name', 'evaporator-eb102-bt84-30540')])",*

 * * "'30911'": "OrderedDict([('title', 'Alarm number from outdoor air heat pump (EB102)'), ('factor', "*

 * *            […]*

```diff
@@ -1,8 +1,14 @@
 {
+    "30001": {
+        "factor": 1,
+        "name": "id-30001-relay-status-30001-relay-status-name-title-dtype-object-id-30001-30001-30001-30001-name-id-dtype-string",
+        "size": "u8",
+        "title": "Relay status"
+    },
     "30002": {
         "factor": 10,
         "name": "current-outdoor-temperature-bt1-30002",
         "size": "s16",
         "title": "Current outdoor temperature (BT1)",
         "unit": "\u00b0C"
     },
@@ -1781,14 +1787,21 @@
     "30539": {
         "factor": 10,
         "name": "evi-pressure-eb102-ep14-bp11-dew-30539",
         "size": "s16",
         "title": "EVI pressure (EB102-EP14-BP11 dew)",
         "unit": "\u00b0C"
     },
+    "30540": {
+        "factor": 10,
+        "name": "evaporator-eb102-bt84-30540",
+        "size": "s16",
+        "title": "Evaporator (EB102-BT84)",
+        "unit": "\u00b0C"
+    },
     "30541": {
         "factor": 1,
         "name": "fan-status-eb102-ep14-30541",
         "size": "u8",
         "title": "Fan status (EB102-EP14)"
     },
     "30542": {
@@ -3066,14 +3079,20 @@
     },
     "30910": {
         "factor": 1,
         "name": "degree-of-opening-evi-eb103-30910",
         "size": "u16",
         "title": "Degree of opening EVI (EB103)"
     },
+    "30911": {
+        "factor": 1,
+        "name": "alarm-number-from-outdoor-air-heat-pump-eb102-30911",
+        "size": "u8",
+        "title": "Alarm number from outdoor air heat pump (EB102)"
+    },
     "30912": {
         "factor": 1,
         "name": "fan-speed-eb102-30912",
         "size": "u16",
         "title": "Fan speed (EB102)",
         "unit": "rpm"
     },
@@ -3087,14 +3106,28 @@
     "30914": {
         "factor": 1,
         "name": "min-fan-speed-eb102-30914",
         "size": "u16",
         "title": "Min fan speed (EB102)",
         "unit": "rpm"
     },
+    "30915": {
+        "factor": 10,
+        "name": "max-compressor-speed-eb102-30915",
+        "size": "u16",
+        "title": "Max compressor speed (EB102)",
+        "unit": "Hz"
+    },
+    "30916": {
+        "factor": 10,
+        "name": "min-compressor-speed-eb102-30916",
+        "size": "u16",
+        "title": "Min compressor speed (EB102)",
+        "unit": "Hz"
+    },
     "30917": {
         "factor": 10,
         "name": "power-eb102-30917",
         "size": "u16",
         "title": "Power (EB102)",
         "unit": "kW"
     },
@@ -3403,14 +3436,20 @@
     },
     "31063": {
         "factor": 1,
         "name": "step-controlled-add-heat-blocking-31063",
         "size": "u8",
         "title": "Step controlled add. heat blocking"
     },
+    "31064": {
+        "factor": 1,
+        "name": "hot-water-circulation-gp11-31064",
+        "size": "u8",
+        "title": "Hot water circulation (GP11)"
+    },
     "31067": {
         "factor": 1,
         "name": "external-heating-medium-pump-gp10-status-31067",
         "size": "u8",
         "title": "External heating medium pump (GP10) status"
     },
     "31068": {
@@ -3966,14 +4005,21 @@
     },
     "31562": {
         "factor": 1,
         "name": "date-periodic-hot-water-31562",
         "size": "u16",
         "title": "Date, periodic hot water"
     },
+    "31568": {
+        "factor": 10,
+        "name": "calculated-cooling-supply-climate-system-1-31568",
+        "size": "s16",
+        "title": "Calculated cooling supply climate system 1",
+        "unit": "\u00b0C"
+    },
     "31569": {
         "factor": 1,
         "name": "status-acs-31569",
         "size": "u8",
         "title": "Status (ACS)"
     },
     "31570": {
@@ -4018,14 +4064,24 @@
         "max": 9999999.0,
         "min": 0.0,
         "name": "hot-water-including-int-add-heat-31576",
         "size": "u32",
         "title": "Hot water, including int. add. heat",
         "unit": "kWh"
     },
+    "31580": {
+        "default": 0.0,
+        "factor": 10,
+        "max": 9999999.0,
+        "min": 0.0,
+        "name": "cooling-compressor-only-31580",
+        "size": "u32",
+        "title": "Cooling, compressor only",
+        "unit": "kWh"
+    },
     "31584": {
         "default": 0.0,
         "factor": 10,
         "max": 9999999.0,
         "min": 0.0,
         "name": "hot-water-compressor-only-31584",
         "size": "u32",
@@ -4998,23 +5054,38 @@
     },
     "32148": {
         "factor": 1,
         "name": "version-inverter-eb101-32148",
         "size": "u8",
         "title": "Version, inverter (EB101)"
     },
+    "32149": {
+        "factor": 1,
+        "name": "version-inverter-eb102-32149",
+        "size": "u8",
+        "title": "Version, inverter (EB102)"
+    },
     "32159": {
         "default": 255.0,
         "factor": 1,
         "max": 255.0,
         "min": 0.0,
         "name": "last-defrost-heat-pump-1-32159",
         "size": "u8",
         "title": "Last defrost, heat pump 1"
     },
+    "32160": {
+        "default": 255.0,
+        "factor": 1,
+        "max": 255.0,
+        "min": 0.0,
+        "name": "last-defrost-heat-pump-2-32160",
+        "size": "u8",
+        "title": "Last defrost, heat pump 2"
+    },
     "32169": {
         "factor": 1,
         "name": "fan-mode-5-32169",
         "size": "u8",
         "title": "Fan mode 5",
         "unit": "%"
     },
@@ -5048,14 +5119,21 @@
     "32177": {
         "factor": 1,
         "name": "current-power-eme-20-32177",
         "size": "u32",
         "title": "Current power (EME 20)",
         "unit": "W"
     },
+    "32178": {
+        "factor": 100,
+        "name": "current-power-32178",
+        "size": "u32",
+        "title": "Current power",
+        "unit": "kW"
+    },
     "32179": {
         "factor": 1,
         "name": "total-average-power-eme-20-32179",
         "size": "u32",
         "title": "Total average power (EME 20)",
         "unit": "W"
     },
@@ -5199,14 +5277,194 @@
     "32308": {
         "factor": 100,
         "name": "energy-log-current-power-consumption-components-32308",
         "size": "u32",
         "title": "Energy log - Current power consumption, components",
         "unit": "kW"
     },
+    "35181": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-main-unit-ep14-35181",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, main unit (EP14)",
+        "unit": "h"
+    },
+    "35182": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-main-unit-ep15-35182",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, main unit (EP15)",
+        "unit": "h"
+    },
+    "35183": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-1-ep14-35183",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 1 (EP14)",
+        "unit": "h"
+    },
+    "35184": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-1-ep15-35184",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 1 (EP15)",
+        "unit": "h"
+    },
+    "35185": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-2-ep14-35185",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 2 (EP14)",
+        "unit": "h"
+    },
+    "35186": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-2-ep15-35186",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 2 (EP15)",
+        "unit": "h"
+    },
+    "35187": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-3-ep14-35187",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 3 (EP14)",
+        "unit": "h"
+    },
+    "35188": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-3-ep15-35188",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 3 (EP15)",
+        "unit": "h"
+    },
+    "35189": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-4-ep14-35189",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 4 (EP14)",
+        "unit": "h"
+    },
+    "35190": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-4-ep15-35190",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 4 (EP15)",
+        "unit": "h"
+    },
+    "35191": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-5-ep14-35191",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 5 (EP14)",
+        "unit": "h"
+    },
+    "35192": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-5-ep15-35192",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 5 (EP15)",
+        "unit": "h"
+    },
+    "35193": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-6-ep14-35193",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 6 (EP14)",
+        "unit": "h"
+    },
+    "35194": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-6-ep15-35194",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 6 (EP15)",
+        "unit": "h"
+    },
+    "35195": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-7-ep14-35195",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 7 (EP14)",
+        "unit": "h"
+    },
+    "35196": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-7-ep15-35196",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 7 (EP15)",
+        "unit": "h"
+    },
+    "35197": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-8-ep14-35197",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 8 (EP14)",
+        "unit": "h"
+    },
+    "35198": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-total-time-energy-storage-heat-pump-8-ep15-35198",
+        "size": "u32",
+        "title": "Compressor, total time energy storage, heat pump 8 (EP15)",
+        "unit": "h"
+    },
     "40001": {
         "default": 1.0,
         "factor": 1,
         "max": 50.0,
         "min": 1.0,
         "name": "temperature-overload-pool-40001",
         "size": "u8",
@@ -5554,14 +5812,25 @@
     "40068": {
         "factor": 1,
         "name": "start-time-periodic-hot-water-40068",
         "size": "u16",
         "title": "Start time periodic hot water",
         "write": true
     },
+    "40070": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 60.0,
+        "min": 0.0,
+        "name": "downtime-40070",
+        "size": "s8",
+        "title": "Downtime",
+        "unit": "min",
+        "write": true
+    },
     "40092": {
         "default": 0.0,
         "factor": 1,
         "max": 22.0,
         "min": 0.0,
         "name": "language-40092",
         "size": "s8",
@@ -6261,65 +6530,65 @@
         "size": "u8",
         "title": "Room sensor factor climate system 1",
         "write": true
     },
     "40212": {
         "default": 0.0,
         "factor": 1,
-        "max": 59.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux5-40212",
         "size": "u8",
         "title": "Input AUX5",
         "write": true
     },
     "40213": {
         "default": 0.0,
         "factor": 1,
-        "max": 59.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux4-40213",
         "size": "u8",
         "title": "Input AUX4",
         "write": true
     },
     "40214": {
         "default": 0.0,
         "factor": 1,
-        "max": 59.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux3-40214",
         "size": "u8",
         "title": "Input AUX3",
         "write": true
     },
     "40215": {
         "default": 0.0,
         "factor": 1,
-        "max": 59.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux2-40215",
         "size": "u8",
         "title": "Input AUX2",
         "write": true
     },
     "40216": {
         "default": 0.0,
         "factor": 1,
-        "max": 59.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux1-40216",
         "size": "u8",
         "title": "Input AUX1",
         "write": true
     },
     "40217": {
         "default": 0.0,
         "factor": 1,
-        "max": 25.0,
+        "max": 27.0,
         "min": 0.0,
         "name": "output-aux1-40217",
         "size": "u8",
         "title": "Output AUX1",
         "write": true
     },
     "40224": {
@@ -6331,19 +6600,19 @@
         "size": "u8",
         "title": "Preset flow setting for climate system",
         "write": true
     },
     "40225": {
         "default": 5.0,
         "factor": 1,
-        "max": 25.0,
+        "max": 27.0,
         "min": 0.0,
-        "name": "aux-relay-x11-40225",
+        "name": "aux-relay-aux11-40225",
         "size": "u8",
-        "title": "AUX relay (X11)",
+        "title": "AUX relay (AUX11)",
         "write": true
     },
     "40226": {
         "factor": 10,
         "name": "more-hot-water-40226",
         "size": "u16",
         "title": "More hot water",
@@ -6482,16 +6751,52 @@
         "max": 1.0,
         "min": 0.0,
         "name": "hw-comfort-additional-heat-40711",
         "size": "u8",
         "title": "HW comfort additional heat",
         "write": true
     },
+    "40721": {
+        "default": 18.0,
+        "factor": 1,
+        "max": 30.0,
+        "min": 7.0,
+        "name": "min-supply-temp-cooling-climate-system-1-40721",
+        "size": "s8",
+        "title": "Min. supply temp. cooling climate system 1",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40722": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p3-40722",
+        "size": "s8",
+        "title": "Own curve, cooling P3",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40723": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p5-40723",
+        "size": "s8",
+        "title": "Own curve, cooling P5",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "40727": {
+        "default": 1.0,
         "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
         "name": "cooling-connected-climate-system-1-40727",
         "size": "u8",
         "title": "Cooling connected, climate system 1",
         "write": true
     },
     "40732": {
         "default": 0.0,
@@ -6499,14 +6804,47 @@
         "max": 1.0,
         "min": 0.0,
         "name": "acs-40732",
         "size": "u8",
         "title": "ACS",
         "write": true
     },
+    "40737": {
+        "default": 30.0,
+        "factor": 1,
+        "max": 180.0,
+        "min": 0.0,
+        "name": "period-time-cooling-40737",
+        "size": "u8",
+        "title": "Period time cooling",
+        "unit": "min",
+        "write": true
+    },
+    "40739": {
+        "default": 3.0,
+        "factor": 1,
+        "max": 10.0,
+        "min": 3.0,
+        "name": "cooling-delta-temp-20degc-40739",
+        "size": "s8",
+        "title": "Cooling delta temp. 20\u00b0C",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40740": {
+        "default": 6.0,
+        "factor": 1,
+        "max": 20.0,
+        "min": 3.0,
+        "name": "cooling-delta-temp-40degc-40740",
+        "size": "s8",
+        "title": "Cooling delta temp. 40\u00b0C",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "40748": {
         "default": 0.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "operating-mode-charge-pump-climate-system-2-40748",
         "size": "u8",
@@ -6562,15 +6900,15 @@
         "size": "u8",
         "title": "Heating (SG Ready)",
         "write": true
     },
     "40768": {
         "default": 0.0,
         "factor": 1,
-        "max": 59.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "input-aux5-40768",
         "size": "u8",
         "title": "Input AUX5",
         "write": true
     },
     "40783": {
@@ -6669,14 +7007,34 @@
         "max": 1.0,
         "min": 0.0,
         "name": "operating-mode-circulation-pump-hot-water-heat-pump-1-40800",
         "size": "u8",
         "title": "Operating mode circulation pump hot water heat pump 1",
         "write": true
     },
+    "40832": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "operating-mode-circulation-pump-cooling-heat-pump-2-40832",
+        "size": "u8",
+        "title": "Operating mode circulation pump cooling heat pump 2",
+        "write": true
+    },
+    "40833": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "operating-mode-circulation-pump-cooling-heat-pump-1-40833",
+        "size": "u8",
+        "title": "Operating mode circulation pump cooling heat pump 1",
+        "write": true
+    },
     "40841": {
         "default": 30.0,
         "factor": 1,
         "max": 100.0,
         "min": 1.0,
         "name": "speed-circulation-pump-waiting-mode-heat-pump-2-40841",
         "size": "u8",
@@ -7062,14 +7420,67 @@
         "max": 60.0,
         "min": 0.0,
         "name": "room-sensor-factor-climate-system-5-40960",
         "size": "u8",
         "title": "Room sensor factor climate system 5",
         "write": true
     },
+    "40968": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 9.0,
+        "min": 0.0,
+        "name": "cooling-curve-climate-system-1-40968",
+        "size": "s8",
+        "title": "Cooling curve climate system 1",
+        "write": true
+    },
+    "40976": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 10.0,
+        "min": -10.0,
+        "name": "cooling-offset-climate-system-1-40976",
+        "size": "s8",
+        "title": "Cooling offset climate system 1",
+        "write": true
+    },
+    "40977": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p4-40977",
+        "size": "s8",
+        "title": "Own curve, cooling P4",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40978": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p2-40978",
+        "size": "s8",
+        "title": "Own curve, cooling P2",
+        "unit": "\u00b0C",
+        "write": true
+    },
+    "40979": {
+        "default": 20.0,
+        "factor": 1,
+        "max": 40.0,
+        "min": 7.0,
+        "name": "own-curve-cooling-p1-40979",
+        "size": "s8",
+        "title": "Own curve, cooling P1",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "40981": {
         "default": 300.0,
         "factor": 1,
         "max": 3000.0,
         "min": 300.0,
         "name": "current-transformer-ratio-40981",
         "size": "u16",
@@ -9080,15 +9491,15 @@
         "size": "u8",
         "title": "Time between filter replacement",
         "write": true
     },
     "42741": {
         "default": 0.0,
         "factor": 1,
-        "max": 59.0,
+        "max": 65.0,
         "min": 0.0,
         "name": "aux-from-modbus-42741",
         "size": "u8",
         "title": "AUX from Modbus",
         "write": true
     },
     "42742": {
@@ -9309,14 +9720,24 @@
         "max": 10.0,
         "min": 1.0,
         "name": "factor-43034",
         "size": "u8",
         "title": "Factor",
         "write": true
     },
+    "43037": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "activate-43037",
+        "size": "u8",
+        "title": "Activate",
+        "write": true
+    },
     "43059": {
         "default": 0.0,
         "factor": 1,
         "max": 7.0,
         "min": 0.0,
         "name": "additional-heat-step-emergency-mode-43059",
         "size": "u8",
@@ -9329,14 +9750,34 @@
         "max": 1.0,
         "min": 0.0,
         "name": "heating-auto-43060",
         "size": "u8",
         "title": "Heating, auto",
         "write": true
     },
+    "43061": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "cooling-auto-43061",
+        "size": "u8",
+        "title": "Cooling, auto",
+        "write": true
+    },
+    "43066": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "activate-43066",
+        "size": "u8",
+        "title": "Activate",
+        "write": true
+    },
     "43067": {
         "default": 0.0,
         "factor": 1,
         "max": 127.0,
         "min": 0.0,
         "name": "active-days-43067",
         "size": "u8",
@@ -9444,14 +9885,25 @@
     "43098": {
         "factor": 1,
         "name": "show-indoor-temperature-43098",
         "size": "u8",
         "title": "Show indoor temperature",
         "write": true
     },
+    "43103": {
+        "default": 60.0,
+        "factor": 1,
+        "max": 60.0,
+        "min": 1.0,
+        "name": "operating-time-43103",
+        "size": "s8",
+        "title": "Operating time",
+        "unit": "min",
+        "write": true
+    },
     "43233": {
         "default": 1.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "audio-signal-on-alarm-43233",
         "size": "u8",
@@ -9518,14 +9970,24 @@
         "max": 1.0,
         "min": 0.0,
         "name": "start-fan-de-icing-eb101-43252",
         "size": "s8",
         "title": "Start fan de-icing (EB101)",
         "write": true
     },
+    "43253": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "start-fan-de-icing-eb102-43253",
+        "size": "s8",
+        "title": "Start fan de-icing (EB102)",
+        "write": true
+    },
     "43987": {
         "default": 0.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "disable-emergency-restart-gp1-43987",
         "size": "u8",
@@ -9548,14 +10010,66 @@
         "max": 10000.0,
         "min": 1.0,
         "name": "external-energy-meter-2-pulse-per-kwh-44019",
         "size": "u16",
         "title": "External energy meter 2 pulse per kWh",
         "write": true
     },
+    "44025": {
+        "factor": 1,
+        "name": "start-time-hwc-period-1-44025",
+        "size": "u16",
+        "title": "Start time HWC period 1",
+        "write": true
+    },
+    "44027": {
+        "factor": 1,
+        "name": "start-time-hwc-period-2-44027",
+        "size": "u16",
+        "title": "Start time HWC period 2",
+        "write": true
+    },
+    "44029": {
+        "factor": 1,
+        "name": "start-time-hwc-period-3-44029",
+        "size": "u16",
+        "title": "Start time HWC period 3",
+        "write": true
+    },
+    "44031": {
+        "factor": 1,
+        "name": "stop-time-hwc-period-1-44031",
+        "size": "u16",
+        "title": "Stop time HWC period 1",
+        "write": true
+    },
+    "44033": {
+        "factor": 1,
+        "name": "stop-time-hwc-period-2-44033",
+        "size": "u16",
+        "title": "Stop time HWC period 2",
+        "write": true
+    },
+    "44035": {
+        "factor": 1,
+        "name": "stop-time-hwc-period-3-44035",
+        "size": "u16",
+        "title": "Stop time HWC period 3",
+        "write": true
+    },
+    "44065": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "shunted-brine-accessory-44065",
+        "size": "u8",
+        "title": "Shunted brine, accessory",
+        "write": true
+    },
     "44068": {
         "default": 20.0,
         "factor": 1,
         "max": 30.0,
         "min": 0.0,
         "name": "shunted-brine-max-temp-44068",
         "size": "u8",
@@ -9903,9 +10417,19 @@
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "disable-emergency-restart-gp1-45026",
         "size": "u8",
         "title": "Disable emergency restart GP1",
         "write": true
+    },
+    "45102": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "heat-pump-test-silent-mode-eb101-eb102-45102",
+        "size": "u8",
+        "title": "Heat pump test - Silent mode (EB101/EB102)",
+        "write": true
     }
 }
```

### Comparing `nibe-2.2.0/nibe/data/vvm225_vvm320_vvm325.json` & `nibe-2.3.0/nibe/data/vvm225_vvm320_vvm325.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/data/vvm310_vvm500.json` & `nibe-2.3.0/nibe/data/vvm310_vvm500.json`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/event_server.py` & `nibe-2.3.0/nibe/event_server.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/exceptions.py` & `nibe-2.3.0/nibe/exceptions.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/heatpump.py` & `nibe-2.3.0/nibe/heatpump.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe/parsers.py` & `nibe-2.3.0/nibe/parsers.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/nibe.egg-info/PKG-INFO` & `nibe-2.3.0/nibe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibe
-Version: 2.2.0
+Version: 2.3.0
 Summary: Nibe heatpump communication library
 Home-page: https://github.com/yozik04/nibe
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/nibe/issues
 Keywords: nibe modbus library nibegw
```

### Comparing `nibe-2.2.0/nibe.egg-info/SOURCES.txt` & `nibe-2.3.0/nibe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/setup.cfg` & `nibe-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/tests/test_coil.py` & `nibe-2.3.0/tests/test_coil.py`

 * *Files identical despite different names*

### Comparing `nibe-2.2.0/tests/test_heatpump.py` & `nibe-2.3.0/tests/test_heatpump.py`

 * *Files identical despite different names*

