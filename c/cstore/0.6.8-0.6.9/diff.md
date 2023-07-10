# Comparing `tmp/cstore-0.6.8.tar.gz` & `tmp/cstore-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cstore-0.6.8.tar", last modified: Mon Jul 10 11:39:33 2023, max compression
+gzip compressed data, was "cstore-0.6.9.tar", last modified: Mon Jul 10 11:56:08 2023, max compression
```

## Comparing `cstore-0.6.8.tar` & `cstore-0.6.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:39:33.093301 cstore-0.6.8/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.8/LICENSE
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-07-10 11:39:33.093301 cstore-0.6.8/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     5529 2023-07-10 11:04:36.000000 cstore-0.6.8/README.md
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:39:33.089301 cstore-0.6.8/cstore/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       21 2023-06-28 21:59:24.000000 cstore-0.6.8/cstore/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15491 2023-07-10 11:03:50.000000 cstore-0.6.8/cstore/cli.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.8/cstore/constants.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      481 2023-06-27 12:02:50.000000 cstore-0.6.8/cstore/database.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1007 2023-06-28 10:47:25.000000 cstore-0.6.8/cstore/models.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:39:33.093301 cstore-0.6.8/cstore/repo/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 10:48:25.000000 cstore-0.6.8/cstore/repo/__init__.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2931 2023-06-28 21:58:54.000000 cstore-0.6.8/cstore/repo/repo_command.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1341 2023-06-28 21:57:57.000000 cstore-0.6.8/cstore/repo/repo_tag.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1757 2023-06-25 23:16:56.000000 cstore-0.6.8/cstore/schemes.py
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.8/cstore/verbose.py
-drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:39:33.093301 cstore-0.6.8/cstore.egg-info/
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-07-10 11:39:33.000000 cstore-0.6.8/cstore.egg-info/PKG-INFO
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-07-10 11:39:33.000000 cstore-0.6.8/cstore.egg-info/SOURCES.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-07-10 11:39:33.000000 cstore-0.6.8/cstore.egg-info/dependency_links.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-07-10 11:39:33.000000 cstore-0.6.8/cstore.egg-info/entry_points.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      124 2023-07-10 11:39:33.000000 cstore-0.6.8/cstore.egg-info/requires.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-07-10 11:39:33.000000 cstore-0.6.8/cstore.egg-info/top_level.txt
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      976 2023-07-10 11:39:21.000000 cstore-0.6.8/pyproject.toml
--rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-07-10 11:39:33.093301 cstore-0.6.8/setup.cfg
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:56:08.144801 cstore-0.6.9/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1073 2023-06-14 08:18:09.000000 cstore-0.6.9/LICENSE
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-07-10 11:56:08.140801 cstore-0.6.9/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     5529 2023-07-10 11:04:36.000000 cstore-0.6.9/README.md
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:56:08.140801 cstore-0.6.9/cstore/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       21 2023-06-28 21:59:24.000000 cstore-0.6.9/cstore/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)    15491 2023-07-10 11:03:50.000000 cstore-0.6.9/cstore/cli.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      180 2023-06-25 12:51:24.000000 cstore-0.6.9/cstore/constants.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      481 2023-06-27 12:02:50.000000 cstore-0.6.9/cstore/database.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1007 2023-06-28 10:47:25.000000 cstore-0.6.9/cstore/models.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:56:08.140801 cstore-0.6.9/cstore/repo/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-06-28 10:48:25.000000 cstore-0.6.9/cstore/repo/__init__.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     2931 2023-06-28 21:58:54.000000 cstore-0.6.9/cstore/repo/repo_command.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1341 2023-06-28 21:57:57.000000 cstore-0.6.9/cstore/repo/repo_tag.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     1757 2023-06-25 23:16:56.000000 cstore-0.6.9/cstore/schemes.py
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      529 2023-06-25 14:04:16.000000 cstore-0.6.9/cstore/verbose.py
+drwxrwxr-x   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        0 2023-07-10 11:56:08.140801 cstore-0.6.9/cstore.egg-info/
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)     6210 2023-07-10 11:56:08.000000 cstore-0.6.9/cstore.egg-info/PKG-INFO
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      415 2023-07-10 11:56:08.000000 cstore-0.6.9/cstore.egg-info/SOURCES.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        1 2023-07-10 11:56:08.000000 cstore-0.6.9/cstore.egg-info/dependency_links.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       42 2023-07-10 11:56:08.000000 cstore-0.6.9/cstore.egg-info/entry_points.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      121 2023-07-10 11:56:08.000000 cstore-0.6.9/cstore.egg-info/requires.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)        7 2023-07-10 11:56:08.000000 cstore-0.6.9/cstore.egg-info/top_level.txt
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)      973 2023-07-10 11:55:58.000000 cstore-0.6.9/pyproject.toml
+-rw-rw-r--   0 navid-ubuntu  (1000) navid-ubuntu  (1000)       38 2023-07-10 11:56:08.144801 cstore-0.6.9/setup.cfg
```

### Comparing `cstore-0.6.8/LICENSE` & `cstore-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/PKG-INFO` & `cstore-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.8
+Version: 0.6.9
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Documentation, https://github.com/navidved/ctore
 Project-URL: Repository, https://github.com/navidved/ctore
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cstore-0.6.8/README.md` & `cstore-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/cstore/cli.py` & `cstore-0.6.9/cstore/cli.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/cstore/models.py` & `cstore-0.6.9/cstore/models.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/cstore/repo/repo_command.py` & `cstore-0.6.9/cstore/repo/repo_command.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/cstore/repo/repo_tag.py` & `cstore-0.6.9/cstore/repo/repo_tag.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/cstore/schemes.py` & `cstore-0.6.9/cstore/schemes.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/cstore/verbose.py` & `cstore-0.6.9/cstore/verbose.py`

 * *Files identical despite different names*

### Comparing `cstore-0.6.8/cstore.egg-info/PKG-INFO` & `cstore-0.6.9/cstore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cstore
-Version: 0.6.8
+Version: 0.6.9
 Summary: A tools to store and recall useful commands, specifically created to assist forgetful individuals
 Author-email: Navid Arabi <navidved@gmail.com>
 Project-URL: Bug Tracker, https://github.com/navidved/ctore/issues
 Project-URL: Homepage, https://github.com/navidved/ctore
 Project-URL: Documentation, https://github.com/navidved/ctore
 Project-URL: Repository, https://github.com/navidved/ctore
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cstore-0.6.8/pyproject.toml` & `cstore-0.6.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cstore"
-version = "0.6.8"
+version = "0.6.9"
 dependencies = [
     "rich==13.4.2",
     "cryptocode==0.1",
     "SQLAlchemy==2.0.16",
-    "pydantic==1.10.9",
+    "pydantic==1.8",
     "typer[all]==0.9.0",
     "simple_term_menu==1.6.1",
     "clipboard==1.8.2",
 ]
 authors = [
   { name="Navid Arabi", email="navidved@gmail.com" },
 ]
```

