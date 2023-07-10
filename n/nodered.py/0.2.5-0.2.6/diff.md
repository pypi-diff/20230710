# Comparing `tmp/nodered.py-0.2.5.tar.gz` & `tmp/nodered.py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.5.tar", last modified: Mon Jul 10 01:53:21 2023, max compression
+gzip compressed data, was "nodered.py-0.2.6.tar", last modified: Mon Jul 10 09:13:53 2023, max compression
```

## Comparing `nodered.py-0.2.5.tar` & `nodered.py-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.5/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-10 01:53:21.590000 nodered.py-0.2.5/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.5/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       28 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-10 01:53:21.000000 nodered.py-0.2.5/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.5/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      474 2023-07-10 01:13:03.000000 nodered.py-0.2.5/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    14560 2023-07-10 01:46:11.000000 nodered.py-0.2.5/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.5/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.460000 nodered.py-0.2.5/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.5/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.5/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.470000 nodered.py-0.2.5/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.5/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.5/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-06-02 04:29:58.000000 nodered.py-0.2.5/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 01:53:21.470000 nodered.py-0.2.5/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.5/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.5/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4998 2023-07-10 01:49:09.000000 nodered.py-0.2.5/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.5/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-10 01:53:21.590000 nodered.py-0.2.5/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.5/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.580000 nodered.py-0.2.6/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.6/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2575 2023-07-10 09:13:53.640000 nodered.py-0.2.6/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2259 2023-07-10 09:05:46.000000 nodered.py-0.2.6/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.580000 nodered.py-0.2.6/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2575 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-10 09:13:53.000000 nodered.py-0.2.6/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.6/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.580000 nodered.py-0.2.6/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      474 2023-07-10 09:12:12.000000 nodered.py-0.2.6/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    18790 2023-07-10 09:11:19.000000 nodered.py-0.2.6/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.6/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.600000 nodered.py-0.2.6/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.6/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.6/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.600000 nodered.py-0.2.6/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.6/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.6/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-07-10 08:42:28.000000 nodered.py-0.2.6/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-10 09:13:53.600000 nodered.py-0.2.6/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.6/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.6/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4998 2023-07-10 01:49:09.000000 nodered.py-0.2.6/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.6/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-10 09:13:53.640000 nodered.py-0.2.6/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.6/setup.py
```

### Comparing `nodered.py-0.2.5/LICENSE` & `nodered.py-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/PKG-INFO` & `nodered.py-0.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: nodered.py
-Version: 0.2.5
-Summary: make python function to Node-RED node
-Home-page: https://github.com/oyajiDev/NodeRED.py
-Author: oyajiDev
-Author-email: this.dev.somehit@gmail.com
-License: MIT license
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
     NodeRED.py
 </h1>
 <p align="center">
     make python function to Node-RED node
 </p>
 <br/>
@@ -24,14 +12,20 @@
     </a>
     <a href="https://pypi.org/project/nodered.py/">
         <img src="https://img.shields.io/pypi/v/nodered.py.svg" alt="pypi" />
     </a>
 </div>
 <br/><br/>
 
+## 🎛️ requirements
+- node.js 18.16.1 or higher(latest stable)
+  - nodered.py 0.2.6 or higher, automatically download from internet if no node.js installed
+- python 3.7 or higher
+
+<br/><br/>
 
 ## 🌐 install
 ### - using pip
 ```zsh
 python -m pip install nodered.py
 ```
 
@@ -56,18 +50,19 @@
 
 <br/>
 
 ### register Node
 - register as decorator
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
 ```python
+from noderedpy import Node
 from noderedpy.decorator import register
 
 @register("test")
-def test(props:dict, msg:dict) -> dict:
+def test(node:Node, props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
 - register from Node-RED object
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
 ```python
 api = API()
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.5 Summary: make python
-function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
-Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
+## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
+0.2.6 or higher, automatically download from internet if no node.js installed -
+python 3.7 or higher
+
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
 ## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
 "node_red_dir"), "/node-red", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
-function for details ```python from noderedpy.decorator import register
-@register("test") def test(props:dict, msg:dict) -> dict: # user codes here
-return msg ``` - register from Node-RED object - See noredpy.decorator.register
-function for details ```python api = API() red.register("test", api.test) ``` -
-See noderedpy._property for details of "Property" - See example for details.
+function for details ```python from noderedpy import Node from
+noderedpy.decorator import register @register("test") def test(node:Node,
+props:dict, msg:dict) -> dict: # user codes here return msg ``` - register from
+Node-RED object - See noredpy.decorator.register_function for details ```python
+api = API() red.register("test", api.test) ``` - See noderedpy._property for
+details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
 ## Todos [x] type support for "list" and "dict"
 
 ## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.2.5/README.md` & `nodered.py-0.2.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: nodered.py
+Version: 0.2.6
+Summary: make python function to Node-RED node
+Home-page: https://github.com/oyajiDev/NodeRED.py
+Author: oyajiDev
+Author-email: this.dev.somehit@gmail.com
+License: MIT license
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">
     NodeRED.py
 </h1>
 <p align="center">
     make python function to Node-RED node
 </p>
 <br/>
@@ -12,14 +24,20 @@
     </a>
     <a href="https://pypi.org/project/nodered.py/">
         <img src="https://img.shields.io/pypi/v/nodered.py.svg" alt="pypi" />
     </a>
 </div>
 <br/><br/>
 
+## 🎛️ requirements
+- node.js 18.16.1 or higher(latest stable)
+  - nodered.py 0.2.6 or higher, automatically download from internet if no node.js installed
+- python 3.7 or higher
+
+<br/><br/>
 
 ## 🌐 install
 ### - using pip
 ```zsh
 python -m pip install nodered.py
 ```
 
@@ -44,18 +62,19 @@
 
 <br/>
 
 ### register Node
 - register as decorator
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
 ```python
+from noderedpy import Node
 from noderedpy.decorator import register
 
 @register("test")
-def test(props:dict, msg:dict) -> dict:
+def test(node:Node, props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
 - register from Node-RED object
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
 ```python
 api = API()
```

#### html2text {}

```diff
@@ -1,25 +1,35 @@
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6 Summary: make python
+function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
+Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
+## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
+0.2.6 or higher, automatically download from internet if no node.js installed -
+python 3.7 or higher
+
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
 ## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
 "node_red_dir"), "/node-red", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
-function for details ```python from noderedpy.decorator import register
-@register("test") def test(props:dict, msg:dict) -> dict: # user codes here
-return msg ``` - register from Node-RED object - See noredpy.decorator.register
-function for details ```python api = API() red.register("test", api.test) ``` -
-See noderedpy._property for details of "Property" - See example for details.
+function for details ```python from noderedpy import Node from
+noderedpy.decorator import register @register("test") def test(node:Node,
+props:dict, msg:dict) -> dict: # user codes here return msg ``` - register from
+Node-RED object - See noredpy.decorator.register_function for details ```python
+api = API() red.register("test", api.test) ``` - See noderedpy._property for
+details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
 ## Todos [x] type support for "list" and "dict"
 
 ## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.2.5/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.6/nodered.py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.5
+Version: 0.2.6
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -24,14 +24,20 @@
     </a>
     <a href="https://pypi.org/project/nodered.py/">
         <img src="https://img.shields.io/pypi/v/nodered.py.svg" alt="pypi" />
     </a>
 </div>
 <br/><br/>
 
+## 🎛️ requirements
+- node.js 18.16.1 or higher(latest stable)
+  - nodered.py 0.2.6 or higher, automatically download from internet if no node.js installed
+- python 3.7 or higher
+
+<br/><br/>
 
 ## 🌐 install
 ### - using pip
 ```zsh
 python -m pip install nodered.py
 ```
 
@@ -56,18 +62,19 @@
 
 <br/>
 
 ### register Node
 - register as decorator
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/decorator.py#L8">noredpy.decorator.register function</a> for details
 ```python
+from noderedpy import Node
 from noderedpy.decorator import register
 
 @register("test")
-def test(props:dict, msg:dict) -> dict:
+def test(node:Node, props:dict, msg:dict) -> dict:
     # user codes here
     return msg
 ```
 - register from Node-RED object
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
 ```python
 api = API()
```

#### html2text {}

```diff
@@ -1,30 +1,35 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.5 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
+## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
+0.2.6 or higher, automatically download from internet if no node.js installed -
+python 3.7 or higher
+
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
 ## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
 "node_red_dir"), "/node-red", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
-function for details ```python from noderedpy.decorator import register
-@register("test") def test(props:dict, msg:dict) -> dict: # user codes here
-return msg ``` - register from Node-RED object - See noredpy.decorator.register
-function for details ```python api = API() red.register("test", api.test) ``` -
-See noderedpy._property for details of "Property" - See example for details.
+function for details ```python from noderedpy import Node from
+noderedpy.decorator import register @register("test") def test(node:Node,
+props:dict, msg:dict) -> dict: # user codes here return msg ``` - register from
+Node-RED object - See noredpy.decorator.register_function for details ```python
+api = API() red.register("test", api.test) ``` - See noderedpy._property for
+details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
 ## Todos [x] type support for "list" and "dict"
 
 ## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.2.5/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.6/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/noderedpy/_nodered.py` & `nodered.py-0.2.6/noderedpy/_nodered.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,19 +33,88 @@
         editor_theme: dict, default {}
             editorTheme of Node-RED server (for detail information, see https://github.com/node-red/node-red/wiki/Design:-Editor-Themes)
         auths: List[dict], default []
             auth list for Node-RED
         """
         self.user_dir, self.admin_root, self.port, self.show_default_category, self.editor_theme =\
             user_dir, admin_root, port, show_default_category, self.__default_editor_theme(editor_theme)
-        
+        self.__temp_dir, self.__node_dir =\
+            os.path.join(__path__[0], ".temp"), os.path.join(__path__[0], ".nodejs")
+
         if not self.admin_root.startswith("/"):
             self.admin_root = f"/{self.admin_root}"
 
         self.node_auths = self.__default_node_auth(auths)
+
+        # check node.js exists
+        try:
+            subprocess.call(
+                [ "npm", "--version" ],
+                stdout = subprocess.DEVNULL,
+                stderr = subprocess.STDOUT
+            )
+            self.__npm_path = "npm"
+            self.__node_path = "node"
+        except FileNotFoundError:
+            if not os.path.exists(self.__node_dir):
+                import platform, wget, tarfile
+
+                node_version = "18.16.1"
+                if not os.path.exists(self.__temp_dir):
+                    os.mkdir(self.__temp_dir)
+
+                if sys.platform == "win32":
+                    node_bin_zip = os.path.join(self.__temp_dir, "node.zip")
+                    if platform.architecture()[0] == "32bit":
+                        wget.download(f"https://nodejs.org/dist/v{node_version}/node-v{node_version}-win-x86.zip", node_bin_zip)
+                        zipfile.ZipFile(node_bin_zip).extractall(self.__temp_dir)
+                        shutil.move(os.path.join(self.__temp_dir, f"node-v{node_version}-win-x86"), self.__node_dir)
+                    else:
+                        wget.download(f"https://nodejs.org/dist/v{node_version}/node-v{node_version}-win-x64.zip", node_bin_zip)
+                        zipfile.ZipFile(node_bin_zip).extractall(self.__temp_dir)
+                        shutil.move(os.path.join(self.__temp_dir, f"node-v{node_version}-win-x64"), self.__node_dir)
+
+                    self.__npm_path = os.path.join(self.__node_dir, "npm.exe")
+                    self.__node_path = os.path.join(self.__node_dir, "node.exe")
+                elif sys.platform == "darwin":
+                    node_bin_zip = os.path.join(self.__temp_dir, "node.tar.gz")
+                    if platform.processor() == "arm":
+                        wget.download(f"https://nodejs.org/dist/v{node_version}/node-v{node_version}-darwin-arm64.tar.gz", node_bin_zip)
+                        with tarfile.open(node_bin_zip, "r", encoding = "utf-8") as nbzr:
+                            nbzr.extractall(self.__temp_dir)
+
+                        shutil.move(os.path.join(self.__temp_dir, f"node-v{node_version}-darwin-arm64"), self.__node_dir)
+                    else:
+                        wget.download(f"https://nodejs.org/dist/v{node_version}/node-v{node_version}-darwin-x64.tar.gz", node_bin_zip)
+                        with tarfile.open(node_bin_zip, "r", encoding = "utf-8") as nbzr:
+                            nbzr.extractall(self.__temp_dir)
+
+                        shutil.move(os.path.join(self.__temp_dir, f"node-v{node_version}-darwin-x64"), self.__node_dir)
+
+                    self.__npm_path = os.path.join(self.__node_dir, "bin", "npm")
+                    self.__node_path = os.path.join(self.__node_dir, "bin", "node")
+                else:
+                    node_bin_zip = os.path.join(self.__temp_dir, "node.tar.xz")
+                    if platform.processor() == "arm":
+                        wget.download(f"https://nodejs.org/dist/v{node_version}/node-v{node_version}-linux-armv7l.tar.xz", node_bin_zip)
+                        with tarfile.open(node_bin_zip, "r", encoding = "utf-8") as nbzr:
+                            nbzr.extractall(self.__temp_dir)
+
+                        shutil.move(os.path.join(self.__temp_dir, f"node-v{node_version}-linux-armv7l"), self.__node_dir)
+                    else:
+                        wget.download(f"https://nodejs.org/dist/v{node_version}/node-v{node_version}-linux-x64.tar.xz", node_bin_zip)
+                        with tarfile.open(node_bin_zip, "r", encoding = "utf-8") as nbzr:
+                            nbzr.extractall(self.__temp_dir)
+
+                        shutil.move(os.path.join(self.__temp_dir, f"node-v{node_version}-linux-x64"), self.__node_dir)
+
+                shutil.rmtree(self.__temp_dir)
+
+            self.__npm_path = os.path.join(self.__node_dir, "bin", "npm")
+            self.__node_path = os.path.join(self.__node_dir, "bin", "node")
         
         # set node_red_dir
         if node_red_dir is None:
             self.node_red_dir = os.path.join(__path__[0], "node-red-starter")
         else:
             self.node_red_dir = node_red_dir = os.path.realpath(node_red_dir)
             if os.path.exists(node_red_dir):
@@ -56,16 +125,17 @@
             else:
                 os.mkdir(node_red_dir)
                 shutil.copyfile(os.path.join(__path__[0], "node-red-starter", "index.js"), os.path.join(node_red_dir, "index.js"))
                 shutil.copyfile(os.path.join(__path__[0], "node-red-starter", "package.json"), os.path.join(node_red_dir, "package.json"))
 
         # setup Node-RED starter
         subprocess.call(
-            [ "npm", "install" ],
+            [ self.__npm_path, "install" ],
             stdout = subprocess.DEVNULL,
+            stderr = subprocess.STDOUT,
             cwd = self.node_red_dir
         )
 
     # create default editor_theme
     def __default_editor_theme(self, editor_theme:dict):
         page_theme = editor_theme.pop("page", {})
         page_theme.update({
@@ -216,17 +286,17 @@
 
         # create custom nodes
         for node in RED.registered_nodes:
             node.create(self.user_dir, self.__cache_dir)
 
         # run Node-RED server
         subprocess.Popen([
-            "node",
+            self.__node_path,
             "index.js"
-        ], shell = False, stdout = sys.stdout if debug else subprocess.DEVNULL, cwd = self.node_red_dir)
+        ], shell = False, stdout = sys.stdout if debug else subprocess.DEVNULL, stderr = subprocess.STDOUT, cwd = self.node_red_dir)
 
         while True:
             if os.path.exists(self.__started_file):
                 if start_browser:
                     import webbrowser
                     webbrowser.open_new(f"http://127.0.0.1:{self.port}{self.admin_root}")
 
@@ -259,17 +329,17 @@
                 "showDefaultCategory": self.show_default_category,
                 "userCategory": list(set([ node.category for node in RED.registered_nodes ])),
                 "editorTheme": self.editor_theme,
                 "adminAuth": []
             }, cfw, indent = 4)
 
         subprocess.Popen([
-            "node",
+            self.__node_path,
             "index.js"
-        ], shell = False, stdout = subprocess.DEVNULL, cwd = self.node_red_dir)
+        ], shell = False, stdout = subprocess.DEVNULL, stderr = subprocess.STDOUT, cwd = self.node_red_dir)
 
         while True:
             if os.path.exists(self.__started_file):
                 self.stop()
                 break
 
         time.sleep(1)
```

### Comparing `nodered.py-0.2.5/noderedpy/_property.py` & `nodered.py-0.2.6/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/noderedpy/assets/python-logo.png` & `nodered.py-0.2.6/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/noderedpy/decorator.py` & `nodered.py-0.2.6/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.6/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/noderedpy/templates/__init__.py` & `nodered.py-0.2.6/noderedpy/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/noderedpy/templates/template.html` & `nodered.py-0.2.6/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/noderedpy/templates/template.js` & `nodered.py-0.2.6/noderedpy/templates/template.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.5/setup.py` & `nodered.py-0.2.6/setup.py`

 * *Files identical despite different names*

