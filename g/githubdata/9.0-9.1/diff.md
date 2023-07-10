# Comparing `tmp/githubdata-9.0.tar.gz` & `tmp/githubdata-9.1.tar.gz`

## Comparing `githubdata-9.0.tar` & `githubdata-9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 githubdata-9.0/.gitattributes
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 githubdata-9.0/requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 githubdata-9.0/src/githubdata/__init__.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 githubdata-9.0/src/githubdata/githubdata.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 githubdata-9.0/tests/test.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 githubdata-9.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 githubdata-9.0/LICENSE
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 githubdata-9.0/README.md
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 githubdata-9.0/pyproject.toml
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 githubdata-9.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 githubdata-9.1/.gitattributes
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 githubdata-9.1/requirements.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 githubdata-9.1/src/githubdata/__init__.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 githubdata-9.1/src/githubdata/githubdata.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 githubdata-9.1/tests/test.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 githubdata-9.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 githubdata-9.1/LICENSE
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 githubdata-9.1/README.md
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 githubdata-9.1/pyproject.toml
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 githubdata-9.1/PKG-INFO
```

### Comparing `githubdata-9.0/src/githubdata/githubdata.py` & `githubdata-9.1/src/githubdata/githubdata.py`

 * *Files identical despite different names*

### Comparing `githubdata-9.0/tests/test.py` & `githubdata-9.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `githubdata-9.0/.gitignore` & `githubdata-9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `githubdata-9.0/LICENSE` & `githubdata-9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `githubdata-9.0/pyproject.toml` & `githubdata-9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "githubdata"
-version = "9.0"
+version = "9.1"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "A simple tool to get the lastest version of a dataset in a Github repository"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
     "giteasy",
     "pandas",
```

### Comparing `githubdata-9.0/PKG-INFO` & `githubdata-9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: githubdata
-Version: 9.0
+Version: 9.1
 Summary: A simple tool to get the lastest version of a dataset in a Github repository
 Project-URL: Homepage, https://github.com/imahdimir/githubdata
 Project-URL: Bug Tracker, https://github.com/imahdimir/githubdata/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

