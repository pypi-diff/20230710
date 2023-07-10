# Comparing `tmp/control_parameters_step-2023.1.23.tar.gz` & `tmp/control_parameters_step-2023.7.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control_parameters_step-2023.1.23.tar", last modified: Tue Jan 24 00:00:36 2023, max compression
+gzip compressed data, was "control_parameters_step-2023.7.10.tar", last modified: Mon Jul 10 20:55:07 2023, max compression
```

## Comparing `control_parameters_step-2023.1.23.tar` & `control_parameters_step-2023.7.10.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.801575 control_parameters_step-2023.1.23/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-01-24 00:00:36.801575 control_parameters_step-2023.1.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.801575 control_parameters_step-2023.1.23/control_parameters_step/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/control_parameters_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-01-24 00:00:36.801575 control_parameters_step-2023.1.23/control_parameters_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/control_parameters_step/control_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/control_parameters_step/control_parameters_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/control_parameters_step/control_parameters_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.793575 control_parameters_step-2023.1.23/control_parameters_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/control_parameters_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/control_parameters_step/tk_control_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.793575 control_parameters_step-2023.1.23/control_parameters_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-01-24 00:00:36.000000 control_parameters_step-2023.1.23/control_parameters_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-01-24 00:00:36.000000 control_parameters_step-2023.1.23/control_parameters_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 00:00:36.000000 control_parameters_step-2023.1.23/control_parameters_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-24 00:00:36.000000 control_parameters_step-2023.1.23/control_parameters_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-24 00:00:36.000000 control_parameters_step-2023.1.23/control_parameters_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-24 00:00:36.000000 control_parameters_step-2023.1.23/control_parameters_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 00:00:24.000000 control_parameters_step-2023.1.23/control_parameters_step.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.797575 control_parameters_step-2023.1.23/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.797575 control_parameters_step-2023.1.23/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.797575 control_parameters_step-2023.1.23/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9674 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.797575 control_parameters_step-2023.1.23/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.797575 control_parameters_step-2023.1.23/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)   451979 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/getting_started/dialog.png
--rw-r--r--   0 runner    (1001) docker     (123)   127077 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   897145 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/getting_started/run.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.797575 control_parameters_step-2023.1.23/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-01-24 00:00:36.801575 control_parameters_step-2023.1.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:36.797575 control_parameters_step-2023.1.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/tests/test_control_parameters_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-01-24 00:00:22.000000 control_parameters_step-2023.1.23/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.683502 control_parameters_step-2023.7.10/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-10 20:55:07.683502 control_parameters_step-2023.7.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.683502 control_parameters_step-2023.7.10/control_parameters_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/control_parameters_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-10 20:55:07.683502 control_parameters_step-2023.7.10/control_parameters_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14674 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/control_parameters_step/control_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/control_parameters_step/control_parameters_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/control_parameters_step/control_parameters_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.671502 control_parameters_step-2023.7.10/control_parameters_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/control_parameters_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/control_parameters_step/tk_control_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.671502 control_parameters_step-2023.7.10/control_parameters_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-10 20:55:07.000000 control_parameters_step-2023.7.10/control_parameters_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-10 20:55:07.000000 control_parameters_step-2023.7.10/control_parameters_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:55:07.000000 control_parameters_step-2023.7.10/control_parameters_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 20:55:07.000000 control_parameters_step-2023.7.10/control_parameters_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 20:55:07.000000 control_parameters_step-2023.7.10/control_parameters_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 20:55:07.000000 control_parameters_step-2023.7.10/control_parameters_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:54:52.000000 control_parameters_step-2023.7.10/control_parameters_step.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.675502 control_parameters_step-2023.7.10/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.675502 control_parameters_step-2023.7.10/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.675502 control_parameters_step-2023.7.10/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9674 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.679502 control_parameters_step-2023.7.10/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.679502 control_parameters_step-2023.7.10/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)   451979 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/getting_started/dialog.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127077 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/getting_started/flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   897145 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/getting_started/run.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.679502 control_parameters_step-2023.7.10/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 20:55:07.683502 control_parameters_step-2023.7.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:55:07.683502 control_parameters_step-2023.7.10/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/tests/test_control_parameters_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-10 20:54:49.000000 control_parameters_step-2023.7.10/versioneer.py
```

### Comparing `control_parameters_step-2023.1.23/CONTRIBUTING.rst` & `control_parameters_step-2023.7.10/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/HISTORY.rst` & `control_parameters_step-2023.7.10/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2023.7.10: Bugfix handling parameters with 0+ values
+
+   * The default was not correctly handled for control parameters with 0+ arguments,
+     where they need to be a list.
+     
 2023.1.23: Fixed issue with  parameters with '_'
 ------------------------------------------------
 
 * Fixed issue with '-' and '_' in parameter/variable names
 
 * Revamped documentation to the new MolSSI style and diátaxis layout.
```

### Comparing `control_parameters_step-2023.1.23/LICENSE` & `control_parameters_step-2023.7.10/LICENSE`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/PKG-INFO` & `control_parameters_step-2023.7.10/control_parameters_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: control_parameters_step
-Version: 2023.1.23
+Name: control-parameters-step
+Version: 2023.7.10
 Summary: A SEAMM plug-in for defining command-line parameters for a flowchart.
 Home-page: https://github.com/molssi-seamm/control_parameters_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart
 Platform: Linux
@@ -116,14 +116,19 @@
 
 
 
 =======
 History
 =======
 
+2023.7.10: Bugfix handling parameters with 0+ values
+
+   * The default was not correctly handled for control parameters with 0+ arguments,
+     where they need to be a list.
+     
 2023.1.23: Fixed issue with  parameters with '_'
 ------------------------------------------------
 
 * Fixed issue with '-' and '_' in parameter/variable names
 
 * Revamped documentation to the new MolSSI style and diátaxis layout.
```

### Comparing `control_parameters_step-2023.1.23/README.rst` & `control_parameters_step-2023.7.10/README.rst`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/control_parameters_step/__init__.py` & `control_parameters_step-2023.7.10/control_parameters_step/__init__.py`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/control_parameters_step/control_parameters.py` & `control_parameters_step-2023.7.10/control_parameters_step/control_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
             "help": "The temperature"
         },
 """
 
 import json
 import logging
 import pprint  # noqa: F401
+import shlex
 import textwrap
 
 from tabulate import tabulate
 
 import control_parameters_step
 import seamm
 import seamm_util
@@ -418,15 +419,18 @@
 
         variables = self.parameters["variables"].value
 
         # plugins = parser.add_argument_group('plug-ins')
         for dest, data in variables.items():
             data_type = data["type"]
             type_ = types[data_type]
-            default = type_(data["default"])
+            if "more" in data["nargs"]:
+                default = [type_(i) for i in shlex.split(data["default"])]
+            else:
+                default = type_(data["default"])
             if data["optional"] == "Yes":
                 name = "--" + dest
             else:
                 name = dest
             nargs = nargs_values[data["nargs"]]
             choices = data["choices"]
             if choices == "":
```

### Comparing `control_parameters_step-2023.1.23/control_parameters_step/control_parameters_parameters.py` & `control_parameters_step-2023.7.10/control_parameters_step/control_parameters_parameters.py`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/control_parameters_step/control_parameters_step.py` & `control_parameters_step-2023.7.10/control_parameters_step/control_parameters_step.py`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/control_parameters_step/data/references.bib` & `control_parameters_step-2023.7.10/control_parameters_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/control_parameters_step/tk_control_parameters.py` & `control_parameters_step-2023.7.10/control_parameters_step/tk_control_parameters.py`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/control_parameters_step.egg-info/PKG-INFO` & `control_parameters_step-2023.7.10/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: control-parameters-step
-Version: 2023.1.23
+Name: control_parameters_step
+Version: 2023.7.10
 Summary: A SEAMM plug-in for defining command-line parameters for a flowchart.
 Home-page: https://github.com/molssi-seamm/control_parameters_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart
 Platform: Linux
@@ -116,14 +116,19 @@
 
 
 
 =======
 History
 =======
 
+2023.7.10: Bugfix handling parameters with 0+ values
+
+   * The default was not correctly handled for control parameters with 0+ arguments,
+     where they need to be a list.
+     
 2023.1.23: Fixed issue with  parameters with '_'
 ------------------------------------------------
 
 * Fixed issue with '-' and '_' in parameter/variable names
 
 * Revamped documentation to the new MolSSI style and diátaxis layout.
```

### Comparing `control_parameters_step-2023.1.23/control_parameters_step.egg-info/SOURCES.txt` & `control_parameters_step-2023.7.10/control_parameters_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/Makefile` & `control_parameters_step-2023.7.10/docs/Makefile`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/_static/SEAMM inverted.png` & `control_parameters_step-2023.7.10/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/_static/SEAMM logo.png` & `control_parameters_step-2023.7.10/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/_static/molssi_main_logo.png` & `control_parameters_step-2023.7.10/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/_static/molssi_main_logo_inverted_white.png` & `control_parameters_step-2023.7.10/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/_static/molssi_square.png` & `control_parameters_step-2023.7.10/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/_static/nsf.png` & `control_parameters_step-2023.7.10/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/conf.py` & `control_parameters_step-2023.7.10/docs/conf.py`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/developer_guide/installation.rst` & `control_parameters_step-2023.7.10/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/getting_started/dialog.png` & `control_parameters_step-2023.7.10/docs/getting_started/dialog.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/getting_started/flowchart.png` & `control_parameters_step-2023.7.10/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/getting_started/index.rst` & `control_parameters_step-2023.7.10/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/getting_started/run.png` & `control_parameters_step-2023.7.10/docs/getting_started/run.png`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/index.rst` & `control_parameters_step-2023.7.10/docs/index.rst`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/make.bat` & `control_parameters_step-2023.7.10/docs/make.bat`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/docs/user_guide/index.rst` & `control_parameters_step-2023.7.10/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/setup.py` & `control_parameters_step-2023.7.10/setup.py`

 * *Files identical despite different names*

### Comparing `control_parameters_step-2023.1.23/versioneer.py` & `control_parameters_step-2023.7.10/versioneer.py`

 * *Files identical despite different names*

