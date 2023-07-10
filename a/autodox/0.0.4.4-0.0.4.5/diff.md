# Comparing `tmp/autodox-0.0.4.4.tar.gz` & `tmp/autodox-0.0.4.5.tar.gz`

## Comparing `autodox-0.0.4.4.tar` & `autodox-0.0.4.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autodox-0.0.4.4/autodox/__init__.py
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 autodox-0.0.4.4/autodox/functions.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 autodox-0.0.4.4/tests/context.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 autodox-0.0.4.4/tests/test_hooks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.4.4/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 autodox-0.0.4.4/license
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.4.4/pyproject.toml
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 autodox-0.0.4.4/readme.md
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 autodox-0.0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 autodox-0.0.4.5/autodox/__init__.py
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 autodox-0.0.4.5/autodox/functions.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 autodox-0.0.4.5/tests/context.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 autodox-0.0.4.5/tests/test_hooks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 autodox-0.0.4.5/.gitignore
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 autodox-0.0.4.5/license
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 autodox-0.0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 autodox-0.0.4.5/readme.md
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 autodox-0.0.4.5/PKG-INFO
```

### Comparing `autodox-0.0.4.4/autodox/functions.py` & `autodox-0.0.4.5/autodox/functions.py`

 * *Files identical despite different names*

### Comparing `autodox-0.0.4.4/tests/test_hooks.py` & `autodox-0.0.4.5/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `autodox-0.0.4.4/pyproject.toml` & `autodox-0.0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autodox"
-version = "0.0.4.4"
+version = "0.0.4.5"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Tool for generating documentation automatically from code annotations, types, and docstrings."
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `autodox-0.0.4.4/readme.md` & `autodox-0.0.4.5/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 documentation function(s). The following are included.
 
 - `dox_a_module(module: ModuleType, options: dict = None) -> str` produces docs for a module
 - `dox_a_value(value: Any, options: dict = None) -> str` produces docs for a value
 - `dox_a_function(function: Callable, options: dict = None) -> str` produces docs for a function
 - `dox_a_class(cls: type, options: dict = None) -> str` produces docs for a class
 
-The valid options will for each will be described below. Additionally, there is
-a system for setting up hooks that interact with the doc generation process to
+The valid options for each will be described below. Additionally, there is a
+system for setting up hooks that interact with the doc generation process to
 change the inputs or outputs, and that will be described below the options for
 the four `dox_a_{thing}` functions.
 
 #### `dox_a_module(module: ModuleType, options: dict = None) -> str`
 
 Produces docs for a module. Valid options are the following:
 
@@ -172,21 +172,14 @@
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
 that the above copyleft notice and this permission notice appear in
 all copies.
 
-Exceptions: this permission is not granted to Alphabet/Google, Amazon,
-Apple, Microsoft, Netflix, Meta/Facebook, Twitter, or Disney; nor is
-permission granted to any company that contracts to supply weapons or
-logistics to any national military; nor is permission granted to any
-national government or governmental agency; nor is permission granted to
-any employees, associates, or affiliates of these designated entities.
-
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL
 WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE
 AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR
 CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS
 OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT,
 NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
```

### Comparing `autodox-0.0.4.4/PKG-INFO` & `autodox-0.0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodox
-Version: 0.0.4.4
+Version: 0.0.4.5
 Summary: Tool for generating documentation automatically from code annotations, types, and docstrings.
 Project-URL: Homepage, https://github.com/k98kurz/autodox
 Project-URL: Bug Tracker, https://github.com/k98kurz/autodox/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -66,16 +66,16 @@
 documentation function(s). The following are included.
 
 - `dox_a_module(module: ModuleType, options: dict = None) -> str` produces docs for a module
 - `dox_a_value(value: Any, options: dict = None) -> str` produces docs for a value
 - `dox_a_function(function: Callable, options: dict = None) -> str` produces docs for a function
 - `dox_a_class(cls: type, options: dict = None) -> str` produces docs for a class
 
-The valid options will for each will be described below. Additionally, there is
-a system for setting up hooks that interact with the doc generation process to
+The valid options for each will be described below. Additionally, there is a
+system for setting up hooks that interact with the doc generation process to
 change the inputs or outputs, and that will be described below the options for
 the four `dox_a_{thing}` functions.
 
 #### `dox_a_module(module: ModuleType, options: dict = None) -> str`
 
 Produces docs for a module. Valid options are the following:
 
@@ -188,21 +188,14 @@
 Copyleft (c) 2023 k98kurz
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
 that the above copyleft notice and this permission notice appear in
 all copies.
 
-Exceptions: this permission is not granted to Alphabet/Google, Amazon,
-Apple, Microsoft, Netflix, Meta/Facebook, Twitter, or Disney; nor is
-permission granted to any company that contracts to supply weapons or
-logistics to any national military; nor is permission granted to any
-national government or governmental agency; nor is permission granted to
-any employees, associates, or affiliates of these designated entities.
-
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL
 WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE
 AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR
 CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS
 OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT,
 NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
```

