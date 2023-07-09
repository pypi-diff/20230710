# Comparing `tmp/pyhowdoi-1.0.1.tar.gz` & `tmp/pyhowdoi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhowdoi-1.0.1.tar", max compression
+gzip compressed data, was "pyhowdoi-1.0.2.tar", max compression
```

## Comparing `pyhowdoi-1.0.1.tar` & `pyhowdoi-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-07-09 22:30:24.182855 pyhowdoi-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1505 2023-07-09 22:26:30.088271 pyhowdoi-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-09 21:25:00.385627 pyhowdoi-1.0.1/pyhowdoi/__init__.py
--rw-r--r--   0        0        0     1186 2023-07-09 22:24:16.238584 pyhowdoi-1.0.1/pyhowdoi/main.py
--rw-r--r--   0        0        0      415 2023-07-09 22:30:48.910436 pyhowdoi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1975 1970-01-01 00:00:00.000000 pyhowdoi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-09 22:30:24.182855 pyhowdoi-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1505 2023-07-09 22:26:30.088271 pyhowdoi-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 21:25:00.385627 pyhowdoi-1.0.2/pyhowdoi/__init__.py
+-rw-r--r--   0        0        0     1186 2023-07-09 22:24:16.238584 pyhowdoi-1.0.2/pyhowdoi/main.py
+-rw-r--r--   0        0        0      487 2023-07-09 22:31:56.905951 pyhowdoi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 pyhowdoi-1.0.2/PKG-INFO
```

### Comparing `pyhowdoi-1.0.1/LICENSE.txt` & `pyhowdoi-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhowdoi-1.0.1/README.md` & `pyhowdoi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhowdoi-1.0.1/pyhowdoi/main.py` & `pyhowdoi-1.0.2/pyhowdoi/main.py`

 * *Files identical despite different names*

### Comparing `pyhowdoi-1.0.1/PKG-INFO` & `pyhowdoi-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: pyhowdoi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use ChatGPT for quick command-line advice
+Home-page: https://github.com/Thomas-McKanna/pyhowdoi
+License: MIT
 Author: Thomas McKanna
 Author-email: thomasmckanna@proton.me
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dependency (>=0.0.3,<0.0.4)
 Requires-Dist: simplechatgpt (>=1.0,<2.0)
 Description-Content-Type: text/markdown
```

