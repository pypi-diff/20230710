# Comparing `tmp/u2p-0.1.0.tar.gz` & `tmp/u2p-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "u2p-0.1.0.tar", last modified: Mon Jul 10 19:36:54 2023, max compression
+gzip compressed data, was "u2p-0.2.0.tar", last modified: Mon Jul 10 20:03:27 2023, max compression
```

## Comparing `u2p-0.1.0.tar` & `u2p-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 19:36:54.549991 u2p-0.1.0/
--rw-r--r--   0 kamilturek   (501) staff       (20)     1055 2023-07-09 03:41:06.000000 u2p-0.1.0/LICENSE
--rw-r--r--   0 kamilturek   (501) staff       (20)       37 2023-07-09 03:39:09.000000 u2p-0.1.0/MANIFEST.in
--rw-r--r--   0 kamilturek   (501) staff       (20)      492 2023-07-10 19:36:54.549851 u2p-0.1.0/PKG-INFO
--rw-r--r--   0 kamilturek   (501) staff       (20)        6 2023-07-08 11:47:52.000000 u2p-0.1.0/README.md
--rw-r--r--   0 kamilturek   (501) staff       (20)      797 2023-07-10 19:15:56.000000 u2p-0.1.0/pyproject.toml
--rw-r--r--   0 kamilturek   (501) staff       (20)       38 2023-07-10 19:36:54.550027 u2p-0.1.0/setup.cfg
-drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 19:36:54.546728 u2p-0.1.0/src/
-drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 19:36:54.547966 u2p-0.1.0/src/u2p/
--rw-r--r--   0 kamilturek   (501) staff       (20)       22 2023-07-09 03:45:31.000000 u2p-0.1.0/src/u2p/__init__.py
--rw-r--r--   0 kamilturek   (501) staff       (20)       49 2023-07-09 03:16:41.000000 u2p-0.1.0/src/u2p/__main__.py
--rw-r--r--   0 kamilturek   (501) staff       (20)      861 2023-07-10 16:28:28.000000 u2p-0.1.0/src/u2p/cli.py
-drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 19:36:54.549200 u2p-0.1.0/src/u2p/transformers/
--rw-r--r--   0 kamilturek   (501) staff       (20)      309 2023-07-08 11:43:18.000000 u2p-0.1.0/src/u2p/transformers/__init__.py
--rw-r--r--   0 kamilturek   (501) staff       (20)     2282 2023-07-08 11:43:16.000000 u2p-0.1.0/src/u2p/transformers/asserts.py
-drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 19:36:54.549649 u2p-0.1.0/src/u2p/transformers/generic/
--rw-r--r--   0 kamilturek   (501) staff       (20)      221 2023-07-08 11:26:35.000000 u2p-0.1.0/src/u2p/transformers/generic/__init__.py
--rw-r--r--   0 kamilturek   (501) staff       (20)     1216 2023-07-09 03:23:43.000000 u2p-0.1.0/src/u2p/transformers/generic/bases.py
--rw-r--r--   0 kamilturek   (501) staff       (20)     1617 2023-07-10 19:15:56.000000 u2p-0.1.0/src/u2p/transformers/generic/imports.py
--rw-r--r--   0 kamilturek   (501) staff       (20)      886 2023-07-08 11:47:43.000000 u2p-0.1.0/src/u2p/transformers/main.py
--rw-r--r--   0 kamilturek   (501) staff       (20)      250 2023-07-08 10:16:26.000000 u2p-0.1.0/src/u2p/utils.py
-drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 19:36:54.548873 u2p-0.1.0/src/u2p.egg-info/
--rw-r--r--   0 kamilturek   (501) staff       (20)      492 2023-07-10 19:36:54.000000 u2p-0.1.0/src/u2p.egg-info/PKG-INFO
--rw-r--r--   0 kamilturek   (501) staff       (20)      517 2023-07-10 19:36:54.000000 u2p-0.1.0/src/u2p.egg-info/SOURCES.txt
--rw-r--r--   0 kamilturek   (501) staff       (20)        1 2023-07-10 19:36:54.000000 u2p-0.1.0/src/u2p.egg-info/dependency_links.txt
--rw-r--r--   0 kamilturek   (501) staff       (20)       36 2023-07-10 19:36:54.000000 u2p-0.1.0/src/u2p.egg-info/entry_points.txt
--rw-r--r--   0 kamilturek   (501) staff       (20)       21 2023-07-10 19:36:54.000000 u2p-0.1.0/src/u2p.egg-info/requires.txt
--rw-r--r--   0 kamilturek   (501) staff       (20)        4 2023-07-10 19:36:54.000000 u2p-0.1.0/src/u2p.egg-info/top_level.txt
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 20:03:27.362933 u2p-0.2.0/
+-rw-r--r--   0 kamilturek   (501) staff       (20)     1055 2023-07-09 03:41:06.000000 u2p-0.2.0/LICENSE
+-rw-r--r--   0 kamilturek   (501) staff       (20)       37 2023-07-09 03:39:09.000000 u2p-0.2.0/MANIFEST.in
+-rw-r--r--   0 kamilturek   (501) staff       (20)      691 2023-07-10 20:03:27.362805 u2p-0.2.0/PKG-INFO
+-rw-r--r--   0 kamilturek   (501) staff       (20)        6 2023-07-08 11:47:52.000000 u2p-0.2.0/README.md
+-rw-r--r--   0 kamilturek   (501) staff       (20)      976 2023-07-10 20:00:11.000000 u2p-0.2.0/pyproject.toml
+-rw-r--r--   0 kamilturek   (501) staff       (20)       38 2023-07-10 20:03:27.362997 u2p-0.2.0/setup.cfg
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 20:03:27.358908 u2p-0.2.0/src/
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 20:03:27.360681 u2p-0.2.0/src/u2p/
+-rw-r--r--   0 kamilturek   (501) staff       (20)       22 2023-07-10 20:00:23.000000 u2p-0.2.0/src/u2p/__init__.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)       49 2023-07-09 03:16:41.000000 u2p-0.2.0/src/u2p/__main__.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)      861 2023-07-10 16:28:28.000000 u2p-0.2.0/src/u2p/cli.py
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 20:03:27.362089 u2p-0.2.0/src/u2p/transformers/
+-rw-r--r--   0 kamilturek   (501) staff       (20)      309 2023-07-08 11:43:18.000000 u2p-0.2.0/src/u2p/transformers/__init__.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)     2408 2023-07-10 19:55:26.000000 u2p-0.2.0/src/u2p/transformers/asserts.py
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 20:03:27.362473 u2p-0.2.0/src/u2p/transformers/generic/
+-rw-r--r--   0 kamilturek   (501) staff       (20)       89 2023-07-10 19:57:32.000000 u2p-0.2.0/src/u2p/transformers/generic/__init__.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)     1452 2023-07-10 19:49:32.000000 u2p-0.2.0/src/u2p/transformers/generic/bases.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)     1170 2023-07-10 19:54:27.000000 u2p-0.2.0/src/u2p/transformers/main.py
+-rw-r--r--   0 kamilturek   (501) staff       (20)      250 2023-07-08 10:16:26.000000 u2p-0.2.0/src/u2p/utils.py
+drwxr-xr-x   0 kamilturek   (501) staff       (20)        0 2023-07-10 20:03:27.361548 u2p-0.2.0/src/u2p.egg-info/
+-rw-r--r--   0 kamilturek   (501) staff       (20)      691 2023-07-10 20:03:27.000000 u2p-0.2.0/src/u2p.egg-info/PKG-INFO
+-rw-r--r--   0 kamilturek   (501) staff       (20)      477 2023-07-10 20:03:27.000000 u2p-0.2.0/src/u2p.egg-info/SOURCES.txt
+-rw-r--r--   0 kamilturek   (501) staff       (20)        1 2023-07-10 20:03:27.000000 u2p-0.2.0/src/u2p.egg-info/dependency_links.txt
+-rw-r--r--   0 kamilturek   (501) staff       (20)       36 2023-07-10 20:03:27.000000 u2p-0.2.0/src/u2p.egg-info/entry_points.txt
+-rw-r--r--   0 kamilturek   (501) staff       (20)       21 2023-07-10 20:03:27.000000 u2p-0.2.0/src/u2p.egg-info/requires.txt
+-rw-r--r--   0 kamilturek   (501) staff       (20)        4 2023-07-10 20:03:27.000000 u2p-0.2.0/src/u2p.egg-info/top_level.txt
```

### Comparing `u2p-0.1.0/LICENSE` & `u2p-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `u2p-0.1.0/pyproject.toml` & `u2p-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 keywords = ["unittest", "pytest", "cst"]
 license = {text = "MIT"}
 dynamic = ["version"]
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "libcst"
 ]
 
 [project.scripts]
```

### Comparing `u2p-0.1.0/src/u2p/cli.py` & `u2p-0.2.0/src/u2p/cli.py`

 * *Files identical despite different names*

### Comparing `u2p-0.1.0/src/u2p/transformers/asserts.py` & `u2p-0.2.0/src/u2p/transformers/asserts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import CodemodContext, ContextAwareTransformer
+from libcst.codemod.visitors import AddImportsVisitor
 
 __all__ = (
     "ReplaceAssertEqualTransfomer",
     "ReplaceAssertTrueTransformer",
     "ReplaceAssertRaisesTransformer",
 )
 
@@ -54,14 +55,15 @@
 
 class ReplaceAssertRaisesTransformer(ContextAwareTransformer):
     def __init__(self, context: CodemodContext) -> None:
         super().__init__(context)
 
     def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
         if m.matches(updated_node.func, AssertRaises):
+            AddImportsVisitor.add_needed_import(self.context, "pytest")
             return updated_node.with_changes(
                 func=cst.Attribute(
                     value=cst.Name(
                         value="pytest",
                     ),
                     attr=cst.Name(
                         value="raises",
```

### Comparing `u2p-0.1.0/src/u2p/transformers/generic/bases.py` & `u2p-0.2.0/src/u2p/transformers/generic/bases.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import functools
+from typing import Callable
+
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import CodemodContext, ContextAwareTransformer
 
 
 class RemoveBaseClassTransformer(ContextAwareTransformer):
     def __init__(self, context: CodemodContext, base: str) -> None:
@@ -12,14 +15,21 @@
             self._base = m.Attribute(
                 value=m.Name(value=value),
                 attr=m.Name(value=attr),
             )
         else:
             self._base = m.Name(value=base)
 
+    @classmethod
+    def for_base_class(
+        cls,
+        base: str,
+    ) -> Callable[[CodemodContext], "RemoveBaseClassTransformer"]:
+        return functools.partial(cls, base=base)
+
     def leave_ClassDef(self, original_node, updated_node):
         updated_bases = [
             base for base in updated_node.bases if not m.matches(base.value, self._base)
         ]
         updated = len(updated_bases) != len(updated_node.bases)
 
         if updated:
```

