# Comparing `tmp/pyxargs-2.2.0.tar.gz` & `tmp/pyxargs-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxargs-2.2.0.tar", last modified: Fri Jul  7 21:51:02 2023, max compression
+gzip compressed data, was "pyxargs-2.3.0.tar", last modified: Mon Jul 10 06:50:21 2023, max compression
```

## Comparing `pyxargs-2.2.0.tar` & `pyxargs-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:51:02.823599 pyxargs-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 21:50:53.000000 pyxargs-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-07 21:51:02.819599 pyxargs-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-07 21:50:53.000000 pyxargs-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:51:02.819599 pyxargs-2.2.0/pyxargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 21:51:02.000000 pyxargs-2.2.0/pyxargs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-07 21:50:53.000000 pyxargs-2.2.0/pyxargs.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:51:02.823599 pyxargs-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-07 21:50:53.000000 pyxargs-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:50:21.660227 pyxargs-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 06:50:09.000000 pyxargs-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-10 06:50:21.660227 pyxargs-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-10 06:50:09.000000 pyxargs-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:50:21.660227 pyxargs-2.3.0/pyxargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 06:50:21.000000 pyxargs-2.3.0/pyxargs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-07-10 06:50:09.000000 pyxargs-2.3.0/pyxargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 06:50:21.660227 pyxargs-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-10 06:50:09.000000 pyxargs-2.3.0/setup.py
```

### Comparing `pyxargs-2.2.0/LICENSE` & `pyxargs-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxargs-2.2.0/PKG-INFO` & `pyxargs-2.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxargs
-Version: 2.2.0
+Version: 2.3.0
 Summary: A partial and opinionated implementation of xargs in python with some added features
 Home-page: https://github.com/elesiuta/pyxargs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
@@ -83,14 +83,17 @@
   --py, --pyex          executes commands as python code using exec()
   --pyev                evaluates commands as python expressions using eval()
   --import library      executes 'import <library>' for each library
   --im library, --importstar library
                         executes 'from <library> import *' for each library
   --pre "code"          runs exec(code) before execution
   --post "code"         runs exec(code) after execution
+  -P P, --procs P       split into P chunks and execute each chunk in parallel
+                        as a separate process and window with byobu or tmux
+  -c c, --chunk c       runs chunk c of P (0 <= c < P) (without multiplexer)
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
 ```bash
```

### Comparing `pyxargs-2.2.0/README.md` & `pyxargs-2.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,17 @@
   --py, --pyex          executes commands as python code using exec()
   --pyev                evaluates commands as python expressions using eval()
   --import library      executes 'import <library>' for each library
   --im library, --importstar library
                         executes 'from <library> import *' for each library
   --pre "code"          runs exec(code) before execution
   --post "code"         runs exec(code) after execution
+  -P P, --procs P       split into P chunks and execute each chunk in parallel
+                        as a separate process and window with byobu or tmux
+  -c c, --chunk c       runs chunk c of P (0 <= c < P) (without multiplexer)
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
 ```bash
```

### Comparing `pyxargs-2.2.0/pyxargs.egg-info/PKG-INFO` & `pyxargs-2.3.0/pyxargs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxargs
-Version: 2.2.0
+Version: 2.3.0
 Summary: A partial and opinionated implementation of xargs in python with some added features
 Home-page: https://github.com/elesiuta/pyxargs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Shells
@@ -83,14 +83,17 @@
   --py, --pyex          executes commands as python code using exec()
   --pyev                evaluates commands as python expressions using eval()
   --import library      executes 'import <library>' for each library
   --im library, --importstar library
                         executes 'from <library> import *' for each library
   --pre "code"          runs exec(code) before execution
   --post "code"         runs exec(code) after execution
+  -P P, --procs P       split into P chunks and execute each chunk in parallel
+                        as a separate process and window with byobu or tmux
+  -c c, --chunk c       runs chunk c of P (0 <= c < P) (without multiplexer)
   -i, --interactive     prompt the user before executing each command, only
                         proceeds if response starts with 'y' or 'Y'
   -n, --dry-run         prints commands without executing them
   -v, --verbose         prints commands before executing them
 ```
 ## Examples
 ```bash
```

### Comparing `pyxargs-2.2.0/pyxargs.py` & `pyxargs-2.3.0/pyxargs.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # https://github.com/elesiuta/pyxargs
 
 import argparse
 import os
+import pickle
+import pty
 import re
 import shlex
+import shutil
 import signal
 import subprocess
 import sys
+import tempfile
 import textwrap
+import time
 import typing
 
 
-__version__: typing.Final[str] = "2.2.0"
+__version__: typing.Final[str] = "2.3.0"
 
 
 def replace_surrogates(string: str) -> str:
     return string.encode('utf16', 'surrogatepass').decode('utf16', 'replace')
 
 
 def colour_print(string: str, colour: str) -> None:
@@ -308,14 +313,20 @@
                         help="executes 'import <library>' for each library")
     parser.add_argument("--im", "--importstar", action="append", type=str, default=[], metavar=("library"), dest="imprtstar",
                         help="executes 'from <library> import *' for each library")
     parser.add_argument("--pre", type=str, default="", metavar=("\"code\""), dest="pre",
                         help="runs exec(code) before execution")
     parser.add_argument("--post", type=str, default="", metavar=("\"code\""), dest="post",
                         help="runs exec(code) after execution")
+    parser.add_argument("-P", "--procs", type=int, default=None, metavar="P", dest="procs",
+                        help="split into P chunks and execute each chunk in parallel as a separate process and window with byobu or tmux")
+    parser.add_argument("-c", "--chunk", type=int, default=None, metavar="c", dest="chunk",
+                        help="runs chunk c of P (0 <= c < P) (without multiplexer)")
+    parser.add_argument("--_command_pickle", nargs=2, default=None, dest="command_pickle",
+                        help=argparse.SUPPRESS)
     parser.add_argument("-i", "--interactive", action="store_true", dest="interactive",
                         help="prompt the user before executing each command, only proceeds if response starts with 'y' or 'Y'")
     parser.add_argument("-n", "--dry-run", action="store_true", dest="dry_run",
                         help="prints commands without executing them")
     parser.add_argument("-v", "--verbose", action="store_true", dest="verbose",
                         help="prints commands before executing them")
     args = parser.parse_args()
@@ -323,15 +334,17 @@
         print(examples)
         return 0
     # determine input mode and read stdin available or required
     stdin = ""
     if args.input_mode in ["f", "p", "a", "s"]:
         short_forms = {"f": "file", "p": "path", "a": "abspath", "s": "stdin"}
         args.input_mode = short_forms[args.input_mode]
-    if args.input_mode is None:
+    if args.command_pickle is not None:
+        args.input_mode = args.command_pickle[0]
+    elif args.input_mode is None:
         if not sys.stdin.isatty():
             stdin = sys.stdin.read()
             args.input_mode = "stdin"
         else:
             args.input_mode = "file"
     elif args.input_mode == "stdin":
         stdin = sys.stdin.read()
@@ -350,18 +363,53 @@
         assert not args.folders, "invalid option --folders for input mode: stdin"
         assert not args.top_level, "invalid option --top for input mode: stdin"
         assert not args.symlinks, "invalid option --symlinks for input mode: stdin"
         assert not args.regex_basename, "invalid option -b for input mode: stdin"
     else:
         assert not args.null, f"invalid option --null for input mode: {args.input_mode}"
         assert not args.delim, f"invalid option --delimiter for input mode: {args.input_mode}"
+    assert args.procs is None or args.procs > 0, "invalid option --procs: requires P > 0"
+    assert args.chunk is None or args.procs is not None, "invalid option --chunk: --procs must be specified"
+    assert args.chunk is None or 0 <= args.chunk < args.procs, "invalid option --chunk: requires 0 <= c < P"
+    assert args.command_pickle is None or args.chunk is not None, "invalid option --_command_pickle: --chunk must be specified"
     # build and run commands
     if len(args.command) >= 1:
-        command_dicts = build_commands(args, stdin)
-        return execute_commands(args, command_dicts)
+        # build commands or load them from pickle if available
+        if args.command_pickle is None:
+            command_dicts = build_commands(args, stdin)
+        else:
+            with open(args.command_pickle[1], "rb") as f:
+                command_dicts = pickle.load(f)
+        # run subprocesses with multiplexer if requested
+        if args.procs is not None and args.chunk is None:
+            multiplexer = "byobu" if shutil.which("byobu") else "tmux" if shutil.which("tmux") else None
+            assert multiplexer is not None, "multiplexer not found: install byobu or tmux"
+            session = time.strftime("pyxargs_%Y%m%d_%H%M%S")
+            command_pickle = tempfile.NamedTemporaryFile()
+            pickle.dump(command_dicts, command_pickle.file)
+            command_pickle.file.flush()
+            pyxargs_command = [sys.executable, os.path.abspath(__file__), "--chunk", "0", "--_command_pickle", args.input_mode, command_pickle.name] + sys.argv[1:]
+            subprocess.run([multiplexer, "new-session", "-d", "-s", session, shlex.join(pyxargs_command)])
+            for i in range(1, args.procs):
+                pyxargs_command[3] = str(i)
+                subprocess.run([multiplexer, "new-window", "-t", f"{session}:{i}", shlex.join(pyxargs_command)])
+            if stdin:
+                sys.stdin = sys.__stdin__ = open("/dev/tty")
+                os.dup2(sys.stdin.fileno(), 0)
+                pty.spawn([multiplexer, "attach-session", "-t", session])
+            else:
+                subprocess.run([multiplexer, "attach-session", "-t", session])
+            return 0
+        # execute commands (in chunks if requested)
+        if args.chunk is None:
+            return execute_commands(args, command_dicts)
+        else:
+            _ = execute_commands(args, command_dicts[args.chunk::args.procs])
+            _ = input(f"Chunk {args.chunk} complete. Press enter to exit. ")
+            return 0
     else:
         parser.print_usage()
         return 2
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pyxargs-2.2.0/setup.py` & `pyxargs-2.3.0/setup.py`

 * *Files identical despite different names*

