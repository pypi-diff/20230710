# Comparing `tmp/confme-2.0.0.tar.gz` & `tmp/confme-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confme-2.0.0.tar", max compression
+gzip compressed data, was "confme-2.0.1.tar", max compression
```

## Comparing `confme-2.0.0.tar` & `confme-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1085 2023-07-10 14:20:04.523162 confme-2.0.0/LICENSE
--rw-r--r--   0        0        0     9849 2023-07-10 14:20:04.523162 confme-2.0.0/README.md
--rw-r--r--   0        0        0      173 2023-07-10 14:20:04.523162 confme-2.0.0/confme/__init__.py
--rw-r--r--   0        0        0      746 2023-07-10 14:20:04.523162 confme-2.0.0/confme/annotation.py
--rw-r--r--   0        0        0        0 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/__init__.py
--rw-r--r--   0        0        0     1091 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/argument_overwrite.py
--rw-r--r--   0        0        0     6814 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/base_config.py
--rw-r--r--   0        0        0      743 2023-07-10 14:20:04.523162 confme-2.0.0/confme/core/env_overwrite.py
--rw-r--r--   0        0        0    18170 2023-07-10 14:20:04.523162 confme-2.0.0/confme/pylintrc
--rw-r--r--   0        0        0      841 2023-07-10 14:20:04.523162 confme-2.0.0/confme/source_backend/__init__.py
--rw-r--r--   0        0        0      728 2023-07-10 14:20:04.523162 confme-2.0.0/confme/source_backend/backend_base.py
--rw-r--r--   0        0        0      847 2023-07-10 14:20:04.523162 confme-2.0.0/confme/source_backend/backend_yaml.py
--rw-r--r--   0        0        0        0 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/base_exception.py
--rw-r--r--   0        0        0      974 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/deprecated.py
--rw-r--r--   0        0        0     1099 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/dict_util.py
--rw-r--r--   0        0        0      763 2023-07-10 14:20:04.523162 confme-2.0.0/confme/utils/typing.py
--rw-r--r--   0        0        0     1353 2023-07-10 14:20:04.523162 confme-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    11100 1970-01-01 00:00:00.000000 confme-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-10 15:13:03.547559 confme-2.0.1/LICENSE
+-rw-r--r--   0        0        0     9849 2023-07-10 15:13:03.547559 confme-2.0.1/README.md
+-rw-r--r--   0        0        0      173 2023-07-10 15:13:03.547559 confme-2.0.1/confme/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-10 15:13:03.547559 confme-2.0.1/confme/annotation.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:13:03.547559 confme-2.0.1/confme/core/__init__.py
+-rw-r--r--   0        0        0     1091 2023-07-10 15:13:03.547559 confme-2.0.1/confme/core/argument_overwrite.py
+-rw-r--r--   0        0        0     6814 2023-07-10 15:13:03.547559 confme-2.0.1/confme/core/base_config.py
+-rw-r--r--   0        0        0      743 2023-07-10 15:13:03.547559 confme-2.0.1/confme/core/env_overwrite.py
+-rw-r--r--   0        0        0    18170 2023-07-10 15:13:03.547559 confme-2.0.1/confme/pylintrc
+-rw-r--r--   0        0        0      841 2023-07-10 15:13:03.547559 confme-2.0.1/confme/source_backend/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-10 15:13:03.547559 confme-2.0.1/confme/source_backend/backend_base.py
+-rw-r--r--   0        0        0      847 2023-07-10 15:13:03.547559 confme-2.0.1/confme/source_backend/backend_yaml.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:13:03.547559 confme-2.0.1/confme/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-10 15:13:03.547559 confme-2.0.1/confme/utils/base_exception.py
+-rw-r--r--   0        0        0      974 2023-07-10 15:13:03.547559 confme-2.0.1/confme/utils/deprecated.py
+-rw-r--r--   0        0        0     1099 2023-07-10 15:13:03.547559 confme-2.0.1/confme/utils/dict_util.py
+-rw-r--r--   0        0        0      763 2023-07-10 15:13:03.547559 confme-2.0.1/confme/utils/typing.py
+-rw-r--r--   0        0        0     1355 2023-07-10 15:13:03.547559 confme-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11088 1970-01-01 00:00:00.000000 confme-2.0.1/PKG-INFO
```

### Comparing `confme-2.0.0/LICENSE` & `confme-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/README.md` & `confme-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/annotation.py` & `confme-2.0.1/confme/annotation.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/core/argument_overwrite.py` & `confme-2.0.1/confme/core/argument_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/core/base_config.py` & `confme-2.0.1/confme/core/base_config.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/core/env_overwrite.py` & `confme-2.0.1/confme/core/env_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/pylintrc` & `confme-2.0.1/confme/pylintrc`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/source_backend/__init__.py` & `confme-2.0.1/confme/source_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/source_backend/backend_base.py` & `confme-2.0.1/confme/source_backend/backend_base.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/source_backend/backend_yaml.py` & `confme-2.0.1/confme/source_backend/backend_yaml.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/utils/deprecated.py` & `confme-2.0.1/confme/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/utils/dict_util.py` & `confme-2.0.1/confme/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/confme/utils/typing.py` & `confme-2.0.1/confme/utils/typing.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.0/pyproject.toml` & `confme-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confme"
-version = "2.0.0"
+version = "2.0.1"
 description = "Easy configuration management in python"
 authors = ["Iwan Silvan Bolzern <iwan.bolzern@roche.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/iwanbolzern/confme"
 repository = "https://github.com/iwanbolzern/confme"
 classifiers = [
@@ -26,17 +26,17 @@
 packages = [
     { include = "confme" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
-pyyaml = "^5.3"
+pyyaml = ">=5.3"
 pydantic = "^2.0"
-tabulate = "^0.8.9"
+tabulate = ">=0.8.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1.2"
 pylint = "^2.17.4"
 sphinx = "^3.2.1"
 recommonmark = "^0.6.0"
 pytest-cov = "^2.11.1"
```

### Comparing `confme-2.0.0/PKG-INFO` & `confme-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confme
-Version: 2.0.0
+Version: 2.0.1
 Summary: Easy configuration management in python
 Home-page: https://github.com/iwanbolzern/confme
 License: LICENSE
 Author: Iwan Silvan Bolzern
 Author-email: iwan.bolzern@roche.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pydantic (>=2.0,<3.0)
-Requires-Dist: pyyaml (>=5.3,<6.0)
-Requires-Dist: tabulate (>=0.8.9,<0.9.0)
+Requires-Dist: pyyaml (>=5.3)
+Requires-Dist: tabulate (>=0.8.9)
 Project-URL: Repository, https://github.com/iwanbolzern/confme
 Description-Content-Type: text/markdown
 
 # ConfMe: Configuration Made Easy 💖
 
 [![image](https://img.shields.io/pypi/v/confme?color=blue)](https://pypi.org/project/confme/) [![image](https://img.shields.io/pypi/l/confme)](https://pypi.org/project/confme/) [![image](https://github.com/iwanbolzern/ConfMe/workflows/Test/badge.svg?branch=master)](https://pypi.org/project/confme/)
 [![image](https://img.shields.io/pypi/pyversions/confme?color=blue)](https://pypi.org/project/confme/)
```

