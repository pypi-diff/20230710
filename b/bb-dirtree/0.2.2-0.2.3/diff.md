# Comparing `tmp/bb_dirtree-0.2.2.tar.gz` & `tmp/bb_dirtree-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.2.2.tar", max compression
+gzip compressed data, was "bb_dirtree-0.2.3.tar", max compression
```

## Comparing `bb_dirtree-0.2.2.tar` & `bb_dirtree-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.2/LICENSE
--rw-r--r--   0        0        0     3828 2023-07-09 22:45:35.687053 bb_dirtree-0.2.2/README.md
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.2/bbdirtree/COLORS.py
--rw-r--r--   0        0        0     3419 2023-07-09 18:22:47.243423 bb_dirtree-0.2.2/bbdirtree/__init__.py
--rw-r--r--   0        0        0    15995 2023-07-09 19:30:42.350166 bb_dirtree-0.2.2/bbdirtree/__main__.py
--rw-r--r--   0        0        0      554 2023-07-09 22:45:48.697053 bb_dirtree-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 bb_dirtree-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3926 2023-07-10 00:01:14.767139 bb_dirtree-0.2.3/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.3/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0     3419 2023-07-10 00:01:45.007139 bb_dirtree-0.2.3/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    18132 2023-07-10 00:04:24.760475 bb_dirtree-0.2.3/bbdirtree/__main__.py
+-rw-r--r--   0        0        0      554 2023-07-10 00:01:51.297139 bb_dirtree-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4451 1970-01-01 00:00:00.000000 bb_dirtree-0.2.3/PKG-INFO
```

### Comparing `bb_dirtree-0.2.2/LICENSE` & `bb_dirtree-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.2/README.md` & `bb_dirtree-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,16 @@
 ```bash
 python -m pip install "BB-DirTree"
 ```
 
 ## DirTree usage
 ================
 
-##### _**Windows:**_
-
 ```bash
-py -m bbdirtree [OPTIONS] [ARGS]
-```
-
-##### _**Linux/Mac:**_
-
-```bash
-python -m bbdirtree [OPTIONS] [ARGS]
+dirtree [OPTIONS] [ARGS]
 ```
 
 ### _**Options:**_
 
 **Short**  | **Long**       | **Description**
 ---------- | -------------- | ---------------------------------------------------------
 -b         |   --base-dir   |  Set base directory <br> *Uses current directory if not specified*
@@ -135,10 +127,17 @@
 #### v0.1.7 - 6-7-2022
 
 - changed color of files in html output
 - small changes to output format
 
 #### v0.2.2 - 7-9-2023
 
-- added script to run from $PATH
+- added script to run from $PATH (run with 'dirtree')
 - cleaned up code
 - changed header text at top of output
+
+#### v0.2.3 - 7-9-2023
+
+- added python project titles to output
+    - searches for pyproject.toml or setup.py
+- added git project titles to output
+    - searches for .SRCINFO file
```

### Comparing `bb_dirtree-0.2.2/bbdirtree/COLORS.py` & `bb_dirtree-0.2.3/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.2.2/bbdirtree/__init__.py` & `bb_dirtree-0.2.3/bbdirtree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.0'
+__version__ = '0.2.3'
 
 __doc__="""
 Create a nice looking directory tree
 
 Installation:
 =============
```

### Comparing `bb_dirtree-0.2.2/bbdirtree/__main__.py` & `bb_dirtree-0.2.3/bbdirtree/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from re import match
 from os.path import ( isdir,
                       isfile,
                       islink,
                       join,
                       basename,
                       dirname )
+from glob import glob
 from .COLORS import *
 from . import __init__
                 #__init__ as main_init )
 
 __doc__ = __init__.__doc__
 
 class DirTree:
@@ -171,15 +172,15 @@
     def list_tty(self):
         """
         Return directory tree formatted for terminal view
         """
         _FORMAT = { 'dir'    : f"{C_b()}_-_{C__()}",     # blue
                     'dirname': f"{C_c()}_-_{C__()}",     # light cyan
                     'text'   : f"{C_Gr()}_-_{C__()}",    # dark gray
-                    'file'    : f"{C_gri()}_-_{C__()}",  # italic gray
+                    'file'   : f"{C_gri()}_-_{C__()}",   # italic gray
                     'tree'   : f"{C_g()}_-_{C__()}",     # green
                     'pre'    : f"\n{C_W()}    {F_U()}_-_{C__()}",
                     'post'   : "",
                     'nl'     : '\n' }
 
         self.__getBase()
         list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir, self.title )
@@ -241,33 +242,87 @@
 
             f = obj['files']
             f.sort()
 
             return d, f
 
         def get_title(D):
-            title = None
-            dname = D + '/'
-            files = os.listdir(D)
-            if os.system('git rev-parse 2> /dev/null > /dev/null') == 0:
-                title = 'Git Master Directory'
-                dname = basename(D).title()
-            elif set([ 'pyproject.toml', 'setup.py' ]) & set(files):
-                title = 'Python Project'
-                dname = basename(D).title()
-
-            return title, dname
-
-        title, dname = get_title(skel)
-        if not TITLE:
-            title = ''
-        elif not title:
-            title = TITLE
+            def findPyProjectName(D):           # Search for python project name
+                cd = D
+                name = None
+                file, file_lines = None, []
+                while True:
+                    if cd == os.path.expanduser('~') or cd == os.path.sep:
+                        return ''
+
+                    files = os.listdir(cd)
+                    if 'pyproject.toml' in files:
+                        file = join( cd, 'pyproject.toml' )
+                    elif 'setup.py' in files:
+                        file = join( cd, 'setup.py' )
+
+                    if file:
+                        with open( file, 'r' ) as f:
+                            file_lines = [ i.strip() for i in f.read().strip().split('\n') ]
+
+                        for line in file_lines:
+                            if line.startswith('name'):
+                                name = line.split('=')[1].replace('"', '').replace("'", '').strip()
+                                return name
+
+                        if not name:
+                            return 'Python Project'
+
+                    else:
+                        cd = dirname(cd)
+
+            def findGitProjectName(D):           # Search for git project name
+                cd = D
+                name = None
+                while True:
+                    if cd == os.path.expanduser('~') or cd == os.path.sep:
+                        return ''
+
+                    files = os.listdir(cd)
+                    if '.SRCINFO' in files:
+                        file = join( cd, '.SRCINFO' )
+                        with open( file, 'r' ) as f:
+                            file_lines = [ i.strip() for i in f.read().strip().split('\n') ]
+
+                        for line in file_lines:
+                            if line.startswith('pkgbase'):
+                                name = line.split('=')[1].replace('"', '').replace("'", '').strip()
+                                return name
+
+                        if not name:
+                            return 'Git Project'
+
+                    else:
+                        cd = dirname(cd)
+
+            name = findPyProjectName(D)
+            if name:
+                return f"Python Project:\x1b[0;0;33m {name}"
+
+            name = findGitProjectName(D)
+            if name:
+                return f"Git Project:\x1b[0;0;33m {name}"
+
+            return ''
+
+        title = get_title(skel)
+        if not title:
+            if os.getcwd() == os.path.expanduser('~'):
+                title = f'Home Directory:\x1b[0;0;33m {basename(cd).title()}'
+            elif TITLE:
+                title = TITLE
+            else:
+                title = 'BB-DirTree'
 
-        Ilist, Plist = [], [ F['pre'].replace( '_-_', title ), F['dirname'].replace('_-_', '      ' + dname ),  ]
+        Ilist, Plist = [], [ F['pre'].replace( '_-_', title ), F['dirname'].replace('_-_', '      ' + skel + os.path.sep ) ]
         form = F
 
         dirs, files = getlist(listing)
         passbar = {0: False}
         level = 1
         passbar[level] = True
         Plist.append( f"{F['tree'].replace('_-_', indentText(level))}" )
```

### Comparing `bb_dirtree-0.2.2/pyproject.toml` & `bb_dirtree-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.2.2"
+version = "0.2.3"
 description = "Create a nice looking directory tree with options"
 authors = ["Erik Beebe <beebeapps_feedback@tuta.io>"]
 license = "MIT"
 packages = [ { include = 'bbdirtree' } ]
 readme = "README.md"
 
 keywords = [ "script", "qt", "files" ]
```

### Comparing `bb_dirtree-0.2.2/PKG-INFO` & `bb_dirtree-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -34,24 +34,16 @@
 ```bash
 python -m pip install "BB-DirTree"
 ```
 
 ## DirTree usage
 ================
 
-##### _**Windows:**_
-
 ```bash
-py -m bbdirtree [OPTIONS] [ARGS]
-```
-
-##### _**Linux/Mac:**_
-
-```bash
-python -m bbdirtree [OPTIONS] [ARGS]
+dirtree [OPTIONS] [ARGS]
 ```
 
 ### _**Options:**_
 
 **Short**  | **Long**       | **Description**
 ---------- | -------------- | ---------------------------------------------------------
 -b         |   --base-dir   |  Set base directory <br> *Uses current directory if not specified*
@@ -151,11 +143,18 @@
 #### v0.1.7 - 6-7-2022
 
 - changed color of files in html output
 - small changes to output format
 
 #### v0.2.2 - 7-9-2023
 
-- added script to run from $PATH
+- added script to run from $PATH (run with 'dirtree')
 - cleaned up code
 - changed header text at top of output
 
+#### v0.2.3 - 7-9-2023
+
+- added python project titles to output
+    - searches for pyproject.toml or setup.py
+- added git project titles to output
+    - searches for .SRCINFO file
+
```

