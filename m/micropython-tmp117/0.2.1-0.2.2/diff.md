# Comparing `tmp/micropython-tmp117-0.2.1.tar.gz` & `tmp/micropython-tmp117-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-tmp117-0.2.1.tar", last modified: Sat Jun 17 14:40:42 2023, max compression
+gzip compressed data, was "micropython-tmp117-0.2.2.tar", last modified: Sun Jul  9 22:06:52 2023, max compression
```

## Comparing `micropython-tmp117-0.2.1.tar` & `micropython-tmp117-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.670043 micropython-tmp117-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.670043 micropython-tmp117-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp117_alert_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp117_averaging_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp117_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp177_temperature_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/micropython_tmp117/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/micropython_tmp117/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/micropython_tmp117/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/micropython_tmp117/tmp117.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.068084 micropython-tmp117-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.064084 micropython-tmp117-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.064084 micropython-tmp117-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-09 22:06:52.068084 micropython-tmp117-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.064084 micropython-tmp117-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.064084 micropython-tmp117-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.068084 micropython-tmp117-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/examples/tmp117_alert_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/examples/tmp117_averaging_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/examples/tmp117_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/examples/tmp177_temperature_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.068084 micropython-tmp117-0.2.2/micropython_tmp117/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/micropython_tmp117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/micropython_tmp117/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/micropython_tmp117/tmp117.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:06:52.068084 micropython-tmp117-0.2.2/micropython_tmp117.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-09 22:06:52.000000 micropython-tmp117-0.2.2/micropython_tmp117.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-09 22:06:52.000000 micropython-tmp117-0.2.2/micropython_tmp117.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:06:52.000000 micropython-tmp117-0.2.2/micropython_tmp117.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 22:06:52.000000 micropython-tmp117-0.2.2/micropython_tmp117.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-09 22:06:42.000000 micropython-tmp117-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-09 22:06:29.000000 micropython-tmp117-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 22:06:52.068084 micropython-tmp117-0.2.2/setup.cfg
```

### Comparing `micropython-tmp117-0.2.1/.gitignore` & `micropython-tmp117-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.1/.pre-commit-config.yaml` & `micropython-tmp117-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.1/LICENSE` & `micropython-tmp117-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.1/PKG-INFO` & `micropython-tmp117-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-tmp117
-Version: 0.2.1
+Version: 0.2.2
 Summary: MicroPython Driver for the TMP117 temperature sensor
 Author-email: "Jose D. Montoya" <tmp117@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/micropython_TMP117
 Keywords: micropython,tmp117,temperature,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -38,18 +38,14 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the TMP117 temperature sensor
 
-Register reding based on
-https://github.com/adafruit/Adafruit_CircuitPython_Register
-
-
 Installing with mip
 ====================
 
 To install using mpremote
 
 .. code-block:: shell
```

### Comparing `micropython-tmp117-0.2.1/README.rst` & `micropython-tmp117-0.2.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -21,18 +21,14 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the TMP117 temperature sensor
 
-Register reding based on
-https://github.com/adafruit/Adafruit_CircuitPython_Register
-
-
 Installing with mip
 ====================
 
 To install using mpremote
 
 .. code-block:: shell
```

### Comparing `micropython-tmp117-0.2.1/docs/_static/Logo.png` & `micropython-tmp117-0.2.2/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.1/docs/_static/favicon.ico` & `micropython-tmp117-0.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.1/docs/conf.py` & `micropython-tmp117-0.2.2/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,34 @@
-# -*- coding: utf-8 -*-
-
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
 import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
+try:
+    # Inject mock modules so that we can build the
+    # documentation without having the real stuff available
+    from mock import Mock
+
+    to_be_mocked = [
+        "micropython",
+        "machine",
+    ]
+    for module in to_be_mocked:
+        sys.modules[module] = Mock()
+        print("Mocked '{}' module".format(module))
+
+    import micropython_tmp117
+except ImportError:
+    raise SystemExit("micropython_tmp117 has to be importable")
+
 # -- General configuration ------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
@@ -56,26 +71,16 @@
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
 release = "1.0"
 html_baseurl = "https://micropython-tmp117.readthedocs.io/"
 language = "en"
 
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "requirements.txt"]
-
-# The reST default role (used for this markup: `text`) to use for all
-# documents.
-#
 default_role = "any"
-
-# If true, '()' will be appended to :func: etc. cross-reference text.
-#
 add_function_parentheses = True
 
 rst_prolog = """
 .. role:: python(code)
    :language: python
    :class: highlight
 .. default-literal-role:: python
@@ -200,40 +205,14 @@
 #
 html_favicon = "_static/favicon.ico"
 
 html_logo = "_static/Logo.png"
 # Output file base name for HTML help builder.
 htmlhelp_basename = "Micropython_Tmp117_Librarydoc"
 
-# -- Options for LaTeX output ---------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "Micropython_TMP117_Library.tex",
-        "Micropython TMP117 Library Documentation",
-        author,
-        "manual",
-    ),
-]
-
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     (
         master_doc,
```

### Comparing `micropython-tmp117-0.2.1/examples/tmp117_alert_mode.py` & `micropython-tmp117-0.2.2/examples/tmp117_alert_mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 
 import time
 from machine import Pin, I2C
-import micropython_tmp117.tmp117 as tmp117
+from micropython_tmp117 import tmp117
 
 i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
 tmp = tmp117.TMP117(i2c)
 
 tmp.high_limit = 23
 tmp.low_limit = 20
 
 print("Alert mode:", tmp.alert_mode)
 print("High limit", tmp.high_limit)
 print("Low limit", tmp.low_limit)
 
 
 while True:
-    print("Temperature: %.2f degrees C" % tmp.temperature)
+    print(f"Alert status: {tmp.alert_status:.2f}°C")
     alert_status = tmp.alert_status
     if alert_status.high_alert:
         print("Temperature above high set limit!")
     if alert_status.low_alert:
         print("Temperature below low set limit!")
     print("Low alert:", alert_status.low_alert)
     time.sleep(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-tmp117-0.2.1/examples.json` & `micropython-tmp117-0.2.2/examples.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'version'": "'1'"}*

```diff
@@ -13,9 +13,9 @@
             "github:jposada202020/MicroPython_TMP117/examples/tmp117_averaging_measurements.py"
         ],
         [
             "micropython_tmp117/examples/tmp117_simpletest.py",
             "github:jposada202020/MicroPython_TMP117/examples/tmp117_simpletest.py"
         ]
     ],
-    "version": "0.1"
+    "version": "1"
 }
```

### Comparing `micropython-tmp117-0.2.1/micropython_tmp117/i2c_helpers.py` & `micropython-tmp117-0.2.2/micropython_tmp117/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.1/micropython_tmp117/tmp117.py` & `micropython-tmp117-0.2.2/micropython_tmp117/tmp117.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 **Software and Dependencies:**
 
 This library depends on Micropython
 
 """
 
-# pylint: disable=too-many-arguments, line-too-long
+# pylint: disable=line-too-long
 
 import time
 from collections import namedtuple
 from micropython import const
 from micropython_tmp117.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __repo__ = "https://github.com/jposada202020/MicroPython_TMP117.git"
 
 
 _REG_WHOAMI = const(0x0F)
 _TEMP_RESULT = const(0x00)
 _CONFIGURATION = const(0x01)
 _TEMP_HIGH_LIMIT = const(0x02)
@@ -49,14 +49,15 @@
 ALERT_HYSTERESIS = const(1)
 
 # Conversion Averaging Mode
 AVERAGE_1X = const(0b00)
 AVERAGE_8X = const(0b01)
 AVERAGE_32X = const(0b10)
 AVERAGE_64X = const(0b11)
+averaging_measurements_values = (AVERAGE_1X, AVERAGE_8X, AVERAGE_32X, AVERAGE_64X)
 
 
 class TMP117:
     """Main class for the Sensor
 
     :param ~machine.I2C i2c: The I2C bus the TMP117 is connected to.
     :param int address: The I2C device address. Defaults to :const:`0x48`
@@ -68,15 +69,15 @@
 
     Here is an example of using the :class:`TMP117` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import micropython_tmp117.tmp117 as tmp117
+        import micropython_tmp117 import tmp117
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
         i2c = I2C(sda=Pin(8), scl=Pin(9))
         tmp117 = tmp117.TMP117(i2c)
@@ -112,15 +113,15 @@
 
     _avg_3 = {0: 1, 1: 1, 2: 1, 3: 1, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_2 = {0: 0.5, 1: 0.5, 2: 0.5, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_1 = {0: 0.125, 1: 0.125, 2: 0.25, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_0 = {0: 0.0155, 1: 0.125, 2: 0.25, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
     _averaging_modes = {0: _avg_0, 1: _avg_1, 2: _avg_2, 3: _avg_3}
 
-    def __init__(self, i2c, address=0x48):
+    def __init__(self, i2c, address=0x48) -> None:
         self._i2c = i2c
         self._address = address
         self._valide_range = range(-256, 255)
 
         if self._device_id != 0x117:
             raise RuntimeError("Failed to find TMP117!")
 
@@ -134,21 +135,21 @@
         )
         self._mode = CONTINUOUS_CONVERSION_MODE
         while not self._data_ready:
             time.sleep(0.001)
         _ = self._raw_temperature * _TMP117_RESOLUTION
 
     @property
-    def temperature(self):
+    def temperature(self) -> float:
         """The current measured temperature in Celsius"""
 
         return self._raw_temperature * _TMP117_RESOLUTION
 
     @property
-    def temperature_offset(self):
+    def temperature_offset(self) -> float:
         """User defined temperature offset to be added to measurements from `temperature`.
         In order the see the new change in the temperature we need for the data to be ready.
         There is a time delay calculated according to current configuration.
 
         .. code-block::python
 
             from machine import Pin, I2C
@@ -161,55 +162,56 @@
             tmp117.temperature_offset = 10.0
             print("Temperature with offset: ", tmp.temperature)
 
         """
         return self._raw_temperature_offset * _TMP117_RESOLUTION
 
     @temperature_offset.setter
-    def temperature_offset(self, value: float):
-
+    def temperature_offset(self, value: float) -> None:
         self._raw_temperature_offset = self.validate_value(value)
         time.sleep(
             self._averaging_modes[self._conversion_averaging_mode][
                 self._conversion_cycle_bit
             ]
         )
 
     @property
-    def high_limit(self):
+    def high_limit(self) -> float:
         """The high temperature limit in Celsius. When the measured temperature exceeds this
-        value, the `high_alert` attribute of the `alert_status` property will be True."""
+        value, the `high_alert` attribute of the `alert_status` property will be True.
+        """
 
         return self._raw_high_limit * _TMP117_RESOLUTION
 
     @high_limit.setter
-    def high_limit(self, value: float):
+    def high_limit(self, value: float) -> None:
         self._raw_high_limit = self.validate_value(value)
 
     @property
-    def low_limit(self):
+    def low_limit(self) -> float:
         """The low  temperature limit in Celsius. When the measured temperature goes below
-        this value, the `low_alert` attribute of the `alert_status` property will be True."""
+        this value, the `low_alert` attribute of the `alert_status` property will be True.
+        """
 
         return self._raw_low_limit * _TMP117_RESOLUTION
 
     @low_limit.setter
-    def low_limit(self, value: float):
+    def low_limit(self, value: float) -> None:
         self._raw_low_limit = self.validate_value(value)
 
-    def validate_value(self, value):
+    def validate_value(self, value: int) -> int:
         """Validates for values to be in the range of :const:`-256` and :const:`255`,
         then return the value divided by the :const:`_TMP117_RESOLUTION`
         """
         if value not in self._valide_range:
             raise ValueError("Value should be within -256 and 255")
         return int(value / _TMP117_RESOLUTION)
 
     @property
-    def alert_status(self):
+    def alert_status(self) -> AlertStatus:
         """The current triggered status of the high and low temperature alerts as a AlertStatus
         named tuple with attributes for the triggered status of each alert.
 
         .. code-block :: python
 
             from machine import Pin, I2C
             import micropython_tmp117.tmp117 as tmp117
@@ -236,15 +238,15 @@
                 time.sleep(1)
 
         """
 
         return AlertStatus(high_alert=self._high_alert, low_alert=self._low_alert)
 
     @property
-    def alert_mode(self):
+    def alert_mode(self) -> str:
         """Sets the behavior of the `low_limit`, `high_limit`, and `alert_status` properties.
 
         When set to :py:const:`ALERT_WINDOW`, the `high_limit` property will unset when the
         measured temperature goes below `high_limit`. Similarly `low_limit` will be True or False
         depending on if the measured temperature is below (`False`) or above(`True`) `low_limit`.
 
         When set to :py:const:`ALERT_HYSTERESIS`, the `high_limit` property will be set to
@@ -259,46 +261,41 @@
         | :py:const:`tmp117.ALERT_WINDOW`        | :py:const:`0b0`         |
         +----------------------------------------+-------------------------+
         | :py:const:`tmp117.ALERT_HYSTERESIS`    | :py:const:`0b1`         |
         +----------------------------------------+-------------------------+
 
         """
 
-        alert_modes = {
-            0: "ALERT_WINDOW",
-            1: "ALERT_HYSTERESIS",
-        }
-
-        return alert_modes[self._raw_alert_mode]
+        values = ("ALERT_WINDOW", "ALERT_HYSTERESIS")
+        return values[self._raw_alert_mode]
 
     @alert_mode.setter
-    def alert_mode(self, value):
-
+    def alert_mode(self, value: int) -> None:
         if value not in [0, 1]:
             raise ValueError("alert_mode must be set to 0 or 1")
         self._raw_alert_mode = value
 
     @property
-    def averaging_measurements(self):
+    def averaging_measurements(self) -> str:
         """Users can configure the device to report the average of multiple temperature
         conversions with the AVG[1:0] bits to reduce noise in the conversion results.
         When the TMP117 is configured to perform averaging with AVG set to 01, the device executes
         the configured number of conversions to eight. The device accumulates those conversion
         results and reports the average of all the collected results at the end of the process.
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
-        | :py:const:`TMP117.AVERAGE_1X`          | :py:const:`0b00`        |
+        | :py:const:`tmp117.AVERAGE_1X`          | :py:const:`0b00`        |
         +----------------------------------------+-------------------------+
-        | :py:const:`TMP117.AVERAGE_8X`          | :py:const:`0b01`        |
+        | :py:const:`tmp117.AVERAGE_8X`          | :py:const:`0b01`        |
         +----------------------------------------+-------------------------+
-        | :py:const:`TMP117.AVERAGE_32X`         | :py:const:`0b10`        |
+        | :py:const:`tmp117.AVERAGE_32X`         | :py:const:`0b10`        |
         +----------------------------------------+-------------------------+
-        | :py:const:`TMP117.AVERAGE_64X`         | :py:const:`0b11`        |
+        | :py:const:`tmp117.AVERAGE_64X`         | :py:const:`0b11`        |
         +----------------------------------------+-------------------------+
 
 
         .. code-block::python3
 
             from machine import Pin, I2C
             import micropython_tmp117.tmp117 as tmp117
@@ -310,61 +307,56 @@
             print("Averaging Measurements: ",tmp.averaging_measurements)
 
             while True:
                 print("Temperature:", tmp.temperature)
                 time.sleep(1)
 
         """
-        average_measure = {
-            0: "AVERAGE_1X",
-            1: "AVERAGE_8X",
-            2: "AVERAGE_32X",
-            3: "AVERAGE_64X",
-        }
 
-        return average_measure[self._conversion_averaging_mode]
+        values = ("AVERAGE_1X", "AVERAGE_8X", "AVERAGE_32X", "AVERAGE_64X")
+        return values[self._conversion_averaging_mode]
 
     @averaging_measurements.setter
-    def averaging_measurements(self, value: int):
-        if value not in range(0, 4):
-            raise ValueError("Value must be set to 0, 1, 2 or 3")
+    def averaging_measurements(self, value: int) -> None:
+        if value not in averaging_measurements_values:
+            raise ValueError("Value must be a valid averaging_measurements setting")
         self._conversion_averaging_mode = value
 
     @property
-    def measurement_mode(self):
+    def measurement_mode(self) -> str:
         """Sets the measurement mode, specifying the behavior of how often measurements are taken.
                 `measurement_mode` must be one of:
 
         When we use the sensor in One shot mode, the sensor will take the average_measurement value
-        into account. However, this measure is done with the formula (15.5 ms × average_time), so in
+        into account. However, this measure is done with the formula (15.5 ms x average_time), so in
         normal operation average_time will be 8, therefore time for measure is 124 ms.
         (See datasheet. 7.3.2 Averaging for more information). If we use 64, time will be 15.5 x 65 = 992 ms,
         the standby time will decrease, but the measure is still under 1 Hz cycle.
         (See Fig 7.2 on the datasheet)
 
-        +----------------------------------------+------------------------------------------------------+
-        | Mode                                   | Behavior                                             |
-        +========================================+======================================================+
-        | :py:const:`MEASUREMENTMODE_CONTINUOUS` | Measurements are made at the interval determined by  |
-        |                                        | `averaging_measurements`.                            |
-        |                                        | `temperature` returns the most recent measurement    |
-        +----------------------------------------+------------------------------------------------------+
-        | :py:const:`MEASUREMENTMODE_ONE_SHOT`   | Take a single measurement with the current number of |
-        |                                        | `averaging_measurements` and switch to               |
-        |                                        | :py:const:`SHUTDOWN` when finished.                  |
-        |                                        | `temperature` will return the new measurement until  |
-        |                                        | `measurement_mode` is set to :py:const:`CONTINUOUS`  |
-        |                                        | or :py:const:`ONE_SHOT` is                           |
-        |                                        | set again.                                           |
-        +----------------------------------------+------------------------------------------------------+
-        | :py:const:`MEASUREMENTMODE_SHUTDOWN`   | The sensor is put into a low power state and no new  |
-        |                                        | measurements are taken.                              |
-        |                                        | `temperature` will return the last measurement until |
-        |                                        | a new `measurement_mode` is selected.                |
-        +----------------------------------------+------------------------------------------------------+
+        +-----------------------------------------------+------------------------------------------------------+
+        | Mode                                          | Behavior                                             |
+        +===============================================+======================================================+
+        | :py:const:`tmp117.CONTINUOUS_CONVERSION_MODE` | Measurements are made at the interval determined by  |
+        |                                               | `averaging_measurements`.                            |
+        |                                               | `temperature` returns the most recent measurement    |
+        +-----------------------------------------------+------------------------------------------------------+
+        | :py:const:`tmp117.SHUTDOWN_MODE`              | Take a single measurement with the current number of |
+        |                                               | `averaging_measurements` and switch to               |
+        |                                               | :py:const:`SHUTDOWN` when finished.                  |
+        |                                               | `temperature` will return the new measurement until  |
+        |                                               | `measurement_mode` is set to :py:const:`CONTINUOUS`  |
+        |                                               | or :py:const:`ONE_SHOT` is                           |
+        |                                               | set again.                                           |
+        +-----------------------------------------------+------------------------------------------------------+
+        | :py:const:`tmp117.ONE_SHOT_MODE`              | The sensor is put into a low power state and no new  |
+        |                                               | measurements are taken.                              |
+        |                                               | `temperature` will return the last measurement until |
+        |                                               | a new `measurement_mode` is selected.                |
+        +-----------------------------------------------+------------------------------------------------------+
 
         """
 
         sensor_modes = {
             0: "CONTINUOUS_CONVERSION_MODE",
             1: "SHUTDOWN_MODE",
             3: "ONE_SHOT_MODE",
```

### Comparing `micropython-tmp117-0.2.1/micropython_tmp117.egg-info/PKG-INFO` & `micropython-tmp117-0.2.2/micropython_tmp117.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-tmp117
-Version: 0.2.1
+Version: 0.2.2
 Summary: MicroPython Driver for the TMP117 temperature sensor
 Author-email: "Jose D. Montoya" <tmp117@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/micropython_TMP117
 Keywords: micropython,tmp117,temperature,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -38,18 +38,14 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the TMP117 temperature sensor
 
-Register reding based on
-https://github.com/adafruit/Adafruit_CircuitPython_Register
-
-
 Installing with mip
 ====================
 
 To install using mpremote
 
 .. code-block:: shell
```

### Comparing `micropython-tmp117-0.2.1/micropython_tmp117.egg-info/SOURCES.txt` & `micropython-tmp117-0.2.2/micropython_tmp117.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
 examples.json
 optional_requirements.txt
-packages.json
+package.json
 pyproject.toml
 requirements.txt
 .github/workflows/release_pypi.yml
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
@@ -25,9 +25,8 @@
 examples/tmp177_temperature_offset.py
 micropython_tmp117/__init__.py
 micropython_tmp117/i2c_helpers.py
 micropython_tmp117/tmp117.py
 micropython_tmp117.egg-info/PKG-INFO
 micropython_tmp117.egg-info/SOURCES.txt
 micropython_tmp117.egg-info/dependency_links.txt
-micropython_tmp117.egg-info/requires.txt
 micropython_tmp117.egg-info/top_level.txt
```

### Comparing `micropython-tmp117-0.2.1/pyproject.toml` & `micropython-tmp117-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-tmp117"
 description = "MicroPython Driver for the TMP117 temperature sensor"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "tmp117@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/micropython_TMP117"}
 keywords = [
     "micropython",
@@ -33,11 +33,11 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["tmp117"]
+packages = ["micropython_tmp117"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

