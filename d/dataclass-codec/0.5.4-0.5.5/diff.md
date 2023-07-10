# Comparing `tmp/dataclass_codec-0.5.4.tar.gz` & `tmp/dataclass_codec-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.5.4.tar", max compression
+gzip compressed data, was "dataclass_codec-0.5.5.tar", max compression
```

## Comparing `dataclass_codec-0.5.4.tar` & `dataclass_codec-0.5.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10143 2023-07-09 19:00:29.355476 dataclass_codec-0.5.4/README.md
--rw-r--r--   0        0        0      577 2023-07-09 20:22:10.354295 dataclass_codec-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.4/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0    15936 2023-07-09 20:21:35.834303 dataclass_codec-0.5.4/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.4/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.4/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    21758 2023-07-09 20:21:53.334299 dataclass_codec-0.5.4/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      845 2023-07-09 20:21:53.284299 dataclass_codec-0.5.4/src/dataclass_codec/tests/test_python3_9.py
--rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.4/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0    10596 1970-01-01 00:00:00.000000 dataclass_codec-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    10143 2023-07-09 19:00:29.355476 dataclass_codec-0.5.5/README.md
+-rw-r--r--   0        0        0      577 2023-07-10 00:54:46.010602 dataclass_codec-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.5.5/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    16549 2023-07-10 00:54:24.140607 dataclass_codec-0.5.5/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.5.5/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.5.5/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    22469 2023-07-10 00:54:23.560608 dataclass_codec-0.5.5/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      845 2023-07-09 20:21:53.284299 dataclass_codec-0.5.5/src/dataclass_codec/tests/test_python3_9.py
+-rw-r--r--   0        0        0      436 2023-07-09 03:52:02.877095 dataclass_codec-0.5.5/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0    10596 1970-01-01 00:00:00.000000 dataclass_codec-0.5.5/PKG-INFO
```

### Comparing `dataclass_codec-0.5.4/README.md` & `dataclass_codec-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.4/pyproject.toml` & `dataclass_codec-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.5.4"
+version = "0.5.5"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.5.4/src/dataclass_codec/decode.py` & `dataclass_codec-0.5.5/src/dataclass_codec/decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generator,
     Generic,
     List,
+    Literal,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     get_args,
@@ -488,14 +489,36 @@
     return _type is Any
 
 
 def any_type_decoder(obj: Any, _type: ANYTYPE, decode_it: DECODEIT) -> Any:
     return obj
 
 
+def is_literal_predicate(_type: ANYTYPE) -> bool:
+    return hasattr(_type, "__origin__") and _type.__origin__ is Literal
+
+
+def generic_literal_decoder(
+    obj: Any, _type: ANYTYPE, decode_it: DECODEIT
+) -> Any:
+    assert is_literal_predicate(_type), "{} is not a literal".format(
+        _type.__name__
+    )
+
+    obj_type = type(obj)
+    allowed_types = _type.__args__
+
+    if obj in allowed_types:
+        return decode_it(obj, obj_type)
+
+    raise ValueError(
+        f"Cannot decode {obj_type} as some of literal [{allowed_types}]"
+    )
+
+
 DEFAULT_DECODERS: Dict[ANYTYPE, TYPEDECODER] = {
     **{
         t: primitive_hook(t)
         for t in (
             int,
             float,
             str,
@@ -517,14 +540,15 @@
     (is_any_type_predicate, any_type_decoder),
     (is_dataclass_predicate, dataclass_from_primitive_dict),
     (is_generic_dataclass_predicate, generic_dataclass_from_primitive_dict),
     (is_generic_list_predicate, generic_list_decoder),
     (is_generic_dict_predicate, generic_dict_decoder),
     (is_union_predicate, generic_union_decoder),
     (is_generic_tuple_predicate, generic_tuple_decoder),
+    (is_literal_predicate, generic_literal_decoder),
     # This must be before is_enum_predicate
     (is_new_type_predicate, generic_new_type_decoder),
     (is_enum_predicate, enum_decoder),
     # This must be last
     (inherits_some_class_predicate, generic_inheritance_decoder),
 ]
```

### Comparing `dataclass_codec-0.5.4/src/dataclass_codec/encode.py` & `dataclass_codec-0.5.5/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.4/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.5.5/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 4% similar despite different names*

```diff
@@ -813,7 +813,35 @@
             dummy: Dict[str, Dummy[T]]
 
         assert decode({"dummy": {"a": 1}}, Dummy2) == Dummy2(dummy=Dummy(a=1))
 
         assert decode({"dummy": {"a": {"a": 1}}}, DummyMap[int]) == DummyMap(
             dummy={"a": Dummy(a=1)}
         )
+
+    def test_decode_literal(self) -> None:
+        from typing import Literal
+
+        @dataclass
+        class Dummy:
+            a: Literal["hello", "world"]
+
+        assert decode({"a": "hello"}, Dummy) == Dummy(a="hello")
+
+    def test_decode_literal_with_invalid_value(self) -> None:
+        from typing import Literal
+
+        @dataclass
+        class Dummy:
+            a: Literal["hello", "world"]
+
+        with pytest.raises(ValueError):
+            decode({"a": "hello2"}, Dummy)
+
+    def test_encode_literal(self) -> None:
+        from typing import Literal
+
+        @dataclass
+        class Dummy:
+            a: Literal["hello", "world"]
+
+        assert encode(Dummy(a="hello")) == {"a": "hello"}
```

### Comparing `dataclass_codec-0.5.4/src/dataclass_codec/tests/test_python3_9.py` & `dataclass_codec-0.5.5/src/dataclass_codec/tests/test_python3_9.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.5.4/PKG-INFO` & `dataclass_codec-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.5.4
+Version: 0.5.5
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

