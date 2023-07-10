# Comparing `tmp/ruamel.yaml.cmd-0.6.3.tar.gz` & `tmp/ruamel.yaml.cmd-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruamel.yaml.cmd-0.6.3.tar", last modified: Thu Sep  1 04:58:12 2022, max compression
+gzip compressed data, was "ruamel.yaml.cmd-0.6.4.tar", last modified: Mon Jul 10 20:43:08 2023, max compression
```

## Comparing `ruamel.yaml.cmd-0.6.3.tar` & `ruamel.yaml.cmd-0.6.4.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2022-09-01 04:58:12.171078 ruamel.yaml.cmd-0.6.3/
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2022-09-01 04:58:12.169972 ruamel.yaml.cmd-0.6.3/.ruamel/
--rw-rw-r--   0 anthon    (1000) users      (500)       63 2017-06-30 04:13:45.000000 ruamel.yaml.cmd-0.6.3/.ruamel/__init__.py
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2022-09-01 04:58:12.170071 ruamel.yaml.cmd-0.6.3/.ruamel/yaml/
--rw-rw-r--   0 anthon    (1000) users      (500)       63 2017-06-30 04:13:45.000000 ruamel.yaml.cmd-0.6.3/.ruamel/yaml/__init__.py
--rw-r--r--   0 anthon    (1000) users      (500)     1121 2022-09-01 04:58:11.000000 ruamel.yaml.cmd-0.6.3/LICENSE
--rw-r--r--   0 anthon    (1000) users      (500)     2446 2022-09-01 04:58:12.170960 ruamel.yaml.cmd-0.6.3/PKG-INFO
--rw-rw-r--   0 anthon    (1000) users      (500)     1844 2022-01-12 10:48:58.000000 ruamel.yaml.cmd-0.6.3/README.rst
--rw-rw-r--   0 anthon    (1000) users      (500)     9939 2022-09-01 04:58:05.000000 ruamel.yaml.cmd-0.6.3/__init__.py
--rw-rw-r--   0 anthon    (1000) users      (500)    33254 2022-09-01 04:44:51.000000 ruamel.yaml.cmd-0.6.3/__main__.py
-drwxr-xr-x   0 anthon    (1000) users      (500)        0 2022-09-01 04:58:12.170809 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/
--rw-r--r--   0 anthon    (1000) users      (500)     2446 2022-09-01 04:58:12.000000 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/PKG-INFO
--rw-r--r--   0 anthon    (1000) users      (500)      428 2022-09-01 04:58:12.000000 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/SOURCES.txt
--rw-r--r--   0 anthon    (1000) users      (500)        1 2022-09-01 04:58:12.000000 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/dependency_links.txt
--rw-r--r--   0 anthon    (1000) users      (500)       55 2022-09-01 04:58:12.000000 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/entry_points.txt
--rw-r--r--   0 anthon    (1000) users      (500)       19 2022-09-01 04:58:12.000000 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/namespace_packages.txt
--rw-r--r--   0 anthon    (1000) users      (500)      100 2022-09-01 04:58:12.000000 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/requires.txt
--rw-r--r--   0 anthon    (1000) users      (500)        7 2022-09-01 04:58:12.000000 ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/top_level.txt
--rw-r--r--   0 anthon    (1000) users      (500)       38 2022-09-01 04:58:12.171114 ruamel.yaml.cmd-0.6.3/setup.cfg
--rw-rw-r--   0 anthon    (1000) users      (500)    35809 2021-10-31 19:58:13.000000 ruamel.yaml.cmd-0.6.3/setup.py
--rw-r--r--   0 anthon    (1000) users      (500)     1358 2021-10-31 20:02:23.000000 ruamel.yaml.cmd-0.6.3/simpleresolver.py
--rw-rw-r--   0 anthon    (1000) users      (500)    42934 2022-09-01 04:47:27.000000 ruamel.yaml.cmd-0.6.3/yaml_cmd.py
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-10 20:43:08.511385 ruamel.yaml.cmd-0.6.4/
+-rw-r--r--   0 anthon    (1000) users      (500)     1121 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/LICENSE
+-rw-r--r--   0 anthon    (1000) users      (500)     2446 2023-07-10 20:43:08.511247 ruamel.yaml.cmd-0.6.4/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)     1844 2022-01-12 10:48:58.000000 ruamel.yaml.cmd-0.6.4/README.rst
+-rw-r--r--   0 anthon    (1000) users      (500)    10649 2023-06-13 21:15:26.000000 ruamel.yaml.cmd-0.6.4/__init__.py
+-rw-r--r--   0 anthon    (1000) users      (500)    39519 2023-06-13 21:15:28.000000 ruamel.yaml.cmd-0.6.4/__main__.py
+-rw-r--r--   0 anthon    (1000) users      (500)     1734 2023-06-17 05:52:40.000000 ruamel.yaml.cmd-0.6.4/analyse.py
+-rw-r--r--   0 anthon    (1000) users      (500)     3986 2023-06-17 05:55:05.000000 ruamel.yaml.cmd-0.6.4/generate.py
+-rw-r--r--   0 anthon    (1000) users      (500)       97 2023-06-08 05:34:02.000000 ruamel.yaml.cmd-0.6.4/pyproject.toml
+drwxr-xr-x   0 anthon    (1000) users      (500)        0 2023-07-10 20:43:08.511078 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/
+-rw-r--r--   0 anthon    (1000) users      (500)     2446 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/PKG-INFO
+-rw-r--r--   0 anthon    (1000) users      (500)      415 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       55 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/entry_points.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        1 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/not-zip-safe
+-rw-r--r--   0 anthon    (1000) users      (500)      100 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/requires.txt
+-rw-r--r--   0 anthon    (1000) users      (500)        7 2023-07-10 20:43:08.000000 ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/top_level.txt
+-rw-r--r--   0 anthon    (1000) users      (500)       38 2023-07-10 20:43:08.511424 ruamel.yaml.cmd-0.6.4/setup.cfg
+-rw-rw-r--   0 anthon    (1000) users      (500)    33384 2023-06-08 05:34:02.000000 ruamel.yaml.cmd-0.6.4/setup.py
+-rw-r--r--   0 anthon    (1000) users      (500)     1358 2021-10-31 20:02:23.000000 ruamel.yaml.cmd-0.6.4/simpleresolver.py
+-rw-r--r--   0 anthon    (1000) users      (500)    45147 2023-07-10 20:30:58.000000 ruamel.yaml.cmd-0.6.4/yaml_cmd.py
```

### Comparing `ruamel.yaml.cmd-0.6.3/LICENSE` & `ruamel.yaml.cmd-0.6.4/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
  The MIT License (MIT)
 
- Copyright (c) 2015-2022 Anthon van der Neut, Ruamel bvba
+ Copyright (c) 2015-2023 Anthon van der Neut, Ruamel bvba
 
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `ruamel.yaml.cmd-0.6.3/PKG-INFO` & `ruamel.yaml.cmd-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.yaml.cmd
-Version: 0.6.3
+Version: 0.6.4
 Summary: commandline utility to manipulate YAML files
 Home-page: https://sourceforge.net/p/ruamel-yaml-cmd/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ruamel.yaml.cmd-0.6.3/README.rst` & `ruamel.yaml.cmd-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.3/__init__.py` & `ruamel.yaml.cmd-0.6.4/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 from __future__ import print_function, absolute_import, division, unicode_literals
 
 _package_data = dict(
     full_package_name='ruamel.yaml.cmd',
-    version_info=(0, 6, 3),
-    __version__='0.6.3',
-    version_timestamp='2022-09-01 06:58:05',
+    version_info=(0, 6, 4),
+    __version__='0.6.4',
+    version_timestamp='2023-06-08 07:34:21',
     author='Anthon van der Neut',
     author_email='a.van.der.neut@ruamel.eu',
     description='commandline utility to manipulate YAML files',
     entry_points='yaml',
     license='MIT',
     since=2015,
     nested=True,
@@ -48,15 +48,16 @@
 # !Action # either one of the actions in subdir _action (by stem of the file) or e.g. "store_action"
 # !Config YAML/INI/PON  read defaults from config file
 # !AddDefaults
 # !Epilog epilog text (for multiline use | )
 # !NQS used on arguments, makes sure the scalar is non-quoted e.g for instance/method/function
 #      call arguments, when cligen knows about what argument a keyword takes, this is not needed
 !Cli 0:
-- !Opt [verbose, v, !Help increase verbosity level, !Action count, const: 1, nargs: 0, default: 0]
+- !AddDefaults
+- !Opt [verbose, v, !Help increase verbosity level, !Action count, const: 1, !Nargs 0, default: 0]
 - !Opt [indent, metavar: IND, !Help 'set indent level (default: auto)']
 - !Opt [bsi, dest: block_seq_indent, metavar: BLOCK_SEQ_IND, type: int, !Help 'set block sequence indent level (default: auto)']
 # - !Opt [map_indent, metavar: M, type: int, !Help 'set indent level for mappings (default: auto)']
 # - !Opt [seq_indent, metavar: M, type: int, !Help 'set indent level for sequences (default: auto)']
 # - !Opt [offset, dest: seq_indicator_offset, metavar: OFFSET, type: int, !Help 'set block sequence indicator offset (default: auto), make sure there is enough space in the sequence indent']
 # options for YAML output 
 - !Opt [flow, !Action store_true, !Help use flow-style YAML instead of block style]
@@ -67,43 +68,44 @@
 - !Opt [smart-string, !Action store_true, !Help set literal block style on strings with \n otherwise plain if possible]
 - !Instance ruamel.yaml.cmd.yaml_cmd.YAMLCommand
 - rt:
   - !Alias round-trip
   - !Prolog round trip on YAML document, test if first or second round stabilizes document
   - !Opt [save, !Action store_true, !Help "save the rewritten data back\n    to the input file (if it doesn't exist a '.orig' backup will be made)\n    "]
   - !Opt [width, metavar: W, default: 80, type: int, !Help 'set width of output (default: %(default)s']
-  - !Arg [file, nargs: +]
+  - !Arg [file, !Nargs +]
   - !Help test round trip on YAML document
 - me:
   - !Alias merge-expand
   - !Prolog expand merges in input file to output file
   - !Opt [allow-anchors, !Action store_true, !Help allow "normal" anchors/aliases in output]
-  - !Arg [file, nargs: 2]
+  - !Arg [file, !Nargs 2]
   - !Help expand merges in input file to output file
 - json:
   - !Alias from-json 
   - !Prolog convert JSON to block-style YAML
   # - !Opt [flow, !Action store_true, !Help use flow-style instead of block style]
   # - !Opt [semi, !Action store_true, !Help write block style except for "leaf" mapping/dict]
   # - !Opt [literal, !Action store_true, !Help convert scalars with newlines to literal block style]
+  - !Opt [width, metavar: W, default: 80, type: int, !Help 'set width of output (default: %(default)s']
   - !Opt [mozlz4, !Action store_true, !Help decode mozilla lz4]
   # - !Opt [write, w, !Action store_true, !Help 'write a  .yaml file, instead of stdout']
-  - !Arg [file, nargs: +]
+  - !Arg [file, !Nargs +]
   - !Help convert JSON to block-style YAML
 - ini:
   - !Alias from-ini
   - !Prolog convert .ini/config file to block YAML
   - !Opt [basename, b, !Action store_true, !Help 're-use basename of .ini file for .yaml file, instead of writing to stdout']
   - !Opt [test, !Action store_true]
   - !Arg [file]
   - !Help convert .ini/config to block YAML
 - pon:
   - !Alias from-pon
   - !Prolog convert .pon config file to block YAML
-  - !Arg [file, nargs: +]
+  - !Arg [file, !Nargs +]
   - !Help convert .pon config file to block YAML
 - htmltable:
   - !Prolog |
       convert YAML to html tables. If hierarchy is two levels deep (
       sequence/mapping over sequence/mapping) this is mapped to one table
       If the hierarchy is three deep, a list of 2 deep tables is assumed, but
       any non-list/mapp second level items are considered text.
@@ -142,22 +144,22 @@
       Combine multiple YAML files into one.
       Path chunks (directories) are converted to mapping entries, the YAML contents
       the value of the (last) key. If there are multiple files in one directory, the
       filenames are used as well (or specify --use-file-name).
   # - !Opt [output, o, !H 'write to file OUTPUT instead of stdout']
   - !Opt [use-file-names, !Action store_true]
   - !Opt [sequence, !Action store_true, !H 'no paths, each YAML content is made an element of a root level sequence']
-  - !Arg [file, nargs: +, !H 'full path names (a/b/data.yaml)']
+  - !Arg [file, !Nargs +, !H 'full path names (a/b/data.yaml)']
   - !Help combine multiple YAML files into one
 - pickle:
   - !Alias [from-pickle, frompickle]
   - !Prolog |
       Load Python pickle file(s) and dump as YAML
   - !Opt [create-to-yaml, !Action store_true, !Help create a tagged to_yaml method even if available]
-  - !Arg [file, nargs: '*']
+  - !Arg [file, !Nargs '*']
   - !Help convert Python pickle file(s) to YAML
 - mapping:
   - !Alias map
   # - !Opt [output, o, !Help write to file OUTPUT instead of stdout]
   - !Arg [key, !Help key of the new root-level mapping]
   - !Arg [file, !Help file with YAML content that will be value for key]
   - !Help create new YAML file with at root a mapping with key and file content
@@ -165,39 +167,57 @@
   - !Option ['parents', !Action store_true, !H create parents if necessary]
   - !Option ['item', !Action store_true, !H 'create item']
   - !Option ['key', !Action store_true, !H 'create key, even if not found in siblings of item']
   - !Option ['str', !Action store_true, !H store value as string]
   - !Option ['file', !H use FILE instead of first argument as YAML file]
   - !Option ['value', !H use FILE instead of first argument as YAML file]
   - !Option ['sep', !H set separator for splitting single element path]
-  - !Arg [args, nargs: '*', !H '[file] path in yaml/path.in.yaml [value]']
+  - !Arg [args, !Nargs '*', !H '[file] path in yaml/path.in.yaml [value]']
   - !Help add a value to a path in the data structure loaded from YAML
   - !Prolog >
      Add a value to a path in the data structure loaded from YAML.
      Use value are resolved like in YAML, use --str if necessary
      The value is the last args token.
      The "path" in the data structure is taken from all other args,
      interpreting numerical values as indices in list/seq.
 
      E.g.:
          yaml add --parents --value Windows test.yaml computers os type
          yaml add --file test.yaml computers os secure false
          yaml add --str test.yaml computers.os.year 2019
 - sort:
   - !Option ['file', !H use FILE instead of first argument as YAML file]
-  - !Arg [args, nargs: '*', !H '[file] [path in yaml/path.in.yaml]']
+  - !Arg [args, !Nargs '*', !H '[file] [path in yaml/path.in.yaml]']
   - !Prolog |
     Load the file, check if path leads to a mapping, sort by key
     and write back. No path -> work on root of data structure.
     File is not written if mapping is already in sorted order.
   - !Help sort the keys of a mapping in a YAML file
 - edit:
   - !Arg [file, !H 'file to edit using $EDITOR']
   - !Help Edit a YAML document, save over orginal only when loadable 
   - !Prolog >
     Edits a copy of the file argument and only updates the file when the copy
     is loadable YAML. The copy is not removed after exiting editor if not
     parseable and used (if not older than the original file) to continue.
 
     Copy is named .ye.<filename>
+- tokens:
+  - !Arg [file, !H 'file to edit using $EDITOR']
+  - !Help show tokens
+- events:
+  - !Arg [file, !H 'file to edit using $EDITOR']
+  - !Help show events
+
+- generate:
+  - !Prolog |
+    generate a file filled with random YAML until it reaches size
+  - !Option [size, default: 10, !Help size in Kb]
+  - !Option [levels, !Help 'levels in file (e.g. sm_s1m) ']
+  - !Arg [file, !H 'name of the file to generate']
+- analyse:
+  - !Option [typ, !Help YAML typ to create]
+  - !Option [pure, !Action store_true, !Help create pure YAML instance]
+  - !Arg [file, !H 'name of the file to load']
+
 
 """  # NOQA
```

### Comparing `ruamel.yaml.cmd-0.6.3/__main__.py` & `ruamel.yaml.cmd-0.6.4/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 # flake8: noqa
-# cligen: 0.2.0, dd: 2022-09-01
+# cligen: 0.3.2, dd: 2023-06-13, args: gen
 
 
 import argparse
 import importlib
 import sys
 import typing
 
@@ -38,25 +38,14 @@
         self.val = val
 
     def __str__(self) -> str:
         return str(self.val)
 
 
 class CountAction(argparse.Action):
-    """argparse action for counting up and down
-
-    standard argparse action='count', only increments with +1, this action uses
-    the value of self.const if provided, and +1 if not provided
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--verbose', '-v', action=CountAction, const=1,
-            nargs=0)
-    parser.add_argument('--quiet', '-q', action=CountAction, dest='verbose',
-            const=-1, nargs=0)
-    """
 
     def __call__(
         self,
         parser: typing.Any,
         namespace: argparse.Namespace,
         values: typing.Union[str, typing.Sequence[str], None],
         option_string: typing.Optional[str] = None,
@@ -113,14 +102,15 @@
     parsers[-1].add_argument('--literal', default=DefaultVal(False), action='store_true', help='convert scalars with newlines to literal block style')
     parsers[-1].add_argument('--write', '-w', default=DefaultVal(False), action='store_true', help='write individual .yaml files (reusing basename), instead of stdout')
     parsers[-1].add_argument('--output', '-o', default=DefaultVal(None), metavar='OUT', help='write to file %(metavar)s instead of stdout')
     parsers[-1].add_argument('--smart-string', default=DefaultVal(False), action='store_true', help='set literal block style on strings with \\n otherwise plain if possible')
     px = subp.add_parser('json', aliases=['from-json'], description='convert JSON to block-style YAML', help='convert JSON to block-style YAML')
     px.set_defaults(subparser_func='json')
     parsers.append(px)
+    parsers[-1].add_argument('--width', default=80, metavar='W', type=int, help='set width of output (default: %(default)s')
     parsers[-1].add_argument('--mozlz4', action='store_true', help='decode mozilla lz4')
     parsers[-1].add_argument('file', nargs='+')
     parsers[-1].add_argument('--verbose', '-v', default=DefaultVal(0), nargs=0, help='increase verbosity level', action=CountAction, const=1)
     parsers[-1].add_argument('--indent', default=DefaultVal(None), metavar='IND', help='set indent level (default: auto)')
     parsers[-1].add_argument('--bsi', dest='block_seq_indent', metavar='BLOCK_SEQ_IND', type=int, help='set block sequence indent level (default: auto)')
     parsers[-1].add_argument('--flow', default=DefaultVal(False), action='store_true', help='use flow-style YAML instead of block style')
     parsers[-1].add_argument('--semi', default=DefaultVal(False), action='store_true', help='write block style YAML except for "leaf" mapping/dict')
@@ -289,14 +279,70 @@
     parsers[-1].add_argument('--bsi', dest='block_seq_indent', metavar='BLOCK_SEQ_IND', type=int, help='set block sequence indent level (default: auto)')
     parsers[-1].add_argument('--flow', default=DefaultVal(False), action='store_true', help='use flow-style YAML instead of block style')
     parsers[-1].add_argument('--semi', default=DefaultVal(False), action='store_true', help='write block style YAML except for "leaf" mapping/dict')
     parsers[-1].add_argument('--literal', default=DefaultVal(False), action='store_true', help='convert scalars with newlines to literal block style')
     parsers[-1].add_argument('--write', '-w', default=DefaultVal(False), action='store_true', help='write individual .yaml files (reusing basename), instead of stdout')
     parsers[-1].add_argument('--output', '-o', default=DefaultVal(None), metavar='OUT', help='write to file %(metavar)s instead of stdout')
     parsers[-1].add_argument('--smart-string', default=DefaultVal(False), action='store_true', help='set literal block style on strings with \\n otherwise plain if possible')
+    px = subp.add_parser('tokens', help='show tokens')
+    px.set_defaults(subparser_func='tokens')
+    parsers.append(px)
+    parsers[-1].add_argument('file', help='file to edit using $EDITOR')
+    parsers[-1].add_argument('--verbose', '-v', default=DefaultVal(0), nargs=0, help='increase verbosity level', action=CountAction, const=1)
+    parsers[-1].add_argument('--indent', default=DefaultVal(None), metavar='IND', help='set indent level (default: auto)')
+    parsers[-1].add_argument('--bsi', dest='block_seq_indent', metavar='BLOCK_SEQ_IND', type=int, help='set block sequence indent level (default: auto)')
+    parsers[-1].add_argument('--flow', default=DefaultVal(False), action='store_true', help='use flow-style YAML instead of block style')
+    parsers[-1].add_argument('--semi', default=DefaultVal(False), action='store_true', help='write block style YAML except for "leaf" mapping/dict')
+    parsers[-1].add_argument('--literal', default=DefaultVal(False), action='store_true', help='convert scalars with newlines to literal block style')
+    parsers[-1].add_argument('--write', '-w', default=DefaultVal(False), action='store_true', help='write individual .yaml files (reusing basename), instead of stdout')
+    parsers[-1].add_argument('--output', '-o', default=DefaultVal(None), metavar='OUT', help='write to file %(metavar)s instead of stdout')
+    parsers[-1].add_argument('--smart-string', default=DefaultVal(False), action='store_true', help='set literal block style on strings with \\n otherwise plain if possible')
+    px = subp.add_parser('events', help='show events')
+    px.set_defaults(subparser_func='events')
+    parsers.append(px)
+    parsers[-1].add_argument('file', help='file to edit using $EDITOR')
+    parsers[-1].add_argument('--verbose', '-v', default=DefaultVal(0), nargs=0, help='increase verbosity level', action=CountAction, const=1)
+    parsers[-1].add_argument('--indent', default=DefaultVal(None), metavar='IND', help='set indent level (default: auto)')
+    parsers[-1].add_argument('--bsi', dest='block_seq_indent', metavar='BLOCK_SEQ_IND', type=int, help='set block sequence indent level (default: auto)')
+    parsers[-1].add_argument('--flow', default=DefaultVal(False), action='store_true', help='use flow-style YAML instead of block style')
+    parsers[-1].add_argument('--semi', default=DefaultVal(False), action='store_true', help='write block style YAML except for "leaf" mapping/dict')
+    parsers[-1].add_argument('--literal', default=DefaultVal(False), action='store_true', help='convert scalars with newlines to literal block style')
+    parsers[-1].add_argument('--write', '-w', default=DefaultVal(False), action='store_true', help='write individual .yaml files (reusing basename), instead of stdout')
+    parsers[-1].add_argument('--output', '-o', default=DefaultVal(None), metavar='OUT', help='write to file %(metavar)s instead of stdout')
+    parsers[-1].add_argument('--smart-string', default=DefaultVal(False), action='store_true', help='set literal block style on strings with \\n otherwise plain if possible')
+    px = subp.add_parser('generate', description='generate a file filled with random YAML until it reaches size\n', help='generate a file filled with random YAML until it reaches size\n')
+    px.set_defaults(subparser_func='generate')
+    parsers.append(px)
+    parsers[-1].add_argument('--size', default=10, help='size in Kb')
+    parsers[-1].add_argument('--levels', help='levels in file (e.g. sm_s1m) ')
+    parsers[-1].add_argument('file', help='name of the file to generate')
+    parsers[-1].add_argument('--verbose', '-v', default=DefaultVal(0), nargs=0, help='increase verbosity level', action=CountAction, const=1)
+    parsers[-1].add_argument('--indent', default=DefaultVal(None), metavar='IND', help='set indent level (default: auto)')
+    parsers[-1].add_argument('--bsi', dest='block_seq_indent', metavar='BLOCK_SEQ_IND', type=int, help='set block sequence indent level (default: auto)')
+    parsers[-1].add_argument('--flow', default=DefaultVal(False), action='store_true', help='use flow-style YAML instead of block style')
+    parsers[-1].add_argument('--semi', default=DefaultVal(False), action='store_true', help='write block style YAML except for "leaf" mapping/dict')
+    parsers[-1].add_argument('--literal', default=DefaultVal(False), action='store_true', help='convert scalars with newlines to literal block style')
+    parsers[-1].add_argument('--write', '-w', default=DefaultVal(False), action='store_true', help='write individual .yaml files (reusing basename), instead of stdout')
+    parsers[-1].add_argument('--output', '-o', default=DefaultVal(None), metavar='OUT', help='write to file %(metavar)s instead of stdout')
+    parsers[-1].add_argument('--smart-string', default=DefaultVal(False), action='store_true', help='set literal block style on strings with \\n otherwise plain if possible')
+    px = subp.add_parser('analyse')
+    px.set_defaults(subparser_func='analyse')
+    parsers.append(px)
+    parsers[-1].add_argument('--typ', help='YAML typ to create')
+    parsers[-1].add_argument('--pure', action='store_true', help='create pure YAML instance')
+    parsers[-1].add_argument('file', help='name of the file to load')
+    parsers[-1].add_argument('--verbose', '-v', default=DefaultVal(0), nargs=0, help='increase verbosity level', action=CountAction, const=1)
+    parsers[-1].add_argument('--indent', default=DefaultVal(None), metavar='IND', help='set indent level (default: auto)')
+    parsers[-1].add_argument('--bsi', dest='block_seq_indent', metavar='BLOCK_SEQ_IND', type=int, help='set block sequence indent level (default: auto)')
+    parsers[-1].add_argument('--flow', default=DefaultVal(False), action='store_true', help='use flow-style YAML instead of block style')
+    parsers[-1].add_argument('--semi', default=DefaultVal(False), action='store_true', help='write block style YAML except for "leaf" mapping/dict')
+    parsers[-1].add_argument('--literal', default=DefaultVal(False), action='store_true', help='convert scalars with newlines to literal block style')
+    parsers[-1].add_argument('--write', '-w', default=DefaultVal(False), action='store_true', help='write individual .yaml files (reusing basename), instead of stdout')
+    parsers[-1].add_argument('--output', '-o', default=DefaultVal(None), metavar='OUT', help='write to file %(metavar)s instead of stdout')
+    parsers[-1].add_argument('--smart-string', default=DefaultVal(False), action='store_true', help='set literal block style on strings with \\n otherwise plain if possible')
     parsers.pop()
     if '--version' in cmdarg[1:]:
         if '-v' in cmdarg[1:] or '--verbose' in cmdarg[1:]:
             return list_versions(pkg_name='ruamel.yaml.cmd', version=None, pkgs=['configobj', 'ruamel.yaml.convert', 'ruamel.yaml', 'ruamel.yaml.base', 'lz4'])
         print(__version__)
         return 0
     if '--help-all' in cmdarg[1:]:
@@ -319,15 +365,15 @@
         delattr(args, '_gl_' + gl)
         if isinstance(getattr(args, gl, None), DefaultVal):
             setattr(args, gl, getattr(args, gl).val)
     cls = getattr(importlib.import_module('ruamel.yaml.cmd.yaml_cmd'), 'YAMLCommand')
     obj = cls(args)
     funcname = getattr(args, 'subparser_func', None)
     if funcname is None:
-        parsers[0].parse_args('--help')
+        parsers[0].parse_args(['--help'])
     fun = getattr(obj, funcname + '_subcommand', None)
     if fun is None:
         fun = getattr(obj, funcname)
     ret_val = fun()
     if ret_val is None:
         return 0
     if isinstance(ret_val, int):
```

### Comparing `ruamel.yaml.cmd-0.6.3/ruamel.yaml.cmd.egg-info/PKG-INFO` & `ruamel.yaml.cmd-0.6.4/ruamel.yaml.cmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ruamel.yaml.cmd
-Version: 0.6.3
+Version: 0.6.4
 Summary: commandline utility to manipulate YAML files
 Home-page: https://sourceforge.net/p/ruamel-yaml-cmd/code/ci/default/tree
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ruamel.yaml.cmd-0.6.3/setup.py` & `ruamel.yaml.cmd-0.6.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # # header
 # coding: utf-8
-# dd: 20200903
-
-from __future__ import print_function, absolute_import, division, unicode_literals
+# dd: 20230418
 
 # # __init__.py parser
 
 import sys
 import os
 import datetime
-import traceback
+from textwrap import dedent
 
 sys.path = [path for path in sys.path if path not in [os.getcwd(), ""]]
 import platform  # NOQA
 from _ast import *  # NOQA
 from ast import parse  # NOQA
 
 from setuptools import setup, Extension, Distribution  # NOQA
 from setuptools.command import install_lib  # NOQA
 from setuptools.command.sdist import sdist as _sdist  # NOQA
 
-try:
-    from setuptools.namespaces import Installer as NameSpaceInstaller # NOQA
-except ImportError:
-    msg = ('You should use the latest setuptools. The namespaces.py file that this setup.py'
-           ' uses was added in setuptools 28.7.0 (Oct 2016)')
-    print(msg)
-    sys.exit()
+# try:
+#     from setuptools.namespaces import Installer as NameSpaceInstaller # NOQA
+# except ImportError:
+#     msg = ('You should use the latest setuptools. The namespaces.py file that this setup.py'
+#            ' uses was added in setuptools 28.7.0 (Oct 2016)')
+#     print(msg)
+#     sys.exit()
 
 if __name__ != '__main__':
     raise NotImplementedError('should never include setup.py')
 
 # # definitions
 
 full_package_name = None
@@ -274,16 +272,15 @@
                 alt_files.append(x)
         return alt_files
 
 
 class MySdist(_sdist):
     def initialize_options(self):
         _sdist.initialize_options(self)
-        # see pep 527, new uploads should be tar.gz or .zip
-        # fmt = getattr(self, 'tarfmt',  None)
+        # failed expiriment, see pep 527, new uploads should be tar.gz or .zip
         # because of unicode_literals
         # self.formats = fmt if fmt else [b'bztar'] if sys.version_info < (3, ) else ['bztar']
         dist_base = os.environ.get('PYDISTBASE')
         fpn = getattr(getattr(self, 'nsp', self), 'full_package_name', None)
         if fpn and dist_base:
             print('setting  distdir {}/{}'.format(dist_base, fpn))
             self.dist_dir = os.path.join(dist_base, fpn)
@@ -313,16 +310,16 @@
     def __init__(self, pkg_data):
         assert isinstance(pkg_data, dict)
         self._pkg_data = pkg_data
         self.full_package_name = self.pn(self._pkg_data['full_package_name'])
         self._split = None
         self.depth = self.full_package_name.count('.')
         self.nested = self._pkg_data.get('nested', False)
-        if self.nested:
-            NameSpaceInstaller.install_namespaces = lambda x: None
+        # if self.nested:
+        #     NameSpaceInstaller.install_namespaces = lambda x: None
         self.command = None
         self.python_version()
         self._pkg = [None, None]  # required and pre-installable packages
         if sys.argv[0] == 'setup.py' and sys.argv[1] == 'install':
             debug('calling setup.py', sys.argv)
             if '-h' in sys.argv:
                 pass
@@ -383,17 +380,14 @@
         if skip:
             # this interferes with output checking
             # print('skipping sub-packages:', ', '.join(skip))
             pass
         return self._split
 
     @property
-    def namespace_packages(self):
-        return self.split[: self.depth]
-
     def namespace_directories(self, depth=None):
         """return list of directories where the namespace should be created /
         can be found
         """
         res = []
         for index, d in enumerate(self.split[:depth]):
             # toplevel gets a dot
@@ -406,31 +400,19 @@
     def package_dir(self):
         d = {
             # don't specify empty dir, clashes with package_data spec
             self.full_package_name: '.'
         }
         if 'extra_packages' in self._pkg_data:
             return d
-        if len(self.split) > 1:  # only if package namespace
-            d[self.split[0]] = self.namespace_directories(1)[0]
+        # if len(self.split) > 1:  # only if package namespace
+        #     d[self.split[0]] = self.namespace_directories(1)[0]
+        # print('d', d, os.getcwd())
         return d
 
-    def create_dirs(self):
-        """create the directories necessary for namespace packaging"""
-        directories = self.namespace_directories(self.depth)
-        if not directories:
-            return
-        if not os.path.exists(directories[0]):
-            for d in directories:
-                os.mkdir(d)
-                with open(os.path.join(d, '__init__.py'), 'w') as fp:
-                    fp.write(
-                        'import pkg_resources\n' 'pkg_resources.declare_namespace(__name__)\n'
-                    )
-
     def python_version(self):
         supported = self._pkg_data.get('supported')
         if supported is None:
             return
         if len(supported) == 1:
             minimum = supported[0]
         else:
@@ -523,15 +505,15 @@
                 # entry_points=['yaml = ruamel.yaml.cmd:main'],
                 return {'console_scripts': [ep]}
             # assume that it is just the script name
             script_name = ep
         if package_name is None:
             package_name = self.full_package_name
         if not script_name:
-            script_name = package_name.split('.')[-1]
+            script_name = package_name.rsplit('.', 1)[-1]
         return {
             'console_scripts': [
                 '{0} = {1}'.format(script_name, pckg_entry_point(package_name))
             ]
         }
 
     @property
@@ -714,15 +696,16 @@
                     pd[str(k)] = pd.pop(k)
             # for k in pd:
             #     pd[k] = [e.encode('utf-8') for e in pd[k]]  # de-unicode
         return pd
 
     @property
     def packages(self):
-        s = self.split
+        # s = self.split
+        s = [self._pkg_data['full_package_name']]
         # fixed this in package_data, the keys there must be non-unicode for py27
         # if sys.version_info < (3, 0):
         #     s = [x.encode('utf-8') for x in self.split]
         return s + self._pkg_data.get('extra_packages', [])
 
     @property
     def python_requires(self):
@@ -750,99 +733,29 @@
         try:
             plat = sys.argv.index('--plat-name')
             if 'win' in sys.argv[plat + 1]:
                 return None
         except ValueError:
             pass
         self._ext_modules = []
-        no_test_compile = False
+        no_test_compile = True
         if '--restructuredtext' in sys.argv:
             no_test_compile = True
         elif 'sdist' in sys.argv:
             no_test_compile = True
         if no_test_compile:
             for target in self._pkg_data.get('ext_modules', []):
                 ext = Extension(
                     self.pn(target['name']),
                     sources=[self.pn(x) for x in target['src']],
                     libraries=[self.pn(x) for x in target.get('lib')],
                 )
                 self._ext_modules.append(ext)
             return self._ext_modules
-
-        print('sys.argv', sys.argv)
-        import tempfile
-        import shutil
-        from textwrap import dedent
-
-        import distutils.sysconfig
-        import distutils.ccompiler
-        from distutils.errors import CompileError, LinkError
-
-        for target in self._pkg_data.get('ext_modules', []):  # list of dicts
-            ext = Extension(
-                self.pn(target['name']),
-                sources=[self.pn(x) for x in target['src']],
-                libraries=[self.pn(x) for x in target.get('lib')],
-            )
-            # debug('test1 in target', 'test' in target, target)
-            if 'test' not in target:  # no test, just hope it works
-                self._ext_modules.append(ext)
-                continue
-            if sys.version_info[:2] == (3, 4) and platform.system() == 'Windows':
-                # this is giving problems on appveyor, so skip
-                if 'FORCE_C_BUILD_TEST' not in os.environ:
-                    self._ext_modules.append(ext)
-                    continue
-            # write a temporary .c file to compile
-            c_code = dedent(target['test'])
-            try:
-                tmp_dir = tempfile.mkdtemp(prefix='tmp_ruamel_')
-                bin_file_name = 'test' + self.pn(target['name'])
-                file_name = os.path.join(tmp_dir, bin_file_name + '.c')
-                print('test compiling', file_name, '->', bin_file_name, end=' ')
-                with open(file_name, 'w') as fp:  # write source
-                    fp.write(c_code)
-                # and try to compile it
-                compiler = distutils.ccompiler.new_compiler()
-                assert isinstance(compiler, distutils.ccompiler.CCompiler)
-                # do any platform specific initialisations
-                distutils.sysconfig.customize_compiler(compiler)
-                # make sure you can reach header files because compile does change dir
-                compiler.add_include_dir(os.getcwd())
-                if sys.version_info < (3,):
-                    tmp_dir = tmp_dir.encode('utf-8')
-                # used to be a different directory, not necessary
-                compile_out_dir = tmp_dir
-                try:
-                    compiler.link_executable(
-                        compiler.compile([file_name], output_dir=compile_out_dir),
-                        bin_file_name,
-                        output_dir=tmp_dir,
-                        libraries=ext.libraries,
-                    )
-                except CompileError:
-                    debug('compile error:', file_name)
-                    print('compile error:', file_name)
-                    raise
-                except LinkError:
-                    debug('link error', file_name)
-                    print('link error', file_name)
-                    raise
-                print('OK')
-                self._ext_modules.append(ext)
-            except Exception as e:  # NOQA
-                debug('Exception:', e)
-                print('Exception:', e)
-                sys.exit(1)
-                if sys.version_info[:2] == (3, 4) and platform.system() == 'Windows':
-                    traceback.print_exc()
-            finally:
-                shutil.rmtree(tmp_dir)
-        return self._ext_modules
+        # this used to use distutils
 
     @property
     def test_suite(self):
         return self._pkg_data.get('test_suite')
 
     def wheel(self, kw, setup):
         """temporary add setup.cfg if creating a wheel to include LICENSE file
@@ -850,56 +763,97 @@
         """
         if 'bdist_wheel' not in sys.argv:
             return False
         file_name = 'setup.cfg'
         if os.path.exists(file_name):  # add it if not in there?
             return False
         with open(file_name, 'w') as fp:
-            if os.path.exists('LICENSE'):
-                fp.write('[metadata]\nlicense_file = LICENSE\n')
-            else:
-                print('\n\n>>>>>> LICENSE file not found <<<<<\n\n')
             if self._pkg_data.get('universal'):
                 fp.write('[bdist_wheel]\nuniversal = 1\n')
         try:
             setup(**kw)
         except Exception:
             raise
         finally:
             os.remove(file_name)
         return True
 
 
-# # call setup
+class TmpFiles:
+    def __init__(self, pkg_data, py_project=True, keep=False):
+        self._rm_after = []
+        self._pkg_data = pkg_data
+        self._py_project = py_project
+        self._bdist_wheel = 'bdist_wheel' in sys.argv
+        self._keep = keep
+
+    def __enter__(self):
+        self.bdist_wheel()
+        self.py_project()
+
+    def bdist_wheel(self):
+        """pyproject doesn't allow for universal, so use setup.cfg if necessary
+        """
+        file_name = 'setup.cfg'
+        if not self._bdist_wheel or os.path.exists(file_name):
+            return
+        if self._pkg_data.get('universal'):
+            self._rm_after.append(file_name)
+            with open(file_name, 'w') as fp:
+                fp.write('[bdist_wheel]\nuniversal = 1\n')
+
+    def py_project(self):
+        """
+        to prevent pip from complaining, or is it too late to create it from setup.py
+        """
+        file_name = 'pyproject.toml'
+        if not self._py_project or os.path.exists(file_name):
+            return
+        self._rm_after.append(file_name)
+        with open(file_name, 'w') as fp:
+            fp.write(dedent("""\
+            [build-system]
+            requires = ["setuptools", "wheel"]
+            # test
+            build-backend = "setuptools.build_meta"
+            """))
+
+    def __exit__(self, typ, value, traceback):
+        if self._keep:
+            return
+        for p in self._rm_after:
+            if not os.path.exists(p):
+                print('file {} already removed'.format(p))
+            else:
+                os.unlink(p)
+
+
+# call setup
 def main():
     dump_kw = '--dump-kw'
     if dump_kw in sys.argv:
         import wheel
-        import distutils
         import setuptools
+        import pip
 
         print('python:    ', sys.version)
+        print('pip:       ', pip.__version__)
         print('setuptools:', setuptools.__version__)
-        print('distutils: ', distutils.__version__)
         print('wheel:     ', wheel.__version__)
     nsp = NameSpacePackager(pkg_data)
     nsp.check()
-    nsp.create_dirs()
+    # nsp.create_dirs()
     MySdist.nsp = nsp
-    if pkg_data.get('tarfmt'):
-        MySdist.tarfmt = pkg_data.get('tarfmt')
-
     cmdclass = dict(install_lib=MyInstallLib, sdist=MySdist)
     if _bdist_wheel_available:
         MyBdistWheel.nsp = nsp
         cmdclass['bdist_wheel'] = MyBdistWheel
 
     kw = dict(
         name=nsp.full_package_name,
-        namespace_packages=nsp.namespace_packages,
         version=version_str,
         packages=nsp.packages,
         python_requires=nsp.python_requires,
         url=nsp.url,
         author=nsp.author,
         author_email=nsp.author_email,
         cmdclass=cmdclass,
@@ -910,52 +864,54 @@
         extras_require=nsp.extras_require,  # available since setuptools 18.0 / 2015-06
         license=nsp.license,
         classifiers=nsp.classifiers,
         keywords=nsp.keywords,
         package_data=nsp.package_data,
         ext_modules=nsp.ext_modules,
         test_suite=nsp.test_suite,
+        zip_safe=False,
     )
 
     if '--version' not in sys.argv and ('--verbose' in sys.argv or dump_kw in sys.argv):
         for k in sorted(kw):
             v = kw[k]
-            print('  "{0}": "{1}",'.format(k, v))
+            print('  "{0}": {1},'.format(k, repr(v)))
     # if '--record' in sys.argv:
     #     return
     if dump_kw in sys.argv:
         sys.argv.remove(dump_kw)
     try:
         with open('README.rst') as fp:
             kw['long_description'] = fp.read()
             kw['long_description_content_type'] = 'text/x-rst'
     except Exception:
         pass
 
-    if nsp.wheel(kw, setup):
-        return
-    for x in ['-c', 'egg_info', '--egg-base', 'pip-egg-info']:
-        if x not in sys.argv:
-            break
-    else:
-        # we're doing a tox setup install any starred package by searching up the source tree
-        # until you match your/package/name for your.package.name
-        for p in nsp.install_pre:
-            import subprocess
-
-            # search other source
-            setup_path = os.path.join(*p.split('.') + ['setup.py'])
-            try_dir = os.path.dirname(sys.executable)
-            while len(try_dir) > 1:
-                full_path_setup_py = os.path.join(try_dir, setup_path)
-                if os.path.exists(full_path_setup_py):
-                    pip = sys.executable.replace('python', 'pip')
-                    cmd = [pip, 'install', os.path.dirname(full_path_setup_py)]
-                    # with open('/var/tmp/notice', 'a') as fp:
-                    #     print('installing', cmd, file=fp)
-                    subprocess.check_output(cmd)
-                    break
-                try_dir = os.path.dirname(try_dir)
-    setup(**kw)
+    # if nsp.wheel(kw, setup):
+    #     return
+    with TmpFiles(pkg_data, keep=True):
+        for x in ['-c', 'egg_info', '--egg-base', 'pip-egg-info']:
+            if x not in sys.argv:
+                break
+        else:
+            # we're doing a tox setup install any starred package by searching up the
+            # source tree until you match your/package/name for your.package.name
+            for p in nsp.install_pre:
+                import subprocess
+
+                # search other source
+                setup_path = os.path.join(*p.split('.') + ['setup.py'])
+                try_dir = os.path.dirname(sys.executable)
+                while len(try_dir) > 1:
+                    full_path_setup_py = os.path.join(try_dir, setup_path)
+                    if os.path.exists(full_path_setup_py):
+                        pip = sys.executable.replace('python', 'pip')
+                        cmd = [pip, 'install', os.path.dirname(full_path_setup_py)]
+                        # with open('/var/tmp/notice', 'a') as fp:
+                        #     print('installing', cmd, file=fp)
+                        subprocess.check_output(cmd)
+                        break
+                    try_dir = os.path.dirname(try_dir)
+        setup(**kw)
 
 
 main()
```

### Comparing `ruamel.yaml.cmd-0.6.3/simpleresolver.py` & `ruamel.yaml.cmd-0.6.4/simpleresolver.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml.cmd-0.6.3/yaml_cmd.py` & `ruamel.yaml.cmd-0.6.4/yaml_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import _ast
 import ast
 import os
 import datetime
 import contextlib
 import subprocess
 import io
-import lz4.block
 import textwrap
 from pathlib import Path
 import typing
 
 import ruamel.yaml
 import ruamel.yaml.base
 from ruamel.yaml import YAML
@@ -451,14 +450,16 @@
         # test end
 
     def json(self):
         return self.from_json()
 
     def from_json(self):
         # use roundtrip to preserve order
+        import lz4.block
+
         errors = 0
         docs = []
         yaml = ruamel.yaml.YAML()
         data = None
         dfs = True if self._args.flow else None if self._args.semi else False
         yaml.default_flow_style = (
             True if self._args.flow else None if self._args.semi else False
@@ -474,15 +475,16 @@
 
                     data = ujson.loads(inp)
             else:
                 inp = open(file_name).read()
             if data is None:
                 yaml = ruamel.yaml.YAML()
                 try:
-                    data = yaml.load(inp)
+                    # data = yaml.load(inp)
+                    data = self.json_load(inp)
                 except ruamel.yaml.composer.ComposerError as e:
                     pm = (e.problem_mark.line, e.problem_mark.column)
                     if 'expected' in e.context and 'single' in e.context and pm == (1, 0):
                         try:
                             data = self._from_line_json(inp)
                         except Exception as e:
                             raise e
@@ -498,18 +500,26 @@
             return 1 if errors else 0
         if self._args.literal:
             from ruamel.yaml.scalarstring import walk_tree
 
             for doc in docs:
                 walk_tree(doc)
         yaml = ruamel.yaml.YAML()
+        yaml.width = self._args.width
+        # print('dfs', dfs)
         yaml.default_flow_style = dfs
         yaml.dump_all(docs, sys.stdout)
         return 1 if errors else 0
 
+    @staticmethod
+    def json_load(inp):
+        import orjson
+
+        return orjson.loads(inp)
+
     def _from_line_json(self, inp):
         """parse line json (i.e. one json document per line) and convert to
            list of loaded constructs"""
         # yaml = ruamel.yaml.YAML(type='safe')
         import ujson
 
         data = []
@@ -557,15 +567,15 @@
             with self.yaml_out() as out:
                 self.yaml.dump(data[0], out)
         else:
             with self.yaml_out() as out:
                 self.yaml.dump_all(data, out)
 
     def htmltable(self):
-        return self.to_htmltable(self)
+        return self.to_htmltable()
 
     def to_htmltable(self):
         def vals(x):
             if isinstance(x, list):
                 return x
             if isinstance(x, (dict, ordereddict)):
                 return x.values()
@@ -785,15 +795,15 @@
         if block_seq_indent is not None:
             block_seq_indent = min(block_seq_indent, seq_indent - 2)
 
         if False:
             loader = ruamel.yaml.RoundTripLoader
             code = ruamel.yaml.load(inp, loader)
             if drop_comment:
-                drop_all_comment(code) # NOQA
+                drop_all_comment(code)  # NOQA
             dumper = ruamel.yaml.RoundTripDumper
             res = ruamel.yaml.dump(
                 code,
                 Dumper=dumper,
                 # indent=indent,
                 block_seq_indent=block_seq_indent,
                 explicit_start=explicit_start,
@@ -977,14 +987,72 @@
         if edit_path.stat().st_mtime == edit_path_time:
             print('not changed')
             edit_path.unlink()
         self.yaml.load(edit_path)
         path.unlink()
         edit_path.rename(path)
 
+    def generate(self):
+        from ruamel.yaml.cmd.generate import Generate
+
+        if self._args.file == 'all':
+            for lvl in ['sm_s1m', 'smm', 'mm_s1m']:
+                for size in [1, 10, 100, 1000, 10000]:
+                    path = Path('data') / f'gen_{size}_{lvl}.yaml'
+                    if path.exists():
+                        continue
+                    print(path)
+                    self._args.size = size
+                    self._args.levels = lvl
+                    generate = Generate(self._args)
+                    try:
+                        with path.open('wb') as fp:
+                            generate(fp)
+                    except Exception as e:
+                        _ = e
+                        path.unlink()
+                        raise
+            return
+        if self._args.levels is None:
+            self._args.levels = 'sm_s1m'
+        generate = Generate(self._args)
+        if self._args.file == '-':
+            generate(sys.stdout)
+        else:
+            with Path(self._args.file).open('wb') as fp:
+                generate(fp)
+
+    def analyse_subcommand(self):
+        from ruamel.yaml.cmd.analyse import Analyse
+
+        analyse = Analyse(self._args)
+        if self._args.file == '-':
+            analyse(sys.stdin)
+        else:
+            with Path(self._args.file).open('rb') as fp:
+                analyse(fp, self._args.file)
+
+    def events_subcommand(self):
+        indent = 0
+        input = Path(self._args.file).read_text()
+        for event in self.yaml.parse(input):
+            compact = event.compact_repr()
+            assert compact[0] in '+=-'
+            if compact[0] == '-':
+                indent -= 1
+            print(f'{" "*indent}{compact}')
+            if compact[0] == '+':
+                indent += 1
+
+    def tokens_subcommand(self):
+        indent = 0
+        input = Path(self._args.file).read_text()
+        for token in self.yaml.scan(input):
+            print(f'{" "*indent}{token}')
+
 
 # ToDo: move to ruamel.yaml.base
 class AddableYAML(ruamel.yaml.base.YAMLBase):
     def add(self, path, value, create_parents=False, create_item=False, create_key=False):
         """
           The path is a list/tuple of which each element is used to "descend" the data
           structure. If an element is an integer a list/sequence is assumed, else a dict/mapping.
```

