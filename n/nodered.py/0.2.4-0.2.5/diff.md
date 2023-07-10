# Comparing `tmp/nodered.py-0.2.4.tar.gz` & `tmp/nodered.py-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.4.tar", last modified: Mon Jul  3 07:00:16 2023, max compression
+gzip compressed data, was "nodered.py-0.2.5.tar", last modified: Mon Jul 10 01:53:21 2023, max compression
```

## Comparing `nodered.py-0.2.4.tar` & `nodered.py-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.4/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-03 07:00:16.780000 nodered.py-0.2.4/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.4/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.630000 nodered.py-0.2.4/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-03 07:00:16.000000 nodered.py-0.2.4/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.4/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-07-03 06:04:11.000000 nodered.py-0.2.4/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    13201 2023-07-03 06:05:41.000000 nodered.py-0.2.4/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.4/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.4/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.4/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.4/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.4/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.4/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-03 07:00:16.720000 nodered.py-0.2.4/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.4/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.4/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.4/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.4/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-03 07:00:16.780000 nodered.py-0.2.4/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.4/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.5/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-10 01:53:21.590000 nodered.py-0.2.5/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.5/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       28 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.5/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      474 2023-07-10 01:13:03.000000 nodered.py-0.2.5/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    14560 2023-07-10 01:46:11.000000 nodered.py-0.2.5/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.5/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.5/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.5/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.470000 nodered.py-0.2.5/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.5/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.5/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.5/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.470000 nodered.py-0.2.5/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.5/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.5/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4998 2023-07-10 01:49:09.000000 nodered.py-0.2.5/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.5/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-10 01:53:21.590000 nodered.py-0.2.5/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.5/setup.py
```

### Comparing `nodered.py-0.2.4/LICENSE` & `nodered.py-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.4/PKG-INFO` & `nodered.py-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.4
+Version: 0.2.5
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.4 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.5 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.4/README.md` & `nodered.py-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.4/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.5/nodered.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.4
+Version: 0.2.5
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.4 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.5 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.2.4/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.5/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.4/noderedpy/_nodered.py` & `nodered.py-0.2.5/noderedpy/_nodered.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import os, sys, subprocess, shutil, json, traceback
 from types import MethodType
-from typing import List
+from typing import List, Literal
 from glob import glob
 from .templates import package_json, node_html, node_js
 from ._property import Property
 from . import __path__
 
 
 class RED:
@@ -293,14 +293,46 @@
                         break
             except ( psutil.AccessDenied, psutil.ZombieProcess ):
                 pass
 
             if killed:
                 break
 
+class NodeCommunicator:
+    def __init__(self, message_file:str, node_name:str):
+        self.__message_file, self.__node_name = message_file, node_name
+
+    def log(self, *args):
+        with open(self.__message_file, "w", encoding = "utf-8") as mfw:
+            json.dump({
+                "name": self.__node_name,
+                "log": args
+            }, mfw, indent = 4)
+
+    def warn(self, *args):
+        with open(self.__message_file, "w", encoding = "utf-8") as mfw:
+            json.dump({
+                "name": self.__node_name,
+                "warn": args
+            }, mfw, indent = 4)
+
+    def error(self, *args):
+        with open(self.__message_file, "w", encoding = "utf-8") as mfw:
+            json.dump({
+                "name": self.__node_name,
+                "error": args
+            }, mfw, indent = 4)
+
+    def status(self, fill:Literal["red", "green", "yellow", "blue", "grey"], shape:Literal["ring", "dot"], text:str):
+        with open(self.__message_file, "w", encoding = "utf-8") as mfw:
+            json.dump({
+                "name": self.__node_name,
+                "status": { "fill": fill, "shape": shape, "text": text }
+            }, mfw, indent = 4)
+
 class Node:
     def __init__(self, name:str, category:str, version:str, description:str, author:str, keywords:List[str], icon:str, properties:List[Property], node_func:MethodType):
         # name of node cannot contain spaces
         if " " in name.strip():
             raise NameError("Node name cannot contain spaces!")
         
         # category of node cannot contain - or ,
@@ -316,14 +348,15 @@
 
         self.name, self.category, self.version, self.description, self.author, self.icon, self.properties =\
             name, category, version, description, author, icon, properties
         
         self.__node_func = node_func
 
     def create(self, node_red_user_dir:str, node_red_user_cache_dir:str):
+        self.__communicator = NodeCommunicator(os.path.join(node_red_user_cache_dir, "message.json"), self.name)
         node_dir = os.path.join(node_red_user_dir, "node_modules", self.name if self.name.startswith("nodered-py-") else f"nodered-py-{self.name}")
         os.makedirs(os.path.join(node_dir, "lib"))
 
         with open(os.path.join(node_dir, "package.json"), "w", encoding = "utf-8") as pjw:
             pjw.write(package_json(self))
 
         with open(os.path.join(node_dir, "lib", f"{self.name}.html"), "w", encoding = "utf-8") as nhw:
@@ -331,16 +364,16 @@
 
         with open(os.path.join(node_dir, "lib", f"{self.name}.js"), "w", encoding = "utf-8") as njw:
             njw.write(node_js(self, node_red_user_cache_dir))
 
     def run(self, props:dict, msg:dict) -> dict:
         print(f"\n{self.name} started\n===================================")
         try:
-            resp = self.__node_func(props, msg)
+            resp = self.__node_func(self.__communicator, props, msg)
             print("============================= ended\n")
 
-            resp.update({ "state": "success" })
+            resp.update({ "state": "success", "name": self.name })
 
             return resp
         except:
             print("============================= error\n")
             return { "state": "fail", "message": traceback.format_exc() }
```

### Comparing `nodered.py-0.2.4/noderedpy/_property.py` & `nodered.py-0.2.5/noderedpy/_property.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-import json
+import json, pandas as pd
 from typing import Any, Union, List
 
 
 
 class Property:
     def __init__(self, name:str, default:Any = None, required:bool = False, display_icon:str = None):
         self.name, self.default, self.required, self.display_icon =\
@@ -69,25 +69,37 @@
                 json.loads(default)
             except:
                 raise ValueError("DictProperty value must be 'dict' or 'json string'!")
 
         if isinstance(default, dict):
             default = json.dumps(default, indent = 4)
 
-        super().__init__(name, default, "json", height, required, display_icon if display_icon else "fa fa-code")
+        super().__init__(name, default, "json", height, required, display_icon if display_icon else "fa fa-file-code-o")
 
 class SpinnerProperty(Property):
     def __init__(self, name:str, default:float = 0, step:float = None, min:float = None, max:float = None, required:bool = False, display_icon:str = None):
         if not isinstance(default, (int, float)):
             raise TypeError("SpinnerProperty can accept types: [ 'int', 'float' ]")
 
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-random")
         self.step, self.min, self.max =\
             step, min, max
 
+class CheckBoxProperty(Property):
+    def __init__(self, name:str, default:bool = False, required:bool = False, display_icon:str = None):
+        super().__init__(name, default, required, display_icon if display_icon else "fa fa-check")
+
 class ComboBoxProperty(Property):
     def __init__(self, name:str, items:List[Any], default:str = None, required:bool = False, display_icon:str = None):
         if not isinstance(items, list):
             raise TypeError("items of ComboBoxProperty must be type: 'list'")
         
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-filter")
         self.items = items
+
+# class FileProperty(Property):
+#     def __init__(self, name:str, default:str = None, required:bool = False, display_icon:str = None):
+#         super().__init__(name, default if default else "", required, display_icon if display_icon else "fa fa-file-text-o")
+
+# class TableProperty(Property):
+#     def __init__(self, name:str, default:pd.DataFrame = None, required:bool = False, display_icon:str = None):
+#         super().__init__(name, default if default else pd.DataFrame(), required, display_icon if display_icon else "fa fa-table")
```

### Comparing `nodered.py-0.2.4/noderedpy/assets/python-logo.png` & `nodered.py-0.2.5/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.4/noderedpy/decorator.py` & `nodered.py-0.2.5/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.4/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.5/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.4/noderedpy/templates/__init__.py` & `nodered.py-0.2.5/noderedpy/templates/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 import os, noderedpy
 from .._property import (
     InputProperty, ListProperty,
-    SpinnerProperty, ComboBoxProperty, CodeProperty
+    SpinnerProperty, CheckBoxProperty, ComboBoxProperty, CodeProperty,
+    # FileProperty, TableProperty
 )
 from . import __path__
 
 
 def package_json(node:"noderedpy._nodered.Node") -> str:
     with open(os.path.join(__path__[0], "template.json"), "r", encoding = "utf-8") as tr:
         tt = tr.read()
@@ -35,25 +36,25 @@
 def node_html(node:"noderedpy._nodered.Node") -> str:
     properties_html, properties_js, properties_js_prepare, properties_js_cancel, properties_js_save = [], [], [], [], []
     default_value = None
     for property in node.properties:
         if isinstance(property, InputProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
-        <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+        <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
         <input type="text" id="node-input-{property.name}" style="width:100%;">
     </div>
 """)
             default_value = f'"{property.default}"' if isinstance(property.default, str) else str(property.default)
         elif isinstance(property, ListProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
-        <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+        <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row node-input-{property.name}-container-row">
         <ol id="node-input-{property.name}-container" style="height:{property.height}px;"></ol>
     </div>
 """)
             properties_js_prepare.append('''
             $("#node-input-''' + property.name + '''-container").editableList({
@@ -77,15 +78,15 @@
                 this.''' + property.name + '''.push(item.find("input.input-list-item").val());
             });
 ''')
             default_value = str(property.default)
         elif isinstance(property, CodeProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
-        <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+        <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row node-text-editor-row">
         <div style="height:{property.height}px;" class="node-text-editor" id="node-input-{property.name}"></div>
     </div>
 """)
             if property.language:
                 properties_js_prepare.append('''
@@ -113,15 +114,15 @@
             this.{property.name}Editor.destroy();
             delete this.{property.name}Editor;
 """)
             default_value = f"`{property.default}`"
         elif isinstance(property, SpinnerProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
-        <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+        <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
         <input type="text" id="node-input-{property.name}" style="width:calc(100% - 22px);">
     </div>
 """)
             spinner_configs = []
             if property.min:
@@ -133,24 +134,32 @@
 
             properties_js_prepare.append('''
             $("#node-input-''' + property.name + '''").spinner({
                 ''' + "\n".join(spinner_configs) + '''
             });
 ''')
             default_value = str(property.default)
+        elif isinstance(property, CheckBoxProperty):
+            properties_html.append(f"""
+    <div class="form-row">
+        <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+        <input type="checkbox" style="margin-left:10px;width:15px;height:15px;margin-bottom:5px;" id="node-input-{property.name}">
+    </div>
+""")
+            default_value = "true" if property.default else "false"
         elif isinstance(property, ComboBoxProperty):
             options = "\n".join([
                 f"""
             <option value="{item}">{item}</option>
 """
                 for item in property.items
             ])
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
-        <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+        <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
         <select id="node-input-{property.name}Select" style="width:100%;">
 {options}
         </select>
         <input type="text" id="node-input-{property.name}" style="display:none;">
     </div>
@@ -158,14 +167,38 @@
             properties_js_prepare.append('''
             $("#node-input-''' + property.name + '''Select").val(this.''' + property.name + ''');
 ''')
             properties_js_save.append('''
             $("#node-input-''' + property.name + '''").val($("#node-input-''' + property.name + ''';").val());
 ''')
             default_value = f'"{property.default}"' if isinstance(property.default, str) else str(property.default)
+#         elif isinstance(property, FileProperty):
+#             properties_html.append(f"""
+#     <div class="form-row" style="display:flex;flex-flow:row;align-items:center;">
+#         <label style="width:auto;margin-bottom:0px;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+#         <input type="file" id="node-input-{property.name}" style="flex:1;">
+#     </div>
+# """)
+#             default_value = f'"{property.default}"'
+#         elif isinstance(property, TableProperty):
+#             theader = "\n".join([ f"                <th>{column}</th>" for column in property.default.columns ])
+#             properties_html.append(f"""
+#     <div class="form-row" style="margin-bottom:0px;">
+#         <label style="width:auto;"><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
+#     </div>
+#     <div class="form-row" style="display:flex;flex-flow:column;">
+#         <table>
+#             <thead>
+# {theader}
+#             </thead>
+#             <tbody>
+#             </tbody>
+#         </table>
+#     </div>
+# """)
 
         if default_value:
             properties_js.append("            " + property.name + ': { value: ' + default_value + ' }')
 
     with open(os.path.join(__path__[0], "template.html"), "r", encoding = "utf-8") as tr:
         tt = tr.read()
```

### Comparing `nodered.py-0.2.4/noderedpy/templates/template.html` & `nodered.py-0.2.5/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.4/noderedpy/templates/template.js` & `nodered.py-0.2.5/noderedpy/templates/template.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -53,14 +53,15 @@
                 fill: "green",
                 shape: "dot",
                 text: "Running"
             });
 
             const inpFile = path.join("{$cache_dir}", "input.json");
             const outFile = path.join("{$cache_dir}", "output.json");
+            const messageFile = path.join("{$cache_dir}", "message.json");
 
             // remove if outFile exists before run
             if (fs.existsSync(outFile)) {
                 fs.unlinkSync(outFile);
             }
 
             // send inputs to python
@@ -69,19 +70,45 @@
                 props: configToSend,
                 msg: message
             }, null, "    "));
 
             // wait until job done
             var resp = null;
             while (true) {
+                if (fs.existsSync(messageFile)) {
+                    try {
+                        var resp_msg = JSON.parse(fs.readFileSync(messageFile));
+                        if (resp_msg.name == "{$node_name}") {
+                            fs.unlinkSync(messageFile);
+
+                            if (resp_msg.status != undefined) {
+                                node.status(resp_msg.status);
+                            }
+                            if (resp_msg.log != undefined) {
+                                node.log(resp_msg.log.join(" "));
+                            }
+                            if (resp_msg.warn != undefined) {
+                                node.warn(resp_msg.warn.join(" "));
+                            }
+                            if (resp_msg.error != undefined) {
+                                node.error(resp_msg.error.join(" "));
+                            }
+                        }
+                    } catch {
+                        continue;
+                    }
+                }
+
                 if (fs.existsSync(outFile)) {
                     try {
                         resp = JSON.parse(fs.readFileSync(outFile));
-                        fs.unlinkSync(outFile);
-                        break;
+                        if (resp.name == "{$node_name}") {
+                            fs.unlinkSync(outFile);
+                            break;
+                        }
                     } catch {
                         continue;
                     }
                 }
             }
 
             // get result ans parse
```

### Comparing `nodered.py-0.2.4/setup.py` & `nodered.py-0.2.5/setup.py`

 * *Files identical despite different names*

