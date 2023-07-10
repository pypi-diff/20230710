# Comparing `tmp/katalytic-0.2.1.tar.gz` & `tmp/katalytic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic-0.2.2.tar", last modified: Mon Jul 10 20:46:26 2023, max compression
```

## Comparing `katalytic-0.2.1.tar` & `katalytic-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,19 @@
--rw-r--r--   0        0        0       78 2023-07-09 19:30:05.161864 katalytic-0.2.1/.coveragerc
--rw-r--r--   0        0        0      651 2023-07-09 19:30:05.161864 katalytic-0.2.1/.gitignore
--rw-r--r--   0        0        0     3256 2023-07-09 19:30:05.161864 katalytic-0.2.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     1695 2023-07-10 05:24:54.879388 katalytic-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     5489 2023-07-09 19:30:05.161864 katalytic-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-07-09 19:30:05.161864 katalytic-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     4412 2023-07-10 04:57:34.292819 katalytic-0.2.1/README.md
--rw-r--r--   0        0        0     1478 2023-07-10 05:24:54.875388 katalytic-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6373 2023-07-10 05:16:15.778535 katalytic-0.2.1/src/katalytic/_pkg/__init__.py
--rw-r--r--   0        0        0    58606 2023-07-09 19:30:05.161864 katalytic-0.2.1/src/katalytic/data/__init__.py
--rw-r--r--   0        0        0    22696 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/data/checks.py
--rw-r--r--   0        0        0    51483 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/files/__init__.py
--rw-r--r--   0        0        0      130 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/katalytic.py
--rw-r--r--   0        0        0     5838 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/maths/__init__.py
--rw-r--r--   0        0        0    22812 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/maths/bboxes.py
--rw-r--r--   0        0        0     4238 2023-07-09 19:30:05.165864 katalytic-0.2.1/src/katalytic/meta/__init__.py
--rw-r--r--   0        0        0    13200 2023-07-09 19:30:05.165864 katalytic-0.2.1/tests/test_bboxes.py
--rw-r--r--   0        0        0    19288 2023-07-09 19:30:05.165864 katalytic-0.2.1/tests/test_checks.py
--rw-r--r--   0        0        0    52443 2023-07-09 19:30:05.165864 katalytic-0.2.1/tests/test_data.py
--rw-r--r--   0        0        0    67110 2023-07-10 05:03:00.709365 katalytic-0.2.1/tests/test_files.py
--rw-r--r--   0        0        0     3868 2023-07-09 19:30:05.169864 katalytic-0.2.1/tests/test_maths.py
--rw-r--r--   0        0        0     3054 2023-07-09 19:30:05.169864 katalytic-0.2.1/tests/test_meta.py
--rw-r--r--   0        0        0     2945 2023-07-10 05:07:24.285719 katalytic-0.2.1/tests/test_pkg.py
--rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 katalytic-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-09 19:30:05.161864 katalytic-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     4412 2023-07-10 04:57:34.292819 katalytic-0.2.2/README.md
+-rw-r--r--   0        0        0     1478 2023-07-10 20:46:26.693366 katalytic-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7097 2023-07-10 20:28:25.612937 katalytic-0.2.2/src/katalytic/_pkg/__init__.py
+-rw-r--r--   0        0        0    58606 2023-07-09 19:30:05.161864 katalytic-0.2.2/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0    22696 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    51483 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/files/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/katalytic.py
+-rw-r--r--   0        0        0     5838 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/maths/__init__.py
+-rw-r--r--   0        0        0    22812 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/maths/bboxes.py
+-rw-r--r--   0        0        0     4238 2023-07-09 19:30:05.165864 katalytic-0.2.2/src/katalytic/meta/__init__.py
+-rw-r--r--   0        0        0    13200 2023-07-09 19:30:05.165864 katalytic-0.2.2/tests/test_bboxes.py
+-rw-r--r--   0        0        0    19288 2023-07-09 19:30:05.165864 katalytic-0.2.2/tests/test_checks.py
+-rw-r--r--   0        0        0    52443 2023-07-09 19:30:05.165864 katalytic-0.2.2/tests/test_data.py
+-rw-r--r--   0        0        0    67110 2023-07-10 05:03:00.709365 katalytic-0.2.2/tests/test_files.py
+-rw-r--r--   0        0        0     3868 2023-07-09 19:30:05.169864 katalytic-0.2.2/tests/test_maths.py
+-rw-r--r--   0        0        0     3054 2023-07-10 18:15:32.788541 katalytic-0.2.2/tests/test_meta.py
+-rw-r--r--   0        0        0     2957 2023-07-10 18:19:12.880623 katalytic-0.2.2/tests/test_pkg.py
+-rw-r--r--   0        0        0     6873 1970-01-01 00:00:00.000000 katalytic-0.2.2/PKG-INFO
```

### Comparing `katalytic-0.2.1/LICENSE.txt` & `katalytic-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/README.md` & `katalytic-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/pyproject.toml` & `katalytic-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[tool.pdm.build]
+includes = [
+    "src/katalytic/",
+]
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
 
 [project]
 name = "katalytic"
-version = "0.2.1"
+version = "0.2.2"
 description = "We'll take care of the boilerplate, so you can focus on your problems."
-license = {file = "LICENSE.txt"}
 readme = "README.md"
-
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
@@ -24,18 +34,23 @@
     "Topic :: Utilities",
 ]
 keywords = [
     "automation",
     "high-level",
     "metaprogramming",
 ]
-authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
+authors = [
+    { name = "Valentin Neagu", email = "vali19th@protonmail.com" },
+]
 requires-python = ">=3.6"
 dependencies = []
 
+[project.license]
+file = "LICENSE.txt"
+
 [project.optional-dependencies]
 all = [
     "katalytic-images>=0.1.0",
 ]
 dev = [
     "pytest",
     "pytest-cov",
@@ -43,14 +58,7 @@
     "pytest-randomly",
 ]
 
 [project.urls]
 Changelog = "https://gitlab.com/katalytic/katalytic/-/blob/main/CHANGELOG.md"
 Homepage = "https://gitlab.com/katalytic/katalytic.git"
 Repository = "https://gitlab.com/katalytic/katalytic.git"
-# Documentation = "TODO"
-
-[tool.pytest.ini_options]
-addopts = ["--import-mode=importlib"]
-
-[tool.flit.module]
-name = "katalytic.katalytic"
```

### Comparing `katalytic-0.2.1/src/katalytic/_pkg/__init__.py` & `katalytic-0.2.2/src/katalytic/_pkg/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,37 +56,40 @@
 
     """
     if sys.version_info >= (3, 8):
         from importlib import metadata
         dunder_name = dunder_name.replace('.', '-')
         dunder_name = dunder_name.replace('-__init__', '')
         version = metadata.version(dunder_name)
-        version_info = tuple(map(int, version.split('.')))
+
+        version_info = version.replace('+editable', '').split('.')
+        version_info = tuple(map(int, version_info))
+        if '+editable' in version:
+            version_info = (*version_info, 'editable')
+
         return version, version_info
 
     version = None
     for p in __find_paths(dunder_name):
         if p.endswith('.dist-info'):
             version = re.search(r'\w+-(\d+\.\d+\.\d+)', p)
             if version:
                 version = version.group(1)
                 break
 
-        if p.endswith('.dist-info/METADATA'):
-            version = __get_version_from_metadata(p)
-            if version:
-                break
-
-        if p.endswith('.egg-info/PKG-INFO'):
+        if p.endswith('.dist-info/METADATA') or p.endswith('.egg-info/PKG-INFO'):
             version = __get_version_from_metadata(p)
             if version:
                 break
 
     if version:
-        version_info = tuple(map(int, version.split('.')))
+        version_info = version.replace('+editable', '').split('.')
+        version_info = tuple(map(int, version_info))
+        if '+editable' in version:
+            version_info = (*version_info, 'editable')
     else:
         version_info = None
 
     # If nothing worked, I would rather return None than raise an exception
     # This could happen if the package is installed on python < 3.8
     return version, version_info
 
@@ -117,36 +120,44 @@
         if item.stem == '__pycache__':
             continue
 
         base_package = __package__.replace('._pkg', '')
         module_name = f'{base_package}.{item.stem}'
         try:
             module = import_module(module_name)
+            modules.append(module)
         except Exception as e:  # pragma: no cover
             warnings.warn(f'Couldn\'t import {module_name!r}\n' + _get_stacktrace(e))
-            continue
 
-        modules.append(module)
+    modules.extend(_find_editable_installs())
+    return sorted(modules, key=lambda m: m.__name__)
+
+
+def _find_editable_installs():
+    env_lib = re.sub(r'/bin/python', '/lib/', sys.executable)
+    for item in Path(env_lib).glob('python*/site-packages/katalytic_*.pth'):  # pragma: no cover
+        # no coverage: because I would have to create an editable install,
+        # just to test this functionality
+        try:
+            module = import_module(item.stem.replace('_', '.'))
+            yield module
+        except Exception as e:  # pragma: no cover
+            warnings.warn(f'Couldn\'t import {item.stem!r}\n' + _get_stacktrace(e))
 
-    # find editable installs
     for item in Path(__file__).parent.parent.parent.iterdir():  # pragma: no cover
         # no coverage: because I would have to create an editable install,
         # just to test this functionality
-        if not re.search(__package__ + r'\..*\.pth', item.name):
+        if not re.search(r'katalytic_\w+.pth', item.name):
             continue
 
         try:
-            module = import_module(item.stem)
+            module = import_module(item.stem.replace('_', '.'))
+            yield module
         except Exception as e:  # pragma: no cover
             warnings.warn(f'Couldn\'t import {item.stem!r}\n' + _get_stacktrace(e))
-            continue
-
-        modules.append(module)
-
-    return sorted(modules, key=lambda m: m.__name__)
 
 
 def find_functions_marked_with(group):
     """
     Get a list of functions within the package that belong to a specific group.
 
     Args:
```

### Comparing `katalytic-0.2.1/src/katalytic/data/__init__.py` & `katalytic-0.2.2/src/katalytic/data/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/src/katalytic/data/checks.py` & `katalytic-0.2.2/src/katalytic/data/checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/src/katalytic/files/__init__.py` & `katalytic-0.2.2/src/katalytic/files/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/src/katalytic/maths/__init__.py` & `katalytic-0.2.2/src/katalytic/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/src/katalytic/maths/bboxes.py` & `katalytic-0.2.2/src/katalytic/maths/bboxes.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/src/katalytic/meta/__init__.py` & `katalytic-0.2.2/src/katalytic/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/tests/test_bboxes.py` & `katalytic-0.2.2/tests/test_bboxes.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/tests/test_checks.py` & `katalytic-0.2.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/tests/test_data.py` & `katalytic-0.2.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/tests/test_files.py` & `katalytic-0.2.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/tests/test_maths.py` & `katalytic-0.2.2/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/tests/test_meta.py` & `katalytic-0.2.2/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `katalytic-0.2.1/tests/test_pkg.py` & `katalytic-0.2.2/tests/test_pkg.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,12 +81,13 @@
         assert all(m.startswith('katalytic') for m in modules)
 
 
 class Test_version:
     def test_is_ok(self):
         v, v_info = get_version('katalytic')
 
-        assert __version__ is not None
         assert v is not None
         assert v_info is not None
-        assert v == '.'.join(str(i) for i in v_info)
         assert v == __version__
+
+        v2 = v.replace('+editable', '.editable')
+        assert v2 == '.'.join(str(i) for i in v_info)
```

### Comparing `katalytic-0.2.1/PKG-INFO` & `katalytic-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 Metadata-Version: 2.1
 Name: katalytic
-Version: 0.2.1
+Version: 0.2.2
 Summary: We'll take care of the boilerplate, so you can focus on your problems.
-Keywords: automation,high-level,metaprogramming
-Author-email: Valentin Neagu <vali19th@protonmail.com>
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Keywords: automation high-level metaprogramming
+Author-Email: Valentin Neagu <vali19th@protonmail.com>
+License: Copyright 2023 - present, Valentin Neagu
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Dist: katalytic-images>=0.1.0 ; extra == "all"
-Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: pytest-cov ; extra == "dev"
-Requires-Dist: pytest-clarity ; extra == "dev"
-Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: Changelog, https://gitlab.com/katalytic/katalytic/-/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://gitlab.com/katalytic/katalytic.git
 Project-URL: Repository, https://gitlab.com/katalytic/katalytic.git
+Requires-Python: >=3.6
 Provides-Extra: all
 Provides-Extra: dev
+Requires-Dist: katalytic-images>=0.1.0; extra == "all"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-clarity; extra == "dev"
+Requires-Dist: pytest-randomly; extra == "dev"
+Description-Content-Type: text/markdown
 
 # katalytic [![version](https://img.shields.io/pypi/v/katalytic)](https://pypi.org/project/katalytic/) [![tests](https://gitlab.com/katalytic/katalytic/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![coverage](https://gitlab.com/katalytic/katalytic/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic/-/commits/main) [![docs](https://img.shields.io/readthedocs/katalytic.svg)](https://katalytic.readthedocs.io/en/latest/) [![license: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
 
 **Don't use in production yet.**
 I will likely tweak the function names and the default behaviour a few more times.
 
 We'll take care of the boilerplate, so you can **focus on your problems.**
@@ -149,8 +156,7 @@
 ## Contributing
 We appreciate any form of contribution, including but not limited to:
 - **Code contributions**: Enhance our repository with your code and tests.
 - **Feature suggestions**: Your ideas can shape the future development of our package.
 - **Architectural improvements**: Help us optimize our system's design and API.
 - **Bug fixes**: Improve user experience by reporting or resolving issues.
 - **Documentation**: Help us maintain clear and up-to-date instructions for users.
-
```

