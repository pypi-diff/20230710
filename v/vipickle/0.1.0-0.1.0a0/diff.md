# Comparing `tmp/vipickle-0.1.0.tar.gz` & `tmp/vipickle-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipickle-0.1.0.tar", last modified: Mon Jul 10 19:05:48 2023, max compression
+gzip compressed data, was "vipickle-0.1.0a0.tar", last modified: Wed Jun 14 22:18:34 2023, max compression
```

## Comparing `vipickle-0.1.0.tar` & `vipickle-0.1.0a0.tar`

### file list

```diff
@@ -1,48 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.313380 vipickle-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 19:05:38.000000 vipickle-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-10 19:05:38.000000 vipickle-0.1.0/.github/workflows/build-mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-10 19:05:38.000000 vipickle-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-10 19:05:38.000000 vipickle-0.1.0/.github/workflows/unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 19:05:38.000000 vipickle-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-10 19:05:38.000000 vipickle-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-10 19:05:48.313380 vipickle-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-10 19:05:38.000000 vipickle-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/docs/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/assets/images/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/assets/images/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/examples/pytorch.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/docs/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/features/blacklist.md
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/features/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/features/loading.md
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/features/saving.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 19:05:38.000000 vipickle-0.1.0/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-10 19:05:38.000000 vipickle-0.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-10 19:05:38.000000 vipickle-0.1.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-10 19:05:38.000000 vipickle-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:05:48.313380 vipickle-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:05:38.000000 vipickle-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.309380 vipickle-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.313380 vipickle-0.1.0/src/vipickle/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-10 19:05:38.000000 vipickle-0.1.0/src/vipickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 19:05:48.000000 vipickle-0.1.0/src/vipickle/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-10 19:05:38.000000 vipickle-0.1.0/src/vipickle/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-10 19:05:38.000000 vipickle-0.1.0/src/vipickle/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-10 19:05:38.000000 vipickle-0.1.0/src/vipickle/save_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.313380 vipickle-0.1.0/src/vipickle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-10 19:05:48.000000 vipickle-0.1.0/src/vipickle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-10 19:05:48.000000 vipickle-0.1.0/src/vipickle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:05:48.000000 vipickle-0.1.0/src/vipickle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-10 19:05:48.000000 vipickle-0.1.0/src/vipickle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 19:05:48.000000 vipickle-0.1.0/src/vipickle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:05:48.313380 vipickle-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 19:05:38.000000 vipickle-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-10 19:05:38.000000 vipickle-0.1.0/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-10 19:05:38.000000 vipickle-0.1.0/tests/test_save_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.970456 vipickle-0.1.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.970456 vipickle-0.1.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.970456 vipickle-0.1.0a0/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/docs/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/docs/assets/images/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/docs/assets/images/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/docs/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/docs/fr/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.970456 vipickle-0.1.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/src/vipickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/src/vipickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 22:18:34.000000 vipickle-0.1.0a0/src/vipickle/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/src/vipickle/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/src/vipickle/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/src/vipickle/save_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/src/vipickle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-14 22:18:34.000000 vipickle-0.1.0a0/src/vipickle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-14 22:18:34.000000 vipickle-0.1.0a0/src/vipickle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:18:34.000000 vipickle-0.1.0a0/src/vipickle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-14 22:18:34.000000 vipickle-0.1.0a0/src/vipickle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 22:18:34.000000 vipickle-0.1.0a0/src/vipickle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:18:34.974456 vipickle-0.1.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-14 22:18:24.000000 vipickle-0.1.0a0/tests/test_save_utils.py
```

### Comparing `vipickle-0.1.0/.github/workflows/python-publish.yml` & `vipickle-0.1.0a0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `vipickle-0.1.0/PKG-INFO` & `vipickle-0.1.0a0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 Metadata-Version: 2.1
 Name: vipickle
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: vipickle is a tiny python package for saving instances with unpickable attributes
 Author-email: Hakim Cheikh <hakimcheikh@yahoo.fr>
 Project-URL: homepage, https://github.com/h4c5/vipickle
-Project-URL: documentation, https://h4c5.github.io/vipickle
+Project-URL: documentation, https://github.com/h4c5/vipickle
 Project-URL: repository, https://github.com/h4c5/vipickle
-Project-URL: Bug Tracker, https://github.com/h4c5/vipickle/issues
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Project-URL: Bug Tracker, https://github.com/h4c5/vipickle
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: doc
 
 <div align="center">
     <img src="https://img.shields.io/pypi/v/vipickle" alt="vipickle package version" />
     <img src="https://img.shields.io/pypi/pyversions/vipickle" alt="Python supported versions" />
-    <a href="https://github.com/h4c5/vipickle/actions/workflows/unit-tests.yml">
-        <img src="https://github.com/h4c5/vipickle/actions/workflows/unit-tests.yml/badge.svg" alt="unit tests status" />
-    </a>
     <a href="https://github.com/PyCQA/bandit">
         <img src="https://img.shields.io/badge/security-bandit-yellow.svg" alt="Security thanks to bandit package" />
     </a>
     <img src="https://img.shields.io/badge/formatting-black-black" alt="Black formatting" />
 </div>
 
 <div align="center">
```

### Comparing `vipickle-0.1.0/README.md` & `vipickle-0.1.0a0/docs/fr/index.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,24 @@
-<div align="center">
-    <img src="https://img.shields.io/pypi/v/vipickle" alt="vipickle package version" />
-    <img src="https://img.shields.io/pypi/pyversions/vipickle" alt="Python supported versions" />
-    <a href="https://github.com/h4c5/vipickle/actions/workflows/unit-tests.yml">
-        <img src="https://github.com/h4c5/vipickle/actions/workflows/unit-tests.yml/badge.svg" alt="unit tests status" />
-    </a>
-    <a href="https://github.com/PyCQA/bandit">
-        <img src="https://img.shields.io/badge/security-bandit-yellow.svg" alt="Security thanks to bandit package" />
-    </a>
-    <img src="https://img.shields.io/badge/formatting-black-black" alt="Black formatting" />
-</div>
-
-<div align="center">
-    <h1>👑 VIPpickle</h1>
-    <p ><b>Tiny python package for saving instances with unpickable attributes</b></p>
-</div>
+# VIPickle
 
-## Quickstart
+VIPicle permet de sauvegarder des instances de classes qui ont des attributs non "picklable".
 
-Install `vipickle` with pip :
+## Démarrage
+
+Installation de `vipickle` avec pip :
 
 ```bash
 pip install vipickle
 ```
 
-Then inherit from `VIPicklable` and define which attribute are not picklable and how they should be dumped and restored.
+Il vous suffit ensuite d'hériter de la classe VIPicklable `VIPicklable` et de spécifier les attributs qui ne doivent pas
+être "picklés".
+
+Vous pouvez également spécifier des fonctions de sauvegarder et de chargement alternatives pour ces attributs afin de
+restaurer l'instance.
 
 ```python
 import torch
 from torchvision import models
 from pathlib import Path
 
 from vipickle import VIPicklable
@@ -59,26 +50,26 @@
 del obj
 
 # we can then reload the object, _restore_vision_model_ will recreate the attribute vision_model and load the weights
 obj = MyClass.load("a/folder")
 obj.vision_model.eval()
 ```
 
-## Additionnal dependencies
+## Dépendances optionnelles
 
-#### Dev dependencies
+#### Dépendances de développement
 
 ```bash
 pip install vipickle[dev]
 ```
 
-#### Unit tests dependencies
+#### Dépendances de test
 
 ```bash
 pip install vipickle[test]
 ```
 
-#### Documentation dependencies
+#### Dépendances de documentation
 
 ```bash
 pip install vipickle[doc]
 ```
```

### Comparing `vipickle-0.1.0/docs/gen_ref_pages.py` & `vipickle-0.1.0a0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `vipickle-0.1.0/mkdocs.yml` & `vipickle-0.1.0a0/mkdocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 site_name: VIPickle
 repo_name: h4c5/vipickle
-site_url: https://h4c5.github.io/vipickle
 repo_url: https://github.com/h4c5/vipickle
 edit_uri: edit/main/docs/
 
 # see
 theme:
     name: material
     logo: assets/images/logo.svg
@@ -20,28 +19,28 @@
         - scheme: slate
           toggle:
               icon: material/weather-sunny
               name: Switch to dark mode
           primary: amber
     features:
         - content.code.annotate
-        - navigation.tabs
-        - navigation.top
 
 nav:
-    - Overview: index.md
-    - Features:
-          - Blacklisting: features/blacklist.md
-          - Saving: features/saving.md
-          - Loading: features/loading.md
-          - Config file: features/config.md
-    - Example:
-          - Pytorch model wrapper: examples/pytorch.md
+    - Home: index.md
     - Code Reference: reference/
 
+extra:
+    alternate:
+        - name: English
+          link: /
+          lang: en
+        - name: Français
+          link: /fr/
+          lang: fr
+
 plugins:
     - search
     - gen-files:
           scripts:
               - docs/gen_ref_pages.py
     - literate-nav:
           nav_file: SUMMARY.md
@@ -50,22 +49,14 @@
           handlers:
               python:
                   options:
                       docstring_style: google
                       show_docstring_attributes: true
 
 markdown_extensions:
-    - admonition
-    - pymdownx.details
     - pymdownx.highlight:
           anchor_linenums: true
           line_spans: __span
           pygments_lang_class: true
     - pymdownx.inlinehilite
     - pymdownx.snippets
-    - pymdownx.tasklist:
-          custom_checkbox: true
-    - pymdownx.superfences:
-          custom_fences:
-              - name: mermaid
-                class: mermaid
-                format: !!python/name:pymdownx.superfences.fence_code_format
+    - pymdownx.superfences
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vipickle-0.1.0/pyproject.toml` & `vipickle-0.1.0a0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -9,28 +9,20 @@
     { name = "Hakim Cheikh", email = "hakimcheikh@yahoo.fr" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
 dependencies = ["loguru", "orjson"]
 dynamic = ["version"]
-classifiers = [
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
 
 [project.urls]
 homepage = "https://github.com/h4c5/vipickle"
-documentation = "https://h4c5.github.io/vipickle"
+documentation = "https://github.com/h4c5/vipickle"
 repository = "https://github.com/h4c5/vipickle"
-"Bug Tracker" = "https://github.com/h4c5/vipickle/issues"
+"Bug Tracker" = "https://github.com/h4c5/vipickle"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
 write_to = "src/vipickle/_version.py"
```

### Comparing `vipickle-0.1.0/src/vipickle/mixin.py` & `vipickle-0.1.0a0/src/vipickle/mixin.py`

 * *Files identical despite different names*

### Comparing `vipickle-0.1.0/src/vipickle/save_utils.py` & `vipickle-0.1.0a0/src/vipickle/save_utils.py`

 * *Files identical despite different names*

### Comparing `vipickle-0.1.0/src/vipickle.egg-info/PKG-INFO` & `vipickle-0.1.0a0/src/vipickle.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 Metadata-Version: 2.1
 Name: vipickle
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: vipickle is a tiny python package for saving instances with unpickable attributes
 Author-email: Hakim Cheikh <hakimcheikh@yahoo.fr>
 Project-URL: homepage, https://github.com/h4c5/vipickle
-Project-URL: documentation, https://h4c5.github.io/vipickle
+Project-URL: documentation, https://github.com/h4c5/vipickle
 Project-URL: repository, https://github.com/h4c5/vipickle
-Project-URL: Bug Tracker, https://github.com/h4c5/vipickle/issues
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Project-URL: Bug Tracker, https://github.com/h4c5/vipickle
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: doc
 
 <div align="center">
     <img src="https://img.shields.io/pypi/v/vipickle" alt="vipickle package version" />
     <img src="https://img.shields.io/pypi/pyversions/vipickle" alt="Python supported versions" />
-    <a href="https://github.com/h4c5/vipickle/actions/workflows/unit-tests.yml">
-        <img src="https://github.com/h4c5/vipickle/actions/workflows/unit-tests.yml/badge.svg" alt="unit tests status" />
-    </a>
     <a href="https://github.com/PyCQA/bandit">
         <img src="https://img.shields.io/badge/security-bandit-yellow.svg" alt="Security thanks to bandit package" />
     </a>
     <img src="https://img.shields.io/badge/formatting-black-black" alt="Black formatting" />
 </div>
 
 <div align="center">
```

### Comparing `vipickle-0.1.0/src/vipickle.egg-info/SOURCES.txt` & `vipickle-0.1.0a0/src/vipickle.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,21 @@
 .gitignore
 Makefile
 README.md
 mkdocs.yml
 noxfile.py
 pyproject.toml
 setup.py
-.github/workflows/build-mkdocs.yml
 .github/workflows/python-publish.yml
-.github/workflows/unit-tests.yml
 docs/gen_ref_pages.py
 docs/index.md
 docs/reference.md
 docs/assets/images/icon.svg
 docs/assets/images/logo.svg
-docs/examples/pytorch.md
-docs/features/blacklist.md
-docs/features/config.md
-docs/features/loading.md
-docs/features/saving.md
+docs/fr/index.md
 src/vipickle/__init__.py
 src/vipickle/_version.py
 src/vipickle/errors.py
 src/vipickle/mixin.py
 src/vipickle/save_utils.py
 src/vipickle.egg-info/PKG-INFO
 src/vipickle.egg-info/SOURCES.txt
```

### Comparing `vipickle-0.1.0/tests/test_mixin.py` & `vipickle-0.1.0a0/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `vipickle-0.1.0/tests/test_save_utils.py` & `vipickle-0.1.0a0/tests/test_save_utils.py`

 * *Files identical despite different names*

