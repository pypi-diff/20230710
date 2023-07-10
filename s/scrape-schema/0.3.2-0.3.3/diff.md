# Comparing `tmp/scrape_schema-0.3.2.tar.gz` & `tmp/scrape_schema-0.3.3.tar.gz`

## Comparing `scrape_schema-0.3.2.tar` & `scrape_schema-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/_logger.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/_typing.py
--rw-r--r--   0        0        0    16576 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/base.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/field.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/field_protocols.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/nested.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/scrape_schema/type_caster.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/LICENSE
--rw-r--r--   0        0        0    10278 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/README.md
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 scrape_schema-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/_protocols.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/_typing.py
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/base.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/field.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/nested.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/type_caster.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/special_methods/__init__.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/special_methods/base.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/special_methods/methods.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/LICENSE
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/README.md
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/PKG-INFO
```

### Comparing `scrape_schema-0.3.2/scrape_schema/_typing.py` & `scrape_schema-0.3.3/scrape_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.2/scrape_schema/base.py` & `scrape_schema-0.3.3/scrape_schema/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,151 +1,65 @@
 import re
 from abc import abstractmethod
-from enum import Enum
 from re import RegexFlag
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    NamedTuple,
-    Optional,
-    Pattern,
-    Tuple,
-    Type,
-    Union,
-)
+from typing import Any, Callable, Dict, List, Optional, Pattern, Tuple, Type, Union
 
-import chompjs
-from parsel import Selector
+from parsel import Selector, SelectorList
 
 from scrape_schema._logger import _logger
-from scrape_schema._typing import (
-    Annotated,
-    NoneType,
-    Self,
-    get_args,
-    get_origin,
-    get_type_hints,
+from scrape_schema._protocols import SpecialMethodsProtocol
+from scrape_schema._typing import Annotated, Self, get_args, get_origin, get_type_hints
+from scrape_schema.special_methods import (
+    DEFAULT_SPEC_METHOD_HANDLER,
+    MarkupMethod,
+    SpecialMethods,
+    SpecialMethodsHandler,
 )
-from scrape_schema.field_protocols import SpecialMethodsProtocol
 from scrape_schema.type_caster import TypeCaster
 
 
-class SpecialMethods(Enum):
-    # special methods for another methods
-    FN = 0
-    CONCAT_L = 1
-    CONCAT_R = 2
-    REPLACE = 3
-    REGEX_SEARCH = 4
-    REGEX_FINDALL = 5
-    CHOMP_JS_PARSE = 6
-    CHOMP_JS_PARSE_ALL = 7
-
-
-class MarkupMethod(NamedTuple):
-    METHOD_NAME: Union[str, SpecialMethods]
-    args: Tuple[Any, ...] = ()
-    kwargs: Dict[str, Any] = {}
-
-    def __repr__(self):
-        return f"{self.METHOD_NAME} args={self.args}, kwargs={self.kwargs}"
-
-
-class FieldConfig:
-    instance: Type[Any] = NoneType
-    defaults: Dict[str, Any] = {}
-
-
 class sc_param(property):
     """Shortcut for adding property-like descriptors in BaseSchema"""
 
     pass
 
 
 class BaseField:
-    class Config(FieldConfig):
-        pass
-
     def __init__(self, auto_type: bool = True, default: Any = ..., **kwargs):
         self._stack_methods: List[MarkupMethod] = []
         self.default = default
         self.auto_type = auto_type
         self.is_default = False  # flag check failed parsed value
+        self._spec_method_handler: SpecialMethodsHandler = DEFAULT_SPEC_METHOD_HANDLER
 
     @abstractmethod
     def _prepare_markup(self, markup):
         pass
 
     @abstractmethod
     def sc_parse(self, markup: Any):
         pass
 
 
 class Field(BaseField):
-    class Config(FieldConfig):
-        pass
-
-    def _prepare_markup(self, markup: Any):
+    def _prepare_markup(self, markup: Union[str, bytes, Selector, SelectorList]):
         """convert string/bytes to parser class context"""
-        if isinstance(self.Config.instance, NoneType):
+        if isinstance(markup, (Selector, SelectorList)):
             return markup
-        elif isinstance(markup, (str, bytes)):
+        elif isinstance(markup, str):
             _logger.debug(
-                "Convert raw markup to %s with kwargs %s",
-                self.Config.instance.__name__,
-                self.Config.defaults,
+                "Convert raw markup to parsel.Selector",
             )
-            return self.Config.instance(markup, **self.Config.defaults)
-        return markup
-
-    @staticmethod
-    def _special_method(markup: Any, method: MarkupMethod):
-        if method.METHOD_NAME == SpecialMethods.FN:
-            return method.kwargs["function"](markup)
-        elif method.METHOD_NAME == SpecialMethods.CONCAT_R:
-            if isinstance(markup, list):
-                return [m + method.args[0] for m in markup]
-            return markup + method.args[0]
-        elif method.METHOD_NAME == SpecialMethods.CONCAT_L:
-            if isinstance(markup, list):
-                return [method.args[0] + m for m in markup]
-            return method.args[0] + markup
-        elif method.METHOD_NAME == SpecialMethods.REPLACE:
-            __old, __new, __count = method.args[0], method.args[1], method.args[2]
-            if isinstance(markup, list):
-                return [m.replace(__old, __new, __count) for m in markup]
-            return markup.replace(__old, __new, __count)
-        elif method.METHOD_NAME == SpecialMethods.REGEX_SEARCH:
-            pattern, groupdict = method.args
-            if groupdict:
-                if not pattern.groupindex:
-                    raise TypeError(
-                        f"Pattern `{pattern.pattern}` is not contains groups"
-                    )
-                return pattern.search(markup).groupdict()
-            return pattern.search(markup)
-        elif method.METHOD_NAME == SpecialMethods.REGEX_FINDALL:
-            pattern, groupdict = method.args
-            if groupdict:
-                if not pattern.groupindex:
-                    raise TypeError(
-                        f"Pattern `{pattern.pattern}` is not contains groups"
-                    )
-                return [match.groupdict() for match in pattern.finditer(markup)]
-            return pattern.findall(markup)
-
-        elif method.METHOD_NAME == SpecialMethods.CHOMP_JS_PARSE:
-            return chompjs.parse_js_object(markup, *method.args)
+            return Selector(markup)
+        elif isinstance(markup, bytes):
+            return Selector(body=markup)
+        raise TypeError("Uncorrected markup type")
 
-        elif method.METHOD_NAME == SpecialMethods.CHOMP_JS_PARSE_ALL:
-            return chompjs.parse_js_objects(markup, *method.args)
-
-        raise TypeError("Unknown special method")
+    def _special_method(self, markup: Any, method: MarkupMethod) -> Any:
+        return self._spec_method_handler.handle(method, markup)
 
     @staticmethod
     def _accept_method(markup: Any, method: MarkupMethod) -> Any:
         if isinstance(method.METHOD_NAME, str):
             class_method = getattr(markup, method.METHOD_NAME)
             if isinstance(class_method, (property, dict)):  # attrib check
                 return class_method
@@ -244,15 +158,15 @@
             string – Input string
             unicode_escape – Attempt to fix input string if it contains escaped special characters
             json_params – Allow passing down standard json.loads options
 
         Returns:
             Extracted JSON object
         """
-        return self.add_method(
+        return self.add_method(  # type: ignore
             SpecialMethods.CHOMP_JS_PARSE, unicode_escape, json_params
         )
 
     def chomp_js_parse_all(
         self,
         unicode_escape: Any = False,
         omitempty: Any = False,
@@ -265,15 +179,15 @@
             unicode_escape – Attempt to fix input string if it contains escaped special characters
             omitempty – Skip empty dictionaries and lists
             json_params – Allow passing down standard json.loads flags
 
         Returns:
             Iterating over it yields all encountered JSON objects
         """
-        return self.add_method(
+        return self.add_method(  # type: ignore
             SpecialMethods.CHOMP_JS_PARSE_ALL, unicode_escape, omitempty, json_params
         )
 
     def add_method(
         self, method_name: Union[str, SpecialMethods], *args, **kwargs
     ) -> Self:
         """low-level interface adding methods to call stack"""
@@ -281,130 +195,101 @@
         return self
 
     def __getitem__(self, item) -> Self:
         return self.add_method("__getitem__", item)
 
 
 class SchemaMeta(type):
-    __meta_info__: Dict[str, Any]  # TODO standardise this
     __schema_fields__: Dict[str, BaseField]
     __schema_annotations__: Dict[str, Type]
-    __parsers__: Dict[str, Type]
 
     @staticmethod
-    def _is_type_field(attr: Type) -> bool:
+    def __is_type_field(attr: Type) -> bool:
         return get_origin(attr) is Annotated and all(
             isinstance(arg, BaseField) for arg in get_args(attr)[1:]
         )
 
     @staticmethod
-    def _extract_annotated(attr: Type) -> Tuple[Type, BaseField]:
+    def __parse_annotated_field(attr: Type) -> Tuple[Type, BaseField]:
         args = get_args(attr)
         return args[0], tuple(arg for arg in args[1:] if isinstance(arg, BaseField))[0]
 
     def __new__(mcs, name, bases, attrs):
         # cache fields, annotations and used parsers for more simplify access
         __schema_fields__: Dict[str, BaseField] = {}  # type: ignore
         __schema_annotations__: Dict[str, Type] = {}  # type: ignore
-        __parsers__: Dict[str, Type] = {}  # type: ignore
 
         cls_schema = super().__new__(mcs, name, bases, attrs)
         if cls_schema.__name__ == "BaseSchema":
             return cls_schema
 
         # localns={} kwarg avoid TypeError 'function' object is not subscriptable
         for name, value in get_type_hints(
             cls_schema, localns={}, include_extras=True
         ).items():
             if name in ("__schema_fields__", "__schema_annotations__", "__parsers__"):
                 continue
-            if mcs._is_type_field(value):
-                field_type, field = mcs._extract_annotated(value)
-
-                if (
-                    field.Config.instance
-                    and field.Config.instance.__name__ not in __parsers__
-                ):
-                    __parsers__[field.Config.instance.__name__] = field.Config.instance
-
+            if mcs.__is_type_field(value):
+                field_type, field = mcs.__parse_annotated_field(value)
                 __schema_fields__[name] = field
                 __schema_annotations__[name] = field_type
+
         setattr(cls_schema, "__schema_fields__", __schema_fields__)
         setattr(cls_schema, "__schema_annotations__", __schema_annotations__)
-        setattr(cls_schema, "__parsers__", __parsers__)
         setattr(cls_schema, "__meta_info__", {})
-
         return cls_schema
 
 
 class BaseSchema(metaclass=SchemaMeta):
     class Config:
-        parsers: Dict[Type[Any], Dict[str, Any]] = {Selector: {}}
+        selector_kwargs: Dict[str, Any] = {}
         type_caster: Optional[TypeCaster] = TypeCaster()  # TODO make interface
 
-    def __init__(self, markup: Any):
-        self.cached_parsers: Dict[str, Any] = {}
-        if isinstance(markup, (str, bytes)):
-            self.__raw__ = markup
-            for cls_parser in self.__parsers__.values():  # type: ignore
-                if (
-                    self.Config.parsers.get(cls_parser, None) is None
-                    and cls_parser != NoneType
-                ):
-                    _logger.error("Config.parser required %s", cls_parser.__name__)
-                    raise AttributeError(
-                        f"Config.parser required {cls_parser.__name__}"
-                    )
-
-            # cache parsers
-            self.cached_parsers.update(
-                {  # type: ignore
-                    cls_parser.__name__: cls_parser(markup, **kw)
-                    for cls_parser, kw in self.Config.parsers.items()
-                    if not isinstance(cls_parser, NoneType)
-                }
-            )
+    @property
+    def __parser__(self) -> Union[Selector, SelectorList]:
+        return self._cached_parser
+
+    @property
+    def __raw__(self) -> str:
+        return self._markup
 
+    def __init__(self, markup: Any):
+        self._cached_parser: Union[Selector, SelectorList]
+        if isinstance(markup, str):
+            self._markup = markup
+            self._cached_parser = Selector(markup, **self.Config.selector_kwargs)
+        elif isinstance(markup, bytes):
+            self._cached_parser = Selector(body=markup, **self.Config.selector_kwargs)
+            self._markup = markup.decode()
         # TODO write adapter for another backends
-        elif isinstance(markup, Selector):
-            self.__raw__ = markup.get()
-            self.cached_parsers["Selector"] = markup
+        elif isinstance(markup, (Selector, SelectorList)):
+            self._markup = markup.get()  # type: ignore
+            self._cached_parser = markup
 
         else:
             raise TypeError(
                 f"markup support only str,bytes or Selector types, not {type(markup).__name__}"
             )
-
         # initialize and parse fields
         self.__init_fields__()
 
-    def clear_cache(self):
-        self.cached_parsers.clear()
-
     def __init_fields__(self):
         _logger.info(
             "[%s] Start parse fields count: %s",
             self.__schema_name__,
             len(self.__schema_fields__.keys()),
         )
         for name, field in self.__schema_fields__.items():
             field_type = self.__schema_annotations__[name]
             _logger.debug("%s.%s start parse", self.__schema_name__, name)
             if field.__class__.__name__ == "Nested":  # todo fix
                 field.type_ = field_type
 
             # todo refactoring
-            if (
-                field.Config.instance == NoneType
-                and field.__class__.__name__ == "Nested"
-            ):
-                value = field.sc_parse(self.cached_parsers["Selector"])
-            else:
-                cache_key = field.Config.instance.__name__
-                value = field.sc_parse(self.cached_parsers[cache_key])  # self.__raw__
+            value = field.sc_parse(self.__parser__)
 
             if self.Config.type_caster and field.auto_type and not field.is_default:
                 value = self.Config.type_caster.cast(field_type, value)
             # disable default value flag
             if field.is_default:
                 field.is_default = False
 
@@ -419,15 +304,15 @@
         elif isinstance(value, list):
             if all(isinstance(val, BaseSchema) for val in value):
                 return [val.dict() for val in value]
         return value
 
     def dict(self):
         result: Dict[str, Any] = {  # type: ignore
-            k: getattr(self, k)
+            k: self._to_dict(getattr(self, k))
             for k, v in self.__class__.__dict__.items()
             if isinstance(v, sc_param)
         }
         # parse public field keys
         for k, v in self.__dict__.items():
             if not k.startswith("_") and self.__schema_fields__.get(k):
                 result[k] = self._to_dict(v)
@@ -451,9 +336,9 @@
             f"{k}={repr(v)}"
             if isinstance(v, BaseSchema)
             else f"{k}:{type(v).__name__}={repr(v)}"
             for k, v in args.items()
         ]
 
     @property
-    def __schema_name__(self):
+    def __schema_name__(self) -> str:
         return self.__class__.__name__
```

### Comparing `scrape_schema-0.3.2/scrape_schema/field.py` & `scrape_schema-0.3.3/scrape_schema/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import Any, Hashable, Mapping, Optional, Pattern, Union
 
 from parsel import Selector
 
 from scrape_schema._logger import _logger
+from scrape_schema._protocols import AttribProtocol, SpecialMethodsProtocol
 from scrape_schema._typing import Self
-from scrape_schema.base import Field, FieldConfig
-from scrape_schema.field_protocols import AttribProtocol, SpecialMethodsProtocol
+from scrape_schema.base import Field
 
 
 class Parsel(Field):
-    class Config(FieldConfig):
-        instance = Selector
-
     def __init__(
         self, auto_type: bool = True, default: Any = ..., *, raw: bool = False
     ):
         super().__init__(auto_type=auto_type, default=default)
         if raw:
             self.xpath("//p/text()").get()
```

### Comparing `scrape_schema-0.3.2/scrape_schema/field_protocols.py` & `scrape_schema-0.3.3/scrape_schema/_protocols.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.2/scrape_schema/nested.py` & `scrape_schema-0.3.3/scrape_schema/nested.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Optional, Type, get_args
 
+from parsel import Selector, SelectorList
+
 from scrape_schema._typing import get_origin
-from scrape_schema.base import BaseField, BaseSchema, FieldConfig
+from scrape_schema.base import BaseField, BaseSchema
 
 
 class Nested(BaseField):
     def __init__(
         self,
         field: BaseField,
         *,
         type_: Optional[Type] = None,
-        markup_parser: Type = type(None),
     ):
         super().__init__()
         self.auto_type = False
         self.type_ = type_
         self._crop_field = field
-        self.Config.instance = markup_parser
 
     def _prepare_markup(self, markup):
         raise NotImplementedError(
             "_prepare_markup not allowed in Nested"
         )  # pragma: no cover
 
     def sc_parse(self, markup) -> Any:
@@ -32,21 +32,22 @@
         ):
             pass
         elif not issubclass(self.type_, BaseSchema):
             raise AttributeError(
                 f"type should be List[BaseSchema] or BaseSchema, not {self.type_}"
             )
 
-        # self.Config = self._crop_field.Config
-        # markup = self._prepare_markup(markup)
-
         if len(get_args(self.type_)) != 0 and issubclass(
             get_args(self.type_)[0], BaseSchema
         ):
             cls_schema = get_args(self.type_)[0]
         else:
             cls_schema = self.type_
 
         chunks = self._crop_field.sc_parse(markup)
-        if get_origin(self.type_) is list:
+        if isinstance(chunks, SelectorList) and get_origin(self.type_) is list:
+            return [cls_schema(chunk.get()) for chunk in chunks]
+        elif get_origin(self.type_) is list:
             return [cls_schema(chunk) for chunk in chunks]
+        elif isinstance(chunks, Selector) and get_origin(self.type_) is not list:
+            return cls_schema(chunks.get())
         return cls_schema(chunks)
```

### Comparing `scrape_schema-0.3.2/scrape_schema/type_caster.py` & `scrape_schema-0.3.3/scrape_schema/type_caster.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.2/.gitignore` & `scrape_schema-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.2/LICENSE` & `scrape_schema-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.2/README.md` & `scrape_schema-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 ![Python-versions](https://img.shields.io/pypi/pyversions/scrape_schema)
 [![codecov](https://codecov.io/gh/vypivshiy/scrape-schema/branch/master/graph/badge.svg?token=jqSNuE7g5l)](https://codecov.io/gh/vypivshiy/scrape-schema)
 
 # Scrape-schema
 This library is designed to write structured, readable, 
 reusable parsers for html, raw text and is inspired by dataclasses
 
+> !!! Scrape-schema is currently in Pre-Alpha. Please expect breaking changes.
+
 # Motivation
 Simplifying parsers support, where it is difficult to use 
 or the complete absence of the **API interfaces** and decrease lines of code
 
 Also structuring, data serialization and use as an intermediate layer 
 for third-party serialization libraries: json, dataclasses, pydantic, etc
 
 _____
 # Features
 - [Parsel](https://github.com/scrapy/parsel) backend.
+- re, css, xpath, jmespath, chompjs features
 - [Fluent interface](https://en.wikipedia.org/wiki/Fluent_interface#Python) simulate original parsel.Selector API for easy to use. 
+- does not depend on the http client implementation, use any!
 - Python 3.8+ support
 - Dataclass-like structure
 - Partial support auto type-casting from annotations (str, int, float, bool, list, dict, Optional)
 - logging to quickly find problems in extracted values
 ____
 
 # Install
@@ -259,31 +263,37 @@
     digits_float: Sc[List[float], Parsel(raw=True).re_findall(r"(\d+)").fn(lambda lst: [f"{s}.5" for s in lst])]
     words_lower: Sc[List[str], Parsel(raw=True).re_findall("([a-z]+)")]
     words_upper: Sc[List[str], Parsel(raw=True).re_findall(r"([A-Z]+)")]
 
     @sc_param
     def sum(self):
         return sum(self.digits)
+    
+    @sc_param
+    def max_digit(self):
+        return max(self.digits)
 
     @sc_param
     def all_words(self):
         return self.words_lower + self.words_upper
 
 
 if __name__ == '__main__':
     pprint.pprint(MySchema(TEXT).dict(), compact=True)
 # {'all_words': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor',
 #                'BANANA', 'POTATO'],
 #  'digits': [10, 20, 192, 168, 0, 1],
 #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5, 1.5],
 #  'failed_value': False,
 #  'ipv4': '192.168.0.1',
+#  'max_digit': 192,
 #  'sum': 391,
 #  'words_lower': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor'],
 #  'words_upper': ['BANANA', 'POTATO']}
+
 ```
 
 _____
 # logging
 In this project, logging to the `DEBUG` level is enabled by default. 
 
 To set up logger, you can get it by the name `"scrape_schema"`
```

### Comparing `scrape_schema-0.3.2/pyproject.toml` & `scrape_schema-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.2/PKG-INFO` & `scrape_schema-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.3.2
+Version: 0.3.3
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -54,25 +54,29 @@
 ![Python-versions](https://img.shields.io/pypi/pyversions/scrape_schema)
 [![codecov](https://codecov.io/gh/vypivshiy/scrape-schema/branch/master/graph/badge.svg?token=jqSNuE7g5l)](https://codecov.io/gh/vypivshiy/scrape-schema)
 
 # Scrape-schema
 This library is designed to write structured, readable, 
 reusable parsers for html, raw text and is inspired by dataclasses
 
+> !!! Scrape-schema is currently in Pre-Alpha. Please expect breaking changes.
+
 # Motivation
 Simplifying parsers support, where it is difficult to use 
 or the complete absence of the **API interfaces** and decrease lines of code
 
 Also structuring, data serialization and use as an intermediate layer 
 for third-party serialization libraries: json, dataclasses, pydantic, etc
 
 _____
 # Features
 - [Parsel](https://github.com/scrapy/parsel) backend.
+- re, css, xpath, jmespath, chompjs features
 - [Fluent interface](https://en.wikipedia.org/wiki/Fluent_interface#Python) simulate original parsel.Selector API for easy to use. 
+- does not depend on the http client implementation, use any!
 - Python 3.8+ support
 - Dataclass-like structure
 - Partial support auto type-casting from annotations (str, int, float, bool, list, dict, Optional)
 - logging to quickly find problems in extracted values
 ____
 
 # Install
@@ -307,31 +311,37 @@
     digits_float: Sc[List[float], Parsel(raw=True).re_findall(r"(\d+)").fn(lambda lst: [f"{s}.5" for s in lst])]
     words_lower: Sc[List[str], Parsel(raw=True).re_findall("([a-z]+)")]
     words_upper: Sc[List[str], Parsel(raw=True).re_findall(r"([A-Z]+)")]
 
     @sc_param
     def sum(self):
         return sum(self.digits)
+    
+    @sc_param
+    def max_digit(self):
+        return max(self.digits)
 
     @sc_param
     def all_words(self):
         return self.words_lower + self.words_upper
 
 
 if __name__ == '__main__':
     pprint.pprint(MySchema(TEXT).dict(), compact=True)
 # {'all_words': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor',
 #                'BANANA', 'POTATO'],
 #  'digits': [10, 20, 192, 168, 0, 1],
 #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5, 1.5],
 #  'failed_value': False,
 #  'ipv4': '192.168.0.1',
+#  'max_digit': 192,
 #  'sum': 391,
 #  'words_lower': ['banana', 'potato', 'foo', 'bar', 'lorem', 'upsum', 'dolor'],
 #  'words_upper': ['BANANA', 'POTATO']}
+
 ```
 
 _____
 # logging
 In this project, logging to the `DEBUG` level is enabled by default. 
 
 To set up logger, you can get it by the name `"scrape_schema"`
```

