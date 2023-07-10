# Comparing `tmp/port4me-0.5.1.post9002.tar.gz` & `tmp/port4me-0.5.1.post9004.tar.gz`

## Comparing `port4me-0.5.1.post9002.tar` & `port4me-0.5.1.post9004.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/Makefile
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/port4me/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/port4me/__main__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/tests/__init__.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/tests/test_port4me.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/tests/test_uint_hash.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/.gitignore
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/LICENSE
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/pyproject.toml
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 port4me-0.5.1.post9002/PKG-INFO
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/Makefile
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/port4me/__init__.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/port4me/__main__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/tests/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/tests/test_port4me.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/tests/test_uint_hash.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/.gitignore
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/LICENSE
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/pyproject.toml
+-rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 port4me-0.5.1.post9004/PKG-INFO
```

### Comparing `port4me-0.5.1.post9002/port4me/__init__.py` & `port4me-0.5.1.post9004/port4me/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from itertools import islice
 import socket
 from getpass import getuser
 from os import getenv
 
 
-__version__ = "0.5.1-9002"
+__version__ = "0.5.1-9004"
 __all__ = ["port4me", "port4me_gen"]
 
 
 # Source: https://chromium.googlesource.com/chromium/src.git/+/refs/heads/master/net/base/port_util.cc
 # Last updated: 2022-10-24
 unsafe_ports_chrome = getenv("PORT4ME_EXCLUDE_UNSAFE_CHROME", "1,7,9,11,13,15,17,19,20,21,22,23,25,37,42,43,53,69,77,79,87,95,101,102,103,104,109,110,111,113,115,117,119,123,135,137,139,143,161,179,389,427,465,512,513,514,515,526,530,531,532,540,548,554,556,563,587,601,636,989,990,993,995,1719,1720,1723,2049,3659,4045,5060,5061,6000,6566,6665,6666,6667,6668,6669,6697,10080")
 
@@ -25,15 +25,19 @@
     for char in s:
         h = (31 * h + ord(char)) % 2**32
     return h
 
 
 def is_port_free(port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        return (s.connect_ex(("", port)) != 0)
+        try:
+            s.bind(("", port))
+        except PermissionError:
+            return False
+        return True
 
 
 def parse_ports(string):
     ports = []
     for port in string.replace("{chrome}", unsafe_ports_chrome).replace(
                                "{firefox}", unsafe_ports_firefox).replace(",", " ").split():
         if port:
```

### Comparing `port4me-0.5.1.post9002/port4me/__main__.py` & `port4me-0.5.1.post9004/port4me/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 from argparse import ArgumentParser
-from . import port4me, parse_ports
+from . import port4me, parse_ports, __version__
 
 parser = ArgumentParser(prog="python -m port4me", description="port4me: Get the Same, Personal, Free TCP Port over and over")
-parser.add_argument("--tool", type=str, help="Used in the seed when generating port numbers, to get a different port sequence for different tools.")
+parser.add_argument("tool", type=str, nargs="?")
+parser.add_argument("--tool", type=str, metavar="TOOL", dest="tool_positional", help="Used in the seed when generating port numbers, to get a different port sequence for different tools.")
 parser.add_argument("--user", type=str, help="Used in the seed when generating port numbers. Defaults to determining the username with getuser().")
 parser.add_argument("--prepend", type=parse_ports, metavar="PORTS", help="A list of ports to try first")
 parser.add_argument("--include", type=parse_ports, metavar="PORTS", help="If specified, skip any ports not in this list")
 parser.add_argument("--exclude", type=parse_ports, metavar="PORTS", help="Skip any ports in this list")
 parser.add_argument("--list", type=int, metavar="N", help="Instead of returning a single port, return a list of this many ports without checking if they are free.")
 parser.add_argument("--test", type=int, metavar="PORT", help="If specified, return whether the port `PORT` is not in use. All other parameters will be ignored.")
+parser.add_argument("--version", action="store_true", help="Show version")
 
-print(port4me(**vars(parser.parse_args())))
+args = vars(parser.parse_args())
+
+tool = args.pop("tool_positional")
+if tool:
+    args["tool"] = tool
+
+if args.pop("version"):
+    print(__version__)
+elif args.get("test"):
+    from sys import exit
+    if port4me(**args):
+        exit(0)
+    else:
+        exit(1)
+elif args.get("list"):
+    print(*port4me(**args), sep="\n")
+else:
+    print(port4me(**args))
```

### Comparing `port4me-0.5.1.post9002/tests/test_port4me.py` & `port4me-0.5.1.post9004/tests/test_port4me.py`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9002/README.md` & `port4me-0.5.1.post9004/README.md`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9002/pyproject.toml` & `port4me-0.5.1.post9004/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port4me-0.5.1.post9002/PKG-INFO` & `port4me-0.5.1.post9004/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port4me
-Version: 0.5.1.post9002
+Version: 0.5.1.post9004
 Summary: The 'port4me' tool: (1) finds a free TCP port in [1024,65535] that the user can open, (2) is designed to work in multi-user environments, (3), gives different users, different ports, (4) gives the user the same port over time with high probability, (5) gives different ports for different software tools, and (6) requires no configuration.
 Project-URL: Homepage, https://github.com/HenrikBengtsson/port4me
 Project-URL: Bug Tracker, https://github.com/HenrikBengtsson/port4me/issues
 Author-email: "Finn Reichertz, Henrik Bengtsson" <henrikb@braju.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

