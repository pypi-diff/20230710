# Comparing `tmp/typefit-0.5.3.tar.gz` & `tmp/typefit-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typefit-0.5.3.tar", max compression
+gzip compressed data, was "typefit-0.5.4.tar", max compression
```

## Comparing `typefit-0.5.3.tar` & `typefit-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-07-08 23:10:16.689586 typefit-0.5.3/LICENSE
--rw-r--r--   0        0        0     1477 2023-07-08 23:10:16.689586 typefit-0.5.3/README.md
--rw-r--r--   0        0        0     1351 2023-07-08 23:10:16.693586 typefit-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      268 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/__init__.py
--rw-r--r--   0        0        0    15459 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/api.py
--rw-r--r--   0        0        0     2008 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/compat.py
--rw-r--r--   0        0        0     9544 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/fitting.py
--rw-r--r--   0        0        0      453 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/httpx_models.py
--rw-r--r--   0        0        0     2428 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/meta.py
--rw-r--r--   0        0        0     1204 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/narrows.py
--rw-r--r--   0        0        0    23219 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/nodes.py
--rw-r--r--   0        0        0     9722 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/reporting.py
--rw-r--r--   0        0        0     7517 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/serialize.py
--rw-r--r--   0        0        0     2895 2023-07-08 23:10:16.693586 typefit-0.5.3/src/typefit/utils.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 typefit-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-07-10 09:42:29.341850 typefit-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1477 2023-07-10 09:42:29.341850 typefit-0.5.4/README.md
+-rw-r--r--   0        0        0     1351 2023-07-10 09:42:29.345850 typefit-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/__init__.py
+-rw-r--r--   0        0        0    15459 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/api.py
+-rw-r--r--   0        0        0     2008 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/compat.py
+-rw-r--r--   0        0        0     9544 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/fitting.py
+-rw-r--r--   0        0        0      453 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/httpx_models.py
+-rw-r--r--   0        0        0     2428 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/meta.py
+-rw-r--r--   0        0        0     1204 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/narrows.py
+-rw-r--r--   0        0        0    23219 2023-07-10 09:42:29.345850 typefit-0.5.4/src/typefit/nodes.py
+-rw-r--r--   0        0        0     9722 2023-07-10 09:42:29.349850 typefit-0.5.4/src/typefit/reporting.py
+-rw-r--r--   0        0        0     7639 2023-07-10 09:42:29.349850 typefit-0.5.4/src/typefit/serialize.py
+-rw-r--r--   0        0        0     2895 2023-07-10 09:42:29.349850 typefit-0.5.4/src/typefit/utils.py
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 typefit-0.5.4/PKG-INFO
```

### Comparing `typefit-0.5.3/README.md` & `typefit-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/pyproject.toml` & `typefit-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "typefit"
-version = "0.5.3"
+version = "0.5.4"
 
 description = "Fits JSON values into Python type-anotated objects"
 license = "WTFPL"
 authors = [
     "Rémy Sanchez <remy.sanchez@hyperthese.net>"
 ]
```

### Comparing `typefit-0.5.3/src/typefit/api.py` & `typefit-0.5.4/src/typefit/api.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/src/typefit/compat.py` & `typefit-0.5.4/src/typefit/compat.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/src/typefit/fitting.py` & `typefit-0.5.4/src/typefit/fitting.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/src/typefit/meta.py` & `typefit-0.5.4/src/typefit/meta.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/src/typefit/narrows.py` & `typefit-0.5.4/src/typefit/narrows.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/src/typefit/nodes.py` & `typefit-0.5.4/src/typefit/nodes.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/src/typefit/reporting.py` & `typefit-0.5.4/src/typefit/reporting.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/src/typefit/serialize.py` & `typefit-0.5.4/src/typefit/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,22 +117,26 @@
         superposed into a single dictionary and returned.
 
         All values of this dictionary are of course recursively serialized.
         """
 
         def _get_values():
             for field in fields(obj.__class__):
-                if field.metadata and "typefit_source" in field.metadata:
-                    source: Source = field.metadata["typefit_source"]
-                    yield {
-                        k: self.serialize(v)
-                        for k, v in source.value_to_json(field.name, obj).items()
-                    }
-                else:
-                    yield {field.name: self.serialize(getattr(obj, field.name))}
+                source: Source
+
+                match (field.metadata):
+                    case {"typefit_source": source}:
+                        yield {
+                            k: self.serialize(v)
+                            for k, v in source.value_to_json(field.name, obj).items()
+                        }
+                    case {"typefit_inject_root": True} | {"typefit_from_context": _}:
+                        pass
+                    case _:
+                        yield {field.name: self.serialize(getattr(obj, field.name))}
 
         return dict(ChainMap(*_get_values()))
 
     def serialize_mapping(self, obj: abc.Mapping):
         """
         Mappings are just copied into another mapping. While copying, all the
         values are recursively serialized.
```

### Comparing `typefit-0.5.3/src/typefit/utils.py` & `typefit-0.5.4/src/typefit/utils.py`

 * *Files identical despite different names*

### Comparing `typefit-0.5.3/PKG-INFO` & `typefit-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typefit
-Version: 0.5.3
+Version: 0.5.4
 Summary: Fits JSON values into Python type-anotated objects
 Home-page: https://github.com/Xowap/typefit/
 License: WTFPL
 Keywords: typing,json,api
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
```

