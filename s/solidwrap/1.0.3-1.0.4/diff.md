# Comparing `tmp/solidwrap-1.0.3.tar.gz` & `tmp/solidwrap-1.0.4.tar.gz`

## Comparing `solidwrap-1.0.3.tar` & `solidwrap-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 solidwrap-1.0.3/info/API Reference.rst
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/__init__.py
--rw-r--r--   0        0        0    13939 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/solidwrap.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/extensions/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/extensions/extensions.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/utilities/__init__.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 solidwrap-1.0.3/solidwrap/utilities/utilities.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.3/tests/test.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 solidwrap-1.0.3/../README.rst
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 solidwrap-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     8008 2020-02-02 00:00:00.000000 solidwrap-1.0.4/info/API Reference.rst
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/__init__.py
+-rw-r--r--   0        0        0    15563 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/solidwrap.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/extensions/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/extensions/extensions.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/utilities/__init__.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 solidwrap-1.0.4/solidwrap/utilities/utilities.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 solidwrap-1.0.4/tests/test.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 solidwrap-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 solidwrap-1.0.4/../README.rst
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 solidwrap-1.0.4/PKG-INFO
```

### Comparing `solidwrap-1.0.3/info/API Reference.rst` & `solidwrap-1.0.4/info/API Reference.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 API Reference ( SolidWrap )
 ===========================
 
 *Copyright (c) 2023 Sean Yeatts. All rights reserved.*
 
 The SolidWorks API ( `SW-API <https://help.solidworks.com/2019/English/SolidWorks/sldworks/c_solidworks_api.htm?verRedirect=1>`_ ) and PDM API ( `PDM-API <https://help.solidworks.com/2019/English/api/epdmapi/Welcome-epdmapi.html?id=2a67aaceb6984695a5ce8a75121853f3#Pg0>`_ ) are built on the Component Object Model ( `COM <https://learn.microsoft.com/en-us/windows/win32/com/component-object-model--com--portal>`_ ) to provide an interface with SolidWorks applications. They do not, however, have direct support for Python. SolidWrap leverages its own implementation of the COM pipeline to provide a streamlined Pythonic interface with SW-API and PDM-API.
 
+----
+
 The core of SolidWrap relies on two objects: ``solidworks`` and ``vault``. These are treated as singletons; they come pre-instanced by the module and should not be manually created by the user. Most interactions with SolidWrap should flow through these objects.
 
 See the Appendix for an overview of the helper classes ( ``Filepath`` & ``Model`` ) that are embedded in many of the SolidWrap class methods.
 
-*NOTE: Items with a 'WIP' label are in development and are not garaunteed to function appropriately.*
+**NOTE : Items labelled 'WIP' are in development and are not guaranteed to function as expected.**
+
+----
 
 ``solidworks`` ( object )
 -------------------------
 The core object of the API. It serves as a representation of SolidWorks, and is responsible for handling all SolidWorks commands.
 
 Attributes
 ``````````
@@ -167,14 +171,26 @@
     """
     Parameters:
       - filepath ( Filepath ) - Target file whos state should change.
       - state ( str ) - Literal name of the target state.
       - message ( str ) - Message to include in the file's PDM history.
     """
 
+``@profile`` ( decorator )
+--------------------------
+The ``@profile`` decorator can be applied to any function to capture its execution details, such as runtime ( seconds ). All ``solidworks`` and ``vault`` methods implement this decorator by default.
+
+To use this decorator, include the following import statement :
+
+.. code:: python
+
+  from solidwrap import profile
+
+----
+
 Appendix
 --------
 Two container classes are used to simplify the concept of a SolidWorks "document." SW-API tends to prefer the use of complete filepaths as direct references to documents. This is cumbersome, and a less verbose solution is implemented by SolidWrap to streamline file references.
 
 ``Model`` ( class )
 -------------------
 A container that holds Filepath, IModelDoc2, and IEdmFile5 information.
```

### Comparing `solidwrap-1.0.3/solidwrap/solidwrap.py` & `solidwrap-1.0.4/solidwrap/solidwrap.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,36 +23,37 @@
 # ---------------------
 # II. Import Definition
 # ---------------------
 
 __all__ = [
     "solidworks",
     "vault",
-    "Model",
+    "SWDocument",
     "Filepath",
     "profile"
 ]
 
 
 # ------------
 # III. Classes
 # ------------
 
 # Helper class
-class Model:
+class SWDocument:
     """
-    Model
-    -----
+    Document
+    --------
     Convenience wrapper for SolidWorks IModelDoc2 objects.
     """
     # Special Methods
     # ---------------
-    def __init__(self, model):
-        self.filepath = Filepath(model.GetPathName) # Filepath
-        self.swobj = model                          # IModelDoc2
+    def __init__(self, swobj):
+        self.filepath   = Filepath(swobj.GetPathName)   # Filepath
+        self.swobj      = swobj                         # IModelDoc2
+        
 
 # Core class
 @singleton
 class SolidWorks:
     """
     SolidWorks
     ---------
@@ -63,258 +64,230 @@
     client  = None
     version = None
 
     # Pubic Methods
     # -------------
     @profile
     def connect(self, version: int=2021, visible: bool=False):
-        """
-        Creates a connection to the SolidWorks process.
-        """
+        '''Creates a connection to the SolidWorks process.'''
         print(f"Connecting to SolidWorks client...")
 
         # Instantiate SolidWorks application via win32com dispatch (w/o concrete CLSID)
         self.version = version
         if not self.client:                                                                     # if a client is not defined...
             self.client = win.Dispatch("SldWorks.Application.%d" % (int(self.version)-1992))    # connect to new client  
             self.client.Visible = visible                                                       # make application visible
         else:                                                                                   # ...else terminal warning
             print(f"SolidWorks client connection is already established!")
 
     @profile
     def disconnect(self):
-        """
-        Terminates connection to the SolidWorks process.
-        """
+        '''Terminates connection to the SolidWorks process.'''
         print(f"Terminating SolidWorks process...")
         subproc.call(f"Taskkill /IM SLDWORKS.exe /F")
         # No follow-up terminal message necessary; subproc.call() auto-responds
 
-    @profile
-    def open(self, filepath: Filepath) -> Model:
-        """
-        Opens a model using the specified complete path.
-        """
+    def open(self, filepath: Filepath) -> SWDocument:
+        '''Opens a document using the specified complete path.'''
         print(f"Opening: {filepath.name}")
 
         # Define COM VARIANT arguments
+        doc_type = None
+        match filepath.extension:
+            case '.SLDPRT':
+                doc_type = win.VARIANT(pycom.VT_I4, 1)
+            case '.SLDASM':
+                doc_type = win.VARIANT(pycom.VT_I4, 2)
+            case '.SLDDRW':
+                doc_type = win.VARIANT(pycom.VT_I4, 3)
+
         file        = win.VARIANT(pycom.VT_BSTR,    filepath.complete)
-        doc_type    = win.VARIANT(pycom.VT_I4,      1)
         options     = win.VARIANT(pycom.VT_I4,      1)
         config      = win.VARIANT(pycom.VT_BSTR,    None)
         errors      = win.VARIANT(pycom.VT_BYREF |  pycom.VT_I4, 2)
         warnings    = win.VARIANT(pycom.VT_BYREF |  pycom.VT_I4, 128)
 
         # Execute SW-API method
-        raw_model = self.client.OpenDoc6(file, doc_type, options, config, errors, warnings)
+        swobj = self.client.OpenDoc6(file, doc_type, options, config, errors, warnings)
 
-        # Execute SW-API method - activate document
-        # arg1 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 0)
-        # self.client.ActivateDoc3(filepath.complete, False, 2, arg1)
-
-        # Return Model
-        return Model(raw_model)
+        # Return Document
+        return SWDocument(swobj)
     
-    @profile
-    def safeclose(self, model: Model):
-        """
-        Closes the target model ( WITH rebuild and save methods ).
-        """
-        self.rebuild(model)
-        self.save(model)
+    def safeclose(self, document: SWDocument):
+        '''Closes the target document ( WITH rebuild and save methods ).'''
+        self.rebuild(document)
+        self.save(document)
 
-        print(f"Closing: {model.filepath.name}")
+        print(f"Closing: {document.filepath.name}")
 
         # Execute SW-API method
-        self.client.CloseDoc(model.filepath.complete)
+        self.client.CloseDoc(document.filepath.complete)
 
-    @profile
-    def close(self, model: Model):
-        """
-        Closes the target model ( WITHOUT rebuild and save methods ).
-        """
-        print(f"Closing: {model.filepath.name}")
+    def close(self, document: SWDocument):
+        '''Closes the target document ( WITHOUT rebuild and save methods ).'''
+        print(f"Closing: {document.filepath.name}")
 
         # Execute SW-API method
-        self.client.CloseDoc(model.filepath.complete)
+        self.client.CloseDoc(document.filepath.complete)
 
-    @profile
-    def save(self, model: Model):
-        """
-        Saves the target model.
-        """
-        print(f"Saving: {model.filepath.name}")
+    def save(self, document: SWDocument):
+        '''Saves the target document.'''
+        print(f"Saving: {document.filepath.name}")
 
         # Define COM VARIANT arguments
         options     = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 1)
         errors      = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 1)
         warnings    = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 1)
 
         # Execute SW-API method
-        model.swobj.Save3(options, errors, warnings)
+        document.swobj.Save3(options, errors, warnings)
 
-    @profile
-    def rebuild(self, model: Model):
-        """
-        Rebuilds the target model.
-        """
-        print(f"Rebuilding: {model.filepath.name}")
+    def rebuild(self, document: SWDocument):
+        '''Rebuilds the target document.'''
+        print(f"Rebuilding: {document.filepath.name}")
         
         # Define COM VARIANT arguments
         arg1 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, False)
 
         # Execute SW-API method
-        model.swobj.ForceRebuild3(arg1)
+        document.swobj.ForceRebuild3(arg1)
+
+    def export(self, document: SWDocument, as_type: str="PNG"):
+        '''Exports the target document as the prescribed file type.'''
+
+        # Guard against incompatible types
+        if document.filepath.extension == '.SLDDRW' and as_type != 'pdf':
+            print(f"Drawings can only be exported as PDFs")
+            return -1
 
-    @profile
-    def export(self, model: Model, as_type: str="PNG"):
-        """
-        Exports the target model as the prescribed file type.
-        """
         # Format components
         extension   = str("." + as_type)
         desktop     = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop')
         destination = str(desktop + fr"\SolidWrap Exports")
-        file        = Filepath(f"{destination}\{model.filepath.root}{extension}")
+        file        = Filepath(f"{destination}\{document.filepath.root}{extension}")
 
         # Make export directory
         if not os.path.exists(destination):
             os.makedirs(destination)
 
         print(f"Exporting: {file.name}")
 
-        self.stage(model)
+        # Ignore staging for drawings
+        if document.filepath.extension != '.SLDDRW':
+            self.stage(document)
 
         # Define COM VARIANT arguments
         arg1 = win.VARIANT(pycom.VT_DISPATCH, None)
         arg2 = win.VARIANT(pycom.VT_BOOL, 0) 
         arg3 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 0)
         arg4 = win.VARIANT(pycom.VT_BYREF | pycom.VT_I4, 0)
 
         # Execute SW-API method
-        model.swobj.Extension.SaveAs2(file.complete, 0, 1, arg1, "", arg2, arg3, arg4)
+        document.swobj.Extension.SaveAs2(file.complete, 0, 1, arg1, "", arg2, arg3, arg4)
 
-    @profile
-    def freeze(self, model: Model):
-        """
-        Freezes the target model's feature tree.
-        """
-        print(f"Freezing: {model.filepath.name}")
+    def freeze(self, document: SWDocument):
+        '''Freezes the target document's feature tree.'''
+        print(f"Freezing: {document.filepath.name}")
 
         # Define COM VARIANT arguments
         setting = win.VARIANT(pycom.VT_I4, 461)
 
         # Execute SW-API method - show freeze bar
         self.client.SetUserPreferenceToggle(setting, True)
 
         # Get last feature in Feature Tree
-        feature = getLastFeature(model)
+        feature = get_last_feature(document)
 
         # Define COM VARIANT arguments
         position = win.VARIANT(pycom.VT_I4, 3)
 
         # Execute SW-API method - move freeze bar to end of feature tree
-        model.swobj.FeatureManager.EditFreeze(position, feature.Name, True)
+        document.swobj.FeatureManager.EditFreeze(position, feature.Name, True)
 
-    @profile
-    def declutter(self, model: Model, declutter: bool=True):
-        """
-        Hides/Shows all of the target model's sketches, reference geometry, etc.
-        """
-        print(f"Decluttering: {model.filepath.name}")
+    def declutter(self, document: SWDocument, declutter: bool=True):
+        '''Hides/Shows all of the target document's sketches, reference geometry, etc.'''
+        print(f"Decluttering: {document.filepath.name}")
 
         # Define COM VARIANT arguments
         setting = win.VARIANT(pycom.VT_I4, 198) # swUserPreferenceToggle_e.swViewDisplayHideAllTypes
         
         # Execute SW-API Method: SetUserPreferenceToggle - hide all types (planes, sketches, etc.)
-        model.swobj.Extension.SetUserPreferenceToggle(setting, 0, declutter)
+        document.swobj.Extension.SetUserPreferenceToggle(setting, 0, declutter)
         
-    @profile
-    def stage(self, model: Model):
-        """
-        Decultters viewport and orients an isometric model view.
-        """
-        print(f"Staging: {model.filepath.name}")
-        self.declutter(model=model)
+    def stage(self, document: SWDocument):
+        '''Declutters viewport and orients an isometric document view.'''
+        print(f"Staging: {document.filepath.name}")
+        self.declutter(document=document)
 
-        # Execute SW-API Method: ShowNamedView2 - orient model to isometric view
-        model.swobj.ShowNamedView2("Isometric", 7)
+        # Execute SW-API Method: ShowNamedView2 - orient document to isometric view
+        document.swobj.ShowNamedView2("Isometric", 7)
 
-        # Execute SW-API Method: ViewZoomtofit2 - center model in viewport
-        model.swobj.ViewZoomtofit2()
+        # Execute SW-API Method: ViewZoomtofit2 - center document in viewport
+        document.swobj.ViewZoomtofit2()
 
         # Execute SW-API Method: InsertScene - force background to plain white
-        model.swobj.Extension.InsertScene(fr"\scenes\01 basic scenes\11 white kitchen.p2s")
+        document.swobj.Extension.InsertScene(fr"\scenes\01 basic scenes\11 white kitchen.p2s")
+
 
 # Core class
 @singleton
 class Vault:
     """
     Vault
     ---------
     Wrapper for SolidWorks PDM API. Represents PDM Vault.
     """
     # Attributes
     # ----------
     client      = None  # win32com application
-    name        = None  # PDM Vault name (ex. "Goddard_Vault")
+    name        = None  # PDM Vault name (ex. "My_Vault")
     auth_state  = False # login credential authorization flag
 
     # Public Methods
     # --------------
     @profile
-    def connect(self, name: str="Goddard_Vault"):
-        """
-        Creates a connection to the PDM Vault.
-        """
+    def connect(self, name: str="My_Vault"):
+        '''Creates a connection to the PDM Vault.'''
         print(f"Connecting to PDM...")
 
         # Instantiate PDM Vault via win32com dispatch (w/o concrete CLSID)
         self.name = name
         if not self.client:                                     # if a client is not defined...
             self.client = win.Dispatch("ConisioLib.EdmVault")   # connect to client
         else:                                                   # ...else terminal warning
             print(f"PDM connection is already established!")
         self.authenticate()
 
     @profile
     def authenticate(self):
-        """
-        Authenticates login credentials for PDM Vault.
-        """
+        '''Authenticates login credentials for PDM Vault.'''
         print(f"Authentiating PDM credentials...")
 
         # Attempt login & flag authentication state
         if not self.client.IsLoggedIn:
             self.client.LoginAuto(self.name, 0)
             self.auth_state = True
 
-    @profile
     def checkout(self, filepath: Filepath):
-        """
-        Checks out model from PDM Vault.
-        """
+        '''Checks out a file from the PDM Vault.'''
         print(f"Check Out: {filepath.name}")
 
         # Get PDM-API objects
         directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
-        file = directory.GetFile(filepath.name)                         # IEdmFile
+        file = directory.GetFile(filepath.name)                        # IEdmFile
 
         # Execute PDM-API method
         if not file.IsLocked:                       # if file is not checked out...
             file.LockFile(directory.ID, 0)          # check out file
         else:
             print(f"File is already checked out!")  # ...else terminal warning
     
     # WIP
-    @profile
     def batch_checkout(self, files):
-        """
-        Checks out a collection of models from PDM Vault.
-        """
+        '''Checks out a collection of files from the PDM Vault.'''
         for file in files:
             self.checkout(filepath=file)
         
         # ---
         # WIP
         # ---
         # filepath = fr"C:\Goddard_Vault\Users\SYeatts\Scripts"
@@ -330,72 +303,99 @@
         #     # utility.AddFile(file_id, folder_id)
         #     utility.AddSelectionEx(vault.client, file_id, folder_id, item.CurrentVersion)
         
         # utility.CreateTree(0, 2)    # @param2 (2) Egcf_Lock
         # # utility.GetFiles()
         # print(f"{utility.FileCount}")
 
-    @profile
     def checkin(self, filepath: Filepath, message: str="SolidWrap Automated Check In"):
-        """
-        Checks in model to PDM Vault.
-        """
+        '''Checks in a file to the PDM Vault.'''
         print(f"Check In: {filepath.name}")
 
         # Get PDM-API objects
-        directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
         file = directory.GetFile(filepath.name)                         # IEdmFile5
 
         # Execute PDM-API method
         if file.IsLocked:                           # if file is not checked in...
             file.UnlockFile(0, message)             # check in file
         else:
             print(f"File is already checked in!")   # ...else terminal warning
 
     # WIP
-    @profile
     def batch_checkin(self, files, message: str="SolidWrap Automated Check In"):
-        """
-        Checks in a collection of models to PDM Vault.
-        """
+        '''Checks in a collection of files to the PDM Vault.'''
         for file in files:
             self.checkin(filepath=file)
 
     # WIP
-    @profile
     def change_state(self, filepath: Filepath, state: str="WIP", message: str="SolidWrap Automated State Change"):
-        """
-        Changes model's PDM state to prescribed value, if allowed.
-        """
-        # print(f"Change State: {filepath.name}")
+        '''Changes a file's PDM state to the prescribed value, if allowed.'''
+        print(f"Change State: {filepath.name}")
 
         # directory   = self.client.GetFolderFromPath(filepath.directory) # IEdmFolder5
         # folder_id   = directory.ID                                      # IEdmFolder5.ID (int?)
         # file        = directory.GetFile(filepath.name)                  # IEdmFile
         # file.ChangeState(state, folder_id, message, 0, 0)
 
+    def get_revision(self, filepath: Filepath) -> str:
+        '''Returns current revision of the target file.'''
+        
+        # Get PDM-API objects
+        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        file = directory.GetFile(filepath.name)                         # IEdmFile5
+        return file.CurrentRevision
+    
+    def is_checked_out(self, filepath: Filepath) -> bool:
+        '''Returns checkout state of the target file.'''
+        
+        # Get PDM-API objects
+        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        file = directory.GetFile(filepath.name)                         # IEdmFile5
+        
+        if file.IsLocked:
+            return True
+        else:
+            return False
+
+    def get_size(self, filepath: Filepath) -> int:
+        '''Returns size of the target file (MB).'''
+
+        # Get PDM-API objects
+        directory = self.client.GetFolderFromPath(filepath.directory)  # IEdmFolder
+        file = directory.GetFile(filepath.name)                        # IEdmFile
+        return int(file.GetLocalFileSize2(directory.ID)/1000)
+
+    # WIP
+    def get_pdm_state(self, filepath: Filepath) -> str:
+        '''Returns PDM state of the target file.'''
+        
+        # Get PDM-API objects
+        directory = vault.client.GetFolderFromPath(filepath.directory)  # IEdmFolder5
+        file = directory.GetFile(filepath.name)                         # IEdmFile5
+        return file.CurrentState.GetFirstTransitionPosition()
+
 
 # --------------
 # IV. Singletons
 # --------------
 
 vault = Vault()
 solidworks = SolidWorks()
 
 
 # ------------
 # V. Functions
 # ------------
 
-def getLastFeature(model: Model):
-    """
-    Gets the last feature in the model's Feature Tree.
-    """
+def get_last_feature(document: SWDocument):
+    '''Gets the last feature in the document's Feature Tree.'''
+
     # Get Feature Manager
-    manager = model.swobj.FeatureManager
+    manager = document.swobj.FeatureManager
 
     # Pre-iteration setup
     count = manager.GetFeatureCount(True)
     tree = manager.GetFeatureTreeRootItem2(0)
 
     # Iterate through tree to get last item (yes, it has to be done this way)
     feature = tree.GetFirstChild
```

### Comparing `solidwrap-1.0.3/solidwrap/utilities/utilities.py` & `solidwrap-1.0.4/solidwrap/utilities/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,10 +29,10 @@
     """
     @functools.wraps(func)                  # helper decorator to preserve function reference
     def wrapper_profile(*args, **kwargs):   # '*args, **kwargs' allows for infinte arguments
         start_time = time.perf_counter()    # get time at start
         value = func(*args, **kwargs)
         end_time = time.perf_counter()      # get time at end
         run_time = end_time - start_time    # calculate runtime
-        print(f"-- process {func.__name__!r} runtime: {run_time:.4f}s")
+        print(f"- {func.__name__!r} runtime: {run_time:.4f}s")
         return value
     return wrapper_profile
```

### Comparing `solidwrap-1.0.3/tests/test.py` & `solidwrap-1.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.3/pyproject.toml` & `solidwrap-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "solidwrap"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Sean Yeatts" },
 ]
 license = {text = "MIT License"}
 description = "Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow."
 readme = "../README.rst"
 requires-python = ">=3.7"
```

### Comparing `solidwrap-1.0.3/../README.rst` & `solidwrap-1.0.4/../README.rst`

 * *Files identical despite different names*

### Comparing `solidwrap-1.0.3/PKG-INFO` & `solidwrap-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidwrap
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wrapper for SolidWorks and PDM APIs for a streamlined, Pythonic workflow.
 Project-URL: Homepage, https://github.com/SeanYeatts/SolidWrap/tree/main
 Project-URL: Bug Tracker, https://github.com/users/SeanYeatts/projects/6/views/1
 Author: Sean Yeatts
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

