# Comparing `tmp/hydropump-0.1.2.tar.gz` & `tmp/hydropump-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydropump-0.1.2.tar", max compression
+gzip compressed data, was "hydropump-0.1.4.tar", max compression
```

## Comparing `hydropump-0.1.2.tar` & `hydropump-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-07-10 12:51:19.925666 hydropump-0.1.2/LICENSE
--rw-r--r--   0        0        0     2623 2023-07-10 12:51:19.925666 hydropump-0.1.2/README.md
--rw-r--r--   0        0        0      214 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/__init__.py
--rw-r--r--   0        0        0    11271 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/backend.py
--rw-r--r--   0        0        0     4742 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/instruction.py
--rw-r--r--   0        0        0     6278 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/service.py
--rw-r--r--   0        0        0     3292 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/TESTING.md
--rw-r--r--   0        0        0        0 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/__init__.py
--rw-r--r--   0        0        0     1398 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/conftest.py
--rw-r--r--   0        0        0        0 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/__init__.py
--rw-r--r--   0        0        0     1483 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/test_instructions.py
--rw-r--r--   0        0        0       13 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/test_root/base/.gitignore
--rw-r--r--   0        0        0       13 2023-07-10 12:51:19.925666 hydropump-0.1.2/hydropump/test/unit/test_root/template/.gitignore
--rw-r--r--   0        0        0      740 2023-07-10 12:51:19.925666 hydropump-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 hydropump-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-10 12:54:58.689278 hydropump-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2623 2023-07-10 12:54:58.689278 hydropump-0.1.4/README.md
+-rw-r--r--   0        0        0      214 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/__init__.py
+-rw-r--r--   0        0        0    11271 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/backend.py
+-rw-r--r--   0        0        0     4742 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/instruction.py
+-rw-r--r--   0        0        0     6278 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/service.py
+-rw-r--r--   0        0        0     3292 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/test/TESTING.md
+-rw-r--r--   0        0        0        0 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/test/__init__.py
+-rw-r--r--   0        0        0     1398 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/test/unit/__init__.py
+-rw-r--r--   0        0        0     1483 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/test/unit/test_instructions.py
+-rw-r--r--   0        0        0       13 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/test/unit/test_root/base/.gitignore
+-rw-r--r--   0        0        0       13 2023-07-10 12:54:58.689278 hydropump-0.1.4/hydropump/test/unit/test_root/template/.gitignore
+-rw-r--r--   0        0        0      740 2023-07-10 12:54:58.693277 hydropump-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 hydropump-0.1.4/PKG-INFO
```

### Comparing `hydropump-0.1.2/LICENSE` & `hydropump-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/README.md` & `hydropump-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/hydropump/backend.py` & `hydropump-0.1.4/hydropump/backend.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/hydropump/instruction.py` & `hydropump-0.1.4/hydropump/instruction.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/hydropump/service.py` & `hydropump-0.1.4/hydropump/service.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/hydropump/test/TESTING.md` & `hydropump-0.1.4/hydropump/test/TESTING.md`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/hydropump/test/conftest.py` & `hydropump-0.1.4/hydropump/test/conftest.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/hydropump/test/unit/test_instructions.py` & `hydropump-0.1.4/hydropump/test/unit/test_instructions.py`

 * *Files identical despite different names*

### Comparing `hydropump-0.1.2/pyproject.toml` & `hydropump-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydropump"
-version = "0.1.2"
+version = "0.1.4"
 description = "Configuration Management Library"
 authors = ["Michael Vecchione <51305946+mvecchione145@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `hydropump-0.1.2/PKG-INFO` & `hydropump-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydropump
-Version: 0.1.2
+Version: 0.1.4
 Summary: Configuration Management Library
 License: MIT
 Author: Michael Vecchione
 Author-email: 51305946+mvecchione145@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

