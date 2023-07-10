# Comparing `tmp/immutable_builder-0.1.0.tar.gz` & `tmp/immutable_builder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immutable_builder-0.1.0.tar", max compression
+gzip compressed data, was "immutable_builder-0.1.1.tar", max compression
```

## Comparing `immutable_builder-0.1.0.tar` & `immutable_builder-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1748 2023-07-10 21:35:09.282791 immutable_builder-0.1.0/README.md
--rw-r--r--   0        0        0      394 2023-07-10 21:37:41.569738 immutable_builder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4067 2023-07-10 21:33:32.313248 immutable_builder-0.1.0/src/immutable-builder/builder.py
--rw-r--r--   0        0        0      340 2023-07-10 20:48:13.143480 immutable_builder-0.1.0/src/immutable-builder/reflect.py
--rw-r--r--   0        0        0     2593 2023-07-10 21:33:32.300248 immutable_builder-0.1.0/src/immutable-builder/registry.py
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 immutable_builder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1811 2023-07-10 21:41:02.240985 immutable_builder-0.1.1/README.md
+-rw-r--r--   0        0        0      394 2023-07-10 21:41:11.942045 immutable_builder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4067 2023-07-10 21:33:32.313248 immutable_builder-0.1.1/src/immutable-builder/builder.py
+-rw-r--r--   0        0        0      340 2023-07-10 20:48:13.143480 immutable_builder-0.1.1/src/immutable-builder/reflect.py
+-rw-r--r--   0        0        0     2593 2023-07-10 21:33:32.300248 immutable_builder-0.1.1/src/immutable-builder/registry.py
+-rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 immutable_builder-0.1.1/PKG-INFO
```

### Comparing `immutable_builder-0.1.0/README.md` & `immutable_builder-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # builder
 
+https://pypi.org/project/immutable-builder/
+
 Carbon copy of https://github.com/lann/builder for making a Python NoSQL query builder.
 
 Installing:
 ```python
-poetry add 
+poetry add immutable-builder 
 ```
 
 Example:
 
 ```python
 from builder import Builder, get_struct, registry
 from pprint import pprint
```

### Comparing `immutable_builder-0.1.0/src/immutable-builder/builder.py` & `immutable_builder-0.1.1/src/immutable-builder/builder.py`

 * *Files identical despite different names*

### Comparing `immutable_builder-0.1.0/src/immutable-builder/registry.py` & `immutable_builder-0.1.1/src/immutable-builder/registry.py`

 * *Files identical despite different names*

### Comparing `immutable_builder-0.1.0/PKG-INFO` & `immutable_builder-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: immutable-builder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Immutable builder, carbon copy of lann/builder package in GoLang.
 Author: damacaner
 Author-email: caner@damacana.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # builder
 
+https://pypi.org/project/immutable-builder/
+
 Carbon copy of https://github.com/lann/builder for making a Python NoSQL query builder.
 
 Installing:
 ```python
-poetry add 
+poetry add immutable-builder 
 ```
 
 Example:
 
 ```python
 from builder import Builder, get_struct, registry
 from pprint import pprint
```

