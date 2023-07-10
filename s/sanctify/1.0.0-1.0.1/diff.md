# Comparing `tmp/sanctify-1.0.0.tar.gz` & `tmp/sanctify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.0.0.tar", last modified: Mon Jul 10 06:16:57 2023, max compression
+gzip compressed data, was "sanctify-1.0.1.tar", last modified: Mon Jul 10 07:28:08 2023, max compression
```

## Comparing `sanctify-1.0.0.tar` & `sanctify-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 06:16:57.210311 sanctify-1.0.0/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.0/LICENSE.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      674 2023-07-10 06:16:57.210152 sanctify-1.0.0/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3283 2023-07-10 06:16:22.000000 sanctify-1.0.0/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1621 2023-07-07 16:45:27.000000 sanctify-1.0.0/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 06:16:57.209146 sanctify-1.0.0/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-07 16:45:27.000000 sanctify-1.0.0/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7047 2023-07-07 16:45:27.000000 sanctify-1.0.0/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2593 2023-07-07 16:45:27.000000 sanctify-1.0.0/sanctify/constants.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.0/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11965 2023-07-10 06:16:23.000000 sanctify-1.0.0/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8726 2023-07-07 16:45:27.000000 sanctify-1.0.0/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3410 2023-07-07 16:45:27.000000 sanctify-1.0.0/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     6399 2023-07-10 06:16:23.000000 sanctify-1.0.0/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 06:16:57.209928 sanctify-1.0.0/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      674 2023-07-10 06:16:57.000000 sanctify-1.0.0/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-10 06:16:57.000000 sanctify-1.0.0/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-10 06:16:57.000000 sanctify-1.0.0/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-10 06:16:57.000000 sanctify-1.0.0/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-10 06:16:57.210386 sanctify-1.0.0/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 07:28:08.395044 sanctify-1.0.1/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.1/LICENSE.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10059 2023-07-10 07:28:08.394822 sanctify-1.0.1/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9344 2023-07-10 07:25:37.000000 sanctify-1.0.1/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1642 2023-07-10 07:27:50.000000 sanctify-1.0.1/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 07:28:08.393844 sanctify-1.0.1/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7047 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2593 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/constants.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11965 2023-07-10 07:25:08.000000 sanctify-1.0.1/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8726 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3410 2023-07-07 16:45:27.000000 sanctify-1.0.1/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     6399 2023-07-10 07:25:09.000000 sanctify-1.0.1/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-10 07:28:08.394607 sanctify-1.0.1/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10059 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-10 07:28:08.000000 sanctify-1.0.1/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-10 07:28:08.395081 sanctify-1.0.1/setup.cfg
```

### Comparing `sanctify-1.0.0/LICENSE.txt` & `sanctify-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.0/pyproject.toml` & `sanctify-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -59,17 +59,18 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Allowed config based cleansing and validations for a given pandas dataframe"
+readme = "README.md"
 requires-python = ">=3.9"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `sanctify-1.0.0/sanctify/cleanser.py` & `sanctify-1.0.1/sanctify/cleanser.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.0/sanctify/constants.py` & `sanctify-1.0.1/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.0/sanctify/processor.py` & `sanctify-1.0.1/sanctify/processor.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.0/sanctify/transformer.py` & `sanctify-1.0.1/sanctify/transformer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.0/sanctify/utils.py` & `sanctify-1.0.1/sanctify/utils.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.0/sanctify/validator.py` & `sanctify-1.0.1/sanctify/validator.py`

 * *Files identical despite different names*

