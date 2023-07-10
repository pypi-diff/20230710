# Comparing `tmp/valcheck-0.3.6.tar.gz` & `tmp/valcheck-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valcheck-0.3.6.tar", last modified: Tue Jul  4 15:47:11 2023, max compression
+gzip compressed data, was "valcheck-0.3.7.tar", last modified: Mon Jul 10 06:28:48 2023, max compression
```

## Comparing `valcheck-0.3.6.tar` & `valcheck-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 15:47:11.107472 valcheck-0.3.6/
--rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      751 2023-07-04 15:47:11.105483 valcheck-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-02 09:39:38.000000 valcheck-0.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 15:47:11.107472 valcheck-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1559 2023-07-02 14:40:18.000000 valcheck-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 15:47:11.074530 valcheck-0.3.6/valcheck/
--rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.3.6/valcheck/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.3.6/valcheck/exceptions.py
--rw-rw-rw-   0        0        0    17995 2023-07-04 15:25:07.000000 valcheck-0.3.6/valcheck/fields.py
--rw-rw-rw-   0        0        0     2202 2023-07-04 15:28:12.000000 valcheck-0.3.6/valcheck/models.py
--rw-rw-rw-   0        0        0     2490 2023-07-03 16:41:25.000000 valcheck-0.3.6/valcheck/utils.py
--rw-rw-rw-   0        0        0     6365 2023-07-04 15:41:10.000000 valcheck-0.3.6/valcheck/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-04 15:47:11.101527 valcheck-0.3.6/valcheck.egg-info/
--rw-rw-rw-   0        0        0      751 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 15:47:11.000000 valcheck-0.3.6/valcheck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 06:28:48.084199 valcheck-0.3.7/
+-rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0      751 2023-07-10 06:28:48.084199 valcheck-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1683 2023-07-10 06:17:03.000000 valcheck-0.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 06:28:48.085196 valcheck-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1559 2023-07-06 22:31:22.000000 valcheck-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:28:48.061266 valcheck-0.3.7/valcheck/
+-rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.3.7/valcheck/__init__.py
+-rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.3.7/valcheck/exceptions.py
+-rw-rw-rw-   0        0        0    18170 2023-07-10 05:47:12.000000 valcheck-0.3.7/valcheck/fields.py
+-rw-rw-rw-   0        0        0     2574 2023-07-09 20:28:55.000000 valcheck-0.3.7/valcheck/models.py
+-rw-rw-rw-   0        0        0     2490 2023-07-09 19:22:10.000000 valcheck-0.3.7/valcheck/utils.py
+-rw-rw-rw-   0        0        0     5322 2023-07-10 06:27:01.000000 valcheck-0.3.7/valcheck/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-10 06:28:48.082204 valcheck-0.3.7/valcheck.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-07-10 06:28:47.000000 valcheck-0.3.7/valcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-10 06:28:47.000000 valcheck-0.3.7/valcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 06:28:47.000000 valcheck-0.3.7/valcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 06:28:47.000000 valcheck-0.3.7/valcheck.egg-info/top_level.txt
```

### Comparing `valcheck-0.3.6/LICENSE` & `valcheck-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `valcheck-0.3.6/PKG-INFO` & `valcheck-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.3.6
+Version: 0.3.7
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `valcheck-0.3.6/setup.py` & `valcheck-0.3.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import find_packages, setup
 
 # Constants
 PACKAGE_NAME = "valcheck"
-PACKAGE_VERSION = "0.3.6"
+PACKAGE_VERSION = "0.3.7"
 AUTHOR_NAME = "Nishant Rao"
 AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
 FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
 REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
 
 # Requirements
```

### Comparing `valcheck-0.3.6/valcheck/exceptions.py` & `valcheck-0.3.7/valcheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.3.6/valcheck/fields.py` & `valcheck-0.3.7/valcheck/fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,122 +15,104 @@
     is_valid_json_string,
     is_valid_object_of_type,
     is_valid_uuid_string,
     set_as_empty,
 )
 
 
-def _invalid_field_error(field: Field, /, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
-    return (
-        f"{prefix if prefix else ''}"
-        f"Invalid {field.__class__.__name__} '{field.field_name}'"
-        f"{suffix if suffix else ''}"
-    )
-
-
-def _missing_field_error(field: Field, /, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
-    return (
-        f"{prefix if prefix else ''}"
-        f"Missing {field.__class__.__name__} '{field.field_name}'"
-        f"{suffix if suffix else ''}"
-    )
-
-
-class FieldInfo:
+class ValidatedField:
     """Class that represents a validated field"""
 
     def __init__(
             self,
             *,
             field_name: str,
-            field_value: Any,
+            field_value: Union[Any, Empty],
             errors: List[Error],
-            converted_value: Union[Any, Empty],
         ) -> None:
         assert isinstance(field_name, str), "Param `field_name` must be of type 'str'"
         assert is_list_of_instances_of_type(errors, type_=Error, allow_empty=True), (
             "Param `errors` must be a list where each item is of type `valcheck.models.Error`"
         )
 
         self.field_name = field_name
-        self.field_value = field_value
+        self._field_value = field_value
         self._errors = errors
-        self._converted_value = converted_value
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}(field_name='{self.field_name}')"
 
     @property
+    def field_value(self) -> Union[Any, Empty]:
+        return self._field_value
+
+    @field_value.setter
+    def field_value(self, value: Union[Any, Empty]) -> None:
+        self._field_value = value
+
+    @property
     def errors(self) -> List[Error]:
         return self._errors
 
     @errors.setter
-    def errors(self, value) -> None:
+    def errors(self, value: List[Error]) -> None:
         assert is_list_of_instances_of_type(value, type_=Error, allow_empty=True), (
             "Param `errors` must be a list where each item is of type `valcheck.models.Error`"
         )
         self._errors = value
 
-    @property
-    def converted_value(self) -> Union[Any, Empty]:
-        return self._converted_value
-
-    @converted_value.setter
-    def converted_value(self, value: Union[Any, Empty]) -> None:
-        self._converted_value = value
-
 
 class Field:
     """Class that represents a field (that needs to be validated)"""
 
     def __init__(
             self,
             *,
             required: Optional[bool] = True,
             nullable: Optional[bool] = False,
             default_factory: Optional[Callable] = None,
+            converter_factory: Optional[Callable] = None,
             validators: Optional[List[Callable]] = None,
             error: Optional[Error] = None,
-            converter_factory: Optional[Callable] = None,
         ) -> None:
         """
         Parameters:
             - required (bool): True if the field is required, else False. Default: True
             - nullable (bool): True if the field is nullable, else False. Default: False
             - default_factory (callable): Callable that returns the default value to set for the field
             if `required=False` and the field is missing.
+            - converter_factory (callable): Callable that takes in the validated value (of the field), and returns
+            the converted value (for the field).
             - validators (list of callables): List of callables that each return a boolean (takes the field value as a param).
             The callable returns True if validation is successful, else False.
             - error (Error instance): Instance of type `valcheck.models.Error`.
-            - converter_factory (callable): Callable that takes in the validated value (of the field), and returns
-            the converted value (for the field).
         """
         assert isinstance(required, bool), "Param `required` must be of type 'bool'"
         assert isinstance(nullable, bool), "Param `nullable` must be of type 'bool'"
         assert default_factory is None or callable(default_factory), (
             "Param `default_factory` must be a callable that returns the default value if the field is missing when `required=False`"
         )
+        assert converter_factory is None or callable(converter_factory), (
+            "Param `converter_factory` must be a callable that takes in the validated value (of the field), and returns"
+            " the converted value (for the field)."
+        )
         assert validators is None or isinstance(validators, list), "Param `validators` must be of type 'list'"
         if isinstance(validators, list):
             for validator in validators:
                 assert callable(validator), "Param `validators` must be a list of callables"
         assert error is None or isinstance(error, Error), "Param `error` must be of type `valcheck.models.Error`"
-        assert converter_factory is None or callable(converter_factory), (
-            "Param `converter_factory` must be a callable that takes in the validated value (of the field), and returns"
-            " the converted value (for the field)."
-        )
 
         self._field_name = set_as_empty()
         self._field_value = set_as_empty()
         self.required = required
         self.nullable = nullable
         self.default_factory = default_factory
+        self.converter_factory = converter_factory
         self.validators = validators or []
         self.error = error or Error()
-        self.converter_factory = converter_factory
 
     @property
     def field_name(self) -> str:
         return self._field_name
 
     @field_name.setter
     def field_name(self, value: str) -> None:
@@ -154,52 +136,72 @@
         validator_return_values = [validator(self.field_value) for validator in self.validators]
         for return_value in validator_return_values:
             assert isinstance(return_value, bool), (
                 f"Expected the return type of `validators` to be 'bool', but got '{type(return_value).__name__}'"
             )
         return all(validator_return_values)
 
-    def _get_converted_value(self) -> Union[Any, Empty]:
-        return self.converter_factory(self.field_value) if self.converter_factory else set_as_empty()
+    def _convert_field_value_if_needed(self) -> Any:
+        """Returns the converted field value if a `converter_factory` is present; otherwise returns the same field value"""
+        return self.converter_factory(self.field_value) if self.converter_factory else self.field_value
 
     def validate(self) -> List[Error]:
         """Returns list of errors (each of type `valcheck.models.Error`)"""
         raise NotImplementedError()
 
-    def run_validations(self) -> FieldInfo:
+    def run_validations(self) -> ValidatedField:
         if is_empty(self.field_value) and not self.required and self.default_factory:
             self.field_value = self.default_factory()
-        field_info = FieldInfo(
+        validated_field = ValidatedField(
             field_name=self.field_name,
             field_value=self.field_value,
             errors=[],
-            converted_value=set_as_empty(),
         )
         if is_empty(self.field_value) and not self.required and not self.default_factory:
-            return field_info
+            return validated_field
         if self._can_be_set_to_null():
-            field_info.converted_value = self._get_converted_value()
-            return field_info
+            validated_field.field_value = self._convert_field_value_if_needed()
+            return validated_field
         if is_empty(self.field_value) and self.required:
-            self.error.validator_message = _missing_field_error(self)
-            self.error.append_to_path(self.field_name)
-            field_info.errors += [self.error]
-            return field_info
+            validated_field.errors += [
+                self.create_error_instance(validator_message=self.missing_field_error_message()),
+            ]
+            return validated_field
         errors = self.validate()
         if errors:
-            field_info.errors += errors
-            return field_info
+            validated_field.errors += errors
+            return validated_field
         if not self._has_valid_custom_validators():
-            self.error.validator_message = _invalid_field_error(self)
-            self.error.append_to_path(self.field_name)
-            field_info.errors += [self.error]
-            return field_info
-        field_info.converted_value = self._get_converted_value()
-        return field_info
+            validated_field.errors += [
+                self.create_error_instance(validator_message=self.invalid_field_error_message()),
+            ]
+            return validated_field
+        validated_field.field_value = self._convert_field_value_if_needed()
+        return validated_field
+
+    def invalid_field_error_message(self, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
+        return (
+            f"{prefix if prefix else ''}"
+            f"Invalid {self.__class__.__name__} '{self.field_name}'"
+            f"{suffix if suffix else ''}"
+        )
+
+    def missing_field_error_message(self, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
+        return (
+            f"{prefix if prefix else ''}"
+            f"Missing {self.__class__.__name__} '{self.field_name}'"
+            f"{suffix if suffix else ''}"
+        )
 
+    def create_error_instance(self, *, validator_message: str) -> Error:
+        """Creates and returns a new `valcheck.models.Error` instance for the field"""
+        error_copy = self.error.copy()
+        error_copy.validator_message = validator_message
+        error_copy.append_to_field_path(self.field_name)
+        return error_copy
 
 
 class AnyField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(AnyField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
@@ -209,241 +211,225 @@
 class BooleanField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(BooleanField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, bool):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class StringField(Field):
 
     def __init__(self, *, allow_empty: Optional[bool] = True, **kwargs: Any) -> None:
         self.allow_empty = allow_empty
         super(StringField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if is_valid_object_of_type(self.field_value, type_=str, allow_empty=self.allow_empty):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class JsonStringField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(JsonStringField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, str) and is_valid_json_string(self.field_value):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class EmailIdField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(EmailIdField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, str) and is_valid_email_id(self.field_value):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class UuidStringField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(UuidStringField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, str) and is_valid_uuid_string(self.field_value):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class DateStringField(Field):
     def __init__(self, *, format_: Optional[str] = "%Y-%m-%d", **kwargs: Any) -> None:
         self.format_ = format_
         super(DateStringField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, str) and is_valid_datetime_string(self.field_value, self.format_):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class DatetimeStringField(Field):
     def __init__(self, *, format_: Optional[str] = "%Y-%m-%d %H:%M:%S", **kwargs: Any) -> None:
         self.format_ = format_
         super(DatetimeStringField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, str) and is_valid_datetime_string(self.field_value, self.format_):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class ChoiceField(Field):
     def __init__(self, *, choices: Iterable[Any], **kwargs: Any) -> None:
         assert is_iterable(choices), "Param `choices` must be an iterable"
         self.choices = choices
         super(ChoiceField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if self.field_value in self.choices:
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class MultiChoiceField(Field):
     def __init__(self, *, choices: Iterable[Any], **kwargs: Any) -> None:
         assert is_iterable(choices), "Param `choices` must be an iterable"
         self.choices = choices
         super(MultiChoiceField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if (
             isinstance(self.field_value, list)
             and all([item in self.choices for item in self.field_value])
         ):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class BytesField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(BytesField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, bytes):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class NumberField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(NumberField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if is_instance_of_any(obj=self.field_value, types=[int, float]):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class IntegerField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(IntegerField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, int):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
 class FloatField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(FloatField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if isinstance(self.field_value, float):
             return []
-        self.error.validator_message = _invalid_field_error(self)
-        self.error.append_to_path(self.field_name)
-        return [self.error]
+        return [self.create_error_instance(validator_message=self.invalid_field_error_message())]
 
 
-class DictionaryOfModelField(Field):
+class ModelDictionaryField(Field):
     def __init__(self, *, validator_model: Type, **kwargs: Any) -> None:
         from valcheck.validator import Validator
         assert validator_model is not Validator and issubclass(validator_model, Validator), (
             "Param `validator_model` must be a sub-class of `valcheck.validator.Validator`"
         )
         kwargs_to_disallow = ['validators', 'error']
         if dict_has_any_keys(kwargs, keys=kwargs_to_disallow):
-            raise ValueError(f"This field does not accept the following params: {kwargs_to_disallow}")
+            msg = (
+                f"This field does not accept the following params: {kwargs_to_disallow}, since"
+                " the `validator_model` handles these parameters"
+            )
+            raise ValueError(msg)
         self.validator_model = validator_model
-        super(DictionaryOfModelField, self).__init__(**kwargs)
+        super(ModelDictionaryField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if not isinstance(self.field_value, dict):
-            error = Error()
-            error.validator_message = _invalid_field_error(self, suffix=" - Field is not a dictionary")
-            error.append_to_path(self.field_name)
+            error = self.create_error_instance(
+                validator_message=self.invalid_field_error_message(suffix=" - Field is not a dictionary"),
+            )
             return [error]
         validator = self.validator_model(data=self.field_value)
         error_objs = validator.run_validations()
         for error_obj in error_objs:
-            error_obj.validator_message = _invalid_field_error(self, suffix=f" - {error_obj.validator_message}")
-            error_obj.append_to_path(self.field_name)
+            error_obj.validator_message = self.invalid_field_error_message(suffix=f" - {error_obj.validator_message}")
+            error_obj.append_to_field_path(self.field_name)
+        if not error_objs:
+            self.field_value = validator.validated_data
         return error_objs
 
 
-class ListOfModelsField(Field):
+class ModelListField(Field):
     def __init__(self, *, validator_model: Type, allow_empty: Optional[bool] = True, **kwargs: Any) -> None:
         from valcheck.validator import Validator
         assert validator_model is not Validator and issubclass(validator_model, Validator), (
             "Param `validator_model` must be a sub-class of `valcheck.validator.Validator`"
         )
         kwargs_to_disallow = ['validators', 'error']
         if dict_has_any_keys(kwargs, keys=kwargs_to_disallow):
-            raise ValueError(f"This field does not accept the following params: {kwargs_to_disallow}")
+            msg = (
+                f"This field does not accept the following params: {kwargs_to_disallow}, since"
+                " the `validator_model` handles these parameters"
+            )
+            raise ValueError(msg)
         self.validator_model = validator_model
         self.allow_empty = allow_empty
-        super(ListOfModelsField, self).__init__(**kwargs)
+        super(ModelListField, self).__init__(**kwargs)
 
     def validate(self) -> List[Error]:
         if not isinstance(self.field_value, list):
-            error = Error()
-            error.validator_message = _invalid_field_error(self, suffix=" - Field is not a list")
-            error.append_to_path(self.field_name)
+            error = self.create_error_instance(
+                validator_message=self.invalid_field_error_message(suffix=" - Field is not a list"),
+            )
             return [error]
         if not self.allow_empty and not self.field_value:
-            error = Error()
-            error.validator_message = _invalid_field_error(self, suffix=" - Field is an empty list")
-            error.append_to_path(self.field_name)
+            error = self.create_error_instance(
+                validator_message=self.invalid_field_error_message(suffix=" - Field is an empty list"),
+            )
             return [error]
         errors: List[Error] = []
+        validated_field_value = []
         for idx, item in enumerate(self.field_value):
             row_number = idx + 1
             row_number_string = f"<Row number: {row_number}>"
             if not isinstance(item, dict):
-                error = Error()
-                error.validator_message = _invalid_field_error(
-                    self,
-                    suffix=f" - Row is not a dictionary {row_number_string}",
+                error = self.create_error_instance(
+                    validator_message=self.invalid_field_error_message(suffix=f" - Row is not a dictionary {row_number_string}"),
                 )
-                error.append_to_path(self.field_name)
                 errors.append(error)
                 continue
             validator = self.validator_model(data=item)
             error_objs = validator.run_validations()
+            validated_field_value.append(validator.validated_data)
             for error_obj in error_objs:
-                error_obj.validator_message = _invalid_field_error(
-                    self,
+                error_obj.validator_message = self.invalid_field_error_message(
                     suffix=f" - {error_obj.validator_message} {row_number_string}",
                 )
-                error_obj.append_to_path(self.field_name)
+                error_obj.append_to_field_path(self.field_name)
             errors.extend(error_objs)
+        if not errors:
+            self.field_value = validated_field_value
         return errors
```

### Comparing `valcheck-0.3.6/valcheck/models.py` & `valcheck-0.3.7/valcheck/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+from copy import deepcopy
 from typing import Any, Dict, Optional
 
 
 class Error:
     """Class that represents an error"""
 
     def __init__(
@@ -14,57 +17,63 @@
         assert (description is None or isinstance(description, str)), "Param `description` must be a string"
         assert (code is None or isinstance(code, str)), "Param `code` must be a string"
         assert (details is None or isinstance(details, dict)), "Param `details` must be a dictionary"
         self.description = description or ""
         self.code = code or ""
         self.details = details or {}
         self._validator_message = ""
-        self._path = ""
+        self._field_path = ""
+
+    def copy(self) -> Error:
+        """Returns deep-copy of current `Error` object"""
+        return deepcopy(self)
 
     @property
     def validator_message(self) -> str:
         return self._validator_message
 
     @validator_message.setter
     def validator_message(self, value: str) -> None:
         assert isinstance(value, str), "The param `validator_message` must be a string"
         self._validator_message = value
 
-    def append_to_path(
+    @property
+    def field_path(self) -> str:
+        return self._field_path
+
+    @field_path.setter
+    def field_path(self, value: str) -> None:
+        assert isinstance(value, str), "The param `field_path` must be a string"
+        self._field_path = value
+
+    def append_to_field_path(
             self,
             s: str,
             /,
             *,
             at_beginning: Optional[bool] = True,
             separator: Optional[str] = ".",
         ) -> None:
-        """Updates path in-place"""
-        if not self.path:
-            self.path += s
+        """Appends the given string `s` to the `field_path` (in-place)"""
+        if not self.field_path:
+            self.field_path += s
             return
-        self.path = (
-            s + separator + self.path
+        self.field_path = (
+            s + separator + self.field_path
             if at_beginning else
-            self.path + separator + s
+            self.field_path + separator + s
         )
 
-    @property
-    def path(self) -> str:
-        return self._path
-
-    @path.setter
-    def path(self, value: str) -> None:
-        assert isinstance(value, str), "The param `path` must be a string"
-        self._path = value
-
     def as_dict(self) -> Dict[str, Any]:
         return {
             "description": self.description,
             "code": self.code,
             "details": self.details,
-            "validator_message": self.validator_message,
-            "path": self.path,
+            "validator_info": {
+                "validator_message": self.validator_message,
+                "field_path": self.field_path,
+            },
         }
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.as_dict()})"
```

### Comparing `valcheck-0.3.6/valcheck/utils.py` & `valcheck-0.3.7/valcheck/utils.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.3.6/valcheck/validator.py` & `valcheck-0.3.7/valcheck/validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from valcheck.exceptions import MissingFieldException, ValidationException
 from valcheck.fields import Field
 from valcheck.models import Error
-from valcheck.utils import is_empty, is_list_of_instances_of_type, set_as_empty
+from valcheck.utils import Empty, is_empty, is_list_of_instances_of_type, set_as_empty
 
 
 class Validator:
     """
     Properties:
-        - converted_data
         - validated_data
 
     Instance methods:
         - get_field_value()
         - list_field_validators()
         - model_validator()
         - run_validations()
@@ -21,15 +20,14 @@
 
     def __init__(self, *, data: Dict[str, Any]) -> None:
         assert isinstance(data, dict), "Param `data` must be a dictionary"
         self.data = data
         self._field_info: Dict[str, Field] = self._get_field_info()
         self._errors: List[Error] = []
         self._validated_data: Dict[str, Any] = {}
-        self._converted_data: Dict[str, Any] = {}
 
     def list_field_validators(self) -> List[Dict[str, Any]]:
         return [
             {
                 "field_type": field.__class__.__name__,
                 "field_name": field_name,
             } for field_name, field in self._field_info.items()
@@ -60,53 +58,33 @@
     def validated_data(self) -> Dict[str, Any]:
         return self._validated_data
 
     def _clear_validated_data(self) -> None:
         """Clears out the dictionary having validated data"""
         self._validated_data.clear()
 
-    def _register_converted_data(self, *, field_name: str, value: Any) -> None:
-        self._converted_data[field_name] = value
-
-    def _clear_converted_data(self) -> None:
-        """Clears out the dictionary having converted data"""
-        self._converted_data.clear()
-
-    @property
-    def converted_data(self) -> Dict[str, Any]:
-        return self._converted_data
-
-    def get_field_value(self, field: str, /) -> Any:
-        """Returns the validated field value. Raises `valcheck.exceptions.MissingFieldException` if the field is missing"""
+    def get_field_value(self, field: str, default: Union[Any, Empty] = set_as_empty(), /) -> Any:
+        """
+        Returns the validated field value. Raises `valcheck.exceptions.MissingFieldException` if the field
+        is missing, and no default is provided.
+        """
         if field in self.validated_data:
             return self.validated_data[field]
+        if not is_empty(default):
+            return default
         raise MissingFieldException(f"The field '{field}' is missing from the validated data")
 
-    def get_converted_value(self, field: str, /) -> Any:
-        """
-        Returns the converted value of the field.
-        Raises `valcheck.exceptions.MissingFieldException` if the field's converted value is missing.
-        """
-        if field in self.converted_data:
-            return self.converted_data[field]
-        raise MissingFieldException(f"The field '{field}' is missing from the converted data")
-
     def _perform_field_validation_checks(self, *, field: Field) -> None:
-        """Performs validation checks for the given field, and registers errors (if any) and validated-data/converted-data"""
-        field_info = field.run_validations()
-        if field_info.errors:
-            self._register_errors(errors=field_info.errors)
+        """Performs validation checks for the given field, and registers errors (if any) and validated-data"""
+        validated_field = field.run_validations()
+        if validated_field.errors:
+            self._register_errors(errors=validated_field.errors)
             return
-        if not is_empty(field_info.field_value):
-            self._register_validated_data(field_name=field_info.field_name, field_value=field_info.field_value)
-        if not is_empty(field_info.field_value) and not is_empty(field_info.converted_value):
-            self._register_converted_data(
-                field_name=field_info.field_name,
-                value=field_info.converted_value,
-            )
+        if not is_empty(validated_field.field_value):
+            self._register_validated_data(field_name=validated_field.field_name, field_value=validated_field.field_value)
 
     def _perform_model_validation_checks(self) -> None:
         """Performs model validation checks, and registers errors (if any)"""
         errors = self.model_validator()
         assert is_list_of_instances_of_type(errors, type_=Error, allow_empty=True), (
             "The output of the model validator method must be a list of errors (each of type `valcheck.models.Error`)."
             " Must be an empty list if there are no errors."
@@ -122,27 +100,25 @@
         The output of the model validator method must be a list of errors (each of type `valcheck.models.Error`).
         Must be an empty list if there are no errors.
         """
         return []
 
     def run_validations(self, *, raise_exception: Optional[bool] = False) -> List[Error]:
         """
-        Runs validations and registers errors/validated-data/converted-data. Returns list of errors.
+        Runs validations and registers errors/validated-data. Returns list of errors.
         If `raise_exception=True` and validations fail, raises `valcheck.exceptions.ValidationException`.
         """
         self._clear_errors()
         self._clear_validated_data()
-        self._clear_converted_data()
         for field_name, field in self._field_info.items():
             field.field_name = field_name
             field.field_value = self.data.get(field_name, set_as_empty())
             self._perform_field_validation_checks(field=field)
         # Perform model validation checks only if there are no errors in field validation checks
         if not self._errors:
             self._perform_model_validation_checks()
         if self._errors:
             self._clear_validated_data()
-            self._clear_converted_data()
         if raise_exception and self._errors:
             raise ValidationException(errors=self._errors)
         return self._errors
```

### Comparing `valcheck-0.3.6/valcheck.egg-info/PKG-INFO` & `valcheck-0.3.7/valcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.3.6
+Version: 0.3.7
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

