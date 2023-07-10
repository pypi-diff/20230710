# Comparing `tmp/openmodule_commands-11.1.1.tar.gz` & `tmp/openmodule_commands-12.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-11.1.1.tar", last modified: Tue Jun 13 12:13:27 2023, max compression
+gzip compressed data, was "openmodule_commands-12.0.0rc0.tar", last modified: Mon Jul 10 13:47:18 2023, max compression
```

## Comparing `openmodule_commands-11.1.1.tar` & `openmodule_commands-12.0.0rc0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:13:27.467871 openmodule_commands-11.1.1/
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6520 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      618 2023-06-13 12:13:27.467871 openmodule_commands-11.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-13 12:13:15.000000 openmodule_commands-11.1.1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:13:27.467871 openmodule_commands-11.1.1/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-13 12:13:27.000000 openmodule_commands-11.1.1/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-13 12:13:27.467871 openmodule_commands-11.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-13 12:13:15.000000 openmodule_commands-11.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-13 12:13:15.000000 openmodule_commands-11.1.1/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:47:18.623892 openmodule_commands-12.0.0rc0/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     7579 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-10 13:47:18.623892 openmodule_commands-12.0.0rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-07-10 13:47:05.000000 openmodule_commands-12.0.0rc0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:47:18.623892 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-10 13:47:18.000000 openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-07-10 13:47:18.623892 openmodule_commands-12.0.0rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-10 13:47:05.000000 openmodule_commands-12.0.0rc0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-07-10 13:47:05.000000 openmodule_commands-12.0.0rc0/translate.py
```

### Comparing `openmodule_commands-11.1.1/ChangeLog` & `openmodule_commands-12.0.0rc0/ChangeLog`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,76 @@
 CHANGES
 =======
 
+v12.0.0.rc0
+-----------
+
+* Removed parking\_area\_id from AccessCheckAccess changed gate permission check in AccessService to new behavior
+* removed Gate and GateType (now from settings models)
+* fixed testcases and removed backend (deprecated in v11)
+* newer settings-models
+* settings models update
+* made gate\_control/day\_mode have no scope
+* schedule exports utility
+* SettingsProvider docs
+* SettingsProvider docs
+* added settings\_models requirement, marking Test\* classes that are not tests with \_\_test\_\_ = False
+* AAAAAAAABBBBBBBBBBBBBBMerge branch 'master' into DEV-5415
+* [skip ci] Broken until settings\_model pip package is fixed. Removed deprecated features for v12. Using settings\_models in SettingsProvider
+
 v11.1.1
 -------
 
 * added state parameter to VehicleBuilder.lpr function
 
 v11.1.0
 -------
 
 * csv export library, databox upload and schedule library tips
+
+v11.1.0.rc5
+-----------
+
+* again no language set in testing
+
+v11.1.0.rc4
+-----------
+
+* arivo-schedule in public pip
+* use temporary arivo-schedule package
+
+v11.1.0.rc3
+-----------
+
+* changed docs and requirements for schedule library until its a pip package
+
+v11.1.0.rc2
+-----------
+
+* added fork of schedule package
+
+v11.1.0.rc1
+-----------
+
+* databox upload now can have dst as folder (endswith "/")
+
+v11.1.0.rc0
+-----------
+
+* fixed testcase
+* small changes in csv export and databox upload adding more testcases docs
+* move files instead of copy
+* readme
+* util for databox upload
+* removing language dependency
+* removing ="asdf" for strings
+* added decimal separator support for english
+* some testcases for csv exporter, incorrect default value + static missing [skip ci]
+* fixed comment
+* added csv\_export library (no testcases)
 * removed mock rpcs from schema
 
 v11.0.3
 -------
 
 * Fixed typo, added compute\_id as label to all metrics, convert all label values to string
 * touch to get rid of skip ci on my commit
@@ -142,32 +199,7 @@
 * drop support for python 3.7
 * cleanup and docs
 * testcases for the new test method
 * better logging for rpc requests, and added a function to the test framework to receive rpc responses async
 * moved config yaml path guesser to separate function, removed GUID again because its not a great idea after all
 * reduced warnings in the testcases
 * GUID type and rpc server changes to better support all pydantic models, in this case Union Types. DEVICE-891
-* fixes an issue in rpc server logging, and adds more debug log output
-
-v7.0.0
-------
-
-* # OpenModule \* rpc client resource filter only applies if resource in message \* all zmq messages now use utc timestamps
-
-v6.1.6
-------
-
-* 6.1.6
-
-v6.1.5
-------
-
-* bug fix test cases
-* rpc-client refactor + kv\_redis
-* rpc-client
-* added default zmq.LINGER for context to be more compatible with OMv1 socket creation
-* wait for rpc assertion
-
-v6.1.4
-------
-
-* Resource Filter in RPC Server + removed urljoin from ApiMocker
```

### Comparing `openmodule_commands-11.1.1/PKG-INFO` & `openmodule_commands-12.0.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 11.1.1
+Version: 12.0.0rc0
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.1/__init__.py` & `openmodule_commands-12.0.0rc0/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.1/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-12.0.0rc0/openmodule_commands.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 11.1.1
+Version: 12.0.0rc0
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.1/setup.cfg` & `openmodule_commands-12.0.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.1/setup.py` & `openmodule_commands-12.0.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.1/translate.py` & `openmodule_commands-12.0.0rc0/translate.py`

 * *Files identical despite different names*

