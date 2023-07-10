# Comparing `tmp/flask_validators-0.3.tar.gz` & `tmp/flask_validators-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_validators-0.3.tar", last modified: Wed Jul  5 13:35:23 2023, max compression
+gzip compressed data, was "flask_validators-0.4.tar", last modified: Mon Jul 10 10:12:25 2023, max compression
```

## Comparing `flask_validators-0.3.tar` & `flask_validators-0.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6742 2023-07-05 13:35:23.661429 flask_validators-0.3/PKG-INFO
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6446 2023-07-05 13:24:53.000000 flask_validators-0.3/README.md
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      241 2023-07-05 13:15:14.000000 flask_validators-0.3/flask_validators/__init__.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/controllers/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:26.000000 flask_validators-0.3/flask_validators/controllers/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      151 2023-07-04 11:51:41.000000 flask_validators-0.3/flask_validators/controllers/error_handler.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      586 2023-07-04 12:16:58.000000 flask_validators-0.3/flask_validators/controllers/validator.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/decorators/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:48:52.000000 flask_validators-0.3/flask_validators/decorators/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3228 2023-07-05 13:19:21.000000 flask_validators-0.3/flask_validators/decorators/validation_decorator.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators/models/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:06.000000 flask_validators-0.3/flask_validators/models/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5102 2023-07-05 10:16:41.000000 flask_validators-0.3/flask_validators/models/fields.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     4838 2023-07-05 10:16:47.000000 flask_validators-0.3/flask_validators/models/schema.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/flask_validators.egg-info/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6742 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/PKG-INFO
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      657 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/SOURCES.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        1 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/dependency_links.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        6 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/requires.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       23 2023-07-05 13:35:23.000000 flask_validators-0.3/flask_validators.egg-info/top_level.txt
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       38 2023-07-05 13:35:23.661429 flask_validators-0.3/setup.cfg
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      687 2023-07-05 13:35:20.000000 flask_validators-0.3/setup.py
-drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-05 13:35:23.661429 flask_validators-0.3/tests/
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:42.000000 flask_validators-0.3/tests/__init__.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      675 2023-07-05 13:19:02.000000 flask_validators-0.3/tests/test_flask.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      107 2023-07-04 11:59:50.000000 flask_validators-0.3/tests/test_schemas.py
--rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3470 2023-07-05 09:52:23.000000 flask_validators-0.3/tests/test_validations.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-10 10:12:25.298610 flask_validators-0.4/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6742 2023-07-10 10:12:25.295277 flask_validators-0.4/PKG-INFO
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6542 2023-07-10 10:10:17.000000 flask_validators-0.4/README.md
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-10 10:12:25.295277 flask_validators-0.4/flask_validators/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      269 2023-07-10 09:57:19.000000 flask_validators-0.4/flask_validators/__init__.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-10 10:12:25.295277 flask_validators-0.4/flask_validators/controllers/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:26.000000 flask_validators-0.4/flask_validators/controllers/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      151 2023-07-04 11:51:41.000000 flask_validators-0.4/flask_validators/controllers/error_handler.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      586 2023-07-04 12:16:58.000000 flask_validators-0.4/flask_validators/controllers/validator.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-10 10:12:25.295277 flask_validators-0.4/flask_validators/decorators/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:48:52.000000 flask_validators-0.4/flask_validators/decorators/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     4479 2023-07-10 10:03:48.000000 flask_validators-0.4/flask_validators/decorators/validation_decorator.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-10 10:12:25.295277 flask_validators-0.4/flask_validators/models/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:06.000000 flask_validators-0.4/flask_validators/models/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5731 2023-07-10 09:41:11.000000 flask_validators-0.4/flask_validators/models/fields.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     5423 2023-07-10 09:41:57.000000 flask_validators-0.4/flask_validators/models/schema.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      557 2023-07-10 10:07:15.000000 flask_validators-0.4/flask_validators/models/validate_db.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-10 10:12:25.295277 flask_validators-0.4/flask_validators.egg-info/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     6742 2023-07-10 10:12:25.000000 flask_validators-0.4/flask_validators.egg-info/PKG-INFO
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      696 2023-07-10 10:12:25.000000 flask_validators-0.4/flask_validators.egg-info/SOURCES.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        1 2023-07-10 10:12:25.000000 flask_validators-0.4/flask_validators.egg-info/dependency_links.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       23 2023-07-10 10:12:25.000000 flask_validators-0.4/flask_validators.egg-info/requires.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       23 2023-07-10 10:12:25.000000 flask_validators-0.4/flask_validators.egg-info/top_level.txt
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)       38 2023-07-10 10:12:25.298610 flask_validators-0.4/setup.cfg
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      727 2023-07-10 10:08:24.000000 flask_validators-0.4/setup.py
+drwxr-xr-x   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-10 10:12:25.295277 flask_validators-0.4/tests/
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)        0 2023-07-04 11:49:42.000000 flask_validators-0.4/tests/__init__.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     1322 2023-07-10 10:07:34.000000 flask_validators-0.4/tests/test_flask.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)      107 2023-07-04 11:59:50.000000 flask_validators-0.4/tests/test_schemas.py
+-rw-r--r--   0 mikef0x   (1000) mikef0x   (1000)     3470 2023-07-05 09:52:23.000000 flask_validators-0.4/tests/test_validations.py
```

### Comparing `flask_validators-0.3/PKG-INFO` & `flask_validators-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_validators
-Version: 0.3
+Version: 0.4
 Summary: Flask request validation
 Author: Dimitri Zhorzholiani
 Author-email: zhorzholiani.dimitri@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `flask_validators-0.3/README.md` & `flask_validators-0.4/flask_validators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+Metadata-Version: 2.1
+Name: flask-validators
+Version: 0.4
+Summary: Flask request validation
+Author: Dimitri Zhorzholiani
+Author-email: zhorzholiani.dimitri@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Flask Validator
 
 Flask Validator is a powerful package designed to simplify data validation in Flask applications. It provides an easy-to-use interface for defining data validation rules and seamlessly integrates with Flask routes using a custom decorator.
 
 * **Simplified Data Validation:** Flask Validator streamlines the process of validating data in Flask applications, reducing the complexity and boilerplate code.
 * **Integration with Flask Routes:** The package seamlessly integrates with Flask routes through a custom decorator, making it easy to apply validation rules to specific endpoints.
 * **Flexible Validation Schema:** Flask Validator allows you to define validation rules using a schema structure, providing a clear and organized way to specify the expected data format.
 * **Custom Validators:** You can create custom validators to extend the validation capabilities of Flask Validator, enabling you to implement complex validation logic tailored to your application's needs.
 * **Error Handling:** Flask Validator automatically generates error messages based on the defined validation rules, simplifying the process of handling validation failures and providing 
 
-<p align="center">
-  <img src="./carbon.png" alt="Size Limit CLI" width="738">
-</p>
 
 With the help of Flask Validator, you can ensure the integrity and consistency of the data submitted to your Flask endpoints, enhancing the reliability and security of your application.
 
 ## How It Works
 
 1. Flask Validator provides a custom decorator, @validate_form, which can be applied to Flask routes.
 2. The decorator takes a validation schema as its argument, defined using the Schema class and Field class from Flask Validator. 
@@ -105,8 +114,8 @@
         return False, 'Validation failed.'
 ```
 
 ## Error Handling
 If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
 
 ## Error Handling
-If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
+If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
```

### Comparing `flask_validators-0.3/flask_validators/controllers/validator.py` & `flask_validators-0.4/flask_validators/controllers/validator.py`

 * *Files identical despite different names*

### Comparing `flask_validators-0.3/flask_validators/decorators/validation_decorator.py` & `flask_validators-0.4/tests/test_validations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,103 @@
-from functools import wraps
-from flask import request, jsonify
-from flask_validators.controllers.validator import DataValidator
-from flask_validators.models.schema import Schema
-from flask_validators.models.fields import Field
-
-field_schemas = {
-    'email': Field(required=True, type='string', validators=[
-        {'name': 'email', 'message': 'Invalid email address.'}
-    ]),
-    'name': Field(required=True, type='string', validators=[
-        {'name': 'name', 'message': 'Invalid name.'}
-    ]),
-    'age': Field(required=True, type='integer', validators=[
-        {'name': 'age', 'message': 'Invalid age.', 'args': (0, 120)}
-    ]),
-    'password': Field(required=True, type='string', validators=[
-        {'name': 'password', 'message': 'Invalid password.', 'kwargs': {'min_length': 8, 'max_length': 16, 'require_special_char': True}}
-    ]),
-    'json': Field(required=True, type='string', validators=[
-        {'name': 'json', 'message': 'Invalid JSON.'}
-    ]),
-    'phone': Field(required=True, type='string', validators=[
-        {'name': 'phone', 'message': 'Invalid phone number.'}
-    ]),
-    'zipcode': Field(required=True, type='string', validators=[
-        {'name': 'zipcode', 'message': 'Invalid zipcode.'}
-    ]),
-    'date': Field(required=True, type='string', validators=[
-        {'name': 'date', 'message': 'Invalid date.'}
-    ]),
-    'credit_card': Field(required=True, type='string', validators=[
-        {'name': 'credit_card', 'message': 'Invalid credit card number.'}
-    ]),
-    'ssn': Field(required=True, type='string', validators=[
-        {'name': 'ssn', 'message': 'Invalid social security number.'}
-    ]),
-    'url': Field(required=True, type='string', validators=[
-        {'name': 'url', 'message': 'Invalid URL.'}
-    ]),
-    'ip_address': Field(required=True, type='string', validators=[
-        {'name': 'ip_address', 'message': 'Invalid IP address.'}
-    ]),
-    'hex_color': Field(required=True, type='string', validators=[
-        {'name': 'hex_color', 'message': 'Invalid hexadecimal color code.'}
-    ]),
-    'latitude': Field(required=True, type='string', validators=[
-        {'name': 'latitude', 'message': 'Invalid latitude.'}
-    ]),
-    'longitude': Field(required=True, type='string', validators=[
-        {'name': 'longitude', 'message': 'Invalid longitude.'}
-    ]),
-}
-
-def validate_form(*fields):
-    def decorator(f):
-        @wraps(f)
-        def decorated_function(*args, **kwargs):
-            data = request.get_json()
-
-            if not data:
-                return jsonify({'error': 'No data provided.'}), 400
-
-            errors = {}
-            for field in fields:
-                if field not in field_schemas:
-                    continue
-
-                schema = field_schemas[field]
-
-                if field not in data:
-                    errors[field] = "Missing data"
-                    continue
-
-                value = data.get(field)
-
-                is_valid, error_message = schema.validate(value)
-                if not is_valid:
-                    errors[field] = error_message
-
-            if errors:
-                return jsonify(errors), 400
-
-            return f(*args, **kwargs)
-        return decorated_function
-    return decorator
+import unittest
+from flask_data_validation.controllers.validator import DataValidator
+from flask_data_validation.models.schema import Schema
+from flask_data_validation.models.fields import Field
+
+class TestDataValidation(unittest.TestCase):
+    def test_valid_data(self):
+        # Define the validation schema
+        schema = Schema({
+            'name': Field(required=True, type='string'),
+            'age': Field(required=True, type='integer', validators=[
+                {'name': 'age', 'args': (18, 65), 'message': 'Age must be between 18 and 65.'},
+            ]),
+            'email': Field(required=True, type='string', validators=[
+                {'name': 'email', 'message': 'Invalid email address.'}
+            ])
+        })
+
+        # Create the data validator
+        data = {
+            'name': 'John Doe',
+            'age': 19,
+            'email': 'johndoe@example.com'
+        }
+        validator = DataValidator(schema, data)
+
+        # Test valid data
+        errors = validator.validate()
+        self.assertEqual(errors, {})  # No errors should be returned for valid data
+
+    def test_invalid_name(self):
+        # Define the validation schema
+        schema = Schema({
+            'name': Field(required=True, type='string', validators=[
+                 {'name': 'name', 'message': 'Invalid name.'}
+            ]),
+            'age': Field(required=True, type='integer', validators=[
+                {'name': 'age', 'args': (18, 65), 'message': 'Age must be between 18 and 65.'},
+            ]),
+            'email': Field(required=True, type='string', validators=[
+                {'name': 'email', 'message': 'Invalid email address.'}
+            ])
+        })
+
+        # Create the data validator
+        data = {
+            'name': '',
+            'age': 18,
+            'email': 'johndoe@example.com'
+        }
+        validator = DataValidator(schema, data)
+
+        # Test invalid name
+        errors = validator.validate()
+        expected_errors = {'name': 'Invalid name.'}
+        self.assertEqual(errors, expected_errors)
+
+    def test_invalid_password(self):
+        schema = Schema({
+            'password': Field(required=True, type='string', validators=[
+                {
+                    'name': 'password',
+                    'args': (8, 16, True),  # Here False means we do not require special characters
+                    'message': 'Invalid password.'
+                }
+            ])
+        })
+
+        data = {
+            'name': '',
+            'age': 18,
+            'email': 'johndoe@example.com',
+            'password': '12345678'
+        }
+        validator = DataValidator(schema, data)
+
+        # Test invalid name
+        errors = validator.validate()
+        expected_errors = {'password': 'Password must contain at least one special character.'}
+        self.assertEqual(errors, expected_errors)
+
+    def test_invalid_json(self):
+        schema = Schema({
+            'data': Field(required=True, type='string', validators=[
+                {
+                    'name': 'json',
+                    'message': 'Invalid JSON data.'
+                }
+            ])
+        })
+
+        data = {
+            'data': 'asdad'
+        }
+        validator = DataValidator(schema, data)
+
+        # Test invalid name
+        errors = validator.validate()
+        expected_errors = {'data': 'Invalid JSON.'}
+        self.assertEqual(errors, expected_errors)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `flask_validators-0.3/flask_validators/models/fields.py` & `flask_validators-0.4/flask_validators/models/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,26 @@
         self.validators = validators or []
 
     def validate(self, value):
         if self.required and value is None:
             return False, 'This field is required.'
 
         if self.type:
-            if self.type == 'string' and not isinstance(value, str):
-                return False, 'Expected a string.'
-            elif self.type == 'integer' and not isinstance(value, int):
-                return False, 'Expected an integer.'
-            elif self.type == 'float' and not isinstance(value, float):
-                return False, 'Expected a float.'
-            elif self.type == 'boolean' and not isinstance(value, bool):
-                return False, 'Expected a boolean.'
+            try:
+                if self.type == 'string':
+                    value = str(value)
+                elif self.type == 'integer':
+                    value = int(value)
+                elif self.type == 'float':
+                    value = float(value)
+                elif self.type == 'boolean':
+                    value = bool(value)
+            except ValueError:
+                return False, f'Expected a {self.type}.'
+
             # Add more type validations as needed
 
         for validator in self.validators:
             validator_name = validator['name']
             if validator_name == 'min_age':
                 validator_name = 'age'
             elif validator_name == 'max_age':
@@ -44,15 +48,16 @@
             if validator_name == 'age':
                 min_age, max_age = validator_args
                 is_valid, error_message = validator_func(value, min_age, max_age, **validator_kwargs)
             else:
                 is_valid, error_message = validator_func(value, *validator_args, **validator_kwargs)
 
             if not is_valid:
-                return False, error_message
+                custom_message = validator.get('message')
+                return False, custom_message if custom_message else error_message
 
         return True, None
 
     def validate_email(self, value):
         if re.match(r'^[\w\.-]+@[\w\.-]+\.\w+$', value):
             return True, None
         return False, 'Invalid email address.'
@@ -130,8 +135,23 @@
         if re.match(r'^[-+]?([1-8]?\d(\.\d+)?|90(\.0+)?)$', value):
             return True, None
         return False, 'Invalid latitude.'
 
     def validate_longitude(self, value):
         if re.match(r'^[-+]?(180(\.0+)?|((1[0-7]\d)|([1-9]?\d))(\.\d+)?)$', value):
             return True, None
-        return False, 'Invalid longitude.'
+        return False, 'Invalid longitude.'
+
+    def validate_file(self, value, allowed_extensions=None, max_size=None):
+        if allowed_extensions and value.filename.split('.')[-1] not in allowed_extensions:
+            return False, 'Invalid file extension.'
+        
+        if max_size and value.content_length > max_size:
+            return False, 'File size is too large.'
+
+        return True, None
+
+    def validate_confirm_password(self, value, password_field):
+        password = self.data.get(password_field)
+        if password != value:
+            return False, 'Passwords must match.'
+        return True, None
```

### Comparing `flask_validators-0.3/flask_validators/models/schema.py` & `flask_validators-0.4/flask_validators/models/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,8 +125,23 @@
         if re.match(r'^[-+]?([1-8]?\d(\.\d+)?|90(\.0+)?)$', value):
             return True, None
         return False, 'Invalid latitude.'
 
     def validate_longitude(self, value):
         if re.match(r'^[-+]?(180(\.0+)?|((1[0-7]\d)|([1-9]?\d))(\.\d+)?)$', value):
             return True, None
-        return False, 'Invalid longitude.'
+        return False, 'Invalid longitude.'
+
+    def validate_file(self, value, allowed_extensions=None, max_size=None):
+        if allowed_extensions and value.filename.split('.')[-1] not in allowed_extensions:
+            return False, 'Invalid file extension.'
+        
+        if max_size and value.content_length > max_size:
+            return False, 'File size is too large.'
+
+        return True, None
+
+    def validate_confirm_password(self, value, password_field):
+        password = self.data.get(password_field)
+        if password != value:
+            return False, 'Passwords must match.'
+        return True, None
```

### Comparing `flask_validators-0.3/flask_validators.egg-info/PKG-INFO` & `flask_validators-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-Metadata-Version: 2.1
-Name: flask-validators
-Version: 0.3
-Summary: Flask request validation
-Author: Dimitri Zhorzholiani
-Author-email: zhorzholiani.dimitri@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Flask Validator
 
 Flask Validator is a powerful package designed to simplify data validation in Flask applications. It provides an easy-to-use interface for defining data validation rules and seamlessly integrates with Flask routes using a custom decorator.
 
 * **Simplified Data Validation:** Flask Validator streamlines the process of validating data in Flask applications, reducing the complexity and boilerplate code.
 * **Integration with Flask Routes:** The package seamlessly integrates with Flask routes through a custom decorator, making it easy to apply validation rules to specific endpoints.
 * **Flexible Validation Schema:** Flask Validator allows you to define validation rules using a schema structure, providing a clear and organized way to specify the expected data format.
 * **Custom Validators:** You can create custom validators to extend the validation capabilities of Flask Validator, enabling you to implement complex validation logic tailored to your application's needs.
 * **Error Handling:** Flask Validator automatically generates error messages based on the defined validation rules, simplifying the process of handling validation failures and providing 
 
+<p align="center">
+  <img src="./carbon.png" alt="CLI" width="738">
+</p>
 
 With the help of Flask Validator, you can ensure the integrity and consistency of the data submitted to your Flask endpoints, enhancing the reliability and security of your application.
 
 ## How It Works
 
 1. Flask Validator provides a custom decorator, @validate_form, which can be applied to Flask routes.
 2. The decorator takes a validation schema as its argument, defined using the Schema class and Field class from Flask Validator. 
@@ -110,12 +101,15 @@
     # Validation logic
     if valid:
         return True, None
     else:
         return False, 'Validation failed.'
 ```
 
+## Currently Working
+Currently I am working on database integration support, any help will be appreciated
+
 ## Error Handling
 If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
 
 ## Error Handling
-If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
+If validation fails, Flask Validator automatically generates error messages based on the defined validation rules. The error response includes a JSON object with the field names as keys and the corresponding error messages as values. This makes it easier to handle validation failures and provide meaningful feedback to the users.
```

### Comparing `flask_validators-0.3/flask_validators.egg-info/SOURCES.txt` & `flask_validators-0.4/flask_validators.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 flask_validators/controllers/error_handler.py
 flask_validators/controllers/validator.py
 flask_validators/decorators/__init__.py
 flask_validators/decorators/validation_decorator.py
 flask_validators/models/__init__.py
 flask_validators/models/fields.py
 flask_validators/models/schema.py
+flask_validators/models/validate_db.py
 tests/__init__.py
 tests/test_flask.py
 tests/test_schemas.py
 tests/test_validations.py
```

### Comparing `flask_validators-0.3/setup.py` & `flask_validators-0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('READMEPypi.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="flask_validators",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     description="Flask request validation",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Dimitri Zhorzholiani",
     author_email="zhorzholiani.dimitri@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=[
         "flask",
+        "flask-sqlalchemy",
+        "",
     ],
     python_requires='>=3.6',
 )
```

