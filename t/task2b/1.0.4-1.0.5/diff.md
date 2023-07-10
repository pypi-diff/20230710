# Comparing `tmp/task2b-1.0.4.tar.gz` & `tmp/task2b-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2b-1.0.4.tar", max compression
+gzip compressed data, was "task2b-1.0.5.tar", max compression
```

## Comparing `task2b-1.0.4.tar` & `task2b-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.4/LICENSE
--rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.4/pwgen2/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.4/pwgen2/__main__.py
--rw-r--r--   0        0        0       23 2023-07-10 20:14:00.326021 task2b-1.0.4/pwgen2/__version__.py
--rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.4/pwgen2/cli/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.4/pwgen2/cli/__main__.py
--rw-r--r--   0        0        0     4664 2023-07-10 15:53:00.202469 task2b-1.0.4/pwgen2/cli/cli.py
--rw-r--r--   0        0        0    10100 2023-07-10 20:52:19.816687 task2b-1.0.4/pwgen2/pwgen2.py
--rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.4/pwgen2/showcase/__init__.py
--rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.4/pwgen2/showcase/__main__.py
--rw-r--r--   0        0        0      132 2023-07-10 16:39:29.431805 task2b-1.0.4/pwgen2/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      284 2023-07-10 16:39:29.435804 task2b-1.0.4/pwgen2/showcase/pattern-list.txt
--rw-r--r--   0        0        0    22956 2023-07-10 20:25:21.106001 task2b-1.0.4/pwgen2/showcase/showcase.py
--rw-r--r--   0        0        0      587 2023-07-10 20:14:00.331019 task2b-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    17418 2023-07-10 20:13:20.833667 task2b-1.0.4/README.md
--rw-r--r--   0        0        0    17813 1970-01-01 00:00:00.000000 task2b-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task2b-1.0.5/LICENSE
+-rw-r--r--   0        0        0      321 2023-07-08 15:34:54.474410 task2b-1.0.5/pwgen2/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:34:54.488388 task2b-1.0.5/pwgen2/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-10 21:08:09.396534 task2b-1.0.5/pwgen2/__version__.py
+-rw-r--r--   0        0        0       74 2023-07-08 15:35:37.625438 task2b-1.0.5/pwgen2/cli/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 15:35:37.612436 task2b-1.0.5/pwgen2/cli/__main__.py
+-rw-r--r--   0        0        0     4664 2023-07-10 15:53:00.202469 task2b-1.0.5/pwgen2/cli/cli.py
+-rw-r--r--   0        0        0    10100 2023-07-10 20:52:19.816687 task2b-1.0.5/pwgen2/pwgen2.py
+-rw-r--r--   0        0        0       94 2023-07-08 15:35:37.620439 task2b-1.0.5/pwgen2/showcase/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-08 15:35:37.616441 task2b-1.0.5/pwgen2/showcase/__main__.py
+-rw-r--r--   0        0        0      132 2023-07-10 16:39:29.431805 task2b-1.0.5/pwgen2/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      284 2023-07-10 16:39:29.435804 task2b-1.0.5/pwgen2/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    22956 2023-07-10 21:06:49.720903 task2b-1.0.5/pwgen2/showcase/showcase.py
+-rw-r--r--   0        0        0      587 2023-07-10 21:08:09.401545 task2b-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    17418 2023-07-10 20:13:20.833667 task2b-1.0.5/README.md
+-rw-r--r--   0        0        0    17813 1970-01-01 00:00:00.000000 task2b-1.0.5/PKG-INFO
```

### Comparing `task2b-1.0.4/pwgen2/cli/cli.py` & `task2b-1.0.5/pwgen2/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.4/pwgen2/pwgen2.py` & `task2b-1.0.5/pwgen2/pwgen2.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.4/pwgen2/showcase/showcase.py` & `task2b-1.0.5/pwgen2/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task2b-1.0.4/pyproject.toml` & `task2b-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task2b"
-version = "1.0.4"
+version = "1.0.5"
 description = "Password generation CLI and library version 2"
 repository = "https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pwgen2"}]
 license = "MIT"
```

### Comparing `task2b-1.0.4/README.md` & `task2b-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `task2b-1.0.4/PKG-INFO` & `task2b-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task2b
-Version: 1.0.4
+Version: 1.0.5
 Summary: Password generation CLI and library version 2
 Home-page: https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task2b
 License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: task2b Version: 1.0.4 Summary: Password generation
+Metadata-Version: 2.1 Name: task2b Version: 1.0.5 Summary: Password generation
 CLI and library version 2 Home-page: https://gitlab.com/Bill-EPAM-
 DevOpsInt2023/python/task2b License: MIT Author: Bill.Avramenko Author-email:
 billavramenko@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/
```

