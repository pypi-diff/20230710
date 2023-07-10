# Comparing `tmp/cmem_plugin_examples-0.2.0.tar.gz` & `tmp/cmem_plugin_examples-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_examples-0.2.0.tar", max compression
+gzip compressed data, was "cmem_plugin_examples-0.3.0.tar", max compression
```

## Comparing `cmem_plugin_examples-0.2.0.tar` & `cmem_plugin_examples-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11334 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/LICENSE
--rw-r--r--   0        0        0      345 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/README-public.md
--rw-r--r--   0        0        0       55 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/transform/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/transform/lifetime.py
--rw-r--r--   0        0        0        0 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/__init__.py
--rw-r--r--   0        0        0      580 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/minimal.py
--rw-r--r--   0        0        0     5422 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/random_values.py
--rw-r--r--   0        0        0     1239 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/sleep.py
--rw-r--r--   0        0        0     2197 2023-03-13 14:16:24.471413 cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/user.py
--rw-r--r--   0        0        0     1617 2023-03-13 14:20:39.712904 cmem_plugin_examples-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 cmem_plugin_examples-0.2.0/setup.py
--rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 cmem_plugin_examples-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/LICENSE
+-rw-r--r--   0        0        0      345 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/README-public.md
+-rw-r--r--   0        0        0       55 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/transform/__init__.py
+-rw-r--r--   0        0        0     2296 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/transform/lifetime.py
+-rw-r--r--   0        0        0        0 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/__init__.py
+-rw-r--r--   0        0        0      580 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/minimal.py
+-rw-r--r--   0        0        0     5422 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/random_values.py
+-rw-r--r--   0        0        0     1239 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/sleep.py
+-rw-r--r--   0        0        0     2197 2023-07-10 07:48:25.839064 cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/user.py
+-rw-r--r--   0        0        0     1636 2023-07-10 07:59:34.430791 cmem_plugin_examples-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 cmem_plugin_examples-0.3.0/PKG-INFO
```

### Comparing `cmem_plugin_examples-0.2.0/LICENSE` & `cmem_plugin_examples-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_examples-0.2.0/cmem_plugin_examples/transform/lifetime.py` & `cmem_plugin_examples-0.3.0/cmem_plugin_examples/transform/lifetime.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/minimal.py` & `cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/minimal.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/random_values.py` & `cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/random_values.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/sleep.py` & `cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/sleep.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_examples-0.2.0/cmem_plugin_examples/workflow/user.py` & `cmem_plugin_examples-0.3.0/cmem_plugin_examples/workflow/user.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_examples-0.2.0/pyproject.toml` & `cmem_plugin_examples-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-examples"
-version = "0.2.0"
+version = "0.3.0"
 license = "Apache-2.0"
 description = "Example plugins for eccenca Corporate Memory."
 authors = ["eccenca <cmempy-developer@eccenca.com>"]
 maintainers = [
     "Sebastian Tramp <sebastian.tramp@eccenca.com>"
 ]
 classifiers = [
@@ -15,27 +15,28 @@
 readme = "README-public.md"
 keywords = [
     "eccenca Corporate Memory", "plugins", "DataIntegration"
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
-cmem-plugin-base = "^3.0.0"
+python = "^3.11"
+cmem-plugin-base = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
-black = "^23.1.0"
-coverage = "^7.2.1"
+black = "^23.3.0"
+coverage = "^7.2.3"
 defusedxml = "^0.7.1"
 flake8-formatter-junit-xml = "^0.0.6"
 genbadge = "^1.1.0"
-mypy = "^1.1.1"
+mypy = "^1.2.0"
+pillow = "^9.5.0"
 pylint-junit = "^0.3.2"
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-memray = "^1.4.0"
 safety = "^1.10.3"
 typed-ast = "^1.5.4"
 wheel = "^0.38.4"
 
 [build-system]
```

### Comparing `cmem_plugin_examples-0.2.0/PKG-INFO` & `cmem_plugin_examples-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-examples
-Version: 0.2.0
+Version: 0.3.0
 Summary: Example plugins for eccenca Corporate Memory.
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugins,DataIntegration
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
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
-Requires-Dist: cmem-plugin-base (>=3.0.0,<4.0.0)
+Requires-Dist: cmem-plugin-base (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-examples
 
 Example plugins for eccenca Corporate Memory.
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
```

