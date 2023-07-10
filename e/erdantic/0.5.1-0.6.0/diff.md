# Comparing `tmp/erdantic-0.5.1.tar.gz` & `tmp/erdantic-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdantic-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "erdantic-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `erdantic-0.5.1.tar` & `erdantic-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2023-07-04 22:27:55.082980 erdantic-0.5.1/LICENSE
--rw-r--r--   0        0        0     3616 2023-07-04 22:27:55.082980 erdantic-0.5.1/README.md
--rw-r--r--   0        0        0      296 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/__init__.py
--rw-r--r--   0        0        0       66 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/__main__.py
--rw-r--r--   0        0        0     7543 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/base.py
--rw-r--r--   0        0        0     4623 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/cli.py
--rw-r--r--   0        0        0     2436 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/dataclasses.py
--rw-r--r--   0        0        0    13858 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/erd.py
--rw-r--r--   0        0        0      166 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/examples/__init__.py
--rw-r--r--   0        0        0     2246 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/examples/dataclasses.py
--rw-r--r--   0        0        0     2199 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/examples/pydantic.py
--rw-r--r--   0        0        0     3710 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/exceptions.py
--rw-r--r--   0        0        0     3994 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/pydantic.py
--rw-r--r--   0        0        0     3919 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/typing.py
--rw-r--r--   0        0        0      205 2023-07-04 22:27:55.086980 erdantic-0.5.1/erdantic/version.py
--rw-r--r--   0        0        0     1758 2023-07-04 22:27:55.086980 erdantic-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 erdantic-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-10 02:05:06.871816 erdantic-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3616 2023-07-10 02:05:06.871816 erdantic-0.6.0/README.md
+-rw-r--r--   0        0        0      296 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/__main__.py
+-rw-r--r--   0        0        0     7543 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/base.py
+-rw-r--r--   0        0        0     4623 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/cli.py
+-rw-r--r--   0        0        0     2127 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/dataclasses.py
+-rw-r--r--   0        0        0    13858 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/erd.py
+-rw-r--r--   0        0        0      166 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/examples/__init__.py
+-rw-r--r--   0        0        0     2246 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/examples/dataclasses.py
+-rw-r--r--   0        0        0     2199 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/examples/pydantic.py
+-rw-r--r--   0        0        0     3710 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/exceptions.py
+-rw-r--r--   0        0        0     4023 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/pydantic.py
+-rw-r--r--   0        0        0     4816 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/typing.py
+-rw-r--r--   0        0        0      205 2023-07-10 02:05:06.875816 erdantic-0.6.0/erdantic/version.py
+-rw-r--r--   0        0        0     1778 2023-07-10 02:05:06.875816 erdantic-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4932 1970-01-01 00:00:00.000000 erdantic-0.6.0/PKG-INFO
```

### Comparing `erdantic-0.5.1/LICENSE` & `erdantic-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/README.md` & `erdantic-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/erdantic/base.py` & `erdantic-0.6.0/erdantic/base.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/erdantic/cli.py` & `erdantic-0.6.0/erdantic/cli.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/erdantic/dataclasses.py` & `erdantic-0.6.0/erdantic/dataclasses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import collections.abc
 import dataclasses
 from typing import Any, List, Union
 
 
 from erdantic.base import Field, Model, register_model_adapter
 from erdantic.exceptions import InvalidFieldError, InvalidModelError
-from erdantic.typing import GenericAlias, get_args, get_origin
+from erdantic.typing import GenericAlias, is_many, is_nullable
 
 
 class DataClassField(Field[dataclasses.Field]):
     """Concrete field adapter class for dataclass fields.
 
     Attributes:
         field (dataclasses.Field): The dataclass field instance that is associated with this
@@ -26,23 +25,18 @@
         return self.field.name
 
     @property
     def type_obj(self) -> Union[type, GenericAlias]:
         return self.field.type
 
     def is_many(self) -> bool:
-        origin = get_origin(self.type_obj)
-        return isinstance(origin, type) and (
-            issubclass(origin, collections.abc.Container)
-            or issubclass(origin, collections.abc.Iterable)
-            or issubclass(origin, collections.abc.Sized)
-        )
+        return is_many(self.type_obj)
 
     def is_nullable(self) -> bool:
-        return get_origin(self.type_obj) is Union and type(None) in get_args(self.type_obj)
+        return is_nullable(self.type_obj)
 
 
 @register_model_adapter("dataclasses")
 class DataClassModel(Model[type]):
     """Concrete model adapter class for a
     [`dataclasses` module](https://docs.python.org/3/library/dataclasses.html) dataclass.
```

### Comparing `erdantic-0.5.1/erdantic/erd.py` & `erdantic-0.6.0/erdantic/erd.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/erdantic/examples/dataclasses.py` & `erdantic-0.6.0/erdantic/examples/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/erdantic/examples/pydantic.py` & `erdantic-0.6.0/erdantic/examples/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/erdantic/exceptions.py` & `erdantic-0.6.0/erdantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `erdantic-0.5.1/erdantic/pydantic.py` & `erdantic-0.6.0/erdantic/pydantic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-from typing import Any, List, Optional, Union, Type
+from typing import Any, List, Union, Type
 
 import pydantic
 import pydantic.fields
+import pydantic_core
 
 from erdantic.base import Field, Model, register_model_adapter
 from erdantic.exceptions import InvalidFieldError, InvalidModelError
-from erdantic.typing import GenericAlias, repr_type_with_mro
+from erdantic.typing import GenericAlias, repr_type_with_mro, is_many, is_nullable
 
 
-class PydanticField(Field[pydantic.fields.ModelField]):
+class PydanticField(Field[pydantic.fields.FieldInfo]):
     """Concrete field adapter class for Pydantic fields.
 
     Attributes:
         field (pydantic.fields.ModelField): The Pydantic field object that is associated with this
             adapter instance.
     """
 
-    def __init__(self, field: pydantic.fields.ModelField):
-        if not isinstance(field, pydantic.fields.ModelField):
+    def __init__(self, name: str, field_info: pydantic.fields.FieldInfo):
+        self._name = name
+        if not isinstance(field_info, pydantic.fields.FieldInfo):
             raise InvalidFieldError(
-                f"field must be of type pydantic.fields.ModelField. Got: {type(field)}"
+                f"field_info must be of type pydantic.fields.FieldInfo. Got: {type(field_info)}"
             )
-        super().__init__(field=field)
+        super().__init__(field=field_info)
 
     @property
     def name(self) -> str:
-        return self.field.name
+        return self._name
 
     @property
     def type_obj(self) -> Union[type, GenericAlias]:
-        tp = self.field.outer_type_
-        if self.field.allow_none:
-            return Optional[tp]
-        return tp
+        return self.field.annotation
 
     def is_many(self) -> bool:
-        return self.field.shape > 1
+        return is_many(self.type_obj)
 
     def is_nullable(self) -> bool:
-        return self.field.allow_none
+        return is_nullable(self.type_obj)
 
 
 @register_model_adapter("pydantic")
 class PydanticModel(Model[Type[pydantic.BaseModel]]):
     """Concrete model adapter class for a Pydantic
     [`BaseModel`](https://pydantic-docs.helpmanual.io/usage/models/).
 
@@ -68,32 +67,33 @@
 
     @staticmethod
     def is_model_type(obj: Any) -> bool:
         return isinstance(obj, type) and issubclass(obj, pydantic.BaseModel)
 
     @property
     def fields(self) -> List[Field]:
-        return [PydanticField(field=f) for f in self.model.__fields__.values()]
+        return [
+            PydanticField(name=name, field_info=field_info)
+            for name, field_info in self.model.model_fields.items()
+        ]
 
     @property
     def docstring(self) -> str:
         out = super().docstring
-        field_descriptions = [
-            getattr(field.field.field_info, "description", None) for field in self.fields
-        ]
+        field_descriptions = [field.field.description for field in self.fields]
         if any(descr is not None for descr in field_descriptions):
             # Sometimes Pydantic models have field documentation as descriptions as metadata on the
             # field instead of in the docstring. If detected, construct docstring and add.
             out += "\nAttributes:\n"
-            field_defaults = [field.field.field_info.default for field in self.fields]
+            field_defaults = [field.field.default for field in self.fields]
             for field, descr, default in zip(self.fields, field_descriptions, field_defaults):
                 if descr is not None:
                     line = f"{field.name} ({field.type_name}): {descr}"
                     if (
-                        not isinstance(default, pydantic.fields.UndefinedType)
+                        not isinstance(default, pydantic_core.PydanticUndefinedType)
                         and default is not ...
                     ):
                         if not line.strip().endswith("."):
                             line = line.rstrip() + ". "
                         else:
                             line = line.rstrip() + " "
                         if isinstance(default, str):
```

### Comparing `erdantic-0.5.1/pyproject.toml` & `erdantic-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "erdantic"
-version = "0.5.1"
+version = "0.6.0"
 description = "Entity relationship diagrams for Python data model classes like Pydantic."
 readme = "README.md"
 authors = [{ name = "DrivenData", email = "info@drivendata.org" }]
 license = { file = "LICENSE" }
 keywords = ["erd", "entity relationship diagram", "dataclasses", "pydantic"]
 classifiers = [
   "Intended Audience :: Developers",
@@ -21,15 +21,16 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.7"
 dependencies = [
   "importlib_metadata ; python_version < '3.8'",
-  "pydantic < 2",
+  "pydantic >= 2",
+  "pydantic-core",
   "pygraphviz",
   "typer",
   "typing_extensions > 4 ; python_version < '3.8'",
 ]
 
 [project.scripts]
 erdantic = "erdantic.cli:app"
```

### Comparing `erdantic-0.5.1/PKG-INFO` & `erdantic-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdantic
-Version: 0.5.1
+Version: 0.6.0
 Summary: Entity relationship diagrams for Python data model classes like Pydantic.
 Keywords: erd,entity relationship diagram,dataclasses,pydantic
 Author-email: DrivenData <info@drivendata.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: importlib_metadata ; python_version < '3.8'
-Requires-Dist: pydantic < 2
+Requires-Dist: pydantic >= 2
+Requires-Dist: pydantic-core
 Requires-Dist: pygraphviz
 Requires-Dist: typer
 Requires-Dist: typing_extensions > 4 ; python_version < '3.8'
 Project-URL: Bug Tracker, https://github.com/drivendataorg/erdantic/issues
 Project-URL: Changelog, https://erdantic.drivendata.org/stable/changelog/
 Project-URL: Documentation, https://erdantic.drivendata.org/
 Project-URL: Repository, https://github.com/drivendataorg/erdantic
```

