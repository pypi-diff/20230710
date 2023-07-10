# Comparing `tmp/bdpycmd-1.3.19.tar.gz` & `tmp/bdpycmd-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.3.19.tar", last modified: Mon Jul 10 07:29:05 2023, max compression
+gzip compressed data, was "bdpycmd-1.3.5.tar", last modified: Tue Jun 13 12:39:16 2023, max compression
```

## Comparing `bdpycmd-1.3.19.tar` & `bdpycmd-1.3.5.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-07-10 07:29:05.494526 bdpycmd-1.3.19/
--rw-r--r--   0 zhicheng   (501) staff       (20)     3834 2023-07-10 07:29:05.494612 bdpycmd-1.3.19/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)     3173 2023-07-10 07:28:30.000000 bdpycmd-1.3.19/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2023-07-06 08:35:22.000000 bdpycmd-1.3.19/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      785 2023-07-10 07:29:05.494894 bdpycmd-1.3.19/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-07-10 07:29:05.491018 bdpycmd-1.3.19/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-07-10 07:29:05.491804 bdpycmd-1.3.19/src/bdpycmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.19/src/bdpycmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-07-10 07:29:05.492827 bdpycmd-1.3.19/src/bdpycmd/cmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.19/src/bdpycmd/cmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-07-10 07:29:05.493036 bdpycmd-1.3.19/src/bdpycmd/cmd/camp/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.19/src/bdpycmd/cmd/camp/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     3320 2023-07-06 08:31:38.000000 bdpycmd-1.3.19/src/bdpycmd/cmd/camp/assistant.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-07-10 07:29:05.494253 bdpycmd-1.3.19/src/bdpycmd/cmd/factory/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 17:12:10.000000 bdpycmd-1.3.19/src/bdpycmd/cmd/factory/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     5815 2023-06-13 17:37:07.000000 bdpycmd-1.3.19/src/bdpycmd/cmd/factory/base.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      957 2023-06-14 02:32:50.000000 bdpycmd-1.3.19/src/bdpycmd/cmd/factory/dacmd.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      903 2023-06-14 16:23:24.000000 bdpycmd-1.3.19/src/bdpycmd/cmd/factory/dafunc.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     8463 2023-07-10 07:28:44.000000 bdpycmd-1.3.19/src/bdpycmd/pycmd.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-07-10 07:29:05.492716 bdpycmd-1.3.19/src/bdpycmd.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     3834 2023-07-10 07:29:05.000000 bdpycmd-1.3.19/src/bdpycmd.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      449 2023-07-10 07:29:05.000000 bdpycmd-1.3.19/src/bdpycmd.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-07-10 07:29:05.000000 bdpycmd-1.3.19/src/bdpycmd.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-07-10 07:29:05.000000 bdpycmd-1.3.19/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.965275 bdpycmd-1.3.5/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:39:16.965357 bdpycmd-1.3.5/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.5/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.5/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 12:39:16.965645 bdpycmd-1.3.5/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.962929 bdpycmd-1.3.5/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.963689 bdpycmd-1.3.5/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.5/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964298 bdpycmd-1.3.5/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964479 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.965159 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     4132 2023-06-13 12:39:09.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      937 2023-06-13 12:25:21.000000 bdpycmd-1.3.5/src/bdpycmd/cmd/factory/cmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     8331 2023-06-13 12:39:08.000000 bdpycmd-1.3.5/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 12:39:16.964191 bdpycmd-1.3.5/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 12:39:16.000000 bdpycmd-1.3.5/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.3.19/setup.cfg` & `bdpycmd-1.3.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpycmd
-version = 1.3.19
+version = 1.3.5
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Run Python`s file as command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-cmd
 project_urls =
```

### Comparing `bdpycmd-1.3.19/src/bdpycmd/cmd/camp/assistant.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/camp/assistant.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,88 @@
 # This file is a command execution file generated by the command assistant. 
-# Do not edit it.
+# Please do not modify it
 
-from bdpyconsts import bdpyconsts as pyconst
+import os
+from ..factory import base
 
 # Command Description Information
 _BDCMD_DESC_ = {
     "name":"assistant",
     "alias":"command assistant",
     "desc":"Generate execution commands from existing modules"
 }
 
-
-if pyconst._BD_CMD_RUN_NOW == True:
-    import os
-    from ..factory import base
-
-    class Command(base.BaseCommand):
-        def __init__(self):
-            super().__init__(name=__class__.__module__,alias='command assistant',description='Generate execution commands from existing modules')
-        
-        @base.BaseCommand.as_cmder
-        def make_cmd(self,mpth:str,cls:str,cdir:str,cmd:str,alias:str,desc:str,abs:str="yes",inner:str='false'):
-            """
-            Create a command from a module
-            
-            :param mpth:  str #Module relative path, such as: ./a/b/c
-            :param cls:   str #Class name
-            :param cdir:  str #Relative Directory, such as: ./cmder
-            :param cmd:   str #Command name
-            :param alias: str #command alias
-            :param desc:  str #command description
-            :param abs:   str #Do you want to forcibly replace existing command files. yes/no
-            """
-            if cdir == "./cmd" or cdir == "cmd":
-                raise Exception("The current command storage directory conflicts with the internal command storage directory")
-
-            # Extract Command Name
-            mpth = mpth.replace("\\","/").rstrip("/")
-            mdu = mpth.replace("/",".")
-
-            # Determine if it has the same cmd as a built-in command
-            if not cmd:
-                cmd  = mpth.split("/")[-1]
-            if cmd in self.INNER_CMD:
-                self.format_print("Command name conflicts with built-in commands")
-                return
-            
-            c_fn = "%s.py" % cmd
-            c_fn = cdir.replace("\\","/").rstrip("/") + "/" + c_fn
-
-            if abs != "yes" and os.path.exists(c_fn):
-                self.format_print("command already exists")
-                return
-
-            if inner == 'true':
-                bscmd = '..factory'
-            else:
-                bscmd = 'bdpycmd.cmd.factory'
-            
-            tmp = \
-            f"""
+class Command(base.BaseCommand):
+    def __init__(self):
+        super().__init__(name=__class__.__module__,alias='command assistant',description='Generate execution commands from existing modules')
+    
+    @base.BaseCommand.as_cmder
+    def make_cmd(self,pkg:str,name:str,pdir:str,alias:str,desc:str,inner:str='false'):
+        """
+        Create a command from a module
+        
+        :param pkg:   str #Module package path such as: a.b.c
+        :param name:  str #Module name, without the .py suffix
+        :param pdir:  str #Script storage relative directory
+        :param alias: str #command alias
+        :param desc:  str #command description
+        """
+        # Determine if it has the same name as a built-in command
+        if name in self.INNER_CMD:
+            self.format_print("Command name conflicts with built-in commands")
+            return
+        
+        fn = "%s.py" % name
+        f_fn = pdir.replace("\\","/").rstrip("/") + "/" + fn
+        
+        if os.path.exists(f_fn):
+            self.format_print("command already exists")
+            return
+
+        if inner == 'true':
+            bscmd = '..factory'
+        else:
+            bscmd = 'bdpycmd.cmd.factory'
+        
+        tmp = \
+        """
 # This file is a command execution file generated by the command assistant. 
-# Do not edit it.
+# Please do not modify it
 
-from bdpyconsts import bdpyconsts as pyconst
+from {bscmd} import base
+from {pkg} import {name}
 
 # Command Description Information
-_BDCMD_DESC_ = {{
-    "name":'{cmd}',
+_BDCMD_DESC_ = {
+    "name":'{name}',
     "alias":'{alias}',
     "desc":'{desc}'
-}}
+}
 
-if pyconst._BD_CMD_RUN_NOW == True:
-    from {bscmd}.base import BaseCommand 
-    from {mdu} import {cls}
-
-    class Command(BaseCommand,{cls}):
-        def __init__(self):
-            super().__init__(name=__class__.__module__,alias='{alias}',description='{desc}')
-            super(BaseCommand,self).__init__()
-            """
-            with open(file=c_fn,mode='w',encoding='utf8') as f:
-                f.write(tmp.lstrip())
-            
-            self.format_print("Command created successfully")
-        
-        @base.BaseCommand.as_cmder
-        def test(self,a=1,b=2):
-            """
-            test command
-            
-            :param a: any
-            :param b: any
-            :return:
-            """
-            self.format_print(a,b)
+class Command(base.BaseCommand,{name}.{name}):
+    def __init__(self):
+        super().__init__(name=__class__.__module__,alias='{alias}',description='{desc}')
+        super(base.BaseCommand,self).__init__()
+        """ .format(
+            bscmd=bscmd,
+            pkg=pkg,
+            name=name,
+            alias=alias,
+            desc=desc
+        )
+        with open(file=f_fn,mode='w',encoding='utf8') as f:
+            f.write(tmp.lstrip())
+        
+        self.format_print("Command created successfully")
+    
+    @base.BaseCommand.as_cmder
+    def test(self,a=1,b=2):
+        """
+        test command
+        
+        :param a: any
+        :param b: any
+        :return:
+        """
+        self.format_print(a,b)
```

### Comparing `bdpycmd-1.3.19/src/bdpycmd/cmd/factory/base.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/factory/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from functools import wraps
 from types import FunctionType
-from .dacmd import CmdMeta
-from .dafunc import MethodMeta
+from ..factory.cmd import CmdMeta
 
 # Command Description Information
 _BDCMD_DESC_ = {
     "name":"base",
     "alias":"command base class",
     "desc":"All commands need to inherit from this base class"
 }
@@ -31,23 +30,25 @@
             alias=alias,
             desc=description
         )
         #Methods not shown in the help information
         self.protected_methods = {'__init__','as_cmder'}
 
 
-    def help(self,**kwargs):
+    def help(self,m=''):
         """
         help    Help method, output help information
         """
         tab = """
         """
+        if not isinstance(m,str):
+            m = ''
 
-        #method to run
-        mtds = []
+        #help output command
+        hps = []
 
         #Handling inheritance of command classes
         class_objects = [self.__class__]
         self.deep_clss(self.__class__,class_objects)
 
         #Traverse the object members of the command class and the parent class
         # inherited by the command class to find the command method
@@ -55,99 +56,32 @@
             class_name = class_object.__name__
             for k, v in vars(class_object).items():
                 k = k.replace(class_name + '_', '')
                 if k in self.protected_methods:
                     continue
                 
                 if not k.startswith('_') and isinstance(v,FunctionType) and v.__name__.endswith('___bdcmder'):
-                    mtds.append(MethodMeta(
-                        number=0,
-                        cname=class_name,
-                        name=k,
-                        desc=str(v.__doc__).lstrip(tab)
-                    ))
+                    hps.append(tab + k + '  ' + str(v.__doc__).lstrip(tab))
 
         print(self.info.info())
-        _mtd,info = self.search(mtds=mtds)
-
-        if not _mtd:
-            msg = """
-        Target method not found
-            """
-            print(msg)
-        else:
-            print(info)
-            self.__getattribute__(_mtd)()
-    
-
-    @classmethod
-    def search(self,mtds:list):
-        """
-        Retrieve command list based on keywords
-
-        :param mtds: list[MethodMeta] Method Meta Information List
-        :return: str Target Command
-        """
-        keyword = ""
-        tag_func = ""
-        checked = "/"
-        exited = "."
-        info = ""
-        
-        while True:
-            if keyword == exited:
-                tag_func = ""
-                info = ""
-                break
-            
-            if keyword == checked:
-                break
-            
-            if not keyword:
-                for _cmd in mtds:
-                    tag_func = _cmd.name
-                    info = _cmd.info()
-                    keyword = input(_cmd.say()).strip()
-                    if not keyword:
-                        continue
-                    else:
-                        break
-                else:
-                    break
-            else:
-                _word = keyword
-                for _cmd in mtds:
-                    if _cmd.search(_word):
-                        tag_func = _cmd.name
-                        info = _cmd.info()
-                        keyword = input(_cmd.say()).strip()
-                        if not keyword or keyword == _word:
-                            continue
-                        else:
-                            break
-                else:
-                    break
-        
-        return tag_func,info
-
+        self.format_print(infos=hps)
 
     def deep_clss(self,obj:object,clss:list):
         """
         Recursively complete inherited class query
         
         :param obj: object #initial class
         :param clss: list #target class list
         """
         for it in obj.__bases__:
             if it.__name__ == 'BaseCommand' or it == object:
                 continue
             else:
                 clss.append(it)
                 self.deep_clss(it,clss=clss)
-    
 
     def format_print(self,*args,infos:list=[],ft:bool=True):
         """
         formatted print
         
         :param infos: list #List of information to be printed
         :param ft: bool #Lines beyond the first line are indented
@@ -178,14 +112,19 @@
         @wraps(fun)
         def wrapper(self,**kwargs):
             args_regex = re.compile(r':param\s([\w]+):',re.DOTALL)
             dc = fun.__doc__
             if not dc:
                 dc = ''
             
+            fn = f"""
+        {fun.__name__}
+            """
+            print(fn + dc)
+            
             all_arg_names = args_regex.findall(dc)
             target = {}
             for k in all_arg_names:
                 if k in kwargs:
                     target[k] = kwargs[k]
                 else:
                     vl = input(k + " = ")
```

### Comparing `bdpycmd-1.3.19/src/bdpycmd/cmd/factory/dafunc.py` & `bdpycmd-1.3.5/src/bdpycmd/cmd/factory/cmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 from dataclasses import dataclass
 
 @dataclass
-class MethodMeta:
+class CmdMeta:
     number:int
-    cname:str
     name:str
+    alias:str
     desc:str
 
     def search(self,vl:str="") -> bool:
         """
         Determine if the search matches
 
         :param vl: str search word
         """
         if not vl:
             return False
 
         if vl.isdigit():
             return vl == str(self.number)
         
-        return vl in self.name or vl in self.desc
+        return vl in self.name or vl in self.alias or vl in self.desc
     
 
     def say(self,) -> str:
         """
         Describe information
         """
         return f"""
-        *** method check **************
-        {self.cname} . {self.name}
-                Number: {self.number}
-                {self.desc}  
+        {self.name} ----------------------
+                    {self.alias}
+                    {self.desc}
+                    Number: {self.number}
         """
 
-
     def info(self,) -> str:
         """
         Describe information
         """
         return f"""
-        *** method run ******************
-        {self.cname} . {self.name}
-        {self.desc}
+        {self.name} ++++++++++++++++++++++
+                    {self.alias}
+                    {self.desc}
         """
```

### Comparing `bdpycmd-1.3.19/src/bdpycmd/pycmd.py` & `bdpycmd-1.3.5/src/bdpycmd/pycmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys,traceback,os
 from types import FunctionType
 from importlib import import_module
-from .cmd.factory.dacmd import CmdMeta
-from bdpyconsts import bdpyconsts as pyconst
+from .cmd.factory.cmd import CmdMeta
 
 class CmdBaseConf:
     # project root directory
     __PROJECT_ROOT_DIR = os.path.abspath('.')
     # command script saver relative path
     __CMD_DIR = "cmd"
     # command folder, which can only be a child of the root directory
@@ -45,17 +44,14 @@
         sys.path.append(cls.__PROJECT_ROOT_DIR)
         
         # set command folder
         cls.__CMD_ROOT_DIR = cls.__PROJECT_ROOT_DIR  + "/" + cls.__CMD_DIR
         
         # Set command import path
         cls.__CMD_MODULE_PATH = cls.__CMD_DIR.replace("/", ".")
-
-        # Set to non execution mode
-        pyconst._BD_CMD_RUN_NOW = False
     
     
     @classmethod
     def initialized(cls):
         return cls.__initialized
 
     @classmethod
@@ -209,20 +205,22 @@
         """
         try:
             # Is it an internal command
             is_inner = True if kwargs['cmd'] in cls.__INNER_CMD else False
             modpth = cls.__INNER_CMD_MODEL_PATH if is_inner and __name__ != "__main__" else cls.__CMD_MODULE_PATH
             
             #import command module
-            import importlib
-            cmd = importlib.import_module(modpth + '.' + kwargs['cmd'])
-            importlib.reload(cmd)
+            cmd = __import__(modpth + '.' + kwargs['cmd'], fromlist=['None'])
 
             #Get command execution method
             cmder = cls.find_real_cmder(cmd=cmd.Command,son=kwargs['son'])
+            if kwargs['son'] == 'help':
+                kwargs = {
+                    'm':kwargs['m']
+                }
 
             #run command
             if not cmder:
                 print('{cmd}`s subcommands `{son}` does not exist'.format(cmd=kwargs['cmd'], son=kwargs['son']))
             else:
                 cmder(cmd.Command(),**kwargs)
         except ImportError:
@@ -259,19 +257,17 @@
                 dic_args['cmd'] = 'help'
 
         if dic_args['cmd'] in help_list:
             cls.help()
         else:
             if 'son' not in dic_args or dic_args['son'] in help_list or not dic_args['son']:
                 dic_args['son'] = 'help'
-            
-            # Start Command Execution
-            pyconst.unlock()
-            pyconst._BD_CMD_RUN_NOW = True
-            pyconst.locked()
+                if 'm' not in dic_args:
+                    dic_args['m'] = ''
+
             cls.run_command(**dic_args)
 
 
 # execution entry
 if __name__ == '__main__':
     # initialization
     if not CmdBaseConf.initialized():
```

