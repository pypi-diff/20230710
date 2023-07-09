# Comparing `tmp/BB-DirTree-0.1.7.tar.gz` & `tmp/bb_dirtree-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BB-DirTree-0.1.7.tar", max compression
+gzip compressed data, was "bb_dirtree-0.2.1.tar", max compression
```

## Comparing `BB-DirTree-0.1.7.tar` & `bb_dirtree-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.909235 BB-DirTree-0.1.7/LICENSE
--rw-r--r--   0        0        0     3711 2022-06-07 10:17:46.311101 BB-DirTree-0.1.7/README.md
--rw-r--r--   0        0        0     3804 2022-05-17 06:52:43.000000 BB-DirTree-0.1.7/bbdirtree/COLORS.py
--rw-r--r--   0        0        0     3419 2022-06-07 10:11:10.856088 BB-DirTree-0.1.7/bbdirtree/__init__.py
--rw-r--r--   0        0        0    14387 2022-06-07 10:17:28.480436 BB-DirTree-0.1.7/bbdirtree/__main__.py
--rw-r--r--   0        0        0      495 2022-06-07 10:10:54.035430 BB-DirTree-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4496 2022-06-07 10:30:48.268873 BB-DirTree-0.1.7/setup.py
--rw-r--r--   0        0        0     4185 2022-06-07 10:30:48.269408 BB-DirTree-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3713 2022-07-19 03:55:14.000000 bb_dirtree-0.2.1/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.2.1/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0     3419 2023-07-09 18:22:47.243423 bb_dirtree-0.2.1/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    15995 2023-07-09 19:30:42.350166 bb_dirtree-0.2.1/bbdirtree/__main__.py
+-rw-r--r--   0        0        0      554 2023-07-09 19:31:47.003501 bb_dirtree-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 bb_dirtree-0.2.1/PKG-INFO
```

### Comparing `BB-DirTree-0.1.7/LICENSE` & `bb_dirtree-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BB-DirTree-0.1.7/README.md` & `bb_dirtree-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ## License
 ==========
 
 <pre>
     MIT License
 
-    Copyright (c) [year] [fullname]
+    Copyright (c) [2022] [Erik Beebe]
 
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:
```

### Comparing `BB-DirTree-0.1.7/bbdirtree/COLORS.py` & `bb_dirtree-0.2.1/bbdirtree/COLORS.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,19 +69,19 @@
 
 def C_pi():
     """ Light Purple **italic** """
     return '\x1b[0;35;3m'
 
 def C_r():
     """ Light Red """
-    return '\x1b[0;30;23m'
+    return '\x1b[1;31;23m'
 
 def C_ri():
     """ Light Red **italic** """
-    return '\x1b[0;30;23m'
+    return '\x1b[1;31;23m'
 
 def C_W():
     """ White """
     return '\x1b[1;37;23m'
 
 def C_Wi():
     """ White **italic** """
@@ -127,15 +127,15 @@
     """ Red **italic** """
     return '\x1b[0;31;3m'
 
 def C_Y():
     """ Yellow """
     return '\x1b[1;33;23m'
 
-def C_Yi():
+def C_Y():
     """ Yellow **italic** """
     return '\x1b[1;33;3m'
 
 def F_B():
     """ Bold """
     return '\x1b[1m'
 
@@ -205,15 +205,15 @@
      n = column number
     """
     return f'\x1b[{n}G'
 
 def c_CLEAR(n=1):
     """
      Clear
-     n = 1 - line  -  -  -  -default
+     n = 1 - current line   [default]
      n = 2 - left of cursor
      n = 3 - right of cursor
      n = 4 - screen
     """
     if n == 1:
         return '\x1b[K'
     elif n == 2:
```

### Comparing `BB-DirTree-0.1.7/bbdirtree/__init__.py` & `bb_dirtree-0.2.1/bbdirtree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.7'
+__version__ = '0.2.0'
 
 __doc__="""
 Create a nice looking directory tree
 
 Installation:
 =============
```

### Comparing `BB-DirTree-0.1.7/bbdirtree/__main__.py` & `bb_dirtree-0.2.1/bbdirtree/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,46 @@
-
 import sys, os, ctypes
+from configparser import ConfigParser
 from re import match
-from os.path import isdir, isfile, islink, join, basename
-from os.path import join, isfile, isdir
+from os.path import ( isdir,
+                      isfile,
+                      islink,
+                      join,
+                      basename,
+                      dirname )
 from .COLORS import *
+from . import __init__
+                #__init__ as main_init )
+
+__doc__ = __init__.__doc__
 
 class DirTree:
     """
     Create and print a directory tree from the given directory
-        dotfiles = [default] False -don't show
+        directory     = directory to create tree of [default current dir]
+        depth         = depth of directory to recurse into [default 999999]
+        dotfiles      = show/not show hidden files [default False]
+        exclude_dirs  = directories to ignore
+        exclude files = files to ignore
+        regex_ex      = regex format of files to exclude
+        regex_in      = regex format to only include files
+        title         = title for top of directory tree [default 'BB-DirTree']
+                          - detects 'git' and 'python project' directories to title automatically
+                          - can be 'None'
     """
 
     def __init__( self,
                   directory     = None,
                   depth         = 999999, *,
                   dotfiles      = False,
                   exclude_dirs  = [],
                   exclude_files = [],
                   regex_ex      = [],
-                  regex_in      = [] ):
+                  regex_in      = [],
+                  title         = 'BB-DirTree' ):
 
         if not directory:
             directory = os.getcwd()
 
         elif not isdir( directory ):
             try:
                 assert isdir( join( os.getcwd(), directory ))
@@ -33,35 +51,34 @@
         self.base_dir      = directory
         self.depth         = depth
         self.dotfiles      = dotfiles
         self.regex_ex      = regex_ex
         self.regex_in      = regex_in
         self.exclude_dirs  = exclude_dirs
         self.exclude_files = exclude_files
+        self.title         = title
 
         self.__getBase()
 
     def __getBase(self):
         """
         Recursive scan of base directory
-
             Returns layered dictionary { 'dirs': {}, 'files': [] }
         """
         @staticmethod
         def create_subdir():
             subdir = { 'dirs' : {},
                        'files': [] }
             return subdir
 
         base_dir     = self.base_dir
         dotfiles     = self.dotfiles
         scandirs     = []
         self.listing = create_subdir()
 
-
         @staticmethod
         def iterDir(directory):
             def has_hidden_attr(filepath):
                 try:
                     attrs = ctypes.windll.kernel32.GetFileAttributesW(unicode(filepath))
                     assert attrs != -1
                     result = bool(attrs & 2)
@@ -151,46 +168,48 @@
 
             return True
 
     def list_tty(self):
         """
         Return directory tree formatted for terminal view
         """
-        _FORMAT = { 'dir'   : f"{C_b()}_-_{C__()}",     # blue
-                    'text'  : f"{C_Gr()}_-_{C__()}",    # dark gray
-                    'file'  : f"{C_gri()}_-_{C__()}",   # italic gray
-                    'tree'  : f"{C_g()}_-_{C__()}",     # green
-                    'pre'   : f"\n{C_W()}    {F_U()}Base Directory{C__()}",
-                    'post'  : "",
-                    'nl'    : '\n' }
+        _FORMAT = { 'dir'    : f"{C_b()}_-_{C__()}",     # blue
+                    'dirname': f"{C_c()}_-_{C__()}",     # light cyan
+                    'text'   : f"{C_Gr()}_-_{C__()}",    # dark gray
+                    'file'    : f"{C_gri()}_-_{C__()}",  # italic gray
+                    'tree'   : f"{C_g()}_-_{C__()}",     # green
+                    'pre'    : f"\n{C_W()}    {F_U()}_-_{C__()}",
+                    'post'   : "",
+                    'nl'     : '\n' }
 
         self.__getBase()
-        list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir )
+        list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir, self.title )
 
         return list_tree
 
     def list_gui(self):
         """
         Return directory tree in html formatting
         """
-        _FORMAT = { 'dir'   : "<font color=\"cyan\" >_-_</font>",          # cyan
-                    'text'  : "<font color=\"gray\" >_-_</font>",          # gray
-                    'file'  : "<font color=\"gray\" >_-_</font>",          # light gray
-                    'tree'  : "<font color=\"green\" >_-_</font>",         # green
-                    'pre'   : "<pre><font color: white;>  <u>Base Directory</u></font>",
-                    'post'  : "</pre>",
-                    'nl'    : "<br>" }
+        _FORMAT = { 'dir'    : "<font color=\"Cyan\" >_-_</font>",          # cyan
+                    'dirname': "<font color=\"Aquamarine\" >_-_</font>",    # cyan
+                    'text'   : "<font color=\"Gray\" >_-_</font>",          # gray
+                    'file'    : "<font color=\"Gray\" >_-_</font>",         # light gray
+                    'tree'   : "<font color=\"Green\" >_-_</font>",         # green
+                    'pre'    : "<pre><font color: White;>  <u>_-_</u></font>",
+                    'post'   : "</pre>",
+                    'nl'     : "<br>" }
 
         self.__getBase()
-        list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir )
+        list_tree = self.get_tree( self.listing, _FORMAT, self.base_dir, self.title )
 
         return list_tree
 
     @staticmethod
-    def get_tree( listing, F, skel ):
+    def get_tree( listing, F, skel, TITLE ):
         def tree(f):
             T, B, L = '     ├', '──', '     └'
 
             if f == 'T':
                 return T + B
 
             elif f == 'L':
@@ -221,15 +240,34 @@
                 d.append(( obj['dirs'][i], i ))
 
             f = obj['files']
             f.sort()
 
             return d, f
 
-        Ilist, Plist = [], [ F['pre'], F['dir'].replace('_-_', '      ' + skel + '/'),  ]
+        def get_title(D):
+            title = None
+            dname = D + '/'
+            files = os.listdir(D)
+            if os.system('git rev-parse 2> /dev/null > /dev/null') == 0:
+                title = 'Git Master Directory'
+                dname = basename(D).title()
+            elif set([ 'pyproject.toml', 'setup.py' ]) & set(files):
+                title = 'Python Project'
+                dname = basename(D).title()
+
+            return title, dname
+
+        title, dname = get_title(skel)
+        if not TITLE:
+            title = ''
+        elif not title:
+            title = TITLE
+
+        Ilist, Plist = [], [ F['pre'].replace( '_-_', title ), F['dirname'].replace('_-_', '      ' + dname ),  ]
         form = F
 
         dirs, files = getlist(listing)
         passbar = {0: False}
         level = 1
         passbar[level] = True
         Plist.append( f"{F['tree'].replace('_-_', indentText(level))}" )
@@ -271,15 +309,18 @@
 
                 except IndexError:
                     Plist.append( F['post'] )
                     break
 
         return F['nl'].join(Plist)
 
-if __name__ == "__main__":
+def err(s):
+    print(f"\x1b[1;31m  [ERROR]\x1b[0;1;30;3m {s}\x1b[0m")
+
+def main():
     from getopt import getopt
     from tabulate import tabulate
     from time import sleep
 
     def help_message():
         headers = [ f"{C_W()}Short{C__()}", f"{C_W()}Long{C__()}", f"{C_W()}Description{C__()}" ]
 
@@ -299,21 +340,19 @@
                            C_Y() + i[1] + C__(),
                            C_Gr() + i[2] + C__() ])
 
         tab  = tabulate(table, headers, tablefmt="fancy_grid").split('\n')
 
         _ = f"{C_Gr()}|{C_Y()}"
         print( '\n'.join([ f"\n{C_W()}    {F_U()}DirTree{C__()}",
-                           f"{C_gr()}      Windows:",
-                           f"{C_B()}        py{C_Y()} -m{C_P()} bbdirtree{C_gri()} [OPTIONS]{C_Gri()} [ARGS]{C__()}\n",
-                           f"{C_gr()}      Linux/Mac:",
-                           f"{C_B()}        python{C_Y()} -m{C_P()} bbdirtree{C_gri()} [OPTIONS]{C_Gri()} [ARGS]{C__()}\n",
+                           f"{C_P()}         dirtree{C_gri()} [OPTIONS]{C_Gri()} [ARGS]{C__()}",
+                           '',
                            f"{C_gr()}    {F_U()}Options:{C__()}",
                            "      " + "\n      ".join(tab),
-                           '\n',
+                           '',
                            f"{C_W()}  *{F_U()}Exclusions{F__U()}*{C__()}",
                            f"{C_gri()}      Provide names of files or directories to exclude. To exclude",
                            "    multiple files/directories, quote entire list and seperate",
                            f"    with a colon '{C__()}{C_W()}:{C_gri()}'. Add a '{C__()}{C_W()}/{C_gri()}' to specify a directory name to",
                            "    exclude.\n",
                            "      Example:",
                            f"{C_P()}        bbdirtree{C_Y()} --exclude{C_Gri()} \"excluded dir/:excluded file\"\n",
@@ -352,23 +391,25 @@
         if opt in ('-b', '--base-dir'):
             bdir = arg
             if not isdir(bdir):
                 bdir = join( os.getcwd(), bdir )
                 if isdir(bdir):
                     BASE_DIR = bdir
                 else:
-                    raise FileNotFoundError(f"Can't find directory - '{arg}'")
+                    err(f"Can't find directory - '{arg}'")
+                    return 1
             else:
                 BASE_DIR = arg
 
         elif opt in ('-d', '--depth'):
             try:
                 dpth = int(arg)
             except:
-                raise TypeError("Depth must be an integer")
+                err("Depth must be an integer")
+                return 1
 
             DEPTH = dpth
 
         elif opt in ('-D', '--dotfiles'):
             DOTFILES = True
 
         elif opt in ('-e', '--exclude'):
@@ -386,30 +427,35 @@
             HTML = True
 
         elif opt in ('-r', '--regex'):
             try:
                 m = arg.split('=', 1)[0]
                 reg = arg.split('=', 1)[1]
             except:
-                raise RuntimeError("Invalid format for regex option. See 'dirtree --help'")
+                err("Invalid format for regex option. See 'dirtree --help'")
+                return 1
 
             if m == 'include':
                 REGEX_IN.append(reg)
             elif m == 'exclude':
                 REGEX_EX.append(reg)
             else:
-                raise RuntimeError(f"Invalid regex option '{m}'. See 'dirtree --help'")
+                err(f"Invalid regex option '{m}'. See 'dirtree --help'")
+                return 1
 
     x = DirTree( BASE_DIR,
                  DEPTH,
                  dotfiles = DOTFILES,
                  exclude_dirs = EXCLUDE_DIRS,
                  exclude_files = EXCLUDE_FILES,
                  regex_ex = REGEX_EX,
                  regex_in = REGEX_IN )
 
     if HTML:
         print(x.list_gui())
     else:
         print(x.list_tty())
 
-    sys.exit()
+    return 0
+
+if __name__ == "__main__":
+    sys.exit( exec(main) )
```

### Comparing `BB-DirTree-0.1.7/PKG-INFO` & `bb_dirtree-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.1.7
+Version: 0.2.1
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Description-Content-Type: text/markdown
 
 
 # DirTree
 
 ##### - create a nice looking directory tree
@@ -97,15 +98,15 @@
 
 ## License
 ==========
 
 <pre>
     MIT License
 
-    Copyright (c) [year] [fullname]
+    Copyright (c) [2022] [Erik Beebe]
 
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:
```

