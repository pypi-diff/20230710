# Comparing `tmp/dotfgen-1.0.0a2.tar.gz` & `tmp/dotfgen-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotfgen-1.0.0a2.tar", max compression
+gzip compressed data, was "dotfgen-1.0.0a3.tar", max compression
```

## Comparing `dotfgen-1.0.0a2.tar` & `dotfgen-1.0.0a3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35053 2023-07-10 08:39:00.913705 dotfgen-1.0.0a2/LICENSE
-drwxr-xr-x   0        0        0        0 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/LICENSES/
--rw-r--r--   0        0        0      400 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/README.md
--rw-r--r--   0        0        0    22351 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-10 08:39:00.914705 dotfgen-1.0.0a2/src/dotfgen/__init__.py
--rw-r--r--   0        0        0      238 2023-07-10 08:39:00.915705 dotfgen-1.0.0a2/src/dotfgen/__main__.py
--rw-r--r--   0        0        0     3872 2023-07-10 08:39:00.915705 dotfgen-1.0.0a2/src/dotfgen/cli.py
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 dotfgen-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0    35053 2023-07-10 08:53:58.106519 dotfgen-1.0.0a3/LICENSE
+drwxr-xr-x   0        0        0        0 2023-07-10 08:53:58.107519 dotfgen-1.0.0a3/LICENSES/
+-rw-r--r--   0        0        0      402 2023-07-10 08:53:58.107519 dotfgen-1.0.0a3/README.md
+-rw-r--r--   0        0        0    22351 2023-07-10 08:53:58.107519 dotfgen-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-10 08:53:58.108518 dotfgen-1.0.0a3/src/dotfgen/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-10 08:53:58.108518 dotfgen-1.0.0a3/src/dotfgen/__main__.py
+-rw-r--r--   0        0        0     3872 2023-07-10 08:53:58.108518 dotfgen-1.0.0a3/src/dotfgen/cli.py
+-rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 dotfgen-1.0.0a3/PKG-INFO
```

### Comparing `dotfgen-1.0.0a2/LICENSE` & `dotfgen-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `dotfgen-1.0.0a2/pyproject.toml` & `dotfgen-1.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2019 Rémy Taymans <remytms@tsmail.eu>
 #
 # SPDX-License-Identifier: CC0-1.0
 
 [tool.poetry]
 name = "dotfgen"
-version = "1.0.0a2"
+version = "1.0.0a3"
 description = "Generate dotfiles based on a template. dotfgen lets you anonymise your dotfiles."
 authors = ["Rémy Taymans <remytms@tsmail.eu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/remytms/dotfgen"
 keywords = ["dotfiles", "generator", "unix"]
 classifiers = [
```

### Comparing `dotfgen-1.0.0a2/src/dotfgen/cli.py` & `dotfgen-1.0.0a3/src/dotfgen/cli.py`

 * *Files identical despite different names*

### Comparing `dotfgen-1.0.0a2/PKG-INFO` & `dotfgen-1.0.0a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotfgen
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Generate dotfiles based on a template. dotfgen lets you anonymise your dotfiles.
 Home-page: https://gitlab.com/remytms/dotfgen
 License: GPL-3.0-or-later
 Keywords: dotfiles,generator,unix
 Author: Rémy Taymans
 Author-email: remytms@tsmail.eu
 Requires-Python: >=3.7,<4.0
@@ -26,15 +26,15 @@
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: sh (>=1.14.3,<2.0.0)
 Project-URL: Bug Tracker, https://gitlab.com/remytms/dotfgen/-/issues
 Project-URL: Repository, https://gitlab.com/remytms/dotfgen
 Description-Content-Type: text/markdown
 
-[![pipeline status](https://gitlab.com/remytms/dotfgen/badges/dev/pipeline.svg)](https://gitlab.com/remytms/dotfgen/commits/dev)
+[![pipeline status](https://gitlab.com/remytms/dotfgen/badges/main/pipeline.svg)](https://gitlab.com/remytms/dotfgen/commits/main)
 
 dotfgen
 =======
 
 dotfgen is a cli program that generates files based on a template file.
 It lets you anonymise your configuration files before sharing it with
 the rest of the world.
```

