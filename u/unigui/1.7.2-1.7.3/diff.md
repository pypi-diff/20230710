# Comparing `tmp/unigui-1.7.2.tar.gz` & `tmp/unigui-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.7.2.tar", last modified: Mon Jul 10 09:41:16 2023, max compression
+gzip compressed data, was "dist/unigui-1.7.3.tar", last modified: Mon Jul 10 20:24:13 2023, max compression
```

## Comparing `unigui-1.7.2.tar` & `unigui-1.7.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    11822 2023-07-02 15:37:04.000000 unigui-1.7.2/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-07-03 20:20:12.000000 unigui-1.7.2/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.7.2/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.7.2/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2396 2023-07-02 15:25:42.000000 unigui-1.7.2/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/css/vendor.49a52e8f.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/css/878.c6483fb6.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    45060 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/js/878.e76799d2.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/js/app.b39a06ae.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-10 09:32:13.000000 unigui-1.7.2/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.7.2/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-10 09:40:45.000000 unigui-1.7.2/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19162 2023-07-10 09:41:16.000000 unigui-1.7.2/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-10 09:41:16.000000 unigui-1.7.2/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18857 2023-07-10 09:39:31.000000 unigui-1.7.2/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.7.2/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19162 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.7.2/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-10 09:41:16.000000 unigui-1.7.2/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     9904 2023-07-10 20:13:51.000000 unigui-1.7.3/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9136 2023-07-10 12:04:53.000000 unigui-1.7.3/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3573 2023-07-10 12:41:32.000000 unigui-1.7.3/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.7.3/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2396 2023-07-02 15:25:42.000000 unigui-1.7.3/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/css/vendor.49a52e8f.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/css/878.c6483fb6.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    45060 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/878.e76799d2.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/app.b39a06ae.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-10 09:32:13.000000 unigui-1.7.3/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.7.3/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-10 20:23:44.000000 unigui-1.7.3/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19083 2023-07-10 20:24:13.000000 unigui-1.7.3/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-10 20:24:13.000000 unigui-1.7.3/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18778 2023-07-10 11:37:36.000000 unigui-1.7.3/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.7.3/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19083 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.7.3/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-10 20:24:13.000000 unigui-1.7.3/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.7.2/unigui/manager.py` & `unigui-1.7.3/unigui/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,36 @@
 import os
 import importlib
 from .utils import *
 from . import utils
 import itertools
-import time
 from .guielements import *
 import sys
 import asyncio
 import requests
 from threading import Thread
 
-users = {}
-
 sign2method = {'=':'changed', '->':'update','?':'complete','+':'append', '-':'delete', '!':'editing', '#':'modify'}    
 
 #loop and thread is only for progress window functionality
 loop = asyncio.new_event_loop()
 def f(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever() 
 
 t = Thread(target=f, args=(loop,))
 t.start()  
 
 class User:      
-    def __init__(self):   
-        self.change_buffer = []
-        self.redo_buffer = []      
-       
+    def __init__(self):          
         self.screens = []        
         self.active_dialog = None
-        self.screen_module = None
-        self.history_switching = []
-        self.history_pointer = 0        
-
-        self.oper_count = 0
-        self.time_last_change = time.time()
-        self.max_oper_time = 0.1  
-
+        self.screen_module = None                
         self.tool_buttons = []
-
-    def append_change(self, change):
-        self.change_buffer.append(change)
-        curr_time = time.time()
-        if curr_time - self.time_last_change > self.max_oper_time:
-            self.oper_count += 1
-            self.redo_buffer = [] #clean redo if new operation
-        change.oper = self.oper_count
-        self.time_last_change = curr_time        
-
-    def save_changes(self,*_):
-        pass
+        User.last_user = self
 
     def translate_path(self, path):        
         return utils.translate_path(path)
 
     @staticmethod
     def cache_name(url):    
         name = url.split('/')[-1]
@@ -94,93 +70,63 @@
                     break
 
     def progress(self, str, *updates):
         """open or update progress window if str != null else close it  """     
         d = {'progress': str}
         if updates:
             d['update'] = None            
-            d['data'] = updates         
-        
+            d['data'] = updates                 
         asyncio.run_coroutine_threadsafe(self.send(d), loop)            
-                          
-    def undo_last_operation(self, *_):
-        if self.undo_last_changes():            
-            return True  
-        return Error("Nothing to undo!")
-        
-    def redo_last_operation(self, *_):    
-        if self.redo_last_changes():            
-            return True     
-        return Error("Nothing to redo!")
-
-    def redo_last_changes(self):
-        if self.redo_buffer != []:
-            oper = self.redo_buffer[-1].oper                
-            undo_buffer_size = len(self.change_buffer)            
-            return True
-
-    def undo_last_changes(self):
-        if self.change_buffer != []:
-            oper = self.change_buffer[-1].oper
-            redo_buffer_size = len(self.redo_buffer)            
-            return True             
-
-    def go_back(self, *_):        
-        if self.history_pointer > 0:
-            self.history_pointer -= 1            
-        return Info('No more back references!')
-
-    def go_forward(self, *_):
-        if self.history_pointer < len(self.history_switching) - 1:
-            self.history_pointer += 1            
-        return Info('No more forward references!')
 
-    def load(self):   
+    def load_module(self, file):
         screen_vars = {
-            'icon' : 'article',
+            'icon' : None,
             'prepare' : None,
             'dispatch' : None,
             'blocks' : [],
             'header' : utils.appname,                        
-            'toolbar' : None, 
+            'toolbar' : [], 
             'order' : 0
         }     
+        
+        name = file[0:-3]
+        screens_dir =  'screens'
+             
+        #if name not in modules:                    
+        path = f'{screens_dir}/{file}'                
+        spec = importlib.util.spec_from_file_location(name,path)
+        module = importlib.util.module_from_spec(spec)        
+        
+        utils.clean_handlers()                                        
+        module.user = self                               
+        
+        spec.loader.exec_module(module)            
+        screen = Screen(module.name)
+        #set system vars
+        for var in screen_vars:                                            
+            setattr(screen, var, getattr(module,var,screen_vars[var])) 
+        screen.handlers__ = utils.handlers__
+        
+        if not screen.toolbar:
+            screen.toolbar = self.tool_buttons
+                        
+        screen.check()                         
+        module.screen = screen
+
+        return module
+                              
+    def load(self):   
          
         blocks_dir = 'blocks'        
         screens_dir =  'screens'
-        modules = {}
+        
         for file in os.listdir(screens_dir):
             if file.endswith(".py") and file != '__init__.py':
-                name = file[0:-3]
-
-                #if name not in modules:                    
-                path = f'{screens_dir}/{file}'                
-                spec = importlib.util.spec_from_file_location(name,path)
-                module = importlib.util.module_from_spec(spec)
-                modules[name] = module, spec                
-                
-                utils.clean_handlers()                                
-                
-                module.user = self                               
-                
-                spec.loader.exec_module(module)            
-
-                screen = Screen(module.name)     
-                module.screen = screen            
-                self.screens.append(module)
-
-                #set system vars
-                for var in screen_vars:                                            
-                    setattr(screen, var, getattr(module,var,screen_vars[var])) 
-                screen.handlers__ = utils.handlers__
-                
-                if not screen.toolbar:
-                    screen.toolbar = self.tool_buttons
-                                
-                screen.check()                         
+                module = self.load_module(file)                
+                self.screens.append(module)                
         
         self.screens.sort(key=lambda s: s.screen.order)
         main = self.screens[0]
         if 'prepare' in dir(main):
             main.prepare()
         self.screen_module = main
         self.menu = [[s.name,getattr(s,'icon', None)] for s in self.screens]        
@@ -250,17 +196,15 @@
                         if sub == elem:
                             return [bl.name, sub.name]
                 elif c == elem:
                     return [bl.name, c.name]
 
     def prepare_result(self, raw):
         if raw == UpdateScreen:
-            raw = self.screen            
-            #if getattr(raw,'prepare', False):
-            #    raw.prepare()
+            raw = self.screen                        
         else:
             if type(raw) == dict and 'update' in raw:
                 if isinstance(raw['data'], (list,tuple)):
                     raw['multi'] = True
                     raw['update'] = [self.find_path(e) for e in raw['data']]
                 else:
                     raw['update'] = self.find_path(raw['data'])
```

### Comparing `unigui-1.7.2/unigui/guielements.py` & `unigui-1.7.3/unigui/guielements.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,16 @@
 
 class Table(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)             
         self.check('headers')
         if not hasattr(self,'type'):
             self.type = 'table'
+        if not hasattr(self,'value'):
+            self.value = None
         if not hasattr(self,'rows'):
             self.rows = []
         if not hasattr(self,'value'):
             self.value = None
 
         if getattr(self,'edit', True):
             edit_setting = hasattr(self,'modify') or hasattr(self,'delete') or hasattr(self,'append')
```

### Comparing `unigui-1.7.2/unigui/server.py` & `unigui-1.7.3/unigui/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,15 @@
         while True:
             chunk = await field.read_chunk()  # 8192 bytes by default.
             if not chunk:
                 break
             size += len(chunk)
             f.write(chunk)
 
-    return web.Response(text='{} sized of {} successfully stored'
-                             ''.format(filename, size))
+    return web.Response(text=f'{filename} sized of {size} successfully stored')
 
 from config import port, user_dir, pretty_print, socket_ip, socket_port, upload_dir
 from pathlib import Path
 
 indent = 2 if pretty_print else 0
 
 def jsonString(obj):
@@ -76,21 +75,19 @@
                 ws.exception())
 
     print('websocket connection closed')
 
     return ws       
 
 def start(appname, user_type = User, translate_path = None, http_handlers = []):
-    wd = os.getcwd()
-    import sys
-    sys.path.insert(0,wd) #load from working directory
     
-    sys.path.pop(0) #delete work path
-
     set_utils(appname,user_dir, port, upload_dir, translate_path, socket_ip, socket_port)    
+    
+    if upload_dir and not os.path.exists(upload_dir):
+        os.makedirs(upload_dir)
 
     User.UserType = user_type
 
     if utils.socket_ip != 'localhost' or utils.resource_port != 8000 or utils.socket_port != 1234:
         User.create_fixed_js()     
         http_handlers.append(web.get(User.fix_file, static_serve))
     else:
```

### Comparing `unigui-1.7.2/unigui/utils.py` & `unigui-1.7.3/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/favicon.ico` & `unigui-1.7.3/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.7.3/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/css/878.c6483fb6.css` & `unigui-1.7.3/unigui/web/css/878.c6483fb6.css`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/icons/favicon-96x96.png` & `unigui-1.7.3/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/icons/favicon-16x16.png` & `unigui-1.7.3/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/icons/favicon-32x32.png` & `unigui-1.7.3/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/icons/favicon-128x128.png` & `unigui-1.7.3/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.7.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.7.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.7.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.7.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/js/430.591e9a73.js` & `unigui-1.7.3/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/js/878.e76799d2.js` & `unigui-1.7.3/unigui/web/js/878.e76799d2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/js/app.b39a06ae.js` & `unigui-1.7.3/unigui/web/js/app.b39a06ae.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/js/193.283445be.js` & `unigui-1.7.3/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.7.3/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/unigui/web/index.html` & `unigui-1.7.3/unigui/web/index.html`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/LICENSE` & `unigui-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.7.2/setup.py` & `unigui-1.7.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.7.2',      
+      version='1.7.3',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.7.2/PKG-INFO` & `unigui-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.7.2
+Version: 1.7.3
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,19 +18,18 @@
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
 ### How it works inside ###
-The exchange protocol for the solution is JSON as the most universally accessible, comprehensible, readable, and popular format compatible with all programming languages.  The server sends JSON data to Unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for user data. No markup, drawing instructions and the other dull job are required. Just the simplest description what you want. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
+The exchange protocol for the solution is JSON as the most universally accessible, readable, and popular format for Web. The server sends JSON data to the front-end unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for the user data. No markup, drawing instructions and the other dull job are required. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
-Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that.
-Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
+Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
@@ -213,15 +212,15 @@
 CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
 ```
 handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is defined in config.py .
 
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
-Edit('Number field', 0.9, type = 'number') #changed haandler will get a number
+Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
 If set edit = false it will be readonly field or text label.
 ```
 Edit('Some field', '', edit = false) 
 #is equal to
 Text('Some field')
 ```
```

### Comparing `unigui-1.7.2/README.md` & `unigui-1.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
 ### How it works inside ###
-The exchange protocol for the solution is JSON as the most universally accessible, comprehensible, readable, and popular format compatible with all programming languages.  The server sends JSON data to Unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for user data. No markup, drawing instructions and the other dull job are required. Just the simplest description what you want. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
+The exchange protocol for the solution is JSON as the most universally accessible, readable, and popular format for Web. The server sends JSON data to the front-end unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for the user data. No markup, drawing instructions and the other dull job are required. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
-Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that.
-Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
+Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
@@ -201,15 +200,15 @@
 CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
 ```
 handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is defined in config.py .
 
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
-Edit('Number field', 0.9, type = 'number') #changed haandler will get a number
+Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
 If set edit = false it will be readonly field or text label.
 ```
 Edit('Some field', '', edit = false) 
 #is equal to
 Text('Some field')
 ```
```

### Comparing `unigui-1.7.2/unigui.egg-info/PKG-INFO` & `unigui-1.7.3/unigui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.7.2
+Version: 1.7.3
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -18,19 +18,18 @@
 
 ### Installing ###
 ```
 pip install unigui
 ```
 
 ### How it works inside ###
-The exchange protocol for the solution is JSON as the most universally accessible, comprehensible, readable, and popular format compatible with all programming languages.  The server sends JSON data to Unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for user data. No markup, drawing instructions and the other dull job are required. Just the simplest description what you want. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
+The exchange protocol for the solution is JSON as the most universally accessible, readable, and popular format for Web. The server sends JSON data to the front-end unigui which has built-in tools (autodesigner) and automatically builds a standart Google Material Design GUI for the user data. No markup, drawing instructions and the other dull job are required. From the constructed Unigui screen the server receives a JSON message flow which fully describes what the user did. The message format is ["Block", "Elem", "type of action", value], where "Block"and "Elem"are the names of the block and its element, "value" is the JSON value of the action/event that has happened. The server can either accept the change or roll it back by sending an info window about an inconsistency. The server can open a dialog box, send popup Warning, Error,.. or an entirely new screen. Unigui instantly and automatically displays actual server state. 
 
 ### Programming ###
-Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that.
-Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
+Unigui is the language and platform independent technology. This repo explains how to work with Unigui using Python and the tiny but optimal framework for that. Unigui web version is included in this library. Unigui for Go is accessible in https://github.com/Claus1/unigui-go
 
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
@@ -213,15 +212,15 @@
 CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
 ```
 handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is defined in config.py .
 
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
-Edit('Number field', 0.9, type = 'number') #changed haandler will get a number
+Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
 If set edit = false it will be readonly field or text label.
 ```
 Edit('Some field', '', edit = false) 
 #is equal to
 Text('Some field')
 ```
```

### Comparing `unigui-1.7.2/unigui.egg-info/SOURCES.txt` & `unigui-1.7.3/unigui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

