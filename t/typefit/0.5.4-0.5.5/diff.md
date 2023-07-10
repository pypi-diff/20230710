# Comparing `tmp/typefit-0.5.4.tar.gz` & `tmp/typefit-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typefit-0.5.4.tar", max compression
+gzip compressed data, was "typefit-0.5.5.tar", max compression
```

## Comparing `typefit-0.5.4.tar` & `typefit-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-07-10 09:42:29.341850 typefit-0.5.4/LICENSE
--rw-r--r--   0        0        0     1477 2023-07-10 09:42:29.341850 typefit-0.5.4/README.md
--rw-r--r--   0        0        0     1351 2023-07-10 09:42:29.345850 typefit-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/__init__.py
--rw-r--r--   0        0        0    15459 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/api.py
--rw-r--r--   0        0        0     2008 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/compat.py
--rw-r--r--   0        0        0     9544 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/fitting.py
--rw-r--r--   0        0        0      453 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/httpx_models.py
--rw-r--r--   0        0        0     2428 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/meta.py
--rw-r--r--   0        0        0     1204 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/narrows.py
--rw-r--r--   0        0        0    23219 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/nodes.py
--rw-r--r--   0        0        0     9722 2023-07-10 09:42:29.349850 typefit-0.5.4/src/typefit/reporting.py
--rw-r--r--   0        0        0     7639 2023-07-10 09:42:29.349850 typefit-0.5.4/src/typefit/serialize.py
--rw-r--r--   0        0        0     2895 2023-07-10 09:42:29.349850 typefit-0.5.4/src/typefit/utils.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 typefit-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-07-10 18:23:22.561514 typefit-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1477 2023-07-10 18:23:22.561514 typefit-0.5.5/README.md
+-rw-r--r--   0        0        0     1351 2023-07-10 18:23:22.561514 typefit-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/__init__.py
+-rw-r--r--   0        0        0    15459 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/api.py
+-rw-r--r--   0        0        0     2008 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/compat.py
+-rw-r--r--   0        0        0     9606 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/fitting.py
+-rw-r--r--   0        0        0      453 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/httpx_models.py
+-rw-r--r--   0        0        0     2428 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/meta.py
+-rw-r--r--   0        0        0     1204 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/narrows.py
+-rw-r--r--   0        0        0    23219 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/nodes.py
+-rw-r--r--   0        0        0     9722 2023-07-10 18:23:22.561514 typefit-0.5.5/src/typefit/reporting.py
+-rw-r--r--   0        0        0     7639 2023-07-10 18:23:22.565513 typefit-0.5.5/src/typefit/serialize.py
+-rw-r--r--   0        0        0     2895 2023-07-10 18:23:22.565513 typefit-0.5.5/src/typefit/utils.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 typefit-0.5.5/PKG-INFO
```

### Comparing `typefit-0.5.4/README.md` & `typefit-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/pyproject.toml` & `typefit-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "typefit"
-version = "0.5.4"
+version = "0.5.5"
 
 description = "Fits JSON values into Python type-anotated objects"
 license = "WTFPL"
 authors = [
     "Rémy Sanchez <remy.sanchez@hyperthese.net>"
 ]
```

### Comparing `typefit-0.5.4/src/typefit/api.py` & `typefit-0.5.5/src/typefit/api.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/src/typefit/compat.py` & `typefit-0.5.5/src/typefit/compat.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/src/typefit/fitting.py` & `typefit-0.5.5/src/typefit/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,19 +176,21 @@
         Raises
         ------
         ValueError
         """
 
         origin = get_origin(t)
 
+        if isinstance(value, LiteralNode):
+            return value.fit(t)
         if origin is Union or origin is UnionType:
             return self._fit_union(t, value)
         elif t is Any:
             return self._fit_any(t, value)
-        elif isinstance(value, (MappingNode, ListNode, LiteralNode)):
+        elif isinstance(value, (MappingNode, ListNode)):
             return value.fit(t)
         elif t is None or t is None.__class__:
             return self._fit_none(t, value)
         elif origin is Literal:
             return self._fit_literal(t, value)
         elif isclass(t):
             if issubclass(t, Enum):
```

### Comparing `typefit-0.5.4/src/typefit/meta.py` & `typefit-0.5.5/src/typefit/meta.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/src/typefit/narrows.py` & `typefit-0.5.5/src/typefit/narrows.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/src/typefit/nodes.py` & `typefit-0.5.5/src/typefit/nodes.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/src/typefit/reporting.py` & `typefit-0.5.5/src/typefit/reporting.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/src/typefit/serialize.py` & `typefit-0.5.5/src/typefit/serialize.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/src/typefit/utils.py` & `typefit-0.5.5/src/typefit/utils.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.4/PKG-INFO` & `typefit-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typefit
-Version: 0.5.4
+Version: 0.5.5
 Summary: Fits JSON values into Python type-anotated objects
 Home-page: https://github.com/Xowap/typefit/
 License: WTFPL
 Keywords: typing,json,api
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
```

