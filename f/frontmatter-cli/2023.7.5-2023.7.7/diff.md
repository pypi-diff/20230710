# Comparing `tmp/frontmatter-cli-2023.7.5.tar.gz` & `tmp/frontmatter-cli-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontmatter-cli-2023.7.5.tar", last modified: Sun Jul  9 14:08:51 2023, max compression
+gzip compressed data, was "frontmatter-cli-2023.7.7.tar", last modified: Mon Jul 10 14:16:45 2023, max compression
```

## Comparing `frontmatter-cli-2023.7.5.tar` & `frontmatter-cli-2023.7.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 14:08:51.670415 frontmatter-cli-2023.7.5/
--rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.5/HISTORY.md
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.5/LICENSE
--rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.5/MANIFEST.in
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2731 2023-07-09 14:08:51.670313 frontmatter-cli-2023.7.5/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-09 02:23:17.000000 frontmatter-cli-2023.7.5/README.md
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 14:08:51.669096 frontmatter-cli-2023.7.5/frontmatter_cli/
--rw-r--r--   0 jefftriplett   (501) staff       (20)       67 2023-07-09 13:35:20.000000 frontmatter-cli-2023.7.5/frontmatter_cli/__init__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.5/frontmatter_cli/__main__.py
--rw-r--r--   0 jefftriplett   (501) staff       (20)     1325 2023-07-09 14:08:38.000000 frontmatter-cli-2023.7.5/frontmatter_cli/cli.py
-drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-09 14:08:51.670159 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2731 2023-07-09 14:08:51.000000 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/PKG-INFO
--rw-r--r--   0 jefftriplett   (501) staff       (20)      408 2023-07-09 14:08:51.000000 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-07-09 14:08:51.000000 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-07-09 14:08:51.000000 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/entry_points.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/not-zip-safe
--rw-r--r--   0 jefftriplett   (501) staff       (20)       81 2023-07-09 14:08:51.000000 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/requires.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-07-09 14:08:51.000000 frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/top_level.txt
--rw-r--r--   0 jefftriplett   (501) staff       (20)     2677 2023-07-09 14:08:38.000000 frontmatter-cli-2023.7.5/pyproject.toml
--rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-07-09 14:08:51.670450 frontmatter-cli-2023.7.5/setup.cfg
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-10 14:16:45.003510 frontmatter-cli-2023.7.7/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       11 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.7/HISTORY.md
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1513 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.7/LICENSE
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      134 2023-06-09 02:13:44.000000 frontmatter-cli-2023.7.7/MANIFEST.in
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2688 2023-07-10 14:16:45.003171 frontmatter-cli-2023.7.7/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1683 2023-06-10 14:14:57.000000 frontmatter-cli-2023.7.7/README.md
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-10 14:16:45.000181 frontmatter-cli-2023.7.7/frontmatter_cli/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       67 2023-07-09 21:37:56.000000 frontmatter-cli-2023.7.7/frontmatter_cli/__init__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       74 2023-07-09 21:25:48.000000 frontmatter-cli-2023.7.7/frontmatter_cli/__main__.py
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     1299 2023-07-10 14:15:12.000000 frontmatter-cli-2023.7.7/frontmatter_cli/cli.py
+drwxr-xr-x   0 jefftriplett   (501) staff       (20)        0 2023-07-10 14:16:45.002782 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2688 2023-07-10 14:16:44.000000 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      408 2023-07-10 14:16:44.000000 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-07-10 14:16:44.000000 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       90 2023-07-10 14:16:44.000000 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)        1 2023-06-09 02:14:15.000000 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/not-zip-safe
+-rw-r--r--   0 jefftriplett   (501) staff       (20)      100 2023-07-10 14:16:44.000000 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/requires.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       16 2023-07-10 14:16:44.000000 frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/top_level.txt
+-rw-r--r--   0 jefftriplett   (501) staff       (20)     2742 2023-07-10 14:15:12.000000 frontmatter-cli-2023.7.7/pyproject.toml
+-rw-r--r--   0 jefftriplett   (501) staff       (20)       38 2023-07-10 14:16:45.003637 frontmatter-cli-2023.7.7/setup.cfg
```

### Comparing `frontmatter-cli-2023.7.5/LICENSE` & `frontmatter-cli-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `frontmatter-cli-2023.7.5/PKG-INFO` & `frontmatter-cli-2023.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: frontmatter-cli
-Version: 2023.7.5
+Version: 2023.7.7
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
 Author-email: Jeff Triplett <jeff.triplett@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
 Project-URL: Issues, https://github.com/jefftriplett/frontmatter-cli/issues
-Project-URL: Source Code, https://github.com/jefftriplett/frontmatter-cli
+Project-URL: Source, https://github.com/jefftriplett/frontmatter-cli
 Keywords: frontmatter,frontmatter-cli
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: Django
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
-Provides-Extra: build
+Provides-Extra: dev
 License-File: LICENSE
 
 # frontmatter-cli
 
 This is a very early WIP project. My goal is to make working with Frontmatter a little nicer from the command line. The API is going to change, and I plan on adding some other features to make editing Frontmatter easier too.
 
 ## Install
```

### Comparing `frontmatter-cli-2023.7.5/README.md` & `frontmatter-cli-2023.7.7/README.md`

 * *Files identical despite different names*

### Comparing `frontmatter-cli-2023.7.5/frontmatter_cli/cli.py` & `frontmatter-cli-2023.7.7/frontmatter_cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# -*- coding: utf-8 -*-
-
 import click
 import frontmatter
-
 from click_default_group import DefaultGroup
 from pydash import set_
 
 __author__ = "Jeff Triplett"
 __email__ = "jeff.triplett@gmail.com"
-__version__ = "2023.7.5"
+__version__ = "2023.7.7"
 
 
 def validate_extra_context(ctx, param, value):
     """Validate extra context."""
     for key in value:
         if "=" not in key:
             raise click.BadParameter(
```

### Comparing `frontmatter-cli-2023.7.5/frontmatter_cli.egg-info/PKG-INFO` & `frontmatter-cli-2023.7.7/frontmatter_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: frontmatter-cli
-Version: 2023.7.5
+Version: 2023.7.7
 Summary: Frontmatter CLI tool to make working with frontmatter easier.
 Author-email: Jeff Triplett <jeff.triplett@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/jefftriplett/frontmatter-cli
 Project-URL: Issues, https://github.com/jefftriplett/frontmatter-cli/issues
-Project-URL: Source Code, https://github.com/jefftriplett/frontmatter-cli
+Project-URL: Source, https://github.com/jefftriplett/frontmatter-cli
 Keywords: frontmatter,frontmatter-cli
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: Django
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
-Provides-Extra: build
+Provides-Extra: dev
 License-File: LICENSE
 
 # frontmatter-cli
 
 This is a very early WIP project. My goal is to make working with Frontmatter a little nicer from the command line. The API is going to change, and I plan on adding some other features to make editing Frontmatter easier too.
 
 ## Install
```

### Comparing `frontmatter-cli-2023.7.5/pyproject.toml` & `frontmatter-cli-2023.7.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "frontmatter-cli"
-version = "2023.7.5"
+version = "2023.7.7"
 description = "Frontmatter CLI tool to make working with frontmatter easier."
 readme = "README.md"
 keywords = [
   "frontmatter",
   "frontmatter-cli",
 ]
 license = {text = "BSD-3-Clause"}
 authors = [{name = "Jeff Triplett", email = "jeff.triplett@gmail.com"}]
 requires-python = ">3.7"
 classifiers = [
-  "Development Status :: 2 - Pre-Alpha",
-  "Framework :: Django",
+  "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -31,40 +30,48 @@
 dependencies = [
   "click",
   "click-default-group",
   "pydash",
   "python-frontmatter",
 ]
 [project.optional-dependencies]
-build = [
+dev = [
   "build",
   "bumpver",
+  "pip-tools",
+  "pre-commit",
   "twine",
 ]
 [project.urls]
 Homepage = "https://github.com/jefftriplett/frontmatter-cli"
 Issues = "https://github.com/jefftriplett/frontmatter-cli/issues"
-"Source Code" = "https://github.com/jefftriplett/frontmatter-cli"
+Source = "https://github.com/jefftriplett/frontmatter-cli"
 [project.scripts]
 frontmatter = "frontmatter_cli:cli"
 frontmatter-cli = "frontmatter_cli:cli"
 
 [tool.setuptools]
 packages = ["frontmatter_cli"]
 zip-safe = false
 license-files = ["LICENSE"]
 include-package-data = false
 
 [tool.ruff]
 # Enable Pyflakes `E` and `F` codes by default.
-select = ["E", "F"]
+select = [
+  "E",  # pycodestyle
+  "F",  # pyflakes
+  "I",   # isort
+  "UP",  # pyupgrade
+  "TRY", # tryceratops
+]
 ignore = ["E501", "E741"] # temporary
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F"]
+fixable = ["ALL"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
@@ -96,15 +103,15 @@
 target-version = "py311"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.bumpver]
-current_version = "2023.7.5"
+current_version = "2023.7.7"
 version_pattern = "YYYY.MM.INC1"
 commit_message = ":bookmark: Bump version {old_version} -> {new_version}"
 commit = true
 push = true  # disable for GitHub Actions
 tag = true
 
 [tool.bumpver.file_patterns]
```

