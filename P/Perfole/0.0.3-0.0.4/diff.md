# Comparing `tmp/Perfole-0.0.3.tar.gz` & `tmp/Perfole-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Perfole-0.0.3.tar", last modified: Mon Jul 10 12:43:42 2023, max compression
+gzip compressed data, was "Perfole-0.0.4.tar", last modified: Mon Jul 10 13:14:09 2023, max compression
```

## Comparing `Perfole-0.0.3.tar` & `Perfole-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:43:42.263121 Perfole-0.0.3/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:43:42.262989 Perfole-0.0.3/PKG-INFO
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:43:42.261525 Perfole-0.0.3/Perfole/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12927 2023-07-10 11:40:47.000000 Perfole-0.0.3/Perfole/Perfole.py
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.3/Perfole/__init__.py
-drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 12:43:42.262432 Perfole-0.0.3/Perfole.egg-info/
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/PKG-INFO
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/SOURCES.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/dependency_links.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/requires.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-10 12:43:42.000000 Perfole-0.0.3/Perfole.egg-info/top_level.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1183 2023-07-10 11:07:54.000000 Perfole-0.0.3/README.md
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.3/license.txt
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-10 12:43:42.263184 Perfole-0.0.3/setup.cfg
--rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      501 2023-07-10 12:43:16.000000 Perfole-0.0.3/setup.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 13:14:09.005096 Perfole-0.0.4/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 13:14:09.004964 Perfole-0.0.4/PKG-INFO
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 13:14:09.003996 Perfole-0.0.4/Perfole/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)    12896 2023-07-10 13:13:47.000000 Perfole-0.0.4/Perfole/Perfole.py
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-07 16:50:05.000000 Perfole-0.0.4/Perfole/__init__.py
+drwxr-xr-x   0 smiljanaradlovic   (502) staff       (20)        0 2023-07-10 13:14:09.004736 Perfole-0.0.4/Perfole.egg-info/
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1374 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/PKG-INFO
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      223 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/SOURCES.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        1 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/dependency_links.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        9 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/requires.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)        8 2023-07-10 13:14:08.000000 Perfole-0.0.4/Perfole.egg-info/top_level.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     1183 2023-07-10 11:07:54.000000 Perfole-0.0.4/README.md
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)     4528 2023-07-10 08:04:58.000000 Perfole-0.0.4/license.txt
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)       38 2023-07-10 13:14:09.005138 Perfole-0.0.4/setup.cfg
+-rw-r--r--   0 smiljanaradlovic   (502) staff       (20)      501 2023-07-10 13:14:03.000000 Perfole-0.0.4/setup.py
```

### Comparing `Perfole-0.0.3/PKG-INFO` & `Perfole-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.3
+Version: 0.0.4
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `Perfole-0.0.3/Perfole/Perfole.py` & `Perfole-0.0.4/Perfole/Perfole.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                     uniqueIdentifier=threading.current_thread().name
                 PERFORMANCE_TEST.writeToActionsBeforeCalculation("end", name, additionalInfo, uniqueIdentifier)
         except:
             PERFORMANCE_TEST.clearResult()
     
     @staticmethod
     def publishResult(apiKey):
-        url = 'https://xwycqvx020.execute-api.us-east-1.amazonaws.com/library/execution'
+        url = 'https://api.perfole.com/library/execution'
 
         executionResult = ExecutionPrivate(machineName = PERFORMANCE_TEST.argumentsValue['machineName'],
                                            startTime = PERFORMANCE_TEST.execution_start_time,
                                            publishTime = PERFORMANCE_TEST.execution_end_time,
                                            duration = PERFORMANCE_TEST.execution_end_time - PERFORMANCE_TEST.execution_start_time,
                                            actions = PERFORMANCE_TEST.calculatedActions,
                                            versionValue = PERFORMANCE_TEST.argumentsValue['appVersion'])
```

### Comparing `Perfole-0.0.3/Perfole.egg-info/PKG-INFO` & `Perfole-0.0.4/Perfole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Perfole
-Version: 0.0.3
+Version: 0.0.4
 Summary: Measure performance
 Author: breeze-testing
 License: license.txt
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `Perfole-0.0.3/README.md` & `Perfole-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Perfole-0.0.3/license.txt` & `Perfole-0.0.4/license.txt`

 * *Files identical despite different names*

