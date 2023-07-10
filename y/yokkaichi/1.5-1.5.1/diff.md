# Comparing `tmp/yokkaichi-1.5.tar.gz` & `tmp/yokkaichi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.5.tar", last modified: Sun Jul  9 20:58:56 2023, max compression
+gzip compressed data, was "yokkaichi-1.5.1.tar", last modified: Sun Jul  9 21:04:35 2023, max compression
```

## Comparing `yokkaichi-1.5.tar` & `yokkaichi-1.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.856030 yokkaichi-1.5/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.5/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2997 2023-07-09 20:58:56.856030 yokkaichi-1.5/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2205 2023-05-24 18:11:37.000000 yokkaichi-1.5/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       57 2023-05-24 14:00:39.000000 yokkaichi-1.5/pyproject.toml
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-09 20:58:56.856030 yokkaichi-1.5/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1626 2023-07-09 20:54:16.000000 yokkaichi-1.5/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2923 2023-05-24 14:00:39.000000 yokkaichi-1.5/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     5939 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       20 2023-07-09 20:55:21.000000 yokkaichi-1.5/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     9027 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1609 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/args_to_cfg.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     4364 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/config_loader.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/constants/
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5/yokkaichi/constants/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.5/yokkaichi/constants/rich_console.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/enums/
--rw-r--r--   0 krystian  (1000) krystian  (1000)       98 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/enums/MasscanMethods.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       89 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/enums/Platforms.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/enums/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1168 2023-05-24 14:00:39.000000 yokkaichi-1.5/yokkaichi/port_parser.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/structs/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1015 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/structs/CFG.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5/yokkaichi/structs/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2997 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      593 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       81 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.5.1/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2949 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2205 2023-05-24 18:11:37.000000 yokkaichi-1.5.1/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       57 2023-05-24 14:00:39.000000 yokkaichi-1.5.1/pyproject.toml
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1577 2023-07-09 21:03:26.000000 yokkaichi-1.5.1/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2923 2023-05-24 14:00:39.000000 yokkaichi-1.5.1/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     5939 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-07-09 21:03:26.000000 yokkaichi-1.5.1/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     9027 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1609 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/args_to_cfg.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4364 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/config_loader.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/yokkaichi/constants/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5.1/yokkaichi/constants/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.5.1/yokkaichi/constants/rich_console.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/yokkaichi/enums/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       98 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/enums/MasscanMethods.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       89 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/enums/Platforms.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/enums/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1168 2023-05-24 14:00:39.000000 yokkaichi-1.5.1/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/yokkaichi/structs/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1015 2023-07-09 20:54:16.000000 yokkaichi-1.5.1/yokkaichi/structs/CFG.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5.1/yokkaichi/structs/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 21:04:35.092333 yokkaichi-1.5.1/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2949 2023-07-09 21:04:35.000000 yokkaichi-1.5.1/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      593 2023-07-09 21:04:35.000000 yokkaichi-1.5.1/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-09 21:04:35.000000 yokkaichi-1.5.1/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       81 2023-07-09 21:04:35.000000 yokkaichi-1.5.1/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-07-09 21:04:35.000000 yokkaichi-1.5.1/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.5/LICENSE.txt` & `yokkaichi-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/PKG-INFO` & `yokkaichi-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.5
+Version: 1.5.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `yokkaichi-1.5/README.md` & `yokkaichi-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/setup.py` & `yokkaichi-1.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     ],
     extras_require={"testing": ["pytest"]},
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=[
```

### Comparing `yokkaichi-1.5/yokkaichi/MasscanScan.py` & `yokkaichi-1.5.1/yokkaichi/MasscanScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/yokkaichi/ServerScan.py` & `yokkaichi-1.5.1/yokkaichi/ServerScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/yokkaichi/__main__.py` & `yokkaichi-1.5.1/yokkaichi/__main__.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/yokkaichi/args_to_cfg.py` & `yokkaichi-1.5.1/yokkaichi/args_to_cfg.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/yokkaichi/config_loader.py` & `yokkaichi-1.5.1/yokkaichi/config_loader.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/yokkaichi/port_parser.py` & `yokkaichi-1.5.1/yokkaichi/port_parser.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/yokkaichi/structs/CFG.py` & `yokkaichi-1.5.1/yokkaichi/structs/CFG.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.5.1/yokkaichi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.5
+Version: 1.5.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `yokkaichi-1.5/yokkaichi.egg-info/SOURCES.txt` & `yokkaichi-1.5.1/yokkaichi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

