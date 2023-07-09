# Comparing `tmp/code-extractor-0.3.0.tar.gz` & `tmp/code-extractor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python_code_extractor/python_code_extractor/dist/.tmp-t23ug6xn/code-extractor-0.3.0.tar", last modified: Tue Dec 13 10:30:26 2022, max compression
+gzip compressed data, was "/home/runner/work/python_code_extractor/python_code_extractor/dist/.tmp-ooo4j068/code-extractor-0.4.0.tar", last modified: Sun Jul  9 23:44:21 2023, max compression
```

## Comparing `code-extractor-0.3.0.tar` & `code-extractor-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:30:26.000000 code-extractor-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-13 10:30:06.000000 code-extractor-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2022-12-13 10:30:26.000000 code-extractor-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2022-12-13 10:30:06.000000 code-extractor-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-13 10:30:06.000000 code-extractor-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2022-12-13 10:30:26.000000 code-extractor-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/extracted_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor/extractor/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/extractor/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/loader/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2022-12-13 10:30:06.000000 code-extractor-0.3.0/src/code_extractor/pickle/pickle_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-13 10:30:26.000000 code-extractor-0.3.0/src/code_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:44:21.000000 code-extractor-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-09 23:44:03.000000 code-extractor-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-09 23:44:21.000000 code-extractor-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-09 23:44:03.000000 code-extractor-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-09 23:44:03.000000 code-extractor-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-09 23:44:21.000000 code-extractor-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/extracted_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor/extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/extractor/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/loader/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-07-09 23:44:03.000000 code-extractor-0.4.0/src/code_extractor/pickle/pickle_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-09 23:44:21.000000 code-extractor-0.4.0/src/code_extractor.egg-info/top_level.txt
```

### Comparing `code-extractor-0.3.0/LICENSE` & `code-extractor-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/PKG-INFO` & `code-extractor-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-extractor
-Version: 0.3.0
+Version: 0.4.0
 Summary: Extract source code from python objects
 Home-page: https://github.com/MatteoH2O1999/python_code_extractor
 Author: MatteoH2O1999
 Author-email: dellacqua.matteo99@gmail.com
 Project-URL: Bug Tracker, https://github.com/MatteoH2O1999/python_code_extractor/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -100,15 +100,15 @@
 ```
 
 ## Pickle module
 
 ```pycon
 >>> import code_extractor
 >>> code_extractor.dump(...)
->>> code_extractor.dumps()
+>>> code_extractor.dumps(...)
 >>> code_extractor.load(...)
 >>> code_extractor.loads(...)
 ```
 
 Or
 
 ```pycon
```

### Comparing `code-extractor-0.3.0/README.md` & `code-extractor-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 ```
 
 ## Pickle module
 
 ```pycon
 >>> import code_extractor
 >>> code_extractor.dump(...)
->>> code_extractor.dumps()
+>>> code_extractor.dumps(...)
 >>> code_extractor.load(...)
 >>> code_extractor.loads(...)
 ```
 
 Or
 
 ```pycon
```

### Comparing `code-extractor-0.3.0/setup.cfg` & `code-extractor-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/src/code_extractor/__init__.py` & `code-extractor-0.4.0/src/code_extractor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 Allows to save python functions and classes and load them without knowing the code.
 
 This exports:
     - extract_code: to extract code to a string
     - load_code: to load code from a string extracted by this package
     - dump, dumps, load, loads: familiar API from the pickle and marshal modules
 """
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 from .extractor.extract import extract_code
 from .loader.load import load_code
 from .pickle import dump, dumps, load, loads
```

### Comparing `code-extractor-0.3.0/src/code_extractor/extracted_code.py` & `code-extractor-0.4.0/src/code_extractor/extracted_code.py`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/src/code_extractor/extractor/__init__.py` & `code-extractor-0.4.0/src/code_extractor/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/src/code_extractor/extractor/extract.py` & `code-extractor-0.4.0/src/code_extractor/extractor/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 Module containing code for extracting source code from live python objects.
 """
 import importlib
 import inspect
+import enum
 import pickle
 import os
 import re
 import site
 import sys
 import textwrap
 
@@ -42,14 +43,30 @@
 from warnings import warn
 
 from ..extracted_code import _ExtractedCode
 
 _MODULE_LOCK: Lock = Lock()
 _SAVED_CODE: Set[str] = set()
 _BUILTINS_MODULE_NAMES: Set[str] = {"__builtin__", "__builtins__", "builtins"}
+_BUILTINS_TYPES: Set[Type[object]] = {
+    bool,
+    int,
+    float,
+    list,
+    tuple,
+    dict,
+    complex,
+    range,
+    str,
+    bytes,
+    bytearray,
+    memoryview,
+    set,
+    frozenset,
+}
 _NESTED_DETECTOR: Pattern[str] = re.compile(
     r"(\A|\n)[\t ]+(async def |def )[a-zA-Z_-]+\([a-zA-Z0-9,:_.-\[\] ]*\)"
 )
 _ADDITIONAL_PATH_KEYWORDS: Set[str] = {os.path.dirname(os.__file__)}
 _USER_BASE: Optional[str] = None
 try:
     _USER_BASE = site.getuserbase()
@@ -203,14 +220,46 @@
                                 possible_module
                             )
                             assert inspect.ismodule(imported_submodule)
                             imports.add(f"import {possible_module}")
                             modules.append(possible_module)
                         except ModuleNotFoundError:
                             pass
+                variables = [(closure_var.__name__, closure_var)]
+                for variable_name, variable in variables:
+                    for possible_other_var in possible_other_vars:
+                        try:
+                            possible_variable = getattr(variable, possible_other_var)
+                        except AttributeError:
+                            continue
+                        if inspect.ismodule(possible_variable):
+                            variables.append(
+                                (
+                                    f"{variable_name}.{possible_other_var}",
+                                    possible_variable,
+                                )
+                            )
+                        elif type(possible_variable) in _BUILTINS_TYPES:
+                            dependencies.add(
+                                f"{variable_name}.{possible_other_var} = {possible_variable}\n"
+                            )
+                        elif isinstance(possible_variable, enum.EnumMeta):
+                            imports.add("import enum")
+                            value = possible_other_var
+                            names = [
+                                (data.name, data.value) for data in possible_variable
+                            ]
+                            dependencies.add(
+                                f"{variable_name}.{value} = enum.Enum(value='{value}', names={names})\n"
+                            )
+        elif isinstance(closure_var, enum.EnumMeta):
+            imports.add("import enum")
+            value = name
+            names = [(data.name, data.value) for data in closure_var]
+            dependencies.add(f"{value} = enum.Enum(value='{value}', names={names})\n")
         elif inspect.isroutine(closure_var) or inspect.isclass(closure_var):
             module = _guess_module(closure_var)
             module_path = getattr(module, "__file__", None)
             if module_path is not None:
                 user_defined = True
                 for possible_path in _POSSIBLE_SITE_PATHS:
                     if possible_path in module_path:
@@ -260,14 +309,16 @@
                 if closure_var.__name__ == name:
                     imports.add(f"from {module.__name__} import {closure_var.__name__}")
                 else:
                     assert "." not in name
                     imports.add(
                         f"from {module.__name__} import {closure_var.__name__} as {name}"
                     )
+        elif type(closure_var) in _BUILTINS_TYPES:
+            dependencies.add(f"{name} = {str(closure_var)}\n")
         else:
             new_dep, new_imp = _pickle(name, closure_var)
             dependencies.update(new_dep)
             imports.update(new_imp)
     for name, closure_var in non_local_closure_vars.items():
         pass
     for name in unbound_closure_vars:
```

### Comparing `code-extractor-0.3.0/src/code_extractor/loader/__init__.py` & `code-extractor-0.4.0/src/code_extractor/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/src/code_extractor/loader/load.py` & `code-extractor-0.4.0/src/code_extractor/loader/load.py`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/src/code_extractor/pickle/__init__.py` & `code-extractor-0.4.0/src/code_extractor/pickle/__init__.py`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/src/code_extractor/pickle/pickle_code.py` & `code-extractor-0.4.0/src/code_extractor/pickle/pickle_code.py`

 * *Files identical despite different names*

### Comparing `code-extractor-0.3.0/src/code_extractor.egg-info/PKG-INFO` & `code-extractor-0.4.0/src/code_extractor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-extractor
-Version: 0.3.0
+Version: 0.4.0
 Summary: Extract source code from python objects
 Home-page: https://github.com/MatteoH2O1999/python_code_extractor
 Author: MatteoH2O1999
 Author-email: dellacqua.matteo99@gmail.com
 Project-URL: Bug Tracker, https://github.com/MatteoH2O1999/python_code_extractor/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -100,15 +100,15 @@
 ```
 
 ## Pickle module
 
 ```pycon
 >>> import code_extractor
 >>> code_extractor.dump(...)
->>> code_extractor.dumps()
+>>> code_extractor.dumps(...)
 >>> code_extractor.load(...)
 >>> code_extractor.loads(...)
 ```
 
 Or
 
 ```pycon
```

