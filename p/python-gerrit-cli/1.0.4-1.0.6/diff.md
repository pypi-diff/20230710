# Comparing `tmp/python-gerrit-cli-1.0.4.tar.gz` & `tmp/python-gerrit-cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/devspace/python-gerrit-cli/dist/.tmp-j_ooo6ko/python-gerrit-cli-1.0.4.tar", last modified: Thu Jun 22 10:39:07 2023, max compression
+gzip compressed data, was "python-gerrit-cli-1.0.6.tar", last modified: Mon Jul 10 14:30:00 2023, max compression
```

## Comparing `python-gerrit-cli-1.0.4.tar` & `python-gerrit-cli-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.658120 python-gerrit-cli-1.0.4/
--rw-rw-r--   0 pk        (1000) pk        (1000)     1113 2023-05-07 07:31:21.000000 python-gerrit-cli-1.0.4/LICENSE
--rw-rw-r--   0 pk        (1000) pk        (1000)     2244 2023-06-22 10:39:07.654120 python-gerrit-cli-1.0.4/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)       33 2023-05-07 07:23:12.000000 python-gerrit-cli-1.0.4/README.md
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.554120 python-gerrit-cli-1.0.4/gerritcli/
--rw-rw-r--   0 pk        (1000) pk        (1000)     6573 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/__init__.py
--rwxrwxr-x   0 pk        (1000) pk        (1000)     1203 2023-05-07 12:34:46.000000 python-gerrit-cli-1.0.4/gerritcli/__main__.py
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.594120 python-gerrit-cli-1.0.4/gerritcli/command/
--rw-rw-r--   0 pk        (1000) pk        (1000)      327 2023-06-22 03:56:56.000000 python-gerrit-cli-1.0.4/gerritcli/command/__init__.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     6090 2023-06-22 09:21:24.000000 python-gerrit-cli-1.0.4/gerritcli/command/account_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     5698 2023-06-22 09:21:57.000000 python-gerrit-cli-1.0.4/gerritcli/command/change_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     5557 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/group_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     1740 2023-06-22 09:32:38.000000 python-gerrit-cli-1.0.4/gerritcli/command/patch_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     4281 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/project_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     2112 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/server_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)      497 2023-05-07 03:24:09.000000 python-gerrit-cli-1.0.4/gerritcli/command/version_command.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     4031 2023-06-22 09:21:14.000000 python-gerrit-cli-1.0.4/gerritcli/utils.py
--rw-rw-r--   0 pk        (1000) pk        (1000)     6021 2023-06-22 10:37:31.000000 python-gerrit-cli-1.0.4/pyproject.toml
-drwxrwxr-x   0 pk        (1000) pk        (1000)        0 2023-06-22 10:39:07.650120 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/
--rw-rw-r--   0 pk        (1000) pk        (1000)     2244 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/PKG-INFO
--rw-rw-r--   0 pk        (1000) pk        (1000)      626 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)        1 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       54 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/entry_points.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       39 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/requires.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       10 2023-06-22 10:39:07.000000 python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/top_level.txt
--rw-rw-r--   0 pk        (1000) pk        (1000)       38 2023-06-22 10:39:07.658120 python-gerrit-cli-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:00.624193 python-gerrit-cli-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-10 14:30:00.624193 python-gerrit-cli-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:00.620192 python-gerrit-cli-1.0.6/gerritcli/
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:00.620192 python-gerrit-cli-1.0.6/gerritcli/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/account_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/change_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/group_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/patch_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/project_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/server_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/command/version_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/gerritcli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-07-10 14:29:37.000000 python-gerrit-cli-1.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:30:00.624193 python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-10 14:30:00.000000 python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-10 14:30:00.000000 python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:30:00.000000 python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 14:30:00.000000 python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 14:30:00.000000 python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 14:30:00.000000 python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 14:30:00.624193 python-gerrit-cli-1.0.6/setup.cfg
```

### Comparing `python-gerrit-cli-1.0.4/LICENSE` & `python-gerrit-cli-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.4/gerritcli/__init__.py` & `python-gerrit-cli-1.0.6/gerritcli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import configparser
 from abc import ABC, abstractmethod
 from gerrit import GerritClient
 import gerrit
 import requests
 import gerritcli.utils
 
+__version__ = "1.0.6"
+version_string = f'gerritcli {__version__}, Written by PKEMB, Kai Peng'
+
 class gerrit_server:
     __instance = None
     gerrit_rc = os.path.join(os.environ['HOME'], '.gerrit.rc')
     gerrit_client = None
 
     def __init__(self) -> None:
         self.config = configparser.ConfigParser()
```

### Comparing `python-gerrit-cli-1.0.4/gerritcli/__main__.py` & `python-gerrit-cli-1.0.6/gerritcli/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,17 @@
             required=False)
     parser.add_argument('--debug',
             dest="debug",
             help='enable debug',
             default=False,
             action='store_true',
             required=False)
+    parser.add_argument('--version', '-v',
+            action='version',
+            version=gerritcli.version_string)
 
     # main command
     subparser = parser.add_subparsers(help='command usage', dest='command', metavar = "command", required=True)
     # call all child init function for add sub command
     for cmd in gerritcli.maincommand.__subclasses__():
         cmd.init(subparser)
```

### Comparing `python-gerrit-cli-1.0.4/gerritcli/command/account_command.py` & `python-gerrit-cli-1.0.6/gerritcli/command/account_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.4/gerritcli/command/change_command.py` & `python-gerrit-cli-1.0.6/gerritcli/command/change_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,24 +104,35 @@
         self.subcmd['search'].add_argument('query', help='set query condition', nargs='+')
         self.subcmd['get'].add_argument('id', help='change id or change number', nargs='+')
         for cmd in [self.subcmd['search'], self.subcmd['get']]:
             gerritcli.utils.add_commmon_argument(cmd, 'output')
             gerritcli.utils.add_commmon_argument(cmd, 'header', default = self.search_default_header)
             gerritcli.utils.add_commmon_argument(cmd, 'format')
 
-        gerritcli.utils.add_commmon_argument(self.subcmd['search'], 'limit')
+        gerritcli.utils.add_commmon_argument(self.subcmd['search'], 'limit', default=0)
         gerritcli.utils.add_commmon_argument(self.subcmd['search'], 'skip')
 
         # subcmd create / delete no argument
         return
 
-    def search_change(self, query, **kwargs):
+    def search_change(self, query, options=None, limit=0, skip=0):
         try:
             client = gerritcli.gerrit_server.get_client()
-            changes = client.changes.search(query, **kwargs)
+            params = {
+                'o': options,
+                'S': skip,
+            }
+            # limit 为 0 表示没有限制
+            if limit == 0:
+                params['no-limit'] = ''
+            else:
+                params['n'] = limit
+
+            # client.changes.search() 不支持 'no-limit' 参数，所以直接使用client.get()
+            changes = client.get(f'/changes/?q={query}', params=params)
             changes_info = list()
             for change in changes:
                 changes_info.append(gerrit_change_info(change))
             return changes_info
         except gerrit.utils.exceptions.ValidationError:
             print("query \"%s\" is invalid!!!" % query)
             sys.exit(1)
```

### Comparing `python-gerrit-cli-1.0.4/gerritcli/command/group_command.py` & `python-gerrit-cli-1.0.6/gerritcli/command/group_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.4/gerritcli/command/patch_command.py` & `python-gerrit-cli-1.0.6/gerritcli/command/patch_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.4/gerritcli/command/project_command.py` & `python-gerrit-cli-1.0.6/gerritcli/command/project_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.4/gerritcli/command/server_command.py` & `python-gerrit-cli-1.0.6/gerritcli/command/server_command.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.4/gerritcli/utils.py` & `python-gerrit-cli-1.0.6/gerritcli/utils.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-cli-1.0.4/pyproject.toml` & `python-gerrit-cli-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 name = "python-gerrit-cli"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.4"  # Required
+# version = "x.y.z"  # Required
+dynamic = ["version"]
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Gerrit Command Line Interface"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -145,7 +146,10 @@
 # package-data = {"sample" = ["*.dat"]}
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools >= 43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools.dynamic]
+version = {attr = "gerritcli.__version__"}
```

### Comparing `python-gerrit-cli-1.0.4/python_gerrit_cli.egg-info/SOURCES.txt` & `python-gerrit-cli-1.0.6/python_gerrit_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

