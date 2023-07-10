# Comparing `tmp/devopsstringtest-0.0.1.tar.gz` & `tmp/devopsstringtest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsstringtest-0.0.1.tar", last modified: Mon Jul 10 17:24:29 2023, max compression
+gzip compressed data, was "devopsstringtest-0.0.2.tar", last modified: Mon Jul 10 18:14:47 2023, max compression
```

## Comparing `devopsstringtest-0.0.1.tar` & `devopsstringtest-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:24:29.510711 devopsstringtest-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 17:24:17.000000 devopsstringtest-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-10 17:24:29.510711 devopsstringtest-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 17:24:17.000000 devopsstringtest-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-10 17:24:17.000000 devopsstringtest-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 17:24:17.000000 devopsstringtest-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 17:24:29.510711 devopsstringtest-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:24:29.510711 devopsstringtest-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:24:29.510711 devopsstringtest-0.0.1/src/devopsstringtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-10 17:24:29.000000 devopsstringtest-0.0.1/src/devopsstringtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-10 17:24:29.000000 devopsstringtest-0.0.1/src/devopsstringtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 17:24:29.000000 devopsstringtest-0.0.1/src/devopsstringtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 17:24:29.000000 devopsstringtest-0.0.1/src/devopsstringtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 17:24:29.000000 devopsstringtest-0.0.1/src/devopsstringtest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:24:29.510711 devopsstringtest-0.0.1/src/stringstandardization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 17:24:17.000000 devopsstringtest-0.0.1/src/stringstandardization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 17:24:17.000000 devopsstringtest-0.0.1/src/stringstandardization/stringstd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 17:24:29.510711 devopsstringtest-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-10 17:24:17.000000 devopsstringtest-0.0.1/test/test_stringstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:47.335039 devopsstringtest-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 18:14:37.000000 devopsstringtest-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-10 18:14:47.335039 devopsstringtest-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 18:14:37.000000 devopsstringtest-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-10 18:14:37.000000 devopsstringtest-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 18:14:37.000000 devopsstringtest-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:14:47.335039 devopsstringtest-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:47.331039 devopsstringtest-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:47.335039 devopsstringtest-0.0.2/src/devopsstringtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-10 18:14:47.000000 devopsstringtest-0.0.2/src/devopsstringtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-10 18:14:47.000000 devopsstringtest-0.0.2/src/devopsstringtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:14:47.000000 devopsstringtest-0.0.2/src/devopsstringtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 18:14:47.000000 devopsstringtest-0.0.2/src/devopsstringtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 18:14:47.000000 devopsstringtest-0.0.2/src/devopsstringtest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:47.335039 devopsstringtest-0.0.2/src/stringstandardization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:37.000000 devopsstringtest-0.0.2/src/stringstandardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 18:14:37.000000 devopsstringtest-0.0.2/src/stringstandardization/stringstd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:14:47.335039 devopsstringtest-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-10 18:14:37.000000 devopsstringtest-0.0.2/test/test_stringstd.py
```

### Comparing `devopsstringtest-0.0.1/LICENSE` & `devopsstringtest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsstringtest-0.0.1/PKG-INFO` & `devopsstringtest-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsstringtest
-Version: 0.0.1
+Version: 0.0.2
 Summary: string standardization package
 Author-email: Sylvio Rubens <srjneto@hotmail.com>
 Project-URL: Homepage, https://github.com/SylvioRubens/devops_project
 Project-URL: Bug Tracker, https://github.com/SylvioRubens/devops_project/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `devopsstringtest-0.0.1/pyproject.toml` & `devopsstringtest-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "devopsstringtest"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Sylvio Rubens", email="srjneto@hotmail.com"},
 ]
 description = "string standardization package"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `devopsstringtest-0.0.1/src/devopsstringtest.egg-info/PKG-INFO` & `devopsstringtest-0.0.2/src/devopsstringtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsstringtest
-Version: 0.0.1
+Version: 0.0.2
 Summary: string standardization package
 Author-email: Sylvio Rubens <srjneto@hotmail.com>
 Project-URL: Homepage, https://github.com/SylvioRubens/devops_project
 Project-URL: Bug Tracker, https://github.com/SylvioRubens/devops_project/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

