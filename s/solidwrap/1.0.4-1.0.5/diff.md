# Comparing `tmp/solidwrap-1.0.4.tar.gz` & `tmp/solidwrap-1.0.5.tar.gz`

## Comparing `solidwrap-1.0.4.tar` & `solidwrap-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 solidwrap-1.0.4/info/API Reference.rst
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/__init__.py
--rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/solidwrap.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/extensions/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/extensions/extensions.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/utilities/__init__.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/utilities/utilities.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.4/tests/test.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 solidwrap-1.0.4/../README.rst
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 solidwrap-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 solidwrap-1.0.5/info/API Reference.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/__init__.py
+-rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/solidwrap.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/extensions/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/extensions/extensions.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/utilities/__init__.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 solidwrap-1.0.5/solidwrap/utilities/utilities.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.5/tests/test.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 solidwrap-1.0.5/../README.rst
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 solidwrap-1.0.5/PKG-INFO
```

### Comparing `solidwrap-1.0.4/info/API Reference.rst` & `solidwrap-1.0.5/info/API Reference.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.4/solidwrap/solidwrap.py` & `solidwrap-1.0.5/solidwrap/solidwrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         # print(f"{utility.FileCount}")
 
     def checkin(self, filepath: Filepath, message: str="SolidWrap Automated Check In"):
         '''Checks in a file to the PDM Vault.'''
         print(f"Check In: {filepath.name}")
 
         # Get PDM-API objects
-        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
         file = directory.GetFile(filepath.name)                         # IEdmFile5
 
         # Execute PDM-API method
         if file.IsLocked:                           # if file is not checked in...
             file.UnlockFile(0, message)             # check in file
         else:
             print(f"File is already checked in!")   # ...else terminal warning
@@ -337,44 +337,44 @@
         # file        = directory.GetFile(filepath.name)                  # IEdmFile
         # file.ChangeState(state, folder_id, message, 0, 0)
 
     def get_revision(self, filepath: Filepath) -> str:
         '''Returns current revision of the target file.'''
         
         # Get PDM-API objects
-        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
         file = directory.GetFile(filepath.name)                         # IEdmFile5
         return file.CurrentRevision
     
     def is_checked_out(self, filepath: Filepath) -> bool:
         '''Returns checkout state of the target file.'''
         
         # Get PDM-API objects
-        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
         file = directory.GetFile(filepath.name)                         # IEdmFile5
         
         if file.IsLocked:
             return True
         else:
             return False
 
     def get_size(self, filepath: Filepath) -> int:
-        '''Returns size of the target file (MB).'''
+        '''Returns size of the target file (KB).'''
 
         # Get PDM-API objects
         directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
         file = directory.GetFile(filepath.name)                        # IEdmFile
         return int(file.GetLocalFileSize2(directory.ID)/1000)
 
     # WIP
     def get_pdm_state(self, filepath: Filepath) -> str:
         '''Returns PDM state of the target file.'''
         
         # Get PDM-API objects
-        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
         file = directory.GetFile(filepath.name)                         # IEdmFile5
         return file.CurrentState.GetFirstTransitionPosition()
 
 
 # --------------
 # IV. Singletons
 # --------------
```

### Comparing `solidwrap-1.0.4/solidwrap/utilities/utilities.py` & `solidwrap-1.0.5/solidwrap/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.4/tests/test.py` & `solidwrap-1.0.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.4/pyproject.toml` & `solidwrap-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solidwrap"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Sean Yeatts" },
 ]
 license = {text = "MIT License"}
 description = "Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
 readme = "../README.rst"
 requires-python = ">=3.7"
```

### Comparing `solidwrap-1.0.4/../README.rst` & `solidwrap-1.0.5/../README.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.4/PKG-INFO` & `solidwrap-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidwrap
-Version: 1.0.4
+Version: 1.0.5
 Summary: Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 Project-URL: Homepage, https://github.com/SeanYeatts/SolidWrap/tree/main
 Project-URL: Bug Tracker, https://github.com/users/SeanYeatts/projects/6/views/1
 Author: Sean Yeatts
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

