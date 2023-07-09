# Comparing `tmp/NameCreator_EricFerreira-0.0.1.tar.gz` & `tmp/NameCreator_EricFerreira-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NameCreator_EricFerreira-0.0.1.tar", last modified: Fri Jul  7 16:16:23 2023, max compression
+gzip compressed data, was "NameCreator_EricFerreira-0.0.2.tar", last modified: Sun Jul  9 23:39:40 2023, max compression
```

## Comparing `NameCreator_EricFerreira-0.0.1.tar` & `NameCreator_EricFerreira-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:16:23.145752 NameCreator_EricFerreira-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 16:16:23.145752 NameCreator_EricFerreira-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 16:16:09.000000 NameCreator_EricFerreira-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:16:23.145752 NameCreator_EricFerreira-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:16:23.141752 NameCreator_EricFerreira-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:16:23.145752 NameCreator_EricFerreira-0.0.1/src/NameCreator_EricFerreira.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 16:16:23.000000 NameCreator_EricFerreira-0.0.1/src/NameCreator_EricFerreira.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-07 16:16:23.000000 NameCreator_EricFerreira-0.0.1/src/NameCreator_EricFerreira.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:16:23.000000 NameCreator_EricFerreira-0.0.1/src/NameCreator_EricFerreira.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 16:16:23.000000 NameCreator_EricFerreira-0.0.1/src/NameCreator_EricFerreira.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:16:09.000000 NameCreator_EricFerreira-0.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 16:16:09.000000 NameCreator_EricFerreira-0.0.1/src/criador_nomes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:16:23.145752 NameCreator_EricFerreira-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 16:16:09.000000 NameCreator_EricFerreira-0.0.1/test/test_criador_nomes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:39:40.402843 NameCreator_EricFerreira-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-09 23:39:40.402843 NameCreator_EricFerreira-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 23:39:27.000000 NameCreator_EricFerreira-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 23:39:40.402843 NameCreator_EricFerreira-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:39:40.402843 NameCreator_EricFerreira-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:39:40.402843 NameCreator_EricFerreira-0.0.2/src/NameCreator_EricFerreira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-09 23:39:40.000000 NameCreator_EricFerreira-0.0.2/src/NameCreator_EricFerreira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-09 23:39:40.000000 NameCreator_EricFerreira-0.0.2/src/NameCreator_EricFerreira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:39:40.000000 NameCreator_EricFerreira-0.0.2/src/NameCreator_EricFerreira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-09 23:39:40.000000 NameCreator_EricFerreira-0.0.2/src/NameCreator_EricFerreira.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 23:39:27.000000 NameCreator_EricFerreira-0.0.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-09 23:39:27.000000 NameCreator_EricFerreira-0.0.2/src/criador_nomes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:39:40.402843 NameCreator_EricFerreira-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-09 23:39:27.000000 NameCreator_EricFerreira-0.0.2/test/test_criador_nomes.py
```

### Comparing `NameCreator_EricFerreira-0.0.1/PKG-INFO` & `NameCreator_EricFerreira-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NameCreator_EricFerreira
-Version: 0.0.1
+Version: 0.0.2
 Summary: A name creator package only for tests of Continuous Delivery
 Author-email: Eric Ferreira <eric_fpereira@hotmail.com>
 Project-URL: Homepage, https://github.com/ericfp87/teste_trabalho_devops
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NameCreator_EricFerreira-0.0.1/pyproject.toml` & `NameCreator_EricFerreira-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "NameCreator_EricFerreira"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Eric Ferreira", email="eric_fpereira@hotmail.com" },
 ]
 description = "A name creator package only for tests of Continuous Delivery"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NameCreator_EricFerreira-0.0.1/src/NameCreator_EricFerreira.egg-info/PKG-INFO` & `NameCreator_EricFerreira-0.0.2/src/NameCreator_EricFerreira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NameCreator-EricFerreira
-Version: 0.0.1
+Version: 0.0.2
 Summary: A name creator package only for tests of Continuous Delivery
 Author-email: Eric Ferreira <eric_fpereira@hotmail.com>
 Project-URL: Homepage, https://github.com/ericfp87/teste_trabalho_devops
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

