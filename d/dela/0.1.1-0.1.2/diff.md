# Comparing `tmp/dela-0.1.1.tar.gz` & `tmp/dela-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dela-0.1.1.tar", max compression
+gzip compressed data, was "dela-0.1.2.tar", max compression
```

## Comparing `dela-0.1.1.tar` & `dela-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1345 2023-07-10 15:34:23.747731 dela-0.1.1/README.md
--rw-r--r--   0        0        0      267 2023-07-10 15:34:23.747731 dela-0.1.1/dela/FileReader.py
--rw-r--r--   0        0        0     2958 2023-07-10 15:34:23.747731 dela-0.1.1/dela/ListCommand.py
--rw-r--r--   0        0        0     1248 2023-07-10 15:34:23.747731 dela-0.1.1/dela/Todo.py
--rw-r--r--   0        0        0      521 2023-07-10 15:34:23.747731 dela-0.1.1/dela/TodoPresentation.py
--rw-r--r--   0        0        0        0 2023-07-10 15:34:23.747731 dela-0.1.1/dela/__init__.py
--rw-r--r--   0        0        0     1776 2023-07-10 15:34:23.747731 dela-0.1.1/dela/__main__.py
--rw-r--r--   0        0        0      123 2023-07-10 15:34:23.747731 dela-0.1.1/dela/logger.py
--rw-r--r--   0        0        0      367 2023-07-10 15:34:23.747731 dela-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 dela-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1345 2023-07-10 17:19:17.322883 dela-0.1.2/README.md
+-rw-r--r--   0        0        0      267 2023-07-10 17:19:17.322883 dela-0.1.2/dela/FileReader.py
+-rw-r--r--   0        0        0     3615 2023-07-10 17:19:17.322883 dela-0.1.2/dela/ListCommand.py
+-rw-r--r--   0        0        0     1282 2023-07-10 17:19:17.322883 dela-0.1.2/dela/Todo.py
+-rw-r--r--   0        0        0      580 2023-07-10 17:19:17.322883 dela-0.1.2/dela/TodoPresentation.py
+-rw-r--r--   0        0        0        0 2023-07-10 17:19:17.322883 dela-0.1.2/dela/__init__.py
+-rw-r--r--   0        0        0     1948 2023-07-10 17:19:17.322883 dela-0.1.2/dela/__main__.py
+-rw-r--r--   0        0        0      123 2023-07-10 17:19:17.322883 dela-0.1.2/dela/logger.py
+-rw-r--r--   0        0        0      367 2023-07-10 17:19:17.326884 dela-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 dela-0.1.2/PKG-INFO
```

### Comparing `dela-0.1.1/README.md` & `dela-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dela-0.1.1/dela/ListCommand.py` & `dela-0.1.2/dela/ListCommand.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,89 +8,103 @@
 
 class ListCommandConfig(object):
     def __init__(self, args):
         self.glob = args['<glob>'] if args['<glob>'] else '*.md'
         self.format = (
             args['--format']
             if args['--format']
-            else '\u001b[30m- \u001b[0m\u001b[01m[$status]\u001b[0m \u001b[31m$file:\u001b[0m $title'
+            else '\u001b[30m- \u001b[0m\u001b[01m[$status]\u001b[0m \u001b[31m$file:\u001b[0m $title \u001b[0m\u001b[34m$tags\u001b[0m'
         )
         self.filter_by_status = args['--status'] if args['--status'] else None
         self.show_all = True if args['--all'] else False
         self.sort_by = args['--sort_by'] if args['--sort_by'] else None
         self.only_today = True if args['--today'] else False
         self.only_done = True if args['--done'] else False
+        self.only_someday = True if args['--someday'] else False
+        self.filter_by_tags = args['--tag'] if args['--tag'] else None
 
     def __str__(self):
         return str(self.__class__) + ': ' + str(self.__dict__)
 
 
 class ListCommand:
     def __init__(self, args) -> None:
         self.config = ListCommandConfig(args)
 
     def run(self):
         log.info(f'Execute list command with config: {self.config}')
 
         files = FileReader.get_files(self.config.glob)
-        log.info(f'Match files: {files}')
+        log.debug(f'Match files: {files}')
 
         result = []
         for file_path in files:
-            log.info(f'Parsing file: {file_path}')
+            log.debug(f'Parsing file: {file_path}')
 
             local = []
             for line in FileReader.read_file(file_path):
                 todo = Todo.from_line(line, file_path)
                 if todo:
                     local.append(todo)
 
-            log.info(f'Found {len(local)} todo(s)')
+            if len(local):
+                log.info(f'Parsed file: {file_path}')
+                log.info(f'Found {len(local)} todo(s)')
+                log.info(f'Todos: {local}')
             result += local
 
         result = self.filter(result)
         result = self.sort(result)
 
         presentation = TodoPresentation(self.config.format)
         for i in result:
             presentation.present(i)
 
     def filter(self, todos):
         result = todos
 
-        if not self.config.show_all and not self.config.only_done:
+        if not self.config.show_all and not self.config.only_done and not self.config.only_someday:
             result = [
                 i
                 for i in result
                 if i.status
                 not in [
                     *Todo.STATUSES_DONE,
                     *Todo.STATUSES_ARCHIVED,
                     *Todo.STATUSES_CLOSED,
+                    *Todo.STATUSES_SOMEDAY,
                 ]
             ]
 
+        if self.config.only_someday:
+            result = [i for i in result if i.status in Todo.STATUSES_SOMEDAY]
+
         if self.config.only_done:
             result = [i for i in result if i.status not in Todo.STATUSES_DONE]
 
         if self.config.filter_by_status is not None:
             result = [
                 i for i in result if i.status == self.config.filter_by_status
             ]
 
+        if self.config.filter_by_tags:
+            result = [
+                i for i in result if bool(set(i.tags) & set(self.config.filter_by_tags))
+            ]
+
         if self.config.only_today:
             YYYYmmDD = datetime.now().strftime('%Y%m%d')
             result = [i for i in result if i.date == YYYYmmDD]
 
         return result
 
     def sort(self, todos):
         result = todos
 
         if self.config.sort_by:
             result = sorted(
                 todos,
-                key=lambda x: getattr(x, self.config.sort_by),
                 reverse=True,
-            )   # type: ignore
+                key=lambda x: getattr(x, self.config.sort_by) # type: ignore
+            )
 
         return result
```

### Comparing `dela-0.1.1/dela/Todo.py` & `dela-0.1.2/dela/Todo.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 TODO_RE = '^\s*-\s+\[(?P<status>.{1})\]\s+(?:(?P<date>\d{8})\s+)?(?P<title>.*?)(?:\s+(?P<tagline>#.*))?$'
 
 
 class Todo(object):
     STATUSES_DONE = ['x', 'X']
     STATUSES_ARCHIVED = ['a', 'A']
     STATUSES_CLOSED = ['c', 'C', '-']
+    STATUSES_SOMEDAY = ['s', 'S']
     STATUSES_IN_PROGRESS = ['~']
 
     title = None
     date = None
     file = None
     tags = []
     status = None
```

### Comparing `dela-0.1.1/dela/TodoPresentation.py` & `dela-0.1.2/dela/TodoPresentation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import sys
 import codecs
 from string import Template
 
-# os.system("color")
-
 
 class TodoPresentation:
     def __init__(self, format) -> None:
         self.template = Template(format)
 
     def present(self, todo):
-        str = self.template.substitute(todo.__dict__)
+        context = todo.__dict__
+        context['tags'] = ' '.join(context['tags'])
+
+        str = self.template.substitute(context)
+
         # NOTE: This 2 lines are here to add support for unicode escape
         #       characters like terminal colors, tabs, etc
         str = codecs.decode(str, 'raw-unicode-escape')
         str = str.encode('latin1').decode('utf8')
+
         print(str)
```

### Comparing `dela-0.1.1/dela/__main__.py` & `dela-0.1.2/dela/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 doc = """dela
 
 CLI to list todos in markdown files, like Obsidian Vaults.
 
 Usage:
   dela -h | --help
   dela --version
-  dela list [-v] [--all] [--today] [--done] [--status=<symbol>] [--sort_by=<key>] [--format=<string>] [<glob>]
+  dela list [-v] [--all] [--today] [--done] [--someday] [--status=<symbol>] [--tag=<string>...] [--sort_by=<key>] [--format=<string>] [<glob>]
 
 Options:
   -h --help                     Show this screen
   -v --verbose                  Enable logging
   -a --all                      Show all todos including closed ones
   -t --today                    Show only today tasks
   -d --done                     Show only done tasks
+  --someday                     Show someday tasks marked with [s] status
   -s --status=<symbol>          Filter by status (x, a, c, ~, ...)
+  -tag=<string>                 Filter by tag (#work, #home, etc)
   --sort_by=<key>               Sort by given key
   --format=<string>             Format result with given template string.
   --version                     Show version.
 
 
 Template example:
     dela list --format='- [$status] $file: $title'
```

### Comparing `dela-0.1.1/PKG-INFO` & `dela-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dela
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: 'Anton Shuvalov'
 Author-email: anton@shuvalov.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

