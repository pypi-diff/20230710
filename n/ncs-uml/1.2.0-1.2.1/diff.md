# Comparing `tmp/ncs-uml-1.2.0.tar.gz` & `tmp/ncs-uml-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncs-uml-1.2.0.tar", last modified: Sun Jul  9 04:35:20 2023, max compression
+gzip compressed data, was "ncs-uml-1.2.1.tar", last modified: Mon Jul 10 20:14:16 2023, max compression
```

## Comparing `ncs-uml-1.2.0.tar` & `ncs-uml-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.574653 ncs-uml-1.2.0/
--rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.2.0/LICENSE
--rw-r--r--   0 kkotari    (501) staff       (20)       58 2023-07-09 04:23:25.000000 ncs-uml-1.2.0/MANIFEST.in
--rw-r--r--   0 kkotari    (501) staff       (20)    15420 2023-07-09 04:35:20.574446 ncs-uml-1.2.0/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)    14419 2023-07-07 22:58:31.000000 ncs-uml-1.2.0/README.md
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.572449 ncs-uml-1.2.0/ncs_uml/
--rw-r--r--   0 kkotari    (501) staff       (20)      253 2023-07-09 01:46:50.000000 ncs-uml-1.2.0/ncs_uml/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     5171 2023-07-09 04:21:55.000000 ncs-uml-1.2.0/ncs_uml/main.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.573983 ncs-uml-1.2.0/ncs_uml/scripts/
--rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-07 21:00:13.000000 ncs-uml-1.2.0/ncs_uml/scripts/__init__.py
--rw-r--r--   0 kkotari    (501) staff       (20)     3179 2023-07-09 04:22:51.000000 ncs-uml-1.2.0/ncs_uml/scripts/run.py
--rw-r--r--   0 kkotari    (501) staff       (20)     6206 2023-07-09 04:21:24.000000 ncs-uml-1.2.0/ncs_uml/utils.py
-drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-09 04:35:20.573629 ncs-uml-1.2.0/ncs_uml.egg-info/
--rw-r--r--   0 kkotari    (501) staff       (20)    15420 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/PKG-INFO
--rw-r--r--   0 kkotari    (501) staff       (20)      347 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/SOURCES.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/dependency_links.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       87 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/entry_points.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/requires.txt
--rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-07-09 04:35:20.000000 ncs-uml-1.2.0/ncs_uml.egg-info/top_level.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.2.0/requirements.txt
--rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-07-09 04:35:20.574708 ncs-uml-1.2.0/setup.cfg
--rw-r--r--   0 kkotari    (501) staff       (20)     1699 2023-07-07 21:55:17.000000 ncs-uml-1.2.0/setup.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.040436 ncs-uml-1.2.1/
+-rw-r--r--   0 kkotari    (501) staff       (20)    11370 2023-06-23 13:28:47.000000 ncs-uml-1.2.1/LICENSE
+-rw-r--r--   0 kkotari    (501) staff       (20)       58 2023-07-09 04:23:25.000000 ncs-uml-1.2.1/MANIFEST.in
+-rw-r--r--   0 kkotari    (501) staff       (20)    15652 2023-07-10 20:14:16.040256 ncs-uml-1.2.1/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)    14651 2023-07-09 04:49:56.000000 ncs-uml-1.2.1/README.md
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.038224 ncs-uml-1.2.1/ncs_uml/
+-rw-r--r--   0 kkotari    (501) staff       (20)      253 2023-07-10 19:47:27.000000 ncs-uml-1.2.1/ncs_uml/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     5258 2023-07-10 20:09:01.000000 ncs-uml-1.2.1/ncs_uml/main.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.039392 ncs-uml-1.2.1/ncs_uml/plugins/
+-rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-10 19:04:44.000000 ncs-uml-1.2.1/ncs_uml/plugins/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)    45628 2023-07-10 19:45:13.000000 ncs-uml-1.2.1/ncs_uml/plugins/uml_patch.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.040046 ncs-uml-1.2.1/ncs_uml/scripts/
+-rw-r--r--   0 kkotari    (501) staff       (20)        0 2023-07-07 21:00:13.000000 ncs-uml-1.2.1/ncs_uml/scripts/__init__.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     2985 2023-07-10 19:52:41.000000 ncs-uml-1.2.1/ncs_uml/scripts/run.py
+-rw-r--r--   0 kkotari    (501) staff       (20)     6206 2023-07-09 04:21:24.000000 ncs-uml-1.2.1/ncs_uml/utils.py
+drwxr-xr-x   0 kkotari    (501) staff       (20)        0 2023-07-10 20:14:16.039120 ncs-uml-1.2.1/ncs_uml.egg-info/
+-rw-r--r--   0 kkotari    (501) staff       (20)    15652 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/PKG-INFO
+-rw-r--r--   0 kkotari    (501) staff       (20)      404 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/SOURCES.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        1 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/dependency_links.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       87 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/entry_points.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/requires.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)        8 2023-07-10 20:14:15.000000 ncs-uml-1.2.1/ncs_uml.egg-info/top_level.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       13 2023-06-24 00:36:25.000000 ncs-uml-1.2.1/requirements.txt
+-rw-r--r--   0 kkotari    (501) staff       (20)       38 2023-07-10 20:14:16.040490 ncs-uml-1.2.1/setup.cfg
+-rw-r--r--   0 kkotari    (501) staff       (20)     1699 2023-07-10 15:28:57.000000 ncs-uml-1.2.1/setup.py
```

### Comparing `ncs-uml-1.2.0/LICENSE` & `ncs-uml-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.2.0/PKG-INFO` & `ncs-uml-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.2.0
+Version: 1.2.1
 Summary: The ncs-uml creates plantUML files for the given YANG file and its dependencies
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
@@ -50,31 +50,34 @@
 ```sh
 Usage: ncs-uml [options] [<filename>...]
 
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins.
 
 Options:
-  -h, --help       Show this help message and exit
-  -v, --version    Show version number and exit
+  -h, --help            Show this help message and exit
+  -v, --version         Show version number and exit
   -V, --verbose
-  --skip=SKIP      skip given yang modules
+  --skip=SKIP           skip given yang modules
   --skip-grouping
-  --dpath=DPATH    dependent yang module paths
+  --dpath=DPATH         dependent yang module paths
+  --skip-module=SKIP MODULE
+                        skips given modules, i.e., --skip-module=tailf-ncs
+  --add-legend          Adds legend about grouping yang file in the UML
 ```
 
 ## Docs
 
 **How to use ncs-uml?**
 
 - Command Line  
   Type `ncs-uml <YangFile>`. For more help type `ncs-uml --help`
 
 ```shell
-user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang
+user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --skip-module=tailf-ncs --add-legend
  INFO |   main | uml file: l3vpn.uml
  INFO |   main | uml clean up done.
 user$
 ```
 
 It returns plantUML code, which can easily converted to image.
```

### Comparing `ncs-uml-1.2.0/README.md` & `ncs-uml-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,34 @@
 ```sh
 Usage: ncs-uml [options] [<filename>...]
 
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins.
 
 Options:
-  -h, --help       Show this help message and exit
-  -v, --version    Show version number and exit
+  -h, --help            Show this help message and exit
+  -v, --version         Show version number and exit
   -V, --verbose
-  --skip=SKIP      skip given yang modules
+  --skip=SKIP           skip given yang modules
   --skip-grouping
-  --dpath=DPATH    dependent yang module paths
+  --dpath=DPATH         dependent yang module paths
+  --skip-module=SKIP MODULE
+                        skips given modules, i.e., --skip-module=tailf-ncs
+  --add-legend          Adds legend about grouping yang file in the UML
 ```
 
 ## Docs
 
 **How to use ncs-uml?**
 
 - Command Line  
   Type `ncs-uml <YangFile>`. For more help type `ncs-uml --help`
 
 ```shell
-user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang
+user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --skip-module=tailf-ncs --add-legend
  INFO |   main | uml file: l3vpn.uml
  INFO |   main | uml clean up done.
 user$
 ```
 
 It returns plantUML code, which can easily converted to image.
```

### Comparing `ncs-uml-1.2.0/ncs_uml/main.py` & `ncs-uml-1.2.1/ncs_uml/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,16 +104,17 @@
 
         self.log.debug("file {file} exists, fetching dependencies")
         file = Path(yf).expanduser().absolute()
         self.copy(self.get_dependencies(file))
         self.generate_umlfile(cmd, file)
 
     def generate_umlfile(self, cmd, file):
+        path = Path(__file__).absolute().parent.as_posix()
         uml_file = f"{file.stem}.uml"
-        cmd += f" -f uml {file} --path={self.ncs_uml}"
+        cmd += f" --plugindir={path}/plugins/ -f uml {file} --path={self.ncs_uml}"
         cmd += f" --uml-no=module,import,annotation"
         if not self.opt.skip_grouping:
             cmd += f" --uml-inline-groupings "
         if getattr(self.opt, 'skip_module', False):
             cmd += f"--uml-skip-module={','.join(self.opt.skip_module)} "
         if getattr(self.opt, 'add_legend', False):
             cmd += f"--uml-add-legend "
```

### Comparing `ncs-uml-1.2.0/ncs_uml/scripts/run.py` & `ncs-uml-1.2.1/ncs_uml/scripts/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,15 @@
                              metavar="SKIP MODULE",
                              help="skips given modules, i.e., --skip-module=tailf-ncs"),
         optparse.make_option("--add-legend",
                              dest="add_legend",
                              action="store_true",
                              help="Adds legend about grouping yang file in the UML"),
     ]
-    try:
-        cmd = Command(allow_log=False)
-        help = cmd.run(['pyang', '--help'])
-        if '--uml-skip-module' in help:
-            return addl_opt
-    except Exception as e:
-        pass
-    return []
+    return addl_opt
 
 def get_options():
     usage = f"""{ncs_uml.__name__} [options] [<filename>...]
 
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins."""
```

### Comparing `ncs-uml-1.2.0/ncs_uml/utils.py` & `ncs-uml-1.2.1/ncs_uml/utils.py`

 * *Files identical despite different names*

### Comparing `ncs-uml-1.2.0/ncs_uml.egg-info/PKG-INFO` & `ncs-uml-1.2.1/ncs_uml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncs-uml
-Version: 1.2.0
+Version: 1.2.1
 Summary: The ncs-uml creates plantUML files for the given YANG file and its dependencies
 Home-page: https://github.com/kirankotari/ncs-uml.git
 Author: Kiran Kumar Kotari
 Author-email: kirankotari@live.com
 License: UNKNOWN
 Keywords: ncs-uml,ncs_uml
 Platform: UNKNOWN
@@ -50,31 +50,34 @@
 ```sh
 Usage: ncs-uml [options] [<filename>...]
 
 Creates plantUML file for the YANG module in <filename>, and all its dependencies.
 It can be converted into PNG/SVG images using www.plantuml.com or with editor plugins.
 
 Options:
-  -h, --help       Show this help message and exit
-  -v, --version    Show version number and exit
+  -h, --help            Show this help message and exit
+  -v, --version         Show version number and exit
   -V, --verbose
-  --skip=SKIP      skip given yang modules
+  --skip=SKIP           skip given yang modules
   --skip-grouping
-  --dpath=DPATH    dependent yang module paths
+  --dpath=DPATH         dependent yang module paths
+  --skip-module=SKIP MODULE
+                        skips given modules, i.e., --skip-module=tailf-ncs
+  --add-legend          Adds legend about grouping yang file in the UML
 ```
 
 ## Docs
 
 **How to use ncs-uml?**
 
 - Command Line  
   Type `ncs-uml <YangFile>`. For more help type `ncs-uml --help`
 
 ```shell
-user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang
+user$ ncs-uml $NCS_DIR/examples.ncs/getting-started/developing-with-ncs/17-mpls-vpn-python/packages/l3vpn/src/yang/l3vpn.yang --skip-module=tailf-ncs --add-legend
  INFO |   main | uml file: l3vpn.uml
  INFO |   main | uml clean up done.
 user$
 ```
 
 It returns plantUML code, which can easily converted to image.
```

### Comparing `ncs-uml-1.2.0/setup.py` & `ncs-uml-1.2.1/setup.py`

 * *Files identical despite different names*

