# Comparing `tmp/task2b-1.0.5.tar.gz` & `tmp/task2b-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2b-1.0.5.tar", max compression
+gzip compressed data, was "task2b-1.0.6.tar", max compression
```

## Comparing `task2b-1.0.5.tar` & `task2b-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.5/LICENSE
--rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.5/pwgen2/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.5/pwgen2/__main__.py
--rw-r--r--   0        0        0       23 2023-07-10 21:08:09.396534 task2b-1.0.5/pwgen2/__version__.py
--rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.5/pwgen2/cli/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.5/pwgen2/cli/__main__.py
--rw-r--r--   0        0        0     4664 2023-07-10 15:53:00.202469 task2b-1.0.5/pwgen2/cli/cli.py
--rw-r--r--   0        0        0    10100 2023-07-10 20:52:19.816687 task2b-1.0.5/pwgen2/pwgen2.py
--rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.5/pwgen2/showcase/__init__.py
--rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.5/pwgen2/showcase/__main__.py
--rw-r--r--   0        0        0      132 2023-07-10 16:39:29.431805 task2b-1.0.5/pwgen2/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      284 2023-07-10 16:39:29.435804 task2b-1.0.5/pwgen2/showcase/pattern-list.txt
--rw-r--r--   0        0        0    22956 2023-07-10 21:06:49.720903 task2b-1.0.5/pwgen2/showcase/showcase.py
--rw-r--r--   0        0        0      587 2023-07-10 21:08:09.401545 task2b-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    17418 2023-07-10 20:13:20.833667 task2b-1.0.5/README.md
--rw-r--r--   0        0        0    17813 1970-01-01 00:00:00.000000 task2b-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.6/LICENSE
+-rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.6/pwgen2/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.6/pwgen2/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-10 21:23:24.406425 task2b-1.0.6/pwgen2/__version__.py
+-rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.6/pwgen2/cli/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.6/pwgen2/cli/__main__.py
+-rw-r--r--   0        0        0     4664 2023-07-10 15:53:00.202469 task2b-1.0.6/pwgen2/cli/cli.py
+-rw-r--r--   0        0        0    10100 2023-07-10 20:52:19.816687 task2b-1.0.6/pwgen2/pwgen2.py
+-rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.6/pwgen2/showcase/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.6/pwgen2/showcase/__main__.py
+-rw-r--r--   0        0        0      132 2023-07-10 16:39:29.431805 task2b-1.0.6/pwgen2/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      284 2023-07-10 16:39:29.435804 task2b-1.0.6/pwgen2/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    23063 2023-07-10 21:23:24.415425 task2b-1.0.6/pwgen2/showcase/showcase.py
+-rw-r--r--   0        0        0      587 2023-07-10 21:23:24.410425 task2b-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    17418 2023-07-10 20:13:20.833667 task2b-1.0.6/README.md
+-rw-r--r--   0        0        0    17813 1970-01-01 00:00:00.000000 task2b-1.0.6/PKG-INFO
```

### Comparing `task2b-1.0.5/pwgen2/cli/cli.py` & `task2b-1.0.6/pwgen2/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.5/pwgen2/pwgen2.py` & `task2b-1.0.6/pwgen2/pwgen2.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.5/pwgen2/showcase/showcase.py` & `task2b-1.0.6/pwgen2/showcase/showcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 
 # Determine the platform
 current_platform = platform.system()
 
 # Set the Python command based on the platform
 if current_platform == 'Windows':
     python_command = 'python -m'
+    bash_symbol = '$'
 else:
     python_command = 'python3 -m'
+    bash_symbol = '\$'
 
 select_style = questionary.Style([
     #     ('default', "bg:#ffffff fg:#000000"),
     # ('selected', 'bg:#336699 fg:#ffffff'),
     ('highlighted', '#008888'),
     ('pointer', '#008888'),
     # ('question', 'fg:#009b06'),
@@ -133,15 +135,15 @@
                 'command': 'pwgen2 -S dp -n{} -c{} {}',
                 'module_command': f'{python_command} pwgen2 -S dp -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
             'charset_additional': {
                 'descr': 'custom charset with additional symbols',
                 'command': 'pwgen2 -S "u\\@\\$\\%\\&\\#\\*\\!" -n{} -c{} {}',
-                'module_command': f'{python_command} pwgen2 -S "u\\@\\$\\%\\&\\#\\*\\!" -n{{}} -c{{}} {{}}',
+                'module_command': f'{python_command} pwgen2 -S "u\\@\\{bash_symbol}\\%\\&\\#\\*\\!" -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
             },
             'charset_exclusions': {
                 'descr': 'custom charset with exclusions',
                 'command': 'pwgen2 -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{} -c{} {}',
                 'module_command': f'{python_command} pwgen2 -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n{{}} -c{{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['n'], OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['v'], ],
@@ -174,29 +176,29 @@
                 'command': 'pwgen2 -t u{{4}}[pd]{{3}}l{{2}} -c{} {} {}',
                 'module_command': f'{python_command} pwgen2 -t u{{{{4}}}}[pd]{{{{3}}}}l{{{{2}}}} -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_custom_charset_specific': {
                 'descr': 'pattern with a custom charset with a specific symbol placeholder',
                 'command': 'pwgen2 -t "u{{4}}[pd\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
-                'module_command': f'{python_command} pwgen2 -t "u{{{{4}}}}[pd\\@\\$\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
+                'module_command': f'{python_command} pwgen2 -t "u{{{{4}}}}[pd\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_custom_charset_exclusions': {
                 'descr': 'pattern with a custom charset placeholder with exclusions',
                 'command': 'pwgen2 -t "u{{4}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{3}}l{{2}}" -c{} {} {}',
                 'module_command': f'{python_command} pwgen2 -t "u{{{{4}}}}[Ld^l^\\4^\\5^\\6^\\7^\\8]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'pattern_complex': {
                 'descr': 'complex pattern',
                 'command':
                     'pwgen2 -t "u{{4}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
                 'module_command':
-                    f'{python_command} pwgen2 -t "u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\$\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
+                    f'{python_command} pwgen2 -t "u{{{{4}}}}\\-[Ld^l^\\4^\\5^\\6^\\7^\\8\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
         },
     },
     'file': {
         'descr': 'pattern from a file',
         'command': 'pwgen2 -f {} -c{} {} {}',
@@ -278,21 +280,21 @@
                 'command': 'pwgen2 -t "HH\\-HH\\-HH\\-HH\\-HH\\-HH" -c{} {} {}',
                 'module_command': f'{python_command} pwgen2 -t "HH\\-HH\\-HH\\-HH\\-HH\\-HH" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'choose_one': {
                 'descr': 'pattern with a placeholder to choose from two',
                 'command': 'pwgen2 -t "u{{4}}|[pd\\@\\$\\%\\&\\#\\*\\!]{{3}}l{{2}}" -c{} {} {}',
-                'module_command': f'{python_command} pwgen2 -t "u{{{{4}}}}|[pd\\@\\$\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
+                'module_command': f'{python_command} pwgen2 -t "u{{{{4}}}}|[pd\\@\\{bash_symbol}\\%\\&\\#\\*\\!]{{{{3}}}}l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
             'symbol_space': {
                 'descr': 'pattern with a space character \\ ',
                 'command': 'pwgen2 -t "u{{4}}[pd\\@\\$\\%\\&\\ \\#\\*\\!]{{3}}\\ l{{2}}" -c{} {} {}',
-                'module_command': f'{python_command} pwgen2 -t "u{{{{4}}}}[pd\\@\\$\\%\\&\\ \\#\\*\\!]{{{{3}}}}\\ l{{{{2}}}}" -c{{}} {{}} {{}}',
+                'module_command': f'{python_command} pwgen2 -t "u{{{{4}}}}[pd\\@\\{bash_symbol}\\%\\&\\ \\#\\*\\!]{{{{3}}}}\\ l{{{{2}}}}" -c{{}} {{}} {{}}',
                 'arguments': [OPTIONS_ARGUMENTS['c'], OPTIONS_ARGUMENTS['p'], OPTIONS_ARGUMENTS['v'], ],
             },
         }
     },
 }
 
 questions = [
```

### Comparing `task2b-1.0.5/pyproject.toml` & `task2b-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task2b"
-version = "1.0.5"
+version = "1.0.6"
 description = "Password generation CLI and library version 2"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen2"}]
 license = "MIT"
```

### Comparing `task2b-1.0.5/README.md` & `task2b-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `task2b-1.0.5/PKG-INFO` & `task2b-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2b
-Version: 1.0.5
+Version: 1.0.6
 Summary: Password generation CLI and library version 2
 Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task2b Version: 1.0.5 Summary: Password generation
+Metadata-Version: 2.1 Name: task2b Version: 1.0.6 Summary: Password generation
 CLI and library version 2 Home-page: https://gitlab.com/Bill-EPAM-
 DevOpsInt2023/python/task2b License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
```

