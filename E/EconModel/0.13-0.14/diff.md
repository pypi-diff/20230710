# Comparing `tmp/EconModel-0.13.tar.gz` & `tmp/EconModel-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EconModel-0.13.tar", last modified: Wed Feb 16 10:59:21 2022, max compression
+gzip compressed data, was "EconModel-0.14.tar", last modified: Mon Jul 10 07:17:17 2023, max compression
```

## Comparing `EconModel-0.13.tar` & `EconModel-0.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-02-16 10:59:21.373654 EconModel-0.13/
-drwxrwxrwx   0        0        0        0 2022-02-16 10:59:21.326736 EconModel-0.13/EconModel/
--rw-rw-rw-   0        0        0    11783 2022-02-16 10:52:19.000000 EconModel-0.13/EconModel/EconModel.py
--rw-rw-rw-   0        0        0       59 2021-06-05 20:09:11.000000 EconModel-0.13/EconModel/__init__.py
--rw-rw-rw-   0        0        0    11265 2022-02-16 10:53:04.000000 EconModel-0.13/EconModel/cppcompile.py
--rw-rw-rw-   0        0        0     7933 2022-02-11 13:27:34.000000 EconModel-0.13/EconModel/cppstruct.py
--rw-rw-rw-   0        0        0    14911 2022-02-16 10:22:51.000000 EconModel-0.13/EconModel/cpptools.py
--rw-rw-rw-   0        0        0     1199 2022-02-12 12:29:23.000000 EconModel-0.13/EconModel/jit.py
-drwxrwxrwx   0        0        0        0 2022-02-16 10:59:21.358028 EconModel-0.13/EconModel.egg-info/
--rw-rw-rw-   0        0        0      322 2022-02-16 10:59:20.000000 EconModel-0.13/EconModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2022-02-16 10:59:21.000000 EconModel-0.13/EconModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-16 10:59:20.000000 EconModel-0.13/EconModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-02-16 10:59:20.000000 EconModel-0.13/EconModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1095 2022-01-29 10:51:26.000000 EconModel-0.13/LICENSE
--rw-rw-rw-   0        0        0      322 2022-02-16 10:59:21.373654 EconModel-0.13/PKG-INFO
--rw-rw-rw-   0        0        0     3162 2022-02-11 08:32:46.000000 EconModel-0.13/README.md
--rw-rw-rw-   0        0        0       86 2022-02-16 10:59:21.373654 EconModel-0.13/setup.cfg
--rw-rw-rw-   0        0        0      315 2022-02-16 10:57:23.000000 EconModel-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:17:17.227231 EconModel-0.14/
+drwxrwxrwx   0        0        0        0 2023-07-10 07:17:17.201247 EconModel-0.14/EconModel/
+-rw-rw-rw-   0        0        0    11921 2023-07-10 07:10:54.000000 EconModel-0.14/EconModel/EconModel.py
+-rw-rw-rw-   0        0        0       59 2023-01-27 12:31:05.000000 EconModel-0.14/EconModel/__init__.py
+-rw-rw-rw-   0        0        0    13724 2023-06-19 07:38:29.000000 EconModel-0.14/EconModel/cppcompile.py
+-rw-rw-rw-   0        0        0     7933 2022-02-11 13:27:34.000000 EconModel-0.14/EconModel/cppstruct.py
+-rw-rw-rw-   0        0        0    15038 2022-02-17 15:53:49.000000 EconModel-0.14/EconModel/cpptools.py
+-rw-rw-rw-   0        0        0     1199 2022-02-16 13:47:45.000000 EconModel-0.14/EconModel/jit.py
+drwxrwxrwx   0        0        0        0 2023-07-10 07:17:17.224233 EconModel-0.14/EconModel.egg-info/
+-rw-rw-rw-   0        0        0      254 2023-07-10 07:17:16.000000 EconModel-0.14/EconModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-10 07:17:17.000000 EconModel-0.14/EconModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 07:17:16.000000 EconModel-0.14/EconModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 07:17:16.000000 EconModel-0.14/EconModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1095 2022-01-29 10:51:26.000000 EconModel-0.14/LICENSE
+-rw-rw-rw-   0        0        0      254 2023-07-10 07:17:17.227231 EconModel-0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     3485 2023-05-11 05:52:08.000000 EconModel-0.14/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-10 07:17:17.230230 EconModel-0.14/setup.cfg
+-rw-rw-rw-   0        0        0      315 2023-07-10 07:14:00.000000 EconModel-0.14/setup.py
```

### Comparing `EconModel-0.13/EconModel/EconModel.py` & `EconModel-0.14/EconModel/EconModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """ EconModelClass
 
-Provides a class for consumption-saving models with methods for saving and loading
+Provides a class for economic models with methods for saving and loading
 and interfacing with numba jitted functions and C++.
 
 """
 
 import os
 from copy import deepcopy
 import pickle
@@ -49,22 +49,22 @@
             assert hasattr(self,'settings'), 'the model must have defined an .settings() method'
             self.settings()
 
             # default to none
             for attr in self.other_attrs:
                 if not hasattr(self,attr): setattr(self,attr,None)
 
-            self.par = SimpleNamespace() # -> helps linter
-            self.sol = SimpleNamespace() # -> helps linter
-            self.sim = SimpleNamespace() # -> helps linter
-
-            for ns in self.namespaces:
-                setattr(self,ns,SimpleNamespace())
-
-            self.namespaces = list(set(self.namespaces + ['par','sol','sim']))
+            if len(self.namespaces) == 0:
+                self.namespaces =  ['par','sol','sim']
+                self.par = SimpleNamespace() # -> helps linter
+                self.sol = SimpleNamespace() # -> helps linter
+                self.sim = SimpleNamespace() # -> helps linter
+            else:
+                for ns in self.namespaces:
+                    setattr(self,ns,SimpleNamespace())
 
             # iii setup
             assert hasattr(self,'setup'), 'the model must have defined an .setup() method'
             self.setup()
 
             if load:
                 
@@ -76,15 +76,15 @@
 
                 # vi. update par
                 self.__update(kwargs)
 
             else:
 
                 # iv. update
-                self.__update(kwargs)
+                self.__update(kwargs,allow_new_keys=True)
                 
                 # vi. allocate
                 assert hasattr(self,'allocate'), 'the model must have defined an .allocate() method'
                 self.allocate()
 
         else:
             
@@ -92,22 +92,22 @@
 
         # c. infrastructure
         self.infer_types()
     
     def __name__(self):
         return 'EconModelClass' 
 
-    def __update(self,upd_dict):
+    def __update(self,upd_dict,allow_new_keys=False):
         """ update """
 
         for nskey,values in upd_dict.items():
             assert nskey in self.namespaces, f'{nskey} is not a namespace'
             assert type(values) is dict, f'{nskey} must be dict'
             for key,value in values.items():
-                assert hasattr(getattr(self,nskey),key), f'{key} is not in {nskey}' 
+                if not allow_new_keys: assert hasattr(getattr(self,nskey),key), f'{key} is not in {nskey}' 
                 setattr(getattr(self,nskey),key,value)        
 
     ####################
     ## infrastructure ##
     ####################
 
     def infer_types(self):
@@ -198,21 +198,23 @@
                             namespace.__dict__[k] = deepcopy(v)
                     else: # full copy
                         setattr(self,attr,deepcopy(model_dict[attr]))
                 else:
                     setattr(self,attr,model_dict[attr])
 
         if model_dict['link_to_cpp']: 
-            self.link_to_cpp(force_compile=False,check=False)
+            self.link_to_cpp(force_compile=False)
         else:
             self.cpp = SimpleNamespace()            
 
-    def save(self,drop=[]):
+    def save(self,drop=None):
         """ save the model """
 
+        if drop is None: drop = []
+
         # a. ensure path        
         if not os.path.exists(self.savefolder):
             os.makedirs(self.savefolder)
 
         # b. create model dict
         model_dict = self.as_dict(drop=drop)
 
@@ -273,17 +275,17 @@
             """ print items in SimpleNamespace """
 
             description = ''
             nbytes = 0
 
             for key,val in sn.__dict__.items():
 
-                if np.isscalar(val) and not type(val) is np.bool:
+                if np.isscalar(val) and not type(val) is np.bool_:
                     description += f' {key} = {val} [{type(val).__name__}]\n'
-                elif type(val) is np.bool:
+                elif type(val) is np.bool_:
                     if val:
                         description += f' {key} = True\n'
                     else:
                         description += f' {key} = False\n'
                 elif type(val) is np.ndarray:
                     description += f' {key} = ndarray with shape = {val.shape} [dtype: {val.dtype}]\n'            
                     nbytes += val.nbytes
```

### Comparing `EconModel-0.13/EconModel/cppcompile.py` & `EconModel-0.14/EconModel/cppcompile.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """ cppcompile
 
 Functions for compiling C++ files to use in Python.
 
 """
 
 import os
+import shutil
 import zipfile
 import urllib.request
 from subprocess import PIPE, run
 
 ############
 # auxilary #
 ############
@@ -95,14 +96,16 @@
             print('C++ files compiled')
         if do_print: print('NLopt successfully installed')
     else:
         print('terminal:')
         print(result.stdout)
         raise RuntimeError('NLopt installation failed')
 
+    os.remove('compile_nlopt.bat')
+
 def setup_tasmanian(download=True,unzip=False,folder='cppfuncs/',do_print=False):
     """download and setup Tasmanian 7.0
 
     Args:
 
         download (bool,optional): download Tasmanian 7.0
         unzip (bool,optional): unzip even if not downloaded
@@ -132,15 +135,15 @@
 def setup_alglib(download=True,unzip=False,folder='cppfuncs/',do_print=False):
     """download and setup ALGLIB 3.17
 
     Args:
 
         download (bool,optional): download ALGLIB 3.17
         unzip (bool,optional): unzip even if not downloaded
-        folder (str,optional): folder to put Tasmanian to
+        folder (str,optional): folder to put ALGLIB to
         do_print (bool,optional): print progress
 
     """
 
     if os.path.isdir(f'{os.getcwd()}/{folder}alglib-3.17.0'):
         if do_print: print('alglib already installed')
         return
@@ -154,14 +157,88 @@
     # b. unzip
     if download or unzip:
         with zipfile.ZipFile(zipfilename) as file:
             file.extractall(f'{os.getcwd()}/{folder}alglib-3.17.0')
 
     if do_print: print('alglib succesfully installed')
 
+def setup_autodiff(download=True,unzip=False,folder='cppfuncs/',do_print=False):
+    """download and setup autodiff
+
+    Args:
+
+        download (bool,optional): download autodiff
+        unzip (bool,optional): unzip even if not downloaded
+        folder (str,optional): folder to put autodiff to
+        do_print (bool,optional): print progress
+
+    """
+
+    if os.path.isdir(f'{os.getcwd()}/{folder}autodiff'):
+        if do_print: print('autodiff already installed')
+        return
+
+    # a. download
+    zipfilename = os.path.abspath(f'{os.getcwd()}/{folder}autodiff-master.zip')
+    if download:
+        url = 'https://github.com/autodiff/autodiff/archive/refs/heads/master.zip'
+        urllib.request.urlretrieve(url,zipfilename)
+        
+    # b. unzip
+    if download or unzip:
+        with zipfile.ZipFile(zipfilename) as file:
+            file.extractall(f'{os.getcwd()}/{folder}')
+        
+    # c. move
+    src = f'{os.getcwd()}/{folder}/autodiff-master/autodiff'
+    dst = f'{os.getcwd()}/{folder}/autodiff'
+    shutil.move(src,dst)
+
+    # d. clean
+    shutil.rmtree(f'{os.getcwd()}/{folder}/autodiff-master/')
+
+    if do_print: print('autodiff succesfully installed')
+
+def setup_Eigen(download=True,unzip=False,folder='cppfuncs/',do_print=False):
+    """download and setup autodiff
+
+    Args:
+
+        download (bool,optional): download Eigen 3.4.0
+        unzip (bool,optional): unzip even if not downloaded
+        folder (str,optional): folder to put Eigen to
+        do_print (bool,optional): print progress
+
+    """
+
+    if os.path.isdir(f'{os.getcwd()}/{folder}Eigen'):
+        if do_print: print('Eigen already installed')
+        return
+
+    # a. download
+    zipfilename = os.path.abspath(f'{os.getcwd()}/{folder}Eigen-master.zip')
+    if download:
+        url = 'https://gitlab.com/libeigen/eigen/-/archive/3.4.0/eigen-3.4.0.zip'
+        urllib.request.urlretrieve(url,zipfilename)
+        
+    # b. unzip
+    if download or unzip:
+        with zipfile.ZipFile(zipfilename) as file:
+            file.extractall(f'{os.getcwd()}/{folder}')
+        
+    # c. move
+    src = f'{os.getcwd()}/{folder}/eigen-3.4.0/Eigen'
+    dst = f'{os.getcwd()}/{folder}/Eigen'
+    shutil.move(src,dst)
+
+    # d. clean
+    shutil.rmtree(f'{os.getcwd()}/{folder}/eigen-3.4.0')
+
+    if do_print: print('Eigen succesfully installed')
+
 def add_macros(macros):
     """ add macros to compile string
         
     Args:
 
         macros (dict/list): preprocessor macros
```

### Comparing `EconModel-0.13/EconModel/cppstruct.py` & `EconModel-0.14/EconModel/cppstruct.py`

 * *Files identical despite different names*

### Comparing `EconModel-0.13/EconModel/cpptools.py` & `EconModel-0.14/EconModel/cpptools.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 """
 
 import os
 import ctypes as ct
 import re
 import numpy as np
 
-from .cppcompile import compile, set_default_options, setup_nlopt, setup_tasmanian, setup_alglib
+from.cppcompile import setup_nlopt, setup_tasmanian, setup_alglib, setup_autodiff, setup_Eigen
+
+from .cppcompile import compile, set_default_options
 from .cppstruct import setup_struct, get_struct_pointer
 
 #################
 # file analysis #
 #################
 
 def find_all_filenames(filename,do_print=False):
@@ -143,15 +145,15 @@
 
         Args:
 
             filename (str): C++ file with .cpp extension (full path)
             force_compile (bool,optional): compile even if .dll is present
             structsmap (dict,optional): struct names as keys and associated pythonobj used in C++ as values
             options (dict,optional): compiler options
-            use_log (bool,optional): assumes log is printed to filename.log (deleted afterwards) (saved in self.log[funcname])
+            use_log (bool,optional): assumes log is printed to filename.log (deleted afterwards, saved in self.log[funcname])
             print_log (bool,optional): print log to screen when function is called
             do_print (bool,optional): print progress
 
         """
 
         assert os.path.isfile(filename), f'"{filename}" does not exist'
         if do_print: print(f'Linking to: {filename}')
@@ -397,17 +399,18 @@
             try:
 
                 p_args = self.__get_p_args(funcname,args)
                 funcnow = getattr(self.cppfile,funcname)
                 result = funcnow(*p_args)
                 break
 
-            except:
+            except Exception as e:
 
                 if n == 0: self.compile(force_compile=False) # re-linking might solve the problem
+                if n == 1: print(e) # print error message
 
         # print log
         if self.use_log:
 
             log_filename = f'{self.filename_raw}.log'
             if os.path.isfile(log_filename):
```

### Comparing `EconModel-0.13/EconModel/jit.py` & `EconModel-0.14/EconModel/jit.py`

 * *Files identical despite different names*

### Comparing `EconModel-0.13/LICENSE` & `EconModel-0.14/LICENSE`

 * *Files identical despite different names*

