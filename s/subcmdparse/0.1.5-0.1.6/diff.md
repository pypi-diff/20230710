# Comparing `tmp/subcmdparse-0.1.5.tar.gz` & `tmp/subcmdparse-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subcmdparse-0.1.5.tar", last modified: Sun Jun 11 13:04:16 2023, max compression
+gzip compressed data, was "subcmdparse-0.1.6.tar", last modified: Mon Jul 10 08:38:23 2023, max compression
```

## Comparing `subcmdparse-0.1.5.tar` & `subcmdparse-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-06-11 13:04:16.660330 subcmdparse-0.1.5/
--rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-06-11 13:04:16.660062 subcmdparse-0.1.5/PKG-INFO
--rw-r--r--   0 dhkim      (501) staff       (20)       60 2022-06-19 07:33:30.000000 subcmdparse-0.1.5/README.md
--rw-r--r--   0 dhkim      (501) staff       (20)       38 2023-06-11 13:04:16.660431 subcmdparse-0.1.5/setup.cfg
--rw-r--r--   0 dhkim      (501) staff       (20)     1219 2023-06-11 13:04:03.000000 subcmdparse-0.1.5/setup.py
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-06-11 13:04:16.654997 subcmdparse-0.1.5/src/
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-06-11 13:04:16.657129 subcmdparse-0.1.5/src/subcmdparse/
--rw-r--r--   0 dhkim      (501) staff       (20)       53 2022-06-19 07:33:30.000000 subcmdparse-0.1.5/src/subcmdparse/__init__.py
--rw-r--r--   0 dhkim      (501) staff       (20)     7546 2023-06-11 13:03:43.000000 subcmdparse-0.1.5/src/subcmdparse/subcmdparse.py
--rw-r--r--   0 dhkim      (501) staff       (20)      300 2022-06-19 07:33:30.000000 subcmdparse-0.1.5/src/subcmdparse/util.py
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-06-11 13:04:16.659187 subcmdparse-0.1.5/src/subcmdparse.egg-info/
--rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-06-11 13:04:16.000000 subcmdparse-0.1.5/src/subcmdparse.egg-info/PKG-INFO
--rw-r--r--   0 dhkim      (501) staff       (20)      320 2023-06-11 13:04:16.000000 subcmdparse-0.1.5/src/subcmdparse.egg-info/SOURCES.txt
--rw-r--r--   0 dhkim      (501) staff       (20)        1 2023-06-11 13:04:16.000000 subcmdparse-0.1.5/src/subcmdparse.egg-info/dependency_links.txt
--rw-r--r--   0 dhkim      (501) staff       (20)       14 2023-06-11 13:04:16.000000 subcmdparse-0.1.5/src/subcmdparse.egg-info/requires.txt
--rw-r--r--   0 dhkim      (501) staff       (20)       12 2023-06-11 13:04:16.000000 subcmdparse-0.1.5/src/subcmdparse.egg-info/top_level.txt
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-06-11 13:04:16.659498 subcmdparse-0.1.5/tests/
--rw-r--r--   0 dhkim      (501) staff       (20)     7227 2022-06-19 07:33:30.000000 subcmdparse-0.1.5/tests/test_subcommand.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.159335 subcmdparse-0.1.6/
+-rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-07-10 08:38:23.158772 subcmdparse-0.1.6/PKG-INFO
+-rw-r--r--   0 dhkim      (501) staff       (20)       60 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/README.md
+-rw-r--r--   0 dhkim      (501) staff       (20)       38 2023-07-10 08:38:23.159527 subcmdparse-0.1.6/setup.cfg
+-rw-r--r--   0 dhkim      (501) staff       (20)     1219 2023-07-10 08:37:47.000000 subcmdparse-0.1.6/setup.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.150925 subcmdparse-0.1.6/src/
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.154292 subcmdparse-0.1.6/src/subcmdparse/
+-rw-r--r--   0 dhkim      (501) staff       (20)       53 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/src/subcmdparse/__init__.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     8407 2023-07-10 08:36:14.000000 subcmdparse-0.1.6/src/subcmdparse/subcmdparse.py
+-rw-r--r--   0 dhkim      (501) staff       (20)      300 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/src/subcmdparse/util.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.157361 subcmdparse-0.1.6/src/subcmdparse.egg-info/
+-rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/PKG-INFO
+-rw-r--r--   0 dhkim      (501) staff       (20)      320 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/SOURCES.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)        1 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/dependency_links.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)       14 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/requires.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)       12 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/top_level.txt
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.157811 subcmdparse-0.1.6/tests/
+-rw-r--r--   0 dhkim      (501) staff       (20)     7227 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/tests/test_subcommand.py
```

### Comparing `subcmdparse-0.1.5/setup.py` & `subcmdparse-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="subcmdparse", # Replace with your own username
-    version="0.1.5",
+    version="0.1.6",
     author="Donghwi Kim",
     author_email="dhkim09@kaist.ac.kr",
     description="Subcommand extension for argparse package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dhkim09a/subcmdparse",
     packages=setuptools.find_packages(where='src'),
```

### Comparing `subcmdparse-0.1.5/src/subcmdparse/subcmdparse.py` & `subcmdparse-0.1.6/src/subcmdparse/subcmdparse.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,30 +27,49 @@
         try:
             super().__call__(parser, namespace, values, *args, **kwargs)
         except argparse.ArgumentError:
             vars(namespace).setdefault(argparse._UNRECOGNIZED_ARGS_ATTR, [])
             getattr(namespace, argparse._UNRECOGNIZED_ARGS_ATTR).extend(values)
 
 
-class _HelpAllAction(argparse.Action):
+class _UsageAllAction(argparse.Action):
 
     def __init__(self,
                  option_strings,
                  dest=argparse.SUPPRESS,
                  default=argparse.SUPPRESS,
                  help=None):
-        super(_HelpAllAction, self).__init__(
+        super(_UsageAllAction, self).__init__(
             option_strings=option_strings,
             dest=dest,
             default=default,
             nargs=0,
             help=help)
 
+    # def print_help(self, parser: argparse.ArgumentParser, file=None, indent=''):
+    #     # message = parser.format_help()
+    #     message = parser.format_usage()
+    #     if indent:
+    #         lines = message.split('\n')
+    #         message = '\n'.join([indent + line for line in lines])
+    #     parser._print_message(message, file)
+
     def __call__(self, parser, namespace, values, option_string=None):
-        parser.print_help()
+        # depth first search
+        stack: list[tuple[SubcommandParser, int]] = []
+        stack.append((parser, 0))
+        while stack and (elm := stack.pop()):
+            parser, level = elm
+            # self.print_help(parser, indent='  ' * level)
+            # self.print_help(parser)
+            parser.print_usage()
+            if parser.subcommands:
+                to_push = [(subcmd.parser, level + 1) for subcmd in parser.subcommands]
+                to_push.reverse()
+                stack.extend(to_push)
         parser.exit()
 
 
 class SubcommandParser(argparse.ArgumentParser):
     subparsers = None
     subcommands: list = None
     parent_shared_parsers: List[argparse.ArgumentParser] = None
@@ -78,17 +97,17 @@
         self.add_help_all = add_help_all
 
         # add help argument if necessary
         # (using explicit default to override global argument_default)
         default_prefix = '-' if '-' in self.prefix_chars else self.prefix_chars[0]
         if self.add_help:
             self.add_argument(
-                default_prefix*2+'help'+default_prefix+'all',
-                action='help', default=argparse.SUPPRESS,
-                help=_('show this help message and exit'))
+                default_prefix*2+'usage'+default_prefix+'all',
+                action=_UsageAllAction, default=argparse.SUPPRESS,
+                help=_('show all subcommand usages recursively'))
 
     def add_subcommands(self, *subcommands, title=None, required=True, help=None, metavar='SUBCOMMAND'):
         if not self.subparsers:
             self.subparsers = self.add_subparsers(
                 **{'title': title} if title else {},
                 required=required,
                 help=help,
@@ -216,7 +235,8 @@
         cmdargs, shargs = compile_shargs(*args, **kwargs)
 
         parser = SubcommandParser()
         parser.add_subcommands(cls(name='subcmd'))
         parserd_args = parser.parse_args(['subcmd', *cmdargs])
 
         parser.exec_subcommands(parserd_args)
+
```

### Comparing `subcmdparse-0.1.5/tests/test_subcommand.py` & `subcmdparse-0.1.6/tests/test_subcommand.py`

 * *Files identical despite different names*

