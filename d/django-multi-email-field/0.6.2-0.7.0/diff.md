# Comparing `tmp/django-multi-email-field-0.6.2.tar.gz` & `tmp/django-multi-email-field-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-multi-email-field-0.6.2.tar", last modified: Thu Jul 23 14:00:08 2020, max compression
+gzip compressed data, was "django-multi-email-field-0.7.0.tar", last modified: Mon Jul 10 08:49:56 2023, max compression
```

## Comparing `django-multi-email-field-0.6.2.tar` & `django-multi-email-field-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sebcorbin   (501)     1000        0 2020-07-23 14:00:08.022881 django-multi-email-field-0.6.2/
--rw-r--r--   0 sebcorbin   (501)     1000      992 2020-07-23 13:55:16.000000 django-multi-email-field-0.6.2/CHANGES
--rw-r--r--   0 sebcorbin   (501)     1000     7651 2020-02-04 16:48:45.000000 django-multi-email-field-0.6.2/LICENSE
--rw-r--r--   0 sebcorbin   (501)     1000       34 2020-02-04 16:48:45.000000 django-multi-email-field-0.6.2/MANIFEST.in
--rw-r--r--   0 sebcorbin   (501)     1000     5330 2020-07-23 14:00:08.022470 django-multi-email-field-0.6.2/PKG-INFO
--rw-r--r--   0 sebcorbin   (501)     1000     1979 2020-02-05 15:18:13.000000 django-multi-email-field-0.6.2/README.rst
-drwxr-xr-x   0 sebcorbin   (501)     1000        0 2020-07-23 14:00:08.018910 django-multi-email-field-0.6.2/django_multi_email_field.egg-info/
--rw-r--r--   0 sebcorbin   (501)     1000     5330 2020-07-23 14:00:07.000000 django-multi-email-field-0.6.2/django_multi_email_field.egg-info/PKG-INFO
--rw-r--r--   0 sebcorbin   (501)     1000      578 2020-07-23 14:00:07.000000 django-multi-email-field-0.6.2/django_multi_email_field.egg-info/SOURCES.txt
--rw-r--r--   0 sebcorbin   (501)     1000        1 2020-07-23 14:00:07.000000 django-multi-email-field-0.6.2/django_multi_email_field.egg-info/dependency_links.txt
--rw-r--r--   0 sebcorbin   (501)     1000        1 2020-07-23 14:00:07.000000 django-multi-email-field-0.6.2/django_multi_email_field.egg-info/not-zip-safe
--rw-r--r--   0 sebcorbin   (501)     1000        7 2020-07-23 14:00:07.000000 django-multi-email-field-0.6.2/django_multi_email_field.egg-info/requires.txt
--rw-r--r--   0 sebcorbin   (501)     1000       18 2020-07-23 14:00:07.000000 django-multi-email-field-0.6.2/django_multi_email_field.egg-info/top_level.txt
-drwxr-xr-x   0 sebcorbin   (501)     1000        0 2020-07-23 14:00:08.020639 django-multi-email-field-0.6.2/multi_email_field/
--rw-r--r--   0 sebcorbin   (501)     1000        0 2020-02-04 16:48:45.000000 django-multi-email-field-0.6.2/multi_email_field/__init__.py
--rw-r--r--   0 sebcorbin   (501)     1000     1388 2020-07-23 13:54:22.000000 django-multi-email-field-0.6.2/multi_email_field/fields.py
--rw-r--r--   0 sebcorbin   (501)     1000      998 2020-02-05 13:03:56.000000 django-multi-email-field-0.6.2/multi_email_field/forms.py
--rw-r--r--   0 sebcorbin   (501)     1000       48 2020-02-04 16:48:45.000000 django-multi-email-field-0.6.2/multi_email_field/models.py
-drwxr-xr-x   0 sebcorbin   (501)     1000        0 2020-07-23 14:00:08.021864 django-multi-email-field-0.6.2/multi_email_field/tests/
--rw-r--r--   0 sebcorbin   (501)     1000       17 2020-02-05 13:03:56.000000 django-multi-email-field-0.6.2/multi_email_field/tests/__init__.py
--rw-r--r--   0 sebcorbin   (501)     1000      248 2020-07-23 13:54:22.000000 django-multi-email-field-0.6.2/multi_email_field/tests/models.py
--rw-r--r--   0 sebcorbin   (501)     1000     6114 2020-07-23 13:54:22.000000 django-multi-email-field-0.6.2/multi_email_field/tests/tests.py
--rw-r--r--   0 sebcorbin   (501)     1000      899 2020-02-05 15:48:18.000000 django-multi-email-field-0.6.2/multi_email_field/widgets.py
--rw-r--r--   0 sebcorbin   (501)     1000       38 2020-07-23 14:00:08.023039 django-multi-email-field-0.6.2/setup.cfg
--rw-r--r--   0 sebcorbin   (501)     1000     1399 2020-07-23 13:56:16.000000 django-multi-email-field-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:49:56.676719 django-multi-email-field-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-07-10 08:49:56.676719 django-multi-email-field-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:49:56.676719 django-multi-email-field-0.7.0/django_multi_email_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-07-10 08:49:56.000000 django-multi-email-field-0.7.0/django_multi_email_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-10 08:49:56.000000 django-multi-email-field-0.7.0/django_multi_email_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:49:56.000000 django-multi-email-field-0.7.0/django_multi_email_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-10 08:49:56.000000 django-multi-email-field-0.7.0/django_multi_email_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 08:49:56.000000 django-multi-email-field-0.7.0/django_multi_email_field.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:49:56.676719 django-multi-email-field-0.7.0/multi_email_field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:49:56.676719 django-multi-email-field-0.7.0/multi_email_field/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/multi_email_field/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:49:56.676719 django-multi-email-field-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:49:45.000000 django-multi-email-field-0.7.0/setup.py
```

### Comparing `django-multi-email-field-0.6.2/CHANGES` & `django-multi-email-field-0.7.0/CHANGES`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 CHANGELOG
 =========
 
+0.7.0 (2023-07-10)
+==================
+
+- Django 4 compatibility
+- Removed Django (1.11,2.2/3.0/3.1) compatibility
+- Moved CI/CD to Github Actions
+
 0.6.2 (2020-07-23)
 ==================
 
 - Set default value to [] in MultiEmailField
 
 
 0.6.1 (2020-02-05)
```

### Comparing `django-multi-email-field-0.6.2/LICENSE` & `django-multi-email-field-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-multi-email-field-0.6.2/README.rst` & `django-multi-email-field-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-multi-email-field-0.6.2/django_multi_email_field.egg-info/SOURCES.txt` & `django-multi-email-field-0.7.0/django_multi_email_field.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 django_multi_email_field.egg-info/PKG-INFO
 django_multi_email_field.egg-info/SOURCES.txt
 django_multi_email_field.egg-info/dependency_links.txt
-django_multi_email_field.egg-info/not-zip-safe
 django_multi_email_field.egg-info/requires.txt
 django_multi_email_field.egg-info/top_level.txt
 multi_email_field/__init__.py
 multi_email_field/fields.py
 multi_email_field/forms.py
 multi_email_field/models.py
 multi_email_field/widgets.py
```

### Comparing `django-multi-email-field-0.6.2/multi_email_field/fields.py` & `django-multi-email-field-0.7.0/multi_email_field/fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 from django.db import models
 
 from multi_email_field.forms import MultiEmailField as MultiEmailFormField
 
-try:
-    from django.utils import six
-
-    string_types = six.string_types
-except ImportError:
-    string_types = str
-
 
 class MultiEmailField(models.Field):
     description = "A multi e-mail field stored as a multi-lines text"
-    
+
     def __init__(self, *args, **kwargs):
-        kwargs.setdefault('default', [])
+        kwargs.setdefault("default", [])
         super(MultiEmailField, self).__init__(*args, **kwargs)
 
     def formfield(self, **kwargs):
         # This is a fairly standard way to set up some defaults
         # while letting the caller override them.
-        defaults = {'form_class': MultiEmailFormField}
+        defaults = {"form_class": MultiEmailFormField}
         defaults.update(kwargs)
         return super(MultiEmailField, self).formfield(**defaults)
 
     def from_db_value(self, value, expression, connection, context=None):
         if value is None:
             return []
         return value.splitlines()
 
     def get_db_prep_value(self, value, connection, prepared=False):
-        if isinstance(value, string_types):
+        if isinstance(value, str):
             return value
         elif isinstance(value, list):
             return "\n".join(value)
 
     def to_python(self, value):
         if not value:
             return []
         if isinstance(value, list):
             return value
         return value.splitlines()
 
     def get_internal_type(self):
-        return 'TextField'
+        return "TextField"
```

### Comparing `django-multi-email-field-0.6.2/multi_email_field/forms.py` & `django-multi-email-field-0.7.0/multi_email_field/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from django import forms
 from django.core.validators import validate_email
 from django.core.exceptions import ValidationError
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from multi_email_field.widgets import MultiEmailWidget
 
 
 class MultiEmailField(forms.Field):
-    message = _('Enter valid email addresses.')
-    code = 'invalid'
+    message = _("Enter valid email addresses.")
+    code = "invalid"
     widget = MultiEmailWidget
 
     def to_python(self, value):
         "Normalize data to a list of strings."
         # Return None if no input was given.
         if not value:
             return []
         return [v.strip() for v in value.splitlines() if v != ""]
 
     def validate(self, value):
-        """ Check if value consists only of valid emails. """
+        """Check if value consists only of valid emails."""
 
         # Use the parent's handling of required fields, etc.
         super(MultiEmailField, self).validate(value)
         try:
             for email in value:
                 validate_email(email)
         except ValidationError:
```

### Comparing `django-multi-email-field-0.6.2/multi_email_field/tests/tests.py` & `django-multi-email-field-0.7.0/multi_email_field/tests/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,48 +10,45 @@
 
 
 class MultiEmailFormTest(SimpleTestCase):
     def test__form(self):
         class TestForm(forms.Form):
             f = MultiEmailFormField()
 
-        form = TestForm(initial={'f': ['foo@foo.fr', 'bar@bar.fr']})
+        form = TestForm(initial={"f": ["foo@foo.fr", "bar@bar.fr"]})
         output = form.as_p()
-        self.assertEqual(1, len(pq('textarea', output)))
+        self.assertEqual(1, len(pq("textarea", output)))
         # The template-based widget add a line-return
-        value = pq('textarea', output).text()
-        self.assertEqual(
-            value.lstrip(),
-            'foo@foo.fr\nbar@bar.fr'
-        )
+        value = pq("textarea", output).text()
+        self.assertEqual(value.lstrip(), "foo@foo.fr\nbar@bar.fr")
 
 
 class MultiEmailModelFormTest(TestCase):
     def test__model_form(self):
         class TestModelForm(forms.ModelForm):
             class Meta:
                 model = TestModel
                 fields = forms.ALL_FIELDS
 
         form = TestModelForm()
-        self.assertIsInstance(form.fields['f'].widget, MultiEmailWidget)
+        self.assertIsInstance(form.fields["f"].widget, MultiEmailWidget)
 
-        form = TestModelForm(data={'f': 'foo@foo.fr\nbar@bar.fr'})
+        form = TestModelForm(data={"f": "foo@foo.fr\nbar@bar.fr"})
         self.assertTrue(form.is_valid())
         instance = form.save()
-        self.assertEqual(instance.f, ['foo@foo.fr', 'bar@bar.fr'])
+        self.assertEqual(instance.f, ["foo@foo.fr", "bar@bar.fr"])
 
         form = TestModelForm(instance=instance)
         output = form.as_p()
-        self.assertEqual(2, len(pq('textarea', output)))
+        self.assertEqual(2, len(pq("textarea", output)))
         # The template-based widget add a line-return
-        value = pq('textarea:first', output).text()
+        value = pq("textarea:first", output).text()
         self.assertEqual(
             value.lstrip(),
-            'foo@foo.fr\nbar@bar.fr',
+            "foo@foo.fr\nbar@bar.fr",
         )
 
 
 class MultiEmailModelTest(TestCase):
     def test_default_value(self):
         self.assertEqual(TestModel().f, [])
 
@@ -60,116 +57,112 @@
 
     def test__clean(self):
         # Nothing of these should raise a ValidationError
         TestModel().full_clean()
         TestModel(f="").full_clean()
         TestModel(f=None).full_clean()
         TestModel(f=False).full_clean()
-        TestModel(f='foobar@foobar.fr\nbaz@baz.fr').full_clean()
-        TestModel(f=['foo@foo.fr', 'bar@bar.fr']).full_clean()
+        TestModel(f="foobar@foobar.fr\nbaz@baz.fr").full_clean()
+        TestModel(f=["foo@foo.fr", "bar@bar.fr"]).full_clean()
 
     def test__string_based_value(self):
-        emails = 'foobar@foobar.fr\nbaz@baz.fr'
+        emails = "foobar@foobar.fr\nbaz@baz.fr"
         TestModel.objects.create(f=emails)
-        values = TestModel.objects.values_list('f', flat=True)
+        values = TestModel.objects.values_list("f", flat=True)
         self.assertEqual(values[0], emails.splitlines())
 
         qs = TestModel.objects.all()
         self.assertTrue(qs.filter(f=emails).exists())
 
     def test__list_based_value(self):
-        emails = ['foo@foo.fr', 'bar@bar.fr']
+        emails = ["foo@foo.fr", "bar@bar.fr"]
         TestModel.objects.create(f=emails)
 
-        values = TestModel.objects.values_list('f', flat=True)
+        values = TestModel.objects.values_list("f", flat=True)
         self.assertEqual(values[0], emails)
 
     def test__empty_based_value(self):
         qs = TestModel.objects.all()
 
         TestModel.objects.create(f=[])
-        self.assertEqual(qs.values_list('f', flat=True)[0], [])
+        self.assertEqual(qs.values_list("f", flat=True)[0], [])
         self.assertTrue(qs.filter(f=[]).exists())
         self.assertTrue(qs.filter(f="").exists())
         TestModel.objects.all().delete()
 
         TestModel.objects.create(f="")
-        self.assertEqual(qs.values_list('f', flat=True)[0], [])
+        self.assertEqual(qs.values_list("f", flat=True)[0], [])
         self.assertTrue(qs.filter(f=[]).exists())
         self.assertTrue(qs.filter(f="").exists())
         TestModel.objects.all().delete()
 
         TestModel.objects.create(f=None)
-        self.assertEqual(TestModel.objects.values_list('f', flat=True)[0], [])
+        self.assertEqual(TestModel.objects.values_list("f", flat=True)[0], [])
 
         self.assertTrue(qs.filter(f=None).exists())
 
 
 class MultiEmailFormFieldTest(SimpleTestCase):
-
     def test__widget(self):
         f = MultiEmailFormField()
         self.assertIsInstance(f.widget, MultiEmailWidget)
 
     def test__to_python(self):
         f = MultiEmailFormField()
         # Empty values
-        for val in ['', None]:
+        for val in ["", None]:
             self.assertEquals([], f.to_python(val))
         # One line correct value
-        val = '  foo@bar.com    '
-        self.assertEquals(['foo@bar.com'], f.to_python(val))
+        val = "  foo@bar.com    "
+        self.assertEquals(["foo@bar.com"], f.to_python(val))
         # Multi lines correct values (test of #0010614)
-        val = 'foo@bar.com\nfoo2@bar2.com\r\nfoo3@bar3.com'
-        self.assertEquals(['foo@bar.com', 'foo2@bar2.com', 'foo3@bar3.com'],
-                          f.to_python(val))
+        val = "foo@bar.com\nfoo2@bar2.com\r\nfoo3@bar3.com"
+        self.assertEquals(
+            ["foo@bar.com", "foo2@bar2.com", "foo3@bar3.com"], f.to_python(val)
+        )
 
     def test__validate(self):
         f = MultiEmailFormField(required=True)
         # Empty value
         val = []
         self.assertRaises(ValidationError, f.validate, val)
         # Incorrect value
-        val = ['not-an-email.com']
+        val = ["not-an-email.com"]
         self.assertRaises(ValidationError, f.validate, val)
         # An incorrect value with correct values
-        val = ['foo@bar.com', 'not-an-email.com', 'foo3@bar3.com']
+        val = ["foo@bar.com", "not-an-email.com", "foo3@bar3.com"]
         self.assertRaises(ValidationError, f.validate, val)
         # Should not happen (to_python do the strip)
-        val = ['  foo@bar.com    ']
+        val = ["  foo@bar.com    "]
         self.assertRaises(ValidationError, f.validate, val)
         # Correct value
-        val = ['foo@bar.com']
+        val = ["foo@bar.com"]
         f.validate(val)
 
 
 class MultiEmailWidgetTest(SimpleTestCase):
-
     def test__prep_value__empty(self):
         w = MultiEmailWidget()
-        value = w.prep_value('')
-        self.assertEqual(value, '')
+        value = w.prep_value("")
+        self.assertEqual(value, "")
 
     def test__prep_value__string(self):
         w = MultiEmailWidget()
-        value = w.prep_value('foo@foo.fr\nbar@bar.fr')
-        self.assertEqual(value, 'foo@foo.fr\nbar@bar.fr')
+        value = w.prep_value("foo@foo.fr\nbar@bar.fr")
+        self.assertEqual(value, "foo@foo.fr\nbar@bar.fr")
 
     def test__prep_value__list(self):
         w = MultiEmailWidget()
-        value = w.prep_value(['foo@foo.fr', 'bar@bar.fr'])
-        self.assertEqual(value, 'foo@foo.fr\nbar@bar.fr')
+        value = w.prep_value(["foo@foo.fr", "bar@bar.fr"])
+        self.assertEqual(value, "foo@foo.fr\nbar@bar.fr")
 
     def test__prep_value__raise(self):
         w = MultiEmailWidget()
         self.assertRaises(ValidationError, w.prep_value, 42)
 
     def test__render(self):
         w = MultiEmailWidget()
-        output = w.render('test', ['foo@foo.fr', 'bar@bar.fr'])
-        self.assertEqual(1, len(pq('textarea', output)))
+        output = w.render("test", ["foo@foo.fr", "bar@bar.fr"])
+        self.assertEqual(1, len(pq("textarea", output)))
         # The template-based widget add a line-return
-        value = pq('textarea', output).text()
-        self.assertEqual(
-            value.lstrip(),
-            'foo@foo.fr\nbar@bar.fr'
-        )
+        value = pq("textarea", output).text()
+        self.assertEqual(value.lstrip(), "foo@foo.fr\nbar@bar.fr")
```

### Comparing `django-multi-email-field-0.6.2/multi_email_field/widgets.py` & `django-multi-email-field-0.7.0/multi_email_field/widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 from django.forms.widgets import Textarea
 from django.core.exceptions import ValidationError
 from django.core import validators
 
-MULTI_EMAIL_FIELD_EMPTY_VALUES = validators.EMPTY_VALUES + ('[]', )
-
-try:
-    from django.utils import six
-
-    string_types = six.string_types
-except ImportError:
-    string_types = str
+MULTI_EMAIL_FIELD_EMPTY_VALUES = validators.EMPTY_VALUES + ("[]",)
 
 
 class MultiEmailWidget(Textarea):
     is_hidden = False
 
     def prep_value(self, value):
-        """ Prepare value before effectively render widget """
+        """Prepare value before effectively render widget"""
         if value in MULTI_EMAIL_FIELD_EMPTY_VALUES:
             return ""
-        elif isinstance(value, string_types):
+        elif isinstance(value, str):
             return value
         elif isinstance(value, list):
             return "\n".join(value)
-        raise ValidationError('Invalid format.')
+        raise ValidationError("Invalid format.")
 
     def render(self, name, value, **kwargs):
         value = self.prep_value(value)
         return super(MultiEmailWidget, self).render(name, value, **kwargs)
```

