# Comparing `tmp/buildlackey-1.0.0.tar.gz` & `tmp/buildlackey-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildlackey-1.0.0.tar", last modified: Sat Jul  8 23:46:33 2023, max compression
+gzip compressed data, was "buildlackey-1.1.0.tar", last modified: Mon Jul 10 20:01:00 2023, max compression
```

## Comparing `buildlackey-1.0.0.tar` & `buildlackey-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.007748 buildlackey-1.0.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-1.0.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43935 2023-07-08 23:46:33.007618 buildlackey-1.0.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3755 2023-05-14 23:46:48.000000 buildlackey-1.0.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.005318 buildlackey-1.0.0/buildlackey/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4637 2023-07-08 20:51:40.000000 buildlackey-1.0.0/buildlackey/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1959 2023-07-07 20:47:53.000000 buildlackey-1.0.0/buildlackey/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      392 2023-07-06 20:28:44.000000 buildlackey-1.0.0/buildlackey/PythonWarnings.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       44 2023-07-05 19:22:15.000000 buildlackey-1.0.0/buildlackey/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-07-07 19:47:36.000000 buildlackey-1.0.0/buildlackey/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.006842 buildlackey-1.0.0/buildlackey/commands/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1257 2023-07-08 00:16:15.000000 buildlackey-1.0.0/buildlackey/commands/Cleanup.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1421 2023-07-08 00:23:30.000000 buildlackey-1.0.0/buildlackey/commands/Package.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      440 2023-07-08 00:47:04.000000 buildlackey-1.0.0/buildlackey/commands/ProductionPush.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      631 2023-07-07 20:48:29.000000 buildlackey-1.0.0/buildlackey/commands/RunMypy.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2128 2023-07-07 20:50:29.000000 buildlackey-1.0.0/buildlackey/commands/RunTests.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-06 19:54:27.000000 buildlackey-1.0.0/buildlackey/commands/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.007178 buildlackey-1.0.0/buildlackey/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-1.0.0/buildlackey/exceptions/ProjectNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-1.0.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-1.0.0/buildlackey/exceptions/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.007359 buildlackey-1.0.0/buildlackey/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-1.0.0/buildlackey/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-1.0.0/buildlackey/resources/loggingConfiguration.json
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-08 23:46:33.006140 buildlackey-1.0.0/buildlackey.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43935 2023-07-08 23:46:32.000000 buildlackey-1.0.0/buildlackey.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      788 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      217 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-07-08 23:46:33.000000 buildlackey-1.0.0/buildlackey.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-07-08 23:46:33.007786 buildlackey-1.0.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1345 2023-07-08 19:41:35.000000 buildlackey-1.0.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-10 20:01:00.331040 buildlackey-1.1.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-1.1.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43935 2023-07-10 20:01:00.330912 buildlackey-1.1.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3755 2023-05-14 23:46:48.000000 buildlackey-1.1.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-10 20:01:00.328584 buildlackey-1.1.0/buildlackey/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4849 2023-07-10 14:54:54.000000 buildlackey-1.1.0/buildlackey/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1923 2023-07-09 20:37:31.000000 buildlackey-1.1.0/buildlackey/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      392 2023-07-06 20:28:44.000000 buildlackey-1.1.0/buildlackey/PythonWarnings.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       44 2023-07-05 19:22:15.000000 buildlackey-1.1.0/buildlackey/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-07-09 20:19:19.000000 buildlackey-1.1.0/buildlackey/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-10 20:01:00.330141 buildlackey-1.1.0/buildlackey/commands/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1257 2023-07-08 00:16:15.000000 buildlackey-1.1.0/buildlackey/commands/Cleanup.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1421 2023-07-08 00:23:30.000000 buildlackey-1.1.0/buildlackey/commands/Package.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      440 2023-07-08 00:47:04.000000 buildlackey-1.1.0/buildlackey/commands/ProductionPush.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      631 2023-07-07 20:48:29.000000 buildlackey-1.1.0/buildlackey/commands/RunMypy.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2203 2023-07-10 14:53:11.000000 buildlackey-1.1.0/buildlackey/commands/RunTests.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-06 19:54:27.000000 buildlackey-1.1.0/buildlackey/commands/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-10 20:01:00.330480 buildlackey-1.1.0/buildlackey/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-1.1.0/buildlackey/exceptions/ProjectNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-1.1.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-1.1.0/buildlackey/exceptions/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-10 20:01:00.330690 buildlackey-1.1.0/buildlackey/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-1.1.0/buildlackey/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-1.1.0/buildlackey/resources/loggingConfiguration.json
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-10 20:01:00.329381 buildlackey-1.1.0/buildlackey.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43935 2023-07-10 20:01:00.000000 buildlackey-1.1.0/buildlackey.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      788 2023-07-10 20:01:00.000000 buildlackey-1.1.0/buildlackey.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-07-10 20:01:00.000000 buildlackey-1.1.0/buildlackey.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      217 2023-07-10 20:01:00.000000 buildlackey-1.1.0/buildlackey.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-07-10 20:01:00.000000 buildlackey-1.1.0/buildlackey.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-07-10 20:01:00.000000 buildlackey-1.1.0/buildlackey.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-07-10 20:01:00.331076 buildlackey-1.1.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1345 2023-07-08 19:41:35.000000 buildlackey-1.1.0/setup.py
```

### Comparing `buildlackey-1.0.0/LICENSE` & `buildlackey-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildlackey-1.0.0/PKG-INFO` & `buildlackey-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 1.0.0
+Version: 1.1.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `buildlackey-1.0.0/README.md` & `buildlackey-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `buildlackey-1.0.0/buildlackey/Commands.py` & `buildlackey-1.1.0/buildlackey/Commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,18 +70,20 @@
     \b
     Environment Variables
 
         PROJECTS_BASE -  The local directory where the python projects are based
         PROJECT       -  The name of the project;  It should be a directory name
 
     \b
-    By default, buildlackey runs the module named tests.TestAll
+    \b
+    However, if one or the other is not defined the command assumes it is executing in a CI
+    environment and thus the current working directory is the project base directory.
 
+    By default, buildlackey runs the module named tests.TestAll
     """
-
     setUpLogging()
     runTests: RunTests = RunTests(inputFile=input_file, warning=warning)
 
     runTests.execute()
 
 
 @command
@@ -149,10 +151,10 @@
     """
     productionPush: ProductionPush = ProductionPush()
     productionPush.execute()
 
 
 if __name__ == "__main__":
 
-    runtests()
+    runtests(['-i', 'tests/unittest.txt'])
     # cleanup(['--help'])
     # deploy(['--help'])
```

### Comparing `buildlackey-1.0.0/buildlackey/Environment.py` & `buildlackey-1.1.0/buildlackey/Environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from os import chdir
 
 from os import environ as osEnvironment
 from os import sep as osSep
 
 from subprocess import run as subProcessRun
 
-from click import ClickException
 from click import clear
 from click import secho
 
 
 class Environment:
     """
 
@@ -28,19 +27,19 @@
 
         self._projectsBase:     str = ''
         self._projectDirectory: str = ''
 
         try:
             self._projectsBase = osEnvironment[Environment.ENV_PROJECTS_BASE]
         except KeyError:
-            raise ClickException('Project Base not set')
+            self.ebLogger.info(f'Project Base not set')
         try:
             self._projectDirectory = osEnvironment[Environment.ENV_PROJECT]
         except KeyError:
-            raise ClickException(f'Project Directory not set')
+            self.ebLogger.info(f'Project Directory not set')
 
         clear()
         secho(f'projects_base={self._projectsBase}', color=True, reverse=True)
         secho(f'project={self._projectDirectory}', color=True, reverse=True)
         secho('')
 
     @property
```

### Comparing `buildlackey-1.0.0/buildlackey/commands/Cleanup.py` & `buildlackey-1.1.0/buildlackey/commands/Cleanup.py`

 * *Files identical despite different names*

### Comparing `buildlackey-1.0.0/buildlackey/commands/Package.py` & `buildlackey-1.1.0/buildlackey/commands/Package.py`

 * *Files identical despite different names*

### Comparing `buildlackey-1.0.0/buildlackey/commands/RunMypy.py` & `buildlackey-1.1.0/buildlackey/commands/RunMypy.py`

 * *Files identical despite different names*

### Comparing `buildlackey-1.0.0/buildlackey/commands/RunTests.py` & `buildlackey-1.1.0/buildlackey/commands/RunTests.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 class RunTests(Environment):
     
     def __init__(self, inputFile: str, warning: str):
         super().__init__()
 
         self.logger: Logger = getLogger(__name__)
 
-        self._inputFile: str            = inputFile
+        self._inputFile: str = inputFile
         if warning is None:
-            self._warning:   PythonWarnings = PythonWarnings.IGNORE
+            self._warning: PythonWarnings = PythonWarnings.IGNORE
         else:
             try:
                 self._warning = PythonWarnings(warning)
             except ValueError:
                 raise ClickException(f'Invalid warning type: {warning}')
 
     def execute(self):
 
-        self._changeToProjectRoot()
+        if self.validProjectsBase is True and self.validProjectDirectory() is True:
+            self._changeToProjectRoot()
 
         if self._inputFile is None:
             defaultCmd: str = f'{PYTHON_CLI} -W{self._warning.value} -m tests.TestAll'
             secho(f'{defaultCmd}')
             status: int = self._runCommand(command=f'python3 -W{self._warning.value} -m {DEFAULT_MODULE_NAME}')
             secho(f'{status=}')
         else:
```

### Comparing `buildlackey-1.0.0/buildlackey/resources/loggingConfiguration.json` & `buildlackey-1.1.0/buildlackey/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `buildlackey-1.0.0/buildlackey.egg-info/PKG-INFO` & `buildlackey-1.1.0/buildlackey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 1.0.0
+Version: 1.1.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `buildlackey-1.0.0/buildlackey.egg-info/SOURCES.txt` & `buildlackey-1.1.0/buildlackey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildlackey-1.0.0/setup.py` & `buildlackey-1.1.0/setup.py`

 * *Files identical despite different names*

