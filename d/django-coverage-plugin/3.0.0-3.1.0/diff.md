# Comparing `tmp/django_coverage_plugin-3.0.0.tar.gz` & `tmp/django_coverage_plugin-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nedbatchelder/coverage/django_coverage_plugin/dist/.tmp-bbzk261g/django_coverage_plugin-3.0.0.tar", last modified: Tue Dec  6 09:56:40 2022, max compression
+gzip compressed data, was "django_coverage_plugin-3.1.0.tar", last modified: Mon Jul 10 13:14:18 2023, max compression
```

## Comparing `django_coverage_plugin-3.0.0.tar` & `django_coverage_plugin-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      200 2021-05-25 01:35:09.000000 django_coverage_plugin-3.0.0/AUTHORS.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10174 2016-06-02 15:25:30.000000 django_coverage_plugin-3.0.0/LICENSE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      371 2021-06-08 23:05:46.000000 django_coverage_plugin-3.0.0/MANIFEST.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      631 2022-05-04 10:26:03.000000 django_coverage_plugin-3.0.0/NOTICE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     8747 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     8470 2022-12-06 09:52:33.000000 django_coverage_plugin-3.0.0/README.rst
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/django_coverage_plugin/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      447 2021-11-11 13:57:19.000000 django_coverage_plugin-3.0.0/django_coverage_plugin/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    14248 2022-12-04 17:03:06.000000 django_coverage_plugin-3.0.0/django_coverage_plugin/plugin.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/django_coverage_plugin.egg-info/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     8747 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/django_coverage_plugin.egg-info/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      373 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/django_coverage_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/django_coverage_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/django_coverage_plugin.egg-info/requires.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       23 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/django_coverage_plugin.egg-info/top_level.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      236 2022-12-06 09:56:40.000000 django_coverage_plugin-3.0.0/setup.cfg
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1890 2022-12-06 09:51:44.000000 django_coverage_plugin-3.0.0/setup.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-10 13:14:18.613103 django_coverage_plugin-3.1.0/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      200 2021-05-25 01:35:09.000000 django_coverage_plugin-3.1.0/AUTHORS.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10174 2016-06-02 15:25:30.000000 django_coverage_plugin-3.1.0/LICENSE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      371 2021-06-08 23:05:46.000000 django_coverage_plugin-3.1.0/MANIFEST.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      631 2022-05-04 10:26:03.000000 django_coverage_plugin-3.1.0/NOTICE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     8892 2023-07-10 13:14:18.613473 django_coverage_plugin-3.1.0/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     8614 2023-07-10 13:13:09.000000 django_coverage_plugin-3.1.0/README.rst
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-10 13:14:18.607009 django_coverage_plugin-3.1.0/django_coverage_plugin/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      447 2021-11-11 13:57:19.000000 django_coverage_plugin-3.1.0/django_coverage_plugin/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    14135 2023-07-10 13:11:14.000000 django_coverage_plugin-3.1.0/django_coverage_plugin/plugin.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-10 13:14:18.612641 django_coverage_plugin-3.1.0/django_coverage_plugin.egg-info/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     8892 2023-07-10 13:14:18.000000 django_coverage_plugin-3.1.0/django_coverage_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      373 2023-07-10 13:14:18.000000 django_coverage_plugin-3.1.0/django_coverage_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-07-10 13:14:18.000000 django_coverage_plugin-3.1.0/django_coverage_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        9 2023-07-10 13:14:18.000000 django_coverage_plugin-3.1.0/django_coverage_plugin.egg-info/requires.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       23 2023-07-10 13:14:18.000000 django_coverage_plugin-3.1.0/django_coverage_plugin.egg-info/top_level.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      236 2023-07-10 13:14:18.614614 django_coverage_plugin-3.1.0/setup.cfg
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1891 2023-07-10 13:11:46.000000 django_coverage_plugin-3.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django_coverage_plugin-3.0.0/LICENSE.txt` & `django_coverage_plugin-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_coverage_plugin-3.0.0/NOTICE.txt` & `django_coverage_plugin-3.1.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `django_coverage_plugin-3.0.0/PKG-INFO` & `django_coverage_plugin-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: django_coverage_plugin
-Version: 3.0.0
+Version: 3.1.0
 Summary: Django template coverage.py plugin
 Home-page: https://github.com/nedbat/django_coverage_plugin
 Author: Ned Batchelder
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 License-File: AUTHORS.txt
 
 ==================================
 Django Template Coverage.py Plugin
@@ -36,23 +36,23 @@
 
 A `coverage.py`_ plugin to measure test coverage of Django templates.
 
 
 
 Supported on:
 
-- Python: 3.7 through 3.11.
+- Python: 3.8 through 3.12.
 
-- Django: 1.11, 2.x, 3.x and 4.x.
+- Django: 2.x, 3.x and 4.x.
 
-- Coverage.py: 4.x or higher.
+- Coverage.py: 6.x or higher.
 
 The plugin is pip installable::
 
-    $ pip install django_coverage_plugin
+    $ python3 -m pip install django_coverage_plugin
 
 To run it, add this setting to your ``.coveragerc`` file::
 
     [run]
     plugins = django_coverage_plugin
 
 Then run your tests under `coverage.py`_.
@@ -133,34 +133,42 @@
 
 
 Tests
 ~~~~~
 
 To run the tests::
 
-    $ pip install -r requirements.txt
+    $ python3 -m pip install -r requirements.txt
     $ tox
 
 
 History
 ~~~~~~~
 
 .. scriv-insert-here
 
+v3.1.0 — 2023-07-10
+-------------------
+
+Dropped support for Python 3.7 and Django 1.x.  Declared support for Python
+3.12.
+
+
 v3.0.0 — 2022-12-06
 -------------------
 
 Dropped support for Python 2.7, Python 3.6, and Django 1.8.
 
 
 v2.0.4 — 2022-10-31
 -------------------
 
 Declare our support for Python 3.11 and Django 4.1.
 
+
 v2.0.3 — 2022-05-04
 -------------------
 
 Add support for Django 4.0.
 
 
 v2.0.2 — 2021-11-11
```

### Comparing `django_coverage_plugin-3.0.0/README.rst` & `django_coverage_plugin-3.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 
 ------------------
 
 .. end-badges
 
 Supported on:
 
-- Python: 3.7 through 3.11.
+- Python: 3.8 through 3.12.
 
-- Django: 1.11, 2.x, 3.x and 4.x.
+- Django: 2.x, 3.x and 4.x.
 
-- Coverage.py: 4.x or higher.
+- Coverage.py: 6.x or higher.
 
 The plugin is pip installable::
 
-    $ pip install django_coverage_plugin
+    $ python3 -m pip install django_coverage_plugin
 
 To run it, add this setting to your ``.coveragerc`` file::
 
     [run]
     plugins = django_coverage_plugin
 
 Then run your tests under `coverage.py`_.
@@ -124,34 +124,42 @@
 
 
 Tests
 ~~~~~
 
 To run the tests::
 
-    $ pip install -r requirements.txt
+    $ python3 -m pip install -r requirements.txt
     $ tox
 
 
 History
 ~~~~~~~
 
 .. scriv-insert-here
 
+v3.1.0 — 2023-07-10
+-------------------
+
+Dropped support for Python 3.7 and Django 1.x.  Declared support for Python
+3.12.
+
+
 v3.0.0 — 2022-12-06
 -------------------
 
 Dropped support for Python 2.7, Python 3.6, and Django 1.8.
 
 
 v2.0.4 — 2022-10-31
 -------------------
 
 Declare our support for Python 3.11 and Django 4.1.
 
+
 v2.0.3 — 2022-05-04
 -------------------
 
 Add support for Django 4.0.
 
 
 v2.0.2 — 2021-11-11
```

### Comparing `django_coverage_plugin-3.0.0/django_coverage_plugin/plugin.py` & `django_coverage_plugin-3.1.0/django_coverage_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             raise DjangoTemplatePluginException(
                 "Template debugging must be enabled in settings."
             )
 
     return True
 
 
-if django.VERSION < (1, 11):
-    raise RuntimeError("Django Coverage Plugin requires Django 1.11 or higher")
+if django.VERSION < (2, 0):
+    raise RuntimeError("Django Coverage Plugin requires Django 2.x or higher")
 
 
 # Since we are grabbing at internal details, we have to adapt as they
 # change over versions.
 def filename_for_frame(frame):
     try:
         return frame.f_locals["self"].origin.name
@@ -308,18 +308,15 @@
 
     def lines(self):
         source_lines = set()
 
         if SHOW_PARSING:
             print(f"-------------- {self.filename}")
 
-        if django.VERSION >= (1, 9):
-            lexer = Lexer(self.source())
-        else:
-            lexer = Lexer(self.source(), self.filename)
+        lexer = Lexer(self.source())
         tokens = lexer.tokenize()
 
         # Are we inside a comment?
         comment = False
         # Is this a template that extends another template?
         extends = False
         # Are we inside a block?
```

### Comparing `django_coverage_plugin-3.0.0/django_coverage_plugin.egg-info/PKG-INFO` & `django_coverage_plugin-3.1.0/django_coverage_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: django-coverage-plugin
-Version: 3.0.0
+Version: 3.1.0
 Summary: Django template coverage.py plugin
 Home-page: https://github.com/nedbat/django_coverage_plugin
 Author: Ned Batchelder
 Author-email: ned@nedbatchelder.com
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 License-File: AUTHORS.txt
 
 ==================================
 Django Template Coverage.py Plugin
@@ -36,23 +36,23 @@
 
 A `coverage.py`_ plugin to measure test coverage of Django templates.
 
 
 
 Supported on:
 
-- Python: 3.7 through 3.11.
+- Python: 3.8 through 3.12.
 
-- Django: 1.11, 2.x, 3.x and 4.x.
+- Django: 2.x, 3.x and 4.x.
 
-- Coverage.py: 4.x or higher.
+- Coverage.py: 6.x or higher.
 
 The plugin is pip installable::
 
-    $ pip install django_coverage_plugin
+    $ python3 -m pip install django_coverage_plugin
 
 To run it, add this setting to your ``.coveragerc`` file::
 
     [run]
     plugins = django_coverage_plugin
 
 Then run your tests under `coverage.py`_.
@@ -133,34 +133,42 @@
 
 
 Tests
 ~~~~~
 
 To run the tests::
 
-    $ pip install -r requirements.txt
+    $ python3 -m pip install -r requirements.txt
     $ tox
 
 
 History
 ~~~~~~~
 
 .. scriv-insert-here
 
+v3.1.0 — 2023-07-10
+-------------------
+
+Dropped support for Python 3.7 and Django 1.x.  Declared support for Python
+3.12.
+
+
 v3.0.0 — 2022-12-06
 -------------------
 
 Dropped support for Python 2.7, Python 3.6, and Django 1.8.
 
 
 v2.0.4 — 2022-10-31
 -------------------
 
 Declare our support for Python 3.11 and Django 4.1.
 
+
 v2.0.3 — 2022-05-04
 -------------------
 
 Add support for Django 4.0.
 
 
 v2.0.2 — 2021-11-11
```

### Comparing `django_coverage_plugin-3.0.0/setup.py` & `django_coverage_plugin-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 
 
 classifiers = """\
 Environment :: Console
 Intended Audience :: Developers
 License :: OSI Approved :: Apache Software License
 Operating System :: OS Independent
-Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3.11
+Programming Language :: Python :: 3.12
 Programming Language :: Python :: Implementation :: CPython
 Programming Language :: Python :: Implementation :: PyPy
 Topic :: Software Development :: Quality Assurance
 Topic :: Software Development :: Testing
 Development Status :: 5 - Production/Stable
 Framework :: Django
 Framework :: Django :: 1.11
 Framework :: Django :: 2.2
 Framework :: Django :: 3.2
-Framework :: Django :: 4.1
+Framework :: Django :: 4.2
 """
 
 setup(
     name='django_coverage_plugin',
-    version='3.0.0',
+    version='3.1.0',
     description='Django template coverage.py plugin',
     long_description=(
         re.sub(
             '(?ms)^.. start-badges.*^.. end-badges',
             '',
             read('README.rst'),
         )
```

