# Comparing `tmp/cmem_plugin_number_conversion-0.5.2.tar.gz` & `tmp/cmem_plugin_number_conversion-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_number_conversion-0.5.2.tar", max compression
+gzip compressed data, was "cmem_plugin_number_conversion-0.6.0.tar", max compression
```

## Comparing `cmem_plugin_number_conversion-0.5.2.tar` & `cmem_plugin_number_conversion-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11334 2023-01-09 10:10:56.681827 cmem_plugin_number_conversion-0.5.2/LICENSE
--rw-r--r--   0        0        0      399 2023-01-09 10:10:56.681827 cmem_plugin_number_conversion-0.5.2/README-public.md
--rw-r--r--   0        0        0        0 2023-01-09 10:10:56.681827 cmem_plugin_number_conversion-0.5.2/cmem_plugin_number_conversion/__init__.py
--rw-r--r--   0        0        0     2819 2023-01-09 10:10:56.681827 cmem_plugin_number_conversion-0.5.2/cmem_plugin_number_conversion/transform/__init__.py
--rw-r--r--   0        0        0     1663 2023-01-09 10:11:30.061411 cmem_plugin_number_conversion-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 cmem_plugin_number_conversion-0.5.2/setup.py
--rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 cmem_plugin_number_conversion-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-10 12:08:56.002825 cmem_plugin_number_conversion-0.6.0/LICENSE
+-rw-r--r--   0        0        0      396 2023-07-10 12:08:56.002825 cmem_plugin_number_conversion-0.6.0/README-public.md
+-rw-r--r--   0        0        0        0 2023-07-10 12:08:56.002825 cmem_plugin_number_conversion-0.6.0/cmem_plugin_number_conversion/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-10 12:08:56.002825 cmem_plugin_number_conversion-0.6.0/cmem_plugin_number_conversion/transform/__init__.py
+-rw-r--r--   0        0        0     1683 2023-07-10 12:09:20.287191 cmem_plugin_number_conversion-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 cmem_plugin_number_conversion-0.6.0/PKG-INFO
```

### Comparing `cmem_plugin_number_conversion-0.5.2/LICENSE` & `cmem_plugin_number_conversion-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_number_conversion-0.5.2/cmem_plugin_number_conversion/transform/__init__.py` & `cmem_plugin_number_conversion-0.6.0/cmem_plugin_number_conversion/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_number_conversion-0.5.2/pyproject.toml` & `cmem_plugin_number_conversion-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [tool.poetry]
 name = "cmem-plugin-number-conversion"
-version = "0.5.2"
+version = "0.6.0"
 license = "Apache-2.0"
-description = "Convert numbers between different number bases (binary, octal, decimal, hexadecimal)."
+description = "Convert numbers between binary, octal, decimal and hexadecimal representation."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugin", "number-conversion"
 ]
 homepage = "https://github.com/eccenca/cmem-plugin-number-conversion"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-plugin-base = "^2.1.0"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.0"
-pytest-cov = "^4.0.0"
-pytest-memray = "^1.3.0"
-black = "^22.1.0"
-bandit = "^1.7.2"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.3"
+defusedxml = "^0.7.1"
+flake8-formatter-junit-xml = "^0.0.6"
+genbadge = "^1.1.0"
+mypy = "^1.2.0"
+pillow = "^9.5.0"
 pylint-junit = "^0.3.2"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-memray = "^1.4.0"
 safety = "^1.10.3"
-genbadge = "^1.0.6"
-flake8-formatter-junit-xml = "^0.0.6"
-typed-ast = "^1.5.2"
-mypy = "^0.991"
-coverage = "^6.3.2"
-defusedxml = "^0.7.1"
-wheel = "^0.38.3"
+typed-ast = "^1.5.4"
+wheel = "^0.38.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `cmem_plugin_number_conversion-0.5.2/PKG-INFO` & `cmem_plugin_number_conversion-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-number-conversion
-Version: 0.5.2
-Summary: Convert numbers between different number bases (binary, octal, decimal, hexadecimal).
+Version: 0.6.0
+Summary: Convert numbers between binary, octal, decimal and hexadecimal representation.
 Home-page: https://github.com/eccenca/cmem-plugin-number-conversion
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,number-conversion
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-plugin-base (>=2.1.0,<3.0.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-number-conversion
 
-Transform plugin allows users to easily convert numbers from one base to another.
+Convert numbers between binary, octal, decimal and hexadecimal representation.
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
 
 You can install it with the [cmemc](https://eccenca.com/go/cmemc) command line
 clients like this:
 
 ```
```

