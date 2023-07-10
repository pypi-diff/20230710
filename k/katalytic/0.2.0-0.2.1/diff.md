# Comparing `tmp/katalytic-0.2.0.tar.gz` & `tmp/katalytic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic-0.2.0.tar` & `katalytic-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       78 2023-07-09 19:30:05.161864 katalytic-0.2.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-07-09 19:30:05.161864 katalytic-0.2.0/.gitignore
--rw-r--r--   0        0        0     3256 2023-07-09 19:30:05.161864 katalytic-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1513 2023-07-09 19:37:21.597758 katalytic-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     5489 2023-07-09 19:30:05.161864 katalytic-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-07-09 19:30:05.161864 katalytic-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     4416 2023-07-09 19:30:05.161864 katalytic-0.2.0/README.md
--rw-r--r--   0        0        0     1478 2023-07-09 19:37:21.597758 katalytic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6303 2023-07-09 19:30:05.161864 katalytic-0.2.0/src/katalytic/_pkg.py
--rw-r--r--   0        0        0    58606 2023-07-09 19:30:05.161864 katalytic-0.2.0/src/katalytic/data/__init__.py
--rw-r--r--   0        0        0    22696 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/data/checks.py
--rw-r--r--   0        0        0    51483 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/files.py
--rw-r--r--   0        0        0      130 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/katalytic.py
--rw-r--r--   0        0        0     5838 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/maths/__init__.py
--rw-r--r--   0        0        0    22812 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/maths/bboxes.py
--rw-r--r--   0        0        0     4238 2023-07-09 19:30:05.165864 katalytic-0.2.0/src/katalytic/meta.py
--rw-r--r--   0        0        0    13200 2023-07-09 19:30:05.165864 katalytic-0.2.0/tests/test_bboxes.py
--rw-r--r--   0        0        0    19288 2023-07-09 19:30:05.165864 katalytic-0.2.0/tests/test_checks.py
--rw-r--r--   0        0        0    52443 2023-07-09 19:30:05.165864 katalytic-0.2.0/tests/test_data.py
--rw-r--r--   0        0        0    67110 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_files.py
--rw-r--r--   0        0        0     3868 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_maths.py
--rw-r--r--   0        0        0     3054 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_meta.py
--rw-r--r--   0        0        0     2903 2023-07-09 19:30:05.169864 katalytic-0.2.0/tests/test_pkg.py
--rw-r--r--   0        0        0     5761 1970-01-01 00:00:00.000000 katalytic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       78 2023-07-09 19:30:05.161864 katalytic-0.2.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-07-09 19:30:05.161864 katalytic-0.2.1/.gitignore
+-rw-r--r--   0        0        0     3256 2023-07-09 19:30:05.161864 katalytic-0.2.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1695 2023-07-10 05:24:54.879388 katalytic-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5489 2023-07-09 19:30:05.161864 katalytic-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-07-09 19:30:05.161864 katalytic-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     4412 2023-07-10 04:57:34.292819 katalytic-0.2.1/README.md
+-rw-r--r--   0        0        0     1478 2023-07-10 05:24:54.875388 katalytic-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6373 2023-07-10 05:16:15.778535 katalytic-0.2.1/src/katalytic/_pkg/__init__.py
+-rw-r--r--   0        0        0    58606 2023-07-09 19:30:05.161864 katalytic-0.2.1/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0    22696 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    51483 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/files/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/katalytic.py
+-rw-r--r--   0        0        0     5838 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/maths/__init__.py
+-rw-r--r--   0        0        0    22812 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/maths/bboxes.py
+-rw-r--r--   0        0        0     4238 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/meta/__init__.py
+-rw-r--r--   0        0        0    13200 2023-07-09 19:30:05.165864 katalytic-0.2.1/tests/test_bboxes.py
+-rw-r--r--   0        0        0    19288 2023-07-09 19:30:05.165864 katalytic-0.2.1/tests/test_checks.py
+-rw-r--r--   0        0        0    52443 2023-07-09 19:30:05.165864 katalytic-0.2.1/tests/test_data.py
+-rw-r--r--   0        0        0    67110 2023-07-10 05:03:00.709365 katalytic-0.2.1/tests/test_files.py
+-rw-r--r--   0        0        0     3868 2023-07-09 19:30:05.169864 katalytic-0.2.1/tests/test_maths.py
+-rw-r--r--   0        0        0     3054 2023-07-09 19:30:05.169864 katalytic-0.2.1/tests/test_meta.py
+-rw-r--r--   0        0        0     2945 2023-07-10 05:07:24.285719 katalytic-0.2.1/tests/test_pkg.py
+-rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 katalytic-0.2.1/PKG-INFO
```

### Comparing `katalytic-0.2.0/.gitignore` & `katalytic-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/.gitlab-ci.yml` & `katalytic-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/CHANGELOG.md` & `katalytic-0.2.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.2.1 (2023-07-10)
+### fix
+- [[`0db306b`](https://gitlab.com/katalytic/katalytic/commit/0db306b5d83c3cc07a688641a0dbcc88a4f14234)] namespace packages need a different structure
+
+
 ## 0.2.0 (2023-07-09)
 ### feat
 - [[`aab4af6`](https://gitlab.com/katalytic/katalytic/commit/aab4af641604f014ba42b099eab7d1c1da153046)] merge all plugins without 3rd-party dependencies into this package: data, files, maths, pkg
 ### fix
 - [[`f06af0f`](https://gitlab.com/katalytic/katalytic/commit/f06af0f2c3399bb46b1db0d8eb30c94715d81a31)] add katalytic.py back
 - [[`e73a745`](https://gitlab.com/katalytic/katalytic/commit/e73a745b5662154a5c03c44762beca9ab9627296)] merge katalytic-data
 ### docs
```

### Comparing `katalytic-0.2.0/CODE_OF_CONDUCT.md` & `katalytic-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/LICENSE.txt` & `katalytic-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/README.md` & `katalytic-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# katalytic [![version](https://img.shields.io/pypi/v/katalytic)](https://pypi.org/project/katalytic/) [![tests](https://gitlab.com/katalytic/katalytic/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![coverage](https://gitlab.com/katalytic/katalytic/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![docs](https://img.shields.io/readthedocs/katalytic.svg)](https://katalytic.readthedocs.io/en/latest/) [![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+# katalytic [![version](https://img.shields.io/pypi/v/katalytic)](https://pypi.org/project/katalytic/) [![tests](https://gitlab.com/katalytic/katalytic/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![coverage](https://gitlab.com/katalytic/katalytic/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![docs](https://img.shields.io/readthedocs/katalytic.svg)](https://katalytic.readthedocs.io/en/latest/) [![license: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 **Don't use in production yet.**
 I will likely tweak the function names and the default behaviour a few more times.
 
 We'll take care of the boilerplate, so you can **focus on your problems.**
 
 ## Installation
@@ -33,15 +33,15 @@
 
 >>> as_list_of_dicts([['b', 'a'], [1, 2], [3, 4]])
 [{'b': 1, 'a': 2}, {'b': 3, 'a': 4}]
 
 >>> flatten_recursive([1, [2, [3, 4], 5], 6])
 [1, 2, 3, 4, 5, 6]
 ```
- 
+
 ### files
 - Atomic operations
 - Load and save files with a uniform interface
 - Copy, move, and delete files without searching the docs for the right function
 - The functions return the same type as the input (`Path` or `str`)
 - TODO: Link to tocs
 
@@ -83,18 +83,18 @@
 ### metaprogramming
 - Access the functions at any depth of the call stack
 - TODO: Link to tocs
 ```python
     >>> def foo():
     ...     caller = reference_caller_function()
     ...     print(f'{caller.__name__}() called foo()')
-    ... 
+    ...
     >>> def bar():
     ...     foo()
-    ... 
+    ...
     >>> bar()
     bar() called foo()
 ```
 
 ## Roadmap
 - decorators
 - regexes
```

### Comparing `katalytic-0.2.0/pyproject.toml` & `katalytic-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic"
-version = "0.2.0"
+version = "0.2.1"
 description = "We'll take care of the boilerplate, so you can focus on your problems."
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-0.2.0/src/katalytic/_pkg.py` & `katalytic-0.2.1/src/katalytic/_pkg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,14 @@
         version_info = None
 
     # If nothing worked, I would rather return None than raise an exception
     # This could happen if the package is installed on python < 3.8
     return version, version_info
 
 
-# __version__, __version_info__ = get_version(__name__)
-
-
 def _get_stacktrace(e):
     return ''.join(traceback.format_exception(None, e, e.__traceback__))
 
 
 def _check(name, group):
     if group.endswith('*'):
         prefix = group.split('*')[0]
@@ -112,29 +109,30 @@
 
     Returns:
         list:
             A list of importable modules within the package, sorted by module name.
 
     """
     modules = []
-    for item in Path(__file__).parent.iterdir():
+    for item in Path(__file__).parent.parent.iterdir():
         if item.stem == '__pycache__':
             continue
 
-        module_name = f'{__package__}.{item.stem}'
+        base_package = __package__.replace('._pkg', '')
+        module_name = f'{base_package}.{item.stem}'
         try:
             module = import_module(module_name)
         except Exception as e:  # pragma: no cover
             warnings.warn(f'Couldn\'t import {module_name!r}\n' + _get_stacktrace(e))
             continue
 
         modules.append(module)
 
     # find editable installs
-    for item in Path(__file__).parent.parent.iterdir():  # pragma: no cover
+    for item in Path(__file__).parent.parent.parent.iterdir():  # pragma: no cover
         # no coverage: because I would have to create an editable install,
         # just to test this functionality
         if not re.search(__package__ + r'\..*\.pth', item.name):
             continue
 
         try:
             module = import_module(item.stem)
@@ -216,7 +214,8 @@
 @mark('__test_3::a')
 @mark('__test_3::b')
 @mark('__test_2')
 def __test_2(): pass
 
 
 _UNDEFINED = object()
+__version__, __version_info__ = get_version('katalytic')
```

### Comparing `katalytic-0.2.0/src/katalytic/data/__init__.py` & `katalytic-0.2.1/src/katalytic/data/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/src/katalytic/data/checks.py` & `katalytic-0.2.1/src/katalytic/data/checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/src/katalytic/files.py` & `katalytic-0.2.1/src/katalytic/files/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/src/katalytic/maths/__init__.py` & `katalytic-0.2.1/src/katalytic/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/src/katalytic/maths/bboxes.py` & `katalytic-0.2.1/src/katalytic/maths/bboxes.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/src/katalytic/meta.py` & `katalytic-0.2.1/src/katalytic/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/tests/test_bboxes.py` & `katalytic-0.2.1/tests/test_bboxes.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/tests/test_checks.py` & `katalytic-0.2.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/tests/test_data.py` & `katalytic-0.2.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/tests/test_files.py` & `katalytic-0.2.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/tests/test_maths.py` & `katalytic-0.2.1/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/tests/test_meta.py` & `katalytic-0.2.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.0/tests/test_pkg.py` & `katalytic-0.2.1/tests/test_pkg.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,16 +72,17 @@
             ('__test_2', ['__test_2'])
         ]
 
 
 class Test_get_modules:
     def test_all(self):
         modules = get_modules()
-        assert 'katalytic._pkg' in [m.__name__ for m in modules]
-        assert all(m.__name__.startswith('katalytic') for m in modules)
+        modules = [m.__name__.replace('.__init__', '') for m in modules]
+        assert 'katalytic._pkg' in modules
+        assert all(m.startswith('katalytic') for m in modules)
 
 
 class Test_version:
     def test_is_ok(self):
         v, v_info = get_version('katalytic')
 
         assert __version__ is not None
```

### Comparing `katalytic-0.2.0/PKG-INFO` & `katalytic-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic
-Version: 0.2.0
+Version: 0.2.1
 Summary: We'll take care of the boilerplate, so you can focus on your problems.
 Keywords: automation,high-level,metaprogramming
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -25,15 +25,15 @@
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: Changelog, https://gitlab.com/katalytic/katalytic/-/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://gitlab.com/katalytic/katalytic.git
 Project-URL: Repository, https://gitlab.com/katalytic/katalytic.git
 Provides-Extra: all
 Provides-Extra: dev
 
-# katalytic [![version](https://img.shields.io/pypi/v/katalytic)](https://pypi.org/project/katalytic/) [![tests](https://gitlab.com/katalytic/katalytic/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![coverage](https://gitlab.com/katalytic/katalytic/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![docs](https://img.shields.io/readthedocs/katalytic.svg)](https://katalytic.readthedocs.io/en/latest/) [![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+# katalytic [![version](https://img.shields.io/pypi/v/katalytic)](https://pypi.org/project/katalytic/) [![tests](https://gitlab.com/katalytic/katalytic/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![coverage](https://gitlab.com/katalytic/katalytic/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![docs](https://img.shields.io/readthedocs/katalytic.svg)](https://katalytic.readthedocs.io/en/latest/) [![license: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 **Don't use in production yet.**
 I will likely tweak the function names and the default behaviour a few more times.
 
 We'll take care of the boilerplate, so you can **focus on your problems.**
 
 ## Installation
@@ -64,15 +64,15 @@
 
 >>> as_list_of_dicts([['b', 'a'], [1, 2], [3, 4]])
 [{'b': 1, 'a': 2}, {'b': 3, 'a': 4}]
 
 >>> flatten_recursive([1, [2, [3, 4], 5], 6])
 [1, 2, 3, 4, 5, 6]
 ```
- 
+
 ### files
 - Atomic operations
 - Load and save files with a uniform interface
 - Copy, move, and delete files without searching the docs for the right function
 - The functions return the same type as the input (`Path` or `str`)
 - TODO: Link to tocs
 
@@ -114,18 +114,18 @@
 ### metaprogramming
 - Access the functions at any depth of the call stack
 - TODO: Link to tocs
 ```python
     >>> def foo():
     ...     caller = reference_caller_function()
     ...     print(f'{caller.__name__}() called foo()')
-    ... 
+    ...
     >>> def bar():
     ...     foo()
-    ... 
+    ...
     >>> bar()
     bar() called foo()
 ```
 
 ## Roadmap
 - decorators
 - regexes
```

