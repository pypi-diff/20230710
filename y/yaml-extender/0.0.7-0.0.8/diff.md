# Comparing `tmp/yaml-extender-0.0.7.tar.gz` & `tmp/yaml-extender-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-extender-0.0.7.tar", last modified: Mon Jun 12 16:44:36 2023, max compression
+gzip compressed data, was "yaml-extender-0.0.8.tar", last modified: Mon Jul 10 13:43:43 2023, max compression
```

## Comparing `yaml-extender-0.0.7.tar` & `yaml-extender-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.593024 yaml-extender-0.0.7/
--rw-rw-rw-   0        0        0      878 2023-06-12 16:43:30.000000 yaml-extender-0.0.7/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7135 2023-06-12 16:44:36.592023 yaml-extender-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4580 2023-01-31 18:06:45.000000 yaml-extender-0.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.559994 yaml-extender-0.0.7/docs/
--rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.0.7/docs/conf.py
--rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 16:44:36.593024 yaml-extender-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.550986 yaml-extender-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.573005 yaml-extender-0.0.7/src/yaml_extender/
--rw-rw-rw-   0        0        0       68 2023-06-12 16:43:36.000000 yaml-extender-0.0.7/src/yaml_extender/__init__.py
--rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.0.7/src/yaml_extender/__main__.py
--rw-rw-rw-   0        0        0     1505 2023-05-11 18:01:55.000000 yaml-extender-0.0.7/src/yaml_extender/cli.py
--rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.0.7/src/yaml_extender/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.592023 yaml-extender-0.0.7/src/yaml_extender/resolver/
--rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/__init__.py
--rw-rw-rw-   0        0        0     5850 2023-06-09 14:42:34.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/include_resolver.py
--rw-rw-rw-   0        0        0     2975 2023-02-27 17:47:13.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/loop_resolver.py
--rw-rw-rw-   0        0        0     6044 2023-06-12 16:41:27.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/reference_resolver.py
--rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/resolver.py
--rw-rw-rw-   0        0        0      469 2023-02-27 18:50:34.000000 yaml-extender-0.0.7/src/yaml_extender/xyml_exception.py
--rw-rw-rw-   0        0        0     1883 2023-05-11 18:04:26.000000 yaml-extender-0.0.7/src/yaml_extender/xyml_file.py
--rw-rw-rw-   0        0        0      963 2023-01-15 11:35:59.000000 yaml-extender-0.0.7/src/yaml_extender/yaml_loader.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.588020 yaml-extender-0.0.7/src/yaml_extender.egg-info/
--rw-rw-rw-   0        0        0     7135 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:43.665813 yaml-extender-0.0.8/
+-rw-rw-rw-   0        0        0     1174 2023-07-10 13:42:54.000000 yaml-extender-0.0.8/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     7135 2023-07-10 13:43:43.664811 yaml-extender-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4580 2023-01-31 18:06:45.000000 yaml-extender-0.0.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:43.607376 yaml-extender-0.0.8/docs/
+-rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.0.8/docs/conf.py
+-rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:43:43.665813 yaml-extender-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:43.596895 yaml-extender-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:43.633929 yaml-extender-0.0.8/src/yaml_extender/
+-rw-rw-rw-   0        0        0       68 2023-07-10 13:42:47.000000 yaml-extender-0.0.8/src/yaml_extender/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.0.8/src/yaml_extender/__main__.py
+-rw-rw-rw-   0        0        0     1505 2023-05-11 18:01:55.000000 yaml-extender-0.0.8/src/yaml_extender/cli.py
+-rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.0.8/src/yaml_extender/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:43.664811 yaml-extender-0.0.8/src/yaml_extender/resolver/
+-rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.0.8/src/yaml_extender/resolver/__init__.py
+-rw-rw-rw-   0        0        0     5809 2023-07-10 13:25:45.000000 yaml-extender-0.0.8/src/yaml_extender/resolver/include_resolver.py
+-rw-rw-rw-   0        0        0     2975 2023-02-27 17:47:13.000000 yaml-extender-0.0.8/src/yaml_extender/resolver/loop_resolver.py
+-rw-rw-rw-   0        0        0     6044 2023-06-12 16:41:27.000000 yaml-extender-0.0.8/src/yaml_extender/resolver/reference_resolver.py
+-rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.0.8/src/yaml_extender/resolver/resolver.py
+-rw-rw-rw-   0        0        0      469 2023-02-27 18:50:34.000000 yaml-extender-0.0.8/src/yaml_extender/xyml_exception.py
+-rw-rw-rw-   0        0        0     1883 2023-05-11 18:04:26.000000 yaml-extender-0.0.8/src/yaml_extender/xyml_file.py
+-rw-rw-rw-   0        0        0      963 2023-01-15 11:35:59.000000 yaml-extender-0.0.8/src/yaml_extender/yaml_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:43:43.646940 yaml-extender-0.0.8/src/yaml_extender.egg-info/
+-rw-rw-rw-   0        0        0     7135 2023-07-10 13:43:43.000000 yaml-extender-0.0.8/src/yaml_extender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2023-07-10 13:43:43.000000 yaml-extender-0.0.8/src/yaml_extender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:43:43.000000 yaml-extender-0.0.8/src/yaml_extender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-10 13:43:43.000000 yaml-extender-0.0.8/src/yaml_extender.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-07-10 13:43:43.000000 yaml-extender-0.0.8/src/yaml_extender.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 13:43:43.000000 yaml-extender-0.0.8/src/yaml_extender.egg-info/top_level.txt
```

### Comparing `yaml-extender-0.0.7/CHANGELOG.rst` & `yaml-extender-0.0.8/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 Changelog
 =========
 
-Version 0.0.6, 2023-05-11
+Version 0.0.8, 2023-07-10
+-----------------------
+
+- Bugfix: Including files, which represent a list value is now possible.
+            + Added additional tests for that
+
+Version 0.0.7, 2023-06-12
 -----------------------
 
 - Changed: occurences of list refs in string will now resolve as whitespace separated string.
 - Changed: resolving lists in lists will now extend the current list.
+
+- Bugfix: Include Resolver will now resolve subsequent values in dicts.
+
+Version 0.0.6, 2023-05-11
+-----------------------
+
 - Added option to enable / disable sorting of yaml keys.
 
 Version 0.0.6, 2023-05-11
 -----------------------
 
 - Added option to enable / disable sorting of yaml keys.
```

### Comparing `yaml-extender-0.0.7/LICENSE` & `yaml-extender-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/PKG-INFO` & `yaml-extender-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.0.7/README.rst` & `yaml-extender-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/docs/conf.py` & `yaml-extender-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/pyproject.toml` & `yaml-extender-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender/cli.py` & `yaml-extender-0.0.8/src/yaml_extender/cli.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender/logger.py` & `yaml-extender-0.0.8/src/yaml_extender/logger.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender/resolver/include_resolver.py` & `yaml-extender-0.0.8/src/yaml_extender/resolver/include_resolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,135 @@
-from __future__ import annotations
-
-import os
-import re
-from pathlib import Path
-from typing import Any, List
-
-from yaml_extender.resolver.reference_resolver import ReferenceResolver
-from yaml_extender.resolver.resolver import Resolver
-from yaml_extender.xyml_exception import ExtYamlError, ExtYamlSyntaxError
-import yaml_extender.logger as logger
-import yaml_extender.yaml_loader as yaml_loader
-
-
-INCLUDE_REGEX = r'([^<]+)\s*(?:<<(.*)>>)?'
-INCLUDE_KEY = "xyml.include"
-
-
-class IncludeResolver(Resolver):
-
-    def __init__(self, include_dirs: List[Path] | None = None, fail_on_resolve: bool = True):
-        if include_dirs:
-            self.include_dirs: List[Path] = include_dirs
-        else:
-            self.include_dirs: List[Path] = []
-        if Path.cwd() not in self.include_dirs:
-            self.include_dirs.append(Path.cwd())
-        super().__init__(fail_on_resolve)
-
-    def _Resolver__resolve(self, cur_value: Any, config: dict) -> dict:
-        return self.__resolve_inc(cur_value, config)
-
-    def __resolve_inc(self, cur_value: Any, config: dict) -> Any:
-        """
-        Resolves all include statements in value
-
-            Returns:
-                The content of the original file with all includes resolved.
-        """
-        if isinstance(cur_value, dict):
-            if INCLUDE_KEY in cur_value:
-                include_content = self.__resolve_include_statement(cur_value[INCLUDE_KEY], config)
-                if isinstance(include_content, dict):
-                    self.update_content_with_include_content(cur_value, include_content)
-                    del cur_value[INCLUDE_KEY]
-                else:
-                    if len(cur_value) > 1:
-                        raise ExtYamlSyntaxError(f"Unable to resolve {cur_value}."
-                                                 f"Included file does not return a dictionary.")
-                    cur_value = include_content
-            for k, v in cur_value.items():
-                cur_value[k] = self.__resolve_inc(cur_value[k], config)
-        elif isinstance(cur_value, list):
-            new_content = []
-            for i, x in enumerate(cur_value):
-                new_value = (self.__resolve_inc(x, config))
-                if isinstance(new_value, list):
-                    new_content.extend(new_value)
-                else:
-                    new_content.append(new_value)
-            if new_content:
-                cur_value = new_content
-        return cur_value
-
-    def __resolve_include_statement(self, value: List | str, config: dict) -> dict:
-        """Resolves an include statement and return the content"""
-        if not isinstance(value, list):
-            statements = [value]
-        else:
-            statements = value
-        # Resolve all references in statement
-        ref_resolver = ReferenceResolver(False)
-        inc_contents = None
-        for statement in statements:
-            statement = ref_resolver.resolve(statement, config)
-            # Resolve include parameters
-            match = re.match(INCLUDE_REGEX, statement)
-            inc_file = match.group(1)
-            # Resolve references in filenames
-            logger.info(f"Resolving Include '{inc_file}'")
-            inc_content = self.__read_included_yaml(inc_file)
-            # Resolve parameters in included file
-            if match.group(2):
-                parameters = self.__parse_include_parameters(match.group(2))
-                inc_content = ref_resolver.resolve(inc_content, parameters)
-            # Add include content to current content
-            include_dirs = self.include_dirs.copy()
-            include_dirs.append(Path(inc_file).parent)
-            inc_resolver = IncludeResolver(include_dirs, self.fail_on_resolve)
-            inc_content = inc_resolver.__resolve_inc(inc_content, config)
-            inc_contents = self.update_inc_content(inc_contents, inc_content)
-        return inc_contents
-
-    def update_content_with_include_content(self, existing_content, include_content):
-        for k, v in include_content.items():
-            if k in existing_content:
-                if isinstance(v, dict):
-                    self.update_content_with_include_content(existing_content[k], v)
-            else:
-                existing_content[k] = v
-
-    def update_inc_content(self, content, include):
-        """Adds include content to existing content based on current datatype"""
-        if content is None:
-            return include
-        if isinstance(include, list):
-            if isinstance(content, dict):
-                content = [content]
-            content.extend(include)
-        elif isinstance(include, dict):
-            if isinstance(content, list):
-                content.append(include)
-            else:
-                content.update(include)
-        else:
-            raise ExtYamlSyntaxError("Resolved include content is not of list or dict type.")
-        return content
-
-    def __parse_include_parameters(self, param_string: str) -> dict:
-        """Parses an include parameter string into a dict"""
-        parameters = {}
-        for param in param_string.split(","):
-            key, value = param.split("=")
-            if not key or not value:
-                raise ExtYamlSyntaxError(f"Invalid parameter string {param_string}")
-            parameters[key.strip()] = yaml_loader.parse_numeric_value(value.strip())
-        return parameters
-
-    def __read_included_yaml(self, file_path: str):
-        # Try path with all include dirs respecting the order
-        file = Path(file_path)
-        if not file.is_absolute():
-            for path in self.include_dirs:
-                file = path / file_path
-                if file.is_file():
-                    return yaml_loader.load(str(file))
-        raise ExtYamlError(f"Include file '{file_path}' not found. Are include directories provided?")
+from __future__ import annotations
+
+import os
+import re
+from pathlib import Path
+from typing import Any, List
+
+from yaml_extender.resolver.reference_resolver import ReferenceResolver
+from yaml_extender.resolver.resolver import Resolver
+from yaml_extender.xyml_exception import ExtYamlError, ExtYamlSyntaxError
+import yaml_extender.logger as logger
+import yaml_extender.yaml_loader as yaml_loader
+
+
+INCLUDE_REGEX = r'([^<]+)\s*(?:<<(.*)>>)?'
+INCLUDE_KEY = "xyml.include"
+
+
+class IncludeResolver(Resolver):
+
+    def __init__(self, include_dirs: List[Path] | None = None, fail_on_resolve: bool = True):
+        if include_dirs:
+            self.include_dirs: List[Path] = include_dirs
+        else:
+            self.include_dirs: List[Path] = []
+        if Path.cwd() not in self.include_dirs:
+            self.include_dirs.append(Path.cwd())
+        super().__init__(fail_on_resolve)
+
+    def _Resolver__resolve(self, cur_value: Any, config: dict) -> dict:
+        return self.__resolve_inc(cur_value, config)
+
+    def __resolve_inc(self, cur_value: Any, config: dict) -> Any:
+        """
+        Resolves all include statements in value
+
+            Returns:
+                The content of the original file with all includes resolved.
+        """
+        if isinstance(cur_value, dict):
+            for k, v in list(cur_value.items()):
+                if k != INCLUDE_KEY:
+                    cur_value[k] = self.__resolve_inc(cur_value[k], config)
+                else:
+                    include_content = self.__resolve_include_statement(cur_value[INCLUDE_KEY], config)
+                    if isinstance(include_content, dict):
+                        self.update_content_with_include_content(cur_value, include_content)
+                        del cur_value[INCLUDE_KEY]
+                    else:
+                        return include_content
+        elif isinstance(cur_value, list):
+            new_content = []
+            for i, x in enumerate(cur_value):
+                new_value = (self.__resolve_inc(x, config))
+                if isinstance(new_value, list):
+                    new_content.extend(new_value)
+                else:
+                    new_content.append(new_value)
+            if new_content:
+                cur_value = new_content
+        return cur_value
+
+    def __resolve_include_statement(self, value: List | str, config: dict) -> dict:
+        """Resolves an include statement and return the content"""
+        if not isinstance(value, list):
+            statements = [value]
+        else:
+            statements = value
+        # Resolve all references in statement
+        ref_resolver = ReferenceResolver(False)
+        inc_contents = None
+        for statement in statements:
+            statement = ref_resolver.resolve(statement, config)
+            # Resolve include parameters
+            match = re.match(INCLUDE_REGEX, statement)
+            inc_file = match.group(1)
+            # Resolve references in filenames
+            logger.info(f"Resolving Include '{inc_file}'")
+            inc_content = self.__read_included_yaml(inc_file)
+            # Resolve parameters in included file
+            if match.group(2):
+                parameters = self.__parse_include_parameters(match.group(2))
+                inc_content = ref_resolver.resolve(inc_content, parameters)
+            # Add include content to current content
+            include_dirs = self.include_dirs.copy()
+            include_dirs.append(Path(inc_file).parent)
+            inc_resolver = IncludeResolver(include_dirs, self.fail_on_resolve)
+            inc_content = inc_resolver.__resolve_inc(inc_content, config)
+            inc_contents = self.update_inc_content(inc_contents, inc_content)
+        return inc_contents
+
+    def update_content_with_include_content(self, existing_content, include_content):
+        for k, v in include_content.items():
+            if k in existing_content:
+                if isinstance(v, dict):
+                    self.update_content_with_include_content(existing_content[k], v)
+            else:
+                existing_content[k] = v
+
+    def update_inc_content(self, content, include):
+        """Adds include content to existing content based on current datatype"""
+        if content is None:
+            return include
+        if isinstance(include, list):
+            if isinstance(content, dict):
+                content = [content]
+            content.extend(include)
+        elif isinstance(include, dict):
+            if isinstance(content, list):
+                content.append(include)
+            else:
+                content.update(include)
+        else:
+            raise ExtYamlSyntaxError("Resolved include content is not of list or dict type.")
+        return content
+
+    def __parse_include_parameters(self, param_string: str) -> dict:
+        """Parses an include parameter string into a dict"""
+        parameters = {}
+        for param in param_string.split(","):
+            key, value = param.split("=")
+            if not key or not value:
+                raise ExtYamlSyntaxError(f"Invalid parameter string {param_string}")
+            parameters[key.strip()] = yaml_loader.parse_numeric_value(value.strip())
+        return parameters
+
+    def __read_included_yaml(self, file_path: str):
+        # Try path with all include dirs respecting the order
+        file = Path(file_path)
+        if not file.is_absolute():
+            for path in self.include_dirs:
+                file = path / file_path
+                if file.is_file():
+                    return yaml_loader.load(str(file))
+        raise ExtYamlError(f"Include file '{file_path}' not found. Are include directories provided?")
```

### Comparing `yaml-extender-0.0.7/src/yaml_extender/resolver/loop_resolver.py` & `yaml-extender-0.0.8/src/yaml_extender/resolver/loop_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender/resolver/reference_resolver.py` & `yaml-extender-0.0.8/src/yaml_extender/resolver/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender/resolver/resolver.py` & `yaml-extender-0.0.8/src/yaml_extender/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender/xyml_file.py` & `yaml-extender-0.0.8/src/yaml_extender/xyml_file.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender/yaml_loader.py` & `yaml-extender-0.0.8/src/yaml_extender/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.7/src/yaml_extender.egg-info/PKG-INFO` & `yaml-extender-0.0.8/src/yaml_extender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.0.7/src/yaml_extender.egg-info/SOURCES.txt` & `yaml-extender-0.0.8/src/yaml_extender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

