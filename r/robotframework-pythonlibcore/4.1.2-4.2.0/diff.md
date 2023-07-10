# Comparing `tmp/robotframework-pythonlibcore-4.1.2.tar.gz` & `tmp/robotframework-pythonlibcore-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-pythonlibcore-4.1.2.tar", last modified: Fri Feb 17 22:42:17 2023, max compression
+gzip compressed data, was "robotframework-pythonlibcore-4.2.0.tar", last modified: Mon Jul 10 11:28:00 2023, max compression
```

## Comparing `robotframework-pythonlibcore-4.1.2.tar` & `robotframework-pythonlibcore-4.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-02-17 22:42:17.535884 robotframework-pythonlibcore-4.1.2/
--rw-r--r--   0 tatuaalto   (501) staff       (20)      568 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.1.2/COPYRIGHT.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)    11358 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.1.2/LICENSE.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)       34 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.1.2/MANIFEST.in
--rw-r--r--   0 tatuaalto   (501) staff       (20)     6031 2023-02-17 22:42:17.535767 robotframework-pythonlibcore-4.1.2/PKG-INFO
--rw-r--r--   0 tatuaalto   (501) staff       (20)     4888 2023-01-31 20:56:25.000000 robotframework-pythonlibcore-4.1.2/README.rst
--rw-r--r--   0 tatuaalto   (501) staff       (20)       38 2023-02-17 22:42:17.535921 robotframework-pythonlibcore-4.1.2/setup.cfg
--rw-r--r--   0 tatuaalto   (501) staff       (20)     1752 2022-11-05 16:36:24.000000 robotframework-pythonlibcore-4.1.2/setup.py
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-02-17 22:42:17.535009 robotframework-pythonlibcore-4.1.2/src/
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-02-17 22:42:17.535567 robotframework-pythonlibcore-4.1.2/src/robotframework_pythonlibcore.egg-info/
--rw-r--r--   0 tatuaalto   (501) staff       (20)     6031 2023-02-17 22:42:17.000000 robotframework-pythonlibcore-4.1.2/src/robotframework_pythonlibcore.egg-info/PKG-INFO
--rw-r--r--   0 tatuaalto   (501) staff       (20)      301 2023-02-17 22:42:17.000000 robotframework-pythonlibcore-4.1.2/src/robotframework_pythonlibcore.egg-info/SOURCES.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)        1 2023-02-17 22:42:17.000000 robotframework-pythonlibcore-4.1.2/src/robotframework_pythonlibcore.egg-info/dependency_links.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)       13 2023-02-17 22:42:17.000000 robotframework-pythonlibcore-4.1.2/src/robotframework_pythonlibcore.egg-info/top_level.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)    12670 2023-02-17 22:38:07.000000 robotframework-pythonlibcore-4.1.2/src/robotlibcore.py
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-07-10 11:28:00.474680 robotframework-pythonlibcore-4.2.0/
+-rw-r--r--   0 tatuaalto   (501) staff       (20)      568 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.2.0/COPYRIGHT.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)    11358 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.2.0/LICENSE.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       34 2022-10-15 18:35:51.000000 robotframework-pythonlibcore-4.2.0/MANIFEST.in
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     6032 2023-07-10 11:28:00.474564 robotframework-pythonlibcore-4.2.0/PKG-INFO
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     4888 2023-01-31 20:56:25.000000 robotframework-pythonlibcore-4.2.0/README.rst
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       38 2023-07-10 11:28:00.474717 robotframework-pythonlibcore-4.2.0/setup.cfg
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     1753 2023-07-10 11:21:47.000000 robotframework-pythonlibcore-4.2.0/setup.py
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-07-10 11:28:00.473946 robotframework-pythonlibcore-4.2.0/src/
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-07-10 11:28:00.474386 robotframework-pythonlibcore-4.2.0/src/robotframework_pythonlibcore.egg-info/
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     6032 2023-07-10 11:28:00.000000 robotframework-pythonlibcore-4.2.0/src/robotframework_pythonlibcore.egg-info/PKG-INFO
+-rw-r--r--   0 tatuaalto   (501) staff       (20)      301 2023-07-10 11:28:00.000000 robotframework-pythonlibcore-4.2.0/src/robotframework_pythonlibcore.egg-info/SOURCES.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)        1 2023-07-10 11:28:00.000000 robotframework-pythonlibcore-4.2.0/src/robotframework_pythonlibcore.egg-info/dependency_links.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       13 2023-07-10 11:28:00.000000 robotframework-pythonlibcore-4.2.0/src/robotframework_pythonlibcore.egg-info/top_level.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)    13294 2023-07-10 11:27:26.000000 robotframework-pythonlibcore-4.2.0/src/robotlibcore.py
```

### Comparing `robotframework-pythonlibcore-4.1.2/COPYRIGHT.txt` & `robotframework-pythonlibcore-4.2.0/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.1.2/LICENSE.txt` & `robotframework-pythonlibcore-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.1.2/PKG-INFO` & `robotframework-pythonlibcore-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: robotframework-pythonlibcore
-Version: 4.1.2
+Version: 4.2.0
 Summary: Tools to ease creating larger test libraries for Robot Framework using Python.
 Home-page: https://github.com/robotframework/PythonLibCore
 Author: Tatu Aalto
 Author-email: aalto.tatu@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation library development
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.7, <4
 License-File: LICENSE.txt
```

### Comparing `robotframework-pythonlibcore-4.1.2/README.rst` & `robotframework-pythonlibcore-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-pythonlibcore-4.1.2/setup.py` & `robotframework-pythonlibcore-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 CURDIR = dirname(abspath(__file__))
 
 CLASSIFIERS = """
 Development Status :: 5 - Production/Stable
 License :: OSI Approved :: Apache Software License
 Operating System :: OS Independent
 Programming Language :: Python :: 3
-Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Programming Language :: Python :: 3 :: Only
 Programming Language :: Python :: Implementation :: CPython
 Programming Language :: Python :: Implementation :: PyPy
 Topic :: Software Development :: Testing
 Framework :: Robot Framework
 """.strip().splitlines()
 with open(join(CURDIR, 'src', 'robotlibcore.py')) as f:
```

### Comparing `robotframework-pythonlibcore-4.1.2/src/robotframework_pythonlibcore.egg-info/PKG-INFO` & `robotframework-pythonlibcore-4.2.0/src/robotframework_pythonlibcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: robotframework-pythonlibcore
-Version: 4.1.2
+Version: 4.2.0
 Summary: Tools to ease creating larger test libraries for Robot Framework using Python.
 Home-page: https://github.com/robotframework/PythonLibCore
 Author: Tatu Aalto
 Author-email: aalto.tatu@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation library development
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.7, <4
 License-File: LICENSE.txt
```

### Comparing `robotframework-pythonlibcore-4.1.2/src/robotlibcore.py` & `robotframework-pythonlibcore-4.2.0/src/robotlibcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,42 +17,46 @@
 Main usage is easing creating larger test libraries. For more information and
 examples see the project pages at
 https://github.com/robotframework/PythonLibCore
 """
 import inspect
 import os
 from dataclasses import dataclass
-from typing import Any, Callable, List, Optional, get_type_hints
+from typing import Any, Callable, List, Optional, Union, get_type_hints
 
 from robot.api.deco import keyword  # noqa F401
 from robot.errors import DataError
 from robot.utils import Importer  # noqa F401
 
-__version__ = "4.1.2"
+__version__ = "4.2.0"
 
 
 class PythonLibCoreException(Exception):
     pass
 
 
 class PluginError(PythonLibCoreException):
     pass
 
 
+class NoKeywordFound(PythonLibCoreException):
+    pass
+
+
 class HybridCore:
     def __init__(self, library_components):
         self.keywords = {}
         self.keywords_spec = {}
         self.attributes = {}
         self.add_library_components(library_components)
         self.add_library_components([self])
         self.__set_library_listeners(library_components)
 
     def add_library_components(self, library_components):
-        self.keywords_spec["__init__"] = KeywordBuilder.build(self.__init__)
+        self.keywords_spec["__init__"] = KeywordBuilder.build(self.__init__)  # type: ignore
         for component in library_components:
             for name, func in self.__get_members(component):
                 if callable(func) and hasattr(func, "robot_name"):
                     kw = getattr(component, name)
                     kw_name = func.robot_name or name
                     self.keywords[kw_name] = kw
                     self.keywords_spec[kw_name] = KeywordBuilder.build(kw)
@@ -119,34 +123,38 @@
 
 class DynamicCore(HybridCore):
     def run_keyword(self, name, args, kwargs=None):
         return self.keywords[name](*args, **(kwargs or {}))
 
     def get_keyword_arguments(self, name):
         spec = self.keywords_spec.get(name)
+        if not spec:
+            raise NoKeywordFound(f"Could not find keyword: {name}")
         return spec.argument_specification
 
     def get_keyword_tags(self, name):
         return self.keywords[name].robot_tags
 
     def get_keyword_documentation(self, name):
         if name == "__intro__":
             return inspect.getdoc(self) or ""
         spec = self.keywords_spec.get(name)
+        if not spec:
+            raise NoKeywordFound(f"Could not find keyword: {name}")
         return spec.documentation
 
     def get_keyword_types(self, name):
         spec = self.keywords_spec.get(name)
         if spec is None:
             raise ValueError('Keyword "%s" not found.' % name)
         return spec.argument_types
 
     def __get_keyword(self, keyword_name):
         if keyword_name == "__init__":
-            return self.__init__
+            return self.__init__  # type: ignore
         if keyword_name.startswith("__") and keyword_name.endswith("__"):
             return None
         method = self.keywords.get(keyword_name)
         if not method:
             raise ValueError('Keyword "%s" not found.' % keyword_name)
         return method
 
@@ -199,50 +207,50 @@
         argument_specification = cls._get_args(arg_spec, function)
         argument_specification.extend(cls._get_varargs(arg_spec))
         argument_specification.extend(cls._get_named_only_args(arg_spec))
         argument_specification.extend(cls._get_kwargs(arg_spec))
         return argument_specification
 
     @classmethod
-    def _get_arg_spec(cls, function: Callable):
+    def _get_arg_spec(cls, function: Callable) -> inspect.FullArgSpec:
         return inspect.getfullargspec(function)
 
     @classmethod
-    def _get_args(cls, arg_spec: inspect.FullArgSpec, function: Callable):
+    def _get_args(cls, arg_spec: inspect.FullArgSpec, function: Callable) -> list:
         args = cls._drop_self_from_args(function, arg_spec)
         args.reverse()
         defaults = list(arg_spec.defaults) if arg_spec.defaults else []
         formated_args = []
         for arg in args:
             if defaults:
                 formated_args.append((arg, defaults.pop()))
             else:
                 formated_args.append(arg)
         formated_args.reverse()
         return formated_args
 
     @classmethod
-    def _drop_self_from_args(cls, function: Callable, arg_spec: inspect.FullArgSpec):
+    def _drop_self_from_args(cls, function: Callable, arg_spec: inspect.FullArgSpec) -> list:
         return arg_spec.args[1:] if inspect.ismethod(function) else arg_spec.args
 
     @classmethod
     def _get_varargs(cls, arg_spec: inspect.FullArgSpec) -> list:
         return [f"*{arg_spec.varargs}"] if arg_spec.varargs else []
 
     @classmethod
     def _get_kwargs(cls, arg_spec: inspect.FullArgSpec) -> list:
         return [f"**{arg_spec.varkw}"] if arg_spec.varkw else []
 
     @classmethod
     def _get_named_only_args(cls, arg_spec: inspect.FullArgSpec) -> list:
-        rf_spec = []
+        rf_spec: list = []
         kw_only_args = arg_spec.kwonlyargs if arg_spec.kwonlyargs else []
         if not arg_spec.varargs and kw_only_args:
             rf_spec.append("*")
-        kw_only_defaults = arg_spec.kwonlydefaults if arg_spec.kwonlydefaults else []
+        kw_only_defaults = arg_spec.kwonlydefaults if arg_spec.kwonlydefaults else {}
         for kw_only_arg in kw_only_args:
             if kw_only_arg in kw_only_defaults:
                 rf_spec.append((kw_only_arg, kw_only_defaults[kw_only_arg]))
             else:
                 rf_spec.append(kw_only_arg)
         return rf_spec
 
@@ -267,17 +275,16 @@
         for arg_with_hint in list(hints):
             # remove return and self statements
             if arg_with_hint not in all_args:
                 hints.pop(arg_with_hint)
         return hints
 
     @classmethod
-    def _args_as_list(cls, function, arg_spec):
-        function_args = []
-        function_args.extend(cls._drop_self_from_args(function, arg_spec))
+    def _args_as_list(cls, function, arg_spec) -> list:
+        function_args = cls._drop_self_from_args(function, arg_spec)
         if arg_spec.varargs:
             function_args.append(arg_spec.varargs)
         function_args.extend(arg_spec.kwonlyargs or [])
         if arg_spec.varkw:
             function_args.append(arg_spec.varkw)
         return function_args
 
@@ -293,19 +300,19 @@
     def __init__(self, argument_specification=None, documentation=None, argument_types=None):
         self.argument_specification = argument_specification
         self.documentation = documentation
         self.argument_types = argument_types
 
 
 class PluginParser:
-    def __init__(self, base_class: Optional[Any] = None, python_object: List[Any] = []):
+    def __init__(self, base_class: Optional[Any] = None, python_object=None):
         self._base_class = base_class
-        self._python_object = python_object
+        self._python_object = python_object if python_object else []
 
-    def parse_plugins(self, plugins: str) -> List:
+    def parse_plugins(self, plugins: Union[str, List[str]]) -> List:
         imported_plugins = []
         importer = Importer("test library")
         for parsed_plugin in self._string_to_modules(plugins):
             plugin = importer.import_class_or_module(parsed_plugin.module)
             if not inspect.isclass(plugin):
                 message = f"Importing test library: '{parsed_plugin.module}' failed."
                 raise DataError(message)
@@ -316,26 +323,34 @@
                 raise PluginError(message)
             imported_plugins.append(plugin)
         return imported_plugins
 
     def get_plugin_keywords(self, plugins: List):
         return DynamicCore(plugins).get_keyword_names()
 
-    def _string_to_modules(self, modules):
-        parsed_modules = []
+    def _string_to_modules(self, modules: Union[str, List[str]]):
+        parsed_modules: list = []
         if not modules:
             return parsed_modules
-        for module in modules.split(","):
+        for module in self._modules_splitter(modules):
             module = module.strip()
             module_and_args = module.split(";")
             module_name = module_and_args.pop(0)
             kw_args = {}
             args = []
             for argument in module_and_args:
                 if "=" in argument:
                     key, value = argument.split("=")
                     kw_args[key] = value
                 else:
                     args.append(argument)
             module = Module(module=module_name, args=args, kw_args=kw_args)
             parsed_modules.append(module)
         return parsed_modules
+
+    def _modules_splitter(self, modules: Union[str, List[str]]):
+        if isinstance(modules, str):
+            for module in modules.split(","):
+                yield module
+        else:
+            for module in modules:
+                yield module
```

