# Comparing `tmp/ssb_altinn_python-0.3.1.tar.gz` & `tmp/ssb_altinn_python-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.3.1.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.3.2.tar", max compression
```

## Comparing `ssb_altinn_python-0.3.1.tar` & `ssb_altinn_python-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-25 16:57:33.912032 ssb_altinn_python-0.3.1/LICENSE
--rw-r--r--   0        0        0     3941 2023-04-25 16:57:33.912032 ssb_altinn_python-0.3.1/README.md
--rw-r--r--   0        0        0     1967 2023-04-25 16:57:52.336315 ssb_altinn_python-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      188 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/__main__.py
--rw-r--r--   0        0        0     1831 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/flatten.py
--rw-r--r--   0        0        0     4208 2023-04-25 16:57:52.336315 ssb_altinn_python-0.3.1/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/py.typed
--rw-r--r--   0        0        0      497 2023-04-25 16:57:33.916033 ssb_altinn_python-0.3.1/src/altinn/utils.py
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-10 16:47:50.446190 ssb_altinn_python-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3941 2023-07-10 16:47:50.446190 ssb_altinn_python-0.3.2/README.md
+-rw-r--r--   0        0        0     1967 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      185 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-10 16:47:50.450191 ssb_altinn_python-0.3.2/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1831 2023-07-10 16:47:50.450191 ssb_altinn_python-0.3.2/src/altinn/file.py
+-rw-r--r--   0        0        0     2179 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/flatten.py
+-rw-r--r--   0        0        0     4007 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-07-10 16:47:50.450191 ssb_altinn_python-0.3.2/src/altinn/py.typed
+-rw-r--r--   0        0        0     1236 2023-07-10 16:48:11.427420 ssb_altinn_python-0.3.2/src/altinn/utils.py
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 ssb_altinn_python-0.3.2/PKG-INFO
```

### Comparing `ssb_altinn_python-0.3.1/LICENSE` & `ssb_altinn_python-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.3.1/README.md` & `ssb_altinn_python-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.3.1/pyproject.toml` & `ssb_altinn_python-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.3.1"
+version = "0.3.2"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.3.1/src/altinn/file.py` & `ssb_altinn_python-0.3.2/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.3.1/PKG-INFO` & `ssb_altinn_python-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.3.1
+Version: 0.3.2
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

